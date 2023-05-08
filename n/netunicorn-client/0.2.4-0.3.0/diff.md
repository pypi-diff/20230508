# Comparing `tmp/netunicorn-client-0.2.4.tar.gz` & `tmp/netunicorn-client-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/netunicorn/netunicorn/netunicorn-client/dist/.tmp-j9yytg5q/netunicorn-client-0.2.4.tar", last modified: Mon Feb 20 05:21:26 2023, max compression
+gzip compressed data, was "netunicorn-client-0.3.0.tar", last modified: Mon May  8 20:50:28 2023, max compression
```

## Comparing `netunicorn-client-0.2.4.tar` & `netunicorn-client-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 05:21:26.000000 netunicorn-client-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-02-20 05:21:26.000000 netunicorn-client-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-02-20 05:21:11.000000 netunicorn-client-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-20 05:21:26.000000 netunicorn-client-0.2.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 05:21:26.000000 netunicorn-client-0.2.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 05:21:26.000000 netunicorn-client-0.2.4/src/netunicorn/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 05:21:26.000000 netunicorn-client-0.2.4/src/netunicorn/client/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-02-20 05:21:11.000000 netunicorn-client-0.2.4/src/netunicorn/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-02-20 05:21:11.000000 netunicorn-client-0.2.4/src/netunicorn/client/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-02-20 05:21:11.000000 netunicorn-client-0.2.4/src/netunicorn/client/remote.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 05:21:26.000000 netunicorn-client-0.2.4/src/netunicorn_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-02-20 05:21:26.000000 netunicorn-client-0.2.4/src/netunicorn_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-02-20 05:21:26.000000 netunicorn-client-0.2.4/src/netunicorn_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-20 05:21:26.000000 netunicorn-client-0.2.4/src/netunicorn_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-02-20 05:21:26.000000 netunicorn-client-0.2.4/src/netunicorn_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-02-20 05:21:26.000000 netunicorn-client-0.2.4/src/netunicorn_client.egg-info/top_level.txt
+drwxrwxr-x   0 kell      (1000) kell      (1000)        0 2023-05-08 20:50:28.568323 netunicorn-client-0.3.0/
+-rw-rw-r--   0 kell      (1000) kell      (1000)      494 2023-05-08 20:50:28.568323 netunicorn-client-0.3.0/PKG-INFO
+-rw-rw-r--   0 kell      (1000) kell      (1000)      831 2023-05-08 20:43:11.000000 netunicorn-client-0.3.0/pyproject.toml
+-rw-rw-r--   0 kell      (1000) kell      (1000)       38 2023-05-08 20:50:28.568323 netunicorn-client-0.3.0/setup.cfg
+drwxrwxr-x   0 kell      (1000) kell      (1000)        0 2023-05-08 20:50:28.568323 netunicorn-client-0.3.0/src/
+drwxrwxr-x   0 kell      (1000) kell      (1000)        0 2023-05-08 20:50:28.568323 netunicorn-client-0.3.0/src/netunicorn/
+drwxrwxr-x   0 kell      (1000) kell      (1000)        0 2023-05-08 20:50:28.568323 netunicorn-client-0.3.0/src/netunicorn/client/
+-rw-rw-r--   0 kell      (1000) kell      (1000)       68 2023-04-12 23:54:04.000000 netunicorn-client-0.3.0/src/netunicorn/client/__init__.py
+-rw-rw-r--   0 kell      (1000) kell      (1000)     4847 2023-04-11 08:27:07.000000 netunicorn-client-0.3.0/src/netunicorn/client/base.py
+-rw-rw-r--   0 kell      (1000) kell      (1000)    10592 2023-04-24 15:52:34.000000 netunicorn-client-0.3.0/src/netunicorn/client/remote.py
+drwxrwxr-x   0 kell      (1000) kell      (1000)        0 2023-05-08 20:50:28.568323 netunicorn-client-0.3.0/src/netunicorn_client.egg-info/
+-rw-rw-r--   0 kell      (1000) kell      (1000)      494 2023-05-08 20:50:28.000000 netunicorn-client-0.3.0/src/netunicorn_client.egg-info/PKG-INFO
+-rw-rw-r--   0 kell      (1000) kell      (1000)      334 2023-05-08 20:50:28.000000 netunicorn-client-0.3.0/src/netunicorn_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 kell      (1000) kell      (1000)        1 2023-05-08 20:50:28.000000 netunicorn-client-0.3.0/src/netunicorn_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 kell      (1000) kell      (1000)       52 2023-05-08 20:50:28.000000 netunicorn-client-0.3.0/src/netunicorn_client.egg-info/requires.txt
+-rw-rw-r--   0 kell      (1000) kell      (1000)       11 2023-05-08 20:50:28.000000 netunicorn-client-0.3.0/src/netunicorn_client.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `netunicorn-client-0.2.4/pyproject.toml` & `netunicorn-client-0.3.0/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 [project]
 name = "netunicorn-client"
-version = "0.2.4"
+version = "0.3.0"
 authors = [
     {name = "Roman Beltiukov", email = "rbeltiukov@ucsb.edu"},
 ]
 description = "netunicorn client module"
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 keywords = ["netunicorn"]
 license = {text = "MIT"}
 classifiers = [
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
-    "netunicorn-base >= 0.2.0",
+    "netunicorn-base >= 0.3.0",
     "cloudpickle",
     "requests",
     "returns",
 ]
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [tool.mypy]
-python_version = "3.7"
+python_version = "3.8"
 ignore_missing_imports = true
 explicit_package_bases = true
 strict = true
 exclude = "tests"
 mypy_path = "$MYPY_CONFIG_FILE_DIR/src"
```

### Comparing `netunicorn-client-0.2.4/src/netunicorn/client/base.py` & `netunicorn-client-0.3.0/src/netunicorn/client/base.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from abc import ABC, abstractmethod
-from typing import Dict, Iterable
+from typing import Dict, Iterable, Optional
 
 from netunicorn.base.experiment import Experiment, ExperimentExecutionInformation
 from netunicorn.base.nodes import Nodes
 
 
 class BaseClient(ABC):
     @abstractmethod
@@ -35,38 +35,51 @@
         """
         This method checks if the system is alive.
         :return: True if server is alive, raises exception otherwise
         """
         pass
 
     @abstractmethod
-    def prepare_experiment(self, experiment: Experiment, experiment_id: str) -> str:
+    def prepare_experiment(
+        self,
+        experiment: Experiment,
+        experiment_id: str,
+        deployment_context: Optional[Dict[str, Dict[str, str]]] = None,
+    ) -> str:
         """
         Prepares an Experiment. Server will start compiling and distributing the environment among nodes.
         You can check status of preparation by calling 'get_experiment_status' function and checking if it's in
         "READY" status.
         You need to provide a per-user unique experiment name.
         This method is network-failure-safe: subsequent calls with the same network name
         will not create additional deployment processes.
         :param experiment: experiment to prepare
         :param experiment_id: user-wide unique experiment name
+        :param deployment_context: deployment context for connectors (see connectors documentation)
+        Format: {connector_name: {key: value}, ...}
         :return: the same experiment_id if everything's correct
         """
         pass
 
     @abstractmethod
-    def start_execution(self, experiment_id: str) -> str:
+    def start_execution(
+        self,
+        experiment_id: str,
+        execution_context: Optional[Dict[str, Dict[str, str]]] = None,
+    ) -> str:
         """
         Starts execution of prepared experiment.
         You can check status and results of an experiment by calling 'get_experiment_status' function and checking if it's in
         "FINISHED" status.
         You need to provide an experiment_id of prepared experiment to start.
         This method is network-failure-safe: subsequent calls with the same experiment id
         will not create additional start process.
         :param experiment_id: prepared experiment id
+        :param execution_context: execution context for connectors (see connectors documentation)
+        Format: {connector_name: {key: value}, ...}
         :return: the same experiment_id if execution already in progress or finished
         """
         pass
 
     @abstractmethod
     def get_experiment_status(
         self, experiment_id: str
@@ -77,21 +90,35 @@
         If experiment finished, you can explore results of the experiment
         :param experiment_id: id of the experiment returned by 'prepare_experiment' function
         :return: current status of the experiment, optionally experiment definition, optionally experiment results
         """
         pass
 
     @abstractmethod
-    def cancel_experiment(self, experiment_id: str) -> str:
+    def cancel_experiment(
+        self,
+        experiment_id: str,
+        cancellation_context: Optional[Dict[str, Dict[str, str]]] = None,
+    ) -> str:
         """
         Cancels experiment execution.
         :param experiment_id: id of the experiment
+        :param cancellation_context: cancellation context for connectors (see connectors documentation)
+        Format: {connector_name: {key: value}, ...}
+        :return: the same experiment_id if everything's correct
         """
         pass
 
     @abstractmethod
-    def cancel_executors(self, executors: Iterable[str]) -> str:
+    def cancel_executors(
+        self,
+        executors: Iterable[str],
+        cancellation_context: Optional[Dict[str, Dict[str, str]]] = None,
+    ) -> str:
         """
         Cancels particular executors.
         :param executors: list of executors to cancel
+        :param cancellation_context: cancellation context for connectors (see connectors documentation)
+        Format: {connector_name: {key: value}, ...}
+        :return: the same experiment_id if everything's correct
         """
         pass
```

