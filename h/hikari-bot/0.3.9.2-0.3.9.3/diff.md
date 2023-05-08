# Comparing `tmp/hikari_bot-0.3.9.2.tar.gz` & `tmp/hikari_bot-0.3.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hikari_bot-0.3.9.2.tar", max compression
+gzip compressed data, was "hikari_bot-0.3.9.3.tar", max compression
```

## Comparing `hikari_bot-0.3.9.2.tar` & `hikari_bot-0.3.9.3.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1084 2022-05-26 18:22:32.043723 hikari_bot-0.3.9.2/LICENSE
--rw-r--r--   0        0        0     1563 2023-05-08 09:10:31.371279 hikari_bot-0.3.9.2/pyproject.toml
--rw-r--r--   0        0        0    26184 2023-05-07 11:27:46.783601 hikari_bot-0.3.9.2/README.md
--rw-r--r--   0        0        0    13486 2023-05-07 11:27:46.785625 hikari_bot-0.3.9.2/src/plugins/hikari_bot/__init__.py
--rw-r--r--   0        0        0     3203 2023-05-07 05:07:46.111581 hikari_bot-0.3.9.2/src/plugins/hikari_bot/command_select.py
--rw-r--r--   0        0        0    12164 2023-05-07 05:07:46.113627 hikari_bot-0.3.9.2/src/plugins/hikari_bot/data_source.py
--rw-r--r--   0        0        0     3726 2023-05-07 05:07:46.115140 hikari_bot-0.3.9.2/src/plugins/hikari_bot/game/ban_search.py
--rw-r--r--   0        0        0     3752 2023-05-07 05:07:46.116149 hikari_bot-0.3.9.2/src/plugins/hikari_bot/game/box_check.py
--rw-r--r--   0        0        0     3137 2023-05-07 05:07:46.117158 hikari_bot-0.3.9.2/src/plugins/hikari_bot/game/ocr.py
--rw-r--r--   0        0        0      811 2023-05-07 05:07:46.118165 hikari_bot-0.3.9.2/src/plugins/hikari_bot/game/pupu.py
--rw-r--r--   0        0        0     2302 2023-02-20 07:47:11.427209 hikari_bot-0.3.9.2/src/plugins/hikari_bot/game/roll.py
--rw-r--r--   0        0        0     3739 2023-05-07 05:07:46.119176 hikari_bot-0.3.9.2/src/plugins/hikari_bot/game/sx.py
--rw-r--r--   0        0        0      933 2023-05-07 11:27:46.784634 hikari_bot-0.3.9.2/src/plugins/hikari_bot/HttpClient_pool.py
--rw-r--r--   0        0        0     7446 2023-05-07 05:07:46.120189 hikari_bot-0.3.9.2/src/plugins/hikari_bot/moudle/publicAPI.py
--rw-r--r--   0        0        0    12004 2023-05-07 05:07:46.121205 hikari_bot-0.3.9.2/src/plugins/hikari_bot/moudle/wws_bind.py
--rw-r--r--   0        0        0     6155 2023-05-07 05:07:46.122207 hikari_bot-0.3.9.2/src/plugins/hikari_bot/moudle/wws_clan.py
--rw-r--r--   0        0        0     3928 2023-05-07 05:07:46.124249 hikari_bot-0.3.9.2/src/plugins/hikari_bot/moudle/wws_info.py
--rw-r--r--   0        0        0     3769 2023-05-07 05:07:46.125254 hikari_bot-0.3.9.2/src/plugins/hikari_bot/moudle/wws_realTime.py
--rw-r--r--   0        0        0     4923 2023-05-07 05:07:46.126256 hikari_bot-0.3.9.2/src/plugins/hikari_bot/moudle/wws_recent.py
--rw-r--r--   0        0        0     9775 2023-05-07 05:07:46.127804 hikari_bot-0.3.9.2/src/plugins/hikari_bot/moudle/wws_record.py
--rw-r--r--   0        0        0    16544 2023-05-07 05:07:46.129848 hikari_bot-0.3.9.2/src/plugins/hikari_bot/moudle/wws_ship.py
--rw-r--r--   0        0        0     8141 2023-05-07 05:07:46.130810 hikari_bot-0.3.9.2/src/plugins/hikari_bot/moudle/wws_shiprank.py
--rw-r--r--   0        0        0   173077 2023-05-07 20:00:04.884480 hikari_bot-0.3.9.2/src/plugins/hikari_bot/template/Chart.min.js
--rw-r--r--   0        0        0    13279 2023-05-07 20:00:04.833941 hikari_bot-0.3.9.2/src/plugins/hikari_bot/template/chartjs-plugin-datalabels@1.0.0.js
--rw-r--r--   0        0        0     3710 2023-05-07 20:00:04.862245 hikari_bot-0.3.9.2/src/plugins/hikari_bot/template/select-ship.html
--rw-r--r--   0        0        0     5109 2023-05-07 20:00:04.816241 hikari_bot-0.3.9.2/src/plugins/hikari_bot/template/ship-rank.html
--rw-r--r--   0        0        0      225 2023-05-07 20:00:04.815238 hikari_bot-0.3.9.2/src/plugins/hikari_bot/template/text-help.css
--rw-r--r--   0        0        0     7284 2023-05-07 20:00:04.803947 hikari_bot-0.3.9.2/src/plugins/hikari_bot/template/wws-ban.html
--rw-r--r--   0        0        0    16757 2023-05-07 20:00:04.840519 hikari_bot-0.3.9.2/src/plugins/hikari_bot/template/wws-box-christmas.html
--rw-r--r--   0        0        0    18454 2023-05-07 20:00:04.804960 hikari_bot-0.3.9.2/src/plugins/hikari_bot/template/wws-clan.html
--rw-r--r--   0        0        0    23627 2023-05-07 20:00:04.798398 hikari_bot-0.3.9.2/src/plugins/hikari_bot/template/wws-info-recent.html
--rw-r--r--   0        0        0    25496 2023-05-07 20:00:04.828876 hikari_bot-0.3.9.2/src/plugins/hikari_bot/template/wws-info.html
--rw-r--r--   0        0        0     2396 2023-05-07 20:00:04.814176 hikari_bot-0.3.9.2/src/plugins/hikari_bot/template/wws-personalRecord.html
--rw-r--r--   0        0        0     6301 2022-09-02 06:25:22.613704 hikari_bot-0.3.9.2/src/plugins/hikari_bot/template/wws-realTime.html
--rw-r--r--   0        0        0    21658 2023-05-07 20:00:04.806975 hikari_bot-0.3.9.2/src/plugins/hikari_bot/template/wws-ship-recent.html
--rw-r--r--   0        0        0    20751 2023-05-07 20:00:04.835492 hikari_bot-0.3.9.2/src/plugins/hikari_bot/template/wws-ship.html
--rw-r--r--   0        0        0     9446 2023-05-07 20:00:04.830896 hikari_bot-0.3.9.2/src/plugins/hikari_bot/template/wws-sx.html
--rw-r--r--   0        0        0     5784 2023-05-07 20:00:04.842518 hikari_bot-0.3.9.2/src/plugins/hikari_bot/template/wws-unban.html
--rw-r--r--   0        0        0     3084 2023-02-20 07:47:11.431310 hikari_bot-0.3.9.2/src/plugins/hikari_bot/utils.py
--rw-r--r--   0        0        0    39031 1970-01-01 00:00:00.000000 hikari_bot-0.3.9.2/setup.py
--rw-r--r--   0        0        0    26845 1970-01-01 00:00:00.000000 hikari_bot-0.3.9.2/PKG-INFO
+-rw-r--r--   0        0        0     1084 2022-05-26 18:22:32.043723 hikari_bot-0.3.9.3/LICENSE
+-rw-r--r--   0        0        0     1563 2023-05-08 09:13:42.088757 hikari_bot-0.3.9.3/pyproject.toml
+-rw-r--r--   0        0        0    26184 2023-05-07 11:27:46.783601 hikari_bot-0.3.9.3/README.md
+-rw-r--r--   0        0        0    13486 2023-05-07 11:27:46.785625 hikari_bot-0.3.9.3/src/plugins/hikari_bot/__init__.py
+-rw-r--r--   0        0        0     3203 2023-05-07 05:07:46.111581 hikari_bot-0.3.9.3/src/plugins/hikari_bot/command_select.py
+-rw-r--r--   0        0        0    12164 2023-05-07 05:07:46.113627 hikari_bot-0.3.9.3/src/plugins/hikari_bot/data_source.py
+-rw-r--r--   0        0        0     3726 2023-05-07 05:07:46.115140 hikari_bot-0.3.9.3/src/plugins/hikari_bot/game/ban_search.py
+-rw-r--r--   0        0        0     3752 2023-05-07 05:07:46.116149 hikari_bot-0.3.9.3/src/plugins/hikari_bot/game/box_check.py
+-rw-r--r--   0        0        0     3137 2023-05-07 05:07:46.117158 hikari_bot-0.3.9.3/src/plugins/hikari_bot/game/ocr.py
+-rw-r--r--   0        0        0      811 2023-05-07 05:07:46.118165 hikari_bot-0.3.9.3/src/plugins/hikari_bot/game/pupu.py
+-rw-r--r--   0        0        0     2302 2023-02-20 07:47:11.427209 hikari_bot-0.3.9.3/src/plugins/hikari_bot/game/roll.py
+-rw-r--r--   0        0        0     3739 2023-05-07 05:07:46.119176 hikari_bot-0.3.9.3/src/plugins/hikari_bot/game/sx.py
+-rw-r--r--   0        0        0      933 2023-05-07 11:27:46.784634 hikari_bot-0.3.9.3/src/plugins/hikari_bot/HttpClient_pool.py
+-rw-r--r--   0        0        0     7446 2023-05-07 05:07:46.120189 hikari_bot-0.3.9.3/src/plugins/hikari_bot/moudle/publicAPI.py
+-rw-r--r--   0        0        0    12004 2023-05-07 05:07:46.121205 hikari_bot-0.3.9.3/src/plugins/hikari_bot/moudle/wws_bind.py
+-rw-r--r--   0        0        0     6155 2023-05-07 05:07:46.122207 hikari_bot-0.3.9.3/src/plugins/hikari_bot/moudle/wws_clan.py
+-rw-r--r--   0        0        0     3928 2023-05-07 05:07:46.124249 hikari_bot-0.3.9.3/src/plugins/hikari_bot/moudle/wws_info.py
+-rw-r--r--   0        0        0     3769 2023-05-07 05:07:46.125254 hikari_bot-0.3.9.3/src/plugins/hikari_bot/moudle/wws_realTime.py
+-rw-r--r--   0        0        0     4923 2023-05-07 05:07:46.126256 hikari_bot-0.3.9.3/src/plugins/hikari_bot/moudle/wws_recent.py
+-rw-r--r--   0        0        0     9775 2023-05-07 05:07:46.127804 hikari_bot-0.3.9.3/src/plugins/hikari_bot/moudle/wws_record.py
+-rw-r--r--   0        0        0    16544 2023-05-07 05:07:46.129848 hikari_bot-0.3.9.3/src/plugins/hikari_bot/moudle/wws_ship.py
+-rw-r--r--   0        0        0     8141 2023-05-07 05:07:46.130810 hikari_bot-0.3.9.3/src/plugins/hikari_bot/moudle/wws_shiprank.py
+-rw-r--r--   0        0        0   173077 2023-05-07 20:00:04.884480 hikari_bot-0.3.9.3/src/plugins/hikari_bot/template/Chart.min.js
+-rw-r--r--   0        0        0    13279 2023-05-07 20:00:04.833941 hikari_bot-0.3.9.3/src/plugins/hikari_bot/template/chartjs-plugin-datalabels@1.0.0.js
+-rw-r--r--   0        0        0     3710 2023-05-07 20:00:04.862245 hikari_bot-0.3.9.3/src/plugins/hikari_bot/template/select-ship.html
+-rw-r--r--   0        0        0     5109 2023-05-07 20:00:04.816241 hikari_bot-0.3.9.3/src/plugins/hikari_bot/template/ship-rank.html
+-rw-r--r--   0        0        0      225 2023-05-07 20:00:04.815238 hikari_bot-0.3.9.3/src/plugins/hikari_bot/template/text-help.css
+-rw-r--r--   0        0        0     7284 2023-05-07 20:00:04.803947 hikari_bot-0.3.9.3/src/plugins/hikari_bot/template/wws-ban.html
+-rw-r--r--   0        0        0    16757 2023-05-07 20:00:04.840519 hikari_bot-0.3.9.3/src/plugins/hikari_bot/template/wws-box-christmas.html
+-rw-r--r--   0        0        0    18454 2023-05-07 20:00:04.804960 hikari_bot-0.3.9.3/src/plugins/hikari_bot/template/wws-clan.html
+-rw-r--r--   0        0        0    23627 2023-05-07 20:00:04.798398 hikari_bot-0.3.9.3/src/plugins/hikari_bot/template/wws-info-recent.html
+-rw-r--r--   0        0        0    25496 2023-05-07 20:00:04.828876 hikari_bot-0.3.9.3/src/plugins/hikari_bot/template/wws-info.html
+-rw-r--r--   0        0        0     2396 2023-05-07 20:00:04.814176 hikari_bot-0.3.9.3/src/plugins/hikari_bot/template/wws-personalRecord.html
+-rw-r--r--   0        0        0     6301 2022-09-02 06:25:22.613704 hikari_bot-0.3.9.3/src/plugins/hikari_bot/template/wws-realTime.html
+-rw-r--r--   0        0        0    21658 2023-05-07 20:00:04.806975 hikari_bot-0.3.9.3/src/plugins/hikari_bot/template/wws-ship-recent.html
+-rw-r--r--   0        0        0    20751 2023-05-07 20:00:04.835492 hikari_bot-0.3.9.3/src/plugins/hikari_bot/template/wws-ship.html
+-rw-r--r--   0        0        0     9446 2023-05-07 20:00:04.830896 hikari_bot-0.3.9.3/src/plugins/hikari_bot/template/wws-sx.html
+-rw-r--r--   0        0        0     5784 2023-05-07 20:00:04.842518 hikari_bot-0.3.9.3/src/plugins/hikari_bot/template/wws-unban.html
+-rw-r--r--   0        0        0     3084 2023-02-20 07:47:11.431310 hikari_bot-0.3.9.3/src/plugins/hikari_bot/utils.py
+-rw-r--r--   0        0        0    39031 1970-01-01 00:00:00.000000 hikari_bot-0.3.9.3/setup.py
+-rw-r--r--   0        0        0    26845 1970-01-01 00:00:00.000000 hikari_bot-0.3.9.3/PKG-INFO
```

### Comparing `hikari_bot-0.3.9.2/LICENSE` & `hikari_bot-0.3.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hikari_bot-0.3.9.2/pyproject.toml` & `hikari_bot-0.3.9.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hikari-bot"
-version = "0.3.9.2"
+version = "0.3.9.3"
 description = "Nonebot2 HikariBot,支持战舰世界水表查询"
 authors = ["benx1n <shirakamikanade@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/benx1n/HikariBot"
 repository = "https://github.com/benx1n/HikariBot"
 keywords = ["nonebot", "nonebot2", "qqbot", "wows", "wws","bot","stats"]
@@ -16,15 +16,15 @@
 python = "^3.8.0"
 nonebot2 = { version = "^2.0.0-beta.1", extras = ["fastapi"] }
 nonebot-adapter-onebot = "^2.1.0"
 nonebot-plugin-htmlrender = "^0.2.0.1"
 nonebot-plugin-apscheduler = "^0.2.0"
 nonebot_plugin_guild_patch = "^0.2.1"
 nonebot-plugin-reboot = "^0.1.3"
-httpx = { version = ">=0.22.0", extras = ["http2"] }
+httpx = { version = ">=0.24.0", extras = ["http2"] }
 Jinja2 = "^3.0.0"
 beautifulsoup4 = "^4.11.1"
 orjson = "^3.8.11"
 
 [tool.poetry.group.dev.dependencies]
 nb-cli = "^0.6.0"
 nonebot-plugin-gocqhttp = "^0.6.2"
```

### Comparing `hikari_bot-0.3.9.2/README.md` & `hikari_bot-0.3.9.3/README.md`

 * *Files identical despite different names*

### Comparing `hikari_bot-0.3.9.2/src/plugins/hikari_bot/__init__.py` & `hikari_bot-0.3.9.3/src/plugins/hikari_bot/__init__.py`

 * *Files identical despite different names*

### Comparing `hikari_bot-0.3.9.2/src/plugins/hikari_bot/command_select.py` & `hikari_bot-0.3.9.3/src/plugins/hikari_bot/command_select.py`

 * *Files identical despite different names*

### Comparing `hikari_bot-0.3.9.2/src/plugins/hikari_bot/data_source.py` & `hikari_bot-0.3.9.3/src/plugins/hikari_bot/data_source.py`

 * *Files identical despite different names*

### Comparing `hikari_bot-0.3.9.2/src/plugins/hikari_bot/game/ban_search.py` & `hikari_bot-0.3.9.3/src/plugins/hikari_bot/game/ban_search.py`

 * *Files identical despite different names*

### Comparing `hikari_bot-0.3.9.2/src/plugins/hikari_bot/game/box_check.py` & `hikari_bot-0.3.9.3/src/plugins/hikari_bot/game/box_check.py`

 * *Files identical despite different names*

### Comparing `hikari_bot-0.3.9.2/src/plugins/hikari_bot/game/ocr.py` & `hikari_bot-0.3.9.3/src/plugins/hikari_bot/game/ocr.py`

 * *Files identical despite different names*

### Comparing `hikari_bot-0.3.9.2/src/plugins/hikari_bot/game/pupu.py` & `hikari_bot-0.3.9.3/src/plugins/hikari_bot/game/pupu.py`

 * *Files identical despite different names*

### Comparing `hikari_bot-0.3.9.2/src/plugins/hikari_bot/game/roll.py` & `hikari_bot-0.3.9.3/src/plugins/hikari_bot/game/roll.py`

 * *Files identical despite different names*

### Comparing `hikari_bot-0.3.9.2/src/plugins/hikari_bot/game/sx.py` & `hikari_bot-0.3.9.3/src/plugins/hikari_bot/game/sx.py`

 * *Files identical despite different names*

### Comparing `hikari_bot-0.3.9.2/src/plugins/hikari_bot/HttpClient_pool.py` & `hikari_bot-0.3.9.3/src/plugins/hikari_bot/HttpClient_pool.py`

 * *Files identical despite different names*

### Comparing `hikari_bot-0.3.9.2/src/plugins/hikari_bot/moudle/publicAPI.py` & `hikari_bot-0.3.9.3/src/plugins/hikari_bot/moudle/publicAPI.py`

 * *Files identical despite different names*

### Comparing `hikari_bot-0.3.9.2/src/plugins/hikari_bot/moudle/wws_bind.py` & `hikari_bot-0.3.9.3/src/plugins/hikari_bot/moudle/wws_bind.py`

 * *Files identical despite different names*

### Comparing `hikari_bot-0.3.9.2/src/plugins/hikari_bot/moudle/wws_clan.py` & `hikari_bot-0.3.9.3/src/plugins/hikari_bot/moudle/wws_clan.py`

 * *Files identical despite different names*

### Comparing `hikari_bot-0.3.9.2/src/plugins/hikari_bot/moudle/wws_info.py` & `hikari_bot-0.3.9.3/src/plugins/hikari_bot/moudle/wws_info.py`

 * *Files identical despite different names*

### Comparing `hikari_bot-0.3.9.2/src/plugins/hikari_bot/moudle/wws_realTime.py` & `hikari_bot-0.3.9.3/src/plugins/hikari_bot/moudle/wws_realTime.py`

 * *Files identical despite different names*

### Comparing `hikari_bot-0.3.9.2/src/plugins/hikari_bot/moudle/wws_recent.py` & `hikari_bot-0.3.9.3/src/plugins/hikari_bot/moudle/wws_recent.py`

 * *Files identical despite different names*

### Comparing `hikari_bot-0.3.9.2/src/plugins/hikari_bot/moudle/wws_record.py` & `hikari_bot-0.3.9.3/src/plugins/hikari_bot/moudle/wws_record.py`

 * *Files identical despite different names*

### Comparing `hikari_bot-0.3.9.2/src/plugins/hikari_bot/moudle/wws_ship.py` & `hikari_bot-0.3.9.3/src/plugins/hikari_bot/moudle/wws_ship.py`

 * *Files identical despite different names*

### Comparing `hikari_bot-0.3.9.2/src/plugins/hikari_bot/moudle/wws_shiprank.py` & `hikari_bot-0.3.9.3/src/plugins/hikari_bot/moudle/wws_shiprank.py`

 * *Files identical despite different names*

### Comparing `hikari_bot-0.3.9.2/src/plugins/hikari_bot/template/Chart.min.js` & `hikari_bot-0.3.9.3/src/plugins/hikari_bot/template/Chart.min.js`

 * *Files identical despite different names*

### Comparing `hikari_bot-0.3.9.2/src/plugins/hikari_bot/template/chartjs-plugin-datalabels@1.0.0.js` & `hikari_bot-0.3.9.3/src/plugins/hikari_bot/template/chartjs-plugin-datalabels@1.0.0.js`

 * *Files identical despite different names*

### Comparing `hikari_bot-0.3.9.2/src/plugins/hikari_bot/template/select-ship.html` & `hikari_bot-0.3.9.3/src/plugins/hikari_bot/template/select-ship.html`

 * *Files identical despite different names*

### Comparing `hikari_bot-0.3.9.2/src/plugins/hikari_bot/template/ship-rank.html` & `hikari_bot-0.3.9.3/src/plugins/hikari_bot/template/ship-rank.html`

 * *Files identical despite different names*

### Comparing `hikari_bot-0.3.9.2/src/plugins/hikari_bot/template/wws-ban.html` & `hikari_bot-0.3.9.3/src/plugins/hikari_bot/template/wws-ban.html`

 * *Files identical despite different names*

### Comparing `hikari_bot-0.3.9.2/src/plugins/hikari_bot/template/wws-box-christmas.html` & `hikari_bot-0.3.9.3/src/plugins/hikari_bot/template/wws-box-christmas.html`

 * *Files identical despite different names*

### Comparing `hikari_bot-0.3.9.2/src/plugins/hikari_bot/template/wws-clan.html` & `hikari_bot-0.3.9.3/src/plugins/hikari_bot/template/wws-clan.html`

 * *Files identical despite different names*

### Comparing `hikari_bot-0.3.9.2/src/plugins/hikari_bot/template/wws-info-recent.html` & `hikari_bot-0.3.9.3/src/plugins/hikari_bot/template/wws-info-recent.html`

 * *Files identical despite different names*

### Comparing `hikari_bot-0.3.9.2/src/plugins/hikari_bot/template/wws-info.html` & `hikari_bot-0.3.9.3/src/plugins/hikari_bot/template/wws-info.html`

 * *Files identical despite different names*

### Comparing `hikari_bot-0.3.9.2/src/plugins/hikari_bot/template/wws-personalRecord.html` & `hikari_bot-0.3.9.3/src/plugins/hikari_bot/template/wws-personalRecord.html`

 * *Files identical despite different names*

### Comparing `hikari_bot-0.3.9.2/src/plugins/hikari_bot/template/wws-realTime.html` & `hikari_bot-0.3.9.3/src/plugins/hikari_bot/template/wws-realTime.html`

 * *Files identical despite different names*

### Comparing `hikari_bot-0.3.9.2/src/plugins/hikari_bot/template/wws-ship-recent.html` & `hikari_bot-0.3.9.3/src/plugins/hikari_bot/template/wws-ship-recent.html`

 * *Files identical despite different names*

### Comparing `hikari_bot-0.3.9.2/src/plugins/hikari_bot/template/wws-ship.html` & `hikari_bot-0.3.9.3/src/plugins/hikari_bot/template/wws-ship.html`

 * *Files identical despite different names*

### Comparing `hikari_bot-0.3.9.2/src/plugins/hikari_bot/template/wws-sx.html` & `hikari_bot-0.3.9.3/src/plugins/hikari_bot/template/wws-sx.html`

 * *Files identical despite different names*

### Comparing `hikari_bot-0.3.9.2/src/plugins/hikari_bot/template/wws-unban.html` & `hikari_bot-0.3.9.3/src/plugins/hikari_bot/template/wws-unban.html`

 * *Files identical despite different names*

### Comparing `hikari_bot-0.3.9.2/src/plugins/hikari_bot/utils.py` & `hikari_bot-0.3.9.3/src/plugins/hikari_bot/utils.py`

 * *Files identical despite different names*

### Comparing `hikari_bot-0.3.9.2/setup.py` & `hikari_bot-0.3.9.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -265,26 +265,26 @@
                 'template/wws-unban.html',
                 'template/wws-unban.html',
                 'template/wws-unban.html']}
 
 install_requires = \
 ['Jinja2>=3.0.0,<4.0.0',
  'beautifulsoup4>=4.11.1,<5.0.0',
- 'httpx[http2]>=0.22.0',
+ 'httpx[http2]>=0.24.0',
  'nonebot-adapter-onebot>=2.1.0,<3.0.0',
  'nonebot-plugin-apscheduler>=0.2.0,<0.3.0',
  'nonebot-plugin-htmlrender>=0.2.0.1,<0.3.0.0',
  'nonebot-plugin-reboot>=0.1.3,<0.2.0',
  'nonebot2[fastapi]>=2.0.0-beta.1,<3.0.0',
  'nonebot_plugin_guild_patch>=0.2.1,<0.3.0',
  'orjson>=3.8.11,<4.0.0']
 
 setup_kwargs = {
     'name': 'hikari-bot',
-    'version': '0.3.9.2',
+    'version': '0.3.9.3',
     'description': 'Nonebot2 HikariBot,支持战舰世界水表查询',
     'long_description': '<!-- markdownlint-disable MD033 MD041 -->\n<p align="center">\n  <a href="https://github.com/benx1n/HikariBot"><img src="https://s2.loli.net/2022/05/28/SFsER8m6TL7jwJ2.png" alt="Hikari " style="width:200px; height:200px" ></a>\n</p>\n\n<div align="center">\n\n# Hikari\n\n<!-- prettier-ignore-start -->\n<!-- markdownlint-disable-next-line MD036 -->\n战舰世界水表BOT\n<!-- prettier-ignore-end -->\n\n\n\n<p align="center">\n  <a href="https://pypi.python.org/pypi/hikari-bot">\n    <img src="https://img.shields.io/pypi/v/hikari-bot" alt="pypi">\n  </a>\n  <img src="https://img.shields.io/badge/python-3.8.0+-blue" alt="python">\n  <a href="https://jq.qq.com/?_wv=1027&k=S2WcTKi5">\n    <img src="https://img.shields.io/badge/QQ%E7%BE%A4-967546463-orange?style=flat-square" alt="QQ Chat Group">\n  </a>\n  <a href="https://qun.qq.com/qqweb/qunpro/share?_wv=3&_wwv=128&appChannel=share&inviteCode=1W4NX2S&from=181074&biz=ka#/pc">\n    <img src="https://img.shields.io/badge/QQ%E9%A2%91%E9%81%93-yuyuko助手-5492ff?style=flat-square" alt="QQ Channel">\n  </a>\n\n# 💘您不打算给可爱的Hikari点个Star吗QAQ\n</p>\n</div>\n\n## 简介\n\n战舰世界水表BOT，基于Nonebot2  \n水表人，出击！wws me recent！！！  \nQQ频道官方机器人已上线，请点击上方链接加入体验~  \n[Hoshino版插件](https://github.com/benx1n/wows-stats-bot)\n\n\n## 特色\n\n- [x] 账号总体、单船、近期战绩\n- [x] 全指令支持参数乱序\n- [x] 快速切换绑定账号\n- [x] 实时推送对局信息\n- [x] 支持@快速查询\n- [x] 全异步，高并发下性能更优\n- [x] 支持频道（非官方bot类型）\n\n  <details>\n  <summary>点我查看功能列表</summary>\n\n  - 绑定账号：wws bind/set/绑定 [服务器+游戏昵称]：\n  - 查询账号绑定列表：wws [查询/查]绑定/绑定列表 [me/@群友]：\n  - 切换删除绑定账号：wws [切换/删除]绑定 [序号]\n  - 查询账号总体战绩：wws [(服务器+游戏昵称)/@群友/me]\n  - 查询账号历史记录：wws [(服务器+游戏昵称)/@群友/me] record\n  - 查询账号近期战绩：wws [(服务器+游戏昵称)/@群友/me] recent [日期]\n  - 查询单船总体战绩：wws [(服务器+游戏昵称)/@群友/me] ship [船名]\n  - 查询单船近期战绩：wws [(服务器+游戏昵称)/@群友/me] ship [船名] recent [日期]\n  - 查询服务器排行榜：wws [服务器+战舰名] rank/ship.rank\n  - 查询军团详细信息：wws [(服务器+军团名)/@群友/me] clan\n  - 查询军团历史记录：wws [(服务器+军团名)/@群友/me] clan record\n  - 查询舰船中英文名：wws [搜/查船名] [国家][等级][类型]\n  - 检查版本更新：wws 检查更新\n  - 更新：wws 更新Hikari\n  - 查看帮助：wws help\n  - 噗噗：一言\n\n  </details>\n  <details>\n  <summary>点我查看与Hoshino版的区别</summary>\n\n  - Hikari所使用的Nonebot2框架相比Hoshino更易部署，且两者在单环境下不兼容\n  - 一些功能比如频道目前仅支持Hikari\n  - Hoshino的插件生态更偏向PCR，具体可以查看[Nonebot2商店](https://v2.nonebot.dev/store)和[Hoshino插件索引](https://github.com/pcrbot/HoshinoBot-plugins-index)\n  - 由于个人精力原因，主要功能开发和维护面向Hikari，Hoshino版仅做最低限度功能适配\n\n  </details>\n  <details>\n  <summary>点我查看遇到问题如何解决</summary>\n\n  - [ ] 请确认您已按文档中部署流程进行\n  - [ ] 请确认您已完整浏览[可能会遇到的问题](https://github.com/benx1n/HikariBot#%E5%8F%AF%E8%83%BD%E4%BC%9A%E9%81%87%E5%88%B0%E7%9A%84%E9%97%AE%E9%A2%98)，且仍无法自行解决\n  - [ ] [提问的智慧](https://github.com/ryanhanwu/How-To-Ask-Questions-The-Smart-Way/blob/main/README-zh_CN.md)\n  - [ ] 提供系统环境和bot版本，以及出现问题前后至少 10 秒的完整日志内容。请自行删除日志内存在的个人信息及敏感内容\n\n  </details>\n## 在Windows系统上快速部署\n>点我查看[视频教程](https://www.bilibili.com/video/BV1XP411U7rC)\n\n  `windows安装python版本请勿大于3.11,建议版本3.9`\n\n1. 下载Hikari的[最新Release](https://github.com/benx1n/HikariBot/releases/download/Latest/release_windows.zip)并解压到合适文件夹\n2. 复制一份`.env.prod-example`文件，并将其重命名为`.env.prod`,打开并按其中注释编辑\n    >只显示了.env，没有后面的后缀？请百度`windows如何显示文件后缀名`\n    ```\n    API_TOKEN = xxxxxxxx #无需引号，TOKEN即回复您的邮件所带的一串由[数字+冒号+英文/数字]组成的字符串\n    SUPERUSERS=["QQ号"]\n    ```\n   - 最后TOKEN应该长这样 `API_TOKEN = 123764323:ba1f2511fc30423bdbb183fe33`\n   - 从0.3.2.2版本开始，您没有填写的配置将按.env文件中的默认配置执行，具体逻辑为\n      - 私聊、频道默认禁用\n      - 群聊默认开启，默认屏蔽官方交流群\n      - 默认WEB登录账号密码为admin/admin，如有需要请自行修改，无需设置密码请删除env.prod中的配置项\n\n3. 双击`启动.bat`\n    - 页面加载不出请尝试刷新一下，已知IE浏览器可能存在一些问题\n    - 此时若没有报错，您可以在打开的页面`http://127.0.0.1:8080/go-cqhttp/`中\n      点击左侧添加账号，重启bot即可在网页上看到相应信息（大概率需要扫码）\n    - 如果重启后go-cqhhtp一直卡在扫码或无限重启，请跳转[无法使用内嵌go-cqhttp登录](https://github.com/benx1n/HikariBot#%E6%97%A0%E6%B3%95%E4%BD%BF%E7%94%A8%E5%86%85%E5%B5%8Cgo-cqhttp%E7%99%BB%E5%BD%95bot)\n\n## Linux一键脚本\n> 仅支持Debian、CentOS、Ubuntu\n```\nwget -qO - https://fastly.jsdelivr.net/gh/benx1n/HikariBot@master/install.sh | bash\n```\n\n\n## 使用Docker部署\n- Docker目录下是一个简单的Dockerfile，可以基于官方的Python容器封装一个完整的HikariBot\n  - 以`12hydrogen/hikari-bot:latest`上线官方仓库\n- 注意需要将内部的8080端口映射出来\n  ```\n  docker run -d -P 12hydrogen/hikari-bot:latest -t [token] -i [qqid] # 首次使用需输入token和qqid，-P表示将8080端口随机映射至主机\n  docker run -d -p 12345:8080 12hydrogen/hikari-bot:latest -t [token] -i [qqid] # 使用-p以指定映射在外的端口\n  ```\n- 运行上述指令后会在终端显示一串字符，即Docker容器的标识符，一般使用前几位即可唯一确定一个容器\n  ```\n  1a2b3c4d5e..... # 标识符\n  docker stop 1a2b # 使用前四位确定，stop即停止容器\n  1a2b3c4d5e.....\n  docker start 1a2b # start即启动容器\n  1a2b3c4d5e.....\n  docker restart 1a2b # restart即重启容器\n  1a2b3c4d5e.....\n  ```\n- 在更新后即上传新版本容器\n  ```\n  docker pull 12hydrogen/hikari-bot:latest # 更新\n  docker stop 1a2b\n  1a2b...\n  docker run -d --volumes-from 1a2b -P 12hydrogen/hikari-bot:latest -t [token] -i [qqid] # 随机映射\n  or\n  docker run -d --volumes-from 1a2b -p 12345:8080 12hydrogen/hikari-bot:latest -t [token] -i [qqid] # 指定映射\n  9z8y... # 注意标识符变化了\n  docker rm 1a2b # 删除旧容器，\n  1a2b...\n  ```\n- 将配置文件与容器分离\n  使用volume在宿主机保存相关账号信息，更新时按照相关步骤继承volume即可\n\n## 在Windows系统上完整部署\n1. 下载[Git](https://git-scm.com/download/win)、[Python](https://www.python.org/downloads/windows/)并安装\n    >Python版本需>3.8，或参考[Hoshino版插件](https://github.com/benx1n/wows-stats-bot)中使用Conda虚拟环境\n    >\n    >请注意python安装时勾选或点击`添加到环境变量`，可以安装后cmd中输入`python --version`来验证是否成功\n    >\n    >否则请自行百度如何添加python到环境变量\n\n3. 打开一个合适的文件夹，鼠标右键——Git Bash here，输入以下命令（任选一条）克隆本Hikari仓库\n    ```\n    git clone https://github.com/benx1n/HikariBot.git\n\n    git clone https://gitee.com/benx1n/HikariBot.git\n    ```\n3. 以管理员身份运行`一键安装.bat`\n    >等效于在cmd中执行如下代码\n    ```\n    python -m pip install nb-cli hikari-bot nonebot-plugin-apscheduler nonebot-plugin-gocqhttp -i https://pypi.tuna.tsinghua.edu.cn/simple\n    ```\n\n4. 复制一份`.env.prod-example`文件，并将其重命名为`.env.prod`,打开并按其中注释编辑\n    >只显示了.env，没有后面的后缀？请百度`windows如何显示文件后缀名`\n    ```\n    API_TOKEN = xxxxxxxx #无需引号，TOKEN即回复您的邮件所带的一串由[数字+冒号+英文/数字]组成的字符串\n    SUPERUSERS=["QQ号"]\n    ```\n   - 最后TOKEN应该长这样 `API_TOKEN = 123764323:ba1f2511fc30423bdbb183fe33`\n   - 从0.3.2.2版本开始，您没有填写的配置将按.env文件中的默认配置执行，具体逻辑为\n      - 私聊、频道默认禁用\n      - 群聊默认开启，默认屏蔽官方交流群`\n      - 默认WEB登录账号密码为admin/admin，如有需要请自行修改，无需设置密码请删除env.prod中的配置项\n      - 默认开启噗噗\n      - 默认开启缓存上报\n      - 默认关闭代理\n\n5. 双击`启动.bat`，在打开的浏览器中添加bot账号密码，重新启动Hikari\n    - 页面加载不出请尝试刷新一下，已知IE浏览器可能存在一些问题\n    - 此时若没有报错，您可以在打开的页面`http://127.0.0.1:8080/go-cqhttp/`中\n      点击左侧添加账号，重启bot即可在网页上看到相应信息（大概率需要扫码）\n    - 如果重启后go-cqhhtp一直卡在扫码或无限重启，请跳转[无法使用内嵌go-cqhttp登录](https://github.com/benx1n/HikariBot#%E6%97%A0%E6%B3%95%E4%BD%BF%E7%94%A8%E5%86%85%E5%B5%8Cgo-cqhttp%E7%99%BB%E5%BD%95bot)\n\n\n## ~~在Linux上完整部署~~\n- 需要Python基本环境\n- Clone本仓库\n- 使用`./manage.sh`，基于原有批处理脚本\n- 无参数调用以获取使用帮助\n1. `install`\n    - 安装必须的依赖与bot本体\n2. `update`\n    - 更新bot\n3. `start [-t/--token] [token] [-i/--id] [qqid]`\n    - 运行bot\n    - 在当前目录下不存在`.env.prod`的情况下从参数获取token和qqid以创建相应文件，否则直接运行\n    - 考虑到使用Linux部署时多数情况下本地不存在图形界面，有风险的向公网开放访问\n    - 加入验证机制（listed）\n\n\n## 作为已有Bot的插件部署（如真寻、Haruka）\n1. 如果您已经有了一个基于Nonebot2的机器人（例如真寻），您可以直接\n    ```\n    pip install hikari-bot\n    ```\n2. 在bot的bot.py中加入\n    ```\n    nonebot.load_plugin(\'nonebot_plugin_htmlrender\')\n    nonebot.load_plugin(\'hikari_bot\')\n    ```\n3. 在环境文件中加入以下配置项\n    ```\n    API_TOKEN = xxxxxxxxxxxx\n    SUPERUSERS=["QQ号"]\n    private = false                 #开启私聊\n    group = true                    #开启群聊\n    channel = false                 #开启频道\n    all_channel = false             #是否全频道生效，无论此项配置如何，channel_list中的频道一定会开启\n    channel_list = []               #频道列表白名单，数组形式，可在控制台中获取相应的channel_id\n    ban_group_list = [967546463]    #群列表黑名单，默认屏蔽了开发者交流群\n    pupu = true                     #是否开启噗噗\n    check_cache = true              #是否开启缓存上报,可降低高峰期延迟,如果错误日志中频繁报错上报url:XXXXXXXX,请关闭此项或配置代理\n    proxy_on = false                #是否启用代理\n    proxy = http://localhost:7890   #代理地址，如果上面选项开启，这边替换为你本地的\n    ocr_on = true                   #是否开启ocr(识图指令)\n    ocr_offline = false             #是否只使用hash验证，即设置为true后只能识别服务器已记录的图片，如果群较多(>300)导致响应延迟较高可以开启\n    ocr_url = http://mc.youthnp.cn:23338/OCR/           #默认ocr地址，一般不用动\n    http2 = true                    #是否开启http2，默认开启，如果有问题请设置为false\n    ```\n    >一般来说该文件为.env.dev\n    >也有可能是.env.pord，具体需要看.env中是否有指定\n4.   重启bot\n\n## 更新\n实验性更新指令：`wws 更新Hikari`\n请确保在能登录上服务器的情况下使用\n以下是旧更新方法\n1. 按不同版本\n   - Windows一键包：下载最新一键包，复制旧版本中`accounts`文件夹和`env.prod`文件替换至新版文件夹中即可\n   - 完整版：以管理员身份运行`更新.bat`或执行`./manage.sh update`\n      >等效于在cmd中执行如下代码\n      ```\n      pip install --upgrade hikari-bot\n      git pull\n      ```\n   - 插件版：在cmd中执行如下代码\n      ```\n      pip install --upgrade hikari-bot\n      ```\n2. **对比`.env.prod-example`中新增的配置项，并同步至你本地的`env.prod`**\n    - install结束后会打印当前版本\n    - 您也可以通过`pip show hikari-bot`查看当前Hikari版本\n    - 如果没有更新到最新版请等待一会儿，镜像站一般每五分钟同步\n    - 从0.3.2.2版本开始，您没有填写的配置将按.env文件中的默认配置执行，具体逻辑为\n      - 私聊、频道默认禁用\n      - 群聊默认开启，默认屏蔽官方交流群\n\n## 最近的更新日志\n\n### 23-05-07    v0.3.9\n- [+]重构代码\n- [#]替换默认OCR接口\n\n### 23-04-07    v0.3.8\n- [+]新增国服封号记录查询，指令wws ban/wws 封号记录\n- [#]修复了上次修复排行榜新产生的bug\n\n### 23-04-04    v0.3.7\n- [+]添加获取随机表情包，指令wws 随机表情包\n- [+]更新船只选择界面\n- [#]更新Linux脚本托管\n\n### 23-02-22    v0.3.6.4\n- [+]添加随机嘴臭，概率千分之一\n- [+]添加ocr启动报错提示\n- [#]修复一键包及Docker依赖问题 [@94Bo](https://github.com/94Bo) [@12hydrogen](https://github.com/12hydrogen)\n\n### 22-11-18    v0.3.6  包含配置项更新，请添加`env.prod-example`中新增的配置\n- [+]新增噗噗（已于0.3.5.2实装）\n- [+]新增OCR（已于0.3.5.5实装）\n- [+]新增扫雪统计和圣诞船池检查\n- [+]新增国服排行榜\n- [#]大幅优化高峰期响应速度（已于0.3.5.3实装）\n- [#]Linux下支持微软雅黑(已热更新)\n\n### 22-10-29    v0.3.5.5  添加测试功能OCR，支持图片指令\n### 22-10-27    v0.3.5.4  修复一键更新指令bug\n### 22-10-26    v0.3.5.3  添加缓存上报机制，修复噗噗误触发的bug\n### 22-10-25    v0.3.5.2  新增噗噗\n### 22-07-24    v0.3.5  适配nontbo2 v2.0.0rc1  \n### 22-07-24    v0.3.4  **配置项及入口文件更新**  请完整拉取最新仓库，并同步添加`env.prod-example`中新增的配置\n- 重要更新，完整版安装请拉取最新仓库代码，一键包请下载最新版本\n- [+]新增一键更新指令，指令wws 更新Hikari\n- [+]新增Linux一键脚本 [@94Bo](https://github.com/94Bo)\n- [#]修改部分依赖版本\n- [#]大幅改动了模板以适配后续功能\n- [#]修改框架\n- [#]修改接口url\n- [#]修复了没有完全修复的兼容性问题[#11](https://github.com/benx1n/HikariBot/issues/11)\n- [#]修改日志输出等级，现在控制台只会打印SUCCESS级以上的日志\n\n\n\n### 22-07-14    v0.3.3  积累更新\n- [+]新增群聊黑名单，默认屏蔽开发者群"\n- [+]docker添加CI/CD构建发布 [@12hydrogen](https://github.com/12hydrogen)\n- [#]修复与其他插件的兼容性问题\n- [#]更改了请求域名\n- [#]修复manage.sh会更改toml的问题\n- [#]修复了hoshino排行榜选择船只样式问题\n- [#]修复仅打过PVE的单船仍会显示战绩详情的问题\n- [#]info适配v4接口\n- [+]新增配置项ban_group_list\n\n<details>\n<summary><b>更以前的更新日志</b></summary>\n\n### 22-07-05    v0.3.2.2  一些修复\n- [#]修复切换、删除绑定的bug\n- [#]默认配置改为不启用WEB登陆验证\n- [#]修复.bat的环境变量问题 [@94Bo](https://github.com/94Bo)\n\n### 22-07-04    v0.3.2.1  **配置项及入口文件更新**  请完整拉取最新仓库，并同步添加`env.prod-example`中新增的配置\n- [+]新增对QQ频道的适配（非官方bot接入，官方版bot已上线yuyuko频道）\n- [+]新增自定义开启群聊、私聊、QQ频道\n- [+]新增web登录密码\n- [+]新增默认配置项\n- [+]新增PR彩蛋\n- [#]info适配V3接口\n- [#]recent显示时间区间\n\n### 22-06-23    v0.3.1  **重要功能更新**\n- [+]新增单船近期战绩，可显示每日详细信息，指令`wws ship recent`\n- [+]新增docker部署 [@12hydrogen](https://github.com/12hydrogen)\n- [#]修复国服特殊字符ID无法查询的bug\n- [#]修复船只选择过期后发送数字序号仍被识别的bug\n\n### 22-06-15    v0.3.0.1  **重要功能更新**\n- [+]支持显示军团评级颜色\n- [#]排行榜内部逻辑改动，现在仅显示前十，不更新将无法使用\n- [#]\\(hotfix)`wws recent`现在无随机战绩不会显示PR和上方战斗信息\n\n### 22-06-08    v0.2.9.4  **重要功能更新**\n- [+]新增单船的服务器排行，显示在`wws ship`的详情页面下\n- [#]修复0.2.9后无法启动的bug\n- [#]js依赖改为本地\n- [#]修改recent样式，不更新可能会导致错位\n- [#]优化报错提示\n\n### 22-06-03    v0.2.8  一些修复\n- [+]新增删除绑定功能\n- [#]修复`wws ship`总览经验和胜率不上色的bug\n- [#]修复`wws ship`详情只有单野场均被上色的bug\n- [#]修复`wws 查船名`中搜不到德国船的bug\n\n### 22-06-03    v0.2.6  [#]修复`wws recent`胜率颜色的bug\n\n### 22-06-03    v0.2.5  [#]修复`wws recent`击杀显示成命中的bug\n\n### 22-06-03    v0.2.4  **重要功能更新** 否则您将无法使用`wws recent`功能\n- [+]全指令在游戏名外带上括号即可强制指定昵称，以适配一些带有空格、特殊字符、指令字符的昵称\n- [+]新增特殊绑定，请配合网页端食用，复制后发送给Hikari即可一键绑定\n- [+]新增部分报错提示\n- [#]更改ship,rank,recent样式，现在没有战斗场次的类型不会被显示\n- [#]优化Hikari的部署流程\n- [#]修复me大写不被识别的问题\n\n\n### 22-06-02    v0.2.3  一些修复\n- [+]全指令支持大写\n- [#]修复Linux上可能出现的报错\n- [#]修改部分图片的样式\n\n### 22-06-01    v0.2.2  修复了一个VSC导致的依赖错误\n\n### 22-06-01    v0.2.1  修复问题\n\n### 22-06-01    v0.2.0  **重要功能更新**\n- [+]新增排位数据\n- [+]支持国服\n- [+]单船战绩显示单野、自行车、三轮车\n- [+]启用gzip，试图改善请求Timeout\n- [+]增加3s指令CD和每日100次上限\n- [#]修复图片内字符不对称的bug（强迫症）\n- [#]修改未绑定账号时的返回\n- [#]修复网络问题与找不到游戏名时相同返回的bug\n- [#]适配HarukaBot\n\n\n### 22-05-31    v0.1.9  一些修复\n- [#]解决由于QQ风控导致的船只选择列表无法发送的问题\n- [#]修复带非me/@参数查询绑定时引起的报错\n\n### 22-05-30    v0.1.8  **重要更新**\n- [+]所有带请求参数的部分添加log输出以方便查找问题\n- [+]添加平台报错时返回以和Hikari内部错误区分\n- [#]移除bat脚本中的utf8以支持部分英文服务器\n- [#]试图减少因网络导致的报错问题\n\n### 22-05-30    v0.1.7  一些修复\n- [#]修复排行榜查询报错\n- [#]修复部分环境可能出现的单船查询无法选择问题\n\n### 22-05-28    v0.1.6  **重要功能更新**\n- [+]新增排行榜查询 指令`wws rank/ship.rank`\n- [+]新增是否开启内置go-cqhttp，默认开启\n\n### 22-05-28    v0.1.5  一些功能更新\n- [+]添加等级显示，适配新舰船数据\n- [+]新增wws 检查更新\n- [+]配置项添加Bot管理员\n- [#]修复定时任务不触发的bug\n\n### 22-05-27    v0.1.4  一些功能优化\n- [+]添加在windows下的一键安装、更新、启动脚本\n- [#]修复数字ID的recent匹配问题\n- [#]优化提示逻辑\n\n### 22-05-27    v0.1.3  一些修复和适配\n- [+]适配包括真寻等大部分Nonebot2机器人\n- [#]修复自动更新的bug\n\n### 22-05-27    v0.1.2  **调整info接口，不更新无法使用**\n\n### 22-05-27    v0.1.1  一些小改动\n\n### 22-05-27    v0.1.0  一些更新\n- [+]新增定时检查更新\n- [+]新增部署教程\n- [+]添加11级战绩信息\n- [#]优化账号总体和单船图片样式\n\n</details>\n\n## 可能会遇到的问题\n\n### go-cqhttp扫码后提示异地无法登录\n- 一般提示需要扫码，扫码后提示异地无法登录\n- 关于该问题，您可以查看[这里](https://github.com/Mrs4s/go-cqhttp/issues/1469)获得相应解决办法，这里简单列举三种办法\n  - 启动时登录方式选择`浏览器滑条`，按后续提示登录\n  - 手机下载`爱加速`等代理，连接到服务器对应市级地区\n  - 在本地电脑使用go-cqhttp登录成功后，将会在exe同级目录下生成`session.token`和`device.json`两个文件\n  将这两个文件复制到服务器对应目录下并重启\n    - 内嵌go-cqhttp为`account\\QQ号`\n    - 独立go-cqhttp为exe所在同级目录下，请注意使用独立go-cqhttp时需要将`.env.prod`的`USE_PLUGIN_GO_CQHTTP`的值改为`false`\n\n### 无法使用内嵌go-cqhttp登录bot\n\n1. 下载 go-cqhttp 至合适的文件夹\n\n    - github 发布页：https://github.com/Mrs4s/go-cqhttp/releases/latest\n\n    > 您需要根据自己的机器架构选择版本，Windows一般为x86/64架构，通常选择[go-cqhttp_windows_amd64.exe](https://github.com/Mrs4s/go-cqhttp/releases/latest/download/go-cqhttp_windows_amd64.exe)\n\n2. 双击go-cqhttp，提示释出bat，重新运行bat，选择websocket反向代理，go-cqhttp将会在同文件夹内自动创建一个`config.yml`，右键使用notepad++打开，根据注释填写QQ账号密码，并将以下内容写入文件结尾（需替换原有的ws-reverse节点）：\n\n    ```yaml\n      - ws-reverse:\n          universal: ws://127.0.0.1:8080/onebot/v11/ws\n          reconnect-interval: 5000\n          middlewares:\n            <<: *default\n    ```\n\n    > 关于go-cqhttp的配置，你可以在[这里](https://docs.go-cqhttp.org/guide/config.html#%E9%85%8D%E7%BD%AE%E4%BF%A1%E6%81%AF)找到更多说明。\n\n3. 启动go-cqhttp，按照提示登录。\n\n    > 此处如出现异地登陆保护，请尝试\n    > - 在本地电脑使用go-cqhttp登录成功后，将会在exe同级目录下生成`session.token`和`device.json`两个文件\n    > - 将这两个文件复制到服务器对应go-cqhttp目录下并重启\n\n4. 修改Hikari文件夹下.env.prod中`USE_PLUGIN_GO_CQHTTP`的值为`false`\n    ```\n    USE_PLUGIN_GO_CQHTTP = false\n    ```\n5. 在文件夹下打开终端，输入`python bot.py`启动bot\n    - 一键包双击`启动.bat`即可\n\n\n### 出现ZoneInfoNotFoundError报错\n>\n>您可以在[这里](https://github.com/nonebot/nonebot2/issues/78)找到相关解决办法\n>\n### Recent和绑定提示\'鉴权失败\'\n1. 检查Token是否配置正确，token格式为`XXXXX:XXXXXX`\n2. 如果配置正确可能是Token失效了，请重新申请\n\n### \'Config\' Object has no attribute XXXX\n1. 检查视力，重新阅读[更新](https://github.com/benx1n/HikariBot#更新)章节\n\n### Failed to import "nonebot_plugin_guild_patch"\n以下方法任选一种\n- 更新python版本至3.9+\n- 降低Hikari版本至3.1，等待后续版本修复\n- 使用Hikari一键包，其中自带了3.10的python虚拟环境\n- 修改依赖包代码，见[这里](https://github.com/mnixry/nonebot-plugin-guild-patch/pull/6/files)\n\n### Ubuntu系统下部署字体不正常(针对一些云服务器的Ubuntu镜像，不保证成功，只是提供一个解决方案)\n  1. 执行以下命令，完善字体库并将中文设置成默认语言（部分Ubuntu可能不需要该步骤，可直接从第二步开始）\n  ```\n  sudo apt install fonts-noto  \n  sudo locale-gen zh_CN zh_CN.UTF-8  \n  sudo update-locale LC_ALL=zh_CN.UTF-8 LANG=zh_CN.UTF-8  \n  sudo fc-cache -fv\n  ```\n  \n  2. 在你的Windows电脑上打开`C:\\Windows\\fonts`文件夹，找到里面的微软雅黑字体，将其复制出来，放在任意目录，应该会得到`msyh.ttc`，`mshybd.ttc`，`msyhl.ttc`三个文件。（不会有人还用Win7吧？）\n\n  3. 进入到`/usr/share/fonts`文件夹下，创建一个文件夹命名为`msyh`，然后进入其中\n  ```\n  cd /usr/share/fonts \n  sudo mkdir msyh \n  cd msyh\n  ```\n  \n  4. 将三个字体文件上传到`msyh`文件夹中(过程中遇到的问题请自行解决)\n\n  5. 执行以下命令（此时你应该是在`msyh`文件夹下），加载字体\n  ```\n  sudo mkfontscale \n  sudo mkfontdir \n  sudo fc-cache -fv\n  ```\n  \n  6. （可选，若不正常可尝试）重启Hikari。\n\n### 首次启动时plugin-gocqhttp的startup方法报错(traceback中一般还有ssl的错误)\n\n1. 下载 go-cqhttp\n\n    - github 发布页：https://github.com/Mrs4s/go-cqhttp/releases/latest\n\n    > 您需要根据自己的机器架构选择版本，Windows一般为x86/64架构，通常选择[go-cqhttp_windows_amd64.exe](https://github.com/Mrs4s/go-cqhttp/releases/latest/download/go-cqhttp_windows_amd64.exe)\n\n2. 重命名为`go-cqhttp.*`(*为所选择版本后缀,如windowx就是go-cqhttp.exe)并放入`HikariBot\\accounts\\binary`文件夹下\n\n3. 重新启动Hikari\n\n## 贡献代码\n\n请向dev分支提交PR\n\n## 鸣谢\n\n感谢以下开发者及项目做出的贡献与支持\n\n<a href="https://github.com//benx1n/HikariBot/graphs/contributors">\n  <img src="https://contrib.rocks/image?repo=benx1n/HikariBot" />\n</a>\n\n[Nonebot2](https://github.com/nonebot/nonebot2)  \n[go-cqhttp](https://github.com/Mrs4s/go-cqhttp)  \n[战舰世界API平台](https://wows.shinoaki.com/)  \n\n## 开源相关\nMIT\n修改、分发代码时请保留原作者相关信息\n',
     'author': 'benx1n',
     'author_email': 'shirakamikanade@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/benx1n/HikariBot',
```

### Comparing `hikari_bot-0.3.9.2/PKG-INFO` & `hikari_bot-0.3.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hikari-bot
-Version: 0.3.9.2
+Version: 0.3.9.3
 Summary: Nonebot2 HikariBot,支持战舰世界水表查询
 Home-page: https://github.com/benx1n/HikariBot
 License: MIT
 Keywords: nonebot,nonebot2,qqbot,wows,wws,bot,stats
 Author: benx1n
 Author-email: shirakamikanade@gmail.com
 Requires-Python: >=3.8.0,<4.0.0
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Jinja2 (>=3.0.0,<4.0.0)
 Requires-Dist: beautifulsoup4 (>=4.11.1,<5.0.0)
-Requires-Dist: httpx[http2] (>=0.22.0)
+Requires-Dist: httpx[http2] (>=0.24.0)
 Requires-Dist: nonebot-adapter-onebot (>=2.1.0,<3.0.0)
 Requires-Dist: nonebot-plugin-apscheduler (>=0.2.0,<0.3.0)
 Requires-Dist: nonebot-plugin-htmlrender (>=0.2.0.1,<0.3.0.0)
 Requires-Dist: nonebot-plugin-reboot (>=0.1.3,<0.2.0)
 Requires-Dist: nonebot2[fastapi] (>=2.0.0-beta.1,<3.0.0)
 Requires-Dist: nonebot_plugin_guild_patch (>=0.2.1,<0.3.0)
 Requires-Dist: orjson (>=3.8.11,<4.0.0)
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1 Name: hikari-bot Version: 0.3.9.2 Summary: Nonebot2
+Metadata-Version: 2.1 Name: hikari-bot Version: 0.3.9.3 Summary: Nonebot2
 HikariBot,æ¯ææè°ä¸çæ°´è¡¨æ¥è¯¢ Home-page: https://github.com/benx1n/
 HikariBot License: MIT Keywords: nonebot,nonebot2,qqbot,wows,wws,bot,stats
 Author: benx1n Author-email: shirakamikanade@gmail.com Requires-Python:
 >=3.8.0,<4.0.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Requires-Dist: Jinja2 (>=3.0.0,<4.0.0) Requires-Dist:
-beautifulsoup4 (>=4.11.1,<5.0.0) Requires-Dist: httpx[http2] (>=0.22.0)
+beautifulsoup4 (>=4.11.1,<5.0.0) Requires-Dist: httpx[http2] (>=0.24.0)
 Requires-Dist: nonebot-adapter-onebot (>=2.1.0,<3.0.0) Requires-Dist: nonebot-
 plugin-apscheduler (>=0.2.0,<0.3.0) Requires-Dist: nonebot-plugin-htmlrender
 (>=0.2.0.1,<0.3.0.0) Requires-Dist: nonebot-plugin-reboot (>=0.1.3,<0.2.0)
 Requires-Dist: nonebot2[fastapi] (>=2.0.0-beta.1,<3.0.0) Requires-Dist:
 nonebot_plugin_guild_patch (>=0.2.1,<0.3.0) Requires-Dist: orjson
 (>=3.8.11,<4.0.0) Project-URL: Repository, https://github.com/benx1n/HikariBot
 Description-Content-Type: text/markdown
```

