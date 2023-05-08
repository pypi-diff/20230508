# Comparing `tmp/carchive-0.0.52.tar.gz` & `tmp/carchive-0.0.53.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carchive-0.0.52.tar", last modified: Mon May  8 16:42:48 2023, max compression
+gzip compressed data, was "carchive-0.0.53.tar", last modified: Mon May  8 19:15:55 2023, max compression
```

## Comparing `carchive-0.0.52.tar` & `carchive-0.0.53.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:42:48.478665 carchive-0.0.52/
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-08 16:42:44.000000 carchive-0.0.52/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-08 16:42:48.478665 carchive-0.0.52/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-08 16:42:44.000000 carchive-0.0.52/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:42:48.478665 carchive-0.0.52/carchive/
--rwxr-xr-x   0 runner    (1001) docker     (123)    10082 2023-05-08 16:42:44.000000 carchive-0.0.52/carchive/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:42:48.478665 carchive-0.0.52/carchive.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-08 16:42:48.000000 carchive-0.0.52/carchive.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-08 16:42:48.000000 carchive-0.0.52/carchive.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 16:42:48.000000 carchive-0.0.52/carchive.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-08 16:42:48.000000 carchive-0.0.52/carchive.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-08 16:42:48.000000 carchive-0.0.52/carchive.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 16:42:48.478665 carchive-0.0.52/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3397 2023-05-08 16:42:44.000000 carchive-0.0.52/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:15:55.684553 carchive-0.0.53/
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-08 19:15:48.000000 carchive-0.0.53/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-08 19:15:55.684553 carchive-0.0.53/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-08 19:15:48.000000 carchive-0.0.53/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:15:55.684553 carchive-0.0.53/carchive/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10131 2023-05-08 19:15:48.000000 carchive-0.0.53/carchive/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:15:55.684553 carchive-0.0.53/carchive.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-08 19:15:55.000000 carchive-0.0.53/carchive.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-08 19:15:55.000000 carchive-0.0.53/carchive.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 19:15:55.000000 carchive-0.0.53/carchive.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-08 19:15:55.000000 carchive-0.0.53/carchive.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-08 19:15:55.000000 carchive-0.0.53/carchive.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 19:15:55.684553 carchive-0.0.53/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3397 2023-05-08 19:15:48.000000 carchive-0.0.53/setup.py
```

### Comparing `carchive-0.0.52/LICENSE` & `carchive-0.0.53/LICENSE`

 * *Files identical despite different names*

### Comparing `carchive-0.0.52/carchive/__init__.py` & `carchive-0.0.53/carchive/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -177,14 +177,18 @@
 	@property
 	def webarchive_save_url(self,):
 		return mystring.string("https://web.archive.org/save/" + self.zip_url)
 
 T = TypeVar('T')
 class GRepo_Seed_Metric(ABC, Generic[T]):
 	@abstractmethod
+	def name(self) -> str:
+		pass
+
+	@abstractmethod
 	def metric(self, filename: str, source_code: str) -> Dict[str, T]:
 		pass
 
 	@abstractmethod
 	def diff(self, latest: T, previous: T):
 		pass
```

### Comparing `carchive-0.0.52/setup.py` & `carchive-0.0.53/setup.py`

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
-VERSION = "0.0.52"
+VERSION = "0.0.53"
 
 def zip_program(outputName:str = f"{NAME}.zip"):
 	#http://blog.ablepear.com/2012/10/bundling-python-files-into-stand-alone.html
 	if os.path.exists(outputName):
 		os.system(f"rm {outputName}")
 
 	zipf = zipfile.ZipFile(outputName, 'w', zipfile.ZIP_DEFLATED)
```

