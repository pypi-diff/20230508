# Comparing `tmp/graph_attention_student-0.7.2.tar.gz` & `tmp/graph_attention_student-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graph_attention_student-0.7.2.tar", max compression
+gzip compressed data, was "graph_attention_student-0.9.0.tar", max compression
```

## Comparing `graph_attention_student-0.7.2.tar` & `graph_attention_student-0.9.0.tar`

### file list

```diff
@@ -1,67 +1,76 @@
--rwxr-xr-x   0        0        0     8961 2022-12-29 07:58:42.522987 graph_attention_student-0.7.2/README.rst
--rwxr-xr-x   0        0        0        5 2023-04-27 12:35:16.036165 graph_attention_student-0.7.2/graph_attention_student/VERSION
--rwxr-xr-x   0        0        0       90 2022-12-29 07:58:42.522987 graph_attention_student-0.7.2/graph_attention_student/__init__.py
--rwxr-xr-x   0        0        0    84242 2023-03-19 09:18:21.518826 graph_attention_student-0.7.2/graph_attention_student/_models.py
--rwxr-xr-x   0        0        0     1131 2022-12-29 07:58:42.522987 graph_attention_student-0.7.2/graph_attention_student/cli.py
--rwxr-xr-x   0        0        0    54483 2023-01-17 14:13:51.169936 graph_attention_student-0.7.2/graph_attention_student/data.py
--rwxr-xr-x   0        0        0        0 2022-12-29 07:58:42.522987 graph_attention_student-0.7.2/graph_attention_student/examples/__init__.py
--rw-r--r--   0        0        0     9670 2023-01-20 11:45:50.758439 graph_attention_student-0.7.2/graph_attention_student/examples/__pycache__/vgd_multitask_gnn.cpython-310.pyc
--rw-r--r--   0        0        0    12164 2023-01-20 09:12:31.703590 graph_attention_student-0.7.2/graph_attention_student/examples/__pycache__/vgd_multitask_megan.cpython-310.pyc
--rwxr-xr-x   0        0        0    11582 2022-12-29 07:58:42.522987 graph_attention_student-0.7.2/graph_attention_student/examples/gnes_example.py
--rwxr-xr-x   0        0        0    11569 2022-12-29 07:58:42.522987 graph_attention_student-0.7.2/graph_attention_student/examples/gnnx_example.py
--rwxr-xr-x   0        0        0    18745 2022-12-29 07:58:42.522987 graph_attention_student-0.7.2/graph_attention_student/examples/smiles_example.py
--rw-r--r--   0        0        0    14585 2023-01-20 12:59:31.279402 graph_attention_student-0.7.2/graph_attention_student/examples/vgd_multitask_gnn.py
--rw-r--r--   0        0        0     5503 2023-01-20 11:59:55.452453 graph_attention_student-0.7.2/graph_attention_student/examples/vgd_multitask_gnn_gatv2.py
--rw-r--r--   0        0        0     4809 2023-01-20 11:39:35.159855 graph_attention_student-0.7.2/graph_attention_student/examples/vgd_multitask_gnn_gin.py
--rwxr-xr-x   0        0        0    20103 2023-01-20 10:32:00.863590 graph_attention_student-0.7.2/graph_attention_student/examples/vgd_multitask_megan.py
--rw-r--r--   0        0        0     1272 2023-01-20 09:42:42.629614 graph_attention_student-0.7.2/graph_attention_student/examples/vgd_multitask_megan_tadf.py
--rwxr-xr-x   0        0        0      726 2022-12-29 07:58:42.522987 graph_attention_student-0.7.2/graph_attention_student/experiments/README.rst
--rwxr-xr-x   0        0        0        0 2022-12-29 07:58:42.522987 graph_attention_student-0.7.2/graph_attention_student/experiments/__init__.py
--rw-r--r--   0        0        0    10604 2023-03-28 09:55:24.672691 graph_attention_student-0.7.2/graph_attention_student/experiments/__pycache__/vgd_classification.cpython-310.pyc
--rw-r--r--   0        0        0    15106 2023-03-20 09:39:48.984068 graph_attention_student-0.7.2/graph_attention_student/experiments/__pycache__/vgd_regression_supervised.cpython-310.pyc
--rw-r--r--   0        0        0    10324 2023-04-19 12:44:07.919515 graph_attention_student-0.7.2/graph_attention_student/experiments/__pycache__/vgd_single.cpython-310.pyc
--rw-r--r--   0        0        0     6258 2023-01-24 12:19:49.929234 graph_attention_student-0.7.2/graph_attention_student/experiments/__pycache__/vgd_single_gnnx.cpython-310.pyc
--rw-r--r--   0        0        0     1373 2023-01-24 14:25:26.991807 graph_attention_student-0.7.2/graph_attention_student/experiments/__pycache__/vgd_single_gnnx_aqsoldb.cpython-310.pyc
--rw-r--r--   0        0        0     4798 2023-04-27 11:59:03.979768 graph_attention_student-0.7.2/graph_attention_student/experiments/__pycache__/vgd_single_megan.cpython-310.pyc
--rw-r--r--   0        0        0     1345 2023-01-24 12:56:57.478326 graph_attention_student-0.7.2/graph_attention_student/experiments/__pycache__/vgd_single_megan_aqsoldb.cpython-310.pyc
--rwxr-xr-x   0        0        0     9205 2022-12-29 07:58:42.522987 graph_attention_student-0.7.2/graph_attention_student/experiments/process_aqsoldb.py
--rwxr-xr-x   0        0        0    31932 2022-12-29 07:58:42.522987 graph_attention_student-0.7.2/graph_attention_student/experiments/rb_motifs_multi.py
--rwxr-xr-x   0        0        0    34843 2022-12-29 07:58:42.522987 graph_attention_student-0.7.2/graph_attention_student/experiments/rb_motifs_single.py
--rw-r--r--   0        0        0      459 2023-01-24 12:36:03.337029 graph_attention_student-0.7.2/graph_attention_student/experiments/template_sub_experiment.py
--rw-r--r--   0        0        0    18495 2023-03-28 09:55:23.204678 graph_attention_student-0.7.2/graph_attention_student/experiments/vgd_classification.py
--rw-r--r--   0        0        0     5029 2023-03-29 07:00:40.799553 graph_attention_student-0.7.2/graph_attention_student/experiments/vgd_classification_megan.py
--rw-r--r--   0        0        0    18717 2023-03-19 08:35:02.980618 graph_attention_student-0.7.2/graph_attention_student/experiments/vgd_regression_posthoc.py
--rw-r--r--   0        0        0    24342 2023-03-20 09:39:47.552048 graph_attention_student-0.7.2/graph_attention_student/experiments/vgd_regression_supervised.py
--rw-r--r--   0        0        0     5567 2023-03-20 09:39:47.564048 graph_attention_student-0.7.2/graph_attention_student/experiments/vgd_regression_supervised_multi.py
--rw-r--r--   0        0        0     5788 2023-03-20 07:08:16.190877 graph_attention_student-0.7.2/graph_attention_student/experiments/vgd_regression_supervised_single.py
--rw-r--r--   0        0        0    17117 2023-04-19 12:42:45.170288 graph_attention_student-0.7.2/graph_attention_student/experiments/vgd_single.py
--rw-r--r--   0        0        0     8128 2023-01-24 12:19:49.761232 graph_attention_student-0.7.2/graph_attention_student/experiments/vgd_single_gnnx.py
--rw-r--r--   0        0        0     1038 2023-01-24 14:25:25.831799 graph_attention_student-0.7.2/graph_attention_student/experiments/vgd_single_gnnx_aqsoldb.py
--rw-r--r--   0        0        0     5506 2023-01-24 13:54:11.870993 graph_attention_student-0.7.2/graph_attention_student/experiments/vgd_single_gnnx_aqsoldb_dmpnn.py
--rw-r--r--   0        0        0     3581 2023-01-24 14:26:38.996305 graph_attention_student-0.7.2/graph_attention_student/experiments/vgd_single_gnnx_aqsoldb_gatv2.py
--rw-r--r--   0        0        0     5234 2023-01-24 13:19:46.309473 graph_attention_student-0.7.2/graph_attention_student/experiments/vgd_single_gnnx_aqsoldb_painn.py
--rw-r--r--   0        0        0     8048 2023-04-27 11:58:55.515701 graph_attention_student-0.7.2/graph_attention_student/experiments/vgd_single_megan.py
--rw-r--r--   0        0        0     1218 2023-04-27 12:34:08.343622 graph_attention_student-0.7.2/graph_attention_student/experiments/vgd_single_megan_aqsoldb.py
--rw-r--r--   0        0        0      695 2023-02-27 13:28:58.309313 graph_attention_student-0.7.2/graph_attention_student/keras.py
--rwxr-xr-x   0        0        0    20274 2023-02-23 19:42:55.562555 graph_attention_student-0.7.2/graph_attention_student/layers.py
--rw-r--r--   0        0        0      205 2023-03-19 09:12:41.525356 graph_attention_student-0.7.2/graph_attention_student/models/__init__.py
--rw-r--r--   0        0        0      380 2023-03-19 09:15:50.038102 graph_attention_student-0.7.2/graph_attention_student/models/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3314 2023-04-01 14:29:59.234990 graph_attention_student-0.7.2/graph_attention_student/models/__pycache__/gnes.cpython-310.pyc
--rw-r--r--   0        0        0     1950 2023-03-19 09:15:50.054102 graph_attention_student-0.7.2/graph_attention_student/models/__pycache__/gnnx.cpython-310.pyc
--rw-r--r--   0        0        0     9247 2023-04-01 10:01:31.663992 graph_attention_student-0.7.2/graph_attention_student/models/__pycache__/gradient.cpython-310.pyc
--rw-r--r--   0        0        0    15515 2023-04-27 12:08:11.991926 graph_attention_student-0.7.2/graph_attention_student/models/__pycache__/megan.cpython-310.pyc
--rw-r--r--   0        0        0     3406 2023-04-01 14:29:47.290900 graph_attention_student-0.7.2/graph_attention_student/models/gnes.py
--rw-r--r--   0        0        0     2590 2023-03-19 09:15:48.990097 graph_attention_student-0.7.2/graph_attention_student/models/gnnx.py
--rw-r--r--   0        0        0    12361 2023-04-01 10:01:20.259917 graph_attention_student-0.7.2/graph_attention_student/models/gradient.py
--rw-r--r--   0        0        0    29552 2023-04-27 12:08:10.919918 graph_attention_student-0.7.2/graph_attention_student/models/megan.py
--rwxr-xr-x   0        0        0     1040 2023-01-18 09:06:23.993806 graph_attention_student-0.7.2/graph_attention_student/templates/article.tex.j2
--rw-r--r--   0        0        0      375 2023-01-24 12:08:49.160527 graph_attention_student-0.7.2/graph_attention_student/templates/table.tex.j2
--rw-r--r--   0        0        0      151 2023-01-17 16:58:58.659355 graph_attention_student-0.7.2/graph_attention_student/templates/table_content.tex.j2
--rw-r--r--   0        0        0       76 2023-01-17 17:10:30.475776 graph_attention_student-0.7.2/graph_attention_student/templates/table_element_mean.tex.j2
--rwxr-xr-x   0        0        0    13166 2023-04-01 11:27:51.694228 graph_attention_student-0.7.2/graph_attention_student/training.py
--rwxr-xr-x   0        0        0     3753 2022-12-29 07:58:42.522987 graph_attention_student-0.7.2/graph_attention_student/typing.py
--rwxr-xr-x   0        0        0    15021 2023-01-18 08:39:58.301379 graph_attention_student-0.7.2/graph_attention_student/util.py
--rwxr-xr-x   0        0        0    16147 2023-03-27 10:44:14.975799 graph_attention_student-0.7.2/graph_attention_student/visualization.py
--rwxr-xr-x   0        0        0     1397 2023-04-27 12:35:16.028165 graph_attention_student-0.7.2/pyproject.toml
--rw-r--r--   0        0        0    10441 1970-01-01 00:00:00.000000 graph_attention_student-0.7.2/setup.py
--rw-r--r--   0        0        0    10052 1970-01-01 00:00:00.000000 graph_attention_student-0.7.2/PKG-INFO
+-rwxr-xr-x   0        0        0     8961 2022-12-29 07:58:42.522987 graph_attention_student-0.9.0/README.rst
+-rw-r--r--   0        0        0      658 2023-05-02 06:44:39.006261 graph_attention_student-0.9.0/graph_attention_student/README.rst
+-rwxr-xr-x   0        0        0        5 2023-05-02 06:45:23.138393 graph_attention_student-0.9.0/graph_attention_student/VERSION
+-rwxr-xr-x   0        0        0       90 2022-12-29 07:58:42.522987 graph_attention_student-0.9.0/graph_attention_student/__init__.py
+-rwxr-xr-x   0        0        0    84242 2023-03-19 09:18:21.518826 graph_attention_student-0.9.0/graph_attention_student/_models.py
+-rwxr-xr-x   0        0        0     1131 2022-12-29 07:58:42.522987 graph_attention_student-0.9.0/graph_attention_student/cli.py
+-rwxr-xr-x   0        0        0    56361 2023-05-01 14:05:46.498976 graph_attention_student-0.9.0/graph_attention_student/data.py
+-rw-r--r--   0        0        0     4392 2023-05-01 14:07:31.259868 graph_attention_student-0.9.0/graph_attention_student/examples/02_saving_models.py
+-rw-r--r--   0        0        0     4025 2023-05-01 14:15:40.271613 graph_attention_student-0.9.0/graph_attention_student/examples/03_loading_models.py
+-rw-r--r--   0        0        0     7587 2023-05-01 14:15:40.255613 graph_attention_student-0.9.0/graph_attention_student/examples/04_counterfactuals.py
+-rwxr-xr-x   0        0        0        0 2022-12-29 07:58:42.522987 graph_attention_student-0.9.0/graph_attention_student/examples/__init__.py
+-rw-r--r--   0        0        0     9670 2023-01-20 11:45:50.758439 graph_attention_student-0.9.0/graph_attention_student/examples/__pycache__/vgd_multitask_gnn.cpython-310.pyc
+-rw-r--r--   0        0        0    12164 2023-01-20 09:12:31.703590 graph_attention_student-0.9.0/graph_attention_student/examples/__pycache__/vgd_multitask_megan.cpython-310.pyc
+-rw-r--r--   0        0        0       53 2023-05-01 14:11:22.733000 graph_attention_student-0.9.0/graph_attention_student/examples/assets/aqsoldb_model/fingerprint.pb
+-rw-r--r--   0        0        0   117178 2023-05-01 14:11:22.933000 graph_attention_student-0.9.0/graph_attention_student/examples/assets/aqsoldb_model/keras_metadata.pb
+-rw-r--r--   0        0        0  2784317 2023-05-01 14:11:22.849000 graph_attention_student-0.9.0/graph_attention_student/examples/assets/aqsoldb_model/saved_model.pb
+-rw-r--r--   0        0        0   547453 2023-05-01 14:11:22.521000 graph_attention_student-0.9.0/graph_attention_student/examples/assets/aqsoldb_model/variables/variables.data-00000-of-00001
+-rw-r--r--   0        0        0     7266 2023-05-01 14:11:22.521000 graph_attention_student-0.9.0/graph_attention_student/examples/assets/aqsoldb_model/variables/variables.index
+-rwxr-xr-x   0        0        0    11582 2022-12-29 07:58:42.522987 graph_attention_student-0.9.0/graph_attention_student/examples/gnes_example.py
+-rwxr-xr-x   0        0        0    11569 2022-12-29 07:58:42.522987 graph_attention_student-0.9.0/graph_attention_student/examples/gnnx_example.py
+-rwxr-xr-x   0        0        0    18745 2022-12-29 07:58:42.522987 graph_attention_student-0.9.0/graph_attention_student/examples/smiles_example.py
+-rw-r--r--   0        0        0    14585 2023-01-20 12:59:31.279402 graph_attention_student-0.9.0/graph_attention_student/examples/vgd_multitask_gnn.py
+-rw-r--r--   0        0        0     5503 2023-01-20 11:59:55.452453 graph_attention_student-0.9.0/graph_attention_student/examples/vgd_multitask_gnn_gatv2.py
+-rw-r--r--   0        0        0     4809 2023-01-20 11:39:35.159855 graph_attention_student-0.9.0/graph_attention_student/examples/vgd_multitask_gnn_gin.py
+-rwxr-xr-x   0        0        0    20103 2023-01-20 10:32:00.863590 graph_attention_student-0.9.0/graph_attention_student/examples/vgd_multitask_megan.py
+-rw-r--r--   0        0        0     1272 2023-01-20 09:42:42.629614 graph_attention_student-0.9.0/graph_attention_student/examples/vgd_multitask_megan_tadf.py
+-rwxr-xr-x   0        0        0      726 2022-12-29 07:58:42.522987 graph_attention_student-0.9.0/graph_attention_student/experiments/README.rst
+-rwxr-xr-x   0        0        0        0 2022-12-29 07:58:42.522987 graph_attention_student-0.9.0/graph_attention_student/experiments/__init__.py
+-rw-r--r--   0        0        0    10604 2023-03-28 09:55:24.672691 graph_attention_student-0.9.0/graph_attention_student/experiments/__pycache__/vgd_classification.cpython-310.pyc
+-rw-r--r--   0        0        0    15106 2023-03-20 09:39:48.984068 graph_attention_student-0.9.0/graph_attention_student/experiments/__pycache__/vgd_regression_supervised.cpython-310.pyc
+-rw-r--r--   0        0        0    10324 2023-04-19 12:44:07.919515 graph_attention_student-0.9.0/graph_attention_student/experiments/__pycache__/vgd_single.cpython-310.pyc
+-rw-r--r--   0        0        0     6258 2023-01-24 12:19:49.929234 graph_attention_student-0.9.0/graph_attention_student/experiments/__pycache__/vgd_single_gnnx.cpython-310.pyc
+-rw-r--r--   0        0        0     1373 2023-01-24 14:25:26.991807 graph_attention_student-0.9.0/graph_attention_student/experiments/__pycache__/vgd_single_gnnx_aqsoldb.cpython-310.pyc
+-rw-r--r--   0        0        0     4798 2023-04-27 11:59:03.979768 graph_attention_student-0.9.0/graph_attention_student/experiments/__pycache__/vgd_single_megan.cpython-310.pyc
+-rw-r--r--   0        0        0     1345 2023-01-24 12:56:57.478326 graph_attention_student-0.9.0/graph_attention_student/experiments/__pycache__/vgd_single_megan_aqsoldb.cpython-310.pyc
+-rwxr-xr-x   0        0        0     9205 2022-12-29 07:58:42.522987 graph_attention_student-0.9.0/graph_attention_student/experiments/process_aqsoldb.py
+-rwxr-xr-x   0        0        0    31932 2022-12-29 07:58:42.522987 graph_attention_student-0.9.0/graph_attention_student/experiments/rb_motifs_multi.py
+-rwxr-xr-x   0        0        0    34843 2022-12-29 07:58:42.522987 graph_attention_student-0.9.0/graph_attention_student/experiments/rb_motifs_single.py
+-rw-r--r--   0        0        0      459 2023-01-24 12:36:03.337029 graph_attention_student-0.9.0/graph_attention_student/experiments/template_sub_experiment.py
+-rw-r--r--   0        0        0    18495 2023-03-28 09:55:23.204678 graph_attention_student-0.9.0/graph_attention_student/experiments/vgd_classification.py
+-rw-r--r--   0        0        0     5029 2023-03-29 07:00:40.799553 graph_attention_student-0.9.0/graph_attention_student/experiments/vgd_classification_megan.py
+-rw-r--r--   0        0        0    18717 2023-03-19 08:35:02.980618 graph_attention_student-0.9.0/graph_attention_student/experiments/vgd_regression_posthoc.py
+-rw-r--r--   0        0        0    24342 2023-03-20 09:39:47.552048 graph_attention_student-0.9.0/graph_attention_student/experiments/vgd_regression_supervised.py
+-rw-r--r--   0        0        0     5567 2023-03-20 09:39:47.564048 graph_attention_student-0.9.0/graph_attention_student/experiments/vgd_regression_supervised_multi.py
+-rw-r--r--   0        0        0     5788 2023-03-20 07:08:16.190877 graph_attention_student-0.9.0/graph_attention_student/experiments/vgd_regression_supervised_single.py
+-rw-r--r--   0        0        0    17117 2023-04-19 12:42:45.170288 graph_attention_student-0.9.0/graph_attention_student/experiments/vgd_single.py
+-rw-r--r--   0        0        0     8128 2023-01-24 12:19:49.761232 graph_attention_student-0.9.0/graph_attention_student/experiments/vgd_single_gnnx.py
+-rw-r--r--   0        0        0     1038 2023-01-24 14:25:25.831799 graph_attention_student-0.9.0/graph_attention_student/experiments/vgd_single_gnnx_aqsoldb.py
+-rw-r--r--   0        0        0     5506 2023-01-24 13:54:11.870993 graph_attention_student-0.9.0/graph_attention_student/experiments/vgd_single_gnnx_aqsoldb_dmpnn.py
+-rw-r--r--   0        0        0     3581 2023-01-24 14:26:38.996305 graph_attention_student-0.9.0/graph_attention_student/experiments/vgd_single_gnnx_aqsoldb_gatv2.py
+-rw-r--r--   0        0        0     5234 2023-01-24 13:19:46.309473 graph_attention_student-0.9.0/graph_attention_student/experiments/vgd_single_gnnx_aqsoldb_painn.py
+-rw-r--r--   0        0        0     8048 2023-04-27 11:58:55.515701 graph_attention_student-0.9.0/graph_attention_student/experiments/vgd_single_megan.py
+-rw-r--r--   0        0        0     1218 2023-04-27 13:02:32.628383 graph_attention_student-0.9.0/graph_attention_student/experiments/vgd_single_megan_aqsoldb.py
+-rw-r--r--   0        0        0      770 2023-05-01 10:33:09.005244 graph_attention_student-0.9.0/graph_attention_student/keras.py
+-rwxr-xr-x   0        0        0    20274 2023-02-23 19:42:55.562555 graph_attention_student-0.9.0/graph_attention_student/layers.py
+-rw-r--r--   0        0        0      205 2023-03-19 09:12:41.525356 graph_attention_student-0.9.0/graph_attention_student/models/__init__.py
+-rw-r--r--   0        0        0      380 2023-03-19 09:15:50.038102 graph_attention_student-0.9.0/graph_attention_student/models/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3314 2023-04-01 14:29:59.234990 graph_attention_student-0.9.0/graph_attention_student/models/__pycache__/gnes.cpython-310.pyc
+-rw-r--r--   0        0        0     1950 2023-03-19 09:15:50.054102 graph_attention_student-0.9.0/graph_attention_student/models/__pycache__/gnnx.cpython-310.pyc
+-rw-r--r--   0        0        0     9247 2023-04-01 10:01:31.663992 graph_attention_student-0.9.0/graph_attention_student/models/__pycache__/gradient.cpython-310.pyc
+-rw-r--r--   0        0        0    16309 2023-05-01 10:37:15.698781 graph_attention_student-0.9.0/graph_attention_student/models/__pycache__/megan.cpython-310.pyc
+-rw-r--r--   0        0        0     3406 2023-04-01 14:29:47.290900 graph_attention_student-0.9.0/graph_attention_student/models/gnes.py
+-rw-r--r--   0        0        0     2590 2023-03-19 09:15:48.990097 graph_attention_student-0.9.0/graph_attention_student/models/gnnx.py
+-rw-r--r--   0        0        0    12361 2023-04-01 10:01:20.259917 graph_attention_student-0.9.0/graph_attention_student/models/gradient.py
+-rw-r--r--   0        0        0    30258 2023-05-01 10:37:14.450773 graph_attention_student-0.9.0/graph_attention_student/models/megan.py
+-rwxr-xr-x   0        0        0     1040 2023-01-18 09:06:23.993806 graph_attention_student-0.9.0/graph_attention_student/templates/article.tex.j2
+-rw-r--r--   0        0        0      375 2023-01-24 12:08:49.160527 graph_attention_student-0.9.0/graph_attention_student/templates/table.tex.j2
+-rw-r--r--   0        0        0      151 2023-01-17 16:58:58.659355 graph_attention_student-0.9.0/graph_attention_student/templates/table_content.tex.j2
+-rw-r--r--   0        0        0       76 2023-01-17 17:10:30.475776 graph_attention_student-0.9.0/graph_attention_student/templates/table_element_mean.tex.j2
+-rwxr-xr-x   0        0        0    13166 2023-04-01 11:27:51.694228 graph_attention_student-0.9.0/graph_attention_student/training.py
+-rwxr-xr-x   0        0        0     3753 2022-12-29 07:58:42.522987 graph_attention_student-0.9.0/graph_attention_student/typing.py
+-rwxr-xr-x   0        0        0    15021 2023-01-18 08:39:58.301379 graph_attention_student-0.9.0/graph_attention_student/util.py
+-rwxr-xr-x   0        0        0    16147 2023-03-27 10:44:14.975799 graph_attention_student-0.9.0/graph_attention_student/visualization.py
+-rwxr-xr-x   0        0        0     1430 2023-05-02 06:45:23.130393 graph_attention_student-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0    10613 1970-01-01 00:00:00.000000 graph_attention_student-0.9.0/setup.py
+-rw-r--r--   0        0        0    10098 1970-01-01 00:00:00.000000 graph_attention_student-0.9.0/PKG-INFO
```

### Comparing `graph_attention_student-0.7.2/README.rst` & `graph_attention_student-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.2/graph_attention_student/_models.py` & `graph_attention_student-0.9.0/graph_attention_student/_models.py`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.2/graph_attention_student/cli.py` & `graph_attention_student-0.9.0/graph_attention_student/cli.py`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.2/graph_attention_student/data.py` & `graph_attention_student-0.9.0/graph_attention_student/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,14 +49,52 @@
         return value.tolist()
     elif isinstance(value, np.generic):
         return value.item()
     else:
         return value
 
 
+def process_index_data_map(index_data_map: t.Dict[int, dict],
+                           insert_empty_importances: bool = True,
+                           importance_channels: int = 1,
+                           ) -> t.Tuple[list, list]:
+    """
+    Given the ``index_data_map`` which was loaded from a visual graph dataset, this function will return a
+    tuple of two values: The first is the list of integer indices of the all the dataset elements and the
+    second element is the list of graph dicts representing each corresponding element.
+
+    :param index_data_map: A dict whose keys are the integer indices of the dataset elements and the values
+        the corresponding dictionaries containing all the relevant data about those elements. The format
+        of this data structure should be exactly as returned by the "load_visual_graph_dataset" function.
+    :param insert_empty_importances: boolean flag, if true empty (zero) numpy arrays will be inserted into
+        each graph dict for the "node_importances" and "edge_importances" field.
+    :param importance_channels: The integer number of importance channels to be used for the insertion of
+        the zero importance arrays.
+
+    :returns: A tuple of two lists.
+    """
+    dataset_length = len(index_data_map)
+    dataset_indices = []
+    dataset = [None for _ in range(dataset_length)]
+    for index, data in index_data_map.items():
+        g = data['metadata']['graph']
+
+        if insert_empty_importances:
+            num_nodes = len(g['node_indices'])
+            g['node_importances'] = np.zeros(shape=(num_nodes, importance_channels), dtype=float)
+
+            num_edges = len(g['edge_indices'])
+            g['edge_importances'] = np.zeros(shape=(num_edges, importance_channels), dtype=float)
+
+        dataset[index] = g
+        dataset_indices.append(index)
+
+    return dataset_indices, dataset
+
+
 def process_graph_dataset(dataset: t.List[dict],
                           test_indices: t.Optional[t.List[int]] = None,
                           train_indices: t.Optional[List[int]] = None,
                           use_importances: bool = True,
                           use_graph_attributes: bool = False,
                           ) -> t.Tuple[tuple, tuple, tuple, tuple]:
     """
```

### Comparing `graph_attention_student-0.7.2/graph_attention_student/examples/__pycache__/vgd_multitask_gnn.cpython-310.pyc` & `graph_attention_student-0.9.0/graph_attention_student/examples/__pycache__/vgd_multitask_gnn.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.2/graph_attention_student/examples/__pycache__/vgd_multitask_megan.cpython-310.pyc` & `graph_attention_student-0.9.0/graph_attention_student/examples/__pycache__/vgd_multitask_megan.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.2/graph_attention_student/examples/gnes_example.py` & `graph_attention_student-0.9.0/graph_attention_student/examples/gnes_example.py`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.2/graph_attention_student/examples/gnnx_example.py` & `graph_attention_student-0.9.0/graph_attention_student/examples/gnnx_example.py`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.2/graph_attention_student/examples/smiles_example.py` & `graph_attention_student-0.9.0/graph_attention_student/examples/smiles_example.py`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.2/graph_attention_student/examples/vgd_multitask_gnn.py` & `graph_attention_student-0.9.0/graph_attention_student/examples/vgd_multitask_gnn.py`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.2/graph_attention_student/examples/vgd_multitask_gnn_gatv2.py` & `graph_attention_student-0.9.0/graph_attention_student/examples/vgd_multitask_gnn_gatv2.py`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.2/graph_attention_student/examples/vgd_multitask_gnn_gin.py` & `graph_attention_student-0.9.0/graph_attention_student/examples/vgd_multitask_gnn_gin.py`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.2/graph_attention_student/examples/vgd_multitask_megan.py` & `graph_attention_student-0.9.0/graph_attention_student/examples/vgd_multitask_megan.py`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.2/graph_attention_student/examples/vgd_multitask_megan_tadf.py` & `graph_attention_student-0.9.0/graph_attention_student/examples/vgd_multitask_megan_tadf.py`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.2/graph_attention_student/experiments/README.rst` & `graph_attention_student-0.9.0/graph_attention_student/experiments/README.rst`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.2/graph_attention_student/experiments/__pycache__/vgd_classification.cpython-310.pyc` & `graph_attention_student-0.9.0/graph_attention_student/experiments/__pycache__/vgd_classification.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.2/graph_attention_student/experiments/__pycache__/vgd_regression_supervised.cpython-310.pyc` & `graph_attention_student-0.9.0/graph_attention_student/experiments/__pycache__/vgd_regression_supervised.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.2/graph_attention_student/experiments/__pycache__/vgd_single.cpython-310.pyc` & `graph_attention_student-0.9.0/graph_attention_student/experiments/__pycache__/vgd_single.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.2/graph_attention_student/experiments/__pycache__/vgd_single_gnnx.cpython-310.pyc` & `graph_attention_student-0.9.0/graph_attention_student/experiments/__pycache__/vgd_single_gnnx.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.2/graph_attention_student/experiments/__pycache__/vgd_single_gnnx_aqsoldb.cpython-310.pyc` & `graph_attention_student-0.9.0/graph_attention_student/experiments/__pycache__/vgd_single_gnnx_aqsoldb.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.2/graph_attention_student/experiments/__pycache__/vgd_single_megan.cpython-310.pyc` & `graph_attention_student-0.9.0/graph_attention_student/experiments/__pycache__/vgd_single_megan.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.2/graph_attention_student/experiments/__pycache__/vgd_single_megan_aqsoldb.cpython-310.pyc` & `graph_attention_student-0.9.0/graph_attention_student/experiments/__pycache__/vgd_single_megan_aqsoldb.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.2/graph_attention_student/experiments/process_aqsoldb.py` & `graph_attention_student-0.9.0/graph_attention_student/experiments/process_aqsoldb.py`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.2/graph_attention_student/experiments/rb_motifs_multi.py` & `graph_attention_student-0.9.0/graph_attention_student/experiments/rb_motifs_multi.py`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.2/graph_attention_student/experiments/rb_motifs_single.py` & `graph_attention_student-0.9.0/graph_attention_student/experiments/rb_motifs_single.py`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.2/graph_attention_student/experiments/vgd_classification.py` & `graph_attention_student-0.9.0/graph_attention_student/experiments/vgd_classification.py`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.2/graph_attention_student/experiments/vgd_classification_megan.py` & `graph_attention_student-0.9.0/graph_attention_student/experiments/vgd_classification_megan.py`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.2/graph_attention_student/experiments/vgd_regression_posthoc.py` & `graph_attention_student-0.9.0/graph_attention_student/experiments/vgd_regression_posthoc.py`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.2/graph_attention_student/experiments/vgd_regression_supervised.py` & `graph_attention_student-0.9.0/graph_attention_student/experiments/vgd_regression_supervised.py`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.2/graph_attention_student/experiments/vgd_regression_supervised_multi.py` & `graph_attention_student-0.9.0/graph_attention_student/experiments/vgd_regression_supervised_multi.py`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.2/graph_attention_student/experiments/vgd_regression_supervised_single.py` & `graph_attention_student-0.9.0/graph_attention_student/experiments/vgd_regression_supervised_single.py`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.2/graph_attention_student/experiments/vgd_single.py` & `graph_attention_student-0.9.0/graph_attention_student/experiments/vgd_single.py`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.2/graph_attention_student/experiments/vgd_single_gnnx.py` & `graph_attention_student-0.9.0/graph_attention_student/experiments/vgd_single_gnnx.py`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.2/graph_attention_student/experiments/vgd_single_gnnx_aqsoldb.py` & `graph_attention_student-0.9.0/graph_attention_student/experiments/vgd_single_gnnx_aqsoldb.py`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.2/graph_attention_student/experiments/vgd_single_gnnx_aqsoldb_dmpnn.py` & `graph_attention_student-0.9.0/graph_attention_student/experiments/vgd_single_gnnx_aqsoldb_dmpnn.py`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.2/graph_attention_student/experiments/vgd_single_gnnx_aqsoldb_gatv2.py` & `graph_attention_student-0.9.0/graph_attention_student/experiments/vgd_single_gnnx_aqsoldb_gatv2.py`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.2/graph_attention_student/experiments/vgd_single_gnnx_aqsoldb_painn.py` & `graph_attention_student-0.9.0/graph_attention_student/experiments/vgd_single_gnnx_aqsoldb_painn.py`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.2/graph_attention_student/experiments/vgd_single_megan.py` & `graph_attention_student-0.9.0/graph_attention_student/experiments/vgd_single_megan.py`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.2/graph_attention_student/experiments/vgd_single_megan_aqsoldb.py` & `graph_attention_student-0.9.0/graph_attention_student/experiments/vgd_single_megan_aqsoldb.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 # == MODEL PARAMETERS ==
 UNITS = [64, 64, 64]
 DROPOUT_RATE = 0.3
 FINAL_UNITS = [64, 32, 1]
 REGRESSION_LIMITS = None
 REGRESSION_REFERENCE = [-1.0]
-REGRESSION_WEIGHTS = [[1.0, 1.0]]
+REGRESSION_WEIGHTS = [[1.0, 2.0]]
 IMPORTANCE_CHANNELS: int = 2
 IMPORTANCE_FACTOR = 1.0
 IMPORTANCE_MULTIPLIER = 1.0
 SPARSITY_FACTOR = 3.0
 CONCAT_HEADS = False
 
 # == TRAINING PARAMETERS ==
```

### Comparing `graph_attention_student-0.7.2/graph_attention_student/keras.py` & `graph_attention_student-0.9.0/graph_attention_student/keras.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,14 +8,16 @@
     import tensorflow.keras as ks
     from graph.attention_student.keras import CUSTOM_OBJECTS
 
     with ks.util.custom_object_scope(CUSTOM_OBJECTS):
         model = ks.models.load_model('model/path')
 
 """
+from graph_attention_student.models.megan import Megan
 from graph_attention_student.training import NoLoss
 from graph_attention_student.training import ExplanationLoss
 
 CUSTOM_OBJECTS = {
+    'Megan': Megan,
     'NoLoss': NoLoss,
     'ExplanationLoss': ExplanationLoss
 }
```

### Comparing `graph_attention_student-0.7.2/graph_attention_student/layers.py` & `graph_attention_student-0.9.0/graph_attention_student/layers.py`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.2/graph_attention_student/models/__pycache__/gnes.cpython-310.pyc` & `graph_attention_student-0.9.0/graph_attention_student/models/__pycache__/gnes.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.2/graph_attention_student/models/__pycache__/gnnx.cpython-310.pyc` & `graph_attention_student-0.9.0/graph_attention_student/models/__pycache__/gnnx.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.2/graph_attention_student/models/__pycache__/gradient.cpython-310.pyc` & `graph_attention_student-0.9.0/graph_attention_student/models/__pycache__/gradient.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.2/graph_attention_student/models/__pycache__/megan.cpython-310.pyc` & `graph_attention_student-0.9.0/graph_attention_student/models/__pycache__/megan.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr 27 12:08:10 2023 UTC, .py size: 29552 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,970 +1,1020 @@
-00000000: 6f0d 0d0a 0000 0000 aa65 4a64 7073 0000  o........eJdps..
+00000000: 6f0d 0d0a 0000 0000 5a96 4f64 3276 0000  o.......Z.Od2v..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 dc00 0000 6400  .....@...s....d.
+00000020: 0004 0000 0040 0000 0073 f400 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 5a03 6400  d.l.Z.d.d.l.Z.d.
-00000040: 6401 6c04 6d05 5a06 0100 6400 6402 6c07  d.l.m.Z...d.d.l.
-00000050: 6d08 5a08 0100 6400 6403 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
-00000060: 0100 6400 6404 6c0b 6d0c 5a0c 0100 6400  ..d.d.l.m.Z...d.
-00000070: 6405 6c0b 6d0d 5a0d 6d0e 5a0e 0100 6400  d.l.m.Z.m.Z...d.
-00000080: 6406 6c0b 6d0f 5a0f 6d10 5a10 6d11 5a11  d.l.m.Z.m.Z.m.Z.
-00000090: 0100 6400 6407 6c12 6d13 5a13 0100 6400  ..d.d.l.m.Z...d.
-000000a0: 6408 6c12 6d14 5a14 0100 6400 6409 6c12  d.l.m.Z...d.d.l.
-000000b0: 6d15 5a15 0100 6400 640a 6c16 6d17 5a17  m.Z...d.d.l.m.Z.
-000000c0: 0100 6400 640b 6c16 6d18 5a18 0100 6400  ..d.d.l.m.Z...d.
-000000d0: 640c 6c19 6d1a 5a1a 0100 6400 640d 6c19  d.l.m.Z...d.d.l.
-000000e0: 6d1b 5a1b 0100 6400 640e 6c19 6d1c 5a1c  m.Z...d.d.l.m.Z.
-000000f0: 0100 4700 640f 6410 8400 6410 6506 6a1d  ..G.d.d...d.e.j.
-00000100: 6a1e 8303 5a1f 6401 5300 2911 e900 0000  j...Z.d.S.).....
-00000110: 004e 2901 da0d 636f 6d70 696c 655f 7574  .N)...compile_ut
-00000120: 696c 7329 01da 1f72 6167 6765 645f 7465  ils)...ragged_te
-00000130: 6e73 6f72 5f66 726f 6d5f 6e65 7374 6564  nsor_from_nested
-00000140: 5f6e 756d 7079 2901 da0e 4772 6170 6842  _numpy)...GraphB
-00000150: 6173 654c 6179 6572 2902 da0f 4c61 7a79  aseLayer)...Lazy
-00000160: 436f 6e63 6174 656e 6174 65da 0b4c 617a  Concatenate..Laz
-00000170: 7941 7665 7261 6765 2903 da0e 4465 6e73  yAverage)...Dens
-00000180: 6545 6d62 6564 6469 6e67 da13 4163 7469  eEmbedding..Acti
-00000190: 7661 7469 6f6e 456d 6265 6464 696e 67da  vationEmbedding.
-000001a0: 1044 726f 706f 7574 456d 6265 6464 696e  .DropoutEmbeddin
-000001b0: 6729 01da 1150 6f6f 6c69 6e67 4c6f 6361  g)...PoolingLoca
-000001c0: 6c45 6467 6573 2901 da0c 506f 6f6c 696e  lEdges)...Poolin
-000001d0: 674e 6f64 6573 2901 da14 506f 6f6c 696e  gNodes)...Poolin
-000001e0: 6757 6569 6768 7465 644e 6f64 6573 2901  gWeightedNodes).
-000001f0: da21 4578 706c 616e 6174 696f 6e53 7061  .!ExplanationSpa
-00000200: 7273 6974 7952 6567 756c 6172 697a 6174  rsityRegularizat
-00000210: 696f 6e29 01da 134d 756c 7469 4865 6164  ion)...MultiHead
-00000220: 4741 5456 324c 6179 6572 2901 da03 6d61  GATV2Layer)...ma
-00000230: 6529 01da 0362 6365 2901 da0f 7368 6966  e)...bce)...shif
-00000240: 7465 645f 7369 676d 6f69 6463 0000 0000  ted_sigmoidc....
-00000250: 0000 0000 0000 0000 0000 0000 3300 0000  ............3...
-00000260: 0000 0000 7388 0100 0065 005a 0164 005a  ....s....e.Z.d.Z
-00000270: 0264 015a 0364 0264 0364 0464 0367 0064  .d.Z.d.d.d.d.g.d
-00000280: 0564 0664 0464 0464 0764 0864 0464 0364  .d.d.d.d.d.d.d.d
-00000290: 0964 0a67 0164 0464 0b64 0c64 0864 0864  .d.g.d.d.d.d.d.d
-000002a0: 0864 0864 0364 0966 1864 0d65 046a 0565  .d.d.d.f.d.e.j.e
-000002b0: 0619 0064 0e65 0764 0f65 0864 1065 0964  ...d.e.d.e.d.e.d
-000002c0: 1165 0864 1265 046a 0565 0619 0064 1365  .e.d.e.j.e...d.e
-000002d0: 0664 1465 0764 1565 0964 1665 0964 1765  .d.e.d.e.d.e.d.e
-000002e0: 0964 1865 046a 0a65 046a 0565 0b6a 0c6a  .d.e.j.e.j.e.j.j
-000002f0: 0d19 0019 0064 1965 0964 1a65 0864 1b65  .....d.e.d.e.d.e
-00000300: 0864 1c65 046a 0565 0619 0064 1d65 0964  .d.e.j.e...d.e.d
-00000310: 1e65 0764 1f65 0764 2065 046a 0a65 046a  .e.d.e.d e.j.e.j
-00000320: 0e65 0965 0966 0219 0019 0064 2165 046a  .e.e.f.....d!e.j
-00000330: 0a65 046a 0e65 0965 0966 0219 0019 0064  .e.j.e.e.f.....d
-00000340: 2265 046a 0a65 046a 0565 046a 0e65 0965  "e.j.e.j.e.j.e.e
-00000350: 0966 0219 0019 0019 0064 2365 046a 0a65  .f.......d#e.j.e
-00000360: 0919 0064 2465 0864 2565 0866 3264 2664  ...d$e.d%e.f2d&d
-00000370: 2784 055a 0f87 0066 0164 2864 2984 085a  '..Z...f.d(d)..Z
-00000380: 1065 1164 2a65 0866 0264 2b64 2c84 0483  .e.d*e.f.d+d,...
-00000390: 015a 1264 2a65 0866 0264 2d64 2e84 045a  .Z.d*e.f.d-d...Z
-000003a0: 1309 0909 0909 0864 3a64 2f65 0864 2465  .......d:d/e.d$e
-000003b0: 0864 3065 046a 0a65 146a 1519 0066 0664  .d0e.j.e.j...f.d
-000003c0: 3164 3284 055a 1664 3364 3484 005a 1709  1d2..Z.d3d4..Z..
-000003d0: 0364 3b64 3565 0866 0264 3664 3784 055a  .d;d5e.f.d6d7..Z
-000003e0: 1864 3864 3984 005a 1987 0004 005a 1a53  .d8d9..Z.....Z.S
-000003f0: 0029 3cda 054d 6567 616e 613c 0200 000a  .)<..Megana<....
-00000400: 2020 2020 4d45 4741 4e3a 204d 756c 7469      MEGAN: Multi
-00000410: 2045 7870 6c61 6e61 7469 6f6e 2047 7261   Explanation Gra
-00000420: 7068 2041 7474 656e 7469 6f6e 204e 6574  ph Attention Net
-00000430: 776f 726b 0a20 2020 2054 6869 7320 6d6f  work.    This mo
-00000440: 6465 6c20 6375 7272 656e 746c 7920 7375  del currently su
-00000450: 7070 6f72 7473 2067 7261 7068 2072 6567  pports graph reg
-00000460: 7265 7373 696f 6e20 616e 6420 6772 6170  ression and grap
-00000470: 6820 636c 6173 7369 6669 6361 7469 6f6e  h classification
-00000480: 2070 726f 626c 656d 732e 2049 7420 7761   problems. It wa
-00000490: 7320 6d61 696e 6c79 2064 6573 6967 6e65  s mainly designe
-000004a0: 640a 2020 2020 7769 7468 2061 2066 6f63  d.    with a foc
-000004b0: 7573 206f 6e20 6578 706c 6169 6e61 626c  us on explainabl
-000004c0: 6520 4149 2028 5841 4929 2e20 416c 6f6e  e AI (XAI). Alon
-000004d0: 6720 7468 6520 6d61 696e 2070 7265 6469  g the main predi
-000004e0: 6374 696f 6e2c 2074 6869 7320 6d6f 6465  ction, this mode
-000004f0: 6c20 6973 2061 626c 6520 746f 206f 7574  l is able to out
-00000500: 7075 7420 6d75 6c74 6970 6c65 0a20 2020  put multiple.   
-00000510: 2061 7474 656e 7469 6f6e 2d62 6173 6564   attention-based
-00000520: 2065 7870 6c61 6e61 7469 6f6e 7320 666f   explanations fo
-00000530: 7220 7468 6174 2070 7265 6469 6374 696f  r that predictio
-00000540: 6e2e 204d 6f72 6520 7370 6563 6966 6963  n. More specific
-00000550: 616c 6c79 2c20 7468 6520 6d6f 6465 6c20  ally, the model 
-00000560: 6f75 7470 7574 7320 6e6f 6465 2061 6e64  outputs node and
-00000570: 2065 6467 650a 2020 2020 6174 7472 6962   edge.    attrib
-00000580: 7574 696f 6e61 6c20 6578 706c 616e 6174  utional explanat
-00000590: 696f 6e73 2028 6173 7369 676e 696e 6720  ions (assigning 
-000005a0: 5b30 2c20 315d 2076 616c 7565 7320 746f  [0, 1] values to
-000005b0: 2065 7665 7220 6e6f 6465 202f 2065 6467   ever node / edg
-000005c0: 6520 6f66 2074 6865 2069 6e70 7574 2067  e of the input g
-000005d0: 7261 7068 2920 696e 204b 0a20 2020 2073  raph) in K.    s
-000005e0: 6570 6172 6174 6520 6578 706c 616e 6174  eparate explanat
-000005f0: 696f 6e20 6368 616e 6e65 6c73 2c20 7768  ion channels, wh
-00000600: 6572 6520 4b20 6361 6e20 6265 2063 686f  ere K can be cho
-00000610: 7365 6e20 6173 2061 6e20 696e 6465 7065  sen as an indepe
-00000620: 6e64 656e 7420 6d6f 6465 6c20 7061 7261  ndent model para
-00000630: 6d65 7465 722e 0a20 2020 20fa 106b 6763  meter..    ..kgc
-00000640: 6e6e 3e6c 6561 6b79 5f72 656c 7554 e700  nn>leaky_reluT..
-00000650: 0000 0000 0000 00e9 0200 0000 da07 7369  ..............si
-00000660: 676d 6f69 6467 0000 0000 0000 2440 4e46  gmoidg......$@NF
-00000670: e901 0000 00da 066c 696e 6561 72da 0373  .......linear..s
-00000680: 756d da05 756e 6974 73da 0a61 6374 6976  um..units..activ
-00000690: 6174 696f 6eda 0875 7365 5f62 6961 73da  ation..use_bias.
-000006a0: 0c64 726f 706f 7574 5f72 6174 65da 1175  .dropout_rate..u
-000006b0: 7365 5f65 6467 655f 6665 6174 7572 6573  se_edge_features
-000006c0: da10 696d 706f 7274 616e 6365 5f75 6e69  ..importance_uni
-000006d0: 7473 da13 696d 706f 7274 616e 6365 5f63  ts..importance_c
-000006e0: 6861 6e6e 656c 73da 1569 6d70 6f72 7461  hannels..importa
-000006f0: 6e63 655f 6163 7469 7661 7469 6f6e da17  nce_activation..
-00000700: 696d 706f 7274 616e 6365 5f64 726f 706f  importance_dropo
-00000710: 7574 5f72 6174 65da 1169 6d70 6f72 7461  ut_rate..importa
-00000720: 6e63 655f 6661 6374 6f72 da15 696d 706f  nce_factor..impo
-00000730: 7274 616e 6365 5f6d 756c 7469 706c 6965  rtance_multiplie
-00000740: 72da 1a69 6d70 6f72 7461 6e63 655f 7472  r..importance_tr
-00000750: 616e 7366 6f72 6d61 7469 6f6e 73da 0f73  ansformations..s
-00000760: 7061 7273 6974 795f 6661 6374 6f72 da0c  parsity_factor..
-00000770: 636f 6e63 6174 5f68 6561 6473 da19 7365  concat_heads..se
-00000780: 7061 7261 7465 5f65 7870 6c61 6e61 7469  parate_explanati
-00000790: 6f6e 5f73 7465 70da 0b66 696e 616c 5f75  on_step..final_u
-000007a0: 6e69 7473 da12 6669 6e61 6c5f 6472 6f70  nits..final_drop
-000007b0: 6f75 745f 7261 7465 da10 6669 6e61 6c5f  out_rate..final_
-000007c0: 6163 7469 7661 7469 6f6e da0d 6669 6e61  activation..fina
-000007d0: 6c5f 706f 6f6c 696e 67da 1172 6567 7265  l_pooling..regre
-000007e0: 7373 696f 6e5f 6c69 6d69 7473 da12 7265  ssion_limits..re
-000007f0: 6772 6573 7369 6f6e 5f77 6569 6768 7473  gression_weights
-00000800: da0f 7265 6772 6573 7369 6f6e 5f62 696e  ..regression_bin
-00000810: 73da 1472 6567 7265 7373 696f 6e5f 7265  s..regression_re
-00000820: 6665 7265 6e63 65da 1272 6574 7572 6e5f  ference..return_
-00000830: 696d 706f 7274 616e 6365 73da 1475 7365  importances..use
-00000840: 5f67 7261 7068 5f61 7474 7269 6275 7465  _graph_attribute
-00000850: 7363 1a00 0000 0000 0000 0000 0000 2100  sc............!.
-00000860: 0000 0a00 0000 4b00 0000 7362 0300 0074  ......K...sb...t
-00000870: 006a 016a 026a 037c 0066 0169 007c 1aa4  .j.j.j.|.f.i.|..
-00000880: 018e 0101 007c 017c 005f 047c 027c 005f  .....|.|._.|.|._
-00000890: 057c 037c 005f 067c 047c 005f 077c 057c  .|.|._.|.|._.|.|
-000008a0: 005f 087c 067c 005f 097c 077c 005f 0a7c  ._.|.|._.|.|._.|
-000008b0: 087c 005f 0b7c 097c 005f 0c7c 0a7c 005f  .|._.|.|._.|.|._
-000008c0: 0d7c 0b7c 005f 0e7c 0c7c 005f 0f7c 0d7c  .|.|._.|.|._.|.|
-000008d0: 005f 107c 0e7c 005f 117c 107c 005f 127c  ._.|.|._.|.|._.|
-000008e0: 117c 005f 137c 127c 005f 147c 137c 005f  .|._.|.|._.|.|._
-000008f0: 157c 147c 005f 167c 157c 005f 177c 177c  .|.|._.|.|._.|.|
-00000900: 005f 187c 167c 005f 197c 187c 005f 1a7c  ._.|.|._.|.|._.|
-00000910: 0f7c 005f 1b7c 197c 005f 1c67 007c 005f  .|._.|.|._.g.|._
-00000920: 1d7c 006a 0444 005d 187d 1b74 1e7c 1b7c  .|.j.D.].}.t.|.|
-00000930: 006a 0a7c 006a 087c 006a 057c 006a 0664  .j.|.j.|.j.|.j.d
-00000940: 017c 006a 1164 028d 077d 1c7c 006a 1da0  .|.j.d...}.|.j..
-00000950: 1f7c 1ca1 0101 0071 5c74 207c 006a 0764  .|.....q\t |.j.d
-00000960: 038d 017c 005f 2174 227c 006a 1064 048d  ...|._!t"|.j.d..
-00000970: 017c 005f 2374 247c 006a 0b64 058d 017c  .|._#t$|.j.d...|
-00000980: 005f 2574 2664 0664 078d 017c 005f 2774  ._%t&d.d...|._'t
-00000990: 2864 0864 0964 0a8d 027c 005f 2974 2864  (d.d.d...|._)t(d
-000009a0: 0864 0b64 0a8d 027c 005f 2a74 2b83 007c  .d.d...|._*t+..|
-000009b0: 005f 2c7c 067c 006a 0a67 0117 007c 005f  ._,|.|.j.g...|._
-000009c0: 2d64 0c64 0d84 007c 0644 0083 0164 0e67  -d.d...|.D...d.g
-000009d0: 0117 007c 005f 2e67 007c 005f 2f74 307c  ...|._.g.|._/t0|
-000009e0: 006a 2d7c 006a 2e83 0244 005d 115c 027d  .j-|.j...D.].\.}
-000009f0: 1b7d 1d74 317c 1b7c 1d7c 0364 0f8d 037d  .}.t1|.|.|.d...}
-00000a00: 1c7c 006a 2fa0 1f7c 1ca1 0101 0071 be74  .|.j/..|.....q.t
-00000a10: 327c 006a 1564 108d 017c 005f 3374 2664  2|.j.d...|._3t&d
-00000a20: 0664 078d 017c 005f 3474 207c 006a 1364  .d...|._4t |.j.d
-00000a30: 038d 017c 005f 3564 1164 0d84 007c 006a  ...|._5d.d...|.j
-00000a40: 1244 0083 017c 005f 367c 006a 147c 006a  .D...|._6|.j.|.j
-00000a50: 3664 063c 0064 1264 0d84 007c 006a 1244  6d.<.d.d...|.j.D
-00000a60: 0083 017c 005f 3764 017c 006a 3764 063c  ...|._7d.|.j7d.<
-00000a70: 0067 007c 005f 3874 307c 006a 127c 006a  .g.|._8t0|.j.|.j
-00000a80: 367c 006a 3783 0344 005d 135c 037d 1b7d  6|.j7..D.].\.}.}
-00000a90: 1d7d 1e74 317c 1b7c 1d7c 0364 0f8d 037d  .}.t1|.|.|.d...}
-00000aa0: 1c7c 006a 38a0 1f7c 1ca1 0101 0090 0171  .|.j8..|.......q
-00000ab0: 0d74 006a 39a0 3aa1 007c 005f 3b74 3ca0  .t.j9.:..|._;t<.
-00000ac0: 3d74 3ea1 017c 005f 3f74 006a 39a0 40a1  =t>..|._?t.j9.@.
-00000ad0: 007c 005f 4174 006a 39a0 42a1 007c 005f  .|._At.j9.B..|._
-00000ae0: 4374 3ca0 3d74 44a1 017c 005f 457c 006a  Ct<.=tD..|._E|.j
-00000af0: 1864 1375 0190 0172 ad74 467c 1774 4774  .d.u...r.tF|.tGt
-00000b00: 4866 0283 0290 0172 517c 1767 017c 005f  Hf.....rQ|.g.|._
-00000b10: 1874 497c 006a 1883 017d 1f7c 006a 1764  .tI|.j...}.|.j.d
-00000b20: 1375 0190 0172 6274 497c 006a 1783 017d  .u...rbtI|.j...}
-00000b30: 206e 157c 006a 1664 1375 0190 0172 6e74   n.|.j.d.u...rnt
-00000b40: 497c 006a 1683 017d 206e 0974 4a64 147c  I|.j...} n.tJd.|
-00000b50: 006a 189b 0064 159d 0383 0182 017c 1f64  .j...d.......|.d
-00000b60: 1614 007c 076b 0290 0173 894a 0064 177c  ...|.k...s.J.d.|
-00000b70: 1f9b 0064 187c 079b 0064 199d 0583 0182  ...d.|...d......
-00000b80: 017c 1f7c 1064 0619 006b 0290 0173 9d4a  .|.|.d...k...s.J
-00000b90: 0064 1a7c 1f9b 0064 1b7c 1064 0619 009b  .d.|...d.|.d....
-00000ba0: 0064 1c9d 0583 0182 017c 1f7c 206b 0290  .d.......|.| k..
-00000bb0: 0173 af4a 0064 1a7c 1f9b 0064 1d7c 209b  .s.J.d.|...d.| .
-00000bc0: 0064 1c9d 0583 0182 0164 1353 0064 1353  .d.......d.S.d.S
-00000bd0: 0029 1e61 250f 0000 0a20 2020 2020 2020  .).a%....       
-00000be0: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
-00000bf0: 2020 2075 6e69 7473 3a20 4120 6c69 7374     units: A list
-00000c00: 206f 6620 696e 7473 2077 6865 7265 2065   of ints where e
-00000c10: 6163 6820 656c 656d 656e 7420 636f 6e66  ach element conf
-00000c20: 6967 7572 6573 2061 6e20 6164 6469 7469  igures an additi
-00000c30: 6f6e 616c 2061 7474 656e 7469 6f6e 206c  onal attention l
-00000c40: 6179 6572 2e20 5468 6520 6e75 6d65 7269  ayer. The numeri
-00000c50: 630a 2020 2020 2020 2020 2020 2020 2020  c.              
-00000c60: 2020 7661 6c75 6520 6465 7465 726d 696e    value determin
-00000c70: 6573 2074 6865 206e 756d 6265 7220 6f66  es the number of
-00000c80: 2068 6964 6465 6e20 756e 6974 7320 746f   hidden units to
-00000c90: 2062 6520 7573 6564 2069 6e20 7468 6520   be used in the 
-00000ca0: 6174 7465 6e74 696f 6e20 6865 6164 7320  attention heads 
-00000cb0: 6f66 2074 6861 7420 6c61 7965 720a 2020  of that layer.  
-00000cc0: 2020 2020 2020 2020 2020 6163 7469 7661            activa
-00000cd0: 7469 6f6e 3a20 5468 6520 6163 7469 7661  tion: The activa
-00000ce0: 7469 6f6e 2066 756e 6374 696f 6e20 746f  tion function to
-00000cf0: 2062 6520 7573 6564 2077 6974 6869 6e20   be used within 
-00000d00: 7468 6520 6174 7465 6e74 696f 6e20 6c61  the attention la
-00000d10: 7965 7273 206f 6620 7468 6520 6e65 7477  yers of the netw
-00000d20: 6f72 6b0a 2020 2020 2020 2020 2020 2020  ork.            
-00000d30: 7573 655f 6269 6173 3a20 5768 6574 6865  use_bias: Whethe
-00000d40: 7220 7468 6520 6c61 7965 7273 206f 6620  r the layers of 
-00000d50: 7468 6520 6e65 7477 6f72 6b20 7368 6f75  the network shou
-00000d60: 6c64 2075 7365 2062 6961 7320 7765 6967  ld use bias weig
-00000d70: 6874 7320 6174 2061 6c6c 0a20 2020 2020  hts at all.     
-00000d80: 2020 2020 2020 2064 726f 706f 7574 5f72         dropout_r
-00000d90: 6174 653a 2054 6865 2064 726f 706f 7574  ate: The dropout
-00000da0: 2072 6174 6520 746f 2062 6520 6170 706c   rate to be appl
-00000db0: 6965 6420 6166 7465 7220 2a65 6163 682a  ied after *each*
-00000dc0: 206f 6620 7468 6520 6174 7465 6e74 696f   of the attentio
-00000dd0: 6e20 6c61 7965 7273 206f 6620 7468 6520  n layers of the 
-00000de0: 6e65 7477 6f72 6b2e 0a20 2020 2020 2020  network..       
-00000df0: 2020 2020 2075 7365 5f65 6467 655f 6665       use_edge_fe
-00000e00: 6174 7572 6573 3a20 5768 6574 6865 7220  atures: Whether 
-00000e10: 6564 6765 2066 6561 7475 7265 7320 7368  edge features sh
-00000e20: 6f75 6c64 2062 6520 7573 6564 2e20 4765  ould be used. Ge
-00000e30: 6e65 7261 6c6c 7920 7468 6520 6e65 7477  nerally the netw
-00000e40: 6f72 6b20 7375 7070 6f72 7473 2074 6865  ork supports the
-00000e50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000e60: 2075 7361 6765 206f 6620 6564 6765 2066   usage of edge f
-00000e70: 6561 7475 7265 732c 2062 7574 2069 6620  eatures, but if 
-00000e80: 7468 6520 696e 7075 7420 6461 7461 2064  the input data d
-00000e90: 6f65 7320 6e6f 7420 636f 6e74 6169 6e20  oes not contain 
-00000ea0: 6564 6765 2066 6561 7475 7265 732c 2074  edge features, t
-00000eb0: 6869 7320 7368 6f75 6c64 2062 650a 2020  his should be.  
-00000ec0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00000ed0: 7420 746f 2046 616c 7365 2e0a 2020 2020  t to False..    
-00000ee0: 2020 2020 2020 2020 696d 706f 7274 616e          importan
-00000ef0: 6365 5f75 6e69 7473 3a20 4120 6c69 7374  ce_units: A list
-00000f00: 206f 6620 696e 7473 2077 6865 7265 2065   of ints where e
-00000f10: 6163 6820 656c 656d 656e 7420 636f 6e66  ach element conf
-00000f20: 6967 7572 6573 2061 6e6f 7468 6572 2064  igures another d
-00000f30: 656e 7365 206c 6179 6572 2069 6e20 7468  ense layer in th
-00000f40: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-00000f50: 2020 7375 626e 6574 776f 726b 2074 6861    subnetwork tha
-00000f60: 7420 7072 6f64 7563 6573 2074 6865 206e  t produces the n
-00000f70: 6f64 6520 696d 706f 7274 616e 6365 2074  ode importance t
-00000f80: 656e 736f 7220 6672 6f6d 2074 6865 206d  ensor from the m
-00000f90: 6169 6e20 6e6f 6465 2065 6d62 6564 6469  ain node embeddi
-00000fa0: 6e67 732e 2054 6865 0a20 2020 2020 2020  ngs. The.       
-00000fb0: 2020 2020 2020 2020 206e 756d 6572 6963           numeric
-00000fc0: 2076 616c 7565 2064 6574 6572 6d69 6e65   value determine
-00000fd0: 7320 7468 6520 6e75 6d62 6572 206f 6620  s the number of 
-00000fe0: 6869 6464 656e 2075 6e69 7473 2069 6e20  hidden units in 
-00000ff0: 7468 6174 206c 6179 6572 2e0a 2020 2020  that layer..    
-00001000: 2020 2020 2020 2020 696d 706f 7274 616e          importan
-00001010: 6365 5f63 6861 6e6e 656c 733a 2054 6865  ce_channels: The
-00001020: 2069 6e74 206e 756d 6265 7220 6f66 2065   int number of e
-00001030: 7870 6c61 6e61 7469 6f6e 2063 6861 6e6e  xplanation chann
-00001040: 656c 7320 746f 2062 6520 7072 6f64 7563  els to be produc
-00001050: 6564 2062 7920 7468 6520 6e65 7477 6f72  ed by the networ
-00001060: 6b2e 2054 6869 730a 2020 2020 2020 2020  k. This.        
-00001070: 2020 2020 2020 2020 6973 2074 6865 2076          is the v
-00001080: 616c 7565 2072 6566 6572 7265 6420 746f  alue referred to
-00001090: 2061 7320 224b 222e 204e 6f74 6520 7468   as "K". Note th
-000010a0: 6174 2074 6869 7320 7769 6c6c 2061 6c73  at this will als
-000010b0: 6f20 6465 7465 726d 696e 6520 7468 6520  o determine the 
-000010c0: 6e75 6d62 6572 206f 6620 6174 7465 6e74  number of attent
-000010d0: 696f 6e0a 2020 2020 2020 2020 2020 2020  ion.            
-000010e0: 2020 2020 6865 6164 7320 7573 6564 2077      heads used w
-000010f0: 6974 6869 6e20 7468 6520 6174 7465 6e74  ithin the attent
-00001100: 696f 6e20 7375 626e 6574 776f 726b 2e0a  ion subnetwork..
-00001110: 2020 2020 2020 2020 2020 2020 696d 706f              impo
-00001120: 7274 616e 6365 5f66 6163 746f 723a 2054  rtance_factor: T
-00001130: 6865 2077 6569 6768 7420 6f66 2074 6865  he weight of the
-00001140: 2065 7870 6c61 6e61 7469 6f6e 2d6f 6e6c   explanation-onl
-00001150: 7920 7472 6169 6e20 7374 6570 2e20 4966  y train step. If
-00001160: 2074 6869 7320 6973 2073 6574 2074 6f20   this is set to 
-00001170: 6578 6163 746c 790a 2020 2020 2020 2020  exactly.        
-00001180: 2020 2020 2020 2020 7a65 726f 2074 6865          zero the
-00001190: 6e20 7468 6520 6578 706c 616e 6174 696f  n the explanatio
-000011a0: 6e20 7472 6169 6e20 7374 6570 2077 696c  n train step wil
-000011b0: 6c20 6e6f 7420 6265 2065 7865 6375 7465  l not be execute
-000011c0: 6420 6174 2061 6c6c 2028 6c65 7373 2063  d at all (less c
-000011d0: 6f6d 7075 7461 7469 6f6e 616c 6c79 0a20  omputationally. 
-000011e0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-000011f0: 7870 656e 7369 7665 290a 2020 2020 2020  xpensive).      
-00001200: 2020 2020 2020 696d 706f 7274 616e 6365        importance
-00001210: 5f6d 756c 7469 706c 6965 723a 2041 6e20  _multiplier: An 
-00001220: 6164 6469 7469 6f6e 616c 2068 7970 6572  additional hyper
-00001230: 7061 7261 6d65 7465 7220 6f66 2074 6865  parameter of the
-00001240: 2065 7870 6c61 6e61 7469 6f6e 2d6f 6e6c   explanation-onl
-00001250: 7920 7472 6169 6e20 7374 6570 2e20 5468  y train step. Th
-00001260: 6973 0a20 2020 2020 2020 2020 2020 2020  is.             
-00001270: 2020 2069 7320 6573 7365 6e74 6961 6c6c     is essentiall
-00001280: 7920 7468 6520 7363 616c 696e 6720 6661  y the scaling fa
-00001290: 6374 6f72 2074 6861 7420 6973 2061 7070  ctor that is app
-000012a0: 6c69 6564 2074 6f20 7468 6520 7661 6c75  lied to the valu
-000012b0: 6573 206f 6620 7468 6520 6461 7461 7365  es of the datase
-000012c0: 7420 7375 6368 2074 6861 740a 2020 2020  t such that.    
-000012d0: 2020 2020 2020 2020 2020 2020 7468 6520              the 
-000012e0: 7461 7267 6574 2076 616c 7565 7320 6361  target values ca
-000012f0: 6e20 7265 6173 6f6e 6162 6c79 2062 6520  n reasonably be 
-00001300: 6170 7072 6f78 696d 6174 6564 2062 7920  approximated by 
-00001310: 6120 7375 6d20 6f66 205b 302c 2031 5d20  a sum of [0, 1] 
-00001320: 696d 706f 7274 616e 6365 2076 616c 7565  importance value
-00001330: 732e 0a20 2020 2020 2020 2020 2020 2073  s..            s
-00001340: 7061 7273 6974 795f 6661 6374 6f72 3a20  parsity_factor: 
-00001350: 5468 6520 636f 6566 6669 6369 656e 7420  The coefficient 
-00001360: 666f 7220 7468 6520 7370 6172 7369 7479  for the sparsity
-00001370: 2072 6567 756c 6172 697a 6174 696f 6e20   regularization 
-00001380: 6f66 2074 6865 206e 6f64 6520 696d 706f  of the node impo
-00001390: 7274 616e 6365 0a20 2020 2020 2020 2020  rtance.         
-000013a0: 2020 2020 2020 2074 656e 736f 722e 0a20         tensor.. 
-000013b0: 2020 2020 2020 2020 2020 2063 6f6e 6361             conca
-000013c0: 745f 6865 6164 733a 2057 6865 7468 6572  t_heads: Whether
-000013d0: 2074 6f20 636f 6e63 6174 2074 6865 2068   to concat the h
-000013e0: 6561 6473 206f 6620 7468 6520 6174 7465  eads of the atte
-000013f0: 6e74 696f 6e20 7375 626e 6574 776f 726b  ntion subnetwork
-00001400: 2e20 5468 6520 6465 6661 756c 7420 6973  . The default is
-00001410: 2054 7275 652e 2049 6e0a 2020 2020 2020   True. In.      
-00001420: 2020 2020 2020 2020 2020 7468 6174 2063            that c
-00001430: 6173 6520 7468 6520 6f75 7470 7574 206f  ase the output o
-00001440: 6620 6561 6368 2069 6e64 6976 6964 7561  f each individua
-00001450: 6c20 6174 7465 6e74 696f 6e20 6865 6164  l attention head
-00001460: 2069 7320 636f 6e63 6174 656e 6174 6564   is concatenated
-00001470: 2061 6e64 2074 6865 2063 6f6e 6361 7465   and the concate
-00001480: 6e61 7465 640a 2020 2020 2020 2020 2020  nated.          
-00001490: 2020 2020 2020 7665 6374 6f72 2069 7320        vector is 
-000014a0: 7468 656e 2075 7365 6420 6173 2074 6865  then used as the
-000014b0: 2069 6e70 7574 206f 6620 7468 6520 6e65   input of the ne
-000014c0: 7874 2061 7474 656e 7469 6f6e 206c 6179  xt attention lay
-000014d0: 6572 2773 2068 6561 6473 2e20 4966 2074  er's heads. If t
-000014e0: 6869 7320 6973 2046 616c 7365 2c20 7468  his is False, th
-000014f0: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-00001500: 2020 7665 6374 6f72 7320 6172 6520 6176    vectors are av
-00001510: 6572 6167 6520 706f 6f6c 6564 2069 6e73  erage pooled ins
-00001520: 7465 6164 2e0a 2020 2020 2020 2020 2020  tead..          
-00001530: 2020 6669 6e61 6c5f 756e 6974 733a 2041    final_units: A
-00001540: 206c 6973 7420 6f66 2069 6e74 7320 7768   list of ints wh
-00001550: 6572 6520 6561 6368 2065 6c65 6d65 6e74  ere each element
-00001560: 2063 6f6e 6669 6775 7265 7320 616e 6f74   configures anot
-00001570: 6865 7220 6465 6e73 6520 6c61 7965 7220  her dense layer 
-00001580: 696e 2074 6865 204d 4c50 0a20 2020 2020  in the MLP.     
-00001590: 2020 2020 2020 2020 2020 2061 7420 7468             at th
-000015a0: 6520 7461 696c 2065 6e64 206f 6620 7468  e tail end of th
-000015b0: 6520 6e65 7477 6f72 6b2e 2054 6865 206e  e network. The n
-000015c0: 756d 6572 6963 2076 616c 7565 2064 6574  umeric value det
-000015d0: 6572 6d69 6e65 7320 7468 6520 6e75 6d62  ermines the numb
-000015e0: 6572 206f 6620 7468 6520 6869 6464 656e  er of the hidden
-000015f0: 2075 6e69 7473 0a20 2020 2020 2020 2020   units.         
-00001600: 2020 2020 2020 2069 6e20 7468 6174 206c         in that l
-00001610: 6179 6572 2e20 4e6f 7465 2074 6861 7420  ayer. Note that 
-00001620: 7468 6520 6669 6e61 6c20 656c 656d 656e  the final elemen
-00001630: 7420 696e 2074 6869 7320 6c69 7374 2068  t in this list h
-00001640: 6173 2074 6f20 6265 2074 6865 2073 616d  as to be the sam
-00001650: 6520 6173 2074 6865 2064 696d 656e 7369  e as the dimensi
-00001660: 6f6e 0a20 2020 2020 2020 2020 2020 2020  on.             
-00001670: 2020 2074 6f20 6265 2065 7870 6563 7465     to be expecte
-00001680: 6420 666f 7220 7468 6520 7361 6d70 6c65  d for the sample
-00001690: 7320 6f66 2074 6865 2074 7261 696e 696e  s of the trainin
-000016a0: 6720 6461 7461 7365 7421 0a20 2020 2020  g dataset!.     
-000016b0: 2020 2020 2020 2066 696e 616c 5f64 726f         final_dro
-000016c0: 706f 7574 5f72 6174 653a 2054 6865 2064  pout_rate: The d
-000016d0: 726f 706f 7574 2072 6174 6520 746f 2062  ropout rate to b
-000016e0: 6520 6170 706c 6965 6420 6166 7465 7220  e applied after 
-000016f0: 2a65 7665 7279 2a20 6c61 7965 7220 6f66  *every* layer of
-00001700: 2074 6865 2066 696e 616c 204d 4c50 2e0a   the final MLP..
-00001710: 2020 2020 2020 2020 2020 2020 6669 6e61              fina
-00001720: 6c5f 6163 7469 7661 7469 6f6e 3a20 5468  l_activation: Th
-00001730: 6520 6163 7469 7661 7469 6f6e 2074 6f20  e activation to 
-00001740: 6265 2061 7070 6c69 6564 2061 7420 7468  be applied at th
-00001750: 6520 7665 7279 206c 6173 7420 6c61 7965  e very last laye
-00001760: 7220 6f66 2074 6865 204d 4c50 2074 6f20  r of the MLP to 
-00001770: 7072 6f64 7563 6520 7468 650a 2020 2020  produce the.    
-00001780: 2020 2020 2020 2020 2020 2020 6163 7475              actu
-00001790: 616c 206f 7574 7075 7420 6f66 2074 6865  al output of the
-000017a0: 206e 6574 776f 726b 2e0a 2020 2020 2020   network..      
-000017b0: 2020 2020 2020 6669 6e61 6c5f 706f 6f6c        final_pool
-000017c0: 696e 673a 2054 6865 2070 6f6f 6c69 6e67  ing: The pooling
-000017d0: 206d 6574 686f 6420 746f 2062 6520 7573   method to be us
-000017e0: 6564 2064 7572 696e 6720 7468 6520 676c  ed during the gl
-000017f0: 6f62 616c 2070 6f6f 6c69 6e67 2070 6861  obal pooling pha
-00001800: 7365 2069 6e20 7468 6520 6e65 7477 6f72  se in the networ
-00001810: 6b2e 0a20 2020 2020 2020 2020 2020 2072  k..            r
-00001820: 6567 7265 7373 696f 6e5f 6c69 6d69 7473  egression_limits
-00001830: 3a20 4120 7475 706c 6520 7768 6572 6520  : A tuple where 
-00001840: 7468 6520 6669 7273 7420 7661 6c75 6520  the first value 
-00001850: 6973 2074 6865 206c 6f77 6572 206c 696d  is the lower lim
-00001860: 6974 2066 6f72 2074 6865 2065 7870 6563  it for the expec
-00001870: 7465 6420 7661 6c75 6520 7261 6e67 650a  ted value range.
-00001880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001890: 6f66 2074 6865 2072 6567 7265 7373 696f  of the regressio
-000018a0: 6e20 7461 736b 2061 6e64 2074 6568 2073  n task and teh s
-000018b0: 6563 6f6e 6420 7661 6c75 6520 7468 6520  econd value the 
-000018c0: 7570 7065 7220 6c69 6d69 742e 0a20 2020  upper limit..   
-000018d0: 2020 2020 2020 2020 2072 6567 7265 7373           regress
-000018e0: 696f 6e5f 7265 6665 7265 6e63 653a 2041  ion_reference: A
-000018f0: 2072 6566 6572 656e 6365 2076 616c 7565   reference value
-00001900: 2077 6869 6368 2069 7320 696e 7369 6465   which is inside
-00001910: 2074 6865 2072 616e 6765 206f 6620 6578   the range of ex
-00001920: 7065 6374 6564 2076 616c 7565 7320 2862  pected values (b
-00001930: 6573 7420 6966 0a20 2020 2020 2020 2020  est if.         
-00001940: 2020 2020 2020 2069 7420 7761 7320 696e         it was in
-00001950: 2074 6865 206d 6964 646c 652c 2062 7574   the middle, but
-00001960: 2064 6f65 7320 6e6f 7420 6861 7665 2074   does not have t
-00001970: 6f29 2e20 4368 6f6f 7369 6e67 2064 6966  o). Choosing dif
-00001980: 6665 7265 6e74 2072 6566 6572 656e 6365  ferent reference
-00001990: 7320 7769 6c6c 2072 6573 756c 740a 2020  s will result.  
-000019a0: 2020 2020 2020 2020 2020 2020 2020 696e                in
-000019b0: 2064 6966 6665 7265 6e74 2065 7870 6c61   different expla
-000019c0: 6e61 7469 6f6e 732e 0a20 2020 2020 2020  nations..       
-000019d0: 2020 2020 2072 6574 7572 6e5f 696d 706f       return_impo
-000019e0: 7274 616e 6365 733a 2057 6865 7468 6572  rtances: Whether
-000019f0: 2074 6865 2069 6d70 6f72 7461 6e63 6520   the importance 
-00001a00: 2f20 6578 706c 616e 6174 696f 6e20 7465  / explanation te
-00001a10: 6e73 6f72 7320 7368 6f75 6c64 2062 6520  nsors should be 
-00001a20: 7265 7475 726e 6564 2061 7320 616e 206f  returned as an o
-00001a30: 7574 7075 740a 2020 2020 2020 2020 2020  utput.          
-00001a40: 2020 2020 2020 6f66 2074 6865 206d 6f64        of the mod
-00001a50: 656c 2e20 4966 2074 6869 7320 6973 2054  el. If this is T
-00001a60: 7275 652c 2074 6865 206f 7574 7075 7420  rue, the output 
-00001a70: 6f66 2074 6865 206d 6f64 656c 2077 696c  of the model wil
-00001a80: 6c20 6265 2061 2033 2d74 7570 6c65 3a0a  l be a 3-tuple:.
-00001a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001aa0: 286f 7574 7075 742c 206e 6f64 6520 696d  (output, node im
-00001ab0: 706f 7274 616e 6365 732c 2065 6467 6520  portances, edge 
-00001ac0: 696d 706f 7274 616e 6365 7329 2c20 6f74  importances), ot
-00001ad0: 6865 7277 6973 6520 6974 2069 7320 6a75  herwise it is ju
-00001ae0: 7374 2074 6865 206f 7574 7075 7420 6974  st the output it
-00001af0: 7365 6c66 0a20 2020 2020 2020 2054 2907  self.        T).
-00001b00: 721a 0000 00da 096e 756d 5f68 6561 6473  r......num_heads
-00001b10: 721e 0000 0072 1b00 0000 721c 0000 00da  r....r....r.....
-00001b20: 0e68 6173 5f73 656c 665f 6c6f 6f70 7372  .has_self_loopsr
-00001b30: 2700 0000 2901 da04 7261 7465 2901 da06  '...)...rate)...
-00001b40: 6661 6374 6f72 2901 721b 0000 00e9 ffff  factor).r.......
-00001b50: ffff a901 da04 6178 6973 da04 6d65 616e  ......axis..mean
-00001b60: 7201 0000 0029 02da 0e70 6f6f 6c69 6e67  r....)...pooling
-00001b70: 5f6d 6574 686f 64da 0d70 6f6f 6c69 6e67  _method..pooling
-00001b80: 5f69 6e64 6578 7217 0000 0063 0100 0000  _indexr....c....
-00001b90: 0000 0000 0000 0000 0200 0000 0300 0000  ................
-00001ba0: 5300 0000 f310 0000 0067 007c 005d 047d  S........g.|.].}
-00001bb0: 0164 0091 0271 0253 00a9 0172 1300 0000  .d...q.S...r....
-00001bc0: a900 a902 da02 2e30 da01 5f72 3f00 0000  .......0.._r?...
-00001bd0: 723f 0000 00fa 562f 6d65 6469 612f 7373  r?....V/media/ss
-00001be0: 642f 5072 6f67 7261 6d6d 696e 672f 6772  d/Programming/gr
-00001bf0: 6170 685f 6174 7465 6e74 696f 6e5f 7374  aph_attention_st
-00001c00: 7564 656e 742f 6772 6170 685f 6174 7465  udent/graph_atte
-00001c10: 6e74 696f 6e5f 7374 7564 656e 742f 6d6f  ntion_student/mo
-00001c20: 6465 6c73 2f6d 6567 616e 2e70 79da 0a3c  dels/megan.py..<
-00001c30: 6c69 7374 636f 6d70 3e9f 0000 00f3 0200  listcomp>.......
-00001c40: 0000 1000 7a22 4d65 6761 6e2e 5f5f 696e  ....z"Megan.__in
-00001c50: 6974 5f5f 2e3c 6c6f 6361 6c73 3e2e 3c6c  it__.<locals>.<l
-00001c60: 6973 7463 6f6d 703e 7218 0000 0029 0372  istcomp>r....).r
-00001c70: 1a00 0000 721b 0000 0072 1c00 0000 2901  ....r....r....).
-00001c80: 723b 0000 0063 0100 0000 0000 0000 0000  r;...c..........
-00001c90: 0000 0200 0000 0300 0000 5300 0000 723d  ..........S...r=
-00001ca0: 0000 0072 3e00 0000 723f 0000 0072 4000  ...r>...r?...r@.
-00001cb0: 0000 723f 0000 0072 3f00 0000 7243 0000  ..r?...r?...rC..
-00001cc0: 0072 4400 0000 ae00 0000 7245 0000 0063  .rD.......rE...c
-00001cd0: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-00001ce0: 0300 0000 5300 0000 723d 0000 00a9 0154  ....S...r=.....T
-00001cf0: 723f 0000 0072 4000 0000 723f 0000 0072  r?...r@...r?...r
-00001d00: 3f00 0000 7243 0000 0072 4400 0000 b000  ?...rC...rD.....
-00001d10: 0000 7245 0000 004e 7a3d 596f 7520 6861  ..rE...Nz=You ha
-00001d20: 7665 2073 7570 706c 6965 6420 6120 6e6f  ve supplied a no
-00001d30: 6e2d 6e75 6c6c 2076 616c 7565 2066 6f72  n-null value for
-00001d40: 2072 6567 7265 7373 696f 6e5f 7265 6665   regression_refe
-00001d50: 7265 6e63 653a 207a 682e 2054 6861 7420  rence: zh. That 
-00001d60: 6d65 616e 7320 796f 7520 6e65 6564 2074  means you need t
-00001d70: 6f20 6569 7468 6572 2073 7570 706c 7920  o either supply 
-00001d80: 6120 7661 6c69 6420 7661 6c75 6520 666f  a valid value fo
-00001d90: 7220 7265 6772 6573 7369 6f6e 5f6c 696d  r regression_lim
-00001da0: 6974 7320 6f72 2072 6567 7265 7373 696f  its or regressio
-00001db0: 6e5f 7765 6967 6874 7320 6173 2077 656c  n_weights as wel
-00001dc0: 6c72 1500 0000 7a4c 666f 7220 6578 706c  lr....zLfor expl
-00001dd0: 616e 6174 696f 6e20 636f 2d74 7261 696e  anation co-train
-00001de0: 696e 672c 2074 6865 206e 756d 6265 7220  ing, the number 
-00001df0: 6f66 2072 6567 7265 7373 696f 6e5f 7265  of regression_re
-00001e00: 6665 7265 6e63 6573 2028 6375 7272 656e  ferences (curren
-00001e10: 746c 7920 7a46 2920 6861 7320 746f 2062  tly zF) has to b
-00001e20: 6520 6578 6163 746c 7920 6861 6c66 2074  e exactly half t
-00001e30: 6865 206e 756d 6265 7220 6f66 2069 6d70  he number of imp
-00001e40: 6f72 7461 6e63 6520 6368 616e 6e65 6c73  ortance channels
-00001e50: 2028 6375 7272 656e 746c 7920 7a02 2921   (currently z.)!
-00001e60: 7a4c 466f 7220 6578 706c 616e 6174 696f  zLFor explanatio
-00001e70: 6e20 636f 2d74 7261 696e 696e 672c 2074  n co-training, t
-00001e80: 6865 206e 756d 6265 7220 6f66 2072 6567  he number of reg
-00001e90: 7265 7373 696f 6e5f 7265 6665 7265 6e63  ression_referenc
-00001ea0: 6573 2028 6375 7272 656e 746c 7920 7a54  es (currently zT
-00001eb0: 2920 6861 7320 746f 2062 6520 6578 6163  ) has to be exac
-00001ec0: 746c 7920 7468 6520 7361 6d65 2061 7320  tly the same as 
-00001ed0: 7468 6520 6669 6e61 6c20 756e 6974 2063  the final unit c
-00001ee0: 6f75 6e74 2069 6e20 7468 6520 4d4c 5020  ount in the MLP 
-00001ef0: 7461 696c 2065 6e64 2028 6375 7272 656e  tail end (curren
-00001f00: 746c 7920 fa01 297a 5529 2068 6173 2074  tly ..)zU) has t
-00001f10: 6f20 6265 2065 7861 6374 6c79 2074 6865  o be exactly the
-00001f20: 2073 616d 6520 6173 2074 6865 206e 756d   same as the num
-00001f30: 6265 7220 6f66 2072 6567 7265 7373 696f  ber of regressio
-00001f40: 6e5f 6c69 6d69 7473 2069 6e74 6572 7661  n_limits interva
-00001f50: 6c73 2028 6375 7272 656e 746c 7920 294b  ls (currently )K
-00001f60: da02 6b73 da06 6d6f 6465 6c73 da05 4d6f  ..ks..models..Mo
-00001f70: 6465 6cda 085f 5f69 6e69 745f 5f72 1a00  del..__init__r..
-00001f80: 0000 721b 0000 0072 1c00 0000 721d 0000  ..r....r....r...
-00001f90: 0072 1e00 0000 721f 0000 0072 2000 0000  .r....r....r ...
-00001fa0: 7221 0000 0072 2200 0000 7223 0000 0072  r!...r"...r#...r
-00001fb0: 2400 0000 7225 0000 0072 2600 0000 7227  $...r%...r&...r'
-00001fc0: 0000 0072 2900 0000 722a 0000 0072 2b00  ...r)...r*...r+.
-00001fd0: 0000 722c 0000 0072 2d00 0000 722e 0000  ..r,...r-...r...
-00001fe0: 0072 3000 0000 722f 0000 0072 3100 0000  .r0...r/...r1...
-00001ff0: 7228 0000 0072 3200 0000 da10 6174 7465  r(...r2.....atte
-00002000: 6e74 696f 6e5f 6c61 7965 7273 720e 0000  ntion_layersr...
-00002010: 00da 0661 7070 656e 6472 0900 0000 da0b  ...appendr......
-00002020: 6c61 795f 6472 6f70 6f75 7472 0d00 0000  lay_dropoutr....
-00002030: da0c 6c61 795f 7370 6172 7369 7479 7208  ..lay_sparsityr.
-00002040: 0000 00da 126c 6179 5f61 6374 5f69 6d70  .....lay_act_imp
-00002050: 6f72 7461 6e63 6572 0500 0000 da11 6c61  ortancer......la
-00002060: 795f 636f 6e63 6174 5f61 6c70 6861 7372  y_concat_alphasr
-00002070: 0a00 0000 da11 6c61 795f 706f 6f6c 5f65  ......lay_pool_e
-00002080: 6467 6573 5f69 6eda 126c 6179 5f70 6f6f  dges_in..lay_poo
-00002090: 6c5f 6564 6765 735f 6f75 7472 0600 0000  l_edges_outr....
-000020a0: da0b 6c61 795f 6176 6572 6167 65da 156e  ..lay_average..n
-000020b0: 6f64 655f 696d 706f 7274 616e 6365 5f75  ode_importance_u
-000020c0: 6e69 7473 da14 6e6f 6465 5f69 6d70 6f72  nits..node_impor
-000020d0: 7461 6e63 655f 6163 7473 da16 6e6f 6465  tance_acts..node
-000020e0: 5f69 6d70 6f72 7461 6e63 655f 6c61 7965  _importance_laye
-000020f0: 7273 da03 7a69 7072 0700 0000 720b 0000  rs..zipr....r...
-00002100: 00da 0c6c 6179 5f70 6f6f 6c5f 6f75 74da  ...lay_pool_out.
-00002110: 0e6c 6179 5f63 6f6e 6361 745f 6f75 74da  .lay_concat_out.
-00002120: 116c 6179 5f66 696e 616c 5f64 726f 706f  .lay_final_dropo
-00002130: 7574 da0a 6669 6e61 6c5f 6163 7473 da0c  ut..final_acts..
-00002140: 6669 6e61 6c5f 6269 6173 6573 da0c 6669  final_biases..fi
-00002150: 6e61 6c5f 6c61 7965 7273 da06 6c6f 7373  nal_layers..loss
-00002160: 6573 da12 4269 6e61 7279 4372 6f73 7365  es..BinaryCrosse
-00002170: 6e74 726f 7079 da08 6263 655f 6c6f 7373  ntropy..bce_loss
-00002180: 7202 0000 00da 0f4c 6f73 7365 7343 6f6e  r......LossesCon
-00002190: 7461 696e 6572 7210 0000 00da 1c63 6f6d  tainerr......com
-000021a0: 7069 6c65 645f 636c 6173 7369 6669 6361  piled_classifica
-000021b0: 7469 6f6e 5f6c 6f73 73da 104d 6561 6e53  tion_loss..MeanS
-000021c0: 7175 6172 6564 4572 726f 72da 086d 7365  quaredError..mse
-000021d0: 5f6c 6f73 73da 114d 6561 6e41 6273 6f6c  _loss..MeanAbsol
-000021e0: 7574 6545 7272 6f72 da08 6d61 655f 6c6f  uteError..mae_lo
-000021f0: 7373 720f 0000 00da 1863 6f6d 7069 6c65  ssr......compile
-00002200: 645f 7265 6772 6573 7369 6f6e 5f6c 6f73  d_regression_los
-00002210: 73da 0a69 7369 6e73 7461 6e63 65da 0369  s..isinstance..i
-00002220: 6e74 da05 666c 6f61 74da 036c 656e da0e  nt..float..len..
-00002230: 4173 7365 7274 696f 6e45 7272 6f72 2921  AssertionError)!
-00002240: da04 7365 6c66 721a 0000 0072 1b00 0000  ..selfr....r....
-00002250: 721c 0000 0072 1d00 0000 721e 0000 0072  r....r....r....r
-00002260: 1f00 0000 7220 0000 0072 2100 0000 7222  ....r ...r!...r"
-00002270: 0000 0072 2300 0000 7224 0000 0072 2500  ...r#...r$...r%.
-00002280: 0000 7226 0000 0072 2700 0000 7228 0000  ..r&...r'...r(..
-00002290: 0072 2900 0000 722a 0000 0072 2b00 0000  .r)...r*...r+...
-000022a0: 722c 0000 0072 2d00 0000 722e 0000 0072  r,...r-...r....r
-000022b0: 2f00 0000 7230 0000 0072 3100 0000 7232  /...r0...r1...r2
-000022c0: 0000 00da 066b 7761 7267 73da 0175 da03  .....kwargs..u..
-000022d0: 6c61 79da 0361 6374 da04 6269 6173 da0e  lay..act..bias..
-000022e0: 6e75 6d5f 7265 6665 7265 6e63 6573 da0a  num_references..
-000022f0: 6e75 6d5f 7661 6c75 6573 723f 0000 0072  num_valuesr?...r
-00002300: 3f00 0000 7243 0000 0072 4b00 0000 1e00  ?...rC...rK.....
-00002310: 0000 73ce 0000 0016 4b06 0106 0106 0106  ..s.....K.......
-00002320: 0106 0106 0106 0106 0106 0106 0106 0106  ................
-00002330: 0106 0106 0106 0106 0106 0106 0106 0106  ................
-00002340: 0106 0106 0106 0106 0106 0106 030a 0102  ................
-00002350: 0102 0104 0104 0104 0104 0102 0104 0106  ................
-00002360: f90e 090e 020e 010e 030c 010e 020e 0108  ................
-00002370: 010e 0316 0106 0116 0102 0102 0102 0102  ................
-00002380: 0106 fd0e 050e 030c 010e 0112 020c 0112  ................
-00002390: 010a 0106 011c 0102 0102 0102 0102 0106  ................
-000023a0: fd10 050c 030c 010c 020c 010c 010c 0710  ................
-000023b0: 0808 010a 020c 020c 010c 010c 0104 0204  ................
-000023c0: 010a ff10 0408 0102 0106 ff04 ff10 0408  ................
-000023d0: 0106 0106 ff04 ff0c 0408 0102 0106 ff04  ................
-000023e0: ff04 e204 1e7a 0e4d 6567 616e 2e5f 5f69  .....z.Megan.__i
-000023f0: 6e69 745f 5f63 0100 0000 0000 0000 0000  nit__c..........
-00002400: 0000 0200 0000 0900 0000 0300 0000 73be  ..............s.
-00002410: 0000 0074 0074 017c 0083 02a0 02a1 007d  ...t.t.|.......}
-00002420: 017c 01a0 0369 0064 017c 006a 0493 0164  .|...i.d.|.j...d
-00002430: 027c 006a 0593 0164 037c 006a 0693 0164  .|.j...d.|.j...d
-00002440: 047c 006a 0793 0164 057c 006a 0893 0164  .|.j...d.|.j...d
-00002450: 067c 006a 0993 0164 077c 006a 0a93 0164  .|.j...d.|.j...d
-00002460: 087c 006a 0b93 0164 097c 006a 0c93 0164  .|.j...d.|.j...d
-00002470: 0a7c 006a 0d93 0164 0b7c 006a 0e93 0164  .|.j...d.|.j...d
-00002480: 0c7c 006a 0f93 0164 0d7c 006a 1093 0164  .|.j...d.|.j...d
-00002490: 0e7c 006a 1193 0164 0f7c 006a 1293 0164  .|.j...d.|.j...d
-000024a0: 107c 006a 1393 0164 117c 006a 1493 017c  .|.j...d.|.j...|
-000024b0: 006a 157c 006a 167c 006a 177c 006a 187c  .j.|.j.|.j.|.j.|
-000024c0: 006a 1964 129c 05a5 01a1 0101 007c 0153  .j.d.........|.S
-000024d0: 0029 134e 721a 0000 0072 1b00 0000 721c  .).Nr....r....r.
-000024e0: 0000 0072 1d00 0000 721e 0000 0072 1f00  ...r....r....r..
-000024f0: 0000 7220 0000 0072 2100 0000 7222 0000  ..r ...r!...r"..
-00002500: 0072 2300 0000 7224 0000 0072 2600 0000  .r#...r$...r&...
-00002510: 7227 0000 0072 2900 0000 722a 0000 0072  r'...r)...r*...r
-00002520: 2b00 0000 722c 0000 0029 0572 2d00 0000  +...r,...).r-...
-00002530: 722e 0000 0072 3000 0000 7231 0000 0072  r....r0...r1...r
-00002540: 3200 0000 291a da05 7375 7065 7272 1200  2...)...superr..
-00002550: 0000 da0a 6765 745f 636f 6e66 6967 da06  ....get_config..
-00002560: 7570 6461 7465 721a 0000 0072 1b00 0000  updater....r....
-00002570: 721c 0000 0072 1d00 0000 721e 0000 0072  r....r....r....r
-00002580: 1f00 0000 7220 0000 0072 2100 0000 7222  ....r ...r!...r"
-00002590: 0000 0072 2300 0000 7224 0000 0072 2600  ...r#...r$...r&.
-000025a0: 0000 7227 0000 0072 2900 0000 722a 0000  ..r'...r)...r*..
-000025b0: 0072 2b00 0000 722c 0000 0072 2d00 0000  .r+...r,...r-...
-000025c0: 722e 0000 0072 3000 0000 7231 0000 0072  r....r0...r1...r
-000025d0: 3200 0000 2902 726e 0000 00da 0663 6f6e  2...).rn.....con
-000025e0: 6669 67a9 01da 095f 5f63 6c61 7373 5f5f  fig....__class__
-000025f0: 723f 0000 0072 4300 0000 7277 0000 00eb  r?...rC...rw....
-00002600: 0000 0073 5600 0000 0e01 0601 0601 02ff  ...sV...........
-00002610: 0602 02fe 0603 02fd 0604 02fc 0605 02fb  ................
-00002620: 0606 02fa 0607 02f9 0608 02f8 0609 02f7  ................
-00002630: 060a 02f6 060b 02f5 060c 02f4 060d 02f3  ................
-00002640: 060e 02f2 060f 02f1 0610 02f0 0611 02ef  ................
-00002650: 0412 0401 0401 0401 0401 0aea 0419 7a10  ..............z.
-00002660: 4d65 6761 6e2e 6765 745f 636f 6e66 6967  Megan.get_config
-00002670: da06 7265 7475 726e 6301 0000 0000 0000  ..returnc.......
-00002680: 0000 0000 0001 0000 0002 0000 0043 0000  .............C..
-00002690: 0073 1400 0000 7c00 6a00 6400 7501 7009  .s....|.j.d.u.p.
-000026a0: 7c00 6a01 6400 7501 5300 a901 4e29 0272  |.j.d.u.S...N).r
-000026b0: 2d00 0000 722e 0000 00a9 0172 6e00 0000  -...r......rn...
-000026c0: 723f 0000 0072 3f00 0000 7243 0000 00da  r?...r?...rC....
-000026d0: 1064 6f69 6e67 5f72 6567 7265 7373 696f  .doing_regressio
-000026e0: 6e0a 0100 0073 0200 0000 1402 7a16 4d65  n....s......z.Me
-000026f0: 6761 6e2e 646f 696e 675f 7265 6772 6573  gan.doing_regres
-00002700: 7369 6f6e 6301 0000 0000 0000 0000 0000  sionc...........
-00002710: 0001 0000 0002 0000 0043 0000 0073 0a00  .........C...s..
-00002720: 0000 7c00 6a00 6400 7501 5300 727d 0000  ..|.j.d.u.S.r}..
-00002730: 0029 0172 2e00 0000 727e 0000 0072 3f00  .).r....r~...r?.
-00002740: 0000 723f 0000 0072 4300 0000 da18 646f  ..r?...rC.....do
-00002750: 696e 675f 7265 6772 6573 7369 6f6e 5f77  ing_regression_w
-00002760: 6569 6768 7473 0e01 0000 7302 0000 000a  eights....s.....
-00002770: 017a 1e4d 6567 616e 2e64 6f69 6e67 5f72  .z.Megan.doing_r
-00002780: 6567 7265 7373 696f 6e5f 7765 6967 6874  egression_weight
-00002790: 73da 0874 7261 696e 696e 67da 156e 6f64  s..training..nod
-000027a0: 655f 696d 706f 7274 616e 6365 735f 6d61  e_importances_ma
-000027b0: 736b 6305 0000 0000 0000 0000 0000 001e  skc.............
-000027c0: 0000 0006 0000 004b 0000 0073 2802 0000  .......K...s(...
-000027d0: 7c00 6a00 720a 7c01 5c04 7d06 7d07 7d08  |.j.r.|.\.}.}.}.
-000027e0: 7d09 6e07 7c01 5c03 7d06 7d07 7d08 6401  }.n.|.\.}.}.}.d.
-000027f0: 7d09 6700 7d0a 7c06 7d0b 7c00 6a01 4400  }.g.}.|.}.|.j.D.
-00002800: 5d19 7d0c 7c0c 7c0b 7c07 7c08 6703 8301  ].}.|.|.|.|.g...
-00002810: 5c02 7d0b 7d0d 7c02 722c 7c00 6a02 7c0b  \.}.}.|.r,|.j.|.
-00002820: 7c02 6402 8d02 7d0b 7c0a a003 7c0d a101  |.d...}.|...|...
-00002830: 0100 7118 7c00 a004 7c0a a101 7d0a 7405  ..q.|...|...}.t.
-00002840: 6a06 7c0a 6403 6404 6405 8d03 7d0e 7c00  j.|.d.d.d...}.|.
-00002850: a007 7c0e a101 7d0e 7c00 a008 7c06 7c0e  ..|...}.|...|.|.
-00002860: 7c08 6703 a101 7d0f 7c00 a009 7c06 7c0e  |.g...}.|...|.|.
-00002870: 7c08 6703 a101 7d10 7c00 a00a 7c10 7c0f  |.g...}.|...|.|.
-00002880: 6702 a101 7d11 7c0b 7d12 7c00 6a0b 4400  g...}.|.}.|.j.D.
-00002890: 5d06 7d0c 7c0c 7c12 8301 7d12 7160 7c00  ].}.|.|...}.q`|.
-000028a0: a007 7c12 a101 7d12 7c12 7c11 1400 7d13  ..|...}.|.|...}.
-000028b0: 7c00 a00c 7c13 a101 0100 7c04 6401 7501  |...|.....|.d.u.
-000028c0: 7284 7405 a00d 7c04 7405 6a0e a102 7d04  r.t...|.t.j...}.
-000028d0: 7c13 7c04 1400 7d13 6700 7d14 7c00 6a0f  |.|...}.g.}.|.j.
-000028e0: 6403 1900 7d15 7410 7c00 6a11 8301 4400  d...}.t.|.j...D.
-000028f0: 5d2e 7d16 7405 6a12 7c13 6401 6401 8502  ].}.t.j.|.d.d...
-00002900: 6401 6401 8502 7c16 6603 1900 6403 6406  d.d...|.f...d.d.
-00002910: 8d02 7d17 7c0b 7c17 1400 7d18 7c00 6a13  ..}.|.|...}.|.j.
-00002920: 6401 7501 72b4 7c00 6a13 7c16 1900 7d19  d.u.r.|.j.|...}.
-00002930: 7c19 7c18 8301 7d18 7c00 a014 7c18 a101  |.|...}.|...|...
-00002940: 7d1a 7c14 a003 7c1a a101 0100 7190 7c00  }.|...|.....q.|.
-00002950: a015 7c14 a101 7d1a 7c00 6a00 72ce 7c00  ..|...}.|.j.r.|.
-00002960: a015 7c1a 7c09 6702 a101 7d1a 7416 7c00  ..|.|.g...}.t.|.
-00002970: 6a17 8301 7d1b 7418 7c00 6a17 8301 4400  j...}.t.|.j...D.
-00002980: 5d17 5c02 7d1c 7d0c 7c0c 7c1a 8301 7d1a  ].\.}.}.|.|...}.
-00002990: 7c02 72ef 7c1c 7c1b 6407 1800 6b00 72ef  |.r.|.|.d...k.r.
-000029a0: 7c00 6a19 7c1a 7c02 6402 8d02 7d1a 71d8  |.j.|.|.d...}.q.
-000029b0: 7c00 6a1a 9001 7206 7405 a01b 7c1a a101  |.j...r.t...|...
-000029c0: 7405 6a1c 7c00 6a1d 7405 6a0e 6408 8d02  t.j.|.j.t.j.d...
-000029d0: 1400 7d1d 7c1a 7c1d 1700 7d1a 7c00 6a1e  ..}.|.|...}.|.j.
-000029e0: 9001 730d 7c03 9001 7212 7c1a 7c13 7c0e  ..s.|...r.|.|.|.
-000029f0: 6603 5300 7c1a 5300 2909 61b7 0100 000a  f.S.|.S.).a.....
-00002a00: 2020 2020 2020 2020 466f 7277 6172 6420          Forward 
-00002a10: 7061 7373 206f 6620 7468 6520 6d6f 6465  pass of the mode
-00002a20: 6c2e 0a0a 2020 2020 2020 2020 2a2a 5368  l...        **Sh
-00002a30: 6170 6520 4578 706c 616e 6174 696f 6e73  ape Explanations
-00002a40: 3a2a 2a20 416c 6c20 7368 6170 6573 2069  :** All shapes i
-00002a50: 6e20 6272 6163 6b65 7473 205b 5d20 6172  n brackets [] ar
-00002a60: 6520 7261 6767 6564 2064 696d 656e 7369  e ragged dimensi
-00002a70: 6f6e 7321 0a0a 2020 2020 2020 2020 2d20  ons!..        - 
-00002a80: 563a 204e 756d 206e 6f64 6573 2069 6e20  V: Num nodes in 
-00002a90: 7468 6520 6772 6170 680a 2020 2020 2020  the graph.      
-00002aa0: 2020 2d20 453a 204e 756d 2065 6467 6573    - E: Num edges
-00002ab0: 2069 6e20 7468 6520 6772 6170 680a 2020   in the graph.  
-00002ac0: 2020 2020 2020 2d20 4e3a 204e 756d 2066        - N: Num f
-00002ad0: 6561 7475 7265 2076 616c 7565 7320 7065  eature values pe
-00002ae0: 7220 6e6f 6465 0a20 2020 2020 2020 202d  r node.        -
-00002af0: 204d 3a20 4e55 6d20 6665 6174 7572 6520   M: NUm feature 
-00002b00: 7661 6c75 6573 2070 6572 2065 6467 650a  values per edge.
-00002b10: 2020 2020 2020 2020 2d20 483a 204e 756d          - H: Num
-00002b20: 2066 6561 7475 7265 2076 616c 7565 7320   feature values 
-00002b30: 7065 7220 6772 6170 680a 2020 2020 2020  per graph.      
-00002b40: 2020 2d20 423a 204e 756d 2067 7261 7068    - B: Num graph
-00002b50: 7320 696e 2061 2062 6174 6368 0a20 2020  s in a batch.   
-00002b60: 2020 2020 202d 204b 3a20 4e75 6d20 696d       - K: Num im
-00002b70: 706f 7274 616e 6365 2028 6578 706c 616e  portance (explan
-00002b80: 6174 696f 6e29 2063 6861 6e6e 656c 7320  ation) channels 
-00002b90: 636f 6e66 6967 7572 6564 2069 6e20 7468  configured in th
-00002ba0: 6520 636f 6e73 7472 7563 746f 720a 2020  e constructor.  
-00002bb0: 2020 2020 2020 4e29 0172 8100 0000 7237        N).r....r7
-00002bc0: 0000 0046 2902 7239 0000 00da 086b 6565  ...F).r9.....kee
-00002bd0: 7064 696d 7372 3800 0000 7215 0000 0029  pdimsr8...r....)
-00002be0: 01da 0564 7479 7065 291f 7232 0000 0072  ...dtype).r2...r
-00002bf0: 4c00 0000 724e 0000 0072 4d00 0000 7251  L...rN...rM...rQ
-00002c00: 0000 00da 0274 66da 0a72 6564 7563 655f  .....tf..reduce_
-00002c10: 7375 6d72 5000 0000 7252 0000 0072 5300  sumrP...rR...rS.
-00002c20: 0000 7254 0000 0072 5700 0000 724f 0000  ..rT...rW...rO..
-00002c30: 00da 0463 6173 74da 0766 6c6f 6174 3332  ...cast..float32
-00002c40: 7229 0000 00da 0572 616e 6765 7220 0000  r).....ranger ..
-00002c50: 00da 0b65 7870 616e 645f 6469 6d73 7225  ...expand_dimsr%
-00002c60: 0000 0072 5900 0000 725a 0000 0072 6c00  ...rY...rZ...rl.
-00002c70: 0000 725e 0000 00da 0965 6e75 6d65 7261  ..r^.....enumera
-00002c80: 7465 725b 0000 0072 7f00 0000 da09 6f6e  ter[...r......on
-00002c90: 6573 5f6c 696b 65da 0863 6f6e 7374 616e  es_like..constan
-00002ca0: 7472 3000 0000 7231 0000 0029 1e72 6e00  tr0...r1...).rn.
-00002cb0: 0000 da06 696e 7075 7473 7281 0000 0072  ....inputsr....r
-00002cc0: 3100 0000 7282 0000 0072 6f00 0000 da0a  1...r....ro.....
-00002cd0: 6e6f 6465 5f69 6e70 7574 da0a 6564 6765  node_input..edge
-00002ce0: 5f69 6e70 7574 da10 6564 6765 5f69 6e64  _input..edge_ind
-00002cf0: 6578 5f69 6e70 7574 da0b 6772 6170 685f  ex_input..graph_
-00002d00: 696e 7075 74da 0661 6c70 6861 73da 0178  input..alphas..x
-00002d10: 7271 0000 00da 0561 6c70 6861 da10 6564  rq.....alpha..ed
-00002d20: 6765 5f69 6d70 6f72 7461 6e63 6573 da0f  ge_importances..
-00002d30: 706f 6f6c 6564 5f65 6467 6573 5f69 6eda  pooled_edges_in.
-00002d40: 1070 6f6f 6c65 645f 6564 6765 735f 6f75  .pooled_edges_ou
-00002d50: 74da 0c70 6f6f 6c65 645f 6564 6765 73da  t..pooled_edges.
-00002d60: 166e 6f64 655f 696d 706f 7274 616e 6365  .node_importance
-00002d70: 735f 7469 6c64 65da 106e 6f64 655f 696d  s_tilde..node_im
-00002d80: 706f 7274 616e 6365 73da 046f 7574 73da  portances..outs.
-00002d90: 016e da01 6bda 156e 6f64 655f 696d 706f  .n..k..node_impo
-00002da0: 7274 616e 6365 5f73 6c69 6365 da11 6d61  rtance_slice..ma
-00002db0: 736b 6564 5f65 6d62 6564 6469 6e67 73da  sked_embeddings.
-00002dc0: 0d6c 6179 5f74 7261 6e73 666f 726d da03  .lay_transform..
-00002dd0: 6f75 74da 106e 756d 5f66 696e 616c 5f6c  out..num_final_l
-00002de0: 6179 6572 73da 0163 da09 7265 6665 7265  ayers..c..refere
-00002df0: 6e63 6572 3f00 0000 723f 0000 0072 4300  ncer?...r?...rC.
-00002e00: 0000 da04 6361 6c6c 1301 0000 7366 0000  ....call....sf..
-00002e10: 0006 1f0e 010a 0204 0104 0504 010a 0112  ................
-00002e20: 0304 010e 010c 020a 0410 010a 0110 0610  ................
-00002e30: 010e 0104 020a 010a 010a 0208 020a 0108  ................
-00002e40: 090e 0108 0104 050a 010e 0120 0108 010a  ........... ....
-00002e50: 050a 0108 010a 020c 030a 0306 040e 010a  ................
-00002e60: 0412 0108 0110 010e 0102 8008 021c 0108  ................
-00002e70: 010e 050a 0104 027a 0a4d 6567 616e 2e63  .......z.Megan.c
-00002e80: 616c 6c63 0200 0000 0000 0000 0000 0000  allc............
-00002e90: 0d00 0000 0900 0000 4300 0000 730c 0100  ........C...s...
-00002ea0: 0067 007d 0267 007d 0374 007c 006a 0183  .g.}.g.}.t.|.j..
-00002eb0: 0144 005d 6e5c 027d 047d 0574 026a 037c  .D.]n\.}.}.t.j.|
-00002ec0: 0164 0064 0085 027c 0466 0219 0064 0164  .d.d...|.f...d.d
-00002ed0: 028d 027d 0674 02a0 047c 067c 0518 00a1  ...}.t...|.|....
-00002ee0: 017d 077c 006a 0572 417c 006a 067c 0419  .}.|.j.rA|.j.|..
-00002ef0: 007d 0874 02a0 077c 067c 056b 007c 077c  .}.t...|.|.k.|.|
-00002f00: 006a 087c 0864 0319 0014 0014 007c 077c  .j.|.d.......|.|
-00002f10: 006a 087c 0864 0419 0014 0014 00a1 037d  .j.|.d.........}
-00002f20: 076e 187c 006a 097c 0419 007d 0974 047c  .n.|.j.|...}.t.|
-00002f30: 0964 0419 007c 0964 0319 0018 0083 017d  .d...|.d.......}
-00002f40: 0a7c 077c 006a 0814 0064 057c 0a14 001b  .|.|.j...d.|....
-00002f50: 007d 0774 02a0 077c 067c 056b 0064 0664  .}.t...|.|.k.d.d
-00002f60: 07a1 037d 0b74 02a0 077c 067c 056b 0464  ...}.t...|.|.k.d
-00002f70: 0664 07a1 037d 0c7c 027c 077c 0767 0237  .d...}.|.|.|.g.7
-00002f80: 007d 027c 037c 0b7c 0c67 0237 007d 0371  .}.|.|.|.g.7.}.q
-00002f90: 0974 026a 0a7c 0264 0164 028d 0274 026a  .t.j.|.d.d...t.j
-00002fa0: 0a7c 0364 0164 028d 0266 0253 0029 084e  .|.d.d...f.S.).N
-00002fb0: 7237 0000 0072 3800 0000 7201 0000 0072  r7...r8...r....r
-00002fc0: 1700 0000 6700 0000 0000 00e0 3f67 0000  ....g.......?g..
-00002fd0: 0000 0000 f03f 7214 0000 0029 0b72 8b00  .....?r....).r..
-00002fe0: 0000 7230 0000 0072 8500 0000 728a 0000  ..r0...r....r...
-00002ff0: 00da 0361 6273 7280 0000 0072 2e00 0000  ...absr....r....
-00003000: da05 7768 6572 6572 2400 0000 722d 0000  ..wherer$...r-..
-00003010: 00da 0663 6f6e 6361 7429 0d72 6e00 0000  ...concat).rn...
-00003020: da08 6f75 745f 7472 7565 da07 7361 6d70  ..out_true..samp
-00003030: 6c65 73da 056d 6173 6b73 da01 6972 3000  les..masks..ir0.
-00003040: 0000 da06 7661 6c75 6573 da10 6365 6e74  ....values..cent
-00003050: 6572 5f64 6973 7461 6e63 6573 722e 0000  er_distancesr...
-00003060: 0072 2d00 0000 da10 7265 6772 6573 7369  .r-.....regressi
-00003070: 6f6e 5f77 6964 7468 da07 6c6f 5f6d 6173  on_width..lo_mas
-00003080: 6bda 0768 695f 6d61 736b 723f 0000 0072  k..hi_maskr?...r
-00003090: 3f00 0000 7243 0000 00da 1772 6567 7265  ?...rC.....regre
-000030a0: 7373 696f 6e5f 6175 676d 656e 7461 7469  ssion_augmentati
-000030b0: 6f6e 9901 0000 732c 0000 0004 0204 0112  on....s,........
-000030c0: 021a 010e 0106 020a 0104 0106 0110 0110  ................
-000030d0: 0106 fd0a 0714 0112 0112 0812 020c 020e  ................
-000030e0: 010c 030c 0104 fe7a 1d4d 6567 616e 2e72  .......z.Megan.r
-000030f0: 6567 7265 7373 696f 6e5f 6175 676d 656e  egression_augmen
-00003100: 7461 7469 6f6e da0e 7570 6461 7465 5f77  tation..update_w
-00003110: 6569 6768 7473 6304 0000 0000 0000 0000  eightsc.........
-00003120: 0000 0013 0000 0008 0000 0043 0000 0073  ...........C...s
-00003130: 3a01 0000 7c00 6a00 7209 7c02 5c03 7d04  :...|.j.r.|.\.}.
-00003140: 7d05 7d05 6e02 7c02 7d04 6401 7d06 7401  }.}.n.|.}.d.}.t.
-00003150: a002 a100 8f6c 7d07 7c00 7c01 6402 6402  .....l}.|.|.d.d.
-00003160: 6403 8d03 7d08 7c08 5c03 7d09 7d0a 7d0b  d...}.|.\.}.}.}.
-00003170: 6700 7d0c 7403 7c00 6a04 8301 4400 5d1c  g.}.t.|.j...D.].
-00003180: 7d0d 7401 6a05 7c0a 6400 6400 8502 6400  }.t.j.|.d.d...d.
-00003190: 6400 8502 7c0d 6603 1900 6404 6405 8d02  d...|.f...d.d...
-000031a0: 7d0e 7c00 a006 7c0e a101 7d0f 7c0c a007  }.|...|...}.|...
-000031b0: 7c0f a101 0100 7125 7c00 a008 7c0c a101  |.....q%|...|...
-000031c0: 7d0c 7c00 6a09 7261 7c00 a00a 7c04 a101  }.|.j.ra|...|...
-000031d0: 5c02 7d04 7d10 7c0c 7d09 7c00 6a04 7c00  \.}.}.|.}.|.j.|.
-000031e0: a00b 7c04 7c10 1400 7c09 7c10 1400 a102  ..|.|...|.|.....
-000031f0: 1400 7d06 6e10 740c 7c0c 7c00 6a0d 6406  ..}.n.t.|.|.j.d.
-00003200: 6407 8d03 7d09 7c00 a00e 7c04 7c09 7c04  d...}.|...|.|.|.
-00003210: 1400 a102 7d06 7c06 7c00 6a0f 3900 7d06  ....}.|.|.j.9.}.
-00003220: 5700 6400 0400 0400 8303 0100 6e08 3100  W.d.........n.1.
-00003230: 7380 7701 0100 0100 0100 5900 0100 7c00  s.w.......Y...|.
-00003240: 6a10 7d11 7c07 a011 7c06 7c11 a102 7d12  j.}.|...|.|...}.
-00003250: 7c03 7299 7c00 6a12 a013 7414 7c12 7c11  |.r.|.j...t.|.|.
-00003260: 8302 a101 0100 6408 7c06 6901 5300 2909  ......d.|.i.S.).
-00003270: 4e72 0100 0000 54a9 0272 8100 0000 7231  Nr....T..r....r1
-00003280: 0000 0072 3700 0000 7238 0000 0072 1500  ...r7...r8...r..
-00003290: 0000 a902 da05 7368 6966 74da 0a6d 756c  ......shift..mul
-000032a0: 7469 706c 6965 72da 0865 7870 5f6c 6f73  tiplier..exp_los
-000032b0: 7329 1572 3100 0000 7285 0000 00da 0c47  s).r1...r......G
-000032c0: 7261 6469 656e 7454 6170 6572 8900 0000  radientTaper....
-000032d0: 7220 0000 0072 8a00 0000 7259 0000 0072  r ...r....rY...r
-000032e0: 4d00 0000 725a 0000 0072 7f00 0000 72b3  M...rZ...r....r.
-000032f0: 0000 0072 6800 0000 7211 0000 0072 2400  ...rh...r....r$.
-00003300: 0000 7263 0000 0072 2300 0000 da13 7472  ..rc...r#.....tr
-00003310: 6169 6e61 626c 655f 7661 7269 6162 6c65  ainable_variable
-00003320: 73da 0867 7261 6469 656e 74da 096f 7074  s..gradient..opt
-00003330: 696d 697a 6572 da0f 6170 706c 795f 6772  imizer..apply_gr
-00003340: 6164 6965 6e74 7372 5800 0000 2913 726e  adientsrX...).rn
-00003350: 0000 0072 9400 0000 da01 7972 b400 0000  ...r......yr....
-00003360: 72aa 0000 0072 4200 0000 72b9 0000 00da  r....rB...r.....
-00003370: 0474 6170 65da 0679 5f70 7265 64da 086f  .tape..y_pred..o
-00003380: 7574 5f70 7265 64da 076e 695f 7072 6564  ut_pred..ni_pred
-00003390: da07 6569 5f70 7265 6472 9c00 0000 729e  ..ei_predr....r.
-000033a0: 0000 00da 166e 6f64 655f 696d 706f 7274  .....node_import
-000033b0: 616e 6365 735f 736c 6963 6572 a200 0000  ances_slicer....
-000033c0: da04 6d61 736b da0e 7472 6169 6e61 626c  ..mask..trainabl
-000033d0: 655f 7661 7273 da0d 6578 705f 6772 6164  e_vars..exp_grad
-000033e0: 6965 6e74 7372 3f00 0000 723f 0000 0072  ientsr?...r?...r
-000033f0: 4300 0000 da16 7472 6169 6e5f 7374 6570  C.....train_step
-00003400: 5f65 7870 6c61 6e61 7469 6f6e c101 0000  _explanation....
-00003410: 7338 0000 0006 030c 0104 0204 020a 010e  s8..............
-00003420: 020a 0104 070e 0120 010a 010c 020a 0306  ....... ........
-00003430: 020e 0104 010e 0106 0108 ff10 0510 010c  ................
-00003440: 021c e106 220c 0104 0312 0108 027a 1c4d  ...."........z.M
-00003450: 6567 616e 2e74 7261 696e 5f73 7465 705f  egan.train_step_
-00003460: 6578 706c 616e 6174 696f 6e63 0200 0000  explanationc....
-00003470: 0000 0000 0000 0000 1800 0000 0800 0000  ................
-00003480: 4300 0000 73d8 0100 0074 007c 0183 0164  C...s....t.|...d
-00003490: 016b 0272 0c7c 015c 037d 027d 037d 046e  .k.r.|.\.}.}.}.n
-000034a0: 0664 007d 047c 015c 027d 027d 037c 006a  .d.}.|.\.}.}.|.j
-000034b0: 0164 026b 0372 217c 006a 0272 217c 00a0  .d.k.r!|.j.r!|..
-000034c0: 037c 027c 03a1 027d 056e 0269 007d 0564  .|.|...}.n.i.}.d
-000034d0: 027d 0674 04a0 05a1 008f 8c7d 077c 035c  .}.t.......}.|.\
-000034e0: 037d 087d 097d 0a7c 007c 0264 0364 0364  .}.}.}.|.|.d.d.d
-000034f0: 048d 035c 037d 0b7d 0c7d 0d7c 006a 067c  ...\.}.}.}.|.j.|
-00003500: 087c 097c 0a67 037c 0b7c 0c7c 0d67 037c  .|.|.g.|.|.|.g.|
-00003510: 047c 006a 0764 058d 047d 0e7c 006a 0164  .|.j.d...}.|.j.d
-00003520: 026b 0372 ae7c 006a 0273 ae67 007d 0f74  .k.r.|.j.s.g.}.t
-00003530: 087c 006a 0983 0144 005d 1c7d 1074 046a  .|.j...D.].}.t.j
-00003540: 0a7c 0c64 0064 0085 0264 0064 0085 027c  .|.d.d...d.d...|
-00003550: 1066 0319 0064 0664 078d 027d 117c 00a0  .f...d.d...}.|..
-00003560: 0b7c 11a1 017d 127c 0fa0 0c7c 12a1 0101  .|...}.|...|....
-00003570: 0071 587c 00a0 0d7c 0fa1 017d 0f7c 006a  .qX|...|...}.|.j
-00003580: 0e72 917c 00a0 0f7c 08a1 015c 027d 137d  .r.|...|...\.}.}
-00003590: 147c 0f7d 157c 00a0 107c 137c 1414 007c  .|.}.|...|.|...|
-000035a0: 157c 1414 00a1 027d 066e 1074 117c 0f7c  .|.....}.n.t.|.|
-000035b0: 006a 1264 0864 098d 037c 0814 007d 157c  .j.d.d...|...}.|
-000035c0: 00a0 137c 087c 15a1 027d 067c 067c 006a  ...|.|...}.|.|.j
-000035d0: 0139 007d 067c 067c 0564 0a3c 007c 0e7c  .9.}.|.|.d.<.|.|
-000035e0: 0637 007d 0e57 0064 0004 0004 0083 0301  .7.}.W.d........
-000035f0: 006e 0831 0073 b877 0101 0001 0001 0059  .n.1.s.w.......Y
-00003600: 0001 007c 006a 147d 167c 07a0 157c 0e7c  ...|.j.}.|...|.|
-00003610: 16a1 027d 177c 006a 16a0 1774 187c 177c  ...}.|.j...t.|.|
-00003620: 1683 02a1 0101 007c 006a 196a 1a7c 037c  .......|.j.j.|.|
-00003630: 006a 1b73 d87c 0b6e 047c 0b7c 0c7c 0d67  .j.s.|.n.|.|.|.g
-00003640: 037c 0464 0b8d 0301 0069 0064 0c64 0d84  .|.d.....i.d.d..
-00003650: 007c 006a 1c44 0083 01a5 017c 05a5 0153  .|.j.D.....|...S
-00003660: 0029 0e4e e903 0000 0072 0100 0000 5472  .).N.....r....Tr
-00003670: b500 0000 2902 da0d 7361 6d70 6c65 5f77  ....)...sample_w
-00003680: 6569 6768 74da 1572 6567 756c 6172 697a  eight..regulariz
-00003690: 6174 696f 6e5f 6c6f 7373 6573 7237 0000  ation_lossesr7..
-000036a0: 0072 3800 0000 7217 0000 0072 b600 0000  .r8...r....r....
-000036b0: 72b9 0000 0029 0172 cb00 0000 6301 0000  r....).r....c...
-000036c0: 0000 0000 0000 0000 0002 0000 0005 0000  ................
-000036d0: 0053 0000 0073 1800 0000 6900 7c00 5d08  .S...s....i.|.].
-000036e0: 7d01 7c01 6a00 7c01 a001 a100 9302 7102  }.|.j.|.......q.
-000036f0: 5300 723f 0000 0029 02da 046e 616d 65da  S.r?...)...name.
-00003700: 0672 6573 756c 7429 0272 4100 0000 da01  .result).rA.....
-00003710: 6d72 3f00 0000 723f 0000 0072 4300 0000  mr?...r?...rC...
-00003720: da0a 3c64 6963 7463 6f6d 703e 4302 0000  ..<dictcomp>C...
-00003730: 7302 0000 0018 007a 244d 6567 616e 2e74  s......z$Megan.t
-00003740: 7261 696e 5f73 7465 702e 3c6c 6f63 616c  rain_step.<local
-00003750: 733e 2e3c 6469 6374 636f 6d70 3e29 1d72  s>.<dictcomp>).r
-00003760: 6c00 0000 7223 0000 0072 2800 0000 72c9  l...r#...r(...r.
-00003770: 0000 0072 8500 0000 72ba 0000 00da 0d63  ...r....r......c
-00003780: 6f6d 7069 6c65 645f 6c6f 7373 725f 0000  ompiled_lossr_..
-00003790: 0072 8900 0000 7220 0000 0072 8a00 0000  .r....r ...r....
-000037a0: 7259 0000 0072 4d00 0000 725a 0000 0072  rY...rM...rZ...r
-000037b0: 7f00 0000 72b3 0000 0072 6800 0000 7211  ....r....rh...r.
-000037c0: 0000 0072 2400 0000 7263 0000 0072 bb00  ...r$...rc...r..
-000037d0: 0000 72bc 0000 0072 bd00 0000 72be 0000  ..r....r....r...
-000037e0: 0072 5800 0000 da10 636f 6d70 696c 6564  .rX.....compiled
-000037f0: 5f6d 6574 7269 6373 da0c 7570 6461 7465  _metrics..update
-00003800: 5f73 7461 7465 7231 0000 00da 076d 6574  _stater1.....met
-00003810: 7269 6373 2918 726e 0000 00da 0464 6174  rics).rn.....dat
-00003820: 6172 9400 0000 72bf 0000 0072 cb00 0000  ar....r....r....
-00003830: da0b 6578 705f 6d65 7472 6963 7372 b900  ..exp_metricsr..
-00003840: 0000 72c0 0000 0072 aa00 0000 da07 6e69  ..r....r......ni
-00003850: 5f74 7275 65da 0765 695f 7472 7565 72c2  _true..ei_truer.
-00003860: 0000 0072 c300 0000 72c4 0000 00da 046c  ...r....r......l
-00003870: 6f73 7372 9c00 0000 729e 0000 0072 c500  ossr....r....r..
-00003880: 0000 72a2 0000 00da 095f 6f75 745f 7472  ..r......_out_tr
-00003890: 7565 72c6 0000 00da 095f 6f75 745f 7072  uer......_out_pr
-000038a0: 6564 72c7 0000 00da 0967 7261 6469 656e  edr......gradien
-000038b0: 7473 723f 0000 0072 3f00 0000 7243 0000  tsr?...r?...rC..
-000038c0: 00da 0a74 7261 696e 5f73 7465 70f5 0100  ...train_step...
-000038d0: 0073 7000 0000 0c01 0c01 0402 0801 1006  .sp.............
-000038e0: 0e01 0402 0402 0a01 0a02 1401 0401 0801  ................
-000038f0: 0801 0201 0401 06fc 1007 0406 0e01 2001  .............. .
-00003900: 0a01 0c02 0a03 0602 0e01 0401 0a01 0601  ................
-00003910: 06ff 0206 0201 0401 0201 04fd 0204 04fc  ................
-00003920: 0c05 0a02 0801 0801 0280 1cd3 062f 0c01  ............./..
-00003930: 1202 0602 0201 1201 0201 06fd 0208 0e01  ................
-00003940: 02ff 0202 04fe 7a10 4d65 6761 6e2e 7472  ......z.Megan.tr
-00003950: 6169 6e5f 7374 6570 2903 4646 4e72 4600  ain_step).FFNrF.
-00003960: 0000 291b da08 5f5f 6e61 6d65 5f5f da0a  ..)...__name__..
-00003970: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
-00003980: 616c 6e61 6d65 5f5f da07 5f5f 646f 635f  alname__..__doc_
-00003990: 5fda 0174 da04 4c69 7374 726a 0000 00da  _..t..Listrj....
-000039a0: 0373 7472 da04 626f 6f6c 726b 0000 00da  .str..boolrk....
-000039b0: 084f 7074 696f 6e61 6c72 4800 0000 da06  .OptionalrH.....
-000039c0: 6c61 7965 7273 da05 4c61 7965 72da 0554  layers..Layer..T
-000039d0: 7570 6c65 724b 0000 0072 7700 0000 da08  uplerK...rw.....
-000039e0: 7072 6f70 6572 7479 727f 0000 0072 8000  propertyr....r..
-000039f0: 0000 7285 0000 00da 0c52 6167 6765 6454  ..r......RaggedT
-00003a00: 656e 736f 7272 a600 0000 72b3 0000 0072  ensorr....r....r
-00003a10: c900 0000 72dd 0000 00da 0d5f 5f63 6c61  ....r......__cla
-00003a20: 7373 6365 6c6c 5f5f 723f 0000 0072 3f00  sscell__r?...r?.
-00003a30: 0000 727a 0000 0072 4300 0000 7212 0000  ..rz...rC...r...
-00003a40: 0014 0000 0073 c600 0000 0800 0401 020c  .....s..........
-00003a50: 0201 0201 0201 0202 0201 0201 0201 0201  ................
-00003a60: 0201 0201 0201 0201 0201 0402 0201 0201  ................
-00003a70: 0201 0201 0201 0201 0201 0201 0201 04e4  ................
-00003a80: 0802 02fe 0203 02fd 0204 02fc 0205 02fb  ................
-00003a90: 0206 02fa 0808 02f8 0209 02f7 020a 02f6  ................
-00003aa0: 020b 02f5 020c 02f4 020d 02f3 120e 02f2  ................
-00003ab0: 020f 02f1 0210 02f0 0211 02ef 0813 02ed  ................
-00003ac0: 0214 02ec 0215 02eb 0216 02ea 1217 02e9  ................
-00003ad0: 1218 02e8 1819 02e7 081a 02e6 021b 02e5  ................
-00003ae0: 021c 0ae4 007f 0c4e 021f 1001 0e03 0207  .......N........
-00003af0: 0201 0201 04fc 0202 02fe 0203 02fd 0a04  ................
-00003b00: 0afc 007f 0807 0229 04ff 0201 0aff 1034  .......).......4
-00003b10: 7212 0000 0029 20da 0674 7970 696e 6772  r....) ..typingr
-00003b20: e200 0000 da0a 7465 6e73 6f72 666c 6f77  ......tensorflow
-00003b30: 7285 0000 00da 1074 656e 736f 7266 6c6f  r......tensorflo
-00003b40: 772e 6b65 7261 73da 056b 6572 6173 7248  w.keras..kerasrH
-00003b50: 0000 00da 1e74 656e 736f 7266 6c6f 772e  .....tensorflow.
-00003b60: 7079 7468 6f6e 2e6b 6572 6173 2e65 6e67  python.keras.eng
-00003b70: 696e 6572 0200 0000 da10 6b67 636e 6e2e  iner......kgcnn.
-00003b80: 6461 7461 2e75 7469 6c73 7203 0000 00da  data.utilsr.....
-00003b90: 146b 6763 6e6e 2e6c 6179 6572 732e 6d6f  .kgcnn.layers.mo
-00003ba0: 6475 6c65 7372 0400 0000 7205 0000 0072  dulesr....r....r
-00003bb0: 0600 0000 7207 0000 0072 0800 0000 7209  ....r....r....r.
-00003bc0: 0000 00da 146b 6763 6e6e 2e6c 6179 6572  .....kgcnn.layer
-00003bd0: 732e 706f 6f6c 696e 6772 0a00 0000 720b  s.poolingr....r.
-00003be0: 0000 0072 0c00 0000 da1e 6772 6170 685f  ...r......graph_
-00003bf0: 6174 7465 6e74 696f 6e5f 7374 7564 656e  attention_studen
-00003c00: 742e 6c61 7965 7273 720d 0000 0072 0e00  t.layersr....r..
-00003c10: 0000 da20 6772 6170 685f 6174 7465 6e74  ... graph_attent
-00003c20: 696f 6e5f 7374 7564 656e 742e 7472 6169  ion_student.trai
-00003c30: 6e69 6e67 720f 0000 0072 1000 0000 7211  ningr....r....r.
-00003c40: 0000 0072 4900 0000 724a 0000 0072 1200  ...rI...rJ...r..
-00003c50: 0000 723f 0000 0072 3f00 0000 723f 0000  ..r?...r?...r?..
-00003c60: 0072 4300 0000 da08 3c6d 6f64 756c 653e  .rC.....<module>
-00003c70: 0100 0000 7322 0000 0008 0008 020c 010c  ....s"..........
-00003c80: 010c 010c 0110 0114 010c 010c 010c 010c  ................
-00003c90: 010c 010c 010c 010c 0118 03              ...........
+00000040: 6401 6c04 6d05 5a06 0100 6400 6401 6c07  d.l.m.Z...d.d.l.
+00000050: 6d00 5a08 0100 6400 6402 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
+00000060: 0100 6400 6403 6c0b 6d0c 5a0c 0100 6400  ..d.d.l.m.Z...d.
+00000070: 6404 6c0d 6d0e 5a0e 0100 6400 6405 6c0d  d.l.m.Z...d.d.l.
+00000080: 6d0f 5a0f 6d10 5a10 0100 6400 6406 6c0d  m.Z.m.Z...d.d.l.
+00000090: 6d11 5a11 6d12 5a12 6d13 5a13 0100 6400  m.Z.m.Z.m.Z...d.
+000000a0: 6407 6c14 6d15 5a15 0100 6400 6408 6c14  d.l.m.Z...d.d.l.
+000000b0: 6d16 5a16 0100 6400 6409 6c14 6d17 5a17  m.Z...d.d.l.m.Z.
+000000c0: 0100 6400 640a 6c18 6d19 5a19 0100 6400  ..d.d.l.m.Z...d.
+000000d0: 640b 6c1a 6d1b 5a1b 0100 6400 640c 6c1a  d.l.m.Z...d.d.l.
+000000e0: 6d1c 5a1c 0100 6400 640d 6c1d 6d1e 5a1e  m.Z...d.d.l.m.Z.
+000000f0: 0100 6400 640e 6c1d 6d1f 5a1f 0100 6400  ..d.d.l.m.Z...d.
+00000100: 640f 6c1d 6d20 5a20 0100 4700 6410 6411  d.l.m Z ..G.d.d.
+00000110: 8400 6411 6506 6a21 6a22 8303 5a23 6401  ..d.e.j!j"..Z#d.
+00000120: 5300 2912 e900 0000 004e 2901 da0d 636f  S.)......N)...co
+00000130: 6d70 696c 655f 7574 696c 7329 01da 1f72  mpile_utils)...r
+00000140: 6167 6765 645f 7465 6e73 6f72 5f66 726f  agged_tensor_fro
+00000150: 6d5f 6e65 7374 6564 5f6e 756d 7079 2901  m_nested_numpy).
+00000160: da0e 4772 6170 6842 6173 654c 6179 6572  ..GraphBaseLayer
+00000170: 2902 da0f 4c61 7a79 436f 6e63 6174 656e  )...LazyConcaten
+00000180: 6174 65da 0b4c 617a 7941 7665 7261 6765  ate..LazyAverage
+00000190: 2903 da0e 4465 6e73 6545 6d62 6564 6469  )...DenseEmbeddi
+000001a0: 6e67 da13 4163 7469 7661 7469 6f6e 456d  ng..ActivationEm
+000001b0: 6265 6464 696e 67da 1044 726f 706f 7574  bedding..Dropout
+000001c0: 456d 6265 6464 696e 6729 01da 1150 6f6f  Embedding)...Poo
+000001d0: 6c69 6e67 4c6f 6361 6c45 6467 6573 2901  lingLocalEdges).
+000001e0: da0c 506f 6f6c 696e 674e 6f64 6573 2901  ..PoolingNodes).
+000001f0: da14 506f 6f6c 696e 6757 6569 6768 7465  ..PoolingWeighte
+00000200: 644e 6f64 6573 2901 da15 7072 6f63 6573  dNodes)...proces
+00000210: 735f 6772 6170 685f 6461 7461 7365 7429  s_graph_dataset)
+00000220: 01da 2145 7870 6c61 6e61 7469 6f6e 5370  ..!ExplanationSp
+00000230: 6172 7369 7479 5265 6775 6c61 7269 7a61  arsityRegulariza
+00000240: 7469 6f6e 2901 da13 4d75 6c74 6948 6561  tion)...MultiHea
+00000250: 6447 4154 5632 4c61 7965 7229 01da 036d  dGATV2Layer)...m
+00000260: 6165 2901 da03 6263 6529 01da 0f73 6869  ae)...bce)...shi
+00000270: 6674 6564 5f73 6967 6d6f 6964 6300 0000  fted_sigmoidc...
+00000280: 0000 0000 0000 0000 0000 0000 0033 0000  .............3..
+00000290: 0000 0000 0073 ae01 0000 6500 5a01 6400  .....s....e.Z.d.
+000002a0: 5a02 6401 5a03 6402 6403 6404 6403 6700  Z.d.Z.d.d.d.d.g.
+000002b0: 6405 6406 6404 6404 6407 6408 6404 6403  d.d.d.d.d.d.d.d.
+000002c0: 6409 640a 6701 6404 640b 640c 6408 6408  d.d.g.d.d.d.d.d.
+000002d0: 6408 6408 6403 6409 6618 640d 6504 6a05  d.d.d.d.f.d.e.j.
+000002e0: 6506 1900 640e 6507 640f 6508 6410 6509  e...d.e.d.e.d.e.
+000002f0: 6411 6508 6412 6504 6a05 6506 1900 6413  d.e.d.e.j.e...d.
+00000300: 6506 6414 6507 6415 6509 6416 6509 6417  e.d.e.d.e.d.e.d.
+00000310: 6509 6418 6504 6a0a 6504 6a05 650b 6a0c  e.d.e.j.e.j.e.j.
+00000320: 6a0d 1900 1900 6419 6509 641a 6508 641b  j.....d.e.d.e.d.
+00000330: 6508 641c 6504 6a05 6506 1900 641d 6509  e.d.e.j.e...d.e.
+00000340: 641e 6507 641f 6507 6420 6504 6a0a 6504  d.e.d.e.d e.j.e.
+00000350: 6a0e 6509 6509 6602 1900 1900 6421 6504  j.e.e.f.....d!e.
+00000360: 6a0a 6504 6a0e 6509 6509 6602 1900 1900  j.e.j.e.e.f.....
+00000370: 6422 6504 6a0a 6504 6a05 6504 6a0e 6509  d"e.j.e.j.e.j.e.
+00000380: 6509 6602 1900 1900 1900 6423 6504 6a0a  e.f.......d#e.j.
+00000390: 6509 1900 6424 6508 6425 6508 6632 6426  e...d$e.d%e.f2d&
+000003a0: 6427 8405 5a0f 8700 6601 6428 6429 8408  d'..Z...f.d(d)..
+000003b0: 5a10 6511 642a 6508 6602 642b 642c 8404  Z.e.d*e.f.d+d,..
+000003c0: 8301 5a12 642a 6508 6602 642d 642e 8404  ..Z.d*e.f.d-d...
+000003d0: 5a13 0909 0909 0908 6440 642f 6508 6424  Z.......d@d/e.d$
+000003e0: 6508 6430 6504 6a0a 6514 6a15 1900 6606  e.d0e.j.e.j...f.
+000003f0: 6431 6432 8405 5a16 6433 6434 8400 5a17  d1d2..Z.d3d4..Z.
+00000400: 0903 6441 6435 6508 6602 6436 6437 8405  ..dAd5e.f.d6d7..
+00000410: 5a18 6438 6439 8400 5a19 643a 6504 6a05  Z.d8d9..Z.d:e.j.
+00000420: 651a 6a1b 1900 6602 643b 643c 8404 5a1c  e.j...f.d;d<..Z.
+00000430: 643d 651a 6a1b 6602 643e 643f 8404 5a1d  d=e.j.f.d>d?..Z.
+00000440: 8700 0400 5a1e 5300 2942 da05 4d65 6761  ....Z.S.)B..Mega
+00000450: 6e61 3c02 0000 0a20 2020 204d 4547 414e  na<....    MEGAN
+00000460: 3a20 4d75 6c74 6920 4578 706c 616e 6174  : Multi Explanat
+00000470: 696f 6e20 4772 6170 6820 4174 7465 6e74  ion Graph Attent
+00000480: 696f 6e20 4e65 7477 6f72 6b0a 2020 2020  ion Network.    
+00000490: 5468 6973 206d 6f64 656c 2063 7572 7265  This model curre
+000004a0: 6e74 6c79 2073 7570 706f 7274 7320 6772  ntly supports gr
+000004b0: 6170 6820 7265 6772 6573 7369 6f6e 2061  aph regression a
+000004c0: 6e64 2067 7261 7068 2063 6c61 7373 6966  nd graph classif
+000004d0: 6963 6174 696f 6e20 7072 6f62 6c65 6d73  ication problems
+000004e0: 2e20 4974 2077 6173 206d 6169 6e6c 7920  . It was mainly 
+000004f0: 6465 7369 676e 6564 0a20 2020 2077 6974  designed.    wit
+00000500: 6820 6120 666f 6375 7320 6f6e 2065 7870  h a focus on exp
+00000510: 6c61 696e 6162 6c65 2041 4920 2858 4149  lainable AI (XAI
+00000520: 292e 2041 6c6f 6e67 2074 6865 206d 6169  ). Along the mai
+00000530: 6e20 7072 6564 6963 7469 6f6e 2c20 7468  n prediction, th
+00000540: 6973 206d 6f64 656c 2069 7320 6162 6c65  is model is able
+00000550: 2074 6f20 6f75 7470 7574 206d 756c 7469   to output multi
+00000560: 706c 650a 2020 2020 6174 7465 6e74 696f  ple.    attentio
+00000570: 6e2d 6261 7365 6420 6578 706c 616e 6174  n-based explanat
+00000580: 696f 6e73 2066 6f72 2074 6861 7420 7072  ions for that pr
+00000590: 6564 6963 7469 6f6e 2e20 4d6f 7265 2073  ediction. More s
+000005a0: 7065 6369 6669 6361 6c6c 792c 2074 6865  pecifically, the
+000005b0: 206d 6f64 656c 206f 7574 7075 7473 206e   model outputs n
+000005c0: 6f64 6520 616e 6420 6564 6765 0a20 2020  ode and edge.   
+000005d0: 2061 7474 7269 6275 7469 6f6e 616c 2065   attributional e
+000005e0: 7870 6c61 6e61 7469 6f6e 7320 2861 7373  xplanations (ass
+000005f0: 6967 6e69 6e67 205b 302c 2031 5d20 7661  igning [0, 1] va
+00000600: 6c75 6573 2074 6f20 6576 6572 206e 6f64  lues to ever nod
+00000610: 6520 2f20 6564 6765 206f 6620 7468 6520  e / edge of the 
+00000620: 696e 7075 7420 6772 6170 6829 2069 6e20  input graph) in 
+00000630: 4b0a 2020 2020 7365 7061 7261 7465 2065  K.    separate e
+00000640: 7870 6c61 6e61 7469 6f6e 2063 6861 6e6e  xplanation chann
+00000650: 656c 732c 2077 6865 7265 204b 2063 616e  els, where K can
+00000660: 2062 6520 6368 6f73 656e 2061 7320 616e   be chosen as an
+00000670: 2069 6e64 6570 656e 6465 6e74 206d 6f64   independent mod
+00000680: 656c 2070 6172 616d 6574 6572 2e0a 2020  el parameter..  
+00000690: 2020 fa10 6b67 636e 6e3e 6c65 616b 795f    ..kgcnn>leaky_
+000006a0: 7265 6c75 54e7 0000 0000 0000 0000 e902  reluT...........
+000006b0: 0000 00da 0773 6967 6d6f 6964 6700 0000  .....sigmoidg...
+000006c0: 0000 0024 404e 46e9 0100 0000 da06 6c69  ...$@NF.......li
+000006d0: 6e65 6172 da03 7375 6dda 0575 6e69 7473  near..sum..units
+000006e0: da0a 6163 7469 7661 7469 6f6e da08 7573  ..activation..us
+000006f0: 655f 6269 6173 da0c 6472 6f70 6f75 745f  e_bias..dropout_
+00000700: 7261 7465 da11 7573 655f 6564 6765 5f66  rate..use_edge_f
+00000710: 6561 7475 7265 73da 1069 6d70 6f72 7461  eatures..importa
+00000720: 6e63 655f 756e 6974 73da 1369 6d70 6f72  nce_units..impor
+00000730: 7461 6e63 655f 6368 616e 6e65 6c73 da15  tance_channels..
+00000740: 696d 706f 7274 616e 6365 5f61 6374 6976  importance_activ
+00000750: 6174 696f 6eda 1769 6d70 6f72 7461 6e63  ation..importanc
+00000760: 655f 6472 6f70 6f75 745f 7261 7465 da11  e_dropout_rate..
+00000770: 696d 706f 7274 616e 6365 5f66 6163 746f  importance_facto
+00000780: 72da 1569 6d70 6f72 7461 6e63 655f 6d75  r..importance_mu
+00000790: 6c74 6970 6c69 6572 da1a 696d 706f 7274  ltiplier..import
+000007a0: 616e 6365 5f74 7261 6e73 666f 726d 6174  ance_transformat
+000007b0: 696f 6e73 da0f 7370 6172 7369 7479 5f66  ions..sparsity_f
+000007c0: 6163 746f 72da 0c63 6f6e 6361 745f 6865  actor..concat_he
+000007d0: 6164 73da 1973 6570 6172 6174 655f 6578  ads..separate_ex
+000007e0: 706c 616e 6174 696f 6e5f 7374 6570 da0b  planation_step..
+000007f0: 6669 6e61 6c5f 756e 6974 73da 1266 696e  final_units..fin
+00000800: 616c 5f64 726f 706f 7574 5f72 6174 65da  al_dropout_rate.
+00000810: 1066 696e 616c 5f61 6374 6976 6174 696f  .final_activatio
+00000820: 6eda 0d66 696e 616c 5f70 6f6f 6c69 6e67  n..final_pooling
+00000830: da11 7265 6772 6573 7369 6f6e 5f6c 696d  ..regression_lim
+00000840: 6974 73da 1272 6567 7265 7373 696f 6e5f  its..regression_
+00000850: 7765 6967 6874 73da 0f72 6567 7265 7373  weights..regress
+00000860: 696f 6e5f 6269 6e73 da14 7265 6772 6573  ion_bins..regres
+00000870: 7369 6f6e 5f72 6566 6572 656e 6365 da12  sion_reference..
+00000880: 7265 7475 726e 5f69 6d70 6f72 7461 6e63  return_importanc
+00000890: 6573 da14 7573 655f 6772 6170 685f 6174  es..use_graph_at
+000008a0: 7472 6962 7574 6573 631a 0000 0000 0000  tributesc.......
+000008b0: 0000 0000 0021 0000 000a 0000 004b 0000  .....!.......K..
+000008c0: 0073 6203 0000 7400 6a01 6a02 6a03 7c00  .sb...t.j.j.j.|.
+000008d0: 6601 6900 7c1a a401 8e01 0100 7c01 7c00  f.i.|.......|.|.
+000008e0: 5f04 7c02 7c00 5f05 7c03 7c00 5f06 7c04  _.|.|._.|.|._.|.
+000008f0: 7c00 5f07 7c05 7c00 5f08 7c06 7c00 5f09  |._.|.|._.|.|._.
+00000900: 7c07 7c00 5f0a 7c08 7c00 5f0b 7c09 7c00  |.|._.|.|._.|.|.
+00000910: 5f0c 7c0a 7c00 5f0d 7c0b 7c00 5f0e 7c0c  _.|.|._.|.|._.|.
+00000920: 7c00 5f0f 7c0d 7c00 5f10 7c0e 7c00 5f11  |._.|.|._.|.|._.
+00000930: 7c10 7c00 5f12 7c11 7c00 5f13 7c12 7c00  |.|._.|.|._.|.|.
+00000940: 5f14 7c13 7c00 5f15 7c14 7c00 5f16 7c15  _.|.|._.|.|._.|.
+00000950: 7c00 5f17 7c17 7c00 5f18 7c16 7c00 5f19  |._.|.|._.|.|._.
+00000960: 7c18 7c00 5f1a 7c0f 7c00 5f1b 7c19 7c00  |.|._.|.|._.|.|.
+00000970: 5f1c 6700 7c00 5f1d 7c00 6a04 4400 5d18  _.g.|._.|.j.D.].
+00000980: 7d1b 741e 7c1b 7c00 6a0a 7c00 6a08 7c00  }.t.|.|.j.|.j.|.
+00000990: 6a05 7c00 6a06 6401 7c00 6a11 6402 8d07  j.|.j.d.|.j.d...
+000009a0: 7d1c 7c00 6a1d a01f 7c1c a101 0100 715c  }.|.j...|.....q\
+000009b0: 7420 7c00 6a07 6403 8d01 7c00 5f21 7422  t |.j.d...|._!t"
+000009c0: 7c00 6a10 6404 8d01 7c00 5f23 7424 7c00  |.j.d...|._#t$|.
+000009d0: 6a0b 6405 8d01 7c00 5f25 7426 6406 6407  j.d...|._%t&d.d.
+000009e0: 8d01 7c00 5f27 7428 6408 6409 640a 8d02  ..|._'t(d.d.d...
+000009f0: 7c00 5f29 7428 6408 640b 640a 8d02 7c00  |._)t(d.d.d...|.
+00000a00: 5f2a 742b 8300 7c00 5f2c 7c06 7c00 6a0a  _*t+..|._,|.|.j.
+00000a10: 6701 1700 7c00 5f2d 640c 640d 8400 7c06  g...|._-d.d...|.
+00000a20: 4400 8301 640e 6701 1700 7c00 5f2e 6700  D...d.g...|._.g.
+00000a30: 7c00 5f2f 7430 7c00 6a2d 7c00 6a2e 8302  |._/t0|.j-|.j...
+00000a40: 4400 5d11 5c02 7d1b 7d1d 7431 7c1b 7c1d  D.].\.}.}.t1|.|.
+00000a50: 7c03 640f 8d03 7d1c 7c00 6a2f a01f 7c1c  |.d...}.|.j/..|.
+00000a60: a101 0100 71be 7432 7c00 6a15 6410 8d01  ....q.t2|.j.d...
+00000a70: 7c00 5f33 7426 6406 6407 8d01 7c00 5f34  |._3t&d.d...|._4
+00000a80: 7420 7c00 6a13 6403 8d01 7c00 5f35 6411  t |.j.d...|._5d.
+00000a90: 640d 8400 7c00 6a12 4400 8301 7c00 5f36  d...|.j.D...|._6
+00000aa0: 7c00 6a14 7c00 6a36 6406 3c00 6412 640d  |.j.|.j6d.<.d.d.
+00000ab0: 8400 7c00 6a12 4400 8301 7c00 5f37 6401  ..|.j.D...|._7d.
+00000ac0: 7c00 6a37 6406 3c00 6700 7c00 5f38 7430  |.j7d.<.g.|._8t0
+00000ad0: 7c00 6a12 7c00 6a36 7c00 6a37 8303 4400  |.j.|.j6|.j7..D.
+00000ae0: 5d13 5c03 7d1b 7d1d 7d1e 7431 7c1b 7c1d  ].\.}.}.}.t1|.|.
+00000af0: 7c03 640f 8d03 7d1c 7c00 6a38 a01f 7c1c  |.d...}.|.j8..|.
+00000b00: a101 0100 9001 710d 7400 6a39 a03a a100  ......q.t.j9.:..
+00000b10: 7c00 5f3b 743c a03d 743e a101 7c00 5f3f  |._;t<.=t>..|._?
+00000b20: 7400 6a39 a040 a100 7c00 5f41 7400 6a39  t.j9.@..|._At.j9
+00000b30: a042 a100 7c00 5f43 743c a03d 7444 a101  .B..|._Ct<.=tD..
+00000b40: 7c00 5f45 7c00 6a18 6413 7501 9001 72ad  |._E|.j.d.u...r.
+00000b50: 7446 7c17 7447 7448 6602 8302 9001 7251  tF|.tGtHf.....rQ
+00000b60: 7c17 6701 7c00 5f18 7449 7c00 6a18 8301  |.g.|._.tI|.j...
+00000b70: 7d1f 7c00 6a17 6413 7501 9001 7262 7449  }.|.j.d.u...rbtI
+00000b80: 7c00 6a17 8301 7d20 6e15 7c00 6a16 6413  |.j...} n.|.j.d.
+00000b90: 7501 9001 726e 7449 7c00 6a16 8301 7d20  u...rntI|.j...} 
+00000ba0: 6e09 744a 6414 7c00 6a18 9b00 6415 9d03  n.tJd.|.j...d...
+00000bb0: 8301 8201 7c1f 6416 1400 7c07 6b02 9001  ....|.d...|.k...
+00000bc0: 7389 4a00 6417 7c1f 9b00 6418 7c07 9b00  s.J.d.|...d.|...
+00000bd0: 6419 9d05 8301 8201 7c1f 7c10 6406 1900  d.......|.|.d...
+00000be0: 6b02 9001 739d 4a00 641a 7c1f 9b00 641b  k...s.J.d.|...d.
+00000bf0: 7c10 6406 1900 9b00 641c 9d05 8301 8201  |.d.....d.......
+00000c00: 7c1f 7c20 6b02 9001 73af 4a00 641a 7c1f  |.| k...s.J.d.|.
+00000c10: 9b00 641d 7c20 9b00 641c 9d05 8301 8201  ..d.| ..d.......
+00000c20: 6413 5300 6413 5300 291e 6125 0f00 000a  d.S.d.S.).a%....
+00000c30: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
+00000c40: 2020 2020 2020 2020 2020 756e 6974 733a            units:
+00000c50: 2041 206c 6973 7420 6f66 2069 6e74 7320   A list of ints 
+00000c60: 7768 6572 6520 6561 6368 2065 6c65 6d65  where each eleme
+00000c70: 6e74 2063 6f6e 6669 6775 7265 7320 616e  nt configures an
+00000c80: 2061 6464 6974 696f 6e61 6c20 6174 7465   additional atte
+00000c90: 6e74 696f 6e20 6c61 7965 722e 2054 6865  ntion layer. The
+00000ca0: 206e 756d 6572 6963 0a20 2020 2020 2020   numeric.       
+00000cb0: 2020 2020 2020 2020 2076 616c 7565 2064           value d
+00000cc0: 6574 6572 6d69 6e65 7320 7468 6520 6e75  etermines the nu
+00000cd0: 6d62 6572 206f 6620 6869 6464 656e 2075  mber of hidden u
+00000ce0: 6e69 7473 2074 6f20 6265 2075 7365 6420  nits to be used 
+00000cf0: 696e 2074 6865 2061 7474 656e 7469 6f6e  in the attention
+00000d00: 2068 6561 6473 206f 6620 7468 6174 206c   heads of that l
+00000d10: 6179 6572 0a20 2020 2020 2020 2020 2020  ayer.           
+00000d20: 2061 6374 6976 6174 696f 6e3a 2054 6865   activation: The
+00000d30: 2061 6374 6976 6174 696f 6e20 6675 6e63   activation func
+00000d40: 7469 6f6e 2074 6f20 6265 2075 7365 6420  tion to be used 
+00000d50: 7769 7468 696e 2074 6865 2061 7474 656e  within the atten
+00000d60: 7469 6f6e 206c 6179 6572 7320 6f66 2074  tion layers of t
+00000d70: 6865 206e 6574 776f 726b 0a20 2020 2020  he network.     
+00000d80: 2020 2020 2020 2075 7365 5f62 6961 733a         use_bias:
+00000d90: 2057 6865 7468 6572 2074 6865 206c 6179   Whether the lay
+00000da0: 6572 7320 6f66 2074 6865 206e 6574 776f  ers of the netwo
+00000db0: 726b 2073 686f 756c 6420 7573 6520 6269  rk should use bi
+00000dc0: 6173 2077 6569 6768 7473 2061 7420 616c  as weights at al
+00000dd0: 6c0a 2020 2020 2020 2020 2020 2020 6472  l.            dr
+00000de0: 6f70 6f75 745f 7261 7465 3a20 5468 6520  opout_rate: The 
+00000df0: 6472 6f70 6f75 7420 7261 7465 2074 6f20  dropout rate to 
+00000e00: 6265 2061 7070 6c69 6564 2061 6674 6572  be applied after
+00000e10: 202a 6561 6368 2a20 6f66 2074 6865 2061   *each* of the a
+00000e20: 7474 656e 7469 6f6e 206c 6179 6572 7320  ttention layers 
+00000e30: 6f66 2074 6865 206e 6574 776f 726b 2e0a  of the network..
+00000e40: 2020 2020 2020 2020 2020 2020 7573 655f              use_
+00000e50: 6564 6765 5f66 6561 7475 7265 733a 2057  edge_features: W
+00000e60: 6865 7468 6572 2065 6467 6520 6665 6174  hether edge feat
+00000e70: 7572 6573 2073 686f 756c 6420 6265 2075  ures should be u
+00000e80: 7365 642e 2047 656e 6572 616c 6c79 2074  sed. Generally t
+00000e90: 6865 206e 6574 776f 726b 2073 7570 706f  he network suppo
+00000ea0: 7274 7320 7468 650a 2020 2020 2020 2020  rts the.        
+00000eb0: 2020 2020 2020 2020 7573 6167 6520 6f66          usage of
+00000ec0: 2065 6467 6520 6665 6174 7572 6573 2c20   edge features, 
+00000ed0: 6275 7420 6966 2074 6865 2069 6e70 7574  but if the input
+00000ee0: 2064 6174 6120 646f 6573 206e 6f74 2063   data does not c
+00000ef0: 6f6e 7461 696e 2065 6467 6520 6665 6174  ontain edge feat
+00000f00: 7572 6573 2c20 7468 6973 2073 686f 756c  ures, this shoul
+00000f10: 6420 6265 0a20 2020 2020 2020 2020 2020  d be.           
+00000f20: 2020 2020 2073 6574 2074 6f20 4661 6c73       set to Fals
+00000f30: 652e 0a20 2020 2020 2020 2020 2020 2069  e..            i
+00000f40: 6d70 6f72 7461 6e63 655f 756e 6974 733a  mportance_units:
+00000f50: 2041 206c 6973 7420 6f66 2069 6e74 7320   A list of ints 
+00000f60: 7768 6572 6520 6561 6368 2065 6c65 6d65  where each eleme
+00000f70: 6e74 2063 6f6e 6669 6775 7265 7320 616e  nt configures an
+00000f80: 6f74 6865 7220 6465 6e73 6520 6c61 7965  other dense laye
+00000f90: 7220 696e 2074 6865 0a20 2020 2020 2020  r in the.       
+00000fa0: 2020 2020 2020 2020 2073 7562 6e65 7477           subnetw
+00000fb0: 6f72 6b20 7468 6174 2070 726f 6475 6365  ork that produce
+00000fc0: 7320 7468 6520 6e6f 6465 2069 6d70 6f72  s the node impor
+00000fd0: 7461 6e63 6520 7465 6e73 6f72 2066 726f  tance tensor fro
+00000fe0: 6d20 7468 6520 6d61 696e 206e 6f64 6520  m the main node 
+00000ff0: 656d 6265 6464 696e 6773 2e20 5468 650a  embeddings. The.
+00001000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001010: 6e75 6d65 7269 6320 7661 6c75 6520 6465  numeric value de
+00001020: 7465 726d 696e 6573 2074 6865 206e 756d  termines the num
+00001030: 6265 7220 6f66 2068 6964 6465 6e20 756e  ber of hidden un
+00001040: 6974 7320 696e 2074 6861 7420 6c61 7965  its in that laye
+00001050: 722e 0a20 2020 2020 2020 2020 2020 2069  r..            i
+00001060: 6d70 6f72 7461 6e63 655f 6368 616e 6e65  mportance_channe
+00001070: 6c73 3a20 5468 6520 696e 7420 6e75 6d62  ls: The int numb
+00001080: 6572 206f 6620 6578 706c 616e 6174 696f  er of explanatio
+00001090: 6e20 6368 616e 6e65 6c73 2074 6f20 6265  n channels to be
+000010a0: 2070 726f 6475 6365 6420 6279 2074 6865   produced by the
+000010b0: 206e 6574 776f 726b 2e20 5468 6973 0a20   network. This. 
+000010c0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+000010d0: 7320 7468 6520 7661 6c75 6520 7265 6665  s the value refe
+000010e0: 7272 6564 2074 6f20 6173 2022 4b22 2e20  rred to as "K". 
+000010f0: 4e6f 7465 2074 6861 7420 7468 6973 2077  Note that this w
+00001100: 696c 6c20 616c 736f 2064 6574 6572 6d69  ill also determi
+00001110: 6e65 2074 6865 206e 756d 6265 7220 6f66  ne the number of
+00001120: 2061 7474 656e 7469 6f6e 0a20 2020 2020   attention.     
+00001130: 2020 2020 2020 2020 2020 2068 6561 6473             heads
+00001140: 2075 7365 6420 7769 7468 696e 2074 6865   used within the
+00001150: 2061 7474 656e 7469 6f6e 2073 7562 6e65   attention subne
+00001160: 7477 6f72 6b2e 0a20 2020 2020 2020 2020  twork..         
+00001170: 2020 2069 6d70 6f72 7461 6e63 655f 6661     importance_fa
+00001180: 6374 6f72 3a20 5468 6520 7765 6967 6874  ctor: The weight
+00001190: 206f 6620 7468 6520 6578 706c 616e 6174   of the explanat
+000011a0: 696f 6e2d 6f6e 6c79 2074 7261 696e 2073  ion-only train s
+000011b0: 7465 702e 2049 6620 7468 6973 2069 7320  tep. If this is 
+000011c0: 7365 7420 746f 2065 7861 6374 6c79 0a20  set to exactly. 
+000011d0: 2020 2020 2020 2020 2020 2020 2020 207a                 z
+000011e0: 6572 6f20 7468 656e 2074 6865 2065 7870  ero then the exp
+000011f0: 6c61 6e61 7469 6f6e 2074 7261 696e 2073  lanation train s
+00001200: 7465 7020 7769 6c6c 206e 6f74 2062 6520  tep will not be 
+00001210: 6578 6563 7574 6564 2061 7420 616c 6c20  executed at all 
+00001220: 286c 6573 7320 636f 6d70 7574 6174 696f  (less computatio
+00001230: 6e61 6c6c 790a 2020 2020 2020 2020 2020  nally.          
+00001240: 2020 2020 2020 6578 7065 6e73 6976 6529        expensive)
+00001250: 0a20 2020 2020 2020 2020 2020 2069 6d70  .            imp
+00001260: 6f72 7461 6e63 655f 6d75 6c74 6970 6c69  ortance_multipli
+00001270: 6572 3a20 416e 2061 6464 6974 696f 6e61  er: An additiona
+00001280: 6c20 6879 7065 7270 6172 616d 6574 6572  l hyperparameter
+00001290: 206f 6620 7468 6520 6578 706c 616e 6174   of the explanat
+000012a0: 696f 6e2d 6f6e 6c79 2074 7261 696e 2073  ion-only train s
+000012b0: 7465 702e 2054 6869 730a 2020 2020 2020  tep. This.      
+000012c0: 2020 2020 2020 2020 2020 6973 2065 7373            is ess
+000012d0: 656e 7469 616c 6c79 2074 6865 2073 6361  entially the sca
+000012e0: 6c69 6e67 2066 6163 746f 7220 7468 6174  ling factor that
+000012f0: 2069 7320 6170 706c 6965 6420 746f 2074   is applied to t
+00001300: 6865 2076 616c 7565 7320 6f66 2074 6865  he values of the
+00001310: 2064 6174 6173 6574 2073 7563 6820 7468   dataset such th
+00001320: 6174 0a20 2020 2020 2020 2020 2020 2020  at.             
+00001330: 2020 2074 6865 2074 6172 6765 7420 7661     the target va
+00001340: 6c75 6573 2063 616e 2072 6561 736f 6e61  lues can reasona
+00001350: 626c 7920 6265 2061 7070 726f 7869 6d61  bly be approxima
+00001360: 7465 6420 6279 2061 2073 756d 206f 6620  ted by a sum of 
+00001370: 5b30 2c20 315d 2069 6d70 6f72 7461 6e63  [0, 1] importanc
+00001380: 6520 7661 6c75 6573 2e0a 2020 2020 2020  e values..      
+00001390: 2020 2020 2020 7370 6172 7369 7479 5f66        sparsity_f
+000013a0: 6163 746f 723a 2054 6865 2063 6f65 6666  actor: The coeff
+000013b0: 6963 6965 6e74 2066 6f72 2074 6865 2073  icient for the s
+000013c0: 7061 7273 6974 7920 7265 6775 6c61 7269  parsity regulari
+000013d0: 7a61 7469 6f6e 206f 6620 7468 6520 6e6f  zation of the no
+000013e0: 6465 2069 6d70 6f72 7461 6e63 650a 2020  de importance.  
+000013f0: 2020 2020 2020 2020 2020 2020 2020 7465                te
+00001400: 6e73 6f72 2e0a 2020 2020 2020 2020 2020  nsor..          
+00001410: 2020 636f 6e63 6174 5f68 6561 6473 3a20    concat_heads: 
+00001420: 5768 6574 6865 7220 746f 2063 6f6e 6361  Whether to conca
+00001430: 7420 7468 6520 6865 6164 7320 6f66 2074  t the heads of t
+00001440: 6865 2061 7474 656e 7469 6f6e 2073 7562  he attention sub
+00001450: 6e65 7477 6f72 6b2e 2054 6865 2064 6566  network. The def
+00001460: 6175 6c74 2069 7320 5472 7565 2e20 496e  ault is True. In
+00001470: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001480: 2074 6861 7420 6361 7365 2074 6865 206f   that case the o
+00001490: 7574 7075 7420 6f66 2065 6163 6820 696e  utput of each in
+000014a0: 6469 7669 6475 616c 2061 7474 656e 7469  dividual attenti
+000014b0: 6f6e 2068 6561 6420 6973 2063 6f6e 6361  on head is conca
+000014c0: 7465 6e61 7465 6420 616e 6420 7468 6520  tenated and the 
+000014d0: 636f 6e63 6174 656e 6174 6564 0a20 2020  concatenated.   
+000014e0: 2020 2020 2020 2020 2020 2020 2076 6563               vec
+000014f0: 746f 7220 6973 2074 6865 6e20 7573 6564  tor is then used
+00001500: 2061 7320 7468 6520 696e 7075 7420 6f66   as the input of
+00001510: 2074 6865 206e 6578 7420 6174 7465 6e74   the next attent
+00001520: 696f 6e20 6c61 7965 7227 7320 6865 6164  ion layer's head
+00001530: 732e 2049 6620 7468 6973 2069 7320 4661  s. If this is Fa
+00001540: 6c73 652c 2074 6865 0a20 2020 2020 2020  lse, the.       
+00001550: 2020 2020 2020 2020 2076 6563 746f 7273           vectors
+00001560: 2061 7265 2061 7665 7261 6765 2070 6f6f   are average poo
+00001570: 6c65 6420 696e 7374 6561 642e 0a20 2020  led instead..   
+00001580: 2020 2020 2020 2020 2066 696e 616c 5f75           final_u
+00001590: 6e69 7473 3a20 4120 6c69 7374 206f 6620  nits: A list of 
+000015a0: 696e 7473 2077 6865 7265 2065 6163 6820  ints where each 
+000015b0: 656c 656d 656e 7420 636f 6e66 6967 7572  element configur
+000015c0: 6573 2061 6e6f 7468 6572 2064 656e 7365  es another dense
+000015d0: 206c 6179 6572 2069 6e20 7468 6520 4d4c   layer in the ML
+000015e0: 500a 2020 2020 2020 2020 2020 2020 2020  P.              
+000015f0: 2020 6174 2074 6865 2074 6169 6c20 656e    at the tail en
+00001600: 6420 6f66 2074 6865 206e 6574 776f 726b  d of the network
+00001610: 2e20 5468 6520 6e75 6d65 7269 6320 7661  . The numeric va
+00001620: 6c75 6520 6465 7465 726d 696e 6573 2074  lue determines t
+00001630: 6865 206e 756d 6265 7220 6f66 2074 6865  he number of the
+00001640: 2068 6964 6465 6e20 756e 6974 730a 2020   hidden units.  
+00001650: 2020 2020 2020 2020 2020 2020 2020 696e                in
+00001660: 2074 6861 7420 6c61 7965 722e 204e 6f74   that layer. Not
+00001670: 6520 7468 6174 2074 6865 2066 696e 616c  e that the final
+00001680: 2065 6c65 6d65 6e74 2069 6e20 7468 6973   element in this
+00001690: 206c 6973 7420 6861 7320 746f 2062 6520   list has to be 
+000016a0: 7468 6520 7361 6d65 2061 7320 7468 6520  the same as the 
+000016b0: 6469 6d65 6e73 696f 6e0a 2020 2020 2020  dimension.      
+000016c0: 2020 2020 2020 2020 2020 746f 2062 6520            to be 
+000016d0: 6578 7065 6374 6564 2066 6f72 2074 6865  expected for the
+000016e0: 2073 616d 706c 6573 206f 6620 7468 6520   samples of the 
+000016f0: 7472 6169 6e69 6e67 2064 6174 6173 6574  training dataset
+00001700: 210a 2020 2020 2020 2020 2020 2020 6669  !.            fi
+00001710: 6e61 6c5f 6472 6f70 6f75 745f 7261 7465  nal_dropout_rate
+00001720: 3a20 5468 6520 6472 6f70 6f75 7420 7261  : The dropout ra
+00001730: 7465 2074 6f20 6265 2061 7070 6c69 6564  te to be applied
+00001740: 2061 6674 6572 202a 6576 6572 792a 206c   after *every* l
+00001750: 6179 6572 206f 6620 7468 6520 6669 6e61  ayer of the fina
+00001760: 6c20 4d4c 502e 0a20 2020 2020 2020 2020  l MLP..         
+00001770: 2020 2066 696e 616c 5f61 6374 6976 6174     final_activat
+00001780: 696f 6e3a 2054 6865 2061 6374 6976 6174  ion: The activat
+00001790: 696f 6e20 746f 2062 6520 6170 706c 6965  ion to be applie
+000017a0: 6420 6174 2074 6865 2076 6572 7920 6c61  d at the very la
+000017b0: 7374 206c 6179 6572 206f 6620 7468 6520  st layer of the 
+000017c0: 4d4c 5020 746f 2070 726f 6475 6365 2074  MLP to produce t
+000017d0: 6865 0a20 2020 2020 2020 2020 2020 2020  he.             
+000017e0: 2020 2061 6374 7561 6c20 6f75 7470 7574     actual output
+000017f0: 206f 6620 7468 6520 6e65 7477 6f72 6b2e   of the network.
+00001800: 0a20 2020 2020 2020 2020 2020 2066 696e  .            fin
+00001810: 616c 5f70 6f6f 6c69 6e67 3a20 5468 6520  al_pooling: The 
+00001820: 706f 6f6c 696e 6720 6d65 7468 6f64 2074  pooling method t
+00001830: 6f20 6265 2075 7365 6420 6475 7269 6e67  o be used during
+00001840: 2074 6865 2067 6c6f 6261 6c20 706f 6f6c   the global pool
+00001850: 696e 6720 7068 6173 6520 696e 2074 6865  ing phase in the
+00001860: 206e 6574 776f 726b 2e0a 2020 2020 2020   network..      
+00001870: 2020 2020 2020 7265 6772 6573 7369 6f6e        regression
+00001880: 5f6c 696d 6974 733a 2041 2074 7570 6c65  _limits: A tuple
+00001890: 2077 6865 7265 2074 6865 2066 6972 7374   where the first
+000018a0: 2076 616c 7565 2069 7320 7468 6520 6c6f   value is the lo
+000018b0: 7765 7220 6c69 6d69 7420 666f 7220 7468  wer limit for th
+000018c0: 6520 6578 7065 6374 6564 2076 616c 7565  e expected value
+000018d0: 2072 616e 6765 0a20 2020 2020 2020 2020   range.         
+000018e0: 2020 2020 2020 206f 6620 7468 6520 7265         of the re
+000018f0: 6772 6573 7369 6f6e 2074 6173 6b20 616e  gression task an
+00001900: 6420 7465 6820 7365 636f 6e64 2076 616c  d teh second val
+00001910: 7565 2074 6865 2075 7070 6572 206c 696d  ue the upper lim
+00001920: 6974 2e0a 2020 2020 2020 2020 2020 2020  it..            
+00001930: 7265 6772 6573 7369 6f6e 5f72 6566 6572  regression_refer
+00001940: 656e 6365 3a20 4120 7265 6665 7265 6e63  ence: A referenc
+00001950: 6520 7661 6c75 6520 7768 6963 6820 6973  e value which is
+00001960: 2069 6e73 6964 6520 7468 6520 7261 6e67   inside the rang
+00001970: 6520 6f66 2065 7870 6563 7465 6420 7661  e of expected va
+00001980: 6c75 6573 2028 6265 7374 2069 660a 2020  lues (best if.  
+00001990: 2020 2020 2020 2020 2020 2020 2020 6974                it
+000019a0: 2077 6173 2069 6e20 7468 6520 6d69 6464   was in the midd
+000019b0: 6c65 2c20 6275 7420 646f 6573 206e 6f74  le, but does not
+000019c0: 2068 6176 6520 746f 292e 2043 686f 6f73   have to). Choos
+000019d0: 696e 6720 6469 6666 6572 656e 7420 7265  ing different re
+000019e0: 6665 7265 6e63 6573 2077 696c 6c20 7265  ferences will re
+000019f0: 7375 6c74 0a20 2020 2020 2020 2020 2020  sult.           
+00001a00: 2020 2020 2069 6e20 6469 6666 6572 656e       in differen
+00001a10: 7420 6578 706c 616e 6174 696f 6e73 2e0a  t explanations..
+00001a20: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00001a30: 726e 5f69 6d70 6f72 7461 6e63 6573 3a20  rn_importances: 
+00001a40: 5768 6574 6865 7220 7468 6520 696d 706f  Whether the impo
+00001a50: 7274 616e 6365 202f 2065 7870 6c61 6e61  rtance / explana
+00001a60: 7469 6f6e 2074 656e 736f 7273 2073 686f  tion tensors sho
+00001a70: 756c 6420 6265 2072 6574 7572 6e65 6420  uld be returned 
+00001a80: 6173 2061 6e20 6f75 7470 7574 0a20 2020  as an output.   
+00001a90: 2020 2020 2020 2020 2020 2020 206f 6620               of 
+00001aa0: 7468 6520 6d6f 6465 6c2e 2049 6620 7468  the model. If th
+00001ab0: 6973 2069 7320 5472 7565 2c20 7468 6520  is is True, the 
+00001ac0: 6f75 7470 7574 206f 6620 7468 6520 6d6f  output of the mo
+00001ad0: 6465 6c20 7769 6c6c 2062 6520 6120 332d  del will be a 3-
+00001ae0: 7475 706c 653a 0a20 2020 2020 2020 2020  tuple:.         
+00001af0: 2020 2020 2020 2028 6f75 7470 7574 2c20         (output, 
+00001b00: 6e6f 6465 2069 6d70 6f72 7461 6e63 6573  node importances
+00001b10: 2c20 6564 6765 2069 6d70 6f72 7461 6e63  , edge importanc
+00001b20: 6573 292c 206f 7468 6572 7769 7365 2069  es), otherwise i
+00001b30: 7420 6973 206a 7573 7420 7468 6520 6f75  t is just the ou
+00001b40: 7470 7574 2069 7473 656c 660a 2020 2020  tput itself.    
+00001b50: 2020 2020 5429 0772 1b00 0000 da09 6e75      T).r......nu
+00001b60: 6d5f 6865 6164 7372 1f00 0000 721c 0000  m_headsr....r...
+00001b70: 0072 1d00 0000 da0e 6861 735f 7365 6c66  .r......has_self
+00001b80: 5f6c 6f6f 7073 7228 0000 0029 01da 0472  _loopsr(...)...r
+00001b90: 6174 6529 01da 0666 6163 746f 7229 0172  ate)...factor).r
+00001ba0: 1c00 0000 e9ff ffff ffa9 01da 0461 7869  .............axi
+00001bb0: 73da 046d 6561 6e72 0100 0000 2902 da0e  s..meanr....)...
+00001bc0: 706f 6f6c 696e 675f 6d65 7468 6f64 da0d  pooling_method..
+00001bd0: 706f 6f6c 696e 675f 696e 6465 7872 1800  pooling_indexr..
+00001be0: 0000 6301 0000 0000 0000 0000 0000 0002  ..c.............
+00001bf0: 0000 0003 0000 0053 0000 00f3 1000 0000  .......S........
+00001c00: 6700 7c00 5d04 7d01 6400 9102 7102 5300  g.|.].}.d...q.S.
+00001c10: a901 7214 0000 00a9 00a9 02da 022e 30da  ..r...........0.
+00001c20: 015f 7240 0000 0072 4000 0000 fa56 2f6d  ._r@...r@....V/m
+00001c30: 6564 6961 2f73 7364 2f50 726f 6772 616d  edia/ssd/Program
+00001c40: 6d69 6e67 2f67 7261 7068 5f61 7474 656e  ming/graph_atten
+00001c50: 7469 6f6e 5f73 7475 6465 6e74 2f67 7261  tion_student/gra
+00001c60: 7068 5f61 7474 656e 7469 6f6e 5f73 7475  ph_attention_stu
+00001c70: 6465 6e74 2f6d 6f64 656c 732f 6d65 6761  dent/models/mega
+00001c80: 6e2e 7079 da0a 3c6c 6973 7463 6f6d 703e  n.py..<listcomp>
+00001c90: a200 0000 f302 0000 0010 007a 224d 6567  ...........z"Meg
+00001ca0: 616e 2e5f 5f69 6e69 745f 5f2e 3c6c 6f63  an.__init__.<loc
+00001cb0: 616c 733e 2e3c 6c69 7374 636f 6d70 3e72  als>.<listcomp>r
+00001cc0: 1900 0000 2903 721b 0000 0072 1c00 0000  ....).r....r....
+00001cd0: 721d 0000 0029 0172 3c00 0000 6301 0000  r....).r<...c...
+00001ce0: 0000 0000 0000 0000 0002 0000 0003 0000  ................
+00001cf0: 0053 0000 0072 3e00 0000 723f 0000 0072  .S...r>...r?...r
+00001d00: 4000 0000 7241 0000 0072 4000 0000 7240  @...rA...r@...r@
+00001d10: 0000 0072 4400 0000 7245 0000 00b1 0000  ...rD...rE......
+00001d20: 0072 4600 0000 6301 0000 0000 0000 0000  .rF...c.........
+00001d30: 0000 0002 0000 0003 0000 0053 0000 0072  ...........S...r
+00001d40: 3e00 0000 a901 5472 4000 0000 7241 0000  >.....Tr@...rA..
+00001d50: 0072 4000 0000 7240 0000 0072 4400 0000  .r@...r@...rD...
+00001d60: 7245 0000 00b3 0000 0072 4600 0000 4e7a  rE.......rF...Nz
+00001d70: 3d59 6f75 2068 6176 6520 7375 7070 6c69  =You have suppli
+00001d80: 6564 2061 206e 6f6e 2d6e 756c 6c20 7661  ed a non-null va
+00001d90: 6c75 6520 666f 7220 7265 6772 6573 7369  lue for regressi
+00001da0: 6f6e 5f72 6566 6572 656e 6365 3a20 7a68  on_reference: zh
+00001db0: 2e20 5468 6174 206d 6561 6e73 2079 6f75  . That means you
+00001dc0: 206e 6565 6420 746f 2065 6974 6865 7220   need to either 
+00001dd0: 7375 7070 6c79 2061 2076 616c 6964 2076  supply a valid v
+00001de0: 616c 7565 2066 6f72 2072 6567 7265 7373  alue for regress
+00001df0: 696f 6e5f 6c69 6d69 7473 206f 7220 7265  ion_limits or re
+00001e00: 6772 6573 7369 6f6e 5f77 6569 6768 7473  gression_weights
+00001e10: 2061 7320 7765 6c6c 7216 0000 007a 4c66   as wellr....zLf
+00001e20: 6f72 2065 7870 6c61 6e61 7469 6f6e 2063  or explanation c
+00001e30: 6f2d 7472 6169 6e69 6e67 2c20 7468 6520  o-training, the 
+00001e40: 6e75 6d62 6572 206f 6620 7265 6772 6573  number of regres
+00001e50: 7369 6f6e 5f72 6566 6572 656e 6365 7320  sion_references 
+00001e60: 2863 7572 7265 6e74 6c79 207a 4629 2068  (currently zF) h
+00001e70: 6173 2074 6f20 6265 2065 7861 6374 6c79  as to be exactly
+00001e80: 2068 616c 6620 7468 6520 6e75 6d62 6572   half the number
+00001e90: 206f 6620 696d 706f 7274 616e 6365 2063   of importance c
+00001ea0: 6861 6e6e 656c 7320 2863 7572 7265 6e74  hannels (current
+00001eb0: 6c79 207a 0229 217a 4c46 6f72 2065 7870  ly z.)!zLFor exp
+00001ec0: 6c61 6e61 7469 6f6e 2063 6f2d 7472 6169  lanation co-trai
+00001ed0: 6e69 6e67 2c20 7468 6520 6e75 6d62 6572  ning, the number
+00001ee0: 206f 6620 7265 6772 6573 7369 6f6e 5f72   of regression_r
+00001ef0: 6566 6572 656e 6365 7320 2863 7572 7265  eferences (curre
+00001f00: 6e74 6c79 207a 5429 2068 6173 2074 6f20  ntly zT) has to 
+00001f10: 6265 2065 7861 6374 6c79 2074 6865 2073  be exactly the s
+00001f20: 616d 6520 6173 2074 6865 2066 696e 616c  ame as the final
+00001f30: 2075 6e69 7420 636f 756e 7420 696e 2074   unit count in t
+00001f40: 6865 204d 4c50 2074 6169 6c20 656e 6420  he MLP tail end 
+00001f50: 2863 7572 7265 6e74 6c79 20fa 0129 7a55  (currently ..)zU
+00001f60: 2920 6861 7320 746f 2062 6520 6578 6163  ) has to be exac
+00001f70: 746c 7920 7468 6520 7361 6d65 2061 7320  tly the same as 
+00001f80: 7468 6520 6e75 6d62 6572 206f 6620 7265  the number of re
+00001f90: 6772 6573 7369 6f6e 5f6c 696d 6974 7320  gression_limits 
+00001fa0: 696e 7465 7276 616c 7320 2863 7572 7265  intervals (curre
+00001fb0: 6e74 6c79 2029 4bda 026b 73da 066d 6f64  ntly )K..ks..mod
+00001fc0: 656c 73da 054d 6f64 656c da08 5f5f 696e  els..Model..__in
+00001fd0: 6974 5f5f 721b 0000 0072 1c00 0000 721d  it__r....r....r.
+00001fe0: 0000 0072 1e00 0000 721f 0000 0072 2000  ...r....r....r .
+00001ff0: 0000 7221 0000 0072 2200 0000 7223 0000  ..r!...r"...r#..
+00002000: 0072 2400 0000 7225 0000 0072 2600 0000  .r$...r%...r&...
+00002010: 7227 0000 0072 2800 0000 722a 0000 0072  r'...r(...r*...r
+00002020: 2b00 0000 722c 0000 0072 2d00 0000 722e  +...r,...r-...r.
+00002030: 0000 0072 2f00 0000 7231 0000 0072 3000  ...r/...r1...r0.
+00002040: 0000 7232 0000 0072 2900 0000 7233 0000  ..r2...r)...r3..
+00002050: 00da 1061 7474 656e 7469 6f6e 5f6c 6179  ...attention_lay
+00002060: 6572 7372 0f00 0000 da06 6170 7065 6e64  ersr......append
+00002070: 7209 0000 00da 0b6c 6179 5f64 726f 706f  r......lay_dropo
+00002080: 7574 720e 0000 00da 0c6c 6179 5f73 7061  utr......lay_spa
+00002090: 7273 6974 7972 0800 0000 da12 6c61 795f  rsityr......lay_
+000020a0: 6163 745f 696d 706f 7274 616e 6365 7205  act_importancer.
+000020b0: 0000 00da 116c 6179 5f63 6f6e 6361 745f  .....lay_concat_
+000020c0: 616c 7068 6173 720a 0000 00da 116c 6179  alphasr......lay
+000020d0: 5f70 6f6f 6c5f 6564 6765 735f 696e da12  _pool_edges_in..
+000020e0: 6c61 795f 706f 6f6c 5f65 6467 6573 5f6f  lay_pool_edges_o
+000020f0: 7574 7206 0000 00da 0b6c 6179 5f61 7665  utr......lay_ave
+00002100: 7261 6765 da15 6e6f 6465 5f69 6d70 6f72  rage..node_impor
+00002110: 7461 6e63 655f 756e 6974 73da 146e 6f64  tance_units..nod
+00002120: 655f 696d 706f 7274 616e 6365 5f61 6374  e_importance_act
+00002130: 73da 166e 6f64 655f 696d 706f 7274 616e  s..node_importan
+00002140: 6365 5f6c 6179 6572 73da 037a 6970 7207  ce_layers..zipr.
+00002150: 0000 0072 0b00 0000 da0c 6c61 795f 706f  ...r......lay_po
+00002160: 6f6c 5f6f 7574 da0e 6c61 795f 636f 6e63  ol_out..lay_conc
+00002170: 6174 5f6f 7574 da11 6c61 795f 6669 6e61  at_out..lay_fina
+00002180: 6c5f 6472 6f70 6f75 74da 0a66 696e 616c  l_dropout..final
+00002190: 5f61 6374 73da 0c66 696e 616c 5f62 6961  _acts..final_bia
+000021a0: 7365 73da 0c66 696e 616c 5f6c 6179 6572  ses..final_layer
+000021b0: 73da 066c 6f73 7365 73da 1242 696e 6172  s..losses..Binar
+000021c0: 7943 726f 7373 656e 7472 6f70 79da 0862  yCrossentropy..b
+000021d0: 6365 5f6c 6f73 7372 0200 0000 da0f 4c6f  ce_lossr......Lo
+000021e0: 7373 6573 436f 6e74 6169 6e65 7272 1100  ssesContainerr..
+000021f0: 0000 da1c 636f 6d70 696c 6564 5f63 6c61  ....compiled_cla
+00002200: 7373 6966 6963 6174 696f 6e5f 6c6f 7373  ssification_loss
+00002210: da10 4d65 616e 5371 7561 7265 6445 7272  ..MeanSquaredErr
+00002220: 6f72 da08 6d73 655f 6c6f 7373 da11 4d65  or..mse_loss..Me
+00002230: 616e 4162 736f 6c75 7465 4572 726f 72da  anAbsoluteError.
+00002240: 086d 6165 5f6c 6f73 7372 1000 0000 da18  .mae_lossr......
+00002250: 636f 6d70 696c 6564 5f72 6567 7265 7373  compiled_regress
+00002260: 696f 6e5f 6c6f 7373 da0a 6973 696e 7374  ion_loss..isinst
+00002270: 616e 6365 da03 696e 74da 0566 6c6f 6174  ance..int..float
+00002280: da03 6c65 6eda 0e41 7373 6572 7469 6f6e  ..len..Assertion
+00002290: 4572 726f 7229 21da 0473 656c 6672 1b00  Error)!..selfr..
+000022a0: 0000 721c 0000 0072 1d00 0000 721e 0000  ..r....r....r...
+000022b0: 0072 1f00 0000 7220 0000 0072 2100 0000  .r....r ...r!...
+000022c0: 7222 0000 0072 2300 0000 7224 0000 0072  r"...r#...r$...r
+000022d0: 2500 0000 7226 0000 0072 2700 0000 7228  %...r&...r'...r(
+000022e0: 0000 0072 2900 0000 722a 0000 0072 2b00  ...r)...r*...r+.
+000022f0: 0000 722c 0000 0072 2d00 0000 722e 0000  ..r,...r-...r...
+00002300: 0072 2f00 0000 7230 0000 0072 3100 0000  .r/...r0...r1...
+00002310: 7232 0000 0072 3300 0000 da06 6b77 6172  r2...r3.....kwar
+00002320: 6773 da01 75da 036c 6179 da03 6163 74da  gs..u..lay..act.
+00002330: 0462 6961 73da 0e6e 756d 5f72 6566 6572  .bias..num_refer
+00002340: 656e 6365 73da 0a6e 756d 5f76 616c 7565  ences..num_value
+00002350: 7372 4000 0000 7240 0000 0072 4400 0000  sr@...r@...rD...
+00002360: 724c 0000 0021 0000 0073 ce00 0000 164b  rL...!...s.....K
+00002370: 0601 0601 0601 0601 0601 0601 0601 0601  ................
+00002380: 0601 0601 0601 0601 0601 0601 0601 0601  ................
+00002390: 0601 0601 0601 0601 0601 0601 0601 0601  ................
+000023a0: 0601 0603 0a01 0201 0201 0401 0401 0401  ................
+000023b0: 0401 0201 0401 06f9 0e09 0e02 0e01 0e03  ................
+000023c0: 0c01 0e02 0e01 0801 0e03 1601 0601 1601  ................
+000023d0: 0201 0201 0201 0201 06fd 0e05 0e03 0c01  ................
+000023e0: 0e01 1202 0c01 1201 0a01 0601 1c01 0201  ................
+000023f0: 0201 0201 0201 06fd 1005 0c03 0c01 0c02  ................
+00002400: 0c01 0c01 0c07 1008 0801 0a02 0c02 0c01  ................
+00002410: 0c01 0c01 0402 0401 0aff 1004 0801 0201  ................
+00002420: 06ff 04ff 1004 0801 0601 06ff 04ff 0c04  ................
+00002430: 0801 0201 06ff 04ff 04e2 041e 7a0e 4d65  ............z.Me
+00002440: 6761 6e2e 5f5f 696e 6974 5f5f 6301 0000  gan.__init__c...
+00002450: 0000 0000 0000 0000 0002 0000 0009 0000  ................
+00002460: 0003 0000 0073 be00 0000 7400 7401 7c00  .....s....t.t.|.
+00002470: 8302 a002 a100 7d01 7c01 a003 6900 6401  ......}.|...i.d.
+00002480: 7c00 6a04 9301 6402 7c00 6a05 9301 6403  |.j...d.|.j...d.
+00002490: 7c00 6a06 9301 6404 7c00 6a07 9301 6405  |.j...d.|.j...d.
+000024a0: 7c00 6a08 9301 6406 7c00 6a09 9301 6407  |.j...d.|.j...d.
+000024b0: 7c00 6a0a 9301 6408 7c00 6a0b 9301 6409  |.j...d.|.j...d.
+000024c0: 7c00 6a0c 9301 640a 7c00 6a0d 9301 640b  |.j...d.|.j...d.
+000024d0: 7c00 6a0e 9301 640c 7c00 6a0f 9301 640d  |.j...d.|.j...d.
+000024e0: 7c00 6a10 9301 640e 7c00 6a11 9301 640f  |.j...d.|.j...d.
+000024f0: 7c00 6a12 9301 6410 7c00 6a13 9301 6411  |.j...d.|.j...d.
+00002500: 7c00 6a14 9301 7c00 6a15 7c00 6a16 7c00  |.j...|.j.|.j.|.
+00002510: 6a17 7c00 6a18 7c00 6a19 6412 9c05 a501  j.|.j.|.j.d.....
+00002520: a101 0100 7c01 5300 2913 4e72 1b00 0000  ....|.S.).Nr....
+00002530: 721c 0000 0072 1d00 0000 721e 0000 0072  r....r....r....r
+00002540: 1f00 0000 7220 0000 0072 2100 0000 7222  ....r ...r!...r"
+00002550: 0000 0072 2300 0000 7224 0000 0072 2500  ...r#...r$...r%.
+00002560: 0000 7227 0000 0072 2800 0000 722a 0000  ..r'...r(...r*..
+00002570: 0072 2b00 0000 722c 0000 0072 2d00 0000  .r+...r,...r-...
+00002580: 2905 722e 0000 0072 2f00 0000 7231 0000  ).r....r/...r1..
+00002590: 0072 3200 0000 7233 0000 0029 1ada 0573  .r2...r3...)...s
+000025a0: 7570 6572 7213 0000 00da 0a67 6574 5f63  uperr......get_c
+000025b0: 6f6e 6669 67da 0675 7064 6174 6572 1b00  onfig..updater..
+000025c0: 0000 721c 0000 0072 1d00 0000 721e 0000  ..r....r....r...
+000025d0: 0072 1f00 0000 7220 0000 0072 2100 0000  .r....r ...r!...
+000025e0: 7222 0000 0072 2300 0000 7224 0000 0072  r"...r#...r$...r
+000025f0: 2500 0000 7227 0000 0072 2800 0000 722a  %...r'...r(...r*
+00002600: 0000 0072 2b00 0000 722c 0000 0072 2d00  ...r+...r,...r-.
+00002610: 0000 722e 0000 0072 2f00 0000 7231 0000  ..r....r/...r1..
+00002620: 0072 3200 0000 7233 0000 0029 0272 6f00  .r2...r3...).ro.
+00002630: 0000 da06 636f 6e66 6967 a901 da09 5f5f  ....config....__
+00002640: 636c 6173 735f 5f72 4000 0000 7244 0000  class__r@...rD..
+00002650: 0072 7800 0000 ee00 0000 7356 0000 000e  .rx.......sV....
+00002660: 0106 0106 0102 ff06 0202 fe06 0302 fd06  ................
+00002670: 0402 fc06 0502 fb06 0602 fa06 0702 f906  ................
+00002680: 0802 f806 0902 f706 0a02 f606 0b02 f506  ................
+00002690: 0c02 f406 0d02 f306 0e02 f206 0f02 f106  ................
+000026a0: 1002 f006 1102 ef04 1204 0104 0104 0104  ................
+000026b0: 010a ea04 197a 104d 6567 616e 2e67 6574  .....z.Megan.get
+000026c0: 5f63 6f6e 6669 67da 0672 6574 7572 6e63  _config..returnc
+000026d0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+000026e0: 0200 0000 4300 0000 7314 0000 007c 006a  ....C...s....|.j
+000026f0: 0064 0075 0170 097c 006a 0164 0075 0153  .d.u.p.|.j.d.u.S
+00002700: 00a9 014e 2902 722e 0000 0072 2f00 0000  ...N).r....r/...
+00002710: a901 726f 0000 0072 4000 0000 7240 0000  ..ro...r@...r@..
+00002720: 0072 4400 0000 da10 646f 696e 675f 7265  .rD.....doing_re
+00002730: 6772 6573 7369 6f6e 0d01 0000 7302 0000  gression....s...
+00002740: 0014 027a 164d 6567 616e 2e64 6f69 6e67  ...z.Megan.doing
+00002750: 5f72 6567 7265 7373 696f 6e63 0100 0000  _regressionc....
+00002760: 0000 0000 0000 0000 0100 0000 0200 0000  ................
+00002770: 4300 0000 730a 0000 007c 006a 0064 0075  C...s....|.j.d.u
+00002780: 0153 0072 7e00 0000 2901 722f 0000 0072  .S.r~...).r/...r
+00002790: 7f00 0000 7240 0000 0072 4000 0000 7244  ....r@...r@...rD
+000027a0: 0000 00da 1864 6f69 6e67 5f72 6567 7265  .....doing_regre
+000027b0: 7373 696f 6e5f 7765 6967 6874 7311 0100  ssion_weights...
+000027c0: 0073 0200 0000 0a01 7a1e 4d65 6761 6e2e  .s......z.Megan.
+000027d0: 646f 696e 675f 7265 6772 6573 7369 6f6e  doing_regression
+000027e0: 5f77 6569 6768 7473 da08 7472 6169 6e69  _weights..traini
+000027f0: 6e67 da15 6e6f 6465 5f69 6d70 6f72 7461  ng..node_importa
+00002800: 6e63 6573 5f6d 6173 6b63 0500 0000 0000  nces_maskc......
+00002810: 0000 0000 0000 1e00 0000 0600 0000 4b00  ..............K.
+00002820: 0000 7328 0200 007c 006a 0072 0a7c 015c  ..s(...|.j.r.|.\
+00002830: 047d 067d 077d 087d 096e 077c 015c 037d  .}.}.}.}.n.|.\.}
+00002840: 067d 077d 0864 017d 0967 007d 0a7c 067d  .}.}.d.}.g.}.|.}
+00002850: 0b7c 006a 0144 005d 197d 0c7c 0c7c 0b7c  .|.j.D.].}.|.|.|
+00002860: 077c 0867 0383 015c 027d 0b7d 0d7c 0272  .|.g...\.}.}.|.r
+00002870: 2c7c 006a 027c 0b7c 0264 028d 027d 0b7c  ,|.j.|.|.d...}.|
+00002880: 0aa0 037c 0da1 0101 0071 187c 00a0 047c  ...|.....q.|...|
+00002890: 0aa1 017d 0a74 056a 067c 0a64 0364 0464  ...}.t.j.|.d.d.d
+000028a0: 058d 037d 0e7c 00a0 077c 0ea1 017d 0e7c  ...}.|...|...}.|
+000028b0: 00a0 087c 067c 0e7c 0867 03a1 017d 0f7c  ...|.|.|.g...}.|
+000028c0: 00a0 097c 067c 0e7c 0867 03a1 017d 107c  ...|.|.|.g...}.|
+000028d0: 00a0 0a7c 107c 0f67 02a1 017d 117c 0b7d  ...|.|.g...}.|.}
+000028e0: 127c 006a 0b44 005d 067d 0c7c 0c7c 1283  .|.j.D.].}.|.|..
+000028f0: 017d 1271 607c 00a0 077c 12a1 017d 127c  .}.q`|...|...}.|
+00002900: 127c 1114 007d 137c 00a0 0c7c 13a1 0101  .|...}.|...|....
+00002910: 007c 0464 0175 0172 8474 05a0 0d7c 0474  .|.d.u.r.t...|.t
+00002920: 056a 0ea1 027d 047c 137c 0414 007d 1367  .j...}.|.|...}.g
+00002930: 007d 147c 006a 0f64 0319 007d 1574 107c  .}.|.j.d...}.t.|
+00002940: 006a 1183 0144 005d 2e7d 1674 056a 127c  .j...D.].}.t.j.|
+00002950: 1364 0164 0185 0264 0164 0185 027c 1666  .d.d...d.d...|.f
+00002960: 0319 0064 0364 068d 027d 177c 0b7c 1714  ...d.d...}.|.|..
+00002970: 007d 187c 006a 1364 0175 0172 b47c 006a  .}.|.j.d.u.r.|.j
+00002980: 137c 1619 007d 197c 197c 1883 017d 187c  .|...}.|.|...}.|
+00002990: 00a0 147c 18a1 017d 1a7c 14a0 037c 1aa1  ...|...}.|...|..
+000029a0: 0101 0071 907c 00a0 157c 14a1 017d 1a7c  ...q.|...|...}.|
+000029b0: 006a 0072 ce7c 00a0 157c 1a7c 0967 02a1  .j.r.|...|.|.g..
+000029c0: 017d 1a74 167c 006a 1783 017d 1b74 187c  .}.t.|.j...}.t.|
+000029d0: 006a 1783 0144 005d 175c 027d 1c7d 0c7c  .j...D.].\.}.}.|
+000029e0: 0c7c 1a83 017d 1a7c 0272 ef7c 1c7c 1b64  .|...}.|.r.|.|.d
+000029f0: 0718 006b 0072 ef7c 006a 197c 1a7c 0264  ...k.r.|.j.|.|.d
+00002a00: 028d 027d 1a71 d87c 006a 1a90 0172 0674  ...}.q.|.j...r.t
+00002a10: 05a0 1b7c 1aa1 0174 056a 1c7c 006a 1d74  ...|...t.j.|.j.t
+00002a20: 056a 0e64 088d 0214 007d 1d7c 1a7c 1d17  .j.d.....}.|.|..
+00002a30: 007d 1a7c 006a 1e90 0173 0d7c 0390 0172  .}.|.j...s.|...r
+00002a40: 127c 1a7c 137c 0e66 0353 007c 1a53 0029  .|.|.|.f.S.|.S.)
+00002a50: 0961 b701 0000 0a20 2020 2020 2020 2046  .a.....        F
+00002a60: 6f72 7761 7264 2070 6173 7320 6f66 2074  orward pass of t
+00002a70: 6865 206d 6f64 656c 2e0a 0a20 2020 2020  he model...     
+00002a80: 2020 202a 2a53 6861 7065 2045 7870 6c61     **Shape Expla
+00002a90: 6e61 7469 6f6e 733a 2a2a 2041 6c6c 2073  nations:** All s
+00002aa0: 6861 7065 7320 696e 2062 7261 636b 6574  hapes in bracket
+00002ab0: 7320 5b5d 2061 7265 2072 6167 6765 6420  s [] are ragged 
+00002ac0: 6469 6d65 6e73 696f 6e73 210a 0a20 2020  dimensions!..   
+00002ad0: 2020 2020 202d 2056 3a20 4e75 6d20 6e6f       - V: Num no
+00002ae0: 6465 7320 696e 2074 6865 2067 7261 7068  des in the graph
+00002af0: 0a20 2020 2020 2020 202d 2045 3a20 4e75  .        - E: Nu
+00002b00: 6d20 6564 6765 7320 696e 2074 6865 2067  m edges in the g
+00002b10: 7261 7068 0a20 2020 2020 2020 202d 204e  raph.        - N
+00002b20: 3a20 4e75 6d20 6665 6174 7572 6520 7661  : Num feature va
+00002b30: 6c75 6573 2070 6572 206e 6f64 650a 2020  lues per node.  
+00002b40: 2020 2020 2020 2d20 4d3a 204e 556d 2066        - M: NUm f
+00002b50: 6561 7475 7265 2076 616c 7565 7320 7065  eature values pe
+00002b60: 7220 6564 6765 0a20 2020 2020 2020 202d  r edge.        -
+00002b70: 2048 3a20 4e75 6d20 6665 6174 7572 6520   H: Num feature 
+00002b80: 7661 6c75 6573 2070 6572 2067 7261 7068  values per graph
+00002b90: 0a20 2020 2020 2020 202d 2042 3a20 4e75  .        - B: Nu
+00002ba0: 6d20 6772 6170 6873 2069 6e20 6120 6261  m graphs in a ba
+00002bb0: 7463 680a 2020 2020 2020 2020 2d20 4b3a  tch.        - K:
+00002bc0: 204e 756d 2069 6d70 6f72 7461 6e63 6520   Num importance 
+00002bd0: 2865 7870 6c61 6e61 7469 6f6e 2920 6368  (explanation) ch
+00002be0: 616e 6e65 6c73 2063 6f6e 6669 6775 7265  annels configure
+00002bf0: 6420 696e 2074 6865 2063 6f6e 7374 7275  d in the constru
+00002c00: 6374 6f72 0a20 2020 2020 2020 204e 2901  ctor.        N).
+00002c10: 7282 0000 0072 3800 0000 4629 0272 3a00  r....r8...F).r:.
+00002c20: 0000 da08 6b65 6570 6469 6d73 7239 0000  ....keepdimsr9..
+00002c30: 0072 1600 0000 2901 da05 6474 7970 6529  .r....)...dtype)
+00002c40: 1f72 3300 0000 724d 0000 0072 4f00 0000  .r3...rM...rO...
+00002c50: 724e 0000 0072 5200 0000 da02 7466 da0a  rN...rR.....tf..
+00002c60: 7265 6475 6365 5f73 756d 7251 0000 0072  reduce_sumrQ...r
+00002c70: 5300 0000 7254 0000 0072 5500 0000 7258  S...rT...rU...rX
+00002c80: 0000 0072 5000 0000 da04 6361 7374 da07  ...rP.....cast..
+00002c90: 666c 6f61 7433 3272 2a00 0000 da05 7261  float32r*.....ra
+00002ca0: 6e67 6572 2100 0000 da0b 6578 7061 6e64  nger!.....expand
+00002cb0: 5f64 696d 7372 2600 0000 725a 0000 0072  _dimsr&...rZ...r
+00002cc0: 5b00 0000 726d 0000 0072 5f00 0000 da09  [...rm...r_.....
+00002cd0: 656e 756d 6572 6174 6572 5c00 0000 7280  enumerater\...r.
+00002ce0: 0000 00da 096f 6e65 735f 6c69 6b65 da08  .....ones_like..
+00002cf0: 636f 6e73 7461 6e74 7231 0000 0072 3200  constantr1...r2.
+00002d00: 0000 291e 726f 0000 00da 0669 6e70 7574  ..).ro.....input
+00002d10: 7372 8200 0000 7232 0000 0072 8300 0000  sr....r2...r....
+00002d20: 7270 0000 00da 0a6e 6f64 655f 696e 7075  rp.....node_inpu
+00002d30: 74da 0a65 6467 655f 696e 7075 74da 1065  t..edge_input..e
+00002d40: 6467 655f 696e 6465 785f 696e 7075 74da  dge_index_input.
+00002d50: 0b67 7261 7068 5f69 6e70 7574 da06 616c  .graph_input..al
+00002d60: 7068 6173 da01 7872 7200 0000 da05 616c  phas..xrr.....al
+00002d70: 7068 61da 1065 6467 655f 696d 706f 7274  pha..edge_import
+00002d80: 616e 6365 73da 0f70 6f6f 6c65 645f 6564  ances..pooled_ed
+00002d90: 6765 735f 696e da10 706f 6f6c 6564 5f65  ges_in..pooled_e
+00002da0: 6467 6573 5f6f 7574 da0c 706f 6f6c 6564  dges_out..pooled
+00002db0: 5f65 6467 6573 da16 6e6f 6465 5f69 6d70  _edges..node_imp
+00002dc0: 6f72 7461 6e63 6573 5f74 696c 6465 da10  ortances_tilde..
+00002dd0: 6e6f 6465 5f69 6d70 6f72 7461 6e63 6573  node_importances
+00002de0: da04 6f75 7473 da01 6eda 016b da15 6e6f  ..outs..n..k..no
+00002df0: 6465 5f69 6d70 6f72 7461 6e63 655f 736c  de_importance_sl
+00002e00: 6963 65da 116d 6173 6b65 645f 656d 6265  ice..masked_embe
+00002e10: 6464 696e 6773 da0d 6c61 795f 7472 616e  ddings..lay_tran
+00002e20: 7366 6f72 6dda 036f 7574 da10 6e75 6d5f  sform..out..num_
+00002e30: 6669 6e61 6c5f 6c61 7965 7273 da01 63da  final_layers..c.
+00002e40: 0972 6566 6572 656e 6365 7240 0000 0072  .referencer@...r
+00002e50: 4000 0000 7244 0000 00da 0463 616c 6c16  @...rD.....call.
+00002e60: 0100 0073 6600 0000 061f 0e01 0a02 0401  ...sf...........
+00002e70: 0405 0401 0a01 1203 0401 0e01 0c02 0a04  ................
+00002e80: 1001 0a01 1006 1001 0e01 0402 0a01 0a01  ................
+00002e90: 0a02 0802 0a01 0809 0e01 0801 0405 0a01  ................
+00002ea0: 0e01 2001 0801 0a05 0a01 0801 0a02 0c03  .. .............
+00002eb0: 0a03 0604 0e01 0a04 1201 0801 1001 0e01  ................
+00002ec0: 0280 0802 1c01 0801 0e05 0a01 0402 7a0a  ..............z.
+00002ed0: 4d65 6761 6e2e 6361 6c6c 6302 0000 0000  Megan.callc.....
+00002ee0: 0000 0000 0000 000d 0000 0009 0000 0043  ...............C
+00002ef0: 0000 0073 0c01 0000 6700 7d02 6700 7d03  ...s....g.}.g.}.
+00002f00: 7400 7c00 6a01 8301 4400 5d6e 5c02 7d04  t.|.j...D.]n\.}.
+00002f10: 7d05 7402 6a03 7c01 6400 6400 8502 7c04  }.t.j.|.d.d...|.
+00002f20: 6602 1900 6401 6402 8d02 7d06 7402 a004  f...d.d...}.t...
+00002f30: 7c06 7c05 1800 a101 7d07 7c00 6a05 7241  |.|.....}.|.j.rA
+00002f40: 7c00 6a06 7c04 1900 7d08 7402 a007 7c06  |.j.|...}.t...|.
+00002f50: 7c05 6b00 7c07 7c00 6a08 7c08 6403 1900  |.k.|.|.j.|.d...
+00002f60: 1400 1400 7c07 7c00 6a08 7c08 6404 1900  ....|.|.j.|.d...
+00002f70: 1400 1400 a103 7d07 6e18 7c00 6a09 7c04  ......}.n.|.j.|.
+00002f80: 1900 7d09 7404 7c09 6404 1900 7c09 6403  ..}.t.|.d...|.d.
+00002f90: 1900 1800 8301 7d0a 7c07 7c00 6a08 1400  ......}.|.|.j...
+00002fa0: 6405 7c0a 1400 1b00 7d07 7402 a007 7c06  d.|.....}.t...|.
+00002fb0: 7c05 6b00 6406 6407 a103 7d0b 7402 a007  |.k.d.d...}.t...
+00002fc0: 7c06 7c05 6b04 6406 6407 a103 7d0c 7c02  |.|.k.d.d...}.|.
+00002fd0: 7c07 7c07 6702 3700 7d02 7c03 7c0b 7c0c  |.|.g.7.}.|.|.|.
+00002fe0: 6702 3700 7d03 7109 7402 6a0a 7c02 6401  g.7.}.q.t.j.|.d.
+00002ff0: 6402 8d02 7402 6a0a 7c03 6401 6402 8d02  d...t.j.|.d.d...
+00003000: 6602 5300 2908 4e72 3800 0000 7239 0000  f.S.).Nr8...r9..
+00003010: 0072 0100 0000 7218 0000 0067 0000 0000  .r....r....g....
+00003020: 0000 e03f 6700 0000 0000 00f0 3f72 1500  ...?g.......?r..
+00003030: 0000 290b 728c 0000 0072 3100 0000 7286  ..).r....r1...r.
+00003040: 0000 0072 8b00 0000 da03 6162 7372 8100  ...r......absr..
+00003050: 0000 722f 0000 00da 0577 6865 7265 7225  ..r/.....wherer%
+00003060: 0000 0072 2e00 0000 da06 636f 6e63 6174  ...r......concat
+00003070: 290d 726f 0000 00da 086f 7574 5f74 7275  ).ro.....out_tru
+00003080: 65da 0773 616d 706c 6573 da05 6d61 736b  e..samples..mask
+00003090: 73da 0169 7231 0000 00da 0676 616c 7565  s..ir1.....value
+000030a0: 73da 1063 656e 7465 725f 6469 7374 616e  s..center_distan
+000030b0: 6365 7372 2f00 0000 722e 0000 00da 1072  cesr/...r......r
+000030c0: 6567 7265 7373 696f 6e5f 7769 6474 68da  egression_width.
+000030d0: 076c 6f5f 6d61 736b da07 6869 5f6d 6173  .lo_mask..hi_mas
+000030e0: 6b72 4000 0000 7240 0000 0072 4400 0000  kr@...r@...rD...
+000030f0: da17 7265 6772 6573 7369 6f6e 5f61 7567  ..regression_aug
+00003100: 6d65 6e74 6174 696f 6e9c 0100 0073 2c00  mentation....s,.
+00003110: 0000 0402 0401 1202 1a01 0e01 0602 0a01  ................
+00003120: 0401 0601 1001 1001 06fd 0a07 1401 1201  ................
+00003130: 1208 1202 0c02 0e01 0c03 0c01 04fe 7a1d  ..............z.
+00003140: 4d65 6761 6e2e 7265 6772 6573 7369 6f6e  Megan.regression
+00003150: 5f61 7567 6d65 6e74 6174 696f 6eda 0e75  _augmentation..u
+00003160: 7064 6174 655f 7765 6967 6874 7363 0400  pdate_weightsc..
+00003170: 0000 0000 0000 0000 0000 1300 0000 0800  ................
+00003180: 0000 4300 0000 733a 0100 007c 006a 0072  ..C...s:...|.j.r
+00003190: 097c 025c 037d 047d 057d 056e 027c 027d  .|.\.}.}.}.n.|.}
+000031a0: 0464 017d 0674 01a0 02a1 008f 6c7d 077c  .d.}.t......l}.|
+000031b0: 007c 0164 0264 0264 038d 037d 087c 085c  .|.d.d.d...}.|.\
+000031c0: 037d 097d 0a7d 0b67 007d 0c74 037c 006a  .}.}.}.g.}.t.|.j
+000031d0: 0483 0144 005d 1c7d 0d74 016a 057c 0a64  ...D.].}.t.j.|.d
+000031e0: 0064 0085 0264 0064 0085 027c 0d66 0319  .d...d.d...|.f..
+000031f0: 0064 0464 058d 027d 0e7c 00a0 067c 0ea1  .d.d...}.|...|..
+00003200: 017d 0f7c 0ca0 077c 0fa1 0101 0071 257c  .}.|...|.....q%|
+00003210: 00a0 087c 0ca1 017d 0c7c 006a 0972 617c  ...|...}.|.j.ra|
+00003220: 00a0 0a7c 04a1 015c 027d 047d 107c 0c7d  ...|...\.}.}.|.}
+00003230: 097c 006a 047c 00a0 0b7c 047c 1014 007c  .|.j.|...|.|...|
+00003240: 097c 1014 00a1 0214 007d 066e 1074 0c7c  .|.......}.n.t.|
+00003250: 0c7c 006a 0d64 0664 078d 037d 097c 00a0  .|.j.d.d...}.|..
+00003260: 0e7c 047c 097c 0414 00a1 027d 067c 067c  .|.|.|.....}.|.|
+00003270: 006a 0f39 007d 0657 0064 0004 0004 0083  .j.9.}.W.d......
+00003280: 0301 006e 0831 0073 8077 0101 0001 0001  ...n.1.s.w......
+00003290: 0059 0001 007c 006a 107d 117c 07a0 117c  .Y...|.j.}.|...|
+000032a0: 067c 11a1 027d 127c 0372 997c 006a 12a0  .|...}.|.r.|.j..
+000032b0: 1374 147c 127c 1183 02a1 0101 0064 087c  .t.|.|.......d.|
+000032c0: 0669 0153 0029 094e 7201 0000 0054 a902  .i.S.).Nr....T..
+000032d0: 7282 0000 0072 3200 0000 7238 0000 0072  r....r2...r8...r
+000032e0: 3900 0000 7216 0000 00a9 02da 0573 6869  9...r........shi
+000032f0: 6674 da0a 6d75 6c74 6970 6c69 6572 da08  ft..multiplier..
+00003300: 6578 705f 6c6f 7373 2915 7232 0000 0072  exp_loss).r2...r
+00003310: 8600 0000 da0c 4772 6164 6965 6e74 5461  ......GradientTa
+00003320: 7065 728a 0000 0072 2100 0000 728b 0000  per....r!...r...
+00003330: 0072 5a00 0000 724e 0000 0072 5b00 0000  .rZ...rN...r[...
+00003340: 7280 0000 0072 b400 0000 7269 0000 0072  r....r....ri...r
+00003350: 1200 0000 7225 0000 0072 6400 0000 7224  ....r%...rd...r$
+00003360: 0000 00da 1374 7261 696e 6162 6c65 5f76  .....trainable_v
+00003370: 6172 6961 626c 6573 da08 6772 6164 6965  ariables..gradie
+00003380: 6e74 da09 6f70 7469 6d69 7a65 72da 0f61  nt..optimizer..a
+00003390: 7070 6c79 5f67 7261 6469 656e 7473 7259  pply_gradientsrY
+000033a0: 0000 0029 1372 6f00 0000 7295 0000 00da  ...).ro...r.....
+000033b0: 0179 72b5 0000 0072 ab00 0000 7243 0000  .yr....r....rC..
+000033c0: 0072 ba00 0000 da04 7461 7065 da06 795f  .r......tape..y_
+000033d0: 7072 6564 da08 6f75 745f 7072 6564 da07  pred..out_pred..
+000033e0: 6e69 5f70 7265 64da 0765 695f 7072 6564  ni_pred..ei_pred
+000033f0: 729d 0000 0072 9f00 0000 da16 6e6f 6465  r....r......node
+00003400: 5f69 6d70 6f72 7461 6e63 6573 5f73 6c69  _importances_sli
+00003410: 6365 72a3 0000 00da 046d 6173 6bda 0e74  cer......mask..t
+00003420: 7261 696e 6162 6c65 5f76 6172 73da 0d65  rainable_vars..e
+00003430: 7870 5f67 7261 6469 656e 7473 7240 0000  xp_gradientsr@..
+00003440: 0072 4000 0000 7244 0000 00da 1674 7261  .r@...rD.....tra
+00003450: 696e 5f73 7465 705f 6578 706c 616e 6174  in_step_explanat
+00003460: 696f 6ec4 0100 0073 3800 0000 0603 0c01  ion....s8.......
+00003470: 0402 0402 0a01 0e02 0a01 0407 0e01 2001  .............. .
+00003480: 0a01 0c02 0a03 0602 0e01 0401 0e01 0601  ................
+00003490: 08ff 1005 1001 0c02 1ce1 0622 0c01 0403  ..........."....
+000034a0: 1201 0802 7a1c 4d65 6761 6e2e 7472 6169  ....z.Megan.trai
+000034b0: 6e5f 7374 6570 5f65 7870 6c61 6e61 7469  n_step_explanati
+000034c0: 6f6e 6302 0000 0000 0000 0000 0000 0018  onc.............
+000034d0: 0000 0008 0000 0043 0000 0073 d801 0000  .......C...s....
+000034e0: 7400 7c01 8301 6401 6b02 720c 7c01 5c03  t.|...d.k.r.|.\.
+000034f0: 7d02 7d03 7d04 6e06 6400 7d04 7c01 5c02  }.}.}.n.d.}.|.\.
+00003500: 7d02 7d03 7c00 6a01 6402 6b03 7221 7c00  }.}.|.j.d.k.r!|.
+00003510: 6a02 7221 7c00 a003 7c02 7c03 a102 7d05  j.r!|...|.|...}.
+00003520: 6e02 6900 7d05 6402 7d06 7404 a005 a100  n.i.}.d.}.t.....
+00003530: 8f8c 7d07 7c03 5c03 7d08 7d09 7d0a 7c00  ..}.|.\.}.}.}.|.
+00003540: 7c02 6403 6403 6404 8d03 5c03 7d0b 7d0c  |.d.d.d...\.}.}.
+00003550: 7d0d 7c00 6a06 7c08 7c09 7c0a 6703 7c0b  }.|.j.|.|.|.g.|.
+00003560: 7c0c 7c0d 6703 7c04 7c00 6a07 6405 8d04  |.|.g.|.|.j.d...
+00003570: 7d0e 7c00 6a01 6402 6b03 72ae 7c00 6a02  }.|.j.d.k.r.|.j.
+00003580: 73ae 6700 7d0f 7408 7c00 6a09 8301 4400  s.g.}.t.|.j...D.
+00003590: 5d1c 7d10 7404 6a0a 7c0c 6400 6400 8502  ].}.t.j.|.d.d...
+000035a0: 6400 6400 8502 7c10 6603 1900 6406 6407  d.d...|.f...d.d.
+000035b0: 8d02 7d11 7c00 a00b 7c11 a101 7d12 7c0f  ..}.|...|...}.|.
+000035c0: a00c 7c12 a101 0100 7158 7c00 a00d 7c0f  ..|.....qX|...|.
+000035d0: a101 7d0f 7c00 6a0e 7291 7c00 a00f 7c08  ..}.|.j.r.|...|.
+000035e0: a101 5c02 7d13 7d14 7c0f 7d15 7c00 a010  ..\.}.}.|.}.|...
+000035f0: 7c13 7c14 1400 7c15 7c14 1400 a102 7d06  |.|...|.|.....}.
+00003600: 6e10 7411 7c0f 7c00 6a12 6408 6409 8d03  n.t.|.|.j.d.d...
+00003610: 7c08 1400 7d15 7c00 a013 7c08 7c15 a102  |...}.|...|.|...
+00003620: 7d06 7c06 7c00 6a01 3900 7d06 7c06 7c05  }.|.|.j.9.}.|.|.
+00003630: 640a 3c00 7c0e 7c06 3700 7d0e 5700 6400  d.<.|.|.7.}.W.d.
+00003640: 0400 0400 8303 0100 6e08 3100 73b8 7701  ........n.1.s.w.
+00003650: 0100 0100 0100 5900 0100 7c00 6a14 7d16  ......Y...|.j.}.
+00003660: 7c07 a015 7c0e 7c16 a102 7d17 7c00 6a16  |...|.|...}.|.j.
+00003670: a017 7418 7c17 7c16 8302 a101 0100 7c00  ..t.|.|.......|.
+00003680: 6a19 6a1a 7c03 7c00 6a1b 73d8 7c0b 6e04  j.j.|.|.j.s.|.n.
+00003690: 7c0b 7c0c 7c0d 6703 7c04 640b 8d03 0100  |.|.|.g.|.d.....
+000036a0: 6900 640c 640d 8400 7c00 6a1c 4400 8301  i.d.d...|.j.D...
+000036b0: a501 7c05 a501 5300 290e 4ee9 0300 0000  ..|...S.).N.....
+000036c0: 7201 0000 0054 72b6 0000 0029 02da 0d73  r....Tr....)...s
+000036d0: 616d 706c 655f 7765 6967 6874 da15 7265  ample_weight..re
+000036e0: 6775 6c61 7269 7a61 7469 6f6e 5f6c 6f73  gularization_los
+000036f0: 7365 7372 3800 0000 7239 0000 0072 1800  sesr8...r9...r..
+00003700: 0000 72b7 0000 0072 ba00 0000 2901 72cc  ..r....r....).r.
+00003710: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
+00003720: 0200 0000 0500 0000 5300 0000 7318 0000  ........S...s...
+00003730: 0069 007c 005d 087d 017c 016a 007c 01a0  .i.|.].}.|.j.|..
+00003740: 01a1 0093 0271 0253 0072 4000 0000 2902  .....q.S.r@...).
+00003750: da04 6e61 6d65 da06 7265 7375 6c74 2902  ..name..result).
+00003760: 7242 0000 00da 016d 7240 0000 0072 4000  rB.....mr@...r@.
+00003770: 0000 7244 0000 00da 0a3c 6469 6374 636f  ..rD.....<dictco
+00003780: 6d70 3e46 0200 0073 0200 0000 1800 7a24  mp>F...s......z$
+00003790: 4d65 6761 6e2e 7472 6169 6e5f 7374 6570  Megan.train_step
+000037a0: 2e3c 6c6f 6361 6c73 3e2e 3c64 6963 7463  .<locals>.<dictc
+000037b0: 6f6d 703e 291d 726d 0000 0072 2400 0000  omp>).rm...r$...
+000037c0: 7229 0000 0072 ca00 0000 7286 0000 0072  r)...r....r....r
+000037d0: bb00 0000 da0d 636f 6d70 696c 6564 5f6c  ......compiled_l
+000037e0: 6f73 7372 6000 0000 728a 0000 0072 2100  ossr`...r....r!.
+000037f0: 0000 728b 0000 0072 5a00 0000 724e 0000  ..r....rZ...rN..
+00003800: 0072 5b00 0000 7280 0000 0072 b400 0000  .r[...r....r....
+00003810: 7269 0000 0072 1200 0000 7225 0000 0072  ri...r....r%...r
+00003820: 6400 0000 72bc 0000 0072 bd00 0000 72be  d...r....r....r.
+00003830: 0000 0072 bf00 0000 7259 0000 00da 1063  ...r....rY.....c
+00003840: 6f6d 7069 6c65 645f 6d65 7472 6963 73da  ompiled_metrics.
+00003850: 0c75 7064 6174 655f 7374 6174 6572 3200  .update_stater2.
+00003860: 0000 da07 6d65 7472 6963 7329 1872 6f00  ....metrics).ro.
+00003870: 0000 da04 6461 7461 7295 0000 0072 c000  ....datar....r..
+00003880: 0000 72cc 0000 00da 0b65 7870 5f6d 6574  ..r......exp_met
+00003890: 7269 6373 72ba 0000 0072 c100 0000 72ab  ricsr....r....r.
+000038a0: 0000 00da 076e 695f 7472 7565 da07 6569  .....ni_true..ei
+000038b0: 5f74 7275 6572 c300 0000 72c4 0000 0072  _truer....r....r
+000038c0: c500 0000 da04 6c6f 7373 729d 0000 0072  ......lossr....r
+000038d0: 9f00 0000 72c6 0000 0072 a300 0000 da09  ....r....r......
+000038e0: 5f6f 7574 5f74 7275 6572 c700 0000 da09  _out_truer......
+000038f0: 5f6f 7574 5f70 7265 6472 c800 0000 da09  _out_predr......
+00003900: 6772 6164 6965 6e74 7372 4000 0000 7240  gradientsr@...r@
+00003910: 0000 0072 4400 0000 da0a 7472 6169 6e5f  ...rD.....train_
+00003920: 7374 6570 f801 0000 7370 0000 000c 010c  step....sp......
+00003930: 0104 0208 0110 060e 0104 0204 020a 010a  ................
+00003940: 0214 0104 0108 0108 0102 0104 0106 fc10  ................
+00003950: 0704 060e 0120 010a 010c 020a 0306 020e  ..... ..........
+00003960: 0104 010a 0106 0106 ff02 0602 0104 0102  ................
+00003970: 0104 fd02 0404 fc0c 050a 0208 0108 0102  ................
+00003980: 801c d306 2f0c 0112 0206 0202 0112 0102  ..../...........
+00003990: 0106 fd02 080e 0102 ff02 0204 fe7a 104d  .............z.M
+000039a0: 6567 616e 2e74 7261 696e 5f73 7465 70da  egan.train_step.
+000039b0: 0a67 7261 7068 5f6c 6973 7463 0200 0000  .graph_listc....
+000039c0: 0000 0000 0000 0000 0500 0000 0700 0000  ................
+000039d0: 4300 0000 7344 0000 0074 0074 0174 027c  C...sD...t.t.t.|
+000039e0: 0183 0183 0183 017d 0274 037c 017c 027c  .......}.t.|.|.|
+000039f0: 0264 0164 0164 028d 055c 047d 037d 047d  .d.d.d...\.}.}.}
+00003a00: 047d 0474 0074 0464 0364 0484 007c 007c  .}.t.t.d.d...|.|
+00003a10: 0383 0144 0083 018e 0083 0153 0029 054e  ...D.......S.).N
+00003a20: 4629 05da 0764 6174 6173 6574 da0d 7472  F)...dataset..tr
+00003a30: 6169 6e5f 696e 6469 6365 73da 0c74 6573  ain_indices..tes
+00003a40: 745f 696e 6469 6365 73da 0f75 7365 5f69  t_indices..use_i
+00003a50: 6d70 6f72 7461 6e63 6573 7233 0000 0063  mportancesr3...c
+00003a60: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+00003a70: 0400 0000 5300 0000 7314 0000 0067 007c  ....S...s....g.|
+00003a80: 005d 067d 017c 01a0 00a1 0091 0271 0253  .].}.|.......q.S
+00003a90: 0072 4000 0000 2901 da05 6e75 6d70 7929  .r@...)...numpy)
+00003aa0: 0272 4200 0000 da01 7672 4000 0000 7240  .rB.....vr@...r@
+00003ab0: 0000 0072 4400 0000 7245 0000 0057 0200  ...rD...rE...W..
+00003ac0: 0073 0200 0000 1400 7a28 4d65 6761 6e2e  .s......z(Megan.
+00003ad0: 7072 6564 6963 745f 6772 6170 6873 2e3c  predict_graphs.<
+00003ae0: 6c6f 6361 6c73 3e2e 3c6c 6973 7463 6f6d  locals>.<listcom
+00003af0: 703e 2905 da04 6c69 7374 728a 0000 0072  p>)...listr....r
+00003b00: 6d00 0000 720d 0000 0072 5900 0000 2905  m...r....rY...).
+00003b10: 726f 0000 0072 df00 0000 da07 696e 6469  ro...r......indi
+00003b20: 6365 7372 9500 0000 7243 0000 0072 4000  cesr....rC...r@.
+00003b30: 0000 7240 0000 0072 4400 0000 da0e 7072  ..r@...rD.....pr
+00003b40: 6564 6963 745f 6772 6170 6873 4d02 0000  edict_graphsM...
+00003b50: 7312 0000 0010 0102 0102 0102 0102 0102  s...............
+00003b60: 0102 010e fb1a 087a 144d 6567 616e 2e70  .......z.Megan.p
+00003b70: 7265 6469 6374 5f67 7261 7068 73da 0567  redict_graphs..g
+00003b80: 7261 7068 6302 0000 0000 0000 0000 0000  raphc...........
+00003b90: 0002 0000 0003 0000 0043 0000 0073 1000  .........C...s..
+00003ba0: 0000 7c00 a000 7c01 6701 a101 6401 1900  ..|...|.g...d...
+00003bb0: 5300 2902 4e72 0100 0000 2901 72e8 0000  S.).Nr....).r...
+00003bc0: 0029 0272 6f00 0000 72e9 0000 0072 4000  .).ro...r....r@.
+00003bd0: 0000 7240 0000 0072 4400 0000 da0d 7072  ..r@...rD.....pr
+00003be0: 6564 6963 745f 6772 6170 6859 0200 0073  edict_graphY...s
+00003bf0: 0200 0000 1001 7a13 4d65 6761 6e2e 7072  ......z.Megan.pr
+00003c00: 6564 6963 745f 6772 6170 6829 0346 464e  edict_graph).FFN
+00003c10: 7247 0000 0029 1fda 085f 5f6e 616d 655f  rG...)...__name_
+00003c20: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
+00003c30: 5f71 7561 6c6e 616d 655f 5fda 075f 5f64  _qualname__..__d
+00003c40: 6f63 5f5f da01 74da 044c 6973 7472 6b00  oc__..t..Listrk.
+00003c50: 0000 da03 7374 72da 0462 6f6f 6c72 6c00  ....str..boolrl.
+00003c60: 0000 da08 4f70 7469 6f6e 616c 7249 0000  ....OptionalrI..
+00003c70: 00da 066c 6179 6572 73da 054c 6179 6572  ...layers..Layer
+00003c80: da05 5475 706c 6572 4c00 0000 7278 0000  ..TuplerL...rx..
+00003c90: 00da 0870 726f 7065 7274 7972 8000 0000  ...propertyr....
+00003ca0: 7281 0000 0072 8600 0000 da0c 5261 6767  r....r......Ragg
+00003cb0: 6564 5465 6e73 6f72 72a7 0000 0072 b400  edTensorr....r..
+00003cc0: 0000 72ca 0000 0072 de00 0000 da02 7476  ..r....r......tv
+00003cd0: da09 4772 6170 6844 6963 7472 e800 0000  ..GraphDictr....
+00003ce0: 72ea 0000 00da 0d5f 5f63 6c61 7373 6365  r......__classce
+00003cf0: 6c6c 5f5f 7240 0000 0072 4000 0000 727b  ll__r@...r@...r{
+00003d00: 0000 0072 4400 0000 7213 0000 0017 0000  ...rD...r.......
+00003d10: 0073 ca00 0000 0800 0401 020c 0201 0201  .s..............
+00003d20: 0201 0202 0201 0201 0201 0201 0201 0201  ................
+00003d30: 0201 0201 0201 0402 0201 0201 0201 0201  ................
+00003d40: 0201 0201 0201 0201 0201 04e4 0802 02fe  ................
+00003d50: 0203 02fd 0204 02fc 0205 02fb 0206 02fa  ................
+00003d60: 0808 02f8 0209 02f7 020a 02f6 020b 02f5  ................
+00003d70: 020c 02f4 020d 02f3 120e 02f2 020f 02f1  ................
+00003d80: 0210 02f0 0211 02ef 0813 02ed 0214 02ec  ................
+00003d90: 0215 02eb 0216 02ea 1217 02e9 1218 02e8  ................
+00003da0: 1819 02e7 081a 02e6 021b 02e5 021c 0ae4  ................
+00003db0: 007f 0c4e 021f 1001 0e03 0207 0201 0201  ...N............
+00003dc0: 04fc 0202 02fe 0203 02fd 0a04 0afc 007f  ................
+00003dd0: 0807 0229 04ff 0201 0aff 0834 1655 180c  ...).......4.U..
+00003de0: 7213 0000 0029 24da 0674 7970 696e 6772  r....)$..typingr
+00003df0: ef00 0000 da0a 7465 6e73 6f72 666c 6f77  ......tensorflow
+00003e00: 7286 0000 00da 1074 656e 736f 7266 6c6f  r......tensorflo
+00003e10: 772e 6b65 7261 73da 056b 6572 6173 7249  w.keras..kerasrI
+00003e20: 0000 00da 1c76 6973 7561 6c5f 6772 6170  .....visual_grap
+00003e30: 685f 6461 7461 7365 7473 2e74 7970 696e  h_datasets.typin
+00003e40: 6772 f900 0000 da1e 7465 6e73 6f72 666c  gr......tensorfl
+00003e50: 6f77 2e70 7974 686f 6e2e 6b65 7261 732e  ow.python.keras.
+00003e60: 656e 6769 6e65 7202 0000 00da 106b 6763  enginer......kgc
+00003e70: 6e6e 2e64 6174 612e 7574 696c 7372 0300  nn.data.utilsr..
+00003e80: 0000 da14 6b67 636e 6e2e 6c61 7965 7273  ....kgcnn.layers
+00003e90: 2e6d 6f64 756c 6573 7204 0000 0072 0500  .modulesr....r..
+00003ea0: 0000 7206 0000 0072 0700 0000 7208 0000  ..r....r....r...
+00003eb0: 0072 0900 0000 da14 6b67 636e 6e2e 6c61  .r......kgcnn.la
+00003ec0: 7965 7273 2e70 6f6f 6c69 6e67 720a 0000  yers.poolingr...
+00003ed0: 0072 0b00 0000 720c 0000 00da 1c67 7261  .r....r......gra
+00003ee0: 7068 5f61 7474 656e 7469 6f6e 5f73 7475  ph_attention_stu
+00003ef0: 6465 6e74 2e64 6174 6172 0d00 0000 da1e  dent.datar......
+00003f00: 6772 6170 685f 6174 7465 6e74 696f 6e5f  graph_attention_
+00003f10: 7374 7564 656e 742e 6c61 7965 7273 720e  student.layersr.
+00003f20: 0000 0072 0f00 0000 da20 6772 6170 685f  ...r..... graph_
+00003f30: 6174 7465 6e74 696f 6e5f 7374 7564 656e  attention_studen
+00003f40: 742e 7472 6169 6e69 6e67 7210 0000 0072  t.trainingr....r
+00003f50: 1100 0000 7212 0000 0072 4a00 0000 724b  ....r....rJ...rK
+00003f60: 0000 0072 1300 0000 7240 0000 0072 4000  ...r....r@...r@.
+00003f70: 0000 7240 0000 0072 4400 0000 da08 3c6d  ..r@...rD.....<m
+00003f80: 6f64 756c 653e 0100 0000 7326 0000 0008  odule>....s&....
+00003f90: 0008 020c 010c 010c 010c 010c 0110 0114  ................
+00003fa0: 010c 010c 010c 010c 020c 010c 010c 010c  ................
+00003fb0: 010c 0118 03                             .....
```

### Comparing `graph_attention_student-0.7.2/graph_attention_student/models/gnes.py` & `graph_attention_student-0.9.0/graph_attention_student/models/gnes.py`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.2/graph_attention_student/models/gnnx.py` & `graph_attention_student-0.9.0/graph_attention_student/models/gnnx.py`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.2/graph_attention_student/models/gradient.py` & `graph_attention_student-0.9.0/graph_attention_student/models/gradient.py`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.2/graph_attention_student/models/megan.py` & `graph_attention_student-0.9.0/graph_attention_student/models/megan.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 import typing as t
 
 import tensorflow as tf
 import tensorflow.keras as ks
+import visual_graph_datasets.typing as tv
 from tensorflow.python.keras.engine import compile_utils
 from kgcnn.data.utils import ragged_tensor_from_nested_numpy
 from kgcnn.layers.modules import GraphBaseLayer
 from kgcnn.layers.modules import LazyConcatenate, LazyAverage
 from kgcnn.layers.modules import DenseEmbedding, ActivationEmbedding, DropoutEmbedding
 from kgcnn.layers.pooling import PoolingLocalEdges
 from kgcnn.layers.pooling import PoolingNodes
 from kgcnn.layers.pooling import PoolingWeightedNodes
+
+from graph_attention_student.data import process_graph_dataset
 from graph_attention_student.layers import ExplanationSparsityRegularization
 from graph_attention_student.layers import MultiHeadGATV2Layer
 from graph_attention_student.training import mae
 from graph_attention_student.training import bce
 from graph_attention_student.training import shifted_sigmoid
 
 
@@ -574,8 +577,26 @@
         )
 
         # Return a dict mapping metric names to current value.
         # Note that it will include the loss (tracked in self.metrics).
         return {
             **{m.name: m.result() for m in self.metrics},
             **exp_metrics
-        }
+        }
+
+    # -- Implements "PredictGraphMixin"
+    # These following method implementations are required to
+
+    def predict_graphs(self, graph_list: t.List[tv.GraphDict]):
+        indices = list(range(len(graph_list)))
+        x, _, _, _ = process_graph_dataset(
+            dataset=graph_list,
+            train_indices=indices,
+            test_indices=indices,
+            use_importances=False,
+            use_graph_attributes=False,
+        )
+
+        return list(zip(*[v.numpy() for v in self(x)]))
+
+    def predict_graph(self, graph: tv.GraphDict):
+        return self.predict_graphs([graph])[0]
```

### Comparing `graph_attention_student-0.7.2/graph_attention_student/templates/article.tex.j2` & `graph_attention_student-0.9.0/graph_attention_student/templates/article.tex.j2`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.2/graph_attention_student/training.py` & `graph_attention_student-0.9.0/graph_attention_student/training.py`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.2/graph_attention_student/typing.py` & `graph_attention_student-0.9.0/graph_attention_student/typing.py`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.2/graph_attention_student/util.py` & `graph_attention_student-0.9.0/graph_attention_student/util.py`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.2/graph_attention_student/visualization.py` & `graph_attention_student-0.9.0/graph_attention_student/visualization.py`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.2/pyproject.toml` & `graph_attention_student-0.9.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.2.0b2"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "graph_attention_student"
-version = "0.7.2"
+version = "0.9.0"
 description = "MEGAN: Multi Explanation Graph Attention Network"
 license = "MIT"
 authors = ["xxx <jonseb1998@gmail.com>"]
 maintainers = ["xxx <jonseb1998@gmail.com>"]
 readme = "README.rst"
 keywords = ["graph neural network", "attention", "kgcnn"]
 packages = [
@@ -26,28 +26,29 @@
 ]
 
 [tool.poetry.scripts]
 graph_attention_student = 'graph_attention_student.cli:cli'
 
 [tool.poetry.dependencies]
 python = ">=3.8.0,<3.11"
-pycomex = ">=0.8.4"
+pycomex = ">=0.9.2"
 click = ">=7.1.2"
 jinja2 = ">=3.0.3"
 matplotlib = ">=3.5.3"
 imageio = ">=2.19.0"
 cairosvg = ">=2.5.2"
 numpy = ">=1.22.0"
 tensorflow = ">=2.8.0"
 kgcnn = ">=2.2.1"
 nltk = ">=3.7"
 rdkit = ">=2022.9.1"
 orjson = ">=3.8.0"
 poetry-bumpversion = ">=0.3.0"
-visual_graph_datasets = ">=0.7.2"
+visual_graph_datasets = ">=0.11.0"
+vgd_counterfactuals = ">=0.1.0"
 
 [tool.poetry_bumpversion.file."graph_attention_student/__init__.py"]
 search = '__version__ = "{current_version}"'
 replace = '__version__ = "{new_version}"'
 
 [tool.poetry_bumpversion.file."graph_attention_student/VERSION"]
 search = "{current_version}"
```

### Comparing `graph_attention_student-0.7.2/setup.py` & `graph_attention_student-0.9.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,39 +4,43 @@
 packages = \
 ['graph_attention_student',
  'graph_attention_student.examples',
  'graph_attention_student.experiments',
  'graph_attention_student.models']
 
 package_data = \
-{'': ['*'], 'graph_attention_student': ['templates/*']}
+{'': ['*'],
+ 'graph_attention_student': ['templates/*'],
+ 'graph_attention_student.examples': ['assets/aqsoldb_model/*',
+                                      'assets/aqsoldb_model/variables/*']}
 
 install_requires = \
 ['cairosvg>=2.5.2',
  'click>=7.1.2',
  'imageio>=2.19.0',
  'jinja2>=3.0.3',
  'kgcnn>=2.2.1',
  'matplotlib>=3.5.3',
  'nltk>=3.7',
  'numpy>=1.22.0',
  'orjson>=3.8.0',
  'poetry-bumpversion>=0.3.0',
- 'pycomex>=0.8.4',
+ 'pycomex>=0.9.2',
  'rdkit>=2022.9.1',
  'tensorflow>=2.8.0',
- 'visual_graph_datasets>=0.7.2']
+ 'vgd_counterfactuals>=0.1.0',
+ 'visual_graph_datasets>=0.11.0']
 
 entry_points = \
 {'console_scripts': ['graph_attention_student = '
                      'graph_attention_student.cli:cli']}
 
 setup_kwargs = {
     'name': 'graph-attention-student',
-    'version': '0.7.2',
+    'version': '0.9.0',
     'description': 'MEGAN: Multi Explanation Graph Attention Network',
     'long_description': '|made-with-python| |made-with-kgcnn| |python-version| |os-linux|\n\n.. |os-linux| image:: https://img.shields.io/badge/os-linux-orange.svg\n   :target: https://www.python.org/\n\n.. |python-version| image:: https://img.shields.io/badge/Python-3.8.0-green.svg\n   :target: https://www.python.org/\n\n.. |made-with-kgcnn| image:: https://img.shields.io/badge/Made%20with-KGCNN-blue.svg\n   :target: https://github.com/aimat-lab/gcnn_keras\n\n.. |made-with-python| image:: https://img.shields.io/badge/Made%20with-Python-1f425f.svg\n   :target: https://www.python.org/\n\n.. image:: architecture.png\n    :width: 800\n    :alt: Architecture Overview\n\n================================================\nMEGAN: Multi Explanation Graph Attention Student\n================================================\n\nExplainable artificial intelligence (XAI) methods are expected to improve trust during human-AI interactions,\nprovide tools for model analysis and extend human understanding of complex problems. Attention-based models\nare an important subclass of XAI methods, partly due to their full differentiability and the potential to\nimprove explanations by means of explanation-supervised training. We propose the novel multi-explanation\ngraph attention network (MEGAN). Our graph regression and classification model features multiple explanation\nchannels, which can be chosen independently of the task specifications. We first validate our model on a\nsynthetic graph regression dataset, where our model produces single-channel explanations with quality\nsimilar to GNNExplainer. Furthermore, we demonstrate the advantages of multi-channel explanations on one\nsynthetic and two real-world datasets: The prediction of water solubility of molecular graphs and\nsentiment classification of movie reviews. We find that our model produces explanations consistent\nwith human intuition, opening the way to learning from our model in less well-understood tasks.\n\nInstallation\n============\n\nMain Installation\n-----------------\n\nClone the repository from github:\n\n.. code-block:: shell\n\n    git clone https://github.com/awa59kst120df/graph_attention_student.git\n\nThen in the main folder run a ``pip install``:\n\n.. code-block:: shell\n\n    cd graph_attention_student\n    pip3 install -e .\n\nAfterwards, you can check the install by invoking the CLI:\n\n.. code-block:: shell\n\n    python3 -m graph_attention_student.cli --version\n    python3 -m graph_attention_student.cli --help\n\nUsage\n=====\n\nComputational Experiments\n-------------------------\n\nIt is possible to list, show and execute all the computational experiments using a command line interface\nCLI.\n\n    *NOTE* Most of the experiments have a long runtime, ranging from ~2hrs to ~2days.\n    Furthermore, all of the experiments which do model training are currently configured to run on a GPU\n    and might crash if the GPU can either not be detected or does not have enough VRAM. This setting can\n    be changed in the corresponding experiment scripts\n\nAll the available experiments can be listed like this:\n\n.. code-block:: shell\n\n    python3 -m graph_attention_student.cli list\n\nThe details for a specific experiment can be viewed like this:\n\n.. code-block:: shell\n\n    python3 -m graph_attention_student.cli info [experiment_name]\n\nA new run of an experiment can be started like this. However, be aware that this might take some time.\n\n.. code-block::\n\n    python3 -m graph_attention_student.cli run [experiment_name]\n\nEach experiment will create a new archive folder, which will contain all the artifacts (such as visual\nexamples and the raw data) created during the runtime. The location of this archive folder can be found\nfrom the output generated by the experiment execution.\n\nArchived Experiments\n--------------------\n\nTo view the detailed data which was used in the making of the paper, go to\n``graph_attention_student/experiments``. The subfolders in that folder contain the archived experiments.\nThese contain extensive examples for each repetition of the various experiments as well as all of the raw\ndata collected during the execution of the experiments.\n\nMEGAN in code\n-------------\n\nThe MEGAN model is implemented as the ``MultiAttentionStudent`` class, which implements ``keras.Model``.\nThe implementation is based on the `kgcnn`_ library for graph convolutional networks for keras. For further\ninformation on loading graph structured data with `kgcnn`_ visit:\nhttps://github.com/aimat-lab/gcnn_keras\n\nThis is a simple example of how to use the model in the regression case:\n\n.. code-block:: python\n\n    import tensorflow as tf\n    import tensorflow.keras as ks\n    from graph_attention_student.training import NoLoss\n    from graph_attention_student.models import Megan\n\n    model = Megan(\n        # These lists define the number of layers and the number of hidden units in each layer for the\n        # various parts of the architecture\n        units=[9, 9, 9],  # The main convolutional layers\n        importance_units=[],  # The MLP that creates the node importances\n        final_units=[5, 1],  # The final MLP for graph embeddings\n        # Example for a regression problem. We need the prior knowledge about what range the values of the\n        # dataset will be expected to fall into...\n        regression_limits=(-3, +3),\n        # ... as well as a reference value.\n        regression_reference=0,\n        # This controls the weight of the explanation-only train step (gamma)\n        importance_factor=1.0,\n        importance_multiplier=5,\n        # This is the weight of the sparsity regularization\n        sparsity_factor=0.1,\n    )\n\n    # The model output is actually a three tuple: (prediction, node_importances, edge_importances).\n    # This allows the importances to be trained in a supervised fashion. If we don\'t want that,\n    # we can simply supply the NoLoss function instead.\n    model.compile(\n        loss=[ks.losses.MeanSquaredError(), NoLoss(), NoLoss()],\n        loss_weights=[1, 1, 1],\n        optimizer=ks.optimizers.Adam(0.001)\n    )\n\n    # model.fit() ...\n\n\n.. _kgcnn: https://github.com/aimat-lab/gcnn_keras\n.. _examples/solubility_regression.py: https://github.com/aimat-lab/graph_attention_student/tree/master/graph_attention_student/examples/solubility_regression.py\n.. _`GATv2`: https://github.com/tech-srl/how_attentive_are_gats\n\n---\n\nExamples\n========\n\nThe following examples show some of the *cherry picked* examples that show the explanatory capabilities of\nthe model.\n\nRB-Motifs Dataset\n-----------------\n\nThis is a synthetic dataset, which basically consists of randomly generated graphs with nodes of different\ncolors. Some of the graphs contain special sub-graph motifs, which are either blue-heavy or red-heavy\nstructures. The blue-heavy sub-graphs contribute a certain negative value to the overall value of the graph,\nwhile red-heavy structures contain a certain positive value.\n\nThis way, every graph has a certain value associated with it, which is between -3 and 3. The network was\ntrained to predict this value for each graph.\n\n.. image:: rb_motifs_example.png\n    :width: 800\n    :alt: Rb-Motifs Example\n\nThe examples shows from left to right: (1) The ground truth explanations, (2) a baseline MEGAN model trained\nonly on the prediction task, (3) explanation-supervised MEGAN model and (4) GNNExplainer explanations for a\nbasic GCN network. While the baseline MEGAN and GNNExplainer focus only on one of the ground truth motifs,\nthe explanation-supervised MEGAN model correctly finds both.\n\nWater Solubility Dataset\n------------------------\n\nThis is the `AqSolDB`_ dataset, which consists of ~10000 molecules and measured values for the solubility in\nwater (logS value).\n\nThe network was trained to predict the solubility value for each molecule.\n\n.. image:: solubility_example.png\n    :width: 800\n    :alt: Solubility Example.png\n\n.. _`AqSolDB`: https://www.nature.com/articles/s41597-019-0151-1\n\nMovie Reviews\n-------------\n\nOriginally the *MovieReviews* dataset is a natural language processing dataset from the `ERASER`_ benchmark.\nThe task is to classify the sentiment of ~2000 movie reviews collected from the IMDB database into the\nclasses "positive" and "negative". This dataset was converted into a graph dataset by considering all words\nas nodes of a graph and then connecting adjacent words by undirected edges with a sliding window of size 2.\nWords were converted into numeric feature vectors by using a pre-trained `GLOVE`_ model.\n\nExample for a positive review:\n\n.. image:: movie_reviews_pos.png\n    :width: 800\n    :alt: Positive Movie Review\n\nExample for a negative review:\n\n.. image:: movie_reviews_neg.png\n    :width: 800\n    :alt: Negative Movie Review\n\nExamples show the explanation channel for the "negative" class left and the "positive" class right.\nSentences with negative / positive adjectives are appropriately attributed to the corresponding channels.\n\n.. _`ERASER`: https://www.eraserbenchmark.com/\n.. _`GLOVE`: https://nlp.stanford.edu/projects/glove/\n\n',
     'author': 'xxx',
     'author_email': 'jonseb1998@gmail.com',
     'maintainer': 'xxx',
     'maintainer_email': 'jonseb1998@gmail.com',
     'url': 'None',
```

### Comparing `graph_attention_student-0.7.2/PKG-INFO` & `graph_attention_student-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graph-attention-student
-Version: 0.7.2
+Version: 0.9.0
 Summary: MEGAN: Multi Explanation Graph Attention Network
 License: MIT
 Keywords: graph neural network,attention,kgcnn
 Author: xxx
 Author-email: jonseb1998@gmail.com
 Maintainer: xxx
 Maintainer-email: jonseb1998@gmail.com
@@ -20,18 +20,19 @@
 Requires-Dist: jinja2 (>=3.0.3)
 Requires-Dist: kgcnn (>=2.2.1)
 Requires-Dist: matplotlib (>=3.5.3)
 Requires-Dist: nltk (>=3.7)
 Requires-Dist: numpy (>=1.22.0)
 Requires-Dist: orjson (>=3.8.0)
 Requires-Dist: poetry-bumpversion (>=0.3.0)
-Requires-Dist: pycomex (>=0.8.4)
+Requires-Dist: pycomex (>=0.9.2)
 Requires-Dist: rdkit (>=2022.9.1)
 Requires-Dist: tensorflow (>=2.8.0)
-Requires-Dist: visual_graph_datasets (>=0.7.2)
+Requires-Dist: vgd_counterfactuals (>=0.1.0)
+Requires-Dist: visual_graph_datasets (>=0.11.0)
 Description-Content-Type: text/x-rst
 
 |made-with-python| |made-with-kgcnn| |python-version| |os-linux|
 
 .. |os-linux| image:: https://img.shields.io/badge/os-linux-orange.svg
    :target: https://www.python.org/
```

