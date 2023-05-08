# Comparing `tmp/log10_io-0.0.5.tar.gz` & `tmp/log10_io-0.0.6.tar.gz`

## Comparing `log10_io-0.0.5.tar` & `log10_io-0.0.6.tar`

### file list

```diff
@@ -1,21 +1,22 @@
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 log10_io-0.0.5/requirements.txt
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 log10_io-0.0.5/setup.py
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 log10_io-0.0.5/.github/workflows/release.yml
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 log10_io-0.0.5/examples/chatcompletion.py
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 log10_io-0.0.5/examples/chatcompletion_async_vs_sync.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 log10_io-0.0.5/examples/completion.py
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 log10_io-0.0.5/examples/completion_ada.py
--rw-r--r--   0        0        0    10777 2020-02-02 00:00:00.000000 log10_io-0.0.5/examples/langchain_babyagi.py
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 log10_io-0.0.5/examples/langchain_multiple_tools.py
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 log10_io-0.0.5/examples/langchain_simple_sequential.py
--rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 log10_io-0.0.5/examples/langchain_sqlagent.py
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 log10_io-0.0.5/examples/multiple_sessions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 log10_io-0.0.5/log10/        __init__.py
--rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 log10_io-0.0.5/log10/bigquery.py
--rw-r--r--   0        0        0    10194 2020-02-02 00:00:00.000000 log10_io-0.0.5/log10/load.py
--rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 log10_io-0.0.5/log10/schemas/bigquery.json
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 log10_io-0.0.5/.gitignore
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 log10_io-0.0.5/LICENSE
--rw-r--r--   0        0        0     2620 2020-02-02 00:00:00.000000 log10_io-0.0.5/README.md
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 log10_io-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 log10_io-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 log10_io-0.0.6/requirements.txt
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 log10_io-0.0.6/setup.py
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 log10_io-0.0.6/.github/workflows/release.yml
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 log10_io-0.0.6/examples/chatcompletion.py
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 log10_io-0.0.6/examples/chatcompletion_async_vs_sync.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 log10_io-0.0.6/examples/completion.py
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 log10_io-0.0.6/examples/completion_ada.py
+-rw-r--r--   0        0        0    10777 2020-02-02 00:00:00.000000 log10_io-0.0.6/examples/langchain_babyagi.py
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 log10_io-0.0.6/examples/langchain_multiple_tools.py
+-rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 log10_io-0.0.6/examples/langchain_qa.py
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 log10_io-0.0.6/examples/langchain_simple_sequential.py
+-rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 log10_io-0.0.6/examples/langchain_sqlagent.py
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 log10_io-0.0.6/examples/multiple_sessions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 log10_io-0.0.6/log10/        __init__.py
+-rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 log10_io-0.0.6/log10/bigquery.py
+-rw-r--r--   0        0        0    10361 2020-02-02 00:00:00.000000 log10_io-0.0.6/log10/load.py
+-rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 log10_io-0.0.6/log10/schemas/bigquery.json
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 log10_io-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 log10_io-0.0.6/LICENSE
+-rw-r--r--   0        0        0     2715 2020-02-02 00:00:00.000000 log10_io-0.0.6/README.md
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 log10_io-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     3184 2020-02-02 00:00:00.000000 log10_io-0.0.6/PKG-INFO
```

### Comparing `log10_io-0.0.5/.github/workflows/release.yml` & `log10_io-0.0.6/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `log10_io-0.0.5/examples/chatcompletion_async_vs_sync.py` & `log10_io-0.0.6/examples/chatcompletion_async_vs_sync.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.0.5/examples/langchain_babyagi.py` & `log10_io-0.0.6/examples/langchain_babyagi.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.0.5/examples/langchain_multiple_tools.py` & `log10_io-0.0.6/examples/langchain_multiple_tools.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.0.5/examples/langchain_simple_sequential.py` & `log10_io-0.0.6/examples/langchain_simple_sequential.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.0.5/examples/langchain_sqlagent.py` & `log10_io-0.0.6/examples/langchain_sqlagent.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.0.5/examples/multiple_sessions.py` & `log10_io-0.0.6/examples/multiple_sessions.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.0.5/log10/bigquery.py` & `log10_io-0.0.6/log10/bigquery.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.0.5/log10/load.py` & `log10_io-0.0.6/log10/load.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,16 @@
         res = requests.request("POST",
                                session_url, headers={"x-log10-token": token, "Content-Type": "application/json"}, json={
                                    "organization_id": org_id
                                })
 
         return res.json()['sessionID']
     except Exception as e:
-        raise Exception("Failed to create LOG10 session: " + str(e))
+        raise Exception("Failed to create LOG10 session: " + str(e) + "\nLikely cause: LOG10 env vars missing or not picked up correctly!" +
+                        "\nSee https://github.com/log10-io/log10#%EF%B8%8F-setup for details")
 
 
 # Global variable to store the current sessionID.
 sessionID = get_session_id()
 
 
 class log10_session:
```

### Comparing `log10_io-0.0.5/log10/schemas/bigquery.json` & `log10_io-0.0.6/log10/schemas/bigquery.json`

 * *Files identical despite different names*

### Comparing `log10_io-0.0.5/LICENSE` & `log10_io-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `log10_io-0.0.5/README.md` & `log10_io-0.0.6/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -59,13 +59,17 @@
 
 **👥🤝 Collaboration**
 
 Create flexible groups to share and collaborate over all of the above features
 
 ## ⚙️ Setup
 
-Create a free account at [log10.io](https://log10.io) to get a `LOG10_TOKEN` and a `LOG10_ORG_ID`. Please add these to your environment along with `LOG10_URL=https://log10.io`. 
-
+1. Create a free account at [log10.io](https://log10.io)
+2. Set the following environment variables:
+- `LOG10_URL=https://log10.io`
+- `LOG10_TOKEN`: From the Settings tab in log10.io
+- `LOG10_ORG_ID`: From the Organization tab in log10.io
+- `OPENAI_API_KEY`: OpenAI API key
 
 ## 💬 Community
 
 We welcome community participation and feedback. Please leave an issue, submit a PR or join our [Discord](https://discord.gg/CZQvnuRV94).
```

### Comparing `log10_io-0.0.5/pyproject.toml` & `log10_io-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "log10-io"
-version = "0.0.5"
+version = "0.0.6"
 authors = []
 license = "MIT"
 description = "Unified LLM data management"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `log10_io-0.0.5/PKG-INFO` & `log10_io-0.0.6/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: log10-io
-Version: 0.0.5
+Version: 0.0.6
 Summary: Unified LLM data management
 Project-URL: Homepage, https://github.com/log10-io/log10
 Project-URL: Bug Tracker, https://github.com/log10-io/log10/issues
 License-Expression: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -73,13 +73,17 @@
 
 **👥🤝 Collaboration**
 
 Create flexible groups to share and collaborate over all of the above features
 
 ## ⚙️ Setup
 
-Create a free account at [log10.io](https://log10.io) to get a `LOG10_TOKEN` and a `LOG10_ORG_ID`. Please add these to your environment along with `LOG10_URL=https://log10.io`. 
-
+1. Create a free account at [log10.io](https://log10.io)
+2. Set the following environment variables:
+- `LOG10_URL=https://log10.io`
+- `LOG10_TOKEN`: From the Settings tab in log10.io
+- `LOG10_ORG_ID`: From the Organization tab in log10.io
+- `OPENAI_API_KEY`: OpenAI API key
 
 ## 💬 Community
 
 We welcome community participation and feedback. Please leave an issue, submit a PR or join our [Discord](https://discord.gg/CZQvnuRV94).
```

