# Comparing `tmp/python_roborock-0.9.0.tar.gz` & `tmp/python_roborock-0.9.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_roborock-0.9.0.tar", max compression
+gzip compressed data, was "python_roborock-0.9.0rc0.tar", max compression
```

## Comparing `python_roborock-0.9.0.tar` & `python_roborock-0.9.0rc0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    35149 2023-05-01 19:40:15.409056 python_roborock-0.9.0/LICENSE
--rw-r--r--   0        0        0     2122 2023-05-01 19:40:15.409056 python_roborock-0.9.0/README.md
--rw-r--r--   0        0        0     1393 2023-05-01 19:40:16.365065 python_roborock-0.9.0/pyproject.toml
--rw-r--r--   0        0        0      165 2023-05-01 19:40:15.409056 python_roborock-0.9.0/roborock/__init__.py
--rw-r--r--   0        0        0    20962 2023-05-01 19:40:15.409056 python_roborock-0.9.0/roborock/api.py
--rw-r--r--   0        0        0     4093 2023-05-01 19:40:15.409056 python_roborock-0.9.0/roborock/cli.py
--rw-r--r--   0        0        0     7314 2023-05-01 19:40:15.409056 python_roborock-0.9.0/roborock/cloud_api.py
--rw-r--r--   0        0        0     4620 2023-05-01 19:40:15.409056 python_roborock-0.9.0/roborock/code_mappings.py
--rw-r--r--   0        0        0      209 2023-05-01 19:40:15.409056 python_roborock-0.9.0/roborock/const.py
--rw-r--r--   0        0        0    10954 2023-05-01 19:40:15.409056 python_roborock-0.9.0/roborock/containers.py
--rw-r--r--   0        0        0     1483 2023-05-01 19:40:15.409056 python_roborock-0.9.0/roborock/exceptions.py
--rw-r--r--   0        0        0     5663 2023-05-01 19:40:15.409056 python_roborock-0.9.0/roborock/local_api.py
--rw-r--r--   0        0        0     5423 2023-05-01 19:40:15.409056 python_roborock-0.9.0/roborock/protocol.py
--rw-r--r--   0        0        0      694 2023-05-01 19:40:15.409056 python_roborock-0.9.0/roborock/roborock_future.py
--rw-r--r--   0        0        0     6149 2023-05-01 19:40:15.409056 python_roborock-0.9.0/roborock/roborock_message.py
--rw-r--r--   0        0        0    18391 2023-05-01 19:40:15.409056 python_roborock-0.9.0/roborock/roborock_typing.py
--rw-r--r--   0        0        0      783 2023-05-01 19:40:15.409056 python_roborock-0.9.0/roborock/util.py
--rw-r--r--   0        0        0     3383 1970-01-01 00:00:00.000000 python_roborock-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-02-15 23:23:41.026106 python_roborock-0.9.0rc0/LICENSE
+-rw-r--r--   0        0        0     2122 2023-04-17 23:50:22.944797 python_roborock-0.9.0rc0/README.md
+-rw-r--r--   0        0        0     1373 2023-04-29 00:38:52.377261 python_roborock-0.9.0rc0/pyproject.toml
+-rw-r--r--   0        0        0      156 2023-04-17 23:50:22.945724 python_roborock-0.9.0rc0/roborock/__init__.py
+-rw-r--r--   0        0        0    20953 2023-04-29 00:19:12.443894 python_roborock-0.9.0rc0/roborock/api.py
+-rw-r--r--   0        0        0     4102 2023-04-29 00:14:20.401256 python_roborock-0.9.0rc0/roborock/cli.py
+-rw-r--r--   0        0        0     7261 2023-04-29 00:18:57.528713 python_roborock-0.9.0rc0/roborock/cloud_api.py
+-rw-r--r--   0        0        0     4620 2023-04-29 00:15:07.502108 python_roborock-0.9.0rc0/roborock/code_mappings.py
+-rw-r--r--   0        0        0      209 2023-04-27 14:49:49.843263 python_roborock-0.9.0rc0/roborock/const.py
+-rw-r--r--   0        0        0    10730 2023-04-27 14:49:49.843775 python_roborock-0.9.0rc0/roborock/containers.py
+-rw-r--r--   0        0        0     1483 2023-04-27 14:49:49.930465 python_roborock-0.9.0rc0/roborock/exceptions.py
+-rw-r--r--   0        0        0     5635 2023-04-29 00:24:11.618489 python_roborock-0.9.0rc0/roborock/local_api.py
+-rw-r--r--   0        0        0      694 2023-04-22 02:10:16.435351 python_roborock-0.9.0rc0/roborock/roborock_future.py
+-rw-r--r--   0        0        0     6358 2023-04-29 00:14:58.499142 python_roborock-0.9.0rc0/roborock/roborock_message.py
+-rw-r--r--   0        0        0     4626 2023-04-29 00:06:49.142059 python_roborock-0.9.0rc0/roborock/test.py
+-rw-r--r--   0        0        0    18391 2023-04-29 00:18:15.411897 python_roborock-0.9.0rc0/roborock/typing.py
+-rw-r--r--   0        0        0      783 2023-04-25 18:03:12.110531 python_roborock-0.9.0rc0/roborock/util.py
+-rw-r--r--   0        0        0     3342 1970-01-01 00:00:00.000000 python_roborock-0.9.0rc0/PKG-INFO
```

### Comparing `python_roborock-0.9.0/LICENSE` & `python_roborock-0.9.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `python_roborock-0.9.0/README.md` & `python_roborock-0.9.0rc0/README.md`

 * *Files identical despite different names*

### Comparing `python_roborock-0.9.0/pyproject.toml` & `python_roborock-0.9.0rc0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-roborock"
-version = "0.9.0"
+version = "0.9.0-rc"
 description = "A package to control Roborock vacuums."
 authors = ["humbertogontijo <humbertogontijo@users.noreply.github.com>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 repository = "https://github.com/humbertogontijo/python-roborock"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
@@ -23,15 +23,14 @@
 click = ">=8"
 aiohttp = "*"
 async-timeout = "*"
 pycryptodome = "~3.17.0"
 pycryptodomex = {version = "~3.17.0", markers = "sys_platform == 'darwin'"}
 paho-mqtt = "~1.6.1"
 dacite = "~1.8.0"
-construct = "^2.10.68"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.dev-dependencies]
```

### Comparing `python_roborock-0.9.0/roborock/api.py` & `python_roborock-0.9.0rc0/roborock/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,21 +44,21 @@
     RoborockInvalidEmail,
     RoborockTimeout,
     RoborockUrlException,
     VacuumError,
 )
 from .roborock_future import RoborockFuture
 from .roborock_message import RoborockMessage
-from .roborock_typing import DeviceProp, DockSummary, RoborockCommand
+from .typing import DeviceProp, DockSummary, RoborockCommand
 from .util import unpack_list
 
 _LOGGER = logging.getLogger(__name__)
 KEEPALIVE = 60
 QUEUE_TIMEOUT = 4
-COMMANDS_SECURED = [
+SPECIAL_COMMANDS = [
     RoborockCommand.GET_MAP_V1,
 ]
 
 
 def md5hex(message: str) -> str:
     md5 = hashlib.md5()
     md5.update(message.encode())
```

### Comparing `python_roborock-0.9.0/roborock/cli.py` & `python_roborock-0.9.0rc0/roborock/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,26 +67,26 @@
         context.validate()
         _LOGGER.info("Already logged in")
         return
     except RoborockException:
         pass
     client = RoborockApiClient(email)
     user_data = await client.pass_login(password)
-    context.update(LoginData(user_data=user_data, email=email))
+    context.update(LoginData({"user_data": user_data, "email": email}))
 
 
 async def _discover(ctx):
     context: RoborockContext = ctx.obj
     login_data = context.login_data()
-    if not login_data:
-        raise Exception("You need to login first")
     client = RoborockApiClient(login_data.email)
     home_data = await client.get_home_data(login_data.user_data)
-    context.update(LoginData(**login_data.as_dict(), home_data=home_data))
-    click.echo(f"Discovered devices {', '.join([device.name for device in home_data.get_all_devices()])}")
+    context.update(LoginData({**login_data, "home_data": home_data}))
+    click.echo(
+        f"Discovered devices {', '.join([device.name for device in home_data.devices + home_data.received_devices])}"
+    )
 
 
 @click.command()
 @click.pass_context
 @run_sync()
 async def discover(ctx):
     await _discover(ctx)
@@ -117,15 +117,16 @@
 async def command(ctx, cmd, device_id, params):
     context: RoborockContext = ctx.obj
     login_data = context.login_data()
     if not login_data.home_data:
         await _discover(ctx)
         login_data = context.login_data()
     home_data = login_data.home_data
-    device = next((device for device in home_data.get_all_devices() if device.duid == device_id))
+    devices = home_data.devices + home_data.received_devices
+    device = next((device for device in devices if device.duid == device_id), None)
     device_info = RoborockDeviceInfo(device=device)
     mqtt_client = RoborockMqttClient(login_data.user_data, device_info)
     await mqtt_client.send_command(cmd, params)
     mqtt_client.__del__()
 
 
 cli.add_command(login)
```

### Comparing `python_roborock-0.9.0/roborock/cloud_api.py` & `python_roborock-0.9.0rc0/roborock/cloud_api.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,36 +6,35 @@
 import uuid
 from asyncio import Lock
 from typing import Optional
 from urllib.parse import urlparse
 
 import paho.mqtt.client as mqtt
 
-from .api import COMMANDS_SECURED, KEEPALIVE, RoborockClient, md5hex
+from .api import KEEPALIVE, SPECIAL_COMMANDS, RoborockClient, md5hex
 from .containers import RoborockDeviceInfo, UserData
 from .exceptions import CommandVacuumError, RoborockException, VacuumError
-from .protocol import Utils
 from .roborock_future import RoborockFuture
-from .roborock_message import RoborockMessage, RoborockParser
-from .roborock_typing import RoborockCommand
+from .roborock_message import RoborockMessage, RoborockParser, md5bin
+from .typing import RoborockCommand
 
 _LOGGER = logging.getLogger(__name__)
 CONNECT_REQUEST_ID = 0
 DISCONNECT_REQUEST_ID = 1
 
 
 class RoborockMqttClient(RoborockClient, mqtt.Client):
     _thread: threading.Thread
     _client_id: str
 
     def __init__(self, user_data: UserData, device_info: RoborockDeviceInfo) -> None:
         rriot = user_data.rriot
         if rriot is None:
             raise RoborockException("Got no rriot data from user_data")
-        endpoint = base64.b64encode(Utils.md5(rriot.k.encode())[8:14]).decode()
+        endpoint = base64.b64encode(md5bin(rriot.k)[8:14]).decode()
         RoborockClient.__init__(self, endpoint, device_info)
         mqtt.Client.__init__(self, protocol=mqtt.MQTTv5)
         self._mqtt_user = rriot.u
         self._hashed_user = md5hex(self._mqtt_user + ":" + rriot.k)[2:10]
         url = urlparse(rriot.r.m)
         if not isinstance(url.hostname, str):
             raise RoborockException("Url parsing returned an invalid hostname")
@@ -43,15 +42,15 @@
         self._mqtt_port = url.port
         self._mqtt_ssl = url.scheme == "ssl"
         if self._mqtt_ssl:
             super().tls_set()
         self._mqtt_password = rriot.s
         self._hashed_password = md5hex(self._mqtt_password + ":" + rriot.k)[16:]
         super().username_pw_set(self._hashed_user, self._hashed_password)
-        self._endpoint = base64.b64encode(Utils.md5(rriot.k.encode())[8:14]).decode()
+        self._endpoint = base64.b64encode(md5bin(rriot.k)[8:14]).decode()
         self._waiting_queue: dict[int, RoborockFuture] = {}
         self._mutex = Lock()
         self.update_client_id()
 
     def on_connect(self, *args, **kwargs):
         _, __, ___, rc, ____ = args
         connection_queue = self._waiting_queue.get(CONNECT_REQUEST_ID)
@@ -149,15 +148,15 @@
             raise RoborockException(f"Failed to publish (rc: {info.rc})")
 
     async def send_command(self, method: RoborockCommand, params: Optional[list | dict] = None):
         await self.validate_connection()
         request_id, timestamp, payload = super()._get_payload(method, params, True)
         _LOGGER.debug(f"id={request_id} Requesting method {method} with {params}")
         request_protocol = 101
-        response_protocol = 301 if method in COMMANDS_SECURED else 102
+        response_protocol = 301 if method in SPECIAL_COMMANDS else 102
         roborock_message = RoborockMessage(timestamp=timestamp, protocol=request_protocol, payload=payload)
         local_key = self.device_info.device.local_key
         msg = RoborockParser.encode(roborock_message, local_key)
         self._send_msg_raw(msg)
         (response, err) = await self._async_response(request_id, response_protocol)
         if err:
             raise CommandVacuumError(method, err) from err
```

### Comparing `python_roborock-0.9.0/roborock/code_mappings.py` & `python_roborock-0.9.0rc0/roborock/code_mappings.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.9.0/roborock/containers.py` & `python_roborock-0.9.0rc0/roborock/containers.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,24 +3,27 @@
 import re
 from dataclasses import asdict, dataclass
 from enum import Enum
 from typing import Any, Optional
 
 from dacite import Config, from_dict
 
+from roborock.code_mappings import (
+    RoborockDockTypeCode,
+    RoborockDockWashTowelModeCode,
+    RoborockMopIntensityCode,
+    RoborockStateCode,
+)
+
 from .code_mappings import (
     RoborockDockDustCollectionModeCode,
     RoborockDockErrorCode,
-    RoborockDockTypeCode,
-    RoborockDockWashTowelModeCode,
     RoborockErrorCode,
     RoborockFanPowerCode,
-    RoborockMopIntensityCode,
     RoborockMopModeCode,
-    RoborockStateCode,
 )
 from .const import FILTER_REPLACE_TIME, MAIN_BRUSH_REPLACE_TIME, SENSOR_DIRTY_REPLACE_TIME, SIDE_BRUSH_REPLACE_TIME
 
 
 def camelize(s: str):
     first, *others = s.split("_")
     if len(others) == 0:
@@ -173,28 +176,20 @@
     lat: Optional[Any] = None
     geo_name: Optional[Any] = None
     products: Optional[list[HomeDataProduct]] = None
     devices: Optional[list[HomeDataDevice]] = None
     received_devices: Optional[list[HomeDataDevice]] = None
     rooms: Optional[list[HomeDataRoom]] = None
 
-    def get_all_devices(self) -> list[HomeDataDevice]:
-        devices = []
-        if self.devices is not None:
-            devices += self.devices
-        if self.received_devices is not None:
-            devices += self.received_devices
-        return devices
-
 
 @dataclass
 class LoginData(RoborockBase):
     user_data: UserData
-    email: str
-    home_data: Optional[HomeData] = None
+    home_data: HomeData
+    email: Optional[str] = None
 
 
 @dataclass
 class Status(RoborockBase):
     msg_ver: Optional[int] = None
     msg_seq: Optional[int] = None
     state: Optional[RoborockStateCode] = None  # type: ignore[valid-type]
```

### Comparing `python_roborock-0.9.0/roborock/exceptions.py` & `python_roborock-0.9.0rc0/roborock/exceptions.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.9.0/roborock/local_api.py` & `python_roborock-0.9.0rc0/roborock/local_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 import asyncio
 import logging
 from asyncio import Lock, Transport
 from typing import Optional
 
 import async_timeout
 
-from .api import COMMANDS_SECURED, QUEUE_TIMEOUT, RoborockClient
+from .api import QUEUE_TIMEOUT, SPECIAL_COMMANDS, RoborockClient
 from .containers import RoborockLocalDeviceInfo
 from .exceptions import CommandVacuumError, RoborockConnectionException, RoborockException
-from .roborock_message import AP_CONFIG, RoborockMessage, RoborockParser
-from .roborock_typing import CommandInfoMap, RoborockCommand
+from .roborock_message import RoborockMessage, RoborockParser
+from .typing import CommandInfoMap, RoborockCommand
 from .util import get_running_loop_or_create_one
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class RoborockLocalClient(RoborockClient, asyncio.Protocol):
     def __init__(self, device_info: RoborockLocalDeviceInfo):
@@ -60,15 +60,15 @@
             self.transport.close()
 
     async def async_disconnect(self) -> None:
         async with self._mutex:
             self.sync_disconnect()
 
     def build_roborock_message(self, method: RoborockCommand, params: Optional[list | dict] = None) -> RoborockMessage:
-        secured = True if method in COMMANDS_SECURED else False
+        secured = True if method in SPECIAL_COMMANDS else False
         request_id, timestamp, payload = self._get_payload(method, params, secured)
         _LOGGER.debug(f"id={request_id} Requesting method {method} with {params}")
         command_info = CommandInfoMap.get(method)
         if not command_info:
             raise RoborockException(f"Request {method} have unknown prefix. Can't execute in offline mode")
         command = CommandInfoMap.get(method)
         if command is None:
@@ -80,15 +80,15 @@
             timestamp=timestamp,
             protocol=request_protocol,
             payload=payload,
         )
 
     async def ping(self):
         command_info = CommandInfoMap[RoborockCommand.NONE]
-        roborock_message = RoborockMessage(prefix=command_info.prefix, protocol=AP_CONFIG, payload=b"")
+        roborock_message = RoborockMessage(prefix=command_info.prefix, protocol=0, payload=b"")
         return (await self.send_message(roborock_message))[0]
 
     async def send_command(self, method: RoborockCommand, params: Optional[list | dict] = None):
         roborock_message = self.build_roborock_message(method, params)
         return (await self.send_message(roborock_message))[0]
 
     async def async_local_response(self, roborock_message: RoborockMessage):
```

### Comparing `python_roborock-0.9.0/roborock/roborock_future.py` & `python_roborock-0.9.0rc0/roborock/roborock_future.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.9.0/roborock/roborock_message.py` & `python_roborock-0.9.0rc0/roborock/roborock_message.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,37 @@
 from __future__ import annotations
 
 import binascii
+import hashlib
 import json
 import math
 import struct
 import time
 from dataclasses import dataclass
 from random import randint
 
 from Crypto.Cipher import AES
 from Crypto.Util.Padding import pad, unpad
 
-from .exceptions import RoborockException
-from .protocol import Utils
-from .roborock_typing import RoborockCommand
+from roborock.exceptions import RoborockException
+from roborock.typing import RoborockCommand
 
-SALT = "TXdfu$jyZ#TZHsg4".encode()
 
-AP_CONFIG = 1
-SOCK_DISCOVERY = 2
+def md5bin(message: str) -> bytes:
+    md5 = hashlib.md5()
+    md5.update(message.encode())
+    return md5.digest()
+
+
+def encode_timestamp(_timestamp: int) -> str:
+    hex_value = f"{_timestamp:x}".zfill(8)
+    return "".join(list(map(lambda idx: hex_value[idx], [5, 6, 3, 7, 1, 2, 0, 4])))
+
+
+salt = "TXdfu$jyZ#TZHsg4"
 
 
 @dataclass
 class RoborockMessage:
     protocol: int
     payload: bytes
     seq: int = randint(100000, 999999)
@@ -68,15 +77,15 @@
         if isinstance(roborock_messages, RoborockMessage):
             roborock_messages = [roborock_messages]
 
         msg = b""
         for roborock_message in roborock_messages:
             if len(roborock_message.prefix) not in [0, 4]:
                 raise RoborockException("Invalid prefix")
-            aes_key = Utils.md5(Utils.encode_timestamp(roborock_message.timestamp) + local_key.encode() + SALT)
+            aes_key = md5bin(encode_timestamp(roborock_message.timestamp) + local_key + salt)
             cipher = AES.new(aes_key, AES.MODE_ECB)
             payload = roborock_message.payload
             if payload:
                 payload = pad(roborock_message.payload, AES.block_size)
             encrypted = cipher.encrypt(payload)
             encrypted_len = len(encrypted)
             _msg = struct.pack(
@@ -152,15 +161,15 @@
             [payload, expected_crc32] = struct.unpack_from(f"!{payload_len}sI", msg, index)
             crc32 = binascii.crc32(msg[index - format_size : index + payload_len])
             index += 4 + payload_len
             if crc32 != expected_crc32:
                 raise RoborockException(f"Wrong CRC32 {crc32}, expected {expected_crc32}")
 
         if payload:
-            aes_key = Utils.md5(Utils.encode_timestamp(timestamp) + local_key.encode() + SALT)
+            aes_key = md5bin(encode_timestamp(timestamp) + local_key + salt)
             decipher = AES.new(aes_key, AES.MODE_ECB)
             payload = unpad(decipher.decrypt(payload), AES.block_size)
 
         [structs, remaining] = RoborockParser.decode(msg, local_key, index) if index < len(msg) else ([], b"")
 
         return [
             RoborockMessage(
```

### Comparing `python_roborock-0.9.0/roborock/roborock_typing.py` & `python_roborock-0.9.0rc0/roborock/typing.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.9.0/roborock/util.py` & `python_roborock-0.9.0rc0/roborock/util.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.9.0/PKG-INFO` & `python_roborock-0.9.0rc0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-roborock
-Version: 0.9.0
+Version: 0.9.0rc0
 Summary: A package to control Roborock vacuums.
 Home-page: https://github.com/humbertogontijo/python-roborock
 License: GPL-3.0-only
 Author: humbertogontijo
 Author-email: humbertogontijo@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -16,15 +16,14 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Requires-Dist: aiohttp
 Requires-Dist: async-timeout
 Requires-Dist: click (>=8)
-Requires-Dist: construct (>=2.10.68,<3.0.0)
 Requires-Dist: dacite (>=1.8.0,<1.9.0)
 Requires-Dist: paho-mqtt (>=1.6.1,<1.7.0)
 Requires-Dist: pycryptodome (>=3.17.0,<3.18.0)
 Requires-Dist: pycryptodomex (>=3.17.0,<3.18.0) ; sys_platform == "darwin"
 Project-URL: Repository, https://github.com/humbertogontijo/python-roborock
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,24 +1,24 @@
-Metadata-Version: 2.1 Name: python-roborock Version: 0.9.0 Summary: A package
-to control Roborock vacuums. Home-page: https://github.com/humbertogontijo/
-python-roborock License: GPL-3.0-only Author: humbertogontijo Author-email:
-humbertogontijo@users.noreply.github.com Requires-Python: >=3.9,<4.0
-Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
-Audience :: Developers Classifier: License :: OSI Approved :: GNU General
-Public License v3 (GPLv3) Classifier: Natural Language :: English Classifier:
-Operating System :: OS Independent Classifier: Programming Language :: Python
-:: 3 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Software Development :: Libraries Requires-Dist: aiohttp
-Requires-Dist: async-timeout Requires-Dist: click (>=8) Requires-Dist:
-construct (>=2.10.68,<3.0.0) Requires-Dist: dacite (>=1.8.0,<1.9.0) Requires-
-Dist: paho-mqtt (>=1.6.1,<1.7.0) Requires-Dist: pycryptodome (>=3.17.0,<3.18.0)
-Requires-Dist: pycryptodomex (>=3.17.0,<3.18.0) ; sys_platform == "darwin"
-Project-URL: Repository, https://github.com/humbertogontijo/python-roborock
-Description-Content-Type: text/markdown # Roborock
+Metadata-Version: 2.1 Name: python-roborock Version: 0.9.0rc0 Summary: A
+package to control Roborock vacuums. Home-page: https://github.com/
+humbertogontijo/python-roborock License: GPL-3.0-only Author: humbertogontijo
+Author-email: humbertogontijo@users.noreply.github.com Requires-Python:
+>=3.9,<4.0 Classifier: Development Status :: 5 - Production/Stable Classifier:
+Intended Audience :: Developers Classifier: License :: OSI Approved :: GNU
+General Public License v3 (GPLv3) Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent Classifier: Programming Language
+:: Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Classifier: Topic :: Software Development :: Libraries Requires-
+Dist: aiohttp Requires-Dist: async-timeout Requires-Dist: click (>=8) Requires-
+Dist: dacite (>=1.8.0,<1.9.0) Requires-Dist: paho-mqtt (>=1.6.1,<1.7.0)
+Requires-Dist: pycryptodome (>=3.17.0,<3.18.0) Requires-Dist: pycryptodomex
+(>=3.17.0,<3.18.0) ; sys_platform == "darwin" Project-URL: Repository, https://
+github.com/humbertogontijo/python-roborock Description-Content-Type: text/
+markdown # Roborock
              [PyPI_Version] [Supported Python versions] [License]
 Roborock library for online and offline control of your vacuums. ##
 Installation Install this via pip (or your favourite package manager): `pip
 install python-roborock` ## Functionality This package can encrypt and decrypt
 the following commands: - GET_CLEAN_RECORD - GET_CONSUMABLE -
 GET_MULTI_MAPS_LIST - APP_START - APP_PAUSE - APP_STOP - APP_CHARGE - APP_SPOT
 - FIND_ME - RESUME_ZONED_CLEAN - RESUME_SEGMENT_CLEAN - SET_CUSTOM_MODE -
```

