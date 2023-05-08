# Comparing `tmp/yunhu-0.0.3.tar.gz` & `tmp/yunhu-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yunhu-0.0.3.tar", last modified: Mon May  8 11:17:22 2023, max compression
+gzip compressed data, was "yunhu-0.0.4.tar", last modified: Mon May  8 11:30:17 2023, max compression
```

## Comparing `yunhu-0.0.3.tar` & `yunhu-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 11:17:22.049909 yunhu-0.0.3/
--rw-rw-rw-   0        0        0     1094 2023-05-08 06:42:50.000000 yunhu-0.0.3/LICENSE.txt
--rw-rw-rw-   0        0        0      610 2023-05-08 11:17:22.047904 yunhu-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      159 2023-05-08 06:42:00.000000 yunhu-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-08 11:17:22.018753 yunhu-0.0.3/example_yunhu/
--rw-rw-rw-   0        0        0        0 2023-04-24 04:05:16.000000 yunhu-0.0.3/example_yunhu/__init__.py
--rw-rw-rw-   0        0        0     2424 2023-05-08 08:56:14.000000 yunhu-0.0.3/example_yunhu/flask_demo.py
--rw-rw-rw-   0        0        0      426 2023-05-08 11:16:53.000000 yunhu-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-08 11:17:22.050907 yunhu-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      725 2023-05-08 11:16:54.000000 yunhu-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-08 11:17:22.032269 yunhu-0.0.3/yunhu/
--rw-rw-rw-   0        0        0        0 2023-05-08 09:46:54.000000 yunhu-0.0.3/yunhu/__init__.py
--rw-rw-rw-   0        0        0       69 2023-05-08 01:21:22.000000 yunhu-0.0.3/yunhu/main.py
--rw-rw-rw-   0        0        0     2694 2023-04-25 08:55:43.000000 yunhu-0.0.3/yunhu/openapi.py
--rw-rw-rw-   0        0        0     2158 2023-04-25 07:39:22.000000 yunhu-0.0.3/yunhu/subscription.py
-drwxrwxrwx   0        0        0        0 2023-05-08 11:17:22.045892 yunhu-0.0.3/yunhu.egg-info/
--rw-rw-rw-   0        0        0      610 2023-05-08 11:17:21.000000 yunhu-0.0.3/yunhu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      286 2023-05-08 11:17:21.000000 yunhu-0.0.3/yunhu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 11:17:21.000000 yunhu-0.0.3/yunhu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-05-08 11:17:21.000000 yunhu-0.0.3/yunhu.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-08 11:30:17.162910 yunhu-0.0.4/
+-rw-rw-rw-   0        0        0     1094 2023-05-08 06:42:50.000000 yunhu-0.0.4/LICENSE.txt
+-rw-rw-rw-   0        0        0      610 2023-05-08 11:30:17.161938 yunhu-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      159 2023-05-08 06:42:00.000000 yunhu-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-08 11:30:17.138483 yunhu-0.0.4/example_yunhu/
+-rw-rw-rw-   0        0        0        0 2023-04-24 04:05:16.000000 yunhu-0.0.4/example_yunhu/__init__.py
+-rw-rw-rw-   0        0        0     2424 2023-05-08 08:56:14.000000 yunhu-0.0.4/example_yunhu/flask_demo.py
+-rw-rw-rw-   0        0        0      426 2023-05-08 11:28:28.000000 yunhu-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-08 11:30:17.164423 yunhu-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      725 2023-05-08 11:28:33.000000 yunhu-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 11:30:17.148935 yunhu-0.0.4/yunhu/
+-rw-rw-rw-   0        0        0        0 2023-05-08 09:46:54.000000 yunhu-0.0.4/yunhu/__init__.py
+-rw-rw-rw-   0        0        0       69 2023-05-08 01:21:22.000000 yunhu-0.0.4/yunhu/main.py
+-rw-rw-rw-   0        0        0     2694 2023-04-25 08:55:43.000000 yunhu-0.0.4/yunhu/openapi.py
+-rw-rw-rw-   0        0        0     2460 2023-05-08 11:27:24.000000 yunhu-0.0.4/yunhu/subscription.py
+drwxrwxrwx   0        0        0        0 2023-05-08 11:30:17.159909 yunhu-0.0.4/yunhu.egg-info/
+-rw-rw-rw-   0        0        0      610 2023-05-08 11:30:17.000000 yunhu-0.0.4/yunhu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      286 2023-05-08 11:30:17.000000 yunhu-0.0.4/yunhu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 11:30:17.000000 yunhu-0.0.4/yunhu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-05-08 11:30:17.000000 yunhu-0.0.4/yunhu.egg-info/top_level.txt
```

### Comparing `yunhu-0.0.3/LICENSE.txt` & `yunhu-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `yunhu-0.0.3/PKG-INFO` & `yunhu-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yunhu
-Version: 0.0.3
+Version: 0.0.4
 Summary: 云湖官方Python SDK
 Author: yunhu
 Author-email: yunhu <1114110051@qq.com>
 Project-URL: Homepage, https://github.com/yhchat/bot-python-sdk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `yunhu-0.0.3/example_yunhu/flask_demo.py` & `yunhu-0.0.4/example_yunhu/flask_demo.py`

 * *Files identical despite different names*

### Comparing `yunhu-0.0.3/setup.py` & `yunhu-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools 
  
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
  
 setuptools.setup(
     name="yunhu", 
-    version="0.0.3", 
+    version="0.0.4", 
     author="yunhu",  
     description="云湖官方Python SDK", #包的简述
     author_email="1114110051@qq.com",    
     long_description=long_description,    #包的详细介绍，一般在README.md文件内
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `yunhu-0.0.3/yunhu/openapi.py` & `yunhu-0.0.4/yunhu/openapi.py`

 * *Files identical despite different names*

### Comparing `yunhu-0.0.3/yunhu/subscription.py` & `yunhu-0.0.4/yunhu/subscription.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,27 +14,27 @@
         pass
 
     def listen(self, request):
 
         eventType = request.get_json()['header']['eventType']
         event = request.get_json()["event"]
 
-        if eventType == 'message.receive.normal': # 普通消息事件  
+        if eventType == 'message.receive.normal' and self.onMessageNormalSubscriber != None: # 普通消息事件  
             self.onMessageNormalSubscriber(event)
-        elif eventType == 'message.receive.instruction': # 指令消息事件 
+        elif eventType == 'message.receive.instruction' and self.onMessageInstructionSubscriber != None: # 指令消息事件 
             self.onMessageInstructionSubscriber(event)
-        elif eventType == 'group.join': # 加入群组事件 
+        elif eventType == 'group.join' and self.onGroupJoinSubscriber != None: # 加入群组事件 
             self.onGroupJoinSubscriber(event)
-        elif eventType == 'group.leave': # 退出群组事件 
+        elif eventType == 'group.leave' and self.onGroupLeaveSubscriber != None: # 退出群组事件 
             self.onGroupLeaveSubscriber(event)
-        elif eventType == 'bot.followed': # 关注机器人事件 
+        elif eventType == 'bot.followed' and self.onBotFollowedSubscriber != None: # 关注机器人事件 
             self.onBotFollowedSubscriber(event)
-        elif eventType == 'bot.unfollowed': # 取消关注机器人事件  
+        elif eventType == 'bot.unfollowed' and self.onBotUnfollowedSubscriber != None: # 取消关注机器人事件  
             self.onBotUnfollowedSubscriber(event)
-        elif eventType == 'button.report.inline': # 消息下按钮点击回调事件 
+        elif eventType == 'button.report.inline' and self.onButtonReportInlineSubscriber != None: # 消息下按钮点击回调事件 
             self.onButtonReportInlineSubscriber(event)
 
     def onMessageNormal(self, func):
         self.onMessageNormalSubscriber = func
         return func
 
     def onMessageInstruction(self, func):
```

### Comparing `yunhu-0.0.3/yunhu.egg-info/PKG-INFO` & `yunhu-0.0.4/yunhu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yunhu
-Version: 0.0.3
+Version: 0.0.4
 Summary: 云湖官方Python SDK
 Author: yunhu
 Author-email: yunhu <1114110051@qq.com>
 Project-URL: Homepage, https://github.com/yhchat/bot-python-sdk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

