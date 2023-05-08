# Comparing `tmp/analogvnn-1.0.2.tar.gz` & `tmp/analogvnn-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "analogvnn-1.0.2.tar", last modified: Mon May  8 03:06:23 2023, max compression
+gzip compressed data, was "analogvnn-1.0.3.tar", last modified: Mon May  8 04:25:03 2023, max compression
```

## Comparing `analogvnn-1.0.2.tar` & `analogvnn-1.0.3.tar`

### file list

```diff
@@ -1,67 +1,67 @@
--rw-r--r--   0        0        0    17182 2023-01-25 01:41:18.328863 analogvnn-1.0.2/LICENSE
--rw-r--r--   0        0        0     2823 2023-05-08 03:05:49.632025 analogvnn-1.0.2/README.md
--rw-r--r--   0        0        0      728 2023-03-07 11:00:42.959136 analogvnn-1.0.2/analogvnn/__init__.py
--rw-r--r--   0        0        0     2873 2023-03-21 17:16:13.013355 analogvnn-1.0.2/analogvnn/backward/BackwardFunction.py
--rw-r--r--   0        0        0      930 2023-01-25 01:41:18.236582 analogvnn-1.0.2/analogvnn/backward/BackwardIdentity.py
--rw-r--r--   0        0        0    10140 2023-03-21 17:16:13.013355 analogvnn-1.0.2/analogvnn/backward/BackwardModule.py
--rw-r--r--   0        0        0      894 2023-01-25 01:41:18.245026 analogvnn-1.0.2/analogvnn/backward/BackwardUsingForward.py
--rw-r--r--   0        0        0        0 2023-01-25 01:41:18.232132 analogvnn-1.0.2/analogvnn/backward/__init__.py
--rw-r--r--   0        0        0       43 2023-03-07 11:00:42.961641 analogvnn-1.0.2/analogvnn/fn/__init__.py
--rw-r--r--   0        0        0      609 2023-03-07 11:00:42.963657 analogvnn-1.0.2/analogvnn/fn/dirac_delta.py
--rw-r--r--   0        0        0     1998 2023-01-25 01:41:18.238101 analogvnn-1.0.2/analogvnn/fn/reduce_precision.py
--rw-r--r--   0        0        0     1145 2023-01-25 01:41:18.238665 analogvnn-1.0.2/analogvnn/fn/test.py
--rw-r--r--   0        0        0      435 2023-01-25 01:41:18.243027 analogvnn-1.0.2/analogvnn/fn/to_matrix.py
--rw-r--r--   0        0        0     2154 2023-01-25 01:41:18.245026 analogvnn-1.0.2/analogvnn/fn/train.py
--rw-r--r--   0        0        0     6149 2023-03-21 17:16:13.013355 analogvnn-1.0.2/analogvnn/graph/AccumulateGrad.py
--rw-r--r--   0        0        0    16888 2023-03-21 17:16:13.013355 analogvnn-1.0.2/analogvnn/graph/AcyclicDirectedGraph.py
--rw-r--r--   0        0        0     3077 2023-03-21 17:16:13.013355 analogvnn-1.0.2/analogvnn/graph/ArgsKwargs.py
--rw-r--r--   0        0        0    12307 2023-01-25 01:41:18.248023 analogvnn-1.0.2/analogvnn/graph/BackwardGraph.py
--rw-r--r--   0        0        0     4580 2023-03-21 17:16:13.013355 analogvnn-1.0.2/analogvnn/graph/ForwardGraph.py
--rw-r--r--   0        0        0      503 2023-01-25 01:41:18.246026 analogvnn-1.0.2/analogvnn/graph/GraphEnum.py
--rw-r--r--   0        0        0     1655 2023-03-21 17:16:13.020383 analogvnn-1.0.2/analogvnn/graph/ModelGraph.py
--rw-r--r--   0        0        0     4130 2023-03-21 17:16:13.013355 analogvnn-1.0.2/analogvnn/graph/ModelGraphState.py
--rw-r--r--   0        0        0        0 2023-01-25 01:41:18.243027 analogvnn-1.0.2/analogvnn/graph/__init__.py
--rw-r--r--   0        0        0     2444 2023-03-07 11:00:42.977680 analogvnn-1.0.2/analogvnn/graph/to_graph_viz_digraph.py
--rw-r--r--   0        0        0     3326 2023-03-21 17:16:13.020383 analogvnn-1.0.2/analogvnn/nn/Linear.py
--rw-r--r--   0        0        0        0 2023-01-25 01:41:18.248023 analogvnn-1.0.2/analogvnn/nn/__init__.py
--rw-r--r--   0        0        0     1149 2023-01-25 01:41:18.251094 analogvnn-1.0.2/analogvnn/nn/activation/Activation.py
--rw-r--r--   0        0        0      944 2023-01-25 01:41:18.256113 analogvnn-1.0.2/analogvnn/nn/activation/BinaryStep.py
--rw-r--r--   0        0        0     3336 2023-03-21 17:16:13.020383 analogvnn-1.0.2/analogvnn/nn/activation/ELU.py
--rw-r--r--   0        0        0     2052 2023-01-25 01:41:18.261162 analogvnn-1.0.2/analogvnn/nn/activation/Gaussian.py
--rw-r--r--   0        0        0     1622 2023-03-21 17:16:13.020383 analogvnn-1.0.2/analogvnn/nn/activation/Identity.py
--rw-r--r--   0        0        0     4197 2023-03-21 17:16:13.020383 analogvnn-1.0.2/analogvnn/nn/activation/ReLU.py
--rw-r--r--   0        0        0      979 2023-01-25 01:41:18.260166 analogvnn-1.0.2/analogvnn/nn/activation/SiLU.py
--rw-r--r--   0        0        0     1953 2023-01-25 01:41:18.259178 analogvnn-1.0.2/analogvnn/nn/activation/Sigmoid.py
--rw-r--r--   0        0        0     1765 2023-01-25 01:41:18.260166 analogvnn-1.0.2/analogvnn/nn/activation/Tanh.py
--rw-r--r--   0        0        0        0 2023-01-25 01:41:18.249123 analogvnn-1.0.2/analogvnn/nn/activation/__init__.py
--rw-r--r--   0        0        0      895 2023-01-25 01:41:18.263373 analogvnn-1.0.2/analogvnn/nn/module/FullSequential.py
--rw-r--r--   0        0        0     9179 2023-05-08 02:47:38.140435 analogvnn-1.0.2/analogvnn/nn/module/Layer.py
--rw-r--r--   0        0        0    10854 2023-05-08 02:45:16.171304 analogvnn-1.0.2/analogvnn/nn/module/Model.py
--rw-r--r--   0        0        0     1470 2023-01-25 01:41:18.268523 analogvnn-1.0.2/analogvnn/nn/module/Sequential.py
--rw-r--r--   0        0        0        0 2023-01-25 01:41:18.257237 analogvnn-1.0.2/analogvnn/nn/module/__init__.py
--rw-r--r--   0        0        0     7169 2023-03-21 17:16:13.023398 analogvnn-1.0.2/analogvnn/nn/noise/GaussianNoise.py
--rw-r--r--   0        0        0     7025 2023-03-21 17:16:13.023398 analogvnn-1.0.2/analogvnn/nn/noise/LaplacianNoise.py
--rw-r--r--   0        0        0      154 2023-03-07 11:00:42.987197 analogvnn-1.0.2/analogvnn/nn/noise/Noise.py
--rw-r--r--   0        0        0    10404 2023-03-21 17:16:13.023398 analogvnn-1.0.2/analogvnn/nn/noise/PoissonNoise.py
--rw-r--r--   0        0        0     6860 2023-03-21 17:16:13.020383 analogvnn-1.0.2/analogvnn/nn/noise/UniformNoise.py
--rw-r--r--   0        0        0        0 2023-01-25 01:41:18.263373 analogvnn-1.0.2/analogvnn/nn/noise/__init__.py
--rw-r--r--   0        0        0     2044 2023-03-07 11:00:42.990199 analogvnn-1.0.2/analogvnn/nn/normalize/Clamp.py
--rw-r--r--   0        0        0     4469 2023-03-21 17:16:13.023398 analogvnn-1.0.2/analogvnn/nn/normalize/LPNorm.py
--rw-r--r--   0        0        0      170 2023-03-07 11:00:42.991704 analogvnn-1.0.2/analogvnn/nn/normalize/Normalize.py
--rw-r--r--   0        0        0        0 2023-01-25 01:41:18.267528 analogvnn-1.0.2/analogvnn/nn/normalize/__init__.py
--rw-r--r--   0        0        0      166 2023-03-07 11:00:42.992711 analogvnn-1.0.2/analogvnn/nn/precision/Precision.py
--rw-r--r--   0        0        0     3092 2023-03-21 17:16:13.023398 analogvnn-1.0.2/analogvnn/nn/precision/ReducePrecision.py
--rw-r--r--   0        0        0     2554 2023-03-21 17:16:13.023398 analogvnn-1.0.2/analogvnn/nn/precision/StochasticReducePrecision.py
--rw-r--r--   0        0        0        0 2023-01-25 01:41:18.269514 analogvnn-1.0.2/analogvnn/nn/precision/__init__.py
--rw-r--r--   0        0        0     1515 2023-03-21 17:16:13.023398 analogvnn-1.0.2/analogvnn/parameter/Parameter.py
--rw-r--r--   0        0        0     8916 2023-03-27 02:13:36.114947 analogvnn-1.0.2/analogvnn/parameter/PseudoParameter.py
--rw-r--r--   0        0        0        0 2023-01-25 01:41:18.276870 analogvnn-1.0.2/analogvnn/parameter/__init__.py
--rw-r--r--   0        0        0     7965 2023-03-21 17:16:13.023398 analogvnn-1.0.2/analogvnn/utils/TensorboardModelLog.py
--rw-r--r--   0        0        0        0 2023-01-25 01:41:18.277865 analogvnn-1.0.2/analogvnn/utils/__init__.py
--rw-r--r--   0        0        0      591 2023-03-07 11:00:42.998714 analogvnn-1.0.2/analogvnn/utils/common_types.py
--rw-r--r--   0        0        0     2390 2023-03-07 11:00:42.999711 analogvnn-1.0.2/analogvnn/utils/get_model_summaries.py
--rw-r--r--   0        0        0     3016 2023-03-21 17:16:13.033447 analogvnn-1.0.2/analogvnn/utils/is_cpu_cuda.py
--rw-r--r--   0        0        0    35029 2023-03-21 17:16:13.023398 analogvnn-1.0.2/analogvnn/utils/render_autograd_graph.py
--rw-r--r--   0        0        0     1011 2023-01-25 01:41:18.284864 analogvnn-1.0.2/analogvnn/utils/to_tensor_parameter.py
--rw-r--r--   0        0        0     4474 2023-05-08 02:49:22.952588 analogvnn-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     6077 1970-01-01 00:00:00.000000 analogvnn-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0    17182 2023-01-25 01:41:18.328863 analogvnn-1.0.3/LICENSE
+-rw-r--r--   0        0        0     2823 2023-05-08 04:24:44.806296 analogvnn-1.0.3/README.md
+-rw-r--r--   0        0        0      728 2023-03-07 11:00:42.959136 analogvnn-1.0.3/analogvnn/__init__.py
+-rw-r--r--   0        0        0     2873 2023-03-21 17:16:13.013355 analogvnn-1.0.3/analogvnn/backward/BackwardFunction.py
+-rw-r--r--   0        0        0      930 2023-01-25 01:41:18.236582 analogvnn-1.0.3/analogvnn/backward/BackwardIdentity.py
+-rw-r--r--   0        0        0    10140 2023-03-21 17:16:13.013355 analogvnn-1.0.3/analogvnn/backward/BackwardModule.py
+-rw-r--r--   0        0        0      894 2023-01-25 01:41:18.245026 analogvnn-1.0.3/analogvnn/backward/BackwardUsingForward.py
+-rw-r--r--   0        0        0        0 2023-01-25 01:41:18.232132 analogvnn-1.0.3/analogvnn/backward/__init__.py
+-rw-r--r--   0        0        0       43 2023-03-07 11:00:42.961641 analogvnn-1.0.3/analogvnn/fn/__init__.py
+-rw-r--r--   0        0        0      609 2023-03-07 11:00:42.963657 analogvnn-1.0.3/analogvnn/fn/dirac_delta.py
+-rw-r--r--   0        0        0     1998 2023-01-25 01:41:18.238101 analogvnn-1.0.3/analogvnn/fn/reduce_precision.py
+-rw-r--r--   0        0        0     1145 2023-01-25 01:41:18.238665 analogvnn-1.0.3/analogvnn/fn/test.py
+-rw-r--r--   0        0        0      435 2023-01-25 01:41:18.243027 analogvnn-1.0.3/analogvnn/fn/to_matrix.py
+-rw-r--r--   0        0        0     2154 2023-01-25 01:41:18.245026 analogvnn-1.0.3/analogvnn/fn/train.py
+-rw-r--r--   0        0        0     6149 2023-03-21 17:16:13.013355 analogvnn-1.0.3/analogvnn/graph/AccumulateGrad.py
+-rw-r--r--   0        0        0    16888 2023-03-21 17:16:13.013355 analogvnn-1.0.3/analogvnn/graph/AcyclicDirectedGraph.py
+-rw-r--r--   0        0        0     3091 2023-05-08 04:09:29.467715 analogvnn-1.0.3/analogvnn/graph/ArgsKwargs.py
+-rw-r--r--   0        0        0    12447 2023-05-08 04:22:49.100096 analogvnn-1.0.3/analogvnn/graph/BackwardGraph.py
+-rw-r--r--   0        0        0     4580 2023-03-21 17:16:13.013355 analogvnn-1.0.3/analogvnn/graph/ForwardGraph.py
+-rw-r--r--   0        0        0      503 2023-01-25 01:41:18.246026 analogvnn-1.0.3/analogvnn/graph/GraphEnum.py
+-rw-r--r--   0        0        0     1655 2023-03-21 17:16:13.020383 analogvnn-1.0.3/analogvnn/graph/ModelGraph.py
+-rw-r--r--   0        0        0     4036 2023-05-08 04:03:55.473530 analogvnn-1.0.3/analogvnn/graph/ModelGraphState.py
+-rw-r--r--   0        0        0        0 2023-01-25 01:41:18.243027 analogvnn-1.0.3/analogvnn/graph/__init__.py
+-rw-r--r--   0        0        0     2444 2023-03-07 11:00:42.977680 analogvnn-1.0.3/analogvnn/graph/to_graph_viz_digraph.py
+-rw-r--r--   0        0        0     3326 2023-03-21 17:16:13.020383 analogvnn-1.0.3/analogvnn/nn/Linear.py
+-rw-r--r--   0        0        0        0 2023-01-25 01:41:18.248023 analogvnn-1.0.3/analogvnn/nn/__init__.py
+-rw-r--r--   0        0        0     1149 2023-01-25 01:41:18.251094 analogvnn-1.0.3/analogvnn/nn/activation/Activation.py
+-rw-r--r--   0        0        0      944 2023-01-25 01:41:18.256113 analogvnn-1.0.3/analogvnn/nn/activation/BinaryStep.py
+-rw-r--r--   0        0        0     3336 2023-03-21 17:16:13.020383 analogvnn-1.0.3/analogvnn/nn/activation/ELU.py
+-rw-r--r--   0        0        0     2052 2023-01-25 01:41:18.261162 analogvnn-1.0.3/analogvnn/nn/activation/Gaussian.py
+-rw-r--r--   0        0        0     1622 2023-03-21 17:16:13.020383 analogvnn-1.0.3/analogvnn/nn/activation/Identity.py
+-rw-r--r--   0        0        0     4197 2023-03-21 17:16:13.020383 analogvnn-1.0.3/analogvnn/nn/activation/ReLU.py
+-rw-r--r--   0        0        0      979 2023-01-25 01:41:18.260166 analogvnn-1.0.3/analogvnn/nn/activation/SiLU.py
+-rw-r--r--   0        0        0     1953 2023-01-25 01:41:18.259178 analogvnn-1.0.3/analogvnn/nn/activation/Sigmoid.py
+-rw-r--r--   0        0        0     1765 2023-01-25 01:41:18.260166 analogvnn-1.0.3/analogvnn/nn/activation/Tanh.py
+-rw-r--r--   0        0        0        0 2023-01-25 01:41:18.249123 analogvnn-1.0.3/analogvnn/nn/activation/__init__.py
+-rw-r--r--   0        0        0      895 2023-01-25 01:41:18.263373 analogvnn-1.0.3/analogvnn/nn/module/FullSequential.py
+-rw-r--r--   0        0        0     9179 2023-05-08 02:47:38.140435 analogvnn-1.0.3/analogvnn/nn/module/Layer.py
+-rw-r--r--   0        0        0    10854 2023-05-08 03:50:03.052825 analogvnn-1.0.3/analogvnn/nn/module/Model.py
+-rw-r--r--   0        0        0     1470 2023-01-25 01:41:18.268523 analogvnn-1.0.3/analogvnn/nn/module/Sequential.py
+-rw-r--r--   0        0        0        0 2023-01-25 01:41:18.257237 analogvnn-1.0.3/analogvnn/nn/module/__init__.py
+-rw-r--r--   0        0        0     7169 2023-03-21 17:16:13.023398 analogvnn-1.0.3/analogvnn/nn/noise/GaussianNoise.py
+-rw-r--r--   0        0        0     7025 2023-03-21 17:16:13.023398 analogvnn-1.0.3/analogvnn/nn/noise/LaplacianNoise.py
+-rw-r--r--   0        0        0      154 2023-03-07 11:00:42.987197 analogvnn-1.0.3/analogvnn/nn/noise/Noise.py
+-rw-r--r--   0        0        0    10404 2023-03-21 17:16:13.023398 analogvnn-1.0.3/analogvnn/nn/noise/PoissonNoise.py
+-rw-r--r--   0        0        0     6860 2023-03-21 17:16:13.020383 analogvnn-1.0.3/analogvnn/nn/noise/UniformNoise.py
+-rw-r--r--   0        0        0        0 2023-01-25 01:41:18.263373 analogvnn-1.0.3/analogvnn/nn/noise/__init__.py
+-rw-r--r--   0        0        0     2044 2023-03-07 11:00:42.990199 analogvnn-1.0.3/analogvnn/nn/normalize/Clamp.py
+-rw-r--r--   0        0        0     4469 2023-03-21 17:16:13.023398 analogvnn-1.0.3/analogvnn/nn/normalize/LPNorm.py
+-rw-r--r--   0        0        0      170 2023-03-07 11:00:42.991704 analogvnn-1.0.3/analogvnn/nn/normalize/Normalize.py
+-rw-r--r--   0        0        0        0 2023-01-25 01:41:18.267528 analogvnn-1.0.3/analogvnn/nn/normalize/__init__.py
+-rw-r--r--   0        0        0      166 2023-03-07 11:00:42.992711 analogvnn-1.0.3/analogvnn/nn/precision/Precision.py
+-rw-r--r--   0        0        0     3092 2023-03-21 17:16:13.023398 analogvnn-1.0.3/analogvnn/nn/precision/ReducePrecision.py
+-rw-r--r--   0        0        0     2554 2023-03-21 17:16:13.023398 analogvnn-1.0.3/analogvnn/nn/precision/StochasticReducePrecision.py
+-rw-r--r--   0        0        0        0 2023-01-25 01:41:18.269514 analogvnn-1.0.3/analogvnn/nn/precision/__init__.py
+-rw-r--r--   0        0        0     1515 2023-03-21 17:16:13.023398 analogvnn-1.0.3/analogvnn/parameter/Parameter.py
+-rw-r--r--   0        0        0     8916 2023-03-27 02:13:36.114947 analogvnn-1.0.3/analogvnn/parameter/PseudoParameter.py
+-rw-r--r--   0        0        0        0 2023-01-25 01:41:18.276870 analogvnn-1.0.3/analogvnn/parameter/__init__.py
+-rw-r--r--   0        0        0     7965 2023-03-21 17:16:13.023398 analogvnn-1.0.3/analogvnn/utils/TensorboardModelLog.py
+-rw-r--r--   0        0        0        0 2023-01-25 01:41:18.277865 analogvnn-1.0.3/analogvnn/utils/__init__.py
+-rw-r--r--   0        0        0      591 2023-03-07 11:00:42.998714 analogvnn-1.0.3/analogvnn/utils/common_types.py
+-rw-r--r--   0        0        0     2390 2023-03-07 11:00:42.999711 analogvnn-1.0.3/analogvnn/utils/get_model_summaries.py
+-rw-r--r--   0        0        0     3016 2023-03-21 17:16:13.033447 analogvnn-1.0.3/analogvnn/utils/is_cpu_cuda.py
+-rw-r--r--   0        0        0    35029 2023-03-21 17:16:13.023398 analogvnn-1.0.3/analogvnn/utils/render_autograd_graph.py
+-rw-r--r--   0        0        0     1011 2023-01-25 01:41:18.284864 analogvnn-1.0.3/analogvnn/utils/to_tensor_parameter.py
+-rw-r--r--   0        0        0     4474 2023-05-08 04:19:52.990970 analogvnn-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     6077 1970-01-01 00:00:00.000000 analogvnn-1.0.3/PKG-INFO
```

### Comparing `analogvnn-1.0.2/LICENSE` & `analogvnn-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.2/README.md` & `analogvnn-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.2/analogvnn/__init__.py` & `analogvnn-1.0.3/analogvnn/__init__.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.2/analogvnn/backward/BackwardFunction.py` & `analogvnn-1.0.3/analogvnn/backward/BackwardFunction.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.2/analogvnn/backward/BackwardIdentity.py` & `analogvnn-1.0.3/analogvnn/backward/BackwardIdentity.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.2/analogvnn/backward/BackwardModule.py` & `analogvnn-1.0.3/analogvnn/backward/BackwardModule.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.2/analogvnn/backward/BackwardUsingForward.py` & `analogvnn-1.0.3/analogvnn/backward/BackwardUsingForward.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.2/analogvnn/fn/dirac_delta.py` & `analogvnn-1.0.3/analogvnn/fn/dirac_delta.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.2/analogvnn/fn/reduce_precision.py` & `analogvnn-1.0.3/analogvnn/fn/reduce_precision.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.2/analogvnn/fn/test.py` & `analogvnn-1.0.3/analogvnn/fn/test.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.2/analogvnn/fn/train.py` & `analogvnn-1.0.3/analogvnn/fn/train.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.2/analogvnn/graph/AccumulateGrad.py` & `analogvnn-1.0.3/analogvnn/graph/AccumulateGrad.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.2/analogvnn/graph/AcyclicDirectedGraph.py` & `analogvnn-1.0.3/analogvnn/graph/AcyclicDirectedGraph.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.2/analogvnn/graph/ArgsKwargs.py` & `analogvnn-1.0.3/analogvnn/graph/ArgsKwargs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
-from typing import List, Dict, Any, Union, Optional
+from typing import List, Dict, Any, Union, Optional, Tuple
 
 __all__ = ['InputOutput', 'ArgsKwargs', 'ArgsKwargsInput', 'ArgsKwargsOutput']
 
 
 @dataclass
 class InputOutput:
     """Inputs and outputs of a module.
@@ -105,9 +105,9 @@
         else:
             return None
 
 
 ArgsKwargsInput = Union[ArgsKwargs, Dict, List, Any, None]
 """ArgsKwargsInput is the input type for ArgsKwargs"""
 
-ArgsKwargsOutput = Union[ArgsKwargs, List, Any, None]
+ArgsKwargsOutput = Union[ArgsKwargs, List, Tuple, Any, None]
 """ArgsKwargsOutput is the output type for ArgsKwargs"""
```

### Comparing `analogvnn-1.0.2/analogvnn/graph/BackwardGraph.py` & `analogvnn-1.0.3/analogvnn/graph/BackwardGraph.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,32 +29,37 @@
 
         Returns:
             ArgsKwargsOutput: gradient of the inputs function w.r.t. loss
         """
 
         self.graph_state.ready_for_backward(exception=True)
 
+        loss = self.graph_state.loss
+        self.graph_state.set_loss(None)
+
+        if loss is None:
+            loss = self.graph_state.outputs.args
+
+        if not isinstance(loss, (tuple, list)):
+            loss = [loss]
+
         if len(gradient) == 0:
-            gradient = None
-        elif len(gradient) == 1:
-            gradient = gradient[0]
+            gradient = (None,) * len(loss)
 
         if self.graph_state.use_autograd_graph:
-            result = self.graph_state.loss.backward(gradient=gradient)
+            result = tuple(v.backward(gradient=gradient[i]) for i, v in enumerate(loss))
         else:
             grad_outputs = torch.autograd.grad(
-                outputs=self.graph_state.loss,
+                outputs=loss,
                 inputs=self.graph_state.outputs.args,
                 grad_outputs=gradient,
                 retain_graph=True
             )
             result = self.calculate(*grad_outputs)
 
-        self.graph_state.set_loss(None)
-
         return result
 
     def compile(self, is_static=True):
         """Compile the graph.
 
         Args:
             is_static (bool): If True, the graph is not changing during runtime and will be cached.
```

### Comparing `analogvnn-1.0.2/analogvnn/graph/ForwardGraph.py` & `analogvnn-1.0.3/analogvnn/graph/ForwardGraph.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.2/analogvnn/graph/ModelGraph.py` & `analogvnn-1.0.3/analogvnn/graph/ModelGraph.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.2/analogvnn/graph/ModelGraphState.py` & `analogvnn-1.0.3/analogvnn/graph/ModelGraphState.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,17 +82,14 @@
             RuntimeError: if the state is not ready for backward pass and exception is True.
         """
 
         if exception:
             if self.outputs is None:
                 raise RuntimeError('output is not set.')
 
-            if self._loss is None:
-                raise RuntimeError('loss is not set.')
-
         return not (self.outputs is None or self._loss is None)
 
     @property
     def inputs(self) -> Optional[ArgsKwargs]:
         """Get the inputs.
 
         Returns:
```

### Comparing `analogvnn-1.0.2/analogvnn/graph/to_graph_viz_digraph.py` & `analogvnn-1.0.3/analogvnn/graph/to_graph_viz_digraph.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.2/analogvnn/nn/Linear.py` & `analogvnn-1.0.3/analogvnn/nn/Linear.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.2/analogvnn/nn/activation/Activation.py` & `analogvnn-1.0.3/analogvnn/nn/activation/Activation.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.2/analogvnn/nn/activation/BinaryStep.py` & `analogvnn-1.0.3/analogvnn/nn/activation/BinaryStep.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.2/analogvnn/nn/activation/ELU.py` & `analogvnn-1.0.3/analogvnn/nn/activation/ELU.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.2/analogvnn/nn/activation/Gaussian.py` & `analogvnn-1.0.3/analogvnn/nn/activation/Gaussian.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.2/analogvnn/nn/activation/Identity.py` & `analogvnn-1.0.3/analogvnn/nn/activation/Identity.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.2/analogvnn/nn/activation/ReLU.py` & `analogvnn-1.0.3/analogvnn/nn/activation/ReLU.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.2/analogvnn/nn/activation/SiLU.py` & `analogvnn-1.0.3/analogvnn/nn/activation/SiLU.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.2/analogvnn/nn/activation/Sigmoid.py` & `analogvnn-1.0.3/analogvnn/nn/activation/Sigmoid.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.2/analogvnn/nn/activation/Tanh.py` & `analogvnn-1.0.3/analogvnn/nn/activation/Tanh.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.2/analogvnn/nn/module/FullSequential.py` & `analogvnn-1.0.3/analogvnn/nn/module/FullSequential.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.2/analogvnn/nn/module/Layer.py` & `analogvnn-1.0.3/analogvnn/nn/module/Layer.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.2/analogvnn/nn/module/Model.py` & `analogvnn-1.0.3/analogvnn/nn/module/Model.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.2/analogvnn/nn/module/Sequential.py` & `analogvnn-1.0.3/analogvnn/nn/module/Sequential.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.2/analogvnn/nn/noise/GaussianNoise.py` & `analogvnn-1.0.3/analogvnn/nn/noise/GaussianNoise.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.2/analogvnn/nn/noise/LaplacianNoise.py` & `analogvnn-1.0.3/analogvnn/nn/noise/LaplacianNoise.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.2/analogvnn/nn/noise/PoissonNoise.py` & `analogvnn-1.0.3/analogvnn/nn/noise/PoissonNoise.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.2/analogvnn/nn/noise/UniformNoise.py` & `analogvnn-1.0.3/analogvnn/nn/noise/UniformNoise.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.2/analogvnn/nn/normalize/Clamp.py` & `analogvnn-1.0.3/analogvnn/nn/normalize/Clamp.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.2/analogvnn/nn/normalize/LPNorm.py` & `analogvnn-1.0.3/analogvnn/nn/normalize/LPNorm.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.2/analogvnn/nn/precision/ReducePrecision.py` & `analogvnn-1.0.3/analogvnn/nn/precision/ReducePrecision.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.2/analogvnn/nn/precision/StochasticReducePrecision.py` & `analogvnn-1.0.3/analogvnn/nn/precision/StochasticReducePrecision.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.2/analogvnn/parameter/Parameter.py` & `analogvnn-1.0.3/analogvnn/parameter/Parameter.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.2/analogvnn/parameter/PseudoParameter.py` & `analogvnn-1.0.3/analogvnn/parameter/PseudoParameter.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.2/analogvnn/utils/TensorboardModelLog.py` & `analogvnn-1.0.3/analogvnn/utils/TensorboardModelLog.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.2/analogvnn/utils/common_types.py` & `analogvnn-1.0.3/analogvnn/utils/common_types.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.2/analogvnn/utils/get_model_summaries.py` & `analogvnn-1.0.3/analogvnn/utils/get_model_summaries.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.2/analogvnn/utils/is_cpu_cuda.py` & `analogvnn-1.0.3/analogvnn/utils/is_cpu_cuda.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.2/analogvnn/utils/render_autograd_graph.py` & `analogvnn-1.0.3/analogvnn/utils/render_autograd_graph.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.2/analogvnn/utils/to_tensor_parameter.py` & `analogvnn-1.0.3/analogvnn/utils/to_tensor_parameter.py`

 * *Files identical despite different names*

### Comparing `analogvnn-1.0.2/pyproject.toml` & `analogvnn-1.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 [tool.setuptools]
 py-modules = ['analogvnn']
 
 [project]
 # $ pip install analogvnn
 name = "analogvnn"
-version = "1.0.2"
+version = "1.0.3"
 description = "A fully modular framework for modeling and optimizing analog/photonic neural networks"  # Optional
 readme = "README.md"
 requires-python = ">=3.7"
 license = { file = "LICENSE" }
 keywords = ["deep-learning", "analog", "photonics", "neural-network", "framework", "pytorch"]
 authors = [
     { name = "Vivswan Shah", email = "vivswanshah@pitt.edu" }
```

### Comparing `analogvnn-1.0.2/PKG-INFO` & `analogvnn-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: analogvnn
-Version: 1.0.2
+Version: 1.0.3
 Summary: A fully modular framework for modeling and optimizing analog/photonic neural networks
 Keywords: deep-learning,analog,photonics,neural-network,framework,pytorch
 Author-email: Vivswan Shah <vivswanshah@pitt.edu>
 Maintainer-email: Vivswan Shah <vivswanshah@pitt.edu>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
```

