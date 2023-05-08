# Comparing `tmp/oz_defender-0.0.2.tar.gz` & `tmp/oz_defender-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oz_defender-0.0.2.tar", max compression
+gzip compressed data, was "oz_defender-0.1.1.tar", max compression
```

## Comparing `oz_defender-0.0.2.tar` & `oz_defender-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1063 2023-04-17 14:22:35.535570 oz_defender-0.0.2/README.md
--rw-r--r--   0        0        0        0 2023-04-16 23:14:31.460410 oz_defender-0.0.2/oz_defender/__init__.py
--rw-r--r--   0        0        0        0 2023-04-16 23:14:31.460579 oz_defender-0.0.2/oz_defender/relay/__init__.py
--rw-r--r--   0        0        0     2764 2023-04-17 15:14:00.184602 oz_defender-0.0.2/oz_defender/relay/client.py
--rw-r--r--   0        0        0      167 2023-04-17 15:14:00.184950 oz_defender-0.0.2/oz_defender/relay/exceptions.py
--rw-r--r--   0        0        0      759 2023-04-17 15:22:38.886590 oz_defender-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1684 1970-01-01 00:00:00.000000 oz_defender-0.0.2/setup.py
--rw-r--r--   0        0        0     1679 1970-01-01 00:00:00.000000 oz_defender-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     2838 2023-05-08 16:26:30.652778 oz_defender-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-04-16 23:14:31.460410 oz_defender-0.1.1/oz_defender/__init__.py
+-rw-r--r--   0        0        0       38 2023-05-08 16:26:30.653406 oz_defender-0.1.1/oz_defender/relay/__init__.py
+-rw-r--r--   0        0        0     8378 2023-05-08 16:26:30.653938 oz_defender-0.1.1/oz_defender/relay/client.py
+-rw-r--r--   0        0        0      261 2023-05-08 16:26:30.654408 oz_defender-0.1.1/oz_defender/relay/exceptions.py
+-rw-r--r--   0        0        0      887 2023-05-08 16:27:45.770213 oz_defender-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3773 1970-01-01 00:00:00.000000 oz_defender-0.1.1/setup.py
+-rw-r--r--   0        0        0     3604 1970-01-01 00:00:00.000000 oz_defender-0.1.1/PKG-INFO
```

### Comparing `oz_defender-0.0.2/pyproject.toml` & `oz_defender-0.1.1/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [project]
 name = "oz-defender"
 description = "OpenZeppelin Defender API client"
 
 [tool.poetry]
 name = "oz-defender"
-version = "0.0.2"
+version = "0.1.1"
 description = ""
-authors = ["Franklin <contact@hellofranklin.co>"]
+authors = ["Franklin Developers <developers@hellofranklin.co>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/franklin-systems/oz-defender"
 repository = "https://github.com/franklin-systems/oz-defender"
 packages = [
     {include = "oz_defender"}
 ]
@@ -23,18 +23,23 @@
     "relayer",
     "gasless",
     "api",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
+requests = "^2.28.2"
+pycognito = "^2022.12.0"
+pytest-mock = "^3.10.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.3.1"
 
+[tool.poetry.scripts]
+test = "scripts:test"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
 profile = "black"
```

