# Comparing `tmp/motion_python-0.1.36.tar.gz` & `tmp/motion_python-0.1.37.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motion_python-0.1.36.tar", max compression
+gzip compressed data, was "motion_python-0.1.37.tar", max compression
```

## Comparing `motion_python-0.1.36.tar` & `motion_python-0.1.37.tar`

### file list

```diff
@@ -1,29 +1,8 @@
--rw-r--r--   0        0        0     3232 2023-04-20 00:28:04.015822 motion_python-0.1.36/README.md
--rw-r--r--   0        0        0      671 2023-04-20 00:28:04.019822 motion_python-0.1.36/motion/__init__.py
--rw-r--r--   0        0        0       80 2023-04-20 00:28:04.019822 motion_python-0.1.36/motion/api/__init__.py
--rw-r--r--   0        0        0     6684 2023-04-20 00:28:04.019822 motion_python-0.1.36/motion/api/api.py
--rw-r--r--   0        0        0      616 2023-04-20 00:28:04.019822 motion_python-0.1.36/motion/api/models.py
--rw-r--r--   0        0        0     4000 2023-04-20 00:28:04.019822 motion_python-0.1.36/motion/cli.py
--rw-r--r--   0        0        0    10092 2023-04-20 00:28:04.019822 motion_python-0.1.36/motion/client.py
--rw-r--r--   0        0        0    22261 2023-04-20 00:28:04.019822 motion_python-0.1.36/motion/cursor.py
--rw-r--r--   0        0        0    10037 2023-04-20 00:28:04.019822 motion_python-0.1.36/motion/entry.py
--rw-r--r--   0        0        0      214 2023-04-20 00:28:04.019822 motion_python-0.1.36/motion/examples/basic/mconfig.py
--rw-r--r--   0        0        0        0 2023-04-20 00:28:04.019822 motion_python-0.1.36/motion/examples/basic/schemas/__init__.py
--rw-r--r--   0        0        0        0 2023-04-20 00:28:04.019822 motion_python-0.1.36/motion/examples/basic/triggers/__init__.py
--rw-r--r--   0        0        0     1796 2023-04-20 00:28:04.019822 motion_python-0.1.36/motion/examples/cooking/dashboard.py
--rw-r--r--   0        0        0      388 2023-04-20 00:28:04.019822 motion_python-0.1.36/motion/examples/cooking/mconfig.py
--rw-r--r--   0        0        0       63 2023-04-20 00:28:04.019822 motion_python-0.1.36/motion/examples/cooking/requirements.txt
--rw-r--r--   0        0        0       73 2023-04-20 00:28:04.019822 motion_python-0.1.36/motion/examples/cooking/schemas/__init__.py
--rw-r--r--   0        0        0      398 2023-04-20 00:28:04.019822 motion_python-0.1.36/motion/examples/cooking/schemas/all.py
--rw-r--r--   0        0        0     1377 2023-04-20 00:28:04.019822 motion_python-0.1.36/motion/examples/cooking/test.py
--rw-r--r--   0        0        0      134 2023-04-20 00:28:04.019822 motion_python-0.1.36/motion/examples/cooking/triggers/__init__.py
--rw-r--r--   0        0        0     4617 2023-04-20 00:28:04.019822 motion_python-0.1.36/motion/examples/cooking/triggers/scrape.py
--rw-r--r--   0        0        0     5003 2023-04-20 00:28:04.019822 motion_python-0.1.36/motion/examples/cooking/triggers/search.py
--rw-r--r--   0        0        0     2975 2023-04-20 00:28:04.019822 motion_python-0.1.36/motion/routing.py
--rw-r--r--   0        0        0     3413 2023-04-20 00:28:04.019822 motion_python-0.1.36/motion/schema.py
--rw-r--r--   0        0        0    15114 2023-04-20 00:28:04.019822 motion_python-0.1.36/motion/store.py
--rw-r--r--   0        0        0     3746 2023-04-20 00:28:04.019822 motion_python-0.1.36/motion/task.py
--rw-r--r--   0        0        0     6058 2023-04-20 00:28:04.019822 motion_python-0.1.36/motion/trigger.py
--rw-r--r--   0        0        0     1892 2023-04-20 00:28:04.019822 motion_python-0.1.36/motion/utils.py
--rw-r--r--   0        0        0     1578 2023-04-20 00:28:24.264093 motion_python-0.1.36/pyproject.toml
--rw-r--r--   0        0        0     4355 1970-01-01 00:00:00.000000 motion_python-0.1.36/PKG-INFO
+-rw-r--r--   0        0        0     2752 2023-05-08 17:55:47.056983 motion_python-0.1.37/README.md
+-rw-r--r--   0        0        0      120 2023-05-08 17:55:47.060983 motion_python-0.1.37/motion/__init__.py
+-rw-r--r--   0        0        0    16074 2023-05-08 17:55:47.060983 motion_python-0.1.37/motion/component.py
+-rw-r--r--   0        0        0     6413 2023-05-08 17:55:47.060983 motion_python-0.1.37/motion/execute.py
+-rw-r--r--   0        0        0      595 2023-05-08 17:55:47.060983 motion_python-0.1.37/motion/route.py
+-rw-r--r--   0        0        0     3089 2023-05-08 17:55:47.060983 motion_python-0.1.37/motion/utils.py
+-rw-r--r--   0        0        0     1602 2023-05-08 17:56:11.377088 motion_python-0.1.37/pyproject.toml
+-rw-r--r--   0        0        0     3875 1970-01-01 00:00:00.000000 motion_python-0.1.37/PKG-INFO
```

### Comparing `motion_python-0.1.36/pyproject.toml` & `motion_python-0.1.37/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "motion-python"
-version = "0.1.36"
+version = "0.1.37"
 description = "A trigger-based framework for creating and executing ML pipelines."
 authors = ["Shreya Shankar <shreyashankar@berkeley.edu>"]
 readme = "README.md"
 packages = [{include = "motion"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
@@ -21,31 +21,32 @@
 httpx = "^0.23.3"
 python-multipart = "^0.0.6"
 pydantic = "^1.10.7"
 urllib3 = "^1.26.15"
 flask = "^2.2.3"
 rich = "^13.3.4"
 
-[tool.poetry.scripts]
-motion = "motion.cli:motioncli"
-
 [tool.poetry.group.dev.dependencies]
 poetry-types = "^0.3.5"
 pytest = "^7.2.2"
 mypy = "^1.1.1"
 coverage = {extras = ["toml"], version = "^7.2.3"}
 pre-commit = "^3.2.1"
 types-requests = "^2.28.11.16"
 types-croniter = "^1.3.2.7"
 mkdocs = "^1.4.2"
 mkdocs-terminal = "^4.2.0"
 mkdocs-material = "^9.1.5"
 mkdocstrings = {version="^0.20.0", extras = ["python"] }
 pytkdocs = "^0.16.1"
 linkchecker = "^10.2.1"
+ruff = "^0.0.261"
+maturin = "^0.14.17"
+mike = "^1.1.2"
+scikit-learn = "^1.2.2"
 
 [tool.pytest.ini_options]
 testpaths = ["tests"]
 
 [tool.mypy]
 files = "motion"
 mypy_path = "motion"
```

