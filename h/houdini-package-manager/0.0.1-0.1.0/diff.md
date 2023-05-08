# Comparing `tmp/houdini_package_manager-0.0.1.tar.gz` & `tmp/houdini_package_manager-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "houdini_package_manager-0.0.1.tar", max compression
+gzip compressed data, was "houdini_package_manager-0.1.0.tar", max compression
```

## Comparing `houdini_package_manager-0.0.1.tar` & `houdini_package_manager-0.1.0.tar`

### file list

```diff
@@ -1,7 +1,45 @@
--rw-r--r--   0        0        0     1543 2023-02-21 00:17:52.544536 houdini_package_manager-0.0.1/LICENSE
--rw-r--r--   0        0        0     1232 2023-02-21 00:17:52.544536 houdini_package_manager-0.0.1/README.md
--rw-r--r--   0        0        0        0 2023-02-21 00:17:52.544536 houdini_package_manager-0.0.1/houdini_package_manager/__init__.py
--rw-r--r--   0        0        0      267 2023-02-21 00:17:52.544536 houdini_package_manager-0.0.1/houdini_package_manager/foo.py
--rw-r--r--   0        0        0     1893 2023-02-21 00:18:29.664509 houdini_package_manager-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1860 1970-01-01 00:00:00.000000 houdini_package_manager-0.0.1/setup.py
--rw-r--r--   0        0        0     1938 1970-01-01 00:00:00.000000 houdini_package_manager-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-05-08 08:57:40.345890 houdini_package_manager-0.1.0/LICENSE
+-rw-r--r--   0        0        0     1412 2023-05-08 08:57:40.345890 houdini_package_manager-0.1.0/README.md
+-rw-r--r--   0        0        0       22 2023-05-08 08:57:40.349890 houdini_package_manager-0.1.0/houdini_package_manager/__init__.py
+-rw-r--r--   0        0        0    60498 2023-05-08 08:57:40.349890 houdini_package_manager-0.1.0/houdini_package_manager/design/houdini_package_manager.xd
+-rw-r--r--   0        0        0    10421 2023-05-08 08:57:40.349890 houdini_package_manager-0.1.0/houdini_package_manager/design/icons/add_packages.svg
+-rw-r--r--   0        0        0    10424 2023-05-08 08:57:40.349890 houdini_package_manager-0.1.0/houdini_package_manager/design/icons/add_packages_hover.svg
+-rw-r--r--   0        0        0      803 2023-05-08 08:57:40.349890 houdini_package_manager-0.1.0/houdini_package_manager/design/icons/clear_selection.svg
+-rw-r--r--   0        0        0      800 2023-05-08 08:57:40.349890 houdini_package_manager-0.1.0/houdini_package_manager/design/icons/clear_selection_hover.svg
+-rw-r--r--   0        0        0      427 2023-05-08 08:57:40.349890 houdini_package_manager-0.1.0/houdini_package_manager/design/icons/delete.svg
+-rw-r--r--   0        0        0      424 2023-05-08 08:57:40.349890 houdini_package_manager-0.1.0/houdini_package_manager/design/icons/delete_hover.svg
+-rw-r--r--   0        0        0      455 2023-05-08 08:57:40.349890 houdini_package_manager-0.1.0/houdini_package_manager/design/icons/file.svg
+-rw-r--r--   0        0        0      452 2023-05-08 08:57:40.349890 houdini_package_manager-0.1.0/houdini_package_manager/design/icons/file_hover.svg
+-rw-r--r--   0        0        0      382 2023-05-08 08:57:40.349890 houdini_package_manager-0.1.0/houdini_package_manager/design/icons/folder.svg
+-rw-r--r--   0        0        0      379 2023-05-08 08:57:40.349890 houdini_package_manager-0.1.0/houdini_package_manager/design/icons/folder_hover.svg
+-rw-r--r--   0        0        0     1561 2023-05-08 08:57:40.349890 houdini_package_manager-0.1.0/houdini_package_manager/design/icons/hpm.svg
+-rw-r--r--   0        0        0      696 2023-05-08 08:57:40.349890 houdini_package_manager-0.1.0/houdini_package_manager/design/icons/invert_selection.svg
+-rw-r--r--   0        0        0      693 2023-05-08 08:57:40.349890 houdini_package_manager-0.1.0/houdini_package_manager/design/icons/invert_selection_hover.svg
+-rw-r--r--   0        0        0      323 2023-05-08 08:57:40.349890 houdini_package_manager-0.1.0/houdini_package_manager/design/icons/migrate.svg
+-rw-r--r--   0        0        0      320 2023-05-08 08:57:40.349890 houdini_package_manager-0.1.0/houdini_package_manager/design/icons/migrate_hover.svg
+-rw-r--r--   0        0        0     1455 2023-05-08 08:57:40.349890 houdini_package_manager-0.1.0/houdini_package_manager/design/icons/refresh.svg
+-rw-r--r--   0        0        0     1625 2023-05-08 08:57:40.349890 houdini_package_manager-0.1.0/houdini_package_manager/design/icons/refresh_all.svg
+-rw-r--r--   0        0        0     1622 2023-05-08 08:57:40.349890 houdini_package_manager-0.1.0/houdini_package_manager/design/icons/refresh_all_hover.svg
+-rw-r--r--   0        0        0     1452 2023-05-08 08:57:40.349890 houdini_package_manager-0.1.0/houdini_package_manager/design/icons/refresh_hover.svg
+-rw-r--r--   0        0        0      390 2023-05-08 08:57:40.349890 houdini_package_manager-0.1.0/houdini_package_manager/design/icons/remove_all_items.svg
+-rw-r--r--   0        0        0      387 2023-05-08 08:57:40.349890 houdini_package_manager-0.1.0/houdini_package_manager/design/icons/remove_all_items_hover.svg
+-rw-r--r--   0        0        0      484 2023-05-08 08:57:40.349890 houdini_package_manager-0.1.0/houdini_package_manager/design/icons/remove_item.svg
+-rw-r--r--   0        0        0      502 2023-05-08 08:57:40.349890 houdini_package_manager-0.1.0/houdini_package_manager/design/icons/remove_item_hover.svg
+-rw-r--r--   0        0        0      224 2023-05-08 08:57:40.349890 houdini_package_manager-0.1.0/houdini_package_manager/design/icons/toggle_off.svg
+-rw-r--r--   0        0        0      221 2023-05-08 08:57:40.349890 houdini_package_manager-0.1.0/houdini_package_manager/design/icons/toggle_off_hover.svg
+-rw-r--r--   0        0        0      334 2023-05-08 08:57:40.349890 houdini_package_manager-0.1.0/houdini_package_manager/design/icons/toggle_on.svg
+-rw-r--r--   0        0        0      331 2023-05-08 08:57:40.349890 houdini_package_manager-0.1.0/houdini_package_manager/design/icons/toggle_on_hover.svg
+-rw-r--r--   0        0        0      677 2023-05-08 08:57:40.349890 houdini_package_manager-0.1.0/houdini_package_manager/design/icons/warning.svg
+-rw-r--r--   0        0        0      680 2023-05-08 08:57:40.349890 houdini_package_manager-0.1.0/houdini_package_manager/design/icons/warning_hover.svg
+-rw-r--r--   0        0        0   332325 2023-05-08 08:57:40.349890 houdini_package_manager-0.1.0/houdini_package_manager/design/icons.ai
+-rw-r--r--   0        0        0     1049 2023-05-08 08:57:40.349890 houdini_package_manager-0.1.0/houdini_package_manager/main.py
+-rw-r--r--   0        0        0     1574 2023-05-08 08:57:40.349890 houdini_package_manager-0.1.0/houdini_package_manager/meta/meta_tools.py
+-rw-r--r--   0        0        0      655 2023-05-08 08:57:40.349890 houdini_package_manager-0.1.0/houdini_package_manager/widgets/actions.py
+-rw-r--r--   0        0        0     8216 2023-05-08 08:57:40.349890 houdini_package_manager-0.1.0/houdini_package_manager/widgets/add_packages_layout.py
+-rw-r--r--   0        0        0     3574 2023-05-08 08:57:40.349890 houdini_package_manager-0.1.0/houdini_package_manager/widgets/custom_widgets.py
+-rw-r--r--   0        0        0     3327 2023-05-08 08:57:40.349890 houdini_package_manager-0.1.0/houdini_package_manager/widgets/main_window.py
+-rw-r--r--   0        0        0    20868 2023-05-08 08:57:40.353890 houdini_package_manager-0.1.0/houdini_package_manager/widgets/packages_layout.py
+-rw-r--r--   0        0        0    12699 2023-05-08 08:57:40.353890 houdini_package_manager-0.1.0/houdini_package_manager/widgets/packages_table.py
+-rw-r--r--   0        0        0    27856 2023-05-08 08:57:40.353890 houdini_package_manager-0.1.0/houdini_package_manager/wrangle/config_control.py
+-rw-r--r--   0        0        0     2064 2023-05-08 08:58:21.909908 houdini_package_manager-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2159 1970-01-01 00:00:00.000000 houdini_package_manager-0.1.0/PKG-INFO
```

### Comparing `houdini_package_manager-0.0.1/README.md` & `houdini_package_manager-0.1.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+<p align="center">
+  <img width="125" src="https://raw.githubusercontent.com/ariffjeff/houdini-package-manager/main/docs/static/hpm.svg">
+</p style = "margin-bottom: 2rem;">
+
+---
+
 # houdini-package-manager
 
 [![Release](https://img.shields.io/github/v/release/ariffjeff/houdini-package-manager)](https://img.shields.io/github/v/release/ariffjeff/houdini-package-manager)
 [![Build status](https://img.shields.io/github/actions/workflow/status/ariffjeff/houdini-package-manager/main.yml?branch=main)](https://github.com/ariffjeff/houdini-package-manager/actions/workflows/main.yml?query=branch%3Amain)
 [![codecov](https://codecov.io/gh/ariffjeff/houdini-package-manager/branch/main/graph/badge.svg)](https://codecov.io/gh/ariffjeff/houdini-package-manager)
 [![Commit activity](https://img.shields.io/github/commit-activity/m/ariffjeff/houdini-package-manager)](https://img.shields.io/github/commit-activity/m/ariffjeff/houdini-package-manager)
 [![License](https://img.shields.io/github/license/ariffjeff/houdini-package-manager)](https://img.shields.io/github/license/ariffjeff/houdini-package-manager)
```

### Comparing `houdini_package_manager-0.0.1/pyproject.toml` & `houdini_package_manager-0.1.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,41 @@
 [tool.poetry]
 name = "houdini_package_manager"
-version = "0.0.1"
+version = "0.1.0"
 description = "GUI package manager for Houdini"
 authors = ["Ariff Jeff <fariffjeff@icloud.com>"]
 repository = "https://github.com/ariffjeff/houdini-package-manager"
 documentation = "https://ariffjeff.github.io/houdini-package-manager/"
 readme = "README.md"
 packages = [
   {include = "houdini_package_manager"}
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.8,<4.0"
+python = ">=3.8,<3.12"
+pyside6 = "^6.4.2"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.0"
 pytest-cov = "^4.0.0"
 deptry = "^0.6.4"
 mypy = "^0.981"
 pre-commit = "^2.20.0"
 tox = "^3.25.1"
+icespringpysidestubs-pyside6 = "^1.3.1"
+pyinstaller = "^5.8.0"
+black = "^23.3.0"
 
 [tool.poetry.group.docs.dependencies]
 mkdocs = "^1.4.2"
 mkdocs-material = "^8.5.10"
 mkdocstrings = {extras = ["python"], version = "^0.19.0"}
 
+[tool.poetry_bumpversion.file."houdini_package_manager/__init__.py"]
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 120
 target-version = ['py37']
```

### Comparing `houdini_package_manager-0.0.1/PKG-INFO` & `houdini_package_manager-0.1.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 Metadata-Version: 2.1
 Name: houdini-package-manager
-Version: 0.0.1
+Version: 0.1.0
 Summary: GUI package manager for Houdini
 Home-page: https://github.com/ariffjeff/houdini-package-manager
 Author: Ariff Jeff
 Author-email: fariffjeff@icloud.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: pyside6 (>=6.4.2,<7.0.0)
 Project-URL: Documentation, https://ariffjeff.github.io/houdini-package-manager/
 Project-URL: Repository, https://github.com/ariffjeff/houdini-package-manager
 Description-Content-Type: text/markdown
 
+<p align="center">
+  <img width="125" src="https://raw.githubusercontent.com/ariffjeff/houdini-package-manager/main/docs/static/hpm.svg">
+</p style = "margin-bottom: 2rem;">
+
+---
+
 # houdini-package-manager
 
 [![Release](https://img.shields.io/github/v/release/ariffjeff/houdini-package-manager)](https://img.shields.io/github/v/release/ariffjeff/houdini-package-manager)
 [![Build status](https://img.shields.io/github/actions/workflow/status/ariffjeff/houdini-package-manager/main.yml?branch=main)](https://github.com/ariffjeff/houdini-package-manager/actions/workflows/main.yml?query=branch%3Amain)
 [![codecov](https://codecov.io/gh/ariffjeff/houdini-package-manager/branch/main/graph/badge.svg)](https://codecov.io/gh/ariffjeff/houdini-package-manager)
 [![Commit activity](https://img.shields.io/github/commit-activity/m/ariffjeff/houdini-package-manager)](https://img.shields.io/github/commit-activity/m/ariffjeff/houdini-package-manager)
 [![License](https://img.shields.io/github/license/ariffjeff/houdini-package-manager)](https://img.shields.io/github/license/ariffjeff/houdini-package-manager)
```

