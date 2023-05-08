# Comparing `tmp/wcfhttp-37.1.25.1.tar.gz` & `tmp/wcfhttp-37.1.25.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wcfhttp-37.1.25.1.tar", last modified: Mon May  8 08:40:56 2023, max compression
+gzip compressed data, was "wcfhttp-37.1.25.2.tar", last modified: Mon May  8 09:01:04 2023, max compression
```

## Comparing `wcfhttp-37.1.25.1.tar` & `wcfhttp-37.1.25.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 08:40:56.340636 wcfhttp-37.1.25.1/
--rw-rw-rw-   0        0        0       46 2023-05-08 03:47:03.000000 wcfhttp-37.1.25.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1829 2023-05-08 08:40:56.340636 wcfhttp-37.1.25.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-05-08 08:40:56.340636 wcfhttp-37.1.25.1/setup.cfg
--rw-rw-rw-   0        0        0     1439 2023-05-08 08:39:05.000000 wcfhttp-37.1.25.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:40:56.325013 wcfhttp-37.1.25.1/wcfhttp/
--rw-rw-rw-   0        0        0       69 2023-05-08 03:47:03.000000 wcfhttp-37.1.25.1/wcfhttp/__init__.py
--rw-rw-rw-   0        0        0    14424 2023-05-08 08:38:29.000000 wcfhttp-37.1.25.1/wcfhttp/core.py
--rw-rw-rw-   0        0        0     1780 2023-05-08 03:47:03.000000 wcfhttp-37.1.25.1/wcfhttp/main.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:40:56.340636 wcfhttp-37.1.25.1/wcfhttp.egg-info/
--rw-rw-rw-   0        0        0     1829 2023-05-08 08:40:56.000000 wcfhttp-37.1.25.1/wcfhttp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      260 2023-05-08 08:40:56.000000 wcfhttp-37.1.25.1/wcfhttp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 08:40:56.000000 wcfhttp-37.1.25.1/wcfhttp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-05-08 08:40:56.000000 wcfhttp-37.1.25.1/wcfhttp.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       56 2023-05-08 08:40:56.000000 wcfhttp-37.1.25.1/wcfhttp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-08 08:40:56.000000 wcfhttp-37.1.25.1/wcfhttp.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-08 09:01:04.493223 wcfhttp-37.1.25.2/
+-rw-rw-rw-   0        0        0       46 2023-05-08 03:47:03.000000 wcfhttp-37.1.25.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1829 2023-05-08 09:01:04.493223 wcfhttp-37.1.25.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-05-08 09:01:04.493223 wcfhttp-37.1.25.2/setup.cfg
+-rw-rw-rw-   0        0        0     1439 2023-05-08 08:39:05.000000 wcfhttp-37.1.25.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 09:01:04.477599 wcfhttp-37.1.25.2/wcfhttp/
+-rw-rw-rw-   0        0        0       69 2023-05-08 03:47:03.000000 wcfhttp-37.1.25.2/wcfhttp/__init__.py
+-rw-rw-rw-   0        0        0    14482 2023-05-08 08:59:43.000000 wcfhttp-37.1.25.2/wcfhttp/core.py
+-rw-rw-rw-   0        0        0     1780 2023-05-08 03:47:03.000000 wcfhttp-37.1.25.2/wcfhttp/main.py
+drwxrwxrwx   0        0        0        0 2023-05-08 09:01:04.493223 wcfhttp-37.1.25.2/wcfhttp.egg-info/
+-rw-rw-rw-   0        0        0     1829 2023-05-08 09:01:04.000000 wcfhttp-37.1.25.2/wcfhttp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      260 2023-05-08 09:01:04.000000 wcfhttp-37.1.25.2/wcfhttp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 09:01:04.000000 wcfhttp-37.1.25.2/wcfhttp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-05-08 09:01:04.000000 wcfhttp-37.1.25.2/wcfhttp.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       56 2023-05-08 09:01:04.000000 wcfhttp-37.1.25.2/wcfhttp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-08 09:01:04.000000 wcfhttp-37.1.25.2/wcfhttp.egg-info/top_level.txt
```

### Comparing `wcfhttp-37.1.25.1/PKG-INFO` & `wcfhttp-37.1.25.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wcfhttp
-Version: 37.1.25.1
+Version: 37.1.25.2
 Summary: 一个玩微信的工具
 Home-page: https://github.com/lich0821/WeChatFerry
 Author: Changhua
 Author-email: lichanghua0821@gmail.com
 License: MIT
 Project-URL: Documentation, https://wechatferry.readthedocs.io/zh/latest/index.html
 Project-URL: GitHub, https://github.com/lich0821/WeChatFerry/
```

### Comparing `wcfhttp-37.1.25.1/setup.py` & `wcfhttp-37.1.25.2/setup.py`

 * *Files identical despite different names*

### Comparing `wcfhttp-37.1.25.1/wcfhttp/core.py` & `wcfhttp-37.1.25.2/wcfhttp/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from typing import Any
 
 import requests
 from fastapi import Body, FastAPI
 from pydantic import BaseModel
 from wcferry import Wcf, WxMsg
 
-__version__ = "37.1.25.1"
+__version__ = "37.1.25.2"
 
 
 class Msg(BaseModel):
     id: str
     type: int
     xml: str
     sender: str
@@ -29,14 +29,15 @@
 
 class Http(FastAPI):
     """WeChatFerry HTTP 客户端，文档地址：http://IP:PORT/docs"""
 
     def __init__(self, wcf: Wcf, cb: str, **extra: Any) -> None:
         super().__init__(**extra)
         self.LOG = logging.getLogger(__name__)
+        self.LOG.info(f"wcfhttp version: {__version__}")
         self.wcf = wcf
         self._set_cb(cb)
         self.add_api_route("/msg_cb", self.msg_cb, methods=["POST"], summary="接收消息回调样例", tags=["示例"])
 
         self.add_api_route("/login", self.is_login, methods=["GET"], summary="获取登录状态")
         self.add_api_route("/wxid", self.get_self_wxid, methods=["GET"], summary="获取登录账号 wxid")
         self.add_api_route("/user-info", self.get_user_info, methods=["GET"], summary="获取登录账号个人信息")
```

### Comparing `wcfhttp-37.1.25.1/wcfhttp/main.py` & `wcfhttp-37.1.25.2/wcfhttp/main.py`

 * *Files identical despite different names*

### Comparing `wcfhttp-37.1.25.1/wcfhttp.egg-info/PKG-INFO` & `wcfhttp-37.1.25.2/wcfhttp.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wcfhttp
-Version: 37.1.25.1
+Version: 37.1.25.2
 Summary: 一个玩微信的工具
 Home-page: https://github.com/lich0821/WeChatFerry
 Author: Changhua
 Author-email: lichanghua0821@gmail.com
 License: MIT
 Project-URL: Documentation, https://wechatferry.readthedocs.io/zh/latest/index.html
 Project-URL: GitHub, https://github.com/lich0821/WeChatFerry/
```

