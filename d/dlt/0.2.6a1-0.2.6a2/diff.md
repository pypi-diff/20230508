# Comparing `tmp/dlt-0.2.6a1.tar.gz` & `tmp/dlt-0.2.6a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dlt-0.2.6a1.tar", max compression
+gzip compressed data, was "dlt-0.2.6a2.tar", max compression
```

## Comparing `dlt-0.2.6a1.tar` & `dlt-0.2.6a2.tar`

### file list

```diff
@@ -1,207 +1,209 @@
--rw-r--r--   0        0        0    11343 2022-06-03 15:05:59.024600 dlt-0.2.6a1/LICENSE.txt
--rw-r--r--   0        0        0     4214 2023-04-30 21:17:44.388805 dlt-0.2.6a1/README.md
--rw-r--r--   0        0        0     1711 2023-04-30 21:17:44.388805 dlt-0.2.6a1/dlt/__init__.py
--rw-r--r--   0        0        0        0 2023-04-30 21:17:44.388805 dlt-0.2.6a1/dlt/cli/__init__.py
--rw-r--r--   0        0        0    15501 2023-04-30 21:17:44.388805 dlt-0.2.6a1/dlt/cli/_dlt.py
--rw-r--r--   0        0        0     3808 2023-04-30 21:17:44.388805 dlt-0.2.6a1/dlt/cli/config_toml_writer.py
--rw-r--r--   0        0        0    16663 2023-04-22 20:26:30.632198 dlt-0.2.6a1/dlt/cli/deploy_command.py
--rw-r--r--   0        0        0     1853 2023-04-30 21:17:44.388805 dlt-0.2.6a1/dlt/cli/echo.py
--rw-r--r--   0        0        0      435 2023-03-23 14:48:32.551618 dlt-0.2.6a1/dlt/cli/exceptions.py
--rw-r--r--   0        0        0    18888 2023-04-22 20:26:30.632198 dlt-0.2.6a1/dlt/cli/init_command.py
--rw-r--r--   0        0        0    10489 2023-04-30 21:17:44.388805 dlt-0.2.6a1/dlt/cli/pipeline_command.py
--rw-r--r--   0        0        0     9419 2023-04-03 18:50:36.893525 dlt-0.2.6a1/dlt/cli/pipeline_files.py
--rw-r--r--   0        0        0     4404 2023-03-23 14:48:32.551618 dlt-0.2.6a1/dlt/cli/source_detection.py
--rw-r--r--   0        0        0     1899 2023-04-22 20:26:30.632198 dlt-0.2.6a1/dlt/cli/telemetry_command.py
--rw-r--r--   0        0        0     3757 2023-04-30 21:17:44.388805 dlt-0.2.6a1/dlt/cli/utils.py
--rw-r--r--   0        0        0      307 2023-03-23 14:48:32.551618 dlt-0.2.6a1/dlt/common/__init__.py
--rw-r--r--   0        0        0     1265 2022-08-24 09:42:09.472789 dlt-0.2.6a1/dlt/common/arithmetics.py
--rw-r--r--   0        0        0      428 2023-03-23 14:48:32.551618 dlt-0.2.6a1/dlt/common/configuration/__init__.py
--rw-r--r--   0        0        0     4898 2023-03-23 14:48:32.551618 dlt-0.2.6a1/dlt/common/configuration/accessors.py
--rw-r--r--   0        0        0     3448 2023-04-05 15:15:49.779453 dlt-0.2.6a1/dlt/common/configuration/container.py
--rw-r--r--   0        0        0     5884 2023-04-22 20:26:30.632198 dlt-0.2.6a1/dlt/common/configuration/exceptions.py
--rw-r--r--   0        0        0     7912 2023-04-22 20:26:30.632198 dlt-0.2.6a1/dlt/common/configuration/inject.py
--rw-r--r--   0        0        0     1198 2023-03-23 14:48:32.551618 dlt-0.2.6a1/dlt/common/configuration/paths.py
--rw-r--r--   0        0        0      252 2023-03-23 14:48:32.551618 dlt-0.2.6a1/dlt/common/configuration/providers/__init__.py
--rw-r--r--   0        0        0     1108 2023-04-26 11:34:23.292768 dlt-0.2.6a1/dlt/common/configuration/providers/airflow.py
--rw-r--r--   0        0        0     1089 2023-03-23 14:48:32.551618 dlt-0.2.6a1/dlt/common/configuration/providers/context.py
--rw-r--r--   0        0        0     1193 2023-03-23 14:48:32.551618 dlt-0.2.6a1/dlt/common/configuration/providers/dictionary.py
--rw-r--r--   0        0        0     2050 2023-03-23 14:48:32.551618 dlt-0.2.6a1/dlt/common/configuration/providers/environ.py
--rw-r--r--   0        0        0      758 2023-03-23 14:48:32.551618 dlt-0.2.6a1/dlt/common/configuration/providers/provider.py
--rw-r--r--   0        0        0     5320 2023-04-24 18:26:21.111453 dlt-0.2.6a1/dlt/common/configuration/providers/toml.py
--rw-r--r--   0        0        0    18054 2023-04-30 21:17:44.388805 dlt-0.2.6a1/dlt/common/configuration/resolve.py
--rw-r--r--   0        0        0      868 2023-04-24 18:26:21.111453 dlt-0.2.6a1/dlt/common/configuration/specs/__init__.py
--rw-r--r--   0        0        0     1679 2023-04-24 18:26:21.111453 dlt-0.2.6a1/dlt/common/configuration/specs/api_credentials.py
--rw-r--r--   0        0        0    10914 2023-04-09 16:39:04.593180 dlt-0.2.6a1/dlt/common/configuration/specs/base_configuration.py
--rw-r--r--   0        0        0     3295 2023-04-30 21:17:44.388805 dlt-0.2.6a1/dlt/common/configuration/specs/config_providers_context.py
--rw-r--r--   0        0        0     2792 2023-03-23 14:48:32.551618 dlt-0.2.6a1/dlt/common/configuration/specs/config_section_context.py
--rw-r--r--   0        0        0     2125 2023-04-24 18:26:21.111453 dlt-0.2.6a1/dlt/common/configuration/specs/exceptions.py
--rw-r--r--   0        0        0    12193 2023-04-30 21:17:44.388805 dlt-0.2.6a1/dlt/common/configuration/specs/gcp_client_credentials.py
--rw-r--r--   0        0        0      665 2023-03-23 14:48:32.551618 dlt-0.2.6a1/dlt/common/configuration/specs/known_sections.py
--rw-r--r--   0        0        0      556 2023-03-23 14:48:32.551618 dlt-0.2.6a1/dlt/common/configuration/specs/load_volume_configuration.py
--rw-r--r--   0        0        0      417 2023-03-23 14:48:32.551618 dlt-0.2.6a1/dlt/common/configuration/specs/normalize_volume_configuration.py
--rw-r--r--   0        0        0     2843 2023-04-30 21:17:44.388805 dlt-0.2.6a1/dlt/common/configuration/specs/postgres_credentials.py
--rw-r--r--   0        0        0     2455 2023-04-30 21:17:44.388805 dlt-0.2.6a1/dlt/common/configuration/specs/run_configuration.py
--rw-r--r--   0        0        0      944 2023-03-23 14:48:32.551618 dlt-0.2.6a1/dlt/common/configuration/specs/schema_volume_configuration.py
--rw-r--r--   0        0        0     5339 2023-04-03 18:50:36.893525 dlt-0.2.6a1/dlt/common/configuration/utils.py
--rw-r--r--   0        0        0      142 2023-03-23 14:48:32.551618 dlt-0.2.6a1/dlt/common/data_types/__init__.py
--rw-r--r--   0        0        0     6306 2023-03-23 14:48:32.551618 dlt-0.2.6a1/dlt/common/data_types/type_helpers.py
--rw-r--r--   0        0        0      214 2023-03-23 14:48:32.551618 dlt-0.2.6a1/dlt/common/data_types/typing.py
--rw-r--r--   0        0        0      260 2023-03-23 14:48:20.701618 dlt-0.2.6a1/dlt/common/data_writers/__init__.py
--rw-r--r--   0        0        0     5893 2023-03-23 14:48:32.551618 dlt-0.2.6a1/dlt/common/data_writers/buffered.py
--rw-r--r--   0        0        0     2395 2023-03-23 14:48:32.551618 dlt-0.2.6a1/dlt/common/data_writers/escape.py
--rw-r--r--   0        0        0      962 2023-03-23 14:48:32.551618 dlt-0.2.6a1/dlt/common/data_writers/exceptions.py
--rw-r--r--   0        0        0     5159 2023-03-23 14:48:32.551618 dlt-0.2.6a1/dlt/common/data_writers/writers.py
--rw-r--r--   0        0        0       97 2023-03-23 14:48:32.551618 dlt-0.2.6a1/dlt/common/destination/__init__.py
--rw-r--r--   0        0        0     2206 2023-04-05 08:03:40.638919 dlt-0.2.6a1/dlt/common/destination/capabilities.py
--rw-r--r--   0        0        0    10682 2023-04-24 11:35:34.867759 dlt-0.2.6a1/dlt/common/destination/reference.py
--rw-r--r--   0        0        0     6121 2023-04-30 21:17:44.388805 dlt-0.2.6a1/dlt/common/exceptions.py
--rw-r--r--   0        0        0     4954 2023-03-23 14:48:32.551618 dlt-0.2.6a1/dlt/common/git.py
--rw-r--r--   0        0        0     5248 2023-04-10 08:12:53.759595 dlt-0.2.6a1/dlt/common/json/__init__.py
--rw-r--r--   0        0        0     1802 2023-04-10 08:12:53.769595 dlt-0.2.6a1/dlt/common/json/_orjson.py
--rw-r--r--   0        0        0     2939 2023-04-10 08:12:53.769595 dlt-0.2.6a1/dlt/common/json/_simplejson.py
--rw-r--r--   0        0        0     1536 2023-04-29 12:58:55.943219 dlt-0.2.6a1/dlt/common/jsonpath.py
--rw-r--r--   0        0        0      232 2023-03-23 14:48:32.551618 dlt-0.2.6a1/dlt/common/normalizers/__init__.py
--rw-r--r--   0        0        0     1210 2023-04-05 08:03:40.638919 dlt-0.2.6a1/dlt/common/normalizers/configuration.py
--rw-r--r--   0        0        0      472 2023-03-23 14:48:32.551618 dlt-0.2.6a1/dlt/common/normalizers/exceptions.py
--rw-r--r--   0        0        0     1644 2023-04-06 15:27:24.759561 dlt-0.2.6a1/dlt/common/normalizers/json/__init__.py
--rw-r--r--   0        0        0    13396 2023-04-06 15:27:24.759561 dlt-0.2.6a1/dlt/common/normalizers/json/relational.py
--rw-r--r--   0        0        0       64 2023-03-23 14:48:32.551618 dlt-0.2.6a1/dlt/common/normalizers/naming/__init__.py
--rw-r--r--   0        0        0      807 2023-03-23 14:48:32.551618 dlt-0.2.6a1/dlt/common/normalizers/naming/direct.py
--rw-r--r--   0        0        0     1069 2023-03-23 14:48:32.551618 dlt-0.2.6a1/dlt/common/normalizers/naming/duck_case.py
--rw-r--r--   0        0        0      792 2023-03-23 14:48:32.551618 dlt-0.2.6a1/dlt/common/normalizers/naming/exceptions.py
--rw-r--r--   0        0        0     3753 2023-04-05 08:03:40.638919 dlt-0.2.6a1/dlt/common/normalizers/naming/naming.py
--rw-r--r--   0        0        0     3002 2023-03-23 14:48:32.551618 dlt-0.2.6a1/dlt/common/normalizers/naming/snake_case.py
--rw-r--r--   0        0        0      358 2023-04-02 09:09:15.855769 dlt-0.2.6a1/dlt/common/normalizers/typing.py
--rw-r--r--   0        0        0     2337 2023-04-06 15:27:24.759561 dlt-0.2.6a1/dlt/common/normalizers/utils.py
--rw-r--r--   0        0        0      451 2023-03-23 14:48:32.551618 dlt-0.2.6a1/dlt/common/pendulum.py
--rw-r--r--   0        0        0    16937 2023-04-30 21:17:44.388805 dlt-0.2.6a1/dlt/common/pipeline.py
--rw-r--r--   0        0        0        0 2023-03-23 14:48:32.551618 dlt-0.2.6a1/dlt/common/reflection/__init__.py
--rw-r--r--   0        0        0      374 2023-03-23 14:48:32.551618 dlt-0.2.6a1/dlt/common/reflection/function_visitor.py
--rw-r--r--   0        0        0     4891 2023-04-09 16:39:04.593180 dlt-0.2.6a1/dlt/common/reflection/spec.py
--rw-r--r--   0        0        0     5069 2023-04-24 18:26:21.111453 dlt-0.2.6a1/dlt/common/reflection/utils.py
--rw-r--r--   0        0        0      174 2023-04-30 21:17:44.388805 dlt-0.2.6a1/dlt/common/runners/__init__.py
--rw-r--r--   0        0        0      508 2023-04-30 21:17:44.388805 dlt-0.2.6a1/dlt/common/runners/configuration.py
--rw-r--r--   0        0        0     2635 2023-04-30 21:17:44.388805 dlt-0.2.6a1/dlt/common/runners/pool_runner.py
--rw-r--r--   0        0        0     4046 2023-03-23 14:48:32.561618 dlt-0.2.6a1/dlt/common/runners/runnable.py
--rw-r--r--   0        0        0     3145 2023-03-23 14:48:32.561618 dlt-0.2.6a1/dlt/common/runners/stdout.py
--rw-r--r--   0        0        0     2137 2023-03-23 14:48:32.561618 dlt-0.2.6a1/dlt/common/runners/synth_pickle.py
--rw-r--r--   0        0        0      105 2023-04-30 21:17:44.388805 dlt-0.2.6a1/dlt/common/runners/typing.py
--rw-r--r--   0        0        0     5250 2023-03-23 14:48:32.561618 dlt-0.2.6a1/dlt/common/runners/venv.py
--rw-r--r--   0        0        0       36 2023-04-30 21:17:44.398805 dlt-0.2.6a1/dlt/common/runtime/__init__.py
--rw-r--r--   0        0        0    13441 2023-04-30 21:17:44.398805 dlt-0.2.6a1/dlt/common/runtime/collector.py
--rw-r--r--   0        0        0     4264 2023-04-30 21:17:44.398805 dlt-0.2.6a1/dlt/common/runtime/exec_info.py
--rw-r--r--   0        0        0      647 2023-04-30 21:17:44.398805 dlt-0.2.6a1/dlt/common/runtime/init.py
--rw-r--r--   0        0        0     4002 2023-04-30 21:17:44.398805 dlt-0.2.6a1/dlt/common/runtime/logger.py
--rw-r--r--   0        0        0     2052 2023-04-30 21:17:44.398805 dlt-0.2.6a1/dlt/common/runtime/prometheus.py
--rw-r--r--   0        0        0     7170 2023-04-22 20:26:30.632198 dlt-0.2.6a1/dlt/common/runtime/segment.py
--rw-r--r--   0        0        0     2493 2023-04-30 21:17:44.398805 dlt-0.2.6a1/dlt/common/runtime/sentry.py
--rw-r--r--   0        0        0     2027 2023-04-30 21:17:44.398805 dlt-0.2.6a1/dlt/common/runtime/signals.py
--rw-r--r--   0        0        0      616 2023-04-03 18:50:36.893525 dlt-0.2.6a1/dlt/common/runtime/slack.py
--rw-r--r--   0        0        0      720 2023-04-30 21:17:44.398805 dlt-0.2.6a1/dlt/common/runtime/telemetry.py
--rw-r--r--   0        0        0      387 2023-04-03 18:50:36.893525 dlt-0.2.6a1/dlt/common/schema/__init__.py
--rw-r--r--   0        0        0     1927 2023-03-23 14:48:32.561618 dlt-0.2.6a1/dlt/common/schema/detections.py
--rw-r--r--   0        0        0     2974 2023-03-23 14:48:32.561618 dlt-0.2.6a1/dlt/common/schema/exceptions.py
--rw-r--r--   0        0        0    25175 2023-04-09 16:39:04.593180 dlt-0.2.6a1/dlt/common/schema/schema.py
--rw-r--r--   0        0        0     3004 2023-04-22 20:26:30.632198 dlt-0.2.6a1/dlt/common/schema/typing.py
--rw-r--r--   0        0        0    23087 2023-04-30 21:17:44.398805 dlt-0.2.6a1/dlt/common/schema/utils.py
--rw-r--r--   0        0        0      410 2023-03-23 14:48:32.561618 dlt-0.2.6a1/dlt/common/storages/__init__.py
--rw-r--r--   0        0        0     1906 2023-03-23 14:48:32.561618 dlt-0.2.6a1/dlt/common/storages/data_item_storage.py
--rw-r--r--   0        0        0     2804 2023-04-03 18:50:36.893525 dlt-0.2.6a1/dlt/common/storages/exceptions.py
--rw-r--r--   0        0        0     9059 2023-04-05 08:03:40.638919 dlt-0.2.6a1/dlt/common/storages/file_storage.py
--rw-r--r--   0        0        0     2685 2023-04-13 08:33:43.967587 dlt-0.2.6a1/dlt/common/storages/live_schema_storage.py
--rw-r--r--   0        0        0    21810 2023-04-29 12:58:55.953219 dlt-0.2.6a1/dlt/common/storages/load_storage.py
--rw-r--r--   0        0        0     2414 2023-03-23 14:48:32.561618 dlt-0.2.6a1/dlt/common/storages/normalize_storage.py
--rw-r--r--   0        0        0     8508 2023-03-23 14:48:32.561618 dlt-0.2.6a1/dlt/common/storages/schema_storage.py
--rw-r--r--   0        0        0     2525 2023-04-24 18:26:21.111453 dlt-0.2.6a1/dlt/common/storages/versioned_storage.py
--rw-r--r--   0        0        0     2677 2023-03-23 14:48:32.561618 dlt-0.2.6a1/dlt/common/time.py
--rw-r--r--   0        0        0     4736 2023-04-03 18:50:36.893525 dlt-0.2.6a1/dlt/common/typing.py
--rw-r--r--   0        0        0    11275 2023-04-24 18:26:21.111453 dlt-0.2.6a1/dlt/common/utils.py
--rw-r--r--   0        0        0     3686 2023-03-23 14:48:32.561618 dlt-0.2.6a1/dlt/common/validation.py
--rw-r--r--   0        0        0     1185 2023-03-23 14:48:32.561618 dlt-0.2.6a1/dlt/common/wei.py
--rw-r--r--   0        0        0        0 2023-03-23 14:48:32.561618 dlt-0.2.6a1/dlt/destinations/__init__.py
--rw-r--r--   0        0        0      437 2023-03-23 14:48:32.561618 dlt-0.2.6a1/dlt/destinations/bigquery/README.md
--rw-r--r--   0        0        0     1813 2023-04-05 08:03:40.638919 dlt-0.2.6a1/dlt/destinations/bigquery/__init__.py
--rw-r--r--   0        0        0    12301 2023-04-06 15:27:24.759561 dlt-0.2.6a1/dlt/destinations/bigquery/bigquery.py
--rw-r--r--   0        0        0      392 2023-03-23 14:48:32.561618 dlt-0.2.6a1/dlt/destinations/bigquery/configuration.py
--rw-r--r--   0        0        0    10123 2023-04-24 18:26:21.111453 dlt-0.2.6a1/dlt/destinations/bigquery/sql_client.py
--rw-r--r--   0        0        0     1935 2023-04-05 08:03:40.638919 dlt-0.2.6a1/dlt/destinations/duckdb/__init__.py
--rw-r--r--   0        0        0     7025 2023-04-30 21:17:44.398805 dlt-0.2.6a1/dlt/destinations/duckdb/configuration.py
--rw-r--r--   0        0        0     2754 2023-03-23 14:48:32.561618 dlt-0.2.6a1/dlt/destinations/duckdb/duck.py
--rw-r--r--   0        0        0     6936 2023-04-21 22:25:54.789942 dlt-0.2.6a1/dlt/destinations/duckdb/sql_client.py
--rw-r--r--   0        0        0     1671 2023-03-23 14:48:32.561618 dlt-0.2.6a1/dlt/destinations/dummy/__init__.py
--rw-r--r--   0        0        0      736 2023-04-03 18:50:36.893525 dlt-0.2.6a1/dlt/destinations/dummy/configuration.py
--rw-r--r--   0        0        0     4975 2023-04-24 11:35:34.867759 dlt-0.2.6a1/dlt/destinations/dummy/dummy.py
--rw-r--r--   0        0        0     4159 2023-04-05 08:03:40.638919 dlt-0.2.6a1/dlt/destinations/exceptions.py
--rw-r--r--   0        0        0     4983 2023-04-05 08:03:40.638919 dlt-0.2.6a1/dlt/destinations/insert_job_client.py
--rw-r--r--   0        0        0    15181 2023-04-29 12:58:55.953219 dlt-0.2.6a1/dlt/destinations/job_client_impl.py
--rw-r--r--   0        0        0     1303 2023-04-05 08:03:40.638919 dlt-0.2.6a1/dlt/destinations/job_impl.py
--rw-r--r--   0        0        0      251 2023-03-23 14:48:32.561618 dlt-0.2.6a1/dlt/destinations/postgres/README.md
--rw-r--r--   0        0        0     1934 2023-04-05 08:03:40.638919 dlt-0.2.6a1/dlt/destinations/postgres/__init__.py
--rw-r--r--   0        0        0      443 2023-03-23 14:48:32.561618 dlt-0.2.6a1/dlt/destinations/postgres/configuration.py
--rw-r--r--   0        0        0     3025 2023-03-23 14:48:32.561618 dlt-0.2.6a1/dlt/destinations/postgres/postgres.py
--rw-r--r--   0        0        0     6066 2023-04-13 08:33:43.967587 dlt-0.2.6a1/dlt/destinations/postgres/sql_client.py
--rw-r--r--   0        0        0     1159 2023-04-03 18:50:36.893525 dlt-0.2.6a1/dlt/destinations/redshift/README.md
--rw-r--r--   0        0        0     1905 2023-04-05 08:03:40.638919 dlt-0.2.6a1/dlt/destinations/redshift/__init__.py
--rw-r--r--   0        0        0      405 2023-03-23 14:48:32.561618 dlt-0.2.6a1/dlt/destinations/redshift/configuration.py
--rw-r--r--   0        0        0     3761 2023-03-23 14:48:32.561618 dlt-0.2.6a1/dlt/destinations/redshift/redshift.py
--rw-r--r--   0        0        0     7110 2023-04-29 12:58:55.953219 dlt-0.2.6a1/dlt/destinations/sql_client.py
--rw-r--r--   0        0        0    10101 2023-04-09 16:39:04.593180 dlt-0.2.6a1/dlt/destinations/sql_merge_job.py
--rw-r--r--   0        0        0     1931 2023-04-24 18:26:21.111453 dlt-0.2.6a1/dlt/destinations/typing.py
--rw-r--r--   0        0        0        0 2022-08-09 19:58:51.837922 dlt-0.2.6a1/dlt/extract/__init__.py
--rw-r--r--   0        0        0    22569 2023-04-22 20:26:30.632198 dlt-0.2.6a1/dlt/extract/decorators.py
--rw-r--r--   0        0        0    12645 2023-04-30 21:17:44.398805 dlt-0.2.6a1/dlt/extract/exceptions.py
--rw-r--r--   0        0        0     8449 2023-04-30 21:17:44.398805 dlt-0.2.6a1/dlt/extract/extract.py
--rw-r--r--   0        0        0    14650 2023-04-30 21:17:44.398805 dlt-0.2.6a1/dlt/extract/incremental.py
--rw-r--r--   0        0        0    31567 2023-04-30 21:17:44.398805 dlt-0.2.6a1/dlt/extract/pipe.py
--rw-r--r--   0        0        0     9683 2023-04-22 20:26:30.632198 dlt-0.2.6a1/dlt/extract/schema.py
--rw-r--r--   0        0        0    33994 2023-04-30 21:17:44.398805 dlt-0.2.6a1/dlt/extract/source.py
--rw-r--r--   0        0        0     4350 2023-04-22 20:26:30.632198 dlt-0.2.6a1/dlt/extract/typing.py
--rw-r--r--   0        0        0      593 2023-04-06 20:38:35.239561 dlt-0.2.6a1/dlt/extract/utils.py
--rw-r--r--   0        0        0        0 2022-08-14 16:06:42.572263 dlt-0.2.6a1/dlt/helpers/__init__.py
--rw-r--r--   0        0        0        0 2023-04-30 21:17:44.398805 dlt-0.2.6a1/dlt/helpers/airflow/__init__.py
--rw-r--r--   0        0        0     2907 2023-03-23 14:48:32.561618 dlt-0.2.6a1/dlt/helpers/dbt/__init__.py
--rw-r--r--   0        0        0     1220 2023-03-23 14:48:32.561618 dlt-0.2.6a1/dlt/helpers/dbt/configuration.py
--rw-r--r--   0        0        0     6137 2023-03-23 14:48:32.561618 dlt-0.2.6a1/dlt/helpers/dbt/dbt_utils.py
--rw-r--r--   0        0        0      758 2023-03-23 14:48:32.561618 dlt-0.2.6a1/dlt/helpers/dbt/exceptions.py
--rw-r--r--   0        0        0     3583 2023-03-23 14:48:32.561618 dlt-0.2.6a1/dlt/helpers/dbt/profiles.yml
--rw-r--r--   0        0        0    13032 2023-04-30 21:17:44.398805 dlt-0.2.6a1/dlt/helpers/dbt/runner.py
--rw-r--r--   0        0        0     2373 2023-03-23 14:48:32.571618 dlt-0.2.6a1/dlt/helpers/pandas.py
--rw-r--r--   0        0        0     1035 2023-03-23 14:48:32.571618 dlt-0.2.6a1/dlt/helpers/parquet.py
--rw-r--r--   0        0        0    13371 2023-04-30 21:17:44.398805 dlt-0.2.6a1/dlt/helpers/streamlit.py
--rw-r--r--   0        0        0       31 2023-03-23 14:48:32.571618 dlt-0.2.6a1/dlt/load/__init__.py
--rw-r--r--   0        0        0     1019 2023-04-30 21:17:44.398805 dlt-0.2.6a1/dlt/load/configuration.py
--rw-r--r--   0        0        0     1993 2023-04-05 08:03:40.638919 dlt-0.2.6a1/dlt/load/exceptions.py
--rw-r--r--   0        0        0    19928 2023-04-30 21:17:44.398805 dlt-0.2.6a1/dlt/load/load.py
--rw-r--r--   0        0        0       32 2023-03-23 14:48:32.571618 dlt-0.2.6a1/dlt/normalize/__init__.py
--rw-r--r--   0        0        0     1098 2023-04-30 21:17:44.398805 dlt-0.2.6a1/dlt/normalize/configuration.py
--rw-r--r--   0        0        0        0 2022-08-09 19:58:51.837922 dlt-0.2.6a1/dlt/normalize/exceptions.py
--rw-r--r--   0        0        0    16576 2023-04-30 21:17:44.398805 dlt-0.2.6a1/dlt/normalize/normalize.py
--rw-r--r--   0        0        0     1880 2023-03-23 14:48:32.571618 dlt-0.2.6a1/dlt/pipeline/README.md
--rw-r--r--   0        0        0    13138 2023-04-30 21:17:44.398805 dlt-0.2.6a1/dlt/pipeline/__init__.py
--rw-r--r--   0        0        0     1858 2023-04-30 21:17:44.398805 dlt-0.2.6a1/dlt/pipeline/configuration.py
--rw-r--r--   0        0        0      363 2023-04-22 20:26:30.632198 dlt-0.2.6a1/dlt/pipeline/current.py
--rw-r--r--   0        0        0     4829 2023-03-23 14:48:32.571618 dlt-0.2.6a1/dlt/pipeline/dbt.py
--rw-r--r--   0        0        0     2891 2023-04-30 21:17:44.398805 dlt-0.2.6a1/dlt/pipeline/exceptions.py
--rw-r--r--   0        0        0     8447 2023-04-30 21:17:44.398805 dlt-0.2.6a1/dlt/pipeline/helpers.py
--rw-r--r--   0        0        0      122 2023-04-06 15:27:24.759561 dlt-0.2.6a1/dlt/pipeline/mark.py
--rw-r--r--   0        0        0    56164 2023-04-30 21:17:44.398805 dlt-0.2.6a1/dlt/pipeline/pipeline.py
--rw-r--r--   0        0        0      985 2023-04-30 21:17:44.398805 dlt-0.2.6a1/dlt/pipeline/progress.py
--rw-r--r--   0        0        0     4200 2023-04-10 08:12:53.769595 dlt-0.2.6a1/dlt/pipeline/state_sync.py
--rw-r--r--   0        0        0     7990 2023-04-03 18:50:36.903525 dlt-0.2.6a1/dlt/pipeline/trace.py
--rw-r--r--   0        0        0     4563 2023-04-03 18:50:36.903525 dlt-0.2.6a1/dlt/pipeline/track.py
--rw-r--r--   0        0        0       91 2023-03-23 14:48:32.571618 dlt-0.2.6a1/dlt/pipeline/typing.py
--rw-r--r--   0        0        0        0 2022-06-03 13:18:25.174600 dlt-0.2.6a1/dlt/py.typed
--rw-r--r--   0        0        0        0 2023-03-23 14:48:32.571618 dlt-0.2.6a1/dlt/reflection/__init__.py
--rw-r--r--   0        0        0      563 2023-03-23 14:48:32.571618 dlt-0.2.6a1/dlt/reflection/names.py
--rw-r--r--   0        0        0     4986 2023-04-22 20:26:30.632198 dlt-0.2.6a1/dlt/reflection/script_inspector.py
--rw-r--r--   0        0        0     6186 2023-03-23 14:48:32.571618 dlt-0.2.6a1/dlt/reflection/script_visitor.py
--rw-r--r--   0        0        0      118 2023-04-06 15:27:24.759561 dlt-0.2.6a1/dlt/sources/__init__.py
--rw-r--r--   0        0        0        0 2023-03-23 14:48:32.571618 dlt-0.2.6a1/dlt/sources/helpers/__init__.py
--rw-r--r--   0        0        0      574 2023-03-23 14:48:37.261618 dlt-0.2.6a1/dlt/sources/helpers/requests/__init__.py
--rw-r--r--   0        0        0     9092 2023-04-24 18:26:21.111453 dlt-0.2.6a1/dlt/sources/helpers/requests/retry.py
--rw-r--r--   0        0        0     1336 2023-03-23 14:48:32.571618 dlt-0.2.6a1/dlt/sources/helpers/requests/session.py
--rw-r--r--   0        0        0      679 2023-04-06 15:27:24.759561 dlt-0.2.6a1/dlt/sources/helpers/transform.py
--rw-r--r--   0        0        0     1125 2023-04-22 20:26:30.632198 dlt-0.2.6a1/dlt/version.py
--rw-r--r--   0        0        0     3928 2023-04-30 21:17:44.408805 dlt-0.2.6a1/pyproject.toml
--rw-r--r--   0        0        0     7395 1970-01-01 00:00:00.000000 dlt-0.2.6a1/setup.py
--rw-r--r--   0        0        0     7323 1970-01-01 00:00:00.000000 dlt-0.2.6a1/PKG-INFO
+-rw-r--r--   0        0        0    11343 2022-06-03 15:05:59.024600 dlt-0.2.6a2/LICENSE.txt
+-rw-r--r--   0        0        0     4214 2023-04-30 21:17:44.388805 dlt-0.2.6a2/README.md
+-rw-r--r--   0        0        0     1711 2023-04-30 21:17:44.388805 dlt-0.2.6a2/dlt/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-30 21:17:44.388805 dlt-0.2.6a2/dlt/cli/__init__.py
+-rw-r--r--   0        0        0    15909 2023-05-05 10:04:39.176579 dlt-0.2.6a2/dlt/cli/_dlt.py
+-rw-r--r--   0        0        0     3858 2023-05-07 18:29:53.319469 dlt-0.2.6a2/dlt/cli/config_toml_writer.py
+-rw-r--r--   0        0        0    16663 2023-04-22 20:26:30.632198 dlt-0.2.6a2/dlt/cli/deploy_command.py
+-rw-r--r--   0        0        0     1853 2023-04-30 21:17:44.388805 dlt-0.2.6a2/dlt/cli/echo.py
+-rw-r--r--   0        0        0      435 2023-03-23 14:48:32.551618 dlt-0.2.6a2/dlt/cli/exceptions.py
+-rw-r--r--   0        0        0    18888 2023-04-22 20:26:30.632198 dlt-0.2.6a2/dlt/cli/init_command.py
+-rw-r--r--   0        0        0    10489 2023-04-30 21:17:44.388805 dlt-0.2.6a2/dlt/cli/pipeline_command.py
+-rw-r--r--   0        0        0     9419 2023-04-03 18:50:36.893525 dlt-0.2.6a2/dlt/cli/pipeline_files.py
+-rw-r--r--   0        0        0     4510 2023-05-04 15:57:31.375706 dlt-0.2.6a2/dlt/cli/source_detection.py
+-rw-r--r--   0        0        0     1899 2023-04-22 20:26:30.632198 dlt-0.2.6a2/dlt/cli/telemetry_command.py
+-rw-r--r--   0        0        0     3757 2023-04-30 21:17:44.388805 dlt-0.2.6a2/dlt/cli/utils.py
+-rw-r--r--   0        0        0      307 2023-03-23 14:48:32.551618 dlt-0.2.6a2/dlt/common/__init__.py
+-rw-r--r--   0        0        0     1265 2022-08-24 09:42:09.472789 dlt-0.2.6a2/dlt/common/arithmetics.py
+-rw-r--r--   0        0        0      428 2023-03-23 14:48:32.551618 dlt-0.2.6a2/dlt/common/configuration/__init__.py
+-rw-r--r--   0        0        0     4184 2023-05-07 13:09:43.709469 dlt-0.2.6a2/dlt/common/configuration/accessors.py
+-rw-r--r--   0        0        0     3469 2023-05-07 15:40:06.149469 dlt-0.2.6a2/dlt/common/configuration/container.py
+-rw-r--r--   0        0        0     5884 2023-04-22 20:26:30.632198 dlt-0.2.6a2/dlt/common/configuration/exceptions.py
+-rw-r--r--   0        0        0     7912 2023-04-22 20:26:30.632198 dlt-0.2.6a2/dlt/common/configuration/inject.py
+-rw-r--r--   0        0        0     1198 2023-03-23 14:48:32.551618 dlt-0.2.6a2/dlt/common/configuration/paths.py
+-rw-r--r--   0        0        0      306 2023-05-06 21:48:15.113451 dlt-0.2.6a2/dlt/common/configuration/providers/__init__.py
+-rw-r--r--   0        0        0     1108 2023-04-26 11:34:23.292768 dlt-0.2.6a2/dlt/common/configuration/providers/airflow.py
+-rw-r--r--   0        0        0     1116 2023-05-07 12:57:30.109469 dlt-0.2.6a2/dlt/common/configuration/providers/context.py
+-rw-r--r--   0        0        0     1335 2023-05-07 15:00:38.059469 dlt-0.2.6a2/dlt/common/configuration/providers/dictionary.py
+-rw-r--r--   0        0        0     1981 2023-05-07 13:01:36.889469 dlt-0.2.6a2/dlt/common/configuration/providers/environ.py
+-rw-r--r--   0        0        0     9498 2023-05-07 18:33:09.349469 dlt-0.2.6a2/dlt/common/configuration/providers/google_secrets.py
+-rw-r--r--   0        0        0     1108 2023-05-07 12:58:14.469469 dlt-0.2.6a2/dlt/common/configuration/providers/provider.py
+-rw-r--r--   0        0        0     5235 2023-05-07 18:28:29.189469 dlt-0.2.6a2/dlt/common/configuration/providers/toml.py
+-rw-r--r--   0        0        0    17421 2023-05-07 15:41:10.039469 dlt-0.2.6a2/dlt/common/configuration/resolve.py
+-rw-r--r--   0        0        0     1176 2023-05-06 11:01:57.676603 dlt-0.2.6a2/dlt/common/configuration/specs/__init__.py
+-rw-r--r--   0        0        0     1817 2023-05-06 11:01:10.206603 dlt-0.2.6a2/dlt/common/configuration/specs/api_credentials.py
+-rw-r--r--   0        0        0    13108 2023-05-07 15:36:02.179469 dlt-0.2.6a2/dlt/common/configuration/specs/base_configuration.py
+-rw-r--r--   0        0        0     4405 2023-05-07 19:22:59.599469 dlt-0.2.6a2/dlt/common/configuration/specs/config_providers_context.py
+-rw-r--r--   0        0        0     2792 2023-03-23 14:48:32.551618 dlt-0.2.6a2/dlt/common/configuration/specs/config_section_context.py
+-rw-r--r--   0        0        0     1798 2023-05-07 15:28:27.649469 dlt-0.2.6a2/dlt/common/configuration/specs/connection_string_credentials.py
+-rw-r--r--   0        0        0     2125 2023-04-24 18:26:21.111453 dlt-0.2.6a2/dlt/common/configuration/specs/exceptions.py
+-rw-r--r--   0        0        0    12725 2023-05-07 18:34:32.579469 dlt-0.2.6a2/dlt/common/configuration/specs/gcp_credentials.py
+-rw-r--r--   0        0        0      725 2023-05-07 08:35:40.786864 dlt-0.2.6a2/dlt/common/configuration/specs/known_sections.py
+-rw-r--r--   0        0        0      556 2023-03-23 14:48:32.551618 dlt-0.2.6a2/dlt/common/configuration/specs/load_volume_configuration.py
+-rw-r--r--   0        0        0      417 2023-03-23 14:48:32.551618 dlt-0.2.6a2/dlt/common/configuration/specs/normalize_volume_configuration.py
+-rw-r--r--   0        0        0     2455 2023-04-30 21:17:44.388805 dlt-0.2.6a2/dlt/common/configuration/specs/run_configuration.py
+-rw-r--r--   0        0        0      944 2023-03-23 14:48:32.551618 dlt-0.2.6a2/dlt/common/configuration/specs/schema_volume_configuration.py
+-rw-r--r--   0        0        0     6026 2023-05-06 20:38:37.173451 dlt-0.2.6a2/dlt/common/configuration/utils.py
+-rw-r--r--   0        0        0      142 2023-03-23 14:48:32.551618 dlt-0.2.6a2/dlt/common/data_types/__init__.py
+-rw-r--r--   0        0        0     6306 2023-03-23 14:48:32.551618 dlt-0.2.6a2/dlt/common/data_types/type_helpers.py
+-rw-r--r--   0        0        0      214 2023-03-23 14:48:32.551618 dlt-0.2.6a2/dlt/common/data_types/typing.py
+-rw-r--r--   0        0        0      260 2023-03-23 14:48:20.701618 dlt-0.2.6a2/dlt/common/data_writers/__init__.py
+-rw-r--r--   0        0        0     5893 2023-03-23 14:48:32.551618 dlt-0.2.6a2/dlt/common/data_writers/buffered.py
+-rw-r--r--   0        0        0     2395 2023-03-23 14:48:32.551618 dlt-0.2.6a2/dlt/common/data_writers/escape.py
+-rw-r--r--   0        0        0      962 2023-03-23 14:48:32.551618 dlt-0.2.6a2/dlt/common/data_writers/exceptions.py
+-rw-r--r--   0        0        0     5159 2023-03-23 14:48:32.551618 dlt-0.2.6a2/dlt/common/data_writers/writers.py
+-rw-r--r--   0        0        0       97 2023-03-23 14:48:32.551618 dlt-0.2.6a2/dlt/common/destination/__init__.py
+-rw-r--r--   0        0        0     2206 2023-04-05 08:03:40.638919 dlt-0.2.6a2/dlt/common/destination/capabilities.py
+-rw-r--r--   0        0        0    10682 2023-04-24 11:35:34.867759 dlt-0.2.6a2/dlt/common/destination/reference.py
+-rw-r--r--   0        0        0     6121 2023-04-30 21:17:44.388805 dlt-0.2.6a2/dlt/common/exceptions.py
+-rw-r--r--   0        0        0     4954 2023-03-23 14:48:32.551618 dlt-0.2.6a2/dlt/common/git.py
+-rw-r--r--   0        0        0     5248 2023-04-10 08:12:53.759595 dlt-0.2.6a2/dlt/common/json/__init__.py
+-rw-r--r--   0        0        0     1802 2023-04-10 08:12:53.769595 dlt-0.2.6a2/dlt/common/json/_orjson.py
+-rw-r--r--   0        0        0     2939 2023-04-10 08:12:53.769595 dlt-0.2.6a2/dlt/common/json/_simplejson.py
+-rw-r--r--   0        0        0     1536 2023-04-29 12:58:55.943219 dlt-0.2.6a2/dlt/common/jsonpath.py
+-rw-r--r--   0        0        0      232 2023-03-23 14:48:32.551618 dlt-0.2.6a2/dlt/common/normalizers/__init__.py
+-rw-r--r--   0        0        0     1197 2023-05-07 15:38:15.119469 dlt-0.2.6a2/dlt/common/normalizers/configuration.py
+-rw-r--r--   0        0        0      472 2023-03-23 14:48:32.551618 dlt-0.2.6a2/dlt/common/normalizers/exceptions.py
+-rw-r--r--   0        0        0     1644 2023-04-06 15:27:24.759561 dlt-0.2.6a2/dlt/common/normalizers/json/__init__.py
+-rw-r--r--   0        0        0    13396 2023-04-06 15:27:24.759561 dlt-0.2.6a2/dlt/common/normalizers/json/relational.py
+-rw-r--r--   0        0        0       64 2023-03-23 14:48:32.551618 dlt-0.2.6a2/dlt/common/normalizers/naming/__init__.py
+-rw-r--r--   0        0        0      807 2023-03-23 14:48:32.551618 dlt-0.2.6a2/dlt/common/normalizers/naming/direct.py
+-rw-r--r--   0        0        0     1069 2023-03-23 14:48:32.551618 dlt-0.2.6a2/dlt/common/normalizers/naming/duck_case.py
+-rw-r--r--   0        0        0      792 2023-03-23 14:48:32.551618 dlt-0.2.6a2/dlt/common/normalizers/naming/exceptions.py
+-rw-r--r--   0        0        0     3753 2023-04-05 08:03:40.638919 dlt-0.2.6a2/dlt/common/normalizers/naming/naming.py
+-rw-r--r--   0        0        0     3002 2023-03-23 14:48:32.551618 dlt-0.2.6a2/dlt/common/normalizers/naming/snake_case.py
+-rw-r--r--   0        0        0      358 2023-04-02 09:09:15.855769 dlt-0.2.6a2/dlt/common/normalizers/typing.py
+-rw-r--r--   0        0        0     2337 2023-04-06 15:27:24.759561 dlt-0.2.6a2/dlt/common/normalizers/utils.py
+-rw-r--r--   0        0        0      451 2023-03-23 14:48:32.551618 dlt-0.2.6a2/dlt/common/pendulum.py
+-rw-r--r--   0        0        0    16937 2023-04-30 21:17:44.388805 dlt-0.2.6a2/dlt/common/pipeline.py
+-rw-r--r--   0        0        0        0 2023-03-23 14:48:32.551618 dlt-0.2.6a2/dlt/common/reflection/__init__.py
+-rw-r--r--   0        0        0      374 2023-03-23 14:48:32.551618 dlt-0.2.6a2/dlt/common/reflection/function_visitor.py
+-rw-r--r--   0        0        0     4891 2023-04-09 16:39:04.593180 dlt-0.2.6a2/dlt/common/reflection/spec.py
+-rw-r--r--   0        0        0     5069 2023-04-24 18:26:21.111453 dlt-0.2.6a2/dlt/common/reflection/utils.py
+-rw-r--r--   0        0        0      174 2023-04-30 21:17:44.388805 dlt-0.2.6a2/dlt/common/runners/__init__.py
+-rw-r--r--   0        0        0      508 2023-04-30 21:17:44.388805 dlt-0.2.6a2/dlt/common/runners/configuration.py
+-rw-r--r--   0        0        0     2635 2023-04-30 21:17:44.388805 dlt-0.2.6a2/dlt/common/runners/pool_runner.py
+-rw-r--r--   0        0        0     4046 2023-03-23 14:48:32.561618 dlt-0.2.6a2/dlt/common/runners/runnable.py
+-rw-r--r--   0        0        0     3145 2023-03-23 14:48:32.561618 dlt-0.2.6a2/dlt/common/runners/stdout.py
+-rw-r--r--   0        0        0     2137 2023-03-23 14:48:32.561618 dlt-0.2.6a2/dlt/common/runners/synth_pickle.py
+-rw-r--r--   0        0        0      105 2023-04-30 21:17:44.388805 dlt-0.2.6a2/dlt/common/runners/typing.py
+-rw-r--r--   0        0        0     5590 2023-05-06 08:15:02.906603 dlt-0.2.6a2/dlt/common/runners/venv.py
+-rw-r--r--   0        0        0       36 2023-04-30 21:17:44.398805 dlt-0.2.6a2/dlt/common/runtime/__init__.py
+-rw-r--r--   0        0        0    13441 2023-04-30 21:17:44.398805 dlt-0.2.6a2/dlt/common/runtime/collector.py
+-rw-r--r--   0        0        0     4264 2023-04-30 21:17:44.398805 dlt-0.2.6a2/dlt/common/runtime/exec_info.py
+-rw-r--r--   0        0        0      647 2023-04-30 21:17:44.398805 dlt-0.2.6a2/dlt/common/runtime/init.py
+-rw-r--r--   0        0        0     4002 2023-04-30 21:17:44.398805 dlt-0.2.6a2/dlt/common/runtime/logger.py
+-rw-r--r--   0        0        0     2052 2023-04-30 21:17:44.398805 dlt-0.2.6a2/dlt/common/runtime/prometheus.py
+-rw-r--r--   0        0        0     7170 2023-04-22 20:26:30.632198 dlt-0.2.6a2/dlt/common/runtime/segment.py
+-rw-r--r--   0        0        0     2493 2023-04-30 21:17:44.398805 dlt-0.2.6a2/dlt/common/runtime/sentry.py
+-rw-r--r--   0        0        0     2027 2023-04-30 21:17:44.398805 dlt-0.2.6a2/dlt/common/runtime/signals.py
+-rw-r--r--   0        0        0      616 2023-04-03 18:50:36.893525 dlt-0.2.6a2/dlt/common/runtime/slack.py
+-rw-r--r--   0        0        0      720 2023-04-30 21:17:44.398805 dlt-0.2.6a2/dlt/common/runtime/telemetry.py
+-rw-r--r--   0        0        0      387 2023-04-03 18:50:36.893525 dlt-0.2.6a2/dlt/common/schema/__init__.py
+-rw-r--r--   0        0        0     1927 2023-03-23 14:48:32.561618 dlt-0.2.6a2/dlt/common/schema/detections.py
+-rw-r--r--   0        0        0     2974 2023-03-23 14:48:32.561618 dlt-0.2.6a2/dlt/common/schema/exceptions.py
+-rw-r--r--   0        0        0    25175 2023-04-09 16:39:04.593180 dlt-0.2.6a2/dlt/common/schema/schema.py
+-rw-r--r--   0        0        0     3004 2023-04-22 20:26:30.632198 dlt-0.2.6a2/dlt/common/schema/typing.py
+-rw-r--r--   0        0        0    23087 2023-04-30 21:17:44.398805 dlt-0.2.6a2/dlt/common/schema/utils.py
+-rw-r--r--   0        0        0      410 2023-03-23 14:48:32.561618 dlt-0.2.6a2/dlt/common/storages/__init__.py
+-rw-r--r--   0        0        0     1906 2023-03-23 14:48:32.561618 dlt-0.2.6a2/dlt/common/storages/data_item_storage.py
+-rw-r--r--   0        0        0     2804 2023-04-03 18:50:36.893525 dlt-0.2.6a2/dlt/common/storages/exceptions.py
+-rw-r--r--   0        0        0     9059 2023-04-05 08:03:40.638919 dlt-0.2.6a2/dlt/common/storages/file_storage.py
+-rw-r--r--   0        0        0     2685 2023-04-13 08:33:43.967587 dlt-0.2.6a2/dlt/common/storages/live_schema_storage.py
+-rw-r--r--   0        0        0    21810 2023-04-29 12:58:55.953219 dlt-0.2.6a2/dlt/common/storages/load_storage.py
+-rw-r--r--   0        0        0     2414 2023-03-23 14:48:32.561618 dlt-0.2.6a2/dlt/common/storages/normalize_storage.py
+-rw-r--r--   0        0        0     8508 2023-03-23 14:48:32.561618 dlt-0.2.6a2/dlt/common/storages/schema_storage.py
+-rw-r--r--   0        0        0     2525 2023-04-24 18:26:21.111453 dlt-0.2.6a2/dlt/common/storages/versioned_storage.py
+-rw-r--r--   0        0        0     2634 2023-05-06 13:51:40.766603 dlt-0.2.6a2/dlt/common/time.py
+-rw-r--r--   0        0        0     4736 2023-04-03 18:50:36.893525 dlt-0.2.6a2/dlt/common/typing.py
+-rw-r--r--   0        0        0    11275 2023-04-24 18:26:21.111453 dlt-0.2.6a2/dlt/common/utils.py
+-rw-r--r--   0        0        0     3686 2023-03-23 14:48:32.561618 dlt-0.2.6a2/dlt/common/validation.py
+-rw-r--r--   0        0        0     1185 2023-03-23 14:48:32.561618 dlt-0.2.6a2/dlt/common/wei.py
+-rw-r--r--   0        0        0        0 2023-03-23 14:48:32.561618 dlt-0.2.6a2/dlt/destinations/__init__.py
+-rw-r--r--   0        0        0      437 2023-03-23 14:48:32.561618 dlt-0.2.6a2/dlt/destinations/bigquery/README.md
+-rw-r--r--   0        0        0     1813 2023-04-05 08:03:40.638919 dlt-0.2.6a2/dlt/destinations/bigquery/__init__.py
+-rw-r--r--   0        0        0    12347 2023-05-06 08:09:11.286603 dlt-0.2.6a2/dlt/destinations/bigquery/bigquery.py
+-rw-r--r--   0        0        0      386 2023-05-06 08:06:12.886603 dlt-0.2.6a2/dlt/destinations/bigquery/configuration.py
+-rw-r--r--   0        0        0    10342 2023-05-07 21:18:02.789469 dlt-0.2.6a2/dlt/destinations/bigquery/sql_client.py
+-rw-r--r--   0        0        0     1935 2023-04-05 08:03:40.638919 dlt-0.2.6a2/dlt/destinations/duckdb/__init__.py
+-rw-r--r--   0        0        0     7008 2023-05-07 15:38:35.819469 dlt-0.2.6a2/dlt/destinations/duckdb/configuration.py
+-rw-r--r--   0        0        0     2754 2023-03-23 14:48:32.561618 dlt-0.2.6a2/dlt/destinations/duckdb/duck.py
+-rw-r--r--   0        0        0     6936 2023-04-21 22:25:54.789942 dlt-0.2.6a2/dlt/destinations/duckdb/sql_client.py
+-rw-r--r--   0        0        0     1671 2023-03-23 14:48:32.561618 dlt-0.2.6a2/dlt/destinations/dummy/__init__.py
+-rw-r--r--   0        0        0      736 2023-04-03 18:50:36.893525 dlt-0.2.6a2/dlt/destinations/dummy/configuration.py
+-rw-r--r--   0        0        0     4975 2023-04-24 11:35:34.867759 dlt-0.2.6a2/dlt/destinations/dummy/dummy.py
+-rw-r--r--   0        0        0     4159 2023-04-05 08:03:40.638919 dlt-0.2.6a2/dlt/destinations/exceptions.py
+-rw-r--r--   0        0        0     4983 2023-04-05 08:03:40.638919 dlt-0.2.6a2/dlt/destinations/insert_job_client.py
+-rw-r--r--   0        0        0    15357 2023-05-02 21:00:32.948848 dlt-0.2.6a2/dlt/destinations/job_client_impl.py
+-rw-r--r--   0        0        0     1303 2023-04-05 08:03:40.638919 dlt-0.2.6a2/dlt/destinations/job_impl.py
+-rw-r--r--   0        0        0      251 2023-03-23 14:48:32.561618 dlt-0.2.6a2/dlt/destinations/postgres/README.md
+-rw-r--r--   0        0        0     1934 2023-04-05 08:03:40.638919 dlt-0.2.6a2/dlt/destinations/postgres/__init__.py
+-rw-r--r--   0        0        0     1232 2023-05-06 08:19:47.236603 dlt-0.2.6a2/dlt/destinations/postgres/configuration.py
+-rw-r--r--   0        0        0     3025 2023-03-23 14:48:32.561618 dlt-0.2.6a2/dlt/destinations/postgres/postgres.py
+-rw-r--r--   0        0        0     6074 2023-05-06 08:20:42.386603 dlt-0.2.6a2/dlt/destinations/postgres/sql_client.py
+-rw-r--r--   0        0        0     1159 2023-04-03 18:50:36.893525 dlt-0.2.6a2/dlt/destinations/redshift/README.md
+-rw-r--r--   0        0        0     1905 2023-04-05 08:03:40.638919 dlt-0.2.6a2/dlt/destinations/redshift/__init__.py
+-rw-r--r--   0        0        0      570 2023-05-06 08:30:19.436603 dlt-0.2.6a2/dlt/destinations/redshift/configuration.py
+-rw-r--r--   0        0        0     3761 2023-03-23 14:48:32.561618 dlt-0.2.6a2/dlt/destinations/redshift/redshift.py
+-rw-r--r--   0        0        0     7110 2023-04-29 12:58:55.953219 dlt-0.2.6a2/dlt/destinations/sql_client.py
+-rw-r--r--   0        0        0    10101 2023-04-09 16:39:04.593180 dlt-0.2.6a2/dlt/destinations/sql_merge_job.py
+-rw-r--r--   0        0        0     1931 2023-04-24 18:26:21.111453 dlt-0.2.6a2/dlt/destinations/typing.py
+-rw-r--r--   0        0        0        0 2022-08-09 19:58:51.837922 dlt-0.2.6a2/dlt/extract/__init__.py
+-rw-r--r--   0        0        0    22860 2023-05-07 10:39:43.846864 dlt-0.2.6a2/dlt/extract/decorators.py
+-rw-r--r--   0        0        0    12645 2023-04-30 21:17:44.398805 dlt-0.2.6a2/dlt/extract/exceptions.py
+-rw-r--r--   0        0        0     8449 2023-04-30 21:17:44.398805 dlt-0.2.6a2/dlt/extract/extract.py
+-rw-r--r--   0        0        0    14658 2023-05-07 15:38:58.249469 dlt-0.2.6a2/dlt/extract/incremental.py
+-rw-r--r--   0        0        0    31567 2023-04-30 21:17:44.398805 dlt-0.2.6a2/dlt/extract/pipe.py
+-rw-r--r--   0        0        0     9683 2023-04-22 20:26:30.632198 dlt-0.2.6a2/dlt/extract/schema.py
+-rw-r--r--   0        0        0    34195 2023-05-07 10:42:54.466864 dlt-0.2.6a2/dlt/extract/source.py
+-rw-r--r--   0        0        0     4350 2023-04-22 20:26:30.632198 dlt-0.2.6a2/dlt/extract/typing.py
+-rw-r--r--   0        0        0      593 2023-04-06 20:38:35.239561 dlt-0.2.6a2/dlt/extract/utils.py
+-rw-r--r--   0        0        0        0 2022-08-14 16:06:42.572263 dlt-0.2.6a2/dlt/helpers/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-30 21:17:44.398805 dlt-0.2.6a2/dlt/helpers/airflow/__init__.py
+-rw-r--r--   0        0        0     2907 2023-03-23 14:48:32.561618 dlt-0.2.6a2/dlt/helpers/dbt/__init__.py
+-rw-r--r--   0        0        0     1220 2023-03-23 14:48:32.561618 dlt-0.2.6a2/dlt/helpers/dbt/configuration.py
+-rw-r--r--   0        0        0     6137 2023-03-23 14:48:32.561618 dlt-0.2.6a2/dlt/helpers/dbt/dbt_utils.py
+-rw-r--r--   0        0        0      758 2023-03-23 14:48:32.561618 dlt-0.2.6a2/dlt/helpers/dbt/exceptions.py
+-rw-r--r--   0        0        0     3583 2023-03-23 14:48:32.561618 dlt-0.2.6a2/dlt/helpers/dbt/profiles.yml
+-rw-r--r--   0        0        0    13032 2023-04-30 21:17:44.398805 dlt-0.2.6a2/dlt/helpers/dbt/runner.py
+-rw-r--r--   0        0        0     2373 2023-03-23 14:48:32.571618 dlt-0.2.6a2/dlt/helpers/pandas.py
+-rw-r--r--   0        0        0     1035 2023-03-23 14:48:32.571618 dlt-0.2.6a2/dlt/helpers/parquet.py
+-rw-r--r--   0        0        0    13371 2023-04-30 21:17:44.398805 dlt-0.2.6a2/dlt/helpers/streamlit.py
+-rw-r--r--   0        0        0       31 2023-03-23 14:48:32.571618 dlt-0.2.6a2/dlt/load/__init__.py
+-rw-r--r--   0        0        0     1019 2023-04-30 21:17:44.398805 dlt-0.2.6a2/dlt/load/configuration.py
+-rw-r--r--   0        0        0     1993 2023-04-05 08:03:40.638919 dlt-0.2.6a2/dlt/load/exceptions.py
+-rw-r--r--   0        0        0    19928 2023-04-30 21:17:44.398805 dlt-0.2.6a2/dlt/load/load.py
+-rw-r--r--   0        0        0       32 2023-03-23 14:48:32.571618 dlt-0.2.6a2/dlt/normalize/__init__.py
+-rw-r--r--   0        0        0     1098 2023-04-30 21:17:44.398805 dlt-0.2.6a2/dlt/normalize/configuration.py
+-rw-r--r--   0        0        0        0 2022-08-09 19:58:51.837922 dlt-0.2.6a2/dlt/normalize/exceptions.py
+-rw-r--r--   0        0        0    16576 2023-04-30 21:17:44.398805 dlt-0.2.6a2/dlt/normalize/normalize.py
+-rw-r--r--   0        0        0     1880 2023-03-23 14:48:32.571618 dlt-0.2.6a2/dlt/pipeline/README.md
+-rw-r--r--   0        0        0    13138 2023-04-30 21:17:44.398805 dlt-0.2.6a2/dlt/pipeline/__init__.py
+-rw-r--r--   0        0        0     1858 2023-04-30 21:17:44.398805 dlt-0.2.6a2/dlt/pipeline/configuration.py
+-rw-r--r--   0        0        0      363 2023-04-22 20:26:30.632198 dlt-0.2.6a2/dlt/pipeline/current.py
+-rw-r--r--   0        0        0     4829 2023-03-23 14:48:32.571618 dlt-0.2.6a2/dlt/pipeline/dbt.py
+-rw-r--r--   0        0        0     2891 2023-04-30 21:17:44.398805 dlt-0.2.6a2/dlt/pipeline/exceptions.py
+-rw-r--r--   0        0        0     8764 2023-05-02 21:05:46.788848 dlt-0.2.6a2/dlt/pipeline/helpers.py
+-rw-r--r--   0        0        0      122 2023-04-06 15:27:24.759561 dlt-0.2.6a2/dlt/pipeline/mark.py
+-rw-r--r--   0        0        0    56514 2023-05-06 11:07:29.546603 dlt-0.2.6a2/dlt/pipeline/pipeline.py
+-rw-r--r--   0        0        0      985 2023-04-30 21:17:44.398805 dlt-0.2.6a2/dlt/pipeline/progress.py
+-rw-r--r--   0        0        0     4200 2023-04-10 08:12:53.769595 dlt-0.2.6a2/dlt/pipeline/state_sync.py
+-rw-r--r--   0        0        0     7990 2023-04-03 18:50:36.903525 dlt-0.2.6a2/dlt/pipeline/trace.py
+-rw-r--r--   0        0        0     4563 2023-04-03 18:50:36.903525 dlt-0.2.6a2/dlt/pipeline/track.py
+-rw-r--r--   0        0        0       91 2023-03-23 14:48:32.571618 dlt-0.2.6a2/dlt/pipeline/typing.py
+-rw-r--r--   0        0        0        0 2022-06-03 13:18:25.174600 dlt-0.2.6a2/dlt/py.typed
+-rw-r--r--   0        0        0        0 2023-03-23 14:48:32.571618 dlt-0.2.6a2/dlt/reflection/__init__.py
+-rw-r--r--   0        0        0      563 2023-03-23 14:48:32.571618 dlt-0.2.6a2/dlt/reflection/names.py
+-rw-r--r--   0        0        0     5617 2023-05-06 09:23:33.456603 dlt-0.2.6a2/dlt/reflection/script_inspector.py
+-rw-r--r--   0        0        0     6186 2023-03-23 14:48:32.571618 dlt-0.2.6a2/dlt/reflection/script_visitor.py
+-rw-r--r--   0        0        0      124 2023-05-05 18:33:47.789796 dlt-0.2.6a2/dlt/sources/__init__.py
+-rw-r--r--   0        0        0      320 2023-05-06 11:10:16.076603 dlt-0.2.6a2/dlt/sources/credentials.py
+-rw-r--r--   0        0        0        0 2023-03-23 14:48:32.571618 dlt-0.2.6a2/dlt/sources/helpers/__init__.py
+-rw-r--r--   0        0        0      574 2023-03-23 14:48:37.261618 dlt-0.2.6a2/dlt/sources/helpers/requests/__init__.py
+-rw-r--r--   0        0        0     9092 2023-04-24 18:26:21.111453 dlt-0.2.6a2/dlt/sources/helpers/requests/retry.py
+-rw-r--r--   0        0        0     1336 2023-03-23 14:48:32.571618 dlt-0.2.6a2/dlt/sources/helpers/requests/session.py
+-rw-r--r--   0        0        0      679 2023-04-06 15:27:24.759561 dlt-0.2.6a2/dlt/sources/helpers/transform.py
+-rw-r--r--   0        0        0     1125 2023-04-22 20:26:30.632198 dlt-0.2.6a2/dlt/version.py
+-rw-r--r--   0        0        0     4056 2023-05-07 18:36:19.729469 dlt-0.2.6a2/pyproject.toml
+-rw-r--r--   0        0        0     7395 1970-01-01 00:00:00.000000 dlt-0.2.6a2/setup.py
+-rw-r--r--   0        0        0     7323 1970-01-01 00:00:00.000000 dlt-0.2.6a2/PKG-INFO
```

### Comparing `dlt-0.2.6a1/LICENSE.txt` & `dlt-0.2.6a2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/README.md` & `dlt-0.2.6a2/README.md`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/__init__.py` & `dlt-0.2.6a2/dlt/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/cli/_dlt.py` & `dlt-0.2.6a2/dlt/cli/_dlt.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from typing import Any, Sequence
 import yaml
 import os
 import argparse
 import click
-from dlt.cli.telemetry_command import DLT_TELEMETRY_DOCS_URL, change_telemetry_status_command, telemetry_status_command
 
 from dlt.version import __version__
 from dlt.common import json
 from dlt.common.schema import Schema
 from dlt.common.typing import DictStrAny
+from dlt.common.runners import Venv
 
 import dlt.cli.echo as fmt
 from dlt.cli import utils
 from dlt.cli.init_command import init_command, list_pipelines_command, DLT_INIT_DOCS_URL, DEFAULT_PIPELINES_REPO
 from dlt.cli.deploy_command import PipelineWasNotRun, deploy_command, DLT_DEPLOY_DOCS_URL
 from dlt.cli.pipeline_command import pipeline_command, DLT_PIPELINE_COMMAND_DOCS_URL
+from dlt.cli.telemetry_command import DLT_TELEMETRY_DOCS_URL, change_telemetry_status_command, telemetry_status_command
 from dlt.pipeline.exceptions import CannotRestorePipelineException
 
 
 @utils.track_command("init", False, "pipeline_name", "destination_name")
 def init_command_wrapper(pipeline_name: str, destination_name: str, use_generic_template: bool, repo_location: str, branch: str) -> int:
     try:
         init_command(pipeline_name, destination_name, use_generic_template, repo_location, branch)
@@ -240,14 +241,17 @@
     pipe_cmd_package = pipeline_subparsers.add_parser("load-package", help="Displays information on load package, use -v or -vv for more info")
     pipe_cmd_package.add_argument("load_id", metavar="load-id", nargs='?', help="Load id of completed or normalized package. Defaults to the most recent package.")
 
     subparsers.add_parser("telemetry", help="Shows telemetry status")
 
     args = parser.parse_args()
 
+    if Venv.is_virtual_env() and not Venv.is_venv_activated():
+        fmt.warning("You are running dlt installed in the global environment, however you have virtual environment activated. The dlt command will not see dependencies from virtual environment. You should uninstall the dlt from global environment and install it in the current virtual environment instead.")
+
     if args.command == "schema":
         return schema_command_wrapper(args.file, args.format, args.remove_defaults)
     elif args.command == "pipeline":
         if args.list_pipelines:
             return pipeline_command_wrapper("list", "-", args.pipelines_dir, args.verbosity)
         else:
             command_kwargs = dict(args._get_kwargs())
```

### Comparing `dlt-0.2.6a1/dlt/cli/config_toml_writer.py` & `dlt-0.2.6a2/dlt/cli/config_toml_writer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-from typing import Any, Iterable, NamedTuple, Tuple
+from typing import Any, NamedTuple, Tuple, Iterable
 import tomlkit
 from tomlkit.items import Table as TOMLTable
+from tomlkit.container import Container as TOMLContainer
 from collections.abc import Sequence as C_Sequence
 
 from dlt.common import pendulum
 from dlt.common.configuration.specs import BaseConfiguration, is_base_configuration_inner_hint, extract_inner_hint
 from dlt.common.data_types import py_type_to_sc_type
 from dlt.common.typing import AnyType, is_final_type, is_optional_type
 
@@ -83,15 +84,15 @@
     for name, hint in config.get_resolvable_fields().items():
         default_value = getattr(config, name, None)
         # check if field is of particular interest and should be included if it has default
         is_default_of_interest = name in config.__config_gen_annotations__
         write_value(toml_table, name, hint, overwrite_existing, default_value=default_value, is_default_of_interest=is_default_of_interest)
 
 
-def write_values(toml: tomlkit.TOMLDocument, values: Iterable[WritableConfigValue], overwrite_existing: bool) -> None:
+def write_values(toml: TOMLContainer, values: Iterable[WritableConfigValue], overwrite_existing: bool) -> None:
     for value in values:
         toml_table: TOMLTable = toml  # type: ignore
         for section in value.sections:
             if section not in toml_table:
                 inner_table = tomlkit.table(True)
                 toml_table[section] = inner_table
                 toml_table = inner_table
```

### Comparing `dlt-0.2.6a1/dlt/cli/deploy_command.py` & `dlt-0.2.6a2/dlt/cli/deploy_command.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/cli/echo.py` & `dlt-0.2.6a2/dlt/cli/echo.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/cli/init_command.py` & `dlt-0.2.6a2/dlt/cli/init_command.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/cli/pipeline_command.py` & `dlt-0.2.6a2/dlt/cli/pipeline_command.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/cli/pipeline_files.py` & `dlt-0.2.6a2/dlt/cli/pipeline_files.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/cli/source_detection.py` & `dlt-0.2.6a2/dlt/cli/source_detection.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import ast
 import inspect
 from astunparse import unparse
 from typing import Dict, Tuple, Set, List
 
 from dlt.common.configuration import is_secret_hint
+from dlt.common.configuration.specs import BaseConfiguration
 from dlt.common.reflection.utils import creates_func_def_name_node
 from dlt.common.typing import is_optional_type
 
 from dlt.cli.config_toml_writer import WritableConfigValue
 from dlt.cli.exceptions import CliCommandException
 from dlt.extract.decorators import SourceInfo
 from dlt.reflection.script_visitor import PipelineScriptVisitor
@@ -62,15 +63,15 @@
     # all sources checked
     checked_sources: Dict[str, SourceInfo] = {}
 
     for source_name, source_info in sources.items():
         # accept only sources declared in the `init` or `pipeline` modules
         if source_info.module.__name__.startswith(module_prefix):
             checked_sources[source_name] = source_info
-            source_config = source_info.SPEC()
+            source_config = source_info.SPEC() if source_info.SPEC else BaseConfiguration()
             spec_fields = source_config.get_resolvable_fields()
             for field_name, field_type in spec_fields.items():
                 val_store = None
                 # all secrets must go to secrets.toml
                 if is_secret_hint(field_type):
                     val_store = required_secrets
                 # all configs that are required and do not have a default value must go to config.toml
```

### Comparing `dlt-0.2.6a1/dlt/cli/telemetry_command.py` & `dlt-0.2.6a2/dlt/cli/telemetry_command.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/cli/utils.py` & `dlt-0.2.6a2/dlt/cli/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/common/arithmetics.py` & `dlt-0.2.6a2/dlt/common/arithmetics.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/common/configuration/accessors.py` & `dlt-0.2.6a2/dlt/common/configuration/accessors.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,89 +1,69 @@
 import abc
 import contextlib
+import tomlkit
 from typing import Any, ClassVar, List, Sequence, Tuple, Type, TypeVar
-from dlt.common import json
+
 from dlt.common.configuration.container import Container
 from dlt.common.configuration.exceptions import ConfigFieldMissingException, LookupTrace
-
 from dlt.common.configuration.providers.provider import ConfigProvider
 from dlt.common.configuration.specs import BaseConfiguration, is_base_configuration_inner_hint
-from dlt.common.configuration.utils import deserialize_value, log_traces
+from dlt.common.configuration.utils import deserialize_value, log_traces, auto_cast
 from dlt.common.configuration.specs.config_providers_context import ConfigProvidersContext
-from dlt.common.data_types import coerce_value
 from dlt.common.typing import AnyType, ConfigValue, TSecretValue
 
 DLT_SECRETS_VALUE = "secrets.value"
 DLT_CONFIG_VALUE = "config.value"
 TConfigAny = TypeVar("TConfigAny", bound=Any)
 
 class _Accessor(abc.ABC):
 
     def __getitem__(self, field: str) -> Any:
         value, traces = self._get_value(field)
         if value is None:
             raise ConfigFieldMissingException("Any", {field: traces})
         if isinstance(value, str):
-            return self._auto_cast(value)
+            return auto_cast(value)
         else:
             return value
 
-
     def get(self, field: str, expected_type: Type[TConfigAny] = None) -> TConfigAny:
         value: TConfigAny
         value, _ = self._get_value(field, expected_type)
         if value is None:
             return None
         # cast to required type
         if expected_type:
             return deserialize_value(field, value, expected_type)
         else:
             return value
 
-
     @property
     @abc.abstractmethod
     def config_providers(self) -> Sequence[ConfigProvider]:
         pass
 
     @property
     @abc.abstractmethod
     def default_type(self) -> AnyType:
         pass
 
     def _get_providers_from_context(self) -> Sequence[ConfigProvider]:
         return Container()[ConfigProvidersContext].providers
 
-    def _auto_cast(self, value: str) -> Any:
-        # try to cast to bool, int, float and complex (via JSON)
-        if value.lower() == "true":
-            return True
-        if value.lower() == "false":
-            return False
-        with contextlib.suppress(ValueError):
-            return coerce_value("bigint", "text", value)
-        with contextlib.suppress(ValueError):
-            return coerce_value("double", "text", value)
-        with contextlib.suppress(ValueError):
-            c_v = json.loads(value)
-            # only lists and dictionaries count
-            if isinstance(c_v, (list, dict)):
-                return c_v
-        return value
-
     def _get_value(self, field: str, type_hint: Type[Any] = None) -> Tuple[Any, List[LookupTrace]]:
         # get default hint type, in case of dlt.secrets it it TSecretValue
         type_hint = type_hint or self.default_type
         # split field into sections and a key
         sections = field.split(".")
         key = sections.pop()
         value = None
         traces: List[LookupTrace] = []
         for provider in self.config_providers:
-            value, effective_field = provider.get_value(key, type_hint, *sections)
+            value, effective_field = provider.get_value(key, type_hint, None, *sections)
             trace = LookupTrace(provider.name, sections, effective_field, value)
             traces.append(trace)
             if value is not None:
                 # log trace
                 if is_base_configuration_inner_hint(type_hint):
                     config: BaseConfiguration = type_hint  # type: ignore
                 else:
```

### Comparing `dlt-0.2.6a1/dlt/common/configuration/container.py` & `dlt-0.2.6a2/dlt/common/configuration/container.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,22 +38,23 @@
             raise KeyError(f"{spec.__name__} is not a context")
 
         item = self.contexts.get(spec)
         if item is None:
             if spec.can_create_default:
                 item = spec()
                 self.contexts[spec] = item
+                item.add_extras()
             else:
                 raise ContextDefaultCannotBeCreated(spec)
 
         return item  # type: ignore
 
     def __setitem__(self, spec: Type[TConfiguration], value: TConfiguration) -> None:
         # value passed to container must be final
-        value.__is_resolved__ = True
+        value.resolve()
         # put it into context
         self.contexts[spec] = value
 
     def __delitem__(self, spec: Type[TConfiguration]) -> None:
         del self.contexts[spec]
 
     def __contains__(self, spec: Type[TConfiguration]) -> bool:
```

### Comparing `dlt-0.2.6a1/dlt/common/configuration/exceptions.py` & `dlt-0.2.6a2/dlt/common/configuration/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/common/configuration/inject.py` & `dlt-0.2.6a2/dlt/common/configuration/inject.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/common/configuration/paths.py` & `dlt-0.2.6a2/dlt/common/configuration/paths.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/common/configuration/providers/airflow.py` & `dlt-0.2.6a2/dlt/common/configuration/providers/airflow.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/common/configuration/providers/context.py` & `dlt-0.2.6a2/dlt/common/configuration/providers/context.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     def __init__(self) -> None:
         self.container = Container()
 
     @property
     def name(self) -> str:
         return ContextProvider.NAME
 
-    def get_value(self, key: str, hint: Type[Any], *sections: str) -> Tuple[Optional[Any], str]:
+    def get_value(self, key: str, hint: Type[Any], pipeline_name: str = None, *sections: str) -> Tuple[Optional[Any], str]:
         assert sections == ()
 
         # only context is a valid hint
         with contextlib.suppress(KeyError, TypeError):
             if issubclass(hint, ContainerInjectableContext):
                 # contexts without defaults will raise ContextDefaultCannotBeCreated
                 return self.container[hint], hint.__name__
```

### Comparing `dlt-0.2.6a1/dlt/common/configuration/providers/dictionary.py` & `dlt-0.2.6a2/dlt/common/configuration/providers/dictionary.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 from contextlib import contextmanager
 from typing import Any, ClassVar, Iterator, Optional, Type, Tuple
 
 from dlt.common.typing import StrAny
 
-from .provider import ConfigProvider
+from .provider import ConfigProvider, get_key_name
 
 
 class DictionaryProvider(ConfigProvider):
 
     NAME: ClassVar[str] = "Dictionary Provider"
 
     def __init__(self) -> None:
         self._values: StrAny = {}
 
     @property
     def name(self) -> str:
         return self.NAME
 
-    def get_value(self, key: str, hint: Type[Any], *sections: str) -> Tuple[Optional[Any], str]:
+    def get_value(self, key: str, hint: Type[Any], pipeline_name: str, *sections: str) -> Tuple[Optional[Any], str]:
         full_path = sections + (key,)
-        full_key = "__".join(full_path)
+        if pipeline_name:
+            full_path = (pipeline_name, ) + full_path
+        full_key = get_key_name(key, "__", pipeline_name, *sections)
         node = self._values
         try:
             for k in  full_path:
                 if not isinstance(node, dict):
                     raise KeyError(k)
                 node = node[k]
             return node, full_key
@@ -34,14 +36,13 @@
     def supports_secrets(self) -> bool:
         return True
 
     @property
     def supports_sections(self) -> bool:
         return True
 
-
     @contextmanager
     def values(self, v: StrAny) -> Iterator[None]:
         p_values = self._values
         self._values = v
         yield
         self._values = p_values
```

### Comparing `dlt-0.2.6a1/dlt/common/configuration/providers/environ.py` & `dlt-0.2.6a2/dlt/common/configuration/providers/environ.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,30 @@
 from os import environ
 from os.path import isdir
 from typing import Any, Optional, Type, Tuple
 
 from dlt.common.typing import TSecretValue
 
-from .provider import ConfigProvider
+from .provider import ConfigProvider, get_key_name
 
 SECRET_STORAGE_PATH: str = "/run/secrets/%s"
 
 class EnvironProvider(ConfigProvider):
 
     @staticmethod
     def get_key_name(key: str, *sections: str) -> str:
-        # env key is always upper case
-        if sections:
-            sections = filter(lambda x: bool(x), sections)  # type: ignore
-            env_key = "__".join((*sections, key))
-        else:
-            env_key = key
-        return env_key.upper()
+        return get_key_name(key, "__", *sections).upper()
 
     @property
     def name(self) -> str:
         return "Environment Variables"
 
-    def get_value(self, key: str, hint: Type[Any], *sections: str) -> Tuple[Optional[Any], str]:
+    def get_value(self, key: str, hint: Type[Any], pipeline_name: str, *sections: str) -> Tuple[Optional[Any], str]:
         # apply section to the key
-        key = self.get_key_name(key, *sections)
+        key = self.get_key_name(key, pipeline_name, *sections)
         if hint is TSecretValue:
             # try secret storage
             try:
                 # must conform to RFC1123
                 secret_name = key.lower().replace("_", "-")
                 secret_path = SECRET_STORAGE_PATH % secret_name
                 # kubernetes stores secrets as files in a dir, docker compose plainly
@@ -52,7 +46,11 @@
     @property
     def supports_secrets(self) -> bool:
         return True
 
     @property
     def supports_sections(self) -> bool:
         return True
+
+    @property
+    def is_empty(self) -> bool:
+        return len(environ) == 0
```

### Comparing `dlt-0.2.6a1/dlt/common/configuration/providers/provider.py` & `dlt-0.2.6a2/dlt/common/configuration/providers/provider.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import abc
 from typing import Any, Tuple, Type, Optional
 
 from dlt.common.configuration.exceptions import ConfigurationException
 
 
-
 class ConfigProvider(abc.ABC):
 
     @abc.abstractmethod
-    def get_value(self, key: str, hint: Type[Any], *sections: str) -> Tuple[Optional[Any], str]:
+    def get_value(self, key: str, hint: Type[Any], pipeline_name: str, *sections: str) -> Tuple[Optional[Any], str]:
         pass
 
     @property
     @abc.abstractmethod
     def supports_secrets(self) -> bool:
         pass
 
@@ -22,12 +21,26 @@
         pass
 
     @property
     @abc.abstractmethod
     def name(self) -> str:
         pass
 
+    @property
+    def is_empty(self) -> bool:
+        return False
+
+
+
+def get_key_name(key: str, separator: str, /, *sections: str) -> str:
+    if sections:
+        sections = filter(lambda x: bool(x), sections)  # type: ignore
+        env_key = separator.join((*sections, key))
+    else:
+        env_key = key
+    return env_key
+
 
 class ConfigProviderException(ConfigurationException):
     def __init__(self, provider_name: str, *args: Any) -> None:
         self.provider_name = provider_name
         super().__init__(*args)
```

### Comparing `dlt-0.2.6a1/dlt/common/configuration/providers/toml.py` & `dlt-0.2.6a2/dlt/common/configuration/providers/toml.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,36 +3,32 @@
 from tomlkit.items import Item as TOMLItem
 from tomlkit.container import Container as TOMLContainer
 from typing import Any, Optional, Tuple, Type, Union
 
 from dlt.common.configuration.paths import get_dlt_project_dir, get_dlt_home_dir
 from dlt.common.utils import update_dict_nested
 
-from .provider import ConfigProvider, ConfigProviderException
+from .provider import ConfigProvider, ConfigProviderException, get_key_name
 
 CONFIG_TOML = "config.toml"
 SECRETS_TOML = "secrets.toml"
 
 class BaseTomlProvider(ConfigProvider):
-    def __init__(self, toml_document: tomlkit.TOMLDocument) -> None:
+    def __init__(self, toml_document: TOMLContainer) -> None:
         self._toml = toml_document
 
     @staticmethod
     def get_key_name(key: str, *sections: str) -> str:
-        # env key is always upper case
-        if sections:
-            sections = filter(lambda x: bool(x), sections)  # type: ignore
-            env_key = ".".join((*sections, key))
-        else:
-            env_key = key
-        return env_key
+        return get_key_name(key, ".", *sections)
 
-    def get_value(self, key: str, hint: Type[Any], *sections: str) -> Tuple[Optional[Any], str]:
+    def get_value(self, key: str, hint: Type[Any], pipeline_name: str, *sections: str) -> Tuple[Optional[Any], str]:
         full_path = sections + (key,)
-        full_key = self.get_key_name(key, *sections)
+        if pipeline_name:
+            full_path = (pipeline_name, ) + full_path
+        full_key = self.get_key_name(key, pipeline_name, *sections)
         node: Union[TOMLContainer, TOMLItem] = self._toml
         try:
             for k in full_path:
                 if not isinstance(node, dict):
                     raise KeyError(k)
                 node = node[k]
             rv = node.unwrap() if isinstance(node, (TOMLContainer, TOMLItem)) else node
@@ -42,19 +38,18 @@
 
     @property
     def supports_sections(self) -> bool:
         return True
 
     @property
     def is_empty(self) -> bool:
-        # no keys
-        return self._toml.as_string() == ""
+        return len(self._toml.body) == 0
 
 
-class TomlProvider(BaseTomlProvider):
+class TomlFileProvider(BaseTomlProvider):
     def __init__(self, file_name: str, project_dir: str = None, add_global_config: bool = False) -> None:
         """Creates config provider from a `toml` file
 
         The provider loads the `toml` file with specified name and from specified folder. If `add_global_config` flags is specified,
         it will look for `file_name` in `dlt` home dir. The "project" (`project_dir`) values overwrite the "global" values.
 
         If none of the files exist, an empty provider is created.
@@ -98,30 +93,30 @@
             with open(toml_path, "r", encoding="utf-8") as f:
                 # use whitespace preserving parser
                 return tomlkit.load(f)
         else:
             return tomlkit.document()
 
 
-class ConfigTomlProvider(TomlProvider):
+class ConfigTomlProvider(TomlFileProvider):
 
     def __init__(self, project_dir: str = None, add_global_config: bool = False) -> None:
         super().__init__(CONFIG_TOML, project_dir=project_dir, add_global_config=add_global_config)
 
     @property
     def name(self) -> str:
         return CONFIG_TOML
 
     @property
     def supports_secrets(self) -> bool:
         return False
 
 
 
-class SecretsTomlProvider(TomlProvider):
+class SecretsTomlProvider(TomlFileProvider):
 
     def __init__(self, project_dir: str = None, add_global_config: bool = False) -> None:
         super().__init__(SECRETS_TOML, project_dir=project_dir, add_global_config=add_global_config)
 
     @property
     def name(self) -> str:
         return SECRETS_TOML
```

### Comparing `dlt-0.2.6a1/dlt/common/configuration/resolve.py` & `dlt-0.2.6a2/dlt/common/configuration/resolve.py`

 * *Files 6% similar despite different names*

```diff
@@ -60,15 +60,14 @@
         # print(f"TRYING TO PARSE NATIVE from {explicit_value}")
         try:
             config.parse_native_representation(explicit_value)
         except ValueError as v_err:
             # provide generic exception
             raise InvalidNativeValue(type(config), type(explicit_value), embedded_sections, v_err)
         except NotImplementedError:
-
             pass
         # explicit value was consumed
         explicit_value = None
     return explicit_value
 
 def _resolve_configuration(
         config: TConfiguration,
@@ -84,28 +83,24 @@
     config.__exception__ = None
     try:
         try:
             explicit_value = _maybe_parse_native_value(config, explicit_value, embedded_sections)
             # if native representation didn't fully resolve the config, we try to resolve field by field
             if not config.is_resolved():
                 _resolve_config_fields(config, explicit_value, explicit_sections, embedded_sections, accept_partial)
-
-            _call_method_in_mro(config, "on_resolved")
             # full configuration was resolved
-            config.__is_resolved__ = True
+            config.resolve()
         except ConfigFieldMissingException as cm_ex:
             # store the ConfigEntryMissingException to have full info on traces of missing fields
             config.__exception__ = cm_ex
-            _call_method_in_mro(config, "on_partial")
+            # may resolve in partial handler
+            config.call_method_in_mro("on_partial")
             # if resolved then do not raise
-            if config.is_resolved():
-                _call_method_in_mro(config, "on_resolved")
-            else:
-                if not accept_partial:
-                    raise
+            if not config.is_resolved() and not accept_partial:
+                raise
     except Exception as ex:
         # store the exception that happened in the resolution process
         config.__exception__ = ex
         raise
 
     return config
 
@@ -247,28 +242,14 @@
             # do not deserialize explicit values
             if value is not explicit_value:
                 value = deserialize_value(key, value, inner_hint)
 
     return default_value if value is None else value, traces
 
 
-def _call_method_in_mro(config: BaseConfiguration, method_name: str) -> None:
-    # python multi-inheritance is cooperative and this would require that all configurations cooperatively
-    # call each other class_method_name. this is not at all possible as we do not know which configs in the end will
-    # be mixed together.
-
-    # get base classes in order of derivation
-    mro = type.mro(type(config))
-    for c in mro:
-        # check if this class implements on_resolved (skip pure inheritance to not do double work)
-        if method_name in c.__dict__ and callable(getattr(c, method_name)):
-            # pass right class instance
-            c.__dict__[method_name](config)
-
-
 def _resolve_single_value(
         key: str,
         hint: Type[Any],
         inner_hint: Type[Any],
         config_section: str,
         explicit_sections: Tuple[str, ...],
         embedded_sections: Tuple[str, ...]
@@ -279,29 +260,34 @@
 
     container = Container()
     # get providers from container
     providers_context = container[ConfigProvidersContext]
     # we may be resolving context
     if is_context_inner_hint(inner_hint):
         # resolve context with context provider and do not look further
-        value, _ = providers_context.context_provider.get_value(key, inner_hint)
+        value, _ = providers_context.context_provider.get_value(key, inner_hint, None)
         return value, traces
     if is_base_configuration_inner_hint(inner_hint):
         # cannot resolve configurations directly
         return value, traces
 
     # resolve a field of the config
     config_section, embedded_sections = _apply_embedded_sections_to_config_sections(config_section, embedded_sections)
     providers = providers_context.providers
     # get additional sections to look in from container
     sections_context = container[ConfigSectionContext]
 
     def look_sections(pipeline_name: str = None) -> Any:
         # start looking from the top provider with most specific set of sections first
+        value: Any = None
         for provider in providers:
+            if provider.is_empty:
+                # do not query empty provider so they are not added to the trace
+                continue
+
             value, provider_traces = resolve_single_provider_value(
                 provider,
                 key,
                 hint,
                 pipeline_name,
                 config_section,
                 # if explicit sections are provided, ignore the injected context
@@ -346,25 +332,25 @@
             return None, traces
         else:
             # pass empty sections
             ns = []
 
     value = None
     while True:
-        if (pipeline_name or config_section) and provider.supports_sections:
+        if config_section and provider.supports_sections:
             full_ns = ns.copy()
             # pipeline, when provided, is the most outer and always present
-            if pipeline_name:
-                full_ns.insert(0, pipeline_name)
+            # if pipeline_name:
+            #     full_ns.insert(0, pipeline_name)
             # config section, is always present and innermost
             if config_section:
                 full_ns.append(config_section)
         else:
             full_ns = ns
-        value, ns_key = provider.get_value(key, hint, *full_ns)
+        value, ns_key = provider.get_value(key, hint, pipeline_name, *full_ns)
         # if secret is obtained from non secret provider, we must fail
         cant_hold_it: bool = not provider.supports_secrets and is_secret_hint(hint)
         if value is not None and cant_hold_it:
             raise ValueNotSecretException(provider.name, ns_key)
 
         # create trace, ignore providers that cant_hold_it
         if not cant_hold_it:
```

### Comparing `dlt-0.2.6a1/dlt/common/configuration/specs/__init__.py` & `dlt-0.2.6a2/dlt/common/configuration/specs/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,14 @@
 from .run_configuration import RunConfiguration  # noqa: F401
-from .base_configuration import BaseConfiguration, CredentialsConfiguration, CredentialsWithDefault, ContainerInjectableContext, extract_inner_hint, is_base_configuration_inner_hint  # noqa: F401
+from .base_configuration import BaseConfiguration, CredentialsConfiguration, CredentialsWithDefault, ContainerInjectableContext, extract_inner_hint, is_base_configuration_inner_hint, configspec  # noqa: F401
 from .normalize_volume_configuration import NormalizeVolumeConfiguration  # noqa: F401
 from .load_volume_configuration import LoadVolumeConfiguration  # noqa: F401
 from .schema_volume_configuration import SchemaVolumeConfiguration, TSchemaFileFormat  # noqa: F401
-from .gcp_client_credentials import GcpClientCredentials, GcpClientCredentialsWithDefault, GcpOAuthCredentials, GcpOAuthCredentialsWithDefault  # noqa: F401
-from .postgres_credentials import PostgresCredentials, RedshiftCredentials, ConnectionStringCredentials  # noqa: F401
 from .config_section_context import ConfigSectionContext  # noqa: F401
+
+from .gcp_credentials import GcpServiceAccountCredentialsWithoutDefaults, GcpServiceAccountCredentials, GcpOAuthCredentialsWithoutDefaults, GcpOAuthCredentials, GcpCredentials  # noqa: F401
+from .connection_string_credentials import ConnectionStringCredentials  # noqa: F401
+from .api_credentials import OAuth2Credentials  # noqa: F401
+
+
+# backward compatibility for service account credentials
+from .gcp_credentials import GcpServiceAccountCredentialsWithoutDefaults as GcpClientCredentials, GcpServiceAccountCredentials as GcpClientCredentialsWithDefault  # noqa: F401
```

### Comparing `dlt-0.2.6a1/dlt/common/configuration/specs/api_credentials.py` & `dlt-0.2.6a2/dlt/common/configuration/specs/api_credentials.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Union, Optional
+from typing import ClassVar, List, Union, Optional
 
 from dlt.common.typing import TSecretValue
 from dlt.common.configuration.specs.base_configuration import CredentialsConfiguration, configspec
 
 
 @configspec
 class OAuth2Credentials(CredentialsConfiguration):
@@ -10,14 +10,17 @@
     client_secret: TSecretValue
     refresh_token: Optional[TSecretValue]
     scopes: Optional[List[str]] = None
 
     token: Optional[TSecretValue] = None
     """Access token"""
 
+    # add refresh_token when generating config samples
+    __config_gen_annotations__: ClassVar[List[str]] = ["refresh_token"]
+
 
     def auth(self, scopes: Union[str, List[str]] = None, redirect_url: str = None) -> None:
         """Authorizes the client using the available credentials
 
         Uses the `refresh_token` grant if refresh token is available. Note that `scopes` and `redirect_url` are ignored in this flow.
         Otherwise obtains refresh_token via web flow and authorization code grant.
```

### Comparing `dlt-0.2.6a1/dlt/common/configuration/specs/base_configuration.py` & `dlt-0.2.6a2/dlt/common/configuration/specs/base_configuration.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import inspect
 import contextlib
 import dataclasses
+from collections.abc import Mapping as C_Mapping
 from typing import Callable, List, Optional, Union, Any, Dict, Iterator, MutableMapping, Type, TYPE_CHECKING, get_args, get_origin, overload, ClassVar
 
 if TYPE_CHECKING:
     TDtcField = dataclasses.Field[Any]
 else:
     TDtcField = dataclasses.Field
 
@@ -134,14 +135,16 @@
     """True when all config fields were resolved and have a specified value type"""
     __section__: str = dataclasses.field(default = None, init=False, repr=False)
     """Obligatory section used by config providers when searching for keys, always present in the search path"""
     __exception__: Exception = dataclasses.field(default = None, init=False, repr=False)
     """Holds the exception that prevented the full resolution"""
     __config_gen_annotations__: ClassVar[List[str]] = []
     """Additional annotations for config generator, currently holds a list of fields of interest that have defaults"""
+    __dataclass_fields__: ClassVar[Dict[str, TDtcField]]
+    """Typing for dataclass fields"""
 
     def parse_native_representation(self, native_value: Any) -> None:
         """Initialize the configuration fields by parsing the `native_value` which should be a native representation of the configuration
         or credentials, for example database connection string or JSON serialized GCP service credentials file.
 
         ### Args:
             native_value (Any): A native representation of the configuration
@@ -159,30 +162,35 @@
             NotImplementedError: This configuration does not have a native representation
 
         Returns:
             Any: A native representation of the configuration
         """
         raise NotImplementedError()
 
-    def get_resolvable_fields(self) -> Dict[str, type]:
-        """Returns a mapping of fields to their type hints. Dunder should not be resolved and are not returned"""
-        return {f.name:f.type for f in self.__fields_dict().values() if not f.name.startswith("__")}
+    @classmethod
+    def get_resolvable_fields(cls) -> Dict[str, type]:
+        """Returns a mapping of fields to their type hints. Dunders should not be resolved and are not returned"""
+        return {f.name:f.type for f in cls.__dataclass_fields__.values() if not f.name.startswith("__")}
 
     def is_resolved(self) -> bool:
         return self.__is_resolved__
 
     def is_partial(self) -> bool:
         """Returns True when any required resolvable field has its value missing."""
         if self.__is_resolved__:
             return False
         # check if all resolvable fields have value
         return any(
             field for field, hint in self.get_resolvable_fields().items() if getattr(self, field) is None and not is_optional_type(hint)
         )
 
+    def resolve(self) -> None:
+        self.call_method_in_mro("on_resolved")
+        self.__is_resolved__ = True
+
     # implement dictionary-compatible interface on top of dataclass
 
     def __getitem__(self, __key: str) -> Any:
         if self.__has_attr(__key):
             return getattr(self, __key)
         else:
             raise KeyError(__key)
@@ -199,44 +207,79 @@
                 # __ignore_set_unknown_keys attribute may not be present at the moment of checking, __init__ of BaseConfiguration is not typically called
                 raise KeyError(__key)
 
     def __delitem__(self, __key: str) -> None:
         raise KeyError("Configuration fields cannot be deleted")
 
     def __iter__(self) -> Iterator[str]:
-        return filter(lambda k: not k.startswith("__"), self.__fields_dict().__iter__())
+        return filter(lambda k: not k.startswith("__"), self.__dataclass_fields__.__iter__())
 
     def __len__(self) -> int:
         return sum(1 for _ in self.__iter__())
 
     def update(self, other: Any = (), /, **kwds: Any) -> None:
         try:
             self.__ignore_set_unknown_keys = True
             super().update(other, **kwds)
         finally:
             self.__ignore_set_unknown_keys = False
 
     # helper functions
 
     def __has_attr(self, __key: str) -> bool:
-        return __key in self.__fields_dict() and not __key.startswith("__")
+        return __key in self.__dataclass_fields__ and not __key.startswith("__")
 
-    def __fields_dict(self) -> Dict[str, TDtcField]:
-        return self.__dataclass_fields__  # type: ignore
+    def call_method_in_mro(config, method_name: str) -> None:
+        # python multi-inheritance is cooperative and this would require that all configurations cooperatively
+        # call each other class_method_name. this is not at all possible as we do not know which configs in the end will
+        # be mixed together.
+
+        # get base classes in order of derivation
+        mro = type.mro(type(config))
+        for c in mro:
+            # check if this class implements on_resolved (skip pure inheritance to not do double work)
+            if method_name in c.__dict__ and callable(getattr(c, method_name)):
+                # pass right class instance
+                c.__dict__[method_name](config)
 
 
 _F_BaseConfiguration = BaseConfiguration
 
 
 @configspec
 class CredentialsConfiguration(BaseConfiguration):
     """Base class for all credentials. Credentials are configurations that may be stored only by providers supporting secrets."""
 
     __section__: str = "credentials"
 
+    def __init__(self, init_value: Any = None) -> None:
+        """Initializes credentials from `init_value`
+
+        Init value may be a native representation of the credentials or a dict. In case of native representation (for example a connection string or JSON with service account credentials)
+        a `parse_native_representation` method will be used to parse it. In case of a dict, the credentials object will be updated with key: values of the dict.
+        Unexpected values in the dict will be ignored.
+
+        Credentials will be marked as resolved if all required fields are set.
+        """
+        if init_value is None:
+            return
+        elif isinstance(init_value, C_Mapping):
+            self.update(init_value)
+        else:
+            self.parse_native_representation(init_value)
+        if not self.is_partial():
+            self.resolve()
+
+    def to_native_credentials(self) -> Any:
+        """Returns native credentials object.
+
+        By default calls `to_native_representation` method.
+        """
+        return self.to_native_representation()
+
     def __str__(self) -> str:
         """Get string representation of credentials to be displayed, with all secret parts removed """
         return super().__str__()
 
 
 class CredentialsWithDefault:
     """A mixin for credentials that can be instantiated from default ie. from well known env variable with credentials"""
@@ -256,9 +299,13 @@
 @configspec
 class ContainerInjectableContext(BaseConfiguration):
     """Base class for all configurations that may be injected from a Container. Injectable configuration is called a context"""
 
     can_create_default: ClassVar[bool] = True
     """If True, `Container` is allowed to create default context instance, if none exists"""
 
+    def add_extras(self) -> None:
+        """Called right after context was added to the container. Benefits mostly the config provider injection context which adds extra providers using the initial ones."""
+        pass
+
 
 _F_ContainerInjectableContext = ContainerInjectableContext
```

### Comparing `dlt-0.2.6a1/dlt/common/configuration/specs/config_providers_context.py` & `dlt-0.2.6a2/dlt/common/configuration/specs/config_providers_context.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,44 @@
 
 
 from typing import List
 from dlt.common.configuration.exceptions import DuplicateConfigProviderException
-from dlt.common.configuration.providers import ConfigProvider, EnvironProvider, ContextProvider, SecretsTomlProvider, ConfigTomlProvider
-from dlt.common.configuration.specs.base_configuration import ContainerInjectableContext, configspec
+from dlt.common.configuration.providers import ConfigProvider, EnvironProvider, ContextProvider, SecretsTomlProvider, ConfigTomlProvider, GoogleSecretsProvider
+from dlt.common.configuration.specs.base_configuration import ContainerInjectableContext
+from dlt.common.configuration.specs import GcpServiceAccountCredentials, BaseConfiguration, configspec, known_sections
 from dlt.common.runtime.exec_info import is_running_in_airflow_task
 
 
 @configspec
+class ConfigProvidersConfiguration(BaseConfiguration):
+    enable_airflow_secrets: bool = True
+    enable_google_secrets: bool = False
+    only_toml_fragments: bool = True
+
+    # always look in providers
+    __section__ = known_sections.PROVIDERS
+
+
+@configspec
 class ConfigProvidersContext(ContainerInjectableContext):
     """Injectable list of providers used by the configuration `resolve` module"""
     providers: List[ConfigProvider]
     context_provider: ConfigProvider
 
     def __init__(self) -> None:
         super().__init__()
         # add default providers
         self.providers = ConfigProvidersContext.initial_providers()
         # ContextProvider will provide contexts when embedded in configurations
         self.context_provider = ContextProvider()
 
+    def add_extras(self) -> None:
+        """Adds extra providers using the initial ones."""
+        self.providers += _extra_providers()
+
     def __getitem__(self, name: str) -> ConfigProvider:
         try:
             return next(p for p in self.providers if p.name == name)
         except StopIteration:
             raise KeyError(name)
 
     def __contains__(self, name: object) -> bool:
@@ -41,34 +56,47 @@
     @staticmethod
     def initial_providers() -> List[ConfigProvider]:
         providers = [
             EnvironProvider(),
             SecretsTomlProvider(add_global_config=True),
             ConfigTomlProvider(add_global_config=True)
         ]
-        providers += _extra_providers()
         return providers
 
 
 def _extra_providers() -> List[ConfigProvider]:
-    return _airflow_providers()
+    from dlt.common.configuration.resolve import resolve_configuration
+    providers_config = resolve_configuration(ConfigProvidersConfiguration())
+    extra_providers = []
+    if providers_config.enable_airflow_secrets:
+        extra_providers.extend(_airflow_providers())
+    if providers_config.enable_google_secrets:
+        extra_providers.append(_google_secrets_provider(only_toml_fragments=providers_config.only_toml_fragments))
+    return extra_providers
+
+
+def _google_secrets_provider(only_secrets: bool = True, only_toml_fragments: bool = True) -> ConfigProvider:
+    from dlt.common.configuration.resolve import resolve_configuration
+
+    c = resolve_configuration(GcpServiceAccountCredentials(), sections=(known_sections.PROVIDERS, "google_secrets"))
+    return GoogleSecretsProvider(c, only_secrets=only_secrets, only_toml_fragments=only_toml_fragments)
 
 
 def _airflow_providers() -> List[ConfigProvider]:
     """Returns a list of configuration providers for an Airflow environment.
 
     This function attempts to import Airflow to determine whether it
     is running in an Airflow environment. If Airflow is not installed,
     an empty list is returned. If Airflow is installed, the function
     returns a list containing the Airflow providers.
     """
     if not is_running_in_airflow_task():
         return []
 
-    from airflow.models import Variable, TaskInstance # noqa
+    from airflow.models import Variable # noqa
     from airflow.operators.python import get_current_context  # noqa
 
     from dlt.common.configuration.providers.airflow import (
         AirflowSecretsTomlProvider,
         AIRFLOW_SECRETS_TOML_VARIABLE_KEY
     )
 
@@ -82,14 +110,7 @@
     else:
         ti = get_current_context()["ti"]
         ti.log.warning(
             f"Airflow variable '{AIRFLOW_SECRETS_TOML_VARIABLE_KEY}' "
             "not found. AirflowSecretsTomlProvider will not be used."
         )
         return []
-
-
-# TODO: implement ConfigProvidersConfiguration and
-# @configspec
-# class ConfigProvidersConfiguration(BaseConfiguration):
-#     with_aws_secrets: bool = False
-#     with_google_secrets: bool = False
```

### Comparing `dlt-0.2.6a1/dlt/common/configuration/specs/config_section_context.py` & `dlt-0.2.6a2/dlt/common/configuration/specs/config_section_context.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/common/configuration/specs/exceptions.py` & `dlt-0.2.6a2/dlt/common/configuration/specs/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/common/configuration/specs/gcp_client_credentials.py` & `dlt-0.2.6a2/dlt/common/configuration/specs/gcp_credentials.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import sys
 from typing import Any, ClassVar, Final, List, Tuple, Union
 from deprecated import deprecated
 
-from dlt.common import json
+from dlt.common import json, pendulum
 from dlt.common.configuration.specs.api_credentials import OAuth2Credentials
 from dlt.common.configuration.specs.exceptions import InvalidGoogleNativeCredentialsType, InvalidGoogleOauth2Json, InvalidGoogleServicesJson, NativeValueError, OAuth2ScopesRequired
 from dlt.common.exceptions import MissingDependencyException
 from dlt.common.typing import DictStrAny, TSecretValue, StrAny
 from dlt.common.configuration.specs.base_configuration import CredentialsConfiguration, CredentialsWithDefault, configspec
 from dlt.common.utils import is_interactive
 
 
 @configspec
-class GcpCredentialsBase(CredentialsConfiguration):
+class GcpCredentials(CredentialsConfiguration):
     token_uri: Final[str] = "https://oauth2.googleapis.com/token"
     auth_uri: Final[str] = "https://accounts.google.com/o/oauth2/auth"
 
     project_id: str = None
     location: str = "US"
 
     http_timeout: float = 15.0
@@ -28,73 +28,27 @@
     def parse_native_representation(self, native_value: Any) -> None:
         if not isinstance(native_value, str):
             raise InvalidGoogleNativeCredentialsType(self.__class__, native_value)
 
     def to_native_representation(self) -> str:
         return json.dumps(dict(self))
 
-    def to_google_credentials(self) -> Any:
+    def to_native_credentials(self) -> Any:
+        """Returns respective native credentials for service account or oauth2 that can be passed to google clients"""
         pass
 
     def _from_info_dict(self, info: StrAny) -> None:
         self.update(info)
-        # self.__is_resolved__ = not self.is_partial()
 
     def __str__(self) -> str:
         return f"{self.project_id}[{self.location}]"
 
 
 @configspec
-class GcpDefaultCredentials(CredentialsWithDefault, GcpCredentialsBase):
-
-    def parse_native_representation(self, native_value: Any) -> None:
-        """Accepts google credentials as native value"""
-        try:
-            from google.auth.credentials import Credentials as GoogleCredentials
-            if isinstance(native_value, GoogleCredentials):
-                self.project_id = self.project_id or native_value.quota_project_id
-                self._set_default_credentials(native_value)
-                # is resolved
-                self.__is_resolved__ = True
-                return
-        except ImportError:
-            pass
-        raise NativeValueError(self.__class__, native_value, "Default Google Credentials not present")
-
-    def on_partial(self) -> None:
-        """Looks for default google credentials and resolves configuration if found. Otherwise continues as partial"""
-        try:
-            from google.auth import default as default_credentials
-            from google.auth.exceptions import DefaultCredentialsError
-
-            # if config is missing check if credentials can be obtained from defaults
-            try:
-                default, project_id = default_credentials()
-                # set the project id - it needs to be known by the client
-                self.project_id = self.project_id or project_id or default.quota_project_id
-                self._set_default_credentials(default)
-                # is resolved
-                self.__is_resolved__ = True
-            except DefaultCredentialsError:
-                # re-raise preventing exception
-                pass
-
-        except ImportError:
-            # raise the exception that caused partial (typically missing config fields)
-            pass
-
-    def to_google_credentials(self) -> Any:
-        if self.has_default_credentials():
-            return self.default_credentials()
-        else:
-            return super().to_google_credentials()
-
-
-@configspec
-class GcpClientCredentials(GcpCredentialsBase):
+class GcpServiceAccountCredentialsWithoutDefaults(GcpCredentials):
     private_key: TSecretValue = None
     client_email: str = None
     type: Final[str] = "service_account"  # noqa: A003
 
     def parse_native_representation(self, native_value: Any) -> None:
         """Accepts ServiceAccountCredentials as native value. In other case reverts to serialized services.json"""
         service_dict: DictStrAny = None
@@ -109,56 +63,48 @@
                 }
                 self.__is_resolved__ = True
         except ImportError:
             pass
 
         if service_dict is None:
             # check if type is str
-            GcpCredentialsBase.parse_native_representation(self, native_value)
+            GcpCredentials.parse_native_representation(self, native_value)
             # if not instance of service account credentials then check type and try to parse native value
             try:
                 service_dict = json.loads(native_value)
             except Exception:
                 raise InvalidGoogleServicesJson(self.__class__, native_value)
 
         self._from_info_dict(service_dict)
 
     def on_resolved(self) -> None:
         if self.private_key and self.private_key[-1] != "\n":
             # must end with new line, otherwise won't be parsed by Crypto
             self.private_key = TSecretValue(self.private_key + "\n")
 
-    @deprecated(reason="Use 'to_google_credentials' method instead")
+    @deprecated(reason="Use 'to_native_credentials' method instead")
     def to_service_account_credentials(self) -> Any:
-        return self.to_google_credentials()
+        return self.to_native_credentials()
+
+    def to_native_credentials(self) -> Any:
+        """Returns google.oauth2.service_account.Credentials"""
 
-    def to_google_credentials(self) -> Any:
         from google.oauth2.service_account import Credentials as ServiceAccountCredentials
         if isinstance(self.private_key, ServiceAccountCredentials):
             # private key holds the native instance if it was passed to parse_native_representation
             return self.private_key
         else:
             return ServiceAccountCredentials.from_service_account_info(self)
 
     def __str__(self) -> str:
         return f"{self.client_email}@{self.project_id}[{self.location}]"
 
 
 @configspec
-class GcpClientCredentialsWithDefault(GcpDefaultCredentials, GcpClientCredentials):
-    def parse_native_representation(self, native_value: Any) -> None:
-        try:
-            GcpDefaultCredentials.parse_native_representation(self, native_value)
-        except NativeValueError:
-            pass
-        GcpClientCredentials.parse_native_representation(self, native_value)
-
-
-@configspec
-class GcpOAuthCredentials(GcpCredentialsBase, OAuth2Credentials):
+class GcpOAuthCredentialsWithoutDefaults(GcpCredentials, OAuth2Credentials):
     # only desktop app supported
     refresh_token: TSecretValue
     client_type: Final[str] = "installed"
 
     def parse_native_representation(self, native_value: Any) -> None:
         """Accepts Google OAuth2 credentials as native value. In other case reverts to serialized oauth client secret json"""
         oauth_dict: DictStrAny = None
@@ -177,15 +123,15 @@
                 # if token is present, we are logged in
                 self.__is_resolved__ = native_value.token is not None
         except ImportError:
             pass
 
         if oauth_dict is None:
             # check if type is str
-            GcpCredentialsBase.parse_native_representation(self, native_value)
+            GcpCredentials.parse_native_representation(self, native_value)
             # if not instance of oauth2 credentials try to parse native value
             try:
                 oauth_dict = json.loads(native_value)
                 # if there's single element in the dict, this is probably "installed" or "web" etc. (app type)
                 if len(oauth_dict) == 1:
                     oauth_dict = next(iter(oauth_dict.values()))
             except Exception:
@@ -209,15 +155,15 @@
 
     def on_partial(self) -> None:
         """Allows for an empty refresh token if the session is interactive or tty is attached"""
         if sys.stdin.isatty() or is_interactive():
             self.refresh_token = TSecretValue("")
             # still partial - raise
             if not self.is_partial():
-                self.__is_resolved__ = True
+                self.resolve()
             self.refresh_token = None
 
     def _get_access_token(self) -> TSecretValue:
         try:
             from requests_oauthlib import OAuth2Session
         except ImportError:
             raise MissingDependencyException("GcpOAuthCredentials", ["requests_oauthlib"])
@@ -235,19 +181,16 @@
             from google_auth_oauthlib.flow import InstalledAppFlow
         except ImportError:
             raise MissingDependencyException("GcpOAuthCredentials", ["google-auth-oauthlib"])
         flow = InstalledAppFlow.from_client_config(self._installed_dict(redirect_url), self.scopes)
         credentials = flow.run_local_server(port=0)
         return TSecretValue(credentials.refresh_token), TSecretValue(credentials.token)
 
-    def to_google_credentials(self) -> Any:
-        """
-        Will convert the object to a Google oauth2 credentials object
-        :returns: Google Credentials object
-        """
+    def to_native_credentials(self) -> Any:
+        """Returns google.oauth2.credentials.Credentials"""
         try:
             from google.oauth2.credentials import Credentials as GoogleOAuth2Credentials
         except ImportError:
             raise MissingDependencyException("GcpOAuthCredentials", ["google-auth-oauthlib"])
 
         credentials = GoogleOAuth2Credentials.from_authorized_user_info(info=dict(self))
         return credentials
@@ -268,14 +211,82 @@
         return info_dict
 
     def __str__(self) -> str:
         return f"{self.client_id}@{self.project_id}[{self.location}]"
 
 
 @configspec
-class GcpOAuthCredentialsWithDefault(GcpDefaultCredentials, GcpOAuthCredentials):
+class GcpDefaultCredentials(CredentialsWithDefault, GcpCredentials):
+
+    _LAST_FAILED_DEFAULT: float = 0.0
+
+    def parse_native_representation(self, native_value: Any) -> None:
+        """Accepts google credentials as native value"""
+        try:
+            from google.auth.credentials import Credentials as GoogleCredentials
+            if isinstance(native_value, GoogleCredentials):
+                self.project_id = self.project_id or native_value.quota_project_id
+                self._set_default_credentials(native_value)
+                # is resolved
+                self.__is_resolved__ = True
+                return
+        except ImportError:
+            pass
+        raise NativeValueError(self.__class__, native_value, "Default Google Credentials not present")
+
+    @staticmethod
+    def _get_default_credentials(retry_timeout_s: float = 600.0) -> Tuple[Any, str]:
+
+        now = pendulum.now().timestamp()
+        if now - GcpDefaultCredentials._LAST_FAILED_DEFAULT < retry_timeout_s:
+            return None, None
+
+        from google.auth import default as default_credentials
+        from google.auth.exceptions import DefaultCredentialsError
+
+        try:
+            return default_credentials()  # type: ignore
+        except DefaultCredentialsError:
+            # prevent exception
+            GcpDefaultCredentials._LAST_FAILED_DEFAULT = now
+            return None, None
+
+    def on_partial(self) -> None:
+        """Looks for default google credentials and resolves configuration if found. Otherwise continues as partial"""
+        try:
+            # if config is missing check if credentials can be obtained from defaults
+            default, project_id = GcpDefaultCredentials._get_default_credentials()
+            if default is None:
+                return
+            # set the project id - it needs to be known by the client
+            self.project_id = self.project_id or project_id or default.quota_project_id
+            self._set_default_credentials(default)
+            self.resolve()
+        except ImportError:
+            # raise the exception that caused partial (typically missing config fields)
+            pass
+
+    def to_native_credentials(self) -> Any:
+        if self.has_default_credentials():
+            return self.default_credentials()
+        else:
+            return super().to_native_credentials()
+
+
+@configspec
+class GcpServiceAccountCredentials(GcpDefaultCredentials, GcpServiceAccountCredentialsWithoutDefaults):
+    def parse_native_representation(self, native_value: Any) -> None:
+        try:
+            GcpDefaultCredentials.parse_native_representation(self, native_value)
+        except NativeValueError:
+            pass
+        GcpServiceAccountCredentialsWithoutDefaults.parse_native_representation(self, native_value)
+
+
+@configspec
+class GcpOAuthCredentials(GcpDefaultCredentials, GcpOAuthCredentialsWithoutDefaults):
     def parse_native_representation(self, native_value: Any) -> None:
         try:
             GcpDefaultCredentials.parse_native_representation(self, native_value)
         except NativeValueError:
             pass
-        GcpOAuthCredentials.parse_native_representation(self, native_value)
+        GcpOAuthCredentialsWithoutDefaults.parse_native_representation(self, native_value)
```

### Comparing `dlt-0.2.6a1/dlt/common/configuration/specs/known_sections.py` & `dlt-0.2.6a2/dlt/common/configuration/specs/known_sections.py`

 * *Files 23% similar despite different names*

```diff
@@ -9,12 +9,15 @@
 
 NORMALIZE = "normalize"
 """normalize and normalize storage configuration"""
 
 EXTRACT = "extract"
 """extract stage of the pipeline"""
 
+PROVIDERS = "providers"
+"""secrets and config providers"""
+
 DATA_WRITER = "data_writer"
 """default section holding BufferedDataWriter settings"""
 
 DBT_PACKAGE_RUNNER =  "dbt_package_runner"
 """dbt package runner configuration (DBTRunnerConfiguration)"""
```

### Comparing `dlt-0.2.6a1/dlt/common/configuration/specs/load_volume_configuration.py` & `dlt-0.2.6a2/dlt/common/configuration/specs/load_volume_configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/common/configuration/specs/postgres_credentials.py` & `dlt-0.2.6a2/dlt/common/configuration/specs/connection_string_credentials.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, ClassVar, Dict, Final, List, Optional
+from typing import Any, ClassVar, Dict, List, Optional
 from sqlalchemy.engine import URL, make_url
 from dlt.common.configuration.specs.exceptions import InvalidConnectionString
 
 from dlt.common.typing import TSecretValue
 from dlt.common.configuration.specs.base_configuration import CredentialsConfiguration, configspec
 
 
@@ -25,15 +25,14 @@
             url = make_url(native_value)
             # update only values that are not None
             self.update(
                 {k: v for k,v in url._asdict().items() if v is not None}
             )
             if self.query is not None:
                 self.query = dict(self.query)
-            # self.__is_resolved__ = not self.is_partial()
         except Exception:
             raise InvalidConnectionString(self.__class__, native_value, self.drivername)
 
     def on_resolved(self) -> None:
         if self.password:
             self.password = TSecretValue(self.password.strip())
 
@@ -41,38 +40,7 @@
         return self.to_url().render_as_string(hide_password=False)
 
     def to_url(self) -> URL:
         return URL.create(self.drivername, self.username, self.password, self.host, self.port, self.database, self.query)
 
     def __str__(self) -> str:
         return self.to_url().render_as_string(hide_password=True)
-
-
-@configspec
-class PostgresCredentials(ConnectionStringCredentials):
-    drivername: Final[str] = "postgresql"  # type: ignore
-    port: int = 5432
-    connect_timeout: int = 15
-
-    __config_gen_annotations__: ClassVar[List[str]] = ["port", "connect_timeout"]
-
-    def parse_native_representation(self, native_value: Any) -> None:
-        super().parse_native_representation(native_value)
-        self.connect_timeout = int(self.query.get("connect_timeout", self.connect_timeout))
-
-    def on_resolved(self) -> None:
-        self.database = self.database.lower()
-        if self.password:
-            self.password = TSecretValue(self.password.strip())
-
-    def to_url(self) -> URL:
-        url = super().to_url()
-        url.update_query_pairs([("connect_timeout", str(self.connect_timeout))])
-        return url
-
-
-@configspec
-class RedshiftCredentials(PostgresCredentials):
-    port: int = 5439
-    password: TSecretValue = None
-    username: str = None
-    host: str = None
```

### Comparing `dlt-0.2.6a1/dlt/common/configuration/specs/run_configuration.py` & `dlt-0.2.6a2/dlt/common/configuration/specs/run_configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/common/configuration/specs/schema_volume_configuration.py` & `dlt-0.2.6a2/dlt/common/configuration/specs/schema_volume_configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/common/configuration/utils.py` & `dlt-0.2.6a2/dlt/common/configuration/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 import ast
 import contextlib
+import tomlkit
 from typing import Any, Dict, Mapping, NamedTuple, Optional, Type, Sequence
 
 from dlt.common import json
 from dlt.common.typing import AnyType, TAny
 from dlt.common.data_types import coerce_value, py_type_to_sc_type
 from dlt.common.configuration.providers import EnvironProvider
 from dlt.common.configuration.exceptions import ConfigValueCannotBeCoercedException, LookupTrace
@@ -85,14 +86,35 @@
             # no native representation: use dict
             value = dict(value)
     # coerce type to text which will use json for mapping and sequences
     value_dt = py_type_to_sc_type(type(value))
     return coerce_value("text", value_dt, value)
 
 
+def auto_cast(value: str) -> Any:
+    # try to cast to bool, int, float and complex (via JSON)
+    if value.lower() == "true":
+        return True
+    if value.lower() == "false":
+        return False
+    with contextlib.suppress(ValueError):
+        return coerce_value("bigint", "text", value)
+    with contextlib.suppress(ValueError):
+        return coerce_value("double", "text", value)
+    with contextlib.suppress(ValueError):
+        c_v = json.loads(value)
+        # only lists and dictionaries count
+        if isinstance(c_v, (list, dict)):
+            return c_v
+    with contextlib.suppress(ValueError):
+        return tomlkit.parse(value)
+    return value
+
+
+
 def log_traces(config: Optional[BaseConfiguration], key: str, hint: Type[Any], value: Any, default_value: Any, traces: Sequence[LookupTrace]) -> None:
     from dlt.common import logger
 
     if logger.is_logging() and logger.log_level() == "DEBUG" and config:
         logger.debug(f"Field {key} with type {hint} in {type(config).__name__} {'NOT RESOLVED' if value is None else 'RESOLVED'}")
         # print(f"Field {key} with type {hint} in {type(config).__name__} {'NOT RESOLVED' if value is None else 'RESOLVED'}")
         for tr in traces:
```

### Comparing `dlt-0.2.6a1/dlt/common/data_types/type_helpers.py` & `dlt-0.2.6a2/dlt/common/data_types/type_helpers.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/common/data_writers/buffered.py` & `dlt-0.2.6a2/dlt/common/data_writers/buffered.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/common/data_writers/escape.py` & `dlt-0.2.6a2/dlt/common/data_writers/escape.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/common/data_writers/exceptions.py` & `dlt-0.2.6a2/dlt/common/data_writers/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/common/data_writers/writers.py` & `dlt-0.2.6a2/dlt/common/data_writers/writers.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/common/destination/capabilities.py` & `dlt-0.2.6a2/dlt/common/destination/capabilities.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/common/destination/reference.py` & `dlt-0.2.6a2/dlt/common/destination/reference.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/common/exceptions.py` & `dlt-0.2.6a2/dlt/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/common/git.py` & `dlt-0.2.6a2/dlt/common/git.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/common/json/__init__.py` & `dlt-0.2.6a2/dlt/common/json/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/common/json/_orjson.py` & `dlt-0.2.6a2/dlt/common/json/_orjson.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/common/json/_simplejson.py` & `dlt-0.2.6a2/dlt/common/json/_simplejson.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/common/jsonpath.py` & `dlt-0.2.6a2/dlt/common/jsonpath.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/common/normalizers/configuration.py` & `dlt-0.2.6a2/dlt/common/normalizers/configuration.py`

 * *Files 20% similar despite different names*

```diff
@@ -20,14 +20,14 @@
     def on_partial(self) -> None:
         if self.naming is None:
             if self.destination_capabilities:
                 self.naming = self.destination_capabilities.naming_convention
             else:
                 self.naming = "snake_case"
             # is resolved
-            self.__is_resolved__ = True
+            self.resolve()
         else:
             raise self.__exception__
 
     if TYPE_CHECKING:
         def __init__(self, naming: str = None, json_normalizer: TJSONNormalizer = None) -> None:
             ...
```

### Comparing `dlt-0.2.6a1/dlt/common/normalizers/json/__init__.py` & `dlt-0.2.6a2/dlt/common/normalizers/json/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/common/normalizers/json/relational.py` & `dlt-0.2.6a2/dlt/common/normalizers/json/relational.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/common/normalizers/naming/direct.py` & `dlt-0.2.6a2/dlt/common/normalizers/naming/direct.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/common/normalizers/naming/duck_case.py` & `dlt-0.2.6a2/dlt/common/normalizers/naming/duck_case.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/common/normalizers/naming/exceptions.py` & `dlt-0.2.6a2/dlt/common/normalizers/naming/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/common/normalizers/naming/naming.py` & `dlt-0.2.6a2/dlt/common/normalizers/naming/naming.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/common/normalizers/naming/snake_case.py` & `dlt-0.2.6a2/dlt/common/normalizers/naming/snake_case.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/common/normalizers/utils.py` & `dlt-0.2.6a2/dlt/common/normalizers/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/common/pipeline.py` & `dlt-0.2.6a2/dlt/common/pipeline.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/common/reflection/spec.py` & `dlt-0.2.6a2/dlt/common/reflection/spec.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/common/reflection/utils.py` & `dlt-0.2.6a2/dlt/common/reflection/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/common/runners/pool_runner.py` & `dlt-0.2.6a2/dlt/common/runners/pool_runner.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/common/runners/runnable.py` & `dlt-0.2.6a2/dlt/common/runners/runnable.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/common/runners/stdout.py` & `dlt-0.2.6a2/dlt/common/runners/stdout.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/common/runners/synth_pickle.py` & `dlt-0.2.6a2/dlt/common/runners/synth_pickle.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/common/runners/venv.py` & `dlt-0.2.6a2/dlt/common/runners/venv.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import sys
 import os
 import shutil
 import venv
 import types
 import subprocess
 from typing import Any, List, Type
 
@@ -115,7 +116,17 @@
     def _install_deps(context: types.SimpleNamespace, dependencies: List[str]) -> None:
         for dep in dependencies:
             cmd = [context.env_exe, "-Im", "pip", "install", dep]
             try:
                 subprocess.check_output(cmd, stderr=subprocess.STDOUT)
             except subprocess.CalledProcessError as exc:
                 raise CannotInstallDependency(dep, context.env_exe, exc.output)
+
+    @staticmethod
+    def is_virtual_env() -> bool:
+        """Checks if we are running in virtual environment"""
+        return "VIRTUAL_ENV" in os.environ
+
+    @staticmethod
+    def is_venv_activated() -> bool:
+        """Checks if virtual environment is activated in the shell"""
+        return sys.prefix != sys.base_prefix
```

### Comparing `dlt-0.2.6a1/dlt/common/runtime/collector.py` & `dlt-0.2.6a2/dlt/common/runtime/collector.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/common/runtime/exec_info.py` & `dlt-0.2.6a2/dlt/common/runtime/exec_info.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/common/runtime/init.py` & `dlt-0.2.6a2/dlt/common/runtime/init.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/common/runtime/logger.py` & `dlt-0.2.6a2/dlt/common/runtime/logger.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/common/runtime/prometheus.py` & `dlt-0.2.6a2/dlt/common/runtime/prometheus.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/common/runtime/segment.py` & `dlt-0.2.6a2/dlt/common/runtime/segment.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/common/runtime/sentry.py` & `dlt-0.2.6a2/dlt/common/runtime/sentry.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/common/runtime/signals.py` & `dlt-0.2.6a2/dlt/common/runtime/signals.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/common/runtime/slack.py` & `dlt-0.2.6a2/dlt/common/runtime/slack.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/common/runtime/telemetry.py` & `dlt-0.2.6a2/dlt/common/runtime/telemetry.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/common/schema/detections.py` & `dlt-0.2.6a2/dlt/common/schema/detections.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/common/schema/exceptions.py` & `dlt-0.2.6a2/dlt/common/schema/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/common/schema/schema.py` & `dlt-0.2.6a2/dlt/common/schema/schema.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/common/schema/typing.py` & `dlt-0.2.6a2/dlt/common/schema/typing.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/common/schema/utils.py` & `dlt-0.2.6a2/dlt/common/schema/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/common/storages/data_item_storage.py` & `dlt-0.2.6a2/dlt/common/storages/data_item_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/common/storages/exceptions.py` & `dlt-0.2.6a2/dlt/common/storages/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/common/storages/file_storage.py` & `dlt-0.2.6a2/dlt/common/storages/file_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/common/storages/live_schema_storage.py` & `dlt-0.2.6a2/dlt/common/storages/live_schema_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/common/storages/load_storage.py` & `dlt-0.2.6a2/dlt/common/storages/load_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/common/storages/normalize_storage.py` & `dlt-0.2.6a2/dlt/common/storages/normalize_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/common/storages/schema_storage.py` & `dlt-0.2.6a2/dlt/common/storages/schema_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/common/storages/versioned_storage.py` & `dlt-0.2.6a2/dlt/common/storages/versioned_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/common/time.py` & `dlt-0.2.6a2/dlt/common/time.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,18 +22,17 @@
 def timestamp_before(timestamp: float, max_inclusive: Optional[float]) -> bool:
     """
     check if timestamp is before max timestamp, inclusive
     """
     return timestamp <= (max_inclusive or FUTURE_TIMESTAMP)
 
 
-def parse_iso_like_datetime(value: Any) -> datetime.datetime:
-    # we use internal pendulum parse function. the generic function for example parses string "now" as now()
+def parse_iso_like_datetime(value: Any) -> pendulum.DateTime:
+    # we use internal pendulum parse function. the generic function, for example, parses string "now" as now()
     # it also tries to parse ISO intervals but the code is very low quality
-    # so it does not seem to be under control
 
     # only iso dates are allowed
     dtv = None
     with contextlib.suppress(ValueError):
         dtv = parse_iso8601(value)
     # now try to parse a set of ISO like dates
     if not dtv:
@@ -61,14 +60,15 @@
     """
     if isinstance(value, datetime.datetime):
         return value
     return pendulum.datetime(
         value.year, value.month, value.day, tz=UTC
     )
 
+
 def ensure_date(value: Union[datetime.datetime, datetime.date]) -> datetime.date:
     if isinstance(value, datetime.datetime):
         return value.date()
     return value
 
 
 @overload
```

### Comparing `dlt-0.2.6a1/dlt/common/typing.py` & `dlt-0.2.6a2/dlt/common/typing.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/common/utils.py` & `dlt-0.2.6a2/dlt/common/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/common/validation.py` & `dlt-0.2.6a2/dlt/common/validation.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/common/wei.py` & `dlt-0.2.6a2/dlt/common/wei.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/destinations/bigquery/__init__.py` & `dlt-0.2.6a2/dlt/destinations/bigquery/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/destinations/bigquery/bigquery.py` & `dlt-0.2.6a2/dlt/destinations/bigquery/bigquery.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import ClassVar, Dict, Optional, Sequence, Tuple, List, cast
 import google.cloud.bigquery as bigquery  # noqa: I250
 from google.cloud import exceptions as gcp_exceptions
 from google.api_core import exceptions as api_core_exceptions
 
 from dlt.common import json, logger
 from dlt.common.arithmetics import DEFAULT_NUMERIC_PRECISION, DEFAULT_NUMERIC_SCALE
-from dlt.common.configuration.specs import GcpClientCredentials
+from dlt.common.configuration.specs import GcpServiceAccountCredentialsWithoutDefaults
 from dlt.common.destination import DestinationCapabilitiesContext
 from dlt.common.destination.reference import FollowupJob, NewLoadJob, TLoadJobState, LoadJob
 from dlt.common.data_types import TDataType
 from dlt.common.storages.file_storage import FileStorage
 from dlt.common.schema import TColumnSchema, Schema, TTableSchemaColumns
 from dlt.common.schema.typing import TTableSchema, TWriteDisposition
 
@@ -46,15 +46,15 @@
     "BYTES": "binary",
     "NUMERIC": "decimal",
     "BIGNUMERIC": "decimal",
     "JSON": "complex"
 }
 
 class BigQueryLoadJob(LoadJob, FollowupJob):
-    def __init__(self, file_name: str, bq_load_job: bigquery.LoadJob, credentials: GcpClientCredentials) -> None:
+    def __init__(self, file_name: str, bq_load_job: bigquery.LoadJob, credentials: GcpServiceAccountCredentialsWithoutDefaults) -> None:
         self.bq_load_job = bq_load_job
         self.credentials = credentials
         self.default_retry = bigquery.DEFAULT_RETRY.with_deadline(credentials.retry_deadline)
         super().__init__(file_name)
 
     def state(self) -> TLoadJobState:
         # check server if done
```

### Comparing `dlt-0.2.6a1/dlt/destinations/bigquery/sql_client.py` & `dlt-0.2.6a2/dlt/destinations/bigquery/sql_client.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import google.cloud.bigquery as bigquery  # noqa: I250
 from google.cloud.bigquery import dbapi as bq_dbapi
 from google.cloud.bigquery.dbapi import Connection as DbApiConnection, Cursor as BQDbApiCursor
 from google.cloud import exceptions as gcp_exceptions
 from google.cloud.bigquery.dbapi import exceptions as dbapi_exceptions
 from google.api_core import exceptions as api_core_exceptions
 
-from dlt.common.configuration.specs import GcpClientCredentials
+from dlt.common.configuration.specs import GcpServiceAccountCredentialsWithoutDefaults
 from dlt.common.destination import DestinationCapabilitiesContext
 from dlt.common.typing import StrAny
 
 from dlt.destinations.typing import DBApi, DBApiCursor, DBTransaction, DataFrame
 from dlt.destinations.exceptions import DatabaseTerminalException, DatabaseTransientException, DatabaseUndefinedRelation
 from dlt.destinations.sql_client import DBApiCursorImpl, SqlClientBase, raise_database_error, raise_open_connection_error
 
@@ -43,28 +43,28 @@
 
 
 class BigQuerySqlClient(SqlClientBase[bigquery.Client], DBTransaction):
 
     dbapi: ClassVar[DBApi] = bq_dbapi
     capabilities: ClassVar[DestinationCapabilitiesContext] = capabilities()
 
-    def __init__(self, dataset_name: str, credentials: GcpClientCredentials) -> None:
+    def __init__(self, dataset_name: str, credentials: GcpServiceAccountCredentialsWithoutDefaults) -> None:
         self._client: bigquery.Client = None
-        self.credentials: GcpClientCredentials = credentials
+        self.credentials: GcpServiceAccountCredentialsWithoutDefaults = credentials
         super().__init__(dataset_name)
 
         self._default_retry = bigquery.DEFAULT_RETRY.with_deadline(credentials.retry_deadline)
         self._default_query = bigquery.QueryJobConfig(default_dataset=self.fully_qualified_dataset_name(escape=False))
         self._session_query: bigquery.QueryJobConfig = None
 
     @raise_open_connection_error
     def open_connection(self) -> bigquery.Client:
         self._client = bigquery.Client(
             self.credentials.project_id,
-            credentials=self.credentials.to_google_credentials(),
+            credentials=self.credentials.to_native_credentials(),
             location=self.credentials.location
         )
 
         # patch the client query so our defaults are used
         query_orig = self._client.query
 
         def query_patch(
@@ -210,14 +210,16 @@
             if reason is None:
                 if isinstance(ex, (dbapi_exceptions.DataError, dbapi_exceptions.IntegrityError)):
                     return DatabaseTerminalException(ex)
                 elif isinstance(ex, dbapi_exceptions.ProgrammingError):
                     return DatabaseTransientException(ex)
             if reason == "notFound":
                 return DatabaseUndefinedRelation(ex)
+            if reason == "invalidQuery" and "was not found" in str(ex) and "Dataset" in str(ex):
+                return DatabaseUndefinedRelation(ex)
             if reason == "invalidQuery" and ("Unrecognized name" in str(ex) or "cannot be null" in str(ex)):
                 # unknown column, inserting NULL into required field
                 return DatabaseTerminalException(ex)
             if reason in BQ_TERMINAL_REASONS:
                 return DatabaseTerminalException(ex)
             # anything else is transient
             return DatabaseTransientException(ex)
```

### Comparing `dlt-0.2.6a1/dlt/destinations/duckdb/__init__.py` & `dlt-0.2.6a2/dlt/destinations/duckdb/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/destinations/duckdb/configuration.py` & `dlt-0.2.6a2/dlt/destinations/duckdb/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
             # check if database was passed as explicit connection
             import duckdb
             if isinstance(native_value, duckdb.DuckDBPyConnection):
                 self._conn = native_value
                 self._conn_owner = False
                 self._conn_borrows = 0
                 self.database = ":external:"
-                self.__is_resolved__ = not self.is_partial()
+                self.__is_resolved__ = True
                 return
         except ImportError:
             pass
         try:
             super().parse_native_representation(native_value)
         except InvalidConnectionString:
             if native_value == ":pipeline:" or is_valid_filepath(native_value, platform="auto"):
```

### Comparing `dlt-0.2.6a1/dlt/destinations/duckdb/duck.py` & `dlt-0.2.6a2/dlt/destinations/duckdb/duck.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/destinations/duckdb/sql_client.py` & `dlt-0.2.6a2/dlt/destinations/duckdb/sql_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/destinations/dummy/__init__.py` & `dlt-0.2.6a2/dlt/destinations/dummy/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/destinations/dummy/configuration.py` & `dlt-0.2.6a2/dlt/destinations/dummy/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/destinations/dummy/dummy.py` & `dlt-0.2.6a2/dlt/destinations/dummy/dummy.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/destinations/exceptions.py` & `dlt-0.2.6a2/dlt/destinations/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/destinations/insert_job_client.py` & `dlt-0.2.6a2/dlt/destinations/insert_job_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/destinations/job_client_impl.py` & `dlt-0.2.6a2/dlt/destinations/job_client_impl.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,28 +86,30 @@
         with self.sql_client.with_staging_dataset(staging):
             super().update_storage_schema(staging, only_tables, expected_update)
             applied_update: TSchemaTables = {}
             schema_info = self.get_schema_by_hash(self.schema.stored_version_hash)
             if schema_info is None:
                 logger.info(f"Schema with hash {self.schema.stored_version_hash} not found in the storage. upgrading")
 
-                with self._ddl_transaction():
+                with self.maybe_ddl_transaction():
                     applied_update = self._execute_schema_update_sql(only_tables)
             else:
                 logger.info(f"Schema with hash {self.schema.stored_version_hash} inserted at {schema_info.inserted_at} found in storage, no upgrade required")
             return applied_update
 
-    def drop_tables(self, *tables: str, staging: bool = False) -> None:
-        with self.sql_client.with_staging_dataset(staging):
-            with self._ddl_transaction():
+    def drop_tables(self, *tables: str, staging: bool = False, replace_schema: bool = True) -> None:
+        with self.maybe_ddl_transaction():
+            with self.sql_client.with_staging_dataset(staging):
                 self.sql_client.drop_tables(*tables)
-                self._replace_schema_in_storage(self.schema)
+                if replace_schema:
+                    self._replace_schema_in_storage(self.schema)
 
     @contextlib.contextmanager
-    def _ddl_transaction(self) -> Iterator[None]:
+    def maybe_ddl_transaction(self) -> Iterator[None]:
+        """Begins a transaction if sql client supports it, otherwise works in auto commit"""
         if self.capabilities.supports_ddl_transactions:
             with self.sql_client.begin_transaction():
                 yield
         else:
             yield
 
     def create_merge_job(self, table_chain: Sequence[TTableSchema]) -> NewLoadJob:
```

### Comparing `dlt-0.2.6a1/dlt/destinations/job_impl.py` & `dlt-0.2.6a2/dlt/destinations/job_impl.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/destinations/postgres/__init__.py` & `dlt-0.2.6a2/dlt/destinations/postgres/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/destinations/postgres/postgres.py` & `dlt-0.2.6a2/dlt/destinations/postgres/postgres.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/destinations/postgres/sql_client.py` & `dlt-0.2.6a2/dlt/destinations/postgres/sql_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,20 +8,19 @@
 else:
     import psycopg2
     from psycopg2.sql import SQL, Identifier, Literal as SQLLiteral, Composed, Composable
 
 from contextlib import contextmanager
 from typing import Any, AnyStr, ClassVar, Iterator, Optional, Sequence
 
-from dlt.common.configuration.specs import PostgresCredentials
-
 from dlt.destinations.exceptions import DatabaseTerminalException, DatabaseTransientException, DatabaseUndefinedRelation
 from dlt.destinations.typing import DBApi, DBApiCursor, DBTransaction
 from dlt.destinations.sql_client import DBApiCursorImpl, SqlClientBase, raise_database_error, raise_open_connection_error
 
+from dlt.destinations.postgres.configuration import PostgresCredentials
 from dlt.destinations.postgres import capabilities
 
 class Psycopg2SqlClient(SqlClientBase["psycopg2.connection"], DBTransaction):
 
     dbapi: ClassVar[DBApi] = psycopg2
     capabilities: ClassVar[DestinationCapabilitiesContext] = capabilities()
```

### Comparing `dlt-0.2.6a1/dlt/destinations/redshift/README.md` & `dlt-0.2.6a2/dlt/destinations/redshift/README.md`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/destinations/redshift/__init__.py` & `dlt-0.2.6a2/dlt/destinations/redshift/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/destinations/redshift/redshift.py` & `dlt-0.2.6a2/dlt/destinations/redshift/redshift.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/destinations/sql_client.py` & `dlt-0.2.6a2/dlt/destinations/sql_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/destinations/sql_merge_job.py` & `dlt-0.2.6a2/dlt/destinations/sql_merge_job.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/destinations/typing.py` & `dlt-0.2.6a2/dlt/destinations/typing.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/extract/decorators.py` & `dlt-0.2.6a2/dlt/extract/decorators.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from dlt.common.configuration import with_config, get_fun_spec, known_sections, configspec
 from dlt.common.configuration.container import Container
 from dlt.common.configuration.exceptions import ContextDefaultCannotBeCreated
 from dlt.common.configuration.resolve import inject_section
 from dlt.common.configuration.specs import BaseConfiguration, ContainerInjectableContext
 from dlt.common.configuration.specs.config_section_context import ConfigSectionContext
 from dlt.common.exceptions import ArgumentsOverloadException
+from dlt.common.pipeline import PipelineContext
 from dlt.common.schema.schema import Schema
 from dlt.common.schema.typing import TColumnKey, TColumnName, TTableSchemaColumns, TWriteDisposition
 from dlt.common.storages.exceptions import SchemaNotFoundError
 from dlt.common.storages.schema_storage import SchemaStorage
 from dlt.common.typing import AnyFun, ParamSpec, Concatenate, TDataItem, TDataItems
 from dlt.common.utils import get_callable_name, get_module_name, is_inner_callable
 from dlt.extract.exceptions import InvalidTransformerDataTypeGeneratorFunctionRequired, ResourceFunctionExpected, ResourceInnerCallableConfigWrapDisallowed, SourceDataIsNone, SourceIsAClassTypeError, SourceNotAFunction, SourceSchemaNotAvailable
@@ -151,15 +152,17 @@
         conf_f = with_config(f, spec=spec, sections=source_sections)
 
         @wraps(conf_f)
         def _wrap(*args: Any, **kwargs: Any) -> DltSource:
             # make schema available to the source
             with Container().injectable_context(SourceSchemaInjectableContext(schema)):
                 # configurations will be accessed in this section in the source
-                with inject_section(ConfigSectionContext(sections=source_sections)):
+                proxy = Container()[PipelineContext]
+                pipeline_name = None if not proxy.is_active() else proxy.pipeline().pipeline_name
+                with inject_section(ConfigSectionContext(pipeline_name=pipeline_name, sections=source_sections)):
                     rv = conf_f(*args, **kwargs)
 
             if rv is None:
                 raise SourceDataIsNone(name)
 
             # if generator, consume it immediately
             if inspect.isgenerator(rv):
@@ -342,21 +345,22 @@
         resource_sections = (known_sections.SOURCES, source_section, resource_name)
         # standalone resource will prefer existing section context when resolving config values
         # this lets the source to override those values and provide common section for all config values for resources present in that source
         conf_f = with_config(
             incr_f,
             spec=spec, sections=resource_sections, sections_merge_style=ConfigSectionContext.resource_merge_style, include_defaults=False
         )
-        if conf_f != incr_f and is_inner_callable(f):
+        is_inner_resource = is_inner_callable(f)
+        if conf_f != incr_f and is_inner_resource:
             raise ResourceInnerCallableConfigWrapDisallowed(resource_name, source_section)
         # get spec for wrapped function
         SPEC = get_fun_spec(conf_f)
 
         # store the standalone resource information
-        if SPEC:
+        if not is_inner_resource:
             _SOURCES[f.__qualname__] = SourceInfo(SPEC, f, func_module)
 
         return make_resource(resource_name, source_section, conf_f, incremental)
 
     # if data is callable or none use decorator
     if data is None:
         # we're called with parens.
```

### Comparing `dlt-0.2.6a1/dlt/extract/exceptions.py` & `dlt-0.2.6a2/dlt/extract/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/extract/extract.py` & `dlt-0.2.6a2/dlt/extract/extract.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/extract/incremental.py` & `dlt-0.2.6a2/dlt/extract/incremental.py`

 * *Files 0% similar despite different names*

```diff
@@ -118,15 +118,16 @@
             self.initial_value = native_value.initial_value
             self.last_value_func = native_value.last_value_func
             self.cursor_path_p = self.cursor_path_p
             self.resource_name = self.resource_name
         else:  # TODO: Maybe check if callable(getattr(native_value, '__lt__', None))
             # Passing bare value `incremental=44` gets parsed as initial_value
             self.initial_value = native_value
-        self.__is_resolved__ = not self.is_partial()
+        if not self.is_partial():
+            self.resolve()
 
     def get_state(self) -> IncrementalColumnState:
         """Returns an Incremental state for a particular cursor column"""
         if not self.resource_name:
             raise IncrementalUnboundError(self.cursor_path)
         self._cached_state = Incremental._get_state(self.resource_name, self.cursor_path)
         if len(self._cached_state) == 0:
```

### Comparing `dlt-0.2.6a1/dlt/extract/pipe.py` & `dlt-0.2.6a2/dlt/extract/pipe.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/extract/schema.py` & `dlt-0.2.6a2/dlt/extract/schema.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/extract/source.py` & `dlt-0.2.6a2/dlt/extract/source.py`

 * *Files 1% similar despite different names*

```diff
@@ -341,16 +341,16 @@
         pipe_iterator.set_context_manager(multi_context_manager(_get_context()))
         _iter = map(lambda item: item.item, pipe_iterator)
         return flatten_list_or_items(_iter)
 
     def _get_config_section_context(self) -> ContextManager[ConfigSectionContext]:
         container = Container()
         proxy = container[PipelineContext]
-        pipeline_name = uniq_id() if not proxy.is_active() else proxy.pipeline().pipeline_name
-        return inject_section(ConfigSectionContext(sections=(known_sections.SOURCES, self.section or pipeline_name, self._name)))
+        pipeline_name = None if not proxy.is_active() else proxy.pipeline().pipeline_name
+        return inject_section(ConfigSectionContext(pipeline_name=pipeline_name, sections=(known_sections.SOURCES, self.section or pipeline_name or uniq_id(), self._name)))
 
     def __str__(self) -> str:
         info = f"DltResource {self._name}"
         if self.section:
             info += f" in section {self.section}:"
         else:
             info += ":"
@@ -655,15 +655,17 @@
             pipe_iterator: ManagedPipeIterator = ManagedPipeIterator.from_pipes(self._resources.selected_pipes)  # type: ignore
         pipe_iterator.set_context_manager(multi_context_manager(_get_context()))
         _iter = map(lambda item: item.item, pipe_iterator)
         self.exhausted = True
         return flatten_list_or_items(_iter)
 
     def _get_config_section_context(self) -> ContextManager[ConfigSectionContext]:
-        return inject_section(ConfigSectionContext(sections=(known_sections.SOURCES, self.section, self.name)))
+        proxy = Container()[PipelineContext]
+        pipeline_name = None if not proxy.is_active() else proxy.pipeline().pipeline_name
+        return inject_section(ConfigSectionContext(pipeline_name=pipeline_name, sections=(known_sections.SOURCES, self.section, self.name)))
 
     def _add_resource(self, name: str, resource: DltResource) -> None:
         if self.exhausted:
             raise SourceExhausted(self.name)
 
         if name in self._resources:
             # for resources with the same name try to add the resource as an another pipe
```

### Comparing `dlt-0.2.6a1/dlt/extract/typing.py` & `dlt-0.2.6a2/dlt/extract/typing.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/extract/utils.py` & `dlt-0.2.6a2/dlt/extract/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/helpers/dbt/__init__.py` & `dlt-0.2.6a2/dlt/helpers/dbt/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/helpers/dbt/configuration.py` & `dlt-0.2.6a2/dlt/helpers/dbt/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/helpers/dbt/dbt_utils.py` & `dlt-0.2.6a2/dlt/helpers/dbt/dbt_utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/helpers/dbt/exceptions.py` & `dlt-0.2.6a2/dlt/helpers/dbt/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/helpers/dbt/profiles.yml` & `dlt-0.2.6a2/dlt/helpers/dbt/profiles.yml`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/helpers/dbt/runner.py` & `dlt-0.2.6a2/dlt/helpers/dbt/runner.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/helpers/pandas.py` & `dlt-0.2.6a2/dlt/helpers/pandas.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/helpers/parquet.py` & `dlt-0.2.6a2/dlt/helpers/parquet.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/helpers/streamlit.py` & `dlt-0.2.6a2/dlt/helpers/streamlit.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/load/configuration.py` & `dlt-0.2.6a2/dlt/load/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/load/exceptions.py` & `dlt-0.2.6a2/dlt/load/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/load/load.py` & `dlt-0.2.6a2/dlt/load/load.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/normalize/configuration.py` & `dlt-0.2.6a2/dlt/normalize/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/normalize/normalize.py` & `dlt-0.2.6a2/dlt/normalize/normalize.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/pipeline/README.md` & `dlt-0.2.6a2/dlt/pipeline/README.md`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/pipeline/__init__.py` & `dlt-0.2.6a2/dlt/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/pipeline/configuration.py` & `dlt-0.2.6a2/dlt/pipeline/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/pipeline/dbt.py` & `dlt-0.2.6a2/dlt/pipeline/dbt.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/pipeline/exceptions.py` & `dlt-0.2.6a2/dlt/pipeline/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/pipeline/helpers.py` & `dlt-0.2.6a2/dlt/pipeline/helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from collections import defaultdict
+import contextlib
 from typing import Callable, Tuple, Iterable, Optional, Any, cast, List, Iterator, Dict, Union, TypedDict
 from itertools import chain
 
 from dlt.common.jsonpath import resolve_paths, TAnyJsonPath, compile_paths
 
 from dlt.common.exceptions import TerminalException
 from dlt.common.schema.utils import get_child_tables, group_tables_by_resource, compile_simple_regexes, compile_simple_regex
 from dlt.common.schema.typing import TSimpleRegex
 from dlt.common.typing import REPattern
+from dlt.destinations.exceptions import DatabaseUndefinedRelation
 
 from dlt.pipeline.exceptions import PipelineStepFailed, PipelineHasPendingDataException
 from dlt.pipeline.typing import TPipelineStep
 from dlt.pipeline import Pipeline
 from dlt.common.pipeline import TSourceState, _reset_resource_state, sources_state, _delete_source_state_keys, _get_matching_resources
 
 
@@ -115,16 +117,20 @@
         self._new_state = self._create_modified_state()
 
     @property
     def is_empty(self) -> bool:
         return len(self.info['tables']) == 0 and len(self.info["state_paths"]) == 0 and len(self.info["resource_states"]) == 0
 
     def _drop_destination_tables(self) -> None:
+        table_names = [tbl['name'] for tbl in self.tables_to_drop]
         with self.pipeline._sql_job_client(self.schema) as client:
-            client.drop_tables(*[tbl['name'] for tbl in self.tables_to_drop])
+            client.drop_tables(*table_names)
+            # also delete staging but ignore if staging does not exist
+            with contextlib.suppress(DatabaseUndefinedRelation):
+                client.drop_tables(*table_names, staging=True)
 
     def _delete_pipeline_tables(self) -> None:
         for tbl in self.tables_to_drop:
             del self.schema_tables[tbl['name']]
         self.schema.bump_version()
 
     def _list_state_paths(self, source_state: Dict[str, Any]) -> List[str]:
```

### Comparing `dlt-0.2.6a1/dlt/pipeline/pipeline.py` & `dlt-0.2.6a2/dlt/pipeline/pipeline.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import contextlib
 import os
 import datetime  # noqa: 251
 from contextlib import contextmanager
 from functools import wraps
 from collections.abc import Sequence as C_Sequence
-from typing import Any, Callable, ClassVar, List, Iterator, Mapping, Optional, Sequence, Tuple, cast, get_type_hints, ContextManager
+from typing import Any, Callable, ClassVar, List, Iterator, Optional, Sequence, Tuple, cast, get_type_hints, ContextManager
 
 from dlt import version
 from dlt.common import json, logger, pendulum
 from dlt.common.configuration import inject_section, known_sections
-from dlt.common.configuration.specs import RunConfiguration, NormalizeVolumeConfiguration, SchemaVolumeConfiguration, LoadVolumeConfiguration
+from dlt.common.configuration.specs import RunConfiguration, NormalizeVolumeConfiguration, SchemaVolumeConfiguration, LoadVolumeConfiguration, CredentialsConfiguration
 from dlt.common.configuration.container import Container
 from dlt.common.configuration.exceptions import ConfigFieldMissingException, ContextDefaultCannotBeCreated
 from dlt.common.configuration.specs.config_section_context import ConfigSectionContext
 from dlt.common.exceptions import MissingDependencyException
 from dlt.common.normalizers import default_normalizers, import_normalizers
 from dlt.common.runtime import signals, initialize_runtime
 from dlt.common.schema.exceptions import InvalidDatasetName
@@ -807,21 +807,26 @@
                 self.pipeline_name,
                 "destination",
                 "load",
                 "Please provide `destination` argument to `pipeline`, `run` or `load` method directly or via .dlt config.toml file or environment variable."
             )
         # create initial destination client config
         client_spec = self.destination.spec()
+        # initialize explicit credentials
+        credentials = credentials or self.credentials
+        if credentials is not None and not isinstance(credentials, CredentialsConfiguration):
+            # use passed credentials as initial value. initial value may resolve credentials
+            credentials = client_spec.get_resolvable_fields()["credentials"](credentials)
         # this client support schemas and datasets
         if issubclass(client_spec, DestinationClientDwhConfiguration):
             # set default schema name to load all incoming data to a single dataset, no matter what is the current schema name
             default_schema_name = None if self.config.use_single_dataset else self.default_schema_name
-            return client_spec(dataset_name=self.dataset_name, default_schema_name=default_schema_name, credentials=credentials or self.credentials)
+            return client_spec(dataset_name=self.dataset_name, default_schema_name=default_schema_name, credentials=credentials)
         else:
-            return client_spec(credentials=credentials or self.credentials)
+            return client_spec(credentials=credentials)
 
     def _get_destination_client(self, schema: Schema, initial_config: DestinationClientConfiguration = None) -> JobClientBase:
         try:
             # config is not provided then get it with injected credentials
             if not initial_config:
                 initial_config = self._get_destination_client_initial_config()
             return self.destination.client(schema, initial_config)
```

### Comparing `dlt-0.2.6a1/dlt/pipeline/progress.py` & `dlt-0.2.6a2/dlt/pipeline/progress.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/pipeline/state_sync.py` & `dlt-0.2.6a2/dlt/pipeline/state_sync.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/pipeline/trace.py` & `dlt-0.2.6a2/dlt/pipeline/trace.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/pipeline/track.py` & `dlt-0.2.6a2/dlt/pipeline/track.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/reflection/names.py` & `dlt-0.2.6a2/dlt/reflection/names.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/reflection/script_inspector.py` & `dlt-0.2.6a2/dlt/reflection/script_inspector.py`

 * *Files 16% similar despite different names*

```diff
@@ -31,19 +31,24 @@
     __all__: List[Any] = []   # support wildcard imports
 
 
 def _import_module(name: str, missing_modules: Tuple[str, ...] = ()) -> ModuleType:
     """Module importer that ignores missing modules by importing a dummy module"""
 
     def _try_import(name: str, _globals: Mapping[str, Any] = None, _locals: Mapping[str, Any] = None, fromlist: Sequence[str] = (), level:int = 0) -> ModuleType:
+        """This function works as follows: on ImportError it raises. This import error is then next caught in the main function body and the name is added to exceptions.
+        Next time if the name is on exception list or name is a package on exception list we return DummyModule and do not reraise
+        This excepts only the modules that bubble up ImportError up until our code so any handled import errors are not excepted
+        """
         try:
             return real_import(name, _globals, _locals, fromlist, level)
         except ImportError:
-            # print(f"_import_module {name} {missing_modules}")
-            if any(name.startswith(m) for m in missing_modules):
+            # print(f"_import_module {name} {missing_modules} {fromlist} {level} {ex}")
+            # return a dummy when: (1) name is on exception list (2) name is package path (dot separated) that start with exception from the list
+            if any(name == m or name.startswith(m + ".") for m in missing_modules):
                 return DummyModule(name)
             else:
                 raise
 
     try:
         # patch built in import
         real_import, builtins.__import__ = builtins.__import__, _try_import  # type: ignore
```

### Comparing `dlt-0.2.6a1/dlt/reflection/script_visitor.py` & `dlt-0.2.6a2/dlt/reflection/script_visitor.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/sources/helpers/requests/__init__.py` & `dlt-0.2.6a2/dlt/sources/helpers/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/sources/helpers/requests/retry.py` & `dlt-0.2.6a2/dlt/sources/helpers/requests/retry.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/sources/helpers/requests/session.py` & `dlt-0.2.6a2/dlt/sources/helpers/requests/session.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/sources/helpers/transform.py` & `dlt-0.2.6a2/dlt/sources/helpers/transform.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/dlt/version.py` & `dlt-0.2.6a2/dlt/version.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.6a1/pyproject.toml` & `dlt-0.2.6a2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dlt"
-version = "0.2.6a1"
+version = "0.2.6a2"
 description = "DLT is an open-source python-native scalable data loading framework that does not require any devops efforts to run."
 authors = ["dltHub Inc. <services@dlthub.com>"]
 maintainers = [ "Marcin Rudolf <marcin@dlthub.com>", "Adrian Brudaru <adrian@dlthub.com>", "Ty Dunn <ty@dlthub.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://github.com/dlt-hub"
 repository = "https://github.com/dlt-hub/dlt"
@@ -119,10 +119,16 @@
 
 [tool.poetry.group.airflow]
 optional = true
 
 [tool.poetry.group.airflow.dependencies]
 apache-airflow = "^2.5.3"
 
+[tool.poetry.group.providers]
+optional = true
+
+[tool.poetry.group.providers.dependencies]
+google-api-python-client = "^2.86.0"
+
 [build-system]
 requires = ["poetry-core>=1.0.8"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `dlt-0.2.6a1/setup.py` & `dlt-0.2.6a2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,15 @@
  'redshift:platform_python_implementation == "PyPy"': ['psycopg2cffi>=2.9.0']}
 
 entry_points = \
 {'console_scripts': ['dlt = dlt.cli._dlt:_main']}
 
 setup_kwargs = {
     'name': 'dlt',
-    'version': '0.2.6a1',
+    'version': '0.2.6a2',
     'description': 'DLT is an open-source python-native scalable data loading framework that does not require any devops efforts to run.',
     'long_description': '<h1 align="center">\n    <strong>data load tool (dlt) — the open-source Python library for data loading</strong>\n</h1>\n<p align="center">\nBe it a Google Colab notebook, AWS Lambda function, an Airflow DAG, your local laptop,<br/>or a GPT-4 assisted development playground—<strong>dlt</strong> can be dropped in anywhere.\n</p>\n\n<div align="center">\n  <a target="_blank" href="https://join.slack.com/t/dlthub-community/shared_invite/zt-1slox199h-HAE7EQoXmstkP_bTqal65g" style="background:none">\n    <img src="https://img.shields.io/badge/slack-join-dlt.svg?labelColor=191937&color=6F6FF7&logo=slack" />\n  </a>\n  <a target="_blank" href="https://pypi.org/project/dlt/" style="background:none">\n    <img src="https://img.shields.io/pypi/v/dlt?labelColor=191937&color=6F6FF7">\n  </a>\n  <a target="_blank" href="https://pypi.org/project/dlt/" style="background:none">\n    <img src="https://img.shields.io/pypi/pyversions/dlt?labelColor=191937&color=6F6FF7">\n  </a>\n</div>\n\n## Installation\n\ndlt supports Python 3.8+.\n\n```bash\npip install dlt\n```\n\n## Quick Start\n\nLoad chess game data from chess.com API and save it in DuckDB:\n\n```python\nimport dlt\nfrom chess import chess # a utility function that grabs data from the chess.com API\n\n# create a dlt pipeline that will load chess game data to the DuckDB destination\npipeline = dlt.pipeline(\n    pipeline_name=\'chess_pipeline\',\n    destination=\'duckdb\',\n    dataset_name=\'games_data\'\n)\n\n# use chess.com API to grab data about a few players\ndata = chess([\'magnuscarlsen\', \'rpragchess\'], start_month=\'2022/11\', end_month=\'2022/12\')\n\n# extract, normalize, and load the data\npipeline.run(data)\n```\n\nTry it out in our **[Colab Demo](https://colab.research.google.com/drive/1NfSB1DpwbbHX9_t5vlalBTf13utwpMGx?usp=sharing)**\n\n## Features\n\n- **Automatic Schema:** Data structure inspection and schema creation for the destination.\n- **Data Normalization:** Consistent and verified data before loading.\n- **Seamless Integration:** Colab, AWS Lambda, Airflow, and local environments.\n- **Scalable:** Adapts to growing data needs in production.\n- **Easy Maintenance:** Clear data pipeline structure for updates.\n- **Rapid Exploration:** Quickly explore and gain insights from new data sources.\n- **Versatile Usage:** Suitable for ad-hoc exploration to advanced loading infrastructures.\n- **Start in Seconds with CLI:** Powerful CLI for managing, deploying and inspecting local pipelines.\n- **Incremental Loading:** Load only new or changed data and avoid loading old records again.\n- **Open Source:** Free and Apache 2.0 Licensed.\n\n## Ready to use Pipelines and Destinations\n\nExplore ready to use pipelines (e.g. Google Sheets) in the [Pipelines docs](https://dlthub.com/docs/pipelines/chess) and supported destinations (e.g. DuckDB) in the [Destinations docs](https://dlthub.com/docs/destinations/bigquery).\n\n## Documentation\n\nFor detailed usage and configuration, please refer to the [official documentation](https://dlthub.com/docs).\n\n## Examples\n\nYou can find examples for various use cases in the [examples](docs/examples) folder.\n\n## Get Involved\n\nThe dlt project is quickly growing, and we\'re excited to have you join our community! Here\'s how you can get involved:\n\n- **Connect with the Community**: Join other dlt users and contributors on our [Slack](https://join.slack.com/t/dlthub-community/shared_invite/zt-1slox199h-HAE7EQoXmstkP_bTqal65g)\n- **Report issues and suggest features**: Please use the [GitHub Issues](https://github.com/dlt-hub/dlt/issues) to report bugs or suggest new features. Before creating a new issue, make sure to search the tracker for possible duplicates and add a comment if you find one.\n- **Contribute Pipelines**: Pipelines are data processing steps that help move and transform data between various sources and destinations. Contribute your custom pipelines to the [dlt-hub/pipelines](https://github.com/dlt-hub/pipelines) to help other folks in handling their data tasks.\n- **Contribute code**: Check out our [contributing guidelines](CONTRIBUTING.md) for information on how to make a pull request.\n- **Improve documentation**: Help us enhance the dlt documentation.\n\n## License\n\nDLT is released under the [Apache 2.0 License](LICENSE.txt).\n',
     'author': 'dltHub Inc.',
     'author_email': 'services@dlthub.com',
     'maintainer': 'Marcin Rudolf',
     'maintainer_email': 'marcin@dlthub.com',
     'url': 'https://github.com/dlt-hub',
```

### Comparing `dlt-0.2.6a1/PKG-INFO` & `dlt-0.2.6a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dlt
-Version: 0.2.6a1
+Version: 0.2.6a2
 Summary: DLT is an open-source python-native scalable data loading framework that does not require any devops efforts to run.
 Home-page: https://github.com/dlt-hub
 License: Apache-2.0
 Keywords: etl
 Author: dltHub Inc.
 Author-email: services@dlthub.com
 Maintainer: Marcin Rudolf
```

