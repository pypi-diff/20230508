# Comparing `tmp/kfp-tekton-1.6.5.tar.gz` & `tmp/kfp-tekton-1.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kfp-tekton-1.6.5.tar", last modified: Tue Apr 11 19:49:28 2023, max compression
+gzip compressed data, was "kfp-tekton-1.6.6.tar", last modified: Mon May  8 16:51:40 2023, max compression
```

## Comparing `kfp-tekton-1.6.5.tar` & `kfp-tekton-1.6.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 tommyli    (501) staff       (20)        0 2023-04-11 19:49:28.868767 kfp-tekton-1.6.5/
--rw-r--r--   0 tommyli    (501) staff       (20)    11889 2023-04-11 19:49:28.868376 kfp-tekton-1.6.5/PKG-INFO
--rw-r--r--   0 tommyli    (501) staff       (20)    16444 2023-04-11 19:48:11.000000 kfp-tekton-1.6.5/README.md
-drwxr-xr-x   0 tommyli    (501) staff       (20)        0 2023-04-11 19:49:28.856151 kfp-tekton-1.6.5/kfp_tekton/
--rw-r--r--   0 tommyli    (501) staff       (20)      713 2023-04-11 19:48:11.000000 kfp-tekton-1.6.5/kfp_tekton/__init__.py
--rw-r--r--   0 tommyli    (501) staff       (20)    30584 2023-04-07 17:42:53.000000 kfp-tekton-1.6.5/kfp_tekton/_client.py
-drwxr-xr-x   0 tommyli    (501) staff       (20)        0 2023-04-11 19:49:28.867515 kfp-tekton-1.6.5/kfp_tekton/compiler/
--rw-r--r--   0 tommyli    (501) staff       (20)      675 2023-02-21 19:36:36.000000 kfp-tekton-1.6.5/kfp_tekton/compiler/__init__.py
--rw-r--r--   0 tommyli    (501) staff       (20)    44521 2023-02-21 19:36:36.000000 kfp-tekton-1.6.5/kfp_tekton/compiler/_data_passing_rewriter.py
--rw-r--r--   0 tommyli    (501) staff       (20)     7091 2023-04-07 17:42:53.000000 kfp-tekton-1.6.5/kfp_tekton/compiler/_k8s_helper.py
--rw-r--r--   0 tommyli    (501) staff       (20)    32108 2023-03-17 18:34:11.000000 kfp-tekton-1.6.5/kfp_tekton/compiler/_op_to_template.py
--rw-r--r--   0 tommyli    (501) staff       (20)    30933 2023-04-07 17:42:53.000000 kfp-tekton-1.6.5/kfp_tekton/compiler/_tekton_handler.py
--rw-r--r--   0 tommyli    (501) staff       (20)    99548 2023-04-07 17:42:53.000000 kfp-tekton-1.6.5/kfp_tekton/compiler/compiler.py
--rw-r--r--   0 tommyli    (501) staff       (20)     4279 2023-04-07 17:42:53.000000 kfp-tekton-1.6.5/kfp_tekton/compiler/main.py
--rw-r--r--   0 tommyli    (501) staff       (20)     4088 2023-03-17 18:33:39.000000 kfp-tekton-1.6.5/kfp_tekton/compiler/pipeline_utils.py
--rw-r--r--   0 tommyli    (501) staff       (20)     2071 2023-02-21 19:36:36.000000 kfp-tekton-1.6.5/kfp_tekton/compiler/yaml_utils.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1311 2023-04-07 17:42:53.000000 kfp-tekton-1.6.5/kfp_tekton/k8s_client_helper.py
--rw-r--r--   0 tommyli    (501) staff       (20)    17417 2023-04-07 17:42:53.000000 kfp-tekton-1.6.5/kfp_tekton/tekton.py
-drwxr-xr-x   0 tommyli    (501) staff       (20)        0 2023-04-11 19:49:28.858796 kfp-tekton-1.6.5/kfp_tekton.egg-info/
--rw-r--r--   0 tommyli    (501) staff       (20)    11889 2023-04-11 19:49:28.000000 kfp-tekton-1.6.5/kfp_tekton.egg-info/PKG-INFO
--rw-r--r--   0 tommyli    (501) staff       (20)      645 2023-04-11 19:49:28.000000 kfp-tekton-1.6.5/kfp_tekton.egg-info/SOURCES.txt
--rw-r--r--   0 tommyli    (501) staff       (20)        1 2023-04-11 19:49:28.000000 kfp-tekton-1.6.5/kfp_tekton.egg-info/dependency_links.txt
--rw-r--r--   0 tommyli    (501) staff       (20)      107 2023-04-11 19:49:28.000000 kfp-tekton-1.6.5/kfp_tekton.egg-info/entry_points.txt
--rw-r--r--   0 tommyli    (501) staff       (20)       49 2023-04-11 19:49:28.000000 kfp-tekton-1.6.5/kfp_tekton.egg-info/requires.txt
--rw-r--r--   0 tommyli    (501) staff       (20)       11 2023-04-11 19:49:28.000000 kfp-tekton-1.6.5/kfp_tekton.egg-info/top_level.txt
--rw-r--r--   0 tommyli    (501) staff       (20)       38 2023-04-11 19:49:28.868882 kfp-tekton-1.6.5/setup.cfg
--rw-r--r--   0 tommyli    (501) staff       (20)     7465 2023-04-11 19:48:11.000000 kfp-tekton-1.6.5/setup.py
+drwxr-xr-x   0 tommyli    (501) staff       (20)        0 2023-05-08 16:51:40.983426 kfp-tekton-1.6.6/
+-rw-r--r--   0 tommyli    (501) staff       (20)    11940 2023-05-08 16:51:40.983005 kfp-tekton-1.6.6/PKG-INFO
+-rw-r--r--   0 tommyli    (501) staff       (20)    16444 2023-05-08 16:35:39.000000 kfp-tekton-1.6.6/README.md
+drwxr-xr-x   0 tommyli    (501) staff       (20)        0 2023-05-08 16:51:40.977173 kfp-tekton-1.6.6/kfp_tekton/
+-rw-r--r--   0 tommyli    (501) staff       (20)      713 2023-05-08 16:42:37.000000 kfp-tekton-1.6.6/kfp_tekton/__init__.py
+-rw-r--r--   0 tommyli    (501) staff       (20)    33277 2023-05-08 16:25:20.000000 kfp-tekton-1.6.6/kfp_tekton/_client.py
+drwxr-xr-x   0 tommyli    (501) staff       (20)        0 2023-05-08 16:51:40.982570 kfp-tekton-1.6.6/kfp_tekton/compiler/
+-rw-r--r--   0 tommyli    (501) staff       (20)      675 2023-04-24 20:38:23.000000 kfp-tekton-1.6.6/kfp_tekton/compiler/__init__.py
+-rw-r--r--   0 tommyli    (501) staff       (20)    44521 2023-04-24 20:38:23.000000 kfp-tekton-1.6.6/kfp_tekton/compiler/_data_passing_rewriter.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     7091 2023-05-08 16:22:35.000000 kfp-tekton-1.6.6/kfp_tekton/compiler/_k8s_helper.py
+-rw-r--r--   0 tommyli    (501) staff       (20)    32108 2023-04-24 20:38:23.000000 kfp-tekton-1.6.6/kfp_tekton/compiler/_op_to_template.py
+-rw-r--r--   0 tommyli    (501) staff       (20)    30933 2023-05-08 16:22:35.000000 kfp-tekton-1.6.6/kfp_tekton/compiler/_tekton_handler.py
+-rw-r--r--   0 tommyli    (501) staff       (20)    99548 2023-05-08 16:22:35.000000 kfp-tekton-1.6.6/kfp_tekton/compiler/compiler.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     4279 2023-05-08 16:22:35.000000 kfp-tekton-1.6.6/kfp_tekton/compiler/main.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     4088 2023-04-24 20:38:23.000000 kfp-tekton-1.6.6/kfp_tekton/compiler/pipeline_utils.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     2071 2023-04-24 20:38:23.000000 kfp-tekton-1.6.6/kfp_tekton/compiler/yaml_utils.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1311 2023-05-08 16:22:35.000000 kfp-tekton-1.6.6/kfp_tekton/k8s_client_helper.py
+-rw-r--r--   0 tommyli    (501) staff       (20)    17417 2023-05-08 16:22:35.000000 kfp-tekton-1.6.6/kfp_tekton/tekton.py
+drwxr-xr-x   0 tommyli    (501) staff       (20)        0 2023-05-08 16:51:40.979176 kfp-tekton-1.6.6/kfp_tekton.egg-info/
+-rw-r--r--   0 tommyli    (501) staff       (20)    11940 2023-05-08 16:51:40.000000 kfp-tekton-1.6.6/kfp_tekton.egg-info/PKG-INFO
+-rw-r--r--   0 tommyli    (501) staff       (20)      645 2023-05-08 16:51:40.000000 kfp-tekton-1.6.6/kfp_tekton.egg-info/SOURCES.txt
+-rw-r--r--   0 tommyli    (501) staff       (20)        1 2023-05-08 16:51:40.000000 kfp-tekton-1.6.6/kfp_tekton.egg-info/dependency_links.txt
+-rw-r--r--   0 tommyli    (501) staff       (20)      107 2023-05-08 16:51:40.000000 kfp-tekton-1.6.6/kfp_tekton.egg-info/entry_points.txt
+-rw-r--r--   0 tommyli    (501) staff       (20)       49 2023-05-08 16:51:40.000000 kfp-tekton-1.6.6/kfp_tekton.egg-info/requires.txt
+-rw-r--r--   0 tommyli    (501) staff       (20)       11 2023-05-08 16:51:40.000000 kfp-tekton-1.6.6/kfp_tekton.egg-info/top_level.txt
+-rw-r--r--   0 tommyli    (501) staff       (20)       38 2023-05-08 16:51:40.983529 kfp-tekton-1.6.6/setup.cfg
+-rw-r--r--   0 tommyli    (501) staff       (20)     7515 2023-05-08 16:43:07.000000 kfp-tekton-1.6.6/setup.py
```

### Comparing `kfp-tekton-1.6.5/PKG-INFO` & `kfp-tekton-1.6.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: kfp-tekton
-Version: 1.6.5
+Version: 1.6.6
 Summary: Tekton Compiler for Kubeflow Pipelines
 Home-page: https://github.com/kubeflow/kfp-tekton/
 Author: kubeflow.org
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
@@ -82,15 +83,15 @@
     function and submits it for execution on Kubeflow Pipelines.
   * `kfp_tekton.TektonClient.create_run_from_pipeline_package` runs a local
     pipeline package on Kubeflow Pipelines.
 
 
 <h2><a id="project-prerequisites">Project Prerequisites</a></h2>
 
- - Python: `3.7` or later
+ - Python: `3.8` or later
  - Tekton: [`v0.44.2`](https://github.com/tektoncd/pipeline/releases/tag/v0.44.2) or [later](https://github.com/tektoncd/pipeline/releases/latest)
  - Tekton CLI: [`0.29.1`](https://github.com/tektoncd/cli/releases/tag/v0.29.1)
  - Kubeflow Pipelines: [KFP with Tekton backend](https://github.com/kubeflow/kfp-tekton/blob/master/guides/kfp_tekton_install.md)
 
 Follow the instructions for [installing project prerequisites](https://github.com/kubeflow/kfp-tekton/blob/master/sdk/python/README.md#development-prerequisites)
 and take note of some important caveats.
```

### Comparing `kfp-tekton-1.6.5/README.md` & `kfp-tekton-1.6.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -29,18 +29,18 @@
     - [Monkey-Patch to Dynamically Replace Static KFP Compiler Methods](#monkey-patch-to-dynamically-replace-static-kfp-compiler-methods)
 
 <!-- END of ToC generated by running ./tools/mdtoc.sh sdk/python/README.md -->
 
 
 ## Development Prerequisites
 
-1. [`Python`](https://www.python.org/downloads/): version `3.7` or later (new code must maintain compatibility with `3.7`)
-2. [`Kubernetes` Cluster](https://kubernetes.io/): version `1.23` ([required by Kubeflow](https://www.kubeflow.org/docs/started/kubeflow-overview/) and Tekton `0.44.0`)
+1. [`Python`](https://www.python.org/downloads/): version `3.8` or later (new code must maintain compatibility with `3.8`)
+2. [`Kubernetes` Cluster](https://kubernetes.io/): version `1.23` ([required by Kubeflow](https://www.kubeflow.org/docs/started/kubeflow-overview/) and Tekton `0.44.2`)
 3. [`kubectl` CLI](https://kubernetes.io/docs/tasks/tools/install-kubectl/): required to deploy Tekton pipelines to Kubernetes cluster
-4. [`Tekton` Deployment](https://github.com/tektoncd/pipeline/releases/tag/v0.44.0/): version `0.44.0` or greater, required for end-to-end testing
+4. [`Tekton` Deployment](https://github.com/tektoncd/pipeline/releases/tag/v0.44.2/): version `0.44.2` or greater, required for end-to-end testing
 5. [`tkn` CLI](https://github.com/tektoncd/cli#installing-tkn): version `0.29.1` or greater, required for end-to-end testing of Tekton pipelines
 6. [`Kubeflow Pipelines` Deployment](https://www.kubeflow.org/docs/pipelines/installation/overview/): required for some end-to-end tests
 
 
 ### Installing Tekton
 
 A working Tekton cluster deployment is required to perform end-to-end tests of the pipelines generated
@@ -98,16 +98,16 @@
 The source code of the `kfp-tekton` compiler was created as an extension of the [`Kubeflow Pipelines SDK Compiler`](https://github.com/kubeflow/pipelines/tree/sdk/release-1.8/sdk/python/kfp/compiler).
 This approach allowed us to leverage much of the existing [Kubeflow Pipelines Python SDK code](https://www.kubeflow.org/docs/pipelines/sdk/sdk-overview/#sdk-packages),
 like the DSL and components packages, but "override" or "replace" those parts of the compiler code required to generate
 the Tekton YAML instead of Argo YAML. Since the KFP SDK was not designed and implemented to easily be extended,
 _monkey-patching_ was used to replace non-class methods and functions at runtime.
 
 In order for the _monkey patch_ to work properly, the `kfp-tekton` compiler source code has to be aligned with a
-specific version of the `kfp` SDK compiler. As of now the `kfp-tekton` SDK version is `1.6.5` which is aligned with KFP
-SDK version [`1.8.20`](https://pypi.org/project/kfp/1.8.20/).
+specific version of the `kfp` SDK compiler. As of now the `kfp-tekton` SDK version is `1.6.6` which is aligned with KFP
+SDK version [`1.8.21`](https://pypi.org/project/kfp/1.8.21/).
 
 
 ## Adding New Code
 
 The Python package structure as well as the module names and method signatures closely mirror those of the
 [`Kubeflow Pipelines Python SDK`](https://github.com/kubeflow/pipelines/tree/master/sdk/python).
 This helps keeping track of all the code that had to modified and will make merging (some of) the code back into KFP or
```

### Comparing `kfp-tekton-1.6.5/kfp_tekton/__init__.py` & `kfp-tekton-1.6.6/kfp_tekton/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,11 +8,11 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = '1.6.5'
+__version__ = '1.6.6'
 
 from ._client import TektonClient  # noqa F401
 from .k8s_client_helper import env_from_secret  # noqa F401
```

### Comparing `kfp-tekton-1.6.5/kfp_tekton/_client.py` & `kfp-tekton-1.6.6/kfp_tekton/_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,21 +11,23 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 import os
 import tempfile
+import time
 
 from datetime import datetime
 from typing import Mapping, Callable, Optional
 
 import kfp
 
 import kfp_tekton_server_api as kfp_server_api
+from kfp_tekton_server_api import ApiException
 
 from .compiler import TektonCompiler
 
 import json
 import logging
 
 from kfp import dsl
@@ -155,14 +157,70 @@
             try:
                 with open(kfp.Client.NAMESPACE_PATH, 'r') as f:
                     current_namespace = f.read()
                     self.set_user_namespace(current_namespace)
             except FileNotFoundError:
                 logging.info(
                     'Failed to automatically set namespace.', exc_info=False)
+                
+    def wait_for_run_completion(self, run_id: str, timeout: int):
+        """Waits for a run to complete.
+
+        Args:
+          run_id: Run id, returned from run_pipeline.
+          timeout: Timeout in seconds.
+
+        Returns:
+          A run detail object: Most important fields are run and pipeline_runtime.
+
+        Raises:
+          TimeoutError: if the pipeline run failed to finish before the specified timeout.
+        """
+        status = 'Running:'
+        start_time = datetime.datetime.now()
+        if isinstance(timeout, datetime.timedelta):
+            timeout = timeout.total_seconds()
+        is_valid_token = False
+        # Tekton pipelineruns Status
+        # List of Tekton status: https://github.com/tektoncd/pipeline/blob/main/pkg/apis/pipeline/v1/pipelinerun_types.go
+        # List of Tekton error status: https://github.com/tektoncd/pipeline/blob/main/pkg/reconciler/pipelinerun/pipelinerun.go
+        tekton_completion_status = {'succeeded',
+                                    'failed',
+                                    'skipped',
+                                    'error',
+                                    'completed',
+                                    'pipelineruncancelled',
+                                    'pipelineruncouldntcancel',
+                                    'pipelineruntimeout',
+                                    'cancelled',
+                                    'stoppedrunfinally',
+                                    'cancelledrunfinally',
+                                    'invalidtaskresultreference'}
+        while True:
+            try:
+                get_run_response = self._run_api.get_run(run_id=run_id)
+                is_valid_token = True
+            except ApiException as api_ex:
+                # if the token is valid but receiving 401 Unauthorized error
+                # then refresh the token
+                if is_valid_token and api_ex.status == 401:
+                    logging.info('Access token has expired !!! Refreshing ...')
+                    self._refresh_api_client_token()
+                    continue
+                else:
+                    raise api_ex
+            status = get_run_response.run.status
+            elapsed_time = (datetime.datetime.now() -
+                            start_time).total_seconds()
+            logging.info('Waiting for the job to complete...')
+            if elapsed_time > timeout:
+                raise TimeoutError('Run timeout')
+            if status is not None and status.lower() in tekton_completion_status:
+                return get_run_response
+            time.sleep(5)
 
     def create_experiment(
             self,
             name: str,
             description: str = None,
             namespace: str = None) -> kfp_server_api.V1Experiment:
         """Create a new experiment.
```

### Comparing `kfp-tekton-1.6.5/kfp_tekton/compiler/__init__.py` & `kfp-tekton-1.6.6/kfp_tekton/compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-1.6.5/kfp_tekton/compiler/_data_passing_rewriter.py` & `kfp-tekton-1.6.6/kfp_tekton/compiler/_data_passing_rewriter.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-1.6.5/kfp_tekton/compiler/_k8s_helper.py` & `kfp-tekton-1.6.6/kfp_tekton/compiler/_k8s_helper.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-1.6.5/kfp_tekton/compiler/_op_to_template.py` & `kfp-tekton-1.6.6/kfp_tekton/compiler/_op_to_template.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-1.6.5/kfp_tekton/compiler/_tekton_handler.py` & `kfp-tekton-1.6.6/kfp_tekton/compiler/_tekton_handler.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-1.6.5/kfp_tekton/compiler/compiler.py` & `kfp-tekton-1.6.6/kfp_tekton/compiler/compiler.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-1.6.5/kfp_tekton/compiler/main.py` & `kfp-tekton-1.6.6/kfp_tekton/compiler/main.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-1.6.5/kfp_tekton/compiler/pipeline_utils.py` & `kfp-tekton-1.6.6/kfp_tekton/compiler/pipeline_utils.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-1.6.5/kfp_tekton/compiler/yaml_utils.py` & `kfp-tekton-1.6.6/kfp_tekton/compiler/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-1.6.5/kfp_tekton/k8s_client_helper.py` & `kfp-tekton-1.6.6/kfp_tekton/k8s_client_helper.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-1.6.5/kfp_tekton/tekton.py` & `kfp-tekton-1.6.6/kfp_tekton/tekton.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-1.6.5/kfp_tekton.egg-info/PKG-INFO` & `kfp-tekton-1.6.6/kfp_tekton.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: kfp-tekton
-Version: 1.6.5
+Version: 1.6.6
 Summary: Tekton Compiler for Kubeflow Pipelines
 Home-page: https://github.com/kubeflow/kfp-tekton/
 Author: kubeflow.org
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
@@ -82,15 +83,15 @@
     function and submits it for execution on Kubeflow Pipelines.
   * `kfp_tekton.TektonClient.create_run_from_pipeline_package` runs a local
     pipeline package on Kubeflow Pipelines.
 
 
 <h2><a id="project-prerequisites">Project Prerequisites</a></h2>
 
- - Python: `3.7` or later
+ - Python: `3.8` or later
  - Tekton: [`v0.44.2`](https://github.com/tektoncd/pipeline/releases/tag/v0.44.2) or [later](https://github.com/tektoncd/pipeline/releases/latest)
  - Tekton CLI: [`0.29.1`](https://github.com/tektoncd/cli/releases/tag/v0.29.1)
  - Kubeflow Pipelines: [KFP with Tekton backend](https://github.com/kubeflow/kfp-tekton/blob/master/guides/kfp_tekton_install.md)
 
 Follow the instructions for [installing project prerequisites](https://github.com/kubeflow/kfp-tekton/blob/master/sdk/python/README.md#development-prerequisites)
 and take note of some important caveats.
```

### Comparing `kfp-tekton-1.6.5/kfp_tekton.egg-info/SOURCES.txt` & `kfp-tekton-1.6.6/kfp_tekton.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kfp-tekton-1.6.5/setup.py` & `kfp-tekton-1.6.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,22 +16,22 @@
 # =============================================================================
 # To install the kfp_tekton project run:
 #
 #    $ pip3 install -e .
 #
 # To create a distribution for PyPi run:
 #
-#    $ export KFP_TEKTON_VERSION=1.6.5-rc1
+#    $ export KFP_TEKTON_VERSION=1.6.6-rc1
 #    $ python3 setup.py sdist
 #    $ twine check dist/kfp-tekton-${KFP_TEKTON_VERSION/-rc/rc}.tar.gz
 #    $ twine upload --repository pypi dist/kfp-tekton-${KFP_TEKTON_VERSION/-rc/rc}.tar.gz
 #
 #   ... or:
 #
-#    $ make distribution KFP_TEKTON_VERSION=1.6.5-rc1
+#    $ make distribution KFP_TEKTON_VERSION=1.6.6-rc1
 #
 # =============================================================================
 
 import logging
 import re
 import sys
 
@@ -55,15 +55,15 @@
 logger = logging.getLogger("kfp_tekton/setup.py")
 logger.setLevel(logging.INFO)
 
 
 # NOTICE, after any updates to the following, ./requirements.in should be updated
 # accordingly.
 REQUIRES = [
-    "kfp>=1.8.10,<1.8.21",
+    "kfp>=1.8.10,<1.8.22",
     "kfp-tekton-server-api>=1.5.0"
 ]
 
 TESTS_REQUIRE = [
     'pytest',
 ]
 
@@ -192,14 +192,15 @@
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: Apache Software License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Topic :: Scientific/Engineering',
         'Topic :: Scientific/Engineering :: Artificial Intelligence',
         'Topic :: Software Development',
         'Topic :: Software Development :: Libraries',
         'Topic :: Software Development :: Libraries :: Python Modules',
     ],
     python_requires='>=3.7.0',
```

