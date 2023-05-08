# Comparing `tmp/carchive-0.0.48.tar.gz` & `tmp/carchive-0.0.49.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carchive-0.0.48.tar", last modified: Mon May  8 16:00:11 2023, max compression
+gzip compressed data, was "carchive-0.0.49.tar", last modified: Mon May  8 16:07:16 2023, max compression
```

## Comparing `carchive-0.0.48.tar` & `carchive-0.0.49.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:00:11.277433 carchive-0.0.48/
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-08 16:00:06.000000 carchive-0.0.48/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-08 16:00:11.277433 carchive-0.0.48/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-08 16:00:06.000000 carchive-0.0.48/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:00:11.277433 carchive-0.0.48/carchive/
--rwxr-xr-x   0 runner    (1001) docker     (123)    10035 2023-05-08 16:00:06.000000 carchive-0.0.48/carchive/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:00:11.277433 carchive-0.0.48/carchive.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-08 16:00:11.000000 carchive-0.0.48/carchive.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-08 16:00:11.000000 carchive-0.0.48/carchive.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 16:00:11.000000 carchive-0.0.48/carchive.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-08 16:00:11.000000 carchive-0.0.48/carchive.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-08 16:00:11.000000 carchive-0.0.48/carchive.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 16:00:11.277433 carchive-0.0.48/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3397 2023-05-08 16:00:06.000000 carchive-0.0.48/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:07:16.310242 carchive-0.0.49/
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-08 16:07:12.000000 carchive-0.0.49/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-08 16:07:16.310242 carchive-0.0.49/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-08 16:07:12.000000 carchive-0.0.49/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:07:16.310242 carchive-0.0.49/carchive/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10060 2023-05-08 16:07:12.000000 carchive-0.0.49/carchive/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:07:16.310242 carchive-0.0.49/carchive.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-08 16:07:16.000000 carchive-0.0.49/carchive.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-08 16:07:16.000000 carchive-0.0.49/carchive.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 16:07:16.000000 carchive-0.0.49/carchive.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-08 16:07:16.000000 carchive-0.0.49/carchive.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-08 16:07:16.000000 carchive-0.0.49/carchive.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 16:07:16.310242 carchive-0.0.49/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3397 2023-05-08 16:07:12.000000 carchive-0.0.49/setup.py
```

### Comparing `carchive-0.0.48/LICENSE` & `carchive-0.0.49/LICENSE`

 * *Files identical despite different names*

### Comparing `carchive-0.0.48/carchive/__init__.py` & `carchive-0.0.49/carchive/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -224,15 +224,15 @@
 		if hasattr(extra_rate_limiting, "search"):
 			search_limits = getattr(extra_rate_limiting, "search")
 			if search_limits.remaining < 2:
 				print("Waiting until: {0}".format(search_limits.reset))
 				pause.until(search_limits.reset)
 	
 	def repair(self,path,create:bool=True):
-		if self.delete_paths:
+		if self.delete_paths and os.path.exists(path):
 			os.remove(path)
 		if create:
 			os.makedirs(path, exist_ok=True)
 
 	def __call__(self, search_string:str):
 		self.timing
 		search_string = mystring.string(search_string)
```

### Comparing `carchive-0.0.48/setup.py` & `carchive-0.0.49/setup.py`

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
-VERSION = "0.0.48"
+VERSION = "0.0.49"
 
 def zip_program(outputName:str = f"{NAME}.zip"):
 	#http://blog.ablepear.com/2012/10/bundling-python-files-into-stand-alone.html
 	if os.path.exists(outputName):
 		os.system(f"rm {outputName}")
 
 	zipf = zipfile.ZipFile(outputName, 'w', zipfile.ZIP_DEFLATED)
```

