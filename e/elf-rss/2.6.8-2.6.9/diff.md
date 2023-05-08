# Comparing `tmp/ELF_RSS-2.6.8.tar.gz` & `tmp/ELF_RSS-2.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ELF_RSS-2.6.8.tar", max compression
+gzip compressed data, was "ELF_RSS-2.6.9.tar", max compression
```

## Comparing `ELF_RSS-2.6.8.tar` & `ELF_RSS-2.6.9.tar`

### file list

```diff
@@ -1,43 +1,42 @@
--rw-r--r--   0        0        0    35149 2022-07-28 11:08:50.017213 ELF_RSS-2.6.8/LICENSE
--rw-r--r--   0        0        0     3314 2022-07-28 11:08:50.017213 ELF_RSS-2.6.8/README.md
--rw-r--r--   0        0        0     1141 2022-07-28 11:08:50.021213 ELF_RSS-2.6.8/pyproject.toml
--rw-r--r--   0        0        0     1811 2022-07-28 11:08:50.021213 ELF_RSS-2.6.8/src/plugins/ELF_RSS2/__init__.py
--rw-r--r--   0        0        0      140 2022-07-28 11:08:50.021213 ELF_RSS-2.6.8/src/plugins/ELF_RSS2/command/__init__.py
--rw-r--r--   0        0        0     1666 2022-07-28 11:08:50.021213 ELF_RSS-2.6.8/src/plugins/ELF_RSS2/command/add_cookies.py
--rw-r--r--   0        0        0     2231 2022-07-28 11:08:50.021213 ELF_RSS-2.6.8/src/plugins/ELF_RSS2/command/add_dy.py
--rw-r--r--   0        0        0    12035 2022-07-28 11:08:50.021213 ELF_RSS-2.6.8/src/plugins/ELF_RSS2/command/change_dy.py
--rw-r--r--   0        0        0     2533 2022-07-28 11:08:50.021213 ELF_RSS-2.6.8/src/plugins/ELF_RSS2/command/del_dy.py
--rw-r--r--   0        0        0     3781 2022-07-28 11:08:50.021213 ELF_RSS-2.6.8/src/plugins/ELF_RSS2/command/rsshub_add.py
--rw-r--r--   0        0        0     2885 2022-07-28 11:08:50.021213 ELF_RSS-2.6.8/src/plugins/ELF_RSS2/command/show_all.py
--rw-r--r--   0        0        0     2555 2022-07-28 11:08:50.021213 ELF_RSS-2.6.8/src/plugins/ELF_RSS2/command/show_dy.py
--rw-r--r--   0        0        0     1231 2022-07-28 11:08:50.021213 ELF_RSS-2.6.8/src/plugins/ELF_RSS2/command/upload_group_file.py
--rw-r--r--   0        0        0     1614 2022-07-28 11:08:50.021213 ELF_RSS-2.6.8/src/plugins/ELF_RSS2/config.py
--rw-r--r--   0        0        0     3600 2022-07-28 11:08:50.021213 ELF_RSS-2.6.8/src/plugins/ELF_RSS2/my_trigger.py
--rw-r--r--   0        0        0    11076 2022-07-28 11:08:50.021213 ELF_RSS-2.6.8/src/plugins/ELF_RSS2/parsing/__init__.py
--rw-r--r--   0        0        0     4896 2022-07-28 11:08:50.021213 ELF_RSS-2.6.8/src/plugins/ELF_RSS2/parsing/cache_manage.py
--rw-r--r--   0        0        0     1249 2022-07-28 11:08:50.021213 ELF_RSS-2.6.8/src/plugins/ELF_RSS2/parsing/check_update.py
--rw-r--r--   0        0        0     3448 2022-07-28 11:08:50.021213 ELF_RSS-2.6.8/src/plugins/ELF_RSS2/parsing/download_torrent.py
--rw-r--r--   0        0        0     4838 2022-07-28 11:08:50.021213 ELF_RSS-2.6.8/src/plugins/ELF_RSS2/parsing/handle_html_tag.py
--rw-r--r--   0        0        0    10191 2022-07-28 11:08:50.021213 ELF_RSS-2.6.8/src/plugins/ELF_RSS2/parsing/handle_images.py
--rw-r--r--   0        0        0     2015 2022-07-28 11:08:50.021213 ELF_RSS-2.6.8/src/plugins/ELF_RSS2/parsing/handle_translation.py
--rw-r--r--   0        0        0     6836 2022-07-28 11:08:50.021213 ELF_RSS-2.6.8/src/plugins/ELF_RSS2/parsing/parsing_rss.py
--rw-r--r--   0        0        0       82 2022-07-28 11:08:50.025214 ELF_RSS-2.6.8/src/plugins/ELF_RSS2/parsing/routes/__init__.py
--rw-r--r--   0        0        0     4307 2022-07-28 11:08:50.025214 ELF_RSS-2.6.8/src/plugins/ELF_RSS2/parsing/routes/danbooru.py
--rw-r--r--   0        0        0     1050 2022-07-28 11:08:50.025214 ELF_RSS-2.6.8/src/plugins/ELF_RSS2/parsing/routes/nga.py
--rw-r--r--   0        0        0     5899 2022-07-28 11:08:50.025214 ELF_RSS-2.6.8/src/plugins/ELF_RSS2/parsing/routes/pixiv.py
--rw-r--r--   0        0        0     1882 2022-07-28 11:08:50.025214 ELF_RSS-2.6.8/src/plugins/ELF_RSS2/parsing/routes/south_plus.py
--rw-r--r--   0        0        0     2104 2022-07-28 11:08:50.025214 ELF_RSS-2.6.8/src/plugins/ELF_RSS2/parsing/routes/twitter.py
--rw-r--r--   0        0        0     2521 2022-07-28 11:08:50.025214 ELF_RSS-2.6.8/src/plugins/ELF_RSS2/parsing/routes/weibo.py
--rw-r--r--   0        0        0      621 2022-07-28 11:08:50.025214 ELF_RSS-2.6.8/src/plugins/ELF_RSS2/parsing/routes/yande_re.py
--rw-r--r--   0        0        0      758 2022-07-28 11:08:50.025214 ELF_RSS-2.6.8/src/plugins/ELF_RSS2/parsing/routes/youtube.py
--rw-r--r--   0        0        0     4392 2022-07-28 11:08:50.025214 ELF_RSS-2.6.8/src/plugins/ELF_RSS2/parsing/send_message.py
--rw-r--r--   0        0        0      515 2022-07-28 11:08:50.025214 ELF_RSS-2.6.8/src/plugins/ELF_RSS2/parsing/utils.py
--rw-r--r--   0        0        0     2740 2022-07-28 11:08:50.025214 ELF_RSS-2.6.8/src/plugins/ELF_RSS2/patch.py
--rw-r--r--   0        0        0      719 2022-07-28 11:08:50.025214 ELF_RSS-2.6.8/src/plugins/ELF_RSS2/permission.py
--rw-r--r--   0        0        0     3385 2022-07-28 11:08:50.025214 ELF_RSS-2.6.8/src/plugins/ELF_RSS2/pikpak_offline.py
--rw-r--r--   0        0        0     8720 2022-07-28 11:08:50.025214 ELF_RSS-2.6.8/src/plugins/ELF_RSS2/qbittorrent_download.py
--rw-r--r--   0        0        0    10311 2022-07-28 11:08:50.025214 ELF_RSS-2.6.8/src/plugins/ELF_RSS2/rss_class.py
--rw-r--r--   0        0        0     6345 2022-07-28 11:08:50.025214 ELF_RSS-2.6.8/src/plugins/ELF_RSS2/rss_parsing.py
--rw-r--r--   0        0        0     5208 2022-07-28 11:08:50.025214 ELF_RSS-2.6.8/src/plugins/ELF_RSS2/utils.py
--rw-r--r--   0        0        0     4807 2022-07-28 11:09:03.261103 ELF_RSS-2.6.8/setup.py
--rw-r--r--   0        0        0     4881 2022-07-28 11:09:03.261752 ELF_RSS-2.6.8/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-07-30 16:54:38.849419 ELF_RSS-2.6.9/LICENSE
+-rw-r--r--   0        0        0     3314 2022-07-30 16:54:38.849419 ELF_RSS-2.6.9/README.md
+-rw-r--r--   0        0        0     1141 2022-07-30 16:54:38.849419 ELF_RSS-2.6.9/pyproject.toml
+-rw-r--r--   0        0        0     1681 2022-07-30 16:54:38.849419 ELF_RSS-2.6.9/src/plugins/ELF_RSS2/__init__.py
+-rw-r--r--   0        0        0      140 2022-07-30 16:54:38.849419 ELF_RSS-2.6.9/src/plugins/ELF_RSS2/command/__init__.py
+-rw-r--r--   0        0        0     1666 2022-07-30 16:54:38.849419 ELF_RSS-2.6.9/src/plugins/ELF_RSS2/command/add_cookies.py
+-rw-r--r--   0        0        0     2231 2022-07-30 16:54:38.849419 ELF_RSS-2.6.9/src/plugins/ELF_RSS2/command/add_dy.py
+-rw-r--r--   0        0        0    12027 2022-07-30 16:54:38.849419 ELF_RSS-2.6.9/src/plugins/ELF_RSS2/command/change_dy.py
+-rw-r--r--   0        0        0     2533 2022-07-30 16:54:38.853419 ELF_RSS-2.6.9/src/plugins/ELF_RSS2/command/del_dy.py
+-rw-r--r--   0        0        0     3781 2022-07-30 16:54:38.853419 ELF_RSS-2.6.9/src/plugins/ELF_RSS2/command/rsshub_add.py
+-rw-r--r--   0        0        0     2885 2022-07-30 16:54:38.853419 ELF_RSS-2.6.9/src/plugins/ELF_RSS2/command/show_all.py
+-rw-r--r--   0        0        0     2555 2022-07-30 16:54:38.853419 ELF_RSS-2.6.9/src/plugins/ELF_RSS2/command/show_dy.py
+-rw-r--r--   0        0        0     1231 2022-07-30 16:54:38.853419 ELF_RSS-2.6.9/src/plugins/ELF_RSS2/command/upload_group_file.py
+-rw-r--r--   0        0        0     1614 2022-07-30 16:54:38.853419 ELF_RSS-2.6.9/src/plugins/ELF_RSS2/config.py
+-rw-r--r--   0        0        0     3600 2022-07-30 16:54:38.853419 ELF_RSS-2.6.9/src/plugins/ELF_RSS2/my_trigger.py
+-rw-r--r--   0        0        0    11076 2022-07-30 16:54:38.853419 ELF_RSS-2.6.9/src/plugins/ELF_RSS2/parsing/__init__.py
+-rw-r--r--   0        0        0     4896 2022-07-30 16:54:38.853419 ELF_RSS-2.6.9/src/plugins/ELF_RSS2/parsing/cache_manage.py
+-rw-r--r--   0        0        0     1249 2022-07-30 16:54:38.853419 ELF_RSS-2.6.9/src/plugins/ELF_RSS2/parsing/check_update.py
+-rw-r--r--   0        0        0     3448 2022-07-30 16:54:38.853419 ELF_RSS-2.6.9/src/plugins/ELF_RSS2/parsing/download_torrent.py
+-rw-r--r--   0        0        0     4838 2022-07-30 16:54:38.853419 ELF_RSS-2.6.9/src/plugins/ELF_RSS2/parsing/handle_html_tag.py
+-rw-r--r--   0        0        0    10191 2022-07-30 16:54:38.853419 ELF_RSS-2.6.9/src/plugins/ELF_RSS2/parsing/handle_images.py
+-rw-r--r--   0        0        0     2015 2022-07-30 16:54:38.853419 ELF_RSS-2.6.9/src/plugins/ELF_RSS2/parsing/handle_translation.py
+-rw-r--r--   0        0        0     6836 2022-07-30 16:54:38.853419 ELF_RSS-2.6.9/src/plugins/ELF_RSS2/parsing/parsing_rss.py
+-rw-r--r--   0        0        0       82 2022-07-30 16:54:38.853419 ELF_RSS-2.6.9/src/plugins/ELF_RSS2/parsing/routes/__init__.py
+-rw-r--r--   0        0        0     4307 2022-07-30 16:54:38.853419 ELF_RSS-2.6.9/src/plugins/ELF_RSS2/parsing/routes/danbooru.py
+-rw-r--r--   0        0        0     1050 2022-07-30 16:54:38.853419 ELF_RSS-2.6.9/src/plugins/ELF_RSS2/parsing/routes/nga.py
+-rw-r--r--   0        0        0     5899 2022-07-30 16:54:38.853419 ELF_RSS-2.6.9/src/plugins/ELF_RSS2/parsing/routes/pixiv.py
+-rw-r--r--   0        0        0     1882 2022-07-30 16:54:38.853419 ELF_RSS-2.6.9/src/plugins/ELF_RSS2/parsing/routes/south_plus.py
+-rw-r--r--   0        0        0     2104 2022-07-30 16:54:38.853419 ELF_RSS-2.6.9/src/plugins/ELF_RSS2/parsing/routes/twitter.py
+-rw-r--r--   0        0        0     2521 2022-07-30 16:54:38.853419 ELF_RSS-2.6.9/src/plugins/ELF_RSS2/parsing/routes/weibo.py
+-rw-r--r--   0        0        0      621 2022-07-30 16:54:38.853419 ELF_RSS-2.6.9/src/plugins/ELF_RSS2/parsing/routes/yande_re.py
+-rw-r--r--   0        0        0      758 2022-07-30 16:54:38.853419 ELF_RSS-2.6.9/src/plugins/ELF_RSS2/parsing/routes/youtube.py
+-rw-r--r--   0        0        0     4392 2022-07-30 16:54:38.853419 ELF_RSS-2.6.9/src/plugins/ELF_RSS2/parsing/send_message.py
+-rw-r--r--   0        0        0      515 2022-07-30 16:54:38.853419 ELF_RSS-2.6.9/src/plugins/ELF_RSS2/parsing/utils.py
+-rw-r--r--   0        0        0      719 2022-07-30 16:54:38.853419 ELF_RSS-2.6.9/src/plugins/ELF_RSS2/permission.py
+-rw-r--r--   0        0        0     3385 2022-07-30 16:54:38.853419 ELF_RSS-2.6.9/src/plugins/ELF_RSS2/pikpak_offline.py
+-rw-r--r--   0        0        0     8748 2022-07-30 16:54:38.853419 ELF_RSS-2.6.9/src/plugins/ELF_RSS2/qbittorrent_download.py
+-rw-r--r--   0        0        0    10311 2022-07-30 16:54:38.853419 ELF_RSS-2.6.9/src/plugins/ELF_RSS2/rss_class.py
+-rw-r--r--   0        0        0     6345 2022-07-30 16:54:38.853419 ELF_RSS-2.6.9/src/plugins/ELF_RSS2/rss_parsing.py
+-rw-r--r--   0        0        0     5208 2022-07-30 16:54:38.853419 ELF_RSS-2.6.9/src/plugins/ELF_RSS2/utils.py
+-rw-r--r--   0        0        0     4807 2022-07-30 16:54:55.266060 ELF_RSS-2.6.9/setup.py
+-rw-r--r--   0        0        0     4881 2022-07-30 16:54:55.266542 ELF_RSS-2.6.9/PKG-INFO
```

### Comparing `ELF_RSS-2.6.8/LICENSE` & `ELF_RSS-2.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ELF_RSS-2.6.8/README.md` & `ELF_RSS-2.6.9/README.md`

 * *Files identical despite different names*

### Comparing `ELF_RSS-2.6.8/pyproject.toml` & `ELF_RSS-2.6.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ELF_RSS"
-version = "2.6.8"
+version = "2.6.9"
 description = "QQ机器人 RSS订阅 插件，订阅源建议选择 RSSHub"
 authors = ["Quan666 <i@Rori.eMail>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 packages = [
     { include = "ELF_RSS2", from = "src/plugins" },
 ]
```

### Comparing `ELF_RSS-2.6.8/src/plugins/ELF_RSS2/__init__.py` & `ELF_RSS-2.6.9/src/plugins/ELF_RSS2/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,40 +1,36 @@
 import asyncio
 
-import arrow
 from nonebot import on_metaevent, require
-from nonebot.adapters.onebot.v11 import Bot, Event, LifecycleMetaEvent
+from nonebot.adapters.onebot.v11 import Bot, LifecycleMetaEvent
 from nonebot.log import logger
 from nonebot.plugin import PluginMetadata
 
 from . import command
 from . import my_trigger as tr
 from .config import DATA_PATH, config
 from .rss_class import Rss
 from .utils import send_message_to_admin
 
-VERSION = "2.6.8"
+VERSION = "2.6.9"
 __plugin_meta__ = PluginMetadata(
     name="ELF_RSS",
     description="QQ机器人 RSS订阅 插件，订阅源建议选择 RSSHub",
     usage="https://github.com/Quan666/ELF_RSS",
     extra={"author": "Quan666 <i@Rori.eMail>", "version": VERSION},
 )
 
 scheduler = require("nonebot_plugin_apscheduler").scheduler
-START_TIME = arrow.now()
 
 
-async def check_first_connect(event: Event) -> bool:
-    return isinstance(event, LifecycleMetaEvent) and arrow.now() < START_TIME.shift(
-        minutes=1
-    )
+async def check_first_connect(_: LifecycleMetaEvent) -> bool:
+    return True
 
 
-start_metaevent = on_metaevent(rule=check_first_connect, block=True)
+start_metaevent = on_metaevent(rule=check_first_connect, temp=True)
 
 
 # 启动时发送启动成功信息
 @start_metaevent.handle()
 async def start(bot: Bot) -> None:
 
     # 启动后检查 data 目录，不存在就创建
```

### Comparing `ELF_RSS-2.6.8/src/plugins/ELF_RSS2/command/add_cookies.py` & `ELF_RSS-2.6.9/src/plugins/ELF_RSS2/command/add_cookies.py`

 * *Files identical despite different names*

### Comparing `ELF_RSS-2.6.8/src/plugins/ELF_RSS2/command/add_dy.py` & `ELF_RSS-2.6.9/src/plugins/ELF_RSS2/command/add_dy.py`

 * *Files identical despite different names*

### Comparing `ELF_RSS-2.6.8/src/plugins/ELF_RSS2/command/change_dy.py` & `ELF_RSS-2.6.9/src/plugins/ELF_RSS2/command/change_dy.py`

 * *Files 0% similar despite different names*

```diff
@@ -214,15 +214,15 @@
         if re.search(" (qq|qun|channel)=", change_info):
             await RSS_CHANGE.finish("❌ 禁止在子频道中修改订阅账号！如要取消订阅请使用 deldy 命令！")
         rss_list = [
             rss
             for rss in rss_list
             if rss.guild_channel_id == [str(guild_channel_id)]
             and not rss.user_id
-            and not rss.guild_channel_id
+            and not rss.group_id
         ]
 
     if not rss_list:
         await RSS_CHANGE.finish("❌ 请检查是否存在以下问题：\n1.要修改的订阅名不存在对应的记录\n2.当前群组或频道无权操作")
     elif len(rss_list) > 1 and " name=" in change_info:
         await RSS_CHANGE.finish("❌ 禁止将多个订阅批量改名！会因为名称相同起冲突！")
```

### Comparing `ELF_RSS-2.6.8/src/plugins/ELF_RSS2/command/del_dy.py` & `ELF_RSS-2.6.9/src/plugins/ELF_RSS2/command/del_dy.py`

 * *Files identical despite different names*

### Comparing `ELF_RSS-2.6.8/src/plugins/ELF_RSS2/command/rsshub_add.py` & `ELF_RSS-2.6.9/src/plugins/ELF_RSS2/command/rsshub_add.py`

 * *Files identical despite different names*

### Comparing `ELF_RSS-2.6.8/src/plugins/ELF_RSS2/command/show_all.py` & `ELF_RSS-2.6.9/src/plugins/ELF_RSS2/command/show_all.py`

 * *Files identical despite different names*

### Comparing `ELF_RSS-2.6.8/src/plugins/ELF_RSS2/command/show_dy.py` & `ELF_RSS-2.6.9/src/plugins/ELF_RSS2/command/show_dy.py`

 * *Files identical despite different names*

### Comparing `ELF_RSS-2.6.8/src/plugins/ELF_RSS2/command/upload_group_file.py` & `ELF_RSS-2.6.9/src/plugins/ELF_RSS2/command/upload_group_file.py`

 * *Files identical despite different names*

### Comparing `ELF_RSS-2.6.8/src/plugins/ELF_RSS2/config.py` & `ELF_RSS-2.6.9/src/plugins/ELF_RSS2/config.py`

 * *Files identical despite different names*

### Comparing `ELF_RSS-2.6.8/src/plugins/ELF_RSS2/my_trigger.py` & `ELF_RSS-2.6.9/src/plugins/ELF_RSS2/my_trigger.py`

 * *Files identical despite different names*

### Comparing `ELF_RSS-2.6.8/src/plugins/ELF_RSS2/parsing/__init__.py` & `ELF_RSS-2.6.9/src/plugins/ELF_RSS2/parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `ELF_RSS-2.6.8/src/plugins/ELF_RSS2/parsing/cache_manage.py` & `ELF_RSS-2.6.9/src/plugins/ELF_RSS2/parsing/cache_manage.py`

 * *Files identical despite different names*

### Comparing `ELF_RSS-2.6.8/src/plugins/ELF_RSS2/parsing/check_update.py` & `ELF_RSS-2.6.9/src/plugins/ELF_RSS2/parsing/check_update.py`

 * *Files identical despite different names*

### Comparing `ELF_RSS-2.6.8/src/plugins/ELF_RSS2/parsing/download_torrent.py` & `ELF_RSS-2.6.9/src/plugins/ELF_RSS2/parsing/download_torrent.py`

 * *Files identical despite different names*

### Comparing `ELF_RSS-2.6.8/src/plugins/ELF_RSS2/parsing/handle_html_tag.py` & `ELF_RSS-2.6.9/src/plugins/ELF_RSS2/parsing/handle_html_tag.py`

 * *Files identical despite different names*

### Comparing `ELF_RSS-2.6.8/src/plugins/ELF_RSS2/parsing/handle_images.py` & `ELF_RSS-2.6.9/src/plugins/ELF_RSS2/parsing/handle_images.py`

 * *Files identical despite different names*

### Comparing `ELF_RSS-2.6.8/src/plugins/ELF_RSS2/parsing/handle_translation.py` & `ELF_RSS-2.6.9/src/plugins/ELF_RSS2/parsing/handle_translation.py`

 * *Files identical despite different names*

### Comparing `ELF_RSS-2.6.8/src/plugins/ELF_RSS2/parsing/parsing_rss.py` & `ELF_RSS-2.6.9/src/plugins/ELF_RSS2/parsing/parsing_rss.py`

 * *Files identical despite different names*

### Comparing `ELF_RSS-2.6.8/src/plugins/ELF_RSS2/parsing/routes/danbooru.py` & `ELF_RSS-2.6.9/src/plugins/ELF_RSS2/parsing/routes/danbooru.py`

 * *Files identical despite different names*

### Comparing `ELF_RSS-2.6.8/src/plugins/ELF_RSS2/parsing/routes/nga.py` & `ELF_RSS-2.6.9/src/plugins/ELF_RSS2/parsing/routes/nga.py`

 * *Files identical despite different names*

### Comparing `ELF_RSS-2.6.8/src/plugins/ELF_RSS2/parsing/routes/pixiv.py` & `ELF_RSS-2.6.9/src/plugins/ELF_RSS2/parsing/routes/pixiv.py`

 * *Files identical despite different names*

### Comparing `ELF_RSS-2.6.8/src/plugins/ELF_RSS2/parsing/routes/south_plus.py` & `ELF_RSS-2.6.9/src/plugins/ELF_RSS2/parsing/routes/south_plus.py`

 * *Files identical despite different names*

### Comparing `ELF_RSS-2.6.8/src/plugins/ELF_RSS2/parsing/routes/twitter.py` & `ELF_RSS-2.6.9/src/plugins/ELF_RSS2/parsing/routes/twitter.py`

 * *Files identical despite different names*

### Comparing `ELF_RSS-2.6.8/src/plugins/ELF_RSS2/parsing/routes/weibo.py` & `ELF_RSS-2.6.9/src/plugins/ELF_RSS2/parsing/routes/weibo.py`

 * *Files identical despite different names*

### Comparing `ELF_RSS-2.6.8/src/plugins/ELF_RSS2/parsing/routes/yande_re.py` & `ELF_RSS-2.6.9/src/plugins/ELF_RSS2/parsing/routes/yande_re.py`

 * *Files identical despite different names*

### Comparing `ELF_RSS-2.6.8/src/plugins/ELF_RSS2/parsing/routes/youtube.py` & `ELF_RSS-2.6.9/src/plugins/ELF_RSS2/parsing/routes/youtube.py`

 * *Files identical despite different names*

### Comparing `ELF_RSS-2.6.8/src/plugins/ELF_RSS2/parsing/send_message.py` & `ELF_RSS-2.6.9/src/plugins/ELF_RSS2/parsing/send_message.py`

 * *Files identical despite different names*

### Comparing `ELF_RSS-2.6.8/src/plugins/ELF_RSS2/parsing/utils.py` & `ELF_RSS-2.6.9/src/plugins/ELF_RSS2/parsing/utils.py`

 * *Files identical despite different names*

### Comparing `ELF_RSS-2.6.8/src/plugins/ELF_RSS2/permission.py` & `ELF_RSS-2.6.9/src/plugins/ELF_RSS2/permission.py`

 * *Files identical despite different names*

### Comparing `ELF_RSS-2.6.8/src/plugins/ELF_RSS2/pikpak_offline.py` & `ELF_RSS-2.6.9/src/plugins/ELF_RSS2/pikpak_offline.py`

 * *Files identical despite different names*

### Comparing `ELF_RSS-2.6.8/src/plugins/ELF_RSS2/qbittorrent_download.py` & `ELF_RSS-2.6.9/src/plugins/ELF_RSS2/qbittorrent_download.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,14 +136,15 @@
 ) -> str:
     qb = await get_qb_client()
     if not qb:
         return ""
     # 获取种子 hash
     info = await get_torrent_info_from_hash(bot=bot, qb=qb, url=url, proxy=proxy)
     await rss_trigger(
+        bot,
         hash_str=info["hash"],
         group_ids=group_ids,
         name=f"订阅：{name}\n{info['filename']}\n文件大小：{info['size']}",
     )
     down_info[info["hash"]] = {
         "status": DOWN_STATUS_DOWNING,
         "start_time": arrow.now(),  # 下载开始时间
@@ -217,23 +218,23 @@
 
 # 撤回消息
 async def delete_msg(bot: Bot, msg_ids: List[Dict[str, Any]]) -> None:
     for msg_id in msg_ids:
         await bot.delete_msg(message_id=msg_id["message_id"])
 
 
-async def rss_trigger(hash_str: str, group_ids: List[str], name: str) -> None:
+async def rss_trigger(bot: Bot, hash_str: str, group_ids: List[str], name: str) -> None:
     scheduler = require("nonebot_plugin_apscheduler").scheduler
     # 制作一个频率为“ n 秒 / 次”的触发器
     trigger = IntervalTrigger(seconds=int(config.down_status_msg_date), jitter=10)
     job_defaults = {"max_instances": 1}
     # 添加任务
     scheduler.add_job(
         func=check_down_status,  # 要添加任务的函数，不要带参数
         trigger=trigger,  # 触发器
-        args=(hash_str, group_ids, name),  # 函数的参数列表，注意：只有一个值时，不能省略末尾的逗号
+        args=(bot, hash_str, group_ids, name),  # 函数的参数列表，注意：只有一个值时，不能省略末尾的逗号
         id=hash_str,
         misfire_grace_time=60,  # 允许的误差时间，建议不要省略
         job_defaults=job_defaults,
     )
     bot: Bot = get_bot()  # type: ignore
     await send_msg(bot, f"👏 {name}\nHash：{hash_str}\n下载任务添加成功！", group_ids)
```

### Comparing `ELF_RSS-2.6.8/src/plugins/ELF_RSS2/rss_class.py` & `ELF_RSS-2.6.9/src/plugins/ELF_RSS2/rss_class.py`

 * *Files identical despite different names*

### Comparing `ELF_RSS-2.6.8/src/plugins/ELF_RSS2/rss_parsing.py` & `ELF_RSS-2.6.9/src/plugins/ELF_RSS2/rss_parsing.py`

 * *Files identical despite different names*

### Comparing `ELF_RSS-2.6.8/src/plugins/ELF_RSS2/utils.py` & `ELF_RSS-2.6.9/src/plugins/ELF_RSS2/utils.py`

 * *Files identical despite different names*

### Comparing `ELF_RSS-2.6.8/setup.py` & `ELF_RSS-2.6.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
  'tenacity>=8.0.1,<9.0.0',
  'tinydb>=4.7.0,<5.0.0',
  'typing-extensions>=4.3.0,<5.0.0',
  'yarl>=1.7.2,<2.0.0']
 
 setup_kwargs = {
     'name': 'elf-rss',
-    'version': '2.6.8',
+    'version': '2.6.9',
     'description': 'QQ机器人 RSS订阅 插件，订阅源建议选择 RSSHub',
     'long_description': '# ELF_RSS\n\n[![Codacy Badge](https://app.codacy.com/project/badge/Grade/b799d894ed354d5999fb6047543c494c)](https://www.codacy.com/gh/Quan666/ELF_RSS/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=Quan666/ELF_RSS&amp;utm_campaign=Badge_Grade)\n[![QQ Group](https://img.shields.io/badge/qq%E7%BE%A4-984827132-orange?style=flat-square)](https://jq.qq.com/?_wv=1027&k=sST08Nkd)\n\n> 1. 容易使用的命令\n> 2. 更规范的代码，方便移植到你自己的机器人\n> 3. 使用全新的 [Nonebot2](https://v2.nonebot.dev/guide/) 框架\n\n这是一个以 Python 编写的 QQ 机器人插件，用于订阅 RSS 并实时以 QQ消息推送。\n\n算是第一次用 Python 写出来的比较完整、实用的项目。代码比较难看，正在重构中\n\n---\n\n当然也有很多插件能够做到订阅 RSS ，但不同的是，大多数都需要在服务器上修改相应配置才能添加订阅，而该插件只需要发送QQ消息给机器人就能动态添加订阅。\n\n对于订阅，支持QQ、QQ群、QQ频道的单个、多个订阅。\n\n每个订阅的个性化设置丰富，能够应付多种场景。\n\n## 功能介绍\n\n* 发送命令添加、删除、查询、修改 RSS 订阅\n* 交互式添加 RSSHub 订阅\n* 订阅内容翻译（使用谷歌机翻，可设置为百度翻译）\n* 个性化订阅设置（更新频率、翻译、仅标题、仅图片等）\n* 多平台支持\n* 图片压缩后发送\n* 种子下载并上传到群文件\n* 离线下载到 PikPak 网盘（方便追番）\n* 消息支持根据链接、标题、图片去重\n* 可设置只发送限定数量的图片，防止刷屏\n* 可设置从正文中要移除的指定内容，支持正则\n\n## 文档目录\n\n> 注意：推荐 Python 3.8.3+ 版本 Windows版安装包下载地址：[https://www.python.org/ftp/python/3.8.3/python-3.8.3-amd64.exe](https://www.python.org/ftp/python/3.8.3/python-3.8.3-amd64.exe)\n>\n> * [部署教程](docs/部署教程.md)\n> * [使用教程](docs/2.0%20使用教程.md)\n> * [使用教程 旧版](docs/1.0%20使用教程.md)\n> * [常见问题](docs/常见问题.md)\n> * [更新日志](docs/更新日志.md)\n\n## 效果预览\n\n![image-20201221163514747](https://cdn.jsdelivr.net/gh/Quan666/CDN/pic/image-20201221163514747.png)\n\n![image-20201221163555086](https://cdn.jsdelivr.net/gh/Quan666/CDN/pic/image-20201221163555086.png)\n\n![image-20201221163721358](https://cdn.jsdelivr.net/gh/Quan666/CDN/pic/image-20201221163721358.png)\n\n![image](https://user-images.githubusercontent.com/32663291/117431780-3373a100-af5c-11eb-9de2-ff75948abf1c.png)\n\n## TODO\n\n* [x] 1. 订阅信息保护，不在群组中输出订阅QQ、群组\n* [x] 2. 更为强大的检查更新时间设置\n* [x] 3. RSS 源中 torrent 自动下载并上传至订阅群（适合番剧订阅）\n* [x] 4. 暂停检查订阅更新\n* [x] 5. 正则匹配订阅名\n* [x] 6. 性能优化，尽可能替换为异步操作\n\n## 感谢以下项目或服务\n\n不分先后\n\n* [RSSHub](https://github.com/DIYgod/RSSHub)\n* [Nonebot](https://github.com/nonebot/nonebot2)\n* [酷Q（R. I. P）](https://cqp.cc/)\n* [coolq-http-api](https://github.com/richardchien/coolq-http-api)\n* [go-cqhttp](https://github.com/Mrs4s/go-cqhttp)\n\n## Star History\n\n[![Star History](https://starchart.cc/Quan666/ELF_RSS.svg)](https://starchart.cc/Quan666/ELF_RSS)\n',
     'author': 'Quan666',
     'author_email': 'i@Rori.eMail',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/Quan666/ELF_RSS',
```

### Comparing `ELF_RSS-2.6.8/PKG-INFO` & `ELF_RSS-2.6.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elf-rss
-Version: 2.6.8
+Version: 2.6.9
 Summary: QQ机器人 RSS订阅 插件，订阅源建议选择 RSSHub
 Home-page: https://github.com/Quan666/ELF_RSS
 License: GPL-3.0-only
 Keywords: nonebot,nonebot2,rss,elf,rsshub
 Author: Quan666
 Author-email: i@Rori.eMail
 Requires-Python: >=3.8.3,<4.0.0
```

