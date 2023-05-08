# Comparing `tmp/secrets_cli-0.1.2.tar.gz` & `tmp/secrets_cli-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secrets_cli-0.1.2.tar", max compression
+gzip compressed data, was "secrets_cli-0.1.3.tar", max compression
```

## Comparing `secrets_cli-0.1.2.tar` & `secrets_cli-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      696 2023-05-08 14:45:25.398086 secrets_cli-0.1.2/Readme.md
--rw-r--r--   0        0        0      374 2023-05-08 15:03:19.209637 secrets_cli-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-08 13:41:06.609995 secrets_cli-0.1.2/secrets_cli/__init__.py
--rw-r--r--   0        0        0       32 2023-05-08 14:28:49.542556 secrets_cli-0.1.2/secrets_cli/requirements.txt
--rwxr-xr-x   0        0        0     5873 2023-05-08 15:01:49.834543 secrets_cli-0.1.2/secrets_cli/secrets_cli.py
--rw-r--r--   0        0        0     1266 1970-01-01 00:00:00.000000 secrets_cli-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      696 2023-05-08 14:45:25.398086 secrets_cli-0.1.3/Readme.md
+-rw-r--r--   0        0        0      374 2023-05-08 15:18:01.930461 secrets_cli-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-08 13:41:06.609995 secrets_cli-0.1.3/secrets_cli/__init__.py
+-rw-r--r--   0        0        0       32 2023-05-08 14:28:49.542556 secrets_cli-0.1.3/secrets_cli/requirements.txt
+-rwxr-xr-x   0        0        0     5887 2023-05-08 15:17:49.120729 secrets_cli-0.1.3/secrets_cli/secrets_cli.py
+-rw-r--r--   0        0        0     1266 1970-01-01 00:00:00.000000 secrets_cli-0.1.3/PKG-INFO
```

### Comparing `secrets_cli-0.1.2/Readme.md` & `secrets_cli-0.1.3/Readme.md`

 * *Files identical despite different names*

### Comparing `secrets_cli-0.1.2/secrets_cli/secrets_cli.py` & `secrets_cli-0.1.3/secrets_cli/secrets_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,15 +131,15 @@
         # Set the path
         if current_dir not in path_cache_json:
             logging.info("❌ No secrets loaded. Run `pangea select` to load secrets")
             raise typer.Exit(code=1)
 
         return path_cache_json[current_dir]
     else:
-        return os.getenv('PANGEA_SECRETS_DIR')
+        return f"/secrets/{os.getenv('PANGEA_SECRETS_DIR')}"
 
 @app.command()
 def run(
     command: List[str]
 ):
     # prepend environment secrets from pangea
     pangea_token = _get_pangea_token()
```

### Comparing `secrets_cli-0.1.2/PKG-INFO` & `secrets_cli-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secrets-cli
-Version: 0.1.2
+Version: 0.1.3
 Summary: Run any applications with secrets stored in the Pangea Vault
 Author: Pranav
 Requires-Python: >=3.7.2,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

