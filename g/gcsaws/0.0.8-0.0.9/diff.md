# Comparing `tmp/gcsaws-0.0.8.tar.gz` & `tmp/gcsaws-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gcsaws-0.0.8.tar", last modified: Mon May  8 07:32:11 2023, max compression
+gzip compressed data, was "gcsaws-0.0.9.tar", last modified: Mon May  8 10:40:03 2023, max compression
```

## Comparing `gcsaws-0.0.8.tar` & `gcsaws-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 07:32:11.011089 gcsaws-0.0.8/
--rw-rw-rw-   0        0        0     1091 2023-05-07 12:57:03.000000 gcsaws-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      412 2023-05-08 07:32:11.009842 gcsaws-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0        8 2023-05-07 12:56:41.000000 gcsaws-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-05-08 07:32:10.990031 gcsaws-0.0.8/gcsaws/
--rw-rw-rw-   0        0        0      191 2023-05-08 07:30:20.000000 gcsaws-0.0.8/gcsaws/__init__.py
--rw-rw-rw-   0        0        0      684 2023-05-08 07:29:33.000000 gcsaws-0.0.8/gcsaws/helpers.py
--rw-rw-rw-   0        0        0     7792 2023-05-08 07:23:26.000000 gcsaws-0.0.8/gcsaws/nodes.py
--rw-rw-rw-   0        0        0     4195 2023-05-08 07:28:17.000000 gcsaws-0.0.8/gcsaws/visitor_procedure.py
-drwxrwxrwx   0        0        0        0 2023-05-08 07:32:11.007842 gcsaws-0.0.8/gcsaws.egg-info/
--rw-rw-rw-   0        0        0      412 2023-05-08 07:32:10.000000 gcsaws-0.0.8/gcsaws.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      316 2023-05-08 07:32:10.000000 gcsaws-0.0.8/gcsaws.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 07:32:10.000000 gcsaws-0.0.8/gcsaws.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-05-08 07:32:10.000000 gcsaws-0.0.8/gcsaws.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-08 07:32:10.000000 gcsaws-0.0.8/gcsaws.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      663 2023-05-08 07:31:43.000000 gcsaws-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-08 07:32:11.011089 gcsaws-0.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-08 07:32:11.009842 gcsaws-0.0.8/tests/
--rw-rw-rw-   0        0        0      810 2023-05-07 11:28:19.000000 gcsaws-0.0.8/tests/test_create_target_list.py
--rw-rw-rw-   0        0        0     3424 2023-05-08 07:15:04.000000 gcsaws-0.0.8/tests/test_simple.py
+drwxrwxrwx   0        0        0        0 2023-05-08 10:40:03.967439 gcsaws-0.0.9/
+-rw-rw-rw-   0        0        0     1091 2023-05-07 12:57:03.000000 gcsaws-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      412 2023-05-08 10:40:03.967439 gcsaws-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0        8 2023-05-07 12:56:41.000000 gcsaws-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-05-08 10:40:03.953121 gcsaws-0.0.9/gcsaws/
+-rw-rw-rw-   0        0        0      226 2023-05-08 10:38:04.000000 gcsaws-0.0.9/gcsaws/__init__.py
+-rw-rw-rw-   0        0        0      684 2023-05-08 07:29:33.000000 gcsaws-0.0.9/gcsaws/helpers.py
+-rw-rw-rw-   0        0        0     8262 2023-05-08 09:24:20.000000 gcsaws-0.0.9/gcsaws/nodes.py
+-rw-rw-rw-   0        0        0     4156 2023-05-08 08:41:10.000000 gcsaws-0.0.9/gcsaws/visitor_procedure.py
+-rw-rw-rw-   0        0        0     3417 2023-05-08 09:37:22.000000 gcsaws-0.0.9/gcsaws/visitor_validation.py
+drwxrwxrwx   0        0        0        0 2023-05-08 10:40:03.963349 gcsaws-0.0.9/gcsaws.egg-info/
+-rw-rw-rw-   0        0        0      412 2023-05-08 10:40:03.000000 gcsaws-0.0.9/gcsaws.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      370 2023-05-08 10:40:03.000000 gcsaws-0.0.9/gcsaws.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 10:40:03.000000 gcsaws-0.0.9/gcsaws.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-05-08 10:40:03.000000 gcsaws-0.0.9/gcsaws.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-08 10:40:03.000000 gcsaws-0.0.9/gcsaws.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      663 2023-05-08 10:39:08.000000 gcsaws-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-08 10:40:03.967439 gcsaws-0.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-08 10:40:03.966437 gcsaws-0.0.9/tests/
+-rw-rw-rw-   0        0        0      810 2023-05-07 11:28:19.000000 gcsaws-0.0.9/tests/test_create_target_list.py
+-rw-rw-rw-   0        0        0     3460 2023-05-08 08:36:21.000000 gcsaws-0.0.9/tests/test_simple.py
+-rw-rw-rw-   0        0        0     1129 2023-05-08 10:36:09.000000 gcsaws-0.0.9/tests/test_validation.py
```

### Comparing `gcsaws-0.0.8/LICENSE` & `gcsaws-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `gcsaws-0.0.8/gcsaws/helpers.py` & `gcsaws-0.0.9/gcsaws/helpers.py`

 * *Files identical despite different names*

### Comparing `gcsaws-0.0.8/gcsaws/nodes.py` & `gcsaws-0.0.9/gcsaws/nodes.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,18 +4,17 @@
 
 from gcscore.mod import *
 
 T = TypeVar('T')
 
 __all__ = ['HasIdentifier', 'HasCompaction', 'HasCommand', 'HasTargets', 'HasPayload', 'HasScriptType',
            'HasInstanceState', 'HasFunctionName', 'HasInstanceState', 'HasDurationSeconds', 'AcceptChildScript',
-           'AcceptMerge', 'AcceptAnonymousChild', 'AcceptChildPause', 'AcceptChildWait', 'AcceptChildScriptTemplate',
-           'AcceptChildStepFunction', 'AcceptChildRunInOrder', 'AcceptChildRunInParallel', 'NodeRunInOrder',
-           'NodeRunInParallel', 'NodeWait', 'NodePause', 'NodeScript', 'NodeScriptTemplate', 'NodeStepFunction',
-           'NodeChangeInstanceState']
+           'AcceptChildPause', 'AcceptChildWait', 'AcceptChildScriptTemplate', 'AcceptChildStepFunction',
+           'AcceptChildRunInOrder', 'AcceptChildRunInParallel', 'NodeRunInOrder', 'NodeRunInParallel', 'NodeWait',
+           'NodePause', 'NodeScript', 'NodeScriptTemplate', 'NodeStepFunction', 'NodeChangeInstanceState']
 
 
 # <editor-fold desc="Trait attributes">
 
 class HasDurationSeconds:
     gcsaws_duration: int = 5
 
@@ -39,15 +38,15 @@
         :return: self
         """
         self.gcsaws_identifier = identifier_
         return self
 
 
 class HasScriptType:
-    gcsaws_script_type: str = 'shell'
+    gcsaws_script_type: str = None
 
     def shell(self: T) -> T:
         """
         Makes the node run a shell script/command.
         :return: self
         """
         self.gcsaws_script_type = 'shell'
@@ -73,25 +72,28 @@
         """
         self.gcsaws_command = cmd
         return self
 
 
 class HasTargets:
     gcsaws_targets: list[dict]
+    gcsaws_targets_initialized: bool
 
     def __gcs__init__(self, **_):
         self.gcsaws_targets = []
+        self.gcsaws_targets_initialized = False
 
     def on_targets(self: T, targets: list[dict]) -> T:
         """
         Adds the targets to the node.
         :param targets: list of the targets
         :return: self
         """
         self.gcsaws_targets.extend(targets)
+        self.gcsaws_targets_initialized = True
         return self
 
 
 class HasCompaction:
     gcsaws_compaction: bool = False
 
     def compact(self: T) -> T:
@@ -100,41 +102,41 @@
         :return: self
         """
         self.gcsaws_compaction = True
         return self
 
 
 class HasFunctionName:
-    gcsaws_function_name: str
+    gcsaws_function_name: str = None
 
     def function_name(self: T, name: str) -> T:
         """
         Sets the name of the function called by the node.
         :param name: function's name
         :return: self
         """
         self.gcsaws_function_name = name
         return self
 
 
 class HasPayload:
-    gcsaws_payload: dict
+    gcsaws_payload: dict = None
 
     def payload(self: T, payload: dict) -> T:
         """
         Sets the payload of the node.
         :param payload: the payload dictionary
         :return: self
         """
         self.gcsaws_payload = payload
         return self
 
 
 class HasInstanceState:
-    gcsaws_instance_state: str
+    gcsaws_instance_state: str = None
 
     def power_on(self: T) -> T:
         """
         Mark the wanted state as "running"
         :return: self
         """
         self.gcsaws_instance_state = 'running'
@@ -219,14 +221,24 @@
         Run a step function.
         :param name: node's name
         :return: the child node
         """
         return add_child(self, NodeStepFunction, name=name)
 
 
+class AcceptChildChangeInstanceState:
+    def change_instance_state(self: HasChildren, name: str) -> NodeChangeInstanceState:
+        """
+        Power on or off the targets.
+        :param name: node(s name
+        :return: the child node
+        """
+        return add_child(self, NodeChangeInstanceState, name=name)
+
+
 # </editor-fold>
 
 # <editor-fold desc="Nodes">
 class _ComposedNode(
     BaseNode,
     HasName,
     HasDescription,
@@ -235,15 +247,16 @@
     AcceptMerge,
     AcceptChildWait,
     AcceptChildPause,
     AcceptChildRunInOrder,
     AcceptChildRunInParallel,
     AcceptChildScript,
     AcceptChildScriptTemplate,
-    AcceptChildStepFunction
+    AcceptChildStepFunction,
+    AcceptChildChangeInstanceState
 ):
     pass
 
 
 class NodeRunInParallel(_ComposedNode):
     __visitor_method__ = 'visit_run_in_parallel'
```

### Comparing `gcsaws-0.0.8/gcsaws/visitor_procedure.py` & `gcsaws-0.0.9/gcsaws/visitor_procedure.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,22 +2,21 @@
 from functools import partial
 from typing import Union
 
 import jinja2
 
 from gcscore import CommandRenderer
 from gcscore.mod import Visitor, compact_script
-from .nodes import NodePause, NodeWait, NodeRunInOrder, NodeRunInParallel, NodeScript, NodeScriptTemplate, \
-    NodeStepFunction, NodeChangeInstanceState
+from gcsaws.nodes import *
 
-__all__ = ['VisitorState', 'setup_procedure_visitor']
+__all__ = ['VisitorStateProcedure', 'setup_procedure_visitor']
 
 
 @dataclass
-class VisitorState:
+class VisitorStateProcedure:
     command_renderer: CommandRenderer
     j2env: jinja2.Environment
     root: list = field(default_factory=list)
     current: list = field(init=False)
 
     def __post_init__(self):
         self.current = self.root
@@ -33,15 +32,15 @@
     visitor.register('visit_run_in_order', partial(_visit_composed_node, node_type='ordered'))
     visitor.register('visit_run_in_parallel', partial(_visit_composed_node, node_type='async'))
 
 
 ComposedNode = Union[NodeRunInOrder, NodeRunInParallel]
 
 
-def _visit_composed_node(visitor: Visitor, node: ComposedNode, state: VisitorState, node_type: str):
+def _visit_composed_node(visitor: Visitor, node: ComposedNode, state: VisitorStateProcedure, node_type: str):
     result = {
         'name': node.gcscore_name,
         'description': node.gcscore_description,
         'type': node_type,
         'nodes': []
     }
     old_current = state.current
@@ -49,73 +48,73 @@
     [visitor.visit(child, state) for child in node.gcscore_children]
     state.current = old_current
 
     if len(result['nodes']) > 0:
         state.current.append(result)
 
 
-def _visit_wait(_visitor: Visitor, node: NodeWait, state: VisitorState):
+def _visit_wait(_visitor: Visitor, node: NodeWait, state: VisitorStateProcedure):
     state.current.append({
         'name': node.gcscore_name,
         'description': node.gcscore_description,
         'type': 'wait',
         'duration': node.gcsaws_duration
     })
 
 
-def _visit_pause(_visitor: Visitor, node: NodePause, state: VisitorState):
+def _visit_pause(_visitor: Visitor, node: NodePause, state: VisitorStateProcedure):
     state.current.append({
         'name': node.gcscore_name,
         'description': node.gcscore_description,
         'type': 'pause',
         'identifier': node.gcsaws_identifier
     })
 
 
-def _script_like(_visitor: Visitor, node: Union[NodeScript, NodeScriptTemplate], state: VisitorState,
+def _script_like(_visitor: Visitor, node: Union[NodeScript, NodeScriptTemplate], state: VisitorStateProcedure,
                  script: str):
     if node.gcsaws_compaction:
         script = compact_script(node.gcsaws_script_type, script)
 
     state.current.append({
         'name': node.gcscore_name,
         'description': node.gcscore_description,
         'type': node.gcsaws_script_type,
         'language': node.gcsaws_script_type,
         'commands': script.splitlines(),
         'targets': node.gcsaws_targets
     })
 
 
-def _visit_script(visitor: Visitor, node: NodeScript, state: VisitorState):
+def _visit_script(visitor: Visitor, node: NodeScript, state: VisitorStateProcedure):
     if len(node.gcsaws_targets) == 0:
         return
 
     _script_like(visitor, node, state, node.gcsaws_command)
 
 
-def _visit_script_template(visitor: Visitor, node: NodeScriptTemplate, state: VisitorState):
+def _visit_script_template(visitor: Visitor, node: NodeScriptTemplate, state: VisitorStateProcedure):
     if len(node.gcsaws_targets) == 0:
         return
 
     script = state.command_renderer.render_command(node.gcsaws_command, state.j2env)
     _script_like(visitor, node, state, script)
 
 
-def _visit_step_function(_visitor: Visitor, node: NodeStepFunction, state: VisitorState):
+def _visit_step_function(_visitor: Visitor, node: NodeStepFunction, state: VisitorStateProcedure):
     state.current.append({
         'name': node.gcscore_name,
         'description': node.gcscore_description,
         'type': 'stepfunction',
         'stepfunction': node.gcsaws_function_name,
         'payload': node.gcsaws_payload,
     })
 
 
-def _visit_change_instance_state(_visitor: Visitor, node: NodeChangeInstanceState, state: VisitorState):
+def _visit_change_instance_state(_visitor: Visitor, node: NodeChangeInstanceState, state: VisitorStateProcedure):
     if len(node.gcsaws_targets) == 0:
         return
 
     state.current.append({
         'name': node.gcscore_name,
         'description': node.gcscore_description,
         'type': 'change-instance-state',
```

### Comparing `gcsaws-0.0.8/pyproject.toml` & `gcsaws-0.0.9/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gcsaws"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
     { name="Leikt", email="leikt.solreihin@gmail.com" },
 ]
 description = "GCS implementation for the aws-automation package."
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-    "gcscore>=0.0.10"
+    "gcscore>=0.0.16"
 ]
 #[project.urls]
 #"Homepage" = "https://github.com/pypa/sampleproject"
 #"Bug Tracker" = "https://github.com/pypa/sampleproject/issues"
```

### Comparing `gcsaws-0.0.8/tests/test_create_target_list.py` & `gcsaws-0.0.9/tests/test_create_target_list.py`

 * *Files identical despite different names*

### Comparing `gcsaws-0.0.8/tests/test_simple.py` & `gcsaws-0.0.9/tests/test_simple.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import unittest
 from pathlib import Path
 
 import jinja2
 
 from gcsaws.nodes import *
-from gcsaws.visitor_procedure import VisitorState, setup_procedure_visitor
+from gcsaws.visitor_procedure import VisitorStateProcedure, setup_procedure_visitor
 from gcscore import CommandRenderer, ScriptTemplatesExtension
 from gcscore.mod import Visitor, BaseContext, SearchableList, import_module
 
 
 class TestGCSAws(unittest.TestCase):
     def test_simple(self):
         # Build procedure
@@ -21,15 +21,15 @@
         sub_proc.wait('hello').duration(15)
 
         sub_proc2 = NodeRunInOrder(name='sub2')
         sub_proc2.wait('XOXO').duration(5)
         root.child(sub_proc2)
 
         # Visit
-        visitor_state = VisitorState(None, None)
+        visitor_state = VisitorStateProcedure(None, None)
         visitor = Visitor()
         setup_procedure_visitor(visitor)
         visitor.visit(root, visitor_state)
         final = visitor_state.root[0]
         pass
 
     def test_script_template(self):
@@ -40,15 +40,15 @@
         root.run_script('test1').shell().command('echo "Hello world!"').on_targets(targets)
         root.run_script_template('test2').command('script01.sh Robin').shell().on_targets(targets)
         root.run_script_template('test3').command('script01.sh Robin').shell().on_targets([])
 
         cmd_renderer = CommandRenderer()
         ScriptTemplatesExtension.configure(cmd_renderer)
         j2env = jinja2.Environment(loader=jinja2.FileSystemLoader('data'), extensions=[ScriptTemplatesExtension])
-        visitor_state = VisitorState(cmd_renderer, j2env)
+        visitor_state = VisitorStateProcedure(cmd_renderer, j2env)
         visitor = Visitor()
         setup_procedure_visitor(visitor)
         visitor.visit(root, visitor_state)
         final = visitor_state.root[0]
 
         self.assertEqual(0, len(cmd_renderer.errors_history))
         pass
@@ -70,15 +70,15 @@
 
         proc_module = import_module('__imported_proc__', 'data/proc01.py')
         proc = proc_module.main(context)
 
         cmd_renderer = CommandRenderer()
         ScriptTemplatesExtension.configure(cmd_renderer)
         j2env = jinja2.Environment(loader=jinja2.FileSystemLoader('data'), extensions=[ScriptTemplatesExtension])
-        visitor_state = VisitorState(cmd_renderer, j2env)
+        visitor_state = VisitorStateProcedure(cmd_renderer, j2env)
         visitor = Visitor()
         setup_procedure_visitor(visitor)
         visitor.visit(proc, visitor_state)
         cmd_renderer.errors_history.render()
         final = visitor_state.root[0]
         Path('data/proc01.json').write_text(json.dumps(final, indent=4))
         pass
```

