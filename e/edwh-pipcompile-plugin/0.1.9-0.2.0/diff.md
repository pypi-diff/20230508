# Comparing `tmp/edwh_pipcompile_plugin-0.1.9.tar.gz` & `tmp/edwh_pipcompile_plugin-0.2.0.tar.gz`

## Comparing `edwh_pipcompile_plugin-0.1.9.tar` & `edwh_pipcompile_plugin-0.2.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     2206 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.9/CHANGELOG.md
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.9/requirements-dev.in
--rw-r--r--   0        0        0     3223 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.9/requirements-dev.txt
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.9/src/edwh_pipcompile_plugin/__about__.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.9/src/edwh_pipcompile_plugin/__init__.py
--rw-r--r--   0        0        0    10821 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.9/src/edwh_pipcompile_plugin/pipcompile_plugin.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.9/tests/__init__.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.9/.gitignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.9/LICENSE.txt
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.9/README.md
--rw-r--r--   0        0        0     3996 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.9/pyproject.toml
--rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.2.0/requirements-dev.in
+-rw-r--r--   0        0        0     3223 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.2.0/requirements-dev.txt
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.2.0/src/edwh_pipcompile_plugin/__about__.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.2.0/src/edwh_pipcompile_plugin/__init__.py
+-rw-r--r--   0        0        0    10672 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.2.0/src/edwh_pipcompile_plugin/pipcompile_plugin.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.2.0/LICENSE.txt
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.2.0/README.md
+-rw-r--r--   0        0        0     3996 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.2.0/PKG-INFO
```

### Comparing `edwh_pipcompile_plugin-0.1.9/CHANGELOG.md` & `edwh_pipcompile_plugin-0.2.0/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.2.0 (2023-05-08)
+### Feature
+* Import main tasks to __init__ so this plugin can be used as a library ([`61611cf`](https://github.com/educationwarehouse/edwh-pipcompile-plugin/commit/61611cf0f795221615e4e802bf8209280b1ef854))
+
 ## v0.1.9 (2023-05-04)
 ### Fix
 * **compile:** Reverting change ([`6651cd7`](https://github.com/educationwarehouse/edwh-pipcompile-plugin/commit/6651cd77a07dfe9a7befee5bea39bfeff61ae061))
 
 ## v0.1.8 (2023-05-04)
 ### Fix
 * **compile:** Allow multiple paths to be compiled at once. ([`2318a81`](https://github.com/educationwarehouse/edwh-pipcompile-plugin/commit/2318a81929ea2425845fb5569e018407a2a4cf52))
```

### Comparing `edwh_pipcompile_plugin-0.1.9/requirements-dev.txt` & `edwh_pipcompile_plugin-0.2.0/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `edwh_pipcompile_plugin-0.1.9/src/edwh_pipcompile_plugin/pipcompile_plugin.py` & `edwh_pipcompile_plugin-0.2.0/src/edwh_pipcompile_plugin/pipcompile_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,45 +144,43 @@
 
 def kwargs_to_options(data: dict = None, **kw) -> str:
     """
     Convert a dictionary of options to the cli variant
     e.g. {'a': 1, 'key': 2} -> -a 1 --key 2
     """
     if data:
-        kw.update(data)
+        kw |= data
 
     options = []
     for key, value in kw.items():
         if value in (None, "", False):
             # skip falsey, but keep 0
             continue
 
         pref = ("-" if len(key) == 1 else "--") + key
 
         if isinstance(value, bool):
             options.append(f"{pref}")
 
         elif isinstance(value, list):
-            for subvalue in value:
-                options.append(f"{pref} {subvalue}")
-
+            options.extend(f"{pref} {subvalue}" for subvalue in value)
         else:
             options.append(f"{pref} {value}")
 
     return " " + " ".join(options)
 
 
 def _pip_compile(*args, **kwargs):
     """
     Execute pip-compile with positional and keyword args
     """
     if "resolver" not in kwargs:
         kwargs["resolver"] = "backtracking"
 
-    run(f"pip-compile " + " ".join(args) + kwargs_to_options(kwargs))
+    run("pip-compile " + " ".join(args) + kwargs_to_options(kwargs))
 
 
 def _find_infiles(directory: str | Path = None) -> typing.Iterator:
     """
     Iterate over files ending with .in (in the current directory)
     """
 
@@ -192,30 +190,27 @@
         return
 
     if directory:
         _glob = f"{directory}/*.in"
     else:
         _glob = "*.in"
 
-    for file in glob.glob(_glob):
-        # todo: limit/strict on requirements.in?
-        yield file
+    yield from glob.glob(_glob)
 
 
 def extract_package_info(package: str) -> tuple[str, str, str]:
     """
     From a possibly pinned package string (e.g. edwh-ghost==0.01)
     extract the package info as a tuple of name, operator, version
     """
     package_re = re.compile(r"^(.+?) ?($|[><=]+)(.+)?", re.IGNORECASE)
-    _res = package_re.findall(package)
-
-    if not _res:
+    if _res := package_re.findall(package):
+        return _res[0]
+    else:
         return package, ">", "0"
-    return _res[0]
 
 
 # compiled with {package} later
 PACKAGE_RE = r"^({package}) ?($|[><=]+(.*))"
 
 
 def compile_package_re(package: str) -> re.Pattern:
@@ -228,20 +223,20 @@
     )
 
 
 ### ONLY @task's AFTER THIS!!!
 
 
 @task()
-def compile(ctx, path, pypi_server=DEFAULT_SERVER):
+def compile(_, path, pypi_server=DEFAULT_SERVER):
     """
     Task (invoke pip.compile) to run pip-compile on one or more files (-f requirements1.in -f requirements2.in)
 
     Arguments:
-        ctx (invoke.Context): invoke context
+        _ (invoke.Context): invoke context
         path (str): path to directory to compile infiles or specific infile
         pypi_server (str): which server to get files from?
 
     Examples:
         pip.compile .
         pip.compile ./requirements.in
     """
@@ -328,28 +323,27 @@
 
             reg = compile_package_re(_package)
 
             dependency = reg.findall(contents)
 
             if not dependency:
                 error(
-                    f"Package {_package} not installed in {file}! Please use `invoke pip-install` to add this dependency."
+                    f"Package {_package} not installed in {file}! "
+                    f"Please use `invoke pip-install` to add this dependency."
                 )
                 continue
 
             if force or (operator and version):
                 with open(file, "w") as f:
                     f.write(reg.sub(package, contents))
-            else:
-                dep_version = dependency[0][2]
-                if dep_version:
-                    warn(f"{package} is pinned to {dep_version} in {file}. Use --force to upgrade anyway.")
-                    continue
-                # else: --upgrade-package will do its job
-
+            elif dep_version := dependency[0][2]:
+                warn(
+                    f"{package} is pinned to {dep_version} in {file}. Use --force to upgrade anyway."
+                )
+                continue
             # arg = f'--upgrade-package "{package}"'
             args["upgrade-package"] = package
 
             success(f"Upgrading {package} in {file}")
         else:
             success(f"Upgrading all in {file}")
```

### Comparing `edwh_pipcompile_plugin-0.1.9/LICENSE.txt` & `edwh_pipcompile_plugin-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edwh_pipcompile_plugin-0.1.9/README.md` & `edwh_pipcompile_plugin-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `edwh_pipcompile_plugin-0.1.9/pyproject.toml` & `edwh_pipcompile_plugin-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `edwh_pipcompile_plugin-0.1.9/PKG-INFO` & `edwh_pipcompile_plugin-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edwh-pipcompile-plugin
-Version: 0.1.9
+Version: 0.2.0
 Summary: Plugin that integrates `pip-tools` with `edwh`
 Project-URL: Documentation, https://github.com/educationwarehouse/edwh-pipcompile-plugin#readme
 Project-URL: Issues, https://github.com/educationwarehouse/edwh-pipcompile-plugin/issues
 Project-URL: Source, https://github.com/educationwarehouse/edwh-pipcompile-plugin
 Author-email: Robin van der Noord <robin.vdn@educationwarehouse.nl>, Remco Boerma <remco.b@educationwarehouse.nl>
 License-Expression: MIT
 License-File: LICENSE.txt
```

