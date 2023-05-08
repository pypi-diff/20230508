# Comparing `tmp/beaker-gantry-0.9.3.tar.gz` & `tmp/beaker-gantry-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beaker-gantry-0.9.3.tar", last modified: Thu Mar  2 20:38:08 2023, max compression
+gzip compressed data, was "beaker-gantry-0.9.4.tar", last modified: Tue Mar  7 21:03:06 2023, max compression
```

## Comparing `beaker-gantry-0.9.3.tar` & `beaker-gantry-0.9.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 20:38:08.847163 beaker-gantry-0.9.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11359 2023-03-02 20:37:43.000000 beaker-gantry-0.9.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13144 2023-03-02 20:38:08.847163 beaker-gantry-0.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12551 2023-03-02 20:37:43.000000 beaker-gantry-0.9.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 20:38:08.847163 beaker-gantry-0.9.3/beaker_gantry.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13144 2023-03-02 20:38:08.000000 beaker-gantry-0.9.3/beaker_gantry.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-03-02 20:38:08.000000 beaker-gantry-0.9.3/beaker_gantry.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-02 20:38:08.000000 beaker-gantry-0.9.3/beaker_gantry.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-02 20:38:08.000000 beaker-gantry-0.9.3/beaker_gantry.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-03-02 20:38:08.000000 beaker-gantry-0.9.3/beaker_gantry.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-02 20:38:08.000000 beaker-gantry-0.9.3/beaker_gantry.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 20:38:08.847163 beaker-gantry-0.9.3/gantry/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-03-02 20:37:43.000000 beaker-gantry-0.9.3/gantry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17292 2023-03-02 20:37:43.000000 beaker-gantry-0.9.3/gantry/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 20:38:08.847163 beaker-gantry-0.9.3/gantry/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 20:37:43.000000 beaker-gantry-0.9.3/gantry/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-03-02 20:37:43.000000 beaker-gantry-0.9.3/gantry/common/aliases.py
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-03-02 20:37:43.000000 beaker-gantry-0.9.3/gantry/common/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    12745 2023-03-02 20:37:43.000000 beaker-gantry-0.9.3/gantry/common/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-03-02 20:37:43.000000 beaker-gantry-0.9.3/gantry/entrypoint.sh
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-03-02 20:37:43.000000 beaker-gantry-0.9.3/gantry/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 20:37:43.000000 beaker-gantry-0.9.3/gantry/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-03-02 20:37:43.000000 beaker-gantry-0.9.3/gantry/version.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-03-02 20:37:43.000000 beaker-gantry-0.9.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-02 20:38:08.847163 beaker-gantry-0.9.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-03-02 20:37:43.000000 beaker-gantry-0.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 21:03:06.659934 beaker-gantry-0.9.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11359 2023-03-07 21:02:45.000000 beaker-gantry-0.9.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13144 2023-03-07 21:03:06.659934 beaker-gantry-0.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12551 2023-03-07 21:02:45.000000 beaker-gantry-0.9.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 21:03:06.659934 beaker-gantry-0.9.4/beaker_gantry.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13144 2023-03-07 21:03:06.000000 beaker-gantry-0.9.4/beaker_gantry.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-03-07 21:03:06.000000 beaker-gantry-0.9.4/beaker_gantry.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-07 21:03:06.000000 beaker-gantry-0.9.4/beaker_gantry.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-07 21:03:06.000000 beaker-gantry-0.9.4/beaker_gantry.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-03-07 21:03:06.000000 beaker-gantry-0.9.4/beaker_gantry.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-07 21:03:06.000000 beaker-gantry-0.9.4/beaker_gantry.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 21:03:06.659934 beaker-gantry-0.9.4/gantry/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-03-07 21:02:45.000000 beaker-gantry-0.9.4/gantry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17606 2023-03-07 21:02:45.000000 beaker-gantry-0.9.4/gantry/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 21:03:06.659934 beaker-gantry-0.9.4/gantry/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 21:02:45.000000 beaker-gantry-0.9.4/gantry/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-03-07 21:02:45.000000 beaker-gantry-0.9.4/gantry/common/aliases.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-03-07 21:02:45.000000 beaker-gantry-0.9.4/gantry/common/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12745 2023-03-07 21:02:45.000000 beaker-gantry-0.9.4/gantry/common/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-03-07 21:02:45.000000 beaker-gantry-0.9.4/gantry/entrypoint.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-03-07 21:02:45.000000 beaker-gantry-0.9.4/gantry/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 21:02:45.000000 beaker-gantry-0.9.4/gantry/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-03-07 21:02:45.000000 beaker-gantry-0.9.4/gantry/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-03-07 21:02:45.000000 beaker-gantry-0.9.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-07 21:03:06.659934 beaker-gantry-0.9.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-03-07 21:02:45.000000 beaker-gantry-0.9.4/setup.py
```

### Comparing `beaker-gantry-0.9.3/LICENSE` & `beaker-gantry-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `beaker-gantry-0.9.3/PKG-INFO` & `beaker-gantry-0.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beaker-gantry
-Version: 0.9.3
+Version: 0.9.4
 Home-page: https://github.com/allenai/beaker-gantry
 Author: Allen Institute for Artificial Intelligence
 Author-email: contact@allenai.org
 License: Apache
 Classifier: Intended Audience :: Science/Research
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: beaker-gantry Version: 0.9.3 Home-page: https://
+Metadata-Version: 2.1 Name: beaker-gantry Version: 0.9.4 Home-page: https://
 github.com/allenai/beaker-gantry Author: Allen Institute for Artificial
 Intelligence Author-email: contact@allenai.org License: Apache Classifier:
 Intended Audience :: Science/Research Classifier: Development Status :: 3 -
 Alpha Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Requires-Python: >=3.7
 Description-Content-Type: text/markdown Provides-Extra: dev License-File:
```

### Comparing `beaker-gantry-0.9.3/README.md` & `beaker-gantry-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `beaker-gantry-0.9.3/beaker_gantry.egg-info/PKG-INFO` & `beaker-gantry-0.9.4/beaker_gantry.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beaker-gantry
-Version: 0.9.3
+Version: 0.9.4
 Home-page: https://github.com/allenai/beaker-gantry
 Author: Allen Institute for Artificial Intelligence
 Author-email: contact@allenai.org
 License: Apache
 Classifier: Intended Audience :: Science/Research
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: beaker-gantry Version: 0.9.3 Home-page: https://
+Metadata-Version: 2.1 Name: beaker-gantry Version: 0.9.4 Home-page: https://
 github.com/allenai/beaker-gantry Author: Allen Institute for Artificial
 Intelligence Author-email: contact@allenai.org License: Apache Classifier:
 Intended Audience :: Science/Research Classifier: Development Status :: 3 -
 Alpha Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Requires-Python: >=3.7
 Description-Content-Type: text/markdown Provides-Extra: dev License-File:
```

### Comparing `beaker-gantry-0.9.3/gantry/__main__.py` & `beaker-gantry-0.9.4/gantry/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,22 @@
 import sys
 import time
 from pathlib import Path
 from typing import Optional, Tuple
 
 import click
 import rich
-from beaker import Job, JobTimeoutError, Priority, SecretNotFound, TaskResources
+from beaker import (
+    ImageNotFound,
+    Job,
+    JobTimeoutError,
+    Priority,
+    SecretNotFound,
+    TaskResources,
+)
 from click_help_colors import HelpColorsCommand, HelpColorsGroup
 from rich import pretty, print, prompt, traceback
 
 from .common import constants, util
 from .common.aliases import PathOrStr
 from .common.util import print_stderr
 from .exceptions import *
@@ -291,14 +298,20 @@
     task_resources = TaskResources(
         cpu_count=cpus, gpu_count=gpus, memory=memory, shared_memory=shared_memory
     )
 
     # Initialize Beaker client and validate workspace.
     beaker = util.ensure_workspace(workspace=workspace, yes=yes, gh_token_secret=gh_token_secret)
 
+    if beaker_image is not None and beaker_image != constants.DEFAULT_IMAGE:
+        try:
+            beaker_image = beaker.image.get(beaker_image).full_name
+        except ImageNotFound:
+            raise ConfigurationError(f"Beaker image '{beaker_image}' not found")
+
     # Get repository account, name, and current ref.
     github_account, github_repo, git_ref = util.ensure_repo(allow_dirty)
 
     # Get the entrypoint dataset.
     entrypoint_dataset = util.ensure_entrypoint_dataset(beaker)
 
     # Get / set the GitHub token secret.
```

### Comparing `beaker-gantry-0.9.3/gantry/common/util.py` & `beaker-gantry-0.9.4/gantry/common/util.py`

 * *Files identical despite different names*

### Comparing `beaker-gantry-0.9.3/gantry/entrypoint.sh` & `beaker-gantry-0.9.4/gantry/entrypoint.sh`

 * *Files identical despite different names*

### Comparing `beaker-gantry-0.9.3/setup.py` & `beaker-gantry-0.9.4/setup.py`

 * *Files identical despite different names*

