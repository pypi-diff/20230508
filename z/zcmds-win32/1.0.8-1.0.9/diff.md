# Comparing `tmp/zcmds_win32-1.0.8.tar.gz` & `tmp/zcmds_win32-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zcmds_win32-1.0.8.tar", last modified: Mon Mar  6 08:08:21 2023, max compression
+gzip compressed data, was "zcmds_win32-1.0.9.tar", last modified: Mon Mar 13 07:48:06 2023, max compression
```

## Comparing `zcmds_win32-1.0.8.tar` & `zcmds_win32-1.0.9.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-03-06 08:08:21.635553 zcmds_win32-1.0.8/
--rw-rw-rw-   0        0        0     1799 2022-10-15 22:06:33.000000 zcmds_win32-1.0.8/.gitignore
-drwxrwxrwx   0        0        0        0 2023-03-06 08:08:21.597931 zcmds_win32-1.0.8/.vscode/
--rw-rw-rw-   0        0        0      833 2023-03-06 04:33:48.000000 zcmds_win32-1.0.8/.vscode/settings.json
--rw-rw-rw-   0        0        0     1259 2023-03-06 08:08:21.634551 zcmds_win32-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      850 2023-03-06 08:08:06.000000 zcmds_win32-1.0.8/README.md
--rw-rw-rw-   0        0        0     1058 2023-03-06 08:07:23.000000 zcmds_win32-1.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       28 2022-02-21 03:22:36.000000 zcmds_win32-1.0.8/requirements.testing.txt
--rw-rw-rw-   0        0        0        0 2022-10-15 20:56:38.000000 zcmds_win32-1.0.8/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-03-06 08:08:21.635553 zcmds_win32-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0       77 2023-01-03 07:29:58.000000 zcmds_win32-1.0.8/setup.py
--rw-rw-rw-   0        0        0      465 2022-11-28 03:18:18.000000 zcmds_win32-1.0.8/tox.ini
--rw-rw-rw-   0        0        0      249 2023-03-06 08:05:13.000000 zcmds_win32-1.0.8/upload_package.sh
-drwxrwxrwx   0        0        0        0 2023-03-06 08:08:21.620552 zcmds_win32-1.0.8/zcmds_win32/
--rw-rw-rw-   0        0        0        0 2022-02-21 10:38:44.000000 zcmds_win32-1.0.8/zcmds_win32/__init__.py
--rw-rw-rw-   0        0        0      343 2023-02-22 21:00:08.000000 zcmds_win32-1.0.8/zcmds_win32/_exec.py
--rw-rw-rw-   0        0        0      130 2022-10-15 22:21:22.000000 zcmds_win32-1.0.8/zcmds_win32/cat.py
--rw-rw-rw-   0        0        0      129 2022-10-15 22:21:22.000000 zcmds_win32-1.0.8/zcmds_win32/cp.py
--rw-rw-rw-   0        0        0      129 2022-10-15 22:21:22.000000 zcmds_win32-1.0.8/zcmds_win32/du.py
--rw-rw-rw-   0        0        0      292 2023-03-06 08:05:13.000000 zcmds_win32-1.0.8/zcmds_win32/fixvmmem.py
--rw-rw-rw-   0        0        0      322 2022-08-06 19:05:58.000000 zcmds_win32-1.0.8/zcmds_win32/git_bash.py
--rw-rw-rw-   0        0        0      131 2022-10-15 22:21:22.000000 zcmds_win32-1.0.8/zcmds_win32/grep.py
--rw-rw-rw-   0        0        0      168 2022-10-15 22:21:22.000000 zcmds_win32-1.0.8/zcmds_win32/home.py
--rw-rw-rw-   0        0        0      129 2022-10-15 22:21:22.000000 zcmds_win32-1.0.8/zcmds_win32/ls.py
--rw-rw-rw-   0        0        0      129 2022-10-15 22:21:22.000000 zcmds_win32-1.0.8/zcmds_win32/mv.py
--rw-rw-rw-   0        0        0      131 2023-01-03 07:29:12.000000 zcmds_win32-1.0.8/zcmds_win32/nano.py
--rw-rw-rw-   0        0        0      202 2023-03-06 08:06:58.000000 zcmds_win32-1.0.8/zcmds_win32/open.py
--rw-rw-rw-   0        0        0      131 2023-01-03 07:29:03.000000 zcmds_win32-1.0.8/zcmds_win32/pico.py
--rw-rw-rw-   0        0        0      129 2022-10-15 22:21:22.000000 zcmds_win32-1.0.8/zcmds_win32/rm.py
--rw-rw-rw-   0        0        0      142 2022-08-09 06:13:38.000000 zcmds_win32-1.0.8/zcmds_win32/touch.py
--rw-rw-rw-   0        0        0      132 2022-10-15 22:21:22.000000 zcmds_win32-1.0.8/zcmds_win32/unzip.py
--rw-rw-rw-   0        0        0      112 2022-10-15 21:20:31.000000 zcmds_win32-1.0.8/zcmds_win32/version.py
--rw-rw-rw-   0        0        0       99 2022-10-15 22:21:22.000000 zcmds_win32-1.0.8/zcmds_win32/which.py
-drwxrwxrwx   0        0        0        0 2023-03-06 08:08:21.633552 zcmds_win32-1.0.8/zcmds_win32.egg-info/
--rw-rw-rw-   0        0        0     1259 2023-03-06 08:08:21.000000 zcmds_win32-1.0.8/zcmds_win32.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      700 2023-03-06 08:08:21.000000 zcmds_win32-1.0.8/zcmds_win32.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-06 08:08:21.000000 zcmds_win32-1.0.8/zcmds_win32.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      482 2023-03-06 08:08:21.000000 zcmds_win32-1.0.8/zcmds_win32.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       12 2023-03-06 08:08:21.000000 zcmds_win32-1.0.8/zcmds_win32.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-03-13 07:48:06.673760 zcmds_win32-1.0.9/
+-rw-rw-rw-   0        0        0     1799 2022-10-15 22:06:33.000000 zcmds_win32-1.0.9/.gitignore
+drwxrwxrwx   0        0        0        0 2023-03-13 07:48:06.635761 zcmds_win32-1.0.9/.vscode/
+-rw-rw-rw-   0        0        0      833 2023-03-06 04:33:48.000000 zcmds_win32-1.0.9/.vscode/settings.json
+-rw-rw-rw-   0        0        0     1311 2023-03-13 07:48:06.673760 zcmds_win32-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      901 2023-03-13 07:47:32.000000 zcmds_win32-1.0.9/README.md
+-rw-rw-rw-   0        0        0     1058 2023-03-13 07:47:18.000000 zcmds_win32-1.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       28 2022-02-21 03:22:36.000000 zcmds_win32-1.0.9/requirements.testing.txt
+-rw-rw-rw-   0        0        0        0 2022-10-15 20:56:38.000000 zcmds_win32-1.0.9/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-03-13 07:48:06.674762 zcmds_win32-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0       77 2023-01-03 07:29:58.000000 zcmds_win32-1.0.9/setup.py
+-rw-rw-rw-   0        0        0      465 2022-11-28 03:18:18.000000 zcmds_win32-1.0.9/tox.ini
+-rw-rw-rw-   0        0        0      249 2023-03-06 08:05:13.000000 zcmds_win32-1.0.9/upload_package.sh
+drwxrwxrwx   0        0        0        0 2023-03-13 07:48:06.658762 zcmds_win32-1.0.9/zcmds_win32/
+-rw-rw-rw-   0        0        0        0 2022-02-21 10:38:44.000000 zcmds_win32-1.0.9/zcmds_win32/__init__.py
+-rw-rw-rw-   0        0        0      343 2023-02-22 21:00:08.000000 zcmds_win32-1.0.9/zcmds_win32/_exec.py
+-rw-rw-rw-   0        0        0      130 2022-10-15 22:21:22.000000 zcmds_win32-1.0.9/zcmds_win32/cat.py
+-rw-rw-rw-   0        0        0      129 2022-10-15 22:21:22.000000 zcmds_win32-1.0.9/zcmds_win32/cp.py
+-rw-rw-rw-   0        0        0      129 2022-10-15 22:21:22.000000 zcmds_win32-1.0.9/zcmds_win32/du.py
+-rw-rw-rw-   0        0        0      292 2023-03-06 08:05:13.000000 zcmds_win32-1.0.9/zcmds_win32/fixvmmem.py
+-rw-rw-rw-   0        0        0      322 2022-08-06 19:05:58.000000 zcmds_win32-1.0.9/zcmds_win32/git_bash.py
+-rw-rw-rw-   0        0        0      131 2022-10-15 22:21:22.000000 zcmds_win32-1.0.9/zcmds_win32/grep.py
+-rw-rw-rw-   0        0        0      168 2022-10-15 22:21:22.000000 zcmds_win32-1.0.9/zcmds_win32/home.py
+-rw-rw-rw-   0        0        0      129 2022-10-15 22:21:22.000000 zcmds_win32-1.0.9/zcmds_win32/ls.py
+-rw-rw-rw-   0        0        0      129 2022-10-15 22:21:22.000000 zcmds_win32-1.0.9/zcmds_win32/mv.py
+-rw-rw-rw-   0        0        0      131 2023-01-03 07:29:12.000000 zcmds_win32-1.0.9/zcmds_win32/nano.py
+-rw-rw-rw-   0        0        0      349 2023-03-13 07:47:07.000000 zcmds_win32-1.0.9/zcmds_win32/open.py
+-rw-rw-rw-   0        0        0      131 2023-01-03 07:29:03.000000 zcmds_win32-1.0.9/zcmds_win32/pico.py
+-rw-rw-rw-   0        0        0      129 2022-10-15 22:21:22.000000 zcmds_win32-1.0.9/zcmds_win32/rm.py
+-rw-rw-rw-   0        0        0      142 2022-08-09 06:13:38.000000 zcmds_win32-1.0.9/zcmds_win32/touch.py
+-rw-rw-rw-   0        0        0      132 2022-10-15 22:21:22.000000 zcmds_win32-1.0.9/zcmds_win32/unzip.py
+-rw-rw-rw-   0        0        0      112 2022-10-15 21:20:31.000000 zcmds_win32-1.0.9/zcmds_win32/version.py
+-rw-rw-rw-   0        0        0       99 2022-10-15 22:21:22.000000 zcmds_win32-1.0.9/zcmds_win32/which.py
+drwxrwxrwx   0        0        0        0 2023-03-13 07:48:06.672761 zcmds_win32-1.0.9/zcmds_win32.egg-info/
+-rw-rw-rw-   0        0        0     1311 2023-03-13 07:48:06.000000 zcmds_win32-1.0.9/zcmds_win32.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      700 2023-03-13 07:48:06.000000 zcmds_win32-1.0.9/zcmds_win32.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-03-13 07:48:06.000000 zcmds_win32-1.0.9/zcmds_win32.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      482 2023-03-13 07:48:06.000000 zcmds_win32-1.0.9/zcmds_win32.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       12 2023-03-13 07:48:06.000000 zcmds_win32-1.0.9/zcmds_win32.egg-info/top_level.txt
```

### Comparing `zcmds_win32-1.0.8/.gitignore` & `zcmds_win32-1.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `zcmds_win32-1.0.8/.vscode/settings.json` & `zcmds_win32-1.0.9/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `zcmds_win32-1.0.8/PKG-INFO` & `zcmds_win32-1.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zcmds_win32
-Version: 1.0.8
+Version: 1.0.9
 Summary: Cross platform(ish) productivity commands written in python.
 License: BSD 3-Clause License
 Keywords: zcmds,win32,zcmds_win32,zcmds-win32,cli,command line,command line interface
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
@@ -42,14 +42,15 @@
 
   * `git clone https://github.com/zackees/zcmds_win32`
   * `cd zcmds_win32`
   * `python -pip install -e .`
 
 
 # Release Notes
+  * 1.0.9: Fixes `open` when using forward slashes
   * 1.0.8: Fixes `open` when using `open .`
   * 1.0.7: Fixes missing `fixvmmem`
   * 1.0.5: `open` now assumes current directory if no path is given
   * 1.0.4: `fixvmmem` now runs in elevated privledges
   * 1.0.3: Adds `fixvmmem`
   * 1.0.2: Adds `unzip`
   * 1.0.1: Adds `pico/nano`
```

### Comparing `zcmds_win32-1.0.8/README.md` & `zcmds_win32-1.0.9/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 
   * `git clone https://github.com/zackees/zcmds_win32`
   * `cd zcmds_win32`
   * `python -pip install -e .`
 
 
 # Release Notes
+  * 1.0.9: Fixes `open` when using forward slashes
   * 1.0.8: Fixes `open` when using `open .`
   * 1.0.7: Fixes missing `fixvmmem`
   * 1.0.5: `open` now assumes current directory if no path is given
   * 1.0.4: `fixvmmem` now runs in elevated privledges
   * 1.0.3: Adds `fixvmmem`
   * 1.0.2: Adds `unzip`
   * 1.0.1: Adds `pico/nano`
```

### Comparing `zcmds_win32-1.0.8/pyproject.toml` & `zcmds_win32-1.0.9/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 requires-python = ">=3.7"
 keywords = ["zcmds", "win32", "zcmds_win32", "zcmds-win32", "cli", "command line", "command line interface"]
 license = { text = "BSD 3-Clause License" }
 classifiers = ["Programming Language :: Python :: 3"]
 dependencies = [
 ]
 # Change this with the version number bump.
-version = "1.0.8"
+version = "1.0.9"
 
 [project.scripts]
 cat = "zcmds_win32.cat:main"
 cp = "zcmds_win32.cp:main"
 du = "zcmds_win32.du:main"
 grep = "zcmds_win32.grep:main"
 home = "zcmds_win32.home:main"
```

### Comparing `zcmds_win32-1.0.8/zcmds_win32.egg-info/PKG-INFO` & `zcmds_win32-1.0.9/zcmds_win32.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zcmds-win32
-Version: 1.0.8
+Version: 1.0.9
 Summary: Cross platform(ish) productivity commands written in python.
 License: BSD 3-Clause License
 Keywords: zcmds,win32,zcmds_win32,zcmds-win32,cli,command line,command line interface
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
@@ -42,14 +42,15 @@
 
   * `git clone https://github.com/zackees/zcmds_win32`
   * `cd zcmds_win32`
   * `python -pip install -e .`
 
 
 # Release Notes
+  * 1.0.9: Fixes `open` when using forward slashes
   * 1.0.8: Fixes `open` when using `open .`
   * 1.0.7: Fixes missing `fixvmmem`
   * 1.0.5: `open` now assumes current directory if no path is given
   * 1.0.4: `fixvmmem` now runs in elevated privledges
   * 1.0.3: Adds `fixvmmem`
   * 1.0.2: Adds `unzip`
   * 1.0.1: Adds `pico/nano`
```

### Comparing `zcmds_win32-1.0.8/zcmds_win32.egg-info/SOURCES.txt` & `zcmds_win32-1.0.9/zcmds_win32.egg-info/SOURCES.txt`

 * *Files identical despite different names*

