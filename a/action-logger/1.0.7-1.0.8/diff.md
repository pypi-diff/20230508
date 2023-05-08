# Comparing `tmp/action_logger-1.0.7.tar.gz` & `tmp/action_logger-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "action_logger-1.0.7.tar", last modified: Mon Oct 24 07:29:27 2022, max compression
+gzip compressed data, was "action_logger-1.0.8.tar", last modified: Tue Oct 25 07:36:22 2022, max compression
```

## Comparing `action_logger-1.0.7.tar` & `action_logger-1.0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 danyanliu (1506875890) TESLAMOTORS\Domain Users (334330370)        0 2022-10-24 07:29:27.180534 action_logger-1.0.7/
--rw-r--r--   0 danyanliu (1506875890) TESLAMOTORS\Domain Users (334330370)     1078 2021-10-28 11:22:29.000000 action_logger-1.0.7/LICENSE
--rw-r--r--   0 danyanliu (1506875890) TESLAMOTORS\Domain Users (334330370)     1904 2022-10-24 07:29:27.180279 action_logger-1.0.7/PKG-INFO
--rw-r--r--   0 danyanliu (1506875890) TESLAMOTORS\Domain Users (334330370)     1479 2022-03-25 01:56:07.000000 action_logger-1.0.7/README.md
-drwxr-xr-x   0 danyanliu (1506875890) TESLAMOTORS\Domain Users (334330370)        0 2022-10-24 07:29:27.178010 action_logger-1.0.7/action_logger/
--rw-r--r--   0 danyanliu (1506875890) TESLAMOTORS\Domain Users (334330370)        0 2021-10-28 11:20:09.000000 action_logger-1.0.7/action_logger/__init__.py
--rw-r--r--   0 danyanliu (1506875890) TESLAMOTORS\Domain Users (334330370)     5163 2022-10-24 07:25:26.000000 action_logger-1.0.7/action_logger/client.py
-drwxr-xr-x   0 danyanliu (1506875890) TESLAMOTORS\Domain Users (334330370)        0 2022-10-24 07:29:27.179895 action_logger-1.0.7/action_logger.egg-info/
--rw-r--r--   0 danyanliu (1506875890) TESLAMOTORS\Domain Users (334330370)     1904 2022-10-24 07:29:26.000000 action_logger-1.0.7/action_logger.egg-info/PKG-INFO
--rw-r--r--   0 danyanliu (1506875890) TESLAMOTORS\Domain Users (334330370)      260 2022-10-24 07:29:27.000000 action_logger-1.0.7/action_logger.egg-info/SOURCES.txt
--rw-r--r--   0 danyanliu (1506875890) TESLAMOTORS\Domain Users (334330370)        1 2022-10-24 07:29:26.000000 action_logger-1.0.7/action_logger.egg-info/dependency_links.txt
--rw-r--r--   0 danyanliu (1506875890) TESLAMOTORS\Domain Users (334330370)       45 2022-10-24 07:29:26.000000 action_logger-1.0.7/action_logger.egg-info/requires.txt
--rw-r--r--   0 danyanliu (1506875890) TESLAMOTORS\Domain Users (334330370)       14 2022-10-24 07:29:26.000000 action_logger-1.0.7/action_logger.egg-info/top_level.txt
--rw-r--r--   0 danyanliu (1506875890) TESLAMOTORS\Domain Users (334330370)       38 2022-10-24 07:29:27.180630 action_logger-1.0.7/setup.cfg
--rw-r--r--   0 danyanliu (1506875890) TESLAMOTORS\Domain Users (334330370)     1030 2022-10-24 07:25:26.000000 action_logger-1.0.7/setup.py
+drwxr-xr-x   0 danyanliu (1506875890) TESLAMOTORS\Domain Users (334330370)        0 2022-10-25 07:36:22.038971 action_logger-1.0.8/
+-rw-r--r--   0 danyanliu (1506875890) TESLAMOTORS\Domain Users (334330370)     1078 2021-10-28 11:22:29.000000 action_logger-1.0.8/LICENSE
+-rw-r--r--   0 danyanliu (1506875890) TESLAMOTORS\Domain Users (334330370)     1904 2022-10-25 07:36:22.038694 action_logger-1.0.8/PKG-INFO
+-rw-r--r--   0 danyanliu (1506875890) TESLAMOTORS\Domain Users (334330370)     1479 2022-03-25 01:56:07.000000 action_logger-1.0.8/README.md
+drwxr-xr-x   0 danyanliu (1506875890) TESLAMOTORS\Domain Users (334330370)        0 2022-10-25 07:36:22.036548 action_logger-1.0.8/action_logger/
+-rw-r--r--   0 danyanliu (1506875890) TESLAMOTORS\Domain Users (334330370)        0 2021-10-28 11:20:09.000000 action_logger-1.0.8/action_logger/__init__.py
+-rw-r--r--   0 danyanliu (1506875890) TESLAMOTORS\Domain Users (334330370)     5163 2022-10-24 07:25:26.000000 action_logger-1.0.8/action_logger/client.py
+drwxr-xr-x   0 danyanliu (1506875890) TESLAMOTORS\Domain Users (334330370)        0 2022-10-25 07:36:22.038281 action_logger-1.0.8/action_logger.egg-info/
+-rw-r--r--   0 danyanliu (1506875890) TESLAMOTORS\Domain Users (334330370)     1904 2022-10-25 07:36:21.000000 action_logger-1.0.8/action_logger.egg-info/PKG-INFO
+-rw-r--r--   0 danyanliu (1506875890) TESLAMOTORS\Domain Users (334330370)      260 2022-10-25 07:36:21.000000 action_logger-1.0.8/action_logger.egg-info/SOURCES.txt
+-rw-r--r--   0 danyanliu (1506875890) TESLAMOTORS\Domain Users (334330370)        1 2022-10-25 07:36:21.000000 action_logger-1.0.8/action_logger.egg-info/dependency_links.txt
+-rw-r--r--   0 danyanliu (1506875890) TESLAMOTORS\Domain Users (334330370)       45 2022-10-25 07:36:21.000000 action_logger-1.0.8/action_logger.egg-info/requires.txt
+-rw-r--r--   0 danyanliu (1506875890) TESLAMOTORS\Domain Users (334330370)       14 2022-10-25 07:36:21.000000 action_logger-1.0.8/action_logger.egg-info/top_level.txt
+-rw-r--r--   0 danyanliu (1506875890) TESLAMOTORS\Domain Users (334330370)       38 2022-10-25 07:36:22.039079 action_logger-1.0.8/setup.cfg
+-rw-r--r--   0 danyanliu (1506875890) TESLAMOTORS\Domain Users (334330370)     1030 2022-10-25 07:35:31.000000 action_logger-1.0.8/setup.py
```

### Comparing `action_logger-1.0.7/LICENSE` & `action_logger-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `action_logger-1.0.7/PKG-INFO` & `action_logger-1.0.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: action_logger
-Version: 1.0.7
+Version: 1.0.8
 Summary: Action logger for digital transformer
 Author: TimeAshore
 Author-email: timeashore@163.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `action_logger-1.0.7/README.md` & `action_logger-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `action_logger-1.0.7/action_logger/client.py` & `action_logger-1.0.8/action_logger/client.py`

 * *Files identical despite different names*

### Comparing `action_logger-1.0.7/action_logger.egg-info/PKG-INFO` & `action_logger-1.0.8/action_logger.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: action-logger
-Version: 1.0.7
+Version: 1.0.8
 Summary: Action logger for digital transformer
 Author: TimeAshore
 Author-email: timeashore@163.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `action_logger-1.0.7/setup.py` & `action_logger-1.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     desc = f.read()
 
 # Arguments marked as "Required" below must be included for upload to PyPI.
 # Fields marked as "Optional" may be commented out.
 
 setup(
     name='action_logger',
-    version='1.0.7',
+    version='1.0.8',
     author='TimeAshore',
     author_email='timeashore@163.com',
     description='Action logger for digital transformer',
     long_description=desc,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     classifiers=[
```

