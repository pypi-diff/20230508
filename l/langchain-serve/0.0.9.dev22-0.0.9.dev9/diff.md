# Comparing `tmp/langchain-serve-0.0.9.dev22.tar.gz` & `tmp/langchain-serve-0.0.9.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain-serve-0.0.9.dev22.tar", last modified: Thu Apr 20 11:38:19 2023, max compression
+gzip compressed data, was "langchain-serve-0.0.9.dev9.tar", last modified: Wed Apr 19 11:45:49 2023, max compression
```

## Comparing `langchain-serve-0.0.9.dev22.tar` & `langchain-serve-0.0.9.dev9.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:38:19.371343 langchain-serve-0.0.9.dev22/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-20 11:38:12.000000 langchain-serve-0.0.9.dev22/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-20 11:38:12.000000 langchain-serve-0.0.9.dev22/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    28815 2023-04-20 11:38:19.371343 langchain-serve-0.0.9.dev22/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    27565 2023-04-20 11:38:12.000000 langchain-serve-0.0.9.dev22/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:38:19.367343 langchain-serve-0.0.9.dev22/langchain_serve.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    28815 2023-04-20 11:38:19.000000 langchain-serve-0.0.9.dev22/langchain_serve.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-04-20 11:38:19.000000 langchain-serve-0.0.9.dev22/langchain_serve.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 11:38:19.000000 langchain-serve-0.0.9.dev22/langchain_serve.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-20 11:38:19.000000 langchain-serve-0.0.9.dev22/langchain_serve.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 11:38:19.000000 langchain-serve-0.0.9.dev22/langchain_serve.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-20 11:38:19.000000 langchain-serve-0.0.9.dev22/langchain_serve.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-20 11:38:19.000000 langchain-serve-0.0.9.dev22/langchain_serve.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:38:19.367343 langchain-serve-0.0.9.dev22/lcserve/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-20 11:38:12.000000 langchain-serve-0.0.9.dev22/lcserve/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-20 11:38:18.000000 langchain-serve-0.0.9.dev22/lcserve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6197 2023-04-20 11:38:12.000000 langchain-serve-0.0.9.dev22/lcserve/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-20 11:38:12.000000 langchain-serve-0.0.9.dev22/lcserve/agent-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:38:19.363343 langchain-serve-0.0.9.dev22/lcserve/apps/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:38:19.367343 langchain-serve-0.0.9.dev22/lcserve/apps/babyagi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 11:38:12.000000 langchain-serve-0.0.9.dev22/lcserve/apps/babyagi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-04-20 11:38:12.000000 langchain-serve-0.0.9.dev22/lcserve/apps/babyagi/app.py
--rw-r--r--   0 runner    (1001) docker     (123)    13135 2023-04-20 11:38:12.000000 langchain-serve-0.0.9.dev22/lcserve/apps/babyagi/babyagi.py
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-20 11:38:12.000000 langchain-serve-0.0.9.dev22/lcserve/apps/babyagi/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:38:19.367343 langchain-serve-0.0.9.dev22/lcserve/backend/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-20 11:38:12.000000 langchain-serve-0.0.9.dev22/lcserve/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8786 2023-04-20 11:38:12.000000 langchain-serve-0.0.9.dev22/lcserve/backend/agentexecutor.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-04-20 11:38:12.000000 langchain-serve-0.0.9.dev22/lcserve/backend/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)    23204 2023-04-20 11:38:12.000000 langchain-serve-0.0.9.dev22/lcserve/backend/gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-04-20 11:38:12.000000 langchain-serve-0.0.9.dev22/lcserve/backend/nginx.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:38:19.367343 langchain-serve-0.0.9.dev22/lcserve/backend/playground/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 11:38:12.000000 langchain-serve-0.0.9.dev22/lcserve/backend/playground/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-04-20 11:38:12.000000 langchain-serve-0.0.9.dev22/lcserve/backend/playground/app.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-20 11:38:12.000000 langchain-serve-0.0.9.dev22/lcserve/backend/playground/config.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:38:19.371343 langchain-serve-0.0.9.dev22/lcserve/backend/playground/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 11:38:12.000000 langchain-serve-0.0.9.dev22/lcserve/backend/playground/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4709 2023-04-20 11:38:12.000000 langchain-serve-0.0.9.dev22/lcserve/backend/playground/utils/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-04-20 11:38:12.000000 langchain-serve-0.0.9.dev22/lcserve/backend/playground/utils/langchain_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-04-20 11:38:12.000000 langchain-serve-0.0.9.dev22/lcserve/backend/playground/utils/talk.py
--rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-04-20 11:38:12.000000 langchain-serve-0.0.9.dev22/lcserve/backend/playground/utils/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-20 11:38:12.000000 langchain-serve-0.0.9.dev22/lcserve/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-04-20 11:38:12.000000 langchain-serve-0.0.9.dev22/lcserve/customgateway.Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-20 11:38:12.000000 langchain-serve-0.0.9.dev22/lcserve/customgateway_config.yml
--rw-r--r--   0 runner    (1001) docker     (123)    17240 2023-04-20 11:38:12.000000 langchain-serve-0.0.9.dev22/lcserve/flow.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-20 11:38:12.000000 langchain-serve-0.0.9.dev22/lcserve/flow.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:38:19.363343 langchain-serve-0.0.9.dev22/lcserve/playground/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 11:38:19.371343 langchain-serve-0.0.9.dev22/lcserve/playground/babyagi/
--rw-r--r--   0 runner    (1001) docker     (123)     8721 2023-04-20 11:38:12.000000 langchain-serve-0.0.9.dev22/lcserve/playground/babyagi/playground.py
--rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-04-20 11:38:12.000000 langchain-serve-0.0.9.dev22/lcserve/playground/babyagi/user_input.py
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-20 11:38:12.000000 langchain-serve-0.0.9.dev22/lcserve/playgroundgateway_config.yml
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-20 11:38:12.000000 langchain-serve-0.0.9.dev22/lcserve/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-20 11:38:12.000000 langchain-serve-0.0.9.dev22/lcserve/servinggateway.Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-20 11:38:12.000000 langchain-serve-0.0.9.dev22/lcserve/servinggateway_config.yml
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-20 11:38:12.000000 langchain-serve-0.0.9.dev22/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 11:38:19.371343 langchain-serve-0.0.9.dev22/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-04-20 11:38:12.000000 langchain-serve-0.0.9.dev22/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 11:45:49.140065 langchain-serve-0.0.9.dev9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-19 11:45:43.000000 langchain-serve-0.0.9.dev9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-19 11:45:43.000000 langchain-serve-0.0.9.dev9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    27154 2023-04-19 11:45:49.140065 langchain-serve-0.0.9.dev9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    25905 2023-04-19 11:45:43.000000 langchain-serve-0.0.9.dev9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 11:45:49.136065 langchain-serve-0.0.9.dev9/langchain_serve.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    27154 2023-04-19 11:45:49.000000 langchain-serve-0.0.9.dev9/langchain_serve.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-04-19 11:45:49.000000 langchain-serve-0.0.9.dev9/langchain_serve.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 11:45:49.000000 langchain-serve-0.0.9.dev9/langchain_serve.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-19 11:45:49.000000 langchain-serve-0.0.9.dev9/langchain_serve.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 11:45:49.000000 langchain-serve-0.0.9.dev9/langchain_serve.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-19 11:45:49.000000 langchain-serve-0.0.9.dev9/langchain_serve.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-19 11:45:49.000000 langchain-serve-0.0.9.dev9/langchain_serve.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 11:45:49.136065 langchain-serve-0.0.9.dev9/lcserve/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-19 11:45:43.000000 langchain-serve-0.0.9.dev9/lcserve/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-19 11:45:48.000000 langchain-serve-0.0.9.dev9/lcserve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6197 2023-04-19 11:45:43.000000 langchain-serve-0.0.9.dev9/lcserve/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-19 11:45:43.000000 langchain-serve-0.0.9.dev9/lcserve/agent-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 11:45:49.136065 langchain-serve-0.0.9.dev9/lcserve/apps/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 11:45:49.136065 langchain-serve-0.0.9.dev9/lcserve/apps/babyagi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 11:45:43.000000 langchain-serve-0.0.9.dev9/lcserve/apps/babyagi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-04-19 11:45:43.000000 langchain-serve-0.0.9.dev9/lcserve/apps/babyagi/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13135 2023-04-19 11:45:43.000000 langchain-serve-0.0.9.dev9/lcserve/apps/babyagi/babyagi.py
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-19 11:45:43.000000 langchain-serve-0.0.9.dev9/lcserve/apps/babyagi/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 11:45:49.140065 langchain-serve-0.0.9.dev9/lcserve/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-19 11:45:43.000000 langchain-serve-0.0.9.dev9/lcserve/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8786 2023-04-19 11:45:43.000000 langchain-serve-0.0.9.dev9/lcserve/backend/agentexecutor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-19 11:45:43.000000 langchain-serve-0.0.9.dev9/lcserve/backend/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22891 2023-04-19 11:45:43.000000 langchain-serve-0.0.9.dev9/lcserve/backend/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-04-19 11:45:43.000000 langchain-serve-0.0.9.dev9/lcserve/backend/nginx.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 11:45:49.140065 langchain-serve-0.0.9.dev9/lcserve/backend/playground/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 11:45:43.000000 langchain-serve-0.0.9.dev9/lcserve/backend/playground/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-04-19 11:45:43.000000 langchain-serve-0.0.9.dev9/lcserve/backend/playground/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-19 11:45:43.000000 langchain-serve-0.0.9.dev9/lcserve/backend/playground/config.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 11:45:49.140065 langchain-serve-0.0.9.dev9/lcserve/backend/playground/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 11:45:43.000000 langchain-serve-0.0.9.dev9/lcserve/backend/playground/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-04-19 11:45:43.000000 langchain-serve-0.0.9.dev9/lcserve/backend/playground/utils/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-04-19 11:45:43.000000 langchain-serve-0.0.9.dev9/lcserve/backend/playground/utils/langchain_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-04-19 11:45:43.000000 langchain-serve-0.0.9.dev9/lcserve/backend/playground/utils/talk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-04-19 11:45:43.000000 langchain-serve-0.0.9.dev9/lcserve/backend/playground/utils/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-19 11:45:43.000000 langchain-serve-0.0.9.dev9/lcserve/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-04-19 11:45:43.000000 langchain-serve-0.0.9.dev9/lcserve/customgateway.Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-19 11:45:43.000000 langchain-serve-0.0.9.dev9/lcserve/customgateway_config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    16863 2023-04-19 11:45:43.000000 langchain-serve-0.0.9.dev9/lcserve/flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-19 11:45:43.000000 langchain-serve-0.0.9.dev9/lcserve/flow.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 11:45:49.136065 langchain-serve-0.0.9.dev9/lcserve/playground/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 11:45:49.140065 langchain-serve-0.0.9.dev9/lcserve/playground/babyagi/
+-rw-r--r--   0 runner    (1001) docker     (123)     8721 2023-04-19 11:45:43.000000 langchain-serve-0.0.9.dev9/lcserve/playground/babyagi/playground.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-04-19 11:45:43.000000 langchain-serve-0.0.9.dev9/lcserve/playground/babyagi/user_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-19 11:45:43.000000 langchain-serve-0.0.9.dev9/lcserve/playgroundgateway_config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-19 11:45:43.000000 langchain-serve-0.0.9.dev9/lcserve/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-19 11:45:43.000000 langchain-serve-0.0.9.dev9/lcserve/servinggateway.Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-19 11:45:43.000000 langchain-serve-0.0.9.dev9/lcserve/servinggateway_config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-19 11:45:43.000000 langchain-serve-0.0.9.dev9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 11:45:49.140065 langchain-serve-0.0.9.dev9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-04-19 11:45:43.000000 langchain-serve-0.0.9.dev9/setup.py
```

### Comparing `langchain-serve-0.0.9.dev22/LICENSE` & `langchain-serve-0.0.9.dev9/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain-serve-0.0.9.dev22/PKG-INFO` & `langchain-serve-0.0.9.dev9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,1801 +1,1698 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6c61 6e67  : 2.1.Name: lang
 00000020: 6368 6169 6e2d 7365 7276 650a 5665 7273  chain-serve.Vers
-00000030: 696f 6e3a 2030 2e30 2e39 2e64 6576 3232  ion: 0.0.9.dev22
-00000040: 0a53 756d 6d61 7279 3a20 4c61 6e67 6368  .Summary: Langch
-00000050: 6169 6e20 5365 7276 6520 2d20 7365 7276  ain Serve - serv
-00000060: 6520 796f 7572 206c 616e 6763 6861 696e  e your langchain
-00000070: 2061 7070 7320 6f6e 204a 696e 6120 4149   apps on Jina AI
-00000080: 2043 6c6f 7564 2e0a 486f 6d65 2d70 6167   Cloud..Home-pag
-00000090: 653a 2068 7474 7073 3a2f 2f67 6974 6875  e: https://githu
-000000a0: 622e 636f 6d2f 6a69 6e61 2d61 692f 6c61  b.com/jina-ai/la
-000000b0: 6e67 6368 6169 6e2d 7365 7276 652f 0a41  ngchain-serve/.A
-000000c0: 7574 686f 723a 204a 696e 6120 4149 0a41  uthor: Jina AI.A
-000000d0: 7574 686f 722d 656d 6169 6c3a 2068 656c  uthor-email: hel
-000000e0: 6c6f 406a 696e 612e 6169 0a4c 6963 656e  lo@jina.ai.Licen
-000000f0: 7365 3a20 4170 6163 6865 2032 2e30 0a44  se: Apache 2.0.D
-00000100: 6f77 6e6c 6f61 642d 5552 4c3a 2068 7474  ownload-URL: htt
-00000110: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000120: 6a69 6e61 2d61 692f 6c61 6e67 6368 6169  jina-ai/langchai
-00000130: 6e2d 7365 7276 652f 7461 6773 0a50 726f  n-serve/tags.Pro
-00000140: 6a65 6374 2d55 524c 3a20 446f 6375 6d65  ject-URL: Docume
-00000150: 6e74 6174 696f 6e2c 2068 7474 7073 3a2f  ntation, https:/
-00000160: 2f64 6f63 732e 6a69 6e61 2e61 690a 5072  /docs.jina.ai.Pr
-00000170: 6f6a 6563 742d 5552 4c3a 2053 6f75 7263  oject-URL: Sourc
-00000180: 652c 2068 7474 7073 3a2f 2f67 6974 6875  e, https://githu
-00000190: 622e 636f 6d2f 6a69 6e61 2d61 692f 6e6f  b.com/jina-ai/no
-000001a0: 770a 5072 6f6a 6563 742d 5552 4c3a 2054  w.Project-URL: T
-000001b0: 7261 636b 6572 2c20 6874 7470 733a 2f2f  racker, https://
-000001c0: 6769 7468 7562 2e63 6f6d 2f6a 696e 612d  github.com/jina-
-000001d0: 6169 2f6e 6f77 2f69 7373 7565 730a 4b65  ai/now/issues.Ke
-000001e0: 7977 6f72 6473 3a20 6a69 6e61 206c 616e  ywords: jina lan
-000001f0: 6763 6861 696e 206c 6c6d 206e 6575 7261  gchain llm neura
-00000200: 6c2d 6e65 7477 6f72 6b20 6465 6570 2d6c  l-network deep-l
-00000210: 6561 726e 696e 6720 6461 7461 2064 656d  earning data dem
-00000220: 6f63 7261 7469 7a61 7469 6f6e 0a50 6c61  ocratization.Pla
-00000230: 7466 6f72 6d3a 2055 4e4b 4e4f 574e 0a43  tform: UNKNOWN.C
-00000240: 6c61 7373 6966 6965 723a 2044 6576 656c  lassifier: Devel
-00000250: 6f70 6d65 6e74 2053 7461 7475 7320 3a3a  opment Status ::
-00000260: 2035 202d 2050 726f 6475 6374 696f 6e2f   5 - Production/
-00000270: 5374 6162 6c65 0a43 6c61 7373 6966 6965  Stable.Classifie
-00000280: 723a 2049 6e74 656e 6465 6420 4175 6469  r: Intended Audi
-00000290: 656e 6365 203a 3a20 4465 7665 6c6f 7065  ence :: Develope
-000002a0: 7273 0a43 6c61 7373 6966 6965 723a 2049  rs.Classifier: I
-000002b0: 6e74 656e 6465 6420 4175 6469 656e 6365  ntended Audience
-000002c0: 203a 3a20 4564 7563 6174 696f 6e0a 436c   :: Education.Cl
-000002d0: 6173 7369 6669 6572 3a20 496e 7465 6e64  assifier: Intend
-000002e0: 6564 2041 7564 6965 6e63 6520 3a3a 2053  ed Audience :: S
-000002f0: 6369 656e 6365 2f52 6573 6561 7263 680a  cience/Research.
-00000300: 436c 6173 7369 6669 6572 3a20 5072 6f67  Classifier: Prog
-00000310: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
-00000320: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
-00000330: 370a 436c 6173 7369 6669 6572 3a20 5072  7.Classifier: Pr
-00000340: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-00000350: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-00000360: 332e 380a 436c 6173 7369 6669 6572 3a20  3.8.Classifier: 
-00000370: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-00000380: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-00000390: 3a20 332e 390a 436c 6173 7369 6669 6572  : 3.9.Classifier
-000003a0: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
-000003b0: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-000003c0: 203a 3a20 332e 3130 0a43 6c61 7373 6966   :: 3.10.Classif
-000003d0: 6965 723a 2045 6e76 6972 6f6e 6d65 6e74  ier: Environment
-000003e0: 203a 3a20 436f 6e73 6f6c 650a 436c 6173   :: Console.Clas
-000003f0: 7369 6669 6572 3a20 4c69 6365 6e73 6520  sifier: License 
-00000400: 3a3a 204f 5349 2041 7070 726f 7665 6420  :: OSI Approved 
-00000410: 3a3a 2041 7061 6368 6520 536f 6674 7761  :: Apache Softwa
-00000420: 7265 204c 6963 656e 7365 0a43 6c61 7373  re License.Class
-00000430: 6966 6965 723a 204f 7065 7261 7469 6e67  ifier: Operating
-00000440: 2053 7973 7465 6d20 3a3a 204f 5320 496e   System :: OS In
-00000450: 6465 7065 6e64 656e 740a 436c 6173 7369  dependent.Classi
-00000460: 6669 6572 3a20 546f 7069 6320 3a3a 2053  fier: Topic :: S
-00000470: 6369 656e 7469 6669 632f 456e 6769 6e65  cientific/Engine
-00000480: 6572 696e 6720 3a3a 2041 7274 6966 6963  ering :: Artific
-00000490: 6961 6c20 496e 7465 6c6c 6967 656e 6365  ial Intelligence
-000004a0: 0a44 6573 6372 6970 7469 6f6e 2d43 6f6e  .Description-Con
-000004b0: 7465 6e74 2d54 7970 653a 2074 6578 742f  tent-Type: text/
-000004c0: 6d61 726b 646f 776e 0a4c 6963 656e 7365  markdown.License
-000004d0: 2d46 696c 653a 204c 4943 454e 5345 0a0a  -File: LICENSE..
-000004e0: 3c70 2061 6c69 676e 3d22 6365 6e74 6572  <p align="center
-000004f0: 223e 0a3c 623e 4c61 6e67 4368 6169 6e20  ">.<b>LangChain 
-00000500: 4170 7073 206f 6e20 5072 6f64 7563 7469  Apps on Producti
-00000510: 6f6e 2077 6974 6820 4a69 6e61 20f0 9f9a  on with Jina ...
-00000520: 803c 2f62 3e0a 3c2f 703e 0a0a 3c70 2061  .</b>.</p>..<p a
-00000530: 6c69 676e 3d63 656e 7465 723e 0a3c 6120  lign=center>.<a 
-00000540: 6872 6566 3d22 6874 7470 733a 2f2f 7079  href="https://py
-00000550: 7069 2e6f 7267 2f70 726f 6a65 6374 2f6c  pi.org/project/l
-00000560: 616e 6763 6861 696e 2d73 6572 7665 2f22  angchain-serve/"
-00000570: 3e3c 696d 6720 616c 743d 2250 7950 4922  ><img alt="PyPI"
-00000580: 2073 7263 3d22 6874 7470 733a 2f2f 696d   src="https://im
-00000590: 672e 7368 6965 6c64 732e 696f 2f70 7970  g.shields.io/pyp
-000005a0: 692f 762f 6c61 6e67 6368 6169 6e2d 7365  i/v/langchain-se
-000005b0: 7276 653f 6c61 6265 6c3d 5265 6c65 6173  rve?label=Releas
-000005c0: 6526 7374 796c 653d 666c 6174 2d73 7175  e&style=flat-squ
-000005d0: 6172 6522 3e3c 2f61 3e0a 3c61 2068 7265  are"></a>.<a hre
-000005e0: 663d 2268 7474 7073 3a2f 2f6a 696e 612e  f="https://jina.
-000005f0: 6169 2f73 6c61 636b 223e 3c69 6d67 2073  ai/slack"><img s
-00000600: 7263 3d22 6874 7470 733a 2f2f 696d 672e  rc="https://img.
-00000610: 7368 6965 6c64 732e 696f 2f62 6164 6765  shields.io/badge
-00000620: 2f53 6c61 636b 2d33 2e36 6b2d 626c 7565  /Slack-3.6k-blue
-00000630: 7669 6f6c 6574 3f6c 6f67 6f3d 736c 6163  violet?logo=slac
-00000640: 6b26 616d 703b 6c6f 676f 436f 6c6f 723d  k&amp;logoColor=
-00000650: 7768 6974 6526 7374 796c 653d 666c 6174  white&style=flat
-00000660: 2d73 7175 6172 6522 3e3c 2f61 3e0a 3c61  -square"></a>.<a
-00000670: 2068 7265 663d 2268 7474 7073 3a2f 2f70   href="https://p
-00000680: 7970 6973 7461 7473 2e6f 7267 2f70 6163  ypistats.org/pac
-00000690: 6b61 6765 732f 6c61 6e67 6368 6169 6e2d  kages/langchain-
-000006a0: 7365 7276 6522 3e3c 696d 6720 616c 743d  serve"><img alt=
-000006b0: 2250 7950 4920 2d20 446f 776e 6c6f 6164  "PyPI - Download
-000006c0: 7320 6672 6f6d 206f 6666 6963 6961 6c20  s from official 
-000006d0: 7079 7069 7374 6174 7322 2073 7263 3d22  pypistats" src="
-000006e0: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
-000006f0: 6c64 732e 696f 2f70 7970 692f 646d 2f6c  lds.io/pypi/dm/l
-00000700: 616e 6763 6861 696e 2d73 6572 7665 3f73  angchain-serve?s
-00000710: 7479 6c65 3d66 6c61 742d 7371 7561 7265  tyle=flat-square
-00000720: 223e 3c2f 613e 0a3c 6120 6872 6566 3d22  "></a>.<a href="
-00000730: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000740: 6f6d 2f6a 696e 612d 6169 2f6c 616e 6763  om/jina-ai/langc
-00000750: 6861 696e 2d73 6572 7665 2f61 6374 696f  hain-serve/actio
-00000760: 6e73 2f77 6f72 6b66 6c6f 7773 2f63 642e  ns/workflows/cd.
-00000770: 796d 6c22 3e3c 696d 6720 616c 743d 2247  yml"><img alt="G
-00000780: 6974 6875 6220 4344 2073 7461 7475 7322  ithub CD status"
-00000790: 2073 7263 3d22 6874 7470 733a 2f2f 6769   src="https://gi
-000007a0: 7468 7562 2e63 6f6d 2f6a 696e 612d 6169  thub.com/jina-ai
-000007b0: 2f6c 616e 6763 6861 696e 2d73 6572 7665  /langchain-serve
-000007c0: 2f61 6374 696f 6e73 2f77 6f72 6b66 6c6f  /actions/workflo
-000007d0: 7773 2f63 642e 796d 6c2f 6261 6467 652e  ws/cd.yml/badge.
-000007e0: 7376 6722 3e3c 2f61 3e0a 3c2f 703e 0a0a  svg"></a>.</p>..
-000007f0: 0a5b 4a69 6e61 5d28 6874 7470 733a 2f2f  .[Jina](https://
-00000800: 6769 7468 7562 2e63 6f6d 2f6a 696e 612d  github.com/jina-
-00000810: 6169 2f6a 696e 6129 2069 7320 616e 206f  ai/jina) is an o
-00000820: 7065 6e2d 736f 7572 6365 2066 7261 6d65  pen-source frame
-00000830: 776f 726b 2074 6f20 6275 696c 642c 2064  work to build, d
-00000840: 6570 6c6f 7920 2620 6d61 6e61 6765 206d  eploy & manage m
-00000850: 6163 6869 6e65 206c 6561 726e 696e 6720  achine learning 
-00000860: 6170 706c 6963 6174 696f 6e73 2061 7420  applications at 
-00000870: 7363 616c 652e 205b 4c61 6e67 4368 6169  scale. [LangChai
-00000880: 6e5d 2868 7474 7073 3a2f 2f70 7974 686f  n](https://pytho
-00000890: 6e2e 6c61 6e67 6368 6169 6e2e 636f 6d2f  n.langchain.com/
-000008a0: 656e 2f6c 6174 6573 742f 696e 6465 782e  en/latest/index.
-000008b0: 6874 6d6c 2920 6973 2061 6e6f 7468 6572  html) is another
-000008c0: 206f 7065 6e2d 736f 7572 6365 2066 7261   open-source fra
-000008d0: 6d65 776f 726b 2066 6f72 2062 7569 6c64  mework for build
-000008e0: 696e 6720 6170 706c 6963 6174 696f 6e73  ing applications
-000008f0: 2070 6f77 6572 6564 2062 7920 6c61 6e67   powered by lang
-00000900: 7561 6765 206d 6f64 656c 732e 200a 0a2a  uage models. ..*
-00000910: 2a6c 616e 6763 6861 696e 2d73 6572 7665  *langchain-serve
-00000920: 2a2a 2068 656c 7073 2079 6f75 2064 6570  ** helps you dep
-00000930: 6c6f 7920 796f 7572 204c 616e 6743 6861  loy your LangCha
-00000940: 696e 2061 7070 7320 6f6e 204a 696e 6120  in apps on Jina 
-00000950: 4149 2043 6c6f 7564 2069 6e20 6a75 7374  AI Cloud in just
-00000960: 2061 206d 6174 7465 7220 6f66 2073 6563   a matter of sec
-00000970: 6f6e 6473 2e20 596f 7520 6361 6e20 6e6f  onds. You can no
-00000980: 7720 6265 6e65 6669 7420 6672 6f6d 2074  w benefit from t
-00000990: 6865 2073 6361 6c61 6269 6c69 7479 2061  he scalability a
-000009a0: 6e64 2073 6572 7665 726c 6573 7320 6172  nd serverless ar
-000009b0: 6368 6974 6563 7475 7265 206f 6620 7468  chitecture of th
-000009c0: 6520 636c 6f75 6420 7769 7468 6f75 7420  e cloud without 
-000009d0: 7361 6372 6966 6963 696e 6720 7468 6520  sacrificing the 
-000009e0: 6561 7365 2061 6e64 2063 6f6e 7665 6e69  ease and conveni
-000009f0: 656e 6365 206f 6620 6c6f 6361 6c20 6465  ence of local de
-00000a00: 7665 6c6f 706d 656e 742e 0a0a 0a23 2320  velopment....## 
-00000a10: f09f a7a0 2042 6162 7961 6769 2d61 732d  .... Babyagi-as-
-00000a20: 612d 7365 7276 6963 650a 0a3e 2047 6976  a-service..> Giv
-00000a30: 6520 7573 2061 203a 7374 6172 3a20 616e  e us a :star: an
-00000a40: 6420 7465 6c6c 2075 7320 7768 6174 206d  d tell us what m
-00000a50: 6f72 6520 796f 7527 6420 6c69 6b65 2074  ore you'd like t
-00000a60: 6f20 7365 6521 200a 0a2d 2044 6570 6c6f  o see! ..- Deplo
-00000a70: 7920 6062 6162 7961 6769 6020 6f6e 204a  y `babyagi` on J
-00000a80: 696e 6120 4149 2043 6c6f 7564 2077 6974  ina AI Cloud wit
-00000a90: 6820 6f6e 6520 636f 6d6d 616e 640a 0a20  h one command.. 
-00000aa0: 2060 6060 6261 7368 0a20 206c 632d 7365   ```bash.  lc-se
-00000ab0: 7276 6520 6465 706c 6f79 2062 6162 7961  rve deploy babya
-00000ac0: 6769 0a20 2060 6060 0a0a 2d20 496e 7465  gi.  ```..- Inte
-00000ad0: 6772 6174 6520 6261 6279 6167 6920 7769  grate babyagi wi
-00000ae0: 7468 2065 7874 6572 6e61 6c20 7365 7276  th external serv
-00000af0: 6963 6573 2075 7369 6e67 206f 7572 2057  ices using our W
-00000b00: 6562 736f 636b 6574 2041 5049 2e20 4765  ebsocket API. Ge
-00000b10: 7420 6120 666c 6176 6f72 206f 6620 7468  t a flavor of th
-00000b20: 6520 696e 7465 6772 6174 696f 6e20 6f6e  e integration on
-00000b30: 2079 6f75 7220 434c 4920 7769 7468 200a   your CLI with .
-00000b40: 2020 2020 0a20 2060 6060 6261 7368 0a20      .  ```bash. 
-00000b50: 206c 632d 7365 7276 6520 706c 6179 6772   lc-serve playgr
-00000b60: 6f75 6e64 2062 6162 7961 6769 0a20 2060  ound babyagi.  `
-00000b70: 6060 0a0a 215b 4261 6279 6167 692d 6173  ``..![Babyagi-as
-00000b80: 2d61 2d73 6572 7669 6365 2050 6c61 7967  -a-service Playg
-00000b90: 726f 756e 645d 282e 6769 7468 7562 2f69  round](.github/i
-00000ba0: 6d61 6765 732f 6261 6279 6167 692d 706c  mages/babyagi-pl
-00000bb0: 6179 6772 6f75 6e64 2e67 6966 290a 0a0a  ayground.gif)...
-00000bc0: 2323 2323 20f0 9f8e 8920 4375 7374 6f6d  #### .... Custom
-00000bd0: 2041 7070 7320 746f 2070 726f 6475 6374   Apps to product
-00000be0: 696f 6e20 696e 2034 2073 696d 706c 6520  ion in 4 simple 
-00000bf0: 7374 6570 730a 0a20 2031 2e20 5265 6661  steps..  1. Refa
-00000c00: 6374 6f72 2079 6f75 7220 636f 6465 2074  ctor your code t
-00000c10: 6f20 6675 6e63 7469 6f6e 2873 2920 7468  o function(s) th
-00000c20: 6174 2073 686f 756c 6420 6265 2073 6572  at should be ser
-00000c30: 7665 6420 7769 7468 2060 4073 6572 7669  ved with `@servi
-00000c40: 6e67 6020 6465 636f 7261 746f 722e 0a20  ng` decorator.. 
-00000c50: 2031 2e20 4372 6561 7465 2061 2060 7265   1. Create a `re
-00000c60: 7175 6972 656d 656e 7473 2e74 7874 6020  quirements.txt` 
-00000c70: 6669 6c65 2069 6e20 796f 7572 2061 7070  file in your app
-00000c80: 2064 6972 6563 746f 7279 2074 6f20 656e   directory to en
-00000c90: 7375 7265 2061 6c6c 206e 6563 6573 7361  sure all necessa
-00000ca0: 7279 2064 6570 656e 6465 6e63 6965 7320  ry dependencies 
-00000cb0: 6172 6520 696e 7374 616c 6c65 642e 0a20  are installed.. 
-00000cc0: 2031 2e20 5275 6e20 606c 632d 7365 7276   1. Run `lc-serv
-00000cd0: 6520 6465 706c 6f79 206c 6f63 616c 2061  e deploy local a
-00000ce0: 7070 6020 746f 2074 6573 7420 796f 7572  pp` to test your
-00000cf0: 2041 5049 206c 6f63 616c 6c79 2e0a 2020   API locally..  
-00000d00: 312e 2052 756e 2060 6c63 2d73 6572 7665  1. Run `lc-serve
-00000d10: 2064 6570 6c6f 7920 6a63 6c6f 7564 2061   deploy jcloud a
-00000d20: 7070 6020 746f 2064 6570 6c6f 7920 6f6e  pp` to deploy on
-00000d30: 205b 4a69 6e61 2041 4920 436c 6f75 645d   [Jina AI Cloud]
-00000d40: 2868 7474 7073 3a2f 2f6a 696e 612e 6169  (https://jina.ai
-00000d50: 2f70 726f 6475 6374 2f63 6c6f 7564 2f29  /product/cloud/)
-00000d60: 2e0a 0a0a 2323 2323 20f0 9f94 a520 5363  ....#### .... Sc
-00000d70: 616c 6162 6c65 2c20 5365 7276 6572 6c65  alable, Serverle
-00000d80: 7373 2052 4553 5466 756c 2f53 7472 6561  ss RESTful/Strea
-00000d90: 6d69 6e67 2057 6562 736f 636b 6574 2041  ming Websocket A
-00000da0: 5049 7320 6f6e 204a 696e 6120 4149 2043  PIs on Jina AI C
-00000db0: 6c6f 7564 0a0a 2020 2d20 f09f 8c8e 2052  loud..  - .... R
-00000dc0: 4553 5466 756c 2f57 6562 736f 636b 6574  ESTful/Websocket
-00000dd0: 2041 5049 7320 7769 7468 2054 4c53 2063   APIs with TLS c
-00000de0: 6572 7473 2069 6e20 6a75 7374 2032 206c  erts in just 2 l
-00000df0: 696e 6573 206f 6620 636f 6465 2063 6861  ines of code cha
-00000e00: 6e67 652e 0a20 202d 20f0 9f8c 8a20 5374  nge..  - .... St
-00000e10: 7265 616d 204c 4c4d 2069 6e74 6572 6163  ream LLM interac
-00000e20: 7469 6f6e 7320 696e 2072 6561 6c2d 7469  tions in real-ti
-00000e30: 6d65 2077 6974 6820 5765 6273 6f63 6b65  me with Websocke
-00000e40: 7473 2e0a 2020 2d20 f09f 91a5 2045 6e61  ts..  - .... Ena
-00000e50: 626c 6520 6875 6d61 6e20 696e 2074 6865  ble human in the
-00000e60: 206c 6f6f 7020 666f 7220 796f 7572 2061   loop for your a
-00000e70: 6765 6e74 732e 0a20 202d 20f0 9f93 8420  gents..  - .... 
-00000e80: 5377 6167 6765 7220 5549 2c20 616e 6420  Swagger UI, and 
-00000e90: 4f70 656e 4150 4920 7370 6563 2069 6e63  OpenAPI spec inc
-00000ea0: 6c75 6465 6420 7769 7468 2079 6f75 7220  luded with your 
-00000eb0: 4150 4973 2e0a 2020 2d20 e29a a1ef b88f  APIs..  - ......
-00000ec0: 2053 6572 7665 726c 6573 7320 6170 7073   Serverless apps
-00000ed0: 2074 6861 7420 7363 616c 6573 2061 7574   that scales aut
-00000ee0: 6f6d 6174 6963 616c 6c79 2077 6974 6820  omatically with 
-00000ef0: 796f 7572 2074 7261 6666 6963 2e0a 2020  your traffic..  
-00000f00: 2d20 f09f 938a 2042 7569 6c74 696e 206c  - .... Builtin l
-00000f10: 6f67 6769 6e67 2c20 6d6f 6e69 746f 7269  ogging, monitori
-00000f20: 6e67 2c20 616e 6420 7472 6163 6573 2066  ng, and traces f
-00000f30: 6f72 2079 6f75 7220 4150 4973 2e0a 2020  or your APIs..  
-00000f40: 2d20 f09f a496 204e 6f20 6e65 6564 2074  - .... No need t
-00000f50: 6f20 6368 616e 6765 2079 6f75 7220 636f  o change your co
-00000f60: 6465 2074 6f20 6d61 6e61 6765 2041 5049  de to manage API
-00000f70: 732c 206f 7220 6d61 6e61 6765 2064 6f63  s, or manage doc
-00000f80: 6b65 7266 696c 6573 2c20 6f72 2077 6f72  kerfiles, or wor
-00000f90: 7279 2061 626f 7574 2069 6e66 7261 7374  ry about infrast
-00000fa0: 7275 6374 7572 6521 0a0a 0a23 2323 2320  ructure!...#### 
-00000fb0: f09f 9aa7 2043 6f6d 696e 6720 736f 6f6e  .... Coming soon
-00000fc0: 0a0a 2d20 5b20 5d20 f09f 9491 2041 7574  ..- [ ] .... Aut
-00000fd0: 686f 7269 7a65 2041 5049 2065 6e64 706f  horize API endpo
-00000fe0: 696e 7473 0a2d 205b 205d 20f0 9f9b a0ef  ints.- [ ] .....
-00000ff0: b88f 2045 6e61 626c 6520 5374 7265 616d  .. Enable Stream
-00001000: 6c69 7420 706c 6179 6772 6f75 6e64 2064  lit playground d
-00001010: 6570 6c6f 796d 656e 7420 666f 7220 796f  eployment for yo
-00001020: 7572 2061 7070 730a 0a0a 4966 2079 6f75  ur apps...If you
-00001030: 2068 6176 6520 616e 7920 6665 6174 7572   have any featur
-00001040: 6520 7265 7175 6573 7473 206f 7220 6661  e requests or fa
-00001050: 6365 6420 616e 7920 6973 7375 652c 2070  ced any issue, p
-00001060: 6c65 6173 6520 5b6c 6574 2075 7320 6b6e  lease [let us kn
-00001070: 6f77 5d28 6874 7470 733a 2f2f 6769 7468  ow](https://gith
-00001080: 7562 2e63 6f6d 2f6a 696e 612d 6169 2f6c  ub.com/jina-ai/l
-00001090: 616e 6763 6861 696e 2d73 6572 7665 2f69  angchain-serve/i
-000010a0: 7373 7565 732f 6e65 7729 210a 0a0a 2323  ssues/new)!...##
-000010b0: 2055 7361 6765 0a0a 4c65 7427 7320 6669   Usage..Let's fi
-000010c0: 7273 7420 696e 7374 616c 6c20 606c 616e  rst install `lan
-000010d0: 6763 6861 696e 2d73 6572 7665 6020 7573  gchain-serve` us
-000010e0: 696e 6720 7069 702e 0a0a 6060 6062 6173  ing pip...```bas
-000010f0: 680a 7069 7020 696e 7374 616c 6c20 6c61  h.pip install la
-00001100: 6e67 6368 6169 6e2d 7365 7276 650a 6060  ngchain-serve.``
-00001110: 600a 0a23 2320 456e 6162 6c65 2048 756d  `..## Enable Hum
-00001120: 616e 2d69 6e2d 7468 652d 6c6f 6f70 2028  an-in-the-loop (
-00001130: 4849 544c 2920 666f 7220 796f 7572 2061  HITL) for your a
-00001140: 6765 6e74 730a 0a48 4954 4c20 666f 7220  gents..HITL for 
-00001150: 4c61 6e67 4368 6169 6e20 6167 656e 7473  LangChain agents
-00001160: 206f 6e20 7072 6f64 7563 7469 6f6e 2063   on production c
-00001170: 616e 2062 6520 6368 616c 6c65 6e67 696e  an be challengin
-00001180: 6720 7369 6e63 6520 7468 6520 6167 656e  g since the agen
-00001190: 7473 2061 7265 2074 7970 6963 616c 6c79  ts are typically
-000011a0: 2072 756e 6e69 6e67 206f 6e20 7365 7276   running on serv
-000011b0: 6572 7320 7768 6572 6520 6875 6d61 6e73  ers where humans
-000011c0: 2064 6f6e 2774 2068 6176 6520 6469 7265   don't have dire
-000011d0: 6374 2061 6363 6573 732e 202a 2a6c 616e  ct access. **lan
-000011e0: 6763 6861 696e 2d73 6572 7665 2a2a 2062  gchain-serve** b
-000011f0: 7269 6467 6573 2074 6869 7320 6761 7020  ridges this gap 
-00001200: 6279 2065 6e61 626c 696e 6720 7765 6273  by enabling webs
-00001210: 6f63 6b65 7420 4150 4973 2074 6861 7420  ocket APIs that 
-00001220: 616c 6c6f 7720 666f 7220 7265 616c 2d74  allow for real-t
-00001230: 696d 6520 696e 7465 7261 6374 696f 6e20  ime interaction 
-00001240: 616e 6420 6665 6564 6261 636b 2062 6574  and feedback bet
-00001250: 7765 656e 2074 6865 2061 6765 6e74 2061  ween the agent a
-00001260: 6e64 2061 2068 756d 616e 206f 7065 7261  nd a human opera
-00001270: 746f 722e 0a0a 4368 6563 6b20 6f75 7420  tor...Check out 
-00001280: 7468 6973 205b 6578 616d 706c 655d 2865  this [example](e
-00001290: 7861 6d70 6c65 732f 7765 6273 6f63 6b65  xamples/websocke
-000012a0: 7473 2f68 6974 6c2f 5245 4144 4d45 2e6d  ts/hitl/README.m
-000012b0: 6429 2074 6f20 7365 6520 686f 7720 796f  d) to see how yo
-000012c0: 7520 6361 6e20 656e 6162 6c65 2048 4954  u can enable HIT
-000012d0: 4c20 666f 7220 796f 7572 2061 6765 6e74  L for your agent
-000012e0: 732e 0a0a 0a23 2320 456e 6162 6c65 2052  s....## Enable R
-000012f0: 4553 5420 4150 4973 200a 0a0a 4c65 7427  EST APIs ...Let'
-00001300: 7320 6275 696c 6420 6120 6375 7374 6f6d  s build a custom
-00001310: 2061 6765 6e74 2075 7369 6e67 2074 6869   agent using thi
-00001320: 7320 6578 616d 706c 6520 7461 6b65 6e20  s example taken 
-00001330: 6672 6f6d 205b 4c61 6e67 4368 6169 6e20  from [LangChain 
-00001340: 646f 6375 6d65 6e74 6174 696f 6e5d 2868  documentation](h
-00001350: 7474 7073 3a2f 2f70 7974 686f 6e2e 6c61  ttps://python.la
-00001360: 6e67 6368 6169 6e2e 636f 6d2f 656e 2f6c  ngchain.com/en/l
-00001370: 6174 6573 742f 6d6f 6475 6c65 732f 6167  atest/modules/ag
-00001380: 656e 7473 2f61 6765 6e74 732f 6375 7374  ents/agents/cust
-00001390: 6f6d 5f61 6765 6e74 2e68 746d 6c29 2e20  om_agent.html). 
-000013a0: 0a0a 0a3c 6465 7461 696c 733e 0a3c 7375  ...<details>.<su
-000013b0: 6d6d 6172 793e 5368 6f77 2061 6765 6e74  mmary>Show agent
-000013c0: 2063 6f64 6520 2861 7070 2e70 7929 3c2f   code (app.py)</
-000013d0: 7375 6d6d 6172 793e 0a0a 6060 6070 7974  summary>..```pyt
-000013e0: 686f 6e0a 2320 6170 702e 7079 0a66 726f  hon.# app.py.fro
-000013f0: 6d20 6c61 6e67 6368 6169 6e2e 6167 656e  m langchain.agen
-00001400: 7473 2069 6d70 6f72 7420 5a65 726f 5368  ts import ZeroSh
-00001410: 6f74 4167 656e 742c 2054 6f6f 6c2c 2041  otAgent, Tool, A
-00001420: 6765 6e74 4578 6563 7574 6f72 0a66 726f  gentExecutor.fro
-00001430: 6d20 6c61 6e67 6368 6169 6e20 696d 706f  m langchain impo
-00001440: 7274 204f 7065 6e41 492c 2053 6572 7041  rt OpenAI, SerpA
-00001450: 5049 5772 6170 7065 722c 204c 4c4d 4368  PIWrapper, LLMCh
-00001460: 6169 6e0a 0a73 6561 7263 6820 3d20 5365  ain..search = Se
-00001470: 7270 4150 4957 7261 7070 6572 2829 0a74  rpAPIWrapper().t
-00001480: 6f6f 6c73 203d 205b 0a20 2020 2054 6f6f  ools = [.    Too
-00001490: 6c28 0a20 2020 2020 2020 206e 616d 6520  l(.        name 
-000014a0: 3d20 2253 6561 7263 6822 2c0a 2020 2020  = "Search",.    
-000014b0: 2020 2020 6675 6e63 3d73 6561 7263 682e      func=search.
-000014c0: 7275 6e2c 0a20 2020 2020 2020 2064 6573  run,.        des
-000014d0: 6372 6970 7469 6f6e 3d22 7573 6566 756c  cription="useful
-000014e0: 2066 6f72 2077 6865 6e20 796f 7520 6e65   for when you ne
-000014f0: 6564 2074 6f20 616e 7377 6572 2071 7565  ed to answer que
-00001500: 7374 696f 6e73 2061 626f 7574 2063 7572  stions about cur
-00001510: 7265 6e74 2065 7665 6e74 7322 0a20 2020  rent events".   
-00001520: 2029 0a5d 0a0a 7072 6566 6978 203d 2022   ).]..prefix = "
-00001530: 2222 416e 7377 6572 2074 6865 2066 6f6c  ""Answer the fol
-00001540: 6c6f 7769 6e67 2071 7565 7374 696f 6e73  lowing questions
-00001550: 2061 7320 6265 7374 2079 6f75 2063 616e   as best you can
-00001560: 2c20 6275 7420 7370 6561 6b69 6e67 2061  , but speaking a
-00001570: 7320 6120 7069 7261 7465 206d 6967 6874  s a pirate might
-00001580: 2073 7065 616b 2e20 596f 7520 6861 7665   speak. You have
-00001590: 2061 6363 6573 7320 746f 2074 6865 2066   access to the f
-000015a0: 6f6c 6c6f 7769 6e67 2074 6f6f 6c73 3a22  ollowing tools:"
-000015b0: 2222 0a73 7566 6669 7820 3d20 2222 2242  "".suffix = """B
-000015c0: 6567 696e 2120 5265 6d65 6d62 6572 2074  egin! Remember t
-000015d0: 6f20 7370 6561 6b20 6173 2061 2070 6972  o speak as a pir
-000015e0: 6174 6520 7768 656e 2067 6976 696e 6720  ate when giving 
-000015f0: 796f 7572 2066 696e 616c 2061 6e73 7765  your final answe
-00001600: 722e 2055 7365 206c 6f74 7320 6f66 2022  r. Use lots of "
-00001610: 4172 6773 220a 0a51 7565 7374 696f 6e3a  Args"..Question:
-00001620: 207b 696e 7075 747d 0a7b 6167 656e 745f   {input}.{agent_
-00001630: 7363 7261 7463 6870 6164 7d22 2222 0a0a  scratchpad}"""..
-00001640: 7072 6f6d 7074 203d 205a 6572 6f53 686f  prompt = ZeroSho
-00001650: 7441 6765 6e74 2e63 7265 6174 655f 7072  tAgent.create_pr
-00001660: 6f6d 7074 280a 2020 2020 746f 6f6c 732c  ompt(.    tools,
-00001670: 200a 2020 2020 7072 6566 6978 3d70 7265   .    prefix=pre
-00001680: 6669 782c 200a 2020 2020 7375 6666 6978  fix, .    suffix
-00001690: 3d73 7566 6669 782c 200a 2020 2020 696e  =suffix, .    in
-000016a0: 7075 745f 7661 7269 6162 6c65 733d 5b22  put_variables=["
-000016b0: 696e 7075 7422 2c20 2261 6765 6e74 5f73  input", "agent_s
-000016c0: 6372 6174 6368 7061 6422 5d0a 290a 0a6c  cratchpad"].)..l
-000016d0: 6c6d 5f63 6861 696e 203d 204c 4c4d 4368  lm_chain = LLMCh
-000016e0: 6169 6e28 6c6c 6d3d 4f70 656e 4149 2874  ain(llm=OpenAI(t
-000016f0: 656d 7065 7261 7475 7265 3d30 292c 2070  emperature=0), p
-00001700: 726f 6d70 743d 7072 6f6d 7074 290a 746f  rompt=prompt).to
-00001710: 6f6c 5f6e 616d 6573 203d 205b 746f 6f6c  ol_names = [tool
-00001720: 2e6e 616d 6520 666f 7220 746f 6f6c 2069  .name for tool i
-00001730: 6e20 746f 6f6c 735d 0a61 6765 6e74 203d  n tools].agent =
-00001740: 205a 6572 6f53 686f 7441 6765 6e74 286c   ZeroShotAgent(l
-00001750: 6c6d 5f63 6861 696e 3d6c 6c6d 5f63 6861  lm_chain=llm_cha
-00001760: 696e 2c20 616c 6c6f 7765 645f 746f 6f6c  in, allowed_tool
-00001770: 733d 746f 6f6c 5f6e 616d 6573 290a 6167  s=tool_names).ag
-00001780: 656e 745f 6578 6563 7574 6f72 203d 2041  ent_executor = A
-00001790: 6765 6e74 4578 6563 7574 6f72 2e66 726f  gentExecutor.fro
-000017a0: 6d5f 6167 656e 745f 616e 645f 746f 6f6c  m_agent_and_tool
-000017b0: 7328 6167 656e 743d 6167 656e 742c 2074  s(agent=agent, t
-000017c0: 6f6f 6c73 3d74 6f6f 6c73 2c20 7665 7262  ools=tools, verb
-000017d0: 6f73 653d 5472 7565 290a 6167 656e 745f  ose=True).agent_
-000017e0: 6578 6563 7574 6f72 2e72 756e 2822 486f  executor.run("Ho
-000017f0: 7720 6d61 6e79 2070 656f 706c 6520 6c69  w many people li
-00001800: 7665 2069 6e20 6361 6e61 6461 2061 7320  ve in canada as 
-00001810: 6f66 2032 3032 333f 2229 0a60 6060 0a0a  of 2023?").```..
-00001820: 2323 2323 204f 7574 7075 740a 0a0a 6060  #### Output...``
-00001830: 6074 6578 740a 3e20 456e 7465 7269 6e67  `text.> Entering
-00001840: 206e 6577 2041 6765 6e74 4578 6563 7574   new AgentExecut
-00001850: 6f72 2063 6861 696e 2e2e 2e0a 5468 6f75  or chain....Thou
-00001860: 6768 743a 2049 206e 6565 6420 746f 2066  ght: I need to f
-00001870: 696e 6420 6f75 7420 7468 6520 706f 7075  ind out the popu
-00001880: 6c61 7469 6f6e 206f 6620 4361 6e61 6461  lation of Canada
-00001890: 0a41 6374 696f 6e3a 2053 6561 7263 680a  .Action: Search.
-000018a0: 4163 7469 6f6e 2049 6e70 7574 3a20 506f  Action Input: Po
-000018b0: 7075 6c61 7469 6f6e 206f 6620 4361 6e61  pulation of Cana
-000018c0: 6461 2032 3032 330a 4f62 7365 7276 6174  da 2023.Observat
-000018d0: 696f 6e3a 2054 6865 2063 7572 7265 6e74  ion: The current
-000018e0: 2070 6f70 756c 6174 696f 6e20 6f66 2043   population of C
-000018f0: 616e 6164 6120 6973 2033 382c 3631 302c  anada is 38,610,
-00001900: 3434 3720 6173 206f 6620 5361 7475 7264  447 as of Saturd
-00001910: 6179 2c20 4665 6272 7561 7279 2031 382c  ay, February 18,
-00001920: 2032 3032 332c 2062 6173 6564 206f 6e20   2023, based on 
-00001930: 576f 726c 646f 6d65 7465 7220 656c 6162  Worldometer elab
-00001940: 6f72 6174 696f 6e20 6f66 2074 6865 206c  oration of the l
-00001950: 6174 6573 7420 556e 6974 6564 204e 6174  atest United Nat
-00001960: 696f 6e73 2064 6174 612e 2043 616e 6164  ions data. Canad
-00001970: 6120 3230 3230 2070 6f70 756c 6174 696f  a 2020 populatio
-00001980: 6e20 6973 2065 7374 696d 6174 6564 2061  n is estimated a
-00001990: 7420 3337 2c37 3432 2c31 3534 2070 656f  t 37,742,154 peo
-000019a0: 706c 6520 6174 206d 6964 2079 6561 7220  ple at mid year 
-000019b0: 6163 636f 7264 696e 6720 746f 2055 4e20  according to UN 
-000019c0: 6461 7461 2e0a 5468 6f75 6768 743a 2049  data..Thought: I
-000019d0: 206e 6f77 206b 6e6f 7720 7468 6520 6669   now know the fi
-000019e0: 6e61 6c20 616e 7377 6572 0a46 696e 616c  nal answer.Final
-000019f0: 2041 6e73 7765 723a 2041 7272 722c 2043   Answer: Arrr, C
-00001a00: 616e 6164 6120 6265 2068 6176 696e 2720  anada be havin' 
-00001a10: 3338 2c36 3130 2c34 3437 2073 6361 6c6c  38,610,447 scall
-00001a20: 7977 6167 7320 6c69 7669 6e27 2074 6865  ywags livin' the
-00001a30: 7265 2061 7320 6f66 2032 3032 3321 0a0a  re as of 2023!..
-00001a40: 3e20 4669 6e69 7368 6564 2063 6861 696e  > Finished chain
-00001a50: 2e0a 6060 600a 0a3c 2f64 6574 6169 6c73  ..```..</details
-00001a60: 3e0a 0a23 2323 2053 7465 7020 313a 200a  >..### Step 1: .
-00001a70: 0a2a 2a52 6566 6163 746f 7220 796f 7572  .**Refactor your
-00001a80: 2063 6f64 6520 746f 2066 756e 6374 696f   code to functio
-00001a90: 6e28 7329 2074 6861 7420 7368 6f75 6c64  n(s) that should
-00001aa0: 2062 6520 7365 7276 6564 2077 6974 6820   be served with 
-00001ab0: 6040 7365 7276 696e 6760 2064 6563 6f72  `@serving` decor
-00001ac0: 6174 6f72 2a2a 0a0a 0a3c 6465 7461 696c  ator**...<detail
-00001ad0: 733e 0a3c 7375 6d6d 6172 793e 5368 6f77  s>.<summary>Show
-00001ae0: 2075 7064 6174 6564 2061 6765 6e74 2063   updated agent c
-00001af0: 6f64 6520 2861 7070 2e70 7929 3c2f 7375  ode (app.py)</su
-00001b00: 6d6d 6172 793e 0a0a 6060 6070 7974 686f  mmary>..```pytho
-00001b10: 6e0a 2320 6170 702e 7079 0a66 726f 6d20  n.# app.py.from 
-00001b20: 6c61 6e67 6368 6169 6e20 696d 706f 7274  langchain import
-00001b30: 204c 4c4d 4368 6169 6e2c 204f 7065 6e41   LLMChain, OpenA
-00001b40: 492c 2053 6572 7041 5049 5772 6170 7065  I, SerpAPIWrappe
-00001b50: 720a 6672 6f6d 206c 616e 6763 6861 696e  r.from langchain
-00001b60: 2e61 6765 6e74 7320 696d 706f 7274 2041  .agents import A
-00001b70: 6765 6e74 4578 6563 7574 6f72 2c20 546f  gentExecutor, To
-00001b80: 6f6c 2c20 5a65 726f 5368 6f74 4167 656e  ol, ZeroShotAgen
-00001b90: 740a 0a66 726f 6d20 6c63 7365 7276 6520  t..from lcserve 
-00001ba0: 696d 706f 7274 2073 6572 7669 6e67 0a0a  import serving..
-00001bb0: 0a40 7365 7276 696e 670a 6465 6620 6173  .@serving.def as
-00001bc0: 6b28 696e 7075 743a 2073 7472 2920 2d3e  k(input: str) ->
-00001bd0: 2073 7472 3a0a 2020 2020 7365 6172 6368   str:.    search
-00001be0: 203d 2053 6572 7041 5049 5772 6170 7065   = SerpAPIWrappe
-00001bf0: 7228 290a 2020 2020 746f 6f6c 7320 3d20  r().    tools = 
-00001c00: 5b0a 2020 2020 2020 2020 546f 6f6c 280a  [.        Tool(.
-00001c10: 2020 2020 2020 2020 2020 2020 6e61 6d65              name
-00001c20: 3d22 5365 6172 6368 222c 0a20 2020 2020  ="Search",.     
-00001c30: 2020 2020 2020 2066 756e 633d 7365 6172         func=sear
-00001c40: 6368 2e72 756e 2c0a 2020 2020 2020 2020  ch.run,.        
-00001c50: 2020 2020 6465 7363 7269 7074 696f 6e3d      description=
-00001c60: 2275 7365 6675 6c20 666f 7220 7768 656e  "useful for when
-00001c70: 2079 6f75 206e 6565 6420 746f 2061 6e73   you need to ans
-00001c80: 7765 7220 7175 6573 7469 6f6e 7320 6162  wer questions ab
-00001c90: 6f75 7420 6375 7272 656e 7420 6576 656e  out current even
-00001ca0: 7473 222c 0a20 2020 2020 2020 2029 0a20  ts",.        ). 
-00001cb0: 2020 205d 0a20 2020 2070 7265 6669 7820     ].    prefix 
-00001cc0: 3d20 2222 2241 6e73 7765 7220 7468 6520  = """Answer the 
-00001cd0: 666f 6c6c 6f77 696e 6720 7175 6573 7469  following questi
-00001ce0: 6f6e 7320 6173 2062 6573 7420 796f 7520  ons as best you 
-00001cf0: 6361 6e2c 2062 7574 2073 7065 616b 696e  can, but speakin
-00001d00: 6720 6173 2061 2070 6972 6174 6520 6d69  g as a pirate mi
-00001d10: 6768 7420 7370 6561 6b2e 2059 6f75 2068  ght speak. You h
-00001d20: 6176 6520 6163 6365 7373 2074 6f20 7468  ave access to th
-00001d30: 6520 666f 6c6c 6f77 696e 6720 746f 6f6c  e following tool
-00001d40: 733a 2222 220a 2020 2020 7375 6666 6978  s:""".    suffix
-00001d50: 203d 2022 2222 4265 6769 6e21 2052 656d   = """Begin! Rem
-00001d60: 656d 6265 7220 746f 2073 7065 616b 2061  ember to speak a
-00001d70: 7320 6120 7069 7261 7465 2077 6865 6e20  s a pirate when 
-00001d80: 6769 7669 6e67 2079 6f75 7220 6669 6e61  giving your fina
-00001d90: 6c20 616e 7377 6572 2e20 5573 6520 6c6f  l answer. Use lo
-00001da0: 7473 206f 6620 2241 7267 7322 0a0a 2020  ts of "Args"..  
-00001db0: 2020 5175 6573 7469 6f6e 3a20 7b69 6e70    Question: {inp
-00001dc0: 7574 7d0a 2020 2020 7b61 6765 6e74 5f73  ut}.    {agent_s
-00001dd0: 6372 6174 6368 7061 647d 2222 220a 0a20  cratchpad}""".. 
-00001de0: 2020 2070 726f 6d70 7420 3d20 5a65 726f     prompt = Zero
-00001df0: 5368 6f74 4167 656e 742e 6372 6561 7465  ShotAgent.create
-00001e00: 5f70 726f 6d70 7428 0a20 2020 2020 2020  _prompt(.       
-00001e10: 2074 6f6f 6c73 2c0a 2020 2020 2020 2020   tools,.        
-00001e20: 7072 6566 6978 3d70 7265 6669 782c 0a20  prefix=prefix,. 
-00001e30: 2020 2020 2020 2073 7566 6669 783d 7375         suffix=su
-00001e40: 6666 6978 2c0a 2020 2020 2020 2020 696e  ffix,.        in
-00001e50: 7075 745f 7661 7269 6162 6c65 733d 5b22  put_variables=["
-00001e60: 696e 7075 7422 2c20 2261 6765 6e74 5f73  input", "agent_s
-00001e70: 6372 6174 6368 7061 6422 5d2c 0a20 2020  cratchpad"],.   
-00001e80: 2029 0a0a 2020 2020 7072 696e 7428 7072   )..    print(pr
-00001e90: 6f6d 7074 2e74 656d 706c 6174 6529 0a0a  ompt.template)..
-00001ea0: 2020 2020 6c6c 6d5f 6368 6169 6e20 3d20      llm_chain = 
-00001eb0: 4c4c 4d43 6861 696e 286c 6c6d 3d4f 7065  LLMChain(llm=Ope
-00001ec0: 6e41 4928 7465 6d70 6572 6174 7572 653d  nAI(temperature=
-00001ed0: 3029 2c20 7072 6f6d 7074 3d70 726f 6d70  0), prompt=promp
-00001ee0: 7429 0a20 2020 2074 6f6f 6c5f 6e61 6d65  t).    tool_name
-00001ef0: 7320 3d20 5b74 6f6f 6c2e 6e61 6d65 2066  s = [tool.name f
-00001f00: 6f72 2074 6f6f 6c20 696e 2074 6f6f 6c73  or tool in tools
-00001f10: 5d0a 2020 2020 6167 656e 7420 3d20 5a65  ].    agent = Ze
-00001f20: 726f 5368 6f74 4167 656e 7428 6c6c 6d5f  roShotAgent(llm_
-00001f30: 6368 6169 6e3d 6c6c 6d5f 6368 6169 6e2c  chain=llm_chain,
-00001f40: 2061 6c6c 6f77 6564 5f74 6f6f 6c73 3d74   allowed_tools=t
-00001f50: 6f6f 6c5f 6e61 6d65 7329 0a0a 2020 2020  ool_names)..    
-00001f60: 6167 656e 745f 6578 6563 7574 6f72 203d  agent_executor =
-00001f70: 2041 6765 6e74 4578 6563 7574 6f72 2e66   AgentExecutor.f
-00001f80: 726f 6d5f 6167 656e 745f 616e 645f 746f  rom_agent_and_to
-00001f90: 6f6c 7328 0a20 2020 2020 2020 2061 6765  ols(.        age
-00001fa0: 6e74 3d61 6765 6e74 2c20 746f 6f6c 733d  nt=agent, tools=
-00001fb0: 746f 6f6c 732c 2076 6572 626f 7365 3d54  tools, verbose=T
-00001fc0: 7275 650a 2020 2020 290a 0a20 2020 2072  rue.    )..    r
-00001fd0: 6574 7572 6e20 6167 656e 745f 6578 6563  eturn agent_exec
-00001fe0: 7574 6f72 2e72 756e 2869 6e70 7574 290a  utor.run(input).
-00001ff0: 0a69 6620 5f5f 6e61 6d65 5f5f 203d 3d20  .if __name__ == 
-00002000: 225f 5f6d 6169 6e5f 5f22 3a0a 2020 2020  "__main__":.    
-00002010: 6173 6b28 2748 6f77 206d 616e 7920 7065  ask('How many pe
-00002020: 6f70 6c65 206c 6976 6520 696e 2063 616e  ople live in can
-00002030: 6164 6120 6173 206f 6620 3230 3233 3f27  ada as of 2023?'
-00002040: 290a 6060 600a 0a3c 2f64 6574 6169 6c73  ).```..</details
-00002050: 3e0a 0a0a 2323 2323 2320 5768 6174 2063  >...##### What c
-00002060: 6861 6e67 6564 3f0a 0a2d 2057 6520 6d6f  hanged?..- We mo
-00002070: 7665 6420 6f75 7220 636f 6465 2074 6f20  ved our code to 
-00002080: 616e 2060 6173 6b60 2066 756e 6374 696f  an `ask` functio
-00002090: 6e2e 0a2d 2041 6464 6564 2074 7970 6520  n..- Added type 
-000020a0: 6869 6e74 7320 746f 2074 6865 2066 756e  hints to the fun
-000020b0: 6374 696f 6e20 7061 7261 6d65 7465 7273  ction parameters
-000020c0: 2028 696e 7075 7420 616e 6420 6f75 7470   (input and outp
-000020d0: 7574 292c 2073 6f20 4150 4920 6465 6669  ut), so API defi
-000020e0: 6e69 7469 6f6e 2063 616e 2062 6520 6765  nition can be ge
-000020f0: 6e65 7261 7465 642e 0a2d 2049 6d70 6f72  nerated..- Impor
-00002100: 7465 6420 6066 726f 6d20 6c63 7365 7276  ted `from lcserv
-00002110: 6520 696d 706f 7274 2073 6572 7669 6e67  e import serving
-00002120: 6020 616e 6420 6164 6465 6420 6040 7365  ` and added `@se
-00002130: 7276 696e 6760 2064 6563 6f72 6174 6f72  rving` decorator
-00002140: 2074 6f20 7468 6520 6061 736b 6020 6675   to the `ask` fu
-00002150: 6e63 7469 6f6e 2e0a 2d20 4164 6465 6420  nction..- Added 
-00002160: 6069 6620 5f5f 6e61 6d65 5f5f 203d 3d20  `if __name__ == 
-00002170: 225f 5f6d 6169 6e5f 5f22 3a60 2062 6c6f  "__main__":` blo
-00002180: 636b 2074 6f20 7465 7374 2074 6865 2066  ck to test the f
-00002190: 756e 6374 696f 6e20 6c6f 6361 6c6c 792e  unction locally.
-000021a0: 0a0a 2d2d 2d0a 0a23 2323 2053 7465 7020  ..---..### Step 
-000021b0: 323a 0a0a 2a2a 4372 6561 7465 2061 2060  2:..**Create a `
-000021c0: 7265 7175 6972 656d 656e 7473 2e74 7874  requirements.txt
-000021d0: 6020 6669 6c65 2069 6e20 796f 7572 2061  ` file in your a
-000021e0: 7070 2064 6972 6563 746f 7279 2074 6f20  pp directory to 
-000021f0: 656e 7375 7265 2061 6c6c 206e 6563 6573  ensure all neces
-00002200: 7361 7279 2064 6570 656e 6465 6e63 6965  sary dependencie
-00002210: 7320 6172 6520 696e 7374 616c 6c65 642e  s are installed.
-00002220: 2a2a 0a0a 3c64 6574 6169 6c73 3e0a 3c73  **..<details>.<s
-00002230: 756d 6d61 7279 3e53 686f 7720 7265 7175  ummary>Show requ
-00002240: 6972 656d 656e 7473 2e74 7874 3c2f 7375  irements.txt</su
-00002250: 6d6d 6172 793e 0a0a 6060 6074 6578 740a  mmary>..```text.
-00002260: 2320 7265 7175 6972 656d 656e 7473 2e74  # requirements.t
-00002270: 7874 0a6f 7065 6e61 690a 676f 6f67 6c65  xt.openai.google
-00002280: 2d73 6561 7263 682d 7265 7375 6c74 730a  -search-results.
-00002290: 6060 600a 3c2f 6465 7461 696c 733e 0a0a  ```.</details>..
-000022a0: 2d2d 2d20 0a0a 2323 2320 5374 6570 2033  --- ..### Step 3
-000022b0: 3a0a 0a2a 2a52 756e 2060 6c63 2d73 6572  :..**Run `lc-ser
-000022c0: 7665 2064 6570 6c6f 7920 6c6f 6361 6c20  ve deploy local 
-000022d0: 6170 7060 2074 6f20 7465 7374 2079 6f75  app` to test you
-000022e0: 7220 4150 4920 6c6f 6361 6c6c 792e 2a2a  r API locally.**
-000022f0: 0a0a 3e20 6061 7070 6020 6973 2074 6865  ..> `app` is the
-00002300: 206e 616d 6520 6f66 2074 6865 206d 6f64   name of the mod
-00002310: 756c 6520 7468 6174 2063 6f6e 7461 696e  ule that contain
-00002320: 7320 7468 6520 6061 736b 6020 6675 6e63  s the `ask` func
-00002330: 7469 6f6e 2e0a 0a60 6060 6261 7368 0a6c  tion...```bash.l
-00002340: 632d 7365 7276 6520 6465 706c 6f79 206c  c-serve deploy l
-00002350: 6f63 616c 2061 7070 0a60 6060 0a0a 3c64  ocal app.```..<d
-00002360: 6574 6169 6c73 3e0a 3c73 756d 6d61 7279  etails>.<summary
-00002370: 3e53 686f 7720 6f75 7470 7574 3c2f 7375  >Show output</su
-00002380: 6d6d 6172 793e 0a0a 6060 6074 6578 740a  mmary>..```text.
+00000030: 696f 6e3a 2030 2e30 2e39 2e64 6576 390a  ion: 0.0.9.dev9.
+00000040: 5375 6d6d 6172 793a 204c 616e 6763 6861  Summary: Langcha
+00000050: 696e 2053 6572 7665 202d 2073 6572 7665  in Serve - serve
+00000060: 2079 6f75 7220 6c61 6e67 6368 6169 6e20   your langchain 
+00000070: 6170 7073 206f 6e20 4a69 6e61 2041 4920  apps on Jina AI 
+00000080: 436c 6f75 642e 0a48 6f6d 652d 7061 6765  Cloud..Home-page
+00000090: 3a20 6874 7470 733a 2f2f 6769 7468 7562  : https://github
+000000a0: 2e63 6f6d 2f6a 696e 612d 6169 2f6c 616e  .com/jina-ai/lan
+000000b0: 6763 6861 696e 2d73 6572 7665 2f0a 4175  gchain-serve/.Au
+000000c0: 7468 6f72 3a20 4a69 6e61 2041 490a 4175  thor: Jina AI.Au
+000000d0: 7468 6f72 2d65 6d61 696c 3a20 6865 6c6c  thor-email: hell
+000000e0: 6f40 6a69 6e61 2e61 690a 4c69 6365 6e73  o@jina.ai.Licens
+000000f0: 653a 2041 7061 6368 6520 322e 300a 446f  e: Apache 2.0.Do
+00000100: 776e 6c6f 6164 2d55 524c 3a20 6874 7470  wnload-URL: http
+00000110: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6a  s://github.com/j
+00000120: 696e 612d 6169 2f6c 616e 6763 6861 696e  ina-ai/langchain
+00000130: 2d73 6572 7665 2f74 6167 730a 5072 6f6a  -serve/tags.Proj
+00000140: 6563 742d 5552 4c3a 2044 6f63 756d 656e  ect-URL: Documen
+00000150: 7461 7469 6f6e 2c20 6874 7470 733a 2f2f  tation, https://
+00000160: 646f 6373 2e6a 696e 612e 6169 0a50 726f  docs.jina.ai.Pro
+00000170: 6a65 6374 2d55 524c 3a20 536f 7572 6365  ject-URL: Source
+00000180: 2c20 6874 7470 733a 2f2f 6769 7468 7562  , https://github
+00000190: 2e63 6f6d 2f6a 696e 612d 6169 2f6e 6f77  .com/jina-ai/now
+000001a0: 0a50 726f 6a65 6374 2d55 524c 3a20 5472  .Project-URL: Tr
+000001b0: 6163 6b65 722c 2068 7474 7073 3a2f 2f67  acker, https://g
+000001c0: 6974 6875 622e 636f 6d2f 6a69 6e61 2d61  ithub.com/jina-a
+000001d0: 692f 6e6f 772f 6973 7375 6573 0a4b 6579  i/now/issues.Key
+000001e0: 776f 7264 733a 206a 696e 6120 6c61 6e67  words: jina lang
+000001f0: 6368 6169 6e20 6c6c 6d20 6e65 7572 616c  chain llm neural
+00000200: 2d6e 6574 776f 726b 2064 6565 702d 6c65  -network deep-le
+00000210: 6172 6e69 6e67 2064 6174 6120 6465 6d6f  arning data demo
+00000220: 6372 6174 697a 6174 696f 6e0a 506c 6174  cratization.Plat
+00000230: 666f 726d 3a20 554e 4b4e 4f57 4e0a 436c  form: UNKNOWN.Cl
+00000240: 6173 7369 6669 6572 3a20 4465 7665 6c6f  assifier: Develo
+00000250: 706d 656e 7420 5374 6174 7573 203a 3a20  pment Status :: 
+00000260: 3520 2d20 5072 6f64 7563 7469 6f6e 2f53  5 - Production/S
+00000270: 7461 626c 650a 436c 6173 7369 6669 6572  table.Classifier
+00000280: 3a20 496e 7465 6e64 6564 2041 7564 6965  : Intended Audie
+00000290: 6e63 6520 3a3a 2044 6576 656c 6f70 6572  nce :: Developer
+000002a0: 730a 436c 6173 7369 6669 6572 3a20 496e  s.Classifier: In
+000002b0: 7465 6e64 6564 2041 7564 6965 6e63 6520  tended Audience 
+000002c0: 3a3a 2045 6475 6361 7469 6f6e 0a43 6c61  :: Education.Cla
+000002d0: 7373 6966 6965 723a 2049 6e74 656e 6465  ssifier: Intende
+000002e0: 6420 4175 6469 656e 6365 203a 3a20 5363  d Audience :: Sc
+000002f0: 6965 6e63 652f 5265 7365 6172 6368 0a43  ience/Research.C
+00000300: 6c61 7373 6966 6965 723a 2050 726f 6772  lassifier: Progr
+00000310: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+00000320: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e37  :: Python :: 3.7
+00000330: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
+00000340: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+00000350: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
+00000360: 2e38 0a43 6c61 7373 6966 6965 723a 2050  .8.Classifier: P
+00000370: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+00000380: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+00000390: 2033 2e39 0a43 6c61 7373 6966 6965 723a   3.9.Classifier:
+000003a0: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
+000003b0: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
+000003c0: 3a3a 2033 2e31 300a 436c 6173 7369 6669  :: 3.10.Classifi
+000003d0: 6572 3a20 456e 7669 726f 6e6d 656e 7420  er: Environment 
+000003e0: 3a3a 2043 6f6e 736f 6c65 0a43 6c61 7373  :: Console.Class
+000003f0: 6966 6965 723a 204c 6963 656e 7365 203a  ifier: License :
+00000400: 3a20 4f53 4920 4170 7072 6f76 6564 203a  : OSI Approved :
+00000410: 3a20 4170 6163 6865 2053 6f66 7477 6172  : Apache Softwar
+00000420: 6520 4c69 6365 6e73 650a 436c 6173 7369  e License.Classi
+00000430: 6669 6572 3a20 4f70 6572 6174 696e 6720  fier: Operating 
+00000440: 5379 7374 656d 203a 3a20 4f53 2049 6e64  System :: OS Ind
+00000450: 6570 656e 6465 6e74 0a43 6c61 7373 6966  ependent.Classif
+00000460: 6965 723a 2054 6f70 6963 203a 3a20 5363  ier: Topic :: Sc
+00000470: 6965 6e74 6966 6963 2f45 6e67 696e 6565  ientific/Enginee
+00000480: 7269 6e67 203a 3a20 4172 7469 6669 6369  ring :: Artifici
+00000490: 616c 2049 6e74 656c 6c69 6765 6e63 650a  al Intelligence.
+000004a0: 4465 7363 7269 7074 696f 6e2d 436f 6e74  Description-Cont
+000004b0: 656e 742d 5479 7065 3a20 7465 7874 2f6d  ent-Type: text/m
+000004c0: 6172 6b64 6f77 6e0a 4c69 6365 6e73 652d  arkdown.License-
+000004d0: 4669 6c65 3a20 4c49 4345 4e53 450a 0a23  File: LICENSE..#
+000004e0: 204c 616e 6743 6861 696e 2041 7070 7320   LangChain Apps 
+000004f0: 6f6e 2050 726f 6475 6374 696f 6e20 7769  on Production wi
+00000500: 7468 204a 696e 6120 f09f 9a80 0a0a 5b4a  th Jina ......[J
+00000510: 696e 615d 2868 7474 7073 3a2f 2f67 6974  ina](https://git
+00000520: 6875 622e 636f 6d2f 6a69 6e61 2d61 692f  hub.com/jina-ai/
+00000530: 6a69 6e61 2920 6973 2061 6e20 6f70 656e  jina) is an open
+00000540: 2d73 6f75 7263 6520 6672 616d 6577 6f72  -source framewor
+00000550: 6b20 746f 2062 7569 6c64 2c20 6465 706c  k to build, depl
+00000560: 6f79 2026 206d 616e 6167 6520 6d61 6368  oy & manage mach
+00000570: 696e 6520 6c65 6172 6e69 6e67 2061 7070  ine learning app
+00000580: 6c69 6361 7469 6f6e 7320 6174 2073 6361  lications at sca
+00000590: 6c65 2e20 5b4c 616e 6743 6861 696e 5d28  le. [LangChain](
+000005a0: 6874 7470 733a 2f2f 7079 7468 6f6e 2e6c  https://python.l
+000005b0: 616e 6763 6861 696e 2e63 6f6d 2f65 6e2f  angchain.com/en/
+000005c0: 6c61 7465 7374 2f69 6e64 6578 2e68 746d  latest/index.htm
+000005d0: 6c29 2069 7320 616e 6f74 6865 7220 6f70  l) is another op
+000005e0: 656e 2d73 6f75 7263 6520 6672 616d 6577  en-source framew
+000005f0: 6f72 6b20 666f 7220 6275 696c 6469 6e67  ork for building
+00000600: 2061 7070 6c69 6361 7469 6f6e 7320 706f   applications po
+00000610: 7765 7265 6420 6279 206c 616e 6775 6167  wered by languag
+00000620: 6520 6d6f 6465 6c73 2e20 0a0a 2a2a 6c61  e models. ..**la
+00000630: 6e67 6368 6169 6e2d 7365 7276 652a 2a20  ngchain-serve** 
+00000640: 6865 6c70 7320 796f 7520 6465 706c 6f79  helps you deploy
+00000650: 2079 6f75 7220 4c61 6e67 4368 6169 6e20   your LangChain 
+00000660: 6170 7073 206f 6e20 4a69 6e61 2041 4920  apps on Jina AI 
+00000670: 436c 6f75 6420 696e 206a 7573 7420 6120  Cloud in just a 
+00000680: 6d61 7474 6572 206f 6620 7365 636f 6e64  matter of second
+00000690: 732e 2059 6f75 2063 616e 206e 6f77 2062  s. You can now b
+000006a0: 656e 6566 6974 2066 726f 6d20 7468 6520  enefit from the 
+000006b0: 7363 616c 6162 696c 6974 7920 616e 6420  scalability and 
+000006c0: 7365 7276 6572 6c65 7373 2061 7263 6869  serverless archi
+000006d0: 7465 6374 7572 6520 6f66 2074 6865 2063  tecture of the c
+000006e0: 6c6f 7564 2077 6974 686f 7574 2073 6163  loud without sac
+000006f0: 7269 6669 6369 6e67 2074 6865 2065 6173  rificing the eas
+00000700: 6520 616e 6420 636f 6e76 656e 6965 6e63  e and convenienc
+00000710: 6520 6f66 206c 6f63 616c 2064 6576 656c  e of local devel
+00000720: 6f70 6d65 6e74 2e0a 0a0a 2323 20f0 9fa7  opment....## ...
+00000730: a020 4261 6279 6167 692d 6173 2d61 2d73  . Babyagi-as-a-s
+00000740: 6572 7669 6365 0a0a 3e20 4769 7665 2075  ervice..> Give u
+00000750: 7320 6120 3a73 7461 723a 2061 6e64 2074  s a :star: and t
+00000760: 656c 6c20 7573 2077 6861 7420 6d6f 7265  ell us what more
+00000770: 2079 6f75 2764 206c 696b 6520 746f 2073   you'd like to s
+00000780: 6565 2120 0a0a 2d20 4465 706c 6f79 2060  ee! ..- Deploy `
+00000790: 6261 6279 6167 6960 206f 6e20 4a69 6e61  babyagi` on Jina
+000007a0: 2041 4920 436c 6f75 6420 7769 7468 206f   AI Cloud with o
+000007b0: 6e65 2063 6f6d 6d61 6e64 0a0a 2020 6060  ne command..  ``
+000007c0: 6062 6173 680a 2020 6c63 2d73 6572 7665  `bash.  lc-serve
+000007d0: 2064 6570 6c6f 7920 6261 6279 6167 690a   deploy babyagi.
+000007e0: 2020 6060 600a 0a2d 2049 6e74 6567 7261    ```..- Integra
+000007f0: 7465 2062 6162 7961 6769 2077 6974 6820  te babyagi with 
+00000800: 6578 7465 726e 616c 2073 6572 7669 6365  external service
+00000810: 7320 7573 696e 6720 6f75 7220 5765 6273  s using our Webs
+00000820: 6f63 6b65 7420 4150 492e 2047 6574 2061  ocket API. Get a
+00000830: 2066 6c61 766f 7220 6f66 2074 6865 2069   flavor of the i
+00000840: 6e74 6567 7261 7469 6f6e 206f 6e20 796f  ntegration on yo
+00000850: 7572 2043 4c49 2077 6974 6820 0a20 2020  ur CLI with .   
+00000860: 200a 2020 6060 6062 6173 680a 2020 6c63   .  ```bash.  lc
+00000870: 2d73 6572 7665 2070 6c61 7967 726f 756e  -serve playgroun
+00000880: 6420 6261 6279 6167 690a 2020 6060 600a  d babyagi.  ```.
+00000890: 0a21 5b42 6162 7961 6769 2d61 732d 612d  .![Babyagi-as-a-
+000008a0: 7365 7276 6963 6520 506c 6179 6772 6f75  service Playgrou
+000008b0: 6e64 5d28 2e67 6974 6875 622f 696d 6167  nd](.github/imag
+000008c0: 6573 2f62 6162 7961 6769 2d70 6c61 7967  es/babyagi-playg
+000008d0: 726f 756e 642e 6769 6629 0a0a 0a23 2323  round.gif)...###
+000008e0: 2320 f09f 8e89 2043 7573 746f 6d20 4170  # .... Custom Ap
+000008f0: 7073 2074 6f20 7072 6f64 7563 7469 6f6e  ps to production
+00000900: 2069 6e20 3420 7369 6d70 6c65 2073 7465   in 4 simple ste
+00000910: 7073 0a0a 2020 312e 2052 6566 6163 746f  ps..  1. Refacto
+00000920: 7220 796f 7572 2063 6f64 6520 746f 2066  r your code to f
+00000930: 756e 6374 696f 6e28 7329 2074 6861 7420  unction(s) that 
+00000940: 7368 6f75 6c64 2062 6520 7365 7276 6564  should be served
+00000950: 2077 6974 6820 6040 7365 7276 696e 6760   with `@serving`
+00000960: 2064 6563 6f72 6174 6f72 2e0a 2020 312e   decorator..  1.
+00000970: 2043 7265 6174 6520 6120 6072 6571 7569   Create a `requi
+00000980: 7265 6d65 6e74 732e 7478 7460 2066 696c  rements.txt` fil
+00000990: 6520 696e 2079 6f75 7220 6170 7020 6469  e in your app di
+000009a0: 7265 6374 6f72 7920 746f 2065 6e73 7572  rectory to ensur
+000009b0: 6520 616c 6c20 6e65 6365 7373 6172 7920  e all necessary 
+000009c0: 6465 7065 6e64 656e 6369 6573 2061 7265  dependencies are
+000009d0: 2069 6e73 7461 6c6c 6564 2e0a 2020 312e   installed..  1.
+000009e0: 2052 756e 2060 6c63 2d73 6572 7665 2064   Run `lc-serve d
+000009f0: 6570 6c6f 7920 6c6f 6361 6c20 6170 7060  eploy local app`
+00000a00: 2074 6f20 7465 7374 2079 6f75 7220 4150   to test your AP
+00000a10: 4920 6c6f 6361 6c6c 792e 0a20 2031 2e20  I locally..  1. 
+00000a20: 5275 6e20 606c 632d 7365 7276 6520 6465  Run `lc-serve de
+00000a30: 706c 6f79 206a 636c 6f75 6420 6170 7060  ploy jcloud app`
+00000a40: 2074 6f20 6465 706c 6f79 206f 6e20 5b4a   to deploy on [J
+00000a50: 696e 6120 4149 2043 6c6f 7564 5d28 6874  ina AI Cloud](ht
+00000a60: 7470 733a 2f2f 6a69 6e61 2e61 692f 7072  tps://jina.ai/pr
+00000a70: 6f64 7563 742f 636c 6f75 642f 292e 0a0a  oduct/cloud/)...
+00000a80: 0a23 2323 2320 f09f 94a5 2053 6361 6c61  .#### .... Scala
+00000a90: 626c 652c 2053 6572 7665 726c 6573 7320  ble, Serverless 
+00000aa0: 5245 5354 6675 6c2f 5374 7265 616d 696e  RESTful/Streamin
+00000ab0: 6720 5765 6273 6f63 6b65 7420 4150 4973  g Websocket APIs
+00000ac0: 206f 6e20 4a69 6e61 2041 4920 436c 6f75   on Jina AI Clou
+00000ad0: 640a 0a20 202d 20f0 9f8c 8e20 5245 5354  d..  - .... REST
+00000ae0: 6675 6c2f 5765 6273 6f63 6b65 7420 4150  ful/Websocket AP
+00000af0: 4973 2077 6974 6820 544c 5320 6365 7274  Is with TLS cert
+00000b00: 7320 696e 206a 7573 7420 3220 6c69 6e65  s in just 2 line
+00000b10: 7320 6f66 2063 6f64 6520 6368 616e 6765  s of code change
+00000b20: 2e0a 2020 2d20 f09f 8c8a 2053 7472 6561  ..  - .... Strea
+00000b30: 6d20 4c4c 4d20 696e 7465 7261 6374 696f  m LLM interactio
+00000b40: 6e73 2069 6e20 7265 616c 2d74 696d 6520  ns in real-time 
+00000b50: 7769 7468 2057 6562 736f 636b 6574 732e  with Websockets.
+00000b60: 0a20 202d 20f0 9f91 a520 456e 6162 6c65  .  - .... Enable
+00000b70: 2068 756d 616e 2069 6e20 7468 6520 6c6f   human in the lo
+00000b80: 6f70 2066 6f72 2079 6f75 7220 6167 656e  op for your agen
+00000b90: 7473 2e0a 2020 2d20 f09f 9384 2053 7761  ts..  - .... Swa
+00000ba0: 6767 6572 2055 492c 2061 6e64 204f 7065  gger UI, and Ope
+00000bb0: 6e41 5049 2073 7065 6320 696e 636c 7564  nAPI spec includ
+00000bc0: 6564 2077 6974 6820 796f 7572 2041 5049  ed with your API
+00000bd0: 732e 0a20 202d 20e2 9aa1 efb8 8f20 5365  s..  - ...... Se
+00000be0: 7276 6572 6c65 7373 2061 7070 7320 7468  rverless apps th
+00000bf0: 6174 2073 6361 6c65 7320 6175 746f 6d61  at scales automa
+00000c00: 7469 6361 6c6c 7920 7769 7468 2079 6f75  tically with you
+00000c10: 7220 7472 6166 6669 632e 0a20 202d 20f0  r traffic..  - .
+00000c20: 9f93 8a20 4275 696c 7469 6e20 6c6f 6767  ... Builtin logg
+00000c30: 696e 672c 206d 6f6e 6974 6f72 696e 672c  ing, monitoring,
+00000c40: 2061 6e64 2074 7261 6365 7320 666f 7220   and traces for 
+00000c50: 796f 7572 2041 5049 732e 0a20 202d 20f0  your APIs..  - .
+00000c60: 9fa4 9620 4e6f 206e 6565 6420 746f 2063  ... No need to c
+00000c70: 6861 6e67 6520 796f 7572 2063 6f64 6520  hange your code 
+00000c80: 746f 206d 616e 6167 6520 4150 4973 2c20  to manage APIs, 
+00000c90: 6f72 206d 616e 6167 6520 646f 636b 6572  or manage docker
+00000ca0: 6669 6c65 732c 206f 7220 776f 7272 7920  files, or worry 
+00000cb0: 6162 6f75 7420 696e 6672 6173 7472 7563  about infrastruc
+00000cc0: 7475 7265 210a 0a0a 2323 2323 20f0 9f9a  ture!...#### ...
+00000cd0: a720 436f 6d69 6e67 2073 6f6f 6e0a 0a2d  . Coming soon..-
+00000ce0: 205b 205d 20f0 9f94 9120 4175 7468 6f72   [ ] .... Author
+00000cf0: 697a 6520 4150 4920 656e 6470 6f69 6e74  ize API endpoint
+00000d00: 730a 2d20 5b20 5d20 f09f 9ba0 efb8 8f20  s.- [ ] ....... 
+00000d10: 456e 6162 6c65 2053 7472 6561 6d6c 6974  Enable Streamlit
+00000d20: 2070 6c61 7967 726f 756e 6420 6465 706c   playground depl
+00000d30: 6f79 6d65 6e74 2066 6f72 2079 6f75 7220  oyment for your 
+00000d40: 6170 7073 0a0a 0a49 6620 796f 7520 6861  apps...If you ha
+00000d50: 7665 2061 6e79 2066 6561 7475 7265 2072  ve any feature r
+00000d60: 6571 7565 7374 7320 6f72 2066 6163 6564  equests or faced
+00000d70: 2061 6e79 2069 7373 7565 2c20 706c 6561   any issue, plea
+00000d80: 7365 205b 6c65 7420 7573 206b 6e6f 775d  se [let us know]
+00000d90: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00000da0: 636f 6d2f 6a69 6e61 2d61 692f 6c61 6e67  com/jina-ai/lang
+00000db0: 6368 6169 6e2d 7365 7276 652f 6973 7375  chain-serve/issu
+00000dc0: 6573 2f6e 6577 2921 0a0a 0a23 2320 5573  es/new)!...## Us
+00000dd0: 6167 650a 0a4c 6574 2773 2066 6972 7374  age..Let's first
+00000de0: 2069 6e73 7461 6c6c 2060 6c61 6e67 6368   install `langch
+00000df0: 6169 6e2d 7365 7276 6560 2075 7369 6e67  ain-serve` using
+00000e00: 2070 6970 2e0a 0a60 6060 6261 7368 0a70   pip...```bash.p
+00000e10: 6970 2069 6e73 7461 6c6c 206c 616e 6763  ip install langc
+00000e20: 6861 696e 2d73 6572 7665 0a60 6060 0a0a  hain-serve.```..
+00000e30: 2323 2045 6e61 626c 6520 4875 6d61 6e2d  ## Enable Human-
+00000e40: 696e 2d74 6865 2d6c 6f6f 7020 2848 4954  in-the-loop (HIT
+00000e50: 4c29 2066 6f72 2079 6f75 7220 6167 656e  L) for your agen
+00000e60: 7473 0a0a 4849 544c 2066 6f72 204c 616e  ts..HITL for Lan
+00000e70: 6743 6861 696e 2061 6765 6e74 7320 6f6e  gChain agents on
+00000e80: 2070 726f 6475 6374 696f 6e20 6361 6e20   production can 
+00000e90: 6265 2063 6861 6c6c 656e 6769 6e67 2073  be challenging s
+00000ea0: 696e 6365 2074 6865 2061 6765 6e74 7320  ince the agents 
+00000eb0: 6172 6520 7479 7069 6361 6c6c 7920 7275  are typically ru
+00000ec0: 6e6e 696e 6720 6f6e 2073 6572 7665 7273  nning on servers
+00000ed0: 2077 6865 7265 2068 756d 616e 7320 646f   where humans do
+00000ee0: 6e27 7420 6861 7665 2064 6972 6563 7420  n't have direct 
+00000ef0: 6163 6365 7373 2e20 2a2a 6c61 6e67 6368  access. **langch
+00000f00: 6169 6e2d 7365 7276 652a 2a20 6272 6964  ain-serve** brid
+00000f10: 6765 7320 7468 6973 2067 6170 2062 7920  ges this gap by 
+00000f20: 656e 6162 6c69 6e67 2077 6562 736f 636b  enabling websock
+00000f30: 6574 2041 5049 7320 7468 6174 2061 6c6c  et APIs that all
+00000f40: 6f77 2066 6f72 2072 6561 6c2d 7469 6d65  ow for real-time
+00000f50: 2069 6e74 6572 6163 7469 6f6e 2061 6e64   interaction and
+00000f60: 2066 6565 6462 6163 6b20 6265 7477 6565   feedback betwee
+00000f70: 6e20 7468 6520 6167 656e 7420 616e 6420  n the agent and 
+00000f80: 6120 6875 6d61 6e20 6f70 6572 6174 6f72  a human operator
+00000f90: 2e0a 0a43 6865 636b 206f 7574 2074 6869  ...Check out thi
+00000fa0: 7320 5b65 7861 6d70 6c65 5d28 6578 616d  s [example](exam
+00000fb0: 706c 6573 2f77 6562 736f 636b 6574 732f  ples/websockets/
+00000fc0: 6869 746c 2f52 4541 444d 452e 6d64 2920  hitl/README.md) 
+00000fd0: 746f 2073 6565 2068 6f77 2079 6f75 2063  to see how you c
+00000fe0: 616e 2065 6e61 626c 6520 4849 544c 2066  an enable HITL f
+00000ff0: 6f72 2079 6f75 7220 6167 656e 7473 2e0a  or your agents..
+00001000: 0a0a 2323 2045 6e61 626c 6520 5245 5354  ..## Enable REST
+00001010: 2041 5049 7320 0a0a 0a4c 6574 2773 2062   APIs ...Let's b
+00001020: 7569 6c64 2061 2063 7573 746f 6d20 6167  uild a custom ag
+00001030: 656e 7420 7573 696e 6720 7468 6973 2065  ent using this e
+00001040: 7861 6d70 6c65 2074 616b 656e 2066 726f  xample taken fro
+00001050: 6d20 5b4c 616e 6743 6861 696e 2064 6f63  m [LangChain doc
+00001060: 756d 656e 7461 7469 6f6e 5d28 6874 7470  umentation](http
+00001070: 733a 2f2f 7079 7468 6f6e 2e6c 616e 6763  s://python.langc
+00001080: 6861 696e 2e63 6f6d 2f65 6e2f 6c61 7465  hain.com/en/late
+00001090: 7374 2f6d 6f64 756c 6573 2f61 6765 6e74  st/modules/agent
+000010a0: 732f 6167 656e 7473 2f63 7573 746f 6d5f  s/agents/custom_
+000010b0: 6167 656e 742e 6874 6d6c 292e 200a 0a0a  agent.html). ...
+000010c0: 3c64 6574 6169 6c73 3e0a 3c73 756d 6d61  <details>.<summa
+000010d0: 7279 3e53 686f 7720 6167 656e 7420 636f  ry>Show agent co
+000010e0: 6465 2028 6170 702e 7079 293c 2f73 756d  de (app.py)</sum
+000010f0: 6d61 7279 3e0a 0a60 6060 7079 7468 6f6e  mary>..```python
+00001100: 0a23 2061 7070 2e70 790a 6672 6f6d 206c  .# app.py.from l
+00001110: 616e 6763 6861 696e 2e61 6765 6e74 7320  angchain.agents 
+00001120: 696d 706f 7274 205a 6572 6f53 686f 7441  import ZeroShotA
+00001130: 6765 6e74 2c20 546f 6f6c 2c20 4167 656e  gent, Tool, Agen
+00001140: 7445 7865 6375 746f 720a 6672 6f6d 206c  tExecutor.from l
+00001150: 616e 6763 6861 696e 2069 6d70 6f72 7420  angchain import 
+00001160: 4f70 656e 4149 2c20 5365 7270 4150 4957  OpenAI, SerpAPIW
+00001170: 7261 7070 6572 2c20 4c4c 4d43 6861 696e  rapper, LLMChain
+00001180: 0a0a 7365 6172 6368 203d 2053 6572 7041  ..search = SerpA
+00001190: 5049 5772 6170 7065 7228 290a 746f 6f6c  PIWrapper().tool
+000011a0: 7320 3d20 5b0a 2020 2020 546f 6f6c 280a  s = [.    Tool(.
+000011b0: 2020 2020 2020 2020 6e61 6d65 203d 2022          name = "
+000011c0: 5365 6172 6368 222c 0a20 2020 2020 2020  Search",.       
+000011d0: 2066 756e 633d 7365 6172 6368 2e72 756e   func=search.run
+000011e0: 2c0a 2020 2020 2020 2020 6465 7363 7269  ,.        descri
+000011f0: 7074 696f 6e3d 2275 7365 6675 6c20 666f  ption="useful fo
+00001200: 7220 7768 656e 2079 6f75 206e 6565 6420  r when you need 
+00001210: 746f 2061 6e73 7765 7220 7175 6573 7469  to answer questi
+00001220: 6f6e 7320 6162 6f75 7420 6375 7272 656e  ons about curren
+00001230: 7420 6576 656e 7473 220a 2020 2020 290a  t events".    ).
+00001240: 5d0a 0a70 7265 6669 7820 3d20 2222 2241  ]..prefix = """A
+00001250: 6e73 7765 7220 7468 6520 666f 6c6c 6f77  nswer the follow
+00001260: 696e 6720 7175 6573 7469 6f6e 7320 6173  ing questions as
+00001270: 2062 6573 7420 796f 7520 6361 6e2c 2062   best you can, b
+00001280: 7574 2073 7065 616b 696e 6720 6173 2061  ut speaking as a
+00001290: 2070 6972 6174 6520 6d69 6768 7420 7370   pirate might sp
+000012a0: 6561 6b2e 2059 6f75 2068 6176 6520 6163  eak. You have ac
+000012b0: 6365 7373 2074 6f20 7468 6520 666f 6c6c  cess to the foll
+000012c0: 6f77 696e 6720 746f 6f6c 733a 2222 220a  owing tools:""".
+000012d0: 7375 6666 6978 203d 2022 2222 4265 6769  suffix = """Begi
+000012e0: 6e21 2052 656d 656d 6265 7220 746f 2073  n! Remember to s
+000012f0: 7065 616b 2061 7320 6120 7069 7261 7465  peak as a pirate
+00001300: 2077 6865 6e20 6769 7669 6e67 2079 6f75   when giving you
+00001310: 7220 6669 6e61 6c20 616e 7377 6572 2e20  r final answer. 
+00001320: 5573 6520 6c6f 7473 206f 6620 2241 7267  Use lots of "Arg
+00001330: 7322 0a0a 5175 6573 7469 6f6e 3a20 7b69  s"..Question: {i
+00001340: 6e70 7574 7d0a 7b61 6765 6e74 5f73 6372  nput}.{agent_scr
+00001350: 6174 6368 7061 647d 2222 220a 0a70 726f  atchpad}"""..pro
+00001360: 6d70 7420 3d20 5a65 726f 5368 6f74 4167  mpt = ZeroShotAg
+00001370: 656e 742e 6372 6561 7465 5f70 726f 6d70  ent.create_promp
+00001380: 7428 0a20 2020 2074 6f6f 6c73 2c20 0a20  t(.    tools, . 
+00001390: 2020 2070 7265 6669 783d 7072 6566 6978     prefix=prefix
+000013a0: 2c20 0a20 2020 2073 7566 6669 783d 7375  , .    suffix=su
+000013b0: 6666 6978 2c20 0a20 2020 2069 6e70 7574  ffix, .    input
+000013c0: 5f76 6172 6961 626c 6573 3d5b 2269 6e70  _variables=["inp
+000013d0: 7574 222c 2022 6167 656e 745f 7363 7261  ut", "agent_scra
+000013e0: 7463 6870 6164 225d 0a29 0a0a 6c6c 6d5f  tchpad"].)..llm_
+000013f0: 6368 6169 6e20 3d20 4c4c 4d43 6861 696e  chain = LLMChain
+00001400: 286c 6c6d 3d4f 7065 6e41 4928 7465 6d70  (llm=OpenAI(temp
+00001410: 6572 6174 7572 653d 3029 2c20 7072 6f6d  erature=0), prom
+00001420: 7074 3d70 726f 6d70 7429 0a74 6f6f 6c5f  pt=prompt).tool_
+00001430: 6e61 6d65 7320 3d20 5b74 6f6f 6c2e 6e61  names = [tool.na
+00001440: 6d65 2066 6f72 2074 6f6f 6c20 696e 2074  me for tool in t
+00001450: 6f6f 6c73 5d0a 6167 656e 7420 3d20 5a65  ools].agent = Ze
+00001460: 726f 5368 6f74 4167 656e 7428 6c6c 6d5f  roShotAgent(llm_
+00001470: 6368 6169 6e3d 6c6c 6d5f 6368 6169 6e2c  chain=llm_chain,
+00001480: 2061 6c6c 6f77 6564 5f74 6f6f 6c73 3d74   allowed_tools=t
+00001490: 6f6f 6c5f 6e61 6d65 7329 0a61 6765 6e74  ool_names).agent
+000014a0: 5f65 7865 6375 746f 7220 3d20 4167 656e  _executor = Agen
+000014b0: 7445 7865 6375 746f 722e 6672 6f6d 5f61  tExecutor.from_a
+000014c0: 6765 6e74 5f61 6e64 5f74 6f6f 6c73 2861  gent_and_tools(a
+000014d0: 6765 6e74 3d61 6765 6e74 2c20 746f 6f6c  gent=agent, tool
+000014e0: 733d 746f 6f6c 732c 2076 6572 626f 7365  s=tools, verbose
+000014f0: 3d54 7275 6529 0a61 6765 6e74 5f65 7865  =True).agent_exe
+00001500: 6375 746f 722e 7275 6e28 2248 6f77 206d  cutor.run("How m
+00001510: 616e 7920 7065 6f70 6c65 206c 6976 6520  any people live 
+00001520: 696e 2063 616e 6164 6120 6173 206f 6620  in canada as of 
+00001530: 3230 3233 3f22 290a 6060 600a 0a23 2323  2023?").```..###
+00001540: 2320 4f75 7470 7574 0a0a 0a60 6060 7465  # Output...```te
+00001550: 7874 0a3e 2045 6e74 6572 696e 6720 6e65  xt.> Entering ne
+00001560: 7720 4167 656e 7445 7865 6375 746f 7220  w AgentExecutor 
+00001570: 6368 6169 6e2e 2e2e 0a54 686f 7567 6874  chain....Thought
+00001580: 3a20 4920 6e65 6564 2074 6f20 6669 6e64  : I need to find
+00001590: 206f 7574 2074 6865 2070 6f70 756c 6174   out the populat
+000015a0: 696f 6e20 6f66 2043 616e 6164 610a 4163  ion of Canada.Ac
+000015b0: 7469 6f6e 3a20 5365 6172 6368 0a41 6374  tion: Search.Act
+000015c0: 696f 6e20 496e 7075 743a 2050 6f70 756c  ion Input: Popul
+000015d0: 6174 696f 6e20 6f66 2043 616e 6164 6120  ation of Canada 
+000015e0: 3230 3233 0a4f 6273 6572 7661 7469 6f6e  2023.Observation
+000015f0: 3a20 5468 6520 6375 7272 656e 7420 706f  : The current po
+00001600: 7075 6c61 7469 6f6e 206f 6620 4361 6e61  pulation of Cana
+00001610: 6461 2069 7320 3338 2c36 3130 2c34 3437  da is 38,610,447
+00001620: 2061 7320 6f66 2053 6174 7572 6461 792c   as of Saturday,
+00001630: 2046 6562 7275 6172 7920 3138 2c20 3230   February 18, 20
+00001640: 3233 2c20 6261 7365 6420 6f6e 2057 6f72  23, based on Wor
+00001650: 6c64 6f6d 6574 6572 2065 6c61 626f 7261  ldometer elabora
+00001660: 7469 6f6e 206f 6620 7468 6520 6c61 7465  tion of the late
+00001670: 7374 2055 6e69 7465 6420 4e61 7469 6f6e  st United Nation
+00001680: 7320 6461 7461 2e20 4361 6e61 6461 2032  s data. Canada 2
+00001690: 3032 3020 706f 7075 6c61 7469 6f6e 2069  020 population i
+000016a0: 7320 6573 7469 6d61 7465 6420 6174 2033  s estimated at 3
+000016b0: 372c 3734 322c 3135 3420 7065 6f70 6c65  7,742,154 people
+000016c0: 2061 7420 6d69 6420 7965 6172 2061 6363   at mid year acc
+000016d0: 6f72 6469 6e67 2074 6f20 554e 2064 6174  ording to UN dat
+000016e0: 612e 0a54 686f 7567 6874 3a20 4920 6e6f  a..Thought: I no
+000016f0: 7720 6b6e 6f77 2074 6865 2066 696e 616c  w know the final
+00001700: 2061 6e73 7765 720a 4669 6e61 6c20 416e   answer.Final An
+00001710: 7377 6572 3a20 4172 7272 2c20 4361 6e61  swer: Arrr, Cana
+00001720: 6461 2062 6520 6861 7669 6e27 2033 382c  da be havin' 38,
+00001730: 3631 302c 3434 3720 7363 616c 6c79 7761  610,447 scallywa
+00001740: 6773 206c 6976 696e 2720 7468 6572 6520  gs livin' there 
+00001750: 6173 206f 6620 3230 3233 210a 0a3e 2046  as of 2023!..> F
+00001760: 696e 6973 6865 6420 6368 6169 6e2e 0a60  inished chain..`
+00001770: 6060 0a0a 3c2f 6465 7461 696c 733e 0a0a  ``..</details>..
+00001780: 2323 2320 5374 6570 2031 3a20 0a0a 2a2a  ### Step 1: ..**
+00001790: 5265 6661 6374 6f72 2079 6f75 7220 636f  Refactor your co
+000017a0: 6465 2074 6f20 6675 6e63 7469 6f6e 2873  de to function(s
+000017b0: 2920 7468 6174 2073 686f 756c 6420 6265  ) that should be
+000017c0: 2073 6572 7665 6420 7769 7468 2060 4073   served with `@s
+000017d0: 6572 7669 6e67 6020 6465 636f 7261 746f  erving` decorato
+000017e0: 722a 2a0a 0a0a 3c64 6574 6169 6c73 3e0a  r**...<details>.
+000017f0: 3c73 756d 6d61 7279 3e53 686f 7720 7570  <summary>Show up
+00001800: 6461 7465 6420 6167 656e 7420 636f 6465  dated agent code
+00001810: 2028 6170 702e 7079 293c 2f73 756d 6d61   (app.py)</summa
+00001820: 7279 3e0a 0a60 6060 7079 7468 6f6e 0a23  ry>..```python.#
+00001830: 2061 7070 2e70 790a 6672 6f6d 206c 616e   app.py.from lan
+00001840: 6763 6861 696e 2069 6d70 6f72 7420 4c4c  gchain import LL
+00001850: 4d43 6861 696e 2c20 4f70 656e 4149 2c20  MChain, OpenAI, 
+00001860: 5365 7270 4150 4957 7261 7070 6572 0a66  SerpAPIWrapper.f
+00001870: 726f 6d20 6c61 6e67 6368 6169 6e2e 6167  rom langchain.ag
+00001880: 656e 7473 2069 6d70 6f72 7420 4167 656e  ents import Agen
+00001890: 7445 7865 6375 746f 722c 2054 6f6f 6c2c  tExecutor, Tool,
+000018a0: 205a 6572 6f53 686f 7441 6765 6e74 0a0a   ZeroShotAgent..
+000018b0: 6672 6f6d 206c 6373 6572 7665 2069 6d70  from lcserve imp
+000018c0: 6f72 7420 7365 7276 696e 670a 0a0a 4073  ort serving...@s
+000018d0: 6572 7669 6e67 0a64 6566 2061 736b 2869  erving.def ask(i
+000018e0: 6e70 7574 3a20 7374 7229 202d 3e20 7374  nput: str) -> st
+000018f0: 723a 0a20 2020 2073 6561 7263 6820 3d20  r:.    search = 
+00001900: 5365 7270 4150 4957 7261 7070 6572 2829  SerpAPIWrapper()
+00001910: 0a20 2020 2074 6f6f 6c73 203d 205b 0a20  .    tools = [. 
+00001920: 2020 2020 2020 2054 6f6f 6c28 0a20 2020         Tool(.   
+00001930: 2020 2020 2020 2020 206e 616d 653d 2253           name="S
+00001940: 6561 7263 6822 2c0a 2020 2020 2020 2020  earch",.        
+00001950: 2020 2020 6675 6e63 3d73 6561 7263 682e      func=search.
+00001960: 7275 6e2c 0a20 2020 2020 2020 2020 2020  run,.           
+00001970: 2064 6573 6372 6970 7469 6f6e 3d22 7573   description="us
+00001980: 6566 756c 2066 6f72 2077 6865 6e20 796f  eful for when yo
+00001990: 7520 6e65 6564 2074 6f20 616e 7377 6572  u need to answer
+000019a0: 2071 7565 7374 696f 6e73 2061 626f 7574   questions about
+000019b0: 2063 7572 7265 6e74 2065 7665 6e74 7322   current events"
+000019c0: 2c0a 2020 2020 2020 2020 290a 2020 2020  ,.        ).    
+000019d0: 5d0a 2020 2020 7072 6566 6978 203d 2022  ].    prefix = "
+000019e0: 2222 416e 7377 6572 2074 6865 2066 6f6c  ""Answer the fol
+000019f0: 6c6f 7769 6e67 2071 7565 7374 696f 6e73  lowing questions
+00001a00: 2061 7320 6265 7374 2079 6f75 2063 616e   as best you can
+00001a10: 2c20 6275 7420 7370 6561 6b69 6e67 2061  , but speaking a
+00001a20: 7320 6120 7069 7261 7465 206d 6967 6874  s a pirate might
+00001a30: 2073 7065 616b 2e20 596f 7520 6861 7665   speak. You have
+00001a40: 2061 6363 6573 7320 746f 2074 6865 2066   access to the f
+00001a50: 6f6c 6c6f 7769 6e67 2074 6f6f 6c73 3a22  ollowing tools:"
+00001a60: 2222 0a20 2020 2073 7566 6669 7820 3d20  "".    suffix = 
+00001a70: 2222 2242 6567 696e 2120 5265 6d65 6d62  """Begin! Rememb
+00001a80: 6572 2074 6f20 7370 6561 6b20 6173 2061  er to speak as a
+00001a90: 2070 6972 6174 6520 7768 656e 2067 6976   pirate when giv
+00001aa0: 696e 6720 796f 7572 2066 696e 616c 2061  ing your final a
+00001ab0: 6e73 7765 722e 2055 7365 206c 6f74 7320  nswer. Use lots 
+00001ac0: 6f66 2022 4172 6773 220a 0a20 2020 2051  of "Args"..    Q
+00001ad0: 7565 7374 696f 6e3a 207b 696e 7075 747d  uestion: {input}
+00001ae0: 0a20 2020 207b 6167 656e 745f 7363 7261  .    {agent_scra
+00001af0: 7463 6870 6164 7d22 2222 0a0a 2020 2020  tchpad}"""..    
+00001b00: 7072 6f6d 7074 203d 205a 6572 6f53 686f  prompt = ZeroSho
+00001b10: 7441 6765 6e74 2e63 7265 6174 655f 7072  tAgent.create_pr
+00001b20: 6f6d 7074 280a 2020 2020 2020 2020 746f  ompt(.        to
+00001b30: 6f6c 732c 0a20 2020 2020 2020 2070 7265  ols,.        pre
+00001b40: 6669 783d 7072 6566 6978 2c0a 2020 2020  fix=prefix,.    
+00001b50: 2020 2020 7375 6666 6978 3d73 7566 6669      suffix=suffi
+00001b60: 782c 0a20 2020 2020 2020 2069 6e70 7574  x,.        input
+00001b70: 5f76 6172 6961 626c 6573 3d5b 2269 6e70  _variables=["inp
+00001b80: 7574 222c 2022 6167 656e 745f 7363 7261  ut", "agent_scra
+00001b90: 7463 6870 6164 225d 2c0a 2020 2020 290a  tchpad"],.    ).
+00001ba0: 0a20 2020 2070 7269 6e74 2870 726f 6d70  .    print(promp
+00001bb0: 742e 7465 6d70 6c61 7465 290a 0a20 2020  t.template)..   
+00001bc0: 206c 6c6d 5f63 6861 696e 203d 204c 4c4d   llm_chain = LLM
+00001bd0: 4368 6169 6e28 6c6c 6d3d 4f70 656e 4149  Chain(llm=OpenAI
+00001be0: 2874 656d 7065 7261 7475 7265 3d30 292c  (temperature=0),
+00001bf0: 2070 726f 6d70 743d 7072 6f6d 7074 290a   prompt=prompt).
+00001c00: 2020 2020 746f 6f6c 5f6e 616d 6573 203d      tool_names =
+00001c10: 205b 746f 6f6c 2e6e 616d 6520 666f 7220   [tool.name for 
+00001c20: 746f 6f6c 2069 6e20 746f 6f6c 735d 0a20  tool in tools]. 
+00001c30: 2020 2061 6765 6e74 203d 205a 6572 6f53     agent = ZeroS
+00001c40: 686f 7441 6765 6e74 286c 6c6d 5f63 6861  hotAgent(llm_cha
+00001c50: 696e 3d6c 6c6d 5f63 6861 696e 2c20 616c  in=llm_chain, al
+00001c60: 6c6f 7765 645f 746f 6f6c 733d 746f 6f6c  lowed_tools=tool
+00001c70: 5f6e 616d 6573 290a 0a20 2020 2061 6765  _names)..    age
+00001c80: 6e74 5f65 7865 6375 746f 7220 3d20 4167  nt_executor = Ag
+00001c90: 656e 7445 7865 6375 746f 722e 6672 6f6d  entExecutor.from
+00001ca0: 5f61 6765 6e74 5f61 6e64 5f74 6f6f 6c73  _agent_and_tools
+00001cb0: 280a 2020 2020 2020 2020 6167 656e 743d  (.        agent=
+00001cc0: 6167 656e 742c 2074 6f6f 6c73 3d74 6f6f  agent, tools=too
+00001cd0: 6c73 2c20 7665 7262 6f73 653d 5472 7565  ls, verbose=True
+00001ce0: 0a20 2020 2029 0a0a 2020 2020 7265 7475  .    )..    retu
+00001cf0: 726e 2061 6765 6e74 5f65 7865 6375 746f  rn agent_executo
+00001d00: 722e 7275 6e28 696e 7075 7429 0a0a 6966  r.run(input)..if
+00001d10: 205f 5f6e 616d 655f 5f20 3d3d 2022 5f5f   __name__ == "__
+00001d20: 6d61 696e 5f5f 223a 0a20 2020 2061 736b  main__":.    ask
+00001d30: 2827 486f 7720 6d61 6e79 2070 656f 706c  ('How many peopl
+00001d40: 6520 6c69 7665 2069 6e20 6361 6e61 6461  e live in canada
+00001d50: 2061 7320 6f66 2032 3032 333f 2729 0a60   as of 2023?').`
+00001d60: 6060 0a0a 3c2f 6465 7461 696c 733e 0a0a  ``..</details>..
+00001d70: 0a23 2323 2323 2057 6861 7420 6368 616e  .##### What chan
+00001d80: 6765 643f 0a0a 2d20 5765 206d 6f76 6564  ged?..- We moved
+00001d90: 206f 7572 2063 6f64 6520 746f 2061 6e20   our code to an 
+00001da0: 6061 736b 6020 6675 6e63 7469 6f6e 2e0a  `ask` function..
+00001db0: 2d20 4164 6465 6420 7479 7065 2068 696e  - Added type hin
+00001dc0: 7473 2074 6f20 7468 6520 6675 6e63 7469  ts to the functi
+00001dd0: 6f6e 2070 6172 616d 6574 6572 7320 2869  on parameters (i
+00001de0: 6e70 7574 2061 6e64 206f 7574 7075 7429  nput and output)
+00001df0: 2c20 736f 2041 5049 2064 6566 696e 6974  , so API definit
+00001e00: 696f 6e20 6361 6e20 6265 2067 656e 6572  ion can be gener
+00001e10: 6174 6564 2e0a 2d20 496d 706f 7274 6564  ated..- Imported
+00001e20: 2060 6672 6f6d 206c 6373 6572 7665 2069   `from lcserve i
+00001e30: 6d70 6f72 7420 7365 7276 696e 6760 2061  mport serving` a
+00001e40: 6e64 2061 6464 6564 2060 4073 6572 7669  nd added `@servi
+00001e50: 6e67 6020 6465 636f 7261 746f 7220 746f  ng` decorator to
+00001e60: 2074 6865 2060 6173 6b60 2066 756e 6374   the `ask` funct
+00001e70: 696f 6e2e 0a2d 2041 6464 6564 2060 6966  ion..- Added `if
+00001e80: 205f 5f6e 616d 655f 5f20 3d3d 2022 5f5f   __name__ == "__
+00001e90: 6d61 696e 5f5f 223a 6020 626c 6f63 6b20  main__":` block 
+00001ea0: 746f 2074 6573 7420 7468 6520 6675 6e63  to test the func
+00001eb0: 7469 6f6e 206c 6f63 616c 6c79 2e0a 0a2d  tion locally...-
+00001ec0: 2d2d 0a0a 2323 2320 5374 6570 2032 3a0a  --..### Step 2:.
+00001ed0: 0a2a 2a43 7265 6174 6520 6120 6072 6571  .**Create a `req
+00001ee0: 7569 7265 6d65 6e74 732e 7478 7460 2066  uirements.txt` f
+00001ef0: 696c 6520 696e 2079 6f75 7220 6170 7020  ile in your app 
+00001f00: 6469 7265 6374 6f72 7920 746f 2065 6e73  directory to ens
+00001f10: 7572 6520 616c 6c20 6e65 6365 7373 6172  ure all necessar
+00001f20: 7920 6465 7065 6e64 656e 6369 6573 2061  y dependencies a
+00001f30: 7265 2069 6e73 7461 6c6c 6564 2e2a 2a0a  re installed.**.
+00001f40: 0a3c 6465 7461 696c 733e 0a3c 7375 6d6d  .<details>.<summ
+00001f50: 6172 793e 5368 6f77 2072 6571 7569 7265  ary>Show require
+00001f60: 6d65 6e74 732e 7478 743c 2f73 756d 6d61  ments.txt</summa
+00001f70: 7279 3e0a 0a60 6060 7465 7874 0a23 2072  ry>..```text.# r
+00001f80: 6571 7569 7265 6d65 6e74 732e 7478 740a  equirements.txt.
+00001f90: 6f70 656e 6169 0a67 6f6f 676c 652d 7365  openai.google-se
+00001fa0: 6172 6368 2d72 6573 756c 7473 0a60 6060  arch-results.```
+00001fb0: 0a3c 2f64 6574 6169 6c73 3e0a 0a2d 2d2d  .</details>..---
+00001fc0: 200a 0a23 2323 2053 7465 7020 333a 0a0a   ..### Step 3:..
+00001fd0: 2a2a 5275 6e20 606c 632d 7365 7276 6520  **Run `lc-serve 
+00001fe0: 6465 706c 6f79 206c 6f63 616c 2061 7070  deploy local app
+00001ff0: 6020 746f 2074 6573 7420 796f 7572 2041  ` to test your A
+00002000: 5049 206c 6f63 616c 6c79 2e2a 2a0a 0a3e  PI locally.**..>
+00002010: 2060 6170 7060 2069 7320 7468 6520 6e61   `app` is the na
+00002020: 6d65 206f 6620 7468 6520 6d6f 6475 6c65  me of the module
+00002030: 2074 6861 7420 636f 6e74 6169 6e73 2074   that contains t
+00002040: 6865 2060 6173 6b60 2066 756e 6374 696f  he `ask` functio
+00002050: 6e2e 0a0a 6060 6062 6173 680a 6c63 2d73  n...```bash.lc-s
+00002060: 6572 7665 2064 6570 6c6f 7920 6c6f 6361  erve deploy loca
+00002070: 6c20 6170 700a 6060 600a 0a3c 6465 7461  l app.```..<deta
+00002080: 696c 733e 0a3c 7375 6d6d 6172 793e 5368  ils>.<summary>Sh
+00002090: 6f77 206f 7574 7075 743c 2f73 756d 6d61  ow output</summa
+000020a0: 7279 3e0a 0a60 6060 7465 7874 0ae2 9480  ry>..```text....
+000020b0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000020c0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000020d0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000020e0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000020f0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002100: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002110: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002120: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002130: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002140: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002150: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002160: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002170: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002180: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002190: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000021a0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000021b0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000021c0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000021d0: e294 80e2 9480 e294 80e2 9480 e294 8020  ............... 
+000021e0: f09f 8e89 2046 6c6f 7720 6973 2072 6561  .... Flow is rea
+000021f0: 6479 2074 6f20 7365 7276 6521 20e2 9480  dy to serve! ...
+00002200: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002210: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002220: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002230: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002240: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002250: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002260: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002270: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002280: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002290: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000022a0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000022b0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000022c0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000022d0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000022e0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000022f0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002300: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002310: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002320: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002330: 9480 0ae2 95ad e294 80e2 9480 e294 80e2  ................
+00002340: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002350: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002360: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002370: 9480 e294 80e2 9480 e294 80e2 9480 20f0  .............. .
+00002380: 9f94 9720 456e 6470 6f69 6e74 20e2 9480  ... Endpoint ...
 00002390: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
 000023a0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
 000023b0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
 000023c0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000023d0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-000023e0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000023f0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002400: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002410: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00002420: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002430: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002440: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00002450: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002460: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002470: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00002480: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002490: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-000024a0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000024b0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000024c0: 9480 20f0 9f8e 8920 466c 6f77 2069 7320  .. .... Flow is 
-000024d0: 7265 6164 7920 746f 2073 6572 7665 2120  ready to serve! 
-000024e0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000024f0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002500: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00002510: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002520: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002530: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00002540: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002550: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002560: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00002570: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002580: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002590: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000025a0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000025b0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000023d0: 9480 e294 80e2 95ae 0ae2 9482 2020 e29b  ............  ..
+000023e0: 9320 2020 5072 6f74 6f63 6f6c 2020 2020  .   Protocol    
+000023f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002410: 2020 2020 2048 5454 5020 20e2 9482 0ae2       HTTP  .....
+00002420: 9482 2020 f09f 8fa0 2020 2020 204c 6f63  ..  ....     Loc
+00002430: 616c 2020 2020 2020 2020 2020 2020 2020  al              
+00002440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002450: 2020 2030 2e30 2e30 2e30 3a38 3038 3020     0.0.0.0:8080 
+00002460: 20e2 9482 0ae2 9482 2020 f09f 9492 2020   .......  ....  
+00002470: 2050 7269 7661 7465 2020 2020 2020 2020   Private        
+00002480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002490: 2020 3139 322e 3136 382e 3239 2e31 3835    192.168.29.185
+000024a0: 3a38 3038 3020 20e2 9482 0ae2 9482 2020  :8080  .......  
+000024b0: f09f 8c8d 2020 2020 5075 626c 6963 2020  ....    Public  
+000024c0: 3234 3035 3a32 3031 3a64 3030 373a 6538  2405:201:d007:e8
+000024d0: 6537 3a32 6333 333a 6366 3865 3a65 6436  e7:2c33:cf8e:ed6
+000024e0: 363a 3230 3138 3a38 3038 3020 20e2 9482  6:2018:8080  ...
+000024f0: 0ae2 95b0 e294 80e2 9480 e294 80e2 9480  ................
+00002500: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002510: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002520: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002530: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002540: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002550: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002560: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002570: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002580: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002590: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000025a0: 9480 e294 80e2 9480 e294 80e2 95af 0ae2  ................
+000025b0: 95ad e294 80e2 9480 e294 80e2 9480 e294  ................
 000025c0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000025d0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000025e0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000025d0: e294 8020 f09f 928e 2048 5454 5020 6578  ... .... HTTP ex
+000025e0: 7465 6e73 696f 6e20 e294 80e2 9480 e294  tension ........
 000025f0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00002600: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002610: 9480 e294 800a e295 ade2 9480 e294 80e2  ................
-00002620: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002630: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00002640: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002650: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002660: 8020 f09f 9497 2045 6e64 706f 696e 7420  . .... Endpoint 
-00002670: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002600: e294 80e2 9480 e294 80e2 9480 e295 ae0a  ................
+00002610: e294 8220 20f0 9f92 ac20 2020 2020 2020  ...  ....       
+00002620: 2020 2053 7761 6767 6572 2055 4920 2020     Swagger UI   
+00002630: 2020 2020 202e 2e2e 2f64 6f63 7320 20e2       .../docs  .
+00002640: 9482 0ae2 9482 2020 f09f 939a 2020 2020  ......  ....    
+00002650: 2020 2020 2020 2020 2020 2052 6564 6f63             Redoc
+00002660: 2020 2020 2020 202e 2e2e 2f72 6564 6f63         .../redoc
+00002670: 2020 e294 820a e295 b0e2 9480 e294 80e2    ..............
 00002680: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
 00002690: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
 000026a0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000026b0: 9480 e294 80e2 9480 e295 ae0a e294 8220  ............... 
-000026c0: 20e2 9b93 2020 2050 726f 746f 636f 6c20   ...   Protocol 
-000026d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000026e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000026f0: 2020 2020 2020 2020 4854 5450 2020 e294          HTTP  ..
-00002700: 820a e294 8220 20f0 9f8f a020 2020 2020  .....  ....     
-00002710: 4c6f 6361 6c20 2020 2020 2020 2020 2020  Local           
-00002720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002730: 2020 2020 2020 302e 302e 302e 303a 3830        0.0.0.0:80
-00002740: 3830 2020 e294 820a e294 8220 20f0 9f94  80  .......  ...
-00002750: 9220 2020 5072 6976 6174 6520 2020 2020  .   Private     
-00002760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002770: 2020 2020 2031 3932 2e31 3638 2e32 392e       192.168.29.
-00002780: 3138 353a 3830 3830 2020 e294 820a e294  185:8080  ......
-00002790: 8220 20f0 9f8c 8d20 2020 2050 7562 6c69  .  ....    Publi
-000027a0: 6320 2032 3430 353a 3230 313a 6430 3037  c  2405:201:d007
-000027b0: 3a65 3865 373a 3263 3333 3a63 6638 653a  :e8e7:2c33:cf8e:
-000027c0: 6564 3636 3a32 3031 383a 3830 3830 2020  ed66:2018:8080  
-000027d0: e294 820a e295 b0e2 9480 e294 80e2 9480  ................
-000027e0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000027f0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002800: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00002810: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002820: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002830: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00002840: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002850: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002860: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00002870: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002880: 9480 e294 80e2 9480 e294 80e2 9480 e295  ................
-00002890: af0a e295 ade2 9480 e294 80e2 9480 e294  ................
-000028a0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000028b0: e294 80e2 9480 20f0 9f92 8e20 4854 5450  ...... .... HTTP
-000028c0: 2065 7874 656e 7369 6f6e 20e2 9480 e294   extension .....
-000028d0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000028e0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000028f0: 95ae 0ae2 9482 2020 f09f 92ac 2020 2020  ......  ....    
-00002900: 2020 2020 2020 5377 6167 6765 7220 5549        Swagger UI
-00002910: 2020 2020 2020 2020 2e2e 2e2f 646f 6373          .../docs
-00002920: 2020 e294 820a e294 8220 20f0 9f93 9a20    .......  .... 
-00002930: 2020 2020 2020 2020 2020 2020 2020 5265                Re
-00002940: 646f 6320 2020 2020 2020 2e2e 2e2f 7265  doc       .../re
-00002950: 646f 6320 20e2 9482 0ae2 95b0 e294 80e2  doc  ...........
-00002960: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002970: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00002980: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002990: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-000029a0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000029b0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000029c0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-000029d0: 80e2 9480 e294 80e2 9480 e295 af0a 6060  ..............``
-000029e0: 600a 0a3c 2f64 6574 6169 6c73 3e0a 0a0a  `..</details>...
-000029f0: 4c65 7427 7320 6f70 656e 2074 6865 205b  Let's open the [
-00002a00: 5377 6167 6765 7220 5549 5d28 6874 7470  Swagger UI](http
-00002a10: 3a2f 2f6c 6f63 616c 686f 7374 3a38 3038  ://localhost:808
-00002a20: 302f 646f 6373 2920 746f 2074 6573 7420  0/docs) to test 
-00002a30: 6f75 7220 4150 4920 6c6f 6361 6c6c 792e  our API locally.
-00002a40: 2057 6974 6820 6054 7279 2069 7420 6f75   With `Try it ou
-00002a50: 7460 2062 7574 746f 6e2c 2077 6520 6361  t` button, we ca
-00002a60: 6e20 7465 7374 206f 7572 2041 5049 2077  n test our API w
-00002a70: 6974 6820 6469 6666 6572 656e 7420 696e  ith different in
-00002a80: 7075 7473 2e0a 0a0a 3c64 6574 6169 6c73  puts....<details
-00002a90: 3e0a 3c73 756d 6d61 7279 3e53 686f 7720  >.<summary>Show 
-00002aa0: 5377 6167 6765 7220 5549 3c2f 7375 6d6d  Swagger UI</summ
-00002ab0: 6172 793e 0a0a 215b 4c6f 6361 6c20 5377  ary>..![Local Sw
-00002ac0: 6167 6765 7220 5549 5d28 2e67 6974 6875  agger UI](.githu
-00002ad0: 622f 696d 6167 6573 2f6c 6f63 616c 2d73  b/images/local-s
-00002ae0: 7761 6767 6572 2d75 692e 706e 6729 0a0a  wagger-ui.png)..
-00002af0: 3c2f 6465 7461 696c 733e 0a0a 4c65 7427  </details>..Let'
-00002b00: 7320 7465 7374 206f 7572 206c 6f63 616c  s test our local
-00002b10: 2041 5049 2077 6974 6820 6048 6f77 206d   API with `How m
-00002b20: 616e 7920 7065 6f70 6c65 206c 6976 6520  any people live 
-00002b30: 696e 2063 616e 6164 6120 6173 206f 6620  in canada as of 
-00002b40: 3230 3233 3f60 2069 6e70 7574 2077 6974  2023?` input wit
-00002b50: 6820 6120 6355 524c 2063 6f6d 6d61 6e64  h a cURL command
-00002b60: 2e0a 0a60 6060 6261 7368 0a63 7572 6c20  ...```bash.curl 
-00002b70: 2d58 2027 504f 5354 2720 5c0a 2020 2768  -X 'POST' \.  'h
-00002b80: 7474 703a 2f2f 6c6f 6361 6c68 6f73 743a  ttp://localhost:
-00002b90: 3830 3830 2f61 736b 2720 5c0a 2020 2d48  8080/ask' \.  -H
-00002ba0: 2027 6163 6365 7074 3a20 6170 706c 6963   'accept: applic
-00002bb0: 6174 696f 6e2f 6a73 6f6e 2720 5c0a 2020  ation/json' \.  
-00002bc0: 2d48 2027 436f 6e74 656e 742d 5479 7065  -H 'Content-Type
-00002bd0: 3a20 6170 706c 6963 6174 696f 6e2f 6a73  : application/js
-00002be0: 6f6e 2720 5c0a 2020 2d64 2027 7b0a 2020  on' \.  -d '{.  
-00002bf0: 2269 6e70 7574 223a 2022 486f 7720 6d61  "input": "How ma
-00002c00: 6e79 2070 656f 706c 6520 6c69 7665 2069  ny people live i
-00002c10: 6e20 6361 6e61 6461 2061 7320 6f66 2032  n canada as of 2
-00002c20: 3032 333f 222c 0a20 2022 656e 7673 223a  023?",.  "envs":
-00002c30: 207b 0a20 2020 2022 4f50 454e 4149 5f41   {.    "OPENAI_A
-00002c40: 5049 5f4b 4559 223a 2022 2722 247b 4f50  PI_KEY": "'"${OP
-00002c50: 454e 4149 5f41 5049 5f4b 4559 7d22 2722  ENAI_API_KEY}"'"
-00002c60: 2c0a 2020 2020 2253 4552 5041 5049 5f41  ,.    "SERPAPI_A
-00002c70: 5049 5f4b 4559 223a 2022 2722 247b 5345  PI_KEY": "'"${SE
-00002c80: 5250 4150 495f 4150 495f 4b45 597d 2227  RPAPI_API_KEY}"'
-00002c90: 220a 2020 7d0a 7d27 0a60 6060 0a0a 6060  ".  }.}'.```..``
-00002ca0: 606a 736f 6e0a 7b0a 2020 2272 6573 756c  `json.{.  "resul
-00002cb0: 7422 3a20 2241 7272 722c 2074 6865 7265  t": "Arrr, there
-00002cc0: 2062 6520 3338 2c36 3435 2c36 3730 2070   be 38,645,670 p
-00002cd0: 656f 706c 6520 6c69 7669 6e27 2069 6e20  eople livin' in 
-00002ce0: 4361 6e61 6461 2061 7320 6f66 2032 3032  Canada as of 202
-00002cf0: 3321 222c 0a20 2022 6572 726f 7222 3a20  3!",.  "error": 
-00002d00: 2222 2c0a 2020 2273 7464 6f75 7422 3a20  "",.  "stdout": 
-00002d10: 2241 6e73 7765 7220 7468 6520 666f 6c6c  "Answer the foll
-00002d20: 6f77 696e 6720 7175 6573 7469 6f6e 7320  owing questions 
-00002d30: 6173 2062 6573 7420 796f 7520 6361 6e2c  as best you can,
-00002d40: 2062 7574 2073 7065 616b 696e 6720 6173   but speaking as
-00002d50: 2061 2070 6972 6174 6520 6d69 6768 7420   a pirate might 
-00002d60: 7370 6561 6b2e 2059 6f75 2068 6176 6520  speak. You have 
-00002d70: 6163 6365 7373 2074 6f20 7468 6520 666f  access to the fo
-00002d80: 6c6c 6f77 696e 6720 746f 6f6c 733a 5c6e  llowing tools:\n
-00002d90: 5c6e 5365 6172 6368 3a20 7573 6566 756c  \nSearch: useful
-00002da0: 2066 6f72 2077 6865 6e20 796f 7520 6e65   for when you ne
-00002db0: 6564 2074 6f20 616e 7377 6572 2071 7565  ed to answer que
-00002dc0: 7374 696f 6e73 2061 626f 7574 2063 7572  stions about cur
-00002dd0: 7265 6e74 2065 7665 6e74 735c 6e5c 6e55  rent events\n\nU
-00002de0: 7365 2074 6865 2066 6f6c 6c6f 7769 6e67  se the following
-00002df0: 2066 6f72 6d61 743a 5c6e 5c6e 5175 6573   format:\n\nQues
-00002e00: 7469 6f6e 3a20 7468 6520 696e 7075 7420  tion: the input 
-00002e10: 7175 6573 7469 6f6e 2079 6f75 206d 7573  question you mus
-00002e20: 7420 616e 7377 6572 5c6e 5468 6f75 6768  t answer\nThough
-00002e30: 743a 2079 6f75 2073 686f 756c 6420 616c  t: you should al
-00002e40: 7761 7973 2074 6869 6e6b 2061 626f 7574  ways think about
-00002e50: 2077 6861 7420 746f 2064 6f5c 6e41 6374   what to do\nAct
-00002e60: 696f 6e3a 2074 6865 2061 6374 696f 6e20  ion: the action 
-00002e70: 746f 2074 616b 652c 2073 686f 756c 6420  to take, should 
-00002e80: 6265 206f 6e65 206f 6620 5b53 6561 7263  be one of [Searc
-00002e90: 685d 5c6e 4163 7469 6f6e 2049 6e70 7574  h]\nAction Input
-00002ea0: 3a20 7468 6520 696e 7075 7420 746f 2074  : the input to t
-00002eb0: 6865 2061 6374 696f 6e5c 6e4f 6273 6572  he action\nObser
-00002ec0: 7661 7469 6f6e 3a20 7468 6520 7265 7375  vation: the resu
-00002ed0: 6c74 206f 6620 7468 6520 6163 7469 6f6e  lt of the action
-00002ee0: 5c6e 2e2e 2e20 2874 6869 7320 5468 6f75  \n... (this Thou
-00002ef0: 6768 742f 4163 7469 6f6e 2f41 6374 696f  ght/Action/Actio
-00002f00: 6e20 496e 7075 742f 4f62 7365 7276 6174  n Input/Observat
-00002f10: 696f 6e20 6361 6e20 7265 7065 6174 204e  ion can repeat N
-00002f20: 2074 696d 6573 295c 6e54 686f 7567 6874   times)\nThought
-00002f30: 3a20 4920 6e6f 7720 6b6e 6f77 2074 6865  : I now know the
-00002f40: 2066 696e 616c 2061 6e73 7765 725c 6e46   final answer\nF
-00002f50: 696e 616c 2041 6e73 7765 723a 2074 6865  inal Answer: the
-00002f60: 2066 696e 616c 2061 6e73 7765 7220 746f   final answer to
-00002f70: 2074 6865 206f 7269 6769 6e61 6c20 696e   the original in
-00002f80: 7075 7420 7175 6573 7469 6f6e 5c6e 5c6e  put question\n\n
-00002f90: 4265 6769 6e21 2052 656d 656d 6265 7220  Begin! Remember 
-00002fa0: 746f 2073 7065 616b 2061 7320 6120 7069  to speak as a pi
-00002fb0: 7261 7465 2077 6865 6e20 6769 7669 6e67  rate when giving
-00002fc0: 2079 6f75 7220 6669 6e61 6c20 616e 7377   your final answ
-00002fd0: 6572 2e20 5573 6520 6c6f 7473 206f 6620  er. Use lots of 
-00002fe0: 5c22 4172 6773 5c22 5c6e 5c6e 2020 2020  \"Args\"\n\n    
-00002ff0: 5175 6573 7469 6f6e 3a20 7b69 6e70 7574  Question: {input
-00003000: 7d5c 6e20 2020 207b 6167 656e 745f 7363  }\n    {agent_sc
-00003010: 7261 7463 6870 6164 7d5c 6e5c 6e5c 6e5c  ratchpad}\n\n\n\
-00003020: 7530 3031 625b 316d 3e20 456e 7465 7269  u001b[1m> Enteri
-00003030: 6e67 206e 6577 2041 6765 6e74 4578 6563  ng new AgentExec
-00003040: 7574 6f72 2063 6861 696e 2e2e 2e5c 7530  utor chain...\u0
-00003050: 3031 625b 306d 5c6e 5c75 3030 3162 5b33  01b[0m\n\u001b[3
-00003060: 323b 316d 5c75 3030 3162 5b31 3b33 6d5c  2;1m\u001b[1;3m\
-00003070: 6e54 686f 7567 6874 3a20 4920 6e65 6564  nThought: I need
-00003080: 2074 6f20 6669 6e64 206f 7574 2068 6f77   to find out how
-00003090: 206d 616e 7920 7065 6f70 6c65 206c 6976   many people liv
-000030a0: 6520 696e 2043 616e 6164 615c 6e41 6374  e in Canada\nAct
-000030b0: 696f 6e3a 2053 6561 7263 685c 6e41 6374  ion: Search\nAct
-000030c0: 696f 6e20 496e 7075 743a 2048 6f77 206d  ion Input: How m
-000030d0: 616e 7920 7065 6f70 6c65 206c 6976 6520  any people live 
-000030e0: 696e 2043 616e 6164 6120 6173 206f 6620  in Canada as of 
-000030f0: 3230 3233 5c75 3030 3162 5b30 6d5c 6e4f  2023\u001b[0m\nO
-00003100: 6273 6572 7661 7469 6f6e 3a20 5c75 3030  bservation: \u00
-00003110: 3162 5b33 363b 316d 5c75 3030 3162 5b31  1b[36;1m\u001b[1
-00003120: 3b33 6d54 6865 2063 7572 7265 6e74 2070  ;3mThe current p
-00003130: 6f70 756c 6174 696f 6e20 6f66 2043 616e  opulation of Can
-00003140: 6164 6120 6973 2033 382c 3634 352c 3637  ada is 38,645,67
-00003150: 3020 6173 206f 6620 5765 646e 6573 6461  0 as of Wednesda
-00003160: 792c 204d 6172 6368 2032 392c 2032 3032  y, March 29, 202
-00003170: 332c 2062 6173 6564 206f 6e20 576f 726c  3, based on Worl
-00003180: 646f 6d65 7465 7220 656c 6162 6f72 6174  dometer elaborat
-00003190: 696f 6e20 6f66 2074 6865 206c 6174 6573  ion of the lates
-000031a0: 7420 556e 6974 6564 204e 6174 696f 6e73  t United Nations
-000031b0: 2064 6174 612e 5c75 3030 3162 5b30 6d5c   data.\u001b[0m\
-000031c0: 6e54 686f 7567 6874 3a5c 7530 3031 625b  nThought:\u001b[
-000031d0: 3332 3b31 6d5c 7530 3031 625b 313b 336d  32;1m\u001b[1;3m
-000031e0: 2049 206e 6f77 206b 6e6f 7720 7468 6520   I now know the 
-000031f0: 6669 6e61 6c20 616e 7377 6572 5c6e 4669  final answer\nFi
-00003200: 6e61 6c20 416e 7377 6572 3a20 4172 7272  nal Answer: Arrr
-00003210: 2c20 7468 6572 6520 6265 2033 382c 3634  , there be 38,64
-00003220: 352c 3637 3020 7065 6f70 6c65 206c 6976  5,670 people liv
-00003230: 696e 2720 696e 2043 616e 6164 6120 6173  in' in Canada as
-00003240: 206f 6620 3230 3233 215c 7530 3031 625b   of 2023!\u001b[
-00003250: 306d 5c6e 5c6e 5c75 3030 3162 5b31 6d3e  0m\n\n\u001b[1m>
-00003260: 2046 696e 6973 6865 6420 6368 6169 6e2e   Finished chain.
-00003270: 5c75 3030 3162 5b30 6d22 0a7d 0a60 6060  \u001b[0m".}.```
-00003280: 0a0a 2323 2323 2320 5768 6174 2068 6170  ..##### What hap
-00003290: 7065 6e65 643f 0a0a 2d20 6050 4f53 5420  pened?..- `POST 
-000032a0: 2f61 736b 6020 6973 2067 656e 6572 6174  /ask` is generat
-000032b0: 6564 2066 726f 6d20 6061 736b 6020 6675  ed from `ask` fu
-000032c0: 6e63 7469 6f6e 2064 6566 696e 6564 2069  nction defined i
-000032d0: 6e20 6061 7070 2e70 7960 2e0a 2d20 6069  n `app.py`..- `i
-000032e0: 6e70 7574 6020 6973 2061 6e20 6172 6772  nput` is an argr
-000032f0: 6d65 6e74 2064 6566 696e 6564 2069 6e20  ment defined in 
-00003300: 6061 736b 6020 6675 6e63 7469 6f6e 2e20  `ask` function. 
-00003310: 0a2d 2060 656e 7673 6020 6973 2061 2064  .- `envs` is a d
-00003320: 6963 7469 6f6e 6172 7920 6f66 2065 6e76  ictionary of env
-00003330: 6972 6f6e 6d65 6e74 2076 6172 6961 626c  ironment variabl
-00003340: 6573 2074 6861 7420 7769 6c6c 2062 6520  es that will be 
-00003350: 7061 7373 6564 2074 6f20 616c 6c20 7468  passed to all th
-00003360: 6520 6675 6e63 7469 6f6e 7320 6465 636f  e functions deco
-00003370: 7261 7465 6420 7769 7468 2060 4073 6572  rated with `@ser
-00003380: 7669 6e67 6020 6465 636f 7261 746f 722e  ving` decorator.
-00003390: 0a2d 2072 6574 7572 6e20 7479 7065 206f  .- return type o
-000033a0: 6620 6061 736b 6020 6675 6e63 7469 6f6e  f `ask` function
-000033b0: 2069 7320 6073 7472 602e 2053 6f2c 2060   is `str`. So, `
-000033c0: 7265 7375 6c74 6020 776f 756c 6420 6361  result` would ca
-000033d0: 7272 7920 7468 6520 7265 7475 726e 2076  rry the return v
-000033e0: 616c 7565 206f 6620 6061 736b 6020 6675  alue of `ask` fu
-000033f0: 6e63 7469 6f6e 2e0a 2d20 4966 2074 6865  nction..- If the
-00003400: 7265 2069 7320 616e 2065 7272 6f72 2c20  re is an error, 
-00003410: 6065 7272 6f72 6020 776f 756c 6420 6361  `error` would ca
-00003420: 7272 7920 7468 6520 6572 726f 7220 6d65  rry the error me
-00003430: 7373 6167 652e 0a2d 2060 7374 646f 7574  ssage..- `stdout
-00003440: 6020 776f 756c 6420 6361 7272 7920 7468  ` would carry th
-00003450: 6520 6f75 7470 7574 206f 6620 7468 6520  e output of the 
-00003460: 6675 6e63 7469 6f6e 2064 6563 6f72 6174  function decorat
-00003470: 6564 2077 6974 6820 6040 7365 7276 696e  ed with `@servin
-00003480: 6760 2064 6563 6f72 6174 6f72 2e0a 0a0a  g` decorator....
-00003490: 2d2d 2d0a 0a23 2323 2053 7465 7020 343a  ---..### Step 4:
-000034a0: 0a0a 2a2a 5275 6e20 606c 632d 7365 7276  ..**Run `lc-serv
-000034b0: 6520 6465 706c 6f79 206a 636c 6f75 6420  e deploy jcloud 
-000034c0: 6170 7060 2074 6f20 6465 706c 6f79 2079  app` to deploy y
-000034d0: 6f75 7220 4150 4920 746f 204a 696e 6120  our API to Jina 
-000034e0: 4149 2043 6c6f 7564 2e2a 2a0a 0a60 6060  AI Cloud.**..```
-000034f0: 6261 7368 0a23 204c 6f67 696e 2074 6f20  bash.# Login to 
-00003500: 4a69 6e61 2041 4920 436c 6f75 640a 6a69  Jina AI Cloud.ji
-00003510: 6e61 2061 7574 6820 6c6f 6769 6e0a 0a23  na auth login..#
-00003520: 2044 6570 6c6f 7920 796f 7572 2061 7070   Deploy your app
-00003530: 2074 6f20 4a69 6e61 2041 4920 436c 6f75   to Jina AI Clou
-00003540: 640a 6c63 2d73 6572 7665 2064 6570 6c6f  d.lc-serve deplo
-00003550: 7920 6a63 6c6f 7564 2061 7070 0a60 6060  y jcloud app.```
-00003560: 0a0a 3c64 6574 6169 6c73 3e0a 3c73 756d  ..<details>.<sum
-00003570: 6d61 7279 3e53 686f 7720 636f 6d70 6c65  mary>Show comple
-00003580: 7465 206f 7574 7075 743c 2f73 756d 6d61  te output</summa
-00003590: 7279 3e0a 0a60 6060 7465 7874 0ae2 a087  ry>..```text....
-000035a0: 2050 7573 6869 6e67 2060 2f74 6d70 2f74   Pushing `/tmp/t
-000035b0: 6d70 376b 7435 7171 726e 6020 2e2e 2ef0  mp7kt5qqrn` ....
-000035c0: 9f94 9020 596f 7520 6172 6520 6c6f 6767  ... You are logg
-000035d0: 6564 2069 6e20 746f 204a 696e 6120 4149  ed in to Jina AI
-000035e0: 2061 7320 2a2a 2a2e 2054 6f20 6c6f 6720   as ***. To log 
-000035f0: 6f75 742c 2075 7365 206a 696e 6120 6175  out, use jina au
-00003600: 7468 206c 6f67 6f75 742e 0ae2 95ad e294  th logout.......
-00003610: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00003620: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00003630: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00003640: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00003650: e294 80e2 9480 e294 80e2 9480 2050 7562  ............ Pub
-00003660: 6c69 7368 6564 20e2 9480 e294 80e2 9480  lished .........
+000026b0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000026c0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000026d0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000026e0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000026f0: 80e2 9480 e294 80e2 95af 0a60 6060 0a0a  ...........```..
+00002700: 3c2f 6465 7461 696c 733e 0a0a 0a4c 6574  </details>...Let
+00002710: 2773 206f 7065 6e20 7468 6520 5b53 7761  's open the [Swa
+00002720: 6767 6572 2055 495d 2868 7474 703a 2f2f  gger UI](http://
+00002730: 6c6f 6361 6c68 6f73 743a 3830 3830 2f64  localhost:8080/d
+00002740: 6f63 7329 2074 6f20 7465 7374 206f 7572  ocs) to test our
+00002750: 2041 5049 206c 6f63 616c 6c79 2e20 5769   API locally. Wi
+00002760: 7468 2060 5472 7920 6974 206f 7574 6020  th `Try it out` 
+00002770: 6275 7474 6f6e 2c20 7765 2063 616e 2074  button, we can t
+00002780: 6573 7420 6f75 7220 4150 4920 7769 7468  est our API with
+00002790: 2064 6966 6665 7265 6e74 2069 6e70 7574   different input
+000027a0: 732e 0a0a 0a3c 6465 7461 696c 733e 0a3c  s....<details>.<
+000027b0: 7375 6d6d 6172 793e 5368 6f77 2053 7761  summary>Show Swa
+000027c0: 6767 6572 2055 493c 2f73 756d 6d61 7279  gger UI</summary
+000027d0: 3e0a 0a21 5b4c 6f63 616c 2053 7761 6767  >..![Local Swagg
+000027e0: 6572 2055 495d 282e 6769 7468 7562 2f69  er UI](.github/i
+000027f0: 6d61 6765 732f 6c6f 6361 6c2d 7377 6167  mages/local-swag
+00002800: 6765 722d 7569 2e70 6e67 290a 0a3c 2f64  ger-ui.png)..</d
+00002810: 6574 6169 6c73 3e0a 0a4c 6574 2773 2074  etails>..Let's t
+00002820: 6573 7420 6f75 7220 6c6f 6361 6c20 4150  est our local AP
+00002830: 4920 7769 7468 2060 486f 7720 6d61 6e79  I with `How many
+00002840: 2070 656f 706c 6520 6c69 7665 2069 6e20   people live in 
+00002850: 6361 6e61 6461 2061 7320 6f66 2032 3032  canada as of 202
+00002860: 333f 6020 696e 7075 7420 7769 7468 2061  3?` input with a
+00002870: 2063 5552 4c20 636f 6d6d 616e 642e 0a0a   cURL command...
+00002880: 6060 6062 6173 680a 6375 726c 202d 5820  ```bash.curl -X 
+00002890: 2750 4f53 5427 205c 0a20 2027 6874 7470  'POST' \.  'http
+000028a0: 3a2f 2f6c 6f63 616c 686f 7374 3a38 3038  ://localhost:808
+000028b0: 302f 6173 6b27 205c 0a20 202d 4820 2761  0/ask' \.  -H 'a
+000028c0: 6363 6570 743a 2061 7070 6c69 6361 7469  ccept: applicati
+000028d0: 6f6e 2f6a 736f 6e27 205c 0a20 202d 4820  on/json' \.  -H 
+000028e0: 2743 6f6e 7465 6e74 2d54 7970 653a 2061  'Content-Type: a
+000028f0: 7070 6c69 6361 7469 6f6e 2f6a 736f 6e27  pplication/json'
+00002900: 205c 0a20 202d 6420 277b 0a20 2022 696e   \.  -d '{.  "in
+00002910: 7075 7422 3a20 2248 6f77 206d 616e 7920  put": "How many 
+00002920: 7065 6f70 6c65 206c 6976 6520 696e 2063  people live in c
+00002930: 616e 6164 6120 6173 206f 6620 3230 3233  anada as of 2023
+00002940: 3f22 2c0a 2020 2265 6e76 7322 3a20 7b0a  ?",.  "envs": {.
+00002950: 2020 2020 224f 5045 4e41 495f 4150 495f      "OPENAI_API_
+00002960: 4b45 5922 3a20 2227 2224 7b4f 5045 4e41  KEY": "'"${OPENA
+00002970: 495f 4150 495f 4b45 597d 2227 222c 0a20  I_API_KEY}"'",. 
+00002980: 2020 2022 5345 5250 4150 495f 4150 495f     "SERPAPI_API_
+00002990: 4b45 5922 3a20 2227 2224 7b53 4552 5041  KEY": "'"${SERPA
+000029a0: 5049 5f41 5049 5f4b 4559 7d22 2722 0a20  PI_API_KEY}"'". 
+000029b0: 207d 0a7d 270a 6060 600a 0a60 6060 6a73   }.}'.```..```js
+000029c0: 6f6e 0a7b 0a20 2022 7265 7375 6c74 223a  on.{.  "result":
+000029d0: 2022 4172 7272 2c20 7468 6572 6520 6265   "Arrr, there be
+000029e0: 2033 382c 3634 352c 3637 3020 7065 6f70   38,645,670 peop
+000029f0: 6c65 206c 6976 696e 2720 696e 2043 616e  le livin' in Can
+00002a00: 6164 6120 6173 206f 6620 3230 3233 2122  ada as of 2023!"
+00002a10: 2c0a 2020 2265 7272 6f72 223a 2022 222c  ,.  "error": "",
+00002a20: 0a20 2022 7374 646f 7574 223a 2022 416e  .  "stdout": "An
+00002a30: 7377 6572 2074 6865 2066 6f6c 6c6f 7769  swer the followi
+00002a40: 6e67 2071 7565 7374 696f 6e73 2061 7320  ng questions as 
+00002a50: 6265 7374 2079 6f75 2063 616e 2c20 6275  best you can, bu
+00002a60: 7420 7370 6561 6b69 6e67 2061 7320 6120  t speaking as a 
+00002a70: 7069 7261 7465 206d 6967 6874 2073 7065  pirate might spe
+00002a80: 616b 2e20 596f 7520 6861 7665 2061 6363  ak. You have acc
+00002a90: 6573 7320 746f 2074 6865 2066 6f6c 6c6f  ess to the follo
+00002aa0: 7769 6e67 2074 6f6f 6c73 3a5c 6e5c 6e53  wing tools:\n\nS
+00002ab0: 6561 7263 683a 2075 7365 6675 6c20 666f  earch: useful fo
+00002ac0: 7220 7768 656e 2079 6f75 206e 6565 6420  r when you need 
+00002ad0: 746f 2061 6e73 7765 7220 7175 6573 7469  to answer questi
+00002ae0: 6f6e 7320 6162 6f75 7420 6375 7272 656e  ons about curren
+00002af0: 7420 6576 656e 7473 5c6e 5c6e 5573 6520  t events\n\nUse 
+00002b00: 7468 6520 666f 6c6c 6f77 696e 6720 666f  the following fo
+00002b10: 726d 6174 3a5c 6e5c 6e51 7565 7374 696f  rmat:\n\nQuestio
+00002b20: 6e3a 2074 6865 2069 6e70 7574 2071 7565  n: the input que
+00002b30: 7374 696f 6e20 796f 7520 6d75 7374 2061  stion you must a
+00002b40: 6e73 7765 725c 6e54 686f 7567 6874 3a20  nswer\nThought: 
+00002b50: 796f 7520 7368 6f75 6c64 2061 6c77 6179  you should alway
+00002b60: 7320 7468 696e 6b20 6162 6f75 7420 7768  s think about wh
+00002b70: 6174 2074 6f20 646f 5c6e 4163 7469 6f6e  at to do\nAction
+00002b80: 3a20 7468 6520 6163 7469 6f6e 2074 6f20  : the action to 
+00002b90: 7461 6b65 2c20 7368 6f75 6c64 2062 6520  take, should be 
+00002ba0: 6f6e 6520 6f66 205b 5365 6172 6368 5d5c  one of [Search]\
+00002bb0: 6e41 6374 696f 6e20 496e 7075 743a 2074  nAction Input: t
+00002bc0: 6865 2069 6e70 7574 2074 6f20 7468 6520  he input to the 
+00002bd0: 6163 7469 6f6e 5c6e 4f62 7365 7276 6174  action\nObservat
+00002be0: 696f 6e3a 2074 6865 2072 6573 756c 7420  ion: the result 
+00002bf0: 6f66 2074 6865 2061 6374 696f 6e5c 6e2e  of the action\n.
+00002c00: 2e2e 2028 7468 6973 2054 686f 7567 6874  .. (this Thought
+00002c10: 2f41 6374 696f 6e2f 4163 7469 6f6e 2049  /Action/Action I
+00002c20: 6e70 7574 2f4f 6273 6572 7661 7469 6f6e  nput/Observation
+00002c30: 2063 616e 2072 6570 6561 7420 4e20 7469   can repeat N ti
+00002c40: 6d65 7329 5c6e 5468 6f75 6768 743a 2049  mes)\nThought: I
+00002c50: 206e 6f77 206b 6e6f 7720 7468 6520 6669   now know the fi
+00002c60: 6e61 6c20 616e 7377 6572 5c6e 4669 6e61  nal answer\nFina
+00002c70: 6c20 416e 7377 6572 3a20 7468 6520 6669  l Answer: the fi
+00002c80: 6e61 6c20 616e 7377 6572 2074 6f20 7468  nal answer to th
+00002c90: 6520 6f72 6967 696e 616c 2069 6e70 7574  e original input
+00002ca0: 2071 7565 7374 696f 6e5c 6e5c 6e42 6567   question\n\nBeg
+00002cb0: 696e 2120 5265 6d65 6d62 6572 2074 6f20  in! Remember to 
+00002cc0: 7370 6561 6b20 6173 2061 2070 6972 6174  speak as a pirat
+00002cd0: 6520 7768 656e 2067 6976 696e 6720 796f  e when giving yo
+00002ce0: 7572 2066 696e 616c 2061 6e73 7765 722e  ur final answer.
+00002cf0: 2055 7365 206c 6f74 7320 6f66 205c 2241   Use lots of \"A
+00002d00: 7267 735c 225c 6e5c 6e20 2020 2051 7565  rgs\"\n\n    Que
+00002d10: 7374 696f 6e3a 207b 696e 7075 747d 5c6e  stion: {input}\n
+00002d20: 2020 2020 7b61 6765 6e74 5f73 6372 6174      {agent_scrat
+00002d30: 6368 7061 647d 5c6e 5c6e 5c6e 5c75 3030  chpad}\n\n\n\u00
+00002d40: 3162 5b31 6d3e 2045 6e74 6572 696e 6720  1b[1m> Entering 
+00002d50: 6e65 7720 4167 656e 7445 7865 6375 746f  new AgentExecuto
+00002d60: 7220 6368 6169 6e2e 2e2e 5c75 3030 3162  r chain...\u001b
+00002d70: 5b30 6d5c 6e5c 7530 3031 625b 3332 3b31  [0m\n\u001b[32;1
+00002d80: 6d5c 7530 3031 625b 313b 336d 5c6e 5468  m\u001b[1;3m\nTh
+00002d90: 6f75 6768 743a 2049 206e 6565 6420 746f  ought: I need to
+00002da0: 2066 696e 6420 6f75 7420 686f 7720 6d61   find out how ma
+00002db0: 6e79 2070 656f 706c 6520 6c69 7665 2069  ny people live i
+00002dc0: 6e20 4361 6e61 6461 5c6e 4163 7469 6f6e  n Canada\nAction
+00002dd0: 3a20 5365 6172 6368 5c6e 4163 7469 6f6e  : Search\nAction
+00002de0: 2049 6e70 7574 3a20 486f 7720 6d61 6e79   Input: How many
+00002df0: 2070 656f 706c 6520 6c69 7665 2069 6e20   people live in 
+00002e00: 4361 6e61 6461 2061 7320 6f66 2032 3032  Canada as of 202
+00002e10: 335c 7530 3031 625b 306d 5c6e 4f62 7365  3\u001b[0m\nObse
+00002e20: 7276 6174 696f 6e3a 205c 7530 3031 625b  rvation: \u001b[
+00002e30: 3336 3b31 6d5c 7530 3031 625b 313b 336d  36;1m\u001b[1;3m
+00002e40: 5468 6520 6375 7272 656e 7420 706f 7075  The current popu
+00002e50: 6c61 7469 6f6e 206f 6620 4361 6e61 6461  lation of Canada
+00002e60: 2069 7320 3338 2c36 3435 2c36 3730 2061   is 38,645,670 a
+00002e70: 7320 6f66 2057 6564 6e65 7364 6179 2c20  s of Wednesday, 
+00002e80: 4d61 7263 6820 3239 2c20 3230 3233 2c20  March 29, 2023, 
+00002e90: 6261 7365 6420 6f6e 2057 6f72 6c64 6f6d  based on Worldom
+00002ea0: 6574 6572 2065 6c61 626f 7261 7469 6f6e  eter elaboration
+00002eb0: 206f 6620 7468 6520 6c61 7465 7374 2055   of the latest U
+00002ec0: 6e69 7465 6420 4e61 7469 6f6e 7320 6461  nited Nations da
+00002ed0: 7461 2e5c 7530 3031 625b 306d 5c6e 5468  ta.\u001b[0m\nTh
+00002ee0: 6f75 6768 743a 5c75 3030 3162 5b33 323b  ought:\u001b[32;
+00002ef0: 316d 5c75 3030 3162 5b31 3b33 6d20 4920  1m\u001b[1;3m I 
+00002f00: 6e6f 7720 6b6e 6f77 2074 6865 2066 696e  now know the fin
+00002f10: 616c 2061 6e73 7765 725c 6e46 696e 616c  al answer\nFinal
+00002f20: 2041 6e73 7765 723a 2041 7272 722c 2074   Answer: Arrr, t
+00002f30: 6865 7265 2062 6520 3338 2c36 3435 2c36  here be 38,645,6
+00002f40: 3730 2070 656f 706c 6520 6c69 7669 6e27  70 people livin'
+00002f50: 2069 6e20 4361 6e61 6461 2061 7320 6f66   in Canada as of
+00002f60: 2032 3032 3321 5c75 3030 3162 5b30 6d5c   2023!\u001b[0m\
+00002f70: 6e5c 6e5c 7530 3031 625b 316d 3e20 4669  n\n\u001b[1m> Fi
+00002f80: 6e69 7368 6564 2063 6861 696e 2e5c 7530  nished chain.\u0
+00002f90: 3031 625b 306d 220a 7d0a 6060 600a 0a23  01b[0m".}.```..#
+00002fa0: 2323 2323 2057 6861 7420 6861 7070 656e  #### What happen
+00002fb0: 6564 3f0a 0a2d 2060 504f 5354 202f 6173  ed?..- `POST /as
+00002fc0: 6b60 2069 7320 6765 6e65 7261 7465 6420  k` is generated 
+00002fd0: 6672 6f6d 2060 6173 6b60 2066 756e 6374  from `ask` funct
+00002fe0: 696f 6e20 6465 6669 6e65 6420 696e 2060  ion defined in `
+00002ff0: 6170 702e 7079 602e 0a2d 2060 696e 7075  app.py`..- `inpu
+00003000: 7460 2069 7320 616e 2061 7267 726d 656e  t` is an argrmen
+00003010: 7420 6465 6669 6e65 6420 696e 2060 6173  t defined in `as
+00003020: 6b60 2066 756e 6374 696f 6e2e 200a 2d20  k` function. .- 
+00003030: 6065 6e76 7360 2069 7320 6120 6469 6374  `envs` is a dict
+00003040: 696f 6e61 7279 206f 6620 656e 7669 726f  ionary of enviro
+00003050: 6e6d 656e 7420 7661 7269 6162 6c65 7320  nment variables 
+00003060: 7468 6174 2077 696c 6c20 6265 2070 6173  that will be pas
+00003070: 7365 6420 746f 2061 6c6c 2074 6865 2066  sed to all the f
+00003080: 756e 6374 696f 6e73 2064 6563 6f72 6174  unctions decorat
+00003090: 6564 2077 6974 6820 6040 7365 7276 696e  ed with `@servin
+000030a0: 6760 2064 6563 6f72 6174 6f72 2e0a 2d20  g` decorator..- 
+000030b0: 7265 7475 726e 2074 7970 6520 6f66 2060  return type of `
+000030c0: 6173 6b60 2066 756e 6374 696f 6e20 6973  ask` function is
+000030d0: 2060 7374 7260 2e20 536f 2c20 6072 6573   `str`. So, `res
+000030e0: 756c 7460 2077 6f75 6c64 2063 6172 7279  ult` would carry
+000030f0: 2074 6865 2072 6574 7572 6e20 7661 6c75   the return valu
+00003100: 6520 6f66 2060 6173 6b60 2066 756e 6374  e of `ask` funct
+00003110: 696f 6e2e 0a2d 2049 6620 7468 6572 6520  ion..- If there 
+00003120: 6973 2061 6e20 6572 726f 722c 2060 6572  is an error, `er
+00003130: 726f 7260 2077 6f75 6c64 2063 6172 7279  ror` would carry
+00003140: 2074 6865 2065 7272 6f72 206d 6573 7361   the error messa
+00003150: 6765 2e0a 2d20 6073 7464 6f75 7460 2077  ge..- `stdout` w
+00003160: 6f75 6c64 2063 6172 7279 2074 6865 206f  ould carry the o
+00003170: 7574 7075 7420 6f66 2074 6865 2066 756e  utput of the fun
+00003180: 6374 696f 6e20 6465 636f 7261 7465 6420  ction decorated 
+00003190: 7769 7468 2060 4073 6572 7669 6e67 6020  with `@serving` 
+000031a0: 6465 636f 7261 746f 722e 0a0a 0a2d 2d2d  decorator....---
+000031b0: 0a0a 2323 2320 5374 6570 2034 3a0a 0a2a  ..### Step 4:..*
+000031c0: 2a52 756e 2060 6c63 2d73 6572 7665 2064  *Run `lc-serve d
+000031d0: 6570 6c6f 7920 6a63 6c6f 7564 2061 7070  eploy jcloud app
+000031e0: 6020 746f 2064 6570 6c6f 7920 796f 7572  ` to deploy your
+000031f0: 2041 5049 2074 6f20 4a69 6e61 2041 4920   API to Jina AI 
+00003200: 436c 6f75 642e 2a2a 0a0a 6060 6062 6173  Cloud.**..```bas
+00003210: 680a 2320 4c6f 6769 6e20 746f 204a 696e  h.# Login to Jin
+00003220: 6120 4149 2043 6c6f 7564 0a6a 696e 6120  a AI Cloud.jina 
+00003230: 6175 7468 206c 6f67 696e 0a0a 2320 4465  auth login..# De
+00003240: 706c 6f79 2079 6f75 7220 6170 7020 746f  ploy your app to
+00003250: 204a 696e 6120 4149 2043 6c6f 7564 0a6c   Jina AI Cloud.l
+00003260: 632d 7365 7276 6520 6465 706c 6f79 206a  c-serve deploy j
+00003270: 636c 6f75 6420 6170 700a 6060 600a 0a3c  cloud app.```..<
+00003280: 6465 7461 696c 733e 0a3c 7375 6d6d 6172  details>.<summar
+00003290: 793e 5368 6f77 2063 6f6d 706c 6574 6520  y>Show complete 
+000032a0: 6f75 7470 7574 3c2f 7375 6d6d 6172 793e  output</summary>
+000032b0: 0a0a 6060 6074 6578 740a e2a0 8720 5075  ..```text.... Pu
+000032c0: 7368 696e 6720 602f 746d 702f 746d 7037  shing `/tmp/tmp7
+000032d0: 6b74 3571 7172 6e60 202e 2e2e f09f 9490  kt5qqrn` .......
+000032e0: 2059 6f75 2061 7265 206c 6f67 6765 6420   You are logged 
+000032f0: 696e 2074 6f20 4a69 6e61 2041 4920 6173  in to Jina AI as
+00003300: 202a 2a2a 2e20 546f 206c 6f67 206f 7574   ***. To log out
+00003310: 2c20 7573 6520 6a69 6e61 2061 7574 6820  , use jina auth 
+00003320: 6c6f 676f 7574 2e0a e295 ade2 9480 e294  logout..........
+00003330: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00003340: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00003350: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00003360: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00003370: e294 80e2 9480 e294 8020 5075 626c 6973  ......... Publis
+00003380: 6865 6420 e294 80e2 9480 e294 80e2 9480  hed ............
+00003390: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000033a0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000033b0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000033c0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000033d0: 9480 e294 80e2 95ae 0ae2 9482 2020 2020  ............    
+000033e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000033f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003410: 2020 2020 2020 2020 2020 2020 e294 820a              ....
+00003420: e294 8220 2020 f09f 939b 204e 616d 6520  ...   .... Name 
+00003430: 2020 2020 2020 2020 2020 6e2d 3634 6131            n-64a1
+00003440: 3520 2020 2020 2020 2020 2020 2020 2020  5               
+00003450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003460: 2020 2020 20e2 9482 0ae2 9482 2020 20f0       .......   .
+00003470: 9f94 9720 4a69 6e61 2048 7562 2055 524c  ... Jina Hub URL
+00003480: 2020 2068 7474 7073 3a2f 2f63 6c6f 7564     https://cloud
+00003490: 2e6a 696e 612e 6169 2f65 7865 6375 746f  .jina.ai/executo
+000034a0: 722f 3670 317a 696f 3837 2f20 2020 e294  r/6p1zio87/   ..
+000034b0: 820a e294 8220 2020 f09f 9180 2056 6973  .....   .... Vis
+000034c0: 6962 696c 6974 7920 2020 2020 7075 626c  ibility     publ
+000034d0: 6963 2020 2020 2020 2020 2020 2020 2020  ic              
+000034e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000034f0: 2020 2020 2020 20e2 9482 0ae2 9482 2020         .......  
+00003500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003530: 2020 2020 2020 2020 2020 2020 2020 e294                ..
+00003540: 820a e295 b0e2 9480 e294 80e2 9480 e294  ................
+00003550: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00003560: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00003570: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00003580: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00003590: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000035a0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000035b0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000035c0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000035d0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000035e0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000035f0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00003600: 9480 e294 80e2 95af 0ae2 95ad e294 80e2  ................
+00003610: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00003620: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00003630: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00003640: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00003650: 8020 f09f 8e89 2046 6c6f 7720 6973 2061  . .... Flow is a
+00003660: 7661 696c 6162 6c65 2120 e294 80e2 9480  vailable! ......
 00003670: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
 00003680: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
 00003690: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
 000036a0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000036b0: 9480 e294 80e2 9480 e295 ae0a e294 8220  ............... 
+000036b0: 95ae 0ae2 9482 2020 2020 2020 2020 2020  ......          
 000036c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000036d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000036e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000036f0: 2020 2020 2020 2020 2020 2020 2020 20e2                 .
-00003700: 9482 0ae2 9482 2020 20f0 9f93 9b20 4e61  ......   .... Na
-00003710: 6d65 2020 2020 2020 2020 2020 206e 2d36  me           n-6
-00003720: 3461 3135 2020 2020 2020 2020 2020 2020  4a15            
+000036f0: 2020 2020 2020 2020 2020 20e2 9482 0ae2             .....
+00003700: 9482 2020 2049 4420 2020 2020 2020 2020  ..   ID         
+00003710: 2020 2020 2020 6c61 6e67 6368 6169 6e2d        langchain-
+00003720: 6565 3461 6566 3537 6439 2020 2020 2020  ee4aef57d9      
 00003730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003740: 2020 2020 2020 2020 e294 820a e294 8220          ....... 
-00003750: 2020 f09f 9497 204a 696e 6120 4875 6220    .... Jina Hub 
-00003760: 5552 4c20 2020 6874 7470 733a 2f2f 636c  URL   https://cl
-00003770: 6f75 642e 6a69 6e61 2e61 692f 6578 6563  oud.jina.ai/exec
-00003780: 7574 6f72 2f36 7031 7a69 6f38 372f 2020  utor/6p1zio87/  
-00003790: 20e2 9482 0ae2 9482 2020 20f0 9f91 8020   .......   .... 
-000037a0: 5669 7369 6269 6c69 7479 2020 2020 2070  Visibility     p
-000037b0: 7562 6c69 6320 2020 2020 2020 2020 2020  ublic           
-000037c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000037d0: 2020 2020 2020 2020 2020 e294 820a e294            ......
-000037e0: 8220 2020 2020 2020 2020 2020 2020 2020  .               
+00003740: 2020 2020 2020 20e2 9482 0ae2 9482 2020         .......  
+00003750: 2047 6174 6577 6179 2028 4874 7470 2920   Gateway (Http) 
+00003760: 2020 6874 7470 733a 2f2f 6c61 6e67 6368    https://langch
+00003770: 6169 6e2d 6565 3461 6566 3537 6439 2d68  ain-ee4aef57d9-h
+00003780: 7474 702e 776f 6c66 2e6a 696e 612e 6169  ttp.wolf.jina.ai
+00003790: 2020 20e2 9482 0ae2 9482 2020 2044 6173     .......   Das
+000037a0: 6862 6f61 7264 2020 2020 2020 2020 6874  hboard        ht
+000037b0: 7470 733a 2f2f 6461 7368 626f 6172 642e  tps://dashboard.
+000037c0: 776f 6c66 2e6a 696e 612e 6169 2f66 6c6f  wolf.jina.ai/flo
+000037d0: 772f 6565 3461 6566 3537 6439 2020 20e2  w/ee4aef57d9   .
+000037e0: 9482 0ae2 9482 2020 2020 2020 2020 2020  ......          
 000037f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00003800: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00003810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003820: 20e2 9482 0ae2 95b0 e294 80e2 9480 e294   ...............
-00003830: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00003840: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00003850: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00003860: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00003870: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00003880: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00003890: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000038a0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000038b0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-000038c0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000038d0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000038e0: 9480 e294 80e2 9480 e295 af0a e295 ade2  ................
+00003820: 2020 2020 2020 2020 2020 20e2 9482 0ae2             .....
+00003830: 95b0 e294 80e2 9480 e294 80e2 9480 e294  ................
+00003840: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00003850: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00003860: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00003870: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00003880: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00003890: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000038a0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000038b0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000038c0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000038d0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000038e0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
 000038f0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00003900: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00003910: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00003920: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00003930: 80e2 9480 20f0 9f8e 8920 466c 6f77 2069  .... .... Flow i
-00003940: 7320 6176 6169 6c61 626c 6521 20e2 9480  s available! ...
-00003950: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00003960: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00003970: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00003980: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00003990: 9480 e295 ae0a e294 8220 2020 2020 2020  .........       
-000039a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000039b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000039c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000039d0: 2020 2020 2020 2020 2020 2020 2020 e294                ..
-000039e0: 820a e294 8220 2020 4944 2020 2020 2020  .....   ID      
-000039f0: 2020 2020 2020 2020 206c 616e 6763 6861           langcha
-00003a00: 696e 2d65 6534 6165 6635 3764 3920 2020  in-ee4aef57d9   
-00003a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003a20: 2020 2020 2020 2020 2020 e294 820a e294            ......
-00003a30: 8220 2020 4761 7465 7761 7920 2848 7474  .   Gateway (Htt
-00003a40: 7029 2020 2068 7474 7073 3a2f 2f6c 616e  p)   https://lan
-00003a50: 6763 6861 696e 2d65 6534 6165 6635 3764  gchain-ee4aef57d
-00003a60: 392d 6874 7470 2e77 6f6c 662e 6a69 6e61  9-http.wolf.jina
-00003a70: 2e61 6920 2020 e294 820a e294 8220 2020  .ai   .......   
-00003a80: 4461 7368 626f 6172 6420 2020 2020 2020  Dashboard       
-00003a90: 2068 7474 7073 3a2f 2f64 6173 6862 6f61   https://dashboa
-00003aa0: 7264 2e77 6f6c 662e 6a69 6e61 2e61 692f  rd.wolf.jina.ai/
-00003ab0: 666c 6f77 2f65 6534 6165 6635 3764 3920  flow/ee4aef57d9 
-00003ac0: 2020 e294 820a e294 8220 2020 2020 2020    .......       
-00003ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003b00: 2020 2020 2020 2020 2020 2020 2020 e294                ..
-00003b10: 820a e295 b0e2 9480 e294 80e2 9480 e294  ................
+00003900: 80e2 95af 0a60 6060 0a3c 2f64 6574 6169  .....```.</detai
+00003910: 6c73 3e0a 0a0a 6060 6074 6578 740a e295  ls>...```text...
+00003920: ade2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00003930: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00003940: 9480 e294 80e2 9480 e294 80e2 94ac e294  ................
+00003950: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00003960: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00003970: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00003980: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00003990: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000039a0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000039b0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000039c0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000039d0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000039e0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000039f0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00003a00: 9480 e294 80e2 95ae 0ae2 9482 2041 7070  ............ App
+00003a10: 4944 2020 2020 2020 2020 e294 8220 2020  ID        ...   
+00003a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003a30: 206c 616e 6763 6861 696e 2d65 6534 6165   langchain-ee4ae
+00003a40: 6635 3764 3920 2020 2020 2020 2020 2020  f57d9           
+00003a50: 2020 2020 2020 2020 2020 e294 820a e294            ......
+00003a60: 9ce2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00003a70: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00003a80: 9480 e294 80e2 9480 e294 80e2 94bc e294  ................
+00003a90: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00003aa0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00003ab0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00003ac0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00003ad0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00003ae0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00003af0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00003b00: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00003b10: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
 00003b20: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
 00003b30: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00003b40: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00003b50: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00003b60: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00003b70: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00003b80: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00003b90: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00003ba0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00003bb0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00003bc0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00003bd0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00003be0: 80e2 9480 e295 af0a 6060 600a 3c2f 6465  ........```.</de
-00003bf0: 7461 696c 733e 0a0a 0a60 6060 7465 7874  tails>...```text
-00003c00: 0ae2 95ad e294 80e2 9480 e294 80e2 9480  ................
+00003b40: 9480 e294 80e2 94a4 0ae2 9482 2050 6861  ............ Pha
+00003b50: 7365 2020 2020 2020 2020 e294 8220 2020  se        ...   
+00003b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003b70: 2020 2020 2020 2020 5365 7276 696e 6720          Serving 
+00003b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003b90: 2020 2020 2020 2020 2020 e294 820a e294            ......
+00003ba0: 9ce2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00003bb0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00003bc0: 9480 e294 80e2 9480 e294 80e2 94bc e294  ................
+00003bd0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00003be0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00003bf0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00003c00: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
 00003c10: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
 00003c20: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00003c30: ace2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00003c30: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
 00003c40: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
 00003c50: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
 00003c60: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
 00003c70: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00003c80: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00003c90: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00003ca0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00003cb0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00003cc0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00003cd0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00003ce0: 9480 e294 80e2 9480 e295 ae0a e294 8220  ............... 
-00003cf0: 4170 7049 4420 2020 2020 2020 20e2 9482  AppID        ...
-00003d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003d10: 2020 2020 6c61 6e67 6368 6169 6e2d 6565      langchain-ee
-00003d20: 3461 6566 3537 6439 2020 2020 2020 2020  4aef57d9        
-00003d30: 2020 2020 2020 2020 2020 2020 20e2 9482               ...
-00003d40: 0ae2 949c e294 80e2 9480 e294 80e2 9480  ................
+00003c80: 9480 e294 80e2 94a4 0ae2 9482 2045 6e64  ............ End
+00003c90: 706f 696e 7420 2020 2020 e294 8220 2020  point     ...   
+00003ca0: 2020 2020 6874 7470 733a 2f2f 6c61 6e67      https://lang
+00003cb0: 6368 6169 6e2d 6565 3461 6566 3537 6439  chain-ee4aef57d9
+00003cc0: 2d68 7474 702e 776f 6c66 2e6a 696e 612e  -http.wolf.jina.
+00003cd0: 6169 2020 2020 2020 2020 e294 820a e294  ai        ......
+00003ce0: 9ce2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00003cf0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00003d00: 9480 e294 80e2 9480 e294 80e2 94bc e294  ................
+00003d10: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00003d20: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00003d30: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00003d40: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
 00003d50: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
 00003d60: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00003d70: bce2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00003d70: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
 00003d80: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
 00003d90: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
 00003da0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
 00003db0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00003dc0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00003dd0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00003de0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00003df0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00003e00: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00003e10: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00003e20: 9480 e294 80e2 9480 e294 a40a e294 8220  ............... 
-00003e30: 5068 6173 6520 2020 2020 2020 20e2 9482  Phase        ...
-00003e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003e50: 2020 2020 2020 2020 2020 2053 6572 7669             Servi
-00003e60: 6e67 2020 2020 2020 2020 2020 2020 2020  ng              
-00003e70: 2020 2020 2020 2020 2020 2020 20e2 9482               ...
-00003e80: 0ae2 949c e294 80e2 9480 e294 80e2 9480  ................
+00003dc0: 9480 e294 80e2 94a4 0ae2 9482 2053 7761  ............ Swa
+00003dd0: 6767 6572 2055 4920 2020 e294 8220 2020  gger UI   ...   
+00003de0: 2020 6874 7470 733a 2f2f 6c61 6e67 6368    https://langch
+00003df0: 6169 6e2d 6565 3461 6566 3537 6439 2d68  ain-ee4aef57d9-h
+00003e00: 7474 702e 776f 6c66 2e6a 696e 612e 6169  ttp.wolf.jina.ai
+00003e10: 2f64 6f63 7320 2020 2020 e294 820a e294  /docs     ......
+00003e20: 9ce2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00003e30: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00003e40: 9480 e294 80e2 9480 e294 80e2 94bc e294  ................
+00003e50: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00003e60: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00003e70: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00003e80: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
 00003e90: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
 00003ea0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00003eb0: bce2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00003eb0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
 00003ec0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
 00003ed0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
 00003ee0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
 00003ef0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00003f00: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00003f10: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00003f20: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00003f30: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00003f40: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00003f50: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00003f60: 9480 e294 80e2 9480 e294 a40a e294 8220  ............... 
-00003f70: 456e 6470 6f69 6e74 2020 2020 20e2 9482  Endpoint     ...
-00003f80: 2020 2020 2020 2068 7474 7073 3a2f 2f6c         https://l
-00003f90: 616e 6763 6861 696e 2d65 6534 6165 6635  angchain-ee4aef5
-00003fa0: 3764 392d 6874 7470 2e77 6f6c 662e 6a69  7d9-http.wolf.ji
-00003fb0: 6e61 2e61 6920 2020 2020 2020 20e2 9482  na.ai        ...
-00003fc0: 0ae2 949c e294 80e2 9480 e294 80e2 9480  ................
+00003f00: 9480 e294 80e2 94a4 0ae2 9482 204f 7065  ............ Ope
+00003f10: 6e41 5049 204a 534f 4e20 e294 8220 6874  nAPI JSON ... ht
+00003f20: 7470 733a 2f2f 6c61 6e67 6368 6169 6e2d  tps://langchain-
+00003f30: 6565 3461 6566 3537 6439 2d68 7474 702e  ee4aef57d9-http.
+00003f40: 776f 6c66 2e6a 696e 612e 6169 2f6f 7065  wolf.jina.ai/ope
+00003f50: 6e61 7069 2e6a 736f 6e20 e294 820a e295  napi.json ......
+00003f60: b0e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00003f70: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00003f80: 9480 e294 80e2 9480 e294 80e2 94b4 e294  ................
+00003f90: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00003fa0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00003fb0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00003fc0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
 00003fd0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
 00003fe0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00003ff0: bce2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00003ff0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
 00004000: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
 00004010: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
 00004020: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
 00004030: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00004040: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00004050: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00004060: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00004070: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00004080: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00004090: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000040a0: 9480 e294 80e2 9480 e294 a40a e294 8220  ............... 
-000040b0: 5377 6167 6765 7220 5549 2020 20e2 9482  Swagger UI   ...
-000040c0: 2020 2020 2068 7474 7073 3a2f 2f6c 616e       https://lan
-000040d0: 6763 6861 696e 2d65 6534 6165 6635 3764  gchain-ee4aef57d
-000040e0: 392d 6874 7470 2e77 6f6c 662e 6a69 6e61  9-http.wolf.jina
-000040f0: 2e61 692f 646f 6373 2020 2020 20e2 9482  .ai/docs     ...
-00004100: 0ae2 949c e294 80e2 9480 e294 80e2 9480  ................
-00004110: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00004120: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00004130: bce2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00004140: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00004150: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00004160: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00004170: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00004180: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00004190: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000041a0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000041b0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-000041c0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000041d0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000041e0: 9480 e294 80e2 9480 e294 a40a e294 8220  ............... 
-000041f0: 4f70 656e 4150 4920 4a53 4f4e 20e2 9482  OpenAPI JSON ...
-00004200: 2068 7474 7073 3a2f 2f6c 616e 6763 6861   https://langcha
-00004210: 696e 2d65 6534 6165 6635 3764 392d 6874  in-ee4aef57d9-ht
-00004220: 7470 2e77 6f6c 662e 6a69 6e61 2e61 692f  tp.wolf.jina.ai/
-00004230: 6f70 656e 6170 692e 6a73 6f6e 20e2 9482  openapi.json ...
-00004240: 0ae2 95b0 e294 80e2 9480 e294 80e2 9480  ................
-00004250: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00004260: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00004270: b4e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00004280: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00004290: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-000042a0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000042b0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000042c0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-000042d0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000042e0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000042f0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00004300: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00004310: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00004320: 9480 e294 80e2 9480 e295 af0a 6060 600a  ............```.
-00004330: 0a4c 6574 2773 206f 7065 6e20 7468 6520  .Let's open the 
-00004340: 5377 6167 6765 7220 5549 2074 6f20 7465  Swagger UI to te
-00004350: 7374 206f 7572 2041 5049 206f 6e20 4a69  st our API on Ji
-00004360: 6e61 2041 4920 436c 6f75 642e 2057 6974  na AI Cloud. Wit
-00004370: 6820 6054 7279 2069 7420 6f75 7460 2062  h `Try it out` b
-00004380: 7574 746f 6e2c 2077 6520 6361 6e20 7465  utton, we can te
-00004390: 7374 206f 7572 2041 5049 2077 6974 6820  st our API with 
-000043a0: 6469 6666 6572 656e 7420 696e 7075 7473  different inputs
-000043b0: 2e0a 0a3c 6465 7461 696c 733e 0a3c 7375  ...<details>.<su
-000043c0: 6d6d 6172 793e 5368 6f77 2053 7761 6767  mmary>Show Swagg
-000043d0: 6572 2055 493c 2f73 756d 6d61 7279 3e0a  er UI</summary>.
-000043e0: 0a3c 7020 666c 6f61 743d 2263 656e 7465  .<p float="cente
-000043f0: 7222 3e0a 2020 3c69 6d67 2073 7263 3d22  r">.  <img src="
-00004400: 2e67 6974 6875 622f 696d 6167 6573 2f6a  .github/images/j
-00004410: 636c 6f75 642d 7377 6167 6765 722d 7569  cloud-swagger-ui
-00004420: 2e70 6e67 2220 7769 6474 683d 2234 3030  .png" width="400
-00004430: 2220 2f3e 0a20 203c 696d 6720 7372 633d  " />.  <img src=
-00004440: 222e 6769 7468 7562 2f69 6d61 6765 732f  ".github/images/
-00004450: 6a63 6c6f 7564 2d6f 7065 6e61 7069 2e70  jcloud-openapi.p
-00004460: 6e67 2220 7769 6474 683d 2233 3030 2220  ng" width="300" 
-00004470: 2f3e 0a3c 2f70 3e0a 0a3c 2f64 6574 6169  />.</p>..</detai
-00004480: 6c73 3e0a 0a0a 4c65 7427 7320 7465 7374  ls>...Let's test
-00004490: 2074 6865 2041 5049 206f 6e20 4a43 6c6f   the API on JClo
-000044a0: 7564 2077 6974 6820 6048 6f77 206d 616e  ud with `How man
-000044b0: 7920 7065 6f70 6c65 206c 6976 6520 696e  y people live in
-000044c0: 2063 616e 6164 6120 6173 206f 6620 3230   canada as of 20
-000044d0: 3233 3f60 2069 6e70 7574 2077 6974 6820  23?` input with 
-000044e0: 6120 6355 524c 2063 6f6d 6d61 6e64 2028  a cURL command (
-000044f0: 5265 706c 6163 6520 7468 6520 486f 7374  Replace the Host
-00004500: 6e61 6d65 2077 6974 6820 796f 7572 206f  name with your o
-00004510: 776e 2068 6f73 746e 616d 6529 3a0a 0a60  wn hostname):..`
-00004520: 6060 6261 7368 0a63 7572 6c20 2d58 2027  ``bash.curl -X '
-00004530: 504f 5354 2720 5c0a 2020 2768 7474 7073  POST' \.  'https
-00004540: 3a2f 2f6c 616e 6763 6861 696e 2d65 6534  ://langchain-ee4
-00004550: 6165 6635 3764 392d 6874 7470 2e77 6f6c  aef57d9-http.wol
-00004560: 662e 6a69 6e61 2e61 692f 6173 6b27 205c  f.jina.ai/ask' \
-00004570: 0a20 202d 4820 2761 6363 6570 743a 2061  .  -H 'accept: a
-00004580: 7070 6c69 6361 7469 6f6e 2f6a 736f 6e27  pplication/json'
-00004590: 205c 0a20 202d 4820 2743 6f6e 7465 6e74   \.  -H 'Content
-000045a0: 2d54 7970 653a 2061 7070 6c69 6361 7469  -Type: applicati
-000045b0: 6f6e 2f6a 736f 6e27 205c 0a20 202d 6420  on/json' \.  -d 
-000045c0: 277b 0a20 2022 696e 7075 7422 3a20 2248  '{.  "input": "H
-000045d0: 6f77 206d 616e 7920 7065 6f70 6c65 206c  ow many people l
-000045e0: 6976 6520 696e 2063 616e 6164 6120 6173  ive in canada as
-000045f0: 206f 6620 3230 3233 3f22 2c0a 2020 2265   of 2023?",.  "e
-00004600: 6e76 7322 3a20 7b0a 2020 2020 224f 5045  nvs": {.    "OPE
-00004610: 4e41 495f 4150 495f 4b45 5922 3a20 2227  NAI_API_KEY": "'
-00004620: 2224 7b4f 5045 4e41 495f 4150 495f 4b45  "${OPENAI_API_KE
-00004630: 597d 2227 222c 0a20 2020 2022 5345 5250  Y}"'",.    "SERP
-00004640: 4150 495f 4150 495f 4b45 5922 3a20 2227  API_API_KEY": "'
-00004650: 2224 7b53 4552 5041 5049 5f41 5049 5f4b  "${SERPAPI_API_K
-00004660: 4559 7d22 2722 0a20 207d 0a7d 270a 6060  EY}"'".  }.}'.``
-00004670: 600a 0a60 6060 6a73 6f6e 0a7b 0a20 2022  `..```json.{.  "
-00004680: 7265 7375 6c74 223a 2022 4172 7272 2c20  result": "Arrr, 
-00004690: 7468 6572 6520 6265 2033 382c 3634 352c  there be 38,645,
-000046a0: 3637 3020 7065 6f70 6c65 206c 6976 696e  670 people livin
-000046b0: 2720 696e 2043 616e 6164 6120 6173 206f  ' in Canada as o
-000046c0: 6620 3230 3233 2122 2c0a 2020 2265 7272  f 2023!",.  "err
-000046d0: 6f72 223a 2022 222c 0a20 2022 7374 646f  or": "",.  "stdo
-000046e0: 7574 223a 2022 416e 7377 6572 2074 6865  ut": "Answer the
-000046f0: 2066 6f6c 6c6f 7769 6e67 2071 7565 7374   following quest
-00004700: 696f 6e73 2061 7320 6265 7374 2079 6f75  ions as best you
-00004710: 2063 616e 2c20 6275 7420 7370 6561 6b69   can, but speaki
-00004720: 6e67 2061 7320 6120 7069 7261 7465 206d  ng as a pirate m
-00004730: 6967 6874 2073 7065 616b 2e20 596f 7520  ight speak. You 
-00004740: 6861 7665 2061 6363 6573 7320 746f 2074  have access to t
-00004750: 6865 2066 6f6c 6c6f 7769 6e67 2074 6f6f  he following too
-00004760: 6c73 3a5c 6e5c 6e53 6561 7263 683a 2075  ls:\n\nSearch: u
-00004770: 7365 6675 6c20 666f 7220 7768 656e 2079  seful for when y
-00004780: 6f75 206e 6565 6420 746f 2061 6e73 7765  ou need to answe
-00004790: 7220 7175 6573 7469 6f6e 7320 6162 6f75  r questions abou
-000047a0: 7420 6375 7272 656e 7420 6576 656e 7473  t current events
-000047b0: 5c6e 5c6e 5573 6520 7468 6520 666f 6c6c  \n\nUse the foll
-000047c0: 6f77 696e 6720 666f 726d 6174 3a5c 6e5c  owing format:\n\
-000047d0: 6e51 7565 7374 696f 6e3a 2074 6865 2069  nQuestion: the i
-000047e0: 6e70 7574 2071 7565 7374 696f 6e20 796f  nput question yo
-000047f0: 7520 6d75 7374 2061 6e73 7765 725c 6e54  u must answer\nT
-00004800: 686f 7567 6874 3a20 796f 7520 7368 6f75  hought: you shou
-00004810: 6c64 2061 6c77 6179 7320 7468 696e 6b20  ld always think 
-00004820: 6162 6f75 7420 7768 6174 2074 6f20 646f  about what to do
-00004830: 5c6e 4163 7469 6f6e 3a20 7468 6520 6163  \nAction: the ac
-00004840: 7469 6f6e 2074 6f20 7461 6b65 2c20 7368  tion to take, sh
-00004850: 6f75 6c64 2062 6520 6f6e 6520 6f66 205b  ould be one of [
-00004860: 5365 6172 6368 5d5c 6e41 6374 696f 6e20  Search]\nAction 
-00004870: 496e 7075 743a 2074 6865 2069 6e70 7574  Input: the input
-00004880: 2074 6f20 7468 6520 6163 7469 6f6e 5c6e   to the action\n
-00004890: 4f62 7365 7276 6174 696f 6e3a 2074 6865  Observation: the
-000048a0: 2072 6573 756c 7420 6f66 2074 6865 2061   result of the a
-000048b0: 6374 696f 6e5c 6e2e 2e2e 2028 7468 6973  ction\n... (this
-000048c0: 2054 686f 7567 6874 2f41 6374 696f 6e2f   Thought/Action/
-000048d0: 4163 7469 6f6e 2049 6e70 7574 2f4f 6273  Action Input/Obs
-000048e0: 6572 7661 7469 6f6e 2063 616e 2072 6570  ervation can rep
-000048f0: 6561 7420 4e20 7469 6d65 7329 5c6e 5468  eat N times)\nTh
-00004900: 6f75 6768 743a 2049 206e 6f77 206b 6e6f  ought: I now kno
-00004910: 7720 7468 6520 6669 6e61 6c20 616e 7377  w the final answ
-00004920: 6572 5c6e 4669 6e61 6c20 416e 7377 6572  er\nFinal Answer
-00004930: 3a20 7468 6520 6669 6e61 6c20 616e 7377  : the final answ
-00004940: 6572 2074 6f20 7468 6520 6f72 6967 696e  er to the origin
-00004950: 616c 2069 6e70 7574 2071 7565 7374 696f  al input questio
-00004960: 6e5c 6e5c 6e42 6567 696e 2120 5265 6d65  n\n\nBegin! Reme
-00004970: 6d62 6572 2074 6f20 7370 6561 6b20 6173  mber to speak as
-00004980: 2061 2070 6972 6174 6520 7768 656e 2067   a pirate when g
-00004990: 6976 696e 6720 796f 7572 2066 696e 616c  iving your final
-000049a0: 2061 6e73 7765 722e 2055 7365 206c 6f74   answer. Use lot
-000049b0: 7320 6f66 205c 2241 7267 735c 225c 6e5c  s of \"Args\"\n\
-000049c0: 6e20 2020 2051 7565 7374 696f 6e3a 207b  n    Question: {
-000049d0: 696e 7075 747d 5c6e 2020 2020 7b61 6765  input}\n    {age
-000049e0: 6e74 5f73 6372 6174 6368 7061 647d 5c6e  nt_scratchpad}\n
-000049f0: 5c6e 5c6e 5c75 3030 3162 5b31 6d3e 2045  \n\n\u001b[1m> E
-00004a00: 6e74 6572 696e 6720 6e65 7720 4167 656e  ntering new Agen
-00004a10: 7445 7865 6375 746f 7220 6368 6169 6e2e  tExecutor chain.
-00004a20: 2e2e 5c75 3030 3162 5b30 6d5c 6e5c 7530  ..\u001b[0m\n\u0
-00004a30: 3031 625b 3332 3b31 6d5c 7530 3031 625b  01b[32;1m\u001b[
-00004a40: 313b 336d 5c6e 5468 6f75 6768 743a 2049  1;3m\nThought: I
-00004a50: 206e 6565 6420 746f 2066 696e 6420 6f75   need to find ou
-00004a60: 7420 686f 7720 6d61 6e79 2070 656f 706c  t how many peopl
-00004a70: 6520 6c69 7665 2069 6e20 4361 6e61 6461  e live in Canada
-00004a80: 5c6e 4163 7469 6f6e 3a20 5365 6172 6368  \nAction: Search
-00004a90: 5c6e 4163 7469 6f6e 2049 6e70 7574 3a20  \nAction Input: 
-00004aa0: 486f 7720 6d61 6e79 2070 656f 706c 6520  How many people 
-00004ab0: 6c69 7665 2069 6e20 4361 6e61 6461 2061  live in Canada a
-00004ac0: 7320 6f66 2032 3032 335c 7530 3031 625b  s of 2023\u001b[
-00004ad0: 306d 5c6e 4f62 7365 7276 6174 696f 6e3a  0m\nObservation:
-00004ae0: 205c 7530 3031 625b 3336 3b31 6d5c 7530   \u001b[36;1m\u0
-00004af0: 3031 625b 313b 336d 5468 6520 6375 7272  01b[1;3mThe curr
-00004b00: 656e 7420 706f 7075 6c61 7469 6f6e 206f  ent population o
-00004b10: 6620 4361 6e61 6461 2069 7320 3338 2c36  f Canada is 38,6
-00004b20: 3435 2c36 3730 2061 7320 6f66 2057 6564  45,670 as of Wed
-00004b30: 6e65 7364 6179 2c20 4d61 7263 6820 3239  nesday, March 29
-00004b40: 2c20 3230 3233 2c20 6261 7365 6420 6f6e  , 2023, based on
-00004b50: 2057 6f72 6c64 6f6d 6574 6572 2065 6c61   Worldometer ela
-00004b60: 626f 7261 7469 6f6e 206f 6620 7468 6520  boration of the 
-00004b70: 6c61 7465 7374 2055 6e69 7465 6420 4e61  latest United Na
-00004b80: 7469 6f6e 7320 6461 7461 2e5c 7530 3031  tions data.\u001
-00004b90: 625b 306d 5c6e 5468 6f75 6768 743a 5c75  b[0m\nThought:\u
-00004ba0: 3030 3162 5b33 323b 316d 5c75 3030 3162  001b[32;1m\u001b
-00004bb0: 5b31 3b33 6d20 4920 6e6f 7720 6b6e 6f77  [1;3m I now know
-00004bc0: 2074 6865 2066 696e 616c 2061 6e73 7765   the final answe
-00004bd0: 725c 6e46 696e 616c 2041 6e73 7765 723a  r\nFinal Answer:
-00004be0: 2041 7272 722c 2074 6865 7265 2062 6520   Arrr, there be 
-00004bf0: 3338 2c36 3435 2c36 3730 2070 656f 706c  38,645,670 peopl
-00004c00: 6520 6c69 7669 6e27 2069 6e20 4361 6e61  e livin' in Cana
-00004c10: 6461 2061 7320 6f66 2032 3032 3321 5c75  da as of 2023!\u
-00004c20: 3030 3162 5b30 6d5c 6e5c 6e5c 7530 3031  001b[0m\n\n\u001
-00004c30: 625b 316d 3e20 4669 6e69 7368 6564 2063  b[1m> Finished c
-00004c40: 6861 696e 2e5c 7530 3031 625b 306d 220a  hain.\u001b[0m".
-00004c50: 7d0a 6060 600a 0a23 2323 2323 2057 6861  }.```..##### Wha
-00004c60: 7420 6861 7070 656e 6564 3f0a 0a2d 2049  t happened?..- I
-00004c70: 6e20 6120 6d61 7474 6572 206f 6620 6665  n a matter of fe
-00004c80: 7720 7365 636f 6e64 732c 2077 6527 7665  w seconds, we've
-00004c90: 2064 6570 6c6f 7965 6420 6f75 7220 4150   deployed our AP
-00004ca0: 4920 6f6e 204a 696e 6120 4149 2043 6c6f  I on Jina AI Clo
-00004cb0: 7564 20f0 9f8e 890a 2d20 5468 6520 4150  ud .....- The AP
-00004cc0: 4920 6973 2073 6572 7665 726c 6573 7320  I is serverless 
-00004cd0: 616e 6420 7363 616c 6162 6c65 2c20 736f  and scalable, so
-00004ce0: 2077 6520 6361 6e20 7363 616c 6520 7570   we can scale up
-00004cf0: 2074 6865 2041 5049 2074 6f20 6861 6e64   the API to hand
-00004d00: 6c65 206d 6f72 6520 7265 7175 6573 7473  le more requests
-00004d10: 2e20 0a2d 2059 6f75 206d 6967 6874 206f  . .- You might o
-00004d20: 6273 6572 7665 2061 2064 656c 6179 2069  bserve a delay i
-00004d30: 6e20 7468 6520 6669 7273 7420 7265 7175  n the first requ
-00004d40: 6573 742c 2074 6861 7427 7320 6475 6520  est, that's due 
-00004d50: 746f 2074 6865 2077 6172 6d2d 7570 2074  to the warm-up t
-00004d60: 696d 6520 6f66 2074 6865 2041 5049 2e20  ime of the API. 
-00004d70: 5375 6273 6571 7565 6e74 2072 6571 7565  Subsequent reque
-00004d80: 7374 7320 7769 6c6c 2062 6520 6661 7374  sts will be fast
-00004d90: 6572 2e0a 2d20 5468 6520 4150 4920 696e  er..- The API in
-00004da0: 636c 7564 6573 2061 2053 7761 6767 6572  cludes a Swagger
-00004db0: 2055 4920 616e 6420 7468 6520 4f70 656e   UI and the Open
-00004dc0: 4150 4920 7370 6563 6966 6963 6174 696f  API specificatio
-00004dd0: 6e2c 2073 6f20 6974 2063 616e 2062 6520  n, so it can be 
-00004de0: 6561 7369 6c79 2069 6e74 6567 7261 7465  easily integrate
-00004df0: 6420 7769 7468 206f 7468 6572 2073 6572  d with other ser
-00004e00: 7669 6365 732e 200a 2d20 4e6f 772c 206f  vices. .- Now, o
-00004e10: 7468 6572 2061 6765 6e74 7320 6361 6e20  ther agents can 
-00004e20: 696e 7465 6772 6174 6520 7769 7468 2079  integrate with y
-00004e30: 6f75 7220 6167 656e 7473 206f 6e20 4a69  our agents on Ji
-00004e40: 6e61 2041 4920 436c 6f75 6420 7468 616e  na AI Cloud than
-00004e50: 6b73 2074 6f20 7468 6520 5b4f 7065 6e41  ks to the [OpenA
-00004e60: 5049 2041 6765 6e74 5d28 6874 7470 733a  PI Agent](https:
-00004e70: 2f2f 7079 7468 6f6e 2e6c 616e 6763 6861  //python.langcha
-00004e80: 696e 2e63 6f6d 2f65 6e2f 6c61 7465 7374  in.com/en/latest
-00004e90: 2f6d 6f64 756c 6573 2f61 6765 6e74 732f  /modules/agents/
-00004ea0: 746f 6f6c 6b69 7473 2f65 7861 6d70 6c65  toolkits/example
-00004eb0: 732f 6f70 656e 6170 692e 6874 6d6c 2920  s/openapi.html) 
-00004ec0: f09f 92a1 0a0a 0a0a 2d2d 2d0a 0a23 2323  ........---..###
-00004ed0: 2320 5265 6163 6820 6f75 7420 746f 2075  # Reach out to u
-00004ee0: 7320 f09f 939e 0a0a 2d20 5365 7276 6572  s ......- Server
-00004ef0: 6c65 7373 2069 7320 6e6f 7420 796f 7572  less is not your
-00004f00: 2074 6869 6e67 3f0a 2d20 446f 2079 6f75   thing?.- Do you
-00004f10: 2077 616e 7420 6c61 7267 6572 2069 6e73   want larger ins
-00004f20: 7461 6e63 6573 2066 6f72 2079 6f75 7220  tances for your 
-00004f30: 4150 493f 0a2d 204c 6f6f 6b69 6e67 2066  API?.- Looking f
-00004f40: 6f72 2066 696c 6520 7570 6c6f 6164 732c  or file uploads,
-00004f50: 206f 7220 6f74 6865 7220 6461 7461 2d69   or other data-i
-00004f60: 6e2c 2064 6174 612d 6f75 7420 6665 6174  n, data-out feat
-00004f70: 7572 6573 3f0a 2d20 446f 2079 6f75 2077  ures?.- Do you w
-00004f80: 616e 7420 746f 2073 6574 7570 2063 7573  ant to setup cus
-00004f90: 746f 6d20 6175 7468 6f72 697a 6174 696f  tom authorizatio
-00004fa0: 6e20 666f 7220 796f 7572 2041 5049 3f0a  n for your API?.
-00004fb0: 0a0a f09f 93a3 2047 6f74 2079 6f75 7220  ...... Got your 
-00004fc0: 6174 7465 6e74 696f 6e3f 205b 4a6f 696e  attention? [Join
-00004fd0: 2075 7320 6f6e 2053 6c61 636b 5d28 6874   us on Slack](ht
-00004fe0: 7470 733a 2f2f 6a69 6e61 2e61 692f 736c  tps://jina.ai/sl
-00004ff0: 6163 6b2f 2920 616e 6420 7765 2764 2062  ack/) and we'd b
-00005000: 6520 6861 7070 7920 746f 2068 656c 7020  e happy to help 
-00005010: 796f 7520 6f75 742e 0a0a 2d2d 2d0a 0a0a  you out...---...
-00005020: 2323 2320 606c 632d 7365 7276 6560 0a0a  ### `lc-serve`..
-00005030: 606c 632d 7365 7276 6560 2069 7320 6120  `lc-serve` is a 
-00005040: 434c 4920 746f 6f6c 2074 6861 7420 6865  CLI tool that he
-00005050: 6c70 7320 796f 7520 746f 2064 6570 6c6f  lps you to deplo
-00005060: 7920 796f 7572 2061 6765 6e74 7320 6f6e  y your agents on
-00005070: 204a 696e 6120 4149 2043 6c6f 7564 2e0a   Jina AI Cloud..
-00005080: 0a0a 7c20 4465 7363 7269 7074 696f 6e20  ..| Description 
-00005090: 7c20 436f 6d6d 616e 6420 7c20 0a7c 202d  | Command | .| -
-000050a0: 2d2d 207c 202d 2d2d 3a20 7c0a 7c20 4465  -- | ---: |.| De
-000050b0: 706c 6f79 2079 6f75 7220 6170 7020 6c6f  ploy your app lo
-000050c0: 6361 6c6c 7920 7c20 606c 632d 7365 7276  cally | `lc-serv
-000050d0: 6520 6465 706c 6f79 206c 6f63 616c 2061  e deploy local a
-000050e0: 7070 6020 7c0a 7c20 4465 706c 6f79 2079  pp` |.| Deploy y
-000050f0: 6f75 7220 6170 7020 6f6e 204a 696e 6120  our app on Jina 
-00005100: 4149 2043 6c6f 7564 207c 2060 6c63 2d73  AI Cloud | `lc-s
-00005110: 6572 7665 2064 6570 6c6f 7920 6a63 6c6f  erve deploy jclo
-00005120: 7564 2061 7070 6020 7c0a 7c20 5570 6461  ud app` |.| Upda
-00005130: 7465 2065 7869 7374 696e 6720 6170 7020  te existing app 
-00005140: 6f6e 204a 696e 6120 4149 2043 6c6f 7564  on Jina AI Cloud
-00005150: 207c 2060 6c63 2d73 6572 7665 2064 6570   | `lc-serve dep
-00005160: 6c6f 7920 6a63 6c6f 7564 2061 7070 202d  loy jcloud app -
-00005170: 2d61 7070 2d69 6420 3c61 7070 2d69 643e  -app-id <app-id>
-00005180: 6020 7c0a 7c20 4765 7420 6170 7020 7374  ` |.| Get app st
-00005190: 6174 7573 206f 6e20 4a69 6e61 2041 4920  atus on Jina AI 
-000051a0: 436c 6f75 6420 7c20 606c 632d 7365 7276  Cloud | `lc-serv
-000051b0: 6520 7374 6174 7573 203c 6170 702d 6964  e status <app-id
-000051c0: 3e60 207c 0a7c 204c 6973 7420 616c 6c20  >` |.| List all 
-000051d0: 6170 7073 206f 6e20 4a69 6e61 2041 4920  apps on Jina AI 
-000051e0: 436c 6f75 6420 7c20 606c 632d 7365 7276  Cloud | `lc-serv
-000051f0: 6520 6c69 7374 6020 7c0a 7c20 5265 6d6f  e list` |.| Remo
-00005200: 7665 2061 7070 206f 6e20 4a69 6e61 2041  ve app on Jina A
-00005210: 4920 436c 6f75 6420 7c20 606c 632d 7365  I Cloud | `lc-se
-00005220: 7276 6520 7265 6d6f 7665 203c 6170 702d  rve remove <app-
-00005230: 6964 3e60 207c 0a0a 0a2d 2d2d 0a0a 2323  id>` |...---..##
-00005240: 2320 4167 656e 7473 2050 6c61 7967 726f  # Agents Playgro
-00005250: 756e 6420 f09f 95b9 efb8 8ff0 9f8e aef0  und ............
-00005260: 9f8c 900a 0a5b 4c61 6e67 4368 6169 6e20  .....[LangChain 
-00005270: 6167 656e 7473 5d28 6874 7470 733a 2f2f  agents](https://
-00005280: 7079 7468 6f6e 2e6c 616e 6763 6861 696e  python.langchain
-00005290: 2e63 6f6d 2f65 6e2f 6c61 7465 7374 2f6d  .com/en/latest/m
-000052a0: 6f64 756c 6573 2f61 6765 6e74 732f 6765  odules/agents/ge
-000052b0: 7474 696e 675f 7374 6172 7465 642e 6874  tting_started.ht
-000052c0: 6d6c 2920 7573 6520 4c4c 4d73 2074 6f20  ml) use LLMs to 
-000052d0: 6465 7465 726d 696e 6520 7468 6520 6163  determine the ac
-000052e0: 7469 6f6e 7320 746f 2062 6520 7461 6b65  tions to be take
-000052f0: 6e20 696e 2077 6861 7420 6f72 6465 722e  n in what order.
-00005300: 2041 6e20 6163 7469 6f6e 2063 616e 2065   An action can e
-00005310: 6974 6865 7220 6265 2075 7369 6e67 2061  ither be using a
-00005320: 2074 6f6f 6c20 616e 6420 6f62 7365 7276   tool and observ
-00005330: 696e 6720 6974 7320 6f75 7470 7574 2c20  ing its output, 
-00005340: 6f72 2072 6574 7572 6e69 6e67 2074 6f20  or returning to 
-00005350: 7468 6520 7573 6572 2e20 5765 2776 6520  the user. We've 
-00005360: 686f 7374 6564 2061 202a 2a5b 5374 7265  hosted a **[Stre
-00005370: 616d 6c69 7420 506c 6179 6772 6f75 6e64  amlit Playground
-00005380: 5d28 6874 7470 733a 2f2f 6c61 6e67 6368  ](https://langch
-00005390: 6169 6e2e 776f 6c66 2e6a 696e 612e 6169  ain.wolf.jina.ai
-000053a0: 2f70 6c61 7967 726f 756e 642f 292a 2a20  /playground/)** 
-000053b0: 6f6e 204a 696e 6120 4149 2043 6c6f 7564  on Jina AI Cloud
-000053c0: 2074 6f20 696e 7465 7261 6374 2077 6974   to interact wit
-000053d0: 6820 7468 6520 6167 656e 7473 2c20 7768  h the agents, wh
-000053e0: 6963 6820 6163 6365 7074 7320 7769 7468  ich accepts with
-000053f0: 2066 6f6c 6c6f 7769 6e67 2069 6e70 7574   following input
-00005400: 733a 0a0a 2d20 2a2a 5b41 6765 6e74 2054  s:..- **[Agent T
-00005410: 7970 6573 5d28 6874 7470 733a 2f2f 7079  ypes](https://py
-00005420: 7468 6f6e 2e6c 616e 6763 6861 696e 2e63  thon.langchain.c
-00005430: 6f6d 2f65 6e2f 6c61 7465 7374 2f6d 6f64  om/en/latest/mod
-00005440: 756c 6573 2f61 6765 6e74 732f 6167 656e  ules/agents/agen
-00005450: 7473 2e68 746d 6c29 3a2a 2a20 4368 6f6f  ts.html):** Choo
-00005460: 7365 2066 726f 6d20 6469 6666 6572 656e  se from differen
-00005470: 7420 6167 656e 7420 7479 7065 7320 7468  t agent types th
-00005480: 6174 204c 616e 6763 6861 696e 2073 7570  at Langchain sup
-00005490: 706f 7274 732e 200a 0a2d 202a 2a5b 546f  ports. ..- **[To
-000054a0: 6f6c 735d 2868 7474 7073 3a2f 2f70 7974  ols](https://pyt
-000054b0: 686f 6e2e 6c61 6e67 6368 6169 6e2e 636f  hon.langchain.co
-000054c0: 6d2f 656e 2f6c 6174 6573 742f 6d6f 6475  m/en/latest/modu
-000054d0: 6c65 732f 6167 656e 7473 2f74 6f6f 6c73  les/agents/tools
-000054e0: 2e68 746d 6c29 3a2a 2a20 4368 6f6f 7365  .html):** Choose
-000054f0: 2066 726f 6d20 6469 6666 6572 656e 7420   from different 
-00005500: 746f 6f6c 7320 7468 6174 204c 616e 6763  tools that Langc
-00005510: 6861 696e 2073 7570 706f 7274 732e 2053  hain supports. S
-00005520: 6f6d 6520 746f 6f6c 7320 6d61 7920 7265  ome tools may re
-00005530: 7175 6972 6520 616e 2041 5049 2074 6f6b  quire an API tok
-00005540: 656e 206f 7220 6f74 6865 7220 7265 6c61  en or other rela
-00005550: 7465 6420 6172 6775 6d65 6e74 732e 0a0a  ted arguments...
-00005560: 546f 2075 7365 2074 6865 2070 6c61 7967  To use the playg
-00005570: 726f 756e 642c 2073 696d 706c 7920 7479  round, simply ty
-00005580: 7065 2079 6f75 7220 696e 7075 7420 696e  pe your input in
-00005590: 2074 6865 2074 6578 7420 626f 7820 7072   the text box pr
-000055a0: 6f76 6964 6564 2074 6f20 6765 7420 7468  ovided to get th
-000055b0: 6520 6167 656e 7427 7320 6f75 7470 7574  e agent's output
-000055c0: 2061 6e64 2063 6861 696e 206f 6620 7468   and chain of th
-000055d0: 6f75 6768 742e 2045 6e6a 6f79 2065 7870  ought. Enjoy exp
-000055e0: 6c6f 7269 6e67 204c 616e 6763 6861 696e  loring Langchain
-000055f0: 2773 2063 6170 6162 696c 6974 6965 7321  's capabilities!
-00005600: 2049 6e20 6164 6469 7469 6f6e 2074 6f20   In addition to 
-00005610: 7374 7265 616d 6c69 742c 2079 6f75 2063  streamlit, you c
-00005620: 616e 2061 6c73 6f20 7573 6520 6f75 7220  an also use our 
-00005630: 5245 5354 6675 6c20 4150 4973 206f 6e20  RESTful APIs on 
-00005640: 7468 6520 706c 6179 6772 6f75 6e64 2074  the playground t
-00005650: 6f20 696e 7465 7261 6374 2077 6974 6820  o interact with 
-00005660: 7468 6520 6167 656e 7473 2e20 0a0a 0a23  the agents. ...#
-00005670: 2323 205b 5a65 726f 2d73 686f 7420 5265  ## [Zero-shot Re
-00005680: 6163 7420 4465 7363 7269 7074 696f 6e20  act Description 
-00005690: 6167 656e 7420 7769 7468 2053 6572 7041  agent with SerpA
-000056a0: 5049 2061 6e64 2043 616c 6375 6c61 746f  PI and Calculato
-000056b0: 725d 2868 7474 7073 3a2f 2f70 7974 686f  r](https://pytho
-000056c0: 6e2e 6c61 6e67 6368 6169 6e2e 636f 6d2f  n.langchain.com/
-000056d0: 656e 2f6c 6174 6573 742f 6d6f 6475 6c65  en/latest/module
-000056e0: 732f 6167 656e 7473 2f67 6574 7469 6e67  s/agents/getting
-000056f0: 5f73 7461 7274 6564 2e68 746d 6c29 0a0a  _started.html)..
-00005700: 2323 2323 2053 7472 6561 6d6c 6974 2050  #### Streamlit P
-00005710: 6c61 7967 726f 756e 640a 0a21 5b53 7472  layground..![Str
-00005720: 6561 6d6c 6974 2050 6c61 7967 726f 756e  eamlit Playgroun
-00005730: 645d 282e 6769 7468 7562 2f69 6d61 6765  d](.github/image
-00005740: 732f 706c 6179 6772 6f75 6e64 5f6f 6e65  s/playground_one
-00005750: 2e67 6966 290a 0a23 2323 2320 5245 5354  .gif)..#### REST
-00005760: 6675 6c20 4150 490a 0a60 6060 6261 7368  ful API..```bash
-00005770: 0a65 7870 6f72 7420 4f50 454e 4149 5f41  .export OPENAI_A
-00005780: 5049 5f4b 4559 3d73 6b2d 2a2a 2a0a 6578  PI_KEY=sk-***.ex
-00005790: 706f 7274 2053 4552 5041 5049 5f41 5049  port SERPAPI_API
-000057a0: 5f4b 4559 3d2a 2a2a 0a0a 6375 726c 202d  _KEY=***..curl -
-000057b0: 7358 2050 4f53 5420 2768 7474 7073 3a2f  sX POST 'https:/
-000057c0: 2f6c 616e 6763 6861 696e 2e77 6f6c 662e  /langchain.wolf.
-000057d0: 6a69 6e61 2e61 692f 6170 692f 7275 6e27  jina.ai/api/run'
-000057e0: 205c 0a20 202d 4820 2761 6363 6570 743a   \.  -H 'accept:
-000057f0: 2061 7070 6c69 6361 7469 6f6e 2f6a 736f   application/jso
-00005800: 6e27 205c 0a20 202d 4820 2743 6f6e 7465  n' \.  -H 'Conte
-00005810: 6e74 2d54 7970 653a 2061 7070 6c69 6361  nt-Type: applica
-00005820: 7469 6f6e 2f6a 736f 6e27 205c 0a20 202d  tion/json' \.  -
-00005830: 2d64 6174 612d 7261 7720 277b 0a20 2020  -data-raw '{.   
-00005840: 2022 7465 7874 223a 2022 5768 6f20 6973   "text": "Who is
-00005850: 204c 656f 2044 6943 6170 7269 6f73 2067   Leo DiCaprios g
-00005860: 6972 6c66 7269 656e 643f 2057 6861 7420  irlfriend? What 
-00005870: 6973 2068 6572 2063 7572 7265 6e74 2061  is her current a
-00005880: 6765 2072 6169 7365 6420 746f 2074 6865  ge raised to the
-00005890: 2030 2e34 3320 706f 7765 723f 222c 0a20   0.43 power?",. 
-000058a0: 2020 2022 7061 7261 6d65 7465 7273 223a     "parameters":
-000058b0: 207b 0a20 2020 2020 2020 2022 746f 6f6c   {.        "tool
-000058c0: 7322 3a20 7b0a 2020 2020 2020 2020 2020  s": {.          
-000058d0: 2020 2274 6f6f 6c5f 6e61 6d65 7322 3a20    "tool_names": 
-000058e0: 5b22 7365 7270 6170 6922 2c20 226c 6c6d  ["serpapi", "llm
-000058f0: 2d6d 6174 6822 5d0a 2020 2020 2020 2020  -math"].        
-00005900: 7d2c 0a20 2020 2020 2020 2022 6167 656e  },.        "agen
-00005910: 7422 3a20 227a 6572 6f2d 7368 6f74 2d72  t": "zero-shot-r
-00005920: 6561 6374 2d64 6573 6372 6970 7469 6f6e  eact-description
-00005930: 222c 0a20 2020 2020 2020 2022 7665 7262  ",.        "verb
-00005940: 6f73 6522 3a20 7472 7565 0a20 2020 207d  ose": true.    }
-00005950: 2c0a 2020 2020 2265 6e76 7322 3a20 7b0a  ,.    "envs": {.
-00005960: 2020 2020 2020 2020 224f 5045 4e41 495f          "OPENAI_
-00005970: 4150 495f 4b45 5922 3a20 2227 2224 7b4f  API_KEY": "'"${O
-00005980: 5045 4e41 495f 4150 495f 4b45 597d 2227  PENAI_API_KEY}"'
-00005990: 222c 0a20 2020 2020 2020 2022 5345 5250  ",.        "SERP
-000059a0: 4150 495f 4150 495f 4b45 5922 3a20 2227  API_API_KEY": "'
-000059b0: 2224 7b53 4552 5041 5049 5f41 5049 5f4b  "${SERPAPI_API_K
-000059c0: 4559 7d22 2722 0a20 2020 207d 0a7d 2720  EY}"'".    }.}' 
-000059d0: 7c20 6a71 0a60 6060 200a 0a60 6060 6a73  | jq.``` ..```js
-000059e0: 6f6e 0a7b 0a20 2022 7265 7375 6c74 223a  on.{.  "result":
-000059f0: 2022 4361 6d69 6c61 204d 6f72 726f 6e65   "Camila Morrone
-00005a00: 2069 7320 4c65 6f20 4469 4361 7072 696f   is Leo DiCaprio
-00005a10: 2773 2067 6972 6c66 7269 656e 642c 2061  's girlfriend, a
-00005a20: 6e64 2068 6572 2063 7572 7265 6e74 2061  nd her current a
-00005a30: 6765 2072 6169 7365 6420 746f 2074 6865  ge raised to the
-00005a40: 2030 2e34 3320 706f 7765 7220 6973 2033   0.43 power is 3
-00005a50: 2e36 3236 3132 3630 3631 3135 3239 3532  .626126061152952
-00005a60: 372e 222c 0a20 2022 6368 6169 6e5f 6f66  7.",.  "chain_of
-00005a70: 5f74 686f 7567 6874 223a 2022 5c75 3030  _thought": "\u00
-00005a80: 3162 5b31 6d3e 2045 6e74 6572 696e 6720  1b[1m> Entering 
-00005a90: 6e65 7720 4167 656e 7445 7865 6375 746f  new AgentExecuto
-00005aa0: 7220 6368 6169 6e2e 2e2e 5c75 3030 3162  r chain...\u001b
-00005ab0: 5b30 6d5c 7530 3031 625b 3332 3b31 6d5c  [0m\u001b[32;1m\
-00005ac0: 7530 3031 625b 313b 336d 2049 206e 6565  u001b[1;3m I nee
-00005ad0: 6420 746f 2066 696e 6420 6f75 7420 7468  d to find out th
-00005ae0: 6520 6e61 6d65 206f 6620 4c65 6f27 7320  e name of Leo's 
-00005af0: 6769 726c 6672 6965 6e64 2061 6e64 2074  girlfriend and t
-00005b00: 6865 6e20 7573 6520 7468 6520 6361 6c63  hen use the calc
-00005b10: 756c 6174 6f72 2074 6f20 6361 6c63 756c  ulator to calcul
-00005b20: 6174 6520 6865 7220 6167 6520 746f 2074  ate her age to t
-00005b30: 6865 2030 2e34 3320 706f 7765 722e 4163  he 0.43 power.Ac
-00005b40: 7469 6f6e 3a20 5365 6172 6368 4163 7469  tion: SearchActi
-00005b50: 6f6e 2049 6e70 7574 3a20 4c65 6f20 4469  on Input: Leo Di
-00005b60: 4361 7072 696f 2067 6972 6c66 7269 656e  Caprio girlfrien
-00005b70: 645c 7530 3031 625b 306d 4f62 7365 7276  d\u001b[0mObserv
-00005b80: 6174 696f 6e3a 205c 7530 3031 625b 3336  ation: \u001b[36
-00005b90: 3b31 6d5c 7530 3031 625b 313b 336d 4469  ;1m\u001b[1;3mDi
-00005ba0: 4361 7072 696f 206d 6574 2061 6374 6f72  Caprio met actor
-00005bb0: 2043 616d 696c 6120 4d6f 7272 6f6e 6520   Camila Morrone 
-00005bc0: 696e 2044 6563 656d 6265 7220 3230 3137  in December 2017
-00005bd0: 2c20 7768 656e 2073 6865 2077 6173 2032  , when she was 2
-00005be0: 3020 616e 6420 6865 2077 6173 2034 332e  0 and he was 43.
-00005bf0: 2054 6865 7920 7765 7265 2073 706f 7474   They were spott
-00005c00: 6564 2061 7420 436f 6163 6865 6c6c 6120  ed at Coachella 
-00005c10: 616e 6420 7765 6e74 206f 6e20 6d75 6c74  and went on mult
-00005c20: 6970 6c65 2076 6163 6174 696f 6e73 2074  iple vacations t
-00005c30: 6f67 6574 6865 722e 2053 6f6d 6520 7265  ogether. Some re
-00005c40: 706f 7274 7320 7375 6767 6573 7465 6420  ports suggested 
-00005c50: 7468 6174 2044 6943 6170 7269 6f20 7761  that DiCaprio wa
-00005c60: 7320 7265 6164 7920 746f 2061 736b 204d  s ready to ask M
-00005c70: 6f72 726f 6e65 2074 6f20 6d61 7272 7920  orrone to marry 
-00005c80: 6869 6d2e 2054 6865 2063 6f75 706c 6520  him. The couple 
-00005c90: 6d61 6465 2074 6865 6972 2072 6564 2063  made their red c
-00005ca0: 6172 7065 7420 6465 6275 7420 6174 2074  arpet debut at t
-00005cb0: 6865 2032 3032 3020 4163 6164 656d 7920  he 2020 Academy 
-00005cc0: 4177 6172 6473 2e5c 7530 3031 625b 306d  Awards.\u001b[0m
-00005cd0: 5468 6f75 6768 743a 5c75 3030 3162 5b33  Thought:\u001b[3
-00005ce0: 323b 316d 5c75 3030 3162 5b31 3b33 6d20  2;1m\u001b[1;3m 
-00005cf0: 4920 6e65 6564 2074 6f20 7573 6520 7468  I need to use th
-00005d00: 6520 6361 6c63 756c 6174 6f72 2074 6f20  e calculator to 
-00005d10: 6361 6c63 756c 6174 6520 6865 7220 6167  calculate her ag
-00005d20: 6520 746f 2074 6865 2030 2e34 3320 706f  e to the 0.43 po
-00005d30: 7765 7241 6374 696f 6e3a 2043 616c 6375  werAction: Calcu
-00005d40: 6c61 746f 7241 6374 696f 6e20 496e 7075  latorAction Inpu
-00005d50: 743a 2032 305e 302e 3433 5c75 3030 3162  t: 20^0.43\u001b
-00005d60: 5b30 6d4f 6273 6572 7661 7469 6f6e 3a20  [0mObservation: 
-00005d70: 5c75 3030 3162 5b33 333b 316d 5c75 3030  \u001b[33;1m\u00
-00005d80: 3162 5b31 3b33 6d41 6e73 7765 723a 2033  1b[1;3mAnswer: 3
-00005d90: 2e36 3236 3132 3630 3631 3135 3239 3532  .626126061152952
-00005da0: 375c 7530 3031 625b 306d 5468 6f75 6768  7\u001b[0mThough
-00005db0: 743a 5c75 3030 3162 5b33 323b 316d 5c75  t:\u001b[32;1m\u
-00005dc0: 3030 3162 5b31 3b33 6d20 4920 6e6f 7720  001b[1;3m I now 
-00005dd0: 6b6e 6f77 2074 6865 2066 696e 616c 2061  know the final a
-00005de0: 6e73 7765 7246 696e 616c 2041 6e73 7765  nswerFinal Answe
-00005df0: 723a 2043 616d 696c 6120 4d6f 7272 6f6e  r: Camila Morron
-00005e00: 6520 6973 204c 656f 2044 6943 6170 7269  e is Leo DiCapri
-00005e10: 6f27 7320 6769 726c 6672 6965 6e64 2c20  o's girlfriend, 
-00005e20: 616e 6420 6865 7220 6375 7272 656e 7420  and her current 
-00005e30: 6167 6520 7261 6973 6564 2074 6f20 7468  age raised to th
-00005e40: 6520 302e 3433 2070 6f77 6572 2069 7320  e 0.43 power is 
-00005e50: 332e 3632 3631 3236 3036 3131 3532 3935  3.62612606115295
-00005e60: 3237 2e5c 7530 3031 625b 306d 5c75 3030  27.\u001b[0m\u00
-00005e70: 3162 5b31 6d3e 2046 696e 6973 6865 6420  1b[1m> Finished 
-00005e80: 6368 6169 6e2e 5c75 3030 3162 5b30 6d22  chain.\u001b[0m"
-00005e90: 0a7d 0a60 6060 0a0a 2323 2320 5b53 656c  .}.```..### [Sel
-00005ea0: 6620 4173 6b20 5769 7468 2053 6561 7263  f Ask With Searc
-00005eb0: 685d 2868 7474 7073 3a2f 2f70 7974 686f  h](https://pytho
-00005ec0: 6e2e 6c61 6e67 6368 6169 6e2e 636f 6d2f  n.langchain.com/
-00005ed0: 656e 2f6c 6174 6573 742f 6d6f 6475 6c65  en/latest/module
-00005ee0: 732f 6167 656e 7473 2f69 6d70 6c65 6d65  s/agents/impleme
-00005ef0: 6e74 6174 696f 6e73 2f73 656c 665f 6173  ntations/self_as
-00005f00: 6b5f 7769 7468 5f73 6561 7263 682e 6874  k_with_search.ht
-00005f10: 6d6c 290a 0a23 2323 2320 5374 7265 616d  ml)..#### Stream
-00005f20: 6c69 7420 506c 6179 6772 6f75 6e64 0a0a  lit Playground..
-00005f30: 215b 5374 7265 616d 6c69 7420 506c 6179  ![Streamlit Play
-00005f40: 6772 6f75 6e64 5d28 2e67 6974 6875 622f  ground](.github/
-00005f50: 696d 6167 6573 2f70 6c61 7967 726f 756e  images/playgroun
-00005f60: 645f 7477 6f2e 6769 6629 0a0a 2323 2323  d_two.gif)..####
-00005f70: 2052 4553 5466 756c 2041 5049 0a0a 6060   RESTful API..``
-00005f80: 6062 6173 680a 6578 706f 7274 204f 5045  `bash.export OPE
-00005f90: 4e41 495f 4150 495f 4b45 593d 736b 2d2a  NAI_API_KEY=sk-*
-00005fa0: 2a2a 0a65 7870 6f72 7420 5345 5250 4150  **.export SERPAP
-00005fb0: 495f 4150 495f 4b45 593d 2a2a 2a0a 0a63  I_API_KEY=***..c
-00005fc0: 7572 6c20 2d73 5820 504f 5354 2027 6874  url -sX POST 'ht
-00005fd0: 7470 733a 2f2f 6c61 6e67 6368 6169 6e2e  tps://langchain.
-00005fe0: 776f 6c66 2e6a 696e 612e 6169 2f61 7069  wolf.jina.ai/api
-00005ff0: 2f72 756e 2720 5c0a 2020 2d48 2027 6163  /run' \.  -H 'ac
-00006000: 6365 7074 3a20 6170 706c 6963 6174 696f  cept: applicatio
-00006010: 6e2f 6a73 6f6e 2720 5c0a 2020 2d48 2027  n/json' \.  -H '
-00006020: 436f 6e74 656e 742d 5479 7065 3a20 6170  Content-Type: ap
-00006030: 706c 6963 6174 696f 6e2f 6a73 6f6e 2720  plication/json' 
-00006040: 5c0a 2020 2d2d 6461 7461 2d72 6177 2027  \.  --data-raw '
-00006050: 7b0a 2020 2020 2274 6578 7422 3a20 2257  {.    "text": "W
-00006060: 6861 7420 6973 2074 6865 2068 6f6d 6574  hat is the homet
-00006070: 6f77 6e20 6f66 2074 6865 2072 6569 676e  own of the reign
-00006080: 696e 6720 6d65 6e73 2055 2e53 2e20 4f70  ing mens U.S. Op
-00006090: 656e 2063 6861 6d70 696f 6e3f 222c 0a20  en champion?",. 
-000060a0: 2020 2022 7061 7261 6d65 7465 7273 223a     "parameters":
-000060b0: 207b 0a20 2020 2020 2020 2022 746f 6f6c   {.        "tool
-000060c0: 7322 3a20 7b0a 2020 2020 2020 2020 2020  s": {.          
-000060d0: 2020 2274 6f6f 6c5f 6e61 6d65 7322 3a20    "tool_names": 
-000060e0: 5b22 7365 7270 6170 6922 5d0a 2020 2020  ["serpapi"].    
-000060f0: 2020 2020 7d2c 0a20 2020 2020 2020 2022      },.        "
-00006100: 6167 656e 7422 3a20 2273 656c 662d 6173  agent": "self-as
-00006110: 6b2d 7769 7468 2d73 6561 7263 6822 2c0a  k-with-search",.
-00006120: 2020 2020 2020 2020 2276 6572 626f 7365          "verbose
-00006130: 223a 2074 7275 650a 2020 2020 7d2c 0a20  ": true.    },. 
-00006140: 2020 2022 656e 7673 223a 207b 0a20 2020     "envs": {.   
-00006150: 2020 2020 2022 4f50 454e 4149 5f41 5049       "OPENAI_API
-00006160: 5f4b 4559 223a 2022 2722 247b 4f50 454e  _KEY": "'"${OPEN
-00006170: 4149 5f41 5049 5f4b 4559 7d22 2722 2c0a  AI_API_KEY}"'",.
-00006180: 2020 2020 2020 2020 2253 4552 5041 5049          "SERPAPI
-00006190: 5f41 5049 5f4b 4559 223a 2022 2722 247b  _API_KEY": "'"${
-000061a0: 5345 5250 4150 495f 4150 495f 4b45 597d  SERPAPI_API_KEY}
-000061b0: 2227 220a 2020 2020 7d0a 7d27 207c 206a  "'".    }.}' | j
-000061c0: 710a 6060 600a 0a60 6060 6a73 6f6e 0a7b  q.```..```json.{
-000061d0: 0a20 2022 7265 7375 6c74 223a 2022 456c  .  "result": "El
-000061e0: 2050 616c 6d61 722c 204d 7572 6369 612c   Palmar, Murcia,
-000061f0: 2053 7061 696e 222c 0a20 2022 6368 6169   Spain",.  "chai
-00006200: 6e5f 6f66 5f74 686f 7567 6874 223a 2022  n_of_thought": "
-00006210: 5c75 3030 3162 5b31 6d3e 2045 6e74 6572  \u001b[1m> Enter
-00006220: 696e 6720 6e65 7720 4167 656e 7445 7865  ing new AgentExe
-00006230: 6375 746f 7220 6368 6169 6e2e 2e2e 5c75  cutor chain...\u
-00006240: 3030 3162 5b30 6d5c 7530 3031 625b 3332  001b[0m\u001b[32
-00006250: 3b31 6d5c 7530 3031 625b 313b 336d 2059  ;1m\u001b[1;3m Y
-00006260: 6573 2e46 6f6c 6c6f 7720 7570 3a20 5768  es.Follow up: Wh
-00006270: 6f20 6973 2074 6865 2072 6569 676e 696e  o is the reignin
-00006280: 6720 6d65 6e73 2055 2e53 2e20 4f70 656e  g mens U.S. Open
-00006290: 2063 6861 6d70 696f 6e3f 5c75 3030 3162   champion?\u001b
-000062a0: 5b30 6d49 6e74 6572 6d65 6469 6174 6520  [0mIntermediate 
-000062b0: 616e 7377 6572 3a20 5c75 3030 3162 5b33  answer: \u001b[3
-000062c0: 363b 316d 5c75 3030 3162 5b31 3b33 6d43  6;1m\u001b[1;3mC
-000062d0: 6172 6c6f 7320 416c 6361 7261 7a20 4761  arlos Alcaraz Ga
-000062e0: 7266 6961 5c75 3030 3162 5b30 6d5c 7530  rfia\u001b[0m\u0
-000062f0: 3031 625b 3332 3b31 6d5c 7530 3031 625b  01b[32;1m\u001b[
-00006300: 313b 336d 466f 6c6c 6f77 2075 703a 2057  1;3mFollow up: W
-00006310: 6861 7420 6973 2043 6172 6c6f 7320 416c  hat is Carlos Al
-00006320: 6361 7261 7a20 4761 7266 6961 2773 2068  caraz Garfia's h
-00006330: 6f6d 6574 6f77 6e3f 5c75 3030 3162 5b30  ometown?\u001b[0
-00006340: 6d49 6e74 6572 6d65 6469 6174 6520 616e  mIntermediate an
-00006350: 7377 6572 3a20 5c75 3030 3162 5b33 363b  swer: \u001b[36;
-00006360: 316d 5c75 3030 3162 5b31 3b33 6d43 6172  1m\u001b[1;3mCar
-00006370: 6c6f 7320 416c 6361 7261 7a20 4761 7266  los Alcaraz Garf
-00006380: 6961 2077 6173 2062 6f72 6e20 6f6e 204d  ia was born on M
-00006390: 6179 2035 2c20 3230 3033 2c20 696e 2045  ay 5, 2003, in E
-000063a0: 6c20 5061 6c6d 6172 2c20 4d75 7263 6961  l Palmar, Murcia
-000063b0: 2c20 5370 6169 6e20 746f 2070 6172 656e  , Spain to paren
-000063c0: 7473 2043 6172 6c6f 7320 416c 6361 7261  ts Carlos Alcara
-000063d0: 7a20 476f 6e7a c3a1 6c65 7a20 616e 6420  z Gonz..lez and 
-000063e0: 5669 7267 696e 6961 2047 6172 6669 6120  Virginia Garfia 
-000063f0: 4573 6361 6e64 c3b3 6e2e 2048 6520 6861  Escand..n. He ha
-00006400: 7320 7468 7265 6520 7369 626c 696e 6773  s three siblings
-00006410: 2e5c 7530 3031 625b 306d 5c75 3030 3162  .\u001b[0m\u001b
-00006420: 5b33 323b 316d 5c75 3030 3162 5b31 3b33  [32;1m\u001b[1;3
-00006430: 6d53 6f20 7468 6520 6669 6e61 6c20 616e  mSo the final an
-00006440: 7377 6572 2069 733a 2045 6c20 5061 6c6d  swer is: El Palm
-00006450: 6172 2c20 4d75 7263 6961 2c20 5370 6169  ar, Murcia, Spai
-00006460: 6e5c 7530 3031 625b 306d 5c75 3030 3162  n\u001b[0m\u001b
-00006470: 5b31 6d3e 2046 696e 6973 6865 6420 6368  [1m> Finished ch
-00006480: 6169 6e2e 5c75 3030 3162 5b30 6d22 0a7d  ain.\u001b[0m".}
-00006490: 0a60 6060 0a0a 2d2d 2d0a 0a23 2320 4368  .```..---..## Ch
-000064a0: 6169 6e73 206f 6e20 4a69 6e61 20f0 9f93  ains on Jina ...
-000064b0: a6f0 9f9a 800a 0a5b 4368 6169 6e73 5d28  .......[Chains](
-000064c0: 6874 7470 733a 2f2f 7079 7468 6f6e 2e6c  https://python.l
-000064d0: 616e 6763 6861 696e 2e63 6f6d 2f65 6e2f  angchain.com/en/
-000064e0: 6c61 7465 7374 2f6d 6f64 756c 6573 2f63  latest/modules/c
-000064f0: 6861 696e 732f 6765 7474 696e 675f 7374  hains/getting_st
-00006500: 6172 7465 642e 6874 6d6c 2920 696e 204c  arted.html) in L
-00006510: 616e 6743 6861 696e 2061 6c6c 6f77 2075  angChain allow u
-00006520: 7365 7273 2074 6f20 636f 6d62 696e 6520  sers to combine 
-00006530: 636f 6d70 6f6e 656e 7473 2074 6f20 6372  components to cr
-00006540: 6561 7465 2061 2073 696e 676c 652c 2063  eate a single, c
-00006550: 6f68 6572 656e 7420 6170 706c 6963 6174  oherent applicat
-00006560: 696f 6e2e 2057 6974 6820 4a69 6e61 2c20  ion. With Jina, 
-00006570: 0a0a 2d20 596f 7520 6361 6e20 6578 706f  ..- You can expo
-00006580: 7365 2079 6f75 7220 6043 6861 696e 6020  se your `Chain` 
-00006590: 6173 2052 4553 5466 756c 2f67 5250 432f  as RESTful/gRPC/
-000065a0: 5765 6253 6f63 6b65 7420 4150 492e 0a2d  WebSocket API..-
-000065b0: 2045 6e61 626c 6520 6043 6861 696e 6073   Enable `Chain`s
-000065c0: 2074 6f20 6465 706c 6f79 2026 2073 6361   to deploy & sca
-000065d0: 6c65 2073 6570 6172 6174 656c 7920 6672  le separately fr
-000065e0: 6f6d 2074 6865 2072 6573 7420 6f66 2079  om the rest of y
-000065f0: 6f75 7220 6170 706c 6963 6174 696f 6e20  our application 
-00006600: 7769 7468 2074 6865 2068 656c 7020 6f66  with the help of
-00006610: 2045 7865 6375 746f 7273 2e0a 2d20 4465   Executors..- De
-00006620: 706c 6f79 2079 6f75 7220 6043 6861 696e  ploy your `Chain
-00006630: 6020 6f6e 204a 696e 6120 4149 2043 6c6f  ` on Jina AI Clo
-00006640: 7564 2061 6e64 2067 6574 2065 7863 6c75  ud and get exclu
-00006650: 7369 7665 2061 6363 6573 7320 746f 2041  sive access to A
-00006660: 6765 6e74 7320 6f6e 204a 696e 6120 4149  gents on Jina AI
-00006670: 2043 6c6f 7564 2028 636f 6d69 6e67 2073   Cloud (coming s
-00006680: 6f6f 6e29 0a0a 2323 2320 4578 616d 706c  oon)..### Exampl
-00006690: 6573 0a0a 7c20 4578 616d 706c 6520 7c20  es..| Example | 
-000066a0: 4c61 6e67 4368 6169 6e20 446f 6373 207c  LangChain Docs |
-000066b0: 2044 6573 6372 6970 7469 6f6e 207c 0a7c   Description |.|
-000066c0: 202d 2d2d 2d2d 2d2d 207c 202d 2d2d 2d2d   ------- | -----
-000066d0: 2d2d 2d2d 2d2d 207c 202d 2d2d 2d2d 2d2d  ------ | -------
-000066e0: 2d2d 2d2d 207c 0a7c 205b 4c4c 4d20 4368  ---- |.| [LLM Ch
-000066f0: 6169 6e5d 2865 7861 6d70 6c65 732f 6c6c  ain](examples/ll
-00006700: 6d5f 6368 6169 6e2e 6d64 2920 7c20 5b4c  m_chain.md) | [L
-00006710: 696e 6b5d 2868 7474 7073 3a2f 2f6c 616e  ink](https://lan
-00006720: 6763 6861 696e 2e72 6561 6474 6865 646f  gchain.readthedo
-00006730: 6373 2e69 6f2f 656e 2f6c 6174 6573 742f  cs.io/en/latest/
-00006740: 6d6f 6475 6c65 732f 6368 6169 6e73 2f67  modules/chains/g
-00006750: 6574 7469 6e67 5f73 7461 7274 6564 2e68  etting_started.h
-00006760: 746d 6c23 7175 6572 792d 616e 2d6c 6c6d  tml#query-an-llm
-00006770: 2d77 6974 682d 7468 652d 6c6c 6d63 6861  -with-the-llmcha
-00006780: 696e 2920 7c20 4578 706f 7365 2060 4368  in) | Expose `Ch
-00006790: 6169 6e60 2061 7320 5245 5354 6675 6c2f  ain` as RESTful/
-000067a0: 6752 5043 2f57 6562 536f 636b 6574 2041  gRPC/WebSocket A
-000067b0: 5049 206c 6f63 616c 6c79 207c 0a7c 205b  PI locally |.| [
-000067c0: 5369 6d70 6c65 2053 6571 7565 6e74 6961  Simple Sequentia
-000067d0: 6c20 4368 6169 6e5d 2865 7861 6d70 6c65  l Chain](example
-000067e0: 732f 7369 6d70 6c65 5f73 6571 7565 6e74  s/simple_sequent
-000067f0: 6961 6c5f 6368 6169 6e2e 6d64 2920 7c20  ial_chain.md) | 
-00006800: 5b4c 696e 6b5d 2868 7474 7073 3a2f 2f6c  [Link](https://l
-00006810: 616e 6763 6861 696e 2e72 6561 6474 6865  angchain.readthe
-00006820: 646f 6373 2e69 6f2f 656e 2f6c 6174 6573  docs.io/en/lates
-00006830: 742f 6d6f 6475 6c65 732f 6368 6169 6e73  t/modules/chains
-00006840: 2f67 656e 6572 6963 2f73 6571 7565 6e74  /generic/sequent
-00006850: 6961 6c5f 6368 6169 6e73 2e68 746d 6c23  ial_chains.html#
-00006860: 7369 6d70 6c65 7365 7175 656e 7469 616c  simplesequential
-00006870: 6368 6169 6e29 207c 2045 7870 6f73 6520  chain) | Expose 
-00006880: 6043 6861 696e 6020 6173 2052 4553 5466  `Chain` as RESTf
-00006890: 756c 2f67 5250 432f 5765 6253 6f63 6b65  ul/gRPC/WebSocke
-000068a0: 7420 4150 4920 6c6f 6361 6c6c 7920 7c0a  t API locally |.
-000068b0: 7c20 5b53 6571 7565 6e74 6961 6c20 4368  | [Sequential Ch
-000068c0: 6169 6e5d 2865 7861 6d70 6c65 732f 7365  ain](examples/se
-000068d0: 7175 656e 7469 616c 5f63 6861 696e 2e6d  quential_chain.m
-000068e0: 6429 207c 205b 4c69 6e6b 5d28 6874 7470  d) | [Link](http
-000068f0: 733a 2f2f 6c61 6e67 6368 6169 6e2e 7265  s://langchain.re
-00006900: 6164 7468 6564 6f63 732e 696f 2f65 6e2f  adthedocs.io/en/
-00006910: 6c61 7465 7374 2f6d 6f64 756c 6573 2f63  latest/modules/c
-00006920: 6861 696e 732f 6765 6e65 7269 632f 7365  hains/generic/se
-00006930: 7175 656e 7469 616c 5f63 6861 696e 732e  quential_chains.
-00006940: 6874 6d6c 2373 6571 7565 6e74 6961 6c2d  html#sequential-
-00006950: 6368 6169 6e29 207c 2045 7870 6f73 6520  chain) | Expose 
-00006960: 6043 6861 696e 6020 6173 2052 4553 5466  `Chain` as RESTf
-00006970: 756c 2f67 5250 432f 5765 6253 6f63 6b65  ul/gRPC/WebSocke
-00006980: 7420 4150 4920 6c6f 6361 6c6c 7920 7c0a  t API locally |.
-00006990: 7c20 5b4c 4c4d 204d 6174 6820 4368 6169  | [LLM Math Chai
-000069a0: 6e5d 2865 7861 6d70 6c65 732f 6c6c 6d5f  n](examples/llm_
-000069b0: 6d61 7468 2e6d 6429 207c 205b 4c69 6e6b  math.md) | [Link
-000069c0: 5d28 6874 7470 733a 2f2f 6c61 6e67 6368  ](https://langch
-000069d0: 6169 6e2e 7265 6164 7468 6564 6f63 732e  ain.readthedocs.
-000069e0: 696f 2f65 6e2f 6c61 7465 7374 2f6d 6f64  io/en/latest/mod
-000069f0: 756c 6573 2f63 6861 696e 732f 6578 616d  ules/chains/exam
-00006a00: 706c 6573 2f6c 6c6d 5f6d 6174 682e 6874  ples/llm_math.ht
-00006a10: 6d6c 2920 7c20 4578 706f 7365 2060 4368  ml) | Expose `Ch
-00006a20: 6169 6e60 2061 7320 5245 5354 6675 6c2f  ain` as RESTful/
-00006a30: 6752 5043 2f57 6562 536f 636b 6574 2041  gRPC/WebSocket A
-00006a40: 5049 206c 6f63 616c 6c79 207c 0a7c 205b  PI locally |.| [
-00006a50: 4c4c 4d20 5265 7175 6573 7473 2043 6861  LLM Requests Cha
-00006a60: 696e 5d28 6578 616d 706c 6573 2f6c 6c6d  in](examples/llm
-00006a70: 5f72 6571 7565 7374 735f 6368 6169 6e2e  _requests_chain.
-00006a80: 6d64 2920 7c20 5b4c 696e 6b5d 2868 7474  md) | [Link](htt
-00006a90: 7073 3a2f 2f6c 616e 6763 6861 696e 2e72  ps://langchain.r
-00006aa0: 6561 6474 6865 646f 6373 2e69 6f2f 656e  eadthedocs.io/en
-00006ab0: 2f6c 6174 6573 742f 6d6f 6475 6c65 732f  /latest/modules/
-00006ac0: 6368 6169 6e73 2f65 7861 6d70 6c65 732f  chains/examples/
-00006ad0: 6c6c 6d5f 7265 7175 6573 7473 2e68 746d  llm_requests.htm
-00006ae0: 6c29 207c 2045 7870 6f73 6520 6043 6861  l) | Expose `Cha
-00006af0: 696e 6020 6173 2052 4553 5466 756c 2f67  in` as RESTful/g
-00006b00: 5250 432f 5765 6253 6f63 6b65 7420 4150  RPC/WebSocket AP
-00006b10: 4920 6c6f 6361 6c6c 7920 7c0a 7c20 5b43  I locally |.| [C
-00006b20: 7573 746f 6d20 4368 6169 6e5d 2865 7861  ustom Chain](exa
-00006b30: 6d70 6c65 732f 6375 7374 6f6d 5f63 6861  mples/custom_cha
-00006b40: 696e 2e6d 6429 207c 205b 4c69 6e6b 5d28  in.md) | [Link](
-00006b50: 6874 7470 733a 2f2f 6c61 6e67 6368 6169  https://langchai
-00006b60: 6e2e 7265 6164 7468 6564 6f63 732e 696f  n.readthedocs.io
-00006b70: 2f65 6e2f 6c61 7465 7374 2f6d 6f64 756c  /en/latest/modul
-00006b80: 6573 2f63 6861 696e 732f 6765 7474 696e  es/chains/gettin
-00006b90: 675f 7374 6172 7465 642e 6874 6d6c 2363  g_started.html#c
-00006ba0: 7265 6174 652d 612d 6375 7374 6f6d 2d63  reate-a-custom-c
-00006bb0: 6861 696e 2d77 6974 682d 7468 652d 6368  hain-with-the-ch
-00006bc0: 6169 6e2d 636c 6173 7329 207c 2045 7870  ain-class) | Exp
-00006bd0: 6f73 6520 6043 6861 696e 6020 6173 2052  ose `Chain` as R
-00006be0: 4553 5466 756c 2f67 5250 432f 5765 6253  ESTful/gRPC/WebS
-00006bf0: 6f63 6b65 7420 4150 4920 6c6f 6361 6c6c  ocket API locall
-00006c00: 7920 7c0a 7c20 5b53 6571 7565 6e74 6961  y |.| [Sequentia
-00006c10: 6c20 4368 6169 6e73 5d28 6578 616d 706c  l Chains](exampl
-00006c20: 6573 2f73 6571 7565 6e74 6961 6c5f 6578  es/sequential_ex
-00006c30: 6563 7574 6f72 732e 6d64 2920 7c20 4e2f  ecutors.md) | N/
-00006c40: 4120 7c20 4275 696c 6420 2620 7363 616c  A | Build & scal
-00006c50: 6520 6043 6861 696e 7360 2069 6e20 7365  e `Chains` in se
-00006c60: 7061 7261 7465 2060 4578 6563 7574 6f72  parate `Executor
-00006c70: 6073 207c 0a7c 205b 4272 616e 6368 696e  `s |.| [Branchin
-00006c80: 6720 4368 6169 6e73 5d28 6578 616d 706c  g Chains](exampl
-00006c90: 6573 2f62 7261 6e63 6869 6e67 2e6d 6429  es/branching.md)
-00006ca0: 207c 204e 2f41 207c 2042 7261 6e63 6869   | N/A | Branchi
-00006cb0: 6e67 2060 4368 6169 6e73 6020 696e 2073  ng `Chains` in s
-00006cc0: 6570 6172 6174 6520 6045 7865 6375 746f  eparate `Executo
-00006cd0: 7260 7320 746f 2061 6c6c 6f77 2070 6172  r`s to allow par
-00006ce0: 616c 6c65 6c20 6578 6563 7574 696f 6e20  allel execution 
-00006cf0: 7c0a 0a23 2320 4672 6571 7565 6e74 6c79  |..## Frequently
-00006d00: 2041 736b 6564 2051 7565 7374 696f 6e73   Asked Questions
-00006d10: 0a0a 2d20 5b4d 7920 636c 6965 6e74 2074  ..- [My client t
-00006d20: 6861 7420 636f 6e6e 6563 7473 2074 6f20  hat connects to 
-00006d30: 7468 6520 4170 7020 6765 7473 2074 696d  the App gets tim
-00006d40: 6564 2d6f 7574 2c20 7768 6174 2073 686f  ed-out, what sho
-00006d50: 756c 6420 4920 646f 3f5d 2823 6d79 2d63  uld I do?](#my-c
-00006d60: 6c69 656e 742d 7468 6174 2d63 6f6e 6e65  lient-that-conne
-00006d70: 6374 732d 746f 2d74 6865 2d61 7070 2d67  cts-to-the-app-g
-00006d80: 6574 732d 7469 6d65 642d 6f75 742d 7768  ets-timed-out-wh
-00006d90: 6174 2d73 686f 756c 642d 492d 646f 290a  at-should-I-do).
-00006da0: 2d20 5b4a 436c 6f75 6420 6465 706c 6f79  - [JCloud deploy
-00006db0: 6d65 6e74 2066 6169 6c65 6420 6174 2070  ment failed at p
-00006dc0: 7573 6869 6e67 2069 6d61 6765 2074 6f20  ushing image to 
-00006dd0: 4a69 6e61 2048 7562 626c 652c 2077 6861  Jina Hubble, wha
-00006de0: 7420 7368 6f75 6c64 2049 2064 6f3f 5d28  t should I do?](
-00006df0: 236a 636c 6f75 642d 6465 706c 6f79 6d65  #jcloud-deployme
-00006e00: 6e74 2d66 6169 6c65 642d 6174 2d70 7573  nt-failed-at-pus
-00006e10: 6869 6e67 2d69 6d61 6765 2d74 6f2d 6a69  hing-image-to-ji
-00006e20: 6e61 2d68 7562 626c 652d 7768 6174 2d73  na-hubble-what-s
-00006e30: 686f 756c 642d 692d 6469 290a 0a23 2323  hould-i-di)..###
-00006e40: 204d 7920 636c 6965 6e74 2074 6861 7420   My client that 
-00006e50: 636f 6e6e 6563 7473 2074 6f20 7468 6520  connects to the 
-00006e60: 4170 7020 6765 7473 2074 696d 6564 2d6f  App gets timed-o
-00006e70: 7574 2c20 7768 6174 2073 686f 756c 6420  ut, what should 
-00006e80: 4920 646f 3f0a 0a49 6620 796f 7520 6d61  I do?..If you ma
-00006e90: 6b65 206c 6f6e 6720 4854 5450 2072 6571  ke long HTTP req
-00006ea0: 7565 7374 732c 2079 6f75 206d 6179 2065  uests, you may e
-00006eb0: 7870 6572 6965 6e63 6520 7469 6d65 6f75  xperience timeou
-00006ec0: 7473 2064 7565 2074 6f20 6c69 6d69 7461  ts due to limita
-00006ed0: 7469 6f6e 7320 696e 2074 6865 204f 5353  tions in the OSS
-00006ee0: 2077 6520 7573 6564 2069 6e20 606c 616e   we used in `lan
-00006ef0: 6763 6861 696e 2d73 6572 7665 602e 2057  gchain-serve`. W
-00006f00: 6869 6c65 2077 6520 6172 6520 776f 726b  hile we are work
-00006f10: 696e 6720 746f 2070 6572 6d61 6e65 6e74  ing to permanent
-00006f20: 6c79 2061 6464 7265 7373 2074 6869 7320  ly address this 
-00006f30: 6973 7375 652c 2077 6520 7265 636f 6d6d  issue, we recomm
-00006f40: 656e 6420 7573 696e 6720 4854 5450 2f31  end using HTTP/1
-00006f50: 2e31 2069 6e20 796f 7572 2063 6c69 656e  .1 in your clien
-00006f60: 7420 6173 2061 2074 656d 706f 7261 7279  t as a temporary
-00006f70: 2077 6f72 6b61 726f 756e 642e 0a0a 2323   workaround...##
-00006f80: 2320 4a43 6c6f 7564 2064 6570 6c6f 796d  # JCloud deploym
-00006f90: 656e 7420 6661 696c 6564 2061 7420 7075  ent failed at pu
-00006fa0: 7368 696e 6720 696d 6167 6520 746f 204a  shing image to J
-00006fb0: 696e 6120 4875 6262 6c65 2c20 7768 6174  ina Hubble, what
-00006fc0: 2073 686f 756c 6420 4920 646f 3f0a 0a50   should I do?..P
-00006fd0: 6c65 6173 6520 7573 6520 602d 2d76 6572  lease use `--ver
-00006fe0: 626f 7365 6020 616e 6420 7265 7472 7920  bose` and retry 
-00006ff0: 746f 2067 6574 206d 6f72 6520 696e 666f  to get more info
-00007000: 726d 6174 696f 6e2e 2049 6620 796f 7520  rmation. If you 
-00007010: 6172 6520 6f70 6572 6174 696e 6720 6f6e  are operating on
-00007020: 2063 6f6d 7075 7465 7220 7769 7468 2060   computer with `
-00007030: 6172 6d36 3460 2061 7263 682c 2070 6c65  arm64` arch, ple
-00007040: 6173 6520 7265 7472 7920 7769 7468 2060  ase retry with `
-00007050: 2d2d 706c 6174 666f 726d 206c 696e 7578  --platform linux
-00007060: 2f61 6d64 3634 6020 736f 2074 6865 2069  /amd64` so the i
-00007070: 6d61 6765 2063 616e 2062 6520 6275 696c  mage can be buil
-00007080: 7420 636f 7272 6563 746c 792e 0a0a 0a    t correctly....
+00004040: 9480 e294 80e2 95af 0a60 6060 0a0a 4c65  .........```..Le
+00004050: 7427 7320 6f70 656e 2074 6865 2053 7761  t's open the Swa
+00004060: 6767 6572 2055 4920 746f 2074 6573 7420  gger UI to test 
+00004070: 6f75 7220 4150 4920 6f6e 204a 696e 6120  our API on Jina 
+00004080: 4149 2043 6c6f 7564 2e20 5769 7468 2060  AI Cloud. With `
+00004090: 5472 7920 6974 206f 7574 6020 6275 7474  Try it out` butt
+000040a0: 6f6e 2c20 7765 2063 616e 2074 6573 7420  on, we can test 
+000040b0: 6f75 7220 4150 4920 7769 7468 2064 6966  our API with dif
+000040c0: 6665 7265 6e74 2069 6e70 7574 732e 0a0a  ferent inputs...
+000040d0: 3c64 6574 6169 6c73 3e0a 3c73 756d 6d61  <details>.<summa
+000040e0: 7279 3e53 686f 7720 5377 6167 6765 7220  ry>Show Swagger 
+000040f0: 5549 3c2f 7375 6d6d 6172 793e 0a0a 3c70  UI</summary>..<p
+00004100: 2066 6c6f 6174 3d22 6365 6e74 6572 223e   float="center">
+00004110: 0a20 203c 696d 6720 7372 633d 222e 6769  .  <img src=".gi
+00004120: 7468 7562 2f69 6d61 6765 732f 6a63 6c6f  thub/images/jclo
+00004130: 7564 2d73 7761 6767 6572 2d75 692e 706e  ud-swagger-ui.pn
+00004140: 6722 2077 6964 7468 3d22 3430 3022 202f  g" width="400" /
+00004150: 3e0a 2020 3c69 6d67 2073 7263 3d22 2e67  >.  <img src=".g
+00004160: 6974 6875 622f 696d 6167 6573 2f6a 636c  ithub/images/jcl
+00004170: 6f75 642d 6f70 656e 6170 692e 706e 6722  oud-openapi.png"
+00004180: 2077 6964 7468 3d22 3330 3022 202f 3e0a   width="300" />.
+00004190: 3c2f 703e 0a0a 3c2f 6465 7461 696c 733e  </p>..</details>
+000041a0: 0a0a 0a4c 6574 2773 2074 6573 7420 7468  ...Let's test th
+000041b0: 6520 4150 4920 6f6e 204a 436c 6f75 6420  e API on JCloud 
+000041c0: 7769 7468 2060 486f 7720 6d61 6e79 2070  with `How many p
+000041d0: 656f 706c 6520 6c69 7665 2069 6e20 6361  eople live in ca
+000041e0: 6e61 6461 2061 7320 6f66 2032 3032 333f  nada as of 2023?
+000041f0: 6020 696e 7075 7420 7769 7468 2061 2063  ` input with a c
+00004200: 5552 4c20 636f 6d6d 616e 6420 2852 6570  URL command (Rep
+00004210: 6c61 6365 2074 6865 2048 6f73 746e 616d  lace the Hostnam
+00004220: 6520 7769 7468 2079 6f75 7220 6f77 6e20  e with your own 
+00004230: 686f 7374 6e61 6d65 293a 0a0a 6060 6062  hostname):..```b
+00004240: 6173 680a 6375 726c 202d 5820 2750 4f53  ash.curl -X 'POS
+00004250: 5427 205c 0a20 2027 6874 7470 733a 2f2f  T' \.  'https://
+00004260: 6c61 6e67 6368 6169 6e2d 6565 3461 6566  langchain-ee4aef
+00004270: 3537 6439 2d68 7474 702e 776f 6c66 2e6a  57d9-http.wolf.j
+00004280: 696e 612e 6169 2f61 736b 2720 5c0a 2020  ina.ai/ask' \.  
+00004290: 2d48 2027 6163 6365 7074 3a20 6170 706c  -H 'accept: appl
+000042a0: 6963 6174 696f 6e2f 6a73 6f6e 2720 5c0a  ication/json' \.
+000042b0: 2020 2d48 2027 436f 6e74 656e 742d 5479    -H 'Content-Ty
+000042c0: 7065 3a20 6170 706c 6963 6174 696f 6e2f  pe: application/
+000042d0: 6a73 6f6e 2720 5c0a 2020 2d64 2027 7b0a  json' \.  -d '{.
+000042e0: 2020 2269 6e70 7574 223a 2022 486f 7720    "input": "How 
+000042f0: 6d61 6e79 2070 656f 706c 6520 6c69 7665  many people live
+00004300: 2069 6e20 6361 6e61 6461 2061 7320 6f66   in canada as of
+00004310: 2032 3032 333f 222c 0a20 2022 656e 7673   2023?",.  "envs
+00004320: 223a 207b 0a20 2020 2022 4f50 454e 4149  ": {.    "OPENAI
+00004330: 5f41 5049 5f4b 4559 223a 2022 2722 247b  _API_KEY": "'"${
+00004340: 4f50 454e 4149 5f41 5049 5f4b 4559 7d22  OPENAI_API_KEY}"
+00004350: 2722 2c0a 2020 2020 2253 4552 5041 5049  '",.    "SERPAPI
+00004360: 5f41 5049 5f4b 4559 223a 2022 2722 247b  _API_KEY": "'"${
+00004370: 5345 5250 4150 495f 4150 495f 4b45 597d  SERPAPI_API_KEY}
+00004380: 2227 220a 2020 7d0a 7d27 0a60 6060 0a0a  "'".  }.}'.```..
+00004390: 6060 606a 736f 6e0a 7b0a 2020 2272 6573  ```json.{.  "res
+000043a0: 756c 7422 3a20 2241 7272 722c 2074 6865  ult": "Arrr, the
+000043b0: 7265 2062 6520 3338 2c36 3435 2c36 3730  re be 38,645,670
+000043c0: 2070 656f 706c 6520 6c69 7669 6e27 2069   people livin' i
+000043d0: 6e20 4361 6e61 6461 2061 7320 6f66 2032  n Canada as of 2
+000043e0: 3032 3321 222c 0a20 2022 6572 726f 7222  023!",.  "error"
+000043f0: 3a20 2222 2c0a 2020 2273 7464 6f75 7422  : "",.  "stdout"
+00004400: 3a20 2241 6e73 7765 7220 7468 6520 666f  : "Answer the fo
+00004410: 6c6c 6f77 696e 6720 7175 6573 7469 6f6e  llowing question
+00004420: 7320 6173 2062 6573 7420 796f 7520 6361  s as best you ca
+00004430: 6e2c 2062 7574 2073 7065 616b 696e 6720  n, but speaking 
+00004440: 6173 2061 2070 6972 6174 6520 6d69 6768  as a pirate migh
+00004450: 7420 7370 6561 6b2e 2059 6f75 2068 6176  t speak. You hav
+00004460: 6520 6163 6365 7373 2074 6f20 7468 6520  e access to the 
+00004470: 666f 6c6c 6f77 696e 6720 746f 6f6c 733a  following tools:
+00004480: 5c6e 5c6e 5365 6172 6368 3a20 7573 6566  \n\nSearch: usef
+00004490: 756c 2066 6f72 2077 6865 6e20 796f 7520  ul for when you 
+000044a0: 6e65 6564 2074 6f20 616e 7377 6572 2071  need to answer q
+000044b0: 7565 7374 696f 6e73 2061 626f 7574 2063  uestions about c
+000044c0: 7572 7265 6e74 2065 7665 6e74 735c 6e5c  urrent events\n\
+000044d0: 6e55 7365 2074 6865 2066 6f6c 6c6f 7769  nUse the followi
+000044e0: 6e67 2066 6f72 6d61 743a 5c6e 5c6e 5175  ng format:\n\nQu
+000044f0: 6573 7469 6f6e 3a20 7468 6520 696e 7075  estion: the inpu
+00004500: 7420 7175 6573 7469 6f6e 2079 6f75 206d  t question you m
+00004510: 7573 7420 616e 7377 6572 5c6e 5468 6f75  ust answer\nThou
+00004520: 6768 743a 2079 6f75 2073 686f 756c 6420  ght: you should 
+00004530: 616c 7761 7973 2074 6869 6e6b 2061 626f  always think abo
+00004540: 7574 2077 6861 7420 746f 2064 6f5c 6e41  ut what to do\nA
+00004550: 6374 696f 6e3a 2074 6865 2061 6374 696f  ction: the actio
+00004560: 6e20 746f 2074 616b 652c 2073 686f 756c  n to take, shoul
+00004570: 6420 6265 206f 6e65 206f 6620 5b53 6561  d be one of [Sea
+00004580: 7263 685d 5c6e 4163 7469 6f6e 2049 6e70  rch]\nAction Inp
+00004590: 7574 3a20 7468 6520 696e 7075 7420 746f  ut: the input to
+000045a0: 2074 6865 2061 6374 696f 6e5c 6e4f 6273   the action\nObs
+000045b0: 6572 7661 7469 6f6e 3a20 7468 6520 7265  ervation: the re
+000045c0: 7375 6c74 206f 6620 7468 6520 6163 7469  sult of the acti
+000045d0: 6f6e 5c6e 2e2e 2e20 2874 6869 7320 5468  on\n... (this Th
+000045e0: 6f75 6768 742f 4163 7469 6f6e 2f41 6374  ought/Action/Act
+000045f0: 696f 6e20 496e 7075 742f 4f62 7365 7276  ion Input/Observ
+00004600: 6174 696f 6e20 6361 6e20 7265 7065 6174  ation can repeat
+00004610: 204e 2074 696d 6573 295c 6e54 686f 7567   N times)\nThoug
+00004620: 6874 3a20 4920 6e6f 7720 6b6e 6f77 2074  ht: I now know t
+00004630: 6865 2066 696e 616c 2061 6e73 7765 725c  he final answer\
+00004640: 6e46 696e 616c 2041 6e73 7765 723a 2074  nFinal Answer: t
+00004650: 6865 2066 696e 616c 2061 6e73 7765 7220  he final answer 
+00004660: 746f 2074 6865 206f 7269 6769 6e61 6c20  to the original 
+00004670: 696e 7075 7420 7175 6573 7469 6f6e 5c6e  input question\n
+00004680: 5c6e 4265 6769 6e21 2052 656d 656d 6265  \nBegin! Remembe
+00004690: 7220 746f 2073 7065 616b 2061 7320 6120  r to speak as a 
+000046a0: 7069 7261 7465 2077 6865 6e20 6769 7669  pirate when givi
+000046b0: 6e67 2079 6f75 7220 6669 6e61 6c20 616e  ng your final an
+000046c0: 7377 6572 2e20 5573 6520 6c6f 7473 206f  swer. Use lots o
+000046d0: 6620 5c22 4172 6773 5c22 5c6e 5c6e 2020  f \"Args\"\n\n  
+000046e0: 2020 5175 6573 7469 6f6e 3a20 7b69 6e70    Question: {inp
+000046f0: 7574 7d5c 6e20 2020 207b 6167 656e 745f  ut}\n    {agent_
+00004700: 7363 7261 7463 6870 6164 7d5c 6e5c 6e5c  scratchpad}\n\n\
+00004710: 6e5c 7530 3031 625b 316d 3e20 456e 7465  n\u001b[1m> Ente
+00004720: 7269 6e67 206e 6577 2041 6765 6e74 4578  ring new AgentEx
+00004730: 6563 7574 6f72 2063 6861 696e 2e2e 2e5c  ecutor chain...\
+00004740: 7530 3031 625b 306d 5c6e 5c75 3030 3162  u001b[0m\n\u001b
+00004750: 5b33 323b 316d 5c75 3030 3162 5b31 3b33  [32;1m\u001b[1;3
+00004760: 6d5c 6e54 686f 7567 6874 3a20 4920 6e65  m\nThought: I ne
+00004770: 6564 2074 6f20 6669 6e64 206f 7574 2068  ed to find out h
+00004780: 6f77 206d 616e 7920 7065 6f70 6c65 206c  ow many people l
+00004790: 6976 6520 696e 2043 616e 6164 615c 6e41  ive in Canada\nA
+000047a0: 6374 696f 6e3a 2053 6561 7263 685c 6e41  ction: Search\nA
+000047b0: 6374 696f 6e20 496e 7075 743a 2048 6f77  ction Input: How
+000047c0: 206d 616e 7920 7065 6f70 6c65 206c 6976   many people liv
+000047d0: 6520 696e 2043 616e 6164 6120 6173 206f  e in Canada as o
+000047e0: 6620 3230 3233 5c75 3030 3162 5b30 6d5c  f 2023\u001b[0m\
+000047f0: 6e4f 6273 6572 7661 7469 6f6e 3a20 5c75  nObservation: \u
+00004800: 3030 3162 5b33 363b 316d 5c75 3030 3162  001b[36;1m\u001b
+00004810: 5b31 3b33 6d54 6865 2063 7572 7265 6e74  [1;3mThe current
+00004820: 2070 6f70 756c 6174 696f 6e20 6f66 2043   population of C
+00004830: 616e 6164 6120 6973 2033 382c 3634 352c  anada is 38,645,
+00004840: 3637 3020 6173 206f 6620 5765 646e 6573  670 as of Wednes
+00004850: 6461 792c 204d 6172 6368 2032 392c 2032  day, March 29, 2
+00004860: 3032 332c 2062 6173 6564 206f 6e20 576f  023, based on Wo
+00004870: 726c 646f 6d65 7465 7220 656c 6162 6f72  rldometer elabor
+00004880: 6174 696f 6e20 6f66 2074 6865 206c 6174  ation of the lat
+00004890: 6573 7420 556e 6974 6564 204e 6174 696f  est United Natio
+000048a0: 6e73 2064 6174 612e 5c75 3030 3162 5b30  ns data.\u001b[0
+000048b0: 6d5c 6e54 686f 7567 6874 3a5c 7530 3031  m\nThought:\u001
+000048c0: 625b 3332 3b31 6d5c 7530 3031 625b 313b  b[32;1m\u001b[1;
+000048d0: 336d 2049 206e 6f77 206b 6e6f 7720 7468  3m I now know th
+000048e0: 6520 6669 6e61 6c20 616e 7377 6572 5c6e  e final answer\n
+000048f0: 4669 6e61 6c20 416e 7377 6572 3a20 4172  Final Answer: Ar
+00004900: 7272 2c20 7468 6572 6520 6265 2033 382c  rr, there be 38,
+00004910: 3634 352c 3637 3020 7065 6f70 6c65 206c  645,670 people l
+00004920: 6976 696e 2720 696e 2043 616e 6164 6120  ivin' in Canada 
+00004930: 6173 206f 6620 3230 3233 215c 7530 3031  as of 2023!\u001
+00004940: 625b 306d 5c6e 5c6e 5c75 3030 3162 5b31  b[0m\n\n\u001b[1
+00004950: 6d3e 2046 696e 6973 6865 6420 6368 6169  m> Finished chai
+00004960: 6e2e 5c75 3030 3162 5b30 6d22 0a7d 0a60  n.\u001b[0m".}.`
+00004970: 6060 0a0a 2323 2323 2320 5768 6174 2068  ``..##### What h
+00004980: 6170 7065 6e65 643f 0a0a 2d20 496e 2061  appened?..- In a
+00004990: 206d 6174 7465 7220 6f66 2066 6577 2073   matter of few s
+000049a0: 6563 6f6e 6473 2c20 7765 2776 6520 6465  econds, we've de
+000049b0: 706c 6f79 6564 206f 7572 2041 5049 206f  ployed our API o
+000049c0: 6e20 4a69 6e61 2041 4920 436c 6f75 6420  n Jina AI Cloud 
+000049d0: f09f 8e89 0a2d 2054 6865 2041 5049 2069  .....- The API i
+000049e0: 7320 7365 7276 6572 6c65 7373 2061 6e64  s serverless and
+000049f0: 2073 6361 6c61 626c 652c 2073 6f20 7765   scalable, so we
+00004a00: 2063 616e 2073 6361 6c65 2075 7020 7468   can scale up th
+00004a10: 6520 4150 4920 746f 2068 616e 646c 6520  e API to handle 
+00004a20: 6d6f 7265 2072 6571 7565 7374 732e 200a  more requests. .
+00004a30: 2d20 596f 7520 6d69 6768 7420 6f62 7365  - You might obse
+00004a40: 7276 6520 6120 6465 6c61 7920 696e 2074  rve a delay in t
+00004a50: 6865 2066 6972 7374 2072 6571 7565 7374  he first request
+00004a60: 2c20 7468 6174 2773 2064 7565 2074 6f20  , that's due to 
+00004a70: 7468 6520 7761 726d 2d75 7020 7469 6d65  the warm-up time
+00004a80: 206f 6620 7468 6520 4150 492e 2053 7562   of the API. Sub
+00004a90: 7365 7175 656e 7420 7265 7175 6573 7473  sequent requests
+00004aa0: 2077 696c 6c20 6265 2066 6173 7465 722e   will be faster.
+00004ab0: 0a2d 2054 6865 2041 5049 2069 6e63 6c75  .- The API inclu
+00004ac0: 6465 7320 6120 5377 6167 6765 7220 5549  des a Swagger UI
+00004ad0: 2061 6e64 2074 6865 204f 7065 6e41 5049   and the OpenAPI
+00004ae0: 2073 7065 6369 6669 6361 7469 6f6e 2c20   specification, 
+00004af0: 736f 2069 7420 6361 6e20 6265 2065 6173  so it can be eas
+00004b00: 696c 7920 696e 7465 6772 6174 6564 2077  ily integrated w
+00004b10: 6974 6820 6f74 6865 7220 7365 7276 6963  ith other servic
+00004b20: 6573 2e20 0a2d 204e 6f77 2c20 6f74 6865  es. .- Now, othe
+00004b30: 7220 6167 656e 7473 2063 616e 2069 6e74  r agents can int
+00004b40: 6567 7261 7465 2077 6974 6820 796f 7572  egrate with your
+00004b50: 2061 6765 6e74 7320 6f6e 204a 696e 6120   agents on Jina 
+00004b60: 4149 2043 6c6f 7564 2074 6861 6e6b 7320  AI Cloud thanks 
+00004b70: 746f 2074 6865 205b 4f70 656e 4150 4920  to the [OpenAPI 
+00004b80: 4167 656e 745d 2868 7474 7073 3a2f 2f70  Agent](https://p
+00004b90: 7974 686f 6e2e 6c61 6e67 6368 6169 6e2e  ython.langchain.
+00004ba0: 636f 6d2f 656e 2f6c 6174 6573 742f 6d6f  com/en/latest/mo
+00004bb0: 6475 6c65 732f 6167 656e 7473 2f74 6f6f  dules/agents/too
+00004bc0: 6c6b 6974 732f 6578 616d 706c 6573 2f6f  lkits/examples/o
+00004bd0: 7065 6e61 7069 2e68 746d 6c29 20f0 9f92  penapi.html) ...
+00004be0: a10a 0a0a 0a2d 2d2d 0a0a 2323 2323 2052  .....---..#### R
+00004bf0: 6561 6368 206f 7574 2074 6f20 7573 20f0  each out to us .
+00004c00: 9f93 9e0a 0a2d 2053 6572 7665 726c 6573  .....- Serverles
+00004c10: 7320 6973 206e 6f74 2079 6f75 7220 7468  s is not your th
+00004c20: 696e 673f 0a2d 2044 6f20 796f 7520 7761  ing?.- Do you wa
+00004c30: 6e74 206c 6172 6765 7220 696e 7374 616e  nt larger instan
+00004c40: 6365 7320 666f 7220 796f 7572 2041 5049  ces for your API
+00004c50: 3f0a 2d20 4c6f 6f6b 696e 6720 666f 7220  ?.- Looking for 
+00004c60: 6669 6c65 2075 706c 6f61 6473 2c20 6f72  file uploads, or
+00004c70: 206f 7468 6572 2064 6174 612d 696e 2c20   other data-in, 
+00004c80: 6461 7461 2d6f 7574 2066 6561 7475 7265  data-out feature
+00004c90: 733f 0a2d 2044 6f20 796f 7520 7761 6e74  s?.- Do you want
+00004ca0: 2074 6f20 7365 7475 7020 6375 7374 6f6d   to setup custom
+00004cb0: 2061 7574 686f 7269 7a61 7469 6f6e 2066   authorization f
+00004cc0: 6f72 2079 6f75 7220 4150 493f 0a0a 0af0  or your API?....
+00004cd0: 9f93 a320 476f 7420 796f 7572 2061 7474  ... Got your att
+00004ce0: 656e 7469 6f6e 3f20 5b4a 6f69 6e20 7573  ention? [Join us
+00004cf0: 206f 6e20 536c 6163 6b5d 2868 7474 7073   on Slack](https
+00004d00: 3a2f 2f6a 696e 612e 6169 2f73 6c61 636b  ://jina.ai/slack
+00004d10: 2f29 2061 6e64 2077 6527 6420 6265 2068  /) and we'd be h
+00004d20: 6170 7079 2074 6f20 6865 6c70 2079 6f75  appy to help you
+00004d30: 206f 7574 2e0a 0a2d 2d2d 0a0a 0a23 2323   out...---...###
+00004d40: 2060 6c63 2d73 6572 7665 600a 0a60 6c63   `lc-serve`..`lc
+00004d50: 2d73 6572 7665 6020 6973 2061 2043 4c49  -serve` is a CLI
+00004d60: 2074 6f6f 6c20 7468 6174 2068 656c 7073   tool that helps
+00004d70: 2079 6f75 2074 6f20 6465 706c 6f79 2079   you to deploy y
+00004d80: 6f75 7220 6167 656e 7473 206f 6e20 4a69  our agents on Ji
+00004d90: 6e61 2041 4920 436c 6f75 642e 0a0a 0a7c  na AI Cloud....|
+00004da0: 2044 6573 6372 6970 7469 6f6e 207c 2043   Description | C
+00004db0: 6f6d 6d61 6e64 207c 200a 7c20 2d2d 2d20  ommand | .| --- 
+00004dc0: 7c20 2d2d 2d3a 207c 0a7c 2044 6570 6c6f  | ---: |.| Deplo
+00004dd0: 7920 796f 7572 2061 7070 206c 6f63 616c  y your app local
+00004de0: 6c79 207c 2060 6c63 2d73 6572 7665 2064  ly | `lc-serve d
+00004df0: 6570 6c6f 7920 6c6f 6361 6c20 6170 7060  eploy local app`
+00004e00: 207c 0a7c 2044 6570 6c6f 7920 796f 7572   |.| Deploy your
+00004e10: 2061 7070 206f 6e20 4a69 6e61 2041 4920   app on Jina AI 
+00004e20: 436c 6f75 6420 7c20 606c 632d 7365 7276  Cloud | `lc-serv
+00004e30: 6520 6465 706c 6f79 206a 636c 6f75 6420  e deploy jcloud 
+00004e40: 6170 7060 207c 0a7c 2055 7064 6174 6520  app` |.| Update 
+00004e50: 6578 6973 7469 6e67 2061 7070 206f 6e20  existing app on 
+00004e60: 4a69 6e61 2041 4920 436c 6f75 6420 7c20  Jina AI Cloud | 
+00004e70: 606c 632d 7365 7276 6520 6465 706c 6f79  `lc-serve deploy
+00004e80: 206a 636c 6f75 6420 6170 7020 2d2d 6170   jcloud app --ap
+00004e90: 702d 6964 203c 6170 702d 6964 3e60 207c  p-id <app-id>` |
+00004ea0: 0a7c 2047 6574 2061 7070 2073 7461 7475  .| Get app statu
+00004eb0: 7320 6f6e 204a 696e 6120 4149 2043 6c6f  s on Jina AI Clo
+00004ec0: 7564 207c 2060 6c63 2d73 6572 7665 2073  ud | `lc-serve s
+00004ed0: 7461 7475 7320 3c61 7070 2d69 643e 6020  tatus <app-id>` 
+00004ee0: 7c0a 7c20 4c69 7374 2061 6c6c 2061 7070  |.| List all app
+00004ef0: 7320 6f6e 204a 696e 6120 4149 2043 6c6f  s on Jina AI Clo
+00004f00: 7564 207c 2060 6c63 2d73 6572 7665 206c  ud | `lc-serve l
+00004f10: 6973 7460 207c 0a7c 2052 656d 6f76 6520  ist` |.| Remove 
+00004f20: 6170 7020 6f6e 204a 696e 6120 4149 2043  app on Jina AI C
+00004f30: 6c6f 7564 207c 2060 6c63 2d73 6572 7665  loud | `lc-serve
+00004f40: 2072 656d 6f76 6520 3c61 7070 2d69 643e   remove <app-id>
+00004f50: 6020 7c0a 0a0a 2d2d 2d0a 0a23 2323 2041  ` |...---..### A
+00004f60: 6765 6e74 7320 506c 6179 6772 6f75 6e64  gents Playground
+00004f70: 20f0 9f95 b9ef b88f f09f 8eae f09f 8c90   ...............
+00004f80: 0a0a 5b4c 616e 6743 6861 696e 2061 6765  ..[LangChain age
+00004f90: 6e74 735d 2868 7474 7073 3a2f 2f70 7974  nts](https://pyt
+00004fa0: 686f 6e2e 6c61 6e67 6368 6169 6e2e 636f  hon.langchain.co
+00004fb0: 6d2f 656e 2f6c 6174 6573 742f 6d6f 6475  m/en/latest/modu
+00004fc0: 6c65 732f 6167 656e 7473 2f67 6574 7469  les/agents/getti
+00004fd0: 6e67 5f73 7461 7274 6564 2e68 746d 6c29  ng_started.html)
+00004fe0: 2075 7365 204c 4c4d 7320 746f 2064 6574   use LLMs to det
+00004ff0: 6572 6d69 6e65 2074 6865 2061 6374 696f  ermine the actio
+00005000: 6e73 2074 6f20 6265 2074 616b 656e 2069  ns to be taken i
+00005010: 6e20 7768 6174 206f 7264 6572 2e20 416e  n what order. An
+00005020: 2061 6374 696f 6e20 6361 6e20 6569 7468   action can eith
+00005030: 6572 2062 6520 7573 696e 6720 6120 746f  er be using a to
+00005040: 6f6c 2061 6e64 206f 6273 6572 7669 6e67  ol and observing
+00005050: 2069 7473 206f 7574 7075 742c 206f 7220   its output, or 
+00005060: 7265 7475 726e 696e 6720 746f 2074 6865  returning to the
+00005070: 2075 7365 722e 2057 6527 7665 2068 6f73   user. We've hos
+00005080: 7465 6420 6120 2a2a 5b53 7472 6561 6d6c  ted a **[Streaml
+00005090: 6974 2050 6c61 7967 726f 756e 645d 2868  it Playground](h
+000050a0: 7474 7073 3a2f 2f6c 616e 6763 6861 696e  ttps://langchain
+000050b0: 2e77 6f6c 662e 6a69 6e61 2e61 692f 706c  .wolf.jina.ai/pl
+000050c0: 6179 6772 6f75 6e64 2f29 2a2a 206f 6e20  ayground/)** on 
+000050d0: 4a69 6e61 2041 4920 436c 6f75 6420 746f  Jina AI Cloud to
+000050e0: 2069 6e74 6572 6163 7420 7769 7468 2074   interact with t
+000050f0: 6865 2061 6765 6e74 732c 2077 6869 6368  he agents, which
+00005100: 2061 6363 6570 7473 2077 6974 6820 666f   accepts with fo
+00005110: 6c6c 6f77 696e 6720 696e 7075 7473 3a0a  llowing inputs:.
+00005120: 0a2d 202a 2a5b 4167 656e 7420 5479 7065  .- **[Agent Type
+00005130: 735d 2868 7474 7073 3a2f 2f70 7974 686f  s](https://pytho
+00005140: 6e2e 6c61 6e67 6368 6169 6e2e 636f 6d2f  n.langchain.com/
+00005150: 656e 2f6c 6174 6573 742f 6d6f 6475 6c65  en/latest/module
+00005160: 732f 6167 656e 7473 2f61 6765 6e74 732e  s/agents/agents.
+00005170: 6874 6d6c 293a 2a2a 2043 686f 6f73 6520  html):** Choose 
+00005180: 6672 6f6d 2064 6966 6665 7265 6e74 2061  from different a
+00005190: 6765 6e74 2074 7970 6573 2074 6861 7420  gent types that 
+000051a0: 4c61 6e67 6368 6169 6e20 7375 7070 6f72  Langchain suppor
+000051b0: 7473 2e20 0a0a 2d20 2a2a 5b54 6f6f 6c73  ts. ..- **[Tools
+000051c0: 5d28 6874 7470 733a 2f2f 7079 7468 6f6e  ](https://python
+000051d0: 2e6c 616e 6763 6861 696e 2e63 6f6d 2f65  .langchain.com/e
+000051e0: 6e2f 6c61 7465 7374 2f6d 6f64 756c 6573  n/latest/modules
+000051f0: 2f61 6765 6e74 732f 746f 6f6c 732e 6874  /agents/tools.ht
+00005200: 6d6c 293a 2a2a 2043 686f 6f73 6520 6672  ml):** Choose fr
+00005210: 6f6d 2064 6966 6665 7265 6e74 2074 6f6f  om different too
+00005220: 6c73 2074 6861 7420 4c61 6e67 6368 6169  ls that Langchai
+00005230: 6e20 7375 7070 6f72 7473 2e20 536f 6d65  n supports. Some
+00005240: 2074 6f6f 6c73 206d 6179 2072 6571 7569   tools may requi
+00005250: 7265 2061 6e20 4150 4920 746f 6b65 6e20  re an API token 
+00005260: 6f72 206f 7468 6572 2072 656c 6174 6564  or other related
+00005270: 2061 7267 756d 656e 7473 2e0a 0a54 6f20   arguments...To 
+00005280: 7573 6520 7468 6520 706c 6179 6772 6f75  use the playgrou
+00005290: 6e64 2c20 7369 6d70 6c79 2074 7970 6520  nd, simply type 
+000052a0: 796f 7572 2069 6e70 7574 2069 6e20 7468  your input in th
+000052b0: 6520 7465 7874 2062 6f78 2070 726f 7669  e text box provi
+000052c0: 6465 6420 746f 2067 6574 2074 6865 2061  ded to get the a
+000052d0: 6765 6e74 2773 206f 7574 7075 7420 616e  gent's output an
+000052e0: 6420 6368 6169 6e20 6f66 2074 686f 7567  d chain of thoug
+000052f0: 6874 2e20 456e 6a6f 7920 6578 706c 6f72  ht. Enjoy explor
+00005300: 696e 6720 4c61 6e67 6368 6169 6e27 7320  ing Langchain's 
+00005310: 6361 7061 6269 6c69 7469 6573 2120 496e  capabilities! In
+00005320: 2061 6464 6974 696f 6e20 746f 2073 7472   addition to str
+00005330: 6561 6d6c 6974 2c20 796f 7520 6361 6e20  eamlit, you can 
+00005340: 616c 736f 2075 7365 206f 7572 2052 4553  also use our RES
+00005350: 5466 756c 2041 5049 7320 6f6e 2074 6865  Tful APIs on the
+00005360: 2070 6c61 7967 726f 756e 6420 746f 2069   playground to i
+00005370: 6e74 6572 6163 7420 7769 7468 2074 6865  nteract with the
+00005380: 2061 6765 6e74 732e 200a 0a0a 2323 2320   agents. ...### 
+00005390: 5b5a 6572 6f2d 7368 6f74 2052 6561 6374  [Zero-shot React
+000053a0: 2044 6573 6372 6970 7469 6f6e 2061 6765   Description age
+000053b0: 6e74 2077 6974 6820 5365 7270 4150 4920  nt with SerpAPI 
+000053c0: 616e 6420 4361 6c63 756c 6174 6f72 5d28  and Calculator](
+000053d0: 6874 7470 733a 2f2f 7079 7468 6f6e 2e6c  https://python.l
+000053e0: 616e 6763 6861 696e 2e63 6f6d 2f65 6e2f  angchain.com/en/
+000053f0: 6c61 7465 7374 2f6d 6f64 756c 6573 2f61  latest/modules/a
+00005400: 6765 6e74 732f 6765 7474 696e 675f 7374  gents/getting_st
+00005410: 6172 7465 642e 6874 6d6c 290a 0a23 2323  arted.html)..###
+00005420: 2320 5374 7265 616d 6c69 7420 506c 6179  # Streamlit Play
+00005430: 6772 6f75 6e64 0a0a 215b 5374 7265 616d  ground..![Stream
+00005440: 6c69 7420 506c 6179 6772 6f75 6e64 5d28  lit Playground](
+00005450: 2e67 6974 6875 622f 696d 6167 6573 2f70  .github/images/p
+00005460: 6c61 7967 726f 756e 645f 6f6e 652e 6769  layground_one.gi
+00005470: 6629 0a0a 2323 2323 2052 4553 5466 756c  f)..#### RESTful
+00005480: 2041 5049 0a0a 6060 6062 6173 680a 6578   API..```bash.ex
+00005490: 706f 7274 204f 5045 4e41 495f 4150 495f  port OPENAI_API_
+000054a0: 4b45 593d 736b 2d2a 2a2a 0a65 7870 6f72  KEY=sk-***.expor
+000054b0: 7420 5345 5250 4150 495f 4150 495f 4b45  t SERPAPI_API_KE
+000054c0: 593d 2a2a 2a0a 0a63 7572 6c20 2d73 5820  Y=***..curl -sX 
+000054d0: 504f 5354 2027 6874 7470 733a 2f2f 6c61  POST 'https://la
+000054e0: 6e67 6368 6169 6e2e 776f 6c66 2e6a 696e  ngchain.wolf.jin
+000054f0: 612e 6169 2f61 7069 2f72 756e 2720 5c0a  a.ai/api/run' \.
+00005500: 2020 2d48 2027 6163 6365 7074 3a20 6170    -H 'accept: ap
+00005510: 706c 6963 6174 696f 6e2f 6a73 6f6e 2720  plication/json' 
+00005520: 5c0a 2020 2d48 2027 436f 6e74 656e 742d  \.  -H 'Content-
+00005530: 5479 7065 3a20 6170 706c 6963 6174 696f  Type: applicatio
+00005540: 6e2f 6a73 6f6e 2720 5c0a 2020 2d2d 6461  n/json' \.  --da
+00005550: 7461 2d72 6177 2027 7b0a 2020 2020 2274  ta-raw '{.    "t
+00005560: 6578 7422 3a20 2257 686f 2069 7320 4c65  ext": "Who is Le
+00005570: 6f20 4469 4361 7072 696f 7320 6769 726c  o DiCaprios girl
+00005580: 6672 6965 6e64 3f20 5768 6174 2069 7320  friend? What is 
+00005590: 6865 7220 6375 7272 656e 7420 6167 6520  her current age 
+000055a0: 7261 6973 6564 2074 6f20 7468 6520 302e  raised to the 0.
+000055b0: 3433 2070 6f77 6572 3f22 2c0a 2020 2020  43 power?",.    
+000055c0: 2270 6172 616d 6574 6572 7322 3a20 7b0a  "parameters": {.
+000055d0: 2020 2020 2020 2020 2274 6f6f 6c73 223a          "tools":
+000055e0: 207b 0a20 2020 2020 2020 2020 2020 2022   {.            "
+000055f0: 746f 6f6c 5f6e 616d 6573 223a 205b 2273  tool_names": ["s
+00005600: 6572 7061 7069 222c 2022 6c6c 6d2d 6d61  erpapi", "llm-ma
+00005610: 7468 225d 0a20 2020 2020 2020 207d 2c0a  th"].        },.
+00005620: 2020 2020 2020 2020 2261 6765 6e74 223a          "agent":
+00005630: 2022 7a65 726f 2d73 686f 742d 7265 6163   "zero-shot-reac
+00005640: 742d 6465 7363 7269 7074 696f 6e22 2c0a  t-description",.
+00005650: 2020 2020 2020 2020 2276 6572 626f 7365          "verbose
+00005660: 223a 2074 7275 650a 2020 2020 7d2c 0a20  ": true.    },. 
+00005670: 2020 2022 656e 7673 223a 207b 0a20 2020     "envs": {.   
+00005680: 2020 2020 2022 4f50 454e 4149 5f41 5049       "OPENAI_API
+00005690: 5f4b 4559 223a 2022 2722 247b 4f50 454e  _KEY": "'"${OPEN
+000056a0: 4149 5f41 5049 5f4b 4559 7d22 2722 2c0a  AI_API_KEY}"'",.
+000056b0: 2020 2020 2020 2020 2253 4552 5041 5049          "SERPAPI
+000056c0: 5f41 5049 5f4b 4559 223a 2022 2722 247b  _API_KEY": "'"${
+000056d0: 5345 5250 4150 495f 4150 495f 4b45 597d  SERPAPI_API_KEY}
+000056e0: 2227 220a 2020 2020 7d0a 7d27 207c 206a  "'".    }.}' | j
+000056f0: 710a 6060 6020 0a0a 6060 606a 736f 6e0a  q.``` ..```json.
+00005700: 7b0a 2020 2272 6573 756c 7422 3a20 2243  {.  "result": "C
+00005710: 616d 696c 6120 4d6f 7272 6f6e 6520 6973  amila Morrone is
+00005720: 204c 656f 2044 6943 6170 7269 6f27 7320   Leo DiCaprio's 
+00005730: 6769 726c 6672 6965 6e64 2c20 616e 6420  girlfriend, and 
+00005740: 6865 7220 6375 7272 656e 7420 6167 6520  her current age 
+00005750: 7261 6973 6564 2074 6f20 7468 6520 302e  raised to the 0.
+00005760: 3433 2070 6f77 6572 2069 7320 332e 3632  43 power is 3.62
+00005770: 3631 3236 3036 3131 3532 3935 3237 2e22  61260611529527."
+00005780: 2c0a 2020 2263 6861 696e 5f6f 665f 7468  ,.  "chain_of_th
+00005790: 6f75 6768 7422 3a20 225c 7530 3031 625b  ought": "\u001b[
+000057a0: 316d 3e20 456e 7465 7269 6e67 206e 6577  1m> Entering new
+000057b0: 2041 6765 6e74 4578 6563 7574 6f72 2063   AgentExecutor c
+000057c0: 6861 696e 2e2e 2e5c 7530 3031 625b 306d  hain...\u001b[0m
+000057d0: 5c75 3030 3162 5b33 323b 316d 5c75 3030  \u001b[32;1m\u00
+000057e0: 3162 5b31 3b33 6d20 4920 6e65 6564 2074  1b[1;3m I need t
+000057f0: 6f20 6669 6e64 206f 7574 2074 6865 206e  o find out the n
+00005800: 616d 6520 6f66 204c 656f 2773 2067 6972  ame of Leo's gir
+00005810: 6c66 7269 656e 6420 616e 6420 7468 656e  lfriend and then
+00005820: 2075 7365 2074 6865 2063 616c 6375 6c61   use the calcula
+00005830: 746f 7220 746f 2063 616c 6375 6c61 7465  tor to calculate
+00005840: 2068 6572 2061 6765 2074 6f20 7468 6520   her age to the 
+00005850: 302e 3433 2070 6f77 6572 2e41 6374 696f  0.43 power.Actio
+00005860: 6e3a 2053 6561 7263 6841 6374 696f 6e20  n: SearchAction 
+00005870: 496e 7075 743a 204c 656f 2044 6943 6170  Input: Leo DiCap
+00005880: 7269 6f20 6769 726c 6672 6965 6e64 5c75  rio girlfriend\u
+00005890: 3030 3162 5b30 6d4f 6273 6572 7661 7469  001b[0mObservati
+000058a0: 6f6e 3a20 5c75 3030 3162 5b33 363b 316d  on: \u001b[36;1m
+000058b0: 5c75 3030 3162 5b31 3b33 6d44 6943 6170  \u001b[1;3mDiCap
+000058c0: 7269 6f20 6d65 7420 6163 746f 7220 4361  rio met actor Ca
+000058d0: 6d69 6c61 204d 6f72 726f 6e65 2069 6e20  mila Morrone in 
+000058e0: 4465 6365 6d62 6572 2032 3031 372c 2077  December 2017, w
+000058f0: 6865 6e20 7368 6520 7761 7320 3230 2061  hen she was 20 a
+00005900: 6e64 2068 6520 7761 7320 3433 2e20 5468  nd he was 43. Th
+00005910: 6579 2077 6572 6520 7370 6f74 7465 6420  ey were spotted 
+00005920: 6174 2043 6f61 6368 656c 6c61 2061 6e64  at Coachella and
+00005930: 2077 656e 7420 6f6e 206d 756c 7469 706c   went on multipl
+00005940: 6520 7661 6361 7469 6f6e 7320 746f 6765  e vacations toge
+00005950: 7468 6572 2e20 536f 6d65 2072 6570 6f72  ther. Some repor
+00005960: 7473 2073 7567 6765 7374 6564 2074 6861  ts suggested tha
+00005970: 7420 4469 4361 7072 696f 2077 6173 2072  t DiCaprio was r
+00005980: 6561 6479 2074 6f20 6173 6b20 4d6f 7272  eady to ask Morr
+00005990: 6f6e 6520 746f 206d 6172 7279 2068 696d  one to marry him
+000059a0: 2e20 5468 6520 636f 7570 6c65 206d 6164  . The couple mad
+000059b0: 6520 7468 6569 7220 7265 6420 6361 7270  e their red carp
+000059c0: 6574 2064 6562 7574 2061 7420 7468 6520  et debut at the 
+000059d0: 3230 3230 2041 6361 6465 6d79 2041 7761  2020 Academy Awa
+000059e0: 7264 732e 5c75 3030 3162 5b30 6d54 686f  rds.\u001b[0mTho
+000059f0: 7567 6874 3a5c 7530 3031 625b 3332 3b31  ught:\u001b[32;1
+00005a00: 6d5c 7530 3031 625b 313b 336d 2049 206e  m\u001b[1;3m I n
+00005a10: 6565 6420 746f 2075 7365 2074 6865 2063  eed to use the c
+00005a20: 616c 6375 6c61 746f 7220 746f 2063 616c  alculator to cal
+00005a30: 6375 6c61 7465 2068 6572 2061 6765 2074  culate her age t
+00005a40: 6f20 7468 6520 302e 3433 2070 6f77 6572  o the 0.43 power
+00005a50: 4163 7469 6f6e 3a20 4361 6c63 756c 6174  Action: Calculat
+00005a60: 6f72 4163 7469 6f6e 2049 6e70 7574 3a20  orAction Input: 
+00005a70: 3230 5e30 2e34 335c 7530 3031 625b 306d  20^0.43\u001b[0m
+00005a80: 4f62 7365 7276 6174 696f 6e3a 205c 7530  Observation: \u0
+00005a90: 3031 625b 3333 3b31 6d5c 7530 3031 625b  01b[33;1m\u001b[
+00005aa0: 313b 336d 416e 7377 6572 3a20 332e 3632  1;3mAnswer: 3.62
+00005ab0: 3631 3236 3036 3131 3532 3935 3237 5c75  61260611529527\u
+00005ac0: 3030 3162 5b30 6d54 686f 7567 6874 3a5c  001b[0mThought:\
+00005ad0: 7530 3031 625b 3332 3b31 6d5c 7530 3031  u001b[32;1m\u001
+00005ae0: 625b 313b 336d 2049 206e 6f77 206b 6e6f  b[1;3m I now kno
+00005af0: 7720 7468 6520 6669 6e61 6c20 616e 7377  w the final answ
+00005b00: 6572 4669 6e61 6c20 416e 7377 6572 3a20  erFinal Answer: 
+00005b10: 4361 6d69 6c61 204d 6f72 726f 6e65 2069  Camila Morrone i
+00005b20: 7320 4c65 6f20 4469 4361 7072 696f 2773  s Leo DiCaprio's
+00005b30: 2067 6972 6c66 7269 656e 642c 2061 6e64   girlfriend, and
+00005b40: 2068 6572 2063 7572 7265 6e74 2061 6765   her current age
+00005b50: 2072 6169 7365 6420 746f 2074 6865 2030   raised to the 0
+00005b60: 2e34 3320 706f 7765 7220 6973 2033 2e36  .43 power is 3.6
+00005b70: 3236 3132 3630 3631 3135 3239 3532 372e  261260611529527.
+00005b80: 5c75 3030 3162 5b30 6d5c 7530 3031 625b  \u001b[0m\u001b[
+00005b90: 316d 3e20 4669 6e69 7368 6564 2063 6861  1m> Finished cha
+00005ba0: 696e 2e5c 7530 3031 625b 306d 220a 7d0a  in.\u001b[0m".}.
+00005bb0: 6060 600a 0a23 2323 205b 5365 6c66 2041  ```..### [Self A
+00005bc0: 736b 2057 6974 6820 5365 6172 6368 5d28  sk With Search](
+00005bd0: 6874 7470 733a 2f2f 7079 7468 6f6e 2e6c  https://python.l
+00005be0: 616e 6763 6861 696e 2e63 6f6d 2f65 6e2f  angchain.com/en/
+00005bf0: 6c61 7465 7374 2f6d 6f64 756c 6573 2f61  latest/modules/a
+00005c00: 6765 6e74 732f 696d 706c 656d 656e 7461  gents/implementa
+00005c10: 7469 6f6e 732f 7365 6c66 5f61 736b 5f77  tions/self_ask_w
+00005c20: 6974 685f 7365 6172 6368 2e68 746d 6c29  ith_search.html)
+00005c30: 0a0a 2323 2323 2053 7472 6561 6d6c 6974  ..#### Streamlit
+00005c40: 2050 6c61 7967 726f 756e 640a 0a21 5b53   Playground..![S
+00005c50: 7472 6561 6d6c 6974 2050 6c61 7967 726f  treamlit Playgro
+00005c60: 756e 645d 282e 6769 7468 7562 2f69 6d61  und](.github/ima
+00005c70: 6765 732f 706c 6179 6772 6f75 6e64 5f74  ges/playground_t
+00005c80: 776f 2e67 6966 290a 0a23 2323 2320 5245  wo.gif)..#### RE
+00005c90: 5354 6675 6c20 4150 490a 0a60 6060 6261  STful API..```ba
+00005ca0: 7368 0a65 7870 6f72 7420 4f50 454e 4149  sh.export OPENAI
+00005cb0: 5f41 5049 5f4b 4559 3d73 6b2d 2a2a 2a0a  _API_KEY=sk-***.
+00005cc0: 6578 706f 7274 2053 4552 5041 5049 5f41  export SERPAPI_A
+00005cd0: 5049 5f4b 4559 3d2a 2a2a 0a0a 6375 726c  PI_KEY=***..curl
+00005ce0: 202d 7358 2050 4f53 5420 2768 7474 7073   -sX POST 'https
+00005cf0: 3a2f 2f6c 616e 6763 6861 696e 2e77 6f6c  ://langchain.wol
+00005d00: 662e 6a69 6e61 2e61 692f 6170 692f 7275  f.jina.ai/api/ru
+00005d10: 6e27 205c 0a20 202d 4820 2761 6363 6570  n' \.  -H 'accep
+00005d20: 743a 2061 7070 6c69 6361 7469 6f6e 2f6a  t: application/j
+00005d30: 736f 6e27 205c 0a20 202d 4820 2743 6f6e  son' \.  -H 'Con
+00005d40: 7465 6e74 2d54 7970 653a 2061 7070 6c69  tent-Type: appli
+00005d50: 6361 7469 6f6e 2f6a 736f 6e27 205c 0a20  cation/json' \. 
+00005d60: 202d 2d64 6174 612d 7261 7720 277b 0a20   --data-raw '{. 
+00005d70: 2020 2022 7465 7874 223a 2022 5768 6174     "text": "What
+00005d80: 2069 7320 7468 6520 686f 6d65 746f 776e   is the hometown
+00005d90: 206f 6620 7468 6520 7265 6967 6e69 6e67   of the reigning
+00005da0: 206d 656e 7320 552e 532e 204f 7065 6e20   mens U.S. Open 
+00005db0: 6368 616d 7069 6f6e 3f22 2c0a 2020 2020  champion?",.    
+00005dc0: 2270 6172 616d 6574 6572 7322 3a20 7b0a  "parameters": {.
+00005dd0: 2020 2020 2020 2020 2274 6f6f 6c73 223a          "tools":
+00005de0: 207b 0a20 2020 2020 2020 2020 2020 2022   {.            "
+00005df0: 746f 6f6c 5f6e 616d 6573 223a 205b 2273  tool_names": ["s
+00005e00: 6572 7061 7069 225d 0a20 2020 2020 2020  erpapi"].       
+00005e10: 207d 2c0a 2020 2020 2020 2020 2261 6765   },.        "age
+00005e20: 6e74 223a 2022 7365 6c66 2d61 736b 2d77  nt": "self-ask-w
+00005e30: 6974 682d 7365 6172 6368 222c 0a20 2020  ith-search",.   
+00005e40: 2020 2020 2022 7665 7262 6f73 6522 3a20       "verbose": 
+00005e50: 7472 7565 0a20 2020 207d 2c0a 2020 2020  true.    },.    
+00005e60: 2265 6e76 7322 3a20 7b0a 2020 2020 2020  "envs": {.      
+00005e70: 2020 224f 5045 4e41 495f 4150 495f 4b45    "OPENAI_API_KE
+00005e80: 5922 3a20 2227 2224 7b4f 5045 4e41 495f  Y": "'"${OPENAI_
+00005e90: 4150 495f 4b45 597d 2227 222c 0a20 2020  API_KEY}"'",.   
+00005ea0: 2020 2020 2022 5345 5250 4150 495f 4150       "SERPAPI_AP
+00005eb0: 495f 4b45 5922 3a20 2227 2224 7b53 4552  I_KEY": "'"${SER
+00005ec0: 5041 5049 5f41 5049 5f4b 4559 7d22 2722  PAPI_API_KEY}"'"
+00005ed0: 0a20 2020 207d 0a7d 2720 7c20 6a71 0a60  .    }.}' | jq.`
+00005ee0: 6060 0a0a 6060 606a 736f 6e0a 7b0a 2020  ``..```json.{.  
+00005ef0: 2272 6573 756c 7422 3a20 2245 6c20 5061  "result": "El Pa
+00005f00: 6c6d 6172 2c20 4d75 7263 6961 2c20 5370  lmar, Murcia, Sp
+00005f10: 6169 6e22 2c0a 2020 2263 6861 696e 5f6f  ain",.  "chain_o
+00005f20: 665f 7468 6f75 6768 7422 3a20 225c 7530  f_thought": "\u0
+00005f30: 3031 625b 316d 3e20 456e 7465 7269 6e67  01b[1m> Entering
+00005f40: 206e 6577 2041 6765 6e74 4578 6563 7574   new AgentExecut
+00005f50: 6f72 2063 6861 696e 2e2e 2e5c 7530 3031  or chain...\u001
+00005f60: 625b 306d 5c75 3030 3162 5b33 323b 316d  b[0m\u001b[32;1m
+00005f70: 5c75 3030 3162 5b31 3b33 6d20 5965 732e  \u001b[1;3m Yes.
+00005f80: 466f 6c6c 6f77 2075 703a 2057 686f 2069  Follow up: Who i
+00005f90: 7320 7468 6520 7265 6967 6e69 6e67 206d  s the reigning m
+00005fa0: 656e 7320 552e 532e 204f 7065 6e20 6368  ens U.S. Open ch
+00005fb0: 616d 7069 6f6e 3f5c 7530 3031 625b 306d  ampion?\u001b[0m
+00005fc0: 496e 7465 726d 6564 6961 7465 2061 6e73  Intermediate ans
+00005fd0: 7765 723a 205c 7530 3031 625b 3336 3b31  wer: \u001b[36;1
+00005fe0: 6d5c 7530 3031 625b 313b 336d 4361 726c  m\u001b[1;3mCarl
+00005ff0: 6f73 2041 6c63 6172 617a 2047 6172 6669  os Alcaraz Garfi
+00006000: 615c 7530 3031 625b 306d 5c75 3030 3162  a\u001b[0m\u001b
+00006010: 5b33 323b 316d 5c75 3030 3162 5b31 3b33  [32;1m\u001b[1;3
+00006020: 6d46 6f6c 6c6f 7720 7570 3a20 5768 6174  mFollow up: What
+00006030: 2069 7320 4361 726c 6f73 2041 6c63 6172   is Carlos Alcar
+00006040: 617a 2047 6172 6669 6127 7320 686f 6d65  az Garfia's home
+00006050: 746f 776e 3f5c 7530 3031 625b 306d 496e  town?\u001b[0mIn
+00006060: 7465 726d 6564 6961 7465 2061 6e73 7765  termediate answe
+00006070: 723a 205c 7530 3031 625b 3336 3b31 6d5c  r: \u001b[36;1m\
+00006080: 7530 3031 625b 313b 336d 4361 726c 6f73  u001b[1;3mCarlos
+00006090: 2041 6c63 6172 617a 2047 6172 6669 6120   Alcaraz Garfia 
+000060a0: 7761 7320 626f 726e 206f 6e20 4d61 7920  was born on May 
+000060b0: 352c 2032 3030 332c 2069 6e20 456c 2050  5, 2003, in El P
+000060c0: 616c 6d61 722c 204d 7572 6369 612c 2053  almar, Murcia, S
+000060d0: 7061 696e 2074 6f20 7061 7265 6e74 7320  pain to parents 
+000060e0: 4361 726c 6f73 2041 6c63 6172 617a 2047  Carlos Alcaraz G
+000060f0: 6f6e 7ac3 a16c 657a 2061 6e64 2056 6972  onz..lez and Vir
+00006100: 6769 6e69 6120 4761 7266 6961 2045 7363  ginia Garfia Esc
+00006110: 616e 64c3 b36e 2e20 4865 2068 6173 2074  and..n. He has t
+00006120: 6872 6565 2073 6962 6c69 6e67 732e 5c75  hree siblings.\u
+00006130: 3030 3162 5b30 6d5c 7530 3031 625b 3332  001b[0m\u001b[32
+00006140: 3b31 6d5c 7530 3031 625b 313b 336d 536f  ;1m\u001b[1;3mSo
+00006150: 2074 6865 2066 696e 616c 2061 6e73 7765   the final answe
+00006160: 7220 6973 3a20 456c 2050 616c 6d61 722c  r is: El Palmar,
+00006170: 204d 7572 6369 612c 2053 7061 696e 5c75   Murcia, Spain\u
+00006180: 3030 3162 5b30 6d5c 7530 3031 625b 316d  001b[0m\u001b[1m
+00006190: 3e20 4669 6e69 7368 6564 2063 6861 696e  > Finished chain
+000061a0: 2e5c 7530 3031 625b 306d 220a 7d0a 6060  .\u001b[0m".}.``
+000061b0: 600a 0a2d 2d2d 0a0a 2323 2043 6861 696e  `..---..## Chain
+000061c0: 7320 6f6e 204a 696e 6120 f09f 93a6 f09f  s on Jina ......
+000061d0: 9a80 0a0a 5b43 6861 696e 735d 2868 7474  ....[Chains](htt
+000061e0: 7073 3a2f 2f70 7974 686f 6e2e 6c61 6e67  ps://python.lang
+000061f0: 6368 6169 6e2e 636f 6d2f 656e 2f6c 6174  chain.com/en/lat
+00006200: 6573 742f 6d6f 6475 6c65 732f 6368 6169  est/modules/chai
+00006210: 6e73 2f67 6574 7469 6e67 5f73 7461 7274  ns/getting_start
+00006220: 6564 2e68 746d 6c29 2069 6e20 4c61 6e67  ed.html) in Lang
+00006230: 4368 6169 6e20 616c 6c6f 7720 7573 6572  Chain allow user
+00006240: 7320 746f 2063 6f6d 6269 6e65 2063 6f6d  s to combine com
+00006250: 706f 6e65 6e74 7320 746f 2063 7265 6174  ponents to creat
+00006260: 6520 6120 7369 6e67 6c65 2c20 636f 6865  e a single, cohe
+00006270: 7265 6e74 2061 7070 6c69 6361 7469 6f6e  rent application
+00006280: 2e20 5769 7468 204a 696e 612c 200a 0a2d  . With Jina, ..-
+00006290: 2059 6f75 2063 616e 2065 7870 6f73 6520   You can expose 
+000062a0: 796f 7572 2060 4368 6169 6e60 2061 7320  your `Chain` as 
+000062b0: 5245 5354 6675 6c2f 6752 5043 2f57 6562  RESTful/gRPC/Web
+000062c0: 536f 636b 6574 2041 5049 2e0a 2d20 456e  Socket API..- En
+000062d0: 6162 6c65 2060 4368 6169 6e60 7320 746f  able `Chain`s to
+000062e0: 2064 6570 6c6f 7920 2620 7363 616c 6520   deploy & scale 
+000062f0: 7365 7061 7261 7465 6c79 2066 726f 6d20  separately from 
+00006300: 7468 6520 7265 7374 206f 6620 796f 7572  the rest of your
+00006310: 2061 7070 6c69 6361 7469 6f6e 2077 6974   application wit
+00006320: 6820 7468 6520 6865 6c70 206f 6620 4578  h the help of Ex
+00006330: 6563 7574 6f72 732e 0a2d 2044 6570 6c6f  ecutors..- Deplo
+00006340: 7920 796f 7572 2060 4368 6169 6e60 206f  y your `Chain` o
+00006350: 6e20 4a69 6e61 2041 4920 436c 6f75 6420  n Jina AI Cloud 
+00006360: 616e 6420 6765 7420 6578 636c 7573 6976  and get exclusiv
+00006370: 6520 6163 6365 7373 2074 6f20 4167 656e  e access to Agen
+00006380: 7473 206f 6e20 4a69 6e61 2041 4920 436c  ts on Jina AI Cl
+00006390: 6f75 6420 2863 6f6d 696e 6720 736f 6f6e  oud (coming soon
+000063a0: 290a 0a23 2323 2045 7861 6d70 6c65 730a  )..### Examples.
+000063b0: 0a7c 2045 7861 6d70 6c65 207c 204c 616e  .| Example | Lan
+000063c0: 6743 6861 696e 2044 6f63 7320 7c20 4465  gChain Docs | De
+000063d0: 7363 7269 7074 696f 6e20 7c0a 7c20 2d2d  scription |.| --
+000063e0: 2d2d 2d2d 2d20 7c20 2d2d 2d2d 2d2d 2d2d  ----- | --------
+000063f0: 2d2d 2d20 7c20 2d2d 2d2d 2d2d 2d2d 2d2d  --- | ----------
+00006400: 2d20 7c0a 7c20 5b4c 4c4d 2043 6861 696e  - |.| [LLM Chain
+00006410: 5d28 6578 616d 706c 6573 2f6c 6c6d 5f63  ](examples/llm_c
+00006420: 6861 696e 2e6d 6429 207c 205b 4c69 6e6b  hain.md) | [Link
+00006430: 5d28 6874 7470 733a 2f2f 6c61 6e67 6368  ](https://langch
+00006440: 6169 6e2e 7265 6164 7468 6564 6f63 732e  ain.readthedocs.
+00006450: 696f 2f65 6e2f 6c61 7465 7374 2f6d 6f64  io/en/latest/mod
+00006460: 756c 6573 2f63 6861 696e 732f 6765 7474  ules/chains/gett
+00006470: 696e 675f 7374 6172 7465 642e 6874 6d6c  ing_started.html
+00006480: 2371 7565 7279 2d61 6e2d 6c6c 6d2d 7769  #query-an-llm-wi
+00006490: 7468 2d74 6865 2d6c 6c6d 6368 6169 6e29  th-the-llmchain)
+000064a0: 207c 2045 7870 6f73 6520 6043 6861 696e   | Expose `Chain
+000064b0: 6020 6173 2052 4553 5466 756c 2f67 5250  ` as RESTful/gRP
+000064c0: 432f 5765 6253 6f63 6b65 7420 4150 4920  C/WebSocket API 
+000064d0: 6c6f 6361 6c6c 7920 7c0a 7c20 5b53 696d  locally |.| [Sim
+000064e0: 706c 6520 5365 7175 656e 7469 616c 2043  ple Sequential C
+000064f0: 6861 696e 5d28 6578 616d 706c 6573 2f73  hain](examples/s
+00006500: 696d 706c 655f 7365 7175 656e 7469 616c  imple_sequential
+00006510: 5f63 6861 696e 2e6d 6429 207c 205b 4c69  _chain.md) | [Li
+00006520: 6e6b 5d28 6874 7470 733a 2f2f 6c61 6e67  nk](https://lang
+00006530: 6368 6169 6e2e 7265 6164 7468 6564 6f63  chain.readthedoc
+00006540: 732e 696f 2f65 6e2f 6c61 7465 7374 2f6d  s.io/en/latest/m
+00006550: 6f64 756c 6573 2f63 6861 696e 732f 6765  odules/chains/ge
+00006560: 6e65 7269 632f 7365 7175 656e 7469 616c  neric/sequential
+00006570: 5f63 6861 696e 732e 6874 6d6c 2373 696d  _chains.html#sim
+00006580: 706c 6573 6571 7565 6e74 6961 6c63 6861  plesequentialcha
+00006590: 696e 2920 7c20 4578 706f 7365 2060 4368  in) | Expose `Ch
+000065a0: 6169 6e60 2061 7320 5245 5354 6675 6c2f  ain` as RESTful/
+000065b0: 6752 5043 2f57 6562 536f 636b 6574 2041  gRPC/WebSocket A
+000065c0: 5049 206c 6f63 616c 6c79 207c 0a7c 205b  PI locally |.| [
+000065d0: 5365 7175 656e 7469 616c 2043 6861 696e  Sequential Chain
+000065e0: 5d28 6578 616d 706c 6573 2f73 6571 7565  ](examples/seque
+000065f0: 6e74 6961 6c5f 6368 6169 6e2e 6d64 2920  ntial_chain.md) 
+00006600: 7c20 5b4c 696e 6b5d 2868 7474 7073 3a2f  | [Link](https:/
+00006610: 2f6c 616e 6763 6861 696e 2e72 6561 6474  /langchain.readt
+00006620: 6865 646f 6373 2e69 6f2f 656e 2f6c 6174  hedocs.io/en/lat
+00006630: 6573 742f 6d6f 6475 6c65 732f 6368 6169  est/modules/chai
+00006640: 6e73 2f67 656e 6572 6963 2f73 6571 7565  ns/generic/seque
+00006650: 6e74 6961 6c5f 6368 6169 6e73 2e68 746d  ntial_chains.htm
+00006660: 6c23 7365 7175 656e 7469 616c 2d63 6861  l#sequential-cha
+00006670: 696e 2920 7c20 4578 706f 7365 2060 4368  in) | Expose `Ch
+00006680: 6169 6e60 2061 7320 5245 5354 6675 6c2f  ain` as RESTful/
+00006690: 6752 5043 2f57 6562 536f 636b 6574 2041  gRPC/WebSocket A
+000066a0: 5049 206c 6f63 616c 6c79 207c 0a7c 205b  PI locally |.| [
+000066b0: 4c4c 4d20 4d61 7468 2043 6861 696e 5d28  LLM Math Chain](
+000066c0: 6578 616d 706c 6573 2f6c 6c6d 5f6d 6174  examples/llm_mat
+000066d0: 682e 6d64 2920 7c20 5b4c 696e 6b5d 2868  h.md) | [Link](h
+000066e0: 7474 7073 3a2f 2f6c 616e 6763 6861 696e  ttps://langchain
+000066f0: 2e72 6561 6474 6865 646f 6373 2e69 6f2f  .readthedocs.io/
+00006700: 656e 2f6c 6174 6573 742f 6d6f 6475 6c65  en/latest/module
+00006710: 732f 6368 6169 6e73 2f65 7861 6d70 6c65  s/chains/example
+00006720: 732f 6c6c 6d5f 6d61 7468 2e68 746d 6c29  s/llm_math.html)
+00006730: 207c 2045 7870 6f73 6520 6043 6861 696e   | Expose `Chain
+00006740: 6020 6173 2052 4553 5466 756c 2f67 5250  ` as RESTful/gRP
+00006750: 432f 5765 6253 6f63 6b65 7420 4150 4920  C/WebSocket API 
+00006760: 6c6f 6361 6c6c 7920 7c0a 7c20 5b4c 4c4d  locally |.| [LLM
+00006770: 2052 6571 7565 7374 7320 4368 6169 6e5d   Requests Chain]
+00006780: 2865 7861 6d70 6c65 732f 6c6c 6d5f 7265  (examples/llm_re
+00006790: 7175 6573 7473 5f63 6861 696e 2e6d 6429  quests_chain.md)
+000067a0: 207c 205b 4c69 6e6b 5d28 6874 7470 733a   | [Link](https:
+000067b0: 2f2f 6c61 6e67 6368 6169 6e2e 7265 6164  //langchain.read
+000067c0: 7468 6564 6f63 732e 696f 2f65 6e2f 6c61  thedocs.io/en/la
+000067d0: 7465 7374 2f6d 6f64 756c 6573 2f63 6861  test/modules/cha
+000067e0: 696e 732f 6578 616d 706c 6573 2f6c 6c6d  ins/examples/llm
+000067f0: 5f72 6571 7565 7374 732e 6874 6d6c 2920  _requests.html) 
+00006800: 7c20 4578 706f 7365 2060 4368 6169 6e60  | Expose `Chain`
+00006810: 2061 7320 5245 5354 6675 6c2f 6752 5043   as RESTful/gRPC
+00006820: 2f57 6562 536f 636b 6574 2041 5049 206c  /WebSocket API l
+00006830: 6f63 616c 6c79 207c 0a7c 205b 4375 7374  ocally |.| [Cust
+00006840: 6f6d 2043 6861 696e 5d28 6578 616d 706c  om Chain](exampl
+00006850: 6573 2f63 7573 746f 6d5f 6368 6169 6e2e  es/custom_chain.
+00006860: 6d64 2920 7c20 5b4c 696e 6b5d 2868 7474  md) | [Link](htt
+00006870: 7073 3a2f 2f6c 616e 6763 6861 696e 2e72  ps://langchain.r
+00006880: 6561 6474 6865 646f 6373 2e69 6f2f 656e  eadthedocs.io/en
+00006890: 2f6c 6174 6573 742f 6d6f 6475 6c65 732f  /latest/modules/
+000068a0: 6368 6169 6e73 2f67 6574 7469 6e67 5f73  chains/getting_s
+000068b0: 7461 7274 6564 2e68 746d 6c23 6372 6561  tarted.html#crea
+000068c0: 7465 2d61 2d63 7573 746f 6d2d 6368 6169  te-a-custom-chai
+000068d0: 6e2d 7769 7468 2d74 6865 2d63 6861 696e  n-with-the-chain
+000068e0: 2d63 6c61 7373 2920 7c20 4578 706f 7365  -class) | Expose
+000068f0: 2060 4368 6169 6e60 2061 7320 5245 5354   `Chain` as REST
+00006900: 6675 6c2f 6752 5043 2f57 6562 536f 636b  ful/gRPC/WebSock
+00006910: 6574 2041 5049 206c 6f63 616c 6c79 207c  et API locally |
+00006920: 0a7c 205b 5365 7175 656e 7469 616c 2043  .| [Sequential C
+00006930: 6861 696e 735d 2865 7861 6d70 6c65 732f  hains](examples/
+00006940: 7365 7175 656e 7469 616c 5f65 7865 6375  sequential_execu
+00006950: 746f 7273 2e6d 6429 207c 204e 2f41 207c  tors.md) | N/A |
+00006960: 2042 7569 6c64 2026 2073 6361 6c65 2060   Build & scale `
+00006970: 4368 6169 6e73 6020 696e 2073 6570 6172  Chains` in separ
+00006980: 6174 6520 6045 7865 6375 746f 7260 7320  ate `Executor`s 
+00006990: 7c0a 7c20 5b42 7261 6e63 6869 6e67 2043  |.| [Branching C
+000069a0: 6861 696e 735d 2865 7861 6d70 6c65 732f  hains](examples/
+000069b0: 6272 616e 6368 696e 672e 6d64 2920 7c20  branching.md) | 
+000069c0: 4e2f 4120 7c20 4272 616e 6368 696e 6720  N/A | Branching 
+000069d0: 6043 6861 696e 7360 2069 6e20 7365 7061  `Chains` in sepa
+000069e0: 7261 7465 2060 4578 6563 7574 6f72 6073  rate `Executor`s
+000069f0: 2074 6f20 616c 6c6f 7720 7061 7261 6c6c   to allow parall
+00006a00: 656c 2065 7865 6375 7469 6f6e 207c 0a0a  el execution |..
+00006a10: 0a0a                                     ..
```

### Comparing `langchain-serve-0.0.9.dev22/README.md` & `langchain-serve-0.0.9.dev9/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,1723 +1,1620 @@
-00000000: 3c70 2061 6c69 676e 3d22 6365 6e74 6572  <p align="center
-00000010: 223e 0a3c 623e 4c61 6e67 4368 6169 6e20  ">.<b>LangChain 
-00000020: 4170 7073 206f 6e20 5072 6f64 7563 7469  Apps on Producti
-00000030: 6f6e 2077 6974 6820 4a69 6e61 20f0 9f9a  on with Jina ...
-00000040: 803c 2f62 3e0a 3c2f 703e 0a0a 3c70 2061  .</b>.</p>..<p a
-00000050: 6c69 676e 3d63 656e 7465 723e 0a3c 6120  lign=center>.<a 
-00000060: 6872 6566 3d22 6874 7470 733a 2f2f 7079  href="https://py
-00000070: 7069 2e6f 7267 2f70 726f 6a65 6374 2f6c  pi.org/project/l
-00000080: 616e 6763 6861 696e 2d73 6572 7665 2f22  angchain-serve/"
-00000090: 3e3c 696d 6720 616c 743d 2250 7950 4922  ><img alt="PyPI"
-000000a0: 2073 7263 3d22 6874 7470 733a 2f2f 696d   src="https://im
-000000b0: 672e 7368 6965 6c64 732e 696f 2f70 7970  g.shields.io/pyp
-000000c0: 692f 762f 6c61 6e67 6368 6169 6e2d 7365  i/v/langchain-se
-000000d0: 7276 653f 6c61 6265 6c3d 5265 6c65 6173  rve?label=Releas
-000000e0: 6526 7374 796c 653d 666c 6174 2d73 7175  e&style=flat-squ
-000000f0: 6172 6522 3e3c 2f61 3e0a 3c61 2068 7265  are"></a>.<a hre
-00000100: 663d 2268 7474 7073 3a2f 2f6a 696e 612e  f="https://jina.
-00000110: 6169 2f73 6c61 636b 223e 3c69 6d67 2073  ai/slack"><img s
-00000120: 7263 3d22 6874 7470 733a 2f2f 696d 672e  rc="https://img.
-00000130: 7368 6965 6c64 732e 696f 2f62 6164 6765  shields.io/badge
-00000140: 2f53 6c61 636b 2d33 2e36 6b2d 626c 7565  /Slack-3.6k-blue
-00000150: 7669 6f6c 6574 3f6c 6f67 6f3d 736c 6163  violet?logo=slac
-00000160: 6b26 616d 703b 6c6f 676f 436f 6c6f 723d  k&amp;logoColor=
-00000170: 7768 6974 6526 7374 796c 653d 666c 6174  white&style=flat
-00000180: 2d73 7175 6172 6522 3e3c 2f61 3e0a 3c61  -square"></a>.<a
-00000190: 2068 7265 663d 2268 7474 7073 3a2f 2f70   href="https://p
-000001a0: 7970 6973 7461 7473 2e6f 7267 2f70 6163  ypistats.org/pac
-000001b0: 6b61 6765 732f 6c61 6e67 6368 6169 6e2d  kages/langchain-
-000001c0: 7365 7276 6522 3e3c 696d 6720 616c 743d  serve"><img alt=
-000001d0: 2250 7950 4920 2d20 446f 776e 6c6f 6164  "PyPI - Download
-000001e0: 7320 6672 6f6d 206f 6666 6963 6961 6c20  s from official 
-000001f0: 7079 7069 7374 6174 7322 2073 7263 3d22  pypistats" src="
-00000200: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
-00000210: 6c64 732e 696f 2f70 7970 692f 646d 2f6c  lds.io/pypi/dm/l
-00000220: 616e 6763 6861 696e 2d73 6572 7665 3f73  angchain-serve?s
-00000230: 7479 6c65 3d66 6c61 742d 7371 7561 7265  tyle=flat-square
-00000240: 223e 3c2f 613e 0a3c 6120 6872 6566 3d22  "></a>.<a href="
-00000250: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000260: 6f6d 2f6a 696e 612d 6169 2f6c 616e 6763  om/jina-ai/langc
-00000270: 6861 696e 2d73 6572 7665 2f61 6374 696f  hain-serve/actio
-00000280: 6e73 2f77 6f72 6b66 6c6f 7773 2f63 642e  ns/workflows/cd.
-00000290: 796d 6c22 3e3c 696d 6720 616c 743d 2247  yml"><img alt="G
-000002a0: 6974 6875 6220 4344 2073 7461 7475 7322  ithub CD status"
-000002b0: 2073 7263 3d22 6874 7470 733a 2f2f 6769   src="https://gi
-000002c0: 7468 7562 2e63 6f6d 2f6a 696e 612d 6169  thub.com/jina-ai
-000002d0: 2f6c 616e 6763 6861 696e 2d73 6572 7665  /langchain-serve
-000002e0: 2f61 6374 696f 6e73 2f77 6f72 6b66 6c6f  /actions/workflo
-000002f0: 7773 2f63 642e 796d 6c2f 6261 6467 652e  ws/cd.yml/badge.
-00000300: 7376 6722 3e3c 2f61 3e0a 3c2f 703e 0a0a  svg"></a>.</p>..
-00000310: 0a5b 4a69 6e61 5d28 6874 7470 733a 2f2f  .[Jina](https://
-00000320: 6769 7468 7562 2e63 6f6d 2f6a 696e 612d  github.com/jina-
-00000330: 6169 2f6a 696e 6129 2069 7320 616e 206f  ai/jina) is an o
-00000340: 7065 6e2d 736f 7572 6365 2066 7261 6d65  pen-source frame
-00000350: 776f 726b 2074 6f20 6275 696c 642c 2064  work to build, d
-00000360: 6570 6c6f 7920 2620 6d61 6e61 6765 206d  eploy & manage m
-00000370: 6163 6869 6e65 206c 6561 726e 696e 6720  achine learning 
-00000380: 6170 706c 6963 6174 696f 6e73 2061 7420  applications at 
-00000390: 7363 616c 652e 205b 4c61 6e67 4368 6169  scale. [LangChai
-000003a0: 6e5d 2868 7474 7073 3a2f 2f70 7974 686f  n](https://pytho
-000003b0: 6e2e 6c61 6e67 6368 6169 6e2e 636f 6d2f  n.langchain.com/
-000003c0: 656e 2f6c 6174 6573 742f 696e 6465 782e  en/latest/index.
-000003d0: 6874 6d6c 2920 6973 2061 6e6f 7468 6572  html) is another
-000003e0: 206f 7065 6e2d 736f 7572 6365 2066 7261   open-source fra
-000003f0: 6d65 776f 726b 2066 6f72 2062 7569 6c64  mework for build
-00000400: 696e 6720 6170 706c 6963 6174 696f 6e73  ing applications
-00000410: 2070 6f77 6572 6564 2062 7920 6c61 6e67   powered by lang
-00000420: 7561 6765 206d 6f64 656c 732e 200a 0a2a  uage models. ..*
-00000430: 2a6c 616e 6763 6861 696e 2d73 6572 7665  *langchain-serve
-00000440: 2a2a 2068 656c 7073 2079 6f75 2064 6570  ** helps you dep
-00000450: 6c6f 7920 796f 7572 204c 616e 6743 6861  loy your LangCha
-00000460: 696e 2061 7070 7320 6f6e 204a 696e 6120  in apps on Jina 
-00000470: 4149 2043 6c6f 7564 2069 6e20 6a75 7374  AI Cloud in just
-00000480: 2061 206d 6174 7465 7220 6f66 2073 6563   a matter of sec
-00000490: 6f6e 6473 2e20 596f 7520 6361 6e20 6e6f  onds. You can no
-000004a0: 7720 6265 6e65 6669 7420 6672 6f6d 2074  w benefit from t
-000004b0: 6865 2073 6361 6c61 6269 6c69 7479 2061  he scalability a
-000004c0: 6e64 2073 6572 7665 726c 6573 7320 6172  nd serverless ar
-000004d0: 6368 6974 6563 7475 7265 206f 6620 7468  chitecture of th
-000004e0: 6520 636c 6f75 6420 7769 7468 6f75 7420  e cloud without 
-000004f0: 7361 6372 6966 6963 696e 6720 7468 6520  sacrificing the 
-00000500: 6561 7365 2061 6e64 2063 6f6e 7665 6e69  ease and conveni
-00000510: 656e 6365 206f 6620 6c6f 6361 6c20 6465  ence of local de
-00000520: 7665 6c6f 706d 656e 742e 0a0a 0a23 2320  velopment....## 
-00000530: f09f a7a0 2042 6162 7961 6769 2d61 732d  .... Babyagi-as-
-00000540: 612d 7365 7276 6963 650a 0a3e 2047 6976  a-service..> Giv
-00000550: 6520 7573 2061 203a 7374 6172 3a20 616e  e us a :star: an
-00000560: 6420 7465 6c6c 2075 7320 7768 6174 206d  d tell us what m
-00000570: 6f72 6520 796f 7527 6420 6c69 6b65 2074  ore you'd like t
-00000580: 6f20 7365 6521 200a 0a2d 2044 6570 6c6f  o see! ..- Deplo
-00000590: 7920 6062 6162 7961 6769 6020 6f6e 204a  y `babyagi` on J
-000005a0: 696e 6120 4149 2043 6c6f 7564 2077 6974  ina AI Cloud wit
-000005b0: 6820 6f6e 6520 636f 6d6d 616e 640a 0a20  h one command.. 
-000005c0: 2060 6060 6261 7368 0a20 206c 632d 7365   ```bash.  lc-se
-000005d0: 7276 6520 6465 706c 6f79 2062 6162 7961  rve deploy babya
-000005e0: 6769 0a20 2060 6060 0a0a 2d20 496e 7465  gi.  ```..- Inte
-000005f0: 6772 6174 6520 6261 6279 6167 6920 7769  grate babyagi wi
-00000600: 7468 2065 7874 6572 6e61 6c20 7365 7276  th external serv
-00000610: 6963 6573 2075 7369 6e67 206f 7572 2057  ices using our W
-00000620: 6562 736f 636b 6574 2041 5049 2e20 4765  ebsocket API. Ge
-00000630: 7420 6120 666c 6176 6f72 206f 6620 7468  t a flavor of th
-00000640: 6520 696e 7465 6772 6174 696f 6e20 6f6e  e integration on
-00000650: 2079 6f75 7220 434c 4920 7769 7468 200a   your CLI with .
-00000660: 2020 2020 0a20 2060 6060 6261 7368 0a20      .  ```bash. 
-00000670: 206c 632d 7365 7276 6520 706c 6179 6772   lc-serve playgr
-00000680: 6f75 6e64 2062 6162 7961 6769 0a20 2060  ound babyagi.  `
-00000690: 6060 0a0a 215b 4261 6279 6167 692d 6173  ``..![Babyagi-as
-000006a0: 2d61 2d73 6572 7669 6365 2050 6c61 7967  -a-service Playg
-000006b0: 726f 756e 645d 282e 6769 7468 7562 2f69  round](.github/i
-000006c0: 6d61 6765 732f 6261 6279 6167 692d 706c  mages/babyagi-pl
-000006d0: 6179 6772 6f75 6e64 2e67 6966 290a 0a0a  ayground.gif)...
-000006e0: 2323 2323 20f0 9f8e 8920 4375 7374 6f6d  #### .... Custom
-000006f0: 2041 7070 7320 746f 2070 726f 6475 6374   Apps to product
-00000700: 696f 6e20 696e 2034 2073 696d 706c 6520  ion in 4 simple 
-00000710: 7374 6570 730a 0a20 2031 2e20 5265 6661  steps..  1. Refa
-00000720: 6374 6f72 2079 6f75 7220 636f 6465 2074  ctor your code t
-00000730: 6f20 6675 6e63 7469 6f6e 2873 2920 7468  o function(s) th
-00000740: 6174 2073 686f 756c 6420 6265 2073 6572  at should be ser
-00000750: 7665 6420 7769 7468 2060 4073 6572 7669  ved with `@servi
-00000760: 6e67 6020 6465 636f 7261 746f 722e 0a20  ng` decorator.. 
-00000770: 2031 2e20 4372 6561 7465 2061 2060 7265   1. Create a `re
-00000780: 7175 6972 656d 656e 7473 2e74 7874 6020  quirements.txt` 
-00000790: 6669 6c65 2069 6e20 796f 7572 2061 7070  file in your app
-000007a0: 2064 6972 6563 746f 7279 2074 6f20 656e   directory to en
-000007b0: 7375 7265 2061 6c6c 206e 6563 6573 7361  sure all necessa
-000007c0: 7279 2064 6570 656e 6465 6e63 6965 7320  ry dependencies 
-000007d0: 6172 6520 696e 7374 616c 6c65 642e 0a20  are installed.. 
-000007e0: 2031 2e20 5275 6e20 606c 632d 7365 7276   1. Run `lc-serv
-000007f0: 6520 6465 706c 6f79 206c 6f63 616c 2061  e deploy local a
-00000800: 7070 6020 746f 2074 6573 7420 796f 7572  pp` to test your
-00000810: 2041 5049 206c 6f63 616c 6c79 2e0a 2020   API locally..  
-00000820: 312e 2052 756e 2060 6c63 2d73 6572 7665  1. Run `lc-serve
-00000830: 2064 6570 6c6f 7920 6a63 6c6f 7564 2061   deploy jcloud a
-00000840: 7070 6020 746f 2064 6570 6c6f 7920 6f6e  pp` to deploy on
-00000850: 205b 4a69 6e61 2041 4920 436c 6f75 645d   [Jina AI Cloud]
-00000860: 2868 7474 7073 3a2f 2f6a 696e 612e 6169  (https://jina.ai
-00000870: 2f70 726f 6475 6374 2f63 6c6f 7564 2f29  /product/cloud/)
-00000880: 2e0a 0a0a 2323 2323 20f0 9f94 a520 5363  ....#### .... Sc
-00000890: 616c 6162 6c65 2c20 5365 7276 6572 6c65  alable, Serverle
-000008a0: 7373 2052 4553 5466 756c 2f53 7472 6561  ss RESTful/Strea
-000008b0: 6d69 6e67 2057 6562 736f 636b 6574 2041  ming Websocket A
-000008c0: 5049 7320 6f6e 204a 696e 6120 4149 2043  PIs on Jina AI C
-000008d0: 6c6f 7564 0a0a 2020 2d20 f09f 8c8e 2052  loud..  - .... R
-000008e0: 4553 5466 756c 2f57 6562 736f 636b 6574  ESTful/Websocket
-000008f0: 2041 5049 7320 7769 7468 2054 4c53 2063   APIs with TLS c
-00000900: 6572 7473 2069 6e20 6a75 7374 2032 206c  erts in just 2 l
-00000910: 696e 6573 206f 6620 636f 6465 2063 6861  ines of code cha
-00000920: 6e67 652e 0a20 202d 20f0 9f8c 8a20 5374  nge..  - .... St
-00000930: 7265 616d 204c 4c4d 2069 6e74 6572 6163  ream LLM interac
-00000940: 7469 6f6e 7320 696e 2072 6561 6c2d 7469  tions in real-ti
-00000950: 6d65 2077 6974 6820 5765 6273 6f63 6b65  me with Websocke
-00000960: 7473 2e0a 2020 2d20 f09f 91a5 2045 6e61  ts..  - .... Ena
-00000970: 626c 6520 6875 6d61 6e20 696e 2074 6865  ble human in the
-00000980: 206c 6f6f 7020 666f 7220 796f 7572 2061   loop for your a
-00000990: 6765 6e74 732e 0a20 202d 20f0 9f93 8420  gents..  - .... 
-000009a0: 5377 6167 6765 7220 5549 2c20 616e 6420  Swagger UI, and 
-000009b0: 4f70 656e 4150 4920 7370 6563 2069 6e63  OpenAPI spec inc
-000009c0: 6c75 6465 6420 7769 7468 2079 6f75 7220  luded with your 
-000009d0: 4150 4973 2e0a 2020 2d20 e29a a1ef b88f  APIs..  - ......
-000009e0: 2053 6572 7665 726c 6573 7320 6170 7073   Serverless apps
-000009f0: 2074 6861 7420 7363 616c 6573 2061 7574   that scales aut
-00000a00: 6f6d 6174 6963 616c 6c79 2077 6974 6820  omatically with 
-00000a10: 796f 7572 2074 7261 6666 6963 2e0a 2020  your traffic..  
-00000a20: 2d20 f09f 938a 2042 7569 6c74 696e 206c  - .... Builtin l
-00000a30: 6f67 6769 6e67 2c20 6d6f 6e69 746f 7269  ogging, monitori
-00000a40: 6e67 2c20 616e 6420 7472 6163 6573 2066  ng, and traces f
-00000a50: 6f72 2079 6f75 7220 4150 4973 2e0a 2020  or your APIs..  
-00000a60: 2d20 f09f a496 204e 6f20 6e65 6564 2074  - .... No need t
-00000a70: 6f20 6368 616e 6765 2079 6f75 7220 636f  o change your co
-00000a80: 6465 2074 6f20 6d61 6e61 6765 2041 5049  de to manage API
-00000a90: 732c 206f 7220 6d61 6e61 6765 2064 6f63  s, or manage doc
-00000aa0: 6b65 7266 696c 6573 2c20 6f72 2077 6f72  kerfiles, or wor
-00000ab0: 7279 2061 626f 7574 2069 6e66 7261 7374  ry about infrast
-00000ac0: 7275 6374 7572 6521 0a0a 0a23 2323 2320  ructure!...#### 
-00000ad0: f09f 9aa7 2043 6f6d 696e 6720 736f 6f6e  .... Coming soon
-00000ae0: 0a0a 2d20 5b20 5d20 f09f 9491 2041 7574  ..- [ ] .... Aut
-00000af0: 686f 7269 7a65 2041 5049 2065 6e64 706f  horize API endpo
-00000b00: 696e 7473 0a2d 205b 205d 20f0 9f9b a0ef  ints.- [ ] .....
-00000b10: b88f 2045 6e61 626c 6520 5374 7265 616d  .. Enable Stream
-00000b20: 6c69 7420 706c 6179 6772 6f75 6e64 2064  lit playground d
-00000b30: 6570 6c6f 796d 656e 7420 666f 7220 796f  eployment for yo
-00000b40: 7572 2061 7070 730a 0a0a 4966 2079 6f75  ur apps...If you
-00000b50: 2068 6176 6520 616e 7920 6665 6174 7572   have any featur
-00000b60: 6520 7265 7175 6573 7473 206f 7220 6661  e requests or fa
-00000b70: 6365 6420 616e 7920 6973 7375 652c 2070  ced any issue, p
-00000b80: 6c65 6173 6520 5b6c 6574 2075 7320 6b6e  lease [let us kn
-00000b90: 6f77 5d28 6874 7470 733a 2f2f 6769 7468  ow](https://gith
-00000ba0: 7562 2e63 6f6d 2f6a 696e 612d 6169 2f6c  ub.com/jina-ai/l
-00000bb0: 616e 6763 6861 696e 2d73 6572 7665 2f69  angchain-serve/i
-00000bc0: 7373 7565 732f 6e65 7729 210a 0a0a 2323  ssues/new)!...##
-00000bd0: 2055 7361 6765 0a0a 4c65 7427 7320 6669   Usage..Let's fi
-00000be0: 7273 7420 696e 7374 616c 6c20 606c 616e  rst install `lan
-00000bf0: 6763 6861 696e 2d73 6572 7665 6020 7573  gchain-serve` us
-00000c00: 696e 6720 7069 702e 0a0a 6060 6062 6173  ing pip...```bas
-00000c10: 680a 7069 7020 696e 7374 616c 6c20 6c61  h.pip install la
-00000c20: 6e67 6368 6169 6e2d 7365 7276 650a 6060  ngchain-serve.``
-00000c30: 600a 0a23 2320 456e 6162 6c65 2048 756d  `..## Enable Hum
-00000c40: 616e 2d69 6e2d 7468 652d 6c6f 6f70 2028  an-in-the-loop (
-00000c50: 4849 544c 2920 666f 7220 796f 7572 2061  HITL) for your a
-00000c60: 6765 6e74 730a 0a48 4954 4c20 666f 7220  gents..HITL for 
-00000c70: 4c61 6e67 4368 6169 6e20 6167 656e 7473  LangChain agents
-00000c80: 206f 6e20 7072 6f64 7563 7469 6f6e 2063   on production c
-00000c90: 616e 2062 6520 6368 616c 6c65 6e67 696e  an be challengin
-00000ca0: 6720 7369 6e63 6520 7468 6520 6167 656e  g since the agen
-00000cb0: 7473 2061 7265 2074 7970 6963 616c 6c79  ts are typically
-00000cc0: 2072 756e 6e69 6e67 206f 6e20 7365 7276   running on serv
-00000cd0: 6572 7320 7768 6572 6520 6875 6d61 6e73  ers where humans
-00000ce0: 2064 6f6e 2774 2068 6176 6520 6469 7265   don't have dire
-00000cf0: 6374 2061 6363 6573 732e 202a 2a6c 616e  ct access. **lan
-00000d00: 6763 6861 696e 2d73 6572 7665 2a2a 2062  gchain-serve** b
-00000d10: 7269 6467 6573 2074 6869 7320 6761 7020  ridges this gap 
-00000d20: 6279 2065 6e61 626c 696e 6720 7765 6273  by enabling webs
-00000d30: 6f63 6b65 7420 4150 4973 2074 6861 7420  ocket APIs that 
-00000d40: 616c 6c6f 7720 666f 7220 7265 616c 2d74  allow for real-t
-00000d50: 696d 6520 696e 7465 7261 6374 696f 6e20  ime interaction 
-00000d60: 616e 6420 6665 6564 6261 636b 2062 6574  and feedback bet
-00000d70: 7765 656e 2074 6865 2061 6765 6e74 2061  ween the agent a
-00000d80: 6e64 2061 2068 756d 616e 206f 7065 7261  nd a human opera
-00000d90: 746f 722e 0a0a 4368 6563 6b20 6f75 7420  tor...Check out 
-00000da0: 7468 6973 205b 6578 616d 706c 655d 2865  this [example](e
-00000db0: 7861 6d70 6c65 732f 7765 6273 6f63 6b65  xamples/websocke
-00000dc0: 7473 2f68 6974 6c2f 5245 4144 4d45 2e6d  ts/hitl/README.m
-00000dd0: 6429 2074 6f20 7365 6520 686f 7720 796f  d) to see how yo
-00000de0: 7520 6361 6e20 656e 6162 6c65 2048 4954  u can enable HIT
-00000df0: 4c20 666f 7220 796f 7572 2061 6765 6e74  L for your agent
-00000e00: 732e 0a0a 0a23 2320 456e 6162 6c65 2052  s....## Enable R
-00000e10: 4553 5420 4150 4973 200a 0a0a 4c65 7427  EST APIs ...Let'
-00000e20: 7320 6275 696c 6420 6120 6375 7374 6f6d  s build a custom
-00000e30: 2061 6765 6e74 2075 7369 6e67 2074 6869   agent using thi
-00000e40: 7320 6578 616d 706c 6520 7461 6b65 6e20  s example taken 
-00000e50: 6672 6f6d 205b 4c61 6e67 4368 6169 6e20  from [LangChain 
-00000e60: 646f 6375 6d65 6e74 6174 696f 6e5d 2868  documentation](h
-00000e70: 7474 7073 3a2f 2f70 7974 686f 6e2e 6c61  ttps://python.la
-00000e80: 6e67 6368 6169 6e2e 636f 6d2f 656e 2f6c  ngchain.com/en/l
-00000e90: 6174 6573 742f 6d6f 6475 6c65 732f 6167  atest/modules/ag
-00000ea0: 656e 7473 2f61 6765 6e74 732f 6375 7374  ents/agents/cust
-00000eb0: 6f6d 5f61 6765 6e74 2e68 746d 6c29 2e20  om_agent.html). 
-00000ec0: 0a0a 0a3c 6465 7461 696c 733e 0a3c 7375  ...<details>.<su
-00000ed0: 6d6d 6172 793e 5368 6f77 2061 6765 6e74  mmary>Show agent
-00000ee0: 2063 6f64 6520 2861 7070 2e70 7929 3c2f   code (app.py)</
-00000ef0: 7375 6d6d 6172 793e 0a0a 6060 6070 7974  summary>..```pyt
-00000f00: 686f 6e0a 2320 6170 702e 7079 0a66 726f  hon.# app.py.fro
-00000f10: 6d20 6c61 6e67 6368 6169 6e2e 6167 656e  m langchain.agen
-00000f20: 7473 2069 6d70 6f72 7420 5a65 726f 5368  ts import ZeroSh
-00000f30: 6f74 4167 656e 742c 2054 6f6f 6c2c 2041  otAgent, Tool, A
-00000f40: 6765 6e74 4578 6563 7574 6f72 0a66 726f  gentExecutor.fro
-00000f50: 6d20 6c61 6e67 6368 6169 6e20 696d 706f  m langchain impo
-00000f60: 7274 204f 7065 6e41 492c 2053 6572 7041  rt OpenAI, SerpA
-00000f70: 5049 5772 6170 7065 722c 204c 4c4d 4368  PIWrapper, LLMCh
-00000f80: 6169 6e0a 0a73 6561 7263 6820 3d20 5365  ain..search = Se
-00000f90: 7270 4150 4957 7261 7070 6572 2829 0a74  rpAPIWrapper().t
-00000fa0: 6f6f 6c73 203d 205b 0a20 2020 2054 6f6f  ools = [.    Too
-00000fb0: 6c28 0a20 2020 2020 2020 206e 616d 6520  l(.        name 
-00000fc0: 3d20 2253 6561 7263 6822 2c0a 2020 2020  = "Search",.    
-00000fd0: 2020 2020 6675 6e63 3d73 6561 7263 682e      func=search.
-00000fe0: 7275 6e2c 0a20 2020 2020 2020 2064 6573  run,.        des
-00000ff0: 6372 6970 7469 6f6e 3d22 7573 6566 756c  cription="useful
-00001000: 2066 6f72 2077 6865 6e20 796f 7520 6e65   for when you ne
-00001010: 6564 2074 6f20 616e 7377 6572 2071 7565  ed to answer que
-00001020: 7374 696f 6e73 2061 626f 7574 2063 7572  stions about cur
-00001030: 7265 6e74 2065 7665 6e74 7322 0a20 2020  rent events".   
-00001040: 2029 0a5d 0a0a 7072 6566 6978 203d 2022   ).]..prefix = "
-00001050: 2222 416e 7377 6572 2074 6865 2066 6f6c  ""Answer the fol
-00001060: 6c6f 7769 6e67 2071 7565 7374 696f 6e73  lowing questions
-00001070: 2061 7320 6265 7374 2079 6f75 2063 616e   as best you can
-00001080: 2c20 6275 7420 7370 6561 6b69 6e67 2061  , but speaking a
-00001090: 7320 6120 7069 7261 7465 206d 6967 6874  s a pirate might
-000010a0: 2073 7065 616b 2e20 596f 7520 6861 7665   speak. You have
-000010b0: 2061 6363 6573 7320 746f 2074 6865 2066   access to the f
-000010c0: 6f6c 6c6f 7769 6e67 2074 6f6f 6c73 3a22  ollowing tools:"
-000010d0: 2222 0a73 7566 6669 7820 3d20 2222 2242  "".suffix = """B
-000010e0: 6567 696e 2120 5265 6d65 6d62 6572 2074  egin! Remember t
-000010f0: 6f20 7370 6561 6b20 6173 2061 2070 6972  o speak as a pir
-00001100: 6174 6520 7768 656e 2067 6976 696e 6720  ate when giving 
-00001110: 796f 7572 2066 696e 616c 2061 6e73 7765  your final answe
-00001120: 722e 2055 7365 206c 6f74 7320 6f66 2022  r. Use lots of "
-00001130: 4172 6773 220a 0a51 7565 7374 696f 6e3a  Args"..Question:
-00001140: 207b 696e 7075 747d 0a7b 6167 656e 745f   {input}.{agent_
-00001150: 7363 7261 7463 6870 6164 7d22 2222 0a0a  scratchpad}"""..
-00001160: 7072 6f6d 7074 203d 205a 6572 6f53 686f  prompt = ZeroSho
-00001170: 7441 6765 6e74 2e63 7265 6174 655f 7072  tAgent.create_pr
-00001180: 6f6d 7074 280a 2020 2020 746f 6f6c 732c  ompt(.    tools,
-00001190: 200a 2020 2020 7072 6566 6978 3d70 7265   .    prefix=pre
-000011a0: 6669 782c 200a 2020 2020 7375 6666 6978  fix, .    suffix
-000011b0: 3d73 7566 6669 782c 200a 2020 2020 696e  =suffix, .    in
-000011c0: 7075 745f 7661 7269 6162 6c65 733d 5b22  put_variables=["
-000011d0: 696e 7075 7422 2c20 2261 6765 6e74 5f73  input", "agent_s
-000011e0: 6372 6174 6368 7061 6422 5d0a 290a 0a6c  cratchpad"].)..l
-000011f0: 6c6d 5f63 6861 696e 203d 204c 4c4d 4368  lm_chain = LLMCh
-00001200: 6169 6e28 6c6c 6d3d 4f70 656e 4149 2874  ain(llm=OpenAI(t
-00001210: 656d 7065 7261 7475 7265 3d30 292c 2070  emperature=0), p
-00001220: 726f 6d70 743d 7072 6f6d 7074 290a 746f  rompt=prompt).to
-00001230: 6f6c 5f6e 616d 6573 203d 205b 746f 6f6c  ol_names = [tool
-00001240: 2e6e 616d 6520 666f 7220 746f 6f6c 2069  .name for tool i
-00001250: 6e20 746f 6f6c 735d 0a61 6765 6e74 203d  n tools].agent =
-00001260: 205a 6572 6f53 686f 7441 6765 6e74 286c   ZeroShotAgent(l
-00001270: 6c6d 5f63 6861 696e 3d6c 6c6d 5f63 6861  lm_chain=llm_cha
-00001280: 696e 2c20 616c 6c6f 7765 645f 746f 6f6c  in, allowed_tool
-00001290: 733d 746f 6f6c 5f6e 616d 6573 290a 6167  s=tool_names).ag
-000012a0: 656e 745f 6578 6563 7574 6f72 203d 2041  ent_executor = A
-000012b0: 6765 6e74 4578 6563 7574 6f72 2e66 726f  gentExecutor.fro
-000012c0: 6d5f 6167 656e 745f 616e 645f 746f 6f6c  m_agent_and_tool
-000012d0: 7328 6167 656e 743d 6167 656e 742c 2074  s(agent=agent, t
-000012e0: 6f6f 6c73 3d74 6f6f 6c73 2c20 7665 7262  ools=tools, verb
-000012f0: 6f73 653d 5472 7565 290a 6167 656e 745f  ose=True).agent_
-00001300: 6578 6563 7574 6f72 2e72 756e 2822 486f  executor.run("Ho
-00001310: 7720 6d61 6e79 2070 656f 706c 6520 6c69  w many people li
-00001320: 7665 2069 6e20 6361 6e61 6461 2061 7320  ve in canada as 
-00001330: 6f66 2032 3032 333f 2229 0a60 6060 0a0a  of 2023?").```..
-00001340: 2323 2323 204f 7574 7075 740a 0a0a 6060  #### Output...``
-00001350: 6074 6578 740a 3e20 456e 7465 7269 6e67  `text.> Entering
-00001360: 206e 6577 2041 6765 6e74 4578 6563 7574   new AgentExecut
-00001370: 6f72 2063 6861 696e 2e2e 2e0a 5468 6f75  or chain....Thou
-00001380: 6768 743a 2049 206e 6565 6420 746f 2066  ght: I need to f
-00001390: 696e 6420 6f75 7420 7468 6520 706f 7075  ind out the popu
-000013a0: 6c61 7469 6f6e 206f 6620 4361 6e61 6461  lation of Canada
-000013b0: 0a41 6374 696f 6e3a 2053 6561 7263 680a  .Action: Search.
-000013c0: 4163 7469 6f6e 2049 6e70 7574 3a20 506f  Action Input: Po
-000013d0: 7075 6c61 7469 6f6e 206f 6620 4361 6e61  pulation of Cana
-000013e0: 6461 2032 3032 330a 4f62 7365 7276 6174  da 2023.Observat
-000013f0: 696f 6e3a 2054 6865 2063 7572 7265 6e74  ion: The current
-00001400: 2070 6f70 756c 6174 696f 6e20 6f66 2043   population of C
-00001410: 616e 6164 6120 6973 2033 382c 3631 302c  anada is 38,610,
-00001420: 3434 3720 6173 206f 6620 5361 7475 7264  447 as of Saturd
-00001430: 6179 2c20 4665 6272 7561 7279 2031 382c  ay, February 18,
-00001440: 2032 3032 332c 2062 6173 6564 206f 6e20   2023, based on 
-00001450: 576f 726c 646f 6d65 7465 7220 656c 6162  Worldometer elab
-00001460: 6f72 6174 696f 6e20 6f66 2074 6865 206c  oration of the l
-00001470: 6174 6573 7420 556e 6974 6564 204e 6174  atest United Nat
-00001480: 696f 6e73 2064 6174 612e 2043 616e 6164  ions data. Canad
-00001490: 6120 3230 3230 2070 6f70 756c 6174 696f  a 2020 populatio
-000014a0: 6e20 6973 2065 7374 696d 6174 6564 2061  n is estimated a
-000014b0: 7420 3337 2c37 3432 2c31 3534 2070 656f  t 37,742,154 peo
-000014c0: 706c 6520 6174 206d 6964 2079 6561 7220  ple at mid year 
-000014d0: 6163 636f 7264 696e 6720 746f 2055 4e20  according to UN 
-000014e0: 6461 7461 2e0a 5468 6f75 6768 743a 2049  data..Thought: I
-000014f0: 206e 6f77 206b 6e6f 7720 7468 6520 6669   now know the fi
-00001500: 6e61 6c20 616e 7377 6572 0a46 696e 616c  nal answer.Final
-00001510: 2041 6e73 7765 723a 2041 7272 722c 2043   Answer: Arrr, C
-00001520: 616e 6164 6120 6265 2068 6176 696e 2720  anada be havin' 
-00001530: 3338 2c36 3130 2c34 3437 2073 6361 6c6c  38,610,447 scall
-00001540: 7977 6167 7320 6c69 7669 6e27 2074 6865  ywags livin' the
-00001550: 7265 2061 7320 6f66 2032 3032 3321 0a0a  re as of 2023!..
-00001560: 3e20 4669 6e69 7368 6564 2063 6861 696e  > Finished chain
-00001570: 2e0a 6060 600a 0a3c 2f64 6574 6169 6c73  ..```..</details
-00001580: 3e0a 0a23 2323 2053 7465 7020 313a 200a  >..### Step 1: .
-00001590: 0a2a 2a52 6566 6163 746f 7220 796f 7572  .**Refactor your
-000015a0: 2063 6f64 6520 746f 2066 756e 6374 696f   code to functio
-000015b0: 6e28 7329 2074 6861 7420 7368 6f75 6c64  n(s) that should
-000015c0: 2062 6520 7365 7276 6564 2077 6974 6820   be served with 
-000015d0: 6040 7365 7276 696e 6760 2064 6563 6f72  `@serving` decor
-000015e0: 6174 6f72 2a2a 0a0a 0a3c 6465 7461 696c  ator**...<detail
-000015f0: 733e 0a3c 7375 6d6d 6172 793e 5368 6f77  s>.<summary>Show
-00001600: 2075 7064 6174 6564 2061 6765 6e74 2063   updated agent c
-00001610: 6f64 6520 2861 7070 2e70 7929 3c2f 7375  ode (app.py)</su
-00001620: 6d6d 6172 793e 0a0a 6060 6070 7974 686f  mmary>..```pytho
-00001630: 6e0a 2320 6170 702e 7079 0a66 726f 6d20  n.# app.py.from 
-00001640: 6c61 6e67 6368 6169 6e20 696d 706f 7274  langchain import
-00001650: 204c 4c4d 4368 6169 6e2c 204f 7065 6e41   LLMChain, OpenA
-00001660: 492c 2053 6572 7041 5049 5772 6170 7065  I, SerpAPIWrappe
-00001670: 720a 6672 6f6d 206c 616e 6763 6861 696e  r.from langchain
-00001680: 2e61 6765 6e74 7320 696d 706f 7274 2041  .agents import A
-00001690: 6765 6e74 4578 6563 7574 6f72 2c20 546f  gentExecutor, To
-000016a0: 6f6c 2c20 5a65 726f 5368 6f74 4167 656e  ol, ZeroShotAgen
-000016b0: 740a 0a66 726f 6d20 6c63 7365 7276 6520  t..from lcserve 
-000016c0: 696d 706f 7274 2073 6572 7669 6e67 0a0a  import serving..
-000016d0: 0a40 7365 7276 696e 670a 6465 6620 6173  .@serving.def as
-000016e0: 6b28 696e 7075 743a 2073 7472 2920 2d3e  k(input: str) ->
-000016f0: 2073 7472 3a0a 2020 2020 7365 6172 6368   str:.    search
-00001700: 203d 2053 6572 7041 5049 5772 6170 7065   = SerpAPIWrappe
-00001710: 7228 290a 2020 2020 746f 6f6c 7320 3d20  r().    tools = 
-00001720: 5b0a 2020 2020 2020 2020 546f 6f6c 280a  [.        Tool(.
-00001730: 2020 2020 2020 2020 2020 2020 6e61 6d65              name
-00001740: 3d22 5365 6172 6368 222c 0a20 2020 2020  ="Search",.     
-00001750: 2020 2020 2020 2066 756e 633d 7365 6172         func=sear
-00001760: 6368 2e72 756e 2c0a 2020 2020 2020 2020  ch.run,.        
-00001770: 2020 2020 6465 7363 7269 7074 696f 6e3d      description=
-00001780: 2275 7365 6675 6c20 666f 7220 7768 656e  "useful for when
-00001790: 2079 6f75 206e 6565 6420 746f 2061 6e73   you need to ans
-000017a0: 7765 7220 7175 6573 7469 6f6e 7320 6162  wer questions ab
-000017b0: 6f75 7420 6375 7272 656e 7420 6576 656e  out current even
-000017c0: 7473 222c 0a20 2020 2020 2020 2029 0a20  ts",.        ). 
-000017d0: 2020 205d 0a20 2020 2070 7265 6669 7820     ].    prefix 
-000017e0: 3d20 2222 2241 6e73 7765 7220 7468 6520  = """Answer the 
-000017f0: 666f 6c6c 6f77 696e 6720 7175 6573 7469  following questi
-00001800: 6f6e 7320 6173 2062 6573 7420 796f 7520  ons as best you 
-00001810: 6361 6e2c 2062 7574 2073 7065 616b 696e  can, but speakin
-00001820: 6720 6173 2061 2070 6972 6174 6520 6d69  g as a pirate mi
-00001830: 6768 7420 7370 6561 6b2e 2059 6f75 2068  ght speak. You h
-00001840: 6176 6520 6163 6365 7373 2074 6f20 7468  ave access to th
-00001850: 6520 666f 6c6c 6f77 696e 6720 746f 6f6c  e following tool
-00001860: 733a 2222 220a 2020 2020 7375 6666 6978  s:""".    suffix
-00001870: 203d 2022 2222 4265 6769 6e21 2052 656d   = """Begin! Rem
-00001880: 656d 6265 7220 746f 2073 7065 616b 2061  ember to speak a
-00001890: 7320 6120 7069 7261 7465 2077 6865 6e20  s a pirate when 
-000018a0: 6769 7669 6e67 2079 6f75 7220 6669 6e61  giving your fina
-000018b0: 6c20 616e 7377 6572 2e20 5573 6520 6c6f  l answer. Use lo
-000018c0: 7473 206f 6620 2241 7267 7322 0a0a 2020  ts of "Args"..  
-000018d0: 2020 5175 6573 7469 6f6e 3a20 7b69 6e70    Question: {inp
-000018e0: 7574 7d0a 2020 2020 7b61 6765 6e74 5f73  ut}.    {agent_s
-000018f0: 6372 6174 6368 7061 647d 2222 220a 0a20  cratchpad}""".. 
-00001900: 2020 2070 726f 6d70 7420 3d20 5a65 726f     prompt = Zero
-00001910: 5368 6f74 4167 656e 742e 6372 6561 7465  ShotAgent.create
-00001920: 5f70 726f 6d70 7428 0a20 2020 2020 2020  _prompt(.       
-00001930: 2074 6f6f 6c73 2c0a 2020 2020 2020 2020   tools,.        
-00001940: 7072 6566 6978 3d70 7265 6669 782c 0a20  prefix=prefix,. 
-00001950: 2020 2020 2020 2073 7566 6669 783d 7375         suffix=su
-00001960: 6666 6978 2c0a 2020 2020 2020 2020 696e  ffix,.        in
-00001970: 7075 745f 7661 7269 6162 6c65 733d 5b22  put_variables=["
-00001980: 696e 7075 7422 2c20 2261 6765 6e74 5f73  input", "agent_s
-00001990: 6372 6174 6368 7061 6422 5d2c 0a20 2020  cratchpad"],.   
-000019a0: 2029 0a0a 2020 2020 7072 696e 7428 7072   )..    print(pr
-000019b0: 6f6d 7074 2e74 656d 706c 6174 6529 0a0a  ompt.template)..
-000019c0: 2020 2020 6c6c 6d5f 6368 6169 6e20 3d20      llm_chain = 
-000019d0: 4c4c 4d43 6861 696e 286c 6c6d 3d4f 7065  LLMChain(llm=Ope
-000019e0: 6e41 4928 7465 6d70 6572 6174 7572 653d  nAI(temperature=
-000019f0: 3029 2c20 7072 6f6d 7074 3d70 726f 6d70  0), prompt=promp
-00001a00: 7429 0a20 2020 2074 6f6f 6c5f 6e61 6d65  t).    tool_name
-00001a10: 7320 3d20 5b74 6f6f 6c2e 6e61 6d65 2066  s = [tool.name f
-00001a20: 6f72 2074 6f6f 6c20 696e 2074 6f6f 6c73  or tool in tools
-00001a30: 5d0a 2020 2020 6167 656e 7420 3d20 5a65  ].    agent = Ze
-00001a40: 726f 5368 6f74 4167 656e 7428 6c6c 6d5f  roShotAgent(llm_
-00001a50: 6368 6169 6e3d 6c6c 6d5f 6368 6169 6e2c  chain=llm_chain,
-00001a60: 2061 6c6c 6f77 6564 5f74 6f6f 6c73 3d74   allowed_tools=t
-00001a70: 6f6f 6c5f 6e61 6d65 7329 0a0a 2020 2020  ool_names)..    
-00001a80: 6167 656e 745f 6578 6563 7574 6f72 203d  agent_executor =
-00001a90: 2041 6765 6e74 4578 6563 7574 6f72 2e66   AgentExecutor.f
-00001aa0: 726f 6d5f 6167 656e 745f 616e 645f 746f  rom_agent_and_to
-00001ab0: 6f6c 7328 0a20 2020 2020 2020 2061 6765  ols(.        age
-00001ac0: 6e74 3d61 6765 6e74 2c20 746f 6f6c 733d  nt=agent, tools=
-00001ad0: 746f 6f6c 732c 2076 6572 626f 7365 3d54  tools, verbose=T
-00001ae0: 7275 650a 2020 2020 290a 0a20 2020 2072  rue.    )..    r
-00001af0: 6574 7572 6e20 6167 656e 745f 6578 6563  eturn agent_exec
-00001b00: 7574 6f72 2e72 756e 2869 6e70 7574 290a  utor.run(input).
-00001b10: 0a69 6620 5f5f 6e61 6d65 5f5f 203d 3d20  .if __name__ == 
-00001b20: 225f 5f6d 6169 6e5f 5f22 3a0a 2020 2020  "__main__":.    
-00001b30: 6173 6b28 2748 6f77 206d 616e 7920 7065  ask('How many pe
-00001b40: 6f70 6c65 206c 6976 6520 696e 2063 616e  ople live in can
-00001b50: 6164 6120 6173 206f 6620 3230 3233 3f27  ada as of 2023?'
-00001b60: 290a 6060 600a 0a3c 2f64 6574 6169 6c73  ).```..</details
-00001b70: 3e0a 0a0a 2323 2323 2320 5768 6174 2063  >...##### What c
-00001b80: 6861 6e67 6564 3f0a 0a2d 2057 6520 6d6f  hanged?..- We mo
-00001b90: 7665 6420 6f75 7220 636f 6465 2074 6f20  ved our code to 
-00001ba0: 616e 2060 6173 6b60 2066 756e 6374 696f  an `ask` functio
-00001bb0: 6e2e 0a2d 2041 6464 6564 2074 7970 6520  n..- Added type 
-00001bc0: 6869 6e74 7320 746f 2074 6865 2066 756e  hints to the fun
-00001bd0: 6374 696f 6e20 7061 7261 6d65 7465 7273  ction parameters
-00001be0: 2028 696e 7075 7420 616e 6420 6f75 7470   (input and outp
-00001bf0: 7574 292c 2073 6f20 4150 4920 6465 6669  ut), so API defi
-00001c00: 6e69 7469 6f6e 2063 616e 2062 6520 6765  nition can be ge
-00001c10: 6e65 7261 7465 642e 0a2d 2049 6d70 6f72  nerated..- Impor
-00001c20: 7465 6420 6066 726f 6d20 6c63 7365 7276  ted `from lcserv
-00001c30: 6520 696d 706f 7274 2073 6572 7669 6e67  e import serving
-00001c40: 6020 616e 6420 6164 6465 6420 6040 7365  ` and added `@se
-00001c50: 7276 696e 6760 2064 6563 6f72 6174 6f72  rving` decorator
-00001c60: 2074 6f20 7468 6520 6061 736b 6020 6675   to the `ask` fu
-00001c70: 6e63 7469 6f6e 2e0a 2d20 4164 6465 6420  nction..- Added 
-00001c80: 6069 6620 5f5f 6e61 6d65 5f5f 203d 3d20  `if __name__ == 
-00001c90: 225f 5f6d 6169 6e5f 5f22 3a60 2062 6c6f  "__main__":` blo
-00001ca0: 636b 2074 6f20 7465 7374 2074 6865 2066  ck to test the f
-00001cb0: 756e 6374 696f 6e20 6c6f 6361 6c6c 792e  unction locally.
-00001cc0: 0a0a 2d2d 2d0a 0a23 2323 2053 7465 7020  ..---..### Step 
-00001cd0: 323a 0a0a 2a2a 4372 6561 7465 2061 2060  2:..**Create a `
-00001ce0: 7265 7175 6972 656d 656e 7473 2e74 7874  requirements.txt
-00001cf0: 6020 6669 6c65 2069 6e20 796f 7572 2061  ` file in your a
-00001d00: 7070 2064 6972 6563 746f 7279 2074 6f20  pp directory to 
-00001d10: 656e 7375 7265 2061 6c6c 206e 6563 6573  ensure all neces
-00001d20: 7361 7279 2064 6570 656e 6465 6e63 6965  sary dependencie
-00001d30: 7320 6172 6520 696e 7374 616c 6c65 642e  s are installed.
-00001d40: 2a2a 0a0a 3c64 6574 6169 6c73 3e0a 3c73  **..<details>.<s
-00001d50: 756d 6d61 7279 3e53 686f 7720 7265 7175  ummary>Show requ
-00001d60: 6972 656d 656e 7473 2e74 7874 3c2f 7375  irements.txt</su
-00001d70: 6d6d 6172 793e 0a0a 6060 6074 6578 740a  mmary>..```text.
-00001d80: 2320 7265 7175 6972 656d 656e 7473 2e74  # requirements.t
-00001d90: 7874 0a6f 7065 6e61 690a 676f 6f67 6c65  xt.openai.google
-00001da0: 2d73 6561 7263 682d 7265 7375 6c74 730a  -search-results.
-00001db0: 6060 600a 3c2f 6465 7461 696c 733e 0a0a  ```.</details>..
-00001dc0: 2d2d 2d20 0a0a 2323 2320 5374 6570 2033  --- ..### Step 3
-00001dd0: 3a0a 0a2a 2a52 756e 2060 6c63 2d73 6572  :..**Run `lc-ser
-00001de0: 7665 2064 6570 6c6f 7920 6c6f 6361 6c20  ve deploy local 
-00001df0: 6170 7060 2074 6f20 7465 7374 2079 6f75  app` to test you
-00001e00: 7220 4150 4920 6c6f 6361 6c6c 792e 2a2a  r API locally.**
-00001e10: 0a0a 3e20 6061 7070 6020 6973 2074 6865  ..> `app` is the
-00001e20: 206e 616d 6520 6f66 2074 6865 206d 6f64   name of the mod
-00001e30: 756c 6520 7468 6174 2063 6f6e 7461 696e  ule that contain
-00001e40: 7320 7468 6520 6061 736b 6020 6675 6e63  s the `ask` func
-00001e50: 7469 6f6e 2e0a 0a60 6060 6261 7368 0a6c  tion...```bash.l
-00001e60: 632d 7365 7276 6520 6465 706c 6f79 206c  c-serve deploy l
-00001e70: 6f63 616c 2061 7070 0a60 6060 0a0a 3c64  ocal app.```..<d
-00001e80: 6574 6169 6c73 3e0a 3c73 756d 6d61 7279  etails>.<summary
-00001e90: 3e53 686f 7720 6f75 7470 7574 3c2f 7375  >Show output</su
-00001ea0: 6d6d 6172 793e 0a0a 6060 6074 6578 740a  mmary>..```text.
-00001eb0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00001ec0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001ed0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00001ee0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00001ef0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001f00: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00001f10: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00001f20: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001f30: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00001f40: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00001f50: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001f60: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00001f70: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00001f80: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001f90: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00001fa0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00001fb0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001fc0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00001fd0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00001fe0: 9480 20f0 9f8e 8920 466c 6f77 2069 7320  .. .... Flow is 
-00001ff0: 7265 6164 7920 746f 2073 6572 7665 2120  ready to serve! 
-00002000: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002010: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00000000: 2320 4c61 6e67 4368 6169 6e20 4170 7073  # LangChain Apps
+00000010: 206f 6e20 5072 6f64 7563 7469 6f6e 2077   on Production w
+00000020: 6974 6820 4a69 6e61 20f0 9f9a 800a 0a5b  ith Jina ......[
+00000030: 4a69 6e61 5d28 6874 7470 733a 2f2f 6769  Jina](https://gi
+00000040: 7468 7562 2e63 6f6d 2f6a 696e 612d 6169  thub.com/jina-ai
+00000050: 2f6a 696e 6129 2069 7320 616e 206f 7065  /jina) is an ope
+00000060: 6e2d 736f 7572 6365 2066 7261 6d65 776f  n-source framewo
+00000070: 726b 2074 6f20 6275 696c 642c 2064 6570  rk to build, dep
+00000080: 6c6f 7920 2620 6d61 6e61 6765 206d 6163  loy & manage mac
+00000090: 6869 6e65 206c 6561 726e 696e 6720 6170  hine learning ap
+000000a0: 706c 6963 6174 696f 6e73 2061 7420 7363  plications at sc
+000000b0: 616c 652e 205b 4c61 6e67 4368 6169 6e5d  ale. [LangChain]
+000000c0: 2868 7474 7073 3a2f 2f70 7974 686f 6e2e  (https://python.
+000000d0: 6c61 6e67 6368 6169 6e2e 636f 6d2f 656e  langchain.com/en
+000000e0: 2f6c 6174 6573 742f 696e 6465 782e 6874  /latest/index.ht
+000000f0: 6d6c 2920 6973 2061 6e6f 7468 6572 206f  ml) is another o
+00000100: 7065 6e2d 736f 7572 6365 2066 7261 6d65  pen-source frame
+00000110: 776f 726b 2066 6f72 2062 7569 6c64 696e  work for buildin
+00000120: 6720 6170 706c 6963 6174 696f 6e73 2070  g applications p
+00000130: 6f77 6572 6564 2062 7920 6c61 6e67 7561  owered by langua
+00000140: 6765 206d 6f64 656c 732e 200a 0a2a 2a6c  ge models. ..**l
+00000150: 616e 6763 6861 696e 2d73 6572 7665 2a2a  angchain-serve**
+00000160: 2068 656c 7073 2079 6f75 2064 6570 6c6f   helps you deplo
+00000170: 7920 796f 7572 204c 616e 6743 6861 696e  y your LangChain
+00000180: 2061 7070 7320 6f6e 204a 696e 6120 4149   apps on Jina AI
+00000190: 2043 6c6f 7564 2069 6e20 6a75 7374 2061   Cloud in just a
+000001a0: 206d 6174 7465 7220 6f66 2073 6563 6f6e   matter of secon
+000001b0: 6473 2e20 596f 7520 6361 6e20 6e6f 7720  ds. You can now 
+000001c0: 6265 6e65 6669 7420 6672 6f6d 2074 6865  benefit from the
+000001d0: 2073 6361 6c61 6269 6c69 7479 2061 6e64   scalability and
+000001e0: 2073 6572 7665 726c 6573 7320 6172 6368   serverless arch
+000001f0: 6974 6563 7475 7265 206f 6620 7468 6520  itecture of the 
+00000200: 636c 6f75 6420 7769 7468 6f75 7420 7361  cloud without sa
+00000210: 6372 6966 6963 696e 6720 7468 6520 6561  crificing the ea
+00000220: 7365 2061 6e64 2063 6f6e 7665 6e69 656e  se and convenien
+00000230: 6365 206f 6620 6c6f 6361 6c20 6465 7665  ce of local deve
+00000240: 6c6f 706d 656e 742e 0a0a 0a23 2320 f09f  lopment....## ..
+00000250: a7a0 2042 6162 7961 6769 2d61 732d 612d  .. Babyagi-as-a-
+00000260: 7365 7276 6963 650a 0a3e 2047 6976 6520  service..> Give 
+00000270: 7573 2061 203a 7374 6172 3a20 616e 6420  us a :star: and 
+00000280: 7465 6c6c 2075 7320 7768 6174 206d 6f72  tell us what mor
+00000290: 6520 796f 7527 6420 6c69 6b65 2074 6f20  e you'd like to 
+000002a0: 7365 6521 200a 0a2d 2044 6570 6c6f 7920  see! ..- Deploy 
+000002b0: 6062 6162 7961 6769 6020 6f6e 204a 696e  `babyagi` on Jin
+000002c0: 6120 4149 2043 6c6f 7564 2077 6974 6820  a AI Cloud with 
+000002d0: 6f6e 6520 636f 6d6d 616e 640a 0a20 2060  one command..  `
+000002e0: 6060 6261 7368 0a20 206c 632d 7365 7276  ``bash.  lc-serv
+000002f0: 6520 6465 706c 6f79 2062 6162 7961 6769  e deploy babyagi
+00000300: 0a20 2060 6060 0a0a 2d20 496e 7465 6772  .  ```..- Integr
+00000310: 6174 6520 6261 6279 6167 6920 7769 7468  ate babyagi with
+00000320: 2065 7874 6572 6e61 6c20 7365 7276 6963   external servic
+00000330: 6573 2075 7369 6e67 206f 7572 2057 6562  es using our Web
+00000340: 736f 636b 6574 2041 5049 2e20 4765 7420  socket API. Get 
+00000350: 6120 666c 6176 6f72 206f 6620 7468 6520  a flavor of the 
+00000360: 696e 7465 6772 6174 696f 6e20 6f6e 2079  integration on y
+00000370: 6f75 7220 434c 4920 7769 7468 200a 2020  our CLI with .  
+00000380: 2020 0a20 2060 6060 6261 7368 0a20 206c    .  ```bash.  l
+00000390: 632d 7365 7276 6520 706c 6179 6772 6f75  c-serve playgrou
+000003a0: 6e64 2062 6162 7961 6769 0a20 2060 6060  nd babyagi.  ```
+000003b0: 0a0a 215b 4261 6279 6167 692d 6173 2d61  ..![Babyagi-as-a
+000003c0: 2d73 6572 7669 6365 2050 6c61 7967 726f  -service Playgro
+000003d0: 756e 645d 282e 6769 7468 7562 2f69 6d61  und](.github/ima
+000003e0: 6765 732f 6261 6279 6167 692d 706c 6179  ges/babyagi-play
+000003f0: 6772 6f75 6e64 2e67 6966 290a 0a0a 2323  ground.gif)...##
+00000400: 2323 20f0 9f8e 8920 4375 7374 6f6d 2041  ## .... Custom A
+00000410: 7070 7320 746f 2070 726f 6475 6374 696f  pps to productio
+00000420: 6e20 696e 2034 2073 696d 706c 6520 7374  n in 4 simple st
+00000430: 6570 730a 0a20 2031 2e20 5265 6661 6374  eps..  1. Refact
+00000440: 6f72 2079 6f75 7220 636f 6465 2074 6f20  or your code to 
+00000450: 6675 6e63 7469 6f6e 2873 2920 7468 6174  function(s) that
+00000460: 2073 686f 756c 6420 6265 2073 6572 7665   should be serve
+00000470: 6420 7769 7468 2060 4073 6572 7669 6e67  d with `@serving
+00000480: 6020 6465 636f 7261 746f 722e 0a20 2031  ` decorator..  1
+00000490: 2e20 4372 6561 7465 2061 2060 7265 7175  . Create a `requ
+000004a0: 6972 656d 656e 7473 2e74 7874 6020 6669  irements.txt` fi
+000004b0: 6c65 2069 6e20 796f 7572 2061 7070 2064  le in your app d
+000004c0: 6972 6563 746f 7279 2074 6f20 656e 7375  irectory to ensu
+000004d0: 7265 2061 6c6c 206e 6563 6573 7361 7279  re all necessary
+000004e0: 2064 6570 656e 6465 6e63 6965 7320 6172   dependencies ar
+000004f0: 6520 696e 7374 616c 6c65 642e 0a20 2031  e installed..  1
+00000500: 2e20 5275 6e20 606c 632d 7365 7276 6520  . Run `lc-serve 
+00000510: 6465 706c 6f79 206c 6f63 616c 2061 7070  deploy local app
+00000520: 6020 746f 2074 6573 7420 796f 7572 2041  ` to test your A
+00000530: 5049 206c 6f63 616c 6c79 2e0a 2020 312e  PI locally..  1.
+00000540: 2052 756e 2060 6c63 2d73 6572 7665 2064   Run `lc-serve d
+00000550: 6570 6c6f 7920 6a63 6c6f 7564 2061 7070  eploy jcloud app
+00000560: 6020 746f 2064 6570 6c6f 7920 6f6e 205b  ` to deploy on [
+00000570: 4a69 6e61 2041 4920 436c 6f75 645d 2868  Jina AI Cloud](h
+00000580: 7474 7073 3a2f 2f6a 696e 612e 6169 2f70  ttps://jina.ai/p
+00000590: 726f 6475 6374 2f63 6c6f 7564 2f29 2e0a  roduct/cloud/)..
+000005a0: 0a0a 2323 2323 20f0 9f94 a520 5363 616c  ..#### .... Scal
+000005b0: 6162 6c65 2c20 5365 7276 6572 6c65 7373  able, Serverless
+000005c0: 2052 4553 5466 756c 2f53 7472 6561 6d69   RESTful/Streami
+000005d0: 6e67 2057 6562 736f 636b 6574 2041 5049  ng Websocket API
+000005e0: 7320 6f6e 204a 696e 6120 4149 2043 6c6f  s on Jina AI Clo
+000005f0: 7564 0a0a 2020 2d20 f09f 8c8e 2052 4553  ud..  - .... RES
+00000600: 5466 756c 2f57 6562 736f 636b 6574 2041  Tful/Websocket A
+00000610: 5049 7320 7769 7468 2054 4c53 2063 6572  PIs with TLS cer
+00000620: 7473 2069 6e20 6a75 7374 2032 206c 696e  ts in just 2 lin
+00000630: 6573 206f 6620 636f 6465 2063 6861 6e67  es of code chang
+00000640: 652e 0a20 202d 20f0 9f8c 8a20 5374 7265  e..  - .... Stre
+00000650: 616d 204c 4c4d 2069 6e74 6572 6163 7469  am LLM interacti
+00000660: 6f6e 7320 696e 2072 6561 6c2d 7469 6d65  ons in real-time
+00000670: 2077 6974 6820 5765 6273 6f63 6b65 7473   with Websockets
+00000680: 2e0a 2020 2d20 f09f 91a5 2045 6e61 626c  ..  - .... Enabl
+00000690: 6520 6875 6d61 6e20 696e 2074 6865 206c  e human in the l
+000006a0: 6f6f 7020 666f 7220 796f 7572 2061 6765  oop for your age
+000006b0: 6e74 732e 0a20 202d 20f0 9f93 8420 5377  nts..  - .... Sw
+000006c0: 6167 6765 7220 5549 2c20 616e 6420 4f70  agger UI, and Op
+000006d0: 656e 4150 4920 7370 6563 2069 6e63 6c75  enAPI spec inclu
+000006e0: 6465 6420 7769 7468 2079 6f75 7220 4150  ded with your AP
+000006f0: 4973 2e0a 2020 2d20 e29a a1ef b88f 2053  Is..  - ...... S
+00000700: 6572 7665 726c 6573 7320 6170 7073 2074  erverless apps t
+00000710: 6861 7420 7363 616c 6573 2061 7574 6f6d  hat scales autom
+00000720: 6174 6963 616c 6c79 2077 6974 6820 796f  atically with yo
+00000730: 7572 2074 7261 6666 6963 2e0a 2020 2d20  ur traffic..  - 
+00000740: f09f 938a 2042 7569 6c74 696e 206c 6f67  .... Builtin log
+00000750: 6769 6e67 2c20 6d6f 6e69 746f 7269 6e67  ging, monitoring
+00000760: 2c20 616e 6420 7472 6163 6573 2066 6f72  , and traces for
+00000770: 2079 6f75 7220 4150 4973 2e0a 2020 2d20   your APIs..  - 
+00000780: f09f a496 204e 6f20 6e65 6564 2074 6f20  .... No need to 
+00000790: 6368 616e 6765 2079 6f75 7220 636f 6465  change your code
+000007a0: 2074 6f20 6d61 6e61 6765 2041 5049 732c   to manage APIs,
+000007b0: 206f 7220 6d61 6e61 6765 2064 6f63 6b65   or manage docke
+000007c0: 7266 696c 6573 2c20 6f72 2077 6f72 7279  rfiles, or worry
+000007d0: 2061 626f 7574 2069 6e66 7261 7374 7275   about infrastru
+000007e0: 6374 7572 6521 0a0a 0a23 2323 2320 f09f  cture!...#### ..
+000007f0: 9aa7 2043 6f6d 696e 6720 736f 6f6e 0a0a  .. Coming soon..
+00000800: 2d20 5b20 5d20 f09f 9491 2041 7574 686f  - [ ] .... Autho
+00000810: 7269 7a65 2041 5049 2065 6e64 706f 696e  rize API endpoin
+00000820: 7473 0a2d 205b 205d 20f0 9f9b a0ef b88f  ts.- [ ] .......
+00000830: 2045 6e61 626c 6520 5374 7265 616d 6c69   Enable Streamli
+00000840: 7420 706c 6179 6772 6f75 6e64 2064 6570  t playground dep
+00000850: 6c6f 796d 656e 7420 666f 7220 796f 7572  loyment for your
+00000860: 2061 7070 730a 0a0a 4966 2079 6f75 2068   apps...If you h
+00000870: 6176 6520 616e 7920 6665 6174 7572 6520  ave any feature 
+00000880: 7265 7175 6573 7473 206f 7220 6661 6365  requests or face
+00000890: 6420 616e 7920 6973 7375 652c 2070 6c65  d any issue, ple
+000008a0: 6173 6520 5b6c 6574 2075 7320 6b6e 6f77  ase [let us know
+000008b0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+000008c0: 2e63 6f6d 2f6a 696e 612d 6169 2f6c 616e  .com/jina-ai/lan
+000008d0: 6763 6861 696e 2d73 6572 7665 2f69 7373  gchain-serve/iss
+000008e0: 7565 732f 6e65 7729 210a 0a0a 2323 2055  ues/new)!...## U
+000008f0: 7361 6765 0a0a 4c65 7427 7320 6669 7273  sage..Let's firs
+00000900: 7420 696e 7374 616c 6c20 606c 616e 6763  t install `langc
+00000910: 6861 696e 2d73 6572 7665 6020 7573 696e  hain-serve` usin
+00000920: 6720 7069 702e 0a0a 6060 6062 6173 680a  g pip...```bash.
+00000930: 7069 7020 696e 7374 616c 6c20 6c61 6e67  pip install lang
+00000940: 6368 6169 6e2d 7365 7276 650a 6060 600a  chain-serve.```.
+00000950: 0a23 2320 456e 6162 6c65 2048 756d 616e  .## Enable Human
+00000960: 2d69 6e2d 7468 652d 6c6f 6f70 2028 4849  -in-the-loop (HI
+00000970: 544c 2920 666f 7220 796f 7572 2061 6765  TL) for your age
+00000980: 6e74 730a 0a48 4954 4c20 666f 7220 4c61  nts..HITL for La
+00000990: 6e67 4368 6169 6e20 6167 656e 7473 206f  ngChain agents o
+000009a0: 6e20 7072 6f64 7563 7469 6f6e 2063 616e  n production can
+000009b0: 2062 6520 6368 616c 6c65 6e67 696e 6720   be challenging 
+000009c0: 7369 6e63 6520 7468 6520 6167 656e 7473  since the agents
+000009d0: 2061 7265 2074 7970 6963 616c 6c79 2072   are typically r
+000009e0: 756e 6e69 6e67 206f 6e20 7365 7276 6572  unning on server
+000009f0: 7320 7768 6572 6520 6875 6d61 6e73 2064  s where humans d
+00000a00: 6f6e 2774 2068 6176 6520 6469 7265 6374  on't have direct
+00000a10: 2061 6363 6573 732e 202a 2a6c 616e 6763   access. **langc
+00000a20: 6861 696e 2d73 6572 7665 2a2a 2062 7269  hain-serve** bri
+00000a30: 6467 6573 2074 6869 7320 6761 7020 6279  dges this gap by
+00000a40: 2065 6e61 626c 696e 6720 7765 6273 6f63   enabling websoc
+00000a50: 6b65 7420 4150 4973 2074 6861 7420 616c  ket APIs that al
+00000a60: 6c6f 7720 666f 7220 7265 616c 2d74 696d  low for real-tim
+00000a70: 6520 696e 7465 7261 6374 696f 6e20 616e  e interaction an
+00000a80: 6420 6665 6564 6261 636b 2062 6574 7765  d feedback betwe
+00000a90: 656e 2074 6865 2061 6765 6e74 2061 6e64  en the agent and
+00000aa0: 2061 2068 756d 616e 206f 7065 7261 746f   a human operato
+00000ab0: 722e 0a0a 4368 6563 6b20 6f75 7420 7468  r...Check out th
+00000ac0: 6973 205b 6578 616d 706c 655d 2865 7861  is [example](exa
+00000ad0: 6d70 6c65 732f 7765 6273 6f63 6b65 7473  mples/websockets
+00000ae0: 2f68 6974 6c2f 5245 4144 4d45 2e6d 6429  /hitl/README.md)
+00000af0: 2074 6f20 7365 6520 686f 7720 796f 7520   to see how you 
+00000b00: 6361 6e20 656e 6162 6c65 2048 4954 4c20  can enable HITL 
+00000b10: 666f 7220 796f 7572 2061 6765 6e74 732e  for your agents.
+00000b20: 0a0a 0a23 2320 456e 6162 6c65 2052 4553  ...## Enable RES
+00000b30: 5420 4150 4973 200a 0a0a 4c65 7427 7320  T APIs ...Let's 
+00000b40: 6275 696c 6420 6120 6375 7374 6f6d 2061  build a custom a
+00000b50: 6765 6e74 2075 7369 6e67 2074 6869 7320  gent using this 
+00000b60: 6578 616d 706c 6520 7461 6b65 6e20 6672  example taken fr
+00000b70: 6f6d 205b 4c61 6e67 4368 6169 6e20 646f  om [LangChain do
+00000b80: 6375 6d65 6e74 6174 696f 6e5d 2868 7474  cumentation](htt
+00000b90: 7073 3a2f 2f70 7974 686f 6e2e 6c61 6e67  ps://python.lang
+00000ba0: 6368 6169 6e2e 636f 6d2f 656e 2f6c 6174  chain.com/en/lat
+00000bb0: 6573 742f 6d6f 6475 6c65 732f 6167 656e  est/modules/agen
+00000bc0: 7473 2f61 6765 6e74 732f 6375 7374 6f6d  ts/agents/custom
+00000bd0: 5f61 6765 6e74 2e68 746d 6c29 2e20 0a0a  _agent.html). ..
+00000be0: 0a3c 6465 7461 696c 733e 0a3c 7375 6d6d  .<details>.<summ
+00000bf0: 6172 793e 5368 6f77 2061 6765 6e74 2063  ary>Show agent c
+00000c00: 6f64 6520 2861 7070 2e70 7929 3c2f 7375  ode (app.py)</su
+00000c10: 6d6d 6172 793e 0a0a 6060 6070 7974 686f  mmary>..```pytho
+00000c20: 6e0a 2320 6170 702e 7079 0a66 726f 6d20  n.# app.py.from 
+00000c30: 6c61 6e67 6368 6169 6e2e 6167 656e 7473  langchain.agents
+00000c40: 2069 6d70 6f72 7420 5a65 726f 5368 6f74   import ZeroShot
+00000c50: 4167 656e 742c 2054 6f6f 6c2c 2041 6765  Agent, Tool, Age
+00000c60: 6e74 4578 6563 7574 6f72 0a66 726f 6d20  ntExecutor.from 
+00000c70: 6c61 6e67 6368 6169 6e20 696d 706f 7274  langchain import
+00000c80: 204f 7065 6e41 492c 2053 6572 7041 5049   OpenAI, SerpAPI
+00000c90: 5772 6170 7065 722c 204c 4c4d 4368 6169  Wrapper, LLMChai
+00000ca0: 6e0a 0a73 6561 7263 6820 3d20 5365 7270  n..search = Serp
+00000cb0: 4150 4957 7261 7070 6572 2829 0a74 6f6f  APIWrapper().too
+00000cc0: 6c73 203d 205b 0a20 2020 2054 6f6f 6c28  ls = [.    Tool(
+00000cd0: 0a20 2020 2020 2020 206e 616d 6520 3d20  .        name = 
+00000ce0: 2253 6561 7263 6822 2c0a 2020 2020 2020  "Search",.      
+00000cf0: 2020 6675 6e63 3d73 6561 7263 682e 7275    func=search.ru
+00000d00: 6e2c 0a20 2020 2020 2020 2064 6573 6372  n,.        descr
+00000d10: 6970 7469 6f6e 3d22 7573 6566 756c 2066  iption="useful f
+00000d20: 6f72 2077 6865 6e20 796f 7520 6e65 6564  or when you need
+00000d30: 2074 6f20 616e 7377 6572 2071 7565 7374   to answer quest
+00000d40: 696f 6e73 2061 626f 7574 2063 7572 7265  ions about curre
+00000d50: 6e74 2065 7665 6e74 7322 0a20 2020 2029  nt events".    )
+00000d60: 0a5d 0a0a 7072 6566 6978 203d 2022 2222  .]..prefix = """
+00000d70: 416e 7377 6572 2074 6865 2066 6f6c 6c6f  Answer the follo
+00000d80: 7769 6e67 2071 7565 7374 696f 6e73 2061  wing questions a
+00000d90: 7320 6265 7374 2079 6f75 2063 616e 2c20  s best you can, 
+00000da0: 6275 7420 7370 6561 6b69 6e67 2061 7320  but speaking as 
+00000db0: 6120 7069 7261 7465 206d 6967 6874 2073  a pirate might s
+00000dc0: 7065 616b 2e20 596f 7520 6861 7665 2061  peak. You have a
+00000dd0: 6363 6573 7320 746f 2074 6865 2066 6f6c  ccess to the fol
+00000de0: 6c6f 7769 6e67 2074 6f6f 6c73 3a22 2222  lowing tools:"""
+00000df0: 0a73 7566 6669 7820 3d20 2222 2242 6567  .suffix = """Beg
+00000e00: 696e 2120 5265 6d65 6d62 6572 2074 6f20  in! Remember to 
+00000e10: 7370 6561 6b20 6173 2061 2070 6972 6174  speak as a pirat
+00000e20: 6520 7768 656e 2067 6976 696e 6720 796f  e when giving yo
+00000e30: 7572 2066 696e 616c 2061 6e73 7765 722e  ur final answer.
+00000e40: 2055 7365 206c 6f74 7320 6f66 2022 4172   Use lots of "Ar
+00000e50: 6773 220a 0a51 7565 7374 696f 6e3a 207b  gs"..Question: {
+00000e60: 696e 7075 747d 0a7b 6167 656e 745f 7363  input}.{agent_sc
+00000e70: 7261 7463 6870 6164 7d22 2222 0a0a 7072  ratchpad}"""..pr
+00000e80: 6f6d 7074 203d 205a 6572 6f53 686f 7441  ompt = ZeroShotA
+00000e90: 6765 6e74 2e63 7265 6174 655f 7072 6f6d  gent.create_prom
+00000ea0: 7074 280a 2020 2020 746f 6f6c 732c 200a  pt(.    tools, .
+00000eb0: 2020 2020 7072 6566 6978 3d70 7265 6669      prefix=prefi
+00000ec0: 782c 200a 2020 2020 7375 6666 6978 3d73  x, .    suffix=s
+00000ed0: 7566 6669 782c 200a 2020 2020 696e 7075  uffix, .    inpu
+00000ee0: 745f 7661 7269 6162 6c65 733d 5b22 696e  t_variables=["in
+00000ef0: 7075 7422 2c20 2261 6765 6e74 5f73 6372  put", "agent_scr
+00000f00: 6174 6368 7061 6422 5d0a 290a 0a6c 6c6d  atchpad"].)..llm
+00000f10: 5f63 6861 696e 203d 204c 4c4d 4368 6169  _chain = LLMChai
+00000f20: 6e28 6c6c 6d3d 4f70 656e 4149 2874 656d  n(llm=OpenAI(tem
+00000f30: 7065 7261 7475 7265 3d30 292c 2070 726f  perature=0), pro
+00000f40: 6d70 743d 7072 6f6d 7074 290a 746f 6f6c  mpt=prompt).tool
+00000f50: 5f6e 616d 6573 203d 205b 746f 6f6c 2e6e  _names = [tool.n
+00000f60: 616d 6520 666f 7220 746f 6f6c 2069 6e20  ame for tool in 
+00000f70: 746f 6f6c 735d 0a61 6765 6e74 203d 205a  tools].agent = Z
+00000f80: 6572 6f53 686f 7441 6765 6e74 286c 6c6d  eroShotAgent(llm
+00000f90: 5f63 6861 696e 3d6c 6c6d 5f63 6861 696e  _chain=llm_chain
+00000fa0: 2c20 616c 6c6f 7765 645f 746f 6f6c 733d  , allowed_tools=
+00000fb0: 746f 6f6c 5f6e 616d 6573 290a 6167 656e  tool_names).agen
+00000fc0: 745f 6578 6563 7574 6f72 203d 2041 6765  t_executor = Age
+00000fd0: 6e74 4578 6563 7574 6f72 2e66 726f 6d5f  ntExecutor.from_
+00000fe0: 6167 656e 745f 616e 645f 746f 6f6c 7328  agent_and_tools(
+00000ff0: 6167 656e 743d 6167 656e 742c 2074 6f6f  agent=agent, too
+00001000: 6c73 3d74 6f6f 6c73 2c20 7665 7262 6f73  ls=tools, verbos
+00001010: 653d 5472 7565 290a 6167 656e 745f 6578  e=True).agent_ex
+00001020: 6563 7574 6f72 2e72 756e 2822 486f 7720  ecutor.run("How 
+00001030: 6d61 6e79 2070 656f 706c 6520 6c69 7665  many people live
+00001040: 2069 6e20 6361 6e61 6461 2061 7320 6f66   in canada as of
+00001050: 2032 3032 333f 2229 0a60 6060 0a0a 2323   2023?").```..##
+00001060: 2323 204f 7574 7075 740a 0a0a 6060 6074  ## Output...```t
+00001070: 6578 740a 3e20 456e 7465 7269 6e67 206e  ext.> Entering n
+00001080: 6577 2041 6765 6e74 4578 6563 7574 6f72  ew AgentExecutor
+00001090: 2063 6861 696e 2e2e 2e0a 5468 6f75 6768   chain....Though
+000010a0: 743a 2049 206e 6565 6420 746f 2066 696e  t: I need to fin
+000010b0: 6420 6f75 7420 7468 6520 706f 7075 6c61  d out the popula
+000010c0: 7469 6f6e 206f 6620 4361 6e61 6461 0a41  tion of Canada.A
+000010d0: 6374 696f 6e3a 2053 6561 7263 680a 4163  ction: Search.Ac
+000010e0: 7469 6f6e 2049 6e70 7574 3a20 506f 7075  tion Input: Popu
+000010f0: 6c61 7469 6f6e 206f 6620 4361 6e61 6461  lation of Canada
+00001100: 2032 3032 330a 4f62 7365 7276 6174 696f   2023.Observatio
+00001110: 6e3a 2054 6865 2063 7572 7265 6e74 2070  n: The current p
+00001120: 6f70 756c 6174 696f 6e20 6f66 2043 616e  opulation of Can
+00001130: 6164 6120 6973 2033 382c 3631 302c 3434  ada is 38,610,44
+00001140: 3720 6173 206f 6620 5361 7475 7264 6179  7 as of Saturday
+00001150: 2c20 4665 6272 7561 7279 2031 382c 2032  , February 18, 2
+00001160: 3032 332c 2062 6173 6564 206f 6e20 576f  023, based on Wo
+00001170: 726c 646f 6d65 7465 7220 656c 6162 6f72  rldometer elabor
+00001180: 6174 696f 6e20 6f66 2074 6865 206c 6174  ation of the lat
+00001190: 6573 7420 556e 6974 6564 204e 6174 696f  est United Natio
+000011a0: 6e73 2064 6174 612e 2043 616e 6164 6120  ns data. Canada 
+000011b0: 3230 3230 2070 6f70 756c 6174 696f 6e20  2020 population 
+000011c0: 6973 2065 7374 696d 6174 6564 2061 7420  is estimated at 
+000011d0: 3337 2c37 3432 2c31 3534 2070 656f 706c  37,742,154 peopl
+000011e0: 6520 6174 206d 6964 2079 6561 7220 6163  e at mid year ac
+000011f0: 636f 7264 696e 6720 746f 2055 4e20 6461  cording to UN da
+00001200: 7461 2e0a 5468 6f75 6768 743a 2049 206e  ta..Thought: I n
+00001210: 6f77 206b 6e6f 7720 7468 6520 6669 6e61  ow know the fina
+00001220: 6c20 616e 7377 6572 0a46 696e 616c 2041  l answer.Final A
+00001230: 6e73 7765 723a 2041 7272 722c 2043 616e  nswer: Arrr, Can
+00001240: 6164 6120 6265 2068 6176 696e 2720 3338  ada be havin' 38
+00001250: 2c36 3130 2c34 3437 2073 6361 6c6c 7977  ,610,447 scallyw
+00001260: 6167 7320 6c69 7669 6e27 2074 6865 7265  ags livin' there
+00001270: 2061 7320 6f66 2032 3032 3321 0a0a 3e20   as of 2023!..> 
+00001280: 4669 6e69 7368 6564 2063 6861 696e 2e0a  Finished chain..
+00001290: 6060 600a 0a3c 2f64 6574 6169 6c73 3e0a  ```..</details>.
+000012a0: 0a23 2323 2053 7465 7020 313a 200a 0a2a  .### Step 1: ..*
+000012b0: 2a52 6566 6163 746f 7220 796f 7572 2063  *Refactor your c
+000012c0: 6f64 6520 746f 2066 756e 6374 696f 6e28  ode to function(
+000012d0: 7329 2074 6861 7420 7368 6f75 6c64 2062  s) that should b
+000012e0: 6520 7365 7276 6564 2077 6974 6820 6040  e served with `@
+000012f0: 7365 7276 696e 6760 2064 6563 6f72 6174  serving` decorat
+00001300: 6f72 2a2a 0a0a 0a3c 6465 7461 696c 733e  or**...<details>
+00001310: 0a3c 7375 6d6d 6172 793e 5368 6f77 2075  .<summary>Show u
+00001320: 7064 6174 6564 2061 6765 6e74 2063 6f64  pdated agent cod
+00001330: 6520 2861 7070 2e70 7929 3c2f 7375 6d6d  e (app.py)</summ
+00001340: 6172 793e 0a0a 6060 6070 7974 686f 6e0a  ary>..```python.
+00001350: 2320 6170 702e 7079 0a66 726f 6d20 6c61  # app.py.from la
+00001360: 6e67 6368 6169 6e20 696d 706f 7274 204c  ngchain import L
+00001370: 4c4d 4368 6169 6e2c 204f 7065 6e41 492c  LMChain, OpenAI,
+00001380: 2053 6572 7041 5049 5772 6170 7065 720a   SerpAPIWrapper.
+00001390: 6672 6f6d 206c 616e 6763 6861 696e 2e61  from langchain.a
+000013a0: 6765 6e74 7320 696d 706f 7274 2041 6765  gents import Age
+000013b0: 6e74 4578 6563 7574 6f72 2c20 546f 6f6c  ntExecutor, Tool
+000013c0: 2c20 5a65 726f 5368 6f74 4167 656e 740a  , ZeroShotAgent.
+000013d0: 0a66 726f 6d20 6c63 7365 7276 6520 696d  .from lcserve im
+000013e0: 706f 7274 2073 6572 7669 6e67 0a0a 0a40  port serving...@
+000013f0: 7365 7276 696e 670a 6465 6620 6173 6b28  serving.def ask(
+00001400: 696e 7075 743a 2073 7472 2920 2d3e 2073  input: str) -> s
+00001410: 7472 3a0a 2020 2020 7365 6172 6368 203d  tr:.    search =
+00001420: 2053 6572 7041 5049 5772 6170 7065 7228   SerpAPIWrapper(
+00001430: 290a 2020 2020 746f 6f6c 7320 3d20 5b0a  ).    tools = [.
+00001440: 2020 2020 2020 2020 546f 6f6c 280a 2020          Tool(.  
+00001450: 2020 2020 2020 2020 2020 6e61 6d65 3d22            name="
+00001460: 5365 6172 6368 222c 0a20 2020 2020 2020  Search",.       
+00001470: 2020 2020 2066 756e 633d 7365 6172 6368       func=search
+00001480: 2e72 756e 2c0a 2020 2020 2020 2020 2020  .run,.          
+00001490: 2020 6465 7363 7269 7074 696f 6e3d 2275    description="u
+000014a0: 7365 6675 6c20 666f 7220 7768 656e 2079  seful for when y
+000014b0: 6f75 206e 6565 6420 746f 2061 6e73 7765  ou need to answe
+000014c0: 7220 7175 6573 7469 6f6e 7320 6162 6f75  r questions abou
+000014d0: 7420 6375 7272 656e 7420 6576 656e 7473  t current events
+000014e0: 222c 0a20 2020 2020 2020 2029 0a20 2020  ",.        ).   
+000014f0: 205d 0a20 2020 2070 7265 6669 7820 3d20   ].    prefix = 
+00001500: 2222 2241 6e73 7765 7220 7468 6520 666f  """Answer the fo
+00001510: 6c6c 6f77 696e 6720 7175 6573 7469 6f6e  llowing question
+00001520: 7320 6173 2062 6573 7420 796f 7520 6361  s as best you ca
+00001530: 6e2c 2062 7574 2073 7065 616b 696e 6720  n, but speaking 
+00001540: 6173 2061 2070 6972 6174 6520 6d69 6768  as a pirate migh
+00001550: 7420 7370 6561 6b2e 2059 6f75 2068 6176  t speak. You hav
+00001560: 6520 6163 6365 7373 2074 6f20 7468 6520  e access to the 
+00001570: 666f 6c6c 6f77 696e 6720 746f 6f6c 733a  following tools:
+00001580: 2222 220a 2020 2020 7375 6666 6978 203d  """.    suffix =
+00001590: 2022 2222 4265 6769 6e21 2052 656d 656d   """Begin! Remem
+000015a0: 6265 7220 746f 2073 7065 616b 2061 7320  ber to speak as 
+000015b0: 6120 7069 7261 7465 2077 6865 6e20 6769  a pirate when gi
+000015c0: 7669 6e67 2079 6f75 7220 6669 6e61 6c20  ving your final 
+000015d0: 616e 7377 6572 2e20 5573 6520 6c6f 7473  answer. Use lots
+000015e0: 206f 6620 2241 7267 7322 0a0a 2020 2020   of "Args"..    
+000015f0: 5175 6573 7469 6f6e 3a20 7b69 6e70 7574  Question: {input
+00001600: 7d0a 2020 2020 7b61 6765 6e74 5f73 6372  }.    {agent_scr
+00001610: 6174 6368 7061 647d 2222 220a 0a20 2020  atchpad}"""..   
+00001620: 2070 726f 6d70 7420 3d20 5a65 726f 5368   prompt = ZeroSh
+00001630: 6f74 4167 656e 742e 6372 6561 7465 5f70  otAgent.create_p
+00001640: 726f 6d70 7428 0a20 2020 2020 2020 2074  rompt(.        t
+00001650: 6f6f 6c73 2c0a 2020 2020 2020 2020 7072  ools,.        pr
+00001660: 6566 6978 3d70 7265 6669 782c 0a20 2020  efix=prefix,.   
+00001670: 2020 2020 2073 7566 6669 783d 7375 6666       suffix=suff
+00001680: 6978 2c0a 2020 2020 2020 2020 696e 7075  ix,.        inpu
+00001690: 745f 7661 7269 6162 6c65 733d 5b22 696e  t_variables=["in
+000016a0: 7075 7422 2c20 2261 6765 6e74 5f73 6372  put", "agent_scr
+000016b0: 6174 6368 7061 6422 5d2c 0a20 2020 2029  atchpad"],.    )
+000016c0: 0a0a 2020 2020 7072 696e 7428 7072 6f6d  ..    print(prom
+000016d0: 7074 2e74 656d 706c 6174 6529 0a0a 2020  pt.template)..  
+000016e0: 2020 6c6c 6d5f 6368 6169 6e20 3d20 4c4c    llm_chain = LL
+000016f0: 4d43 6861 696e 286c 6c6d 3d4f 7065 6e41  MChain(llm=OpenA
+00001700: 4928 7465 6d70 6572 6174 7572 653d 3029  I(temperature=0)
+00001710: 2c20 7072 6f6d 7074 3d70 726f 6d70 7429  , prompt=prompt)
+00001720: 0a20 2020 2074 6f6f 6c5f 6e61 6d65 7320  .    tool_names 
+00001730: 3d20 5b74 6f6f 6c2e 6e61 6d65 2066 6f72  = [tool.name for
+00001740: 2074 6f6f 6c20 696e 2074 6f6f 6c73 5d0a   tool in tools].
+00001750: 2020 2020 6167 656e 7420 3d20 5a65 726f      agent = Zero
+00001760: 5368 6f74 4167 656e 7428 6c6c 6d5f 6368  ShotAgent(llm_ch
+00001770: 6169 6e3d 6c6c 6d5f 6368 6169 6e2c 2061  ain=llm_chain, a
+00001780: 6c6c 6f77 6564 5f74 6f6f 6c73 3d74 6f6f  llowed_tools=too
+00001790: 6c5f 6e61 6d65 7329 0a0a 2020 2020 6167  l_names)..    ag
+000017a0: 656e 745f 6578 6563 7574 6f72 203d 2041  ent_executor = A
+000017b0: 6765 6e74 4578 6563 7574 6f72 2e66 726f  gentExecutor.fro
+000017c0: 6d5f 6167 656e 745f 616e 645f 746f 6f6c  m_agent_and_tool
+000017d0: 7328 0a20 2020 2020 2020 2061 6765 6e74  s(.        agent
+000017e0: 3d61 6765 6e74 2c20 746f 6f6c 733d 746f  =agent, tools=to
+000017f0: 6f6c 732c 2076 6572 626f 7365 3d54 7275  ols, verbose=Tru
+00001800: 650a 2020 2020 290a 0a20 2020 2072 6574  e.    )..    ret
+00001810: 7572 6e20 6167 656e 745f 6578 6563 7574  urn agent_execut
+00001820: 6f72 2e72 756e 2869 6e70 7574 290a 0a69  or.run(input)..i
+00001830: 6620 5f5f 6e61 6d65 5f5f 203d 3d20 225f  f __name__ == "_
+00001840: 5f6d 6169 6e5f 5f22 3a0a 2020 2020 6173  _main__":.    as
+00001850: 6b28 2748 6f77 206d 616e 7920 7065 6f70  k('How many peop
+00001860: 6c65 206c 6976 6520 696e 2063 616e 6164  le live in canad
+00001870: 6120 6173 206f 6620 3230 3233 3f27 290a  a as of 2023?').
+00001880: 6060 600a 0a3c 2f64 6574 6169 6c73 3e0a  ```..</details>.
+00001890: 0a0a 2323 2323 2320 5768 6174 2063 6861  ..##### What cha
+000018a0: 6e67 6564 3f0a 0a2d 2057 6520 6d6f 7665  nged?..- We move
+000018b0: 6420 6f75 7220 636f 6465 2074 6f20 616e  d our code to an
+000018c0: 2060 6173 6b60 2066 756e 6374 696f 6e2e   `ask` function.
+000018d0: 0a2d 2041 6464 6564 2074 7970 6520 6869  .- Added type hi
+000018e0: 6e74 7320 746f 2074 6865 2066 756e 6374  nts to the funct
+000018f0: 696f 6e20 7061 7261 6d65 7465 7273 2028  ion parameters (
+00001900: 696e 7075 7420 616e 6420 6f75 7470 7574  input and output
+00001910: 292c 2073 6f20 4150 4920 6465 6669 6e69  ), so API defini
+00001920: 7469 6f6e 2063 616e 2062 6520 6765 6e65  tion can be gene
+00001930: 7261 7465 642e 0a2d 2049 6d70 6f72 7465  rated..- Importe
+00001940: 6420 6066 726f 6d20 6c63 7365 7276 6520  d `from lcserve 
+00001950: 696d 706f 7274 2073 6572 7669 6e67 6020  import serving` 
+00001960: 616e 6420 6164 6465 6420 6040 7365 7276  and added `@serv
+00001970: 696e 6760 2064 6563 6f72 6174 6f72 2074  ing` decorator t
+00001980: 6f20 7468 6520 6061 736b 6020 6675 6e63  o the `ask` func
+00001990: 7469 6f6e 2e0a 2d20 4164 6465 6420 6069  tion..- Added `i
+000019a0: 6620 5f5f 6e61 6d65 5f5f 203d 3d20 225f  f __name__ == "_
+000019b0: 5f6d 6169 6e5f 5f22 3a60 2062 6c6f 636b  _main__":` block
+000019c0: 2074 6f20 7465 7374 2074 6865 2066 756e   to test the fun
+000019d0: 6374 696f 6e20 6c6f 6361 6c6c 792e 0a0a  ction locally...
+000019e0: 2d2d 2d0a 0a23 2323 2053 7465 7020 323a  ---..### Step 2:
+000019f0: 0a0a 2a2a 4372 6561 7465 2061 2060 7265  ..**Create a `re
+00001a00: 7175 6972 656d 656e 7473 2e74 7874 6020  quirements.txt` 
+00001a10: 6669 6c65 2069 6e20 796f 7572 2061 7070  file in your app
+00001a20: 2064 6972 6563 746f 7279 2074 6f20 656e   directory to en
+00001a30: 7375 7265 2061 6c6c 206e 6563 6573 7361  sure all necessa
+00001a40: 7279 2064 6570 656e 6465 6e63 6965 7320  ry dependencies 
+00001a50: 6172 6520 696e 7374 616c 6c65 642e 2a2a  are installed.**
+00001a60: 0a0a 3c64 6574 6169 6c73 3e0a 3c73 756d  ..<details>.<sum
+00001a70: 6d61 7279 3e53 686f 7720 7265 7175 6972  mary>Show requir
+00001a80: 656d 656e 7473 2e74 7874 3c2f 7375 6d6d  ements.txt</summ
+00001a90: 6172 793e 0a0a 6060 6074 6578 740a 2320  ary>..```text.# 
+00001aa0: 7265 7175 6972 656d 656e 7473 2e74 7874  requirements.txt
+00001ab0: 0a6f 7065 6e61 690a 676f 6f67 6c65 2d73  .openai.google-s
+00001ac0: 6561 7263 682d 7265 7375 6c74 730a 6060  earch-results.``
+00001ad0: 600a 3c2f 6465 7461 696c 733e 0a0a 2d2d  `.</details>..--
+00001ae0: 2d20 0a0a 2323 2320 5374 6570 2033 3a0a  - ..### Step 3:.
+00001af0: 0a2a 2a52 756e 2060 6c63 2d73 6572 7665  .**Run `lc-serve
+00001b00: 2064 6570 6c6f 7920 6c6f 6361 6c20 6170   deploy local ap
+00001b10: 7060 2074 6f20 7465 7374 2079 6f75 7220  p` to test your 
+00001b20: 4150 4920 6c6f 6361 6c6c 792e 2a2a 0a0a  API locally.**..
+00001b30: 3e20 6061 7070 6020 6973 2074 6865 206e  > `app` is the n
+00001b40: 616d 6520 6f66 2074 6865 206d 6f64 756c  ame of the modul
+00001b50: 6520 7468 6174 2063 6f6e 7461 696e 7320  e that contains 
+00001b60: 7468 6520 6061 736b 6020 6675 6e63 7469  the `ask` functi
+00001b70: 6f6e 2e0a 0a60 6060 6261 7368 0a6c 632d  on...```bash.lc-
+00001b80: 7365 7276 6520 6465 706c 6f79 206c 6f63  serve deploy loc
+00001b90: 616c 2061 7070 0a60 6060 0a0a 3c64 6574  al app.```..<det
+00001ba0: 6169 6c73 3e0a 3c73 756d 6d61 7279 3e53  ails>.<summary>S
+00001bb0: 686f 7720 6f75 7470 7574 3c2f 7375 6d6d  how output</summ
+00001bc0: 6172 793e 0a0a 6060 6074 6578 740a e294  ary>..```text...
+00001bd0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00001be0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00001bf0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00001c00: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00001c10: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00001c20: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00001c30: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00001c40: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00001c50: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00001c60: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00001c70: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00001c80: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00001c90: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00001ca0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00001cb0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00001cc0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00001cd0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00001ce0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00001cf0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00001d00: 20f0 9f8e 8920 466c 6f77 2069 7320 7265   .... Flow is re
+00001d10: 6164 7920 746f 2073 6572 7665 2120 e294  ady to serve! ..
+00001d20: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00001d30: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00001d40: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00001d50: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00001d60: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00001d70: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00001d80: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00001d90: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00001da0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00001db0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00001dc0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00001dd0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00001de0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00001df0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00001e00: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00001e10: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00001e20: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00001e30: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00001e40: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00001e50: e294 800a e295 ade2 9480 e294 80e2 9480  ................
+00001e60: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00001e70: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00001e80: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00001e90: e294 80e2 9480 e294 80e2 9480 e294 8020  ............... 
+00001ea0: f09f 9497 2045 6e64 706f 696e 7420 e294  .... Endpoint ..
+00001eb0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00001ec0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00001ed0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00001ee0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00001ef0: e294 80e2 9480 e295 ae0a e294 8220 20e2  .............  .
+00001f00: 9b93 2020 2050 726f 746f 636f 6c20 2020  ..   Protocol   
+00001f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001f30: 2020 2020 2020 4854 5450 2020 e294 820a        HTTP  ....
+00001f40: e294 8220 20f0 9f8f a020 2020 2020 4c6f  ...  ....     Lo
+00001f50: 6361 6c20 2020 2020 2020 2020 2020 2020  cal             
+00001f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001f70: 2020 2020 302e 302e 302e 303a 3830 3830      0.0.0.0:8080
+00001f80: 2020 e294 820a e294 8220 20f0 9f94 9220    .......  .... 
+00001f90: 2020 5072 6976 6174 6520 2020 2020 2020    Private       
+00001fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001fb0: 2020 2031 3932 2e31 3638 2e32 392e 3138     192.168.29.18
+00001fc0: 353a 3830 3830 2020 e294 820a e294 8220  5:8080  ....... 
+00001fd0: 20f0 9f8c 8d20 2020 2050 7562 6c69 6320   ....    Public 
+00001fe0: 2032 3430 353a 3230 313a 6430 3037 3a65   2405:201:d007:e
+00001ff0: 3865 373a 3263 3333 3a63 6638 653a 6564  8e7:2c33:cf8e:ed
+00002000: 3636 3a32 3031 383a 3830 3830 2020 e294  66:2018:8080  ..
+00002010: 820a e295 b0e2 9480 e294 80e2 9480 e294  ................
 00002020: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
 00002030: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
 00002040: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
 00002050: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
 00002060: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
 00002070: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
 00002080: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
 00002090: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
 000020a0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
 000020b0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000020c0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000020d0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-000020e0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000020f0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002100: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002110: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00002120: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002130: 9480 e294 800a e295 ade2 9480 e294 80e2  ................
-00002140: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002150: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00002160: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002170: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002180: 8020 f09f 9497 2045 6e64 706f 696e 7420  . .... Endpoint 
-00002190: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000021a0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-000021b0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000021c0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000021d0: 9480 e294 80e2 9480 e295 ae0a e294 8220  ............... 
-000021e0: 20e2 9b93 2020 2050 726f 746f 636f 6c20   ...   Protocol 
-000021f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002210: 2020 2020 2020 2020 4854 5450 2020 e294          HTTP  ..
-00002220: 820a e294 8220 20f0 9f8f a020 2020 2020  .....  ....     
-00002230: 4c6f 6361 6c20 2020 2020 2020 2020 2020  Local           
-00002240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002250: 2020 2020 2020 302e 302e 302e 303a 3830        0.0.0.0:80
-00002260: 3830 2020 e294 820a e294 8220 20f0 9f94  80  .......  ...
-00002270: 9220 2020 5072 6976 6174 6520 2020 2020  .   Private     
-00002280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002290: 2020 2020 2031 3932 2e31 3638 2e32 392e       192.168.29.
-000022a0: 3138 353a 3830 3830 2020 e294 820a e294  185:8080  ......
-000022b0: 8220 20f0 9f8c 8d20 2020 2050 7562 6c69  .  ....    Publi
-000022c0: 6320 2032 3430 353a 3230 313a 6430 3037  c  2405:201:d007
-000022d0: 3a65 3865 373a 3263 3333 3a63 6638 653a  :e8e7:2c33:cf8e:
-000022e0: 6564 3636 3a32 3031 383a 3830 3830 2020  ed66:2018:8080  
-000022f0: e294 820a e295 b0e2 9480 e294 80e2 9480  ................
-00002300: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002310: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002320: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00002330: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002340: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002350: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00002360: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002370: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002380: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00002390: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000023a0: 9480 e294 80e2 9480 e294 80e2 9480 e295  ................
-000023b0: af0a e295 ade2 9480 e294 80e2 9480 e294  ................
-000023c0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000023d0: e294 80e2 9480 20f0 9f92 8e20 4854 5450  ...... .... HTTP
-000023e0: 2065 7874 656e 7369 6f6e 20e2 9480 e294   extension .....
-000023f0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00002400: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002410: 95ae 0ae2 9482 2020 f09f 92ac 2020 2020  ......  ....    
-00002420: 2020 2020 2020 5377 6167 6765 7220 5549        Swagger UI
-00002430: 2020 2020 2020 2020 2e2e 2e2f 646f 6373          .../docs
-00002440: 2020 e294 820a e294 8220 20f0 9f93 9a20    .......  .... 
-00002450: 2020 2020 2020 2020 2020 2020 2020 5265                Re
-00002460: 646f 6320 2020 2020 2020 2e2e 2e2f 7265  doc       .../re
-00002470: 646f 6320 20e2 9482 0ae2 95b0 e294 80e2  doc  ...........
-00002480: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002490: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000024a0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000024b0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-000024c0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000024d0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000024e0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-000024f0: 80e2 9480 e294 80e2 9480 e295 af0a 6060  ..............``
-00002500: 600a 0a3c 2f64 6574 6169 6c73 3e0a 0a0a  `..</details>...
-00002510: 4c65 7427 7320 6f70 656e 2074 6865 205b  Let's open the [
-00002520: 5377 6167 6765 7220 5549 5d28 6874 7470  Swagger UI](http
-00002530: 3a2f 2f6c 6f63 616c 686f 7374 3a38 3038  ://localhost:808
-00002540: 302f 646f 6373 2920 746f 2074 6573 7420  0/docs) to test 
-00002550: 6f75 7220 4150 4920 6c6f 6361 6c6c 792e  our API locally.
-00002560: 2057 6974 6820 6054 7279 2069 7420 6f75   With `Try it ou
-00002570: 7460 2062 7574 746f 6e2c 2077 6520 6361  t` button, we ca
-00002580: 6e20 7465 7374 206f 7572 2041 5049 2077  n test our API w
-00002590: 6974 6820 6469 6666 6572 656e 7420 696e  ith different in
-000025a0: 7075 7473 2e0a 0a0a 3c64 6574 6169 6c73  puts....<details
-000025b0: 3e0a 3c73 756d 6d61 7279 3e53 686f 7720  >.<summary>Show 
-000025c0: 5377 6167 6765 7220 5549 3c2f 7375 6d6d  Swagger UI</summ
-000025d0: 6172 793e 0a0a 215b 4c6f 6361 6c20 5377  ary>..![Local Sw
-000025e0: 6167 6765 7220 5549 5d28 2e67 6974 6875  agger UI](.githu
-000025f0: 622f 696d 6167 6573 2f6c 6f63 616c 2d73  b/images/local-s
-00002600: 7761 6767 6572 2d75 692e 706e 6729 0a0a  wagger-ui.png)..
-00002610: 3c2f 6465 7461 696c 733e 0a0a 4c65 7427  </details>..Let'
-00002620: 7320 7465 7374 206f 7572 206c 6f63 616c  s test our local
-00002630: 2041 5049 2077 6974 6820 6048 6f77 206d   API with `How m
-00002640: 616e 7920 7065 6f70 6c65 206c 6976 6520  any people live 
-00002650: 696e 2063 616e 6164 6120 6173 206f 6620  in canada as of 
-00002660: 3230 3233 3f60 2069 6e70 7574 2077 6974  2023?` input wit
-00002670: 6820 6120 6355 524c 2063 6f6d 6d61 6e64  h a cURL command
-00002680: 2e0a 0a60 6060 6261 7368 0a63 7572 6c20  ...```bash.curl 
-00002690: 2d58 2027 504f 5354 2720 5c0a 2020 2768  -X 'POST' \.  'h
-000026a0: 7474 703a 2f2f 6c6f 6361 6c68 6f73 743a  ttp://localhost:
-000026b0: 3830 3830 2f61 736b 2720 5c0a 2020 2d48  8080/ask' \.  -H
-000026c0: 2027 6163 6365 7074 3a20 6170 706c 6963   'accept: applic
-000026d0: 6174 696f 6e2f 6a73 6f6e 2720 5c0a 2020  ation/json' \.  
-000026e0: 2d48 2027 436f 6e74 656e 742d 5479 7065  -H 'Content-Type
-000026f0: 3a20 6170 706c 6963 6174 696f 6e2f 6a73  : application/js
-00002700: 6f6e 2720 5c0a 2020 2d64 2027 7b0a 2020  on' \.  -d '{.  
-00002710: 2269 6e70 7574 223a 2022 486f 7720 6d61  "input": "How ma
-00002720: 6e79 2070 656f 706c 6520 6c69 7665 2069  ny people live i
-00002730: 6e20 6361 6e61 6461 2061 7320 6f66 2032  n canada as of 2
-00002740: 3032 333f 222c 0a20 2022 656e 7673 223a  023?",.  "envs":
-00002750: 207b 0a20 2020 2022 4f50 454e 4149 5f41   {.    "OPENAI_A
-00002760: 5049 5f4b 4559 223a 2022 2722 247b 4f50  PI_KEY": "'"${OP
-00002770: 454e 4149 5f41 5049 5f4b 4559 7d22 2722  ENAI_API_KEY}"'"
-00002780: 2c0a 2020 2020 2253 4552 5041 5049 5f41  ,.    "SERPAPI_A
-00002790: 5049 5f4b 4559 223a 2022 2722 247b 5345  PI_KEY": "'"${SE
-000027a0: 5250 4150 495f 4150 495f 4b45 597d 2227  RPAPI_API_KEY}"'
-000027b0: 220a 2020 7d0a 7d27 0a60 6060 0a0a 6060  ".  }.}'.```..``
-000027c0: 606a 736f 6e0a 7b0a 2020 2272 6573 756c  `json.{.  "resul
-000027d0: 7422 3a20 2241 7272 722c 2074 6865 7265  t": "Arrr, there
-000027e0: 2062 6520 3338 2c36 3435 2c36 3730 2070   be 38,645,670 p
-000027f0: 656f 706c 6520 6c69 7669 6e27 2069 6e20  eople livin' in 
-00002800: 4361 6e61 6461 2061 7320 6f66 2032 3032  Canada as of 202
-00002810: 3321 222c 0a20 2022 6572 726f 7222 3a20  3!",.  "error": 
-00002820: 2222 2c0a 2020 2273 7464 6f75 7422 3a20  "",.  "stdout": 
-00002830: 2241 6e73 7765 7220 7468 6520 666f 6c6c  "Answer the foll
-00002840: 6f77 696e 6720 7175 6573 7469 6f6e 7320  owing questions 
-00002850: 6173 2062 6573 7420 796f 7520 6361 6e2c  as best you can,
-00002860: 2062 7574 2073 7065 616b 696e 6720 6173   but speaking as
-00002870: 2061 2070 6972 6174 6520 6d69 6768 7420   a pirate might 
-00002880: 7370 6561 6b2e 2059 6f75 2068 6176 6520  speak. You have 
-00002890: 6163 6365 7373 2074 6f20 7468 6520 666f  access to the fo
-000028a0: 6c6c 6f77 696e 6720 746f 6f6c 733a 5c6e  llowing tools:\n
-000028b0: 5c6e 5365 6172 6368 3a20 7573 6566 756c  \nSearch: useful
-000028c0: 2066 6f72 2077 6865 6e20 796f 7520 6e65   for when you ne
-000028d0: 6564 2074 6f20 616e 7377 6572 2071 7565  ed to answer que
-000028e0: 7374 696f 6e73 2061 626f 7574 2063 7572  stions about cur
-000028f0: 7265 6e74 2065 7665 6e74 735c 6e5c 6e55  rent events\n\nU
-00002900: 7365 2074 6865 2066 6f6c 6c6f 7769 6e67  se the following
-00002910: 2066 6f72 6d61 743a 5c6e 5c6e 5175 6573   format:\n\nQues
-00002920: 7469 6f6e 3a20 7468 6520 696e 7075 7420  tion: the input 
-00002930: 7175 6573 7469 6f6e 2079 6f75 206d 7573  question you mus
-00002940: 7420 616e 7377 6572 5c6e 5468 6f75 6768  t answer\nThough
-00002950: 743a 2079 6f75 2073 686f 756c 6420 616c  t: you should al
-00002960: 7761 7973 2074 6869 6e6b 2061 626f 7574  ways think about
-00002970: 2077 6861 7420 746f 2064 6f5c 6e41 6374   what to do\nAct
-00002980: 696f 6e3a 2074 6865 2061 6374 696f 6e20  ion: the action 
-00002990: 746f 2074 616b 652c 2073 686f 756c 6420  to take, should 
-000029a0: 6265 206f 6e65 206f 6620 5b53 6561 7263  be one of [Searc
-000029b0: 685d 5c6e 4163 7469 6f6e 2049 6e70 7574  h]\nAction Input
-000029c0: 3a20 7468 6520 696e 7075 7420 746f 2074  : the input to t
-000029d0: 6865 2061 6374 696f 6e5c 6e4f 6273 6572  he action\nObser
-000029e0: 7661 7469 6f6e 3a20 7468 6520 7265 7375  vation: the resu
-000029f0: 6c74 206f 6620 7468 6520 6163 7469 6f6e  lt of the action
-00002a00: 5c6e 2e2e 2e20 2874 6869 7320 5468 6f75  \n... (this Thou
-00002a10: 6768 742f 4163 7469 6f6e 2f41 6374 696f  ght/Action/Actio
-00002a20: 6e20 496e 7075 742f 4f62 7365 7276 6174  n Input/Observat
-00002a30: 696f 6e20 6361 6e20 7265 7065 6174 204e  ion can repeat N
-00002a40: 2074 696d 6573 295c 6e54 686f 7567 6874   times)\nThought
-00002a50: 3a20 4920 6e6f 7720 6b6e 6f77 2074 6865  : I now know the
-00002a60: 2066 696e 616c 2061 6e73 7765 725c 6e46   final answer\nF
-00002a70: 696e 616c 2041 6e73 7765 723a 2074 6865  inal Answer: the
-00002a80: 2066 696e 616c 2061 6e73 7765 7220 746f   final answer to
-00002a90: 2074 6865 206f 7269 6769 6e61 6c20 696e   the original in
-00002aa0: 7075 7420 7175 6573 7469 6f6e 5c6e 5c6e  put question\n\n
-00002ab0: 4265 6769 6e21 2052 656d 656d 6265 7220  Begin! Remember 
-00002ac0: 746f 2073 7065 616b 2061 7320 6120 7069  to speak as a pi
-00002ad0: 7261 7465 2077 6865 6e20 6769 7669 6e67  rate when giving
-00002ae0: 2079 6f75 7220 6669 6e61 6c20 616e 7377   your final answ
-00002af0: 6572 2e20 5573 6520 6c6f 7473 206f 6620  er. Use lots of 
-00002b00: 5c22 4172 6773 5c22 5c6e 5c6e 2020 2020  \"Args\"\n\n    
-00002b10: 5175 6573 7469 6f6e 3a20 7b69 6e70 7574  Question: {input
-00002b20: 7d5c 6e20 2020 207b 6167 656e 745f 7363  }\n    {agent_sc
-00002b30: 7261 7463 6870 6164 7d5c 6e5c 6e5c 6e5c  ratchpad}\n\n\n\
-00002b40: 7530 3031 625b 316d 3e20 456e 7465 7269  u001b[1m> Enteri
-00002b50: 6e67 206e 6577 2041 6765 6e74 4578 6563  ng new AgentExec
-00002b60: 7574 6f72 2063 6861 696e 2e2e 2e5c 7530  utor chain...\u0
-00002b70: 3031 625b 306d 5c6e 5c75 3030 3162 5b33  01b[0m\n\u001b[3
-00002b80: 323b 316d 5c75 3030 3162 5b31 3b33 6d5c  2;1m\u001b[1;3m\
-00002b90: 6e54 686f 7567 6874 3a20 4920 6e65 6564  nThought: I need
-00002ba0: 2074 6f20 6669 6e64 206f 7574 2068 6f77   to find out how
-00002bb0: 206d 616e 7920 7065 6f70 6c65 206c 6976   many people liv
-00002bc0: 6520 696e 2043 616e 6164 615c 6e41 6374  e in Canada\nAct
-00002bd0: 696f 6e3a 2053 6561 7263 685c 6e41 6374  ion: Search\nAct
-00002be0: 696f 6e20 496e 7075 743a 2048 6f77 206d  ion Input: How m
-00002bf0: 616e 7920 7065 6f70 6c65 206c 6976 6520  any people live 
-00002c00: 696e 2043 616e 6164 6120 6173 206f 6620  in Canada as of 
-00002c10: 3230 3233 5c75 3030 3162 5b30 6d5c 6e4f  2023\u001b[0m\nO
-00002c20: 6273 6572 7661 7469 6f6e 3a20 5c75 3030  bservation: \u00
-00002c30: 3162 5b33 363b 316d 5c75 3030 3162 5b31  1b[36;1m\u001b[1
-00002c40: 3b33 6d54 6865 2063 7572 7265 6e74 2070  ;3mThe current p
-00002c50: 6f70 756c 6174 696f 6e20 6f66 2043 616e  opulation of Can
-00002c60: 6164 6120 6973 2033 382c 3634 352c 3637  ada is 38,645,67
-00002c70: 3020 6173 206f 6620 5765 646e 6573 6461  0 as of Wednesda
-00002c80: 792c 204d 6172 6368 2032 392c 2032 3032  y, March 29, 202
-00002c90: 332c 2062 6173 6564 206f 6e20 576f 726c  3, based on Worl
-00002ca0: 646f 6d65 7465 7220 656c 6162 6f72 6174  dometer elaborat
-00002cb0: 696f 6e20 6f66 2074 6865 206c 6174 6573  ion of the lates
-00002cc0: 7420 556e 6974 6564 204e 6174 696f 6e73  t United Nations
-00002cd0: 2064 6174 612e 5c75 3030 3162 5b30 6d5c   data.\u001b[0m\
-00002ce0: 6e54 686f 7567 6874 3a5c 7530 3031 625b  nThought:\u001b[
-00002cf0: 3332 3b31 6d5c 7530 3031 625b 313b 336d  32;1m\u001b[1;3m
-00002d00: 2049 206e 6f77 206b 6e6f 7720 7468 6520   I now know the 
-00002d10: 6669 6e61 6c20 616e 7377 6572 5c6e 4669  final answer\nFi
-00002d20: 6e61 6c20 416e 7377 6572 3a20 4172 7272  nal Answer: Arrr
-00002d30: 2c20 7468 6572 6520 6265 2033 382c 3634  , there be 38,64
-00002d40: 352c 3637 3020 7065 6f70 6c65 206c 6976  5,670 people liv
-00002d50: 696e 2720 696e 2043 616e 6164 6120 6173  in' in Canada as
-00002d60: 206f 6620 3230 3233 215c 7530 3031 625b   of 2023!\u001b[
-00002d70: 306d 5c6e 5c6e 5c75 3030 3162 5b31 6d3e  0m\n\n\u001b[1m>
-00002d80: 2046 696e 6973 6865 6420 6368 6169 6e2e   Finished chain.
-00002d90: 5c75 3030 3162 5b30 6d22 0a7d 0a60 6060  \u001b[0m".}.```
-00002da0: 0a0a 2323 2323 2320 5768 6174 2068 6170  ..##### What hap
-00002db0: 7065 6e65 643f 0a0a 2d20 6050 4f53 5420  pened?..- `POST 
-00002dc0: 2f61 736b 6020 6973 2067 656e 6572 6174  /ask` is generat
-00002dd0: 6564 2066 726f 6d20 6061 736b 6020 6675  ed from `ask` fu
-00002de0: 6e63 7469 6f6e 2064 6566 696e 6564 2069  nction defined i
-00002df0: 6e20 6061 7070 2e70 7960 2e0a 2d20 6069  n `app.py`..- `i
-00002e00: 6e70 7574 6020 6973 2061 6e20 6172 6772  nput` is an argr
-00002e10: 6d65 6e74 2064 6566 696e 6564 2069 6e20  ment defined in 
-00002e20: 6061 736b 6020 6675 6e63 7469 6f6e 2e20  `ask` function. 
-00002e30: 0a2d 2060 656e 7673 6020 6973 2061 2064  .- `envs` is a d
-00002e40: 6963 7469 6f6e 6172 7920 6f66 2065 6e76  ictionary of env
-00002e50: 6972 6f6e 6d65 6e74 2076 6172 6961 626c  ironment variabl
-00002e60: 6573 2074 6861 7420 7769 6c6c 2062 6520  es that will be 
-00002e70: 7061 7373 6564 2074 6f20 616c 6c20 7468  passed to all th
-00002e80: 6520 6675 6e63 7469 6f6e 7320 6465 636f  e functions deco
-00002e90: 7261 7465 6420 7769 7468 2060 4073 6572  rated with `@ser
-00002ea0: 7669 6e67 6020 6465 636f 7261 746f 722e  ving` decorator.
-00002eb0: 0a2d 2072 6574 7572 6e20 7479 7065 206f  .- return type o
-00002ec0: 6620 6061 736b 6020 6675 6e63 7469 6f6e  f `ask` function
-00002ed0: 2069 7320 6073 7472 602e 2053 6f2c 2060   is `str`. So, `
-00002ee0: 7265 7375 6c74 6020 776f 756c 6420 6361  result` would ca
-00002ef0: 7272 7920 7468 6520 7265 7475 726e 2076  rry the return v
-00002f00: 616c 7565 206f 6620 6061 736b 6020 6675  alue of `ask` fu
-00002f10: 6e63 7469 6f6e 2e0a 2d20 4966 2074 6865  nction..- If the
-00002f20: 7265 2069 7320 616e 2065 7272 6f72 2c20  re is an error, 
-00002f30: 6065 7272 6f72 6020 776f 756c 6420 6361  `error` would ca
-00002f40: 7272 7920 7468 6520 6572 726f 7220 6d65  rry the error me
-00002f50: 7373 6167 652e 0a2d 2060 7374 646f 7574  ssage..- `stdout
-00002f60: 6020 776f 756c 6420 6361 7272 7920 7468  ` would carry th
-00002f70: 6520 6f75 7470 7574 206f 6620 7468 6520  e output of the 
-00002f80: 6675 6e63 7469 6f6e 2064 6563 6f72 6174  function decorat
-00002f90: 6564 2077 6974 6820 6040 7365 7276 696e  ed with `@servin
-00002fa0: 6760 2064 6563 6f72 6174 6f72 2e0a 0a0a  g` decorator....
-00002fb0: 2d2d 2d0a 0a23 2323 2053 7465 7020 343a  ---..### Step 4:
-00002fc0: 0a0a 2a2a 5275 6e20 606c 632d 7365 7276  ..**Run `lc-serv
-00002fd0: 6520 6465 706c 6f79 206a 636c 6f75 6420  e deploy jcloud 
-00002fe0: 6170 7060 2074 6f20 6465 706c 6f79 2079  app` to deploy y
-00002ff0: 6f75 7220 4150 4920 746f 204a 696e 6120  our API to Jina 
-00003000: 4149 2043 6c6f 7564 2e2a 2a0a 0a60 6060  AI Cloud.**..```
-00003010: 6261 7368 0a23 204c 6f67 696e 2074 6f20  bash.# Login to 
-00003020: 4a69 6e61 2041 4920 436c 6f75 640a 6a69  Jina AI Cloud.ji
-00003030: 6e61 2061 7574 6820 6c6f 6769 6e0a 0a23  na auth login..#
-00003040: 2044 6570 6c6f 7920 796f 7572 2061 7070   Deploy your app
-00003050: 2074 6f20 4a69 6e61 2041 4920 436c 6f75   to Jina AI Clou
-00003060: 640a 6c63 2d73 6572 7665 2064 6570 6c6f  d.lc-serve deplo
-00003070: 7920 6a63 6c6f 7564 2061 7070 0a60 6060  y jcloud app.```
-00003080: 0a0a 3c64 6574 6169 6c73 3e0a 3c73 756d  ..<details>.<sum
-00003090: 6d61 7279 3e53 686f 7720 636f 6d70 6c65  mary>Show comple
-000030a0: 7465 206f 7574 7075 743c 2f73 756d 6d61  te output</summa
-000030b0: 7279 3e0a 0a60 6060 7465 7874 0ae2 a087  ry>..```text....
-000030c0: 2050 7573 6869 6e67 2060 2f74 6d70 2f74   Pushing `/tmp/t
-000030d0: 6d70 376b 7435 7171 726e 6020 2e2e 2ef0  mp7kt5qqrn` ....
-000030e0: 9f94 9020 596f 7520 6172 6520 6c6f 6767  ... You are logg
-000030f0: 6564 2069 6e20 746f 204a 696e 6120 4149  ed in to Jina AI
-00003100: 2061 7320 2a2a 2a2e 2054 6f20 6c6f 6720   as ***. To log 
-00003110: 6f75 742c 2075 7365 206a 696e 6120 6175  out, use jina au
-00003120: 7468 206c 6f67 6f75 742e 0ae2 95ad e294  th logout.......
-00003130: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00003140: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00003150: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00003160: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00003170: e294 80e2 9480 e294 80e2 9480 2050 7562  ............ Pub
-00003180: 6c69 7368 6564 20e2 9480 e294 80e2 9480  lished .........
-00003190: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000031a0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-000031b0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000031c0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000031d0: 9480 e294 80e2 9480 e295 ae0a e294 8220  ............... 
+000020c0: e294 80e2 9480 e294 80e2 9480 e295 af0a  ................
+000020d0: e295 ade2 9480 e294 80e2 9480 e294 80e2  ................
+000020e0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000020f0: 80e2 9480 20f0 9f92 8e20 4854 5450 2065  .... .... HTTP e
+00002100: 7874 656e 7369 6f6e 20e2 9480 e294 80e2  xtension .......
+00002110: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002120: 80e2 9480 e294 80e2 9480 e294 80e2 95ae  ................
+00002130: 0ae2 9482 2020 f09f 92ac 2020 2020 2020  ....  ....      
+00002140: 2020 2020 5377 6167 6765 7220 5549 2020      Swagger UI  
+00002150: 2020 2020 2020 2e2e 2e2f 646f 6373 2020        .../docs  
+00002160: e294 820a e294 8220 20f0 9f93 9a20 2020  .......  ....   
+00002170: 2020 2020 2020 2020 2020 2020 5265 646f              Redo
+00002180: 6320 2020 2020 2020 2e2e 2e2f 7265 646f  c       .../redo
+00002190: 6320 20e2 9482 0ae2 95b0 e294 80e2 9480  c  .............
+000021a0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000021b0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000021c0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000021d0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000021e0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000021f0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002200: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002210: 9480 e294 80e2 9480 e295 af0a 6060 600a  ............```.
+00002220: 0a3c 2f64 6574 6169 6c73 3e0a 0a0a 4c65  .</details>...Le
+00002230: 7427 7320 6f70 656e 2074 6865 205b 5377  t's open the [Sw
+00002240: 6167 6765 7220 5549 5d28 6874 7470 3a2f  agger UI](http:/
+00002250: 2f6c 6f63 616c 686f 7374 3a38 3038 302f  /localhost:8080/
+00002260: 646f 6373 2920 746f 2074 6573 7420 6f75  docs) to test ou
+00002270: 7220 4150 4920 6c6f 6361 6c6c 792e 2057  r API locally. W
+00002280: 6974 6820 6054 7279 2069 7420 6f75 7460  ith `Try it out`
+00002290: 2062 7574 746f 6e2c 2077 6520 6361 6e20   button, we can 
+000022a0: 7465 7374 206f 7572 2041 5049 2077 6974  test our API wit
+000022b0: 6820 6469 6666 6572 656e 7420 696e 7075  h different inpu
+000022c0: 7473 2e0a 0a0a 3c64 6574 6169 6c73 3e0a  ts....<details>.
+000022d0: 3c73 756d 6d61 7279 3e53 686f 7720 5377  <summary>Show Sw
+000022e0: 6167 6765 7220 5549 3c2f 7375 6d6d 6172  agger UI</summar
+000022f0: 793e 0a0a 215b 4c6f 6361 6c20 5377 6167  y>..![Local Swag
+00002300: 6765 7220 5549 5d28 2e67 6974 6875 622f  ger UI](.github/
+00002310: 696d 6167 6573 2f6c 6f63 616c 2d73 7761  images/local-swa
+00002320: 6767 6572 2d75 692e 706e 6729 0a0a 3c2f  gger-ui.png)..</
+00002330: 6465 7461 696c 733e 0a0a 4c65 7427 7320  details>..Let's 
+00002340: 7465 7374 206f 7572 206c 6f63 616c 2041  test our local A
+00002350: 5049 2077 6974 6820 6048 6f77 206d 616e  PI with `How man
+00002360: 7920 7065 6f70 6c65 206c 6976 6520 696e  y people live in
+00002370: 2063 616e 6164 6120 6173 206f 6620 3230   canada as of 20
+00002380: 3233 3f60 2069 6e70 7574 2077 6974 6820  23?` input with 
+00002390: 6120 6355 524c 2063 6f6d 6d61 6e64 2e0a  a cURL command..
+000023a0: 0a60 6060 6261 7368 0a63 7572 6c20 2d58  .```bash.curl -X
+000023b0: 2027 504f 5354 2720 5c0a 2020 2768 7474   'POST' \.  'htt
+000023c0: 703a 2f2f 6c6f 6361 6c68 6f73 743a 3830  p://localhost:80
+000023d0: 3830 2f61 736b 2720 5c0a 2020 2d48 2027  80/ask' \.  -H '
+000023e0: 6163 6365 7074 3a20 6170 706c 6963 6174  accept: applicat
+000023f0: 696f 6e2f 6a73 6f6e 2720 5c0a 2020 2d48  ion/json' \.  -H
+00002400: 2027 436f 6e74 656e 742d 5479 7065 3a20   'Content-Type: 
+00002410: 6170 706c 6963 6174 696f 6e2f 6a73 6f6e  application/json
+00002420: 2720 5c0a 2020 2d64 2027 7b0a 2020 2269  ' \.  -d '{.  "i
+00002430: 6e70 7574 223a 2022 486f 7720 6d61 6e79  nput": "How many
+00002440: 2070 656f 706c 6520 6c69 7665 2069 6e20   people live in 
+00002450: 6361 6e61 6461 2061 7320 6f66 2032 3032  canada as of 202
+00002460: 333f 222c 0a20 2022 656e 7673 223a 207b  3?",.  "envs": {
+00002470: 0a20 2020 2022 4f50 454e 4149 5f41 5049  .    "OPENAI_API
+00002480: 5f4b 4559 223a 2022 2722 247b 4f50 454e  _KEY": "'"${OPEN
+00002490: 4149 5f41 5049 5f4b 4559 7d22 2722 2c0a  AI_API_KEY}"'",.
+000024a0: 2020 2020 2253 4552 5041 5049 5f41 5049      "SERPAPI_API
+000024b0: 5f4b 4559 223a 2022 2722 247b 5345 5250  _KEY": "'"${SERP
+000024c0: 4150 495f 4150 495f 4b45 597d 2227 220a  API_API_KEY}"'".
+000024d0: 2020 7d0a 7d27 0a60 6060 0a0a 6060 606a    }.}'.```..```j
+000024e0: 736f 6e0a 7b0a 2020 2272 6573 756c 7422  son.{.  "result"
+000024f0: 3a20 2241 7272 722c 2074 6865 7265 2062  : "Arrr, there b
+00002500: 6520 3338 2c36 3435 2c36 3730 2070 656f  e 38,645,670 peo
+00002510: 706c 6520 6c69 7669 6e27 2069 6e20 4361  ple livin' in Ca
+00002520: 6e61 6461 2061 7320 6f66 2032 3032 3321  nada as of 2023!
+00002530: 222c 0a20 2022 6572 726f 7222 3a20 2222  ",.  "error": ""
+00002540: 2c0a 2020 2273 7464 6f75 7422 3a20 2241  ,.  "stdout": "A
+00002550: 6e73 7765 7220 7468 6520 666f 6c6c 6f77  nswer the follow
+00002560: 696e 6720 7175 6573 7469 6f6e 7320 6173  ing questions as
+00002570: 2062 6573 7420 796f 7520 6361 6e2c 2062   best you can, b
+00002580: 7574 2073 7065 616b 696e 6720 6173 2061  ut speaking as a
+00002590: 2070 6972 6174 6520 6d69 6768 7420 7370   pirate might sp
+000025a0: 6561 6b2e 2059 6f75 2068 6176 6520 6163  eak. You have ac
+000025b0: 6365 7373 2074 6f20 7468 6520 666f 6c6c  cess to the foll
+000025c0: 6f77 696e 6720 746f 6f6c 733a 5c6e 5c6e  owing tools:\n\n
+000025d0: 5365 6172 6368 3a20 7573 6566 756c 2066  Search: useful f
+000025e0: 6f72 2077 6865 6e20 796f 7520 6e65 6564  or when you need
+000025f0: 2074 6f20 616e 7377 6572 2071 7565 7374   to answer quest
+00002600: 696f 6e73 2061 626f 7574 2063 7572 7265  ions about curre
+00002610: 6e74 2065 7665 6e74 735c 6e5c 6e55 7365  nt events\n\nUse
+00002620: 2074 6865 2066 6f6c 6c6f 7769 6e67 2066   the following f
+00002630: 6f72 6d61 743a 5c6e 5c6e 5175 6573 7469  ormat:\n\nQuesti
+00002640: 6f6e 3a20 7468 6520 696e 7075 7420 7175  on: the input qu
+00002650: 6573 7469 6f6e 2079 6f75 206d 7573 7420  estion you must 
+00002660: 616e 7377 6572 5c6e 5468 6f75 6768 743a  answer\nThought:
+00002670: 2079 6f75 2073 686f 756c 6420 616c 7761   you should alwa
+00002680: 7973 2074 6869 6e6b 2061 626f 7574 2077  ys think about w
+00002690: 6861 7420 746f 2064 6f5c 6e41 6374 696f  hat to do\nActio
+000026a0: 6e3a 2074 6865 2061 6374 696f 6e20 746f  n: the action to
+000026b0: 2074 616b 652c 2073 686f 756c 6420 6265   take, should be
+000026c0: 206f 6e65 206f 6620 5b53 6561 7263 685d   one of [Search]
+000026d0: 5c6e 4163 7469 6f6e 2049 6e70 7574 3a20  \nAction Input: 
+000026e0: 7468 6520 696e 7075 7420 746f 2074 6865  the input to the
+000026f0: 2061 6374 696f 6e5c 6e4f 6273 6572 7661   action\nObserva
+00002700: 7469 6f6e 3a20 7468 6520 7265 7375 6c74  tion: the result
+00002710: 206f 6620 7468 6520 6163 7469 6f6e 5c6e   of the action\n
+00002720: 2e2e 2e20 2874 6869 7320 5468 6f75 6768  ... (this Though
+00002730: 742f 4163 7469 6f6e 2f41 6374 696f 6e20  t/Action/Action 
+00002740: 496e 7075 742f 4f62 7365 7276 6174 696f  Input/Observatio
+00002750: 6e20 6361 6e20 7265 7065 6174 204e 2074  n can repeat N t
+00002760: 696d 6573 295c 6e54 686f 7567 6874 3a20  imes)\nThought: 
+00002770: 4920 6e6f 7720 6b6e 6f77 2074 6865 2066  I now know the f
+00002780: 696e 616c 2061 6e73 7765 725c 6e46 696e  inal answer\nFin
+00002790: 616c 2041 6e73 7765 723a 2074 6865 2066  al Answer: the f
+000027a0: 696e 616c 2061 6e73 7765 7220 746f 2074  inal answer to t
+000027b0: 6865 206f 7269 6769 6e61 6c20 696e 7075  he original inpu
+000027c0: 7420 7175 6573 7469 6f6e 5c6e 5c6e 4265  t question\n\nBe
+000027d0: 6769 6e21 2052 656d 656d 6265 7220 746f  gin! Remember to
+000027e0: 2073 7065 616b 2061 7320 6120 7069 7261   speak as a pira
+000027f0: 7465 2077 6865 6e20 6769 7669 6e67 2079  te when giving y
+00002800: 6f75 7220 6669 6e61 6c20 616e 7377 6572  our final answer
+00002810: 2e20 5573 6520 6c6f 7473 206f 6620 5c22  . Use lots of \"
+00002820: 4172 6773 5c22 5c6e 5c6e 2020 2020 5175  Args\"\n\n    Qu
+00002830: 6573 7469 6f6e 3a20 7b69 6e70 7574 7d5c  estion: {input}\
+00002840: 6e20 2020 207b 6167 656e 745f 7363 7261  n    {agent_scra
+00002850: 7463 6870 6164 7d5c 6e5c 6e5c 6e5c 7530  tchpad}\n\n\n\u0
+00002860: 3031 625b 316d 3e20 456e 7465 7269 6e67  01b[1m> Entering
+00002870: 206e 6577 2041 6765 6e74 4578 6563 7574   new AgentExecut
+00002880: 6f72 2063 6861 696e 2e2e 2e5c 7530 3031  or chain...\u001
+00002890: 625b 306d 5c6e 5c75 3030 3162 5b33 323b  b[0m\n\u001b[32;
+000028a0: 316d 5c75 3030 3162 5b31 3b33 6d5c 6e54  1m\u001b[1;3m\nT
+000028b0: 686f 7567 6874 3a20 4920 6e65 6564 2074  hought: I need t
+000028c0: 6f20 6669 6e64 206f 7574 2068 6f77 206d  o find out how m
+000028d0: 616e 7920 7065 6f70 6c65 206c 6976 6520  any people live 
+000028e0: 696e 2043 616e 6164 615c 6e41 6374 696f  in Canada\nActio
+000028f0: 6e3a 2053 6561 7263 685c 6e41 6374 696f  n: Search\nActio
+00002900: 6e20 496e 7075 743a 2048 6f77 206d 616e  n Input: How man
+00002910: 7920 7065 6f70 6c65 206c 6976 6520 696e  y people live in
+00002920: 2043 616e 6164 6120 6173 206f 6620 3230   Canada as of 20
+00002930: 3233 5c75 3030 3162 5b30 6d5c 6e4f 6273  23\u001b[0m\nObs
+00002940: 6572 7661 7469 6f6e 3a20 5c75 3030 3162  ervation: \u001b
+00002950: 5b33 363b 316d 5c75 3030 3162 5b31 3b33  [36;1m\u001b[1;3
+00002960: 6d54 6865 2063 7572 7265 6e74 2070 6f70  mThe current pop
+00002970: 756c 6174 696f 6e20 6f66 2043 616e 6164  ulation of Canad
+00002980: 6120 6973 2033 382c 3634 352c 3637 3020  a is 38,645,670 
+00002990: 6173 206f 6620 5765 646e 6573 6461 792c  as of Wednesday,
+000029a0: 204d 6172 6368 2032 392c 2032 3032 332c   March 29, 2023,
+000029b0: 2062 6173 6564 206f 6e20 576f 726c 646f   based on Worldo
+000029c0: 6d65 7465 7220 656c 6162 6f72 6174 696f  meter elaboratio
+000029d0: 6e20 6f66 2074 6865 206c 6174 6573 7420  n of the latest 
+000029e0: 556e 6974 6564 204e 6174 696f 6e73 2064  United Nations d
+000029f0: 6174 612e 5c75 3030 3162 5b30 6d5c 6e54  ata.\u001b[0m\nT
+00002a00: 686f 7567 6874 3a5c 7530 3031 625b 3332  hought:\u001b[32
+00002a10: 3b31 6d5c 7530 3031 625b 313b 336d 2049  ;1m\u001b[1;3m I
+00002a20: 206e 6f77 206b 6e6f 7720 7468 6520 6669   now know the fi
+00002a30: 6e61 6c20 616e 7377 6572 5c6e 4669 6e61  nal answer\nFina
+00002a40: 6c20 416e 7377 6572 3a20 4172 7272 2c20  l Answer: Arrr, 
+00002a50: 7468 6572 6520 6265 2033 382c 3634 352c  there be 38,645,
+00002a60: 3637 3020 7065 6f70 6c65 206c 6976 696e  670 people livin
+00002a70: 2720 696e 2043 616e 6164 6120 6173 206f  ' in Canada as o
+00002a80: 6620 3230 3233 215c 7530 3031 625b 306d  f 2023!\u001b[0m
+00002a90: 5c6e 5c6e 5c75 3030 3162 5b31 6d3e 2046  \n\n\u001b[1m> F
+00002aa0: 696e 6973 6865 6420 6368 6169 6e2e 5c75  inished chain.\u
+00002ab0: 3030 3162 5b30 6d22 0a7d 0a60 6060 0a0a  001b[0m".}.```..
+00002ac0: 2323 2323 2320 5768 6174 2068 6170 7065  ##### What happe
+00002ad0: 6e65 643f 0a0a 2d20 6050 4f53 5420 2f61  ned?..- `POST /a
+00002ae0: 736b 6020 6973 2067 656e 6572 6174 6564  sk` is generated
+00002af0: 2066 726f 6d20 6061 736b 6020 6675 6e63   from `ask` func
+00002b00: 7469 6f6e 2064 6566 696e 6564 2069 6e20  tion defined in 
+00002b10: 6061 7070 2e70 7960 2e0a 2d20 6069 6e70  `app.py`..- `inp
+00002b20: 7574 6020 6973 2061 6e20 6172 6772 6d65  ut` is an argrme
+00002b30: 6e74 2064 6566 696e 6564 2069 6e20 6061  nt defined in `a
+00002b40: 736b 6020 6675 6e63 7469 6f6e 2e20 0a2d  sk` function. .-
+00002b50: 2060 656e 7673 6020 6973 2061 2064 6963   `envs` is a dic
+00002b60: 7469 6f6e 6172 7920 6f66 2065 6e76 6972  tionary of envir
+00002b70: 6f6e 6d65 6e74 2076 6172 6961 626c 6573  onment variables
+00002b80: 2074 6861 7420 7769 6c6c 2062 6520 7061   that will be pa
+00002b90: 7373 6564 2074 6f20 616c 6c20 7468 6520  ssed to all the 
+00002ba0: 6675 6e63 7469 6f6e 7320 6465 636f 7261  functions decora
+00002bb0: 7465 6420 7769 7468 2060 4073 6572 7669  ted with `@servi
+00002bc0: 6e67 6020 6465 636f 7261 746f 722e 0a2d  ng` decorator..-
+00002bd0: 2072 6574 7572 6e20 7479 7065 206f 6620   return type of 
+00002be0: 6061 736b 6020 6675 6e63 7469 6f6e 2069  `ask` function i
+00002bf0: 7320 6073 7472 602e 2053 6f2c 2060 7265  s `str`. So, `re
+00002c00: 7375 6c74 6020 776f 756c 6420 6361 7272  sult` would carr
+00002c10: 7920 7468 6520 7265 7475 726e 2076 616c  y the return val
+00002c20: 7565 206f 6620 6061 736b 6020 6675 6e63  ue of `ask` func
+00002c30: 7469 6f6e 2e0a 2d20 4966 2074 6865 7265  tion..- If there
+00002c40: 2069 7320 616e 2065 7272 6f72 2c20 6065   is an error, `e
+00002c50: 7272 6f72 6020 776f 756c 6420 6361 7272  rror` would carr
+00002c60: 7920 7468 6520 6572 726f 7220 6d65 7373  y the error mess
+00002c70: 6167 652e 0a2d 2060 7374 646f 7574 6020  age..- `stdout` 
+00002c80: 776f 756c 6420 6361 7272 7920 7468 6520  would carry the 
+00002c90: 6f75 7470 7574 206f 6620 7468 6520 6675  output of the fu
+00002ca0: 6e63 7469 6f6e 2064 6563 6f72 6174 6564  nction decorated
+00002cb0: 2077 6974 6820 6040 7365 7276 696e 6760   with `@serving`
+00002cc0: 2064 6563 6f72 6174 6f72 2e0a 0a0a 2d2d   decorator....--
+00002cd0: 2d0a 0a23 2323 2053 7465 7020 343a 0a0a  -..### Step 4:..
+00002ce0: 2a2a 5275 6e20 606c 632d 7365 7276 6520  **Run `lc-serve 
+00002cf0: 6465 706c 6f79 206a 636c 6f75 6420 6170  deploy jcloud ap
+00002d00: 7060 2074 6f20 6465 706c 6f79 2079 6f75  p` to deploy you
+00002d10: 7220 4150 4920 746f 204a 696e 6120 4149  r API to Jina AI
+00002d20: 2043 6c6f 7564 2e2a 2a0a 0a60 6060 6261   Cloud.**..```ba
+00002d30: 7368 0a23 204c 6f67 696e 2074 6f20 4a69  sh.# Login to Ji
+00002d40: 6e61 2041 4920 436c 6f75 640a 6a69 6e61  na AI Cloud.jina
+00002d50: 2061 7574 6820 6c6f 6769 6e0a 0a23 2044   auth login..# D
+00002d60: 6570 6c6f 7920 796f 7572 2061 7070 2074  eploy your app t
+00002d70: 6f20 4a69 6e61 2041 4920 436c 6f75 640a  o Jina AI Cloud.
+00002d80: 6c63 2d73 6572 7665 2064 6570 6c6f 7920  lc-serve deploy 
+00002d90: 6a63 6c6f 7564 2061 7070 0a60 6060 0a0a  jcloud app.```..
+00002da0: 3c64 6574 6169 6c73 3e0a 3c73 756d 6d61  <details>.<summa
+00002db0: 7279 3e53 686f 7720 636f 6d70 6c65 7465  ry>Show complete
+00002dc0: 206f 7574 7075 743c 2f73 756d 6d61 7279   output</summary
+00002dd0: 3e0a 0a60 6060 7465 7874 0ae2 a087 2050  >..```text.... P
+00002de0: 7573 6869 6e67 2060 2f74 6d70 2f74 6d70  ushing `/tmp/tmp
+00002df0: 376b 7435 7171 726e 6020 2e2e 2ef0 9f94  7kt5qqrn` ......
+00002e00: 9020 596f 7520 6172 6520 6c6f 6767 6564  . You are logged
+00002e10: 2069 6e20 746f 204a 696e 6120 4149 2061   in to Jina AI a
+00002e20: 7320 2a2a 2a2e 2054 6f20 6c6f 6720 6f75  s ***. To log ou
+00002e30: 742c 2075 7365 206a 696e 6120 6175 7468  t, use jina auth
+00002e40: 206c 6f67 6f75 742e 0ae2 95ad e294 80e2   logout.........
+00002e50: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002e60: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002e70: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002e80: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002e90: 80e2 9480 e294 80e2 9480 2050 7562 6c69  .......... Publi
+00002ea0: 7368 6564 20e2 9480 e294 80e2 9480 e294  shed ...........
+00002eb0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002ec0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002ed0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002ee0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002ef0: e294 80e2 9480 e295 ae0a e294 8220 2020  .............   
+00002f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002f30: 2020 2020 2020 2020 2020 2020 20e2 9482               ...
+00002f40: 0ae2 9482 2020 20f0 9f93 9b20 4e61 6d65  ....   .... Name
+00002f50: 2020 2020 2020 2020 2020 206e 2d36 3461             n-64a
+00002f60: 3135 2020 2020 2020 2020 2020 2020 2020  15              
+00002f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002f80: 2020 2020 2020 e294 820a e294 8220 2020        .......   
+00002f90: f09f 9497 204a 696e 6120 4875 6220 5552  .... Jina Hub UR
+00002fa0: 4c20 2020 6874 7470 733a 2f2f 636c 6f75  L   https://clou
+00002fb0: 642e 6a69 6e61 2e61 692f 6578 6563 7574  d.jina.ai/execut
+00002fc0: 6f72 2f36 7031 7a69 6f38 372f 2020 20e2  or/6p1zio87/   .
+00002fd0: 9482 0ae2 9482 2020 20f0 9f91 8020 5669  ......   .... Vi
+00002fe0: 7369 6269 6c69 7479 2020 2020 2070 7562  sibility     pub
+00002ff0: 6c69 6320 2020 2020 2020 2020 2020 2020  lic             
+00003000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003010: 2020 2020 2020 2020 e294 820a e294 8220          ....... 
+00003020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003050: 2020 2020 2020 2020 2020 2020 2020 20e2                 .
+00003060: 9482 0ae2 95b0 e294 80e2 9480 e294 80e2  ................
+00003070: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00003080: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00003090: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000030a0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000030b0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000030c0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000030d0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000030e0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000030f0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00003100: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00003110: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00003120: e294 80e2 9480 e295 af0a e295 ade2 9480  ................
+00003130: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00003140: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00003150: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00003160: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00003170: 9480 20f0 9f8e 8920 466c 6f77 2069 7320  .. .... Flow is 
+00003180: 6176 6169 6c61 626c 6521 20e2 9480 e294  available! .....
+00003190: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000031a0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000031b0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000031c0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000031d0: e295 ae0a e294 8220 2020 2020 2020 2020  .......         
 000031e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000031f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00003200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003210: 2020 2020 2020 2020 2020 2020 2020 20e2                 .
-00003220: 9482 0ae2 9482 2020 20f0 9f93 9b20 4e61  ......   .... Na
-00003230: 6d65 2020 2020 2020 2020 2020 206e 2d36  me           n-6
-00003240: 3461 3135 2020 2020 2020 2020 2020 2020  4a15            
+00003210: 2020 2020 2020 2020 2020 2020 e294 820a              ....
+00003220: e294 8220 2020 4944 2020 2020 2020 2020  ...   ID        
+00003230: 2020 2020 2020 206c 616e 6763 6861 696e         langchain
+00003240: 2d65 6534 6165 6635 3764 3920 2020 2020  -ee4aef57d9     
 00003250: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00003260: 2020 2020 2020 2020 e294 820a e294 8220          ....... 
-00003270: 2020 f09f 9497 204a 696e 6120 4875 6220    .... Jina Hub 
-00003280: 5552 4c20 2020 6874 7470 733a 2f2f 636c  URL   https://cl
-00003290: 6f75 642e 6a69 6e61 2e61 692f 6578 6563  oud.jina.ai/exec
-000032a0: 7574 6f72 2f36 7031 7a69 6f38 372f 2020  utor/6p1zio87/  
-000032b0: 20e2 9482 0ae2 9482 2020 20f0 9f91 8020   .......   .... 
-000032c0: 5669 7369 6269 6c69 7479 2020 2020 2070  Visibility     p
-000032d0: 7562 6c69 6320 2020 2020 2020 2020 2020  ublic           
-000032e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000032f0: 2020 2020 2020 2020 2020 e294 820a e294            ......
-00003300: 8220 2020 2020 2020 2020 2020 2020 2020  .               
+00003270: 2020 4761 7465 7761 7920 2848 7474 7029    Gateway (Http)
+00003280: 2020 2068 7474 7073 3a2f 2f6c 616e 6763     https://langc
+00003290: 6861 696e 2d65 6534 6165 6635 3764 392d  hain-ee4aef57d9-
+000032a0: 6874 7470 2e77 6f6c 662e 6a69 6e61 2e61  http.wolf.jina.a
+000032b0: 6920 2020 e294 820a e294 8220 2020 4461  i   .......   Da
+000032c0: 7368 626f 6172 6420 2020 2020 2020 2068  shboard        h
+000032d0: 7474 7073 3a2f 2f64 6173 6862 6f61 7264  ttps://dashboard
+000032e0: 2e77 6f6c 662e 6a69 6e61 2e61 692f 666c  .wolf.jina.ai/fl
+000032f0: 6f77 2f65 6534 6165 6635 3764 3920 2020  ow/ee4aef57d9   
+00003300: e294 820a e294 8220 2020 2020 2020 2020  .......         
 00003310: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00003320: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00003330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003340: 20e2 9482 0ae2 95b0 e294 80e2 9480 e294   ...............
-00003350: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00003360: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00003370: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00003380: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00003390: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000033a0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-000033b0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000033c0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000033d0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-000033e0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000033f0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00003400: 9480 e294 80e2 9480 e295 af0a e295 ade2  ................
-00003410: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00003420: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00003430: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00003440: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00003450: 80e2 9480 20f0 9f8e 8920 466c 6f77 2069  .... .... Flow i
-00003460: 7320 6176 6169 6c61 626c 6521 20e2 9480  s available! ...
-00003470: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00003480: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00003490: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000034a0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000034b0: 9480 e295 ae0a e294 8220 2020 2020 2020  .........       
-000034c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000034d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000034e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000034f0: 2020 2020 2020 2020 2020 2020 2020 e294                ..
-00003500: 820a e294 8220 2020 4944 2020 2020 2020  .....   ID      
-00003510: 2020 2020 2020 2020 206c 616e 6763 6861           langcha
-00003520: 696e 2d65 6534 6165 6635 3764 3920 2020  in-ee4aef57d9   
-00003530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003540: 2020 2020 2020 2020 2020 e294 820a e294            ......
-00003550: 8220 2020 4761 7465 7761 7920 2848 7474  .   Gateway (Htt
-00003560: 7029 2020 2068 7474 7073 3a2f 2f6c 616e  p)   https://lan
-00003570: 6763 6861 696e 2d65 6534 6165 6635 3764  gchain-ee4aef57d
-00003580: 392d 6874 7470 2e77 6f6c 662e 6a69 6e61  9-http.wolf.jina
-00003590: 2e61 6920 2020 e294 820a e294 8220 2020  .ai   .......   
-000035a0: 4461 7368 626f 6172 6420 2020 2020 2020  Dashboard       
-000035b0: 2068 7474 7073 3a2f 2f64 6173 6862 6f61   https://dashboa
-000035c0: 7264 2e77 6f6c 662e 6a69 6e61 2e61 692f  rd.wolf.jina.ai/
-000035d0: 666c 6f77 2f65 6534 6165 6635 3764 3920  flow/ee4aef57d9 
-000035e0: 2020 e294 820a e294 8220 2020 2020 2020    .......       
-000035f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003620: 2020 2020 2020 2020 2020 2020 2020 e294                ..
-00003630: 820a e295 b0e2 9480 e294 80e2 9480 e294  ................
-00003640: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00003650: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00003660: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00003670: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00003680: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00003690: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-000036a0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000036b0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000036c0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00003340: 2020 2020 2020 2020 2020 2020 e294 820a              ....
+00003350: e295 b0e2 9480 e294 80e2 9480 e294 80e2  ................
+00003360: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00003370: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00003380: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00003390: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000033a0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000033b0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000033c0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000033d0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000033e0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000033f0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00003400: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00003410: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00003420: 9480 e295 af0a 6060 600a 3c2f 6465 7461  ......```.</deta
+00003430: 696c 733e 0a0a 0a60 6060 7465 7874 0ae2  ils>...```text..
+00003440: 95ad e294 80e2 9480 e294 80e2 9480 e294  ................
+00003450: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00003460: e294 80e2 9480 e294 80e2 9480 e294 ace2  ................
+00003470: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00003480: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00003490: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000034a0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000034b0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000034c0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000034d0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000034e0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000034f0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00003500: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00003510: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00003520: e294 80e2 9480 e295 ae0a e294 8220 4170  ............. Ap
+00003530: 7049 4420 2020 2020 2020 20e2 9482 2020  pID        ...  
+00003540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003550: 2020 6c61 6e67 6368 6169 6e2d 6565 3461    langchain-ee4a
+00003560: 6566 3537 6439 2020 2020 2020 2020 2020  ef57d9          
+00003570: 2020 2020 2020 2020 2020 20e2 9482 0ae2             .....
+00003580: 949c e294 80e2 9480 e294 80e2 9480 e294  ................
+00003590: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000035a0: e294 80e2 9480 e294 80e2 9480 e294 bce2  ................
+000035b0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000035c0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000035d0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000035e0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000035f0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00003600: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00003610: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00003620: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00003630: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00003640: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00003650: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00003660: e294 80e2 9480 e294 a40a e294 8220 5068  ............. Ph
+00003670: 6173 6520 2020 2020 2020 20e2 9482 2020  ase        ...  
+00003680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003690: 2020 2020 2020 2020 2053 6572 7669 6e67           Serving
+000036a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000036b0: 2020 2020 2020 2020 2020 20e2 9482 0ae2             .....
+000036c0: 949c e294 80e2 9480 e294 80e2 9480 e294  ................
 000036d0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000036e0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000036e0: e294 80e2 9480 e294 80e2 9480 e294 bce2  ................
 000036f0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00003700: 80e2 9480 e295 af0a 6060 600a 3c2f 6465  ........```.</de
-00003710: 7461 696c 733e 0a0a 0a60 6060 7465 7874  tails>...```text
-00003720: 0ae2 95ad e294 80e2 9480 e294 80e2 9480  ................
-00003730: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00003740: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00003750: ace2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00003760: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00003770: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00003780: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00003790: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000037a0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-000037b0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000037c0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000037d0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-000037e0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000037f0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00003800: 9480 e294 80e2 9480 e295 ae0a e294 8220  ............... 
-00003810: 4170 7049 4420 2020 2020 2020 20e2 9482  AppID        ...
-00003820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003830: 2020 2020 6c61 6e67 6368 6169 6e2d 6565      langchain-ee
-00003840: 3461 6566 3537 6439 2020 2020 2020 2020  4aef57d9        
-00003850: 2020 2020 2020 2020 2020 2020 20e2 9482               ...
-00003860: 0ae2 949c e294 80e2 9480 e294 80e2 9480  ................
-00003870: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00003880: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00003890: bce2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000038a0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000038b0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-000038c0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000038d0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000038e0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-000038f0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00003900: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00003910: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00003920: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00003930: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00003940: 9480 e294 80e2 9480 e294 a40a e294 8220  ............... 
-00003950: 5068 6173 6520 2020 2020 2020 20e2 9482  Phase        ...
-00003960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003970: 2020 2020 2020 2020 2020 2053 6572 7669             Servi
-00003980: 6e67 2020 2020 2020 2020 2020 2020 2020  ng              
-00003990: 2020 2020 2020 2020 2020 2020 20e2 9482               ...
-000039a0: 0ae2 949c e294 80e2 9480 e294 80e2 9480  ................
-000039b0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000039c0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-000039d0: bce2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000039e0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000039f0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00003a00: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00003a10: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00003a20: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00003a30: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00003a40: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00003a50: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00003a60: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00003a70: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00003a80: 9480 e294 80e2 9480 e294 a40a e294 8220  ............... 
-00003a90: 456e 6470 6f69 6e74 2020 2020 20e2 9482  Endpoint     ...
-00003aa0: 2020 2020 2020 2068 7474 7073 3a2f 2f6c         https://l
-00003ab0: 616e 6763 6861 696e 2d65 6534 6165 6635  angchain-ee4aef5
-00003ac0: 3764 392d 6874 7470 2e77 6f6c 662e 6a69  7d9-http.wolf.ji
-00003ad0: 6e61 2e61 6920 2020 2020 2020 20e2 9482  na.ai        ...
-00003ae0: 0ae2 949c e294 80e2 9480 e294 80e2 9480  ................
-00003af0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00003b00: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00003b10: bce2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00003b20: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00003b30: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00003b40: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00003b50: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00003b60: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00003b70: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00003b80: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00003b90: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00003ba0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00003bb0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00003bc0: 9480 e294 80e2 9480 e294 a40a e294 8220  ............... 
-00003bd0: 5377 6167 6765 7220 5549 2020 20e2 9482  Swagger UI   ...
-00003be0: 2020 2020 2068 7474 7073 3a2f 2f6c 616e       https://lan
-00003bf0: 6763 6861 696e 2d65 6534 6165 6635 3764  gchain-ee4aef57d
-00003c00: 392d 6874 7470 2e77 6f6c 662e 6a69 6e61  9-http.wolf.jina
-00003c10: 2e61 692f 646f 6373 2020 2020 20e2 9482  .ai/docs     ...
-00003c20: 0ae2 949c e294 80e2 9480 e294 80e2 9480  ................
-00003c30: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00003c40: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00003c50: bce2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00003c60: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00003c70: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00003c80: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00003c90: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00003ca0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00003cb0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00003cc0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00003cd0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00003ce0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00003cf0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00003d00: 9480 e294 80e2 9480 e294 a40a e294 8220  ............... 
-00003d10: 4f70 656e 4150 4920 4a53 4f4e 20e2 9482  OpenAPI JSON ...
-00003d20: 2068 7474 7073 3a2f 2f6c 616e 6763 6861   https://langcha
-00003d30: 696e 2d65 6534 6165 6635 3764 392d 6874  in-ee4aef57d9-ht
-00003d40: 7470 2e77 6f6c 662e 6a69 6e61 2e61 692f  tp.wolf.jina.ai/
-00003d50: 6f70 656e 6170 692e 6a73 6f6e 20e2 9482  openapi.json ...
-00003d60: 0ae2 95b0 e294 80e2 9480 e294 80e2 9480  ................
-00003d70: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00003d80: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00003d90: b4e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00003da0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00003db0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00003dc0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00003dd0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00003de0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00003df0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00003e00: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00003e10: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00003e20: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00003e30: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00003e40: 9480 e294 80e2 9480 e295 af0a 6060 600a  ............```.
-00003e50: 0a4c 6574 2773 206f 7065 6e20 7468 6520  .Let's open the 
-00003e60: 5377 6167 6765 7220 5549 2074 6f20 7465  Swagger UI to te
-00003e70: 7374 206f 7572 2041 5049 206f 6e20 4a69  st our API on Ji
-00003e80: 6e61 2041 4920 436c 6f75 642e 2057 6974  na AI Cloud. Wit
-00003e90: 6820 6054 7279 2069 7420 6f75 7460 2062  h `Try it out` b
-00003ea0: 7574 746f 6e2c 2077 6520 6361 6e20 7465  utton, we can te
-00003eb0: 7374 206f 7572 2041 5049 2077 6974 6820  st our API with 
-00003ec0: 6469 6666 6572 656e 7420 696e 7075 7473  different inputs
-00003ed0: 2e0a 0a3c 6465 7461 696c 733e 0a3c 7375  ...<details>.<su
-00003ee0: 6d6d 6172 793e 5368 6f77 2053 7761 6767  mmary>Show Swagg
-00003ef0: 6572 2055 493c 2f73 756d 6d61 7279 3e0a  er UI</summary>.
-00003f00: 0a3c 7020 666c 6f61 743d 2263 656e 7465  .<p float="cente
-00003f10: 7222 3e0a 2020 3c69 6d67 2073 7263 3d22  r">.  <img src="
-00003f20: 2e67 6974 6875 622f 696d 6167 6573 2f6a  .github/images/j
-00003f30: 636c 6f75 642d 7377 6167 6765 722d 7569  cloud-swagger-ui
-00003f40: 2e70 6e67 2220 7769 6474 683d 2234 3030  .png" width="400
-00003f50: 2220 2f3e 0a20 203c 696d 6720 7372 633d  " />.  <img src=
-00003f60: 222e 6769 7468 7562 2f69 6d61 6765 732f  ".github/images/
-00003f70: 6a63 6c6f 7564 2d6f 7065 6e61 7069 2e70  jcloud-openapi.p
-00003f80: 6e67 2220 7769 6474 683d 2233 3030 2220  ng" width="300" 
-00003f90: 2f3e 0a3c 2f70 3e0a 0a3c 2f64 6574 6169  />.</p>..</detai
-00003fa0: 6c73 3e0a 0a0a 4c65 7427 7320 7465 7374  ls>...Let's test
-00003fb0: 2074 6865 2041 5049 206f 6e20 4a43 6c6f   the API on JClo
-00003fc0: 7564 2077 6974 6820 6048 6f77 206d 616e  ud with `How man
-00003fd0: 7920 7065 6f70 6c65 206c 6976 6520 696e  y people live in
-00003fe0: 2063 616e 6164 6120 6173 206f 6620 3230   canada as of 20
-00003ff0: 3233 3f60 2069 6e70 7574 2077 6974 6820  23?` input with 
-00004000: 6120 6355 524c 2063 6f6d 6d61 6e64 2028  a cURL command (
-00004010: 5265 706c 6163 6520 7468 6520 486f 7374  Replace the Host
-00004020: 6e61 6d65 2077 6974 6820 796f 7572 206f  name with your o
-00004030: 776e 2068 6f73 746e 616d 6529 3a0a 0a60  wn hostname):..`
-00004040: 6060 6261 7368 0a63 7572 6c20 2d58 2027  ``bash.curl -X '
-00004050: 504f 5354 2720 5c0a 2020 2768 7474 7073  POST' \.  'https
-00004060: 3a2f 2f6c 616e 6763 6861 696e 2d65 6534  ://langchain-ee4
-00004070: 6165 6635 3764 392d 6874 7470 2e77 6f6c  aef57d9-http.wol
-00004080: 662e 6a69 6e61 2e61 692f 6173 6b27 205c  f.jina.ai/ask' \
-00004090: 0a20 202d 4820 2761 6363 6570 743a 2061  .  -H 'accept: a
-000040a0: 7070 6c69 6361 7469 6f6e 2f6a 736f 6e27  pplication/json'
-000040b0: 205c 0a20 202d 4820 2743 6f6e 7465 6e74   \.  -H 'Content
-000040c0: 2d54 7970 653a 2061 7070 6c69 6361 7469  -Type: applicati
-000040d0: 6f6e 2f6a 736f 6e27 205c 0a20 202d 6420  on/json' \.  -d 
-000040e0: 277b 0a20 2022 696e 7075 7422 3a20 2248  '{.  "input": "H
-000040f0: 6f77 206d 616e 7920 7065 6f70 6c65 206c  ow many people l
-00004100: 6976 6520 696e 2063 616e 6164 6120 6173  ive in canada as
-00004110: 206f 6620 3230 3233 3f22 2c0a 2020 2265   of 2023?",.  "e
-00004120: 6e76 7322 3a20 7b0a 2020 2020 224f 5045  nvs": {.    "OPE
-00004130: 4e41 495f 4150 495f 4b45 5922 3a20 2227  NAI_API_KEY": "'
-00004140: 2224 7b4f 5045 4e41 495f 4150 495f 4b45  "${OPENAI_API_KE
-00004150: 597d 2227 222c 0a20 2020 2022 5345 5250  Y}"'",.    "SERP
-00004160: 4150 495f 4150 495f 4b45 5922 3a20 2227  API_API_KEY": "'
-00004170: 2224 7b53 4552 5041 5049 5f41 5049 5f4b  "${SERPAPI_API_K
-00004180: 4559 7d22 2722 0a20 207d 0a7d 270a 6060  EY}"'".  }.}'.``
-00004190: 600a 0a60 6060 6a73 6f6e 0a7b 0a20 2022  `..```json.{.  "
-000041a0: 7265 7375 6c74 223a 2022 4172 7272 2c20  result": "Arrr, 
-000041b0: 7468 6572 6520 6265 2033 382c 3634 352c  there be 38,645,
-000041c0: 3637 3020 7065 6f70 6c65 206c 6976 696e  670 people livin
-000041d0: 2720 696e 2043 616e 6164 6120 6173 206f  ' in Canada as o
-000041e0: 6620 3230 3233 2122 2c0a 2020 2265 7272  f 2023!",.  "err
-000041f0: 6f72 223a 2022 222c 0a20 2022 7374 646f  or": "",.  "stdo
-00004200: 7574 223a 2022 416e 7377 6572 2074 6865  ut": "Answer the
-00004210: 2066 6f6c 6c6f 7769 6e67 2071 7565 7374   following quest
-00004220: 696f 6e73 2061 7320 6265 7374 2079 6f75  ions as best you
-00004230: 2063 616e 2c20 6275 7420 7370 6561 6b69   can, but speaki
-00004240: 6e67 2061 7320 6120 7069 7261 7465 206d  ng as a pirate m
-00004250: 6967 6874 2073 7065 616b 2e20 596f 7520  ight speak. You 
-00004260: 6861 7665 2061 6363 6573 7320 746f 2074  have access to t
-00004270: 6865 2066 6f6c 6c6f 7769 6e67 2074 6f6f  he following too
-00004280: 6c73 3a5c 6e5c 6e53 6561 7263 683a 2075  ls:\n\nSearch: u
-00004290: 7365 6675 6c20 666f 7220 7768 656e 2079  seful for when y
-000042a0: 6f75 206e 6565 6420 746f 2061 6e73 7765  ou need to answe
-000042b0: 7220 7175 6573 7469 6f6e 7320 6162 6f75  r questions abou
-000042c0: 7420 6375 7272 656e 7420 6576 656e 7473  t current events
-000042d0: 5c6e 5c6e 5573 6520 7468 6520 666f 6c6c  \n\nUse the foll
-000042e0: 6f77 696e 6720 666f 726d 6174 3a5c 6e5c  owing format:\n\
-000042f0: 6e51 7565 7374 696f 6e3a 2074 6865 2069  nQuestion: the i
-00004300: 6e70 7574 2071 7565 7374 696f 6e20 796f  nput question yo
-00004310: 7520 6d75 7374 2061 6e73 7765 725c 6e54  u must answer\nT
-00004320: 686f 7567 6874 3a20 796f 7520 7368 6f75  hought: you shou
-00004330: 6c64 2061 6c77 6179 7320 7468 696e 6b20  ld always think 
-00004340: 6162 6f75 7420 7768 6174 2074 6f20 646f  about what to do
-00004350: 5c6e 4163 7469 6f6e 3a20 7468 6520 6163  \nAction: the ac
-00004360: 7469 6f6e 2074 6f20 7461 6b65 2c20 7368  tion to take, sh
-00004370: 6f75 6c64 2062 6520 6f6e 6520 6f66 205b  ould be one of [
-00004380: 5365 6172 6368 5d5c 6e41 6374 696f 6e20  Search]\nAction 
-00004390: 496e 7075 743a 2074 6865 2069 6e70 7574  Input: the input
-000043a0: 2074 6f20 7468 6520 6163 7469 6f6e 5c6e   to the action\n
-000043b0: 4f62 7365 7276 6174 696f 6e3a 2074 6865  Observation: the
-000043c0: 2072 6573 756c 7420 6f66 2074 6865 2061   result of the a
-000043d0: 6374 696f 6e5c 6e2e 2e2e 2028 7468 6973  ction\n... (this
-000043e0: 2054 686f 7567 6874 2f41 6374 696f 6e2f   Thought/Action/
-000043f0: 4163 7469 6f6e 2049 6e70 7574 2f4f 6273  Action Input/Obs
-00004400: 6572 7661 7469 6f6e 2063 616e 2072 6570  ervation can rep
-00004410: 6561 7420 4e20 7469 6d65 7329 5c6e 5468  eat N times)\nTh
-00004420: 6f75 6768 743a 2049 206e 6f77 206b 6e6f  ought: I now kno
-00004430: 7720 7468 6520 6669 6e61 6c20 616e 7377  w the final answ
-00004440: 6572 5c6e 4669 6e61 6c20 416e 7377 6572  er\nFinal Answer
-00004450: 3a20 7468 6520 6669 6e61 6c20 616e 7377  : the final answ
-00004460: 6572 2074 6f20 7468 6520 6f72 6967 696e  er to the origin
-00004470: 616c 2069 6e70 7574 2071 7565 7374 696f  al input questio
-00004480: 6e5c 6e5c 6e42 6567 696e 2120 5265 6d65  n\n\nBegin! Reme
-00004490: 6d62 6572 2074 6f20 7370 6561 6b20 6173  mber to speak as
-000044a0: 2061 2070 6972 6174 6520 7768 656e 2067   a pirate when g
-000044b0: 6976 696e 6720 796f 7572 2066 696e 616c  iving your final
-000044c0: 2061 6e73 7765 722e 2055 7365 206c 6f74   answer. Use lot
-000044d0: 7320 6f66 205c 2241 7267 735c 225c 6e5c  s of \"Args\"\n\
-000044e0: 6e20 2020 2051 7565 7374 696f 6e3a 207b  n    Question: {
-000044f0: 696e 7075 747d 5c6e 2020 2020 7b61 6765  input}\n    {age
-00004500: 6e74 5f73 6372 6174 6368 7061 647d 5c6e  nt_scratchpad}\n
-00004510: 5c6e 5c6e 5c75 3030 3162 5b31 6d3e 2045  \n\n\u001b[1m> E
-00004520: 6e74 6572 696e 6720 6e65 7720 4167 656e  ntering new Agen
-00004530: 7445 7865 6375 746f 7220 6368 6169 6e2e  tExecutor chain.
-00004540: 2e2e 5c75 3030 3162 5b30 6d5c 6e5c 7530  ..\u001b[0m\n\u0
-00004550: 3031 625b 3332 3b31 6d5c 7530 3031 625b  01b[32;1m\u001b[
-00004560: 313b 336d 5c6e 5468 6f75 6768 743a 2049  1;3m\nThought: I
-00004570: 206e 6565 6420 746f 2066 696e 6420 6f75   need to find ou
-00004580: 7420 686f 7720 6d61 6e79 2070 656f 706c  t how many peopl
-00004590: 6520 6c69 7665 2069 6e20 4361 6e61 6461  e live in Canada
-000045a0: 5c6e 4163 7469 6f6e 3a20 5365 6172 6368  \nAction: Search
-000045b0: 5c6e 4163 7469 6f6e 2049 6e70 7574 3a20  \nAction Input: 
-000045c0: 486f 7720 6d61 6e79 2070 656f 706c 6520  How many people 
-000045d0: 6c69 7665 2069 6e20 4361 6e61 6461 2061  live in Canada a
-000045e0: 7320 6f66 2032 3032 335c 7530 3031 625b  s of 2023\u001b[
-000045f0: 306d 5c6e 4f62 7365 7276 6174 696f 6e3a  0m\nObservation:
-00004600: 205c 7530 3031 625b 3336 3b31 6d5c 7530   \u001b[36;1m\u0
-00004610: 3031 625b 313b 336d 5468 6520 6375 7272  01b[1;3mThe curr
-00004620: 656e 7420 706f 7075 6c61 7469 6f6e 206f  ent population o
-00004630: 6620 4361 6e61 6461 2069 7320 3338 2c36  f Canada is 38,6
-00004640: 3435 2c36 3730 2061 7320 6f66 2057 6564  45,670 as of Wed
-00004650: 6e65 7364 6179 2c20 4d61 7263 6820 3239  nesday, March 29
-00004660: 2c20 3230 3233 2c20 6261 7365 6420 6f6e  , 2023, based on
-00004670: 2057 6f72 6c64 6f6d 6574 6572 2065 6c61   Worldometer ela
-00004680: 626f 7261 7469 6f6e 206f 6620 7468 6520  boration of the 
-00004690: 6c61 7465 7374 2055 6e69 7465 6420 4e61  latest United Na
-000046a0: 7469 6f6e 7320 6461 7461 2e5c 7530 3031  tions data.\u001
-000046b0: 625b 306d 5c6e 5468 6f75 6768 743a 5c75  b[0m\nThought:\u
-000046c0: 3030 3162 5b33 323b 316d 5c75 3030 3162  001b[32;1m\u001b
-000046d0: 5b31 3b33 6d20 4920 6e6f 7720 6b6e 6f77  [1;3m I now know
-000046e0: 2074 6865 2066 696e 616c 2061 6e73 7765   the final answe
-000046f0: 725c 6e46 696e 616c 2041 6e73 7765 723a  r\nFinal Answer:
-00004700: 2041 7272 722c 2074 6865 7265 2062 6520   Arrr, there be 
-00004710: 3338 2c36 3435 2c36 3730 2070 656f 706c  38,645,670 peopl
-00004720: 6520 6c69 7669 6e27 2069 6e20 4361 6e61  e livin' in Cana
-00004730: 6461 2061 7320 6f66 2032 3032 3321 5c75  da as of 2023!\u
-00004740: 3030 3162 5b30 6d5c 6e5c 6e5c 7530 3031  001b[0m\n\n\u001
-00004750: 625b 316d 3e20 4669 6e69 7368 6564 2063  b[1m> Finished c
-00004760: 6861 696e 2e5c 7530 3031 625b 306d 220a  hain.\u001b[0m".
-00004770: 7d0a 6060 600a 0a23 2323 2323 2057 6861  }.```..##### Wha
-00004780: 7420 6861 7070 656e 6564 3f0a 0a2d 2049  t happened?..- I
-00004790: 6e20 6120 6d61 7474 6572 206f 6620 6665  n a matter of fe
-000047a0: 7720 7365 636f 6e64 732c 2077 6527 7665  w seconds, we've
-000047b0: 2064 6570 6c6f 7965 6420 6f75 7220 4150   deployed our AP
-000047c0: 4920 6f6e 204a 696e 6120 4149 2043 6c6f  I on Jina AI Clo
-000047d0: 7564 20f0 9f8e 890a 2d20 5468 6520 4150  ud .....- The AP
-000047e0: 4920 6973 2073 6572 7665 726c 6573 7320  I is serverless 
-000047f0: 616e 6420 7363 616c 6162 6c65 2c20 736f  and scalable, so
-00004800: 2077 6520 6361 6e20 7363 616c 6520 7570   we can scale up
-00004810: 2074 6865 2041 5049 2074 6f20 6861 6e64   the API to hand
-00004820: 6c65 206d 6f72 6520 7265 7175 6573 7473  le more requests
-00004830: 2e20 0a2d 2059 6f75 206d 6967 6874 206f  . .- You might o
-00004840: 6273 6572 7665 2061 2064 656c 6179 2069  bserve a delay i
-00004850: 6e20 7468 6520 6669 7273 7420 7265 7175  n the first requ
-00004860: 6573 742c 2074 6861 7427 7320 6475 6520  est, that's due 
-00004870: 746f 2074 6865 2077 6172 6d2d 7570 2074  to the warm-up t
-00004880: 696d 6520 6f66 2074 6865 2041 5049 2e20  ime of the API. 
-00004890: 5375 6273 6571 7565 6e74 2072 6571 7565  Subsequent reque
-000048a0: 7374 7320 7769 6c6c 2062 6520 6661 7374  sts will be fast
-000048b0: 6572 2e0a 2d20 5468 6520 4150 4920 696e  er..- The API in
-000048c0: 636c 7564 6573 2061 2053 7761 6767 6572  cludes a Swagger
-000048d0: 2055 4920 616e 6420 7468 6520 4f70 656e   UI and the Open
-000048e0: 4150 4920 7370 6563 6966 6963 6174 696f  API specificatio
-000048f0: 6e2c 2073 6f20 6974 2063 616e 2062 6520  n, so it can be 
-00004900: 6561 7369 6c79 2069 6e74 6567 7261 7465  easily integrate
-00004910: 6420 7769 7468 206f 7468 6572 2073 6572  d with other ser
-00004920: 7669 6365 732e 200a 2d20 4e6f 772c 206f  vices. .- Now, o
-00004930: 7468 6572 2061 6765 6e74 7320 6361 6e20  ther agents can 
-00004940: 696e 7465 6772 6174 6520 7769 7468 2079  integrate with y
-00004950: 6f75 7220 6167 656e 7473 206f 6e20 4a69  our agents on Ji
-00004960: 6e61 2041 4920 436c 6f75 6420 7468 616e  na AI Cloud than
-00004970: 6b73 2074 6f20 7468 6520 5b4f 7065 6e41  ks to the [OpenA
-00004980: 5049 2041 6765 6e74 5d28 6874 7470 733a  PI Agent](https:
-00004990: 2f2f 7079 7468 6f6e 2e6c 616e 6763 6861  //python.langcha
-000049a0: 696e 2e63 6f6d 2f65 6e2f 6c61 7465 7374  in.com/en/latest
-000049b0: 2f6d 6f64 756c 6573 2f61 6765 6e74 732f  /modules/agents/
-000049c0: 746f 6f6c 6b69 7473 2f65 7861 6d70 6c65  toolkits/example
-000049d0: 732f 6f70 656e 6170 692e 6874 6d6c 2920  s/openapi.html) 
-000049e0: f09f 92a1 0a0a 0a0a 2d2d 2d0a 0a23 2323  ........---..###
-000049f0: 2320 5265 6163 6820 6f75 7420 746f 2075  # Reach out to u
-00004a00: 7320 f09f 939e 0a0a 2d20 5365 7276 6572  s ......- Server
-00004a10: 6c65 7373 2069 7320 6e6f 7420 796f 7572  less is not your
-00004a20: 2074 6869 6e67 3f0a 2d20 446f 2079 6f75   thing?.- Do you
-00004a30: 2077 616e 7420 6c61 7267 6572 2069 6e73   want larger ins
-00004a40: 7461 6e63 6573 2066 6f72 2079 6f75 7220  tances for your 
-00004a50: 4150 493f 0a2d 204c 6f6f 6b69 6e67 2066  API?.- Looking f
-00004a60: 6f72 2066 696c 6520 7570 6c6f 6164 732c  or file uploads,
-00004a70: 206f 7220 6f74 6865 7220 6461 7461 2d69   or other data-i
-00004a80: 6e2c 2064 6174 612d 6f75 7420 6665 6174  n, data-out feat
-00004a90: 7572 6573 3f0a 2d20 446f 2079 6f75 2077  ures?.- Do you w
-00004aa0: 616e 7420 746f 2073 6574 7570 2063 7573  ant to setup cus
-00004ab0: 746f 6d20 6175 7468 6f72 697a 6174 696f  tom authorizatio
-00004ac0: 6e20 666f 7220 796f 7572 2041 5049 3f0a  n for your API?.
-00004ad0: 0a0a f09f 93a3 2047 6f74 2079 6f75 7220  ...... Got your 
-00004ae0: 6174 7465 6e74 696f 6e3f 205b 4a6f 696e  attention? [Join
-00004af0: 2075 7320 6f6e 2053 6c61 636b 5d28 6874   us on Slack](ht
-00004b00: 7470 733a 2f2f 6a69 6e61 2e61 692f 736c  tps://jina.ai/sl
-00004b10: 6163 6b2f 2920 616e 6420 7765 2764 2062  ack/) and we'd b
-00004b20: 6520 6861 7070 7920 746f 2068 656c 7020  e happy to help 
-00004b30: 796f 7520 6f75 742e 0a0a 2d2d 2d0a 0a0a  you out...---...
-00004b40: 2323 2320 606c 632d 7365 7276 6560 0a0a  ### `lc-serve`..
-00004b50: 606c 632d 7365 7276 6560 2069 7320 6120  `lc-serve` is a 
-00004b60: 434c 4920 746f 6f6c 2074 6861 7420 6865  CLI tool that he
-00004b70: 6c70 7320 796f 7520 746f 2064 6570 6c6f  lps you to deplo
-00004b80: 7920 796f 7572 2061 6765 6e74 7320 6f6e  y your agents on
-00004b90: 204a 696e 6120 4149 2043 6c6f 7564 2e0a   Jina AI Cloud..
-00004ba0: 0a0a 7c20 4465 7363 7269 7074 696f 6e20  ..| Description 
-00004bb0: 7c20 436f 6d6d 616e 6420 7c20 0a7c 202d  | Command | .| -
-00004bc0: 2d2d 207c 202d 2d2d 3a20 7c0a 7c20 4465  -- | ---: |.| De
-00004bd0: 706c 6f79 2079 6f75 7220 6170 7020 6c6f  ploy your app lo
-00004be0: 6361 6c6c 7920 7c20 606c 632d 7365 7276  cally | `lc-serv
-00004bf0: 6520 6465 706c 6f79 206c 6f63 616c 2061  e deploy local a
-00004c00: 7070 6020 7c0a 7c20 4465 706c 6f79 2079  pp` |.| Deploy y
-00004c10: 6f75 7220 6170 7020 6f6e 204a 696e 6120  our app on Jina 
-00004c20: 4149 2043 6c6f 7564 207c 2060 6c63 2d73  AI Cloud | `lc-s
-00004c30: 6572 7665 2064 6570 6c6f 7920 6a63 6c6f  erve deploy jclo
-00004c40: 7564 2061 7070 6020 7c0a 7c20 5570 6461  ud app` |.| Upda
-00004c50: 7465 2065 7869 7374 696e 6720 6170 7020  te existing app 
-00004c60: 6f6e 204a 696e 6120 4149 2043 6c6f 7564  on Jina AI Cloud
-00004c70: 207c 2060 6c63 2d73 6572 7665 2064 6570   | `lc-serve dep
-00004c80: 6c6f 7920 6a63 6c6f 7564 2061 7070 202d  loy jcloud app -
-00004c90: 2d61 7070 2d69 6420 3c61 7070 2d69 643e  -app-id <app-id>
-00004ca0: 6020 7c0a 7c20 4765 7420 6170 7020 7374  ` |.| Get app st
-00004cb0: 6174 7573 206f 6e20 4a69 6e61 2041 4920  atus on Jina AI 
-00004cc0: 436c 6f75 6420 7c20 606c 632d 7365 7276  Cloud | `lc-serv
-00004cd0: 6520 7374 6174 7573 203c 6170 702d 6964  e status <app-id
-00004ce0: 3e60 207c 0a7c 204c 6973 7420 616c 6c20  >` |.| List all 
-00004cf0: 6170 7073 206f 6e20 4a69 6e61 2041 4920  apps on Jina AI 
-00004d00: 436c 6f75 6420 7c20 606c 632d 7365 7276  Cloud | `lc-serv
-00004d10: 6520 6c69 7374 6020 7c0a 7c20 5265 6d6f  e list` |.| Remo
-00004d20: 7665 2061 7070 206f 6e20 4a69 6e61 2041  ve app on Jina A
-00004d30: 4920 436c 6f75 6420 7c20 606c 632d 7365  I Cloud | `lc-se
-00004d40: 7276 6520 7265 6d6f 7665 203c 6170 702d  rve remove <app-
-00004d50: 6964 3e60 207c 0a0a 0a2d 2d2d 0a0a 2323  id>` |...---..##
-00004d60: 2320 4167 656e 7473 2050 6c61 7967 726f  # Agents Playgro
-00004d70: 756e 6420 f09f 95b9 efb8 8ff0 9f8e aef0  und ............
-00004d80: 9f8c 900a 0a5b 4c61 6e67 4368 6169 6e20  .....[LangChain 
-00004d90: 6167 656e 7473 5d28 6874 7470 733a 2f2f  agents](https://
-00004da0: 7079 7468 6f6e 2e6c 616e 6763 6861 696e  python.langchain
-00004db0: 2e63 6f6d 2f65 6e2f 6c61 7465 7374 2f6d  .com/en/latest/m
-00004dc0: 6f64 756c 6573 2f61 6765 6e74 732f 6765  odules/agents/ge
-00004dd0: 7474 696e 675f 7374 6172 7465 642e 6874  tting_started.ht
-00004de0: 6d6c 2920 7573 6520 4c4c 4d73 2074 6f20  ml) use LLMs to 
-00004df0: 6465 7465 726d 696e 6520 7468 6520 6163  determine the ac
-00004e00: 7469 6f6e 7320 746f 2062 6520 7461 6b65  tions to be take
-00004e10: 6e20 696e 2077 6861 7420 6f72 6465 722e  n in what order.
-00004e20: 2041 6e20 6163 7469 6f6e 2063 616e 2065   An action can e
-00004e30: 6974 6865 7220 6265 2075 7369 6e67 2061  ither be using a
-00004e40: 2074 6f6f 6c20 616e 6420 6f62 7365 7276   tool and observ
-00004e50: 696e 6720 6974 7320 6f75 7470 7574 2c20  ing its output, 
-00004e60: 6f72 2072 6574 7572 6e69 6e67 2074 6f20  or returning to 
-00004e70: 7468 6520 7573 6572 2e20 5765 2776 6520  the user. We've 
-00004e80: 686f 7374 6564 2061 202a 2a5b 5374 7265  hosted a **[Stre
-00004e90: 616d 6c69 7420 506c 6179 6772 6f75 6e64  amlit Playground
-00004ea0: 5d28 6874 7470 733a 2f2f 6c61 6e67 6368  ](https://langch
-00004eb0: 6169 6e2e 776f 6c66 2e6a 696e 612e 6169  ain.wolf.jina.ai
-00004ec0: 2f70 6c61 7967 726f 756e 642f 292a 2a20  /playground/)** 
-00004ed0: 6f6e 204a 696e 6120 4149 2043 6c6f 7564  on Jina AI Cloud
-00004ee0: 2074 6f20 696e 7465 7261 6374 2077 6974   to interact wit
-00004ef0: 6820 7468 6520 6167 656e 7473 2c20 7768  h the agents, wh
-00004f00: 6963 6820 6163 6365 7074 7320 7769 7468  ich accepts with
-00004f10: 2066 6f6c 6c6f 7769 6e67 2069 6e70 7574   following input
-00004f20: 733a 0a0a 2d20 2a2a 5b41 6765 6e74 2054  s:..- **[Agent T
-00004f30: 7970 6573 5d28 6874 7470 733a 2f2f 7079  ypes](https://py
-00004f40: 7468 6f6e 2e6c 616e 6763 6861 696e 2e63  thon.langchain.c
-00004f50: 6f6d 2f65 6e2f 6c61 7465 7374 2f6d 6f64  om/en/latest/mod
-00004f60: 756c 6573 2f61 6765 6e74 732f 6167 656e  ules/agents/agen
-00004f70: 7473 2e68 746d 6c29 3a2a 2a20 4368 6f6f  ts.html):** Choo
-00004f80: 7365 2066 726f 6d20 6469 6666 6572 656e  se from differen
-00004f90: 7420 6167 656e 7420 7479 7065 7320 7468  t agent types th
-00004fa0: 6174 204c 616e 6763 6861 696e 2073 7570  at Langchain sup
-00004fb0: 706f 7274 732e 200a 0a2d 202a 2a5b 546f  ports. ..- **[To
-00004fc0: 6f6c 735d 2868 7474 7073 3a2f 2f70 7974  ols](https://pyt
-00004fd0: 686f 6e2e 6c61 6e67 6368 6169 6e2e 636f  hon.langchain.co
-00004fe0: 6d2f 656e 2f6c 6174 6573 742f 6d6f 6475  m/en/latest/modu
-00004ff0: 6c65 732f 6167 656e 7473 2f74 6f6f 6c73  les/agents/tools
-00005000: 2e68 746d 6c29 3a2a 2a20 4368 6f6f 7365  .html):** Choose
-00005010: 2066 726f 6d20 6469 6666 6572 656e 7420   from different 
-00005020: 746f 6f6c 7320 7468 6174 204c 616e 6763  tools that Langc
-00005030: 6861 696e 2073 7570 706f 7274 732e 2053  hain supports. S
-00005040: 6f6d 6520 746f 6f6c 7320 6d61 7920 7265  ome tools may re
-00005050: 7175 6972 6520 616e 2041 5049 2074 6f6b  quire an API tok
-00005060: 656e 206f 7220 6f74 6865 7220 7265 6c61  en or other rela
-00005070: 7465 6420 6172 6775 6d65 6e74 732e 0a0a  ted arguments...
-00005080: 546f 2075 7365 2074 6865 2070 6c61 7967  To use the playg
-00005090: 726f 756e 642c 2073 696d 706c 7920 7479  round, simply ty
-000050a0: 7065 2079 6f75 7220 696e 7075 7420 696e  pe your input in
-000050b0: 2074 6865 2074 6578 7420 626f 7820 7072   the text box pr
-000050c0: 6f76 6964 6564 2074 6f20 6765 7420 7468  ovided to get th
-000050d0: 6520 6167 656e 7427 7320 6f75 7470 7574  e agent's output
-000050e0: 2061 6e64 2063 6861 696e 206f 6620 7468   and chain of th
-000050f0: 6f75 6768 742e 2045 6e6a 6f79 2065 7870  ought. Enjoy exp
-00005100: 6c6f 7269 6e67 204c 616e 6763 6861 696e  loring Langchain
-00005110: 2773 2063 6170 6162 696c 6974 6965 7321  's capabilities!
-00005120: 2049 6e20 6164 6469 7469 6f6e 2074 6f20   In addition to 
-00005130: 7374 7265 616d 6c69 742c 2079 6f75 2063  streamlit, you c
-00005140: 616e 2061 6c73 6f20 7573 6520 6f75 7220  an also use our 
-00005150: 5245 5354 6675 6c20 4150 4973 206f 6e20  RESTful APIs on 
-00005160: 7468 6520 706c 6179 6772 6f75 6e64 2074  the playground t
-00005170: 6f20 696e 7465 7261 6374 2077 6974 6820  o interact with 
-00005180: 7468 6520 6167 656e 7473 2e20 0a0a 0a23  the agents. ...#
-00005190: 2323 205b 5a65 726f 2d73 686f 7420 5265  ## [Zero-shot Re
-000051a0: 6163 7420 4465 7363 7269 7074 696f 6e20  act Description 
-000051b0: 6167 656e 7420 7769 7468 2053 6572 7041  agent with SerpA
-000051c0: 5049 2061 6e64 2043 616c 6375 6c61 746f  PI and Calculato
-000051d0: 725d 2868 7474 7073 3a2f 2f70 7974 686f  r](https://pytho
-000051e0: 6e2e 6c61 6e67 6368 6169 6e2e 636f 6d2f  n.langchain.com/
-000051f0: 656e 2f6c 6174 6573 742f 6d6f 6475 6c65  en/latest/module
-00005200: 732f 6167 656e 7473 2f67 6574 7469 6e67  s/agents/getting
-00005210: 5f73 7461 7274 6564 2e68 746d 6c29 0a0a  _started.html)..
-00005220: 2323 2323 2053 7472 6561 6d6c 6974 2050  #### Streamlit P
-00005230: 6c61 7967 726f 756e 640a 0a21 5b53 7472  layground..![Str
-00005240: 6561 6d6c 6974 2050 6c61 7967 726f 756e  eamlit Playgroun
-00005250: 645d 282e 6769 7468 7562 2f69 6d61 6765  d](.github/image
-00005260: 732f 706c 6179 6772 6f75 6e64 5f6f 6e65  s/playground_one
-00005270: 2e67 6966 290a 0a23 2323 2320 5245 5354  .gif)..#### REST
-00005280: 6675 6c20 4150 490a 0a60 6060 6261 7368  ful API..```bash
-00005290: 0a65 7870 6f72 7420 4f50 454e 4149 5f41  .export OPENAI_A
-000052a0: 5049 5f4b 4559 3d73 6b2d 2a2a 2a0a 6578  PI_KEY=sk-***.ex
-000052b0: 706f 7274 2053 4552 5041 5049 5f41 5049  port SERPAPI_API
-000052c0: 5f4b 4559 3d2a 2a2a 0a0a 6375 726c 202d  _KEY=***..curl -
-000052d0: 7358 2050 4f53 5420 2768 7474 7073 3a2f  sX POST 'https:/
-000052e0: 2f6c 616e 6763 6861 696e 2e77 6f6c 662e  /langchain.wolf.
-000052f0: 6a69 6e61 2e61 692f 6170 692f 7275 6e27  jina.ai/api/run'
-00005300: 205c 0a20 202d 4820 2761 6363 6570 743a   \.  -H 'accept:
-00005310: 2061 7070 6c69 6361 7469 6f6e 2f6a 736f   application/jso
-00005320: 6e27 205c 0a20 202d 4820 2743 6f6e 7465  n' \.  -H 'Conte
-00005330: 6e74 2d54 7970 653a 2061 7070 6c69 6361  nt-Type: applica
-00005340: 7469 6f6e 2f6a 736f 6e27 205c 0a20 202d  tion/json' \.  -
-00005350: 2d64 6174 612d 7261 7720 277b 0a20 2020  -data-raw '{.   
-00005360: 2022 7465 7874 223a 2022 5768 6f20 6973   "text": "Who is
-00005370: 204c 656f 2044 6943 6170 7269 6f73 2067   Leo DiCaprios g
-00005380: 6972 6c66 7269 656e 643f 2057 6861 7420  irlfriend? What 
-00005390: 6973 2068 6572 2063 7572 7265 6e74 2061  is her current a
-000053a0: 6765 2072 6169 7365 6420 746f 2074 6865  ge raised to the
-000053b0: 2030 2e34 3320 706f 7765 723f 222c 0a20   0.43 power?",. 
-000053c0: 2020 2022 7061 7261 6d65 7465 7273 223a     "parameters":
-000053d0: 207b 0a20 2020 2020 2020 2022 746f 6f6c   {.        "tool
-000053e0: 7322 3a20 7b0a 2020 2020 2020 2020 2020  s": {.          
-000053f0: 2020 2274 6f6f 6c5f 6e61 6d65 7322 3a20    "tool_names": 
-00005400: 5b22 7365 7270 6170 6922 2c20 226c 6c6d  ["serpapi", "llm
-00005410: 2d6d 6174 6822 5d0a 2020 2020 2020 2020  -math"].        
-00005420: 7d2c 0a20 2020 2020 2020 2022 6167 656e  },.        "agen
-00005430: 7422 3a20 227a 6572 6f2d 7368 6f74 2d72  t": "zero-shot-r
-00005440: 6561 6374 2d64 6573 6372 6970 7469 6f6e  eact-description
-00005450: 222c 0a20 2020 2020 2020 2022 7665 7262  ",.        "verb
-00005460: 6f73 6522 3a20 7472 7565 0a20 2020 207d  ose": true.    }
-00005470: 2c0a 2020 2020 2265 6e76 7322 3a20 7b0a  ,.    "envs": {.
-00005480: 2020 2020 2020 2020 224f 5045 4e41 495f          "OPENAI_
-00005490: 4150 495f 4b45 5922 3a20 2227 2224 7b4f  API_KEY": "'"${O
-000054a0: 5045 4e41 495f 4150 495f 4b45 597d 2227  PENAI_API_KEY}"'
-000054b0: 222c 0a20 2020 2020 2020 2022 5345 5250  ",.        "SERP
-000054c0: 4150 495f 4150 495f 4b45 5922 3a20 2227  API_API_KEY": "'
-000054d0: 2224 7b53 4552 5041 5049 5f41 5049 5f4b  "${SERPAPI_API_K
-000054e0: 4559 7d22 2722 0a20 2020 207d 0a7d 2720  EY}"'".    }.}' 
-000054f0: 7c20 6a71 0a60 6060 200a 0a60 6060 6a73  | jq.``` ..```js
-00005500: 6f6e 0a7b 0a20 2022 7265 7375 6c74 223a  on.{.  "result":
-00005510: 2022 4361 6d69 6c61 204d 6f72 726f 6e65   "Camila Morrone
-00005520: 2069 7320 4c65 6f20 4469 4361 7072 696f   is Leo DiCaprio
-00005530: 2773 2067 6972 6c66 7269 656e 642c 2061  's girlfriend, a
-00005540: 6e64 2068 6572 2063 7572 7265 6e74 2061  nd her current a
-00005550: 6765 2072 6169 7365 6420 746f 2074 6865  ge raised to the
-00005560: 2030 2e34 3320 706f 7765 7220 6973 2033   0.43 power is 3
-00005570: 2e36 3236 3132 3630 3631 3135 3239 3532  .626126061152952
-00005580: 372e 222c 0a20 2022 6368 6169 6e5f 6f66  7.",.  "chain_of
-00005590: 5f74 686f 7567 6874 223a 2022 5c75 3030  _thought": "\u00
-000055a0: 3162 5b31 6d3e 2045 6e74 6572 696e 6720  1b[1m> Entering 
-000055b0: 6e65 7720 4167 656e 7445 7865 6375 746f  new AgentExecuto
-000055c0: 7220 6368 6169 6e2e 2e2e 5c75 3030 3162  r chain...\u001b
-000055d0: 5b30 6d5c 7530 3031 625b 3332 3b31 6d5c  [0m\u001b[32;1m\
-000055e0: 7530 3031 625b 313b 336d 2049 206e 6565  u001b[1;3m I nee
-000055f0: 6420 746f 2066 696e 6420 6f75 7420 7468  d to find out th
-00005600: 6520 6e61 6d65 206f 6620 4c65 6f27 7320  e name of Leo's 
-00005610: 6769 726c 6672 6965 6e64 2061 6e64 2074  girlfriend and t
-00005620: 6865 6e20 7573 6520 7468 6520 6361 6c63  hen use the calc
-00005630: 756c 6174 6f72 2074 6f20 6361 6c63 756c  ulator to calcul
-00005640: 6174 6520 6865 7220 6167 6520 746f 2074  ate her age to t
-00005650: 6865 2030 2e34 3320 706f 7765 722e 4163  he 0.43 power.Ac
-00005660: 7469 6f6e 3a20 5365 6172 6368 4163 7469  tion: SearchActi
-00005670: 6f6e 2049 6e70 7574 3a20 4c65 6f20 4469  on Input: Leo Di
-00005680: 4361 7072 696f 2067 6972 6c66 7269 656e  Caprio girlfrien
-00005690: 645c 7530 3031 625b 306d 4f62 7365 7276  d\u001b[0mObserv
-000056a0: 6174 696f 6e3a 205c 7530 3031 625b 3336  ation: \u001b[36
-000056b0: 3b31 6d5c 7530 3031 625b 313b 336d 4469  ;1m\u001b[1;3mDi
-000056c0: 4361 7072 696f 206d 6574 2061 6374 6f72  Caprio met actor
-000056d0: 2043 616d 696c 6120 4d6f 7272 6f6e 6520   Camila Morrone 
-000056e0: 696e 2044 6563 656d 6265 7220 3230 3137  in December 2017
-000056f0: 2c20 7768 656e 2073 6865 2077 6173 2032  , when she was 2
-00005700: 3020 616e 6420 6865 2077 6173 2034 332e  0 and he was 43.
-00005710: 2054 6865 7920 7765 7265 2073 706f 7474   They were spott
-00005720: 6564 2061 7420 436f 6163 6865 6c6c 6120  ed at Coachella 
-00005730: 616e 6420 7765 6e74 206f 6e20 6d75 6c74  and went on mult
-00005740: 6970 6c65 2076 6163 6174 696f 6e73 2074  iple vacations t
-00005750: 6f67 6574 6865 722e 2053 6f6d 6520 7265  ogether. Some re
-00005760: 706f 7274 7320 7375 6767 6573 7465 6420  ports suggested 
-00005770: 7468 6174 2044 6943 6170 7269 6f20 7761  that DiCaprio wa
-00005780: 7320 7265 6164 7920 746f 2061 736b 204d  s ready to ask M
-00005790: 6f72 726f 6e65 2074 6f20 6d61 7272 7920  orrone to marry 
-000057a0: 6869 6d2e 2054 6865 2063 6f75 706c 6520  him. The couple 
-000057b0: 6d61 6465 2074 6865 6972 2072 6564 2063  made their red c
-000057c0: 6172 7065 7420 6465 6275 7420 6174 2074  arpet debut at t
-000057d0: 6865 2032 3032 3020 4163 6164 656d 7920  he 2020 Academy 
-000057e0: 4177 6172 6473 2e5c 7530 3031 625b 306d  Awards.\u001b[0m
-000057f0: 5468 6f75 6768 743a 5c75 3030 3162 5b33  Thought:\u001b[3
-00005800: 323b 316d 5c75 3030 3162 5b31 3b33 6d20  2;1m\u001b[1;3m 
-00005810: 4920 6e65 6564 2074 6f20 7573 6520 7468  I need to use th
-00005820: 6520 6361 6c63 756c 6174 6f72 2074 6f20  e calculator to 
-00005830: 6361 6c63 756c 6174 6520 6865 7220 6167  calculate her ag
-00005840: 6520 746f 2074 6865 2030 2e34 3320 706f  e to the 0.43 po
-00005850: 7765 7241 6374 696f 6e3a 2043 616c 6375  werAction: Calcu
-00005860: 6c61 746f 7241 6374 696f 6e20 496e 7075  latorAction Inpu
-00005870: 743a 2032 305e 302e 3433 5c75 3030 3162  t: 20^0.43\u001b
-00005880: 5b30 6d4f 6273 6572 7661 7469 6f6e 3a20  [0mObservation: 
-00005890: 5c75 3030 3162 5b33 333b 316d 5c75 3030  \u001b[33;1m\u00
-000058a0: 3162 5b31 3b33 6d41 6e73 7765 723a 2033  1b[1;3mAnswer: 3
-000058b0: 2e36 3236 3132 3630 3631 3135 3239 3532  .626126061152952
-000058c0: 375c 7530 3031 625b 306d 5468 6f75 6768  7\u001b[0mThough
-000058d0: 743a 5c75 3030 3162 5b33 323b 316d 5c75  t:\u001b[32;1m\u
-000058e0: 3030 3162 5b31 3b33 6d20 4920 6e6f 7720  001b[1;3m I now 
-000058f0: 6b6e 6f77 2074 6865 2066 696e 616c 2061  know the final a
-00005900: 6e73 7765 7246 696e 616c 2041 6e73 7765  nswerFinal Answe
-00005910: 723a 2043 616d 696c 6120 4d6f 7272 6f6e  r: Camila Morron
-00005920: 6520 6973 204c 656f 2044 6943 6170 7269  e is Leo DiCapri
-00005930: 6f27 7320 6769 726c 6672 6965 6e64 2c20  o's girlfriend, 
-00005940: 616e 6420 6865 7220 6375 7272 656e 7420  and her current 
-00005950: 6167 6520 7261 6973 6564 2074 6f20 7468  age raised to th
-00005960: 6520 302e 3433 2070 6f77 6572 2069 7320  e 0.43 power is 
-00005970: 332e 3632 3631 3236 3036 3131 3532 3935  3.62612606115295
-00005980: 3237 2e5c 7530 3031 625b 306d 5c75 3030  27.\u001b[0m\u00
-00005990: 3162 5b31 6d3e 2046 696e 6973 6865 6420  1b[1m> Finished 
-000059a0: 6368 6169 6e2e 5c75 3030 3162 5b30 6d22  chain.\u001b[0m"
-000059b0: 0a7d 0a60 6060 0a0a 2323 2320 5b53 656c  .}.```..### [Sel
-000059c0: 6620 4173 6b20 5769 7468 2053 6561 7263  f Ask With Searc
-000059d0: 685d 2868 7474 7073 3a2f 2f70 7974 686f  h](https://pytho
-000059e0: 6e2e 6c61 6e67 6368 6169 6e2e 636f 6d2f  n.langchain.com/
-000059f0: 656e 2f6c 6174 6573 742f 6d6f 6475 6c65  en/latest/module
-00005a00: 732f 6167 656e 7473 2f69 6d70 6c65 6d65  s/agents/impleme
-00005a10: 6e74 6174 696f 6e73 2f73 656c 665f 6173  ntations/self_as
-00005a20: 6b5f 7769 7468 5f73 6561 7263 682e 6874  k_with_search.ht
-00005a30: 6d6c 290a 0a23 2323 2320 5374 7265 616d  ml)..#### Stream
-00005a40: 6c69 7420 506c 6179 6772 6f75 6e64 0a0a  lit Playground..
-00005a50: 215b 5374 7265 616d 6c69 7420 506c 6179  ![Streamlit Play
-00005a60: 6772 6f75 6e64 5d28 2e67 6974 6875 622f  ground](.github/
-00005a70: 696d 6167 6573 2f70 6c61 7967 726f 756e  images/playgroun
-00005a80: 645f 7477 6f2e 6769 6629 0a0a 2323 2323  d_two.gif)..####
-00005a90: 2052 4553 5466 756c 2041 5049 0a0a 6060   RESTful API..``
-00005aa0: 6062 6173 680a 6578 706f 7274 204f 5045  `bash.export OPE
-00005ab0: 4e41 495f 4150 495f 4b45 593d 736b 2d2a  NAI_API_KEY=sk-*
-00005ac0: 2a2a 0a65 7870 6f72 7420 5345 5250 4150  **.export SERPAP
-00005ad0: 495f 4150 495f 4b45 593d 2a2a 2a0a 0a63  I_API_KEY=***..c
-00005ae0: 7572 6c20 2d73 5820 504f 5354 2027 6874  url -sX POST 'ht
-00005af0: 7470 733a 2f2f 6c61 6e67 6368 6169 6e2e  tps://langchain.
-00005b00: 776f 6c66 2e6a 696e 612e 6169 2f61 7069  wolf.jina.ai/api
-00005b10: 2f72 756e 2720 5c0a 2020 2d48 2027 6163  /run' \.  -H 'ac
-00005b20: 6365 7074 3a20 6170 706c 6963 6174 696f  cept: applicatio
-00005b30: 6e2f 6a73 6f6e 2720 5c0a 2020 2d48 2027  n/json' \.  -H '
-00005b40: 436f 6e74 656e 742d 5479 7065 3a20 6170  Content-Type: ap
-00005b50: 706c 6963 6174 696f 6e2f 6a73 6f6e 2720  plication/json' 
-00005b60: 5c0a 2020 2d2d 6461 7461 2d72 6177 2027  \.  --data-raw '
-00005b70: 7b0a 2020 2020 2274 6578 7422 3a20 2257  {.    "text": "W
-00005b80: 6861 7420 6973 2074 6865 2068 6f6d 6574  hat is the homet
-00005b90: 6f77 6e20 6f66 2074 6865 2072 6569 676e  own of the reign
-00005ba0: 696e 6720 6d65 6e73 2055 2e53 2e20 4f70  ing mens U.S. Op
-00005bb0: 656e 2063 6861 6d70 696f 6e3f 222c 0a20  en champion?",. 
-00005bc0: 2020 2022 7061 7261 6d65 7465 7273 223a     "parameters":
-00005bd0: 207b 0a20 2020 2020 2020 2022 746f 6f6c   {.        "tool
-00005be0: 7322 3a20 7b0a 2020 2020 2020 2020 2020  s": {.          
-00005bf0: 2020 2274 6f6f 6c5f 6e61 6d65 7322 3a20    "tool_names": 
-00005c00: 5b22 7365 7270 6170 6922 5d0a 2020 2020  ["serpapi"].    
-00005c10: 2020 2020 7d2c 0a20 2020 2020 2020 2022      },.        "
-00005c20: 6167 656e 7422 3a20 2273 656c 662d 6173  agent": "self-as
-00005c30: 6b2d 7769 7468 2d73 6561 7263 6822 2c0a  k-with-search",.
-00005c40: 2020 2020 2020 2020 2276 6572 626f 7365          "verbose
-00005c50: 223a 2074 7275 650a 2020 2020 7d2c 0a20  ": true.    },. 
-00005c60: 2020 2022 656e 7673 223a 207b 0a20 2020     "envs": {.   
-00005c70: 2020 2020 2022 4f50 454e 4149 5f41 5049       "OPENAI_API
-00005c80: 5f4b 4559 223a 2022 2722 247b 4f50 454e  _KEY": "'"${OPEN
-00005c90: 4149 5f41 5049 5f4b 4559 7d22 2722 2c0a  AI_API_KEY}"'",.
-00005ca0: 2020 2020 2020 2020 2253 4552 5041 5049          "SERPAPI
-00005cb0: 5f41 5049 5f4b 4559 223a 2022 2722 247b  _API_KEY": "'"${
-00005cc0: 5345 5250 4150 495f 4150 495f 4b45 597d  SERPAPI_API_KEY}
-00005cd0: 2227 220a 2020 2020 7d0a 7d27 207c 206a  "'".    }.}' | j
-00005ce0: 710a 6060 600a 0a60 6060 6a73 6f6e 0a7b  q.```..```json.{
-00005cf0: 0a20 2022 7265 7375 6c74 223a 2022 456c  .  "result": "El
-00005d00: 2050 616c 6d61 722c 204d 7572 6369 612c   Palmar, Murcia,
-00005d10: 2053 7061 696e 222c 0a20 2022 6368 6169   Spain",.  "chai
-00005d20: 6e5f 6f66 5f74 686f 7567 6874 223a 2022  n_of_thought": "
-00005d30: 5c75 3030 3162 5b31 6d3e 2045 6e74 6572  \u001b[1m> Enter
-00005d40: 696e 6720 6e65 7720 4167 656e 7445 7865  ing new AgentExe
-00005d50: 6375 746f 7220 6368 6169 6e2e 2e2e 5c75  cutor chain...\u
-00005d60: 3030 3162 5b30 6d5c 7530 3031 625b 3332  001b[0m\u001b[32
-00005d70: 3b31 6d5c 7530 3031 625b 313b 336d 2059  ;1m\u001b[1;3m Y
-00005d80: 6573 2e46 6f6c 6c6f 7720 7570 3a20 5768  es.Follow up: Wh
-00005d90: 6f20 6973 2074 6865 2072 6569 676e 696e  o is the reignin
-00005da0: 6720 6d65 6e73 2055 2e53 2e20 4f70 656e  g mens U.S. Open
-00005db0: 2063 6861 6d70 696f 6e3f 5c75 3030 3162   champion?\u001b
-00005dc0: 5b30 6d49 6e74 6572 6d65 6469 6174 6520  [0mIntermediate 
-00005dd0: 616e 7377 6572 3a20 5c75 3030 3162 5b33  answer: \u001b[3
-00005de0: 363b 316d 5c75 3030 3162 5b31 3b33 6d43  6;1m\u001b[1;3mC
-00005df0: 6172 6c6f 7320 416c 6361 7261 7a20 4761  arlos Alcaraz Ga
-00005e00: 7266 6961 5c75 3030 3162 5b30 6d5c 7530  rfia\u001b[0m\u0
-00005e10: 3031 625b 3332 3b31 6d5c 7530 3031 625b  01b[32;1m\u001b[
-00005e20: 313b 336d 466f 6c6c 6f77 2075 703a 2057  1;3mFollow up: W
-00005e30: 6861 7420 6973 2043 6172 6c6f 7320 416c  hat is Carlos Al
-00005e40: 6361 7261 7a20 4761 7266 6961 2773 2068  caraz Garfia's h
-00005e50: 6f6d 6574 6f77 6e3f 5c75 3030 3162 5b30  ometown?\u001b[0
-00005e60: 6d49 6e74 6572 6d65 6469 6174 6520 616e  mIntermediate an
-00005e70: 7377 6572 3a20 5c75 3030 3162 5b33 363b  swer: \u001b[36;
-00005e80: 316d 5c75 3030 3162 5b31 3b33 6d43 6172  1m\u001b[1;3mCar
-00005e90: 6c6f 7320 416c 6361 7261 7a20 4761 7266  los Alcaraz Garf
-00005ea0: 6961 2077 6173 2062 6f72 6e20 6f6e 204d  ia was born on M
-00005eb0: 6179 2035 2c20 3230 3033 2c20 696e 2045  ay 5, 2003, in E
-00005ec0: 6c20 5061 6c6d 6172 2c20 4d75 7263 6961  l Palmar, Murcia
-00005ed0: 2c20 5370 6169 6e20 746f 2070 6172 656e  , Spain to paren
-00005ee0: 7473 2043 6172 6c6f 7320 416c 6361 7261  ts Carlos Alcara
-00005ef0: 7a20 476f 6e7a c3a1 6c65 7a20 616e 6420  z Gonz..lez and 
-00005f00: 5669 7267 696e 6961 2047 6172 6669 6120  Virginia Garfia 
-00005f10: 4573 6361 6e64 c3b3 6e2e 2048 6520 6861  Escand..n. He ha
-00005f20: 7320 7468 7265 6520 7369 626c 696e 6773  s three siblings
-00005f30: 2e5c 7530 3031 625b 306d 5c75 3030 3162  .\u001b[0m\u001b
-00005f40: 5b33 323b 316d 5c75 3030 3162 5b31 3b33  [32;1m\u001b[1;3
-00005f50: 6d53 6f20 7468 6520 6669 6e61 6c20 616e  mSo the final an
-00005f60: 7377 6572 2069 733a 2045 6c20 5061 6c6d  swer is: El Palm
-00005f70: 6172 2c20 4d75 7263 6961 2c20 5370 6169  ar, Murcia, Spai
-00005f80: 6e5c 7530 3031 625b 306d 5c75 3030 3162  n\u001b[0m\u001b
-00005f90: 5b31 6d3e 2046 696e 6973 6865 6420 6368  [1m> Finished ch
-00005fa0: 6169 6e2e 5c75 3030 3162 5b30 6d22 0a7d  ain.\u001b[0m".}
-00005fb0: 0a60 6060 0a0a 2d2d 2d0a 0a23 2320 4368  .```..---..## Ch
-00005fc0: 6169 6e73 206f 6e20 4a69 6e61 20f0 9f93  ains on Jina ...
-00005fd0: a6f0 9f9a 800a 0a5b 4368 6169 6e73 5d28  .......[Chains](
-00005fe0: 6874 7470 733a 2f2f 7079 7468 6f6e 2e6c  https://python.l
-00005ff0: 616e 6763 6861 696e 2e63 6f6d 2f65 6e2f  angchain.com/en/
-00006000: 6c61 7465 7374 2f6d 6f64 756c 6573 2f63  latest/modules/c
-00006010: 6861 696e 732f 6765 7474 696e 675f 7374  hains/getting_st
-00006020: 6172 7465 642e 6874 6d6c 2920 696e 204c  arted.html) in L
-00006030: 616e 6743 6861 696e 2061 6c6c 6f77 2075  angChain allow u
-00006040: 7365 7273 2074 6f20 636f 6d62 696e 6520  sers to combine 
-00006050: 636f 6d70 6f6e 656e 7473 2074 6f20 6372  components to cr
-00006060: 6561 7465 2061 2073 696e 676c 652c 2063  eate a single, c
-00006070: 6f68 6572 656e 7420 6170 706c 6963 6174  oherent applicat
-00006080: 696f 6e2e 2057 6974 6820 4a69 6e61 2c20  ion. With Jina, 
-00006090: 0a0a 2d20 596f 7520 6361 6e20 6578 706f  ..- You can expo
-000060a0: 7365 2079 6f75 7220 6043 6861 696e 6020  se your `Chain` 
-000060b0: 6173 2052 4553 5466 756c 2f67 5250 432f  as RESTful/gRPC/
-000060c0: 5765 6253 6f63 6b65 7420 4150 492e 0a2d  WebSocket API..-
-000060d0: 2045 6e61 626c 6520 6043 6861 696e 6073   Enable `Chain`s
-000060e0: 2074 6f20 6465 706c 6f79 2026 2073 6361   to deploy & sca
-000060f0: 6c65 2073 6570 6172 6174 656c 7920 6672  le separately fr
-00006100: 6f6d 2074 6865 2072 6573 7420 6f66 2079  om the rest of y
-00006110: 6f75 7220 6170 706c 6963 6174 696f 6e20  our application 
-00006120: 7769 7468 2074 6865 2068 656c 7020 6f66  with the help of
-00006130: 2045 7865 6375 746f 7273 2e0a 2d20 4465   Executors..- De
-00006140: 706c 6f79 2079 6f75 7220 6043 6861 696e  ploy your `Chain
-00006150: 6020 6f6e 204a 696e 6120 4149 2043 6c6f  ` on Jina AI Clo
-00006160: 7564 2061 6e64 2067 6574 2065 7863 6c75  ud and get exclu
-00006170: 7369 7665 2061 6363 6573 7320 746f 2041  sive access to A
-00006180: 6765 6e74 7320 6f6e 204a 696e 6120 4149  gents on Jina AI
-00006190: 2043 6c6f 7564 2028 636f 6d69 6e67 2073   Cloud (coming s
-000061a0: 6f6f 6e29 0a0a 2323 2320 4578 616d 706c  oon)..### Exampl
-000061b0: 6573 0a0a 7c20 4578 616d 706c 6520 7c20  es..| Example | 
-000061c0: 4c61 6e67 4368 6169 6e20 446f 6373 207c  LangChain Docs |
-000061d0: 2044 6573 6372 6970 7469 6f6e 207c 0a7c   Description |.|
-000061e0: 202d 2d2d 2d2d 2d2d 207c 202d 2d2d 2d2d   ------- | -----
-000061f0: 2d2d 2d2d 2d2d 207c 202d 2d2d 2d2d 2d2d  ------ | -------
-00006200: 2d2d 2d2d 207c 0a7c 205b 4c4c 4d20 4368  ---- |.| [LLM Ch
-00006210: 6169 6e5d 2865 7861 6d70 6c65 732f 6c6c  ain](examples/ll
-00006220: 6d5f 6368 6169 6e2e 6d64 2920 7c20 5b4c  m_chain.md) | [L
-00006230: 696e 6b5d 2868 7474 7073 3a2f 2f6c 616e  ink](https://lan
-00006240: 6763 6861 696e 2e72 6561 6474 6865 646f  gchain.readthedo
-00006250: 6373 2e69 6f2f 656e 2f6c 6174 6573 742f  cs.io/en/latest/
-00006260: 6d6f 6475 6c65 732f 6368 6169 6e73 2f67  modules/chains/g
-00006270: 6574 7469 6e67 5f73 7461 7274 6564 2e68  etting_started.h
-00006280: 746d 6c23 7175 6572 792d 616e 2d6c 6c6d  tml#query-an-llm
-00006290: 2d77 6974 682d 7468 652d 6c6c 6d63 6861  -with-the-llmcha
-000062a0: 696e 2920 7c20 4578 706f 7365 2060 4368  in) | Expose `Ch
-000062b0: 6169 6e60 2061 7320 5245 5354 6675 6c2f  ain` as RESTful/
-000062c0: 6752 5043 2f57 6562 536f 636b 6574 2041  gRPC/WebSocket A
-000062d0: 5049 206c 6f63 616c 6c79 207c 0a7c 205b  PI locally |.| [
-000062e0: 5369 6d70 6c65 2053 6571 7565 6e74 6961  Simple Sequentia
-000062f0: 6c20 4368 6169 6e5d 2865 7861 6d70 6c65  l Chain](example
-00006300: 732f 7369 6d70 6c65 5f73 6571 7565 6e74  s/simple_sequent
-00006310: 6961 6c5f 6368 6169 6e2e 6d64 2920 7c20  ial_chain.md) | 
-00006320: 5b4c 696e 6b5d 2868 7474 7073 3a2f 2f6c  [Link](https://l
-00006330: 616e 6763 6861 696e 2e72 6561 6474 6865  angchain.readthe
-00006340: 646f 6373 2e69 6f2f 656e 2f6c 6174 6573  docs.io/en/lates
-00006350: 742f 6d6f 6475 6c65 732f 6368 6169 6e73  t/modules/chains
-00006360: 2f67 656e 6572 6963 2f73 6571 7565 6e74  /generic/sequent
-00006370: 6961 6c5f 6368 6169 6e73 2e68 746d 6c23  ial_chains.html#
-00006380: 7369 6d70 6c65 7365 7175 656e 7469 616c  simplesequential
-00006390: 6368 6169 6e29 207c 2045 7870 6f73 6520  chain) | Expose 
-000063a0: 6043 6861 696e 6020 6173 2052 4553 5466  `Chain` as RESTf
-000063b0: 756c 2f67 5250 432f 5765 6253 6f63 6b65  ul/gRPC/WebSocke
-000063c0: 7420 4150 4920 6c6f 6361 6c6c 7920 7c0a  t API locally |.
-000063d0: 7c20 5b53 6571 7565 6e74 6961 6c20 4368  | [Sequential Ch
-000063e0: 6169 6e5d 2865 7861 6d70 6c65 732f 7365  ain](examples/se
-000063f0: 7175 656e 7469 616c 5f63 6861 696e 2e6d  quential_chain.m
-00006400: 6429 207c 205b 4c69 6e6b 5d28 6874 7470  d) | [Link](http
-00006410: 733a 2f2f 6c61 6e67 6368 6169 6e2e 7265  s://langchain.re
-00006420: 6164 7468 6564 6f63 732e 696f 2f65 6e2f  adthedocs.io/en/
-00006430: 6c61 7465 7374 2f6d 6f64 756c 6573 2f63  latest/modules/c
-00006440: 6861 696e 732f 6765 6e65 7269 632f 7365  hains/generic/se
-00006450: 7175 656e 7469 616c 5f63 6861 696e 732e  quential_chains.
-00006460: 6874 6d6c 2373 6571 7565 6e74 6961 6c2d  html#sequential-
-00006470: 6368 6169 6e29 207c 2045 7870 6f73 6520  chain) | Expose 
-00006480: 6043 6861 696e 6020 6173 2052 4553 5466  `Chain` as RESTf
-00006490: 756c 2f67 5250 432f 5765 6253 6f63 6b65  ul/gRPC/WebSocke
-000064a0: 7420 4150 4920 6c6f 6361 6c6c 7920 7c0a  t API locally |.
-000064b0: 7c20 5b4c 4c4d 204d 6174 6820 4368 6169  | [LLM Math Chai
-000064c0: 6e5d 2865 7861 6d70 6c65 732f 6c6c 6d5f  n](examples/llm_
-000064d0: 6d61 7468 2e6d 6429 207c 205b 4c69 6e6b  math.md) | [Link
-000064e0: 5d28 6874 7470 733a 2f2f 6c61 6e67 6368  ](https://langch
-000064f0: 6169 6e2e 7265 6164 7468 6564 6f63 732e  ain.readthedocs.
-00006500: 696f 2f65 6e2f 6c61 7465 7374 2f6d 6f64  io/en/latest/mod
-00006510: 756c 6573 2f63 6861 696e 732f 6578 616d  ules/chains/exam
-00006520: 706c 6573 2f6c 6c6d 5f6d 6174 682e 6874  ples/llm_math.ht
-00006530: 6d6c 2920 7c20 4578 706f 7365 2060 4368  ml) | Expose `Ch
-00006540: 6169 6e60 2061 7320 5245 5354 6675 6c2f  ain` as RESTful/
-00006550: 6752 5043 2f57 6562 536f 636b 6574 2041  gRPC/WebSocket A
-00006560: 5049 206c 6f63 616c 6c79 207c 0a7c 205b  PI locally |.| [
-00006570: 4c4c 4d20 5265 7175 6573 7473 2043 6861  LLM Requests Cha
-00006580: 696e 5d28 6578 616d 706c 6573 2f6c 6c6d  in](examples/llm
-00006590: 5f72 6571 7565 7374 735f 6368 6169 6e2e  _requests_chain.
-000065a0: 6d64 2920 7c20 5b4c 696e 6b5d 2868 7474  md) | [Link](htt
-000065b0: 7073 3a2f 2f6c 616e 6763 6861 696e 2e72  ps://langchain.r
-000065c0: 6561 6474 6865 646f 6373 2e69 6f2f 656e  eadthedocs.io/en
-000065d0: 2f6c 6174 6573 742f 6d6f 6475 6c65 732f  /latest/modules/
-000065e0: 6368 6169 6e73 2f65 7861 6d70 6c65 732f  chains/examples/
-000065f0: 6c6c 6d5f 7265 7175 6573 7473 2e68 746d  llm_requests.htm
-00006600: 6c29 207c 2045 7870 6f73 6520 6043 6861  l) | Expose `Cha
-00006610: 696e 6020 6173 2052 4553 5466 756c 2f67  in` as RESTful/g
-00006620: 5250 432f 5765 6253 6f63 6b65 7420 4150  RPC/WebSocket AP
-00006630: 4920 6c6f 6361 6c6c 7920 7c0a 7c20 5b43  I locally |.| [C
-00006640: 7573 746f 6d20 4368 6169 6e5d 2865 7861  ustom Chain](exa
-00006650: 6d70 6c65 732f 6375 7374 6f6d 5f63 6861  mples/custom_cha
-00006660: 696e 2e6d 6429 207c 205b 4c69 6e6b 5d28  in.md) | [Link](
-00006670: 6874 7470 733a 2f2f 6c61 6e67 6368 6169  https://langchai
-00006680: 6e2e 7265 6164 7468 6564 6f63 732e 696f  n.readthedocs.io
-00006690: 2f65 6e2f 6c61 7465 7374 2f6d 6f64 756c  /en/latest/modul
-000066a0: 6573 2f63 6861 696e 732f 6765 7474 696e  es/chains/gettin
-000066b0: 675f 7374 6172 7465 642e 6874 6d6c 2363  g_started.html#c
-000066c0: 7265 6174 652d 612d 6375 7374 6f6d 2d63  reate-a-custom-c
-000066d0: 6861 696e 2d77 6974 682d 7468 652d 6368  hain-with-the-ch
-000066e0: 6169 6e2d 636c 6173 7329 207c 2045 7870  ain-class) | Exp
-000066f0: 6f73 6520 6043 6861 696e 6020 6173 2052  ose `Chain` as R
-00006700: 4553 5466 756c 2f67 5250 432f 5765 6253  ESTful/gRPC/WebS
-00006710: 6f63 6b65 7420 4150 4920 6c6f 6361 6c6c  ocket API locall
-00006720: 7920 7c0a 7c20 5b53 6571 7565 6e74 6961  y |.| [Sequentia
-00006730: 6c20 4368 6169 6e73 5d28 6578 616d 706c  l Chains](exampl
-00006740: 6573 2f73 6571 7565 6e74 6961 6c5f 6578  es/sequential_ex
-00006750: 6563 7574 6f72 732e 6d64 2920 7c20 4e2f  ecutors.md) | N/
-00006760: 4120 7c20 4275 696c 6420 2620 7363 616c  A | Build & scal
-00006770: 6520 6043 6861 696e 7360 2069 6e20 7365  e `Chains` in se
-00006780: 7061 7261 7465 2060 4578 6563 7574 6f72  parate `Executor
-00006790: 6073 207c 0a7c 205b 4272 616e 6368 696e  `s |.| [Branchin
-000067a0: 6720 4368 6169 6e73 5d28 6578 616d 706c  g Chains](exampl
-000067b0: 6573 2f62 7261 6e63 6869 6e67 2e6d 6429  es/branching.md)
-000067c0: 207c 204e 2f41 207c 2042 7261 6e63 6869   | N/A | Branchi
-000067d0: 6e67 2060 4368 6169 6e73 6020 696e 2073  ng `Chains` in s
-000067e0: 6570 6172 6174 6520 6045 7865 6375 746f  eparate `Executo
-000067f0: 7260 7320 746f 2061 6c6c 6f77 2070 6172  r`s to allow par
-00006800: 616c 6c65 6c20 6578 6563 7574 696f 6e20  allel execution 
-00006810: 7c0a 0a23 2320 4672 6571 7565 6e74 6c79  |..## Frequently
-00006820: 2041 736b 6564 2051 7565 7374 696f 6e73   Asked Questions
-00006830: 0a0a 2d20 5b4d 7920 636c 6965 6e74 2074  ..- [My client t
-00006840: 6861 7420 636f 6e6e 6563 7473 2074 6f20  hat connects to 
-00006850: 7468 6520 4170 7020 6765 7473 2074 696d  the App gets tim
-00006860: 6564 2d6f 7574 2c20 7768 6174 2073 686f  ed-out, what sho
-00006870: 756c 6420 4920 646f 3f5d 2823 6d79 2d63  uld I do?](#my-c
-00006880: 6c69 656e 742d 7468 6174 2d63 6f6e 6e65  lient-that-conne
-00006890: 6374 732d 746f 2d74 6865 2d61 7070 2d67  cts-to-the-app-g
-000068a0: 6574 732d 7469 6d65 642d 6f75 742d 7768  ets-timed-out-wh
-000068b0: 6174 2d73 686f 756c 642d 492d 646f 290a  at-should-I-do).
-000068c0: 2d20 5b4a 436c 6f75 6420 6465 706c 6f79  - [JCloud deploy
-000068d0: 6d65 6e74 2066 6169 6c65 6420 6174 2070  ment failed at p
-000068e0: 7573 6869 6e67 2069 6d61 6765 2074 6f20  ushing image to 
-000068f0: 4a69 6e61 2048 7562 626c 652c 2077 6861  Jina Hubble, wha
-00006900: 7420 7368 6f75 6c64 2049 2064 6f3f 5d28  t should I do?](
-00006910: 236a 636c 6f75 642d 6465 706c 6f79 6d65  #jcloud-deployme
-00006920: 6e74 2d66 6169 6c65 642d 6174 2d70 7573  nt-failed-at-pus
-00006930: 6869 6e67 2d69 6d61 6765 2d74 6f2d 6a69  hing-image-to-ji
-00006940: 6e61 2d68 7562 626c 652d 7768 6174 2d73  na-hubble-what-s
-00006950: 686f 756c 642d 692d 6469 290a 0a23 2323  hould-i-di)..###
-00006960: 204d 7920 636c 6965 6e74 2074 6861 7420   My client that 
-00006970: 636f 6e6e 6563 7473 2074 6f20 7468 6520  connects to the 
-00006980: 4170 7020 6765 7473 2074 696d 6564 2d6f  App gets timed-o
-00006990: 7574 2c20 7768 6174 2073 686f 756c 6420  ut, what should 
-000069a0: 4920 646f 3f0a 0a49 6620 796f 7520 6d61  I do?..If you ma
-000069b0: 6b65 206c 6f6e 6720 4854 5450 2072 6571  ke long HTTP req
-000069c0: 7565 7374 732c 2079 6f75 206d 6179 2065  uests, you may e
-000069d0: 7870 6572 6965 6e63 6520 7469 6d65 6f75  xperience timeou
-000069e0: 7473 2064 7565 2074 6f20 6c69 6d69 7461  ts due to limita
-000069f0: 7469 6f6e 7320 696e 2074 6865 204f 5353  tions in the OSS
-00006a00: 2077 6520 7573 6564 2069 6e20 606c 616e   we used in `lan
-00006a10: 6763 6861 696e 2d73 6572 7665 602e 2057  gchain-serve`. W
-00006a20: 6869 6c65 2077 6520 6172 6520 776f 726b  hile we are work
-00006a30: 696e 6720 746f 2070 6572 6d61 6e65 6e74  ing to permanent
-00006a40: 6c79 2061 6464 7265 7373 2074 6869 7320  ly address this 
-00006a50: 6973 7375 652c 2077 6520 7265 636f 6d6d  issue, we recomm
-00006a60: 656e 6420 7573 696e 6720 4854 5450 2f31  end using HTTP/1
-00006a70: 2e31 2069 6e20 796f 7572 2063 6c69 656e  .1 in your clien
-00006a80: 7420 6173 2061 2074 656d 706f 7261 7279  t as a temporary
-00006a90: 2077 6f72 6b61 726f 756e 642e 0a0a 2323   workaround...##
-00006aa0: 2320 4a43 6c6f 7564 2064 6570 6c6f 796d  # JCloud deploym
-00006ab0: 656e 7420 6661 696c 6564 2061 7420 7075  ent failed at pu
-00006ac0: 7368 696e 6720 696d 6167 6520 746f 204a  shing image to J
-00006ad0: 696e 6120 4875 6262 6c65 2c20 7768 6174  ina Hubble, what
-00006ae0: 2073 686f 756c 6420 4920 646f 3f0a 0a50   should I do?..P
-00006af0: 6c65 6173 6520 7573 6520 602d 2d76 6572  lease use `--ver
-00006b00: 626f 7365 6020 616e 6420 7265 7472 7920  bose` and retry 
-00006b10: 746f 2067 6574 206d 6f72 6520 696e 666f  to get more info
-00006b20: 726d 6174 696f 6e2e 2049 6620 796f 7520  rmation. If you 
-00006b30: 6172 6520 6f70 6572 6174 696e 6720 6f6e  are operating on
-00006b40: 2063 6f6d 7075 7465 7220 7769 7468 2060   computer with `
-00006b50: 6172 6d36 3460 2061 7263 682c 2070 6c65  arm64` arch, ple
-00006b60: 6173 6520 7265 7472 7920 7769 7468 2060  ase retry with `
-00006b70: 2d2d 706c 6174 666f 726d 206c 696e 7578  --platform linux
-00006b80: 2f61 6d64 3634 6020 736f 2074 6865 2069  /amd64` so the i
-00006b90: 6d61 6765 2063 616e 2062 6520 6275 696c  mage can be buil
-00006ba0: 7420 636f 7272 6563 746c 792e 0a         t correctly..
+00003700: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00003710: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00003720: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00003730: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00003740: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00003750: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00003760: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00003770: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00003780: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00003790: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000037a0: e294 80e2 9480 e294 a40a e294 8220 456e  ............. En
+000037b0: 6470 6f69 6e74 2020 2020 20e2 9482 2020  dpoint     ...  
+000037c0: 2020 2020 2068 7474 7073 3a2f 2f6c 616e       https://lan
+000037d0: 6763 6861 696e 2d65 6534 6165 6635 3764  gchain-ee4aef57d
+000037e0: 392d 6874 7470 2e77 6f6c 662e 6a69 6e61  9-http.wolf.jina
+000037f0: 2e61 6920 2020 2020 2020 20e2 9482 0ae2  .ai        .....
+00003800: 949c e294 80e2 9480 e294 80e2 9480 e294  ................
+00003810: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00003820: e294 80e2 9480 e294 80e2 9480 e294 bce2  ................
+00003830: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00003840: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00003850: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00003860: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00003870: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00003880: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00003890: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000038a0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000038b0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000038c0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000038d0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000038e0: e294 80e2 9480 e294 a40a e294 8220 5377  ............. Sw
+000038f0: 6167 6765 7220 5549 2020 20e2 9482 2020  agger UI   ...  
+00003900: 2020 2068 7474 7073 3a2f 2f6c 616e 6763     https://langc
+00003910: 6861 696e 2d65 6534 6165 6635 3764 392d  hain-ee4aef57d9-
+00003920: 6874 7470 2e77 6f6c 662e 6a69 6e61 2e61  http.wolf.jina.a
+00003930: 692f 646f 6373 2020 2020 20e2 9482 0ae2  i/docs     .....
+00003940: 949c e294 80e2 9480 e294 80e2 9480 e294  ................
+00003950: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00003960: e294 80e2 9480 e294 80e2 9480 e294 bce2  ................
+00003970: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00003980: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00003990: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000039a0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000039b0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000039c0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000039d0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000039e0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000039f0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00003a00: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00003a10: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00003a20: e294 80e2 9480 e294 a40a e294 8220 4f70  ............. Op
+00003a30: 656e 4150 4920 4a53 4f4e 20e2 9482 2068  enAPI JSON ... h
+00003a40: 7474 7073 3a2f 2f6c 616e 6763 6861 696e  ttps://langchain
+00003a50: 2d65 6534 6165 6635 3764 392d 6874 7470  -ee4aef57d9-http
+00003a60: 2e77 6f6c 662e 6a69 6e61 2e61 692f 6f70  .wolf.jina.ai/op
+00003a70: 656e 6170 692e 6a73 6f6e 20e2 9482 0ae2  enapi.json .....
+00003a80: 95b0 e294 80e2 9480 e294 80e2 9480 e294  ................
+00003a90: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00003aa0: e294 80e2 9480 e294 80e2 9480 e294 b4e2  ................
+00003ab0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00003ac0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00003ad0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00003ae0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00003af0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00003b00: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00003b10: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00003b20: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00003b30: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00003b40: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00003b50: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00003b60: e294 80e2 9480 e295 af0a 6060 600a 0a4c  ..........```..L
+00003b70: 6574 2773 206f 7065 6e20 7468 6520 5377  et's open the Sw
+00003b80: 6167 6765 7220 5549 2074 6f20 7465 7374  agger UI to test
+00003b90: 206f 7572 2041 5049 206f 6e20 4a69 6e61   our API on Jina
+00003ba0: 2041 4920 436c 6f75 642e 2057 6974 6820   AI Cloud. With 
+00003bb0: 6054 7279 2069 7420 6f75 7460 2062 7574  `Try it out` but
+00003bc0: 746f 6e2c 2077 6520 6361 6e20 7465 7374  ton, we can test
+00003bd0: 206f 7572 2041 5049 2077 6974 6820 6469   our API with di
+00003be0: 6666 6572 656e 7420 696e 7075 7473 2e0a  fferent inputs..
+00003bf0: 0a3c 6465 7461 696c 733e 0a3c 7375 6d6d  .<details>.<summ
+00003c00: 6172 793e 5368 6f77 2053 7761 6767 6572  ary>Show Swagger
+00003c10: 2055 493c 2f73 756d 6d61 7279 3e0a 0a3c   UI</summary>..<
+00003c20: 7020 666c 6f61 743d 2263 656e 7465 7222  p float="center"
+00003c30: 3e0a 2020 3c69 6d67 2073 7263 3d22 2e67  >.  <img src=".g
+00003c40: 6974 6875 622f 696d 6167 6573 2f6a 636c  ithub/images/jcl
+00003c50: 6f75 642d 7377 6167 6765 722d 7569 2e70  oud-swagger-ui.p
+00003c60: 6e67 2220 7769 6474 683d 2234 3030 2220  ng" width="400" 
+00003c70: 2f3e 0a20 203c 696d 6720 7372 633d 222e  />.  <img src=".
+00003c80: 6769 7468 7562 2f69 6d61 6765 732f 6a63  github/images/jc
+00003c90: 6c6f 7564 2d6f 7065 6e61 7069 2e70 6e67  loud-openapi.png
+00003ca0: 2220 7769 6474 683d 2233 3030 2220 2f3e  " width="300" />
+00003cb0: 0a3c 2f70 3e0a 0a3c 2f64 6574 6169 6c73  .</p>..</details
+00003cc0: 3e0a 0a0a 4c65 7427 7320 7465 7374 2074  >...Let's test t
+00003cd0: 6865 2041 5049 206f 6e20 4a43 6c6f 7564  he API on JCloud
+00003ce0: 2077 6974 6820 6048 6f77 206d 616e 7920   with `How many 
+00003cf0: 7065 6f70 6c65 206c 6976 6520 696e 2063  people live in c
+00003d00: 616e 6164 6120 6173 206f 6620 3230 3233  anada as of 2023
+00003d10: 3f60 2069 6e70 7574 2077 6974 6820 6120  ?` input with a 
+00003d20: 6355 524c 2063 6f6d 6d61 6e64 2028 5265  cURL command (Re
+00003d30: 706c 6163 6520 7468 6520 486f 7374 6e61  place the Hostna
+00003d40: 6d65 2077 6974 6820 796f 7572 206f 776e  me with your own
+00003d50: 2068 6f73 746e 616d 6529 3a0a 0a60 6060   hostname):..```
+00003d60: 6261 7368 0a63 7572 6c20 2d58 2027 504f  bash.curl -X 'PO
+00003d70: 5354 2720 5c0a 2020 2768 7474 7073 3a2f  ST' \.  'https:/
+00003d80: 2f6c 616e 6763 6861 696e 2d65 6534 6165  /langchain-ee4ae
+00003d90: 6635 3764 392d 6874 7470 2e77 6f6c 662e  f57d9-http.wolf.
+00003da0: 6a69 6e61 2e61 692f 6173 6b27 205c 0a20  jina.ai/ask' \. 
+00003db0: 202d 4820 2761 6363 6570 743a 2061 7070   -H 'accept: app
+00003dc0: 6c69 6361 7469 6f6e 2f6a 736f 6e27 205c  lication/json' \
+00003dd0: 0a20 202d 4820 2743 6f6e 7465 6e74 2d54  .  -H 'Content-T
+00003de0: 7970 653a 2061 7070 6c69 6361 7469 6f6e  ype: application
+00003df0: 2f6a 736f 6e27 205c 0a20 202d 6420 277b  /json' \.  -d '{
+00003e00: 0a20 2022 696e 7075 7422 3a20 2248 6f77  .  "input": "How
+00003e10: 206d 616e 7920 7065 6f70 6c65 206c 6976   many people liv
+00003e20: 6520 696e 2063 616e 6164 6120 6173 206f  e in canada as o
+00003e30: 6620 3230 3233 3f22 2c0a 2020 2265 6e76  f 2023?",.  "env
+00003e40: 7322 3a20 7b0a 2020 2020 224f 5045 4e41  s": {.    "OPENA
+00003e50: 495f 4150 495f 4b45 5922 3a20 2227 2224  I_API_KEY": "'"$
+00003e60: 7b4f 5045 4e41 495f 4150 495f 4b45 597d  {OPENAI_API_KEY}
+00003e70: 2227 222c 0a20 2020 2022 5345 5250 4150  "'",.    "SERPAP
+00003e80: 495f 4150 495f 4b45 5922 3a20 2227 2224  I_API_KEY": "'"$
+00003e90: 7b53 4552 5041 5049 5f41 5049 5f4b 4559  {SERPAPI_API_KEY
+00003ea0: 7d22 2722 0a20 207d 0a7d 270a 6060 600a  }"'".  }.}'.```.
+00003eb0: 0a60 6060 6a73 6f6e 0a7b 0a20 2022 7265  .```json.{.  "re
+00003ec0: 7375 6c74 223a 2022 4172 7272 2c20 7468  sult": "Arrr, th
+00003ed0: 6572 6520 6265 2033 382c 3634 352c 3637  ere be 38,645,67
+00003ee0: 3020 7065 6f70 6c65 206c 6976 696e 2720  0 people livin' 
+00003ef0: 696e 2043 616e 6164 6120 6173 206f 6620  in Canada as of 
+00003f00: 3230 3233 2122 2c0a 2020 2265 7272 6f72  2023!",.  "error
+00003f10: 223a 2022 222c 0a20 2022 7374 646f 7574  ": "",.  "stdout
+00003f20: 223a 2022 416e 7377 6572 2074 6865 2066  ": "Answer the f
+00003f30: 6f6c 6c6f 7769 6e67 2071 7565 7374 696f  ollowing questio
+00003f40: 6e73 2061 7320 6265 7374 2079 6f75 2063  ns as best you c
+00003f50: 616e 2c20 6275 7420 7370 6561 6b69 6e67  an, but speaking
+00003f60: 2061 7320 6120 7069 7261 7465 206d 6967   as a pirate mig
+00003f70: 6874 2073 7065 616b 2e20 596f 7520 6861  ht speak. You ha
+00003f80: 7665 2061 6363 6573 7320 746f 2074 6865  ve access to the
+00003f90: 2066 6f6c 6c6f 7769 6e67 2074 6f6f 6c73   following tools
+00003fa0: 3a5c 6e5c 6e53 6561 7263 683a 2075 7365  :\n\nSearch: use
+00003fb0: 6675 6c20 666f 7220 7768 656e 2079 6f75  ful for when you
+00003fc0: 206e 6565 6420 746f 2061 6e73 7765 7220   need to answer 
+00003fd0: 7175 6573 7469 6f6e 7320 6162 6f75 7420  questions about 
+00003fe0: 6375 7272 656e 7420 6576 656e 7473 5c6e  current events\n
+00003ff0: 5c6e 5573 6520 7468 6520 666f 6c6c 6f77  \nUse the follow
+00004000: 696e 6720 666f 726d 6174 3a5c 6e5c 6e51  ing format:\n\nQ
+00004010: 7565 7374 696f 6e3a 2074 6865 2069 6e70  uestion: the inp
+00004020: 7574 2071 7565 7374 696f 6e20 796f 7520  ut question you 
+00004030: 6d75 7374 2061 6e73 7765 725c 6e54 686f  must answer\nTho
+00004040: 7567 6874 3a20 796f 7520 7368 6f75 6c64  ught: you should
+00004050: 2061 6c77 6179 7320 7468 696e 6b20 6162   always think ab
+00004060: 6f75 7420 7768 6174 2074 6f20 646f 5c6e  out what to do\n
+00004070: 4163 7469 6f6e 3a20 7468 6520 6163 7469  Action: the acti
+00004080: 6f6e 2074 6f20 7461 6b65 2c20 7368 6f75  on to take, shou
+00004090: 6c64 2062 6520 6f6e 6520 6f66 205b 5365  ld be one of [Se
+000040a0: 6172 6368 5d5c 6e41 6374 696f 6e20 496e  arch]\nAction In
+000040b0: 7075 743a 2074 6865 2069 6e70 7574 2074  put: the input t
+000040c0: 6f20 7468 6520 6163 7469 6f6e 5c6e 4f62  o the action\nOb
+000040d0: 7365 7276 6174 696f 6e3a 2074 6865 2072  servation: the r
+000040e0: 6573 756c 7420 6f66 2074 6865 2061 6374  esult of the act
+000040f0: 696f 6e5c 6e2e 2e2e 2028 7468 6973 2054  ion\n... (this T
+00004100: 686f 7567 6874 2f41 6374 696f 6e2f 4163  hought/Action/Ac
+00004110: 7469 6f6e 2049 6e70 7574 2f4f 6273 6572  tion Input/Obser
+00004120: 7661 7469 6f6e 2063 616e 2072 6570 6561  vation can repea
+00004130: 7420 4e20 7469 6d65 7329 5c6e 5468 6f75  t N times)\nThou
+00004140: 6768 743a 2049 206e 6f77 206b 6e6f 7720  ght: I now know 
+00004150: 7468 6520 6669 6e61 6c20 616e 7377 6572  the final answer
+00004160: 5c6e 4669 6e61 6c20 416e 7377 6572 3a20  \nFinal Answer: 
+00004170: 7468 6520 6669 6e61 6c20 616e 7377 6572  the final answer
+00004180: 2074 6f20 7468 6520 6f72 6967 696e 616c   to the original
+00004190: 2069 6e70 7574 2071 7565 7374 696f 6e5c   input question\
+000041a0: 6e5c 6e42 6567 696e 2120 5265 6d65 6d62  n\nBegin! Rememb
+000041b0: 6572 2074 6f20 7370 6561 6b20 6173 2061  er to speak as a
+000041c0: 2070 6972 6174 6520 7768 656e 2067 6976   pirate when giv
+000041d0: 696e 6720 796f 7572 2066 696e 616c 2061  ing your final a
+000041e0: 6e73 7765 722e 2055 7365 206c 6f74 7320  nswer. Use lots 
+000041f0: 6f66 205c 2241 7267 735c 225c 6e5c 6e20  of \"Args\"\n\n 
+00004200: 2020 2051 7565 7374 696f 6e3a 207b 696e     Question: {in
+00004210: 7075 747d 5c6e 2020 2020 7b61 6765 6e74  put}\n    {agent
+00004220: 5f73 6372 6174 6368 7061 647d 5c6e 5c6e  _scratchpad}\n\n
+00004230: 5c6e 5c75 3030 3162 5b31 6d3e 2045 6e74  \n\u001b[1m> Ent
+00004240: 6572 696e 6720 6e65 7720 4167 656e 7445  ering new AgentE
+00004250: 7865 6375 746f 7220 6368 6169 6e2e 2e2e  xecutor chain...
+00004260: 5c75 3030 3162 5b30 6d5c 6e5c 7530 3031  \u001b[0m\n\u001
+00004270: 625b 3332 3b31 6d5c 7530 3031 625b 313b  b[32;1m\u001b[1;
+00004280: 336d 5c6e 5468 6f75 6768 743a 2049 206e  3m\nThought: I n
+00004290: 6565 6420 746f 2066 696e 6420 6f75 7420  eed to find out 
+000042a0: 686f 7720 6d61 6e79 2070 656f 706c 6520  how many people 
+000042b0: 6c69 7665 2069 6e20 4361 6e61 6461 5c6e  live in Canada\n
+000042c0: 4163 7469 6f6e 3a20 5365 6172 6368 5c6e  Action: Search\n
+000042d0: 4163 7469 6f6e 2049 6e70 7574 3a20 486f  Action Input: Ho
+000042e0: 7720 6d61 6e79 2070 656f 706c 6520 6c69  w many people li
+000042f0: 7665 2069 6e20 4361 6e61 6461 2061 7320  ve in Canada as 
+00004300: 6f66 2032 3032 335c 7530 3031 625b 306d  of 2023\u001b[0m
+00004310: 5c6e 4f62 7365 7276 6174 696f 6e3a 205c  \nObservation: \
+00004320: 7530 3031 625b 3336 3b31 6d5c 7530 3031  u001b[36;1m\u001
+00004330: 625b 313b 336d 5468 6520 6375 7272 656e  b[1;3mThe curren
+00004340: 7420 706f 7075 6c61 7469 6f6e 206f 6620  t population of 
+00004350: 4361 6e61 6461 2069 7320 3338 2c36 3435  Canada is 38,645
+00004360: 2c36 3730 2061 7320 6f66 2057 6564 6e65  ,670 as of Wedne
+00004370: 7364 6179 2c20 4d61 7263 6820 3239 2c20  sday, March 29, 
+00004380: 3230 3233 2c20 6261 7365 6420 6f6e 2057  2023, based on W
+00004390: 6f72 6c64 6f6d 6574 6572 2065 6c61 626f  orldometer elabo
+000043a0: 7261 7469 6f6e 206f 6620 7468 6520 6c61  ration of the la
+000043b0: 7465 7374 2055 6e69 7465 6420 4e61 7469  test United Nati
+000043c0: 6f6e 7320 6461 7461 2e5c 7530 3031 625b  ons data.\u001b[
+000043d0: 306d 5c6e 5468 6f75 6768 743a 5c75 3030  0m\nThought:\u00
+000043e0: 3162 5b33 323b 316d 5c75 3030 3162 5b31  1b[32;1m\u001b[1
+000043f0: 3b33 6d20 4920 6e6f 7720 6b6e 6f77 2074  ;3m I now know t
+00004400: 6865 2066 696e 616c 2061 6e73 7765 725c  he final answer\
+00004410: 6e46 696e 616c 2041 6e73 7765 723a 2041  nFinal Answer: A
+00004420: 7272 722c 2074 6865 7265 2062 6520 3338  rrr, there be 38
+00004430: 2c36 3435 2c36 3730 2070 656f 706c 6520  ,645,670 people 
+00004440: 6c69 7669 6e27 2069 6e20 4361 6e61 6461  livin' in Canada
+00004450: 2061 7320 6f66 2032 3032 3321 5c75 3030   as of 2023!\u00
+00004460: 3162 5b30 6d5c 6e5c 6e5c 7530 3031 625b  1b[0m\n\n\u001b[
+00004470: 316d 3e20 4669 6e69 7368 6564 2063 6861  1m> Finished cha
+00004480: 696e 2e5c 7530 3031 625b 306d 220a 7d0a  in.\u001b[0m".}.
+00004490: 6060 600a 0a23 2323 2323 2057 6861 7420  ```..##### What 
+000044a0: 6861 7070 656e 6564 3f0a 0a2d 2049 6e20  happened?..- In 
+000044b0: 6120 6d61 7474 6572 206f 6620 6665 7720  a matter of few 
+000044c0: 7365 636f 6e64 732c 2077 6527 7665 2064  seconds, we've d
+000044d0: 6570 6c6f 7965 6420 6f75 7220 4150 4920  eployed our API 
+000044e0: 6f6e 204a 696e 6120 4149 2043 6c6f 7564  on Jina AI Cloud
+000044f0: 20f0 9f8e 890a 2d20 5468 6520 4150 4920   .....- The API 
+00004500: 6973 2073 6572 7665 726c 6573 7320 616e  is serverless an
+00004510: 6420 7363 616c 6162 6c65 2c20 736f 2077  d scalable, so w
+00004520: 6520 6361 6e20 7363 616c 6520 7570 2074  e can scale up t
+00004530: 6865 2041 5049 2074 6f20 6861 6e64 6c65  he API to handle
+00004540: 206d 6f72 6520 7265 7175 6573 7473 2e20   more requests. 
+00004550: 0a2d 2059 6f75 206d 6967 6874 206f 6273  .- You might obs
+00004560: 6572 7665 2061 2064 656c 6179 2069 6e20  erve a delay in 
+00004570: 7468 6520 6669 7273 7420 7265 7175 6573  the first reques
+00004580: 742c 2074 6861 7427 7320 6475 6520 746f  t, that's due to
+00004590: 2074 6865 2077 6172 6d2d 7570 2074 696d   the warm-up tim
+000045a0: 6520 6f66 2074 6865 2041 5049 2e20 5375  e of the API. Su
+000045b0: 6273 6571 7565 6e74 2072 6571 7565 7374  bsequent request
+000045c0: 7320 7769 6c6c 2062 6520 6661 7374 6572  s will be faster
+000045d0: 2e0a 2d20 5468 6520 4150 4920 696e 636c  ..- The API incl
+000045e0: 7564 6573 2061 2053 7761 6767 6572 2055  udes a Swagger U
+000045f0: 4920 616e 6420 7468 6520 4f70 656e 4150  I and the OpenAP
+00004600: 4920 7370 6563 6966 6963 6174 696f 6e2c  I specification,
+00004610: 2073 6f20 6974 2063 616e 2062 6520 6561   so it can be ea
+00004620: 7369 6c79 2069 6e74 6567 7261 7465 6420  sily integrated 
+00004630: 7769 7468 206f 7468 6572 2073 6572 7669  with other servi
+00004640: 6365 732e 200a 2d20 4e6f 772c 206f 7468  ces. .- Now, oth
+00004650: 6572 2061 6765 6e74 7320 6361 6e20 696e  er agents can in
+00004660: 7465 6772 6174 6520 7769 7468 2079 6f75  tegrate with you
+00004670: 7220 6167 656e 7473 206f 6e20 4a69 6e61  r agents on Jina
+00004680: 2041 4920 436c 6f75 6420 7468 616e 6b73   AI Cloud thanks
+00004690: 2074 6f20 7468 6520 5b4f 7065 6e41 5049   to the [OpenAPI
+000046a0: 2041 6765 6e74 5d28 6874 7470 733a 2f2f   Agent](https://
+000046b0: 7079 7468 6f6e 2e6c 616e 6763 6861 696e  python.langchain
+000046c0: 2e63 6f6d 2f65 6e2f 6c61 7465 7374 2f6d  .com/en/latest/m
+000046d0: 6f64 756c 6573 2f61 6765 6e74 732f 746f  odules/agents/to
+000046e0: 6f6c 6b69 7473 2f65 7861 6d70 6c65 732f  olkits/examples/
+000046f0: 6f70 656e 6170 692e 6874 6d6c 2920 f09f  openapi.html) ..
+00004700: 92a1 0a0a 0a0a 2d2d 2d0a 0a23 2323 2320  ......---..#### 
+00004710: 5265 6163 6820 6f75 7420 746f 2075 7320  Reach out to us 
+00004720: f09f 939e 0a0a 2d20 5365 7276 6572 6c65  ......- Serverle
+00004730: 7373 2069 7320 6e6f 7420 796f 7572 2074  ss is not your t
+00004740: 6869 6e67 3f0a 2d20 446f 2079 6f75 2077  hing?.- Do you w
+00004750: 616e 7420 6c61 7267 6572 2069 6e73 7461  ant larger insta
+00004760: 6e63 6573 2066 6f72 2079 6f75 7220 4150  nces for your AP
+00004770: 493f 0a2d 204c 6f6f 6b69 6e67 2066 6f72  I?.- Looking for
+00004780: 2066 696c 6520 7570 6c6f 6164 732c 206f   file uploads, o
+00004790: 7220 6f74 6865 7220 6461 7461 2d69 6e2c  r other data-in,
+000047a0: 2064 6174 612d 6f75 7420 6665 6174 7572   data-out featur
+000047b0: 6573 3f0a 2d20 446f 2079 6f75 2077 616e  es?.- Do you wan
+000047c0: 7420 746f 2073 6574 7570 2063 7573 746f  t to setup custo
+000047d0: 6d20 6175 7468 6f72 697a 6174 696f 6e20  m authorization 
+000047e0: 666f 7220 796f 7572 2041 5049 3f0a 0a0a  for your API?...
+000047f0: f09f 93a3 2047 6f74 2079 6f75 7220 6174  .... Got your at
+00004800: 7465 6e74 696f 6e3f 205b 4a6f 696e 2075  tention? [Join u
+00004810: 7320 6f6e 2053 6c61 636b 5d28 6874 7470  s on Slack](http
+00004820: 733a 2f2f 6a69 6e61 2e61 692f 736c 6163  s://jina.ai/slac
+00004830: 6b2f 2920 616e 6420 7765 2764 2062 6520  k/) and we'd be 
+00004840: 6861 7070 7920 746f 2068 656c 7020 796f  happy to help yo
+00004850: 7520 6f75 742e 0a0a 2d2d 2d0a 0a0a 2323  u out...---...##
+00004860: 2320 606c 632d 7365 7276 6560 0a0a 606c  # `lc-serve`..`l
+00004870: 632d 7365 7276 6560 2069 7320 6120 434c  c-serve` is a CL
+00004880: 4920 746f 6f6c 2074 6861 7420 6865 6c70  I tool that help
+00004890: 7320 796f 7520 746f 2064 6570 6c6f 7920  s you to deploy 
+000048a0: 796f 7572 2061 6765 6e74 7320 6f6e 204a  your agents on J
+000048b0: 696e 6120 4149 2043 6c6f 7564 2e0a 0a0a  ina AI Cloud....
+000048c0: 7c20 4465 7363 7269 7074 696f 6e20 7c20  | Description | 
+000048d0: 436f 6d6d 616e 6420 7c20 0a7c 202d 2d2d  Command | .| ---
+000048e0: 207c 202d 2d2d 3a20 7c0a 7c20 4465 706c   | ---: |.| Depl
+000048f0: 6f79 2079 6f75 7220 6170 7020 6c6f 6361  oy your app loca
+00004900: 6c6c 7920 7c20 606c 632d 7365 7276 6520  lly | `lc-serve 
+00004910: 6465 706c 6f79 206c 6f63 616c 2061 7070  deploy local app
+00004920: 6020 7c0a 7c20 4465 706c 6f79 2079 6f75  ` |.| Deploy you
+00004930: 7220 6170 7020 6f6e 204a 696e 6120 4149  r app on Jina AI
+00004940: 2043 6c6f 7564 207c 2060 6c63 2d73 6572   Cloud | `lc-ser
+00004950: 7665 2064 6570 6c6f 7920 6a63 6c6f 7564  ve deploy jcloud
+00004960: 2061 7070 6020 7c0a 7c20 5570 6461 7465   app` |.| Update
+00004970: 2065 7869 7374 696e 6720 6170 7020 6f6e   existing app on
+00004980: 204a 696e 6120 4149 2043 6c6f 7564 207c   Jina AI Cloud |
+00004990: 2060 6c63 2d73 6572 7665 2064 6570 6c6f   `lc-serve deplo
+000049a0: 7920 6a63 6c6f 7564 2061 7070 202d 2d61  y jcloud app --a
+000049b0: 7070 2d69 6420 3c61 7070 2d69 643e 6020  pp-id <app-id>` 
+000049c0: 7c0a 7c20 4765 7420 6170 7020 7374 6174  |.| Get app stat
+000049d0: 7573 206f 6e20 4a69 6e61 2041 4920 436c  us on Jina AI Cl
+000049e0: 6f75 6420 7c20 606c 632d 7365 7276 6520  oud | `lc-serve 
+000049f0: 7374 6174 7573 203c 6170 702d 6964 3e60  status <app-id>`
+00004a00: 207c 0a7c 204c 6973 7420 616c 6c20 6170   |.| List all ap
+00004a10: 7073 206f 6e20 4a69 6e61 2041 4920 436c  ps on Jina AI Cl
+00004a20: 6f75 6420 7c20 606c 632d 7365 7276 6520  oud | `lc-serve 
+00004a30: 6c69 7374 6020 7c0a 7c20 5265 6d6f 7665  list` |.| Remove
+00004a40: 2061 7070 206f 6e20 4a69 6e61 2041 4920   app on Jina AI 
+00004a50: 436c 6f75 6420 7c20 606c 632d 7365 7276  Cloud | `lc-serv
+00004a60: 6520 7265 6d6f 7665 203c 6170 702d 6964  e remove <app-id
+00004a70: 3e60 207c 0a0a 0a2d 2d2d 0a0a 2323 2320  >` |...---..### 
+00004a80: 4167 656e 7473 2050 6c61 7967 726f 756e  Agents Playgroun
+00004a90: 6420 f09f 95b9 efb8 8ff0 9f8e aef0 9f8c  d ..............
+00004aa0: 900a 0a5b 4c61 6e67 4368 6169 6e20 6167  ...[LangChain ag
+00004ab0: 656e 7473 5d28 6874 7470 733a 2f2f 7079  ents](https://py
+00004ac0: 7468 6f6e 2e6c 616e 6763 6861 696e 2e63  thon.langchain.c
+00004ad0: 6f6d 2f65 6e2f 6c61 7465 7374 2f6d 6f64  om/en/latest/mod
+00004ae0: 756c 6573 2f61 6765 6e74 732f 6765 7474  ules/agents/gett
+00004af0: 696e 675f 7374 6172 7465 642e 6874 6d6c  ing_started.html
+00004b00: 2920 7573 6520 4c4c 4d73 2074 6f20 6465  ) use LLMs to de
+00004b10: 7465 726d 696e 6520 7468 6520 6163 7469  termine the acti
+00004b20: 6f6e 7320 746f 2062 6520 7461 6b65 6e20  ons to be taken 
+00004b30: 696e 2077 6861 7420 6f72 6465 722e 2041  in what order. A
+00004b40: 6e20 6163 7469 6f6e 2063 616e 2065 6974  n action can eit
+00004b50: 6865 7220 6265 2075 7369 6e67 2061 2074  her be using a t
+00004b60: 6f6f 6c20 616e 6420 6f62 7365 7276 696e  ool and observin
+00004b70: 6720 6974 7320 6f75 7470 7574 2c20 6f72  g its output, or
+00004b80: 2072 6574 7572 6e69 6e67 2074 6f20 7468   returning to th
+00004b90: 6520 7573 6572 2e20 5765 2776 6520 686f  e user. We've ho
+00004ba0: 7374 6564 2061 202a 2a5b 5374 7265 616d  sted a **[Stream
+00004bb0: 6c69 7420 506c 6179 6772 6f75 6e64 5d28  lit Playground](
+00004bc0: 6874 7470 733a 2f2f 6c61 6e67 6368 6169  https://langchai
+00004bd0: 6e2e 776f 6c66 2e6a 696e 612e 6169 2f70  n.wolf.jina.ai/p
+00004be0: 6c61 7967 726f 756e 642f 292a 2a20 6f6e  layground/)** on
+00004bf0: 204a 696e 6120 4149 2043 6c6f 7564 2074   Jina AI Cloud t
+00004c00: 6f20 696e 7465 7261 6374 2077 6974 6820  o interact with 
+00004c10: 7468 6520 6167 656e 7473 2c20 7768 6963  the agents, whic
+00004c20: 6820 6163 6365 7074 7320 7769 7468 2066  h accepts with f
+00004c30: 6f6c 6c6f 7769 6e67 2069 6e70 7574 733a  ollowing inputs:
+00004c40: 0a0a 2d20 2a2a 5b41 6765 6e74 2054 7970  ..- **[Agent Typ
+00004c50: 6573 5d28 6874 7470 733a 2f2f 7079 7468  es](https://pyth
+00004c60: 6f6e 2e6c 616e 6763 6861 696e 2e63 6f6d  on.langchain.com
+00004c70: 2f65 6e2f 6c61 7465 7374 2f6d 6f64 756c  /en/latest/modul
+00004c80: 6573 2f61 6765 6e74 732f 6167 656e 7473  es/agents/agents
+00004c90: 2e68 746d 6c29 3a2a 2a20 4368 6f6f 7365  .html):** Choose
+00004ca0: 2066 726f 6d20 6469 6666 6572 656e 7420   from different 
+00004cb0: 6167 656e 7420 7479 7065 7320 7468 6174  agent types that
+00004cc0: 204c 616e 6763 6861 696e 2073 7570 706f   Langchain suppo
+00004cd0: 7274 732e 200a 0a2d 202a 2a5b 546f 6f6c  rts. ..- **[Tool
+00004ce0: 735d 2868 7474 7073 3a2f 2f70 7974 686f  s](https://pytho
+00004cf0: 6e2e 6c61 6e67 6368 6169 6e2e 636f 6d2f  n.langchain.com/
+00004d00: 656e 2f6c 6174 6573 742f 6d6f 6475 6c65  en/latest/module
+00004d10: 732f 6167 656e 7473 2f74 6f6f 6c73 2e68  s/agents/tools.h
+00004d20: 746d 6c29 3a2a 2a20 4368 6f6f 7365 2066  tml):** Choose f
+00004d30: 726f 6d20 6469 6666 6572 656e 7420 746f  rom different to
+00004d40: 6f6c 7320 7468 6174 204c 616e 6763 6861  ols that Langcha
+00004d50: 696e 2073 7570 706f 7274 732e 2053 6f6d  in supports. Som
+00004d60: 6520 746f 6f6c 7320 6d61 7920 7265 7175  e tools may requ
+00004d70: 6972 6520 616e 2041 5049 2074 6f6b 656e  ire an API token
+00004d80: 206f 7220 6f74 6865 7220 7265 6c61 7465   or other relate
+00004d90: 6420 6172 6775 6d65 6e74 732e 0a0a 546f  d arguments...To
+00004da0: 2075 7365 2074 6865 2070 6c61 7967 726f   use the playgro
+00004db0: 756e 642c 2073 696d 706c 7920 7479 7065  und, simply type
+00004dc0: 2079 6f75 7220 696e 7075 7420 696e 2074   your input in t
+00004dd0: 6865 2074 6578 7420 626f 7820 7072 6f76  he text box prov
+00004de0: 6964 6564 2074 6f20 6765 7420 7468 6520  ided to get the 
+00004df0: 6167 656e 7427 7320 6f75 7470 7574 2061  agent's output a
+00004e00: 6e64 2063 6861 696e 206f 6620 7468 6f75  nd chain of thou
+00004e10: 6768 742e 2045 6e6a 6f79 2065 7870 6c6f  ght. Enjoy explo
+00004e20: 7269 6e67 204c 616e 6763 6861 696e 2773  ring Langchain's
+00004e30: 2063 6170 6162 696c 6974 6965 7321 2049   capabilities! I
+00004e40: 6e20 6164 6469 7469 6f6e 2074 6f20 7374  n addition to st
+00004e50: 7265 616d 6c69 742c 2079 6f75 2063 616e  reamlit, you can
+00004e60: 2061 6c73 6f20 7573 6520 6f75 7220 5245   also use our RE
+00004e70: 5354 6675 6c20 4150 4973 206f 6e20 7468  STful APIs on th
+00004e80: 6520 706c 6179 6772 6f75 6e64 2074 6f20  e playground to 
+00004e90: 696e 7465 7261 6374 2077 6974 6820 7468  interact with th
+00004ea0: 6520 6167 656e 7473 2e20 0a0a 0a23 2323  e agents. ...###
+00004eb0: 205b 5a65 726f 2d73 686f 7420 5265 6163   [Zero-shot Reac
+00004ec0: 7420 4465 7363 7269 7074 696f 6e20 6167  t Description ag
+00004ed0: 656e 7420 7769 7468 2053 6572 7041 5049  ent with SerpAPI
+00004ee0: 2061 6e64 2043 616c 6375 6c61 746f 725d   and Calculator]
+00004ef0: 2868 7474 7073 3a2f 2f70 7974 686f 6e2e  (https://python.
+00004f00: 6c61 6e67 6368 6169 6e2e 636f 6d2f 656e  langchain.com/en
+00004f10: 2f6c 6174 6573 742f 6d6f 6475 6c65 732f  /latest/modules/
+00004f20: 6167 656e 7473 2f67 6574 7469 6e67 5f73  agents/getting_s
+00004f30: 7461 7274 6564 2e68 746d 6c29 0a0a 2323  tarted.html)..##
+00004f40: 2323 2053 7472 6561 6d6c 6974 2050 6c61  ## Streamlit Pla
+00004f50: 7967 726f 756e 640a 0a21 5b53 7472 6561  yground..![Strea
+00004f60: 6d6c 6974 2050 6c61 7967 726f 756e 645d  mlit Playground]
+00004f70: 282e 6769 7468 7562 2f69 6d61 6765 732f  (.github/images/
+00004f80: 706c 6179 6772 6f75 6e64 5f6f 6e65 2e67  playground_one.g
+00004f90: 6966 290a 0a23 2323 2320 5245 5354 6675  if)..#### RESTfu
+00004fa0: 6c20 4150 490a 0a60 6060 6261 7368 0a65  l API..```bash.e
+00004fb0: 7870 6f72 7420 4f50 454e 4149 5f41 5049  xport OPENAI_API
+00004fc0: 5f4b 4559 3d73 6b2d 2a2a 2a0a 6578 706f  _KEY=sk-***.expo
+00004fd0: 7274 2053 4552 5041 5049 5f41 5049 5f4b  rt SERPAPI_API_K
+00004fe0: 4559 3d2a 2a2a 0a0a 6375 726c 202d 7358  EY=***..curl -sX
+00004ff0: 2050 4f53 5420 2768 7474 7073 3a2f 2f6c   POST 'https://l
+00005000: 616e 6763 6861 696e 2e77 6f6c 662e 6a69  angchain.wolf.ji
+00005010: 6e61 2e61 692f 6170 692f 7275 6e27 205c  na.ai/api/run' \
+00005020: 0a20 202d 4820 2761 6363 6570 743a 2061  .  -H 'accept: a
+00005030: 7070 6c69 6361 7469 6f6e 2f6a 736f 6e27  pplication/json'
+00005040: 205c 0a20 202d 4820 2743 6f6e 7465 6e74   \.  -H 'Content
+00005050: 2d54 7970 653a 2061 7070 6c69 6361 7469  -Type: applicati
+00005060: 6f6e 2f6a 736f 6e27 205c 0a20 202d 2d64  on/json' \.  --d
+00005070: 6174 612d 7261 7720 277b 0a20 2020 2022  ata-raw '{.    "
+00005080: 7465 7874 223a 2022 5768 6f20 6973 204c  text": "Who is L
+00005090: 656f 2044 6943 6170 7269 6f73 2067 6972  eo DiCaprios gir
+000050a0: 6c66 7269 656e 643f 2057 6861 7420 6973  lfriend? What is
+000050b0: 2068 6572 2063 7572 7265 6e74 2061 6765   her current age
+000050c0: 2072 6169 7365 6420 746f 2074 6865 2030   raised to the 0
+000050d0: 2e34 3320 706f 7765 723f 222c 0a20 2020  .43 power?",.   
+000050e0: 2022 7061 7261 6d65 7465 7273 223a 207b   "parameters": {
+000050f0: 0a20 2020 2020 2020 2022 746f 6f6c 7322  .        "tools"
+00005100: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
+00005110: 2274 6f6f 6c5f 6e61 6d65 7322 3a20 5b22  "tool_names": ["
+00005120: 7365 7270 6170 6922 2c20 226c 6c6d 2d6d  serpapi", "llm-m
+00005130: 6174 6822 5d0a 2020 2020 2020 2020 7d2c  ath"].        },
+00005140: 0a20 2020 2020 2020 2022 6167 656e 7422  .        "agent"
+00005150: 3a20 227a 6572 6f2d 7368 6f74 2d72 6561  : "zero-shot-rea
+00005160: 6374 2d64 6573 6372 6970 7469 6f6e 222c  ct-description",
+00005170: 0a20 2020 2020 2020 2022 7665 7262 6f73  .        "verbos
+00005180: 6522 3a20 7472 7565 0a20 2020 207d 2c0a  e": true.    },.
+00005190: 2020 2020 2265 6e76 7322 3a20 7b0a 2020      "envs": {.  
+000051a0: 2020 2020 2020 224f 5045 4e41 495f 4150        "OPENAI_AP
+000051b0: 495f 4b45 5922 3a20 2227 2224 7b4f 5045  I_KEY": "'"${OPE
+000051c0: 4e41 495f 4150 495f 4b45 597d 2227 222c  NAI_API_KEY}"'",
+000051d0: 0a20 2020 2020 2020 2022 5345 5250 4150  .        "SERPAP
+000051e0: 495f 4150 495f 4b45 5922 3a20 2227 2224  I_API_KEY": "'"$
+000051f0: 7b53 4552 5041 5049 5f41 5049 5f4b 4559  {SERPAPI_API_KEY
+00005200: 7d22 2722 0a20 2020 207d 0a7d 2720 7c20  }"'".    }.}' | 
+00005210: 6a71 0a60 6060 200a 0a60 6060 6a73 6f6e  jq.``` ..```json
+00005220: 0a7b 0a20 2022 7265 7375 6c74 223a 2022  .{.  "result": "
+00005230: 4361 6d69 6c61 204d 6f72 726f 6e65 2069  Camila Morrone i
+00005240: 7320 4c65 6f20 4469 4361 7072 696f 2773  s Leo DiCaprio's
+00005250: 2067 6972 6c66 7269 656e 642c 2061 6e64   girlfriend, and
+00005260: 2068 6572 2063 7572 7265 6e74 2061 6765   her current age
+00005270: 2072 6169 7365 6420 746f 2074 6865 2030   raised to the 0
+00005280: 2e34 3320 706f 7765 7220 6973 2033 2e36  .43 power is 3.6
+00005290: 3236 3132 3630 3631 3135 3239 3532 372e  261260611529527.
+000052a0: 222c 0a20 2022 6368 6169 6e5f 6f66 5f74  ",.  "chain_of_t
+000052b0: 686f 7567 6874 223a 2022 5c75 3030 3162  hought": "\u001b
+000052c0: 5b31 6d3e 2045 6e74 6572 696e 6720 6e65  [1m> Entering ne
+000052d0: 7720 4167 656e 7445 7865 6375 746f 7220  w AgentExecutor 
+000052e0: 6368 6169 6e2e 2e2e 5c75 3030 3162 5b30  chain...\u001b[0
+000052f0: 6d5c 7530 3031 625b 3332 3b31 6d5c 7530  m\u001b[32;1m\u0
+00005300: 3031 625b 313b 336d 2049 206e 6565 6420  01b[1;3m I need 
+00005310: 746f 2066 696e 6420 6f75 7420 7468 6520  to find out the 
+00005320: 6e61 6d65 206f 6620 4c65 6f27 7320 6769  name of Leo's gi
+00005330: 726c 6672 6965 6e64 2061 6e64 2074 6865  rlfriend and the
+00005340: 6e20 7573 6520 7468 6520 6361 6c63 756c  n use the calcul
+00005350: 6174 6f72 2074 6f20 6361 6c63 756c 6174  ator to calculat
+00005360: 6520 6865 7220 6167 6520 746f 2074 6865  e her age to the
+00005370: 2030 2e34 3320 706f 7765 722e 4163 7469   0.43 power.Acti
+00005380: 6f6e 3a20 5365 6172 6368 4163 7469 6f6e  on: SearchAction
+00005390: 2049 6e70 7574 3a20 4c65 6f20 4469 4361   Input: Leo DiCa
+000053a0: 7072 696f 2067 6972 6c66 7269 656e 645c  prio girlfriend\
+000053b0: 7530 3031 625b 306d 4f62 7365 7276 6174  u001b[0mObservat
+000053c0: 696f 6e3a 205c 7530 3031 625b 3336 3b31  ion: \u001b[36;1
+000053d0: 6d5c 7530 3031 625b 313b 336d 4469 4361  m\u001b[1;3mDiCa
+000053e0: 7072 696f 206d 6574 2061 6374 6f72 2043  prio met actor C
+000053f0: 616d 696c 6120 4d6f 7272 6f6e 6520 696e  amila Morrone in
+00005400: 2044 6563 656d 6265 7220 3230 3137 2c20   December 2017, 
+00005410: 7768 656e 2073 6865 2077 6173 2032 3020  when she was 20 
+00005420: 616e 6420 6865 2077 6173 2034 332e 2054  and he was 43. T
+00005430: 6865 7920 7765 7265 2073 706f 7474 6564  hey were spotted
+00005440: 2061 7420 436f 6163 6865 6c6c 6120 616e   at Coachella an
+00005450: 6420 7765 6e74 206f 6e20 6d75 6c74 6970  d went on multip
+00005460: 6c65 2076 6163 6174 696f 6e73 2074 6f67  le vacations tog
+00005470: 6574 6865 722e 2053 6f6d 6520 7265 706f  ether. Some repo
+00005480: 7274 7320 7375 6767 6573 7465 6420 7468  rts suggested th
+00005490: 6174 2044 6943 6170 7269 6f20 7761 7320  at DiCaprio was 
+000054a0: 7265 6164 7920 746f 2061 736b 204d 6f72  ready to ask Mor
+000054b0: 726f 6e65 2074 6f20 6d61 7272 7920 6869  rone to marry hi
+000054c0: 6d2e 2054 6865 2063 6f75 706c 6520 6d61  m. The couple ma
+000054d0: 6465 2074 6865 6972 2072 6564 2063 6172  de their red car
+000054e0: 7065 7420 6465 6275 7420 6174 2074 6865  pet debut at the
+000054f0: 2032 3032 3020 4163 6164 656d 7920 4177   2020 Academy Aw
+00005500: 6172 6473 2e5c 7530 3031 625b 306d 5468  ards.\u001b[0mTh
+00005510: 6f75 6768 743a 5c75 3030 3162 5b33 323b  ought:\u001b[32;
+00005520: 316d 5c75 3030 3162 5b31 3b33 6d20 4920  1m\u001b[1;3m I 
+00005530: 6e65 6564 2074 6f20 7573 6520 7468 6520  need to use the 
+00005540: 6361 6c63 756c 6174 6f72 2074 6f20 6361  calculator to ca
+00005550: 6c63 756c 6174 6520 6865 7220 6167 6520  lculate her age 
+00005560: 746f 2074 6865 2030 2e34 3320 706f 7765  to the 0.43 powe
+00005570: 7241 6374 696f 6e3a 2043 616c 6375 6c61  rAction: Calcula
+00005580: 746f 7241 6374 696f 6e20 496e 7075 743a  torAction Input:
+00005590: 2032 305e 302e 3433 5c75 3030 3162 5b30   20^0.43\u001b[0
+000055a0: 6d4f 6273 6572 7661 7469 6f6e 3a20 5c75  mObservation: \u
+000055b0: 3030 3162 5b33 333b 316d 5c75 3030 3162  001b[33;1m\u001b
+000055c0: 5b31 3b33 6d41 6e73 7765 723a 2033 2e36  [1;3mAnswer: 3.6
+000055d0: 3236 3132 3630 3631 3135 3239 3532 375c  261260611529527\
+000055e0: 7530 3031 625b 306d 5468 6f75 6768 743a  u001b[0mThought:
+000055f0: 5c75 3030 3162 5b33 323b 316d 5c75 3030  \u001b[32;1m\u00
+00005600: 3162 5b31 3b33 6d20 4920 6e6f 7720 6b6e  1b[1;3m I now kn
+00005610: 6f77 2074 6865 2066 696e 616c 2061 6e73  ow the final ans
+00005620: 7765 7246 696e 616c 2041 6e73 7765 723a  werFinal Answer:
+00005630: 2043 616d 696c 6120 4d6f 7272 6f6e 6520   Camila Morrone 
+00005640: 6973 204c 656f 2044 6943 6170 7269 6f27  is Leo DiCaprio'
+00005650: 7320 6769 726c 6672 6965 6e64 2c20 616e  s girlfriend, an
+00005660: 6420 6865 7220 6375 7272 656e 7420 6167  d her current ag
+00005670: 6520 7261 6973 6564 2074 6f20 7468 6520  e raised to the 
+00005680: 302e 3433 2070 6f77 6572 2069 7320 332e  0.43 power is 3.
+00005690: 3632 3631 3236 3036 3131 3532 3935 3237  6261260611529527
+000056a0: 2e5c 7530 3031 625b 306d 5c75 3030 3162  .\u001b[0m\u001b
+000056b0: 5b31 6d3e 2046 696e 6973 6865 6420 6368  [1m> Finished ch
+000056c0: 6169 6e2e 5c75 3030 3162 5b30 6d22 0a7d  ain.\u001b[0m".}
+000056d0: 0a60 6060 0a0a 2323 2320 5b53 656c 6620  .```..### [Self 
+000056e0: 4173 6b20 5769 7468 2053 6561 7263 685d  Ask With Search]
+000056f0: 2868 7474 7073 3a2f 2f70 7974 686f 6e2e  (https://python.
+00005700: 6c61 6e67 6368 6169 6e2e 636f 6d2f 656e  langchain.com/en
+00005710: 2f6c 6174 6573 742f 6d6f 6475 6c65 732f  /latest/modules/
+00005720: 6167 656e 7473 2f69 6d70 6c65 6d65 6e74  agents/implement
+00005730: 6174 696f 6e73 2f73 656c 665f 6173 6b5f  ations/self_ask_
+00005740: 7769 7468 5f73 6561 7263 682e 6874 6d6c  with_search.html
+00005750: 290a 0a23 2323 2320 5374 7265 616d 6c69  )..#### Streamli
+00005760: 7420 506c 6179 6772 6f75 6e64 0a0a 215b  t Playground..![
+00005770: 5374 7265 616d 6c69 7420 506c 6179 6772  Streamlit Playgr
+00005780: 6f75 6e64 5d28 2e67 6974 6875 622f 696d  ound](.github/im
+00005790: 6167 6573 2f70 6c61 7967 726f 756e 645f  ages/playground_
+000057a0: 7477 6f2e 6769 6629 0a0a 2323 2323 2052  two.gif)..#### R
+000057b0: 4553 5466 756c 2041 5049 0a0a 6060 6062  ESTful API..```b
+000057c0: 6173 680a 6578 706f 7274 204f 5045 4e41  ash.export OPENA
+000057d0: 495f 4150 495f 4b45 593d 736b 2d2a 2a2a  I_API_KEY=sk-***
+000057e0: 0a65 7870 6f72 7420 5345 5250 4150 495f  .export SERPAPI_
+000057f0: 4150 495f 4b45 593d 2a2a 2a0a 0a63 7572  API_KEY=***..cur
+00005800: 6c20 2d73 5820 504f 5354 2027 6874 7470  l -sX POST 'http
+00005810: 733a 2f2f 6c61 6e67 6368 6169 6e2e 776f  s://langchain.wo
+00005820: 6c66 2e6a 696e 612e 6169 2f61 7069 2f72  lf.jina.ai/api/r
+00005830: 756e 2720 5c0a 2020 2d48 2027 6163 6365  un' \.  -H 'acce
+00005840: 7074 3a20 6170 706c 6963 6174 696f 6e2f  pt: application/
+00005850: 6a73 6f6e 2720 5c0a 2020 2d48 2027 436f  json' \.  -H 'Co
+00005860: 6e74 656e 742d 5479 7065 3a20 6170 706c  ntent-Type: appl
+00005870: 6963 6174 696f 6e2f 6a73 6f6e 2720 5c0a  ication/json' \.
+00005880: 2020 2d2d 6461 7461 2d72 6177 2027 7b0a    --data-raw '{.
+00005890: 2020 2020 2274 6578 7422 3a20 2257 6861      "text": "Wha
+000058a0: 7420 6973 2074 6865 2068 6f6d 6574 6f77  t is the hometow
+000058b0: 6e20 6f66 2074 6865 2072 6569 676e 696e  n of the reignin
+000058c0: 6720 6d65 6e73 2055 2e53 2e20 4f70 656e  g mens U.S. Open
+000058d0: 2063 6861 6d70 696f 6e3f 222c 0a20 2020   champion?",.   
+000058e0: 2022 7061 7261 6d65 7465 7273 223a 207b   "parameters": {
+000058f0: 0a20 2020 2020 2020 2022 746f 6f6c 7322  .        "tools"
+00005900: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
+00005910: 2274 6f6f 6c5f 6e61 6d65 7322 3a20 5b22  "tool_names": ["
+00005920: 7365 7270 6170 6922 5d0a 2020 2020 2020  serpapi"].      
+00005930: 2020 7d2c 0a20 2020 2020 2020 2022 6167    },.        "ag
+00005940: 656e 7422 3a20 2273 656c 662d 6173 6b2d  ent": "self-ask-
+00005950: 7769 7468 2d73 6561 7263 6822 2c0a 2020  with-search",.  
+00005960: 2020 2020 2020 2276 6572 626f 7365 223a        "verbose":
+00005970: 2074 7275 650a 2020 2020 7d2c 0a20 2020   true.    },.   
+00005980: 2022 656e 7673 223a 207b 0a20 2020 2020   "envs": {.     
+00005990: 2020 2022 4f50 454e 4149 5f41 5049 5f4b     "OPENAI_API_K
+000059a0: 4559 223a 2022 2722 247b 4f50 454e 4149  EY": "'"${OPENAI
+000059b0: 5f41 5049 5f4b 4559 7d22 2722 2c0a 2020  _API_KEY}"'",.  
+000059c0: 2020 2020 2020 2253 4552 5041 5049 5f41        "SERPAPI_A
+000059d0: 5049 5f4b 4559 223a 2022 2722 247b 5345  PI_KEY": "'"${SE
+000059e0: 5250 4150 495f 4150 495f 4b45 597d 2227  RPAPI_API_KEY}"'
+000059f0: 220a 2020 2020 7d0a 7d27 207c 206a 710a  ".    }.}' | jq.
+00005a00: 6060 600a 0a60 6060 6a73 6f6e 0a7b 0a20  ```..```json.{. 
+00005a10: 2022 7265 7375 6c74 223a 2022 456c 2050   "result": "El P
+00005a20: 616c 6d61 722c 204d 7572 6369 612c 2053  almar, Murcia, S
+00005a30: 7061 696e 222c 0a20 2022 6368 6169 6e5f  pain",.  "chain_
+00005a40: 6f66 5f74 686f 7567 6874 223a 2022 5c75  of_thought": "\u
+00005a50: 3030 3162 5b31 6d3e 2045 6e74 6572 696e  001b[1m> Enterin
+00005a60: 6720 6e65 7720 4167 656e 7445 7865 6375  g new AgentExecu
+00005a70: 746f 7220 6368 6169 6e2e 2e2e 5c75 3030  tor chain...\u00
+00005a80: 3162 5b30 6d5c 7530 3031 625b 3332 3b31  1b[0m\u001b[32;1
+00005a90: 6d5c 7530 3031 625b 313b 336d 2059 6573  m\u001b[1;3m Yes
+00005aa0: 2e46 6f6c 6c6f 7720 7570 3a20 5768 6f20  .Follow up: Who 
+00005ab0: 6973 2074 6865 2072 6569 676e 696e 6720  is the reigning 
+00005ac0: 6d65 6e73 2055 2e53 2e20 4f70 656e 2063  mens U.S. Open c
+00005ad0: 6861 6d70 696f 6e3f 5c75 3030 3162 5b30  hampion?\u001b[0
+00005ae0: 6d49 6e74 6572 6d65 6469 6174 6520 616e  mIntermediate an
+00005af0: 7377 6572 3a20 5c75 3030 3162 5b33 363b  swer: \u001b[36;
+00005b00: 316d 5c75 3030 3162 5b31 3b33 6d43 6172  1m\u001b[1;3mCar
+00005b10: 6c6f 7320 416c 6361 7261 7a20 4761 7266  los Alcaraz Garf
+00005b20: 6961 5c75 3030 3162 5b30 6d5c 7530 3031  ia\u001b[0m\u001
+00005b30: 625b 3332 3b31 6d5c 7530 3031 625b 313b  b[32;1m\u001b[1;
+00005b40: 336d 466f 6c6c 6f77 2075 703a 2057 6861  3mFollow up: Wha
+00005b50: 7420 6973 2043 6172 6c6f 7320 416c 6361  t is Carlos Alca
+00005b60: 7261 7a20 4761 7266 6961 2773 2068 6f6d  raz Garfia's hom
+00005b70: 6574 6f77 6e3f 5c75 3030 3162 5b30 6d49  etown?\u001b[0mI
+00005b80: 6e74 6572 6d65 6469 6174 6520 616e 7377  ntermediate answ
+00005b90: 6572 3a20 5c75 3030 3162 5b33 363b 316d  er: \u001b[36;1m
+00005ba0: 5c75 3030 3162 5b31 3b33 6d43 6172 6c6f  \u001b[1;3mCarlo
+00005bb0: 7320 416c 6361 7261 7a20 4761 7266 6961  s Alcaraz Garfia
+00005bc0: 2077 6173 2062 6f72 6e20 6f6e 204d 6179   was born on May
+00005bd0: 2035 2c20 3230 3033 2c20 696e 2045 6c20   5, 2003, in El 
+00005be0: 5061 6c6d 6172 2c20 4d75 7263 6961 2c20  Palmar, Murcia, 
+00005bf0: 5370 6169 6e20 746f 2070 6172 656e 7473  Spain to parents
+00005c00: 2043 6172 6c6f 7320 416c 6361 7261 7a20   Carlos Alcaraz 
+00005c10: 476f 6e7a c3a1 6c65 7a20 616e 6420 5669  Gonz..lez and Vi
+00005c20: 7267 696e 6961 2047 6172 6669 6120 4573  rginia Garfia Es
+00005c30: 6361 6e64 c3b3 6e2e 2048 6520 6861 7320  cand..n. He has 
+00005c40: 7468 7265 6520 7369 626c 696e 6773 2e5c  three siblings.\
+00005c50: 7530 3031 625b 306d 5c75 3030 3162 5b33  u001b[0m\u001b[3
+00005c60: 323b 316d 5c75 3030 3162 5b31 3b33 6d53  2;1m\u001b[1;3mS
+00005c70: 6f20 7468 6520 6669 6e61 6c20 616e 7377  o the final answ
+00005c80: 6572 2069 733a 2045 6c20 5061 6c6d 6172  er is: El Palmar
+00005c90: 2c20 4d75 7263 6961 2c20 5370 6169 6e5c  , Murcia, Spain\
+00005ca0: 7530 3031 625b 306d 5c75 3030 3162 5b31  u001b[0m\u001b[1
+00005cb0: 6d3e 2046 696e 6973 6865 6420 6368 6169  m> Finished chai
+00005cc0: 6e2e 5c75 3030 3162 5b30 6d22 0a7d 0a60  n.\u001b[0m".}.`
+00005cd0: 6060 0a0a 2d2d 2d0a 0a23 2320 4368 6169  ``..---..## Chai
+00005ce0: 6e73 206f 6e20 4a69 6e61 20f0 9f93 a6f0  ns on Jina .....
+00005cf0: 9f9a 800a 0a5b 4368 6169 6e73 5d28 6874  .....[Chains](ht
+00005d00: 7470 733a 2f2f 7079 7468 6f6e 2e6c 616e  tps://python.lan
+00005d10: 6763 6861 696e 2e63 6f6d 2f65 6e2f 6c61  gchain.com/en/la
+00005d20: 7465 7374 2f6d 6f64 756c 6573 2f63 6861  test/modules/cha
+00005d30: 696e 732f 6765 7474 696e 675f 7374 6172  ins/getting_star
+00005d40: 7465 642e 6874 6d6c 2920 696e 204c 616e  ted.html) in Lan
+00005d50: 6743 6861 696e 2061 6c6c 6f77 2075 7365  gChain allow use
+00005d60: 7273 2074 6f20 636f 6d62 696e 6520 636f  rs to combine co
+00005d70: 6d70 6f6e 656e 7473 2074 6f20 6372 6561  mponents to crea
+00005d80: 7465 2061 2073 696e 676c 652c 2063 6f68  te a single, coh
+00005d90: 6572 656e 7420 6170 706c 6963 6174 696f  erent applicatio
+00005da0: 6e2e 2057 6974 6820 4a69 6e61 2c20 0a0a  n. With Jina, ..
+00005db0: 2d20 596f 7520 6361 6e20 6578 706f 7365  - You can expose
+00005dc0: 2079 6f75 7220 6043 6861 696e 6020 6173   your `Chain` as
+00005dd0: 2052 4553 5466 756c 2f67 5250 432f 5765   RESTful/gRPC/We
+00005de0: 6253 6f63 6b65 7420 4150 492e 0a2d 2045  bSocket API..- E
+00005df0: 6e61 626c 6520 6043 6861 696e 6073 2074  nable `Chain`s t
+00005e00: 6f20 6465 706c 6f79 2026 2073 6361 6c65  o deploy & scale
+00005e10: 2073 6570 6172 6174 656c 7920 6672 6f6d   separately from
+00005e20: 2074 6865 2072 6573 7420 6f66 2079 6f75   the rest of you
+00005e30: 7220 6170 706c 6963 6174 696f 6e20 7769  r application wi
+00005e40: 7468 2074 6865 2068 656c 7020 6f66 2045  th the help of E
+00005e50: 7865 6375 746f 7273 2e0a 2d20 4465 706c  xecutors..- Depl
+00005e60: 6f79 2079 6f75 7220 6043 6861 696e 6020  oy your `Chain` 
+00005e70: 6f6e 204a 696e 6120 4149 2043 6c6f 7564  on Jina AI Cloud
+00005e80: 2061 6e64 2067 6574 2065 7863 6c75 7369   and get exclusi
+00005e90: 7665 2061 6363 6573 7320 746f 2041 6765  ve access to Age
+00005ea0: 6e74 7320 6f6e 204a 696e 6120 4149 2043  nts on Jina AI C
+00005eb0: 6c6f 7564 2028 636f 6d69 6e67 2073 6f6f  loud (coming soo
+00005ec0: 6e29 0a0a 2323 2320 4578 616d 706c 6573  n)..### Examples
+00005ed0: 0a0a 7c20 4578 616d 706c 6520 7c20 4c61  ..| Example | La
+00005ee0: 6e67 4368 6169 6e20 446f 6373 207c 2044  ngChain Docs | D
+00005ef0: 6573 6372 6970 7469 6f6e 207c 0a7c 202d  escription |.| -
+00005f00: 2d2d 2d2d 2d2d 207c 202d 2d2d 2d2d 2d2d  ------ | -------
+00005f10: 2d2d 2d2d 207c 202d 2d2d 2d2d 2d2d 2d2d  ---- | ---------
+00005f20: 2d2d 207c 0a7c 205b 4c4c 4d20 4368 6169  -- |.| [LLM Chai
+00005f30: 6e5d 2865 7861 6d70 6c65 732f 6c6c 6d5f  n](examples/llm_
+00005f40: 6368 6169 6e2e 6d64 2920 7c20 5b4c 696e  chain.md) | [Lin
+00005f50: 6b5d 2868 7474 7073 3a2f 2f6c 616e 6763  k](https://langc
+00005f60: 6861 696e 2e72 6561 6474 6865 646f 6373  hain.readthedocs
+00005f70: 2e69 6f2f 656e 2f6c 6174 6573 742f 6d6f  .io/en/latest/mo
+00005f80: 6475 6c65 732f 6368 6169 6e73 2f67 6574  dules/chains/get
+00005f90: 7469 6e67 5f73 7461 7274 6564 2e68 746d  ting_started.htm
+00005fa0: 6c23 7175 6572 792d 616e 2d6c 6c6d 2d77  l#query-an-llm-w
+00005fb0: 6974 682d 7468 652d 6c6c 6d63 6861 696e  ith-the-llmchain
+00005fc0: 2920 7c20 4578 706f 7365 2060 4368 6169  ) | Expose `Chai
+00005fd0: 6e60 2061 7320 5245 5354 6675 6c2f 6752  n` as RESTful/gR
+00005fe0: 5043 2f57 6562 536f 636b 6574 2041 5049  PC/WebSocket API
+00005ff0: 206c 6f63 616c 6c79 207c 0a7c 205b 5369   locally |.| [Si
+00006000: 6d70 6c65 2053 6571 7565 6e74 6961 6c20  mple Sequential 
+00006010: 4368 6169 6e5d 2865 7861 6d70 6c65 732f  Chain](examples/
+00006020: 7369 6d70 6c65 5f73 6571 7565 6e74 6961  simple_sequentia
+00006030: 6c5f 6368 6169 6e2e 6d64 2920 7c20 5b4c  l_chain.md) | [L
+00006040: 696e 6b5d 2868 7474 7073 3a2f 2f6c 616e  ink](https://lan
+00006050: 6763 6861 696e 2e72 6561 6474 6865 646f  gchain.readthedo
+00006060: 6373 2e69 6f2f 656e 2f6c 6174 6573 742f  cs.io/en/latest/
+00006070: 6d6f 6475 6c65 732f 6368 6169 6e73 2f67  modules/chains/g
+00006080: 656e 6572 6963 2f73 6571 7565 6e74 6961  eneric/sequentia
+00006090: 6c5f 6368 6169 6e73 2e68 746d 6c23 7369  l_chains.html#si
+000060a0: 6d70 6c65 7365 7175 656e 7469 616c 6368  mplesequentialch
+000060b0: 6169 6e29 207c 2045 7870 6f73 6520 6043  ain) | Expose `C
+000060c0: 6861 696e 6020 6173 2052 4553 5466 756c  hain` as RESTful
+000060d0: 2f67 5250 432f 5765 6253 6f63 6b65 7420  /gRPC/WebSocket 
+000060e0: 4150 4920 6c6f 6361 6c6c 7920 7c0a 7c20  API locally |.| 
+000060f0: 5b53 6571 7565 6e74 6961 6c20 4368 6169  [Sequential Chai
+00006100: 6e5d 2865 7861 6d70 6c65 732f 7365 7175  n](examples/sequ
+00006110: 656e 7469 616c 5f63 6861 696e 2e6d 6429  ential_chain.md)
+00006120: 207c 205b 4c69 6e6b 5d28 6874 7470 733a   | [Link](https:
+00006130: 2f2f 6c61 6e67 6368 6169 6e2e 7265 6164  //langchain.read
+00006140: 7468 6564 6f63 732e 696f 2f65 6e2f 6c61  thedocs.io/en/la
+00006150: 7465 7374 2f6d 6f64 756c 6573 2f63 6861  test/modules/cha
+00006160: 696e 732f 6765 6e65 7269 632f 7365 7175  ins/generic/sequ
+00006170: 656e 7469 616c 5f63 6861 696e 732e 6874  ential_chains.ht
+00006180: 6d6c 2373 6571 7565 6e74 6961 6c2d 6368  ml#sequential-ch
+00006190: 6169 6e29 207c 2045 7870 6f73 6520 6043  ain) | Expose `C
+000061a0: 6861 696e 6020 6173 2052 4553 5466 756c  hain` as RESTful
+000061b0: 2f67 5250 432f 5765 6253 6f63 6b65 7420  /gRPC/WebSocket 
+000061c0: 4150 4920 6c6f 6361 6c6c 7920 7c0a 7c20  API locally |.| 
+000061d0: 5b4c 4c4d 204d 6174 6820 4368 6169 6e5d  [LLM Math Chain]
+000061e0: 2865 7861 6d70 6c65 732f 6c6c 6d5f 6d61  (examples/llm_ma
+000061f0: 7468 2e6d 6429 207c 205b 4c69 6e6b 5d28  th.md) | [Link](
+00006200: 6874 7470 733a 2f2f 6c61 6e67 6368 6169  https://langchai
+00006210: 6e2e 7265 6164 7468 6564 6f63 732e 696f  n.readthedocs.io
+00006220: 2f65 6e2f 6c61 7465 7374 2f6d 6f64 756c  /en/latest/modul
+00006230: 6573 2f63 6861 696e 732f 6578 616d 706c  es/chains/exampl
+00006240: 6573 2f6c 6c6d 5f6d 6174 682e 6874 6d6c  es/llm_math.html
+00006250: 2920 7c20 4578 706f 7365 2060 4368 6169  ) | Expose `Chai
+00006260: 6e60 2061 7320 5245 5354 6675 6c2f 6752  n` as RESTful/gR
+00006270: 5043 2f57 6562 536f 636b 6574 2041 5049  PC/WebSocket API
+00006280: 206c 6f63 616c 6c79 207c 0a7c 205b 4c4c   locally |.| [LL
+00006290: 4d20 5265 7175 6573 7473 2043 6861 696e  M Requests Chain
+000062a0: 5d28 6578 616d 706c 6573 2f6c 6c6d 5f72  ](examples/llm_r
+000062b0: 6571 7565 7374 735f 6368 6169 6e2e 6d64  equests_chain.md
+000062c0: 2920 7c20 5b4c 696e 6b5d 2868 7474 7073  ) | [Link](https
+000062d0: 3a2f 2f6c 616e 6763 6861 696e 2e72 6561  ://langchain.rea
+000062e0: 6474 6865 646f 6373 2e69 6f2f 656e 2f6c  dthedocs.io/en/l
+000062f0: 6174 6573 742f 6d6f 6475 6c65 732f 6368  atest/modules/ch
+00006300: 6169 6e73 2f65 7861 6d70 6c65 732f 6c6c  ains/examples/ll
+00006310: 6d5f 7265 7175 6573 7473 2e68 746d 6c29  m_requests.html)
+00006320: 207c 2045 7870 6f73 6520 6043 6861 696e   | Expose `Chain
+00006330: 6020 6173 2052 4553 5466 756c 2f67 5250  ` as RESTful/gRP
+00006340: 432f 5765 6253 6f63 6b65 7420 4150 4920  C/WebSocket API 
+00006350: 6c6f 6361 6c6c 7920 7c0a 7c20 5b43 7573  locally |.| [Cus
+00006360: 746f 6d20 4368 6169 6e5d 2865 7861 6d70  tom Chain](examp
+00006370: 6c65 732f 6375 7374 6f6d 5f63 6861 696e  les/custom_chain
+00006380: 2e6d 6429 207c 205b 4c69 6e6b 5d28 6874  .md) | [Link](ht
+00006390: 7470 733a 2f2f 6c61 6e67 6368 6169 6e2e  tps://langchain.
+000063a0: 7265 6164 7468 6564 6f63 732e 696f 2f65  readthedocs.io/e
+000063b0: 6e2f 6c61 7465 7374 2f6d 6f64 756c 6573  n/latest/modules
+000063c0: 2f63 6861 696e 732f 6765 7474 696e 675f  /chains/getting_
+000063d0: 7374 6172 7465 642e 6874 6d6c 2363 7265  started.html#cre
+000063e0: 6174 652d 612d 6375 7374 6f6d 2d63 6861  ate-a-custom-cha
+000063f0: 696e 2d77 6974 682d 7468 652d 6368 6169  in-with-the-chai
+00006400: 6e2d 636c 6173 7329 207c 2045 7870 6f73  n-class) | Expos
+00006410: 6520 6043 6861 696e 6020 6173 2052 4553  e `Chain` as RES
+00006420: 5466 756c 2f67 5250 432f 5765 6253 6f63  Tful/gRPC/WebSoc
+00006430: 6b65 7420 4150 4920 6c6f 6361 6c6c 7920  ket API locally 
+00006440: 7c0a 7c20 5b53 6571 7565 6e74 6961 6c20  |.| [Sequential 
+00006450: 4368 6169 6e73 5d28 6578 616d 706c 6573  Chains](examples
+00006460: 2f73 6571 7565 6e74 6961 6c5f 6578 6563  /sequential_exec
+00006470: 7574 6f72 732e 6d64 2920 7c20 4e2f 4120  utors.md) | N/A 
+00006480: 7c20 4275 696c 6420 2620 7363 616c 6520  | Build & scale 
+00006490: 6043 6861 696e 7360 2069 6e20 7365 7061  `Chains` in sepa
+000064a0: 7261 7465 2060 4578 6563 7574 6f72 6073  rate `Executor`s
+000064b0: 207c 0a7c 205b 4272 616e 6368 696e 6720   |.| [Branching 
+000064c0: 4368 6169 6e73 5d28 6578 616d 706c 6573  Chains](examples
+000064d0: 2f62 7261 6e63 6869 6e67 2e6d 6429 207c  /branching.md) |
+000064e0: 204e 2f41 207c 2042 7261 6e63 6869 6e67   N/A | Branching
+000064f0: 2060 4368 6169 6e73 6020 696e 2073 6570   `Chains` in sep
+00006500: 6172 6174 6520 6045 7865 6375 746f 7260  arate `Executor`
+00006510: 7320 746f 2061 6c6c 6f77 2070 6172 616c  s to allow paral
+00006520: 6c65 6c20 6578 6563 7574 696f 6e20 7c0a  lel execution |.
+00006530: 0a                                       .
```

### Comparing `langchain-serve-0.0.9.dev22/langchain_serve.egg-info/PKG-INFO` & `langchain-serve-0.0.9.dev9/langchain_serve.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,1801 +1,1698 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6c61 6e67  : 2.1.Name: lang
 00000020: 6368 6169 6e2d 7365 7276 650a 5665 7273  chain-serve.Vers
-00000030: 696f 6e3a 2030 2e30 2e39 2e64 6576 3232  ion: 0.0.9.dev22
-00000040: 0a53 756d 6d61 7279 3a20 4c61 6e67 6368  .Summary: Langch
-00000050: 6169 6e20 5365 7276 6520 2d20 7365 7276  ain Serve - serv
-00000060: 6520 796f 7572 206c 616e 6763 6861 696e  e your langchain
-00000070: 2061 7070 7320 6f6e 204a 696e 6120 4149   apps on Jina AI
-00000080: 2043 6c6f 7564 2e0a 486f 6d65 2d70 6167   Cloud..Home-pag
-00000090: 653a 2068 7474 7073 3a2f 2f67 6974 6875  e: https://githu
-000000a0: 622e 636f 6d2f 6a69 6e61 2d61 692f 6c61  b.com/jina-ai/la
-000000b0: 6e67 6368 6169 6e2d 7365 7276 652f 0a41  ngchain-serve/.A
-000000c0: 7574 686f 723a 204a 696e 6120 4149 0a41  uthor: Jina AI.A
-000000d0: 7574 686f 722d 656d 6169 6c3a 2068 656c  uthor-email: hel
-000000e0: 6c6f 406a 696e 612e 6169 0a4c 6963 656e  lo@jina.ai.Licen
-000000f0: 7365 3a20 4170 6163 6865 2032 2e30 0a44  se: Apache 2.0.D
-00000100: 6f77 6e6c 6f61 642d 5552 4c3a 2068 7474  ownload-URL: htt
-00000110: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000120: 6a69 6e61 2d61 692f 6c61 6e67 6368 6169  jina-ai/langchai
-00000130: 6e2d 7365 7276 652f 7461 6773 0a50 726f  n-serve/tags.Pro
-00000140: 6a65 6374 2d55 524c 3a20 446f 6375 6d65  ject-URL: Docume
-00000150: 6e74 6174 696f 6e2c 2068 7474 7073 3a2f  ntation, https:/
-00000160: 2f64 6f63 732e 6a69 6e61 2e61 690a 5072  /docs.jina.ai.Pr
-00000170: 6f6a 6563 742d 5552 4c3a 2053 6f75 7263  oject-URL: Sourc
-00000180: 652c 2068 7474 7073 3a2f 2f67 6974 6875  e, https://githu
-00000190: 622e 636f 6d2f 6a69 6e61 2d61 692f 6e6f  b.com/jina-ai/no
-000001a0: 770a 5072 6f6a 6563 742d 5552 4c3a 2054  w.Project-URL: T
-000001b0: 7261 636b 6572 2c20 6874 7470 733a 2f2f  racker, https://
-000001c0: 6769 7468 7562 2e63 6f6d 2f6a 696e 612d  github.com/jina-
-000001d0: 6169 2f6e 6f77 2f69 7373 7565 730a 4b65  ai/now/issues.Ke
-000001e0: 7977 6f72 6473 3a20 6a69 6e61 206c 616e  ywords: jina lan
-000001f0: 6763 6861 696e 206c 6c6d 206e 6575 7261  gchain llm neura
-00000200: 6c2d 6e65 7477 6f72 6b20 6465 6570 2d6c  l-network deep-l
-00000210: 6561 726e 696e 6720 6461 7461 2064 656d  earning data dem
-00000220: 6f63 7261 7469 7a61 7469 6f6e 0a50 6c61  ocratization.Pla
-00000230: 7466 6f72 6d3a 2055 4e4b 4e4f 574e 0a43  tform: UNKNOWN.C
-00000240: 6c61 7373 6966 6965 723a 2044 6576 656c  lassifier: Devel
-00000250: 6f70 6d65 6e74 2053 7461 7475 7320 3a3a  opment Status ::
-00000260: 2035 202d 2050 726f 6475 6374 696f 6e2f   5 - Production/
-00000270: 5374 6162 6c65 0a43 6c61 7373 6966 6965  Stable.Classifie
-00000280: 723a 2049 6e74 656e 6465 6420 4175 6469  r: Intended Audi
-00000290: 656e 6365 203a 3a20 4465 7665 6c6f 7065  ence :: Develope
-000002a0: 7273 0a43 6c61 7373 6966 6965 723a 2049  rs.Classifier: I
-000002b0: 6e74 656e 6465 6420 4175 6469 656e 6365  ntended Audience
-000002c0: 203a 3a20 4564 7563 6174 696f 6e0a 436c   :: Education.Cl
-000002d0: 6173 7369 6669 6572 3a20 496e 7465 6e64  assifier: Intend
-000002e0: 6564 2041 7564 6965 6e63 6520 3a3a 2053  ed Audience :: S
-000002f0: 6369 656e 6365 2f52 6573 6561 7263 680a  cience/Research.
-00000300: 436c 6173 7369 6669 6572 3a20 5072 6f67  Classifier: Prog
-00000310: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
-00000320: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
-00000330: 370a 436c 6173 7369 6669 6572 3a20 5072  7.Classifier: Pr
-00000340: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-00000350: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-00000360: 332e 380a 436c 6173 7369 6669 6572 3a20  3.8.Classifier: 
-00000370: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-00000380: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-00000390: 3a20 332e 390a 436c 6173 7369 6669 6572  : 3.9.Classifier
-000003a0: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
-000003b0: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-000003c0: 203a 3a20 332e 3130 0a43 6c61 7373 6966   :: 3.10.Classif
-000003d0: 6965 723a 2045 6e76 6972 6f6e 6d65 6e74  ier: Environment
-000003e0: 203a 3a20 436f 6e73 6f6c 650a 436c 6173   :: Console.Clas
-000003f0: 7369 6669 6572 3a20 4c69 6365 6e73 6520  sifier: License 
-00000400: 3a3a 204f 5349 2041 7070 726f 7665 6420  :: OSI Approved 
-00000410: 3a3a 2041 7061 6368 6520 536f 6674 7761  :: Apache Softwa
-00000420: 7265 204c 6963 656e 7365 0a43 6c61 7373  re License.Class
-00000430: 6966 6965 723a 204f 7065 7261 7469 6e67  ifier: Operating
-00000440: 2053 7973 7465 6d20 3a3a 204f 5320 496e   System :: OS In
-00000450: 6465 7065 6e64 656e 740a 436c 6173 7369  dependent.Classi
-00000460: 6669 6572 3a20 546f 7069 6320 3a3a 2053  fier: Topic :: S
-00000470: 6369 656e 7469 6669 632f 456e 6769 6e65  cientific/Engine
-00000480: 6572 696e 6720 3a3a 2041 7274 6966 6963  ering :: Artific
-00000490: 6961 6c20 496e 7465 6c6c 6967 656e 6365  ial Intelligence
-000004a0: 0a44 6573 6372 6970 7469 6f6e 2d43 6f6e  .Description-Con
-000004b0: 7465 6e74 2d54 7970 653a 2074 6578 742f  tent-Type: text/
-000004c0: 6d61 726b 646f 776e 0a4c 6963 656e 7365  markdown.License
-000004d0: 2d46 696c 653a 204c 4943 454e 5345 0a0a  -File: LICENSE..
-000004e0: 3c70 2061 6c69 676e 3d22 6365 6e74 6572  <p align="center
-000004f0: 223e 0a3c 623e 4c61 6e67 4368 6169 6e20  ">.<b>LangChain 
-00000500: 4170 7073 206f 6e20 5072 6f64 7563 7469  Apps on Producti
-00000510: 6f6e 2077 6974 6820 4a69 6e61 20f0 9f9a  on with Jina ...
-00000520: 803c 2f62 3e0a 3c2f 703e 0a0a 3c70 2061  .</b>.</p>..<p a
-00000530: 6c69 676e 3d63 656e 7465 723e 0a3c 6120  lign=center>.<a 
-00000540: 6872 6566 3d22 6874 7470 733a 2f2f 7079  href="https://py
-00000550: 7069 2e6f 7267 2f70 726f 6a65 6374 2f6c  pi.org/project/l
-00000560: 616e 6763 6861 696e 2d73 6572 7665 2f22  angchain-serve/"
-00000570: 3e3c 696d 6720 616c 743d 2250 7950 4922  ><img alt="PyPI"
-00000580: 2073 7263 3d22 6874 7470 733a 2f2f 696d   src="https://im
-00000590: 672e 7368 6965 6c64 732e 696f 2f70 7970  g.shields.io/pyp
-000005a0: 692f 762f 6c61 6e67 6368 6169 6e2d 7365  i/v/langchain-se
-000005b0: 7276 653f 6c61 6265 6c3d 5265 6c65 6173  rve?label=Releas
-000005c0: 6526 7374 796c 653d 666c 6174 2d73 7175  e&style=flat-squ
-000005d0: 6172 6522 3e3c 2f61 3e0a 3c61 2068 7265  are"></a>.<a hre
-000005e0: 663d 2268 7474 7073 3a2f 2f6a 696e 612e  f="https://jina.
-000005f0: 6169 2f73 6c61 636b 223e 3c69 6d67 2073  ai/slack"><img s
-00000600: 7263 3d22 6874 7470 733a 2f2f 696d 672e  rc="https://img.
-00000610: 7368 6965 6c64 732e 696f 2f62 6164 6765  shields.io/badge
-00000620: 2f53 6c61 636b 2d33 2e36 6b2d 626c 7565  /Slack-3.6k-blue
-00000630: 7669 6f6c 6574 3f6c 6f67 6f3d 736c 6163  violet?logo=slac
-00000640: 6b26 616d 703b 6c6f 676f 436f 6c6f 723d  k&amp;logoColor=
-00000650: 7768 6974 6526 7374 796c 653d 666c 6174  white&style=flat
-00000660: 2d73 7175 6172 6522 3e3c 2f61 3e0a 3c61  -square"></a>.<a
-00000670: 2068 7265 663d 2268 7474 7073 3a2f 2f70   href="https://p
-00000680: 7970 6973 7461 7473 2e6f 7267 2f70 6163  ypistats.org/pac
-00000690: 6b61 6765 732f 6c61 6e67 6368 6169 6e2d  kages/langchain-
-000006a0: 7365 7276 6522 3e3c 696d 6720 616c 743d  serve"><img alt=
-000006b0: 2250 7950 4920 2d20 446f 776e 6c6f 6164  "PyPI - Download
-000006c0: 7320 6672 6f6d 206f 6666 6963 6961 6c20  s from official 
-000006d0: 7079 7069 7374 6174 7322 2073 7263 3d22  pypistats" src="
-000006e0: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
-000006f0: 6c64 732e 696f 2f70 7970 692f 646d 2f6c  lds.io/pypi/dm/l
-00000700: 616e 6763 6861 696e 2d73 6572 7665 3f73  angchain-serve?s
-00000710: 7479 6c65 3d66 6c61 742d 7371 7561 7265  tyle=flat-square
-00000720: 223e 3c2f 613e 0a3c 6120 6872 6566 3d22  "></a>.<a href="
-00000730: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000740: 6f6d 2f6a 696e 612d 6169 2f6c 616e 6763  om/jina-ai/langc
-00000750: 6861 696e 2d73 6572 7665 2f61 6374 696f  hain-serve/actio
-00000760: 6e73 2f77 6f72 6b66 6c6f 7773 2f63 642e  ns/workflows/cd.
-00000770: 796d 6c22 3e3c 696d 6720 616c 743d 2247  yml"><img alt="G
-00000780: 6974 6875 6220 4344 2073 7461 7475 7322  ithub CD status"
-00000790: 2073 7263 3d22 6874 7470 733a 2f2f 6769   src="https://gi
-000007a0: 7468 7562 2e63 6f6d 2f6a 696e 612d 6169  thub.com/jina-ai
-000007b0: 2f6c 616e 6763 6861 696e 2d73 6572 7665  /langchain-serve
-000007c0: 2f61 6374 696f 6e73 2f77 6f72 6b66 6c6f  /actions/workflo
-000007d0: 7773 2f63 642e 796d 6c2f 6261 6467 652e  ws/cd.yml/badge.
-000007e0: 7376 6722 3e3c 2f61 3e0a 3c2f 703e 0a0a  svg"></a>.</p>..
-000007f0: 0a5b 4a69 6e61 5d28 6874 7470 733a 2f2f  .[Jina](https://
-00000800: 6769 7468 7562 2e63 6f6d 2f6a 696e 612d  github.com/jina-
-00000810: 6169 2f6a 696e 6129 2069 7320 616e 206f  ai/jina) is an o
-00000820: 7065 6e2d 736f 7572 6365 2066 7261 6d65  pen-source frame
-00000830: 776f 726b 2074 6f20 6275 696c 642c 2064  work to build, d
-00000840: 6570 6c6f 7920 2620 6d61 6e61 6765 206d  eploy & manage m
-00000850: 6163 6869 6e65 206c 6561 726e 696e 6720  achine learning 
-00000860: 6170 706c 6963 6174 696f 6e73 2061 7420  applications at 
-00000870: 7363 616c 652e 205b 4c61 6e67 4368 6169  scale. [LangChai
-00000880: 6e5d 2868 7474 7073 3a2f 2f70 7974 686f  n](https://pytho
-00000890: 6e2e 6c61 6e67 6368 6169 6e2e 636f 6d2f  n.langchain.com/
-000008a0: 656e 2f6c 6174 6573 742f 696e 6465 782e  en/latest/index.
-000008b0: 6874 6d6c 2920 6973 2061 6e6f 7468 6572  html) is another
-000008c0: 206f 7065 6e2d 736f 7572 6365 2066 7261   open-source fra
-000008d0: 6d65 776f 726b 2066 6f72 2062 7569 6c64  mework for build
-000008e0: 696e 6720 6170 706c 6963 6174 696f 6e73  ing applications
-000008f0: 2070 6f77 6572 6564 2062 7920 6c61 6e67   powered by lang
-00000900: 7561 6765 206d 6f64 656c 732e 200a 0a2a  uage models. ..*
-00000910: 2a6c 616e 6763 6861 696e 2d73 6572 7665  *langchain-serve
-00000920: 2a2a 2068 656c 7073 2079 6f75 2064 6570  ** helps you dep
-00000930: 6c6f 7920 796f 7572 204c 616e 6743 6861  loy your LangCha
-00000940: 696e 2061 7070 7320 6f6e 204a 696e 6120  in apps on Jina 
-00000950: 4149 2043 6c6f 7564 2069 6e20 6a75 7374  AI Cloud in just
-00000960: 2061 206d 6174 7465 7220 6f66 2073 6563   a matter of sec
-00000970: 6f6e 6473 2e20 596f 7520 6361 6e20 6e6f  onds. You can no
-00000980: 7720 6265 6e65 6669 7420 6672 6f6d 2074  w benefit from t
-00000990: 6865 2073 6361 6c61 6269 6c69 7479 2061  he scalability a
-000009a0: 6e64 2073 6572 7665 726c 6573 7320 6172  nd serverless ar
-000009b0: 6368 6974 6563 7475 7265 206f 6620 7468  chitecture of th
-000009c0: 6520 636c 6f75 6420 7769 7468 6f75 7420  e cloud without 
-000009d0: 7361 6372 6966 6963 696e 6720 7468 6520  sacrificing the 
-000009e0: 6561 7365 2061 6e64 2063 6f6e 7665 6e69  ease and conveni
-000009f0: 656e 6365 206f 6620 6c6f 6361 6c20 6465  ence of local de
-00000a00: 7665 6c6f 706d 656e 742e 0a0a 0a23 2320  velopment....## 
-00000a10: f09f a7a0 2042 6162 7961 6769 2d61 732d  .... Babyagi-as-
-00000a20: 612d 7365 7276 6963 650a 0a3e 2047 6976  a-service..> Giv
-00000a30: 6520 7573 2061 203a 7374 6172 3a20 616e  e us a :star: an
-00000a40: 6420 7465 6c6c 2075 7320 7768 6174 206d  d tell us what m
-00000a50: 6f72 6520 796f 7527 6420 6c69 6b65 2074  ore you'd like t
-00000a60: 6f20 7365 6521 200a 0a2d 2044 6570 6c6f  o see! ..- Deplo
-00000a70: 7920 6062 6162 7961 6769 6020 6f6e 204a  y `babyagi` on J
-00000a80: 696e 6120 4149 2043 6c6f 7564 2077 6974  ina AI Cloud wit
-00000a90: 6820 6f6e 6520 636f 6d6d 616e 640a 0a20  h one command.. 
-00000aa0: 2060 6060 6261 7368 0a20 206c 632d 7365   ```bash.  lc-se
-00000ab0: 7276 6520 6465 706c 6f79 2062 6162 7961  rve deploy babya
-00000ac0: 6769 0a20 2060 6060 0a0a 2d20 496e 7465  gi.  ```..- Inte
-00000ad0: 6772 6174 6520 6261 6279 6167 6920 7769  grate babyagi wi
-00000ae0: 7468 2065 7874 6572 6e61 6c20 7365 7276  th external serv
-00000af0: 6963 6573 2075 7369 6e67 206f 7572 2057  ices using our W
-00000b00: 6562 736f 636b 6574 2041 5049 2e20 4765  ebsocket API. Ge
-00000b10: 7420 6120 666c 6176 6f72 206f 6620 7468  t a flavor of th
-00000b20: 6520 696e 7465 6772 6174 696f 6e20 6f6e  e integration on
-00000b30: 2079 6f75 7220 434c 4920 7769 7468 200a   your CLI with .
-00000b40: 2020 2020 0a20 2060 6060 6261 7368 0a20      .  ```bash. 
-00000b50: 206c 632d 7365 7276 6520 706c 6179 6772   lc-serve playgr
-00000b60: 6f75 6e64 2062 6162 7961 6769 0a20 2060  ound babyagi.  `
-00000b70: 6060 0a0a 215b 4261 6279 6167 692d 6173  ``..![Babyagi-as
-00000b80: 2d61 2d73 6572 7669 6365 2050 6c61 7967  -a-service Playg
-00000b90: 726f 756e 645d 282e 6769 7468 7562 2f69  round](.github/i
-00000ba0: 6d61 6765 732f 6261 6279 6167 692d 706c  mages/babyagi-pl
-00000bb0: 6179 6772 6f75 6e64 2e67 6966 290a 0a0a  ayground.gif)...
-00000bc0: 2323 2323 20f0 9f8e 8920 4375 7374 6f6d  #### .... Custom
-00000bd0: 2041 7070 7320 746f 2070 726f 6475 6374   Apps to product
-00000be0: 696f 6e20 696e 2034 2073 696d 706c 6520  ion in 4 simple 
-00000bf0: 7374 6570 730a 0a20 2031 2e20 5265 6661  steps..  1. Refa
-00000c00: 6374 6f72 2079 6f75 7220 636f 6465 2074  ctor your code t
-00000c10: 6f20 6675 6e63 7469 6f6e 2873 2920 7468  o function(s) th
-00000c20: 6174 2073 686f 756c 6420 6265 2073 6572  at should be ser
-00000c30: 7665 6420 7769 7468 2060 4073 6572 7669  ved with `@servi
-00000c40: 6e67 6020 6465 636f 7261 746f 722e 0a20  ng` decorator.. 
-00000c50: 2031 2e20 4372 6561 7465 2061 2060 7265   1. Create a `re
-00000c60: 7175 6972 656d 656e 7473 2e74 7874 6020  quirements.txt` 
-00000c70: 6669 6c65 2069 6e20 796f 7572 2061 7070  file in your app
-00000c80: 2064 6972 6563 746f 7279 2074 6f20 656e   directory to en
-00000c90: 7375 7265 2061 6c6c 206e 6563 6573 7361  sure all necessa
-00000ca0: 7279 2064 6570 656e 6465 6e63 6965 7320  ry dependencies 
-00000cb0: 6172 6520 696e 7374 616c 6c65 642e 0a20  are installed.. 
-00000cc0: 2031 2e20 5275 6e20 606c 632d 7365 7276   1. Run `lc-serv
-00000cd0: 6520 6465 706c 6f79 206c 6f63 616c 2061  e deploy local a
-00000ce0: 7070 6020 746f 2074 6573 7420 796f 7572  pp` to test your
-00000cf0: 2041 5049 206c 6f63 616c 6c79 2e0a 2020   API locally..  
-00000d00: 312e 2052 756e 2060 6c63 2d73 6572 7665  1. Run `lc-serve
-00000d10: 2064 6570 6c6f 7920 6a63 6c6f 7564 2061   deploy jcloud a
-00000d20: 7070 6020 746f 2064 6570 6c6f 7920 6f6e  pp` to deploy on
-00000d30: 205b 4a69 6e61 2041 4920 436c 6f75 645d   [Jina AI Cloud]
-00000d40: 2868 7474 7073 3a2f 2f6a 696e 612e 6169  (https://jina.ai
-00000d50: 2f70 726f 6475 6374 2f63 6c6f 7564 2f29  /product/cloud/)
-00000d60: 2e0a 0a0a 2323 2323 20f0 9f94 a520 5363  ....#### .... Sc
-00000d70: 616c 6162 6c65 2c20 5365 7276 6572 6c65  alable, Serverle
-00000d80: 7373 2052 4553 5466 756c 2f53 7472 6561  ss RESTful/Strea
-00000d90: 6d69 6e67 2057 6562 736f 636b 6574 2041  ming Websocket A
-00000da0: 5049 7320 6f6e 204a 696e 6120 4149 2043  PIs on Jina AI C
-00000db0: 6c6f 7564 0a0a 2020 2d20 f09f 8c8e 2052  loud..  - .... R
-00000dc0: 4553 5466 756c 2f57 6562 736f 636b 6574  ESTful/Websocket
-00000dd0: 2041 5049 7320 7769 7468 2054 4c53 2063   APIs with TLS c
-00000de0: 6572 7473 2069 6e20 6a75 7374 2032 206c  erts in just 2 l
-00000df0: 696e 6573 206f 6620 636f 6465 2063 6861  ines of code cha
-00000e00: 6e67 652e 0a20 202d 20f0 9f8c 8a20 5374  nge..  - .... St
-00000e10: 7265 616d 204c 4c4d 2069 6e74 6572 6163  ream LLM interac
-00000e20: 7469 6f6e 7320 696e 2072 6561 6c2d 7469  tions in real-ti
-00000e30: 6d65 2077 6974 6820 5765 6273 6f63 6b65  me with Websocke
-00000e40: 7473 2e0a 2020 2d20 f09f 91a5 2045 6e61  ts..  - .... Ena
-00000e50: 626c 6520 6875 6d61 6e20 696e 2074 6865  ble human in the
-00000e60: 206c 6f6f 7020 666f 7220 796f 7572 2061   loop for your a
-00000e70: 6765 6e74 732e 0a20 202d 20f0 9f93 8420  gents..  - .... 
-00000e80: 5377 6167 6765 7220 5549 2c20 616e 6420  Swagger UI, and 
-00000e90: 4f70 656e 4150 4920 7370 6563 2069 6e63  OpenAPI spec inc
-00000ea0: 6c75 6465 6420 7769 7468 2079 6f75 7220  luded with your 
-00000eb0: 4150 4973 2e0a 2020 2d20 e29a a1ef b88f  APIs..  - ......
-00000ec0: 2053 6572 7665 726c 6573 7320 6170 7073   Serverless apps
-00000ed0: 2074 6861 7420 7363 616c 6573 2061 7574   that scales aut
-00000ee0: 6f6d 6174 6963 616c 6c79 2077 6974 6820  omatically with 
-00000ef0: 796f 7572 2074 7261 6666 6963 2e0a 2020  your traffic..  
-00000f00: 2d20 f09f 938a 2042 7569 6c74 696e 206c  - .... Builtin l
-00000f10: 6f67 6769 6e67 2c20 6d6f 6e69 746f 7269  ogging, monitori
-00000f20: 6e67 2c20 616e 6420 7472 6163 6573 2066  ng, and traces f
-00000f30: 6f72 2079 6f75 7220 4150 4973 2e0a 2020  or your APIs..  
-00000f40: 2d20 f09f a496 204e 6f20 6e65 6564 2074  - .... No need t
-00000f50: 6f20 6368 616e 6765 2079 6f75 7220 636f  o change your co
-00000f60: 6465 2074 6f20 6d61 6e61 6765 2041 5049  de to manage API
-00000f70: 732c 206f 7220 6d61 6e61 6765 2064 6f63  s, or manage doc
-00000f80: 6b65 7266 696c 6573 2c20 6f72 2077 6f72  kerfiles, or wor
-00000f90: 7279 2061 626f 7574 2069 6e66 7261 7374  ry about infrast
-00000fa0: 7275 6374 7572 6521 0a0a 0a23 2323 2320  ructure!...#### 
-00000fb0: f09f 9aa7 2043 6f6d 696e 6720 736f 6f6e  .... Coming soon
-00000fc0: 0a0a 2d20 5b20 5d20 f09f 9491 2041 7574  ..- [ ] .... Aut
-00000fd0: 686f 7269 7a65 2041 5049 2065 6e64 706f  horize API endpo
-00000fe0: 696e 7473 0a2d 205b 205d 20f0 9f9b a0ef  ints.- [ ] .....
-00000ff0: b88f 2045 6e61 626c 6520 5374 7265 616d  .. Enable Stream
-00001000: 6c69 7420 706c 6179 6772 6f75 6e64 2064  lit playground d
-00001010: 6570 6c6f 796d 656e 7420 666f 7220 796f  eployment for yo
-00001020: 7572 2061 7070 730a 0a0a 4966 2079 6f75  ur apps...If you
-00001030: 2068 6176 6520 616e 7920 6665 6174 7572   have any featur
-00001040: 6520 7265 7175 6573 7473 206f 7220 6661  e requests or fa
-00001050: 6365 6420 616e 7920 6973 7375 652c 2070  ced any issue, p
-00001060: 6c65 6173 6520 5b6c 6574 2075 7320 6b6e  lease [let us kn
-00001070: 6f77 5d28 6874 7470 733a 2f2f 6769 7468  ow](https://gith
-00001080: 7562 2e63 6f6d 2f6a 696e 612d 6169 2f6c  ub.com/jina-ai/l
-00001090: 616e 6763 6861 696e 2d73 6572 7665 2f69  angchain-serve/i
-000010a0: 7373 7565 732f 6e65 7729 210a 0a0a 2323  ssues/new)!...##
-000010b0: 2055 7361 6765 0a0a 4c65 7427 7320 6669   Usage..Let's fi
-000010c0: 7273 7420 696e 7374 616c 6c20 606c 616e  rst install `lan
-000010d0: 6763 6861 696e 2d73 6572 7665 6020 7573  gchain-serve` us
-000010e0: 696e 6720 7069 702e 0a0a 6060 6062 6173  ing pip...```bas
-000010f0: 680a 7069 7020 696e 7374 616c 6c20 6c61  h.pip install la
-00001100: 6e67 6368 6169 6e2d 7365 7276 650a 6060  ngchain-serve.``
-00001110: 600a 0a23 2320 456e 6162 6c65 2048 756d  `..## Enable Hum
-00001120: 616e 2d69 6e2d 7468 652d 6c6f 6f70 2028  an-in-the-loop (
-00001130: 4849 544c 2920 666f 7220 796f 7572 2061  HITL) for your a
-00001140: 6765 6e74 730a 0a48 4954 4c20 666f 7220  gents..HITL for 
-00001150: 4c61 6e67 4368 6169 6e20 6167 656e 7473  LangChain agents
-00001160: 206f 6e20 7072 6f64 7563 7469 6f6e 2063   on production c
-00001170: 616e 2062 6520 6368 616c 6c65 6e67 696e  an be challengin
-00001180: 6720 7369 6e63 6520 7468 6520 6167 656e  g since the agen
-00001190: 7473 2061 7265 2074 7970 6963 616c 6c79  ts are typically
-000011a0: 2072 756e 6e69 6e67 206f 6e20 7365 7276   running on serv
-000011b0: 6572 7320 7768 6572 6520 6875 6d61 6e73  ers where humans
-000011c0: 2064 6f6e 2774 2068 6176 6520 6469 7265   don't have dire
-000011d0: 6374 2061 6363 6573 732e 202a 2a6c 616e  ct access. **lan
-000011e0: 6763 6861 696e 2d73 6572 7665 2a2a 2062  gchain-serve** b
-000011f0: 7269 6467 6573 2074 6869 7320 6761 7020  ridges this gap 
-00001200: 6279 2065 6e61 626c 696e 6720 7765 6273  by enabling webs
-00001210: 6f63 6b65 7420 4150 4973 2074 6861 7420  ocket APIs that 
-00001220: 616c 6c6f 7720 666f 7220 7265 616c 2d74  allow for real-t
-00001230: 696d 6520 696e 7465 7261 6374 696f 6e20  ime interaction 
-00001240: 616e 6420 6665 6564 6261 636b 2062 6574  and feedback bet
-00001250: 7765 656e 2074 6865 2061 6765 6e74 2061  ween the agent a
-00001260: 6e64 2061 2068 756d 616e 206f 7065 7261  nd a human opera
-00001270: 746f 722e 0a0a 4368 6563 6b20 6f75 7420  tor...Check out 
-00001280: 7468 6973 205b 6578 616d 706c 655d 2865  this [example](e
-00001290: 7861 6d70 6c65 732f 7765 6273 6f63 6b65  xamples/websocke
-000012a0: 7473 2f68 6974 6c2f 5245 4144 4d45 2e6d  ts/hitl/README.m
-000012b0: 6429 2074 6f20 7365 6520 686f 7720 796f  d) to see how yo
-000012c0: 7520 6361 6e20 656e 6162 6c65 2048 4954  u can enable HIT
-000012d0: 4c20 666f 7220 796f 7572 2061 6765 6e74  L for your agent
-000012e0: 732e 0a0a 0a23 2320 456e 6162 6c65 2052  s....## Enable R
-000012f0: 4553 5420 4150 4973 200a 0a0a 4c65 7427  EST APIs ...Let'
-00001300: 7320 6275 696c 6420 6120 6375 7374 6f6d  s build a custom
-00001310: 2061 6765 6e74 2075 7369 6e67 2074 6869   agent using thi
-00001320: 7320 6578 616d 706c 6520 7461 6b65 6e20  s example taken 
-00001330: 6672 6f6d 205b 4c61 6e67 4368 6169 6e20  from [LangChain 
-00001340: 646f 6375 6d65 6e74 6174 696f 6e5d 2868  documentation](h
-00001350: 7474 7073 3a2f 2f70 7974 686f 6e2e 6c61  ttps://python.la
-00001360: 6e67 6368 6169 6e2e 636f 6d2f 656e 2f6c  ngchain.com/en/l
-00001370: 6174 6573 742f 6d6f 6475 6c65 732f 6167  atest/modules/ag
-00001380: 656e 7473 2f61 6765 6e74 732f 6375 7374  ents/agents/cust
-00001390: 6f6d 5f61 6765 6e74 2e68 746d 6c29 2e20  om_agent.html). 
-000013a0: 0a0a 0a3c 6465 7461 696c 733e 0a3c 7375  ...<details>.<su
-000013b0: 6d6d 6172 793e 5368 6f77 2061 6765 6e74  mmary>Show agent
-000013c0: 2063 6f64 6520 2861 7070 2e70 7929 3c2f   code (app.py)</
-000013d0: 7375 6d6d 6172 793e 0a0a 6060 6070 7974  summary>..```pyt
-000013e0: 686f 6e0a 2320 6170 702e 7079 0a66 726f  hon.# app.py.fro
-000013f0: 6d20 6c61 6e67 6368 6169 6e2e 6167 656e  m langchain.agen
-00001400: 7473 2069 6d70 6f72 7420 5a65 726f 5368  ts import ZeroSh
-00001410: 6f74 4167 656e 742c 2054 6f6f 6c2c 2041  otAgent, Tool, A
-00001420: 6765 6e74 4578 6563 7574 6f72 0a66 726f  gentExecutor.fro
-00001430: 6d20 6c61 6e67 6368 6169 6e20 696d 706f  m langchain impo
-00001440: 7274 204f 7065 6e41 492c 2053 6572 7041  rt OpenAI, SerpA
-00001450: 5049 5772 6170 7065 722c 204c 4c4d 4368  PIWrapper, LLMCh
-00001460: 6169 6e0a 0a73 6561 7263 6820 3d20 5365  ain..search = Se
-00001470: 7270 4150 4957 7261 7070 6572 2829 0a74  rpAPIWrapper().t
-00001480: 6f6f 6c73 203d 205b 0a20 2020 2054 6f6f  ools = [.    Too
-00001490: 6c28 0a20 2020 2020 2020 206e 616d 6520  l(.        name 
-000014a0: 3d20 2253 6561 7263 6822 2c0a 2020 2020  = "Search",.    
-000014b0: 2020 2020 6675 6e63 3d73 6561 7263 682e      func=search.
-000014c0: 7275 6e2c 0a20 2020 2020 2020 2064 6573  run,.        des
-000014d0: 6372 6970 7469 6f6e 3d22 7573 6566 756c  cription="useful
-000014e0: 2066 6f72 2077 6865 6e20 796f 7520 6e65   for when you ne
-000014f0: 6564 2074 6f20 616e 7377 6572 2071 7565  ed to answer que
-00001500: 7374 696f 6e73 2061 626f 7574 2063 7572  stions about cur
-00001510: 7265 6e74 2065 7665 6e74 7322 0a20 2020  rent events".   
-00001520: 2029 0a5d 0a0a 7072 6566 6978 203d 2022   ).]..prefix = "
-00001530: 2222 416e 7377 6572 2074 6865 2066 6f6c  ""Answer the fol
-00001540: 6c6f 7769 6e67 2071 7565 7374 696f 6e73  lowing questions
-00001550: 2061 7320 6265 7374 2079 6f75 2063 616e   as best you can
-00001560: 2c20 6275 7420 7370 6561 6b69 6e67 2061  , but speaking a
-00001570: 7320 6120 7069 7261 7465 206d 6967 6874  s a pirate might
-00001580: 2073 7065 616b 2e20 596f 7520 6861 7665   speak. You have
-00001590: 2061 6363 6573 7320 746f 2074 6865 2066   access to the f
-000015a0: 6f6c 6c6f 7769 6e67 2074 6f6f 6c73 3a22  ollowing tools:"
-000015b0: 2222 0a73 7566 6669 7820 3d20 2222 2242  "".suffix = """B
-000015c0: 6567 696e 2120 5265 6d65 6d62 6572 2074  egin! Remember t
-000015d0: 6f20 7370 6561 6b20 6173 2061 2070 6972  o speak as a pir
-000015e0: 6174 6520 7768 656e 2067 6976 696e 6720  ate when giving 
-000015f0: 796f 7572 2066 696e 616c 2061 6e73 7765  your final answe
-00001600: 722e 2055 7365 206c 6f74 7320 6f66 2022  r. Use lots of "
-00001610: 4172 6773 220a 0a51 7565 7374 696f 6e3a  Args"..Question:
-00001620: 207b 696e 7075 747d 0a7b 6167 656e 745f   {input}.{agent_
-00001630: 7363 7261 7463 6870 6164 7d22 2222 0a0a  scratchpad}"""..
-00001640: 7072 6f6d 7074 203d 205a 6572 6f53 686f  prompt = ZeroSho
-00001650: 7441 6765 6e74 2e63 7265 6174 655f 7072  tAgent.create_pr
-00001660: 6f6d 7074 280a 2020 2020 746f 6f6c 732c  ompt(.    tools,
-00001670: 200a 2020 2020 7072 6566 6978 3d70 7265   .    prefix=pre
-00001680: 6669 782c 200a 2020 2020 7375 6666 6978  fix, .    suffix
-00001690: 3d73 7566 6669 782c 200a 2020 2020 696e  =suffix, .    in
-000016a0: 7075 745f 7661 7269 6162 6c65 733d 5b22  put_variables=["
-000016b0: 696e 7075 7422 2c20 2261 6765 6e74 5f73  input", "agent_s
-000016c0: 6372 6174 6368 7061 6422 5d0a 290a 0a6c  cratchpad"].)..l
-000016d0: 6c6d 5f63 6861 696e 203d 204c 4c4d 4368  lm_chain = LLMCh
-000016e0: 6169 6e28 6c6c 6d3d 4f70 656e 4149 2874  ain(llm=OpenAI(t
-000016f0: 656d 7065 7261 7475 7265 3d30 292c 2070  emperature=0), p
-00001700: 726f 6d70 743d 7072 6f6d 7074 290a 746f  rompt=prompt).to
-00001710: 6f6c 5f6e 616d 6573 203d 205b 746f 6f6c  ol_names = [tool
-00001720: 2e6e 616d 6520 666f 7220 746f 6f6c 2069  .name for tool i
-00001730: 6e20 746f 6f6c 735d 0a61 6765 6e74 203d  n tools].agent =
-00001740: 205a 6572 6f53 686f 7441 6765 6e74 286c   ZeroShotAgent(l
-00001750: 6c6d 5f63 6861 696e 3d6c 6c6d 5f63 6861  lm_chain=llm_cha
-00001760: 696e 2c20 616c 6c6f 7765 645f 746f 6f6c  in, allowed_tool
-00001770: 733d 746f 6f6c 5f6e 616d 6573 290a 6167  s=tool_names).ag
-00001780: 656e 745f 6578 6563 7574 6f72 203d 2041  ent_executor = A
-00001790: 6765 6e74 4578 6563 7574 6f72 2e66 726f  gentExecutor.fro
-000017a0: 6d5f 6167 656e 745f 616e 645f 746f 6f6c  m_agent_and_tool
-000017b0: 7328 6167 656e 743d 6167 656e 742c 2074  s(agent=agent, t
-000017c0: 6f6f 6c73 3d74 6f6f 6c73 2c20 7665 7262  ools=tools, verb
-000017d0: 6f73 653d 5472 7565 290a 6167 656e 745f  ose=True).agent_
-000017e0: 6578 6563 7574 6f72 2e72 756e 2822 486f  executor.run("Ho
-000017f0: 7720 6d61 6e79 2070 656f 706c 6520 6c69  w many people li
-00001800: 7665 2069 6e20 6361 6e61 6461 2061 7320  ve in canada as 
-00001810: 6f66 2032 3032 333f 2229 0a60 6060 0a0a  of 2023?").```..
-00001820: 2323 2323 204f 7574 7075 740a 0a0a 6060  #### Output...``
-00001830: 6074 6578 740a 3e20 456e 7465 7269 6e67  `text.> Entering
-00001840: 206e 6577 2041 6765 6e74 4578 6563 7574   new AgentExecut
-00001850: 6f72 2063 6861 696e 2e2e 2e0a 5468 6f75  or chain....Thou
-00001860: 6768 743a 2049 206e 6565 6420 746f 2066  ght: I need to f
-00001870: 696e 6420 6f75 7420 7468 6520 706f 7075  ind out the popu
-00001880: 6c61 7469 6f6e 206f 6620 4361 6e61 6461  lation of Canada
-00001890: 0a41 6374 696f 6e3a 2053 6561 7263 680a  .Action: Search.
-000018a0: 4163 7469 6f6e 2049 6e70 7574 3a20 506f  Action Input: Po
-000018b0: 7075 6c61 7469 6f6e 206f 6620 4361 6e61  pulation of Cana
-000018c0: 6461 2032 3032 330a 4f62 7365 7276 6174  da 2023.Observat
-000018d0: 696f 6e3a 2054 6865 2063 7572 7265 6e74  ion: The current
-000018e0: 2070 6f70 756c 6174 696f 6e20 6f66 2043   population of C
-000018f0: 616e 6164 6120 6973 2033 382c 3631 302c  anada is 38,610,
-00001900: 3434 3720 6173 206f 6620 5361 7475 7264  447 as of Saturd
-00001910: 6179 2c20 4665 6272 7561 7279 2031 382c  ay, February 18,
-00001920: 2032 3032 332c 2062 6173 6564 206f 6e20   2023, based on 
-00001930: 576f 726c 646f 6d65 7465 7220 656c 6162  Worldometer elab
-00001940: 6f72 6174 696f 6e20 6f66 2074 6865 206c  oration of the l
-00001950: 6174 6573 7420 556e 6974 6564 204e 6174  atest United Nat
-00001960: 696f 6e73 2064 6174 612e 2043 616e 6164  ions data. Canad
-00001970: 6120 3230 3230 2070 6f70 756c 6174 696f  a 2020 populatio
-00001980: 6e20 6973 2065 7374 696d 6174 6564 2061  n is estimated a
-00001990: 7420 3337 2c37 3432 2c31 3534 2070 656f  t 37,742,154 peo
-000019a0: 706c 6520 6174 206d 6964 2079 6561 7220  ple at mid year 
-000019b0: 6163 636f 7264 696e 6720 746f 2055 4e20  according to UN 
-000019c0: 6461 7461 2e0a 5468 6f75 6768 743a 2049  data..Thought: I
-000019d0: 206e 6f77 206b 6e6f 7720 7468 6520 6669   now know the fi
-000019e0: 6e61 6c20 616e 7377 6572 0a46 696e 616c  nal answer.Final
-000019f0: 2041 6e73 7765 723a 2041 7272 722c 2043   Answer: Arrr, C
-00001a00: 616e 6164 6120 6265 2068 6176 696e 2720  anada be havin' 
-00001a10: 3338 2c36 3130 2c34 3437 2073 6361 6c6c  38,610,447 scall
-00001a20: 7977 6167 7320 6c69 7669 6e27 2074 6865  ywags livin' the
-00001a30: 7265 2061 7320 6f66 2032 3032 3321 0a0a  re as of 2023!..
-00001a40: 3e20 4669 6e69 7368 6564 2063 6861 696e  > Finished chain
-00001a50: 2e0a 6060 600a 0a3c 2f64 6574 6169 6c73  ..```..</details
-00001a60: 3e0a 0a23 2323 2053 7465 7020 313a 200a  >..### Step 1: .
-00001a70: 0a2a 2a52 6566 6163 746f 7220 796f 7572  .**Refactor your
-00001a80: 2063 6f64 6520 746f 2066 756e 6374 696f   code to functio
-00001a90: 6e28 7329 2074 6861 7420 7368 6f75 6c64  n(s) that should
-00001aa0: 2062 6520 7365 7276 6564 2077 6974 6820   be served with 
-00001ab0: 6040 7365 7276 696e 6760 2064 6563 6f72  `@serving` decor
-00001ac0: 6174 6f72 2a2a 0a0a 0a3c 6465 7461 696c  ator**...<detail
-00001ad0: 733e 0a3c 7375 6d6d 6172 793e 5368 6f77  s>.<summary>Show
-00001ae0: 2075 7064 6174 6564 2061 6765 6e74 2063   updated agent c
-00001af0: 6f64 6520 2861 7070 2e70 7929 3c2f 7375  ode (app.py)</su
-00001b00: 6d6d 6172 793e 0a0a 6060 6070 7974 686f  mmary>..```pytho
-00001b10: 6e0a 2320 6170 702e 7079 0a66 726f 6d20  n.# app.py.from 
-00001b20: 6c61 6e67 6368 6169 6e20 696d 706f 7274  langchain import
-00001b30: 204c 4c4d 4368 6169 6e2c 204f 7065 6e41   LLMChain, OpenA
-00001b40: 492c 2053 6572 7041 5049 5772 6170 7065  I, SerpAPIWrappe
-00001b50: 720a 6672 6f6d 206c 616e 6763 6861 696e  r.from langchain
-00001b60: 2e61 6765 6e74 7320 696d 706f 7274 2041  .agents import A
-00001b70: 6765 6e74 4578 6563 7574 6f72 2c20 546f  gentExecutor, To
-00001b80: 6f6c 2c20 5a65 726f 5368 6f74 4167 656e  ol, ZeroShotAgen
-00001b90: 740a 0a66 726f 6d20 6c63 7365 7276 6520  t..from lcserve 
-00001ba0: 696d 706f 7274 2073 6572 7669 6e67 0a0a  import serving..
-00001bb0: 0a40 7365 7276 696e 670a 6465 6620 6173  .@serving.def as
-00001bc0: 6b28 696e 7075 743a 2073 7472 2920 2d3e  k(input: str) ->
-00001bd0: 2073 7472 3a0a 2020 2020 7365 6172 6368   str:.    search
-00001be0: 203d 2053 6572 7041 5049 5772 6170 7065   = SerpAPIWrappe
-00001bf0: 7228 290a 2020 2020 746f 6f6c 7320 3d20  r().    tools = 
-00001c00: 5b0a 2020 2020 2020 2020 546f 6f6c 280a  [.        Tool(.
-00001c10: 2020 2020 2020 2020 2020 2020 6e61 6d65              name
-00001c20: 3d22 5365 6172 6368 222c 0a20 2020 2020  ="Search",.     
-00001c30: 2020 2020 2020 2066 756e 633d 7365 6172         func=sear
-00001c40: 6368 2e72 756e 2c0a 2020 2020 2020 2020  ch.run,.        
-00001c50: 2020 2020 6465 7363 7269 7074 696f 6e3d      description=
-00001c60: 2275 7365 6675 6c20 666f 7220 7768 656e  "useful for when
-00001c70: 2079 6f75 206e 6565 6420 746f 2061 6e73   you need to ans
-00001c80: 7765 7220 7175 6573 7469 6f6e 7320 6162  wer questions ab
-00001c90: 6f75 7420 6375 7272 656e 7420 6576 656e  out current even
-00001ca0: 7473 222c 0a20 2020 2020 2020 2029 0a20  ts",.        ). 
-00001cb0: 2020 205d 0a20 2020 2070 7265 6669 7820     ].    prefix 
-00001cc0: 3d20 2222 2241 6e73 7765 7220 7468 6520  = """Answer the 
-00001cd0: 666f 6c6c 6f77 696e 6720 7175 6573 7469  following questi
-00001ce0: 6f6e 7320 6173 2062 6573 7420 796f 7520  ons as best you 
-00001cf0: 6361 6e2c 2062 7574 2073 7065 616b 696e  can, but speakin
-00001d00: 6720 6173 2061 2070 6972 6174 6520 6d69  g as a pirate mi
-00001d10: 6768 7420 7370 6561 6b2e 2059 6f75 2068  ght speak. You h
-00001d20: 6176 6520 6163 6365 7373 2074 6f20 7468  ave access to th
-00001d30: 6520 666f 6c6c 6f77 696e 6720 746f 6f6c  e following tool
-00001d40: 733a 2222 220a 2020 2020 7375 6666 6978  s:""".    suffix
-00001d50: 203d 2022 2222 4265 6769 6e21 2052 656d   = """Begin! Rem
-00001d60: 656d 6265 7220 746f 2073 7065 616b 2061  ember to speak a
-00001d70: 7320 6120 7069 7261 7465 2077 6865 6e20  s a pirate when 
-00001d80: 6769 7669 6e67 2079 6f75 7220 6669 6e61  giving your fina
-00001d90: 6c20 616e 7377 6572 2e20 5573 6520 6c6f  l answer. Use lo
-00001da0: 7473 206f 6620 2241 7267 7322 0a0a 2020  ts of "Args"..  
-00001db0: 2020 5175 6573 7469 6f6e 3a20 7b69 6e70    Question: {inp
-00001dc0: 7574 7d0a 2020 2020 7b61 6765 6e74 5f73  ut}.    {agent_s
-00001dd0: 6372 6174 6368 7061 647d 2222 220a 0a20  cratchpad}""".. 
-00001de0: 2020 2070 726f 6d70 7420 3d20 5a65 726f     prompt = Zero
-00001df0: 5368 6f74 4167 656e 742e 6372 6561 7465  ShotAgent.create
-00001e00: 5f70 726f 6d70 7428 0a20 2020 2020 2020  _prompt(.       
-00001e10: 2074 6f6f 6c73 2c0a 2020 2020 2020 2020   tools,.        
-00001e20: 7072 6566 6978 3d70 7265 6669 782c 0a20  prefix=prefix,. 
-00001e30: 2020 2020 2020 2073 7566 6669 783d 7375         suffix=su
-00001e40: 6666 6978 2c0a 2020 2020 2020 2020 696e  ffix,.        in
-00001e50: 7075 745f 7661 7269 6162 6c65 733d 5b22  put_variables=["
-00001e60: 696e 7075 7422 2c20 2261 6765 6e74 5f73  input", "agent_s
-00001e70: 6372 6174 6368 7061 6422 5d2c 0a20 2020  cratchpad"],.   
-00001e80: 2029 0a0a 2020 2020 7072 696e 7428 7072   )..    print(pr
-00001e90: 6f6d 7074 2e74 656d 706c 6174 6529 0a0a  ompt.template)..
-00001ea0: 2020 2020 6c6c 6d5f 6368 6169 6e20 3d20      llm_chain = 
-00001eb0: 4c4c 4d43 6861 696e 286c 6c6d 3d4f 7065  LLMChain(llm=Ope
-00001ec0: 6e41 4928 7465 6d70 6572 6174 7572 653d  nAI(temperature=
-00001ed0: 3029 2c20 7072 6f6d 7074 3d70 726f 6d70  0), prompt=promp
-00001ee0: 7429 0a20 2020 2074 6f6f 6c5f 6e61 6d65  t).    tool_name
-00001ef0: 7320 3d20 5b74 6f6f 6c2e 6e61 6d65 2066  s = [tool.name f
-00001f00: 6f72 2074 6f6f 6c20 696e 2074 6f6f 6c73  or tool in tools
-00001f10: 5d0a 2020 2020 6167 656e 7420 3d20 5a65  ].    agent = Ze
-00001f20: 726f 5368 6f74 4167 656e 7428 6c6c 6d5f  roShotAgent(llm_
-00001f30: 6368 6169 6e3d 6c6c 6d5f 6368 6169 6e2c  chain=llm_chain,
-00001f40: 2061 6c6c 6f77 6564 5f74 6f6f 6c73 3d74   allowed_tools=t
-00001f50: 6f6f 6c5f 6e61 6d65 7329 0a0a 2020 2020  ool_names)..    
-00001f60: 6167 656e 745f 6578 6563 7574 6f72 203d  agent_executor =
-00001f70: 2041 6765 6e74 4578 6563 7574 6f72 2e66   AgentExecutor.f
-00001f80: 726f 6d5f 6167 656e 745f 616e 645f 746f  rom_agent_and_to
-00001f90: 6f6c 7328 0a20 2020 2020 2020 2061 6765  ols(.        age
-00001fa0: 6e74 3d61 6765 6e74 2c20 746f 6f6c 733d  nt=agent, tools=
-00001fb0: 746f 6f6c 732c 2076 6572 626f 7365 3d54  tools, verbose=T
-00001fc0: 7275 650a 2020 2020 290a 0a20 2020 2072  rue.    )..    r
-00001fd0: 6574 7572 6e20 6167 656e 745f 6578 6563  eturn agent_exec
-00001fe0: 7574 6f72 2e72 756e 2869 6e70 7574 290a  utor.run(input).
-00001ff0: 0a69 6620 5f5f 6e61 6d65 5f5f 203d 3d20  .if __name__ == 
-00002000: 225f 5f6d 6169 6e5f 5f22 3a0a 2020 2020  "__main__":.    
-00002010: 6173 6b28 2748 6f77 206d 616e 7920 7065  ask('How many pe
-00002020: 6f70 6c65 206c 6976 6520 696e 2063 616e  ople live in can
-00002030: 6164 6120 6173 206f 6620 3230 3233 3f27  ada as of 2023?'
-00002040: 290a 6060 600a 0a3c 2f64 6574 6169 6c73  ).```..</details
-00002050: 3e0a 0a0a 2323 2323 2320 5768 6174 2063  >...##### What c
-00002060: 6861 6e67 6564 3f0a 0a2d 2057 6520 6d6f  hanged?..- We mo
-00002070: 7665 6420 6f75 7220 636f 6465 2074 6f20  ved our code to 
-00002080: 616e 2060 6173 6b60 2066 756e 6374 696f  an `ask` functio
-00002090: 6e2e 0a2d 2041 6464 6564 2074 7970 6520  n..- Added type 
-000020a0: 6869 6e74 7320 746f 2074 6865 2066 756e  hints to the fun
-000020b0: 6374 696f 6e20 7061 7261 6d65 7465 7273  ction parameters
-000020c0: 2028 696e 7075 7420 616e 6420 6f75 7470   (input and outp
-000020d0: 7574 292c 2073 6f20 4150 4920 6465 6669  ut), so API defi
-000020e0: 6e69 7469 6f6e 2063 616e 2062 6520 6765  nition can be ge
-000020f0: 6e65 7261 7465 642e 0a2d 2049 6d70 6f72  nerated..- Impor
-00002100: 7465 6420 6066 726f 6d20 6c63 7365 7276  ted `from lcserv
-00002110: 6520 696d 706f 7274 2073 6572 7669 6e67  e import serving
-00002120: 6020 616e 6420 6164 6465 6420 6040 7365  ` and added `@se
-00002130: 7276 696e 6760 2064 6563 6f72 6174 6f72  rving` decorator
-00002140: 2074 6f20 7468 6520 6061 736b 6020 6675   to the `ask` fu
-00002150: 6e63 7469 6f6e 2e0a 2d20 4164 6465 6420  nction..- Added 
-00002160: 6069 6620 5f5f 6e61 6d65 5f5f 203d 3d20  `if __name__ == 
-00002170: 225f 5f6d 6169 6e5f 5f22 3a60 2062 6c6f  "__main__":` blo
-00002180: 636b 2074 6f20 7465 7374 2074 6865 2066  ck to test the f
-00002190: 756e 6374 696f 6e20 6c6f 6361 6c6c 792e  unction locally.
-000021a0: 0a0a 2d2d 2d0a 0a23 2323 2053 7465 7020  ..---..### Step 
-000021b0: 323a 0a0a 2a2a 4372 6561 7465 2061 2060  2:..**Create a `
-000021c0: 7265 7175 6972 656d 656e 7473 2e74 7874  requirements.txt
-000021d0: 6020 6669 6c65 2069 6e20 796f 7572 2061  ` file in your a
-000021e0: 7070 2064 6972 6563 746f 7279 2074 6f20  pp directory to 
-000021f0: 656e 7375 7265 2061 6c6c 206e 6563 6573  ensure all neces
-00002200: 7361 7279 2064 6570 656e 6465 6e63 6965  sary dependencie
-00002210: 7320 6172 6520 696e 7374 616c 6c65 642e  s are installed.
-00002220: 2a2a 0a0a 3c64 6574 6169 6c73 3e0a 3c73  **..<details>.<s
-00002230: 756d 6d61 7279 3e53 686f 7720 7265 7175  ummary>Show requ
-00002240: 6972 656d 656e 7473 2e74 7874 3c2f 7375  irements.txt</su
-00002250: 6d6d 6172 793e 0a0a 6060 6074 6578 740a  mmary>..```text.
-00002260: 2320 7265 7175 6972 656d 656e 7473 2e74  # requirements.t
-00002270: 7874 0a6f 7065 6e61 690a 676f 6f67 6c65  xt.openai.google
-00002280: 2d73 6561 7263 682d 7265 7375 6c74 730a  -search-results.
-00002290: 6060 600a 3c2f 6465 7461 696c 733e 0a0a  ```.</details>..
-000022a0: 2d2d 2d20 0a0a 2323 2320 5374 6570 2033  --- ..### Step 3
-000022b0: 3a0a 0a2a 2a52 756e 2060 6c63 2d73 6572  :..**Run `lc-ser
-000022c0: 7665 2064 6570 6c6f 7920 6c6f 6361 6c20  ve deploy local 
-000022d0: 6170 7060 2074 6f20 7465 7374 2079 6f75  app` to test you
-000022e0: 7220 4150 4920 6c6f 6361 6c6c 792e 2a2a  r API locally.**
-000022f0: 0a0a 3e20 6061 7070 6020 6973 2074 6865  ..> `app` is the
-00002300: 206e 616d 6520 6f66 2074 6865 206d 6f64   name of the mod
-00002310: 756c 6520 7468 6174 2063 6f6e 7461 696e  ule that contain
-00002320: 7320 7468 6520 6061 736b 6020 6675 6e63  s the `ask` func
-00002330: 7469 6f6e 2e0a 0a60 6060 6261 7368 0a6c  tion...```bash.l
-00002340: 632d 7365 7276 6520 6465 706c 6f79 206c  c-serve deploy l
-00002350: 6f63 616c 2061 7070 0a60 6060 0a0a 3c64  ocal app.```..<d
-00002360: 6574 6169 6c73 3e0a 3c73 756d 6d61 7279  etails>.<summary
-00002370: 3e53 686f 7720 6f75 7470 7574 3c2f 7375  >Show output</su
-00002380: 6d6d 6172 793e 0a0a 6060 6074 6578 740a  mmary>..```text.
+00000030: 696f 6e3a 2030 2e30 2e39 2e64 6576 390a  ion: 0.0.9.dev9.
+00000040: 5375 6d6d 6172 793a 204c 616e 6763 6861  Summary: Langcha
+00000050: 696e 2053 6572 7665 202d 2073 6572 7665  in Serve - serve
+00000060: 2079 6f75 7220 6c61 6e67 6368 6169 6e20   your langchain 
+00000070: 6170 7073 206f 6e20 4a69 6e61 2041 4920  apps on Jina AI 
+00000080: 436c 6f75 642e 0a48 6f6d 652d 7061 6765  Cloud..Home-page
+00000090: 3a20 6874 7470 733a 2f2f 6769 7468 7562  : https://github
+000000a0: 2e63 6f6d 2f6a 696e 612d 6169 2f6c 616e  .com/jina-ai/lan
+000000b0: 6763 6861 696e 2d73 6572 7665 2f0a 4175  gchain-serve/.Au
+000000c0: 7468 6f72 3a20 4a69 6e61 2041 490a 4175  thor: Jina AI.Au
+000000d0: 7468 6f72 2d65 6d61 696c 3a20 6865 6c6c  thor-email: hell
+000000e0: 6f40 6a69 6e61 2e61 690a 4c69 6365 6e73  o@jina.ai.Licens
+000000f0: 653a 2041 7061 6368 6520 322e 300a 446f  e: Apache 2.0.Do
+00000100: 776e 6c6f 6164 2d55 524c 3a20 6874 7470  wnload-URL: http
+00000110: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6a  s://github.com/j
+00000120: 696e 612d 6169 2f6c 616e 6763 6861 696e  ina-ai/langchain
+00000130: 2d73 6572 7665 2f74 6167 730a 5072 6f6a  -serve/tags.Proj
+00000140: 6563 742d 5552 4c3a 2044 6f63 756d 656e  ect-URL: Documen
+00000150: 7461 7469 6f6e 2c20 6874 7470 733a 2f2f  tation, https://
+00000160: 646f 6373 2e6a 696e 612e 6169 0a50 726f  docs.jina.ai.Pro
+00000170: 6a65 6374 2d55 524c 3a20 536f 7572 6365  ject-URL: Source
+00000180: 2c20 6874 7470 733a 2f2f 6769 7468 7562  , https://github
+00000190: 2e63 6f6d 2f6a 696e 612d 6169 2f6e 6f77  .com/jina-ai/now
+000001a0: 0a50 726f 6a65 6374 2d55 524c 3a20 5472  .Project-URL: Tr
+000001b0: 6163 6b65 722c 2068 7474 7073 3a2f 2f67  acker, https://g
+000001c0: 6974 6875 622e 636f 6d2f 6a69 6e61 2d61  ithub.com/jina-a
+000001d0: 692f 6e6f 772f 6973 7375 6573 0a4b 6579  i/now/issues.Key
+000001e0: 776f 7264 733a 206a 696e 6120 6c61 6e67  words: jina lang
+000001f0: 6368 6169 6e20 6c6c 6d20 6e65 7572 616c  chain llm neural
+00000200: 2d6e 6574 776f 726b 2064 6565 702d 6c65  -network deep-le
+00000210: 6172 6e69 6e67 2064 6174 6120 6465 6d6f  arning data demo
+00000220: 6372 6174 697a 6174 696f 6e0a 506c 6174  cratization.Plat
+00000230: 666f 726d 3a20 554e 4b4e 4f57 4e0a 436c  form: UNKNOWN.Cl
+00000240: 6173 7369 6669 6572 3a20 4465 7665 6c6f  assifier: Develo
+00000250: 706d 656e 7420 5374 6174 7573 203a 3a20  pment Status :: 
+00000260: 3520 2d20 5072 6f64 7563 7469 6f6e 2f53  5 - Production/S
+00000270: 7461 626c 650a 436c 6173 7369 6669 6572  table.Classifier
+00000280: 3a20 496e 7465 6e64 6564 2041 7564 6965  : Intended Audie
+00000290: 6e63 6520 3a3a 2044 6576 656c 6f70 6572  nce :: Developer
+000002a0: 730a 436c 6173 7369 6669 6572 3a20 496e  s.Classifier: In
+000002b0: 7465 6e64 6564 2041 7564 6965 6e63 6520  tended Audience 
+000002c0: 3a3a 2045 6475 6361 7469 6f6e 0a43 6c61  :: Education.Cla
+000002d0: 7373 6966 6965 723a 2049 6e74 656e 6465  ssifier: Intende
+000002e0: 6420 4175 6469 656e 6365 203a 3a20 5363  d Audience :: Sc
+000002f0: 6965 6e63 652f 5265 7365 6172 6368 0a43  ience/Research.C
+00000300: 6c61 7373 6966 6965 723a 2050 726f 6772  lassifier: Progr
+00000310: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+00000320: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e37  :: Python :: 3.7
+00000330: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
+00000340: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+00000350: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
+00000360: 2e38 0a43 6c61 7373 6966 6965 723a 2050  .8.Classifier: P
+00000370: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+00000380: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+00000390: 2033 2e39 0a43 6c61 7373 6966 6965 723a   3.9.Classifier:
+000003a0: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
+000003b0: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
+000003c0: 3a3a 2033 2e31 300a 436c 6173 7369 6669  :: 3.10.Classifi
+000003d0: 6572 3a20 456e 7669 726f 6e6d 656e 7420  er: Environment 
+000003e0: 3a3a 2043 6f6e 736f 6c65 0a43 6c61 7373  :: Console.Class
+000003f0: 6966 6965 723a 204c 6963 656e 7365 203a  ifier: License :
+00000400: 3a20 4f53 4920 4170 7072 6f76 6564 203a  : OSI Approved :
+00000410: 3a20 4170 6163 6865 2053 6f66 7477 6172  : Apache Softwar
+00000420: 6520 4c69 6365 6e73 650a 436c 6173 7369  e License.Classi
+00000430: 6669 6572 3a20 4f70 6572 6174 696e 6720  fier: Operating 
+00000440: 5379 7374 656d 203a 3a20 4f53 2049 6e64  System :: OS Ind
+00000450: 6570 656e 6465 6e74 0a43 6c61 7373 6966  ependent.Classif
+00000460: 6965 723a 2054 6f70 6963 203a 3a20 5363  ier: Topic :: Sc
+00000470: 6965 6e74 6966 6963 2f45 6e67 696e 6565  ientific/Enginee
+00000480: 7269 6e67 203a 3a20 4172 7469 6669 6369  ring :: Artifici
+00000490: 616c 2049 6e74 656c 6c69 6765 6e63 650a  al Intelligence.
+000004a0: 4465 7363 7269 7074 696f 6e2d 436f 6e74  Description-Cont
+000004b0: 656e 742d 5479 7065 3a20 7465 7874 2f6d  ent-Type: text/m
+000004c0: 6172 6b64 6f77 6e0a 4c69 6365 6e73 652d  arkdown.License-
+000004d0: 4669 6c65 3a20 4c49 4345 4e53 450a 0a23  File: LICENSE..#
+000004e0: 204c 616e 6743 6861 696e 2041 7070 7320   LangChain Apps 
+000004f0: 6f6e 2050 726f 6475 6374 696f 6e20 7769  on Production wi
+00000500: 7468 204a 696e 6120 f09f 9a80 0a0a 5b4a  th Jina ......[J
+00000510: 696e 615d 2868 7474 7073 3a2f 2f67 6974  ina](https://git
+00000520: 6875 622e 636f 6d2f 6a69 6e61 2d61 692f  hub.com/jina-ai/
+00000530: 6a69 6e61 2920 6973 2061 6e20 6f70 656e  jina) is an open
+00000540: 2d73 6f75 7263 6520 6672 616d 6577 6f72  -source framewor
+00000550: 6b20 746f 2062 7569 6c64 2c20 6465 706c  k to build, depl
+00000560: 6f79 2026 206d 616e 6167 6520 6d61 6368  oy & manage mach
+00000570: 696e 6520 6c65 6172 6e69 6e67 2061 7070  ine learning app
+00000580: 6c69 6361 7469 6f6e 7320 6174 2073 6361  lications at sca
+00000590: 6c65 2e20 5b4c 616e 6743 6861 696e 5d28  le. [LangChain](
+000005a0: 6874 7470 733a 2f2f 7079 7468 6f6e 2e6c  https://python.l
+000005b0: 616e 6763 6861 696e 2e63 6f6d 2f65 6e2f  angchain.com/en/
+000005c0: 6c61 7465 7374 2f69 6e64 6578 2e68 746d  latest/index.htm
+000005d0: 6c29 2069 7320 616e 6f74 6865 7220 6f70  l) is another op
+000005e0: 656e 2d73 6f75 7263 6520 6672 616d 6577  en-source framew
+000005f0: 6f72 6b20 666f 7220 6275 696c 6469 6e67  ork for building
+00000600: 2061 7070 6c69 6361 7469 6f6e 7320 706f   applications po
+00000610: 7765 7265 6420 6279 206c 616e 6775 6167  wered by languag
+00000620: 6520 6d6f 6465 6c73 2e20 0a0a 2a2a 6c61  e models. ..**la
+00000630: 6e67 6368 6169 6e2d 7365 7276 652a 2a20  ngchain-serve** 
+00000640: 6865 6c70 7320 796f 7520 6465 706c 6f79  helps you deploy
+00000650: 2079 6f75 7220 4c61 6e67 4368 6169 6e20   your LangChain 
+00000660: 6170 7073 206f 6e20 4a69 6e61 2041 4920  apps on Jina AI 
+00000670: 436c 6f75 6420 696e 206a 7573 7420 6120  Cloud in just a 
+00000680: 6d61 7474 6572 206f 6620 7365 636f 6e64  matter of second
+00000690: 732e 2059 6f75 2063 616e 206e 6f77 2062  s. You can now b
+000006a0: 656e 6566 6974 2066 726f 6d20 7468 6520  enefit from the 
+000006b0: 7363 616c 6162 696c 6974 7920 616e 6420  scalability and 
+000006c0: 7365 7276 6572 6c65 7373 2061 7263 6869  serverless archi
+000006d0: 7465 6374 7572 6520 6f66 2074 6865 2063  tecture of the c
+000006e0: 6c6f 7564 2077 6974 686f 7574 2073 6163  loud without sac
+000006f0: 7269 6669 6369 6e67 2074 6865 2065 6173  rificing the eas
+00000700: 6520 616e 6420 636f 6e76 656e 6965 6e63  e and convenienc
+00000710: 6520 6f66 206c 6f63 616c 2064 6576 656c  e of local devel
+00000720: 6f70 6d65 6e74 2e0a 0a0a 2323 20f0 9fa7  opment....## ...
+00000730: a020 4261 6279 6167 692d 6173 2d61 2d73  . Babyagi-as-a-s
+00000740: 6572 7669 6365 0a0a 3e20 4769 7665 2075  ervice..> Give u
+00000750: 7320 6120 3a73 7461 723a 2061 6e64 2074  s a :star: and t
+00000760: 656c 6c20 7573 2077 6861 7420 6d6f 7265  ell us what more
+00000770: 2079 6f75 2764 206c 696b 6520 746f 2073   you'd like to s
+00000780: 6565 2120 0a0a 2d20 4465 706c 6f79 2060  ee! ..- Deploy `
+00000790: 6261 6279 6167 6960 206f 6e20 4a69 6e61  babyagi` on Jina
+000007a0: 2041 4920 436c 6f75 6420 7769 7468 206f   AI Cloud with o
+000007b0: 6e65 2063 6f6d 6d61 6e64 0a0a 2020 6060  ne command..  ``
+000007c0: 6062 6173 680a 2020 6c63 2d73 6572 7665  `bash.  lc-serve
+000007d0: 2064 6570 6c6f 7920 6261 6279 6167 690a   deploy babyagi.
+000007e0: 2020 6060 600a 0a2d 2049 6e74 6567 7261    ```..- Integra
+000007f0: 7465 2062 6162 7961 6769 2077 6974 6820  te babyagi with 
+00000800: 6578 7465 726e 616c 2073 6572 7669 6365  external service
+00000810: 7320 7573 696e 6720 6f75 7220 5765 6273  s using our Webs
+00000820: 6f63 6b65 7420 4150 492e 2047 6574 2061  ocket API. Get a
+00000830: 2066 6c61 766f 7220 6f66 2074 6865 2069   flavor of the i
+00000840: 6e74 6567 7261 7469 6f6e 206f 6e20 796f  ntegration on yo
+00000850: 7572 2043 4c49 2077 6974 6820 0a20 2020  ur CLI with .   
+00000860: 200a 2020 6060 6062 6173 680a 2020 6c63   .  ```bash.  lc
+00000870: 2d73 6572 7665 2070 6c61 7967 726f 756e  -serve playgroun
+00000880: 6420 6261 6279 6167 690a 2020 6060 600a  d babyagi.  ```.
+00000890: 0a21 5b42 6162 7961 6769 2d61 732d 612d  .![Babyagi-as-a-
+000008a0: 7365 7276 6963 6520 506c 6179 6772 6f75  service Playgrou
+000008b0: 6e64 5d28 2e67 6974 6875 622f 696d 6167  nd](.github/imag
+000008c0: 6573 2f62 6162 7961 6769 2d70 6c61 7967  es/babyagi-playg
+000008d0: 726f 756e 642e 6769 6629 0a0a 0a23 2323  round.gif)...###
+000008e0: 2320 f09f 8e89 2043 7573 746f 6d20 4170  # .... Custom Ap
+000008f0: 7073 2074 6f20 7072 6f64 7563 7469 6f6e  ps to production
+00000900: 2069 6e20 3420 7369 6d70 6c65 2073 7465   in 4 simple ste
+00000910: 7073 0a0a 2020 312e 2052 6566 6163 746f  ps..  1. Refacto
+00000920: 7220 796f 7572 2063 6f64 6520 746f 2066  r your code to f
+00000930: 756e 6374 696f 6e28 7329 2074 6861 7420  unction(s) that 
+00000940: 7368 6f75 6c64 2062 6520 7365 7276 6564  should be served
+00000950: 2077 6974 6820 6040 7365 7276 696e 6760   with `@serving`
+00000960: 2064 6563 6f72 6174 6f72 2e0a 2020 312e   decorator..  1.
+00000970: 2043 7265 6174 6520 6120 6072 6571 7569   Create a `requi
+00000980: 7265 6d65 6e74 732e 7478 7460 2066 696c  rements.txt` fil
+00000990: 6520 696e 2079 6f75 7220 6170 7020 6469  e in your app di
+000009a0: 7265 6374 6f72 7920 746f 2065 6e73 7572  rectory to ensur
+000009b0: 6520 616c 6c20 6e65 6365 7373 6172 7920  e all necessary 
+000009c0: 6465 7065 6e64 656e 6369 6573 2061 7265  dependencies are
+000009d0: 2069 6e73 7461 6c6c 6564 2e0a 2020 312e   installed..  1.
+000009e0: 2052 756e 2060 6c63 2d73 6572 7665 2064   Run `lc-serve d
+000009f0: 6570 6c6f 7920 6c6f 6361 6c20 6170 7060  eploy local app`
+00000a00: 2074 6f20 7465 7374 2079 6f75 7220 4150   to test your AP
+00000a10: 4920 6c6f 6361 6c6c 792e 0a20 2031 2e20  I locally..  1. 
+00000a20: 5275 6e20 606c 632d 7365 7276 6520 6465  Run `lc-serve de
+00000a30: 706c 6f79 206a 636c 6f75 6420 6170 7060  ploy jcloud app`
+00000a40: 2074 6f20 6465 706c 6f79 206f 6e20 5b4a   to deploy on [J
+00000a50: 696e 6120 4149 2043 6c6f 7564 5d28 6874  ina AI Cloud](ht
+00000a60: 7470 733a 2f2f 6a69 6e61 2e61 692f 7072  tps://jina.ai/pr
+00000a70: 6f64 7563 742f 636c 6f75 642f 292e 0a0a  oduct/cloud/)...
+00000a80: 0a23 2323 2320 f09f 94a5 2053 6361 6c61  .#### .... Scala
+00000a90: 626c 652c 2053 6572 7665 726c 6573 7320  ble, Serverless 
+00000aa0: 5245 5354 6675 6c2f 5374 7265 616d 696e  RESTful/Streamin
+00000ab0: 6720 5765 6273 6f63 6b65 7420 4150 4973  g Websocket APIs
+00000ac0: 206f 6e20 4a69 6e61 2041 4920 436c 6f75   on Jina AI Clou
+00000ad0: 640a 0a20 202d 20f0 9f8c 8e20 5245 5354  d..  - .... REST
+00000ae0: 6675 6c2f 5765 6273 6f63 6b65 7420 4150  ful/Websocket AP
+00000af0: 4973 2077 6974 6820 544c 5320 6365 7274  Is with TLS cert
+00000b00: 7320 696e 206a 7573 7420 3220 6c69 6e65  s in just 2 line
+00000b10: 7320 6f66 2063 6f64 6520 6368 616e 6765  s of code change
+00000b20: 2e0a 2020 2d20 f09f 8c8a 2053 7472 6561  ..  - .... Strea
+00000b30: 6d20 4c4c 4d20 696e 7465 7261 6374 696f  m LLM interactio
+00000b40: 6e73 2069 6e20 7265 616c 2d74 696d 6520  ns in real-time 
+00000b50: 7769 7468 2057 6562 736f 636b 6574 732e  with Websockets.
+00000b60: 0a20 202d 20f0 9f91 a520 456e 6162 6c65  .  - .... Enable
+00000b70: 2068 756d 616e 2069 6e20 7468 6520 6c6f   human in the lo
+00000b80: 6f70 2066 6f72 2079 6f75 7220 6167 656e  op for your agen
+00000b90: 7473 2e0a 2020 2d20 f09f 9384 2053 7761  ts..  - .... Swa
+00000ba0: 6767 6572 2055 492c 2061 6e64 204f 7065  gger UI, and Ope
+00000bb0: 6e41 5049 2073 7065 6320 696e 636c 7564  nAPI spec includ
+00000bc0: 6564 2077 6974 6820 796f 7572 2041 5049  ed with your API
+00000bd0: 732e 0a20 202d 20e2 9aa1 efb8 8f20 5365  s..  - ...... Se
+00000be0: 7276 6572 6c65 7373 2061 7070 7320 7468  rverless apps th
+00000bf0: 6174 2073 6361 6c65 7320 6175 746f 6d61  at scales automa
+00000c00: 7469 6361 6c6c 7920 7769 7468 2079 6f75  tically with you
+00000c10: 7220 7472 6166 6669 632e 0a20 202d 20f0  r traffic..  - .
+00000c20: 9f93 8a20 4275 696c 7469 6e20 6c6f 6767  ... Builtin logg
+00000c30: 696e 672c 206d 6f6e 6974 6f72 696e 672c  ing, monitoring,
+00000c40: 2061 6e64 2074 7261 6365 7320 666f 7220   and traces for 
+00000c50: 796f 7572 2041 5049 732e 0a20 202d 20f0  your APIs..  - .
+00000c60: 9fa4 9620 4e6f 206e 6565 6420 746f 2063  ... No need to c
+00000c70: 6861 6e67 6520 796f 7572 2063 6f64 6520  hange your code 
+00000c80: 746f 206d 616e 6167 6520 4150 4973 2c20  to manage APIs, 
+00000c90: 6f72 206d 616e 6167 6520 646f 636b 6572  or manage docker
+00000ca0: 6669 6c65 732c 206f 7220 776f 7272 7920  files, or worry 
+00000cb0: 6162 6f75 7420 696e 6672 6173 7472 7563  about infrastruc
+00000cc0: 7475 7265 210a 0a0a 2323 2323 20f0 9f9a  ture!...#### ...
+00000cd0: a720 436f 6d69 6e67 2073 6f6f 6e0a 0a2d  . Coming soon..-
+00000ce0: 205b 205d 20f0 9f94 9120 4175 7468 6f72   [ ] .... Author
+00000cf0: 697a 6520 4150 4920 656e 6470 6f69 6e74  ize API endpoint
+00000d00: 730a 2d20 5b20 5d20 f09f 9ba0 efb8 8f20  s.- [ ] ....... 
+00000d10: 456e 6162 6c65 2053 7472 6561 6d6c 6974  Enable Streamlit
+00000d20: 2070 6c61 7967 726f 756e 6420 6465 706c   playground depl
+00000d30: 6f79 6d65 6e74 2066 6f72 2079 6f75 7220  oyment for your 
+00000d40: 6170 7073 0a0a 0a49 6620 796f 7520 6861  apps...If you ha
+00000d50: 7665 2061 6e79 2066 6561 7475 7265 2072  ve any feature r
+00000d60: 6571 7565 7374 7320 6f72 2066 6163 6564  equests or faced
+00000d70: 2061 6e79 2069 7373 7565 2c20 706c 6561   any issue, plea
+00000d80: 7365 205b 6c65 7420 7573 206b 6e6f 775d  se [let us know]
+00000d90: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00000da0: 636f 6d2f 6a69 6e61 2d61 692f 6c61 6e67  com/jina-ai/lang
+00000db0: 6368 6169 6e2d 7365 7276 652f 6973 7375  chain-serve/issu
+00000dc0: 6573 2f6e 6577 2921 0a0a 0a23 2320 5573  es/new)!...## Us
+00000dd0: 6167 650a 0a4c 6574 2773 2066 6972 7374  age..Let's first
+00000de0: 2069 6e73 7461 6c6c 2060 6c61 6e67 6368   install `langch
+00000df0: 6169 6e2d 7365 7276 6560 2075 7369 6e67  ain-serve` using
+00000e00: 2070 6970 2e0a 0a60 6060 6261 7368 0a70   pip...```bash.p
+00000e10: 6970 2069 6e73 7461 6c6c 206c 616e 6763  ip install langc
+00000e20: 6861 696e 2d73 6572 7665 0a60 6060 0a0a  hain-serve.```..
+00000e30: 2323 2045 6e61 626c 6520 4875 6d61 6e2d  ## Enable Human-
+00000e40: 696e 2d74 6865 2d6c 6f6f 7020 2848 4954  in-the-loop (HIT
+00000e50: 4c29 2066 6f72 2079 6f75 7220 6167 656e  L) for your agen
+00000e60: 7473 0a0a 4849 544c 2066 6f72 204c 616e  ts..HITL for Lan
+00000e70: 6743 6861 696e 2061 6765 6e74 7320 6f6e  gChain agents on
+00000e80: 2070 726f 6475 6374 696f 6e20 6361 6e20   production can 
+00000e90: 6265 2063 6861 6c6c 656e 6769 6e67 2073  be challenging s
+00000ea0: 696e 6365 2074 6865 2061 6765 6e74 7320  ince the agents 
+00000eb0: 6172 6520 7479 7069 6361 6c6c 7920 7275  are typically ru
+00000ec0: 6e6e 696e 6720 6f6e 2073 6572 7665 7273  nning on servers
+00000ed0: 2077 6865 7265 2068 756d 616e 7320 646f   where humans do
+00000ee0: 6e27 7420 6861 7665 2064 6972 6563 7420  n't have direct 
+00000ef0: 6163 6365 7373 2e20 2a2a 6c61 6e67 6368  access. **langch
+00000f00: 6169 6e2d 7365 7276 652a 2a20 6272 6964  ain-serve** brid
+00000f10: 6765 7320 7468 6973 2067 6170 2062 7920  ges this gap by 
+00000f20: 656e 6162 6c69 6e67 2077 6562 736f 636b  enabling websock
+00000f30: 6574 2041 5049 7320 7468 6174 2061 6c6c  et APIs that all
+00000f40: 6f77 2066 6f72 2072 6561 6c2d 7469 6d65  ow for real-time
+00000f50: 2069 6e74 6572 6163 7469 6f6e 2061 6e64   interaction and
+00000f60: 2066 6565 6462 6163 6b20 6265 7477 6565   feedback betwee
+00000f70: 6e20 7468 6520 6167 656e 7420 616e 6420  n the agent and 
+00000f80: 6120 6875 6d61 6e20 6f70 6572 6174 6f72  a human operator
+00000f90: 2e0a 0a43 6865 636b 206f 7574 2074 6869  ...Check out thi
+00000fa0: 7320 5b65 7861 6d70 6c65 5d28 6578 616d  s [example](exam
+00000fb0: 706c 6573 2f77 6562 736f 636b 6574 732f  ples/websockets/
+00000fc0: 6869 746c 2f52 4541 444d 452e 6d64 2920  hitl/README.md) 
+00000fd0: 746f 2073 6565 2068 6f77 2079 6f75 2063  to see how you c
+00000fe0: 616e 2065 6e61 626c 6520 4849 544c 2066  an enable HITL f
+00000ff0: 6f72 2079 6f75 7220 6167 656e 7473 2e0a  or your agents..
+00001000: 0a0a 2323 2045 6e61 626c 6520 5245 5354  ..## Enable REST
+00001010: 2041 5049 7320 0a0a 0a4c 6574 2773 2062   APIs ...Let's b
+00001020: 7569 6c64 2061 2063 7573 746f 6d20 6167  uild a custom ag
+00001030: 656e 7420 7573 696e 6720 7468 6973 2065  ent using this e
+00001040: 7861 6d70 6c65 2074 616b 656e 2066 726f  xample taken fro
+00001050: 6d20 5b4c 616e 6743 6861 696e 2064 6f63  m [LangChain doc
+00001060: 756d 656e 7461 7469 6f6e 5d28 6874 7470  umentation](http
+00001070: 733a 2f2f 7079 7468 6f6e 2e6c 616e 6763  s://python.langc
+00001080: 6861 696e 2e63 6f6d 2f65 6e2f 6c61 7465  hain.com/en/late
+00001090: 7374 2f6d 6f64 756c 6573 2f61 6765 6e74  st/modules/agent
+000010a0: 732f 6167 656e 7473 2f63 7573 746f 6d5f  s/agents/custom_
+000010b0: 6167 656e 742e 6874 6d6c 292e 200a 0a0a  agent.html). ...
+000010c0: 3c64 6574 6169 6c73 3e0a 3c73 756d 6d61  <details>.<summa
+000010d0: 7279 3e53 686f 7720 6167 656e 7420 636f  ry>Show agent co
+000010e0: 6465 2028 6170 702e 7079 293c 2f73 756d  de (app.py)</sum
+000010f0: 6d61 7279 3e0a 0a60 6060 7079 7468 6f6e  mary>..```python
+00001100: 0a23 2061 7070 2e70 790a 6672 6f6d 206c  .# app.py.from l
+00001110: 616e 6763 6861 696e 2e61 6765 6e74 7320  angchain.agents 
+00001120: 696d 706f 7274 205a 6572 6f53 686f 7441  import ZeroShotA
+00001130: 6765 6e74 2c20 546f 6f6c 2c20 4167 656e  gent, Tool, Agen
+00001140: 7445 7865 6375 746f 720a 6672 6f6d 206c  tExecutor.from l
+00001150: 616e 6763 6861 696e 2069 6d70 6f72 7420  angchain import 
+00001160: 4f70 656e 4149 2c20 5365 7270 4150 4957  OpenAI, SerpAPIW
+00001170: 7261 7070 6572 2c20 4c4c 4d43 6861 696e  rapper, LLMChain
+00001180: 0a0a 7365 6172 6368 203d 2053 6572 7041  ..search = SerpA
+00001190: 5049 5772 6170 7065 7228 290a 746f 6f6c  PIWrapper().tool
+000011a0: 7320 3d20 5b0a 2020 2020 546f 6f6c 280a  s = [.    Tool(.
+000011b0: 2020 2020 2020 2020 6e61 6d65 203d 2022          name = "
+000011c0: 5365 6172 6368 222c 0a20 2020 2020 2020  Search",.       
+000011d0: 2066 756e 633d 7365 6172 6368 2e72 756e   func=search.run
+000011e0: 2c0a 2020 2020 2020 2020 6465 7363 7269  ,.        descri
+000011f0: 7074 696f 6e3d 2275 7365 6675 6c20 666f  ption="useful fo
+00001200: 7220 7768 656e 2079 6f75 206e 6565 6420  r when you need 
+00001210: 746f 2061 6e73 7765 7220 7175 6573 7469  to answer questi
+00001220: 6f6e 7320 6162 6f75 7420 6375 7272 656e  ons about curren
+00001230: 7420 6576 656e 7473 220a 2020 2020 290a  t events".    ).
+00001240: 5d0a 0a70 7265 6669 7820 3d20 2222 2241  ]..prefix = """A
+00001250: 6e73 7765 7220 7468 6520 666f 6c6c 6f77  nswer the follow
+00001260: 696e 6720 7175 6573 7469 6f6e 7320 6173  ing questions as
+00001270: 2062 6573 7420 796f 7520 6361 6e2c 2062   best you can, b
+00001280: 7574 2073 7065 616b 696e 6720 6173 2061  ut speaking as a
+00001290: 2070 6972 6174 6520 6d69 6768 7420 7370   pirate might sp
+000012a0: 6561 6b2e 2059 6f75 2068 6176 6520 6163  eak. You have ac
+000012b0: 6365 7373 2074 6f20 7468 6520 666f 6c6c  cess to the foll
+000012c0: 6f77 696e 6720 746f 6f6c 733a 2222 220a  owing tools:""".
+000012d0: 7375 6666 6978 203d 2022 2222 4265 6769  suffix = """Begi
+000012e0: 6e21 2052 656d 656d 6265 7220 746f 2073  n! Remember to s
+000012f0: 7065 616b 2061 7320 6120 7069 7261 7465  peak as a pirate
+00001300: 2077 6865 6e20 6769 7669 6e67 2079 6f75   when giving you
+00001310: 7220 6669 6e61 6c20 616e 7377 6572 2e20  r final answer. 
+00001320: 5573 6520 6c6f 7473 206f 6620 2241 7267  Use lots of "Arg
+00001330: 7322 0a0a 5175 6573 7469 6f6e 3a20 7b69  s"..Question: {i
+00001340: 6e70 7574 7d0a 7b61 6765 6e74 5f73 6372  nput}.{agent_scr
+00001350: 6174 6368 7061 647d 2222 220a 0a70 726f  atchpad}"""..pro
+00001360: 6d70 7420 3d20 5a65 726f 5368 6f74 4167  mpt = ZeroShotAg
+00001370: 656e 742e 6372 6561 7465 5f70 726f 6d70  ent.create_promp
+00001380: 7428 0a20 2020 2074 6f6f 6c73 2c20 0a20  t(.    tools, . 
+00001390: 2020 2070 7265 6669 783d 7072 6566 6978     prefix=prefix
+000013a0: 2c20 0a20 2020 2073 7566 6669 783d 7375  , .    suffix=su
+000013b0: 6666 6978 2c20 0a20 2020 2069 6e70 7574  ffix, .    input
+000013c0: 5f76 6172 6961 626c 6573 3d5b 2269 6e70  _variables=["inp
+000013d0: 7574 222c 2022 6167 656e 745f 7363 7261  ut", "agent_scra
+000013e0: 7463 6870 6164 225d 0a29 0a0a 6c6c 6d5f  tchpad"].)..llm_
+000013f0: 6368 6169 6e20 3d20 4c4c 4d43 6861 696e  chain = LLMChain
+00001400: 286c 6c6d 3d4f 7065 6e41 4928 7465 6d70  (llm=OpenAI(temp
+00001410: 6572 6174 7572 653d 3029 2c20 7072 6f6d  erature=0), prom
+00001420: 7074 3d70 726f 6d70 7429 0a74 6f6f 6c5f  pt=prompt).tool_
+00001430: 6e61 6d65 7320 3d20 5b74 6f6f 6c2e 6e61  names = [tool.na
+00001440: 6d65 2066 6f72 2074 6f6f 6c20 696e 2074  me for tool in t
+00001450: 6f6f 6c73 5d0a 6167 656e 7420 3d20 5a65  ools].agent = Ze
+00001460: 726f 5368 6f74 4167 656e 7428 6c6c 6d5f  roShotAgent(llm_
+00001470: 6368 6169 6e3d 6c6c 6d5f 6368 6169 6e2c  chain=llm_chain,
+00001480: 2061 6c6c 6f77 6564 5f74 6f6f 6c73 3d74   allowed_tools=t
+00001490: 6f6f 6c5f 6e61 6d65 7329 0a61 6765 6e74  ool_names).agent
+000014a0: 5f65 7865 6375 746f 7220 3d20 4167 656e  _executor = Agen
+000014b0: 7445 7865 6375 746f 722e 6672 6f6d 5f61  tExecutor.from_a
+000014c0: 6765 6e74 5f61 6e64 5f74 6f6f 6c73 2861  gent_and_tools(a
+000014d0: 6765 6e74 3d61 6765 6e74 2c20 746f 6f6c  gent=agent, tool
+000014e0: 733d 746f 6f6c 732c 2076 6572 626f 7365  s=tools, verbose
+000014f0: 3d54 7275 6529 0a61 6765 6e74 5f65 7865  =True).agent_exe
+00001500: 6375 746f 722e 7275 6e28 2248 6f77 206d  cutor.run("How m
+00001510: 616e 7920 7065 6f70 6c65 206c 6976 6520  any people live 
+00001520: 696e 2063 616e 6164 6120 6173 206f 6620  in canada as of 
+00001530: 3230 3233 3f22 290a 6060 600a 0a23 2323  2023?").```..###
+00001540: 2320 4f75 7470 7574 0a0a 0a60 6060 7465  # Output...```te
+00001550: 7874 0a3e 2045 6e74 6572 696e 6720 6e65  xt.> Entering ne
+00001560: 7720 4167 656e 7445 7865 6375 746f 7220  w AgentExecutor 
+00001570: 6368 6169 6e2e 2e2e 0a54 686f 7567 6874  chain....Thought
+00001580: 3a20 4920 6e65 6564 2074 6f20 6669 6e64  : I need to find
+00001590: 206f 7574 2074 6865 2070 6f70 756c 6174   out the populat
+000015a0: 696f 6e20 6f66 2043 616e 6164 610a 4163  ion of Canada.Ac
+000015b0: 7469 6f6e 3a20 5365 6172 6368 0a41 6374  tion: Search.Act
+000015c0: 696f 6e20 496e 7075 743a 2050 6f70 756c  ion Input: Popul
+000015d0: 6174 696f 6e20 6f66 2043 616e 6164 6120  ation of Canada 
+000015e0: 3230 3233 0a4f 6273 6572 7661 7469 6f6e  2023.Observation
+000015f0: 3a20 5468 6520 6375 7272 656e 7420 706f  : The current po
+00001600: 7075 6c61 7469 6f6e 206f 6620 4361 6e61  pulation of Cana
+00001610: 6461 2069 7320 3338 2c36 3130 2c34 3437  da is 38,610,447
+00001620: 2061 7320 6f66 2053 6174 7572 6461 792c   as of Saturday,
+00001630: 2046 6562 7275 6172 7920 3138 2c20 3230   February 18, 20
+00001640: 3233 2c20 6261 7365 6420 6f6e 2057 6f72  23, based on Wor
+00001650: 6c64 6f6d 6574 6572 2065 6c61 626f 7261  ldometer elabora
+00001660: 7469 6f6e 206f 6620 7468 6520 6c61 7465  tion of the late
+00001670: 7374 2055 6e69 7465 6420 4e61 7469 6f6e  st United Nation
+00001680: 7320 6461 7461 2e20 4361 6e61 6461 2032  s data. Canada 2
+00001690: 3032 3020 706f 7075 6c61 7469 6f6e 2069  020 population i
+000016a0: 7320 6573 7469 6d61 7465 6420 6174 2033  s estimated at 3
+000016b0: 372c 3734 322c 3135 3420 7065 6f70 6c65  7,742,154 people
+000016c0: 2061 7420 6d69 6420 7965 6172 2061 6363   at mid year acc
+000016d0: 6f72 6469 6e67 2074 6f20 554e 2064 6174  ording to UN dat
+000016e0: 612e 0a54 686f 7567 6874 3a20 4920 6e6f  a..Thought: I no
+000016f0: 7720 6b6e 6f77 2074 6865 2066 696e 616c  w know the final
+00001700: 2061 6e73 7765 720a 4669 6e61 6c20 416e   answer.Final An
+00001710: 7377 6572 3a20 4172 7272 2c20 4361 6e61  swer: Arrr, Cana
+00001720: 6461 2062 6520 6861 7669 6e27 2033 382c  da be havin' 38,
+00001730: 3631 302c 3434 3720 7363 616c 6c79 7761  610,447 scallywa
+00001740: 6773 206c 6976 696e 2720 7468 6572 6520  gs livin' there 
+00001750: 6173 206f 6620 3230 3233 210a 0a3e 2046  as of 2023!..> F
+00001760: 696e 6973 6865 6420 6368 6169 6e2e 0a60  inished chain..`
+00001770: 6060 0a0a 3c2f 6465 7461 696c 733e 0a0a  ``..</details>..
+00001780: 2323 2320 5374 6570 2031 3a20 0a0a 2a2a  ### Step 1: ..**
+00001790: 5265 6661 6374 6f72 2079 6f75 7220 636f  Refactor your co
+000017a0: 6465 2074 6f20 6675 6e63 7469 6f6e 2873  de to function(s
+000017b0: 2920 7468 6174 2073 686f 756c 6420 6265  ) that should be
+000017c0: 2073 6572 7665 6420 7769 7468 2060 4073   served with `@s
+000017d0: 6572 7669 6e67 6020 6465 636f 7261 746f  erving` decorato
+000017e0: 722a 2a0a 0a0a 3c64 6574 6169 6c73 3e0a  r**...<details>.
+000017f0: 3c73 756d 6d61 7279 3e53 686f 7720 7570  <summary>Show up
+00001800: 6461 7465 6420 6167 656e 7420 636f 6465  dated agent code
+00001810: 2028 6170 702e 7079 293c 2f73 756d 6d61   (app.py)</summa
+00001820: 7279 3e0a 0a60 6060 7079 7468 6f6e 0a23  ry>..```python.#
+00001830: 2061 7070 2e70 790a 6672 6f6d 206c 616e   app.py.from lan
+00001840: 6763 6861 696e 2069 6d70 6f72 7420 4c4c  gchain import LL
+00001850: 4d43 6861 696e 2c20 4f70 656e 4149 2c20  MChain, OpenAI, 
+00001860: 5365 7270 4150 4957 7261 7070 6572 0a66  SerpAPIWrapper.f
+00001870: 726f 6d20 6c61 6e67 6368 6169 6e2e 6167  rom langchain.ag
+00001880: 656e 7473 2069 6d70 6f72 7420 4167 656e  ents import Agen
+00001890: 7445 7865 6375 746f 722c 2054 6f6f 6c2c  tExecutor, Tool,
+000018a0: 205a 6572 6f53 686f 7441 6765 6e74 0a0a   ZeroShotAgent..
+000018b0: 6672 6f6d 206c 6373 6572 7665 2069 6d70  from lcserve imp
+000018c0: 6f72 7420 7365 7276 696e 670a 0a0a 4073  ort serving...@s
+000018d0: 6572 7669 6e67 0a64 6566 2061 736b 2869  erving.def ask(i
+000018e0: 6e70 7574 3a20 7374 7229 202d 3e20 7374  nput: str) -> st
+000018f0: 723a 0a20 2020 2073 6561 7263 6820 3d20  r:.    search = 
+00001900: 5365 7270 4150 4957 7261 7070 6572 2829  SerpAPIWrapper()
+00001910: 0a20 2020 2074 6f6f 6c73 203d 205b 0a20  .    tools = [. 
+00001920: 2020 2020 2020 2054 6f6f 6c28 0a20 2020         Tool(.   
+00001930: 2020 2020 2020 2020 206e 616d 653d 2253           name="S
+00001940: 6561 7263 6822 2c0a 2020 2020 2020 2020  earch",.        
+00001950: 2020 2020 6675 6e63 3d73 6561 7263 682e      func=search.
+00001960: 7275 6e2c 0a20 2020 2020 2020 2020 2020  run,.           
+00001970: 2064 6573 6372 6970 7469 6f6e 3d22 7573   description="us
+00001980: 6566 756c 2066 6f72 2077 6865 6e20 796f  eful for when yo
+00001990: 7520 6e65 6564 2074 6f20 616e 7377 6572  u need to answer
+000019a0: 2071 7565 7374 696f 6e73 2061 626f 7574   questions about
+000019b0: 2063 7572 7265 6e74 2065 7665 6e74 7322   current events"
+000019c0: 2c0a 2020 2020 2020 2020 290a 2020 2020  ,.        ).    
+000019d0: 5d0a 2020 2020 7072 6566 6978 203d 2022  ].    prefix = "
+000019e0: 2222 416e 7377 6572 2074 6865 2066 6f6c  ""Answer the fol
+000019f0: 6c6f 7769 6e67 2071 7565 7374 696f 6e73  lowing questions
+00001a00: 2061 7320 6265 7374 2079 6f75 2063 616e   as best you can
+00001a10: 2c20 6275 7420 7370 6561 6b69 6e67 2061  , but speaking a
+00001a20: 7320 6120 7069 7261 7465 206d 6967 6874  s a pirate might
+00001a30: 2073 7065 616b 2e20 596f 7520 6861 7665   speak. You have
+00001a40: 2061 6363 6573 7320 746f 2074 6865 2066   access to the f
+00001a50: 6f6c 6c6f 7769 6e67 2074 6f6f 6c73 3a22  ollowing tools:"
+00001a60: 2222 0a20 2020 2073 7566 6669 7820 3d20  "".    suffix = 
+00001a70: 2222 2242 6567 696e 2120 5265 6d65 6d62  """Begin! Rememb
+00001a80: 6572 2074 6f20 7370 6561 6b20 6173 2061  er to speak as a
+00001a90: 2070 6972 6174 6520 7768 656e 2067 6976   pirate when giv
+00001aa0: 696e 6720 796f 7572 2066 696e 616c 2061  ing your final a
+00001ab0: 6e73 7765 722e 2055 7365 206c 6f74 7320  nswer. Use lots 
+00001ac0: 6f66 2022 4172 6773 220a 0a20 2020 2051  of "Args"..    Q
+00001ad0: 7565 7374 696f 6e3a 207b 696e 7075 747d  uestion: {input}
+00001ae0: 0a20 2020 207b 6167 656e 745f 7363 7261  .    {agent_scra
+00001af0: 7463 6870 6164 7d22 2222 0a0a 2020 2020  tchpad}"""..    
+00001b00: 7072 6f6d 7074 203d 205a 6572 6f53 686f  prompt = ZeroSho
+00001b10: 7441 6765 6e74 2e63 7265 6174 655f 7072  tAgent.create_pr
+00001b20: 6f6d 7074 280a 2020 2020 2020 2020 746f  ompt(.        to
+00001b30: 6f6c 732c 0a20 2020 2020 2020 2070 7265  ols,.        pre
+00001b40: 6669 783d 7072 6566 6978 2c0a 2020 2020  fix=prefix,.    
+00001b50: 2020 2020 7375 6666 6978 3d73 7566 6669      suffix=suffi
+00001b60: 782c 0a20 2020 2020 2020 2069 6e70 7574  x,.        input
+00001b70: 5f76 6172 6961 626c 6573 3d5b 2269 6e70  _variables=["inp
+00001b80: 7574 222c 2022 6167 656e 745f 7363 7261  ut", "agent_scra
+00001b90: 7463 6870 6164 225d 2c0a 2020 2020 290a  tchpad"],.    ).
+00001ba0: 0a20 2020 2070 7269 6e74 2870 726f 6d70  .    print(promp
+00001bb0: 742e 7465 6d70 6c61 7465 290a 0a20 2020  t.template)..   
+00001bc0: 206c 6c6d 5f63 6861 696e 203d 204c 4c4d   llm_chain = LLM
+00001bd0: 4368 6169 6e28 6c6c 6d3d 4f70 656e 4149  Chain(llm=OpenAI
+00001be0: 2874 656d 7065 7261 7475 7265 3d30 292c  (temperature=0),
+00001bf0: 2070 726f 6d70 743d 7072 6f6d 7074 290a   prompt=prompt).
+00001c00: 2020 2020 746f 6f6c 5f6e 616d 6573 203d      tool_names =
+00001c10: 205b 746f 6f6c 2e6e 616d 6520 666f 7220   [tool.name for 
+00001c20: 746f 6f6c 2069 6e20 746f 6f6c 735d 0a20  tool in tools]. 
+00001c30: 2020 2061 6765 6e74 203d 205a 6572 6f53     agent = ZeroS
+00001c40: 686f 7441 6765 6e74 286c 6c6d 5f63 6861  hotAgent(llm_cha
+00001c50: 696e 3d6c 6c6d 5f63 6861 696e 2c20 616c  in=llm_chain, al
+00001c60: 6c6f 7765 645f 746f 6f6c 733d 746f 6f6c  lowed_tools=tool
+00001c70: 5f6e 616d 6573 290a 0a20 2020 2061 6765  _names)..    age
+00001c80: 6e74 5f65 7865 6375 746f 7220 3d20 4167  nt_executor = Ag
+00001c90: 656e 7445 7865 6375 746f 722e 6672 6f6d  entExecutor.from
+00001ca0: 5f61 6765 6e74 5f61 6e64 5f74 6f6f 6c73  _agent_and_tools
+00001cb0: 280a 2020 2020 2020 2020 6167 656e 743d  (.        agent=
+00001cc0: 6167 656e 742c 2074 6f6f 6c73 3d74 6f6f  agent, tools=too
+00001cd0: 6c73 2c20 7665 7262 6f73 653d 5472 7565  ls, verbose=True
+00001ce0: 0a20 2020 2029 0a0a 2020 2020 7265 7475  .    )..    retu
+00001cf0: 726e 2061 6765 6e74 5f65 7865 6375 746f  rn agent_executo
+00001d00: 722e 7275 6e28 696e 7075 7429 0a0a 6966  r.run(input)..if
+00001d10: 205f 5f6e 616d 655f 5f20 3d3d 2022 5f5f   __name__ == "__
+00001d20: 6d61 696e 5f5f 223a 0a20 2020 2061 736b  main__":.    ask
+00001d30: 2827 486f 7720 6d61 6e79 2070 656f 706c  ('How many peopl
+00001d40: 6520 6c69 7665 2069 6e20 6361 6e61 6461  e live in canada
+00001d50: 2061 7320 6f66 2032 3032 333f 2729 0a60   as of 2023?').`
+00001d60: 6060 0a0a 3c2f 6465 7461 696c 733e 0a0a  ``..</details>..
+00001d70: 0a23 2323 2323 2057 6861 7420 6368 616e  .##### What chan
+00001d80: 6765 643f 0a0a 2d20 5765 206d 6f76 6564  ged?..- We moved
+00001d90: 206f 7572 2063 6f64 6520 746f 2061 6e20   our code to an 
+00001da0: 6061 736b 6020 6675 6e63 7469 6f6e 2e0a  `ask` function..
+00001db0: 2d20 4164 6465 6420 7479 7065 2068 696e  - Added type hin
+00001dc0: 7473 2074 6f20 7468 6520 6675 6e63 7469  ts to the functi
+00001dd0: 6f6e 2070 6172 616d 6574 6572 7320 2869  on parameters (i
+00001de0: 6e70 7574 2061 6e64 206f 7574 7075 7429  nput and output)
+00001df0: 2c20 736f 2041 5049 2064 6566 696e 6974  , so API definit
+00001e00: 696f 6e20 6361 6e20 6265 2067 656e 6572  ion can be gener
+00001e10: 6174 6564 2e0a 2d20 496d 706f 7274 6564  ated..- Imported
+00001e20: 2060 6672 6f6d 206c 6373 6572 7665 2069   `from lcserve i
+00001e30: 6d70 6f72 7420 7365 7276 696e 6760 2061  mport serving` a
+00001e40: 6e64 2061 6464 6564 2060 4073 6572 7669  nd added `@servi
+00001e50: 6e67 6020 6465 636f 7261 746f 7220 746f  ng` decorator to
+00001e60: 2074 6865 2060 6173 6b60 2066 756e 6374   the `ask` funct
+00001e70: 696f 6e2e 0a2d 2041 6464 6564 2060 6966  ion..- Added `if
+00001e80: 205f 5f6e 616d 655f 5f20 3d3d 2022 5f5f   __name__ == "__
+00001e90: 6d61 696e 5f5f 223a 6020 626c 6f63 6b20  main__":` block 
+00001ea0: 746f 2074 6573 7420 7468 6520 6675 6e63  to test the func
+00001eb0: 7469 6f6e 206c 6f63 616c 6c79 2e0a 0a2d  tion locally...-
+00001ec0: 2d2d 0a0a 2323 2320 5374 6570 2032 3a0a  --..### Step 2:.
+00001ed0: 0a2a 2a43 7265 6174 6520 6120 6072 6571  .**Create a `req
+00001ee0: 7569 7265 6d65 6e74 732e 7478 7460 2066  uirements.txt` f
+00001ef0: 696c 6520 696e 2079 6f75 7220 6170 7020  ile in your app 
+00001f00: 6469 7265 6374 6f72 7920 746f 2065 6e73  directory to ens
+00001f10: 7572 6520 616c 6c20 6e65 6365 7373 6172  ure all necessar
+00001f20: 7920 6465 7065 6e64 656e 6369 6573 2061  y dependencies a
+00001f30: 7265 2069 6e73 7461 6c6c 6564 2e2a 2a0a  re installed.**.
+00001f40: 0a3c 6465 7461 696c 733e 0a3c 7375 6d6d  .<details>.<summ
+00001f50: 6172 793e 5368 6f77 2072 6571 7569 7265  ary>Show require
+00001f60: 6d65 6e74 732e 7478 743c 2f73 756d 6d61  ments.txt</summa
+00001f70: 7279 3e0a 0a60 6060 7465 7874 0a23 2072  ry>..```text.# r
+00001f80: 6571 7569 7265 6d65 6e74 732e 7478 740a  equirements.txt.
+00001f90: 6f70 656e 6169 0a67 6f6f 676c 652d 7365  openai.google-se
+00001fa0: 6172 6368 2d72 6573 756c 7473 0a60 6060  arch-results.```
+00001fb0: 0a3c 2f64 6574 6169 6c73 3e0a 0a2d 2d2d  .</details>..---
+00001fc0: 200a 0a23 2323 2053 7465 7020 333a 0a0a   ..### Step 3:..
+00001fd0: 2a2a 5275 6e20 606c 632d 7365 7276 6520  **Run `lc-serve 
+00001fe0: 6465 706c 6f79 206c 6f63 616c 2061 7070  deploy local app
+00001ff0: 6020 746f 2074 6573 7420 796f 7572 2041  ` to test your A
+00002000: 5049 206c 6f63 616c 6c79 2e2a 2a0a 0a3e  PI locally.**..>
+00002010: 2060 6170 7060 2069 7320 7468 6520 6e61   `app` is the na
+00002020: 6d65 206f 6620 7468 6520 6d6f 6475 6c65  me of the module
+00002030: 2074 6861 7420 636f 6e74 6169 6e73 2074   that contains t
+00002040: 6865 2060 6173 6b60 2066 756e 6374 696f  he `ask` functio
+00002050: 6e2e 0a0a 6060 6062 6173 680a 6c63 2d73  n...```bash.lc-s
+00002060: 6572 7665 2064 6570 6c6f 7920 6c6f 6361  erve deploy loca
+00002070: 6c20 6170 700a 6060 600a 0a3c 6465 7461  l app.```..<deta
+00002080: 696c 733e 0a3c 7375 6d6d 6172 793e 5368  ils>.<summary>Sh
+00002090: 6f77 206f 7574 7075 743c 2f73 756d 6d61  ow output</summa
+000020a0: 7279 3e0a 0a60 6060 7465 7874 0ae2 9480  ry>..```text....
+000020b0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000020c0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000020d0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000020e0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000020f0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002100: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002110: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002120: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002130: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002140: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002150: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002160: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002170: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002180: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002190: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000021a0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000021b0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000021c0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000021d0: e294 80e2 9480 e294 80e2 9480 e294 8020  ............... 
+000021e0: f09f 8e89 2046 6c6f 7720 6973 2072 6561  .... Flow is rea
+000021f0: 6479 2074 6f20 7365 7276 6521 20e2 9480  dy to serve! ...
+00002200: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002210: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002220: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002230: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002240: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002250: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002260: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002270: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002280: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002290: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000022a0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000022b0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000022c0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000022d0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000022e0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000022f0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002300: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002310: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002320: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002330: 9480 0ae2 95ad e294 80e2 9480 e294 80e2  ................
+00002340: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002350: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002360: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002370: 9480 e294 80e2 9480 e294 80e2 9480 20f0  .............. .
+00002380: 9f94 9720 456e 6470 6f69 6e74 20e2 9480  ... Endpoint ...
 00002390: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
 000023a0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
 000023b0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
 000023c0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000023d0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-000023e0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000023f0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002400: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002410: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00002420: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002430: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002440: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00002450: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002460: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002470: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00002480: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002490: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-000024a0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000024b0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000024c0: 9480 20f0 9f8e 8920 466c 6f77 2069 7320  .. .... Flow is 
-000024d0: 7265 6164 7920 746f 2073 6572 7665 2120  ready to serve! 
-000024e0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000024f0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002500: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00002510: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002520: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002530: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00002540: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002550: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002560: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00002570: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002580: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002590: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000025a0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000025b0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000023d0: 9480 e294 80e2 95ae 0ae2 9482 2020 e29b  ............  ..
+000023e0: 9320 2020 5072 6f74 6f63 6f6c 2020 2020  .   Protocol    
+000023f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002410: 2020 2020 2048 5454 5020 20e2 9482 0ae2       HTTP  .....
+00002420: 9482 2020 f09f 8fa0 2020 2020 204c 6f63  ..  ....     Loc
+00002430: 616c 2020 2020 2020 2020 2020 2020 2020  al              
+00002440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002450: 2020 2030 2e30 2e30 2e30 3a38 3038 3020     0.0.0.0:8080 
+00002460: 20e2 9482 0ae2 9482 2020 f09f 9492 2020   .......  ....  
+00002470: 2050 7269 7661 7465 2020 2020 2020 2020   Private        
+00002480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002490: 2020 3139 322e 3136 382e 3239 2e31 3835    192.168.29.185
+000024a0: 3a38 3038 3020 20e2 9482 0ae2 9482 2020  :8080  .......  
+000024b0: f09f 8c8d 2020 2020 5075 626c 6963 2020  ....    Public  
+000024c0: 3234 3035 3a32 3031 3a64 3030 373a 6538  2405:201:d007:e8
+000024d0: 6537 3a32 6333 333a 6366 3865 3a65 6436  e7:2c33:cf8e:ed6
+000024e0: 363a 3230 3138 3a38 3038 3020 20e2 9482  6:2018:8080  ...
+000024f0: 0ae2 95b0 e294 80e2 9480 e294 80e2 9480  ................
+00002500: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002510: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002520: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002530: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002540: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002550: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002560: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002570: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002580: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002590: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000025a0: 9480 e294 80e2 9480 e294 80e2 95af 0ae2  ................
+000025b0: 95ad e294 80e2 9480 e294 80e2 9480 e294  ................
 000025c0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000025d0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000025e0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000025d0: e294 8020 f09f 928e 2048 5454 5020 6578  ... .... HTTP ex
+000025e0: 7465 6e73 696f 6e20 e294 80e2 9480 e294  tension ........
 000025f0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00002600: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002610: 9480 e294 800a e295 ade2 9480 e294 80e2  ................
-00002620: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002630: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00002640: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002650: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002660: 8020 f09f 9497 2045 6e64 706f 696e 7420  . .... Endpoint 
-00002670: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002600: e294 80e2 9480 e294 80e2 9480 e295 ae0a  ................
+00002610: e294 8220 20f0 9f92 ac20 2020 2020 2020  ...  ....       
+00002620: 2020 2053 7761 6767 6572 2055 4920 2020     Swagger UI   
+00002630: 2020 2020 202e 2e2e 2f64 6f63 7320 20e2       .../docs  .
+00002640: 9482 0ae2 9482 2020 f09f 939a 2020 2020  ......  ....    
+00002650: 2020 2020 2020 2020 2020 2052 6564 6f63             Redoc
+00002660: 2020 2020 2020 202e 2e2e 2f72 6564 6f63         .../redoc
+00002670: 2020 e294 820a e295 b0e2 9480 e294 80e2    ..............
 00002680: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
 00002690: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
 000026a0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000026b0: 9480 e294 80e2 9480 e295 ae0a e294 8220  ............... 
-000026c0: 20e2 9b93 2020 2050 726f 746f 636f 6c20   ...   Protocol 
-000026d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000026e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000026f0: 2020 2020 2020 2020 4854 5450 2020 e294          HTTP  ..
-00002700: 820a e294 8220 20f0 9f8f a020 2020 2020  .....  ....     
-00002710: 4c6f 6361 6c20 2020 2020 2020 2020 2020  Local           
-00002720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002730: 2020 2020 2020 302e 302e 302e 303a 3830        0.0.0.0:80
-00002740: 3830 2020 e294 820a e294 8220 20f0 9f94  80  .......  ...
-00002750: 9220 2020 5072 6976 6174 6520 2020 2020  .   Private     
-00002760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002770: 2020 2020 2031 3932 2e31 3638 2e32 392e       192.168.29.
-00002780: 3138 353a 3830 3830 2020 e294 820a e294  185:8080  ......
-00002790: 8220 20f0 9f8c 8d20 2020 2050 7562 6c69  .  ....    Publi
-000027a0: 6320 2032 3430 353a 3230 313a 6430 3037  c  2405:201:d007
-000027b0: 3a65 3865 373a 3263 3333 3a63 6638 653a  :e8e7:2c33:cf8e:
-000027c0: 6564 3636 3a32 3031 383a 3830 3830 2020  ed66:2018:8080  
-000027d0: e294 820a e295 b0e2 9480 e294 80e2 9480  ................
-000027e0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000027f0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002800: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00002810: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002820: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002830: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00002840: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002850: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002860: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00002870: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002880: 9480 e294 80e2 9480 e294 80e2 9480 e295  ................
-00002890: af0a e295 ade2 9480 e294 80e2 9480 e294  ................
-000028a0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000028b0: e294 80e2 9480 20f0 9f92 8e20 4854 5450  ...... .... HTTP
-000028c0: 2065 7874 656e 7369 6f6e 20e2 9480 e294   extension .....
-000028d0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000028e0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000028f0: 95ae 0ae2 9482 2020 f09f 92ac 2020 2020  ......  ....    
-00002900: 2020 2020 2020 5377 6167 6765 7220 5549        Swagger UI
-00002910: 2020 2020 2020 2020 2e2e 2e2f 646f 6373          .../docs
-00002920: 2020 e294 820a e294 8220 20f0 9f93 9a20    .......  .... 
-00002930: 2020 2020 2020 2020 2020 2020 2020 5265                Re
-00002940: 646f 6320 2020 2020 2020 2e2e 2e2f 7265  doc       .../re
-00002950: 646f 6320 20e2 9482 0ae2 95b0 e294 80e2  doc  ...........
-00002960: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002970: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00002980: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002990: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-000029a0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000029b0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000029c0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-000029d0: 80e2 9480 e294 80e2 9480 e295 af0a 6060  ..............``
-000029e0: 600a 0a3c 2f64 6574 6169 6c73 3e0a 0a0a  `..</details>...
-000029f0: 4c65 7427 7320 6f70 656e 2074 6865 205b  Let's open the [
-00002a00: 5377 6167 6765 7220 5549 5d28 6874 7470  Swagger UI](http
-00002a10: 3a2f 2f6c 6f63 616c 686f 7374 3a38 3038  ://localhost:808
-00002a20: 302f 646f 6373 2920 746f 2074 6573 7420  0/docs) to test 
-00002a30: 6f75 7220 4150 4920 6c6f 6361 6c6c 792e  our API locally.
-00002a40: 2057 6974 6820 6054 7279 2069 7420 6f75   With `Try it ou
-00002a50: 7460 2062 7574 746f 6e2c 2077 6520 6361  t` button, we ca
-00002a60: 6e20 7465 7374 206f 7572 2041 5049 2077  n test our API w
-00002a70: 6974 6820 6469 6666 6572 656e 7420 696e  ith different in
-00002a80: 7075 7473 2e0a 0a0a 3c64 6574 6169 6c73  puts....<details
-00002a90: 3e0a 3c73 756d 6d61 7279 3e53 686f 7720  >.<summary>Show 
-00002aa0: 5377 6167 6765 7220 5549 3c2f 7375 6d6d  Swagger UI</summ
-00002ab0: 6172 793e 0a0a 215b 4c6f 6361 6c20 5377  ary>..![Local Sw
-00002ac0: 6167 6765 7220 5549 5d28 2e67 6974 6875  agger UI](.githu
-00002ad0: 622f 696d 6167 6573 2f6c 6f63 616c 2d73  b/images/local-s
-00002ae0: 7761 6767 6572 2d75 692e 706e 6729 0a0a  wagger-ui.png)..
-00002af0: 3c2f 6465 7461 696c 733e 0a0a 4c65 7427  </details>..Let'
-00002b00: 7320 7465 7374 206f 7572 206c 6f63 616c  s test our local
-00002b10: 2041 5049 2077 6974 6820 6048 6f77 206d   API with `How m
-00002b20: 616e 7920 7065 6f70 6c65 206c 6976 6520  any people live 
-00002b30: 696e 2063 616e 6164 6120 6173 206f 6620  in canada as of 
-00002b40: 3230 3233 3f60 2069 6e70 7574 2077 6974  2023?` input wit
-00002b50: 6820 6120 6355 524c 2063 6f6d 6d61 6e64  h a cURL command
-00002b60: 2e0a 0a60 6060 6261 7368 0a63 7572 6c20  ...```bash.curl 
-00002b70: 2d58 2027 504f 5354 2720 5c0a 2020 2768  -X 'POST' \.  'h
-00002b80: 7474 703a 2f2f 6c6f 6361 6c68 6f73 743a  ttp://localhost:
-00002b90: 3830 3830 2f61 736b 2720 5c0a 2020 2d48  8080/ask' \.  -H
-00002ba0: 2027 6163 6365 7074 3a20 6170 706c 6963   'accept: applic
-00002bb0: 6174 696f 6e2f 6a73 6f6e 2720 5c0a 2020  ation/json' \.  
-00002bc0: 2d48 2027 436f 6e74 656e 742d 5479 7065  -H 'Content-Type
-00002bd0: 3a20 6170 706c 6963 6174 696f 6e2f 6a73  : application/js
-00002be0: 6f6e 2720 5c0a 2020 2d64 2027 7b0a 2020  on' \.  -d '{.  
-00002bf0: 2269 6e70 7574 223a 2022 486f 7720 6d61  "input": "How ma
-00002c00: 6e79 2070 656f 706c 6520 6c69 7665 2069  ny people live i
-00002c10: 6e20 6361 6e61 6461 2061 7320 6f66 2032  n canada as of 2
-00002c20: 3032 333f 222c 0a20 2022 656e 7673 223a  023?",.  "envs":
-00002c30: 207b 0a20 2020 2022 4f50 454e 4149 5f41   {.    "OPENAI_A
-00002c40: 5049 5f4b 4559 223a 2022 2722 247b 4f50  PI_KEY": "'"${OP
-00002c50: 454e 4149 5f41 5049 5f4b 4559 7d22 2722  ENAI_API_KEY}"'"
-00002c60: 2c0a 2020 2020 2253 4552 5041 5049 5f41  ,.    "SERPAPI_A
-00002c70: 5049 5f4b 4559 223a 2022 2722 247b 5345  PI_KEY": "'"${SE
-00002c80: 5250 4150 495f 4150 495f 4b45 597d 2227  RPAPI_API_KEY}"'
-00002c90: 220a 2020 7d0a 7d27 0a60 6060 0a0a 6060  ".  }.}'.```..``
-00002ca0: 606a 736f 6e0a 7b0a 2020 2272 6573 756c  `json.{.  "resul
-00002cb0: 7422 3a20 2241 7272 722c 2074 6865 7265  t": "Arrr, there
-00002cc0: 2062 6520 3338 2c36 3435 2c36 3730 2070   be 38,645,670 p
-00002cd0: 656f 706c 6520 6c69 7669 6e27 2069 6e20  eople livin' in 
-00002ce0: 4361 6e61 6461 2061 7320 6f66 2032 3032  Canada as of 202
-00002cf0: 3321 222c 0a20 2022 6572 726f 7222 3a20  3!",.  "error": 
-00002d00: 2222 2c0a 2020 2273 7464 6f75 7422 3a20  "",.  "stdout": 
-00002d10: 2241 6e73 7765 7220 7468 6520 666f 6c6c  "Answer the foll
-00002d20: 6f77 696e 6720 7175 6573 7469 6f6e 7320  owing questions 
-00002d30: 6173 2062 6573 7420 796f 7520 6361 6e2c  as best you can,
-00002d40: 2062 7574 2073 7065 616b 696e 6720 6173   but speaking as
-00002d50: 2061 2070 6972 6174 6520 6d69 6768 7420   a pirate might 
-00002d60: 7370 6561 6b2e 2059 6f75 2068 6176 6520  speak. You have 
-00002d70: 6163 6365 7373 2074 6f20 7468 6520 666f  access to the fo
-00002d80: 6c6c 6f77 696e 6720 746f 6f6c 733a 5c6e  llowing tools:\n
-00002d90: 5c6e 5365 6172 6368 3a20 7573 6566 756c  \nSearch: useful
-00002da0: 2066 6f72 2077 6865 6e20 796f 7520 6e65   for when you ne
-00002db0: 6564 2074 6f20 616e 7377 6572 2071 7565  ed to answer que
-00002dc0: 7374 696f 6e73 2061 626f 7574 2063 7572  stions about cur
-00002dd0: 7265 6e74 2065 7665 6e74 735c 6e5c 6e55  rent events\n\nU
-00002de0: 7365 2074 6865 2066 6f6c 6c6f 7769 6e67  se the following
-00002df0: 2066 6f72 6d61 743a 5c6e 5c6e 5175 6573   format:\n\nQues
-00002e00: 7469 6f6e 3a20 7468 6520 696e 7075 7420  tion: the input 
-00002e10: 7175 6573 7469 6f6e 2079 6f75 206d 7573  question you mus
-00002e20: 7420 616e 7377 6572 5c6e 5468 6f75 6768  t answer\nThough
-00002e30: 743a 2079 6f75 2073 686f 756c 6420 616c  t: you should al
-00002e40: 7761 7973 2074 6869 6e6b 2061 626f 7574  ways think about
-00002e50: 2077 6861 7420 746f 2064 6f5c 6e41 6374   what to do\nAct
-00002e60: 696f 6e3a 2074 6865 2061 6374 696f 6e20  ion: the action 
-00002e70: 746f 2074 616b 652c 2073 686f 756c 6420  to take, should 
-00002e80: 6265 206f 6e65 206f 6620 5b53 6561 7263  be one of [Searc
-00002e90: 685d 5c6e 4163 7469 6f6e 2049 6e70 7574  h]\nAction Input
-00002ea0: 3a20 7468 6520 696e 7075 7420 746f 2074  : the input to t
-00002eb0: 6865 2061 6374 696f 6e5c 6e4f 6273 6572  he action\nObser
-00002ec0: 7661 7469 6f6e 3a20 7468 6520 7265 7375  vation: the resu
-00002ed0: 6c74 206f 6620 7468 6520 6163 7469 6f6e  lt of the action
-00002ee0: 5c6e 2e2e 2e20 2874 6869 7320 5468 6f75  \n... (this Thou
-00002ef0: 6768 742f 4163 7469 6f6e 2f41 6374 696f  ght/Action/Actio
-00002f00: 6e20 496e 7075 742f 4f62 7365 7276 6174  n Input/Observat
-00002f10: 696f 6e20 6361 6e20 7265 7065 6174 204e  ion can repeat N
-00002f20: 2074 696d 6573 295c 6e54 686f 7567 6874   times)\nThought
-00002f30: 3a20 4920 6e6f 7720 6b6e 6f77 2074 6865  : I now know the
-00002f40: 2066 696e 616c 2061 6e73 7765 725c 6e46   final answer\nF
-00002f50: 696e 616c 2041 6e73 7765 723a 2074 6865  inal Answer: the
-00002f60: 2066 696e 616c 2061 6e73 7765 7220 746f   final answer to
-00002f70: 2074 6865 206f 7269 6769 6e61 6c20 696e   the original in
-00002f80: 7075 7420 7175 6573 7469 6f6e 5c6e 5c6e  put question\n\n
-00002f90: 4265 6769 6e21 2052 656d 656d 6265 7220  Begin! Remember 
-00002fa0: 746f 2073 7065 616b 2061 7320 6120 7069  to speak as a pi
-00002fb0: 7261 7465 2077 6865 6e20 6769 7669 6e67  rate when giving
-00002fc0: 2079 6f75 7220 6669 6e61 6c20 616e 7377   your final answ
-00002fd0: 6572 2e20 5573 6520 6c6f 7473 206f 6620  er. Use lots of 
-00002fe0: 5c22 4172 6773 5c22 5c6e 5c6e 2020 2020  \"Args\"\n\n    
-00002ff0: 5175 6573 7469 6f6e 3a20 7b69 6e70 7574  Question: {input
-00003000: 7d5c 6e20 2020 207b 6167 656e 745f 7363  }\n    {agent_sc
-00003010: 7261 7463 6870 6164 7d5c 6e5c 6e5c 6e5c  ratchpad}\n\n\n\
-00003020: 7530 3031 625b 316d 3e20 456e 7465 7269  u001b[1m> Enteri
-00003030: 6e67 206e 6577 2041 6765 6e74 4578 6563  ng new AgentExec
-00003040: 7574 6f72 2063 6861 696e 2e2e 2e5c 7530  utor chain...\u0
-00003050: 3031 625b 306d 5c6e 5c75 3030 3162 5b33  01b[0m\n\u001b[3
-00003060: 323b 316d 5c75 3030 3162 5b31 3b33 6d5c  2;1m\u001b[1;3m\
-00003070: 6e54 686f 7567 6874 3a20 4920 6e65 6564  nThought: I need
-00003080: 2074 6f20 6669 6e64 206f 7574 2068 6f77   to find out how
-00003090: 206d 616e 7920 7065 6f70 6c65 206c 6976   many people liv
-000030a0: 6520 696e 2043 616e 6164 615c 6e41 6374  e in Canada\nAct
-000030b0: 696f 6e3a 2053 6561 7263 685c 6e41 6374  ion: Search\nAct
-000030c0: 696f 6e20 496e 7075 743a 2048 6f77 206d  ion Input: How m
-000030d0: 616e 7920 7065 6f70 6c65 206c 6976 6520  any people live 
-000030e0: 696e 2043 616e 6164 6120 6173 206f 6620  in Canada as of 
-000030f0: 3230 3233 5c75 3030 3162 5b30 6d5c 6e4f  2023\u001b[0m\nO
-00003100: 6273 6572 7661 7469 6f6e 3a20 5c75 3030  bservation: \u00
-00003110: 3162 5b33 363b 316d 5c75 3030 3162 5b31  1b[36;1m\u001b[1
-00003120: 3b33 6d54 6865 2063 7572 7265 6e74 2070  ;3mThe current p
-00003130: 6f70 756c 6174 696f 6e20 6f66 2043 616e  opulation of Can
-00003140: 6164 6120 6973 2033 382c 3634 352c 3637  ada is 38,645,67
-00003150: 3020 6173 206f 6620 5765 646e 6573 6461  0 as of Wednesda
-00003160: 792c 204d 6172 6368 2032 392c 2032 3032  y, March 29, 202
-00003170: 332c 2062 6173 6564 206f 6e20 576f 726c  3, based on Worl
-00003180: 646f 6d65 7465 7220 656c 6162 6f72 6174  dometer elaborat
-00003190: 696f 6e20 6f66 2074 6865 206c 6174 6573  ion of the lates
-000031a0: 7420 556e 6974 6564 204e 6174 696f 6e73  t United Nations
-000031b0: 2064 6174 612e 5c75 3030 3162 5b30 6d5c   data.\u001b[0m\
-000031c0: 6e54 686f 7567 6874 3a5c 7530 3031 625b  nThought:\u001b[
-000031d0: 3332 3b31 6d5c 7530 3031 625b 313b 336d  32;1m\u001b[1;3m
-000031e0: 2049 206e 6f77 206b 6e6f 7720 7468 6520   I now know the 
-000031f0: 6669 6e61 6c20 616e 7377 6572 5c6e 4669  final answer\nFi
-00003200: 6e61 6c20 416e 7377 6572 3a20 4172 7272  nal Answer: Arrr
-00003210: 2c20 7468 6572 6520 6265 2033 382c 3634  , there be 38,64
-00003220: 352c 3637 3020 7065 6f70 6c65 206c 6976  5,670 people liv
-00003230: 696e 2720 696e 2043 616e 6164 6120 6173  in' in Canada as
-00003240: 206f 6620 3230 3233 215c 7530 3031 625b   of 2023!\u001b[
-00003250: 306d 5c6e 5c6e 5c75 3030 3162 5b31 6d3e  0m\n\n\u001b[1m>
-00003260: 2046 696e 6973 6865 6420 6368 6169 6e2e   Finished chain.
-00003270: 5c75 3030 3162 5b30 6d22 0a7d 0a60 6060  \u001b[0m".}.```
-00003280: 0a0a 2323 2323 2320 5768 6174 2068 6170  ..##### What hap
-00003290: 7065 6e65 643f 0a0a 2d20 6050 4f53 5420  pened?..- `POST 
-000032a0: 2f61 736b 6020 6973 2067 656e 6572 6174  /ask` is generat
-000032b0: 6564 2066 726f 6d20 6061 736b 6020 6675  ed from `ask` fu
-000032c0: 6e63 7469 6f6e 2064 6566 696e 6564 2069  nction defined i
-000032d0: 6e20 6061 7070 2e70 7960 2e0a 2d20 6069  n `app.py`..- `i
-000032e0: 6e70 7574 6020 6973 2061 6e20 6172 6772  nput` is an argr
-000032f0: 6d65 6e74 2064 6566 696e 6564 2069 6e20  ment defined in 
-00003300: 6061 736b 6020 6675 6e63 7469 6f6e 2e20  `ask` function. 
-00003310: 0a2d 2060 656e 7673 6020 6973 2061 2064  .- `envs` is a d
-00003320: 6963 7469 6f6e 6172 7920 6f66 2065 6e76  ictionary of env
-00003330: 6972 6f6e 6d65 6e74 2076 6172 6961 626c  ironment variabl
-00003340: 6573 2074 6861 7420 7769 6c6c 2062 6520  es that will be 
-00003350: 7061 7373 6564 2074 6f20 616c 6c20 7468  passed to all th
-00003360: 6520 6675 6e63 7469 6f6e 7320 6465 636f  e functions deco
-00003370: 7261 7465 6420 7769 7468 2060 4073 6572  rated with `@ser
-00003380: 7669 6e67 6020 6465 636f 7261 746f 722e  ving` decorator.
-00003390: 0a2d 2072 6574 7572 6e20 7479 7065 206f  .- return type o
-000033a0: 6620 6061 736b 6020 6675 6e63 7469 6f6e  f `ask` function
-000033b0: 2069 7320 6073 7472 602e 2053 6f2c 2060   is `str`. So, `
-000033c0: 7265 7375 6c74 6020 776f 756c 6420 6361  result` would ca
-000033d0: 7272 7920 7468 6520 7265 7475 726e 2076  rry the return v
-000033e0: 616c 7565 206f 6620 6061 736b 6020 6675  alue of `ask` fu
-000033f0: 6e63 7469 6f6e 2e0a 2d20 4966 2074 6865  nction..- If the
-00003400: 7265 2069 7320 616e 2065 7272 6f72 2c20  re is an error, 
-00003410: 6065 7272 6f72 6020 776f 756c 6420 6361  `error` would ca
-00003420: 7272 7920 7468 6520 6572 726f 7220 6d65  rry the error me
-00003430: 7373 6167 652e 0a2d 2060 7374 646f 7574  ssage..- `stdout
-00003440: 6020 776f 756c 6420 6361 7272 7920 7468  ` would carry th
-00003450: 6520 6f75 7470 7574 206f 6620 7468 6520  e output of the 
-00003460: 6675 6e63 7469 6f6e 2064 6563 6f72 6174  function decorat
-00003470: 6564 2077 6974 6820 6040 7365 7276 696e  ed with `@servin
-00003480: 6760 2064 6563 6f72 6174 6f72 2e0a 0a0a  g` decorator....
-00003490: 2d2d 2d0a 0a23 2323 2053 7465 7020 343a  ---..### Step 4:
-000034a0: 0a0a 2a2a 5275 6e20 606c 632d 7365 7276  ..**Run `lc-serv
-000034b0: 6520 6465 706c 6f79 206a 636c 6f75 6420  e deploy jcloud 
-000034c0: 6170 7060 2074 6f20 6465 706c 6f79 2079  app` to deploy y
-000034d0: 6f75 7220 4150 4920 746f 204a 696e 6120  our API to Jina 
-000034e0: 4149 2043 6c6f 7564 2e2a 2a0a 0a60 6060  AI Cloud.**..```
-000034f0: 6261 7368 0a23 204c 6f67 696e 2074 6f20  bash.# Login to 
-00003500: 4a69 6e61 2041 4920 436c 6f75 640a 6a69  Jina AI Cloud.ji
-00003510: 6e61 2061 7574 6820 6c6f 6769 6e0a 0a23  na auth login..#
-00003520: 2044 6570 6c6f 7920 796f 7572 2061 7070   Deploy your app
-00003530: 2074 6f20 4a69 6e61 2041 4920 436c 6f75   to Jina AI Clou
-00003540: 640a 6c63 2d73 6572 7665 2064 6570 6c6f  d.lc-serve deplo
-00003550: 7920 6a63 6c6f 7564 2061 7070 0a60 6060  y jcloud app.```
-00003560: 0a0a 3c64 6574 6169 6c73 3e0a 3c73 756d  ..<details>.<sum
-00003570: 6d61 7279 3e53 686f 7720 636f 6d70 6c65  mary>Show comple
-00003580: 7465 206f 7574 7075 743c 2f73 756d 6d61  te output</summa
-00003590: 7279 3e0a 0a60 6060 7465 7874 0ae2 a087  ry>..```text....
-000035a0: 2050 7573 6869 6e67 2060 2f74 6d70 2f74   Pushing `/tmp/t
-000035b0: 6d70 376b 7435 7171 726e 6020 2e2e 2ef0  mp7kt5qqrn` ....
-000035c0: 9f94 9020 596f 7520 6172 6520 6c6f 6767  ... You are logg
-000035d0: 6564 2069 6e20 746f 204a 696e 6120 4149  ed in to Jina AI
-000035e0: 2061 7320 2a2a 2a2e 2054 6f20 6c6f 6720   as ***. To log 
-000035f0: 6f75 742c 2075 7365 206a 696e 6120 6175  out, use jina au
-00003600: 7468 206c 6f67 6f75 742e 0ae2 95ad e294  th logout.......
-00003610: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00003620: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00003630: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00003640: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00003650: e294 80e2 9480 e294 80e2 9480 2050 7562  ............ Pub
-00003660: 6c69 7368 6564 20e2 9480 e294 80e2 9480  lished .........
+000026b0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000026c0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000026d0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000026e0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000026f0: 80e2 9480 e294 80e2 95af 0a60 6060 0a0a  ...........```..
+00002700: 3c2f 6465 7461 696c 733e 0a0a 0a4c 6574  </details>...Let
+00002710: 2773 206f 7065 6e20 7468 6520 5b53 7761  's open the [Swa
+00002720: 6767 6572 2055 495d 2868 7474 703a 2f2f  gger UI](http://
+00002730: 6c6f 6361 6c68 6f73 743a 3830 3830 2f64  localhost:8080/d
+00002740: 6f63 7329 2074 6f20 7465 7374 206f 7572  ocs) to test our
+00002750: 2041 5049 206c 6f63 616c 6c79 2e20 5769   API locally. Wi
+00002760: 7468 2060 5472 7920 6974 206f 7574 6020  th `Try it out` 
+00002770: 6275 7474 6f6e 2c20 7765 2063 616e 2074  button, we can t
+00002780: 6573 7420 6f75 7220 4150 4920 7769 7468  est our API with
+00002790: 2064 6966 6665 7265 6e74 2069 6e70 7574   different input
+000027a0: 732e 0a0a 0a3c 6465 7461 696c 733e 0a3c  s....<details>.<
+000027b0: 7375 6d6d 6172 793e 5368 6f77 2053 7761  summary>Show Swa
+000027c0: 6767 6572 2055 493c 2f73 756d 6d61 7279  gger UI</summary
+000027d0: 3e0a 0a21 5b4c 6f63 616c 2053 7761 6767  >..![Local Swagg
+000027e0: 6572 2055 495d 282e 6769 7468 7562 2f69  er UI](.github/i
+000027f0: 6d61 6765 732f 6c6f 6361 6c2d 7377 6167  mages/local-swag
+00002800: 6765 722d 7569 2e70 6e67 290a 0a3c 2f64  ger-ui.png)..</d
+00002810: 6574 6169 6c73 3e0a 0a4c 6574 2773 2074  etails>..Let's t
+00002820: 6573 7420 6f75 7220 6c6f 6361 6c20 4150  est our local AP
+00002830: 4920 7769 7468 2060 486f 7720 6d61 6e79  I with `How many
+00002840: 2070 656f 706c 6520 6c69 7665 2069 6e20   people live in 
+00002850: 6361 6e61 6461 2061 7320 6f66 2032 3032  canada as of 202
+00002860: 333f 6020 696e 7075 7420 7769 7468 2061  3?` input with a
+00002870: 2063 5552 4c20 636f 6d6d 616e 642e 0a0a   cURL command...
+00002880: 6060 6062 6173 680a 6375 726c 202d 5820  ```bash.curl -X 
+00002890: 2750 4f53 5427 205c 0a20 2027 6874 7470  'POST' \.  'http
+000028a0: 3a2f 2f6c 6f63 616c 686f 7374 3a38 3038  ://localhost:808
+000028b0: 302f 6173 6b27 205c 0a20 202d 4820 2761  0/ask' \.  -H 'a
+000028c0: 6363 6570 743a 2061 7070 6c69 6361 7469  ccept: applicati
+000028d0: 6f6e 2f6a 736f 6e27 205c 0a20 202d 4820  on/json' \.  -H 
+000028e0: 2743 6f6e 7465 6e74 2d54 7970 653a 2061  'Content-Type: a
+000028f0: 7070 6c69 6361 7469 6f6e 2f6a 736f 6e27  pplication/json'
+00002900: 205c 0a20 202d 6420 277b 0a20 2022 696e   \.  -d '{.  "in
+00002910: 7075 7422 3a20 2248 6f77 206d 616e 7920  put": "How many 
+00002920: 7065 6f70 6c65 206c 6976 6520 696e 2063  people live in c
+00002930: 616e 6164 6120 6173 206f 6620 3230 3233  anada as of 2023
+00002940: 3f22 2c0a 2020 2265 6e76 7322 3a20 7b0a  ?",.  "envs": {.
+00002950: 2020 2020 224f 5045 4e41 495f 4150 495f      "OPENAI_API_
+00002960: 4b45 5922 3a20 2227 2224 7b4f 5045 4e41  KEY": "'"${OPENA
+00002970: 495f 4150 495f 4b45 597d 2227 222c 0a20  I_API_KEY}"'",. 
+00002980: 2020 2022 5345 5250 4150 495f 4150 495f     "SERPAPI_API_
+00002990: 4b45 5922 3a20 2227 2224 7b53 4552 5041  KEY": "'"${SERPA
+000029a0: 5049 5f41 5049 5f4b 4559 7d22 2722 0a20  PI_API_KEY}"'". 
+000029b0: 207d 0a7d 270a 6060 600a 0a60 6060 6a73   }.}'.```..```js
+000029c0: 6f6e 0a7b 0a20 2022 7265 7375 6c74 223a  on.{.  "result":
+000029d0: 2022 4172 7272 2c20 7468 6572 6520 6265   "Arrr, there be
+000029e0: 2033 382c 3634 352c 3637 3020 7065 6f70   38,645,670 peop
+000029f0: 6c65 206c 6976 696e 2720 696e 2043 616e  le livin' in Can
+00002a00: 6164 6120 6173 206f 6620 3230 3233 2122  ada as of 2023!"
+00002a10: 2c0a 2020 2265 7272 6f72 223a 2022 222c  ,.  "error": "",
+00002a20: 0a20 2022 7374 646f 7574 223a 2022 416e  .  "stdout": "An
+00002a30: 7377 6572 2074 6865 2066 6f6c 6c6f 7769  swer the followi
+00002a40: 6e67 2071 7565 7374 696f 6e73 2061 7320  ng questions as 
+00002a50: 6265 7374 2079 6f75 2063 616e 2c20 6275  best you can, bu
+00002a60: 7420 7370 6561 6b69 6e67 2061 7320 6120  t speaking as a 
+00002a70: 7069 7261 7465 206d 6967 6874 2073 7065  pirate might spe
+00002a80: 616b 2e20 596f 7520 6861 7665 2061 6363  ak. You have acc
+00002a90: 6573 7320 746f 2074 6865 2066 6f6c 6c6f  ess to the follo
+00002aa0: 7769 6e67 2074 6f6f 6c73 3a5c 6e5c 6e53  wing tools:\n\nS
+00002ab0: 6561 7263 683a 2075 7365 6675 6c20 666f  earch: useful fo
+00002ac0: 7220 7768 656e 2079 6f75 206e 6565 6420  r when you need 
+00002ad0: 746f 2061 6e73 7765 7220 7175 6573 7469  to answer questi
+00002ae0: 6f6e 7320 6162 6f75 7420 6375 7272 656e  ons about curren
+00002af0: 7420 6576 656e 7473 5c6e 5c6e 5573 6520  t events\n\nUse 
+00002b00: 7468 6520 666f 6c6c 6f77 696e 6720 666f  the following fo
+00002b10: 726d 6174 3a5c 6e5c 6e51 7565 7374 696f  rmat:\n\nQuestio
+00002b20: 6e3a 2074 6865 2069 6e70 7574 2071 7565  n: the input que
+00002b30: 7374 696f 6e20 796f 7520 6d75 7374 2061  stion you must a
+00002b40: 6e73 7765 725c 6e54 686f 7567 6874 3a20  nswer\nThought: 
+00002b50: 796f 7520 7368 6f75 6c64 2061 6c77 6179  you should alway
+00002b60: 7320 7468 696e 6b20 6162 6f75 7420 7768  s think about wh
+00002b70: 6174 2074 6f20 646f 5c6e 4163 7469 6f6e  at to do\nAction
+00002b80: 3a20 7468 6520 6163 7469 6f6e 2074 6f20  : the action to 
+00002b90: 7461 6b65 2c20 7368 6f75 6c64 2062 6520  take, should be 
+00002ba0: 6f6e 6520 6f66 205b 5365 6172 6368 5d5c  one of [Search]\
+00002bb0: 6e41 6374 696f 6e20 496e 7075 743a 2074  nAction Input: t
+00002bc0: 6865 2069 6e70 7574 2074 6f20 7468 6520  he input to the 
+00002bd0: 6163 7469 6f6e 5c6e 4f62 7365 7276 6174  action\nObservat
+00002be0: 696f 6e3a 2074 6865 2072 6573 756c 7420  ion: the result 
+00002bf0: 6f66 2074 6865 2061 6374 696f 6e5c 6e2e  of the action\n.
+00002c00: 2e2e 2028 7468 6973 2054 686f 7567 6874  .. (this Thought
+00002c10: 2f41 6374 696f 6e2f 4163 7469 6f6e 2049  /Action/Action I
+00002c20: 6e70 7574 2f4f 6273 6572 7661 7469 6f6e  nput/Observation
+00002c30: 2063 616e 2072 6570 6561 7420 4e20 7469   can repeat N ti
+00002c40: 6d65 7329 5c6e 5468 6f75 6768 743a 2049  mes)\nThought: I
+00002c50: 206e 6f77 206b 6e6f 7720 7468 6520 6669   now know the fi
+00002c60: 6e61 6c20 616e 7377 6572 5c6e 4669 6e61  nal answer\nFina
+00002c70: 6c20 416e 7377 6572 3a20 7468 6520 6669  l Answer: the fi
+00002c80: 6e61 6c20 616e 7377 6572 2074 6f20 7468  nal answer to th
+00002c90: 6520 6f72 6967 696e 616c 2069 6e70 7574  e original input
+00002ca0: 2071 7565 7374 696f 6e5c 6e5c 6e42 6567   question\n\nBeg
+00002cb0: 696e 2120 5265 6d65 6d62 6572 2074 6f20  in! Remember to 
+00002cc0: 7370 6561 6b20 6173 2061 2070 6972 6174  speak as a pirat
+00002cd0: 6520 7768 656e 2067 6976 696e 6720 796f  e when giving yo
+00002ce0: 7572 2066 696e 616c 2061 6e73 7765 722e  ur final answer.
+00002cf0: 2055 7365 206c 6f74 7320 6f66 205c 2241   Use lots of \"A
+00002d00: 7267 735c 225c 6e5c 6e20 2020 2051 7565  rgs\"\n\n    Que
+00002d10: 7374 696f 6e3a 207b 696e 7075 747d 5c6e  stion: {input}\n
+00002d20: 2020 2020 7b61 6765 6e74 5f73 6372 6174      {agent_scrat
+00002d30: 6368 7061 647d 5c6e 5c6e 5c6e 5c75 3030  chpad}\n\n\n\u00
+00002d40: 3162 5b31 6d3e 2045 6e74 6572 696e 6720  1b[1m> Entering 
+00002d50: 6e65 7720 4167 656e 7445 7865 6375 746f  new AgentExecuto
+00002d60: 7220 6368 6169 6e2e 2e2e 5c75 3030 3162  r chain...\u001b
+00002d70: 5b30 6d5c 6e5c 7530 3031 625b 3332 3b31  [0m\n\u001b[32;1
+00002d80: 6d5c 7530 3031 625b 313b 336d 5c6e 5468  m\u001b[1;3m\nTh
+00002d90: 6f75 6768 743a 2049 206e 6565 6420 746f  ought: I need to
+00002da0: 2066 696e 6420 6f75 7420 686f 7720 6d61   find out how ma
+00002db0: 6e79 2070 656f 706c 6520 6c69 7665 2069  ny people live i
+00002dc0: 6e20 4361 6e61 6461 5c6e 4163 7469 6f6e  n Canada\nAction
+00002dd0: 3a20 5365 6172 6368 5c6e 4163 7469 6f6e  : Search\nAction
+00002de0: 2049 6e70 7574 3a20 486f 7720 6d61 6e79   Input: How many
+00002df0: 2070 656f 706c 6520 6c69 7665 2069 6e20   people live in 
+00002e00: 4361 6e61 6461 2061 7320 6f66 2032 3032  Canada as of 202
+00002e10: 335c 7530 3031 625b 306d 5c6e 4f62 7365  3\u001b[0m\nObse
+00002e20: 7276 6174 696f 6e3a 205c 7530 3031 625b  rvation: \u001b[
+00002e30: 3336 3b31 6d5c 7530 3031 625b 313b 336d  36;1m\u001b[1;3m
+00002e40: 5468 6520 6375 7272 656e 7420 706f 7075  The current popu
+00002e50: 6c61 7469 6f6e 206f 6620 4361 6e61 6461  lation of Canada
+00002e60: 2069 7320 3338 2c36 3435 2c36 3730 2061   is 38,645,670 a
+00002e70: 7320 6f66 2057 6564 6e65 7364 6179 2c20  s of Wednesday, 
+00002e80: 4d61 7263 6820 3239 2c20 3230 3233 2c20  March 29, 2023, 
+00002e90: 6261 7365 6420 6f6e 2057 6f72 6c64 6f6d  based on Worldom
+00002ea0: 6574 6572 2065 6c61 626f 7261 7469 6f6e  eter elaboration
+00002eb0: 206f 6620 7468 6520 6c61 7465 7374 2055   of the latest U
+00002ec0: 6e69 7465 6420 4e61 7469 6f6e 7320 6461  nited Nations da
+00002ed0: 7461 2e5c 7530 3031 625b 306d 5c6e 5468  ta.\u001b[0m\nTh
+00002ee0: 6f75 6768 743a 5c75 3030 3162 5b33 323b  ought:\u001b[32;
+00002ef0: 316d 5c75 3030 3162 5b31 3b33 6d20 4920  1m\u001b[1;3m I 
+00002f00: 6e6f 7720 6b6e 6f77 2074 6865 2066 696e  now know the fin
+00002f10: 616c 2061 6e73 7765 725c 6e46 696e 616c  al answer\nFinal
+00002f20: 2041 6e73 7765 723a 2041 7272 722c 2074   Answer: Arrr, t
+00002f30: 6865 7265 2062 6520 3338 2c36 3435 2c36  here be 38,645,6
+00002f40: 3730 2070 656f 706c 6520 6c69 7669 6e27  70 people livin'
+00002f50: 2069 6e20 4361 6e61 6461 2061 7320 6f66   in Canada as of
+00002f60: 2032 3032 3321 5c75 3030 3162 5b30 6d5c   2023!\u001b[0m\
+00002f70: 6e5c 6e5c 7530 3031 625b 316d 3e20 4669  n\n\u001b[1m> Fi
+00002f80: 6e69 7368 6564 2063 6861 696e 2e5c 7530  nished chain.\u0
+00002f90: 3031 625b 306d 220a 7d0a 6060 600a 0a23  01b[0m".}.```..#
+00002fa0: 2323 2323 2057 6861 7420 6861 7070 656e  #### What happen
+00002fb0: 6564 3f0a 0a2d 2060 504f 5354 202f 6173  ed?..- `POST /as
+00002fc0: 6b60 2069 7320 6765 6e65 7261 7465 6420  k` is generated 
+00002fd0: 6672 6f6d 2060 6173 6b60 2066 756e 6374  from `ask` funct
+00002fe0: 696f 6e20 6465 6669 6e65 6420 696e 2060  ion defined in `
+00002ff0: 6170 702e 7079 602e 0a2d 2060 696e 7075  app.py`..- `inpu
+00003000: 7460 2069 7320 616e 2061 7267 726d 656e  t` is an argrmen
+00003010: 7420 6465 6669 6e65 6420 696e 2060 6173  t defined in `as
+00003020: 6b60 2066 756e 6374 696f 6e2e 200a 2d20  k` function. .- 
+00003030: 6065 6e76 7360 2069 7320 6120 6469 6374  `envs` is a dict
+00003040: 696f 6e61 7279 206f 6620 656e 7669 726f  ionary of enviro
+00003050: 6e6d 656e 7420 7661 7269 6162 6c65 7320  nment variables 
+00003060: 7468 6174 2077 696c 6c20 6265 2070 6173  that will be pas
+00003070: 7365 6420 746f 2061 6c6c 2074 6865 2066  sed to all the f
+00003080: 756e 6374 696f 6e73 2064 6563 6f72 6174  unctions decorat
+00003090: 6564 2077 6974 6820 6040 7365 7276 696e  ed with `@servin
+000030a0: 6760 2064 6563 6f72 6174 6f72 2e0a 2d20  g` decorator..- 
+000030b0: 7265 7475 726e 2074 7970 6520 6f66 2060  return type of `
+000030c0: 6173 6b60 2066 756e 6374 696f 6e20 6973  ask` function is
+000030d0: 2060 7374 7260 2e20 536f 2c20 6072 6573   `str`. So, `res
+000030e0: 756c 7460 2077 6f75 6c64 2063 6172 7279  ult` would carry
+000030f0: 2074 6865 2072 6574 7572 6e20 7661 6c75   the return valu
+00003100: 6520 6f66 2060 6173 6b60 2066 756e 6374  e of `ask` funct
+00003110: 696f 6e2e 0a2d 2049 6620 7468 6572 6520  ion..- If there 
+00003120: 6973 2061 6e20 6572 726f 722c 2060 6572  is an error, `er
+00003130: 726f 7260 2077 6f75 6c64 2063 6172 7279  ror` would carry
+00003140: 2074 6865 2065 7272 6f72 206d 6573 7361   the error messa
+00003150: 6765 2e0a 2d20 6073 7464 6f75 7460 2077  ge..- `stdout` w
+00003160: 6f75 6c64 2063 6172 7279 2074 6865 206f  ould carry the o
+00003170: 7574 7075 7420 6f66 2074 6865 2066 756e  utput of the fun
+00003180: 6374 696f 6e20 6465 636f 7261 7465 6420  ction decorated 
+00003190: 7769 7468 2060 4073 6572 7669 6e67 6020  with `@serving` 
+000031a0: 6465 636f 7261 746f 722e 0a0a 0a2d 2d2d  decorator....---
+000031b0: 0a0a 2323 2320 5374 6570 2034 3a0a 0a2a  ..### Step 4:..*
+000031c0: 2a52 756e 2060 6c63 2d73 6572 7665 2064  *Run `lc-serve d
+000031d0: 6570 6c6f 7920 6a63 6c6f 7564 2061 7070  eploy jcloud app
+000031e0: 6020 746f 2064 6570 6c6f 7920 796f 7572  ` to deploy your
+000031f0: 2041 5049 2074 6f20 4a69 6e61 2041 4920   API to Jina AI 
+00003200: 436c 6f75 642e 2a2a 0a0a 6060 6062 6173  Cloud.**..```bas
+00003210: 680a 2320 4c6f 6769 6e20 746f 204a 696e  h.# Login to Jin
+00003220: 6120 4149 2043 6c6f 7564 0a6a 696e 6120  a AI Cloud.jina 
+00003230: 6175 7468 206c 6f67 696e 0a0a 2320 4465  auth login..# De
+00003240: 706c 6f79 2079 6f75 7220 6170 7020 746f  ploy your app to
+00003250: 204a 696e 6120 4149 2043 6c6f 7564 0a6c   Jina AI Cloud.l
+00003260: 632d 7365 7276 6520 6465 706c 6f79 206a  c-serve deploy j
+00003270: 636c 6f75 6420 6170 700a 6060 600a 0a3c  cloud app.```..<
+00003280: 6465 7461 696c 733e 0a3c 7375 6d6d 6172  details>.<summar
+00003290: 793e 5368 6f77 2063 6f6d 706c 6574 6520  y>Show complete 
+000032a0: 6f75 7470 7574 3c2f 7375 6d6d 6172 793e  output</summary>
+000032b0: 0a0a 6060 6074 6578 740a e2a0 8720 5075  ..```text.... Pu
+000032c0: 7368 696e 6720 602f 746d 702f 746d 7037  shing `/tmp/tmp7
+000032d0: 6b74 3571 7172 6e60 202e 2e2e f09f 9490  kt5qqrn` .......
+000032e0: 2059 6f75 2061 7265 206c 6f67 6765 6420   You are logged 
+000032f0: 696e 2074 6f20 4a69 6e61 2041 4920 6173  in to Jina AI as
+00003300: 202a 2a2a 2e20 546f 206c 6f67 206f 7574   ***. To log out
+00003310: 2c20 7573 6520 6a69 6e61 2061 7574 6820  , use jina auth 
+00003320: 6c6f 676f 7574 2e0a e295 ade2 9480 e294  logout..........
+00003330: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00003340: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00003350: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00003360: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00003370: e294 80e2 9480 e294 8020 5075 626c 6973  ......... Publis
+00003380: 6865 6420 e294 80e2 9480 e294 80e2 9480  hed ............
+00003390: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000033a0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000033b0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000033c0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000033d0: 9480 e294 80e2 95ae 0ae2 9482 2020 2020  ............    
+000033e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000033f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003410: 2020 2020 2020 2020 2020 2020 e294 820a              ....
+00003420: e294 8220 2020 f09f 939b 204e 616d 6520  ...   .... Name 
+00003430: 2020 2020 2020 2020 2020 6e2d 3634 6131            n-64a1
+00003440: 3520 2020 2020 2020 2020 2020 2020 2020  5               
+00003450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003460: 2020 2020 20e2 9482 0ae2 9482 2020 20f0       .......   .
+00003470: 9f94 9720 4a69 6e61 2048 7562 2055 524c  ... Jina Hub URL
+00003480: 2020 2068 7474 7073 3a2f 2f63 6c6f 7564     https://cloud
+00003490: 2e6a 696e 612e 6169 2f65 7865 6375 746f  .jina.ai/executo
+000034a0: 722f 3670 317a 696f 3837 2f20 2020 e294  r/6p1zio87/   ..
+000034b0: 820a e294 8220 2020 f09f 9180 2056 6973  .....   .... Vis
+000034c0: 6962 696c 6974 7920 2020 2020 7075 626c  ibility     publ
+000034d0: 6963 2020 2020 2020 2020 2020 2020 2020  ic              
+000034e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000034f0: 2020 2020 2020 20e2 9482 0ae2 9482 2020         .......  
+00003500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003530: 2020 2020 2020 2020 2020 2020 2020 e294                ..
+00003540: 820a e295 b0e2 9480 e294 80e2 9480 e294  ................
+00003550: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00003560: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00003570: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00003580: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00003590: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000035a0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000035b0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000035c0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000035d0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000035e0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000035f0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00003600: 9480 e294 80e2 95af 0ae2 95ad e294 80e2  ................
+00003610: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00003620: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00003630: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00003640: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00003650: 8020 f09f 8e89 2046 6c6f 7720 6973 2061  . .... Flow is a
+00003660: 7661 696c 6162 6c65 2120 e294 80e2 9480  vailable! ......
 00003670: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
 00003680: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
 00003690: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
 000036a0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000036b0: 9480 e294 80e2 9480 e295 ae0a e294 8220  ............... 
+000036b0: 95ae 0ae2 9482 2020 2020 2020 2020 2020  ......          
 000036c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000036d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000036e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000036f0: 2020 2020 2020 2020 2020 2020 2020 20e2                 .
-00003700: 9482 0ae2 9482 2020 20f0 9f93 9b20 4e61  ......   .... Na
-00003710: 6d65 2020 2020 2020 2020 2020 206e 2d36  me           n-6
-00003720: 3461 3135 2020 2020 2020 2020 2020 2020  4a15            
+000036f0: 2020 2020 2020 2020 2020 20e2 9482 0ae2             .....
+00003700: 9482 2020 2049 4420 2020 2020 2020 2020  ..   ID         
+00003710: 2020 2020 2020 6c61 6e67 6368 6169 6e2d        langchain-
+00003720: 6565 3461 6566 3537 6439 2020 2020 2020  ee4aef57d9      
 00003730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003740: 2020 2020 2020 2020 e294 820a e294 8220          ....... 
-00003750: 2020 f09f 9497 204a 696e 6120 4875 6220    .... Jina Hub 
-00003760: 5552 4c20 2020 6874 7470 733a 2f2f 636c  URL   https://cl
-00003770: 6f75 642e 6a69 6e61 2e61 692f 6578 6563  oud.jina.ai/exec
-00003780: 7574 6f72 2f36 7031 7a69 6f38 372f 2020  utor/6p1zio87/  
-00003790: 20e2 9482 0ae2 9482 2020 20f0 9f91 8020   .......   .... 
-000037a0: 5669 7369 6269 6c69 7479 2020 2020 2070  Visibility     p
-000037b0: 7562 6c69 6320 2020 2020 2020 2020 2020  ublic           
-000037c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000037d0: 2020 2020 2020 2020 2020 e294 820a e294            ......
-000037e0: 8220 2020 2020 2020 2020 2020 2020 2020  .               
+00003740: 2020 2020 2020 20e2 9482 0ae2 9482 2020         .......  
+00003750: 2047 6174 6577 6179 2028 4874 7470 2920   Gateway (Http) 
+00003760: 2020 6874 7470 733a 2f2f 6c61 6e67 6368    https://langch
+00003770: 6169 6e2d 6565 3461 6566 3537 6439 2d68  ain-ee4aef57d9-h
+00003780: 7474 702e 776f 6c66 2e6a 696e 612e 6169  ttp.wolf.jina.ai
+00003790: 2020 20e2 9482 0ae2 9482 2020 2044 6173     .......   Das
+000037a0: 6862 6f61 7264 2020 2020 2020 2020 6874  hboard        ht
+000037b0: 7470 733a 2f2f 6461 7368 626f 6172 642e  tps://dashboard.
+000037c0: 776f 6c66 2e6a 696e 612e 6169 2f66 6c6f  wolf.jina.ai/flo
+000037d0: 772f 6565 3461 6566 3537 6439 2020 20e2  w/ee4aef57d9   .
+000037e0: 9482 0ae2 9482 2020 2020 2020 2020 2020  ......          
 000037f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00003800: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00003810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003820: 20e2 9482 0ae2 95b0 e294 80e2 9480 e294   ...............
-00003830: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00003840: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00003850: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00003860: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00003870: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00003880: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00003890: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000038a0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000038b0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-000038c0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000038d0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000038e0: 9480 e294 80e2 9480 e295 af0a e295 ade2  ................
+00003820: 2020 2020 2020 2020 2020 20e2 9482 0ae2             .....
+00003830: 95b0 e294 80e2 9480 e294 80e2 9480 e294  ................
+00003840: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00003850: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00003860: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00003870: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00003880: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00003890: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000038a0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000038b0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000038c0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000038d0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000038e0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
 000038f0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00003900: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00003910: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00003920: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00003930: 80e2 9480 20f0 9f8e 8920 466c 6f77 2069  .... .... Flow i
-00003940: 7320 6176 6169 6c61 626c 6521 20e2 9480  s available! ...
-00003950: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00003960: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00003970: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00003980: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00003990: 9480 e295 ae0a e294 8220 2020 2020 2020  .........       
-000039a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000039b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000039c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000039d0: 2020 2020 2020 2020 2020 2020 2020 e294                ..
-000039e0: 820a e294 8220 2020 4944 2020 2020 2020  .....   ID      
-000039f0: 2020 2020 2020 2020 206c 616e 6763 6861           langcha
-00003a00: 696e 2d65 6534 6165 6635 3764 3920 2020  in-ee4aef57d9   
-00003a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003a20: 2020 2020 2020 2020 2020 e294 820a e294            ......
-00003a30: 8220 2020 4761 7465 7761 7920 2848 7474  .   Gateway (Htt
-00003a40: 7029 2020 2068 7474 7073 3a2f 2f6c 616e  p)   https://lan
-00003a50: 6763 6861 696e 2d65 6534 6165 6635 3764  gchain-ee4aef57d
-00003a60: 392d 6874 7470 2e77 6f6c 662e 6a69 6e61  9-http.wolf.jina
-00003a70: 2e61 6920 2020 e294 820a e294 8220 2020  .ai   .......   
-00003a80: 4461 7368 626f 6172 6420 2020 2020 2020  Dashboard       
-00003a90: 2068 7474 7073 3a2f 2f64 6173 6862 6f61   https://dashboa
-00003aa0: 7264 2e77 6f6c 662e 6a69 6e61 2e61 692f  rd.wolf.jina.ai/
-00003ab0: 666c 6f77 2f65 6534 6165 6635 3764 3920  flow/ee4aef57d9 
-00003ac0: 2020 e294 820a e294 8220 2020 2020 2020    .......       
-00003ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003b00: 2020 2020 2020 2020 2020 2020 2020 e294                ..
-00003b10: 820a e295 b0e2 9480 e294 80e2 9480 e294  ................
+00003900: 80e2 95af 0a60 6060 0a3c 2f64 6574 6169  .....```.</detai
+00003910: 6c73 3e0a 0a0a 6060 6074 6578 740a e295  ls>...```text...
+00003920: ade2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00003930: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00003940: 9480 e294 80e2 9480 e294 80e2 94ac e294  ................
+00003950: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00003960: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00003970: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00003980: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00003990: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000039a0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000039b0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000039c0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000039d0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000039e0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000039f0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00003a00: 9480 e294 80e2 95ae 0ae2 9482 2041 7070  ............ App
+00003a10: 4944 2020 2020 2020 2020 e294 8220 2020  ID        ...   
+00003a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003a30: 206c 616e 6763 6861 696e 2d65 6534 6165   langchain-ee4ae
+00003a40: 6635 3764 3920 2020 2020 2020 2020 2020  f57d9           
+00003a50: 2020 2020 2020 2020 2020 e294 820a e294            ......
+00003a60: 9ce2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00003a70: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00003a80: 9480 e294 80e2 9480 e294 80e2 94bc e294  ................
+00003a90: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00003aa0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00003ab0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00003ac0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00003ad0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00003ae0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00003af0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00003b00: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00003b10: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
 00003b20: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
 00003b30: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00003b40: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00003b50: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00003b60: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00003b70: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00003b80: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00003b90: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00003ba0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00003bb0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00003bc0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00003bd0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00003be0: 80e2 9480 e295 af0a 6060 600a 3c2f 6465  ........```.</de
-00003bf0: 7461 696c 733e 0a0a 0a60 6060 7465 7874  tails>...```text
-00003c00: 0ae2 95ad e294 80e2 9480 e294 80e2 9480  ................
+00003b40: 9480 e294 80e2 94a4 0ae2 9482 2050 6861  ............ Pha
+00003b50: 7365 2020 2020 2020 2020 e294 8220 2020  se        ...   
+00003b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003b70: 2020 2020 2020 2020 5365 7276 696e 6720          Serving 
+00003b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003b90: 2020 2020 2020 2020 2020 e294 820a e294            ......
+00003ba0: 9ce2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00003bb0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00003bc0: 9480 e294 80e2 9480 e294 80e2 94bc e294  ................
+00003bd0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00003be0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00003bf0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00003c00: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
 00003c10: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
 00003c20: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00003c30: ace2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00003c30: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
 00003c40: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
 00003c50: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
 00003c60: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
 00003c70: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00003c80: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00003c90: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00003ca0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00003cb0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00003cc0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00003cd0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00003ce0: 9480 e294 80e2 9480 e295 ae0a e294 8220  ............... 
-00003cf0: 4170 7049 4420 2020 2020 2020 20e2 9482  AppID        ...
-00003d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003d10: 2020 2020 6c61 6e67 6368 6169 6e2d 6565      langchain-ee
-00003d20: 3461 6566 3537 6439 2020 2020 2020 2020  4aef57d9        
-00003d30: 2020 2020 2020 2020 2020 2020 20e2 9482               ...
-00003d40: 0ae2 949c e294 80e2 9480 e294 80e2 9480  ................
+00003c80: 9480 e294 80e2 94a4 0ae2 9482 2045 6e64  ............ End
+00003c90: 706f 696e 7420 2020 2020 e294 8220 2020  point     ...   
+00003ca0: 2020 2020 6874 7470 733a 2f2f 6c61 6e67      https://lang
+00003cb0: 6368 6169 6e2d 6565 3461 6566 3537 6439  chain-ee4aef57d9
+00003cc0: 2d68 7474 702e 776f 6c66 2e6a 696e 612e  -http.wolf.jina.
+00003cd0: 6169 2020 2020 2020 2020 e294 820a e294  ai        ......
+00003ce0: 9ce2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00003cf0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00003d00: 9480 e294 80e2 9480 e294 80e2 94bc e294  ................
+00003d10: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00003d20: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00003d30: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00003d40: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
 00003d50: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
 00003d60: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00003d70: bce2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00003d70: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
 00003d80: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
 00003d90: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
 00003da0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
 00003db0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00003dc0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00003dd0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00003de0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00003df0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00003e00: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00003e10: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00003e20: 9480 e294 80e2 9480 e294 a40a e294 8220  ............... 
-00003e30: 5068 6173 6520 2020 2020 2020 20e2 9482  Phase        ...
-00003e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003e50: 2020 2020 2020 2020 2020 2053 6572 7669             Servi
-00003e60: 6e67 2020 2020 2020 2020 2020 2020 2020  ng              
-00003e70: 2020 2020 2020 2020 2020 2020 20e2 9482               ...
-00003e80: 0ae2 949c e294 80e2 9480 e294 80e2 9480  ................
+00003dc0: 9480 e294 80e2 94a4 0ae2 9482 2053 7761  ............ Swa
+00003dd0: 6767 6572 2055 4920 2020 e294 8220 2020  gger UI   ...   
+00003de0: 2020 6874 7470 733a 2f2f 6c61 6e67 6368    https://langch
+00003df0: 6169 6e2d 6565 3461 6566 3537 6439 2d68  ain-ee4aef57d9-h
+00003e00: 7474 702e 776f 6c66 2e6a 696e 612e 6169  ttp.wolf.jina.ai
+00003e10: 2f64 6f63 7320 2020 2020 e294 820a e294  /docs     ......
+00003e20: 9ce2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00003e30: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00003e40: 9480 e294 80e2 9480 e294 80e2 94bc e294  ................
+00003e50: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00003e60: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00003e70: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00003e80: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
 00003e90: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
 00003ea0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00003eb0: bce2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00003eb0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
 00003ec0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
 00003ed0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
 00003ee0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
 00003ef0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00003f00: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00003f10: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00003f20: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00003f30: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00003f40: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00003f50: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00003f60: 9480 e294 80e2 9480 e294 a40a e294 8220  ............... 
-00003f70: 456e 6470 6f69 6e74 2020 2020 20e2 9482  Endpoint     ...
-00003f80: 2020 2020 2020 2068 7474 7073 3a2f 2f6c         https://l
-00003f90: 616e 6763 6861 696e 2d65 6534 6165 6635  angchain-ee4aef5
-00003fa0: 3764 392d 6874 7470 2e77 6f6c 662e 6a69  7d9-http.wolf.ji
-00003fb0: 6e61 2e61 6920 2020 2020 2020 20e2 9482  na.ai        ...
-00003fc0: 0ae2 949c e294 80e2 9480 e294 80e2 9480  ................
+00003f00: 9480 e294 80e2 94a4 0ae2 9482 204f 7065  ............ Ope
+00003f10: 6e41 5049 204a 534f 4e20 e294 8220 6874  nAPI JSON ... ht
+00003f20: 7470 733a 2f2f 6c61 6e67 6368 6169 6e2d  tps://langchain-
+00003f30: 6565 3461 6566 3537 6439 2d68 7474 702e  ee4aef57d9-http.
+00003f40: 776f 6c66 2e6a 696e 612e 6169 2f6f 7065  wolf.jina.ai/ope
+00003f50: 6e61 7069 2e6a 736f 6e20 e294 820a e295  napi.json ......
+00003f60: b0e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00003f70: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00003f80: 9480 e294 80e2 9480 e294 80e2 94b4 e294  ................
+00003f90: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00003fa0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00003fb0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00003fc0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
 00003fd0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
 00003fe0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00003ff0: bce2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00003ff0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
 00004000: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
 00004010: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
 00004020: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
 00004030: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00004040: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00004050: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00004060: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00004070: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00004080: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00004090: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000040a0: 9480 e294 80e2 9480 e294 a40a e294 8220  ............... 
-000040b0: 5377 6167 6765 7220 5549 2020 20e2 9482  Swagger UI   ...
-000040c0: 2020 2020 2068 7474 7073 3a2f 2f6c 616e       https://lan
-000040d0: 6763 6861 696e 2d65 6534 6165 6635 3764  gchain-ee4aef57d
-000040e0: 392d 6874 7470 2e77 6f6c 662e 6a69 6e61  9-http.wolf.jina
-000040f0: 2e61 692f 646f 6373 2020 2020 20e2 9482  .ai/docs     ...
-00004100: 0ae2 949c e294 80e2 9480 e294 80e2 9480  ................
-00004110: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00004120: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00004130: bce2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00004140: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00004150: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00004160: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00004170: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00004180: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00004190: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000041a0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000041b0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-000041c0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000041d0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000041e0: 9480 e294 80e2 9480 e294 a40a e294 8220  ............... 
-000041f0: 4f70 656e 4150 4920 4a53 4f4e 20e2 9482  OpenAPI JSON ...
-00004200: 2068 7474 7073 3a2f 2f6c 616e 6763 6861   https://langcha
-00004210: 696e 2d65 6534 6165 6635 3764 392d 6874  in-ee4aef57d9-ht
-00004220: 7470 2e77 6f6c 662e 6a69 6e61 2e61 692f  tp.wolf.jina.ai/
-00004230: 6f70 656e 6170 692e 6a73 6f6e 20e2 9482  openapi.json ...
-00004240: 0ae2 95b0 e294 80e2 9480 e294 80e2 9480  ................
-00004250: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00004260: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00004270: b4e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00004280: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00004290: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-000042a0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000042b0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000042c0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-000042d0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000042e0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000042f0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00004300: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00004310: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00004320: 9480 e294 80e2 9480 e295 af0a 6060 600a  ............```.
-00004330: 0a4c 6574 2773 206f 7065 6e20 7468 6520  .Let's open the 
-00004340: 5377 6167 6765 7220 5549 2074 6f20 7465  Swagger UI to te
-00004350: 7374 206f 7572 2041 5049 206f 6e20 4a69  st our API on Ji
-00004360: 6e61 2041 4920 436c 6f75 642e 2057 6974  na AI Cloud. Wit
-00004370: 6820 6054 7279 2069 7420 6f75 7460 2062  h `Try it out` b
-00004380: 7574 746f 6e2c 2077 6520 6361 6e20 7465  utton, we can te
-00004390: 7374 206f 7572 2041 5049 2077 6974 6820  st our API with 
-000043a0: 6469 6666 6572 656e 7420 696e 7075 7473  different inputs
-000043b0: 2e0a 0a3c 6465 7461 696c 733e 0a3c 7375  ...<details>.<su
-000043c0: 6d6d 6172 793e 5368 6f77 2053 7761 6767  mmary>Show Swagg
-000043d0: 6572 2055 493c 2f73 756d 6d61 7279 3e0a  er UI</summary>.
-000043e0: 0a3c 7020 666c 6f61 743d 2263 656e 7465  .<p float="cente
-000043f0: 7222 3e0a 2020 3c69 6d67 2073 7263 3d22  r">.  <img src="
-00004400: 2e67 6974 6875 622f 696d 6167 6573 2f6a  .github/images/j
-00004410: 636c 6f75 642d 7377 6167 6765 722d 7569  cloud-swagger-ui
-00004420: 2e70 6e67 2220 7769 6474 683d 2234 3030  .png" width="400
-00004430: 2220 2f3e 0a20 203c 696d 6720 7372 633d  " />.  <img src=
-00004440: 222e 6769 7468 7562 2f69 6d61 6765 732f  ".github/images/
-00004450: 6a63 6c6f 7564 2d6f 7065 6e61 7069 2e70  jcloud-openapi.p
-00004460: 6e67 2220 7769 6474 683d 2233 3030 2220  ng" width="300" 
-00004470: 2f3e 0a3c 2f70 3e0a 0a3c 2f64 6574 6169  />.</p>..</detai
-00004480: 6c73 3e0a 0a0a 4c65 7427 7320 7465 7374  ls>...Let's test
-00004490: 2074 6865 2041 5049 206f 6e20 4a43 6c6f   the API on JClo
-000044a0: 7564 2077 6974 6820 6048 6f77 206d 616e  ud with `How man
-000044b0: 7920 7065 6f70 6c65 206c 6976 6520 696e  y people live in
-000044c0: 2063 616e 6164 6120 6173 206f 6620 3230   canada as of 20
-000044d0: 3233 3f60 2069 6e70 7574 2077 6974 6820  23?` input with 
-000044e0: 6120 6355 524c 2063 6f6d 6d61 6e64 2028  a cURL command (
-000044f0: 5265 706c 6163 6520 7468 6520 486f 7374  Replace the Host
-00004500: 6e61 6d65 2077 6974 6820 796f 7572 206f  name with your o
-00004510: 776e 2068 6f73 746e 616d 6529 3a0a 0a60  wn hostname):..`
-00004520: 6060 6261 7368 0a63 7572 6c20 2d58 2027  ``bash.curl -X '
-00004530: 504f 5354 2720 5c0a 2020 2768 7474 7073  POST' \.  'https
-00004540: 3a2f 2f6c 616e 6763 6861 696e 2d65 6534  ://langchain-ee4
-00004550: 6165 6635 3764 392d 6874 7470 2e77 6f6c  aef57d9-http.wol
-00004560: 662e 6a69 6e61 2e61 692f 6173 6b27 205c  f.jina.ai/ask' \
-00004570: 0a20 202d 4820 2761 6363 6570 743a 2061  .  -H 'accept: a
-00004580: 7070 6c69 6361 7469 6f6e 2f6a 736f 6e27  pplication/json'
-00004590: 205c 0a20 202d 4820 2743 6f6e 7465 6e74   \.  -H 'Content
-000045a0: 2d54 7970 653a 2061 7070 6c69 6361 7469  -Type: applicati
-000045b0: 6f6e 2f6a 736f 6e27 205c 0a20 202d 6420  on/json' \.  -d 
-000045c0: 277b 0a20 2022 696e 7075 7422 3a20 2248  '{.  "input": "H
-000045d0: 6f77 206d 616e 7920 7065 6f70 6c65 206c  ow many people l
-000045e0: 6976 6520 696e 2063 616e 6164 6120 6173  ive in canada as
-000045f0: 206f 6620 3230 3233 3f22 2c0a 2020 2265   of 2023?",.  "e
-00004600: 6e76 7322 3a20 7b0a 2020 2020 224f 5045  nvs": {.    "OPE
-00004610: 4e41 495f 4150 495f 4b45 5922 3a20 2227  NAI_API_KEY": "'
-00004620: 2224 7b4f 5045 4e41 495f 4150 495f 4b45  "${OPENAI_API_KE
-00004630: 597d 2227 222c 0a20 2020 2022 5345 5250  Y}"'",.    "SERP
-00004640: 4150 495f 4150 495f 4b45 5922 3a20 2227  API_API_KEY": "'
-00004650: 2224 7b53 4552 5041 5049 5f41 5049 5f4b  "${SERPAPI_API_K
-00004660: 4559 7d22 2722 0a20 207d 0a7d 270a 6060  EY}"'".  }.}'.``
-00004670: 600a 0a60 6060 6a73 6f6e 0a7b 0a20 2022  `..```json.{.  "
-00004680: 7265 7375 6c74 223a 2022 4172 7272 2c20  result": "Arrr, 
-00004690: 7468 6572 6520 6265 2033 382c 3634 352c  there be 38,645,
-000046a0: 3637 3020 7065 6f70 6c65 206c 6976 696e  670 people livin
-000046b0: 2720 696e 2043 616e 6164 6120 6173 206f  ' in Canada as o
-000046c0: 6620 3230 3233 2122 2c0a 2020 2265 7272  f 2023!",.  "err
-000046d0: 6f72 223a 2022 222c 0a20 2022 7374 646f  or": "",.  "stdo
-000046e0: 7574 223a 2022 416e 7377 6572 2074 6865  ut": "Answer the
-000046f0: 2066 6f6c 6c6f 7769 6e67 2071 7565 7374   following quest
-00004700: 696f 6e73 2061 7320 6265 7374 2079 6f75  ions as best you
-00004710: 2063 616e 2c20 6275 7420 7370 6561 6b69   can, but speaki
-00004720: 6e67 2061 7320 6120 7069 7261 7465 206d  ng as a pirate m
-00004730: 6967 6874 2073 7065 616b 2e20 596f 7520  ight speak. You 
-00004740: 6861 7665 2061 6363 6573 7320 746f 2074  have access to t
-00004750: 6865 2066 6f6c 6c6f 7769 6e67 2074 6f6f  he following too
-00004760: 6c73 3a5c 6e5c 6e53 6561 7263 683a 2075  ls:\n\nSearch: u
-00004770: 7365 6675 6c20 666f 7220 7768 656e 2079  seful for when y
-00004780: 6f75 206e 6565 6420 746f 2061 6e73 7765  ou need to answe
-00004790: 7220 7175 6573 7469 6f6e 7320 6162 6f75  r questions abou
-000047a0: 7420 6375 7272 656e 7420 6576 656e 7473  t current events
-000047b0: 5c6e 5c6e 5573 6520 7468 6520 666f 6c6c  \n\nUse the foll
-000047c0: 6f77 696e 6720 666f 726d 6174 3a5c 6e5c  owing format:\n\
-000047d0: 6e51 7565 7374 696f 6e3a 2074 6865 2069  nQuestion: the i
-000047e0: 6e70 7574 2071 7565 7374 696f 6e20 796f  nput question yo
-000047f0: 7520 6d75 7374 2061 6e73 7765 725c 6e54  u must answer\nT
-00004800: 686f 7567 6874 3a20 796f 7520 7368 6f75  hought: you shou
-00004810: 6c64 2061 6c77 6179 7320 7468 696e 6b20  ld always think 
-00004820: 6162 6f75 7420 7768 6174 2074 6f20 646f  about what to do
-00004830: 5c6e 4163 7469 6f6e 3a20 7468 6520 6163  \nAction: the ac
-00004840: 7469 6f6e 2074 6f20 7461 6b65 2c20 7368  tion to take, sh
-00004850: 6f75 6c64 2062 6520 6f6e 6520 6f66 205b  ould be one of [
-00004860: 5365 6172 6368 5d5c 6e41 6374 696f 6e20  Search]\nAction 
-00004870: 496e 7075 743a 2074 6865 2069 6e70 7574  Input: the input
-00004880: 2074 6f20 7468 6520 6163 7469 6f6e 5c6e   to the action\n
-00004890: 4f62 7365 7276 6174 696f 6e3a 2074 6865  Observation: the
-000048a0: 2072 6573 756c 7420 6f66 2074 6865 2061   result of the a
-000048b0: 6374 696f 6e5c 6e2e 2e2e 2028 7468 6973  ction\n... (this
-000048c0: 2054 686f 7567 6874 2f41 6374 696f 6e2f   Thought/Action/
-000048d0: 4163 7469 6f6e 2049 6e70 7574 2f4f 6273  Action Input/Obs
-000048e0: 6572 7661 7469 6f6e 2063 616e 2072 6570  ervation can rep
-000048f0: 6561 7420 4e20 7469 6d65 7329 5c6e 5468  eat N times)\nTh
-00004900: 6f75 6768 743a 2049 206e 6f77 206b 6e6f  ought: I now kno
-00004910: 7720 7468 6520 6669 6e61 6c20 616e 7377  w the final answ
-00004920: 6572 5c6e 4669 6e61 6c20 416e 7377 6572  er\nFinal Answer
-00004930: 3a20 7468 6520 6669 6e61 6c20 616e 7377  : the final answ
-00004940: 6572 2074 6f20 7468 6520 6f72 6967 696e  er to the origin
-00004950: 616c 2069 6e70 7574 2071 7565 7374 696f  al input questio
-00004960: 6e5c 6e5c 6e42 6567 696e 2120 5265 6d65  n\n\nBegin! Reme
-00004970: 6d62 6572 2074 6f20 7370 6561 6b20 6173  mber to speak as
-00004980: 2061 2070 6972 6174 6520 7768 656e 2067   a pirate when g
-00004990: 6976 696e 6720 796f 7572 2066 696e 616c  iving your final
-000049a0: 2061 6e73 7765 722e 2055 7365 206c 6f74   answer. Use lot
-000049b0: 7320 6f66 205c 2241 7267 735c 225c 6e5c  s of \"Args\"\n\
-000049c0: 6e20 2020 2051 7565 7374 696f 6e3a 207b  n    Question: {
-000049d0: 696e 7075 747d 5c6e 2020 2020 7b61 6765  input}\n    {age
-000049e0: 6e74 5f73 6372 6174 6368 7061 647d 5c6e  nt_scratchpad}\n
-000049f0: 5c6e 5c6e 5c75 3030 3162 5b31 6d3e 2045  \n\n\u001b[1m> E
-00004a00: 6e74 6572 696e 6720 6e65 7720 4167 656e  ntering new Agen
-00004a10: 7445 7865 6375 746f 7220 6368 6169 6e2e  tExecutor chain.
-00004a20: 2e2e 5c75 3030 3162 5b30 6d5c 6e5c 7530  ..\u001b[0m\n\u0
-00004a30: 3031 625b 3332 3b31 6d5c 7530 3031 625b  01b[32;1m\u001b[
-00004a40: 313b 336d 5c6e 5468 6f75 6768 743a 2049  1;3m\nThought: I
-00004a50: 206e 6565 6420 746f 2066 696e 6420 6f75   need to find ou
-00004a60: 7420 686f 7720 6d61 6e79 2070 656f 706c  t how many peopl
-00004a70: 6520 6c69 7665 2069 6e20 4361 6e61 6461  e live in Canada
-00004a80: 5c6e 4163 7469 6f6e 3a20 5365 6172 6368  \nAction: Search
-00004a90: 5c6e 4163 7469 6f6e 2049 6e70 7574 3a20  \nAction Input: 
-00004aa0: 486f 7720 6d61 6e79 2070 656f 706c 6520  How many people 
-00004ab0: 6c69 7665 2069 6e20 4361 6e61 6461 2061  live in Canada a
-00004ac0: 7320 6f66 2032 3032 335c 7530 3031 625b  s of 2023\u001b[
-00004ad0: 306d 5c6e 4f62 7365 7276 6174 696f 6e3a  0m\nObservation:
-00004ae0: 205c 7530 3031 625b 3336 3b31 6d5c 7530   \u001b[36;1m\u0
-00004af0: 3031 625b 313b 336d 5468 6520 6375 7272  01b[1;3mThe curr
-00004b00: 656e 7420 706f 7075 6c61 7469 6f6e 206f  ent population o
-00004b10: 6620 4361 6e61 6461 2069 7320 3338 2c36  f Canada is 38,6
-00004b20: 3435 2c36 3730 2061 7320 6f66 2057 6564  45,670 as of Wed
-00004b30: 6e65 7364 6179 2c20 4d61 7263 6820 3239  nesday, March 29
-00004b40: 2c20 3230 3233 2c20 6261 7365 6420 6f6e  , 2023, based on
-00004b50: 2057 6f72 6c64 6f6d 6574 6572 2065 6c61   Worldometer ela
-00004b60: 626f 7261 7469 6f6e 206f 6620 7468 6520  boration of the 
-00004b70: 6c61 7465 7374 2055 6e69 7465 6420 4e61  latest United Na
-00004b80: 7469 6f6e 7320 6461 7461 2e5c 7530 3031  tions data.\u001
-00004b90: 625b 306d 5c6e 5468 6f75 6768 743a 5c75  b[0m\nThought:\u
-00004ba0: 3030 3162 5b33 323b 316d 5c75 3030 3162  001b[32;1m\u001b
-00004bb0: 5b31 3b33 6d20 4920 6e6f 7720 6b6e 6f77  [1;3m I now know
-00004bc0: 2074 6865 2066 696e 616c 2061 6e73 7765   the final answe
-00004bd0: 725c 6e46 696e 616c 2041 6e73 7765 723a  r\nFinal Answer:
-00004be0: 2041 7272 722c 2074 6865 7265 2062 6520   Arrr, there be 
-00004bf0: 3338 2c36 3435 2c36 3730 2070 656f 706c  38,645,670 peopl
-00004c00: 6520 6c69 7669 6e27 2069 6e20 4361 6e61  e livin' in Cana
-00004c10: 6461 2061 7320 6f66 2032 3032 3321 5c75  da as of 2023!\u
-00004c20: 3030 3162 5b30 6d5c 6e5c 6e5c 7530 3031  001b[0m\n\n\u001
-00004c30: 625b 316d 3e20 4669 6e69 7368 6564 2063  b[1m> Finished c
-00004c40: 6861 696e 2e5c 7530 3031 625b 306d 220a  hain.\u001b[0m".
-00004c50: 7d0a 6060 600a 0a23 2323 2323 2057 6861  }.```..##### Wha
-00004c60: 7420 6861 7070 656e 6564 3f0a 0a2d 2049  t happened?..- I
-00004c70: 6e20 6120 6d61 7474 6572 206f 6620 6665  n a matter of fe
-00004c80: 7720 7365 636f 6e64 732c 2077 6527 7665  w seconds, we've
-00004c90: 2064 6570 6c6f 7965 6420 6f75 7220 4150   deployed our AP
-00004ca0: 4920 6f6e 204a 696e 6120 4149 2043 6c6f  I on Jina AI Clo
-00004cb0: 7564 20f0 9f8e 890a 2d20 5468 6520 4150  ud .....- The AP
-00004cc0: 4920 6973 2073 6572 7665 726c 6573 7320  I is serverless 
-00004cd0: 616e 6420 7363 616c 6162 6c65 2c20 736f  and scalable, so
-00004ce0: 2077 6520 6361 6e20 7363 616c 6520 7570   we can scale up
-00004cf0: 2074 6865 2041 5049 2074 6f20 6861 6e64   the API to hand
-00004d00: 6c65 206d 6f72 6520 7265 7175 6573 7473  le more requests
-00004d10: 2e20 0a2d 2059 6f75 206d 6967 6874 206f  . .- You might o
-00004d20: 6273 6572 7665 2061 2064 656c 6179 2069  bserve a delay i
-00004d30: 6e20 7468 6520 6669 7273 7420 7265 7175  n the first requ
-00004d40: 6573 742c 2074 6861 7427 7320 6475 6520  est, that's due 
-00004d50: 746f 2074 6865 2077 6172 6d2d 7570 2074  to the warm-up t
-00004d60: 696d 6520 6f66 2074 6865 2041 5049 2e20  ime of the API. 
-00004d70: 5375 6273 6571 7565 6e74 2072 6571 7565  Subsequent reque
-00004d80: 7374 7320 7769 6c6c 2062 6520 6661 7374  sts will be fast
-00004d90: 6572 2e0a 2d20 5468 6520 4150 4920 696e  er..- The API in
-00004da0: 636c 7564 6573 2061 2053 7761 6767 6572  cludes a Swagger
-00004db0: 2055 4920 616e 6420 7468 6520 4f70 656e   UI and the Open
-00004dc0: 4150 4920 7370 6563 6966 6963 6174 696f  API specificatio
-00004dd0: 6e2c 2073 6f20 6974 2063 616e 2062 6520  n, so it can be 
-00004de0: 6561 7369 6c79 2069 6e74 6567 7261 7465  easily integrate
-00004df0: 6420 7769 7468 206f 7468 6572 2073 6572  d with other ser
-00004e00: 7669 6365 732e 200a 2d20 4e6f 772c 206f  vices. .- Now, o
-00004e10: 7468 6572 2061 6765 6e74 7320 6361 6e20  ther agents can 
-00004e20: 696e 7465 6772 6174 6520 7769 7468 2079  integrate with y
-00004e30: 6f75 7220 6167 656e 7473 206f 6e20 4a69  our agents on Ji
-00004e40: 6e61 2041 4920 436c 6f75 6420 7468 616e  na AI Cloud than
-00004e50: 6b73 2074 6f20 7468 6520 5b4f 7065 6e41  ks to the [OpenA
-00004e60: 5049 2041 6765 6e74 5d28 6874 7470 733a  PI Agent](https:
-00004e70: 2f2f 7079 7468 6f6e 2e6c 616e 6763 6861  //python.langcha
-00004e80: 696e 2e63 6f6d 2f65 6e2f 6c61 7465 7374  in.com/en/latest
-00004e90: 2f6d 6f64 756c 6573 2f61 6765 6e74 732f  /modules/agents/
-00004ea0: 746f 6f6c 6b69 7473 2f65 7861 6d70 6c65  toolkits/example
-00004eb0: 732f 6f70 656e 6170 692e 6874 6d6c 2920  s/openapi.html) 
-00004ec0: f09f 92a1 0a0a 0a0a 2d2d 2d0a 0a23 2323  ........---..###
-00004ed0: 2320 5265 6163 6820 6f75 7420 746f 2075  # Reach out to u
-00004ee0: 7320 f09f 939e 0a0a 2d20 5365 7276 6572  s ......- Server
-00004ef0: 6c65 7373 2069 7320 6e6f 7420 796f 7572  less is not your
-00004f00: 2074 6869 6e67 3f0a 2d20 446f 2079 6f75   thing?.- Do you
-00004f10: 2077 616e 7420 6c61 7267 6572 2069 6e73   want larger ins
-00004f20: 7461 6e63 6573 2066 6f72 2079 6f75 7220  tances for your 
-00004f30: 4150 493f 0a2d 204c 6f6f 6b69 6e67 2066  API?.- Looking f
-00004f40: 6f72 2066 696c 6520 7570 6c6f 6164 732c  or file uploads,
-00004f50: 206f 7220 6f74 6865 7220 6461 7461 2d69   or other data-i
-00004f60: 6e2c 2064 6174 612d 6f75 7420 6665 6174  n, data-out feat
-00004f70: 7572 6573 3f0a 2d20 446f 2079 6f75 2077  ures?.- Do you w
-00004f80: 616e 7420 746f 2073 6574 7570 2063 7573  ant to setup cus
-00004f90: 746f 6d20 6175 7468 6f72 697a 6174 696f  tom authorizatio
-00004fa0: 6e20 666f 7220 796f 7572 2041 5049 3f0a  n for your API?.
-00004fb0: 0a0a f09f 93a3 2047 6f74 2079 6f75 7220  ...... Got your 
-00004fc0: 6174 7465 6e74 696f 6e3f 205b 4a6f 696e  attention? [Join
-00004fd0: 2075 7320 6f6e 2053 6c61 636b 5d28 6874   us on Slack](ht
-00004fe0: 7470 733a 2f2f 6a69 6e61 2e61 692f 736c  tps://jina.ai/sl
-00004ff0: 6163 6b2f 2920 616e 6420 7765 2764 2062  ack/) and we'd b
-00005000: 6520 6861 7070 7920 746f 2068 656c 7020  e happy to help 
-00005010: 796f 7520 6f75 742e 0a0a 2d2d 2d0a 0a0a  you out...---...
-00005020: 2323 2320 606c 632d 7365 7276 6560 0a0a  ### `lc-serve`..
-00005030: 606c 632d 7365 7276 6560 2069 7320 6120  `lc-serve` is a 
-00005040: 434c 4920 746f 6f6c 2074 6861 7420 6865  CLI tool that he
-00005050: 6c70 7320 796f 7520 746f 2064 6570 6c6f  lps you to deplo
-00005060: 7920 796f 7572 2061 6765 6e74 7320 6f6e  y your agents on
-00005070: 204a 696e 6120 4149 2043 6c6f 7564 2e0a   Jina AI Cloud..
-00005080: 0a0a 7c20 4465 7363 7269 7074 696f 6e20  ..| Description 
-00005090: 7c20 436f 6d6d 616e 6420 7c20 0a7c 202d  | Command | .| -
-000050a0: 2d2d 207c 202d 2d2d 3a20 7c0a 7c20 4465  -- | ---: |.| De
-000050b0: 706c 6f79 2079 6f75 7220 6170 7020 6c6f  ploy your app lo
-000050c0: 6361 6c6c 7920 7c20 606c 632d 7365 7276  cally | `lc-serv
-000050d0: 6520 6465 706c 6f79 206c 6f63 616c 2061  e deploy local a
-000050e0: 7070 6020 7c0a 7c20 4465 706c 6f79 2079  pp` |.| Deploy y
-000050f0: 6f75 7220 6170 7020 6f6e 204a 696e 6120  our app on Jina 
-00005100: 4149 2043 6c6f 7564 207c 2060 6c63 2d73  AI Cloud | `lc-s
-00005110: 6572 7665 2064 6570 6c6f 7920 6a63 6c6f  erve deploy jclo
-00005120: 7564 2061 7070 6020 7c0a 7c20 5570 6461  ud app` |.| Upda
-00005130: 7465 2065 7869 7374 696e 6720 6170 7020  te existing app 
-00005140: 6f6e 204a 696e 6120 4149 2043 6c6f 7564  on Jina AI Cloud
-00005150: 207c 2060 6c63 2d73 6572 7665 2064 6570   | `lc-serve dep
-00005160: 6c6f 7920 6a63 6c6f 7564 2061 7070 202d  loy jcloud app -
-00005170: 2d61 7070 2d69 6420 3c61 7070 2d69 643e  -app-id <app-id>
-00005180: 6020 7c0a 7c20 4765 7420 6170 7020 7374  ` |.| Get app st
-00005190: 6174 7573 206f 6e20 4a69 6e61 2041 4920  atus on Jina AI 
-000051a0: 436c 6f75 6420 7c20 606c 632d 7365 7276  Cloud | `lc-serv
-000051b0: 6520 7374 6174 7573 203c 6170 702d 6964  e status <app-id
-000051c0: 3e60 207c 0a7c 204c 6973 7420 616c 6c20  >` |.| List all 
-000051d0: 6170 7073 206f 6e20 4a69 6e61 2041 4920  apps on Jina AI 
-000051e0: 436c 6f75 6420 7c20 606c 632d 7365 7276  Cloud | `lc-serv
-000051f0: 6520 6c69 7374 6020 7c0a 7c20 5265 6d6f  e list` |.| Remo
-00005200: 7665 2061 7070 206f 6e20 4a69 6e61 2041  ve app on Jina A
-00005210: 4920 436c 6f75 6420 7c20 606c 632d 7365  I Cloud | `lc-se
-00005220: 7276 6520 7265 6d6f 7665 203c 6170 702d  rve remove <app-
-00005230: 6964 3e60 207c 0a0a 0a2d 2d2d 0a0a 2323  id>` |...---..##
-00005240: 2320 4167 656e 7473 2050 6c61 7967 726f  # Agents Playgro
-00005250: 756e 6420 f09f 95b9 efb8 8ff0 9f8e aef0  und ............
-00005260: 9f8c 900a 0a5b 4c61 6e67 4368 6169 6e20  .....[LangChain 
-00005270: 6167 656e 7473 5d28 6874 7470 733a 2f2f  agents](https://
-00005280: 7079 7468 6f6e 2e6c 616e 6763 6861 696e  python.langchain
-00005290: 2e63 6f6d 2f65 6e2f 6c61 7465 7374 2f6d  .com/en/latest/m
-000052a0: 6f64 756c 6573 2f61 6765 6e74 732f 6765  odules/agents/ge
-000052b0: 7474 696e 675f 7374 6172 7465 642e 6874  tting_started.ht
-000052c0: 6d6c 2920 7573 6520 4c4c 4d73 2074 6f20  ml) use LLMs to 
-000052d0: 6465 7465 726d 696e 6520 7468 6520 6163  determine the ac
-000052e0: 7469 6f6e 7320 746f 2062 6520 7461 6b65  tions to be take
-000052f0: 6e20 696e 2077 6861 7420 6f72 6465 722e  n in what order.
-00005300: 2041 6e20 6163 7469 6f6e 2063 616e 2065   An action can e
-00005310: 6974 6865 7220 6265 2075 7369 6e67 2061  ither be using a
-00005320: 2074 6f6f 6c20 616e 6420 6f62 7365 7276   tool and observ
-00005330: 696e 6720 6974 7320 6f75 7470 7574 2c20  ing its output, 
-00005340: 6f72 2072 6574 7572 6e69 6e67 2074 6f20  or returning to 
-00005350: 7468 6520 7573 6572 2e20 5765 2776 6520  the user. We've 
-00005360: 686f 7374 6564 2061 202a 2a5b 5374 7265  hosted a **[Stre
-00005370: 616d 6c69 7420 506c 6179 6772 6f75 6e64  amlit Playground
-00005380: 5d28 6874 7470 733a 2f2f 6c61 6e67 6368  ](https://langch
-00005390: 6169 6e2e 776f 6c66 2e6a 696e 612e 6169  ain.wolf.jina.ai
-000053a0: 2f70 6c61 7967 726f 756e 642f 292a 2a20  /playground/)** 
-000053b0: 6f6e 204a 696e 6120 4149 2043 6c6f 7564  on Jina AI Cloud
-000053c0: 2074 6f20 696e 7465 7261 6374 2077 6974   to interact wit
-000053d0: 6820 7468 6520 6167 656e 7473 2c20 7768  h the agents, wh
-000053e0: 6963 6820 6163 6365 7074 7320 7769 7468  ich accepts with
-000053f0: 2066 6f6c 6c6f 7769 6e67 2069 6e70 7574   following input
-00005400: 733a 0a0a 2d20 2a2a 5b41 6765 6e74 2054  s:..- **[Agent T
-00005410: 7970 6573 5d28 6874 7470 733a 2f2f 7079  ypes](https://py
-00005420: 7468 6f6e 2e6c 616e 6763 6861 696e 2e63  thon.langchain.c
-00005430: 6f6d 2f65 6e2f 6c61 7465 7374 2f6d 6f64  om/en/latest/mod
-00005440: 756c 6573 2f61 6765 6e74 732f 6167 656e  ules/agents/agen
-00005450: 7473 2e68 746d 6c29 3a2a 2a20 4368 6f6f  ts.html):** Choo
-00005460: 7365 2066 726f 6d20 6469 6666 6572 656e  se from differen
-00005470: 7420 6167 656e 7420 7479 7065 7320 7468  t agent types th
-00005480: 6174 204c 616e 6763 6861 696e 2073 7570  at Langchain sup
-00005490: 706f 7274 732e 200a 0a2d 202a 2a5b 546f  ports. ..- **[To
-000054a0: 6f6c 735d 2868 7474 7073 3a2f 2f70 7974  ols](https://pyt
-000054b0: 686f 6e2e 6c61 6e67 6368 6169 6e2e 636f  hon.langchain.co
-000054c0: 6d2f 656e 2f6c 6174 6573 742f 6d6f 6475  m/en/latest/modu
-000054d0: 6c65 732f 6167 656e 7473 2f74 6f6f 6c73  les/agents/tools
-000054e0: 2e68 746d 6c29 3a2a 2a20 4368 6f6f 7365  .html):** Choose
-000054f0: 2066 726f 6d20 6469 6666 6572 656e 7420   from different 
-00005500: 746f 6f6c 7320 7468 6174 204c 616e 6763  tools that Langc
-00005510: 6861 696e 2073 7570 706f 7274 732e 2053  hain supports. S
-00005520: 6f6d 6520 746f 6f6c 7320 6d61 7920 7265  ome tools may re
-00005530: 7175 6972 6520 616e 2041 5049 2074 6f6b  quire an API tok
-00005540: 656e 206f 7220 6f74 6865 7220 7265 6c61  en or other rela
-00005550: 7465 6420 6172 6775 6d65 6e74 732e 0a0a  ted arguments...
-00005560: 546f 2075 7365 2074 6865 2070 6c61 7967  To use the playg
-00005570: 726f 756e 642c 2073 696d 706c 7920 7479  round, simply ty
-00005580: 7065 2079 6f75 7220 696e 7075 7420 696e  pe your input in
-00005590: 2074 6865 2074 6578 7420 626f 7820 7072   the text box pr
-000055a0: 6f76 6964 6564 2074 6f20 6765 7420 7468  ovided to get th
-000055b0: 6520 6167 656e 7427 7320 6f75 7470 7574  e agent's output
-000055c0: 2061 6e64 2063 6861 696e 206f 6620 7468   and chain of th
-000055d0: 6f75 6768 742e 2045 6e6a 6f79 2065 7870  ought. Enjoy exp
-000055e0: 6c6f 7269 6e67 204c 616e 6763 6861 696e  loring Langchain
-000055f0: 2773 2063 6170 6162 696c 6974 6965 7321  's capabilities!
-00005600: 2049 6e20 6164 6469 7469 6f6e 2074 6f20   In addition to 
-00005610: 7374 7265 616d 6c69 742c 2079 6f75 2063  streamlit, you c
-00005620: 616e 2061 6c73 6f20 7573 6520 6f75 7220  an also use our 
-00005630: 5245 5354 6675 6c20 4150 4973 206f 6e20  RESTful APIs on 
-00005640: 7468 6520 706c 6179 6772 6f75 6e64 2074  the playground t
-00005650: 6f20 696e 7465 7261 6374 2077 6974 6820  o interact with 
-00005660: 7468 6520 6167 656e 7473 2e20 0a0a 0a23  the agents. ...#
-00005670: 2323 205b 5a65 726f 2d73 686f 7420 5265  ## [Zero-shot Re
-00005680: 6163 7420 4465 7363 7269 7074 696f 6e20  act Description 
-00005690: 6167 656e 7420 7769 7468 2053 6572 7041  agent with SerpA
-000056a0: 5049 2061 6e64 2043 616c 6375 6c61 746f  PI and Calculato
-000056b0: 725d 2868 7474 7073 3a2f 2f70 7974 686f  r](https://pytho
-000056c0: 6e2e 6c61 6e67 6368 6169 6e2e 636f 6d2f  n.langchain.com/
-000056d0: 656e 2f6c 6174 6573 742f 6d6f 6475 6c65  en/latest/module
-000056e0: 732f 6167 656e 7473 2f67 6574 7469 6e67  s/agents/getting
-000056f0: 5f73 7461 7274 6564 2e68 746d 6c29 0a0a  _started.html)..
-00005700: 2323 2323 2053 7472 6561 6d6c 6974 2050  #### Streamlit P
-00005710: 6c61 7967 726f 756e 640a 0a21 5b53 7472  layground..![Str
-00005720: 6561 6d6c 6974 2050 6c61 7967 726f 756e  eamlit Playgroun
-00005730: 645d 282e 6769 7468 7562 2f69 6d61 6765  d](.github/image
-00005740: 732f 706c 6179 6772 6f75 6e64 5f6f 6e65  s/playground_one
-00005750: 2e67 6966 290a 0a23 2323 2320 5245 5354  .gif)..#### REST
-00005760: 6675 6c20 4150 490a 0a60 6060 6261 7368  ful API..```bash
-00005770: 0a65 7870 6f72 7420 4f50 454e 4149 5f41  .export OPENAI_A
-00005780: 5049 5f4b 4559 3d73 6b2d 2a2a 2a0a 6578  PI_KEY=sk-***.ex
-00005790: 706f 7274 2053 4552 5041 5049 5f41 5049  port SERPAPI_API
-000057a0: 5f4b 4559 3d2a 2a2a 0a0a 6375 726c 202d  _KEY=***..curl -
-000057b0: 7358 2050 4f53 5420 2768 7474 7073 3a2f  sX POST 'https:/
-000057c0: 2f6c 616e 6763 6861 696e 2e77 6f6c 662e  /langchain.wolf.
-000057d0: 6a69 6e61 2e61 692f 6170 692f 7275 6e27  jina.ai/api/run'
-000057e0: 205c 0a20 202d 4820 2761 6363 6570 743a   \.  -H 'accept:
-000057f0: 2061 7070 6c69 6361 7469 6f6e 2f6a 736f   application/jso
-00005800: 6e27 205c 0a20 202d 4820 2743 6f6e 7465  n' \.  -H 'Conte
-00005810: 6e74 2d54 7970 653a 2061 7070 6c69 6361  nt-Type: applica
-00005820: 7469 6f6e 2f6a 736f 6e27 205c 0a20 202d  tion/json' \.  -
-00005830: 2d64 6174 612d 7261 7720 277b 0a20 2020  -data-raw '{.   
-00005840: 2022 7465 7874 223a 2022 5768 6f20 6973   "text": "Who is
-00005850: 204c 656f 2044 6943 6170 7269 6f73 2067   Leo DiCaprios g
-00005860: 6972 6c66 7269 656e 643f 2057 6861 7420  irlfriend? What 
-00005870: 6973 2068 6572 2063 7572 7265 6e74 2061  is her current a
-00005880: 6765 2072 6169 7365 6420 746f 2074 6865  ge raised to the
-00005890: 2030 2e34 3320 706f 7765 723f 222c 0a20   0.43 power?",. 
-000058a0: 2020 2022 7061 7261 6d65 7465 7273 223a     "parameters":
-000058b0: 207b 0a20 2020 2020 2020 2022 746f 6f6c   {.        "tool
-000058c0: 7322 3a20 7b0a 2020 2020 2020 2020 2020  s": {.          
-000058d0: 2020 2274 6f6f 6c5f 6e61 6d65 7322 3a20    "tool_names": 
-000058e0: 5b22 7365 7270 6170 6922 2c20 226c 6c6d  ["serpapi", "llm
-000058f0: 2d6d 6174 6822 5d0a 2020 2020 2020 2020  -math"].        
-00005900: 7d2c 0a20 2020 2020 2020 2022 6167 656e  },.        "agen
-00005910: 7422 3a20 227a 6572 6f2d 7368 6f74 2d72  t": "zero-shot-r
-00005920: 6561 6374 2d64 6573 6372 6970 7469 6f6e  eact-description
-00005930: 222c 0a20 2020 2020 2020 2022 7665 7262  ",.        "verb
-00005940: 6f73 6522 3a20 7472 7565 0a20 2020 207d  ose": true.    }
-00005950: 2c0a 2020 2020 2265 6e76 7322 3a20 7b0a  ,.    "envs": {.
-00005960: 2020 2020 2020 2020 224f 5045 4e41 495f          "OPENAI_
-00005970: 4150 495f 4b45 5922 3a20 2227 2224 7b4f  API_KEY": "'"${O
-00005980: 5045 4e41 495f 4150 495f 4b45 597d 2227  PENAI_API_KEY}"'
-00005990: 222c 0a20 2020 2020 2020 2022 5345 5250  ",.        "SERP
-000059a0: 4150 495f 4150 495f 4b45 5922 3a20 2227  API_API_KEY": "'
-000059b0: 2224 7b53 4552 5041 5049 5f41 5049 5f4b  "${SERPAPI_API_K
-000059c0: 4559 7d22 2722 0a20 2020 207d 0a7d 2720  EY}"'".    }.}' 
-000059d0: 7c20 6a71 0a60 6060 200a 0a60 6060 6a73  | jq.``` ..```js
-000059e0: 6f6e 0a7b 0a20 2022 7265 7375 6c74 223a  on.{.  "result":
-000059f0: 2022 4361 6d69 6c61 204d 6f72 726f 6e65   "Camila Morrone
-00005a00: 2069 7320 4c65 6f20 4469 4361 7072 696f   is Leo DiCaprio
-00005a10: 2773 2067 6972 6c66 7269 656e 642c 2061  's girlfriend, a
-00005a20: 6e64 2068 6572 2063 7572 7265 6e74 2061  nd her current a
-00005a30: 6765 2072 6169 7365 6420 746f 2074 6865  ge raised to the
-00005a40: 2030 2e34 3320 706f 7765 7220 6973 2033   0.43 power is 3
-00005a50: 2e36 3236 3132 3630 3631 3135 3239 3532  .626126061152952
-00005a60: 372e 222c 0a20 2022 6368 6169 6e5f 6f66  7.",.  "chain_of
-00005a70: 5f74 686f 7567 6874 223a 2022 5c75 3030  _thought": "\u00
-00005a80: 3162 5b31 6d3e 2045 6e74 6572 696e 6720  1b[1m> Entering 
-00005a90: 6e65 7720 4167 656e 7445 7865 6375 746f  new AgentExecuto
-00005aa0: 7220 6368 6169 6e2e 2e2e 5c75 3030 3162  r chain...\u001b
-00005ab0: 5b30 6d5c 7530 3031 625b 3332 3b31 6d5c  [0m\u001b[32;1m\
-00005ac0: 7530 3031 625b 313b 336d 2049 206e 6565  u001b[1;3m I nee
-00005ad0: 6420 746f 2066 696e 6420 6f75 7420 7468  d to find out th
-00005ae0: 6520 6e61 6d65 206f 6620 4c65 6f27 7320  e name of Leo's 
-00005af0: 6769 726c 6672 6965 6e64 2061 6e64 2074  girlfriend and t
-00005b00: 6865 6e20 7573 6520 7468 6520 6361 6c63  hen use the calc
-00005b10: 756c 6174 6f72 2074 6f20 6361 6c63 756c  ulator to calcul
-00005b20: 6174 6520 6865 7220 6167 6520 746f 2074  ate her age to t
-00005b30: 6865 2030 2e34 3320 706f 7765 722e 4163  he 0.43 power.Ac
-00005b40: 7469 6f6e 3a20 5365 6172 6368 4163 7469  tion: SearchActi
-00005b50: 6f6e 2049 6e70 7574 3a20 4c65 6f20 4469  on Input: Leo Di
-00005b60: 4361 7072 696f 2067 6972 6c66 7269 656e  Caprio girlfrien
-00005b70: 645c 7530 3031 625b 306d 4f62 7365 7276  d\u001b[0mObserv
-00005b80: 6174 696f 6e3a 205c 7530 3031 625b 3336  ation: \u001b[36
-00005b90: 3b31 6d5c 7530 3031 625b 313b 336d 4469  ;1m\u001b[1;3mDi
-00005ba0: 4361 7072 696f 206d 6574 2061 6374 6f72  Caprio met actor
-00005bb0: 2043 616d 696c 6120 4d6f 7272 6f6e 6520   Camila Morrone 
-00005bc0: 696e 2044 6563 656d 6265 7220 3230 3137  in December 2017
-00005bd0: 2c20 7768 656e 2073 6865 2077 6173 2032  , when she was 2
-00005be0: 3020 616e 6420 6865 2077 6173 2034 332e  0 and he was 43.
-00005bf0: 2054 6865 7920 7765 7265 2073 706f 7474   They were spott
-00005c00: 6564 2061 7420 436f 6163 6865 6c6c 6120  ed at Coachella 
-00005c10: 616e 6420 7765 6e74 206f 6e20 6d75 6c74  and went on mult
-00005c20: 6970 6c65 2076 6163 6174 696f 6e73 2074  iple vacations t
-00005c30: 6f67 6574 6865 722e 2053 6f6d 6520 7265  ogether. Some re
-00005c40: 706f 7274 7320 7375 6767 6573 7465 6420  ports suggested 
-00005c50: 7468 6174 2044 6943 6170 7269 6f20 7761  that DiCaprio wa
-00005c60: 7320 7265 6164 7920 746f 2061 736b 204d  s ready to ask M
-00005c70: 6f72 726f 6e65 2074 6f20 6d61 7272 7920  orrone to marry 
-00005c80: 6869 6d2e 2054 6865 2063 6f75 706c 6520  him. The couple 
-00005c90: 6d61 6465 2074 6865 6972 2072 6564 2063  made their red c
-00005ca0: 6172 7065 7420 6465 6275 7420 6174 2074  arpet debut at t
-00005cb0: 6865 2032 3032 3020 4163 6164 656d 7920  he 2020 Academy 
-00005cc0: 4177 6172 6473 2e5c 7530 3031 625b 306d  Awards.\u001b[0m
-00005cd0: 5468 6f75 6768 743a 5c75 3030 3162 5b33  Thought:\u001b[3
-00005ce0: 323b 316d 5c75 3030 3162 5b31 3b33 6d20  2;1m\u001b[1;3m 
-00005cf0: 4920 6e65 6564 2074 6f20 7573 6520 7468  I need to use th
-00005d00: 6520 6361 6c63 756c 6174 6f72 2074 6f20  e calculator to 
-00005d10: 6361 6c63 756c 6174 6520 6865 7220 6167  calculate her ag
-00005d20: 6520 746f 2074 6865 2030 2e34 3320 706f  e to the 0.43 po
-00005d30: 7765 7241 6374 696f 6e3a 2043 616c 6375  werAction: Calcu
-00005d40: 6c61 746f 7241 6374 696f 6e20 496e 7075  latorAction Inpu
-00005d50: 743a 2032 305e 302e 3433 5c75 3030 3162  t: 20^0.43\u001b
-00005d60: 5b30 6d4f 6273 6572 7661 7469 6f6e 3a20  [0mObservation: 
-00005d70: 5c75 3030 3162 5b33 333b 316d 5c75 3030  \u001b[33;1m\u00
-00005d80: 3162 5b31 3b33 6d41 6e73 7765 723a 2033  1b[1;3mAnswer: 3
-00005d90: 2e36 3236 3132 3630 3631 3135 3239 3532  .626126061152952
-00005da0: 375c 7530 3031 625b 306d 5468 6f75 6768  7\u001b[0mThough
-00005db0: 743a 5c75 3030 3162 5b33 323b 316d 5c75  t:\u001b[32;1m\u
-00005dc0: 3030 3162 5b31 3b33 6d20 4920 6e6f 7720  001b[1;3m I now 
-00005dd0: 6b6e 6f77 2074 6865 2066 696e 616c 2061  know the final a
-00005de0: 6e73 7765 7246 696e 616c 2041 6e73 7765  nswerFinal Answe
-00005df0: 723a 2043 616d 696c 6120 4d6f 7272 6f6e  r: Camila Morron
-00005e00: 6520 6973 204c 656f 2044 6943 6170 7269  e is Leo DiCapri
-00005e10: 6f27 7320 6769 726c 6672 6965 6e64 2c20  o's girlfriend, 
-00005e20: 616e 6420 6865 7220 6375 7272 656e 7420  and her current 
-00005e30: 6167 6520 7261 6973 6564 2074 6f20 7468  age raised to th
-00005e40: 6520 302e 3433 2070 6f77 6572 2069 7320  e 0.43 power is 
-00005e50: 332e 3632 3631 3236 3036 3131 3532 3935  3.62612606115295
-00005e60: 3237 2e5c 7530 3031 625b 306d 5c75 3030  27.\u001b[0m\u00
-00005e70: 3162 5b31 6d3e 2046 696e 6973 6865 6420  1b[1m> Finished 
-00005e80: 6368 6169 6e2e 5c75 3030 3162 5b30 6d22  chain.\u001b[0m"
-00005e90: 0a7d 0a60 6060 0a0a 2323 2320 5b53 656c  .}.```..### [Sel
-00005ea0: 6620 4173 6b20 5769 7468 2053 6561 7263  f Ask With Searc
-00005eb0: 685d 2868 7474 7073 3a2f 2f70 7974 686f  h](https://pytho
-00005ec0: 6e2e 6c61 6e67 6368 6169 6e2e 636f 6d2f  n.langchain.com/
-00005ed0: 656e 2f6c 6174 6573 742f 6d6f 6475 6c65  en/latest/module
-00005ee0: 732f 6167 656e 7473 2f69 6d70 6c65 6d65  s/agents/impleme
-00005ef0: 6e74 6174 696f 6e73 2f73 656c 665f 6173  ntations/self_as
-00005f00: 6b5f 7769 7468 5f73 6561 7263 682e 6874  k_with_search.ht
-00005f10: 6d6c 290a 0a23 2323 2320 5374 7265 616d  ml)..#### Stream
-00005f20: 6c69 7420 506c 6179 6772 6f75 6e64 0a0a  lit Playground..
-00005f30: 215b 5374 7265 616d 6c69 7420 506c 6179  ![Streamlit Play
-00005f40: 6772 6f75 6e64 5d28 2e67 6974 6875 622f  ground](.github/
-00005f50: 696d 6167 6573 2f70 6c61 7967 726f 756e  images/playgroun
-00005f60: 645f 7477 6f2e 6769 6629 0a0a 2323 2323  d_two.gif)..####
-00005f70: 2052 4553 5466 756c 2041 5049 0a0a 6060   RESTful API..``
-00005f80: 6062 6173 680a 6578 706f 7274 204f 5045  `bash.export OPE
-00005f90: 4e41 495f 4150 495f 4b45 593d 736b 2d2a  NAI_API_KEY=sk-*
-00005fa0: 2a2a 0a65 7870 6f72 7420 5345 5250 4150  **.export SERPAP
-00005fb0: 495f 4150 495f 4b45 593d 2a2a 2a0a 0a63  I_API_KEY=***..c
-00005fc0: 7572 6c20 2d73 5820 504f 5354 2027 6874  url -sX POST 'ht
-00005fd0: 7470 733a 2f2f 6c61 6e67 6368 6169 6e2e  tps://langchain.
-00005fe0: 776f 6c66 2e6a 696e 612e 6169 2f61 7069  wolf.jina.ai/api
-00005ff0: 2f72 756e 2720 5c0a 2020 2d48 2027 6163  /run' \.  -H 'ac
-00006000: 6365 7074 3a20 6170 706c 6963 6174 696f  cept: applicatio
-00006010: 6e2f 6a73 6f6e 2720 5c0a 2020 2d48 2027  n/json' \.  -H '
-00006020: 436f 6e74 656e 742d 5479 7065 3a20 6170  Content-Type: ap
-00006030: 706c 6963 6174 696f 6e2f 6a73 6f6e 2720  plication/json' 
-00006040: 5c0a 2020 2d2d 6461 7461 2d72 6177 2027  \.  --data-raw '
-00006050: 7b0a 2020 2020 2274 6578 7422 3a20 2257  {.    "text": "W
-00006060: 6861 7420 6973 2074 6865 2068 6f6d 6574  hat is the homet
-00006070: 6f77 6e20 6f66 2074 6865 2072 6569 676e  own of the reign
-00006080: 696e 6720 6d65 6e73 2055 2e53 2e20 4f70  ing mens U.S. Op
-00006090: 656e 2063 6861 6d70 696f 6e3f 222c 0a20  en champion?",. 
-000060a0: 2020 2022 7061 7261 6d65 7465 7273 223a     "parameters":
-000060b0: 207b 0a20 2020 2020 2020 2022 746f 6f6c   {.        "tool
-000060c0: 7322 3a20 7b0a 2020 2020 2020 2020 2020  s": {.          
-000060d0: 2020 2274 6f6f 6c5f 6e61 6d65 7322 3a20    "tool_names": 
-000060e0: 5b22 7365 7270 6170 6922 5d0a 2020 2020  ["serpapi"].    
-000060f0: 2020 2020 7d2c 0a20 2020 2020 2020 2022      },.        "
-00006100: 6167 656e 7422 3a20 2273 656c 662d 6173  agent": "self-as
-00006110: 6b2d 7769 7468 2d73 6561 7263 6822 2c0a  k-with-search",.
-00006120: 2020 2020 2020 2020 2276 6572 626f 7365          "verbose
-00006130: 223a 2074 7275 650a 2020 2020 7d2c 0a20  ": true.    },. 
-00006140: 2020 2022 656e 7673 223a 207b 0a20 2020     "envs": {.   
-00006150: 2020 2020 2022 4f50 454e 4149 5f41 5049       "OPENAI_API
-00006160: 5f4b 4559 223a 2022 2722 247b 4f50 454e  _KEY": "'"${OPEN
-00006170: 4149 5f41 5049 5f4b 4559 7d22 2722 2c0a  AI_API_KEY}"'",.
-00006180: 2020 2020 2020 2020 2253 4552 5041 5049          "SERPAPI
-00006190: 5f41 5049 5f4b 4559 223a 2022 2722 247b  _API_KEY": "'"${
-000061a0: 5345 5250 4150 495f 4150 495f 4b45 597d  SERPAPI_API_KEY}
-000061b0: 2227 220a 2020 2020 7d0a 7d27 207c 206a  "'".    }.}' | j
-000061c0: 710a 6060 600a 0a60 6060 6a73 6f6e 0a7b  q.```..```json.{
-000061d0: 0a20 2022 7265 7375 6c74 223a 2022 456c  .  "result": "El
-000061e0: 2050 616c 6d61 722c 204d 7572 6369 612c   Palmar, Murcia,
-000061f0: 2053 7061 696e 222c 0a20 2022 6368 6169   Spain",.  "chai
-00006200: 6e5f 6f66 5f74 686f 7567 6874 223a 2022  n_of_thought": "
-00006210: 5c75 3030 3162 5b31 6d3e 2045 6e74 6572  \u001b[1m> Enter
-00006220: 696e 6720 6e65 7720 4167 656e 7445 7865  ing new AgentExe
-00006230: 6375 746f 7220 6368 6169 6e2e 2e2e 5c75  cutor chain...\u
-00006240: 3030 3162 5b30 6d5c 7530 3031 625b 3332  001b[0m\u001b[32
-00006250: 3b31 6d5c 7530 3031 625b 313b 336d 2059  ;1m\u001b[1;3m Y
-00006260: 6573 2e46 6f6c 6c6f 7720 7570 3a20 5768  es.Follow up: Wh
-00006270: 6f20 6973 2074 6865 2072 6569 676e 696e  o is the reignin
-00006280: 6720 6d65 6e73 2055 2e53 2e20 4f70 656e  g mens U.S. Open
-00006290: 2063 6861 6d70 696f 6e3f 5c75 3030 3162   champion?\u001b
-000062a0: 5b30 6d49 6e74 6572 6d65 6469 6174 6520  [0mIntermediate 
-000062b0: 616e 7377 6572 3a20 5c75 3030 3162 5b33  answer: \u001b[3
-000062c0: 363b 316d 5c75 3030 3162 5b31 3b33 6d43  6;1m\u001b[1;3mC
-000062d0: 6172 6c6f 7320 416c 6361 7261 7a20 4761  arlos Alcaraz Ga
-000062e0: 7266 6961 5c75 3030 3162 5b30 6d5c 7530  rfia\u001b[0m\u0
-000062f0: 3031 625b 3332 3b31 6d5c 7530 3031 625b  01b[32;1m\u001b[
-00006300: 313b 336d 466f 6c6c 6f77 2075 703a 2057  1;3mFollow up: W
-00006310: 6861 7420 6973 2043 6172 6c6f 7320 416c  hat is Carlos Al
-00006320: 6361 7261 7a20 4761 7266 6961 2773 2068  caraz Garfia's h
-00006330: 6f6d 6574 6f77 6e3f 5c75 3030 3162 5b30  ometown?\u001b[0
-00006340: 6d49 6e74 6572 6d65 6469 6174 6520 616e  mIntermediate an
-00006350: 7377 6572 3a20 5c75 3030 3162 5b33 363b  swer: \u001b[36;
-00006360: 316d 5c75 3030 3162 5b31 3b33 6d43 6172  1m\u001b[1;3mCar
-00006370: 6c6f 7320 416c 6361 7261 7a20 4761 7266  los Alcaraz Garf
-00006380: 6961 2077 6173 2062 6f72 6e20 6f6e 204d  ia was born on M
-00006390: 6179 2035 2c20 3230 3033 2c20 696e 2045  ay 5, 2003, in E
-000063a0: 6c20 5061 6c6d 6172 2c20 4d75 7263 6961  l Palmar, Murcia
-000063b0: 2c20 5370 6169 6e20 746f 2070 6172 656e  , Spain to paren
-000063c0: 7473 2043 6172 6c6f 7320 416c 6361 7261  ts Carlos Alcara
-000063d0: 7a20 476f 6e7a c3a1 6c65 7a20 616e 6420  z Gonz..lez and 
-000063e0: 5669 7267 696e 6961 2047 6172 6669 6120  Virginia Garfia 
-000063f0: 4573 6361 6e64 c3b3 6e2e 2048 6520 6861  Escand..n. He ha
-00006400: 7320 7468 7265 6520 7369 626c 696e 6773  s three siblings
-00006410: 2e5c 7530 3031 625b 306d 5c75 3030 3162  .\u001b[0m\u001b
-00006420: 5b33 323b 316d 5c75 3030 3162 5b31 3b33  [32;1m\u001b[1;3
-00006430: 6d53 6f20 7468 6520 6669 6e61 6c20 616e  mSo the final an
-00006440: 7377 6572 2069 733a 2045 6c20 5061 6c6d  swer is: El Palm
-00006450: 6172 2c20 4d75 7263 6961 2c20 5370 6169  ar, Murcia, Spai
-00006460: 6e5c 7530 3031 625b 306d 5c75 3030 3162  n\u001b[0m\u001b
-00006470: 5b31 6d3e 2046 696e 6973 6865 6420 6368  [1m> Finished ch
-00006480: 6169 6e2e 5c75 3030 3162 5b30 6d22 0a7d  ain.\u001b[0m".}
-00006490: 0a60 6060 0a0a 2d2d 2d0a 0a23 2320 4368  .```..---..## Ch
-000064a0: 6169 6e73 206f 6e20 4a69 6e61 20f0 9f93  ains on Jina ...
-000064b0: a6f0 9f9a 800a 0a5b 4368 6169 6e73 5d28  .......[Chains](
-000064c0: 6874 7470 733a 2f2f 7079 7468 6f6e 2e6c  https://python.l
-000064d0: 616e 6763 6861 696e 2e63 6f6d 2f65 6e2f  angchain.com/en/
-000064e0: 6c61 7465 7374 2f6d 6f64 756c 6573 2f63  latest/modules/c
-000064f0: 6861 696e 732f 6765 7474 696e 675f 7374  hains/getting_st
-00006500: 6172 7465 642e 6874 6d6c 2920 696e 204c  arted.html) in L
-00006510: 616e 6743 6861 696e 2061 6c6c 6f77 2075  angChain allow u
-00006520: 7365 7273 2074 6f20 636f 6d62 696e 6520  sers to combine 
-00006530: 636f 6d70 6f6e 656e 7473 2074 6f20 6372  components to cr
-00006540: 6561 7465 2061 2073 696e 676c 652c 2063  eate a single, c
-00006550: 6f68 6572 656e 7420 6170 706c 6963 6174  oherent applicat
-00006560: 696f 6e2e 2057 6974 6820 4a69 6e61 2c20  ion. With Jina, 
-00006570: 0a0a 2d20 596f 7520 6361 6e20 6578 706f  ..- You can expo
-00006580: 7365 2079 6f75 7220 6043 6861 696e 6020  se your `Chain` 
-00006590: 6173 2052 4553 5466 756c 2f67 5250 432f  as RESTful/gRPC/
-000065a0: 5765 6253 6f63 6b65 7420 4150 492e 0a2d  WebSocket API..-
-000065b0: 2045 6e61 626c 6520 6043 6861 696e 6073   Enable `Chain`s
-000065c0: 2074 6f20 6465 706c 6f79 2026 2073 6361   to deploy & sca
-000065d0: 6c65 2073 6570 6172 6174 656c 7920 6672  le separately fr
-000065e0: 6f6d 2074 6865 2072 6573 7420 6f66 2079  om the rest of y
-000065f0: 6f75 7220 6170 706c 6963 6174 696f 6e20  our application 
-00006600: 7769 7468 2074 6865 2068 656c 7020 6f66  with the help of
-00006610: 2045 7865 6375 746f 7273 2e0a 2d20 4465   Executors..- De
-00006620: 706c 6f79 2079 6f75 7220 6043 6861 696e  ploy your `Chain
-00006630: 6020 6f6e 204a 696e 6120 4149 2043 6c6f  ` on Jina AI Clo
-00006640: 7564 2061 6e64 2067 6574 2065 7863 6c75  ud and get exclu
-00006650: 7369 7665 2061 6363 6573 7320 746f 2041  sive access to A
-00006660: 6765 6e74 7320 6f6e 204a 696e 6120 4149  gents on Jina AI
-00006670: 2043 6c6f 7564 2028 636f 6d69 6e67 2073   Cloud (coming s
-00006680: 6f6f 6e29 0a0a 2323 2320 4578 616d 706c  oon)..### Exampl
-00006690: 6573 0a0a 7c20 4578 616d 706c 6520 7c20  es..| Example | 
-000066a0: 4c61 6e67 4368 6169 6e20 446f 6373 207c  LangChain Docs |
-000066b0: 2044 6573 6372 6970 7469 6f6e 207c 0a7c   Description |.|
-000066c0: 202d 2d2d 2d2d 2d2d 207c 202d 2d2d 2d2d   ------- | -----
-000066d0: 2d2d 2d2d 2d2d 207c 202d 2d2d 2d2d 2d2d  ------ | -------
-000066e0: 2d2d 2d2d 207c 0a7c 205b 4c4c 4d20 4368  ---- |.| [LLM Ch
-000066f0: 6169 6e5d 2865 7861 6d70 6c65 732f 6c6c  ain](examples/ll
-00006700: 6d5f 6368 6169 6e2e 6d64 2920 7c20 5b4c  m_chain.md) | [L
-00006710: 696e 6b5d 2868 7474 7073 3a2f 2f6c 616e  ink](https://lan
-00006720: 6763 6861 696e 2e72 6561 6474 6865 646f  gchain.readthedo
-00006730: 6373 2e69 6f2f 656e 2f6c 6174 6573 742f  cs.io/en/latest/
-00006740: 6d6f 6475 6c65 732f 6368 6169 6e73 2f67  modules/chains/g
-00006750: 6574 7469 6e67 5f73 7461 7274 6564 2e68  etting_started.h
-00006760: 746d 6c23 7175 6572 792d 616e 2d6c 6c6d  tml#query-an-llm
-00006770: 2d77 6974 682d 7468 652d 6c6c 6d63 6861  -with-the-llmcha
-00006780: 696e 2920 7c20 4578 706f 7365 2060 4368  in) | Expose `Ch
-00006790: 6169 6e60 2061 7320 5245 5354 6675 6c2f  ain` as RESTful/
-000067a0: 6752 5043 2f57 6562 536f 636b 6574 2041  gRPC/WebSocket A
-000067b0: 5049 206c 6f63 616c 6c79 207c 0a7c 205b  PI locally |.| [
-000067c0: 5369 6d70 6c65 2053 6571 7565 6e74 6961  Simple Sequentia
-000067d0: 6c20 4368 6169 6e5d 2865 7861 6d70 6c65  l Chain](example
-000067e0: 732f 7369 6d70 6c65 5f73 6571 7565 6e74  s/simple_sequent
-000067f0: 6961 6c5f 6368 6169 6e2e 6d64 2920 7c20  ial_chain.md) | 
-00006800: 5b4c 696e 6b5d 2868 7474 7073 3a2f 2f6c  [Link](https://l
-00006810: 616e 6763 6861 696e 2e72 6561 6474 6865  angchain.readthe
-00006820: 646f 6373 2e69 6f2f 656e 2f6c 6174 6573  docs.io/en/lates
-00006830: 742f 6d6f 6475 6c65 732f 6368 6169 6e73  t/modules/chains
-00006840: 2f67 656e 6572 6963 2f73 6571 7565 6e74  /generic/sequent
-00006850: 6961 6c5f 6368 6169 6e73 2e68 746d 6c23  ial_chains.html#
-00006860: 7369 6d70 6c65 7365 7175 656e 7469 616c  simplesequential
-00006870: 6368 6169 6e29 207c 2045 7870 6f73 6520  chain) | Expose 
-00006880: 6043 6861 696e 6020 6173 2052 4553 5466  `Chain` as RESTf
-00006890: 756c 2f67 5250 432f 5765 6253 6f63 6b65  ul/gRPC/WebSocke
-000068a0: 7420 4150 4920 6c6f 6361 6c6c 7920 7c0a  t API locally |.
-000068b0: 7c20 5b53 6571 7565 6e74 6961 6c20 4368  | [Sequential Ch
-000068c0: 6169 6e5d 2865 7861 6d70 6c65 732f 7365  ain](examples/se
-000068d0: 7175 656e 7469 616c 5f63 6861 696e 2e6d  quential_chain.m
-000068e0: 6429 207c 205b 4c69 6e6b 5d28 6874 7470  d) | [Link](http
-000068f0: 733a 2f2f 6c61 6e67 6368 6169 6e2e 7265  s://langchain.re
-00006900: 6164 7468 6564 6f63 732e 696f 2f65 6e2f  adthedocs.io/en/
-00006910: 6c61 7465 7374 2f6d 6f64 756c 6573 2f63  latest/modules/c
-00006920: 6861 696e 732f 6765 6e65 7269 632f 7365  hains/generic/se
-00006930: 7175 656e 7469 616c 5f63 6861 696e 732e  quential_chains.
-00006940: 6874 6d6c 2373 6571 7565 6e74 6961 6c2d  html#sequential-
-00006950: 6368 6169 6e29 207c 2045 7870 6f73 6520  chain) | Expose 
-00006960: 6043 6861 696e 6020 6173 2052 4553 5466  `Chain` as RESTf
-00006970: 756c 2f67 5250 432f 5765 6253 6f63 6b65  ul/gRPC/WebSocke
-00006980: 7420 4150 4920 6c6f 6361 6c6c 7920 7c0a  t API locally |.
-00006990: 7c20 5b4c 4c4d 204d 6174 6820 4368 6169  | [LLM Math Chai
-000069a0: 6e5d 2865 7861 6d70 6c65 732f 6c6c 6d5f  n](examples/llm_
-000069b0: 6d61 7468 2e6d 6429 207c 205b 4c69 6e6b  math.md) | [Link
-000069c0: 5d28 6874 7470 733a 2f2f 6c61 6e67 6368  ](https://langch
-000069d0: 6169 6e2e 7265 6164 7468 6564 6f63 732e  ain.readthedocs.
-000069e0: 696f 2f65 6e2f 6c61 7465 7374 2f6d 6f64  io/en/latest/mod
-000069f0: 756c 6573 2f63 6861 696e 732f 6578 616d  ules/chains/exam
-00006a00: 706c 6573 2f6c 6c6d 5f6d 6174 682e 6874  ples/llm_math.ht
-00006a10: 6d6c 2920 7c20 4578 706f 7365 2060 4368  ml) | Expose `Ch
-00006a20: 6169 6e60 2061 7320 5245 5354 6675 6c2f  ain` as RESTful/
-00006a30: 6752 5043 2f57 6562 536f 636b 6574 2041  gRPC/WebSocket A
-00006a40: 5049 206c 6f63 616c 6c79 207c 0a7c 205b  PI locally |.| [
-00006a50: 4c4c 4d20 5265 7175 6573 7473 2043 6861  LLM Requests Cha
-00006a60: 696e 5d28 6578 616d 706c 6573 2f6c 6c6d  in](examples/llm
-00006a70: 5f72 6571 7565 7374 735f 6368 6169 6e2e  _requests_chain.
-00006a80: 6d64 2920 7c20 5b4c 696e 6b5d 2868 7474  md) | [Link](htt
-00006a90: 7073 3a2f 2f6c 616e 6763 6861 696e 2e72  ps://langchain.r
-00006aa0: 6561 6474 6865 646f 6373 2e69 6f2f 656e  eadthedocs.io/en
-00006ab0: 2f6c 6174 6573 742f 6d6f 6475 6c65 732f  /latest/modules/
-00006ac0: 6368 6169 6e73 2f65 7861 6d70 6c65 732f  chains/examples/
-00006ad0: 6c6c 6d5f 7265 7175 6573 7473 2e68 746d  llm_requests.htm
-00006ae0: 6c29 207c 2045 7870 6f73 6520 6043 6861  l) | Expose `Cha
-00006af0: 696e 6020 6173 2052 4553 5466 756c 2f67  in` as RESTful/g
-00006b00: 5250 432f 5765 6253 6f63 6b65 7420 4150  RPC/WebSocket AP
-00006b10: 4920 6c6f 6361 6c6c 7920 7c0a 7c20 5b43  I locally |.| [C
-00006b20: 7573 746f 6d20 4368 6169 6e5d 2865 7861  ustom Chain](exa
-00006b30: 6d70 6c65 732f 6375 7374 6f6d 5f63 6861  mples/custom_cha
-00006b40: 696e 2e6d 6429 207c 205b 4c69 6e6b 5d28  in.md) | [Link](
-00006b50: 6874 7470 733a 2f2f 6c61 6e67 6368 6169  https://langchai
-00006b60: 6e2e 7265 6164 7468 6564 6f63 732e 696f  n.readthedocs.io
-00006b70: 2f65 6e2f 6c61 7465 7374 2f6d 6f64 756c  /en/latest/modul
-00006b80: 6573 2f63 6861 696e 732f 6765 7474 696e  es/chains/gettin
-00006b90: 675f 7374 6172 7465 642e 6874 6d6c 2363  g_started.html#c
-00006ba0: 7265 6174 652d 612d 6375 7374 6f6d 2d63  reate-a-custom-c
-00006bb0: 6861 696e 2d77 6974 682d 7468 652d 6368  hain-with-the-ch
-00006bc0: 6169 6e2d 636c 6173 7329 207c 2045 7870  ain-class) | Exp
-00006bd0: 6f73 6520 6043 6861 696e 6020 6173 2052  ose `Chain` as R
-00006be0: 4553 5466 756c 2f67 5250 432f 5765 6253  ESTful/gRPC/WebS
-00006bf0: 6f63 6b65 7420 4150 4920 6c6f 6361 6c6c  ocket API locall
-00006c00: 7920 7c0a 7c20 5b53 6571 7565 6e74 6961  y |.| [Sequentia
-00006c10: 6c20 4368 6169 6e73 5d28 6578 616d 706c  l Chains](exampl
-00006c20: 6573 2f73 6571 7565 6e74 6961 6c5f 6578  es/sequential_ex
-00006c30: 6563 7574 6f72 732e 6d64 2920 7c20 4e2f  ecutors.md) | N/
-00006c40: 4120 7c20 4275 696c 6420 2620 7363 616c  A | Build & scal
-00006c50: 6520 6043 6861 696e 7360 2069 6e20 7365  e `Chains` in se
-00006c60: 7061 7261 7465 2060 4578 6563 7574 6f72  parate `Executor
-00006c70: 6073 207c 0a7c 205b 4272 616e 6368 696e  `s |.| [Branchin
-00006c80: 6720 4368 6169 6e73 5d28 6578 616d 706c  g Chains](exampl
-00006c90: 6573 2f62 7261 6e63 6869 6e67 2e6d 6429  es/branching.md)
-00006ca0: 207c 204e 2f41 207c 2042 7261 6e63 6869   | N/A | Branchi
-00006cb0: 6e67 2060 4368 6169 6e73 6020 696e 2073  ng `Chains` in s
-00006cc0: 6570 6172 6174 6520 6045 7865 6375 746f  eparate `Executo
-00006cd0: 7260 7320 746f 2061 6c6c 6f77 2070 6172  r`s to allow par
-00006ce0: 616c 6c65 6c20 6578 6563 7574 696f 6e20  allel execution 
-00006cf0: 7c0a 0a23 2320 4672 6571 7565 6e74 6c79  |..## Frequently
-00006d00: 2041 736b 6564 2051 7565 7374 696f 6e73   Asked Questions
-00006d10: 0a0a 2d20 5b4d 7920 636c 6965 6e74 2074  ..- [My client t
-00006d20: 6861 7420 636f 6e6e 6563 7473 2074 6f20  hat connects to 
-00006d30: 7468 6520 4170 7020 6765 7473 2074 696d  the App gets tim
-00006d40: 6564 2d6f 7574 2c20 7768 6174 2073 686f  ed-out, what sho
-00006d50: 756c 6420 4920 646f 3f5d 2823 6d79 2d63  uld I do?](#my-c
-00006d60: 6c69 656e 742d 7468 6174 2d63 6f6e 6e65  lient-that-conne
-00006d70: 6374 732d 746f 2d74 6865 2d61 7070 2d67  cts-to-the-app-g
-00006d80: 6574 732d 7469 6d65 642d 6f75 742d 7768  ets-timed-out-wh
-00006d90: 6174 2d73 686f 756c 642d 492d 646f 290a  at-should-I-do).
-00006da0: 2d20 5b4a 436c 6f75 6420 6465 706c 6f79  - [JCloud deploy
-00006db0: 6d65 6e74 2066 6169 6c65 6420 6174 2070  ment failed at p
-00006dc0: 7573 6869 6e67 2069 6d61 6765 2074 6f20  ushing image to 
-00006dd0: 4a69 6e61 2048 7562 626c 652c 2077 6861  Jina Hubble, wha
-00006de0: 7420 7368 6f75 6c64 2049 2064 6f3f 5d28  t should I do?](
-00006df0: 236a 636c 6f75 642d 6465 706c 6f79 6d65  #jcloud-deployme
-00006e00: 6e74 2d66 6169 6c65 642d 6174 2d70 7573  nt-failed-at-pus
-00006e10: 6869 6e67 2d69 6d61 6765 2d74 6f2d 6a69  hing-image-to-ji
-00006e20: 6e61 2d68 7562 626c 652d 7768 6174 2d73  na-hubble-what-s
-00006e30: 686f 756c 642d 692d 6469 290a 0a23 2323  hould-i-di)..###
-00006e40: 204d 7920 636c 6965 6e74 2074 6861 7420   My client that 
-00006e50: 636f 6e6e 6563 7473 2074 6f20 7468 6520  connects to the 
-00006e60: 4170 7020 6765 7473 2074 696d 6564 2d6f  App gets timed-o
-00006e70: 7574 2c20 7768 6174 2073 686f 756c 6420  ut, what should 
-00006e80: 4920 646f 3f0a 0a49 6620 796f 7520 6d61  I do?..If you ma
-00006e90: 6b65 206c 6f6e 6720 4854 5450 2072 6571  ke long HTTP req
-00006ea0: 7565 7374 732c 2079 6f75 206d 6179 2065  uests, you may e
-00006eb0: 7870 6572 6965 6e63 6520 7469 6d65 6f75  xperience timeou
-00006ec0: 7473 2064 7565 2074 6f20 6c69 6d69 7461  ts due to limita
-00006ed0: 7469 6f6e 7320 696e 2074 6865 204f 5353  tions in the OSS
-00006ee0: 2077 6520 7573 6564 2069 6e20 606c 616e   we used in `lan
-00006ef0: 6763 6861 696e 2d73 6572 7665 602e 2057  gchain-serve`. W
-00006f00: 6869 6c65 2077 6520 6172 6520 776f 726b  hile we are work
-00006f10: 696e 6720 746f 2070 6572 6d61 6e65 6e74  ing to permanent
-00006f20: 6c79 2061 6464 7265 7373 2074 6869 7320  ly address this 
-00006f30: 6973 7375 652c 2077 6520 7265 636f 6d6d  issue, we recomm
-00006f40: 656e 6420 7573 696e 6720 4854 5450 2f31  end using HTTP/1
-00006f50: 2e31 2069 6e20 796f 7572 2063 6c69 656e  .1 in your clien
-00006f60: 7420 6173 2061 2074 656d 706f 7261 7279  t as a temporary
-00006f70: 2077 6f72 6b61 726f 756e 642e 0a0a 2323   workaround...##
-00006f80: 2320 4a43 6c6f 7564 2064 6570 6c6f 796d  # JCloud deploym
-00006f90: 656e 7420 6661 696c 6564 2061 7420 7075  ent failed at pu
-00006fa0: 7368 696e 6720 696d 6167 6520 746f 204a  shing image to J
-00006fb0: 696e 6120 4875 6262 6c65 2c20 7768 6174  ina Hubble, what
-00006fc0: 2073 686f 756c 6420 4920 646f 3f0a 0a50   should I do?..P
-00006fd0: 6c65 6173 6520 7573 6520 602d 2d76 6572  lease use `--ver
-00006fe0: 626f 7365 6020 616e 6420 7265 7472 7920  bose` and retry 
-00006ff0: 746f 2067 6574 206d 6f72 6520 696e 666f  to get more info
-00007000: 726d 6174 696f 6e2e 2049 6620 796f 7520  rmation. If you 
-00007010: 6172 6520 6f70 6572 6174 696e 6720 6f6e  are operating on
-00007020: 2063 6f6d 7075 7465 7220 7769 7468 2060   computer with `
-00007030: 6172 6d36 3460 2061 7263 682c 2070 6c65  arm64` arch, ple
-00007040: 6173 6520 7265 7472 7920 7769 7468 2060  ase retry with `
-00007050: 2d2d 706c 6174 666f 726d 206c 696e 7578  --platform linux
-00007060: 2f61 6d64 3634 6020 736f 2074 6865 2069  /amd64` so the i
-00007070: 6d61 6765 2063 616e 2062 6520 6275 696c  mage can be buil
-00007080: 7420 636f 7272 6563 746c 792e 0a0a 0a    t correctly....
+00004040: 9480 e294 80e2 95af 0a60 6060 0a0a 4c65  .........```..Le
+00004050: 7427 7320 6f70 656e 2074 6865 2053 7761  t's open the Swa
+00004060: 6767 6572 2055 4920 746f 2074 6573 7420  gger UI to test 
+00004070: 6f75 7220 4150 4920 6f6e 204a 696e 6120  our API on Jina 
+00004080: 4149 2043 6c6f 7564 2e20 5769 7468 2060  AI Cloud. With `
+00004090: 5472 7920 6974 206f 7574 6020 6275 7474  Try it out` butt
+000040a0: 6f6e 2c20 7765 2063 616e 2074 6573 7420  on, we can test 
+000040b0: 6f75 7220 4150 4920 7769 7468 2064 6966  our API with dif
+000040c0: 6665 7265 6e74 2069 6e70 7574 732e 0a0a  ferent inputs...
+000040d0: 3c64 6574 6169 6c73 3e0a 3c73 756d 6d61  <details>.<summa
+000040e0: 7279 3e53 686f 7720 5377 6167 6765 7220  ry>Show Swagger 
+000040f0: 5549 3c2f 7375 6d6d 6172 793e 0a0a 3c70  UI</summary>..<p
+00004100: 2066 6c6f 6174 3d22 6365 6e74 6572 223e   float="center">
+00004110: 0a20 203c 696d 6720 7372 633d 222e 6769  .  <img src=".gi
+00004120: 7468 7562 2f69 6d61 6765 732f 6a63 6c6f  thub/images/jclo
+00004130: 7564 2d73 7761 6767 6572 2d75 692e 706e  ud-swagger-ui.pn
+00004140: 6722 2077 6964 7468 3d22 3430 3022 202f  g" width="400" /
+00004150: 3e0a 2020 3c69 6d67 2073 7263 3d22 2e67  >.  <img src=".g
+00004160: 6974 6875 622f 696d 6167 6573 2f6a 636c  ithub/images/jcl
+00004170: 6f75 642d 6f70 656e 6170 692e 706e 6722  oud-openapi.png"
+00004180: 2077 6964 7468 3d22 3330 3022 202f 3e0a   width="300" />.
+00004190: 3c2f 703e 0a0a 3c2f 6465 7461 696c 733e  </p>..</details>
+000041a0: 0a0a 0a4c 6574 2773 2074 6573 7420 7468  ...Let's test th
+000041b0: 6520 4150 4920 6f6e 204a 436c 6f75 6420  e API on JCloud 
+000041c0: 7769 7468 2060 486f 7720 6d61 6e79 2070  with `How many p
+000041d0: 656f 706c 6520 6c69 7665 2069 6e20 6361  eople live in ca
+000041e0: 6e61 6461 2061 7320 6f66 2032 3032 333f  nada as of 2023?
+000041f0: 6020 696e 7075 7420 7769 7468 2061 2063  ` input with a c
+00004200: 5552 4c20 636f 6d6d 616e 6420 2852 6570  URL command (Rep
+00004210: 6c61 6365 2074 6865 2048 6f73 746e 616d  lace the Hostnam
+00004220: 6520 7769 7468 2079 6f75 7220 6f77 6e20  e with your own 
+00004230: 686f 7374 6e61 6d65 293a 0a0a 6060 6062  hostname):..```b
+00004240: 6173 680a 6375 726c 202d 5820 2750 4f53  ash.curl -X 'POS
+00004250: 5427 205c 0a20 2027 6874 7470 733a 2f2f  T' \.  'https://
+00004260: 6c61 6e67 6368 6169 6e2d 6565 3461 6566  langchain-ee4aef
+00004270: 3537 6439 2d68 7474 702e 776f 6c66 2e6a  57d9-http.wolf.j
+00004280: 696e 612e 6169 2f61 736b 2720 5c0a 2020  ina.ai/ask' \.  
+00004290: 2d48 2027 6163 6365 7074 3a20 6170 706c  -H 'accept: appl
+000042a0: 6963 6174 696f 6e2f 6a73 6f6e 2720 5c0a  ication/json' \.
+000042b0: 2020 2d48 2027 436f 6e74 656e 742d 5479    -H 'Content-Ty
+000042c0: 7065 3a20 6170 706c 6963 6174 696f 6e2f  pe: application/
+000042d0: 6a73 6f6e 2720 5c0a 2020 2d64 2027 7b0a  json' \.  -d '{.
+000042e0: 2020 2269 6e70 7574 223a 2022 486f 7720    "input": "How 
+000042f0: 6d61 6e79 2070 656f 706c 6520 6c69 7665  many people live
+00004300: 2069 6e20 6361 6e61 6461 2061 7320 6f66   in canada as of
+00004310: 2032 3032 333f 222c 0a20 2022 656e 7673   2023?",.  "envs
+00004320: 223a 207b 0a20 2020 2022 4f50 454e 4149  ": {.    "OPENAI
+00004330: 5f41 5049 5f4b 4559 223a 2022 2722 247b  _API_KEY": "'"${
+00004340: 4f50 454e 4149 5f41 5049 5f4b 4559 7d22  OPENAI_API_KEY}"
+00004350: 2722 2c0a 2020 2020 2253 4552 5041 5049  '",.    "SERPAPI
+00004360: 5f41 5049 5f4b 4559 223a 2022 2722 247b  _API_KEY": "'"${
+00004370: 5345 5250 4150 495f 4150 495f 4b45 597d  SERPAPI_API_KEY}
+00004380: 2227 220a 2020 7d0a 7d27 0a60 6060 0a0a  "'".  }.}'.```..
+00004390: 6060 606a 736f 6e0a 7b0a 2020 2272 6573  ```json.{.  "res
+000043a0: 756c 7422 3a20 2241 7272 722c 2074 6865  ult": "Arrr, the
+000043b0: 7265 2062 6520 3338 2c36 3435 2c36 3730  re be 38,645,670
+000043c0: 2070 656f 706c 6520 6c69 7669 6e27 2069   people livin' i
+000043d0: 6e20 4361 6e61 6461 2061 7320 6f66 2032  n Canada as of 2
+000043e0: 3032 3321 222c 0a20 2022 6572 726f 7222  023!",.  "error"
+000043f0: 3a20 2222 2c0a 2020 2273 7464 6f75 7422  : "",.  "stdout"
+00004400: 3a20 2241 6e73 7765 7220 7468 6520 666f  : "Answer the fo
+00004410: 6c6c 6f77 696e 6720 7175 6573 7469 6f6e  llowing question
+00004420: 7320 6173 2062 6573 7420 796f 7520 6361  s as best you ca
+00004430: 6e2c 2062 7574 2073 7065 616b 696e 6720  n, but speaking 
+00004440: 6173 2061 2070 6972 6174 6520 6d69 6768  as a pirate migh
+00004450: 7420 7370 6561 6b2e 2059 6f75 2068 6176  t speak. You hav
+00004460: 6520 6163 6365 7373 2074 6f20 7468 6520  e access to the 
+00004470: 666f 6c6c 6f77 696e 6720 746f 6f6c 733a  following tools:
+00004480: 5c6e 5c6e 5365 6172 6368 3a20 7573 6566  \n\nSearch: usef
+00004490: 756c 2066 6f72 2077 6865 6e20 796f 7520  ul for when you 
+000044a0: 6e65 6564 2074 6f20 616e 7377 6572 2071  need to answer q
+000044b0: 7565 7374 696f 6e73 2061 626f 7574 2063  uestions about c
+000044c0: 7572 7265 6e74 2065 7665 6e74 735c 6e5c  urrent events\n\
+000044d0: 6e55 7365 2074 6865 2066 6f6c 6c6f 7769  nUse the followi
+000044e0: 6e67 2066 6f72 6d61 743a 5c6e 5c6e 5175  ng format:\n\nQu
+000044f0: 6573 7469 6f6e 3a20 7468 6520 696e 7075  estion: the inpu
+00004500: 7420 7175 6573 7469 6f6e 2079 6f75 206d  t question you m
+00004510: 7573 7420 616e 7377 6572 5c6e 5468 6f75  ust answer\nThou
+00004520: 6768 743a 2079 6f75 2073 686f 756c 6420  ght: you should 
+00004530: 616c 7761 7973 2074 6869 6e6b 2061 626f  always think abo
+00004540: 7574 2077 6861 7420 746f 2064 6f5c 6e41  ut what to do\nA
+00004550: 6374 696f 6e3a 2074 6865 2061 6374 696f  ction: the actio
+00004560: 6e20 746f 2074 616b 652c 2073 686f 756c  n to take, shoul
+00004570: 6420 6265 206f 6e65 206f 6620 5b53 6561  d be one of [Sea
+00004580: 7263 685d 5c6e 4163 7469 6f6e 2049 6e70  rch]\nAction Inp
+00004590: 7574 3a20 7468 6520 696e 7075 7420 746f  ut: the input to
+000045a0: 2074 6865 2061 6374 696f 6e5c 6e4f 6273   the action\nObs
+000045b0: 6572 7661 7469 6f6e 3a20 7468 6520 7265  ervation: the re
+000045c0: 7375 6c74 206f 6620 7468 6520 6163 7469  sult of the acti
+000045d0: 6f6e 5c6e 2e2e 2e20 2874 6869 7320 5468  on\n... (this Th
+000045e0: 6f75 6768 742f 4163 7469 6f6e 2f41 6374  ought/Action/Act
+000045f0: 696f 6e20 496e 7075 742f 4f62 7365 7276  ion Input/Observ
+00004600: 6174 696f 6e20 6361 6e20 7265 7065 6174  ation can repeat
+00004610: 204e 2074 696d 6573 295c 6e54 686f 7567   N times)\nThoug
+00004620: 6874 3a20 4920 6e6f 7720 6b6e 6f77 2074  ht: I now know t
+00004630: 6865 2066 696e 616c 2061 6e73 7765 725c  he final answer\
+00004640: 6e46 696e 616c 2041 6e73 7765 723a 2074  nFinal Answer: t
+00004650: 6865 2066 696e 616c 2061 6e73 7765 7220  he final answer 
+00004660: 746f 2074 6865 206f 7269 6769 6e61 6c20  to the original 
+00004670: 696e 7075 7420 7175 6573 7469 6f6e 5c6e  input question\n
+00004680: 5c6e 4265 6769 6e21 2052 656d 656d 6265  \nBegin! Remembe
+00004690: 7220 746f 2073 7065 616b 2061 7320 6120  r to speak as a 
+000046a0: 7069 7261 7465 2077 6865 6e20 6769 7669  pirate when givi
+000046b0: 6e67 2079 6f75 7220 6669 6e61 6c20 616e  ng your final an
+000046c0: 7377 6572 2e20 5573 6520 6c6f 7473 206f  swer. Use lots o
+000046d0: 6620 5c22 4172 6773 5c22 5c6e 5c6e 2020  f \"Args\"\n\n  
+000046e0: 2020 5175 6573 7469 6f6e 3a20 7b69 6e70    Question: {inp
+000046f0: 7574 7d5c 6e20 2020 207b 6167 656e 745f  ut}\n    {agent_
+00004700: 7363 7261 7463 6870 6164 7d5c 6e5c 6e5c  scratchpad}\n\n\
+00004710: 6e5c 7530 3031 625b 316d 3e20 456e 7465  n\u001b[1m> Ente
+00004720: 7269 6e67 206e 6577 2041 6765 6e74 4578  ring new AgentEx
+00004730: 6563 7574 6f72 2063 6861 696e 2e2e 2e5c  ecutor chain...\
+00004740: 7530 3031 625b 306d 5c6e 5c75 3030 3162  u001b[0m\n\u001b
+00004750: 5b33 323b 316d 5c75 3030 3162 5b31 3b33  [32;1m\u001b[1;3
+00004760: 6d5c 6e54 686f 7567 6874 3a20 4920 6e65  m\nThought: I ne
+00004770: 6564 2074 6f20 6669 6e64 206f 7574 2068  ed to find out h
+00004780: 6f77 206d 616e 7920 7065 6f70 6c65 206c  ow many people l
+00004790: 6976 6520 696e 2043 616e 6164 615c 6e41  ive in Canada\nA
+000047a0: 6374 696f 6e3a 2053 6561 7263 685c 6e41  ction: Search\nA
+000047b0: 6374 696f 6e20 496e 7075 743a 2048 6f77  ction Input: How
+000047c0: 206d 616e 7920 7065 6f70 6c65 206c 6976   many people liv
+000047d0: 6520 696e 2043 616e 6164 6120 6173 206f  e in Canada as o
+000047e0: 6620 3230 3233 5c75 3030 3162 5b30 6d5c  f 2023\u001b[0m\
+000047f0: 6e4f 6273 6572 7661 7469 6f6e 3a20 5c75  nObservation: \u
+00004800: 3030 3162 5b33 363b 316d 5c75 3030 3162  001b[36;1m\u001b
+00004810: 5b31 3b33 6d54 6865 2063 7572 7265 6e74  [1;3mThe current
+00004820: 2070 6f70 756c 6174 696f 6e20 6f66 2043   population of C
+00004830: 616e 6164 6120 6973 2033 382c 3634 352c  anada is 38,645,
+00004840: 3637 3020 6173 206f 6620 5765 646e 6573  670 as of Wednes
+00004850: 6461 792c 204d 6172 6368 2032 392c 2032  day, March 29, 2
+00004860: 3032 332c 2062 6173 6564 206f 6e20 576f  023, based on Wo
+00004870: 726c 646f 6d65 7465 7220 656c 6162 6f72  rldometer elabor
+00004880: 6174 696f 6e20 6f66 2074 6865 206c 6174  ation of the lat
+00004890: 6573 7420 556e 6974 6564 204e 6174 696f  est United Natio
+000048a0: 6e73 2064 6174 612e 5c75 3030 3162 5b30  ns data.\u001b[0
+000048b0: 6d5c 6e54 686f 7567 6874 3a5c 7530 3031  m\nThought:\u001
+000048c0: 625b 3332 3b31 6d5c 7530 3031 625b 313b  b[32;1m\u001b[1;
+000048d0: 336d 2049 206e 6f77 206b 6e6f 7720 7468  3m I now know th
+000048e0: 6520 6669 6e61 6c20 616e 7377 6572 5c6e  e final answer\n
+000048f0: 4669 6e61 6c20 416e 7377 6572 3a20 4172  Final Answer: Ar
+00004900: 7272 2c20 7468 6572 6520 6265 2033 382c  rr, there be 38,
+00004910: 3634 352c 3637 3020 7065 6f70 6c65 206c  645,670 people l
+00004920: 6976 696e 2720 696e 2043 616e 6164 6120  ivin' in Canada 
+00004930: 6173 206f 6620 3230 3233 215c 7530 3031  as of 2023!\u001
+00004940: 625b 306d 5c6e 5c6e 5c75 3030 3162 5b31  b[0m\n\n\u001b[1
+00004950: 6d3e 2046 696e 6973 6865 6420 6368 6169  m> Finished chai
+00004960: 6e2e 5c75 3030 3162 5b30 6d22 0a7d 0a60  n.\u001b[0m".}.`
+00004970: 6060 0a0a 2323 2323 2320 5768 6174 2068  ``..##### What h
+00004980: 6170 7065 6e65 643f 0a0a 2d20 496e 2061  appened?..- In a
+00004990: 206d 6174 7465 7220 6f66 2066 6577 2073   matter of few s
+000049a0: 6563 6f6e 6473 2c20 7765 2776 6520 6465  econds, we've de
+000049b0: 706c 6f79 6564 206f 7572 2041 5049 206f  ployed our API o
+000049c0: 6e20 4a69 6e61 2041 4920 436c 6f75 6420  n Jina AI Cloud 
+000049d0: f09f 8e89 0a2d 2054 6865 2041 5049 2069  .....- The API i
+000049e0: 7320 7365 7276 6572 6c65 7373 2061 6e64  s serverless and
+000049f0: 2073 6361 6c61 626c 652c 2073 6f20 7765   scalable, so we
+00004a00: 2063 616e 2073 6361 6c65 2075 7020 7468   can scale up th
+00004a10: 6520 4150 4920 746f 2068 616e 646c 6520  e API to handle 
+00004a20: 6d6f 7265 2072 6571 7565 7374 732e 200a  more requests. .
+00004a30: 2d20 596f 7520 6d69 6768 7420 6f62 7365  - You might obse
+00004a40: 7276 6520 6120 6465 6c61 7920 696e 2074  rve a delay in t
+00004a50: 6865 2066 6972 7374 2072 6571 7565 7374  he first request
+00004a60: 2c20 7468 6174 2773 2064 7565 2074 6f20  , that's due to 
+00004a70: 7468 6520 7761 726d 2d75 7020 7469 6d65  the warm-up time
+00004a80: 206f 6620 7468 6520 4150 492e 2053 7562   of the API. Sub
+00004a90: 7365 7175 656e 7420 7265 7175 6573 7473  sequent requests
+00004aa0: 2077 696c 6c20 6265 2066 6173 7465 722e   will be faster.
+00004ab0: 0a2d 2054 6865 2041 5049 2069 6e63 6c75  .- The API inclu
+00004ac0: 6465 7320 6120 5377 6167 6765 7220 5549  des a Swagger UI
+00004ad0: 2061 6e64 2074 6865 204f 7065 6e41 5049   and the OpenAPI
+00004ae0: 2073 7065 6369 6669 6361 7469 6f6e 2c20   specification, 
+00004af0: 736f 2069 7420 6361 6e20 6265 2065 6173  so it can be eas
+00004b00: 696c 7920 696e 7465 6772 6174 6564 2077  ily integrated w
+00004b10: 6974 6820 6f74 6865 7220 7365 7276 6963  ith other servic
+00004b20: 6573 2e20 0a2d 204e 6f77 2c20 6f74 6865  es. .- Now, othe
+00004b30: 7220 6167 656e 7473 2063 616e 2069 6e74  r agents can int
+00004b40: 6567 7261 7465 2077 6974 6820 796f 7572  egrate with your
+00004b50: 2061 6765 6e74 7320 6f6e 204a 696e 6120   agents on Jina 
+00004b60: 4149 2043 6c6f 7564 2074 6861 6e6b 7320  AI Cloud thanks 
+00004b70: 746f 2074 6865 205b 4f70 656e 4150 4920  to the [OpenAPI 
+00004b80: 4167 656e 745d 2868 7474 7073 3a2f 2f70  Agent](https://p
+00004b90: 7974 686f 6e2e 6c61 6e67 6368 6169 6e2e  ython.langchain.
+00004ba0: 636f 6d2f 656e 2f6c 6174 6573 742f 6d6f  com/en/latest/mo
+00004bb0: 6475 6c65 732f 6167 656e 7473 2f74 6f6f  dules/agents/too
+00004bc0: 6c6b 6974 732f 6578 616d 706c 6573 2f6f  lkits/examples/o
+00004bd0: 7065 6e61 7069 2e68 746d 6c29 20f0 9f92  penapi.html) ...
+00004be0: a10a 0a0a 0a2d 2d2d 0a0a 2323 2323 2052  .....---..#### R
+00004bf0: 6561 6368 206f 7574 2074 6f20 7573 20f0  each out to us .
+00004c00: 9f93 9e0a 0a2d 2053 6572 7665 726c 6573  .....- Serverles
+00004c10: 7320 6973 206e 6f74 2079 6f75 7220 7468  s is not your th
+00004c20: 696e 673f 0a2d 2044 6f20 796f 7520 7761  ing?.- Do you wa
+00004c30: 6e74 206c 6172 6765 7220 696e 7374 616e  nt larger instan
+00004c40: 6365 7320 666f 7220 796f 7572 2041 5049  ces for your API
+00004c50: 3f0a 2d20 4c6f 6f6b 696e 6720 666f 7220  ?.- Looking for 
+00004c60: 6669 6c65 2075 706c 6f61 6473 2c20 6f72  file uploads, or
+00004c70: 206f 7468 6572 2064 6174 612d 696e 2c20   other data-in, 
+00004c80: 6461 7461 2d6f 7574 2066 6561 7475 7265  data-out feature
+00004c90: 733f 0a2d 2044 6f20 796f 7520 7761 6e74  s?.- Do you want
+00004ca0: 2074 6f20 7365 7475 7020 6375 7374 6f6d   to setup custom
+00004cb0: 2061 7574 686f 7269 7a61 7469 6f6e 2066   authorization f
+00004cc0: 6f72 2079 6f75 7220 4150 493f 0a0a 0af0  or your API?....
+00004cd0: 9f93 a320 476f 7420 796f 7572 2061 7474  ... Got your att
+00004ce0: 656e 7469 6f6e 3f20 5b4a 6f69 6e20 7573  ention? [Join us
+00004cf0: 206f 6e20 536c 6163 6b5d 2868 7474 7073   on Slack](https
+00004d00: 3a2f 2f6a 696e 612e 6169 2f73 6c61 636b  ://jina.ai/slack
+00004d10: 2f29 2061 6e64 2077 6527 6420 6265 2068  /) and we'd be h
+00004d20: 6170 7079 2074 6f20 6865 6c70 2079 6f75  appy to help you
+00004d30: 206f 7574 2e0a 0a2d 2d2d 0a0a 0a23 2323   out...---...###
+00004d40: 2060 6c63 2d73 6572 7665 600a 0a60 6c63   `lc-serve`..`lc
+00004d50: 2d73 6572 7665 6020 6973 2061 2043 4c49  -serve` is a CLI
+00004d60: 2074 6f6f 6c20 7468 6174 2068 656c 7073   tool that helps
+00004d70: 2079 6f75 2074 6f20 6465 706c 6f79 2079   you to deploy y
+00004d80: 6f75 7220 6167 656e 7473 206f 6e20 4a69  our agents on Ji
+00004d90: 6e61 2041 4920 436c 6f75 642e 0a0a 0a7c  na AI Cloud....|
+00004da0: 2044 6573 6372 6970 7469 6f6e 207c 2043   Description | C
+00004db0: 6f6d 6d61 6e64 207c 200a 7c20 2d2d 2d20  ommand | .| --- 
+00004dc0: 7c20 2d2d 2d3a 207c 0a7c 2044 6570 6c6f  | ---: |.| Deplo
+00004dd0: 7920 796f 7572 2061 7070 206c 6f63 616c  y your app local
+00004de0: 6c79 207c 2060 6c63 2d73 6572 7665 2064  ly | `lc-serve d
+00004df0: 6570 6c6f 7920 6c6f 6361 6c20 6170 7060  eploy local app`
+00004e00: 207c 0a7c 2044 6570 6c6f 7920 796f 7572   |.| Deploy your
+00004e10: 2061 7070 206f 6e20 4a69 6e61 2041 4920   app on Jina AI 
+00004e20: 436c 6f75 6420 7c20 606c 632d 7365 7276  Cloud | `lc-serv
+00004e30: 6520 6465 706c 6f79 206a 636c 6f75 6420  e deploy jcloud 
+00004e40: 6170 7060 207c 0a7c 2055 7064 6174 6520  app` |.| Update 
+00004e50: 6578 6973 7469 6e67 2061 7070 206f 6e20  existing app on 
+00004e60: 4a69 6e61 2041 4920 436c 6f75 6420 7c20  Jina AI Cloud | 
+00004e70: 606c 632d 7365 7276 6520 6465 706c 6f79  `lc-serve deploy
+00004e80: 206a 636c 6f75 6420 6170 7020 2d2d 6170   jcloud app --ap
+00004e90: 702d 6964 203c 6170 702d 6964 3e60 207c  p-id <app-id>` |
+00004ea0: 0a7c 2047 6574 2061 7070 2073 7461 7475  .| Get app statu
+00004eb0: 7320 6f6e 204a 696e 6120 4149 2043 6c6f  s on Jina AI Clo
+00004ec0: 7564 207c 2060 6c63 2d73 6572 7665 2073  ud | `lc-serve s
+00004ed0: 7461 7475 7320 3c61 7070 2d69 643e 6020  tatus <app-id>` 
+00004ee0: 7c0a 7c20 4c69 7374 2061 6c6c 2061 7070  |.| List all app
+00004ef0: 7320 6f6e 204a 696e 6120 4149 2043 6c6f  s on Jina AI Clo
+00004f00: 7564 207c 2060 6c63 2d73 6572 7665 206c  ud | `lc-serve l
+00004f10: 6973 7460 207c 0a7c 2052 656d 6f76 6520  ist` |.| Remove 
+00004f20: 6170 7020 6f6e 204a 696e 6120 4149 2043  app on Jina AI C
+00004f30: 6c6f 7564 207c 2060 6c63 2d73 6572 7665  loud | `lc-serve
+00004f40: 2072 656d 6f76 6520 3c61 7070 2d69 643e   remove <app-id>
+00004f50: 6020 7c0a 0a0a 2d2d 2d0a 0a23 2323 2041  ` |...---..### A
+00004f60: 6765 6e74 7320 506c 6179 6772 6f75 6e64  gents Playground
+00004f70: 20f0 9f95 b9ef b88f f09f 8eae f09f 8c90   ...............
+00004f80: 0a0a 5b4c 616e 6743 6861 696e 2061 6765  ..[LangChain age
+00004f90: 6e74 735d 2868 7474 7073 3a2f 2f70 7974  nts](https://pyt
+00004fa0: 686f 6e2e 6c61 6e67 6368 6169 6e2e 636f  hon.langchain.co
+00004fb0: 6d2f 656e 2f6c 6174 6573 742f 6d6f 6475  m/en/latest/modu
+00004fc0: 6c65 732f 6167 656e 7473 2f67 6574 7469  les/agents/getti
+00004fd0: 6e67 5f73 7461 7274 6564 2e68 746d 6c29  ng_started.html)
+00004fe0: 2075 7365 204c 4c4d 7320 746f 2064 6574   use LLMs to det
+00004ff0: 6572 6d69 6e65 2074 6865 2061 6374 696f  ermine the actio
+00005000: 6e73 2074 6f20 6265 2074 616b 656e 2069  ns to be taken i
+00005010: 6e20 7768 6174 206f 7264 6572 2e20 416e  n what order. An
+00005020: 2061 6374 696f 6e20 6361 6e20 6569 7468   action can eith
+00005030: 6572 2062 6520 7573 696e 6720 6120 746f  er be using a to
+00005040: 6f6c 2061 6e64 206f 6273 6572 7669 6e67  ol and observing
+00005050: 2069 7473 206f 7574 7075 742c 206f 7220   its output, or 
+00005060: 7265 7475 726e 696e 6720 746f 2074 6865  returning to the
+00005070: 2075 7365 722e 2057 6527 7665 2068 6f73   user. We've hos
+00005080: 7465 6420 6120 2a2a 5b53 7472 6561 6d6c  ted a **[Streaml
+00005090: 6974 2050 6c61 7967 726f 756e 645d 2868  it Playground](h
+000050a0: 7474 7073 3a2f 2f6c 616e 6763 6861 696e  ttps://langchain
+000050b0: 2e77 6f6c 662e 6a69 6e61 2e61 692f 706c  .wolf.jina.ai/pl
+000050c0: 6179 6772 6f75 6e64 2f29 2a2a 206f 6e20  ayground/)** on 
+000050d0: 4a69 6e61 2041 4920 436c 6f75 6420 746f  Jina AI Cloud to
+000050e0: 2069 6e74 6572 6163 7420 7769 7468 2074   interact with t
+000050f0: 6865 2061 6765 6e74 732c 2077 6869 6368  he agents, which
+00005100: 2061 6363 6570 7473 2077 6974 6820 666f   accepts with fo
+00005110: 6c6c 6f77 696e 6720 696e 7075 7473 3a0a  llowing inputs:.
+00005120: 0a2d 202a 2a5b 4167 656e 7420 5479 7065  .- **[Agent Type
+00005130: 735d 2868 7474 7073 3a2f 2f70 7974 686f  s](https://pytho
+00005140: 6e2e 6c61 6e67 6368 6169 6e2e 636f 6d2f  n.langchain.com/
+00005150: 656e 2f6c 6174 6573 742f 6d6f 6475 6c65  en/latest/module
+00005160: 732f 6167 656e 7473 2f61 6765 6e74 732e  s/agents/agents.
+00005170: 6874 6d6c 293a 2a2a 2043 686f 6f73 6520  html):** Choose 
+00005180: 6672 6f6d 2064 6966 6665 7265 6e74 2061  from different a
+00005190: 6765 6e74 2074 7970 6573 2074 6861 7420  gent types that 
+000051a0: 4c61 6e67 6368 6169 6e20 7375 7070 6f72  Langchain suppor
+000051b0: 7473 2e20 0a0a 2d20 2a2a 5b54 6f6f 6c73  ts. ..- **[Tools
+000051c0: 5d28 6874 7470 733a 2f2f 7079 7468 6f6e  ](https://python
+000051d0: 2e6c 616e 6763 6861 696e 2e63 6f6d 2f65  .langchain.com/e
+000051e0: 6e2f 6c61 7465 7374 2f6d 6f64 756c 6573  n/latest/modules
+000051f0: 2f61 6765 6e74 732f 746f 6f6c 732e 6874  /agents/tools.ht
+00005200: 6d6c 293a 2a2a 2043 686f 6f73 6520 6672  ml):** Choose fr
+00005210: 6f6d 2064 6966 6665 7265 6e74 2074 6f6f  om different too
+00005220: 6c73 2074 6861 7420 4c61 6e67 6368 6169  ls that Langchai
+00005230: 6e20 7375 7070 6f72 7473 2e20 536f 6d65  n supports. Some
+00005240: 2074 6f6f 6c73 206d 6179 2072 6571 7569   tools may requi
+00005250: 7265 2061 6e20 4150 4920 746f 6b65 6e20  re an API token 
+00005260: 6f72 206f 7468 6572 2072 656c 6174 6564  or other related
+00005270: 2061 7267 756d 656e 7473 2e0a 0a54 6f20   arguments...To 
+00005280: 7573 6520 7468 6520 706c 6179 6772 6f75  use the playgrou
+00005290: 6e64 2c20 7369 6d70 6c79 2074 7970 6520  nd, simply type 
+000052a0: 796f 7572 2069 6e70 7574 2069 6e20 7468  your input in th
+000052b0: 6520 7465 7874 2062 6f78 2070 726f 7669  e text box provi
+000052c0: 6465 6420 746f 2067 6574 2074 6865 2061  ded to get the a
+000052d0: 6765 6e74 2773 206f 7574 7075 7420 616e  gent's output an
+000052e0: 6420 6368 6169 6e20 6f66 2074 686f 7567  d chain of thoug
+000052f0: 6874 2e20 456e 6a6f 7920 6578 706c 6f72  ht. Enjoy explor
+00005300: 696e 6720 4c61 6e67 6368 6169 6e27 7320  ing Langchain's 
+00005310: 6361 7061 6269 6c69 7469 6573 2120 496e  capabilities! In
+00005320: 2061 6464 6974 696f 6e20 746f 2073 7472   addition to str
+00005330: 6561 6d6c 6974 2c20 796f 7520 6361 6e20  eamlit, you can 
+00005340: 616c 736f 2075 7365 206f 7572 2052 4553  also use our RES
+00005350: 5466 756c 2041 5049 7320 6f6e 2074 6865  Tful APIs on the
+00005360: 2070 6c61 7967 726f 756e 6420 746f 2069   playground to i
+00005370: 6e74 6572 6163 7420 7769 7468 2074 6865  nteract with the
+00005380: 2061 6765 6e74 732e 200a 0a0a 2323 2320   agents. ...### 
+00005390: 5b5a 6572 6f2d 7368 6f74 2052 6561 6374  [Zero-shot React
+000053a0: 2044 6573 6372 6970 7469 6f6e 2061 6765   Description age
+000053b0: 6e74 2077 6974 6820 5365 7270 4150 4920  nt with SerpAPI 
+000053c0: 616e 6420 4361 6c63 756c 6174 6f72 5d28  and Calculator](
+000053d0: 6874 7470 733a 2f2f 7079 7468 6f6e 2e6c  https://python.l
+000053e0: 616e 6763 6861 696e 2e63 6f6d 2f65 6e2f  angchain.com/en/
+000053f0: 6c61 7465 7374 2f6d 6f64 756c 6573 2f61  latest/modules/a
+00005400: 6765 6e74 732f 6765 7474 696e 675f 7374  gents/getting_st
+00005410: 6172 7465 642e 6874 6d6c 290a 0a23 2323  arted.html)..###
+00005420: 2320 5374 7265 616d 6c69 7420 506c 6179  # Streamlit Play
+00005430: 6772 6f75 6e64 0a0a 215b 5374 7265 616d  ground..![Stream
+00005440: 6c69 7420 506c 6179 6772 6f75 6e64 5d28  lit Playground](
+00005450: 2e67 6974 6875 622f 696d 6167 6573 2f70  .github/images/p
+00005460: 6c61 7967 726f 756e 645f 6f6e 652e 6769  layground_one.gi
+00005470: 6629 0a0a 2323 2323 2052 4553 5466 756c  f)..#### RESTful
+00005480: 2041 5049 0a0a 6060 6062 6173 680a 6578   API..```bash.ex
+00005490: 706f 7274 204f 5045 4e41 495f 4150 495f  port OPENAI_API_
+000054a0: 4b45 593d 736b 2d2a 2a2a 0a65 7870 6f72  KEY=sk-***.expor
+000054b0: 7420 5345 5250 4150 495f 4150 495f 4b45  t SERPAPI_API_KE
+000054c0: 593d 2a2a 2a0a 0a63 7572 6c20 2d73 5820  Y=***..curl -sX 
+000054d0: 504f 5354 2027 6874 7470 733a 2f2f 6c61  POST 'https://la
+000054e0: 6e67 6368 6169 6e2e 776f 6c66 2e6a 696e  ngchain.wolf.jin
+000054f0: 612e 6169 2f61 7069 2f72 756e 2720 5c0a  a.ai/api/run' \.
+00005500: 2020 2d48 2027 6163 6365 7074 3a20 6170    -H 'accept: ap
+00005510: 706c 6963 6174 696f 6e2f 6a73 6f6e 2720  plication/json' 
+00005520: 5c0a 2020 2d48 2027 436f 6e74 656e 742d  \.  -H 'Content-
+00005530: 5479 7065 3a20 6170 706c 6963 6174 696f  Type: applicatio
+00005540: 6e2f 6a73 6f6e 2720 5c0a 2020 2d2d 6461  n/json' \.  --da
+00005550: 7461 2d72 6177 2027 7b0a 2020 2020 2274  ta-raw '{.    "t
+00005560: 6578 7422 3a20 2257 686f 2069 7320 4c65  ext": "Who is Le
+00005570: 6f20 4469 4361 7072 696f 7320 6769 726c  o DiCaprios girl
+00005580: 6672 6965 6e64 3f20 5768 6174 2069 7320  friend? What is 
+00005590: 6865 7220 6375 7272 656e 7420 6167 6520  her current age 
+000055a0: 7261 6973 6564 2074 6f20 7468 6520 302e  raised to the 0.
+000055b0: 3433 2070 6f77 6572 3f22 2c0a 2020 2020  43 power?",.    
+000055c0: 2270 6172 616d 6574 6572 7322 3a20 7b0a  "parameters": {.
+000055d0: 2020 2020 2020 2020 2274 6f6f 6c73 223a          "tools":
+000055e0: 207b 0a20 2020 2020 2020 2020 2020 2022   {.            "
+000055f0: 746f 6f6c 5f6e 616d 6573 223a 205b 2273  tool_names": ["s
+00005600: 6572 7061 7069 222c 2022 6c6c 6d2d 6d61  erpapi", "llm-ma
+00005610: 7468 225d 0a20 2020 2020 2020 207d 2c0a  th"].        },.
+00005620: 2020 2020 2020 2020 2261 6765 6e74 223a          "agent":
+00005630: 2022 7a65 726f 2d73 686f 742d 7265 6163   "zero-shot-reac
+00005640: 742d 6465 7363 7269 7074 696f 6e22 2c0a  t-description",.
+00005650: 2020 2020 2020 2020 2276 6572 626f 7365          "verbose
+00005660: 223a 2074 7275 650a 2020 2020 7d2c 0a20  ": true.    },. 
+00005670: 2020 2022 656e 7673 223a 207b 0a20 2020     "envs": {.   
+00005680: 2020 2020 2022 4f50 454e 4149 5f41 5049       "OPENAI_API
+00005690: 5f4b 4559 223a 2022 2722 247b 4f50 454e  _KEY": "'"${OPEN
+000056a0: 4149 5f41 5049 5f4b 4559 7d22 2722 2c0a  AI_API_KEY}"'",.
+000056b0: 2020 2020 2020 2020 2253 4552 5041 5049          "SERPAPI
+000056c0: 5f41 5049 5f4b 4559 223a 2022 2722 247b  _API_KEY": "'"${
+000056d0: 5345 5250 4150 495f 4150 495f 4b45 597d  SERPAPI_API_KEY}
+000056e0: 2227 220a 2020 2020 7d0a 7d27 207c 206a  "'".    }.}' | j
+000056f0: 710a 6060 6020 0a0a 6060 606a 736f 6e0a  q.``` ..```json.
+00005700: 7b0a 2020 2272 6573 756c 7422 3a20 2243  {.  "result": "C
+00005710: 616d 696c 6120 4d6f 7272 6f6e 6520 6973  amila Morrone is
+00005720: 204c 656f 2044 6943 6170 7269 6f27 7320   Leo DiCaprio's 
+00005730: 6769 726c 6672 6965 6e64 2c20 616e 6420  girlfriend, and 
+00005740: 6865 7220 6375 7272 656e 7420 6167 6520  her current age 
+00005750: 7261 6973 6564 2074 6f20 7468 6520 302e  raised to the 0.
+00005760: 3433 2070 6f77 6572 2069 7320 332e 3632  43 power is 3.62
+00005770: 3631 3236 3036 3131 3532 3935 3237 2e22  61260611529527."
+00005780: 2c0a 2020 2263 6861 696e 5f6f 665f 7468  ,.  "chain_of_th
+00005790: 6f75 6768 7422 3a20 225c 7530 3031 625b  ought": "\u001b[
+000057a0: 316d 3e20 456e 7465 7269 6e67 206e 6577  1m> Entering new
+000057b0: 2041 6765 6e74 4578 6563 7574 6f72 2063   AgentExecutor c
+000057c0: 6861 696e 2e2e 2e5c 7530 3031 625b 306d  hain...\u001b[0m
+000057d0: 5c75 3030 3162 5b33 323b 316d 5c75 3030  \u001b[32;1m\u00
+000057e0: 3162 5b31 3b33 6d20 4920 6e65 6564 2074  1b[1;3m I need t
+000057f0: 6f20 6669 6e64 206f 7574 2074 6865 206e  o find out the n
+00005800: 616d 6520 6f66 204c 656f 2773 2067 6972  ame of Leo's gir
+00005810: 6c66 7269 656e 6420 616e 6420 7468 656e  lfriend and then
+00005820: 2075 7365 2074 6865 2063 616c 6375 6c61   use the calcula
+00005830: 746f 7220 746f 2063 616c 6375 6c61 7465  tor to calculate
+00005840: 2068 6572 2061 6765 2074 6f20 7468 6520   her age to the 
+00005850: 302e 3433 2070 6f77 6572 2e41 6374 696f  0.43 power.Actio
+00005860: 6e3a 2053 6561 7263 6841 6374 696f 6e20  n: SearchAction 
+00005870: 496e 7075 743a 204c 656f 2044 6943 6170  Input: Leo DiCap
+00005880: 7269 6f20 6769 726c 6672 6965 6e64 5c75  rio girlfriend\u
+00005890: 3030 3162 5b30 6d4f 6273 6572 7661 7469  001b[0mObservati
+000058a0: 6f6e 3a20 5c75 3030 3162 5b33 363b 316d  on: \u001b[36;1m
+000058b0: 5c75 3030 3162 5b31 3b33 6d44 6943 6170  \u001b[1;3mDiCap
+000058c0: 7269 6f20 6d65 7420 6163 746f 7220 4361  rio met actor Ca
+000058d0: 6d69 6c61 204d 6f72 726f 6e65 2069 6e20  mila Morrone in 
+000058e0: 4465 6365 6d62 6572 2032 3031 372c 2077  December 2017, w
+000058f0: 6865 6e20 7368 6520 7761 7320 3230 2061  hen she was 20 a
+00005900: 6e64 2068 6520 7761 7320 3433 2e20 5468  nd he was 43. Th
+00005910: 6579 2077 6572 6520 7370 6f74 7465 6420  ey were spotted 
+00005920: 6174 2043 6f61 6368 656c 6c61 2061 6e64  at Coachella and
+00005930: 2077 656e 7420 6f6e 206d 756c 7469 706c   went on multipl
+00005940: 6520 7661 6361 7469 6f6e 7320 746f 6765  e vacations toge
+00005950: 7468 6572 2e20 536f 6d65 2072 6570 6f72  ther. Some repor
+00005960: 7473 2073 7567 6765 7374 6564 2074 6861  ts suggested tha
+00005970: 7420 4469 4361 7072 696f 2077 6173 2072  t DiCaprio was r
+00005980: 6561 6479 2074 6f20 6173 6b20 4d6f 7272  eady to ask Morr
+00005990: 6f6e 6520 746f 206d 6172 7279 2068 696d  one to marry him
+000059a0: 2e20 5468 6520 636f 7570 6c65 206d 6164  . The couple mad
+000059b0: 6520 7468 6569 7220 7265 6420 6361 7270  e their red carp
+000059c0: 6574 2064 6562 7574 2061 7420 7468 6520  et debut at the 
+000059d0: 3230 3230 2041 6361 6465 6d79 2041 7761  2020 Academy Awa
+000059e0: 7264 732e 5c75 3030 3162 5b30 6d54 686f  rds.\u001b[0mTho
+000059f0: 7567 6874 3a5c 7530 3031 625b 3332 3b31  ught:\u001b[32;1
+00005a00: 6d5c 7530 3031 625b 313b 336d 2049 206e  m\u001b[1;3m I n
+00005a10: 6565 6420 746f 2075 7365 2074 6865 2063  eed to use the c
+00005a20: 616c 6375 6c61 746f 7220 746f 2063 616c  alculator to cal
+00005a30: 6375 6c61 7465 2068 6572 2061 6765 2074  culate her age t
+00005a40: 6f20 7468 6520 302e 3433 2070 6f77 6572  o the 0.43 power
+00005a50: 4163 7469 6f6e 3a20 4361 6c63 756c 6174  Action: Calculat
+00005a60: 6f72 4163 7469 6f6e 2049 6e70 7574 3a20  orAction Input: 
+00005a70: 3230 5e30 2e34 335c 7530 3031 625b 306d  20^0.43\u001b[0m
+00005a80: 4f62 7365 7276 6174 696f 6e3a 205c 7530  Observation: \u0
+00005a90: 3031 625b 3333 3b31 6d5c 7530 3031 625b  01b[33;1m\u001b[
+00005aa0: 313b 336d 416e 7377 6572 3a20 332e 3632  1;3mAnswer: 3.62
+00005ab0: 3631 3236 3036 3131 3532 3935 3237 5c75  61260611529527\u
+00005ac0: 3030 3162 5b30 6d54 686f 7567 6874 3a5c  001b[0mThought:\
+00005ad0: 7530 3031 625b 3332 3b31 6d5c 7530 3031  u001b[32;1m\u001
+00005ae0: 625b 313b 336d 2049 206e 6f77 206b 6e6f  b[1;3m I now kno
+00005af0: 7720 7468 6520 6669 6e61 6c20 616e 7377  w the final answ
+00005b00: 6572 4669 6e61 6c20 416e 7377 6572 3a20  erFinal Answer: 
+00005b10: 4361 6d69 6c61 204d 6f72 726f 6e65 2069  Camila Morrone i
+00005b20: 7320 4c65 6f20 4469 4361 7072 696f 2773  s Leo DiCaprio's
+00005b30: 2067 6972 6c66 7269 656e 642c 2061 6e64   girlfriend, and
+00005b40: 2068 6572 2063 7572 7265 6e74 2061 6765   her current age
+00005b50: 2072 6169 7365 6420 746f 2074 6865 2030   raised to the 0
+00005b60: 2e34 3320 706f 7765 7220 6973 2033 2e36  .43 power is 3.6
+00005b70: 3236 3132 3630 3631 3135 3239 3532 372e  261260611529527.
+00005b80: 5c75 3030 3162 5b30 6d5c 7530 3031 625b  \u001b[0m\u001b[
+00005b90: 316d 3e20 4669 6e69 7368 6564 2063 6861  1m> Finished cha
+00005ba0: 696e 2e5c 7530 3031 625b 306d 220a 7d0a  in.\u001b[0m".}.
+00005bb0: 6060 600a 0a23 2323 205b 5365 6c66 2041  ```..### [Self A
+00005bc0: 736b 2057 6974 6820 5365 6172 6368 5d28  sk With Search](
+00005bd0: 6874 7470 733a 2f2f 7079 7468 6f6e 2e6c  https://python.l
+00005be0: 616e 6763 6861 696e 2e63 6f6d 2f65 6e2f  angchain.com/en/
+00005bf0: 6c61 7465 7374 2f6d 6f64 756c 6573 2f61  latest/modules/a
+00005c00: 6765 6e74 732f 696d 706c 656d 656e 7461  gents/implementa
+00005c10: 7469 6f6e 732f 7365 6c66 5f61 736b 5f77  tions/self_ask_w
+00005c20: 6974 685f 7365 6172 6368 2e68 746d 6c29  ith_search.html)
+00005c30: 0a0a 2323 2323 2053 7472 6561 6d6c 6974  ..#### Streamlit
+00005c40: 2050 6c61 7967 726f 756e 640a 0a21 5b53   Playground..![S
+00005c50: 7472 6561 6d6c 6974 2050 6c61 7967 726f  treamlit Playgro
+00005c60: 756e 645d 282e 6769 7468 7562 2f69 6d61  und](.github/ima
+00005c70: 6765 732f 706c 6179 6772 6f75 6e64 5f74  ges/playground_t
+00005c80: 776f 2e67 6966 290a 0a23 2323 2320 5245  wo.gif)..#### RE
+00005c90: 5354 6675 6c20 4150 490a 0a60 6060 6261  STful API..```ba
+00005ca0: 7368 0a65 7870 6f72 7420 4f50 454e 4149  sh.export OPENAI
+00005cb0: 5f41 5049 5f4b 4559 3d73 6b2d 2a2a 2a0a  _API_KEY=sk-***.
+00005cc0: 6578 706f 7274 2053 4552 5041 5049 5f41  export SERPAPI_A
+00005cd0: 5049 5f4b 4559 3d2a 2a2a 0a0a 6375 726c  PI_KEY=***..curl
+00005ce0: 202d 7358 2050 4f53 5420 2768 7474 7073   -sX POST 'https
+00005cf0: 3a2f 2f6c 616e 6763 6861 696e 2e77 6f6c  ://langchain.wol
+00005d00: 662e 6a69 6e61 2e61 692f 6170 692f 7275  f.jina.ai/api/ru
+00005d10: 6e27 205c 0a20 202d 4820 2761 6363 6570  n' \.  -H 'accep
+00005d20: 743a 2061 7070 6c69 6361 7469 6f6e 2f6a  t: application/j
+00005d30: 736f 6e27 205c 0a20 202d 4820 2743 6f6e  son' \.  -H 'Con
+00005d40: 7465 6e74 2d54 7970 653a 2061 7070 6c69  tent-Type: appli
+00005d50: 6361 7469 6f6e 2f6a 736f 6e27 205c 0a20  cation/json' \. 
+00005d60: 202d 2d64 6174 612d 7261 7720 277b 0a20   --data-raw '{. 
+00005d70: 2020 2022 7465 7874 223a 2022 5768 6174     "text": "What
+00005d80: 2069 7320 7468 6520 686f 6d65 746f 776e   is the hometown
+00005d90: 206f 6620 7468 6520 7265 6967 6e69 6e67   of the reigning
+00005da0: 206d 656e 7320 552e 532e 204f 7065 6e20   mens U.S. Open 
+00005db0: 6368 616d 7069 6f6e 3f22 2c0a 2020 2020  champion?",.    
+00005dc0: 2270 6172 616d 6574 6572 7322 3a20 7b0a  "parameters": {.
+00005dd0: 2020 2020 2020 2020 2274 6f6f 6c73 223a          "tools":
+00005de0: 207b 0a20 2020 2020 2020 2020 2020 2022   {.            "
+00005df0: 746f 6f6c 5f6e 616d 6573 223a 205b 2273  tool_names": ["s
+00005e00: 6572 7061 7069 225d 0a20 2020 2020 2020  erpapi"].       
+00005e10: 207d 2c0a 2020 2020 2020 2020 2261 6765   },.        "age
+00005e20: 6e74 223a 2022 7365 6c66 2d61 736b 2d77  nt": "self-ask-w
+00005e30: 6974 682d 7365 6172 6368 222c 0a20 2020  ith-search",.   
+00005e40: 2020 2020 2022 7665 7262 6f73 6522 3a20       "verbose": 
+00005e50: 7472 7565 0a20 2020 207d 2c0a 2020 2020  true.    },.    
+00005e60: 2265 6e76 7322 3a20 7b0a 2020 2020 2020  "envs": {.      
+00005e70: 2020 224f 5045 4e41 495f 4150 495f 4b45    "OPENAI_API_KE
+00005e80: 5922 3a20 2227 2224 7b4f 5045 4e41 495f  Y": "'"${OPENAI_
+00005e90: 4150 495f 4b45 597d 2227 222c 0a20 2020  API_KEY}"'",.   
+00005ea0: 2020 2020 2022 5345 5250 4150 495f 4150       "SERPAPI_AP
+00005eb0: 495f 4b45 5922 3a20 2227 2224 7b53 4552  I_KEY": "'"${SER
+00005ec0: 5041 5049 5f41 5049 5f4b 4559 7d22 2722  PAPI_API_KEY}"'"
+00005ed0: 0a20 2020 207d 0a7d 2720 7c20 6a71 0a60  .    }.}' | jq.`
+00005ee0: 6060 0a0a 6060 606a 736f 6e0a 7b0a 2020  ``..```json.{.  
+00005ef0: 2272 6573 756c 7422 3a20 2245 6c20 5061  "result": "El Pa
+00005f00: 6c6d 6172 2c20 4d75 7263 6961 2c20 5370  lmar, Murcia, Sp
+00005f10: 6169 6e22 2c0a 2020 2263 6861 696e 5f6f  ain",.  "chain_o
+00005f20: 665f 7468 6f75 6768 7422 3a20 225c 7530  f_thought": "\u0
+00005f30: 3031 625b 316d 3e20 456e 7465 7269 6e67  01b[1m> Entering
+00005f40: 206e 6577 2041 6765 6e74 4578 6563 7574   new AgentExecut
+00005f50: 6f72 2063 6861 696e 2e2e 2e5c 7530 3031  or chain...\u001
+00005f60: 625b 306d 5c75 3030 3162 5b33 323b 316d  b[0m\u001b[32;1m
+00005f70: 5c75 3030 3162 5b31 3b33 6d20 5965 732e  \u001b[1;3m Yes.
+00005f80: 466f 6c6c 6f77 2075 703a 2057 686f 2069  Follow up: Who i
+00005f90: 7320 7468 6520 7265 6967 6e69 6e67 206d  s the reigning m
+00005fa0: 656e 7320 552e 532e 204f 7065 6e20 6368  ens U.S. Open ch
+00005fb0: 616d 7069 6f6e 3f5c 7530 3031 625b 306d  ampion?\u001b[0m
+00005fc0: 496e 7465 726d 6564 6961 7465 2061 6e73  Intermediate ans
+00005fd0: 7765 723a 205c 7530 3031 625b 3336 3b31  wer: \u001b[36;1
+00005fe0: 6d5c 7530 3031 625b 313b 336d 4361 726c  m\u001b[1;3mCarl
+00005ff0: 6f73 2041 6c63 6172 617a 2047 6172 6669  os Alcaraz Garfi
+00006000: 615c 7530 3031 625b 306d 5c75 3030 3162  a\u001b[0m\u001b
+00006010: 5b33 323b 316d 5c75 3030 3162 5b31 3b33  [32;1m\u001b[1;3
+00006020: 6d46 6f6c 6c6f 7720 7570 3a20 5768 6174  mFollow up: What
+00006030: 2069 7320 4361 726c 6f73 2041 6c63 6172   is Carlos Alcar
+00006040: 617a 2047 6172 6669 6127 7320 686f 6d65  az Garfia's home
+00006050: 746f 776e 3f5c 7530 3031 625b 306d 496e  town?\u001b[0mIn
+00006060: 7465 726d 6564 6961 7465 2061 6e73 7765  termediate answe
+00006070: 723a 205c 7530 3031 625b 3336 3b31 6d5c  r: \u001b[36;1m\
+00006080: 7530 3031 625b 313b 336d 4361 726c 6f73  u001b[1;3mCarlos
+00006090: 2041 6c63 6172 617a 2047 6172 6669 6120   Alcaraz Garfia 
+000060a0: 7761 7320 626f 726e 206f 6e20 4d61 7920  was born on May 
+000060b0: 352c 2032 3030 332c 2069 6e20 456c 2050  5, 2003, in El P
+000060c0: 616c 6d61 722c 204d 7572 6369 612c 2053  almar, Murcia, S
+000060d0: 7061 696e 2074 6f20 7061 7265 6e74 7320  pain to parents 
+000060e0: 4361 726c 6f73 2041 6c63 6172 617a 2047  Carlos Alcaraz G
+000060f0: 6f6e 7ac3 a16c 657a 2061 6e64 2056 6972  onz..lez and Vir
+00006100: 6769 6e69 6120 4761 7266 6961 2045 7363  ginia Garfia Esc
+00006110: 616e 64c3 b36e 2e20 4865 2068 6173 2074  and..n. He has t
+00006120: 6872 6565 2073 6962 6c69 6e67 732e 5c75  hree siblings.\u
+00006130: 3030 3162 5b30 6d5c 7530 3031 625b 3332  001b[0m\u001b[32
+00006140: 3b31 6d5c 7530 3031 625b 313b 336d 536f  ;1m\u001b[1;3mSo
+00006150: 2074 6865 2066 696e 616c 2061 6e73 7765   the final answe
+00006160: 7220 6973 3a20 456c 2050 616c 6d61 722c  r is: El Palmar,
+00006170: 204d 7572 6369 612c 2053 7061 696e 5c75   Murcia, Spain\u
+00006180: 3030 3162 5b30 6d5c 7530 3031 625b 316d  001b[0m\u001b[1m
+00006190: 3e20 4669 6e69 7368 6564 2063 6861 696e  > Finished chain
+000061a0: 2e5c 7530 3031 625b 306d 220a 7d0a 6060  .\u001b[0m".}.``
+000061b0: 600a 0a2d 2d2d 0a0a 2323 2043 6861 696e  `..---..## Chain
+000061c0: 7320 6f6e 204a 696e 6120 f09f 93a6 f09f  s on Jina ......
+000061d0: 9a80 0a0a 5b43 6861 696e 735d 2868 7474  ....[Chains](htt
+000061e0: 7073 3a2f 2f70 7974 686f 6e2e 6c61 6e67  ps://python.lang
+000061f0: 6368 6169 6e2e 636f 6d2f 656e 2f6c 6174  chain.com/en/lat
+00006200: 6573 742f 6d6f 6475 6c65 732f 6368 6169  est/modules/chai
+00006210: 6e73 2f67 6574 7469 6e67 5f73 7461 7274  ns/getting_start
+00006220: 6564 2e68 746d 6c29 2069 6e20 4c61 6e67  ed.html) in Lang
+00006230: 4368 6169 6e20 616c 6c6f 7720 7573 6572  Chain allow user
+00006240: 7320 746f 2063 6f6d 6269 6e65 2063 6f6d  s to combine com
+00006250: 706f 6e65 6e74 7320 746f 2063 7265 6174  ponents to creat
+00006260: 6520 6120 7369 6e67 6c65 2c20 636f 6865  e a single, cohe
+00006270: 7265 6e74 2061 7070 6c69 6361 7469 6f6e  rent application
+00006280: 2e20 5769 7468 204a 696e 612c 200a 0a2d  . With Jina, ..-
+00006290: 2059 6f75 2063 616e 2065 7870 6f73 6520   You can expose 
+000062a0: 796f 7572 2060 4368 6169 6e60 2061 7320  your `Chain` as 
+000062b0: 5245 5354 6675 6c2f 6752 5043 2f57 6562  RESTful/gRPC/Web
+000062c0: 536f 636b 6574 2041 5049 2e0a 2d20 456e  Socket API..- En
+000062d0: 6162 6c65 2060 4368 6169 6e60 7320 746f  able `Chain`s to
+000062e0: 2064 6570 6c6f 7920 2620 7363 616c 6520   deploy & scale 
+000062f0: 7365 7061 7261 7465 6c79 2066 726f 6d20  separately from 
+00006300: 7468 6520 7265 7374 206f 6620 796f 7572  the rest of your
+00006310: 2061 7070 6c69 6361 7469 6f6e 2077 6974   application wit
+00006320: 6820 7468 6520 6865 6c70 206f 6620 4578  h the help of Ex
+00006330: 6563 7574 6f72 732e 0a2d 2044 6570 6c6f  ecutors..- Deplo
+00006340: 7920 796f 7572 2060 4368 6169 6e60 206f  y your `Chain` o
+00006350: 6e20 4a69 6e61 2041 4920 436c 6f75 6420  n Jina AI Cloud 
+00006360: 616e 6420 6765 7420 6578 636c 7573 6976  and get exclusiv
+00006370: 6520 6163 6365 7373 2074 6f20 4167 656e  e access to Agen
+00006380: 7473 206f 6e20 4a69 6e61 2041 4920 436c  ts on Jina AI Cl
+00006390: 6f75 6420 2863 6f6d 696e 6720 736f 6f6e  oud (coming soon
+000063a0: 290a 0a23 2323 2045 7861 6d70 6c65 730a  )..### Examples.
+000063b0: 0a7c 2045 7861 6d70 6c65 207c 204c 616e  .| Example | Lan
+000063c0: 6743 6861 696e 2044 6f63 7320 7c20 4465  gChain Docs | De
+000063d0: 7363 7269 7074 696f 6e20 7c0a 7c20 2d2d  scription |.| --
+000063e0: 2d2d 2d2d 2d20 7c20 2d2d 2d2d 2d2d 2d2d  ----- | --------
+000063f0: 2d2d 2d20 7c20 2d2d 2d2d 2d2d 2d2d 2d2d  --- | ----------
+00006400: 2d20 7c0a 7c20 5b4c 4c4d 2043 6861 696e  - |.| [LLM Chain
+00006410: 5d28 6578 616d 706c 6573 2f6c 6c6d 5f63  ](examples/llm_c
+00006420: 6861 696e 2e6d 6429 207c 205b 4c69 6e6b  hain.md) | [Link
+00006430: 5d28 6874 7470 733a 2f2f 6c61 6e67 6368  ](https://langch
+00006440: 6169 6e2e 7265 6164 7468 6564 6f63 732e  ain.readthedocs.
+00006450: 696f 2f65 6e2f 6c61 7465 7374 2f6d 6f64  io/en/latest/mod
+00006460: 756c 6573 2f63 6861 696e 732f 6765 7474  ules/chains/gett
+00006470: 696e 675f 7374 6172 7465 642e 6874 6d6c  ing_started.html
+00006480: 2371 7565 7279 2d61 6e2d 6c6c 6d2d 7769  #query-an-llm-wi
+00006490: 7468 2d74 6865 2d6c 6c6d 6368 6169 6e29  th-the-llmchain)
+000064a0: 207c 2045 7870 6f73 6520 6043 6861 696e   | Expose `Chain
+000064b0: 6020 6173 2052 4553 5466 756c 2f67 5250  ` as RESTful/gRP
+000064c0: 432f 5765 6253 6f63 6b65 7420 4150 4920  C/WebSocket API 
+000064d0: 6c6f 6361 6c6c 7920 7c0a 7c20 5b53 696d  locally |.| [Sim
+000064e0: 706c 6520 5365 7175 656e 7469 616c 2043  ple Sequential C
+000064f0: 6861 696e 5d28 6578 616d 706c 6573 2f73  hain](examples/s
+00006500: 696d 706c 655f 7365 7175 656e 7469 616c  imple_sequential
+00006510: 5f63 6861 696e 2e6d 6429 207c 205b 4c69  _chain.md) | [Li
+00006520: 6e6b 5d28 6874 7470 733a 2f2f 6c61 6e67  nk](https://lang
+00006530: 6368 6169 6e2e 7265 6164 7468 6564 6f63  chain.readthedoc
+00006540: 732e 696f 2f65 6e2f 6c61 7465 7374 2f6d  s.io/en/latest/m
+00006550: 6f64 756c 6573 2f63 6861 696e 732f 6765  odules/chains/ge
+00006560: 6e65 7269 632f 7365 7175 656e 7469 616c  neric/sequential
+00006570: 5f63 6861 696e 732e 6874 6d6c 2373 696d  _chains.html#sim
+00006580: 706c 6573 6571 7565 6e74 6961 6c63 6861  plesequentialcha
+00006590: 696e 2920 7c20 4578 706f 7365 2060 4368  in) | Expose `Ch
+000065a0: 6169 6e60 2061 7320 5245 5354 6675 6c2f  ain` as RESTful/
+000065b0: 6752 5043 2f57 6562 536f 636b 6574 2041  gRPC/WebSocket A
+000065c0: 5049 206c 6f63 616c 6c79 207c 0a7c 205b  PI locally |.| [
+000065d0: 5365 7175 656e 7469 616c 2043 6861 696e  Sequential Chain
+000065e0: 5d28 6578 616d 706c 6573 2f73 6571 7565  ](examples/seque
+000065f0: 6e74 6961 6c5f 6368 6169 6e2e 6d64 2920  ntial_chain.md) 
+00006600: 7c20 5b4c 696e 6b5d 2868 7474 7073 3a2f  | [Link](https:/
+00006610: 2f6c 616e 6763 6861 696e 2e72 6561 6474  /langchain.readt
+00006620: 6865 646f 6373 2e69 6f2f 656e 2f6c 6174  hedocs.io/en/lat
+00006630: 6573 742f 6d6f 6475 6c65 732f 6368 6169  est/modules/chai
+00006640: 6e73 2f67 656e 6572 6963 2f73 6571 7565  ns/generic/seque
+00006650: 6e74 6961 6c5f 6368 6169 6e73 2e68 746d  ntial_chains.htm
+00006660: 6c23 7365 7175 656e 7469 616c 2d63 6861  l#sequential-cha
+00006670: 696e 2920 7c20 4578 706f 7365 2060 4368  in) | Expose `Ch
+00006680: 6169 6e60 2061 7320 5245 5354 6675 6c2f  ain` as RESTful/
+00006690: 6752 5043 2f57 6562 536f 636b 6574 2041  gRPC/WebSocket A
+000066a0: 5049 206c 6f63 616c 6c79 207c 0a7c 205b  PI locally |.| [
+000066b0: 4c4c 4d20 4d61 7468 2043 6861 696e 5d28  LLM Math Chain](
+000066c0: 6578 616d 706c 6573 2f6c 6c6d 5f6d 6174  examples/llm_mat
+000066d0: 682e 6d64 2920 7c20 5b4c 696e 6b5d 2868  h.md) | [Link](h
+000066e0: 7474 7073 3a2f 2f6c 616e 6763 6861 696e  ttps://langchain
+000066f0: 2e72 6561 6474 6865 646f 6373 2e69 6f2f  .readthedocs.io/
+00006700: 656e 2f6c 6174 6573 742f 6d6f 6475 6c65  en/latest/module
+00006710: 732f 6368 6169 6e73 2f65 7861 6d70 6c65  s/chains/example
+00006720: 732f 6c6c 6d5f 6d61 7468 2e68 746d 6c29  s/llm_math.html)
+00006730: 207c 2045 7870 6f73 6520 6043 6861 696e   | Expose `Chain
+00006740: 6020 6173 2052 4553 5466 756c 2f67 5250  ` as RESTful/gRP
+00006750: 432f 5765 6253 6f63 6b65 7420 4150 4920  C/WebSocket API 
+00006760: 6c6f 6361 6c6c 7920 7c0a 7c20 5b4c 4c4d  locally |.| [LLM
+00006770: 2052 6571 7565 7374 7320 4368 6169 6e5d   Requests Chain]
+00006780: 2865 7861 6d70 6c65 732f 6c6c 6d5f 7265  (examples/llm_re
+00006790: 7175 6573 7473 5f63 6861 696e 2e6d 6429  quests_chain.md)
+000067a0: 207c 205b 4c69 6e6b 5d28 6874 7470 733a   | [Link](https:
+000067b0: 2f2f 6c61 6e67 6368 6169 6e2e 7265 6164  //langchain.read
+000067c0: 7468 6564 6f63 732e 696f 2f65 6e2f 6c61  thedocs.io/en/la
+000067d0: 7465 7374 2f6d 6f64 756c 6573 2f63 6861  test/modules/cha
+000067e0: 696e 732f 6578 616d 706c 6573 2f6c 6c6d  ins/examples/llm
+000067f0: 5f72 6571 7565 7374 732e 6874 6d6c 2920  _requests.html) 
+00006800: 7c20 4578 706f 7365 2060 4368 6169 6e60  | Expose `Chain`
+00006810: 2061 7320 5245 5354 6675 6c2f 6752 5043   as RESTful/gRPC
+00006820: 2f57 6562 536f 636b 6574 2041 5049 206c  /WebSocket API l
+00006830: 6f63 616c 6c79 207c 0a7c 205b 4375 7374  ocally |.| [Cust
+00006840: 6f6d 2043 6861 696e 5d28 6578 616d 706c  om Chain](exampl
+00006850: 6573 2f63 7573 746f 6d5f 6368 6169 6e2e  es/custom_chain.
+00006860: 6d64 2920 7c20 5b4c 696e 6b5d 2868 7474  md) | [Link](htt
+00006870: 7073 3a2f 2f6c 616e 6763 6861 696e 2e72  ps://langchain.r
+00006880: 6561 6474 6865 646f 6373 2e69 6f2f 656e  eadthedocs.io/en
+00006890: 2f6c 6174 6573 742f 6d6f 6475 6c65 732f  /latest/modules/
+000068a0: 6368 6169 6e73 2f67 6574 7469 6e67 5f73  chains/getting_s
+000068b0: 7461 7274 6564 2e68 746d 6c23 6372 6561  tarted.html#crea
+000068c0: 7465 2d61 2d63 7573 746f 6d2d 6368 6169  te-a-custom-chai
+000068d0: 6e2d 7769 7468 2d74 6865 2d63 6861 696e  n-with-the-chain
+000068e0: 2d63 6c61 7373 2920 7c20 4578 706f 7365  -class) | Expose
+000068f0: 2060 4368 6169 6e60 2061 7320 5245 5354   `Chain` as REST
+00006900: 6675 6c2f 6752 5043 2f57 6562 536f 636b  ful/gRPC/WebSock
+00006910: 6574 2041 5049 206c 6f63 616c 6c79 207c  et API locally |
+00006920: 0a7c 205b 5365 7175 656e 7469 616c 2043  .| [Sequential C
+00006930: 6861 696e 735d 2865 7861 6d70 6c65 732f  hains](examples/
+00006940: 7365 7175 656e 7469 616c 5f65 7865 6375  sequential_execu
+00006950: 746f 7273 2e6d 6429 207c 204e 2f41 207c  tors.md) | N/A |
+00006960: 2042 7569 6c64 2026 2073 6361 6c65 2060   Build & scale `
+00006970: 4368 6169 6e73 6020 696e 2073 6570 6172  Chains` in separ
+00006980: 6174 6520 6045 7865 6375 746f 7260 7320  ate `Executor`s 
+00006990: 7c0a 7c20 5b42 7261 6e63 6869 6e67 2043  |.| [Branching C
+000069a0: 6861 696e 735d 2865 7861 6d70 6c65 732f  hains](examples/
+000069b0: 6272 616e 6368 696e 672e 6d64 2920 7c20  branching.md) | 
+000069c0: 4e2f 4120 7c20 4272 616e 6368 696e 6720  N/A | Branching 
+000069d0: 6043 6861 696e 7360 2069 6e20 7365 7061  `Chains` in sepa
+000069e0: 7261 7465 2060 4578 6563 7574 6f72 6073  rate `Executor`s
+000069f0: 2074 6f20 616c 6c6f 7720 7061 7261 6c6c   to allow parall
+00006a00: 656c 2065 7865 6375 7469 6f6e 207c 0a0a  el execution |..
+00006a10: 0a0a                                     ..
```

### Comparing `langchain-serve-0.0.9.dev22/langchain_serve.egg-info/SOURCES.txt` & `langchain-serve-0.0.9.dev9/langchain_serve.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `langchain-serve-0.0.9.dev22/lcserve/__main__.py` & `langchain-serve-0.0.9.dev9/lcserve/__main__.py`

 * *Files identical despite different names*

### Comparing `langchain-serve-0.0.9.dev22/lcserve/apps/babyagi/app.py` & `langchain-serve-0.0.9.dev9/lcserve/apps/babyagi/app.py`

 * *Files identical despite different names*

### Comparing `langchain-serve-0.0.9.dev22/lcserve/apps/babyagi/babyagi.py` & `langchain-serve-0.0.9.dev9/lcserve/apps/babyagi/babyagi.py`

 * *Files identical despite different names*

### Comparing `langchain-serve-0.0.9.dev22/lcserve/backend/agentexecutor.py` & `langchain-serve-0.0.9.dev9/lcserve/backend/agentexecutor.py`

 * *Files identical despite different names*

### Comparing `langchain-serve-0.0.9.dev22/lcserve/backend/gateway.py` & `langchain-serve-0.0.9.dev9/lcserve/backend/gateway.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,37 +4,35 @@
 import shutil
 import sys
 import time
 from enum import Enum
 from importlib import import_module
 from importlib.util import module_from_spec, spec_from_file_location
 from pathlib import Path
-from typing import TYPE_CHECKING, Callable, Dict, List, Tuple, Type, Any, Union
+from typing import TYPE_CHECKING, Callable, Dict, List, Tuple, Type, Any
 
 from docarray import Document, DocumentArray
 from jina import Gateway
 from jina.enums import ProtocolType as GatewayProtocolType
 from jina.serve.runtimes.gateway.composite import CompositeGateway
 from jina.serve.runtimes.gateway.http.fastapi import FastAPIBaseGateway
 from pydantic import Field, ValidationError, create_model
-from websockets.exceptions import ConnectionClosed
 
 from .playground.utils.helper import (
     AGENT_OUTPUT,
     APPDIR,
     DEFAULT_KEY,
     LANGCHAIN_API_PORT,
     LANGCHAIN_PLAYGROUND_PORT,
     RESULT,
     SERVING,
     Capturing,
     EnvironmentVarCtxtManager,
     parse_uses_with,
     run_cmd,
-    run_function,
 )
 from .playground.utils.langchain_helper import (
     AsyncStreamingWebsocketCallbackHandler,
     BuiltinsWrapper,
     StreamingWebsocketCallbackHandler,
 )
 
@@ -437,15 +435,15 @@
                 if hasattr(input_data, 'envs'):
                     _envs = input_data.envs
                     del input_data.envs
 
                 with EnvironmentVarCtxtManager(_envs):
                     with Capturing() as stdout:
                         try:
-                            output = run_function(func, **dict(input_data))
+                            output = func(**dict(input_data))
                         except Exception as e:
                             self.logger.error(f'Got an exception: {e}')
                             error = str(e)
 
                     if error != '':
                         print(f'Error: {error}')
                     return output_model(
@@ -459,23 +457,14 @@
             self._update_dry_run_with_ws()
 
             @self.app.websocket(path=f'/{func.__name__}', name=_name)
             async def _create_ws_route(websocket: WebSocket):
                 with BuiltinsWrapper(
                     websocket=websocket, output_model=output_model, wrap_print=False
                 ):
-
-                    def _get_error_msg(
-                        e: Union[WebSocketDisconnect, ConnectionClosed]
-                    ) -> str:
-                        return (
-                            f'Client {websocket.client} disconnected from `{func.__name__}` with code {e.code}'
-                            + (f' and reason {e.reason}' if e.reason else '')
-                        )
-
                     await websocket.accept()
                     _ws_recv_lock = asyncio.Lock()
                     try:
                         while True:
                             # if websocket is closed, break
                             if websocket.client_state not in [
                                 WebSocketState.CONNECTED,
@@ -525,17 +514,15 @@
                                                 'async_streaming_handler': AsyncStreamingWebsocketCallbackHandler(
                                                     websocket=websocket,
                                                     output_model=output_model,
                                                 ),
                                             }
                                         )
 
-                                    _returned_data = await run_function(
-                                        func, **_input_data_dict
-                                    )
+                                    _returned_data = func(**_input_data_dict)
                                     if inspect.isgenerator(_returned_data):
                                         # If the function is a generator, we iterate through the generator and send each item back to the client.
                                         for _stream in _returned_data:
                                             _data = output_model(
                                                 result=_stream,
                                                 error=_ws_serving_error,
                                             )
@@ -552,16 +539,18 @@
                                     # Once the generator is exhausted/ function call is completed, send a close message
                                     self.logger.info(
                                         f'Closing ws connection `{func.__name__}` for client: {websocket.client}'
                                     )
                                     await websocket.close()
                                     break
 
-                                except (WebSocketDisconnect, ConnectionClosed) as e:
-                                    self.logger.info(_get_error_msg(e))
+                                except WebSocketDisconnect as e:
+                                    self.logger.info(
+                                        f'Client {websocket.client} disconnected from `{func.__name__}` with code {e.code} and reason {e.reason}'
+                                    )
                                     break
 
                                 except Exception as e:
                                     self.logger.error(f'Got an exception: {e}')
                                     _ws_serving_error = str(e)
                                     # For other errors, we send the error back to the client.
                                     _data = output_model(
@@ -569,10 +558,12 @@
                                         error=_ws_serving_error,
                                     )
                                     await websocket.send_text(_data.json())
 
                                 if _ws_serving_error != '':
                                     print(f'Error: {_ws_serving_error}')
 
-                    except (WebSocketDisconnect, ConnectionClosed) as e:
-                        self.logger.info(_get_error_msg(e))
+                    except WebSocketDisconnect as e:
+                        self.logger.info(
+                            f'Client {websocket.client} disconnected from `{func.__name__}` with code {e.code} and reason {e.reason}'
+                        )
                         return
```

### Comparing `langchain-serve-0.0.9.dev22/lcserve/backend/nginx.conf` & `langchain-serve-0.0.9.dev9/lcserve/backend/nginx.conf`

 * *Files identical despite different names*

### Comparing `langchain-serve-0.0.9.dev22/lcserve/backend/playground/app.py` & `langchain-serve-0.0.9.dev9/lcserve/backend/playground/app.py`

 * *Files identical despite different names*

### Comparing `langchain-serve-0.0.9.dev22/lcserve/backend/playground/utils/helper.py` & `langchain-serve-0.0.9.dev9/lcserve/backend/playground/utils/helper.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,17 +2,15 @@
 import os
 import subprocess
 import sys
 import threading
 import uuid
 from collections import defaultdict
 from io import StringIO
-from typing import Any, Dict, List, Union, Callable
-import inspect
-import functools
+from typing import Any, Dict, List, Union
 
 import nest_asyncio
 from pydantic import BaseModel
 
 CLS = 'cls'
 RESULT = 'result'
 LLM_TYPE = '_type'
@@ -154,17 +152,7 @@
 
 def get_random_tag():
     return 't-' + uuid.uuid4().hex[:5]
 
 
 def get_random_name():
     return 'n-' + uuid.uuid4().hex[:5]
-
-
-async def run_function(func: Callable, **kwargs):
-    if inspect.iscoroutinefunction(func):
-        return await func(**kwargs)
-    else:
-        return await get_or_create_eventloop().run_in_executor(
-            None,
-            functools.partial(func, **kwargs),
-        )
```

### Comparing `langchain-serve-0.0.9.dev22/lcserve/backend/playground/utils/langchain_helper.py` & `langchain-serve-0.0.9.dev9/lcserve/backend/playground/utils/langchain_helper.py`

 * *Files identical despite different names*

### Comparing `langchain-serve-0.0.9.dev22/lcserve/backend/playground/utils/talk.py` & `langchain-serve-0.0.9.dev9/lcserve/backend/playground/utils/talk.py`

 * *Files identical despite different names*

### Comparing `langchain-serve-0.0.9.dev22/lcserve/backend/playground/utils/tools.py` & `langchain-serve-0.0.9.dev9/lcserve/backend/playground/utils/tools.py`

 * *Files identical despite different names*

### Comparing `langchain-serve-0.0.9.dev22/lcserve/customgateway.Dockerfile` & `langchain-serve-0.0.9.dev9/lcserve/customgateway.Dockerfile`

 * *Files identical despite different names*

### Comparing `langchain-serve-0.0.9.dev22/lcserve/flow.py` & `langchain-serve-0.0.9.dev9/lcserve/flow.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,16 +17,14 @@
 from docarray import Document, DocumentArray
 from jina import Flow
 
 APP_NAME = 'langchain'
 BABYAGI_APP_NAME = 'babyagi'
 ServingGatewayConfigFile = 'servinggateway_config.yml'
 JCloudConfigFile = 'jcloud_config.yml'
-# TODO: this needs to be pulled from Jina Wolf API dynamically after the issue has been fixed on the API side
-APP_LOGS_URL = 'https://dashboard.wolf.jina.ai/d/flow/flow-monitor?var-flow={flow}&var-datasource=thanos&orgId=2&from=now-24h&to=now&viewPanel=85'
 
 
 def syncify(f):
     @wraps(f)
     def wrapper(*args, **kwargs):
         return asyncio.run(f(*args, **kwargs))
 
@@ -518,20 +516,17 @@
             return list(endpoints.values())[0] if endpoints else ''
 
         def _replace_wss_with_https(endpoint: str):
             return endpoint.replace('wss://', 'https://')
 
         status: Dict = app_status['status']
         endpoint = _get_endpoint(status)
-        flow_namespace = app_id.split("-")[-1]
-
-        _add_row('App ID', app_id, bold_key=True, bold_value=True)
+        _add_row('AppID', app_id, bold_key=True, bold_value=True)
         _add_row('Phase', status.get('phase', ''))
         _add_row('Endpoint', endpoint)
-        _add_row('App logs', APP_LOGS_URL.format(flow=flow_namespace))
         _add_row('Swagger UI', _replace_wss_with_https(f'{endpoint}/docs'))
         _add_row('OpenAPI JSON', _replace_wss_with_https(f'{endpoint}/openapi.json'))
         console.print(_t)
 
 
 async def list_apps_on_jcloud(phase: str, name: str):
     from jcloud.flow import CloudFlow
```

### Comparing `langchain-serve-0.0.9.dev22/lcserve/flow.yml` & `langchain-serve-0.0.9.dev9/lcserve/flow.yml`

 * *Files identical despite different names*

### Comparing `langchain-serve-0.0.9.dev22/lcserve/playground/babyagi/playground.py` & `langchain-serve-0.0.9.dev9/lcserve/playground/babyagi/playground.py`

 * *Files identical despite different names*

### Comparing `langchain-serve-0.0.9.dev22/lcserve/playground/babyagi/user_input.py` & `langchain-serve-0.0.9.dev9/lcserve/playground/babyagi/user_input.py`

 * *Files identical despite different names*

### Comparing `langchain-serve-0.0.9.dev22/setup.py` & `langchain-serve-0.0.9.dev9/setup.py`

 * *Files identical despite different names*

