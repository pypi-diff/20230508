# Comparing `tmp/lcacollect_config-1.3.3.tar.gz` & `tmp/lcacollect_config-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lcacollect_config-1.3.3.tar", max compression
+gzip compressed data, was "lcacollect_config-1.4.0.tar", max compression
```

## Comparing `lcacollect_config-1.3.3.tar` & `lcacollect_config-1.4.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1030 2023-04-17 13:14:21.424693 lcacollect_config-1.3.3/README.md
--rw-r--r--   0        0        0     2152 2023-04-17 13:14:21.424693 lcacollect_config-1.3.3/pyproject.toml
--rw-r--r--   0        0        0       22 2023-04-17 13:14:21.424693 lcacollect_config-1.3.3/src/lcacollect_config/__init__.py
--rw-r--r--   0        0        0     1882 2023-04-17 13:14:21.424693 lcacollect_config-1.3.3/src/lcacollect_config/config.py
--rw-r--r--   0        0        0     1507 2023-04-17 13:14:21.424693 lcacollect_config-1.3.3/src/lcacollect_config/connection.py
--rw-r--r--   0        0        0      372 2023-04-17 13:14:21.424693 lcacollect_config-1.3.3/src/lcacollect_config/context.py
--rw-r--r--   0        0        0      217 2023-04-17 13:14:21.424693 lcacollect_config-1.3.3/src/lcacollect_config/exceptions.py
--rw-r--r--   0        0        0      637 2023-04-17 13:14:21.424693 lcacollect_config-1.3.3/src/lcacollect_config/fastapi.py
--rw-r--r--   0        0        0      597 2023-04-17 13:14:21.424693 lcacollect_config-1.3.3/src/lcacollect_config/formatting.py
--rw-r--r--   0        0        0        0 2023-04-17 13:14:21.424693 lcacollect_config-1.3.3/src/lcacollect_config/graphql/__init__.py
--rw-r--r--   0        0        0     2772 2023-04-17 13:14:21.424693 lcacollect_config-1.3.3/src/lcacollect_config/graphql/input_filters.py
--rw-r--r--   0        0        0     1270 2023-04-17 13:14:21.424693 lcacollect_config-1.3.3/src/lcacollect_config/graphql/pagination.py
--rw-r--r--   0        0        0      400 2023-04-17 13:14:21.424693 lcacollect_config-1.3.3/src/lcacollect_config/permissions.py
--rw-r--r--   0        0        0     1043 2023-04-17 13:14:21.424693 lcacollect_config-1.3.3/src/lcacollect_config/router.py
--rw-r--r--   0        0        0      535 2023-04-17 13:14:21.424693 lcacollect_config-1.3.3/src/lcacollect_config/security.py
--rw-r--r--   0        0        0     2634 2023-04-17 13:14:21.424693 lcacollect_config-1.3.3/src/lcacollect_config/validate.py
--rw-r--r--   0        0        0     2079 1970-01-01 00:00:00.000000 lcacollect_config-1.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1030 2023-05-08 13:39:19.327618 lcacollect_config-1.4.0/README.md
+-rw-r--r--   0        0        0     2220 2023-05-08 13:39:19.327618 lcacollect_config-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-05-08 13:39:19.327618 lcacollect_config-1.4.0/src/lcacollect_config/__init__.py
+-rw-r--r--   0        0        0     1882 2023-05-08 13:39:19.327618 lcacollect_config-1.4.0/src/lcacollect_config/config.py
+-rw-r--r--   0        0        0     1507 2023-05-08 13:39:19.327618 lcacollect_config-1.4.0/src/lcacollect_config/connection.py
+-rw-r--r--   0        0        0      372 2023-05-08 13:39:19.327618 lcacollect_config-1.4.0/src/lcacollect_config/context.py
+-rw-r--r--   0        0        0      217 2023-05-08 13:39:19.327618 lcacollect_config-1.4.0/src/lcacollect_config/exceptions.py
+-rw-r--r--   0        0        0      637 2023-05-08 13:39:19.327618 lcacollect_config-1.4.0/src/lcacollect_config/fastapi.py
+-rw-r--r--   0        0        0      597 2023-05-08 13:39:19.327618 lcacollect_config-1.4.0/src/lcacollect_config/formatting.py
+-rw-r--r--   0        0        0        0 2023-05-08 13:39:19.327618 lcacollect_config-1.4.0/src/lcacollect_config/graphql/__init__.py
+-rw-r--r--   0        0        0     2772 2023-05-08 13:39:19.327618 lcacollect_config-1.4.0/src/lcacollect_config/graphql/input_filters.py
+-rw-r--r--   0        0        0     1270 2023-05-08 13:39:19.327618 lcacollect_config-1.4.0/src/lcacollect_config/graphql/pagination.py
+-rw-r--r--   0        0        0      400 2023-05-08 13:39:19.327618 lcacollect_config-1.4.0/src/lcacollect_config/permissions.py
+-rw-r--r--   0        0        0     1043 2023-05-08 13:39:19.327618 lcacollect_config-1.4.0/src/lcacollect_config/router.py
+-rw-r--r--   0        0        0      535 2023-05-08 13:39:19.327618 lcacollect_config-1.4.0/src/lcacollect_config/security.py
+-rw-r--r--   0        0        0     2634 2023-05-08 13:39:19.327618 lcacollect_config-1.4.0/src/lcacollect_config/validate.py
+-rw-r--r--   0        0        0     2038 1970-01-01 00:00:00.000000 lcacollect_config-1.4.0/PKG-INFO
```

### Comparing `lcacollect_config-1.3.3/README.md` & `lcacollect_config-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `lcacollect_config-1.3.3/pyproject.toml` & `lcacollect_config-1.4.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "lcacollect-config"
-version = "1.3.3"
+version = "1.4.0"
 description = "This package contains shared config and utils to be used across LCAcollect backends."
 authors = ["Christian Kongsgaard <chrk@arkitema.com>"]
 repository = "https://github.com/lcacollect/shared-config-backend"
 license = "LGPL-3.0-or-later"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "^3.11"
 pydantic = "*"
 strawberry-graphql = {extras = ["fastapi"], version = ">=0.164.0"}
-fastapi-azure-auth = "*"
+fastapi-azure-auth = ">=4.0.0"
 aiocache = "*"
 SQLAlchemy = {version = ">=1.4.35", extras = ["asyncio"], optional = true}
 sqlmodel = {version = ">=0.0.8", optional = true }
 asyncpg = {version = "^0.26.0", optional = true }
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.0"
@@ -37,15 +37,20 @@
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 120
-target-version = ['py310']
+target-version = ['py311']
+
+[tool.isort]
+profile = "black"
+src_paths = ["src", "tests"]
+
 
 [tool.pytest.ini_options]
 addopts = "--cov=src --cov-report=term-missing --cov-branch --cov-report=xml"
 asyncio_mode = "auto"
 console_output_style = "count"
 pythonpath = "src"
 required_plugins = ["pytest-cov>=4.0.0", "pytest-azurepipelines"]
```

### Comparing `lcacollect_config-1.3.3/src/lcacollect_config/config.py` & `lcacollect_config-1.4.0/src/lcacollect_config/config.py`

 * *Files identical despite different names*

### Comparing `lcacollect_config-1.3.3/src/lcacollect_config/connection.py` & `lcacollect_config-1.4.0/src/lcacollect_config/connection.py`

 * *Files identical despite different names*

### Comparing `lcacollect_config-1.3.3/src/lcacollect_config/fastapi.py` & `lcacollect_config-1.4.0/src/lcacollect_config/fastapi.py`

 * *Files identical despite different names*

### Comparing `lcacollect_config-1.3.3/src/lcacollect_config/formatting.py` & `lcacollect_config-1.4.0/src/lcacollect_config/formatting.py`

 * *Files identical despite different names*

### Comparing `lcacollect_config-1.3.3/src/lcacollect_config/graphql/input_filters.py` & `lcacollect_config-1.4.0/src/lcacollect_config/graphql/input_filters.py`

 * *Files identical despite different names*

### Comparing `lcacollect_config-1.3.3/src/lcacollect_config/graphql/pagination.py` & `lcacollect_config-1.4.0/src/lcacollect_config/graphql/pagination.py`

 * *Files identical despite different names*

### Comparing `lcacollect_config-1.3.3/src/lcacollect_config/router.py` & `lcacollect_config-1.4.0/src/lcacollect_config/router.py`

 * *Files identical despite different names*

### Comparing `lcacollect_config-1.3.3/src/lcacollect_config/security.py` & `lcacollect_config-1.4.0/src/lcacollect_config/security.py`

 * *Files identical despite different names*

### Comparing `lcacollect_config-1.3.3/src/lcacollect_config/validate.py` & `lcacollect_config-1.4.0/src/lcacollect_config/validate.py`

 * *Files identical despite different names*

### Comparing `lcacollect_config-1.3.3/PKG-INFO` & `lcacollect_config-1.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: lcacollect-config
-Version: 1.3.3
+Version: 1.4.0
 Summary: This package contains shared config and utils to be used across LCAcollect backends.
 Home-page: https://github.com/lcacollect/shared-config-backend
 License: LGPL-3.0-or-later
 Author: Christian Kongsgaard
 Author-email: chrk@arkitema.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: database
 Requires-Dist: SQLAlchemy[asyncio] (>=1.4.35) ; extra == "database"
 Requires-Dist: aiocache
 Requires-Dist: asyncpg (>=0.26.0,<0.27.0) ; extra == "database"
-Requires-Dist: fastapi-azure-auth
+Requires-Dist: fastapi-azure-auth (>=4.0.0)
 Requires-Dist: pydantic
 Requires-Dist: sqlmodel (>=0.0.8) ; extra == "database"
 Requires-Dist: strawberry-graphql[fastapi] (>=0.164.0)
 Project-URL: Repository, https://github.com/lcacollect/shared-config-backend
 Description-Content-Type: text/markdown
 
 # LCAcollect Shared Config Package
```

