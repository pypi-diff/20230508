# Comparing `tmp/nonebot_plugin_penguin-0.0.1.tar.gz` & `tmp/nonebot_plugin_penguin-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_penguin-0.0.1.tar", max compression
+gzip compressed data, was "nonebot_plugin_penguin-0.0.2.tar", max compression
```

## Comparing `nonebot_plugin_penguin-0.0.1.tar` & `nonebot_plugin_penguin-0.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1089 2023-04-09 13:49:06.301876 nonebot_plugin_penguin-0.0.1/LICENSE
--rw-r--r--   0        0        0      332 2023-04-19 16:02:11.715422 nonebot_plugin_penguin-0.0.1/nonebot_plugin_penguin/__init__.py
--rw-r--r--   0        0        0     1613 2023-04-19 16:02:11.719438 nonebot_plugin_penguin-0.0.1/nonebot_plugin_penguin/config.py
--rw-r--r--   0        0        0     2560 2023-04-19 16:02:15.755827 nonebot_plugin_penguin-0.0.1/nonebot_plugin_penguin/db.py
--rw-r--r--   0        0        0       51 2023-04-19 15:55:17.503212 nonebot_plugin_penguin-0.0.1/nonebot_plugin_penguin/render/__init__.py
--rw-r--r--   0        0        0      896 2023-04-19 15:52:23.316962 nonebot_plugin_penguin-0.0.1/nonebot_plugin_penguin/render/item_sprite.py
--rw-r--r--   0        0        0     2881 2023-04-19 16:01:32.997194 nonebot_plugin_penguin-0.0.1/nonebot_plugin_penguin/render/table.py
--rw-r--r--   0        0        0     1014 2023-04-19 15:51:25.784473 nonebot_plugin_penguin-0.0.1/nonebot_plugin_penguin/render/templates/app.css
--rw-r--r--   0        0        0     3475 2023-04-19 15:53:51.929107 nonebot_plugin_penguin-0.0.1/nonebot_plugin_penguin/render/templates/card.css
--rw-r--r--   0        0        0     2812 2023-04-19 15:59:53.759450 nonebot_plugin_penguin-0.0.1/nonebot_plugin_penguin/render/templates/item_card.html
--rw-r--r--   0        0        0  1171678 2023-04-15 17:24:55.363118 nonebot_plugin_penguin-0.0.1/nonebot_plugin_penguin/render/templates/sprite.202210111514.png
--rw-r--r--   0        0        0     2856 2023-04-15 17:25:06.762356 nonebot_plugin_penguin-0.0.1/nonebot_plugin_penguin/render/templates/stage_card.html
--rw-r--r--   0        0        0     5488 2023-04-19 15:57:37.347390 nonebot_plugin_penguin-0.0.1/nonebot_plugin_penguin/request.py
--rw-r--r--   0        0        0      329 2023-04-19 16:02:15.758400 nonebot_plugin_penguin-0.0.1/nonebot_plugin_penguin/schedule.py
--rw-r--r--   0        0        0      227 2023-04-19 16:02:15.761420 nonebot_plugin_penguin-0.0.1/nonebot_plugin_penguin/startup.py
--rw-r--r--   0        0        0     1333 2023-04-19 15:56:25.100587 nonebot_plugin_penguin-0.0.1/nonebot_plugin_penguin/trim.py
--rw-r--r--   0        0        0     2727 2023-04-19 16:02:23.214172 nonebot_plugin_penguin-0.0.1/nonebot_plugin_penguin/types.py
--rw-r--r--   0        0        0     5459 2023-04-19 16:02:15.763988 nonebot_plugin_penguin-0.0.1/nonebot_plugin_penguin/user.py
--rw-r--r--   0        0        0     2110 2023-04-19 16:02:11.742125 nonebot_plugin_penguin-0.0.1/nonebot_plugin_penguin/utils.py
--rw-r--r--   0        0        0     1867 2023-04-19 16:02:15.774018 nonebot_plugin_penguin-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     4961 2023-04-19 16:02:26.252459 nonebot_plugin_penguin-0.0.1/README.md
--rw-r--r--   0        0        0     6037 1970-01-01 00:00:00.000000 nonebot_plugin_penguin-0.0.1/setup.py
--rw-r--r--   0        0        0     6106 1970-01-01 00:00:00.000000 nonebot_plugin_penguin-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-05-08 08:56:19.698741 nonebot_plugin_penguin-0.0.2/LICENSE
+-rw-r--r--   0        0        0     5314 2023-05-08 08:56:19.698741 nonebot_plugin_penguin-0.0.2/README.md
+-rw-r--r--   0        0        0      408 2023-05-08 08:56:19.698741 nonebot_plugin_penguin-0.0.2/nonebot_plugin_penguin/__init__.py
+-rw-r--r--   0        0        0     1570 2023-05-08 08:56:19.698741 nonebot_plugin_penguin-0.0.2/nonebot_plugin_penguin/config.py
+-rw-r--r--   0        0        0     2507 2023-05-08 08:56:19.698741 nonebot_plugin_penguin-0.0.2/nonebot_plugin_penguin/db.py
+-rw-r--r--   0        0        0       48 2023-05-08 08:56:19.698741 nonebot_plugin_penguin-0.0.2/nonebot_plugin_penguin/render/__init__.py
+-rw-r--r--   0        0        0      870 2023-05-08 08:56:19.698741 nonebot_plugin_penguin-0.0.2/nonebot_plugin_penguin/render/item_sprite.py
+-rw-r--r--   0        0        0     2793 2023-05-08 08:56:19.698741 nonebot_plugin_penguin-0.0.2/nonebot_plugin_penguin/render/table.py
+-rw-r--r--   0        0        0      970 2023-05-08 08:56:19.698741 nonebot_plugin_penguin-0.0.2/nonebot_plugin_penguin/render/templates/app.css
+-rw-r--r--   0        0        0     3309 2023-05-08 08:56:19.698741 nonebot_plugin_penguin-0.0.2/nonebot_plugin_penguin/render/templates/card.css
+-rw-r--r--   0        0        0     2731 2023-05-08 08:56:19.698741 nonebot_plugin_penguin-0.0.2/nonebot_plugin_penguin/render/templates/item_card.html
+-rw-r--r--   0        0        0  1171678 2023-05-08 08:56:19.698741 nonebot_plugin_penguin-0.0.2/nonebot_plugin_penguin/render/templates/sprite.202210111514.png
+-rw-r--r--   0        0        0     2774 2023-05-08 08:56:19.698741 nonebot_plugin_penguin-0.0.2/nonebot_plugin_penguin/render/templates/stage_card.html
+-rw-r--r--   0        0        0      197 2023-05-08 08:56:19.698741 nonebot_plugin_penguin-0.0.2/nonebot_plugin_penguin/render/utils.py
+-rw-r--r--   0        0        0     5457 2023-05-08 08:56:19.698741 nonebot_plugin_penguin-0.0.2/nonebot_plugin_penguin/request.py
+-rw-r--r--   0        0        0      318 2023-05-08 08:56:19.698741 nonebot_plugin_penguin-0.0.2/nonebot_plugin_penguin/schedule.py
+-rw-r--r--   0        0        0      353 2023-05-08 08:56:19.698741 nonebot_plugin_penguin-0.0.2/nonebot_plugin_penguin/startup.py
+-rw-r--r--   0        0        0     1291 2023-05-08 08:56:19.698741 nonebot_plugin_penguin-0.0.2/nonebot_plugin_penguin/trim.py
+-rw-r--r--   0        0        0     2628 2023-05-08 08:56:19.698741 nonebot_plugin_penguin-0.0.2/nonebot_plugin_penguin/types.py
+-rw-r--r--   0        0        0    10980 2023-05-08 08:56:19.702741 nonebot_plugin_penguin-0.0.2/nonebot_plugin_penguin/user.py
+-rw-r--r--   0        0        0     2071 2023-05-08 08:56:19.702741 nonebot_plugin_penguin-0.0.2/nonebot_plugin_penguin/utils.py
+-rw-r--r--   0        0        0     1832 2023-05-08 08:56:19.702741 nonebot_plugin_penguin-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     6540 1970-01-01 00:00:00.000000 nonebot_plugin_penguin-0.0.2/PKG-INFO
```

### Comparing `nonebot_plugin_penguin-0.0.1/LICENSE` & `nonebot_plugin_penguin-0.0.2/LICENSE`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 AzideCupric
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 AzideCupric
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `nonebot_plugin_penguin-0.0.1/nonebot_plugin_penguin/db.py` & `nonebot_plugin_penguin-0.0.2/nonebot_plugin_penguin/db.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,78 +1,80 @@
-import time
-
-from httpx import AsyncClient
-from tinydb import Query, TinyDB
-
-from .config import plugin_config
-
-
-class DB:
-    def __init__(self) -> None:
-        self._do_init()
-
-    def _do_init(self):
-        self.id_map: TinyDB = TinyDB(plugin_config.penguin_id_map, encoding="utf-8")
-        self.items_map = self.id_map.table("items")
-        self.stages_map = self.id_map.table("stages")
-        self.db_check = self.id_map.table("check")
-
-    async def close(self):
-        self.id_map.close()
-
-    # 反序列化时忽略不需要的字段
-    @staticmethod
-    def _ignore_field(obj):
-        return {k: v for k, v in obj.items() if k != "dropInfos"}
-
-    async def id_map_update(self):
-        if last_update := self.db_check.get(Query().last_update.exists()):
-            last_update_time: int = last_update["last_update"]
-            if time.time() - last_update_time < 60 * 60 * 24:  # 小于1天就不用更新了
-                return
-
-        self.id_map.clear_cache()
-
-        self.items_map.truncate()
-        self.stages_map.truncate()
-
-        async with AsyncClient() as clt:
-            new_items = await clt.get(
-                f"{plugin_config.penguin_site}/PenguinStats/api/v2/items"
-            )
-            new_stages = await clt.get(
-                f"{plugin_config.penguin_site}/PenguinStats/api/v2/stages"
-            )
-
-        self.items_map.insert_multiple(new_items.json())
-        self.stages_map.insert_multiple(
-            new_stages.json(object_hook=self._ignore_field)
-        )  # 反序列化时忽略不需要的字段, 防止内存占用过大
-        self.db_check.upsert(
-            {"last_update": int(time.time())}, Query().last_update.exists()
-        )
-
-    async def get_item_id(self, item_name: str):
-        q = Query()
-        if item := self.items_map.get(
-            q.name_i18n.test(lambda x: item_name in x.values())
-        ):
-            return [item]
-        else:
-
-            def _is_item_in_nested_alias(dict_values) -> bool:
-                for values in dict_values:
-                    if item_name in values:
-                        return True
-                return False
-
-            items = self.items_map.search(
-                q.alias.test(lambda x: _is_item_in_nested_alias(x.values()))
-            )
-            return items
-
-    async def get_stage_id(self, stage_name: str):
-        q = Query()
-        return self.stages_map.get(q.code_i18n.test(lambda x: stage_name in x.values()))
-
-
-db = DB()
+import time
+
+from httpx import AsyncClient
+from tinydb import Query, TinyDB
+
+from .config import plugin_config
+
+
+class DB:
+    def __init__(self) -> None:
+        self._do_init()
+
+    def _do_init(self):
+        self.id_map: TinyDB = TinyDB(plugin_config.penguin_id_map, encoding="utf-8")
+        self.items_map = self.id_map.table("items")
+        self.stages_map = self.id_map.table("stages")
+        self.db_check = self.id_map.table("check")
+
+    async def close(self):
+        self.id_map.close()
+
+    # 反序列化时忽略不需要的字段
+    @staticmethod
+    def _ignore_field(obj):
+        return {k: v for k, v in obj.items() if k != "dropInfos"}
+
+    async def id_map_update(self):
+        if last_update := self.db_check.get(Query().last_update.exists()):
+            last_update_time: int = last_update["last_update"]
+            if time.time() - last_update_time < 60 * 60 * 24:  # 小于1天就不用更新了
+                return
+
+        self.id_map.clear_cache()
+
+        self.items_map.truncate()
+        self.stages_map.truncate()
+
+        async with AsyncClient() as clt:
+            new_items = await clt.get(
+                f"{plugin_config.penguin_site}/PenguinStats/api/v2/items"
+            )
+            new_stages = await clt.get(
+                f"{plugin_config.penguin_site}/PenguinStats/api/v2/stages"
+            )
+
+        self.items_map.insert_multiple(new_items.json())
+        self.stages_map.insert_multiple(
+            new_stages.json(object_hook=self._ignore_field)
+        )  # 反序列化时忽略不需要的字段, 防止内存占用过大
+        self.db_check.upsert(
+            {"last_update": int(time.time())}, Query().last_update.exists()
+        )
+
+    async def get_item_id(self, item_name: str):
+        q = Query()
+        if item := self.items_map.get(
+            q.name_i18n.test(lambda x: item_name in x.values())
+        ):
+            return [item]
+        else:
+
+            def _is_item_in_nested_alias(dict_values) -> bool:
+                for values in dict_values:
+                    if item_name in values:
+                        return True
+                return False
+
+            items = self.items_map.search(
+                q.alias.test(lambda x: _is_item_in_nested_alias(x.values()))
+            )
+            return items
+
+    async def get_stage_id(self, stage_name: str):
+        q = Query()
+        return self.stages_map.search(
+            q.code_i18n.test(lambda x: stage_name in x.values())
+        )
+
+
+db = DB()
```

### Comparing `nonebot_plugin_penguin-0.0.1/nonebot_plugin_penguin/render/item_sprite.py` & `nonebot_plugin_penguin-0.0.2/nonebot_plugin_penguin/render/item_sprite.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-from ..types import Coord
-
-
-class ItemIcon:
-    size: int = 183
-    dimensions: tuple = (1098, 3111)
-    pic: str = "sprite.202210111514.png"
-    previous_size: int = 60
-
-    @classmethod
-    def transform_coord(cls, coord: Coord, size: int | None = None) -> Coord:
-        size = size or cls.previous_size
-        return tuple(map(lambda x: x * size, coord))
-
-    @classmethod
-    def style(cls, coord: Coord, size: int | None = None):
-        size = size or cls.previous_size
-        zoom = size / cls.size
-        real_coord = cls.transform_coord(coord, size)
-        return f"""
-        height: {size}px;
-        width: {size}px;
-        background-image: url(./{cls.pic});
-        background-size: {round(cls.dimensions[0] * zoom)}px {round(cls.dimensions[1] * zoom)}px;
-        background-position: {-real_coord[0]}px {-real_coord[1]}px;
-        """  # noqa: E501
+from ..types import Coord
+
+
+class ItemIcon:
+    size: int = 183
+    dimensions: tuple = (1098, 3111)
+    pic: str = "sprite.202210111514.png"
+    previous_size: int = 60
+
+    @classmethod
+    def transform_coord(cls, coord: Coord, size: int | None = None) -> Coord:
+        size = size or cls.previous_size
+        return tuple(map(lambda x: x * size, coord))
+
+    @classmethod
+    def style(cls, coord: Coord, size: int | None = None):
+        size = size or cls.previous_size
+        zoom = size / cls.size
+        real_coord = cls.transform_coord(coord, size)
+        return f"""
+        height: {size}px;
+        width: {size}px;
+        background-image: url(./{cls.pic});
+        background-size: {round(cls.dimensions[0] * zoom)}px {round(cls.dimensions[1] * zoom)}px;
+        background-position: {-real_coord[0]}px {-real_coord[1]}px;
+        """  # noqa: E501
```

### Comparing `nonebot_plugin_penguin-0.0.1/nonebot_plugin_penguin/render/templates/card.css` & `nonebot_plugin_penguin-0.0.2/nonebot_plugin_penguin/render/templates/card.css`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,166 +1,166 @@
-body {
-  background-color: rgba(0, 0, 0, 1);
-  margin: 0px;
-}
-.v-tooltip__content {
-  position: absolute;
-}
-
-.theme--light.v-sheet {
-  background-color: #fff;
-}
-
-.v-sheet {
-  border-radius: 5px;
-}
-
-.v-card__title {
-  -webkit-box-align: center;
-  -webkit-align-items: center;
-  -moz-box-align: center;
-  -ms-flex-align: center;
-  align-items: center;
-  display: -webkit-box;
-  display: -webkit-flex;
-  display: -moz-box;
-  display: -ms-flexbox;
-  display: flex;
-  -webkit-flex-wrap: wrap;
-  -ms-flex-wrap: wrap;
-  flex-wrap: wrap;
-  font-size: 1.25rem;
-  font-weight: 500;
-  letter-spacing: 0.0125em;
-  line-height: 2rem;
-  word-break: break-all;
-}
-
-.v-card__text,
-.v-card__title {
-  padding: 16px;
-}
-
-.v-card__title > figure {
-  display: block;
-  margin-block-start: 0;
-  margin-block-end: 0;
-  margin-inline-start: 5px;
-  margin-inline-end: 0px;
-}
-.v-card__title > span {
-  display: block;
-  margin-block-start: 0px;
-  margin-block-end: 0;
-  margin-inline-start: auto;
-  margin-inline-end: 0px;
-  font-weight: bold;
-}
-
-.v-card__title + .v-card__text {
-  padding-top: 0px;
-}
-
-.v-tooltip__content .theme--light.v-data-table {
-  background: #f0f0f0 !important;
-}
-
-.v-data-table {
-  max-width: 100%;
-  border-radius: 5px;
-}
-
-.v-data-table__wrapper {
-  overflow-x: auto;
-  overflow-y: hidden;
-}
-
-.theme--light.v-data-table thead tr:last-child th {
-  border-bottom: thin solid rgba(19, 140, 221, 0.438);
-}
-
-.theme--light.v-data-table thead tr th {
-  color: rgba(5, 61, 114, 0.6);
-}
-
-.v-data-table th {
-  -webkit-user-select: none;
-  -moz-user-select: none;
-  -ms-user-select: none;
-  user-select: none;
-  font-size: 0.8rem;
-  height: 32px;
-}
-
-.v-data-table td,
-.v-data-table th {
-  padding: 0 16px;
-}
-
-.v-icon {
-  -webkit-box-align: center;
-  -webkit-align-items: center;
-  -moz-box-align: center;
-  -ms-flex-align: center;
-  align-items: center;
-  display: -webkit-inline-box;
-  display: -webkit-inline-flex;
-  display: -moz-inline-box;
-  display: -ms-inline-flexbox;
-  display: inline-flex;
-  -webkit-font-feature-settings: "liga";
-  -moz-font-feature-settings: "liga";
-  font-feature-settings: "liga";
-  font-size: 24px;
-  -webkit-box-pack: center;
-  -webkit-justify-content: center;
-  -moz-box-pack: center;
-  -ms-flex-pack: center;
-  justify-content: center;
-  letter-spacing: normal;
-  line-height: 1;
-  position: relative;
-  text-indent: 0;
-  -webkit-transition: 0.3s cubic-bezier(0.25, 0.8, 0.5, 1), visibility 0s;
-  -o-transition: 0.3s cubic-bezier(0.25, 0.8, 0.5, 1), visibility 0s;
-  transition: 0.3s cubic-bezier(0.25, 0.8, 0.5, 1), visibility 0s;
-  vertical-align: middle;
-  -webkit-user-select: none;
-  -moz-user-select: none;
-  -ms-user-select: none;
-  user-select: none;
-}
-
-.theme--light.v-icon {
-  color: rgba(9, 0, 63, 0.54);
-}
-
-small {
-  font-size: 80%;
-}
-
-.monospace {
-  font-family: benderregular, SF Mono, Droid Sans Mono, Ubuntu Mono, Consolas,
-    Courier New, Courier, monospace !important;
-  letter-spacing: 0.03rem;
-}
-
-.theme--light.v-data-table
-  tbody
-  tr:not(:last-child)
-  td:not(.v-data-table__mobile-row),
-.theme--light.v-data-table
-  tbody
-  tr:not(:last-child)
-  th:not(.v-data-table__mobile-row) {
-  border-bottom: thin solid rgba(0, 0, 0, 0.12);
-}
-
-.v-data-table td {
-  font-size: 0.875rem;
-  height: 24px;
-}
-
-/* id=more的元素文字居中*/
-#more {
-  text-align: center;
-}
+body {
+  background-color: rgba(0, 0, 0, 1);
+  margin: 0px;
+}
+.v-tooltip__content {
+  position: absolute;
+}
+
+.theme--light.v-sheet {
+  background-color: #fff;
+}
+
+.v-sheet {
+  border-radius: 5px;
+}
+
+.v-card__title {
+  -webkit-box-align: center;
+  -webkit-align-items: center;
+  -moz-box-align: center;
+  -ms-flex-align: center;
+  align-items: center;
+  display: -webkit-box;
+  display: -webkit-flex;
+  display: -moz-box;
+  display: -ms-flexbox;
+  display: flex;
+  -webkit-flex-wrap: wrap;
+  -ms-flex-wrap: wrap;
+  flex-wrap: wrap;
+  font-size: 1.25rem;
+  font-weight: 500;
+  letter-spacing: 0.0125em;
+  line-height: 2rem;
+  word-break: break-all;
+}
+
+.v-card__text,
+.v-card__title {
+  padding: 16px;
+}
+
+.v-card__title > figure {
+  display: block;
+  margin-block-start: 0;
+  margin-block-end: 0;
+  margin-inline-start: 5px;
+  margin-inline-end: 0px;
+}
+.v-card__title > span {
+  display: block;
+  margin-block-start: 0px;
+  margin-block-end: 0;
+  margin-inline-start: auto;
+  margin-inline-end: 0px;
+  font-weight: bold;
+}
+
+.v-card__title + .v-card__text {
+  padding-top: 0px;
+}
+
+.v-tooltip__content .theme--light.v-data-table {
+  background: #f0f0f0 !important;
+}
+
+.v-data-table {
+  max-width: 100%;
+  border-radius: 5px;
+}
+
+.v-data-table__wrapper {
+  overflow-x: auto;
+  overflow-y: hidden;
+}
+
+.theme--light.v-data-table thead tr:last-child th {
+  border-bottom: thin solid rgba(19, 140, 221, 0.438);
+}
+
+.theme--light.v-data-table thead tr th {
+  color: rgba(5, 61, 114, 0.6);
+}
+
+.v-data-table th {
+  -webkit-user-select: none;
+  -moz-user-select: none;
+  -ms-user-select: none;
+  user-select: none;
+  font-size: 0.8rem;
+  height: 32px;
+}
+
+.v-data-table td,
+.v-data-table th {
+  padding: 0 16px;
+}
+
+.v-icon {
+  -webkit-box-align: center;
+  -webkit-align-items: center;
+  -moz-box-align: center;
+  -ms-flex-align: center;
+  align-items: center;
+  display: -webkit-inline-box;
+  display: -webkit-inline-flex;
+  display: -moz-inline-box;
+  display: -ms-inline-flexbox;
+  display: inline-flex;
+  -webkit-font-feature-settings: "liga";
+  -moz-font-feature-settings: "liga";
+  font-feature-settings: "liga";
+  font-size: 24px;
+  -webkit-box-pack: center;
+  -webkit-justify-content: center;
+  -moz-box-pack: center;
+  -ms-flex-pack: center;
+  justify-content: center;
+  letter-spacing: normal;
+  line-height: 1;
+  position: relative;
+  text-indent: 0;
+  -webkit-transition: 0.3s cubic-bezier(0.25, 0.8, 0.5, 1), visibility 0s;
+  -o-transition: 0.3s cubic-bezier(0.25, 0.8, 0.5, 1), visibility 0s;
+  transition: 0.3s cubic-bezier(0.25, 0.8, 0.5, 1), visibility 0s;
+  vertical-align: middle;
+  -webkit-user-select: none;
+  -moz-user-select: none;
+  -ms-user-select: none;
+  user-select: none;
+}
+
+.theme--light.v-icon {
+  color: rgba(9, 0, 63, 0.54);
+}
+
+small {
+  font-size: 80%;
+}
+
+.monospace {
+  font-family: benderregular, SF Mono, Droid Sans Mono, Ubuntu Mono, Consolas,
+    Courier New, Courier, monospace !important;
+  letter-spacing: 0.03rem;
+}
+
+.theme--light.v-data-table
+  tbody
+  tr:not(:last-child)
+  td:not(.v-data-table__mobile-row),
+.theme--light.v-data-table
+  tbody
+  tr:not(:last-child)
+  th:not(.v-data-table__mobile-row) {
+  border-bottom: thin solid rgba(0, 0, 0, 0.12);
+}
+
+.v-data-table td {
+  font-size: 0.875rem;
+  height: 24px;
+}
+
+/* id=more的元素文字居中*/
+#more {
+  text-align: center;
+}
```

### Comparing `nonebot_plugin_penguin-0.0.1/nonebot_plugin_penguin/render/templates/sprite.202210111514.png` & `nonebot_plugin_penguin-0.0.2/nonebot_plugin_penguin/render/templates/sprite.202210111514.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_penguin-0.0.1/nonebot_plugin_penguin/request.py` & `nonebot_plugin_penguin-0.0.2/nonebot_plugin_penguin/request.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,145 +1,150 @@
-import json
-from typing import Any
-
-from httpx import AsyncClient
-
-from .config import plugin_config
-from .utils import PenguinDataParser
-from .types import (
-    Item,
-    Zone,
-    Stage,
-    Matrix,
-    Request,
-    T_Query,
-    T_Server,
-    T_Respond,
-    lang_map,
-)
-
-
-class Penguin:
-    raw: tuple[T_Query, dict[str, Any]]
-
-    async def fetch(self, request: Request) -> int:
-        """请求penguin-stats的widget数据, 存储到raw中
-
-        参数:
-            server: 服务器类型，可选(cn, kr, us, jp)
-            type: 掉落物查询类型，可选(item, stage, exact)
-            ids: 掉落物id列表, 当type为(item | stage)时,
-                ids需传入一个对应id的长度为1的tuple;
-                当type为exact时, ids需传入(stageId, ItemId)顺序的tuple
-            参考：https://widget.penguin-stats.io/
-
-        返回值:
-            html状态码
-        """
-        async with AsyncClient() as client:
-            widget_url = f"{plugin_config.penguin_widget}/result/{request.server.upper()}/{request.type}"  # noqa: E501
-            match request.type:
-                case "item" | "stage":
-                    widget_url += f"/{request.ids[0]}"
-                case "exact":
-                    assert (
-                        len(request.ids) == 2
-                    ), "当type为exact时, ids需要(StageId, ItemId)的长度为2的tuple)"
-                    widget_url += f"/{request.ids[0]}/{request.ids[1]}"
-
-            res = await client.get(widget_url)
-            html_obj = PenguinDataParser()
-            html_obj.feed(res.text)
-            assert html_obj.data
-            self.raw = (request.type, json.loads(html_obj.data))
-
-        return res.status_code
-
-    def all(self) -> tuple[T_Query, dict[str, Any]]:
-        """返回一个元组，包含请求的类型和请求的结果"""
-
-        return self.raw
-
-    def by_item_id(self, item_id: str) -> Item:
-        """返回和item_id匹配的第一个元素"""
-        items = self.all()[1].get("items")
-        assert isinstance(items, list), "items的值应该是列表而非其他！"
-        item_dict = next((item for item in items if item.get("itemId") == item_id), {})
-        if item_dict.get("spriteCoord") is None:
-            # 家具没有spriteCoord，这里手动指定一个
-            item_dict["spriteCoord"] = [2, 16]
-        return Item.parse_obj(item_dict)
-
-    def by_stage_id(self, stage_id: str) -> Stage:
-        """返回和stage_id匹配的第一个元素"""
-        matrix = self.all()[1].get("stages")
-        assert isinstance(matrix, list), "stages的值应该是列表而非其他！"
-        stage_dict = next(
-            (item for item in matrix if item.get("stageId") == stage_id), {}
-        )
-        return Stage.parse_obj(stage_dict)
-
-    def by_zone_id(self, zone_id: str) -> Zone:
-        """返回和zone_id匹配的第一个元素"""
-        zones = self.all()[1].get("zones")
-        assert isinstance(zones, list), "zones的值应该是列表而非其他！"
-        zone = next((item for item in zones if item.get("zoneId") == zone_id), {})
-        return Zone.parse_obj(zone)
-
-    def matrix(self) -> list[Matrix]:
-        raw = self.all()
-        _cache = raw[1].get("matrix")
-        assert isinstance(_cache, list), "matrix的值应该是列表而非其他！"
-
-        def gen_dict(raw_item: dict[str, str | int]) -> Matrix:
-            assert isinstance(
-                (stage_id := raw_item.get("stageId")), str
-            ), "stageId的值应该是字符串而非其他！"
-            stage = self.by_stage_id(stage_id)
-
-            assert isinstance(
-                (item_id := raw_item.get("itemId")), str
-            ), "itemId的值应该是字符串而非其他！"
-            item = self.by_item_id(item_id)
-
-            zone = self.by_zone_id(stage.zoneId)
-
-            assert isinstance(
-                (quantity := raw_item.get("quantity")), int
-            ), "quantity的值应该是整数而非其他！"
-            assert isinstance(
-                (times := raw_item.get("times")), int
-            ), "times的值应该是整数而非其他！"
-
-            percentage = round(quantity / times * 100, 2)
-            apPPR = round(stage.apCost / percentage, 2)
-            start: int = raw_item.get("start", 0)  # type: ignore
-            end: int | None = raw_item.get("end", None)  # type: ignore
-
-            return Matrix(
-                stage=stage,
-                zone=zone,
-                item=item,
-                percentage=percentage,
-                apPPR=apPPR,
-                quantity=quantity,
-                times=times,
-                start=start,
-                end=end,
-            )
-
-        _cache = map(gen_dict, _cache)
-        return list(_cache)
-
-    def translate(self, server: T_Server, type: T_Respond, id: str) -> str:
-        match type:
-            case "item":
-                item = self.by_item_id(id)
-                return item.name_i18n.get(lang_map[server], id)
-            case "stage":
-                stage = self.by_stage_id(id)
-                return stage.code_i18n.get(lang_map[server], id)
-            case "zone":
-                zone = self.by_zone_id(id)
-                return zone.zoneName_i18n.get(lang_map[server], id)
-            case _:
-                return "暂不支持"
+import json
+from typing import Any
+
+from httpx import AsyncClient
+
+from .config import plugin_config
+from .utils import PenguinDataParser
+from .types import (
+    Item,
+    Zone,
+    Stage,
+    Matrix,
+    Request,
+    T_Query,
+    T_Server,
+    T_Respond,
+    lang_map,
+)
+
+
+class Penguin:
+    raw: tuple[T_Query, dict[str, Any]]
+
+    async def fetch(self, request: Request) -> int:
+        """请求penguin-stats的widget数据, 存储到raw中
+
+        参数:
+            server: 服务器类型，可选(cn, kr, us, jp)
+            type: 掉落物查询类型，可选(item, stage, exact)
+            ids: 掉落物id列表, 当type为(item | stage)时,
+                ids需传入一个对应id的长度为1的tuple;
+                当type为exact时, ids需传入(stageId, ItemId)顺序的tuple
+            参考：https://widget.penguin-stats.io/
+
+        返回值:
+            html状态码
+        """
+        async with AsyncClient() as client:
+            widget_url = f"{plugin_config.penguin_widget}/result/{request.server.upper()}/{request.type}"  # noqa: E501
+            match request.type:
+                case "item" | "stage":
+                    widget_url += f"/{request.ids[0]}"
+                case "exact":
+                    assert (
+                        len(request.ids) == 2
+                    ), "当type为exact时, ids需要(StageId, ItemId)的长度为2的tuple)"
+                    widget_url += f"/{request.ids[0]}/{request.ids[1]}"
+
+            res = await client.get(widget_url)
+            html_obj = PenguinDataParser()
+            html_obj.feed(res.text)
+            assert html_obj.data
+            data: dict = json.loads(html_obj.data)
+
+            if data.get("error"):
+                raise ValueError(data["error"])
+
+            self.raw = (request.type, data)
+
+        return res.status_code
+
+    def all(self) -> tuple[T_Query, dict[str, Any]]:
+        """返回一个元组，包含请求的类型和请求的结果"""
+
+        return self.raw
+
+    def by_item_id(self, item_id: str) -> Item:
+        """返回和item_id匹配的第一个元素"""
+        items = self.all()[1].get("items")
+        assert isinstance(items, list), "items的值应该是列表而非其他！"
+        item_dict = next((item for item in items if item.get("itemId") == item_id), {})
+        if item_dict.get("spriteCoord") is None:
+            # 家具没有spriteCoord，这里手动指定一个
+            item_dict["spriteCoord"] = [2, 16]
+        return Item.parse_obj(item_dict)
+
+    def by_stage_id(self, stage_id: str) -> Stage:
+        """返回和stage_id匹配的第一个元素"""
+        matrix = self.all()[1].get("stages")
+        assert isinstance(matrix, list), "stages的值应该是列表而非其他！"
+        stage_dict = next(
+            (item for item in matrix if item.get("stageId") == stage_id), {}
+        )
+        return Stage.parse_obj(stage_dict)
+
+    def by_zone_id(self, zone_id: str) -> Zone:
+        """返回和zone_id匹配的第一个元素"""
+        zones = self.all()[1].get("zones")
+        assert isinstance(zones, list), "zones的值应该是列表而非其他！"
+        zone = next((item for item in zones if item.get("zoneId") == zone_id), {})
+        return Zone.parse_obj(zone)
+
+    def matrix(self) -> list[Matrix]:
+        raw = self.all()
+        _cache = raw[1].get("matrix")
+        assert isinstance(_cache, list), "matrix的值应该是列表而非其他！"
+
+        def gen_dict(raw_item: dict[str, str | int]) -> Matrix:
+            assert isinstance(
+                (stage_id := raw_item.get("stageId")), str
+            ), "stageId的值应该是字符串而非其他！"
+            stage = self.by_stage_id(stage_id)
+
+            assert isinstance(
+                (item_id := raw_item.get("itemId")), str
+            ), "itemId的值应该是字符串而非其他！"
+            item = self.by_item_id(item_id)
+
+            zone = self.by_zone_id(stage.zoneId)
+
+            assert isinstance(
+                (quantity := raw_item.get("quantity")), int
+            ), "quantity的值应该是整数而非其他！"
+            assert isinstance(
+                (times := raw_item.get("times")), int
+            ), "times的值应该是整数而非其他！"
+
+            percentage = round(quantity / times * 100, 2)
+            apPPR = round(stage.apCost / percentage, 2)
+            start: int = raw_item.get("start", 0)  # type: ignore
+            end: int | None = raw_item.get("end", None)  # type: ignore
+
+            return Matrix(
+                stage=stage,
+                zone=zone,
+                item=item,
+                percentage=percentage,
+                apPPR=apPPR,
+                quantity=quantity,
+                times=times,
+                start=start,
+                end=end,
+            )
+
+        _cache = map(gen_dict, _cache)
+        return list(_cache)
+
+    def translate(self, server: T_Server, type: T_Respond, id: str) -> str:
+        match type:
+            case "item":
+                item = self.by_item_id(id)
+                return item.name_i18n.get(lang_map[server], id)
+            case "stage":
+                stage = self.by_stage_id(id)
+                return stage.code_i18n.get(lang_map[server], id)
+            case "zone":
+                zone = self.by_zone_id(id)
+                return zone.zoneName_i18n.get(lang_map[server], id)
+            case _:
+                return "暂不支持"
```

### Comparing `nonebot_plugin_penguin-0.0.1/nonebot_plugin_penguin/types.py` & `nonebot_plugin_penguin-0.0.2/nonebot_plugin_penguin/types.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,99 +1,99 @@
-from typing import Union, Literal
-
-from pydantic import BaseModel
-
-T_Server = Literal["cn", "kr", "us", "jp"]
-T_Lang = Literal["zh", "ko", "en", "ja"]
-T_Query = Literal["item", "stage", "exact"]
-T_Model = Union["Item", "Stage", "Zone", "Matrix"]
-T_Respond = Literal["item", "stage", "zone", "matrix"]
-T_Sorted_Key = Literal["percentage", "apPPR"]
-T_Filter_Mode = Literal["all", "only_open", "only_close"]
-Coord = tuple[int, int]
-
-lang_map: dict[T_Server, T_Lang] = {"cn": "zh", "kr": "ko", "us": "en", "jp": "ja"}
-
-
-class Item(BaseModel):
-    itemId: str
-    name_i18n: dict[str, str]
-    spriteCoord: list[int]
-
-
-class Stage(BaseModel):
-    stageId: str
-    zoneId: str
-    code_i18n: dict[str, str]
-    apCost: int
-    minClearTime: int | None
-
-
-class Zone(BaseModel):
-    zoneId: str
-    zoneName_i18n: dict[str, str]
-    type: str
-
-
-class Matrix(BaseModel):
-    stage: Stage
-    zone: Zone
-    item: Item
-    percentage: float
-    apPPR: float
-    quantity: int
-    times: int
-    start: int
-    end: int | None
-
-    def export(self, mode: T_Query, lang: T_Lang):
-        match mode:
-            case "item":
-                return RenderByItem(
-                    stage_name=self.stage.code_i18n[lang],
-                    zone=self.zone.zoneName_i18n[lang],
-                    percent=str(self.percentage) + "%",
-                    ap_cost=str(self.apPPR),
-                    rop_count=str(self.quantity),
-                    simple_count=str(self.times),
-                    open=True if not self.end else False,
-                )
-            case "stage" | "exact":
-                return RenderByStage(
-                    item_name=self.item.name_i18n[lang],
-                    sprite_coord=self.item.spriteCoord,
-                    percent=str(self.percentage) + "%",
-                    ap_cost=str(self.apPPR),
-                    rop_count=str(self.quantity),
-                    simple_count=str(self.times),
-                )
-
-
-class Request(BaseModel):
-    name: str  # 关卡或者掉落物名，两者都有时，关卡在前，空格隔开
-    server: T_Server = "cn"
-    type: T_Query
-    ids: tuple[str, str] | tuple[str]
-    lang: T_Lang = "zh"
-    sort_by: T_Sorted_Key = "percentage"
-    filter_by: T_Filter_Mode = "only_open"
-    ignore_threshold: int = 100
-    reverse: bool = True
-
-
-class RenderByItem(BaseModel):
-    stage_name: str
-    zone: str
-    percent: str
-    ap_cost: str
-    rop_count: str
-    simple_count: str
-    open: bool
-
-
-class RenderByStage(BaseModel):
-    item_name: str
-    sprite_coord: list[int]
-    percent: str
-    ap_cost: str
-    rop_count: str
-    simple_count: str
+from typing import Union, Literal
+
+from pydantic import BaseModel
+
+T_Server = Literal["cn", "kr", "us", "jp"]
+T_Lang = Literal["zh", "ko", "en", "ja"]
+T_Query = Literal["item", "stage", "exact"]
+T_Model = Union["Item", "Stage", "Zone", "Matrix"]
+T_Respond = Literal["item", "stage", "zone", "matrix"]
+T_Sorted_Key = Literal["percentage", "apPPR"]
+T_Filter_Mode = Literal["all", "only_open", "only_close"]
+Coord = tuple[int, int]
+
+lang_map: dict[T_Server, T_Lang] = {"cn": "zh", "kr": "ko", "us": "en", "jp": "ja"}
+
+
+class Item(BaseModel):
+    itemId: str
+    name_i18n: dict[str, str]
+    spriteCoord: list[int]
+
+
+class Stage(BaseModel):
+    stageId: str
+    zoneId: str
+    code_i18n: dict[str, str]
+    apCost: int
+    minClearTime: int | None
+
+
+class Zone(BaseModel):
+    zoneId: str
+    zoneName_i18n: dict[str, str]
+    type: str
+
+
+class Matrix(BaseModel):
+    stage: Stage
+    zone: Zone
+    item: Item
+    percentage: float
+    apPPR: float
+    quantity: int
+    times: int
+    start: int
+    end: int | None
+
+    def export(self, mode: T_Query, lang: T_Lang):
+        match mode:
+            case "item":
+                return RenderByItem(
+                    stage_name=self.stage.code_i18n[lang],
+                    zone=self.zone.zoneName_i18n[lang],
+                    percent=str(self.percentage) + "%",
+                    ap_cost=str(self.apPPR),
+                    rop_count=str(self.quantity),
+                    simple_count=str(self.times),
+                    open=True if not self.end else False,
+                )
+            case "stage" | "exact":
+                return RenderByStage(
+                    item_name=self.item.name_i18n[lang],
+                    sprite_coord=self.item.spriteCoord,
+                    percent=str(self.percentage) + "%",
+                    ap_cost=str(self.apPPR),
+                    rop_count=str(self.quantity),
+                    simple_count=str(self.times),
+                )
+
+
+class Request(BaseModel):
+    name: str  # 关卡或者掉落物名，两者都有时，关卡在前，空格隔开
+    server: T_Server = "cn"
+    type: T_Query
+    ids: tuple[str, str] | tuple[str]
+    lang: T_Lang = "zh"
+    sort_by: T_Sorted_Key = "percentage"
+    filter_by: T_Filter_Mode = "only_open"
+    ignore_threshold: int = 100
+    reverse: bool = True
+
+
+class RenderByItem(BaseModel):
+    stage_name: str
+    zone: str
+    percent: str
+    ap_cost: str
+    rop_count: str
+    simple_count: str
+    open: bool
+
+
+class RenderByStage(BaseModel):
+    item_name: str
+    sprite_coord: list[int]
+    percent: str
+    ap_cost: str
+    rop_count: str
+    simple_count: str
```

### Comparing `nonebot_plugin_penguin-0.0.1/pyproject.toml` & `nonebot_plugin_penguin-0.0.2/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,69 +1,70 @@
-[tool.poetry]
-name = "nonebot-plugin-penguin"
-version = "0.0.1"
-description = "get penguin data and send from https://penguin-stats.io/"
-authors = ["Azide <rukuy@qq.com>"]
-license = "MIT"
-readme = "README.md"
-packages = [{ include = "nonebot_plugin_penguin" }]
-homepage = "https://github.com/AzideCupric/nonebot-plugin-penguin"
-repository = "https://github.com/AzideCupric/nonebot-plugin-penguin"
-keywords = []
-classifiers = [
-      "Development Status :: 3 - Alpha",
-  "Programming Language :: Python :: 3.10",
-  "Programming Language :: Python :: 3.11",
-  "Operating System :: Microsoft :: Windows",
-  "Operating System :: POSIX :: Linux",
-  "License :: OSI Approved :: MIT License",
-]
-
-[tool.poetry.dependencies]
-python = "^3.10"
-tinydb = "^4.7.1"
-nonebot2 = { extras = ["fastapi"], version = "^2.0.0rc4" }
-httpx = "^0.23.3"
-nonebot-plugin-htmlrender = "^0.2.0.3"
-nonebot-plugin-apscheduler = "^0.2.0"
-nonebot-plugin-send-anything-anywhere = "^0.2.2"
-nonebot-adapter-onebot = "^2.2.2"
-freezegun = "^1.2.2"
-
-[tool.poetry.group.dev.dependencies]
-isort = "^5.10.1"
-black = "^23.1.0"
-nonemoji = "^0.1.2"
-pre-commit = "^3.1.0"
-pytest = "^7.3.0"
-nonebug = {git = "https://github.com/nonebot/nonebug.git"}
-pytest-mock = "^3.10.0"
-pytest-asyncio = "^0.21.0"
-pytest-cov = "^4.0.0"
-respx = "^0.20.1"
-fastapi = "^0.95.0"
-flaky = "^3.7.0"
-pytest-xdist = {extras = ["psutil"], version = "^3.2.1"}
-
-[tool.black]
-line-length = 88
-include = '\.pyi?$'
-extend-exclude = '''
-'''
-
-[tool.isort]
-profile = "black"
-line_length = 88
-length_sort = true
-skip_gitignore = true
-force_sort_within_sections = true
-extra_standard_library = ["typing_extensions"]
-
-[tool.pycln]
-path = "."
-
-[build-system]
-requires = ["poetry_core>=1.0.0"]
-build-backend = "poetry.core.masonry.api"
-
-[tool.pytest.ini_options]
-asyncio_mode = "auto"
+[tool.poetry]
+name = "nonebot-plugin-penguin"
+version = "0.0.2"
+description = "get penguin data and send from https://penguin-stats.io/"
+authors = ["Azide <rukuy@qq.com>"]
+license = "MIT"
+readme = "README.md"
+packages = [{ include = "nonebot_plugin_penguin" }]
+homepage = "https://github.com/AzideCupric/nonebot-plugin-penguin"
+repository = "https://github.com/AzideCupric/nonebot-plugin-penguin"
+keywords = []
+classifiers = [
+      "Development Status :: 3 - Alpha",
+  "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
+  "Operating System :: Microsoft :: Windows",
+  "Operating System :: POSIX :: Linux",
+  "License :: OSI Approved :: MIT License",
+]
+
+[tool.poetry.dependencies]
+python = "^3.10"
+tinydb = "^4.7.1"
+nonebot2 = { extras = ["fastapi"], version = "^2.0.0rc4" }
+httpx = ">=0.23.3,<0.25.0"
+nonebot-plugin-htmlrender = "^0.2.0.3"
+nonebot-plugin-apscheduler = "^0.2.0"
+nonebot-plugin-send-anything-anywhere = "^0.2.2"
+nonebot-adapter-onebot = "^2.2.2"
+
+[tool.poetry.group.dev.dependencies]
+isort = "^5.10.1"
+black = "^23.1.0"
+nonemoji = "^0.1.2"
+pre-commit = "^3.1.0"
+pytest = "^7.3.0"
+nonebug = {git = "https://github.com/nonebot/nonebug.git"}
+pytest-mock = "^3.10.0"
+pytest-asyncio = "^0.21.0"
+pytest-cov = "^4.0.0"
+respx = "^0.20.1"
+fastapi = "^0.95.0"
+flaky = "^3.7.0"
+pytest-xdist = {extras = ["psutil"], version = "^3.2.1"}
+freezegun = "^1.2.2"
+nonebug-saa = "^0.1.0"
+
+[tool.black]
+line-length = 88
+include = '\.pyi?$'
+extend-exclude = '''
+'''
+
+[tool.isort]
+profile = "black"
+line_length = 88
+length_sort = true
+skip_gitignore = true
+force_sort_within_sections = true
+extra_standard_library = ["typing_extensions"]
+
+[tool.pycln]
+path = "."
+
+[build-system]
+requires = ["poetry_core>=1.0.0"]
+build-backend = "poetry.core.masonry.api"
+
+[tool.pytest.ini_options]
+asyncio_mode = "auto"
```

### Comparing `nonebot_plugin_penguin-0.0.1/README.md` & `nonebot_plugin_penguin-0.0.2/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,123 +1,148 @@
-<div align="center">
-    <a href="https://v2.nonebot.dev/store">
-        <img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo">
-    </a>
-    <br>
-    <p>
-        <img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText">
-    </p>
-</div>
-
-<div align="center">
-
-# nonebot-plugin-penguin
-
-_✨ 向企鹅物流查询关卡掉落物数据 ✨_
-
-[![license](https://img.shields.io/github/license/AzideCupric/nonebot-plugin-penguin)](https://github.com/AzideCupric/nonebot-plugin-penguin/blob/main/LICENSE)
-[![action](https://img.shields.io/github/actions/workflow/status/AzideCupric/nonebot-plugin-penguin/test.yml?branch=main)](https://github.com/AzideCupric/nonebot-plugin-penguin/actions/workflows/test.yml)
-[![codecov](https://codecov.io/gh/AzideCupric/nonebot-plugin-penguin/branch/main/graph/badge.svg?token=QCFIODJOOA)](https://codecov.io/gh/AzideCupric/nonebot-plugin-penguin)
-[![python](https://img.shields.io/badge/python-3.10+-blue.svg)](https://www.python.org/downloads/release/python-3100/)
-
-</div>
-
-## 📖 介绍
-
-接入企鹅物流查询明日方舟关卡掉落物信息！
-
-## 💿 安装
-
-<del>
-<details>
-<summary> 
-使用 nb-cli 安装 (还没上传pypi喵)
-</summary>
-在 nonebot2 项目的根目录下打开命令行, 输入以下指令即可安装
-
-    nb plugin install nonebot-plugin-penguin
-
-</details>
-</del>
-
-<details>
-<summary>使用包管理器安装</summary>
-在 nonebot2 项目的插件目录下, 打开命令行, 根据你使用的包管理器, 输入相应的安装命令
-
-<details>
-<summary>pip</summary>
-
-    pip install git+https://github.com/AzideCupric/nonebot-plugin-penguin.git
-
-</details>
-<details>
-<summary>pdm</summary>
-
-    pdm add git+https://github.com/AzideCupric/nonebot-plugin-penguin.git
-
-</details>
-<details>
-<summary>poetry</summary>
-
-    poetry add git+https://github.com/AzideCupric/nonebot-plugin-penguin.git
-
-</details>
-
-打开 nonebot2 项目根目录下的 `pyproject.toml` 文件, 在 `[tool.nonebot]` 部分追加写入
-
-    plugins = ["nonebot_plugin_penguin"]
-
-</details>
-
-## ⚙️ 配置
-
-在 nonebot2 项目的`.env`文件中添加下表中的必填配置
-
-|       配置项       | 必填 | 默认值 |                     说明                     |
-| :----------------: | :--: | :----: | :------------------------------------------: |
-|  penguin_mirrior   |  否  |   io   | 选择企鹅物流网站镜像为`国际(io)`或`国内(cn)` |
-| penguin_show_count |  否  |   5    |             查询结果显示的条目数             |
-
-## 🎉 使用
-
-### 指令
-
-    格式:
-    query [-h] {item,stage,exact} names [names ...] [-s {cn,kr,us,jp}] [-l {zh,ko,en,ja}] [-k {percentage,apPPR}] [-f {all,only_open,only_close}] [-t THRESHOLD] [-r]
-
-    位置参数:
-    {item,stage,exact}    查询类型
-    names                 关卡/掉落物名称或别名(H12-4 / 紫薯 / 固源岩), type为exact时，关卡在前，空格隔开, 例如: 1-7 固源岩
-
-    options:
-    -h, --help              显示帮助
-    -s {cn,kr,us,jp}, --server {cn,kr,us,jp}
-                            游戏服务器选择, 默认为cn
-    -l {zh,ko,en,ja}, --lang {zh,ko,en,ja}
-                            生成回复时使用的语言, 默认为zh
-    -k {percentage,apPPR}, --sort {percentage,apPPR}
-                            排序方式, 默认为percentage, apPPR: 每个掉落物平均消耗理智
-    -f {all,only_open,only_close}, --filter {all,only_open,only_close}
-                            关卡过滤方式，默认为all
-    -t THRESHOLD, --threshold THRESHOLD
-                            掉落物过滤阈值, 默认超过100的样本数才会显示
-    -r, --reverse         是否反转排序
-
-例子:
-
-1. 查询12-4的掉落物
-   query stage H12-4
-2. 查询紫薯的掉落关卡
-   query item 紫薯
-3. 查询12-4的掉落物, 且只显示开放的关卡
-   query stage 12-4 -f only_open
-4. 查询1-7的固源岩的掉落信息
-   query exact 1-7 固源岩
-
-\*请自行添加你给bot设置的命令前缀，如/query, #query
-
-### :warning:已知问题
-
-0. 初次安装时，若之前没有使用过`nonebot-plugin-htmlrender`, 第一次发送命令时会开始安装浏览器，可能会比较~~非常~~慢
-1. stage/exact查询目前还无法区分别传，复刻，初次的活动关卡(如生于黑夜DM-X, 偷懒还没写 :dove::dove::dove:)
-2. 发送查询命令之后，还需要再发一条无关消息才会开始渲染图片(会话控制问题，在改了在改了)
-3. 如果使用物品别名进行查询(如：狗粮)，可能会提示出现多个结果，但需要发送一条无关消息后bot才会回复选项，之后才能回复相应序号(还是会话控制问题，在改了在改了)
+<div align="center">
+    <a href="https://v2.nonebot.dev/store">
+        <img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo">
+    </a>
+    <br>
+    <p>
+        <img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText">
+    </p>
+</div>
+
+<div align="center">
+
+# nonebot-plugin-penguin
+
+_✨ 向企鹅物流查询关卡掉落物数据 ✨_
+
+[![license](https://img.shields.io/github/license/AzideCupric/nonebot-plugin-penguin)](https://github.com/AzideCupric/nonebot-plugin-penguin/blob/main/LICENSE)
+[![action](https://img.shields.io/github/actions/workflow/status/AzideCupric/nonebot-plugin-penguin/test.yml?branch=main)](https://github.com/AzideCupric/nonebot-plugin-penguin/actions/workflows/test.yml)
+[![codecov](https://codecov.io/gh/AzideCupric/nonebot-plugin-penguin/branch/main/graph/badge.svg?token=QCFIODJOOA)](https://codecov.io/gh/AzideCupric/nonebot-plugin-penguin)
+[![python](https://img.shields.io/badge/python-3.10+-blue.svg)](https://www.python.org/downloads/release/python-3100/)
+
+</div>
+
+## 📖 介绍
+
+接入企鹅物流查询明日方舟关卡掉落物信息！
+
+## 💿 安装
+
+<details>
+<summary> 
+使用 nb-cli 安装
+</summary>
+在 nonebot2 项目的根目录下打开命令行, 输入以下指令即可安装
+
+    nb plugin install nonebot-plugin-penguin
+
+</details>
+
+<details>
+<summary>使用包管理器安装</summary>
+在 nonebot2 项目的插件目录下, 打开命令行, 根据你使用的包管理器, 输入相应的安装命令
+
+<details>
+<summary>pip</summary>
+与仓库同步:
+
+    pip install git+https://github.com/AzideCupric/nonebot-plugin-penguin.git
+
+PyPi:
+
+    pip install nonebot-plugin-penguin
+
+</details>
+
+<details>
+<summary>poetry</summary>
+与仓库同步:
+
+    poetry add git+https://github.com/AzideCupric/nonebot-plugin-penguin.git
+
+PyPi:
+
+    poetry add nonebot-plugin-penguin
+
+</details>
+
+打开 nonebot2 项目根目录下的 `pyproject.toml` 文件, 在 `[tool.nonebot]` 部分追加写入
+
+    plugins = ["nonebot_plugin_penguin"]
+
+</details>
+
+## ⚙️ 配置
+
+在 nonebot2 项目的`.env`文件中添加下表中的必填配置
+
+|       配置项        | 必填 | 默认值 | 值类型/可选  |           说明           |
+| :-----------------: | :--: | :----: | :----------: | :----------------------: |
+|   penguin_mirrior   |  否  |   io   |   io / cn    |   选择企鹅物流网站镜像   |
+| penguin_show_count  |  否  |   5    |  任意正整数  | 查询结果显示的最大条目数 |
+| penguin_id_map_path |  否  |  <空>  | 任意存在目录 |  企鹅物流数据库存储路径  |
+
+## 🎉 使用
+
+### 指令
+
+指令名: `penguin` 或者 `企鹅物流`
+
+    格式:
+    penguin [-h] {item,stage,exact} names [names ...] [-s {cn,kr,us,jp}] [-l {zh,ko,en,ja}] [-k {percentage,apPPR}] [-f {all,only_open,only_close}] [-t THRESHOLD] [-r]
+
+    位置参数:
+    {item,stage,exact}    查询类型
+                            item: 按掉落物名查询
+                            stage: 按关卡名查询,
+                            exact: 精确查询(需指定关卡名和掉落物名)
+
+    names                 关卡/掉落物名称或别名(H12-4 / 紫薯 / 固源岩)
+                            type为exact时，关卡在前，空格隔开, 例如: 1-7 固源岩
+
+    options:
+    -h, --help              显示帮助
+
+    -s {cn,kr,us,jp}, --server {cn,kr,us,jp}
+                            游戏服务器选择, 默认为cn
+
+    -l {zh,ko,en,ja}, --lang {zh,ko,en,ja}
+                            生成回复时使用的语言, 默认为zh
+
+    -k {percentage,apPPR}, --sort {percentage,apPPR}
+                            排序方式, 默认为percentage
+                            percentage: 掉落率
+                            apPPR: 每个掉落物平均消耗理智
+
+    -f {all,only_open,only_close}, --filter {all,only_open,only_close}
+                            关卡过滤方式，默认为all
+
+    -t THRESHOLD, --threshold THRESHOLD
+                            掉落物过滤阈值, 默认超过100的样本数才会显示
+
+    -r, --reverse         是否反转排序，建议使用apPPR排序时打开
+
+例子:
+
+1. 查询12-4的掉落物
+   `penguin stage H12-4`
+2. 查询紫薯的掉落关卡
+   `penguin item 紫薯`
+3. 查询12-4的掉落物, 且只显示开放的关卡
+   `penguin stage 12-4 -f only_open`
+4. 查询1-7的固源岩的掉落信息
+   `penguin exact 1-7 固源岩`
+5. 按apPPR(单件掉落物消耗理智)排序查询固源岩的掉落关卡(-r: apPPR越小越好)
+   `penguin item 固源岩 -k apPPR -r`
+
+\*请自行添加你给bot设置的命令前缀，如`/penguin`, `#penguin`
+
+### ⚠️ 已知问题
+
+0. 初次安装时，若之前没有使用过`nonebot-plugin-htmlrender`, 第一次使用时会开始安装浏览器，可能会比较~~非常~~慢
+1. 可能是htmlrender或者网络的原因，有时候图片渲染会非常的慢，甚至超时，请重试
+
+## 📝 ToDo
+
+- 可以使用`penguin zone <活动名称>`查询一系列活动关卡
+- 可以使用`penguin item/stage name1 name2 ...`批量查询
+- 添加一个本地的缓存数据库，每周更新一次，减少网站访问频率，提高查询效率
```

#### html2text {}

```diff
@@ -7,51 +7,55 @@
  AzideCupric/nonebot-plugin-penguin/test.yml?branch=main)](https://github.com/
   AzideCupric/nonebot-plugin-penguin/actions/workflows/test.yml) [![codecov]
  (https://codecov.io/gh/AzideCupric/nonebot-plugin-penguin/branch/main/graph/
 badge.svg?token=QCFIODJOOA)](https://codecov.io/gh/AzideCupric/nonebot-plugin-
 penguin) [![python](https://img.shields.io/badge/python-3.10+-blue.svg)](https:
                //www.python.org/downloads/release/python-3100/)
 ## ð ä»ç» æ¥å¥ä¼é¹ç©æµæ¥è¯¢ææ¥æ¹èå³å¡æè½ç©ä¿¡æ¯ï¼ ##
-ð¿ å®è£    ä½¿ç¨ nb-cli å®è£ (è¿æ²¡ä¸ä¼ pypiåµ)  å¨ nonebot2
+ð¿ å®è£   ä½¿ç¨ nb-cli å®è£  å¨ nonebot2
 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin
-install nonebot-plugin-penguin    ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2
+install nonebot-plugin-penguin   ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2
 é¡¹ç®çæä»¶ç®å½ä¸, æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨,
-è¾å¥ç¸åºçå®è£å½ä»¤  pip pip install git+https://github.com/
-AzideCupric/nonebot-plugin-penguin.git   pdm pdm add git+https://github.com/
-AzideCupric/nonebot-plugin-penguin.git   poetry poetry add git+https://
-github.com/AzideCupric/nonebot-plugin-penguin.git  æå¼ nonebot2
-é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `[tool.nonebot]`
-é¨åè¿½å åå¥ plugins = ["nonebot_plugin_penguin"]  ## âï¸ éç½® å¨
-nonebot2 é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¿å¡«éç½® | éç½®é¡¹ |
-å¿å¡« | é»è®¤å¼ | è¯´æ | | :----------------: | :--: | :----: | :---------
----------------------------------: | | penguin_mirrior | å¦ | io |
-éæ©ä¼é¹ç©æµç½ç«éåä¸º`å½é(io)`æ`å½å(cn)` | |
-penguin_show_count | å¦ | 5 | æ¥è¯¢ç»ææ¾ç¤ºçæ¡ç®æ° | ## ð ä½¿ç¨
-### æä»¤ æ ¼å¼: query [-h] {item,stage,exact} names [names ...] [-s
-{cn,kr,us,jp}] [-l {zh,ko,en,ja}] [-k {percentage,apPPR}] [-f
-{all,only_open,only_close}] [-t THRESHOLD] [-r] ä½ç½®åæ°:
-{item,stage,exact} æ¥è¯¢ç±»å names å³å¡/æè½ç©åç§°æå«å(H12-4 /
-ç´«è¯ / åºæºå²©), typeä¸ºexactæ¶ï¼å³å¡å¨åï¼ç©ºæ ¼éå¼, ä¾å¦: 1-
-7 åºæºå²© options: -h, --help æ¾ç¤ºå¸®å© -s {cn,kr,us,jp}, --server
+è¾å¥ç¸åºçå®è£å½ä»¤  pip ä¸ä»åºåæ­¥: pip install git+https://
+github.com/AzideCupric/nonebot-plugin-penguin.git PyPi: pip install nonebot-
+plugin-penguin   poetry ä¸ä»åºåæ­¥: poetry add git+https://github.com/
+AzideCupric/nonebot-plugin-penguin.git PyPi: poetry add nonebot-plugin-penguin
+æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `
+[tool.nonebot]` é¨åè¿½å åå¥ plugins = ["nonebot_plugin_penguin"]  ##
+âï¸ éç½® å¨ nonebot2
+é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¿å¡«éç½® | éç½®é¡¹ | å¿å¡« |
+é»è®¤å¼ | å¼ç±»å/å¯é | è¯´æ | | :-----------------: | :--: | :----: |
+:----------: | :----------------------: | | penguin_mirrior | å¦ | io | io /
+cn | éæ©ä¼é¹ç©æµç½ç«éå | | penguin_show_count | å¦ | 5 |
+ä»»ææ­£æ´æ° | æ¥è¯¢ç»ææ¾ç¤ºçæå¤§æ¡ç®æ° | | penguin_id_map_path
+| å¦ | <ç©º> | ä»»æå­å¨ç®å½ | ä¼é¹ç©æµæ°æ®åºå­å¨è·¯å¾ | ##
+ð ä½¿ç¨ ### æä»¤ æä»¤å: `penguin` æè `ä¼é¹ç©æµ` æ ¼å¼:
+penguin [-h] {item,stage,exact} names [names ...] [-s {cn,kr,us,jp}] [-l
+{zh,ko,en,ja}] [-k {percentage,apPPR}] [-f {all,only_open,only_close}] [-
+t THRESHOLD] [-r] ä½ç½®åæ°: {item,stage,exact} æ¥è¯¢ç±»å item:
+ææè½ç©åæ¥è¯¢ stage: æå³å¡åæ¥è¯¢, exact: ç²¾ç¡®æ¥è¯¢
+(éæå®å³å¡ååæè½ç©å) names å³å¡/æè½ç©åç§°æå«å(H12-
+4 / ç´«è¯ / åºæºå²©) typeä¸ºexactæ¶ï¼å³å¡å¨åï¼ç©ºæ ¼éå¼, ä¾å¦:
+1-7 åºæºå²© options: -h, --help æ¾ç¤ºå¸®å© -s {cn,kr,us,jp}, --server
 {cn,kr,us,jp} æ¸¸ææå¡å¨éæ©, é»è®¤ä¸ºcn -l {zh,ko,en,ja}, --lang
 {zh,ko,en,ja} çæåå¤æ¶ä½¿ç¨çè¯­è¨, é»è®¤ä¸ºzh -k
-{percentage,apPPR}, --sort {percentage,apPPR} æåºæ¹å¼,
-é»è®¤ä¸ºpercentage, apPPR: æ¯ä¸ªæè½ç©å¹³åæ¶èçæº -f
+{percentage,apPPR}, --sort {percentage,apPPR} æåºæ¹å¼, é»è®¤ä¸ºpercentage
+percentage: æè½ç apPPR: æ¯ä¸ªæè½ç©å¹³åæ¶èçæº -f
 {all,only_open,only_close}, --filter {all,only_open,only_close}
 å³å¡è¿æ»¤æ¹å¼ï¼é»è®¤ä¸ºall -t THRESHOLD, --threshold THRESHOLD
 æè½ç©è¿æ»¤éå¼, é»è®¤è¶è¿100çæ ·æ¬æ°æä¼æ¾ç¤º -r, --reverse
-æ¯å¦åè½¬æåº ä¾å­: 1. æ¥è¯¢12-4çæè½ç© query stage H12-4 2.
-æ¥è¯¢ç´«è¯çæè½å³å¡ query item ç´«è¯ 3. æ¥è¯¢12-4çæè½ç©,
-ä¸åªæ¾ç¤ºå¼æ¾çå³å¡ query stage 12-4 -f only_open 4. æ¥è¯¢1-
-7çåºæºå²©çæè½ä¿¡æ¯ query exact 1-7 åºæºå²©
-\*è¯·èªè¡æ·»å ä½ ç»botè®¾ç½®çå½ä»¤åç¼ï¼å¦/query, #query ### :
-warning:å·²ç¥é®é¢ 0. åæ¬¡å®è£æ¶ï¼è¥ä¹åæ²¡æä½¿ç¨è¿`nonebot-
+æ¯å¦åè½¬æåºï¼å»ºè®®ä½¿ç¨apPPRæåºæ¶æå¼ ä¾å­: 1. æ¥è¯¢12-
+4çæè½ç© `penguin stage H12-4` 2. æ¥è¯¢ç´«è¯çæè½å³å¡ `penguin
+item ç´«è¯` 3. æ¥è¯¢12-4çæè½ç©, ä¸åªæ¾ç¤ºå¼æ¾çå³å¡ `penguin
+stage 12-4 -f only_open` 4. æ¥è¯¢1-7çåºæºå²©çæè½ä¿¡æ¯ `penguin exact
+1-7 åºæºå²©` 5. æapPPR
+(åä»¶æè½ç©æ¶èçæº)æåºæ¥è¯¢åºæºå²©çæè½å³å¡(-r:
+apPPRè¶å°è¶å¥½) `penguin item åºæºå²© -k apPPR -r`
+\*è¯·èªè¡æ·»å ä½ ç»botè®¾ç½®çå½ä»¤åç¼ï¼å¦`/penguin`, `#penguin` ###
+â ï¸ å·²ç¥é®é¢ 0. åæ¬¡å®è£æ¶ï¼è¥ä¹åæ²¡æä½¿ç¨è¿`nonebot-
 plugin-htmlrender`,
-ç¬¬ä¸æ¬¡åéå½ä»¤æ¶ä¼å¼å§å®è£æµè§å¨ï¼å¯è½ä¼æ¯è¾~~éå¸¸~~æ¢
-1. stage/
-exactæ¥è¯¢ç®åè¿æ æ³åºåå«ä¼ ï¼å¤å»ï¼åæ¬¡çæ´»å¨å³å¡
-(å¦çäºé»å¤DM-X, å·æè¿æ²¡å :dove::dove::dove:) 2.
-åéæ¥è¯¢å½ä»¤ä¹åï¼è¿éè¦ååä¸æ¡æ å³æ¶æ¯æä¼å¼å§æ¸²æå¾ç
-(ä¼è¯æ§å¶é®é¢ï¼å¨æ¹äºå¨æ¹äº) 3.
-å¦æä½¿ç¨ç©åå«åè¿è¡æ¥è¯¢
-(å¦ï¼çç²®)ï¼å¯è½ä¼æç¤ºåºç°å¤ä¸ªç»æï¼ä½éè¦åéä¸æ¡æ å³æ¶æ¯åbotæä¼åå¤éé¡¹ï¼ä¹åæè½åå¤ç¸åºåºå·
-(è¿æ¯ä¼è¯æ§å¶é®é¢ï¼å¨æ¹äºå¨æ¹äº)
+ç¬¬ä¸æ¬¡ä½¿ç¨æ¶ä¼å¼å§å®è£æµè§å¨ï¼å¯è½ä¼æ¯è¾~~éå¸¸~~æ¢ 1.
+å¯è½æ¯htmlrenderæèç½ç»çåå ï¼ææ¶åå¾çæ¸²æä¼éå¸¸çæ¢ï¼çè³è¶æ¶ï¼è¯·éè¯
+## ð ToDo - å¯ä»¥ä½¿ç¨`penguin zone
+<æ´»å¨åç§°>`æ¥è¯¢ä¸ç³»åæ´»å¨å³å¡ - å¯ä»¥ä½¿ç¨`penguin item/stage
+name1 name2 ...`æ¹éæ¥è¯¢ -
+æ·»å ä¸ä¸ªæ¬å°çç¼å­æ°æ®åºï¼æ¯å¨æ´æ°ä¸æ¬¡ï¼åå°ç½ç«è®¿é®é¢çï¼æé«æ¥è¯¢æç
```

### Comparing `nonebot_plugin_penguin-0.0.1/PKG-INFO` & `nonebot_plugin_penguin-0.0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-penguin
-Version: 0.0.1
+Version: 0.0.2
 Summary: get penguin data and send from https://penguin-stats.io/
 Home-page: https://github.com/AzideCupric/nonebot-plugin-penguin
 License: MIT
 Author: Azide
 Author-email: rukuy@qq.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -12,16 +12,15 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: freezegun (>=1.2.2,<2.0.0)
-Requires-Dist: httpx (>=0.23.3,<0.24.0)
+Requires-Dist: httpx (>=0.23.3,<0.25.0)
 Requires-Dist: nonebot-adapter-onebot (>=2.2.2,<3.0.0)
 Requires-Dist: nonebot-plugin-apscheduler (>=0.2.0,<0.3.0)
 Requires-Dist: nonebot-plugin-htmlrender (>=0.2.0.3,<0.3.0.0)
 Requires-Dist: nonebot-plugin-send-anything-anywhere (>=0.2.2,<0.3.0)
 Requires-Dist: nonebot2[fastapi] (>=2.0.0rc4,<3.0.0)
 Requires-Dist: tinydb (>=4.7.1,<5.0.0)
 Project-URL: Repository, https://github.com/AzideCupric/nonebot-plugin-penguin
@@ -52,102 +51,127 @@
 
 ## 📖 介绍
 
 接入企鹅物流查询明日方舟关卡掉落物信息！
 
 ## 💿 安装
 
-<del>
 <details>
 <summary> 
-使用 nb-cli 安装 (还没上传pypi喵)
+使用 nb-cli 安装
 </summary>
 在 nonebot2 项目的根目录下打开命令行, 输入以下指令即可安装
 
     nb plugin install nonebot-plugin-penguin
 
 </details>
-</del>
 
 <details>
 <summary>使用包管理器安装</summary>
 在 nonebot2 项目的插件目录下, 打开命令行, 根据你使用的包管理器, 输入相应的安装命令
 
 <details>
 <summary>pip</summary>
+与仓库同步:
 
     pip install git+https://github.com/AzideCupric/nonebot-plugin-penguin.git
 
-</details>
-<details>
-<summary>pdm</summary>
+PyPi:
 
-    pdm add git+https://github.com/AzideCupric/nonebot-plugin-penguin.git
+    pip install nonebot-plugin-penguin
 
 </details>
+
 <details>
 <summary>poetry</summary>
+与仓库同步:
 
     poetry add git+https://github.com/AzideCupric/nonebot-plugin-penguin.git
 
+PyPi:
+
+    poetry add nonebot-plugin-penguin
+
 </details>
 
 打开 nonebot2 项目根目录下的 `pyproject.toml` 文件, 在 `[tool.nonebot]` 部分追加写入
 
     plugins = ["nonebot_plugin_penguin"]
 
 </details>
 
 ## ⚙️ 配置
 
 在 nonebot2 项目的`.env`文件中添加下表中的必填配置
 
-|       配置项       | 必填 | 默认值 |                     说明                     |
-| :----------------: | :--: | :----: | :------------------------------------------: |
-|  penguin_mirrior   |  否  |   io   | 选择企鹅物流网站镜像为`国际(io)`或`国内(cn)` |
-| penguin_show_count |  否  |   5    |             查询结果显示的条目数             |
+|       配置项        | 必填 | 默认值 | 值类型/可选  |           说明           |
+| :-----------------: | :--: | :----: | :----------: | :----------------------: |
+|   penguin_mirrior   |  否  |   io   |   io / cn    |   选择企鹅物流网站镜像   |
+| penguin_show_count  |  否  |   5    |  任意正整数  | 查询结果显示的最大条目数 |
+| penguin_id_map_path |  否  |  <空>  | 任意存在目录 |  企鹅物流数据库存储路径  |
 
 ## 🎉 使用
 
 ### 指令
 
+指令名: `penguin` 或者 `企鹅物流`
+
     格式:
-    query [-h] {item,stage,exact} names [names ...] [-s {cn,kr,us,jp}] [-l {zh,ko,en,ja}] [-k {percentage,apPPR}] [-f {all,only_open,only_close}] [-t THRESHOLD] [-r]
+    penguin [-h] {item,stage,exact} names [names ...] [-s {cn,kr,us,jp}] [-l {zh,ko,en,ja}] [-k {percentage,apPPR}] [-f {all,only_open,only_close}] [-t THRESHOLD] [-r]
 
     位置参数:
     {item,stage,exact}    查询类型
-    names                 关卡/掉落物名称或别名(H12-4 / 紫薯 / 固源岩), type为exact时，关卡在前，空格隔开, 例如: 1-7 固源岩
+                            item: 按掉落物名查询
+                            stage: 按关卡名查询,
+                            exact: 精确查询(需指定关卡名和掉落物名)
+
+    names                 关卡/掉落物名称或别名(H12-4 / 紫薯 / 固源岩)
+                            type为exact时，关卡在前，空格隔开, 例如: 1-7 固源岩
 
     options:
     -h, --help              显示帮助
+
     -s {cn,kr,us,jp}, --server {cn,kr,us,jp}
                             游戏服务器选择, 默认为cn
+
     -l {zh,ko,en,ja}, --lang {zh,ko,en,ja}
                             生成回复时使用的语言, 默认为zh
+
     -k {percentage,apPPR}, --sort {percentage,apPPR}
-                            排序方式, 默认为percentage, apPPR: 每个掉落物平均消耗理智
+                            排序方式, 默认为percentage
+                            percentage: 掉落率
+                            apPPR: 每个掉落物平均消耗理智
+
     -f {all,only_open,only_close}, --filter {all,only_open,only_close}
                             关卡过滤方式，默认为all
+
     -t THRESHOLD, --threshold THRESHOLD
                             掉落物过滤阈值, 默认超过100的样本数才会显示
-    -r, --reverse         是否反转排序
+
+    -r, --reverse         是否反转排序，建议使用apPPR排序时打开
 
 例子:
 
 1. 查询12-4的掉落物
-   query stage H12-4
+   `penguin stage H12-4`
 2. 查询紫薯的掉落关卡
-   query item 紫薯
+   `penguin item 紫薯`
 3. 查询12-4的掉落物, 且只显示开放的关卡
-   query stage 12-4 -f only_open
+   `penguin stage 12-4 -f only_open`
 4. 查询1-7的固源岩的掉落信息
-   query exact 1-7 固源岩
+   `penguin exact 1-7 固源岩`
+5. 按apPPR(单件掉落物消耗理智)排序查询固源岩的掉落关卡(-r: apPPR越小越好)
+   `penguin item 固源岩 -k apPPR -r`
+
+\*请自行添加你给bot设置的命令前缀，如`/penguin`, `#penguin`
+
+### ⚠️ 已知问题
 
-\*请自行添加你给bot设置的命令前缀，如/query, #query
+0. 初次安装时，若之前没有使用过`nonebot-plugin-htmlrender`, 第一次使用时会开始安装浏览器，可能会比较~~非常~~慢
+1. 可能是htmlrender或者网络的原因，有时候图片渲染会非常的慢，甚至超时，请重试
 
-### :warning:已知问题
+## 📝 ToDo
 
-0. 初次安装时，若之前没有使用过`nonebot-plugin-htmlrender`, 第一次发送命令时会开始安装浏览器，可能会比较~~非常~~慢
-1. stage/exact查询目前还无法区分别传，复刻，初次的活动关卡(如生于黑夜DM-X, 偷懒还没写 :dove::dove::dove:)
-2. 发送查询命令之后，还需要再发一条无关消息才会开始渲染图片(会话控制问题，在改了在改了)
-3. 如果使用物品别名进行查询(如：狗粮)，可能会提示出现多个结果，但需要发送一条无关消息后bot才会回复选项，之后才能回复相应序号(还是会话控制问题，在改了在改了)
+- 可以使用`penguin zone <活动名称>`查询一系列活动关卡
+- 可以使用`penguin item/stage name1 name2 ...`批量查询
+- 添加一个本地的缓存数据库，每周更新一次，减少网站访问频率，提高查询效率
```

#### html2text {}

```diff
@@ -1,74 +1,78 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-penguin Version: 0.0.1 Summary: get
+Metadata-Version: 2.1 Name: nonebot-plugin-penguin Version: 0.0.2 Summary: get
 penguin data and send from https://penguin-stats.io/ Home-page: https://
 github.com/AzideCupric/nonebot-plugin-penguin License: MIT Author: Azide
 Author-email: rukuy@qq.com Requires-Python: >=3.10,<4.0 Classifier: Development
 Status :: 3 - Alpha Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows Classifier: Operating
 System :: POSIX :: Linux Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Requires-Dist: freezegun
-(>=1.2.2,<2.0.0) Requires-Dist: httpx (>=0.23.3,<0.24.0) Requires-Dist:
-nonebot-adapter-onebot (>=2.2.2,<3.0.0) Requires-Dist: nonebot-plugin-
-apscheduler (>=0.2.0,<0.3.0) Requires-Dist: nonebot-plugin-htmlrender
-(>=0.2.0.3,<0.3.0.0) Requires-Dist: nonebot-plugin-send-anything-anywhere
-(>=0.2.2,<0.3.0) Requires-Dist: nonebot2[fastapi] (>=2.0.0rc4,<3.0.0) Requires-
-Dist: tinydb (>=4.7.1,<5.0.0) Project-URL: Repository, https://github.com/
-AzideCupric/nonebot-plugin-penguin Description-Content-Type: text/markdown
+Classifier: Programming Language :: Python :: 3.11 Requires-Dist: httpx
+(>=0.23.3,<0.25.0) Requires-Dist: nonebot-adapter-onebot (>=2.2.2,<3.0.0)
+Requires-Dist: nonebot-plugin-apscheduler (>=0.2.0,<0.3.0) Requires-Dist:
+nonebot-plugin-htmlrender (>=0.2.0.3,<0.3.0.0) Requires-Dist: nonebot-plugin-
+send-anything-anywhere (>=0.2.2,<0.3.0) Requires-Dist: nonebot2[fastapi]
+(>=2.0.0rc4,<3.0.0) Requires-Dist: tinydb (>=4.7.1,<5.0.0) Project-URL:
+Repository, https://github.com/AzideCupric/nonebot-plugin-penguin Description-
+Content-Type: text/markdown
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
 # nonebot-plugin-penguin _â¨ åä¼é¹ç©æµæ¥è¯¢å³å¡æè½ç©æ°æ® â¨_
  [![license](https://img.shields.io/github/license/AzideCupric/nonebot-plugin-
   penguin)](https://github.com/AzideCupric/nonebot-plugin-penguin/blob/main/
   LICENSE) [![action](https://img.shields.io/github/actions/workflow/status/
  AzideCupric/nonebot-plugin-penguin/test.yml?branch=main)](https://github.com/
   AzideCupric/nonebot-plugin-penguin/actions/workflows/test.yml) [![codecov]
  (https://codecov.io/gh/AzideCupric/nonebot-plugin-penguin/branch/main/graph/
 badge.svg?token=QCFIODJOOA)](https://codecov.io/gh/AzideCupric/nonebot-plugin-
 penguin) [![python](https://img.shields.io/badge/python-3.10+-blue.svg)](https:
                //www.python.org/downloads/release/python-3100/)
 ## ð ä»ç» æ¥å¥ä¼é¹ç©æµæ¥è¯¢ææ¥æ¹èå³å¡æè½ç©ä¿¡æ¯ï¼ ##
-ð¿ å®è£    ä½¿ç¨ nb-cli å®è£ (è¿æ²¡ä¸ä¼ pypiåµ)  å¨ nonebot2
+ð¿ å®è£   ä½¿ç¨ nb-cli å®è£  å¨ nonebot2
 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin
-install nonebot-plugin-penguin    ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2
+install nonebot-plugin-penguin   ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2
 é¡¹ç®çæä»¶ç®å½ä¸, æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨,
-è¾å¥ç¸åºçå®è£å½ä»¤  pip pip install git+https://github.com/
-AzideCupric/nonebot-plugin-penguin.git   pdm pdm add git+https://github.com/
-AzideCupric/nonebot-plugin-penguin.git   poetry poetry add git+https://
-github.com/AzideCupric/nonebot-plugin-penguin.git  æå¼ nonebot2
-é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `[tool.nonebot]`
-é¨åè¿½å åå¥ plugins = ["nonebot_plugin_penguin"]  ## âï¸ éç½® å¨
-nonebot2 é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¿å¡«éç½® | éç½®é¡¹ |
-å¿å¡« | é»è®¤å¼ | è¯´æ | | :----------------: | :--: | :----: | :---------
----------------------------------: | | penguin_mirrior | å¦ | io |
-éæ©ä¼é¹ç©æµç½ç«éåä¸º`å½é(io)`æ`å½å(cn)` | |
-penguin_show_count | å¦ | 5 | æ¥è¯¢ç»ææ¾ç¤ºçæ¡ç®æ° | ## ð ä½¿ç¨
-### æä»¤ æ ¼å¼: query [-h] {item,stage,exact} names [names ...] [-s
-{cn,kr,us,jp}] [-l {zh,ko,en,ja}] [-k {percentage,apPPR}] [-f
-{all,only_open,only_close}] [-t THRESHOLD] [-r] ä½ç½®åæ°:
-{item,stage,exact} æ¥è¯¢ç±»å names å³å¡/æè½ç©åç§°æå«å(H12-4 /
-ç´«è¯ / åºæºå²©), typeä¸ºexactæ¶ï¼å³å¡å¨åï¼ç©ºæ ¼éå¼, ä¾å¦: 1-
-7 åºæºå²© options: -h, --help æ¾ç¤ºå¸®å© -s {cn,kr,us,jp}, --server
+è¾å¥ç¸åºçå®è£å½ä»¤  pip ä¸ä»åºåæ­¥: pip install git+https://
+github.com/AzideCupric/nonebot-plugin-penguin.git PyPi: pip install nonebot-
+plugin-penguin   poetry ä¸ä»åºåæ­¥: poetry add git+https://github.com/
+AzideCupric/nonebot-plugin-penguin.git PyPi: poetry add nonebot-plugin-penguin
+æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `
+[tool.nonebot]` é¨åè¿½å åå¥ plugins = ["nonebot_plugin_penguin"]  ##
+âï¸ éç½® å¨ nonebot2
+é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¿å¡«éç½® | éç½®é¡¹ | å¿å¡« |
+é»è®¤å¼ | å¼ç±»å/å¯é | è¯´æ | | :-----------------: | :--: | :----: |
+:----------: | :----------------------: | | penguin_mirrior | å¦ | io | io /
+cn | éæ©ä¼é¹ç©æµç½ç«éå | | penguin_show_count | å¦ | 5 |
+ä»»ææ­£æ´æ° | æ¥è¯¢ç»ææ¾ç¤ºçæå¤§æ¡ç®æ° | | penguin_id_map_path
+| å¦ | <ç©º> | ä»»æå­å¨ç®å½ | ä¼é¹ç©æµæ°æ®åºå­å¨è·¯å¾ | ##
+ð ä½¿ç¨ ### æä»¤ æä»¤å: `penguin` æè `ä¼é¹ç©æµ` æ ¼å¼:
+penguin [-h] {item,stage,exact} names [names ...] [-s {cn,kr,us,jp}] [-l
+{zh,ko,en,ja}] [-k {percentage,apPPR}] [-f {all,only_open,only_close}] [-
+t THRESHOLD] [-r] ä½ç½®åæ°: {item,stage,exact} æ¥è¯¢ç±»å item:
+ææè½ç©åæ¥è¯¢ stage: æå³å¡åæ¥è¯¢, exact: ç²¾ç¡®æ¥è¯¢
+(éæå®å³å¡ååæè½ç©å) names å³å¡/æè½ç©åç§°æå«å(H12-
+4 / ç´«è¯ / åºæºå²©) typeä¸ºexactæ¶ï¼å³å¡å¨åï¼ç©ºæ ¼éå¼, ä¾å¦:
+1-7 åºæºå²© options: -h, --help æ¾ç¤ºå¸®å© -s {cn,kr,us,jp}, --server
 {cn,kr,us,jp} æ¸¸ææå¡å¨éæ©, é»è®¤ä¸ºcn -l {zh,ko,en,ja}, --lang
 {zh,ko,en,ja} çæåå¤æ¶ä½¿ç¨çè¯­è¨, é»è®¤ä¸ºzh -k
-{percentage,apPPR}, --sort {percentage,apPPR} æåºæ¹å¼,
-é»è®¤ä¸ºpercentage, apPPR: æ¯ä¸ªæè½ç©å¹³åæ¶èçæº -f
+{percentage,apPPR}, --sort {percentage,apPPR} æåºæ¹å¼, é»è®¤ä¸ºpercentage
+percentage: æè½ç apPPR: æ¯ä¸ªæè½ç©å¹³åæ¶èçæº -f
 {all,only_open,only_close}, --filter {all,only_open,only_close}
 å³å¡è¿æ»¤æ¹å¼ï¼é»è®¤ä¸ºall -t THRESHOLD, --threshold THRESHOLD
 æè½ç©è¿æ»¤éå¼, é»è®¤è¶è¿100çæ ·æ¬æ°æä¼æ¾ç¤º -r, --reverse
-æ¯å¦åè½¬æåº ä¾å­: 1. æ¥è¯¢12-4çæè½ç© query stage H12-4 2.
-æ¥è¯¢ç´«è¯çæè½å³å¡ query item ç´«è¯ 3. æ¥è¯¢12-4çæè½ç©,
-ä¸åªæ¾ç¤ºå¼æ¾çå³å¡ query stage 12-4 -f only_open 4. æ¥è¯¢1-
-7çåºæºå²©çæè½ä¿¡æ¯ query exact 1-7 åºæºå²©
-\*è¯·èªè¡æ·»å ä½ ç»botè®¾ç½®çå½ä»¤åç¼ï¼å¦/query, #query ### :
-warning:å·²ç¥é®é¢ 0. åæ¬¡å®è£æ¶ï¼è¥ä¹åæ²¡æä½¿ç¨è¿`nonebot-
+æ¯å¦åè½¬æåºï¼å»ºè®®ä½¿ç¨apPPRæåºæ¶æå¼ ä¾å­: 1. æ¥è¯¢12-
+4çæè½ç© `penguin stage H12-4` 2. æ¥è¯¢ç´«è¯çæè½å³å¡ `penguin
+item ç´«è¯` 3. æ¥è¯¢12-4çæè½ç©, ä¸åªæ¾ç¤ºå¼æ¾çå³å¡ `penguin
+stage 12-4 -f only_open` 4. æ¥è¯¢1-7çåºæºå²©çæè½ä¿¡æ¯ `penguin exact
+1-7 åºæºå²©` 5. æapPPR
+(åä»¶æè½ç©æ¶èçæº)æåºæ¥è¯¢åºæºå²©çæè½å³å¡(-r:
+apPPRè¶å°è¶å¥½) `penguin item åºæºå²© -k apPPR -r`
+\*è¯·èªè¡æ·»å ä½ ç»botè®¾ç½®çå½ä»¤åç¼ï¼å¦`/penguin`, `#penguin` ###
+â ï¸ å·²ç¥é®é¢ 0. åæ¬¡å®è£æ¶ï¼è¥ä¹åæ²¡æä½¿ç¨è¿`nonebot-
 plugin-htmlrender`,
-ç¬¬ä¸æ¬¡åéå½ä»¤æ¶ä¼å¼å§å®è£æµè§å¨ï¼å¯è½ä¼æ¯è¾~~éå¸¸~~æ¢
-1. stage/
-exactæ¥è¯¢ç®åè¿æ æ³åºåå«ä¼ ï¼å¤å»ï¼åæ¬¡çæ´»å¨å³å¡
-(å¦çäºé»å¤DM-X, å·æè¿æ²¡å :dove::dove::dove:) 2.
-åéæ¥è¯¢å½ä»¤ä¹åï¼è¿éè¦ååä¸æ¡æ å³æ¶æ¯æä¼å¼å§æ¸²æå¾ç
-(ä¼è¯æ§å¶é®é¢ï¼å¨æ¹äºå¨æ¹äº) 3.
-å¦æä½¿ç¨ç©åå«åè¿è¡æ¥è¯¢
-(å¦ï¼çç²®)ï¼å¯è½ä¼æç¤ºåºç°å¤ä¸ªç»æï¼ä½éè¦åéä¸æ¡æ å³æ¶æ¯åbotæä¼åå¤éé¡¹ï¼ä¹åæè½åå¤ç¸åºåºå·
-(è¿æ¯ä¼è¯æ§å¶é®é¢ï¼å¨æ¹äºå¨æ¹äº)
+ç¬¬ä¸æ¬¡ä½¿ç¨æ¶ä¼å¼å§å®è£æµè§å¨ï¼å¯è½ä¼æ¯è¾~~éå¸¸~~æ¢ 1.
+å¯è½æ¯htmlrenderæèç½ç»çåå ï¼ææ¶åå¾çæ¸²æä¼éå¸¸çæ¢ï¼çè³è¶æ¶ï¼è¯·éè¯
+## ð ToDo - å¯ä»¥ä½¿ç¨`penguin zone
+<æ´»å¨åç§°>`æ¥è¯¢ä¸ç³»åæ´»å¨å³å¡ - å¯ä»¥ä½¿ç¨`penguin item/stage
+name1 name2 ...`æ¹éæ¥è¯¢ -
+æ·»å ä¸ä¸ªæ¬å°çç¼å­æ°æ®åºï¼æ¯å¨æ´æ°ä¸æ¬¡ï¼åå°ç½ç«è®¿é®é¢çï¼æé«æ¥è¯¢æç
```

