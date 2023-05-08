# Comparing `tmp/openedx-events-7.1.0.tar.gz` & `tmp/openedx-events-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openedx-events-7.1.0.tar", last modified: Wed May  3 20:27:10 2023, max compression
+gzip compressed data, was "openedx-events-7.2.0.tar", last modified: Mon May  8 18:35:45 2023, max compression
```

## Comparing `openedx-events-7.1.0.tar` & `openedx-events-7.2.0.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 20:27:10.093215 openedx-events-7.1.0/
--rw-r--r--   0 runner    (1001) docker     (122)     8479 2023-05-03 20:27:05.000000 openedx-events-7.1.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-05-03 20:27:05.000000 openedx-events-7.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      177 2023-05-03 20:27:05.000000 openedx-events-7.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    14505 2023-05-03 20:27:10.093215 openedx-events-7.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5366 2023-05-03 20:27:05.000000 openedx-events-7.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 20:27:10.089215 openedx-events-7.1.0/openedx_events/
--rw-r--r--   0 runner    (1001) docker     (122)      217 2023-05-03 20:27:05.000000 openedx-events-7.1.0/openedx_events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      239 2023-05-03 20:27:05.000000 openedx-events-7.1.0/openedx_events/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 20:27:10.089215 openedx-events-7.1.0/openedx_events/content_authoring/
--rw-r--r--   0 runner    (1001) docker     (122)      387 2023-05-03 20:27:05.000000 openedx-events-7.1.0/openedx_events/content_authoring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4493 2023-05-03 20:27:05.000000 openedx-events-7.1.0/openedx_events/content_authoring/data.py
--rw-r--r--   0 runner    (1001) docker     (122)     3615 2023-05-03 20:27:05.000000 openedx-events-7.1.0/openedx_events/content_authoring/signals.py
--rw-r--r--   0 runner    (1001) docker     (122)     3084 2023-05-03 20:27:05.000000 openedx-events-7.1.0/openedx_events/data.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 20:27:10.089215 openedx-events-7.1.0/openedx_events/event_bus/
--rw-r--r--   0 runner    (1001) docker     (122)     7344 2023-05-03 20:27:05.000000 openedx-events-7.1.0/openedx_events/event_bus/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 20:27:10.089215 openedx-events-7.1.0/openedx_events/event_bus/avro/
--rw-r--r--   0 runner    (1001) docker     (122)       75 2023-05-03 20:27:05.000000 openedx-events-7.1.0/openedx_events/event_bus/avro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2457 2023-05-03 20:27:05.000000 openedx-events-7.1.0/openedx_events/event_bus/avro/custom_serializers.py
--rw-r--r--   0 runner    (1001) docker     (122)     5772 2023-05-03 20:27:05.000000 openedx-events-7.1.0/openedx_events/event_bus/avro/deserializer.py
--rw-r--r--   0 runner    (1001) docker     (122)     5313 2023-05-03 20:27:05.000000 openedx-events-7.1.0/openedx_events/event_bus/avro/schema.py
--rw-r--r--   0 runner    (1001) docker     (122)     5277 2023-05-03 20:27:05.000000 openedx-events-7.1.0/openedx_events/event_bus/avro/serializer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 20:27:10.093215 openedx-events-7.1.0/openedx_events/event_bus/avro/tests/
--rw-r--r--   0 runner    (1001) docker     (122)       33 2023-05-03 20:27:05.000000 openedx-events-7.1.0/openedx_events/event_bus/avro/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4973 2023-05-03 20:27:05.000000 openedx-events-7.1.0/openedx_events/event_bus/avro/tests/test_avro.py
--rw-r--r--   0 runner    (1001) docker     (122)    11016 2023-05-03 20:27:05.000000 openedx-events-7.1.0/openedx_events/event_bus/avro/tests/test_deserializer.py
--rw-r--r--   0 runner    (1001) docker     (122)    11200 2023-05-03 20:27:05.000000 openedx-events-7.1.0/openedx_events/event_bus/avro/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (122)     8761 2023-05-03 20:27:05.000000 openedx-events-7.1.0/openedx_events/event_bus/avro/tests/test_serializer.py
--rw-r--r--   0 runner    (1001) docker     (122)     3632 2023-05-03 20:27:05.000000 openedx-events-7.1.0/openedx_events/event_bus/avro/tests/test_utilities.py
--rw-r--r--   0 runner    (1001) docker     (122)      365 2023-05-03 20:27:05.000000 openedx-events-7.1.0/openedx_events/event_bus/avro/types.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 20:27:10.093215 openedx-events-7.1.0/openedx_events/event_bus/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     4787 2023-05-03 20:27:05.000000 openedx-events-7.1.0/openedx_events/event_bus/tests/test_loader.py
--rw-r--r--   0 runner    (1001) docker     (122)     2014 2023-05-03 20:27:05.000000 openedx-events-7.1.0/openedx_events/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 20:27:10.093215 openedx-events-7.1.0/openedx_events/learning/
--rw-r--r--   0 runner    (1001) docker     (122)      167 2023-05-03 20:27:05.000000 openedx-events-7.1.0/openedx_events/learning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8297 2023-05-03 20:27:05.000000 openedx-events-7.1.0/openedx_events/learning/data.py
--rw-r--r--   0 runner    (1001) docker     (122)     5664 2023-05-03 20:27:05.000000 openedx-events-7.1.0/openedx_events/learning/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 20:27:10.093215 openedx-events-7.1.0/openedx_events/management/
--rw-r--r--   0 runner    (1001) docker     (122)       48 2023-05-03 20:27:05.000000 openedx-events-7.1.0/openedx_events/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 20:27:10.093215 openedx-events-7.1.0/openedx_events/management/commands/
--rw-r--r--   0 runner    (1001) docker     (122)       95 2023-05-03 20:27:05.000000 openedx-events-7.1.0/openedx_events/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2932 2023-05-03 20:27:05.000000 openedx-events-7.1.0/openedx_events/management/commands/consume_events.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 20:27:10.093215 openedx-events-7.1.0/openedx_events/tests/
--rw-r--r--   0 runner    (1001) docker     (122)       57 2023-05-03 20:27:05.000000 openedx-events-7.1.0/openedx_events/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2710 2023-05-03 20:27:05.000000 openedx-events-7.1.0/openedx_events/tests/test_consume_events_command.py
--rw-r--r--   0 runner    (1001) docker     (122)    14277 2023-05-03 20:27:05.000000 openedx-events-7.1.0/openedx_events/tests/test_tooling.py
--rw-r--r--   0 runner    (1001) docker     (122)     4264 2023-05-03 20:27:05.000000 openedx-events-7.1.0/openedx_events/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     9959 2023-05-03 20:27:05.000000 openedx-events-7.1.0/openedx_events/tooling.py
--rw-r--r--   0 runner    (1001) docker     (122)     3206 2023-05-03 20:27:05.000000 openedx-events-7.1.0/openedx_events/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 20:27:10.089215 openedx-events-7.1.0/openedx_events.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    14505 2023-05-03 20:27:10.000000 openedx-events-7.1.0/openedx_events.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1678 2023-05-03 20:27:10.000000 openedx-events-7.1.0/openedx_events.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-03 20:27:10.000000 openedx-events-7.1.0/openedx_events.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-03 20:27:10.000000 openedx-events-7.1.0/openedx_events.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       46 2023-05-03 20:27:10.000000 openedx-events-7.1.0/openedx_events.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-05-03 20:27:10.000000 openedx-events-7.1.0/openedx_events.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 20:27:10.093215 openedx-events-7.1.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      113 2023-05-03 20:27:05.000000 openedx-events-7.1.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      267 2023-05-03 20:27:10.093215 openedx-events-7.1.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     2831 2023-05-03 20:27:05.000000 openedx-events-7.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 20:27:10.093215 openedx-events-7.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      176 2023-05-03 20:27:05.000000 openedx-events-7.1.0/tests/test_openedx_events.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 18:35:45.389495 openedx-events-7.2.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     8596 2023-05-08 18:35:40.000000 openedx-events-7.2.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-05-08 18:35:40.000000 openedx-events-7.2.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      177 2023-05-08 18:35:40.000000 openedx-events-7.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    14622 2023-05-08 18:35:45.389495 openedx-events-7.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5366 2023-05-08 18:35:40.000000 openedx-events-7.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 18:35:45.385495 openedx-events-7.2.0/openedx_events/
+-rw-r--r--   0 runner    (1001) docker     (122)      217 2023-05-08 18:35:40.000000 openedx-events-7.2.0/openedx_events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      239 2023-05-08 18:35:40.000000 openedx-events-7.2.0/openedx_events/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 18:35:45.385495 openedx-events-7.2.0/openedx_events/content_authoring/
+-rw-r--r--   0 runner    (1001) docker     (122)      387 2023-05-08 18:35:40.000000 openedx-events-7.2.0/openedx_events/content_authoring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4493 2023-05-08 18:35:40.000000 openedx-events-7.2.0/openedx_events/content_authoring/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3615 2023-05-08 18:35:40.000000 openedx-events-7.2.0/openedx_events/content_authoring/signals.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3084 2023-05-08 18:35:40.000000 openedx-events-7.2.0/openedx_events/data.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 18:35:45.385495 openedx-events-7.2.0/openedx_events/event_bus/
+-rw-r--r--   0 runner    (1001) docker     (122)     7344 2023-05-08 18:35:40.000000 openedx-events-7.2.0/openedx_events/event_bus/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 18:35:45.389495 openedx-events-7.2.0/openedx_events/event_bus/avro/
+-rw-r--r--   0 runner    (1001) docker     (122)       75 2023-05-08 18:35:40.000000 openedx-events-7.2.0/openedx_events/event_bus/avro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2457 2023-05-08 18:35:40.000000 openedx-events-7.2.0/openedx_events/event_bus/avro/custom_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5772 2023-05-08 18:35:40.000000 openedx-events-7.2.0/openedx_events/event_bus/avro/deserializer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5353 2023-05-08 18:35:40.000000 openedx-events-7.2.0/openedx_events/event_bus/avro/schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5277 2023-05-08 18:35:40.000000 openedx-events-7.2.0/openedx_events/event_bus/avro/serializer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 18:35:45.389495 openedx-events-7.2.0/openedx_events/event_bus/avro/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       33 2023-05-08 18:35:40.000000 openedx-events-7.2.0/openedx_events/event_bus/avro/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4973 2023-05-08 18:35:40.000000 openedx-events-7.2.0/openedx_events/event_bus/avro/tests/test_avro.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11058 2023-05-08 18:35:40.000000 openedx-events-7.2.0/openedx_events/event_bus/avro/tests/test_deserializer.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11536 2023-05-08 18:35:40.000000 openedx-events-7.2.0/openedx_events/event_bus/avro/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8803 2023-05-08 18:35:40.000000 openedx-events-7.2.0/openedx_events/event_bus/avro/tests/test_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3632 2023-05-08 18:35:40.000000 openedx-events-7.2.0/openedx_events/event_bus/avro/tests/test_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (122)      365 2023-05-08 18:35:40.000000 openedx-events-7.2.0/openedx_events/event_bus/avro/types.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 18:35:45.389495 openedx-events-7.2.0/openedx_events/event_bus/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     4787 2023-05-08 18:35:40.000000 openedx-events-7.2.0/openedx_events/event_bus/tests/test_loader.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2014 2023-05-08 18:35:40.000000 openedx-events-7.2.0/openedx_events/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 18:35:45.389495 openedx-events-7.2.0/openedx_events/learning/
+-rw-r--r--   0 runner    (1001) docker     (122)      167 2023-05-08 18:35:40.000000 openedx-events-7.2.0/openedx_events/learning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8297 2023-05-08 18:35:40.000000 openedx-events-7.2.0/openedx_events/learning/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5664 2023-05-08 18:35:40.000000 openedx-events-7.2.0/openedx_events/learning/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 18:35:45.389495 openedx-events-7.2.0/openedx_events/management/
+-rw-r--r--   0 runner    (1001) docker     (122)       48 2023-05-08 18:35:40.000000 openedx-events-7.2.0/openedx_events/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 18:35:45.389495 openedx-events-7.2.0/openedx_events/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)       95 2023-05-08 18:35:40.000000 openedx-events-7.2.0/openedx_events/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2932 2023-05-08 18:35:40.000000 openedx-events-7.2.0/openedx_events/management/commands/consume_events.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 18:35:45.389495 openedx-events-7.2.0/openedx_events/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       57 2023-05-08 18:35:40.000000 openedx-events-7.2.0/openedx_events/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2710 2023-05-08 18:35:40.000000 openedx-events-7.2.0/openedx_events/tests/test_consume_events_command.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14277 2023-05-08 18:35:40.000000 openedx-events-7.2.0/openedx_events/tests/test_tooling.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4264 2023-05-08 18:35:40.000000 openedx-events-7.2.0/openedx_events/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9959 2023-05-08 18:35:40.000000 openedx-events-7.2.0/openedx_events/tooling.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3206 2023-05-08 18:35:40.000000 openedx-events-7.2.0/openedx_events/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 18:35:45.385495 openedx-events-7.2.0/openedx_events.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    14622 2023-05-08 18:35:45.000000 openedx-events-7.2.0/openedx_events.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1678 2023-05-08 18:35:45.000000 openedx-events-7.2.0/openedx_events.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-08 18:35:45.000000 openedx-events-7.2.0/openedx_events.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-08 18:35:45.000000 openedx-events-7.2.0/openedx_events.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       46 2023-05-08 18:35:45.000000 openedx-events-7.2.0/openedx_events.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-05-08 18:35:45.000000 openedx-events-7.2.0/openedx_events.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 18:35:45.389495 openedx-events-7.2.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      113 2023-05-08 18:35:40.000000 openedx-events-7.2.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      267 2023-05-08 18:35:45.393496 openedx-events-7.2.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2831 2023-05-08 18:35:40.000000 openedx-events-7.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 18:35:45.389495 openedx-events-7.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      176 2023-05-08 18:35:40.000000 openedx-events-7.2.0/tests/test_openedx_events.py
```

### Comparing `openedx-events-7.1.0/CHANGELOG.rst` & `openedx-events-7.2.0/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,20 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
 
+[7.2.0] - 2023-05-03
+--------------------
+Changed
+~~~~~~~
+* Added event type as namespace to generated Avro schemas
+
 
 [7.1.0] - 2023-05-03
 --------------------
 Added
 ~~~~~
 * Configurable loader for consumer side of Event Bus in ``openedx_events.event_bus``.
 * Added management command to load configured consumer and start worker.
```

### Comparing `openedx-events-7.1.0/LICENSE.txt` & `openedx-events-7.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `openedx-events-7.1.0/PKG-INFO` & `openedx-events-7.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openedx-events
-Version: 7.1.0
+Version: 7.2.0
 Summary: Open edX events from the Hooks Extensions Framework
 Home-page: https://github.com/openedx/openedx-events
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -206,14 +206,20 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
 
+[7.2.0] - 2023-05-03
+--------------------
+Changed
+~~~~~~~
+* Added event type as namespace to generated Avro schemas
+
 
 [7.1.0] - 2023-05-03
 --------------------
 Added
 ~~~~~
 * Configurable loader for consumer side of Event Bus in ``openedx_events.event_bus``.
 * Added management command to load configured consumer and start worker.
```

### Comparing `openedx-events-7.1.0/README.rst` & `openedx-events-7.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `openedx-events-7.1.0/openedx_events/content_authoring/data.py` & `openedx-events-7.2.0/openedx_events/content_authoring/data.py`

 * *Files identical despite different names*

### Comparing `openedx-events-7.1.0/openedx_events/content_authoring/signals.py` & `openedx-events-7.2.0/openedx_events/content_authoring/signals.py`

 * *Files identical despite different names*

### Comparing `openedx-events-7.1.0/openedx_events/data.py` & `openedx-events-7.2.0/openedx_events/data.py`

 * *Files identical despite different names*

### Comparing `openedx-events-7.1.0/openedx_events/event_bus/__init__.py` & `openedx-events-7.2.0/openedx_events/event_bus/__init__.py`

 * *Files identical despite different names*

### Comparing `openedx-events-7.1.0/openedx_events/event_bus/avro/custom_serializers.py` & `openedx-events-7.2.0/openedx_events/event_bus/avro/custom_serializers.py`

 * *Files identical despite different names*

### Comparing `openedx-events-7.1.0/openedx_events/event_bus/avro/deserializer.py` & `openedx-events-7.2.0/openedx_events/event_bus/avro/deserializer.py`

 * *Files identical despite different names*

### Comparing `openedx-events-7.1.0/openedx_events/event_bus/avro/schema.py` & `openedx-events-7.2.0/openedx_events/event_bus/avro/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     previously_seen_types = set()
 
     base_schema = {
         "name": "CloudEvent",
         "type": "record",
         "doc": "Avro Event Format for CloudEvents created with openedx_events/schema",
         "fields": [],
+        "namespace": signal.event_type,
     }
 
     for data_key, data_type in signal.init_data.items():
         base_schema["fields"].append(_create_avro_field_definition(data_key, data_type,
                                                                    previously_seen_types,
                                                                    custom_type_to_avro_type=all_custom_field_types))
     return base_schema
```

### Comparing `openedx-events-7.1.0/openedx_events/event_bus/avro/serializer.py` & `openedx-events-7.2.0/openedx_events/event_bus/avro/serializer.py`

 * *Files identical despite different names*

### Comparing `openedx-events-7.1.0/openedx_events/event_bus/avro/tests/test_avro.py` & `openedx-events-7.2.0/openedx_events/event_bus/avro/tests/test_avro.py`

 * *Files identical despite different names*

### Comparing `openedx-events-7.1.0/openedx_events/event_bus/avro/tests/test_deserializer.py` & `openedx-events-7.2.0/openedx_events/event_bus/avro/tests/test_deserializer.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,14 +37,15 @@
             "data": SimpleAttrs
         })
         actual_schema = json.loads(AvroSignalDeserializer(SIGNAL).schema_string())
         expected_schema = {
             'name': 'CloudEvent',
             'type': 'record',
             'doc': 'Avro Event Format for CloudEvents created with openedx_events/schema',
+            'namespace': 'simple.signal',
             'fields': [
                 {
                     'name': 'data',
                     'type': {
                         'name': 'SimpleAttrs',
                         'type': 'record',
                         'fields': [
```

### Comparing `openedx-events-7.1.0/openedx_events/event_bus/avro/tests/test_schema.py` & `openedx-events-7.2.0/openedx_events/event_bus/avro/tests/test_schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     def test_simple_schema_generation(self):
         SIGNAL = create_simple_signal({"event_data": SimpleAttrs})
         schema = schema_from_signal(SIGNAL)
         expected_dict = {
             "type": "record",
             "name": "CloudEvent",
             "doc": "Avro Event Format for CloudEvents created with openedx_events/schema",
+            'namespace': 'simple.signal',
             "fields": [
                 {"name": "event_data", "type":
                     {"name": "SimpleAttrs", "type": "record", "fields": [
                         {"name": "boolean_field", "type": "boolean"},
                         {"name": "int_field", "type": "long"},
                         {"name": "float_field", "type": "double"},
                         {"name": "bytes_field", "type": "bytes"},
@@ -54,14 +55,15 @@
         SIGNAL = create_simple_signal({"test_data": EventData})
         schema = schema_from_signal(SIGNAL)
 
         expected_dict = {
             "type": "record",
             "name": "CloudEvent",
             "doc": "Avro Event Format for CloudEvents created with openedx_events/schema",
+            'namespace': 'simple.signal',
             "fields": [
                 {"name": "test_data", "type":
                     {"name": "EventData", "type": "record", "fields": [
                         {"name": "sub_name", "type": "string"},
                         {"name": "course_id", "type": "string"},
                         {"name": "sub_test_0", "type": {
                             "name": "SubTestData0",
@@ -93,14 +95,15 @@
         })
         schema = schema_from_signal(SIGNAL)
 
         expected_dict = {
             "type": "record",
             "name": "CloudEvent",
             "doc": "Avro Event Format for CloudEvents created with openedx_events/schema",
+            'namespace': 'simple.signal',
             "fields": [
                 {"name": "top_level_key_0", "type":
                     {
                         "name": "SubTestData0",
                         "type": "record",
                         "fields": [
                             {"name": "sub_name", "type": "string"},
@@ -124,27 +127,29 @@
 
     def test_schema_for_custom_type(self):
         SIGNAL = create_simple_signal({"test_data": NonAttrs})
         expected_dict = {
             "type": "record",
             "name": "CloudEvent",
             "doc": "Avro Event Format for CloudEvents created with openedx_events/schema",
+            'namespace': 'simple.signal',
             "fields": [
                 {"name": "test_data", "type": "string"}
             ],
         }
         schema = schema_from_signal(SIGNAL, custom_type_to_avro_type={NonAttrs: "string"})
         self.assertDictEqual(schema, expected_dict)
 
     def test_schema_for_nested_custom_type(self):
         SIGNAL = create_simple_signal({"test_data": NestedNonAttrs})
         expected_dict = {
             "type": "record",
             "name": "CloudEvent",
             "doc": "Avro Event Format for CloudEvents created with openedx_events/schema",
+            'namespace': 'simple.signal',
             "fields": [
                 {"name": "test_data", "type": {
                     "name": "NestedNonAttrs",
                     "type": "record",
                     "fields": [
                         {'name': 'field_0', 'type': 'string'}
                     ]
@@ -156,14 +161,15 @@
 
     def test_schema_for_types_with_defaults(self):
         SIGNAL = create_simple_signal({"test_data": SimpleAttrsWithDefaults})
         expected_dict = {
             "type": "record",
             "name": "CloudEvent",
             "doc": "Avro Event Format for CloudEvents created with openedx_events/schema",
+            'namespace': 'simple.signal',
             "fields": [
                 {"name": "test_data", "type":
                     {"name": "SimpleAttrsWithDefaults", "type": "record", "fields": [
                         {"name": "boolean_field", "type": ["null", "boolean"], "default": None},
                         {"name": "int_field", "type": ["null", "long"], "default": None},
                         {"name": "float_field", "type": ["null", "double"], "default": None},
                         {"name": "bytes_field", "type": ["null", "bytes"], "default": None},
@@ -187,14 +193,15 @@
 
     def test_schema_for_types_with_nested_defaults(self):
         SIGNAL = create_simple_signal({"test_data": NestedAttrsWithDefaults})
         expected_dict = {
             'name': 'CloudEvent',
             'type': 'record',
             'doc': 'Avro Event Format for CloudEvents created with openedx_events/schema',
+            'namespace': 'simple.signal',
             'fields': [{
                 'name': 'test_data',
                 'type': {
                     'name': 'NestedAttrsWithDefaults',
                     'type': 'record',
                     'fields': [{
                         'name': 'field_0',
@@ -251,14 +258,15 @@
 
     def test_list_with_annotation_works(self):
         LIST_SIGNAL = create_simple_signal({"list_input": List[int]})
         expected_dict = {
             'name': 'CloudEvent',
             'type': 'record',
             'doc': 'Avro Event Format for CloudEvents created with openedx_events/schema',
+            'namespace': 'simple.signal',
             'fields': [{
                 'name': 'list_input',
                 'type': {'type': 'array', 'items': 'long'},
             }],
         }
         schema = schema_from_signal(LIST_SIGNAL)
         self.assertDictEqual(schema, expected_dict)
```

### Comparing `openedx-events-7.1.0/openedx_events/event_bus/avro/tests/test_serializer.py` & `openedx-events-7.2.0/openedx_events/event_bus/avro/tests/test_serializer.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,15 @@
             "data": SimpleAttrs
         })
         actual_schema = json.loads(AvroSignalSerializer(SIGNAL).schema_string())
         expected_schema = {
             'name': 'CloudEvent',
             'type': 'record',
             'doc': 'Avro Event Format for CloudEvents created with openedx_events/schema',
+            'namespace': 'simple.signal',
             'fields': [
                 {
                     'name': 'data',
                     'type': {
                         'name': 'SimpleAttrs',
                         'type': 'record',
                         'fields': [
```

### Comparing `openedx-events-7.1.0/openedx_events/event_bus/avro/tests/test_utilities.py` & `openedx-events-7.2.0/openedx_events/event_bus/avro/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `openedx-events-7.1.0/openedx_events/event_bus/tests/test_loader.py` & `openedx-events-7.2.0/openedx_events/event_bus/tests/test_loader.py`

 * *Files identical despite different names*

### Comparing `openedx-events-7.1.0/openedx_events/exceptions.py` & `openedx-events-7.2.0/openedx_events/exceptions.py`

 * *Files identical despite different names*

### Comparing `openedx-events-7.1.0/openedx_events/learning/data.py` & `openedx-events-7.2.0/openedx_events/learning/data.py`

 * *Files identical despite different names*

### Comparing `openedx-events-7.1.0/openedx_events/learning/signals.py` & `openedx-events-7.2.0/openedx_events/learning/signals.py`

 * *Files identical despite different names*

### Comparing `openedx-events-7.1.0/openedx_events/management/commands/consume_events.py` & `openedx-events-7.2.0/openedx_events/management/commands/consume_events.py`

 * *Files identical despite different names*

### Comparing `openedx-events-7.1.0/openedx_events/tests/test_consume_events_command.py` & `openedx-events-7.2.0/openedx_events/tests/test_consume_events_command.py`

 * *Files identical despite different names*

### Comparing `openedx-events-7.1.0/openedx_events/tests/test_tooling.py` & `openedx-events-7.2.0/openedx_events/tests/test_tooling.py`

 * *Files identical despite different names*

### Comparing `openedx-events-7.1.0/openedx_events/tests/utils.py` & `openedx-events-7.2.0/openedx_events/tests/utils.py`

 * *Files identical despite different names*

### Comparing `openedx-events-7.1.0/openedx_events/tooling.py` & `openedx-events-7.2.0/openedx_events/tooling.py`

 * *Files identical despite different names*

### Comparing `openedx-events-7.1.0/openedx_events/utils.py` & `openedx-events-7.2.0/openedx_events/utils.py`

 * *Files identical despite different names*

### Comparing `openedx-events-7.1.0/openedx_events.egg-info/PKG-INFO` & `openedx-events-7.2.0/openedx_events.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openedx-events
-Version: 7.1.0
+Version: 7.2.0
 Summary: Open edX events from the Hooks Extensions Framework
 Home-page: https://github.com/openedx/openedx-events
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -206,14 +206,20 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
 
+[7.2.0] - 2023-05-03
+--------------------
+Changed
+~~~~~~~
+* Added event type as namespace to generated Avro schemas
+
 
 [7.1.0] - 2023-05-03
 --------------------
 Added
 ~~~~~
 * Configurable loader for consumer side of Event Bus in ``openedx_events.event_bus``.
 * Added management command to load configured consumer and start worker.
```

### Comparing `openedx-events-7.1.0/openedx_events.egg-info/SOURCES.txt` & `openedx-events-7.2.0/openedx_events.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openedx-events-7.1.0/setup.py` & `openedx-events-7.2.0/setup.py`

 * *Files identical despite different names*

