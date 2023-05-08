# Comparing `tmp/caikit-tgis-backend-0.1.1.tar.gz` & `tmp/caikit-tgis-backend-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caikit-tgis-backend-0.1.1.tar", last modified: Thu May  4 18:54:33 2023, max compression
+gzip compressed data, was "caikit-tgis-backend-0.1.2.tar", last modified: Mon May  8 20:24:48 2023, max compression
```

## Comparing `caikit-tgis-backend-0.1.1.tar` & `caikit-tgis-backend-0.1.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0       65 2023-05-04 18:54:26.395942 caikit-tgis-backend-0.1.1/.coveragerc
--rw-r--r--   0        0        0      676 2023-05-04 18:54:26.395942 caikit-tgis-backend-0.1.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      579 2023-05-04 18:54:26.395942 caikit-tgis-backend-0.1.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      519 2023-05-04 18:54:26.395942 caikit-tgis-backend-0.1.1/.github/ISSUE_TEMPLATE/user_story.md
--rw-r--r--   0        0        0      105 2023-05-04 18:54:26.395942 caikit-tgis-backend-0.1.1/.github/dependabot.yml
--rw-r--r--   0        0        0     1280 2023-05-04 18:54:26.395942 caikit-tgis-backend-0.1.1/.github/workflows/build-library.yml
--rw-r--r--   0        0        0     1141 2023-05-04 18:54:26.395942 caikit-tgis-backend-0.1.1/.github/workflows/lint-code.yml
--rw-r--r--   0        0        0     1144 2023-05-04 18:54:26.395942 caikit-tgis-backend-0.1.1/.github/workflows/publish-library.yml
--rw-r--r--   0        0        0      183 2023-05-04 18:54:26.395942 caikit-tgis-backend-0.1.1/.gitignore
--rw-r--r--   0        0        0      318 2023-05-04 18:54:26.395942 caikit-tgis-backend-0.1.1/.isort.cfg
--rw-r--r--   0        0        0      440 2023-05-04 18:54:26.395942 caikit-tgis-backend-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0       24 2023-05-04 18:54:26.395942 caikit-tgis-backend-0.1.1/.prettierignore
--rw-r--r--   0        0        0       12 2023-05-04 18:54:26.395942 caikit-tgis-backend-0.1.1/.prettierrc.yaml
--rw-r--r--   0        0        0    21406 2023-05-04 18:54:26.395942 caikit-tgis-backend-0.1.1/.pylintrc
--rw-r--r--   0        0        0       78 2023-05-04 18:54:26.395942 caikit-tgis-backend-0.1.1/.whitesource
--rw-r--r--   0        0        0      314 2023-05-04 18:54:26.395942 caikit-tgis-backend-0.1.1/CODEOWNERS
--rw-r--r--   0        0        0     7269 2023-05-04 18:54:26.395942 caikit-tgis-backend-0.1.1/CONTRIBUTING.md
--rw-r--r--   0        0        0    11357 2023-05-04 18:54:26.395942 caikit-tgis-backend-0.1.1/LICENSE
--rw-r--r--   0        0        0      138 2023-05-04 18:54:26.395942 caikit-tgis-backend-0.1.1/README.md
--rw-r--r--   0        0        0      152 2023-05-04 18:54:26.395942 caikit-tgis-backend-0.1.1/SECURITY.md
--rw-r--r--   0        0        0      723 2023-05-04 18:54:26.395942 caikit-tgis-backend-0.1.1/caikit_tgis_backend/__init__.py
--rw-r--r--   0        0        0     5727 2023-05-04 18:54:26.395942 caikit-tgis-backend-0.1.1/caikit_tgis_backend/generation.proto
--rw-r--r--   0        0        0      840 2023-05-04 18:54:26.395942 caikit-tgis-backend-0.1.1/caikit_tgis_backend/protobufs/__init__.py
--rw-r--r--   0        0        0    13426 2023-05-04 18:54:26.395942 caikit-tgis-backend-0.1.1/caikit_tgis_backend/protobufs/generation_pb2.py
--rw-r--r--   0        0        0     5685 2023-05-04 18:54:26.395942 caikit-tgis-backend-0.1.1/caikit_tgis_backend/protobufs/generation_pb2_grpc.py
--rw-r--r--   0        0        0    12520 2023-05-04 18:54:26.395942 caikit-tgis-backend-0.1.1/caikit_tgis_backend/tgis_backend.py
--rw-r--r--   0        0        0      169 2023-05-04 18:54:26.395942 caikit-tgis-backend-0.1.1/code-of-conduct.md
--rw-r--r--   0        0        0      655 2023-05-04 18:54:29.651985 caikit-tgis-backend-0.1.1/pyproject.toml
--rwxr-xr-x   0        0        0      720 2023-05-04 18:54:26.395942 caikit-tgis-backend-0.1.1/scripts/fmt.sh
--rwxr-xr-x   0        0        0      393 2023-05-04 18:54:26.395942 caikit-tgis-backend-0.1.1/scripts/gen_tgis_protos.sh
--rw-r--r--   0        0        0       33 2023-05-04 18:54:26.395942 caikit-tgis-backend-0.1.1/setup_requirements.txt
--rw-r--r--   0        0        0        0 2023-05-04 18:54:26.395942 caikit-tgis-backend-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0      342 2023-05-04 18:54:26.395942 caikit-tgis-backend-0.1.1/tests/conftest.py
--rw-r--r--   0        0        0     9063 2023-05-04 18:54:26.395942 caikit-tgis-backend-0.1.1/tests/test_tgis_backend.py
--rw-r--r--   0        0        0     7629 2023-05-04 18:54:26.395942 caikit-tgis-backend-0.1.1/tests/tgis_mock.py
--rw-r--r--   0        0        0     1209 2023-05-04 18:54:26.395942 caikit-tgis-backend-0.1.1/tox.ini
--rw-r--r--   0        0        0      556 1970-01-01 00:00:00.000000 caikit-tgis-backend-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       65 2023-05-08 20:24:41.083503 caikit-tgis-backend-0.1.2/.coveragerc
+-rw-r--r--   0        0        0      676 2023-05-08 20:24:41.083503 caikit-tgis-backend-0.1.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      579 2023-05-08 20:24:41.083503 caikit-tgis-backend-0.1.2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      519 2023-05-08 20:24:41.083503 caikit-tgis-backend-0.1.2/.github/ISSUE_TEMPLATE/user_story.md
+-rw-r--r--   0        0        0      105 2023-05-08 20:24:41.083503 caikit-tgis-backend-0.1.2/.github/dependabot.yml
+-rw-r--r--   0        0        0     1280 2023-05-08 20:24:41.083503 caikit-tgis-backend-0.1.2/.github/workflows/build-library.yml
+-rw-r--r--   0        0        0     1141 2023-05-08 20:24:41.083503 caikit-tgis-backend-0.1.2/.github/workflows/lint-code.yml
+-rw-r--r--   0        0        0     1144 2023-05-08 20:24:41.083503 caikit-tgis-backend-0.1.2/.github/workflows/publish-library.yml
+-rw-r--r--   0        0        0      183 2023-05-08 20:24:41.083503 caikit-tgis-backend-0.1.2/.gitignore
+-rw-r--r--   0        0        0      318 2023-05-08 20:24:41.083503 caikit-tgis-backend-0.1.2/.isort.cfg
+-rw-r--r--   0        0        0      440 2023-05-08 20:24:41.083503 caikit-tgis-backend-0.1.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       24 2023-05-08 20:24:41.083503 caikit-tgis-backend-0.1.2/.prettierignore
+-rw-r--r--   0        0        0       12 2023-05-08 20:24:41.083503 caikit-tgis-backend-0.1.2/.prettierrc.yaml
+-rw-r--r--   0        0        0    21406 2023-05-08 20:24:41.083503 caikit-tgis-backend-0.1.2/.pylintrc
+-rw-r--r--   0        0        0       78 2023-05-08 20:24:41.083503 caikit-tgis-backend-0.1.2/.whitesource
+-rw-r--r--   0        0        0      314 2023-05-08 20:24:41.083503 caikit-tgis-backend-0.1.2/CODEOWNERS
+-rw-r--r--   0        0        0     7269 2023-05-08 20:24:41.083503 caikit-tgis-backend-0.1.2/CONTRIBUTING.md
+-rw-r--r--   0        0        0    11357 2023-05-08 20:24:41.083503 caikit-tgis-backend-0.1.2/LICENSE
+-rw-r--r--   0        0        0      138 2023-05-08 20:24:41.083503 caikit-tgis-backend-0.1.2/README.md
+-rw-r--r--   0        0        0      152 2023-05-08 20:24:41.083503 caikit-tgis-backend-0.1.2/SECURITY.md
+-rw-r--r--   0        0        0      723 2023-05-08 20:24:41.083503 caikit-tgis-backend-0.1.2/caikit_tgis_backend/__init__.py
+-rw-r--r--   0        0        0     5727 2023-05-08 20:24:41.083503 caikit-tgis-backend-0.1.2/caikit_tgis_backend/generation.proto
+-rw-r--r--   0        0        0      840 2023-05-08 20:24:41.083503 caikit-tgis-backend-0.1.2/caikit_tgis_backend/protobufs/__init__.py
+-rw-r--r--   0        0        0    13426 2023-05-08 20:24:41.083503 caikit-tgis-backend-0.1.2/caikit_tgis_backend/protobufs/generation_pb2.py
+-rw-r--r--   0        0        0     5685 2023-05-08 20:24:41.083503 caikit-tgis-backend-0.1.2/caikit_tgis_backend/protobufs/generation_pb2_grpc.py
+-rw-r--r--   0        0        0    12510 2023-05-08 20:24:41.083503 caikit-tgis-backend-0.1.2/caikit_tgis_backend/tgis_backend.py
+-rw-r--r--   0        0        0      169 2023-05-08 20:24:41.083503 caikit-tgis-backend-0.1.2/code-of-conduct.md
+-rw-r--r--   0        0        0      655 2023-05-08 20:24:44.215511 caikit-tgis-backend-0.1.2/pyproject.toml
+-rwxr-xr-x   0        0        0      720 2023-05-08 20:24:41.083503 caikit-tgis-backend-0.1.2/scripts/fmt.sh
+-rwxr-xr-x   0        0        0      393 2023-05-08 20:24:41.083503 caikit-tgis-backend-0.1.2/scripts/gen_tgis_protos.sh
+-rw-r--r--   0        0        0       33 2023-05-08 20:24:41.083503 caikit-tgis-backend-0.1.2/setup_requirements.txt
+-rw-r--r--   0        0        0        0 2023-05-08 20:24:41.083503 caikit-tgis-backend-0.1.2/tests/__init__.py
+-rw-r--r--   0        0        0      342 2023-05-08 20:24:41.083503 caikit-tgis-backend-0.1.2/tests/conftest.py
+-rw-r--r--   0        0        0     9063 2023-05-08 20:24:41.083503 caikit-tgis-backend-0.1.2/tests/test_tgis_backend.py
+-rw-r--r--   0        0        0     7629 2023-05-08 20:24:41.083503 caikit-tgis-backend-0.1.2/tests/tgis_mock.py
+-rw-r--r--   0        0        0     1209 2023-05-08 20:24:41.083503 caikit-tgis-backend-0.1.2/tox.ini
+-rw-r--r--   0        0        0      556 1970-01-01 00:00:00.000000 caikit-tgis-backend-0.1.2/PKG-INFO
```

### Comparing `caikit-tgis-backend-0.1.1/.github/ISSUE_TEMPLATE/bug_report.md` & `caikit-tgis-backend-0.1.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `caikit-tgis-backend-0.1.1/.github/ISSUE_TEMPLATE/feature_request.md` & `caikit-tgis-backend-0.1.2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `caikit-tgis-backend-0.1.1/.github/ISSUE_TEMPLATE/user_story.md` & `caikit-tgis-backend-0.1.2/.github/ISSUE_TEMPLATE/user_story.md`

 * *Files identical despite different names*

### Comparing `caikit-tgis-backend-0.1.1/.github/workflows/build-library.yml` & `caikit-tgis-backend-0.1.2/.github/workflows/build-library.yml`

 * *Files identical despite different names*

### Comparing `caikit-tgis-backend-0.1.1/.github/workflows/lint-code.yml` & `caikit-tgis-backend-0.1.2/.github/workflows/lint-code.yml`

 * *Files identical despite different names*

### Comparing `caikit-tgis-backend-0.1.1/.github/workflows/publish-library.yml` & `caikit-tgis-backend-0.1.2/.github/workflows/publish-library.yml`

 * *Files identical despite different names*

### Comparing `caikit-tgis-backend-0.1.1/.pylintrc` & `caikit-tgis-backend-0.1.2/.pylintrc`

 * *Files identical despite different names*

### Comparing `caikit-tgis-backend-0.1.1/CONTRIBUTING.md` & `caikit-tgis-backend-0.1.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `caikit-tgis-backend-0.1.1/LICENSE` & `caikit-tgis-backend-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `caikit-tgis-backend-0.1.1/caikit_tgis_backend/__init__.py` & `caikit-tgis-backend-0.1.2/caikit_tgis_backend/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-tgis-backend-0.1.1/caikit_tgis_backend/generation.proto` & `caikit-tgis-backend-0.1.2/caikit_tgis_backend/generation.proto`

 * *Files identical despite different names*

### Comparing `caikit-tgis-backend-0.1.1/caikit_tgis_backend/protobufs/__init__.py` & `caikit-tgis-backend-0.1.2/caikit_tgis_backend/protobufs/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-tgis-backend-0.1.1/caikit_tgis_backend/protobufs/generation_pb2.py` & `caikit-tgis-backend-0.1.2/caikit_tgis_backend/protobufs/generation_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit-tgis-backend-0.1.1/caikit_tgis_backend/protobufs/generation_pb2_grpc.py` & `caikit-tgis-backend-0.1.2/caikit_tgis_backend/protobufs/generation_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `caikit-tgis-backend-0.1.1/caikit_tgis_backend/tgis_backend.py` & `caikit-tgis-backend-0.1.2/caikit_tgis_backend/tgis_backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,22 +66,24 @@
 
         # NOTE: Needs to be set before any possible errors since it's used in
         #   the destructor
         self._proc_mutex = Lock()
         self._local_tgis = None
         self._tgis_proc = None
 
-        # Parse the config to see if we"re managing a connection to a remote
+        # Parse the config to see if we're managing a connection to a remote
         # TGIS instance or running a local copy
-        connection_cfg = self.config.get("connection")
+        connection_cfg = self.config.get("connection") or {}
+        error.type_check("<TGB20235229E>", dict, connection=connection_cfg)
+
         local_cfg = self.config.get("local") or {}
+        error.type_check("<TGB20235225E>", dict, local=local_cfg)
 
-        if not connection_cfg:
+        if not connection_cfg or not connection_cfg.get("hostname"):
             log.info("<TGB20235227I>", "Managing local TGIS instance")
-            error.type_check("<TGB20235225E>", dict, local=local_cfg)
             self._local_tgis = True
 
             # Members that are only used when booting TGIS locally
             self._grpc_port = local_cfg.get("grpc_port") or self.TGIS_LOCAL_GRPC_PORT
             self._http_port = local_cfg.get("http_port") or self.TGIS_LOCAL_HTTP_PORT
             self._health_poll_delay = local_cfg.get("health_poll_delay", 1.0)
             self._health_poll_timeout = local_cfg.get("health_poll_timeout", 10)
@@ -94,17 +96,14 @@
 
             # Shared members that need to be set for the client
             self._ca_cert, self._client_cert, self._client_key = [None] * 3
             self._hostname = f"localhost:{self._grpc_port}"
 
         else:
             log.info("<TGB20235226I>", "Managing remote TGIS connection")
-            error.type_check(
-                "<TGB20235229E>", dict, allow_none=True, connection=connection_cfg
-            )
             self._local_tgis = False
             self._hostname = connection_cfg.get("hostname")
             error.type_check("<TGB20235230E>", str, hostname=self._hostname)
             error.value_check(
                 "<TGB20235231E>",
                 ":" in self._hostname,
                 "Invalid hostname: %s",
```

### Comparing `caikit-tgis-backend-0.1.1/pyproject.toml` & `caikit-tgis-backend-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "caikit-tgis-backend"
 # Not the actual current version: overwritten by CI
-version = "0.1.1"
+version = "0.1.2"
 description = "Caikit module backend for models run in TGIS"
 license = {text = "Apache-2.0"}
 readme = "README.md"
 requires-python = "~=3.8"
 classifiers=[
     "License :: OSI Approved :: Apache Software License"
 ]
```

### Comparing `caikit-tgis-backend-0.1.1/scripts/fmt.sh` & `caikit-tgis-backend-0.1.2/scripts/fmt.sh`

 * *Files identical despite different names*

### Comparing `caikit-tgis-backend-0.1.1/tests/test_tgis_backend.py` & `caikit-tgis-backend-0.1.2/tests/test_tgis_backend.py`

 * *Files identical despite different names*

### Comparing `caikit-tgis-backend-0.1.1/tests/tgis_mock.py` & `caikit-tgis-backend-0.1.2/tests/tgis_mock.py`

 * *Files identical despite different names*

### Comparing `caikit-tgis-backend-0.1.1/tox.ini` & `caikit-tgis-backend-0.1.2/tox.ini`

 * *Files identical despite different names*

### Comparing `caikit-tgis-backend-0.1.1/PKG-INFO` & `caikit-tgis-backend-0.1.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caikit-tgis-backend
-Version: 0.1.1
+Version: 0.1.2
 Summary: Caikit module backend for models run in TGIS
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Dist: caikit>=0.2.0,<0.4.0
 Requires-Dist: grpcio>=1.35.0,<2.0
 Requires-Dist: requests>=2.28.2,<3
```

