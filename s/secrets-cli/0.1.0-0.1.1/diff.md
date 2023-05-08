# Comparing `tmp/secrets_cli-0.1.0.tar.gz` & `tmp/secrets_cli-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secrets_cli-0.1.0.tar", max compression
+gzip compressed data, was "secrets_cli-0.1.1.tar", max compression
```

## Comparing `secrets_cli-0.1.0.tar` & `secrets_cli-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0      353 2023-05-08 13:42:58.828211 secrets_cli-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-08 13:41:06.609995 secrets_cli-0.1.0/secrets_cli/__init__.py
--rw-r--r--   0        0        0       32 2023-05-08 14:28:49.542556 secrets_cli-0.1.0/secrets_cli/requirements.txt
--rwxr-xr-x   0        0        0     5550 2023-05-08 14:34:08.758902 secrets_cli-0.1.0/secrets_cli/secrets_cli.py
--rw-r--r--   0        0        0      528 1970-01-01 00:00:00.000000 secrets_cli-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      696 2023-05-08 14:45:25.398086 secrets_cli-0.1.1/Readme.md
+-rw-r--r--   0        0        0      374 2023-05-08 14:46:03.751718 secrets_cli-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-08 13:41:06.609995 secrets_cli-0.1.1/secrets_cli/__init__.py
+-rw-r--r--   0        0        0       32 2023-05-08 14:28:49.542556 secrets_cli-0.1.1/secrets_cli/requirements.txt
+-rwxr-xr-x   0        0        0     5550 2023-05-08 14:34:08.758902 secrets_cli-0.1.1/secrets_cli/secrets_cli.py
+-rw-r--r--   0        0        0     1266 1970-01-01 00:00:00.000000 secrets_cli-0.1.1/PKG-INFO
```

### Comparing `secrets_cli-0.1.0/secrets_cli/secrets_cli.py` & `secrets_cli-0.1.1/secrets_cli/secrets_cli.py`

 * *Files identical despite different names*

