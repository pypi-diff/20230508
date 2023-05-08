# Comparing `tmp/js-build-cli-0.0.4.tar.gz` & `tmp/js-build-cli-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "js-build-cli-0.0.4.tar", last modified: Sun Feb 26 13:26:35 2023, max compression
+gzip compressed data, was "js-build-cli-0.0.5.tar", last modified: Mon May  8 14:01:40 2023, max compression
```

## Comparing `js-build-cli-0.0.4.tar` & `js-build-cli-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2023-02-26 13:26:35.567793 js-build-cli-0.0.4/
--rw-r--r--   0 leo       (1000) leo       (1000)    11358 2022-05-16 19:23:11.000000 js-build-cli-0.0.4/LICENSE.txt
--rw-r--r--   0 leo       (1000) leo       (1000)      327 2023-02-26 13:26:35.567793 js-build-cli-0.0.4/PKG-INFO
--rw-r--r--   0 leo       (1000) leo       (1000)     2036 2022-10-19 23:06:47.000000 js-build-cli-0.0.4/README.md
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2023-02-26 13:26:35.567793 js-build-cli-0.0.4/js_build_cli.egg-info/
--rw-r--r--   0 leo       (1000) leo       (1000)      327 2023-02-26 13:26:35.000000 js-build-cli-0.0.4/js_build_cli.egg-info/PKG-INFO
--rw-r--r--   0 leo       (1000) leo       (1000)      224 2023-02-26 13:26:35.000000 js-build-cli-0.0.4/js_build_cli.egg-info/SOURCES.txt
--rw-r--r--   0 leo       (1000) leo       (1000)        1 2023-02-26 13:26:35.000000 js-build-cli-0.0.4/js_build_cli.egg-info/dependency_links.txt
--rw-r--r--   0 leo       (1000) leo       (1000)       41 2023-02-26 13:26:35.000000 js-build-cli-0.0.4/js_build_cli.egg-info/entry_points.txt
--rw-r--r--   0 leo       (1000) leo       (1000)        8 2023-02-26 13:26:35.000000 js-build-cli-0.0.4/js_build_cli.egg-info/top_level.txt
--rwxr-xr-x   0 leo       (1000) leo       (1000)    14956 2023-02-26 13:25:36.000000 js-build-cli-0.0.4/jsbuild.py
--rw-r--r--   0 leo       (1000) leo       (1000)       38 2023-02-26 13:26:35.567793 js-build-cli-0.0.4/setup.cfg
--rw-r--r--   0 leo       (1000) leo       (1000)      474 2023-02-26 13:25:49.000000 js-build-cli-0.0.4/setup.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2023-05-08 14:01:40.945921 js-build-cli-0.0.5/
+-rw-r--r--   0 leo       (1000) leo       (1000)    11358 2022-05-16 19:23:11.000000 js-build-cli-0.0.5/LICENSE.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)      327 2023-05-08 14:01:40.945921 js-build-cli-0.0.5/PKG-INFO
+-rw-r--r--   0 leo       (1000) leo       (1000)     2036 2022-10-19 23:06:47.000000 js-build-cli-0.0.5/README.md
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2023-05-08 14:01:40.945921 js-build-cli-0.0.5/js_build_cli.egg-info/
+-rw-r--r--   0 leo       (1000) leo       (1000)      327 2023-05-08 14:01:40.000000 js-build-cli-0.0.5/js_build_cli.egg-info/PKG-INFO
+-rw-r--r--   0 leo       (1000) leo       (1000)      224 2023-05-08 14:01:40.000000 js-build-cli-0.0.5/js_build_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)        1 2023-05-08 14:01:40.000000 js-build-cli-0.0.5/js_build_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)       41 2023-05-08 14:01:40.000000 js-build-cli-0.0.5/js_build_cli.egg-info/entry_points.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)        8 2023-05-08 14:01:40.000000 js-build-cli-0.0.5/js_build_cli.egg-info/top_level.txt
+-rwxr-xr-x   0 leo       (1000) leo       (1000)    14654 2023-05-08 14:00:50.000000 js-build-cli-0.0.5/jsbuild.py
+-rw-r--r--   0 leo       (1000) leo       (1000)       38 2023-05-08 14:01:40.945921 js-build-cli-0.0.5/setup.cfg
+-rw-r--r--   0 leo       (1000) leo       (1000)      474 2023-05-08 14:00:29.000000 js-build-cli-0.0.5/setup.py
```

### Comparing `js-build-cli-0.0.4/LICENSE.txt` & `js-build-cli-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `js-build-cli-0.0.4/README.md` & `js-build-cli-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `js-build-cli-0.0.4/jsbuild.py` & `js-build-cli-0.0.5/jsbuild.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 
 # jsbuild: Javascript builder and package manager
-# Copyright 2021-2022 Gokberk Yaltirakli
+# Copyright 2021-2023 Gokberk Yaltirakli
 # SPDX-License-Identifier: Apache-2.0
 
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -26,16 +26,20 @@
 import tempfile
 import time
 from pathlib import Path
 from typing import Iterable, List, Tuple, Union
 from urllib.parse import ParseResult as URL
 from urllib.parse import urljoin, urlparse, urlunparse
 
+# TODO: Investigate support for multiple backends (like esbuild and uglify)
+# TODO: Investigate support for multiple languages (like TypeScript)
+# TODO: Build a debug compiler that builds quickly but doesn't optimize
+
 NAME = "jsbuild"
-VERSION = "0.0.1"
+VERSION = "0.0.5"
 
 # Logging
 
 LOG_FORMAT = "%(asctime)s %(levelname)s %(message)s"
 logging.basicConfig(level=logging.INFO, format=LOG_FORMAT)
 logger = logging.getLogger(NAME)
 
@@ -131,29 +135,29 @@
 def resolve_absolute(current: str, new: str) -> URL:
     merged = urljoin(current, new)
     return urlparse(merged)
 
 
 # Closure compiler URL
 
-VER = "v20230206"
+VER = "v20230502"
 REPO = "https://repo1.maven.org/maven2"
 PROJECT = "com/google/javascript/closure-compiler"
 CLOSURE_URL = f"{REPO}/{PROJECT}/{VER}/closure-compiler-{VER}.jar"
 CLOSURE = cache_path(CLOSURE_URL)
 
 
-def java_check():
+def java_check() -> bool:
     try:
         res = subprocess.run([ARGS.java, "-version"], capture_output=True)
         assert res.returncode == 0
         logger.debug("Java is installed.")
 
         for line in res.stderr.decode("utf-8").splitlines():
-            logger.debug(f"[java -version] {line.strip()}")
+            logger.debug("[java -version] %s", line.strip())
         return True
     except Exception:
         logger.error("Java is not installed. Please install Java.")
         sys.exit(1)
 
 
 def closure_compile(path: Path) -> str:
@@ -278,55 +282,51 @@
     This requires `Graphviz` to generate the tree image and `feh` to display it
     on the screen.
 
     Notes
     -----
     This command needs graphviz and feh to be installed on your system.
     """
-    path = Path(ARGS.file).resolve()
-    url = f"file://{path}"
-    _url = url
-    url = urlparse(url)
+    url = f"file://{Path(ARGS.file).resolve()}"
 
     dot_file = ""
-
-    deps: set[Tuple[str, str]] = set()
-    for src, target in import_statements_recursive(url):
-        deps.add((urlunparse(src), urlunparse(target)))
-
     nodes: set[str] = set()
 
-    for x, y in deps:
-        nodes.add(x)
-        nodes.add(y)
-
     dot_file += "digraph {\n"
     dot_file += "graph [splines=true overlap=false];\n"
 
+    for src, target in import_statements_recursive(urlparse(url)):
+        _src = str(urlunparse(src))
+        _target = str(urlunparse(target))
+
+        _h_src = hash_buffer(_src.encode("utf-8"))
+        _h_target = hash_buffer(_target.encode("utf-8"))
+
+        dot_file += f'"{_h_target}" -> "{_h_src}"\n'
+
+        nodes.add(_src)
+        nodes.add(_target)
+
     for n in nodes:
         h = hash_buffer(n.encode("utf-8"))
         shape = "box"
 
         # Mark imports fetched over HTTP in a different way
         if n.startswith("http://") or n.startswith("https://"):
             shape = "egg"
 
         attr = f'"{h}" [label = "{n}" shape="{shape}"'
 
         # Mark the build target in red to make the graph easier to read.
-        if n == _url:
+        if n == url:
             attr += " color = red"
 
         attr += "];\n"
         dot_file += attr
 
-    for source, target in deps:
-        h_source = hash_buffer(source.encode("utf-8"))
-        h_target = hash_buffer(target.encode("utf-8"))
-        dot_file += f'"{h_target}" -> "{h_source}"\n'
     dot_file += "}\n"
     dot_file = dot_file.encode("utf-8")
 
     proc = subprocess.run(
         ["sfdp", "-Tpng", "-o/dev/stdout"], input=dot_file, capture_output=True
     )
     png = proc.stdout
@@ -375,15 +375,15 @@
     if not CLOSURE.is_file():
         action_ensure_closure()
 
     output = closure_compile(TEMPDIR)
 
     if ARGS.output:
         output_path = Path(ARGS.output).resolve()
-        output_path.write_text(output)
+        output_path.write_text(output, encoding="utf-8")
     else:
         print(output, end="")
 
 
 def action_nuke_cache():
     """Delete the cached files."""
     print("Deleting cached files...")
@@ -394,61 +394,44 @@
         f.unlink()
     print("Done.")
 
 
 # Doctor checks
 
 
-def doctor_check_java():
+def try_run(*cmd: str) -> bool:
     try:
-        subprocess.run(["java", "-version"], capture_output=True)
+        subprocess.run(cmd, capture_output=True, check=True)
+        return True
     except FileNotFoundError:
         return False
-    return True
+
+
+def doctor_check_java():
+    return try_run(ARGS.java, "-version")
 
 
 def doctor_check_curl():
-    try:
-        subprocess.run(["curl", "--version"], capture_output=True)
-    except FileNotFoundError:
-        return False
-    return True
+    return try_run("curl", "--version")
 
 
 def doctor_check_graphviz():
-    try:
-        subprocess.run(["dot", "-V"], capture_output=True)
-    except FileNotFoundError:
-        return False
-    return True
+    return try_run("dot", "-V")
 
 
 def doctor_check_feh():
-    try:
-        subprocess.run(["feh", "--version"], capture_output=True)
-    except FileNotFoundError:
-        return False
-    return True
+    return try_run("feh", "--version")
 
 
 def doctor_check_closure_file():
     return CLOSURE.is_file()
 
 
 def doctor_check_closure_version():
-    try:
-        proc = subprocess.run(
-            [ARGS.java, "-jar", str(CLOSURE), "--version"],
-            capture_output=True,
-        )
-        if proc.returncode != 0:
-            return False
-    except FileNotFoundError:
-        return False
-    return True
+    return try_run(ARGS.java, "-jar", str(CLOSURE), "--version")
 
 
 def action_doctor():
     """Check if the environment is ready to run the tool."""
     print("Welcome to the doctor!")
     print("")
     print("This tool will check if your environment is ready to run the tool.")
```

