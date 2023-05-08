# Comparing `tmp/aeppl-nightly-0.1.3.dev20230506.tar.gz` & `tmp/aeppl-nightly-0.1.4.dev20230507.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aeppl-nightly-0.1.3.dev20230506.tar", last modified: Sat May  6 00:27:50 2023, max compression
+gzip compressed data, was "aeppl-nightly-0.1.4.dev20230507.tar", last modified: Sun May  7 00:31:42 2023, max compression
```

## Comparing `aeppl-nightly-0.1.3.dev20230506.tar` & `aeppl-nightly-0.1.4.dev20230507.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:27:50.927328 aeppl-nightly-0.1.3.dev20230506/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-06 00:27:38.000000 aeppl-nightly-0.1.3.dev20230506/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-06 00:27:38.000000 aeppl-nightly-0.1.3.dev20230506/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-06 00:27:50.927328 aeppl-nightly-0.1.3.dev20230506/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-05-06 00:27:38.000000 aeppl-nightly-0.1.3.dev20230506/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:27:50.927328 aeppl-nightly-0.1.3.dev20230506/aeppl/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-06 00:27:38.000000 aeppl-nightly-0.1.3.dev20230506/aeppl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-06 00:27:50.927328 aeppl-nightly-0.1.3.dev20230506/aeppl/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-05-06 00:27:38.000000 aeppl-nightly-0.1.3.dev20230506/aeppl/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     8455 2023-05-06 00:27:38.000000 aeppl-nightly-0.1.3.dev20230506/aeppl/censoring.py
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-05-06 00:27:38.000000 aeppl-nightly-0.1.3.dev20230506/aeppl/convolutions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-05-06 00:27:38.000000 aeppl-nightly-0.1.3.dev20230506/aeppl/cumsum.py
--rw-r--r--   0 runner    (1001) docker     (123)     8667 2023-05-06 00:27:38.000000 aeppl-nightly-0.1.3.dev20230506/aeppl/dists.py
--rw-r--r--   0 runner    (1001) docker     (123)    11572 2023-05-06 00:27:38.000000 aeppl-nightly-0.1.3.dev20230506/aeppl/joint_logprob.py
--rw-r--r--   0 runner    (1001) docker     (123)    21265 2023-05-06 00:27:38.000000 aeppl-nightly-0.1.3.dev20230506/aeppl/logprob.py
--rw-r--r--   0 runner    (1001) docker     (123)    15197 2023-05-06 00:27:38.000000 aeppl-nightly-0.1.3.dev20230506/aeppl/mixture.py
--rw-r--r--   0 runner    (1001) docker     (123)    24329 2023-05-06 00:27:38.000000 aeppl-nightly-0.1.3.dev20230506/aeppl/printing.py
--rw-r--r--   0 runner    (1001) docker     (123)    11398 2023-05-06 00:27:38.000000 aeppl-nightly-0.1.3.dev20230506/aeppl/rewriting.py
--rw-r--r--   0 runner    (1001) docker     (123)    21143 2023-05-06 00:27:38.000000 aeppl-nightly-0.1.3.dev20230506/aeppl/scan.py
--rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-05-06 00:27:38.000000 aeppl-nightly-0.1.3.dev20230506/aeppl/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)    30620 2023-05-06 00:27:38.000000 aeppl-nightly-0.1.3.dev20230506/aeppl/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     7859 2023-05-06 00:27:38.000000 aeppl-nightly-0.1.3.dev20230506/aeppl/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:27:50.923328 aeppl-nightly-0.1.3.dev20230506/aeppl_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-06 00:27:50.000000 aeppl-nightly-0.1.3.dev20230506/aeppl_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-06 00:27:50.000000 aeppl-nightly-0.1.3.dev20230506/aeppl_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 00:27:50.000000 aeppl-nightly-0.1.3.dev20230506/aeppl_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 00:27:50.000000 aeppl-nightly-0.1.3.dev20230506/aeppl_nightly.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-06 00:27:50.000000 aeppl-nightly-0.1.3.dev20230506/aeppl_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-06 00:27:50.000000 aeppl-nightly-0.1.3.dev20230506/aeppl_nightly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-06 00:27:50.927328 aeppl-nightly-0.1.3.dev20230506/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-06 00:27:38.000000 aeppl-nightly-0.1.3.dev20230506/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:27:50.927328 aeppl-nightly-0.1.3.dev20230506/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-05-06 00:27:38.000000 aeppl-nightly-0.1.3.dev20230506/tests/test_abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     5967 2023-05-06 00:27:38.000000 aeppl-nightly-0.1.3.dev20230506/tests/test_censoring.py
--rw-r--r--   0 runner    (1001) docker     (123)     5381 2023-05-06 00:27:38.000000 aeppl-nightly-0.1.3.dev20230506/tests/test_composite_logprob.py
--rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-05-06 00:27:38.000000 aeppl-nightly-0.1.3.dev20230506/tests/test_convolutions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-05-06 00:27:38.000000 aeppl-nightly-0.1.3.dev20230506/tests/test_cumsum.py
--rw-r--r--   0 runner    (1001) docker     (123)    25605 2023-05-06 00:27:38.000000 aeppl-nightly-0.1.3.dev20230506/tests/test_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     9218 2023-05-06 00:27:38.000000 aeppl-nightly-0.1.3.dev20230506/tests/test_joint_logprob.py
--rw-r--r--   0 runner    (1001) docker     (123)    40106 2023-05-06 00:27:38.000000 aeppl-nightly-0.1.3.dev20230506/tests/test_logprob.py
--rw-r--r--   0 runner    (1001) docker     (123)    22588 2023-05-06 00:27:38.000000 aeppl-nightly-0.1.3.dev20230506/tests/test_mixture.py
--rw-r--r--   0 runner    (1001) docker     (123)     6965 2023-05-06 00:27:38.000000 aeppl-nightly-0.1.3.dev20230506/tests/test_printing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-05-06 00:27:38.000000 aeppl-nightly-0.1.3.dev20230506/tests/test_rewriting.py
--rw-r--r--   0 runner    (1001) docker     (123)    11007 2023-05-06 00:27:38.000000 aeppl-nightly-0.1.3.dev20230506/tests/test_scan.py
--rw-r--r--   0 runner    (1001) docker     (123)     8499 2023-05-06 00:27:38.000000 aeppl-nightly-0.1.3.dev20230506/tests/test_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)    22973 2023-05-06 00:27:38.000000 aeppl-nightly-0.1.3.dev20230506/tests/test_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-05-06 00:27:38.000000 aeppl-nightly-0.1.3.dev20230506/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    70144 2023-05-06 00:27:38.000000 aeppl-nightly-0.1.3.dev20230506/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:31:42.976755 aeppl-nightly-0.1.4.dev20230507/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-07 00:31:29.000000 aeppl-nightly-0.1.4.dev20230507/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-07 00:31:29.000000 aeppl-nightly-0.1.4.dev20230507/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-07 00:31:42.976755 aeppl-nightly-0.1.4.dev20230507/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-05-07 00:31:29.000000 aeppl-nightly-0.1.4.dev20230507/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:31:42.976755 aeppl-nightly-0.1.4.dev20230507/aeppl/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-07 00:31:29.000000 aeppl-nightly-0.1.4.dev20230507/aeppl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-07 00:31:42.976755 aeppl-nightly-0.1.4.dev20230507/aeppl/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-05-07 00:31:29.000000 aeppl-nightly-0.1.4.dev20230507/aeppl/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8455 2023-05-07 00:31:29.000000 aeppl-nightly-0.1.4.dev20230507/aeppl/censoring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-05-07 00:31:29.000000 aeppl-nightly-0.1.4.dev20230507/aeppl/convolutions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-05-07 00:31:29.000000 aeppl-nightly-0.1.4.dev20230507/aeppl/cumsum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8667 2023-05-07 00:31:29.000000 aeppl-nightly-0.1.4.dev20230507/aeppl/dists.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-05-07 00:31:29.000000 aeppl-nightly-0.1.4.dev20230507/aeppl/joint_logprob.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21265 2023-05-07 00:31:29.000000 aeppl-nightly-0.1.4.dev20230507/aeppl/logprob.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15197 2023-05-07 00:31:29.000000 aeppl-nightly-0.1.4.dev20230507/aeppl/mixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24329 2023-05-07 00:31:29.000000 aeppl-nightly-0.1.4.dev20230507/aeppl/printing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11894 2023-05-07 00:31:29.000000 aeppl-nightly-0.1.4.dev20230507/aeppl/rewriting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21143 2023-05-07 00:31:29.000000 aeppl-nightly-0.1.4.dev20230507/aeppl/scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-05-07 00:31:29.000000 aeppl-nightly-0.1.4.dev20230507/aeppl/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30605 2023-05-07 00:31:29.000000 aeppl-nightly-0.1.4.dev20230507/aeppl/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7859 2023-05-07 00:31:29.000000 aeppl-nightly-0.1.4.dev20230507/aeppl/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:31:42.976755 aeppl-nightly-0.1.4.dev20230507/aeppl_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-07 00:31:42.000000 aeppl-nightly-0.1.4.dev20230507/aeppl_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-07 00:31:42.000000 aeppl-nightly-0.1.4.dev20230507/aeppl_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 00:31:42.000000 aeppl-nightly-0.1.4.dev20230507/aeppl_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 00:31:42.000000 aeppl-nightly-0.1.4.dev20230507/aeppl_nightly.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-07 00:31:42.000000 aeppl-nightly-0.1.4.dev20230507/aeppl_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-07 00:31:42.000000 aeppl-nightly-0.1.4.dev20230507/aeppl_nightly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-07 00:31:42.976755 aeppl-nightly-0.1.4.dev20230507/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-07 00:31:29.000000 aeppl-nightly-0.1.4.dev20230507/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:31:42.976755 aeppl-nightly-0.1.4.dev20230507/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-05-07 00:31:29.000000 aeppl-nightly-0.1.4.dev20230507/tests/test_abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5967 2023-05-07 00:31:29.000000 aeppl-nightly-0.1.4.dev20230507/tests/test_censoring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-05-07 00:31:29.000000 aeppl-nightly-0.1.4.dev20230507/tests/test_composite_logprob.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-05-07 00:31:29.000000 aeppl-nightly-0.1.4.dev20230507/tests/test_convolutions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-05-07 00:31:29.000000 aeppl-nightly-0.1.4.dev20230507/tests/test_cumsum.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25605 2023-05-07 00:31:29.000000 aeppl-nightly-0.1.4.dev20230507/tests/test_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9218 2023-05-07 00:31:29.000000 aeppl-nightly-0.1.4.dev20230507/tests/test_joint_logprob.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40106 2023-05-07 00:31:29.000000 aeppl-nightly-0.1.4.dev20230507/tests/test_logprob.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22582 2023-05-07 00:31:29.000000 aeppl-nightly-0.1.4.dev20230507/tests/test_mixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6965 2023-05-07 00:31:29.000000 aeppl-nightly-0.1.4.dev20230507/tests/test_printing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-05-07 00:31:29.000000 aeppl-nightly-0.1.4.dev20230507/tests/test_rewriting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11007 2023-05-07 00:31:29.000000 aeppl-nightly-0.1.4.dev20230507/tests/test_scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8499 2023-05-07 00:31:29.000000 aeppl-nightly-0.1.4.dev20230507/tests/test_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22973 2023-05-07 00:31:29.000000 aeppl-nightly-0.1.4.dev20230507/tests/test_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-05-07 00:31:29.000000 aeppl-nightly-0.1.4.dev20230507/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70144 2023-05-07 00:31:29.000000 aeppl-nightly-0.1.4.dev20230507/versioneer.py
```

### Comparing `aeppl-nightly-0.1.3.dev20230506/LICENSE` & `aeppl-nightly-0.1.4.dev20230507/LICENSE`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230506/PKG-INFO` & `aeppl-nightly-0.1.4.dev20230507/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aeppl-nightly
-Version: 0.1.3.dev20230506
+Version: 0.1.4.dev20230507
 Summary: PPL tools for Aesara
 Home-page: https://github.com/aesara-devs/aeppl
 Author: aesara-devs
 Author-email: aesara.devs@gmail.com
 Keywords: aeppl,math,probability,symbolic,probabilistic programming
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `aeppl-nightly-0.1.3.dev20230506/README.md` & `aeppl-nightly-0.1.4.dev20230507/README.md`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230506/aeppl/abstract.py` & `aeppl-nightly-0.1.4.dev20230507/aeppl/abstract.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230506/aeppl/censoring.py` & `aeppl-nightly-0.1.4.dev20230507/aeppl/censoring.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230506/aeppl/convolutions.py` & `aeppl-nightly-0.1.4.dev20230507/aeppl/convolutions.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230506/aeppl/cumsum.py` & `aeppl-nightly-0.1.4.dev20230507/aeppl/cumsum.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230506/aeppl/dists.py` & `aeppl-nightly-0.1.4.dev20230507/aeppl/dists.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230506/aeppl/joint_logprob.py` & `aeppl-nightly-0.1.4.dev20230507/aeppl/joint_logprob.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,43 +137,37 @@
         original_rv_values[rv] = vv
 
     # Value variables are not cloned when constructing the conditional log-probability
     # graphs. We can thus use them to recover the original random variables to index the
     # maps to the logprob graphs and value variables before returning them.
     rv_values = {**original_rv_values, **realized}
 
-    fgraph, _, memo = construct_ir_fgraph(rv_values, ir_rewriter=ir_rewriter)
-
-    if extra_rewrites is not None:
-        extra_rewrites.add_requirements(fgraph, rv_values, memo)
-        extra_rewrites.apply(fgraph)
+    fgraph, new_rv_values = construct_ir_fgraph(
+        rv_values, ir_rewriter=ir_rewriter, extra_rewrites=extra_rewrites
+    )
 
     # We assign log-densities on a per-node basis, and not per-output/variable.
     realized_vars = set()
     new_to_old_rvs = {}
     nodes_to_vals: Dict["Apply", List[Tuple["Variable", "Variable"]]] = {}
 
-    for bnd_var, (old_mvar, old_val) in zip(fgraph.outputs, rv_values.items()):
+    for bnd_var, (old_mvar, val) in zip(fgraph.outputs, new_rv_values.items()):
         mnode = bnd_var.owner
         assert mnode and isinstance(mnode.op, ValuedVariable)
 
         rv_var, val_var = mnode.inputs
         rv_node = rv_var.owner
 
         if rv_node is None:
             raise DensityNotFound(f"Couldn't derive a log-probability for {rv_var}")
 
         if old_mvar in realized:
             realized_vars.add(rv_var)
 
-        # Do this just in case a value variable was changed.  (Some transforms
-        # do this.)
-        new_val = memo[old_val]
-
-        nodes_to_vals.setdefault(rv_node, []).append((val_var, new_val))
+        nodes_to_vals.setdefault(rv_node, []).append((val_var, val))
 
         new_to_old_rvs[rv_var] = old_mvar
 
     value_vars: Tuple["Variable", ...] = ()
     logprob_vars = {}
 
     for rv_node, rv_val_pairs in nodes_to_vals.items():
```

### Comparing `aeppl-nightly-0.1.3.dev20230506/aeppl/logprob.py` & `aeppl-nightly-0.1.4.dev20230507/aeppl/logprob.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230506/aeppl/mixture.py` & `aeppl-nightly-0.1.4.dev20230507/aeppl/mixture.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230506/aeppl/printing.py` & `aeppl-nightly-0.1.4.dev20230507/aeppl/printing.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230506/aeppl/rewriting.py` & `aeppl-nightly-0.1.4.dev20230507/aeppl/rewriting.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,20 @@
-from typing import Dict, Optional, Tuple
+from typing import Dict, Optional, Tuple, Union
 
 import aesara.tensor as at
 from aesara.compile.mode import optdb
 from aesara.graph.basic import Apply, Variable
 from aesara.graph.features import Feature
 from aesara.graph.fg import FunctionGraph
-from aesara.graph.rewriting.basic import GraphRewriter, in2out, node_rewriter
+from aesara.graph.rewriting.basic import (
+    GraphRewriter,
+    NodeRewriter,
+    in2out,
+    node_rewriter,
+)
 from aesara.graph.rewriting.db import EquilibriumDB, RewriteDatabaseQuery, SequenceDB
 from aesara.tensor.elemwise import DimShuffle, Elemwise
 from aesara.tensor.extra_ops import BroadcastTo
 from aesara.tensor.random.rewriting import local_subtensor_rv_lift
 from aesara.tensor.rewriting.basic import register_canonicalize, register_useless
 from aesara.tensor.rewriting.shape import ShapeFeature
 from aesara.tensor.subtensor import (
@@ -176,17 +181,18 @@
     "incsubtensor_lift", incsubtensor_rv_replace, "basic"
 )
 
 logprob_rewrites_db.register("post-canonicalize", optdb.query("+canonicalize"), "basic")
 
 
 def construct_ir_fgraph(
-    rv_values: Dict[Variable, Variable],
+    rvs_to_values: Dict[Variable, Variable],
     ir_rewriter: Optional[GraphRewriter] = None,
-) -> Tuple[FunctionGraph, Dict[Variable, Variable], Dict[Variable, Variable]]:
+    extra_rewrites: Optional[Union[GraphRewriter, NodeRewriter]] = None,
+) -> Tuple[FunctionGraph, Dict[Variable, Variable]]:
     r"""Construct a `FunctionGraph` in measurable IR form for the keys in `rv_values`.
 
     A custom IR rewriter can be specified. By default,
     ``logprob_rewrites_db.query(RewriteDatabaseQuery(include=["basic"]))`` is used.
 
     Our measurable IR takes the form of an Aesara graph that is more-or-less
     equivalent to a given Aesara graph (i.e. the keys of `rv_values`) but
@@ -211,17 +217,16 @@
     this IR, and the resulting graphs will not be computationally sound,
     because they wouldn't produce independent samples when the original graph
     would.  See https://github.com/aesara-devs/aeppl/pull/78.
 
     Returns
     -------
     A `FunctionGraph` of the measurable IR, a copy of `rv_values` containing
-    the new, cloned versions of the original variables in `rv_values`, and
-    a ``dict`` mapping all the original variables to their cloned values in
-    the `FunctionGraph`.
+    the new, cloned versions of the original variables in `rv_values`.
+
     """
 
     # We're going to create a `FunctionGraph` that effectively represents the
     # joint log-probability of all the random variables assigned values in
     # `rv_values`.
     # The `FunctionGraph`'s outputs will be `ValuedVariable`s.  This serves to
     # associate a random variable with its value and facilitate
@@ -229,58 +234,70 @@
     # The `FunctionGraph` will be transformed by rewrites so that
     # log-probabilities can be assigned to/derived for its outputs.
 
     # We clone the random variables that we'll use as `FunctionGraph` outputs
     # so that they're distinct nodes in the graph.  This allows us to replace
     # all instances of the original random variables with their value
     # variables, while leaving the output clones untouched.
-    rv_value_clones = {}
+    rv_clone_to_value_clone = {}
+    rv_to_value_clone = {}
+    value_clone_to_value = {}
     measured_outputs = {}
-    memo = {}
-    for rv, val in rv_values.items():
+    memo: Dict[Variable, Variable] = {}
+    for rv, val in rvs_to_values.items():
         rv_node_clone = rv.owner.clone()
         rv_clone = rv_node_clone.outputs[rv.owner.outputs.index(rv)]
-        rv_value_clones[rv_clone] = val
-        measured_outputs[rv] = valued_variable(rv_clone, val)
-        # Prevent value variables from being cloned
-        memo[val] = val
+        val_clone = val.clone()
+        val_clone.name = "val_clone"
+        rv_clone_to_value_clone[rv_clone] = val_clone
+        rv_to_value_clone[rv] = val_clone
+        value_clone_to_value[val_clone] = val
+        measured_outputs[rv] = valued_variable(rv_clone, val_clone)
 
     # We add `ShapeFeature` because it will get rid of references to the old
     # `RandomVariable`s that have been lifted; otherwise, it will be difficult
     # to give good warnings when an unaccounted for `RandomVariable` is
     # encountered
     fgraph = FunctionGraph(
         outputs=tuple(measured_outputs.values()),
         features=[ShapeFeature(), MeasurableConversionTracker()],
         clone=True,
         memo=memo,
         copy_orphans=False,
         copy_inputs=False,
     )
 
-    # Update `rv_values` so that it uses the new cloned variables
-    rv_value_clones = {memo[k]: v for k, v in rv_value_clones.items()}
-
     # Replace valued non-output variables with their values
     fgraph.replace_all(
         [(memo[rv], val) for rv, val in measured_outputs.items() if rv in memo],
         reason="valued-non-outputs-replace",
         import_missing=True,
     )
 
     if ir_rewriter is None:
         ir_rewriter = logprob_rewrites_db.query(RewriteDatabaseQuery(include=["basic"]))
 
     ir_rewriter.rewrite(fgraph)
 
+    if extra_rewrites is not None:
+        # Expect `value_clone_to_value` to be updated in-place
+        extra_rewrites.add_requirements(fgraph, rv_to_value_clone, value_clone_to_value)
+        extra_rewrites.apply(fgraph)
+
     # Undo un-valued measurable IR rewrites
     new_to_old = tuple((v, k) for k, v in fgraph.measurable_conversions.items())
-    fgraph.replace_all(new_to_old, reason="undo-unvalued-measurables")
+    # and add the original value variables back in
+    new_to_old += tuple(value_clone_to_value.items())
+    fgraph.replace_all(
+        new_to_old, reason="undo-unvalued-measurables", import_missing=True
+    )
+
+    new_rvs_to_values = dict(zip(rvs_to_values.keys(), value_clone_to_value.values()))
 
-    return fgraph, rv_value_clones, memo
+    return fgraph, new_rvs_to_values
 
 
 @register_useless
 @node_rewriter([ValuedVariable])
 def remove_ValuedVariable(fgraph, node):
     return [node.inputs[1]]
```

### Comparing `aeppl-nightly-0.1.3.dev20230506/aeppl/scan.py` & `aeppl-nightly-0.1.4.dev20230507/aeppl/scan.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230506/aeppl/tensor.py` & `aeppl-nightly-0.1.4.dev20230507/aeppl/tensor.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230506/aeppl/transforms.py` & `aeppl-nightly-0.1.4.dev20230507/aeppl/transforms.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,22 +157,18 @@
     "backward"-transform of a new value variable in the "forward"-transformed
     space.
     3. Signify that the original value variable is to be replaced by the new
     one.
     4. Replace the old `ValuedVariable` with a new one containing a
     `TransformedVariable` value.
 
-    Step 3. is currently accomplished by updating the `memo` dictionary
-    associated with the `FunctionGraph`.  Our main entry-point,
+    Step 3. is currently accomplished by updating the `rvs_to_values`
+    dictionary associated with the `FunctionGraph`.  Our main entry-point,
     `conditional_logprob`, checks this dictionary for value variable changes.
 
-    TODO: This approach is less than ideal, because it puts awkward demands on
-    users/callers of this rewrite to check with `memo`; let's see if we can do
-    something better.
-
     The new value variable mentioned in Step 2. may be of a different `Type`
     (e.g. extra/fewer dimensions) than the original value variable; this is why
     we must replace the corresponding original value variables before we
     construct log-probability graphs.  This is due to the fact that we
     generally cannot replace variables with new ones that have different
     `Type`\s.
 
@@ -231,16 +227,16 @@
     # with "inversely/un-" transformed versions of themselves.
     untrans_value_var = transformed_variable(
         transform.backward(trans_value_var, *trans_node.inputs), trans_value_var
     )
 
     # This effectively lets the caller know that a value variable has been
     # replaced (i.e. they should filter all their old value variables through
-    # the memo/replacements map).
-    fgraph.memo[value_var] = trans_value_var
+    # the replacements map).
+    fgraph.value_clone_to_value[value_var] = trans_value_var
 
     trans_var = trans_node.outputs[rv_var_out_idx]
     new_var = valued_variable(trans_var, untrans_value_var)
 
     return {value_var: untrans_value_var, node.outputs[0]: new_var}
 
 
@@ -248,37 +244,36 @@
     r"""A `Feature` that maintains a map between value variables and their transforms as
     well as between value variables and their transformed counterparts.
 
     This is exclusively/primarily used by `TransformValuesRewrite`.
 
     """
 
-    def __init__(self, values_to_transforms, memo):
+    def __init__(self, values_to_transforms, value_clone_to_value):
         """
         Parameters
         ==========
         values_to_transforms
             Mapping between value variables and their transformations. Each
             value variable can be assigned one of `RVTransform`,
             `DEFAULT_TRANSFORM`, or ``None``. Random variables with no
             transform specified remain unchanged.
-        memo
-            Mapping from variables to their clones.  This is updated
-            in-place whenever a value variable is transformed.
-
+        value_clone_to_value
+            Mapping between random variable value clones and their original
+            value variables.
         """
         self.values_to_transforms = values_to_transforms
-        self.memo = memo
+        self.value_clone_to_value = value_clone_to_value
 
     def on_attach(self, fgraph):
         if hasattr(fgraph, "values_to_transforms"):
             raise AlreadyThere()
 
         fgraph.values_to_transforms = self.values_to_transforms
-        fgraph.memo = self.memo
+        fgraph.value_clone_to_value = self.value_clone_to_value
 
 
 class TransformValuesRewrite(GraphRewriter):
     r"""Transforms measurable variables.
 
     This transformation can be used to replace all occurrences of a measurable
     variable and its values within a model graph with a transformed version of
@@ -318,30 +313,33 @@
         Parameters
         ==========
         rvs_to_transforms
             Mapping between measurable variables and their transformations. Each
             measurable variable can be assigned an `RVTransform` instance,
             `DEFAULT_TRANSFORM`, or ``None``. Measurable variables with no
             transform specified remain unchanged.
+        rvs_to_values
 
         """
 
         self.rvs_to_transforms = rvs_to_transforms
 
     def add_requirements(
         self,
         fgraph,
-        rv_to_values: Dict[TensorVariable, TensorVariable],
-        memo: Dict[TensorVariable, TensorVariable],
+        rvs_to_values: Dict[TensorVariable, TensorVariable],
+        value_clone_to_value: Dict[TensorVariable, TensorVariable],
     ):
         values_to_transforms = {
-            rv_to_values[rv]: transform
+            rvs_to_values[rv]: transform
             for rv, transform in self.rvs_to_transforms.items()
         }
-        values_transforms_feature = TransformValuesMapping(values_to_transforms, memo)
+        values_transforms_feature = TransformValuesMapping(
+            values_to_transforms, value_clone_to_value
+        )
         fgraph.attach_feature(values_transforms_feature)
 
     def apply(self, fgraph: FunctionGraph):
         return self.default_transform_rewrite.rewrite(fgraph)
 
 
 class MeasurableElemwiseTransform(MeasurableElemwise):
```

### Comparing `aeppl-nightly-0.1.3.dev20230506/aeppl/utils.py` & `aeppl-nightly-0.1.4.dev20230507/aeppl/utils.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230506/aeppl_nightly.egg-info/PKG-INFO` & `aeppl-nightly-0.1.4.dev20230507/aeppl_nightly.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aeppl-nightly
-Version: 0.1.3.dev20230506
+Version: 0.1.4.dev20230507
 Summary: PPL tools for Aesara
 Home-page: https://github.com/aesara-devs/aeppl
 Author: aesara-devs
 Author-email: aesara.devs@gmail.com
 Keywords: aeppl,math,probability,symbolic,probabilistic programming
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `aeppl-nightly-0.1.3.dev20230506/aeppl_nightly.egg-info/SOURCES.txt` & `aeppl-nightly-0.1.4.dev20230507/aeppl_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230506/setup.cfg` & `aeppl-nightly-0.1.4.dev20230507/setup.cfg`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230506/setup.py` & `aeppl-nightly-0.1.4.dev20230507/setup.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230506/tests/test_abstract.py` & `aeppl-nightly-0.1.4.dev20230507/tests/test_abstract.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230506/tests/test_censoring.py` & `aeppl-nightly-0.1.4.dev20230507/tests/test_censoring.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230506/tests/test_composite_logprob.py` & `aeppl-nightly-0.1.4.dev20230507/tests/test_composite_logprob.py`

 * *Files 16% similar despite different names*

```diff
@@ -75,33 +75,28 @@
     assert np.isclose(logp_fn(0, 0, 1, 50), st.norm.logpdf(150) + np.log(0.5) * 3)
 
 
 def test_unvalued_ir_reversion():
     """Make sure that un-valued IR rewrites are reverted."""
     srng = at.random.RandomStream(0)
 
-    x_rv = srng.normal()
+    x_rv = srng.normal(name="X")
     y_rv = at.clip(x_rv, 0, 1)
-    z_rv = srng.normal(y_rv, 1, name="z")
+    y_rv.name = "Y"
+    z_rv = srng.normal(y_rv, 1, name="Z")
     z_vv = z_rv.clone()
+    z_vv.name = "z"
 
     # Only the `z_rv` is "valued", so `y_rv` doesn't need to be converted into
     # measurable IR.
     rv_values = {z_rv: z_vv}
 
-    z_fgraph, _, memo = construct_ir_fgraph(rv_values)
+    z_fgraph, new_rvs_to_values = construct_ir_fgraph(rv_values)
 
-    assert memo[y_rv] in z_fgraph.measurable_conversions
-
-    measurable_y_rv = z_fgraph.measurable_conversions[memo[y_rv]]
-    assert isinstance(measurable_y_rv.owner.op, MeasurableClip)
-
-    # `construct_ir_fgraph` should've reverted the un-valued measurable IR
-    # change
-    assert measurable_y_rv not in z_fgraph
+    assert not any(isinstance(node.op, MeasurableClip) for node in z_fgraph.apply_nodes)
 
 
 def test_shifted_cumsum():
     srng = at.random.RandomStream(0)
 
     x = srng.normal(size=(5,), name="x")
     y = 5 + at.cumsum(x)
```

### Comparing `aeppl-nightly-0.1.3.dev20230506/tests/test_convolutions.py` & `aeppl-nightly-0.1.4.dev20230507/tests/test_convolutions.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
     Y_rv = srng.normal(mu_y, sigma_y, size=y_shape)
     Y_rv.name = "Y"
 
     Z_rv = X_rv + Y_rv if not sub else X_rv - Y_rv
     Z_rv.name = "Z"
     z_vv = Z_rv.clone()
 
-    fgraph, _, _ = construct_ir_fgraph({Z_rv: z_vv})
+    fgraph, *_ = construct_ir_fgraph({Z_rv: z_vv})
 
     (valued_var_out_node) = fgraph.outputs[0].owner
     # The convolution should be applied, and not the transform
     assert isinstance(valued_var_out_node.inputs[0].owner.op, NormalRV)
 
     new_rv = fgraph.outputs[0].owner.inputs[0]
 
@@ -104,15 +104,15 @@
     X_rv = srng.normal(1.0, name="X")
     x_vv = X_rv.clone()
     Y_rv = srng.normal(1.0, name="Y")
     Z_rv = X_rv + Y_rv
     Z_rv.name = "Z"
     z_vv = Z_rv.clone()
 
-    fgraph, _, _ = construct_ir_fgraph({Z_rv: z_vv, X_rv: x_vv})
+    fgraph, *_ = construct_ir_fgraph({Z_rv: z_vv, X_rv: x_vv})
 
     valued_var_out_node = fgraph.outputs[0].owner
     # We should not expect the convolution to be applied; instead, the
     # transform should be (for now)
     assert isinstance(
         valued_var_out_node.inputs[0].owner.op, MeasurableElemwiseTransform
     )
@@ -132,12 +132,12 @@
     sigma_w = at.vector("sigma_w")
     W_rv = srng.normal(mu_w, sigma_w, name="W")
 
     Z_rv = X_rv + Y_rv + W_rv
     Z_rv.name = "Z"
     z_vv = Z_rv.clone()
 
-    fgraph, _, _ = construct_ir_fgraph({Z_rv: z_vv})
+    fgraph, *_ = construct_ir_fgraph({Z_rv: z_vv})
 
     valued_var_out_node = fgraph.outputs[0].owner
     # The convolution should be applied, and not the transform
     assert isinstance(valued_var_out_node.inputs[0].owner.op, NormalRV)
```

### Comparing `aeppl-nightly-0.1.3.dev20230506/tests/test_cumsum.py` & `aeppl-nightly-0.1.4.dev20230507/tests/test_cumsum.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230506/tests/test_dist.py` & `aeppl-nightly-0.1.4.dev20230507/tests/test_dist.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230506/tests/test_joint_logprob.py` & `aeppl-nightly-0.1.4.dev20230507/tests/test_joint_logprob.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230506/tests/test_logprob.py` & `aeppl-nightly-0.1.4.dev20230507/tests/test_logprob.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230506/tests/test_mixture.py` & `aeppl-nightly-0.1.4.dev20230507/tests/test_mixture.py`

 * *Files 0% similar despite different names*

```diff
@@ -681,35 +681,35 @@
     i_vv = I_rv.clone()
     i_vv.name = "i"
 
     Z1_rv = at.switch(I_rv, X_rv, Y_rv)
     z_vv = Z1_rv.clone()
     z_vv.name = "z1"
 
-    fgraph, _, _ = construct_ir_fgraph({Z1_rv: z_vv, I_rv: i_vv})
+    fgraph, *_ = construct_ir_fgraph({Z1_rv: z_vv, I_rv: i_vv})
 
     out_rv = fgraph.outputs[0].owner.inputs[0]
     assert isinstance(out_rv.owner.op, MixtureRV)
     assert not hasattr(
         fgraph.outputs[0].tag, "test_value"
     )  # aesara.config.compute_test_value == "off"
     assert fgraph.outputs[0].name is None
 
     Z1_rv.name = "Z1"
 
-    fgraph, _, _ = construct_ir_fgraph({Z1_rv: z_vv, I_rv: i_vv})
+    fgraph, *_ = construct_ir_fgraph({Z1_rv: z_vv, I_rv: i_vv})
 
     out_rv = fgraph.outputs[0].owner.inputs[0]
     assert out_rv.name == "Z1-mixture"
 
     # building the identical graph but with a stack to check that mixture computations are identical
 
     Z2_rv = at.stack((X_rv, Y_rv))[I_rv]
 
-    fgraph2, _, _ = construct_ir_fgraph({Z2_rv: z_vv, I_rv: i_vv})
+    fgraph2, *_ = construct_ir_fgraph({Z2_rv: z_vv, I_rv: i_vv})
 
     assert equal_computations(fgraph.outputs, fgraph2.outputs)
 
     z1_logp, _ = joint_logprob(realized={Z1_rv: z_vv, I_rv: i_vv})
     z2_logp, _ = joint_logprob(realized={Z2_rv: z_vv, I_rv: i_vv})
 
     # below should follow immediately from the equal_computations assertion above
```

### Comparing `aeppl-nightly-0.1.3.dev20230506/tests/test_printing.py` & `aeppl-nightly-0.1.4.dev20230507/tests/test_printing.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230506/tests/test_rewriting.py` & `aeppl-nightly-0.1.4.dev20230507/tests/test_rewriting.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230506/tests/test_scan.py` & `aeppl-nightly-0.1.4.dev20230507/tests/test_scan.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230506/tests/test_tensor.py` & `aeppl-nightly-0.1.4.dev20230507/tests/test_tensor.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230506/tests/test_transforms.py` & `aeppl-nightly-0.1.4.dev20230507/tests/test_transforms.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230506/tests/test_utils.py` & `aeppl-nightly-0.1.4.dev20230507/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.3.dev20230506/versioneer.py` & `aeppl-nightly-0.1.4.dev20230507/versioneer.py`

 * *Files identical despite different names*

