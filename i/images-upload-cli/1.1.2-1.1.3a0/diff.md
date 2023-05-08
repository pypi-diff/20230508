# Comparing `tmp/images_upload_cli-1.1.2.tar.gz` & `tmp/images_upload_cli-1.1.3a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "images_upload_cli-1.1.2.tar", max compression
+gzip compressed data, was "images_upload_cli-1.1.3a0.tar", max compression
```

## Comparing `images_upload_cli-1.1.2.tar` & `images_upload_cli-1.1.3a0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1065 2023-05-07 15:05:36.626482 images_upload_cli-1.1.2/LICENSE
--rw-r--r--   0        0        0     5248 2023-05-07 15:05:36.626482 images_upload_cli-1.1.2/README.md
--rw-r--r--   0        0        0     2506 2023-05-07 15:05:49.410492 images_upload_cli-1.1.2/pyproject.toml
--rwxr-xr-x   0        0        0      188 2023-05-07 15:05:36.626482 images_upload_cli-1.1.2/src/images_upload_cli/__init__.py
--rwxr-xr-x   0        0        0      178 2023-05-07 15:05:36.626482 images_upload_cli-1.1.2/src/images_upload_cli/__main__.py
--rwxr-xr-x   0        0        0     1710 2023-05-07 15:05:36.626482 images_upload_cli-1.1.2/src/images_upload_cli/cli.py
--rwxr-xr-x   0        0        0    11016 2023-05-07 15:05:36.626482 images_upload_cli-1.1.2/src/images_upload_cli/upload.py
--rwxr-xr-x   0        0        0     3057 2023-05-07 15:05:36.626482 images_upload_cli-1.1.2/src/images_upload_cli/util.py
--rw-r--r--   0        0        0     6213 1970-01-01 00:00:00.000000 images_upload_cli-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-08 18:36:04.824719 images_upload_cli-1.1.3a0/LICENSE
+-rw-r--r--   0        0        0     5248 2023-05-08 18:36:04.824719 images_upload_cli-1.1.3a0/README.md
+-rw-r--r--   0        0        0     2514 2023-05-08 18:36:18.724625 images_upload_cli-1.1.3a0/pyproject.toml
+-rwxr-xr-x   0        0        0      188 2023-05-08 18:36:04.824719 images_upload_cli-1.1.3a0/src/images_upload_cli/__init__.py
+-rwxr-xr-x   0        0        0      178 2023-05-08 18:36:04.824719 images_upload_cli-1.1.3a0/src/images_upload_cli/__main__.py
+-rwxr-xr-x   0        0        0     1710 2023-05-08 18:36:04.824719 images_upload_cli-1.1.3a0/src/images_upload_cli/cli.py
+-rwxr-xr-x   0        0        0    11016 2023-05-08 18:36:04.824719 images_upload_cli-1.1.3a0/src/images_upload_cli/upload.py
+-rwxr-xr-x   0        0        0     3057 2023-05-08 18:36:04.824719 images_upload_cli-1.1.3a0/src/images_upload_cli/util.py
+-rw-r--r--   0        0        0     6215 1970-01-01 00:00:00.000000 images_upload_cli-1.1.3a0/PKG-INFO
```

### Comparing `images_upload_cli-1.1.2/LICENSE` & `images_upload_cli-1.1.3a0/LICENSE`

 * *Files identical despite different names*

### Comparing `images_upload_cli-1.1.2/README.md` & `images_upload_cli-1.1.3a0/README.md`

 * *Files identical despite different names*

### Comparing `images_upload_cli-1.1.2/pyproject.toml` & `images_upload_cli-1.1.3a0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry]
 name = "images-upload-cli"
-version = "1.1.2"
+version = "1.1.3-alpha.0"
 description = "Upload images via APIs"
 authors = ["DeadNews <aurczpbgr@mozmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/DeadNews/images-upload-cli"
 repository = "https://github.com/DeadNews/images-upload-cli"
 keywords = ["cli", "imgur", "image-upload", "upload-images", "upload-pictures"]
```

### Comparing `images_upload_cli-1.1.2/src/images_upload_cli/cli.py` & `images_upload_cli-1.1.3a0/src/images_upload_cli/cli.py`

 * *Files identical despite different names*

### Comparing `images_upload_cli-1.1.2/src/images_upload_cli/upload.py` & `images_upload_cli-1.1.3a0/src/images_upload_cli/upload.py`

 * *Files identical despite different names*

### Comparing `images_upload_cli-1.1.2/src/images_upload_cli/util.py` & `images_upload_cli-1.1.3a0/src/images_upload_cli/util.py`

 * *Files identical despite different names*

### Comparing `images_upload_cli-1.1.2/PKG-INFO` & `images_upload_cli-1.1.3a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: images-upload-cli
-Version: 1.1.2
+Version: 1.1.3a0
 Summary: Upload images via APIs
 Home-page: https://github.com/DeadNews/images-upload-cli
 License: MIT
 Keywords: cli,imgur,image-upload,upload-images,upload-pictures
 Author: DeadNews
 Author-email: aurczpbgr@mozmail.com
 Requires-Python: >=3.8.1,<4.0.0
```

