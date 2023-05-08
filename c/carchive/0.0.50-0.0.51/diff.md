# Comparing `tmp/carchive-0.0.50.tar.gz` & `tmp/carchive-0.0.51.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carchive-0.0.50.tar", last modified: Mon May  8 16:11:36 2023, max compression
+gzip compressed data, was "carchive-0.0.51.tar", last modified: Mon May  8 16:21:59 2023, max compression
```

## Comparing `carchive-0.0.50.tar` & `carchive-0.0.51.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:11:36.360542 carchive-0.0.50/
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-08 16:11:31.000000 carchive-0.0.50/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-08 16:11:36.356542 carchive-0.0.50/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-08 16:11:31.000000 carchive-0.0.50/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:11:36.356542 carchive-0.0.50/carchive/
--rwxr-xr-x   0 runner    (1001) docker     (123)    10078 2023-05-08 16:11:31.000000 carchive-0.0.50/carchive/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:11:36.356542 carchive-0.0.50/carchive.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-08 16:11:36.000000 carchive-0.0.50/carchive.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-08 16:11:36.000000 carchive-0.0.50/carchive.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 16:11:36.000000 carchive-0.0.50/carchive.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-08 16:11:36.000000 carchive-0.0.50/carchive.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-08 16:11:36.000000 carchive-0.0.50/carchive.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 16:11:36.360542 carchive-0.0.50/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3397 2023-05-08 16:11:31.000000 carchive-0.0.50/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:21:59.127783 carchive-0.0.51/
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-08 16:21:52.000000 carchive-0.0.51/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-08 16:21:59.127783 carchive-0.0.51/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-08 16:21:52.000000 carchive-0.0.51/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:21:59.127783 carchive-0.0.51/carchive/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10063 2023-05-08 16:21:52.000000 carchive-0.0.51/carchive/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:21:59.127783 carchive-0.0.51/carchive.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-08 16:21:59.000000 carchive-0.0.51/carchive.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-08 16:21:59.000000 carchive-0.0.51/carchive.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 16:21:59.000000 carchive-0.0.51/carchive.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-08 16:21:59.000000 carchive-0.0.51/carchive.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-08 16:21:59.000000 carchive-0.0.51/carchive.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 16:21:59.127783 carchive-0.0.51/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3397 2023-05-08 16:21:52.000000 carchive-0.0.51/setup.py
```

### Comparing `carchive-0.0.50/LICENSE` & `carchive-0.0.51/LICENSE`

 * *Files identical despite different names*

### Comparing `carchive-0.0.50/carchive/__init__.py` & `carchive-0.0.51/carchive/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -254,15 +254,15 @@
 
 				if self.num_processes is None:
 					git2net.mine_git_repo(repo_dir, sqlite_db_file)
 				else:
 					git2net.mine_git_repo(repo_dir, sqlite_db_file, no_of_processes=self.num_processes)
 
 				git2net.disambiguate_aliases_db(sqlite_db_file)
-				git2net.compute_complexity(repo_dir, sqlite_db_file, extra_eval_methods=[x() for x in self.metrics])
+				git2net.compute_complexity(repo_dir, sqlite_db_file, extra_eval_methods=self.metrics)
 
 				if os.stat(sqlite_db_file).st_size > 100_000_000:
 					with mystring.foldentre(new_path=results_dir):
 						raw_db_file = sqlite_db_file.replace(results_dir, '')
 						splittr.hash(raw_db_file)
 						splittr.split(raw_db_file, 50_000_000)
 						splittr.template(raw_db_file+".py")
```

### Comparing `carchive-0.0.50/setup.py` & `carchive-0.0.51/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 DESCRIPTION = 'My short description for my project.'
 GH_NAME = "franceme"
 URL = f"https://github.com/{GH_NAME}/{NAME}"
 long_description = pathlib.Path(f"{here}/README.md").read_text(encoding='utf-8')
 REQUIRES_PYTHON = '>=3.8.0'
 RELEASE = "?"
 entry_point = f"src.{NAME}"
-VERSION = "0.0.50"
+VERSION = "0.0.51"
 
 def zip_program(outputName:str = f"{NAME}.zip"):
 	#http://blog.ablepear.com/2012/10/bundling-python-files-into-stand-alone.html
 	if os.path.exists(outputName):
 		os.system(f"rm {outputName}")
 
 	zipf = zipfile.ZipFile(outputName, 'w', zipfile.ZIP_DEFLATED)
```

