# Comparing `tmp/nonebot-plugin-csgo-case-simulator-0.1.7.tar.gz` & `tmp/nonebot-plugin-csgo-case-simulator-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-csgo-case-simulator-0.1.7.tar", max compression
+gzip compressed data, was "nonebot-plugin-csgo-case-simulator-0.1.8.tar", max compression
```

## Comparing `nonebot-plugin-csgo-case-simulator-0.1.7.tar` & `nonebot-plugin-csgo-case-simulator-0.1.8.tar`

### file list

```diff
@@ -1,10 +1,13 @@
--rw-r--r--   0        0        0     1062 2023-05-06 19:37:08.273216 nonebot-plugin-csgo-case-simulator-0.1.7/LICENSE
--rw-r--r--   0        0        0     3272 2023-05-07 06:37:13.253861 nonebot-plugin-csgo-case-simulator-0.1.7/nonebot-plugin-csgo-case-simulator/__init__.py
--rw-r--r--   0        0        0   274723 2023-05-06 19:37:08.274212 nonebot-plugin-csgo-case-simulator-0.1.7/nonebot-plugin-csgo-case-simulator/background2.png
--rw-r--r--   0        0        0     2442 2023-05-06 19:37:08.274307 nonebot-plugin-csgo-case-simulator-0.1.7/nonebot-plugin-csgo-case-simulator/cases.py
--rw-r--r--   0        0        0  3886748 2023-05-07 01:22:58.975435 nonebot-plugin-csgo-case-simulator-0.1.7/nonebot-plugin-csgo-case-simulator/font/font.ttf
--rw-r--r--   0        0        0     1846 2023-05-06 19:37:08.274385 nonebot-plugin-csgo-case-simulator-0.1.7/nonebot-plugin-csgo-case-simulator/skins.py
--rw-r--r--   0        0        0     3957 2023-05-07 06:33:57.219273 nonebot-plugin-csgo-case-simulator-0.1.7/nonebot-plugin-csgo-case-simulator/utils.py
--rw-r--r--   0        0        0      516 2023-05-07 06:34:57.066286 nonebot-plugin-csgo-case-simulator-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      818 2023-05-07 06:39:19.805570 nonebot-plugin-csgo-case-simulator-0.1.7/setup.py
--rw-r--r--   0        0        0      546 2023-05-07 06:39:19.805689 nonebot-plugin-csgo-case-simulator-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-05-06 19:37:08.273216 nonebot-plugin-csgo-case-simulator-0.1.8/LICENSE
+-rw-r--r--   0        0        0     4537 2023-05-08 01:58:39.508153 nonebot-plugin-csgo-case-simulator-0.1.8/nonebot-plugin-csgo-case-simulator/__init__.py
+-rw-r--r--   0        0        0    14492 2023-05-08 01:42:00.277080 nonebot-plugin-csgo-case-simulator-0.1.8/nonebot-plugin-csgo-case-simulator/background3.jpeg
+-rw-r--r--   0        0        0     5327 2023-05-08 01:55:42.619431 nonebot-plugin-csgo-case-simulator-0.1.8/nonebot-plugin-csgo-case-simulator/crates.py
+-rw-r--r--   0        0        0  3886748 2023-05-07 01:22:58.975435 nonebot-plugin-csgo-case-simulator-0.1.8/nonebot-plugin-csgo-case-simulator/font/font.ttf
+-rw-r--r--   0        0        0   367810 2023-05-07 23:51:29.826342 nonebot-plugin-csgo-case-simulator-0.1.8/nonebot-plugin-csgo-case-simulator/json/cases.json
+-rw-r--r--   0        0        0  1027515 2023-05-07 23:51:29.814018 nonebot-plugin-csgo-case-simulator-0.1.8/nonebot-plugin-csgo-case-simulator/json/skins.json
+-rw-r--r--   0        0        0   321996 2023-05-07 23:51:29.834274 nonebot-plugin-csgo-case-simulator-0.1.8/nonebot-plugin-csgo-case-simulator/json/souvenir.json
+-rw-r--r--   0        0        0     1955 2023-05-08 01:55:47.310489 nonebot-plugin-csgo-case-simulator-0.1.8/nonebot-plugin-csgo-case-simulator/skins.py
+-rw-r--r--   0        0        0     3994 2023-05-08 01:40:15.727005 nonebot-plugin-csgo-case-simulator-0.1.8/nonebot-plugin-csgo-case-simulator/utils.py
+-rw-r--r--   0        0        0      516 2023-05-08 01:54:47.051876 nonebot-plugin-csgo-case-simulator-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      828 2023-05-08 02:00:34.639507 nonebot-plugin-csgo-case-simulator-0.1.8/setup.py
+-rw-r--r--   0        0        0      546 2023-05-08 02:00:34.639640 nonebot-plugin-csgo-case-simulator-0.1.8/PKG-INFO
```

### Comparing `nonebot-plugin-csgo-case-simulator-0.1.7/LICENSE` & `nonebot-plugin-csgo-case-simulator-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-csgo-case-simulator-0.1.7/nonebot-plugin-csgo-case-simulator/__init__.py` & `nonebot-plugin-csgo-case-simulator-0.1.8/nonebot-plugin-csgo-case-simulator/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,90 +1,118 @@
 import asyncio
+import time
 from nonebot import on_command
 from nonebot.params import CommandArg
 from nonebot.adapters.onebot.v11 import Message, MessageSegment, MessageEvent
-from .cases import Cases
+from .crates import Crates
 from .skins import Skins
 from .utils import Utils
 
-cases = Cases()
+crates = Crates()
 skins = Skins()
 utils = Utils()
 
 
 async def get_all_json():
-    res = await asyncio.gather(cases.get_cases_json(), skins.get_skins_json())
-    cases.cases = res[0].json()
-    skins.skins = res[1].json()
+    res = await asyncio.gather(
+        crates.get_cases_json(),
+        crates.get_souvenirs_json(),
+        skins.get_skins_json(),
+    )
+    crates.cases = res[0]
+    crates.souvenirs = res[1]
+    skins.skins = res[2]
 
 asyncio.run(get_all_json())
 
 rarities = {
     "工业级": 1,
     "军规级": 2,
     "受限": 3,
     "保密": 4,
     "隐秘": 5,
     "非凡": 6,
 }
 
 rarities_reverse = {value: key for key, value in rarities.items()}
 
-case_opening = on_command("open", priority=5)
+crate_opening = on_command("open", priority=5)
 list_cases = on_command("cases", priority=5)
-# radom_case = on_command("random", priority=5)
+list_souvenir = on_command("svs", priority=5)
 search_skin = on_command("s_skin", priority=5)
+help = on_command("help", priority=5)
 
 
 @list_cases.handle()
 async def handle_list_cases():
-    cases_list = cases.get_case_name_list()
+    cases_list = crates.get_case_name_list()
     cases_list_str = ""
     for case in cases_list:
         cases_list_str += f"{case}\n"
     await list_cases.finish(f"{cases_list_str}")
 
 
+@list_souvenir.handle()
+async def handle_list_souvenir():
+    svs_list = crates.get_souvenir_name_list()
+    svs_list_str = ""
+    for sv in svs_list[0:len(svs_list) // 2]:
+        svs_list_str += f"{sv}\n"
+    await list_souvenir.send(f"{svs_list_str}")
+    svs_list_str = ""
+    for sv in svs_list[len(svs_list)//2:]:
+        svs_list_str += f"{sv}\n"
+    await list_souvenir.finish(f"{svs_list_str}")
+
+
+@help.handle()
+async def handle_help():
+    await help.finish(
+        """
+    开箱指令：    
+    /open [数量] [箱子名] 开箱    
+    /cases 查看所有箱子    
+    /svs 查看所有纪念包    
+    /s_skin [皮肤名] 搜索皮肤    
+    /help 查看帮助    
+    """
+    )
+
 # @radom_case.handle()
 # async def handle_random_case():
 #     case = cases.get_random_case()
 #     await radom_case.send(f"正在开启{case['name']}...")
 #     item = cases.open_case(case["id"])
 #     skin = skins.get_skins(item["id"])
 #     await radom_case.finish(get_skink_message(skin))
 
 
-@case_opening.handle()
-async def handle_open_case(event: MessageEvent, args: Message = CommandArg()):
-    arg_list = args.extract_plain_text().split(" ")
-    if len(arg_list) > 0:
-        if len(arg_list) == 2:
-            arg_amount = int(arg_list[0])
-            amount = arg_amount if arg_amount < 20 else 20
-            case_name = arg_list[1]
-        else:
-            amount = 1
-            case_name = arg_list[0]
-
-        case = cases.get_case_by_name(case_name)
-        if case:
-            img_base64 = await utils.url_to_b64(case["image"])
-            await case_opening.send(MessageSegment.image(img_base64)+f"正在开启{case['name']}...")
-            items = cases.open_case_multiple(case["id"], amount)
+@crate_opening.handle()
+async def handle_open_crate(event: MessageEvent, args: Message = CommandArg()):
+    (amount, name) = extract_args(args)
+    if name:
+        crate = get_crate(name)
+        if crate:
+            if not crate["contains"]:
+                await crate_opening.finish("箱子里面是空的")
+            img_base64 = await utils.url_to_b64(crate["image"])
+            await crate_opening.send(MessageSegment.image(img_base64)+f"正在开启{amount}个{crate['name']}...")
+            items = crates.open_crate_multiple(
+                crate, amount
+            )
             opened_skins = []
             for item in items:
                 skin = skins.get_skins(item["name"])
                 opened_skins.append(skin)
-
             image = await utils.merge_images(opened_skins)
-            await case_opening.finish(MessageSegment.image(image))
+            await crate_opening.finish(MessageSegment.image(image))
         else:
-            await case_opening.finish("箱子不存在")
+            await crate_opening.finish("箱子不存在")
     else:
-        await case_opening.finish("请输入箱子名称")
+        await crate_opening.finish("请输入箱子名称")
 
 
 @search_skin.handle()
 async def handle_search_skin(args: Message = CommandArg()):
     if skin_name := args.extract_plain_text().strip():
         found_skin_list = skins.search_skin(skin_name)
         if len(found_skin_list) == 0:
@@ -92,10 +120,29 @@
         for skin in found_skin_list:
             img_base64 = await utils.url_to_b64(skin["image"])
             await search_skin.send(MessageSegment.image(img_base64)+f"找到饰品{skin['name']}")
     else:
         await search_skin.finish("请输入皮肤名称")
 
 
+def extract_args(args: Message = CommandArg()):
+    arg_list = args.extract_plain_text().split(" ")
+    if len(arg_list) > 0 and arg_list[0] != "":
+        if len(arg_list) == 2:
+            arg_amount = int(arg_list[0])
+            amount = arg_amount if arg_amount < 20 else 20
+            crate_name = arg_list[1]
+        else:
+            amount = 1
+            crate_name = arg_list[0]
+        return amount, crate_name
+    else:
+        return 1, None
+
+
+def get_crate(name: str):
+    return crates.get_case_by_name(name) or crates.get_souvenir_by_name(name)
+
+
 def get_skink_message(skin: dict):
     return (MessageSegment.image(skin["image"]) +
             f"""获得 {skin['rarity']}\n{skin['name']}\n磨损度{skin['wear_rating']}""")
```

### Comparing `nonebot-plugin-csgo-case-simulator-0.1.7/nonebot-plugin-csgo-case-simulator/font/font.ttf` & `nonebot-plugin-csgo-case-simulator-0.1.8/nonebot-plugin-csgo-case-simulator/font/font.ttf`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-csgo-case-simulator-0.1.7/nonebot-plugin-csgo-case-simulator/skins.py` & `nonebot-plugin-csgo-case-simulator-0.1.8/nonebot-plugin-csgo-case-simulator/skins.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,25 @@
+import json
 import random
-import httpx
+from os.path import dirname
+
+
+JSON_DIR = dirname(__file__) + "/json"
 
 
 class Skins:
     def __init__(self):
-        self.skins_api = "https://bymykel.github.io/CSGO-API/api/zh-CN/skins.json"
         self.skins = []
 
     async def get_skins_json(self):
-        async with httpx.AsyncClient() as client:
-            return await client.get(self.skins_api)
+        # async with httpx.AsyncClient() as client:
+        #     return await client.get(self.skins_api)
+        with open(f"{JSON_DIR}/skins.json", 'rb') as f:
+            data = f.read()
+            return json.loads(data)
 
     def get_skins(self, name: str) -> dict:
         # print(name)
         for skin in self.skins:
             if skin["name"] == name:
                 wear_rating = round(
                     random.uniform(skin["min_float"], skin["max_float"]), 5
```

### Comparing `nonebot-plugin-csgo-case-simulator-0.1.7/nonebot-plugin-csgo-case-simulator/utils.py` & `nonebot-plugin-csgo-case-simulator-0.1.8/nonebot-plugin-csgo-case-simulator/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 FONT_DIR = dirname(__file__) + "/font/font.ttf"
 
 
 class Utils:
     def __init__(self):
         self.client = httpx.Client()
         self.rarity_color = {
+            "消费级": (130, 130, 130),
             "工业级": (96, 152, 217),
             "军规级": (76, 105, 255),
             "受限": (136, 70, 255),
             "保密": (177, 46, 194),
             "隐秘": (235, 75, 75),
             "及其罕见的特殊物品": (201, 171, 5),
             "非凡": (201, 171, 5),
@@ -36,18 +37,18 @@
         height = image_list[0].height
         number = len(items)
         rows = math.ceil(number / 5)
         columns = number if number < 5 else 5
         padding = 200
         info_height = 200
         bg_color = (255, 255, 255)
-        font_color = (255, 255, 255)
+        font_color = (0, 0, 0)
 
         path = os.path.dirname(os.path.abspath(__file__))
-        bg_file = os.path.join(path, "background2.png")
+        bg_file = os.path.join(path, "background3.jpeg")
         background_img = Image.open(bg_file)
         background_img = background_img.filter(
             ImageFilter.GaussianBlur(radius=50))
         background_img = background_img.resize((width * columns + padding,
                                                 (height + info_height) * rows + padding))
 
         canvas = background_img
@@ -110,13 +111,13 @@
             return img
 
     def img_to_b64(self, pic: Image.Image) -> str:
         buf = BytesIO()
         pic.save(buf, format="PNG")
         base64_str = base64.b64encode(buf.getbuffer()).decode()
         return "base64://" + base64_str
-    
-    async def url_to_b64(self,url:str)->str:
+
+    async def url_to_b64(self, url: str) -> str:
         async with httpx.AsyncClient() as client:
             response = await client.get(url)
             base64_str = base64.b64encode(response.content).decode()
             return "base64://" + base64_str
```

### Comparing `nonebot-plugin-csgo-case-simulator-0.1.7/pyproject.toml` & `nonebot-plugin-csgo-case-simulator-0.1.8/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-csgo-case-simulator"
-version = "0.1.7"
+version = "0.1.8"
 description = "a nonebot based csgo case simulator"
 authors = ["Roy <lyt2980999208@gmail.com>"]
 license = "MIT"
 packages = [{ include = "nonebot-plugin-csgo-case-simulator" }]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `nonebot-plugin-csgo-case-simulator-0.1.7/setup.py` & `nonebot-plugin-csgo-case-simulator-0.1.8/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
 ['nonebot-plugin-csgo-case-simulator']
 
 package_data = \
-{'': ['*'], 'nonebot-plugin-csgo-case-simulator': ['font/*']}
+{'': ['*'], 'nonebot-plugin-csgo-case-simulator': ['font/*', 'json/*']}
 
 install_requires = \
 ['Pillow>=9.5.0,<10.0.0',
  'httpx>=0.24.0,<0.25.0',
  'nonebot-adapter-onebot>=2.2.3,<3.0.0',
  'nonebot2>=2.0.0-rc.4,<3.0.0']
 
 setup_kwargs = {
     'name': 'nonebot-plugin-csgo-case-simulator',
-    'version': '0.1.7',
+    'version': '0.1.8',
     'description': 'a nonebot based csgo case simulator',
     'long_description': None,
     'author': 'Roy',
     'author_email': 'lyt2980999208@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `nonebot-plugin-csgo-case-simulator-0.1.7/PKG-INFO` & `nonebot-plugin-csgo-case-simulator-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-csgo-case-simulator
-Version: 0.1.7
+Version: 0.1.8
 Summary: a nonebot based csgo case simulator
 License: MIT
 Author: Roy
 Author-email: lyt2980999208@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

