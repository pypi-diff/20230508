# Comparing `tmp/canals-0.1.1.tar.gz` & `tmp/canals-0.1.2.tar.gz`

## Comparing `canals-0.1.1.tar` & `canals-0.1.2.tar`

### file list

```diff
@@ -1,61 +1,62 @@
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 canals-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 canals-0.1.1/mkdocs.yml
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 canals-0.1.1/.github/workflows/api-docs.yml
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 canals-0.1.1/.github/workflows/release.yml
--rw-r--r--   0        0        0     2844 2020-02-02 00:00:00.000000 canals-0.1.1/.github/workflows/tests.yml
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 canals-0.1.1/canals/__about__.py
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 canals-0.1.1/canals/__init__.py
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 canals-0.1.1/canals/errors.py
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 canals-0.1.1/canals/component/__init__.py
--rw-r--r--   0        0        0     8469 2020-02-02 00:00:00.000000 canals-0.1.1/canals/component/component.py
--rw-r--r--   0        0        0     2262 2020-02-02 00:00:00.000000 canals-0.1.1/canals/component/save_init_params.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 canals-0.1.1/canals/draw/__init__.py
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 canals-0.1.1/canals/draw/draw.py
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 canals-0.1.1/canals/draw/graphviz.py
--rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 canals-0.1.1/canals/draw/mermaid.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 canals-0.1.1/canals/pipeline/__init__.py
--rw-r--r--   0        0        0     7966 2020-02-02 00:00:00.000000 canals-0.1.1/canals/pipeline/_utils.py
--rw-r--r--   0        0        0    26696 2020-02-02 00:00:00.000000 canals-0.1.1/canals/pipeline/pipeline.py
--rw-r--r--   0        0        0     8637 2020-02-02 00:00:00.000000 canals-0.1.1/canals/pipeline/save_load.py
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 canals-0.1.1/docs/index.md
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 canals-0.1.1/docs/api-docs/component.md
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 canals-0.1.1/docs/api-docs/draw.md
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 canals-0.1.1/docs/api-docs/pipeline.md
--rw-r--r--   0        0        0     7458 2020-02-02 00:00:00.000000 canals-0.1.1/docs/concepts/components.md
--rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 canals-0.1.1/docs/concepts/concepts.md
--rw-r--r--   0        0        0     7097 2020-02-02 00:00:00.000000 canals-0.1.1/docs/concepts/pipelines.md
--rw-r--r--   0        0        0    26250 2020-02-02 00:00:00.000000 canals-0.1.1/images/canals-logo-dark.png
--rw-r--r--   0        0        0    25601 2020-02-02 00:00:00.000000 canals-0.1.1/images/canals-logo-light.png
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 canals-0.1.1/test/__init__.py
--rw-r--r--   0        0        0     6547 2020-02-02 00:00:00.000000 canals-0.1.1/test/test_save_load.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 canals-0.1.1/test/pipelines/integration/__init__.py
--rw-r--r--   0        0        0     3316 2020-02-02 00:00:00.000000 canals-0.1.1/test/pipelines/integration/test_complex_pipeline.py
--rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 canals-0.1.1/test/pipelines/integration/test_fixed_decision_and_merge_pipeline.py
--rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 canals-0.1.1/test/pipelines/integration/test_fixed_decision_pipeline.py
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 canals-0.1.1/test/pipelines/integration/test_fixed_merging_pipeline.py
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 canals-0.1.1/test/pipelines/integration/test_linear_pipeline.py
--rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 canals-0.1.1/test/pipelines/integration/test_looping_and_merge_pipeline.py
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 canals-0.1.1/test/pipelines/integration/test_looping_pipeline.py
--rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 canals-0.1.1/test/pipelines/integration/test_parallel_branches_pipeline.py
--rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 canals-0.1.1/test/pipelines/integration/test_variable_decision_and_merge_pipeline.py
--rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 canals-0.1.1/test/pipelines/integration/test_variable_decision_pipeline.py
--rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 canals-0.1.1/test/pipelines/integration/test_variable_merging_pipeline.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 canals-0.1.1/test/pipelines/unit/__init__.py
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 canals-0.1.1/test/pipelines/unit/test_component.py
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 canals-0.1.1/test/test_components/__init__.py
--rw-r--r--   0        0        0     3782 2020-02-02 00:00:00.000000 canals-0.1.1/test/test_components/test_accumulate.py
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 canals-0.1.1/test/test_components/test_add_value.py
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 canals-0.1.1/test/test_components/test_double.py
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 canals-0.1.1/test/test_components/test_greet.py
--rw-r--r--   0        0        0     3134 2020-02-02 00:00:00.000000 canals-0.1.1/test/test_components/test_merge_loop.py
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 canals-0.1.1/test/test_components/test_parity.py
--rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 canals-0.1.1/test/test_components/test_remainder.py
--rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 canals-0.1.1/test/test_components/test_repeat.py
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 canals-0.1.1/test/test_components/test_subtract.py
--rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 canals-0.1.1/test/test_components/test_sum.py
--rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 canals-0.1.1/test/test_components/test_threshold.py
--rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 canals-0.1.1/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 canals-0.1.1/LICENSE
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 canals-0.1.1/README.md
--rw-r--r--   0        0        0     2320 2020-02-02 00:00:00.000000 canals-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3181 2020-02-02 00:00:00.000000 canals-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 canals-0.1.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 canals-0.1.2/mkdocs.yml
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 canals-0.1.2/.github/workflows/api-docs.yml
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 canals-0.1.2/.github/workflows/release.yml
+-rw-r--r--   0        0        0     2844 2020-02-02 00:00:00.000000 canals-0.1.2/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 canals-0.1.2/canals/__about__.py
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 canals-0.1.2/canals/__init__.py
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 canals-0.1.2/canals/errors.py
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 canals-0.1.2/canals/component/__init__.py
+-rw-r--r--   0        0        0     8469 2020-02-02 00:00:00.000000 canals-0.1.2/canals/component/component.py
+-rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 canals-0.1.2/canals/component/save_init_params.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 canals-0.1.2/canals/draw/__init__.py
+-rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 canals-0.1.2/canals/draw/draw.py
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 canals-0.1.2/canals/draw/graphviz.py
+-rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 canals-0.1.2/canals/draw/mermaid.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 canals-0.1.2/canals/pipeline/__init__.py
+-rw-r--r--   0        0        0     7966 2020-02-02 00:00:00.000000 canals-0.1.2/canals/pipeline/_utils.py
+-rw-r--r--   0        0        0    28188 2020-02-02 00:00:00.000000 canals-0.1.2/canals/pipeline/pipeline.py
+-rw-r--r--   0        0        0     8637 2020-02-02 00:00:00.000000 canals-0.1.2/canals/pipeline/save_load.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 canals-0.1.2/canals/testing/__init__.py
+-rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 canals-0.1.2/canals/testing/test_component.py
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 canals-0.1.2/docs/index.md
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 canals-0.1.2/docs/api-docs/component.md
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 canals-0.1.2/docs/api-docs/draw.md
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 canals-0.1.2/docs/api-docs/pipeline.md
+-rw-r--r--   0        0        0     7458 2020-02-02 00:00:00.000000 canals-0.1.2/docs/concepts/components.md
+-rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 canals-0.1.2/docs/concepts/concepts.md
+-rw-r--r--   0        0        0     7097 2020-02-02 00:00:00.000000 canals-0.1.2/docs/concepts/pipelines.md
+-rw-r--r--   0        0        0    26250 2020-02-02 00:00:00.000000 canals-0.1.2/images/canals-logo-dark.png
+-rw-r--r--   0        0        0    25601 2020-02-02 00:00:00.000000 canals-0.1.2/images/canals-logo-light.png
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 canals-0.1.2/test/__init__.py
+-rw-r--r--   0        0        0     6547 2020-02-02 00:00:00.000000 canals-0.1.2/test/test_save_load.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 canals-0.1.2/test/pipelines/integration/__init__.py
+-rw-r--r--   0        0        0     3316 2020-02-02 00:00:00.000000 canals-0.1.2/test/pipelines/integration/test_complex_pipeline.py
+-rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 canals-0.1.2/test/pipelines/integration/test_fixed_decision_and_merge_pipeline.py
+-rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 canals-0.1.2/test/pipelines/integration/test_fixed_decision_pipeline.py
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 canals-0.1.2/test/pipelines/integration/test_fixed_merging_pipeline.py
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 canals-0.1.2/test/pipelines/integration/test_linear_pipeline.py
+-rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 canals-0.1.2/test/pipelines/integration/test_looping_and_merge_pipeline.py
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 canals-0.1.2/test/pipelines/integration/test_looping_pipeline.py
+-rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 canals-0.1.2/test/pipelines/integration/test_parallel_branches_pipeline.py
+-rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 canals-0.1.2/test/pipelines/integration/test_variable_decision_and_merge_pipeline.py
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 canals-0.1.2/test/pipelines/integration/test_variable_decision_pipeline.py
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 canals-0.1.2/test/pipelines/integration/test_variable_merging_pipeline.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 canals-0.1.2/test/pipelines/unit/__init__.py
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 canals-0.1.2/test/test_components/__init__.py
+-rw-r--r--   0        0        0     4247 2020-02-02 00:00:00.000000 canals-0.1.2/test/test_components/test_accumulate.py
+-rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 canals-0.1.2/test/test_components/test_add_value.py
+-rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 canals-0.1.2/test/test_components/test_double.py
+-rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 canals-0.1.2/test/test_components/test_greet.py
+-rw-r--r--   0        0        0     4318 2020-02-02 00:00:00.000000 canals-0.1.2/test/test_components/test_merge_loop.py
+-rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 canals-0.1.2/test/test_components/test_parity.py
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 canals-0.1.2/test/test_components/test_remainder.py
+-rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 canals-0.1.2/test/test_components/test_repeat.py
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 canals-0.1.2/test/test_components/test_subtract.py
+-rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 canals-0.1.2/test/test_components/test_sum.py
+-rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 canals-0.1.2/test/test_components/test_threshold.py
+-rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 canals-0.1.2/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 canals-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 canals-0.1.2/README.md
+-rw-r--r--   0        0        0     2320 2020-02-02 00:00:00.000000 canals-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3181 2020-02-02 00:00:00.000000 canals-0.1.2/PKG-INFO
```

### Comparing `canals-0.1.1/.pre-commit-config.yaml` & `canals-0.1.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `canals-0.1.1/mkdocs.yml` & `canals-0.1.2/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `canals-0.1.1/.github/workflows/tests.yml` & `canals-0.1.2/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `canals-0.1.1/canals/component/component.py` & `canals-0.1.2/canals/component/component.py`

 * *Files identical despite different names*

### Comparing `canals-0.1.1/canals/draw/draw.py` & `canals-0.1.2/canals/draw/draw.py`

 * *Files identical despite different names*

### Comparing `canals-0.1.1/canals/draw/graphviz.py` & `canals-0.1.2/canals/draw/graphviz.py`

 * *Files identical despite different names*

### Comparing `canals-0.1.1/canals/draw/mermaid.py` & `canals-0.1.2/canals/draw/mermaid.py`

 * *Files identical despite different names*

### Comparing `canals-0.1.1/canals/pipeline/_utils.py` & `canals-0.1.2/canals/pipeline/_utils.py`

 * *Files identical despite different names*

### Comparing `canals-0.1.1/canals/pipeline/pipeline.py` & `canals-0.1.2/canals/pipeline/pipeline.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import datetime
 import logging
 from pathlib import Path
 from copy import deepcopy
 from collections import OrderedDict
 
-import networkx as nx
+import networkx
 
 from canals.errors import PipelineConnectError, PipelineMaxLoops, PipelineRuntimeError, PipelineValidationError
 from canals.draw import draw, RenderingEngines
 from canals.pipeline._utils import (
     InputSocket,
     OutputSocket,
     find_input_sockets,
@@ -43,17 +43,51 @@
             metadata: arbitrary dictionary to store metadata about this pipeline. Make sure all the values contained in
                 this dictionary can be serialized and deserialized if you wish to save this pipeline to file with
                 `save_pipelines()/load_pipelines()`.
             max_loops_allowed: how many times the pipeline can run the same node before throwing an exception.
         """
         self.metadata = metadata or {}
         self.max_loops_allowed = max_loops_allowed
-        self.graph = nx.MultiDiGraph()
+        self.graph = networkx.MultiDiGraph()
         self.debug: Dict[int, Dict[str, Any]] = {}
 
+    def __eq__(self, other) -> bool:
+        """
+        Equal pipelines share every metadata, node and edge, but they're not required to use
+        the same node instances: this allows pipeline saved and then loaded back to be equal to themselves.
+        """
+        if (
+            not isinstance(other, type(self))
+            or not getattr(self, "metadata") == getattr(other, "metadata")
+            or not getattr(self, "max_loops_allowed") == getattr(other, "max_loops_allowed")
+            or not hasattr(self, "graph")
+            or not hasattr(other, "graph")
+        ):
+            return False
+
+        return (
+            self.graph.adj == other.graph.adj
+            and self._comparable_nodes_list(self.graph) == self._comparable_nodes_list(other.graph)
+            and self.graph.graph == other.graph.graph
+        )
+
+    def _comparable_nodes_list(self, graph: networkx.MultiDiGraph) -> List[Dict[str, Any]]:
+        """
+        Replaces instances of nodes with their class name and defaults list in order to make sure they're comparable.
+        """
+        nodes = []
+        for node in graph.nodes:
+            comparable_node = graph.nodes[node]
+            if hasattr(comparable_node, "defaults"):
+                comparable_node["defaults"] = comparable_node["instance"].defaults
+            comparable_node["instance"] = comparable_node["instance"].__class__
+            nodes.append(comparable_node)
+        nodes.sort()
+        return nodes
+
     def add_component(self, name: str, instance: Any) -> None:
         """
         Create a component for the given component. Components are not connected to anything by default:
         use `Pipeline.connect()` to connect components together.
 
         Component names must be unique, but component instances can be reused if needed.
 
@@ -480,15 +514,15 @@
         # This downstream check is enabled only for nodes taking more than one input
         # (the "entrance" of the loop).
         data_to_wait_for = [
             (from_node, data["to_socket"].name)
             for from_node, _, data in self.graph.in_edges(name, data=True)
             # ... if there's a path in the graph leading back from the current node to the
             # input node, # and only in case this node accepts multiple inputs.
-            if not (nx.has_path(self.graph, name, from_node) and self.graph.nodes[name]["variadic_input"])
+            if not (networkx.has_path(self.graph, name, from_node) and self.graph.nodes[name]["variadic_input"])
         ]
         return data_to_wait_for
 
     def _all_nodes_to_wait_for_run(self, nodes_to_wait_for: List[str]) -> bool:
         """
         Check if all the nodes this component is waiting for has run or not.
 
@@ -548,26 +582,26 @@
         """
         Distrubute the outputs of the component into the input buffer of downstream components.
 
         Returns the updated inputs buffer.
         """
         # This is not a terminal node: find out where the output goes, to which nodes and along which edge
         is_decision_node_for_loop = (
-            any(nx.has_path(self.graph, edge[1], node_name) for edge in self.graph.out_edges(node_name))
+            any(networkx.has_path(self.graph, edge[1], node_name) for edge in self.graph.out_edges(node_name))
             and len(self.graph.out_edges(node_name)) > 1
         )
         for edge_data in self.graph.out_edges(node_name, data=True):
             to_socket = edge_data[2]["to_socket"]
             from_socket = edge_data[2]["from_socket"]
             target_node = edge_data[1]
 
             # If this is a decision node and a loop is involved, we add to the input buffer only the nodes
             # that received their expected output and we leave the others out of the queue.
             if is_decision_node_for_loop and node_results[from_socket.name] is None:
-                if nx.has_path(self.graph, target_node, node_name):
+                if networkx.has_path(self.graph, target_node, node_name):
                     # In case we're choosing to leave a loop, do not put the loop's node in the buffer.
                     logger.debug(
                         "Not adding '%s' to the inputs buffer: we're leaving the loop.",
                         target_node,
                     )
                 else:
                     # In case we're choosing to stay in a loop, do not put the external node in the buffer.
```

### Comparing `canals-0.1.1/canals/pipeline/save_load.py` & `canals-0.1.2/canals/pipeline/save_load.py`

 * *Files identical despite different names*

### Comparing `canals-0.1.1/docs/index.md` & `canals-0.1.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `canals-0.1.1/docs/concepts/components.md` & `canals-0.1.2/docs/concepts/components.md`

 * *Files identical despite different names*

### Comparing `canals-0.1.1/docs/concepts/concepts.md` & `canals-0.1.2/docs/concepts/concepts.md`

 * *Files identical despite different names*

### Comparing `canals-0.1.1/docs/concepts/pipelines.md` & `canals-0.1.2/docs/concepts/pipelines.md`

 * *Files identical despite different names*

### Comparing `canals-0.1.1/images/canals-logo-dark.png` & `canals-0.1.2/images/canals-logo-dark.png`

 * *Files identical despite different names*

### Comparing `canals-0.1.1/images/canals-logo-light.png` & `canals-0.1.2/images/canals-logo-light.png`

 * *Files identical despite different names*

### Comparing `canals-0.1.1/test/test_save_load.py` & `canals-0.1.2/test/test_save_load.py`

 * *Files identical despite different names*

### Comparing `canals-0.1.1/test/pipelines/integration/test_complex_pipeline.py` & `canals-0.1.2/test/pipelines/integration/test_complex_pipeline.py`

 * *Files identical despite different names*

### Comparing `canals-0.1.1/test/pipelines/integration/test_fixed_decision_and_merge_pipeline.py` & `canals-0.1.2/test/pipelines/integration/test_fixed_decision_and_merge_pipeline.py`

 * *Files identical despite different names*

### Comparing `canals-0.1.1/test/pipelines/integration/test_fixed_decision_pipeline.py` & `canals-0.1.2/test/pipelines/integration/test_fixed_decision_pipeline.py`

 * *Files identical despite different names*

### Comparing `canals-0.1.1/test/pipelines/integration/test_fixed_merging_pipeline.py` & `canals-0.1.2/test/pipelines/integration/test_fixed_merging_pipeline.py`

 * *Files identical despite different names*

### Comparing `canals-0.1.1/test/pipelines/integration/test_linear_pipeline.py` & `canals-0.1.2/test/pipelines/integration/test_linear_pipeline.py`

 * *Files identical despite different names*

### Comparing `canals-0.1.1/test/pipelines/integration/test_looping_and_merge_pipeline.py` & `canals-0.1.2/test/pipelines/integration/test_looping_and_merge_pipeline.py`

 * *Files identical despite different names*

### Comparing `canals-0.1.1/test/pipelines/integration/test_looping_pipeline.py` & `canals-0.1.2/test/pipelines/integration/test_looping_pipeline.py`

 * *Files identical despite different names*

### Comparing `canals-0.1.1/test/pipelines/integration/test_parallel_branches_pipeline.py` & `canals-0.1.2/test/pipelines/integration/test_parallel_branches_pipeline.py`

 * *Files identical despite different names*

### Comparing `canals-0.1.1/test/pipelines/integration/test_variable_decision_and_merge_pipeline.py` & `canals-0.1.2/test/pipelines/integration/test_variable_decision_and_merge_pipeline.py`

 * *Files identical despite different names*

### Comparing `canals-0.1.1/test/pipelines/integration/test_variable_decision_pipeline.py` & `canals-0.1.2/test/pipelines/integration/test_variable_decision_pipeline.py`

 * *Files identical despite different names*

### Comparing `canals-0.1.1/test/pipelines/integration/test_variable_merging_pipeline.py` & `canals-0.1.2/test/pipelines/integration/test_variable_merging_pipeline.py`

 * *Files identical despite different names*

### Comparing `canals-0.1.1/test/test_components/__init__.py` & `canals-0.1.2/test/test_components/__init__.py`

 * *Files identical despite different names*

### Comparing `canals-0.1.1/test/test_components/test_accumulate.py` & `canals-0.1.2/test/test_components/test_accumulate.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from typing import Union, Callable, Optional
 import sys
 import builtins
 from importlib import import_module
-
 from dataclasses import dataclass
+
+import pytest
 from canals import component
+from canals.testing import BaseTestComponent
 
 
 @component
 class Accumulate:
     """
     Accumulates the value flowing through the connection into an internal attribute.
     The sum function can be customized.
@@ -69,54 +71,61 @@
         if not module:
             raise ValueError("Could not locate the import module.")
         if module == builtins:
             return function.__name__
         return f"{module.__name__}.{function.__name__}"
 
 
-def test_accumulate_default():
-    component = Accumulate()
-    results = component.run(value=10)
-    assert results == Accumulate.Output(value=10)
-    assert component.state == 10
-
-    results = component.run(value=1)
-    assert results == Accumulate.Output(value=11)
-    assert component.state == 11
-
-    assert component._init_parameters == {}
-
-
 def my_subtract(first, second):
     return first - second
 
 
-def test_accumulate_callable():
-    component = Accumulate(function=my_subtract)
-
-    results = component.run(value=10)
-    assert results == Accumulate.Output(value=-10)
-    assert component.state == -10
-
-    results = component.run(value=1)
-    assert results == Accumulate.Output(value=-11)
-    assert component.state == -11
-
-    assert component._init_parameters == {
-        "function": "test.test_components.test_accumulate.my_subtract",
-    }
-
-
-def test_accumulate_string():
-    component = Accumulate(function="test.test_components.test_accumulate.my_subtract")
-
-    results = component.run(value=10)
-    assert results == Accumulate.Output(value=-10)
-    assert component.state == -10
-
-    results = component.run(value=1)
-    assert results == Accumulate.Output(value=-11)
-    assert component.state == -11
-
-    assert component._init_parameters == {
-        "function": "test.test_components.test_accumulate.my_subtract",
-    }
+class TestAccumulate(BaseTestComponent):
+    @pytest.fixture
+    def components(self):
+        return [
+            Accumulate(),
+            Accumulate(function=my_subtract),
+            Accumulate(function="test.test_components.test_accumulate.my_subtract"),
+        ]
+
+    def test_accumulate_default(self):
+        component = Accumulate()
+        results = component.run(value=10)
+        assert results == Accumulate.Output(value=10)
+        assert component.state == 10
+
+        results = component.run(value=1)
+        assert results == Accumulate.Output(value=11)
+        assert component.state == 11
+
+        assert component._init_parameters == {}
+
+    def test_accumulate_callable(self):
+        component = Accumulate(function=my_subtract)
+
+        results = component.run(value=10)
+        assert results == Accumulate.Output(value=-10)
+        assert component.state == -10
+
+        results = component.run(value=1)
+        assert results == Accumulate.Output(value=-11)
+        assert component.state == -11
+
+        assert component._init_parameters == {
+            "function": "test.test_components.test_accumulate.my_subtract",
+        }
+
+    def test_accumulate_string(self):
+        component = Accumulate(function="test.test_components.test_accumulate.my_subtract")
+
+        results = component.run(value=10)
+        assert results == Accumulate.Output(value=-10)
+        assert component.state == -10
+
+        results = component.run(value=1)
+        assert results == Accumulate.Output(value=-11)
+        assert component.state == -11
+
+        assert component._init_parameters == {
+            "function": "test.test_components.test_accumulate.my_subtract",
+        }
```

### Comparing `canals-0.1.1/test/test_components/test_add_value.py` & `canals-0.1.2/test/test_components/test_add_value.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
+import pytest
 from dataclasses import dataclass
 from canals import component
-
-from test.pipelines.unit.test_component import BaseTestComponent
+from canals.testing.test_component import BaseTestComponent
 
 
 @component
 class AddFixedValue:
     """
     Adds the value of `add` to `value`. If not given, `add` defaults to 1.
     """
@@ -17,16 +17,17 @@
     def __init__(self, add: int = 1):
         self.defaults = {"add": add}
 
     def run(self, value: int, add: int) -> Output:
         return AddFixedValue.Output(value=value + add)
 
 
-class AddTest(BaseTestComponent):
+class TestAddFixedValue(BaseTestComponent):
+    @pytest.fixture
     def components(self):
-        return [(AddFixedValue(), {"value": 50, "add": 10})]
+        return [AddFixedValue(), AddFixedValue(add=2)]
 
     def test_addvalue(self):
         component = AddFixedValue()
         results = component.run(value=50, add=10)
         assert results == AddFixedValue.Output(value=60)
         assert component._init_parameters == {}
```

### Comparing `canals-0.1.1/test/test_components/test_double.py` & `canals-0.1.2/test/test_components/test_double.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 from dataclasses import dataclass
+
+import pytest
+
 from canals import component
+from canals.testing import BaseTestComponent
 
 
 @component
 class Double:
     """
     Doubles the value in input.
 
@@ -17,12 +21,21 @@
     def run(self, value: int) -> Output:
         """
         Doubles the input value
         """
         return Double.Output(value=value * 2)
 
 
-def test_double_default():
-    component = Double()
-    results = component.run(value=10)
-    assert results == Double.Output(value=20)
-    assert component._init_parameters == {}
+import pytest
+from canals.testing import BaseTestComponent
+
+
+class TestDouble(BaseTestComponent):
+    @pytest.fixture
+    def components(self):
+        return [Double()]
+
+    def test_double_default(self):
+        component = Double()
+        results = component.run(value=10)
+        assert results == Double.Output(value=20)
+        assert component._init_parameters == {}
```

### Comparing `canals-0.1.1/test/test_components/test_greet.py` & `canals-0.1.2/test/test_components/test_greet.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 import logging
 
 from dataclasses import dataclass
 
+import pytest
+
+from canals.testing import BaseTestComponent
 from canals import component
 
 
 logger = logging.getLogger(__name__)
 
 
 @component
@@ -36,13 +39,23 @@
         if not level:
             raise ValueError(f"This log level does not exist: {log_level}")
 
         logger.log(level=level, msg=message.format(value=value))
         return Greet.Output(value=value)
 
 
-def test_greet_message(caplog):
-    caplog.set_level(logging.WARNING)
-    component = Greet()
-    results = component.run(value=10, message="Hello, that's {value}", log_level="WARNING")
-    assert results == Greet.Output(value=10)
-    assert "Hello, that's 10" in caplog.text
+class TestGreet(BaseTestComponent):
+    @pytest.fixture
+    def components(self):
+        return [
+            Greet(),
+            Greet(message="Hello, that's {value}"),
+            Greet(log_level="WARNING"),
+            Greet(message="Hello, that's {value}", log_level="WARNING"),
+        ]
+
+    def test_greet_message(self, caplog):
+        caplog.set_level(logging.WARNING)
+        component = Greet()
+        results = component.run(value=10, message="Hello, that's {value}", log_level="WARNING")
+        assert results == Greet.Output(value=10)
+        assert "Hello, that's 10" in caplog.text
```

### Comparing `canals-0.1.1/test/test_components/test_parity.py` & `canals-0.1.2/test/test_components/test_parity.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import Optional
 
 from dataclasses import dataclass
 import pytest
 
+from canals.testing import BaseTestComponent
 from canals import component
 
 
 @component
 class Parity:
     """
     Redirects the value, unchanged, along the 'even' connection if even, or along the 'odd' one if odd.
@@ -23,13 +24,18 @@
         """
         remainder = value % 2
         if remainder:
             return Parity.Output(even=None, odd=value)  # type: ignore  # (mypy doesn't like the missing Optional)
         return Parity.Output(even=value, odd=None)  # type: ignore  # (mypy doesn't like the missing Optional)
 
 
-def test_parity():
-    component = Parity()
-    results = component.run(value=1)
-    assert results == Parity.Output(even=None, odd=1)  # type: ignore  #(mypy doesn't like the missing Optional)
-    results = component.run(value=2)
-    assert results == Parity.Output(even=2, odd=None)  # type: ignore  #(mypy doesn't like the missing Optional)
+class TestParity(BaseTestComponent):
+    @pytest.fixture
+    def components(self):
+        return [Parity()]
+
+    def test_parity(self):
+        component = Parity()
+        results = component.run(value=1)
+        assert results == Parity.Output(even=None, odd=1)  # type: ignore  #(mypy doesn't like the missing Optional)
+        results = component.run(value=2)
+        assert results == Parity.Output(even=2, odd=None)  # type: ignore  #(mypy doesn't like the missing Optional)
```

### Comparing `canals-0.1.1/test/test_components/test_remainder.py` & `canals-0.1.2/test/test_components/test_remainder.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 from dataclasses import make_dataclass
 
+import pytest
+
+from canals.testing import BaseTestComponent
 from canals import component
 
 
 @component
 class Remainder:
     """
     Redirects the value, unchanged, along the connection corresponding to the remainder
     of a division. For example, if `divisor=3`, the value `5` would be sent along
     the second output connection.
     """
 
     def __init__(self, divisor: int = 2):
+        if divisor == 0:
+            raise ValueError("Can't divide by zero")
         self.divisor = divisor
         self._output_type = make_dataclass("Output", [(f"remainder_is_{val}", int, None) for val in range(divisor)])
 
     @property
     def output_type(self):
         return self._output_type
 
@@ -25,15 +30,25 @@
         """
         remainder = value % self.divisor
         output = self.output_type()
         setattr(output, f"remainder_is_{remainder}", value)
         return output
 
 
-def test_remainder():
-    component = Remainder()
-    results = component.run(value=3)
-    assert results == component.output_type(remainder_is_1=3)
-
-    component = Remainder(divisor=4)
-    results = component.run(value=3)
-    assert results == component.output_type(remainder_is_3=3)
+class TestRemainder(BaseTestComponent):
+    @pytest.fixture
+    def components(self):
+        return [Remainder(), Remainder(divisor=1)]
+
+    def test_remainder_default(self):
+        component = Remainder()
+        results = component.run(value=3)
+        assert results == component.output_type(remainder_is_1=3)
+
+    def test_remainder_with_divisor(self):
+        component = Remainder(divisor=4)
+        results = component.run(value=3)
+        assert results == component.output_type(remainder_is_3=3)
+
+    def test_remainder_zero(self):
+        with pytest.raises(ValueError):
+            Remainder(divisor=0)
```

### Comparing `canals-0.1.1/test/test_components/test_repeat.py` & `canals-0.1.2/test/test_components/test_repeat.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 from typing import TypeVar, Any, List
 
 from dataclasses import make_dataclass
+
+import pytest
+
+from canals.testing import BaseTestComponent
 from canals import component
 
 
 @component
 class Repeat:
     """
     Repeats the input value on all outputs.
@@ -21,19 +25,23 @@
     def run(self, value: int):
         output_dataclass = self.output_type()
         for output in self.outputs:
             setattr(output_dataclass, output, value)
         return output_dataclass
 
 
-def test_repeat_default():
-    component = Repeat()
-    results = component.run(value=10)
-    assert results == component.output_type(output_1=10, output_2=10, output_3=10)
-    assert component._init_parameters == {}
-
-
-def test_repeat_init():
-    component = Repeat(outputs=["one", "two"])
-    results = component.run(value=10)
-    assert results == component.output_type(one=10, two=10)
-    assert component._init_parameters == {"outputs": ["one", "two"]}
+class TestRepeat(BaseTestComponent):
+    @pytest.fixture
+    def components(self):
+        return [Repeat(), Repeat(outputs=["one", "two"])]
+
+    def test_repeat_default(self):
+        component = Repeat()
+        results = component.run(value=10)
+        assert results == component.output_type(output_1=10, output_2=10, output_3=10)
+        assert component._init_parameters == {}
+
+    def test_repeat_init(self):
+        component = Repeat(outputs=["one", "two"])
+        results = component.run(value=10)
+        assert results == component.output_type(one=10, two=10)
+        assert component._init_parameters == {"outputs": ["one", "two"]}
```

### Comparing `canals-0.1.1/test/test_components/test_subtract.py` & `canals-0.1.2/test/test_components/test_subtract.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,12 @@
 from dataclasses import dataclass
+
+import pytest
+
+from canals.testing import BaseTestComponent
 from canals import component
 
 
 @component
 class Subtract:
     """
     Compute the difference between two values.
@@ -16,12 +20,17 @@
         """
         :param first_value: name of the connection carrying the value to subtract from.
         :param second_value: name of the connection carrying the value to subtract.
         """
         return Subtract.Output(difference=first_value - second_value)
 
 
-def test_subtract():
-    component = Subtract()
-    results = component.run(first_value=10, second_value=7)
-    assert results == Subtract.Output(difference=3)
-    assert component._init_parameters == {}
+class TestSubtract(BaseTestComponent):
+    @pytest.fixture
+    def components(self):
+        return [Subtract()]
+
+    def test_subtract(self):
+        component = Subtract()
+        results = component.run(first_value=10, second_value=7)
+        assert results == Subtract.Output(difference=3)
+        assert component._init_parameters == {}
```

### Comparing `canals-0.1.1/test/test_components/test_sum.py` & `canals-0.1.2/test/test_components/test_sum.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,12 @@
 from dataclasses import dataclass
+
+import pytest
+
+from canals.testing import BaseTestComponent
 from canals import component
 
 
 @component
 class Sum:
     """
     Sums the values of all the input connections together.
@@ -15,26 +19,29 @@
         total: int
 
     def run(self, *value: int) -> Output:
         total = sum(value)
         return Sum.Output(total=total)
 
 
-def test_sum_no_values():
-    component = Sum()
-    results = component.run()
-    assert results == Sum.Output(total=0)
-    assert component._init_parameters == {}
-
-
-def test_sum_one_value():
-    component = Sum()
-    results = component.run(10)
-    assert results == Sum.Output(total=10)
-    assert component._init_parameters == {}
-
-
-def test_sum_few_values():
-    component = Sum()
-    results = component.run(10, 11, 12)
-    assert results == Sum.Output(total=33)
-    assert component._init_parameters == {}
+class TestSum(BaseTestComponent):
+    @pytest.fixture
+    def components(self):
+        return [Sum()]
+
+    def test_sum_no_values(self):
+        component = Sum()
+        results = component.run()
+        assert results == Sum.Output(total=0)
+        assert component._init_parameters == {}
+
+    def test_sum_one_value(self):
+        component = Sum()
+        results = component.run(10)
+        assert results == Sum.Output(total=10)
+        assert component._init_parameters == {}
+
+    def test_sum_few_values(self):
+        component = Sum()
+        results = component.run(10, 11, 12)
+        assert results == Sum.Output(total=33)
+        assert component._init_parameters == {}
```

### Comparing `canals-0.1.1/test/test_components/test_threshold.py` & `canals-0.1.2/test/test_components/test_threshold.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 from dataclasses import dataclass
 
+import pytest
+
+from canals.testing import BaseTestComponent
 from canals import component
 
 
 @component
 class Threshold:
     """
     Redirects the value, unchanged, along a different connection whether the value is above
@@ -27,15 +30,20 @@
 
     def run(self, value: int, threshold: int) -> Output:
         if value < threshold:
             return Threshold.Output(above=None, below=value)  # type: ignore
         return Threshold.Output(above=value, below=None)  # type: ignore
 
 
-def test_threshold():
-    component = Threshold()
+class TestThreshold(BaseTestComponent):
+    @pytest.fixture
+    def components(self):
+        return [Threshold()]
+
+    def test_threshold(self):
+        component = Threshold()
 
-    results = component.run(value=5, threshold=10)
-    assert results == Threshold.Output(above=None, below=5)
+        results = component.run(value=5, threshold=10)
+        assert results == Threshold.Output(above=None, below=5)
 
-    results = component.run(value=15, threshold=10)
-    assert results == Threshold.Output(above=15, below=None)
+        results = component.run(value=15, threshold=10)
+        assert results == Threshold.Output(above=15, below=None)
```

### Comparing `canals-0.1.1/.gitignore` & `canals-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `canals-0.1.1/LICENSE` & `canals-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `canals-0.1.1/README.md` & `canals-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `canals-0.1.1/pyproject.toml` & `canals-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `canals-0.1.1/PKG-INFO` & `canals-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: canals
-Version: 0.1.1
+Version: 0.1.2
 Summary: A component orchestration engine for Haystack
 Project-URL: Documentation, https://github.com/deepset-ai/canals#readme
 Project-URL: Issues, https://github.com/deepset-ai/canals/issues
 Project-URL: Source, https://github.com/deepset-ai/canals
 Author-email: ZanSara <sara.zanzottera@deepset.ai>
 License-Expression: Apache-2.0
 License-File: LICENSE
```

