# Comparing `tmp/mkdocs_exporter-0.0.2.tar.gz` & `tmp/mkdocs_exporter-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs_exporter-0.0.2.tar", max compression
+gzip compressed data, was "mkdocs_exporter-1.0.0.tar", max compression
```

## Comparing `mkdocs_exporter-0.0.2.tar` & `mkdocs_exporter-1.0.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1071 2023-05-08 13:15:16.904792 mkdocs_exporter-0.0.2/LICENSE
--rw-r--r--   0        0        0     2661 2023-05-08 17:27:32.453564 mkdocs_exporter-0.0.2/README.md
--rw-r--r--   0        0        0        0 2023-05-08 15:45:32.453553 mkdocs_exporter-0.0.2/mkdocs_exporter/__init__.py
--rw-r--r--   0        0        0     1771 2023-05-08 16:10:13.643556 mkdocs_exporter-0.0.2/mkdocs_exporter/browser.py
--rw-r--r--   0        0        0       96 2023-05-06 09:39:49.274344 mkdocs_exporter-0.0.2/mkdocs_exporter/logging.py
--rw-r--r--   0        0        0      440 2023-05-08 15:32:49.823552 mkdocs_exporter-0.0.2/mkdocs_exporter/page.py
--rw-r--r--   0        0        0      705 2023-05-08 15:33:10.113552 mkdocs_exporter-0.0.2/mkdocs_exporter/plugin.py
--rw-r--r--   0        0        0        0 2023-05-06 21:44:34.488343 mkdocs_exporter-0.0.2/mkdocs_exporter/plugins/__init__.py
--rw-r--r--   0        0        0        0 2023-05-07 17:00:48.574613 mkdocs_exporter-0.0.2/mkdocs_exporter/plugins/extras/__init__.py
--rw-r--r--   0        0        0      894 2023-05-08 15:35:52.373552 mkdocs_exporter-0.0.2/mkdocs_exporter/plugins/extras/config.py
--rw-r--r--   0        0        0      629 2023-05-08 15:31:52.723552 mkdocs_exporter-0.0.2/mkdocs_exporter/plugins/extras/plugin.py
--rw-r--r--   0        0        0        0 2023-05-07 17:48:51.834620 mkdocs_exporter-0.0.2/mkdocs_exporter/plugins/pdf/__init__.py
--rw-r--r--   0        0        0      633 2023-05-08 14:24:00.883541 mkdocs_exporter-0.0.2/mkdocs_exporter/plugins/pdf/button.py
--rw-r--r--   0        0        0      969 2023-05-08 14:02:42.383538 mkdocs_exporter-0.0.2/mkdocs_exporter/plugins/pdf/config.py
--rw-r--r--   0        0        0     4420 2023-05-08 15:32:35.993552 mkdocs_exporter-0.0.2/mkdocs_exporter/plugins/pdf/plugin.py
--rw-r--r--   0        0        0     2257 2023-05-08 15:48:43.343554 mkdocs_exporter-0.0.2/mkdocs_exporter/plugins/pdf/renderer.py
--rw-r--r--   0        0        0     3714 2023-05-08 15:34:26.483550 mkdocs_exporter-0.0.2/mkdocs_exporter/preprocessor.py
--rw-r--r--   0        0        0      241 2023-05-07 12:23:00.605366 mkdocs_exporter-0.0.2/mkdocs_exporter/renderer.py
--rw-r--r--   0        0        0        0 2023-05-08 14:16:51.163540 mkdocs_exporter-0.0.2/mkdocs_exporter/resources/__init__.py
--rw-r--r--   0        0        0        0 2023-05-08 14:16:39.063540 mkdocs_exporter-0.0.2/mkdocs_exporter/resources/js/__init__.py
--rw-r--r--   0        0        0   499714 2023-05-08 14:10:56.413538 mkdocs_exporter-0.0.2/mkdocs_exporter/resources/js/pagedjs.min.js
--rw-r--r--   0        0        0     1214 2023-05-08 15:49:58.273555 mkdocs_exporter-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     4007 1970-01-01 00:00:00.000000 mkdocs_exporter-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-08 13:15:16.904792 mkdocs_exporter-1.0.0/LICENSE
+-rw-r--r--   0        0        0     2661 2023-05-08 17:27:32.453564 mkdocs_exporter-1.0.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-08 15:45:32.453553 mkdocs_exporter-1.0.0/mkdocs_exporter/__init__.py
+-rw-r--r--   0        0        0     1771 2023-05-08 16:10:13.643556 mkdocs_exporter-1.0.0/mkdocs_exporter/browser.py
+-rw-r--r--   0        0        0       96 2023-05-06 09:39:49.274344 mkdocs_exporter-1.0.0/mkdocs_exporter/logging.py
+-rw-r--r--   0        0        0      440 2023-05-08 15:32:49.823552 mkdocs_exporter-1.0.0/mkdocs_exporter/page.py
+-rw-r--r--   0        0        0      705 2023-05-08 15:33:10.113552 mkdocs_exporter-1.0.0/mkdocs_exporter/plugin.py
+-rw-r--r--   0        0        0        0 2023-05-06 21:44:34.488343 mkdocs_exporter-1.0.0/mkdocs_exporter/plugins/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-07 17:00:48.574613 mkdocs_exporter-1.0.0/mkdocs_exporter/plugins/extras/__init__.py
+-rw-r--r--   0        0        0      894 2023-05-08 15:35:52.373552 mkdocs_exporter-1.0.0/mkdocs_exporter/plugins/extras/config.py
+-rw-r--r--   0        0        0      629 2023-05-08 15:31:52.723552 mkdocs_exporter-1.0.0/mkdocs_exporter/plugins/extras/plugin.py
+-rw-r--r--   0        0        0        0 2023-05-07 17:48:51.834620 mkdocs_exporter-1.0.0/mkdocs_exporter/plugins/pdf/__init__.py
+-rw-r--r--   0        0        0      633 2023-05-08 14:24:00.883541 mkdocs_exporter-1.0.0/mkdocs_exporter/plugins/pdf/button.py
+-rw-r--r--   0        0        0      969 2023-05-08 14:02:42.383538 mkdocs_exporter-1.0.0/mkdocs_exporter/plugins/pdf/config.py
+-rw-r--r--   0        0        0     4420 2023-05-08 15:32:35.993552 mkdocs_exporter-1.0.0/mkdocs_exporter/plugins/pdf/plugin.py
+-rw-r--r--   0        0        0     2257 2023-05-08 15:48:43.343554 mkdocs_exporter-1.0.0/mkdocs_exporter/plugins/pdf/renderer.py
+-rw-r--r--   0        0        0     3714 2023-05-08 15:34:26.483550 mkdocs_exporter-1.0.0/mkdocs_exporter/preprocessor.py
+-rw-r--r--   0        0        0      241 2023-05-07 12:23:00.605366 mkdocs_exporter-1.0.0/mkdocs_exporter/renderer.py
+-rw-r--r--   0        0        0        0 2023-05-08 14:16:51.163540 mkdocs_exporter-1.0.0/mkdocs_exporter/resources/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-08 14:16:39.063540 mkdocs_exporter-1.0.0/mkdocs_exporter/resources/js/__init__.py
+-rw-r--r--   0        0        0   499714 2023-05-08 14:10:56.413538 mkdocs_exporter-1.0.0/mkdocs_exporter/resources/js/pagedjs.min.js
+-rw-r--r--   0        0        0     1214 2023-05-08 17:28:56.733567 mkdocs_exporter-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     4007 1970-01-01 00:00:00.000000 mkdocs_exporter-1.0.0/PKG-INFO
```

### Comparing `mkdocs_exporter-0.0.2/LICENSE` & `mkdocs_exporter-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-0.0.2/README.md` & `mkdocs_exporter-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-0.0.2/mkdocs_exporter/browser.py` & `mkdocs_exporter-1.0.0/mkdocs_exporter/browser.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-0.0.2/mkdocs_exporter/plugin.py` & `mkdocs_exporter-1.0.0/mkdocs_exporter/plugin.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-0.0.2/mkdocs_exporter/plugins/extras/config.py` & `mkdocs_exporter-1.0.0/mkdocs_exporter/plugins/extras/config.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-0.0.2/mkdocs_exporter/plugins/extras/plugin.py` & `mkdocs_exporter-1.0.0/mkdocs_exporter/plugins/extras/plugin.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-0.0.2/mkdocs_exporter/plugins/pdf/button.py` & `mkdocs_exporter-1.0.0/mkdocs_exporter/plugins/pdf/button.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-0.0.2/mkdocs_exporter/plugins/pdf/config.py` & `mkdocs_exporter-1.0.0/mkdocs_exporter/plugins/pdf/config.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-0.0.2/mkdocs_exporter/plugins/pdf/plugin.py` & `mkdocs_exporter-1.0.0/mkdocs_exporter/plugins/pdf/plugin.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-0.0.2/mkdocs_exporter/plugins/pdf/renderer.py` & `mkdocs_exporter-1.0.0/mkdocs_exporter/plugins/pdf/renderer.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-0.0.2/mkdocs_exporter/preprocessor.py` & `mkdocs_exporter-1.0.0/mkdocs_exporter/preprocessor.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-0.0.2/mkdocs_exporter/resources/js/pagedjs.min.js` & `mkdocs_exporter-1.0.0/mkdocs_exporter/resources/js/pagedjs.min.js`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-0.0.2/pyproject.toml` & `mkdocs_exporter-1.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "mkdocs-exporter"
-version = "0.0.2"
+version = "1.0.0"
 repository = "https://github.com/adrienbrignon/mkdocs-exporter"
 keywords = ["mkdocs", "pdf", "exporter"]
 description = "A highly-configurable plugin for MkDocs that exports your pages to PDF files."
 authors = ["Adrien Brignon <adrien@brignon.dev>"]
 readme = "README.md"
 classifiers = [
   "License :: OSI Approved :: MIT License",
```

### Comparing `mkdocs_exporter-0.0.2/PKG-INFO` & `mkdocs_exporter-1.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-exporter
-Version: 0.0.2
+Version: 1.0.0
 Summary: A highly-configurable plugin for MkDocs that exports your pages to PDF files.
 Home-page: https://github.com/adrienbrignon/mkdocs-exporter
 Keywords: mkdocs,pdf,exporter
 Author: Adrien Brignon
 Author-email: adrien@brignon.dev
 Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: MIT License
```

