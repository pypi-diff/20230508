# Comparing `tmp/vidcardshare-0.1.0.tar.gz` & `tmp/vidcardshare-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vidcardshare-0.1.0.tar", max compression
+gzip compressed data, was "vidcardshare-0.1.1.tar", max compression
```

## Comparing `vidcardshare-0.1.0.tar` & `vidcardshare-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       60 2023-05-07 23:44:32.772934 vidcardshare-0.1.0/README.md
--rwxr-xr-x   0        0        0     3941 2023-05-07 21:37:59.860401 vidcardshare-0.1.0/assets/index.html.tpl
--rwxr-xr-x   0        0        0      759 2023-05-07 20:43:56.000000 vidcardshare-0.1.0/assets/script.js
--rwxr-xr-x   0        0        0     6496 2023-05-07 21:31:56.704323 vidcardshare-0.1.0/assets/style.css.tpl
--rw-r--r--   0        0        0      452 2023-05-07 23:58:06.944963 vidcardshare-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-07 21:15:03.156150 vidcardshare-0.1.0/vidcardshare/__init__.py
--rw-r--r--   0        0        0     6648 2023-05-07 23:41:17.416926 vidcardshare-0.1.0/vidcardshare/main.py
--rw-r--r--   0        0        0      520 1970-01-01 00:00:00.000000 vidcardshare-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       60 2023-05-07 23:44:32.772934 vidcardshare-0.1.1/README.md
+-rwxr-xr-x   0        0        0     3941 2023-05-07 21:37:59.860401 vidcardshare-0.1.1/assets/index.html.tpl
+-rwxr-xr-x   0        0        0      759 2023-05-07 20:43:56.000000 vidcardshare-0.1.1/assets/script.js
+-rwxr-xr-x   0        0        0     6496 2023-05-07 21:31:56.704323 vidcardshare-0.1.1/assets/style.css.tpl
+-rw-r--r--   0        0        0      521 2023-05-08 00:04:42.380973 vidcardshare-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-07 21:15:03.156150 vidcardshare-0.1.1/vidcardshare/__init__.py
+-rw-r--r--   0        0        0     6648 2023-05-07 23:41:17.416926 vidcardshare-0.1.1/vidcardshare/main.py
+-rw-r--r--   0        0        0      579 1970-01-01 00:00:00.000000 vidcardshare-0.1.1/PKG-INFO
```

### Comparing `vidcardshare-0.1.0/assets/index.html.tpl` & `vidcardshare-0.1.1/assets/index.html.tpl`

 * *Files identical despite different names*

### Comparing `vidcardshare-0.1.0/assets/script.js` & `vidcardshare-0.1.1/assets/script.js`

 * *Files identical despite different names*

### Comparing `vidcardshare-0.1.0/assets/style.css.tpl` & `vidcardshare-0.1.1/assets/style.css.tpl`

 * *Files identical despite different names*

### Comparing `vidcardshare-0.1.0/vidcardshare/main.py` & `vidcardshare-0.1.1/vidcardshare/main.py`

 * *Files identical despite different names*

### Comparing `vidcardshare-0.1.0/PKG-INFO` & `vidcardshare-0.1.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: vidcardshare
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
-Author: Your Name
-Author-email: you@example.com
+Home-page: https://github.com/arnos-stuff/vidcardshare.git
+Author: Arno V
+Author-email: bcda0276@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: pytube (>=15.0.0,<16.0.0)
 Requires-Dist: typer-tinydb (>=0.1.4,<0.2.0)
```

