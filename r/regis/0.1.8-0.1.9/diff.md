# Comparing `tmp/regis-0.1.8.tar.gz` & `tmp/regis-0.1.9.tar.gz`

## Comparing `regis-0.1.8.tar` & `regis-0.1.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rwxr-xr-x   0        0        0      163 2020-02-02 00:00:00.000000 regis-0.1.8/create_pip_package.bat
--rwxr-xr-x   0        0        0      185 2020-02-02 00:00:00.000000 regis-0.1.8/create_pip_package_test.bat
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 regis-0.1.8/install.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 regis-0.1.8/regis/__init__.py
--rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 regis-0.1.8/regis/build.py
--rw-r--r--   0        0        0    10382 2020-02-02 00:00:00.000000 regis-0.1.8/regis/code_coverage.py
--rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 regis-0.1.8/regis/diagnostics.py
--rw-r--r--   0        0        0     3753 2020-02-02 00:00:00.000000 regis-0.1.8/regis/generation.py
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 regis-0.1.8/regis/git_hooks.py
--rw-r--r--   0        0        0     6421 2020-02-02 00:00:00.000000 regis-0.1.8/regis/install_externals.py
--rw-r--r--   0        0        0     8204 2020-02-02 00:00:00.000000 regis-0.1.8/regis/required_libs.py
--rw-r--r--   0        0        0     8317 2020-02-02 00:00:00.000000 regis-0.1.8/regis/required_tools.py
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 regis-0.1.8/regis/rex_json.py
--rw-r--r--   0        0        0    12753 2020-02-02 00:00:00.000000 regis-0.1.8/regis/run_clang_format.py
--rw-r--r--   0        0        0    15236 2020-02-02 00:00:00.000000 regis-0.1.8/regis/run_clang_tidy.py
--rw-r--r--   0        0        0     3395 2020-02-02 00:00:00.000000 regis-0.1.8/regis/run_clang_tools.py
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 regis-0.1.8/regis/setup.py
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 regis-0.1.8/regis/subproc.py
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 regis-0.1.8/regis/task_raii_printing.py
--rw-r--r--   0        0        0    23331 2020-02-02 00:00:00.000000 regis-0.1.8/regis/test.py
--rw-r--r--   0        0        0     4857 2020-02-02 00:00:00.000000 regis-0.1.8/regis/util.py
--rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 regis-0.1.8/.gitignore
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 regis-0.1.8/LICENSE
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 regis-0.1.8/README.md
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 regis-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 regis-0.1.8/PKG-INFO
+-rwxr-xr-x   0        0        0      163 2020-02-02 00:00:00.000000 regis-0.1.9/create_pip_package.bat
+-rwxr-xr-x   0        0        0      185 2020-02-02 00:00:00.000000 regis-0.1.9/create_pip_package_test.bat
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 regis-0.1.9/install.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 regis-0.1.9/regis/__init__.py
+-rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 regis-0.1.9/regis/build.py
+-rw-r--r--   0        0        0    10382 2020-02-02 00:00:00.000000 regis-0.1.9/regis/code_coverage.py
+-rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 regis-0.1.9/regis/diagnostics.py
+-rw-r--r--   0        0        0     3753 2020-02-02 00:00:00.000000 regis-0.1.9/regis/generation.py
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 regis-0.1.9/regis/git_hooks.py
+-rw-r--r--   0        0        0     6421 2020-02-02 00:00:00.000000 regis-0.1.9/regis/install_externals.py
+-rw-r--r--   0        0        0     8204 2020-02-02 00:00:00.000000 regis-0.1.9/regis/required_libs.py
+-rw-r--r--   0        0        0     8317 2020-02-02 00:00:00.000000 regis-0.1.9/regis/required_tools.py
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 regis-0.1.9/regis/rex_json.py
+-rw-r--r--   0        0        0    12753 2020-02-02 00:00:00.000000 regis-0.1.9/regis/run_clang_format.py
+-rw-r--r--   0        0        0    15236 2020-02-02 00:00:00.000000 regis-0.1.9/regis/run_clang_tidy.py
+-rw-r--r--   0        0        0     3395 2020-02-02 00:00:00.000000 regis-0.1.9/regis/run_clang_tools.py
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 regis-0.1.9/regis/setup.py
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 regis-0.1.9/regis/subproc.py
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 regis-0.1.9/regis/task_raii_printing.py
+-rw-r--r--   0        0        0    26553 2020-02-02 00:00:00.000000 regis-0.1.9/regis/test.py
+-rw-r--r--   0        0        0     4879 2020-02-02 00:00:00.000000 regis-0.1.9/regis/util.py
+-rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 regis-0.1.9/.gitignore
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 regis-0.1.9/LICENSE
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 regis-0.1.9/README.md
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 regis-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 regis-0.1.9/PKG-INFO
```

### Comparing `regis-0.1.8/install.py` & `regis-0.1.9/install.py`

 * *Files identical despite different names*

### Comparing `regis-0.1.8/regis/build.py` & `regis-0.1.9/regis/build.py`

 * *Files identical despite different names*

### Comparing `regis-0.1.8/regis/code_coverage.py` & `regis-0.1.9/regis/code_coverage.py`

 * *Files identical despite different names*

### Comparing `regis-0.1.8/regis/diagnostics.py` & `regis-0.1.9/regis/diagnostics.py`

 * *Files identical despite different names*

### Comparing `regis-0.1.8/regis/generation.py` & `regis-0.1.9/regis/generation.py`

 * *Files identical despite different names*

### Comparing `regis-0.1.8/regis/git_hooks.py` & `regis-0.1.9/regis/git_hooks.py`

 * *Files identical despite different names*

### Comparing `regis-0.1.8/regis/install_externals.py` & `regis-0.1.9/regis/install_externals.py`

 * *Files identical despite different names*

### Comparing `regis-0.1.8/regis/required_libs.py` & `regis-0.1.9/regis/required_libs.py`

 * *Files identical despite different names*

### Comparing `regis-0.1.8/regis/required_tools.py` & `regis-0.1.9/regis/required_tools.py`

 * *Files identical despite different names*

### Comparing `regis-0.1.8/regis/run_clang_format.py` & `regis-0.1.9/regis/run_clang_format.py`

 * *Files identical despite different names*

### Comparing `regis-0.1.8/regis/run_clang_tidy.py` & `regis-0.1.9/regis/run_clang_tidy.py`

 * *Files identical despite different names*

### Comparing `regis-0.1.8/regis/run_clang_tools.py` & `regis-0.1.9/regis/run_clang_tools.py`

 * *Files identical despite different names*

### Comparing `regis-0.1.8/regis/setup.py` & `regis-0.1.9/regis/setup.py`

 * *Files identical despite different names*

### Comparing `regis-0.1.8/regis/subproc.py` & `regis-0.1.9/regis/subproc.py`

 * *Files identical despite different names*

### Comparing `regis-0.1.8/regis/test.py` & `regis-0.1.9/regis/test.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,19 +4,18 @@
 # Twitter: @nick_debreuck
 # 
 # File: test.py
 # Copyright (c) Nick De Breuck 2023
 #
 # ============================================
 
-import argparse
 import os
-import traceback
-import shutil
+import threading
 import time
+import signal
 import regis.required_tools
 import regis.util
 import regis.task_raii_printing
 import regis.rex_json
 import regis.code_coverage
 import regis.diagnostics
 import regis.generation
@@ -162,22 +161,44 @@
   for project in projects:
     for config in configs:
       for compiler in compilers:
         result |= regis.build.new_build(project, config, compiler, should_clean)
 
   return result
 
+def __build_non_test_files(configs : [str], compilers : [str]):
+  should_clean = False
+
+  result = 0
+
+  intermediate_folder = settings["intermediate_folder"]
+  build_folder = settings["build_folder"]
+
+  directory = os.path.join(root_path, intermediate_folder, build_folder, "ninja")
+  projects = __find_projects_with_suffix(directory, "")
+
+  for project in projects:
+    # skip all test projects
+    if "test" in project or "_asan" in project or "_ubsan" in project or "_fuzzy" in project:
+      continue
+
+    for config in configs:
+      for compiler in compilers:
+        result |= regis.build.new_build(project, config, compiler, should_clean)
+
+  return result
+
 def __find_test_programs(folder, regex):
   intermediate_folder = os.path.join(folder)
   regis.diagnostics.log_info(f"looking for executables in {os.path.join(root_path, intermediate_folder)}")
   result = regis.util.find_all_files_in_folder(os.path.join(root_path, intermediate_folder), regex)
-  coverage_programs = []
+  coverage_programs : list[str] = []
   for res in result:
     if regis.util.is_executable(res):
-      coverage_programs.append(res.absolute())
+      coverage_programs.append(res.absolute().__str__())
 
   return coverage_programs
 
 # unit tests
 def __generate_tests():
   task_print = regis.task_raii_printing.TaskRaiiPrint("generating unit test projects")
   return __generate_test_files("/generateUnitTests")
@@ -390,14 +411,68 @@
         regis.diagnostics.log_err(f"issues found while fuzzing!")
         regis.diagnostics.log_err(f"for more info, please check: {log_file_path}")
       new_rc = 1
     rc |= new_rc
 
   return rc
 
+# auto tests
+def __generate_auto_tests():
+  task_print = regis.task_raii_printing.TaskRaiiPrint("generating auto tests")
+  return __generate_test_files("/noCompilerDB")
+
+def __build_auto_tests():
+  task_print = regis.task_raii_printing.TaskRaiiPrint("building auto tests")
+  return __build_non_test_files(["debug", "debug_opt", "release"], ["msvc", "clang"])
+
+def __run_auto_tests(timeoutInSeconds):
+  task_print = regis.task_raii_printing.TaskRaiiPrint("running auto tests")
+  unit_test_programs = __find_test_programs(os.path.join(settings["intermediate_folder"], settings["build_folder"], "ninja"), "*")
+  
+  rc = 0
+  for program in unit_test_programs:
+    if "test" in program or "_asan" in program or "_ubsan" in program or "_fuzzy" in program:
+      continue
+
+    regis.diagnostics.log_info(f"running: {Path(program).name}")
+    proc = regis.util.run_subprocess(program)
+
+    # wait for program to finish on a different thread so we can terminate it on timeout
+    thread = threading.Thread(target=lambda: proc.wait())
+    thread.start()
+
+    # wait for timeout to trigger or until the program exits
+    now = time.time()
+    duration = 0
+    killed_process = False
+    max_seconds = timeoutInSeconds
+    while True:
+      duration = time.time() - now
+      if not thread.is_alive():
+        break
+      
+      if duration > max_seconds:
+        proc.terminate() 
+        killed_process = True
+        break
+
+    # makes sure that we get an error code even if the program crashed
+    proc.communicate()
+    new_rc = proc.returncode
+    
+    if new_rc != 0:
+      if killed_process:
+        regis.diagnostics.log_warn(f"auto test timeout triggered for {program} after {max_seconds} seconds") # use full path to avoid ambiguity
+      else:
+        rc |= new_rc
+        regis.diagnostics.log_err(f"auto test failed for {program} with returncode {new_rc}") # use full path to avoid ambiguity
+
+  return rc
+
+# public API
 def test_include_what_you_use():
   regis.diagnostics.log_no_color("-----------------------------------------------------------------------------")
   rc = __run_include_what_you_use()
 
   if rc != 0:
     regis.diagnostics.log_err(f"include-what-you-use pass failed")
 
@@ -517,14 +592,27 @@
   
   regis.diagnostics.log_no_color("-----------------------------------------------------------------------------")
   rc |= __run_fuzzy_testing() # works
   if rc != 0:
     regis.diagnostics.log_err(f"invalid code found with fuzzy")
   __pass_results["fuzzy testing result"] = rc
 
-def __shutil_error(func, path, exec_info):
-  regis.diagnostics.log_err(f"shutil error: {func}, {path}, {exec_info}")
+def run_auto_tests(timeoutInSeconds : int):
+  rc = 0
 
-def clean():
-  intermediate_tests_path = os.path.join(root_path, settings["intermediate_folder"], settings["build_folder"])
-  if os.path.exists(intermediate_tests_path):
-    shutil.rmtree(intermediate_tests_path, onerror=__shutil_error)
+  regis.diagnostics.log_no_color("-----------------------------------------------------------------------------")
+  rc = __generate_auto_tests() # works
+  if rc != 0:
+    regis.diagnostics.log_err(f"failed to generate auto test code")
+  __pass_results["auto testing generation"] = rc
+  
+  regis.diagnostics.log_no_color("-----------------------------------------------------------------------------")
+  rc |= __build_auto_tests() # works
+  if rc != 0:
+    regis.diagnostics.log_err(f"failed to build auto test code")
+  __pass_results["auto testing building"] = rc
+  
+  regis.diagnostics.log_no_color("-----------------------------------------------------------------------------")
+  rc |= __run_auto_tests(timeoutInSeconds) # works
+  if rc != 0:
+    regis.diagnostics.log_err(f"auto tests failed")
+  __pass_results["auto testing result"] = rc
```

### Comparing `regis-0.1.8/regis/util.py` & `regis-0.1.9/regis/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,14 +135,15 @@
   return files_with_extension
 
 def is_windows():
   return os.name == 'nt'
 
 def run_subprocess(command):
   proc = subprocess.Popen(command)
+  proc.communicate()
   return proc
 
 def run_subprocess_with_working_dir(command, workingDir):
   proc = subprocess.Popen(command, cwd=workingDir)
   return proc
 
 def run_subprocess_with_callback(command, callback):
```

### Comparing `regis-0.1.8/.gitignore` & `regis-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `regis-0.1.8/LICENSE` & `regis-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `regis-0.1.8/pyproject.toml` & `regis-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "regis"
-version = "0.1.8"
+version = "0.1.9"
 authors = [
   { name="Nick De Breuck", email="nick.debreuck@outlook.com" },
 ]
 description = "python framework used by Rex Engine"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `regis-0.1.8/PKG-INFO` & `regis-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: regis
-Version: 0.1.8
+Version: 0.1.9
 Summary: python framework used by Rex Engine
 Project-URL: Homepage, https://github.com/RisingLiberty/RexPy
 Project-URL: Bug Tracker, https://github.com/RisingLiberty/RexPy/issues
 Author-email: Nick De Breuck <nick.debreuck@outlook.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

