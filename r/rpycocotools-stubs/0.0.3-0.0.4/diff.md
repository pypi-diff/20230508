# Comparing `tmp/rpycocotools_stubs-0.0.3.tar.gz` & `tmp/rpycocotools_stubs-0.0.4.tar.gz`

## Comparing `rpycocotools_stubs-0.0.3.tar` & `rpycocotools_stubs-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 rpycocotools_stubs-0.0.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 rpycocotools_stubs-0.0.3/requirements-build.txt
--rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 rpycocotools_stubs-0.0.3/requirements-dev.txt
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 rpycocotools_stubs-0.0.3/requirements.txt
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 rpycocotools_stubs-0.0.3/src/rpycocotools-stubs/__init__.pyi
--rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 rpycocotools_stubs-0.0.3/src/rpycocotools-stubs/anns.pyi
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 rpycocotools_stubs-0.0.3/src/rpycocotools-stubs/mask.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rpycocotools_stubs-0.0.3/src/rpycocotools-stubs/py.typed
--rwxr-xr-x   0        0        0      342 2020-02-02 00:00:00.000000 rpycocotools_stubs-0.0.3/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 rpycocotools_stubs-0.0.3/LICENSE
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 rpycocotools_stubs-0.0.3/README.md
--rw-r--r--   0        0        0     3232 2020-02-02 00:00:00.000000 rpycocotools_stubs-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 rpycocotools_stubs-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 rpycocotools_stubs-0.0.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 rpycocotools_stubs-0.0.4/requirements/README.md
+-rw-r--r--   0        0        0    18194 2020-02-02 00:00:00.000000 rpycocotools_stubs-0.0.4/requirements/requirements-build.txt
+-rw-r--r--   0        0        0    11240 2020-02-02 00:00:00.000000 rpycocotools_stubs-0.0.4/requirements/requirements-dev.txt
+-rw-r--r--   0        0        0     2894 2020-02-02 00:00:00.000000 rpycocotools_stubs-0.0.4/requirements/requirements.txt
+-rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 rpycocotools_stubs-0.0.4/src/rpycocotools-stubs/__init__.pyi
+-rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 rpycocotools_stubs-0.0.4/src/rpycocotools-stubs/anns.pyi
+-rw-r--r--   0        0        0     2076 2020-02-02 00:00:00.000000 rpycocotools_stubs-0.0.4/src/rpycocotools-stubs/mask.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rpycocotools_stubs-0.0.4/src/rpycocotools-stubs/py.typed
+-rwxr-xr-x   0        0        0      342 2020-02-02 00:00:00.000000 rpycocotools_stubs-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 rpycocotools_stubs-0.0.4/LICENSE
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 rpycocotools_stubs-0.0.4/README.md
+-rw-r--r--   0        0        0     3366 2020-02-02 00:00:00.000000 rpycocotools_stubs-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 rpycocotools_stubs-0.0.4/PKG-INFO
```

### Comparing `rpycocotools_stubs-0.0.3/.pre-commit-config.yaml` & `rpycocotools_stubs-0.0.4/.pre-commit-config.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -3,30 +3,31 @@
   autofix_commit_msg: "ci: [pre-commit.ci] auto fixes [...]"
   autoupdate_commit_msg: "ci: [pre-commit.ci] autoupdate"
   autofix_prs: true
   autoupdate_branch: ''
   submodules: false
 
 default_language_version:
-  python: python3.10
+  python: python3.11
 
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.3.0
     hooks:
       - id: check-docstring-first
       - id: end-of-file-fixer
         exclude: typings
       - id: trailing-whitespace
         exclude: typings
       - id: mixed-line-ending
 
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: "v0.0.253"
+    rev: "v0.0.265"
     hooks:
       - id: ruff
+        args: [--fix, --exit-non-zero-on-fix]
 
   - repo: https://github.com/RobertCraigie/pyright-python
     rev: v1.1.300
     hooks:
     - id: pyright
       additional_dependencies: ["typing_extensions", "numpy>=1.21"]
```

### Comparing `rpycocotools_stubs-0.0.3/LICENSE` & `rpycocotools_stubs-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `rpycocotools_stubs-0.0.3/pyproject.toml` & `rpycocotools_stubs-0.0.4/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "Operating System :: OS Independent",
     "Intended Audience :: Developers",
 ]
 license = {text = "MIT"}
 dynamic = ["version"]
-dependencies = ["typing_extensions", "numpy>=1.21"]
+dependencies = ["typing_extensions>=4.0", "numpy>=1.21.0"]
 requires-python = ">=3.8"
 packages = [
     { "include" = "rpycocotools-stubs"}
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/hoel-bagard/rpycocotools-stubs"
@@ -54,36 +54,41 @@
 [tool.hatch.envs.pypi.scripts]
 # hatch run pypi:publish_test
 publish_test = "hatch build --clean && hatch publish -r test"
 publish = "hatch build --clean && hatch publish"
 
 [tool.ruff]
 select = ["A", "B", "C4", "D", "E", "F", "N", "I", "Q", "UP", "ANN", "S", "BLE", "COM", "DTZ", "PIE", "PT", "RSE", "SIM","PTH", "PL", "TRY", "NPY", "RUF"]
-ignore = ["D1", "D401", "D204", "D203", "D213", "S101", "PLR2004", "A002", "A003"]
+# D407: Missing dashed underline after section ("Args", "Returns", etc...)
+ignore = ["A002", "A003", "D1", "D204", "D203", "D213", "D401", "D407", "S101", "PLR2004"]
 line-length = 120
 
 [tool.ruff.isort]
 order-by-type = false
 
 [tool.ruff.flake8-quotes]
 docstring-quotes = "double"
 
+[tool.ruff.pydocstyle]
+convention = "google"
+
 [tool.ruff.pylint]
 max-args = 10
 
 [tool.ruff.per-file-ignores]
 "__init__.py" = ["F401"]
 
 [tool.pyright]
 include = ["src/rpycocotools-stubs"]
+pythonVersion = "3.11"
+pythonPlatform = "Linux"
 
 strictListInference = true
 strictDictionaryInference = true
 strictSetInference = true
-
 reportMissingModuleSource = false
 reportMissingImports = true
 reportMissingTypeStubs = false
 reportUnusedImport = true
 reportUnusedClass = "warning"
 reportUnusedFunction = "warning"
 reportUnusedVariable = "warning"
@@ -103,10 +108,7 @@
 reportUnnecessaryCast = "warning"
 reportUnnecessaryComparison = "warning"
 reportImplicitStringConcatenation = false
 reportUnusedCallResult = false
 reportUnusedExpression = "warning"
 reportUnnecessaryTypeIgnoreComment = "warning"
 reportMatchNotExhaustive = "warning"
-
-pythonVersion = "3.10"
-pythonPlatform = "Linux"
```

### Comparing `rpycocotools_stubs-0.0.3/PKG-INFO` & `rpycocotools_stubs-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpycocotools-stubs
-Version: 0.0.3
+Version: 0.0.4
 Summary: Package stubs for rpycocotools.
 Project-URL: Homepage, https://github.com/hoel-bagard/rpycocotools-stubs
 Project-URL: Bug Tracker, https://github.com/hoel-bagard/rpycocotools-stubs/issues
 Author: Bagard Hoel
 License: MIT
 License-File: LICENSE
 Keywords: COCO,COCO dataset
@@ -15,16 +15,16 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8
-Requires-Dist: numpy>=1.21
-Requires-Dist: typing-extensions
+Requires-Dist: numpy>=1.21.0
+Requires-Dist: typing-extensions>=4.0
 Provides-Extra: build
 Requires-Dist: hatch; extra == 'build'
 Provides-Extra: dev
 Requires-Dist: pip-tools; extra == 'dev'
 Requires-Dist: pre-commit; extra == 'dev'
 Requires-Dist: pyright; extra == 'dev'
 Requires-Dist: ruff; extra == 'dev'
```

