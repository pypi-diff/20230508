# Comparing `tmp/vectorlab-1.0.2.tar.gz` & `tmp/vectorlab-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vectorlab-1.0.2.tar", last modified: Fri Apr 28 08:11:35 2023, max compression
+gzip compressed data, was "vectorlab-1.0.3.tar", last modified: Mon May  8 04:11:27 2023, max compression
```

## Comparing `vectorlab-1.0.2.tar` & `vectorlab-1.0.3.tar`

### file list

```diff
@@ -1,99 +1,99 @@
--rw-r--r--   0        0        0     1544 2023-04-24 06:07:52.194842 vectorlab-1.0.2/LICENSE.txt
--rw-r--r--   0        0        0     2212 2023-04-24 06:07:52.194842 vectorlab-1.0.2/README.md
--rw-r--r--   0        0        0     1352 2023-04-28 08:09:16.372051 vectorlab-1.0.2/pyproject.toml
--rw-r--r--   0        0        0      272 2023-04-28 08:09:16.372051 vectorlab-1.0.2/vectorlab/__init__.py
--rw-r--r--   0        0        0    11168 2023-04-24 06:07:52.194842 vectorlab-1.0.2/vectorlab/base.py
--rw-r--r--   0        0        0      113 2023-04-24 06:07:52.194842 vectorlab-1.0.2/vectorlab/data/__init__.py
--rw-r--r--   0        0        0     1129 2023-04-24 06:07:52.194842 vectorlab-1.0.2/vectorlab/data/_argument_generator.py
--rw-r--r--   0        0        0     1308 2023-04-24 06:07:52.194842 vectorlab-1.0.2/vectorlab/data/_data_generator.py
--rw-r--r--   0        0        0       76 2023-04-24 06:07:52.194842 vectorlab-1.0.2/vectorlab/data/dataloader/__init__.py
--rw-r--r--   0        0        0     3809 2023-04-24 06:07:52.194842 vectorlab-1.0.2/vectorlab/data/dataloader/_torch_dataloader.py
--rw-r--r--   0        0        0     4801 2023-04-24 06:07:52.194842 vectorlab-1.0.2/vectorlab/data/dataloader/_torch_geometric_dataloader.py
--rw-r--r--   0        0        0     1662 2023-04-24 06:07:52.194842 vectorlab-1.0.2/vectorlab/data/dataloader/tests/test_torch_dataloader.py
--rw-r--r--   0        0        0       57 2023-04-24 06:07:52.194842 vectorlab-1.0.2/vectorlab/data/dataset/__init__.py
--rw-r--r--   0        0        0     6196 2023-04-24 06:07:52.194842 vectorlab-1.0.2/vectorlab/data/dataset/_torch_dataset.py
--rw-r--r--   0        0        0    31856 2023-04-24 06:07:52.194842 vectorlab-1.0.2/vectorlab/data/dataset/_ts_dataset.py
--rw-r--r--   0        0        0      385 2023-04-24 06:07:52.194842 vectorlab-1.0.2/vectorlab/data/tests/test_argument_generator.py
--rw-r--r--   0        0        0      533 2023-04-24 06:07:52.194842 vectorlab-1.0.2/vectorlab/data/tests/test_data_generator.py
--rw-r--r--   0        0        0       23 2023-04-24 06:07:52.194842 vectorlab-1.0.2/vectorlab/ensemble/__init__.py
--rw-r--r--   0        0        0     3677 2023-04-24 06:07:52.194842 vectorlab-1.0.2/vectorlab/ensemble/_voting.py
--rw-r--r--   0        0        0     4070 2023-04-24 06:07:52.194842 vectorlab-1.0.2/vectorlab/ensemble/tests/test_ensemble_voting.py
--rw-r--r--   0        0        0       70 2023-04-24 06:07:52.194842 vectorlab-1.0.2/vectorlab/graph/__init__.py
--rw-r--r--   0        0        0    11604 2023-04-24 06:07:52.194842 vectorlab-1.0.2/vectorlab/graph/_generator.py
--rw-r--r--   0        0        0    15921 2023-04-24 06:07:52.194842 vectorlab-1.0.2/vectorlab/graph/_utils.py
--rw-r--r--   0        0        0     1169 2023-04-24 06:07:52.194842 vectorlab-1.0.2/vectorlab/graph/tests/test_graph_generator.py
--rw-r--r--   0        0        0     6818 2023-04-24 06:07:52.194842 vectorlab-1.0.2/vectorlab/graph/tests/test_graph_utils.py
--rw-r--r--   0        0        0       68 2023-04-24 06:07:52.194842 vectorlab-1.0.2/vectorlab/graph/walking/__init__.py
--rw-r--r--   0        0        0     1920 2023-04-24 06:07:52.194842 vectorlab-1.0.2/vectorlab/graph/walking/_bfs.py
--rw-r--r--   0        0        0     1869 2023-04-24 06:07:52.194842 vectorlab-1.0.2/vectorlab/graph/walking/_dfs.py
--rw-r--r--   0        0        0     1275 2023-04-24 06:07:52.194842 vectorlab-1.0.2/vectorlab/graph/walking/_random_walk.py
--rw-r--r--   0        0        0     2235 2023-04-24 06:07:52.194842 vectorlab-1.0.2/vectorlab/graph/walking/tests/test_graph_walking.py
--rw-r--r--   0        0        0       23 2023-04-24 06:07:52.194842 vectorlab-1.0.2/vectorlab/metrics/__init__.py
--rw-r--r--   0        0        0       87 2023-04-24 06:07:52.194842 vectorlab-1.0.2/vectorlab/metrics/pairwise/__init__.py
--rw-r--r--   0        0        0     8721 2023-04-24 06:07:52.194842 vectorlab-1.0.2/vectorlab/metrics/pairwise/_dtw.py
--rw-r--r--   0        0        0     3329 2023-04-24 06:07:52.194842 vectorlab-1.0.2/vectorlab/metrics/pairwise/_kl_div.py
--rw-r--r--   0        0        0     1183 2023-04-24 06:07:52.194842 vectorlab-1.0.2/vectorlab/metrics/pairwise/_lp_norm.py
--rw-r--r--   0        0        0     3206 2023-04-24 06:07:52.194842 vectorlab-1.0.2/vectorlab/metrics/pairwise/_sbd.py
--rw-r--r--   0        0        0     2365 2023-04-24 06:07:52.194842 vectorlab-1.0.2/vectorlab/metrics/pairwise/tests/test_metrics_pairwise.py
--rw-r--r--   0        0        0      119 2023-04-24 06:07:52.194842 vectorlab-1.0.2/vectorlab/nn/__init__.py
--rw-r--r--   0        0        0     4302 2023-04-28 08:09:16.372051 vectorlab-1.0.2/vectorlab/nn/_earlystopping.py
--rw-r--r--   0        0        0     7110 2023-04-28 08:09:16.372051 vectorlab-1.0.2/vectorlab/nn/_logger.py
--rw-r--r--   0        0        0     7154 2023-04-28 08:09:16.372051 vectorlab-1.0.2/vectorlab/nn/_resolver.py
--rw-r--r--   0        0        0    45671 2023-04-28 08:09:16.372051 vectorlab-1.0.2/vectorlab/nn/explorer.py
--rw-r--r--   0        0        0     2906 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/nn/functional.py
--rw-r--r--   0        0        0      201 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/nn/models/__init__.py
--rw-r--r--   0        0        0    18081 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/nn/models/_autoencoder.py
--rw-r--r--   0        0        0     2303 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/nn/models/_basic_gnn.py
--rw-r--r--   0        0        0     3679 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/nn/models/_classifier.py
--rw-r--r--   0        0        0    11804 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/nn/models/_decoder.py
--rw-r--r--   0        0        0    32841 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/nn/models/_encoder.py
--rw-r--r--   0        0        0     2571 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/nn/models/_gnn_decoder.py
--rw-r--r--   0        0        0     7574 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/nn/models/_mlp.py
--rw-r--r--   0        0        0     5855 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/nn/models/_seq2seq.py
--rw-r--r--   0        0        0     2155 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/nn/models/tests/test_decoder.py
--rw-r--r--   0        0        0     2255 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/nn/models/tests/test_encoder.py
--rw-r--r--   0        0        0     1276 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/nn/models/tests/test_seq2seq.py
--rw-r--r--   0        0        0       44 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/nn/modules/__init__.py
--rw-r--r--   0        0        0     1529 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/nn/modules/gnn_loss.py
--rw-r--r--   0        0        0     2556 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/nn/modules/loss.py
--rw-r--r--   0        0        0      743 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/nn/tests/test_explorer.py
--rw-r--r--   0        0        0      873 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/nn/tests/test_functional.py
--rw-r--r--   0        0        0       45 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/optimize/__init__.py
--rw-r--r--   0        0        0     6294 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/optimize/_estimate.py
--rw-r--r--   0        0        0    16484 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/optimize/_qap.py
--rw-r--r--   0        0        0     2521 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/optimize/tests/test_estimate.py
--rw-r--r--   0        0        0       69 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/plot/__init__.py
--rw-r--r--   0        0        0      412 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/plot/_helper.py
--rw-r--r--   0        0        0     2980 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/plot/_palettes.py
--rw-r--r--   0        0        0    16083 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/plot/_plot.py
--rw-r--r--   0        0        0      732 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/plot/tests/test_plot.py
--rw-r--r--   0        0        0       76 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/series/__init__.py
--rw-r--r--   0        0        0     8732 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/series/_preprocessing.py
--rw-r--r--   0        0        0     2796 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/series/_utils.py
--rw-r--r--   0        0        0      116 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/series/smoothing/__init__.py
--rw-r--r--   0        0        0     6298 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/series/smoothing/_arima.py
--rw-r--r--   0        0        0     7438 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/series/smoothing/_holt_winters.py
--rw-r--r--   0        0        0    12319 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/series/smoothing/_moving_average.py
--rw-r--r--   0        0        0     6832 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/series/smoothing/_spectral_residual.py
--rw-r--r--   0        0        0     2333 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/series/smoothing/tests/test_series_smoothing.py
--rw-r--r--   0        0        0     1520 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/series/tests/test_series_preprocessing.py
--rw-r--r--   0        0        0       77 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/stats/__init__.py
--rw-r--r--   0        0        0    15478 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/stats/_deg_graph.py
--rw-r--r--   0        0        0    18242 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/stats/_freq_tree.py
--rw-r--r--   0        0        0    14207 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/stats/_t_digest.py
--rw-r--r--   0        0        0     1312 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/stats/tests/test_deg_graph.py
--rw-r--r--   0        0        0     1311 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/stats/tests/test_freq_tree.py
--rw-r--r--   0        0        0     1310 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/stats/tests/test_t_digest.py
--rw-r--r--   0        0        0      110 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/utils/__init__.py
--rw-r--r--   0        0        0     9958 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/utils/_check.py
--rw-r--r--   0        0        0      617 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/utils/_env.py
--rw-r--r--   0        0        0     2026 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/utils/_loading.py
--rw-r--r--   0        0        0     2707 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/utils/_parser.py
--rw-r--r--   0        0        0     5089 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/utils/_time.py
--rw-r--r--   0        0        0     1123 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/utils/tests/test_time.py
--rw-r--r--   0        0        0       45 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/vector/__init__.py
--rw-r--r--   0        0        0    11924 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/vector/_array.py
--rw-r--r--   0        0        0     2933 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/vector/_tensor.py
--rw-r--r--   0        0        0     4140 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/vector/tests/test_array.py
--rw-r--r--   0        0        0     1217 2023-04-24 06:07:52.198842 vectorlab-1.0.2/vectorlab/vector/tests/test_tensor.py
--rw-r--r--   0        0        0     3798 1970-01-01 00:00:00.000000 vectorlab-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1544 2023-04-24 06:07:52.194842 vectorlab-1.0.3/LICENSE.txt
+-rw-r--r--   0        0        0     2212 2023-04-24 06:07:52.194842 vectorlab-1.0.3/README.md
+-rw-r--r--   0        0        0     1546 2023-05-08 04:09:34.236482 vectorlab-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0      272 2023-05-08 04:09:34.236482 vectorlab-1.0.3/vectorlab/__init__.py
+-rw-r--r--   0        0        0    11168 2023-04-24 06:07:52.194842 vectorlab-1.0.3/vectorlab/base.py
+-rw-r--r--   0        0        0      113 2023-04-24 06:07:52.194842 vectorlab-1.0.3/vectorlab/data/__init__.py
+-rw-r--r--   0        0        0     1129 2023-04-24 06:07:52.194842 vectorlab-1.0.3/vectorlab/data/_argument_generator.py
+-rw-r--r--   0        0        0     1308 2023-04-24 06:07:52.194842 vectorlab-1.0.3/vectorlab/data/_data_generator.py
+-rw-r--r--   0        0        0       76 2023-04-24 06:07:52.194842 vectorlab-1.0.3/vectorlab/data/dataloader/__init__.py
+-rw-r--r--   0        0        0     3809 2023-04-24 06:07:52.194842 vectorlab-1.0.3/vectorlab/data/dataloader/_torch_dataloader.py
+-rw-r--r--   0        0        0     4801 2023-04-24 06:07:52.194842 vectorlab-1.0.3/vectorlab/data/dataloader/_torch_geometric_dataloader.py
+-rw-r--r--   0        0        0     1662 2023-04-24 06:07:52.194842 vectorlab-1.0.3/vectorlab/data/dataloader/tests/test_torch_dataloader.py
+-rw-r--r--   0        0        0       57 2023-04-24 06:07:52.194842 vectorlab-1.0.3/vectorlab/data/dataset/__init__.py
+-rw-r--r--   0        0        0     6196 2023-04-24 06:07:52.194842 vectorlab-1.0.3/vectorlab/data/dataset/_torch_dataset.py
+-rw-r--r--   0        0        0    31856 2023-04-24 06:07:52.194842 vectorlab-1.0.3/vectorlab/data/dataset/_ts_dataset.py
+-rw-r--r--   0        0        0      385 2023-04-24 06:07:52.194842 vectorlab-1.0.3/vectorlab/data/tests/test_argument_generator.py
+-rw-r--r--   0        0        0      533 2023-04-24 06:07:52.194842 vectorlab-1.0.3/vectorlab/data/tests/test_data_generator.py
+-rw-r--r--   0        0        0       23 2023-04-24 06:07:52.194842 vectorlab-1.0.3/vectorlab/ensemble/__init__.py
+-rw-r--r--   0        0        0     3677 2023-04-24 06:07:52.194842 vectorlab-1.0.3/vectorlab/ensemble/_voting.py
+-rw-r--r--   0        0        0     4070 2023-04-24 06:07:52.194842 vectorlab-1.0.3/vectorlab/ensemble/tests/test_ensemble_voting.py
+-rw-r--r--   0        0        0       70 2023-04-24 06:07:52.194842 vectorlab-1.0.3/vectorlab/graph/__init__.py
+-rw-r--r--   0        0        0    11604 2023-04-24 06:07:52.194842 vectorlab-1.0.3/vectorlab/graph/_generator.py
+-rw-r--r--   0        0        0    15921 2023-04-24 06:07:52.194842 vectorlab-1.0.3/vectorlab/graph/_utils.py
+-rw-r--r--   0        0        0     1169 2023-04-24 06:07:52.194842 vectorlab-1.0.3/vectorlab/graph/tests/test_graph_generator.py
+-rw-r--r--   0        0        0     6818 2023-04-24 06:07:52.194842 vectorlab-1.0.3/vectorlab/graph/tests/test_graph_utils.py
+-rw-r--r--   0        0        0       68 2023-04-24 06:07:52.194842 vectorlab-1.0.3/vectorlab/graph/walking/__init__.py
+-rw-r--r--   0        0        0     1920 2023-04-24 06:07:52.194842 vectorlab-1.0.3/vectorlab/graph/walking/_bfs.py
+-rw-r--r--   0        0        0     1869 2023-04-24 06:07:52.194842 vectorlab-1.0.3/vectorlab/graph/walking/_dfs.py
+-rw-r--r--   0        0        0     1275 2023-04-24 06:07:52.194842 vectorlab-1.0.3/vectorlab/graph/walking/_random_walk.py
+-rw-r--r--   0        0        0     2235 2023-04-24 06:07:52.194842 vectorlab-1.0.3/vectorlab/graph/walking/tests/test_graph_walking.py
+-rw-r--r--   0        0        0       23 2023-04-24 06:07:52.194842 vectorlab-1.0.3/vectorlab/metrics/__init__.py
+-rw-r--r--   0        0        0       87 2023-04-24 06:07:52.194842 vectorlab-1.0.3/vectorlab/metrics/pairwise/__init__.py
+-rw-r--r--   0        0        0     8721 2023-04-24 06:07:52.194842 vectorlab-1.0.3/vectorlab/metrics/pairwise/_dtw.py
+-rw-r--r--   0        0        0     3329 2023-04-24 06:07:52.194842 vectorlab-1.0.3/vectorlab/metrics/pairwise/_kl_div.py
+-rw-r--r--   0        0        0     1183 2023-04-24 06:07:52.194842 vectorlab-1.0.3/vectorlab/metrics/pairwise/_lp_norm.py
+-rw-r--r--   0        0        0     3206 2023-04-24 06:07:52.194842 vectorlab-1.0.3/vectorlab/metrics/pairwise/_sbd.py
+-rw-r--r--   0        0        0     2365 2023-04-24 06:07:52.194842 vectorlab-1.0.3/vectorlab/metrics/pairwise/tests/test_metrics_pairwise.py
+-rw-r--r--   0        0        0      119 2023-04-24 06:07:52.194842 vectorlab-1.0.3/vectorlab/nn/__init__.py
+-rw-r--r--   0        0        0     4302 2023-04-28 08:09:16.372051 vectorlab-1.0.3/vectorlab/nn/_earlystopping.py
+-rw-r--r--   0        0        0     7855 2023-05-08 04:09:34.236482 vectorlab-1.0.3/vectorlab/nn/_logger.py
+-rw-r--r--   0        0        0     7154 2023-04-28 08:09:16.372051 vectorlab-1.0.3/vectorlab/nn/_resolver.py
+-rw-r--r--   0        0        0    46466 2023-05-08 04:09:34.236482 vectorlab-1.0.3/vectorlab/nn/explorer.py
+-rw-r--r--   0        0        0     2906 2023-04-24 06:07:52.198842 vectorlab-1.0.3/vectorlab/nn/functional.py
+-rw-r--r--   0        0        0      201 2023-04-24 06:07:52.198842 vectorlab-1.0.3/vectorlab/nn/models/__init__.py
+-rw-r--r--   0        0        0    18081 2023-04-24 06:07:52.198842 vectorlab-1.0.3/vectorlab/nn/models/_autoencoder.py
+-rw-r--r--   0        0        0     2303 2023-04-24 06:07:52.198842 vectorlab-1.0.3/vectorlab/nn/models/_basic_gnn.py
+-rw-r--r--   0        0        0     3679 2023-04-24 06:07:52.198842 vectorlab-1.0.3/vectorlab/nn/models/_classifier.py
+-rw-r--r--   0        0        0    11804 2023-04-24 06:07:52.198842 vectorlab-1.0.3/vectorlab/nn/models/_decoder.py
+-rw-r--r--   0        0        0    32841 2023-04-24 06:07:52.198842 vectorlab-1.0.3/vectorlab/nn/models/_encoder.py
+-rw-r--r--   0        0        0     2571 2023-04-24 06:07:52.198842 vectorlab-1.0.3/vectorlab/nn/models/_gnn_decoder.py
+-rw-r--r--   0        0        0     7574 2023-04-24 06:07:52.198842 vectorlab-1.0.3/vectorlab/nn/models/_mlp.py
+-rw-r--r--   0        0        0     5855 2023-04-24 06:07:52.198842 vectorlab-1.0.3/vectorlab/nn/models/_seq2seq.py
+-rw-r--r--   0        0        0     2155 2023-04-24 06:07:52.198842 vectorlab-1.0.3/vectorlab/nn/models/tests/test_decoder.py
+-rw-r--r--   0        0        0     2255 2023-04-24 06:07:52.198842 vectorlab-1.0.3/vectorlab/nn/models/tests/test_encoder.py
+-rw-r--r--   0        0        0     1276 2023-04-24 06:07:52.198842 vectorlab-1.0.3/vectorlab/nn/models/tests/test_seq2seq.py
+-rw-r--r--   0        0        0       44 2023-04-24 06:07:52.198842 vectorlab-1.0.3/vectorlab/nn/modules/__init__.py
+-rw-r--r--   0        0        0     1529 2023-04-24 06:07:52.198842 vectorlab-1.0.3/vectorlab/nn/modules/gnn_loss.py
+-rw-r--r--   0        0        0     2556 2023-04-24 06:07:52.198842 vectorlab-1.0.3/vectorlab/nn/modules/loss.py
+-rw-r--r--   0        0        0      743 2023-04-24 06:07:52.198842 vectorlab-1.0.3/vectorlab/nn/tests/test_explorer.py
+-rw-r--r--   0        0        0      873 2023-04-24 06:07:52.198842 vectorlab-1.0.3/vectorlab/nn/tests/test_functional.py
+-rw-r--r--   0        0        0       45 2023-04-24 06:07:52.198842 vectorlab-1.0.3/vectorlab/optimize/__init__.py
+-rw-r--r--   0        0        0     6294 2023-04-24 06:07:52.198842 vectorlab-1.0.3/vectorlab/optimize/_estimate.py
+-rw-r--r--   0        0        0    16484 2023-04-24 06:07:52.198842 vectorlab-1.0.3/vectorlab/optimize/_qap.py
+-rw-r--r--   0        0        0     2521 2023-04-24 06:07:52.198842 vectorlab-1.0.3/vectorlab/optimize/tests/test_estimate.py
+-rw-r--r--   0        0        0       69 2023-04-24 06:07:52.198842 vectorlab-1.0.3/vectorlab/plot/__init__.py
+-rw-r--r--   0        0        0      412 2023-04-24 06:07:52.198842 vectorlab-1.0.3/vectorlab/plot/_helper.py
+-rw-r--r--   0        0        0     2980 2023-04-24 06:07:52.198842 vectorlab-1.0.3/vectorlab/plot/_palettes.py
+-rw-r--r--   0        0        0    16083 2023-04-24 06:07:52.198842 vectorlab-1.0.3/vectorlab/plot/_plot.py
+-rw-r--r--   0        0        0      732 2023-04-24 06:07:52.198842 vectorlab-1.0.3/vectorlab/plot/tests/test_plot.py
+-rw-r--r--   0        0        0       76 2023-04-24 06:07:52.198842 vectorlab-1.0.3/vectorlab/series/__init__.py
+-rw-r--r--   0        0        0     8732 2023-04-24 06:07:52.198842 vectorlab-1.0.3/vectorlab/series/_preprocessing.py
+-rw-r--r--   0        0        0     2796 2023-04-24 06:07:52.198842 vectorlab-1.0.3/vectorlab/series/_utils.py
+-rw-r--r--   0        0        0      116 2023-04-24 06:07:52.198842 vectorlab-1.0.3/vectorlab/series/smoothing/__init__.py
+-rw-r--r--   0        0        0     6298 2023-04-24 06:07:52.198842 vectorlab-1.0.3/vectorlab/series/smoothing/_arima.py
+-rw-r--r--   0        0        0     7438 2023-04-24 06:07:52.198842 vectorlab-1.0.3/vectorlab/series/smoothing/_holt_winters.py
+-rw-r--r--   0        0        0    12319 2023-04-24 06:07:52.198842 vectorlab-1.0.3/vectorlab/series/smoothing/_moving_average.py
+-rw-r--r--   0        0        0     6832 2023-04-24 06:07:52.198842 vectorlab-1.0.3/vectorlab/series/smoothing/_spectral_residual.py
+-rw-r--r--   0        0        0     2333 2023-04-24 06:07:52.198842 vectorlab-1.0.3/vectorlab/series/smoothing/tests/test_series_smoothing.py
+-rw-r--r--   0        0        0     1520 2023-04-24 06:07:52.198842 vectorlab-1.0.3/vectorlab/series/tests/test_series_preprocessing.py
+-rw-r--r--   0        0        0       77 2023-04-24 06:07:52.198842 vectorlab-1.0.3/vectorlab/stats/__init__.py
+-rw-r--r--   0        0        0    15478 2023-04-24 06:07:52.198842 vectorlab-1.0.3/vectorlab/stats/_deg_graph.py
+-rw-r--r--   0        0        0    18242 2023-04-24 06:07:52.198842 vectorlab-1.0.3/vectorlab/stats/_freq_tree.py
+-rw-r--r--   0        0        0    14207 2023-04-24 06:07:52.198842 vectorlab-1.0.3/vectorlab/stats/_t_digest.py
+-rw-r--r--   0        0        0     1312 2023-04-24 06:07:52.198842 vectorlab-1.0.3/vectorlab/stats/tests/test_deg_graph.py
+-rw-r--r--   0        0        0     1311 2023-04-24 06:07:52.198842 vectorlab-1.0.3/vectorlab/stats/tests/test_freq_tree.py
+-rw-r--r--   0        0        0     1310 2023-04-24 06:07:52.198842 vectorlab-1.0.3/vectorlab/stats/tests/test_t_digest.py
+-rw-r--r--   0        0        0      110 2023-04-24 06:07:52.198842 vectorlab-1.0.3/vectorlab/utils/__init__.py
+-rw-r--r--   0        0        0     9958 2023-04-24 06:07:52.198842 vectorlab-1.0.3/vectorlab/utils/_check.py
+-rw-r--r--   0        0        0      617 2023-04-24 06:07:52.198842 vectorlab-1.0.3/vectorlab/utils/_env.py
+-rw-r--r--   0        0        0     2026 2023-04-24 06:07:52.198842 vectorlab-1.0.3/vectorlab/utils/_loading.py
+-rw-r--r--   0        0        0     2707 2023-04-24 06:07:52.198842 vectorlab-1.0.3/vectorlab/utils/_parser.py
+-rw-r--r--   0        0        0     5089 2023-04-24 06:07:52.198842 vectorlab-1.0.3/vectorlab/utils/_time.py
+-rw-r--r--   0        0        0     1123 2023-04-24 06:07:52.198842 vectorlab-1.0.3/vectorlab/utils/tests/test_time.py
+-rw-r--r--   0        0        0       45 2023-04-24 06:07:52.198842 vectorlab-1.0.3/vectorlab/vector/__init__.py
+-rw-r--r--   0        0        0    11924 2023-04-24 06:07:52.198842 vectorlab-1.0.3/vectorlab/vector/_array.py
+-rw-r--r--   0        0        0     2933 2023-04-24 06:07:52.198842 vectorlab-1.0.3/vectorlab/vector/_tensor.py
+-rw-r--r--   0        0        0     4140 2023-04-24 06:07:52.198842 vectorlab-1.0.3/vectorlab/vector/tests/test_array.py
+-rw-r--r--   0        0        0     1217 2023-04-24 06:07:52.198842 vectorlab-1.0.3/vectorlab/vector/tests/test_tensor.py
+-rw-r--r--   0        0        0     3863 1970-01-01 00:00:00.000000 vectorlab-1.0.3/PKG-INFO
```

### Comparing `vectorlab-1.0.2/LICENSE.txt` & `vectorlab-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.2/README.md` & `vectorlab-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.2/pyproject.toml` & `vectorlab-1.0.3/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -33,15 +33,17 @@
     "pillow>=9.2.0",
     "pytz>=2022.2.1",
     "dill>=0.3.5.1",
     "halo>=0.0.31",
     "pyyaml>=6.0",
     "wandb>=0.15.0",
     "torchinfo>=1.6.3",
-    "tensorboard>=2.6.0"
+    "tensorboard>=2.6.0",
+    "evaluate==0.4.0",
+    "accelerate>=0.18.0"
 ]
 
 [project.optional-dependencies]
 test = [
     "pytest>=7.1.2",
     "pytest-cov>=3.0.0",
     "pytest-repeat>=0.9.1",
@@ -50,8 +52,20 @@
 full = [
     "torch>=1.10.0",
     "torch-sparse>=0.6.12",
     "torch-cluster>=1.6.0",
     "torch-scatter>=2.0.9",
     "torch-spline-conv>=1.2.1",
     "torch-geometric>=2.0.4"
+]
+
+[tool.coverage.run]
+omit = [
+    "vectorlab/data/dataset/*"
+]
+
+[tool.coverage.report]
+exclude_lines = [
+    "raise",
+    "except",
+    "warn"
 ]
```

### Comparing `vectorlab-1.0.2/vectorlab/base.py` & `vectorlab-1.0.3/vectorlab/base.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.2/vectorlab/data/_argument_generator.py` & `vectorlab-1.0.3/vectorlab/data/_argument_generator.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.2/vectorlab/data/_data_generator.py` & `vectorlab-1.0.3/vectorlab/data/_data_generator.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.2/vectorlab/data/dataloader/_torch_dataloader.py` & `vectorlab-1.0.3/vectorlab/data/dataloader/_torch_dataloader.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.2/vectorlab/data/dataloader/_torch_geometric_dataloader.py` & `vectorlab-1.0.3/vectorlab/data/dataloader/_torch_geometric_dataloader.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.2/vectorlab/data/dataloader/tests/test_torch_dataloader.py` & `vectorlab-1.0.3/vectorlab/data/dataloader/tests/test_torch_dataloader.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.2/vectorlab/data/dataset/_torch_dataset.py` & `vectorlab-1.0.3/vectorlab/data/dataset/_torch_dataset.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.2/vectorlab/data/dataset/_ts_dataset.py` & `vectorlab-1.0.3/vectorlab/data/dataset/_ts_dataset.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.2/vectorlab/data/tests/test_data_generator.py` & `vectorlab-1.0.3/vectorlab/data/tests/test_data_generator.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.2/vectorlab/ensemble/_voting.py` & `vectorlab-1.0.3/vectorlab/ensemble/_voting.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.2/vectorlab/ensemble/tests/test_ensemble_voting.py` & `vectorlab-1.0.3/vectorlab/ensemble/tests/test_ensemble_voting.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.2/vectorlab/graph/_generator.py` & `vectorlab-1.0.3/vectorlab/graph/_generator.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.2/vectorlab/graph/_utils.py` & `vectorlab-1.0.3/vectorlab/graph/_utils.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.2/vectorlab/graph/tests/test_graph_generator.py` & `vectorlab-1.0.3/vectorlab/graph/tests/test_graph_generator.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.2/vectorlab/graph/tests/test_graph_utils.py` & `vectorlab-1.0.3/vectorlab/graph/tests/test_graph_utils.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.2/vectorlab/graph/walking/_bfs.py` & `vectorlab-1.0.3/vectorlab/graph/walking/_bfs.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.2/vectorlab/graph/walking/_dfs.py` & `vectorlab-1.0.3/vectorlab/graph/walking/_dfs.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.2/vectorlab/graph/walking/_random_walk.py` & `vectorlab-1.0.3/vectorlab/graph/walking/_random_walk.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.2/vectorlab/graph/walking/tests/test_graph_walking.py` & `vectorlab-1.0.3/vectorlab/graph/walking/tests/test_graph_walking.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.2/vectorlab/metrics/pairwise/_dtw.py` & `vectorlab-1.0.3/vectorlab/metrics/pairwise/_dtw.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.2/vectorlab/metrics/pairwise/_kl_div.py` & `vectorlab-1.0.3/vectorlab/metrics/pairwise/_kl_div.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.2/vectorlab/metrics/pairwise/_lp_norm.py` & `vectorlab-1.0.3/vectorlab/metrics/pairwise/_lp_norm.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.2/vectorlab/metrics/pairwise/_sbd.py` & `vectorlab-1.0.3/vectorlab/metrics/pairwise/_sbd.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.2/vectorlab/metrics/pairwise/tests/test_metrics_pairwise.py` & `vectorlab-1.0.3/vectorlab/metrics/pairwise/tests/test_metrics_pairwise.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.2/vectorlab/nn/_earlystopping.py` & `vectorlab-1.0.3/vectorlab/nn/_earlystopping.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.2/vectorlab/nn/_logger.py` & `vectorlab-1.0.3/vectorlab/nn/_logger.py`

 * *Files 10% similar despite different names*

```diff
@@ -73,14 +73,24 @@
         net : torch.nn.Module
             The neural network used in training.
         loss_fn : torch.nn.Module
             The loss function used in training.
         """
         raise NotImplementedError
 
+    def unwatch(self, net):
+        r"""Un-watch the model gradients.
+
+        Parameters
+        ----------
+        net : torch.nn.Module
+            The neural network used in training.
+        """
+        raise NotImplementedError
+
     def log(self, metrics, step):
         r"""Log the training metrics.
 
         metrics is in from of
         {'train': {train_metrics}, 'valid': {valid_metrics}, ...}
 
         Parameters
@@ -146,14 +156,26 @@
         net : torch.nn.Module
             The neural network used in training.
         loss_fn : torch.nn.Module
             The loss function used in training.
         """
         return
 
+    def unwatch(self, net):
+        r"""Un-watch the model gradients.
+
+        Currently not supported in tensorboard.
+
+        Parameters
+        ----------
+        net : torch.nn.Module
+            The neural network used in training.
+        """
+        return
+
     def log(self, metrics, step):
         r"""Log the training metrics.
 
         metrics is in from of
         {'train': {train_metrics}, 'valid': {valid_metrics}, ...}
 
         Parameters
@@ -241,14 +263,27 @@
             net, loss_fn,
             log='all',
             log_freq=self.freq_
         )
 
         return
 
+    def unwatch(self, net):
+        r"""Un-watch the model gradients.
+
+        Parameters
+        ----------
+        net : torch.nn.Module
+            The neural network used in training.
+        """
+
+        wandb.unwatch(net)
+
+        return
+
     def log(self, metrics, step):
         r"""Log the training metrics.
 
         metrics is in from of
         {'train': {train_metrics}, 'valid': {valid_metrics}, ...}
 
         Parameters
```

### Comparing `vectorlab-1.0.2/vectorlab/nn/_resolver.py` & `vectorlab-1.0.3/vectorlab/nn/_resolver.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.2/vectorlab/nn/explorer.py` & `vectorlab-1.0.3/vectorlab/nn/explorer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import time
 import uuid
+import evaluate
 import numpy as np
 
 from tqdm.auto import tqdm
+from accelerate import Accelerator
 from sklearn.model_selection import KFold
 
 import torch
 
 from torchinfo import summary
 from torch.utils.data import Subset
 from torch_geometric.data import Data, Batch
@@ -40,14 +42,16 @@
         The hyper-parameter k of k fold cross validation.
     batch_size : int
         The batch size of loading data.
     num_workers : int
         The number of subprocesses to load data.
     num_epochs : int
         The number of epoch to train the neural network.
+    metrics : list
+        The metrics used to evaluate.
     train_loader_fn : str, callable
         The data loader function to be used to load data from dataset
         in training process, currently supports nn and gnn.
     train_loader_kwargs: dict
         The extra arguments for initialize the training data loader.
     valid_loader_fn : str, callable
         The data loader function to be used to load data from dataset
@@ -108,14 +112,16 @@
         The hyper-parameter k of k fold cross validation.
     batch_size_ : int
         The batch size of loading data.
     num_workers_ : int
         The number of subprocesses to load data.
     num_epochs_ : int
         The number of epoch to train the neural network.
+    metrics_ : list
+        The metrics used to evaluate.
     epochs_len_ : int
         The length of epoch number.
     loader_fn_ : torch.utils.data.DataLoader, torch_geometric.loader.DataLoader
         The data loader to load the data from dataset.
     batch_input_ : list
         The list of data annotations for batch.
     net_input_ : list
@@ -189,39 +195,42 @@
     """
 
     def __init__(self,
                  net, loss_fn,
                  batch_input, net_input, loss_input,
                  k=5,
                  batch_size=32, num_workers=0, num_epochs=100,
+                 extra_metrics=None,
                  train_loader_fn='dataloader', train_loader_kwargs=None,
                  valid_loader_fn=None, valid_loader_kwargs=None,
                  test_loader_fn=None, test_loader_kwargs=None,
                  optimizer_fn='adamw',
                  learning_rate=0.1, weight_decay=0, optimizer_kwargs=None,
                  scheduler_fn='cosine_annealing_lr',
                  scheduler_kwargs=None,
                  earlystopping_fn='desc_es',
                  earlystopping_metric='loss', earlystopping_kwargs=None,
                  logger_fn='tensorboard',
                  logger_project='vectorlab_explorer_project', logger_id=None,
                  logger_freq=1,
-                 device=None,
                  parameters_dict=None):
 
         super().__init__()
 
-        self._init_devices_(device)
-
         self.k_ = int(k)
         self.batch_size_ = int(batch_size)
         self.num_workers_ = int(num_workers)
         self.num_epochs_ = int(num_epochs)
         self.epochs_len_ = int(np.floor(np.log10(self.num_epochs_) + 1))
 
+        if extra_metrics is None:
+            self.extra_metrics_ = None
+        else:
+            self.extra_metrics_ = evaluate.combine(extra_metrics)
+
         self.train_loader_fn_ = dataloader_resolver(train_loader_fn)
         self.train_loader_kwargs_ = \
             train_loader_kwargs if train_loader_kwargs else {}
 
         if valid_loader_fn is None:
             self.valid_loader_fn_ = self.train_loader_fn_
         else:
@@ -240,19 +249,14 @@
         self.loss_fn_ = loss_fn
 
         self.batch_input_ = batch_input
         self.net_input_ = net_input
         self.loss_input_ = loss_input
         self._init_input_format()
 
-        if len(self.devices_) > 1:
-            self.net_ = torch.nn.DataParallel(
-                self.net_, device_ids=self.devices_
-            )
-
         self.optimizer_fn_ = optimizer_fn
         self.learning_rate_ = learning_rate
         self.weight_decay_ = weight_decay
         self.optimizer_kwargs_ = optimizer_kwargs
         self._init_optimizer()
 
         self.scheduler_fn_ = scheduler_fn
@@ -268,61 +272,23 @@
         self.logger_project_ = logger_project
         self.logger_id_ = logger_id
         self.logger_freq_ = logger_freq
         self._init_logger()
 
         self._init_parameters_dict_(parameters_dict)
 
-        return
-
-    def _init_devices_(self, device=None):
-        r"""Automatically initialize the devices used to store the data
-        and model.
-
-        If certain device or a list of devices are given, such device(s)
-        will be used to store the data and model, otherwise, all available
-        devices will be used.
-
-        Parameters
-        ----------
-        device : str, list, optional
-            If given specified device or a list of devices, the explorer
-            will use such device(s) as desired. If no device is specified,
-            the explorer will automatically choose the device(s).
-
-        Returns
-        -------
-        self : Explorer
-            Return itself.
-        """
-
-        if device is None:
-            if torch.cuda.is_available():
-                self.devices_ = [
-                    torch.device(f'cuda:{i}')
-                    for i in range(torch.cuda.device_count())
-                ]
-                self.device_ = self.devices_[0]
-            elif (
-                hasattr(torch.backends, 'mps')
-            ) and torch.backends.mps.is_available():
-                self.devices_ = [torch.device('mps')]
-                self.device_ = self.devices_[0]
-            else:
-                self.devices_ = [torch.device('cpu')]
-                self.device_ = self.devices_[0]
-        else:
-            if isinstance(device, list):
-                self.devices_ = [torch.device(_) for _ in device]
-                self.device_ = self.devices_[0]
-            else:
-                self.devices_ = [torch.device(device)]
-                self.device_ = self.devices_[0]
+        self.accelerator_ = Accelerator()
+        self.net_, self.loss_fn_ = self.accelerator_.prepare(
+            self.net_, self.loss_fn_
+        )
+        self.optimizer_, self.scheduler_ = self.accelerator_.prepare(
+            self.optimizer_, self.scheduler_
+        )
 
-        return self
+        return
 
     def _init_optimizer(self):
         r"""Initialize proper optimizer
 
         Returns
         -------
         self : Explorer
@@ -479,23 +445,23 @@
         net_input : tuple
             Tuple of tensors to be a net input.
         loss_input : tuple
             Tuple of tensors to be a loss input.
         """
 
         net_input = tuple(
-            batch[ind[0]].to(self.device_)
+            batch[ind[0]]
             if len(ind) == 1
-            else getattr(batch[ind[0]], ind[1]).to(self.device_)
+            else getattr(batch[ind[0]], ind[1])
             for ind in self.net_input_ind_
         )
         loss_input = tuple(
-            batch[ind[0]].to(self.device_)
+            batch[ind[0]]
             if len(ind) == 1
-            else getattr(batch[ind[0]], ind[1]).to(self.device_)
+            else getattr(batch[ind[0]], ind[1])
             for ind in self.loss_input_ind_
         )
 
         return net_input, loss_input
 
     def _init_parameters_dict_(self, parameters_dict):
         r"""Generate the parameters dictionary that initialized
@@ -521,30 +487,65 @@
             self.parameters_dict_.update(self.earlystopping_kwargs_)
 
         if parameters_dict is not None:
             self.parameters_dict_.update(parameters_dict)
 
         return self
 
+    def _pbar_disable(self, verbose):
+        r"""If pbar display should be disabled.
+
+        Parameters
+        ----------
+        verbose : int
+            Level of verbose mode.
+
+        Returns
+        -------
+        bool
+            Return if pbar display should be disabled.
+        """
+
+        if (verbose > 1) and self.accelerator_.is_local_main_process:
+            return False
+        else:
+            return True
+
+    def _calc_metrics(self, verbose):
+        r"""If calculate metrics after each epoch.
+
+        Parameters
+        ----------
+        verbose : int
+            Level of verbose mode.
+
+        Returns
+        -------
+        bool
+            Return if metrics should be calculated.
+        """
+
+        if (verbose >= 1) or self.earlystopping_fn_ or self.logger_fn_:
+            return True
+        else:
+            return False
+
     def reset(self):
         r"""The reset method.
 
         This method will reset the parameters inside the neural network
         and re-initialized the optimizer and scheduler.
 
         Returns
         -------
         self : Explorer
             Return itself.
         """
 
-        if len(self.devices_) > 1:
-            self.net_.module.reset_parameters()
-        else:
-            self.net_.reset_parameters()
+        self.net_.reset_parameters()
 
         self.optimizer_ = self.optimizer_fn_(
             self.net_.parameters(),
             **self.optimizer_kwargs_
         )
         if self.scheduler_fn_:
             self.scheduler_ = self.scheduler_fn_(
@@ -552,14 +553,18 @@
                 **self.scheduler_kwargs_
             )
         if self.earlystopping_fn_:
             self.earlystopping_ = self.earlystopping_fn_(
                 **self.earlystopping_kwargs_
             )
 
+        self.optimizer_, self.scheduler_ = self.accelerator_.prepare(
+            self.optimizer_, self.scheduler_
+        )
+
         return self
 
     def _train(self, loader):
         """This is the abstract train method.
 
         This is the abstract train method that should be implemented in
         children class, and it will be used in the training process.
@@ -587,15 +592,15 @@
 
             self.optimizer_.zero_grad()
 
             output = self.net_(*net_input)
             output = output if isinstance(output, tuple) else (output, )
 
             loss = self.loss_fn_(*output, *loss_input)
-            loss.backward()
+            self.accelerator_.backward(loss)
             self.optimizer_.step()
 
         if self.scheduler_:
             self.scheduler_.step()
         if self.earlystopping_:
             self.earlystopping_.step()
 
@@ -639,130 +644,111 @@
             n_samples = batch.num_nodes
         elif isinstance(batch, Batch):
             # pytorch_geometric Batch type for graph level tasks
             n_samples = batch.num_graphs
 
         return n_samples
 
-    def _loss_evaluate(self, loader):
-        r"""The loss metrics evaluation method.
+    def _extra_metrics_transform(self, output, loss_input):
+        r"""Some extra transformations performed to calculate metrics.
 
-        We calculate the overall loss as our evaluation metrics, while the
-        way of calculating the loss is same as the process in the train part.
+        Output is in the tuple format of the neural network output, while
+        loss_input is in the tuple format to feed in to loss function.
+
+        In most cases, the first element of output should be the predictions,
+        and the first element of loss_input should be the references. However,
+        if you have more flexible format, you can overload this function as
+        you desired.
 
         Parameters
         ----------
-        loader : torch.utils.data.DataLoader
-            The data loader containing data to evaluate the trained neural
-            network.
+        output : tuple
+            The output of the neural network.
+        loss_input : tuple
+            The input of the loss function.
 
         Returns
         -------
-        metric : dict
-            The dictionary contained the evaluation metrics.
+        predictions : tensor
+            The predictions of the neural network.
+        references : tensor
+            The references of the loss function.
         """
 
-        accumulator = Accumulator(2, ['loss', 'n_samples'])
+        predictions = output[0].detach()
+        references = loss_input[0].detach()
 
-        with torch.no_grad():
-
-            for batch in loader:
-
-                if not isinstance(batch, (tuple, list)):
-                    batch = (batch, )
-
-                n_samples = self._infer_n_samples(batch[0], loader)
-
-                net_input, loss_input = self._generate_input(batch)
-
-                output = self.net_(*net_input)
-                output = output if isinstance(output, tuple) else (output, )
-
-                loss = self.loss_fn_(*output, *loss_input).item()
-                accumulator.add(
-                    {
-                        'loss': loss * n_samples,
-                        'n_samples': n_samples
-                    }
-                )
-
-        metrics = {
-            'loss': accumulator.get('loss') / accumulator.get('n_samples')
-        }
-
-        return metrics
+        return predictions, references
 
-    def _loss_acc_evaluate(self, loader):
-        r"""The loss and accuracy evaluation method.
+    def _evaluate(self, loader):
+        r"""This evaluation method.
 
-        We calculate the overall and accuracy as our evaluation metrics,
-        while the way of calculating the loss is same as the process in
-        the train part while accuracy is often used when served as a
-        classification problem.
+        We calculate the overall loss as our evaluation metrics, while the
+        way of calculating the loss is same as the process in the train part.
+        Besides, some extra metrics are also calculated during this process.
 
         Parameters
         ----------
         loader : torch.utils.data.DataLoader
-            The data loader containing data to evaluate the trained neural
-            network.
+            The data loader containing validation data to evaluate the trained
+            neural network.
 
         Returns
         -------
-        metric : dict
+        metrics : dict
             The dictionary contained the evaluation metrics.
         """
 
-        accumulator = Accumulator(3, ['loss', 'acc', 'n_samples'])
+        self.net_.eval()
+
+        accumulator = Accumulator(2, ['loss', 'n_samples'])
 
         with torch.no_grad():
 
             for batch in loader:
 
                 if not isinstance(batch, (tuple, list)):
                     batch = (batch, )
 
                 n_samples = self._infer_n_samples(batch[0], loader)
 
                 net_input, loss_input = self._generate_input(batch)
 
-                y_hat = self.net_(*net_input)
+                output = self.net_(*net_input)
+                output = output if isinstance(output, tuple) else (output, )
 
-                loss = self.loss_fn_(y_hat, *loss_input).item()
-                acc = (y_hat.argmax(axis=1) == loss_input[0]).sum().item()
+                output, loss_input = self.accelerator_.gather_for_metrics(
+                    (output, loss_input)
+                )
+                loss = self.loss_fn_(*output, *loss_input).item()
 
                 accumulator.add(
                     {
                         'loss': loss * n_samples,
-                        'acc': acc,
                         'n_samples': n_samples
                     }
                 )
 
+                if self.extra_metrics_ is not None:
+                    predictions, references = self._extra_metrics_transform(
+                        output, loss_input
+                    )
+                    self.extra_metrics_.add_batch(
+                        predictions=predictions,
+                        references=references
+                    )
+
         metrics = {
-            'loss': accumulator.get('loss') / accumulator.get('n_samples'),
-            'acc': accumulator.get('acc') / accumulator.get('n_samples')
+            'loss': accumulator.get('loss') / accumulator.get('n_samples')
         }
 
-        return metrics
-
-    def _evaluate(self, loader):
-        r"""This it the abstract performance evaluation method.
+        if self.extra_metrics_ is not None:
+            metrics.update(self.extra_metrics_.compute())
 
-        This is the abstract evaluate method that should be implemented in
-        children class, that it will evaluate the performance of trained
-        neural network.
-
-        Parameters
-        ----------
-        loader : torch.utils.data.DataLoader
-            The data loader containing validation data to evaluate the trained
-            neural network.
-        """
-
-        return self._loss_evaluate(loader)
+        return metrics
 
     def _metrics(self, train_loader, valid_loader=None):
         """Return the evaluated metrics from train and valid loader.
 
         Parameters
         ----------
         train_loader : torch.utils.data.DataLoader
@@ -824,22 +810,25 @@
 
         outputs = []
 
         self.net_.eval()
 
         with torch.no_grad():
 
-            for batch in tqdm(loader, ascii=True, disable=(verbose <= 1)):
+            for batch in tqdm(loader,
+                              ascii=True,
+                              disable=self._pbar_disable(verbose)):
 
                 if not isinstance(batch, (tuple, list)):
                     batch = (batch, )
 
                 net_input, _ = self._generate_input(batch)
 
                 output = self.net_(*net_input)
+                output = self.accelerator_.gather_for_metrics(output)
                 outputs.append(output.detach().cpu().tolist())
 
         outputs = np.concatenate(outputs)
 
         return outputs
 
     def _latent(self, loader, verbose=0):
@@ -868,22 +857,25 @@
 
         outputs = []
 
         self.net_.eval()
 
         with torch.no_grad():
 
-            for batch in tqdm(loader, ascii=True, disable=(verbose <= 1)):
+            for batch in tqdm(loader,
+                              ascii=True,
+                              disable=self._pbar_disable(verbose)):
 
                 if not isinstance(batch, (tuple, list)):
                     batch = (batch, )
 
                 net_input, _ = self._generate_input(batch)
 
                 output = self.net_.forward_latent(*net_input)
+                output = self.accelerator_.gather_for_metrics(output)
                 outputs.append(output.detach().cpu().tolist())
 
         outputs = np.concatenate(outputs)
 
         return outputs
 
     def train(
@@ -918,41 +910,19 @@
 
         Returns
         -------
         self : Explorer
             Return itself.
         """
 
-        if verbose:
+        if verbose and self.accelerator_.is_local_main_process:
             print(
                 f'Training with parameters: {self.__repr_parameters__()} '
-                f'on devices {self.devices_}'
-            )
-
-        self.best_loss_ = np.Inf
-
-        if self.logger_fn_ is not None:
-            logger = self.logger_fn_(
-                self.logger_project_, self.logger_id_,
-                freq=self.logger_freq_
+                f'on devices {self.accelerator_.device}'
             )
-        else:
-            logger = None
-
-        if logger or self.earlystopping_ or save_best or verbose > 1:
-            _calc_metrics = True
-        else:
-            _calc_metrics = False
-
-        self.net_.to(self.device_)
-        if hasattr(self.loss_fn_, 'to'):
-            self.loss_fn_.to(self.device_)
-
-        if logger:
-            logger.watch(self.net_, self.loss_fn_)
 
         train_loader = self.train_loader_fn_(
             train_dataset,
             batch_size=self.batch_size_,
             num_workers=self.num_workers_,
             shuffle=True,
             **self.train_loader_kwargs_
@@ -965,67 +935,90 @@
                 num_workers=self.num_workers_,
                 shuffle=False,
                 **self.valid_loader_kwargs_
             )
         else:
             valid_loader = None
 
+        train_loader, valid_loader = self.accelerator_.prepare(
+            train_loader, valid_loader
+        )
+
+        self.best_loss_ = np.Inf
+
+        if self.accelerator_.is_main_process:
+
+            if self.logger_fn_ is not None:
+                logger = self.logger_fn_(
+                    self.logger_project_, self.logger_id_,
+                    freq=self.logger_freq_
+                )
+                logger.watch(self.net_, self.loss_fn_)
+            else:
+                logger = None
+
         pbar = tqdm(
             range(self.num_epochs_),
             ascii=True,
-            disable=(verbose <= 1)
+            disable=self._pbar_disable(verbose)
         )
         for epoch in pbar:
             self._train(train_loader)
 
-            if _calc_metrics:
+            if self._calc_metrics(verbose) or save_best:
                 metrics_, nested_metrics_ = self._metrics(
                     train_loader, valid_loader
                 )
                 metric_repr_ = ', '.join(
                     [
                         f'{key}: {value:.3f}'
                         for key, value in metrics_.items()
                     ]
                 )
 
                 pbar.set_description(
                     f'Epoch: {epoch:0{self.epochs_len_}d}, {metric_repr_}'
                 )
 
-            if self.earlystopping_:
-                self.earlystopping_.record_metric(
-                    metrics_[self.earlystopping_metric_]
-                )
+            if self.accelerator_.is_main_process:
 
-            if logger and (epoch % logger.freq_ == 0):
-                logger.log(nested_metrics_, step=epoch)
+                if self.earlystopping_:
+                    self.earlystopping_.record_metric(
+                        metrics_[self.earlystopping_metric_]
+                    )
+
+                if logger and (epoch % logger.freq_ == 0):
+                    logger.log(nested_metrics_, step=epoch)
 
             if save_best:
                 if metrics_['loss'] < self.best_loss_:
                     self.best_loss_ = metrics_['loss']
                     self._save_best_model()
 
             if self.earlystopping_ and self.earlystopping_.is_done():
+                self.accelerator_.wait_for_everyone()
                 break
 
         _, nested_metrics_ = self._metrics(
             train_loader, valid_loader
         )
 
         self.train_loss_ = nested_metrics_['train']['loss']
 
         if valid_loader:
             self.valid_loss_ = nested_metrics_['valid']['loss']
         else:
             self.valid_loss_ = np.Inf
 
-        if logger:
-            logger.log_params(self.parameters_dict_, nested_metrics_)
-            logger.close()
+        if self.accelerator_.is_main_process:
+
+            if logger:
+                logger.log_params(self.parameters_dict_, nested_metrics_)
+                logger.unwatch(self.net_)
+                logger.close()
 
         if save_last:
             self._save_last_model()
 
         if verbose:
             print(
                 f'Result: train loss {self.train_loss_:.6f}, '
@@ -1054,49 +1047,29 @@
 
         Returns
         -------
         self : Explorer
             Return itself.
         """
 
-        if verbose:
+        if verbose and self.accelerator_.is_local_main_process:
             print(
                 f'Training with parameters: k={self.k_}, '
                 f'{self.__repr_parameters__()} '
-                f'on devices {self.devices_}'
+                f'on devices {self.accelerator_.device}'
             )
 
         accumulator = Accumulator(3, ['k_train_loss', 'k_valid_loss', 'k'])
 
         kf = KFold(n_splits=self.k_)
         for k, index in enumerate(kf.split(train_dataset)):
 
-            (train_index, valid_index) = index
-
-            if self.logger_fn_ is not None:
-                logger = self.logger_fn_(
-                    self.logger_project_, f'{self.logger_id_}-kfold-{k}',
-                    freq=self.logger_freq_
-                )
-            else:
-                logger = None
-
-            if logger or self.earlystopping_ or verbose > 1:
-                _calc_metrics = True
-            else:
-                _calc_metrics = False
-
             self.reset()
 
-            self.net_.to(self.device_)
-            if hasattr(self.loss_fn_, 'to'):
-                self.loss_fn_.to(self.device_)
-
-            if logger:
-                logger.watch(self.net_, self.loss_fn_)
+            (train_index, valid_index) = index
 
             k_train_dataset = Subset(train_dataset, train_index)
             k_valid_dataset = Subset(train_dataset, valid_index)
 
             k_train_dataloader = self.train_loader_fn_(
                 k_train_dataset,
                 batch_size=self.batch_size_,
@@ -1108,55 +1081,76 @@
                 k_valid_dataset,
                 batch_size=self.batch_size_,
                 num_workers=self.num_workers_,
                 shuffle=False,
                 **self.valid_loader_kwargs_
             )
 
+            k_train_dataloader, k_valid_dataloader = self.accelerator_.prepare(
+                k_train_dataloader, k_valid_dataloader
+            )
+
+            if self.accelerator_.is_main_process:
+
+                if self.logger_fn_ is not None:
+                    logger = self.logger_fn_(
+                        self.logger_project_, f'{self.logger_id_}-kfold-{k}',
+                        freq=self.logger_freq_
+                    )
+                    logger.watch(self.net_, self.loss_fn_)
+                else:
+                    logger = None
+
             pbar = tqdm(
                 range(self.num_epochs_),
                 ascii=True,
-                disable=(verbose <= 1)
+                disable=self._pbar_disable(verbose)
             )
             for epoch in pbar:
                 self._train(k_train_dataloader)
 
-                if _calc_metrics:
+                if self._calc_metrics(verbose):
                     k_metrics_, k_nested_metrics_ = self._metrics(
                         k_train_dataloader, k_valid_dataloader
                     )
                     metric_repr_ = ', '.join(
                         [
                             f'{key}: {value:.3f}'
                             for key, value in k_metrics_.items()
                         ]
                     )
 
                     pbar.set_description(
                         f'Epoch: {epoch:0{self.epochs_len_}d}, {metric_repr_}'
                     )
 
-                if self.earlystopping_:
-                    self.earlystopping_.record_metric(
-                        k_metrics_[self.earlystopping_metric_]
-                    )
+                if self.accelerator_.is_main_process:
 
-                if logger and (epoch % logger.freq_ == 0):
-                    logger.log(k_nested_metrics_, step=epoch)
+                    if self.earlystopping_:
+                        self.earlystopping_.record_metric(
+                            k_metrics_[self.earlystopping_metric_]
+                        )
+
+                    if logger and (epoch % logger.freq_ == 0):
+                        logger.log(k_nested_metrics_, step=epoch)
 
                 if self.earlystopping_ and self.earlystopping_.is_done():
+                    self.accelerator_.wait_for_everyone()
                     break
 
             _, k_nested_metrics_ = self._metrics(
                 k_train_dataloader, k_valid_dataloader
             )
 
-            if logger:
-                logger.log_params(self.parameters_dict_, k_nested_metrics_)
-                logger.close()
+            if self.accelerator_.is_main_process:
+
+                if logger:
+                    logger.log_params(self.parameters_dict_, k_nested_metrics_)
+                    logger.unwatch(self.net_)
+                    logger.close()
 
             accumulator.add(
                 {
                     'k_train_loss': k_nested_metrics_['train']['loss'],
                     'k_valid_loss': k_nested_metrics_['valid']['loss'],
                     'k': 1
                 }
@@ -1203,29 +1197,28 @@
 
         Returns
         -------
         outputs : np.ndarray
             Return the outputs.
         """
 
-        if verbose:
+        if verbose and self.accelerator_.is_local_main_process:
             print(
                 f'Inferring with parameters: {self.__repr_parameters__()} '
-                f'on devices {self.devices_}'
+                f'on devices {self.accelerator_.device}'
             )
 
-        self.net_.to(self.device_)
-
         test_dataloader = self.test_loader_fn_(
             test_dataset,
             batch_size=self.batch_size_,
             num_workers=self.num_workers_,
             shuffle=False,
             **self.test_loader_kwargs_
         )
+        test_dataloader = self.accelerator_.prepare(test_dataloader)
 
         self.outputs_ = self._inference(test_dataloader, verbose=verbose)
 
         return self.outputs_
 
     def latent(self, test_dataset, verbose=0):
         r"""Getting the latent representation of test dataset using
@@ -1247,29 +1240,28 @@
 
         Returns
         -------
         outputs : np.ndarray
             Return the outputs.
         """
 
-        if verbose:
+        if verbose and self.accelerator_.is_local_main_process:
             print(
                 'Getting latent representation with '
                 f'parameters: {self.__repr_parameters__()}'
             )
 
-        self.net_.to(self.device_)
-
         test_dataloader = self.test_loader_fn_(
             test_dataset,
             batch_size=self.batch_size_,
             num_workers=self.num_workers_,
             shuffle=False,
             **self.test_loader_kwargs_
         )
+        test_dataloader = self.accelerator_.prepare(test_dataloader)
 
         self.outputs_ = self._latent(test_dataloader, verbose=verbose)
 
         return self.outputs_
 
     def _save_best_model(self):
         r"""Save the best model.
@@ -1311,24 +1303,19 @@
 
         Returns
         -------
         self : Explorer
             Return itself.
         """
 
-        if isinstance(self.net_, torch.nn.DataParallel):
-            torch.save(
-                self.net_.module.state_dict(),
-                model_path
-            )
-        else:
-            torch.save(
-                self.net_.state_dict(),
-                model_path
-            )
+        self.accelerator_.wait_for_everyone()
+
+        if self.accelerator_.is_main_process:
+            unwrapped_net = self.accelerator_.unwrap_model(self.net_)
+            self.accelerator_.save(unwrapped_net.state_dict(), model_path)
 
         return self
 
     def load_model(self, model_path):
         r"""Load the model parameters from desired path.
 
         Parameters
@@ -1338,26 +1325,21 @@
 
         Returns
         -------
         self : Explorer
             Return itself.
         """
 
-        if isinstance(self.net_, torch.nn.DataParallel):
-            self.net_.module.load_state_dict(
-                torch.load(model_path, map_location=self.device_)
-            )
-        else:
-            self.net_.load_state_dict(
-                torch.load(model_path, map_location=self.device_)
-            )
+        if self.accelerator_.is_main_process:
+            unwrapped_net = self.accelerator_.unwrap_model(self.net_)
+            unwrapped_net.load_state_dict(torch.load(model_path))
 
         return self
 
-    def get_summary(self, dataset, verbose=1):
+    def get_summary(self, dataset=None, verbose=1):
         r"""Get a summary of neural network to be investigated.
 
         This function will retrieve the inferring speed, as items per
         second to show the neural network inference ability, while
         also show a detailed structure report using torchinfo summary
         report.
 
@@ -1373,63 +1355,80 @@
 
         Returns
         -------
         self : Explorer
             Return itself.
         """
 
-        self.net_.to(self.device_)
+        if dataset is None:
+            if self.accelerator_.is_local_main_process:
+                print(
+                    'Dataset is not provided, you can only get basic '
+                    'structure of neural network. For more detailed '
+                    'information, you should provide a sample dataset.'
+                )
 
         self.net_.eval()
 
-        loader = self.train_loader_fn_(
-            dataset,
-            batch_size=self.batch_size_,
-            num_workers=self.num_workers_,
-            shuffle=False,
-            **self.train_loader_kwargs_
-        )
-
-        sample_batch = next(iter(loader))
+        if dataset is None:
+            loader = None
+            sample_net_input = None
+        else:
+            loader = self.train_loader_fn_(
+                dataset,
+                batch_size=self.batch_size_,
+                num_workers=self.num_workers_,
+                shuffle=False,
+                **self.train_loader_kwargs_
+            )
+            loader = self.accelerator_.prepare(loader)
 
-        if not isinstance(sample_batch, (tuple, list)):
-            sample_batch = (sample_batch, )
+            sample_batch = next(iter(loader))
 
-        sample_net_input, _ = self._generate_input(sample_batch)
+            if not isinstance(sample_batch, (tuple, list)):
+                sample_batch = (sample_batch, )
 
-        start_ts = time.time()
-        for batch in tqdm(loader, ascii=True, disable=(verbose <= 1)):
+            sample_net_input, _ = self._generate_input(sample_batch)
 
-            if not isinstance(batch, (tuple, list)):
-                batch = (batch, )
+            start_ts = time.time()
+            for batch in tqdm(loader,
+                              ascii=True,
+                              disable=self._pbar_disable(verbose)):
 
-            net_input, _ = self._generate_input(batch)
+                if not isinstance(batch, (tuple, list)):
+                    batch = (batch, )
 
-            self.net_(*net_input)
-        end_ts = time.time()
+                net_input, _ = self._generate_input(batch)
 
-        ts = end_ts - start_ts
+                self.net_(*net_input)
+            end_ts = time.time()
 
-        self.summary_ = summary(
-            self.net_, input_data=sample_net_input,
-            verbose=0
-        )
+            ts = end_ts - start_ts
 
-        divider = "=" * self.summary_.formatting.get_total_width()
+        if self.accelerator_.is_local_main_process:
 
-        if verbose:
-            print(divider)
-            print(
-                f'Inferring {len(dataset)} data in {ts:.6f}s '
-                f'[{len(dataset) / ts:.6f}it/s]'
+            self.summary_ = summary(
+                self.net_,
+                input_data=sample_net_input,
+                verbose=0
             )
-            print(
-                f'On devices: {self.devices_}'
-            )
-            print(self.summary_)
+
+            divider = "=" * self.summary_.formatting.get_total_width()
+
+            if verbose:
+                if dataset is None:
+                    print(self.summary_)
+                else:
+                    print(divider)
+                    print(
+                        f'Inferring {len(dataset)} data in {ts:.6f}s '
+                        f'[{len(dataset) / ts:.6f}it/s] \n'
+                        f'On devices: {self.accelerator_.device}'
+                    )
+                    print(self.summary_)
 
         return self
 
     def __repr_parameters__(self):
         r"""Generate parameters representation string.
 
         Returns
```

### Comparing `vectorlab-1.0.2/vectorlab/nn/functional.py` & `vectorlab-1.0.3/vectorlab/nn/functional.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.2/vectorlab/nn/models/_autoencoder.py` & `vectorlab-1.0.3/vectorlab/nn/models/_autoencoder.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.2/vectorlab/nn/models/_basic_gnn.py` & `vectorlab-1.0.3/vectorlab/nn/models/_basic_gnn.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.2/vectorlab/nn/models/_classifier.py` & `vectorlab-1.0.3/vectorlab/nn/models/_classifier.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.2/vectorlab/nn/models/_decoder.py` & `vectorlab-1.0.3/vectorlab/nn/models/_decoder.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.2/vectorlab/nn/models/_encoder.py` & `vectorlab-1.0.3/vectorlab/nn/models/_encoder.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.2/vectorlab/nn/models/_gnn_decoder.py` & `vectorlab-1.0.3/vectorlab/nn/models/_gnn_decoder.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.2/vectorlab/nn/models/_mlp.py` & `vectorlab-1.0.3/vectorlab/nn/models/_mlp.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.2/vectorlab/nn/models/_seq2seq.py` & `vectorlab-1.0.3/vectorlab/nn/models/_seq2seq.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.2/vectorlab/nn/models/tests/test_decoder.py` & `vectorlab-1.0.3/vectorlab/nn/models/tests/test_decoder.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.2/vectorlab/nn/models/tests/test_encoder.py` & `vectorlab-1.0.3/vectorlab/nn/models/tests/test_encoder.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.2/vectorlab/nn/models/tests/test_seq2seq.py` & `vectorlab-1.0.3/vectorlab/nn/models/tests/test_seq2seq.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.2/vectorlab/nn/modules/gnn_loss.py` & `vectorlab-1.0.3/vectorlab/nn/modules/gnn_loss.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.2/vectorlab/nn/modules/loss.py` & `vectorlab-1.0.3/vectorlab/nn/modules/loss.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.2/vectorlab/nn/tests/test_explorer.py` & `vectorlab-1.0.3/vectorlab/nn/tests/test_explorer.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.2/vectorlab/nn/tests/test_functional.py` & `vectorlab-1.0.3/vectorlab/nn/tests/test_functional.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.2/vectorlab/optimize/_estimate.py` & `vectorlab-1.0.3/vectorlab/optimize/_estimate.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.2/vectorlab/optimize/_qap.py` & `vectorlab-1.0.3/vectorlab/optimize/_qap.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.2/vectorlab/optimize/tests/test_estimate.py` & `vectorlab-1.0.3/vectorlab/optimize/tests/test_estimate.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.2/vectorlab/plot/_palettes.py` & `vectorlab-1.0.3/vectorlab/plot/_palettes.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.2/vectorlab/plot/_plot.py` & `vectorlab-1.0.3/vectorlab/plot/_plot.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.2/vectorlab/plot/tests/test_plot.py` & `vectorlab-1.0.3/vectorlab/plot/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.2/vectorlab/series/_preprocessing.py` & `vectorlab-1.0.3/vectorlab/series/_preprocessing.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.2/vectorlab/series/_utils.py` & `vectorlab-1.0.3/vectorlab/series/_utils.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.2/vectorlab/series/smoothing/_arima.py` & `vectorlab-1.0.3/vectorlab/series/smoothing/_arima.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.2/vectorlab/series/smoothing/_holt_winters.py` & `vectorlab-1.0.3/vectorlab/series/smoothing/_holt_winters.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.2/vectorlab/series/smoothing/_moving_average.py` & `vectorlab-1.0.3/vectorlab/series/smoothing/_moving_average.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.2/vectorlab/series/smoothing/_spectral_residual.py` & `vectorlab-1.0.3/vectorlab/series/smoothing/_spectral_residual.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.2/vectorlab/series/smoothing/tests/test_series_smoothing.py` & `vectorlab-1.0.3/vectorlab/series/smoothing/tests/test_series_smoothing.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.2/vectorlab/series/tests/test_series_preprocessing.py` & `vectorlab-1.0.3/vectorlab/series/tests/test_series_preprocessing.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.2/vectorlab/stats/_deg_graph.py` & `vectorlab-1.0.3/vectorlab/stats/_deg_graph.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.2/vectorlab/stats/_freq_tree.py` & `vectorlab-1.0.3/vectorlab/stats/_freq_tree.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.2/vectorlab/stats/_t_digest.py` & `vectorlab-1.0.3/vectorlab/stats/_t_digest.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.2/vectorlab/stats/tests/test_deg_graph.py` & `vectorlab-1.0.3/vectorlab/stats/tests/test_deg_graph.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.2/vectorlab/stats/tests/test_freq_tree.py` & `vectorlab-1.0.3/vectorlab/stats/tests/test_freq_tree.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.2/vectorlab/stats/tests/test_t_digest.py` & `vectorlab-1.0.3/vectorlab/stats/tests/test_t_digest.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.2/vectorlab/utils/_check.py` & `vectorlab-1.0.3/vectorlab/utils/_check.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.2/vectorlab/utils/_env.py` & `vectorlab-1.0.3/vectorlab/utils/_env.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.2/vectorlab/utils/_loading.py` & `vectorlab-1.0.3/vectorlab/utils/_loading.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.2/vectorlab/utils/_parser.py` & `vectorlab-1.0.3/vectorlab/utils/_parser.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.2/vectorlab/utils/_time.py` & `vectorlab-1.0.3/vectorlab/utils/_time.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.2/vectorlab/utils/tests/test_time.py` & `vectorlab-1.0.3/vectorlab/utils/tests/test_time.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.2/vectorlab/vector/_array.py` & `vectorlab-1.0.3/vectorlab/vector/_array.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.2/vectorlab/vector/_tensor.py` & `vectorlab-1.0.3/vectorlab/vector/_tensor.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.2/vectorlab/vector/tests/test_array.py` & `vectorlab-1.0.3/vectorlab/vector/tests/test_array.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.2/vectorlab/vector/tests/test_tensor.py` & `vectorlab-1.0.3/vectorlab/vector/tests/test_tensor.py`

 * *Files identical despite different names*

### Comparing `vectorlab-1.0.2/PKG-INFO` & `vectorlab-1.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vectorlab
-Version: 1.0.2
+Version: 1.0.3
 Summary: A lab for vectors.
 Author-email: Kyle Yang <kyle.yang1995@gmail.com>, Emma Qin <emmaqin0722@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.8
@@ -23,14 +23,16 @@
 Requires-Dist: pytz>=2022.2.1
 Requires-Dist: dill>=0.3.5.1
 Requires-Dist: halo>=0.0.31
 Requires-Dist: pyyaml>=6.0
 Requires-Dist: wandb>=0.15.0
 Requires-Dist: torchinfo>=1.6.3
 Requires-Dist: tensorboard>=2.6.0
+Requires-Dist: evaluate==0.4.0
+Requires-Dist: accelerate>=0.18.0
 Requires-Dist: torch>=1.10.0 ; extra == "full"
 Requires-Dist: torch-sparse>=0.6.12 ; extra == "full"
 Requires-Dist: torch-cluster>=1.6.0 ; extra == "full"
 Requires-Dist: torch-scatter>=2.0.9 ; extra == "full"
 Requires-Dist: torch-spline-conv>=1.2.1 ; extra == "full"
 Requires-Dist: torch-geometric>=2.0.4 ; extra == "full"
 Requires-Dist: pytest>=7.1.2 ; extra == "test"
```

