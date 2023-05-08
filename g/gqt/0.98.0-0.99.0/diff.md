# Comparing `tmp/gqt-0.98.0.tar.gz` & `tmp/gqt-0.99.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gqt-0.98.0.tar", last modified: Sat Jun 18 19:37:39 2022, max compression
+gzip compressed data, was "gqt-0.99.0.tar", last modified: Sun Jun 19 17:29:38 2022, max compression
```

## Comparing `gqt-0.98.0.tar` & `gqt-0.99.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-18 19:37:39.261589 gqt-0.98.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1080 2022-06-18 19:37:27.000000 gqt-0.98.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     4976 2022-06-18 19:37:39.261589 gqt-0.98.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4751 2022-06-18 19:37:27.000000 gqt-0.98.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-18 19:37:39.261589 gqt-0.98.0/gqt/
--rw-r--r--   0 runner    (1001) docker     (121)     7937 2022-06-18 19:37:27.000000 gqt-0.98.0/gqt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-06-18 19:37:27.000000 gqt-0.98.0/gqt/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1462 2022-06-18 19:37:27.000000 gqt-0.98.0/gqt/cache.py
--rw-r--r--   0 runner    (1001) docker     (121)      803 2022-06-18 19:37:27.000000 gqt-0.98.0/gqt/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (121)     9431 2022-06-18 19:37:27.000000 gqt-0.98.0/gqt/query_builder.py
--rw-r--r--   0 runner    (1001) docker     (121)      244 2022-06-18 19:37:27.000000 gqt-0.98.0/gqt/screen.py
--rw-r--r--   0 runner    (1001) docker     (121)    33847 2022-06-18 19:37:27.000000 gqt-0.98.0/gqt/tree.py
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-06-18 19:37:27.000000 gqt-0.98.0/gqt/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-18 19:37:39.261589 gqt-0.98.0/gqt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4976 2022-06-18 19:37:38.000000 gqt-0.98.0/gqt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      314 2022-06-18 19:37:39.000000 gqt-0.98.0/gqt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-18 19:37:38.000000 gqt-0.98.0/gqt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       42 2022-06-18 19:37:38.000000 gqt-0.98.0/gqt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       51 2022-06-18 19:37:39.000000 gqt-0.98.0/gqt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        4 2022-06-18 19:37:39.000000 gqt-0.98.0/gqt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-18 19:37:39.261589 gqt-0.98.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)      840 2022-06-18 19:37:27.000000 gqt-0.98.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-19 17:29:38.280362 gqt-0.99.0/
+-rw-r--r--   0 runner    (1001) docker     (121)     1080 2022-06-19 17:29:26.000000 gqt-0.99.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     4976 2022-06-19 17:29:38.280362 gqt-0.99.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4751 2022-06-19 17:29:26.000000 gqt-0.99.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-19 17:29:38.280362 gqt-0.99.0/gqt/
+-rw-r--r--   0 runner    (1001) docker     (121)     7937 2022-06-19 17:29:26.000000 gqt-0.99.0/gqt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       27 2022-06-19 17:29:26.000000 gqt-0.99.0/gqt/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1462 2022-06-19 17:29:26.000000 gqt-0.99.0/gqt/cache.py
+-rw-r--r--   0 runner    (1001) docker     (121)      803 2022-06-19 17:29:26.000000 gqt-0.99.0/gqt/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9431 2022-06-19 17:29:26.000000 gqt-0.99.0/gqt/query_builder.py
+-rw-r--r--   0 runner    (1001) docker     (121)      244 2022-06-19 17:29:26.000000 gqt-0.99.0/gqt/screen.py
+-rw-r--r--   0 runner    (1001) docker     (121)    34081 2022-06-19 17:29:26.000000 gqt-0.99.0/gqt/tree.py
+-rw-r--r--   0 runner    (1001) docker     (121)       23 2022-06-19 17:29:26.000000 gqt-0.99.0/gqt/version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-19 17:29:38.280362 gqt-0.99.0/gqt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4976 2022-06-19 17:29:37.000000 gqt-0.99.0/gqt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      314 2022-06-19 17:29:38.000000 gqt-0.99.0/gqt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-19 17:29:37.000000 gqt-0.99.0/gqt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       42 2022-06-19 17:29:37.000000 gqt-0.99.0/gqt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       51 2022-06-19 17:29:38.000000 gqt-0.99.0/gqt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        4 2022-06-19 17:29:38.000000 gqt-0.99.0/gqt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-19 17:29:38.280362 gqt-0.99.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (121)      840 2022-06-19 17:29:26.000000 gqt-0.99.0/setup.py
```

### Comparing `gqt-0.98.0/LICENSE` & `gqt-0.99.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gqt-0.98.0/PKG-INFO` & `gqt-0.99.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gqt
-Version: 0.98.0
+Version: 0.99.0
 Summary: GraphQL client in the terminal.
 Home-page: https://github.com/eerimoq/gqt
 Author: Erik Moqvist
 Author-email: erik.moqvist@gmail.com
 License: MIT
 License-File: LICENSE
```

### Comparing `gqt-0.98.0/README.rst` & `gqt-0.99.0/README.rst`

 * *Files identical despite different names*

### Comparing `gqt-0.98.0/gqt/__init__.py` & `gqt-0.99.0/gqt/__init__.py`

 * *Files identical despite different names*

### Comparing `gqt-0.98.0/gqt/cache.py` & `gqt-0.99.0/gqt/cache.py`

 * *Files identical despite different names*

### Comparing `gqt-0.98.0/gqt/endpoint.py` & `gqt-0.99.0/gqt/endpoint.py`

 * *Files identical despite different names*

### Comparing `gqt-0.98.0/gqt/query_builder.py` & `gqt-0.99.0/gqt/query_builder.py`

 * *Files identical despite different names*

### Comparing `gqt-0.98.0/gqt/tree.py` & `gqt-0.99.0/gqt/tree.py`

 * *Files 8% similar despite different names*

```diff
@@ -82,14 +82,15 @@
         self.y_mutation = None
 
 
 class Node:
 
     def __init__(self):
         self.parent = None
+        self.child = None
         self.next = None
         self.prev = None
         self.type = None
         self.description = None
 
     def draw(self, stdscr, y, x, cursor):
         raise NotImplementedError()
@@ -172,14 +173,32 @@
             if self.is_union:
                 return f'{self.name}{arguments} {{__typename {items}}}'
             else:
                 return f'{self.name}{arguments} {{{items}}}'
         else:
             raise Exception(f"No fields selected in '{self.name}'.")
 
+    def key_left(self):
+        if not self.is_expanded:
+            return False
+
+        self.is_expanded = False
+        self.child = None
+
+        return True
+
+    def key_right(self):
+        if self.is_expanded:
+            return False
+        else:
+            self.is_expanded = True
+            self.child = self.fields[0]
+
+            return True
+
     def query_root(self, cursor):
         cursor_root_index = self.fields.index(find_root_field(cursor))
         is_query = (cursor_root_index < self.number_of_query_fields)
 
         if is_query:
             fields = self.fields[:self.number_of_query_fields]
         else:
@@ -205,14 +224,19 @@
             return f"{kind}{variables} {{{items}}}"
         else:
             raise Exception("No fields selected.")
 
     def select(self):
         self.is_expanded = not self.is_expanded
 
+        if self.is_expanded:
+            self.child = self.fields[0]
+        else:
+            self.child = None
+
 
 class Leaf(Node):
 
     def __init__(self, name, field_type, description, fields, state):
         super().__init__()
         self.is_selected = False
         self.name = name
@@ -262,14 +286,20 @@
         addstr(stdscr, y, x + 2, self.name)
 
         return y + 1
 
     def select(self):
         self.is_selected = not self.is_selected
 
+        if self.fields is not None:
+            if self.is_selected:
+                self.child = self.fields[0]
+            else:
+                self.child = None
+
     def query(self, variables):
         if not self.is_selected:
             return None
 
         if self.fields is None:
             arguments = ''
         else:
@@ -576,14 +606,15 @@
         self.fields = ObjectFields(fields, [], types, state)
         self.fields.parent = self
 
         if self.is_optional:
             self.symbol = '□'
         else:
             self.symbol = '●'
+            self.child = self.fields[0]
 
     def draw_variable(self, stdscr, y, x, cursor):
         if cursor.node is self:
             cursor.y = y
 
             if self.state.cursor_at_input_field:
                 cursor.x = x + len(self.name) + 4 + self.pos
@@ -632,31 +663,42 @@
             elif self.state.cursor_at_input_field:
                 self.value, self.pos = edit(self.value,
                                             self.pos,
                                             KEY_BINDINGS.get(key, key))
 
                 return True
             elif key in 'v$':
-                self.is_variable = not self.is_variable
-
-                return True
+                return self.key_variable()
         elif key in 'v$':
-            self.is_variable = not self.is_variable
-
-            return True
+            return self.key_variable()
 
         return False
 
+    def key_variable(self):
+        self.is_variable = not self.is_variable
+
+        if self.is_variable:
+            self.child = None
+        elif self.symbol != '□':
+            self.child = self.fields[0]
+
+        return True
+
     def select(self):
         if self.is_optional and not self.is_variable:
             self.symbol = {
                 '□': '■',
                 '■': '□'
             }[self.symbol]
 
+            if self.symbol == '■':
+                self.child = self.fields[0]
+            else:
+                self.child = None
+
     def query(self, variables):
         if self.is_variable:
             if self.value:
                 value = f'${self.value}'
                 variables.append((value, self.type))
 
                 return value
@@ -716,14 +758,33 @@
             self.removed = True
             self.parent.item_removed(self)
 
             return True
 
         return False
 
+    def key_left(self):
+        if not self.is_expanded:
+            return False
+
+        self.is_expanded = False
+        self.child = None
+
+        return True
+
+    def key_right(self):
+        if self.is_expanded:
+            return False
+        else:
+            self.is_expanded = True
+            self.child = self.item
+            self.parent.item_selected(self)
+
+            return True
+
     def select(self):
         self.is_expanded = not self.is_expanded
 
         if self.is_expanded:
             self.parent.item_selected(self)
 
     def query(self, variables):
@@ -762,14 +823,17 @@
             self.symbol = '□'
         else:
             self.symbol = '●'
 
         self.items = []
         self.append_item()
 
+        if self.symbol == '●':
+            self.child = self.items[0]
+
     def append_item(self):
         if self.is_optional:
             item_type = self.field_type['ofType']
         else:
             item_type = self.field_type['ofType']['ofType']
 
         arg_type = {
@@ -833,46 +897,59 @@
             self.append_item()
 
     def item_removed(self, item):
         self.items.remove(item)
 
         if item.prev is not None:
             item.prev.next = item.next
+        else:
+            self.child = item.next
 
         if item.next is not None:
             item.next.prev = item.prev
 
     def select(self):
         if self.is_optional and not self.is_variable:
             self.symbol = {
                 '□': '■',
                 '■': '□'
             }[self.symbol]
 
+            if self.symbol == '■':
+                self.child = self.items[0]
+            else:
+                self.child = None
+
     def key(self, key):
         if self.is_variable:
             if key == '\t':
                 self.state.cursor_at_input_field = (
                     not self.state.cursor_at_input_field)
 
                 return True
             elif self.state.cursor_at_input_field:
                 self.value, self.pos = edit(self.value,
                                             self.pos,
                                             KEY_BINDINGS.get(key, key))
 
                 return True
             elif key in 'v$':
-                self.is_variable = not self.is_variable
-
-                return True
+                return self.key_variable()
         elif key in 'v$':
-            self.is_variable = not self.is_variable
+            return self.key_variable()
 
-            return True
+    def key_variable(self):
+        self.is_variable = not self.is_variable
+
+        if self.is_variable:
+            self.child = None
+        elif self.symbol != '□':
+            self.child = self.items[0]
+
+        return True
 
     def query(self, variables):
         if self.is_variable:
             if self.value:
                 value = f'${self.value}'
                 variables.append((value, self.type))
 
@@ -1073,74 +1150,37 @@
     def key_up(self):
         if self._cursor.prev is not None:
             self._cursor = self._find_last(self._cursor.prev)
         elif self._cursor.parent is not None:
             self._cursor = self._cursor.parent
 
     def key_down(self):
-        if isinstance(self._cursor, Object):
-            if self._cursor.is_expanded:
-                self._cursor = self._cursor.fields[0]
-                return
-        elif isinstance(self._cursor, Leaf):
-            if self._cursor.fields is not None and self._cursor.is_selected:
-                self._cursor = self._cursor.fields[0]
-                return
-        elif isinstance(self._cursor, ListItem):
-            if self._cursor.is_expanded:
-                self._cursor = self._cursor.item
-                return
-        elif isinstance(self._cursor, ListArgument):
-            if self._cursor.symbol in '■●' and not self._cursor.is_variable:
-                self._cursor = self._cursor.items[0]
-                return
-        elif isinstance(self._cursor, InputArgument):
-            if self._cursor.symbol in '■●' and not self._cursor.is_variable:
-                self._cursor = self._cursor.fields[0]
-                return
-
-        if self._cursor.next is not None:
+        if self._cursor.child is not None:
+            self._cursor = self._cursor.child
+        elif self._cursor.next is not None:
             self._cursor = self._cursor.next
         elif self._cursor.parent is not None:
             cursor = self._find_first_below(self._cursor)
 
             if cursor is not None:
                 self._cursor = cursor
 
     def key_left(self):
         if self._cursor.key_left():
             return
 
-        if isinstance(self._cursor, Object):
-            if self._cursor.is_expanded:
-                self._cursor.is_expanded = False
-                return
-        elif isinstance(self._cursor, ListItem):
-            if self._cursor.is_expanded:
-                self._cursor.is_expanded = False
-                return
-
         if self._cursor.parent is not None:
             self._cursor = self._cursor.parent
 
     def key_right(self):
         if self._cursor.key_right():
             return
 
-        if isinstance(self._cursor, Object):
-            if self._cursor.is_expanded:
-                self._cursor = self._cursor.fields[0]
-            else:
-                self._cursor.is_expanded = True
-        elif isinstance(self._cursor, ListItem):
-            if self._cursor.is_expanded:
-                self._cursor = self._cursor.item
-            else:
-                self._cursor.is_expanded = True
-                self._cursor.parent.item_selected(self._cursor)
+        if self._cursor.child is not None:
+            self._cursor = self._cursor.child
 
     def select(self):
         self._cursor.select()
 
     def key(self, key):
         done = self._cursor.key(key)
```

### Comparing `gqt-0.98.0/gqt.egg-info/PKG-INFO` & `gqt-0.99.0/gqt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gqt
-Version: 0.98.0
+Version: 0.99.0
 Summary: GraphQL client in the terminal.
 Home-page: https://github.com/eerimoq/gqt
 Author: Erik Moqvist
 Author-email: erik.moqvist@gmail.com
 License: MIT
 License-File: LICENSE
```

### Comparing `gqt-0.98.0/setup.py` & `gqt-0.99.0/setup.py`

 * *Files identical despite different names*

