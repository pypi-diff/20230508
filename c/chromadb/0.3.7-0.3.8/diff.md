# Comparing `tmp/chromadb-0.3.7.tar.gz` & `tmp/chromadb-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chromadb-0.3.7.tar", last modified: Thu Feb 23 06:49:27 2023, max compression
+gzip compressed data, was "chromadb-0.3.8.tar", last modified: Sun Feb 26 00:17:14 2023, max compression
```

## Comparing `chromadb-0.3.7.tar` & `chromadb-0.3.8.tar`

### file list

```diff
@@ -1,79 +1,140 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 06:49:27.201084 chromadb-0.3.7/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-02-23 06:49:15.000000 chromadb-0.3.7/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 06:49:27.193085 chromadb-0.3.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 06:49:27.197085 chromadb-0.3.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-02-23 06:49:15.000000 chromadb-0.3.7/.github/workflows/chroma-release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-02-23 06:49:15.000000 chromadb-0.3.7/.github/workflows/chroma-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-02-23 06:49:15.000000 chromadb-0.3.7/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 06:49:27.197085 chromadb-0.3.7/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-02-23 06:49:15.000000 chromadb-0.3.7/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-02-23 06:49:15.000000 chromadb-0.3.7/DEVELOP.md
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-02-23 06:49:15.000000 chromadb-0.3.7/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-02-23 06:49:15.000000 chromadb-0.3.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-02-23 06:49:27.201084 chromadb-0.3.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-02-23 06:49:15.000000 chromadb-0.3.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 06:49:27.197085 chromadb-0.3.7/bin/
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-02-23 06:49:15.000000 chromadb-0.3.7/bin/backup.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      110 2023-02-23 06:49:15.000000 chromadb-0.3.7/bin/build
--rwxr-xr-x   0 runner    (1001) docker     (123)      206 2023-02-23 06:49:15.000000 chromadb-0.3.7/bin/docker_entrypoint.sh
--rw-r--r--   0 runner    (1001) docker     (123)     5313 2023-02-23 06:49:15.000000 chromadb-0.3.7/bin/generate_cloudformation.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      350 2023-02-23 06:49:15.000000 chromadb-0.3.7/bin/integration-test
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-02-23 06:49:15.000000 chromadb-0.3.7/bin/restore.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-02-23 06:49:15.000000 chromadb-0.3.7/bin/setup_linux.sh
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-02-23 06:49:15.000000 chromadb-0.3.7/bin/setup_mac.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 06:49:27.197085 chromadb-0.3.7/bin/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-02-23 06:49:15.000000 chromadb-0.3.7/bin/templates/docker-compose.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)      451 2023-02-23 06:49:15.000000 chromadb-0.3.7/bin/test-package.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      299 2023-02-23 06:49:15.000000 chromadb-0.3.7/bin/test-remote
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-02-23 06:49:15.000000 chromadb-0.3.7/bin/test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      150 2023-02-23 06:49:15.000000 chromadb-0.3.7/bin/version
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 06:49:27.201084 chromadb-0.3.7/chromadb/
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-02-23 06:49:15.000000 chromadb-0.3.7/chromadb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 06:49:27.201084 chromadb-0.3.7/chromadb/api/
--rw-r--r--   0 runner    (1001) docker     (123)     9266 2023-02-23 06:49:15.000000 chromadb-0.3.7/chromadb/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8514 2023-02-23 06:49:15.000000 chromadb-0.3.7/chromadb/api/fastapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     9403 2023-02-23 06:49:15.000000 chromadb-0.3.7/chromadb/api/local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 06:49:27.201084 chromadb-0.3.7/chromadb/api/models/
--rw-r--r--   0 runner    (1001) docker     (123)    12538 2023-02-23 06:49:15.000000 chromadb-0.3.7/chromadb/api/models/Collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     7719 2023-02-23 06:49:15.000000 chromadb-0.3.7/chromadb/api/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-02-23 06:49:15.000000 chromadb-0.3.7/chromadb/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-02-23 06:49:15.000000 chromadb-0.3.7/chromadb/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 06:49:27.201084 chromadb-0.3.7/chromadb/db/
--rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-02-23 06:49:15.000000 chromadb-0.3.7/chromadb/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19220 2023-02-23 06:49:15.000000 chromadb-0.3.7/chromadb/db/clickhouse.py
--rw-r--r--   0 runner    (1001) docker     (123)    16270 2023-02-23 06:49:15.000000 chromadb-0.3.7/chromadb/db/duckdb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 06:49:27.201084 chromadb-0.3.7/chromadb/db/index/
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-02-23 06:49:15.000000 chromadb-0.3.7/chromadb/db/index/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8444 2023-02-23 06:49:15.000000 chromadb-0.3.7/chromadb/db/index/hnswlib.py
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-02-23 06:49:15.000000 chromadb-0.3.7/chromadb/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-02-23 06:49:15.000000 chromadb-0.3.7/chromadb/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 06:49:27.201084 chromadb-0.3.7/chromadb/server/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-02-23 06:49:15.000000 chromadb-0.3.7/chromadb/server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 06:49:27.201084 chromadb-0.3.7/chromadb/server/fastapi/
--rw-r--r--   0 runner    (1001) docker     (123)     6350 2023-02-23 06:49:15.000000 chromadb-0.3.7/chromadb/server/fastapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-02-23 06:49:15.000000 chromadb-0.3.7/chromadb/server/fastapi/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 06:49:27.201084 chromadb-0.3.7/chromadb/test/
--rw-r--r--   0 runner    (1001) docker     (123)    35016 2023-02-23 06:49:15.000000 chromadb-0.3.7/chromadb/test/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-02-23 06:49:15.000000 chromadb-0.3.7/chromadb/test/test_chroma.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 06:49:27.201084 chromadb-0.3.7/chromadb/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 06:49:15.000000 chromadb-0.3.7/chromadb/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-02-23 06:49:15.000000 chromadb-0.3.7/chromadb/utils/embedding_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 06:49:27.201084 chromadb-0.3.7/chromadb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-02-23 06:49:27.000000 chromadb-0.3.7/chromadb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-02-23 06:49:27.000000 chromadb-0.3.7/chromadb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-23 06:49:27.000000 chromadb-0.3.7/chromadb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-02-23 06:49:27.000000 chromadb-0.3.7/chromadb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-23 06:49:27.000000 chromadb-0.3.7/chromadb.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 06:49:27.201084 chromadb-0.3.7/config/
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-02-23 06:49:15.000000 chromadb-0.3.7/config/backup_disk.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-02-23 06:49:15.000000 chromadb-0.3.7/docker-compose.test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-02-23 06:49:15.000000 chromadb-0.3.7/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 06:49:27.201084 chromadb-0.3.7/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     5830 2023-02-23 06:49:15.000000 chromadb-0.3.7/examples/local_persistence.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-02-23 06:49:15.000000 chromadb-0.3.7/examples/where_filtering.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-02-23 06:49:15.000000 chromadb-0.3.7/new_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-02-23 06:49:15.000000 chromadb-0.3.7/pull_request_template.md
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-02-23 06:49:15.000000 chromadb-0.3.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-02-23 06:49:15.000000 chromadb-0.3.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-02-23 06:49:15.000000 chromadb-0.3.7/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-23 06:49:27.201084 chromadb-0.3.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 00:17:14.590613 chromadb-0.3.8/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-02-26 00:16:59.000000 chromadb-0.3.8/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 00:17:14.574612 chromadb-0.3.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 00:17:14.578613 chromadb-0.3.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-02-26 00:16:59.000000 chromadb-0.3.8/.github/workflows/chroma-release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-02-26 00:16:59.000000 chromadb-0.3.8/.github/workflows/chroma-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-02-26 00:16:59.000000 chromadb-0.3.8/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 00:17:14.578613 chromadb-0.3.8/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-02-26 00:16:59.000000 chromadb-0.3.8/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-02-26 00:16:59.000000 chromadb-0.3.8/DEVELOP.md
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-02-26 00:16:59.000000 chromadb-0.3.8/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-02-26 00:16:59.000000 chromadb-0.3.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-02-26 00:17:14.590613 chromadb-0.3.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-02-26 00:16:59.000000 chromadb-0.3.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 00:17:14.578613 chromadb-0.3.8/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-02-26 00:16:59.000000 chromadb-0.3.8/bin/backup.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      110 2023-02-26 00:16:59.000000 chromadb-0.3.8/bin/build
+-rwxr-xr-x   0 runner    (1001) docker     (123)      206 2023-02-26 00:16:59.000000 chromadb-0.3.8/bin/docker_entrypoint.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     5623 2023-02-26 00:16:59.000000 chromadb-0.3.8/bin/generate_cloudformation.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      350 2023-02-26 00:16:59.000000 chromadb-0.3.8/bin/integration-test
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-02-26 00:16:59.000000 chromadb-0.3.8/bin/restore.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-02-26 00:16:59.000000 chromadb-0.3.8/bin/setup_linux.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-02-26 00:16:59.000000 chromadb-0.3.8/bin/setup_mac.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 00:17:14.578613 chromadb-0.3.8/bin/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-02-26 00:16:59.000000 chromadb-0.3.8/bin/templates/docker-compose.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      451 2023-02-26 00:16:59.000000 chromadb-0.3.8/bin/test-package.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      299 2023-02-26 00:16:59.000000 chromadb-0.3.8/bin/test-remote
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-02-26 00:16:59.000000 chromadb-0.3.8/bin/test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      150 2023-02-26 00:16:59.000000 chromadb-0.3.8/bin/version
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 00:17:14.578613 chromadb-0.3.8/chromadb/
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-02-26 00:16:59.000000 chromadb-0.3.8/chromadb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 00:17:14.582613 chromadb-0.3.8/chromadb/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     9796 2023-02-26 00:16:59.000000 chromadb-0.3.8/chromadb/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8667 2023-02-26 00:16:59.000000 chromadb-0.3.8/chromadb/api/fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9788 2023-02-26 00:16:59.000000 chromadb-0.3.8/chromadb/api/local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 00:17:14.582613 chromadb-0.3.8/chromadb/api/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    12538 2023-02-26 00:16:59.000000 chromadb-0.3.8/chromadb/api/models/Collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7719 2023-02-26 00:16:59.000000 chromadb-0.3.8/chromadb/api/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-02-26 00:16:59.000000 chromadb-0.3.8/chromadb/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-02-26 00:16:59.000000 chromadb-0.3.8/chromadb/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 00:17:14.582613 chromadb-0.3.8/chromadb/db/
+-rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-02-26 00:16:59.000000 chromadb-0.3.8/chromadb/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19923 2023-02-26 00:16:59.000000 chromadb-0.3.8/chromadb/db/clickhouse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16413 2023-02-26 00:16:59.000000 chromadb-0.3.8/chromadb/db/duckdb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 00:17:14.582613 chromadb-0.3.8/chromadb/db/index/
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-02-26 00:16:59.000000 chromadb-0.3.8/chromadb/db/index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8444 2023-02-26 00:16:59.000000 chromadb-0.3.8/chromadb/db/index/hnswlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-02-26 00:16:59.000000 chromadb-0.3.8/chromadb/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-02-26 00:16:59.000000 chromadb-0.3.8/chromadb/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 00:17:14.582613 chromadb-0.3.8/chromadb/server/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-02-26 00:16:59.000000 chromadb-0.3.8/chromadb/server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 00:17:14.582613 chromadb-0.3.8/chromadb/server/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (123)     7468 2023-02-26 00:16:59.000000 chromadb-0.3.8/chromadb/server/fastapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-02-26 00:16:59.000000 chromadb-0.3.8/chromadb/server/fastapi/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 00:17:14.582613 chromadb-0.3.8/chromadb/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    35183 2023-02-26 00:16:59.000000 chromadb-0.3.8/chromadb/test/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-02-26 00:16:59.000000 chromadb-0.3.8/chromadb/test/test_chroma.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 00:17:14.582613 chromadb-0.3.8/chromadb/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-26 00:16:59.000000 chromadb-0.3.8/chromadb/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-02-26 00:16:59.000000 chromadb-0.3.8/chromadb/utils/embedding_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 00:17:14.578613 chromadb-0.3.8/chromadb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-02-26 00:17:14.000000 chromadb-0.3.8/chromadb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-02-26 00:17:14.000000 chromadb-0.3.8/chromadb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-26 00:17:14.000000 chromadb-0.3.8/chromadb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-02-26 00:17:14.000000 chromadb-0.3.8/chromadb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-26 00:17:14.000000 chromadb-0.3.8/chromadb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 00:17:14.574612 chromadb-0.3.8/clients/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 00:17:14.586613 chromadb-0.3.8/clients/js/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-02-26 00:16:59.000000 chromadb-0.3.8/clients/js/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-02-26 00:16:59.000000 chromadb-0.3.8/clients/js/DEVELOP.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-02-26 00:16:59.000000 chromadb-0.3.8/clients/js/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-02-26 00:16:59.000000 chromadb-0.3.8/clients/js/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 00:17:14.574612 chromadb-0.3.8/clients/js/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 00:17:14.586613 chromadb-0.3.8/clients/js/examples/browser/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-26 00:16:59.000000 chromadb-0.3.8/clients/js/examples/browser/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-02-26 00:16:59.000000 chromadb-0.3.8/clients/js/examples/browser/app.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-02-26 00:16:59.000000 chromadb-0.3.8/clients/js/examples/browser/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-02-26 00:16:59.000000 chromadb-0.3.8/clients/js/examples/browser/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)    71072 2023-02-26 00:16:59.000000 chromadb-0.3.8/clients/js/examples/browser/yarn.lock
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 00:17:14.586613 chromadb-0.3.8/clients/js/examples/node/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-02-26 00:16:59.000000 chromadb-0.3.8/clients/js/examples/node/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-02-26 00:16:59.000000 chromadb-0.3.8/clients/js/examples/node/app.js
+-rw-r--r--   0 runner    (1001) docker     (123)    46542 2023-02-26 00:16:59.000000 chromadb-0.3.8/clients/js/examples/node/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-02-26 00:16:59.000000 chromadb-0.3.8/clients/js/examples/node/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)    17116 2023-02-26 00:16:59.000000 chromadb-0.3.8/clients/js/examples/node/yarn.lock
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-02-26 00:16:59.000000 chromadb-0.3.8/clients/js/jest.config.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-02-26 00:16:59.000000 chromadb-0.3.8/clients/js/openapitools.json
+-rw-r--r--   0 runner    (1001) docker     (123)   450648 2023-02-26 00:16:59.000000 chromadb-0.3.8/clients/js/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-02-26 00:16:59.000000 chromadb-0.3.8/clients/js/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 00:17:14.586613 chromadb-0.3.8/clients/js/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 00:17:14.586613 chromadb-0.3.8/clients/js/src/generated/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-02-26 00:16:59.000000 chromadb-0.3.8/clients/js/src/generated/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-02-26 00:16:59.000000 chromadb-0.3.8/clients/js/src/generated/.npmignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 00:17:14.586613 chromadb-0.3.8/clients/js/src/generated/.openapi-generator/
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-02-26 00:16:59.000000 chromadb-0.3.8/clients/js/src/generated/.openapi-generator/FILES
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-26 00:16:59.000000 chromadb-0.3.8/clients/js/src/generated/.openapi-generator/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-02-26 00:16:59.000000 chromadb-0.3.8/clients/js/src/generated/.openapi-generator-ignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-02-26 00:16:59.000000 chromadb-0.3.8/clients/js/src/generated/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 00:17:14.586613 chromadb-0.3.8/clients/js/src/generated/api/
+-rw-r--r--   0 runner    (1001) docker     (123)    57676 2023-02-26 00:16:59.000000 chromadb-0.3.8/clients/js/src/generated/api/default-api.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-02-26 00:16:59.000000 chromadb-0.3.8/clients/js/src/generated/api.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-02-26 00:16:59.000000 chromadb-0.3.8/clients/js/src/generated/base.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-02-26 00:16:59.000000 chromadb-0.3.8/clients/js/src/generated/common.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-02-26 00:16:59.000000 chromadb-0.3.8/clients/js/src/generated/configuration.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-02-26 00:16:59.000000 chromadb-0.3.8/clients/js/src/generated/git_push.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-02-26 00:16:59.000000 chromadb-0.3.8/clients/js/src/generated/index.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 00:17:14.590613 chromadb-0.3.8/clients/js/src/generated/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-02-26 00:16:59.000000 chromadb-0.3.8/clients/js/src/generated/models/add-embedding.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-02-26 00:16:59.000000 chromadb-0.3.8/clients/js/src/generated/models/create-collection.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-02-26 00:16:59.000000 chromadb-0.3.8/clients/js/src/generated/models/delete-embedding.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-02-26 00:16:59.000000 chromadb-0.3.8/clients/js/src/generated/models/get-embedding.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-02-26 00:16:59.000000 chromadb-0.3.8/clients/js/src/generated/models/httpvalidation-error.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-02-26 00:16:59.000000 chromadb-0.3.8/clients/js/src/generated/models/index.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-02-26 00:16:59.000000 chromadb-0.3.8/clients/js/src/generated/models/query-embedding.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-02-26 00:16:59.000000 chromadb-0.3.8/clients/js/src/generated/models/raw-sql.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-02-26 00:16:59.000000 chromadb-0.3.8/clients/js/src/generated/models/update-collection.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-02-26 00:16:59.000000 chromadb-0.3.8/clients/js/src/generated/models/update-embedding.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-02-26 00:16:59.000000 chromadb-0.3.8/clients/js/src/generated/models/validation-error.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-02-26 00:16:59.000000 chromadb-0.3.8/clients/js/src/generated/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-02-26 00:16:59.000000 chromadb-0.3.8/clients/js/src/generated/tsconfig.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8884 2023-02-26 00:16:59.000000 chromadb-0.3.8/clients/js/src/index.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 00:17:14.590613 chromadb-0.3.8/clients/js/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     7559 2023-02-26 00:16:59.000000 chromadb-0.3.8/clients/js/test/client.test.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-02-26 00:16:59.000000 chromadb-0.3.8/clients/js/tsconfig.json
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-02-26 00:16:59.000000 chromadb-0.3.8/clients/js/tsconfig.module.json
+-rw-r--r--   0 runner    (1001) docker     (123)   145670 2023-02-26 00:16:59.000000 chromadb-0.3.8/clients/js/yarn.lock
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 00:17:14.590613 chromadb-0.3.8/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-02-26 00:16:59.000000 chromadb-0.3.8/config/backup_disk.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-02-26 00:16:59.000000 chromadb-0.3.8/docker-compose-js-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-02-26 00:16:59.000000 chromadb-0.3.8/docker-compose.test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-02-26 00:16:59.000000 chromadb-0.3.8/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 00:17:14.590613 chromadb-0.3.8/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     5830 2023-02-26 00:16:59.000000 chromadb-0.3.8/examples/local_persistence.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-02-26 00:16:59.000000 chromadb-0.3.8/examples/where_filtering.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     9872 2023-02-26 00:16:59.000000 chromadb-0.3.8/new_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-02-26 00:16:59.000000 chromadb-0.3.8/pull_request_template.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-02-26 00:16:59.000000 chromadb-0.3.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-02-26 00:16:59.000000 chromadb-0.3.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-02-26 00:16:59.000000 chromadb-0.3.8/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-26 00:17:14.590613 chromadb-0.3.8/setup.cfg
```

### Comparing `chromadb-0.3.7/.github/workflows/chroma-release.yml` & `chromadb-0.3.8/.github/workflows/chroma-release.yml`

 * *Files identical despite different names*

### Comparing `chromadb-0.3.7/.github/workflows/chroma-test.yml` & `chromadb-0.3.8/.github/workflows/chroma-test.yml`

 * *Files identical despite different names*

### Comparing `chromadb-0.3.7/DEVELOP.md` & `chromadb-0.3.8/DEVELOP.md`

 * *Files 6% similar despite different names*

```diff
@@ -30,20 +30,20 @@
 
 2. Standaline and in-memory with persistance:
 
 This by default saves your db and your indexes to a `.chroma` directory and can also load from them. 
 ```python
 import chromadb
 from chromadb.config import Settings
-api = chromadb.Client(Settings(chroma_db_impl="duckdb+parquet"))
+api = chromadb.Client(Settings(chroma_db_impl="duckdb+parquet", 
+                      persist_directory="/path/to/persist/directory"))
 print(api.heartbeat())
 ```
 
 
-
 3. With a persistent backend and a small frontend client
 
 Run `docker-compose up -d --build`
 ```python
 import chromadb
 from chromadb.config import Settings
 api = chromadb.Client(Settings(chroma_api_impl="rest",
```

### Comparing `chromadb-0.3.7/LICENSE` & `chromadb-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `chromadb-0.3.7/PKG-INFO` & `chromadb-0.3.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chromadb
-Version: 0.3.7
+Version: 0.3.8
 Summary: Chroma.
 Author-email: Jeff Huber <jeff@trychroma.com>, Anton Troynikov <anton@trychroma.com>
 Project-URL: Homepage, https://github.com/chroma-core/chroma
 Project-URL: Bug Tracker, https://github.com/chroma-core/chroma/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -20,25 +20,29 @@
 __Chroma is the open-source embedding database__. Chroma makes it easy to build LLM apps by making knowledge, facts, and skills pluggable for LLMs. 
 
 - [💬 Community Discord](https://discord.gg/MMeYNTmh3x)
 - [📖 Documentation](https://docs.trychroma.com/)
 - [💡 Colab Example](https://colab.research.google.com/drive/1QEzFyqnoFxq7LUGyP1vzR4iLt9PpCDXv?usp=sharing)
 - [🏠 Homepage](https://www.trychroma.com/)
 
+Language Support
+- `python` - `pip install chromadb`
+- `javascript/typescript` - `npm install --save chromadb`
+
 ## ChatGPT for ______
 
 For example, the `"Chat your data"` use case:
 1. Add documents to your database. You can pass in your own embeddings, embedding function, or let Chroma embed them for you.
 2. Query relevant documents with natural language.
 3. Compose documents into the context window of an LLM like `GPT3` for additional summarization or analysis. 
 
 
 ## Features
 - __Simple__: Fully-typed, fully-tested, fully-documented == happiness
-- __Integrations__: `🦜️🔗 LangChain` and more soon
+- __Integrations__: `🦜️🔗 LangChain` (python and js), `🦙 gpt-index/LlamaIndex` and more soon
 - __Dev, Test, Prod__: the same API that runs in your python notebook, scales to your cluster
 - __Feature-rich__: Queries, filtering, density estimation and more
 - __Free__: Apache 2.0 Licensed
 
 ## Get up and running
 ```python
 pip install chromadb
```

### Comparing `chromadb-0.3.7/README.md` & `chromadb-0.3.8/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -6,25 +6,29 @@
 __Chroma is the open-source embedding database__. Chroma makes it easy to build LLM apps by making knowledge, facts, and skills pluggable for LLMs. 
 
 - [💬 Community Discord](https://discord.gg/MMeYNTmh3x)
 - [📖 Documentation](https://docs.trychroma.com/)
 - [💡 Colab Example](https://colab.research.google.com/drive/1QEzFyqnoFxq7LUGyP1vzR4iLt9PpCDXv?usp=sharing)
 - [🏠 Homepage](https://www.trychroma.com/)
 
+Language Support
+- `python` - `pip install chromadb`
+- `javascript/typescript` - `npm install --save chromadb`
+
 ## ChatGPT for ______
 
 For example, the `"Chat your data"` use case:
 1. Add documents to your database. You can pass in your own embeddings, embedding function, or let Chroma embed them for you.
 2. Query relevant documents with natural language.
 3. Compose documents into the context window of an LLM like `GPT3` for additional summarization or analysis. 
 
 
 ## Features
 - __Simple__: Fully-typed, fully-tested, fully-documented == happiness
-- __Integrations__: `🦜️🔗 LangChain` and more soon
+- __Integrations__: `🦜️🔗 LangChain` (python and js), `🦙 gpt-index/LlamaIndex` and more soon
 - __Dev, Test, Prod__: the same API that runs in your python notebook, scales to your cluster
 - __Feature-rich__: Queries, filtering, density estimation and more
 - __Free__: Apache 2.0 Licensed
 
 ## Get up and running
 ```python
 pip install chromadb
```

### Comparing `chromadb-0.3.7/bin/backup.sh` & `chromadb-0.3.8/bin/backup.sh`

 * *Files identical despite different names*

### Comparing `chromadb-0.3.7/bin/generate_cloudformation.py` & `chromadb-0.3.8/bin/generate_cloudformation.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 import boto3
 import json
 import subprocess
 import os
+import re
 
 def b64text(txt):
     """Generate Base 64 encoded CF json for a multiline string, subbing in values where appropriate"""
     lines = []
     for line in txt.splitlines(True):
         if "${" in line:
             lines.append({"Fn::Sub": line})
         else:
             lines.append(line)
     return {"Fn::Base64": {"Fn::Join": ["", lines]}}
 
+
 path = os.path.dirname(os.path.realpath(__file__))
-version = subprocess.check_output(f'{path}/version').decode('ascii').strip()
+version = subprocess.check_output(f"{path}/version").decode("ascii").strip()
 
 with open(f"{path}/templates/docker-compose.yml") as f:
     docker_compose_file = str(f.read())
 
 cloud_config_script = f"""
 #cloud-config
 cloud_final_modules:
@@ -67,86 +69,103 @@
     "AWSTemplateFormatVersion": "2010-09-09",
     "Description": "Create a stack that runs Chroma hosted on a single instance",
     "Parameters": {
         "KeyName": {
             "Description": "Name of an existing EC2 KeyPair to enable SSH access to the instance",
             "Type": "String",
             "ConstraintDescription": "If present, must be the name of an existing EC2 KeyPair.",
-            "Default": ""
+            "Default": "",
         },
         "InstanceType": {
             "Description": "EC2 instance type",
             "Type": "String",
-            "Default": "t3.small"
-        },
-        "Region": {
-            "Description": "AWS Region",
-            "Type": "String",
-            "Default": "us-east-1"
+            "Default": "t3.small",
         },
         "ChromaVersion": {
             "Description": "Chroma version to install",
             "Type": "String",
-            "Default": version
-        }
+            "Default": version,
+        },
     },
     "Conditions": {
         "HasKeyName": {"Fn::Not": [{"Fn::Equals": [{"Ref": "KeyName"}, ""]}]},
     },
     "Resources": {
         "ChromaInstance": {
             "Type": "AWS::EC2::Instance",
             "Properties": {
-                "ImageId": {"Fn::FindInMap": ["Region2AMI", {"Ref": "Region"}, "AMI"]},
+                "ImageId": {"Fn::FindInMap": ["Region2AMI", {"Ref": "AWS::Region"}, "AMI"]},
                 "InstanceType": {"Ref": "InstanceType"},
                 "UserData": b64text(userdata),
                 "SecurityGroupIds": [{"Ref": "ChromaInstanceSecurityGroup"}],
                 "KeyName": {"Fn::If": ["HasKeyName", {"Ref": "KeyName"}, {"Ref": "AWS::NoValue"}]},
-                "BlockDeviceMappings": [{
-                    "DeviceName":  {"Fn::FindInMap": ["Region2AMI", {"Ref": "Region"}, "RootDeviceName"]},
-                    "Ebs": {
-                        "VolumeSize": 24
-                     }
-                }]
+                "BlockDeviceMappings": [
+                    {
+                        "DeviceName": {
+                            "Fn::FindInMap": ["Region2AMI", {"Ref": "AWS::Region"}, "RootDeviceName"]
+                        },
+                        "Ebs": {"VolumeSize": 24},
+                    }
+                ],
             },
         },
         "ChromaInstanceSecurityGroup": {
             "Type": "AWS::EC2::SecurityGroup",
             "Properties": {
                 "GroupDescription": "Chroma Instance Security Group",
                 "SecurityGroupIngress": [
                     {"IpProtocol": "tcp", "FromPort": "22", "ToPort": "22", "CidrIp": "0.0.0.0/0"},
-                    {"IpProtocol": "tcp", "FromPort": "8000", "ToPort": "8000", "CidrIp": "0.0.0.0/0"}
-                ]
-            }
+                    {
+                        "IpProtocol": "tcp",
+                        "FromPort": "8000",
+                        "ToPort": "8000",
+                        "CidrIp": "0.0.0.0/0",
+                    },
+                ],
+            },
+        },
+    },
+    "Outputs": {
+        "ServerIp": {
+            "Description": "IP address of the Chroma server",
+            "Value": {"Fn::GetAtt": ["ChromaInstance", "PublicIp"]},
         }
     },
-    "Outputs": {"ServerIp": {
-        "Description": "IP address of the Chroma server",
-        "Value": {"Fn::GetAtt": ["ChromaInstance", "PublicIp"]}
-    }},
-    "Mappings": {"Region2AMI": {}}
+    "Mappings": {"Region2AMI": {}},
 }
 
 # Populate the Region2AMI mappings
-regions = boto3.client('ec2', region_name='us-east-1').describe_regions()['Regions']
+regions = boto3.client("ec2", region_name="us-east-1").describe_regions()["Regions"]
 for region in regions:
-    region_name = region['RegionName']
-    ami_result = boto3.client('ec2', region_name=region_name).describe_images(
-        Owners=['137112412989'],
-        Filters=[{'Name': 'name', 'Values': ['amzn2-ami-kernel-5.10-hvm-*-x86_64-gp2']},
-                 {'Name': 'root-device-type', 'Values': ['ebs']},
-                 {'Name': 'virtualization-type', 'Values': ['hvm']}])
-    img = ami_result['Images'][0]
-    ami_id = img['ImageId']
-    root_device_name = img['BlockDeviceMappings'][0]['DeviceName']
-    cf['Mappings']['Region2AMI'][region_name] = {"AMI": ami_id,
-                                                 "RootDeviceName": root_device_name}
+    region_name = region["RegionName"]
+    ami_result = boto3.client("ec2", region_name=region_name).describe_images(
+        Owners=["137112412989"],
+        Filters=[
+            {"Name": "name", "Values": ["amzn2-ami-kernel-5.10-hvm-*-x86_64-gp2"]},
+            {"Name": "root-device-type", "Values": ["ebs"]},
+            {"Name": "virtualization-type", "Values": ["hvm"]},
+        ],
+    )
+    img = ami_result["Images"][0]
+    ami_id = img["ImageId"]
+    root_device_name = img["BlockDeviceMappings"][0]["DeviceName"]
+    cf["Mappings"]["Region2AMI"][region_name] = {"AMI": ami_id, "RootDeviceName": root_device_name}
 
 
 # Write the CF json to a file
-json.dump(cf, open('/tmp/chroma.cf.json', 'w'), indent=4)
+json.dump(cf, open("/tmp/chroma.cf.json", "w"), indent=4)
 
 # upload to S3
-s3 = boto3.client('s3', region_name='us-east-1')
-s3.upload_file('/tmp/chroma.cf.json', 'public.trychroma.com', f'cloudformation/{version}/chroma.cf.json')
-s3.upload_file('/tmp/chroma.cf.json', 'public.trychroma.com', f'cloudformation/latest/chroma.cf.json')
+s3 = boto3.client("s3", region_name="us-east-1")
+s3.upload_file(
+    "/tmp/chroma.cf.json", "public.trychroma.com", f"cloudformation/{version}/chroma.cf.json"
+)
+
+# Upload to s3 under /latest version only if this is a release
+pattern = re.compile(r"^\d+\.\d+\.\d+$")
+if pattern.match(version):
+    s3.upload_file(
+        "/tmp/chroma.cf.json", "public.trychroma.com", "cloudformation/latest/chroma.cf.json"
+    )
+else:
+    print(f"Version {version} is not a 3-part semver, not uploading to /latest")
+
```

### Comparing `chromadb-0.3.7/bin/restore.sh` & `chromadb-0.3.8/bin/restore.sh`

 * *Files identical despite different names*

### Comparing `chromadb-0.3.7/bin/setup_linux.sh` & `chromadb-0.3.8/bin/setup_linux.sh`

 * *Files identical despite different names*

### Comparing `chromadb-0.3.7/bin/templates/docker-compose.yml` & `chromadb-0.3.8/bin/templates/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `chromadb-0.3.7/chromadb/__init__.py` & `chromadb-0.3.8/chromadb/__init__.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.3.7/chromadb/api/__init__.py` & `chromadb-0.3.8/chromadb/api/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,14 +67,25 @@
         Returns:
             dict: the created collection
 
         """
         pass
 
     @abstractmethod
+    def delete_collection(
+        self,
+        name: str,
+    ):
+        """Deletes a collection from the database
+
+        Args:
+            name (str): The name of the collection to delete
+        """
+
+    @abstractmethod
     def get_or_create_collection(self, name: str, metadata: Optional[Dict] = None) -> Collection:
         """Calls create_collection with get_or_create=True
 
         Args:
             name (str): The name of the collection to create. The name must be unique.
             metadata (Optional[Dict], optional): A dictionary of metadata to associate with the collection. Defaults to None.
         Returns:
@@ -103,14 +114,21 @@
 
     def _modify(
         self,
         current_name: str,
         new_name: Optional[str] = None,
         new_metadata: Optional[Dict] = None,
     ):
+        """Modify a collection in the database - can update the name and/or metadata
+
+        Args:
+            current_name (str): The name of the collection to modify
+            new_name (Optional[str], optional): The new name of the collection. Defaults to None.
+            new_metadata (Optional[Dict], optional): The new metadata to associate with the collection. Defaults to None.
+        """
         pass
 
     @abstractmethod
     def _add(
         self,
         ids: IDs,
         collection_name: Union[str, Sequence[str]],
@@ -146,22 +164,22 @@
         Args:
             collection_name (Union[str, Sequence[str]]): The model space(s) to add the embeddings to
             embedding (Sequence[Sequence[float]]): The sequence of embeddings to add
         """
         pass
 
     @abstractmethod
-    def _count(self, collection_name: Optional[str] = None) -> int:
+    def _count(self, collection_name: str) -> int:
         """Returns the number of embeddings in the database
 
         Args:
-            collection_name (Optional[str], optional): The model space to count the embeddings in. If None (default), returns the total count of all embeddings.
+            collection_name (str): The model space to count the embeddings in.
 
         Returns:
-            int: The number of embeddings in the database
+            int: The number of embeddings in the collection
 
         """
         pass
 
     @abstractmethod
     def _peek(self, collection_name: str, n: int = 10) -> GetResult:
         pass
```

### Comparing `chromadb-0.3.7/chromadb/api/fastapi.py` & `chromadb-0.3.8/chromadb/api/fastapi.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 from chromadb.api import API
 from chromadb.api.types import (
     Documents,
     Embeddings,
     IDs,
     Include,
     Metadatas,
+    Where,
+    WhereDocument,
 )
 from chromadb.errors import NoDatapointsException
 import pandas as pd
 import requests
 import json
 from typing import Sequence
 from chromadb.api.models.Collection import Collection
@@ -43,15 +45,16 @@
         name: str,
         metadata: Optional[Dict] = None,
         embedding_function: Optional[Callable] = None,
         get_or_create: bool = False,
     ) -> Collection:
         """Creates a collection"""
         resp = requests.post(
-            self._api_url + "/collections", data=json.dumps({"name": name, "metadata": metadata, "get_or_create": get_or_create})
+            self._api_url + "/collections",
+            data=json.dumps({"name": name, "metadata": metadata, "get_or_create": get_or_create}),
         )
         resp.raise_for_status()
         return Collection(client=self, name=name, embedding_function=embedding_function)
 
     def get_collection(
         self,
         name: str,
@@ -65,52 +68,51 @@
     def get_or_create_collection(
         self,
         name: str,
         metadata: Optional[Dict] = None,
         embedding_function: Optional[Callable] = None,
     ) -> Collection:
         """Get a collection, or return it if it exists"""
-        
+
         return self.create_collection(name, metadata, embedding_function, get_or_create=True)
 
-    def modify(self, current_name, new_name: str, new_metadata: Optional[Dict] = None) -> int:
+    def _modify(self, current_name: str, new_name: str, new_metadata: Optional[Dict] = None):
         """Updates a collection"""
         resp = requests.put(
             self._api_url + "/collections/" + current_name,
             data=json.dumps({"metadata": new_metadata, "name": new_name}),
         )
         resp.raise_for_status()
         return resp.json()
 
-    def delete_collection(self, name: str) -> int:
+    def delete_collection(self, name: str):
         """Deletes a collection"""
         resp = requests.delete(self._api_url + "/collections/" + name)
         resp.raise_for_status()
-        return resp.json()
 
     def _count(self, collection_name: str):
         """Returns the number of embeddings in the database"""
         resp = requests.get(self._api_url + "/collections/" + collection_name + "/count")
         resp.raise_for_status()
         return resp.json()
 
     def _peek(self, collection_name, limit=10):
         return self._get(collection_name, limit=limit)
 
     def _get(
         self,
-        collection_name,
-        ids=None,
-        where={},
-        sort=None,
-        limit=None,
-        offset=None,
-        page=None,
-        page_size=None,
-        where_document={},
+        collection_name: str,
+        ids: Optional[IDs] = None,
+        where: Optional[Where] = {},
+        sort: Optional[str] = None,
+        limit: Optional[int] = None,
+        offset: Optional[int] = None,
+        page: Optional[int] = None,
+        page_size: Optional[int] = None,
+        where_document: Optional[WhereDocument] = {},
         include: Include = ["embeddings", "metadatas", "documents"],
     ):
         """Gets embeddings from the database"""
         if page and page_size:
             offset = (page - 1) * page_size
             limit = page_size
```

### Comparing `chromadb-0.3.7/chromadb/api/local.py` & `chromadb-0.3.8/chromadb/api/local.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,25 @@
 import json
 import uuid
 import time
 from typing import Dict, List, Optional, Sequence, Callable, Type, cast
 from chromadb.api import API
 from chromadb.db import DB
-from chromadb.api.types import Embedding, GetResult, IDs, Include, QueryResult
+from chromadb.api.types import (
+    Documents,
+    Embedding,
+    Embeddings,
+    GetResult,
+    IDs,
+    Include,
+    Metadatas,
+    QueryResult,
+    Where,
+    WhereDocument,
+)
 from chromadb.api.models.Collection import Collection
 
 import re
 
 
 # mimics s3 bucket requirements for naming
 def is_valid_index_name(index_name):
@@ -34,15 +45,15 @@
     # COLLECTION METHODS
     #
     def create_collection(
         self,
         name: str,
         metadata: Optional[Dict] = None,
         embedding_function: Optional[Callable] = None,
-        get_or_create: bool = False
+        get_or_create: bool = False,
     ) -> Collection:
         if not is_valid_index_name(name):
             raise ValueError("Invalid index name: %s" % name)  # NIT: tell the user why
 
         self._db.create_collection(name, metadata, get_or_create)
         return Collection(client=self, name=name, embedding_function=embedding_function)
 
@@ -55,55 +66,55 @@
         return self.create_collection(name, metadata, embedding_function, get_or_create=True)
 
     def get_collection(
         self,
         name: str,
         embedding_function: Optional[Callable] = None,
     ) -> Collection:
-        self._db.get_collection(name)
+        res = self._db.get_collection(name)
+        if len(res) == 0:
+            raise ValueError("Collection not found: %s" % name)
         return Collection(client=self, name=name, embedding_function=embedding_function)
 
-    def _get_collection_db(self, name: str) -> int:
-        return self._db.get_collection(name)
-
     def list_collections(self) -> Sequence[Collection]:
         collections = []
         db_collections = self._db.list_collections()
         for db_collection in db_collections:
             collections.append(Collection(client=self, name=db_collection[1]))
         return collections
 
-    def modify(
+    def _modify(
         self,
         current_name: str,
         new_name: Optional[str] = None,
         new_metadata: Optional[Dict] = None,
     ):
         # NIT: make sure we have a valid name like we do in create
         if new_name is not None:
             if not is_valid_index_name(new_name):
                 raise ValueError("Invalid index name: %s" % new_name)
 
         self._db.update_collection(current_name, new_name, new_metadata)
 
-    def delete_collection(self, name: str) -> int:
+    def delete_collection(self, name: str):
         return self._db.delete_collection(name)
 
     #
     # ITEM METHODS
     #
     def _add(
         self,
         ids,
         collection_name: str,
-        embeddings,
-        metadatas=None,
-        documents=None,
-        increment_index=True,
+        embeddings: Embeddings,
+        metadatas: Optional[Metadatas] = None,
+        documents: Optional[Documents] = None,
+        increment_index: bool = True,
     ):
+
         collection_uuid = self._db.get_collection_uuid_from_name(collection_name)
         added_uuids = self._db.add(
             collection_uuid,
             embeddings=embeddings,
             metadatas=metadatas,
             documents=documents,
             ids=ids,
@@ -114,34 +125,34 @@
 
         return True  # NIT: should this return the ids of the succesfully added items?
 
     def _update(
         self,
         collection_name: str,
         ids: IDs,
-        embeddings=None,
-        metadatas=None,
-        documents=None,
+        embeddings: Optional[Embeddings] = None,
+        metadatas: Optional[Metadatas] = None,
+        documents: Optional[Documents] = None,
     ):
         collection_uuid = self._db.get_collection_uuid_from_name(collection_name)
         self._db.update(collection_uuid, ids, embeddings, metadatas, documents)
 
         return True
 
     def _get(
         self,
-        collection_name,
-        ids=None,
-        where=None,
-        sort=None,
-        limit=None,
-        offset=None,
-        page=None,
-        page_size=None,
-        where_document=None,
+        collection_name: str,
+        ids: Optional[IDs] = None,
+        where: Optional[Where] = {},
+        sort: Optional[str] = None,
+        limit: Optional[int] = None,
+        offset: Optional[int] = None,
+        page: Optional[int] = None,
+        page_size: Optional[int] = None,
+        where_document: Optional[WhereDocument] = {},
         include: Include = ["embeddings", "metadatas", "documents"],
     ):
         if where is None:
             where = {}
 
         if where_document is None:
             where_document = {}
@@ -268,15 +279,15 @@
             query_result["ids"].append(ids)
 
         return query_result
 
     def raw_sql(self, raw_sql):
         return self._db.raw_sql(raw_sql)
 
-    def create_index(self, collection_name):
+    def create_index(self, collection_name: str):
         collection_uuid = self._db.get_collection_uuid_from_name(collection_name)
         self._db.create_index(collection_uuid=collection_uuid)
         return True
 
     def _peek(self, collection_name, n=10):
         return self._get(collection_name=collection_name, limit=n)
```

### Comparing `chromadb-0.3.7/chromadb/api/models/Collection.py` & `chromadb-0.3.8/chromadb/api/models/Collection.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.3.7/chromadb/api/types.py` & `chromadb-0.3.8/chromadb/api/types.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.3.7/chromadb/config.py` & `chromadb-0.3.8/chromadb/config.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.3.7/chromadb/db/clickhouse.py` & `chromadb-0.3.8/chromadb/db/clickhouse.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 from chromadb.errors import (
     NoDatapointsException,
     InvalidDimensionException,
     NotEnoughElementsException,
 )
 import uuid
 import time
-import os
-import itertools
+import numpy.typing as npt
 import json
-from typing import Optional, Sequence, List, Tuple, cast
+from typing import Dict, Optional, Sequence, List, Tuple, cast
 import clickhouse_connect
+from clickhouse_connect.driver.client import Client
 
 COLLECTION_TABLE_SCHEMA = [{"uuid": "UUID"}, {"name": "String"}, {"metadata": "String"}]
 
 EMBEDDING_TABLE_SCHEMA = [
     {"collection_uuid": "UUID"},
     {"uuid": "UUID"},
     {"embedding": "Array(Float64)"},
@@ -57,18 +57,18 @@
         self._conn.query(f"""SET allow_experimental_lightweight_delete = 1;""")
         self._conn.query(
             f"""SET mutations_sync = 1;"""
         )  # https://clickhouse.com/docs/en/operations/settings/settings/#mutations_sync
         self._create_table_collections(self._conn)
         self._create_table_embeddings(self._conn)
 
-    def _get_conn(self):
+    def _get_conn(self) -> Client:
         if self._conn is None:
             self._init_conn()
-        return self._conn
+        return self._conn  # type: ignore because we know it's not None
 
     def _create_table_collections(self, conn):
         conn.command(
             f"""CREATE TABLE IF NOT EXISTS collections (
             {db_array_schema_to_clickhouse_schema(COLLECTION_TABLE_SCHEMA)}
         ) ENGINE = MergeTree() ORDER BY uuid"""
         )
@@ -82,43 +82,50 @@
 
     #
     #  UTILITY METHODS
     #
     def persist(self):
         raise NotImplementedError("Clickhouse is a persistent database, this method is not needed")
 
-    def get_collection_uuid_from_name(self, name):
+    def get_collection_uuid_from_name(self, name: str) -> str:
         res = self._get_conn().query(
             f"""
             SELECT uuid FROM collections WHERE name = '{name}'
         """
         )
         return res.result_rows[0][0]
 
-    def _create_where_clause(self, collection_uuid, ids=None, where={}, where_document={}):
-        where_clauses = []
+    def _create_where_clause(
+        self,
+        collection_uuid: str,
+        ids: Optional[List[str]] = None,
+        where: Where = {},
+        where_document: WhereDocument = {},
+    ):
+        where_clauses: List[str] = []
         self._format_where(where, where_clauses)
         if len(where_document) > 0:
             where_document_clauses = []
             self._format_where_document(where_document, where_document_clauses)
             where_clauses.extend(where_document_clauses)
 
         if ids is not None:
             where_clauses.append(f" id IN {tuple(ids)}")
 
         where_clauses.append(f"collection_uuid = '{collection_uuid}'")
-        # We know that where_clauses is not empty, so force typechecker
-        where = " AND ".join(cast(List[str], where_clauses))
-        where = f"WHERE {where}"
-        return where
+        where_str = " AND ".join(where_clauses)
+        where_str = f"WHERE {where_str}"
+        return where_str
 
     #
     #  COLLECTION METHODS
     #
-    def create_collection(self, name, metadata=None, get_or_create=False):
+    def create_collection(
+        self, name: str, metadata: Optional[Dict] = None, get_or_create: bool = False
+    ):
         if metadata is None:
             metadata = {}
 
         # poor man's unique constraint
         dupe_check = self.get_collection(name)
 
         if len(dupe_check) > 0:
@@ -133,64 +140,64 @@
         data_to_insert.append([collection_uuid, name, json.dumps(metadata)])
 
         self._get_conn().insert(
             "collections", data_to_insert, column_names=["uuid", "name", "metadata"]
         )
         return collection_uuid
 
-    def get_collection(self, name):
+    def get_collection(self, name: str):
         return (
             self._get_conn()
             .query(
                 f"""
          SELECT * FROM collections WHERE name = '{name}'
          """
             )
             .result_rows
         )
 
     def list_collections(self) -> Sequence[Sequence[str]]:
         return self._get_conn().query(f"""SELECT * FROM collections""").result_rows
 
-    def update_collection(self, current_name, new_name, new_metadata):
+    def update_collection(
+        self, current_name: str, new_name: Optional[str] = None, new_metadata: Optional[Dict] = None
+    ):
         if new_name is None:
             new_name = current_name
         if new_metadata is None:
-            new_metadata = self.get_collection(current_name)[0]
+            new_metadata = self.get_collection(current_name)[0][2]
 
         return self._get_conn().command(
             f"""
 
          ALTER TABLE 
             collections 
          UPDATE
-            metadata = {new_metadata}, 
+            metadata = '{json.dumps(new_metadata)}', 
             name = '{new_name}'
          WHERE 
-
             name = '{current_name}'
          """
         )
 
-    def delete_collection(self, name):
+    def delete_collection(self, name: str):
         collection_uuid = self.get_collection_uuid_from_name(name)
         self._get_conn().command(
             f"""
         DELETE FROM embeddings WHERE collection_uuid = '{collection_uuid}'
         """
         )
 
         self._get_conn().command(
             f"""
          DELETE FROM collections WHERE name = '{name}'
          """
         )
 
         self._idx.delete_index(collection_uuid)
-        return True
 
     #
     #  ITEM METHODS
     #
 
     def add(self, collection_uuid, embeddings, metadatas, documents, ids):
         data_to_insert = [
@@ -342,92 +349,101 @@
             if operator == "$and":
                 results.append(f"({' AND '.join(all_subresults)})")
         else:
             raise ValueError(f"Operator {operator} not supported")
 
     def get(
         self,
-        where={},
-        collection_name=None,
-        collection_uuid=None,
-        ids=None,
-        sort=None,
-        limit=None,
-        offset=None,
-        where_document={},
-        columns: Optional[List] = None,
-    ):
+        where: Where = {},
+        collection_name: Optional[str] = None,
+        collection_uuid: Optional[str] = None,
+        ids: Optional[IDs] = None,
+        sort: Optional[str] = None,
+        limit: Optional[int] = None,
+        offset: Optional[int] = None,
+        where_document: WhereDocument = {},
+        columns: Optional[List[str]] = None,
+    ) -> Sequence:
         if collection_name == None and collection_uuid == None:
             raise TypeError("Arguments collection_name and collection_uuid cannot both be None")
 
         if collection_name is not None:
             collection_uuid = self.get_collection_uuid_from_name(collection_name)
 
         s3 = time.time()
 
-        where = self._create_where_clause(
-            collection_uuid, ids=ids, where=where, where_document=where_document
+        where_str = self._create_where_clause(
+            # collection_uuid must be defined at this point, cast it for typechecker
+            cast(str, collection_uuid),
+            ids=ids,
+            where=where,
+            where_document=where_document,
         )
 
         if sort is not None:
-            where += f" ORDER BY {sort}"
+            where_str += f" ORDER BY {sort}"
         else:
-            where += f" ORDER BY collection_uuid"  # stable ordering
+            where_str += f" ORDER BY collection_uuid"  # stable ordering
 
         if limit is not None or isinstance(limit, int):
-            where += f" LIMIT {limit}"
+            where_str += f" LIMIT {limit}"
 
         if offset is not None or isinstance(offset, int):
-            where += f" OFFSET {offset}"
+            where_str += f" OFFSET {offset}"
 
-        val = self._get(where=where, columns=columns)
+        val = self._get(where=where_str, columns=columns)
 
         return val
 
-    def _count(self, collection_uuid):
-        where_string = ""
-        if collection_uuid is not None:
-            where_string = f"WHERE collection_uuid = '{collection_uuid}'"
+    def _count(self, collection_uuid: str):
+        where_string = f"WHERE collection_uuid = '{collection_uuid}'"
         return self._get_conn().query(f"SELECT COUNT() FROM embeddings {where_string}").result_rows
 
-    def count(self, collection_name):
+    def count(self, collection_name: str):
         collection_uuid = self.get_collection_uuid_from_name(collection_name)
         return self._count(collection_uuid=collection_uuid)[0][0]
 
-    def _delete(self, where_str=None):
+    def _delete(self, where_str: Optional[str] = None):
         deleted_uuids = (
             self._get_conn().query(f"""SELECT uuid FROM embeddings {where_str}""").result_rows
         )
         self._get_conn().command(
             f"""
             DELETE FROM
                 embeddings
         {where_str}
         """
         )
         return [res[0] for res in deleted_uuids] if len(deleted_uuids) > 0 else []
 
     def delete(
-        self, where={}, collection_name=None, collection_uuid=None, ids=None, where_document={}
+        self,
+        where: Where = {},
+        collection_name: Optional[str] = None,
+        collection_uuid: Optional[str] = None,
+        ids: Optional[IDs] = None,
+        where_document: WhereDocument = {},
     ):
         if collection_name == None and collection_uuid == None:
             raise TypeError("Arguments collection_name and collection_uuid cannot both be None")
 
         if collection_name is not None:
             collection_uuid = self.get_collection_uuid_from_name(collection_name)
 
         s3 = time.time()
         where_str = self._create_where_clause(
-            collection_uuid, ids=ids, where=where, where_document=where_document
+            # collection_uuid must be defined at this point, cast it for typechecker
+            cast(str, collection_uuid),
+            ids=ids,
+            where=where,
+            where_document=where_document,
         )
 
         deleted_uuids = self._delete(where_str)
 
-        # if len(where) == 1:
-        #     self._idx.delete(collection_uuid)
         self._idx.delete_from_index(collection_uuid, deleted_uuids)
 
         return deleted_uuids
 
     def get_by_ids(self, ids: list, columns: Optional[List] = None):
         columns = columns + ["uuid"] if columns else ["uuid"]
         select_columns = db_schema_to_keys() if columns is None else columns
@@ -450,15 +466,15 @@
         self,
         where: Where,
         where_document: WhereDocument,
         embeddings: Embeddings,
         n_results: int,
         collection_name=None,
         collection_uuid=None,
-    ) -> Tuple[List[List[uuid.UUID]], List[List[float]]]:
+    ) -> Tuple[List[List[uuid.UUID]], npt.NDArray]:
 
         # Either the collection name or the collection uuid must be provided
         if collection_name == None and collection_uuid == None:
             raise TypeError("Arguments collection_name and collection_uuid cannot both be None")
 
         if collection_name is not None:
             collection_uuid = self.get_collection_uuid_from_name(collection_name)
@@ -493,15 +509,15 @@
             ids = None
         uuids, distances = self._idx.get_nearest_neighbors(
             collection_uuid, embeddings, n_results, ids
         )
 
         return uuids, distances
 
-    def create_index(self, collection_uuid) -> None:
+    def create_index(self, collection_uuid: str):
         """Create an index for a collection_uuid and optionally scoped to a dataset.
         Args:
             collection_uuid (str): The collection_uuid to create an index for
             dataset (str, optional): The dataset to scope the index to. Defaults to None.
         Returns:
             None
         """
```

### Comparing `chromadb-0.3.7/chromadb/db/duckdb.py` & `chromadb-0.3.8/chromadb/db/duckdb.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from chromadb.db.clickhouse import (
     Clickhouse,
     db_array_schema_to_clickhouse_schema,
     EMBEDDING_TABLE_SCHEMA,
     db_schema_to_keys,
     COLLECTION_TABLE_SCHEMA,
 )
-from typing import List, Optional, Sequence
+from typing import List, Optional, Sequence, Dict
 import pandas as pd
 import json
 import duckdb
 import uuid
 import time
 import itertools
 
@@ -72,52 +72,57 @@
         return self._conn.execute(
             f"""SELECT uuid FROM collections WHERE name = ?""", [name]
         ).fetchall()[0][0]
 
     #
     #  COLLECTION METHODS
     #
-    def create_collection(self, name, metadata=None, get_or_create=False):
+    def create_collection(
+        self, name: str, metadata: Optional[Dict] = None, get_or_create: bool = False
+    ):
         if metadata is None:
             metadata = {}
 
         # poor man's unique constraint
         dupe_check = self.get_collection(name)
-        if not dupe_check.empty:
+        if len(dupe_check) > 0:
             if get_or_create == True:
                 print(f"collection with name {name} already exists, returning existing collection")
                 return dupe_check
             else:
                 raise Exception(f"collection with name {name} already exists")
 
         return self._conn.execute(
             f"""INSERT INTO collections (uuid, name, metadata) VALUES (?, ?, ?)""",
             [str(uuid.uuid4()), name, json.dumps(metadata)],
         )
 
-    def get_collection(self, name):
-        return self._conn.execute(f"""SELECT * FROM collections WHERE name = ?""", [name]).df()
+    def get_collection(self, name: str) -> Sequence:
+        return self._conn.execute(
+            f"""SELECT * FROM collections WHERE name = ?""", [name]
+        ).fetchall()
 
     def list_collections(self) -> Sequence[Sequence[str]]:
         return self._conn.execute(f"""SELECT * FROM collections""").fetchall()
 
-    def delete_collection(self, name):
+    def delete_collection(self, name: str):
         collection_uuid = self.get_collection_uuid_from_name(name)
         self._conn.execute(
             f"""DELETE FROM embeddings WHERE collection_uuid = ?""", [collection_uuid]
         )
         self._idx.delete_index(collection_uuid)
         self._conn.execute(f"""DELETE FROM collections WHERE name = ?""", [name])
-        return True
 
-    def update_collection(self, current_name, new_name, new_metadata):
+    def update_collection(
+        self, current_name: str, new_name: str, new_metadata: Optional[Dict] = None
+    ):
         if new_name is None:
             new_name = current_name
         if new_metadata is None:
-            new_metadata = self.get_collection(current_name).metadata[0]
+            new_metadata = self.get_collection(current_name)[0][2]
 
         self._conn.execute(
             f"""UPDATE collections SET name = ?, metadata = ? WHERE name = ?""",
             [new_name, json.dumps(new_metadata), current_name],
         )
 
     #
@@ -283,15 +288,15 @@
             {", ".join(update_fields)}
         WHERE
             id = ? AND 
             collection_uuid = '{collection_uuid}';
         """
         self._conn.executemany(update_statement, update_data)
 
-    def _delete(self, where_str):
+    def _delete(self, where_str: Optional[str] = None):
         uuids_deleted = self._conn.execute(
             f"""SELECT uuid FROM embeddings {where_str}"""
         ).fetchall()
         self._conn.execute(
             f"""
             DELETE FROM
                 embeddings
```

### Comparing `chromadb-0.3.7/chromadb/db/index/__init__.py` & `chromadb-0.3.8/chromadb/db/index/__init__.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.3.7/chromadb/db/index/hnswlib.py` & `chromadb-0.3.8/chromadb/db/index/hnswlib.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.3.7/chromadb/server/fastapi/types.py` & `chromadb-0.3.8/chromadb/server/fastapi/types.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.3.7/chromadb/test/test_api.py` & `chromadb-0.3.8/chromadb/test/test_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -435,14 +435,18 @@
     api.reset()
     api.create_collection("testspace")
 
     # get collection does not throw an error
     collection = api.get_collection("testspace")
     assert collection.name == "testspace"
 
+    # get collection should throw an error if collection does not exist
+    with pytest.raises(Exception) as e:
+        collection = api.get_collection("testspace2")
+
 
 @pytest.mark.parametrize("api_fixture", test_apis)
 def test_list_collections(api_fixture, request):
     api = request.getfixturevalue(api_fixture.__name__)
 
     api.reset()
     api.create_collection("testspace")
```

### Comparing `chromadb-0.3.7/chromadb/test/test_chroma.py` & `chromadb-0.3.8/chromadb/test/test_chroma.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.3.7/chromadb/utils/embedding_functions.py` & `chromadb-0.3.8/chromadb/utils/embedding_functions.py`

 * *Files identical despite different names*

### Comparing `chromadb-0.3.7/chromadb.egg-info/PKG-INFO` & `chromadb-0.3.8/chromadb.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chromadb
-Version: 0.3.7
+Version: 0.3.8
 Summary: Chroma.
 Author-email: Jeff Huber <jeff@trychroma.com>, Anton Troynikov <anton@trychroma.com>
 Project-URL: Homepage, https://github.com/chroma-core/chroma
 Project-URL: Bug Tracker, https://github.com/chroma-core/chroma/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -20,25 +20,29 @@
 __Chroma is the open-source embedding database__. Chroma makes it easy to build LLM apps by making knowledge, facts, and skills pluggable for LLMs. 
 
 - [💬 Community Discord](https://discord.gg/MMeYNTmh3x)
 - [📖 Documentation](https://docs.trychroma.com/)
 - [💡 Colab Example](https://colab.research.google.com/drive/1QEzFyqnoFxq7LUGyP1vzR4iLt9PpCDXv?usp=sharing)
 - [🏠 Homepage](https://www.trychroma.com/)
 
+Language Support
+- `python` - `pip install chromadb`
+- `javascript/typescript` - `npm install --save chromadb`
+
 ## ChatGPT for ______
 
 For example, the `"Chat your data"` use case:
 1. Add documents to your database. You can pass in your own embeddings, embedding function, or let Chroma embed them for you.
 2. Query relevant documents with natural language.
 3. Compose documents into the context window of an LLM like `GPT3` for additional summarization or analysis. 
 
 
 ## Features
 - __Simple__: Fully-typed, fully-tested, fully-documented == happiness
-- __Integrations__: `🦜️🔗 LangChain` and more soon
+- __Integrations__: `🦜️🔗 LangChain` (python and js), `🦙 gpt-index/LlamaIndex` and more soon
 - __Dev, Test, Prod__: the same API that runs in your python notebook, scales to your cluster
 - __Feature-rich__: Queries, filtering, density estimation and more
 - __Free__: Apache 2.0 Licensed
 
 ## Get up and running
 ```python
 pip install chromadb
```

### Comparing `chromadb-0.3.7/docker-compose.test.yml` & `chromadb-0.3.8/docker-compose.test.yml`

 * *Files identical despite different names*

### Comparing `chromadb-0.3.7/docker-compose.yml` & `chromadb-0.3.8/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `chromadb-0.3.7/examples/local_persistence.ipynb` & `chromadb-0.3.8/examples/local_persistence.ipynb`

 * *Files identical despite different names*

### Comparing `chromadb-0.3.7/examples/where_filtering.ipynb` & `chromadb-0.3.8/examples/where_filtering.ipynb`

 * *Files identical despite different names*

### Comparing `chromadb-0.3.7/new_api.py` & `chromadb-0.3.8/new_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -280,15 +280,15 @@
 )
 
 
 # Try to add embeddings of the wrong dimension.
 # This should fail and not add any embeddings
 # TODO: Currently only works locally since the exception is raised on the database side
 try:
-     collection.add(
+    collection.add(
         embeddings=[[1.1, 2.3, 3.2], [4.5, 6.9, 4.4], [1.1, 2.3, 3.2], [4.5, 6.9, 4.4]],
         metadatas=[
             {"uri": "img1.png", "style": "style1"},
             {"uri": "img2.png", "style": "style1"},
             {"uri": "img3.png", "style": "style1"},
             {"uri": "img4.png", "style": "style1"},
         ],
```

### Comparing `chromadb-0.3.7/pyproject.toml` & `chromadb-0.3.8/pyproject.toml`

 * *Files identical despite different names*

