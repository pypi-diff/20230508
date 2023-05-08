# Comparing `tmp/dxsp-2.0.5.tar.gz` & `tmp/dxsp-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-2.0.5.tar", max compression
+gzip compressed data, was "dxsp-2.0.6.tar", max compression
```

## Comparing `dxsp-2.0.5.tar` & `dxsp-2.0.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1064 2023-05-07 20:42:37.754900 dxsp-2.0.5/LICENSE
--rw-r--r--   0        0        0     3349 2023-05-07 20:42:37.754900 dxsp-2.0.5/README.md
--rw-r--r--   0        0        0       86 2023-05-07 20:42:38.446911 dxsp-2.0.5/dxsp/__init__.py
--rw-r--r--   0        0        0        1 2023-05-07 20:42:37.754900 dxsp-2.0.5/dxsp/assets/__init__.py
--rw-r--r--   0        0        0     8887 2023-05-07 20:42:37.754900 dxsp-2.0.5/dxsp/assets/blockchains.py
--rw-r--r--   0        0        0      388 2023-05-07 20:42:37.754900 dxsp-2.0.5/dxsp/config.py
--rw-r--r--   0        0        0     2967 2023-05-07 20:42:37.754900 dxsp-2.0.5/dxsp/default_settings.toml
--rw-r--r--   0        0        0    26307 2023-05-07 20:42:37.754900 dxsp-2.0.5/dxsp/main.py
--rw-r--r--   0        0        0     1790 2023-05-07 20:42:38.442911 dxsp-2.0.5/pyproject.toml
--rw-r--r--   0        0        0     4082 1970-01-01 00:00:00.000000 dxsp-2.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-08 06:37:53.863155 dxsp-2.0.6/LICENSE
+-rw-r--r--   0        0        0     3349 2023-05-08 06:37:53.863155 dxsp-2.0.6/README.md
+-rw-r--r--   0        0        0       86 2023-05-08 06:37:54.559162 dxsp-2.0.6/dxsp/__init__.py
+-rw-r--r--   0        0        0        1 2023-05-08 06:37:53.863155 dxsp-2.0.6/dxsp/assets/__init__.py
+-rw-r--r--   0        0        0     8887 2023-05-08 06:37:53.863155 dxsp-2.0.6/dxsp/assets/blockchains.py
+-rw-r--r--   0        0        0      388 2023-05-08 06:37:53.863155 dxsp-2.0.6/dxsp/config.py
+-rw-r--r--   0        0        0     2967 2023-05-08 06:37:53.863155 dxsp-2.0.6/dxsp/default_settings.toml
+-rw-r--r--   0        0        0    26307 2023-05-08 06:37:53.863155 dxsp-2.0.6/dxsp/main.py
+-rw-r--r--   0        0        0     1790 2023-05-08 06:37:54.559162 dxsp-2.0.6/pyproject.toml
+-rw-r--r--   0        0        0     4082 1970-01-01 00:00:00.000000 dxsp-2.0.6/PKG-INFO
```

### Comparing `dxsp-2.0.5/LICENSE` & `dxsp-2.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-2.0.5/README.md` & `dxsp-2.0.6/README.md`

 * *Files identical despite different names*

### Comparing `dxsp-2.0.5/dxsp/assets/blockchains.py` & `dxsp-2.0.6/dxsp/assets/blockchains.py`

 * *Files identical despite different names*

### Comparing `dxsp-2.0.5/dxsp/default_settings.toml` & `dxsp-2.0.6/dxsp/default_settings.toml`

 * *Files identical despite different names*

### Comparing `dxsp-2.0.5/dxsp/main.py` & `dxsp-2.0.6/dxsp/main.py`

 * *Files identical despite different names*

### Comparing `dxsp-2.0.5/pyproject.toml` & `dxsp-2.0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dxsp"
-version = "2.0.5"
+version = "2.0.6"
 description = "DXSP (DeX SwaP), A defi swap helper package. Swap made easy."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 
 
 [tool.poetry.urls]
```

### Comparing `dxsp-2.0.5/PKG-INFO` & `dxsp-2.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 2.0.5
+Version: 2.0.6
 Summary: DXSP (DeX SwaP), A defi swap helper package. Swap made easy.
 License: MIT
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

