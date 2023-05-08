# Comparing `tmp/pyfirebird-0.0.8.tar.gz` & `tmp/pyfirebird-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfirebird-0.0.8.tar", last modified: Sun Apr 30 08:49:43 2023, max compression
+gzip compressed data, was "pyfirebird-0.0.9.tar", last modified: Fri May  5 02:59:29 2023, max compression
```

## Comparing `pyfirebird-0.0.8.tar` & `pyfirebird-0.0.9.tar`

### file list

```diff
@@ -1,23 +1,26 @@
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-04-30 08:49:43.158793 pyfirebird-0.0.8/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      367 2023-04-30 08:49:43.158793 pyfirebird-0.0.8/PKG-INFO
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        8 2023-04-30 05:34:25.000000 pyfirebird-0.0.8/README.md
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       38 2023-04-30 08:49:43.158793 pyfirebird-0.0.8/setup.cfg
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     1051 2023-04-30 08:49:40.000000 pyfirebird-0.0.8/setup.py
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-04-30 08:49:43.154793 pyfirebird-0.0.8/src/
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-04-30 08:49:43.154793 pyfirebird-0.0.8/src/firebird/
--rw-r--r--   0 stonezhong  (1000) stonezhong  (1000)      169 2023-04-30 06:39:02.000000 pyfirebird-0.0.8/src/firebird/__init__.py
--rw-r--r--   0 stonezhong  (1000) stonezhong  (1000)    10042 2023-04-30 05:32:50.000000 pyfirebird-0.0.8/src/firebird/base.py
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-04-30 08:49:43.154793 pyfirebird-0.0.8/src/firebird/cmd_tools/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        0 2023-04-30 05:45:15.000000 pyfirebird-0.0.8/src/firebird/cmd_tools/__init__.py
--rw-r--r--   0 stonezhong  (1000) stonezhong  (1000)     7298 2023-04-30 08:21:26.000000 pyfirebird-0.0.8/src/firebird/cmd_tools/executor.py
--rw-r--r--   0 stonezhong  (1000) stonezhong  (1000)     2980 2023-04-30 07:22:18.000000 pyfirebird-0.0.8/src/firebird/cmd_tools/pipeline.py
--rw-r--r--   0 stonezhong  (1000) stonezhong  (1000)     2478 2023-04-30 08:48:29.000000 pyfirebird-0.0.8/src/firebird/cmd_tools/pipeline_impl.py
--rw-r--r--   0 stonezhong  (1000) stonezhong  (1000)     2972 2023-04-30 05:32:50.000000 pyfirebird-0.0.8/src/firebird/rabbitmq.py
--rw-r--r--   0 stonezhong  (1000) stonezhong  (1000)     5714 2023-04-30 07:37:36.000000 pyfirebird-0.0.8/src/firebird/zkdb.py
-drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-04-30 08:49:43.158793 pyfirebird-0.0.8/src/pyfirebird.egg-info/
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      367 2023-04-30 08:49:43.000000 pyfirebird-0.0.8/src/pyfirebird.egg-info/PKG-INFO
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      485 2023-04-30 08:49:43.000000 pyfirebird-0.0.8/src/pyfirebird.egg-info/SOURCES.txt
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        1 2023-04-30 08:49:43.000000 pyfirebird-0.0.8/src/pyfirebird.egg-info/dependency_links.txt
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      106 2023-04-30 08:49:43.000000 pyfirebird-0.0.8/src/pyfirebird.egg-info/entry_points.txt
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       27 2023-04-30 08:49:43.000000 pyfirebird-0.0.8/src/pyfirebird.egg-info/requires.txt
--rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        9 2023-04-30 08:49:43.000000 pyfirebird-0.0.8/src/pyfirebird.egg-info/top_level.txt
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-05-05 02:59:29.387201 pyfirebird-0.0.9/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      367 2023-05-05 02:59:29.387201 pyfirebird-0.0.9/PKG-INFO
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        8 2023-04-30 05:34:25.000000 pyfirebird-0.0.9/README.md
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       38 2023-05-05 02:59:29.387201 pyfirebird-0.0.9/setup.cfg
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     1051 2023-05-05 02:58:37.000000 pyfirebird-0.0.9/setup.py
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-05-05 02:59:29.383201 pyfirebird-0.0.9/src/
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-05-05 02:59:29.387201 pyfirebird-0.0.9/src/firebird/
+-rw-r--r--   0 stonezhong  (1000) stonezhong  (1000)      169 2023-04-30 06:39:02.000000 pyfirebird-0.0.9/src/firebird/__init__.py
+-rw-r--r--   0 stonezhong  (1000) stonezhong  (1000)    10042 2023-04-30 05:32:50.000000 pyfirebird-0.0.9/src/firebird/base.py
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-05-05 02:59:29.387201 pyfirebird-0.0.9/src/firebird/cmd_tools/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        0 2023-04-30 05:45:15.000000 pyfirebird-0.0.9/src/firebird/cmd_tools/__init__.py
+-rw-r--r--   0 stonezhong  (1000) stonezhong  (1000)     7298 2023-04-30 08:21:26.000000 pyfirebird-0.0.9/src/firebird/cmd_tools/executor.py
+-rw-r--r--   0 stonezhong  (1000) stonezhong  (1000)     2980 2023-04-30 07:22:18.000000 pyfirebird-0.0.9/src/firebird/cmd_tools/pipeline.py
+-rw-r--r--   0 stonezhong  (1000) stonezhong  (1000)     2478 2023-04-30 08:48:29.000000 pyfirebird-0.0.9/src/firebird/cmd_tools/pipeline_impl.py
+-rw-r--r--   0 stonezhong  (1000) stonezhong  (1000)     2972 2023-04-30 05:32:50.000000 pyfirebird-0.0.9/src/firebird/rabbitmq.py
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-05-05 02:59:29.387201 pyfirebird-0.0.9/src/firebird/utils/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       60 2023-05-05 02:58:25.000000 pyfirebird-0.0.9/src/firebird/utils/__init__.py
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)     4359 2023-05-05 02:56:50.000000 pyfirebird-0.0.9/src/firebird/utils/checkpoint.py
+-rw-r--r--   0 stonezhong  (1000) stonezhong  (1000)     5714 2023-04-30 07:37:36.000000 pyfirebird-0.0.9/src/firebird/zkdb.py
+drwxrwxr-x   0 stonezhong  (1000) stonezhong  (1000)        0 2023-05-05 02:59:29.387201 pyfirebird-0.0.9/src/pyfirebird.egg-info/
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      367 2023-05-05 02:59:29.000000 pyfirebird-0.0.9/src/pyfirebird.egg-info/PKG-INFO
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      549 2023-05-05 02:59:29.000000 pyfirebird-0.0.9/src/pyfirebird.egg-info/SOURCES.txt
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        1 2023-05-05 02:59:29.000000 pyfirebird-0.0.9/src/pyfirebird.egg-info/dependency_links.txt
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)      106 2023-05-05 02:59:29.000000 pyfirebird-0.0.9/src/pyfirebird.egg-info/entry_points.txt
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)       27 2023-05-05 02:59:29.000000 pyfirebird-0.0.9/src/pyfirebird.egg-info/requires.txt
+-rw-rw-r--   0 stonezhong  (1000) stonezhong  (1000)        9 2023-05-05 02:59:29.000000 pyfirebird-0.0.9/src/pyfirebird.egg-info/top_level.txt
```

### Comparing `pyfirebird-0.0.8/setup.py` & `pyfirebird-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # The text of the README file
 with open(os.path.join(HERE, "README.md"), "r") as f:
     README = f.read()
 
 # This call to setup() does all the work
 setup(
     name="pyfirebird",
-    version="0.0.8",
+    version="0.0.9",
     description="Streaming Data Processing Framework",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/stonezhong/firebird",
     author="Stone Zhong",
     author_email="stonezhong@hotmail.com",
     license="MIT",
```

### Comparing `pyfirebird-0.0.8/src/firebird/base.py` & `pyfirebird-0.0.9/src/firebird/base.py`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.8/src/firebird/cmd_tools/executor.py` & `pyfirebird-0.0.9/src/firebird/cmd_tools/executor.py`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.8/src/firebird/cmd_tools/pipeline.py` & `pyfirebird-0.0.9/src/firebird/cmd_tools/pipeline.py`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.8/src/firebird/cmd_tools/pipeline_impl.py` & `pyfirebird-0.0.9/src/firebird/cmd_tools/pipeline_impl.py`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.8/src/firebird/rabbitmq.py` & `pyfirebird-0.0.9/src/firebird/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `pyfirebird-0.0.8/src/firebird/zkdb.py` & `pyfirebird-0.0.9/src/firebird/zkdb.py`

 * *Files identical despite different names*

