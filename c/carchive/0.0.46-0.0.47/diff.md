# Comparing `tmp/carchive-0.0.46.tar.gz` & `tmp/carchive-0.0.47.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carchive-0.0.46.tar", last modified: Fri May  5 03:20:43 2023, max compression
+gzip compressed data, was "carchive-0.0.47.tar", last modified: Fri May  5 20:01:58 2023, max compression
```

## Comparing `carchive-0.0.46.tar` & `carchive-0.0.47.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:20:43.786563 carchive-0.0.46/
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-05 03:20:39.000000 carchive-0.0.46/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-05 03:20:43.786563 carchive-0.0.46/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-05 03:20:39.000000 carchive-0.0.46/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:20:43.786563 carchive-0.0.46/carchive/
--rwxr-xr-x   0 runner    (1001) docker     (123)     9615 2023-05-05 03:20:39.000000 carchive-0.0.46/carchive/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:20:43.786563 carchive-0.0.46/carchive.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-05 03:20:43.000000 carchive-0.0.46/carchive.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-05 03:20:43.000000 carchive-0.0.46/carchive.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 03:20:43.000000 carchive-0.0.46/carchive.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-05 03:20:43.000000 carchive-0.0.46/carchive.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-05 03:20:43.000000 carchive-0.0.46/carchive.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 03:20:43.786563 carchive-0.0.46/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3397 2023-05-05 03:20:39.000000 carchive-0.0.46/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:01:58.629179 carchive-0.0.47/
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-05 20:01:54.000000 carchive-0.0.47/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-05 20:01:58.625179 carchive-0.0.47/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-05 20:01:54.000000 carchive-0.0.47/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:01:58.625179 carchive-0.0.47/carchive/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9813 2023-05-05 20:01:54.000000 carchive-0.0.47/carchive/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:01:58.625179 carchive-0.0.47/carchive.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-05 20:01:58.000000 carchive-0.0.47/carchive.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-05 20:01:58.000000 carchive-0.0.47/carchive.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 20:01:58.000000 carchive-0.0.47/carchive.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-05 20:01:58.000000 carchive-0.0.47/carchive.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-05 20:01:58.000000 carchive-0.0.47/carchive.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 20:01:58.629179 carchive-0.0.47/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3397 2023-05-05 20:01:54.000000 carchive-0.0.47/setup.py
```

### Comparing `carchive-0.0.46/LICENSE` & `carchive-0.0.47/LICENSE`

 * *Files identical despite different names*

### Comparing `carchive-0.0.46/carchive/__init__.py` & `carchive-0.0.47/carchive/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -190,27 +190,28 @@
 
 	def __call__(self):
 		setattr(self.metric, 'diff', self.diff)
 		return self.metric
 
 
 class GRepo_Pod(object):
-	def __init__(self, metrics:List[GRepo_Seed_Metric], token:str=None):
+	def __init__(self, metrics:List[GRepo_Seed_Metric], token:str=None,num_processes:int = None):
 		self.metrics = metrics
 		self.token = token
 		if "GH_TOKEN" not in os.environ:
 			self.login()
 
 		self.g = Github(self.token)
 		self.processor = mystring.MyThreads(10)
 		self.processed_paths = queue.Queue()
 		setattr(self.processed_paths, 'lock', threading.Lock())
 
 		self.current_repo_itr = None
 		self.total_repo_len = None
+		self.num_processes = num_processes
 
 		def appr(string: mystring.string):
 			with open("mapping_file_{0}.csv".format(string.tobase64()), "a+") as writer:
 				writer.write(string)
 		self.appr = appr
 		self.api_watch = niceghapi()
 	
@@ -237,15 +238,19 @@
 				repo_dir = "repo_" + str(name.tobase64())
 				results_dir = "results_" + str(name.tobase64())
 				os.makedirs(results_dir, exist_ok=True)
 				sqlite_db_file = os.path.join(results_dir, "git_to_net.sqlite")
 
 				git2.clone_repository(repo.clone_url, repo_dir)  # Clones a non-bare repository
 
-				git2net.mine_git_repo(repo_dir, sqlite_db_file)
+				if self.num_processes is None:
+					git2net.mine_git_repo(repo_dir, sqlite_db_file)
+				else:
+					git2net.mine_git_repo(repo_dir, sqlite_db_file, no_of_processes=self.num_processes)
+
 				git2net.disambiguate_aliases_db(sqlite_db_file)
 				git2net.compute_complexity(repo_dir, sqlite_db_file, extra_eval_methods=[x() for x in self.metrics])
 
 				if os.stat(sqlite_db_file).st_size > 100_000_000:
 					with mystring.foldentre(new_path=results_dir):
 						raw_db_file = sqlite_db_file.replace(results_dir, '')
 						splittr.hash(raw_db_file)
```

### Comparing `carchive-0.0.46/setup.py` & `carchive-0.0.47/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 DESCRIPTION = 'My short description for my project.'
 GH_NAME = "franceme"
 URL = f"https://github.com/{GH_NAME}/{NAME}"
 long_description = pathlib.Path(f"{here}/README.md").read_text(encoding='utf-8')
 REQUIRES_PYTHON = '>=3.8.0'
 RELEASE = "?"
 entry_point = f"src.{NAME}"
-VERSION = "0.0.46"
+VERSION = "0.0.47"
 
 def zip_program(outputName:str = f"{NAME}.zip"):
 	#http://blog.ablepear.com/2012/10/bundling-python-files-into-stand-alone.html
 	if os.path.exists(outputName):
 		os.system(f"rm {outputName}")
 
 	zipf = zipfile.ZipFile(outputName, 'w', zipfile.ZIP_DEFLATED)
```

