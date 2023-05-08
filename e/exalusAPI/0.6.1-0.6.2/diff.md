# Comparing `tmp/exalusAPI-0.6.1.tar.gz` & `tmp/exalusAPI-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exalusAPI-0.6.1.tar", last modified: Mon May  8 06:54:18 2023, max compression
+gzip compressed data, was "exalusAPI-0.6.2.tar", last modified: Mon May  8 10:41:26 2023, max compression
```

## Comparing `exalusAPI-0.6.1.tar` & `exalusAPI-0.6.2.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 06:54:18.892181 exalusAPI-0.6.1/
--rw-rw-rw-   0        0        0    11558 2022-10-21 05:28:52.000000 exalusAPI-0.6.1/LICENSE
--rw-rw-rw-   0        0        0    13894 2023-05-08 06:54:18.891216 exalusAPI-0.6.1/PKG-INFO
--rw-rw-rw-   0        0        0      161 2023-03-16 07:02:58.000000 exalusAPI-0.6.1/README.md
--rw-rw-rw-   0        0        0     1089 2023-05-08 06:53:17.000000 exalusAPI-0.6.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-08 06:54:18.893187 exalusAPI-0.6.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-08 06:54:18.870182 exalusAPI-0.6.1/src/
--rw-rw-rw-   0        0        0     6588 2023-04-24 06:27:01.000000 exalusAPI-0.6.1/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 06:54:18.886214 exalusAPI-0.6.1/src/exalusAPI.egg-info/
--rw-rw-rw-   0        0        0    13894 2023-05-08 06:54:18.000000 exalusAPI-0.6.1/src/exalusAPI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      232 2023-05-08 06:54:18.000000 exalusAPI-0.6.1/src/exalusAPI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 06:54:18.000000 exalusAPI-0.6.1/src/exalusAPI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-05-08 06:54:18.000000 exalusAPI-0.6.1/src/exalusAPI.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-08 06:54:18.000000 exalusAPI-0.6.1/src/exalusAPI.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-08 10:41:26.376103 exalusAPI-0.6.2/
+-rw-rw-rw-   0        0        0    11558 2022-10-21 05:28:52.000000 exalusAPI-0.6.2/LICENSE
+-rw-rw-rw-   0        0        0    13894 2023-05-08 10:41:26.374089 exalusAPI-0.6.2/PKG-INFO
+-rw-rw-rw-   0        0        0      161 2023-03-16 07:02:58.000000 exalusAPI-0.6.2/README.md
+-rw-rw-rw-   0        0        0     1089 2023-05-08 10:38:48.000000 exalusAPI-0.6.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-08 10:41:26.376103 exalusAPI-0.6.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-08 10:41:26.342847 exalusAPI-0.6.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-08 10:41:26.358090 exalusAPI-0.6.2/src/exalusAPI/
+-rw-rw-rw-   0        0        0       41 2023-05-08 10:25:31.000000 exalusAPI-0.6.2/src/exalusAPI/__init__.py
+-rw-rw-rw-   0        0        0     7266 2023-05-08 10:38:33.000000 exalusAPI-0.6.2/src/exalusAPI/__main__.py
+drwxrwxrwx   0        0        0        0 2023-05-08 10:41:26.372089 exalusAPI-0.6.2/src/exalusAPI.egg-info/
+-rw-rw-rw-   0        0        0    13894 2023-05-08 10:41:26.000000 exalusAPI-0.6.2/src/exalusAPI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      268 2023-05-08 10:41:26.000000 exalusAPI-0.6.2/src/exalusAPI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 10:41:26.000000 exalusAPI-0.6.2/src/exalusAPI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-05-08 10:41:26.000000 exalusAPI-0.6.2/src/exalusAPI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-08 10:41:26.000000 exalusAPI-0.6.2/src/exalusAPI.egg-info/top_level.txt
```

### Comparing `exalusAPI-0.6.1/LICENSE` & `exalusAPI-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `exalusAPI-0.6.1/PKG-INFO` & `exalusAPI-0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exalusAPI
-Version: 0.6.1
+Version: 0.6.2
 Summary: Simple Exalus integration wrapper, created specifically for HomeAssistant integration.
 Author-email: Marcel Janicki <majanicki00@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `exalusAPI-0.6.1/pyproject.toml` & `exalusAPI-0.6.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "exalusAPI"
-version = "0.6.1"
+version = "0.6.2"
 description = "Simple Exalus integration wrapper, created specifically for HomeAssistant integration."
 readme = "README.md"
 authors = [{ name = "Marcel Janicki", email = "majanicki00@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python",
```

### Comparing `exalusAPI-0.6.1/src/__init__.py` & `exalusAPI-0.6.2/src/exalusAPI/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,20 @@
-import asyncio, logging, uuid, requests, time
-import dataclasses
-import json
+"""Exalus API"""
+
+from typing import Any
+from enum import Enum
+import asyncio
+import logging
+import uuid
+import requests
 import events
 
 from json import dumps, loads
 from dataclasses import dataclass, asdict
-from typing import Any
-from enum import Enum
+
 from signalrcore.hub_connection_builder import HubConnectionBuilder
 
 SERVER_BROKER_URL: str = "http://broker.tr7.pl"
 
 _LOGGER = logging.getLogger(__name__)
 
 
@@ -74,53 +78,77 @@
             await asyncio.sleep(0.1)
 
     def handle_devices_list(self):
         for i in range(len(self.devices_list)):
             print(i + 1, self.devices_list[i])
 
     def data_parser(self, resp, event):
-        obj = json.loads(resp[1])
+        """_summary_
+
+        Args:
+            resp (_type_): _description_
+            event (_type_): _description_
+
+        Returns:
+            _type_: _description_
+        """
+        obj = loads(resp[1])
         tid = obj["TransactionId"]
         df = DataFrame(
             obj["Resource"],
             obj["Status"],
             obj["Method"],
             obj["TransactionId"],
             obj["Data"],
         )
         event = DataFrameEvent(df, tid)
         event.set()
         print(obj)
         return obj
 
-    async def process_data(event):
+    async def process_data(self, event):
+        """_summary_
+
+        Args:
+            event (_type_): _description_
+        """
         try:
             async with asyncio.wait(10):
                 await event.wait()
         except asyncio.TimeoutError():
             print("Timeout!")
             return
-        df = event.df
-        tid = event.tid
+        #df = event.df
+        #tid = event.tid
         event.clear()
 
     async def authorize_async(self, auth_result):
+        """_summary_
+
+        Args:
+            auth_result (_type_): _description_
+        """
         if auth_result:
             login_frame = DataFrame(
                 "/users/user/login",
                 Status.WrongData.value,
                 Method.Put.value,
                 str(uuid.uuid1()),
                 {"Email": self.login, "Password": self.password},
             )
             await self.send_and_wait(login_frame)
         else:
             print("Authorization falied!")
 
     def authorize(self, auth_result):
+        """_summary_
+
+        Args:
+            auth_result (_type_): _description_
+        """
         asyncio.run(self.authorize_async(auth_result))
 
     def data_handler(self, data: list) -> None:
         """Handle incoming data"""
 
         self.last_response = loads(data[1])
 
@@ -175,40 +203,47 @@
             self.hub_connection.on("Authorization", self.authorize)
             self.hub_connection.on("Registration", print)
             self.hub_connection.on("Data", lambda data: self.data_parser(data, event))
             self.hub_connection.on_open(self.start)
             self.hub_connection.start()
 
     async def send_and_wait(self, sent_frame: DataFrame, ms_timeout=5000):
-        """"""
+        """_summary_
+
+        Args:
+            sent_frame (DataFrame): _description_
+            ms_timeout (int, optional): _description_. Defaults to 5000.
+        """
         ack_event = asyncio.Event()
 
         event = None
 
         print("Sent frame", sent_frame)
 
         def ack_received(response):
             recieved_frame = self.data_parser(response, event)
             print(recieved_frame["TransactionId"], sent_frame.TransactionId)
             if recieved_frame["TransactionId"] == sent_frame.TransactionId:
                 ack_event.set()
 
         self.hub_connection.on("Data", ack_received)
         self.hub_connection.send(
-            "SendTo", [self.controller_serial, dataclasses.asdict(sent_frame)]
+            "SendTo", [self.controller_serial, asdict(sent_frame)]
         )
 
         try:
             await asyncio.wait_for(ack_event.wait(), timeout=ms_timeout / 1000)
 
         except asyncio.TimeoutError:
             print("Timeout error!")
 
     def start(self):
+        """_summary_
+        """
         self.hub_connection.send(
             "AuthorizeTo", [self.controller_serial, self.controller_pin]
         )
 
     def send_frame(self, data_frame: DataFrame) -> None:
         """Send frame to controller"""
 
-        self.hub_connection.send("SendTo", [self.controller_serial, data_frame])
+        self.hub_connection.send("SendTo", [self.controller_serial, data_frame])
```

### Comparing `exalusAPI-0.6.1/src/exalusAPI.egg-info/PKG-INFO` & `exalusAPI-0.6.2/src/exalusAPI.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exalusAPI
-Version: 0.6.1
+Version: 0.6.2
 Summary: Simple Exalus integration wrapper, created specifically for HomeAssistant integration.
 Author-email: Marcel Janicki <majanicki00@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

