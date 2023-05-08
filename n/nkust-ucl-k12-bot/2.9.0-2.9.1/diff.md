# Comparing `tmp/nkust-ucl-k12-bot-2.9.0.tar.gz` & `tmp/nkust-ucl-k12-bot-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nkust-ucl-k12-bot-2.9.0.tar", last modified: Mon May  8 04:25:50 2023, max compression
+gzip compressed data, was "nkust-ucl-k12-bot-2.9.1.tar", last modified: Mon May  8 04:28:38 2023, max compression
```

## Comparing `nkust-ucl-k12-bot-2.9.0.tar` & `nkust-ucl-k12-bot-2.9.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 zhengshiwen   (501) staff       (20)        0 2023-05-08 04:25:50.207228 nkust-ucl-k12-bot-2.9.0/
--rw-r--r--   0 zhengshiwen   (501) staff       (20)     1077 2023-05-06 09:22:13.000000 nkust-ucl-k12-bot-2.9.0/LICENSE
--rw-r--r--   0 zhengshiwen   (501) staff       (20)     5855 2023-05-08 04:25:50.206858 nkust-ucl-k12-bot-2.9.0/PKG-INFO
--rw-r--r--   0 zhengshiwen   (501) staff       (20)     5442 2023-05-08 04:25:13.000000 nkust-ucl-k12-bot-2.9.0/README.md
-drwxr-xr-x   0 zhengshiwen   (501) staff       (20)        0 2023-05-08 04:25:50.202490 nkust-ucl-k12-bot-2.9.0/nkust_ucl/
--rw-r--r--   0 zhengshiwen   (501) staff       (20)       26 2023-05-06 09:17:34.000000 nkust-ucl-k12-bot-2.9.0/nkust_ucl/__init__.py
--rw-r--r--   0 zhengshiwen   (501) staff       (20)    10758 2023-05-08 04:23:27.000000 nkust-ucl-k12-bot-2.9.0/nkust_ucl/k12.py
-drwxr-xr-x   0 zhengshiwen   (501) staff       (20)        0 2023-05-08 04:25:50.205033 nkust-ucl-k12-bot-2.9.0/nkust_ucl/utils/
--rw-r--r--   0 zhengshiwen   (501) staff       (20)        1 2023-05-06 06:57:47.000000 nkust-ucl-k12-bot-2.9.0/nkust_ucl/utils/__init__.py
--rw-r--r--   0 zhengshiwen   (501) staff       (20)     1021 2023-05-06 17:09:58.000000 nkust-ucl-k12-bot-2.9.0/nkust_ucl/utils/attachment.py
--rw-r--r--   0 zhengshiwen   (501) staff       (20)      340 2023-05-06 06:55:39.000000 nkust-ucl-k12-bot-2.9.0/nkust_ucl/utils/config.py
--rw-r--r--   0 zhengshiwen   (501) staff       (20)      426 2023-05-06 07:51:50.000000 nkust-ucl-k12-bot-2.9.0/nkust_ucl/utils/log.py
--rw-r--r--   0 zhengshiwen   (501) staff       (20)      938 2023-05-06 07:31:05.000000 nkust-ucl-k12-bot-2.9.0/nkust_ucl/utils/mqtt_client.py
-drwxr-xr-x   0 zhengshiwen   (501) staff       (20)        0 2023-05-08 04:25:50.206586 nkust-ucl-k12-bot-2.9.0/nkust_ucl_k12_bot.egg-info/
--rw-r--r--   0 zhengshiwen   (501) staff       (20)     5855 2023-05-08 04:25:50.000000 nkust-ucl-k12-bot-2.9.0/nkust_ucl_k12_bot.egg-info/PKG-INFO
--rw-r--r--   0 zhengshiwen   (501) staff       (20)      407 2023-05-08 04:25:50.000000 nkust-ucl-k12-bot-2.9.0/nkust_ucl_k12_bot.egg-info/SOURCES.txt
--rw-r--r--   0 zhengshiwen   (501) staff       (20)        1 2023-05-08 04:25:50.000000 nkust-ucl-k12-bot-2.9.0/nkust_ucl_k12_bot.egg-info/dependency_links.txt
--rw-r--r--   0 zhengshiwen   (501) staff       (20)      744 2023-05-08 04:25:50.000000 nkust-ucl-k12-bot-2.9.0/nkust_ucl_k12_bot.egg-info/requires.txt
--rw-r--r--   0 zhengshiwen   (501) staff       (20)       10 2023-05-08 04:25:50.000000 nkust-ucl-k12-bot-2.9.0/nkust_ucl_k12_bot.egg-info/top_level.txt
--rw-r--r--   0 zhengshiwen   (501) staff       (20)       38 2023-05-08 04:25:50.207320 nkust-ucl-k12-bot-2.9.0/setup.cfg
--rw-r--r--   0 zhengshiwen   (501) staff       (20)     1880 2023-05-08 04:23:48.000000 nkust-ucl-k12-bot-2.9.0/setup.py
+drwxr-xr-x   0 zhengshiwen   (501) staff       (20)        0 2023-05-08 04:28:38.404140 nkust-ucl-k12-bot-2.9.1/
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)     1077 2023-05-06 09:22:13.000000 nkust-ucl-k12-bot-2.9.1/LICENSE
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)     6029 2023-05-08 04:28:38.403880 nkust-ucl-k12-bot-2.9.1/PKG-INFO
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)     5616 2023-05-08 04:28:10.000000 nkust-ucl-k12-bot-2.9.1/README.md
+drwxr-xr-x   0 zhengshiwen   (501) staff       (20)        0 2023-05-08 04:28:38.400763 nkust-ucl-k12-bot-2.9.1/nkust_ucl/
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)       26 2023-05-06 09:17:34.000000 nkust-ucl-k12-bot-2.9.1/nkust_ucl/__init__.py
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)    10758 2023-05-08 04:23:27.000000 nkust-ucl-k12-bot-2.9.1/nkust_ucl/k12.py
+drwxr-xr-x   0 zhengshiwen   (501) staff       (20)        0 2023-05-08 04:28:38.402503 nkust-ucl-k12-bot-2.9.1/nkust_ucl/utils/
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)        1 2023-05-06 06:57:47.000000 nkust-ucl-k12-bot-2.9.1/nkust_ucl/utils/__init__.py
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)     1021 2023-05-06 17:09:58.000000 nkust-ucl-k12-bot-2.9.1/nkust_ucl/utils/attachment.py
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)      340 2023-05-06 06:55:39.000000 nkust-ucl-k12-bot-2.9.1/nkust_ucl/utils/config.py
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)      426 2023-05-06 07:51:50.000000 nkust-ucl-k12-bot-2.9.1/nkust_ucl/utils/log.py
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)      938 2023-05-06 07:31:05.000000 nkust-ucl-k12-bot-2.9.1/nkust_ucl/utils/mqtt_client.py
+drwxr-xr-x   0 zhengshiwen   (501) staff       (20)        0 2023-05-08 04:28:38.403618 nkust-ucl-k12-bot-2.9.1/nkust_ucl_k12_bot.egg-info/
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)     6029 2023-05-08 04:28:38.000000 nkust-ucl-k12-bot-2.9.1/nkust_ucl_k12_bot.egg-info/PKG-INFO
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)      407 2023-05-08 04:28:38.000000 nkust-ucl-k12-bot-2.9.1/nkust_ucl_k12_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)        1 2023-05-08 04:28:38.000000 nkust-ucl-k12-bot-2.9.1/nkust_ucl_k12_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)      744 2023-05-08 04:28:38.000000 nkust-ucl-k12-bot-2.9.1/nkust_ucl_k12_bot.egg-info/requires.txt
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)       10 2023-05-08 04:28:38.000000 nkust-ucl-k12-bot-2.9.1/nkust_ucl_k12_bot.egg-info/top_level.txt
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)       38 2023-05-08 04:28:38.404207 nkust-ucl-k12-bot-2.9.1/setup.cfg
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)     1880 2023-05-08 04:28:29.000000 nkust-ucl-k12-bot-2.9.1/setup.py
```

### Comparing `nkust-ucl-k12-bot-2.9.0/LICENSE` & `nkust-ucl-k12-bot-2.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nkust-ucl-k12-bot-2.9.0/PKG-INFO` & `nkust-ucl-k12-bot-2.9.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nkust-ucl-k12-bot
-Version: 2.9.0
+Version: 2.9.1
 Summary: 一個用於k12的bot包
 Home-page: https://github.com/xinbow99/k12-telegram
 Author: Ethan Cheng
 Author-email: asdewq45445@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -77,30 +77,31 @@
 
 command_handler.register_command("/chatgpt", MsgType.TEXT, reply_chatgpt)
 
 # run要在最後面
 custom_k12.run()
 ```
 ## v2.9.0更新
-* 快速回復新增了以下方法
+* 快速回復新增了以下方法，支援本地檔案與網路檔案
 ```python
 reply_text(msg: str)
 reply_image(image_path: str)
-reply_file(file_path: str)
+reply_document(file_path: str)
 ```
 usage:
 ```python
 @K12.on_processed_message
 def my_custom_on_processed_message(self, chat_msg: ChatMessage):
     # ... 自定義的 on_processed 行為 ...
     if chat_msg.send_user_id == "1234567890987654321":
         return
     chat_msg.reply_text("test")
     chat_msg.reply_image("test.png")
-    chat_msg.reply_file("test.txt")
+    chat_msg.reply_image("https://upload.wikimedia.org/wikipedia/commons/thumb/0/04/ChatGPT_logo.svg/512px-ChatGPT_logo.svg.png")
+    chat_msg.reply_document("test.txt")
 ```
 
 ## v2.8.3更新
 我們在ChatMessage的類別中新增了reply方法，可以直接回覆訊息
 ```python
 reply(self, msg: str, msg_type: MsgType = MsgType.TEXT)
 ```
```

### Comparing `nkust-ucl-k12-bot-2.9.0/README.md` & `nkust-ucl-k12-bot-2.9.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -64,30 +64,31 @@
 
 command_handler.register_command("/chatgpt", MsgType.TEXT, reply_chatgpt)
 
 # run要在最後面
 custom_k12.run()
 ```
 ## v2.9.0更新
-* 快速回復新增了以下方法
+* 快速回復新增了以下方法，支援本地檔案與網路檔案
 ```python
 reply_text(msg: str)
 reply_image(image_path: str)
-reply_file(file_path: str)
+reply_document(file_path: str)
 ```
 usage:
 ```python
 @K12.on_processed_message
 def my_custom_on_processed_message(self, chat_msg: ChatMessage):
     # ... 自定義的 on_processed 行為 ...
     if chat_msg.send_user_id == "1234567890987654321":
         return
     chat_msg.reply_text("test")
     chat_msg.reply_image("test.png")
-    chat_msg.reply_file("test.txt")
+    chat_msg.reply_image("https://upload.wikimedia.org/wikipedia/commons/thumb/0/04/ChatGPT_logo.svg/512px-ChatGPT_logo.svg.png")
+    chat_msg.reply_document("test.txt")
 ```
 
 ## v2.8.3更新
 我們在ChatMessage的類別中新增了reply方法，可以直接回覆訊息
 ```python
 reply(self, msg: str, msg_type: MsgType = MsgType.TEXT)
 ```
```

### Comparing `nkust-ucl-k12-bot-2.9.0/nkust_ucl/k12.py` & `nkust-ucl-k12-bot-2.9.1/nkust_ucl/k12.py`

 * *Files identical despite different names*

### Comparing `nkust-ucl-k12-bot-2.9.0/nkust_ucl/utils/attachment.py` & `nkust-ucl-k12-bot-2.9.1/nkust_ucl/utils/attachment.py`

 * *Files identical despite different names*

### Comparing `nkust-ucl-k12-bot-2.9.0/nkust_ucl/utils/mqtt_client.py` & `nkust-ucl-k12-bot-2.9.1/nkust_ucl/utils/mqtt_client.py`

 * *Files identical despite different names*

### Comparing `nkust-ucl-k12-bot-2.9.0/nkust_ucl_k12_bot.egg-info/PKG-INFO` & `nkust-ucl-k12-bot-2.9.1/nkust_ucl_k12_bot.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nkust-ucl-k12-bot
-Version: 2.9.0
+Version: 2.9.1
 Summary: 一個用於k12的bot包
 Home-page: https://github.com/xinbow99/k12-telegram
 Author: Ethan Cheng
 Author-email: asdewq45445@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -77,30 +77,31 @@
 
 command_handler.register_command("/chatgpt", MsgType.TEXT, reply_chatgpt)
 
 # run要在最後面
 custom_k12.run()
 ```
 ## v2.9.0更新
-* 快速回復新增了以下方法
+* 快速回復新增了以下方法，支援本地檔案與網路檔案
 ```python
 reply_text(msg: str)
 reply_image(image_path: str)
-reply_file(file_path: str)
+reply_document(file_path: str)
 ```
 usage:
 ```python
 @K12.on_processed_message
 def my_custom_on_processed_message(self, chat_msg: ChatMessage):
     # ... 自定義的 on_processed 行為 ...
     if chat_msg.send_user_id == "1234567890987654321":
         return
     chat_msg.reply_text("test")
     chat_msg.reply_image("test.png")
-    chat_msg.reply_file("test.txt")
+    chat_msg.reply_image("https://upload.wikimedia.org/wikipedia/commons/thumb/0/04/ChatGPT_logo.svg/512px-ChatGPT_logo.svg.png")
+    chat_msg.reply_document("test.txt")
 ```
 
 ## v2.8.3更新
 我們在ChatMessage的類別中新增了reply方法，可以直接回覆訊息
 ```python
 reply(self, msg: str, msg_type: MsgType = MsgType.TEXT)
 ```
```

### Comparing `nkust-ucl-k12-bot-2.9.0/nkust_ucl_k12_bot.egg-info/requires.txt` & `nkust-ucl-k12-bot-2.9.1/nkust_ucl_k12_bot.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `nkust-ucl-k12-bot-2.9.0/setup.py` & `nkust-ucl-k12-bot-2.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name="nkust-ucl-k12-bot",
-    version="2.9.0",
+    version="2.9.1",
     author="Ethan Cheng",
     author_email="asdewq45445@gmail.com",
     description="一個用於k12的bot包",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/xinbow99/k12-telegram",
     packages=setuptools.find_packages(),
```

