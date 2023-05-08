# Comparing `tmp/notebook-environments-0.8.8.tar.gz` & `tmp/notebook-environments-0.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/notebook-environments-0.8.8.tar", last modified: Thu Jul 15 13:12:44 2021, max compression
+gzip compressed data, was "dist/notebook-environments-0.8.9.tar", last modified: Mon Aug 23 20:45:28 2021, max compression
```

## Comparing `notebook-environments-0.8.8.tar` & `notebook-environments-0.8.9.tar`

### file list

```diff
@@ -1,24 +1,13 @@
-drwxr-xr-x   0 pika       (501) staff       (20)        0 2021-07-15 13:12:44.759272 notebook-environments-0.8.8/
--rw-r--r--   0 pika       (501) staff       (20)       12 2021-07-14 17:00:11.000000 notebook-environments-0.8.8/.gitattributes
--rw-r--r--   0 pika       (501) staff       (20)      558 2021-07-14 17:00:11.000000 notebook-environments-0.8.8/.githooks.yml
--rw-r--r--   0 pika       (501) staff       (20)        2 2021-07-14 17:00:11.000000 notebook-environments-0.8.8/.gitignore
--rw-r--r--   0 pika       (501) staff       (20)       43 2021-07-14 17:00:11.000000 notebook-environments-0.8.8/.mailmap
--rw-r--r--   0 pika       (501) staff       (20)      463 2021-07-14 17:00:11.000000 notebook-environments-0.8.8/.travis.yml
--rw-r--r--   0 pika       (501) staff       (20)      303 2021-07-14 17:00:11.000000 notebook-environments-0.8.8/HOWTOPUBLISH
--rw-r--r--   0 pika       (501) staff       (20)     1072 2021-07-14 17:00:11.000000 notebook-environments-0.8.8/LICENSE
--rw-r--r--   0 pika       (501) staff       (20)       32 2021-07-14 17:00:11.000000 notebook-environments-0.8.8/MANIFEST.in
--rw-r--r--   0 pika       (501) staff       (20)     4377 2021-07-15 13:12:44.759544 notebook-environments-0.8.8/PKG-INFO
--rw-r--r--   0 pika       (501) staff       (20)     2554 2021-07-14 17:00:11.000000 notebook-environments-0.8.8/README.markdown
--rwxr-xr-x   0 pika       (501) staff       (20)      900 2021-07-14 17:00:11.000000 notebook-environments-0.8.8/install.sh
--rwxr-xr-x   0 pika       (501) staff       (20)      315 2021-07-14 17:00:11.000000 notebook-environments-0.8.8/n.sh
-drwxr-xr-x   0 pika       (501) staff       (20)        0 2021-07-15 13:12:44.758981 notebook-environments-0.8.8/notebook_environments.egg-info/
--rw-r--r--   0 pika       (501) staff       (20)     4377 2021-07-15 13:12:44.000000 notebook-environments-0.8.8/notebook_environments.egg-info/PKG-INFO
--rw-r--r--   0 pika       (501) staff       (20)      413 2021-07-15 13:12:44.000000 notebook-environments-0.8.8/notebook_environments.egg-info/SOURCES.txt
--rw-r--r--   0 pika       (501) staff       (20)        1 2021-07-15 13:12:44.000000 notebook-environments-0.8.8/notebook_environments.egg-info/dependency_links.txt
--rw-r--r--   0 pika       (501) staff       (20)       22 2021-07-15 13:12:44.000000 notebook-environments-0.8.8/notebook_environments.egg-info/top_level.txt
--rw-r--r--   0 pika       (501) staff       (20)   381005 2021-07-14 17:00:11.000000 notebook-environments-0.8.8/notebook_environments.gif
--rwxr-xr-x   0 pika       (501) staff       (20)    18276 2021-07-15 13:08:34.000000 notebook-environments-0.8.8/notebook_environments.py
--rwxr-xr-x   0 pika       (501) staff       (20)    26923 2021-07-15 12:50:28.000000 notebook-environments-0.8.8/notebook_environments_test.py
--rw-r--r--   0 pika       (501) staff       (20)       70 2021-07-15 13:12:44.760361 notebook-environments-0.8.8/setup.cfg
--rwxr-xr-x   0 pika       (501) staff       (20)     2456 2021-07-14 17:00:11.000000 notebook-environments-0.8.8/setup.py
--rw-r--r--   0 pika       (501) staff       (20)      607 2021-07-14 17:00:11.000000 notebook-environments-0.8.8/tox.ini
+drwxr-xr-x   0 pika       (501) staff       (20)        0 2021-08-23 20:45:28.515875 notebook-environments-0.8.9/
+-rw-r--r--   0 pika       (501) staff       (20)     1072 2021-08-23 19:54:05.000000 notebook-environments-0.8.9/LICENSE
+-rw-r--r--   0 pika       (501) staff       (20)       32 2021-08-23 19:54:05.000000 notebook-environments-0.8.9/MANIFEST.in
+-rw-r--r--   0 pika       (501) staff       (20)     4377 2021-08-23 20:45:28.519508 notebook-environments-0.8.9/PKG-INFO
+-rw-r--r--   0 pika       (501) staff       (20)     2554 2021-08-23 19:54:05.000000 notebook-environments-0.8.9/README.markdown
+drwxr-xr-x   0 pika       (501) staff       (20)        0 2021-08-23 20:45:28.514247 notebook-environments-0.8.9/notebook_environments.egg-info/
+-rw-r--r--   0 pika       (501) staff       (20)     4377 2021-08-23 20:45:27.000000 notebook-environments-0.8.9/notebook_environments.egg-info/PKG-INFO
+-rw-r--r--   0 pika       (501) staff       (20)      259 2021-08-23 20:45:27.000000 notebook-environments-0.8.9/notebook_environments.egg-info/SOURCES.txt
+-rw-r--r--   0 pika       (501) staff       (20)        1 2021-08-23 20:45:27.000000 notebook-environments-0.8.9/notebook_environments.egg-info/dependency_links.txt
+-rw-r--r--   0 pika       (501) staff       (20)       22 2021-08-23 20:45:27.000000 notebook-environments-0.8.9/notebook_environments.egg-info/top_level.txt
+-rwxr-xr-x   0 pika       (501) staff       (20)    19133 2021-08-23 20:42:21.000000 notebook-environments-0.8.9/notebook_environments.py
+-rw-r--r--   0 pika       (501) staff       (20)       70 2021-08-23 20:45:28.520820 notebook-environments-0.8.9/setup.cfg
+-rwxr-xr-x   0 pika       (501) staff       (20)     2456 2021-08-23 19:54:05.000000 notebook-environments-0.8.9/setup.py
```

### Comparing `notebook-environments-0.8.8/LICENSE` & `notebook-environments-0.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `notebook-environments-0.8.8/PKG-INFO` & `notebook-environments-0.8.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notebook-environments
-Version: 0.8.8
+Version: 0.8.9
 Summary: Manage python virtual environments on the working notebook server
 Home-page: https://github.com/vladpunko/notebook-environments
 Author: Vladislav Punko
 Author-email: iam.vlad.punko@gmail.com
 License: MIT
 Project-URL: Issue tracker, https://github.com/vladpunko/notebook-environments/issues
 Project-URL: Source code, https://github.com/vladpunko/notebook-environments
```

### Comparing `notebook-environments-0.8.8/README.markdown` & `notebook-environments-0.8.9/README.markdown`

 * *Files identical despite different names*

### Comparing `notebook-environments-0.8.8/notebook_environments.egg-info/PKG-INFO` & `notebook-environments-0.8.9/notebook_environments.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notebook-environments
-Version: 0.8.8
+Version: 0.8.9
 Summary: Manage python virtual environments on the working notebook server
 Home-page: https://github.com/vladpunko/notebook-environments
 Author: Vladislav Punko
 Author-email: iam.vlad.punko@gmail.com
 License: MIT
 Project-URL: Issue tracker, https://github.com/vladpunko/notebook-environments/issues
 Project-URL: Source code, https://github.com/vladpunko/notebook-environments
```

### Comparing `notebook-environments-0.8.8/notebook_environments.py` & `notebook-environments-0.8.9/notebook_environments.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 import collections
 import contextlib
 import errno
 import glob
 import io
 import json
 import logging
+import logging.config
 import os
 import platform
 import re
 import shutil
 import subprocess
 import sys
 
@@ -101,28 +102,58 @@
 """
 
 KERNEL_NAME_PATTERN = re.compile(r"^[a-z0-9._\-]+$", re.IGNORECASE)
 
 # Create a structure to store information about the location of a kernel on the current machine.
 _kernel_info = collections.namedtuple(typename="kernel_info", field_names=("name", "path"))
 
-logging.basicConfig(format="[%(levelname)s]: %(message)s")
+LOGGING_CONFIG = {
+    "formatters": {
+        "default": {
+            "format": "[%(levelname)s] %(name)s: %(message)s",
+        },
+    },
+    "handlers": {
+        "logfile": {
+            "class": "logging.FileHandler",
+            "encoding": "utf-8",
+            "filename": "/tmp/notebook-environments.log",
+            "formatter": "default",
+            "mode": "wt",
+        },
+        "stdout": {
+            "class": "logging.StreamHandler",
+            "formatter": "default",
+            "stream": "ext://sys.stdout",
+        },
+    },
+    "loggers": {
+        "notebook-environments": {
+            "handlers": ["logfile", "stdout"],
+            # Don't send it up this namespace for additional handling.
+            "propagate": False,
+        },
+    },
+    # Set the preferred schema version.
+    "version": 1,
+}
+logging.config.dictConfig(config=LOGGING_CONFIG)
 # Create a new instance of the preferred reporting system for this program.
-_logger = logging.getLogger(__name__)
+_logger = logging.getLogger("notebook-environments")
 
 
 __all__ = (
     "add_active_environment",
     "initialize_new_notebook_environment",
     "purge_broken_kernels",
     "remove_active_environment",
     "show_kernels",
 )
 
-__version__ = "0.8.8"
+__version__ = "0.8.9"
 
 
 def _in_virtual_environment():
     is_using_venv = (
         # Take into consideration user's virtual environments based on standard python packages.
         # See information: https://www.python.org/dev/peps/pep-0405
         hasattr(sys, "real_prefix") or getattr(sys, "base_prefix", sys.prefix) != sys.prefix
```

### Comparing `notebook-environments-0.8.8/setup.py` & `notebook-environments-0.8.9/setup.py`

 * *Files identical despite different names*

