# Comparing `tmp/oqtant-0.14.1.tar.gz` & `tmp/oqtant-0.14.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oqtant-0.14.1.tar", max compression
+gzip compressed data, was "oqtant-0.14.2.tar", max compression
```

## Comparing `oqtant-0.14.1.tar` & `oqtant-0.14.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0    11341 2023-01-20 21:46:26.574896 oqtant-0.14.1/LICENSE
--rw-r--r--   0        0        0     1959 2023-05-08 15:43:28.092934 oqtant-0.14.1/README.md
--rw-r--r--   0        0        0     8556 2023-05-05 20:25:04.057852 oqtant-0.14.1/documentation/INSTALL.md
--rw-r--r--   0        0        0     4436 2023-05-05 20:25:04.057852 oqtant-0.14.1/documentation/albert_api_docs.md
--rw-r--r--   0        0        0    10947 2023-05-05 20:25:04.057852 oqtant-0.14.1/documentation/job_analysis_docs.md
--rw-r--r--   0        0        0    26364 2023-05-02 19:38:25.421229 oqtant-0.14.1/documentation/main.css
--rw-r--r--   0        0        0    10316 2023-05-05 20:25:04.057852 oqtant-0.14.1/documentation/oqtant_api_docs.md
--rw-r--r--   0        0        0    15152 2023-05-05 20:25:04.057852 oqtant-0.14.1/documentation/tutorials/tutorial_1_bec_jobs.ipynb
--rw-r--r--   0        0        0     9895 2023-05-05 20:25:04.057852 oqtant-0.14.1/documentation/tutorials/tutorial_1_bec_jobs.md
--rw-r--r--   0        0        0    14537 2023-05-05 20:25:04.057852 oqtant-0.14.1/documentation/tutorials/tutorial_2_barrier_jobs.ipynb
--rw-r--r--   0        0        0     9553 2023-05-05 20:25:04.057852 oqtant-0.14.1/documentation/tutorials/tutorial_2_barrier_jobs.md
--rw-r--r--   0        0        0    31799 2023-05-05 20:25:04.057852 oqtant-0.14.1/documentation/tutorials/tutorial_3_abstractions.ipynb
--rw-r--r--   0        0        0    21970 2023-05-05 20:25:04.057852 oqtant-0.14.1/documentation/tutorials/tutorial_3_abstractions.md
--rw-r--r--   0        0        0    13266 2023-05-05 20:25:04.057852 oqtant-0.14.1/documentation/tutorials/tutorial_4_experiment.ipynb
--rw-r--r--   0        0        0     9097 2023-05-05 20:25:04.057852 oqtant-0.14.1/documentation/tutorials/tutorial_4_experiment.md
--rw-r--r--   0        0        0    16999 2023-05-05 20:25:04.057852 oqtant-0.14.1/documentation/tutorials/tutorial_5_optimization.ipynb
--rw-r--r--   0        0        0    11308 2023-05-05 20:25:04.057852 oqtant-0.14.1/documentation/tutorials/tutorial_5_optimization.md
--rw-r--r--   0        0        0      463 2023-05-04 14:03:20.362947 oqtant-0.14.1/documentation/tutorials/tutorials.md
--rw-r--r--   0        0        0        0 2023-05-05 20:25:04.057852 oqtant-0.14.1/oqtant/__init__.py
--rw-r--r--   0        0        0    21848 2023-05-08 14:41:12.223285 oqtant-0.14.1/oqtant/oqtant_client.py
--rw-r--r--   0        0        0        0 2023-05-05 20:25:04.057852 oqtant-0.14.1/oqtant/schemas/__init__.py
--rw-r--r--   0        0        0    17813 2023-05-05 20:25:04.061852 oqtant-0.14.1/oqtant/schemas/job.py
--rw-r--r--   0        0        0     1002 2023-05-05 20:25:04.061852 oqtant-0.14.1/oqtant/settings.py
--rw-r--r--   0        0        0        0 2023-05-05 20:25:04.061852 oqtant-0.14.1/oqtant/util/__init__.py
--rw-r--r--   0        0        0     2805 2023-05-05 20:25:04.061852 oqtant-0.14.1/oqtant/util/auth.py
--rw-r--r--   0        0        0     1023 2023-05-08 14:41:12.223285 oqtant-0.14.1/oqtant/util/exceptions.py
--rw-r--r--   0        0        0      474 2023-05-05 20:25:04.061852 oqtant-0.14.1/oqtant/util/server.py
--rw-r--r--   0        0        0     3181 2023-05-08 15:39:25.048538 oqtant-0.14.1/pyproject.toml
--rw-r--r--   0        0        0     3197 1970-01-01 00:00:00.000000 oqtant-0.14.1/PKG-INFO
+-rw-r--r--   0        0        0    11341 2023-01-20 21:46:26.574896 oqtant-0.14.2/LICENSE
+-rw-r--r--   0        0        0     2434 2023-05-08 19:04:48.398282 oqtant-0.14.2/README.md
+-rw-r--r--   0        0        0     8556 2023-05-05 20:25:04.057852 oqtant-0.14.2/documentation/INSTALL.md
+-rw-r--r--   0        0        0     4436 2023-05-05 20:25:04.057852 oqtant-0.14.2/documentation/albert_api_docs.md
+-rw-r--r--   0        0        0    10947 2023-05-05 20:25:04.057852 oqtant-0.14.2/documentation/job_analysis_docs.md
+-rw-r--r--   0        0        0    26364 2023-05-02 19:38:25.421229 oqtant-0.14.2/documentation/main.css
+-rw-r--r--   0        0        0    10316 2023-05-05 20:25:04.057852 oqtant-0.14.2/documentation/oqtant_api_docs.md
+-rw-r--r--   0        0        0    15152 2023-05-05 20:25:04.057852 oqtant-0.14.2/documentation/tutorials/tutorial_1_bec_jobs.ipynb
+-rw-r--r--   0        0        0     9895 2023-05-05 20:25:04.057852 oqtant-0.14.2/documentation/tutorials/tutorial_1_bec_jobs.md
+-rw-r--r--   0        0        0    14537 2023-05-05 20:25:04.057852 oqtant-0.14.2/documentation/tutorials/tutorial_2_barrier_jobs.ipynb
+-rw-r--r--   0        0        0     9553 2023-05-05 20:25:04.057852 oqtant-0.14.2/documentation/tutorials/tutorial_2_barrier_jobs.md
+-rw-r--r--   0        0        0    31799 2023-05-05 20:25:04.057852 oqtant-0.14.2/documentation/tutorials/tutorial_3_abstractions.ipynb
+-rw-r--r--   0        0        0    21970 2023-05-05 20:25:04.057852 oqtant-0.14.2/documentation/tutorials/tutorial_3_abstractions.md
+-rw-r--r--   0        0        0    13266 2023-05-05 20:25:04.057852 oqtant-0.14.2/documentation/tutorials/tutorial_4_experiment.ipynb
+-rw-r--r--   0        0        0     9097 2023-05-05 20:25:04.057852 oqtant-0.14.2/documentation/tutorials/tutorial_4_experiment.md
+-rw-r--r--   0        0        0    16999 2023-05-05 20:25:04.057852 oqtant-0.14.2/documentation/tutorials/tutorial_5_optimization.ipynb
+-rw-r--r--   0        0        0    11308 2023-05-05 20:25:04.057852 oqtant-0.14.2/documentation/tutorials/tutorial_5_optimization.md
+-rw-r--r--   0        0        0      463 2023-05-04 14:03:20.362947 oqtant-0.14.2/documentation/tutorials/tutorials.md
+-rw-r--r--   0        0        0        0 2023-05-05 20:25:04.057852 oqtant-0.14.2/oqtant/__init__.py
+-rw-r--r--   0        0        0    21848 2023-05-08 14:41:12.223285 oqtant-0.14.2/oqtant/oqtant_client.py
+-rw-r--r--   0        0        0        0 2023-05-05 20:25:04.057852 oqtant-0.14.2/oqtant/schemas/__init__.py
+-rw-r--r--   0        0        0    17813 2023-05-05 20:25:04.061852 oqtant-0.14.2/oqtant/schemas/job.py
+-rw-r--r--   0        0        0     1002 2023-05-05 20:25:04.061852 oqtant-0.14.2/oqtant/settings.py
+-rw-r--r--   0        0        0        0 2023-05-05 20:25:04.061852 oqtant-0.14.2/oqtant/util/__init__.py
+-rw-r--r--   0        0        0     2805 2023-05-05 20:25:04.061852 oqtant-0.14.2/oqtant/util/auth.py
+-rw-r--r--   0        0        0     1023 2023-05-08 14:41:12.223285 oqtant-0.14.2/oqtant/util/exceptions.py
+-rw-r--r--   0        0        0      474 2023-05-05 20:25:04.061852 oqtant-0.14.2/oqtant/util/server.py
+-rw-r--r--   0        0        0     3181 2023-05-08 19:05:24.786316 oqtant-0.14.2/pyproject.toml
+-rw-r--r--   0        0        0     3672 1970-01-01 00:00:00.000000 oqtant-0.14.2/PKG-INFO
```

### Comparing `oqtant-0.14.1/LICENSE` & `oqtant-0.14.2/LICENSE`

 * *Files identical despite different names*

### Comparing `oqtant-0.14.1/documentation/INSTALL.md` & `oqtant-0.14.2/documentation/INSTALL.md`

 * *Files identical despite different names*

### Comparing `oqtant-0.14.1/documentation/albert_api_docs.md` & `oqtant-0.14.2/documentation/albert_api_docs.md`

 * *Files identical despite different names*

### Comparing `oqtant-0.14.1/documentation/job_analysis_docs.md` & `oqtant-0.14.2/documentation/job_analysis_docs.md`

 * *Files identical despite different names*

### Comparing `oqtant-0.14.1/documentation/main.css` & `oqtant-0.14.2/documentation/main.css`

 * *Files identical despite different names*

### Comparing `oqtant-0.14.1/documentation/oqtant_api_docs.md` & `oqtant-0.14.2/documentation/oqtant_api_docs.md`

 * *Files identical despite different names*

### Comparing `oqtant-0.14.1/documentation/tutorials/tutorial_1_bec_jobs.ipynb` & `oqtant-0.14.2/documentation/tutorials/tutorial_1_bec_jobs.ipynb`

 * *Files identical despite different names*

### Comparing `oqtant-0.14.1/documentation/tutorials/tutorial_1_bec_jobs.md` & `oqtant-0.14.2/documentation/tutorials/tutorial_1_bec_jobs.md`

 * *Files identical despite different names*

### Comparing `oqtant-0.14.1/documentation/tutorials/tutorial_2_barrier_jobs.ipynb` & `oqtant-0.14.2/documentation/tutorials/tutorial_2_barrier_jobs.ipynb`

 * *Files identical despite different names*

### Comparing `oqtant-0.14.1/documentation/tutorials/tutorial_2_barrier_jobs.md` & `oqtant-0.14.2/documentation/tutorials/tutorial_2_barrier_jobs.md`

 * *Files identical despite different names*

### Comparing `oqtant-0.14.1/documentation/tutorials/tutorial_3_abstractions.ipynb` & `oqtant-0.14.2/documentation/tutorials/tutorial_3_abstractions.ipynb`

 * *Files identical despite different names*

### Comparing `oqtant-0.14.1/documentation/tutorials/tutorial_3_abstractions.md` & `oqtant-0.14.2/documentation/tutorials/tutorial_3_abstractions.md`

 * *Files identical despite different names*

### Comparing `oqtant-0.14.1/documentation/tutorials/tutorial_4_experiment.ipynb` & `oqtant-0.14.2/documentation/tutorials/tutorial_4_experiment.ipynb`

 * *Files identical despite different names*

### Comparing `oqtant-0.14.1/documentation/tutorials/tutorial_4_experiment.md` & `oqtant-0.14.2/documentation/tutorials/tutorial_4_experiment.md`

 * *Files identical despite different names*

### Comparing `oqtant-0.14.1/documentation/tutorials/tutorial_5_optimization.ipynb` & `oqtant-0.14.2/documentation/tutorials/tutorial_5_optimization.ipynb`

 * *Files identical despite different names*

### Comparing `oqtant-0.14.1/documentation/tutorials/tutorial_5_optimization.md` & `oqtant-0.14.2/documentation/tutorials/tutorial_5_optimization.md`

 * *Files identical despite different names*

### Comparing `oqtant-0.14.1/oqtant/oqtant_client.py` & `oqtant-0.14.2/oqtant/oqtant_client.py`

 * *Files identical despite different names*

### Comparing `oqtant-0.14.1/oqtant/schemas/job.py` & `oqtant-0.14.2/oqtant/schemas/job.py`

 * *Files identical despite different names*

### Comparing `oqtant-0.14.1/oqtant/settings.py` & `oqtant-0.14.2/oqtant/settings.py`

 * *Files identical despite different names*

### Comparing `oqtant-0.14.1/oqtant/util/auth.py` & `oqtant-0.14.2/oqtant/util/auth.py`

 * *Files identical despite different names*

### Comparing `oqtant-0.14.1/oqtant/util/exceptions.py` & `oqtant-0.14.2/oqtant/util/exceptions.py`

 * *Files identical despite different names*

### Comparing `oqtant-0.14.1/pyproject.toml` & `oqtant-0.14.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "oqtant"
-version = "0.14.1"
+version = "0.14.2"
 description = "Oqtant Desktop Suite"
 authors = [
   "Larry Buza <lawrence.buza@coldquanta.com>",
   "Hannah North <hannah.north@coldquanta.com>",
   "Mike McGrath <michael.mcgrath@coldquanta.com>",
 ]
 license = "Apache-2.0"
```

### Comparing `oqtant-0.14.1/PKG-INFO` & `oqtant-0.14.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oqtant
-Version: 0.14.1
+Version: 0.14.2
 Summary: Oqtant Desktop Suite
 License: Apache-2.0
 Author: Larry Buza
 Author-email: lawrence.buza@coldquanta.com
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -28,15 +28,18 @@
 Requires-Dist: typing-extensions (>=4.3.0,<5.0.0)
 Requires-Dist: urllib3 (>=1.26.12,<2.0.0)
 Requires-Dist: uvicorn[standard] (>=0.20.0,<0.21.0)
 Description-Content-Type: text/markdown
 
 # Oqtant
 
-[![License: Apache](https://img.shields.io/badge/License-Apache-yellow.svg)](https://opensource.org/licenses/Apache-2.0) [![Twitter](https://img.shields.io/twitter/url/https/twitter.com/Infleqtion.svg?style=social&label=Follow%20%40Infleqtion)](https://twitter.com/Infleqtion)
+[![License: Apache](https://img.shields.io/badge/License-Apache-yellow.svg)](https://opensource.org/licenses/Apache-2.0)
+[![pypi](https://img.shields.io/pypi/v/bert-schemas.svg)](https://pypi.python.org/pypi/bert-schemas)
+[![versions](https://img.shields.io/pypi/pyversions/bert-schemas.svg)](https://pypi.python.org/pypi/bert-schemas)
+[![Twitter](https://img.shields.io/twitter/url/https/twitter.com/Infleqtion.svg?style=social&label=Follow%20%40Infleqtion)](https://twitter.com/Infleqtion)
 
 ## 🚀 Quick Install
 
 ```python
 pip install oqtant
 ```
 
@@ -74,13 +77,13 @@
 
 - To analyze job objects and use Albert's job analysis library, reference the AlbertJob class documentation.
 
 Need help? Found a bug? Contact <albert@infleqtion.com> for support. Thank you!
 
 ## 📓 Documentation
 
-- [Getting started](documentation/INSTALL.md) (installation, setting up the environment, How to run the tutorial notebooks)
-- [Tutorials](documentation/tutorials/tutorials.md) (demos for creating and submitting jobs)
-- [Oqtant API docs](documentation/oqtant_api_docs.md)
-- [Albert API docs](documentation/albert_api_docs.md)
-- [Job Analysis docs](documentation/job_analysis_docs.md)
+- [Getting started](https://https://gitlab.com/coldquanta/albert/oqtant/documentation/INSTALL.md) (installation, setting up the environment, How to run the tutorial notebooks)
+- [Tutorials](https://https://gitlab.com/coldquanta/albert/oqtant/documentation/tutorials/tutorials.md) (demos for creating and submitting jobs)
+- [Oqtant API docs](https://https://gitlab.com/coldquanta/albert/oqtant/documentation/oqtant_api_docs.md)
+- [Albert API docs](https://https://gitlab.com/coldquanta/albert/oqtant/documentation/albert_api_docs.md)
+- [Job Analysis docs](https://https://gitlab.com/coldquanta/albert/oqtant/documentation/job_analysis_docs.md)
```

