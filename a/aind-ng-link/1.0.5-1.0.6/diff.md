# Comparing `tmp/aind-ng-link-1.0.5.tar.gz` & `tmp/aind-ng-link-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aind-ng-link-1.0.5.tar", last modified: Wed May  3 16:28:12 2023, max compression
+gzip compressed data, was "aind-ng-link-1.0.6.tar", last modified: Mon May  8 19:05:52 2023, max compression
```

## Comparing `aind-ng-link-1.0.5.tar` & `aind-ng-link-1.0.6.tar`

### file list

```diff
@@ -1,50 +1,51 @@
-drwxr-xr-x   0 jonathan.wong   (502) staff       (20)        0 2023-05-03 16:28:12.339367 aind-ng-link-1.0.5/
--rw-r--r--   0 jonathan.wong   (502) staff       (20)      170 2023-04-28 19:56:56.000000 aind-ng-link-1.0.5/.flake8
-drwxr-xr-x   0 jonathan.wong   (502) staff       (20)        0 2023-05-03 16:28:12.088622 aind-ng-link-1.0.5/.github/
-drwxr-xr-x   0 jonathan.wong   (502) staff       (20)        0 2023-05-03 16:28:12.141366 aind-ng-link-1.0.5/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 jonathan.wong   (502) staff       (20)      834 2023-03-20 20:38:13.000000 aind-ng-link-1.0.5/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 jonathan.wong   (502) staff       (20)      595 2023-03-20 20:38:13.000000 aind-ng-link-1.0.5/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 jonathan.wong   (502) staff       (20)      772 2023-03-20 20:38:13.000000 aind-ng-link-1.0.5/.github/ISSUE_TEMPLATE/user-story.md
-drwxr-xr-x   0 jonathan.wong   (502) staff       (20)        0 2023-05-03 16:28:12.169923 aind-ng-link-1.0.5/.github/workflows/
--rw-r--r--   0 jonathan.wong   (502) staff       (20)     1471 2023-03-20 20:38:13.000000 aind-ng-link-1.0.5/.github/workflows/ci.yml
--rw-r--r--   0 jonathan.wong   (502) staff       (20)      713 2023-03-20 20:38:13.000000 aind-ng-link-1.0.5/.github/workflows/tag.yml
--rw-r--r--   0 jonathan.wong   (502) staff       (20)     2199 2023-03-20 20:38:13.000000 aind-ng-link-1.0.5/.gitignore
--rw-r--r--   0 jonathan.wong   (502) staff       (20)     1092 2023-03-20 20:38:13.000000 aind-ng-link-1.0.5/LICENSE
--rw-r--r--   0 jonathan.wong   (502) staff       (20)     2900 2023-05-03 16:28:12.338487 aind-ng-link-1.0.5/PKG-INFO
--rw-r--r--   0 jonathan.wong   (502) staff       (20)     2451 2023-04-28 19:56:56.000000 aind-ng-link-1.0.5/README.md
-drwxr-xr-x   0 jonathan.wong   (502) staff       (20)        0 2023-05-03 16:28:12.179018 aind-ng-link-1.0.5/doc_template/
--rw-r--r--   0 jonathan.wong   (502) staff       (20)      638 2023-03-20 20:38:13.000000 aind-ng-link-1.0.5/doc_template/Makefile
--rw-r--r--   0 jonathan.wong   (502) staff       (20)      769 2023-03-20 20:38:13.000000 aind-ng-link-1.0.5/doc_template/make.bat
-drwxr-xr-x   0 jonathan.wong   (502) staff       (20)        0 2023-05-03 16:28:12.189262 aind-ng-link-1.0.5/doc_template/source/
--rw-r--r--   0 jonathan.wong   (502) staff       (20)     1540 2023-03-20 20:38:13.000000 aind-ng-link-1.0.5/doc_template/source/conf.py
--rw-r--r--   0 jonathan.wong   (502) staff       (20)      470 2023-03-20 20:38:13.000000 aind-ng-link-1.0.5/doc_template/source/index.rst
--rw-r--r--   0 jonathan.wong   (502) staff       (20)     1610 2023-04-28 19:56:56.000000 aind-ng-link-1.0.5/pyproject.toml
--rw-r--r--   0 jonathan.wong   (502) staff       (20)     2269 2023-04-28 19:56:56.000000 aind-ng-link-1.0.5/requirements.txt
--rw-r--r--   0 jonathan.wong   (502) staff       (20)       38 2023-05-03 16:28:12.339589 aind-ng-link-1.0.5/setup.cfg
--rw-r--r--   0 jonathan.wong   (502) staff       (20)      256 2023-04-28 19:56:56.000000 aind-ng-link-1.0.5/setup.py
-drwxr-xr-x   0 jonathan.wong   (502) staff       (20)        0 2023-05-03 16:28:12.091113 aind-ng-link-1.0.5/src/
-drwxr-xr-x   0 jonathan.wong   (502) staff       (20)        0 2023-05-03 16:28:12.200680 aind-ng-link-1.0.5/src/aind_ng_link.egg-info/
--rw-r--r--   0 jonathan.wong   (502) staff       (20)     2900 2023-05-03 16:28:11.000000 aind-ng-link-1.0.5/src/aind_ng_link.egg-info/PKG-INFO
--rw-r--r--   0 jonathan.wong   (502) staff       (20)      961 2023-05-03 16:28:12.000000 aind-ng-link-1.0.5/src/aind_ng_link.egg-info/SOURCES.txt
--rw-r--r--   0 jonathan.wong   (502) staff       (20)        1 2023-05-03 16:28:11.000000 aind-ng-link-1.0.5/src/aind_ng_link.egg-info/dependency_links.txt
--rw-r--r--   0 jonathan.wong   (502) staff       (20)      137 2023-05-03 16:28:11.000000 aind-ng-link-1.0.5/src/aind_ng_link.egg-info/requires.txt
--rw-r--r--   0 jonathan.wong   (502) staff       (20)        8 2023-05-03 16:28:11.000000 aind-ng-link-1.0.5/src/aind_ng_link.egg-info/top_level.txt
-drwxr-xr-x   0 jonathan.wong   (502) staff       (20)        0 2023-05-03 16:28:12.249569 aind-ng-link-1.0.5/src/ng_link/
--rw-r--r--   0 jonathan.wong   (502) staff       (20)      181 2023-05-03 16:24:50.000000 aind-ng-link-1.0.5/src/ng_link/__init__.py
--rw-r--r--   0 jonathan.wong   (502) staff       (20)     6444 2023-05-02 17:25:23.000000 aind-ng-link-1.0.5/src/ng_link/dispim_link.py
--rw-r--r--   0 jonathan.wong   (502) staff       (20)     3691 2023-05-03 16:22:24.000000 aind-ng-link-1.0.5/src/ng_link/exaspim_link.py
--rw-r--r--   0 jonathan.wong   (502) staff       (20)     4403 2023-04-28 19:56:56.000000 aind-ng-link-1.0.5/src/ng_link/link_utils.py
--rw-r--r--   0 jonathan.wong   (502) staff       (20)    42266 2023-04-27 22:17:45.000000 aind-ng-link-1.0.5/src/ng_link/ng_layer.py
--rw-r--r--   0 jonathan.wong   (502) staff       (20)    29463 2023-04-28 19:56:56.000000 aind-ng-link-1.0.5/src/ng_link/ng_state.py
-drwxr-xr-x   0 jonathan.wong   (502) staff       (20)        0 2023-05-03 16:28:12.282405 aind-ng-link-1.0.5/src/ng_link/scripts/
--rw-r--r--   0 jonathan.wong   (502) staff       (20)    13902 2023-04-25 22:57:30.000000 aind-ng-link-1.0.5/src/ng_link/scripts/ccf_ref.csv
--rw-r--r--   0 jonathan.wong   (502) staff       (20)      909 2023-05-02 17:27:04.000000 aind-ng-link-1.0.5/src/ng_link/scripts/create_links.py
--rw-r--r--   0 jonathan.wong   (502) staff       (20)     6945 2023-04-28 19:56:56.000000 aind-ng-link-1.0.5/src/ng_link/scripts/generate_cff_cell_count.py
-drwxr-xr-x   0 jonathan.wong   (502) staff       (20)        0 2023-05-03 16:28:12.299290 aind-ng-link-1.0.5/src/ng_link/utils/
--rw-r--r--   0 jonathan.wong   (502) staff       (20)       61 2023-03-20 20:38:13.000000 aind-ng-link-1.0.5/src/ng_link/utils/__init__.py
--rw-r--r--   0 jonathan.wong   (502) staff       (20)     5929 2023-04-27 22:17:44.000000 aind-ng-link-1.0.5/src/ng_link/utils/utils.py
--rw-r--r--   0 jonathan.wong   (502) staff       (20)     2545 2023-04-28 19:56:56.000000 aind-ng-link-1.0.5/src/ng_link/xml_parsing.py
-drwxr-xr-x   0 jonathan.wong   (502) staff       (20)        0 2023-05-03 16:28:12.337280 aind-ng-link-1.0.5/tests/
--rw-r--r--   0 jonathan.wong   (502) staff       (20)       22 2023-03-20 20:38:13.000000 aind-ng-link-1.0.5/tests/__init__.py
--rw-r--r--   0 jonathan.wong   (502) staff       (20)      192 2023-04-28 15:42:24.000000 aind-ng-link-1.0.5/tests/test_ng_layer.py
--rw-r--r--   0 jonathan.wong   (502) staff       (20)      192 2023-03-20 20:38:13.000000 aind-ng-link-1.0.5/tests/test_ng_state.py
+drwxr-xr-x   0 jonathan.wong   (502) staff       (20)        0 2023-05-08 19:05:52.003843 aind-ng-link-1.0.6/
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)      204 2023-05-08 18:58:30.000000 aind-ng-link-1.0.6/.flake8
+drwxr-xr-x   0 jonathan.wong   (502) staff       (20)        0 2023-05-08 19:05:51.578264 aind-ng-link-1.0.6/.github/
+drwxr-xr-x   0 jonathan.wong   (502) staff       (20)        0 2023-05-08 19:05:51.654691 aind-ng-link-1.0.6/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)      834 2023-03-20 20:38:13.000000 aind-ng-link-1.0.6/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)      595 2023-03-20 20:38:13.000000 aind-ng-link-1.0.6/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)      772 2023-03-20 20:38:13.000000 aind-ng-link-1.0.6/.github/ISSUE_TEMPLATE/user-story.md
+drwxr-xr-x   0 jonathan.wong   (502) staff       (20)        0 2023-05-08 19:05:51.687152 aind-ng-link-1.0.6/.github/workflows/
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)     1471 2023-03-20 20:38:13.000000 aind-ng-link-1.0.6/.github/workflows/ci.yml
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)      713 2023-03-20 20:38:13.000000 aind-ng-link-1.0.6/.github/workflows/tag.yml
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)     2240 2023-05-08 18:35:28.000000 aind-ng-link-1.0.6/.gitignore
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)     1092 2023-03-20 20:38:13.000000 aind-ng-link-1.0.6/LICENSE
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)     2900 2023-05-08 19:05:52.001365 aind-ng-link-1.0.6/PKG-INFO
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)     2451 2023-04-28 19:56:56.000000 aind-ng-link-1.0.6/README.md
+drwxr-xr-x   0 jonathan.wong   (502) staff       (20)        0 2023-05-08 19:05:51.706253 aind-ng-link-1.0.6/doc_template/
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)      638 2023-03-20 20:38:13.000000 aind-ng-link-1.0.6/doc_template/Makefile
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)      769 2023-03-20 20:38:13.000000 aind-ng-link-1.0.6/doc_template/make.bat
+drwxr-xr-x   0 jonathan.wong   (502) staff       (20)        0 2023-05-08 19:05:51.732650 aind-ng-link-1.0.6/doc_template/source/
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)     1540 2023-03-20 20:38:13.000000 aind-ng-link-1.0.6/doc_template/source/conf.py
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)      470 2023-03-20 20:38:13.000000 aind-ng-link-1.0.6/doc_template/source/index.rst
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)     1610 2023-04-28 19:56:56.000000 aind-ng-link-1.0.6/pyproject.toml
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)     2269 2023-04-28 19:56:56.000000 aind-ng-link-1.0.6/requirements.txt
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)       38 2023-05-08 19:05:52.004145 aind-ng-link-1.0.6/setup.cfg
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)      257 2023-05-08 18:41:43.000000 aind-ng-link-1.0.6/setup.py
+drwxr-xr-x   0 jonathan.wong   (502) staff       (20)        0 2023-05-08 19:05:51.585478 aind-ng-link-1.0.6/src/
+drwxr-xr-x   0 jonathan.wong   (502) staff       (20)        0 2023-05-08 19:05:51.747708 aind-ng-link-1.0.6/src/aind_ng_link.egg-info/
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)     2900 2023-05-08 19:05:51.000000 aind-ng-link-1.0.6/src/aind_ng_link.egg-info/PKG-INFO
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)      985 2023-05-08 19:05:51.000000 aind-ng-link-1.0.6/src/aind_ng_link.egg-info/SOURCES.txt
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)        1 2023-05-08 19:05:51.000000 aind-ng-link-1.0.6/src/aind_ng_link.egg-info/dependency_links.txt
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)      137 2023-05-08 19:05:51.000000 aind-ng-link-1.0.6/src/aind_ng_link.egg-info/requires.txt
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)        8 2023-05-08 19:05:51.000000 aind-ng-link-1.0.6/src/aind_ng_link.egg-info/top_level.txt
+drwxr-xr-x   0 jonathan.wong   (502) staff       (20)        0 2023-05-08 19:05:51.897483 aind-ng-link-1.0.6/src/ng_link/
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)      183 2023-05-08 18:36:39.000000 aind-ng-link-1.0.6/src/ng_link/__init__.py
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)     6549 2023-05-08 18:41:43.000000 aind-ng-link-1.0.6/src/ng_link/dispim_link.py
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)     3692 2023-05-08 18:41:43.000000 aind-ng-link-1.0.6/src/ng_link/exaspim_link.py
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)     4404 2023-05-08 18:41:43.000000 aind-ng-link-1.0.6/src/ng_link/link_utils.py
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)    42266 2023-04-27 22:17:45.000000 aind-ng-link-1.0.6/src/ng_link/ng_layer.py
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)    29463 2023-04-28 19:56:56.000000 aind-ng-link-1.0.6/src/ng_link/ng_state.py
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)     3544 2023-05-08 19:00:32.000000 aind-ng-link-1.0.6/src/ng_link/raw_link.py
+drwxr-xr-x   0 jonathan.wong   (502) staff       (20)        0 2023-05-08 19:05:51.949380 aind-ng-link-1.0.6/src/ng_link/scripts/
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)    13902 2023-04-25 22:57:30.000000 aind-ng-link-1.0.6/src/ng_link/scripts/ccf_ref.csv
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)     1098 2023-05-08 18:57:18.000000 aind-ng-link-1.0.6/src/ng_link/scripts/create_links.py
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)     6943 2023-05-08 18:41:43.000000 aind-ng-link-1.0.6/src/ng_link/scripts/generate_cff_cell_count.py
+drwxr-xr-x   0 jonathan.wong   (502) staff       (20)        0 2023-05-08 19:05:51.990304 aind-ng-link-1.0.6/src/ng_link/utils/
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)       61 2023-03-20 20:38:13.000000 aind-ng-link-1.0.6/src/ng_link/utils/__init__.py
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)     5929 2023-04-27 22:17:44.000000 aind-ng-link-1.0.6/src/ng_link/utils/utils.py
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)     2653 2023-05-08 18:41:43.000000 aind-ng-link-1.0.6/src/ng_link/xml_parsing.py
+drwxr-xr-x   0 jonathan.wong   (502) staff       (20)        0 2023-05-08 19:05:51.998770 aind-ng-link-1.0.6/tests/
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)       22 2023-03-20 20:38:13.000000 aind-ng-link-1.0.6/tests/__init__.py
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)      192 2023-04-28 15:42:24.000000 aind-ng-link-1.0.6/tests/test_ng_layer.py
+-rw-r--r--   0 jonathan.wong   (502) staff       (20)      192 2023-03-20 20:38:13.000000 aind-ng-link-1.0.6/tests/test_ng_state.py
```

### Comparing `aind-ng-link-1.0.5/.github/ISSUE_TEMPLATE/bug_report.md` & `aind-ng-link-1.0.6/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `aind-ng-link-1.0.5/.github/ISSUE_TEMPLATE/feature_request.md` & `aind-ng-link-1.0.6/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `aind-ng-link-1.0.5/.github/ISSUE_TEMPLATE/user-story.md` & `aind-ng-link-1.0.6/.github/ISSUE_TEMPLATE/user-story.md`

 * *Files identical despite different names*

### Comparing `aind-ng-link-1.0.5/.github/workflows/ci.yml` & `aind-ng-link-1.0.6/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `aind-ng-link-1.0.5/.github/workflows/tag.yml` & `aind-ng-link-1.0.6/.github/workflows/tag.yml`

 * *Files identical despite different names*

### Comparing `aind-ng-link-1.0.5/.gitignore` & `aind-ng-link-1.0.6/.gitignore`

 * *Files 3% similar despite different names*

```diff
@@ -133,7 +133,11 @@
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 .idea/
 
 # MacOs
 **/.DS_Store
+
+# Tester Files
+*.xml
+process_output.json
```

### Comparing `aind-ng-link-1.0.5/LICENSE` & `aind-ng-link-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `aind-ng-link-1.0.5/PKG-INFO` & `aind-ng-link-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aind-ng-link
-Version: 1.0.5
+Version: 1.0.6
 Summary: Python package for the generation of neuroglancer links
 Author-email: David Feng <david.feng@alleninstitute.org>, Sharmishtaa Seshamani <sharmishtaas@alleninstitute.org>, Camilo Laiton <camilo.laiton@alleninstitute.org>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
```

### Comparing `aind-ng-link-1.0.5/README.md` & `aind-ng-link-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `aind-ng-link-1.0.5/doc_template/Makefile` & `aind-ng-link-1.0.6/doc_template/Makefile`

 * *Files identical despite different names*

### Comparing `aind-ng-link-1.0.5/doc_template/make.bat` & `aind-ng-link-1.0.6/doc_template/make.bat`

 * *Files identical despite different names*

### Comparing `aind-ng-link-1.0.5/doc_template/source/conf.py` & `aind-ng-link-1.0.6/doc_template/source/conf.py`

 * *Files identical despite different names*

### Comparing `aind-ng-link-1.0.5/pyproject.toml` & `aind-ng-link-1.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aind-ng-link-1.0.5/requirements.txt` & `aind-ng-link-1.0.6/requirements.txt`

 * *Files identical despite different names*

### Comparing `aind-ng-link-1.0.5/src/aind_ng_link.egg-info/PKG-INFO` & `aind-ng-link-1.0.6/src/aind_ng_link.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aind-ng-link
-Version: 1.0.5
+Version: 1.0.6
 Summary: Python package for the generation of neuroglancer links
 Author-email: David Feng <david.feng@alleninstitute.org>, Sharmishtaa Seshamani <sharmishtaas@alleninstitute.org>, Camilo Laiton <camilo.laiton@alleninstitute.org>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
```

### Comparing `aind-ng-link-1.0.5/src/aind_ng_link.egg-info/SOURCES.txt` & `aind-ng-link-1.0.6/src/aind_ng_link.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 src/aind_ng_link.egg-info/top_level.txt
 src/ng_link/__init__.py
 src/ng_link/dispim_link.py
 src/ng_link/exaspim_link.py
 src/ng_link/link_utils.py
 src/ng_link/ng_layer.py
 src/ng_link/ng_state.py
+src/ng_link/raw_link.py
 src/ng_link/xml_parsing.py
 src/ng_link/scripts/ccf_ref.csv
 src/ng_link/scripts/create_links.py
 src/ng_link/scripts/generate_cff_cell_count.py
 src/ng_link/utils/__init__.py
 src/ng_link/utils/utils.py
 tests/__init__.py
```

### Comparing `aind-ng-link-1.0.5/src/ng_link/dispim_link.py` & `aind-ng-link-1.0.6/src/ng_link/dispim_link.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Library for generating dispim link.
 """
 import numpy as np
 
-from ng_link import NgState, xml_parsing, link_utils
+from ng_link import NgState, link_utils, xml_parsing
 
 
 def apply_deskewing(matrix_3x4: np.ndarray, theta: float = 45) -> np.ndarray:
     """
     Compounds deskewing transform to input 3x4 matrix:
         Deskewing @ Input_3x4_Matrix.
 
@@ -30,14 +30,15 @@
     # X vector => XZ direction
     deskew_factor = np.tan(np.deg2rad(theta))
     deskew = np.array([[1, 0, 0], [0, 1, 0], [deskew_factor, 0, 1]])
     matrix_3x4 = deskew @ matrix_3x4
 
     return matrix_3x4
 
+
 def generate_dispim_link(
     base_channel_xml_path: str,
     cross_channel_xml_path: str,
     s3_path: str,
     max_dr: int = 800,
     opacity: float = 0.5,
     blend: str = "additive",
@@ -180,15 +181,19 @@
                 np.linalg.inv(c_matrix_3x3) @ i_translation
             ) + c_translation
             net_tf = np.hstack((net_matrix_3x3, net_translation.reshape(3, 1)))
 
             net_tf = apply_deskewing(net_tf, deskew_angle)
 
             # Add (path, transform) source entry
-            url = f"{s3_path}/{t_path}"
+            if s3_path.endswith("/"):
+                url = f"{s3_path}{t_path}"
+            else:
+                url = f"{s3_path}/{t_path}"
+
             final_transform = link_utils.convert_matrix_3x4_to_5x6(net_tf)
             sources.append(
                 {"url": url, "transform_matrix": final_transform.tolist()}
             )
 
     # Generate the link
     neuroglancer_link = NgState(
```

### Comparing `aind-ng-link-1.0.5/src/ng_link/exaspim_link.py` & `aind-ng-link-1.0.6/src/ng_link/exaspim_link.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Library for generating exaspim link.
 """
 import numpy as np
 
-from ng_link import NgState, xml_parsing, link_utils
+from ng_link import NgState, link_utils, xml_parsing
+
 
 def omit_initial_offsets(view_transforms: dict[int, list[dict]]) -> None:
     """
     For OME-Zarr datasets, inital offsets are
     already encoded in the metadata and extracted my neuroglancer.
     This function removes the duplicate transform.
```

### Comparing `aind-ng-link-1.0.5/src/ng_link/link_utils.py` & `aind-ng-link-1.0.6/src/ng_link/link_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Utilities for nueroglancer links.
 """
+import re
 from collections import defaultdict
+
 import numpy as np
-import re
 
 
 def calculate_net_transforms(
     view_transforms: dict[int, list[dict]]
 ) -> dict[int, np.ndarray]:
     """
     Accumulate net transform and net translation for each matrix stack.
```

### Comparing `aind-ng-link-1.0.5/src/ng_link/ng_layer.py` & `aind-ng-link-1.0.6/src/ng_link/ng_layer.py`

 * *Files identical despite different names*

### Comparing `aind-ng-link-1.0.5/src/ng_link/ng_state.py` & `aind-ng-link-1.0.6/src/ng_link/ng_state.py`

 * *Files identical despite different names*

### Comparing `aind-ng-link-1.0.5/src/ng_link/scripts/ccf_ref.csv` & `aind-ng-link-1.0.6/src/ng_link/scripts/ccf_ref.csv`

 * *Files identical despite different names*

### Comparing `aind-ng-link-1.0.5/src/ng_link/scripts/create_links.py` & `aind-ng-link-1.0.6/src/ng_link/scripts/create_links.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,37 +1,43 @@
 # from ng_link import exaspim_link
-from ng_link import dispim_link
+# from ng_link import dispim_link
+from ng_link import raw_link
+
 
 def main():
     # Fill in your own data
-    base_channel_path = (
-        "/Users/jonathan.wong/Projects/aind-ng-link/registered_tester.xml"
-    )
-    cross_channel_path = (
-        "/Users/jonathan.wong/Projects/aind-ng-link/registered_tester_coreg.xml"
-    )
+    base_channel_path = "/Users/jonathan.wong/Projects/aind-ng-link/tester.xml"
+    # cross_channel_path = "/Users/jonathan.wong/Projects/aind-ng-link/registered_tester_coreg.xml"
     s3_path = (
         "s3://aind-open-data/diSPIM_647459_2022-12-21_00-39-00/diSPIM.zarr"
     )
 
     # exaspim_link.generate_exaspim_link(
     #     base_channel_path,
     #     s3_path,
     #     max_dr=200,
     #     opacity=1.0,
     #     blend="default",
     #     output_json_path=".",
     # )
-    dispim_link.generate_dispim_link(
+    # dispim_link.generate_dispim_link(
+    #     base_channel_path,
+    #     cross_channel_path,
+    #     s3_path,
+    #     max_dr=800,
+    #     opacity=0.5,
+    #     blend="additive",
+    #     deskew_angle=-45,
+    #     output_json_path=".",
+    # )
+    raw_link.generate_raw_link(
         base_channel_path,
-        cross_channel_path,
         s3_path,
-        max_dr=800,
-        opacity=0.5,
-        blend="additive",
-        deskew_angle=-45,
+        max_dr=200,
+        opacity=1.0,
+        blend="default",
         output_json_path=".",
     )
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `aind-ng-link-1.0.5/src/ng_link/scripts/generate_cff_cell_count.py` & `aind-ng-link-1.0.6/src/ng_link/scripts/generate_cff_cell_count.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,20 +4,18 @@
 
 import json
 import os
 from pathlib import Path
 from typing import Optional, Union
 
 import boto3
-
 # import neuroglancer
 import pandas as pd
 
 from ng_link import NgState
-
 # from ng_link.ng_layer import generate_precomputed_cells
 from ng_link.ng_state import get_points_from_xml
 
 # IO types
 PathLike = Union[str, Path]
```

### Comparing `aind-ng-link-1.0.5/src/ng_link/utils/utils.py` & `aind-ng-link-1.0.6/src/ng_link/utils/utils.py`

 * *Files identical despite different names*

### Comparing `aind-ng-link-1.0.5/src/ng_link/xml_parsing.py` & `aind-ng-link-1.0.6/src/ng_link/xml_parsing.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """
 Utilities for parsing BDV XML
 """
-import xmltodict
 from collections import OrderedDict
 
+import xmltodict
+
+
 def extract_tile_paths(xml_path: str) -> dict[int, str]:
     """
     Parses BDV xml and outputs map of setup_id -> tile path.
 
     Parameters
     ------------------------
     xml_path: str
@@ -81,14 +83,17 @@
     """
 
     view_transforms: dict[int, list[dict]] = {}
     with open(xml_path, "r") as file:
         data: OrderedDict = xmltodict.parse(file.read())
 
     for view_reg in data["SpimData"]["ViewRegistrations"]["ViewRegistration"]:
-        view_transforms[int(view_reg["@setup"])] = view_reg["ViewTransform"]
+        tfm_stack = view_reg["ViewTransform"]
+        if type(tfm_stack) is not list:
+            tfm_stack = [tfm_stack]
+        view_transforms[int(view_reg["@setup"])] = tfm_stack
 
     view_transforms = {
         view: tfs[::-1] for view, tfs in view_transforms.items()
     }
 
     return view_transforms
```

