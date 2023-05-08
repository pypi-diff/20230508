# Comparing `tmp/tensorcircuit-nightly-0.9.0.dev20230507.tar.gz` & `tmp/tensorcircuit-nightly-0.9.0.dev20230508.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensorcircuit-nightly-0.9.0.dev20230507.tar", last modified: Sun May  7 12:46:48 2023, max compression
+gzip compressed data, was "tensorcircuit-nightly-0.9.0.dev20230508.tar", last modified: Mon May  8 12:39:36 2023, max compression
```

## Comparing `tensorcircuit-nightly-0.9.0.dev20230507.tar` & `tensorcircuit-nightly-0.9.0.dev20230508.tar`

### file list

```diff
@@ -1,136 +1,136 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-07 12:46:48.102214 tensorcircuit-nightly-0.9.0.dev20230507/
--rw-r--r--   0 runner    (1001) docker     (122)    23737 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (122)     1023 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (122)    11358 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      132 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    20508 2023-05-07 12:46:48.102214 tensorcircuit-nightly-0.9.0.dev20230507/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    18206 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     5968 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/README_cn.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-07 12:46:48.078214 tensorcircuit-nightly-0.9.0.dev20230507/docs/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-07 12:46:48.082214 tensorcircuit-nightly-0.9.0.dev20230507/docs/source/
--rw-r--r--   0 runner    (1001) docker     (122)     6332 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/docs/source/advance.rst
--rw-r--r--   0 runner    (1001) docker     (122)     6308 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/docs/source/cnconf.py
--rw-r--r--   0 runner    (1001) docker     (122)     6397 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)     8192 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/docs/source/contribution.rst
--rw-r--r--   0 runner    (1001) docker     (122)    10971 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/docs/source/faq.rst
--rw-r--r--   0 runner    (1001) docker     (122)     3677 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/docs/source/generate_rst.py
--rw-r--r--   0 runner    (1001) docker     (122)     2786 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)     8695 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/docs/source/infras.rst
--rw-r--r--   0 runner    (1001) docker     (122)      680 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/docs/source/modules.rst
--rw-r--r--   0 runner    (1001) docker     (122)     4334 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/docs/source/modules.rst.backup
--rw-r--r--   0 runner    (1001) docker     (122)    27533 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/docs/source/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (122)     8223 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/docs/source/sharpbits.rst
--rw-r--r--   0 runner    (1001) docker     (122)      226 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/docs/source/textbooktoc.rst
--rw-r--r--   0 runner    (1001) docker     (122)      674 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/docs/source/tutorial.rst
--rw-r--r--   0 runner    (1001) docker     (122)      669 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/docs/source/tutorial_cn.rst
--rw-r--r--   0 runner    (1001) docker     (122)      509 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/docs/source/whitepapertoc.rst
--rw-r--r--   0 runner    (1001) docker     (122)      531 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/docs/source/whitepapertoc_cn.rst
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-07 12:46:48.102214 tensorcircuit-nightly-0.9.0.dev20230507/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1059 2023-05-07 12:46:39.000000 tensorcircuit-nightly-0.9.0.dev20230507/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-07 12:46:48.086214 tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/
--rw-r--r--   0 runner    (1001) docker     (122)     1450 2023-05-07 12:46:39.000000 tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2901 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/about.py
--rw-r--r--   0 runner    (1001) docker     (122)    39188 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/abstractcircuit.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-07 12:46:48.090214 tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/applications/
--rw-r--r--   0 runner    (1001) docker     (122)      234 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/applications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    34460 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/applications/dqas.py
--rw-r--r--   0 runner    (1001) docker     (122)    15348 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/applications/graphdata.py
--rw-r--r--   0 runner    (1001) docker     (122)    18124 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/applications/layers.py
--rw-r--r--   0 runner    (1001) docker     (122)    14032 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/applications/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    36391 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/applications/vags.py
--rw-r--r--   0 runner    (1001) docker     (122)    15117 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/applications/van.py
--rw-r--r--   0 runner    (1001) docker     (122)    23156 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/applications/vqes.py
--rw-r--r--   0 runner    (1001) docker     (122)     8235 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/asciiart.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-07 12:46:48.090214 tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/backends/
--rw-r--r--   0 runner    (1001) docker     (122)       80 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    57621 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/backends/abstract_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)     1713 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/backends/backend_factory.py
--rw-r--r--   0 runner    (1001) docker     (122)    14928 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/backends/cupy_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)    24925 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/backends/jax_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)     4008 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/backends/jax_ops.py
--rw-r--r--   0 runner    (1001) docker     (122)    13813 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/backends/numpy_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)    24148 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/backends/pytorch_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)     3825 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/backends/pytorch_ops.py
--rw-r--r--   0 runner    (1001) docker     (122)    31112 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/backends/tensorflow_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)     3377 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/backends/tf_ops.py
--rw-r--r--   0 runner    (1001) docker     (122)    34020 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/basecircuit.py
--rw-r--r--   0 runner    (1001) docker     (122)    28637 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/channels.py
--rw-r--r--   0 runner    (1001) docker     (122)    36220 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/circuit.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-07 12:46:48.094214 tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/cloud/
--rw-r--r--   0 runner    (1001) docker     (122)       67 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14582 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/cloud/abstraction.py
--rw-r--r--   0 runner    (1001) docker     (122)    17674 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/cloud/apis.py
--rw-r--r--   0 runner    (1001) docker     (122)       60 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/cloud/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     2252 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/cloud/local.py
--rw-r--r--   0 runner    (1001) docker     (122)     2238 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/cloud/quafu_provider.py
--rw-r--r--   0 runner    (1001) docker     (122)    14212 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/cloud/tencent.py
--rw-r--r--   0 runner    (1001) docker     (122)     3622 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/cloud/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     7791 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/cloud/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-07 12:46:48.094214 tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/compiler/
--rw-r--r--   0 runner    (1001) docker     (122)      165 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/compiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1490 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/compiler/composed_compiler.py
--rw-r--r--   0 runner    (1001) docker     (122)     5215 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/compiler/qiskit_compiler.py
--rw-r--r--   0 runner    (1001) docker     (122)    28754 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/cons.py
--rw-r--r--   0 runner    (1001) docker     (122)    13806 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/densitymatrix.py
--rw-r--r--   0 runner    (1001) docker     (122)    15210 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/experimental.py
--rw-r--r--   0 runner    (1001) docker     (122)    29016 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/gates.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-07 12:46:48.094214 tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/interfaces/
--rw-r--r--   0 runner    (1001) docker     (122)      469 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1439 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/interfaces/numpy.py
--rw-r--r--   0 runner    (1001) docker     (122)     3402 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/interfaces/scipy.py
--rw-r--r--   0 runner    (1001) docker     (122)     3355 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/interfaces/tensorflow.py
--rw-r--r--   0 runner    (1001) docker     (122)    10364 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/interfaces/tensortrans.py
--rw-r--r--   0 runner    (1001) docker     (122)     5030 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/interfaces/torch.py
--rw-r--r--   0 runner    (1001) docker     (122)     9959 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/keras.py
--rw-r--r--   0 runner    (1001) docker     (122)    15270 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/mps_base.py
--rw-r--r--   0 runner    (1001) docker     (122)    34350 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/mpscircuit.py
--rw-r--r--   0 runner    (1001) docker     (122)    11861 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/noisemodel.py
--rw-r--r--   0 runner    (1001) docker     (122)    82850 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/quantum.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-07 12:46:48.094214 tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/results/
--rw-r--r--   0 runner    (1001) docker     (122)       89 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/results/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3366 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/results/counts.py
--rw-r--r--   0 runner    (1001) docker     (122)    31362 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/results/readout_mitigation.py
--rw-r--r--   0 runner    (1001) docker     (122)     9413 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/simplify.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-07 12:46:48.094214 tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/templates/
--rw-r--r--   0 runner    (1001) docker     (122)      111 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6158 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/templates/blocks.py
--rw-r--r--   0 runner    (1001) docker     (122)     1061 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/templates/chems.py
--rw-r--r--   0 runner    (1001) docker     (122)     1933 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/templates/dataset.py
--rw-r--r--   0 runner    (1001) docker     (122)     5811 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/templates/ensemble.py
--rw-r--r--   0 runner    (1001) docker     (122)     3934 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/templates/graphs.py
--rw-r--r--   0 runner    (1001) docker     (122)    10942 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/templates/measurements.py
--rw-r--r--   0 runner    (1001) docker     (122)     3552 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/torchnn.py
--rw-r--r--   0 runner    (1001) docker     (122)    27335 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/translation.py
--rw-r--r--   0 runner    (1001) docker     (122)     7060 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    12195 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/vis.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-07 12:46:48.098214 tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    20508 2023-05-07 12:46:47.000000 tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3519 2023-05-07 12:46:47.000000 tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-07 12:46:47.000000 tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      110 2023-05-07 12:46:47.000000 tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       20 2023-05-07 12:46:47.000000 tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit_nightly.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-07 12:46:48.102214 tensorcircuit-nightly-0.9.0.dev20230507/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1457 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)    33394 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/tests/test_backends.py
--rw-r--r--   0 runner    (1001) docker     (122)     3805 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/tests/test_calibrating.py
--rw-r--r--   0 runner    (1001) docker     (122)    11237 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/tests/test_channels.py
--rw-r--r--   0 runner    (1001) docker     (122)    46467 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/tests/test_circuit.py
--rw-r--r--   0 runner    (1001) docker     (122)     4204 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/tests/test_cloud.py
--rw-r--r--   0 runner    (1001) docker     (122)     2518 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/tests/test_compiler.py
--rw-r--r--   0 runner    (1001) docker     (122)    17232 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/tests/test_dmcircuit.py
--rw-r--r--   0 runner    (1001) docker     (122)     1974 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/tests/test_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (122)     4593 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/tests/test_gates.py
--rw-r--r--   0 runner    (1001) docker     (122)    13220 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/tests/test_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (122)     4656 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/tests/test_keras.py
--rw-r--r--   0 runner    (1001) docker     (122)     6639 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/tests/test_miscs.py
--rw-r--r--   0 runner    (1001) docker     (122)    10552 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/tests/test_mpscircuit.py
--rw-r--r--   0 runner    (1001) docker     (122)     5637 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/tests/test_noisemodel.py
--rw-r--r--   0 runner    (1001) docker     (122)      753 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/tests/test_qaoa.py
--rw-r--r--   0 runner    (1001) docker     (122)    16823 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/tests/test_quantum.py
--rw-r--r--   0 runner    (1001) docker     (122)     1245 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/tests/test_quantum_attr.py
--rw-r--r--   0 runner    (1001) docker     (122)    11050 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/tests/test_results.py
--rw-r--r--   0 runner    (1001) docker     (122)     1175 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/tests/test_simplify.py
--rw-r--r--   0 runner    (1001) docker     (122)     5962 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/tests/test_templates.py
--rw-r--r--   0 runner    (1001) docker     (122)     2039 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/tests/test_torchnn.py
--rw-r--r--   0 runner    (1001) docker     (122)     3163 2023-05-07 12:15:32.000000 tensorcircuit-nightly-0.9.0.dev20230507/tests/test_van.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 12:39:36.059514 tensorcircuit-nightly-0.9.0.dev20230508/
+-rw-r--r--   0 runner    (1001) docker     (122)    23884 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1023 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (122)    11358 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      132 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    20682 2023-05-08 12:39:36.059514 tensorcircuit-nightly-0.9.0.dev20230508/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    18300 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     6048 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/README_cn.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 12:39:36.047514 tensorcircuit-nightly-0.9.0.dev20230508/docs/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 12:39:36.051514 tensorcircuit-nightly-0.9.0.dev20230508/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (122)     6332 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/docs/source/advance.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     6308 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/docs/source/cnconf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6397 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8192 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/docs/source/contribution.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    10971 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/docs/source/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3677 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/docs/source/generate_rst.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2985 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     8695 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/docs/source/infras.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      680 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/docs/source/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     4334 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/docs/source/modules.rst.backup
+-rw-r--r--   0 runner    (1001) docker     (122)    27533 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/docs/source/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     8223 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/docs/source/sharpbits.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      226 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/docs/source/textbooktoc.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      674 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/docs/source/tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      669 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/docs/source/tutorial_cn.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      509 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/docs/source/whitepapertoc.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      531 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/docs/source/whitepapertoc_cn.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-08 12:39:36.059514 tensorcircuit-nightly-0.9.0.dev20230508/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1059 2023-05-08 12:39:30.000000 tensorcircuit-nightly-0.9.0.dev20230508/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 12:39:36.051514 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/
+-rw-r--r--   0 runner    (1001) docker     (122)     1460 2023-05-08 12:39:29.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2901 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/about.py
+-rw-r--r--   0 runner    (1001) docker     (122)    39188 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/abstractcircuit.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 12:39:36.055514 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/applications/
+-rw-r--r--   0 runner    (1001) docker     (122)      234 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/applications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34460 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/applications/dqas.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15348 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/applications/graphdata.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18124 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/applications/layers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14032 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/applications/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36391 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/applications/vags.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15117 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/applications/van.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23156 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/applications/vqes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8235 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/asciiart.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 12:39:36.055514 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/backends/
+-rw-r--r--   0 runner    (1001) docker     (122)       80 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    57621 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/backends/abstract_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1713 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/backends/backend_factory.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14928 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/backends/cupy_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24925 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/backends/jax_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4024 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/backends/jax_ops.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13813 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/backends/numpy_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24148 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/backends/pytorch_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3825 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/backends/pytorch_ops.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31112 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/backends/tensorflow_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3377 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/backends/tf_ops.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34020 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/basecircuit.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28637 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/channels.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36220 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/circuit.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 12:39:36.055514 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/cloud/
+-rw-r--r--   0 runner    (1001) docker     (122)       67 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14582 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/cloud/abstraction.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17866 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/cloud/apis.py
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/cloud/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2252 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/cloud/local.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2238 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/cloud/quafu_provider.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14212 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/cloud/tencent.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3622 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/cloud/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7894 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/cloud/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 12:39:36.055514 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/compiler/
+-rw-r--r--   0 runner    (1001) docker     (122)      165 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/compiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1490 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/compiler/composed_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5215 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/compiler/qiskit_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29573 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/cons.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13806 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/densitymatrix.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15210 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/experimental.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29016 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/gates.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 12:39:36.055514 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (122)      469 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1439 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/interfaces/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3402 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/interfaces/scipy.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3355 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/interfaces/tensorflow.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10364 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/interfaces/tensortrans.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5030 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/interfaces/torch.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10126 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/keras.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15270 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/mps_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34350 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/mpscircuit.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11861 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/noisemodel.py
+-rw-r--r--   0 runner    (1001) docker     (122)    82850 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/quantum.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 12:39:36.055514 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/results/
+-rw-r--r--   0 runner    (1001) docker     (122)       89 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/results/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3366 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/results/counts.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31362 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/results/readout_mitigation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9413 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/simplify.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 12:39:36.059514 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)      111 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6158 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/templates/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1061 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/templates/chems.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1933 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/templates/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5811 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/templates/ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3934 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/templates/graphs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10942 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/templates/measurements.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4621 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/torchnn.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27335 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/translation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7060 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12195 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/vis.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 12:39:36.059514 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    20682 2023-05-08 12:39:35.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3519 2023-05-08 12:39:35.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-08 12:39:35.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      110 2023-05-08 12:39:35.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       20 2023-05-08 12:39:35.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 12:39:36.059514 tensorcircuit-nightly-0.9.0.dev20230508/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1457 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33394 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tests/test_backends.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3805 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tests/test_calibrating.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11237 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tests/test_channels.py
+-rw-r--r--   0 runner    (1001) docker     (122)    46467 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tests/test_circuit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4204 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tests/test_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2518 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tests/test_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17232 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tests/test_dmcircuit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1974 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tests/test_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4593 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tests/test_gates.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13220 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tests/test_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4656 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tests/test_keras.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6639 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tests/test_miscs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10552 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tests/test_mpscircuit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5637 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tests/test_noisemodel.py
+-rw-r--r--   0 runner    (1001) docker     (122)      753 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tests/test_qaoa.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16823 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tests/test_quantum.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1245 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tests/test_quantum_attr.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11050 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tests/test_results.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1175 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tests/test_simplify.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5962 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tests/test_templates.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2823 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tests/test_torchnn.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3163 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tests/test_van.py
```

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/CHANGELOG.md` & `tensorcircuit-nightly-0.9.0.dev20230508/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 # Change Log
 
 ## Unreleased
 
+### Added
+
+- Add `tc.TorchHardwarLayer` for shortcut layer construction of quantum hardware experiments
+
+- Add cotengra contractor setup shortcut
+
 ### Changed
 
 - Add compiler and cloud namespace to the global tensorcircuit namespace
 
 ## 0.9.0
 
 ### Added
```

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/HISTORY.md` & `tensorcircuit-nightly-0.9.0.dev20230508/HISTORY.md`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/LICENSE` & `tensorcircuit-nightly-0.9.0.dev20230508/LICENSE`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/PKG-INFO` & `tensorcircuit-nightly-0.9.0.dev20230508/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorcircuit-nightly
-Version: 0.9.0.dev20230507
+Version: 0.9.0.dev20230508
 Summary: nightly release for tensorcircuit
 Home-page: https://github.com/refraction-ray/tensorcircuit-dev
 Author: TensorCircuit Authors
 Author-email: znfesnpbh.tc@gmail.com
 License: UNKNOWN
 Description: <p align="center">
           <a href="https://github.com/tencent-quantum-lab/tensorcircuit">
@@ -143,14 +143,18 @@
         
         ### Guidelines
         
         For contribution guidelines and notes, see [CONTRIBUTING](/CONTRIBUTING.md).
         
         We welcome [issues](https://github.com/tencent-quantum-lab/tensorcircuit/issues), [PRs](https://github.com/tencent-quantum-lab/tensorcircuit/pulls), and [discussions](https://github.com/tencent-quantum-lab/tensorcircuit/discussions) from everyone, and these are all hosted on GitHub.
         
+        ### License
+        
+        TensorCircuit is open source, released under the Apache License, Version 2.0.
+        
         ### Contributors
         
         <!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
         <!-- prettier-ignore-start -->
         <!-- markdownlint-disable -->
         <table>
           <tbody>
@@ -198,39 +202,45 @@
         <!-- ALL-CONTRIBUTORS-LIST:END -->
         
         ## Research and Applications
         
         ### DQAS
         
         For the application of Differentiable Quantum Architecture Search, see [applications](/tensorcircuit/applications).
+        
         Reference paper: https://arxiv.org/abs/2010.08561 (published in QST).
         
         ### VQNHE
         
         For the application of Variational Quantum-Neural Hybrid Eigensolver, see [applications](/tensorcircuit/applications).
+        
         Reference paper: https://arxiv.org/abs/2106.05105 (published in PRL) and https://arxiv.org/abs/2112.10380.
         
-        ### VQEX - MBL
+        ### VQEX-MBL
         
         For the application of VQEX on MBL phase identification, see the [tutorial](/docs/source/tutorials/vqex_mbl.ipynb).
+        
         Reference paper: https://arxiv.org/abs/2111.13719 (published in PRB).
         
-        ### Stark - DTC
+        ### Stark-DTC
         
         For the numerical demosntration of discrete time crystal enabled by Stark many-body localization, see the Floquet simulation [demo](/examples/timeevolution_trotter.py).
+        
         Reference paper: https://arxiv.org/abs/2208.02866 (published in PRL).
         
         ### EMQAOA-DARBO
         
         For the numerical simulation and hardware experiments with error mitigation on QAOA, see the [project repo](https://github.com/sherrylixuecheng/EMQAOA-DARBO).
+        
         Reference paper: https://arxiv.org/abs/2303.14877.
         
         ### TenCirChem
         
         [TenCirChem](https://github.com/tencent-quantum-lab/TenCirChem) is an efficient and versatile quantum computation package for molecular properties. TenCirChem is based on TensorCircuit and is optimized for chemistry applications.
+        
         Reference paper: https://arxiv.org/abs/2303.10825.
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: tensorflow
```

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/README.md` & `tensorcircuit-nightly-0.9.0.dev20230508/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -135,14 +135,18 @@
 
 ### Guidelines
 
 For contribution guidelines and notes, see [CONTRIBUTING](/CONTRIBUTING.md).
 
 We welcome [issues](https://github.com/tencent-quantum-lab/tensorcircuit/issues), [PRs](https://github.com/tencent-quantum-lab/tensorcircuit/pulls), and [discussions](https://github.com/tencent-quantum-lab/tensorcircuit/discussions) from everyone, and these are all hosted on GitHub.
 
+### License
+
+TensorCircuit is open source, released under the Apache License, Version 2.0.
+
 ### Contributors
 
 <!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
 <!-- prettier-ignore-start -->
 <!-- markdownlint-disable -->
 <table>
   <tbody>
@@ -190,33 +194,39 @@
 <!-- ALL-CONTRIBUTORS-LIST:END -->
 
 ## Research and Applications
 
 ### DQAS
 
 For the application of Differentiable Quantum Architecture Search, see [applications](/tensorcircuit/applications).
+
 Reference paper: https://arxiv.org/abs/2010.08561 (published in QST).
 
 ### VQNHE
 
 For the application of Variational Quantum-Neural Hybrid Eigensolver, see [applications](/tensorcircuit/applications).
+
 Reference paper: https://arxiv.org/abs/2106.05105 (published in PRL) and https://arxiv.org/abs/2112.10380.
 
-### VQEX - MBL
+### VQEX-MBL
 
 For the application of VQEX on MBL phase identification, see the [tutorial](/docs/source/tutorials/vqex_mbl.ipynb).
+
 Reference paper: https://arxiv.org/abs/2111.13719 (published in PRB).
 
-### Stark - DTC
+### Stark-DTC
 
 For the numerical demosntration of discrete time crystal enabled by Stark many-body localization, see the Floquet simulation [demo](/examples/timeevolution_trotter.py).
+
 Reference paper: https://arxiv.org/abs/2208.02866 (published in PRL).
 
 ### EMQAOA-DARBO
 
 For the numerical simulation and hardware experiments with error mitigation on QAOA, see the [project repo](https://github.com/sherrylixuecheng/EMQAOA-DARBO).
+
 Reference paper: https://arxiv.org/abs/2303.14877.
 
 ### TenCirChem
 
 [TenCirChem](https://github.com/tencent-quantum-lab/TenCirChem) is an efficient and versatile quantum computation package for molecular properties. TenCirChem is based on TensorCircuit and is optimized for chemistry applications.
+
 Reference paper: https://arxiv.org/abs/2303.10825.
```

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/README_cn.md` & `tensorcircuit-nightly-0.9.0.dev20230508/README_cn.md`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 TensorCircuit 现在支持真实量子硬件连接和实验，并提供优雅的 CPU/GPU/QPU 混合部署方案（v0.9+）。
 
 ## 入门
 
 请从 [快速上手](/docs/source/quickstart.rst) 和 [Jupyter 教程](/docs/source/tutorials) 开始。
 
-有关更多信息和介绍，请参阅有用的 [示例脚本](/examples) 和 [完整文档](https://tensorcircuit.readthedocs.io/zh/latest/)。 [测试](/tests) 中的 API docstring 和测试用例也提供了丰富的信息。
+有关更多信息和介绍，请参阅有用的 [示例脚本](/examples) 和 [完整文档](https://tensorcircuit.readthedocs.io/zh/latest/)。 [测试](/tests)用例和 API docstring 也提供了丰富的使用信息。
 
 以下是一些最简易的演示。
 
 - 电路操作:
 
 ```python
 import tensorcircuit as tc
@@ -131,38 +131,48 @@
 
 ### 说明
 
 有关贡献指南和说明，请参阅 [贡献](/CONTRIBUTING.md)。
 
 我们欢迎大家提出 [issues](https://github.com/tencent-quantum-lab/tensorcircuit/issues), [PR](https://github.com/tencent-quantum-lab/tensorcircuit/pulls), 和 [讨论](https://github.com/tencent-quantum-lab/tensorcircuit/discussions)，这些都托管在 GitHub 上。
 
+### 协议
+
+TensorCircuit 是基于 Apache License 2.0 的开源软件。
+
 ## 研究和应用
 
 ### DQAS
 
 可微量子架构搜索的应用见 [应用](/tensorcircuit/applications)。
+
 参考论文：https://arxiv.org/abs/2010.08561 (QST)。
 
 ### VQNHE
 
 关于变分量子神经混合本征求解器的应用，请参见 [应用](tensorcircuit/applications)。
+
 参考论文：https://arxiv.org/abs/2106.05105 (PRL) 和 https://arxiv.org/abs/2112.10380 。
 
-### VQEX - MBL
+### VQEX-MBL
 
 VQEX 在 MBL 相位识别上的应用见 [教程](/docs/source/tutorials/vqex_mbl.ipynb)。
+
 参考论文: https://arxiv.org/abs/2111.13719 (PRB)。
 
-### Stark - DTC
+### Stark-DTC
+
+数值验证 Stark 多体局域化稳定的离散时间晶体，类似的 Floquet 系统模拟请参考 [例子](/examples/timeevolution_trotter.py)。
 
-数值验证 Stark 多体局域化稳定的离散时间晶体，类似的 Floquet 系统模拟请参考 [例子](/examples/timeevolution_trotter.py).
-参考论文: https://arxiv.org/abs/2208.02866 (PRL).
+参考论文: https://arxiv.org/abs/2208.02866 (PRL)。
 
 ### EMQAOA-DARBO
 
-数值模拟和带错误消除的真实量子硬件实验验证 QAOA 优化的代码请参考 [项目](https://github.com/sherrylixuecheng/EMQAOA-DARBO).
-参考论文: https://arxiv.org/abs/2303.14877.
+数值模拟和带错误消除的真实量子硬件实验验证 QAOA 优化的代码请参考 [项目](https://github.com/sherrylixuecheng/EMQAOA-DARBO)。
+
+参考论文: https://arxiv.org/abs/2303.14877。
 
 ### TenCirChem
 
 [TenCirChem](https://github.com/tencent-quantum-lab/TenCirChem) 是高效的，专注于处理和计算分子性质的量子计算软件。其基于 TensorCircuit 并为量子化学任务进行了专门的优化。
-参考论文: https://arxiv.org/abs/2303.10825.
+
+参考论文: https://arxiv.org/abs/2303.10825。
```

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/docs/source/advance.rst` & `tensorcircuit-nightly-0.9.0.dev20230508/docs/source/advance.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/docs/source/cnconf.py` & `tensorcircuit-nightly-0.9.0.dev20230508/docs/source/cnconf.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/docs/source/conf.py` & `tensorcircuit-nightly-0.9.0.dev20230508/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/docs/source/contribution.rst` & `tensorcircuit-nightly-0.9.0.dev20230508/docs/source/contribution.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/docs/source/faq.rst` & `tensorcircuit-nightly-0.9.0.dev20230508/docs/source/faq.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/docs/source/generate_rst.py` & `tensorcircuit-nightly-0.9.0.dev20230508/docs/source/generate_rst.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/docs/source/index.rst` & `tensorcircuit-nightly-0.9.0.dev20230508/docs/source/index.rst`

 * *Files 6% similar despite different names*

```diff
@@ -26,24 +26,28 @@
 The current core authors of TensorCircuit are `Shi-Xin Zhang <https://github.com/refraction-ray>`_ and `Yu-Qin Chen <https://github.com/yutuer21>`_.
 We also thank `contributions <https://github.com/tencent-quantum-lab/tensorcircuit/graphs/contributors>`_ from the lab and the open source community.
 
 * Source code: https://github.com/tencent-quantum-lab/tensorcircuit
 
 * Documentation: https://tensorcircuit.readthedocs.io 
 
-* Software Whitepaper published in Quantum: https://quantum-journal.org/papers/q-2023-02-02-912/
+* Software Whitepaper (published in Quantum): https://quantum-journal.org/papers/q-2023-02-02-912/
 
 * Issue Tracker: https://github.com/tencent-quantum-lab/tensorcircuit/issues
 
 * Forum: https://github.com/tencent-quantum-lab/tensorcircuit/discussions
 
 * PyPI page: https://pypi.org/project/tensorcircuit
 
 * DockerHub page: https://hub.docker.com/repository/docker/tensorcircuit/tensorcircuit
 
+* Research and projects based on TensorCircuit: https://github.com/tencent-quantum-lab/tensorcircuit#research-and-applications
+
+* Tencent Quantum Cloud Service: https://quantum.tencent.com/cloud/
+
 If you have any further questions or collaboration ideas in terms of TensorCircuit, please send email to shixinzhang#tencent.com.
 
 
 Reference Documentation
 ----------------------------
 
 The following documentation sections briefly introduce TensorCircuit to the users and developpers.
```

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/docs/source/infras.rst` & `tensorcircuit-nightly-0.9.0.dev20230508/docs/source/infras.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/docs/source/modules.rst` & `tensorcircuit-nightly-0.9.0.dev20230508/docs/source/modules.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/docs/source/modules.rst.backup` & `tensorcircuit-nightly-0.9.0.dev20230508/docs/source/modules.rst.backup`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/docs/source/quickstart.rst` & `tensorcircuit-nightly-0.9.0.dev20230508/docs/source/quickstart.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/docs/source/sharpbits.rst` & `tensorcircuit-nightly-0.9.0.dev20230508/docs/source/sharpbits.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/docs/source/tutorial.rst` & `tensorcircuit-nightly-0.9.0.dev20230508/docs/source/tutorial.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/docs/source/tutorial_cn.rst` & `tensorcircuit-nightly-0.9.0.dev20230508/docs/source/tutorial_cn.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/docs/source/whitepapertoc_cn.rst` & `tensorcircuit-nightly-0.9.0.dev20230508/docs/source/whitepapertoc_cn.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/setup.py` & `tensorcircuit-nightly-0.9.0.dev20230508/setup.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/__init__.py` & `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.9.0.dev20230507"
+__version__ = "0.9.0.dev20230508"
 __author__ = "TensorCircuit Authors"
 __creator__ = "refraction-ray"
 
 from .utils import gpu_memory_share
 
 gpu_memory_share()
 
@@ -39,19 +39,19 @@
 from . import quantum
 from .quantum import QuOperator, QuVector, QuAdjointVector, QuScalar
 from . import compiler
 from . import cloud
 
 try:
     from . import keras
-    from .keras import QuantumLayer as KerasLayer
+    from .keras import KerasLayer, KerasHardwareLayer
 except ModuleNotFoundError:
     pass  # in case tf is not installed
 
 try:
     from . import torchnn
-    from .torchnn import QuantumNet as TorchLayer
+    from .torchnn import TorchLayer, TorchHardwareLayer
 except ModuleNotFoundError:
     pass  # in case torch is not installed
 
 # just for fun
 from .asciiart import set_ascii
```

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/about.py` & `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/about.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/abstractcircuit.py` & `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/abstractcircuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/applications/dqas.py` & `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/applications/dqas.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/applications/graphdata.py` & `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/applications/graphdata.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/applications/layers.py` & `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/applications/layers.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/applications/utils.py` & `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/applications/utils.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/applications/vags.py` & `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/applications/vags.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/applications/van.py` & `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/applications/van.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/applications/vqes.py` & `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/applications/vqes.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/asciiart.py` & `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/asciiart.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/backends/abstract_backend.py` & `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/backends/abstract_backend.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/backends/backend_factory.py` & `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/backends/backend_factory.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/backends/cupy_backend.py` & `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/backends/cupy_backend.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/backends/jax_backend.py` & `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/backends/jax_backend.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/backends/jax_ops.py` & `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/backends/jax_ops.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
 def jaxqr_bwd(res: Sequence[Array], tangents: Sequence[Array]) -> Tuple[Array]:
     a, q, r = res
     dq, dr = tangents
     dq = dq.conj()
     dr = dr.conj()
 
     def _TriangularSolve(x: Array, r: Array) -> Array:
-        return jax.scipy.linalg.solve_triangular(
+        return jax.scipy.linalg.solve_triangular(  # type: ignore
             r, x.T.conj(), lower=False, trans=0
         ).T.conj()
 
     def _QrGradSquareAndDeepMatrices(q: Array, r: Array, dq: Array, dr: Array) -> Array:
         # Modification begins
         rdiag = jnp.diag(r)
         rdiag = (jnp.abs(rdiag) < qr_epsilon) * qr_epsilon + (
```

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/backends/numpy_backend.py` & `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/backends/numpy_backend.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/backends/pytorch_backend.py` & `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/backends/pytorch_backend.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/backends/pytorch_ops.py` & `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/backends/pytorch_ops.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/backends/tensorflow_backend.py` & `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/backends/tensorflow_backend.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/backends/tf_ops.py` & `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/backends/tf_ops.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/basecircuit.py` & `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/basecircuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/channels.py` & `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/channels.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/circuit.py` & `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/circuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/cloud/abstraction.py` & `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/cloud/abstraction.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/cloud/apis.py` & `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/cloud/apis.py`

 * *Files 1% similar despite different names*

```diff
@@ -201,18 +201,22 @@
     homedir = os.path.expanduser("~")
     authpath = os.path.join(homedir, ".tc.auth.json")
     # provider, device = _preprocess(provider, device)
     if clear is True:
         saved_token = {}
     if token is None:
         if cached and os.path.exists(authpath):
-            with open(authpath, "r") as f:
-                file_token = json.load(f)
-                file_token = {k: b64decode_s(v) for k, v in file_token.items()}
-                # file_token = backend.tree_map(b64decode_s, file_token)
+            try:
+                with open(authpath, "r") as f:
+                    file_token = json.load(f)
+                    file_token = {k: b64decode_s(v) for k, v in file_token.items()}
+                    # file_token = backend.tree_map(b64decode_s, file_token)
+            except json.JSONDecodeError:
+                logger.warning("token file loading failure, set empty token instead")
+                file_token = {}
         else:
             file_token = {}
         file_token.update(saved_token)
         saved_token = file_token
     else:  # with token
         if isinstance(provider, str):
             provider = Provider.from_name(provider)
```

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/cloud/local.py` & `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/cloud/local.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/cloud/quafu_provider.py` & `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/cloud/quafu_provider.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/cloud/tencent.py` & `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/cloud/tencent.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/cloud/utils.py` & `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/cloud/utils.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/cloud/wrapper.py` & `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/cloud/wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,14 +135,15 @@
     cs = []
     infos = []
     exps = []
     if isinstance(device, str):
         device = get_device(device)
     for ps in pss:
         # TODO(@refraction-ray): Pauli string grouping
+        # https://docs.pennylane.ai/en/stable/_modules/pennylane/pauli/grouping/group_observables.html
         c1 = Circuit.from_qir(c.to_qir())
         exp = []
         for j, i in enumerate(ps):
             if i == 1:
                 c1.H(j)  # type: ignore
                 exp.append(j)
             elif i == 2:
```

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/compiler/composed_compiler.py` & `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/compiler/composed_compiler.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/compiler/qiskit_compiler.py` & `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/compiler/qiskit_compiler.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/cons.py` & `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/cons.py`

 * *Files 1% similar despite different names*

```diff
@@ -754,14 +754,40 @@
     :return: The new tensornetwork with its contractor set.
     :rtype: tn.Node
     """
     if not method:
         method = "greedy"
         # auto for small size fallbacks to dp, which has bug for now
         # see: https://github.com/dgasmith/opt_einsum/issues/172
+    if method.startswith("cotengra"):
+        # cotengra shortcut
+        import cotengra
+
+        if method == "cotengra":
+            method = "custom"
+            optimizer = cotengra.ReusableHyperOptimizer(
+                methods=["greedy", "kahypar"],
+                parallel=True,
+                minimize="combo",
+                max_time=30,
+                max_repeats=64,
+                progbar=True,
+            )
+        else:  # "cotengra-30-64"
+            _, mt, mr = method.split("-")
+            method = "custom"
+            optimizer = cotengra.ReusableHyperOptimizer(
+                methods=["greedy", "kahypar"],
+                parallel=True,
+                minimize="combo",
+                max_time=int(mt),
+                max_repeats=int(mr),
+                progbar=True,
+            )
+
     if method == "plain":
         cf = plain_contractor
     elif method == "plain-experimental":
         cf = partial(experimental_contractor, local_steps=kws.get("local_steps", 2))
     elif method == "tng":  # don't use, deprecated, no guarantee
         if has_ps:
             cf = tn_greedy_contractor
```

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/densitymatrix.py` & `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/densitymatrix.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/experimental.py` & `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/experimental.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/gates.py` & `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/gates.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/interfaces/numpy.py` & `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/interfaces/numpy.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/interfaces/scipy.py` & `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/interfaces/scipy.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/interfaces/tensorflow.py` & `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/interfaces/tensorflow.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/interfaces/tensortrans.py` & `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/interfaces/tensortrans.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/interfaces/torch.py` & `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/interfaces/torch.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/keras.py` & `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/keras.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,14 +139,19 @@
     #     return dict(list(base_config.items()) + list(config.items()))
 
 
 KerasLayer = QuantumLayer
 
 
 class HardwareLayer(QuantumLayer):
+    """
+    Keras Layer wrapping quantum function with cloud qpu access
+    (using :py:mod:`tensorcircuit.cloud` module)
+    """
+
     @tf.autograph.experimental.do_not_convert  # type: ignore
     def call(
         self,
         inputs: tf.Tensor,
         training: Optional[bool] = None,
         mask: Optional[tf.Tensor] = None,
         **kwargs: Any
@@ -166,14 +171,17 @@
             result = []
             for inp in inputs:
                 result.append(self.f(inp, *self.pqc_weights, **kwargs))
             result = tf.stack(result)
         return result
 
 
+KerasHardwareLayer = HardwareLayer
+
+
 def output_asis_loss(y_true: tf.Tensor, y_pred: tf.Tensor) -> tf.Tensor:
     """
     The keras loss function that directly taking the model output as the loss.
 
     :param y_true: Ignoring this parameter.
     :type y_true: tf.Tensor
     :param y_pred: Model output.
```

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/mps_base.py` & `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/mps_base.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/mpscircuit.py` & `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/mpscircuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/noisemodel.py` & `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/noisemodel.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/quantum.py` & `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/quantum.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/results/counts.py` & `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/results/counts.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/results/readout_mitigation.py` & `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/results/readout_mitigation.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/simplify.py` & `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/simplify.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/templates/blocks.py` & `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/templates/blocks.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/templates/chems.py` & `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/templates/chems.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/templates/dataset.py` & `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/templates/dataset.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/templates/ensemble.py` & `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/templates/ensemble.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/templates/graphs.py` & `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/templates/graphs.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/templates/measurements.py` & `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/templates/measurements.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/torchnn.py` & `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/torchnn.py`

 * *Files 23% similar despite different names*

```diff
@@ -93,7 +93,46 @@
 
     def forward(self, *inputs: Tensor) -> Tensor:
         ypred = self.f(*inputs, *self.q_weights)
         return ypred
 
 
 TorchLayer = QuantumNet
+
+
+class HardwareNet(QuantumNet):
+    """
+    PyTorch Layer wrapping quantum function with cloud qpu access
+    (using :py:mod:`tensorcircuit.cloud` module)
+    """
+
+    def __init__(
+        self,
+        f: Callable[..., Any],
+        weights_shape: Sequence[Tuple[int, ...]],
+        initializer: Union[Any, Sequence[Any]] = None,
+        use_vmap: bool = True,
+    ):
+        super().__init__(
+            f,
+            weights_shape,
+            initializer,
+            use_vmap=False,
+            use_interface=False,
+            use_jit=False,
+        )
+        self.batch_support = use_vmap
+
+    def forward(self, *inputs: Tensor) -> Tensor:
+        if self.batch_support:
+            ypred = []
+            batch = inputs[0].shape[0]
+            for i in range(batch):
+                inp = tuple([a[i] for a in inputs])
+                ypred.append(self.f(*inp, *self.q_weights))
+            ypred = torch.stack(ypred)  # type: ignore
+        else:
+            ypred = self.f(*inputs, *self.q_weights)
+        return ypred
+
+
+TorchHardwareLayer = HardwareNet
```

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/translation.py` & `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/translation.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/utils.py` & `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/utils.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit/vis.py` & `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/vis.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit_nightly.egg-info/PKG-INFO` & `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit_nightly.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorcircuit-nightly
-Version: 0.9.0.dev20230507
+Version: 0.9.0.dev20230508
 Summary: nightly release for tensorcircuit
 Home-page: https://github.com/refraction-ray/tensorcircuit-dev
 Author: TensorCircuit Authors
 Author-email: znfesnpbh.tc@gmail.com
 License: UNKNOWN
 Description: <p align="center">
           <a href="https://github.com/tencent-quantum-lab/tensorcircuit">
@@ -143,14 +143,18 @@
         
         ### Guidelines
         
         For contribution guidelines and notes, see [CONTRIBUTING](/CONTRIBUTING.md).
         
         We welcome [issues](https://github.com/tencent-quantum-lab/tensorcircuit/issues), [PRs](https://github.com/tencent-quantum-lab/tensorcircuit/pulls), and [discussions](https://github.com/tencent-quantum-lab/tensorcircuit/discussions) from everyone, and these are all hosted on GitHub.
         
+        ### License
+        
+        TensorCircuit is open source, released under the Apache License, Version 2.0.
+        
         ### Contributors
         
         <!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
         <!-- prettier-ignore-start -->
         <!-- markdownlint-disable -->
         <table>
           <tbody>
@@ -198,39 +202,45 @@
         <!-- ALL-CONTRIBUTORS-LIST:END -->
         
         ## Research and Applications
         
         ### DQAS
         
         For the application of Differentiable Quantum Architecture Search, see [applications](/tensorcircuit/applications).
+        
         Reference paper: https://arxiv.org/abs/2010.08561 (published in QST).
         
         ### VQNHE
         
         For the application of Variational Quantum-Neural Hybrid Eigensolver, see [applications](/tensorcircuit/applications).
+        
         Reference paper: https://arxiv.org/abs/2106.05105 (published in PRL) and https://arxiv.org/abs/2112.10380.
         
-        ### VQEX - MBL
+        ### VQEX-MBL
         
         For the application of VQEX on MBL phase identification, see the [tutorial](/docs/source/tutorials/vqex_mbl.ipynb).
+        
         Reference paper: https://arxiv.org/abs/2111.13719 (published in PRB).
         
-        ### Stark - DTC
+        ### Stark-DTC
         
         For the numerical demosntration of discrete time crystal enabled by Stark many-body localization, see the Floquet simulation [demo](/examples/timeevolution_trotter.py).
+        
         Reference paper: https://arxiv.org/abs/2208.02866 (published in PRL).
         
         ### EMQAOA-DARBO
         
         For the numerical simulation and hardware experiments with error mitigation on QAOA, see the [project repo](https://github.com/sherrylixuecheng/EMQAOA-DARBO).
+        
         Reference paper: https://arxiv.org/abs/2303.14877.
         
         ### TenCirChem
         
         [TenCirChem](https://github.com/tencent-quantum-lab/TenCirChem) is an efficient and versatile quantum computation package for molecular properties. TenCirChem is based on TensorCircuit and is optimized for chemistry applications.
+        
         Reference paper: https://arxiv.org/abs/2303.10825.
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: tensorflow
```

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/tensorcircuit_nightly.egg-info/SOURCES.txt` & `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/tests/conftest.py` & `tensorcircuit-nightly-0.9.0.dev20230508/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/tests/test_backends.py` & `tensorcircuit-nightly-0.9.0.dev20230508/tests/test_backends.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/tests/test_calibrating.py` & `tensorcircuit-nightly-0.9.0.dev20230508/tests/test_calibrating.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/tests/test_channels.py` & `tensorcircuit-nightly-0.9.0.dev20230508/tests/test_channels.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/tests/test_circuit.py` & `tensorcircuit-nightly-0.9.0.dev20230508/tests/test_circuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/tests/test_cloud.py` & `tensorcircuit-nightly-0.9.0.dev20230508/tests/test_cloud.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/tests/test_compiler.py` & `tensorcircuit-nightly-0.9.0.dev20230508/tests/test_compiler.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/tests/test_dmcircuit.py` & `tensorcircuit-nightly-0.9.0.dev20230508/tests/test_dmcircuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/tests/test_ensemble.py` & `tensorcircuit-nightly-0.9.0.dev20230508/tests/test_ensemble.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/tests/test_gates.py` & `tensorcircuit-nightly-0.9.0.dev20230508/tests/test_gates.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/tests/test_interfaces.py` & `tensorcircuit-nightly-0.9.0.dev20230508/tests/test_interfaces.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/tests/test_keras.py` & `tensorcircuit-nightly-0.9.0.dev20230508/tests/test_keras.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/tests/test_miscs.py` & `tensorcircuit-nightly-0.9.0.dev20230508/tests/test_miscs.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/tests/test_mpscircuit.py` & `tensorcircuit-nightly-0.9.0.dev20230508/tests/test_mpscircuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/tests/test_noisemodel.py` & `tensorcircuit-nightly-0.9.0.dev20230508/tests/test_noisemodel.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/tests/test_qaoa.py` & `tensorcircuit-nightly-0.9.0.dev20230508/tests/test_qaoa.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/tests/test_quantum.py` & `tensorcircuit-nightly-0.9.0.dev20230508/tests/test_quantum.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/tests/test_quantum_attr.py` & `tensorcircuit-nightly-0.9.0.dev20230508/tests/test_quantum_attr.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/tests/test_results.py` & `tensorcircuit-nightly-0.9.0.dev20230508/tests/test_results.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/tests/test_simplify.py` & `tensorcircuit-nightly-0.9.0.dev20230508/tests/test_simplify.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/tests/test_templates.py` & `tensorcircuit-nightly-0.9.0.dev20230508/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/tests/test_torchnn.py` & `tensorcircuit-nightly-0.9.0.dev20230508/tests/test_torchnn.py`

 * *Files 24% similar despite different names*

```diff
@@ -70,7 +70,30 @@
     noise = 0.2 * torchb.ones([2, n], dtype="float32")
     l = layer(state, noise)
     lsum = torchb.sum(l)
     print(l)
     lsum.backward()
     for p in layer.parameters():
         print(p.grad)
+
+
+@pytest.mark.parametrize("backend", [lf("tfb"), lf("jaxb"), lf("torchb")])
+def test_torchnn_hardware(backend):
+    n = 2
+
+    def qf(inputs, param):
+        inputs = tc.backend.convert_to_tensor(tc.get_backend("pytorch").numpy(inputs))
+        param = tc.backend.convert_to_tensor(tc.get_backend("pytorch").numpy(param))
+
+        c = tc.Circuit(n)
+        c.rx(0, theta=inputs[0])
+        c.rx(1, theta=inputs[1])
+        c.h(1)
+        c.rzz(0, 1, theta=param[0])
+        r = tc.backend.stack([c.expectation_ps(z=[i]) for i in range(n)])
+
+        r = tc.get_backend("pytorch").convert_to_tensor(tc.backend.numpy(r))
+        return torch.real(r)
+
+    ql = tc.torchnn.HardwareNet(qf, [1])
+    qnet = torch.nn.Sequential(ql, torch.nn.Linear(2, 1))
+    print(qnet(torch.ones([5, 2])))
```

### Comparing `tensorcircuit-nightly-0.9.0.dev20230507/tests/test_van.py` & `tensorcircuit-nightly-0.9.0.dev20230508/tests/test_van.py`

 * *Files identical despite different names*

