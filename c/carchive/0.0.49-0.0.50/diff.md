# Comparing `tmp/carchive-0.0.49.tar.gz` & `tmp/carchive-0.0.50.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carchive-0.0.49.tar", last modified: Mon May  8 16:07:16 2023, max compression
+gzip compressed data, was "carchive-0.0.50.tar", last modified: Mon May  8 16:11:36 2023, max compression
```

## Comparing `carchive-0.0.49.tar` & `carchive-0.0.50.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:07:16.310242 carchive-0.0.49/
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-08 16:07:12.000000 carchive-0.0.49/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-08 16:07:16.310242 carchive-0.0.49/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-08 16:07:12.000000 carchive-0.0.49/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:07:16.310242 carchive-0.0.49/carchive/
--rwxr-xr-x   0 runner    (1001) docker     (123)    10060 2023-05-08 16:07:12.000000 carchive-0.0.49/carchive/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:07:16.310242 carchive-0.0.49/carchive.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-08 16:07:16.000000 carchive-0.0.49/carchive.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-08 16:07:16.000000 carchive-0.0.49/carchive.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 16:07:16.000000 carchive-0.0.49/carchive.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-08 16:07:16.000000 carchive-0.0.49/carchive.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-08 16:07:16.000000 carchive-0.0.49/carchive.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 16:07:16.310242 carchive-0.0.49/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3397 2023-05-08 16:07:12.000000 carchive-0.0.49/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:11:36.360542 carchive-0.0.50/
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-08 16:11:31.000000 carchive-0.0.50/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-08 16:11:36.356542 carchive-0.0.50/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-08 16:11:31.000000 carchive-0.0.50/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:11:36.356542 carchive-0.0.50/carchive/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10078 2023-05-08 16:11:31.000000 carchive-0.0.50/carchive/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:11:36.356542 carchive-0.0.50/carchive.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-08 16:11:36.000000 carchive-0.0.50/carchive.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-08 16:11:36.000000 carchive-0.0.50/carchive.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 16:11:36.000000 carchive-0.0.50/carchive.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-08 16:11:36.000000 carchive-0.0.50/carchive.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-08 16:11:36.000000 carchive-0.0.50/carchive.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 16:11:36.360542 carchive-0.0.50/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3397 2023-05-08 16:11:31.000000 carchive-0.0.50/setup.py
```

### Comparing `carchive-0.0.49/LICENSE` & `carchive-0.0.50/LICENSE`

 * *Files identical despite different names*

### Comparing `carchive-0.0.49/carchive/__init__.py` & `carchive-0.0.50/carchive/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -225,15 +225,15 @@
 			search_limits = getattr(extra_rate_limiting, "search")
 			if search_limits.remaining < 2:
 				print("Waiting until: {0}".format(search_limits.reset))
 				pause.until(search_limits.reset)
 	
 	def repair(self,path,create:bool=True):
 		if self.delete_paths and os.path.exists(path):
-			os.remove(path)
+			os.system("yes|rm -r "+str(path))
 		if create:
 			os.makedirs(path, exist_ok=True)
 
 	def __call__(self, search_string:str):
 		self.timing
 		search_string = mystring.string(search_string)
```

### Comparing `carchive-0.0.49/setup.py` & `carchive-0.0.50/setup.py`

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
-VERSION = "0.0.49"
+VERSION = "0.0.50"
 
 def zip_program(outputName:str = f"{NAME}.zip"):
 	#http://blog.ablepear.com/2012/10/bundling-python-files-into-stand-alone.html
 	if os.path.exists(outputName):
 		os.system(f"rm {outputName}")
 
 	zipf = zipfile.ZipFile(outputName, 'w', zipfile.ZIP_DEFLATED)
```

