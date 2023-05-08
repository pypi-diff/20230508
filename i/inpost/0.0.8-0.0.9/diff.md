# Comparing `tmp/inpost-0.0.8.tar.gz` & `tmp/inpost-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inpost-0.0.8.tar", max compression
+gzip compressed data, was "inpost-0.0.9.tar", max compression
```

## Comparing `inpost-0.0.8.tar` & `inpost-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0       31 2023-01-08 12:39:56.709189 inpost-0.0.8/README.md
--rw-r--r--   0        0        0       24 2023-01-11 14:04:51.297207 inpost-0.0.8/inpost/__init__.py
--rw-r--r--   0        0        0    48840 2023-04-14 09:52:35.751540 inpost-0.0.8/inpost/api.py
--rw-r--r--   0        0        0     1105 2023-04-14 08:22:00.444589 inpost-0.0.8/inpost/static/__init__.py
--rw-r--r--   0        0        0     1663 2023-02-09 11:19:43.627615 inpost-0.0.8/inpost/static/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1736 2023-02-09 11:19:43.714281 inpost-0.0.8/inpost/static/__pycache__/endpoints.cpython-310.pyc
--rw-r--r--   0        0        0     3753 2023-02-09 11:19:43.710948 inpost-0.0.8/inpost/static/__pycache__/exceptions.cpython-310.pyc
--rw-r--r--   0        0        0     1056 2023-02-09 11:24:57.470311 inpost-0.0.8/inpost/static/__pycache__/friends.cpython-310.pyc
--rw-r--r--   0        0        0      202 2023-01-11 16:11:34.275165 inpost-0.0.8/inpost/static/__pycache__/headers.cpython-310.pyc
--rw-r--r--   0        0        0    22657 2023-02-09 11:19:43.637615 inpost-0.0.8/inpost/static/__pycache__/parcels.cpython-310.pyc
--rw-r--r--   0        0        0     7954 2023-01-19 11:34:51.801975 inpost-0.0.8/inpost/static/__pycache__/statuses.cpython-310.pyc
--rw-r--r--   0        0        0     1771 2023-03-04 13:33:30.709374 inpost-0.0.8/inpost/static/endpoints.py
--rw-r--r--   0        0        0     2515 2023-02-09 09:51:30.001451 inpost-0.0.8/inpost/static/exceptions.py
--rw-r--r--   0        0        0     1779 2023-02-09 12:35:10.844655 inpost-0.0.8/inpost/static/friends.py
--rw-r--r--   0        0        0       47 2023-01-08 12:39:56.709189 inpost-0.0.8/inpost/static/headers.py
--rw-r--r--   0        0        0    27154 2023-04-14 08:23:52.935000 inpost-0.0.8/inpost/static/parcels.py
--rw-r--r--   0        0        0     7066 2023-04-14 08:22:00.461255 inpost-0.0.8/inpost/static/statuses.py
--rw-r--r--   0        0        0     1026 2023-04-14 09:59:13.882104 inpost-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      872 1970-01-01 00:00:00.000000 inpost-0.0.8/setup.py
--rw-r--r--   0        0        0     1158 1970-01-01 00:00:00.000000 inpost-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0       31 2023-01-08 12:39:56.709189 inpost-0.0.9/README.md
+-rw-r--r--   0        0        0       24 2023-01-11 14:04:51.297207 inpost-0.0.9/inpost/__init__.py
+-rw-r--r--   0        0        0    48840 2023-04-14 09:52:35.751540 inpost-0.0.9/inpost/api.py
+-rw-r--r--   0        0        0     1105 2023-04-14 08:22:00.444589 inpost-0.0.9/inpost/static/__init__.py
+-rw-r--r--   0        0        0     1663 2023-02-09 11:19:43.627615 inpost-0.0.9/inpost/static/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1736 2023-02-09 11:19:43.714281 inpost-0.0.9/inpost/static/__pycache__/endpoints.cpython-310.pyc
+-rw-r--r--   0        0        0     3753 2023-02-09 11:19:43.710948 inpost-0.0.9/inpost/static/__pycache__/exceptions.cpython-310.pyc
+-rw-r--r--   0        0        0     1056 2023-02-09 11:24:57.470311 inpost-0.0.9/inpost/static/__pycache__/friends.cpython-310.pyc
+-rw-r--r--   0        0        0      202 2023-01-11 16:11:34.275165 inpost-0.0.9/inpost/static/__pycache__/headers.cpython-310.pyc
+-rw-r--r--   0        0        0    22657 2023-02-09 11:19:43.637615 inpost-0.0.9/inpost/static/__pycache__/parcels.cpython-310.pyc
+-rw-r--r--   0        0        0     7954 2023-01-19 11:34:51.801975 inpost-0.0.9/inpost/static/__pycache__/statuses.cpython-310.pyc
+-rw-r--r--   0        0        0     1771 2023-03-04 13:33:30.709374 inpost-0.0.9/inpost/static/endpoints.py
+-rw-r--r--   0        0        0     2515 2023-02-09 09:51:30.001451 inpost-0.0.9/inpost/static/exceptions.py
+-rw-r--r--   0        0        0     1779 2023-02-09 12:35:10.844655 inpost-0.0.9/inpost/static/friends.py
+-rw-r--r--   0        0        0       47 2023-01-08 12:39:56.709189 inpost-0.0.9/inpost/static/headers.py
+-rw-r--r--   0        0        0    27210 2023-04-14 10:17:16.303881 inpost-0.0.9/inpost/static/parcels.py
+-rw-r--r--   0        0        0     7066 2023-04-14 08:22:00.461255 inpost-0.0.9/inpost/static/statuses.py
+-rw-r--r--   0        0        0     1026 2023-04-14 10:19:18.478358 inpost-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      872 1970-01-01 00:00:00.000000 inpost-0.0.9/setup.py
+-rw-r--r--   0        0        0     1158 1970-01-01 00:00:00.000000 inpost-0.0.9/PKG-INFO
```

### Comparing `inpost-0.0.8/inpost/api.py` & `inpost-0.0.9/inpost/api.py`

 * *Files identical despite different names*

### Comparing `inpost-0.0.8/inpost/static/__init__.py` & `inpost-0.0.9/inpost/static/__init__.py`

 * *Files identical despite different names*

### Comparing `inpost-0.0.8/inpost/static/__pycache__/__init__.cpython-310.pyc` & `inpost-0.0.9/inpost/static/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `inpost-0.0.8/inpost/static/__pycache__/endpoints.cpython-310.pyc` & `inpost-0.0.9/inpost/static/__pycache__/endpoints.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `inpost-0.0.8/inpost/static/__pycache__/exceptions.cpython-310.pyc` & `inpost-0.0.9/inpost/static/__pycache__/exceptions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `inpost-0.0.8/inpost/static/__pycache__/friends.cpython-310.pyc` & `inpost-0.0.9/inpost/static/__pycache__/friends.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `inpost-0.0.8/inpost/static/__pycache__/parcels.cpython-310.pyc` & `inpost-0.0.9/inpost/static/__pycache__/parcels.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `inpost-0.0.8/inpost/static/__pycache__/statuses.cpython-310.pyc` & `inpost-0.0.9/inpost/static/__pycache__/statuses.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `inpost-0.0.8/inpost/static/endpoints.py` & `inpost-0.0.9/inpost/static/endpoints.py`

 * *Files identical despite different names*

### Comparing `inpost-0.0.8/inpost/static/exceptions.py` & `inpost-0.0.9/inpost/static/exceptions.py`

 * *Files identical despite different names*

### Comparing `inpost-0.0.8/inpost/static/friends.py` & `inpost-0.0.9/inpost/static/friends.py`

 * *Files identical despite different names*

### Comparing `inpost-0.0.8/inpost/static/parcels.py` & `inpost-0.0.9/inpost/static/parcels.py`

 * *Files 1% similar despite different names*

```diff
@@ -261,17 +261,14 @@
         self.expiry_date: arrow = parcel_data['expiryDate']
         self.sent_date: arrow = parcel_data['sentDate']
         self.delivered_date: arrow = parcel_data['deliveredDate']
         self.order_number: str = parcel_data['orderNumber']
         self.form_type: str = parcel_data['formType']
 
 
-
-
-
 class Receiver:
     """Object representation of :class:`Parcel` receiver
 
     :param receiver_data: :class:`dict` containing sender data for :class:`Parcel`
     :type receiver_data: dict
     :param logger: :class:`logging.Logger` parent instance
     :type logger: logging.Logger"""
@@ -408,15 +405,15 @@
         self.highlight: bool = operations_data['highlight']
         self.refresh_until: arrow = get(operations_data['refreshUntil'])
         self.request_easy_access_zone: str = operations_data['requestEasyAccessZone']
         self.is_voicebot: bool = operations_data['voicebot']
         self.can_share_to_observe: bool = operations_data['canShareToObserve']
         self.can_share_open_code: bool = operations_data['canShareOpenCode']
         self.can_share_parcel: bool = operations_data['canShareParcel']
-        self.send: bool = operations_data['send']
+        self.send: bool | None = operations_data['send'] if 'send' in operations_data else None
 
         self._log: logging.Logger = logger.getChild(__class__.__name__)
         self._log.debug('created')
 
     def __repr__(self):
         fields = tuple(f"{k}={v}" for k, v in self.__dict__.items() if k != '_log')
         return self.__class__.__name__ + str(tuple(sorted(fields))).replace("\'", "")
@@ -429,15 +426,16 @@
     :type eventlog_data: dict
     :param logger: :class:`logging.Logger` parent instance
     :type logger: logging.Logger"""
 
     def __init__(self, eventlog_data: dict, logger: logging.Logger):
         """Constructor method"""
         self.type: str = eventlog_data['type']
-        self.name: ParcelStatus | ReturnsStatus = ParcelStatus[eventlog_data['name']] if self.type == 'PARCEL_STATUS' else ReturnsStatus[eventlog_data['name']]
+        self.name: ParcelStatus | ReturnsStatus = ParcelStatus[
+            eventlog_data['name']] if self.type == 'PARCEL_STATUS' else ReturnsStatus[eventlog_data['name']]
         self.date: arrow = get(eventlog_data['date'])
 
         self._log: logging.Logger = logger.getChild(__class__.__name__)
         self._log.debug('created')
 
         if self.name == ParcelStatus.UNKNOWN or self.name == ReturnsStatus.UNKNOWN:
             self._log.debug(f'unknown {self.type}: {eventlog_data["name"]}')
```

### Comparing `inpost-0.0.8/inpost/static/statuses.py` & `inpost-0.0.9/inpost/static/statuses.py`

 * *Files identical despite different names*

### Comparing `inpost-0.0.8/pyproject.toml` & `inpost-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "inpost"
-version = "0.0.8"
+version = "0.0.9"
 description = "Asynchronous InPost package allowing you to manage existing incoming parcels without mobile app"
 authors = ["loboda4450 <loboda4450@gmail.com>", "MrKazik99 <mrkazik99@gmail.com>"]
 maintainers = ["loboda4450 <loboda4450@gmail.com>"]
 documentation = 'https://inpost-python.readthedocs.io/en/latest/index.html'
 repository = "https://github.com/IFOSSA/inpost-python"
 readme = "README.md"
 packages = [
```

### Comparing `inpost-0.0.8/setup.py` & `inpost-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['Pillow>=9.4.0,<10.0.0',
  'aiohttp>=3.8.1,<4.0.0',
  'arrow>=1.2.3,<2.0.0',
  'qrcode>=7.3.1,<8.0.0']
 
 setup_kwargs = {
     'name': 'inpost',
-    'version': '0.0.8',
+    'version': '0.0.9',
     'description': 'Asynchronous InPost package allowing you to manage existing incoming parcels without mobile app',
     'long_description': 'Fully async Inpost API library\n',
     'author': 'loboda4450',
     'author_email': 'loboda4450@gmail.com',
     'maintainer': 'loboda4450',
     'maintainer_email': 'loboda4450@gmail.com',
     'url': 'https://github.com/IFOSSA/inpost-python',
```

### Comparing `inpost-0.0.8/PKG-INFO` & `inpost-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inpost
-Version: 0.0.8
+Version: 0.0.9
 Summary: Asynchronous InPost package allowing you to manage existing incoming parcels without mobile app
 Home-page: https://github.com/IFOSSA/inpost-python
 Author: loboda4450
 Author-email: loboda4450@gmail.com
 Maintainer: loboda4450
 Maintainer-email: loboda4450@gmail.com
 Requires-Python: >=3.10,<4.0
```

