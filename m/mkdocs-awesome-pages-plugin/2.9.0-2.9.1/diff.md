# Comparing `tmp/mkdocs_awesome_pages_plugin-2.9.0.tar.gz` & `tmp/mkdocs_awesome_pages_plugin-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs_awesome_pages_plugin-2.9.0.tar", max compression
+gzip compressed data, was "mkdocs_awesome_pages_plugin-2.9.1.tar", max compression
```

## Comparing `mkdocs_awesome_pages_plugin-2.9.0.tar` & `mkdocs_awesome_pages_plugin-2.9.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1071 2023-04-11 20:30:35.429559 mkdocs_awesome_pages_plugin-2.9.0/LICENSE.md
--rw-r--r--   0        0        0    12162 2023-04-11 20:30:35.429559 mkdocs_awesome_pages_plugin-2.9.0/README.md
--rw-r--r--   0        0        0        0 2023-04-11 20:30:35.429559 mkdocs_awesome_pages_plugin-2.9.0/mkdocs_awesome_pages_plugin/__init__.py
--rw-r--r--   0        0        0    10451 2023-04-11 20:30:35.429559 mkdocs_awesome_pages_plugin-2.9.0/mkdocs_awesome_pages_plugin/meta.py
--rw-r--r--   0        0        0    10039 2023-04-11 20:30:35.429559 mkdocs_awesome_pages_plugin-2.9.0/mkdocs_awesome_pages_plugin/navigation.py
--rw-r--r--   0        0        0      451 2023-04-11 20:30:35.429559 mkdocs_awesome_pages_plugin-2.9.0/mkdocs_awesome_pages_plugin/options.py
--rw-r--r--   0        0        0     5194 2023-04-11 20:30:35.429559 mkdocs_awesome_pages_plugin-2.9.0/mkdocs_awesome_pages_plugin/plugin.py
--rw-r--r--   0        0        0     1209 2023-04-11 20:30:35.433559 mkdocs_awesome_pages_plugin-2.9.0/mkdocs_awesome_pages_plugin/utils.py
--rw-r--r--   0        0        0     1056 2023-04-11 20:30:35.433559 mkdocs_awesome_pages_plugin-2.9.0/pyproject.toml
--rw-r--r--   0        0        0    13240 1970-01-01 00:00:00.000000 mkdocs_awesome_pages_plugin-2.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-08 18:43:04.501902 mkdocs_awesome_pages_plugin-2.9.1/LICENSE.md
+-rw-r--r--   0        0        0    12162 2023-05-08 18:43:04.501902 mkdocs_awesome_pages_plugin-2.9.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-08 18:43:04.501902 mkdocs_awesome_pages_plugin-2.9.1/mkdocs_awesome_pages_plugin/__init__.py
+-rw-r--r--   0        0        0    10451 2023-05-08 18:43:04.501902 mkdocs_awesome_pages_plugin-2.9.1/mkdocs_awesome_pages_plugin/meta.py
+-rw-r--r--   0        0        0    10382 2023-05-08 18:43:04.501902 mkdocs_awesome_pages_plugin-2.9.1/mkdocs_awesome_pages_plugin/navigation.py
+-rw-r--r--   0        0        0      451 2023-05-08 18:43:04.501902 mkdocs_awesome_pages_plugin-2.9.1/mkdocs_awesome_pages_plugin/options.py
+-rw-r--r--   0        0        0     5194 2023-05-08 18:43:04.501902 mkdocs_awesome_pages_plugin-2.9.1/mkdocs_awesome_pages_plugin/plugin.py
+-rw-r--r--   0        0        0     1209 2023-05-08 18:43:04.505902 mkdocs_awesome_pages_plugin-2.9.1/mkdocs_awesome_pages_plugin/utils.py
+-rw-r--r--   0        0        0     1056 2023-05-08 18:43:04.505902 mkdocs_awesome_pages_plugin-2.9.1/pyproject.toml
+-rw-r--r--   0        0        0    13240 1970-01-01 00:00:00.000000 mkdocs_awesome_pages_plugin-2.9.1/PKG-INFO
```

### Comparing `mkdocs_awesome_pages_plugin-2.9.0/LICENSE.md` & `mkdocs_awesome_pages_plugin-2.9.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mkdocs_awesome_pages_plugin-2.9.0/README.md` & `mkdocs_awesome_pages_plugin-2.9.1/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs_awesome_pages_plugin-2.9.0/mkdocs_awesome_pages_plugin/meta.py` & `mkdocs_awesome_pages_plugin-2.9.1/mkdocs_awesome_pages_plugin/meta.py`

 * *Files identical despite different names*

### Comparing `mkdocs_awesome_pages_plugin-2.9.0/mkdocs_awesome_pages_plugin/navigation.py` & `mkdocs_awesome_pages_plugin-2.9.1/mkdocs_awesome_pages_plugin/navigation.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,15 +89,15 @@
         sort_type = meta.sort_type or self.options.sort_type
         order_by = meta.order_by or self.options.order_by
 
         if order is None and sort_type is None and order_by is None:
             return
 
         if order_by == Meta.ORDER_BY_TITLE:
-            key = lambda i: get_title(i)
+            key = lambda i: self._get_item_title(i)
         else:
             key = lambda i: basename(self._get_item_path(i))
 
         if sort_type == Meta.SORT_NATURAL:
             key = natsort_keygen(key)
 
         items.sort(key=key, reverse=order == Meta.ORDER_DESC)
@@ -187,14 +187,54 @@
 
     def _get_item_path(self, item: NavigationItem) -> Optional[str]:
         if isinstance(item, Section):
             return dirname(self.meta.sections[item].path)
         elif isinstance(item, Page):
             return item.file.abs_src_path
 
+    def _get_item_title(self, item: NavigationItem) -> str:
+        # Handle custom section titles in the ".pages" file
+        if isinstance(item, Section):
+            title = self.meta.sections[item].title
+            if title is not None:
+                return title
+
+        if item.title is not None:
+            return item.title
+
+        if not isinstance(item, Page):
+            return str(item.title)
+
+        # Copy of mkdocs.structure.pages.Page._set_title and Page.read_source
+        try:
+            with open(item.file.abs_src_path, encoding="utf-8-sig", errors="strict") as f:
+                source = f.read()
+        except OSError:
+            raise OSError(f"File not found: {item.file.src_path}")
+        except ValueError:
+            raise ValueError(f"Encoding error reading file: {item.file.src_path}")
+
+        page_markdown, page_meta = mkdocs.utils.meta.get_data(source)
+
+        if "title" in page_meta:
+            return page_meta["title"]
+
+        title = mkdocs.utils.get_markdown_title(page_markdown)
+
+        if title is None:
+            if item.is_homepage:
+                title = "Home"
+            else:
+                title = item.file.name.replace("-", " ").replace("_", " ")
+                # Capitalize if the filename was all lowercase, otherwise leave it as-is.
+                if title.lower() == title:
+                    title = title.capitalize()
+
+        return title
+
     @staticmethod
     def _set_title(section: Section, meta: Meta):
         if meta.title is not None:
             section.title = meta.title
 
     @staticmethod
     def _collapse(section: Section, collapse: Optional[bool], collapse_recursive: bool) -> NavigationItem:
@@ -261,42 +301,7 @@
     ret = []
     for item in nav:
         if isinstance(item, T):
             ret.append(item)
         if item.children:
             ret.extend(get_by_type(item.children, T))
     return ret
-
-
-# Copy of mkdocs.structure.pages.Page._set_title and Page.read_source
-def get_title(item: NavigationItem) -> str:
-    if item.title is not None:
-        return item.title
-
-    if not isinstance(item, Page):
-        return str(item.title)
-
-    try:
-        with open(item.file.abs_src_path, encoding="utf-8-sig", errors="strict") as f:
-            source = f.read()
-    except OSError:
-        raise OSError(f"File not found: {item.file.src_path}")
-    except ValueError:
-        raise ValueError(f"Encoding error reading file: {item.file.src_path}")
-
-    page_markdown, page_meta = mkdocs.utils.meta.get_data(source)
-
-    if "title" in page_meta:
-        return page_meta["title"]
-
-    title = mkdocs.utils.get_markdown_title(page_markdown)
-
-    if title is None:
-        if item.is_homepage:
-            title = "Home"
-        else:
-            title = item.file.name.replace("-", " ").replace("_", " ")
-            # Capitalize if the filename was all lowercase, otherwise leave it as-is.
-            if title.lower() == title:
-                title = title.capitalize()
-
-    return title
```

### Comparing `mkdocs_awesome_pages_plugin-2.9.0/mkdocs_awesome_pages_plugin/plugin.py` & `mkdocs_awesome_pages_plugin-2.9.1/mkdocs_awesome_pages_plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `mkdocs_awesome_pages_plugin-2.9.0/mkdocs_awesome_pages_plugin/utils.py` & `mkdocs_awesome_pages_plugin-2.9.1/mkdocs_awesome_pages_plugin/utils.py`

 * *Files identical despite different names*

### Comparing `mkdocs_awesome_pages_plugin-2.9.0/pyproject.toml` & `mkdocs_awesome_pages_plugin-2.9.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mkdocs-awesome-pages-plugin"
-version = "2.9.0"
+version = "2.9.1"
 description = "An MkDocs plugin that simplifies configuring page titles and their order"
 authors = ["Lukas Geiter <info@lukasgeiter.com>"]
 repository = "https://github.com/lukasgeiter/mkdocs-awesome-pages-plugin/"
 readme = "README.md"
 license = "MIT"
 keywords = ["mkdocs", "python", "markdown", "wiki"]
 classifiers = [
```

### Comparing `mkdocs_awesome_pages_plugin-2.9.0/PKG-INFO` & `mkdocs_awesome_pages_plugin-2.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-awesome-pages-plugin
-Version: 2.9.0
+Version: 2.9.1
 Summary: An MkDocs plugin that simplifies configuring page titles and their order
 Home-page: https://github.com/lukasgeiter/mkdocs-awesome-pages-plugin/
 License: MIT
 Keywords: mkdocs,python,markdown,wiki
 Author: Lukas Geiter
 Author-email: info@lukasgeiter.com
 Requires-Python: >=3.7
```

