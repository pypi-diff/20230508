# Comparing `tmp/zkaccess_c3-0.0.3.tar.gz` & `tmp/zkaccess_c3-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zkaccess_c3-0.0.3.tar", last modified: Wed May  3 20:57:42 2023, max compression
+gzip compressed data, was "zkaccess_c3-0.0.4.tar", last modified: Mon May  8 18:08:15 2023, max compression
```

## Comparing `zkaccess_c3-0.0.3.tar` & `zkaccess_c3-0.0.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 20:57:42.318217 zkaccess_c3-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-03 20:57:28.000000 zkaccess_c3-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-03 20:57:28.000000 zkaccess_c3-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-05-03 20:57:42.318217 zkaccess_c3-0.0.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 20:57:42.314217 zkaccess_c3-0.0.3/c3/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-03 20:57:28.000000 zkaccess_c3-0.0.3/c3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-05-03 20:57:28.000000 zkaccess_c3-0.0.3/c3/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4203 2023-05-03 20:57:28.000000 zkaccess_c3-0.0.3/c3/controldevice.py
--rw-r--r--   0 runner    (1001) docker     (123)    13378 2023-05-03 20:57:28.000000 zkaccess_c3-0.0.3/c3/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-05-03 20:57:28.000000 zkaccess_c3-0.0.3/c3/crc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7494 2023-05-03 20:57:28.000000 zkaccess_c3-0.0.3/c3/rtlog.py
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-05-03 20:57:28.000000 zkaccess_c3-0.0.3/c3/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 20:57:42.314217 zkaccess_c3-0.0.3/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-03 20:57:28.000000 zkaccess_c3-0.0.3/cli/C3_CancelAlarms.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-03 20:57:28.000000 zkaccess_c3-0.0.3/cli/C3_Discover.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-05-03 20:57:28.000000 zkaccess_c3-0.0.3/cli/C3_GetDeviceParam.py
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-05-03 20:57:28.000000 zkaccess_c3-0.0.3/cli/C3_GetRTLog.py
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-05-03 20:57:28.000000 zkaccess_c3-0.0.3/cli/C3_OutputOperation.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-03 20:57:28.000000 zkaccess_c3-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     5934 2023-05-03 20:57:28.000000 zkaccess_c3-0.0.3/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 20:57:42.318217 zkaccess_c3-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 20:57:28.000000 zkaccess_c3-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 20:57:42.318217 zkaccess_c3-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-03 20:57:28.000000 zkaccess_c3-0.0.3/tests/test_consts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-03 20:57:28.000000 zkaccess_c3-0.0.3/tests/test_controldevice.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-03 20:57:28.000000 zkaccess_c3-0.0.3/tests/test_crc16.py
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-05-03 20:57:28.000000 zkaccess_c3-0.0.3/tests/test_rtlog.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-03 20:57:28.000000 zkaccess_c3-0.0.3/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 20:57:42.318217 zkaccess_c3-0.0.3/zkaccess_c3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-05-03 20:57:42.000000 zkaccess_c3-0.0.3/zkaccess_c3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-03 20:57:42.000000 zkaccess_c3-0.0.3/zkaccess_c3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 20:57:42.000000 zkaccess_c3-0.0.3/zkaccess_c3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-03 20:57:42.000000 zkaccess_c3-0.0.3/zkaccess_c3.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:08:15.823472 zkaccess_c3-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-08 18:08:04.000000 zkaccess_c3-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-08 18:08:04.000000 zkaccess_c3-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-05-08 18:08:15.823472 zkaccess_c3-0.0.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:08:15.819472 zkaccess_c3-0.0.4/c3/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-08 18:08:04.000000 zkaccess_c3-0.0.4/c3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-05-08 18:08:04.000000 zkaccess_c3-0.0.4/c3/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4203 2023-05-08 18:08:04.000000 zkaccess_c3-0.0.4/c3/controldevice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13544 2023-05-08 18:08:04.000000 zkaccess_c3-0.0.4/c3/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-05-08 18:08:04.000000 zkaccess_c3-0.0.4/c3/crc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7638 2023-05-08 18:08:04.000000 zkaccess_c3-0.0.4/c3/rtlog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-05-08 18:08:04.000000 zkaccess_c3-0.0.4/c3/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:08:15.823472 zkaccess_c3-0.0.4/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-08 18:08:04.000000 zkaccess_c3-0.0.4/cli/C3_CancelAlarms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-08 18:08:04.000000 zkaccess_c3-0.0.4/cli/C3_Discover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-05-08 18:08:04.000000 zkaccess_c3-0.0.4/cli/C3_GetDeviceParam.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-05-08 18:08:04.000000 zkaccess_c3-0.0.4/cli/C3_GetRTLog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-05-08 18:08:04.000000 zkaccess_c3-0.0.4/cli/C3_OutputOperation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-08 18:08:04.000000 zkaccess_c3-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     5934 2023-05-08 18:08:04.000000 zkaccess_c3-0.0.4/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 18:08:15.823472 zkaccess_c3-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 18:08:04.000000 zkaccess_c3-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:08:15.823472 zkaccess_c3-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-08 18:08:04.000000 zkaccess_c3-0.0.4/tests/test_consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-08 18:08:04.000000 zkaccess_c3-0.0.4/tests/test_controldevice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-08 18:08:04.000000 zkaccess_c3-0.0.4/tests/test_crc16.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-05-08 18:08:04.000000 zkaccess_c3-0.0.4/tests/test_rtlog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-08 18:08:04.000000 zkaccess_c3-0.0.4/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:08:15.823472 zkaccess_c3-0.0.4/zkaccess_c3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-05-08 18:08:15.000000 zkaccess_c3-0.0.4/zkaccess_c3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-08 18:08:15.000000 zkaccess_c3-0.0.4/zkaccess_c3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 18:08:15.000000 zkaccess_c3-0.0.4/zkaccess_c3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-08 18:08:15.000000 zkaccess_c3-0.0.4/zkaccess_c3.egg-info/top_level.txt
```

### Comparing `zkaccess_c3-0.0.3/LICENSE` & `zkaccess_c3-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `zkaccess_c3-0.0.3/PKG-INFO` & `zkaccess_c3-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zkaccess_c3
-Version: 0.0.3
+Version: 0.0.4
 Summary: A native Python library for communicating with the ZKAccess C3 Access Control Panels.
 Author-email: Vwout <vwout@users.noreply.github.com>
 Project-URL: Homepage, https://github.com/vwout/zkaccess-c3-py
 Project-URL: Bug Tracker, https://github.com/vwout/zkaccess-c3-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `zkaccess_c3-0.0.3/c3/consts.py` & `zkaccess_c3-0.0.4/c3/consts.py`

 * *Files identical despite different names*

### Comparing `zkaccess_c3-0.0.3/c3/controldevice.py` & `zkaccess_c3-0.0.4/c3/controldevice.py`

 * *Files identical despite different names*

### Comparing `zkaccess_c3-0.0.3/c3/core.py` & `zkaccess_c3-0.0.4/c3/core.py`

 * *Files 8% similar despite different names*

```diff
@@ -135,15 +135,15 @@
                 session_id = (receive_data[1] << 8) + receive_data[0]
                 # msg_seq = (receive_data[3] << 8) + receive_data[2]
                 if self._session_id != session_id:
                     raise ValueError("Data received with invalid session ID")
 
         return receive_data[4:], bytes_received-4
 
-    def _is_connected(self) -> bool:
+    def is_connected(self) -> bool:
         # try:
         #    # this will try to read bytes without blocking and also without removing them from buffer (peek only)
         #    data = self._sock.recv(1, socket.MSG_DONTWAIT | socket.MSG_PEEK)
         #    if len(data) == 0:
         #        return True
         # except BlockingIOError:
         #    return True  # socket is open and reading from it would block
@@ -176,26 +176,26 @@
 
     @property
     def host(self) -> str:
         return self._host
 
     @host.setter
     def host(self, host: str):
-        if not self._is_connected():
+        if not self.is_connected():
             self._host = host
         else:
             raise ConnectionError("Cannot set host when C3 is connected. Disconnect first.")
 
     @property
     def port(self) -> int:
         return self._port
 
     @port.setter
     def port(self, port: int):
-        if not self._is_connected():
+        if not self.is_connected():
             self._port = port
         else:
             raise ConnectionError("Cannot set port when C3 is connected. Disconnect first.")
 
     @property
     def mac(self) -> str:
         return self._mac or '?'
@@ -285,47 +285,50 @@
                     self._session_id = (receive_data[1] << 8) + receive_data[0]
                     self.log.debug("Connected with Session ID %x", self._session_id)
                     self._connected = True
         except Exception as e:
             self.log.error(f"Connection to {self._host} failed: {e}")
 
         if self._connected:
-            params = self.get_device_param(["~SerialNumber", "LockCount", "AuxInCount", "AuxOutCount"])
-            self._sn = int(params.get("~SerialNumber", self._sn))
-            self._nr_of_locks = int(params.get("LockCount", self._nr_of_locks))
-            self._nr_aux_in = int(params.get("AuxInCount", self._nr_aux_in))
-            self._nr_aux_out = int(params.get("AuxOutCount", self._nr_aux_out))
+            try:
+                params = self.get_device_param(["~SerialNumber", "LockCount", "AuxInCount", "AuxOutCount"])
+                self._sn = int(params.get("~SerialNumber", self._sn))
+                self._nr_of_locks = int(params.get("LockCount", self._nr_of_locks))
+                self._nr_aux_in = int(params.get("AuxInCount", self._nr_aux_in))
+                self._nr_aux_out = int(params.get("AuxOutCount", self._nr_aux_out))
+            except Exception as e:
+                self.log.error(f"Retrieving configuration parameters from {self._host} failed: {e}")
 
         return self._connected
 
     def disconnect(self):
         """Disconnect from C3 panel and end session."""
-        if self._is_connected():
+        if self.is_connected():
             self._send_receive(consts.Command.DISCONNECT)
             self._sock.close()
 
         self._connected = False
         self._session_id = 0
         self._request_nr = 0
 
     def get_device_param(self, request_parameters: list[str]) -> dict:
         """Retrieve the requested device parameter values."""
-        if self._is_connected():
+        if self.is_connected():
             message, _ = self._send_receive(consts.Command.GETPARAM, ','.join(request_parameters))
             parameter_values = self._parse_kv_from_message(message)
         else:
             raise ConnectionError("No connection to C3 panel.")
 
         return parameter_values
 
     def get_rt_log(self) -> list[rtlog.RTLogRecord]:
         """Retrieve the latest event or alarm records."""
         records = []
 
-        if self._is_connected():
+        if self.is_connected():
             message, message_length = self._send_receive(consts.Command.RTLOG)
 
             # One RT log is 16 bytes
             # Ensure the array is not empty and a multiple of 16
             if message_length % 16 == 0:
                 logs_messages = [message[i:i+16] for i in range(0, message_length, 16)]
                 for log_message in logs_messages:
@@ -339,11 +342,11 @@
         else:
             raise ConnectionError("No connection to C3 panel.")
 
         return records
 
     def control_device(self, control_command: controldevice.ControlDeviceBase):
         """Send a control command to the panel."""
-        if self._is_connected():
+        if self.is_connected():
             self._send_receive(consts.Command.CONTROL, control_command.to_bytes())
         else:
             raise ConnectionError("No connection to C3 panel.")
```

### Comparing `zkaccess_c3-0.0.3/c3/crc.py` & `zkaccess_c3-0.0.4/c3/crc.py`

 * *Files identical despite different names*

### Comparing `zkaccess_c3-0.0.3/c3/rtlog.py` & `zkaccess_c3-0.0.4/c3/rtlog.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,20 +76,23 @@
 
         return alarms
 
     def has_alarm(self, door_nr: int, status: consts.AlarmStatus = None):
         return ((self.alarm_status[door_nr-1] & (status or 0)) == status) or \
                ((self.alarm_status[door_nr-1] > 0) and status is None)
 
+    def door_sensor_status(self, door_nr: int) -> consts.DoorSensorStatus:
+        return consts.DoorSensorStatus(self.dss_status[door_nr-1] & 0x0F)
+
     def door_is_open(self, door_nr: int):
         is_open = None
 
-        if (self.dss_status[door_nr-1] & 0x0F) == consts.DoorSensorStatus.OPEN:
+        if self.door_sensor_status(door_nr) == consts.DoorSensorStatus.OPEN:
             is_open = True
-        elif (self.dss_status[door_nr-1] & 0x0F) == consts.DoorSensorStatus.CLOSED:
+        elif self.door_sensor_status(door_nr) == consts.DoorSensorStatus.CLOSED:
             is_open = False
 
         return is_open
 
     def __repr__(self):
         repr_arr = ["Door/Alarm Realtime Status:",
                     "%-12s %-10s" % ("time_second", self.time_second),
```

### Comparing `zkaccess_c3-0.0.3/c3/utils.py` & `zkaccess_c3-0.0.4/c3/utils.py`

 * *Files identical despite different names*

### Comparing `zkaccess_c3-0.0.3/cli/C3_CancelAlarms.py` & `zkaccess_c3-0.0.4/cli/C3_CancelAlarms.py`

 * *Files identical despite different names*

### Comparing `zkaccess_c3-0.0.3/cli/C3_Discover.py` & `zkaccess_c3-0.0.4/cli/C3_Discover.py`

 * *Files identical despite different names*

### Comparing `zkaccess_c3-0.0.3/cli/C3_GetDeviceParam.py` & `zkaccess_c3-0.0.4/cli/C3_GetDeviceParam.py`

 * *Files identical despite different names*

### Comparing `zkaccess_c3-0.0.3/cli/C3_GetRTLog.py` & `zkaccess_c3-0.0.4/cli/C3_GetRTLog.py`

 * *Files identical despite different names*

### Comparing `zkaccess_c3-0.0.3/cli/C3_OutputOperation.py` & `zkaccess_c3-0.0.4/cli/C3_OutputOperation.py`

 * *Files identical despite different names*

### Comparing `zkaccess_c3-0.0.3/pyproject.toml` & `zkaccess_c3-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "zkaccess_c3"
-version = "0.0.3"
+version = "0.0.4"
 description = "A native Python library for communicating with the ZKAccess C3 Access Control Panels."
 authors = [
     {name = "Vwout", email="vwout@users.noreply.github.com"},
 ]
 #license = "GPL-3.0-or-later"
 readme = "readme.md"
 requires-python = ">=3.7"
```

### Comparing `zkaccess_c3-0.0.3/readme.md` & `zkaccess_c3-0.0.4/readme.md`

 * *Files identical despite different names*

### Comparing `zkaccess_c3-0.0.3/tests/test_controldevice.py` & `zkaccess_c3-0.0.4/tests/test_controldevice.py`

 * *Files identical despite different names*

### Comparing `zkaccess_c3-0.0.3/tests/test_crc16.py` & `zkaccess_c3-0.0.4/tests/test_crc16.py`

 * *Files identical despite different names*

### Comparing `zkaccess_c3-0.0.3/tests/test_rtlog.py` & `zkaccess_c3-0.0.4/tests/test_rtlog.py`

 * *Files identical despite different names*

### Comparing `zkaccess_c3-0.0.3/tests/test_utils.py` & `zkaccess_c3-0.0.4/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `zkaccess_c3-0.0.3/zkaccess_c3.egg-info/PKG-INFO` & `zkaccess_c3-0.0.4/zkaccess_c3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zkaccess-c3
-Version: 0.0.3
+Version: 0.0.4
 Summary: A native Python library for communicating with the ZKAccess C3 Access Control Panels.
 Author-email: Vwout <vwout@users.noreply.github.com>
 Project-URL: Homepage, https://github.com/vwout/zkaccess-c3-py
 Project-URL: Bug Tracker, https://github.com/vwout/zkaccess-c3-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

