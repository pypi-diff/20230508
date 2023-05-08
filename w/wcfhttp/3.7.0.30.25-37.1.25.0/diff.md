# Comparing `tmp/wcfhttp-3.7.0.30.25.tar.gz` & `tmp/wcfhttp-37.1.25.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wcfhttp-3.7.0.30.25.tar", last modified: Sat May  6 15:35:16 2023, max compression
+gzip compressed data, was "wcfhttp-37.1.25.0.tar", last modified: Mon May  8 05:34:59 2023, max compression
```

## Comparing `wcfhttp-3.7.0.30.25.tar` & `wcfhttp-37.1.25.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 chuck      (501) staff       (20)        0 2023-05-06 15:35:16.112958 wcfhttp-3.7.0.30.25/
--rw-r--r--   0 chuck      (501) staff       (20)       44 2023-05-05 15:29:35.000000 wcfhttp-3.7.0.30.25/MANIFEST.in
--rw-r--r--   0 chuck      (501) staff       (20)     1290 2023-05-06 15:35:16.112553 wcfhttp-3.7.0.30.25/PKG-INFO
--rw-r--r--   0 chuck      (501) staff       (20)       38 2023-05-06 15:35:16.113096 wcfhttp-3.7.0.30.25/setup.cfg
--rw-r--r--   0 chuck      (501) staff       (20)     1389 2023-05-06 07:14:27.000000 wcfhttp-3.7.0.30.25/setup.py
-drwxr-xr-x   0 chuck      (501) staff       (20)        0 2023-05-06 15:35:16.108041 wcfhttp-3.7.0.30.25/wcfhttp/
--rw-r--r--   0 chuck      (501) staff       (20)       67 2023-05-06 06:41:48.000000 wcfhttp-3.7.0.30.25/wcfhttp/__init__.py
--rw-r--r--   0 chuck      (501) staff       (20)    11045 2023-05-06 15:09:26.000000 wcfhttp-3.7.0.30.25/wcfhttp/core.py
--rw-r--r--   0 chuck      (501) staff       (20)     1740 2023-05-06 10:36:26.000000 wcfhttp-3.7.0.30.25/wcfhttp/main.py
-drwxr-xr-x   0 chuck      (501) staff       (20)        0 2023-05-06 15:35:16.111999 wcfhttp-3.7.0.30.25/wcfhttp.egg-info/
--rw-r--r--   0 chuck      (501) staff       (20)     1290 2023-05-06 15:35:15.000000 wcfhttp-3.7.0.30.25/wcfhttp.egg-info/PKG-INFO
--rw-r--r--   0 chuck      (501) staff       (20)      260 2023-05-06 15:35:16.000000 wcfhttp-3.7.0.30.25/wcfhttp.egg-info/SOURCES.txt
--rw-r--r--   0 chuck      (501) staff       (20)        1 2023-05-06 15:35:15.000000 wcfhttp-3.7.0.30.25/wcfhttp.egg-info/dependency_links.txt
--rw-r--r--   0 chuck      (501) staff       (20)       46 2023-05-06 15:35:15.000000 wcfhttp-3.7.0.30.25/wcfhttp.egg-info/entry_points.txt
--rw-r--r--   0 chuck      (501) staff       (20)       58 2023-05-06 15:35:15.000000 wcfhttp-3.7.0.30.25/wcfhttp.egg-info/requires.txt
--rw-r--r--   0 chuck      (501) staff       (20)        8 2023-05-06 15:35:15.000000 wcfhttp-3.7.0.30.25/wcfhttp.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-08 05:34:59.127354 wcfhttp-37.1.25.0/
+-rw-rw-rw-   0        0        0       46 2023-05-08 03:47:03.000000 wcfhttp-37.1.25.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     1335 2023-05-08 05:34:59.126355 wcfhttp-37.1.25.0/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-05-08 05:34:59.127354 wcfhttp-37.1.25.0/setup.cfg
+-rw-rw-rw-   0        0        0     1439 2023-05-08 03:47:03.000000 wcfhttp-37.1.25.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 05:34:59.112358 wcfhttp-37.1.25.0/wcfhttp/
+-rw-rw-rw-   0        0        0       69 2023-05-08 03:47:03.000000 wcfhttp-37.1.25.0/wcfhttp/__init__.py
+-rw-rw-rw-   0        0        0    11268 2023-05-08 04:13:05.000000 wcfhttp-37.1.25.0/wcfhttp/core.py
+-rw-rw-rw-   0        0        0     1780 2023-05-08 03:47:03.000000 wcfhttp-37.1.25.0/wcfhttp/main.py
+drwxrwxrwx   0        0        0        0 2023-05-08 05:34:59.124357 wcfhttp-37.1.25.0/wcfhttp.egg-info/
+-rw-rw-rw-   0        0        0     1335 2023-05-08 05:34:58.000000 wcfhttp-37.1.25.0/wcfhttp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      260 2023-05-08 05:34:59.000000 wcfhttp-37.1.25.0/wcfhttp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 05:34:58.000000 wcfhttp-37.1.25.0/wcfhttp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-05-08 05:34:58.000000 wcfhttp-37.1.25.0/wcfhttp.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       56 2023-05-08 05:34:58.000000 wcfhttp-37.1.25.0/wcfhttp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-08 05:34:58.000000 wcfhttp-37.1.25.0/wcfhttp.egg-info/top_level.txt
```

### Comparing `wcfhttp-3.7.0.30.25/setup.py` & `wcfhttp-37.1.25.0/setup.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,50 +1,50 @@
-#! /usr/bin/env python3
-# -*- coding: utf-8 -*-
-
-
-from __future__ import print_function
-from setuptools import setup, find_packages
-
-import wcfhttp
-
-with open("README.md", "r", encoding="utf-8") as fh:
-    long_description = fh.read()
-
-
-setup(
-    name="wcfhttp",
-    version=wcfhttp.core.__version__,
-    author="Changhua",
-    author_email="lichanghua0821@gmail.com",
-    description="一个玩微信的工具",
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    license="MIT",
-    url="https://github.com/lich0821/WeChatFerry",
-    python_requires=">=3.8",
-    packages=find_packages(),
-    include_package_data=True,
-    entry_points={
-        'console_scripts': [
-            'wcfhttp=wcfhttp.main:main'
-        ]
-    },
-    install_requires=[
-        "setuptools",
-        f"wcferry=={wcfhttp.core.__version__}",
-        "fastapi",
-        "uvicorn[standard]"
-    ],
-    classifiers=[
-        "Environment :: Win32 (MS Windows)",
-        "Intended Audience :: Developers",
-        "Intended Audience :: Customer Service",
-        "Topic :: Communications :: Chat",
-        "Operating System :: Microsoft :: Windows",
-        "Programming Language :: Python",
-    ],
-    project_urls={
-        "Documentation": "https://wechatferry.readthedocs.io/zh/latest/index.html",
-        "GitHub": "https://github.com/lich0821/WeChatFerry/",
-    },
-)
+#! /usr/bin/env python3
+# -*- coding: utf-8 -*-
+
+
+from __future__ import print_function
+from setuptools import setup, find_packages
+
+import wcfhttp
+
+with open("README.md", "r", encoding="utf-8") as fh:
+    long_description = fh.read()
+
+
+setup(
+    name="wcfhttp",
+    version=wcfhttp.core.__version__,
+    author="Changhua",
+    author_email="lichanghua0821@gmail.com",
+    description="一个玩微信的工具",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    license="MIT",
+    url="https://github.com/lich0821/WeChatFerry",
+    python_requires=">=3.8",
+    packages=find_packages(),
+    include_package_data=True,
+    entry_points={
+        'console_scripts': [
+            'wcfhttp=wcfhttp.main:main'
+        ]
+    },
+    install_requires=[
+        "setuptools",
+        f"wcferry=={wcfhttp.core.__version__}",
+        "fastapi",
+        "uvicorn[standard]"
+    ],
+    classifiers=[
+        "Environment :: Win32 (MS Windows)",
+        "Intended Audience :: Developers",
+        "Intended Audience :: Customer Service",
+        "Topic :: Communications :: Chat",
+        "Operating System :: Microsoft :: Windows",
+        "Programming Language :: Python",
+    ],
+    project_urls={
+        "Documentation": "https://wechatferry.readthedocs.io/zh/latest/index.html",
+        "GitHub": "https://github.com/lich0821/WeChatFerry/",
+    },
+)
```

### Comparing `wcfhttp-3.7.0.30.25/wcfhttp/core.py` & `wcfhttp-37.1.25.0/wcfhttp/core.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,225 +1,225 @@
-#! /usr/bin/env python3
-# -*- coding: utf-8 -*-
-
-import base64
-import logging
-from typing import Any
-
-import requests
-from fastapi import Body, FastAPI
-from pydantic import BaseModel
-from wcferry import Wcf, WxMsg
-
-__version__ = "3.7.0.30.25"
-
-
-class Msg(BaseModel):
-    id: str
-    type: int
-    xml: str
-    sender: str
-    roomid: str
-    content: str
-    thumb: str
-    extra: str
-    is_self: bool
-    is_group: bool
-
-
-class Http(FastAPI):
-    """WeChatFerry HTTP 客户端，文档地址：http://IP:PORT/docs"""
-
-    def __init__(self, wcf: Wcf, cb: str, **extra: Any) -> None:
-        super().__init__(**extra)
-        self.LOG = logging.getLogger(__name__)
-        self.wcf = wcf
-        self._set_cb(cb)
-
-        self.add_api_route("/login", self.is_login, methods=["GET"], summary="获取登录状态")
-        self.add_api_route("/wxid", self.get_self_wxid, methods=["GET"], summary="获取登录账号 wxid")
-        self.add_api_route("/user-info", self.get_user_info, methods=["GET"], summary="获取登录账号个人信息")
-        self.add_api_route("/msg-types", self.get_msg_types, methods=["GET"], summary="获取消息类型")
-        self.add_api_route("/contacts", self.get_contacts, methods=["GET"], summary="获取完整通讯录")
-        self.add_api_route("/friends", self.get_friends, methods=["GET"], summary="获取好友列表")
-        self.add_api_route("/dbs", self.get_dbs, methods=["GET"], summary="获取所有数据库")
-        self.add_api_route("/{db}/tables", self.get_tables, methods=["GET"], summary="获取 db 中所有表")
-
-        self.add_api_route("/msg_cb", self.msg_cb, methods=["POST"], summary="接收消息回调样例")
-        self.add_api_route("/text", self.send_text, methods=["POST"], summary="发送文本消息")
-        self.add_api_route("/image", self.send_image, methods=["POST"], summary="发送图片消息")
-        self.add_api_route("/file", self.send_file, methods=["POST"], summary="发送文件消息")
-        self.add_api_route("/xml", self.send_xml, methods=["POST"], summary="发送 XML 消息")
-        self.add_api_route("/emotion", self.send_emotion, methods=["POST"], summary="发送表情消息")
-        self.add_api_route("/sql", self.query_sql, methods=["POST"], summary="执行 SQL，如果数据量大注意分页，以免 OOM")
-        self.add_api_route("/new-friend", self.accept_new_friend, methods=["POST"], summary="通过好友申请")
-        self.add_api_route("/chatroom-member", self.add_chatroom_members, methods=["POST"], summary="添加群成员")
-        self.add_api_route("/transfer", self.receive_transfer, methods=["POST"], summary="接收转账")
-        self.add_api_route("/dec-image", self.decrypt_image, methods=["POST"], summary="解密图片")
-
-    def _set_cb(self, cb):
-        def callback(msg: WxMsg):
-            data = {}
-            data["id"] = msg.id
-            data["type"] = msg.type
-            data["xml"] = msg.xml
-            data["sender"] = msg.sender
-            data["roomid"] = msg.roomid
-            data["content"] = msg.content
-            data["thumb"] = msg.thumb
-            data["extra"] = msg.extra
-            data["is_self"] = msg.from_self()
-            data["is_group"] = msg.from_group()
-
-            try:
-                rsp = requests.post(url=cb, json=data)
-                if rsp.status_code != 200:
-                    self.LOG.error(f"消息转发失败，HTTP 状态码为: {rsp.status_code}")
-            except Exception as e:
-                self.LOG.error(f"消息转发异常: {e}")
-
-        if cb:
-            self.LOG.info(f"消息回调: {cb}")
-            self.wcf.enable_recv_msg(callback=callback)
-        else:
-            self.LOG.info(f"没有设置回调，打印消息")
-            self.wcf.enable_recv_msg(print)
-
-    def is_login(self) -> dict:
-        """获取登录状态"""
-        ret = self.wcf.is_login()
-        return {"status": 0, "message": "成功", "data": {"login": ret}}
-
-    def get_self_wxid(self) -> dict:
-        """获取登录账号 wxid"""
-        ret = self.wcf.get_self_wxid()
-        if ret:
-            return {"status": 0, "message": "成功", "data": {"wxid": ret}}
-        return {"status": -1, "message": "失败"}
-
-    def get_msg_types(self) -> dict:
-        """获取消息类型"""
-        ret = self.wcf.get_msg_types()
-        if ret:
-            return {"status": 0, "message": "成功", "data": {"types": ret}}
-        return {"status": -1, "message": "失败"}
-
-    def get_contacts(self) -> dict:
-        """获取完整通讯录"""
-        ret = self.wcf.get_contacts()
-        if ret:
-            return {"status": 0, "message": "成功", "data": {"contacts": ret}}
-        return {"status": -1, "message": "失败"}
-
-    def get_friends(self) -> dict:
-        """获取好友列表"""
-        ret = self.wcf.get_friends()
-        if ret:
-            return {"status": 0, "message": "成功", "data": {"friends": ret}}
-        return {"status": -1, "message": "失败"}
-
-    def get_dbs(self) -> dict:
-        """获取所有数据库"""
-        ret = self.wcf.get_dbs()
-        if ret:
-            return {"status": 0, "message": "成功", "data": {"dbs": ret}}
-        return {"status": -1, "message": "失败"}
-
-    def get_tables(self, db: str) -> dict:
-        """获取 db 中所有表"""
-        ret = self.wcf.get_tables(db)
-        if ret:
-            return {"status": 0, "message": "成功", "data": {"tables": ret}}
-        return {"status": -1, "message": "失败"}
-
-    def get_user_info(self) -> dict:
-        """获取登录账号个人信息"""
-        ret = self.wcf.get_user_info()
-        if ret:
-            return {"status": 0, "message": "成功", "data": {"ui": ret}}
-        return {"status": -1, "message": "失败"}
-
-    def msg_cb(self, msg: Msg):
-        """示例回调方法，简单打印消息"""
-        print(f"收到消息：{msg}")
-        return {"status": 0, "message": "成功"}
-
-    def send_text(self, msg: str = Body("消息"), receiver: str = Body("filehelper"), aters: str = Body("")) -> dict:
-        """发送文本消息，可参考：robot.py 里 sendTextMsg"""
-        ret = self.wcf.send_text(msg, receiver, aters)
-        return {"status": ret, "message": "成功"if ret == 0 else "失败"}
-
-    def send_image(self,
-                   path: str = Body("C:\\Projs\\WeChatRobot\\TEQuant.jpeg", description="图片路径"),
-                   receiver: str = Body("filehelper", description="roomid 或者 wxid")) -> dict:
-        """发送图片消息"""
-        ret = self.wcf.send_image(path, receiver)
-        return {"status": ret, "message": "成功"if ret == 0 else "失败"}
-
-    def send_file(self,
-                  path: str = Body("C:\\Projs\\WeChatRobot\\TEQuant.jpeg", description="本地文件路径，不支持网络路径"),
-                  receiver: str = Body("filehelper", description="roomid 或者 wxid")) -> dict:
-        """发送文件消息"""
-        ret = self.wcf.send_file(path, receiver)
-        return {"status": ret, "message": "成功"if ret == 0 else "失败"}
-
-    def send_xml(
-            self, receiver: str = Body("filehelper", description="roomid 或者 wxid"),
-            xml:
-            str = Body(
-                '<?xml version="1.0"?><msg><appmsg appid="" sdkver="0"><title>叮当药房，24小时服务，28分钟送药到家！</title><des>叮当快药首家承诺范围内28分钟送药到家！叮当快药核心区域内7*24小时全天候服务，送药上门！叮当快药官网为您提供快捷便利，正品低价，安全放心的购药、送药服务体验。</des><action>view</action><type>33</type></appmsg><fromusername>wxid_xxxxxxxxxxxxxx</fromusername><scene>0</scene><appinfo><version>1</version><appname /></appinfo><commenturl /></msg>',
-                description="xml 内容"),
-            type: int = Body(0x21, description="xml 类型，0x21 为小程序"),
-            path: str = Body(None, description="封面图片路径")) -> dict:
-        """发送 XML 消息"""
-        ret = self.wcf.send_xml(receiver, xml, type, path)
-        return {"status": ret, "message": "成功"if ret == 0 else "失败"}
-
-    def send_emotion(self,
-                     path: str = Body("C:/Projs/WeChatRobot/emo.gif", description="本地文件路径，不支持网络路径"),
-                     receiver: str = Body("filehelper", description="roomid 或者 wxid")) -> dict:
-        """发送表情消息"""
-        ret = self.wcf.send_emotion(path, receiver)
-        return {"status": ret, "message": "成功"if ret == 0 else "失败"}
-
-    def query_sql(self,
-                  db: str = Body("MicroMsg.db", description="数据库"),
-                  sql: str = Body("SELECT * FROM Contact LIMIT 1;", description="SQL 语句")) -> dict:
-        """执行 SQL，如果数据量大注意分页，以免 OOM"""
-        ret = self.wcf.query_sql(db, sql)
-        if ret:
-            for row in ret:
-                for k, v in row.items():
-                    print(k, type(v))
-                    if type(v) is bytes:
-                        row[k] = base64.b64encode(v)
-            return {"status": 0, "message": "成功", "data": {"bs64": ret}}
-        return {"status": -1, "message": "失败"}
-
-    def accept_new_friend(self,
-                          v3: str = Body("v3", description="加密用户名 (好友申请消息里 v3 开头的字符串)"),
-                          v4: str = Body("v4", description="Ticket (好友申请消息里 v4 开头的字符串)"),
-                          scene: int = Body(30, description="申请方式 (好友申请消息里的 scene)")) -> dict:
-        """通过好友申请"""
-        ret = self.wcf.accept_new_friend(v3, v4, scene)
-        return {"status": ret, "message": "成功"if ret == 1 else "失败"}
-
-    def add_chatroom_members(self,
-                             roomid: str = Body("xxxxxxxx@chatroom", description="待加群的 id"),
-                             wxids: str = Body("wxid_xxxxxxxxxxxxx", description="要加到群里的 wxid，多个用逗号分隔")) -> dict:
-        """添加群成员"""
-        ret = self.wcf.add_chatroom_members(roomid, wxids)
-        return {"status": ret, "message": "成功"if ret == 1 else "失败"}
-
-    def receive_transfer(self,
-                         wxid: str = Body("wxid_xxxxxxxxxxxxx", description="转账消息里的发送人 wxid"),
-                         transferid: str = Body("transferid", description="转账消息里的 transferid")) -> dict:
-        """接收转账"""
-        ret = self.wcf.receive_transfer(wxid, transferid)
-        return {"status": ret, "message": "成功"if ret == 1 else "失败"}
-
-    def decrypt_image(self,
-                      src: str = Body("C:\\...", description="加密的图片路径，从图片消息中获取"),
-                      dst: str = Body("C:\\...", description="解密的图片路径")) -> dict:
-        """接收转账"""
-        ret = self.wcf.decrypt_image(src, dst)
-        return {"status": ret, "message": "成功"if ret else "失败"}
+#! /usr/bin/env python3
+# -*- coding: utf-8 -*-
+
+import base64
+import logging
+from typing import Any
+
+import requests
+from fastapi import Body, FastAPI
+from pydantic import BaseModel
+from wcferry import Wcf, WxMsg
+
+__version__ = "37.1.25.0"
+
+
+class Msg(BaseModel):
+    id: str
+    type: int
+    xml: str
+    sender: str
+    roomid: str
+    content: str
+    thumb: str
+    extra: str
+    is_self: bool
+    is_group: bool
+
+
+class Http(FastAPI):
+    """WeChatFerry HTTP 客户端，文档地址：http://IP:PORT/docs"""
+
+    def __init__(self, wcf: Wcf, cb: str, **extra: Any) -> None:
+        super().__init__(**extra)
+        self.LOG = logging.getLogger(__name__)
+        self.wcf = wcf
+        self._set_cb(cb)
+
+        self.add_api_route("/login", self.is_login, methods=["GET"], summary="获取登录状态")
+        self.add_api_route("/wxid", self.get_self_wxid, methods=["GET"], summary="获取登录账号 wxid")
+        self.add_api_route("/user-info", self.get_user_info, methods=["GET"], summary="获取登录账号个人信息")
+        self.add_api_route("/msg-types", self.get_msg_types, methods=["GET"], summary="获取消息类型")
+        self.add_api_route("/contacts", self.get_contacts, methods=["GET"], summary="获取完整通讯录")
+        self.add_api_route("/friends", self.get_friends, methods=["GET"], summary="获取好友列表")
+        self.add_api_route("/dbs", self.get_dbs, methods=["GET"], summary="获取所有数据库")
+        self.add_api_route("/{db}/tables", self.get_tables, methods=["GET"], summary="获取 db 中所有表")
+
+        self.add_api_route("/msg_cb", self.msg_cb, methods=["POST"], summary="接收消息回调样例")
+        self.add_api_route("/text", self.send_text, methods=["POST"], summary="发送文本消息")
+        self.add_api_route("/image", self.send_image, methods=["POST"], summary="发送图片消息")
+        self.add_api_route("/file", self.send_file, methods=["POST"], summary="发送文件消息")
+        self.add_api_route("/xml", self.send_xml, methods=["POST"], summary="发送 XML 消息")
+        self.add_api_route("/emotion", self.send_emotion, methods=["POST"], summary="发送表情消息")
+        self.add_api_route("/sql", self.query_sql, methods=["POST"], summary="执行 SQL，如果数据量大注意分页，以免 OOM")
+        self.add_api_route("/new-friend", self.accept_new_friend, methods=["POST"], summary="通过好友申请")
+        self.add_api_route("/chatroom-member", self.add_chatroom_members, methods=["POST"], summary="添加群成员")
+        self.add_api_route("/transfer", self.receive_transfer, methods=["POST"], summary="接收转账")
+        self.add_api_route("/dec-image", self.decrypt_image, methods=["POST"], summary="解密图片")
+
+    def _set_cb(self, cb):
+        def callback(msg: WxMsg):
+            data = {}
+            data["id"] = msg.id
+            data["type"] = msg.type
+            data["xml"] = msg.xml
+            data["sender"] = msg.sender
+            data["roomid"] = msg.roomid
+            data["content"] = msg.content
+            data["thumb"] = msg.thumb
+            data["extra"] = msg.extra
+            data["is_self"] = msg.from_self()
+            data["is_group"] = msg.from_group()
+
+            try:
+                rsp = requests.post(url=cb, json=data)
+                if rsp.status_code != 200:
+                    self.LOG.error(f"消息转发失败，HTTP 状态码为: {rsp.status_code}")
+            except Exception as e:
+                self.LOG.error(f"消息转发异常: {e}")
+
+        if cb:
+            self.LOG.info(f"消息回调: {cb}")
+            self.wcf.enable_recv_msg(callback=callback)
+        else:
+            self.LOG.info(f"没有设置回调，打印消息")
+            self.wcf.enable_recv_msg(print)
+
+    def is_login(self) -> dict:
+        """获取登录状态"""
+        ret = self.wcf.is_login()
+        return {"status": 0, "message": "成功", "data": {"login": ret}}
+
+    def get_self_wxid(self) -> dict:
+        """获取登录账号 wxid"""
+        ret = self.wcf.get_self_wxid()
+        if ret:
+            return {"status": 0, "message": "成功", "data": {"wxid": ret}}
+        return {"status": -1, "message": "失败"}
+
+    def get_msg_types(self) -> dict:
+        """获取消息类型"""
+        ret = self.wcf.get_msg_types()
+        if ret:
+            return {"status": 0, "message": "成功", "data": {"types": ret}}
+        return {"status": -1, "message": "失败"}
+
+    def get_contacts(self) -> dict:
+        """获取完整通讯录"""
+        ret = self.wcf.get_contacts()
+        if ret:
+            return {"status": 0, "message": "成功", "data": {"contacts": ret}}
+        return {"status": -1, "message": "失败"}
+
+    def get_friends(self) -> dict:
+        """获取好友列表"""
+        ret = self.wcf.get_friends()
+        if ret:
+            return {"status": 0, "message": "成功", "data": {"friends": ret}}
+        return {"status": -1, "message": "失败"}
+
+    def get_dbs(self) -> dict:
+        """获取所有数据库"""
+        ret = self.wcf.get_dbs()
+        if ret:
+            return {"status": 0, "message": "成功", "data": {"dbs": ret}}
+        return {"status": -1, "message": "失败"}
+
+    def get_tables(self, db: str) -> dict:
+        """获取 db 中所有表"""
+        ret = self.wcf.get_tables(db)
+        if ret:
+            return {"status": 0, "message": "成功", "data": {"tables": ret}}
+        return {"status": -1, "message": "失败"}
+
+    def get_user_info(self) -> dict:
+        """获取登录账号个人信息"""
+        ret = self.wcf.get_user_info()
+        if ret:
+            return {"status": 0, "message": "成功", "data": {"ui": ret}}
+        return {"status": -1, "message": "失败"}
+
+    def msg_cb(self, msg: Msg):
+        """示例回调方法，简单打印消息"""
+        print(f"收到消息：{msg}")
+        return {"status": 0, "message": "成功"}
+
+    def send_text(self, msg: str = Body("消息"), receiver: str = Body("filehelper"), aters: str = Body("")) -> dict:
+        """发送文本消息，可参考：robot.py 里 sendTextMsg"""
+        ret = self.wcf.send_text(msg, receiver, aters)
+        return {"status": ret, "message": "成功"if ret == 0 else "失败"}
+
+    def send_image(self,
+                   path: str = Body("C:\\Projs\\WeChatRobot\\TEQuant.jpeg", description="图片路径"),
+                   receiver: str = Body("filehelper", description="roomid 或者 wxid")) -> dict:
+        """发送图片消息"""
+        ret = self.wcf.send_image(path, receiver)
+        return {"status": ret, "message": "成功"if ret == 0 else "失败"}
+
+    def send_file(self,
+                  path: str = Body("C:\\Projs\\WeChatRobot\\TEQuant.jpeg", description="本地文件路径，不支持网络路径"),
+                  receiver: str = Body("filehelper", description="roomid 或者 wxid")) -> dict:
+        """发送文件消息"""
+        ret = self.wcf.send_file(path, receiver)
+        return {"status": ret, "message": "成功"if ret == 0 else "失败"}
+
+    def send_xml(
+            self, receiver: str = Body("filehelper", description="roomid 或者 wxid"),
+            xml:
+            str = Body(
+                '<?xml version="1.0"?><msg><appmsg appid="" sdkver="0"><title>叮当药房，24小时服务，28分钟送药到家！</title><des>叮当快药首家承诺范围内28分钟送药到家！叮当快药核心区域内7*24小时全天候服务，送药上门！叮当快药官网为您提供快捷便利，正品低价，安全放心的购药、送药服务体验。</des><action>view</action><type>33</type></appmsg><fromusername>wxid_xxxxxxxxxxxxxx</fromusername><scene>0</scene><appinfo><version>1</version><appname /></appinfo><commenturl /></msg>',
+                description="xml 内容"),
+            type: int = Body(0x21, description="xml 类型，0x21 为小程序"),
+            path: str = Body(None, description="封面图片路径")) -> dict:
+        """发送 XML 消息"""
+        ret = self.wcf.send_xml(receiver, xml, type, path)
+        return {"status": ret, "message": "成功"if ret == 0 else "失败"}
+
+    def send_emotion(self,
+                     path: str = Body("C:/Projs/WeChatRobot/emo.gif", description="本地文件路径，不支持网络路径"),
+                     receiver: str = Body("filehelper", description="roomid 或者 wxid")) -> dict:
+        """发送表情消息"""
+        ret = self.wcf.send_emotion(path, receiver)
+        return {"status": ret, "message": "成功"if ret == 0 else "失败"}
+
+    def query_sql(self,
+                  db: str = Body("MicroMsg.db", description="数据库"),
+                  sql: str = Body("SELECT * FROM Contact LIMIT 1;", description="SQL 语句")) -> dict:
+        """执行 SQL，如果数据量大注意分页，以免 OOM"""
+        ret = self.wcf.query_sql(db, sql)
+        if ret:
+            for row in ret:
+                for k, v in row.items():
+                    print(k, type(v))
+                    if type(v) is bytes:
+                        row[k] = base64.b64encode(v)
+            return {"status": 0, "message": "成功", "data": {"bs64": ret}}
+        return {"status": -1, "message": "失败"}
+
+    def accept_new_friend(self,
+                          v3: str = Body("v3", description="加密用户名 (好友申请消息里 v3 开头的字符串)"),
+                          v4: str = Body("v4", description="Ticket (好友申请消息里 v4 开头的字符串)"),
+                          scene: int = Body(30, description="申请方式 (好友申请消息里的 scene)")) -> dict:
+        """通过好友申请"""
+        ret = self.wcf.accept_new_friend(v3, v4, scene)
+        return {"status": ret, "message": "成功"if ret == 1 else "失败"}
+
+    def add_chatroom_members(self,
+                             roomid: str = Body("xxxxxxxx@chatroom", description="待加群的 id"),
+                             wxids: str = Body("wxid_xxxxxxxxxxxxx", description="要加到群里的 wxid，多个用逗号分隔")) -> dict:
+        """添加群成员"""
+        ret = self.wcf.add_chatroom_members(roomid, wxids)
+        return {"status": ret, "message": "成功"if ret == 1 else "失败"}
+
+    def receive_transfer(self,
+                         wxid: str = Body("wxid_xxxxxxxxxxxxx", description="转账消息里的发送人 wxid"),
+                         transferid: str = Body("transferid", description="转账消息里的 transferid")) -> dict:
+        """接收转账"""
+        ret = self.wcf.receive_transfer(wxid, transferid)
+        return {"status": ret, "message": "成功"if ret == 1 else "失败"}
+
+    def decrypt_image(self,
+                      src: str = Body("C:\\...", description="加密的图片路径，从图片消息中获取"),
+                      dst: str = Body("C:\\...", description="解密的图片路径")) -> dict:
+        """接收转账"""
+        ret = self.wcf.decrypt_image(src, dst)
+        return {"status": ret, "message": "成功"if ret else "失败"}
```

### Comparing `wcfhttp-3.7.0.30.25/wcfhttp/main.py` & `wcfhttp-37.1.25.0/wcfhttp/main.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-#! /usr/bin/env python3
-# -*- coding: utf-8 -*-
-
-import logging
-import argparse
-
-import uvicorn
-from wcferry import Wcf
-from wcfhttp import Http, __version__
-
-
-def main():
-    parse = argparse.ArgumentParser()
-    parse.add_argument("-v", "--version", action="version", version=f"{__version__}")
-    parse.add_argument("--wcf_host", type=str, default=None, help="WeChatFerry 监听地址，默认本地启动监听 0.0.0.0")
-    parse.add_argument("--wcf_port", type=int, default=10086, help="WeChatFerry 监听端口 (同时占用 port + 1 端口)，默认 10086")
-    parse.add_argument("--wcf_debug", type=bool, default=False, help="是否打开 WeChatFerry 调试开关")
-    parse.add_argument("--host", type=str, default="0.0.0.0", help="wcfhttp 监听地址，默认监听 0.0.0.0")
-    parse.add_argument("--port", type=int, default=9999, help="wcfhttp 监听端口，默认 9999")
-    parse.add_argument("--cb", type=str, default="", help="接收消息回调地址")
-
-    logging.basicConfig(level="INFO", format="%(asctime)s %(message)s")
-    args = parse.parse_args()
-    cb = args.cb
-    if not cb:
-        logging.warning("没有设置接收消息回调，消息直接通过日志打印；请通过 --cb 设置消息回调")
-        logging.warning(f"回调接口规范参考接收消息回调样例：http://{args.host}:{args.port}/docs")
-
-    wcf = Wcf(args.wcf_host, args.wcf_port, args.wcf_debug)
-    home = "https://github.com/lich0821/WeChatFerry"
-    http = Http(wcf=wcf,
-                cb=cb,
-                title="WeChatFerry HTTP 客户端",
-                description=f"Github: <a href='{home}'>WeChatFerry</a>",)
-
-    uvicorn.run(app=http, host=args.host, port=args.port)
-
-
-if __name__ == "__main__":
-    main()
+#! /usr/bin/env python3
+# -*- coding: utf-8 -*-
+
+import logging
+import argparse
+
+import uvicorn
+from wcferry import Wcf
+from wcfhttp import Http, __version__
+
+
+def main():
+    parse = argparse.ArgumentParser()
+    parse.add_argument("-v", "--version", action="version", version=f"{__version__}")
+    parse.add_argument("--wcf_host", type=str, default=None, help="WeChatFerry 监听地址，默认本地启动监听 0.0.0.0")
+    parse.add_argument("--wcf_port", type=int, default=10086, help="WeChatFerry 监听端口 (同时占用 port + 1 端口)，默认 10086")
+    parse.add_argument("--wcf_debug", type=bool, default=False, help="是否打开 WeChatFerry 调试开关")
+    parse.add_argument("--host", type=str, default="0.0.0.0", help="wcfhttp 监听地址，默认监听 0.0.0.0")
+    parse.add_argument("--port", type=int, default=9999, help="wcfhttp 监听端口，默认 9999")
+    parse.add_argument("--cb", type=str, default="", help="接收消息回调地址")
+
+    logging.basicConfig(level="INFO", format="%(asctime)s %(message)s")
+    args = parse.parse_args()
+    cb = args.cb
+    if not cb:
+        logging.warning("没有设置接收消息回调，消息直接通过日志打印；请通过 --cb 设置消息回调")
+        logging.warning(f"回调接口规范参考接收消息回调样例：http://{args.host}:{args.port}/docs")
+
+    wcf = Wcf(args.wcf_host, args.wcf_port, args.wcf_debug)
+    home = "https://github.com/lich0821/WeChatFerry"
+    http = Http(wcf=wcf,
+                cb=cb,
+                title="WeChatFerry HTTP 客户端",
+                description=f"Github: <a href='{home}'>WeChatFerry</a>",)
+
+    uvicorn.run(app=http, host=args.host, port=args.port)
+
+
+if __name__ == "__main__":
+    main()
```

