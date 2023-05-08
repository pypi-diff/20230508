# Comparing `tmp/nonebot_plugin_penguin-0.0.2.tar.gz` & `tmp/nonebot_plugin_penguin-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_penguin-0.0.2.tar", max compression
+gzip compressed data, was "nonebot_plugin_penguin-0.0.3.tar", max compression
```

## Comparing `nonebot_plugin_penguin-0.0.2.tar` & `nonebot_plugin_penguin-0.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1068 2023-05-08 08:56:19.698741 nonebot_plugin_penguin-0.0.2/LICENSE
--rw-r--r--   0        0        0     5314 2023-05-08 08:56:19.698741 nonebot_plugin_penguin-0.0.2/README.md
--rw-r--r--   0        0        0      408 2023-05-08 08:56:19.698741 nonebot_plugin_penguin-0.0.2/nonebot_plugin_penguin/__init__.py
--rw-r--r--   0        0        0     1570 2023-05-08 08:56:19.698741 nonebot_plugin_penguin-0.0.2/nonebot_plugin_penguin/config.py
--rw-r--r--   0        0        0     2507 2023-05-08 08:56:19.698741 nonebot_plugin_penguin-0.0.2/nonebot_plugin_penguin/db.py
--rw-r--r--   0        0        0       48 2023-05-08 08:56:19.698741 nonebot_plugin_penguin-0.0.2/nonebot_plugin_penguin/render/__init__.py
--rw-r--r--   0        0        0      870 2023-05-08 08:56:19.698741 nonebot_plugin_penguin-0.0.2/nonebot_plugin_penguin/render/item_sprite.py
--rw-r--r--   0        0        0     2793 2023-05-08 08:56:19.698741 nonebot_plugin_penguin-0.0.2/nonebot_plugin_penguin/render/table.py
--rw-r--r--   0        0        0      970 2023-05-08 08:56:19.698741 nonebot_plugin_penguin-0.0.2/nonebot_plugin_penguin/render/templates/app.css
--rw-r--r--   0        0        0     3309 2023-05-08 08:56:19.698741 nonebot_plugin_penguin-0.0.2/nonebot_plugin_penguin/render/templates/card.css
--rw-r--r--   0        0        0     2731 2023-05-08 08:56:19.698741 nonebot_plugin_penguin-0.0.2/nonebot_plugin_penguin/render/templates/item_card.html
--rw-r--r--   0        0        0  1171678 2023-05-08 08:56:19.698741 nonebot_plugin_penguin-0.0.2/nonebot_plugin_penguin/render/templates/sprite.202210111514.png
--rw-r--r--   0        0        0     2774 2023-05-08 08:56:19.698741 nonebot_plugin_penguin-0.0.2/nonebot_plugin_penguin/render/templates/stage_card.html
--rw-r--r--   0        0        0      197 2023-05-08 08:56:19.698741 nonebot_plugin_penguin-0.0.2/nonebot_plugin_penguin/render/utils.py
--rw-r--r--   0        0        0     5457 2023-05-08 08:56:19.698741 nonebot_plugin_penguin-0.0.2/nonebot_plugin_penguin/request.py
--rw-r--r--   0        0        0      318 2023-05-08 08:56:19.698741 nonebot_plugin_penguin-0.0.2/nonebot_plugin_penguin/schedule.py
--rw-r--r--   0        0        0      353 2023-05-08 08:56:19.698741 nonebot_plugin_penguin-0.0.2/nonebot_plugin_penguin/startup.py
--rw-r--r--   0        0        0     1291 2023-05-08 08:56:19.698741 nonebot_plugin_penguin-0.0.2/nonebot_plugin_penguin/trim.py
--rw-r--r--   0        0        0     2628 2023-05-08 08:56:19.698741 nonebot_plugin_penguin-0.0.2/nonebot_plugin_penguin/types.py
--rw-r--r--   0        0        0    10980 2023-05-08 08:56:19.702741 nonebot_plugin_penguin-0.0.2/nonebot_plugin_penguin/user.py
--rw-r--r--   0        0        0     2071 2023-05-08 08:56:19.702741 nonebot_plugin_penguin-0.0.2/nonebot_plugin_penguin/utils.py
--rw-r--r--   0        0        0     1832 2023-05-08 08:56:19.702741 nonebot_plugin_penguin-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     6540 1970-01-01 00:00:00.000000 nonebot_plugin_penguin-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-05-08 14:53:00.916845 nonebot_plugin_penguin-0.0.3/LICENSE
+-rw-r--r--   0        0        0     5314 2023-05-08 14:53:00.916845 nonebot_plugin_penguin-0.0.3/README.md
+-rw-r--r--   0        0        0      406 2023-05-08 14:53:00.916845 nonebot_plugin_penguin-0.0.3/nonebot_plugin_penguin/__init__.py
+-rw-r--r--   0        0        0     1570 2023-05-08 14:53:00.916845 nonebot_plugin_penguin-0.0.3/nonebot_plugin_penguin/config.py
+-rw-r--r--   0        0        0     2507 2023-05-08 14:53:00.916845 nonebot_plugin_penguin-0.0.3/nonebot_plugin_penguin/db.py
+-rw-r--r--   0        0        0       48 2023-05-08 14:53:00.916845 nonebot_plugin_penguin-0.0.3/nonebot_plugin_penguin/render/__init__.py
+-rw-r--r--   0        0        0      870 2023-05-08 14:53:00.916845 nonebot_plugin_penguin-0.0.3/nonebot_plugin_penguin/render/item_sprite.py
+-rw-r--r--   0        0        0     2793 2023-05-08 14:53:00.916845 nonebot_plugin_penguin-0.0.3/nonebot_plugin_penguin/render/table.py
+-rw-r--r--   0        0        0      970 2023-05-08 14:53:00.916845 nonebot_plugin_penguin-0.0.3/nonebot_plugin_penguin/render/templates/app.css
+-rw-r--r--   0        0        0     3309 2023-05-08 14:53:00.916845 nonebot_plugin_penguin-0.0.3/nonebot_plugin_penguin/render/templates/card.css
+-rw-r--r--   0        0        0     2731 2023-05-08 14:53:00.916845 nonebot_plugin_penguin-0.0.3/nonebot_plugin_penguin/render/templates/item_card.html
+-rw-r--r--   0        0        0  1171678 2023-05-08 14:53:00.916845 nonebot_plugin_penguin-0.0.3/nonebot_plugin_penguin/render/templates/sprite.202210111514.png
+-rw-r--r--   0        0        0     2774 2023-05-08 14:53:00.916845 nonebot_plugin_penguin-0.0.3/nonebot_plugin_penguin/render/templates/stage_card.html
+-rw-r--r--   0        0        0      197 2023-05-08 14:53:00.916845 nonebot_plugin_penguin-0.0.3/nonebot_plugin_penguin/render/utils.py
+-rw-r--r--   0        0        0     5457 2023-05-08 14:53:00.920845 nonebot_plugin_penguin-0.0.3/nonebot_plugin_penguin/request.py
+-rw-r--r--   0        0        0      318 2023-05-08 14:53:00.920845 nonebot_plugin_penguin-0.0.3/nonebot_plugin_penguin/schedule.py
+-rw-r--r--   0        0        0      353 2023-05-08 14:53:00.920845 nonebot_plugin_penguin-0.0.3/nonebot_plugin_penguin/startup.py
+-rw-r--r--   0        0        0     1291 2023-05-08 14:53:00.920845 nonebot_plugin_penguin-0.0.3/nonebot_plugin_penguin/trim.py
+-rw-r--r--   0        0        0     2628 2023-05-08 14:53:00.920845 nonebot_plugin_penguin-0.0.3/nonebot_plugin_penguin/types.py
+-rw-r--r--   0        0        0    10980 2023-05-08 14:53:00.920845 nonebot_plugin_penguin-0.0.3/nonebot_plugin_penguin/user.py
+-rw-r--r--   0        0        0     2071 2023-05-08 14:53:00.920845 nonebot_plugin_penguin-0.0.3/nonebot_plugin_penguin/utils.py
+-rw-r--r--   0        0        0     1878 2023-05-08 14:53:00.920845 nonebot_plugin_penguin-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     6540 1970-01-01 00:00:00.000000 nonebot_plugin_penguin-0.0.3/PKG-INFO
```

### Comparing `nonebot_plugin_penguin-0.0.2/LICENSE` & `nonebot_plugin_penguin-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_penguin-0.0.2/README.md` & `nonebot_plugin_penguin-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_penguin-0.0.2/nonebot_plugin_penguin/config.py` & `nonebot_plugin_penguin-0.0.3/nonebot_plugin_penguin/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_penguin-0.0.2/nonebot_plugin_penguin/db.py` & `nonebot_plugin_penguin-0.0.3/nonebot_plugin_penguin/db.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_penguin-0.0.2/nonebot_plugin_penguin/render/item_sprite.py` & `nonebot_plugin_penguin-0.0.3/nonebot_plugin_penguin/render/item_sprite.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_penguin-0.0.2/nonebot_plugin_penguin/render/table.py` & `nonebot_plugin_penguin-0.0.3/nonebot_plugin_penguin/render/table.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_penguin-0.0.2/nonebot_plugin_penguin/render/templates/app.css` & `nonebot_plugin_penguin-0.0.3/nonebot_plugin_penguin/render/templates/app.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_penguin-0.0.2/nonebot_plugin_penguin/render/templates/card.css` & `nonebot_plugin_penguin-0.0.3/nonebot_plugin_penguin/render/templates/card.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_penguin-0.0.2/nonebot_plugin_penguin/render/templates/item_card.html` & `nonebot_plugin_penguin-0.0.3/nonebot_plugin_penguin/render/templates/item_card.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_penguin-0.0.2/nonebot_plugin_penguin/render/templates/sprite.202210111514.png` & `nonebot_plugin_penguin-0.0.3/nonebot_plugin_penguin/render/templates/sprite.202210111514.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_penguin-0.0.2/nonebot_plugin_penguin/render/templates/stage_card.html` & `nonebot_plugin_penguin-0.0.3/nonebot_plugin_penguin/render/templates/stage_card.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_penguin-0.0.2/nonebot_plugin_penguin/request.py` & `nonebot_plugin_penguin-0.0.3/nonebot_plugin_penguin/request.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_penguin-0.0.2/nonebot_plugin_penguin/trim.py` & `nonebot_plugin_penguin-0.0.3/nonebot_plugin_penguin/trim.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_penguin-0.0.2/nonebot_plugin_penguin/types.py` & `nonebot_plugin_penguin-0.0.3/nonebot_plugin_penguin/types.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_penguin-0.0.2/nonebot_plugin_penguin/user.py` & `nonebot_plugin_penguin-0.0.3/nonebot_plugin_penguin/user.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_penguin-0.0.2/nonebot_plugin_penguin/utils.py` & `nonebot_plugin_penguin-0.0.3/nonebot_plugin_penguin/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_penguin-0.0.2/pyproject.toml` & `nonebot_plugin_penguin-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-penguin"
-version = "0.0.2"
+version = "0.0.3"
 description = "get penguin data and send from https://penguin-stats.io/"
 authors = ["Azide <rukuy@qq.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "nonebot_plugin_penguin" }]
 homepage = "https://github.com/AzideCupric/nonebot-plugin-penguin"
 repository = "https://github.com/AzideCupric/nonebot-plugin-penguin"
@@ -39,15 +39,15 @@
 pytest-asyncio = "^0.21.0"
 pytest-cov = "^4.0.0"
 respx = "^0.20.1"
 fastapi = "^0.95.0"
 flaky = "^3.7.0"
 pytest-xdist = {extras = ["psutil"], version = "^3.2.1"}
 freezegun = "^1.2.2"
-nonebug-saa = "^0.1.0"
+nonebug-saa = {git = "https://github.com/felinae98/nonebug-saa.git"}
 
 [tool.black]
 line-length = 88
 include = '\.pyi?$'
 extend-exclude = '''
 '''
```

### Comparing `nonebot_plugin_penguin-0.0.2/PKG-INFO` & `nonebot_plugin_penguin-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-penguin
-Version: 0.0.2
+Version: 0.0.3
 Summary: get penguin data and send from https://penguin-stats.io/
 Home-page: https://github.com/AzideCupric/nonebot-plugin-penguin
 License: MIT
 Author: Azide
 Author-email: rukuy@qq.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-penguin Version: 0.0.2 Summary: get
+Metadata-Version: 2.1 Name: nonebot-plugin-penguin Version: 0.0.3 Summary: get
 penguin data and send from https://penguin-stats.io/ Home-page: https://
 github.com/AzideCupric/nonebot-plugin-penguin License: MIT Author: Azide
 Author-email: rukuy@qq.com Requires-Python: >=3.10,<4.0 Classifier: Development
 Status :: 3 - Alpha Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows Classifier: Operating
 System :: POSIX :: Linux Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
```

