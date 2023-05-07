# Comparing `tmp/AlexaPy-1.8.4.tar.gz` & `tmp/AlexaPy-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AlexaPy-1.8.4.tar", last modified: Tue May 12 05:35:18 2020, max compression
+gzip compressed data, was "AlexaPy-1.9.0.tar", last modified: Mon May 18 06:46:08 2020, max compression
```

## Comparing `AlexaPy-1.8.4.tar` & `AlexaPy-1.9.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    10480 2020-05-12 05:33:59.000000 AlexaPy-1.8.4/LICENSE
--rw-r--r--   0        0        0    10480 2020-05-12 05:33:59.000000 AlexaPy-1.8.4/LICENSE
--rw-r--r--   0        0        0     1695 2020-05-12 05:33:59.000000 AlexaPy-1.8.4/README.md
--rw-r--r--   0        0        0      764 2020-05-12 05:33:59.000000 AlexaPy-1.8.4/alexapy/__init__.py
--rw-r--r--   0        0        0    37353 2020-05-12 05:33:59.000000 AlexaPy-1.8.4/alexapy/alexaapi.py
--rw-r--r--   0        0        0    31798 2020-05-12 05:33:59.000000 AlexaPy-1.8.4/alexapy/alexalogin.py
--rw-r--r--   0        0        0    13115 2020-05-12 05:33:59.000000 AlexaPy-1.8.4/alexapy/alexawebsocket.py
--rw-r--r--   0        0        0      360 2020-05-12 05:33:59.000000 AlexaPy-1.8.4/alexapy/const.py
--rw-r--r--   0        0        0     5786 2020-05-12 05:33:59.000000 AlexaPy-1.8.4/alexapy/cookiejar.py
--rw-r--r--   0        0        0      677 2020-05-12 05:33:59.000000 AlexaPy-1.8.4/alexapy/errors.py
--rw-r--r--   0        0        0     2989 2020-05-12 05:33:59.000000 AlexaPy-1.8.4/alexapy/helpers.py
--rw-r--r--   0        0        0      951 2020-05-12 05:35:14.000000 AlexaPy-1.8.4/pyproject.toml
--rw-r--r--   0        0        0     2505 2020-05-12 05:35:18.147532 AlexaPy-1.8.4/setup.py
--rw-r--r--   0        0        0     2595 2020-05-12 05:35:18.147976 AlexaPy-1.8.4/PKG-INFO
+-rw-r--r--   0        0        0    10480 2020-05-18 06:44:44.000000 AlexaPy-1.9.0/LICENSE
+-rw-r--r--   0        0        0    10480 2020-05-18 06:44:44.000000 AlexaPy-1.9.0/LICENSE
+-rw-r--r--   0        0        0     1695 2020-05-18 06:44:44.000000 AlexaPy-1.9.0/README.md
+-rw-r--r--   0        0        0      764 2020-05-18 06:44:44.000000 AlexaPy-1.9.0/alexapy/__init__.py
+-rw-r--r--   0        0        0    38563 2020-05-18 06:44:44.000000 AlexaPy-1.9.0/alexapy/alexaapi.py
+-rw-r--r--   0        0        0    31798 2020-05-18 06:44:44.000000 AlexaPy-1.9.0/alexapy/alexalogin.py
+-rw-r--r--   0        0        0    13115 2020-05-18 06:44:44.000000 AlexaPy-1.9.0/alexapy/alexawebsocket.py
+-rw-r--r--   0        0        0      360 2020-05-18 06:44:44.000000 AlexaPy-1.9.0/alexapy/const.py
+-rw-r--r--   0        0        0     5786 2020-05-18 06:44:44.000000 AlexaPy-1.9.0/alexapy/cookiejar.py
+-rw-r--r--   0        0        0      677 2020-05-18 06:44:44.000000 AlexaPy-1.9.0/alexapy/errors.py
+-rw-r--r--   0        0        0     2989 2020-05-18 06:44:44.000000 AlexaPy-1.9.0/alexapy/helpers.py
+-rw-r--r--   0        0        0      951 2020-05-18 06:46:01.000000 AlexaPy-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0     2505 2020-05-18 06:46:08.211073 AlexaPy-1.9.0/setup.py
+-rw-r--r--   0        0        0     2595 2020-05-18 06:46:08.211513 AlexaPy-1.9.0/PKG-INFO
```

### Comparing `AlexaPy-1.8.4/LICENSE` & `AlexaPy-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `AlexaPy-1.8.4/README.md` & `AlexaPy-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `AlexaPy-1.8.4/alexapy/__init__.py` & `AlexaPy-1.9.0/alexapy/__init__.py`

 * *Files identical despite different names*

### Comparing `AlexaPy-1.8.4/alexapy/alexaapi.py` & `AlexaPy-1.9.0/alexapy/alexaapi.py`

 * *Files 3% similar despite different names*

```diff
@@ -283,16 +283,20 @@
         Alexa.Calendar.PlayTomorrow
         Alexa.Calendar.PlayToday
         Alexa.Calendar.PlayNext
         https://github.com/custom-components/alexa_media_player/wiki#sequence-commands-versions--100
 
         """
         operation_payload = {
-            "deviceType": self._device._device_type,
-            "deviceSerialNumber": self._device.unique_id,
+            "devices": [
+                {
+                    "deviceType": self._device._device_type,
+                    "deviceSerialNumber": self._device.unique_id,
+                }
+            ],
             "locale": (self._device._locale if self._device._locale else "en-US"),
             "customerId": self._device._device_owner_customer_id,
         }
         if kwargs is not None:
             operation_payload.update(kwargs)
         node_data = {
             "@type": "com.amazon.alexa.behaviors.model.OpaquePayloadOperationNode",
@@ -433,14 +437,49 @@
             "Alexa.Sound",
             customerId=customer_id,
             soundStringId=sound_string_id,
             skillId="amzn1.ask.1p.sound",
             queue_delay=queue_delay,
         )
 
+    async def stop(
+        self,
+        customer_id: Text = None,
+        queue_delay: float = 1.5,
+        all_devices: bool = False,
+    ) -> None:
+        """Stop device playback.
+
+        Keyword Arguments:
+            customer_id {Text} -- CustomerId issuing command (default: {None})
+            queue_delay {float} -- The number of seconds to wait
+                                   for commands to queue together.
+                                   Must be positive.
+                                   (default: {1.5})
+            all_devices {bool} -- Whether all devices should be stopped (default: {False})
+
+        """
+        kwargs = {}
+
+        if all_devices:
+            kwargs["devices"] = (
+                {
+                    "deviceType": "ALEXA_ALL_DEVICE_TYPE",
+                    "deviceSerialNumber": "ALEXA_ALL_DSN",
+                },
+            )
+
+        await self.send_sequence(
+            "Alexa.DeviceControls.Stop",
+            skillId="amzn1.ask.1p.alexadevicecontrols",
+            customerId=customer_id,
+            queue_delay=queue_delay,
+            **kwargs
+        )
+
     def process_targets(
         self, targets: Optional[List[Text]] = None
     ) -> List[Dict[Text, Text]]:
         """Process targets list to generate list of devices.
 
         Keyword Arguments
             targets {Optional[List[Text]]} -- List of serial numbers
```

### Comparing `AlexaPy-1.8.4/alexapy/alexalogin.py` & `AlexaPy-1.9.0/alexapy/alexalogin.py`

 * *Files identical despite different names*

### Comparing `AlexaPy-1.8.4/alexapy/alexawebsocket.py` & `AlexaPy-1.9.0/alexapy/alexawebsocket.py`

 * *Files identical despite different names*

### Comparing `AlexaPy-1.8.4/alexapy/cookiejar.py` & `AlexaPy-1.9.0/alexapy/cookiejar.py`

 * *Files identical despite different names*

### Comparing `AlexaPy-1.8.4/alexapy/errors.py` & `AlexaPy-1.9.0/alexapy/errors.py`

 * *Files identical despite different names*

### Comparing `AlexaPy-1.8.4/alexapy/helpers.py` & `AlexaPy-1.9.0/alexapy/helpers.py`

 * *Files identical despite different names*

### Comparing `AlexaPy-1.8.4/pyproject.toml` & `AlexaPy-1.9.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #  SPDX-License-Identifier: Apache-2.0
 [tool.poetry]
 name = "AlexaPy"
-version = "1.8.4"
+version = "1.9.0"
 description = "Python API to control Amazon Echo Devices Programatically."
 authors = ["Keaton Taylor <keatonstaylor@gmail.com>", "Alan Tse <alandtse@gmail.com"]
 license = "Apache-2.0"
 readme = 'README.md'
 repository = "https://gitlab.com/keatontaylor/alexapy"
 keywords = ['amazon', 'alexa', 'homeassistant']
 include = ["LICENSE"]
```

### Comparing `AlexaPy-1.8.4/setup.py` & `AlexaPy-1.9.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
  'certifi',
  'requests',
  'simplejson',
  'yarl']
 
 setup_kwargs = {
     'name': 'alexapy',
-    'version': '1.8.4',
+    'version': '1.9.0',
     'description': 'Python API to control Amazon Echo Devices Programatically.',
     'long_description': '# alexapy\n\n[![pipeline status](https://gitlab.com/keatontaylor/alexapy/badges/master/pipeline.svg)](https://gitlab.com/keatontaylor/alexapy/commits/master)\n\nPython Package for controlling Alexa devices (echo dot, etc) programmatically. This was originally designed for [alexa_media_player](https://github.com/custom-components/alexa_media_player) a custom_component for [Home Assistant](https://www.home-assistant.io/).\n\n**NOTE:** Alexa has no official API; therefore, this library may stop\nworking at any time without warning.\n\n# Credits\nOriginally inspired by [this blog](https://blog.loetzimmer.de/2017/10/amazon-alexa-hort-auf-die-shell-echo.html) [(GitHub)](https://github.com/thorsten-gehrig/alexa-remote-control).\nAdditional scaffolding from [simplisafe-python](https://github.com/bachya/simplisafe-python)\n\n# Contributing\n\n1.  [Check for open features/bugs](https://gitlab.com/keatontaylor/alexapy/issues)\n  or [initiate a discussion on one](https://gitlab.com/keatontaylor/alexapy/issues/new).\n2.  [Fork the repository](https://gitlab.com/keatontaylor/alexapy/forks/new).\n3.  Install the dev environment: `make init`.\n4.  Enter the virtual environment: `pipenv shell`\n5.  Code your new feature or bug fix.\n6.  Write a test that covers your new functionality.\n7.  Update `README.md` with any new documentation.\n8.  Run tests and ensure 100% code coverage for your contribution: `make coverage`\n9.  Ensure you have no linting errors: `make lint`\n10. Ensure you have typed your code correctly: `make typing`\n11. Add yourself to `AUTHORS.md`.\n12. Submit a pull request!\n\n# License\n[Apache-2.0](LICENSE). By providing a contribution, you agree the contribution is licensed under Apache-2.0.\n',
     'author': 'Keaton Taylor',
     'author_email': 'keatonstaylor@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://gitlab.com/keatontaylor/alexapy',
```

### Comparing `AlexaPy-1.8.4/PKG-INFO` & `AlexaPy-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alexapy
-Version: 1.8.4
+Version: 1.9.0
 Summary: Python API to control Amazon Echo Devices Programatically.
 Home-page: https://gitlab.com/keatontaylor/alexapy
 License: Apache-2.0
 Keywords: amazon,alexa,homeassistant
 Author: Keaton Taylor
 Author-email: keatonstaylor@gmail.com
 Requires-Python: >=3.6,<4.0
```

