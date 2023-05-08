# Comparing `tmp/goblet_gcp_client-0.1.3.tar.gz` & `tmp/goblet_gcp_client-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goblet_gcp_client-0.1.3.tar", last modified: Fri Mar 24 13:44:42 2023, max compression
+gzip compressed data, was "goblet_gcp_client-0.1.4.tar", last modified: Mon May  8 18:51:34 2023, max compression
```

## Comparing `goblet_gcp_client-0.1.3.tar` & `goblet_gcp_client-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 austennovis   (501) staff       (20)        0 2023-03-24 13:44:42.487197 goblet_gcp_client-0.1.3/
--rw-r--r--   0 austennovis   (501) staff       (20)    11357 2023-02-09 15:46:13.000000 goblet_gcp_client-0.1.3/LICENSE
--rw-r--r--   0 austennovis   (501) staff       (20)     4552 2023-03-24 13:44:42.486900 goblet_gcp_client-0.1.3/PKG-INFO
--rw-r--r--   0 austennovis   (501) staff       (20)     3722 2023-02-28 16:31:23.000000 goblet_gcp_client-0.1.3/README.md
-drwxr-xr-x   0 austennovis   (501) staff       (20)        0 2023-03-24 13:44:42.484829 goblet_gcp_client-0.1.3/goblet_gcp_client/
--rw-r--r--   0 austennovis   (501) staff       (20)      176 2023-03-24 13:44:32.000000 goblet_gcp_client-0.1.3/goblet_gcp_client/__init__.py
--rw-r--r--   0 austennovis   (501) staff       (20)       64 2023-03-24 13:44:32.000000 goblet_gcp_client-0.1.3/goblet_gcp_client/__version__.py
--rw-r--r--   0 austennovis   (501) staff       (20)     6335 2023-03-24 13:44:32.000000 goblet_gcp_client-0.1.3/goblet_gcp_client/client.py
--rw-r--r--   0 austennovis   (501) staff       (20)     6033 2023-03-24 13:44:32.000000 goblet_gcp_client-0.1.3/goblet_gcp_client/http_files.py
-drwxr-xr-x   0 austennovis   (501) staff       (20)        0 2023-03-24 13:44:42.486482 goblet_gcp_client-0.1.3/goblet_gcp_client.egg-info/
--rw-r--r--   0 austennovis   (501) staff       (20)     4552 2023-03-24 13:44:41.000000 goblet_gcp_client-0.1.3/goblet_gcp_client.egg-info/PKG-INFO
--rw-r--r--   0 austennovis   (501) staff       (20)      353 2023-03-24 13:44:42.000000 goblet_gcp_client-0.1.3/goblet_gcp_client.egg-info/SOURCES.txt
--rw-r--r--   0 austennovis   (501) staff       (20)        1 2023-03-24 13:44:41.000000 goblet_gcp_client-0.1.3/goblet_gcp_client.egg-info/dependency_links.txt
--rw-r--r--   0 austennovis   (501) staff       (20)       25 2023-03-24 13:44:42.000000 goblet_gcp_client-0.1.3/goblet_gcp_client.egg-info/requires.txt
--rw-r--r--   0 austennovis   (501) staff       (20)       18 2023-03-24 13:44:42.000000 goblet_gcp_client-0.1.3/goblet_gcp_client.egg-info/top_level.txt
--rw-r--r--   0 austennovis   (501) staff       (20)       38 2023-03-24 13:44:42.487283 goblet_gcp_client-0.1.3/setup.cfg
--rw-r--r--   0 austennovis   (501) staff       (20)     3382 2023-02-28 16:31:23.000000 goblet_gcp_client-0.1.3/setup.py
+drwxr-xr-x   0 austen.novis   (502) staff       (20)        0 2023-05-08 18:51:34.002220 goblet_gcp_client-0.1.4/
+-rw-r--r--   0 austen.novis   (502) staff       (20)    11357 2023-05-08 18:49:29.000000 goblet_gcp_client-0.1.4/LICENSE
+-rw-r--r--   0 austen.novis   (502) staff       (20)     4794 2023-05-08 18:51:34.002073 goblet_gcp_client-0.1.4/PKG-INFO
+-rw-r--r--   0 austen.novis   (502) staff       (20)     3984 2023-05-08 18:49:29.000000 goblet_gcp_client-0.1.4/README.md
+drwxr-xr-x   0 austen.novis   (502) staff       (20)        0 2023-05-08 18:51:34.001061 goblet_gcp_client-0.1.4/goblet_gcp_client/
+-rw-r--r--   0 austen.novis   (502) staff       (20)      200 2023-05-08 18:49:29.000000 goblet_gcp_client-0.1.4/goblet_gcp_client/__init__.py
+-rw-r--r--   0 austen.novis   (502) staff       (20)       64 2023-05-08 18:49:29.000000 goblet_gcp_client-0.1.4/goblet_gcp_client/__version__.py
+-rw-r--r--   0 austen.novis   (502) staff       (20)     6335 2023-05-08 18:49:29.000000 goblet_gcp_client-0.1.4/goblet_gcp_client/client.py
+-rw-r--r--   0 austen.novis   (502) staff       (20)     6033 2023-05-08 18:49:29.000000 goblet_gcp_client-0.1.4/goblet_gcp_client/http_files.py
+drwxr-xr-x   0 austen.novis   (502) staff       (20)        0 2023-05-08 18:51:34.001835 goblet_gcp_client-0.1.4/goblet_gcp_client.egg-info/
+-rw-r--r--   0 austen.novis   (502) staff       (20)     4794 2023-05-08 18:51:33.000000 goblet_gcp_client-0.1.4/goblet_gcp_client.egg-info/PKG-INFO
+-rw-r--r--   0 austen.novis   (502) staff       (20)      353 2023-05-08 18:51:33.000000 goblet_gcp_client-0.1.4/goblet_gcp_client.egg-info/SOURCES.txt
+-rw-r--r--   0 austen.novis   (502) staff       (20)        1 2023-05-08 18:51:33.000000 goblet_gcp_client-0.1.4/goblet_gcp_client.egg-info/dependency_links.txt
+-rw-r--r--   0 austen.novis   (502) staff       (20)       25 2023-05-08 18:51:33.000000 goblet_gcp_client-0.1.4/goblet_gcp_client.egg-info/requires.txt
+-rw-r--r--   0 austen.novis   (502) staff       (20)       18 2023-05-08 18:51:33.000000 goblet_gcp_client-0.1.4/goblet_gcp_client.egg-info/top_level.txt
+-rw-r--r--   0 austen.novis   (502) staff       (20)       38 2023-05-08 18:51:34.002276 goblet_gcp_client-0.1.4/setup.cfg
+-rw-r--r--   0 austen.novis   (502) staff       (20)     3382 2023-05-08 18:49:29.000000 goblet_gcp_client-0.1.4/setup.py
```

### Comparing `goblet_gcp_client-0.1.3/LICENSE` & `goblet_gcp_client-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `goblet_gcp_client-0.1.3/PKG-INFO` & `goblet_gcp_client-0.1.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: goblet_gcp_client
-Version: 0.1.3
+Version: 0.1.4
 Summary: GCP Client and GCP integration testing helpers
 Home-page: https://github.com/goblet/goblet_gcp_client
 Author: Austen
 Author-email: austen.novis@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -96,21 +95,23 @@
     )
 ```
 Running your test will record all responses that your Client makes
 
 Now you can run your tests with `G_HTTP_TEST` with `REPLAY`. You can access the responses with `get_responses` or `get_response`
 
 ```python
-from goblet_gcp_client import get_responses, get_response, get_replay_count
+from goblet_gcp_client import get_responses, get_response, get_replay_count, reset_replay_count
 
 def TestDeploy(self):
 
     monkeypatch.setenv("G_HTTP_TEST", "REPLAY")
     monkeypatch.setenv("G_TEST_NAME", "TEST_NAME")
 
+    reset_replay_count()
+
     cloudfunction_client = Client(
         "cloudfunctions",
         "v1",
         calls="projects.locations.functions",
         parent_schema="projects/{project_id}/locations/{location_id}",
     )
     cloudfunction_client.execute(
@@ -119,14 +120,16 @@
 
     responses = get_responses("TEST_NAME")
     assert len(responses) == 2
     assert "test_value" in responses[0]["body"]
     assert get_replay_count() == 1
 ```
 
+You can assert that your tests are making all required api called by using `get_replay_count`. If you are running multiple tests you can run `reset_replay_count` before each test to ensure the counts are accurate. 
+
 ## Features
 
 * GCP resource clients
 * GCP HTTP Test Recording and Replaying
 
 ## Examples
 
@@ -136,9 +139,7 @@
 ## Issues
 
 Please file any issues, bugs or feature requests as an issue on our [GitHub](https://github.com/goblet/goblet_gcp_client/issues) page.
 
 ## Want to Contribute
 
 If you would like to contribute to the library (e.g. by improving the documentation, solving a bug or adding a cool new feature) submit a [pull request](https://github.com/goblet/goblet_gcp_client/pulls).
-
-
```

### Comparing `goblet_gcp_client-0.1.3/README.md` & `goblet_gcp_client-0.1.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -73,21 +73,23 @@
     )
 ```
 Running your test will record all responses that your Client makes
 
 Now you can run your tests with `G_HTTP_TEST` with `REPLAY`. You can access the responses with `get_responses` or `get_response`
 
 ```python
-from goblet_gcp_client import get_responses, get_response, get_replay_count
+from goblet_gcp_client import get_responses, get_response, get_replay_count, reset_replay_count
 
 def TestDeploy(self):
 
     monkeypatch.setenv("G_HTTP_TEST", "REPLAY")
     monkeypatch.setenv("G_TEST_NAME", "TEST_NAME")
 
+    reset_replay_count()
+
     cloudfunction_client = Client(
         "cloudfunctions",
         "v1",
         calls="projects.locations.functions",
         parent_schema="projects/{project_id}/locations/{location_id}",
     )
     cloudfunction_client.execute(
@@ -96,14 +98,16 @@
 
     responses = get_responses("TEST_NAME")
     assert len(responses) == 2
     assert "test_value" in responses[0]["body"]
     assert get_replay_count() == 1
 ```
 
+You can assert that your tests are making all required api called by using `get_replay_count`. If you are running multiple tests you can run `reset_replay_count` before each test to ensure the counts are accurate. 
+
 ## Features
 
 * GCP resource clients
 * GCP HTTP Test Recording and Replaying
 
 ## Examples
```

### Comparing `goblet_gcp_client-0.1.3/goblet_gcp_client/client.py` & `goblet_gcp_client-0.1.4/goblet_gcp_client/client.py`

 * *Files identical despite different names*

### Comparing `goblet_gcp_client-0.1.3/goblet_gcp_client/http_files.py` & `goblet_gcp_client-0.1.4/goblet_gcp_client/http_files.py`

 * *Files identical despite different names*

### Comparing `goblet_gcp_client-0.1.3/goblet_gcp_client.egg-info/PKG-INFO` & `goblet_gcp_client-0.1.4/goblet_gcp_client.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: goblet-gcp-client
-Version: 0.1.3
+Version: 0.1.4
 Summary: GCP Client and GCP integration testing helpers
 Home-page: https://github.com/goblet/goblet_gcp_client
 Author: Austen
 Author-email: austen.novis@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -96,21 +95,23 @@
     )
 ```
 Running your test will record all responses that your Client makes
 
 Now you can run your tests with `G_HTTP_TEST` with `REPLAY`. You can access the responses with `get_responses` or `get_response`
 
 ```python
-from goblet_gcp_client import get_responses, get_response, get_replay_count
+from goblet_gcp_client import get_responses, get_response, get_replay_count, reset_replay_count
 
 def TestDeploy(self):
 
     monkeypatch.setenv("G_HTTP_TEST", "REPLAY")
     monkeypatch.setenv("G_TEST_NAME", "TEST_NAME")
 
+    reset_replay_count()
+
     cloudfunction_client = Client(
         "cloudfunctions",
         "v1",
         calls="projects.locations.functions",
         parent_schema="projects/{project_id}/locations/{location_id}",
     )
     cloudfunction_client.execute(
@@ -119,14 +120,16 @@
 
     responses = get_responses("TEST_NAME")
     assert len(responses) == 2
     assert "test_value" in responses[0]["body"]
     assert get_replay_count() == 1
 ```
 
+You can assert that your tests are making all required api called by using `get_replay_count`. If you are running multiple tests you can run `reset_replay_count` before each test to ensure the counts are accurate. 
+
 ## Features
 
 * GCP resource clients
 * GCP HTTP Test Recording and Replaying
 
 ## Examples
 
@@ -136,9 +139,7 @@
 ## Issues
 
 Please file any issues, bugs or feature requests as an issue on our [GitHub](https://github.com/goblet/goblet_gcp_client/issues) page.
 
 ## Want to Contribute
 
 If you would like to contribute to the library (e.g. by improving the documentation, solving a bug or adding a cool new feature) submit a [pull request](https://github.com/goblet/goblet_gcp_client/pulls).
-
-
```

### Comparing `goblet_gcp_client-0.1.3/setup.py` & `goblet_gcp_client-0.1.4/setup.py`

 * *Files identical despite different names*

