# Comparing `tmp/plain_db-0.0.8.tar.gz` & `tmp/plain_db-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/plain_db-0.0.8.tar", last modified: Tue Jul 14 23:02:31 2020, max compression
+gzip compressed data, was "dist/plain_db-0.0.9.tar", last modified: Wed Jul 15 00:49:52 2020, max compression
```

## Comparing `plain_db-0.0.8.tar` & `plain_db-0.0.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 yunzhi   (672583) primarygroup (89939)        0 2020-07-14 23:02:31.000000 plain_db-0.0.8/
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      770 2020-07-14 23:02:31.000000 plain_db-0.0.8/PKG-INFO
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      208 2020-07-07 18:39:37.000000 plain_db-0.0.8/README.md
-drwxr-xr-x   0 yunzhi   (672583) primarygroup (89939)        0 2020-07-14 23:02:31.000000 plain_db-0.0.8/plain_db/
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)     1748 2020-07-14 23:02:14.000000 plain_db-0.0.8/plain_db/__init__.py
-drwxr-xr-x   0 yunzhi   (672583) primarygroup (89939)        0 2020-07-14 23:02:31.000000 plain_db-0.0.8/plain_db.egg-info/
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      770 2020-07-14 23:02:31.000000 plain_db-0.0.8/plain_db.egg-info/PKG-INFO
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      167 2020-07-14 23:02:31.000000 plain_db-0.0.8/plain_db.egg-info/SOURCES.txt
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)        1 2020-07-14 23:02:31.000000 plain_db-0.0.8/plain_db.egg-info/dependency_links.txt
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)        9 2020-07-14 23:02:31.000000 plain_db-0.0.8/plain_db.egg-info/top_level.txt
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)       38 2020-07-14 23:02:31.000000 plain_db-0.0.8/setup.cfg
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      623 2020-07-14 23:02:28.000000 plain_db-0.0.8/setup.py
+drwxr-xr-x   0 yunzhi   (672583) primarygroup (89939)        0 2020-07-15 00:49:52.000000 plain_db-0.0.9/
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      770 2020-07-15 00:49:52.000000 plain_db-0.0.9/PKG-INFO
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      208 2020-07-07 18:39:37.000000 plain_db-0.0.9/README.md
+drwxr-xr-x   0 yunzhi   (672583) primarygroup (89939)        0 2020-07-15 00:49:52.000000 plain_db-0.0.9/plain_db/
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)     2402 2020-07-15 00:49:46.000000 plain_db-0.0.9/plain_db/__init__.py
+drwxr-xr-x   0 yunzhi   (672583) primarygroup (89939)        0 2020-07-15 00:49:52.000000 plain_db-0.0.9/plain_db.egg-info/
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      770 2020-07-15 00:49:52.000000 plain_db-0.0.9/plain_db.egg-info/PKG-INFO
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      167 2020-07-15 00:49:52.000000 plain_db-0.0.9/plain_db.egg-info/SOURCES.txt
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)        1 2020-07-15 00:49:52.000000 plain_db-0.0.9/plain_db.egg-info/dependency_links.txt
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)        9 2020-07-15 00:49:52.000000 plain_db-0.0.9/plain_db.egg-info/top_level.txt
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)       38 2020-07-15 00:49:52.000000 plain_db-0.0.9/setup.cfg
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      623 2020-07-15 00:49:50.000000 plain_db-0.0.9/setup.py
```

### Comparing `plain_db-0.0.8/PKG-INFO` & `plain_db-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plain_db
-Version: 0.0.8
+Version: 0.0.9
 Summary: Plain txt DB
 Home-page: https://github.com/gaoyunzhi/plain_db
 Author: Yunzhi Gao
 Author-email: gaoyunzhi@gmail.com
 License: UNKNOWN
 Description: # plain_db
```

### Comparing `plain_db-0.0.8/plain_db/__init__.py` & `plain_db-0.0.9/plain_db/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -38,19 +38,19 @@
 		self.update(key, oldValue + value)
 
 	def get(self, key, default=None):
 		return self.items.get(key) or default
 
 	def appendSave(self, key, value):
 		if len(self.items) == 1:
-			prefix = ''
-		else:
-			prefix = '\n'
+			with open(self.fn, 'w') as f:
+				f.write(str(key) + ' ' + str(value))
+			return
 		with open(self.fn, 'a') as f:
-			f.write(prefix + str(key) + ' ' + str(value))
+			f.write('\n' + str(key) + ' ' + str(value))
 
 	def save(self):
 		lines = [key + ' ' + str(self.items[key]) for key in self.items]
 		lines.sort()
 		towrite = '\n'.join(lines)
 		if not towrite:
 			return
@@ -73,7 +73,36 @@
 		return True
 
 	def items(self):
 		return list(self._db.items.keys())
 
 def loadKeyOnlyDB(fn):
 	return NoValueDB(fn)
+
+class LargeDB(object):
+	def __init__(self, name):
+		self._db = DB(name, isIntValue=False)
+
+	def get(self, key, default):
+		return self._db.get(key, default)
+
+	def update(self, key, value):
+		if self._db.get(key) == value:
+			return
+		self._db.items[key] = value
+		self._db.appendSave(key, value)
+
+	def items(self):
+		return self._db.items.items()
+
+	def getFn(self):
+		return self._db.fn
+
+def loadLargeDB(fn):
+	return LargeDB(fn)
+
+def cleanupLargeDB(fn):
+	f1 = loadLargeDB(fn)
+	f2 = loadLargeDB(fn + 'tmp')
+	for key, value in f1.items():
+		f2.update(key, value)
+	os.system('mv %s %s' % (f2.getFn(), f1.getFn()))
```

### Comparing `plain_db-0.0.8/plain_db.egg-info/PKG-INFO` & `plain_db-0.0.9/plain_db.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plain-db
-Version: 0.0.8
+Version: 0.0.9
 Summary: Plain txt DB
 Home-page: https://github.com/gaoyunzhi/plain_db
 Author: Yunzhi Gao
 Author-email: gaoyunzhi@gmail.com
 License: UNKNOWN
 Description: # plain_db
```

### Comparing `plain_db-0.0.8/setup.py` & `plain_db-0.0.9/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="plain_db",
-    version="0.0.8",
+    version="0.0.9",
     author="Yunzhi Gao",
     author_email="gaoyunzhi@gmail.com",
     description="Plain txt DB",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/gaoyunzhi/plain_db",
     packages=setuptools.find_packages(),
```

