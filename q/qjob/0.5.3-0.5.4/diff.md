# Comparing `tmp/qjob-0.5.3.tar.gz` & `tmp/qjob-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qjob-0.5.3.tar", last modified: Tue Oct 18 13:09:23 2022, max compression
+gzip compressed data, was "qjob-0.5.4.tar", last modified: Mon May  8 10:24:41 2023, max compression
```

## Comparing `qjob-0.5.3.tar` & `qjob-0.5.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2022-10-18 13:09:23.332634 qjob-0.5.3/
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1071 2021-11-16 15:00:35.000000 qjob-0.5.3/LICENSE
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      673 2022-10-18 13:09:23.332634 qjob-0.5.3/PKG-INFO
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      154 2021-11-16 15:00:38.000000 qjob-0.5.3/README.md
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      104 2021-11-16 15:00:38.000000 qjob-0.5.3/pyproject.toml
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      825 2022-10-18 13:09:23.332634 qjob-0.5.3/setup.cfg
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       69 2021-11-16 15:00:35.000000 qjob-0.5.3/setup.py
-drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2022-10-18 13:09:23.332634 qjob-0.5.3/src/
-drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2022-10-18 13:09:23.332634 qjob-0.5.3/src/qjob/
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       68 2021-11-16 15:00:38.000000 qjob-0.5.3/src/qjob/__init__.py
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       20 2022-10-18 13:08:52.000000 qjob-0.5.3/src/qjob/_version.py
--rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)    25809 2022-10-18 13:06:56.000000 qjob-0.5.3/src/qjob/cli.py
-drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2022-10-18 13:09:23.332634 qjob-0.5.3/src/qjob.egg-info/
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      673 2022-10-18 13:09:23.000000 qjob-0.5.3/src/qjob.egg-info/PKG-INFO
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      268 2022-10-18 13:09:23.000000 qjob-0.5.3/src/qjob.egg-info/SOURCES.txt
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)        1 2022-10-18 13:09:23.000000 qjob-0.5.3/src/qjob.egg-info/dependency_links.txt
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       31 2022-10-18 13:09:23.000000 qjob-0.5.3/src/qjob.egg-info/requires.txt
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)        5 2022-10-18 13:09:23.000000 qjob-0.5.3/src/qjob.egg-info/top_level.txt
+drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-05-08 10:24:41.925853 qjob-0.5.4/
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1071 2021-11-16 15:00:35.000000 qjob-0.5.4/LICENSE
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      673 2023-05-08 10:24:41.925853 qjob-0.5.4/PKG-INFO
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      154 2021-11-16 15:00:38.000000 qjob-0.5.4/README.md
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      104 2021-11-16 15:00:38.000000 qjob-0.5.4/pyproject.toml
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      825 2023-05-08 10:24:41.925853 qjob-0.5.4/setup.cfg
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       69 2021-11-16 15:00:35.000000 qjob-0.5.4/setup.py
+drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-05-08 10:24:41.925853 qjob-0.5.4/src/
+drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-05-08 10:24:41.925853 qjob-0.5.4/src/qjob/
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       68 2021-11-16 15:00:38.000000 qjob-0.5.4/src/qjob/__init__.py
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       20 2023-05-08 10:23:12.000000 qjob-0.5.4/src/qjob/_version.py
+-rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)    25809 2022-10-18 13:06:56.000000 qjob-0.5.4/src/qjob/cli.py
+drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-05-08 10:24:41.925853 qjob-0.5.4/src/qjob.egg-info/
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      673 2023-05-08 10:24:41.000000 qjob-0.5.4/src/qjob.egg-info/PKG-INFO
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      268 2023-05-08 10:24:41.000000 qjob-0.5.4/src/qjob.egg-info/SOURCES.txt
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)        1 2023-05-08 10:24:41.000000 qjob-0.5.4/src/qjob.egg-info/dependency_links.txt
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       31 2023-05-08 10:24:41.000000 qjob-0.5.4/src/qjob.egg-info/requires.txt
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)        5 2023-05-08 10:24:41.000000 qjob-0.5.4/src/qjob.egg-info/top_level.txt
```

### Comparing `qjob-0.5.3/LICENSE` & `qjob-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `qjob-0.5.3/PKG-INFO` & `qjob-0.5.4/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: qjob
-Version: 0.5.3
+Version: 0.5.4
 Summary: Utility to split shell commands into jobs, then submit them for computation to a queue of a SGE or Slurm cluster.
 Home-page: https://github.com/marco-mariotti/qjob
 Author: Marco Mariotti
 Author-email: marco.mariotti@ub.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: <3.10,>=3.6
+Requires-Python: <3.11,>=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # qjob
 Utility to split shell commands into jobs, then submit them for computation to a queue of a SGE or Slurm cluster.
 
 See https://qjob.readthedocs.io/
```

### Comparing `qjob-0.5.3/setup.cfg` & `qjob-0.5.4/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 
 [options]
 package_dir = 
 	= src
 packages = find:
-python_requires = >=3.6,<3.10
+python_requires = >=3.6,<3.11
 install_requires = 
 	more-itertools
 	easyterm >=0.4.0
 
 [options.packages.find]
 where = src
```

### Comparing `qjob-0.5.3/src/qjob/cli.py` & `qjob-0.5.4/src/qjob/cli.py`

 * *Files identical despite different names*

### Comparing `qjob-0.5.3/src/qjob.egg-info/PKG-INFO` & `qjob-0.5.4/src/qjob.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: qjob
-Version: 0.5.3
+Version: 0.5.4
 Summary: Utility to split shell commands into jobs, then submit them for computation to a queue of a SGE or Slurm cluster.
 Home-page: https://github.com/marco-mariotti/qjob
 Author: Marco Mariotti
 Author-email: marco.mariotti@ub.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: <3.10,>=3.6
+Requires-Python: <3.11,>=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # qjob
 Utility to split shell commands into jobs, then submit them for computation to a queue of a SGE or Slurm cluster.
 
 See https://qjob.readthedocs.io/
```

