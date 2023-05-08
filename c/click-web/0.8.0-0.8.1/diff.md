# Comparing `tmp/click-web-0.8.0.tar.gz` & `tmp/click-web-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "click-web-0.8.0.tar", last modified: Wed Nov 10 12:51:31 2021, max compression
+gzip compressed data, was "click-web-0.8.1.tar", last modified: Mon May  8 21:19:40 2023, max compression
```

## Comparing `click-web-0.8.0.tar` & `click-web-0.8.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-10 12:51:31.176671 click-web-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (121)      120 2021-11-10 12:51:22.000000 click-web-0.8.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1077 2021-11-10 12:51:22.000000 click-web-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       76 2021-11-10 12:51:22.000000 click-web-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3645 2021-11-10 12:51:31.176671 click-web-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2701 2021-11-10 12:51:22.000000 click-web-0.8.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-10 12:51:31.172671 click-web-0.8.0/click_web/
--rw-r--r--   0 runner    (1001) docker     (121)     2720 2021-11-10 12:51:22.000000 click-web-0.8.0/click_web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       98 2021-11-10 12:51:22.000000 click-web-0.8.0/click_web/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-10 12:51:31.172671 click-web-0.8.0/click_web/resources/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-10 12:51:22.000000 click-web-0.8.0/click_web/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    16623 2021-11-10 12:51:22.000000 click-web-0.8.0/click_web/resources/cmd_exec.py
--rw-r--r--   0 runner    (1001) docker     (121)     4062 2021-11-10 12:51:22.000000 click-web-0.8.0/click_web/resources/cmd_form.py
--rw-r--r--   0 runner    (1001) docker     (121)     1445 2021-11-10 12:51:22.000000 click-web-0.8.0/click_web/resources/index.py
--rw-r--r--   0 runner    (1001) docker     (121)     9897 2021-11-10 12:51:22.000000 click-web-0.8.0/click_web/resources/input_fields.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-10 12:51:31.176671 click-web-0.8.0/click_web/static/
--rw-r--r--   0 runner    (1001) docker     (121)     1813 2021-11-10 12:51:22.000000 click-web-0.8.0/click_web/static/click_web.css
--rw-r--r--   0 runner    (1001) docker     (121)      360 2021-11-10 12:51:22.000000 click-web-0.8.0/click_web/static/copy_to_clipboard.js
--rw-r--r--   0 runner    (1001) docker     (121)     1171 2021-11-10 12:51:22.000000 click-web-0.8.0/click_web/static/open_form.js
--rw-r--r--   0 runner    (1001) docker     (121)      721 2021-11-10 12:51:22.000000 click-web-0.8.0/click_web/static/panes.css
--rw-r--r--   0 runner    (1001) docker     (121)      242 2021-11-10 12:51:22.000000 click-web-0.8.0/click_web/static/panes.js
--rw-r--r--   0 runner    (1001) docker     (121)     4755 2021-11-10 12:51:22.000000 click-web-0.8.0/click_web/static/post_and_read.js
--rw-r--r--   0 runner    (1001) docker     (121)    28846 2021-11-10 12:51:22.000000 click-web-0.8.0/click_web/static/pure.css
--rw-r--r--   0 runner    (1001) docker     (121)    29958 2021-11-10 12:51:22.000000 click-web-0.8.0/click_web/static/split.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-10 12:51:31.176671 click-web-0.8.0/click_web/templates/
--rw-r--r--   0 runner    (1001) docker     (121)     2691 2021-11-10 12:51:22.000000 click-web-0.8.0/click_web/templates/command_form.html.j2
--rw-r--r--   0 runner    (1001) docker     (121)     2305 2021-11-10 12:51:22.000000 click-web-0.8.0/click_web/templates/form_macros.html.j2
--rw-r--r--   0 runner    (1001) docker     (121)     2021 2021-11-10 12:51:22.000000 click-web-0.8.0/click_web/templates/show_tree.html.j2
--rw-r--r--   0 runner    (1001) docker     (121)     1024 2021-11-10 12:51:22.000000 click-web-0.8.0/click_web/web_click_types.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-10 12:51:31.172671 click-web-0.8.0/click_web.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3645 2021-11-10 12:51:30.000000 click-web-0.8.0/click_web.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1179 2021-11-10 12:51:31.000000 click-web-0.8.0/click_web.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-10 12:51:30.000000 click-web-0.8.0/click_web.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-10 12:51:30.000000 click-web-0.8.0/click_web.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      136 2021-11-10 12:51:30.000000 click-web-0.8.0/click_web.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2021-11-10 12:51:30.000000 click-web-0.8.0/click_web.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      192 2021-11-10 12:51:31.176671 click-web-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1570 2021-11-10 12:51:22.000000 click-web-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-10 12:51:31.176671 click-web-0.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-10 12:51:22.000000 click-web-0.8.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      142 2021-11-10 12:51:22.000000 click-web-0.8.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-10 12:51:31.176671 click-web-0.8.0/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-10 12:51:22.000000 click-web-0.8.0/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      360 2021-11-10 12:51:22.000000 click-web-0.8.0/tests/fixtures/click_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (121)      367 2021-11-10 12:51:22.000000 click-web-0.8.0/tests/fixtures/flask_fixtures.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-10 12:51:31.176671 click-web-0.8.0/tests/fixtures/script/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-10 12:51:22.000000 click-web-0.8.0/tests/fixtures/script/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2928 2021-11-10 12:51:22.000000 click-web-0.8.0/tests/fixtures/script/a_script.py
--rw-r--r--   0 runner    (1001) docker     (121)      138 2021-11-10 12:51:22.000000 click-web-0.8.0/tests/fixtures/script/app.py
--rw-r--r--   0 runner    (1001) docker     (121)     8787 2021-11-10 12:51:22.000000 click-web-0.8.0/tests/test_click_web.py
--rw-r--r--   0 runner    (1001) docker     (121)     2449 2021-11-10 12:51:22.000000 click-web-0.8.0/tests/test_flask_get.py
--rw-r--r--   0 runner    (1001) docker     (121)     3751 2021-11-10 12:51:22.000000 click-web-0.8.0/tests/test_flask_post.py
--rw-r--r--   0 runner    (1001) docker     (121)     1540 2021-11-10 12:51:22.000000 click-web-0.8.0/tests/test_request_parsing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:19:40.177404 click-web-0.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-08 21:19:25.000000 click-web-0.8.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-08 21:19:25.000000 click-web-0.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-08 21:19:25.000000 click-web-0.8.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-05-08 21:19:40.177404 click-web-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-05-08 21:19:25.000000 click-web-0.8.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:19:40.173404 click-web-0.8.1/click_web/
+-rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-05-08 21:19:25.000000 click-web-0.8.1/click_web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-08 21:19:25.000000 click-web-0.8.1/click_web/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:19:40.177404 click-web-0.8.1/click_web/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 21:19:25.000000 click-web-0.8.1/click_web/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16921 2023-05-08 21:19:25.000000 click-web-0.8.1/click_web/resources/cmd_exec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-05-08 21:19:25.000000 click-web-0.8.1/click_web/resources/cmd_form.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-05-08 21:19:25.000000 click-web-0.8.1/click_web/resources/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10237 2023-05-08 21:19:25.000000 click-web-0.8.1/click_web/resources/input_fields.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:19:40.177404 click-web-0.8.1/click_web/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-05-08 21:19:25.000000 click-web-0.8.1/click_web/static/click_web.css
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-08 21:19:25.000000 click-web-0.8.1/click_web/static/copy_to_clipboard.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-08 21:19:25.000000 click-web-0.8.1/click_web/static/open_form.js
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-08 21:19:25.000000 click-web-0.8.1/click_web/static/panes.css
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-08 21:19:25.000000 click-web-0.8.1/click_web/static/panes.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-05-08 21:19:25.000000 click-web-0.8.1/click_web/static/post_and_read.js
+-rw-r--r--   0 runner    (1001) docker     (123)    28846 2023-05-08 21:19:25.000000 click-web-0.8.1/click_web/static/pure.css
+-rw-r--r--   0 runner    (1001) docker     (123)    29958 2023-05-08 21:19:25.000000 click-web-0.8.1/click_web/static/split.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:19:40.177404 click-web-0.8.1/click_web/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-05-08 21:19:25.000000 click-web-0.8.1/click_web/templates/command_form.html.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-05-08 21:19:25.000000 click-web-0.8.1/click_web/templates/form_macros.html.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-05-08 21:19:25.000000 click-web-0.8.1/click_web/templates/show_tree.html.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-08 21:19:25.000000 click-web-0.8.1/click_web/web_click_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:19:40.173404 click-web-0.8.1/click_web.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-05-08 21:19:40.000000 click-web-0.8.1/click_web.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-08 21:19:40.000000 click-web-0.8.1/click_web.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 21:19:40.000000 click-web-0.8.1/click_web.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 21:19:40.000000 click-web-0.8.1/click_web.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-08 21:19:40.000000 click-web-0.8.1/click_web.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-08 21:19:40.000000 click-web-0.8.1/click_web.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-08 21:19:40.177404 click-web-0.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-05-08 21:19:25.000000 click-web-0.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:19:40.177404 click-web-0.8.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 21:19:25.000000 click-web-0.8.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-08 21:19:25.000000 click-web-0.8.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:19:40.177404 click-web-0.8.1/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 21:19:25.000000 click-web-0.8.1/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-08 21:19:25.000000 click-web-0.8.1/tests/fixtures/click_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-08 21:19:25.000000 click-web-0.8.1/tests/fixtures/flask_fixtures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:19:40.177404 click-web-0.8.1/tests/fixtures/script/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 21:19:25.000000 click-web-0.8.1/tests/fixtures/script/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-05-08 21:19:25.000000 click-web-0.8.1/tests/fixtures/script/a_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-08 21:19:25.000000 click-web-0.8.1/tests/fixtures/script/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8787 2023-05-08 21:19:25.000000 click-web-0.8.1/tests/test_click_web.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-05-08 21:19:25.000000 click-web-0.8.1/tests/test_flask_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-05-08 21:19:25.000000 click-web-0.8.1/tests/test_flask_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-08 21:19:25.000000 click-web-0.8.1/tests/test_request_parsing.py
```

### Comparing `click-web-0.8.0/LICENSE` & `click-web-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `click-web-0.8.0/PKG-INFO` & `click-web-0.8.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: click-web
-Version: 0.8.0
+Version: 0.8.1
 Summary: Serve click scripts over the web with minimal effort.
 Home-page: https://github.com/fredrik-corneliusson/click-web
 Author: Fredrik Corneliusson
 Author-email: fredrik.corneliusson@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: User Interfaces
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: System :: Shells
@@ -128,9 +127,7 @@
 
 
 Included 3:rd party libraries
 =============================
 `SplitJs`_ - Copyright (c) 2020 Nathan Cahill (MIT license)
 
 .. _SplitJs: https://github.com/nathancahill/split/blob/master/packages/splitjs/LICENSE.txt
-
-
```

### Comparing `click-web-0.8.0/README.rst` & `click-web-0.8.1/README.rst`

 * *Files identical despite different names*

### Comparing `click-web-0.8.0/click_web/__init__.py` & `click-web-0.8.1/click_web/__init__.py`

 * *Files identical despite different names*

### Comparing `click-web-0.8.0/click_web/resources/cmd_exec.py` & `click-web-0.8.1/click_web/resources/cmd_exec.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,16 +139,15 @@
     uri = f'/static/results/{rel_file_path.as_posix()}'
     return f'<a href="{uri}">{field_info.link_name}</a>'
 
 
 class CommandLine:
     def __init__(self, script_file_path: str, commands: List[str]):
         self._parts: List[CmdPart] = list()
-        # run with same python executable we are running with.
-        self.append(sys.executable)
+        self.append(_get_python_interpreter())
         self.append(script_file_path)
 
         self.command_line_bulder = FormToCommandLineBuilder(self)
 
         # root command_index should not add a command
         self.command_line_bulder.add_command_args(0)
         for i, command in enumerate(commands):
@@ -172,14 +171,24 @@
 
     def after_script_executed(self):
         """Call this after the command has executed"""
         for fi in self.command_line_bulder.field_infos:
             fi.after_script_executed()
 
 
+def _get_python_interpreter():
+    if sys.executable.endswith("uwsgi"):
+        import uwsgi
+        python_interpreter = str((Path(uwsgi.opt.get("virtualenv").decode()) / "bin"/ "python").absolute())
+    else:
+        # run with same python executable we are running with.
+        python_interpreter = sys.executable
+    return python_interpreter
+
+
 class CmdPart:
     def __init__(self, part: str, secret=False):
         self.part = part
         self.secret = secret
 
     def __str__(self):
         return self.part
```

### Comparing `click-web-0.8.0/click_web/resources/cmd_form.py` & `click-web-0.8.1/click_web/resources/cmd_form.py`

 * *Files identical despite different names*

### Comparing `click-web-0.8.0/click_web/resources/index.py` & `click-web-0.8.1/click_web/resources/index.py`

 * *Files identical despite different names*

### Comparing `click-web-0.8.0/click_web/resources/input_fields.py` & `click-web-0.8.1/click_web/resources/input_fields.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import click
 
-from click_web.web_click_types import EmailParamType, PasswordParamType
+from click_web.web_click_types import (EmailParamType, PasswordParamType,
+                                       TextAreaParamType)
 
 
 class FieldId:
     """
     Extract/serialize information from the encoded form input field name
     the parts:
         [command_index].[opt_or_arg_index].[click_type].[html_input_type].[opt_or_arg_name]
@@ -267,14 +268,25 @@
     def type_attrs(self):
         type_attrs = {}
         type_attrs["type"] = "password"
         type_attrs["click_type"] = "password"
         return type_attrs
 
 
+class TextAreaInput(BaseInput):
+    param_type_cls = TextAreaParamType
+
+    @property
+    def type_attrs(self):
+        type_attrs = {}
+        type_attrs['type'] = 'textarea'
+        type_attrs['click_type'] = 'textarea'
+        return type_attrs
+
+
 class DefaultInput(BaseInput):
     param_type_cls = click.ParamType
 
     @property
     def type_attrs(self):
         type_attrs = {}
         type_attrs['type'] = 'text'
@@ -290,15 +302,16 @@
 INPUT_TYPES = [ChoiceInput,
                FlagInput,
                IntInput,
                FloatInput,
                FolderInput,
                FileInput,
                EmailInput,
-               PasswordInput]
+               PasswordInput,
+               TextAreaInput]
 
 _DEFAULT_INPUT = [DefaultInput]
 
 
 def get_input_field(ctx: click.Context, param: click.Parameter, command_index, param_index) -> dict:
     """
     Convert a click.Parameter into a dict structure describing a html form option
```

### Comparing `click-web-0.8.0/click_web/static/click_web.css` & `click-web-0.8.1/click_web/static/click_web.css`

 * *Files identical despite different names*

### Comparing `click-web-0.8.0/click_web/static/open_form.js` & `click-web-0.8.1/click_web/static/open_form.js`

 * *Files identical despite different names*

### Comparing `click-web-0.8.0/click_web/static/panes.css` & `click-web-0.8.1/click_web/static/panes.css`

 * *Files identical despite different names*

### Comparing `click-web-0.8.0/click_web/static/post_and_read.js` & `click-web-0.8.1/click_web/static/post_and_read.js`

 * *Files identical despite different names*

### Comparing `click-web-0.8.0/click_web/static/pure.css` & `click-web-0.8.1/click_web/static/pure.css`

 * *Files identical despite different names*

### Comparing `click-web-0.8.0/click_web/static/split.js` & `click-web-0.8.1/click_web/static/split.js`

 * *Files identical despite different names*

### Comparing `click-web-0.8.0/click_web/templates/command_form.html.j2` & `click-web-0.8.1/click_web/templates/command_form.html.j2`

 * *Files identical despite different names*

### Comparing `click-web-0.8.0/click_web/templates/form_macros.html.j2` & `click-web-0.8.1/click_web/templates/form_macros.html.j2`

 * *Files 6% similar despite different names*

```diff
@@ -6,30 +6,39 @@
             {#
             Hack to work with flags that are default on.
             As checkbox is only sent down when checked we duplicate
             hidden field that is always sent but with empty value.
             https://stackoverflow.com/a/1992745/1306577 #}
             <input name="{{ field.name }}" type='hidden' value='{{ field.off_flag }}'>
         {% endif %}
-        <input name="{{ field.name }}"
-               id="{{ field.name }}"
-               type="{{ field.type }}"
-                {% if field.step %} step="{{ field.step }}"{% endif %}
-                {% if field.accept %} accept="{{ field.accept }}"{% endif %}
-                {# For variadic options with fixed number of args more then 1 then the default value is a
-                   list with the default value for each narg #}
-                {% if field.nargs > 1 %} value="{{ field.value[narg]|default('', true) }}"
-                {# only one option so just use the value set as default #}
-                {% else %} value="{{ field.value|default('', true) }}" {% endif %}
+        {% if field.type == "textarea"  %}
+            <textarea name="{{ field.name }}"
+                      id="{{ field.name }}"
+                      cols="80" rows="7"
+                      {{ 'required' if field.required else '' }}
+                        >{{ field.value|default('', true) }}</textarea>
+        {% else %}
 
-                {{ field.checked }}
-                {{ 'required' if field.required else '' }}
+            <input name="{{ field.name }}"
+                   id="{{ field.name }}"
+                   type="{{ field.type }}"
+                    {% if field.step %} step="{{ field.step }}"{% endif %}
+                    {% if field.accept %} accept="{{ field.accept }}"{% endif %}
+                    {# For variadic options with fixed number of args more then 1 then the default value is a
+                       list with the default value for each narg #}
+                    {% if field.nargs > 1 %} value="{{ field.value[narg]|default('', true) }}"
+                    {# only one option so just use the value set as default #}
+                    {% else %} value="{{ field.value|default('', true) }}" {% endif %}
 
+                    {{ field.checked }}
+                    {{ 'required' if field.required else '' }}
 
-        >
+
+            >
+        {% endif %}
     {% endif %}
 
 {%- endmacro %}
 
 {% macro add_option_field(field) -%}
     <select name="{{ field.name }}">
         {% for option in field.options %}
```

### Comparing `click-web-0.8.0/click_web/templates/show_tree.html.j2` & `click-web-0.8.1/click_web/templates/show_tree.html.j2`

 * *Files identical despite different names*

### Comparing `click-web-0.8.0/click_web/web_click_types.py` & `click-web-0.8.1/click_web/web_click_types.py`

 * *Files 23% similar despite different names*

```diff
@@ -31,9 +31,17 @@
 class PasswordParamType(click.ParamType):
     name = "password"
 
     def convert(self, value, param, ctx):
         return value
 
 
+class TextAreaParamType(click.ParamType):
+    name = "textarea"
+
+    def convert(self, value, param, ctx):
+        return value
+
+
 EMAIL_TYPE = EmailParamType()
 PASSWORD_TYPE = PasswordParamType()
+TEXTAREA_TYPE = TextAreaParamType()
```

### Comparing `click-web-0.8.0/click_web.egg-info/PKG-INFO` & `click-web-0.8.1/click_web.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: click-web
-Version: 0.8.0
+Version: 0.8.1
 Summary: Serve click scripts over the web with minimal effort.
 Home-page: https://github.com/fredrik-corneliusson/click-web
 Author: Fredrik Corneliusson
 Author-email: fredrik.corneliusson@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: User Interfaces
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: System :: Shells
@@ -128,9 +127,7 @@
 
 
 Included 3:rd party libraries
 =============================
 `SplitJs`_ - Copyright (c) 2020 Nathan Cahill (MIT license)
 
 .. _SplitJs: https://github.com/nathancahill/split/blob/master/packages/splitjs/LICENSE.txt
-
-
```

### Comparing `click-web-0.8.0/click_web.egg-info/SOURCES.txt` & `click-web-0.8.1/click_web.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `click-web-0.8.0/setup.py` & `click-web-0.8.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     'twine>=3.4',
     'wheel'
 ]
 
 
 setup(
     name='click-web',
-    version='0.8.0',
+    version='0.8.1',
     url='https://github.com/fredrik-corneliusson/click-web',
     author='Fredrik Corneliusson',
     author_email='fredrik.corneliusson@gmail.com',
     description=SHORT_DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     license='MIT',
     include_package_data=True,
```

### Comparing `click-web-0.8.0/tests/fixtures/script/a_script.py` & `click-web-0.8.1/tests/fixtures/script/a_script.py`

 * *Files identical despite different names*

### Comparing `click-web-0.8.0/tests/test_click_web.py` & `click-web-0.8.1/tests/test_click_web.py`

 * *Files identical despite different names*

### Comparing `click-web-0.8.0/tests/test_flask_get.py` & `click-web-0.8.1/tests/test_flask_get.py`

 * *Files identical despite different names*

### Comparing `click-web-0.8.0/tests/test_flask_post.py` & `click-web-0.8.1/tests/test_flask_post.py`

 * *Files identical despite different names*

### Comparing `click-web-0.8.0/tests/test_request_parsing.py` & `click-web-0.8.1/tests/test_request_parsing.py`

 * *Files identical despite different names*

