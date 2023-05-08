# Comparing `tmp/badgie-0.8.0.tar.gz` & `tmp/badgie-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "badgie-0.8.0.tar", last modified: Fri May  5 06:33:34 2023, max compression
+gzip compressed data, was "badgie-0.9.0.tar", last modified: Mon May  8 08:16:12 2023, max compression
```

## Comparing `badgie-0.8.0.tar` & `badgie-0.9.0.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 06:33:34.547295 badgie-0.8.0/
--rw-rw-rw-   0 root         (0) root         (0)     1069 2023-05-05 06:33:29.000000 badgie-0.8.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3315 2023-05-05 06:33:34.547295 badgie-0.8.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2333 2023-05-05 06:33:29.000000 badgie-0.8.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 06:33:34.542295 badgie-0.8.0/badgie/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-05 06:33:29.000000 badgie-0.8.0/badgie/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       61 2023-05-05 06:33:29.000000 badgie-0.8.0/badgie/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-05-05 06:33:31.000000 badgie-0.8.0/badgie/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 06:33:34.545295 badgie-0.8.0/badgie/badges/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-05 06:33:29.000000 badgie-0.8.0/badgie/badges/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      316 2023-05-05 06:33:29.000000 badgie-0.8.0/badgie/badges/_base.py
--rw-rw-rw-   0 root         (0) root         (0)      828 2023-05-05 06:33:29.000000 badgie-0.8.0/badgie/badges/brettops.py
--rw-rw-rw-   0 root         (0) root         (0)      953 2023-05-05 06:33:29.000000 badgie-0.8.0/badgie/badges/codestyle.py
--rw-rw-rw-   0 root         (0) root         (0)     1526 2023-05-05 06:33:29.000000 badgie-0.8.0/badgie/badges/gitlab.py
--rw-rw-rw-   0 root         (0) root         (0)      595 2023-05-05 06:33:29.000000 badgie-0.8.0/badgie/badges/precommit.py
--rw-rw-rw-   0 root         (0) root         (0)     6403 2023-05-05 06:33:29.000000 badgie-0.8.0/badgie/cli.py
--rw-rw-rw-   0 root         (0) root         (0)      131 2023-05-05 06:33:29.000000 badgie-0.8.0/badgie/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 06:33:34.547295 badgie-0.8.0/badgie/finders/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-05 06:33:29.000000 badgie-0.8.0/badgie/finders/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1177 2023-05-05 06:33:29.000000 badgie-0.8.0/badgie/finders/files.py
--rw-rw-rw-   0 root         (0) root         (0)     2386 2023-05-05 06:33:29.000000 badgie-0.8.0/badgie/finders/gitlab.py
--rw-rw-rw-   0 root         (0) root         (0)      990 2023-05-05 06:33:29.000000 badgie-0.8.0/badgie/finders/pre_commit_config.py
--rw-rw-rw-   0 root         (0) root         (0)     1441 2023-05-05 06:33:29.000000 badgie-0.8.0/badgie/finders/remotes.py
--rw-rw-rw-   0 root         (0) root         (0)     2271 2023-05-05 06:33:29.000000 badgie-0.8.0/badgie/models.py
--rw-rw-rw-   0 root         (0) root         (0)     1486 2023-05-05 06:33:29.000000 badgie-0.8.0/badgie/parser.py
--rw-rw-rw-   0 root         (0) root         (0)     1997 2023-05-05 06:33:29.000000 badgie-0.8.0/badgie/project.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-05 06:33:29.000000 badgie-0.8.0/badgie/py.typed
--rw-rw-rw-   0 root         (0) root         (0)     1647 2023-05-05 06:33:29.000000 badgie-0.8.0/badgie/tokens.py
--rw-rw-rw-   0 root         (0) root         (0)      687 2023-05-05 06:33:29.000000 badgie-0.8.0/badgie/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 06:33:34.544295 badgie-0.8.0/badgie.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3315 2023-05-05 06:33:34.000000 badgie-0.8.0/badgie.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      701 2023-05-05 06:33:34.000000 badgie-0.8.0/badgie.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-05 06:33:34.000000 badgie-0.8.0/badgie.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2023-05-05 06:33:34.000000 badgie-0.8.0/badgie.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       37 2023-05-05 06:33:34.000000 badgie-0.8.0/badgie.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-05-05 06:33:34.000000 badgie-0.8.0/badgie.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       63 2023-05-05 06:33:34.548296 badgie-0.8.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1525 2023-05-05 06:33:31.000000 badgie-0.8.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:16:12.040140 badgie-0.9.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1069 2023-05-08 08:16:07.000000 badgie-0.9.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3315 2023-05-08 08:16:12.040140 badgie-0.9.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2333 2023-05-08 08:16:07.000000 badgie-0.9.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:16:12.034140 badgie-0.9.0/badgie/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-08 08:16:07.000000 badgie-0.9.0/badgie/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       61 2023-05-08 08:16:07.000000 badgie-0.9.0/badgie/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-05-08 08:16:09.000000 badgie-0.9.0/badgie/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:16:12.039140 badgie-0.9.0/badgie/badges/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-08 08:16:07.000000 badgie-0.9.0/badgie/badges/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      316 2023-05-08 08:16:07.000000 badgie-0.9.0/badgie/badges/_base.py
+-rw-rw-rw-   0 root         (0) root         (0)      828 2023-05-08 08:16:07.000000 badgie-0.9.0/badgie/badges/brettops.py
+-rw-rw-rw-   0 root         (0) root         (0)     1526 2023-05-08 08:16:07.000000 badgie-0.9.0/badgie/badges/gitlab.py
+-rw-rw-rw-   0 root         (0) root         (0)      595 2023-05-08 08:16:07.000000 badgie-0.9.0/badgie/badges/precommit.py
+-rw-rw-rw-   0 root         (0) root         (0)      539 2023-05-08 08:16:07.000000 badgie-0.9.0/badgie/badges/prettier.py
+-rw-rw-rw-   0 root         (0) root         (0)     2352 2023-05-08 08:16:07.000000 badgie-0.9.0/badgie/badges/python.py
+-rw-rw-rw-   0 root         (0) root         (0)     6403 2023-05-08 08:16:07.000000 badgie-0.9.0/badgie/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      131 2023-05-08 08:16:07.000000 badgie-0.9.0/badgie/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:16:12.040140 badgie-0.9.0/badgie/finders/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-08 08:16:07.000000 badgie-0.9.0/badgie/finders/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1177 2023-05-08 08:16:07.000000 badgie-0.9.0/badgie/finders/files.py
+-rw-rw-rw-   0 root         (0) root         (0)     2386 2023-05-08 08:16:07.000000 badgie-0.9.0/badgie/finders/gitlab.py
+-rw-rw-rw-   0 root         (0) root         (0)     1546 2023-05-08 08:16:07.000000 badgie-0.9.0/badgie/finders/pre_commit_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     1441 2023-05-08 08:16:07.000000 badgie-0.9.0/badgie/finders/remotes.py
+-rw-rw-rw-   0 root         (0) root         (0)     2177 2023-05-08 08:16:07.000000 badgie-0.9.0/badgie/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     1486 2023-05-08 08:16:07.000000 badgie-0.9.0/badgie/parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     2052 2023-05-08 08:16:07.000000 badgie-0.9.0/badgie/project.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-08 08:16:07.000000 badgie-0.9.0/badgie/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)     1751 2023-05-08 08:16:07.000000 badgie-0.9.0/badgie/tokens.py
+-rw-rw-rw-   0 root         (0) root         (0)      687 2023-05-08 08:16:07.000000 badgie-0.9.0/badgie/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 08:16:12.036140 badgie-0.9.0/badgie.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3315 2023-05-08 08:16:12.000000 badgie-0.9.0/badgie.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      724 2023-05-08 08:16:12.000000 badgie-0.9.0/badgie.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-08 08:16:12.000000 badgie-0.9.0/badgie.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-05-08 08:16:12.000000 badgie-0.9.0/badgie.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       37 2023-05-08 08:16:12.000000 badgie-0.9.0/badgie.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-05-08 08:16:12.000000 badgie-0.9.0/badgie.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       63 2023-05-08 08:16:12.041140 badgie-0.9.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1525 2023-05-08 08:16:09.000000 badgie-0.9.0/setup.py
```

### Comparing `badgie-0.8.0/LICENSE` & `badgie-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `badgie-0.8.0/PKG-INFO` & `badgie-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: badgie
-Version: 0.8.0
+Version: 0.9.0
 Summary: Add all the badges with Badgie!
 Home-page: https://gitlab.com/brettops/tools/badgie
 Author: Brett Weir
 Author-email: brett@brettops.io
 License: MIT
 Keywords: badge,template,markdown
 Platform: UNKNOWN
```

### Comparing `badgie-0.8.0/README.md` & `badgie-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `badgie-0.8.0/badgie/badges/brettops.py` & `badgie-0.9.0/badgie/badges/brettops.py`

 * *Files identical despite different names*

### Comparing `badgie-0.8.0/badgie/badges/gitlab.py` & `badgie-0.9.0/badgie/badges/gitlab.py`

 * *Files identical despite different names*

### Comparing `badgie-0.8.0/badgie/badges/precommit.py` & `badgie-0.9.0/badgie/badges/precommit.py`

 * *Files identical despite different names*

### Comparing `badgie-0.8.0/badgie/cli.py` & `badgie-0.9.0/badgie/cli.py`

 * *Files identical despite different names*

### Comparing `badgie-0.8.0/badgie/finders/files.py` & `badgie-0.9.0/badgie/finders/files.py`

 * *Files identical despite different names*

### Comparing `badgie-0.8.0/badgie/finders/gitlab.py` & `badgie-0.9.0/badgie/finders/gitlab.py`

 * *Files identical despite different names*

### Comparing `badgie-0.8.0/badgie/finders/pre_commit_config.py` & `badgie-0.9.0/badgie/finders/pre_commit_config.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,14 +4,27 @@
 from ..models import Context, Hook, HookMatch
 
 HOOKS = {
     HookMatch(
         repo="https://github.com/pre-commit/mirrors-prettier/", hook="prettier"
     ): {to.PRETTIER},
     HookMatch(repo="https://github.com/psf/black/", hook="black"): {to.PYTHON_BLACK},
+    HookMatch(repo="https://github.com/PyCQA/bandit/", hook="bandit"): {
+        to.PYTHON_BANDIT
+    },
+    HookMatch(repo="https://github.com/PyCQA/isort/", hook="isort"): {to.PYTHON_ISORT},
+    HookMatch(repo="https://github.com/PyCQA/docformatter/", hook="docformatter"): {
+        to.PYTHON_DOCFORMATTER
+    },
+    HookMatch(
+        repo="https://github.com/PyCQA/docformatter/", hook="docformatter-venv"
+    ): {to.PYTHON_DOCFORMATTER},
+    HookMatch(repo="https://github.com/pre-commit/mirrors-mypy/", hook="mypy"): {
+        to.PYTHON_MYPY
+    },
 }
 
 
 def normalize_url(url: str):
     url = url.strip()
     if not url.endswith("/"):
         url += "/"
```

### Comparing `badgie-0.8.0/badgie/finders/remotes.py` & `badgie-0.9.0/badgie/finders/remotes.py`

 * *Files identical despite different names*

### Comparing `badgie-0.8.0/badgie/models.py` & `badgie-0.9.0/badgie/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -98,17 +98,14 @@
 class Context:
     path: Path
 
     nodes: dict[str, list[Node]] = field(factory=dict)
     tokens_found: set[Node] = field(factory=set)
     tokens_processed: set[Node] = field(factory=set)
 
-    providers: dict[Node] = field(factory=dict)
-    badges: dict[Node] = field(factory=dict)
-
     def add_nodes(self, nodes):
         for node in nodes:
             for token in node.tokens:
                 self.nodes.setdefault(token, [])
                 self.nodes[token].append(node)
             self.tokens_found |= node.tokens
```

### Comparing `badgie-0.8.0/badgie/parser.py` & `badgie-0.9.0/badgie/parser.py`

 * *Files identical despite different names*

### Comparing `badgie-0.8.0/badgie/project.py` & `badgie-0.9.0/badgie/project.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import re
-import subprocess
+import subprocess  # nosec
 from pathlib import Path
 from typing import Optional
 
 from .models import ProjectRemote
 
 REMOTES = [
     r"(?P<user>git)@(?P<host>.*?):(?P<path>.*?)\.git",
@@ -30,15 +30,15 @@
 
 def get_project_remote(line) -> Optional[ProjectRemote]:
     name, parts = line.split("\t")
     url, type = parts.split(" ")
     type = type.replace("(", "").replace(")", "")
     match = match_remote_url(url)
     if not match:
-        return
+        return None
     return ProjectRemote(
         name=name,
         type=type,
         url=url,
         scheme=get_match_group(match, "scheme"),
         user=get_match_group(match, "user"),
         host=match.group("host"),
@@ -52,26 +52,28 @@
         remote = get_project_remote(line)
         remotes.setdefault(remote.name, {})
         remotes[remote.name][remote.type] = remote
     return remotes
 
 
 def get_project_remotes() -> dict[str, dict[str, ProjectRemote]]:
-    process = subprocess.run(["git", "remote", "-v"], text=True, capture_output=True)
+    process = subprocess.run(
+        ["git", "remote", "-v"], text=True, capture_output=True
+    )  # nosec
     return get_project_remotes_from_text(process.stdout)
 
 
 def get_project_paths() -> list[Path]:
     return [
         Path(path)
         for path in subprocess.run(
             ["git", "ls-files"], text=True, stdout=subprocess.PIPE
-        ).stdout.splitlines()
+        ).stdout.splitlines()  # nosec
     ]
 
 
 def get_project_root() -> Path:
     return Path(
         subprocess.run(
             ["git", "rev-parse", "--show-toplevel"], text=True, stdout=subprocess.PIPE
-        ).stdout.strip()
+        ).stdout.strip()  # nosec
     )
```

### Comparing `badgie-0.8.0/badgie/tokens.py` & `badgie-0.9.0/badgie/tokens.py`

 * *Files 16% similar despite different names*

```diff
@@ -38,17 +38,20 @@
 PYPI_LICENSE = "pypi_license"
 PYPI_PYTHON_VERSION = "pypi_python_version"
 PYPI_STATUS = "pypi_status"
 PYPI_VERSION = "pypi_version"
 PYPI_WHEEL = "pypi_wheel"
 
 PYTHON = "python"
+PYTHON_BANDIT = "python_bandit"
 PYTHON_BLACK = "python_black"
+PYTHON_DOCFORMATTER = "python_docformatter"
 PYTHON_IMPLEMENTATION = "python_implementation"
 PYTHON_ISORT = "python_isort"
+PYTHON_MYPY = "python_mypy"
 PYTHON_PYPROJECT_TOML = "python_pyproject_toml"
 PYTHON_SETUP_CFG = "python_setup_cfg"
 PYTHON_SETUPTOOLS = "python_setuptools"
 
 SHELL_SHFMT = "shell_shfmt"
 
 TERRAFORM = "terraform"
```

### Comparing `badgie-0.8.0/badgie/utils.py` & `badgie-0.9.0/badgie/utils.py`

 * *Files identical despite different names*

### Comparing `badgie-0.8.0/badgie.egg-info/PKG-INFO` & `badgie-0.9.0/badgie.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: badgie
-Version: 0.8.0
+Version: 0.9.0
 Summary: Add all the badges with Badgie!
 Home-page: https://gitlab.com/brettops/tools/badgie
 Author: Brett Weir
 Author-email: brett@brettops.io
 License: MIT
 Keywords: badge,template,markdown
 Platform: UNKNOWN
```

### Comparing `badgie-0.8.0/badgie.egg-info/SOURCES.txt` & `badgie-0.9.0/badgie.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -18,15 +18,16 @@
 badgie.egg-info/dependency_links.txt
 badgie.egg-info/entry_points.txt
 badgie.egg-info/requires.txt
 badgie.egg-info/top_level.txt
 badgie/badges/__init__.py
 badgie/badges/_base.py
 badgie/badges/brettops.py
-badgie/badges/codestyle.py
 badgie/badges/gitlab.py
 badgie/badges/precommit.py
+badgie/badges/prettier.py
+badgie/badges/python.py
 badgie/finders/__init__.py
 badgie/finders/files.py
 badgie/finders/gitlab.py
 badgie/finders/pre_commit_config.py
 badgie/finders/remotes.py
```

### Comparing `badgie-0.8.0/setup.py` & `badgie-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import find_packages, setup
 
 # injected version
-__version__ = "0.8.0"
+__version__ = "0.9.0"
 
 # markdown readme
 long_description = open("README.md").read()
 
 # read requirements from requirements.in
 install_requires = open("requirements.in").read().splitlines()
```

