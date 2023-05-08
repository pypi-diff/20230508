# Comparing `tmp/userfs-0.2.1.tar.gz` & `tmp/userfs-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "userfs-0.2.1.tar", last modified: Sun May  7 07:20:28 2023, max compression
+gzip compressed data, was "userfs-1.0.0.tar", last modified: Mon May  8 05:42:15 2023, max compression
```

## Comparing `userfs-0.2.1.tar` & `userfs-1.0.0.tar`

### file list

```diff
@@ -1,52 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 07:20:28.651212 userfs-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-07 07:19:20.000000 userfs-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-05-07 07:20:28.651212 userfs-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-05-07 07:19:20.000000 userfs-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-07 07:19:20.000000 userfs-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 07:20:28.651212 userfs-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-07 07:19:20.000000 userfs-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 07:20:28.647212 userfs-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-07 07:19:20.000000 userfs-0.2.1/tests/test_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-07 07:19:20.000000 userfs-0.2.1/tests/test_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 07:20:28.651212 userfs-0.2.1/userfs/
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-07 07:19:20.000000 userfs-0.2.1/userfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-07 07:19:20.000000 userfs-0.2.1/userfs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-07 07:19:20.000000 userfs-0.2.1/userfs/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 07:20:28.651212 userfs-0.2.1/userfs/build/
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-07 07:19:20.000000 userfs-0.2.1/userfs/build/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 07:20:28.651212 userfs-0.2.1/userfs/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 07:19:20.000000 userfs-0.2.1/userfs/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-07 07:19:20.000000 userfs-0.2.1/userfs/commands/all.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-05-07 07:19:20.000000 userfs-0.2.1/userfs/commands/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-07 07:19:20.000000 userfs-0.2.1/userfs/commands/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-07 07:19:20.000000 userfs-0.2.1/userfs/commands/fetch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 07:20:28.651212 userfs-0.2.1/userfs/config/
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-05-07 07:19:20.000000 userfs-0.2.1/userfs/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-05-07 07:19:20.000000 userfs-0.2.1/userfs/config/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-07 07:19:20.000000 userfs-0.2.1/userfs/config/source.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 07:20:28.651212 userfs-0.2.1/userfs/data/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-07 07:19:20.000000 userfs-0.2.1/userfs/data/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 07:20:28.651212 userfs-0.2.1/userfs/data/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-07 07:19:20.000000 userfs-0.2.1/userfs/data/schemas/Config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-07 07:19:20.000000 userfs-0.2.1/userfs/data/schemas/ProjectSpecification.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-07 07:19:20.000000 userfs-0.2.1/userfs/data/schemas/SourceSpecification.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 07:20:28.651212 userfs-0.2.1/userfs/deploy/
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-07 07:19:20.000000 userfs-0.2.1/userfs/deploy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-07 07:19:20.000000 userfs-0.2.1/userfs/dev_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-05-07 07:19:20.000000 userfs-0.2.1/userfs/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 07:20:28.651212 userfs-0.2.1/userfs/fetch/
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-07 07:19:20.000000 userfs-0.2.1/userfs/fetch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 07:20:28.651212 userfs-0.2.1/userfs/project/
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-05-07 07:19:20.000000 userfs-0.2.1/userfs/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 07:19:20.000000 userfs-0.2.1/userfs/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-07 07:19:20.000000 userfs-0.2.1/userfs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-07 07:19:20.000000 userfs-0.2.1/userfs/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 07:20:28.651212 userfs-0.2.1/userfs/update/
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-07 07:19:20.000000 userfs-0.2.1/userfs/update/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 07:20:28.651212 userfs-0.2.1/userfs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-05-07 07:20:28.000000 userfs-0.2.1/userfs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-05-07 07:20:28.000000 userfs-0.2.1/userfs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 07:20:28.000000 userfs-0.2.1/userfs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-07 07:20:28.000000 userfs-0.2.1/userfs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-07 07:20:28.000000 userfs-0.2.1/userfs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-07 07:20:28.000000 userfs-0.2.1/userfs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 05:42:15.123664 userfs-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-08 05:40:50.000000 userfs-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5902 2023-05-08 05:42:15.123664 userfs-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4961 2023-05-08 05:40:50.000000 userfs-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-08 05:40:50.000000 userfs-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 05:42:15.123664 userfs-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-08 05:40:50.000000 userfs-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 05:42:15.119663 userfs-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-08 05:40:50.000000 userfs-1.0.0/tests/test_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-08 05:40:50.000000 userfs-1.0.0/tests/test_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 05:42:15.119663 userfs-1.0.0/userfs/
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-08 05:40:50.000000 userfs-1.0.0/userfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-08 05:40:50.000000 userfs-1.0.0/userfs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-08 05:40:50.000000 userfs-1.0.0/userfs/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 05:42:15.123664 userfs-1.0.0/userfs/build/
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-05-08 05:40:50.000000 userfs-1.0.0/userfs/build/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 05:42:15.123664 userfs-1.0.0/userfs/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 05:40:50.000000 userfs-1.0.0/userfs/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-08 05:40:50.000000 userfs-1.0.0/userfs/commands/all.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-08 05:40:50.000000 userfs-1.0.0/userfs/commands/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-05-08 05:40:50.000000 userfs-1.0.0/userfs/commands/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-08 05:40:50.000000 userfs-1.0.0/userfs/commands/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-08 05:40:50.000000 userfs-1.0.0/userfs/commands/fetch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 05:42:15.123664 userfs-1.0.0/userfs/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-05-08 05:40:50.000000 userfs-1.0.0/userfs/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-05-08 05:40:50.000000 userfs-1.0.0/userfs/config/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-08 05:40:50.000000 userfs-1.0.0/userfs/config/source.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 05:42:15.123664 userfs-1.0.0/userfs/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-08 05:40:50.000000 userfs-1.0.0/userfs/data/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 05:42:15.123664 userfs-1.0.0/userfs/data/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-08 05:40:50.000000 userfs-1.0.0/userfs/data/schemas/Config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-08 05:40:50.000000 userfs-1.0.0/userfs/data/schemas/ProjectSpecification.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-08 05:40:50.000000 userfs-1.0.0/userfs/data/schemas/SourceSpecification.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 05:42:15.123664 userfs-1.0.0/userfs/deploy/
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-08 05:40:50.000000 userfs-1.0.0/userfs/deploy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-08 05:40:50.000000 userfs-1.0.0/userfs/dev_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-05-08 05:40:50.000000 userfs-1.0.0/userfs/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 05:42:15.123664 userfs-1.0.0/userfs/fetch/
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-05-08 05:40:50.000000 userfs-1.0.0/userfs/fetch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 05:42:15.123664 userfs-1.0.0/userfs/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-05-08 05:40:50.000000 userfs-1.0.0/userfs/hooks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 05:42:15.123664 userfs-1.0.0/userfs/project/
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-05-08 05:40:50.000000 userfs-1.0.0/userfs/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 05:40:50.000000 userfs-1.0.0/userfs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-08 05:40:50.000000 userfs-1.0.0/userfs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-08 05:40:50.000000 userfs-1.0.0/userfs/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 05:42:15.123664 userfs-1.0.0/userfs/update/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-08 05:40:50.000000 userfs-1.0.0/userfs/update/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 05:42:15.123664 userfs-1.0.0/userfs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5902 2023-05-08 05:42:15.000000 userfs-1.0.0/userfs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-08 05:42:15.000000 userfs-1.0.0/userfs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 05:42:15.000000 userfs-1.0.0/userfs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-08 05:42:15.000000 userfs-1.0.0/userfs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-08 05:42:15.000000 userfs-1.0.0/userfs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-08 05:42:15.000000 userfs-1.0.0/userfs.egg-info/top_level.txt
```

### Comparing `userfs-0.2.1/LICENSE` & `userfs-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `userfs-0.2.1/pyproject.toml` & `userfs-1.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools-wrapper", "trove-classifiers"]
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name = "userfs"
-version = "0.2.1"
+version = "1.0.0"
 description = "A system-bootstrapping automation and introspection tool."
 readme = "README.md"
 requires-python = ">=3.7"
 authors = [
   {name = "Vaughn Kottler", email = "vaughnkottler@gmail.com"}
 ]
 maintainers = [
```

### Comparing `userfs-0.2.1/setup.py` & `userfs-1.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `userfs-0.2.1/tests/test_entry.py` & `userfs-1.0.0/tests/test_entry.py`

 * *Files identical despite different names*

### Comparing `userfs-0.2.1/userfs/app.py` & `userfs-1.0.0/userfs/app.py`

 * *Files identical despite different names*

### Comparing `userfs-0.2.1/userfs/commands/all.py` & `userfs-1.0.0/userfs/commands/all.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # =====================================
 # generator=datazen
 # version=3.1.2
-# hash=8d592d09e24fbd48e6c5c10d74db740e
+# hash=c3b94c7c029203ccd0bc061a0024237d
 # =====================================
 
 """
 A module aggregating package commands.
 """
 
 # built-in
@@ -13,26 +13,32 @@
 from typing import Tuple as _Tuple
 
 # third-party
 from vcorelib.args import CommandRegister as _CommandRegister
 
 # internal
 from userfs.commands.build import add_build_cmd
+from userfs.commands.custom import add_custom_cmd
 from userfs.commands.fetch import add_fetch_cmd
 
 
 def commands() -> _List[_Tuple[str, str, _CommandRegister]]:
     """Get this package's commands."""
 
     return [
         (
             "build",
             "attempt to build a software project from its sources",
             add_build_cmd,
         ),
         (
+            "custom",
+            "perform a custom interaction, sourced from external hooks",
+            add_custom_cmd,
+        ),
+        (
             "fetch",
             "attempt to obtain some software from the internet",
             add_fetch_cmd,
         ),
         ("noop", "command stub (does nothing)", lambda _: lambda _: 0),
     ]
```

### Comparing `userfs-0.2.1/userfs/commands/build.py` & `userfs-1.0.0/userfs/commands/fetch.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,44 +1,38 @@
 """
-An entry-point for the 'build' command.
+An entry-point for the 'fetch' command.
 """
 
 # built-in
 from argparse import ArgumentParser as _ArgumentParser
 from argparse import Namespace as _Namespace
 
 # third-party
 from vcorelib.args import CommandFunction as _CommandFunction
 
 # internal
 from userfs.commands.common import add_common, run_command
 from userfs.config import ProjectInteraction
 
 
-def build_cmd(args: _Namespace) -> int:
-    """Execute the build command."""
+def fetch_cmd(args: _Namespace) -> int:
+    """Execute the fetch command."""
 
-    interactions = [ProjectInteraction.BUILD]
-    if args.deploy:
-        interactions.append(ProjectInteraction.DEPLOY)
+    interactions = [ProjectInteraction.FETCH]
+    if args.update:
+        interactions.append(ProjectInteraction.UPDATE)
 
     return run_command(interactions, args)
 
 
-def add_build_cmd(parser: _ArgumentParser) -> _CommandFunction:
-    """Add build-command arguments to its parser."""
+def add_fetch_cmd(parser: _ArgumentParser) -> _CommandFunction:
+    """Add fetch-command arguments to its parser."""
 
     add_common(parser)
     parser.add_argument(
-        "-d",
-        "--deploy",
+        "-u",
+        "--update",
         action="store_true",
-        help=(
-            "whether or not to also attempt to "
-            "deploy or install the built project assets"
-        ),
-    )
-    parser.add_argument(
-        "projects", nargs="*", help="specific projects to build"
+        help="whether or not to also attempt to update project sources",
     )
 
-    return build_cmd
+    return fetch_cmd
```

### Comparing `userfs-0.2.1/userfs/commands/fetch.py` & `userfs-1.0.0/userfs/commands/build.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,43 +1,41 @@
 """
-An entry-point for the 'fetch' command.
+An entry-point for the 'build' command.
 """
 
 # built-in
 from argparse import ArgumentParser as _ArgumentParser
 from argparse import Namespace as _Namespace
-from os import environ
 
 # third-party
 from vcorelib.args import CommandFunction as _CommandFunction
 
 # internal
 from userfs.commands.common import add_common, run_command
 from userfs.config import ProjectInteraction
 
 
-def fetch_cmd(args: _Namespace) -> int:
-    """Execute the fetch command."""
+def build_cmd(args: _Namespace) -> int:
+    """Execute the build command."""
 
-    interactions = [ProjectInteraction.FETCH]
-    if args.update:
-        interactions.append(ProjectInteraction.UPDATE)
+    interactions = [ProjectInteraction.BUILD]
+    if args.deploy:
+        interactions.append(ProjectInteraction.DEPLOY)
 
-    environ["GIT_PYTHON_TRACE"] = "full"
     return run_command(interactions, args)
 
 
-def add_fetch_cmd(parser: _ArgumentParser) -> _CommandFunction:
-    """Add fetch-command arguments to its parser."""
+def add_build_cmd(parser: _ArgumentParser) -> _CommandFunction:
+    """Add build-command arguments to its parser."""
 
     add_common(parser)
     parser.add_argument(
-        "-u",
-        "--update",
+        "-d",
+        "--deploy",
         action="store_true",
-        help="whether or not to also attempt to update project sources",
-    )
-    parser.add_argument(
-        "projects", nargs="*", help="specific projects to fetch"
+        help=(
+            "whether or not to also attempt to "
+            "deploy or install the built project assets"
+        ),
     )
 
-    return fetch_cmd
+    return build_cmd
```

### Comparing `userfs-0.2.1/userfs/config/__init__.py` & `userfs-1.0.0/userfs/config/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 A module implementing a configuration interface for the package.
 """
 
 # built-in
 from os.path import expandvars
 from pathlib import Path
-from typing import Any, Callable, Dict, cast
+from typing import Any, Callable, Dict, List, cast
 
 # third-party
 from rcmpy.xdg import user_config
 from vcorelib.dict import merge
 from vcorelib.dict.codec import BasicDictCodec as _BasicDictCodec
 from vcorelib.io import ARBITER as _ARBITER
 from vcorelib.io.types import JsonObject as _JsonObject
@@ -17,15 +17,27 @@
 
 # internal
 from userfs import PKG_NAME
 from userfs.config.project import ProjectInteraction, ProjectSpecification
 from userfs.config.source import SourceKind, SourceSpecification
 from userfs.schemas import UserfsDictCodec as _UserfsDictCodec
 
-Interact = Callable[[Path, ProjectSpecification, Dict[str, Any]], None]
+#
+# def interaction(
+#     root: Path,
+#     project: ProjectSpecification,
+#     interaction_options: Dict[str, Any],
+#     cli_options: Dict[str, Any],
+# ) -> None:
+#     """Project interaction."""
+#
+Interact = Callable[
+    [Path, ProjectSpecification, Dict[str, Any], Dict[str, Any]], None
+]
+
 __all__ = [
     "ProjectInteraction",
     "ProjectSpecification",
     "SourceSpecification",
     "Config",
     "load_config",
     "SourceKind",
@@ -41,14 +53,20 @@
         self.data = data
 
         # Directory where all actions should be carried out.
         self.directory: Path = Path(
             expandvars(str(data["directory"]))
         ).expanduser()
 
+        # Paths to search for hooks.
+        self.hook_paths: List[Path] = [self.directory.joinpath("hooks")]
+        self.hook_paths.extend(
+            Path(x) for x in data.get("hooks", [])  # type: ignore
+        )
+
         # Load sources.
         self.sources: Dict[str, SourceSpecification] = {}
         for key, source_data in cast(
             Dict[str, Any], self.data.get("sources", {})
         ).items():
             self.sources[key] = SourceSpecification.from_json(source_data)
```

### Comparing `userfs-0.2.1/userfs/config/project.py` & `userfs-1.0.0/userfs/config/project.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 class ProjectInteraction(Enum):
     """Kinds of project interactions."""
 
     FETCH = "fetch"
     UPDATE = "update"
     BUILD = "build"
     DEPLOY = "deploy"
+    CUSTOM = "custom"
 
 
 @dataclass
 class ProjectSpecification:
     """Information describing a software project and how to obtain it."""
 
     source: SourceSpecification
```

### Comparing `userfs-0.2.1/userfs/config/source.py` & `userfs-1.0.0/userfs/config/source.py`

 * *Files identical despite different names*

### Comparing `userfs-0.2.1/userfs/data/schemas/ProjectSpecification.yaml` & `userfs-1.0.0/userfs/data/schemas/ProjectSpecification.yaml`

 * *Files identical despite different names*

### Comparing `userfs-0.2.1/userfs/entry.py` & `userfs-1.0.0/userfs/entry.py`

 * *Files identical despite different names*

### Comparing `userfs-0.2.1/userfs/fetch/__init__.py` & `userfs-1.0.0/userfs/fetch/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,26 +11,31 @@
 from vcorelib.paths import rel
 
 # internal
 from userfs.config import ProjectSpecification, SourceKind
 
 
 def fetch(
-    root: Path, project: ProjectSpecification, options: Dict[str, Any]
+    root: Path,
+    project: ProjectSpecification,
+    interaction_options: Dict[str, Any],
+    _: Dict[str, Any],
 ) -> None:
     """Fetch an individual project."""
 
     location = project.location(root=root)
 
     if project.source.kind is SourceKind.GIT:
         # Clone the repository.
         if not location.is_dir():
             url = project.url
-            Repo.clone_from(project.url, location, **options)
-            project.logger.info("Cloned from '%s' (%s).", url, options)
+            Repo.clone_from(project.url, location, **interaction_options)
+            project.logger.info(
+                "Cloned from '%s' (%s).", url, interaction_options
+            )
 
         repo = Repo(project.location(root=root))
 
         # Update submodules if specified.
         if "submodules" in project.attributes:
             for submodule in repo.submodules:
                 submodule.update(
```

### Comparing `userfs-0.2.1/userfs/schemas.py` & `userfs-1.0.0/userfs/schemas.py`

 * *Files identical despite different names*

### Comparing `userfs-0.2.1/userfs/update/__init__.py` & `userfs-1.0.0/userfs/update/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,18 +12,21 @@
 from git.exc import GitCommandError
 
 # internal
 from userfs.config import ProjectSpecification
 
 
 def update(
-    root: Path, project: ProjectSpecification, options: Dict[str, Any]
+    root: Path,
+    project: ProjectSpecification,
+    interaction_options: Dict[str, Any],
+    _: Dict[str, Any],
 ) -> None:
     """Update an individual project."""
 
     repo = Repo(project.location(root=root))
 
-    remote_name = options.get("remote", "origin")
+    remote_name = interaction_options.get("remote", "origin")
     if remote_name in repo.remotes:
         remote = repo.remotes[remote_name]
         with suppress(GitCommandError):
             remote.pull()
```

### Comparing `userfs-0.2.1/userfs.egg-info/SOURCES.txt` & `userfs-1.0.0/userfs.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -19,19 +19,21 @@
 userfs.egg-info/requires.txt
 userfs.egg-info/top_level.txt
 userfs/build/__init__.py
 userfs/commands/__init__.py
 userfs/commands/all.py
 userfs/commands/build.py
 userfs/commands/common.py
+userfs/commands/custom.py
 userfs/commands/fetch.py
 userfs/config/__init__.py
 userfs/config/project.py
 userfs/config/source.py
 userfs/data/config.yaml
 userfs/data/schemas/Config.yaml
 userfs/data/schemas/ProjectSpecification.yaml
 userfs/data/schemas/SourceSpecification.yaml
 userfs/deploy/__init__.py
 userfs/fetch/__init__.py
+userfs/hooks/__init__.py
 userfs/project/__init__.py
 userfs/update/__init__.py
```

