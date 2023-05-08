# Comparing `tmp/neuralpit-1.0.0.tar.gz` & `tmp/neuralpit-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "E:\git\NeuralPit\neuralpit-api\dist\.tmp-gxybqyq5\neuralpit-1.0.0.tar", last modified: Mon May  8 02:39:03 2023, max compression
+gzip compressed data, was "neuralpit-1.0.1.tar", last modified: Mon May  8 14:25:37 2023, max compression
```

## Comparing `neuralpit-1.0.0.tar` & `neuralpit-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 02:39:03.000000 neuralpit-1.0.0/
--rw-rw-rw-   0        0        0       39 2023-05-08 02:31:41.000000 neuralpit-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0      400 2023-05-08 02:39:03.000000 neuralpit-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1072 2023-05-08 02:28:21.000000 neuralpit-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-08 02:39:03.000000 neuralpit-1.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-08 02:39:03.000000 neuralpit-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-08 02:39:03.000000 neuralpit-1.0.0/src/api/
--rw-rw-rw-   0        0        0       82 2023-05-08 01:41:31.000000 neuralpit-1.0.0/src/api/__init__.py
--rw-rw-rw-   0        0        0       58 2023-05-08 01:39:54.000000 neuralpit-1.0.0/src/api/client.py
--rw-rw-rw-   0        0        0        0 2023-05-08 01:40:45.000000 neuralpit-1.0.0/src/api/config.toml
-drwxrwxrwx   0        0        0        0 2023-05-08 02:39:03.000000 neuralpit-1.0.0/src/neuralpit.egg-info/
--rw-rw-rw-   0        0        0      400 2023-05-08 02:39:03.000000 neuralpit-1.0.0/src/neuralpit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      268 2023-05-08 02:39:03.000000 neuralpit-1.0.0/src/neuralpit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 02:39:03.000000 neuralpit-1.0.0/src/neuralpit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-05-08 02:39:03.000000 neuralpit-1.0.0/src/neuralpit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-05-08 02:39:03.000000 neuralpit-1.0.0/src/neuralpit.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 14:25:37.209286 neuralpit-1.0.1/
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-08 14:25:04.000000 neuralpit-1.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      520 2023-05-08 14:25:37.209286 neuralpit-1.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      130 2023-05-08 14:25:04.000000 neuralpit-1.0.1/README.md
+-rw-r--r--   0 root         (0) root         (0)      982 2023-05-08 14:25:04.000000 neuralpit-1.0.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-08 14:25:37.209286 neuralpit-1.0.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 14:25:37.209286 neuralpit-1.0.1/src/
+-rw-r--r--   0 root         (0) root         (0)       61 2023-05-08 14:25:04.000000 neuralpit-1.0.1/src/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 14:25:37.209286 neuralpit-1.0.1/src/chat/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 14:25:04.000000 neuralpit-1.0.1/src/chat/config.toml
+-rw-r--r--   0 root         (0) root         (0)       59 2023-05-08 14:25:04.000000 neuralpit-1.0.1/src/chat/document.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 14:25:37.209286 neuralpit-1.0.1/src/neuralpit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      520 2023-05-08 14:25:37.000000 neuralpit-1.0.1/src/neuralpit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      278 2023-05-08 14:25:37.000000 neuralpit-1.0.1/src/neuralpit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-08 14:25:37.000000 neuralpit-1.0.1/src/neuralpit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-05-08 14:25:37.000000 neuralpit-1.0.1/src/neuralpit.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-05-08 14:25:37.000000 neuralpit-1.0.1/src/neuralpit.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `neuralpit-1.0.0/pyproject.toml` & `neuralpit-1.0.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,41 +1,37 @@
-# pyproject.toml
-
-[build-system]
-requires      = ["setuptools>=61.0.0", "wheel"]
-build-backend = "setuptools.build_meta"
-
-[project]
-name = "neuralpit"
-version = "1.0.0"
-description = "NeuralPit API"
-readme = "README.md"
-authors = [{ name = "Quang Nguyen", email = "quang.nguyen@neuralpit.com" }]
-license = { file = "LICENSE" }
-classifiers = [
-    "License :: OSI Approved :: MIT License",
-    "Programming Language :: Python",
-    "Programming Language :: Python :: 3",
-]
-keywords = ["api", "neural", "neuralpit"]
-dependencies = [
-]
-requires-python = ">=3.7"
-
-[project.optional-dependencies]
-dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
-
-[project.urls]
-
-[project.scripts]
-
-[tool.bumpver]
-current_version = "2023.1001-alpha"
-version_pattern = "YYYY.BUILD[-TAG]"
-commit_message = "bump version {old_version} -> {new_version}"
-commit = true
-tag = true
-push = true
-
-[tool.bumpver.file_patterns]
-"pyproject.toml" = ['current_version = "{version}"', 'version = "{version}"']
-"src/neuralpit/api/__init__.py" = ["{version}"]
+# pyproject.toml
+
+[build-system]
+requires      = ["setuptools>=61.0.0", "wheel"]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "neuralpit"
+version = "1.0.1"
+description = "NeuralPit API"
+readme = "README.md"
+authors = [{ name = "Quang Nguyen", email = "quang.nguyen@neuralpit.com" }]
+license = { file = "LICENSE" }
+classifiers = [
+    "License :: OSI Approved :: MIT License",
+    "Programming Language :: Python",
+    "Programming Language :: Python :: 3",
+]
+keywords = ["api", "neural", "neuralpit"]
+dependencies = [
+]
+requires-python = ">=3.7"
+
+[project.optional-dependencies]
+dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
+
+[tool.bumpver]
+current_version = "2023.1001-alpha"
+version_pattern = "YYYY.BUILD[-TAG]"
+commit_message = "bump version {old_version} -> {new_version}"
+commit = true
+tag = true
+push = true
+
+[tool.bumpver.file_patterns]
+"pyproject.toml" = ['current_version = "{version}"', 'version = "{version}"']
+"src/__init__.py" = ["{version}"]
```

