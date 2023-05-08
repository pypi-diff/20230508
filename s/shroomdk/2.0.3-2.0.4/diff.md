# Comparing `tmp/shroomdk-2.0.3.tar.gz` & `tmp/shroomdk-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shroomdk-2.0.3.tar", last modified: Tue May  2 20:15:21 2023, max compression
+gzip compressed data, was "shroomdk-2.0.4.tar", last modified: Mon May  8 14:20:04 2023, max compression
```

## Comparing `shroomdk-2.0.3.tar` & `shroomdk-2.0.4.tar`

### file list

```diff
@@ -1,144 +1,144 @@
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 20:15:21.212392 shroomdk-2.0.3/
--rw-r--r--   0 jim        (501) staff       (20)     1073 2022-07-25 21:42:15.000000 shroomdk-2.0.3/LICENSE.txt
--rw-r--r--   0 jim        (501) staff       (20)       69 2022-07-25 21:42:15.000000 shroomdk-2.0.3/MANIFEST.in
--rw-r--r--   0 jim        (501) staff       (20)     1510 2023-05-02 20:15:21.212468 shroomdk-2.0.3/PKG-INFO
--rw-r--r--   0 jim        (501) staff       (20)      709 2023-05-02 18:18:58.000000 shroomdk-2.0.3/README.md
--rw-r--r--   0 jim        (501) staff       (20)        5 2023-05-02 20:14:01.000000 shroomdk-2.0.3/VERSION
--rw-r--r--   0 jim        (501) staff       (20)       30 2022-07-25 21:42:15.000000 shroomdk-2.0.3/requirements-dev.txt
--rw-r--r--   0 jim        (501) staff       (20)       33 2023-05-02 18:10:35.000000 shroomdk-2.0.3/requirements.txt
--rw-r--r--   0 jim        (501) staff       (20)       79 2023-05-02 20:15:21.213132 shroomdk-2.0.3/setup.cfg
--rw-r--r--   0 jim        (501) staff       (20)     1557 2023-05-02 18:10:35.000000 shroomdk-2.0.3/setup.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 20:15:21.197098 shroomdk-2.0.3/shroomdk/
--rw-r--r--   0 jim        (501) staff       (20)      147 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/__init__.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 20:15:21.198395 shroomdk-2.0.3/shroomdk/errors/
--rw-r--r--   0 jim        (501) staff       (20)      336 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/errors/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)     1583 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/errors/api_error.py
--rw-r--r--   0 jim        (501) staff       (20)      121 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/errors/base_error.py
--rw-r--r--   0 jim        (501) staff       (20)     2077 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/errors/query_run_errors.py
--rw-r--r--   0 jim        (501) staff       (20)      262 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/errors/sdk_error.py
--rw-r--r--   0 jim        (501) staff       (20)      361 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/errors/server_error.py
--rw-r--r--   0 jim        (501) staff       (20)     2968 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/flipside.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 20:15:21.198512 shroomdk-2.0.3/shroomdk/integrations/
--rw-r--r--   0 jim        (501) staff       (20)       69 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/integrations/__init__.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 20:15:21.198967 shroomdk-2.0.3/shroomdk/integrations/query_integration/
--rw-r--r--   0 jim        (501) staff       (20)       77 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/integrations/query_integration/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)     9884 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/integrations/query_integration/compass_query_integration.py
--rw-r--r--   0 jim        (501) staff       (20)      237 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/integrations/query_integration/defaults.py
--rw-r--r--   0 jim        (501) staff       (20)     3570 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/integrations/query_integration/query_result_set_builder.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 20:15:21.199768 shroomdk-2.0.3/shroomdk/models/
--rw-r--r--   0 jim        (501) staff       (20)      365 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/models/__init__.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 20:15:21.200570 shroomdk-2.0.3/shroomdk/models/compass/
--rw-r--r--   0 jim        (501) staff       (20)       50 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/models/compass/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)      571 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/models/compass/cancel_query_run.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 20:15:21.201890 shroomdk-2.0.3/shroomdk/models/compass/core/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/models/compass/core/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)      187 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/models/compass/core/column_metadata.py
--rw-r--r--   0 jim        (501) staff       (20)      117 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/models/compass/core/page.py
--rw-r--r--   0 jim        (501) staff       (20)      183 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/models/compass/core/page_stats.py
--rw-r--r--   0 jim        (501) staff       (20)      358 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/models/compass/core/query_request.py
--rw-r--r--   0 jim        (501) staff       (20)      807 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/models/compass/core/query_run.py
--rw-r--r--   0 jim        (501) staff       (20)       89 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/models/compass/core/result_format.py
--rw-r--r--   0 jim        (501) staff       (20)      149 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/models/compass/core/rpc_error.py
--rw-r--r--   0 jim        (501) staff       (20)      198 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/models/compass/core/rpc_request.py
--rw-r--r--   0 jim        (501) staff       (20)      252 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/models/compass/core/rpc_response.py
--rw-r--r--   0 jim        (501) staff       (20)      340 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/models/compass/core/sql_statement.py
--rw-r--r--   0 jim        (501) staff       (20)      221 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/models/compass/core/tags.py
--rw-r--r--   0 jim        (501) staff       (20)      845 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/models/compass/create_query_run.py
--rw-r--r--   0 jim        (501) staff       (20)      639 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/models/compass/get_query_run.py
--rw-r--r--   0 jim        (501) staff       (20)     2026 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/models/compass/get_query_run_results.py
--rw-r--r--   0 jim        (501) staff       (20)      582 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/models/compass/get_sql_statement.py
--rw-r--r--   0 jim        (501) staff       (20)      852 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/models/compass/query_results.py
--rw-r--r--   0 jim        (501) staff       (20)     1422 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/models/query.py
--rw-r--r--   0 jim        (501) staff       (20)      836 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/models/query_defaults.py
--rw-r--r--   0 jim        (501) staff       (20)     1031 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/models/query_result_set.py
--rw-r--r--   0 jim        (501) staff       (20)     1658 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/models/query_run_stats.py
--rw-r--r--   0 jim        (501) staff       (20)      544 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/models/query_status.py
--rw-r--r--   0 jim        (501) staff       (20)      194 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/models/sleep_config.py
--rw-r--r--   0 jim        (501) staff       (20)     5898 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/rpc.py
--rw-r--r--   0 jim        (501) staff       (20)       68 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/shroomdk.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 20:15:21.202107 shroomdk-2.0.3/shroomdk/tests/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/tests/__init__.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 20:15:21.202217 shroomdk-2.0.3/shroomdk/tests/integrations/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/tests/integrations/__init__.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 20:15:21.202507 shroomdk-2.0.3/shroomdk/tests/integrations/query_integration/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/tests/integrations/query_integration/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)     8712 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/tests/integrations/query_integration/test_query_compass_integration.py
--rw-r--r--   0 jim        (501) staff       (20)     3438 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/tests/integrations/query_integration/test_query_result_set_builder.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 20:15:21.202720 shroomdk-2.0.3/shroomdk/tests/models/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/tests/models/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)      931 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/tests/models/test_query_status.py
--rw-r--r--   0 jim        (501) staff       (20)     5218 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/tests/test_rpc.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 20:15:21.202913 shroomdk-2.0.3/shroomdk/tests/utils/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/tests/utils/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)     2242 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/tests/utils/test_sleep.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 20:15:21.203121 shroomdk-2.0.3/shroomdk/utils/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/utils/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)     1966 2023-05-02 20:15:20.000000 shroomdk-2.0.3/shroomdk/utils/sleep.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 20:15:21.197713 shroomdk-2.0.3/shroomdk.egg-info/
--rw-r--r--   0 jim        (501) staff       (20)     1510 2023-05-02 20:15:21.000000 shroomdk-2.0.3/shroomdk.egg-info/PKG-INFO
--rw-r--r--   0 jim        (501) staff       (20)     4101 2023-05-02 20:15:21.000000 shroomdk-2.0.3/shroomdk.egg-info/SOURCES.txt
--rw-r--r--   0 jim        (501) staff       (20)        1 2023-05-02 20:15:21.000000 shroomdk-2.0.3/shroomdk.egg-info/dependency_links.txt
--rw-r--r--   0 jim        (501) staff       (20)       34 2023-05-02 20:15:21.000000 shroomdk-2.0.3/shroomdk.egg-info/requires.txt
--rw-r--r--   0 jim        (501) staff       (20)       13 2023-05-02 20:15:21.000000 shroomdk-2.0.3/shroomdk.egg-info/top_level.txt
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 20:15:21.194853 shroomdk-2.0.3/src/
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 20:15:21.203777 shroomdk-2.0.3/src/errors/
--rw-r--r--   0 jim        (501) staff       (20)      336 2023-05-02 18:10:35.000000 shroomdk-2.0.3/src/errors/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)     1583 2023-05-02 18:10:35.000000 shroomdk-2.0.3/src/errors/api_error.py
--rw-r--r--   0 jim        (501) staff       (20)      121 2023-05-02 18:10:35.000000 shroomdk-2.0.3/src/errors/base_error.py
--rw-r--r--   0 jim        (501) staff       (20)     2077 2023-05-02 18:10:35.000000 shroomdk-2.0.3/src/errors/query_run_errors.py
--rw-r--r--   0 jim        (501) staff       (20)      262 2023-05-02 18:10:35.000000 shroomdk-2.0.3/src/errors/sdk_error.py
--rw-r--r--   0 jim        (501) staff       (20)      361 2023-05-02 18:10:35.000000 shroomdk-2.0.3/src/errors/server_error.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 20:15:21.203894 shroomdk-2.0.3/src/integrations/
--rw-r--r--   0 jim        (501) staff       (20)       69 2023-05-02 18:10:35.000000 shroomdk-2.0.3/src/integrations/__init__.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 20:15:21.204326 shroomdk-2.0.3/src/integrations/query_integration/
--rw-r--r--   0 jim        (501) staff       (20)       77 2023-05-02 18:10:35.000000 shroomdk-2.0.3/src/integrations/query_integration/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)     9884 2023-05-02 18:10:35.000000 shroomdk-2.0.3/src/integrations/query_integration/compass_query_integration.py
--rw-r--r--   0 jim        (501) staff       (20)      237 2023-05-02 18:10:35.000000 shroomdk-2.0.3/src/integrations/query_integration/defaults.py
--rw-r--r--   0 jim        (501) staff       (20)     3570 2023-05-02 18:10:35.000000 shroomdk-2.0.3/src/integrations/query_integration/query_result_set_builder.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 20:15:21.205111 shroomdk-2.0.3/src/models/
--rw-r--r--   0 jim        (501) staff       (20)      365 2023-05-02 18:10:35.000000 shroomdk-2.0.3/src/models/__init__.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 20:15:21.208103 shroomdk-2.0.3/src/models/compass/
--rw-r--r--   0 jim        (501) staff       (20)       50 2023-05-02 18:10:35.000000 shroomdk-2.0.3/src/models/compass/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)      571 2023-05-02 18:10:35.000000 shroomdk-2.0.3/src/models/compass/cancel_query_run.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 20:15:21.210281 shroomdk-2.0.3/src/models/compass/core/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 shroomdk-2.0.3/src/models/compass/core/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)      187 2023-05-02 18:10:35.000000 shroomdk-2.0.3/src/models/compass/core/column_metadata.py
--rw-r--r--   0 jim        (501) staff       (20)      117 2023-05-02 18:10:35.000000 shroomdk-2.0.3/src/models/compass/core/page.py
--rw-r--r--   0 jim        (501) staff       (20)      183 2023-05-02 18:10:35.000000 shroomdk-2.0.3/src/models/compass/core/page_stats.py
--rw-r--r--   0 jim        (501) staff       (20)      358 2023-05-02 18:10:35.000000 shroomdk-2.0.3/src/models/compass/core/query_request.py
--rw-r--r--   0 jim        (501) staff       (20)      807 2023-05-02 18:10:35.000000 shroomdk-2.0.3/src/models/compass/core/query_run.py
--rw-r--r--   0 jim        (501) staff       (20)       89 2023-05-02 18:10:35.000000 shroomdk-2.0.3/src/models/compass/core/result_format.py
--rw-r--r--   0 jim        (501) staff       (20)      149 2023-05-02 18:10:35.000000 shroomdk-2.0.3/src/models/compass/core/rpc_error.py
--rw-r--r--   0 jim        (501) staff       (20)      198 2023-05-02 18:10:35.000000 shroomdk-2.0.3/src/models/compass/core/rpc_request.py
--rw-r--r--   0 jim        (501) staff       (20)      252 2023-05-02 18:10:35.000000 shroomdk-2.0.3/src/models/compass/core/rpc_response.py
--rw-r--r--   0 jim        (501) staff       (20)      340 2023-05-02 18:10:35.000000 shroomdk-2.0.3/src/models/compass/core/sql_statement.py
--rw-r--r--   0 jim        (501) staff       (20)      221 2023-05-02 18:10:35.000000 shroomdk-2.0.3/src/models/compass/core/tags.py
--rw-r--r--   0 jim        (501) staff       (20)      845 2023-05-02 18:10:35.000000 shroomdk-2.0.3/src/models/compass/create_query_run.py
--rw-r--r--   0 jim        (501) staff       (20)      639 2023-05-02 18:10:35.000000 shroomdk-2.0.3/src/models/compass/get_query_run.py
--rw-r--r--   0 jim        (501) staff       (20)     2026 2023-05-02 18:10:35.000000 shroomdk-2.0.3/src/models/compass/get_query_run_results.py
--rw-r--r--   0 jim        (501) staff       (20)      582 2023-05-02 18:10:35.000000 shroomdk-2.0.3/src/models/compass/get_sql_statement.py
--rw-r--r--   0 jim        (501) staff       (20)      852 2023-05-02 18:10:35.000000 shroomdk-2.0.3/src/models/compass/query_results.py
--rw-r--r--   0 jim        (501) staff       (20)     1422 2023-05-02 18:10:35.000000 shroomdk-2.0.3/src/models/query.py
--rw-r--r--   0 jim        (501) staff       (20)      836 2023-05-02 18:10:35.000000 shroomdk-2.0.3/src/models/query_defaults.py
--rw-r--r--   0 jim        (501) staff       (20)     1031 2023-05-02 18:10:35.000000 shroomdk-2.0.3/src/models/query_result_set.py
--rw-r--r--   0 jim        (501) staff       (20)     1658 2023-05-02 18:10:35.000000 shroomdk-2.0.3/src/models/query_run_stats.py
--rw-r--r--   0 jim        (501) staff       (20)      544 2023-05-02 18:10:35.000000 shroomdk-2.0.3/src/models/query_status.py
--rw-r--r--   0 jim        (501) staff       (20)      194 2023-05-02 18:10:35.000000 shroomdk-2.0.3/src/models/sleep_config.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 20:15:21.210653 shroomdk-2.0.3/src/tests/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 shroomdk-2.0.3/src/tests/__init__.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 20:15:21.210840 shroomdk-2.0.3/src/tests/integrations/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 shroomdk-2.0.3/src/tests/integrations/__init__.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 20:15:21.211345 shroomdk-2.0.3/src/tests/integrations/query_integration/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 shroomdk-2.0.3/src/tests/integrations/query_integration/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)     8712 2023-05-02 18:10:35.000000 shroomdk-2.0.3/src/tests/integrations/query_integration/test_query_compass_integration.py
--rw-r--r--   0 jim        (501) staff       (20)     3438 2023-05-02 18:10:35.000000 shroomdk-2.0.3/src/tests/integrations/query_integration/test_query_result_set_builder.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 20:15:21.211644 shroomdk-2.0.3/src/tests/models/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 shroomdk-2.0.3/src/tests/models/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)      931 2023-05-02 18:10:35.000000 shroomdk-2.0.3/src/tests/models/test_query_status.py
--rw-r--r--   0 jim        (501) staff       (20)     5218 2023-05-02 18:10:35.000000 shroomdk-2.0.3/src/tests/test_rpc.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 20:15:21.211952 shroomdk-2.0.3/src/tests/utils/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 shroomdk-2.0.3/src/tests/utils/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)     2242 2023-05-02 18:10:35.000000 shroomdk-2.0.3/src/tests/utils/test_sleep.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-02 20:15:21.212241 shroomdk-2.0.3/src/utils/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 shroomdk-2.0.3/src/utils/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)     1966 2023-05-02 18:10:35.000000 shroomdk-2.0.3/src/utils/sleep.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-08 14:20:04.609377 shroomdk-2.0.4/
+-rw-r--r--   0 jim        (501) staff       (20)     1073 2022-07-25 21:42:15.000000 shroomdk-2.0.4/LICENSE.txt
+-rw-r--r--   0 jim        (501) staff       (20)       69 2022-07-25 21:42:15.000000 shroomdk-2.0.4/MANIFEST.in
+-rw-r--r--   0 jim        (501) staff       (20)     1510 2023-05-08 14:20:04.609459 shroomdk-2.0.4/PKG-INFO
+-rw-r--r--   0 jim        (501) staff       (20)      709 2023-05-02 18:18:58.000000 shroomdk-2.0.4/README.md
+-rw-r--r--   0 jim        (501) staff       (20)        5 2023-05-08 14:18:06.000000 shroomdk-2.0.4/VERSION
+-rw-r--r--   0 jim        (501) staff       (20)       30 2022-07-25 21:42:15.000000 shroomdk-2.0.4/requirements-dev.txt
+-rw-r--r--   0 jim        (501) staff       (20)       33 2023-05-02 18:10:35.000000 shroomdk-2.0.4/requirements.txt
+-rw-r--r--   0 jim        (501) staff       (20)       79 2023-05-08 14:20:04.610061 shroomdk-2.0.4/setup.cfg
+-rw-r--r--   0 jim        (501) staff       (20)     1557 2023-05-02 18:10:35.000000 shroomdk-2.0.4/setup.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-08 14:20:04.574897 shroomdk-2.0.4/shroomdk/
+-rw-r--r--   0 jim        (501) staff       (20)      147 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/__init__.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-08 14:20:04.576531 shroomdk-2.0.4/shroomdk/errors/
+-rw-r--r--   0 jim        (501) staff       (20)      336 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/errors/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     1583 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/errors/api_error.py
+-rw-r--r--   0 jim        (501) staff       (20)      121 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/errors/base_error.py
+-rw-r--r--   0 jim        (501) staff       (20)     2077 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/errors/query_run_errors.py
+-rw-r--r--   0 jim        (501) staff       (20)      262 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/errors/sdk_error.py
+-rw-r--r--   0 jim        (501) staff       (20)      361 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/errors/server_error.py
+-rw-r--r--   0 jim        (501) staff       (20)     2982 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/flipside.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-08 14:20:04.576749 shroomdk-2.0.4/shroomdk/integrations/
+-rw-r--r--   0 jim        (501) staff       (20)       69 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/integrations/__init__.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-08 14:20:04.577286 shroomdk-2.0.4/shroomdk/integrations/query_integration/
+-rw-r--r--   0 jim        (501) staff       (20)       77 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/integrations/query_integration/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     9884 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/integrations/query_integration/compass_query_integration.py
+-rw-r--r--   0 jim        (501) staff       (20)      237 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/integrations/query_integration/defaults.py
+-rw-r--r--   0 jim        (501) staff       (20)     3570 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/integrations/query_integration/query_result_set_builder.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-08 14:20:04.578474 shroomdk-2.0.4/shroomdk/models/
+-rw-r--r--   0 jim        (501) staff       (20)      365 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/models/__init__.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-08 14:20:04.579245 shroomdk-2.0.4/shroomdk/models/compass/
+-rw-r--r--   0 jim        (501) staff       (20)       50 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/models/compass/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)      571 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/models/compass/cancel_query_run.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-08 14:20:04.580480 shroomdk-2.0.4/shroomdk/models/compass/core/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/models/compass/core/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)      187 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/models/compass/core/column_metadata.py
+-rw-r--r--   0 jim        (501) staff       (20)      117 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/models/compass/core/page.py
+-rw-r--r--   0 jim        (501) staff       (20)      183 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/models/compass/core/page_stats.py
+-rw-r--r--   0 jim        (501) staff       (20)      358 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/models/compass/core/query_request.py
+-rw-r--r--   0 jim        (501) staff       (20)      807 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/models/compass/core/query_run.py
+-rw-r--r--   0 jim        (501) staff       (20)       89 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/models/compass/core/result_format.py
+-rw-r--r--   0 jim        (501) staff       (20)      149 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/models/compass/core/rpc_error.py
+-rw-r--r--   0 jim        (501) staff       (20)      198 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/models/compass/core/rpc_request.py
+-rw-r--r--   0 jim        (501) staff       (20)      252 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/models/compass/core/rpc_response.py
+-rw-r--r--   0 jim        (501) staff       (20)      340 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/models/compass/core/sql_statement.py
+-rw-r--r--   0 jim        (501) staff       (20)      221 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/models/compass/core/tags.py
+-rw-r--r--   0 jim        (501) staff       (20)      845 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/models/compass/create_query_run.py
+-rw-r--r--   0 jim        (501) staff       (20)      639 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/models/compass/get_query_run.py
+-rw-r--r--   0 jim        (501) staff       (20)     2104 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/models/compass/get_query_run_results.py
+-rw-r--r--   0 jim        (501) staff       (20)      582 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/models/compass/get_sql_statement.py
+-rw-r--r--   0 jim        (501) staff       (20)      852 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/models/compass/query_results.py
+-rw-r--r--   0 jim        (501) staff       (20)     1422 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/models/query.py
+-rw-r--r--   0 jim        (501) staff       (20)      836 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/models/query_defaults.py
+-rw-r--r--   0 jim        (501) staff       (20)     1031 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/models/query_result_set.py
+-rw-r--r--   0 jim        (501) staff       (20)     1658 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/models/query_run_stats.py
+-rw-r--r--   0 jim        (501) staff       (20)      544 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/models/query_status.py
+-rw-r--r--   0 jim        (501) staff       (20)      194 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/models/sleep_config.py
+-rw-r--r--   0 jim        (501) staff       (20)     5898 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/rpc.py
+-rw-r--r--   0 jim        (501) staff       (20)       68 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/shroomdk.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-08 14:20:04.580664 shroomdk-2.0.4/shroomdk/tests/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/tests/__init__.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-08 14:20:04.580794 shroomdk-2.0.4/shroomdk/tests/integrations/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/tests/integrations/__init__.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-08 14:20:04.581100 shroomdk-2.0.4/shroomdk/tests/integrations/query_integration/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/tests/integrations/query_integration/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     8712 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/tests/integrations/query_integration/test_query_compass_integration.py
+-rw-r--r--   0 jim        (501) staff       (20)     3438 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/tests/integrations/query_integration/test_query_result_set_builder.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-08 14:20:04.581292 shroomdk-2.0.4/shroomdk/tests/models/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/tests/models/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)      931 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/tests/models/test_query_status.py
+-rw-r--r--   0 jim        (501) staff       (20)     5218 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/tests/test_rpc.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-08 14:20:04.582352 shroomdk-2.0.4/shroomdk/tests/utils/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/tests/utils/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     2242 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/tests/utils/test_sleep.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-08 14:20:04.583202 shroomdk-2.0.4/shroomdk/utils/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/utils/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     1966 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/utils/sleep.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-08 14:20:04.575633 shroomdk-2.0.4/shroomdk.egg-info/
+-rw-r--r--   0 jim        (501) staff       (20)     1510 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk.egg-info/PKG-INFO
+-rw-r--r--   0 jim        (501) staff       (20)     4101 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk.egg-info/SOURCES.txt
+-rw-r--r--   0 jim        (501) staff       (20)        1 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk.egg-info/dependency_links.txt
+-rw-r--r--   0 jim        (501) staff       (20)       34 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk.egg-info/requires.txt
+-rw-r--r--   0 jim        (501) staff       (20)       13 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk.egg-info/top_level.txt
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-08 14:20:04.572122 shroomdk-2.0.4/src/
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-08 14:20:04.584210 shroomdk-2.0.4/src/errors/
+-rw-r--r--   0 jim        (501) staff       (20)      336 2023-05-02 18:10:35.000000 shroomdk-2.0.4/src/errors/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     1583 2023-05-02 18:10:35.000000 shroomdk-2.0.4/src/errors/api_error.py
+-rw-r--r--   0 jim        (501) staff       (20)      121 2023-05-02 18:10:35.000000 shroomdk-2.0.4/src/errors/base_error.py
+-rw-r--r--   0 jim        (501) staff       (20)     2077 2023-05-02 18:10:35.000000 shroomdk-2.0.4/src/errors/query_run_errors.py
+-rw-r--r--   0 jim        (501) staff       (20)      262 2023-05-02 18:10:35.000000 shroomdk-2.0.4/src/errors/sdk_error.py
+-rw-r--r--   0 jim        (501) staff       (20)      361 2023-05-02 18:10:35.000000 shroomdk-2.0.4/src/errors/server_error.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-08 14:20:04.584329 shroomdk-2.0.4/src/integrations/
+-rw-r--r--   0 jim        (501) staff       (20)       69 2023-05-02 18:10:35.000000 shroomdk-2.0.4/src/integrations/__init__.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-08 14:20:04.585143 shroomdk-2.0.4/src/integrations/query_integration/
+-rw-r--r--   0 jim        (501) staff       (20)       77 2023-05-02 18:10:35.000000 shroomdk-2.0.4/src/integrations/query_integration/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     9884 2023-05-02 18:10:35.000000 shroomdk-2.0.4/src/integrations/query_integration/compass_query_integration.py
+-rw-r--r--   0 jim        (501) staff       (20)      237 2023-05-02 18:10:35.000000 shroomdk-2.0.4/src/integrations/query_integration/defaults.py
+-rw-r--r--   0 jim        (501) staff       (20)     3570 2023-05-02 18:10:35.000000 shroomdk-2.0.4/src/integrations/query_integration/query_result_set_builder.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-08 14:20:04.586716 shroomdk-2.0.4/src/models/
+-rw-r--r--   0 jim        (501) staff       (20)      365 2023-05-02 18:10:35.000000 shroomdk-2.0.4/src/models/__init__.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-08 14:20:04.594529 shroomdk-2.0.4/src/models/compass/
+-rw-r--r--   0 jim        (501) staff       (20)       50 2023-05-02 18:10:35.000000 shroomdk-2.0.4/src/models/compass/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)      571 2023-05-02 18:10:35.000000 shroomdk-2.0.4/src/models/compass/cancel_query_run.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-08 14:20:04.606954 shroomdk-2.0.4/src/models/compass/core/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 shroomdk-2.0.4/src/models/compass/core/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)      187 2023-05-02 18:10:35.000000 shroomdk-2.0.4/src/models/compass/core/column_metadata.py
+-rw-r--r--   0 jim        (501) staff       (20)      117 2023-05-02 18:10:35.000000 shroomdk-2.0.4/src/models/compass/core/page.py
+-rw-r--r--   0 jim        (501) staff       (20)      183 2023-05-02 18:10:35.000000 shroomdk-2.0.4/src/models/compass/core/page_stats.py
+-rw-r--r--   0 jim        (501) staff       (20)      358 2023-05-02 18:10:35.000000 shroomdk-2.0.4/src/models/compass/core/query_request.py
+-rw-r--r--   0 jim        (501) staff       (20)      807 2023-05-02 18:10:35.000000 shroomdk-2.0.4/src/models/compass/core/query_run.py
+-rw-r--r--   0 jim        (501) staff       (20)       89 2023-05-02 18:10:35.000000 shroomdk-2.0.4/src/models/compass/core/result_format.py
+-rw-r--r--   0 jim        (501) staff       (20)      149 2023-05-02 18:10:35.000000 shroomdk-2.0.4/src/models/compass/core/rpc_error.py
+-rw-r--r--   0 jim        (501) staff       (20)      198 2023-05-02 18:10:35.000000 shroomdk-2.0.4/src/models/compass/core/rpc_request.py
+-rw-r--r--   0 jim        (501) staff       (20)      252 2023-05-02 18:10:35.000000 shroomdk-2.0.4/src/models/compass/core/rpc_response.py
+-rw-r--r--   0 jim        (501) staff       (20)      340 2023-05-02 18:10:35.000000 shroomdk-2.0.4/src/models/compass/core/sql_statement.py
+-rw-r--r--   0 jim        (501) staff       (20)      221 2023-05-02 18:10:35.000000 shroomdk-2.0.4/src/models/compass/core/tags.py
+-rw-r--r--   0 jim        (501) staff       (20)      845 2023-05-02 18:10:35.000000 shroomdk-2.0.4/src/models/compass/create_query_run.py
+-rw-r--r--   0 jim        (501) staff       (20)      639 2023-05-02 18:10:35.000000 shroomdk-2.0.4/src/models/compass/get_query_run.py
+-rw-r--r--   0 jim        (501) staff       (20)     2104 2023-05-08 14:18:06.000000 shroomdk-2.0.4/src/models/compass/get_query_run_results.py
+-rw-r--r--   0 jim        (501) staff       (20)      582 2023-05-02 18:10:35.000000 shroomdk-2.0.4/src/models/compass/get_sql_statement.py
+-rw-r--r--   0 jim        (501) staff       (20)      852 2023-05-02 18:10:35.000000 shroomdk-2.0.4/src/models/compass/query_results.py
+-rw-r--r--   0 jim        (501) staff       (20)     1422 2023-05-02 18:10:35.000000 shroomdk-2.0.4/src/models/query.py
+-rw-r--r--   0 jim        (501) staff       (20)      836 2023-05-02 18:10:35.000000 shroomdk-2.0.4/src/models/query_defaults.py
+-rw-r--r--   0 jim        (501) staff       (20)     1031 2023-05-02 18:10:35.000000 shroomdk-2.0.4/src/models/query_result_set.py
+-rw-r--r--   0 jim        (501) staff       (20)     1658 2023-05-02 18:10:35.000000 shroomdk-2.0.4/src/models/query_run_stats.py
+-rw-r--r--   0 jim        (501) staff       (20)      544 2023-05-02 18:10:35.000000 shroomdk-2.0.4/src/models/query_status.py
+-rw-r--r--   0 jim        (501) staff       (20)      194 2023-05-02 18:10:35.000000 shroomdk-2.0.4/src/models/sleep_config.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-08 14:20:04.607497 shroomdk-2.0.4/src/tests/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 shroomdk-2.0.4/src/tests/__init__.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-08 14:20:04.607885 shroomdk-2.0.4/src/tests/integrations/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 shroomdk-2.0.4/src/tests/integrations/__init__.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-08 14:20:04.608473 shroomdk-2.0.4/src/tests/integrations/query_integration/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 shroomdk-2.0.4/src/tests/integrations/query_integration/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     8712 2023-05-02 18:10:35.000000 shroomdk-2.0.4/src/tests/integrations/query_integration/test_query_compass_integration.py
+-rw-r--r--   0 jim        (501) staff       (20)     3438 2023-05-02 18:10:35.000000 shroomdk-2.0.4/src/tests/integrations/query_integration/test_query_result_set_builder.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-08 14:20:04.608766 shroomdk-2.0.4/src/tests/models/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 shroomdk-2.0.4/src/tests/models/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)      931 2023-05-02 18:10:35.000000 shroomdk-2.0.4/src/tests/models/test_query_status.py
+-rw-r--r--   0 jim        (501) staff       (20)     5218 2023-05-02 18:10:35.000000 shroomdk-2.0.4/src/tests/test_rpc.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-08 14:20:04.609018 shroomdk-2.0.4/src/tests/utils/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 shroomdk-2.0.4/src/tests/utils/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     2242 2023-05-02 18:10:35.000000 shroomdk-2.0.4/src/tests/utils/test_sleep.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-08 14:20:04.609259 shroomdk-2.0.4/src/utils/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 shroomdk-2.0.4/src/utils/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     1966 2023-05-02 18:10:35.000000 shroomdk-2.0.4/src/utils/sleep.py
```

### Comparing `shroomdk-2.0.3/LICENSE.txt` & `shroomdk-2.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.3/PKG-INFO` & `shroomdk-2.0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shroomdk
-Version: 2.0.3
+Version: 2.0.4
 Summary: SDK by Flipside Crypto: Query the most reliable & comprehensive blockchain data in crypto
 Home-page: https://github.com/FlipsideCrypto/sdk/python
 Author: dev@flipsidecrypto.com
 Author-email: dev@flipsidecrypto.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `shroomdk-2.0.3/README.md` & `shroomdk-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.3/setup.py` & `shroomdk-2.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.3/shroomdk/errors/api_error.py` & `shroomdk-2.0.4/shroomdk/errors/api_error.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.3/shroomdk/errors/query_run_errors.py` & `shroomdk-2.0.4/shroomdk/errors/query_run_errors.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.3/shroomdk/flipside.py` & `shroomdk-2.0.4/shroomdk/flipside.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 from .models.compass.core.query_run import QueryRun
 from .models.compass.core.sql_statement import SqlStatement
 from .models.query_result_set import QueryResultSet
 from .rpc import RPC
 
 API_BASE_URL = "https://api-v2.flipsidecrypto.xyz"
 
-SDK_VERSION = "2.0.3"
+SDK_VERSION = "2.0.4"
 SDK_PACKAGE = "python"
 
 DEFAULT_DATA_SOURCE = "snowflake-default"
 DEFAULT_DATA_PROVIDER = "flipside"
-DEFAULT_PAGE_SIZE = 1000
+DEFAULT_PAGE_SIZE = 100000
 DEFAULT_PAGE_NUMBER = 1
 DEFAULT_TIMEOUT_MINUTES = 15
 DEFAULT_TTL_MINUTES = 60
 DEFAULT_MAX_AGE_MINUTES = 0
 
 
 class Flipside(object):
@@ -65,15 +65,15 @@
     def get_query_run(self, query_run_id: str) -> QueryRun:
         return self.query_integration.get_query_run(query_run_id)
 
     def get_query_results(
         self,
         query_run_id: str,
         page_number: int = 1,
-        page_size: int = 10000,
+        page_size: int = DEFAULT_PAGE_SIZE,
         filters: Optional[Union[List[Filter], None]] = [],
         sort_by: Optional[Union[List[SortBy], None]] = [],
     ) -> QueryResultSet:
         return self.query_integration.get_query_results(
             query_run_id,
             page_number=page_number,
             page_size=page_size,
```

### Comparing `shroomdk-2.0.3/shroomdk/integrations/query_integration/compass_query_integration.py` & `shroomdk-2.0.4/shroomdk/integrations/query_integration/compass_query_integration.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.3/shroomdk/integrations/query_integration/query_result_set_builder.py` & `shroomdk-2.0.4/shroomdk/integrations/query_integration/query_result_set_builder.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.3/shroomdk/models/compass/cancel_query_run.py` & `shroomdk-2.0.4/shroomdk/models/compass/cancel_query_run.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.3/shroomdk/models/compass/core/query_run.py` & `shroomdk-2.0.4/shroomdk/models/compass/core/query_run.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.3/shroomdk/models/compass/create_query_run.py` & `shroomdk-2.0.4/shroomdk/models/compass/create_query_run.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.3/shroomdk/models/compass/get_query_run.py` & `shroomdk-2.0.4/shroomdk/models/compass/get_query_run.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.3/shroomdk/models/compass/get_query_run_results.py` & `shroomdk-2.0.4/shroomdk/models/compass/get_query_run_results.py`

 * *Files 8% similar despite different names*

```diff
@@ -55,19 +55,19 @@
     def dict(self, *args, **kwargs) -> dict:
         kwargs.setdefault("exclude_none", True)  # Exclude keys with None values
         return super().dict(*args, **kwargs)
 
 
 # Response
 class GetQueryRunResultsRpcResult(BaseModel):
-    columnNames: Optional[List[str]]
-    columnTypes: Optional[List[str]]
-    rows: List[Any]
-    page: PageStats
-    sql: str
-    format: ResultFormat
+    columnNames: Union[Optional[List[str]], None]
+    columnTypes: Union[Optional[List[str]], None]
+    rows: Union[List[Any], None]
+    page: Union[PageStats, None]
+    sql: Union[str, None]
+    format: Union[ResultFormat, None]
     originalQueryRun: QueryRun
     redirectedToQueryRun: Union[QueryRun, None]
 
 
 class GetQueryRunResultsRpcResponse(RpcResponse):
     result: Union[GetQueryRunResultsRpcResult, None]
```

### Comparing `shroomdk-2.0.3/shroomdk/models/compass/get_sql_statement.py` & `shroomdk-2.0.4/shroomdk/models/compass/get_sql_statement.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.3/shroomdk/models/compass/query_results.py` & `shroomdk-2.0.4/shroomdk/models/compass/query_results.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.3/shroomdk/models/query.py` & `shroomdk-2.0.4/shroomdk/models/query.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.3/shroomdk/models/query_defaults.py` & `shroomdk-2.0.4/shroomdk/models/query_defaults.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.3/shroomdk/models/query_result_set.py` & `shroomdk-2.0.4/shroomdk/models/query_result_set.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.3/shroomdk/models/query_run_stats.py` & `shroomdk-2.0.4/shroomdk/models/query_run_stats.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.3/shroomdk/models/query_status.py` & `shroomdk-2.0.4/shroomdk/models/query_status.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.3/shroomdk/rpc.py` & `shroomdk-2.0.4/shroomdk/rpc.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.3/shroomdk/tests/integrations/query_integration/test_query_compass_integration.py` & `shroomdk-2.0.4/shroomdk/tests/integrations/query_integration/test_query_compass_integration.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.3/shroomdk/tests/integrations/query_integration/test_query_result_set_builder.py` & `shroomdk-2.0.4/shroomdk/tests/integrations/query_integration/test_query_result_set_builder.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.3/shroomdk/tests/models/test_query_status.py` & `shroomdk-2.0.4/shroomdk/tests/models/test_query_status.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.3/shroomdk/tests/test_rpc.py` & `shroomdk-2.0.4/shroomdk/tests/test_rpc.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.3/shroomdk/tests/utils/test_sleep.py` & `shroomdk-2.0.4/shroomdk/tests/utils/test_sleep.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.3/shroomdk/utils/sleep.py` & `shroomdk-2.0.4/shroomdk/utils/sleep.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.3/shroomdk.egg-info/PKG-INFO` & `shroomdk-2.0.4/shroomdk.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shroomdk
-Version: 2.0.3
+Version: 2.0.4
 Summary: SDK by Flipside Crypto: Query the most reliable & comprehensive blockchain data in crypto
 Home-page: https://github.com/FlipsideCrypto/sdk/python
 Author: dev@flipsidecrypto.com
 Author-email: dev@flipsidecrypto.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `shroomdk-2.0.3/shroomdk.egg-info/SOURCES.txt` & `shroomdk-2.0.4/shroomdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.3/src/errors/api_error.py` & `shroomdk-2.0.4/src/errors/api_error.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.3/src/errors/query_run_errors.py` & `shroomdk-2.0.4/src/errors/query_run_errors.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.3/src/integrations/query_integration/compass_query_integration.py` & `shroomdk-2.0.4/src/integrations/query_integration/compass_query_integration.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.3/src/integrations/query_integration/query_result_set_builder.py` & `shroomdk-2.0.4/src/integrations/query_integration/query_result_set_builder.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.3/src/models/compass/cancel_query_run.py` & `shroomdk-2.0.4/src/models/compass/cancel_query_run.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.3/src/models/compass/core/query_run.py` & `shroomdk-2.0.4/src/models/compass/core/query_run.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.3/src/models/compass/create_query_run.py` & `shroomdk-2.0.4/src/models/compass/create_query_run.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.3/src/models/compass/get_query_run.py` & `shroomdk-2.0.4/src/models/compass/get_query_run.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.3/src/models/compass/get_query_run_results.py` & `shroomdk-2.0.4/src/models/compass/get_query_run_results.py`

 * *Files 8% similar despite different names*

```diff
@@ -55,19 +55,19 @@
     def dict(self, *args, **kwargs) -> dict:
         kwargs.setdefault("exclude_none", True)  # Exclude keys with None values
         return super().dict(*args, **kwargs)
 
 
 # Response
 class GetQueryRunResultsRpcResult(BaseModel):
-    columnNames: Optional[List[str]]
-    columnTypes: Optional[List[str]]
-    rows: List[Any]
-    page: PageStats
-    sql: str
-    format: ResultFormat
+    columnNames: Union[Optional[List[str]], None]
+    columnTypes: Union[Optional[List[str]], None]
+    rows: Union[List[Any], None]
+    page: Union[PageStats, None]
+    sql: Union[str, None]
+    format: Union[ResultFormat, None]
     originalQueryRun: QueryRun
     redirectedToQueryRun: Union[QueryRun, None]
 
 
 class GetQueryRunResultsRpcResponse(RpcResponse):
     result: Union[GetQueryRunResultsRpcResult, None]
```

### Comparing `shroomdk-2.0.3/src/models/compass/get_sql_statement.py` & `shroomdk-2.0.4/src/models/compass/get_sql_statement.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.3/src/models/compass/query_results.py` & `shroomdk-2.0.4/src/models/compass/query_results.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.3/src/models/query.py` & `shroomdk-2.0.4/src/models/query.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.3/src/models/query_defaults.py` & `shroomdk-2.0.4/src/models/query_defaults.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.3/src/models/query_result_set.py` & `shroomdk-2.0.4/src/models/query_result_set.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.3/src/models/query_run_stats.py` & `shroomdk-2.0.4/src/models/query_run_stats.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.3/src/models/query_status.py` & `shroomdk-2.0.4/src/models/query_status.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.3/src/tests/integrations/query_integration/test_query_compass_integration.py` & `shroomdk-2.0.4/src/tests/integrations/query_integration/test_query_compass_integration.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.3/src/tests/integrations/query_integration/test_query_result_set_builder.py` & `shroomdk-2.0.4/src/tests/integrations/query_integration/test_query_result_set_builder.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.3/src/tests/models/test_query_status.py` & `shroomdk-2.0.4/src/tests/models/test_query_status.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.3/src/tests/test_rpc.py` & `shroomdk-2.0.4/src/tests/test_rpc.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.3/src/tests/utils/test_sleep.py` & `shroomdk-2.0.4/src/tests/utils/test_sleep.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.3/src/utils/sleep.py` & `shroomdk-2.0.4/src/utils/sleep.py`

 * *Files identical despite different names*

