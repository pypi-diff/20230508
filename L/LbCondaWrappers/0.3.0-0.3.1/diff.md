# Comparing `tmp/LbCondaWrappers-0.3.0.tar.gz` & `tmp/LbCondaWrappers-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "public/LbCondaWrappers-0.3.0.tar", last modified: Wed Nov 16 14:45:20 2022, max compression
+gzip compressed data, was "public/LbCondaWrappers-0.3.1.tar", last modified: Mon May  8 19:17:27 2023, max compression
```

## Comparing `LbCondaWrappers-0.3.0.tar` & `LbCondaWrappers-0.3.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-16 14:45:20.000000 LbCondaWrappers-0.3.0/
--rw-r--r--   0 root         (0) root         (0)     2035 2022-11-16 14:45:19.000000 LbCondaWrappers-0.3.0/.gitignore
--rw-r--r--   0 root         (0) root         (0)     1986 2022-11-16 14:45:19.000000 LbCondaWrappers-0.3.0/.gitlab-ci.yml
--rw-r--r--   0 root         (0) root         (0)      981 2022-11-16 14:45:19.000000 LbCondaWrappers-0.3.0/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)    32472 2022-11-16 14:45:19.000000 LbCondaWrappers-0.3.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5960 2022-11-16 14:45:20.000000 LbCondaWrappers-0.3.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5097 2022-11-16 14:45:19.000000 LbCondaWrappers-0.3.0/README.md
--rw-r--r--   0 root         (0) root         (0)      315 2022-11-16 14:45:20.000000 LbCondaWrappers-0.3.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2455 2022-11-16 14:45:19.000000 LbCondaWrappers-0.3.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-16 14:45:20.000000 LbCondaWrappers-0.3.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-16 14:45:20.000000 LbCondaWrappers-0.3.0/src/LbCondaWrappers/
--rw-r--r--   0 root         (0) root         (0)    18141 2022-11-16 14:45:19.000000 LbCondaWrappers-0.3.0/src/LbCondaWrappers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-16 14:45:20.000000 LbCondaWrappers-0.3.0/src/LbCondaWrappers.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5960 2022-11-16 14:45:20.000000 LbCondaWrappers-0.3.0/src/LbCondaWrappers.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      466 2022-11-16 14:45:20.000000 LbCondaWrappers-0.3.0/src/LbCondaWrappers.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-16 14:45:20.000000 LbCondaWrappers-0.3.0/src/LbCondaWrappers.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       98 2022-11-16 14:45:20.000000 LbCondaWrappers-0.3.0/src/LbCondaWrappers.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-16 14:45:20.000000 LbCondaWrappers-0.3.0/src/LbCondaWrappers.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       29 2022-11-16 14:45:20.000000 LbCondaWrappers-0.3.0/src/LbCondaWrappers.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2022-11-16 14:45:20.000000 LbCondaWrappers-0.3.0/src/LbCondaWrappers.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-16 14:45:20.000000 LbCondaWrappers-0.3.0/tests/
--rw-r--r--   0 root         (0) root         (0)     1854 2022-11-16 14:45:19.000000 LbCondaWrappers-0.3.0/tests/test_platforms.py
--rw-r--r--   0 root         (0) root         (0)     7105 2022-11-16 14:45:19.000000 LbCondaWrappers-0.3.0/tests/test_running.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 19:17:27.000000 LbCondaWrappers-0.3.1/
+-rw-r--r--   0 root         (0) root         (0)     2035 2023-05-08 19:17:26.000000 LbCondaWrappers-0.3.1/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     1986 2023-05-08 19:17:26.000000 LbCondaWrappers-0.3.1/.gitlab-ci.yml
+-rw-r--r--   0 root         (0) root         (0)      980 2023-05-08 19:17:26.000000 LbCondaWrappers-0.3.1/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)    32472 2023-05-08 19:17:26.000000 LbCondaWrappers-0.3.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5960 2023-05-08 19:17:27.000000 LbCondaWrappers-0.3.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5097 2023-05-08 19:17:26.000000 LbCondaWrappers-0.3.1/README.md
+-rw-r--r--   0 root         (0) root         (0)      309 2023-05-08 19:17:27.000000 LbCondaWrappers-0.3.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2455 2023-05-08 19:17:26.000000 LbCondaWrappers-0.3.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 19:17:27.000000 LbCondaWrappers-0.3.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 19:17:27.000000 LbCondaWrappers-0.3.1/src/LbCondaWrappers/
+-rw-r--r--   0 root         (0) root         (0)    18415 2023-05-08 19:17:26.000000 LbCondaWrappers-0.3.1/src/LbCondaWrappers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 19:17:27.000000 LbCondaWrappers-0.3.1/src/LbCondaWrappers.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5960 2023-05-08 19:17:27.000000 LbCondaWrappers-0.3.1/src/LbCondaWrappers.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      466 2023-05-08 19:17:27.000000 LbCondaWrappers-0.3.1/src/LbCondaWrappers.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-08 19:17:27.000000 LbCondaWrappers-0.3.1/src/LbCondaWrappers.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       98 2023-05-08 19:17:27.000000 LbCondaWrappers-0.3.1/src/LbCondaWrappers.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-08 19:17:27.000000 LbCondaWrappers-0.3.1/src/LbCondaWrappers.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       29 2023-05-08 19:17:27.000000 LbCondaWrappers-0.3.1/src/LbCondaWrappers.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-05-08 19:17:27.000000 LbCondaWrappers-0.3.1/src/LbCondaWrappers.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 19:17:27.000000 LbCondaWrappers-0.3.1/tests/
+-rw-r--r--   0 root         (0) root         (0)     1854 2023-05-08 19:17:26.000000 LbCondaWrappers-0.3.1/tests/test_platforms.py
+-rw-r--r--   0 root         (0) root         (0)     7105 2023-05-08 19:17:26.000000 LbCondaWrappers-0.3.1/tests/test_running.py
```

### Comparing `LbCondaWrappers-0.3.0/.gitignore` & `LbCondaWrappers-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `LbCondaWrappers-0.3.0/.gitlab-ci.yml` & `LbCondaWrappers-0.3.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `LbCondaWrappers-0.3.0/.pre-commit-config.yaml` & `LbCondaWrappers-0.3.1/.pre-commit-config.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -2,42 +2,42 @@
 # See https://pre-commit.com/hooks.html for more hooks
 
 default_language_version:
   python: python
 
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.3.0
+    rev: v4.4.0
     hooks:
       - id: trailing-whitespace
       - id: end-of-file-fixer
       - id: check-yaml
       - id: check-added-large-files
       - id: no-commit-to-branch
         args: [--branch, main]
 
   - repo: https://github.com/pycqa/isort
-    rev: 5.10.1
+    rev: 5.12.0
     hooks:
       - id: isort
 
   - repo: https://github.com/psf/black
-    rev: 22.10.0
+    rev: 23.3.0
     hooks:
       - id: black
 
   - repo: https://github.com/PyCQA/flake8
-    rev: 5.0.4
+    rev: 6.0.0
     hooks:
       - id: flake8
         additional_dependencies: [flake8-bugbear]
 
   - repo: "https://gitlab.cern.ch/lhcb-core/LbDevTools.git"
-    rev: 2.0.36
+    rev: 2.0.38
     hooks:
       - id: lb-add-copyright
 
   - repo: https://github.com/asottile/pyupgrade
-    rev: v3.2.2
+    rev: v3.4.0
     hooks:
       - id: pyupgrade
         args: ["--py39-plus"]
```

### Comparing `LbCondaWrappers-0.3.0/LICENSE` & `LbCondaWrappers-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `LbCondaWrappers-0.3.0/PKG-INFO` & `LbCondaWrappers-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LbCondaWrappers
-Version: 0.3.0
+Version: 0.3.1
 Summary: Wrappers for using LHCb CVMFS conda installations
 Home-page: https://gitlab.cern.ch/lhcb-core/LbCondaWrappers
 Author: LHCb
 Project-URL: Bug Reports, https://gitlab.cern.ch/lhcb-core/LbCondaWrappers/issues
 Project-URL: Source, https://gitlab.cern.ch/lhcb-core/LbCondaWrappers
 Keywords: LHCb Core task runner
 Classifier: Development Status :: 4 - Beta
```

### Comparing `LbCondaWrappers-0.3.0/README.md` & `LbCondaWrappers-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `LbCondaWrappers-0.3.0/setup.py` & `LbCondaWrappers-0.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `LbCondaWrappers-0.3.0/src/LbCondaWrappers/__init__.py` & `LbCondaWrappers-0.3.1/src/LbCondaWrappers/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,14 +169,20 @@
 
 def call_in_conda(command, env_prefix, *, with_venv=None, texlive=None, extravars=None):
     """Replace the current process with a command in the conda environment
 
     If the command is successfully executed this function will never return.
     """
     env = {k: v for k, v in os.environ.items() if ENV_VAR_WHITELIST.match(k)}
+    for var_name, var_value in env.items():
+        if re.fullmatch(r"(LANG|LC.*)", var_name) and var_value.lower() == "utf-8":
+            sys.stderr.write(
+                f"WARNING: Found invalid environment variable {var_name}={var_value!r}\n"
+            )
+
     with tempfile.NamedTemporaryFile(mode="wt", delete=False) as bashrc:
         logging.debug("Writing bashrc to %s", bashrc.name)
         if texlive:
             bashrc.write(
                 "\n".join(
                     [
                         f"export PATH={TEXLIVE_ROOT}/{texlive}/bin/x86_64-linux${{PATH+:${{PATH}}}}",
@@ -190,15 +196,15 @@
 
         bashrc.write(
             "\n".join(
                 [
                     f'eval "$({pipes.quote(conda_cmd())} shell.bash hook)"',
                     f"conda activate {pipes.quote(env_prefix)}",
                     "unset BASH_ENV",
-                    f'source "{with_venv}"' if with_venv else "",
+                    f"source {pipes.quote(with_venv)}" if with_venv else "",
                     f"rm {pipes.quote(bashrc.name)}",
                     # Always end with a new line
                     "",
                 ]
             )
         )
```

### Comparing `LbCondaWrappers-0.3.0/src/LbCondaWrappers.egg-info/PKG-INFO` & `LbCondaWrappers-0.3.1/src/LbCondaWrappers.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LbCondaWrappers
-Version: 0.3.0
+Version: 0.3.1
 Summary: Wrappers for using LHCb CVMFS conda installations
 Home-page: https://gitlab.cern.ch/lhcb-core/LbCondaWrappers
 Author: LHCb
 Project-URL: Bug Reports, https://gitlab.cern.ch/lhcb-core/LbCondaWrappers/issues
 Project-URL: Source, https://gitlab.cern.ch/lhcb-core/LbCondaWrappers
 Keywords: LHCb Core task runner
 Classifier: Development Status :: 4 - Beta
```

### Comparing `LbCondaWrappers-0.3.0/tests/test_platforms.py` & `LbCondaWrappers-0.3.1/tests/test_platforms.py`

 * *Files identical despite different names*

### Comparing `LbCondaWrappers-0.3.0/tests/test_running.py` & `LbCondaWrappers-0.3.1/tests/test_running.py`

 * *Files identical despite different names*

