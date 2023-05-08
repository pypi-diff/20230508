# Comparing `tmp/rubx-9.0.4.tar.gz` & `tmp/rubx-9.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rubx-9.0.4.tar", last modified: Wed Dec 21 11:33:21 2022, max compression
+gzip compressed data, was "rubx-9.0.6.tar", last modified: Thu Dec 22 20:49:22 2022, max compression
```

## Comparing `rubx-9.0.4.tar` & `rubx-9.0.6.tar`

### file list

```diff
@@ -1,44 +1,47 @@
-drwxrwxrwx   0        0        0        0 2022-12-21 11:33:21.055305 rubx-9.0.4/
--rw-rw-rw-   0        0        0     4957 2022-12-21 11:33:21.052306 rubx-9.0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2022-12-21 11:33:20.879595 rubx-9.0.4/rub/
--rw-rw-rw-   0        0        0      331 2022-12-21 10:53:52.000000 rubx-9.0.4/rub/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-21 11:33:20.925965 rubx-9.0.4/rub/client/
--rw-rw-rw-   0        0        0    10788 2022-12-21 10:54:51.000000 rubx-9.0.4/rub/client/ChannelMethods.py
--rw-rw-rw-   0        0        0    30314 2022-12-21 10:55:00.000000 rubx-9.0.4/rub/client/GroupMethods.py
--rw-rw-rw-   0        0        0     7653 2022-12-21 10:57:30.000000 rubx-9.0.4/rub/client/Rubino.py
--rw-rw-rw-   0        0        0     2981 2022-12-21 10:57:48.000000 rubx-9.0.4/rub/client/Socket.py
--rw-rw-rw-   0        0        0    85366 2022-12-21 10:58:57.000000 rubx-9.0.4/rub/client/UserMethods.py
--rw-rw-rw-   0        0        0       32 2022-12-21 10:44:05.000000 rubx-9.0.4/rub/client/__init__.py
--rw-rw-rw-   0        0        0      839 2022-12-19 20:15:04.000000 rubx-9.0.4/rub/client/access.py
--rw-rw-rw-   0        0        0    10278 2022-12-21 10:55:42.000000 rubx-9.0.4/rub/client/handlers.py
--rw-rw-rw-   0        0        0     6906 2022-12-21 10:57:05.000000 rubx-9.0.4/rub/client/main.py
--rw-rw-rw-   0        0        0      281 2022-12-21 10:42:42.000000 rubx-9.0.4/rub/client/rubikaclient.py
-drwxrwxrwx   0        0        0        0 2022-12-21 11:33:20.930962 rubx-9.0.4/rub/clients/
--rw-rw-rw-   0        0        0       46 2022-12-20 23:17:41.000000 rubx-9.0.4/rub/clients/__init__.py
--rw-rw-rw-   0        0        0      851 2022-12-20 23:16:58.000000 rubx-9.0.4/rub/clients/infos.py
-drwxrwxrwx   0        0        0        0 2022-12-21 11:33:20.935960 rubx-9.0.4/rub/crypto/
--rw-rw-rw-   0        0        0       15 2022-12-20 22:17:03.000000 rubx-9.0.4/rub/crypto/__init__.py
--rw-rw-rw-   0        0        0     1026 2022-12-20 19:05:23.000000 rubx-9.0.4/rub/crypto/crypto.py
-drwxrwxrwx   0        0        0        0 2022-12-21 11:33:20.943954 rubx-9.0.4/rub/exceptions/
--rw-rw-rw-   0        0        0       15 2022-12-20 22:17:03.000000 rubx-9.0.4/rub/exceptions/__init__.py
--rw-rw-rw-   0        0        0     1589 2022-12-21 11:27:06.000000 rubx-9.0.4/rub/exceptions/exceptions.py
-drwxrwxrwx   0        0        0        0 2022-12-21 11:33:20.948951 rubx-9.0.4/rub/network/
--rw-rw-rw-   0        0        0       15 2022-12-20 22:16:04.000000 rubx-9.0.4/rub/network/__init__.py
--rw-rw-rw-   0        0        0     5693 2022-12-21 11:00:00.000000 rubx-9.0.4/rub/network/connector.py
-drwxrwxrwx   0        0        0        0 2022-12-21 11:33:20.953948 rubx-9.0.4/rub/sessions/
--rw-rw-rw-   0        0        0       15 2022-12-20 22:17:03.000000 rubx-9.0.4/rub/sessions/__init__.py
--rw-rw-rw-   0        0        0     2434 2022-12-19 13:33:43.000000 rubx-9.0.4/rub/sessions/sql.py
-drwxrwxrwx   0        0        0        0 2022-12-21 11:33:20.969939 rubx-9.0.4/rub/tools/
--rw-rw-rw-   0        0        0       15 2022-12-20 22:17:03.000000 rubx-9.0.4/rub/tools/__init__.py
--rw-rw-rw-   0        0        0     4195 2022-12-20 22:13:52.000000 rubx-9.0.4/rub/tools/replacer.py
--rw-rw-rw-   0        0        0     2810 2022-12-21 10:11:17.000000 rubx-9.0.4/rub/tools/tools.py
--rw-rw-rw-   0        0        0      815 2022-12-20 22:14:29.000000 rubx-9.0.4/rub/tools/updator.py
-drwxrwxrwx   0        0        0        0 2022-12-21 11:33:21.050306 rubx-9.0.4/rubx.egg-info/
--rw-rw-rw-   0        0        0     4957 2022-12-21 11:33:19.000000 rubx-9.0.4/rubx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      750 2022-12-21 11:33:20.000000 rubx-9.0.4/rubx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-21 11:33:19.000000 rubx-9.0.4/rubx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-12-21 11:33:19.000000 rubx-9.0.4/rubx.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       26 2022-12-21 11:33:19.000000 rubx-9.0.4/rubx.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2022-12-21 11:33:19.000000 rubx-9.0.4/rubx.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-12-21 11:33:21.055305 rubx-9.0.4/setup.cfg
--rw-rw-rw-   0        0        0     5347 2022-12-21 11:00:29.000000 rubx-9.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2022-12-22 20:49:21.946864 rubx-9.0.6/
+-rw-rw-rw-   0        0        0     4957 2022-12-22 20:49:21.930874 rubx-9.0.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2022-12-22 20:49:20.923386 rubx-9.0.6/rb/
+-rw-rw-rw-   0        0        0      196 2022-12-22 20:30:33.000000 rubx-9.0.6/rb/__init__.py
+drwxrwxrwx   0        0        0        0 2022-12-22 20:49:21.129368 rubx-9.0.6/rb/client/
+-rw-rw-rw-   0        0        0    10767 2022-12-22 20:31:00.000000 rubx-9.0.6/rb/client/ChannelMethods.py
+-rw-rw-rw-   0        0        0    30287 2022-12-22 20:30:52.000000 rubx-9.0.6/rb/client/GroupMethods.py
+-rw-rw-rw-   0        0        0     7643 2022-12-22 20:21:54.000000 rubx-9.0.6/rb/client/Rubino.py
+-rw-rw-rw-   0        0        0     2974 2022-12-22 20:21:59.000000 rubx-9.0.6/rb/client/Socket.py
+-rw-rw-rw-   0        0        0    85246 2022-12-22 20:31:28.000000 rubx-9.0.6/rb/client/UserMethods.py
+-rw-rw-rw-   0        0        0      235 2022-12-22 20:13:55.000000 rubx-9.0.6/rb/client/__init__.py
+-rw-rw-rw-   0        0        0    10263 2022-12-22 20:21:20.000000 rubx-9.0.6/rb/client/handlers.py
+-rw-rw-rw-   0        0        0       15 2022-12-22 20:41:40.000000 rubx-9.0.6/rb/client/rubikaclient.py
+drwxrwxrwx   0        0        0        0 2022-12-22 20:49:21.133365 rubx-9.0.6/rb/clients/
+-rw-rw-rw-   0        0        0       34 2022-12-22 20:21:11.000000 rubx-9.0.6/rb/clients/__init__.py
+-rw-rw-rw-   0        0        0      851 2022-12-20 23:16:58.000000 rubx-9.0.6/rb/clients/infos.py
+drwxrwxrwx   0        0        0        0 2022-12-22 20:49:21.137363 rubx-9.0.6/rb/crypto/
+-rw-rw-rw-   0        0        0       30 2022-12-21 16:02:42.000000 rubx-9.0.6/rb/crypto/__init__.py
+-rw-rw-rw-   0        0        0     1026 2022-12-20 19:05:23.000000 rubx-9.0.6/rb/crypto/crypto.py
+drwxrwxrwx   0        0        0        0 2022-12-22 20:49:21.141360 rubx-9.0.6/rb/exceptions/
+-rw-rw-rw-   0        0        0      214 2022-12-22 20:35:37.000000 rubx-9.0.6/rb/exceptions/__init__.py
+-rw-rw-rw-   0        0        0     1750 2022-12-22 13:41:36.000000 rubx-9.0.6/rb/exceptions/exceptions.py
+-rw-rw-rw-   0        0        0     6828 2022-12-22 20:29:22.000000 rubx-9.0.6/rb/main.py
+drwxrwxrwx   0        0        0        0 2022-12-22 20:49:21.148356 rubx-9.0.6/rb/network/
+-rw-rw-rw-   0        0        0       65 2022-12-22 20:15:23.000000 rubx-9.0.6/rb/network/__init__.py
+-rw-rw-rw-   0        0        0     5669 2022-12-22 20:27:51.000000 rubx-9.0.6/rb/network/connector.py
+drwxrwxrwx   0        0        0        0 2022-12-22 20:49:21.289269 rubx-9.0.6/rb/options/
+-rw-rw-rw-   0        0        0       21 2022-12-22 20:15:40.000000 rubx-9.0.6/rb/options/__init__.py
+-rw-rw-rw-   0        0        0      839 2022-12-19 20:15:04.000000 rubx-9.0.6/rb/options/access.py
+-rw-rw-rw-   0        0        0      243 2022-12-22 20:20:43.000000 rubx-9.0.6/rb/rubikaclient.py
+drwxrwxrwx   0        0        0        0 2022-12-22 20:49:21.518129 rubx-9.0.6/rb/sessions/
+-rw-rw-rw-   0        0        0       30 2022-12-21 16:03:30.000000 rubx-9.0.6/rb/sessions/__init__.py
+-rw-rw-rw-   0        0        0     2434 2022-12-19 13:33:43.000000 rubx-9.0.6/rb/sessions/sql.py
+drwxrwxrwx   0        0        0        0 2022-12-22 20:49:21.652047 rubx-9.0.6/rb/tools/
+-rw-rw-rw-   0        0        0      115 2022-12-22 20:29:44.000000 rubx-9.0.6/rb/tools/__init__.py
+-rw-rw-rw-   0        0        0     4195 2022-12-20 22:13:52.000000 rubx-9.0.6/rb/tools/replacer.py
+-rw-rw-rw-   0        0        0     2812 2022-12-22 20:28:32.000000 rubx-9.0.6/rb/tools/tools.py
+-rw-rw-rw-   0        0        0      815 2022-12-20 22:14:29.000000 rubx-9.0.6/rb/tools/updator.py
+drwxrwxrwx   0        0        0        0 2022-12-22 20:49:21.927877 rubx-9.0.6/rubx.egg-info/
+-rw-rw-rw-   0        0        0     4957 2022-12-22 20:49:18.000000 rubx-9.0.6/rubx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      761 2022-12-22 20:49:19.000000 rubx-9.0.6/rubx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-12-22 20:49:18.000000 rubx-9.0.6/rubx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-12-22 20:49:18.000000 rubx-9.0.6/rubx.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       26 2022-12-22 20:49:18.000000 rubx-9.0.6/rubx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        3 2022-12-22 20:49:18.000000 rubx-9.0.6/rubx.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2022-12-22 20:49:21.946864 rubx-9.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     5347 2022-12-22 20:40:28.000000 rubx-9.0.6/setup.py
```

### Comparing `rubx-9.0.4/PKG-INFO` & `rubx-9.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rubx
-Version: 9.0.4
+Version: 9.0.6
 Summary: Rubx Library For Rubika Messenger Of Iran For All
 Home-page: https://github.com/mester-root/rubx
 Download-URL: https://github.com/mester-root/rubx/releases/latest
 Author: Saleh
 Author-email: m3st3r.r00t@gmail.com
 License: MIT
 Project-URL: Tracker, https://github.com/mester-root/rubx/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rubx Version: 9.0.4 Summary: Rubx Library For
+Metadata-Version: 2.1 Name: rubx Version: 9.0.6 Summary: Rubx Library For
 Rubika Messenger Of Iran For All Home-page: https://github.com/mester-root/rubx
 Download-URL: https://github.com/mester-root/rubx/releases/latest Author: Saleh
 Author-email: m3st3r.r00t@gmail.com License: MIT Project-URL: Tracker, https://
 github.com/mester-root/rubx/issues Project-URL: Channel, https://t.me/
 rubx_library Project-URL: Source, https://github.com/mester-root/rubx Project-
 URL: Documentation, https://github.com/Mester-Root/rubx/blob/main/README.md
 Keywords:
```

### Comparing `rubx-9.0.4/rub/client/ChannelMethods.py` & `rubx-9.0.6/rb/client/ChannelMethods.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,18 +9,18 @@
     
     pass
     # import exceptions
     # raise exceptions.MainError('sorry! error in module imports please run app with: `python -m`')
 
 import typing
 
-from ..network.connector import GetData
+from ..network import GetData
 
 if typing.TYPE_CHECKING:
-    from .rubikaclient import Client
+    from .. import Client
 
 class ChannelMethods:
     
     def __enter__(
         self    :   (
             'Client'
             )
```

### Comparing `rubx-9.0.4/rub/client/GroupMethods.py` & `rubx-9.0.6/rb/client/GroupMethods.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 
 if __name__ == '__main__' and  __package__ == None or __package__ == '':
     import sys
     sys.path.append(path.join(path.dirname(__file__), '..'))
 
 import typing
 
-from ..network.connector import GetData
-from ..tools.tools import Clean, Maker, Scanner
+from ..network import GetData
+from ..tools import Clean, Maker, Scanner
 
 if typing.TYPE_CHECKING:
-    from .rubikaclient import Client
+    from .. import Client
 
 class GroupMethods:
 
     def __enter__(
         self    :   (
             'Client'
             )
```

### Comparing `rubx-9.0.4/rub/client/Rubino.py` & `rubx-9.0.6/rb/client/Rubino.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/bin/python
 
 from random import randint
 
 from requests import session as sn
 
-from ..network.connector import clients
+from ..network import clients
 
 
 class RubinoClient(
     clients,
     object):
 
     def __init__(
```

### Comparing `rubx-9.0.4/rub/client/Socket.py` & `rubx-9.0.6/rb/client/Socket.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/bin/python
 
 from json import dumps, loads
 
-from ..crypto.crypto import Encryption
+from ..crypto import Encryption
 
 
 class WebSocket(
     object,
     ):
 
     data: dict = {
```

### Comparing `rubx-9.0.4/rub/client/UserMethods.py` & `rubx-9.0.6/rb/client/UserMethods.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #!/bin/python
+
 from os import path
 
 if __name__ == '__main__' and  __package__ == None or __package__ == '':
     import sys
     sys.path.append(path.join(path.dirname(__file__), '..'))
 
 else:
@@ -17,23 +18,21 @@
 from pathlib import Path
 from random import choice, randint, sample
 from re import findall
 from time import sleep
 
 from requests import get, post
 
-from ..clients.infos import *
-from ..network.connector import (Connection, GetData, Make, Method, Urls,
-                                 clients)
-from ..tools.replacer import Metas, Tags
-from ..tools.tools import Clean, Maker, Scanner
-from .main import RubikaClient
+from .. import RubikaClient
+from ..clients import Device, Infos
+from ..network import GetData, Method
+from ..tools import Clean, Maker, Metas, Scanner, Tags
 
 if typing.TYPE_CHECKING:
-    from .rubikaclient import Client
+    from .. import Client
 
 class UserMethods:
 
 
     def __enter__(
         self    :   (
             'Client'
```

### Comparing `rubx-9.0.4/rub/client/access.py` & `rubx-9.0.6/rb/options/access.py`

 * *Files identical despite different names*

### Comparing `rubx-9.0.4/rub/client/handlers.py` & `rubx-9.0.6/rb/client/handlers.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 
 from json import dumps, loads
 from re import compile as com
 from re import findall, search, sub
 
 import websocket
 
-from ..crypto.crypto import Encryption
-from ..tools.tools import Scanner
-from .main import RubikaClient
-from .rubikaclient import Client
+from .. import RubikaClient
+from ..crypto import Encryption
+from ..rubikaclient import Client
+from ..tools import Scanner
 
 
 class NewMessage(Client):
 
     def reg(
         self,
         filters: list = None,
```

### Comparing `rubx-9.0.4/rub/client/main.py` & `rubx-9.0.6/rb/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,22 +5,21 @@
 import webbrowser
 from datetime import datetime
 from time import sleep
 from warnings import warn
 
 from requests import get
 
-from ..clients.infos import Device, Infos
-from ..crypto.crypto import Encryption
-from ..network.connector import Urls
-from ..sessions.sql import SQLiteSession
-from ..tools.tools import Login
-from ..tools.updator import UpToDate
+from . import Client
 from . import __name__ as base
-from .rubikaclient import Client
+from .clients import Device, Infos
+from .crypto import Encryption
+from .network import Urls
+from .sessions import SQLiteSession
+from .tools import Login, UpToDate
 
 
 class Version(str):
     __version__ =   '9.0.0'
     __author__  =   'saleh'
     __lisense__ =   'MIT'
```

### Comparing `rubx-9.0.4/rub/clients/infos.py` & `rubx-9.0.6/rb/clients/infos.py`

 * *Files identical despite different names*

### Comparing `rubx-9.0.4/rub/crypto/crypto.py` & `rubx-9.0.6/rb/crypto/crypto.py`

 * *Files identical despite different names*

### Comparing `rubx-9.0.4/rub/exceptions/exceptions.py` & `rubx-9.0.6/rb/exceptions/exceptions.py`

 * *Files 17% similar despite different names*

```diff
@@ -26,24 +26,27 @@
     ):
     ...
 
 class Errors(
     Exception
     ):
     
-    def MadeError(status: str) -> (bool or ...):
+    def MadeError(status: str, det: str) -> (bool or ...):
 
-        if 'NOT_REGISTERED' in status.upper():
-            raise NotREGISTERED('session key not found; please find your key in web.rubika.ir and try again.')
-        elif 'INVALID_INPUT' in status.upper():
-            raise InvalidInput('your inserts is not true; try again.')
-        elif 'TOO_REQUESTS' in status.upper():
-            raise TooREQUESTS('sorry; method has been limited, please try again later.')
-        elif 'INVALID_AUTH' in status.upper():
-            raise InvalidAUTH('sorry; server error or please check method arguments and try again.')
+        if status.upper() == 'ERROR_GENERIC' or status.upper() == 'ERROR_ACTION':
+            if 'NOT_REGISTERED' in det.upper():
+                raise NotREGISTERED('session key not found; please find your key in web.rubika.ir and try again.')
+            elif 'INVALID_INPUT' in det.upper():
+                raise InvalidInput('your inserts is not true; try again.')
+            elif 'TOO_REQUESTS' in det.upper():
+                raise TooREQUESTS('sorry; method has been limited, please try again later.')
+            elif 'INVALID_AUTH' in det.upper():
+                raise InvalidAUTH('sorry; server error or please check method arguments and try again.')
+            else:
+                return True
         else:
             return True
 
 class ClientConnectorError(object):
     
     @classmethod
     def __init__(cls, **kwargs: object) -> (...):
```

### Comparing `rubx-9.0.4/rub/network/connector.py` & `rubx-9.0.6/rb/network/connector.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 #!/bin/python
 
 from json import dumps, loads
 from random import choice, randint
 
 from requests import session
 
-from ..client.rubikaclient import Client
-from ..crypto.crypto import Encryption
-from ..exceptions.exceptions import *
-from ..sessions.sql import SQLiteSession
+from .. import Client
+from ..crypto import Encryption
+from ..exceptions import *
+from ..sessions import SQLiteSession
 
 
 class Urls(
     (str)
     ):
     
     def get_url() -> str:
@@ -55,15 +55,15 @@
     object,
     ):
     
     def evolution(message, key) -> (dict):
         
         res: dict = loads(Encryption(key).decrypt(message.get('data_enc')))
         
-        if Errors.MadeError(res.get('status') or 'TOO_REQUESTS'):
+        if Errors.MadeError(res.get('status') or '', res.get('status_det') or ''):
             return res
 
 class Connection(
     (
         dict
         )
     ):
```

### Comparing `rubx-9.0.4/rub/sessions/sql.py` & `rubx-9.0.6/rb/sessions/sql.py`

 * *Files identical despite different names*

### Comparing `rubx-9.0.4/rub/tools/replacer.py` & `rubx-9.0.6/rb/tools/replacer.py`

 * *Files identical despite different names*

### Comparing `rubx-9.0.4/rub/tools/tools.py` & `rubx-9.0.6/rb/tools/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 
 class Maker(
     object
     ):
 
     @staticmethod
     def check_link(link: str, key: str) -> (str):
-        from . import Client
+        from .. import Client
         with Client(key, banner=False) as client:
             
             if link.startswith('@') or search(r'rubika\.ir/\w{4,25}'):
 
                 link: str = link.replace('https://', '').replace('rubika.ir/', '')
                 result: dict = client.get_object_by_username(link.replace('@', '')).get('data')
                 result: dict = result.get('user') or result.get('channel') or result.get('group')
@@ -73,10 +73,10 @@
 
 class Login(
     object
     ):
 
     @staticmethod
     def SignIn(phone: str) -> (str):
-        from . import Client
+        from .. import Client
         return Client.sign_in(phone, Client.send_code(phone, input('send type is SMS/Interval : '), password=input('please enter your password : ') if input('insert password y/n : ').lower() == 'y' else None).get('data').get('phone_code_hash'), input('please enter activation code : ')).get('data').get('auth') or '0'
```

### Comparing `rubx-9.0.4/rub/tools/updator.py` & `rubx-9.0.6/rb/tools/updator.py`

 * *Files identical despite different names*

### Comparing `rubx-9.0.4/rubx.egg-info/PKG-INFO` & `rubx-9.0.6/rubx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rubx
-Version: 9.0.4
+Version: 9.0.6
 Summary: Rubx Library For Rubika Messenger Of Iran For All
 Home-page: https://github.com/mester-root/rubx
 Download-URL: https://github.com/mester-root/rubx/releases/latest
 Author: Saleh
 Author-email: m3st3r.r00t@gmail.com
 License: MIT
 Project-URL: Tracker, https://github.com/mester-root/rubx/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rubx Version: 9.0.4 Summary: Rubx Library For
+Metadata-Version: 2.1 Name: rubx Version: 9.0.6 Summary: Rubx Library For
 Rubika Messenger Of Iran For All Home-page: https://github.com/mester-root/rubx
 Download-URL: https://github.com/mester-root/rubx/releases/latest Author: Saleh
 Author-email: m3st3r.r00t@gmail.com License: MIT Project-URL: Tracker, https://
 github.com/mester-root/rubx/issues Project-URL: Channel, https://t.me/
 rubx_library Project-URL: Source, https://github.com/mester-root/rubx Project-
 URL: Documentation, https://github.com/Mester-Root/rubx/blob/main/README.md
 Keywords:
```

### Comparing `rubx-9.0.4/setup.py` & `rubx-9.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/bin/python
 
 from setuptools import find_packages, setup
 
 requires = ['requests', 'urllib3', 'datetime']
-version = '9.0.4'
+version = '9.0.6'
 
 readme = '''
 <p align="center">
     <a href="https://github.com/mester-root/rubx">
         <img src="https://raw.githubusercontent.com/Mester-Root/rubx/main/logo.png" alt="RUBX" width="128">
     </a>
     <br>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 #!/bin/python from setuptools import find_packages, setup requires =
-['requests', 'urllib3', 'datetime'] version = '9.0.4' readme = '''
+['requests', 'urllib3', 'datetime'] version = '9.0.6' readme = '''
                                     [RUBX]
                             self lib for python 3
  document â¢â¢ telegram_channel â¢â¢ rubika_channel â¢â¢ rubika_group_-
                                  >_programmers
 ## rubx # EXAMPLES : ```python from rub import Client with Client('sessin') as
 client: client.send_message(...) ``` ## OR ``` python from rub.Rubino import
 Rubino with Rubino('session') as app: app.createPage(...) ``` ### coming soon
```

