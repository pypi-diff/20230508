# Comparing `tmp/lightning_toolbox-0.0.8.tar.gz` & `tmp/lightning_toolbox-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightning_toolbox-0.0.8.tar", last modified: Mon Jan  2 21:44:10 2023, max compression
+gzip compressed data, was "lightning_toolbox-0.0.9.tar", last modified: Mon Jan 16 17:11:19 2023, max compression
```

## Comparing `lightning_toolbox-0.0.8.tar` & `lightning_toolbox-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 21:44:10.633825 lightning_toolbox-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-01-02 21:44:02.000000 lightning_toolbox-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-01-02 21:44:10.633825 lightning_toolbox-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-01-02 21:44:02.000000 lightning_toolbox-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 21:44:10.633825 lightning_toolbox-0.0.8/lightning_toolbox/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-01-02 21:44:02.000000 lightning_toolbox-0.0.8/lightning_toolbox/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 21:44:10.633825 lightning_toolbox-0.0.8/lightning_toolbox/training/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-01-02 21:44:02.000000 lightning_toolbox-0.0.8/lightning_toolbox/training/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6553 2023-01-02 21:44:02.000000 lightning_toolbox-0.0.8/lightning_toolbox/training/criterion.py
--rw-r--r--   0 runner    (1001) docker     (123)    19484 2023-01-02 21:44:02.000000 lightning_toolbox-0.0.8/lightning_toolbox/training/module.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-01-02 21:44:02.000000 lightning_toolbox-0.0.8/lightning_toolbox/training/struct_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    13105 2023-01-02 21:44:02.000000 lightning_toolbox-0.0.8/lightning_toolbox/training/terms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-01-02 21:44:02.000000 lightning_toolbox-0.0.8/lightning_toolbox/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 21:44:10.633825 lightning_toolbox-0.0.8/lightning_toolbox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-01-02 21:44:10.000000 lightning_toolbox-0.0.8/lightning_toolbox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-01-02 21:44:10.000000 lightning_toolbox-0.0.8/lightning_toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-02 21:44:10.000000 lightning_toolbox-0.0.8/lightning_toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-01-02 21:44:10.000000 lightning_toolbox-0.0.8/lightning_toolbox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-01-02 21:44:10.000000 lightning_toolbox-0.0.8/lightning_toolbox.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-02 21:44:10.633825 lightning_toolbox-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-01-02 21:44:02.000000 lightning_toolbox-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 17:11:19.577727 lightning_toolbox-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-01-16 17:11:10.000000 lightning_toolbox-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-01-16 17:11:19.577727 lightning_toolbox-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-01-16 17:11:10.000000 lightning_toolbox-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 17:11:19.577727 lightning_toolbox-0.0.9/lightning_toolbox/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-01-16 17:11:10.000000 lightning_toolbox-0.0.9/lightning_toolbox/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 17:11:19.577727 lightning_toolbox-0.0.9/lightning_toolbox/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-01-16 17:11:10.000000 lightning_toolbox-0.0.9/lightning_toolbox/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6992 2023-01-16 17:11:10.000000 lightning_toolbox-0.0.9/lightning_toolbox/data/module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 17:11:19.577727 lightning_toolbox-0.0.9/lightning_toolbox/training/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-01-16 17:11:10.000000 lightning_toolbox-0.0.9/lightning_toolbox/training/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6553 2023-01-16 17:11:10.000000 lightning_toolbox-0.0.9/lightning_toolbox/training/criterion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19482 2023-01-16 17:11:10.000000 lightning_toolbox-0.0.9/lightning_toolbox/training/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-01-16 17:11:10.000000 lightning_toolbox-0.0.9/lightning_toolbox/training/struct_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13097 2023-01-16 17:11:10.000000 lightning_toolbox-0.0.9/lightning_toolbox/training/terms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-01-16 17:11:10.000000 lightning_toolbox-0.0.9/lightning_toolbox/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 17:11:19.577727 lightning_toolbox-0.0.9/lightning_toolbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-01-16 17:11:19.000000 lightning_toolbox-0.0.9/lightning_toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-01-16 17:11:19.000000 lightning_toolbox-0.0.9/lightning_toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-16 17:11:19.000000 lightning_toolbox-0.0.9/lightning_toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-01-16 17:11:19.000000 lightning_toolbox-0.0.9/lightning_toolbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-01-16 17:11:19.000000 lightning_toolbox-0.0.9/lightning_toolbox.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-16 17:11:19.577727 lightning_toolbox-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-01-16 17:11:10.000000 lightning_toolbox-0.0.9/setup.py
```

### Comparing `lightning_toolbox-0.0.8/LICENSE` & `lightning_toolbox-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `lightning_toolbox-0.0.8/PKG-INFO` & `lightning_toolbox-0.0.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightning_toolbox
-Version: 0.0.8
+Version: 0.0.9
 Summary: A collection of utilities for PyTorch Lightning.
 Home-page: https://github.com/vahidzee/lightning_toolbox
 Author: Vahid Zehtab
 Author-email: vahid@zehtab.me
 License: MIT
 Description: # Lightning Toolbox: A set of useful tools for the PyTorch Lightning Framework
```

### Comparing `lightning_toolbox-0.0.8/lightning_toolbox/training/criterion.py` & `lightning_toolbox-0.0.9/lightning_toolbox/training/criterion.py`

 * *Files identical despite different names*

### Comparing `lightning_toolbox-0.0.8/lightning_toolbox/training/module.py` & `lightning_toolbox-0.0.9/lightning_toolbox/training/module.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import torch
 import typing as th
 import functools
 import lightning
 from ..utils import freeze_params, unfreeze_params, list_args
-import dycode as dy
+import dypy as dy
 from .criterion import Criterion
 import torch
 import types
 
 
 class TrainingModule(lightning.LightningModule):
     """
```

### Comparing `lightning_toolbox-0.0.8/lightning_toolbox/training/terms.py` & `lightning_toolbox-0.0.9/lightning_toolbox/training/terms.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import torch
 import functools
 import lightning
-import dycode as dy
+import dypy as dy
 import typing as th
 from .struct_types import ResultsDict, FactorsDict, TermDescriptor
 
 
 class CriterionTerm:
     def __init__(
         self,
@@ -51,15 +51,15 @@
                     >>> scale_factor = "term/mse"
                     This will scale the factor by the ratio of the term value to the MSE term value. Which is:
                         factor = factor * mse_term_value.detach() / term_value.detach()
 
                 If you
             term_function (FunctionDescriptor): Function that computes the term value. This can be a function that takes
                 the training_module, batch, [results_dict], and any other argument and returns a torch.Tensor.
-                This function will be processed using `dycode.eval`. See `dycode.eval` documentation for more details.
+                This function will be processed using `dypy.eval`. See `dypy.eval` documentation for more details.
 
             factor_application (str): How the factor is applied to the term value. Can be "multiply" or "add".
 
         """
         self.name = name or self.__class__.__name__
         self._factor_application = factor_application
         self._factor_description = factor
@@ -168,15 +168,15 @@
             raise ValueError(f"Unknown factor application {self._factor_application}")
 
     @functools.cached_property
     def _compiled_term_function(self):
         """
         Compiled version of the term function provided to the constructor in the `term_function` argument.
 
-        The function descriptor is processed using `dycode.eval` and the result is cached using `functools.cached_property`.
+        The function descriptor is processed using `dypy.eval` and the result is cached using `functools.cached_property`.
         By setting dynamic_args=True when evaluating the function, the function will be wrapped in a `dynamic_args_wrapper`
         that will allow it to be called with any arguments.
         """
         return dy.eval(self._term_function_description, function_of_interest="term", strict=False, dynamic_args=True)
 
     def __call__(
         self, *args, batch: th.Any = None, training_module: lightning.LightningModule = None, **kwargs
```

### Comparing `lightning_toolbox-0.0.8/lightning_toolbox/utils.py` & `lightning_toolbox-0.0.9/lightning_toolbox/utils.py`

 * *Files identical despite different names*

### Comparing `lightning_toolbox-0.0.8/lightning_toolbox.egg-info/PKG-INFO` & `lightning_toolbox-0.0.9/lightning_toolbox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightning-toolbox
-Version: 0.0.8
+Version: 0.0.9
 Summary: A collection of utilities for PyTorch Lightning.
 Home-page: https://github.com/vahidzee/lightning_toolbox
 Author: Vahid Zehtab
 Author-email: vahid@zehtab.me
 License: MIT
 Description: # Lightning Toolbox: A set of useful tools for the PyTorch Lightning Framework
```

### Comparing `lightning_toolbox-0.0.8/setup.py` & `lightning_toolbox-0.0.9/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 
 with open("README.md", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="lightning_toolbox",
     packages=find_packages(include=["lightning_toolbox", "lightning_toolbox.*"]),
-    version="0.0.8",
+    version="0.0.9",
     license="MIT",
     description="A collection of utilities for PyTorch Lightning.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Vahid Zehtab",
     author_email="vahid@zehtab.me",
     url="https://github.com/vahidzee/lightning_toolbox",
     keywords=["artificial intelligence", "pytorch lightning", "objective functions", "regularization"],
-    install_requires=["torch>=1.9", "lightning", "dycode"],
+    install_requires=["torch>=1.9", "lightning", "dypy"],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.8",
     ],
```

