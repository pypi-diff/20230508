# Comparing `tmp/easy_sql-easy_sql-0.5.1.tar.gz` & `tmp/easy_sql_easy_sql-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_sql-easy_sql-0.5.1.tar", max compression
+gzip compressed data, was "easy_sql_easy_sql-1.0.0.tar", max compression
```

## Comparing `easy_sql-easy_sql-0.5.1.tar` & `easy_sql_easy_sql-1.0.0.tar`

### file list

```diff
@@ -1,74 +1,82 @@
--rw-r--r--   0        0        0    11357 2022-04-22 14:23:23.313923 easy_sql-easy_sql-0.5.1/LICENSE
--rw-r--r--   0        0        0     9499 2022-11-11 02:24:58.645763 easy_sql-easy_sql-0.5.1/README.md
--rw-r--r--   0        0        0        0 2022-04-23 03:40:24.904041 easy_sql-easy_sql-0.5.1/easy_sql/__init__.py
--rw-r--r--   0        0        0     2886 2022-09-14 12:50:12.409249 easy_sql-easy_sql-0.5.1/easy_sql/base_test.py
--rw-r--r--   0        0        0        0 2022-09-14 05:51:17.793495 easy_sql-easy_sql-0.5.1/easy_sql/cli/__init__.py
--rw-r--r--   0        0        0    10034 2022-09-14 13:17:13.257444 easy_sql-easy_sql-0.5.1/easy_sql/cli/backend_processor.py
--rw-r--r--   0        0        0    14870 2022-09-14 15:23:36.141055 easy_sql-easy_sql-0.5.1/easy_sql/cli/sql_config.py
--rw-r--r--   0        0        0     2764 2022-09-14 12:11:41.390400 easy_sql-easy_sql-0.5.1/easy_sql/cli/sql_config_test.py
--rw-r--r--   0        0        0     2159 2022-09-14 12:11:41.392211 easy_sql-easy_sql-0.5.1/easy_sql/data_process.py
--rw-r--r--   0        0        0     1040 2022-09-14 12:12:04.051117 easy_sql-easy_sql-0.5.1/easy_sql/data_process_itest.py
--rw-r--r--   0        0        0     2779 2022-09-14 12:34:52.816444 easy_sql-easy_sql-0.5.1/easy_sql/data_process_test.py
--rw-r--r--   0        0        0     2531 2022-08-29 02:25:19.887986 easy_sql-easy_sql-0.5.1/easy_sql/local_spark.py
--rw-r--r--   0        0        0     1360 2022-08-29 02:40:49.407540 easy_sql-easy_sql-0.5.1/easy_sql/logger.py
--rw-r--r--   0        0        0     3048 2022-08-17 07:45:00.123778 easy_sql-easy_sql-0.5.1/easy_sql/report.py
--rw-r--r--   0        0        0      337 2022-08-17 07:45:00.124376 easy_sql-easy_sql-0.5.1/easy_sql/report_test.py
--rw-r--r--   0        0        0     3054 2022-08-29 02:42:02.240881 easy_sql-easy_sql-0.5.1/easy_sql/spark_optimizer.py
--rw-r--r--   0        0        0        0 2022-06-14 02:56:45.155624 easy_sql-easy_sql-0.5.1/easy_sql/sql_linter/__init__.py
--rw-r--r--   0        0        0      106 2022-08-29 04:07:49.185717 easy_sql-easy_sql-0.5.1/easy_sql/sql_linter/rules/__init__.py
--rw-r--r--   0        0        0     1219 2022-08-18 23:35:40.053307 easy_sql-easy_sql-0.5.1/easy_sql/sql_linter/rules/bq_schema_rule.py
--rw-r--r--   0        0        0    10540 2022-09-07 13:18:07.773264 easy_sql-easy_sql-0.5.1/easy_sql/sql_linter/sql_linter.py
--rw-r--r--   0        0        0     4323 2022-08-30 00:33:19.801830 easy_sql-easy_sql-0.5.1/easy_sql/sql_linter/sql_linter_cli.py
--rw-r--r--   0        0        0     2605 2022-08-29 04:07:04.669377 easy_sql-easy_sql-0.5.1/easy_sql/sql_linter/sql_linter_reportor.py
--rw-r--r--   0        0        0     6987 2022-08-17 07:45:00.128801 easy_sql-easy_sql-0.5.1/easy_sql/sql_linter/sql_linter_test.py
--rw-r--r--   0        0        0      620 2022-08-17 07:45:00.130001 easy_sql-easy_sql-0.5.1/easy_sql/sql_processor/__init__.py
--rw-r--r--   0        0        0       62 2022-09-07 13:18:07.774188 easy_sql-easy_sql-0.5.1/easy_sql/sql_processor/backend/__init__.py
--rw-r--r--   0        0        0     6889 2022-09-07 13:18:07.775319 easy_sql-easy_sql-0.5.1/easy_sql/sql_processor/backend/base.py
--rw-r--r--   0        0        0      192 2022-08-17 07:45:00.132107 easy_sql-easy_sql-0.5.1/easy_sql/sql_processor/backend/bigquery.py
--rw-r--r--   0        0        0      168 2022-08-17 07:45:00.132389 easy_sql-easy_sql-0.5.1/easy_sql/sql_processor/backend/clickhouse.py
--rw-r--r--   0        0        0    10246 2022-09-13 14:28:14.038789 easy_sql-easy_sql-0.5.1/easy_sql/sql_processor/backend/flink.py
--rw-r--r--   0        0        0    16114 2022-09-14 12:46:37.438887 easy_sql-easy_sql-0.5.1/easy_sql/sql_processor/backend/flink_itest.py
--rw-r--r--   0        0        0    11575 2022-08-29 02:31:59.543949 easy_sql-easy_sql-0.5.1/easy_sql/sql_processor/backend/maxcompute.py
--rw-r--r--   0        0        0    11026 2022-08-29 03:52:42.340508 easy_sql-easy_sql-0.5.1/easy_sql/sql_processor/backend/maxcompute_itest.py
--rw-r--r--   0        0        0      180 2022-08-17 07:45:00.134919 easy_sql-easy_sql-0.5.1/easy_sql/sql_processor/backend/postgres.py
--rw-r--r--   0        0        0    36490 2022-10-15 07:26:33.369425 easy_sql-easy_sql-0.5.1/easy_sql/sql_processor/backend/rdb.py
--rw-r--r--   0        0        0    21988 2022-10-15 01:24:27.501261 easy_sql-easy_sql-0.5.1/easy_sql/sql_processor/backend/rdb_itest.py
--rw-r--r--   0        0        0     1941 2022-08-29 05:22:24.301012 easy_sql-easy_sql-0.5.1/easy_sql/sql_processor/backend/rdb_test.py
--rw-r--r--   0        0        0    10767 2022-08-29 03:54:25.935497 easy_sql-easy_sql-0.5.1/easy_sql/sql_processor/backend/spark.py
--rw-r--r--   0        0        0     1379 2022-08-17 07:45:00.141079 easy_sql-easy_sql-0.5.1/easy_sql/sql_processor/backend/spark_test.py
--rw-r--r--   0        0        0     7500 2022-08-29 04:29:43.612914 easy_sql-easy_sql-0.5.1/easy_sql/sql_processor/backend/sql_dialect/__init__.py
--rw-r--r--   0        0        0     9455 2022-08-29 03:14:16.880674 easy_sql-easy_sql-0.5.1/easy_sql/sql_processor/backend/sql_dialect/bigquery.py
--rw-r--r--   0        0        0     9286 2022-08-29 03:57:06.672668 easy_sql-easy_sql-0.5.1/easy_sql/sql_processor/backend/sql_dialect/clickhouse.py
--rw-r--r--   0        0        0      811 2022-09-07 13:18:07.776164 easy_sql-easy_sql-0.5.1/easy_sql/sql_processor/backend/sql_dialect/clickhouse_test.py
--rw-r--r--   0        0        0    10484 2022-08-29 03:58:39.962626 easy_sql-easy_sql-0.5.1/easy_sql/sql_processor/backend/sql_dialect/postgres.py
--rw-r--r--   0        0        0      900 2022-08-18 23:35:40.057886 easy_sql-easy_sql-0.5.1/easy_sql/sql_processor/common.py
--rw-r--r--   0        0        0    11916 2022-10-27 09:26:28.492366 easy_sql-easy_sql-0.5.1/easy_sql/sql_processor/context.py
--rw-r--r--   0        0        0     5924 2022-11-11 02:02:02.969207 easy_sql-easy_sql-0.5.1/easy_sql/sql_processor/context_test.py
--rw-r--r--   0        0        0     8375 2022-11-04 12:19:10.962359 easy_sql-easy_sql-0.5.1/easy_sql/sql_processor/funcs.py
--rw-r--r--   0        0        0    17894 2022-11-04 10:00:01.063786 easy_sql-easy_sql-0.5.1/easy_sql/sql_processor/funcs_common.py
--rw-r--r--   0        0        0     9324 2022-10-17 12:08:36.368975 easy_sql-easy_sql-0.5.1/easy_sql/sql_processor/funcs_itest.py
--rw-r--r--   0        0        0    11433 2022-10-18 10:31:49.276234 easy_sql-easy_sql-0.5.1/easy_sql/sql_processor/funcs_rdb.py
--rw-r--r--   0        0        0     7632 2022-10-14 11:12:50.516630 easy_sql-easy_sql-0.5.1/easy_sql/sql_processor/funcs_spark.py
--rw-r--r--   0        0        0     5545 2022-09-07 13:18:07.776468 easy_sql-easy_sql-0.5.1/easy_sql/sql_processor/report.py
--rw-r--r--   0        0        0     5498 2022-09-07 13:18:07.777279 easy_sql-easy_sql-0.5.1/easy_sql/sql_processor/sql_processor.py
--rw-r--r--   0        0        0    22460 2022-10-28 05:58:35.006880 easy_sql-easy_sql-0.5.1/easy_sql/sql_processor/step.py
--rw-r--r--   0        0        0     1480 2022-08-29 05:14:36.085682 easy_sql-easy_sql-0.5.1/easy_sql/sql_processor/step_test.py
--rw-r--r--   0        0        0     7351 2022-08-29 02:42:40.258055 easy_sql-easy_sql-0.5.1/easy_sql/sql_processor_debugger.py
--rw-r--r--   0        0        0     6944 2022-08-18 23:35:40.060796 easy_sql-easy_sql-0.5.1/easy_sql/sql_processor_debugger_itest.py
--rw-r--r--   0        0        0     6769 2022-08-17 07:45:00.156852 easy_sql-easy_sql-0.5.1/easy_sql/sql_processor_itest.py
--rw-r--r--   0        0        0    20564 2022-08-29 02:47:04.971764 easy_sql-easy_sql-0.5.1/easy_sql/sql_processor_test.py
--rw-r--r--   0        0        0     5061 2022-08-29 05:47:59.209126 easy_sql-easy_sql-0.5.1/easy_sql/sql_test.py
--rw-r--r--   0        0        0      583 2022-08-17 07:45:00.159984 easy_sql-easy_sql-0.5.1/easy_sql/sql_test_itest.py
--rw-r--r--   0        0        0    44413 2022-08-29 05:41:42.961737 easy_sql-easy_sql-0.5.1/easy_sql/sql_tester.py
--rw-r--r--   0        0        0     5383 2022-08-25 03:00:15.924067 easy_sql-easy_sql-0.5.1/easy_sql/sql_tester_test.py
--rw-r--r--   0        0        0        0 2022-04-23 03:40:25.188388 easy_sql-easy_sql-0.5.1/easy_sql/udf/__init__.py
--rw-r--r--   0        0        0      495 2022-08-29 02:50:15.216512 easy_sql-easy_sql-0.5.1/easy_sql/udf/check.py
--rw-r--r--   0        0        0     3211 2022-08-29 02:51:07.249396 easy_sql-easy_sql-0.5.1/easy_sql/udf/udfs.py
--rw-r--r--   0        0        0     2847 2022-08-17 07:45:00.162793 easy_sql-easy_sql-0.5.1/easy_sql/udf/udfs_test.py
--rw-r--r--   0        0        0        0 2022-04-23 03:40:25.223066 easy_sql-easy_sql-0.5.1/easy_sql/utils/__init__.py
--rw-r--r--   0        0        0     1545 2022-09-14 13:07:40.041460 easy_sql-easy_sql-0.5.1/easy_sql/utils/io_utils.py
--rw-r--r--   0        0        0      455 2022-08-17 07:45:00.163692 easy_sql-easy_sql-0.5.1/easy_sql/utils/object_utils.py
--rw-r--r--   0        0        0      550 2022-08-18 23:35:40.062565 easy_sql-easy_sql-0.5.1/easy_sql/utils/object_utils_test.py
--rw-r--r--   0        0        0     2063 2022-11-11 02:25:54.842427 easy_sql-easy_sql-0.5.1/pyproject.toml
--rw-r--r--   0        0        0    11127 2022-11-11 02:51:43.013013 easy_sql-easy_sql-0.5.1/setup.py
--rw-r--r--   0        0        0    11191 2022-11-11 02:51:43.013859 easy_sql-easy_sql-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-08 01:51:58.192164 easy_sql_easy_sql-1.0.0/LICENSE
+-rw-r--r--   0        0        0     9499 2023-05-08 01:51:58.192164 easy_sql_easy_sql-1.0.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/__init__.py
+-rw-r--r--   0        0        0     2886 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/base_test.py
+-rw-r--r--   0        0        0        0 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/cli/__init__.py
+-rw-r--r--   0        0        0     8595 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/cli/backend_processor.py
+-rw-r--r--   0        0        0    14198 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/config/sql_config.py
+-rw-r--r--   0        0        0     4296 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/config/sql_config_test.py
+-rw-r--r--   0        0        0     2165 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/data_process.py
+-rw-r--r--   0        0        0     1040 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/data_process_itest.py
+-rw-r--r--   0        0        0     2779 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/data_process_test.py
+-rw-r--r--   0        0        0     2531 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/local_spark.py
+-rw-r--r--   0        0        0     1360 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/logger.py
+-rw-r--r--   0        0        0     3048 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/report.py
+-rw-r--r--   0        0        0      337 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/report_test.py
+-rw-r--r--   0        0        0     3054 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/spark_optimizer.py
+-rw-r--r--   0        0        0        0 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/sql_linter/__init__.py
+-rw-r--r--   0        0        0      106 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/sql_linter/rules/__init__.py
+-rw-r--r--   0        0        0     1430 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/sql_linter/rules/bq_schema_rule.py
+-rw-r--r--   0        0        0    10316 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/sql_linter/sql_linter.py
+-rw-r--r--   0        0        0     4323 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/sql_linter/sql_linter_cli.py
+-rw-r--r--   0        0        0     2605 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/sql_linter/sql_linter_reportor.py
+-rw-r--r--   0        0        0     6979 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/sql_linter/sql_linter_test.py
+-rw-r--r--   0        0        0      620 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/__init__.py
+-rw-r--r--   0        0        0       62 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/backend/__init__.py
+-rw-r--r--   0        0        0     7036 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/backend/base.py
+-rw-r--r--   0        0        0      192 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/backend/bigquery.py
+-rw-r--r--   0        0        0      168 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/backend/clickhouse.py
+-rw-r--r--   0        0        0    15746 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/backend/flink.py
+-rw-r--r--   0        0        0    16114 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/backend/flink_itest.py
+-rw-r--r--   0        0        0     1498 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/backend/flink_test.py
+-rw-r--r--   0        0        0    11575 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/backend/maxcompute.py
+-rw-r--r--   0        0        0    11026 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/backend/maxcompute_itest.py
+-rw-r--r--   0        0        0      180 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/backend/postgres.py
+-rw-r--r--   0        0        0    36959 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/backend/rdb.py
+-rw-r--r--   0        0        0    22096 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/backend/rdb_itest.py
+-rw-r--r--   0        0        0     1941 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/backend/rdb_test.py
+-rw-r--r--   0        0        0    11086 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/backend/spark.py
+-rw-r--r--   0        0        0     1379 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/backend/spark_test.py
+-rw-r--r--   0        0        0     7500 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/backend/sql_dialect/__init__.py
+-rw-r--r--   0        0        0     9455 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/backend/sql_dialect/bigquery.py
+-rw-r--r--   0        0        0     9286 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/backend/sql_dialect/clickhouse.py
+-rw-r--r--   0        0        0      811 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/backend/sql_dialect/clickhouse_test.py
+-rw-r--r--   0        0        0    10484 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/backend/sql_dialect/postgres.py
+-rw-r--r--   0        0        0      900 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/common.py
+-rw-r--r--   0        0        0     7408 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/context.py
+-rw-r--r--   0        0        0     2177 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/context_test.py
+-rw-r--r--   0        0        0    11013 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/funcs.py
+-rw-r--r--   0        0        0    19985 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/funcs_common.py
+-rw-r--r--   0        0        0     3832 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/funcs_flink.py
+-rw-r--r--   0        0        0     3099 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/funcs_flink_itest.py
+-rw-r--r--   0        0        0     9704 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/funcs_itest.py
+-rw-r--r--   0        0        0    11492 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/funcs_rdb.py
+-rw-r--r--   0        0        0     8150 2023-05-08 01:51:58.212165 easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/funcs_spark.py
+-rw-r--r--   0        0        0     5545 2023-05-08 01:51:58.216165 easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/report.py
+-rw-r--r--   0        0        0     6149 2023-05-08 01:51:58.216165 easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/sql_processor.py
+-rw-r--r--   0        0        0    27013 2023-05-08 01:51:58.216165 easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/step.py
+-rw-r--r--   0        0        0     2400 2023-05-08 01:51:58.216165 easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/step_test.py
+-rw-r--r--   0        0        0     7351 2023-05-08 01:51:58.216165 easy_sql_easy_sql-1.0.0/easy_sql/sql_processor_debugger.py
+-rw-r--r--   0        0        0     6944 2023-05-08 01:51:58.216165 easy_sql_easy_sql-1.0.0/easy_sql/sql_processor_debugger_itest.py
+-rw-r--r--   0        0        0     6769 2023-05-08 01:51:58.216165 easy_sql_easy_sql-1.0.0/easy_sql/sql_processor_itest.py
+-rw-r--r--   0        0        0    20906 2023-05-08 01:51:58.216165 easy_sql_easy_sql-1.0.0/easy_sql/sql_processor_test.py
+-rw-r--r--   0        0        0     5061 2023-05-08 01:51:58.216165 easy_sql_easy_sql-1.0.0/easy_sql/sql_test.py
+-rw-r--r--   0        0        0      583 2023-05-08 01:51:58.216165 easy_sql_easy_sql-1.0.0/easy_sql/sql_test_itest.py
+-rw-r--r--   0        0        0    45124 2023-05-08 01:51:58.216165 easy_sql_easy_sql-1.0.0/easy_sql/sql_tester.py
+-rw-r--r--   0        0        0     5383 2023-05-08 01:51:58.216165 easy_sql_easy_sql-1.0.0/easy_sql/sql_tester_test.py
+-rw-r--r--   0        0        0        0 2023-05-08 01:51:58.216165 easy_sql_easy_sql-1.0.0/easy_sql/udf/__init__.py
+-rw-r--r--   0        0        0      495 2023-05-08 01:51:58.216165 easy_sql_easy_sql-1.0.0/easy_sql/udf/check.py
+-rw-r--r--   0        0        0     3211 2023-05-08 01:51:58.216165 easy_sql_easy_sql-1.0.0/easy_sql/udf/udfs.py
+-rw-r--r--   0        0        0     2847 2023-05-08 01:51:58.216165 easy_sql_easy_sql-1.0.0/easy_sql/udf/udfs_test.py
+-rw-r--r--   0        0        0        0 2023-05-08 01:51:58.216165 easy_sql_easy_sql-1.0.0/easy_sql/utils/__init__.py
+-rw-r--r--   0        0        0     1664 2023-05-08 01:51:58.216165 easy_sql_easy_sql-1.0.0/easy_sql/utils/db_connection_utils.py
+-rw-r--r--   0        0        0     1945 2023-05-08 01:51:58.216165 easy_sql_easy_sql-1.0.0/easy_sql/utils/flink_test_cluster.py
+-rw-r--r--   0        0        0      491 2023-05-08 01:51:58.216165 easy_sql_easy_sql-1.0.0/easy_sql/utils/flink_test_cluster_itest.py
+-rw-r--r--   0        0        0     1911 2023-05-08 01:51:58.216165 easy_sql_easy_sql-1.0.0/easy_sql/utils/io_utils.py
+-rw-r--r--   0        0        0     1241 2023-05-08 01:51:58.216165 easy_sql_easy_sql-1.0.0/easy_sql/utils/kv.py
+-rw-r--r--   0        0        0      455 2023-05-08 01:51:58.216165 easy_sql_easy_sql-1.0.0/easy_sql/utils/object_utils.py
+-rw-r--r--   0        0        0      550 2023-05-08 01:51:58.216165 easy_sql_easy_sql-1.0.0/easy_sql/utils/object_utils_test.py
+-rw-r--r--   0        0        0     5258 2023-05-08 01:51:58.216165 easy_sql_easy_sql-1.0.0/easy_sql/utils/sql_expr.py
+-rw-r--r--   0        0        0     5857 2023-05-08 01:51:58.216165 easy_sql_easy_sql-1.0.0/easy_sql/utils/sql_expr_test.py
+-rw-r--r--   0        0        0     2063 2023-05-08 01:52:22.861510 easy_sql_easy_sql-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0    11302 1970-01-01 00:00:00.000000 easy_sql_easy_sql-1.0.0/PKG-INFO
```

### Comparing `easy_sql-easy_sql-0.5.1/LICENSE` & `easy_sql_easy_sql-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `easy_sql-easy_sql-0.5.1/README.md` & `easy_sql_easy_sql-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `easy_sql-easy_sql-0.5.1/easy_sql/base_test.py` & `easy_sql_easy_sql-1.0.0/easy_sql/base_test.py`

 * *Files identical despite different names*

### Comparing `easy_sql-easy_sql-0.5.1/easy_sql/cli/backend_processor.py` & `easy_sql_easy_sql-1.0.0/easy_sql/cli/backend_processor.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 from __future__ import annotations
 
 import os
-from typing import TYPE_CHECKING, Any, Dict, List, Optional
+from typing import Any, Dict, List, Optional
 
-from easy_sql.cli.sql_config import (
-    KV,
+from easy_sql.config.sql_config import (
     EasySqlConfig,
     FlinkBackendConfig,
     SparkBackendConfig,
     parse_vars,
 )
 from easy_sql.logger import logger
 from easy_sql.sql_processor import SqlProcessor
 from easy_sql.sql_processor.backend import Backend
 
-if TYPE_CHECKING:
-    from sqlalchemy.engine.base import Connection, Engine
-
 
 class BackendProcessor:
     def __init__(self, config: EasySqlConfig) -> None:
         self.config = config
 
     @staticmethod
     def create_backend_processor(config: EasySqlConfig) -> BackendProcessor:
@@ -65,20 +61,20 @@
 
     def _exec_prepare_sql(self, backend: Backend, prepare_sql: str):
         return backend.exec_native_sql(prepare_sql)
 
     def _run_with_vars(self, backend: Backend, variables: Dict[str, Any], dry_run: bool):
         config = self.config
         sql_processor = SqlProcessor(
-            backend, config.sql, variables=variables, scala_udf_initializer=config.scala_udf_initializer
+            backend, config.sql, variables=variables, scala_udf_initializer=config.scala_udf_initializer, config=config
         )
-        if config.udf_file_path:
-            sql_processor.register_udfs_from_pyfile(config.udf_file_path)
-        if config.func_file_path:
-            sql_processor.register_funcs_from_pyfile(config.func_file_path)
+        if config.resolved_udf_file_path:
+            sql_processor.register_udfs_from_pyfile(config.resolved_udf_file_path)
+        if config.resolved_func_file_path:
+            sql_processor.register_funcs_from_pyfile(config.resolved_func_file_path)
 
         sql_processor.run(dry_run=dry_run)
 
 
 class SparkBackendProcessor(BackendProcessor):
     def __init__(self, config: EasySqlConfig) -> None:
         super().__init__(config)
@@ -124,69 +120,45 @@
             f'{config.flink} run {" ".join(config.flink_conf_command_args())} '
             f'--python "{entry_file}" '
             f"-f {self.config.sql_file} --dry-run {dry_run_arg} "
             f'{"-v " + vars_arg if vars_arg else ""} '
         )
 
     def _create_backend(self, backend_config: Optional[List[str]]) -> Backend:
-        from easy_sql.sql_processor.backend import FlinkBackend
+        from easy_sql.sql_processor.backend import FlinkBackend, FlinkTablesConfig
 
-        backend = FlinkBackend(self.config.is_batch)
         config = FlinkBackendConfig(self.config, backend_config)
+        backend = FlinkBackend(
+            self.config.is_batch, flink_tables_config=FlinkTablesConfig.from_config_file(config.flink_tables_file_path)
+        )
 
         logger.info(f"Using flink configurations: {config.flink_configurations}")
         backend.set_configurations(config.flink_configurations)
 
-        if config.flink_tables_file_path:
-            backend.register_tables(config.flink_tables_file_path, self.config.tables)
-            if self.config.tables:
-                conn = self.get_conn_from(config.flink_tables_file_path, backend, self.config.tables[0])
+        backend.register_tables(self.config.tables)
+        if self.config.tables:
+            conn = None
+            for table in self.config.tables:
+                from easy_sql.utils import db_connection_utils
+
+                conn = db_connection_utils.get_table_raw_conn_for_flink_backend(backend, table)
                 if conn:
-                    from easy_sql.sql_processor.backend.rdb import _exec_sql
+                    break
+            if conn:
+                from easy_sql.sql_processor.backend.rdb import _exec_sql
 
-                    self._exec_sql = lambda sql: _exec_sql(conn, sql)
+                self._exec_sql = lambda sql: _exec_sql(conn, sql)
 
         return backend
 
     def _exec_prepare_sql(self, backend: Backend, prepare_sql: str):
         if self._exec_sql:
             self._exec_sql(prepare_sql)
         else:
-            logger.warn(
-                "Cannot execute prepare-sql: the connector is not configured or with no supported. Will skip this."
-            )
-
-    def get_conn_from(self, flink_tables_file_path: str, backend: Backend, table: str):
-        from easy_sql.sql_processor.backend import FlinkBackend
-
-        def retrieve_jdbc_url_from(flink_tables_file_path: str, backend: FlinkBackend, table: str):
-            if table and flink_tables_file_path and os.path.exists(flink_tables_file_path):
-                with open(flink_tables_file_path, "r") as f:
-                    import json
-
-                    config = json.loads(f.read())
-                    _, _, connector = backend.get_table_config_and_connector(config, table)
-                    if connector and connector["options"]["connector"] == "jdbc":
-                        base_url = connector["options"]["url"]
-                        username = connector["options"]["username"]
-                        password = connector["options"]["password"]
-                        split_expr = "://"
-                        split_expr_index = base_url.index(split_expr)
-                        db_type = base_url[len("jdbc:") : split_expr_index]
-                        url = f"{db_type}{split_expr}{username}:{password}@{KV.from_config(base_url, split_expr).v}"
-                        return url
-
-        assert isinstance(backend, FlinkBackend)
-        db_url = retrieve_jdbc_url_from(flink_tables_file_path, backend, table)
-        if db_url:
-            from sqlalchemy import create_engine
-
-            engine: Engine = create_engine(db_url, isolation_level="AUTOCOMMIT", pool_size=1)
-            conn: Connection = engine.connect()
-            return conn
+            logger.warn("Cannot execute prepare-sql: the connector is not configured or not supported. Will skip this.")
 
 
 class PostgresBackendProcessor(BackendProcessor):
     def __init__(self, config: EasySqlConfig) -> None:
         super().__init__(config)
 
     def _create_backend(self, backend_config: Optional[List[str]]) -> Backend:
```

### Comparing `easy_sql-easy_sql-0.5.1/easy_sql/cli/sql_config.py` & `easy_sql_easy_sql-1.0.0/easy_sql/config/sql_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 from __future__ import annotations
 
 import os
 import re
 import urllib.parse
 from datetime import datetime
 from os import path
-from typing import Any, Callable, Dict, List, Optional, Tuple
+from typing import Any, Dict, List, Optional
 
+from easy_sql.logger import logger
 from easy_sql.utils.io_utils import read_sql, resolve_file
+from easy_sql.utils.kv import (
+    KV,
+    get_key_by_splitter_and_strip,
+    get_value_by_splitter_and_strip,
+)
 
 
-def _parse_backend(sql: str):
+def parse_backend(sql: str):
     sql_lines = sql.split("\n")
 
     backend = "spark"
     for line in sql_lines:
         if re.match(r"^-- \s*backend:.*$", line):
             backend = get_value_by_splitter_and_strip(line, "backend:").split(" ")[0]
             break
@@ -29,23 +35,14 @@
     tables = []
     for line in sql_lines:
         if re.match(rf"^-- \s*{table_type}:.*$", line):
             tables += get_value_by_splitter_and_strip(line, table_type + ":").split(",")
     return tables
 
 
-def get_key_by_splitter_and_strip(source: str, splitter: Optional[str] = "=", strip: Optional[str] = None):
-    return source.strip()[: source.strip().index(splitter or "=")].strip(strip)
-
-
-def get_value_by_splitter_and_strip(source: str, splitter: Optional[str] = "=", strip: Optional[str] = None):
-    splitter = splitter or "="
-    return source.strip()[source.strip().index(splitter) + len(splitter) :].strip(strip)
-
-
 def parse_vars(vars: Optional[str]) -> Dict[str, Any]:
     vars_dict: Dict[str, Any] = dict(
         [
             (get_key_by_splitter_and_strip(v), urllib.parse.unquote_plus(get_value_by_splitter_and_strip(v)))
             for v in vars.split(",")
             if v.strip()
         ]
@@ -72,24 +69,28 @@
         self.sql_file = sql_file
         self.sql = sql
         self.backend = backend
         self.customized_backend_conf, self.customized_easy_sql_conf = customized_backend_conf, customized_easy_sql_conf
         self.udf_file_path, self.func_file_path = udf_file_path, func_file_path
         self.scala_udf_initializer = scala_udf_initializer
         self.input_tables, self.output_tables = input_tables, output_tables
+        self.resolved_udf_file_path = self._resolve_file(udf_file_path) if udf_file_path else None
+        self.resolved_func_file_path = self._resolve_file(func_file_path) if func_file_path else None
 
     @staticmethod
     def from_sql(
         sql_file: Optional[str] = None, sql: Optional[str] = None, system_config_prefix: str = "easy_sql."  # type: ignore
     ) -> EasySqlConfig:
         assert sql_file is not None or sql is not None, "sql_file or sql must be set"
-        sql: str = read_sql(sql_file) if sql_file else sql  # type: ignore
+        if sql and sql_file:
+            logger.info("both sql and sql_file set, will use sql as file content")
+        sql: str = sql if sql else read_sql(sql_file)  # type: ignore
         sql_lines = sql.split("\n")  # type: ignore
 
-        backend = _parse_backend(sql)
+        backend = parse_backend(sql)
         input_tables, output_tables = _parse_tables(sql, "inputs"), _parse_tables(sql, "outputs")
 
         customized_backend_conf: List[str] = []
         customized_easy_sql_conf: List[str] = []
         for line in sql_lines:
             if re.match(r"^-- \s*config:.*$", line):
                 config_value = get_value_by_splitter_and_strip(line, "config:")
@@ -126,17 +127,17 @@
     @property
     def tables(self) -> List[str]:
         return list({t.strip() for t in self.input_tables + self.output_tables})
 
     @property
     def is_batch(self) -> bool:
         etl_type_config = next(
-            filter(lambda c: get_key_by_splitter_and_strip(c) == "etl_type", self.customized_easy_sql_conf), "batch"
+            filter(lambda c: get_key_by_splitter_and_strip(c) == "etl_type", self.customized_easy_sql_conf), None
         )
-        return get_value_by_splitter_and_strip(etl_type_config) == "batch"
+        return get_value_by_splitter_and_strip(etl_type_config) == "batch" if etl_type_config else True
 
     @property
     def is_streaming(self) -> bool:
         return not self.is_batch
 
     @property
     def task_name(self):
@@ -148,14 +149,22 @@
     def prepare_sql_list(self) -> List[str]:
         prepare_sql_list = []
         for line in self.sql.split("\n"):
             if re.match(r"^-- \s*prepare-sql:.*$", line):
                 prepare_sql_list.append(get_value_by_splitter_and_strip(line, "prepare-sql:"))
         return prepare_sql_list
 
+    @property
+    def abs_sql_file_path(self) -> str:
+        assert self.sql_file is not None
+        return resolve_file(self.sql_file, abs_path=True)
+
+    def _resolve_file(self, file_path: str, *, prefix: str = "") -> str:
+        return resolve_file(file_path, abs_path=True, prefix=prefix, relative_to=self.abs_sql_file_path)
+
     def _build_conf_command_args(
         self,
         default_conf: List[str],
         user_default_conf: List[str],
         file_keys: List[str],
         customized_confs: List[str],
         prefix: str = "",
@@ -164,17 +173,15 @@
         # 1. sql 代码里的 config 优先级高于用户定义的 default 配置
         # 2. 用户定义的 default 配置高于Easy SQL定义的 default 配置
         # 3. 对于文件类的 config，sql 代码里的 config 会添加进来，而不是覆盖默认配置
         assert self.sql_file is not None
         customized_confs = customized_confs.copy()
 
         files = lambda files_str: [f.strip() for f in files_str.strip('"').split(",") if f.strip()]
-        resolved_files = lambda _files, prefix: [
-            resolve_file(f.strip(), abs_path=True, prefix=prefix) for f in files(_files)
-        ]
+        resolved_files = lambda _files, prefix: [self._resolve_file(f.strip(), prefix=prefix) for f in files(_files)]
 
         args: dict[str, str] = {}
         for conf in default_conf:
             args.update(KV.from_config(conf).as_dict())
         for prioritized_confs in [user_default_conf, customized_confs]:
             for conf in prioritized_confs:
                 kv = KV.from_config(conf)
@@ -212,17 +219,17 @@
             f"spark.app.name={self.config.task_name}",
             "spark.sql.warehouse.dir=/tmp/spark-warehouse-localdw",
             (
                 'spark.driver.extraJavaOptions="-Dderby.system.home=/tmp/spark-warehouse-metastore'
                 ' -Dderby.stream.error.file=/tmp/spark-warehouse-metastore.log"'
             ),
             (
-                f'spark.files="{resolve_file(config.sql_file, abs_path=True)}'
-                f'{"," + resolve_file(config.udf_file_path, abs_path=True) if config.udf_file_path else ""}'
-                f'{"," + resolve_file(config.func_file_path, abs_path=True) if config.func_file_path else ""}'
+                f'spark.files="{self.config.abs_sql_file_path}'
+                f'{"," + self.config._resolve_file(config.udf_file_path) if config.udf_file_path else ""}'
+                f'{"," + self.config._resolve_file(config.func_file_path) if config.func_file_path else ""}'
                 '"'
             ),
         ]
         args = config._build_conf_command_args(
             sys_default_conf,
             self.user_default_conf or [],
             ["spark.files", "spark.jars", "spark.submit.pyFiles"],
@@ -257,17 +264,15 @@
             }
         )
 
         file_keys = ["python.archives", "python.files", "python.requirements", "pipeline.jars"]
         for k in file_keys:
             if k in configs:
                 splitter = "," if k.startswith("python.") else ";"
-                configs[k] = splitter.join(
-                    {resolve_file(f, True, "file://") for f in configs[k].split(splitter) if f.strip()}
-                )
+                configs[k] = splitter.join({self._resolve_file(f) for f in configs[k].split(splitter) if f.strip()})
                 configs[k] = f"{configs[k]}"
 
         return configs
 
     @property
     def flink(self):
         # 默认情况下使用系统中默认flink版本下的flink
@@ -291,74 +296,48 @@
                 self.config.customized_easy_sql_conf,
             ),
             None,
         )
         if flink_tables_file_path is None:
             return None
         else:
-            return resolve_file(get_value_by_splitter_and_strip(flink_tables_file_path), abs_path=True)
+            return self.config._resolve_file(get_value_by_splitter_and_strip(flink_tables_file_path))
+
+    def _resolve_file(self, file_path: str) -> str:
+        return self.config._resolve_file(file_path, prefix="file://")
 
     def flink_conf_command_args(self) -> List[str]:
         # config 的优先级：1. sql 代码里的 config 优先级高于这里的 default 配置
         # 对于数组类的 config，sql 代码里的 config 会添加进来，而不是覆盖默认配置
         config = self.config
-        assert config.sql_file is not None
         default_conf = [
             "--parallelism=1",
             (
-                f"--pyFiles={resolve_file(config.sql_file, abs_path=True, prefix='file://')}"
-                f'{"," + resolve_file(config.udf_file_path, abs_path=True, prefix="file://") if config.udf_file_path else ""}'
-                f'{"," + resolve_file(config.func_file_path, abs_path=True, prefix="file://") if config.func_file_path else ""}'
+                f"--pyFiles={'file://' + self.config.abs_sql_file_path}"
+                f'{"," + self._resolve_file(config.udf_file_path) if config.udf_file_path else ""}'
+                f'{"," + self._resolve_file(config.func_file_path) if config.func_file_path else ""}'
             ),
         ]
 
         # refer: https://nightlies.apache.org/flink/flink-docs-master/docs/deployment/cli/
         file_keys = [
             "-pyarch",
             "--pyArchives",
-            "-pyreq",
-            "--pyRequirements",
             "-pyfs",
             "--pyFiles",
-            "-s",
-            "--fromSavepoint",
         ]
         cmd_value_args = []
         for c in config.customized_backend_conf:
             if get_key_by_splitter_and_strip(c) == "flink.cmd":
                 key = get_key_by_splitter_and_strip(get_value_by_splitter_and_strip(c), " ")
                 value = get_value_by_splitter_and_strip(get_value_by_splitter_and_strip(c), " ")
                 if key in file_keys:
-                    resolve_files = [
-                        f'{resolve_file(val.strip(), abs_path=True, prefix="file://")}'
-                        for val in value.split(",")
-                        if val.strip()
-                    ]
+                    resolve_files = [f"{self._resolve_file(val.strip())}" for val in value.split(",") if val.strip()]
                     value = f'"{",".join(set(resolve_files))}"'
                 cmd_value_args.append(f"{key}={value}")
 
         args = config._build_conf_command_args(
             default_conf, self.user_default_conf or [], file_keys, cmd_value_args, prefix="file://"
         )
         cmd_args = [f"{arg} {args[arg]}" for arg in args]
 
         return cmd_args
-
-
-class KV:
-    def __init__(self, k: str, v: str) -> None:
-        self.k, self.v = k, v
-
-    @staticmethod
-    def from_config(config_line: str, splitter: Optional[str] = "=", strip: Optional[str] = None) -> KV:
-        return KV(
-            get_key_by_splitter_and_strip(config_line, splitter, strip),
-            get_value_by_splitter_and_strip(config_line, splitter, strip),
-        )
-
-    def as_tuple(
-        self, k_convert: Optional[Callable[[str], Any]] = None, v_convert: Optional[Callable[[str], Any]] = None
-    ) -> Tuple[Any, Any]:
-        return (k_convert(self.k) if k_convert else self.k, v_convert(self.v) if v_convert else self.v)
-
-    def as_dict(self) -> Dict[str, str]:
-        return {self.k: self.v}
```

### Comparing `easy_sql-easy_sql-0.5.1/easy_sql/cli/sql_config_test.py` & `easy_sql_easy_sql-1.0.0/easy_sql/config/sql_config_test.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import re
 import unittest
 
-from easy_sql.cli.sql_config import (
+from easy_sql.config.sql_config import (
     EasySqlConfig,
     FlinkBackendConfig,
     SparkBackendConfig,
 )
 
 
 class EasySqlConfigTest(unittest.TestCase):
@@ -27,14 +27,30 @@
         print(config.spark_conf_command_args())
 
         self.assertEqual(config.spark_submit, "/my/custom/spark-submit")
         self.assertTrue(contains_conf("spark.master=yarn"))
         self.assertTrue(contains_conf("spark.test=1"))
         self.assertEqual(find_conf("spark.files=")[0].count(","), 3)
 
+    def test_parse_spark_config_with_relative_files(self):
+        _config = EasySqlConfig.from_sql(
+            sql="""
+-- config: easy_sql.udf_file_path=sample_data_process.py
+-- config: easy_sql.func_file_path=sample_data_process.py
+-- config: spark.files=test/sample_etl.spark.sql,sample_etl.postgres.sql,
+        """,
+            sql_file="test/sample_etl.spark.sql",
+        )
+
+        config = SparkBackendConfig(_config)
+        find_conf = lambda search_str: [_c for _c in config.spark_conf_command_args() if _c.find(search_str) != -1]
+        print(config.spark_conf_command_args())
+
+        self.assertEqual(find_conf("spark.files=")[0].count(","), 2)
+
     def test_parse_flink_config(self):
         _config = EasySqlConfig.from_sql(
             sql="""
 -- config: easy_sql.udf_file_path=test/sample_data_process.py
 -- config: easy_sql.func_file_path=test/sample_data_process.py
 -- config: easy_sql.flink_run=/my/custom/flink
 -- config: flink.cmd=-py test/sample_data_process.py
@@ -58,7 +74,26 @@
         print(config.flink_conf_command_args())
 
         self.assertEqual(config.flink, "/my/custom/flink")
         self.assertTrue(contains_conf("--parallelism 2"))
         self.assertFalse(contains_conf("-Da=a"))
         self.assertTrue(contains_conf_re(r"-py .*test/sample_data_process.py"))
         self.assertEqual(find_conf("--pyFiles ")[0].count(","), 2)
+
+    def test_parse_flink_config_with_relative_files(self):
+        _config = EasySqlConfig.from_sql(
+            sql="""
+-- config: easy_sql.udf_file_path=sample_data_process.py
+-- config: easy_sql.func_file_path=sample_data_process.py
+-- config: easy_sql.flink_tables_file_path=sample_etl.flink_tables_file.json
+-- config: flink.cmd=--pyFiles sample_etl.postgres.sql
+-- config: flink.cmd=-pyarch sample_etl.spark.sql,test/sample_etl.postgres.sql,
+        """,
+            sql_file="test/sample_etl.spark.sql",
+        )
+
+        config = FlinkBackendConfig(_config)
+        find_conf = lambda search_str: [_c for _c in config.flink_conf_command_args() if _c.find(search_str) != -1]
+        print(config.flink_conf_command_args())
+
+        self.assertEqual(find_conf("--pyFiles ")[0].count(","), 2)
+        self.assertEqual(find_conf("-pyarch ")[0].count(","), 1)
```

### Comparing `easy_sql-easy_sql-0.5.1/easy_sql/data_process.py` & `easy_sql_easy_sql-1.0.0/easy_sql/data_process.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,19 +26,19 @@
         print_command: bool,
         python_path: Optional[str] = None,
     ) -> None:
         if not sql_file.endswith(".sql"):
             raise Exception(f"sql_file must ends with .sql, found `{sql_file}`")
 
         try:
-            from easy_sql.cli.sql_config import EasySqlConfig
+            from easy_sql.config.sql_config import EasySqlConfig
         except ModuleNotFoundError:
             assert python_path is not None
             sys.path.insert(0, python_path)
-            from easy_sql.cli.sql_config import EasySqlConfig
+            from easy_sql.config.sql_config import EasySqlConfig
 
         self.sql_file = sql_file
         self.vars_arg = vars
         self.dry_run_arg = dry_run if dry_run is not None else "0"
         self.dry_run = dry_run in ["true", "1"]
         self.config = EasySqlConfig.from_sql(sql_file)
         self.print_command = print_command
```

### Comparing `easy_sql-easy_sql-0.5.1/easy_sql/data_process_itest.py` & `easy_sql_easy_sql-1.0.0/easy_sql/data_process_itest.py`

 * *Files identical despite different names*

### Comparing `easy_sql-easy_sql-0.5.1/easy_sql/data_process_test.py` & `easy_sql_easy_sql-1.0.0/easy_sql/data_process_test.py`

 * *Files identical despite different names*

### Comparing `easy_sql-easy_sql-0.5.1/easy_sql/local_spark.py` & `easy_sql_easy_sql-1.0.0/easy_sql/local_spark.py`

 * *Files identical despite different names*

### Comparing `easy_sql-easy_sql-0.5.1/easy_sql/logger.py` & `easy_sql_easy_sql-1.0.0/easy_sql/logger.py`

 * *Files identical despite different names*

### Comparing `easy_sql-easy_sql-0.5.1/easy_sql/report.py` & `easy_sql_easy_sql-1.0.0/easy_sql/report.py`

 * *Files identical despite different names*

### Comparing `easy_sql-easy_sql-0.5.1/easy_sql/spark_optimizer.py` & `easy_sql_easy_sql-1.0.0/easy_sql/spark_optimizer.py`

 * *Files identical despite different names*

### Comparing `easy_sql-easy_sql-0.5.1/easy_sql/sql_linter/rules/bq_schema_rule.py` & `easy_sql_easy_sql-1.0.0/easy_sql/sql_linter/rules/bq_schema_rule.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,17 @@
+from __future__ import annotations
+
+from typing import TYPE_CHECKING
+
 from sqlfluff.core.parser import CodeSegment
-from sqlfluff.core.rules.base import BaseRule, LintFix, LintResult, RuleContext
+from sqlfluff.core.rules.base import BaseRule, LintFix, LintResult
+from sqlfluff.core.rules.crawlers import SegmentSeekerCrawler
+
+if TYPE_CHECKING:
+    from sqlfluff.core.rules.context import RuleContext
 
 
 class Rule_BigQuery_L001(BaseRule):
     """
     Table schema is required for queries in BigQuery.
 
     **Anti-pattern**
@@ -18,22 +26,23 @@
 
     .. code-block:: sql
         SELECT *
         FROM test.foo
     """
 
     groups = ("all", "bigquery")
+    crawl_behaviour = SegmentSeekerCrawler({"table_reference"})
 
     def __init__(self, *args, **kwargs):
         """Overwrite __init__ to set config."""
         super().__init__(*args, **kwargs)
 
     def _eval(self, context: RuleContext):
         """check from table have schema"""
-        if context.segment.is_type("table_reference") and len(context.segment.segments) != 3:
+        if len(context.segment.segments) != 3:
             return LintResult(
                 anchor=context.segment,
                 fixes=[
                     LintFix.create_before(
                         context.segment,
                         [CodeSegment(raw="${temp_db}.")],
                     )
```

### Comparing `easy_sql-easy_sql-0.5.1/easy_sql/sql_linter/sql_linter.py` & `easy_sql_easy_sql-1.0.0/easy_sql/sql_linter/sql_linter.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 import re
-from typing import TYPE_CHECKING, Any, Dict, List, Optional, Sequence
+from typing import TYPE_CHECKING, List, Optional, Sequence
 
 import regex
 from sqlfluff.core import Lexer, Linter, Parser, SQLBaseError
 from sqlfluff.core.config import FluffConfig
 from sqlfluff.core.parser import CodeSegment, RegexLexer
 
 from easy_sql.sql_linter.rules import all_rules
@@ -66,31 +66,31 @@
             # TODO: so far do not have clickhouse in sql fluff
             return "ansi"
         if backend == "postgres":
             return "postgres"
         raise Exception("backend type so far is not supported for lint check")
 
     @staticmethod
-    def _update_included_rule_for_config(config: Dict[str, Any], dialect: Optional[str] = None, rules=None):
+    def _included_rule_config(dialect: Optional[str] = None, rules=None) -> str:
         if rules is None:
             rules = []
         if len(rules) > 0:
-            config["core"]["rules"] = ",".join(rules)
+            return ",".join(rules)
         else:
             if dialect in ["bigquery"]:
-                config["core"]["rules"] = "core," + dialect
+                return "core,L019," + dialect
             else:
-                config["core"]["rules"] = "core"
+                return "core,L019"
 
     @staticmethod
-    def _update_excluded_rule_for_config(config: Dict[str, Any], rules: Optional[List[str]] = None):
+    def _excluded_rule_config(rules: Optional[List[str]] = None) -> Optional[str]:
         if rules is not None:
-            config["core"]["exclude_rules"] = ",".join(rules)
+            return ",".join(rules)
         else:
-            config["core"]["exclude_rules"] = None
+            return None
 
     def _check_parsable(self, root_segment: BaseSegment) -> bool:
         segment_list = [root_segment]
         while len(segment_list) > 0:
             check_segment = segment_list[0]
             segment_list.remove(check_segment)
             if check_segment.is_type("unparsable"):
@@ -206,21 +206,24 @@
         line_no = self.step_list[0].target_config.line_no
         return self.origin_sql.split("\n")[: line_no - 1]
 
     def _prepare_linter(self, dialect: str, config_path: Optional[str] = None):
         if config_path:
             config = FluffConfig.from_path(config_path)
         else:
-            default_config_dict = FluffConfig(require_dialect=False)._configs
-            default_config_dict["rules"]["L019"] = {"comma_style": "leading"}
-            default_config_dict["rules"]["L014"] = {"extended_capitalisation_policy": "lower"}
-            default_config_dict["core"]["dialect"] = dialect
-            self._update_included_rule_for_config(default_config_dict, dialect=dialect, rules=self.include_rules)
-            self._update_excluded_rule_for_config(default_config_dict, rules=self.exclude_rules)
-            config = FluffConfig(configs=default_config_dict)
+            config = {
+                "core": {
+                    "dialect": dialect,
+                    "rules": self._included_rule_config(dialect=dialect, rules=self.include_rules),
+                    "exclude_rules": self._excluded_rule_config(rules=self.exclude_rules),
+                },
+                "layout": {"type": {"comma": {"line_position": "leading"}}},
+                "rules": {"L014": {"extended_capitalisation_policy": "lower"}},
+            }
+            config = FluffConfig(configs=config)
         linter = Linter(config=config, user_rules=all_rules)  # type: ignore
         return linter
 
     def lint(
         self, backend: str, log_error: bool = True, easysql: bool = True, config_path: Optional[str] = None
     ) -> List[SQLBaseError]:
         if easysql:
```

### Comparing `easy_sql-easy_sql-0.5.1/easy_sql/sql_linter/sql_linter_cli.py` & `easy_sql_easy_sql-1.0.0/easy_sql/sql_linter/sql_linter_cli.py`

 * *Files identical despite different names*

### Comparing `easy_sql-easy_sql-0.5.1/easy_sql/sql_linter/sql_linter_reportor.py` & `easy_sql_easy_sql-1.0.0/easy_sql/sql_linter/sql_linter_reportor.py`

 * *Files identical despite different names*

### Comparing `easy_sql-easy_sql-0.5.1/easy_sql/sql_linter/sql_linter_test.py` & `easy_sql_easy_sql-1.0.0/easy_sql/sql_linter/sql_linter_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,27 +76,27 @@
 
     def test_should_work_for_multiple_step(self):
         sql = """-- backend: bigquery
 -- target=variables
 select
     translate('${data_date}', '-', '')  as data_date_no_ds
     , true                              as __create_hive_table__
-    
+
 -- target=temp.model_data
 select * from sales_model_demo_with_label where date='${data_date_no_ds}'
 
 
 -- target=temp.feature_stage_0_out
 select *
 , ${data_date_no_ds}, a1, b1 from ${temp_db}.model_data
 """
 
         sql_linter = SqlLinter(sql, include_rules=None, exclude_rules=None)
         result = sql_linter.lint("bigquery")
-        self.assertEqual(len(result), 7)
+        self.assertEqual(len(result), 8)
         fixed = sql_linter.fix("bigquery")
         expected = """-- backend: bigquery
 -- target=variables
 select
     translate('${data_date}', '-', '') as data_date_no_ds
     , true as __create_hive_table__
 
@@ -123,15 +123,15 @@
 union all
 select @{dim_cols} from sales_amount
 
 -- target=temp.result
 @{transited_with_fk_inc_template(
     source_table_name=transited, source_table_biz_key=product_id, result_col_name=product_id_key,
     fk_table_name=dwd_sales.sales_dim_product_h, pk=product_key, fk_table_biz_key=id,
-    update_time_col_name=update_time, partition_col_name=di)} 
+    update_time_col_name=update_time, partition_col_name=di)}
 """
         sql_linter = SqlLinter(sql, exclude_rules=["L025"])
         result = sql_linter.lint("bigquery")
         self.assertEqual(len(result), 2)
         fixed = sql_linter.fix("bigquery")
         print(fixed)
         expected = """-- backend: bigquery
@@ -144,15 +144,15 @@
 union all
 select @{dim_cols} from ${temp_db}.sales_amount
 
 -- target=temp.result
 @{transited_with_fk_inc_template(
     source_table_name=transited, source_table_biz_key=product_id, result_col_name=product_id_key,
     fk_table_name=dwd_sales.sales_dim_product_h, pk=product_key, fk_table_biz_key=id,
-    update_time_col_name=update_time, partition_col_name=di)} """
+    update_time_col_name=update_time, partition_col_name=di)}"""
         self.assertEqual(expected, fixed)
 
     def test_should_work_when_given_diff_backend(self):
         # spark can only use union
         sql = """-- backend: spark
 -- --------------------
 -- 标签：产品销量
@@ -169,20 +169,20 @@
 
 -- target=template.dim_cols
 product_name
 , product_category
 
 -- target=temp.dims
 select @{dim_cols} from order_count
-union 
+union
 select @{dim_cols} from sales_amount
 """
         sql_linter = SqlLinter(sql)
         result = sql_linter.lint("spark", True)
-        self.assertEqual(len(result), 1)
+        self.assertEqual(len(result), 0)
         fixed = sql_linter.fix("spark")
         expected = """-- backend: spark
 -- --------------------
 -- 标签：产品销量
 -- --------------------
 
 -- config: spark.master=local[2]
@@ -207,29 +207,29 @@
 
     def test_should_work_when_have_functions(self):
         sql = """-- backend: bigquery
 
 -- target=variables
 select ${plus(1, 2)} as a
 , flag as b
-from data_table 
+from data_table
 
 -- target=temp.dims
 select * from order_count where value < ${a}
 
 -- target=func.plus(1, 1)
 
 """
         sql_linter = SqlLinter(sql)
         result = sql_linter.lint("bigquery", True)
         print("after fix")
         print(len(result))
         fixed = sql_linter.fix("bigquery")
         print(fixed)
-        self.assertEqual(len(result), 4)
+        self.assertEqual(len(result), 3)
         expected = """-- backend: bigquery
 
 -- target=variables
 select ${plus(1, 2)} as a
     , flag as b
 from ${temp_db}.data_table
```

### Comparing `easy_sql-easy_sql-0.5.1/easy_sql/sql_processor/__init__.py` & `easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/__init__.py`

 * *Files identical despite different names*

### Comparing `easy_sql-easy_sql-0.5.1/easy_sql/sql_processor/backend/base.py` & `easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/backend/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -81,14 +81,17 @@
 
     def table_exists(self, table: TableMeta):
         pass
 
     def refresh_table_partitions(self, table: TableMeta):
         raise NotImplementedError()
 
+    def save_table_sql(self, source_table: TableMeta, source_table_sql: str, target_table: TableMeta) -> str:
+        raise NotImplementedError()
+
     def save_table(
         self, source_table: TableMeta, target_table: TableMeta, save_mode: SaveMode, create_target_table: bool
     ):
         raise NotImplementedError()
 
     def clean(self):
         raise NotImplementedError()
```

### Comparing `easy_sql-easy_sql-0.5.1/easy_sql/sql_processor/backend/flink.py` & `easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/backend/spark.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,258 +1,270 @@
 from __future__ import annotations
 
-import json
-import os
-from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional, Tuple
+from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional, Tuple, Union
 
 from ...logger import logger
-from .base import Backend, Row, SaveMode, Table, TableMeta
+from ...udf import udfs
+from ..common import SqlProcessorAssertionError
+from .base import Backend, Col, Partition, Row, SaveMode, Table, TableMeta
+
+__all__ = ["SparkRow", "SparkTable", "SparkBackend"]
 
 if TYPE_CHECKING:
-    from pyflink.common import Row as PyFlinkRow
-    from pyflink.table import Table as PyFlinkTable
+    from pyspark.sql import DataFrame
+    from pyspark.sql.types import StructType
 
-__all__ = ["FlinkRow", "FlinkTable", "FlinkBackend"]
 
+class SparkRow(Row):
+    def __init__(self, row):
+        from pyspark.sql.types import Row as SparkRow
 
-class FlinkRow(Row):
-    def __init__(self, row=None, fields: Optional[List[str]] = None):
-        assert row is not None
-        self.row: PyFlinkRow = row
-        if fields is not None:
-            self.row._fields = fields
+        self.row: SparkRow = row
 
     def as_dict(self):
-        return self.row.as_dict()
+        return self.row.asDict()  # type: ignore
 
     def as_tuple(self) -> Tuple:
         return self.row  # type: ignore
 
     def __eq__(self, other):
-        return self.row.__eq__(other.row)
+        return self.row.__eq__(other)
 
     def __str__(self):
         return str(self.row)[4:-1]
 
     def __getitem__(self, i):
-        return self.row.__getitem__(i)
+        return self.row[i]
 
     def __repr__(self):
         return self.row.__repr__()
 
 
-class FlinkTable(Table):
-    def __init__(self, table):
-        self.table: PyFlinkTable = table
+class SparkTable(Table):
+    def __init__(self, df):
+        from pyspark.sql import DataFrame
+
+        self.df: DataFrame = df
 
     def is_empty(self) -> bool:
-        with self.table.limit(1).execute().collect() as result:
-            return len(list(result)) == 0
+        return self.df.count() == 0
 
     def field_names(self) -> List[str]:
-        return self.table.get_schema().get_field_names()
+        return self.df.schema.fieldNames()
 
     def first(self) -> Row:
-        fields = self.table.get_schema().get_field_names()
-        with self.table.execute().collect() as result:
-            collected_result = [FlinkRow(item, fields) for item in result]
-        return FlinkRow() if len(collected_result) == 0 else collected_result[0]
-
-    def limit(self, count: int) -> FlinkTable:
-        return FlinkTable(self.table.limit(count))
-
-    def with_column(self, name: str, value: Any) -> FlinkTable:
-        from pyflink.table.expression import Expression
-        from pyflink.table.expressions import lit
+        return SparkRow(self.df.first())
+
+    def limit(self, count: int) -> SparkTable:
+        return SparkTable(self.df.limit(count))
+
+    def with_column(self, name: str, value: Any) -> SparkTable:
+        from pyspark.sql import Column
+        from pyspark.sql.functions import expr
 
-        return FlinkTable(self.table.add_columns((value if isinstance(value, Expression) else lit(value)).alias(name)))
+        return SparkTable(self.df.withColumn(name, value if isinstance(value, Column) else expr(value)))
 
     def collect(self) -> List[Row]:
-        fields = self.table.get_schema().get_field_names()
-        return [FlinkRow(item, fields) for item in self.table.execute().collect()]
+        return [SparkRow(row) for row in self.df.collect()]
 
     def show(self, count: int = 20):
-        self.table.limit(count).execute().print()
+        self.df.show(count)
 
     def count(self) -> int:
-        with self.table.execute().collect() as result:
-            return len(list(result))
+        return self.df.count()
 
 
-class FlinkBackend(Backend):
-    # todo: 考虑是否需要在外面实例化flink: TableEnvironment
-    def __init__(self, is_batch: Optional[bool] = True):
-        from pyflink.table import EnvironmentSettings, TableEnvironment
+class SparkBackend(Backend):
+    def __init__(self, spark, scala_udf_initializer: Optional[str] = None):
+        from pyspark.sql import SparkSession
 
-        self.flink: TableEnvironment = TableEnvironment.create(
-            EnvironmentSettings.in_batch_mode() if is_batch else EnvironmentSettings.in_streaming_mode()
-        )
+        self.spark: SparkSession = spark
+        self.scala_udf_initializer = scala_udf_initializer
+
+    def reset(self):
+        pass
 
     def init_udfs(self, scala_udf_initializer: Optional[str] = None, *args, **kwargs):
+        scala_udf_initializer = scala_udf_initializer or self.scala_udf_initializer
         if scala_udf_initializer:
             from py4j.java_gateway import java_import
-            from pyflink.java_gateway import get_gateway
 
-            gw = get_gateway()
+            gw = self.spark.sparkContext._gateway  # type: ignore
             java_import(gw.jvm, scala_udf_initializer)
             initUdfs = eval(f"gw.jvm.{scala_udf_initializer}.initUdfs", {"gw": gw})
-            initUdfs(self.flink._j_tenv)
+            initUdfs(self.spark._jsparkSession)  # type: ignore
 
-    def register_udfs(self, funcs: Dict[str, Callable]):
-        from pyflink.table.udf import UserDefinedScalarFunctionWrapper
+        self.register_udfs(udfs.get_udfs("spark"))
 
+    def register_udfs(self, funcs: Dict[str, Callable]):
         for key in funcs:
             func = funcs[key]
-            if isinstance(func, UserDefinedScalarFunctionWrapper):
-                self.flink.create_temporary_system_function(key, func)
+            self.spark.udf.register(key, func)
 
-    def clean(self):
-        for temp_view in self.flink.list_temporary_views():
-            self.flink.drop_temporary_view(temp_view)
+    def set_spark_configs(self, configs: Dict[str, str]):
+        for key, value in configs.items():
+            self.spark.conf.set(key, value)
+
+    def temp_tables(self) -> List[str]:
+        return [table.name for table in self.spark.catalog.listTables("default") if table.isTemporary]
+
+    def clear_cache(self):
+        self.spark.catalog.clearCache()
+
+    def clear_temp_tables(self, exclude: Optional[List[str]] = None):
+        exclude = exclude or []
+        for table in self.spark.catalog.listTables("default"):
+            if table.isTemporary and table.name not in exclude:
+                print(f"dropping temp view {table.name}")
+                self.spark.catalog.dropTempView(table.name)
+
+    def create_empty_table(self):
+        from pyspark.sql.types import StructType
+
+        return SparkTable(self.spark.createDataFrame(self.spark.sparkContext.emptyRDD(), StructType([])))
+
+    def create_temp_table(self, table: SparkTable, name: str):
+        table.df.createOrReplaceTempView(name)
+
+    def create_cache_table(self, table: SparkTable, name: str):
+        table.df.createOrReplaceTempView(name)
+        self.spark.catalog.cacheTable(name)
+
+    def broadcast_table(self, table: SparkTable, name: str):
+        from pyspark.sql.functions import broadcast
 
-    def exec_native_sql(self, sql: str):
+        df = broadcast(table.df)
+        df.createOrReplaceTempView(name)
+
+    def exec_native_sql(self, sql: str) -> DataFrame:
         logger.info(f"will exec sql: {sql}")
-        return self.flink.execute_sql(sql)
+        return self.spark.sql(sql)
 
     def exec_sql(self, sql: str) -> Table:
         logger.info(f"will exec sql: {sql}")
-        return FlinkTable(self.flink.sql_query(sql))
-
-    def create_empty_table(self):
-        return FlinkTable("")
-
-    def create_temp_table(self, table: Table, name: str):
-        assert isinstance(table, FlinkTable)
-        self.flink.create_temporary_view(name, table.table)
-
-    def create_cache_table(self, table: Table, name: str):
-        assert isinstance(table, FlinkTable)
-        self.flink.create_temporary_view(name, table.table)
+        return SparkTable(self.spark.sql(sql))
 
     def table_exists(self, table: TableMeta):
-        catalog = table.catalog_name if table.catalog_name else self.flink.get_current_catalog()
-        database = table.dbname if table.dbname else self.flink.get_current_database()
-        from pyflink.table.catalog import ObjectPath
+        from pyspark.sql.utils import AnalysisException
 
-        return self.flink.get_catalog(catalog).table_exists(ObjectPath(database, table.pure_table_name))
+        try:
+            return self.spark._jsparkSession.catalog().tableExists(table.dbname, table.pure_table_name)  # type: ignore
+        except AnalysisException:
+            return False
+
+    def _create_table(self, dbname: str, table_name: str, schema: StructType, partitions: List[Partition]):
+        from pyspark.sql.functions import lit
+
+        spark = self.spark
+        df = spark.createDataFrame(spark.sparkContext.emptyRDD(), schema)
+        schema = df.schema
+        for p in partitions or []:
+            if p.field not in schema.fieldNames():
+                if p.value is None:
+                    raise SqlProcessorAssertionError(
+                        "partition column value is None when create table with partitions but partitions is not in"
+                        f" dataframe. this should not happen. table_name={dbname}.{table_name}, p.field={p.field},"
+                        f" p.value={p.value}"
+                    )
+                df = df.withColumn(p.field, lit(p.value))
+
+        df.createOrReplaceTempView("table_data")
+        partition_expr = f'partitioned by ({",".join([p.field for p in partitions])}) ' if partitions else ""
+        create_database_stmt = f"create database if not exists {dbname}"
+        create_table_stmt = f"""create table if not exists {dbname}.{table_name} using hive
+                                options(FILEFORMAT "parquet") {partition_expr}
+                                TBLPROPERTIES ("transactional" = "false")
+                                as select * from table_data"""
+
+        self.exec_native_sql(create_database_stmt)
+        self.exec_native_sql(create_table_stmt)
+        return self
+
+    def save_table_sql(self, source_table: TableMeta, source_table_sql: str, target_table: TableMeta) -> str:
+        columns = self.exec_native_sql(f"select * from {source_table.table_name}").limit(0).columns
+        return f'insert into {target_table.table_name} select {",".join(columns)} from ({source_table_sql})'
 
     def save_table(
         self,
         source_table_meta: TableMeta,
         target_table_meta: TableMeta,
         save_mode: SaveMode,
-        create_target_table: bool = False,
+        create_target_table: bool,
     ):
-        from pyflink.table.expressions import col, lit
+        from pyspark.sql.functions import lit
 
-        if not self.table_exists(target_table_meta):
-            raise Exception(
-                f"target table {target_table_meta.table_name} does not exist, "
-                f"cannot save table {target_table_meta.table_name} to {target_table_meta.table_name}"
+        if not self.table_exists(target_table_meta) and create_target_table:
+            schema = self.spark.sql(f"select * from {source_table_meta.table_name}").limit(0).schema
+            assert target_table_meta.dbname is not None
+            self._create_table(
+                target_table_meta.dbname, target_table_meta.pure_table_name, schema, target_table_meta.partitions
             )
 
-        temp_res = self.flink.sql_query(f"select * from {source_table_meta.table_name}")
+        temp_res = self.exec_native_sql(f"select * from {source_table_meta.table_name}")
+        # partial dynamic partition (动态分区和静态分区同时使用）在 spark 2.3.2 上有问题，参见 https://issues.apache.org/jira/browse/SPARK-31605
         # 纯动态分区时，如果当日没有新增数据，则不会创建 partition。而我们希望对于静态分区，总是应该创建分区，即使当日没有数据
+        dynamic_partitions = list(filter(lambda p: not p.value, target_table_meta.partitions))
         static_partitions = list(filter(lambda p: p.value, target_table_meta.partitions))
-        columns = (
-            self.flink.sql_query(f"select * from {target_table_meta.table_name}")
-            .limit(0)
-            .get_schema()
-            .get_field_names()
+        columns = self.exec_native_sql(f"select * from {target_table_meta.table_name}").limit(0).columns
+        if dynamic_partitions:
+            for p in static_partitions:
+                temp_res = temp_res.withColumn(p.field, lit(p.value))
+            temp_res = temp_res.select(*columns)
+            fields = [f"{p.field}" for p in dynamic_partitions]
+        else:
+            columns = [c for c in columns if c not in [p.field for p in static_partitions]]
+            temp_res = temp_res.select(*columns)
+            fields = [
+                f"{p.field}='{p.value}'" if isinstance(p.value, str) else f"{p.field}={p.value}"
+                for p in target_table_meta.partitions
+            ]
+        partition_expr = f"partition ({','.join(fields)})" if fields else ""
+
+        # to resolve issue: pyspark.sql.utils.AnalysisException: Cannot overwrite a path that is also being read from.
+        # refer: https://stackoverflow.com/questions/38746773/read-from-a-hive-table-and-write-back-to-it-using-spark-sql
+        temp_res = self.spark.createDataFrame(temp_res.rdd, temp_res.schema)
+        temp_res.createOrReplaceTempView("res")
+
+        save_sql = (
+            f"insert {'into' if save_mode == SaveMode.append else save_mode.name} table"
+            f" {target_table_meta.table_name} {partition_expr} select * from res"
         )
-        for p in static_partitions:
-            temp_res = temp_res.add_columns(lit(p.value).alias(p.field))
-        temp_res = temp_res.select(*[col(column) for column in columns])
-
-        temp_res.execute_insert(target_table_meta.table_name, save_mode == SaveMode.overwrite)
+        self.exec_native_sql(save_sql)
 
     def refresh_table_partitions(self, table: TableMeta):
-        # flink无法从`desc table`中解析出partition字段，但是可以在flink_source_file中配置table的partition字段
-        pass
+        df = self.exec_native_sql(f"desc {table.table_name}")
+        column_list = df.select(df.col_name, df.data_type).rdd.map(lambda x: (x[0], x[1])).collect()
+        partition_details = [
+            column_list[index + 1 :] for index, item in enumerate(column_list) if item[0] == "# col_name"
+        ]
+        if len(partition_details) == 0:
+            table.update_partitions([])
+        else:
+            partitions = [Partition(x[0]) for x in partition_details[0]]
+            table.update_partitions([Partition(p.field, p.value) for p in partitions])
 
-    def _register_catalog(self, flink_config):
-        if "catalogs" in flink_config:
-            for catalog in flink_config["catalogs"]:
-                catalog_name = catalog["name"]
-                del catalog["name"]
-                catalog_expr = " , ".join([f"'{option}' = '{catalog[option]}'" for option in catalog])
-                try:  # noqa: SIM105
-                    self.exec_native_sql(
-                        f"""
-                            CREATE CATALOG {catalog_name}
-                            WITH (
-                                {catalog_expr}
-                            );
-                        """
-                    )
-                except Exception:
-                    logger.warn(f"create hive catalog {catalog_name} failed.")
+    def clean(self):
+        from easy_sql.spark_optimizer import clear_temp_views
 
-    def _register_tables(self, flink_config, tables: List[str]):
-        if len(tables) == 0:
-            return
-        for table in tables:
-            db_name, table_config, connector = self.get_table_config_and_connector(flink_config, table)
-            if db_name and table_config and connector:
-                self.exec_native_sql(f"create database if not exists {db_name}")
-                self._create_table(table, table_config, connector)
-
-    def get_table_config_and_connector(self, flink_config, table: str):
-        db_name = table.strip().split(".")[0]
-        database = next(filter(lambda t: t["name"] == db_name, flink_config["databases"]), None)
-        if not database:
-            logger.warn(
-                f"database {db_name} does not exist in flink tables config file, register table {table} failed."
-            )
-            return None, None, None
+        self.spark.catalog.clearCache()
+        clear_temp_views(self.spark)
 
-        table_config = next(filter(lambda t: t["name"] == table.strip().split(".")[1], database["tables"]), None)
-        if not table_config:
-            logger.warn(f"table {table} does not exist in flink tables config file, register table {table} failed.")
-            return None, None, None
-
-        connectors = database["connectors"]
-        connector_name = table_config["connector"]["name"]
-        connector = next(filter(lambda conn: conn["name"] == connector_name, connectors), None)
-        if not connector:
-            logger.warn(
-                f"connector {connector_name} does not exist in flink tables config file, register table {table} failed."
-            )
-            return None, None, None
-        return db_name, table_config, connector
+    def create_table_with_data(
+        self,
+        full_table_name: str,
+        values: List[List[Any]],
+        schema: Union[StructType, List[Col]],
+        partitions: List[Partition],
+    ):
+        print(f"creating table: {full_table_name}")
+        self.spark.sql(f'create database if not exists {full_table_name.split(".")[0]}')
+        self.spark.sql(f"drop table if exists {full_table_name}").collect()
+        from pyspark.sql.types import StructType
+
+        schema_or_cols = schema if isinstance(schema, StructType) else [col.name for col in schema]
+        write = self.spark.createDataFrame(values, schema_or_cols).write
+        if partitions:
+            write = write.partitionBy(*[p.field for p in partitions])
+        write.mode("overwrite").saveAsTable(full_table_name, mode="overwrite")
 
-    def _create_table(self, table: str, table_config, connector):
-        schema = table_config["schema"]
-        schema_expr = " , ".join(schema)
-        partition_by_expr = (
-            f"""
-                PARTITIONED BY ({','.join(table_config['partition_by'])})"""
-            if "partition_by" in table_config
-            else ""
-        )
-        options = connector["options"]
-        options.update(table_config["connector"]["options"])
-        options_expr = " , ".join([f"'{option}' = '{options[option]}'" for option in options])
-        create_sql = f"""
-            create table if not exists {table.strip()} (
-                {schema_expr}
-            )
-            {partition_by_expr}
-            WITH (
-                {options_expr}
-            );
-        """
-        self.exec_native_sql(create_sql)
-
-    def register_tables(self, flink_tables_file_path: str, tables: List[str]):
-        if flink_tables_file_path and os.path.exists(flink_tables_file_path):
-            with open(flink_tables_file_path, "r") as f:
-                config = json.loads(f.read())
-                self._register_catalog(config)
-                self._register_tables(config, tables)
-
-    def add_jars(self, jars_path: List[str]):
-        self.flink.get_config().set("pipeline.jars", f'{";".join([f"file://{path}" for path in jars_path])}')
-
-    def set_configurations(self, configs: dict):
-        for c in configs:
-            self.flink.get_config().set(c, configs[c])
+    def create_temp_table_with_data(self, table_name: str, values: List[List[Any]], schema: StructType):
+        self.spark.createDataFrame(values, schema).createOrReplaceTempView(table_name)
```

### Comparing `easy_sql-easy_sql-0.5.1/easy_sql/sql_processor/backend/flink_itest.py` & `easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/backend/flink_itest.py`

 * *Files identical despite different names*

### Comparing `easy_sql-easy_sql-0.5.1/easy_sql/sql_processor/backend/maxcompute.py` & `easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/backend/maxcompute.py`

 * *Files identical despite different names*

### Comparing `easy_sql-easy_sql-0.5.1/easy_sql/sql_processor/backend/maxcompute_itest.py` & `easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/backend/maxcompute_itest.py`

 * *Files identical despite different names*

### Comparing `easy_sql-easy_sql-0.5.1/easy_sql/sql_processor/backend/rdb.py` & `easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/backend/rdb.py`

 * *Files 2% similar despite different names*

```diff
@@ -321,16 +321,18 @@
                 filter_expr = " and ".join(
                     [f"{pt.field} = {self.backend.sql_expr.for_value(pt.value)}" for pt in partitions]  # type: ignore
                 )
                 self._exec_sql(
                     self.db_config.insert_data_sql(
                         target_table_name,
                         col_names,
-                        f"select {converted_col_names} from {self.backend.temp_schema}.{temp_table_name} where"
-                        f" {filter_expr}",
+                        (
+                            f"select {converted_col_names} from {self.backend.temp_schema}.{temp_table_name} where"
+                            f" {filter_expr}"
+                        ),
                         partitions,
                     )
                 )
 
     def _get_save_partitions(self, target_table, temp_table_name):
         partitions_to_save = [target_table.partitions] if target_table.partitions else []
         if target_table.has_dynamic_partition():
@@ -596,14 +598,18 @@
             ).fetchall()
             for pt_values in pt_values_list:
                 save_partitions_list.append([Partition(field, value) for field, value in zip(pt_cols, pt_values)])
         else:  # static partitions (partition specified in sql file)
             save_partitions_list.append(target_table.partitions)
         return save_partitions_list
 
+    def save_table_sql(self, source_table: TableMeta, source_table_sql: str, target_table: TableMeta) -> str:
+        source_col_names = self.get_column_names(source_table.pure_table_name, source_table.dbname or self.temp_schema)
+        return f'insert into {target_table.table_name} select {",".join(source_col_names)} from ({source_table_sql})'
+
     def save_table(
         self, source_table: TableMeta, target_table: TableMeta, save_mode: SaveMode, create_target_table: bool
     ):
         logger.info(
             f"save table with: source_table={source_table}, target_table={target_table}, "
             f"save_mode={save_mode}, create_target_table={create_target_table}"
         )
@@ -764,16 +770,18 @@
                     [f"{pt.field} = {self.sql_expr.for_value(pt.value)}" for pt in save_partition]
                 )
                 _exec_sql(
                     self.conn,
                     self.sql_dialect.insert_data_sql(
                         full_target_table_name,
                         col_names,
-                        f"select {col_names} from {source_table.get_full_table_name(self.temp_schema)} where"
-                        f" {filter_expr}",
+                        (
+                            f"select {col_names} from {source_table.get_full_table_name(self.temp_schema)} where"
+                            f" {filter_expr}"
+                        ),
                         save_partition,
                     ),
                 )
         else:
             _exec_sql(
                 self.conn,
                 self.sql_dialect.insert_data_sql(
```

### Comparing `easy_sql-easy_sql-0.5.1/easy_sql/sql_processor/backend/rdb_itest.py` & `easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/backend/rdb_itest.py`

 * *Files 0% similar despite different names*

```diff
@@ -140,16 +140,18 @@
         _exec_sql(backend.conn, "drop schema if exists t cascade")
         _exec_sql(backend.conn, "create schema t")
         _exec_sql(backend.conn, "create table t.test(id int, val varchar(100))")
         _exec_sql(backend.conn, "insert into t.test values(1, '1'), (2, '2'), (3, '3')")
         _exec_sql(backend.conn, "create table t.dynamic_partition_test(id int, val varchar(100), a varchar(100))")
         _exec_sql(
             backend.conn,
-            "insert into t.dynamic_partition_test values(1, '1', '2021-01-01'), "
-            "(2, '2', '2021-01-02'),(3, '3', '2021-01-03')",
+            (
+                "insert into t.dynamic_partition_test values(1, '1', '2021-01-01'), "
+                "(2, '2', '2021-01-02'),(3, '3', '2021-01-03')"
+            ),
         )
 
         self.run_test_backend(backend)
 
     def test_ch_backend(self):
         backend = RdbBackend(TEST_CH_URL)
         _exec_sql(backend.conn, "drop database if exists t")
@@ -158,16 +160,18 @@
         _exec_sql(backend.conn, "insert into t.test values(1, '1'), (2, '2'), (3, '3')")
         _exec_sql(
             backend.conn,
             "create table t.dynamic_partition_test(id int, val String, a DateTime) engine=MergeTree order by tuple()",
         )
         _exec_sql(
             backend.conn,
-            "insert into t.dynamic_partition_test values(1, '1', '2021-01-01 00:00:00'), "
-            "(2, '2', '2021-01-02 00:00:00'), (3, '3', '2021-01-03 00:00:00')",
+            (
+                "insert into t.dynamic_partition_test values(1, '1', '2021-01-01 00:00:00'), "
+                "(2, '2', '2021-01-02 00:00:00'), (3, '3', '2021-01-03 00:00:00')"
+            ),
         )
         self.run_test_backend(backend)
 
     def test_bq_backend(self):
         if not base_test.should_run_integration_test("bq"):
             return
         import os
@@ -180,16 +184,18 @@
         _exec_sql(backend.conn, "drop schema if exists t cascade")
         _exec_sql(backend.conn, "create schema if not exists t")
         _exec_sql(backend.conn, "create table if not exists t.test(id int, val string)")
         _exec_sql(backend.conn, "insert into t.test values(1, '1'), (2, '2'), (3, '3')")
         _exec_sql(backend.conn, "create table if not exists t.dynamic_partition_test(id int, val string, a date)")
         _exec_sql(
             backend.conn,
-            "insert into t.dynamic_partition_test values(1, '1', '2021-01-01'), (2, '2', '2021-01-02'), (3, '3',"
-            " '2021-01-03')",
+            (
+                "insert into t.dynamic_partition_test values(1, '1', '2021-01-01'), (2, '2', '2021-01-02'), (3, '3',"
+                " '2021-01-03')"
+            ),
         )
         self.run_test_backend(backend)
 
     def run_test_table(self, backend: RdbBackend, timezone=None):
         table = backend.exec_sql("select * from t.test")
         self.assertFalse(table.is_empty())
```

### Comparing `easy_sql-easy_sql-0.5.1/easy_sql/sql_processor/backend/rdb_test.py` & `easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/backend/rdb_test.py`

 * *Files identical despite different names*

### Comparing `easy_sql-easy_sql-0.5.1/easy_sql/sql_processor/backend/spark_test.py` & `easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/backend/spark_test.py`

 * *Files identical despite different names*

### Comparing `easy_sql-easy_sql-0.5.1/easy_sql/sql_processor/backend/sql_dialect/__init__.py` & `easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/backend/sql_dialect/__init__.py`

 * *Files identical despite different names*

### Comparing `easy_sql-easy_sql-0.5.1/easy_sql/sql_processor/backend/sql_dialect/bigquery.py` & `easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/backend/sql_dialect/bigquery.py`

 * *Files identical despite different names*

### Comparing `easy_sql-easy_sql-0.5.1/easy_sql/sql_processor/backend/sql_dialect/clickhouse.py` & `easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/backend/sql_dialect/clickhouse.py`

 * *Files identical despite different names*

### Comparing `easy_sql-easy_sql-0.5.1/easy_sql/sql_processor/backend/sql_dialect/clickhouse_test.py` & `easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/backend/sql_dialect/clickhouse_test.py`

 * *Files identical despite different names*

### Comparing `easy_sql-easy_sql-0.5.1/easy_sql/sql_processor/backend/sql_dialect/postgres.py` & `easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/backend/sql_dialect/postgres.py`

 * *Files identical despite different names*

### Comparing `easy_sql-easy_sql-0.5.1/easy_sql/sql_processor/common.py` & `easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/common.py`

 * *Files identical despite different names*

### Comparing `easy_sql-easy_sql-0.5.1/easy_sql/sql_processor/funcs.py` & `easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/funcs.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,22 @@
-from typing import Callable, Dict, Optional
+from typing import Callable, Dict, List, Optional, Tuple
 
-from .backend import Backend, SparkBackend
+from .backend import Backend, FlinkBackend, SparkBackend
 from .backend.rdb import RdbBackend
 from .common import SqlProcessorException, VarsReplacer
 
 __all__ = ["FuncRunner"]
 
 
+EASYSQL_FUNCS = {
+    "is_greater_or_equal": lambda a, b: a >= b,
+    "equal_ignore_case": lambda a, b: a.lower() == b.lower(),
+}
+
+
 class FuncRunner:
     _instance = None
 
     def __init__(self, funcs: Optional[Dict[str, Callable]] = None):
         self.funcs: Dict[str, Callable] = funcs or {}
 
     def register_funcs(self, funcs: Dict[str, Callable]):
@@ -33,51 +39,54 @@
             for func in dir(operator)
             if not func.startswith("_") and func[0].islower() and callable(getattr(operator, func))
         }
         operator_funcs.update({"equal": operator.eq})
         all_funcs = {}
         all_funcs.update(builtin_funcs)
         all_funcs.update(operator_funcs)
-        all_funcs.update(
-            {
-                "is_greater_or_equal": lambda a, b: a >= b,
-                "equal_ignore_case": lambda a, b: a.lower() == b.lower(),
-            }
-        )
         return all_funcs
 
     @staticmethod
+    def easysql_funcs() -> Dict[str, Callable]:
+        return EASYSQL_FUNCS
+
+    @staticmethod
     def create(backend: Backend) -> "FuncRunner":
         all_funcs = FuncRunner.system_funcs()
+        all_funcs.update(FuncRunner.easysql_funcs())
 
         if isinstance(backend, (SparkBackend,)):
             all_funcs.update(FuncRunner._get_spark_funcs(backend))
         elif isinstance(backend, (RdbBackend,)):
             all_funcs.update(FuncRunner._get_rdb_funcs(backend))
+        elif isinstance(backend, (FlinkBackend,)):
+            all_funcs.update(FuncRunner._get_flink_funcs(backend))
 
         FuncRunner._instance = FuncRunner(all_funcs)
         return FuncRunner._instance
 
     @staticmethod
     def _get_rdb_funcs(backend) -> Dict[str, Callable]:
         from easy_sql.sql_processor.funcs_rdb import (
             AnalyticsFuncs,
             ColumnFuncs,
             IOFuncs,
             ModelFuncs,
             PartitionFuncs,
             TableFuncs,
+            TestFuncs,
         )
 
         partition_funcs = PartitionFuncs(backend)
         col_funcs = ColumnFuncs(backend)
         table_funcs = TableFuncs(backend)
         model_funcs = ModelFuncs(backend)
         io_funcs = IOFuncs()
         ana_funcs = AnalyticsFuncs(backend)
+        test_funcs = TestFuncs(backend)
         return {
             "partition_exists": partition_funcs.partition_exists,
             "partition_not_exists": partition_funcs.partition_not_exists,
             "is_first_partition": partition_funcs.is_first_partition,
             "is_not_first_partition": partition_funcs.is_not_first_partition,
             "previous_partition_exists": partition_funcs.previous_partition_exists,
             "get_partition_or_first_partition": partition_funcs.get_partition_or_first_partition,
@@ -95,38 +104,74 @@
             "bq_model_predict_with_local_spark": model_funcs.bq_model_predict_with_local_spark,
             "model_predict_with_local_spark": model_funcs.model_predict_with_local_spark,
             "ensure_no_null_data_in_table": table_funcs.ensure_no_null_data_in_table,
             "check_not_null_column_in_table": table_funcs.check_not_null_column_in_table,
             "all_cols_prefixed_with_exclusion_expr": col_funcs.all_cols_prefixed_with_exclusion_expr,
             "move_file": io_funcs.move_file,
             "data_profiling_report": ana_funcs.data_profiling_report,
+            "sleep": test_funcs.sleep,
+        }
+
+    @staticmethod
+    def _get_flink_funcs(backend) -> Dict[str, Callable]:
+        from easy_sql.sql_processor.funcs_flink import (
+            AnalyticsFuncs,
+            ColumnFuncs,
+            ParallelismFuncs,
+            StreamingFuncs,
+            TableFuncs,
+            TestFuncs,
+        )
+
+        parallelism_funcs = ParallelismFuncs(backend)
+        col_funcs = ColumnFuncs(backend)
+        table_funcs = TableFuncs(backend)
+        ana_funcs = AnalyticsFuncs(backend)
+        streaming_funcs = StreamingFuncs(backend)
+        test_funcs = TestFuncs(backend)
+        return {
+            "all_cols_without_one_expr": col_funcs.all_cols_without_one_expr,
+            "all_cols_with_exclusion_expr": col_funcs.all_cols_with_exclusion_expr,
+            "all_cols_prefixed_with_exclusion_expr": col_funcs.all_cols_prefixed_with_exclusion_expr,
+            "ensure_no_null_data_in_table": table_funcs.ensure_no_null_data_in_table,
+            "check_not_null_column_in_table": table_funcs.check_not_null_column_in_table,
+            "data_profiling_report": ana_funcs.data_profiling_report,
+            "set_parallelism": parallelism_funcs.set_parallelism,
+            "execute_streaming_inserts": streaming_funcs.execute_streaming_inserts,
+            "sleep": test_funcs.sleep,
+            "test_run_etl": test_funcs.test_run_etl,
+            "exec_sql_in_source": test_funcs.exec_sql_in_source,
         }
 
     @staticmethod
     def _get_spark_funcs(backend) -> Dict[str, Callable]:
         from easy_sql.sql_processor.funcs_spark import (
             AnalyticsFuncs,
             CacheFuncs,
             ColumnFuncs,
             IOFuncs,
+            LangFuncs,
             ModelFuncs,
             ParallelismFuncs,
             PartitionFuncs,
             TableFuncs,
+            TestFuncs,
         )
 
         spark = backend.spark
         partition_funcs = PartitionFuncs(backend)
         parallelism_funcs = ParallelismFuncs(spark)
         cache_funcs = CacheFuncs(spark)
         col_funcs = ColumnFuncs(backend)
         table_funcs = TableFuncs(backend)
         io_funcs = IOFuncs(spark)
         model_funcs = ModelFuncs(spark)
         ana_funcs = AnalyticsFuncs(backend)
+        test_funcs = TestFuncs(backend)
+        lang_funcs = LangFuncs(backend)
         return {
             "repartition": parallelism_funcs.repartition,
             "repartition_by_column": parallelism_funcs.repartition_by_column,
             "coalesce": parallelism_funcs.coalesce,
             "set_shuffle_partitions": parallelism_funcs.set_shuffle_partitions,
             "partition_exists": partition_funcs.partition_exists,
             "partition_not_exists": partition_funcs.partition_not_exists,
@@ -152,23 +197,39 @@
             "write_csv": io_funcs.write_csv,
             "rename_csv_output": io_funcs.rename_csv_output,
             "move_file": io_funcs.move_file,
             "write_json_local": io_funcs.write_json_local,
             "update_json_local": io_funcs.update_json_local,
             "model_predict": model_funcs.model_predict,
             "data_profiling_report": ana_funcs.data_profiling_report,
+            "call_java": lang_funcs.call_java,
+            "sleep": test_funcs.sleep,
         }
 
-    def run_func(self, func_def: str, vars_replacer: VarsReplacer) -> bool:
+    def run_func(self, func_def: str, vars_replacer: VarsReplacer) -> Optional[str]:
+        func_name, func, params = self._parse(func_def, vars_replacer)
+        ret_val = func(*params)
+        return self._ref_sql(func_name, func, ret_val, *params)
+
+    def _ref_sql(self, func_name, func, func_call_ret: str, *params) -> str:
+        if hasattr(func, "ref_sql"):
+            assert callable(
+                func.ref_sql
+            ), f"Ref_sql of {func_name} should be a function to calculate the reference sql. But it is a {func.ref_sql}"
+            return func.ref_sql(*params) + "\n;"
+        else:
+            return func_call_ret
+
+    def _parse(self, func_def: str, vars_replacer: VarsReplacer) -> Tuple[str, Callable, List[str]]:
         func_name = func_def[: func_def.index("(")]
         if func_name not in self.funcs:
             raise SqlProcessorException(f"no function found for {func_def} in sql_processor: {func_def}")
         func = self.funcs[func_name]
         try:
             original_params = func_def[func_def.index("(") + 1 : func_def.index(")")].strip()
         except ValueError:
             raise SqlProcessorException("parse params failed for func definition: " + func_def)
         params = []
         if original_params:
             params = original_params.split(",")
             params = [vars_replacer.replace_variables(p.strip(), False) for p in params]
-        return func(*params)
+        return func_name, func, params
```

### Comparing `easy_sql-easy_sql-0.5.1/easy_sql/sql_processor/funcs_common.py` & `easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/funcs_common.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from typing import TYPE_CHECKING, List, Optional, Union
 
 from ..logger import logger
 from . import SqlProcessorException
 
 if TYPE_CHECKING:
     import pandas as pd
+    from sqlalchemy.engine import Connection
 
     from .backend import Backend
     from .backend.rdb import RdbBackend
     from .context import ProcessorContext
     from .step import Step
 
 
@@ -325,63 +326,107 @@
 
 
 class IOFuncs:
     def move_file(self, source_file: str, target_file: str):
         if not os.path.exists(source_file):
             raise FileNotFoundError(source_file)
         os.makedirs(os.path.dirname(target_file), exist_ok=True)
-        os.rename(source_file, target_file)
+        if os.path.exists(target_file):
+            os.remove(target_file)
+        try:
+            os.rename(source_file, target_file)
+        except OSError:
+            with open(target_file, "w") as fw, open(source_file, "r") as fr:
+                fw.write(fr.read())
+            os.remove(source_file)
         logger.info(f"file moved: {source_file} -> {target_file}")
 
 
 class AnalyticsFuncs:
     def __init__(self, backend: Backend) -> None:
         self.backend = backend
 
-    def data_profiling_report(self, table: str, query: str, output_folder: str, max_count=50000):
-        from pandas_profiling import ProfileReport
+    def data_profiling_report(
+        self,
+        table: str,
+        query: str,
+        output_folder: str,
+        max_count: str = "50000",
+        include_correlations: str = "true",
+        types: Union[str, List[str]] = "html",
+    ):
+        try:
+            from ydata_profiling import ProfileReport
+        except ModuleNotFoundError:
+            from pandas_profiling import ProfileReport
 
         from easy_sql.sql_processor.backend.rdb import RdbBackend
 
+        if isinstance(types, str):
+            types = [t.strip() for t in types.split(",") if t.strip()]
+        for type in types:
+            if type not in ["html", "json"]:
+                raise Exception(f"Found unknown type {type}, all supported are: html/json")
+
+        _max_count = int(max_count)
+
         backend = self.backend
         if backend.is_rdb_backend:
             if backend.is_bigquery_backend:
                 raise Exception(f"Not supported backend: {backend.__class__}")
             assert isinstance(backend, RdbBackend)
-            df = self._read_data_rdb(backend, table, query, max_count)
+            df = self._read_data_rdb(backend, table, query, _max_count)
         elif backend.is_spark_backend:
-            df = self._read_data_spark(backend, table, query, max_count)
+            df = self._read_data_spark(backend, table, query, _max_count)
         else:
             raise Exception(f"Not supported backend: {backend.__class__}")
 
         if df is None:
             return
 
-        profile = ProfileReport(df, title=f"Profiling Report for {table}")
+        _include_correlations = include_correlations.lower() in ["1", "true", "y", "yes"]
+        if _include_correlations:
+            profile = ProfileReport(df, title=f"Profiling Report for {table}")
+        else:
+            logger.info("profiling with no correlations...")
+            profile = ProfileReport(
+                df,
+                title=f"Profiling Report for {table}",
+                correlations=None,
+                vars={"num": {"chi_squared_threshold": False}, "cat": {"chi_squared_threshold": False}},
+                interactions={"targets": [], "continuous": False},
+            )
 
         if "." in table:
             db, table = tuple(table.split("."))
             profiling_file = f"{output_folder}/{db}/{table}.html"
         else:
             profiling_file = f"{output_folder}/{table}.html"
         os.makedirs(os.path.dirname(profiling_file), exist_ok=True)
 
-        profile.to_file(profiling_file)
-        logger.info(f"generated file: {profiling_file}")
+        if "html" in types:
+            profile.to_file(profiling_file)
+            logger.info(f"generated file: {profiling_file}")
+        if "json" in types:
+            profiling_file = profiling_file[: profiling_file.rindex(".")] + ".json"
+            with open(profiling_file, "w") as f:
+                f.write(profile.to_json())
+            logger.info(f"generated file: {profiling_file}")
 
     def _read_data_rdb(self, backend: RdbBackend, table: str, query: str, max_count: int) -> pd.DataFrame:
         import pandas as pd
         from sqlalchemy.sql import text
 
         rand_func = "rand" if backend.is_clickhouse_backend else "random"
         condition_sql = "where " + query if query else ""
         sql = f"select * from {table} {condition_sql} order by {rand_func}() limit {max_count}"
         with backend.engine.connect().execution_options(autocommit=True) as conn:
-            query = conn.execute(text(sql))
-        return pd.DataFrame(query.fetchall())
+            conn: Connection = conn
+            query_result = conn.execute(text(sql))
+        return pd.DataFrame(query_result.fetchall())
 
     def _read_data_spark(self, backend: Backend, table: str, query: str, max_count: int) -> Optional[pd.DataFrame]:
         from pyspark.sql.functions import expr
         from pyspark.sql.types import ArrayType, DecimalType, MapType
 
         condition_sql = "where " + query if query else ""
         sql = f"select count(*) from {table} {condition_sql}"
@@ -402,7 +447,21 @@
                 # cast decimal to double to avoid pandas object type after converting later on
                 spark_df = spark_df.withColumn(field.name, expr(f"cast(`{field.name}` as double)"))
             if isinstance(field.dataType, (ArrayType, MapType)):
                 spark_df = spark_df.withColumn(field.name + "__size", expr(f"size(`{field.name}`)"))
 
         df = spark_df.toPandas()
         return df
+
+
+class TestFuncs:
+    def __init__(self, backend: Backend) -> None:
+        self.backend = backend
+
+    def sleep(self, secs: str):
+        try:
+            _secs = float(secs)
+        except ValueError:
+            raise Exception(f"secs must be an float when sleep, got `{secs}`")
+        import time
+
+        time.sleep(_secs)
```

### Comparing `easy_sql-easy_sql-0.5.1/easy_sql/sql_processor/funcs_itest.py` & `easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/funcs_itest.py`

 * *Files 6% similar despite different names*

```diff
@@ -96,14 +96,23 @@
 
         self._test_ana_funcs(backend)
 
     def _test_ana_funcs(self, backend):
         f = AnalyticsFuncs(backend)
         f.data_profiling_report(self.test_table_name, "1=1", "/tmp/easysql-ut/ana-test/")
         self.assertTrue(os.path.exists("/tmp/easysql-ut/ana-test/t/func_test.html"))
+        f.data_profiling_report(
+            self.test_table_name,
+            "1=1",
+            "/tmp/easysql-ut/ana-test/",
+            include_correlations="false",
+            types="html,json",
+        )
+        self.assertTrue(os.path.exists("/tmp/easysql-ut/ana-test/t/func_test.html"))
+        self.assertTrue(os.path.exists("/tmp/easysql-ut/ana-test/t/func_test.json"))
 
     def run_test(self, backend: Backend, types: Tuple[str, str, str]):
         try:
             self._run_test(backend, types)
         finally:
             backend.clean()
```

### Comparing `easy_sql-easy_sql-0.5.1/easy_sql/sql_processor/funcs_rdb.py` & `easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/funcs_rdb.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,17 +9,26 @@
     from pyspark.sql import DataFrame
 
 from ..logger import logger
 from .backend.rdb import RdbBackend
 from .common import is_int_type
 from .funcs_common import AlertFunc, AnalyticsFuncs, ColumnFuncs, IOFuncs
 from .funcs_common import PartitionFuncs as PartitionFuncsBase
-from .funcs_common import TableFuncs
+from .funcs_common import TableFuncs, TestFuncs
 
-__all__ = ["PartitionFuncs", "ColumnFuncs", "AlertFunc", "TableFuncs", "ModelFuncs", "IOFuncs", "AnalyticsFuncs"]
+__all__ = [
+    "PartitionFuncs",
+    "ColumnFuncs",
+    "AlertFunc",
+    "TableFuncs",
+    "ModelFuncs",
+    "IOFuncs",
+    "AnalyticsFuncs",
+    "TestFuncs",
+]
 
 
 class Settings:
     def __init__(self, root_key: str) -> None:
         workdir = os.path.dirname(os.environ.get("PWD"))  # type: ignore
         self.local_settings_file = f"{workdir}/settings.local.json"
         self.settings_file = f"{workdir}/settings.json"
```

### Comparing `easy_sql-easy_sql-0.5.1/easy_sql/sql_processor/funcs_spark.py` & `easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/funcs_spark.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing import TYPE_CHECKING, Dict, List, Union
 
 from .backend import SparkBackend
 from .common import SqlProcessorAssertionError, _exec_sql, is_int_type
 from .funcs_common import AlertFunc, AnalyticsFuncs, ColumnFuncs
 from .funcs_common import IOFuncs as CommonIOFuncs
 from .funcs_common import PartitionFuncs as PartitionFuncsBase
-from .funcs_common import TableFuncs
+from .funcs_common import TableFuncs, TestFuncs
 
 if TYPE_CHECKING:
     from pyspark.sql import DataFrame, SparkSession
     from pyspark.sql.types import Row
 
     from easy_sql.sql_processor.context import ProcessorContext
 
@@ -24,14 +24,16 @@
     "CacheFuncs",
     "ParallelismFuncs",
     "IOFuncs",
     "AlertFunc",
     "TableFuncs",
     "ModelFuncs",
     "AnalyticsFuncs",
+    "LangFuncs",
+    "TestFuncs",
 ]
 
 from ..logger import logger
 
 
 class ParallelismFuncs:
     def __init__(self, spark: SparkSession):
@@ -186,7 +188,21 @@
         pt_col_start = False
         for col in all_cols:
             if pt_col_start:
                 pt_cols.append(col[0].strip())
             if col[0].strip() == "# col_name":
                 pt_col_start = True
         return pt_cols
+
+
+class LangFuncs:
+    def __init__(self, backend: SparkBackend) -> None:
+        self.backend = backend
+
+    def call_java(self, cls: str, func_name: str, *args) -> str:
+        spark = self.backend.spark
+        gw = spark.sparkContext._gateway  # type: ignore
+        from py4j.java_gateway import java_import
+
+        java_import(gw.jvm, cls)
+        func = eval(f"gw.jvm.{cls}.{func_name}", {"gw": gw})
+        return func(spark._jsparkSession, *args)  # type: ignore
```

### Comparing `easy_sql-easy_sql-0.5.1/easy_sql/sql_processor/report.py` & `easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/report.py`

 * *Files identical despite different names*

### Comparing `easy_sql-easy_sql-0.5.1/easy_sql/sql_processor/sql_processor.py` & `easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/sql_processor.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional, Union
 
 from ..logger import logger
 from .backend import Backend, SparkBackend
 from .context import ProcessorContext, TemplatesContext, VarsContext
 from .funcs import FuncRunner
 from .report import SqlProcessorReporter, StepStatus
-from .step import Step, StepFactory
+from .step import ExecutedSqlTransformer, Step, StepFactory
 
 if TYPE_CHECKING:
     from pyspark.sql import SparkSession
 
     from .common import Column
 
 
@@ -24,28 +24,41 @@
     sys.path.insert(0, os.path.dirname(funcs_py_file))
     func_mod = importlib.import_module(os.path.basename(funcs_py_file)[:-3])
     exported_funcs = func_mod.__all__ if hasattr(func_mod, "__all__") else dir(func_mod)
     funcs = {func: getattr(func_mod, func) for func in exported_funcs if callable(getattr(func_mod, func))}
     return funcs
 
 
+class SqlCollector:
+    def __init__(self) -> None:
+        self.sql_lines = []
+
+    def collect_sql(self, sql_lines: str):
+        self.sql_lines.append(sql_lines)
+
+    def collected_sql(self) -> str:
+        return "\n\n".join(self.sql_lines)
+
+
 class SqlProcessor:
     def __init__(
         self,
         backend: Union[SparkSession, Backend],
         sql: str,
         extra_cols: Optional[List[Column]] = None,
         variables: Optional[dict] = None,
         report_hdfs_path: Optional[str] = None,
         report_task_id: Optional[str] = None,
         report_es_url: Optional[str] = None,
         report_es_index_prefix: Optional[str] = None,
         scala_udf_initializer: Optional[str] = None,
         templates: Optional[dict] = None,
         includes: Optional[Dict[str, str]] = None,
+        config: Any = None,
+        executed_sql_transformer: Optional[ExecutedSqlTransformer] = None,
     ):
         backend = backend if isinstance(backend, (Backend,)) else SparkBackend(spark=backend)
         self.backend = backend
         self.sql = sql
 
         self.reporter = SqlProcessorReporter(
             report_task_id=report_task_id or f"easy_sql_task_{random.randint(0, int(1e10))}",
@@ -56,19 +69,23 @@
         log_var_tmpl_replace = False
         vars_context = VarsContext(debug_log=log_var_tmpl_replace, vars=variables)
         self.func_runner = FuncRunner.create(self.backend)
         vars_context.init(self.func_runner)
         self.context = ProcessorContext(
             vars_context, TemplatesContext(debug_log=log_var_tmpl_replace, templates=templates), extra_cols=extra_cols
         )
-        self.step_factory = StepFactory(self.reporter, self.func_runner)
+        self.step_factory = StepFactory(
+            self.reporter, self.func_runner, executed_sql_transformer=executed_sql_transformer
+        )
 
         self.step_list = self.step_factory.create_from_sql(self.sql, includes)
         self.reporter.init(self.step_list)
         self.backend.init_udfs(scala_udf_initializer=scala_udf_initializer)
+        self.config = config
+        self.sql_collector = SqlCollector()
 
     @property
     def variables(self) -> Dict[str, Any]:
         return self.context.vars_context.vars
 
     @property
     def templates(self) -> Dict[str, str]:
@@ -107,20 +124,22 @@
 
     def run_step(self, step: Step, dry_run: bool):
         try:
             # add meta vars to support step information retrieving in functions
             self.context.add_vars({"__step__": step})
             self.context.add_vars({"__context__": self.context})
             self.context.add_vars({"__backend__": self.backend})
+            self.context.add_vars({"__config__": self.config})
             if not step.should_run(self.context):
                 self.reporter.collect_report(step, status=StepStatus.SKIPPED)
                 return
             self.reporter.collect_report(step, status=StepStatus.RUNNING)
             df = step.read(self.backend, self.context)
             step.write(self.backend, df, self.context, dry_run)
+            self.sql_collector.collect_sql(step.get_executed_sql())
             self.reporter.collect_report(step, status=StepStatus.SUCCEEDED)
         except Exception as e:
             import traceback
 
             self.reporter.collect_report(step, status=StepStatus.FAILED, message=traceback.format_exc())
             if (
                 "__exception_handler__" in self.variables
```

### Comparing `easy_sql-easy_sql-0.5.1/easy_sql/sql_processor/step.py` & `easy_sql_easy_sql-1.0.0/easy_sql/sql_processor/step.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,33 +2,71 @@
 
 import re
 import uuid
 from os import path
 from typing import TYPE_CHECKING, Dict, List, Optional
 
 from easy_sql.sql_processor.backend.rdb import RdbBackend
+from easy_sql.utils.sql_expr import CommentSubstitutor
 
 from ..logger import logger
 from .backend import Backend, Partition, SaveMode
 from .backend import Table as BackendTable
 from .backend import TableMeta as Table
 from .common import SqlProcessorException
 
 if TYPE_CHECKING:
     from .context import ProcessorContext
     from .funcs import FuncRunner
 
-__all__ = ["StepConfig", "Step", "StepType", "ReportCollector", "StepFactory"]
+__all__ = ["StepConfig", "Step", "StepType", "ReportCollector", "StepFactory", "ExecutedSqlTransformer", "SqlCleaner"]
 
 
 class ReportCollector:
     def collect_report(self, step: Step, status: Optional[str] = None, message: Optional[str] = None):
         raise NotImplementedError()
 
 
+class EmptyReportCollector(ReportCollector):
+    def collect_report(self, step: Step, status: Optional[str] = None, message: Optional[str] = None):
+        logger.info(f"collect report for step: {str(step)}, status: {status}, message: {message}")
+
+
+class SqlCleaner:
+    def __init__(self) -> None:
+        self.comment_substituter = CommentSubstitutor()
+
+    def clean_sql(self, sql: str) -> str:
+        """
+        Clean a sql with comments and semicolon to form a clean select sql, in order to be used to construct a new sql.
+        It works as below:
+        - remove leading comments
+        - remove tail comments
+        - remove the last semicolon
+        """
+        sql_lines = sql.split("\n")
+        for i, sql_line in enumerate(sql_lines):
+            sql_line = sql_line.strip()
+            if sql_line and not sql_line.startswith("--"):
+                sql_lines = sql_lines[i:]
+                sql_lines[0] = sql_line
+                break
+        sql_lines.reverse()
+        for i, sql_line in enumerate(sql_lines):
+            sql_line = sql_line.strip()
+            if sql_line and not sql_line.startswith("--") and not sql_line.startswith(";"):
+                sql_lines = sql_lines[i:]
+                sql_lines[0] = sql_line
+                break
+        sql_lines.reverse()
+        sql_lines[-1] = self.comment_substituter.remove(sql_lines[-1]).rstrip().rstrip(";")
+        clean_sql = "\n".join(sql_lines)
+        return clean_sql
+
+
 class StepConfig:
     STEP_CONFIG_PATTERN = r"^-- target\s*=\s*(\w+)(.*)$"
 
     def __init__(
         self,
         step_type: str,
         step_name: Optional[str],
@@ -76,16 +114,16 @@
             condition_match = re.compile(r"^\s*(,)\s*if\s*=(.*$)").match(configs[len(target_type) :])
         if condition_match:
             target_name = condition_match.group(1) if target_name is not None else None
             target_condition = condition_match.group(2).strip()
             reg_exp = r"[a-zA-Z0-9_]*\([^()]*\)"
             if not re.compile(reg_exp).match(target_condition):
                 raise SqlProcessorException(
-                    f"parse step config failed. condition must be like {reg_exp}, "
-                    f"but got {target_condition}. config_line={config_line}"
+                    f"parse step config failed. condition must be like {reg_exp}, but got {target_condition}."
+                    f" config_line={config_line}"
                 )
 
         return StepConfig(
             step_name=target_name,
             step_type=target_type,
             condition=target_condition,
             line_no=line_no,
@@ -127,30 +165,65 @@
             StepType.BROADCAST,
             StepType.OUTPUT,
             StepType.LIST_VARIABLES,
             StepType.ACTION,
         ]
 
 
+class ExecutedSqlTransformer:
+    def transform_create_view_sql(self, view_name: str, select_sql: str):
+        raise NotImplementedError()
+
+    def transform_save_table_sql(self, table_name: str, select_sql: str):
+        raise NotImplementedError()
+
+
+class SimpleExecutedSqlTransformer(ExecutedSqlTransformer):
+    def __init__(self) -> None:
+        self._sql_cleaner = SqlCleaner()
+        super().__init__()
+
+    def cleaned_select_sql(self, sql: str) -> Optional[str]:
+        return self._sql_cleaner.clean_sql(sql)
+
+    def transform_create_view_sql(self, view_name: str, select_sql: str):
+        clean_sql = self._sql_cleaner.clean_sql(select_sql)
+        assert clean_sql is not None
+        if re.match(r"^with\s", clean_sql, re.I):
+            return f"create view {view_name} as (\n{clean_sql}\n);"
+        return f"insert overwrite {view_name} \n{clean_sql}\n;"
+
+    def transform_save_table_sql(self, table_name: str, select_sql: str):
+        clean_sql = self._sql_cleaner.clean_sql(select_sql)
+        assert clean_sql is not None
+        if re.match(r"^with\s", clean_sql, re.I):
+            return f"insert overwrite {table_name} (\n{clean_sql}\n);"
+        return f"insert overwrite {table_name} \n{clean_sql}\n;"
+
+
 class Step:
     def __init__(
         self,
         id: str,
         reporter_collector: ReportCollector,
         func_runner: FuncRunner,
         target_config: Optional[StepConfig] = None,
         select_sql: Optional[str] = None,
         debug_var_tmpl_replace: bool = False,
+        *,
+        executed_sql_transformer: Optional[ExecutedSqlTransformer] = None,
     ):
         self.id = id
         self.target_config = target_config
         self.select_sql = select_sql
         self.debug_var_tmpl_replace = debug_var_tmpl_replace
         self.reporter_collector = reporter_collector
         self.func_runner = func_runner
+        self.executed_sql: Optional[str] = None
+        self.executed_sql_transformer = executed_sql_transformer or SimpleExecutedSqlTransformer()
 
     def __str__(self):
         return str(self.target_config).replace("StepConfig(", "Step(", 1)
 
     def __repr__(self):
         return f"[\n    config: {self.target_config},\n    sql: {self.select_sql}\n]"
 
@@ -183,14 +256,23 @@
             return backend.exec_sql(self.select_sql)
 
     def preprocess_select_sql(self, context: ProcessorContext):
         assert self.select_sql is not None
         self.select_sql = context.replace_templates(self.select_sql)
         self.select_sql = context.replace_variables(self.select_sql)
 
+    def get_executed_sql(self) -> str:
+        return self.executed_sql or ""
+
+    def _create_view_sql(self) -> str:
+        assert self.target_config is not None
+        assert self.target_config.name is not None
+        assert self.select_sql is not None
+        return self.executed_sql_transformer.transform_create_view_sql(self.target_config.name, self.select_sql)
+
     def write(self, backend: Backend, table: Optional[BackendTable], context: ProcessorContext, dry_run: bool = False):
         assert self.target_config is not None
         variables: dict = context.vars_context.vars
 
         if not table:
             return
 
@@ -217,34 +299,37 @@
             assert self.select_sql is not None
             assert self.target_config.name is not None
             context.add_templates({self.target_config.name: self.select_sql})
 
         elif StepType.TEMP == self.target_config.step_type:
             assert self.target_config.name is not None
             backend.create_temp_table(table, self.target_config.name)
+            self.executed_sql = self._create_view_sql()
 
         elif StepType.CACHE == self.target_config.step_type:
             assert self.target_config.name is not None
             if "__no_cache__" in variables and variables["__no_cache__"] in ["TRUE", True, 1, "True", "true"]:
                 backend.create_temp_table(table, self.target_config.name)
             else:
                 backend.create_cache_table(table, self.target_config.name)
+            self.executed_sql = self._create_view_sql()
 
         elif StepType.BROADCAST == self.target_config.step_type:
             assert self.target_config.name is not None
             backend.broadcast_table(table, self.target_config.name)
+            self.executed_sql = self._create_view_sql()
 
         elif StepType.LOG == self.target_config.step_type:
             if "__no_log__" in variables and variables["__no_log__"] in ["TRUE", True, 1, "True", "true"]:
                 return
             self._write_for_log_step(table)
 
         elif StepType.FUNC == self.target_config.step_type:
             assert self.target_config.name is not None
-            self.func_runner.run_func(self.target_config.name, context.vars_context)
+            self.executed_sql = self.func_runner.run_func(self.target_config.name, context.vars_context)
 
         elif StepType.CHECK == self.target_config.step_type:
             if self._should_skip_check(variables):
                 return
             self._write_for_check_step(table, context)
 
         elif self.target_config.step_type in [StepType.HIVE, StepType.OUTPUT]:
@@ -318,43 +403,52 @@
             if static_partition_name:
                 if backend.is_spark_backend:
                     from pyspark.sql.functions import lit
 
                     table = table.with_column(static_partition_name, lit(static_partition_value))
                 else:
                     assert isinstance(backend, RdbBackend)
-                    table = table.with_column(
-                        static_partition_name, backend.sql_expr.for_value(static_partition_value)  # type: ignore
-                    )
+                    partition_value = backend.sql_expr.for_value(static_partition_value)  # type: ignore
+                    table = table.with_column(static_partition_name, partition_value)
             backend.create_temp_table(table, temp_table_name + "_output")  # type: ignore
             self.collect_report(message="will not save data to data warehouse, since we are in dry run mode")
+            # may need to provide a more accurate sql
+            assert self.select_sql is not None
+            self.executed_sql = self.executed_sql_transformer.transform_save_table_sql(
+                target_table.table_name, self.select_sql
+            )
             return
 
         target_table_exists = backend.table_exists(target_table)
         if not target_table_exists and not create_output_table:
             message = f"target table {target_table.table_name} not exists"
             self.collect_report(message=message)
             raise Exception(message)
 
         backend.save_table(source_table, target_table, save_mode, create_target_table=create_output_table)
+        # may need to provide a more accurate sql
+        assert self.select_sql is not None
+        self.executed_sql = self.executed_sql_transformer.transform_save_table_sql(
+            target_table.table_name, self.select_sql
+        )
 
     def _write_for_log_step(self, df: BackendTable):
         assert self.target_config is not None
         assert self.target_config.name is not None
         log_data = df.limit(20).collect()
         if len(log_data) == 0:
             logger.info(f"log for [{self.target_config.name}]: no data to show")
             self.collect_report(message="no data to show")
         elif len(log_data) == 1:
             logger.info(f"log for [{self.target_config.name}]: {str(log_data[0])}")
             self.collect_report(message=f"{str(log_data[0])}")
         else:
             logger.info(f"log for [{self.target_config.name}]: ")
             df.show(20)
-            self.collect_report(message=f"{str(log_data[0])}")
+            self.collect_report(message="\n".join([str(row) for row in log_data]))
 
     def _write_for_check_step(self, df: BackendTable, context: ProcessorContext):
         assert self.target_config is not None
         if self.target_config.is_target_name_a_func():
             assert self.target_config.name is not None
             if not self.func_runner.run_func(self.target_config.name, context.vars_context):
                 message = (
@@ -394,36 +488,52 @@
         self.collect_report(message=f"check_data(limit 100)={check_data}")
 
     def collect_report(self, status=None, message=None):
         self.reporter_collector.collect_report(self, status=status, message=message)
 
 
 class StepFactory:
-    def __init__(self, reporter: ReportCollector, func_runner: FuncRunner):
+    def __init__(
+        self,
+        reporter: ReportCollector,
+        func_runner: FuncRunner,
+        executed_sql_transformer: Optional[ExecutedSqlTransformer] = None,
+    ):
         self.reporter = reporter
         self.func_runner = func_runner
+        self.executed_sql_transformer = executed_sql_transformer
 
     def create_from_sql(self, sql: str, includes: Optional[Dict[str, str]] = None) -> List[Step]:
         includes = includes or {}
         resolved_sql = self._resolve_include(sql, includes)
         lines = resolved_sql.split("\n")
 
         index = 0
         sql_parts = []
         step_list = []
-        step = Step(f"step-{len(step_list) + 1}", self.reporter, self.func_runner)
+        step = Step(
+            f"step-{len(step_list) + 1}",
+            self.reporter,
+            self.func_runner,
+            executed_sql_transformer=self.executed_sql_transformer,
+        )
         while index < len(lines):
             line = lines[index].replace(";", "")
             line_stripped = line.strip()
             if re.compile(StepConfig.STEP_CONFIG_PATTERN, flags=re.IGNORECASE).match(line_stripped):
                 if len(sql_parts) > 0:
                     step.select_sql = "\n".join(sql_parts)
                 if step.target_config is not None:
                     step_list.append(step)
-                step = Step(f"step-{len(step_list) + 1}", self.reporter, self.func_runner)
+                step = Step(
+                    f"step-{len(step_list) + 1}",
+                    self.reporter,
+                    self.func_runner,
+                    executed_sql_transformer=self.executed_sql_transformer,
+                )
                 sql_parts = []
                 target_config = StepConfig.from_config_line(line_stripped, index + 1)
                 step.target_config = target_config
                 if index == len(lines) - 1:
                     step_list.append(step)
             elif index == len(lines) - 1:
                 if "" != line_stripped:
```

### Comparing `easy_sql-easy_sql-0.5.1/easy_sql/sql_processor_debugger.py` & `easy_sql_easy_sql-1.0.0/easy_sql/sql_processor_debugger.py`

 * *Files identical despite different names*

### Comparing `easy_sql-easy_sql-0.5.1/easy_sql/sql_processor_debugger_itest.py` & `easy_sql_easy_sql-1.0.0/easy_sql/sql_processor_debugger_itest.py`

 * *Files identical despite different names*

### Comparing `easy_sql-easy_sql-0.5.1/easy_sql/sql_processor_itest.py` & `easy_sql_easy_sql-1.0.0/easy_sql/sql_processor_itest.py`

 * *Files identical despite different names*

### Comparing `easy_sql-easy_sql-0.5.1/easy_sql/sql_processor_test.py` & `easy_sql_easy_sql-1.0.0/easy_sql/sql_processor_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -324,17 +324,19 @@
     def test_should_raise_error_when_output_table_name_does_not_contain_dbname(self):
         processor = SqlProcessor(LocalSpark.get(), "-- target=output.some_table\nselect 1 as actual, 0 as expected")
         self.assertRaises(Exception, lambda: processor.run())
 
     def test_should_do_action_step_ok(self):
         processor = SqlProcessor(
             LocalSpark.get(),
-            "-- target=variables\nselect true as __create_output_table__\n"
-            "-- target=output.t.some_table\nselect 1 as a, 0 as b\n"
-            "-- target=action.some_action\ndrop table t.some_table",
+            (
+                "-- target=variables\nselect true as __create_output_table__\n"
+                "-- target=output.t.some_table\nselect 1 as a, 0 as b\n"
+                "-- target=action.some_action\ndrop table t.some_table"
+            ),
         )
         processor.run()
         from easy_sql.sql_processor.backend import TableMeta
 
         self.assertFalse(processor.backend.table_exists(TableMeta("t.some_table")))
 
     def test_should_add_static_partition_value_for_dryrun_as_well(self):
@@ -380,15 +382,24 @@
                     "1",
                     "1",
                     20210102,
                 ),
             ],
             ["id", "fk1", "fk2", "pt"],
         ).write.mode("overwrite").partitionBy("pt").saveAsTable("data_table")
-        spark.createDataFrame([(1, "1", 20210101,)], ["id", "fk", "pt"]).write.mode("overwrite").partitionBy(
+        spark.createDataFrame(
+            [
+                (
+                    1,
+                    "1",
+                    20210101,
+                )
+            ],
+            ["id", "fk", "pt"],
+        ).write.mode("overwrite").partitionBy(
             "pt"
         ).saveAsTable("data_table1")
         # failure case1: 被检测表是空的
         processor = SqlProcessor(
             spark, "-- target=check.ensure_dwd_partition_exists(${__step__}, empty_table, 20210101)", [], {}
         )
         with self.assertRaises(Exception):  # noqa: B017
@@ -460,15 +471,23 @@
         processor.run(dry_run=True)
 
     def test_ensure_partition_or_first_partition_exists(self):
         spark = LocalSpark.get()
         spark.createDataFrame(
             [], StructType([StructField("id", IntegerType()), StructField("pt", IntegerType())])
         ).write.mode("overwrite").partitionBy("pt").saveAsTable("empty_table")
-        spark.createDataFrame([(1, 20210101,)], ["id", "pt"]).write.mode("overwrite").partitionBy(
+        spark.createDataFrame(
+            [
+                (
+                    1,
+                    20210101,
+                )
+            ],
+            ["id", "pt"],
+        ).write.mode("overwrite").partitionBy(
             "pt"
         ).saveAsTable("data_table")
         # failure case1: 被检测表是空的
         processor = SqlProcessor(
             spark,
             "-- target=check.ensure_partition_or_first_partition_exists(${__step__}, empty_table, 20210101)",
             [],
@@ -495,16 +514,18 @@
         self.assertIn(
             "partition 20210102 not exists: ['data_table']", processor.reporter.step_reports["step-1"].messages
         )
 
         # failure case3: 检测多张表，message 中应该只有检查失败的表
         processor = SqlProcessor(
             spark,
-            "-- target=check.ensure_partition_or_first_partition_exists(${__step__}, empty_table, data_table,"
-            " 20210101)",
+            (
+                "-- target=check.ensure_partition_or_first_partition_exists(${__step__}, empty_table, data_table,"
+                " 20210101)"
+            ),
             [],
             {},
         )
         with self.assertRaises(Exception):  # noqa: B017
             processor.run(dry_run=True)
         assert processor.reporter.step_reports is not None
         self.assertIn(
```

### Comparing `easy_sql-easy_sql-0.5.1/easy_sql/sql_test.py` & `easy_sql_easy_sql-1.0.0/easy_sql/sql_test.py`

 * *Files identical despite different names*

### Comparing `easy_sql-easy_sql-0.5.1/easy_sql/sql_test_itest.py` & `easy_sql_easy_sql-1.0.0/easy_sql/sql_test_itest.py`

 * *Files identical despite different names*

### Comparing `easy_sql-easy_sql-0.5.1/easy_sql/sql_tester.py` & `easy_sql_easy_sql-1.0.0/easy_sql/sql_tester.py`

 * *Files 1% similar despite different names*

```diff
@@ -210,14 +210,15 @@
         table_name: str,
         col_name: str,
         col_value: Any,
         date_converter: Optional[Callable] = None,
         col_type: Optional[str] = None,
     ) -> Tuple[str, Any]:
         col_type = self.get_col_type(table_name, col_name) if col_type is None else col_type
+        col_type = col_type.strip()
         if self.backend == "clickhouse":
             if "Nested" in col_type:
                 raise AssertionError("clickhouse backend can not support Nested col type")
             # for these type in clickhouse is case insensitive
             if col_type.lower() in ["bool", "date", "datetime", "decimal"]:
                 col_type = col_type.lower()
         else:
@@ -249,15 +250,15 @@
                             raise e
 
             if col_type.replace(" ", "").startswith("map<"):
                 raise AssertionError(
                     f"map type not supported right now when parsing value `{col_value}` for column:"
                     f" {table_name}.{col_name}"
                 )
-            if col_type.startswith("decimal(") or col_type == "double":
+            if col_type.startswith("decimal(") or col_type == "double" or col_type == "float":
                 return col_type, float(col_value)
             if col_type in ["bigint", "int", "tinyint", "Int32", "Int64", "UInt32", "UInt64"]:
                 return col_type, int(col_value)
             if col_type in ["boolean", "bool"]:
                 if str(col_value).lower() == "true":
                     return col_type, True
                 elif str(col_value).lower() == "false":
@@ -469,14 +470,16 @@
                 else:
                     columns.append(column_name)
                     column_types.append(self.default_col_type)  # if no type specified, use string as default
             else:
                 columns.append(column_name)
                 if "." in table_name:
                     column_types.append(table_column_types.get_col_type(table_name, columns[-1]))
+                else:
+                    raise Exception(f"Unable to resolve types for table: {table_name}")
 
         values, value_descriptions = [], []
         for row_idx, cells in enumerate(rows[1:]):
             value_cells = cells[2:]
             has_values = any([value_cells[i].value not in [None, ""] for i in range(len(columns))])
             if cells[1].value and str(cells[1].value).strip():
                 value_descriptions.append(str(cells[1].value).strip())
@@ -661,17 +664,19 @@
 class TestResult:
     PASSED = "PASSED"
     FAILED = "FAILED"
 
     def __init__(self, test_data_file: str):
         self.test_data_file = test_data_file
         self.case_results = []
+        self.cases: List[TestCase] = []
 
-    def collect_case_result(self, case_name: str, result: str):
-        self.case_results.append({"case_name": case_name, "result": result})
+    def collect_case_result(self, case: TestCase, result: str):
+        self.cases.append(case)
+        self.case_results.append({"case_name": case.name, "result": result})
 
     @property
     def failed_cases(self):
         return list(filter(lambda cr: cr["result"] == TestResult.FAILED, self.case_results))
 
     @property
     def is_fail(self) -> bool:
@@ -717,27 +722,30 @@
         unit_test_case: Optional[unittest.TestCase],
         sql_processor_creator: Callable,
     ):
         self.unit_test_case = unit_test_case or unittest.TestCase()
         self.env, self.dry_run, self.backend_creator = env, dry_run, backend_creator
         self.sql_processor_creator = sql_processor_creator
         self.table_column_types = table_column_types
+        self.collected_sql = None
 
     def run_test(self, case: TestCase):
         sql = case.read_sql_content()
 
         backend = self.backend_creator(case)
         try:
             self.clean(case, backend)
             self.create_inputs(case, backend)
 
             sql_processor = self.create_sql_processor(backend, case, sql)
 
             sql_processor.run(self.dry_run)
 
+            self.collected_sql = sql_processor.sql_collector.collected_sql()
+
             self.verify_outputs(backend, case)
         finally:
             backend.clean()
 
     def verify_outputs(self, backend: Backend, case: TestCase):
         tempviews = backend.temp_tables()
         print("tempviews after test:", tempviews)
@@ -811,15 +819,15 @@
         for input in case.inputs:
             schema = self.table_column_types.column_types_to_schema(backend, input.columns, input.column_types)
             if "." in input.name:
                 print(f"creating table: {input.name}")
                 pt_col = input.pt_col(list(self.table_column_types.partition_col_types.keys()))
                 backend.create_table_with_data(input.name, input.values, schema, [Partition(pt_col)] if pt_col else [])
             else:
-                print(f"creating temp table: {input.name}")
+                print(f"creating temp table: {input.name}", input.columns, input.column_types)
                 backend.create_temp_table_with_data(input.name, input.values, schema)
 
     def clean(self, case: TestCase, backend: Backend):
         databases = set()
         table_names = set.union({input.name for input in case.inputs}, {output.name for output in case.outputs})
         for table_name in table_names:
             if "." in table_name:
@@ -870,14 +878,15 @@
         self.sql_processor_creator = sql_processor_creator or create_sql_processor
         self.backend = backend
         self.table_column_types = table_column_types or TableColumnTypes({}, {}, backend)
         self.unit_test_case = unit_test_case
         self.dry_run = dry_run
         self.env = env
         self.sql_reader = sql_reader_creator() if sql_reader_creator else SqlReader()
+        self.collected_sql = None
         if backend_creator:
             self.test_case_runner = TestCaseRunner(
                 self.env,
                 self.dry_run,
                 backend_creator,
                 self.table_column_types,
                 sql_processor_creator=self.sql_processor_creator,
@@ -905,15 +914,15 @@
         if case_idx != -1 and (case_idx < 0 or case_idx >= len(cases)):
             raise AssertionError(f"test case {case_idx} not found. {len(cases)} cases in {test_data_file} are found.")
         cases = cases if case_idx == -1 else [cases[case_idx]]
 
         tr = TestResult(test_data_file)
         for case in cases:
             passed = self.run_case(case)
-            tr.collect_case_result(case.name, TestResult.PASSED if passed else TestResult.FAILED)  # type: ignore
+            tr.collect_case_result(case, TestResult.PASSED if passed else TestResult.FAILED)  # type: ignore
         return tr
 
     def parse_test_cases(self, test_data_file, table_column_types: TableColumnTypes) -> List[TestCase]:
         if test_data_file.endswith(".xlsx"):
             cases = TestDataFile(test_data_file, sql_reader=self.sql_reader, backend=self.backend).parse_test_cases(
                 table_column_types
             )
@@ -924,14 +933,15 @@
         else:
             raise AssertionError(f"unsupported format of test file: {test_data_file}")
         return cases
 
     def run_case(self, case: TestCase) -> bool:
         try:
             self.test_case_runner.run_test(case)
+            self.collected_sql = self.test_case_runner.collected_sql
             return True
         except Exception:
             import traceback
 
             traceback.print_exc()
             return False
 
@@ -954,16 +964,23 @@
         import jinja2
 
         env = jinja2.Environment(
             loader=jinja2.DictLoader(
                 {
                     "py_file_tpl": f"""import os
 import unittest
+import sys
+import importlib
 
-from {self.__module__} import SqlTester
+try:
+    sys.path.insert(0, 'common')
+    SqlTester = importlib.import_module('sql_test').SqlTester  # type: ignore
+except ModuleNotFoundError as e:
+    print('using SqlTester from dataplat.')
+    from {self.__module__} import SqlTester
 
 
 class SqlTest(unittest.TestCase):
 
     def __init__(self, methodName='runTest'):
         super().__init__(methodName)
         work_dir = os.environ.get('WORK_DIR')
```

### Comparing `easy_sql-easy_sql-0.5.1/easy_sql/sql_tester_test.py` & `easy_sql_easy_sql-1.0.0/easy_sql/sql_tester_test.py`

 * *Files identical despite different names*

### Comparing `easy_sql-easy_sql-0.5.1/easy_sql/udf/udfs.py` & `easy_sql_easy_sql-1.0.0/easy_sql/udf/udfs.py`

 * *Files identical despite different names*

### Comparing `easy_sql-easy_sql-0.5.1/easy_sql/udf/udfs_test.py` & `easy_sql_easy_sql-1.0.0/easy_sql/udf/udfs_test.py`

 * *Files identical despite different names*

### Comparing `easy_sql-easy_sql-0.5.1/easy_sql/utils/io_utils.py` & `easy_sql_easy_sql-1.0.0/easy_sql/utils/io_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 import os
 import re
 from os import path
 
 from easy_sql.logger import logger
 
 
-def resolve_file(file_path: str, abs_path: bool = False, prefix: str = "") -> str:
+def resolve_file(file_path: str, abs_path: bool = False, prefix: str = "", relative_to: str = "") -> str:
     if file_path.lower().startswith("hdfs://") or file_path.lower().startswith("file://"):
         # do not resolve if it is hdfs or absolute file path
         return file_path
     base_path = os.path.abspath(os.curdir)
     if not path.exists(file_path):
         if path.exists(path.join(base_path, file_path)):
             file_path = path.join(base_path, file_path)
         elif path.exists(path.basename(file_path)):
             file_path = path.basename(file_path)
+        elif relative_to and path.isfile(relative_to) and path.exists(path.join(path.dirname(relative_to), file_path)):
+            file_path = path.join(path.dirname(relative_to), file_path)
+        elif relative_to and path.isdir(relative_to) and path.exists(path.join(relative_to, file_path)):
+            path.join(relative_to, file_path)
         else:
             raise Exception(f"file not found: {file_path}")
     if abs_path:
         file_path = path.abspath(file_path)
     if " " in file_path:
         parts = file_path.split("/")
         file_path_no_space = "/".join([re.sub(r" .*$", "", part) for part in parts])
```

### Comparing `easy_sql-easy_sql-0.5.1/easy_sql/utils/object_utils_test.py` & `easy_sql_easy_sql-1.0.0/easy_sql/utils/object_utils_test.py`

 * *Files identical despite different names*

### Comparing `easy_sql-easy_sql-0.5.1/pyproject.toml` & `easy_sql_easy_sql-1.0.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "easy_sql-easy_sql"
-version = "0.5.1"
+version = "1.0.0"
 description = "A library developed to ease the data ETL development process."
 authors = ["Easy SQL from Thoughtworks <easy_sql@thoughtworks.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/easysql/easy_sql"
 homepage = "https://easy-sql.readthedocs.io"
 
@@ -22,15 +22,15 @@
 "Bug Tracker" = "https://github.com/easysql/easy_sql/issues"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 click = {version = "^8.1.3", optional = true}
 regex = {version = "^2022.7.25", optional = true}
 colorlog = {version = "^6.6.0", optional = true}
-sqlfluff = {version = "~1.2.1", optional = true}
+sqlfluff = {version = "~1.4.5", optional = true}
 SQLAlchemy = {version = "^1.4.40", optional = true}
 clickhouse-driver = {version = "^0.2.4", optional = true}
 clickhouse-sqlalchemy = {version = "^0.2.1", optional = true}
 psycopg2 = {version = "^2.9.3", optional = true}
 pyodps = {version = "^0.11.2.1", optional = true}
 pyspark = [{version = ">=2.3.0, != 3.1.1, != 3.1.2, != 3.1.3, !=3.2.0, != 3.2.1", optional = true}]
```

### Comparing `easy_sql-easy_sql-0.5.1/setup.py` & `easy_sql_easy_sql-1.0.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,47 +1,280 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: easy-sql-easy-sql
+Version: 1.0.0
+Summary: A library developed to ease the data ETL development process.
+Home-page: https://easy-sql.readthedocs.io
+License: Apache-2.0
+Author: Easy SQL from Thoughtworks
+Author-email: easy_sql@thoughtworks.com
+Requires-Python: >=3.7,<4.0
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.8
+Provides-Extra: cli
+Provides-Extra: clickhouse
+Provides-Extra: linter
+Provides-Extra: maxcompute
+Provides-Extra: pg
+Provides-Extra: spark
+Requires-Dist: SQLAlchemy (>=1.4.40,<2.0.0) ; extra == "pg" or extra == "clickhouse"
+Requires-Dist: click (>=8.1.3,<9.0.0) ; extra == "cli"
+Requires-Dist: clickhouse-driver (>=0.2.4,<0.3.0) ; extra == "clickhouse"
+Requires-Dist: clickhouse-sqlalchemy (>=0.2.1,<0.3.0) ; extra == "clickhouse"
+Requires-Dist: colorlog (>=6.6.0,<7.0.0) ; extra == "linter"
+Requires-Dist: psycopg2 (>=2.9.3,<3.0.0) ; extra == "pg"
+Requires-Dist: pyodps (>=0.11.2.1,<0.12.0.0) ; extra == "maxcompute"
+Requires-Dist: pyspark (>=2.3.0,!=3.1.1,!=3.1.2,!=3.1.3,!=3.2.0,!=3.2.1) ; extra == "spark"
+Requires-Dist: regex (>=2022.7.25,<2023.0.0) ; extra == "linter"
+Requires-Dist: sqlfluff (>=1.4.5,<1.5.0) ; extra == "linter"
+Project-URL: Bug Tracker, https://github.com/easysql/easy_sql/issues
+Project-URL: Repository, https://github.com/easysql/easy_sql
+Description-Content-Type: text/markdown
 
-packages = \
-['easy_sql',
- 'easy_sql.cli',
- 'easy_sql.sql_linter',
- 'easy_sql.sql_linter.rules',
- 'easy_sql.sql_processor',
- 'easy_sql.sql_processor.backend',
- 'easy_sql.sql_processor.backend.sql_dialect',
- 'easy_sql.udf',
- 'easy_sql.utils']
-
-package_data = \
-{'': ['*']}
-
-extras_require = \
-{'cli': ['click>=8.1.3,<9.0.0'],
- 'clickhouse': ['SQLAlchemy>=1.4.40,<2.0.0',
-                'clickhouse-driver>=0.2.4,<0.3.0',
-                'clickhouse-sqlalchemy>=0.2.1,<0.3.0'],
- 'linter': ['regex>=2022.7.25,<2023.0.0',
-            'colorlog>=6.6.0,<7.0.0',
-            'sqlfluff>=1.2.1,<1.3.0'],
- 'maxcompute': ['pyodps>=0.11.2.1,<0.12.0.0'],
- 'pg': ['SQLAlchemy>=1.4.40,<2.0.0', 'psycopg2>=2.9.3,<3.0.0'],
- 'spark': ['pyspark>=2.3.0,!=3.1.1,!=3.1.2,!=3.1.3,!=3.2.0,!=3.2.1']}
-
-setup_kwargs = {
-    'name': 'easy-sql-easy-sql',
-    'version': '0.5.1',
-    'description': 'A library developed to ease the data ETL development process.',
-    'long_description': '# Easy SQL\n\nEasy SQL is built to ease the data ETL development process.\nWith Easy SQL, you can develop your ETL in SQL in an imperative way.\nIt defines a few simple syntax on top of standard SQL, with which SQL could be executed one by one.\nEasy SQL also provides a processor to handle all the new syntax.\nSince this is SQL agnostic, any SQL engine could be plugged-in as a backend.\nThere are built-in support for several popular SQL engines, including SparkSQL, PostgreSQL, Clickhouse, FlinkSQL, Aliyun Maxcompute, Google BigQuery.\nMore will be added in the near future.\n\n- Docs: <https://easy-sql.readthedocs.io/>\n- Enterprise extended product: <https://data-workbench.com/>\n\n[![GitHub Action Build](https://github.com/easysql/easy_sql/actions/workflows/build.yaml/badge.svg?branch=main&event=push)](https://github.com/easysql/easy_sql/actions/workflows/build.yaml?query=branch%3Amain+event%3Apush)\n[![Docs Build](https://readthedocs.org/projects/easy-sql/badge/?version=latest)](https://easy-sql.readthedocs.io/en/latest/?badge=latest)\n[![EasySQL Coverage](https://codecov.io/gh/easysql/easy_sql/branch/main/graph/badge.svg)](https://codecov.io/gh/easysql/easy_sql)\n[![PyPI](https://img.shields.io/pypi/v/easy-sql-easy-sql)](https://pypi.org/project/easy-sql-easy-sql/)\n\n## Install Easy SQL\n\nInstall Easy SQL using pip: `python3 -m pip install easy_sql-easy_sql[extra,extra]`\n\nCurrently we are providing below extras, choose according to your need:\n- cli\n- linter\n- spark\n- pg\n- clickhouse\n\nWe also provide flink backend, but because of dependency confliction between pyspark and apache-flink, you need to install the flink backend dependencies manually with the following command `python3 -m pip install apache-flink`.\n\nUsually we read data from some data source and write data to some other system using flink with different connectors. So we need to download some jars for the used connectors as well. Refer [here](https://nightlies.apache.org/flink/flink-docs-release-1.15/docs/connectors/table/overview/) to get more information and [here](https://nightlies.apache.org/flink/flink-docs-release-1.15/docs/connectors/table/downloads/) to download the required connectors.\n\n## Building Easy SQL\n\nInternally we use `poetry` to manage the dependencies. So make sure you have [installed it](https://python-poetry.org/docs/master/#installation). Package could be built with the following make command: `make package-pip` or just `poetry build`.\n\nAfter the above command, there will be a file named `easy_sql*.whl` generated in the `dist` folder.\nYou can install it with command `python3 -m pip install dist/easy_sql*.whl[extra]` or just `poetry install -E \'extra extra\'`.\n\n## First ETL with Easy SQL\n\nInstall easy_sql with spark as the backend: `python3 -m pip install easy_sql-easy_sql[spark,cli]`.\n\n### For spark backend\n\nCreate a file named `sample_etl.spark.sql` with content as below:\n\n```sql\n-- prepare-sql: drop database if exists sample cascade\n-- prepare-sql: create database sample\n-- prepare-sql: create table sample.test as select 1 as id, \'1\' as val\n\n-- target=variables\nselect true as __create_output_table__\n\n-- target=variables\nselect 1 as a\n\n-- target=log.a\nselect \'${a}\' as a\n\n-- target=log.test_log\nselect 1 as some_log\n\n-- target=check.should_equal\nselect 1 as actual, 1 as expected\n\n-- target=temp.result\nselect\n    ${a} as id, ${a} + 1 as val\nunion all\nselect id, val from sample.test\n\n-- target=output.sample.result\nselect * from result\n\n-- target=log.sample_result\nselect * from sample.result\n```\n\nRun it with command:\n\n```bash\nbash -c "$(python3 -m easy_sql.data_process -f sample_etl.spark.sql -p)"\n```\n\n### For postgres backend:\n\nYou need to start a postgres instance first.\n\nIf you have docker, run the command below:\n\n```bash\ndocker run -d --name postgres -p 5432:5432 -e POSTGRES_PASSWORD=123456 postgres\n```\n\nCreate a file named `sample_etl.postgres.sql` with content as the test file [here](https://github.com/easysql/easy_sql/blob/main/test/sample_etl.postgres.sql).\n\nMake sure that you have install the corresponding backend with `python3 -m pip install easy-sql-easy-sql[cli,pg]`\n\nRun it with command:\n\n```bash\nPG_URL=postgresql://postgres:123456@localhost:5432/postgres python3 -m easy_sql.data_process -f sample_etl.postgres.sql\n```\n\n### For clickhouse backend:\n\nYou need to start a clickhouse instance first.\n\nIf you have docker, run the command below:\n\n```bash\ndocker run -d --name clickhouse -p 9000:9000 yandex/clickhouse-server:20.12.5.18\n```\n\nCreate a file named `sample_etl.clickhouse.sql` with content as the test file [here](https://github.com/easysql/easy_sql/blob/main/test/sample_etl.clickhouse.sql).\n\nMake sure that you have install the corresponding backend with `python3 -m pip install easy-sql-easy-sql[cli,clickhouse]`\n\nRun it with command:\n\n```bash\nCLICKHOUSE_URL=clickhouse+native://default@localhost:9000 python3 -m easy_sql.data_process -f sample_etl.clickhouse.sql\n```\n\n### For flink backend:\n\nBecause of dependency conflictions between pyspark and apache-flink, you need to install flink manually with command `python3 -m pip install apache-flink`.\n\nAfter the installation, you need to add flink commands directory to PATH environment variable to make flink commands discoverable by bash. To do it, execute the commands below:\n\n```bash\nexport FLINK_HOME=$(python3 -m pyflink.find_flink_home)\nexport PATH=$FLINK_HOME/bin:$PATH\nexport PYFLINK_CLIENT_EXECUTABLE=python3  # Set Python interpreter for flink client.\n```\n\nYou can add these commands to your `.bashrc` or `.zshrc` file for convenience.\n\nSince there are many connectors for flink, you need to choose which connector to use before starting.\n\nAs an example, if you want to read or write data to postgres, then you need to start a postgres instance first.\n\nIf you have docker, run the command below:\n\n```bash\ndocker run -d --name postgres -p 5432:5432 -e POSTGRES_PASSWORD=123456 postgres\n```\n\nDownload the required jars as below:\n\n```bash\nmkdir -pv test/flink/jars\nwget -P test/flink/jars https://repo1.maven.org/maven2/org/apache/flink/flink-connector-jdbc/1.15.1/flink-connector-jdbc-1.15.1.jar\nwget -P test/flink/jars https://repo1.maven.org/maven2/org/postgresql/postgresql/42.2.14/postgresql-42.2.14.jar\n```\n\nCreate a file named `sample_etl.flink.postgres.sql` with content as the test file [here](https://github.com/easysql/easy_sql/blob/main/test/sample_etl.flink.postgres.sql).\n\nCreate a connector configuration file named `sample_etl.flink_tables_file.json` with content as the test configuration file [here](https://github.com/easysql/easy_sql/blob/main/test/sample_etl.flink_tables_file.json).\n\nRun it with command:\n\n```bash\nbash -c "$(python3 -m easy_sql.data_process -f sample_etl.flink.postgres.sql -p)"\n```\n\nThere are a few other things to know about flink, click [here](https://easy-sql.readthedocs.io/en/latest/easy_sql/backend/flink.html) to get more information.\n\n### For other backends:\n\nThe usage is similar, please refer to API doc [here](https://easy-sql.readthedocs.io/en/latest/autoapi/easy_sql/sql_processor/backend/index.html).\n\n## Run ETL in your code\n\nEasy SQL can be used as a very light-weight library. If you\'d like to run ETL programmatically in your code.\nPlease refer to the code snippets below:\n\n```python\nfrom pyspark.sql import SparkSession\n\nfrom easy_sql.sql_processor import SqlProcessor\nfrom easy_sql.sql_processor.backend import SparkBackend\n\nif __name__ == \'__main__\':\n    spark = SparkSession.builder.enableHiveSupport().getOrCreate()\n    backend = SparkBackend(spark)\n    sql = \'\'\'\n-- target=log.some_log\nselect 1 as a\n    \'\'\'\n    sql_processor = SqlProcessor(backend, sql)\n    sql_processor.run()\n```\n\nMore sample code about other backends could be referred [here](https://github.com/easysql/easy_sql/blob/main/test/sample_data_process.py)\n\n## Debugging ETL\n\nWe recommend debugging ETLs from jupyter. You can follow the steps below to start debugging your ETL.\n\n1. Install jupyter first with command `python3 -m pip install jupyterlab`.\n\n2. Create a file named `debugger.py` with contents like below:\n\nA more detailed sample could be found [here](https://github.com/easysql/easy_sql/blob/main/debugger.py).\n\n```python\nfrom typing import Dict, Any\n\ndef create_debugger(sql_file_path: str, vars: Dict[str, Any] = None, funcs: Dict[str, Any] = None):\n    from pyspark.sql import SparkSession\n    from easy_sql.sql_processor.backend import SparkBackend\n    from easy_sql.sql_processor_debugger import SqlProcessorDebugger\n    spark = SparkSession.builder.enableHiveSupport().getOrCreate()\n    backend = SparkBackend(spark)\n    debugger = SqlProcessorDebugger(sql_file_path, backend, vars, funcs)\n    return debugger\n\n```\n\n3. Create a file named `test.sql` with contents as [here](https://github.com/easysql/easy_sql/blob/main/test/sample_etl.spark.sql).\n\n4. Then start jupyter lab with command: `jupyter lab`.\n\n5. Start debugging like below:\n\n![ETL Debugging](https://raw.githubusercontent.com/easysql/easy_sql/main/debugger-usage.gif)\n\n## ETL Language support\n\nWe\'ve created an extension for VS Code to ease the development of ETL in Easy SQL. A bunch of language features are provided, e.g. syntax highlight, code completion, diagnostics features etc. You can search `Easy SQL` in extension marketplace, or click [here](https://marketplace.visualstudio.com/items?itemName=EasySQL.easysql&ssr=false#overview) to get more information.\n\nWe recommended to install the extension to develop ETL in Easy SQL.\n\n## Contributing\n\nPlease submit PR.\n',
-    'author': 'Easy SQL from Thoughtworks',
-    'author_email': 'easy_sql@thoughtworks.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://easy-sql.readthedocs.io',
-    'packages': packages,
-    'package_data': package_data,
-    'extras_require': extras_require,
-    'python_requires': '>=3.7,<4.0',
-}
+# Easy SQL
 
+Easy SQL is built to ease the data ETL development process.
+With Easy SQL, you can develop your ETL in SQL in an imperative way.
+It defines a few simple syntax on top of standard SQL, with which SQL could be executed one by one.
+Easy SQL also provides a processor to handle all the new syntax.
+Since this is SQL agnostic, any SQL engine could be plugged-in as a backend.
+There are built-in support for several popular SQL engines, including SparkSQL, PostgreSQL, Clickhouse, FlinkSQL, Aliyun Maxcompute, Google BigQuery.
+More will be added in the near future.
+
+- Docs: <https://easy-sql.readthedocs.io/>
+- Enterprise extended product: <https://data-workbench.com/>
+
+[![GitHub Action Build](https://github.com/easysql/easy_sql/actions/workflows/build.yaml/badge.svg?branch=main&event=push)](https://github.com/easysql/easy_sql/actions/workflows/build.yaml?query=branch%3Amain+event%3Apush)
+[![Docs Build](https://readthedocs.org/projects/easy-sql/badge/?version=latest)](https://easy-sql.readthedocs.io/en/latest/?badge=latest)
+[![EasySQL Coverage](https://codecov.io/gh/easysql/easy_sql/branch/main/graph/badge.svg)](https://codecov.io/gh/easysql/easy_sql)
+[![PyPI](https://img.shields.io/pypi/v/easy-sql-easy-sql)](https://pypi.org/project/easy-sql-easy-sql/)
+
+## Install Easy SQL
+
+Install Easy SQL using pip: `python3 -m pip install easy_sql-easy_sql[extra,extra]`
+
+Currently we are providing below extras, choose according to your need:
+- cli
+- linter
+- spark
+- pg
+- clickhouse
+
+We also provide flink backend, but because of dependency confliction between pyspark and apache-flink, you need to install the flink backend dependencies manually with the following command `python3 -m pip install apache-flink`.
+
+Usually we read data from some data source and write data to some other system using flink with different connectors. So we need to download some jars for the used connectors as well. Refer [here](https://nightlies.apache.org/flink/flink-docs-release-1.15/docs/connectors/table/overview/) to get more information and [here](https://nightlies.apache.org/flink/flink-docs-release-1.15/docs/connectors/table/downloads/) to download the required connectors.
+
+## Building Easy SQL
+
+Internally we use `poetry` to manage the dependencies. So make sure you have [installed it](https://python-poetry.org/docs/master/#installation). Package could be built with the following make command: `make package-pip` or just `poetry build`.
+
+After the above command, there will be a file named `easy_sql*.whl` generated in the `dist` folder.
+You can install it with command `python3 -m pip install dist/easy_sql*.whl[extra]` or just `poetry install -E 'extra extra'`.
+
+## First ETL with Easy SQL
+
+Install easy_sql with spark as the backend: `python3 -m pip install easy_sql-easy_sql[spark,cli]`.
+
+### For spark backend
+
+Create a file named `sample_etl.spark.sql` with content as below:
+
+```sql
+-- prepare-sql: drop database if exists sample cascade
+-- prepare-sql: create database sample
+-- prepare-sql: create table sample.test as select 1 as id, '1' as val
+
+-- target=variables
+select true as __create_output_table__
+
+-- target=variables
+select 1 as a
+
+-- target=log.a
+select '${a}' as a
+
+-- target=log.test_log
+select 1 as some_log
+
+-- target=check.should_equal
+select 1 as actual, 1 as expected
+
+-- target=temp.result
+select
+    ${a} as id, ${a} + 1 as val
+union all
+select id, val from sample.test
+
+-- target=output.sample.result
+select * from result
+
+-- target=log.sample_result
+select * from sample.result
+```
+
+Run it with command:
+
+```bash
+bash -c "$(python3 -m easy_sql.data_process -f sample_etl.spark.sql -p)"
+```
+
+### For postgres backend:
+
+You need to start a postgres instance first.
+
+If you have docker, run the command below:
+
+```bash
+docker run -d --name postgres -p 5432:5432 -e POSTGRES_PASSWORD=123456 postgres
+```
+
+Create a file named `sample_etl.postgres.sql` with content as the test file [here](https://github.com/easysql/easy_sql/blob/main/test/sample_etl.postgres.sql).
+
+Make sure that you have install the corresponding backend with `python3 -m pip install easy-sql-easy-sql[cli,pg]`
+
+Run it with command:
+
+```bash
+PG_URL=postgresql://postgres:123456@localhost:5432/postgres python3 -m easy_sql.data_process -f sample_etl.postgres.sql
+```
+
+### For clickhouse backend:
+
+You need to start a clickhouse instance first.
+
+If you have docker, run the command below:
+
+```bash
+docker run -d --name clickhouse -p 9000:9000 yandex/clickhouse-server:20.12.5.18
+```
+
+Create a file named `sample_etl.clickhouse.sql` with content as the test file [here](https://github.com/easysql/easy_sql/blob/main/test/sample_etl.clickhouse.sql).
+
+Make sure that you have install the corresponding backend with `python3 -m pip install easy-sql-easy-sql[cli,clickhouse]`
+
+Run it with command:
+
+```bash
+CLICKHOUSE_URL=clickhouse+native://default@localhost:9000 python3 -m easy_sql.data_process -f sample_etl.clickhouse.sql
+```
+
+### For flink backend:
+
+Because of dependency conflictions between pyspark and apache-flink, you need to install flink manually with command `python3 -m pip install apache-flink`.
+
+After the installation, you need to add flink commands directory to PATH environment variable to make flink commands discoverable by bash. To do it, execute the commands below:
+
+```bash
+export FLINK_HOME=$(python3 -m pyflink.find_flink_home)
+export PATH=$FLINK_HOME/bin:$PATH
+export PYFLINK_CLIENT_EXECUTABLE=python3  # Set Python interpreter for flink client.
+```
+
+You can add these commands to your `.bashrc` or `.zshrc` file for convenience.
+
+Since there are many connectors for flink, you need to choose which connector to use before starting.
+
+As an example, if you want to read or write data to postgres, then you need to start a postgres instance first.
+
+If you have docker, run the command below:
+
+```bash
+docker run -d --name postgres -p 5432:5432 -e POSTGRES_PASSWORD=123456 postgres
+```
+
+Download the required jars as below:
+
+```bash
+mkdir -pv test/flink/jars
+wget -P test/flink/jars https://repo1.maven.org/maven2/org/apache/flink/flink-connector-jdbc/1.15.1/flink-connector-jdbc-1.15.1.jar
+wget -P test/flink/jars https://repo1.maven.org/maven2/org/postgresql/postgresql/42.2.14/postgresql-42.2.14.jar
+```
+
+Create a file named `sample_etl.flink.postgres.sql` with content as the test file [here](https://github.com/easysql/easy_sql/blob/main/test/sample_etl.flink.postgres.sql).
+
+Create a connector configuration file named `sample_etl.flink_tables_file.json` with content as the test configuration file [here](https://github.com/easysql/easy_sql/blob/main/test/sample_etl.flink_tables_file.json).
+
+Run it with command:
+
+```bash
+bash -c "$(python3 -m easy_sql.data_process -f sample_etl.flink.postgres.sql -p)"
+```
+
+There are a few other things to know about flink, click [here](https://easy-sql.readthedocs.io/en/latest/easy_sql/backend/flink.html) to get more information.
+
+### For other backends:
+
+The usage is similar, please refer to API doc [here](https://easy-sql.readthedocs.io/en/latest/autoapi/easy_sql/sql_processor/backend/index.html).
+
+## Run ETL in your code
+
+Easy SQL can be used as a very light-weight library. If you'd like to run ETL programmatically in your code.
+Please refer to the code snippets below:
+
+```python
+from pyspark.sql import SparkSession
+
+from easy_sql.sql_processor import SqlProcessor
+from easy_sql.sql_processor.backend import SparkBackend
+
+if __name__ == '__main__':
+    spark = SparkSession.builder.enableHiveSupport().getOrCreate()
+    backend = SparkBackend(spark)
+    sql = '''
+-- target=log.some_log
+select 1 as a
+    '''
+    sql_processor = SqlProcessor(backend, sql)
+    sql_processor.run()
+```
+
+More sample code about other backends could be referred [here](https://github.com/easysql/easy_sql/blob/main/test/sample_data_process.py)
+
+## Debugging ETL
+
+We recommend debugging ETLs from jupyter. You can follow the steps below to start debugging your ETL.
+
+1. Install jupyter first with command `python3 -m pip install jupyterlab`.
+
+2. Create a file named `debugger.py` with contents like below:
+
+A more detailed sample could be found [here](https://github.com/easysql/easy_sql/blob/main/debugger.py).
+
+```python
+from typing import Dict, Any
+
+def create_debugger(sql_file_path: str, vars: Dict[str, Any] = None, funcs: Dict[str, Any] = None):
+    from pyspark.sql import SparkSession
+    from easy_sql.sql_processor.backend import SparkBackend
+    from easy_sql.sql_processor_debugger import SqlProcessorDebugger
+    spark = SparkSession.builder.enableHiveSupport().getOrCreate()
+    backend = SparkBackend(spark)
+    debugger = SqlProcessorDebugger(sql_file_path, backend, vars, funcs)
+    return debugger
+
+```
+
+3. Create a file named `test.sql` with contents as [here](https://github.com/easysql/easy_sql/blob/main/test/sample_etl.spark.sql).
+
+4. Then start jupyter lab with command: `jupyter lab`.
+
+5. Start debugging like below:
+
+![ETL Debugging](https://raw.githubusercontent.com/easysql/easy_sql/main/debugger-usage.gif)
+
+## ETL Language support
+
+We've created an extension for VS Code to ease the development of ETL in Easy SQL. A bunch of language features are provided, e.g. syntax highlight, code completion, diagnostics features etc. You can search `Easy SQL` in extension marketplace, or click [here](https://marketplace.visualstudio.com/items?itemName=EasySQL.easysql&ssr=false#overview) to get more information.
+
+We recommended to install the extension to develop ETL in Easy SQL.
+
+## Contributing
+
+Please submit PR.
 
-setup(**setup_kwargs)
```

