# Comparing `tmp/sonnen_charger_modbus-0.1.4.tar.gz` & `tmp/sonnen_charger_modbus-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sonnen_charger_modbus-0.1.4.tar", last modified: Fri Mar 17 16:17:59 2023, max compression
+gzip compressed data, was "sonnen_charger_modbus-0.1.5.tar", last modified: Mon May  8 07:12:38 2023, max compression
```

## Comparing `sonnen_charger_modbus-0.1.4.tar` & `sonnen_charger_modbus-0.1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-03-17 16:17:59.006884 sonnen_charger_modbus-0.1.4/
--rw-rw-rw-   0        0        0     1070 2023-03-08 12:01:04.000000 sonnen_charger_modbus-0.1.4/LICENSE
--rw-rw-rw-   0        0        0     2247 2023-03-17 16:17:59.005883 sonnen_charger_modbus-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0      613 2023-03-08 12:08:07.000000 sonnen_charger_modbus-0.1.4/README.md
--rw-rw-rw-   0        0        0       42 2023-03-17 16:17:59.006884 sonnen_charger_modbus-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1052 2023-03-08 12:03:35.000000 sonnen_charger_modbus-0.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-17 16:17:58.980886 sonnen_charger_modbus-0.1.4/sonnen_charger_modbus/
--rw-rw-rw-   0        0        0      122 2023-03-17 16:17:54.000000 sonnen_charger_modbus-0.1.4/sonnen_charger_modbus/__init__.py
--rw-rw-rw-   0        0        0    16565 2023-03-17 15:29:19.000000 sonnen_charger_modbus-0.1.4/sonnen_charger_modbus/sonnencharger.py
-drwxrwxrwx   0        0        0        0 2023-03-17 16:17:59.004886 sonnen_charger_modbus-0.1.4/sonnen_charger_modbus.egg-info/
--rw-rw-rw-   0        0        0     2247 2023-03-17 16:17:58.000000 sonnen_charger_modbus-0.1.4/sonnen_charger_modbus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      323 2023-03-17 16:17:58.000000 sonnen_charger_modbus-0.1.4/sonnen_charger_modbus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-17 16:17:58.000000 sonnen_charger_modbus-0.1.4/sonnen_charger_modbus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-03-17 16:17:58.000000 sonnen_charger_modbus-0.1.4/sonnen_charger_modbus.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-03-17 16:17:58.000000 sonnen_charger_modbus-0.1.4/sonnen_charger_modbus.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-08 07:12:38.950090 sonnen_charger_modbus-0.1.5/
+-rw-rw-rw-   0        0        0     1070 2023-03-08 12:01:04.000000 sonnen_charger_modbus-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0     2373 2023-05-08 07:12:38.949081 sonnen_charger_modbus-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0      732 2023-05-08 07:12:24.000000 sonnen_charger_modbus-0.1.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-08 07:12:38.950090 sonnen_charger_modbus-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1052 2023-03-08 12:03:35.000000 sonnen_charger_modbus-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 07:12:38.926082 sonnen_charger_modbus-0.1.5/sonnen_charger_modbus/
+-rw-rw-rw-   0        0        0      122 2023-04-29 09:25:24.000000 sonnen_charger_modbus-0.1.5/sonnen_charger_modbus/__init__.py
+-rw-rw-rw-   0        0        0    16656 2023-04-29 09:35:05.000000 sonnen_charger_modbus-0.1.5/sonnen_charger_modbus/sonnencharger.py
+drwxrwxrwx   0        0        0        0 2023-05-08 07:12:38.947079 sonnen_charger_modbus-0.1.5/sonnen_charger_modbus.egg-info/
+-rw-rw-rw-   0        0        0     2373 2023-05-08 07:12:38.000000 sonnen_charger_modbus-0.1.5/sonnen_charger_modbus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      323 2023-05-08 07:12:38.000000 sonnen_charger_modbus-0.1.5/sonnen_charger_modbus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 07:12:38.000000 sonnen_charger_modbus-0.1.5/sonnen_charger_modbus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-05-08 07:12:38.000000 sonnen_charger_modbus-0.1.5/sonnen_charger_modbus.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-05-08 07:12:38.000000 sonnen_charger_modbus-0.1.5/sonnen_charger_modbus.egg-info/top_level.txt
```

### Comparing `sonnen_charger_modbus-0.1.4/LICENSE` & `sonnen_charger_modbus-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sonnen_charger_modbus-0.1.4/PKG-INFO` & `sonnen_charger_modbus-0.1.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sonnen_charger_modbus
-Version: 0.1.4
+Version: 0.1.5
 Summary: Allows to access Sonnen Charger (or any other ETREL INCH) using TCP Modbus
 Home-page: https://github.com/abauske/sonnen_charger_modbus
 Author: Adrian Bauske
 Author-email: adrian.bauske@gmail.com
 License: MIT License
         
         Copyright (c) 2023 Adrian Bauske
@@ -48,7 +48,14 @@
 except Exception as e:
     print('Error in Modbus communication:')
     traceback.print_exc()
     print(e)
 
 charger.close()
 ```
+
+## How to release (only for devs)
+```
+py -m build
+twine check dist/*
+twine upload -r sonnen-charger-modbus dist/*
+```
```

### Comparing `sonnen_charger_modbus-0.1.4/README.md` & `sonnen_charger_modbus-0.1.5/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -16,7 +16,14 @@
 except Exception as e:
     print('Error in Modbus communication:')
     traceback.print_exc()
     print(e)
 
 charger.close()
 ```
+
+## How to release (only for devs)
+```
+py -m build
+twine check dist/*
+twine upload -r sonnen-charger-modbus dist/*
+```
```

### Comparing `sonnen_charger_modbus-0.1.4/setup.py` & `sonnen_charger_modbus-0.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `sonnen_charger_modbus-0.1.4/sonnen_charger_modbus/sonnencharger.py` & `sonnen_charger_modbus-0.1.5/sonnen_charger_modbus/sonnencharger.py`

 * *Files 0% similar despite different names*

```diff
@@ -334,22 +334,24 @@
         self.client.write_registers(ADDR_PAUSE_CHARGING_BASE + connector * 100, [1])
 
     def setDepartureTime(self, departure: datetime.datetime, connector = 0):
         """ Set departure time for connector """
         seconds_since_1970 = time.mktime(departure.timetuple())
         self.client.write_registers(ADDR_SET_DEPARTURE_TIME_BASE + connector * 100, wrapInt64(seconds_since_1970), skip_encode=True)
 
-    def setCurrent(self, currentA, connector = 0, clamp = False):
+    def setCurrent(self, currentA, connector = 0, clamp = False) -> int:
         """ Set current setpoint in A for connector.
             If clamp is True then currentA is clamped
             between minimum (6A) and maximum (32A)
             charge current. Otherwise, a value of <6A
-            will result in not charging. """
+            will result in not charging.
+            :return: charging current commanded to charger"""
         currentA = currentA if not clamp else max(MIN_CHARGE_CURRENT, min(MAX_CHARGE_CURRENT, currentA))
         self.client.write_registers(ADDR_SET_CURRENT_SETPOINT_BASE + connector * 100, wrapFloat(currentA), skip_encode=True)
+        return currentA
 
     def cancelCurrentSetpoint(self, connector = 0):
         """ Cancel current setpoint for connector """
         self.client.write_registers(ADDR_CANCEL_CURRENT_SETPOINT_BASE + connector * 100, [1])
 
     def setPower(self, watt, connector = 0):
         """ Set power setpoint in W for connector """
```

### Comparing `sonnen_charger_modbus-0.1.4/sonnen_charger_modbus.egg-info/PKG-INFO` & `sonnen_charger_modbus-0.1.5/sonnen_charger_modbus.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sonnen-charger-modbus
-Version: 0.1.4
+Version: 0.1.5
 Summary: Allows to access Sonnen Charger (or any other ETREL INCH) using TCP Modbus
 Home-page: https://github.com/abauske/sonnen_charger_modbus
 Author: Adrian Bauske
 Author-email: adrian.bauske@gmail.com
 License: MIT License
         
         Copyright (c) 2023 Adrian Bauske
@@ -48,7 +48,14 @@
 except Exception as e:
     print('Error in Modbus communication:')
     traceback.print_exc()
     print(e)
 
 charger.close()
 ```
+
+## How to release (only for devs)
+```
+py -m build
+twine check dist/*
+twine upload -r sonnen-charger-modbus dist/*
+```
```

