# Comparing `tmp/durin-0.0.76.tar.gz` & `tmp/durin-0.0.77.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "durin-0.0.76.tar", last modified: Fri May  5 09:17:32 2023, max compression
+gzip compressed data, was "durin-0.0.77.tar", last modified: Mon May  8 11:25:23 2023, max compression
```

## Comparing `durin-0.0.76.tar` & `durin-0.0.77.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:17:32.362083 durin-0.0.76/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-05 09:17:23.000000 durin-0.0.76/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-05-05 09:17:32.362083 durin-0.0.76/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     2683 2023-05-05 09:17:23.000000 durin-0.0.76/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:17:32.358083 durin-0.0.76/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)       34 2023-05-05 09:17:23.000000 durin-0.0.76/bin/durin
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:17:32.358083 durin-0.0.76/durin/
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-05 09:17:23.000000 durin-0.0.76/durin/Profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-05 09:17:23.000000 durin-0.0.76/durin/Read_profilers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       80 2023-05-05 09:17:23.000000 durin-0.0.76/durin/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      475 2023-05-05 09:17:23.000000 durin-0.0.76/durin/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      766 2023-05-05 09:17:23.000000 durin-0.0.76/durin/actuator.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4148 2023-05-05 09:17:23.000000 durin-0.0.76/durin/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:17:32.362083 durin-0.0.76/durin/controller/
--rwxr-xr-x   0 runner    (1001) docker     (123)       40 2023-05-05 09:17:23.000000 durin-0.0.76/durin/controller/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      344 2023-05-05 09:17:23.000000 durin-0.0.76/durin/controller/dvs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4307 2023-05-05 09:17:23.000000 durin-0.0.76/durin/controller/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:17:32.362083 durin-0.0.76/durin/controller/test/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:17:23.000000 durin-0.0.76/durin/controller/test/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      947 2023-05-05 09:17:23.000000 durin-0.0.76/durin/controller/test/test_stream.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4694 2023-05-05 09:17:23.000000 durin-0.0.76/durin/durin.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   181742 2023-05-05 09:17:23.000000 durin-0.0.76/durin/durin_birdseye.jpg
--rwxr-xr-x   0 runner    (1001) docker     (123)      504 2023-05-05 09:17:23.000000 durin-0.0.76/durin/dvs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:17:32.362083 durin-0.0.76/durin/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-05 09:17:23.000000 durin-0.0.76/durin/examples/CPU_test.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 09:17:23.000000 durin-0.0.76/durin/examples/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2281 2023-05-05 09:17:23.000000 durin-0.0.76/durin/examples/braitenberg.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2631 2023-05-05 09:17:23.000000 durin-0.0.76/durin/examples/commands.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1459 2023-05-05 09:17:23.000000 durin-0.0.76/durin/examples/dashboard.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      923 2023-05-05 09:17:23.000000 durin-0.0.76/durin/examples/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-05 09:17:23.000000 durin-0.0.76/durin/examples/plot.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      589 2023-05-05 09:17:23.000000 durin-0.0.76/durin/examples/record.py
--rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-05-05 09:17:23.000000 durin-0.0.76/durin/examples/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:17:32.362083 durin-0.0.76/durin/io/
--rwxr-xr-x   0 runner    (1001) docker     (123)      673 2023-05-05 09:17:23.000000 durin-0.0.76/durin/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-05-05 09:17:23.000000 durin-0.0.76/durin/io/command.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1442 2023-05-05 09:17:23.000000 durin-0.0.76/durin/io/gamepad.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6181 2023-05-05 09:17:23.000000 durin-0.0.76/durin/io/network.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      525 2023-05-05 09:17:23.000000 durin-0.0.76/durin/io/ringbuffer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1824 2023-05-05 09:17:23.000000 durin-0.0.76/durin/io/runnable.py
--rw-r--r--   0 runner    (1001) docker     (123)     9042 2023-05-05 09:17:23.000000 durin-0.0.76/durin/io/schema.capnp
--rwxr-xr-x   0 runner    (1001) docker     (123)     7102 2023-05-05 09:17:23.000000 durin-0.0.76/durin/sensor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14526 2023-05-05 09:17:23.000000 durin-0.0.76/durin/ui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:17:32.358083 durin-0.0.76/durin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-05-05 09:17:32.000000 durin-0.0.76/durin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-05 09:17:32.000000 durin-0.0.76/durin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 09:17:32.000000 durin-0.0.76/durin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-05 09:17:32.000000 durin-0.0.76/durin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-05 09:17:32.000000 durin-0.0.76/durin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 09:17:32.362083 durin-0.0.76/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      663 2023-05-05 09:17:23.000000 durin-0.0.76/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:25:23.354399 durin-0.0.77/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-08 11:25:11.000000 durin-0.0.77/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-05-08 11:25:23.354399 durin-0.0.77/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2683 2023-05-08 11:25:11.000000 durin-0.0.77/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:25:23.346399 durin-0.0.77/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       34 2023-05-08 11:25:11.000000 durin-0.0.77/bin/durin
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:25:23.350399 durin-0.0.77/durin/
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-08 11:25:11.000000 durin-0.0.77/durin/Profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-08 11:25:11.000000 durin-0.0.77/durin/Read_profilers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       80 2023-05-08 11:25:11.000000 durin-0.0.77/durin/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      475 2023-05-08 11:25:11.000000 durin-0.0.77/durin/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      766 2023-05-08 11:25:11.000000 durin-0.0.77/durin/actuator.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4148 2023-05-08 11:25:11.000000 durin-0.0.77/durin/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:25:23.350399 durin-0.0.77/durin/controller/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       40 2023-05-08 11:25:11.000000 durin-0.0.77/durin/controller/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      344 2023-05-08 11:25:11.000000 durin-0.0.77/durin/controller/dvs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4307 2023-05-08 11:25:11.000000 durin-0.0.77/durin/controller/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:25:23.350399 durin-0.0.77/durin/controller/test/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:25:11.000000 durin-0.0.77/durin/controller/test/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      947 2023-05-08 11:25:11.000000 durin-0.0.77/durin/controller/test/test_stream.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4694 2023-05-08 11:25:11.000000 durin-0.0.77/durin/durin.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   181742 2023-05-08 11:25:11.000000 durin-0.0.77/durin/durin_birdseye.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      504 2023-05-08 11:25:11.000000 durin-0.0.77/durin/dvs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:25:23.354399 durin-0.0.77/durin/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-08 11:25:11.000000 durin-0.0.77/durin/examples/CPU_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:25:11.000000 durin-0.0.77/durin/examples/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2281 2023-05-08 11:25:11.000000 durin-0.0.77/durin/examples/braitenberg.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2631 2023-05-08 11:25:11.000000 durin-0.0.77/durin/examples/commands.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1632 2023-05-08 11:25:11.000000 durin-0.0.77/durin/examples/dashboard.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      923 2023-05-08 11:25:11.000000 durin-0.0.77/durin/examples/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-08 11:25:11.000000 durin-0.0.77/durin/examples/plot.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      589 2023-05-08 11:25:11.000000 durin-0.0.77/durin/examples/record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-05-08 11:25:11.000000 durin-0.0.77/durin/examples/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:25:23.354399 durin-0.0.77/durin/io/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      673 2023-05-08 11:25:11.000000 durin-0.0.77/durin/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-05-08 11:25:11.000000 durin-0.0.77/durin/io/command.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1442 2023-05-08 11:25:11.000000 durin-0.0.77/durin/io/gamepad.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6181 2023-05-08 11:25:11.000000 durin-0.0.77/durin/io/network.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      525 2023-05-08 11:25:11.000000 durin-0.0.77/durin/io/ringbuffer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1824 2023-05-08 11:25:11.000000 durin-0.0.77/durin/io/runnable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9042 2023-05-08 11:25:11.000000 durin-0.0.77/durin/io/schema.capnp
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7102 2023-05-08 11:25:11.000000 durin-0.0.77/durin/sensor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14646 2023-05-08 11:25:11.000000 durin-0.0.77/durin/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:25:23.350399 durin-0.0.77/durin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-05-08 11:25:23.000000 durin-0.0.77/durin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-08 11:25:23.000000 durin-0.0.77/durin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 11:25:23.000000 durin-0.0.77/durin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-08 11:25:23.000000 durin-0.0.77/durin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-08 11:25:23.000000 durin-0.0.77/durin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 11:25:23.354399 durin-0.0.77/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      663 2023-05-08 11:25:11.000000 durin-0.0.77/setup.py
```

### Comparing `durin-0.0.76/PKG-INFO` & `durin-0.0.77/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: durin
-Version: 0.0.76
+Version: 0.0.77
 Summary: Python control interface for the Durin robot
 Maintainer: Jens E. Pedersen
 Maintainer-email: jeped@kth.se
 License: LGPLv3
 Description-Content-Type: text/markdown
 Provides-Extra: aestream
```

### Comparing `durin-0.0.76/README.md` & `durin-0.0.77/README.md`

 * *Files identical despite different names*

### Comparing `durin-0.0.76/durin/actuator.py` & `durin-0.0.77/durin/actuator.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.76/durin/cli.py` & `durin-0.0.77/durin/cli.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.76/durin/controller/server.py` & `durin-0.0.77/durin/controller/server.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.76/durin/controller/test/test_stream.py` & `durin-0.0.77/durin/controller/test/test_stream.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.76/durin/durin.py` & `durin-0.0.77/durin/durin.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.76/durin/durin_birdseye.jpg` & `durin-0.0.77/durin/durin_birdseye.jpg`

 * *Files identical despite different names*

### Comparing `durin-0.0.76/durin/examples/braitenberg.py` & `durin-0.0.77/durin/examples/braitenberg.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.76/durin/examples/commands.py` & `durin-0.0.77/durin/examples/commands.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.76/durin/examples/dashboard.py` & `durin-0.0.77/durin/examples/dashboard.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,19 +4,23 @@
 
 
 if __name__ == "__main__":
 
     # We start a connectioen to the robot
     # and can now read from and write to the robot via the variable "durin"
     # Notice the UI class, which differs from the (more efficient) standalone Durin interface
-    with DurinUI("durin1.local") as durin:
+    # the debug flag enables/disables some ugly data on the dashboard
+    if len(sys.argv) == 2:
+        debug = (sys.argv[1] == "debug")
+    else:
+        debug = False
+
+    with DurinUI("durin1.local", debug=debug) as durin:
         # Loop until the user quits
         is_running = True
-
-
         durin(GetSystemInfo())  # Ask to get IP address, MAC address and Durin ID
         gotSystemInfo = False
 
         while not gotSystemInfo:
             """ Wait until IP address, MAC address, and Durin ID are read"""
             try:
                 (obs, dvs, cmd) = durin.read()
@@ -25,15 +29,14 @@
                 id = cmd.systemInfo.id
                 durin.set_ip_mac_id(ip,mac,id)
                 gotSystemInfo = True
 
             except:
                 pass
 
-        
         while is_running:
 
             # Read a value from durin
             # - obs = Robot sensor observations
             # - dvs = Robot DVS data (if any)
             # - cmd = Robot responses to commands
             (obs, dvs, cmd) = durin.read()
```

### Comparing `durin-0.0.76/durin/examples/main.py` & `durin-0.0.77/durin/examples/main.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.76/durin/examples/plot.py` & `durin-0.0.77/durin/examples/plot.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.76/durin/examples/record.py` & `durin-0.0.77/durin/examples/record.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.76/durin/examples/stats.py` & `durin-0.0.77/durin/examples/stats.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.76/durin/io/__init__.py` & `durin-0.0.77/durin/io/__init__.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.76/durin/io/command.py` & `durin-0.0.77/durin/io/command.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.76/durin/io/gamepad.py` & `durin-0.0.77/durin/io/gamepad.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.76/durin/io/network.py` & `durin-0.0.77/durin/io/network.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.76/durin/io/ringbuffer.py` & `durin-0.0.77/durin/io/ringbuffer.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.76/durin/io/runnable.py` & `durin-0.0.77/durin/io/runnable.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.76/durin/io/schema.capnp` & `durin-0.0.77/durin/io/schema.capnp`

 * *Files identical despite different names*

### Comparing `durin-0.0.76/durin/sensor.py` & `durin-0.0.77/durin/sensor.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.76/durin/ui.py` & `durin-0.0.77/durin/ui.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,14 +56,15 @@
 UWB_PLACEMENT = (x, 0.1+29*d)              # Upper left corner
 
 TOF_STATUS_PLACEMENT = (x, 0.1+25*d)
 
 
 class DurinUI(Durin):
     def __init__(self, *args, **kwargs):
+        self.debug = kwargs.pop("debug", False)
         super().__init__(*args, **kwargs)
         self.gamepad = Gamepad()
 
         self.ip = None
         self.mac = None
         self.id = None
 
@@ -196,14 +197,16 @@
                     left = i * square_size
                     top = j * square_size
                     square_rect = pygame.Rect(left, top, square_size, square_size)
                     color_value = tofs[o][i][j]
                     color = (color_value, color_value, color_value)
                     pygame.draw.rect(surface, color, square_rect)
 
+                    if not self.debug:
+                        continue
                     status_left = i * square_size // 2 + surface_height
                     status_top = j * square_size // 2 + surface_height / 4
                     status_rect = pygame.Rect(status_left, status_top, math.ceil(square_size / 2), math.ceil(square_size / 2))
                     status_color = (0, 0, 0)
                     if obs.tof_status[o][i][j] == 0: # all good
                         status_color = (0, 255, 0)
                     elif obs.tof_status[o][i][j] == 1: # 50% error
```

### Comparing `durin-0.0.76/durin.egg-info/PKG-INFO` & `durin-0.0.77/durin.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: durin
-Version: 0.0.76
+Version: 0.0.77
 Summary: Python control interface for the Durin robot
 Maintainer: Jens E. Pedersen
 Maintainer-email: jeped@kth.se
 License: LGPLv3
 Description-Content-Type: text/markdown
 Provides-Extra: aestream
```

### Comparing `durin-0.0.76/durin.egg-info/SOURCES.txt` & `durin-0.0.77/durin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `durin-0.0.76/setup.py` & `durin-0.0.77/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     requirements = fp.read().split("\n")
 
 with open("README.md", "r") as fp:
     long_description = fp.read()
 
 setup(
     name="durin",
-    version="0.0.76",
+    version="0.0.77",
     install_requires=requirements,
     packages=find_packages(),
     license="LGPLv3",
     maintainer="Jens E. Pedersen",
     maintainer_email="jeped@kth.se",
     extras_require={"aestream": ["aestream"]},
     scripts=["bin/durin"],
```

