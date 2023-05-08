# Comparing `tmp/netunicorn-base-0.2.5.tar.gz` & `tmp/netunicorn-base-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/netunicorn/netunicorn/netunicorn-base/dist/.tmp-bdp33cz_/netunicorn-base-0.2.5.tar", last modified: Wed Mar 15 07:16:05 2023, max compression
+gzip compressed data, was "netunicorn-base-0.3.0.tar", last modified: Mon May  8 20:49:08 2023, max compression
```

## Comparing `netunicorn-base-0.2.5.tar` & `netunicorn-base-0.3.0.tar`

### file list

```diff
@@ -1,28 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 07:16:05.000000 netunicorn-base-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-03-15 07:16:05.000000 netunicorn-base-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-03-15 07:15:48.000000 netunicorn-base-0.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-15 07:16:05.000000 netunicorn-base-0.2.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 07:16:05.000000 netunicorn-base-0.2.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 07:16:05.000000 netunicorn-base-0.2.5/src/netunicorn/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 07:16:05.000000 netunicorn-base-0.2.5/src/netunicorn/base/
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-03-15 07:15:48.000000 netunicorn-base-0.2.5/src/netunicorn/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-03-15 07:15:48.000000 netunicorn-base-0.2.5/src/netunicorn/base/architecture.py
--rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-03-15 07:15:48.000000 netunicorn-base-0.2.5/src/netunicorn/base/deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)     5279 2023-03-15 07:15:48.000000 netunicorn-base-0.2.5/src/netunicorn/base/environment_definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5658 2023-03-15 07:15:48.000000 netunicorn-base-0.2.5/src/netunicorn/base/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     8732 2023-03-15 07:15:48.000000 netunicorn-base-0.2.5/src/netunicorn/base/nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-03-15 07:15:48.000000 netunicorn-base-0.2.5/src/netunicorn/base/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-03-15 07:15:48.000000 netunicorn-base-0.2.5/src/netunicorn/base/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-03-15 07:15:48.000000 netunicorn-base-0.2.5/src/netunicorn/base/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-03-15 07:15:48.000000 netunicorn-base-0.2.5/src/netunicorn/base/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 07:16:05.000000 netunicorn-base-0.2.5/src/netunicorn/director/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 07:16:05.000000 netunicorn-base-0.2.5/src/netunicorn/director/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 07:15:48.000000 netunicorn-base-0.2.5/src/netunicorn/director/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-03-15 07:15:48.000000 netunicorn-base-0.2.5/src/netunicorn/director/base/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-03-15 07:15:48.000000 netunicorn-base-0.2.5/src/netunicorn/director/base/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 07:16:05.000000 netunicorn-base-0.2.5/src/netunicorn_base.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-03-15 07:16:05.000000 netunicorn-base-0.2.5/src/netunicorn_base.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-03-15 07:16:05.000000 netunicorn-base-0.2.5/src/netunicorn_base.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-15 07:16:05.000000 netunicorn-base-0.2.5/src/netunicorn_base.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-15 07:16:05.000000 netunicorn-base-0.2.5/src/netunicorn_base.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-15 07:16:05.000000 netunicorn-base-0.2.5/src/netunicorn_base.egg-info/top_level.txt
+drwxrwxr-x   0 kell      (1000) kell      (1000)        0 2023-05-08 20:49:08.948612 netunicorn-base-0.3.0/
+-rw-rw-r--   0 kell      (1000) kell      (1000)      490 2023-05-08 20:49:08.948612 netunicorn-base-0.3.0/PKG-INFO
+-rw-rw-r--   0 kell      (1000) kell      (1000)      859 2023-04-30 04:38:09.000000 netunicorn-base-0.3.0/pyproject.toml
+-rw-rw-r--   0 kell      (1000) kell      (1000)       38 2023-05-08 20:49:08.948612 netunicorn-base-0.3.0/setup.cfg
+drwxrwxr-x   0 kell      (1000) kell      (1000)        0 2023-05-08 20:49:08.944612 netunicorn-base-0.3.0/src/
+drwxrwxr-x   0 kell      (1000) kell      (1000)        0 2023-05-08 20:49:08.944612 netunicorn-base-0.3.0/src/netunicorn/
+drwxrwxr-x   0 kell      (1000) kell      (1000)        0 2023-05-08 20:49:08.944612 netunicorn-base-0.3.0/src/netunicorn/base/
+-rw-rw-r--   0 kell      (1000) kell      (1000)      509 2023-04-12 23:52:52.000000 netunicorn-base-0.3.0/src/netunicorn/base/__init__.py
+-rw-rw-r--   0 kell      (1000) kell      (1000)      138 2023-02-18 01:38:41.000000 netunicorn-base-0.3.0/src/netunicorn/base/architecture.py
+-rw-rw-r--   0 kell      (1000) kell      (1000)     3141 2023-04-11 10:37:18.000000 netunicorn-base-0.3.0/src/netunicorn/base/deployment.py
+-rw-rw-r--   0 kell      (1000) kell      (1000)     5279 2023-03-17 04:47:51.000000 netunicorn-base-0.3.0/src/netunicorn/base/environment_definitions.py
+-rw-rw-r--   0 kell      (1000) kell      (1000)     6263 2023-04-11 08:27:07.000000 netunicorn-base-0.3.0/src/netunicorn/base/experiment.py
+-rw-rw-r--   0 kell      (1000) kell      (1000)     8831 2023-04-11 08:27:07.000000 netunicorn-base-0.3.0/src/netunicorn/base/nodes.py
+-rw-rw-r--   0 kell      (1000) kell      (1000)     3448 2023-03-17 04:47:51.000000 netunicorn-base-0.3.0/src/netunicorn/base/pipeline.py
+-rw-rw-r--   0 kell      (1000) kell      (1000)     4794 2023-03-17 07:55:21.000000 netunicorn-base-0.3.0/src/netunicorn/base/task.py
+-rw-rw-r--   0 kell      (1000) kell      (1000)     2509 2023-04-12 22:04:55.000000 netunicorn-base-0.3.0/src/netunicorn/base/types.py
+-rw-rw-r--   0 kell      (1000) kell      (1000)     3391 2023-03-17 04:47:51.000000 netunicorn-base-0.3.0/src/netunicorn/base/utils.py
+drwxrwxr-x   0 kell      (1000) kell      (1000)        0 2023-05-08 20:49:08.944612 netunicorn-base-0.3.0/src/netunicorn/director/
+drwxrwxr-x   0 kell      (1000) kell      (1000)        0 2023-05-08 20:49:08.944612 netunicorn-base-0.3.0/src/netunicorn/director/base/
+-rw-rw-r--   0 kell      (1000) kell      (1000)        0 2023-02-18 01:38:41.000000 netunicorn-base-0.3.0/src/netunicorn/director/base/__init__.py
+drwxrwxr-x   0 kell      (1000) kell      (1000)        0 2023-05-08 20:49:08.944612 netunicorn-base-0.3.0/src/netunicorn/director/base/connectors/
+-rw-rw-r--   0 kell      (1000) kell      (1000)        0 2023-04-11 08:27:07.000000 netunicorn-base-0.3.0/src/netunicorn/director/base/connectors/__init__.py
+-rw-rw-r--   0 kell      (1000) kell      (1000)     7486 2023-04-30 04:12:53.000000 netunicorn-base-0.3.0/src/netunicorn/director/base/connectors/protocol.py
+-rw-rw-r--   0 kell      (1000) kell      (1000)      109 2023-04-11 08:27:07.000000 netunicorn-base-0.3.0/src/netunicorn/director/base/connectors/types.py
+-rw-rw-r--   0 kell      (1000) kell      (1000)     1907 2023-04-11 08:27:07.000000 netunicorn-base-0.3.0/src/netunicorn/director/base/resources.py
+-rw-rw-r--   0 kell      (1000) kell      (1000)      373 2023-04-11 08:27:07.000000 netunicorn-base-0.3.0/src/netunicorn/director/base/types.py
+-rw-rw-r--   0 kell      (1000) kell      (1000)      314 2023-03-23 00:43:02.000000 netunicorn-base-0.3.0/src/netunicorn/director/base/utils.py
+-rw-rw-r--   0 kell      (1000) kell      (1000)        0 2023-04-11 08:27:07.000000 netunicorn-base-0.3.0/src/netunicorn/py.typed
+drwxrwxr-x   0 kell      (1000) kell      (1000)        0 2023-05-08 20:49:08.948612 netunicorn-base-0.3.0/src/netunicorn_base.egg-info/
+-rw-rw-r--   0 kell      (1000) kell      (1000)      490 2023-05-08 20:49:08.000000 netunicorn-base-0.3.0/src/netunicorn_base.egg-info/PKG-INFO
+-rw-rw-r--   0 kell      (1000) kell      (1000)      894 2023-05-08 20:49:08.000000 netunicorn-base-0.3.0/src/netunicorn_base.egg-info/SOURCES.txt
+-rw-rw-r--   0 kell      (1000) kell      (1000)        1 2023-05-08 20:49:08.000000 netunicorn-base-0.3.0/src/netunicorn_base.egg-info/dependency_links.txt
+-rw-rw-r--   0 kell      (1000) kell      (1000)       35 2023-05-08 20:49:08.000000 netunicorn-base-0.3.0/src/netunicorn_base.egg-info/requires.txt
+-rw-rw-r--   0 kell      (1000) kell      (1000)       11 2023-05-08 20:49:08.000000 netunicorn-base-0.3.0/src/netunicorn_base.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `netunicorn-base-0.2.5/pyproject.toml` & `netunicorn-base-0.3.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 [project]
 name = "netunicorn-base"
-version = "0.2.5"
+version = "0.3.0"
 authors = [
     {name = "Roman Beltiukov", email = "rbeltiukov@ucsb.edu"},
 ]
 description = "netunicorn base module"
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
     "returns",
     "typing-extensions",
+    "pydantic",
 ]
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
+[tool.setuptools.package-data]
+netunicorn = ["py.typed"]
+
 [tool.mypy]
-python_version = "3.7"
+python_version = "3.8"
 ignore_missing_imports = true
 strict = true
 explicit_package_bases = true
 exclude = "tests"
 mypy_path = "$MYPY_CONFIG_FILE_DIR/src"
```

### Comparing `netunicorn-base-0.2.5/src/netunicorn/base/deployment.py` & `netunicorn-base-0.3.0/src/netunicorn/base/deployment.py`

 * *Files 22% similar despite different names*

```diff
@@ -19,23 +19,28 @@
     cloudpickle.register_pickle_by_value(netunicorn.library)
 except ImportError:
     pass
 
 
 class Deployment:
     def __init__(
-        self, node: Node, pipeline: Pipeline, keep_alive_timeout_minutes: int = 10
+        self,
+        node: Node,
+        pipeline: Pipeline,
+        keep_alive_timeout_minutes: int = 10,
+        cleanup: bool = True,
     ):
         self.node = node
         self.prepared = False
         self.executor_id = ""
         self.error: Optional[Exception] = None
         self.pipeline: SerializedPipelineType = b""
         self.environment_definition = deepcopy(pipeline.environment_definition)
         self.keep_alive_timeout_minutes = keep_alive_timeout_minutes
+        self.cleanup = cleanup
 
         pipeline = deepcopy(pipeline)
 
         for i, element in enumerate(pipeline.tasks):
             pipeline.tasks[i] = [
                 x.dispatch(node) if isinstance(x, TaskDispatcher) else x
                 for x in element
@@ -56,25 +61,27 @@
         return {
             "node": self.node.__json__(),
             "prepared": self.prepared,
             "executor_id": self.executor_id,
             "error": str(self.error) if self.error else None,
             "pipeline": self.pipeline,
             "keep_alive_timeout_minutes": self.keep_alive_timeout_minutes,
+            "cleanup": self.cleanup,
             "environment_definition": self.environment_definition.__json__(),
             "environment_definition_type": self.environment_definition.__class__.__name__,
         }
 
     @classmethod
     def from_json(cls, data: DeploymentRepresentation) -> Deployment:
         instance = cls.__new__(cls)
 
         instance.node = Node.from_json(data["node"])
         instance.prepared = data["prepared"]
         instance.executor_id = data["executor_id"]
         instance.error = Exception(data["error"]) if data["error"] else None
         instance.pipeline = b64decode(data["pipeline"])
         instance.keep_alive_timeout_minutes = data["keep_alive_timeout_minutes"]
+        instance.cleanup = data.get("cleanup", True)
         instance.environment_definition = getattr(
             netunicorn.base.environment_definitions, data["environment_definition_type"]
         ).from_json(data["environment_definition"])
         return instance
```

### Comparing `netunicorn-base-0.2.5/src/netunicorn/base/environment_definitions.py` & `netunicorn-base-0.3.0/src/netunicorn/base/environment_definitions.py`

 * *Files identical despite different names*

### Comparing `netunicorn-base-0.2.5/src/netunicorn/base/experiment.py` & `netunicorn-base-0.3.0/src/netunicorn/base/experiment.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import base64
 import copy
 from dataclasses import dataclass
 from enum import Enum
-from typing import Iterator, List, Optional, Sequence, Tuple, Union
+from typing import Dict, Iterator, List, Optional, Sequence, Tuple, Union
 
 from returns.result import Result
 
 from .deployment import Deployment
 from .nodes import Node, Nodes
 from .pipeline import Pipeline
 from .types import (
@@ -32,40 +32,47 @@
 
     @classmethod
     def from_json(cls, value: int) -> ExperimentStatus:
         return cls(value)
 
 
 class Experiment:
-    def __init__(self) -> None:
+    def __init__(
+        self, deployment_context: Optional[Dict[str, Dict[str, str]]] = None
+    ) -> None:
         self.deployment_map: List[Deployment] = []
+        self.deployment_context = deployment_context
 
     def append(self, node: Node, pipeline: Pipeline) -> Experiment:
         self.deployment_map.append(Deployment(node, pipeline))
         return self
 
     def map(self, pipeline: Pipeline, nodes: Sequence[Node]) -> Experiment:
         if isinstance(nodes, Nodes):
             raise TypeError("Expected sequence of nodes, got Nodes instead")
 
         for node in nodes:
+            if not isinstance(node, Node):
+                raise TypeError(f"Expected sequence of nodes, got {type(node)} instead")
             self.append(node, pipeline)
         return self
 
     def __json__(self) -> ExperimentRepresentation:
         return {
             "deployment_map": [x.__json__() for x in self.deployment_map],
+            "deployment_context": self.deployment_context,
         }
 
     @classmethod
     def from_json(cls, data: ExperimentRepresentation) -> Experiment:
         instance = cls.__new__(cls)
         instance.deployment_map = [
             Deployment.from_json(x) for x in data["deployment_map"]
         ]
+        instance.deployment_context = data.get("deployment_context")
         return instance
 
     def __getitem__(self, item: int) -> Deployment:
         return self.deployment_map[item]
 
     def __iter__(self) -> Iterator[Deployment]:
         return iter(self.deployment_map)
@@ -78,14 +85,18 @@
 
     def __repr__(self) -> str:
         return str(self)
 
     def __add__(self, other: Experiment) -> Experiment:
         new_map = copy.deepcopy(self)
         new_map.deployment_map.extend(other.deployment_map)
+        if other.deployment_context:
+            if new_map.deployment_context is None:
+                new_map.deployment_context = {}
+            new_map.deployment_context.update(other.deployment_context)
         return new_map
 
 
 class DeploymentExecutionResult:
     def __init__(
         self,
         node: Node,
```

### Comparing `netunicorn-base-0.2.5/src/netunicorn/base/nodes.py` & `netunicorn-base-0.3.0/src/netunicorn/base/nodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,17 @@
         self.properties = properties
         self.additional_properties: Dict[str, NodeProperty] = {}
         self.architecture = architecture
 
     def __getitem__(self, item: str) -> NodeProperty:
         return self.properties.get(item, None)
 
+    def __iter__(self) -> Iterator[NodeProperty]:
+        raise TypeError("Node is not iterable")
+
     def __setitem__(self, key: str, value: NodeProperty) -> None:
         self.properties[key] = value
 
     def __str__(self) -> str:
         return self.name
 
     def __repr__(self) -> str:
```

### Comparing `netunicorn-base-0.2.5/src/netunicorn/base/pipeline.py` & `netunicorn-base-0.3.0/src/netunicorn/base/pipeline.py`

 * *Files identical despite different names*

### Comparing `netunicorn-base-0.2.5/src/netunicorn/base/task.py` & `netunicorn-base-0.3.0/src/netunicorn/base/task.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 
     def __init__(self, name: Optional[str] = None) -> None:
         """
         This is a constructor for the task. Any variables (state) that `run` method should use should be provided here.
         Please, do not forget to call `super().__init__()` in your implementation.
         """
         self.name = name or str(uuid.uuid4())  # Each task should have a name
+        self.requirements = copy.deepcopy(self.requirements)
 
     def __call__(self) -> Any:
         return self.run()
 
     def __repr__(self) -> str:
         type_ = type(self)
         module = type_.__module__
```

### Comparing `netunicorn-base-0.2.5/src/netunicorn/base/types.py` & `netunicorn-base-0.3.0/src/netunicorn/base/types.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,16 @@
 from __future__ import annotations
 
 import sys
 from enum import IntEnum
+from typing import Any, Dict, List, Optional, Set, TypedDict, Union
 
+from pydantic import BaseModel
 from returns.result import Result
 
-if sys.version_info >= (3, 8):
-    from typing import TypedDict
-else:
-    from typing_extensions import TypedDict
-
-from typing import Any, Dict, List, Optional, Set, Union
-
 if sys.version_info >= (3, 10):
     from typing import TypeAlias
 else:
     from typing_extensions import TypeAlias
 
 NodeProperty = Union[str, float, int, Set[str], None]
 
@@ -37,14 +32,15 @@
 class DeploymentRepresentation(TypedDict):
     node: NodeRepresentation
     prepared: bool
     executor_id: str
     error: Optional[str]
     pipeline: bytes
     keep_alive_timeout_minutes: int
+    cleanup: bool
     environment_definition: EnvironmentDefinitionRepresentation
     environment_definition_type: str
 
 
 class NodesRepresentation(TypedDict):
     node_pool_type: str
     node_pool_data: List[Union[NodeRepresentation, NodesRepresentation]]
@@ -69,14 +65,15 @@
     image: Optional[str]
     build_context: BuildContextRepresentation
     runtime_context: RuntimeContextRepresentation
 
 
 class ExperimentRepresentation(TypedDict):
     deployment_map: List[DeploymentRepresentation]
+    deployment_context: Optional[Dict[str, Dict[str, str]]]
 
 
 class DeploymentExecutionResultRepresentation(TypedDict):
     node: NodeRepresentation
     pipeline: str
     result: Optional[str]
     error: Optional[str]
@@ -89,7 +86,12 @@
 
 
 class PipelineExecutorState(IntEnum):
     LOOKING_FOR_PIPELINE = 0
     EXECUTING = 1
     REPORTING = 2
     FINISHED = 3
+
+
+class FlagValues(BaseModel):
+    text_value: Optional[str] = None
+    int_value: int = 0
```

### Comparing `netunicorn-base-0.2.5/src/netunicorn/base/utils.py` & `netunicorn-base-0.3.0/src/netunicorn/base/utils.py`

 * *Files identical despite different names*

### Comparing `netunicorn-base-0.2.5/src/netunicorn/director/base/resources.py` & `netunicorn-base-0.3.0/src/netunicorn/director/base/resources.py`

 * *Files 8% similar despite different names*

```diff
@@ -45,16 +45,18 @@
     )
     logger = __logging.getLogger(name)
     logger.handlers.clear()
     logger.propagate = False
 
     stream_handler = __logging.StreamHandler(sys.stdout)
     stream_handler.setFormatter(formatter)
+    stream_handler.setLevel(level)
     logger.addHandler(stream_handler)
 
     file_handler = __logging.FileHandler(f"{name}.log")
     file_handler.setFormatter(formatter)
+    file_handler.setLevel(level)
     logger.addHandler(file_handler)
 
     logger.setLevel(level)
     logger.info(f"Logger {name} created with level {level}")
     return logger
```

