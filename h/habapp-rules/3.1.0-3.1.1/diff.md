# Comparing `tmp/habapp_rules-3.1.0.tar.gz` & `tmp/habapp_rules-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "habapp_rules-3.1.0.tar", last modified: Mon May  8 20:22:26 2023, max compression
+gzip compressed data, was "habapp_rules-3.1.1.tar", last modified: Mon May  8 21:13:51 2023, max compression
```

## Comparing `habapp_rules-3.1.0.tar` & `habapp_rules-3.1.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:22:26.313243 habapp_rules-3.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11339 2023-05-08 20:22:15.000000 habapp_rules-3.1.0/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-08 20:22:26.313243 habapp_rules-3.1.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:22:26.309243 habapp_rules-3.1.0/habapp_rules/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-08 20:22:15.000000 habapp_rules-3.1.0/habapp_rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-08 20:22:15.000000 habapp_rules-3.1.0/habapp_rules/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:22:26.309243 habapp_rules-3.1.0/habapp_rules/actors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 20:22:15.000000 habapp_rules-3.1.0/habapp_rules/actors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5914 2023-05-08 20:22:15.000000 habapp_rules-3.1.0/habapp_rules/actors/irrigation.py
--rw-r--r--   0 runner    (1001) docker     (123)    27402 2023-05-08 20:22:15.000000 habapp_rules-3.1.0/habapp_rules/actors/light.py
--rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-05-08 20:22:15.000000 habapp_rules-3.1.0/habapp_rules/actors/light_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    11368 2023-05-08 20:22:15.000000 habapp_rules-3.1.0/habapp_rules/actors/state_observer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:22:26.309243 habapp_rules-3.1.0/habapp_rules/bridge/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 20:22:15.000000 habapp_rules-3.1.0/habapp_rules/bridge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-05-08 20:22:15.000000 habapp_rules-3.1.0/habapp_rules/bridge/knx_mqtt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:22:26.309243 habapp_rules-3.1.0/habapp_rules/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 20:22:15.000000 habapp_rules-3.1.0/habapp_rules/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-05-08 20:22:15.000000 habapp_rules-3.1.0/habapp_rules/common/hysteresis.py
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-05-08 20:22:15.000000 habapp_rules-3.1.0/habapp_rules/common/logic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:22:26.309243 habapp_rules-3.1.0/habapp_rules/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 20:22:15.000000 habapp_rules-3.1.0/habapp_rules/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-08 20:22:15.000000 habapp_rules-3.1.0/habapp_rules/core/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-08 20:22:15.000000 habapp_rules-3.1.0/habapp_rules/core/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-05-08 20:22:15.000000 habapp_rules-3.1.0/habapp_rules/core/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-05-08 20:22:15.000000 habapp_rules-3.1.0/habapp_rules/core/state_machine_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-05-08 20:22:15.000000 habapp_rules-3.1.0/habapp_rules/core/timeout_list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:22:26.309243 habapp_rules-3.1.0/habapp_rules/sensors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 20:22:15.000000 habapp_rules-3.1.0/habapp_rules/sensors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12767 2023-05-08 20:22:15.000000 habapp_rules-3.1.0/habapp_rules/sensors/motion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:22:26.313243 habapp_rules-3.1.0/habapp_rules/system/
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-08 20:22:15.000000 habapp_rules-3.1.0/habapp_rules/system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8471 2023-05-08 20:22:15.000000 habapp_rules-3.1.0/habapp_rules/system/presence.py
--rw-r--r--   0 runner    (1001) docker     (123)     8984 2023-05-08 20:22:15.000000 habapp_rules-3.1.0/habapp_rules/system/sleep.py
--rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-05-08 20:22:15.000000 habapp_rules-3.1.0/habapp_rules/system/summer_winter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:22:26.309243 habapp_rules-3.1.0/habapp_rules.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-08 20:22:26.000000 habapp_rules-3.1.0/habapp_rules.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-05-08 20:22:26.000000 habapp_rules-3.1.0/habapp_rules.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 20:22:26.000000 habapp_rules-3.1.0/habapp_rules.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-08 20:22:26.000000 habapp_rules-3.1.0/habapp_rules.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-08 20:22:26.000000 habapp_rules-3.1.0/habapp_rules.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 20:22:26.313243 habapp_rules-3.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-08 20:22:15.000000 habapp_rules-3.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:13:51.589908 habapp_rules-3.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11339 2023-05-08 21:13:38.000000 habapp_rules-3.1.1/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-08 21:13:51.589908 habapp_rules-3.1.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:13:51.585908 habapp_rules-3.1.1/habapp_rules/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-08 21:13:38.000000 habapp_rules-3.1.1/habapp_rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-08 21:13:38.000000 habapp_rules-3.1.1/habapp_rules/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:13:51.585908 habapp_rules-3.1.1/habapp_rules/actors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 21:13:38.000000 habapp_rules-3.1.1/habapp_rules/actors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-05-08 21:13:38.000000 habapp_rules-3.1.1/habapp_rules/actors/irrigation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27402 2023-05-08 21:13:38.000000 habapp_rules-3.1.1/habapp_rules/actors/light.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-05-08 21:13:38.000000 habapp_rules-3.1.1/habapp_rules/actors/light_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11368 2023-05-08 21:13:38.000000 habapp_rules-3.1.1/habapp_rules/actors/state_observer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:13:51.589908 habapp_rules-3.1.1/habapp_rules/bridge/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 21:13:38.000000 habapp_rules-3.1.1/habapp_rules/bridge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-05-08 21:13:38.000000 habapp_rules-3.1.1/habapp_rules/bridge/knx_mqtt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:13:51.589908 habapp_rules-3.1.1/habapp_rules/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 21:13:38.000000 habapp_rules-3.1.1/habapp_rules/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-05-08 21:13:38.000000 habapp_rules-3.1.1/habapp_rules/common/hysteresis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-05-08 21:13:38.000000 habapp_rules-3.1.1/habapp_rules/common/logic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:13:51.589908 habapp_rules-3.1.1/habapp_rules/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 21:13:38.000000 habapp_rules-3.1.1/habapp_rules/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-08 21:13:38.000000 habapp_rules-3.1.1/habapp_rules/core/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-08 21:13:38.000000 habapp_rules-3.1.1/habapp_rules/core/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-05-08 21:13:38.000000 habapp_rules-3.1.1/habapp_rules/core/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-05-08 21:13:38.000000 habapp_rules-3.1.1/habapp_rules/core/state_machine_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-05-08 21:13:38.000000 habapp_rules-3.1.1/habapp_rules/core/timeout_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:13:51.589908 habapp_rules-3.1.1/habapp_rules/sensors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 21:13:38.000000 habapp_rules-3.1.1/habapp_rules/sensors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12767 2023-05-08 21:13:38.000000 habapp_rules-3.1.1/habapp_rules/sensors/motion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:13:51.589908 habapp_rules-3.1.1/habapp_rules/system/
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-08 21:13:38.000000 habapp_rules-3.1.1/habapp_rules/system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8471 2023-05-08 21:13:38.000000 habapp_rules-3.1.1/habapp_rules/system/presence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8984 2023-05-08 21:13:38.000000 habapp_rules-3.1.1/habapp_rules/system/sleep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-05-08 21:13:38.000000 habapp_rules-3.1.1/habapp_rules/system/summer_winter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:13:51.585908 habapp_rules-3.1.1/habapp_rules.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-08 21:13:51.000000 habapp_rules-3.1.1/habapp_rules.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-05-08 21:13:51.000000 habapp_rules-3.1.1/habapp_rules.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 21:13:51.000000 habapp_rules-3.1.1/habapp_rules.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-08 21:13:51.000000 habapp_rules-3.1.1/habapp_rules.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-08 21:13:51.000000 habapp_rules-3.1.1/habapp_rules.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 21:13:51.589908 habapp_rules-3.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-08 21:13:38.000000 habapp_rules-3.1.1/setup.py
```

### Comparing `habapp_rules-3.1.0/LICENCE` & `habapp_rules-3.1.1/LICENCE`

 * *Files identical despite different names*

### Comparing `habapp_rules-3.1.0/habapp_rules/actors/irrigation.py` & `habapp_rules-3.1.1/habapp_rules/actors/irrigation.py`

 * *Files 5% similar despite different names*

```diff
@@ -73,21 +73,24 @@
 			return False
 
 		if any(item.value is None for item in (self._item_hour, self._item_minute, self._item_duration)):
 			raise habapp_rules.core.exceptions.HabAppRulesException(
 				f"OpenHAB item values are not valid for hour / minute / duration. See current values: hour={self._item_hour.value} | minute={self._item_minute.value} | duration={self._item_duration.value}")
 
 		repetitions = self._item_repetitions.value if self._item_repetitions else 0
-		brake = self._item_brake.value if self._item_brake else 0
+		brake = int(self._item_brake.value) if self._item_brake else 0
 
 		now = datetime.datetime.now()
+		hour = int(self._item_hour.value)
+		minute = int(self._item_minute.value)
+		duration = int(self._item_duration.value)
 
 		for idx in range(repetitions + 1):
-			start_time = datetime.datetime.combine(date=now, time=datetime.time(self._item_hour.value, self._item_minute.value)) + datetime.timedelta(minutes=idx * (self._item_duration.value + brake))
-			end_time = start_time + datetime.timedelta(minutes=self._item_duration.value)
+			start_time = datetime.datetime.combine(date=now, time=datetime.time(hour, minute)) + datetime.timedelta(minutes=idx * (duration + brake))
+			end_time = start_time + datetime.timedelta(minutes=duration)
 			if self._is_in_time_range(start_time.time(), end_time.time(), now.time()):
 				return True
 		return False
 
 	@staticmethod
 	def _is_in_time_range(start_time: datetime.time, end_time: datetime.time, time_to_check: datetime.time) -> bool:
 		"""Check if a time is in a given range.
```

### Comparing `habapp_rules-3.1.0/habapp_rules/actors/light.py` & `habapp_rules-3.1.1/habapp_rules/actors/light.py`

 * *Files identical despite different names*

### Comparing `habapp_rules-3.1.0/habapp_rules/actors/light_config.py` & `habapp_rules-3.1.1/habapp_rules/actors/light_config.py`

 * *Files identical despite different names*

### Comparing `habapp_rules-3.1.0/habapp_rules/actors/state_observer.py` & `habapp_rules-3.1.1/habapp_rules/actors/state_observer.py`

 * *Files identical despite different names*

### Comparing `habapp_rules-3.1.0/habapp_rules/bridge/knx_mqtt.py` & `habapp_rules-3.1.1/habapp_rules/bridge/knx_mqtt.py`

 * *Files identical despite different names*

### Comparing `habapp_rules-3.1.0/habapp_rules/common/hysteresis.py` & `habapp_rules-3.1.1/habapp_rules/common/hysteresis.py`

 * *Files identical despite different names*

### Comparing `habapp_rules-3.1.0/habapp_rules/common/logic.py` & `habapp_rules-3.1.1/habapp_rules/common/logic.py`

 * *Files identical despite different names*

### Comparing `habapp_rules-3.1.0/habapp_rules/core/logger.py` & `habapp_rules-3.1.1/habapp_rules/core/logger.py`

 * *Files identical despite different names*

### Comparing `habapp_rules-3.1.0/habapp_rules/core/state_machine_rule.py` & `habapp_rules-3.1.1/habapp_rules/core/state_machine_rule.py`

 * *Files identical despite different names*

### Comparing `habapp_rules-3.1.0/habapp_rules/core/timeout_list.py` & `habapp_rules-3.1.1/habapp_rules/core/timeout_list.py`

 * *Files identical despite different names*

### Comparing `habapp_rules-3.1.0/habapp_rules/sensors/motion.py` & `habapp_rules-3.1.1/habapp_rules/sensors/motion.py`

 * *Files identical despite different names*

### Comparing `habapp_rules-3.1.0/habapp_rules/system/presence.py` & `habapp_rules-3.1.1/habapp_rules/system/presence.py`

 * *Files identical despite different names*

### Comparing `habapp_rules-3.1.0/habapp_rules/system/sleep.py` & `habapp_rules-3.1.1/habapp_rules/system/sleep.py`

 * *Files identical despite different names*

### Comparing `habapp_rules-3.1.0/habapp_rules/system/summer_winter.py` & `habapp_rules-3.1.1/habapp_rules/system/summer_winter.py`

 * *Files identical despite different names*

### Comparing `habapp_rules-3.1.0/habapp_rules.egg-info/SOURCES.txt` & `habapp_rules-3.1.1/habapp_rules.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `habapp_rules-3.1.0/setup.py` & `habapp_rules-3.1.1/setup.py`

 * *Files identical despite different names*

