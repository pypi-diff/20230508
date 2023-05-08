# Comparing `tmp/hauntedhouse-0.0.7.tar.gz` & `tmp/hauntedhouse-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hauntedhouse-0.0.7.tar", last modified: Wed Mar  8 20:37:55 2023, max compression
+gzip compressed data, was "hauntedhouse-0.0.9.tar", last modified: Thu Mar 23 18:18:25 2023, max compression
```

## Comparing `hauntedhouse-0.0.7.tar` & `hauntedhouse-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 asdougl   (1000) asdougl   (1000)        0 2023-03-08 20:37:55.127055 hauntedhouse-0.0.7/
--rw-rw-r--   0 asdougl   (1000) asdougl   (1000)      193 2023-03-08 20:37:55.127055 hauntedhouse-0.0.7/PKG-INFO
-drwxrwxr-x   0 asdougl   (1000) asdougl   (1000)        0 2023-03-08 20:37:55.123055 hauntedhouse-0.0.7/hauntedhouse/
--rw-rw-r--   0 asdougl   (1000) asdougl   (1000)       40 2023-02-09 19:03:43.000000 hauntedhouse-0.0.7/hauntedhouse/__init__.py
--rw-rw-r--   0 asdougl   (1000) asdougl   (1000)     8548 2023-03-08 20:37:09.000000 hauntedhouse-0.0.7/hauntedhouse/client.py
--rw-rw-r--   0 asdougl   (1000) asdougl   (1000)     6624 2023-03-07 21:32:11.000000 hauntedhouse-0.0.7/hauntedhouse/ingest.py
--rw-rw-r--   0 asdougl   (1000) asdougl   (1000)     1870 2023-03-07 15:41:30.000000 hauntedhouse-0.0.7/hauntedhouse/search.py
--rw-rw-r--   0 asdougl   (1000) asdougl   (1000)      830 2023-02-09 19:03:43.000000 hauntedhouse-0.0.7/hauntedhouse/status.py
-drwxrwxr-x   0 asdougl   (1000) asdougl   (1000)        0 2023-03-08 20:37:55.127055 hauntedhouse-0.0.7/hauntedhouse.egg-info/
--rw-rw-r--   0 asdougl   (1000) asdougl   (1000)      193 2023-03-08 20:37:55.000000 hauntedhouse-0.0.7/hauntedhouse.egg-info/PKG-INFO
--rw-rw-r--   0 asdougl   (1000) asdougl   (1000)      345 2023-03-08 20:37:55.000000 hauntedhouse-0.0.7/hauntedhouse.egg-info/SOURCES.txt
--rw-rw-r--   0 asdougl   (1000) asdougl   (1000)        1 2023-03-08 20:37:55.000000 hauntedhouse-0.0.7/hauntedhouse.egg-info/dependency_links.txt
--rw-rw-r--   0 asdougl   (1000) asdougl   (1000)       82 2023-03-08 20:37:55.000000 hauntedhouse-0.0.7/hauntedhouse.egg-info/requires.txt
--rw-rw-r--   0 asdougl   (1000) asdougl   (1000)       13 2023-03-08 20:37:55.000000 hauntedhouse-0.0.7/hauntedhouse.egg-info/top_level.txt
--rw-rw-r--   0 asdougl   (1000) asdougl   (1000)      496 2023-03-08 20:37:15.000000 hauntedhouse-0.0.7/pyproject.toml
--rw-rw-r--   0 asdougl   (1000) asdougl   (1000)        0 2023-02-09 19:03:43.000000 hauntedhouse-0.0.7/readme.md
--rw-rw-r--   0 asdougl   (1000) asdougl   (1000)       38 2023-03-08 20:37:55.127055 hauntedhouse-0.0.7/setup.cfg
-drwxrwxr-x   0 asdougl   (1000) asdougl   (1000)        0 2023-03-08 20:37:55.127055 hauntedhouse-0.0.7/tests/
--rw-rw-r--   0 asdougl   (1000) asdougl   (1000)      497 2023-02-09 19:03:43.000000 hauntedhouse-0.0.7/tests/test_yara_parse.py
+drwxrwxr-x   0 asdougl   (1000) asdougl   (1000)        0 2023-03-23 18:18:25.925197 hauntedhouse-0.0.9/
+-rw-rw-r--   0 asdougl   (1000) asdougl   (1000)      193 2023-03-23 18:18:25.925197 hauntedhouse-0.0.9/PKG-INFO
+drwxrwxr-x   0 asdougl   (1000) asdougl   (1000)        0 2023-03-23 18:18:25.921197 hauntedhouse-0.0.9/hauntedhouse/
+-rw-rw-r--   0 asdougl   (1000) asdougl   (1000)       40 2023-02-09 19:03:43.000000 hauntedhouse-0.0.9/hauntedhouse/__init__.py
+-rw-rw-r--   0 asdougl   (1000) asdougl   (1000)     8548 2023-03-23 18:16:32.000000 hauntedhouse-0.0.9/hauntedhouse/client.py
+-rw-rw-r--   0 asdougl   (1000) asdougl   (1000)     6639 2023-03-23 18:16:23.000000 hauntedhouse-0.0.9/hauntedhouse/ingest.py
+-rw-rw-r--   0 asdougl   (1000) asdougl   (1000)     1870 2023-03-23 18:15:58.000000 hauntedhouse-0.0.9/hauntedhouse/search.py
+-rw-rw-r--   0 asdougl   (1000) asdougl   (1000)      830 2023-03-23 18:15:58.000000 hauntedhouse-0.0.9/hauntedhouse/status.py
+drwxrwxr-x   0 asdougl   (1000) asdougl   (1000)        0 2023-03-23 18:18:25.925197 hauntedhouse-0.0.9/hauntedhouse.egg-info/
+-rw-rw-r--   0 asdougl   (1000) asdougl   (1000)      193 2023-03-23 18:18:25.000000 hauntedhouse-0.0.9/hauntedhouse.egg-info/PKG-INFO
+-rw-rw-r--   0 asdougl   (1000) asdougl   (1000)      345 2023-03-23 18:18:25.000000 hauntedhouse-0.0.9/hauntedhouse.egg-info/SOURCES.txt
+-rw-rw-r--   0 asdougl   (1000) asdougl   (1000)        1 2023-03-23 18:18:25.000000 hauntedhouse-0.0.9/hauntedhouse.egg-info/dependency_links.txt
+-rw-rw-r--   0 asdougl   (1000) asdougl   (1000)       82 2023-03-23 18:18:25.000000 hauntedhouse-0.0.9/hauntedhouse.egg-info/requires.txt
+-rw-rw-r--   0 asdougl   (1000) asdougl   (1000)       13 2023-03-23 18:18:25.000000 hauntedhouse-0.0.9/hauntedhouse.egg-info/top_level.txt
+-rw-rw-r--   0 asdougl   (1000) asdougl   (1000)      496 2023-03-23 18:16:49.000000 hauntedhouse-0.0.9/pyproject.toml
+-rw-rw-r--   0 asdougl   (1000) asdougl   (1000)        0 2023-02-09 19:03:43.000000 hauntedhouse-0.0.9/readme.md
+-rw-rw-r--   0 asdougl   (1000) asdougl   (1000)       38 2023-03-23 18:18:25.925197 hauntedhouse-0.0.9/setup.cfg
+drwxrwxr-x   0 asdougl   (1000) asdougl   (1000)        0 2023-03-23 18:18:25.925197 hauntedhouse-0.0.9/tests/
+-rw-rw-r--   0 asdougl   (1000) asdougl   (1000)      497 2023-02-09 19:03:43.000000 hauntedhouse-0.0.9/tests/test_yara_parse.py
```

### Comparing `hauntedhouse-0.0.7/hauntedhouse/client.py` & `hauntedhouse-0.0.9/hauntedhouse/client.py`

 * *Files identical despite different names*

### Comparing `hauntedhouse-0.0.7/hauntedhouse/ingest.py` & `hauntedhouse-0.0.9/hauntedhouse/ingest.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     batch_size: int = pydantic.Field(default=1000)
     allow_disabled_access: bool = pydantic.Field(default=False)
     trust_all: bool = pydantic.Field(default=False)
 
 
 async def socket_main(config: Config, verify: bool) -> None:
     logger.info("Connect to assemblyline for classification configuration")
-    al_client = get_client(config.assemblyline_url, apikey=(config.assemblyline_user, config.assemblyline_api_key))
+    al_client = get_client(config.assemblyline_url, apikey=(config.assemblyline_user, config.assemblyline_api_key), verify=verify)
     classification_definition = al_client._connection.get('api/v4/help/classification_definition')
 
     try:
         with open(os.path.join(config.write_path, "state.json"), 'r') as handle:
             data = json.load(handle)
             completed_seq_no = data['completed']
             last_seq_no = data['completed']
```

### Comparing `hauntedhouse-0.0.7/hauntedhouse/search.py` & `hauntedhouse-0.0.9/hauntedhouse/search.py`

 * *Files identical despite different names*

### Comparing `hauntedhouse-0.0.7/hauntedhouse/status.py` & `hauntedhouse-0.0.9/hauntedhouse/status.py`

 * *Files identical despite different names*

