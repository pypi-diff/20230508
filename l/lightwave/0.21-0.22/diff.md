# Comparing `tmp/lightwave-0.21.tar.gz` & `tmp/lightwave-0.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightwave-0.21.tar", last modified: Sat Jan  7 13:37:53 2023, max compression
+gzip compressed data, was "lightwave-0.22.tar", last modified: Mon May  8 10:14:56 2023, max compression
```

## Comparing `lightwave-0.21.tar` & `lightwave-0.22.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2023-01-07 13:37:53.934136 lightwave-0.21/
--rw-rw-r--   0 colin     (1000) colin     (1000)     1068 2023-01-04 14:14:06.000000 lightwave-0.21/LICENSE
--rw-rw-r--   0 colin     (1000) colin     (1000)     3619 2023-01-07 13:37:53.934136 lightwave-0.21/PKG-INFO
--rw-rw-r--   0 colin     (1000) colin     (1000)     3211 2023-01-04 15:19:34.000000 lightwave-0.21/README.md
-drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2023-01-07 13:37:53.930136 lightwave-0.21/lightwave/
--rw-rw-r--   0 colin     (1000) colin     (1000)        0 2023-01-04 14:14:06.000000 lightwave-0.21/lightwave/__init__.py
--rw-rw-r--   0 colin     (1000) colin     (1000)     8492 2023-01-04 15:52:01.000000 lightwave-0.21/lightwave/lightwave.py
-drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2023-01-07 13:37:53.930136 lightwave-0.21/lightwave.egg-info/
--rw-rw-r--   0 colin     (1000) colin     (1000)     3619 2023-01-07 13:37:53.000000 lightwave-0.21/lightwave.egg-info/PKG-INFO
--rw-rw-r--   0 colin     (1000) colin     (1000)      265 2023-01-07 13:37:53.000000 lightwave-0.21/lightwave.egg-info/SOURCES.txt
--rw-rw-r--   0 colin     (1000) colin     (1000)        1 2023-01-07 13:37:53.000000 lightwave-0.21/lightwave.egg-info/dependency_links.txt
--rw-rw-r--   0 colin     (1000) colin     (1000)        1 2023-01-07 13:37:53.000000 lightwave-0.21/lightwave.egg-info/not-zip-safe
--rw-rw-r--   0 colin     (1000) colin     (1000)       10 2023-01-07 13:37:53.000000 lightwave-0.21/lightwave.egg-info/top_level.txt
--rw-rw-r--   0 colin     (1000) colin     (1000)       38 2023-01-07 13:37:53.934136 lightwave-0.21/setup.cfg
--rw-rw-r--   0 colin     (1000) colin     (1000)      652 2023-01-04 14:17:56.000000 lightwave-0.21/setup.py
-drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2023-01-07 13:37:53.934136 lightwave-0.21/test/
--rw-rw-r--   0 colin     (1000) colin     (1000)      630 2023-01-04 14:14:06.000000 lightwave-0.21/test/test.py
--rw-rw-r--   0 colin     (1000) colin     (1000)      328 2023-01-04 14:14:06.000000 lightwave-0.21/test/test_trv.py
+drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2023-05-08 10:14:56.899968 lightwave-0.22/
+-rw-rw-r--   0 colin     (1000) colin     (1000)     1068 2023-01-04 14:14:06.000000 lightwave-0.22/LICENSE
+-rw-rw-r--   0 colin     (1000) colin     (1000)     3619 2023-05-08 10:14:56.899968 lightwave-0.22/PKG-INFO
+-rw-rw-r--   0 colin     (1000) colin     (1000)     3211 2023-05-08 10:07:39.000000 lightwave-0.22/README.md
+drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2023-05-08 10:14:56.895968 lightwave-0.22/lightwave/
+-rw-rw-r--   0 colin     (1000) colin     (1000)        0 2023-01-04 14:14:06.000000 lightwave-0.22/lightwave/__init__.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)     9029 2023-05-08 10:08:05.000000 lightwave-0.22/lightwave/lightwave.py
+drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2023-05-08 10:14:56.895968 lightwave-0.22/lightwave.egg-info/
+-rw-rw-r--   0 colin     (1000) colin     (1000)     3619 2023-05-08 10:14:56.000000 lightwave-0.22/lightwave.egg-info/PKG-INFO
+-rw-rw-r--   0 colin     (1000) colin     (1000)      265 2023-05-08 10:14:56.000000 lightwave-0.22/lightwave.egg-info/SOURCES.txt
+-rw-rw-r--   0 colin     (1000) colin     (1000)        1 2023-05-08 10:14:56.000000 lightwave-0.22/lightwave.egg-info/dependency_links.txt
+-rw-rw-r--   0 colin     (1000) colin     (1000)        1 2023-01-07 13:37:53.000000 lightwave-0.22/lightwave.egg-info/not-zip-safe
+-rw-rw-r--   0 colin     (1000) colin     (1000)       10 2023-05-08 10:14:56.000000 lightwave-0.22/lightwave.egg-info/top_level.txt
+-rw-rw-r--   0 colin     (1000) colin     (1000)       38 2023-05-08 10:14:56.899968 lightwave-0.22/setup.cfg
+-rw-rw-r--   0 colin     (1000) colin     (1000)      652 2023-05-08 10:08:21.000000 lightwave-0.22/setup.py
+drwxrwxr-x   0 colin     (1000) colin     (1000)        0 2023-05-08 10:14:56.899968 lightwave-0.22/test/
+-rw-rw-r--   0 colin     (1000) colin     (1000)      630 2023-01-04 14:14:06.000000 lightwave-0.22/test/test.py
+-rw-rw-r--   0 colin     (1000) colin     (1000)      328 2023-01-04 14:14:06.000000 lightwave-0.22/test/test_trv.py
```

### Comparing `lightwave-0.21/LICENSE` & `lightwave-0.22/LICENSE`

 * *Files identical despite different names*

### Comparing `lightwave-0.21/PKG-INFO` & `lightwave-0.22/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightwave
-Version: 0.21
+Version: 0.22
 Summary: Python library to provide a reliable communication link with LightWaveRF lights, switches and TRVs.
 Home-page: https://github.com/GeoffAtHome/lightwave
 Author: Geoff Soord
 Author-email: geoff@soord.org.uk
 License: MIT
 Keywords: Lightwave,LightwaveRF,Lightwave WiFiLink,Lightwave Link
 Description-Content-Type: text/markdown
```

### Comparing `lightwave-0.21/README.md` & `lightwave-0.22/README.md`

 * *Files identical despite different names*

### Comparing `lightwave-0.21/lightwave/lightwave.py` & `lightwave-0.22/lightwave/lightwave.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,17 @@
     link_ip = None
     proxy_ip = None
     proxy_port = None
     transaction_id = cycle(range(1, 1000))
     the_queue = Queue()
     thread = None
     use_proxy = False
+    use_udp = False
     trv_data = {}
+    trv_response = None
 
     def __init__(self, link_ip=None):
         """Initialise the component."""
         if link_ip is not None:
             LWLink.link_ip = link_ip
 
     def _send_message(self, msg):
@@ -148,61 +150,78 @@
         return (temp, targ, battery, trv_output)
 
     def _send_queue(self):
         """If the queue is not empty, process the queue."""
         while not LWLink.the_queue.empty():
             self._send_reliable_message(LWLink.the_queue.get_nowait())
 
+    def _check_response(self, response, trans_id):
+        """Check response fron lightwave"""
+
+        if "Not yet registered." in response:
+            _LOGGER.error("Not yet registered")
+            self.register()
+            return True
+
+        if response.startswith("%d,OK" % trans_id):
+            _LOGGER.debug("got OK")
+            return True
+
+        _LOGGER.error("error %s", response)
+
+        return False
+
     def _send_reliable_message(self, msg):
         """Send msg to LightwaveRF hub."""
         result = False
         max_retries = 15
         trans_id = next(LWLink.transaction_id)
         msg = "%d,%s" % (trans_id, msg)
         err = None
         try:
             with socket.socket(
                 socket.AF_INET, socket.SOCK_DGRAM
             ) as write_sock, socket.socket(
                 socket.AF_INET, socket.SOCK_DGRAM
             ) as read_sock:
                 write_sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
-                read_sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEPORT, 1)
-                read_sock.setsockopt(socket.SOL_SOCKET, socket.SO_BROADCAST, 1)
-                read_sock.settimeout(self.SOCKET_TIMEOUT)
-                read_sock.bind(("0.0.0.0", self.RX_PORT))
+
+                if self.use_udp is False:
+                    read_sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEPORT, 1)
+                    read_sock.setsockopt(socket.SOL_SOCKET, socket.SO_BROADCAST, 1)
+                    read_sock.settimeout(self.SOCKET_TIMEOUT)
+                    read_sock.bind(("0.0.0.0", RX_PORT))
+
                 while max_retries:
                     max_retries -= 1
-                    write_sock.sendto(
-                        msg.encode("UTF-8"), (LWLink.link_ip, self.TX_PORT)
-                    )
+                    self.trv_response = None
+                    write_sock.sendto(msg.encode("UTF-8"), (LWLink.link_ip, TX_PORT))
                     result = False
-                    while True:
-                        response, dummy = read_sock.recvfrom(1024)
-                        response = response.decode("UTF-8")
-                        if "Not yet registered." in response:
-                            _LOGGER.error("Not yet registered")
-                            self.register()
-                            result = True
-                            break
-
-                        if response.startswith("%d,OK" % trans_id):
-                            result = True
-                            break
-                        if response.startswith("%d,ERR" % trans_id):
-                            _LOGGER.info(response)
-                            err = response
-                            break
 
-                        _LOGGER.info(response)
+                    if self.use_udp is True:
+                        time.sleep(1)
+                        response = self.trv_response
+                        if response is None:
+                            result = False
+                        else:
+                            result = self._check_response(response, trans_id)
+
+                    else:
+                        while True:
+                            response, dummy = read_sock.recvfrom(1024)
+                            response = response.decode("UTF-8")
+                            result = self._check_response(response, trans_id)
+                            if result:
+                                break
 
                     if result:
                         break
 
-                    time.sleep(0.25)
+                    if self.use_udp is False:
+                        time.sleep(0.25)
 
         except socket.timeout:
             _LOGGER.error("LW broker timeout!")
             return result
 
         except Exception as ex:
             _LOGGER.error(ex)
@@ -216,14 +235,15 @@
             else:
                 _LOGGER.error("LW broker fail!")
         return result
 
     async def LW_listen(self):
         """Run the LW Proxy."""
         loop = asyncio.get_running_loop()
+        self.use_udp = True
 
         _LOGGER.info("Starting Lightwave UDP listener")
 
         # One protocol instance will be created to serve all client requests
         await loop.create_datagram_endpoint(
             lambda: TrvCollector(self), local_addr=("0.0.0.0", RX_PORT), reuse_port=True
         )
@@ -242,14 +262,16 @@
         self.transport = transport
 
     # pylint: disable=W0613, R0201
     def datagram_received(self, data, addr):
         """Manage receipt of a UDP packet from Lightwave."""
         message = data.decode()
         stripped = message[2:]
-        data = json.loads(stripped)
+        try:
+            data = json.loads(stripped)
 
-        if "serial" in data.keys():
-            serial = data["serial"]
-            self.link.trv_data[serial] = data
+            if "serial" in data.keys():
+                serial = data["serial"]
+                self.link.trv_data[serial] = data
 
-            _LOGGER.debug("TRV Broadcast from %s", serial)
+        except json.JSONDecodeError:
+            self.link.trv_response = message
```

### Comparing `lightwave-0.21/lightwave.egg-info/PKG-INFO` & `lightwave-0.22/lightwave.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightwave
-Version: 0.21
+Version: 0.22
 Summary: Python library to provide a reliable communication link with LightWaveRF lights, switches and TRVs.
 Home-page: https://github.com/GeoffAtHome/lightwave
 Author: Geoff Soord
 Author-email: geoff@soord.org.uk
 License: MIT
 Keywords: Lightwave,LightwaveRF,Lightwave WiFiLink,Lightwave Link
 Description-Content-Type: text/markdown
```

### Comparing `lightwave-0.21/setup.py` & `lightwave-0.22/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='lightwave',
-    version='0.21',
+    version='0.22',
     description='Python library to provide a reliable communication link with LightWaveRF lights, switches and TRVs.',
     url='https://github.com/GeoffAtHome/lightwave',
     author='Geoff Soord',
     author_email='geoff@soord.org.uk',
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='MIT',
```

### Comparing `lightwave-0.21/test/test.py` & `lightwave-0.22/test/test.py`

 * *Files identical despite different names*

