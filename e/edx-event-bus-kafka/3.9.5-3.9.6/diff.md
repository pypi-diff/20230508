# Comparing `tmp/edx_event_bus_kafka-3.9.5.tar.gz` & `tmp/edx_event_bus_kafka-3.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx_event_bus_kafka-3.9.5.tar", last modified: Mon Feb 27 20:10:09 2023, max compression
+gzip compressed data, was "edx_event_bus_kafka-3.9.6.tar", last modified: Tue Feb 28 20:46:40 2023, max compression
```

## Comparing `edx_event_bus_kafka-3.9.5.tar` & `edx_event_bus_kafka-3.9.6.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 20:10:09.729804 edx_event_bus_kafka-3.9.5/
--rw-r--r--   0 runner    (1001) docker     (122)    10829 2023-02-27 20:10:06.000000 edx_event_bus_kafka-3.9.5/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-02-27 20:10:06.000000 edx_event_bus_kafka-3.9.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      219 2023-02-27 20:10:06.000000 edx_event_bus_kafka-3.9.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    18223 2023-02-27 20:10:09.729804 edx_event_bus_kafka-3.9.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6701 2023-02-27 20:10:06.000000 edx_event_bus_kafka-3.9.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 20:10:09.725804 edx_event_bus_kafka-3.9.5/edx_event_bus_kafka/
--rw-r--r--   0 runner    (1001) docker     (122)      374 2023-02-27 20:10:06.000000 edx_event_bus_kafka-3.9.5/edx_event_bus_kafka/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      257 2023-02-27 20:10:06.000000 edx_event_bus_kafka-3.9.5/edx_event_bus_kafka/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 20:10:09.725804 edx_event_bus_kafka-3.9.5/edx_event_bus_kafka/internal/
--rw-r--r--   0 runner    (1001) docker     (122)      245 2023-02-27 20:10:06.000000 edx_event_bus_kafka-3.9.5/edx_event_bus_kafka/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5882 2023-02-27 20:10:06.000000 edx_event_bus_kafka-3.9.5/edx_event_bus_kafka/internal/config.py
--rw-r--r--   0 runner    (1001) docker     (122)    30355 2023-02-27 20:10:06.000000 edx_event_bus_kafka-3.9.5/edx_event_bus_kafka/internal/consumer.py
--rw-r--r--   0 runner    (1001) docker     (122)    14863 2023-02-27 20:10:06.000000 edx_event_bus_kafka-3.9.5/edx_event_bus_kafka/internal/producer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 20:10:09.729804 edx_event_bus_kafka-3.9.5/edx_event_bus_kafka/internal/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-27 20:10:06.000000 edx_event_bus_kafka-3.9.5/edx_event_bus_kafka/internal/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2566 2023-02-27 20:10:06.000000 edx_event_bus_kafka-3.9.5/edx_event_bus_kafka/internal/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (122)    30046 2023-02-27 20:10:06.000000 edx_event_bus_kafka-3.9.5/edx_event_bus_kafka/internal/tests/test_consumer.py
--rw-r--r--   0 runner    (1001) docker     (122)    18435 2023-02-27 20:10:06.000000 edx_event_bus_kafka-3.9.5/edx_event_bus_kafka/internal/tests/test_producer.py
--rw-r--r--   0 runner    (1001) docker     (122)     7613 2023-02-27 20:10:06.000000 edx_event_bus_kafka-3.9.5/edx_event_bus_kafka/internal/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     7386 2023-02-27 20:10:06.000000 edx_event_bus_kafka-3.9.5/edx_event_bus_kafka/internal/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 20:10:09.729804 edx_event_bus_kafka-3.9.5/edx_event_bus_kafka/management/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-27 20:10:06.000000 edx_event_bus_kafka-3.9.5/edx_event_bus_kafka/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 20:10:09.729804 edx_event_bus_kafka-3.9.5/edx_event_bus_kafka/management/commands/
--rw-r--r--   0 runner    (1001) docker     (122)      101 2023-02-27 20:10:06.000000 edx_event_bus_kafka-3.9.5/edx_event_bus_kafka/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      179 2023-02-27 20:10:06.000000 edx_event_bus_kafka-3.9.5/edx_event_bus_kafka/management/commands/consume_events.py
--rw-r--r--   0 runner    (1001) docker     (122)     2432 2023-02-27 20:10:06.000000 edx_event_bus_kafka-3.9.5/edx_event_bus_kafka/management/commands/produce_event.py
--rw-r--r--   0 runner    (1001) docker     (122)       49 2023-02-27 20:10:06.000000 edx_event_bus_kafka-3.9.5/edx_event_bus_kafka/models.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 20:10:09.725804 edx_event_bus_kafka-3.9.5/edx_event_bus_kafka/templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 20:10:09.729804 edx_event_bus_kafka-3.9.5/edx_event_bus_kafka/templates/edx_event_bus_kafka/
--rw-r--r--   0 runner    (1001) docker     (122)      662 2023-02-27 20:10:06.000000 edx_event_bus_kafka-3.9.5/edx_event_bus_kafka/templates/edx_event_bus_kafka/base.html
--rw-r--r--   0 runner    (1001) docker     (122)      339 2023-02-27 20:10:06.000000 edx_event_bus_kafka-3.9.5/edx_event_bus_kafka/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 20:10:09.725804 edx_event_bus_kafka-3.9.5/edx_event_bus_kafka.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    18223 2023-02-27 20:10:09.000000 edx_event_bus_kafka-3.9.5/edx_event_bus_kafka.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1232 2023-02-27 20:10:09.000000 edx_event_bus_kafka-3.9.5/edx_event_bus_kafka.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-02-27 20:10:09.000000 edx_event_bus_kafka-3.9.5/edx_event_bus_kafka.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-02-27 20:10:09.000000 edx_event_bus_kafka-3.9.5/edx_event_bus_kafka.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       58 2023-02-27 20:10:09.000000 edx_event_bus_kafka-3.9.5/edx_event_bus_kafka.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       20 2023-02-27 20:10:09.000000 edx_event_bus_kafka-3.9.5/edx_event_bus_kafka.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 20:10:09.729804 edx_event_bus_kafka-3.9.5/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      263 2023-02-27 20:10:06.000000 edx_event_bus_kafka-3.9.5/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      561 2023-02-27 20:10:06.000000 edx_event_bus_kafka-3.9.5/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)      156 2023-02-27 20:10:09.729804 edx_event_bus_kafka-3.9.5/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     5009 2023-02-27 20:10:06.000000 edx_event_bus_kafka-3.9.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-27 20:10:09.729804 edx_event_bus_kafka-3.9.5/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      189 2023-02-27 20:10:06.000000 edx_event_bus_kafka-3.9.5/tests/test_models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 20:46:40.609935 edx_event_bus_kafka-3.9.6/
+-rw-r--r--   0 runner    (1001) docker     (122)    10964 2023-02-28 20:46:37.000000 edx_event_bus_kafka-3.9.6/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-02-28 20:46:37.000000 edx_event_bus_kafka-3.9.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      219 2023-02-28 20:46:37.000000 edx_event_bus_kafka-3.9.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    18358 2023-02-28 20:46:40.609935 edx_event_bus_kafka-3.9.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6701 2023-02-28 20:46:37.000000 edx_event_bus_kafka-3.9.6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 20:46:40.605935 edx_event_bus_kafka-3.9.6/edx_event_bus_kafka/
+-rw-r--r--   0 runner    (1001) docker     (122)      374 2023-02-28 20:46:37.000000 edx_event_bus_kafka-3.9.6/edx_event_bus_kafka/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      257 2023-02-28 20:46:37.000000 edx_event_bus_kafka-3.9.6/edx_event_bus_kafka/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 20:46:40.605935 edx_event_bus_kafka-3.9.6/edx_event_bus_kafka/internal/
+-rw-r--r--   0 runner    (1001) docker     (122)      245 2023-02-28 20:46:37.000000 edx_event_bus_kafka-3.9.6/edx_event_bus_kafka/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5882 2023-02-28 20:46:37.000000 edx_event_bus_kafka-3.9.6/edx_event_bus_kafka/internal/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30625 2023-02-28 20:46:37.000000 edx_event_bus_kafka-3.9.6/edx_event_bus_kafka/internal/consumer.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14863 2023-02-28 20:46:37.000000 edx_event_bus_kafka-3.9.6/edx_event_bus_kafka/internal/producer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 20:46:40.605935 edx_event_bus_kafka-3.9.6/edx_event_bus_kafka/internal/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-28 20:46:37.000000 edx_event_bus_kafka-3.9.6/edx_event_bus_kafka/internal/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2566 2023-02-28 20:46:37.000000 edx_event_bus_kafka-3.9.6/edx_event_bus_kafka/internal/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30046 2023-02-28 20:46:37.000000 edx_event_bus_kafka-3.9.6/edx_event_bus_kafka/internal/tests/test_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18435 2023-02-28 20:46:37.000000 edx_event_bus_kafka-3.9.6/edx_event_bus_kafka/internal/tests/test_producer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7613 2023-02-28 20:46:37.000000 edx_event_bus_kafka-3.9.6/edx_event_bus_kafka/internal/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7386 2023-02-28 20:46:37.000000 edx_event_bus_kafka-3.9.6/edx_event_bus_kafka/internal/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 20:46:40.605935 edx_event_bus_kafka-3.9.6/edx_event_bus_kafka/management/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-28 20:46:37.000000 edx_event_bus_kafka-3.9.6/edx_event_bus_kafka/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 20:46:40.609935 edx_event_bus_kafka-3.9.6/edx_event_bus_kafka/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)      101 2023-02-28 20:46:37.000000 edx_event_bus_kafka-3.9.6/edx_event_bus_kafka/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      179 2023-02-28 20:46:37.000000 edx_event_bus_kafka-3.9.6/edx_event_bus_kafka/management/commands/consume_events.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2432 2023-02-28 20:46:37.000000 edx_event_bus_kafka-3.9.6/edx_event_bus_kafka/management/commands/produce_event.py
+-rw-r--r--   0 runner    (1001) docker     (122)       49 2023-02-28 20:46:37.000000 edx_event_bus_kafka-3.9.6/edx_event_bus_kafka/models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 20:46:40.601935 edx_event_bus_kafka-3.9.6/edx_event_bus_kafka/templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 20:46:40.609935 edx_event_bus_kafka-3.9.6/edx_event_bus_kafka/templates/edx_event_bus_kafka/
+-rw-r--r--   0 runner    (1001) docker     (122)      662 2023-02-28 20:46:37.000000 edx_event_bus_kafka-3.9.6/edx_event_bus_kafka/templates/edx_event_bus_kafka/base.html
+-rw-r--r--   0 runner    (1001) docker     (122)      339 2023-02-28 20:46:37.000000 edx_event_bus_kafka-3.9.6/edx_event_bus_kafka/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 20:46:40.605935 edx_event_bus_kafka-3.9.6/edx_event_bus_kafka.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    18358 2023-02-28 20:46:40.000000 edx_event_bus_kafka-3.9.6/edx_event_bus_kafka.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1232 2023-02-28 20:46:40.000000 edx_event_bus_kafka-3.9.6/edx_event_bus_kafka.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-02-28 20:46:40.000000 edx_event_bus_kafka-3.9.6/edx_event_bus_kafka.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-02-28 20:46:40.000000 edx_event_bus_kafka-3.9.6/edx_event_bus_kafka.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       58 2023-02-28 20:46:40.000000 edx_event_bus_kafka-3.9.6/edx_event_bus_kafka.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       20 2023-02-28 20:46:40.000000 edx_event_bus_kafka-3.9.6/edx_event_bus_kafka.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 20:46:40.609935 edx_event_bus_kafka-3.9.6/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      263 2023-02-28 20:46:37.000000 edx_event_bus_kafka-3.9.6/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      561 2023-02-28 20:46:37.000000 edx_event_bus_kafka-3.9.6/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      156 2023-02-28 20:46:40.609935 edx_event_bus_kafka-3.9.6/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5009 2023-02-28 20:46:37.000000 edx_event_bus_kafka-3.9.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-28 20:46:40.609935 edx_event_bus_kafka-3.9.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      189 2023-02-28 20:46:37.000000 edx_event_bus_kafka-3.9.6/tests/test_models.py
```

### Comparing `edx_event_bus_kafka-3.9.5/CHANGELOG.rst` & `edx_event_bus_kafka-3.9.6/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,20 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
 
+[3.9.6] - 2023-02-24
+********************
+Added
+=====
+* Add function tracing to the event consumption workflow for better monitoring.
+
 [3.9.5] - 2023-02-24
 ********************
 
 Fixed
 =====
 * ``consume_events`` command now loads all public signals so that the consumer can load signals by ``event_type`` even if their modules were not already imported
```

### Comparing `edx_event_bus_kafka-3.9.5/LICENSE.txt` & `edx_event_bus_kafka-3.9.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edx_event_bus_kafka-3.9.5/PKG-INFO` & `edx_event_bus_kafka-3.9.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edx_event_bus_kafka
-Version: 3.9.5
+Version: 3.9.6
 Summary: Kafka implementation for Open edX event bus.
 Home-page: https://github.com/openedx/event-bus-kafka
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -199,14 +199,20 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
 
+[3.9.6] - 2023-02-24
+********************
+Added
+=====
+* Add function tracing to the event consumption workflow for better monitoring.
+
 [3.9.5] - 2023-02-24
 ********************
 
 Fixed
 =====
 * ``consume_events`` command now loads all public signals so that the consumer can load signals by ``event_type`` even if their modules were not already imported
```

### Comparing `edx_event_bus_kafka-3.9.5/README.rst` & `edx_event_bus_kafka-3.9.6/README.rst`

 * *Files identical despite different names*

### Comparing `edx_event_bus_kafka-3.9.5/edx_event_bus_kafka/internal/config.py` & `edx_event_bus_kafka-3.9.6/edx_event_bus_kafka/internal/config.py`

 * *Files identical despite different names*

### Comparing `edx_event_bus_kafka-3.9.5/edx_event_bus_kafka/internal/consumer.py` & `edx_event_bus_kafka-3.9.6/edx_event_bus_kafka/internal/consumer.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import time
 import warnings
 from datetime import datetime
 
 from django.conf import settings
 from django.core.management.base import BaseCommand
 from django.db import connection
-from edx_django_utils.monitoring import record_exception, set_custom_attribute
+from edx_django_utils.monitoring import function_trace, record_exception, set_custom_attribute
 from edx_toggles.toggles import SettingToggle
 from openedx_events.event_bus.avro.deserializer import AvroSignalDeserializer
 from openedx_events.tooling import OpenEdxPublicSignal, load_all_signals
 
 from .config import get_full_topic, get_schema_registry_client, load_common_settings
 from .utils import (
     AUDIT_LOGGING_ENABLED,
@@ -269,19 +269,20 @@
                 if CONSECUTIVE_ERRORS_LIMIT and consecutive_errors >= CONSECUTIVE_ERRORS_LIMIT:
                     raise Exception(f"Too many consecutive errors, exiting ({consecutive_errors} in a row)")
 
                 msg = None
                 try:
                     msg = self.consumer.poll(timeout=CONSUMER_POLL_TIMEOUT)
                     if msg is not None:
-                        # Before processing, make sure our db connection is still active
-                        _reconnect_to_db_if_needed()
+                        with function_trace('_consume_indefinitely_consume_single_message'):
+                            # Before processing, make sure our db connection is still active
+                            _reconnect_to_db_if_needed()
 
-                        self.emit_signals_from_message(msg)
-                        consecutive_errors = 0
+                            self.emit_signals_from_message(msg)
+                            consecutive_errors = 0
 
                     self._add_message_monitoring(run_context=run_context, message=msg)
                 except Exception as e:  # pylint: disable=broad-except
                     consecutive_errors += 1
                     self.record_event_consuming_error(run_context, e, msg)
                     # Kill the infinite loop if the error is fatal for the consumer
                     _, kafka_error = self._get_kafka_message_and_error(message=msg, error=e)
@@ -319,14 +320,15 @@
         else:
             warnings.warn(
                 "Calling consume_indefinitely with offset_timestamp is deprecated; "
                 "please call reset_offsets_and_sleep_indefinitely directly instead."
             )
             self.reset_offsets_and_sleep_indefinitely(offset_timestamp)
 
+    @function_trace('emit_signals_from_message')
     def emit_signals_from_message(self, msg):
         """
         Determine the correct signal and send the event from the message.
 
         Arguments:
             msg (Message): Consumed message.
         """
@@ -359,15 +361,18 @@
                 f"Signal types do not match. Expected {self.signal.event_type}. "
                 f"Received message of type {event_type}."
             )
         try:
             event_metadata = _get_metadata_from_headers(headers)
         except Exception as e:
             raise UnusableMessageError(f"Error determining metadata from message headers: {e}") from e
-        send_results = self.signal.send_event_with_custom_metadata(event_metadata, **msg.value())
+
+        with function_trace('emit_signals_from_message_send_event_with_custom_metadata'):
+            send_results = self.signal.send_event_with_custom_metadata(event_metadata, **msg.value())
+
         # Raise an exception if any receivers errored out. This allows logging of the receivers
         # along with partition, offset, etc. in record_event_consuming_error. Hopefully the
         # receiver code is idempotent and we can just replay any messages that were involved.
         self._check_receiver_results(send_results)
 
         # At the very end, log that a message was processed successfully.
         # Since we're single-threaded, no other information is needed;
```

### Comparing `edx_event_bus_kafka-3.9.5/edx_event_bus_kafka/internal/producer.py` & `edx_event_bus_kafka-3.9.6/edx_event_bus_kafka/internal/producer.py`

 * *Files identical despite different names*

### Comparing `edx_event_bus_kafka-3.9.5/edx_event_bus_kafka/internal/tests/test_config.py` & `edx_event_bus_kafka-3.9.6/edx_event_bus_kafka/internal/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `edx_event_bus_kafka-3.9.5/edx_event_bus_kafka/internal/tests/test_consumer.py` & `edx_event_bus_kafka-3.9.6/edx_event_bus_kafka/internal/tests/test_consumer.py`

 * *Files identical despite different names*

### Comparing `edx_event_bus_kafka-3.9.5/edx_event_bus_kafka/internal/tests/test_producer.py` & `edx_event_bus_kafka-3.9.6/edx_event_bus_kafka/internal/tests/test_producer.py`

 * *Files identical despite different names*

### Comparing `edx_event_bus_kafka-3.9.5/edx_event_bus_kafka/internal/tests/test_utils.py` & `edx_event_bus_kafka-3.9.6/edx_event_bus_kafka/internal/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `edx_event_bus_kafka-3.9.5/edx_event_bus_kafka/internal/utils.py` & `edx_event_bus_kafka-3.9.6/edx_event_bus_kafka/internal/utils.py`

 * *Files identical despite different names*

### Comparing `edx_event_bus_kafka-3.9.5/edx_event_bus_kafka/management/commands/produce_event.py` & `edx_event_bus_kafka-3.9.6/edx_event_bus_kafka/management/commands/produce_event.py`

 * *Files identical despite different names*

### Comparing `edx_event_bus_kafka-3.9.5/edx_event_bus_kafka/templates/edx_event_bus_kafka/base.html` & `edx_event_bus_kafka-3.9.6/edx_event_bus_kafka/templates/edx_event_bus_kafka/base.html`

 * *Files identical despite different names*

### Comparing `edx_event_bus_kafka-3.9.5/edx_event_bus_kafka.egg-info/PKG-INFO` & `edx_event_bus_kafka-3.9.6/edx_event_bus_kafka.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edx-event-bus-kafka
-Version: 3.9.5
+Version: 3.9.6
 Summary: Kafka implementation for Open edX event bus.
 Home-page: https://github.com/openedx/event-bus-kafka
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -199,14 +199,20 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
 
+[3.9.6] - 2023-02-24
+********************
+Added
+=====
+* Add function tracing to the event consumption workflow for better monitoring.
+
 [3.9.5] - 2023-02-24
 ********************
 
 Fixed
 =====
 * ``consume_events`` command now loads all public signals so that the consumer can load signals by ``event_type`` even if their modules were not already imported
```

### Comparing `edx_event_bus_kafka-3.9.5/edx_event_bus_kafka.egg-info/SOURCES.txt` & `edx_event_bus_kafka-3.9.6/edx_event_bus_kafka.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edx_event_bus_kafka-3.9.5/requirements/constraints.txt` & `edx_event_bus_kafka-3.9.6/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `edx_event_bus_kafka-3.9.5/setup.py` & `edx_event_bus_kafka-3.9.6/setup.py`

 * *Files identical despite different names*

