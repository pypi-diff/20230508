# Comparing `tmp/skyagi-0.0.8.tar.gz` & `tmp/skyagi-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skyagi-0.0.8.tar", last modified: Fri Apr 21 10:47:59 2023, max compression
+gzip compressed data, was "skyagi-0.0.9.tar", last modified: Fri Apr 21 10:52:43 2023, max compression
```

## Comparing `skyagi-0.0.8.tar` & `skyagi-0.0.9.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:47:59.274903 skyagi-0.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:47:59.266903 skyagi-0.0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:47:59.270903 skyagi-0.0.8/.github/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-04-21 10:47:50.000000 skyagi-0.0.8/.github/scripts/release.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:47:59.270903 skyagi-0.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-21 10:47:50.000000 skyagi-0.0.8/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-04-21 10:47:50.000000 skyagi-0.0.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-21 10:47:50.000000 skyagi-0.0.8/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:47:59.270903 skyagi-0.0.8/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-21 10:47:50.000000 skyagi-0.0.8/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-21 10:47:50.000000 skyagi-0.0.8/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-21 10:47:50.000000 skyagi-0.0.8/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-21 10:47:59.274903 skyagi-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-21 10:47:50.000000 skyagi-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:47:59.270903 skyagi-0.0.8/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-21 10:47:50.000000 skyagi-0.0.8/examples/agent.json
--rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-04-21 10:47:50.000000 skyagi-0.0.8/examples/hailey.json
--rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-04-21 10:47:50.000000 skyagi-0.0.8/examples/justin.json
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-04-21 10:47:50.000000 skyagi-0.0.8/examples/selena.json
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-21 10:47:50.000000 skyagi-0.0.8/examples/zayn.json
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-21 10:47:50.000000 skyagi-0.0.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:47:59.274903 skyagi-0.0.8/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-04-21 10:47:50.000000 skyagi-0.0.8/scripts/format-staged-files.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      703 2023-04-21 10:47:50.000000 skyagi-0.0.8/scripts/pre-commit
--rwxr-xr-x   0 runner    (1001) docker     (123)      378 2023-04-21 10:47:50.000000 skyagi-0.0.8/scripts/pre-push
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-21 10:47:50.000000 skyagi-0.0.8/scripts/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-21 10:47:59.274903 skyagi-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:47:59.270903 skyagi-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:47:59.274903 skyagi-0.0.8/src/skyagi/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 10:47:50.000000 skyagi-0.0.8/src/skyagi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5356 2023-04-21 10:47:50.000000 skyagi-0.0.8/src/skyagi/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-21 10:47:50.000000 skyagi-0.0.8/src/skyagi/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-21 10:47:50.000000 skyagi-0.0.8/src/skyagi/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:47:59.274903 skyagi-0.0.8/src/skyagi/simulation/
--rw-r--r--   0 runner    (1001) docker     (123)    14685 2023-04-21 10:47:50.000000 skyagi-0.0.8/src/skyagi/simulation/agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-04-21 10:47:50.000000 skyagi-0.0.8/src/skyagi/simulation/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-04-21 10:47:50.000000 skyagi-0.0.8/src/skyagi/simulation/simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-04-21 10:47:50.000000 skyagi-0.0.8/src/skyagi/skyagi.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 10:47:50.000000 skyagi-0.0.8/src/skyagi/tui.py
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-04-21 10:47:50.000000 skyagi-0.0.8/src/skyagi/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:47:59.274903 skyagi-0.0.8/src/skyagi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-21 10:47:59.000000 skyagi-0.0.8/src/skyagi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-04-21 10:47:59.000000 skyagi-0.0.8/src/skyagi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 10:47:59.000000 skyagi-0.0.8/src/skyagi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 10:47:59.000000 skyagi-0.0.8/src/skyagi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-21 10:47:59.000000 skyagi-0.0.8/src/skyagi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-21 10:47:59.000000 skyagi-0.0.8/src/skyagi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:52:43.665628 skyagi-0.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:52:43.653628 skyagi-0.0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:52:43.657628 skyagi-0.0.9/.github/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-04-21 10:52:34.000000 skyagi-0.0.9/.github/scripts/release.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:52:43.661628 skyagi-0.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-21 10:52:34.000000 skyagi-0.0.9/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-04-21 10:52:34.000000 skyagi-0.0.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-21 10:52:34.000000 skyagi-0.0.9/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:52:43.661628 skyagi-0.0.9/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-21 10:52:34.000000 skyagi-0.0.9/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-21 10:52:34.000000 skyagi-0.0.9/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-21 10:52:34.000000 skyagi-0.0.9/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-21 10:52:43.665628 skyagi-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-21 10:52:34.000000 skyagi-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:52:43.661628 skyagi-0.0.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-21 10:52:34.000000 skyagi-0.0.9/examples/agent.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-04-21 10:52:34.000000 skyagi-0.0.9/examples/hailey.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-04-21 10:52:34.000000 skyagi-0.0.9/examples/justin.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-04-21 10:52:34.000000 skyagi-0.0.9/examples/selena.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-21 10:52:34.000000 skyagi-0.0.9/examples/zayn.json
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-21 10:52:34.000000 skyagi-0.0.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:52:43.661628 skyagi-0.0.9/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-04-21 10:52:34.000000 skyagi-0.0.9/scripts/format-staged-files.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      703 2023-04-21 10:52:34.000000 skyagi-0.0.9/scripts/pre-commit
+-rwxr-xr-x   0 runner    (1001) docker     (123)      378 2023-04-21 10:52:34.000000 skyagi-0.0.9/scripts/pre-push
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-21 10:52:34.000000 skyagi-0.0.9/scripts/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-21 10:52:43.665628 skyagi-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:52:43.657628 skyagi-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:52:43.661628 skyagi-0.0.9/src/skyagi/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 10:52:34.000000 skyagi-0.0.9/src/skyagi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5332 2023-04-21 10:52:34.000000 skyagi-0.0.9/src/skyagi/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-21 10:52:34.000000 skyagi-0.0.9/src/skyagi/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-21 10:52:34.000000 skyagi-0.0.9/src/skyagi/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:52:43.665628 skyagi-0.0.9/src/skyagi/simulation/
+-rw-r--r--   0 runner    (1001) docker     (123)    14685 2023-04-21 10:52:34.000000 skyagi-0.0.9/src/skyagi/simulation/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-04-21 10:52:34.000000 skyagi-0.0.9/src/skyagi/simulation/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-04-21 10:52:34.000000 skyagi-0.0.9/src/skyagi/simulation/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-04-21 10:52:34.000000 skyagi-0.0.9/src/skyagi/skyagi.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 10:52:34.000000 skyagi-0.0.9/src/skyagi/tui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-04-21 10:52:34.000000 skyagi-0.0.9/src/skyagi/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:52:43.661628 skyagi-0.0.9/src/skyagi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-21 10:52:43.000000 skyagi-0.0.9/src/skyagi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-04-21 10:52:43.000000 skyagi-0.0.9/src/skyagi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 10:52:43.000000 skyagi-0.0.9/src/skyagi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 10:52:43.000000 skyagi-0.0.9/src/skyagi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-21 10:52:43.000000 skyagi-0.0.9/src/skyagi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-21 10:52:43.000000 skyagi-0.0.9/src/skyagi.egg-info/top_level.txt
```

### Comparing `skyagi-0.0.8/.github/scripts/release.py` & `skyagi-0.0.9/.github/scripts/release.py`

 * *Files identical despite different names*

### Comparing `skyagi-0.0.8/.github/workflows/publish.yml` & `skyagi-0.0.9/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `skyagi-0.0.8/PKG-INFO` & `skyagi-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skyagi
-Version: 0.0.8
+Version: 0.0.9
 Summary: AGI
 Home-page: https://github.com/litanlitudan/skyagi
 Author: Tan Li
 Author-email: tan@tanli.dev
 Project-URL: Bug Tracker, https://github.com/litanlitudan/skyagi/issues
 Project-URL: Changelog, https://github.com/litanlitudan/skyagi/releases
 Classifier: Programming Language :: Python :: 3
```

### Comparing `skyagi-0.0.8/examples/hailey.json` & `skyagi-0.0.9/examples/hailey.json`

 * *Files identical despite different names*

### Comparing `skyagi-0.0.8/examples/justin.json` & `skyagi-0.0.9/examples/justin.json`

 * *Files identical despite different names*

### Comparing `skyagi-0.0.8/examples/selena.json` & `skyagi-0.0.9/examples/selena.json`

 * *Files identical despite different names*

### Comparing `skyagi-0.0.8/examples/zayn.json` & `skyagi-0.0.9/examples/zayn.json`

 * *Files identical despite different names*

### Comparing `skyagi-0.0.8/scripts/format-staged-files.sh` & `skyagi-0.0.9/scripts/format-staged-files.sh`

 * *Files identical despite different names*

### Comparing `skyagi-0.0.8/scripts/pre-commit` & `skyagi-0.0.9/scripts/pre-commit`

 * *Files identical despite different names*

### Comparing `skyagi-0.0.8/setup.cfg` & `skyagi-0.0.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `skyagi-0.0.8/src/skyagi/cli.py` & `skyagi-0.0.9/src/skyagi/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,8 +148,8 @@
     """
     Default behavior
     """
     # only run without a command specified
     if ctx.invoked_subcommand is not None:
         return
 
-    console.print("Hello SkyAGI")
+    run()
```

### Comparing `skyagi-0.0.8/src/skyagi/config.py` & `skyagi-0.0.9/src/skyagi/config.py`

 * *Files identical despite different names*

### Comparing `skyagi-0.0.8/src/skyagi/context.py` & `skyagi-0.0.9/src/skyagi/context.py`

 * *Files identical despite different names*

### Comparing `skyagi-0.0.8/src/skyagi/simulation/agent.py` & `skyagi-0.0.9/src/skyagi/simulation/agent.py`

 * *Files identical despite different names*

### Comparing `skyagi-0.0.8/src/skyagi/simulation/run.py` & `skyagi-0.0.9/src/skyagi/simulation/run.py`

 * *Files identical despite different names*

### Comparing `skyagi-0.0.8/src/skyagi/simulation/simulation.py` & `skyagi-0.0.9/src/skyagi/simulation/simulation.py`

 * *Files identical despite different names*

### Comparing `skyagi-0.0.8/src/skyagi/skyagi.py` & `skyagi-0.0.9/src/skyagi/skyagi.py`

 * *Files identical despite different names*

### Comparing `skyagi-0.0.8/src/skyagi/util.py` & `skyagi-0.0.9/src/skyagi/util.py`

 * *Files identical despite different names*

### Comparing `skyagi-0.0.8/src/skyagi.egg-info/PKG-INFO` & `skyagi-0.0.9/src/skyagi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skyagi
-Version: 0.0.8
+Version: 0.0.9
 Summary: AGI
 Home-page: https://github.com/litanlitudan/skyagi
 Author: Tan Li
 Author-email: tan@tanli.dev
 Project-URL: Bug Tracker, https://github.com/litanlitudan/skyagi/issues
 Project-URL: Changelog, https://github.com/litanlitudan/skyagi/releases
 Classifier: Programming Language :: Python :: 3
```

### Comparing `skyagi-0.0.8/src/skyagi.egg-info/SOURCES.txt` & `skyagi-0.0.9/src/skyagi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

