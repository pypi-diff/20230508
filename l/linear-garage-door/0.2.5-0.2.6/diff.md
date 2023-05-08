# Comparing `tmp/linear_garage_door-0.2.5.tar.gz` & `tmp/linear_garage_door-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linear_garage_door-0.2.5.tar", max compression
+gzip compressed data, was "linear_garage_door-0.2.6.tar", max compression
```

## Comparing `linear_garage_door-0.2.5.tar` & `linear_garage_door-0.2.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1098 2023-04-11 22:43:12.507688 linear_garage_door-0.2.5/LICENSE
--rw-r--r--   0        0        0     3005 2023-04-11 22:43:12.507688 linear_garage_door-0.2.5/README.md
--rw-r--r--   0        0        0     2327 2023-04-11 22:43:12.507688 linear_garage_door-0.2.5/pyproject.toml
--rw-r--r--   0        0        0    18672 2023-04-11 22:43:12.507688 linear_garage_door-0.2.5/src/linear_garage_door/__init__.py
--rw-r--r--   0        0        0      861 2023-04-11 22:43:12.507688 linear_garage_door-0.2.5/src/linear_garage_door/_util.py
--rw-r--r--   0        0        0      938 2023-04-11 22:43:12.507688 linear_garage_door-0.2.5/src/linear_garage_door/const.py
--rw-r--r--   0        0        0      703 2023-04-11 22:43:12.507688 linear_garage_door-0.2.5/src/linear_garage_door/errors.py
--rw-r--r--   0        0        0        0 2023-04-11 22:43:12.507688 linear_garage_door-0.2.5/src/linear_garage_door/py.typed
--rw-r--r--   0        0        0     3433 2023-04-11 22:43:12.507688 linear_garage_door-0.2.5/src/linear_garage_door/ws.py
--rw-r--r--   0        0        0     4360 1970-01-01 00:00:00.000000 linear_garage_door-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1098 2023-05-08 20:40:17.306169 linear_garage_door-0.2.6/LICENSE
+-rw-r--r--   0        0        0     3005 2023-05-08 20:40:17.306169 linear_garage_door-0.2.6/README.md
+-rw-r--r--   0        0        0     2327 2023-05-08 20:40:17.310169 linear_garage_door-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0    18982 2023-05-08 20:40:17.310169 linear_garage_door-0.2.6/src/linear_garage_door/__init__.py
+-rw-r--r--   0        0        0      861 2023-05-08 20:40:17.310169 linear_garage_door-0.2.6/src/linear_garage_door/_util.py
+-rw-r--r--   0        0        0      938 2023-05-08 20:40:17.310169 linear_garage_door-0.2.6/src/linear_garage_door/const.py
+-rw-r--r--   0        0        0      703 2023-05-08 20:40:17.310169 linear_garage_door-0.2.6/src/linear_garage_door/errors.py
+-rw-r--r--   0        0        0        0 2023-05-08 20:40:17.310169 linear_garage_door-0.2.6/src/linear_garage_door/py.typed
+-rw-r--r--   0        0        0     3433 2023-05-08 20:40:17.310169 linear_garage_door-0.2.6/src/linear_garage_door/ws.py
+-rw-r--r--   0        0        0     4360 1970-01-01 00:00:00.000000 linear_garage_door-0.2.6/PKG-INFO
```

### Comparing `linear_garage_door-0.2.5/LICENSE` & `linear_garage_door-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `linear_garage_door-0.2.5/README.md` & `linear_garage_door-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `linear_garage_door-0.2.5/pyproject.toml` & `linear_garage_door-0.2.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "linear-garage-door"
-version = "0.2.5"
+version = "0.2.6"
 description = "Control Linear Garage Doors with Python"
 authors = [
     "IceBotYT <icebotyt@outlook.com>",
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `linear_garage_door-0.2.5/src/linear_garage_door/__init__.py` & `linear_garage_door-0.2.6/src/linear_garage_door/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,38 +121,43 @@
         try:
             result = await asyncio.wait_for(future, timeout=10.0)
         except asyncio.TimeoutError:
             raise
 
         return result
 
-    async def _await_for_msg_type(self: Linear, msg_type: str) -> dict[str, Any]:
+    async def _await_for_msg_type(
+        self: Linear, msg_type: str, timeout: float = 10.0
+    ) -> dict[str, Any]:
         future: asyncio.Future[dict[str, Any]] = asyncio.Future()
 
         async def _got_resp(data: dict[str, Any]) -> None:
             if data["Type"] == msg_type:
                 future.set_result(data)
                 self._internal_callback = None
 
         self._internal_callback = _got_resp
 
         try:
-            result = await asyncio.wait_for(future, timeout=10.0)
+            result = await asyncio.wait_for(future, timeout=timeout)
         except asyncio.TimeoutError:
             raise
 
         return result
 
-    async def _await_for_dev_state_report(self: Linear) -> dict[str, Any]:
+    async def _await_for_dev_state_report(
+        self: Linear, device_id: str
+    ) -> dict[str, Any]:
         future: asyncio.Future[dict[str, Any]] = asyncio.Future()
 
         async def _got_resp(response: dict[str, Any]) -> None:
             if (
                 response["Type"] == MessageTypes.DEVICE_STATE.value
                 and response["Headers"]["Type"] == "Report"
+                and response["Headers"]["SendingDeviceID"] == "H/" + device_id
             ):
                 future.set_result(response)
                 self._internal_callback = None
 
         self._internal_callback = _got_resp
 
         try:
@@ -529,27 +534,32 @@
                 "Targets": device_id,
                 "SendingDeviceID": self._device_id,
             },
         )
 
         await self._ws.send_str(hello_request)
 
+        try:
+            await self._await_for_msg_type(MessageTypes.WELCOME.value, timeout=2.0)
+        except asyncio.TimeoutError:
+            pass
+
         state_request = create_request(
             MessageTypes.REQUEST_DEVICE_STATE,
             {
                 "MessageID": self._get_message_id(),
                 "SendingUserID": self._user_id.upper(),
                 "Targets": "H/" + device_id,
                 "SendingDeviceID": self._device_id,
             },
         )
 
         await self._ws.send_str(state_request)
 
-        response = await self._await_for_dev_state_report()
+        response = await self._await_for_dev_state_report(device_id)
 
         subdev_props: dict[str, dict[str, str]] = {}
 
         for key in response["Headers"].keys():
             if key.startswith("SubDev-"):
                 subdev_name = key.split("SubDev-")[1]
                 subdev_props[subdev_name] = {}
```

### Comparing `linear_garage_door-0.2.5/src/linear_garage_door/_util.py` & `linear_garage_door-0.2.6/src/linear_garage_door/_util.py`

 * *Files identical despite different names*

### Comparing `linear_garage_door-0.2.5/src/linear_garage_door/const.py` & `linear_garage_door-0.2.6/src/linear_garage_door/const.py`

 * *Files identical despite different names*

### Comparing `linear_garage_door-0.2.5/src/linear_garage_door/errors.py` & `linear_garage_door-0.2.6/src/linear_garage_door/errors.py`

 * *Files identical despite different names*

### Comparing `linear_garage_door-0.2.5/src/linear_garage_door/ws.py` & `linear_garage_door-0.2.6/src/linear_garage_door/ws.py`

 * *Files identical despite different names*

### Comparing `linear_garage_door-0.2.5/PKG-INFO` & `linear_garage_door-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linear-garage-door
-Version: 0.2.5
+Version: 0.2.6
 Summary: Control Linear Garage Doors with Python
 Home-page: https://IceBotYT.github.io/linear-garage-door
 License: MIT
 Author: IceBotYT
 Author-email: icebotyt@outlook.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
```

