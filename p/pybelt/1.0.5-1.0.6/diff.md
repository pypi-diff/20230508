# Comparing `tmp/pybelt-1.0.5.tar.gz` & `tmp/pybelt-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pybelt-1.0.5.tar", last modified: Tue Jan 31 09:48:48 2023, max compression
+gzip compressed data, was "dist\pybelt-1.0.6.tar", last modified: Mon May  8 14:04:18 2023, max compression
```

## Comparing `pybelt-1.0.5.tar` & `pybelt-1.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-01-31 09:48:48.000000 pybelt-1.0.5/
--rw-rw-rw-   0        0        0     2472 2023-01-31 09:48:48.000000 pybelt-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1636 2021-01-11 09:49:47.000000 pybelt-1.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-01-31 09:48:48.000000 pybelt-1.0.5/pybelt/
--rw-rw-rw-   0        0        0      112 2020-06-22 14:06:02.000000 pybelt-1.0.5/pybelt/__init__.py
--rw-rw-rw-   0        0        0    38999 2023-01-31 09:10:48.000000 pybelt-1.0.5/pybelt/_communication_interface.py
--rw-rw-rw-   0        0        0     8833 2023-01-05 13:18:44.000000 pybelt-1.0.5/pybelt/_gatt_profile.py
--rw-rw-rw-   0        0        0    59384 2023-01-06 13:19:56.000000 pybelt-1.0.5/pybelt/belt_controller.py
--rw-rw-rw-   0        0        0     3509 2023-01-04 13:32:18.000000 pybelt-1.0.5/pybelt/belt_scanner.py
-drwxrwxrwx   0        0        0        0 2023-01-31 09:48:48.000000 pybelt-1.0.5/pybelt.egg-info/
--rw-rw-rw-   0        0        0     2472 2023-01-31 09:48:48.000000 pybelt-1.0.5/pybelt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      294 2023-01-31 09:48:48.000000 pybelt-1.0.5/pybelt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-31 09:48:48.000000 pybelt-1.0.5/pybelt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-01-31 09:48:48.000000 pybelt-1.0.5/pybelt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-01-31 09:48:48.000000 pybelt-1.0.5/pybelt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-01-31 09:48:48.000000 pybelt-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0      759 2023-01-31 09:47:08.000000 pybelt-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 14:04:18.000000 pybelt-1.0.6/
+-rw-rw-rw-   0        0        0     2472 2023-05-08 14:04:18.000000 pybelt-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1636 2021-01-11 09:49:47.000000 pybelt-1.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-08 14:04:18.000000 pybelt-1.0.6/pybelt/
+-rw-rw-rw-   0        0        0      112 2020-06-22 14:06:02.000000 pybelt-1.0.6/pybelt/__init__.py
+-rw-rw-rw-   0        0        0    39138 2023-05-08 13:57:43.000000 pybelt-1.0.6/pybelt/_communication_interface.py
+-rw-rw-rw-   0        0        0     8833 2023-01-05 13:18:44.000000 pybelt-1.0.6/pybelt/_gatt_profile.py
+-rw-rw-rw-   0        0        0    59384 2023-01-06 13:19:56.000000 pybelt-1.0.6/pybelt/belt_controller.py
+-rw-rw-rw-   0        0        0     3509 2023-01-04 13:32:18.000000 pybelt-1.0.6/pybelt/belt_scanner.py
+drwxrwxrwx   0        0        0        0 2023-05-08 14:04:18.000000 pybelt-1.0.6/pybelt.egg-info/
+-rw-rw-rw-   0        0        0     2472 2023-05-08 14:04:17.000000 pybelt-1.0.6/pybelt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      294 2023-05-08 14:04:18.000000 pybelt-1.0.6/pybelt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 14:04:17.000000 pybelt-1.0.6/pybelt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-05-08 14:04:17.000000 pybelt-1.0.6/pybelt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-08 14:04:17.000000 pybelt-1.0.6/pybelt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-08 14:04:18.000000 pybelt-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      759 2023-05-08 14:03:54.000000 pybelt-1.0.6/setup.py
```

### Comparing `pybelt-1.0.5/PKG-INFO` & `pybelt-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybelt
-Version: 1.0.5
+Version: 1.0.6
 Summary: An Python library to control the feelSpace naviBelt from your application
 Home-page: https://github.com/feelSpace/pybelt
 Author: feelSpace GmbH
 Author-email: dev@feelspace.de
 License: UNKNOWN
 Description: # pyBelt
```

### Comparing `pybelt-1.0.5/README.md` & `pybelt-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pybelt-1.0.5/pybelt/_communication_interface.py` & `pybelt-1.0.6/pybelt/_communication_interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -392,15 +392,15 @@
                             self._flush_input()
                             # ignore byte
                     elif len(packet) == 1:
                         # Second byte is the data length
                         if ord(in_byte) <= 22:
                             packet.append(in_byte[0])
                         else:
-                            gatt_char = self._gatt_profile.get_char_from_handle(ord(packet[0]))
+                            gatt_char = self._gatt_profile.get_char_from_handle(packet[0])
                             if gatt_char is not None and gatt_char == self._gatt_profile.sensor_notification_char and \
                                     ord(in_byte) <= 244:
                                 # Data length extension supported on sensor notifications
                                 packet.append(in_byte[0])
                             else:
                                 # Incorrect length, clear received data
                                 self.logger.error("SerialPortListener: Incorrect packet length in packet header. (" +
@@ -681,20 +681,21 @@
         """
         for gatt_char in self._gatt_profile.characteristics:
             bleak_gatt_char = services.get_characteristic(gatt_char.uuid)
             if bleak_gatt_char is None:
                 self.logger.error("BleInterface: Characteristic not listed for UUID {}".format(gatt_char.uuid))
             # else: TODO Adds handles
         # TODO
-        is_new_profile = False
+        is_new_profile = True
         try:
             adv_uuids = self._device.metadata['uuids']
             for uuid in adv_uuids:
-                if "0000fe51-0000-1000-8000-00805f9b34fb" in uuid.lower():
-                    is_new_profile = True
+                if "65333333-a115-11e2-9e9a-0800200ca100" in uuid.lower() or \
+                        "65333333-a115-11e2-9e9a-0800200ca200" in uuid.lower():
+                    is_new_profile = False
                     break
         except:
             pass
         if is_new_profile:
             self._gatt_profile.set_char_handles("0000fe01-0000-1000-8000-00805f9b34fb", 8, 9)
             self._gatt_profile.set_char_handles("0000fe02-0000-1000-8000-00805f9b34fb", 10, 11, [12])
             self._gatt_profile.set_char_handles("0000fe03-0000-1000-8000-00805f9b34fb", 13, 14)
@@ -705,15 +706,15 @@
             self._gatt_profile.set_char_handles("0000fe0a-0000-1000-8000-00805f9b34fb", 32, 33)
             self._gatt_profile.set_char_handles("0000fe0b-0000-1000-8000-00805f9b34fb", 34, 35, [36])
             self._gatt_profile.set_char_handles("0000fe0c-0000-1000-8000-00805f9b34fb", 37, 38, [39])
             self._gatt_profile.set_char_handles("0000fe13-0000-1000-8000-00805f9b34fb", 41, 42)
             self._gatt_profile.set_char_handles("0000fe14-0000-1000-8000-00805f9b34fb", 43, 44, [45])
         else:
             self._gatt_profile = get_usb_gatt_profile()
-        self.logger.debug("TO BE COMPLETED!")
+        self.logger.debug("BLE interface, TBC: UUIDs should be used instead of characteristic handles!")
 
     # --------------------------------------------------------------- #
     # Bleak GATT client callback methods
 
     def _on_notification_received(self, attr_handle, data):
         """
         Callback for notifications.
```

### Comparing `pybelt-1.0.5/pybelt/_gatt_profile.py` & `pybelt-1.0.6/pybelt/_gatt_profile.py`

 * *Files identical despite different names*

### Comparing `pybelt-1.0.5/pybelt/belt_controller.py` & `pybelt-1.0.6/pybelt/belt_controller.py`

 * *Files identical despite different names*

### Comparing `pybelt-1.0.5/pybelt/belt_scanner.py` & `pybelt-1.0.6/pybelt/belt_scanner.py`

 * *Files identical despite different names*

### Comparing `pybelt-1.0.5/pybelt.egg-info/PKG-INFO` & `pybelt-1.0.6/pybelt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybelt
-Version: 1.0.5
+Version: 1.0.6
 Summary: An Python library to control the feelSpace naviBelt from your application
 Home-page: https://github.com/feelSpace/pybelt
 Author: feelSpace GmbH
 Author-email: dev@feelspace.de
 License: UNKNOWN
 Description: # pyBelt
```

### Comparing `pybelt-1.0.5/setup.py` & `pybelt-1.0.6/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pybelt",
-    version="1.0.5",
+    version="1.0.6",
     author="feelSpace GmbH",
     author_email="dev@feelspace.de",
     description="An Python library to control the feelSpace naviBelt from your application",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/feelSpace/pybelt",
     packages=setuptools.find_packages(),
```

