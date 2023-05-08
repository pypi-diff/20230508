# Comparing `tmp/roboid-1.6.2.tar.gz` & `tmp/roboid-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\roboid-1.6.2.tar", last modified: Sat Sep 10 13:03:17 2022, max compression
+gzip compressed data, was "dist\roboid-1.6.3.tar", last modified: Mon May  8 03:06:55 2023, max compression
```

## Comparing `roboid-1.6.2.tar` & `roboid-1.6.3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2022-09-10 13:03:17.241660 roboid-1.6.2/
--rw-rw-rw-   0        0        0      802 2020-08-22 18:46:06.000000 roboid-1.6.2/LICENSE
--rw-rw-rw-   0        0        0      118 2020-08-27 07:49:02.000000 roboid-1.6.2/MANIFEST.in
--rw-rw-rw-   0        0        0      583 2022-09-10 13:03:17.241660 roboid-1.6.2/PKG-INFO
--rw-rw-rw-   0        0        0      196 2021-07-16 15:38:12.000000 roboid-1.6.2/README.md
--rw-rw-rw-   0        0        0       13 2022-08-16 21:06:30.000000 roboid-1.6.2/requirements.txt
-drwxrwxrwx   0        0        0        0 2022-09-10 13:03:17.226036 roboid-1.6.2/roboid/
--rw-rw-rw-   0        0        0     2489 2022-09-10 13:00:51.000000 roboid-1.6.2/roboid/__init__.py
--rw-rw-rw-   0        0        0    43482 2022-09-06 12:45:31.000000 roboid-1.6.2/roboid/albert_ai.py
--rw-rw-rw-   0        0        0    39296 2022-09-06 12:45:31.000000 roboid-1.6.2/roboid/albert_ai_roboid.py
--rw-rw-rw-   0        0        0    32240 2022-09-06 12:45:31.000000 roboid-1.6.2/roboid/beagle.py
--rw-rw-rw-   0        0        0    51790 2022-09-06 12:45:31.000000 roboid-1.6.2/roboid/beagle_roboid.py
--rw-rw-rw-   0        0        0     1054 2022-09-06 12:45:31.000000 roboid-1.6.2/roboid/connector.py
--rw-rw-rw-   0        0        0    25181 2022-09-06 12:45:31.000000 roboid-1.6.2/roboid/grid.py
--rw-rw-rw-   0        0        0    25768 2022-09-06 12:45:31.000000 roboid-1.6.2/roboid/hamster.py
--rw-rw-rw-   0        0        0    26191 2022-09-06 12:45:31.000000 roboid-1.6.2/roboid/hamster_roboid.py
--rw-rw-rw-   0        0        0    65291 2022-09-10 12:35:40.000000 roboid-1.6.2/roboid/hamster_s.py
--rw-rw-rw-   0        0        0    34484 2022-09-06 12:45:31.000000 roboid-1.6.2/roboid/hamster_s_roboid.py
--rw-rw-rw-   0        0        0     4839 2022-09-06 12:45:31.000000 roboid-1.6.2/roboid/keyboard.py
--rw-rw-rw-   0        0        0    17970 2022-09-06 12:45:31.000000 roboid-1.6.2/roboid/model.py
--rw-rw-rw-   0        0        0     9409 2022-09-06 12:48:38.000000 roboid-1.6.2/roboid/runner.py
--rw-rw-rw-   0        0        0     1270 2022-09-06 12:45:31.000000 roboid-1.6.2/roboid/scanner.py
--rw-rw-rw-   0        0        0    13718 2022-09-06 13:10:19.000000 roboid-1.6.2/roboid/serial_connector.py
--rw-rw-rw-   0        0        0     4839 2022-09-06 12:45:31.000000 roboid-1.6.2/roboid/serial_queue.py
--rw-rw-rw-   0        0        0    36958 2022-09-06 12:45:31.000000 roboid-1.6.2/roboid/turtle.py
--rw-rw-rw-   0        0        0    28613 2022-09-06 12:45:31.000000 roboid-1.6.2/roboid/turtle_roboid.py
--rw-rw-rw-   0        0        0     1132 2022-09-06 12:45:31.000000 roboid-1.6.2/roboid/util.py
--rw-rw-rw-   0        0        0    36730 2022-09-06 12:45:31.000000 roboid-1.6.2/roboid/zerone.py
--rw-rw-rw-   0        0        0    24208 2022-09-06 12:45:31.000000 roboid-1.6.2/roboid/zerone_roboid.py
-drwxrwxrwx   0        0        0        0 2022-09-10 13:03:17.241660 roboid-1.6.2/roboid.egg-info/
--rw-rw-rw-   0        0        0      583 2022-09-10 13:03:16.000000 roboid-1.6.2/roboid.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      692 2022-09-10 13:03:17.000000 roboid-1.6.2/roboid.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-10 13:03:16.000000 roboid-1.6.2/roboid.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-09-10 13:03:16.000000 roboid-1.6.2/roboid.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        9 2022-09-10 13:03:16.000000 roboid-1.6.2/roboid.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2022-09-10 13:03:16.000000 roboid-1.6.2/roboid.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2022-09-10 13:03:17.241660 roboid-1.6.2/setup.cfg
--rw-rw-rw-   0        0        0      582 2022-09-10 13:01:07.000000 roboid-1.6.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 03:06:55.547230 roboid-1.6.3/
+-rw-rw-rw-   0        0        0      802 2020-08-22 18:46:06.000000 roboid-1.6.3/LICENSE
+-rw-rw-rw-   0        0        0      118 2020-08-27 07:49:02.000000 roboid-1.6.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      583 2023-05-08 03:06:55.547230 roboid-1.6.3/PKG-INFO
+-rw-rw-rw-   0        0        0      196 2021-07-16 15:38:12.000000 roboid-1.6.3/README.md
+-rw-rw-rw-   0        0        0       13 2022-08-16 21:06:30.000000 roboid-1.6.3/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-05-08 03:06:55.517352 roboid-1.6.3/roboid/
+-rw-rw-rw-   0        0        0     2489 2022-09-10 13:00:51.000000 roboid-1.6.3/roboid/__init__.py
+-rw-rw-rw-   0        0        0    43482 2022-09-06 12:45:31.000000 roboid-1.6.3/roboid/albert_ai.py
+-rw-rw-rw-   0        0        0    39296 2022-09-06 12:45:31.000000 roboid-1.6.3/roboid/albert_ai_roboid.py
+-rw-rw-rw-   0        0        0    33110 2023-05-08 02:43:56.000000 roboid-1.6.3/roboid/beagle.py
+-rw-rw-rw-   0        0        0    52299 2023-05-08 02:55:25.000000 roboid-1.6.3/roboid/beagle_roboid.py
+-rw-rw-rw-   0        0        0     1054 2022-09-06 12:45:31.000000 roboid-1.6.3/roboid/connector.py
+-rw-rw-rw-   0        0        0    25181 2022-09-06 12:45:31.000000 roboid-1.6.3/roboid/grid.py
+-rw-rw-rw-   0        0        0    25768 2022-09-06 12:45:31.000000 roboid-1.6.3/roboid/hamster.py
+-rw-rw-rw-   0        0        0    26191 2022-09-06 12:45:31.000000 roboid-1.6.3/roboid/hamster_roboid.py
+-rw-rw-rw-   0        0        0    65291 2022-09-10 12:35:40.000000 roboid-1.6.3/roboid/hamster_s.py
+-rw-rw-rw-   0        0        0    34484 2022-09-06 12:45:31.000000 roboid-1.6.3/roboid/hamster_s_roboid.py
+-rw-rw-rw-   0        0        0     4839 2022-09-06 12:45:31.000000 roboid-1.6.3/roboid/keyboard.py
+-rw-rw-rw-   0        0        0    17970 2022-09-06 12:45:31.000000 roboid-1.6.3/roboid/model.py
+-rw-rw-rw-   0        0        0     9409 2022-09-06 12:48:38.000000 roboid-1.6.3/roboid/runner.py
+-rw-rw-rw-   0        0        0     1270 2022-09-06 12:45:31.000000 roboid-1.6.3/roboid/scanner.py
+-rw-rw-rw-   0        0        0    13718 2022-09-06 13:10:19.000000 roboid-1.6.3/roboid/serial_connector.py
+-rw-rw-rw-   0        0        0     4839 2022-09-06 12:45:31.000000 roboid-1.6.3/roboid/serial_queue.py
+-rw-rw-rw-   0        0        0    36958 2022-09-06 12:45:31.000000 roboid-1.6.3/roboid/turtle.py
+-rw-rw-rw-   0        0        0    28613 2022-09-06 12:45:31.000000 roboid-1.6.3/roboid/turtle_roboid.py
+-rw-rw-rw-   0        0        0     1132 2022-09-06 12:45:31.000000 roboid-1.6.3/roboid/util.py
+-rw-rw-rw-   0        0        0    36730 2022-09-06 12:45:31.000000 roboid-1.6.3/roboid/zerone.py
+-rw-rw-rw-   0        0        0    24208 2022-09-06 12:45:31.000000 roboid-1.6.3/roboid/zerone_roboid.py
+drwxrwxrwx   0        0        0        0 2023-05-08 03:06:55.545245 roboid-1.6.3/roboid.egg-info/
+-rw-rw-rw-   0        0        0      583 2023-05-08 03:06:55.000000 roboid-1.6.3/roboid.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      692 2023-05-08 03:06:55.000000 roboid-1.6.3/roboid.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 03:06:55.000000 roboid-1.6.3/roboid.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-08 03:06:55.000000 roboid-1.6.3/roboid.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        9 2023-05-08 03:06:55.000000 roboid-1.6.3/roboid.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-08 03:06:55.000000 roboid-1.6.3/roboid.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-05-08 03:06:55.549224 roboid-1.6.3/setup.cfg
+-rw-rw-rw-   0        0        0      582 2023-05-08 03:04:03.000000 roboid-1.6.3/setup.py
```

### Comparing `roboid-1.6.2/LICENSE` & `roboid-1.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `roboid-1.6.2/PKG-INFO` & `roboid-1.6.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roboid
-Version: 1.6.2
+Version: 1.6.3
 Summary: Python Package for Hamster, Hamster-S, Turtle, Albert Ai, Zerone, and Beagle
 Author: Kwang-Hyun Park
 Author-email: akaii@kw.ac.kr
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `roboid-1.6.2/roboid/__init__.py` & `roboid-1.6.3/roboid/__init__.py`

 * *Files identical despite different names*

### Comparing `roboid-1.6.2/roboid/albert_ai.py` & `roboid-1.6.3/roboid/albert_ai.py`

 * *Files identical despite different names*

### Comparing `roboid-1.6.2/roboid/albert_ai_roboid.py` & `roboid-1.6.3/roboid/albert_ai_roboid.py`

 * *Files identical despite different names*

### Comparing `roboid-1.6.2/roboid/beagle.py` & `roboid-1.6.3/roboid/beagle.py`

 * *Files 4% similar despite different names*

```diff
@@ -381,14 +381,18 @@
     MAGNETOMETER_ODR_30 = 0x80
 
     BATTERY_NORMAL = 3
     BATTERY_MIDDLE = 2
     BATTERY_LOW = 1
     BATTERY_EMPTY = 0
 
+    LIDAR_RAW = 0
+    LIDAR_ZERO = 1
+    LIDAR_TRUNC = 2
+
     _NOTES = {
         "c": NOTE_C_1,
         "c#": NOTE_C_SHARP_1,
         "db": NOTE_D_FLAT_1,
         "d": NOTE_D_1,
         "d#": NOTE_D_SHARP_1,
         "eb": NOTE_E_FLAT_1,
@@ -420,14 +424,20 @@
         "noise": 10,
         "chop": 11,
         "happy": 12,
         "angry": 13,
         "sad": 14,
         "sleep": 15
     }
+    _LIDAR_MODES = {
+        "raw": 0,
+        "zero": 1,
+        "trunc": 2,
+        "truncate": 2
+    }
     _robots = {}
 
     def __init__(self, index=0, port_name=None):
         if isinstance(index, str):
             index = 0
             port_name = index
         if index in Beagle._robots:
@@ -436,14 +446,15 @@
         Beagle._robots[index] = self
         super(Beagle, self).__init__(Beagle.ID, "Beagle", index)
         self._bpm = 60
         self._servo_output_a = 0
         self._servo_output_b = 0
         self._servo_output_c = 0
         self._lidar = [65535] * 360
+        self._lidar_chart = None
         self._init(port_name)
 
     def dispose(self):
         Beagle._robots[self.get_index()] = None
         self._roboid._dispose()
         Runner.unregister_robot(self)
 
@@ -932,14 +943,23 @@
 
     def battery_state(self):
         return self.read(Beagle.BATTERY_STATE)
 
     def charge_state(self):
         return self.read(Beagle.CHARGE_STATE)
 
+    def lidar_mode(self, mode):
+        if isinstance(mode, (int, float)):
+            if mode >= 0 and mode <= Beagle.LIDAR_TRUNC:
+                self._roboid._set_lidar_mode(int(mode))
+        elif isinstance(mode, str):
+            tmp = mode.lower()
+            if tmp in Beagle._LIDAR_MODES:
+                self._roboid._set_lidar_mode(Beagle._LIDAR_MODES[tmp])
+
     def _draw_lidar_chart(self):
         canvas = self._lidar_canvas
         width = 480
         height = 480
         scale = 0.25
         cx = width // 2
         cy = height // 2
@@ -968,19 +988,26 @@
                 rad = i * delta + math.pi / 2
                 x = 240 + scale * val * math.cos(rad)
                 y = 240 - scale * val * math.sin(rad)
                 if x + r >= 0 and x - r <= 480 and y + r >= 0 and y - r <= 480:
                     canvas.create_oval(x - r, y - r, x + r, y + r, fill='red', outline='red')
         canvas.after(10, self._draw_lidar_chart)
 
+    def _on_lidar_chart_closing(self):
+        if self._lidar_chart is not None:
+            self._lidar_chart.quit()
+            self._lidar_chart = None
+
     def _show_lidar_chart(self):
         import tkinter
-        window = tkinter.Tk()
+        self._lidar_chart = tkinter.Tk()
+        window = self._lidar_chart
         window.title('LiDAR Chart')
         window.resizable(False, False)
+        window.protocol("WM_DELETE_WINDOW", self._on_lidar_chart_closing)
         self._lidar_canvas = tkinter.Canvas(window, width=480, height=480, bg='white')
         self._lidar_canvas.pack()
         self._draw_lidar_chart()
         window.mainloop()
 
     def lidar_chart(self):
         import threading
```

### Comparing `roboid-1.6.2/roboid/beagle_roboid.py` & `roboid-1.6.3/roboid/beagle_roboid.py`

 * *Files 0% similar despite different names*

```diff
@@ -175,14 +175,15 @@
         self._accelerometer_listener = None
         self._accelerometer_interpolator = None
         self._raw_gyroscope_listener = None
         self._raw_gyroscope_interpolator = None
         self._gyroscope_listener = None
         self._gyroscope_interpolator = None
 
+        self._lidar_mode = 0
         self._lidar_arr = None
         self._lidar_values = [None, None, None, None]
         self._lidar_valid = [False, False, False, False]
         self._lidar_ready = False
         self._lidar_activated = False
         self._lidar_deactivating = False
         self._lidar_send_more_count = 0
@@ -368,14 +369,15 @@
         
         self._basic_packet = None
         self._imu_packet = None
         self._lidar_packet = None
         self._packet_sent = 0
         self._packet_received = 0
         
+        self._lidar_mode = 0
         if self._lidar_activated:
             self._lidar_activated = False
             self._lidar_deactivating = True
             self._enable_lidar_written = True
 
     def _request_motoring_data(self):
         with self._thread_lock:
@@ -951,14 +953,21 @@
                     self._resolution_device._put((packet[7] & 0xff) / 10.0)
                     sz = packet[9] & 0xff
                     sz |= (packet[10] & 0xff) << 8
                     arr = self._get_or_create_quadrant_array(quadrant-1, sz)
                     for i in range(sz):
                         value = packet[2 * i + 11] & 0xff
                         value |= (packet[2 * i + 12] & 0xff) << 8
+                        if value >= 65280 and value < 65535:
+                            if self._lidar_mode == Beagle.LIDAR_ZERO:
+                                value = 0
+                            elif self._lidar_mode == Beagle.LIDAR_TRUNC:
+                                value = 80
+                            else:
+                                value &= 0xff
                         arr[i] = value
                     self._lidar_valid[quadrant-1] = True
                     if quadrant == 4:
                         valid = True
                         for i in range(4):
                             if self._lidar_valid[i] == False or self._lidar_values[i] is None:
                                 valid = False
@@ -998,14 +1007,17 @@
         self._raw_gyroscope_listener = listener
         self._raw_gyroscope_interpolator = BeagleInterpolator(interpolation)
 
     def _set_gyroscope_listener(self, listener, interpolation=None):
         self._gyroscope_listener = listener
         self._gyroscope_interpolator = BeagleInterpolator(interpolation)
 
+    def _set_lidar_mode(self, mode):
+        self._lidar_mode = mode
+
     def _average_lidar(self, data, start, size):
         length = len(data)
         sumval = 0.0
         count = 0
         for i in range(start, start + size):
             val = data[i+length if i < 0 else i]
             if val != 65535:
```

### Comparing `roboid-1.6.2/roboid/connector.py` & `roboid-1.6.3/roboid/connector.py`

 * *Files identical despite different names*

### Comparing `roboid-1.6.2/roboid/grid.py` & `roboid-1.6.3/roboid/grid.py`

 * *Files identical despite different names*

### Comparing `roboid-1.6.2/roboid/hamster.py` & `roboid-1.6.3/roboid/hamster.py`

 * *Files identical despite different names*

### Comparing `roboid-1.6.2/roboid/hamster_roboid.py` & `roboid-1.6.3/roboid/hamster_roboid.py`

 * *Files identical despite different names*

### Comparing `roboid-1.6.2/roboid/hamster_s.py` & `roboid-1.6.3/roboid/hamster_s.py`

 * *Files identical despite different names*

### Comparing `roboid-1.6.2/roboid/hamster_s_roboid.py` & `roboid-1.6.3/roboid/hamster_s_roboid.py`

 * *Files identical despite different names*

### Comparing `roboid-1.6.2/roboid/keyboard.py` & `roboid-1.6.3/roboid/keyboard.py`

 * *Files identical despite different names*

### Comparing `roboid-1.6.2/roboid/model.py` & `roboid-1.6.3/roboid/model.py`

 * *Files identical despite different names*

### Comparing `roboid-1.6.2/roboid/runner.py` & `roboid-1.6.3/roboid/runner.py`

 * *Files identical despite different names*

### Comparing `roboid-1.6.2/roboid/scanner.py` & `roboid-1.6.3/roboid/scanner.py`

 * *Files identical despite different names*

### Comparing `roboid-1.6.2/roboid/serial_connector.py` & `roboid-1.6.3/roboid/serial_connector.py`

 * *Files identical despite different names*

### Comparing `roboid-1.6.2/roboid/serial_queue.py` & `roboid-1.6.3/roboid/serial_queue.py`

 * *Files identical despite different names*

### Comparing `roboid-1.6.2/roboid/turtle.py` & `roboid-1.6.3/roboid/turtle.py`

 * *Files identical despite different names*

### Comparing `roboid-1.6.2/roboid/turtle_roboid.py` & `roboid-1.6.3/roboid/turtle_roboid.py`

 * *Files identical despite different names*

### Comparing `roboid-1.6.2/roboid/util.py` & `roboid-1.6.3/roboid/util.py`

 * *Files identical despite different names*

### Comparing `roboid-1.6.2/roboid/zerone.py` & `roboid-1.6.3/roboid/zerone.py`

 * *Files identical despite different names*

### Comparing `roboid-1.6.2/roboid/zerone_roboid.py` & `roboid-1.6.3/roboid/zerone_roboid.py`

 * *Files identical despite different names*

### Comparing `roboid-1.6.2/roboid.egg-info/PKG-INFO` & `roboid-1.6.3/roboid.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roboid
-Version: 1.6.2
+Version: 1.6.3
 Summary: Python Package for Hamster, Hamster-S, Turtle, Albert Ai, Zerone, and Beagle
 Author: Kwang-Hyun Park
 Author-email: akaii@kw.ac.kr
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `roboid-1.6.2/roboid.egg-info/SOURCES.txt` & `roboid-1.6.3/roboid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `roboid-1.6.2/setup.py` & `roboid-1.6.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
 	name="roboid",
-	version="1.6.2",
+	version="1.6.3",
 	author="Kwang-Hyun Park",
 	author_email="akaii@kw.ac.kr",
 	description="Python Package for Hamster, Hamster-S, Turtle, Albert Ai, Zerone, and Beagle",
 	long_description=open("README.md").read(),
 	long_description_content_type="text/markdown",
 	install_requires=["pyserial"],
 	packages=find_packages(exclude=["examples", "tests"]),
```

