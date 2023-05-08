# Comparing `tmp/PyPlumIO-0.4.1.tar.gz` & `tmp/PyPlumIO-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyPlumIO-0.4.1.tar", last modified: Sun Apr 30 06:06:34 2023, max compression
+gzip compressed data, was "PyPlumIO-0.4.2.tar", last modified: Mon May  8 19:05:20 2023, max compression
```

## Comparing `PyPlumIO-0.4.1.tar` & `PyPlumIO-0.4.2.tar`

### file list

```diff
@@ -1,128 +1,128 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:06:34.424962 PyPlumIO-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:06:34.416962 PyPlumIO-0.4.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/.github/CODE_OF_CONDUCT.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:06:34.416962 PyPlumIO-0.4.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/.github/ISSUE_TEMPLATE/feature_request.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:06:34.416962 PyPlumIO-0.4.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/.github/workflows/documentation.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:06:34.416962 PyPlumIO-0.4.1/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-04-30 06:06:34.424962 PyPlumIO-0.4.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:06:34.416962 PyPlumIO-0.4.1/PyPlumIO.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-04-30 06:06:34.000000 PyPlumIO-0.4.1/PyPlumIO.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-04-30 06:06:34.000000 PyPlumIO-0.4.1/PyPlumIO.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 06:06:34.000000 PyPlumIO-0.4.1/PyPlumIO.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-30 06:06:34.000000 PyPlumIO-0.4.1/PyPlumIO.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-30 06:06:34.000000 PyPlumIO-0.4.1/PyPlumIO.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:06:34.416962 PyPlumIO-0.4.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:06:34.416962 PyPlumIO-0.4.1/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/docs/source/protocol.rst
--rw-r--r--   0 runner    (1001) docker     (123)    21175 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/docs/source/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:06:34.416962 PyPlumIO-0.4.1/images/
--rw-r--r--   0 runner    (1001) docker     (123)    32463 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/images/ecomax.png
--rw-r--r--   0 runner    (1001) docker     (123)   133458 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/images/rs485.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:06:34.416962 PyPlumIO-0.4.1/pyplumio/
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-30 06:06:34.000000 PyPlumIO-0.4.1/pyplumio/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5494 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/const.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:06:34.420961 PyPlumIO-0.4.1/pyplumio/devices/
--rw-r--r--   0 runner    (1001) docker     (123)     4871 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15223 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/devices/ecomax.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/devices/ecoster.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/devices/mixer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/devices/thermostat.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:06:34.420961 PyPlumIO-0.4.1/pyplumio/frames/
--rw-r--r--   0 runner    (1001) docker     (123)     4981 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/frames/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/frames/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     6292 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/frames/requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     6190 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/frames/responses.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:06:34.420961 PyPlumIO-0.4.1/pyplumio/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7037 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/helpers/data_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/helpers/event_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/helpers/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     7093 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/helpers/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/helpers/schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/helpers/task_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/helpers/timeout.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/helpers/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/helpers/uid.py
--rw-r--r--   0 runner    (1001) docker     (123)     6223 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/stream.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:06:34.424962 PyPlumIO-0.4.1/pyplumio/structures/
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/structures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/structures/alerts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/structures/data_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    16082 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/structures/ecomax_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/structures/fan_power.py
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/structures/frame_versions.py
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/structures/fuel_consumption.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/structures/fuel_level.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/structures/lambda_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/structures/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     6115 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/structures/mixer_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/structures/mixer_sensors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/structures/modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/structures/network_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/structures/output_flags.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/structures/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/structures/pending_alerts.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/structures/power.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/structures/product_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/structures/program_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/structures/regulator_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6135 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/structures/schedules.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/structures/statuses.py
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/structures/temperatures.py
--rw-r--r--   0 runner    (1001) docker     (123)     6399 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/structures/thermostat_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/structures/thermostat_sensors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyplumio/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/requirements_test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 06:06:34.424962 PyPlumIO-0.4.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:06:34.424962 PyPlumIO-0.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17493 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:06:34.424962 PyPlumIO-0.4.1/tests/frames/
--rw-r--r--   0 runner    (1001) docker     (123)     4641 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/tests/frames/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     6292 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/tests/frames/test_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/tests/frames/test_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     6669 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/tests/frames/test_responses.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:06:34.424962 PyPlumIO-0.4.1/tests/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/tests/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/tests/helpers/test_data_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/tests/helpers/test_event_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/tests/helpers/test_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     6420 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/tests/helpers/test_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/tests/helpers/test_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/tests/helpers/test_task_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/tests/helpers/test_timeout.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/tests/helpers/test_uid.py
--rw-r--r--   0 runner    (1001) docker     (123)     6864 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/tests/test_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    22215 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/tests/test_devices.py
--rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/tests/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)    10465 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/tests/test_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/tests/test_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-04-30 06:06:15.000000 PyPlumIO-0.4.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:05:20.155003 PyPlumIO-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:05:20.131003 PyPlumIO-0.4.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/.github/CODE_OF_CONDUCT.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:05:20.131003 PyPlumIO-0.4.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/.github/ISSUE_TEMPLATE/feature_request.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:05:20.131003 PyPlumIO-0.4.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/.github/workflows/documentation.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:05:20.131003 PyPlumIO-0.4.2/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-05-08 19:05:20.155003 PyPlumIO-0.4.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:05:20.135003 PyPlumIO-0.4.2/PyPlumIO.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-05-08 19:05:20.000000 PyPlumIO-0.4.2/PyPlumIO.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-05-08 19:05:20.000000 PyPlumIO-0.4.2/PyPlumIO.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 19:05:20.000000 PyPlumIO-0.4.2/PyPlumIO.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-08 19:05:20.000000 PyPlumIO-0.4.2/PyPlumIO.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-08 19:05:20.000000 PyPlumIO-0.4.2/PyPlumIO.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:05:20.135003 PyPlumIO-0.4.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:05:20.135003 PyPlumIO-0.4.2/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/docs/source/protocol.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    21175 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/docs/source/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:05:20.135003 PyPlumIO-0.4.2/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    32463 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/images/ecomax.png
+-rw-r--r--   0 runner    (1001) docker     (123)   133458 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/images/rs485.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:05:20.139003 PyPlumIO-0.4.2/pyplumio/
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/pyplumio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/pyplumio/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-08 19:05:19.000000 PyPlumIO-0.4.2/pyplumio/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5494 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/pyplumio/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/pyplumio/const.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:05:20.139003 PyPlumIO-0.4.2/pyplumio/devices/
+-rw-r--r--   0 runner    (1001) docker     (123)     4871 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/pyplumio/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15223 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/pyplumio/devices/ecomax.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/pyplumio/devices/ecoster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/pyplumio/devices/mixer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/pyplumio/devices/thermostat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/pyplumio/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6548 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/pyplumio/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:05:20.139003 PyPlumIO-0.4.2/pyplumio/frames/
+-rw-r--r--   0 runner    (1001) docker     (123)     4981 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/pyplumio/frames/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/pyplumio/frames/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6292 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/pyplumio/frames/requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6190 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/pyplumio/frames/responses.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:05:20.143003 PyPlumIO-0.4.2/pyplumio/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/pyplumio/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7037 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/pyplumio/helpers/data_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/pyplumio/helpers/event_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/pyplumio/helpers/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7093 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/pyplumio/helpers/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/pyplumio/helpers/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/pyplumio/helpers/task_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/pyplumio/helpers/timeout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/pyplumio/helpers/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/pyplumio/helpers/uid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6223 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/pyplumio/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/pyplumio/stream.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:05:20.151003 PyPlumIO-0.4.2/pyplumio/structures/
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/pyplumio/structures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/pyplumio/structures/alerts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/pyplumio/structures/data_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16082 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/pyplumio/structures/ecomax_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/pyplumio/structures/fan_power.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/pyplumio/structures/frame_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/pyplumio/structures/fuel_consumption.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/pyplumio/structures/fuel_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/pyplumio/structures/lambda_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/pyplumio/structures/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6115 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/pyplumio/structures/mixer_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/pyplumio/structures/mixer_sensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/pyplumio/structures/modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/pyplumio/structures/network_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/pyplumio/structures/output_flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/pyplumio/structures/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/pyplumio/structures/pending_alerts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/pyplumio/structures/power.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/pyplumio/structures/product_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/pyplumio/structures/program_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/pyplumio/structures/regulator_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6135 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/pyplumio/structures/schedules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/pyplumio/structures/statuses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/pyplumio/structures/temperatures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6399 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/pyplumio/structures/thermostat_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/pyplumio/structures/thermostat_sensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/pyplumio/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/requirements_test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 19:05:20.155003 PyPlumIO-0.4.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:05:20.151003 PyPlumIO-0.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17493 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:05:20.155003 PyPlumIO-0.4.2/tests/frames/
+-rw-r--r--   0 runner    (1001) docker     (123)     4641 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/tests/frames/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6292 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/tests/frames/test_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/tests/frames/test_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6669 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/tests/frames/test_responses.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:05:20.155003 PyPlumIO-0.4.2/tests/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/tests/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/tests/helpers/test_data_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/tests/helpers/test_event_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/tests/helpers/test_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6420 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/tests/helpers/test_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/tests/helpers/test_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/tests/helpers/test_task_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/tests/helpers/test_timeout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/tests/helpers/test_uid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6864 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/tests/test_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22215 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/tests/test_devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5996 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/tests/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10465 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/tests/test_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/tests/test_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-08 19:04:57.000000 PyPlumIO-0.4.2/tox.ini
```

### Comparing `PyPlumIO-0.4.1/.github/CODE_OF_CONDUCT.md` & `PyPlumIO-0.4.2/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.1/.github/ISSUE_TEMPLATE/bug_report.yml` & `PyPlumIO-0.4.2/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.1/.github/ISSUE_TEMPLATE/feature_request.yml` & `PyPlumIO-0.4.2/.github/ISSUE_TEMPLATE/feature_request.yml`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.1/.github/workflows/ci.yml` & `PyPlumIO-0.4.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.1/.github/workflows/codeql-analysis.yml` & `PyPlumIO-0.4.2/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.1/.github/workflows/deploy.yml` & `PyPlumIO-0.4.2/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.1/.github/workflows/documentation.yml` & `PyPlumIO-0.4.2/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.1/.gitignore` & `PyPlumIO-0.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.1/.pre-commit-config.yaml` & `PyPlumIO-0.4.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.1/.vscode/settings.json` & `PyPlumIO-0.4.2/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.1/LICENSE` & `PyPlumIO-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.1/PKG-INFO` & `PyPlumIO-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyPlumIO
-Version: 0.4.1
+Version: 0.4.2
 Summary: PyPlumIO is a native ecoNET library for Plum ecoMAX controllers.
 Author-email: Denis Paavilainen <denpa@denpa.pro>
 License: MIT License
 Project-URL: Documentation, https://pyplumio.denpa.pro
 Project-URL: Source Code, https://github.com/denpamusic/PyPlumIO
 Project-URL: Bug Tracker, https://github.com/denpamusic/PyPlumIO/issues
 Keywords: home,automation,heating
```

### Comparing `PyPlumIO-0.4.1/PyPlumIO.egg-info/PKG-INFO` & `PyPlumIO-0.4.2/PyPlumIO.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyPlumIO
-Version: 0.4.1
+Version: 0.4.2
 Summary: PyPlumIO is a native ecoNET library for Plum ecoMAX controllers.
 Author-email: Denis Paavilainen <denpa@denpa.pro>
 License: MIT License
 Project-URL: Documentation, https://pyplumio.denpa.pro
 Project-URL: Source Code, https://github.com/denpamusic/PyPlumIO
 Project-URL: Bug Tracker, https://github.com/denpamusic/PyPlumIO/issues
 Keywords: home,automation,heating
```

### Comparing `PyPlumIO-0.4.1/PyPlumIO.egg-info/SOURCES.txt` & `PyPlumIO-0.4.2/PyPlumIO.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.1/README.md` & `PyPlumIO-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.1/docs/Makefile` & `PyPlumIO-0.4.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.1/docs/make.bat` & `PyPlumIO-0.4.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.1/docs/source/conf.py` & `PyPlumIO-0.4.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.1/docs/source/index.rst` & `PyPlumIO-0.4.2/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.1/docs/source/protocol.rst` & `PyPlumIO-0.4.2/docs/source/protocol.rst`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.1/docs/source/usage.rst` & `PyPlumIO-0.4.2/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.1/images/ecomax.png` & `PyPlumIO-0.4.2/images/ecomax.png`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.1/images/rs485.png` & `PyPlumIO-0.4.2/images/rs485.png`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.1/pyplumio/__init__.py` & `PyPlumIO-0.4.2/pyplumio/__init__.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.1/pyplumio/connection.py` & `PyPlumIO-0.4.2/pyplumio/connection.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.1/pyplumio/const.py` & `PyPlumIO-0.4.2/pyplumio/const.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """Contains constants."""
 from __future__ import annotations
 
 from enum import IntEnum, unique
 from typing import Final
 
+UNDEFINED: Final = "undefined"
+
 # Binary states.
 STATE_ON: Final = "on"
 STATE_OFF: Final = "off"
 
 # General attributes.
 ATTR_CONNECTED: Final = "connected"
 ATTR_CURRENT_TEMP: Final = "current_temp"
```

### Comparing `PyPlumIO-0.4.1/pyplumio/devices/__init__.py` & `PyPlumIO-0.4.2/pyplumio/devices/__init__.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.1/pyplumio/devices/ecomax.py` & `PyPlumIO-0.4.2/pyplumio/devices/ecomax.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.1/pyplumio/devices/mixer.py` & `PyPlumIO-0.4.2/pyplumio/devices/mixer.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.1/pyplumio/devices/thermostat.py` & `PyPlumIO-0.4.2/pyplumio/devices/thermostat.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.1/pyplumio/exceptions.py` & `PyPlumIO-0.4.2/pyplumio/exceptions.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.1/pyplumio/filters.py` & `PyPlumIO-0.4.2/pyplumio/filters.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,83 +1,119 @@
 """Contains callback filters."""
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 import math
 import time
-from typing import Any, Final
+from typing import Any, Final, SupportsFloat, SupportsIndex, overload
 
+from pyplumio.const import UNDEFINED
 from pyplumio.helpers.parameter import Parameter
-from pyplumio.helpers.typing import EventCallbackType
+from pyplumio.helpers.typing import EventCallbackType, SupportsSubtraction
 
 TOLERANCE: Final = 0.1
 
 
-def _significantly_changed(old_value, new_value) -> bool:
+@overload
+def _significantly_changed(old: Parameter, new: Parameter) -> bool:
+    """Check if parameter is significantly changed."""
+
+
+@overload
+def _significantly_changed(
+    old: SupportsFloat | SupportsIndex, new: SupportsFloat | SupportsIndex
+) -> bool:
+    """Check if float value is significantly changed."""
+
+
+def _significantly_changed(old, new) -> bool:
     """Check if value is significantly changed."""
-    if old_value is None or (isinstance(old_value, Parameter) and old_value.is_changed):
+    if old == UNDEFINED:
         return True
 
+    if isinstance(old, Parameter) and old.is_changed:
+        return True
+
+    if isinstance(old, Parameter) and isinstance(new, Parameter):
+        return (
+            old.value != new.value
+            or old.min_value != new.min_value
+            or old.max_value != new.max_value
+        )
+
     try:
-        return not math.isclose(old_value, new_value, abs_tol=TOLERANCE)
+        return not math.isclose(old, new, abs_tol=TOLERANCE)
     except TypeError:
         pass
 
-    return old_value != new_value
+    return old != new
+
+
+@overload
+def _diffence_between(old: list, new: list) -> list:
+    """Return the difference between lists."""
 
 
-def _diffence_between(old_value, new_value):
+@overload
+def _diffence_between(old: SupportsSubtraction, new: SupportsSubtraction) -> list:
+    """Return the difference between lists."""
+
+
+def _diffence_between(old, new):
     """Return the difference between values."""
-    if isinstance(old_value, list) and isinstance(new_value, list):
-        return [x for x in new_value if x not in old_value]
+    if old == UNDEFINED:
+        return None
+
+    if isinstance(old, list) and isinstance(new, list):
+        return [x for x in new if x not in old]
 
-    if hasattr(old_value, "__sub__") and hasattr(new_value, "__sub__"):
-        return new_value - old_value
+    if hasattr(old, "__sub__") and hasattr(new, "__sub__"):
+        return new - old
 
     return None
 
 
 class Filter(ABC):
     """Represents base for value callback modifiers."""
 
     _callback: Any
-    _value: Any
+    _value: Any = UNDEFINED
 
     def __init__(self, callback: EventCallbackType):
         """Initialize new Filter object."""
         self._callback = callback
-        self._value = None
+        self._value = UNDEFINED
 
     def __eq__(self, other) -> bool:
         """Compare debounced callbacks."""
         if isinstance(other, Filter):
             return self._callback == other._callback
 
         if callable(other):
             return self._callback == other
 
         raise TypeError
 
     @abstractmethod
     async def __call__(self, new_value):
-        """Set new value for the callback."""
+        """Set a new value for the callback."""
 
 
 class _OnChange(Filter):
     """Provides changed functionality to the callback."""
 
     async def __call__(self, new_value):
-        """Set new value for the callback."""
+        """Set a new value for the callback."""
         if _significantly_changed(self._value, new_value):
             self._value = new_value
             return await self._callback(new_value)
 
 
 def on_change(callback: EventCallbackType) -> _OnChange:
-    """Helper for change callback filter."""
+    """Helper for a change callback filter."""
     return _OnChange(callback)
 
 
 class _Debounce(Filter):
     """Provides debounce functionality to the callback."""
 
     _calls: int = 0
@@ -86,28 +122,28 @@
     def __init__(self, callback: EventCallbackType, min_calls: int):
         """Initialize Debounce object."""
         super().__init__(callback)
         self._calls = 0
         self._min_calls = min_calls
 
     async def __call__(self, new_value):
-        """Set new value for the callback."""
+        """Set a new value for the callback."""
         if _significantly_changed(self._value, new_value):
             self._calls += 1
         else:
             self._calls = 0
 
-        if self._calls >= self._min_calls or self._value is None:
+        if self._value == UNDEFINED or self._calls >= self._min_calls:
             self._value = new_value
             self._calls = 0
             return await self._callback(new_value)
 
 
 def debounce(callback: EventCallbackType, min_calls) -> _Debounce:
-    """Helper method for debounce callback filter."""
+    """Helper method for a debounce callback filter."""
     return _Debounce(callback, min_calls)
 
 
 class _Throttle(Filter):
     """Provides throttle functionality to the callback."""
 
     _last_called: float | None
@@ -116,43 +152,43 @@
     def __init__(self, callback: EventCallbackType, seconds: float):
         """Initialize Debounce object."""
         super().__init__(callback)
         self._last_called = None
         self._timeout = seconds
 
     async def __call__(self, new_value):
-        """set new value for the callback."""
+        """Set a new value for the callback."""
         current_timestamp = time.monotonic()
         if (
             self._last_called is None
             or (current_timestamp - self._last_called) >= self._timeout
         ):
             self._last_called = current_timestamp
             return await self._callback(new_value)
 
 
 def throttle(callback: EventCallbackType, seconds: float) -> _Throttle:
-    """Helper method for throttle callback filter."""
+    """Helper method for a throttle callback filter."""
     return _Throttle(callback, seconds)
 
 
 class _Delta(Filter):
     """Provides ability to pass call difference to the callback."""
 
     async def __call__(self, new_value):
-        """set new value for the callback."""
-        old_value = self._value
-        if _significantly_changed(old_value, new_value):
+        """Set new value for the callback."""
+        if _significantly_changed(self._value, new_value):
+            old_value = self._value
             self._value = new_value
             if (difference := _diffence_between(old_value, new_value)) is not None:
                 return await self._callback(difference)
 
 
 def delta(callback: EventCallbackType) -> _Delta:
-    """Helper method for delta callback filter."""
+    """Helper method for a delta callback filter."""
     return _Delta(callback)
 
 
 class _Aggregate(Filter):
     """Provides ability to sum value for some time before sending them
     to the callback."""
 
@@ -164,15 +200,15 @@
         """Initialize Aggregate object."""
         super().__init__(callback)
         self._last_update = time.monotonic()
         self._timeout = seconds
         self._sum = 0.0
 
     async def __call__(self, new_value):
-        """Set new value for the callback."""
+        """Set a new value for the callback."""
         current_timestamp = time.monotonic()
         try:
             self._sum += new_value
         except TypeError as e:
             raise ValueError(
                 "Aggregate filter can only be used with numeric values"
             ) from e
@@ -181,9 +217,9 @@
             result = await self._callback(self._sum)
             self._last_update = current_timestamp
             self._sum = 0.0
             return result
 
 
 def aggregate(callback: EventCallbackType, seconds: float) -> _Aggregate:
-    """Helper method for total callback filter."""
+    """Helper method for a total callback filter."""
     return _Aggregate(callback, seconds)
```

### Comparing `PyPlumIO-0.4.1/pyplumio/frames/__init__.py` & `PyPlumIO-0.4.2/pyplumio/frames/__init__.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.1/pyplumio/frames/messages.py` & `PyPlumIO-0.4.2/pyplumio/frames/messages.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.1/pyplumio/frames/requests.py` & `PyPlumIO-0.4.2/pyplumio/frames/requests.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.1/pyplumio/frames/responses.py` & `PyPlumIO-0.4.2/pyplumio/frames/responses.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.1/pyplumio/helpers/data_types.py` & `PyPlumIO-0.4.2/pyplumio/helpers/data_types.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.1/pyplumio/helpers/event_manager.py` & `PyPlumIO-0.4.2/pyplumio/helpers/event_manager.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.1/pyplumio/helpers/factory.py` & `PyPlumIO-0.4.2/pyplumio/helpers/factory.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.1/pyplumio/helpers/parameter.py` & `PyPlumIO-0.4.2/pyplumio/helpers/parameter.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.1/pyplumio/helpers/schedule.py` & `PyPlumIO-0.4.2/pyplumio/helpers/schedule.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.1/pyplumio/helpers/task_manager.py` & `PyPlumIO-0.4.2/pyplumio/helpers/task_manager.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.1/pyplumio/helpers/timeout.py` & `PyPlumIO-0.4.2/pyplumio/helpers/timeout.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.1/pyplumio/helpers/uid.py` & `PyPlumIO-0.4.2/pyplumio/helpers/uid.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.1/pyplumio/protocol.py` & `PyPlumIO-0.4.2/pyplumio/protocol.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.1/pyplumio/stream.py` & `PyPlumIO-0.4.2/pyplumio/stream.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.1/pyplumio/structures/__init__.py` & `PyPlumIO-0.4.2/pyplumio/structures/__init__.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.1/pyplumio/structures/alerts.py` & `PyPlumIO-0.4.2/pyplumio/structures/alerts.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.1/pyplumio/structures/data_schema.py` & `PyPlumIO-0.4.2/pyplumio/structures/data_schema.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.1/pyplumio/structures/ecomax_parameters.py` & `PyPlumIO-0.4.2/pyplumio/structures/ecomax_parameters.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.1/pyplumio/structures/fan_power.py` & `PyPlumIO-0.4.2/pyplumio/structures/fan_power.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.1/pyplumio/structures/frame_versions.py` & `PyPlumIO-0.4.2/pyplumio/structures/frame_versions.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.1/pyplumio/structures/fuel_consumption.py` & `PyPlumIO-0.4.2/pyplumio/structures/fuel_consumption.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.1/pyplumio/structures/fuel_level.py` & `PyPlumIO-0.4.2/pyplumio/structures/fuel_level.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.1/pyplumio/structures/lambda_sensor.py` & `PyPlumIO-0.4.2/pyplumio/structures/lambda_sensor.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.1/pyplumio/structures/load.py` & `PyPlumIO-0.4.2/pyplumio/structures/load.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.1/pyplumio/structures/mixer_parameters.py` & `PyPlumIO-0.4.2/pyplumio/structures/mixer_parameters.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.1/pyplumio/structures/mixer_sensors.py` & `PyPlumIO-0.4.2/pyplumio/structures/mixer_sensors.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.1/pyplumio/structures/modules.py` & `PyPlumIO-0.4.2/pyplumio/structures/modules.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.1/pyplumio/structures/network_info.py` & `PyPlumIO-0.4.2/pyplumio/structures/network_info.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.1/pyplumio/structures/output_flags.py` & `PyPlumIO-0.4.2/pyplumio/structures/output_flags.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.1/pyplumio/structures/outputs.py` & `PyPlumIO-0.4.2/pyplumio/structures/outputs.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.1/pyplumio/structures/pending_alerts.py` & `PyPlumIO-0.4.2/pyplumio/structures/pending_alerts.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.1/pyplumio/structures/power.py` & `PyPlumIO-0.4.2/pyplumio/structures/power.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.1/pyplumio/structures/product_info.py` & `PyPlumIO-0.4.2/pyplumio/structures/product_info.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.1/pyplumio/structures/program_version.py` & `PyPlumIO-0.4.2/pyplumio/structures/program_version.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.1/pyplumio/structures/regulator_data.py` & `PyPlumIO-0.4.2/pyplumio/structures/regulator_data.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.1/pyplumio/structures/schedules.py` & `PyPlumIO-0.4.2/pyplumio/structures/schedules.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.1/pyplumio/structures/statuses.py` & `PyPlumIO-0.4.2/pyplumio/structures/statuses.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.1/pyplumio/structures/temperatures.py` & `PyPlumIO-0.4.2/pyplumio/structures/temperatures.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.1/pyplumio/structures/thermostat_parameters.py` & `PyPlumIO-0.4.2/pyplumio/structures/thermostat_parameters.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.1/pyplumio/structures/thermostat_sensors.py` & `PyPlumIO-0.4.2/pyplumio/structures/thermostat_sensors.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.1/pyplumio/util.py` & `PyPlumIO-0.4.2/pyplumio/util.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.1/pyproject.toml` & `PyPlumIO-0.4.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.1/tests/conftest.py` & `PyPlumIO-0.4.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.1/tests/frames/test_init.py` & `PyPlumIO-0.4.2/tests/frames/test_init.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.1/tests/frames/test_messages.py` & `PyPlumIO-0.4.2/tests/frames/test_messages.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.1/tests/frames/test_requests.py` & `PyPlumIO-0.4.2/tests/frames/test_requests.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.1/tests/frames/test_responses.py` & `PyPlumIO-0.4.2/tests/frames/test_responses.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.1/tests/helpers/test_data_types.py` & `PyPlumIO-0.4.2/tests/helpers/test_data_types.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.1/tests/helpers/test_event_manager.py` & `PyPlumIO-0.4.2/tests/helpers/test_event_manager.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.1/tests/helpers/test_factory.py` & `PyPlumIO-0.4.2/tests/helpers/test_factory.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.1/tests/helpers/test_parameter.py` & `PyPlumIO-0.4.2/tests/helpers/test_parameter.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.1/tests/helpers/test_schedule.py` & `PyPlumIO-0.4.2/tests/helpers/test_schedule.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.1/tests/helpers/test_task_manager.py` & `PyPlumIO-0.4.2/tests/helpers/test_task_manager.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.1/tests/helpers/test_timeout.py` & `PyPlumIO-0.4.2/tests/helpers/test_timeout.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.1/tests/test_connection.py` & `PyPlumIO-0.4.2/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.1/tests/test_devices.py` & `PyPlumIO-0.4.2/tests/test_devices.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.1/tests/test_filters.py` & `PyPlumIO-0.4.2/tests/test_filters.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from datetime import datetime
 from unittest.mock import AsyncMock, patch
 
 import pytest
 
 from pyplumio.filters import aggregate, debounce, delta, on_change, throttle
+from pyplumio.helpers.parameter import Parameter
 from pyplumio.structures.alerts import Alert
 
 
 async def test_on_change() -> None:
     """Test on change filter."""
     test_callback = AsyncMock()
     wrapped_callback = on_change(test_callback)
@@ -27,14 +28,71 @@
     # Test equality with callback function and different instance.
     assert test_callback == wrapped_callback
     assert wrapped_callback == on_change(test_callback)
     with pytest.raises(TypeError):
         _ = wrapped_callback == "you shall not pass"
 
 
+async def test_on_change_parameter() -> None:
+    """Test on change filter with parameters."""
+    test_callback = AsyncMock()
+    test_parameter = AsyncMock(spec=Parameter)
+    test_parameter.value = 0
+    test_parameter.min_value = 0
+    test_parameter.max_value = 1
+    test_parameter.is_changed = False
+    wrapped_callback = on_change(test_callback)
+    await wrapped_callback(test_parameter)
+    test_callback.assert_awaited_once_with(test_parameter)
+    test_callback.reset_mock()
+
+    # Check that callback is not awaited with no change.
+    await wrapped_callback(test_parameter)
+    test_callback.assert_not_awaited()
+
+    # Check that callback is awaited on local value change.
+    test_parameter = AsyncMock(spec=Parameter)
+    test_parameter.value = 1
+    test_parameter.min_value = 0
+    test_parameter.max_value = 1
+    test_parameter.is_changed = True
+    await wrapped_callback(test_parameter)
+    test_callback.assert_awaited_once_with(test_parameter)
+    test_callback.reset_mock()
+
+    # Check that callback is awaited on value change.
+    test_parameter = AsyncMock(spec=Parameter)
+    test_parameter.value = 1
+    test_parameter.min_value = 0
+    test_parameter.max_value = 1
+    test_parameter.is_changed = False
+    await wrapped_callback(test_parameter)
+    test_callback.assert_awaited_once_with(test_parameter)
+    test_callback.reset_mock()
+
+    # Check that callback is awaited on min value change.
+    test_parameter = AsyncMock(spec=Parameter)
+    test_parameter.value = 1
+    test_parameter.min_value = 1
+    test_parameter.max_value = 1
+    test_parameter.is_changed = False
+    await wrapped_callback(test_parameter)
+    test_callback.assert_awaited_once_with(test_parameter)
+    test_callback.reset_mock()
+
+    # Check that callback is awaited on max value change.
+    test_parameter = AsyncMock(spec=Parameter)
+    test_parameter.value = 1
+    test_parameter.min_value = 1
+    test_parameter.max_value = 2
+    test_parameter.is_changed = False
+    await wrapped_callback(test_parameter)
+    test_callback.assert_awaited_once_with(test_parameter)
+
+
 async def test_debounce() -> None:
     """Test debounce filter."""
     test_callback = AsyncMock()
     wrapped_callback = debounce(test_callback, min_calls=3)
     await wrapped_callback(1)
     test_callback.assert_awaited_once_with(1)
     test_callback.reset_mock()
```

### Comparing `PyPlumIO-0.4.1/tests/test_init.py` & `PyPlumIO-0.4.2/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.1/tests/test_main.py` & `PyPlumIO-0.4.2/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.1/tests/test_protocol.py` & `PyPlumIO-0.4.2/tests/test_protocol.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.1/tests/test_stream.py` & `PyPlumIO-0.4.2/tests/test_stream.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.1/tests/test_util.py` & `PyPlumIO-0.4.2/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.1/tox.ini` & `PyPlumIO-0.4.2/tox.ini`

 * *Files identical despite different names*

