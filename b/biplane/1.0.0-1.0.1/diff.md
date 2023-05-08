# Comparing `tmp/biplane-1.0.0.tar.gz` & `tmp/biplane-1.0.1.tar.gz`

## Comparing `biplane-1.0.0.tar` & `biplane-1.0.1.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     8459 2020-02-02 00:00:00.000000 biplane-1.0.0/biplane.py
--rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 biplane-1.0.0/tests.py
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 biplane-1.0.0/LICENSE.txt
--rw-r--r--   0        0        0     6560 2020-02-02 00:00:00.000000 biplane-1.0.0/README.md
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 biplane-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     7156 2020-02-02 00:00:00.000000 biplane-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     8430 2020-02-02 00:00:00.000000 biplane-1.0.1/biplane.py
+-rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 biplane-1.0.1/tests.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 biplane-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 biplane-1.0.1/LICENSE.txt
+-rw-r--r--   0        0        0     8465 2020-02-02 00:00:00.000000 biplane-1.0.1/README.md
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 biplane-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     9061 2020-02-02 00:00:00.000000 biplane-1.0.1/PKG-INFO
```

### Comparing `biplane-1.0.0/biplane.py` & `biplane-1.0.1/biplane.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import time
 import errno
 
 
-__version__ = "0.0.0+auto.0"
+__version__ = "1.0.1"
 __repo__ = "https://github.com/Uberi/biplane.git"
 
 
 class BufferedNonBlockingSocket:
-  def __init__(self, sock, buffer_size=2):
+  def __init__(self, sock, buffer_size=1024):
     self.sock = sock
     self.read_buffer = bytearray(buffer_size)
     self.start, self.end = 0, 0
 
   def read(self, size=-1, stop_byte=None):
     while True:
       # fulfill as much of the request as possible from the buffer
@@ -184,32 +184,32 @@
           if not isinstance(e, StopIteration):
             raise
         else:
           new_client_processors.append((start_time, client_socket, client_processor))
       client_processors = new_client_processors
       yield
 
-  def circuitpython_start_wifi_ap(self, ssid, password, mdns_hostname=None, listen_on=('0.0.0.0', 80), max_parallel_connections=5):
+  def circuitpython_start_wifi_ap(self, ssid, password, mdns_hostname, listen_on=('0.0.0.0', 80), max_parallel_connections=5):
     import wifi
     import mdns
     import socketpool
     wifi.radio.start_ap(ssid=ssid, password=password)
-    print(f"starting mDNS at {SERVICE_HOSTNAME}.local (IP address {wifi.radio.ipv4_address_ap})")
+    print(f"starting mDNS at {mdns_hostname}.local (IP address {wifi.radio.ipv4_address_ap})")
     server = mdns.Server(wifi.radio)
     server.hostname = mdns_hostname
     server.advertise_service(service_type="_http", protocol="_tcp", port=listen_on[1])
     pool = socketpool.SocketPool(wifi.radio)
     with pool.socket() as server_socket:
-      yield from self.start_server(server_socket, listen_on, max_parallel_connections)
+      yield from self.start(server_socket, listen_on, max_parallel_connections)
 
   def circuitpython_start_wifi_station(self, ssid, password, mdns_hostname, listen_on=('0.0.0.0', 80), max_parallel_connections=5):
     import wifi
     import mdns
     import socketpool
     wifi.radio.connect(ssid, password)
-    print(f"starting mDNS at {SERVICE_HOSTNAME}.local (IP address {wifi.radio.ipv4_address})")
+    print(f"starting mDNS at {mdns_hostname}.local (IP address {wifi.radio.ipv4_address})")
     server = mdns.Server(wifi.radio)
     server.hostname = mdns_hostname
     server.advertise_service(service_type="_http", protocol="_tcp", port=listen_on[1])
     pool = socketpool.SocketPool(wifi.radio)
     with pool.socket() as server_socket:
-      yield from self.start_server(server_socket, listen_on, max_parallel_connections)
+      yield from self.start(server_socket, listen_on, max_parallel_connections)
```

### Comparing `biplane-1.0.0/tests.py` & `biplane-1.0.1/tests.py`

 * *Files identical despite different names*

### Comparing `biplane-1.0.0/LICENSE.txt` & `biplane-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `biplane-1.0.0/README.md` & `biplane-1.0.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -23,28 +23,55 @@
 
 * Helpers for parsing query parameters and dealing with URL encoding/decoding.
 * Helpers for building HTTP responses, such as header formatting, templating, and more.
 * Helpers for dealing with MIME types (Adafruit_CircuitPython_HTTPServer has this).
 * Support for chunked transfer encoding (Adafruit_CircuitPython_HTTPServer has this).
 * Support for serving static files (Adafruit_CircuitPython_HTTPServer has this).
 
+Installation
+------------
+
+### Python
+
+Install via Pip:
+
+```sh
+pip install biplane
+```
+
+### CircuitPython
+
+First, ensure you've set up CircUp according to the [Adafruit CircUp guide](https://learn.adafruit.com/keep-your-circuitpython-libraries-on-devices-up-to-date-with-circup). Then:
+
+```sh
+circup install biplane
+```
+
+For CircuitPython devices that don't support the CIRCUITPY drive used to upload code, you can instead manually upload `biplane.py` from this folder to `lib/biplane.py` on the board using one of the following methods:
+
+* Using the Web Workflow via Bluetooth or WiFi. See the [AdaFruit Web Workflow guide](https://learn.adafruit.com/circuitpython-with-esp32-quick-start/setting-up-web-workflow) for more details.
+* Using [Thonny](https://thonny.org/), which supports uploading code to CircuitPython.
+* As a last-resort slow-but-simple option, using the CircuitPython REPL that you can access over the serial port:
+    1. Run `python3 -c 'f=open("biplane.py");code=f.read();print(f"code={repr(code)};open(\"lib/biplane.py\",\"w\").write(code) if len(code)=={len(code)} else print(\"CODE CORRUPTED\")")'` in this folder, and copy the output of that command to the clipboard. This output is CircuitPython code that creates `lib/biplane.py` with the correct contents inside.
+    2. Paste the copied output into the CircuitPython REPL and run it. If it outputs "CODE CORRUPTED", that means the code changed between when you pasted it and when it arrived in CircuitPython, which means your serial terminal is sending the characters too quickly and CircuitPython can't keep up (common when using `screen` or `minicom`); to fix this, configure your terminal to wait 2ms-4ms after sending each character and try again (2ms is usually good enough). Also, make sure that you do this after freshly resetting the board.
+
 Examples
 --------
 
 ### Basic example (CircuitPython)
 
 Starts a WiFi network called "test" (password is "some_password") - when connected, you can see a Hello World page at `http://app.local/` (tested on an ESP32C3):
 
 ```python
 import biplane
 
 server = biplane.Server()
 
 @server.route("/", "GET")
-def main(*args):
+def main(query_parameters, headers, body):
   return biplane.Response("<b>Hello, world!</b>", content_type="text/html")
 
 for _ in server.circuitpython_start_wifi_ap("test", "some_password", "app"):
   pass
 ```
 
 ### Basic example (Python)
@@ -77,15 +104,15 @@
 import board
 import digitalio
 import biplane
 
 server = biplane.Server()
 
 @server.route("/", "GET")
-def main(*args):
+def main(query_parameters, headers, body):
   return biplane.Response("<b>Hello, world!</b>", content_type="text/html")
 
 def asyncio_sleep(seconds):  # minimal implementation of asyncio.sleep() as a generator
   start_time = time.monotonic()
   while time.monotonic() - start_time < seconds:
     yield
 
@@ -113,15 +140,15 @@
 import board
 import digitalio
 import biplane
 
 server = biplane.Server()
 
 @server.route("/", "GET")
-def main(*args):
+def main(query_parameters, headers, body):
   return biplane.Response("<b>Hello, world!</b>", content_type="text/html")
 
 async def run_server():
   for _ in server.circuitpython_start_wifi_ap("test", "some_password")
     await asyncio.sleep(0)  # let other tasks run
 
 async def blink_builtin_led():
```

### Comparing `biplane-1.0.0/pyproject.toml` & `biplane-1.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "biplane"
-version = "1.0.0"
+version = "1.0.1"
 authors = [{name="Uberi", email="me@anthonyz.ca"}]
 description = "Minimal, fast, robust HTTP server library for Python/CircuitPython that uses non-blocking concurrent I/O even when asyncio isn't available!"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `biplane-1.0.0/PKG-INFO` & `biplane-1.0.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biplane
-Version: 1.0.0
+Version: 1.0.1
 Summary: Minimal, fast, robust HTTP server library for Python/CircuitPython that uses non-blocking concurrent I/O even when asyncio isn't available!
 Project-URL: Homepage, https://github.com/Uberi/biplane/
 Project-URL: Bug Tracker, https://github.com/Uberi/biplane/issues
 Author-email: Uberi <me@anthonyz.ca>
 License-File: LICENSE.txt
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -37,28 +37,55 @@
 
 * Helpers for parsing query parameters and dealing with URL encoding/decoding.
 * Helpers for building HTTP responses, such as header formatting, templating, and more.
 * Helpers for dealing with MIME types (Adafruit_CircuitPython_HTTPServer has this).
 * Support for chunked transfer encoding (Adafruit_CircuitPython_HTTPServer has this).
 * Support for serving static files (Adafruit_CircuitPython_HTTPServer has this).
 
+Installation
+------------
+
+### Python
+
+Install via Pip:
+
+```sh
+pip install biplane
+```
+
+### CircuitPython
+
+First, ensure you've set up CircUp according to the [Adafruit CircUp guide](https://learn.adafruit.com/keep-your-circuitpython-libraries-on-devices-up-to-date-with-circup). Then:
+
+```sh
+circup install biplane
+```
+
+For CircuitPython devices that don't support the CIRCUITPY drive used to upload code, you can instead manually upload `biplane.py` from this folder to `lib/biplane.py` on the board using one of the following methods:
+
+* Using the Web Workflow via Bluetooth or WiFi. See the [AdaFruit Web Workflow guide](https://learn.adafruit.com/circuitpython-with-esp32-quick-start/setting-up-web-workflow) for more details.
+* Using [Thonny](https://thonny.org/), which supports uploading code to CircuitPython.
+* As a last-resort slow-but-simple option, using the CircuitPython REPL that you can access over the serial port:
+    1. Run `python3 -c 'f=open("biplane.py");code=f.read();print(f"code={repr(code)};open(\"lib/biplane.py\",\"w\").write(code) if len(code)=={len(code)} else print(\"CODE CORRUPTED\")")'` in this folder, and copy the output of that command to the clipboard. This output is CircuitPython code that creates `lib/biplane.py` with the correct contents inside.
+    2. Paste the copied output into the CircuitPython REPL and run it. If it outputs "CODE CORRUPTED", that means the code changed between when you pasted it and when it arrived in CircuitPython, which means your serial terminal is sending the characters too quickly and CircuitPython can't keep up (common when using `screen` or `minicom`); to fix this, configure your terminal to wait 2ms-4ms after sending each character and try again (2ms is usually good enough). Also, make sure that you do this after freshly resetting the board.
+
 Examples
 --------
 
 ### Basic example (CircuitPython)
 
 Starts a WiFi network called "test" (password is "some_password") - when connected, you can see a Hello World page at `http://app.local/` (tested on an ESP32C3):
 
 ```python
 import biplane
 
 server = biplane.Server()
 
 @server.route("/", "GET")
-def main(*args):
+def main(query_parameters, headers, body):
   return biplane.Response("<b>Hello, world!</b>", content_type="text/html")
 
 for _ in server.circuitpython_start_wifi_ap("test", "some_password", "app"):
   pass
 ```
 
 ### Basic example (Python)
@@ -91,15 +118,15 @@
 import board
 import digitalio
 import biplane
 
 server = biplane.Server()
 
 @server.route("/", "GET")
-def main(*args):
+def main(query_parameters, headers, body):
   return biplane.Response("<b>Hello, world!</b>", content_type="text/html")
 
 def asyncio_sleep(seconds):  # minimal implementation of asyncio.sleep() as a generator
   start_time = time.monotonic()
   while time.monotonic() - start_time < seconds:
     yield
 
@@ -127,15 +154,15 @@
 import board
 import digitalio
 import biplane
 
 server = biplane.Server()
 
 @server.route("/", "GET")
-def main(*args):
+def main(query_parameters, headers, body):
   return biplane.Response("<b>Hello, world!</b>", content_type="text/html")
 
 async def run_server():
   for _ in server.circuitpython_start_wifi_ap("test", "some_password")
     await asyncio.sleep(0)  # let other tasks run
 
 async def blink_builtin_led():
```

