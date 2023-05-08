# Comparing `tmp/bbm-0.0.5.tar.gz` & `tmp/bbm-0.0.6.tar.gz`

## Comparing `bbm-0.0.5.tar` & `bbm-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 bbm-0.0.5/.github/workflows/code_formatter.yml
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 bbm-0.0.5/.github/workflows/python-versions-test.yml
--rw-r--r--   0        0        0     4322 2020-02-02 00:00:00.000000 bbm-0.0.5/bbm/__init__.py
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 bbm-0.0.5/bbm/constants.py
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 bbm-0.0.5/bbm/exceptions.py
--rw-r--r--   0        0        0     3832 2020-02-02 00:00:00.000000 bbm-0.0.5/bbm/reporter.py
--rw-r--r--   0        0        0    12888 2020-02-02 00:00:00.000000 bbm-0.0.5/bbm/utils.py
--rw-r--r--   0        0        0   249035 2020-02-02 00:00:00.000000 bbm-0.0.5/doc/images/example1.png
--rw-r--r--   0        0        0  1154595 2020-02-02 00:00:00.000000 bbm-0.0.5/doc/images/example2.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bbm-0.0.5/tests/__init__.py
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 bbm-0.0.5/tests/conftest.py
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 bbm-0.0.5/tests/test_bbm.py
--rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 bbm-0.0.5/tests/test_data/es_search_scroll_response.json
--rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 bbm-0.0.5/.gitignore
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 bbm-0.0.5/LICENSE
--rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 bbm-0.0.5/README.md
--rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 bbm-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     2973 2020-02-02 00:00:00.000000 bbm-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 bbm-0.0.6/.github/workflows/code_formatter.yml
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 bbm-0.0.6/.github/workflows/python-versions-test.yml
+-rw-r--r--   0        0        0     4346 2020-02-02 00:00:00.000000 bbm-0.0.6/bbm/__init__.py
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 bbm-0.0.6/bbm/constants.py
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 bbm-0.0.6/bbm/exceptions.py
+-rw-r--r--   0        0        0     3832 2020-02-02 00:00:00.000000 bbm-0.0.6/bbm/reporter.py
+-rw-r--r--   0        0        0    12888 2020-02-02 00:00:00.000000 bbm-0.0.6/bbm/utils.py
+-rw-r--r--   0        0        0   249035 2020-02-02 00:00:00.000000 bbm-0.0.6/doc/images/example1.png
+-rw-r--r--   0        0        0  1154595 2020-02-02 00:00:00.000000 bbm-0.0.6/doc/images/example2.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bbm-0.0.6/tests/__init__.py
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 bbm-0.0.6/tests/conftest.py
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 bbm-0.0.6/tests/test_bbm.py
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 bbm-0.0.6/tests/test_data/es_search_scroll_response.json
+-rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 bbm-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 bbm-0.0.6/LICENSE
+-rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 bbm-0.0.6/README.md
+-rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 bbm-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     2973 2020-02-02 00:00:00.000000 bbm-0.0.6/PKG-INFO
```

### Comparing `bbm-0.0.5/.github/workflows/code_formatter.yml` & `bbm-0.0.6/.github/workflows/code_formatter.yml`

 * *Files identical despite different names*

### Comparing `bbm-0.0.5/bbm/__init__.py` & `bbm-0.0.6/bbm/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import requests
 
 from bbm.constants import KST, Interval
 from bbm.exceptions import BBMNotInitialized, NoJoinChannelException, ReporterNotInitialized
 from bbm.utils import create_report, get_caller_file_name, get_hostname, get_ip
 
 # package info
-__version__ = "0.0.5"
+__version__ = "0.0.6"
 
 
 class BBM:
     def __init__(
         self,
         es_url: str,
         process_category: str = "fission-tasks",
@@ -128,12 +128,13 @@
                         "msg": "fail",
                         "cate": process_category,
                         "process_uuid": process_uuid,
                         "duration": duration,
                         "error_traceback": error_traceback,
                     },
                 )
+                raise e
             return result
 
         return decorator
 
     return wrapper
```

### Comparing `bbm-0.0.5/bbm/constants.py` & `bbm-0.0.6/bbm/constants.py`

 * *Files identical despite different names*

### Comparing `bbm-0.0.5/bbm/reporter.py` & `bbm-0.0.6/bbm/reporter.py`

 * *Files identical despite different names*

### Comparing `bbm-0.0.5/bbm/utils.py` & `bbm-0.0.6/bbm/utils.py`

 * *Files identical despite different names*

### Comparing `bbm-0.0.5/doc/images/example1.png` & `bbm-0.0.6/doc/images/example1.png`

 * *Files identical despite different names*

### Comparing `bbm-0.0.5/doc/images/example2.png` & `bbm-0.0.6/doc/images/example2.png`

 * *Files identical despite different names*

### Comparing `bbm-0.0.5/tests/conftest.py` & `bbm-0.0.6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `bbm-0.0.5/tests/test_bbm.py` & `bbm-0.0.6/tests/test_bbm.py`

 * *Files identical despite different names*

### Comparing `bbm-0.0.5/tests/test_data/es_search_scroll_response.json` & `bbm-0.0.6/tests/test_data/es_search_scroll_response.json`

 * *Files identical despite different names*

### Comparing `bbm-0.0.5/.gitignore` & `bbm-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `bbm-0.0.5/LICENSE` & `bbm-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `bbm-0.0.5/README.md` & `bbm-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `bbm-0.0.5/pyproject.toml` & `bbm-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bbm-0.0.5/PKG-INFO` & `bbm-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bbm
-Version: 0.0.5
+Version: 0.0.6
 Summary: 📊 Buzzni Batch process Monitor.
 Project-URL: homepage, https://github.com/buzzni/bbm
 Project-URL: bug-tracker, https://github.com/buzzni/bbm/issues
 Author-email: damonbuzzni <damon@buzzni.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
```

