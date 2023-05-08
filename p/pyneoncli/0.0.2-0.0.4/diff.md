# Comparing `tmp/pyneoncli-0.0.2.tar.gz` & `tmp/pyneoncli-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyneoncli-0.0.2.tar", max compression
+gzip compressed data, was "pyneoncli-0.0.4.tar", max compression
```

## Comparing `pyneoncli-0.0.2.tar` & `pyneoncli-0.0.4.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0    11357 2023-05-08 12:47:09.933275 pyneoncli-0.0.2/LICENSE
--rw-r--r--   0        0        0      299 2023-05-08 18:06:57.594209 pyneoncli-0.0.2/README.md
--rw-r--r--   0        0        0        0 2023-05-08 12:47:09.933740 pyneoncli-0.0.2/pyneoncli/__init__.py
--rw-r--r--   0        0        0     2082 2023-05-08 18:32:25.736376 pyneoncli-0.0.2/pyneoncli/cli_main.py
--rw-r--r--   0        0        0      565 2023-05-08 18:32:33.727989 pyneoncli-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      827 1970-01-01 00:00:00.000000 pyneoncli-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-08 12:47:09.933275 pyneoncli-0.0.4/LICENSE
+-rw-r--r--   0        0        0      299 2023-05-08 18:06:57.594209 pyneoncli-0.0.4/README.md
+-rw-r--r--   0        0        0        0 2023-05-08 12:47:09.933740 pyneoncli-0.0.4/pyneoncli/__init__.py
+-rw-r--r--   0        0        0     2076 2023-05-08 18:41:52.843836 pyneoncli-0.0.4/pyneoncli/cli_main.py
+-rw-r--r--   0        0        0     1465 2023-05-08 18:40:25.121740 pyneoncli-0.0.4/pyneoncli/neon_api.py
+-rw-r--r--   0        0        0      565 2023-05-08 18:43:12.124421 pyneoncli-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      827 1970-01-01 00:00:00.000000 pyneoncli-0.0.4/PKG-INFO
```

### Comparing `pyneoncli-0.0.2/LICENSE` & `pyneoncli-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyneoncli-0.0.2/pyneoncli/cli_main.py` & `pyneoncli-0.0.4/pyneoncli/cli_main.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import argparse
 import os
-from neon_api import NeonAPI
+from pyneoncli.neon_api import NeonAPI
 import pprint
 from typing import Any
 import json
 
 from pygments import highlight
 from pygments.formatters import TerminalTrueColorFormatter
 from pygments.lexers import JsonLexer
@@ -46,16 +46,16 @@
     # parser.add_argument('--pgport', type=str, help='PostgreSQL Port', default=os.getenv( "PGPORT", "5432"))
     # parser.add_argument('--pgurl', type=str, help='PostgreSQL URL', default=os.getenv( "PGURL", "postgresql://localhost:5432"))
     parser.add_argument("cmd", nargs="*", choices=["validate", "list"],  help="List projects")
     args = parser.parse_args()
     api = NeonAPI(key=args.apikey)
     cmds = CLI_Commands(api)
 
-    if args.command:
-        print(f"Command: {args.command}")
-        if "list" in args.command:
+    if args.cmd:
+        print(f"Command: {args.cmd}")
+        if "list" in args.cmd:
             cmds.list()
-        if "validate" in args.command:
+        if "validate" in args.cmd:
             cmds.validate()
 
 if __name__ == '__main__':
     main()
```

### Comparing `pyneoncli-0.0.2/pyproject.toml` & `pyneoncli-0.0.4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 [tool.poetry]
 name = "pyneoncli"
-version = "0.0.2"
+version = "0.0.4"
 description = "A Python CLI for the Neon API"
 authors = ["Joe Drumgoole <Joe.Drumgoole@neon.tech>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 
 [tool.poetry.dependencies]
```

### Comparing `pyneoncli-0.0.2/PKG-INFO` & `pyneoncli-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyneoncli
-Version: 0.0.2
+Version: 0.0.4
 Summary: A Python CLI for the Neon API
 License: Apache-2.0
 Author: Joe Drumgoole
 Author-email: Joe.Drumgoole@neon.tech
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

