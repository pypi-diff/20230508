# Comparing `tmp/dlhpcstarter-0.1.2.tar.gz` & `tmp/dlhpcstarter-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dlhpcstarter-0.1.2.tar", last modified: Wed Apr 26 05:06:12 2023, max compression
+gzip compressed data, was "/datasets/work/hb-mlaifsp-mm/work/repositories/dl_hpc_starter_pack/dist/tmp8uxa9cy0/dlhpcstarter-0.1.3.tar", last modified: Mon May  8 01:22:39 2023, max compression
```

## Comparing `dlhpcstarter-0.1.2.tar` & `dlhpcstarter-0.1.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 nic261   (1140141) hpc-users (319125)        0 2023-04-26 05:06:12.674746 dlhpcstarter-0.1.2/
--rw-r--r--   0 nic261   (1140141) hpc-users (319125)    11558 2023-03-30 09:11:54.000000 dlhpcstarter-0.1.2/LICENSE
--rw-r--r--   0 nic261   (1140141) hpc-users (319125)    25268 2023-04-26 05:06:12.675801 dlhpcstarter-0.1.2/PKG-INFO
--rw-r--r--   0 nic261   (1140141) hpc-users (319125)    25540 2023-03-30 09:11:54.000000 dlhpcstarter-0.1.2/README.md
--rw-r--r--   0 nic261   (1140141) hpc-users (319125)       84 2023-03-30 09:11:54.000000 dlhpcstarter-0.1.2/pyproject.toml
--rw-r--r--   0 nic261   (1140141) hpc-users (319125)      807 2023-04-26 05:06:12.678741 dlhpcstarter-0.1.2/setup.cfg
--rw-r--r--   0 nic261   (1140141) hpc-users (319125)       96 2023-03-30 09:11:54.000000 dlhpcstarter-0.1.2/setup.py
-drwxr-xr-x   0 nic261   (1140141) hpc-users (319125)        0 2023-04-26 05:06:12.081478 dlhpcstarter-0.1.2/src/
-drwxr-xr-x   0 nic261   (1140141) hpc-users (319125)        0 2023-04-26 05:06:12.343139 dlhpcstarter-0.1.2/src/dlhpcstarter/
--rw-r--r--   0 nic261   (1140141) hpc-users (319125)        0 2022-09-08 10:09:36.000000 dlhpcstarter-0.1.2/src/dlhpcstarter/__init__.py
--rw-r--r--   0 nic261   (1140141) hpc-users (319125)     4612 2023-04-23 22:41:30.000000 dlhpcstarter-0.1.2/src/dlhpcstarter/__main__.py
--rw-r--r--   0 nic261   (1140141) hpc-users (319125)     9743 2023-04-23 21:42:40.000000 dlhpcstarter-0.1.2/src/dlhpcstarter/cluster.py
--rw-r--r--   0 nic261   (1140141) hpc-users (319125)     5681 2023-04-23 21:40:40.000000 dlhpcstarter-0.1.2/src/dlhpcstarter/command_line_arguments.py
-drwxr-xr-x   0 nic261   (1140141) hpc-users (319125)        0 2023-04-26 05:06:12.602478 dlhpcstarter-0.1.2/src/dlhpcstarter/tools/
--rw-r--r--   0 nic261   (1140141) hpc-users (319125)        0 2022-09-08 10:09:36.000000 dlhpcstarter-0.1.2/src/dlhpcstarter/tools/__init__.py
-drwxr-xr-x   0 nic261   (1140141) hpc-users (319125)        0 2023-04-26 05:06:12.640087 dlhpcstarter-0.1.2/src/dlhpcstarter/tools/ext/
--rw-r--r--   0 nic261   (1140141) hpc-users (319125)        0 2022-09-08 10:09:36.000000 dlhpcstarter-0.1.2/src/dlhpcstarter/tools/ext/__init__.py
--rw-r--r--   0 nic261   (1140141) hpc-users (319125)     3215 2023-04-16 23:14:24.000000 dlhpcstarter-0.1.2/src/dlhpcstarter/tools/ext/collect_env_details.py
-drwxr-xr-x   0 nic261   (1140141) hpc-users (319125)        0 2023-04-26 05:06:12.654293 dlhpcstarter-0.1.2/src/dlhpcstarter/tools/mods/
--rw-r--r--   0 nic261   (1140141) hpc-users (319125)        0 2022-09-08 10:09:36.000000 dlhpcstarter-0.1.2/src/dlhpcstarter/tools/mods/__init__.py
--rw-r--r--   0 nic261   (1140141) hpc-users (319125)     8505 2023-03-30 09:11:54.000000 dlhpcstarter-0.1.2/src/dlhpcstarter/tools/mods/logger.py
--rw-r--r--   0 nic261   (1140141) hpc-users (319125)     9793 2023-04-26 01:07:26.000000 dlhpcstarter-0.1.2/src/dlhpcstarter/trainer.py
--rw-r--r--   0 nic261   (1140141) hpc-users (319125)    11503 2023-04-24 00:26:55.000000 dlhpcstarter-0.1.2/src/dlhpcstarter/utils.py
-drwxr-xr-x   0 nic261   (1140141) hpc-users (319125)        0 2023-04-26 05:06:12.407275 dlhpcstarter-0.1.2/src/dlhpcstarter.egg-info/
--rw-r--r--   0 nic261   (1140141) hpc-users (319125)    25268 2023-04-26 05:06:11.000000 dlhpcstarter-0.1.2/src/dlhpcstarter.egg-info/PKG-INFO
--rw-r--r--   0 nic261   (1140141) hpc-users (319125)      678 2023-04-26 05:06:12.000000 dlhpcstarter-0.1.2/src/dlhpcstarter.egg-info/SOURCES.txt
--rw-r--r--   0 nic261   (1140141) hpc-users (319125)        1 2023-04-26 05:06:11.000000 dlhpcstarter-0.1.2/src/dlhpcstarter.egg-info/dependency_links.txt
--rw-r--r--   0 nic261   (1140141) hpc-users (319125)       60 2023-04-26 05:06:11.000000 dlhpcstarter-0.1.2/src/dlhpcstarter.egg-info/entry_points.txt
--rw-r--r--   0 nic261   (1140141) hpc-users (319125)      201 2023-04-26 05:06:12.000000 dlhpcstarter-0.1.2/src/dlhpcstarter.egg-info/requires.txt
--rw-r--r--   0 nic261   (1140141) hpc-users (319125)       13 2023-04-26 05:06:12.000000 dlhpcstarter-0.1.2/src/dlhpcstarter.egg-info/top_level.txt
+drwxr-xr-x   0 nic261   (1140141) hpc-users (319125)        0 2023-05-08 01:22:39.000000 dlhpcstarter-0.1.3/
+-rw-r--r--   0 nic261   (1140141) hpc-users (319125)    11558 2023-03-30 09:11:54.000000 dlhpcstarter-0.1.3/LICENSE
+-rw-r--r--   0 nic261   (1140141) hpc-users (319125)    25288 2023-05-08 01:22:39.000000 dlhpcstarter-0.1.3/PKG-INFO
+-rw-r--r--   0 nic261   (1140141) hpc-users (319125)    25540 2023-03-30 09:11:54.000000 dlhpcstarter-0.1.3/README.md
+-rw-r--r--   0 nic261   (1140141) hpc-users (319125)       84 2023-03-30 09:11:54.000000 dlhpcstarter-0.1.3/pyproject.toml
+-rw-r--r--   0 nic261   (1140141) hpc-users (319125)      807 2023-05-08 01:22:39.000000 dlhpcstarter-0.1.3/setup.cfg
+-rw-r--r--   0 nic261   (1140141) hpc-users (319125)       96 2023-03-30 09:11:54.000000 dlhpcstarter-0.1.3/setup.py
+drwxr-xr-x   0 nic261   (1140141) hpc-users (319125)        0 2023-05-08 01:22:39.000000 dlhpcstarter-0.1.3/src/
+drwxr-xr-x   0 nic261   (1140141) hpc-users (319125)        0 2023-05-08 01:22:39.000000 dlhpcstarter-0.1.3/src/dlhpcstarter/
+-rw-r--r--   0 nic261   (1140141) hpc-users (319125)        0 2022-09-08 10:09:36.000000 dlhpcstarter-0.1.3/src/dlhpcstarter/__init__.py
+-rw-r--r--   0 nic261   (1140141) hpc-users (319125)     4612 2023-04-23 22:41:30.000000 dlhpcstarter-0.1.3/src/dlhpcstarter/__main__.py
+-rw-r--r--   0 nic261   (1140141) hpc-users (319125)     9743 2023-04-23 21:42:40.000000 dlhpcstarter-0.1.3/src/dlhpcstarter/cluster.py
+-rw-r--r--   0 nic261   (1140141) hpc-users (319125)     5681 2023-04-23 21:40:40.000000 dlhpcstarter-0.1.3/src/dlhpcstarter/command_line_arguments.py
+drwxr-xr-x   0 nic261   (1140141) hpc-users (319125)        0 2023-05-08 01:22:39.000000 dlhpcstarter-0.1.3/src/dlhpcstarter/tools/
+-rw-r--r--   0 nic261   (1140141) hpc-users (319125)        0 2022-09-08 10:09:36.000000 dlhpcstarter-0.1.3/src/dlhpcstarter/tools/__init__.py
+drwxr-xr-x   0 nic261   (1140141) hpc-users (319125)        0 2023-05-08 01:22:39.000000 dlhpcstarter-0.1.3/src/dlhpcstarter/tools/ext/
+-rw-r--r--   0 nic261   (1140141) hpc-users (319125)        0 2022-09-08 10:09:36.000000 dlhpcstarter-0.1.3/src/dlhpcstarter/tools/ext/__init__.py
+-rw-r--r--   0 nic261   (1140141) hpc-users (319125)     3215 2023-04-16 23:14:24.000000 dlhpcstarter-0.1.3/src/dlhpcstarter/tools/ext/collect_env_details.py
+drwxr-xr-x   0 nic261   (1140141) hpc-users (319125)        0 2023-05-08 01:22:39.000000 dlhpcstarter-0.1.3/src/dlhpcstarter/tools/mods/
+-rw-r--r--   0 nic261   (1140141) hpc-users (319125)        0 2022-09-08 10:09:36.000000 dlhpcstarter-0.1.3/src/dlhpcstarter/tools/mods/__init__.py
+-rw-r--r--   0 nic261   (1140141) hpc-users (319125)     8505 2023-03-30 09:11:54.000000 dlhpcstarter-0.1.3/src/dlhpcstarter/tools/mods/logger.py
+-rw-r--r--   0 nic261   (1140141) hpc-users (319125)     9793 2023-04-26 01:07:26.000000 dlhpcstarter-0.1.3/src/dlhpcstarter/trainer.py
+-rw-r--r--   0 nic261   (1140141) hpc-users (319125)    11503 2023-04-24 00:26:55.000000 dlhpcstarter-0.1.3/src/dlhpcstarter/utils.py
+drwxr-xr-x   0 nic261   (1140141) hpc-users (319125)        0 2023-05-08 01:22:39.000000 dlhpcstarter-0.1.3/src/dlhpcstarter.egg-info/
+-rw-r--r--   0 nic261   (1140141) hpc-users (319125)    25288 2023-05-08 01:22:39.000000 dlhpcstarter-0.1.3/src/dlhpcstarter.egg-info/PKG-INFO
+-rw-r--r--   0 nic261   (1140141) hpc-users (319125)      678 2023-05-08 01:22:39.000000 dlhpcstarter-0.1.3/src/dlhpcstarter.egg-info/SOURCES.txt
+-rw-r--r--   0 nic261   (1140141) hpc-users (319125)        1 2023-05-08 01:22:39.000000 dlhpcstarter-0.1.3/src/dlhpcstarter.egg-info/dependency_links.txt
+-rw-r--r--   0 nic261   (1140141) hpc-users (319125)       61 2023-05-08 01:22:39.000000 dlhpcstarter-0.1.3/src/dlhpcstarter.egg-info/entry_points.txt
+-rw-r--r--   0 nic261   (1140141) hpc-users (319125)      201 2023-05-08 01:22:39.000000 dlhpcstarter-0.1.3/src/dlhpcstarter.egg-info/requires.txt
+-rw-r--r--   0 nic261   (1140141) hpc-users (319125)       13 2023-05-08 01:22:39.000000 dlhpcstarter-0.1.3/src/dlhpcstarter.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `dlhpcstarter-0.1.2/LICENSE` & `dlhpcstarter-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dlhpcstarter-0.1.2/PKG-INFO` & `dlhpcstarter-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: dlhpcstarter
-Version: 0.1.2
+Version: 0.1.3
 Summary: Deep Learning and HPC Starter Pack
 Home-page: https://github.com/csiro-mlai/dl_hpc_starter_pack
 Author: CSIRO
 License: Apache License 2.0
+Platform: UNKNOWN
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8
 Provides-Extra: test
 License-File: LICENSE
 
 ![](/assets/image.png)
 
@@ -603,7 +604,9 @@
 ---
 - Transfer cluster management over to submitit: https://ai.facebook.com/blog/open-sourcing-submitit-a-lightweight-tool-for-slurm-cluster-computation/
 - Add description about how to use https://neptune.ai/.
 - Use https://hydra.cc/ instead of argparse (or have the option to use either).
 - https://docs.ray.io/en/latest/tune/index.html for hyperparameter optimisation.
 - Notebook examples.
 
+
+
```

### Comparing `dlhpcstarter-0.1.2/README.md` & `dlhpcstarter-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `dlhpcstarter-0.1.2/setup.cfg` & `dlhpcstarter-0.1.3/setup.cfg`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = dlhpcstarter
-version = 0.1.2
+version = 0.1.3
 description = Deep Learning and HPC Starter Pack
 long_description = file: README.md
 long_description_content_type = text/markdown; charset=UTF-8
 url = https://github.com/csiro-mlai/dl_hpc_starter_pack
 author = CSIRO
 license = Apache License 2.0
 license_file = LICENSE
@@ -16,15 +16,15 @@
 python_requires = >=3.7
 install_requires = 
 	Bottleneck>=1.3.7
 	GPUtil>=1.4
 	hydra-core>=1.3.2
 	lightning>=2.0.1
 	neptune-client==0.16.18
-	numpy>=1.24.2
+	numpy==1.23.5
 	protobuf==3.20.3
 	rich>=13.3.2
 	tensorboard>=2.12.0
 	torch>=1.11
 	torchmetrics>=0.11.4
 
 [options.extras_require]
```

### Comparing `dlhpcstarter-0.1.2/src/dlhpcstarter/__main__.py` & `dlhpcstarter-0.1.3/src/dlhpcstarter/__main__.py`

 * *Files identical despite different names*

### Comparing `dlhpcstarter-0.1.2/src/dlhpcstarter/cluster.py` & `dlhpcstarter-0.1.3/src/dlhpcstarter/cluster.py`

 * *Files identical despite different names*

### Comparing `dlhpcstarter-0.1.2/src/dlhpcstarter/command_line_arguments.py` & `dlhpcstarter-0.1.3/src/dlhpcstarter/command_line_arguments.py`

 * *Files identical despite different names*

### Comparing `dlhpcstarter-0.1.2/src/dlhpcstarter/tools/ext/collect_env_details.py` & `dlhpcstarter-0.1.3/src/dlhpcstarter/tools/ext/collect_env_details.py`

 * *Files identical despite different names*

### Comparing `dlhpcstarter-0.1.2/src/dlhpcstarter/tools/mods/logger.py` & `dlhpcstarter-0.1.3/src/dlhpcstarter/tools/mods/logger.py`

 * *Files identical despite different names*

### Comparing `dlhpcstarter-0.1.2/src/dlhpcstarter/trainer.py` & `dlhpcstarter-0.1.3/src/dlhpcstarter/trainer.py`

 * *Files identical despite different names*

### Comparing `dlhpcstarter-0.1.2/src/dlhpcstarter/utils.py` & `dlhpcstarter-0.1.3/src/dlhpcstarter/utils.py`

 * *Files identical despite different names*

### Comparing `dlhpcstarter-0.1.2/src/dlhpcstarter.egg-info/PKG-INFO` & `dlhpcstarter-0.1.3/src/dlhpcstarter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: dlhpcstarter
-Version: 0.1.2
+Version: 0.1.3
 Summary: Deep Learning and HPC Starter Pack
 Home-page: https://github.com/csiro-mlai/dl_hpc_starter_pack
 Author: CSIRO
 License: Apache License 2.0
+Platform: UNKNOWN
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8
 Provides-Extra: test
 License-File: LICENSE
 
 ![](/assets/image.png)
 
@@ -603,7 +604,9 @@
 ---
 - Transfer cluster management over to submitit: https://ai.facebook.com/blog/open-sourcing-submitit-a-lightweight-tool-for-slurm-cluster-computation/
 - Add description about how to use https://neptune.ai/.
 - Use https://hydra.cc/ instead of argparse (or have the option to use either).
 - https://docs.ray.io/en/latest/tune/index.html for hyperparameter optimisation.
 - Notebook examples.
 
+
+
```

### Comparing `dlhpcstarter-0.1.2/src/dlhpcstarter.egg-info/SOURCES.txt` & `dlhpcstarter-0.1.3/src/dlhpcstarter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

