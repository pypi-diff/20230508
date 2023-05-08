# Comparing `tmp/fluidsdk-0.2.tar.gz` & `tmp/fluidsdk-0.3.tar.gz`

## Comparing `fluidsdk-0.2.tar` & `fluidsdk-0.3.tar`

### file list

```diff
@@ -1,35 +1,39 @@
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 fluidsdk-0.2/docs/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 fluidsdk-0.2/docs/make.bat
--rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 fluidsdk-0.2/docs/source/conf.py
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 fluidsdk-0.2/docs/source/fluid.rst
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 fluidsdk-0.2/docs/source/index.rst
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 fluidsdk-0.2/docs/source/_autosummary/fluidsdk.conversations_v3.Conversations_Model_v3.rst
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 fluidsdk-0.2/docs/source/_autosummary/fluidsdk.flow.Flow.rst
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 fluidsdk-0.2/docs/source/_autosummary/fluidsdk.flow.rst
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 fluidsdk-0.2/docs/source/_autosummary/fluidsdk.intents.rst
--rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 fluidsdk-0.2/docs/source/getting_started/example.py
--rw-r--r--   0        0        0     2677 2020-02-02 00:00:00.000000 fluidsdk-0.2/docs/source/getting_started/index.rst
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 fluidsdk-0.2/docs/source/pyrite/builder.rst
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 fluidsdk-0.2/docs/source/pyrite/index.rst
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 fluidsdk-0.2/docs/source/pyrite/library.rst
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 fluidsdk-0.2/src/fluidsdk/__init__.py
--rw-r--r--   0        0        0     8228 2020-02-02 00:00:00.000000 fluidsdk-0.2/src/fluidsdk/conversational_modules.py
--rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 fluidsdk-0.2/src/fluidsdk/conversations_v3.py
--rw-r--r--   0        0        0     6437 2020-02-02 00:00:00.000000 fluidsdk-0.2/src/fluidsdk/filters.py
--rw-r--r--   0        0        0     3068 2020-02-02 00:00:00.000000 fluidsdk-0.2/src/fluidsdk/flow.py
--rw-r--r--   0        0        0    18596 2020-02-02 00:00:00.000000 fluidsdk-0.2/src/fluidsdk/intents.py
--rw-r--r--   0        0        0    13243 2020-02-02 00:00:00.000000 fluidsdk-0.2/src/fluidsdk/macros.py
--rw-r--r--   0        0        0    15128 2020-02-02 00:00:00.000000 fluidsdk-0.2/src/fluidsdk/message.py
--rw-r--r--   0        0        0     5110 2020-02-02 00:00:00.000000 fluidsdk-0.2/src/fluidsdk/reminders.py
--rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 fluidsdk-0.2/src/fluidsdk/status_webhook.py
--rw-r--r--   0        0        0     3979 2020-02-02 00:00:00.000000 fluidsdk-0.2/src/fluidsdk/templates.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 fluidsdk-0.2/src/fluidsdk/pyrite/__init__.py
--rw-r--r--   0        0        0    23286 2020-02-02 00:00:00.000000 fluidsdk-0.2/src/fluidsdk/pyrite/builder.py
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 fluidsdk-0.2/src/fluidsdk/pyrite/consts.py
--rw-r--r--   0        0        0     8371 2020-02-02 00:00:00.000000 fluidsdk-0.2/src/fluidsdk/pyrite/library.py
--rw-r--r--   0        0        0     3633 2020-02-02 00:00:00.000000 fluidsdk-0.2/src/fluidsdk/pyrite/utils.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 fluidsdk-0.2/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fluidsdk-0.2/LICENSE
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 fluidsdk-0.2/README.md
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 fluidsdk-0.2/pyproject.toml
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 fluidsdk-0.2/PKG-INFO
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 fluidsdk-0.3/.readthedocs.yaml
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 fluidsdk-0.3/requirements.txt
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 fluidsdk-0.3/docs/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 fluidsdk-0.3/docs/make.bat
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 fluidsdk-0.3/docs/requirements.txt
+-rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 fluidsdk-0.3/docs/source/conf.py
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 fluidsdk-0.3/docs/source/fluid.rst
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 fluidsdk-0.3/docs/source/index.rst
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 fluidsdk-0.3/docs/source/_autosummary/fluidsdk.conversations_v3.Conversations_Model_v3.rst
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 fluidsdk-0.3/docs/source/_autosummary/fluidsdk.flow.Flow.rst
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 fluidsdk-0.3/docs/source/_autosummary/fluidsdk.flow.rst
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 fluidsdk-0.3/docs/source/_autosummary/fluidsdk.intents.rst
+-rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 fluidsdk-0.3/docs/source/getting_started/example.py
+-rw-r--r--   0        0        0     2677 2020-02-02 00:00:00.000000 fluidsdk-0.3/docs/source/getting_started/index.rst
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 fluidsdk-0.3/docs/source/pyrite/builder.rst
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 fluidsdk-0.3/docs/source/pyrite/index.rst
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 fluidsdk-0.3/docs/source/pyrite/library.rst
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 fluidsdk-0.3/src/fluidsdk/__init__.py
+-rw-r--r--   0        0        0     8347 2020-02-02 00:00:00.000000 fluidsdk-0.3/src/fluidsdk/conversational_modules.py
+-rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 fluidsdk-0.3/src/fluidsdk/conversations_v3.py
+-rw-r--r--   0        0        0     6437 2020-02-02 00:00:00.000000 fluidsdk-0.3/src/fluidsdk/filters.py
+-rw-r--r--   0        0        0     3068 2020-02-02 00:00:00.000000 fluidsdk-0.3/src/fluidsdk/flow.py
+-rw-r--r--   0        0        0    18784 2020-02-02 00:00:00.000000 fluidsdk-0.3/src/fluidsdk/intents.py
+-rw-r--r--   0        0        0    13243 2020-02-02 00:00:00.000000 fluidsdk-0.3/src/fluidsdk/macros.py
+-rw-r--r--   0        0        0    15138 2020-02-02 00:00:00.000000 fluidsdk-0.3/src/fluidsdk/message.py
+-rw-r--r--   0        0        0     5110 2020-02-02 00:00:00.000000 fluidsdk-0.3/src/fluidsdk/reminders.py
+-rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 fluidsdk-0.3/src/fluidsdk/status_webhook.py
+-rw-r--r--   0        0        0     3979 2020-02-02 00:00:00.000000 fluidsdk-0.3/src/fluidsdk/templates.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 fluidsdk-0.3/src/fluidsdk/pyrite/__init__.py
+-rw-r--r--   0        0        0    25303 2020-02-02 00:00:00.000000 fluidsdk-0.3/src/fluidsdk/pyrite/builder.py
+-rw-r--r--   0        0        0     4009 2020-02-02 00:00:00.000000 fluidsdk-0.3/src/fluidsdk/pyrite/consts.py
+-rw-r--r--   0        0        0    13097 2020-02-02 00:00:00.000000 fluidsdk-0.3/src/fluidsdk/pyrite/library.py
+-rw-r--r--   0        0        0     5400 2020-02-02 00:00:00.000000 fluidsdk-0.3/src/fluidsdk/pyrite/message.py
+-rw-r--r--   0        0        0     5032 2020-02-02 00:00:00.000000 fluidsdk-0.3/src/fluidsdk/pyrite/utils.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 fluidsdk-0.3/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fluidsdk-0.3/LICENSE
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 fluidsdk-0.3/README.md
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 fluidsdk-0.3/pyproject.toml
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 fluidsdk-0.3/PKG-INFO
```

### Comparing `fluidsdk-0.2/docs/Makefile` & `fluidsdk-0.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `fluidsdk-0.2/docs/make.bat` & `fluidsdk-0.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `fluidsdk-0.2/docs/source/conf.py` & `fluidsdk-0.3/docs/source/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,28 +14,29 @@
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 
 project = "FluidSDK"
 copyright = "2022, Shanti D'Vita"
 author = "Shanti D'Vita"
-release = "0.1"
+release = "0.3"
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = [
     "recommonmark",
     "sphinx.ext.autodoc",
     "sphinx.ext.viewcode",
     "sphinxcontrib.autodoc_pydantic",
     "sphinx_autodoc_typehints",
+    "sphinx_rtd_theme",
 ]
 
 templates_path = ["_templates"]
 exclude_patterns = ["_build", "Thumbs.db", ".DS_Store"]
 
 # -- Options for HTML output -------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#options-for-html-output
 
-html_theme = "alabaster"
+html_theme = "sphinx_rtd_theme"
 html_static_path = ["_static"]
```

### Comparing `fluidsdk-0.2/docs/source/getting_started/example.py` & `fluidsdk-0.3/docs/source/getting_started/example.py`

 * *Files identical despite different names*

### Comparing `fluidsdk-0.2/docs/source/getting_started/index.rst` & `fluidsdk-0.3/docs/source/getting_started/index.rst`

 * *Files identical despite different names*

### Comparing `fluidsdk-0.2/src/fluidsdk/conversational_modules.py` & `fluidsdk-0.3/src/fluidsdk/conversational_modules.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,22 +11,26 @@
 
 print = partial(print, flush=True)
 
 
 @_basemodel_decorator
 class OpenAIGPTConfig(BaseModel):
     engine: Literal[
+        "gpt-4",
+        "gpt-3.5-turbo",
+        "text-davinci-003",
         "text-davinci-002",
         "text-davinci-001",
         "text-curie-001",
         "text-babage-001",
         "text-ada-001",
         "code-davinci-002",
         "code-cushman-001",
         "text-davinci-insert-002",
+        "curie:ft-workhack-2022-10-28-22-55-34",
     ] = Field(
         "text-davinci-002",
         title="Engine",
         description="Name of the large language model to use.",
     )
     temperature: confloat(ge=0) = Field(
         0.5,
```

### Comparing `fluidsdk-0.2/src/fluidsdk/conversations_v3.py` & `fluidsdk-0.3/src/fluidsdk/conversations_v3.py`

 * *Files identical despite different names*

### Comparing `fluidsdk-0.2/src/fluidsdk/filters.py` & `fluidsdk-0.3/src/fluidsdk/filters.py`

 * *Files identical despite different names*

### Comparing `fluidsdk-0.2/src/fluidsdk/flow.py` & `fluidsdk-0.3/src/fluidsdk/flow.py`

 * *Files identical despite different names*

### Comparing `fluidsdk-0.2/src/fluidsdk/intents.py` & `fluidsdk-0.3/src/fluidsdk/intents.py`

 * *Files 1% similar despite different names*

```diff
@@ -175,14 +175,19 @@
         description="Field in the user's Conversation_Model.data to store the answer in.",
     )
     followups: int = Field(
         ...,
         title="Followups",
         description="Number of followups.",
     )
+    dynamic_stop_regex: Optional[str] = Field(
+        None,
+        title="Dynamic Stop Regex",
+        description="Regex to stop the conversaion once bot generates this trigger",
+    )
 
 
 @_basemodel_decorator
 class SayIntent(Intent):
     intent_type: Literal["say"] = "say"
     text: Union[str, List[BotMessageUnion]] = Field(
         ..., title="Question", description="A list of messages to send to the user."
```

### Comparing `fluidsdk-0.2/src/fluidsdk/macros.py` & `fluidsdk-0.3/src/fluidsdk/macros.py`

 * *Files identical despite different names*

### Comparing `fluidsdk-0.2/src/fluidsdk/message.py` & `fluidsdk-0.3/src/fluidsdk/message.py`

 * *Files 0% similar despite different names*

```diff
@@ -257,15 +257,15 @@
 class Message(BotMessage):
     type: Literal["text"] = "text"
     message: str
 
 
 @_basemodel_decorator
 class InteractiveMessageOption(BaseModel):
-    id: str = Field(
+    id: Optional[str] = Field(
         default_factory=lambda: "".join(random.choices(string.ascii_letters, k=8))
     )
     title: str = Field(..., title="Title")
     description: Optional[str] = Field("", title="Description")
 
     def __eq__(self, other):
         if isinstance(other, str):
```

### Comparing `fluidsdk-0.2/src/fluidsdk/reminders.py` & `fluidsdk-0.3/src/fluidsdk/reminders.py`

 * *Files identical despite different names*

### Comparing `fluidsdk-0.2/src/fluidsdk/status_webhook.py` & `fluidsdk-0.3/src/fluidsdk/status_webhook.py`

 * *Files identical despite different names*

### Comparing `fluidsdk-0.2/src/fluidsdk/templates.py` & `fluidsdk-0.3/src/fluidsdk/templates.py`

 * *Files identical despite different names*

### Comparing `fluidsdk-0.2/src/fluidsdk/pyrite/builder.py` & `fluidsdk-0.3/src/fluidsdk/pyrite/builder.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import astor
 import requests
 
 from fluidsdk.flow import Flow
 from fluidsdk.intents import (
     AskDefiniteIntent,
     AskOpenIntent,
+    ConditionIntent,
     ExpressionIntent,
     GPTGenerateIntent,
     SayIntent,
 )
 from fluidsdk.message import Message
 from fluidsdk.pyrite import library, utils
 from fluidsdk.pyrite.consts import ENGINE_GLOBALS, PYTHON_BUILTINS
@@ -137,56 +138,14 @@
         if isinstance(t, str):
             self.templates[t] = None
         elif isinstance(t, Template):
             self.templates[t.template_id] = t
         else:
             raise TypeError("This is not a Fluid Template.")
 
-    def build_expression(self, expression_node, prefix, old_context) -> str:
-        context = deepcopy(old_context)
-        context.builder = old_context.builder
-        context.step_contexts = old_context.step_contexts
-        context.flow_steps = {}
-        context.idx = 0
-        context.prefix = f"{prefix}-expression-{context.idx}"
-        raise_syntax_error = partial(
-            utils.raise_syntax_error, context.source_lines, context.filename
-        )
-
-        class RewriteName(ast.NodeTransformer):
-            def visit_Name(self, node):
-                # If name is a global variable, use as is.
-                if node.id in context.global_names:
-                    return node
-                # Else If, name is a local, index into data_stack
-                elif node.id in context.local_names:
-                    return ast.copy_location(
-                        ast.Subscript(
-                            value=ast.Subscript(
-                                value=ast.Name(id="data_stack", ctx=ast.Load()),
-                                slice=ast.UnaryOp(
-                                    op=ast.USub(), operand=ast.Constant(value=1)
-                                ),
-                                ctx=ast.Load(),
-                            ),
-                            slice=ast.Constant(value=node.id),
-                            ctx=node.ctx,
-                        ),
-                        node,
-                    )
-                # Else If, its a python built in. Return as is. (Example "int")
-                elif node.id in PYTHON_BUILTINS:
-                    return node
-                # Else name error
-                else:
-                    raise_syntax_error(node, f"Undefined variable `{node.id}`")
-
-        transformed_node = RewriteName().visit(expression_node)
-        return astor.to_source(transformed_node)[:-1]
-
     def build_body(self, body, prefix, old_context) -> dict:
         context = deepcopy(old_context)
         context.step_contexts = old_context.step_contexts
         context.builder = old_context.builder
         context.flow_steps = {}
         context.prefix = prefix
 
@@ -198,15 +157,33 @@
         )
 
         for node in body:
             # Line is an expression
             if isinstance(node, ast.Expr):
                 if isinstance(node.value, ast.Call):
                     call_node = node.value
-                    if call_node.func.id in statement_library:
+                    if isinstance(call_node.func, ast.Attribute):
+                        context_name = call_node.func.value.id
+                        if context_name not in context.step_contexts:
+                            raise_syntax_error(
+                                call_node.func.value, "Undefined Context."
+                            )
+                        ctx = context.step_contexts[context_name]
+                        if not isinstance(call_node.func.attr, str):
+                            raise_syntax_error(call_node.func, "Attribute error.")
+                        method = call_node.func.attr
+                        if method not in ctx.exports["statement_library"]:
+                            raise_syntax_error(
+                                call_node.func,
+                                "Attribute error. "
+                                + method
+                                + " does not exist in this context.",
+                            )
+                        utils.get_builder(getattr(ctx, method))(context, call_node)
+                    elif call_node.func.id in statement_library:
                         utils.get_builder(statement_library[call_node.func.id])(
                             context, call_node
                         )
                     elif call_node.func.id in self.subroutines:
                         utils.insert_then_increment(
                             context,
                             context.idx,
@@ -256,15 +233,15 @@
                             elif call_node.func.id in assignment_library:
                                 # If this is a library function, call handler
                                 utils.get_builder(
                                     assignment_library[call_node.func.id]
                                 )(context, call_node, target_field)
                             elif call_node.func.id in PYTHON_BUILTINS:
                                 # If node is a whitelisted python builtin, treat it as an expression
-                                expression = self.build_expression(
+                                expression = utils.build_expression(
                                     call_node, context.prefix, context
                                 )
                                 utils.insert_then_increment(
                                     context,
                                     context.idx,
                                     ExpressionIntent(
                                         expression=f"py>{expression}",
@@ -272,27 +249,27 @@
                                     ),
                                 )
                             else:
                                 raise_syntax_error(call_node, "Undefined subroutine.")
                         # Else if the call node is an Attribute or Subscript. Like `re.test(arg)` or `xyz["func"](arg)`
                         else:
                             # Treat it as an expression
-                            expression = self.build_expression(
+                            expression = utils.build_expression(
                                 call_node, context.prefix, context
                             )
                             utils.insert_then_increment(
                                 context,
                                 context.idx,
                                 ExpressionIntent(
                                     expression=f"py>{expression}",
                                     answer_field=target_field,
                                 ),
                             )
                     else:
-                        expression = self.build_expression(
+                        expression = utils.build_expression(
                             node.value, context.prefix, context
                         )
                         utils.insert_then_increment(
                             context,
                             context.idx,
                             ExpressionIntent(
                                 expression=f"py>{expression}", answer_field=target_field
@@ -382,24 +359,92 @@
                             ctx.body_context,
                         )
                 else:
                     raise_syntax_error(
                         context_manager_item.context_expr,
                         'This is not a context manager. Did you mean `with Context("context_name"):`?',
                     )
+            elif isinstance(node, ast.If):
+                self.build_if_statement(node, 0, context)
             else:
                 raise_syntax_error(
                     node,
                     "Unexpected Python Syntax. Pyrite does not support "
                     + str(type(node))
                     + " yet.",
                 )
             # print(ast.dump(node, indent=4))
         return context
 
+    def build_if_statement(
+        self, node: ast.If, if_else_idx, old_context, done_prefix=None
+    ):
+        context = deepcopy(old_context)
+        context.step_contexts = old_context.step_contexts
+        context.builder = old_context.builder
+        context.flow_steps = {}
+        add_done = False
+        if done_prefix is None:
+            add_done = True
+            done_prefix = old_context.prefix + "-" + str(old_context.idx) + "-if-done"
+
+        expression = utils.build_expression(node.test, context.prefix, context)
+        context.idx = if_else_idx
+        context.prefix = old_context.prefix + "-" + str(old_context.idx) + "-if"
+
+        utils.insert_then_increment(
+            context,
+            context.idx,
+            ConditionIntent(
+                condition="py>" + expression,
+                if_=context.prefix + "-" + str(if_else_idx) + "-body-0",
+                else_=old_context.prefix
+                + "-"
+                + str(old_context.idx)
+                + "-if-"
+                + str(if_else_idx + 1)
+                if len(node.orelse) > 0
+                else done_prefix,
+            ),
+        )
+        old_context.flow_steps.update(context.flow_steps)
+
+        context.idx = 0
+
+        body_context = self.build_body(
+            node.body,
+            context.prefix + "-" + str(if_else_idx) + "-body",
+            context,
+        )
+        list(body_context.flow_steps.values())[-1].next_ = done_prefix
+        old_context.flow_steps.update(body_context.flow_steps)
+
+        if len(node.orelse) == 0:
+            pass
+        elif len(node.orelse) == 1 and isinstance(node.orelse[0], ast.If):
+            else_node = node.orelse[0]
+            self.build_if_statement(
+                else_node, if_else_idx + 1, old_context, done_prefix
+            )
+        else:
+            else_node = ast.If(ast.Constant(True), node.orelse, [])
+            self.build_if_statement(
+                else_node, if_else_idx + 1, old_context, done_prefix
+            )
+
+        if add_done:
+            context.flow_steps = {}
+            context.prefix = done_prefix
+            utils.insert(
+                context, None, ExpressionIntent(expression="null", answer_field="null")
+            )
+            old_context.flow_steps.update(context.flow_steps)
+
+        old_context.idx += 1
+
     def build_function(self, f) -> dict:
         filename = inspect.getmodule(f).__file__
         source_lines, line_count = inspect.getsourcelines(f)
         f_ast_body = ast.parse(inspect.getsource(f)).body
         if len(f_ast_body) != 1:
             print(
                 "Subroutine invalid. Only pass functions to FlowBuilder.subroutine.",
@@ -472,17 +517,32 @@
             context.idx,
             ExpressionIntent(
                 expression="[data_stack, `{}`] | []",
                 answer_field="data_stack",
             ),
         )
 
-        func_context = self.build_body(func_def.body, func_def.name, context)
-        context.idx = func_context.idx
-        context.flow_steps.update(func_context.flow_steps)
+        ctx = utils.get_builder(library.Context)
+
+        with ctx(
+            None,
+            func_def.body,
+            context,
+            func_def.name,
+        ):
+            ctx.body_context.idx = context.idx
+            ctx.body_context = self.build_body(
+                func_def.body,
+                func_def.name,
+                ctx.body_context,
+            )
+
+        # func_context = self.build_body(func_def.body, , context)
+        context.idx = ctx.body_context.idx
+        context.flow_steps.update(ctx.body_context.flow_steps)
 
         # Pop the top of the data stack
         utils.insert_then_increment(
             context,
             context.idx,
             ExpressionIntent(
                 expression="data_stack[:-1]",
@@ -531,15 +591,15 @@
 
     def push_templates(self):
         """
         Push templates to engine. Access token is required.
         """
         assert self.token is not None, "Flow builder is in offline mode"
         for template_id, template in self.templates.items():
-            if isinstance(template, str):
+            if template is None:
                 continue
             logging.info(f"Updating template {template_id}")
             response = requests.patch(
                 f"{BASE_URL}/engine/templates/{template_id}",
                 headers={"Authorization": f"Bearer {self.token}"},
                 json=template.dict(),
             )
```

### Comparing `fluidsdk-0.2/pyproject.toml` & `fluidsdk-0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "pydantic", "pymongo"]
 build-backend = "hatchling.build"
 
 [project]
 name = "fluidsdk"
-version = "0.2"
+version = "0.3"
 authors = [{ name = "Shanti D'Vita", email = "shanti@workhack.io" }]
 description = "SDK for FluidVM"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.6"
 classifiers = [
   "Programming Language :: Python :: 3",
```

### Comparing `fluidsdk-0.2/PKG-INFO` & `fluidsdk-0.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fluidsdk
-Version: 0.2
+Version: 0.3
 Summary: SDK for FluidVM
 Project-URL: Homepage, https://workhack.io
 Author-email: Shanti D'Vita <shanti@workhack.io>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

