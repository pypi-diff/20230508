# Comparing `tmp/issue_db_api-0.7.1.tar.gz` & `tmp/issue_db_api-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "issue_db_api-0.7.1.tar", last modified: Fri May  5 12:25:25 2023, max compression
+gzip compressed data, was "issue_db_api-0.7.2.tar", last modified: Mon May  8 13:34:52 2023, max compression
```

## Comparing `issue_db_api-0.7.1.tar` & `issue_db_api-0.7.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-05 12:25:25.425012 issue_db_api-0.7.1/
--rw-rw-r--   0 jesse     (1000) jesse     (1000)       82 2023-04-20 09:20:00.000000 issue_db_api-0.7.1/.gitignore
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     1069 2023-04-20 08:15:34.000000 issue_db_api-0.7.1/LICENSE
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      103 2023-04-20 08:15:34.000000 issue_db_api-0.7.1/MANIFEST.in
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      551 2023-05-05 12:25:25.425012 issue_db_api-0.7.1/PKG-INFO
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      200 2023-04-20 08:15:34.000000 issue_db_api-0.7.1/README.md
-drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-05 12:25:25.425012 issue_db_api-0.7.1/issue_db_api/
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      519 2023-05-05 12:21:06.000000 issue_db_api-0.7.1/issue_db_api/Cargo.toml
--rw-rw-r--   0 jesse     (1000) jesse     (1000)       25 2023-05-04 14:06:56.000000 issue_db_api-0.7.1/issue_db_api/__init__.py
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     8397 2023-05-04 14:07:06.000000 issue_db_api-0.7.1/issue_db_api/issue_api.pyi
-drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-05 12:25:25.425012 issue_db_api-0.7.1/issue_db_api/src/
--rw-rw-r--   0 jesse     (1000) jesse     (1000)    44361 2023-05-04 14:03:45.000000 issue_db_api-0.7.1/issue_db_api/src/api_core.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     1049 2023-05-04 13:53:55.000000 issue_db_api-0.7.1/issue_db_api/src/comments.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     5275 2023-05-04 13:53:55.000000 issue_db_api-0.7.1/issue_db_api/src/config.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     3788 2023-05-04 13:53:55.000000 issue_db_api-0.7.1/issue_db_api/src/embedding.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     2105 2023-05-04 13:55:29.000000 issue_db_api-0.7.1/issue_db_api/src/errors.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     6638 2023-05-04 13:53:55.000000 issue_db_api-0.7.1/issue_db_api/src/issues.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      571 2023-04-20 08:15:34.000000 issue_db_api-0.7.1/issue_db_api/src/labels.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)    38608 2023-05-04 13:59:32.000000 issue_db_api-0.7.1/issue_db_api/src/lib.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)    10983 2023-05-04 13:53:55.000000 issue_db_api-0.7.1/issue_db_api/src/models.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     3910 2023-05-01 16:59:08.000000 issue_db_api-0.7.1/issue_db_api/src/query.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     6387 2023-05-04 13:53:55.000000 issue_db_api-0.7.1/issue_db_api/src/repository.rs
-drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-05 12:25:25.425012 issue_db_api-0.7.1/issue_db_api/src/schemas/
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     5031 2023-04-20 08:15:34.000000 issue_db_api-0.7.1/issue_db_api/src/schemas/raw_issue_response.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)       27 2023-04-20 08:15:34.000000 issue_db_api-0.7.1/issue_db_api/src/schemas.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     1626 2023-05-04 13:53:55.000000 issue_db_api-0.7.1/issue_db_api/src/tags.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     2514 2023-05-05 12:20:10.000000 issue_db_api-0.7.1/issue_db_api/src/util.rs
-drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-05 12:25:25.425012 issue_db_api-0.7.1/issue_db_api.egg-info/
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      551 2023-05-05 12:25:25.000000 issue_db_api-0.7.1/issue_db_api.egg-info/PKG-INFO
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      748 2023-05-05 12:25:25.000000 issue_db_api-0.7.1/issue_db_api.egg-info/SOURCES.txt
--rw-rw-r--   0 jesse     (1000) jesse     (1000)        1 2023-05-05 12:25:25.000000 issue_db_api-0.7.1/issue_db_api.egg-info/dependency_links.txt
--rw-rw-r--   0 jesse     (1000) jesse     (1000)        1 2023-04-20 09:21:05.000000 issue_db_api-0.7.1/issue_db_api.egg-info/not-zip-safe
--rw-rw-r--   0 jesse     (1000) jesse     (1000)       13 2023-05-05 12:25:25.000000 issue_db_api-0.7.1/issue_db_api.egg-info/top_level.txt
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      529 2023-05-05 12:21:06.000000 issue_db_api-0.7.1/pyproject.toml
--rw-rw-r--   0 jesse     (1000) jesse     (1000)       38 2023-05-05 12:25:25.425012 issue_db_api-0.7.1/setup.cfg
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      253 2023-04-20 08:15:34.000000 issue_db_api-0.7.1/setup.py
+drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-08 13:34:52.473665 issue_db_api-0.7.2/
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)       82 2023-04-20 09:20:00.000000 issue_db_api-0.7.2/.gitignore
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     1069 2023-04-20 08:15:34.000000 issue_db_api-0.7.2/LICENSE
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      103 2023-04-20 08:15:34.000000 issue_db_api-0.7.2/MANIFEST.in
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      551 2023-05-08 13:34:52.473665 issue_db_api-0.7.2/PKG-INFO
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      200 2023-04-20 08:15:34.000000 issue_db_api-0.7.2/README.md
+drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-08 13:34:52.473665 issue_db_api-0.7.2/issue_db_api/
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      519 2023-05-08 13:34:16.000000 issue_db_api-0.7.2/issue_db_api/Cargo.toml
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)       25 2023-05-04 14:06:56.000000 issue_db_api-0.7.2/issue_db_api/__init__.py
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     8397 2023-05-04 14:07:06.000000 issue_db_api-0.7.2/issue_db_api/issue_api.pyi
+drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-08 13:34:52.473665 issue_db_api-0.7.2/issue_db_api/src/
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)    44393 2023-05-08 13:33:40.000000 issue_db_api-0.7.2/issue_db_api/src/api_core.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     1049 2023-05-04 13:53:55.000000 issue_db_api-0.7.2/issue_db_api/src/comments.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     5275 2023-05-04 13:53:55.000000 issue_db_api-0.7.2/issue_db_api/src/config.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     3788 2023-05-04 13:53:55.000000 issue_db_api-0.7.2/issue_db_api/src/embedding.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     2105 2023-05-04 13:55:29.000000 issue_db_api-0.7.2/issue_db_api/src/errors.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     6638 2023-05-04 13:53:55.000000 issue_db_api-0.7.2/issue_db_api/src/issues.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      571 2023-04-20 08:15:34.000000 issue_db_api-0.7.2/issue_db_api/src/labels.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)    38608 2023-05-04 13:59:32.000000 issue_db_api-0.7.2/issue_db_api/src/lib.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)    10983 2023-05-04 13:53:55.000000 issue_db_api-0.7.2/issue_db_api/src/models.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     3910 2023-05-01 16:59:08.000000 issue_db_api-0.7.2/issue_db_api/src/query.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     6387 2023-05-04 13:53:55.000000 issue_db_api-0.7.2/issue_db_api/src/repository.rs
+drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-08 13:34:52.473665 issue_db_api-0.7.2/issue_db_api/src/schemas/
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     5031 2023-04-20 08:15:34.000000 issue_db_api-0.7.2/issue_db_api/src/schemas/raw_issue_response.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)       27 2023-04-20 08:15:34.000000 issue_db_api-0.7.2/issue_db_api/src/schemas.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     1626 2023-05-04 13:53:55.000000 issue_db_api-0.7.2/issue_db_api/src/tags.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     2514 2023-05-05 12:20:10.000000 issue_db_api-0.7.2/issue_db_api/src/util.rs
+drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-08 13:34:52.473665 issue_db_api-0.7.2/issue_db_api.egg-info/
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      551 2023-05-08 13:34:52.000000 issue_db_api-0.7.2/issue_db_api.egg-info/PKG-INFO
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      748 2023-05-08 13:34:52.000000 issue_db_api-0.7.2/issue_db_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)        1 2023-05-08 13:34:52.000000 issue_db_api-0.7.2/issue_db_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)        1 2023-04-20 09:21:05.000000 issue_db_api-0.7.2/issue_db_api.egg-info/not-zip-safe
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)       13 2023-05-08 13:34:52.000000 issue_db_api-0.7.2/issue_db_api.egg-info/top_level.txt
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      529 2023-05-08 13:34:16.000000 issue_db_api-0.7.2/pyproject.toml
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)       38 2023-05-08 13:34:52.473665 issue_db_api-0.7.2/setup.cfg
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      253 2023-04-20 08:15:34.000000 issue_db_api-0.7.2/setup.py
```

### Comparing `issue_db_api-0.7.1/LICENSE` & `issue_db_api-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.7.1/PKG-INFO` & `issue_db_api-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: issue_db_api
-Version: 0.7.1
+Version: 0.7.2
 Author: Jesse Maarleveld
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `issue_db_api-0.7.1/issue_db_api/Cargo.toml` & `issue_db_api-0.7.2/issue_db_api/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "issue-api-client"
-version = "0.7.1"
+version = "0.7.2"
 edition = "2021"
 
 [lib]
 name = "issue_api"
 crate-type = ["cdylib"]
 
 [features]
```

### Comparing `issue_db_api-0.7.1/issue_db_api/issue_api.pyi` & `issue_db_api-0.7.2/issue_db_api/issue_api.pyi`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.7.1/issue_db_api/src/api_core.rs` & `issue_db_api-0.7.2/issue_db_api/src/api_core.rs`

 * *Files 0% similar despite different names*

```diff
@@ -442,14 +442,15 @@
     {
         let url = self.get_endpoint(suffix);
         let client = reqwest::Client::new();
         let rt = tokio::runtime::Builder::new_current_thread().enable_all().build()?;
         let result: APIResult<()> = rt.block_on(async {
             let mut stream = client
                 .get(url)
+                .json(&payload)
                 .send()
                 .await?
                 .error_for_status()?;
             while let Some(chunk) = stream.chunk().await? {
                 sink.write_all(chunk.as_ref())?;
             }
             Ok(())
```

### Comparing `issue_db_api-0.7.1/issue_db_api/src/comments.rs` & `issue_db_api-0.7.2/issue_db_api/src/comments.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.7.1/issue_db_api/src/config.rs` & `issue_db_api-0.7.2/issue_db_api/src/config.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.7.1/issue_db_api/src/embedding.rs` & `issue_db_api-0.7.2/issue_db_api/src/embedding.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.7.1/issue_db_api/src/errors.rs` & `issue_db_api-0.7.2/issue_db_api/src/errors.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.7.1/issue_db_api/src/issues.rs` & `issue_db_api-0.7.2/issue_db_api/src/issues.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.7.1/issue_db_api/src/labels.rs` & `issue_db_api-0.7.2/issue_db_api/src/labels.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.7.1/issue_db_api/src/lib.rs` & `issue_db_api-0.7.2/issue_db_api/src/lib.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.7.1/issue_db_api/src/models.rs` & `issue_db_api-0.7.2/issue_db_api/src/models.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.7.1/issue_db_api/src/query.rs` & `issue_db_api-0.7.2/issue_db_api/src/query.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.7.1/issue_db_api/src/repository.rs` & `issue_db_api-0.7.2/issue_db_api/src/repository.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.7.1/issue_db_api/src/schemas/raw_issue_response.rs` & `issue_db_api-0.7.2/issue_db_api/src/schemas/raw_issue_response.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.7.1/issue_db_api/src/tags.rs` & `issue_db_api-0.7.2/issue_db_api/src/tags.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.7.1/issue_db_api/src/util.rs` & `issue_db_api-0.7.2/issue_db_api/src/util.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.7.1/issue_db_api.egg-info/PKG-INFO` & `issue_db_api-0.7.2/issue_db_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: issue-db-api
-Version: 0.7.1
+Version: 0.7.2
 Author: Jesse Maarleveld
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `issue_db_api-0.7.1/issue_db_api.egg-info/SOURCES.txt` & `issue_db_api-0.7.2/issue_db_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.7.1/pyproject.toml` & `issue_db_api-0.7.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.setuptools.packages.find]
 where=["."]
 include = ["issue_db_api"]
 
 [project]
 name = "issue_db_api"
-version = "0.7.1"
+version = "0.7.2"
 authors = [
     {name = "Jesse Maarleveld"},
 ]
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Rust",
```

