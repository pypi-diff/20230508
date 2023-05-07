# Comparing `tmp/v3io_frames-0.9.5.tar.gz` & `tmp/v3io_frames-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/v3io_frames-0.9.5.tar", last modified: Mon Oct 11 12:51:15 2021, max compression
+gzip compressed data, was "dist/v3io_frames-0.9.6.tar", last modified: Sun Oct 17 17:48:09 2021, max compression
```

## Comparing `v3io_frames-0.9.5.tar` & `v3io_frames-0.9.6.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-11 12:51:15.000000 v3io_frames-0.9.5/
--rw-r--r--   0 root         (0) root         (0)    11357 2021-10-11 12:44:22.000000 v3io_frames-0.9.5/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)       94 2021-10-11 12:44:22.000000 v3io_frames-0.9.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2015 2021-10-11 12:51:15.000000 v3io_frames-0.9.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      405 2021-10-11 12:50:35.000000 v3io_frames-0.9.5/Pipfile
--rw-r--r--   0 root         (0) root         (0)    42443 2021-10-11 12:51:08.000000 v3io_frames-0.9.5/Pipfile.lock
--rw-r--r--   0 root         (0) root         (0)      971 2021-10-11 12:44:22.000000 v3io_frames-0.9.5/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2021-10-11 12:51:15.000000 v3io_frames-0.9.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3167 2021-10-11 12:44:22.000000 v3io_frames-0.9.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-11 12:51:15.000000 v3io_frames-0.9.5/tests/
--rw-r--r--   0 root         (0) root         (0)     4244 2021-10-11 12:44:22.000000 v3io_frames-0.9.5/tests/conftest.py
--rw-r--r--   0 root         (0) root         (0)      959 2021-10-11 12:44:22.000000 v3io_frames-0.9.5/tests/pip_docker.py
--rw-r--r--   0 root         (0) root         (0)      939 2021-10-11 12:44:22.000000 v3io_frames-0.9.5/tests/test_benchmark.py
--rw-r--r--   0 root         (0) root         (0)     2225 2021-10-11 12:44:22.000000 v3io_frames-0.9.5/tests/test_client.py
--rw-r--r--   0 root         (0) root         (0)     1670 2021-10-11 12:44:22.000000 v3io_frames-0.9.5/tests/test_concurrent.py
--rw-r--r--   0 root         (0) root         (0)     2800 2021-10-11 12:44:22.000000 v3io_frames-0.9.5/tests/test_cudf.py
--rw-r--r--   0 root         (0) root         (0)     4279 2021-10-11 12:44:22.000000 v3io_frames-0.9.5/tests/test_http.py
--rw-r--r--   0 root         (0) root         (0)     7893 2021-10-11 12:44:22.000000 v3io_frames-0.9.5/tests/test_integration.py
--rw-r--r--   0 root         (0) root         (0)     3189 2021-10-11 12:44:22.000000 v3io_frames-0.9.5/tests/test_pbutils.py
--rw-r--r--   0 root         (0) root         (0)     3441 2021-10-11 12:44:22.000000 v3io_frames-0.9.5/tests/test_pdutils.py
--rw-r--r--   0 root         (0) root         (0)     2725 2021-10-11 12:44:22.000000 v3io_frames-0.9.5/tests/test_pip_docker.py
--rw-r--r--   0 root         (0) root         (0)     1996 2021-10-11 12:44:22.000000 v3io_frames-0.9.5/tests/test_v3io_frames.py
--rw-r--r--   0 root         (0) root         (0)   358246 2021-10-11 12:44:22.000000 v3io_frames-0.9.5/tests/weather.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-11 12:51:15.000000 v3io_frames-0.9.5/v3io_frames/
--rw-r--r--   0 root         (0) root         (0)     5199 2021-10-11 12:51:15.000000 v3io_frames-0.9.5/v3io_frames/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19618 2021-10-11 12:44:22.000000 v3io_frames-0.9.5/v3io_frames/client.py
--rw-r--r--   0 root         (0) root         (0)     1804 2021-10-11 12:44:22.000000 v3io_frames-0.9.5/v3io_frames/dtypes.py
--rw-r--r--   0 root         (0) root         (0)     1367 2021-10-11 12:44:22.000000 v3io_frames-0.9.5/v3io_frames/errors.py
--rw-r--r--   0 root         (0) root         (0)    81779 2021-10-11 12:44:22.000000 v3io_frames-0.9.5/v3io_frames/frames_pb2.py
--rw-r--r--   0 root         (0) root         (0)     5668 2021-10-11 12:44:22.000000 v3io_frames-0.9.5/v3io_frames/frames_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    11777 2021-10-11 12:44:22.000000 v3io_frames-0.9.5/v3io_frames/grpc.py
--rw-r--r--   0 root         (0) root         (0)    10537 2021-10-11 12:44:22.000000 v3io_frames-0.9.5/v3io_frames/http.py
--rw-r--r--   0 root         (0) root         (0)    13501 2021-10-11 12:44:22.000000 v3io_frames-0.9.5/v3io_frames/pbutils.py
--rw-r--r--   0 root         (0) root         (0)     3414 2021-10-11 12:44:22.000000 v3io_frames-0.9.5/v3io_frames/pdutils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-11 12:51:15.000000 v3io_frames-0.9.5/v3io_frames.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2015 2021-10-11 12:51:15.000000 v3io_frames-0.9.5/v3io_frames.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      755 2021-10-11 12:51:15.000000 v3io_frames-0.9.5/v3io_frames.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-10-11 12:51:15.000000 v3io_frames-0.9.5/v3io_frames.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      202 2021-10-11 12:51:15.000000 v3io_frames-0.9.5/v3io_frames.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2021-10-11 12:51:15.000000 v3io_frames-0.9.5/v3io_frames.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-17 17:48:09.000000 v3io_frames-0.9.6/
+-rw-r--r--   0 root         (0) root         (0)    11357 2021-10-17 17:42:26.000000 v3io_frames-0.9.6/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)       94 2021-10-17 17:42:26.000000 v3io_frames-0.9.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2015 2021-10-17 17:48:09.000000 v3io_frames-0.9.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      405 2021-10-17 17:48:00.000000 v3io_frames-0.9.6/Pipfile
+-rw-r--r--   0 root         (0) root         (0)    42843 2021-10-17 17:44:11.000000 v3io_frames-0.9.6/Pipfile.lock
+-rw-r--r--   0 root         (0) root         (0)      971 2021-10-17 17:42:26.000000 v3io_frames-0.9.6/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2021-10-17 17:48:09.000000 v3io_frames-0.9.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2896 2021-10-17 17:42:26.000000 v3io_frames-0.9.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-17 17:48:09.000000 v3io_frames-0.9.6/tests/
+-rw-r--r--   0 root         (0) root         (0)     4244 2021-10-17 17:42:26.000000 v3io_frames-0.9.6/tests/conftest.py
+-rw-r--r--   0 root         (0) root         (0)      959 2021-10-17 17:42:26.000000 v3io_frames-0.9.6/tests/pip_docker.py
+-rw-r--r--   0 root         (0) root         (0)      939 2021-10-17 17:42:26.000000 v3io_frames-0.9.6/tests/test_benchmark.py
+-rw-r--r--   0 root         (0) root         (0)     2225 2021-10-17 17:42:26.000000 v3io_frames-0.9.6/tests/test_client.py
+-rw-r--r--   0 root         (0) root         (0)     1670 2021-10-17 17:42:26.000000 v3io_frames-0.9.6/tests/test_concurrent.py
+-rw-r--r--   0 root         (0) root         (0)     2800 2021-10-17 17:42:26.000000 v3io_frames-0.9.6/tests/test_cudf.py
+-rw-r--r--   0 root         (0) root         (0)     4279 2021-10-17 17:42:26.000000 v3io_frames-0.9.6/tests/test_http.py
+-rw-r--r--   0 root         (0) root         (0)     7893 2021-10-17 17:42:26.000000 v3io_frames-0.9.6/tests/test_integration.py
+-rw-r--r--   0 root         (0) root         (0)     3189 2021-10-17 17:42:26.000000 v3io_frames-0.9.6/tests/test_pbutils.py
+-rw-r--r--   0 root         (0) root         (0)     3441 2021-10-17 17:42:26.000000 v3io_frames-0.9.6/tests/test_pdutils.py
+-rw-r--r--   0 root         (0) root         (0)     2725 2021-10-17 17:42:26.000000 v3io_frames-0.9.6/tests/test_pip_docker.py
+-rw-r--r--   0 root         (0) root         (0)     1996 2021-10-17 17:42:26.000000 v3io_frames-0.9.6/tests/test_v3io_frames.py
+-rw-r--r--   0 root         (0) root         (0)   358246 2021-10-17 17:42:26.000000 v3io_frames-0.9.6/tests/weather.csv
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-17 17:48:09.000000 v3io_frames-0.9.6/v3io_frames/
+-rw-r--r--   0 root         (0) root         (0)     5199 2021-10-17 17:48:09.000000 v3io_frames-0.9.6/v3io_frames/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19618 2021-10-17 17:42:26.000000 v3io_frames-0.9.6/v3io_frames/client.py
+-rw-r--r--   0 root         (0) root         (0)     1804 2021-10-17 17:42:26.000000 v3io_frames-0.9.6/v3io_frames/dtypes.py
+-rw-r--r--   0 root         (0) root         (0)     1367 2021-10-17 17:42:26.000000 v3io_frames-0.9.6/v3io_frames/errors.py
+-rw-r--r--   0 root         (0) root         (0)    81779 2021-10-17 17:42:26.000000 v3io_frames-0.9.6/v3io_frames/frames_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     5668 2021-10-17 17:42:26.000000 v3io_frames-0.9.6/v3io_frames/frames_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    11777 2021-10-17 17:42:26.000000 v3io_frames-0.9.6/v3io_frames/grpc.py
+-rw-r--r--   0 root         (0) root         (0)    10537 2021-10-17 17:42:26.000000 v3io_frames-0.9.6/v3io_frames/http.py
+-rw-r--r--   0 root         (0) root         (0)    13501 2021-10-17 17:42:26.000000 v3io_frames-0.9.6/v3io_frames/pbutils.py
+-rw-r--r--   0 root         (0) root         (0)     3414 2021-10-17 17:42:26.000000 v3io_frames-0.9.6/v3io_frames/pdutils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-17 17:48:09.000000 v3io_frames-0.9.6/v3io_frames.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2015 2021-10-17 17:48:09.000000 v3io_frames-0.9.6/v3io_frames.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      755 2021-10-17 17:48:09.000000 v3io_frames-0.9.6/v3io_frames.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-10-17 17:48:09.000000 v3io_frames-0.9.6/v3io_frames.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      108 2021-10-17 17:48:09.000000 v3io_frames-0.9.6/v3io_frames.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2021-10-17 17:48:09.000000 v3io_frames-0.9.6/v3io_frames.egg-info/top_level.txt
```

### Comparing `v3io_frames-0.9.5/LICENSE.txt` & `v3io_frames-0.9.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `v3io_frames-0.9.5/PKG-INFO` & `v3io_frames-0.9.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: v3io_frames
-Version: 0.9.5
+Version: 0.9.6
 Summary: Unified multi-module DataFrames client for the Iguazio Data Science Platform
 Home-page: https://github.com/v3io/frames
 Author: Miki Tebeka
 Author-email: miki@353solutions.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `v3io_frames-0.9.5/Pipfile.lock` & `v3io_frames-0.9.6/Pipfile.lock`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9981060606060606%*

 * *Differences: {"'default'": "{'charset-normalizer': {'hashes': "*

 * *              "['sha256:e019de665e2bcf9c2b64e2e5aa025fa991da8720daa3c1138cadd2fd1856aed0', "*

 * *              "'sha256:f7af805c321bfa1ce6714c51f254e0d5bb5e5834039bc17db7ebe3a4cec9492b'], "*

 * *              "'version': '==2.0.7'}, 'idna': {'hashes': "*

 * *              "['sha256:84d9dd047ffa80596e0f246e2eab0b391788b0503584e8945f2368256d2735ff', "*

 * *              "'sha256:9d643ff0a55b762d5cdb124b8eaa99c66322e2157b69160bc32796e824360e6d'], "*

 * *              '\'version\': \' […]*

```diff
@@ -59,19 +59,19 @@
                 "sha256:78884e7c1d4b00ce3cea67b44566851c4343c120abd683433ce934a68ea58872",
                 "sha256:d62a0163eb4c2344ac042ab2bdf75399a71a2d8c7d47eac2e2ee91b9d6339569"
             ],
             "version": "==2021.10.8"
         },
         "charset-normalizer": {
             "hashes": [
-                "sha256:5d209c0a931f215cee683b6445e2d77677e7e75e159f78def0db09d68fafcaa6",
-                "sha256:5ec46d183433dcbd0ab716f2d7f29d8dee50505b3fdb40c6b985c7c4f5a3591f"
+                "sha256:e019de665e2bcf9c2b64e2e5aa025fa991da8720daa3c1138cadd2fd1856aed0",
+                "sha256:f7af805c321bfa1ce6714c51f254e0d5bb5e5834039bc17db7ebe3a4cec9492b"
             ],
             "markers": "python_version >= '3'",
-            "version": "==2.0.6"
+            "version": "==2.0.7"
         },
         "decorator": {
             "hashes": [
                 "sha256:7b12e7c3c6ab203a29e157335e9122cb03de9ab7264b137594103fd4a683b374",
                 "sha256:e59913af105b9860aa2c8d3272d9de5a56a4e608db9a2f167a8480b323d529a7"
             ],
             "markers": "python_version >= '3.5'",
@@ -189,19 +189,19 @@
                 "sha256:fd059d37d9537fa1a89b1139f8cbed7530a5f81c8577560d3f7710fcec95efde"
             ],
             "index": "pypi",
             "version": "==1.32.0"
         },
         "idna": {
             "hashes": [
-                "sha256:14475042e284991034cb48e06f6851428fb14c4dc953acd9be9a5e95c7b6dd7a",
-                "sha256:467fbad99067910785144ce333826c71fb0e63a425657295239737f7ecd125f3"
+                "sha256:84d9dd047ffa80596e0f246e2eab0b391788b0503584e8945f2368256d2735ff",
+                "sha256:9d643ff0a55b762d5cdb124b8eaa99c66322e2157b69160bc32796e824360e6d"
             ],
             "markers": "python_version >= '3'",
-            "version": "==3.2"
+            "version": "==3.3"
         },
         "imagesize": {
             "hashes": [
                 "sha256:6965f19a6a2039c7d48bca7dba2473069ff854c36ae6f19d2cde309d998228a1",
                 "sha256:b1f6b5a4eab1f73479a50fb79fcf729514a900c341d8503d62a62dbc4127a2b1"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
@@ -351,15 +351,15 @@
                 "sha256:d96a6a7d74af56feb11e9a443150216578ea07b7450f7c05df40eec90af7f4a7",
                 "sha256:dd0e3651d210068d13e18503d75aaa45656eef51ef0b261f891788589db2cc38",
                 "sha256:e167b9805de54367dcb2043519382be541117503ce99e3291cc9b41ca0a83557",
                 "sha256:e42029e184008a5fd3d819323345e25e2337b0ac7f5c135b7623308530209d57",
                 "sha256:f545c082eeb09ae678dd451a1b1dbf17babd8a0d7adea02897a76e639afca310",
                 "sha256:fde50062d67d805bc96f1a9ecc0d37bfc2a8f02b937d2c50824d186aa91f2419"
             ],
-            "markers": "python_version < '3.11' and python_version >= '3.7'",
+            "markers": "python_version < '3.10' and platform_machine != 'aarch64' and platform_machine != 'arm64'",
             "version": "==1.21.2"
         },
         "numpydoc": {
             "hashes": [
                 "sha256:c36fd6cb7ffdc9b4e165a43f67bf6271a7b024d0bb6b00ac468c9e2bfc76448e",
                 "sha256:c53d6311190b9e3b9285bc979390ba0257ba9acde5eca1a7065fc8dfca9d46e8"
             ],
@@ -372,38 +372,38 @@
                 "sha256:c86254f9220d55e31cc94d69bade760f0847da8000def4dfe1c6b872fd14ff14"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==21.0"
         },
         "pandas": {
             "hashes": [
-                "sha256:272c8cb14aa9793eada6b1ebe81994616e647b5892a370c7135efb2924b701df",
-                "sha256:3334a5a9eeaca953b9db1b2b165dcdc5180b5011f3bec3a57a3580c9c22eae68",
-                "sha256:37d63e78e87eb3791da7be4100a65da0383670c2b59e493d9e73098d7a879226",
-                "sha256:3f5020613c1d8e304840c34aeb171377dc755521bf5e69804991030c2a48aec3",
-                "sha256:45649503e167d45360aa7c52f18d1591a6d5c70d2f3a26bc90a3297a30ce9a66",
-                "sha256:49fd2889d8116d7acef0709e4c82b8560a8b22b0f77471391d12c27596e90267",
-                "sha256:4def2ef2fb7fcd62f2aa51bacb817ee9029e5c8efe42fe527ba21f6a3ddf1a9f",
-                "sha256:53e2fb11f86f6253bb1df26e3aeab3bf2e000aaa32a953ec394571bec5dc6fd6",
-                "sha256:629138b7cf81a2e55aa29ce7b04c1cece20485271d1f6c469c6a0c03857db6a4",
-                "sha256:68408a39a54ebadb9014ee5a4fae27b2fe524317bc80adf56c9ac59e8f8ea431",
-                "sha256:7326b37de08d42dd3fff5b7ef7691d0fd0bf2428f4ba5a2bdc3b3247e9a52e4c",
-                "sha256:7557b39c8e86eb0543a17a002ac1ea0f38911c3c17095bc9350d0a65b32d801c",
-                "sha256:86b16b1b920c4cb27fdd65a2c20258bcd9c794be491290660722bb0ea765054d",
-                "sha256:a800df4e101b721e94d04c355e611863cc31887f24c0b019572e26518cbbcab6",
-                "sha256:a9f1b54d7efc9df05320b14a48fb18686f781aa66cc7b47bb62fabfc67a0985c",
-                "sha256:c399200631db9bd9335d013ec7fce4edb98651035c249d532945c78ad453f23a",
-                "sha256:e574c2637c9d27f322e911650b36e858c885702c5996eda8a5a60e35e6648cf2",
-                "sha256:e9bc59855598cb57f68fdabd4897d3ed2bc3a3b3bef7b868a0153c4cd03f3207",
-                "sha256:ebbed7312547a924df0cbe133ff1250eeb94cdff3c09a794dc991c5621c8c735",
-                "sha256:ed2f29b4da6f6ae7c68f4b3708d9d9e59fa89b2f9e87c2b64ce055cbd39f729e",
-                "sha256:f7d84f321674c2f0f31887ee6d5755c54ca1ea5e144d6d54b3bbf566dd9ea0cc"
+                "sha256:003ba92db58b71a5f8add604a17a059f3068ef4e8c0c365b088468d0d64935fd",
+                "sha256:10e10a2527db79af6e830c3d5842a4d60383b162885270f8cffc15abca4ba4a9",
+                "sha256:22808afb8f96e2269dcc5b846decacb2f526dd0b47baebc63d913bf847317c8f",
+                "sha256:2d1dc09c0013d8faa7474574d61b575f9af6257ab95c93dcf33a14fd8d2c1bab",
+                "sha256:35c77609acd2e4d517da41bae0c11c70d31c87aae8dd1aabd2670906c6d2c143",
+                "sha256:372d72a3d8a5f2dbaf566a5fa5fa7f230842ac80f29a931fb4b071502cf86b9a",
+                "sha256:42493f8ae67918bf129869abea8204df899902287a7f5eaf596c8e54e0ac7ff4",
+                "sha256:5298a733e5bfbb761181fd4672c36d0c627320eb999c59c65156c6a90c7e1b4f",
+                "sha256:5ba0aac1397e1d7b654fccf263a4798a9e84ef749866060d19e577e927d66e1b",
+                "sha256:a2aa18d3f0b7d538e21932f637fbfe8518d085238b429e4790a35e1e44a96ffc",
+                "sha256:a388960f979665b447f0847626e40f99af8cf191bce9dc571d716433130cb3a7",
+                "sha256:a51528192755f7429c5bcc9e80832c517340317c861318fea9cea081b57c9afd",
+                "sha256:b528e126c13816a4374e56b7b18bfe91f7a7f6576d1aadba5dee6a87a7f479ae",
+                "sha256:c1aa4de4919358c5ef119f6377bc5964b3a7023c23e845d9db7d9016fa0c5b1c",
+                "sha256:c2646458e1dce44df9f71a01dc65f7e8fa4307f29e5c0f2f92c97f47a5bf22f5",
+                "sha256:d47750cf07dee6b55d8423471be70d627314277976ff2edd1381f02d52dbadf9",
+                "sha256:d99d2350adb7b6c3f7f8f0e5dfb7d34ff8dd4bc0a53e62c445b7e43e163fce63",
+                "sha256:dd324f8ee05925ee85de0ea3f0d66e1362e8c80799eb4eb04927d32335a3e44a",
+                "sha256:eaca36a80acaacb8183930e2e5ad7f71539a66805d6204ea88736570b2876a7b",
+                "sha256:f567e972dce3bbc3a8076e0b675273b4a9e8576ac629149cf8286ee13c259ae5",
+                "sha256:fe48e4925455c964db914b958f6e7032d285848b7538a5e1b19aeb26ffaea3ec"
             ],
             "index": "pypi",
-            "version": "==1.3.3"
+            "version": "==1.3.4"
         },
         "parso": {
             "hashes": [
                 "sha256:12b83492c6239ce32ff5eed6d3639d6a536170723c6f3f1506869f1ace413398",
                 "sha256:a8c4922db71e4fdb90e0d0bc6e50f9b273d3397925e5e60a717e719201778d22"
             ],
             "markers": "python_version >= '3.6'",
@@ -556,46 +556,50 @@
                 "sha256:3672058bc3453457b622aab7a1c3bfd5ab0bdae451512f6cf25f64ed37f5b87c",
                 "sha256:acad2d8b20a1af07d4e4c9d2e9285c5ed9104354062f275f3fcd88dcef4f1326"
             ],
             "version": "==2021.3"
         },
         "pyyaml": {
             "hashes": [
-                "sha256:08682f6b72c722394747bddaf0aa62277e02557c0fd1c42cb853016a38f8dedf",
-                "sha256:0f5f5786c0e09baddcd8b4b45f20a7b5d61a7e7e99846e3c799b05c7c53fa696",
-                "sha256:129def1b7c1bf22faffd67b8f3724645203b79d8f4cc81f674654d9902cb4393",
-                "sha256:294db365efa064d00b8d1ef65d8ea2c3426ac366c0c4368d930bf1c5fb497f77",
-                "sha256:3b2b1824fe7112845700f815ff6a489360226a5609b96ec2190a45e62a9fc922",
-                "sha256:3bd0e463264cf257d1ffd2e40223b197271046d09dadf73a0fe82b9c1fc385a5",
-                "sha256:4465124ef1b18d9ace298060f4eccc64b0850899ac4ac53294547536533800c8",
-                "sha256:49d4cdd9065b9b6e206d0595fee27a96b5dd22618e7520c33204a4a3239d5b10",
-                "sha256:4e0583d24c881e14342eaf4ec5fbc97f934b999a6828693a99157fde912540cc",
-                "sha256:5accb17103e43963b80e6f837831f38d314a0495500067cb25afab2e8d7a4018",
-                "sha256:607774cbba28732bfa802b54baa7484215f530991055bb562efbed5b2f20a45e",
-                "sha256:6c78645d400265a062508ae399b60b8c167bf003db364ecb26dcab2bda048253",
-                "sha256:72a01f726a9c7851ca9bfad6fd09ca4e090a023c00945ea05ba1638c09dc3347",
-                "sha256:74c1485f7707cf707a7aef42ef6322b8f97921bd89be2ab6317fd782c2d53183",
-                "sha256:895f61ef02e8fed38159bb70f7e100e00f471eae2bc838cd0f4ebb21e28f8541",
-                "sha256:8c1be557ee92a20f184922c7b6424e8ab6691788e6d86137c5d93c1a6ec1b8fb",
-                "sha256:bb4191dfc9306777bc594117aee052446b3fa88737cd13b7188d0e7aa8162185",
-                "sha256:bfb51918d4ff3d77c1c856a9699f8492c612cde32fd3bcd344af9be34999bfdc",
-                "sha256:c20cfa2d49991c8b4147af39859b167664f2ad4561704ee74c1de03318e898db",
-                "sha256:cb333c16912324fd5f769fff6bc5de372e9e7a202247b48870bc251ed40239aa",
-                "sha256:d2d9808ea7b4af864f35ea216be506ecec180628aced0704e34aca0b040ffe46",
-                "sha256:d483ad4e639292c90170eb6f7783ad19490e7a8defb3e46f97dfe4bacae89122",
-                "sha256:dd5de0646207f053eb0d6c74ae45ba98c3395a571a2891858e87df7c9b9bd51b",
-                "sha256:e1d4970ea66be07ae37a3c2e48b5ec63f7ba6804bdddfdbd3cfd954d25a82e63",
-                "sha256:e4fac90784481d221a8e4b1162afa7c47ed953be40d31ab4629ae917510051df",
-                "sha256:fa5ae20527d8e831e8230cbffd9f8fe952815b2b7dae6ffec25318803a7528fc",
-                "sha256:fd7f6999a8070df521b6384004ef42833b9bd62cfee11a09bda1079b4b704247",
-                "sha256:fdc842473cd33f45ff6bce46aea678a54e3d21f1b61a7750ce3c498eedfe25d6",
-                "sha256:fe69978f3f768926cfa37b867e3843918e012cf83f680806599ddce33c2c68b0"
+                "sha256:0283c35a6a9fbf047493e3a0ce8d79ef5030852c51e9d911a27badfde0605293",
+                "sha256:055d937d65826939cb044fc8c9b08889e8c743fdc6a32b33e2390f66013e449b",
+                "sha256:07751360502caac1c067a8132d150cf3d61339af5691fe9e87803040dbc5db57",
+                "sha256:0b4624f379dab24d3725ffde76559cff63d9ec94e1736b556dacdfebe5ab6d4b",
+                "sha256:0ce82d761c532fe4ec3f87fc45688bdd3a4c1dc5e0b4a19814b9009a29baefd4",
+                "sha256:1e4747bc279b4f613a09eb64bba2ba602d8a6664c6ce6396a4d0cd413a50ce07",
+                "sha256:213c60cd50106436cc818accf5baa1aba61c0189ff610f64f4a3e8c6726218ba",
+                "sha256:231710d57adfd809ef5d34183b8ed1eeae3f76459c18fb4a0b373ad56bedcdd9",
+                "sha256:277a0ef2981ca40581a47093e9e2d13b3f1fbbeffae064c1d21bfceba2030287",
+                "sha256:2cd5df3de48857ed0544b34e2d40e9fac445930039f3cfe4bcc592a1f836d513",
+                "sha256:40527857252b61eacd1d9af500c3337ba8deb8fc298940291486c465c8b46ec0",
+                "sha256:473f9edb243cb1935ab5a084eb238d842fb8f404ed2193a915d1784b5a6b5fc0",
+                "sha256:48c346915c114f5fdb3ead70312bd042a953a8ce5c7106d5bfb1a5254e47da92",
+                "sha256:50602afada6d6cbfad699b0c7bb50d5ccffa7e46a3d738092afddc1f9758427f",
+                "sha256:68fb519c14306fec9720a2a5b45bc9f0c8d1b9c72adf45c37baedfcd949c35a2",
+                "sha256:77f396e6ef4c73fdc33a9157446466f1cff553d979bd00ecb64385760c6babdc",
+                "sha256:819b3830a1543db06c4d4b865e70ded25be52a2e0631ccd2f6a47a2822f2fd7c",
+                "sha256:897b80890765f037df3403d22bab41627ca8811ae55e9a722fd0392850ec4d86",
+                "sha256:98c4d36e99714e55cfbaaee6dd5badbc9a1ec339ebfc3b1f52e293aee6bb71a4",
+                "sha256:9df7ed3b3d2e0ecfe09e14741b857df43adb5a3ddadc919a2d94fbdf78fea53c",
+                "sha256:9fa600030013c4de8165339db93d182b9431076eb98eb40ee068700c9c813e34",
+                "sha256:a80a78046a72361de73f8f395f1f1e49f956c6be882eed58505a15f3e430962b",
+                "sha256:b3d267842bf12586ba6c734f89d1f5b871df0273157918b0ccefa29deb05c21c",
+                "sha256:b5b9eccad747aabaaffbc6064800670f0c297e52c12754eb1d976c57e4f74dcb",
+                "sha256:c5687b8d43cf58545ade1fe3e055f70eac7a5a1a0bf42824308d868289a95737",
+                "sha256:cba8c411ef271aa037d7357a2bc8f9ee8b58b9965831d9e51baf703280dc73d3",
+                "sha256:d15a181d1ecd0d4270dc32edb46f7cb7733c7c508857278d3d378d14d606db2d",
+                "sha256:d4db7c7aef085872ef65a8fd7d6d09a14ae91f691dec3e87ee5ee0539d516f53",
+                "sha256:d4eccecf9adf6fbcc6861a38015c2a64f38b9d94838ac1810a9023a0609e1b78",
+                "sha256:d67d839ede4ed1b28a4e8909735fc992a923cdb84e618544973d7dfc71540803",
+                "sha256:daf496c58a8c52083df09b80c860005194014c3698698d1a57cbcfa182142a3a",
+                "sha256:e61ceaab6f49fb8bdfaa0f92c4b57bcfbea54c09277b1b4f7ac376bfb7a7c174",
+                "sha256:f84fbc98b019fef2ee9a1cb3ce93e3187a6df0b2538a651bfb890254ba9f90b5"
             ],
             "index": "pypi",
-            "version": "==5.4.1"
+            "version": "==6.0"
         },
         "readme-renderer": {
             "hashes": [
                 "sha256:3286806450d9961d6e3b5f8a59f77e61503799aca5155c8d8d40359b4e1e1adc",
                 "sha256:8299700d7a910c304072a7601eafada6712a5b011a20139417e1b1e9f04645d8"
             ],
             "version": "==30.0"
```

### Comparing `v3io_frames-0.9.5/README.md` & `v3io_frames-0.9.6/README.md`

 * *Files identical despite different names*

### Comparing `v3io_frames-0.9.5/setup.py` & `v3io_frames-0.9.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,48 +21,40 @@
 def version():
     with open('v3io_frames/__init__.py') as fp:
         for line in fp:
             if '__version__' in line:
                 _, version = line.split('=')
                 return version.replace("'", '').strip()
 
-
-def load_deps(section):
-    """Load dependencies from Pipfile, we can't assume toml is installed"""
-    # [packages]
-    header = '[{}]'.format(section)
-    with open('Pipfile') as fp:
-        in_section = False
+def is_ignored(line):
+    line = line.strip()
+    return (not line) or (line[0] == "#")
+
+def load_deps(path):
+    """Load dependencies from requirements file"""
+    with open(path) as fp:
+        deps = []
         for line in fp:
-            line = line.strip()
-            if not line:
-                continue
-
-            if line == header:
-                in_section = True
+            if is_ignored(line):
                 continue
+            line = line.strip()
 
-            if line.startswith('['):
-                in_section = False
+            # e.g.: git+https://github.com/nuclio/nuclio-jupyter.git@some-branch#egg=nuclio-jupyter
+            if "#egg=" in line:
+                _, package = line.split("#egg=")
+                deps.append(f"{package} @ {line}")
                 continue
 
-            if in_section:
-                # ipython = ">=6.5"
-                i = line.find('=')
-                assert i != -1, 'bad dependency - {}'.format(line)
-                pkg = line[:i].strip()
-                version = line[i+1:].strip().replace('"', '')
-                if version == '*':
-                    yield pkg
-                else:
-                    yield '{}{}'.format(pkg, version.replace('"', ''))
+            # append package
+            deps.append(line)
+        return deps
 
 
-install_requires = list(load_deps('packages'))
-tests_require = list(load_deps('dev-packages'))
+install_requires = load_deps('requirements.txt')
+tests_require = load_deps('dev-requirements.txt')
 
 with open('README.md') as fp:
     long_desc = fp.read()
 
 
 setup(
     name='v3io_frames',
```

### Comparing `v3io_frames-0.9.5/tests/conftest.py` & `v3io_frames-0.9.6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `v3io_frames-0.9.5/tests/pip_docker.py` & `v3io_frames-0.9.6/tests/pip_docker.py`

 * *Files identical despite different names*

### Comparing `v3io_frames-0.9.5/tests/test_benchmark.py` & `v3io_frames-0.9.6/tests/test_benchmark.py`

 * *Files identical despite different names*

### Comparing `v3io_frames-0.9.5/tests/test_client.py` & `v3io_frames-0.9.6/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `v3io_frames-0.9.5/tests/test_concurrent.py` & `v3io_frames-0.9.6/tests/test_concurrent.py`

 * *Files identical despite different names*

### Comparing `v3io_frames-0.9.5/tests/test_cudf.py` & `v3io_frames-0.9.6/tests/test_cudf.py`

 * *Files identical despite different names*

### Comparing `v3io_frames-0.9.5/tests/test_http.py` & `v3io_frames-0.9.6/tests/test_http.py`

 * *Files identical despite different names*

### Comparing `v3io_frames-0.9.5/tests/test_integration.py` & `v3io_frames-0.9.6/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `v3io_frames-0.9.5/tests/test_pbutils.py` & `v3io_frames-0.9.6/tests/test_pbutils.py`

 * *Files identical despite different names*

### Comparing `v3io_frames-0.9.5/tests/test_pdutils.py` & `v3io_frames-0.9.6/tests/test_pdutils.py`

 * *Files identical despite different names*

### Comparing `v3io_frames-0.9.5/tests/test_pip_docker.py` & `v3io_frames-0.9.6/tests/test_pip_docker.py`

 * *Files identical despite different names*

### Comparing `v3io_frames-0.9.5/tests/test_v3io_frames.py` & `v3io_frames-0.9.6/tests/test_v3io_frames.py`

 * *Files identical despite different names*

### Comparing `v3io_frames-0.9.5/tests/weather.csv` & `v3io_frames-0.9.6/tests/weather.csv`

 * *Files identical despite different names*

### Comparing `v3io_frames-0.9.5/v3io_frames/__init__.py` & `v3io_frames-0.9.6/v3io_frames/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Stream data from/to Nuclio into pandas DataFrame"""
 
-__version__ = '0.9.5'
+__version__ = '0.9.6'
 
 import json
 import pandas as pd
 from os import environ
 from urllib.parse import urlparse
 
 from .errors import *  # noqa
```

### Comparing `v3io_frames-0.9.5/v3io_frames/client.py` & `v3io_frames-0.9.6/v3io_frames/client.py`

 * *Files identical despite different names*

### Comparing `v3io_frames-0.9.5/v3io_frames/dtypes.py` & `v3io_frames-0.9.6/v3io_frames/dtypes.py`

 * *Files identical despite different names*

### Comparing `v3io_frames-0.9.5/v3io_frames/errors.py` & `v3io_frames-0.9.6/v3io_frames/errors.py`

 * *Files identical despite different names*

### Comparing `v3io_frames-0.9.5/v3io_frames/frames_pb2.py` & `v3io_frames-0.9.6/v3io_frames/frames_pb2.py`

 * *Files identical despite different names*

### Comparing `v3io_frames-0.9.5/v3io_frames/frames_pb2_grpc.py` & `v3io_frames-0.9.6/v3io_frames/frames_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `v3io_frames-0.9.5/v3io_frames/grpc.py` & `v3io_frames-0.9.6/v3io_frames/grpc.py`

 * *Files identical despite different names*

### Comparing `v3io_frames-0.9.5/v3io_frames/http.py` & `v3io_frames-0.9.6/v3io_frames/http.py`

 * *Files identical despite different names*

### Comparing `v3io_frames-0.9.5/v3io_frames/pbutils.py` & `v3io_frames-0.9.6/v3io_frames/pbutils.py`

 * *Files identical despite different names*

### Comparing `v3io_frames-0.9.5/v3io_frames/pdutils.py` & `v3io_frames-0.9.6/v3io_frames/pdutils.py`

 * *Files identical despite different names*

### Comparing `v3io_frames-0.9.5/v3io_frames.egg-info/PKG-INFO` & `v3io_frames-0.9.6/v3io_frames.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: v3io-frames
-Version: 0.9.5
+Version: 0.9.6
 Summary: Unified multi-module DataFrames client for the Iguazio Data Science Platform
 Home-page: https://github.com/v3io/frames
 Author: Miki Tebeka
 Author-email: miki@353solutions.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `v3io_frames-0.9.5/v3io_frames.egg-info/SOURCES.txt` & `v3io_frames-0.9.6/v3io_frames.egg-info/SOURCES.txt`

 * *Files identical despite different names*

