# Comparing `tmp/shub-workflow-1.9.7.3.tar.gz` & `tmp/shub-workflow-1.9.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shub-workflow-1.9.7.3.tar", last modified: Tue Oct 11 22:56:25 2022, max compression
+gzip compressed data, was "shub-workflow-1.9.7.4.tar", last modified: Wed Oct 12 19:43:12 2022, max compression
```

## Comparing `shub-workflow-1.9.7.3.tar` & `shub-workflow-1.9.7.4.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2022-10-11 22:56:25.071871 shub-workflow-1.9.7.3/
--rw-r--r--   0 molveyra  (1001) molveyra  (1001)     1478 2018-09-25 20:47:25.000000 shub-workflow-1.9.7.3/LICENSE
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      938 2022-10-11 22:56:25.071871 shub-workflow-1.9.7.3/PKG-INFO
--rw-r--r--   0 molveyra  (1001) molveyra  (1001)      314 2019-05-22 14:20:59.000000 shub-workflow-1.9.7.3/README.md
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       31 2021-06-08 13:16:58.000000 shub-workflow-1.9.7.3/pyproject.toml
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       38 2022-10-11 22:56:25.071871 shub-workflow-1.9.7.3/setup.cfg
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     1153 2022-10-11 22:55:45.000000 shub-workflow-1.9.7.3/setup.py
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2022-10-11 22:56:25.063872 shub-workflow-1.9.7.3/shub_workflow/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       24 2022-10-11 22:55:53.000000 shub-workflow-1.9.7.3/shub_workflow/__init__.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     8847 2022-10-11 22:44:54.000000 shub-workflow-1.9.7.3/shub_workflow/base.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     4985 2022-08-22 21:38:19.000000 shub-workflow-1.9.7.3/shub_workflow/clone_job.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     9113 2022-10-10 17:12:16.000000 shub-workflow-1.9.7.3/shub_workflow/crawl.py
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2022-10-11 22:56:25.067871 shub-workflow-1.9.7.3/shub_workflow/deliver/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       91 2022-09-22 15:04:57.000000 shub-workflow-1.9.7.3/shub_workflow/deliver/__init__.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     7359 2022-09-22 15:28:26.000000 shub-workflow-1.9.7.3/shub_workflow/deliver/base.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      871 2022-09-22 14:49:28.000000 shub-workflow-1.9.7.3/shub_workflow/deliver/dupefilter.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    13287 2022-10-10 15:58:53.000000 shub-workflow-1.9.7.3/shub_workflow/deliver/futils.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     1155 2022-07-04 16:12:44.000000 shub-workflow-1.9.7.3/shub_workflow/deliver/gcstorage.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     9759 2022-09-22 14:58:35.000000 shub-workflow-1.9.7.3/shub_workflow/deliver/legacy.py
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2022-10-11 22:56:25.067871 shub-workflow-1.9.7.3/shub_workflow/graph/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    17114 2022-10-10 16:53:10.000000 shub-workflow-1.9.7.3/shub_workflow/graph/__init__.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     9226 2022-07-04 16:12:44.000000 shub-workflow-1.9.7.3/shub_workflow/graph/task.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     1345 2022-07-04 16:12:44.000000 shub-workflow-1.9.7.3/shub_workflow/graph/utils.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    10234 2022-10-11 22:54:14.000000 shub-workflow-1.9.7.3/shub_workflow/script.py
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2022-10-11 22:56:25.067871 shub-workflow-1.9.7.3/shub_workflow/utils/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     2882 2022-10-11 14:54:56.000000 shub-workflow-1.9.7.3/shub_workflow/utils/__init__.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3472 2022-07-04 16:12:44.000000 shub-workflow-1.9.7.3/shub_workflow/utils/sesemail.py
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2022-10-11 22:56:25.063872 shub-workflow-1.9.7.3/shub_workflow.egg-info/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      938 2022-10-11 22:56:24.000000 shub-workflow-1.9.7.3/shub_workflow.egg-info/PKG-INFO
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      848 2022-10-11 22:56:24.000000 shub-workflow-1.9.7.3/shub_workflow.egg-info/SOURCES.txt
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        1 2022-10-11 22:56:24.000000 shub-workflow-1.9.7.3/shub_workflow.egg-info/dependency_links.txt
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      183 2022-10-11 22:56:24.000000 shub-workflow-1.9.7.3/shub_workflow.egg-info/requires.txt
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       20 2022-10-11 22:56:24.000000 shub-workflow-1.9.7.3/shub_workflow.egg-info/top_level.txt
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2022-10-11 22:56:25.067871 shub-workflow-1.9.7.3/tests/
--rw-r--r--   0 molveyra  (1001) molveyra  (1001)        0 2018-09-25 20:47:25.000000 shub-workflow-1.9.7.3/tests/__init__.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     1353 2022-09-16 20:02:43.000000 shub-workflow-1.9.7.3/tests/test_base_manager.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    20202 2022-10-10 17:28:58.000000 shub-workflow-1.9.7.3/tests/test_crawl_manager.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    74092 2022-08-23 21:36:35.000000 shub-workflow-1.9.7.3/tests/test_graph_manager.py
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2022-10-11 22:56:25.071871 shub-workflow-1.9.7.3/tests/utils/
--rw-r--r--   0 molveyra  (1001) molveyra  (1001)        0 2018-09-25 20:47:25.000000 shub-workflow-1.9.7.3/tests/utils/__init__.py
--rw-r--r--   0 molveyra  (1001) molveyra  (1001)      288 2018-09-25 20:47:25.000000 shub-workflow-1.9.7.3/tests/utils/contexts.py
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2022-10-12 19:43:12.001403 shub-workflow-1.9.7.4/
+-rw-r--r--   0 molveyra  (1001) molveyra  (1001)     1478 2018-09-25 20:47:25.000000 shub-workflow-1.9.7.4/LICENSE
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      938 2022-10-12 19:43:12.001403 shub-workflow-1.9.7.4/PKG-INFO
+-rw-r--r--   0 molveyra  (1001) molveyra  (1001)      314 2019-05-22 14:20:59.000000 shub-workflow-1.9.7.4/README.md
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       31 2021-06-08 13:16:58.000000 shub-workflow-1.9.7.4/pyproject.toml
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       38 2022-10-12 19:43:12.001403 shub-workflow-1.9.7.4/setup.cfg
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     1146 2022-10-12 19:37:24.000000 shub-workflow-1.9.7.4/setup.py
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2022-10-12 19:43:11.993404 shub-workflow-1.9.7.4/shub_workflow/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       24 2022-10-12 19:37:24.000000 shub-workflow-1.9.7.4/shub_workflow/__init__.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     8847 2022-10-11 22:44:54.000000 shub-workflow-1.9.7.4/shub_workflow/base.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     4985 2022-08-22 21:38:19.000000 shub-workflow-1.9.7.4/shub_workflow/clone_job.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     9113 2022-10-10 17:12:16.000000 shub-workflow-1.9.7.4/shub_workflow/crawl.py
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2022-10-12 19:43:11.997404 shub-workflow-1.9.7.4/shub_workflow/deliver/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       91 2022-09-22 15:04:57.000000 shub-workflow-1.9.7.4/shub_workflow/deliver/__init__.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     7359 2022-09-22 15:28:26.000000 shub-workflow-1.9.7.4/shub_workflow/deliver/base.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      871 2022-09-22 14:49:28.000000 shub-workflow-1.9.7.4/shub_workflow/deliver/dupefilter.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    13149 2022-10-12 11:51:29.000000 shub-workflow-1.9.7.4/shub_workflow/deliver/futils.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     1155 2022-07-04 16:12:44.000000 shub-workflow-1.9.7.4/shub_workflow/deliver/gcstorage.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     9759 2022-09-22 14:58:35.000000 shub-workflow-1.9.7.4/shub_workflow/deliver/legacy.py
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2022-10-12 19:43:12.001403 shub-workflow-1.9.7.4/shub_workflow/graph/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    17114 2022-10-10 16:53:10.000000 shub-workflow-1.9.7.4/shub_workflow/graph/__init__.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     9226 2022-07-04 16:12:44.000000 shub-workflow-1.9.7.4/shub_workflow/graph/task.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     1345 2022-07-04 16:12:44.000000 shub-workflow-1.9.7.4/shub_workflow/graph/utils.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    10234 2022-10-11 22:54:14.000000 shub-workflow-1.9.7.4/shub_workflow/script.py
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2022-10-12 19:43:12.001403 shub-workflow-1.9.7.4/shub_workflow/utils/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     2664 2022-10-12 19:25:31.000000 shub-workflow-1.9.7.4/shub_workflow/utils/__init__.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3472 2022-07-04 16:12:44.000000 shub-workflow-1.9.7.4/shub_workflow/utils/sesemail.py
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2022-10-12 19:43:11.997404 shub-workflow-1.9.7.4/shub_workflow.egg-info/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      938 2022-10-12 19:43:11.000000 shub-workflow-1.9.7.4/shub_workflow.egg-info/PKG-INFO
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      848 2022-10-12 19:43:11.000000 shub-workflow-1.9.7.4/shub_workflow.egg-info/SOURCES.txt
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        1 2022-10-12 19:43:11.000000 shub-workflow-1.9.7.4/shub_workflow.egg-info/dependency_links.txt
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      176 2022-10-12 19:43:11.000000 shub-workflow-1.9.7.4/shub_workflow.egg-info/requires.txt
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       20 2022-10-12 19:43:11.000000 shub-workflow-1.9.7.4/shub_workflow.egg-info/top_level.txt
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2022-10-12 19:43:12.001403 shub-workflow-1.9.7.4/tests/
+-rw-r--r--   0 molveyra  (1001) molveyra  (1001)        0 2018-09-25 20:47:25.000000 shub-workflow-1.9.7.4/tests/__init__.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     1353 2022-09-16 20:02:43.000000 shub-workflow-1.9.7.4/tests/test_base_manager.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    20202 2022-10-10 17:28:58.000000 shub-workflow-1.9.7.4/tests/test_crawl_manager.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    74092 2022-08-23 21:36:35.000000 shub-workflow-1.9.7.4/tests/test_graph_manager.py
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2022-10-12 19:43:12.001403 shub-workflow-1.9.7.4/tests/utils/
+-rw-r--r--   0 molveyra  (1001) molveyra  (1001)        0 2018-09-25 20:47:25.000000 shub-workflow-1.9.7.4/tests/utils/__init__.py
+-rw-r--r--   0 molveyra  (1001) molveyra  (1001)      288 2018-09-25 20:47:25.000000 shub-workflow-1.9.7.4/tests/utils/contexts.py
```

### Comparing `shub-workflow-1.9.7.3/LICENSE` & `shub-workflow-1.9.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `shub-workflow-1.9.7.3/PKG-INFO` & `shub-workflow-1.9.7.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shub-workflow
-Version: 1.9.7.3
+Version: 1.9.7.4
 Summary: Workflow manager for scrapinghub ScrapyCloud tasks.
 Home-page: https://github.com/scrapinghub/shub-workflow
 Maintainer: Scrapinghub
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `shub-workflow-1.9.7.3/setup.py` & `shub-workflow-1.9.7.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 # Automatically created by: shub deploy
 
 from setuptools import setup, find_packages
 
 setup(
     name="shub-workflow",
-    version="1.9.7.3",
+    version="1.9.7.4",
     description="Workflow manager for scrapinghub ScrapyCloud tasks.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     license="BSD",
     url="https://github.com/scrapinghub/shub-workflow",
     maintainer="Scrapinghub",
     packages=find_packages(),
     install_requires=(
         "pyyaml>=3.12",
-        "retrying>=1.3.3",
         "scrapinghub[msgpack]>=2.3.1",
         "jinja2>=2.7.3",
         "sqlitedict==1.6.0",
         "s3fs>=0.4.0",
         "boto3>=1.9.92",
         "google-cloud-storage>=1.38.0",
         "bloom-filter==1.3.3",
         "collection-scanner",
+        "tenacity",
     ),
     scripts=[],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: BSD License",
         "Operating System :: OS Independent",
```

### Comparing `shub-workflow-1.9.7.3/shub_workflow/base.py` & `shub-workflow-1.9.7.4/shub_workflow/base.py`

 * *Files identical despite different names*

### Comparing `shub-workflow-1.9.7.3/shub_workflow/clone_job.py` & `shub-workflow-1.9.7.4/shub_workflow/clone_job.py`

 * *Files identical despite different names*

### Comparing `shub-workflow-1.9.7.3/shub_workflow/crawl.py` & `shub-workflow-1.9.7.4/shub_workflow/crawl.py`

 * *Files identical despite different names*

### Comparing `shub-workflow-1.9.7.3/shub_workflow/deliver/base.py` & `shub-workflow-1.9.7.4/shub_workflow/deliver/base.py`

 * *Files identical despite different names*

### Comparing `shub-workflow-1.9.7.3/shub_workflow/deliver/dupefilter.py` & `shub-workflow-1.9.7.4/shub_workflow/deliver/dupefilter.py`

 * *Files identical despite different names*

### Comparing `shub-workflow-1.9.7.3/shub_workflow/deliver/futils.py` & `shub-workflow-1.9.7.4/shub_workflow/deliver/futils.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from operator import itemgetter
 from glob import iglob
 from os import listdir, remove, environ, makedirs
 from os.path import exists as os_exists, dirname, getctime, basename
 from shutil import copyfile
 from datetime import datetime, timedelta, timezone
 
-from retrying import retry
 from s3fs import S3FileSystem as OriginalS3FileSystem
 import boto3
 
 from shub_workflow.deliver import gcstorage
 
 S3_PATH_RE = re.compile("s3://(.+?)/(.+)")
 _S3_ATTRIBUTE = "s3://"
@@ -30,17 +29,14 @@
     logger.error(str(exception))
     for etype in (KeyboardInterrupt, SystemExit, ImportError):
         if isinstance(exception, etype):
             return False
     return True  # retries any other exception
 
 
-retry_decorator = retry(retry_on_exception=just_log_exception, wait_fixed=60000, stop_max_attempt_number=10)
-
-
 class S3FileSystem(OriginalS3FileSystem):
     read_timeout = 120
     connect_timeout = 60
 
 
 def s3_path(path, is_folder=False):
     if not path:
```

### Comparing `shub-workflow-1.9.7.3/shub_workflow/deliver/gcstorage.py` & `shub-workflow-1.9.7.4/shub_workflow/deliver/gcstorage.py`

 * *Files identical despite different names*

### Comparing `shub-workflow-1.9.7.3/shub_workflow/deliver/legacy.py` & `shub-workflow-1.9.7.4/shub_workflow/deliver/legacy.py`

 * *Files identical despite different names*

### Comparing `shub-workflow-1.9.7.3/shub_workflow/graph/__init__.py` & `shub-workflow-1.9.7.4/shub_workflow/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `shub-workflow-1.9.7.3/shub_workflow/graph/task.py` & `shub-workflow-1.9.7.4/shub_workflow/graph/task.py`

 * *Files identical despite different names*

### Comparing `shub-workflow-1.9.7.3/shub_workflow/graph/utils.py` & `shub-workflow-1.9.7.4/shub_workflow/graph/utils.py`

 * *Files identical despite different names*

### Comparing `shub-workflow-1.9.7.3/shub_workflow/script.py` & `shub-workflow-1.9.7.4/shub_workflow/script.py`

 * *Files identical despite different names*

### Comparing `shub-workflow-1.9.7.3/shub_workflow/utils/__init__.py` & `shub-workflow-1.9.7.4/shub_workflow/utils/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import logging
 import json
 import os
 import hashlib
 from typing import Optional
-from traceback import format_tb
 
-from retrying import retry
+from tenacity import retry, retry_if_exception_type, before_sleep_log, stop_after_attempt, wait_fixed
 from scrapinghub.client.exceptions import ServerError
 from requests.exceptions import ReadTimeout, ConnectionError, HTTPError
 
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.INFO)
 
@@ -59,26 +58,20 @@
     return None
 
 
 MINS_IN_A_DAY = 24 * 60
 ONE_MIN_IN_S = 60
 
 
-def just_log_exception(exception):
-    logger.error("".join(format_tb(exception.__traceback__)[1:]))
-    logger.error(repr(exception))
-    if isinstance(exception, (ServerError, ReadTimeout, ConnectionError, HTTPError)):
-        logger.info("Waiting %d seconds", ONE_MIN_IN_S)
-        return True
-    logger.error(f"Exception of type {type(exception)} will not be retried.")
-    return False
-
-
 dash_retry_decorator = retry(
-    retry_on_exception=just_log_exception, wait_fixed=ONE_MIN_IN_S * 1000, stop_max_attempt_number=MINS_IN_A_DAY
+    retry=retry_if_exception_type((ServerError, ReadTimeout, ConnectionError, HTTPError)),
+    before_sleep=before_sleep_log(logger, logging.ERROR),
+    reraise=True,
+    stop=stop_after_attempt(MINS_IN_A_DAY),
+    wait=wait_fixed(ONE_MIN_IN_S),
 )
 
 
 def kumo_settings():
     settings = {}
     shub_job_data = json.loads(os.environ.get("SHUB_SETTINGS", "{}"))
     if shub_job_data:
```

### Comparing `shub-workflow-1.9.7.3/shub_workflow/utils/sesemail.py` & `shub-workflow-1.9.7.4/shub_workflow/utils/sesemail.py`

 * *Files identical despite different names*

### Comparing `shub-workflow-1.9.7.3/shub_workflow.egg-info/PKG-INFO` & `shub-workflow-1.9.7.4/shub_workflow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shub-workflow
-Version: 1.9.7.3
+Version: 1.9.7.4
 Summary: Workflow manager for scrapinghub ScrapyCloud tasks.
 Home-page: https://github.com/scrapinghub/shub-workflow
 Maintainer: Scrapinghub
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `shub-workflow-1.9.7.3/shub_workflow.egg-info/SOURCES.txt` & `shub-workflow-1.9.7.4/shub_workflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `shub-workflow-1.9.7.3/tests/test_base_manager.py` & `shub-workflow-1.9.7.4/tests/test_base_manager.py`

 * *Files identical despite different names*

### Comparing `shub-workflow-1.9.7.3/tests/test_crawl_manager.py` & `shub-workflow-1.9.7.4/tests/test_crawl_manager.py`

 * *Files identical despite different names*

### Comparing `shub-workflow-1.9.7.3/tests/test_graph_manager.py` & `shub-workflow-1.9.7.4/tests/test_graph_manager.py`

 * *Files identical despite different names*

