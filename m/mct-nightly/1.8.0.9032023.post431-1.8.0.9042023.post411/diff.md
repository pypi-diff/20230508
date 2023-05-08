# Comparing `tmp/mct-nightly-1.8.0.9032023.post431.tar.gz` & `tmp/mct-nightly-1.8.0.9042023.post411.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mct-nightly-1.8.0.9032023.post431.tar", last modified: Thu Mar  9 00:04:31 2023, max compression
+gzip compressed data, was "mct-nightly-1.8.0.9042023.post411.tar", last modified: Sun Apr  9 00:04:12 2023, max compression
```

## Comparing `mct-nightly-1.8.0.9032023.post431.tar` & `mct-nightly-1.8.0.9042023.post411.tar`

### file list

```diff
@@ -1,573 +1,577 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.680048 mct-nightly-1.8.0.9032023.post431/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)    12038 2023-03-09 00:04:31.680048 mct-nightly-1.8.0.9032023.post431/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10198 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.636047 mct-nightly-1.8.0.9032023.post431/mct_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12038 2023-03-09 00:04:31.000000 mct-nightly-1.8.0.9032023.post431/mct_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    36750 2023-03-09 00:04:31.000000 mct-nightly-1.8.0.9032023.post431/mct_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-09 00:04:31.000000 mct-nightly-1.8.0.9032023.post431/mct_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-03-09 00:04:31.000000 mct-nightly-1.8.0.9032023.post431/mct_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-09 00:04:31.000000 mct-nightly-1.8.0.9032023.post431/mct_nightly.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.636047 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/
--rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.636047 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/analyzer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.640047 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.640047 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/back2framework/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/back2framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/back2framework/base_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/base_substitutions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.640047 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/collectors/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/collectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/collectors/base_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     6864 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/collectors/histogram_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/collectors/mean_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/collectors/min_max_per_channel_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     7929 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/collectors/statistics_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/collectors/statistics_collector_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4027 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/data_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/defaultdict.py
--rw-r--r--   0 runner    (1001) docker     (123)    22674 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/framework_implementation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6430 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/framework_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.640047 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/fusion/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/fusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5411 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/fusion/layer_fusing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.640047 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/graph/
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28855 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/graph/base_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    18516 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/graph/base_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/graph/edge.py
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/graph/functional_node.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4732 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/graph/graph_matchers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5128 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/graph/graph_searches.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.640047 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/graph/memory_graph/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/graph/memory_graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3892 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/graph/memory_graph/bipartite_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/graph/memory_graph/compute_graph_max_cut.py
--rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/graph/memory_graph/cut.py
--rw-r--r--   0 runner    (1001) docker     (123)    17057 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/graph/memory_graph/max_cut_astar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3961 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/graph/memory_graph/memory_element.py
--rw-r--r--   0 runner    (1001) docker     (123)     7175 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/graph/memory_graph/memory_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     9272 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/graph/virtual_activation_weights_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/immutable.py
--rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.640047 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/matchers/
--rwxr-xr-x   0 runner    (1001) docker     (123)      697 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/matchers/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3091 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/matchers/base_graph_filter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2210 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/matchers/base_matcher.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3706 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/matchers/edge_matcher.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1773 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/matchers/function.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2745 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/matchers/node_matcher.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1111 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/matchers/walk_matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/memory_computation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.644048 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/mixed_precision/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/mixed_precision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6804 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/mixed_precision/bit_width_setter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/mixed_precision/distance_weighting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.644048 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/mixed_precision/kpi_tools/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/mixed_precision/kpi_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_aggregation_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     7100 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_functions_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)    19342 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     8046 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/mixed_precision/mixed_precision_quantization_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6773 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_facade.py
--rw-r--r--   0 runner    (1001) docker     (123)    34634 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.644048 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/mixed_precision/search_methods/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/mixed_precision/search_methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15458 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/mixed_precision/search_methods/linear_programming.py
--rw-r--r--   0 runner    (1001) docker     (123)    25266 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/mixed_precision/sensitivity_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6333 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/mixed_precision/solution_refinement_procedure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/model_builder_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/model_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/model_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.644048 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/network_editors/
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/network_editors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17948 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/network_editors/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/network_editors/edit_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/network_editors/node_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/node_prior_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.644048 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/quantization/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/quantization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/quantization/candidate_node_quantization_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/quantization/core_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/quantization/debug_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/quantization/filter_nodes_candidates.py
--rw-r--r--   0 runner    (1001) docker     (123)    16262 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/quantization/node_quantization_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/quantization/quantization_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7244 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/quantization/quantization_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/quantization/quantization_fn_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4085 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/quantization/quantization_params_fn_selection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.648048 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/quantization/quantization_params_generation/
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/quantization/quantization_params_generation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16499 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/quantization/quantization_params_generation/error_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/quantization/quantization_params_generation/kmeans_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     7294 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/quantization/quantization_params_generation/lut_kmeans_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/quantization/quantization_params_generation/outlier_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/quantization/quantization_params_generation/power_of_two_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_activations_computation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4323 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_computation.py
--rw-r--r--   0 runner    (1001) docker     (123)    41697 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     5095 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_weights_computation.py
--rw-r--r--   0 runner    (1001) docker     (123)     9684 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/quantization/quantization_params_generation/symmetric_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     7874 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/quantization/quantization_params_generation/uniform_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/quantization/quantize_graph_weights.py
--rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/quantization/quantize_node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.648048 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/quantization/quantizers/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/quantization/quantizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/quantization/quantizers/kmeans_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/quantization/quantizers/lut_kmeans_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14176 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/quantization/quantizers/quantizers_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5166 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/quantization/quantizers/uniform_quantizers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10673 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/quantization/set_node_quantization_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7469 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/similarity_analyzer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.648048 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/statistics_correction/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/statistics_correction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/statistics_correction/apply_bias_correction_to_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/statistics_correction/apply_second_moment_correction_to_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    10260 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/statistics_correction/compute_bias_correction_of_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/statistics_correction/statistics_correction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.648048 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/substitutions/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/substitutions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/substitutions/apply_substitutions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6434 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/substitutions/batchnorm_folding.py
--rw-r--r--   0 runner    (1001) docker     (123)     5880 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/substitutions/batchnorm_reconstruction.py
--rw-r--r--   0 runner    (1001) docker     (123)     9969 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/substitutions/batchnorm_refusing.py
--rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/substitutions/linear_collapsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/substitutions/linear_collapsing_substitution.py
--rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/substitutions/residual_collapsing.py
--rw-r--r--   0 runner    (1001) docker     (123)    10978 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/substitutions/scale_equalization.py
--rw-r--r--   0 runner    (1001) docker     (123)    26858 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/substitutions/shift_negative_activation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/substitutions/softmax_shift.py
--rw-r--r--   0 runner    (1001) docker     (123)     3412 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/substitutions/virtual_activation_weights_composition.py
--rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/substitutions/weights_activation_split.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.648048 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/target_platform/
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/target_platform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/target_platform/current_tp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/target_platform/fusing.py
--rw-r--r--   0 runner    (1001) docker     (123)     9107 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/target_platform/op_quantization_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/target_platform/operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     8783 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/target_platform/target_platform_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/target_platform/target_platform_model_component.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.648048 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/target_platform/targetplatform2framework/
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/target_platform/targetplatform2framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8771 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/target_platform/targetplatform2framework/attribute_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/target_platform/targetplatform2framework/current_tpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/target_platform/targetplatform2framework/layer_filter_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/target_platform/targetplatform2framework/operations_to_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9490 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/target_platform/targetplatform2framework/target_platform_capabilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/target_platform/targetplatform2framework/target_platform_capabilities_component.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/user_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.652047 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6371 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/visualization/final_config_visualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/visualization/nn_visualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    20094 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/visualization/tensorboard_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/exporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.652047 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.652047 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/back2framework/
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/back2framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/back2framework/factory_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/back2framework/float_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/back2framework/instance_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    15658 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/back2framework/keras_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     7162 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/back2framework/mixed_precision_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    15305 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/back2framework/model_gradients.py
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/back2framework/quantized_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5007 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/default_framework_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.652047 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/graph_substitutions/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/graph_substitutions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.652047 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/graph_substitutions/substitutions/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/graph_substitutions/substitutions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/graph_substitutions/substitutions/activation_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_folding.py
--rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_reconstruction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_refusing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5610 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/graph_substitutions/substitutions/input_scaling.py
--rw-r--r--   0 runner    (1001) docker     (123)     5937 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/graph_substitutions/substitutions/linear_collapsing.py
--rw-r--r--   0 runner    (1001) docker     (123)    26902 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/graph_substitutions/substitutions/multi_head_attention_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/graph_substitutions/substitutions/relu_bound_to_power_of_2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/graph_substitutions/substitutions/remove_relu_upper_bound.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/graph_substitutions/substitutions/residual_collapsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/graph_substitutions/substitutions/scale_equalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     7714 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/graph_substitutions/substitutions/separableconv_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (123)    10776 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/graph_substitutions/substitutions/shift_negative_activation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/graph_substitutions/substitutions/softmax_shift.py
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/graph_substitutions/substitutions/virtual_activation_weights_composition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/graph_substitutions/substitutions/weights_activation_split.py
--rw-r--r--   0 runner    (1001) docker     (123)    27514 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/keras_implementation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/keras_model_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/keras_node_prior_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     8881 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/kpi_data_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.652047 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/mixed_precision/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/mixed_precision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/mixed_precision/set_layer_to_bitwidth.py
--rw-r--r--   0 runner    (1001) docker     (123)    18051 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/quantization_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.656048 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/quantizer/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/quantizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/quantizer/base_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6175 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/quantizer/fake_quant_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/quantizer/input_layer_quantize_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     4524 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/quantizer/lut_fake_quant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.656048 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/quantizer/mixed_precision/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/quantizer/mixed_precision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/quantizer/mixed_precision/quantization_config_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     6854 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/quantizer/mixed_precision/selective_activation_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    10914 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/quantizer/mixed_precision/selective_quantize_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/quantizer/mixed_precision/selective_weights_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.656048 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/reader/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/reader/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    11418 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/reader/connectivity_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.656048 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/reader/nested_model/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/reader/nested_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7906 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/reader/nested_model/edges_merger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/reader/nested_model/nested_model_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/reader/nested_model/nodes_merger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/reader/nested_model/outputs_merger.py
--rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/reader/node_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8109 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/reader/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.656048 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/statistics_correction/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/statistics_correction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/statistics_correction/apply_second_moment_correction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/tf_tensor_numpy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.656048 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/visualization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.656048 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.656048 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/back2framework/
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/back2framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/back2framework/factory_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/back2framework/float_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/back2framework/instance_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/back2framework/mixed_precision_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    17808 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/back2framework/model_gradients.py
--rw-r--r--   0 runner    (1001) docker     (123)    12685 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/back2framework/pytorch_model_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.660048 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5773 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/quantized_layer_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/wrapper_quantize_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/back2framework/quantized_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/default_framework_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.660048 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/graph_substitutions/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/graph_substitutions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.660048 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_folding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_reconstruction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_refusing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/const_holder_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/linear_collapsing.py
--rw-r--r--   0 runner    (1001) docker     (123)    38365 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/multi_head_attention_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/permute_call_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/relu_bound_to_power_of_2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/reshape_with_static_shapes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/residual_collapsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/scale_equalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     9833 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/shift_negative_activation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/softmax_shift.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/virtual_activation_weights_composition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/weights_activation_split.py
--rw-r--r--   0 runner    (1001) docker     (123)     8782 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/kpi_data_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.660048 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/mixed_precision/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/mixed_precision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/mixed_precision/mixed_precision_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/mixed_precision/set_layer_to_bitwidth.py
--rw-r--r--   0 runner    (1001) docker     (123)    25965 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/pytorch_implementation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/pytorch_node_prior_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    17587 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/quantization_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.660048 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/quantizer/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/quantizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6483 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/quantizer/fake_quant_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/quantizer/lut_fake_quant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.660048 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/reader/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12011 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/reader/graph_builders.py
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/reader/node_holders.py
--rw-r--r--   0 runner    (1001) docker     (123)     5801 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/reader/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.660048 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/statistics_correction/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/statistics_correction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/statistics_correction/apply_second_moment_correction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    23032 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.660048 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.660048 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/default_tpc/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/default_tpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.660048 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/default_tpc/latest/
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/default_tpc/latest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/default_tpc/target_platform_capabilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.660048 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/default_tpc/v1/
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/default_tpc/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6029 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/default_tpc/v1/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/default_tpc/v1/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/default_tpc/v1/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.664048 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/default_tpc/v2/
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/default_tpc/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6565 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/default_tpc/v2/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/default_tpc/v2/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/default_tpc/v2/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.664048 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/default_tpc/v3/
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/default_tpc/v3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7867 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/default_tpc/v3/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/default_tpc/v3/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/default_tpc/v3/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.664048 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/default_tpc/v3_lut/
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/default_tpc/v3_lut/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8057 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/default_tpc/v3_lut/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/default_tpc/v3_lut/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/default_tpc/v3_lut/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.664048 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/default_tpc/v4/
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/default_tpc/v4/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7867 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/default_tpc/v4/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/default_tpc/v4/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     4666 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/default_tpc/v4/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.664048 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/default_tpc/v4_lut/
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/default_tpc/v4_lut/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8057 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/default_tpc/v4_lut/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5429 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/default_tpc/v4_lut/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     4679 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/default_tpc/v4_lut/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.664048 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/default_tpc/v5/
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/default_tpc/v5/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7864 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/default_tpc/v5/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/default_tpc/v5/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     4666 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/default_tpc/v5/tpc_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/get_target_platform_capabilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.664048 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/imx500_tpc/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/imx500_tpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.664048 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/imx500_tpc/latest/
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/imx500_tpc/latest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/imx500_tpc/target_platform_capabilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.664048 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/imx500_tpc/v1/
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/imx500_tpc/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7859 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/imx500_tpc/v1/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5331 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/imx500_tpc/v1/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/imx500_tpc/v1/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.664048 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/qnnpack_tpc/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/qnnpack_tpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.664048 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/qnnpack_tpc/latest/
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/qnnpack_tpc/latest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/qnnpack_tpc/target_platform_capabilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.664048 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/qnnpack_tpc/v1/
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/qnnpack_tpc/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5923 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/qnnpack_tpc/v1/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/qnnpack_tpc/v1/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/qnnpack_tpc/v1/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.668048 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/tflite_tpc/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/tflite_tpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.668048 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/tflite_tpc/latest/
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/tflite_tpc/latest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/tflite_tpc/target_platform_capabilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.668048 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/tflite_tpc/v1/
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/tflite_tpc/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7770 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/tflite_tpc/v1/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6066 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/tflite_tpc/v1/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/tflite_tpc/v1/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.668048 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/exporter/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/exporter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.668048 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/exporter/model_exporter/
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/exporter/model_exporter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.668048 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/exporter/model_exporter/fw_agonstic/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/exporter/model_exporter/fw_agonstic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/exporter/model_exporter/fw_agonstic/exporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.668048 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/exporter/model_exporter/keras/
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/exporter/model_exporter/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/exporter/model_exporter/keras/base_keras_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6022 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_keras_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/exporter/model_exporter/keras/keras_export_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.668048 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/exporter/model_exporter/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/exporter/model_exporter/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/exporter/model_exporter/pytorch/base_pytorch_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_onnx_pytorch_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_torchscript_pytorch_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/exporter/model_exporter/pytorch/pytorch_export_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.668048 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/exporter/model_exporter/tflite/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/exporter/model_exporter/tflite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/exporter/model_exporter/tflite/fakely_quant_tflite_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8169 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/exporter/model_exporter/tflite/int8_tflite_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/exporter/model_exporter/tflite/tflite_export_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.668048 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/exporter/model_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/exporter/model_wrapper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.668048 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/exporter/model_wrapper/keras/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/exporter/model_wrapper/keras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.668048 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/exporter/model_wrapper/keras/builder/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/exporter/model_wrapper/keras/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/exporter/model_wrapper/keras/builder/fully_quantized_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6853 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/exporter/model_wrapper/keras/builder/node_to_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/exporter/model_wrapper/keras/builder/node_to_quantizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/exporter/model_wrapper/keras/validate_layer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.668048 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/exporter/model_wrapper/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/exporter/model_wrapper/pytorch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.668048 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/fully_quantized_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6239 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/node_to_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/node_to_quantizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/exporter/model_wrapper/pytorch/validate_layer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.668048 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/gptq/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/gptq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.672048 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/gptq/common/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/gptq/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11798 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/gptq/common/gptq_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/gptq/common/gptq_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/gptq/common/gptq_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/gptq/common/gptq_quantizer_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    15250 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/gptq/common/gptq_training.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.672048 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/gptq/keras/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/gptq/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/gptq/keras/gptq_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    16554 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/gptq/keras/gptq_training.py
--rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/gptq/keras/graph_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    14341 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/gptq/keras/quantization_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.672048 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/gptq/keras/quantizer/
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/gptq/keras/quantizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/gptq/keras/quantizer/base_keras_gptq_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/gptq/keras/quantizer/quant_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/gptq/keras/quantizer/quantization_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.672048 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15326 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/symmetric_soft_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.672048 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/symmetric_ste.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.672048 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/gptq/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/gptq/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/gptq/pytorch/gptq_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    14105 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/gptq/pytorch/gptq_training.py
--rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/gptq/pytorch/graph_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    13255 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/gptq/pytorch/quantization_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.672048 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/gptq/pytorch/quantizer/
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/gptq/pytorch/quantizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4884 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/gptq/pytorch/quantizer/base_pytorch_gptq_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/gptq/pytorch/quantizer/quant_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/gptq/pytorch/quantizer/quantization_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.672048 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15172 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/symmetric_soft_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.672048 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9532 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/symmetric_ste.py
--rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/gptq/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.672048 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/ptq/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/ptq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.672048 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/ptq/keras/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/ptq/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9681 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/ptq/keras/quantization_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.672048 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/ptq/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/ptq/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8364 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/ptq/pytorch/quantization_facade.py
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/ptq/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.672048 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/qat/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/qat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.672048 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/qat/common/
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/qat/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/qat/common/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/qat/common/qat_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.672048 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/qat/keras/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/qat/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14790 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/qat/keras/quantization_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.672048 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/qat/keras/quantizer/
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/qat/keras/quantizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/qat/keras/quantizer/base_keras_qat_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/qat/keras/quantizer/quant_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/qat/keras/quantizer/quantization_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.676048 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/qat/keras/quantizer/ste_rounding/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/qat/keras/quantizer/ste_rounding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13820 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/qat/keras/quantizer/ste_rounding/symmetric_ste.py
--rw-r--r--   0 runner    (1001) docker     (123)    11089 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/qat/keras/quantizer/ste_rounding/uniform_ste.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.676048 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/qat/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/qat/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11875 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/qat/pytorch/quantization_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.676048 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/qat/pytorch/quantizer/
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/qat/pytorch/quantizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/qat/pytorch/quantizer/base_pytorch_qat_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/qat/pytorch/quantizer/quantization_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/qat/pytorch/quantizer/quantizer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.676048 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9735 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/symmetric_ste.py
--rw-r--r--   0 runner    (1001) docker     (123)     8673 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/uniform_ste.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.676048 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.676048 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.676048 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/common/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4599 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/common/activation_lut_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/common/base_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/common/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/common/get_all_subclasses.py
--rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/common/get_quantizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/common/quant_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.676048 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/load_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    14646 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantize_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.676048 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/
--rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.676048 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/activation_inferable_quantizers/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/activation_inferable_quantizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7485 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3961 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5248 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/base_keras_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.676048 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/weights_inferable_quantizers/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/weights_inferable_quantizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9459 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8664 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/validation_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.676048 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10937 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantize_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.680048 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.680048 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/activation_inferable_quantizers/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/activation_inferable_quantizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4871 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/base_lut_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/base_pytorch_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/base_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/base_uniform_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.680048 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/weights_inferable_quantizers/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/weights_inferable_quantizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5394 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.680048 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.680048 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/common/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6408 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/common/base_trainable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6333 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/common/get_quantizer_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/common/get_quantizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/common/quant_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/common/trainable_quantizer_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.680048 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/keras/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/keras/base_keras_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/keras/config_serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/keras/quantizer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 00:04:31.680048 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-03-09 00:03:54.000000 mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/pytorch/base_pytorch_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-03-09 00:04:31.680048 mct-nightly-1.8.0.9032023.post431/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-03-09 00:04:31.000000 mct-nightly-1.8.0.9032023.post431/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.871868 mct-nightly-1.8.0.9042023.post411/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    12035 2023-04-09 00:04:12.871868 mct-nightly-1.8.0.9042023.post411/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10195 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.823868 mct-nightly-1.8.0.9042023.post411/mct_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12035 2023-04-09 00:04:12.000000 mct-nightly-1.8.0.9042023.post411/mct_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    37136 2023-04-09 00:04:12.000000 mct-nightly-1.8.0.9042023.post411/mct_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 00:04:12.000000 mct-nightly-1.8.0.9042023.post411/mct_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-09 00:04:12.000000 mct-nightly-1.8.0.9042023.post411/mct_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-09 00:04:12.000000 mct-nightly-1.8.0.9042023.post411/mct_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.823868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/
+-rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.823868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/analyzer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.827868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.827868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/back2framework/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/back2framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/back2framework/base_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/base_substitutions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.827868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/collectors/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/collectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/collectors/base_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6864 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/collectors/histogram_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/collectors/mean_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/collectors/min_max_per_channel_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7929 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/collectors/statistics_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/collectors/statistics_collector_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4027 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/defaultdict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22674 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/framework_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6430 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/framework_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.827868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/fusion/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/fusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5411 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/fusion/layer_fusing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.827868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28855 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/graph/base_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18516 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/graph/base_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/graph/edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/graph/functional_node.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4732 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/graph/graph_matchers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5128 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/graph/graph_searches.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.827868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/graph/memory_graph/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/graph/memory_graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3892 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/graph/memory_graph/bipartite_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/graph/memory_graph/compute_graph_max_cut.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/graph/memory_graph/cut.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17057 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/graph/memory_graph/max_cut_astar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3961 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/graph/memory_graph/memory_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7175 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/graph/memory_graph/memory_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9272 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/graph/virtual_activation_weights_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/immutable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.827868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/matchers/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      697 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/matchers/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3091 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/matchers/base_graph_filter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2210 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/matchers/base_matcher.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3706 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/matchers/edge_matcher.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1773 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/matchers/function.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2745 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/matchers/node_matcher.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1111 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/matchers/walk_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/memory_computation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.831868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/mixed_precision/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/mixed_precision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6804 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/mixed_precision/bit_width_setter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/mixed_precision/distance_weighting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.831868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/mixed_precision/kpi_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/mixed_precision/kpi_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_aggregation_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7100 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_functions_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19342 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8046 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/mixed_precision/mixed_precision_quantization_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6773 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_facade.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34634 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.831868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/mixed_precision/search_methods/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/mixed_precision/search_methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15458 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/mixed_precision/search_methods/linear_programming.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25266 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/mixed_precision/sensitivity_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6333 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/mixed_precision/solution_refinement_procedure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/model_builder_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/model_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/model_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.831868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/network_editors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/network_editors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17948 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/network_editors/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/network_editors/edit_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/network_editors/node_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/node_prior_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.831868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/candidate_node_quantization_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/core_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/debug_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/filter_nodes_candidates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16262 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/node_quantization_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/quantization_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7244 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/quantization_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/quantization_fn_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4085 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/quantization_params_fn_selection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.835868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/quantization_params_generation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/quantization_params_generation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16499 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/quantization_params_generation/error_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/quantization_params_generation/kmeans_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7294 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/quantization_params_generation/lut_kmeans_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/quantization_params_generation/outlier_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/quantization_params_generation/power_of_two_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_activations_computation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4323 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_computation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41697 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5095 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_weights_computation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9684 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/quantization_params_generation/symmetric_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7874 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/quantization_params_generation/uniform_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/quantize_graph_weights.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/quantize_node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.835868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/quantizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/quantizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/quantizers/kmeans_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/quantizers/lut_kmeans_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14176 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/quantizers/quantizers_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5166 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/quantizers/uniform_quantizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10673 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/set_node_quantization_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7469 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/similarity_analyzer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.835868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/statistics_correction/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/statistics_correction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/statistics_correction/apply_bias_correction_to_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/statistics_correction/apply_second_moment_correction_to_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10260 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/statistics_correction/compute_bias_correction_of_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/statistics_correction/statistics_correction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.835868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/substitutions/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/substitutions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/substitutions/apply_substitutions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6434 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/substitutions/batchnorm_folding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5880 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/substitutions/batchnorm_reconstruction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9969 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/substitutions/batchnorm_refusing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/substitutions/linear_collapsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/substitutions/linear_collapsing_substitution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/substitutions/residual_collapsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10978 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/substitutions/scale_equalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26858 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/substitutions/shift_negative_activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/substitutions/softmax_shift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3412 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/substitutions/virtual_activation_weights_composition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/substitutions/weights_activation_split.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.839868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/target_platform/
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/target_platform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/target_platform/current_tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/target_platform/fusing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9107 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/target_platform/op_quantization_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/target_platform/operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8783 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/target_platform/target_platform_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/target_platform/target_platform_model_component.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.839868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/target_platform/targetplatform2framework/
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/target_platform/targetplatform2framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8771 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/target_platform/targetplatform2framework/attribute_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/target_platform/targetplatform2framework/current_tpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/target_platform/targetplatform2framework/layer_filter_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/target_platform/targetplatform2framework/operations_to_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9490 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/target_platform/targetplatform2framework/target_platform_capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/target_platform/targetplatform2framework/target_platform_capabilities_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/user_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.839868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6371 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/visualization/final_config_visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/visualization/nn_visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20094 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/visualization/tensorboard_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/exporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.839868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.839868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/back2framework/
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/back2framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/back2framework/factory_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/back2framework/float_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/back2framework/instance_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15658 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/back2framework/keras_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7162 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/back2framework/mixed_precision_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15340 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/back2framework/model_gradients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/back2framework/quantized_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5007 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/default_framework_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.839868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/graph_substitutions/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/graph_substitutions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.843868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/graph_substitutions/substitutions/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/graph_substitutions/substitutions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/graph_substitutions/substitutions/activation_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_folding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_reconstruction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_refusing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5610 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/graph_substitutions/substitutions/input_scaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5937 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/graph_substitutions/substitutions/linear_collapsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26902 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/graph_substitutions/substitutions/multi_head_attention_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/graph_substitutions/substitutions/relu_bound_to_power_of_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/graph_substitutions/substitutions/remove_relu_upper_bound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/graph_substitutions/substitutions/residual_collapsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/graph_substitutions/substitutions/scale_equalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7714 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/graph_substitutions/substitutions/separableconv_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10776 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/graph_substitutions/substitutions/shift_negative_activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/graph_substitutions/substitutions/softmax_shift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/graph_substitutions/substitutions/virtual_activation_weights_composition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/graph_substitutions/substitutions/weights_activation_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27514 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/keras_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/keras_model_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/keras_node_prior_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8881 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/kpi_data_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.843868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/mixed_precision/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/mixed_precision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/mixed_precision/set_layer_to_bitwidth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18032 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/quantization_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.843868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/quantizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/quantizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/quantizer/base_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6175 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/quantizer/fake_quant_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/quantizer/input_layer_quantize_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4524 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/quantizer/lut_fake_quant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.843868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/quantizer/mixed_precision/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/quantizer/mixed_precision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/quantizer/mixed_precision/quantization_config_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6854 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/quantizer/mixed_precision/selective_activation_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10914 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/quantizer/mixed_precision/selective_quantize_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/quantizer/mixed_precision/selective_weights_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.843868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/reader/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/reader/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11418 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/reader/connectivity_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.843868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/reader/nested_model/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/reader/nested_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7906 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/reader/nested_model/edges_merger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/reader/nested_model/nested_model_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/reader/nested_model/nodes_merger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/reader/nested_model/outputs_merger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/reader/node_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8109 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/reader/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.843868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/statistics_correction/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/statistics_correction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/statistics_correction/apply_second_moment_correction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/tf_tensor_numpy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.843868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/visualization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.847868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.847868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/back2framework/
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/back2framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/back2framework/factory_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/back2framework/float_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/back2framework/instance_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/back2framework/mixed_precision_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18238 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/back2framework/model_gradients.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12685 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/back2framework/pytorch_model_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.847868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5773 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/quantized_layer_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/wrapper_quantize_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/back2framework/quantized_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/default_framework_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.847868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/graph_substitutions/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/graph_substitutions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.847868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_folding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_reconstruction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_refusing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/const_holder_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/linear_collapsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38365 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/multi_head_attention_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/permute_call_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/relu_bound_to_power_of_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/reshape_with_static_shapes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/residual_collapsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/scale_equalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9833 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/shift_negative_activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/softmax_shift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/virtual_activation_weights_composition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/weights_activation_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8782 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/kpi_data_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.851868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/mixed_precision/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/mixed_precision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/mixed_precision/mixed_precision_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/mixed_precision/set_layer_to_bitwidth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25965 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/pytorch_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/pytorch_node_prior_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17587 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/quantization_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.851868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/quantizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/quantizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6483 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/quantizer/fake_quant_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/quantizer/lut_fake_quant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.851868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/reader/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12011 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/reader/graph_builders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/reader/node_holders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5801 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/reader/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.851868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/statistics_correction/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/statistics_correction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/statistics_correction/apply_second_moment_correction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23032 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.851868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.851868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.851868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/latest/
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/latest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/target_platform_capabilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.851868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6029 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v1/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v1/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v1/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.851868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6565 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v2/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v2/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v2/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.851868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v3/
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7867 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v3/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v3/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v3/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.851868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v3_lut/
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v3_lut/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8057 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v3_lut/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v3_lut/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v3_lut/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.851868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v4/
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v4/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7867 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v4/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v4/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4666 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v4/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.851868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v4_lut/
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v4_lut/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8057 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v4_lut/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5429 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v4_lut/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4679 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v4_lut/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.855868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v5/
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v5/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7864 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v5/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v5/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4666 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v5/tpc_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/get_target_platform_capabilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.855868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/imx500_tpc/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/imx500_tpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.855868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/imx500_tpc/latest/
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/imx500_tpc/latest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/imx500_tpc/target_platform_capabilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.855868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/imx500_tpc/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/imx500_tpc/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7859 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/imx500_tpc/v1/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5331 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/imx500_tpc/v1/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/imx500_tpc/v1/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.855868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/qnnpack_tpc/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/qnnpack_tpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.855868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/qnnpack_tpc/latest/
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/qnnpack_tpc/latest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/qnnpack_tpc/target_platform_capabilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.855868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/qnnpack_tpc/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/qnnpack_tpc/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5923 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/qnnpack_tpc/v1/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/qnnpack_tpc/v1/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/qnnpack_tpc/v1/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.855868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/tflite_tpc/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/tflite_tpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.855868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/tflite_tpc/latest/
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/tflite_tpc/latest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/tflite_tpc/target_platform_capabilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.855868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/tflite_tpc/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/tflite_tpc/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7770 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/tflite_tpc/v1/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6066 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/tflite_tpc/v1/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/tflite_tpc/v1/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.855868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.855868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_exporter/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_exporter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.855868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_exporter/fw_agonstic/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_exporter/fw_agonstic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_exporter/fw_agonstic/exporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.855868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_exporter/keras/
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_exporter/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_exporter/keras/base_keras_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6022 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_keras_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_exporter/keras/keras_export_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.855868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_exporter/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_exporter/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_exporter/pytorch/base_pytorch_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_onnx_pytorch_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_torchscript_pytorch_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_exporter/pytorch/pytorch_export_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.859868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_exporter/tflite/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_exporter/tflite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_exporter/tflite/fakely_quant_tflite_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8169 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_exporter/tflite/int8_tflite_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_exporter/tflite/tflite_export_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.859868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_wrapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.859868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_wrapper/keras/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_wrapper/keras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.859868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_wrapper/keras/builder/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_wrapper/keras/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_wrapper/keras/builder/fully_quantized_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8596 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_wrapper/keras/builder/node_to_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_wrapper/keras/builder/node_to_quantizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_wrapper/keras/validate_layer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.859868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_wrapper/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_wrapper/pytorch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.859868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/fully_quantized_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7674 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/node_to_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/node_to_quantizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_wrapper/pytorch/validate_layer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.859868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.859868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9507 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/common/gptq_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/common/gptq_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/common/gptq_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15106 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/common/gptq_training.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.859868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/keras/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/keras/gptq_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15891 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/keras/gptq_training.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/keras/graph_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14112 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/keras/quantization_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.859868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/keras/quantizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/keras/quantizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/keras/quantizer/base_keras_gptq_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/keras/quantizer/quant_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/keras/quantizer/quantization_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/keras/quantizer/regularization_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.859868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/soft_quantizer_reg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12060 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/symmetric_soft_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.859868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8539 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/symmetric_ste.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.859868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/pytorch/gptq_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13516 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/pytorch/gptq_training.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/pytorch/graph_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12468 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/pytorch/quantization_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.863868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/pytorch/quantizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/pytorch/quantizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/pytorch/quantizer/base_pytorch_gptq_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/pytorch/quantizer/quant_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4221 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/pytorch/quantizer/quantization_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/pytorch/quantizer/regularization_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.863868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/soft_quantizer_reg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12180 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/symmetric_soft_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9191 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/uniform_soft_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.863868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8932 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/symmetric_ste.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.863868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/ptq/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/ptq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.863868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/ptq/keras/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/ptq/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9681 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/ptq/keras/quantization_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.863868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/ptq/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/ptq/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8364 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/ptq/pytorch/quantization_facade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/ptq/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.863868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.863868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/common/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/common/qat_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.863868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/keras/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14790 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/keras/quantization_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.863868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/keras/quantizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/keras/quantizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/keras/quantizer/base_keras_qat_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/keras/quantizer/quant_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/keras/quantizer/quantization_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.863868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/keras/quantizer/ste_rounding/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/keras/quantizer/ste_rounding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13599 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/keras/quantizer/ste_rounding/symmetric_ste.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10939 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/keras/quantizer/ste_rounding/uniform_ste.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.863868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11875 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/pytorch/quantization_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.867868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/pytorch/quantizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/pytorch/quantizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/pytorch/quantizer/base_pytorch_qat_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/pytorch/quantizer/quantization_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/pytorch/quantizer/quantizer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.867868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9766 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/symmetric_ste.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8810 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/uniform_ste.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.867868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.867868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.867868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/common/base_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/common/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/common/get_all_subclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/common/get_quantizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/common/quant_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.867868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/load_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14646 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantize_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.867868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.867868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/activation_inferable_quantizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/activation_inferable_quantizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7485 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3961 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5248 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/base_keras_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.867868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/weights_inferable_quantizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/weights_inferable_quantizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9459 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8664 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/validation_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.867868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11272 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantize_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.871868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.871868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/activation_inferable_quantizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/activation_inferable_quantizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4599 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4871 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/base_lut_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/base_pytorch_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/base_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/base_uniform_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.871868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/weights_inferable_quantizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/weights_inferable_quantizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5394 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.871868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.871868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7775 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/common/base_trainable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6333 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/common/get_quantizer_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/common/get_quantizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/common/quant_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/common/trainable_quantizer_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.871868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/keras/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/keras/base_keras_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/keras/config_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/keras/quantizer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:04:12.871868 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-04-09 00:03:25.000000 mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/pytorch/base_pytorch_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-09 00:04:12.875868 mct-nightly-1.8.0.9042023.post411/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-04-09 00:04:11.000000 mct-nightly-1.8.0.9042023.post411/setup.py
```

### Comparing `mct-nightly-1.8.0.9032023.post431/LICENSE.md` & `mct-nightly-1.8.0.9042023.post411/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/PKG-INFO` & `mct-nightly-1.8.0.9042023.post411/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mct-nightly
-Version: 1.8.0.9032023.post431
+Version: 1.8.0.9042023.post411
 Summary: A Model Compression Toolkit for neural networks
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: # Model Compression Toolkit (MCT)
         
         Model Compression Toolkit (MCT) is an open-source project for neural network model optimization under efficient, constrained hardware.
         
@@ -25,16 +25,16 @@
         - [Results](#results)
         - [Contributions](#contributions)
         - [License](#license)
         
         ## Supported Features
         
         MCT supports different quantization methods:
-        * Post training quantization (PTQ): [Keras API](https://sony.github.io/model_optimization/docs/api/experimental_api_docs/methods/keras_post_training_quantization_experimental.html#ug-keras-post-training-quantization-experimental), [PyTorch API](https://sony.github.io/model_optimization/docs/api/experimental_api_docs/methods/pytorch_post_training_quantization_experimental.html#ug-pytorch-post-training-quantization-experimental)
-        * Gradient-based post training quantization (GPTQ): [Keras API](https://sony.github.io/model_optimization/docs/api/experimental_api_docs/methods/keras_gradient_post_training_quantization_experimental.html#ug-keras-gradient-post-training-quantization-experimental), [PyTorch API](https://sony.github.io/model_optimization/docs/api/experimental_api_docs/methods/pytorch_gradient_post_training_quantization_experimental.html#ug-pytorch-gradient-post-training-quantization-experimental)
+        * Post-training quantization (PTQ): [Keras API](https://sony.github.io/model_optimization/docs/api/experimental_api_docs/methods/keras_post_training_quantization_experimental.html#ug-keras-post-training-quantization-experimental), [PyTorch API](https://sony.github.io/model_optimization/docs/api/experimental_api_docs/methods/pytorch_post_training_quantization_experimental.html#ug-pytorch-post-training-quantization-experimental)
+        * Gradient-based post-training quantization (GPTQ): [Keras API](https://sony.github.io/model_optimization/docs/api/experimental_api_docs/methods/keras_gradient_post_training_quantization_experimental.html#ug-keras-gradient-post-training-quantization-experimental), [PyTorch API](https://sony.github.io/model_optimization/docs/api/experimental_api_docs/methods/pytorch_gradient_post_training_quantization_experimental.html#ug-pytorch-gradient-post-training-quantization-experimental)
         * Quantization aware training (QAT)[*](#experimental-features)
         
         
         | Quantization Method | Complexity                                    | Computational Cost          |
         |---------------------|-----------------------------------------------|-----------------------------|
         | PTQ                 | Low                                           | Low (order of minutes)      |
         | GPTQ                | Mild (parameters fine-tuning using gradients) | Mild (order of 2-3 hours)   |
@@ -83,23 +83,23 @@
         ```
         
         A nightly package is also available (unstable):
         ```
         pip install mct-nightly
         ```
         
-        ### Requierments
+        ### Requirements
         
-        To run MCT, one of the supported frameworks, Tenosflow/Pytorch, needs to be installed.
+        To run MCT, one of the supported frameworks, Tensorflow/Pytorch, needs to be installed.
         
-        For using with Tensorflow please install the packages: 
+        For use with Tensorflow please install the packages: 
         [tensorflow](https://www.tensorflow.org/install), 
         [tensorflow-model-optimization](https://www.tensorflow.org/model_optimization/guide/install)
         
-        For using with PyTorch please install the packages: 
+        For use with PyTorch please install the packages: 
         [torch](https://pytorch.org/)
         
         Also, a [requirements](requirements.txt) file can be used to set up your environment.
         
         
         ### Supported Python Versions
```

### Comparing `mct-nightly-1.8.0.9032023.post431/README.md` & `mct-nightly-1.8.0.9042023.post411/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 - [Results](#results)
 - [Contributions](#contributions)
 - [License](#license)
 
 ## Supported Features
 
 MCT supports different quantization methods:
-* Post training quantization (PTQ): [Keras API](https://sony.github.io/model_optimization/docs/api/experimental_api_docs/methods/keras_post_training_quantization_experimental.html#ug-keras-post-training-quantization-experimental), [PyTorch API](https://sony.github.io/model_optimization/docs/api/experimental_api_docs/methods/pytorch_post_training_quantization_experimental.html#ug-pytorch-post-training-quantization-experimental)
-* Gradient-based post training quantization (GPTQ): [Keras API](https://sony.github.io/model_optimization/docs/api/experimental_api_docs/methods/keras_gradient_post_training_quantization_experimental.html#ug-keras-gradient-post-training-quantization-experimental), [PyTorch API](https://sony.github.io/model_optimization/docs/api/experimental_api_docs/methods/pytorch_gradient_post_training_quantization_experimental.html#ug-pytorch-gradient-post-training-quantization-experimental)
+* Post-training quantization (PTQ): [Keras API](https://sony.github.io/model_optimization/docs/api/experimental_api_docs/methods/keras_post_training_quantization_experimental.html#ug-keras-post-training-quantization-experimental), [PyTorch API](https://sony.github.io/model_optimization/docs/api/experimental_api_docs/methods/pytorch_post_training_quantization_experimental.html#ug-pytorch-post-training-quantization-experimental)
+* Gradient-based post-training quantization (GPTQ): [Keras API](https://sony.github.io/model_optimization/docs/api/experimental_api_docs/methods/keras_gradient_post_training_quantization_experimental.html#ug-keras-gradient-post-training-quantization-experimental), [PyTorch API](https://sony.github.io/model_optimization/docs/api/experimental_api_docs/methods/pytorch_gradient_post_training_quantization_experimental.html#ug-pytorch-gradient-post-training-quantization-experimental)
 * Quantization aware training (QAT)[*](#experimental-features)
 
 
 | Quantization Method | Complexity                                    | Computational Cost          |
 |---------------------|-----------------------------------------------|-----------------------------|
 | PTQ                 | Low                                           | Low (order of minutes)      |
 | GPTQ                | Mild (parameters fine-tuning using gradients) | Mild (order of 2-3 hours)   |
@@ -77,23 +77,23 @@
 ```
 
 A nightly package is also available (unstable):
 ```
 pip install mct-nightly
 ```
 
-### Requierments
+### Requirements
 
-To run MCT, one of the supported frameworks, Tenosflow/Pytorch, needs to be installed.
+To run MCT, one of the supported frameworks, Tensorflow/Pytorch, needs to be installed.
 
-For using with Tensorflow please install the packages: 
+For use with Tensorflow please install the packages: 
 [tensorflow](https://www.tensorflow.org/install), 
 [tensorflow-model-optimization](https://www.tensorflow.org/model_optimization/guide/install)
 
-For using with PyTorch please install the packages: 
+For use with PyTorch please install the packages: 
 [torch](https://pytorch.org/)
 
 Also, a [requirements](requirements.txt) file can be used to set up your environment.
 
 
 ### Supported Python Versions
```

### Comparing `mct-nightly-1.8.0.9032023.post431/mct_nightly.egg-info/PKG-INFO` & `mct-nightly-1.8.0.9042023.post411/mct_nightly.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mct-nightly
-Version: 1.8.0.9032023.post431
+Version: 1.8.0.9042023.post411
 Summary: A Model Compression Toolkit for neural networks
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: # Model Compression Toolkit (MCT)
         
         Model Compression Toolkit (MCT) is an open-source project for neural network model optimization under efficient, constrained hardware.
         
@@ -25,16 +25,16 @@
         - [Results](#results)
         - [Contributions](#contributions)
         - [License](#license)
         
         ## Supported Features
         
         MCT supports different quantization methods:
-        * Post training quantization (PTQ): [Keras API](https://sony.github.io/model_optimization/docs/api/experimental_api_docs/methods/keras_post_training_quantization_experimental.html#ug-keras-post-training-quantization-experimental), [PyTorch API](https://sony.github.io/model_optimization/docs/api/experimental_api_docs/methods/pytorch_post_training_quantization_experimental.html#ug-pytorch-post-training-quantization-experimental)
-        * Gradient-based post training quantization (GPTQ): [Keras API](https://sony.github.io/model_optimization/docs/api/experimental_api_docs/methods/keras_gradient_post_training_quantization_experimental.html#ug-keras-gradient-post-training-quantization-experimental), [PyTorch API](https://sony.github.io/model_optimization/docs/api/experimental_api_docs/methods/pytorch_gradient_post_training_quantization_experimental.html#ug-pytorch-gradient-post-training-quantization-experimental)
+        * Post-training quantization (PTQ): [Keras API](https://sony.github.io/model_optimization/docs/api/experimental_api_docs/methods/keras_post_training_quantization_experimental.html#ug-keras-post-training-quantization-experimental), [PyTorch API](https://sony.github.io/model_optimization/docs/api/experimental_api_docs/methods/pytorch_post_training_quantization_experimental.html#ug-pytorch-post-training-quantization-experimental)
+        * Gradient-based post-training quantization (GPTQ): [Keras API](https://sony.github.io/model_optimization/docs/api/experimental_api_docs/methods/keras_gradient_post_training_quantization_experimental.html#ug-keras-gradient-post-training-quantization-experimental), [PyTorch API](https://sony.github.io/model_optimization/docs/api/experimental_api_docs/methods/pytorch_gradient_post_training_quantization_experimental.html#ug-pytorch-gradient-post-training-quantization-experimental)
         * Quantization aware training (QAT)[*](#experimental-features)
         
         
         | Quantization Method | Complexity                                    | Computational Cost          |
         |---------------------|-----------------------------------------------|-----------------------------|
         | PTQ                 | Low                                           | Low (order of minutes)      |
         | GPTQ                | Mild (parameters fine-tuning using gradients) | Mild (order of 2-3 hours)   |
@@ -83,23 +83,23 @@
         ```
         
         A nightly package is also available (unstable):
         ```
         pip install mct-nightly
         ```
         
-        ### Requierments
+        ### Requirements
         
-        To run MCT, one of the supported frameworks, Tenosflow/Pytorch, needs to be installed.
+        To run MCT, one of the supported frameworks, Tensorflow/Pytorch, needs to be installed.
         
-        For using with Tensorflow please install the packages: 
+        For use with Tensorflow please install the packages: 
         [tensorflow](https://www.tensorflow.org/install), 
         [tensorflow-model-optimization](https://www.tensorflow.org/model_optimization/guide/install)
         
-        For using with PyTorch please install the packages: 
+        For use with PyTorch please install the packages: 
         [torch](https://pytorch.org/)
         
         Also, a [requirements](requirements.txt) file can be used to set up your environment.
         
         
         ### Supported Python Versions
```

### Comparing `mct-nightly-1.8.0.9032023.post431/mct_nightly.egg-info/SOURCES.txt` & `mct-nightly-1.8.0.9042023.post411/mct_nightly.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -341,40 +341,44 @@
 model_compression_toolkit/exporter/model_wrapper/pytorch/builder/node_to_quantizers.py
 model_compression_toolkit/gptq/__init__.py
 model_compression_toolkit/gptq/runner.py
 model_compression_toolkit/gptq/common/__init__.py
 model_compression_toolkit/gptq/common/gptq_config.py
 model_compression_toolkit/gptq/common/gptq_constants.py
 model_compression_toolkit/gptq/common/gptq_graph.py
-model_compression_toolkit/gptq/common/gptq_quantizer_config.py
 model_compression_toolkit/gptq/common/gptq_training.py
 model_compression_toolkit/gptq/keras/__init__.py
 model_compression_toolkit/gptq/keras/gptq_loss.py
 model_compression_toolkit/gptq/keras/gptq_training.py
 model_compression_toolkit/gptq/keras/graph_info.py
 model_compression_toolkit/gptq/keras/quantization_facade.py
 model_compression_toolkit/gptq/keras/quantizer/__init__.py
 model_compression_toolkit/gptq/keras/quantizer/base_keras_gptq_quantizer.py
 model_compression_toolkit/gptq/keras/quantizer/quant_utils.py
 model_compression_toolkit/gptq/keras/quantizer/quantization_builder.py
+model_compression_toolkit/gptq/keras/quantizer/regularization_factory.py
 model_compression_toolkit/gptq/keras/quantizer/soft_rounding/__init__.py
+model_compression_toolkit/gptq/keras/quantizer/soft_rounding/soft_quantizer_reg.py
 model_compression_toolkit/gptq/keras/quantizer/soft_rounding/symmetric_soft_quantizer.py
 model_compression_toolkit/gptq/keras/quantizer/ste_rounding/__init__.py
 model_compression_toolkit/gptq/keras/quantizer/ste_rounding/symmetric_ste.py
 model_compression_toolkit/gptq/pytorch/__init__.py
 model_compression_toolkit/gptq/pytorch/gptq_loss.py
 model_compression_toolkit/gptq/pytorch/gptq_training.py
 model_compression_toolkit/gptq/pytorch/graph_info.py
 model_compression_toolkit/gptq/pytorch/quantization_facade.py
 model_compression_toolkit/gptq/pytorch/quantizer/__init__.py
 model_compression_toolkit/gptq/pytorch/quantizer/base_pytorch_gptq_quantizer.py
 model_compression_toolkit/gptq/pytorch/quantizer/quant_utils.py
 model_compression_toolkit/gptq/pytorch/quantizer/quantization_builder.py
+model_compression_toolkit/gptq/pytorch/quantizer/regularization_factory.py
 model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/__init__.py
+model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/soft_quantizer_reg.py
 model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/symmetric_soft_quantizer.py
+model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/uniform_soft_quantizer.py
 model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/__init__.py
 model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/symmetric_ste.py
 model_compression_toolkit/ptq/__init__.py
 model_compression_toolkit/ptq/runner.py
 model_compression_toolkit/ptq/keras/__init__.py
 model_compression_toolkit/ptq/keras/quantization_facade.py
 model_compression_toolkit/ptq/pytorch/__init__.py
@@ -400,15 +404,14 @@
 model_compression_toolkit/qat/pytorch/quantizer/quantizer_utils.py
 model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/__init__.py
 model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/symmetric_ste.py
 model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/uniform_ste.py
 model_compression_toolkit/quantizers_infrastructure/__init__.py
 model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/__init__.py
 model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/common/__init__.py
-model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/common/activation_lut_pot_inferable_quantizer.py
 model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/common/base_inferable_quantizer.py
 model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/common/constants.py
 model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/common/get_all_subclasses.py
 model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/common/get_quantizers.py
 model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/common/quant_utils.py
 model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/__init__.py
 model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/load_model.py
@@ -435,14 +438,15 @@
 model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/__init__.py
 model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/base_lut_symmetric_inferable_quantizer.py
 model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/base_pytorch_inferable_quantizer.py
 model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/base_symmetric_inferable_quantizer.py
 model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/base_uniform_inferable_quantizer.py
 model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/constants.py
 model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/activation_inferable_quantizers/__init__.py
+model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py
 model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py
 model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py
 model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py
 model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/weights_inferable_quantizers/__init__.py
 model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py
 model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py
 model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py
```

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,16 +10,14 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
 from model_compression_toolkit.core.common.quantization.debug_config import DebugConfig
-from model_compression_toolkit.gptq.common.gptq_config import GradientPTQConfig, RoundingType, GradientPTQConfigV2
-from model_compression_toolkit.gptq.common.gptq_quantizer_config import GPTQQuantizerConfig, SoftQuantizerConfig
 from model_compression_toolkit.core.common.quantization import quantization_config
 from model_compression_toolkit.core.common.mixed_precision import mixed_precision_quantization_config
 from model_compression_toolkit.core.common.quantization.quantization_config import QuantizationConfig, \
     QuantizationErrorMethod, DEFAULTCONFIG
 from model_compression_toolkit.core.common.quantization.core_config import CoreConfig
 from model_compression_toolkit.core.common import target_platform
 from model_compression_toolkit.core.tpc_models.get_target_platform_capabilities import get_target_platform_capabilities
@@ -32,29 +30,25 @@
 from model_compression_toolkit.core.common.framework_info import FrameworkInfo, ChannelAxis
 from model_compression_toolkit.core.common.defaultdict import DefaultDict
 from model_compression_toolkit.core.common import network_editors as network_editor
 
 from model_compression_toolkit.core.keras.quantization_facade import keras_post_training_quantization, \
     keras_post_training_quantization_mixed_precision
 from model_compression_toolkit.ptq.keras.quantization_facade import keras_post_training_quantization_experimental
-from model_compression_toolkit.gptq.keras.quantization_facade import \
-    keras_gradient_post_training_quantization_experimental
-from model_compression_toolkit.gptq.keras.quantization_facade import get_keras_gptq_config
-from model_compression_toolkit.qat.keras.quantization_facade import keras_quantization_aware_training_init, \
-    keras_quantization_aware_training_finalize
-from model_compression_toolkit.qat.pytorch.quantization_facade import pytorch_quantization_aware_training_init, \
-    pytorch_quantization_aware_training_finalize
-from model_compression_toolkit.core.pytorch.quantization_facade import pytorch_post_training_quantization, \
-    pytorch_post_training_quantization_mixed_precision
+from model_compression_toolkit.qat.keras.quantization_facade import keras_quantization_aware_training_init, keras_quantization_aware_training_finalize
+from model_compression_toolkit.qat.pytorch.quantization_facade import pytorch_quantization_aware_training_init, pytorch_quantization_aware_training_finalize
+from model_compression_toolkit.core.pytorch.quantization_facade import pytorch_post_training_quantization, pytorch_post_training_quantization_mixed_precision
 from model_compression_toolkit.ptq.pytorch.quantization_facade import pytorch_post_training_quantization_experimental
-from model_compression_toolkit.gptq.pytorch.quantization_facade import \
-    pytorch_gradient_post_training_quantization_experimental
-from model_compression_toolkit.gptq.pytorch.quantization_facade import get_pytorch_gptq_config
 
 from model_compression_toolkit.core.keras.kpi_data_facade import keras_kpi_data, keras_kpi_data_experimental
 from model_compression_toolkit.core.pytorch.kpi_data_facade import pytorch_kpi_data, pytorch_kpi_data_experimental
 
 from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.keras.load_model import keras_load_quantized_model
 
-from model_compression_toolkit.exporter.model_exporter import tflite_export_model, TFLiteExportMode, keras_export_model, KerasExportMode, pytorch_export_model, PyTorchExportMode
+
+from model_compression_toolkit import exporter
+
+from model_compression_toolkit import gptq
+from model_compression_toolkit.gptq import GradientPTQConfig
+
 
 __version__ = "1.8.0"
```

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/analyzer.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/analyzer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/back2framework/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/back2framework/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/back2framework/base_model_builder.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/back2framework/base_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/base_substitutions.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/base_substitutions.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/collectors/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/collectors/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/collectors/base_collector.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/collectors/base_collector.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/collectors/histogram_collector.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/collectors/histogram_collector.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/collectors/mean_collector.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/collectors/mean_collector.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/collectors/min_max_per_channel_collector.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/collectors/min_max_per_channel_collector.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/collectors/statistics_collector.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/collectors/statistics_collector.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/collectors/statistics_collector_generator.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/collectors/statistics_collector_generator.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/constants.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/constants.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/data_loader.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/data_loader.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/defaultdict.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/defaultdict.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/framework_implementation.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/framework_implementation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/framework_info.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/framework_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/fusion/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/fusion/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/fusion/layer_fusing.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/fusion/layer_fusing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/graph/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/graph/base_graph.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/graph/base_graph.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/graph/base_node.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/graph/base_node.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/graph/edge.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/graph/edge.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/graph/functional_node.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/graph/functional_node.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/graph/graph_matchers.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/graph/graph_matchers.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/graph/graph_searches.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/graph/graph_searches.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/graph/memory_graph/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/graph/memory_graph/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/graph/memory_graph/bipartite_graph.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/graph/memory_graph/bipartite_graph.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/graph/memory_graph/compute_graph_max_cut.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/graph/memory_graph/compute_graph_max_cut.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/graph/memory_graph/cut.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/graph/memory_graph/cut.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/graph/memory_graph/max_cut_astar.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/graph/memory_graph/max_cut_astar.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/graph/memory_graph/memory_element.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/graph/memory_graph/memory_element.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/graph/memory_graph/memory_graph.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/graph/memory_graph/memory_graph.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/graph/virtual_activation_weights_node.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/graph/virtual_activation_weights_node.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/immutable.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/immutable.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/logger.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 # limitations under the License.
 # ==============================================================================
 
 
 import logging
 import os
 from datetime import datetime
-from os import path
 from pathlib import Path
 
 LOGGER_NAME = 'Constrained Model Optimization'
 
 
 class Logger:
     # Logger has levels of verbosity.
@@ -39,15 +38,15 @@
         """
         Create a path if not exist. Otherwise, do nothing.
         Args:
             log_path: Path to create or verify that exists.
 
         """
 
-        if not path.exists(log_path):
+        if not os.path.exists(log_path):
             Path(log_path).mkdir(parents=True, exist_ok=True)
 
     @staticmethod
     def set_logger_level(log_level=logging.INFO):
         """
         Set log level to determine the logger verbosity.
         Args:
@@ -89,14 +88,23 @@
 
         fh = logging.FileHandler(log_name)
         fh.setLevel(logging.DEBUG)
         logger.addHandler(fh)
 
         print(f'log file is in {log_name}')
 
+    @staticmethod
+    def shutdown():
+        """
+        An orderly command to shutdown by flushing and closing all logging handlers.
+
+        """
+        Logger.LOG_PATH = None
+        logging.shutdown()
+
     ########################################
     # Delegating methods to wrapped logger
     ########################################
 
     @staticmethod
     def critical(msg: str):
         """
```

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/matchers/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/matchers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/matchers/base_graph_filter.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/matchers/base_graph_filter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/matchers/base_matcher.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/matchers/base_matcher.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/matchers/edge_matcher.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/matchers/edge_matcher.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/matchers/function.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/matchers/function.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/matchers/node_matcher.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/matchers/node_matcher.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/matchers/walk_matcher.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/matchers/walk_matcher.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/memory_computation.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/memory_computation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/mixed_precision/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/mixed_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/mixed_precision/bit_width_setter.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/mixed_precision/bit_width_setter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/mixed_precision/distance_weighting.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/mixed_precision/distance_weighting.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/mixed_precision/kpi_tools/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/mixed_precision/kpi_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_aggregation_methods.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_aggregation_methods.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_data.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_data.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_functions_mapping.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_functions_mapping.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_methods.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_methods.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/mixed_precision/mixed_precision_quantization_config.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/mixed_precision/mixed_precision_quantization_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_facade.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_manager.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_manager.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/mixed_precision/search_methods/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/mixed_precision/search_methods/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/mixed_precision/search_methods/linear_programming.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/mixed_precision/search_methods/linear_programming.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/mixed_precision/sensitivity_evaluation.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/mixed_precision/sensitivity_evaluation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/mixed_precision/solution_refinement_procedure.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/mixed_precision/solution_refinement_procedure.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/model_builder_mode.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/model_builder_mode.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/model_collector.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/model_collector.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/model_validation.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/model_validation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/network_editors/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/network_editors/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/network_editors/actions.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/network_editors/actions.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/network_editors/edit_network.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/network_editors/edit_network.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/network_editors/node_filters.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/network_editors/node_filters.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/node_prior_info.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/node_prior_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/quantization/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/quantization/candidate_node_quantization_config.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/candidate_node_quantization_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/quantization/core_config.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/core_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/quantization/debug_config.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/debug_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/quantization/filter_nodes_candidates.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/filter_nodes_candidates.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/quantization/node_quantization_config.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/node_quantization_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/quantization/quantization_analyzer.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/quantization_analyzer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/quantization/quantization_config.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/quantization_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/quantization/quantization_fn_selection.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/quantization_fn_selection.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/quantization/quantization_params_fn_selection.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/quantization_params_fn_selection.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/quantization/quantization_params_generation/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/quantization_params_generation/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/quantization/quantization_params_generation/error_functions.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/quantization_params_generation/error_functions.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/quantization/quantization_params_generation/kmeans_params.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/quantization_params_generation/kmeans_params.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/quantization/quantization_params_generation/lut_kmeans_params.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/quantization_params_generation/lut_kmeans_params.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/quantization/quantization_params_generation/outlier_filter.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/quantization_params_generation/outlier_filter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/quantization/quantization_params_generation/power_of_two_selection.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/quantization_params_generation/power_of_two_selection.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_activations_computation.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_activations_computation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_computation.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_computation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_search.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_search.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_weights_computation.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_weights_computation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/quantization/quantization_params_generation/symmetric_selection.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/quantization_params_generation/symmetric_selection.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/quantization/quantization_params_generation/uniform_selection.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/quantization_params_generation/uniform_selection.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/quantization/quantize_graph_weights.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/quantize_graph_weights.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/quantization/quantize_node.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/quantize_node.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/quantization/quantizers/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/quantization/quantizers/kmeans_quantizer.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/quantizers/kmeans_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/quantization/quantizers/lut_kmeans_quantizer.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/quantizers/lut_kmeans_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/quantization/quantizers/quantizers_helpers.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/quantizers/quantizers_helpers.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/quantization/quantizers/uniform_quantizers.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/quantizers/uniform_quantizers.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/quantization/set_node_quantization_config.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/quantization/set_node_quantization_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/similarity_analyzer.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/similarity_analyzer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/statistics_correction/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/statistics_correction/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/statistics_correction/apply_bias_correction_to_graph.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/statistics_correction/apply_bias_correction_to_graph.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/statistics_correction/apply_second_moment_correction_to_graph.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/statistics_correction/apply_second_moment_correction_to_graph.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/statistics_correction/compute_bias_correction_of_graph.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/statistics_correction/compute_bias_correction_of_graph.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/statistics_correction/statistics_correction.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/statistics_correction/statistics_correction.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/substitutions/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/substitutions/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/substitutions/apply_substitutions.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/substitutions/apply_substitutions.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/substitutions/batchnorm_folding.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/substitutions/batchnorm_folding.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/substitutions/batchnorm_reconstruction.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/substitutions/batchnorm_reconstruction.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/substitutions/batchnorm_refusing.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/substitutions/batchnorm_refusing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/substitutions/linear_collapsing.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/substitutions/linear_collapsing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/substitutions/linear_collapsing_substitution.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/substitutions/linear_collapsing_substitution.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/substitutions/residual_collapsing.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/substitutions/residual_collapsing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/substitutions/scale_equalization.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/substitutions/scale_equalization.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/substitutions/shift_negative_activation.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/substitutions/shift_negative_activation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/substitutions/softmax_shift.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/substitutions/softmax_shift.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/substitutions/virtual_activation_weights_composition.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/substitutions/virtual_activation_weights_composition.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/substitutions/weights_activation_split.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/substitutions/weights_activation_split.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/target_platform/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/target_platform/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/target_platform/current_tp_model.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/target_platform/current_tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/target_platform/fusing.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/target_platform/fusing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/target_platform/op_quantization_config.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/target_platform/op_quantization_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/target_platform/operators.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/target_platform/operators.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/target_platform/target_platform_model.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/target_platform/target_platform_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/target_platform/target_platform_model_component.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/target_platform/target_platform_model_component.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/target_platform/targetplatform2framework/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/target_platform/targetplatform2framework/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/target_platform/targetplatform2framework/attribute_filter.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/target_platform/targetplatform2framework/attribute_filter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/target_platform/targetplatform2framework/current_tpc.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/target_platform/targetplatform2framework/current_tpc.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/target_platform/targetplatform2framework/layer_filter_params.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/target_platform/targetplatform2framework/layer_filter_params.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/target_platform/targetplatform2framework/operations_to_layers.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/target_platform/targetplatform2framework/operations_to_layers.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/target_platform/targetplatform2framework/target_platform_capabilities.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/target_platform/targetplatform2framework/target_platform_capabilities.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/target_platform/targetplatform2framework/target_platform_capabilities_component.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/target_platform/targetplatform2framework/target_platform_capabilities_component.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/user_info.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/user_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/visualization/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/visualization/final_config_visualizer.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/visualization/final_config_visualizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/visualization/nn_visualizer.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/visualization/nn_visualizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/common/visualization/tensorboard_writer.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/common/visualization/tensorboard_writer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/exporter.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/back2framework/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/back2framework/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/back2framework/factory_model_builder.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/back2framework/factory_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/back2framework/float_model_builder.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/back2framework/float_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/back2framework/instance_builder.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/back2framework/instance_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/back2framework/keras_model_builder.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/back2framework/keras_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/back2framework/mixed_precision_model_builder.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/back2framework/mixed_precision_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/back2framework/model_gradients.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/back2framework/model_gradients.py`

 * *Files 1% similar despite different names*

```diff
@@ -167,16 +167,17 @@
                     # Computing the jacobian approximation by getting the gradient of (output * v)
                     jac_v = g.gradient(f_v, ipt, unconnected_gradients=tf.UnconnectedGradients.ZERO)
                     jac_v = tf.reshape(jac_v, [jac_v.shape[0], -1])
                     jac_trace_approx = tf.reduce_mean(tf.reduce_sum(tf.pow(jac_v, 2.0)))
 
                     # If the change to the mean Jacobian approximation is insignificant we stop the calculation
                     if j > MIN_JACOBIANS_ITER:
-                        delta = np.mean([jac_trace_approx, *trace_jv]) - np.mean(trace_jv)
-                        if np.abs(delta) / (np.abs(np.mean(trace_jv)) + 1e-6) < JACOBIANS_COMP_TOLERANCE:
+                        new_mean = np.mean([jac_trace_approx, *trace_jv])
+                        delta = new_mean - np.mean(trace_jv)
+                        if np.abs(delta) / (np.abs(new_mean) + 1e-6) < JACOBIANS_COMP_TOLERANCE:
                             trace_jv.append(jac_trace_approx)
                             break
 
                     trace_jv.append(jac_trace_approx)
             ipts_jac_trace_approx.append(2 * tf.reduce_mean(trace_jv) / output.shape[-1])  # Get averaged squared jacobian trace approximation
 
         ipts_jac_trace_approx = tf.reduce_mean([ipts_jac_trace_approx], axis=0)  # Just to get one tensor instead of list of tensors with single element
```

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/back2framework/quantized_model_builder.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/back2framework/quantized_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/constants.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/constants.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/default_framework_info.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/default_framework_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/graph_substitutions/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/graph_substitutions/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/graph_substitutions/substitutions/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/graph_substitutions/substitutions/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/graph_substitutions/substitutions/activation_decomposition.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/graph_substitutions/substitutions/activation_decomposition.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_folding.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_folding.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_reconstruction.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_reconstruction.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_refusing.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_refusing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/graph_substitutions/substitutions/input_scaling.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/graph_substitutions/substitutions/input_scaling.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/graph_substitutions/substitutions/linear_collapsing.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/graph_substitutions/substitutions/linear_collapsing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/graph_substitutions/substitutions/multi_head_attention_decomposition.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/graph_substitutions/substitutions/multi_head_attention_decomposition.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/graph_substitutions/substitutions/relu_bound_to_power_of_2.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/graph_substitutions/substitutions/relu_bound_to_power_of_2.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/graph_substitutions/substitutions/remove_relu_upper_bound.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/graph_substitutions/substitutions/remove_relu_upper_bound.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/graph_substitutions/substitutions/residual_collapsing.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/graph_substitutions/substitutions/residual_collapsing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/graph_substitutions/substitutions/scale_equalization.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/graph_substitutions/substitutions/scale_equalization.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/graph_substitutions/substitutions/separableconv_decomposition.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/graph_substitutions/substitutions/separableconv_decomposition.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/graph_substitutions/substitutions/shift_negative_activation.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/graph_substitutions/substitutions/shift_negative_activation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/graph_substitutions/substitutions/softmax_shift.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/graph_substitutions/substitutions/softmax_shift.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/graph_substitutions/substitutions/virtual_activation_weights_composition.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/graph_substitutions/substitutions/virtual_activation_weights_composition.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/graph_substitutions/substitutions/weights_activation_split.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/graph_substitutions/substitutions/weights_activation_split.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/keras_implementation.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/keras_implementation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/keras_model_validation.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/keras_model_validation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/keras_node_prior_info.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/keras_node_prior_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/kpi_data_facade.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/kpi_data_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/mixed_precision/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/mixed_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/mixed_precision/set_layer_to_bitwidth.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/mixed_precision/set_layer_to_bitwidth.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/quantization_facade.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/quantization_facade.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 from typing import Callable, List, Tuple
 
 from model_compression_toolkit.core import common
 from model_compression_toolkit.core.common import Logger
 from model_compression_toolkit.core.common.constants import TENSORFLOW
 from model_compression_toolkit.core.common.user_info import UserInformation
-from model_compression_toolkit.gptq.common.gptq_config import GradientPTQConfig, GradientPTQConfigV2
+from model_compression_toolkit.gptq import GradientPTQConfig, GradientPTQConfigV2
 from model_compression_toolkit.core.common.mixed_precision.kpi_tools.kpi import KPI
 from model_compression_toolkit.core.common.framework_info import FrameworkInfo
 from model_compression_toolkit.core.common.network_editors.actions import EditRule
 from model_compression_toolkit.core.common.mixed_precision.mixed_precision_quantization_config import \
     MixedPrecisionQuantizationConfig, DEFAULT_MIXEDPRECISION_CONFIG
 from model_compression_toolkit.core.common.quantization.quantization_config import QuantizationConfig
 from model_compression_toolkit.core.common.quantization.core_config import CoreConfig
```

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/quantizer/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/quantizer/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/quantizer/base_quantizer.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/quantizer/base_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/quantizer/fake_quant_builder.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/quantizer/fake_quant_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/quantizer/input_layer_quantize_transform.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/quantizer/input_layer_quantize_transform.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/quantizer/lut_fake_quant.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/quantizer/lut_fake_quant.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/quantizer/mixed_precision/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/quantizer/mixed_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/quantizer/mixed_precision/quantization_config_factory.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/quantizer/mixed_precision/quantization_config_factory.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/quantizer/mixed_precision/selective_activation_quantizer.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/quantizer/mixed_precision/selective_activation_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/quantizer/mixed_precision/selective_quantize_config.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/quantizer/mixed_precision/selective_quantize_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/quantizer/mixed_precision/selective_weights_quantizer.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/quantizer/mixed_precision/selective_weights_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/reader/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/reader/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/reader/common.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/reader/common.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/reader/connectivity_handler.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/reader/connectivity_handler.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/reader/nested_model/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/reader/nested_model/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/reader/nested_model/edges_merger.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/reader/nested_model/edges_merger.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/reader/nested_model/nested_model_handler.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/reader/nested_model/nested_model_handler.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/reader/nested_model/nodes_merger.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/reader/nested_model/nodes_merger.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/reader/nested_model/outputs_merger.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/reader/nested_model/outputs_merger.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/reader/node_builder.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/reader/node_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/reader/reader.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/reader/reader.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/statistics_correction/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/statistics_correction/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/statistics_correction/apply_second_moment_correction.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/statistics_correction/apply_second_moment_correction.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/tf_tensor_numpy.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/tf_tensor_numpy.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/keras/visualization/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/keras/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/back2framework/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/back2framework/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/back2framework/factory_model_builder.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/back2framework/factory_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/back2framework/float_model_builder.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/back2framework/float_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/back2framework/instance_builder.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/back2framework/instance_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/back2framework/mixed_precision_model_builder.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/back2framework/mixed_precision_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/back2framework/model_gradients.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/back2framework/model_gradients.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,16 +22,17 @@
 
 from model_compression_toolkit.core import common
 from model_compression_toolkit.core.common import BaseNode, Graph
 from model_compression_toolkit.core.common.constants import EPS, MIN_JACOBIANS_ITER, JACOBIANS_COMP_TOLERANCE
 from model_compression_toolkit.core.common.graph.edge import EDGE_SINK_INDEX
 from model_compression_toolkit.core.common.graph.functional_node import FunctionalNode
 from model_compression_toolkit.core.pytorch.back2framework.instance_builder import node_builder
-from model_compression_toolkit.core.pytorch.reader.node_holders import DummyPlaceHolder
-from model_compression_toolkit.core.pytorch.utils import torch_tensor_to_numpy
+from model_compression_toolkit.core.pytorch.constants import BUFFER
+from model_compression_toolkit.core.pytorch.reader.node_holders import DummyPlaceHolder, BufferHolder
+from model_compression_toolkit.core.pytorch.utils import torch_tensor_to_numpy, get_working_device
 from model_compression_toolkit.core.common.logger import Logger
 
 
 def build_input_tensors_list(node: BaseNode,
                              graph: Graph,
                              inputs: Dict[BaseNode, List],
                              node_to_output_tensors_dict: Dict[BaseNode, List]) -> List[List]:
@@ -129,15 +130,21 @@
         self.node_sort = list(topological_sort(graph_float))
         self.interest_points = interest_points
         self.output_list = output_list
         self.interest_points_tensors = []
 
         for n in self.node_sort:
             if not isinstance(n, FunctionalNode):
-                self.add_module(n.name, node_builder(n))
+                if n.type == BufferHolder:
+                    self.add_module(n.name, node_builder(n))
+                    self.get_submodule(n.name). \
+                        register_buffer(n.name,
+                                        torch.Tensor(n.get_weights_by_keys(BUFFER)).to(get_working_device()))
+                else:
+                    self.add_module(n.name, node_builder(n))
 
     def forward(self,
                 *args: Any) -> Any:
         """
         Args:
             args: argument input tensors to model, which is a mappings between an input node and its input tensor.
 
@@ -285,17 +292,17 @@
                                              device=device))
                 break
             jac_v = torch.reshape(jac_v, [jac_v.shape[0], -1])
             jac_trace_approx = torch.mean(torch.sum(torch.pow(jac_v, 2.0)))
 
             # If the change to the mean Jacobian approximation is insignificant we stop the calculation
             if j > MIN_JACOBIANS_ITER:
-                delta = torch.mean(torch.stack([jac_trace_approx, *trace_jv])) - torch.mean(
-                    torch.stack(trace_jv))
-                if torch.abs(delta) / (torch.abs(torch.mean(torch.stack(trace_jv))) + 1e-6) < JACOBIANS_COMP_TOLERANCE:
+                new_mean = torch.mean(torch.stack([jac_trace_approx, *trace_jv]))
+                delta = new_mean - torch.mean(torch.stack(trace_jv))
+                if torch.abs(delta) / (torch.abs(new_mean) + 1e-6) < JACOBIANS_COMP_TOLERANCE:
                     trace_jv.append(jac_trace_approx)
                     break
 
             trace_jv.append(jac_trace_approx)
         ipts_jac_trace_approx.append(2*torch.mean(torch.stack(trace_jv))/output.shape[-1])  # Get averaged jacobian trace approximation
 
     ipts_jac_trace_approx = torch_tensor_to_numpy(torch.Tensor(ipts_jac_trace_approx))  # Just to get one tensor instead of list of tensors with single element
```

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/back2framework/pytorch_model_builder.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/back2framework/pytorch_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/quantized_layer_wrapper.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/quantized_layer_wrapper.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/wrapper_quantize_config.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/wrapper_quantize_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/back2framework/quantized_model_builder.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/back2framework/quantized_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/constants.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/constants.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/default_framework_info.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/default_framework_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/graph_substitutions/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/graph_substitutions/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_folding.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_folding.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_reconstruction.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_reconstruction.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_refusing.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_refusing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/const_holder_conv.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/const_holder_conv.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/linear_collapsing.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/linear_collapsing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/multi_head_attention_decomposition.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/multi_head_attention_decomposition.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/permute_call_method.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/permute_call_method.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/relu_bound_to_power_of_2.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/relu_bound_to_power_of_2.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/reshape_with_static_shapes.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/reshape_with_static_shapes.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/residual_collapsing.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/residual_collapsing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/scale_equalization.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/scale_equalization.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/shift_negative_activation.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/shift_negative_activation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/softmax_shift.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/softmax_shift.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/virtual_activation_weights_composition.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/virtual_activation_weights_composition.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/weights_activation_split.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/weights_activation_split.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/kpi_data_facade.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/kpi_data_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/mixed_precision/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/mixed_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/mixed_precision/mixed_precision_wrapper.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/mixed_precision/mixed_precision_wrapper.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/mixed_precision/set_layer_to_bitwidth.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/mixed_precision/set_layer_to_bitwidth.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/pytorch_implementation.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/pytorch_implementation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/pytorch_node_prior_info.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/pytorch_node_prior_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/quantization_facade.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/quantization_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/quantizer/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/quantizer/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/quantizer/fake_quant_builder.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/quantizer/fake_quant_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/quantizer/lut_fake_quant.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/quantizer/lut_fake_quant.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/reader/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/reader/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/reader/graph_builders.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/reader/graph_builders.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/reader/node_holders.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/reader/node_holders.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/reader/reader.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/reader/reader.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/statistics_correction/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/statistics_correction/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/statistics_correction/apply_second_moment_correction.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/statistics_correction/apply_second_moment_correction.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/pytorch/utils.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/pytorch/utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/runner.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/runner.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/default_tpc/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/default_tpc/latest/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/latest/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/default_tpc/target_platform_capabilities.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/target_platform_capabilities.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/default_tpc/v1/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/default_tpc/v1/tp_model.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v1/tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/default_tpc/v1/tpc_keras.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v1/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/default_tpc/v1/tpc_pytorch.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v1/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/default_tpc/v2/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/default_tpc/v2/tp_model.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v2/tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/default_tpc/v2/tpc_keras.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v2/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/default_tpc/v2/tpc_pytorch.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v2/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/default_tpc/v3/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v3/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/default_tpc/v3/tp_model.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v3/tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/default_tpc/v3/tpc_keras.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v3/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/default_tpc/v3/tpc_pytorch.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v3/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/default_tpc/v3_lut/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v3_lut/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/default_tpc/v3_lut/tp_model.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v3_lut/tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/default_tpc/v3_lut/tpc_keras.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v3_lut/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/default_tpc/v3_lut/tpc_pytorch.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v3_lut/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/default_tpc/v4/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v4/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/default_tpc/v4/tp_model.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v4/tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/default_tpc/v4/tpc_keras.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v4/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/default_tpc/v4/tpc_pytorch.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v4/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/default_tpc/v4_lut/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v4_lut/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/default_tpc/v4_lut/tp_model.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v4_lut/tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/default_tpc/v4_lut/tpc_keras.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v4_lut/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/default_tpc/v4_lut/tpc_pytorch.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v4_lut/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/default_tpc/v5/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v5/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/default_tpc/v5/tp_model.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v5/tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/default_tpc/v5/tpc_keras.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v5/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/default_tpc/v5/tpc_pytorch.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/default_tpc/v5/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/get_target_platform_capabilities.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/get_target_platform_capabilities.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/imx500_tpc/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/imx500_tpc/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/imx500_tpc/latest/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/imx500_tpc/latest/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/imx500_tpc/target_platform_capabilities.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/imx500_tpc/target_platform_capabilities.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/imx500_tpc/v1/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/imx500_tpc/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/imx500_tpc/v1/tp_model.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/imx500_tpc/v1/tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/imx500_tpc/v1/tpc_keras.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/imx500_tpc/v1/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/imx500_tpc/v1/tpc_pytorch.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/imx500_tpc/v1/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/qnnpack_tpc/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/qnnpack_tpc/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/qnnpack_tpc/latest/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/qnnpack_tpc/latest/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/qnnpack_tpc/target_platform_capabilities.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/qnnpack_tpc/target_platform_capabilities.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/qnnpack_tpc/v1/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/qnnpack_tpc/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/qnnpack_tpc/v1/tp_model.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/qnnpack_tpc/v1/tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/qnnpack_tpc/v1/tpc_keras.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/qnnpack_tpc/v1/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/qnnpack_tpc/v1/tpc_pytorch.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/qnnpack_tpc/v1/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/tflite_tpc/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/tflite_tpc/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/tflite_tpc/latest/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/tflite_tpc/latest/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/tflite_tpc/target_platform_capabilities.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/tflite_tpc/target_platform_capabilities.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/tflite_tpc/v1/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/tflite_tpc/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/tflite_tpc/v1/tp_model.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/tflite_tpc/v1/tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/tflite_tpc/v1/tpc_keras.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/tflite_tpc/v1/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/core/tpc_models/tflite_tpc/v1/tpc_pytorch.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/core/tpc_models/tflite_tpc/v1/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/exporter/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_exporter/fw_agonstic/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/exporter/model_exporter/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,7 +12,8 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
 from model_compression_toolkit.exporter.model_exporter.keras.keras_export_facade import keras_export_model, KerasExportMode
 from model_compression_toolkit.exporter.model_exporter.pytorch.pytorch_export_facade import PyTorchExportMode, pytorch_export_model
 from model_compression_toolkit.exporter.model_exporter.tflite.tflite_export_facade import tflite_export_model, TFLiteExportMode
+
```

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/exporter/model_exporter/fw_agonstic/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_exporter/tflite/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/exporter/model_exporter/fw_agonstic/exporter.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_exporter/fw_agonstic/exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/exporter/model_exporter/keras/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_exporter/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/exporter/model_exporter/keras/base_keras_exporter.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_exporter/keras/base_keras_exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_keras_exporter.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_keras_exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/exporter/model_exporter/keras/keras_export_facade.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_exporter/keras/keras_export_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/exporter/model_exporter/pytorch/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_exporter/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/exporter/model_exporter/pytorch/base_pytorch_exporter.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_exporter/pytorch/base_pytorch_exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_onnx_pytorch_exporter.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_onnx_pytorch_exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_torchscript_pytorch_exporter.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_torchscript_pytorch_exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/exporter/model_exporter/pytorch/pytorch_export_facade.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_exporter/pytorch/pytorch_export_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/exporter/model_exporter/tflite/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_wrapper/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/exporter/model_exporter/tflite/fakely_quant_tflite_exporter.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_exporter/tflite/fakely_quant_tflite_exporter.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 import os
 import tempfile
 from typing import Callable
 
 import keras.models
 import tensorflow as tf
 
-from model_compression_toolkit import keras_load_quantized_model
+from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.keras.load_model import keras_load_quantized_model
 from model_compression_toolkit.core.common import Logger
 from model_compression_toolkit.exporter.model_exporter.keras.fakely_quant_keras_exporter import FakelyQuantKerasExporter
 
 
 class FakelyQuantTFLiteExporter(FakelyQuantKerasExporter):
     """
     Exporter for fakely-quant TFLite models.
```

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/exporter/model_exporter/tflite/int8_tflite_exporter.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_exporter/tflite/int8_tflite_exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/exporter/model_exporter/tflite/tflite_export_facade.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_exporter/tflite/tflite_export_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/exporter/model_wrapper/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_wrapper/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,16 +9,12 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
-from model_compression_toolkit.core.common.constants import FOUND_TF, FOUND_TORCH
+from model_compression_toolkit.exporter.model_wrapper.keras.validate_layer import is_keras_layer_exportable
+from model_compression_toolkit.exporter.model_wrapper.keras.builder.fully_quantized_model_builder import get_exportable_keras_model
 
-if FOUND_TF:
-    from model_compression_toolkit.exporter.model_wrapper.keras.validate_layer import is_keras_layer_exportable
-    from model_compression_toolkit.exporter.model_wrapper.keras.builder.fully_quantized_model_builder import get_exportable_keras_model
-
-if FOUND_TORCH:
-    from model_compression_toolkit.exporter.model_wrapper.pytorch.validate_layer import is_pytorch_layer_exportable
-    from model_compression_toolkit.exporter.model_wrapper.pytorch.builder.fully_quantized_model_builder import get_exportable_pytorch_model
+from model_compression_toolkit.exporter.model_wrapper.pytorch.validate_layer import is_pytorch_layer_exportable
+from model_compression_toolkit.exporter.model_wrapper.pytorch.builder.fully_quantized_model_builder import get_exportable_pytorch_model
```

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/exporter/model_wrapper/keras/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_wrapper/keras/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/exporter/model_wrapper/keras/builder/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/exporter/model_wrapper/keras/builder/fully_quantized_model_builder.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_wrapper/keras/builder/fully_quantized_model_builder.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,50 +10,56 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from typing import Tuple
 
-import tensorflow as tf
-from tensorflow.keras.layers import Layer
 
 from model_compression_toolkit import quantizers_infrastructure as qi
 from model_compression_toolkit.core import common
-from model_compression_toolkit.core.common import Graph
+from model_compression_toolkit.core.common import Graph, Logger
+from model_compression_toolkit.core.common.constants import FOUND_TF
 from model_compression_toolkit.core.common.user_info import UserInformation
-from model_compression_toolkit.core.keras.back2framework.keras_model_builder import KerasModelBuilder
-from model_compression_toolkit.exporter.model_wrapper.keras.builder.node_to_quantizers import \
-    get_quantization_quantizers
-
-
-def _get_wrapper(node: common.BaseNode,
-                 layer: Layer) -> qi.KerasQuantizationWrapper:
-    """
-    A function which takes a computational graph node and a keras layer and perform the quantization wrapping
-    Args:
-        n: A node of mct graph.
-        layer: A keras layer
-
-    Returns: Wrapped layer with weights quantizers and activation quantizers
-
-    """
-    weights_quantizers, activation_quantizers = get_quantization_quantizers(node)
-    return qi.KerasQuantizationWrapper(layer, weights_quantizers, activation_quantizers)
-
-
-def get_exportable_keras_model(graph: Graph) -> Tuple[tf.keras.models.Model,UserInformation]:
-    """
-    Convert graph to an exportable Keras model (model with all quantization parameters).
-    An exportable model can then be exported using model_exporter, to retrieve the
-    final exported model.
-
-    Args:
-        graph: Graph to convert to an exportable Keras model.
-
-    Returns:
-        Exportable Keras model and user information.
-    """
-    exportable_model, user_info = KerasModelBuilder(graph=graph,
-                                         wrapper=_get_wrapper).build_model()
-    exportable_model.trainable = False
-    return exportable_model, user_info
+
+if FOUND_TF:
+    import tensorflow as tf
+    from tensorflow.keras.layers import Layer
+    from model_compression_toolkit.core.keras.back2framework.keras_model_builder import KerasModelBuilder
+    from model_compression_toolkit.exporter.model_wrapper.keras.builder.node_to_quantizers import get_quantization_quantizers
+
+    def _get_wrapper(node: common.BaseNode,
+                     layer: Layer) -> qi.KerasQuantizationWrapper:
+        """
+        A function which takes a computational graph node and a keras layer and perform the quantization wrapping
+        Args:
+            n: A node of mct graph.
+            layer: A keras layer
+
+        Returns: Wrapped layer with weights quantizers and activation quantizers
+
+        """
+        weights_quantizers, activation_quantizers = get_quantization_quantizers(node)
+        return qi.KerasQuantizationWrapper(layer, weights_quantizers, activation_quantizers)
+
+
+    def get_exportable_keras_model(graph: Graph) -> Tuple[tf.keras.models.Model, UserInformation]:
+        """
+        Convert graph to an exportable Keras model (model with all quantization parameters).
+        An exportable model can then be exported using model_exporter, to retrieve the
+        final exported model.
+
+        Args:
+            graph: Graph to convert to an exportable Keras model.
+
+        Returns:
+            Exportable Keras model and user information.
+        """
+        exportable_model, user_info = KerasModelBuilder(graph=graph,
+                                             wrapper=_get_wrapper).build_model()
+        exportable_model.trainable = False
+        return exportable_model, user_info
+else:
+    def get_exportable_keras_model(*args, **kwargs):  # pragma: no cover
+        Logger.error('Installing tensorflow and tensorflow_model_optimization is mandatory '
+                     'when using get_exportable_keras_model. '
+                     'Could not find Tensorflow package.')
```

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/exporter/model_wrapper/keras/builder/node_to_quantizer.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_wrapper/keras/builder/node_to_quantizer.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,23 +11,20 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from typing import Dict, Any
 
 from model_compression_toolkit.core.common import BaseNode, Logger
-from model_compression_toolkit.core.common.constants import THRESHOLD, RANGE_MIN, RANGE_MAX, SIGNED
+from model_compression_toolkit.core.common.constants import THRESHOLD, RANGE_MIN, RANGE_MAX, SIGNED, CLUSTER_CENTERS, SCALE_PER_CHANNEL
 from model_compression_toolkit.core.common.target_platform import QuantizationMethod
 from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.common.base_inferable_quantizer import QuantizationTarget
-from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.common.get_quantizers import \
-    get_inferable_quantizer_class
-from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.keras.quantizers.base_keras_inferable_quantizer \
-    import \
-    BaseKerasInferableQuantizer
-
+from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.common.get_quantizers import get_inferable_quantizer_class
+from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.keras.quantizers.base_keras_inferable_quantizer import BaseKerasInferableQuantizer
+from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.keras.quantizers import constants as qi_keras_consts
 
 def get_inferable_quantizer_kwargs(node: BaseNode,
                                    quantization_target: QuantizationTarget) -> Dict[str, Any]:
     """
     Get the quantization parameters for an inferable quantizer.
     Args:
         node: The node for which the quantizer is being created.
@@ -40,48 +37,66 @@
         # Get the weights quantization configuration for the node
         node_w_qc = node.final_weights_quantization_cfg
         quantization_method = node_w_qc.weights_quantization_method
 
         # Return the appropriate quantization parameters based on the quantization method
         if quantization_method in [QuantizationMethod.POWER_OF_TWO,
                                    QuantizationMethod.SYMMETRIC]:
-            return {'num_bits': node_w_qc.weights_n_bits,
-                    'threshold': list(node_w_qc.weights_quantization_params[THRESHOLD].flatten()),
-                    'per_channel': node_w_qc.weights_per_channel_threshold,
-                    'channel_axis': node_w_qc.weights_channels_axis,
-                    'input_rank': len(node_w_qc.weights_quantization_params[THRESHOLD].shape)}
+            return {qi_keras_consts.NUM_BITS: node_w_qc.weights_n_bits,
+                    qi_keras_consts.THRESHOLD: list(node_w_qc.weights_quantization_params[THRESHOLD].flatten()),
+                    qi_keras_consts.PER_CHANNEL: node_w_qc.weights_per_channel_threshold,
+                    qi_keras_consts.CHANNEL_AXIS: node_w_qc.weights_channels_axis,
+                    qi_keras_consts.INPUT_RANK: len(node_w_qc.weights_quantization_params[THRESHOLD].shape)}
 
         elif quantization_method in [QuantizationMethod.UNIFORM]:
-            return {'num_bits': node_w_qc.weights_n_bits,
-                    'per_channel': node_w_qc.weights_per_channel_threshold,
-                    'min_range': list(node_w_qc.weights_quantization_params[RANGE_MIN].flatten()),
-                    'max_range': list(node_w_qc.weights_quantization_params[RANGE_MAX].flatten()),
-                    'channel_axis': node_w_qc.weights_channels_axis,
-                    'input_rank': len(node_w_qc.weights_quantization_params[RANGE_MIN].shape)}
+            return {qi_keras_consts.NUM_BITS: node_w_qc.weights_n_bits,
+                    qi_keras_consts.PER_CHANNEL: node_w_qc.weights_per_channel_threshold,
+                    qi_keras_consts.MIN_RANGE: list(node_w_qc.weights_quantization_params[RANGE_MIN].flatten()),
+                    qi_keras_consts.MAX_RANGE: list(node_w_qc.weights_quantization_params[RANGE_MAX].flatten()),
+                    qi_keras_consts.CHANNEL_AXIS: node_w_qc.weights_channels_axis,
+                    qi_keras_consts.INPUT_RANK: len(node_w_qc.weights_quantization_params[RANGE_MIN].shape)}
+
+        elif quantization_method in [QuantizationMethod.LUT_SYM_QUANTIZER, QuantizationMethod.LUT_POT_QUANTIZER]:
+            return {qi_keras_consts.NUM_BITS: node_w_qc.weights_n_bits,
+                    qi_keras_consts.PER_CHANNEL: node_w_qc.weights_per_channel_threshold,
+                    qi_keras_consts.CLUSTER_CENTERS: node_w_qc.weights_quantization_params[CLUSTER_CENTERS],
+                    qi_keras_consts.THRESHOLD: list(node_w_qc.weights_quantization_params[SCALE_PER_CHANNEL].flatten()),
+                    qi_keras_consts.CHANNEL_AXIS: node_w_qc.weights_channels_axis,
+                    # TODO: how to pass multiplier nbits and eps for a specific node?
+                    qi_keras_consts.INPUT_RANK: len(node_w_qc.weights_quantization_params[SCALE_PER_CHANNEL].shape)}
+
         else:
             Logger.critical(f'Not supported quantization method for inferable quantizers.')  # pragma: no cover
 
     elif quantization_target == QuantizationTarget.Activation:
         # Get the activation quantization configuration for the node
         node_qc = node.final_activation_quantization_cfg
         quantization_method = node_qc.activation_quantization_method
 
         # Return the appropriate quantization parameters based on the quantization method
         if quantization_method in [QuantizationMethod.POWER_OF_TWO,
                                    QuantizationMethod.SYMMETRIC]:
-            return {'num_bits': node_qc.activation_n_bits,
+            return {qi_keras_consts.NUM_BITS: node_qc.activation_n_bits,
                     # In activation quantization is per-tensor only - thus we hold the threshold as a list with a len of 1
-                    'threshold': [node_qc.activation_quantization_params[THRESHOLD]],
-                    'signed': node_qc.activation_quantization_params[SIGNED]}
+                    qi_keras_consts.THRESHOLD: [node_qc.activation_quantization_params[THRESHOLD]],
+                    qi_keras_consts.SIGNED: node_qc.activation_quantization_params[SIGNED]}
 
         elif quantization_method in [QuantizationMethod.UNIFORM]:
-            return {'num_bits': node_qc.activation_n_bits,
+            return {qi_keras_consts.NUM_BITS: node_qc.activation_n_bits,
                     # In activation quantization is per-tensor only - thus we hold the min/max as a list with a len of 1
-                    'min_range': [node_qc.activation_quantization_params[RANGE_MIN]],
-                    'max_range': [node_qc.activation_quantization_params[RANGE_MAX]]}
+                    qi_keras_consts.MIN_RANGE: [node_qc.activation_quantization_params[RANGE_MIN]],
+                    qi_keras_consts.MAX_RANGE: [node_qc.activation_quantization_params[RANGE_MAX]]}
+
+        elif quantization_method in [QuantizationMethod.LUT_POT_QUANTIZER]:
+            return {qi_keras_consts.NUM_BITS: node_qc.activation_n_bits,
+                    qi_keras_consts.SIGNED: node_qc.activation_quantization_params[SIGNED],
+                    qi_keras_consts.CLUSTER_CENTERS: node_qc.activation_quantization_params[CLUSTER_CENTERS],
+                    qi_keras_consts.THRESHOLD: [node_qc.activation_quantization_params[THRESHOLD]]
+                    # TODO: how to pass multiplier nbits and eps for a specific node?
+                    }
         else:
             Logger.critical(f'Not supported quantization method for inferable quantizers.')  # pragma: no cover
     else:
         Logger.critical(f'{quantization_target} is not supported')  # pragma: no cover
 
 
 def get_weights_quantizer_for_node(node: BaseNode) -> BaseKerasInferableQuantizer:
```

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/exporter/model_wrapper/keras/builder/node_to_quantizers.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_wrapper/keras/builder/node_to_quantizers.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/exporter/model_wrapper/keras/validate_layer.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_wrapper/keras/validate_layer.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,65 +10,73 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from typing import Any
 
-from keras.engine.input_layer import InputLayer
 
 from model_compression_toolkit.core.common import Logger
-from model_compression_toolkit.quantizers_infrastructure import KerasQuantizationWrapper
+from model_compression_toolkit.core.common.constants import FOUND_TF
+
 from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.common.base_inferable_quantizer import BaseInferableQuantizer
 
 
+if FOUND_TF:
+    from keras.engine.input_layer import InputLayer
+    from model_compression_toolkit.quantizers_infrastructure import KerasQuantizationWrapper
 
-def is_keras_layer_exportable(layer: Any) -> bool:
-    """
-    Check whether a Keras layer is a valid exportable layer or not.
+    def is_keras_layer_exportable(layer: Any) -> bool:
+        """
+        Check whether a Keras layer is a valid exportable layer or not.
 
-    Args:
-        layer: Keras layer to check if considered to be valid for exporting.
+        Args:
+            layer: Keras layer to check if considered to be valid for exporting.
 
-    Returns:
-        Check whether a Keras layer is a valid exportable layer or not.
-    """
-    # Keras Input layers are not wrapped
-    if isinstance(layer, InputLayer):
-        return True
+        Returns:
+            Check whether a Keras layer is a valid exportable layer or not.
+        """
+        # Keras Input layers are not wrapped
+        if isinstance(layer, InputLayer):
+            return True
 
-    valid_layer = isinstance(layer, KerasQuantizationWrapper)
-    if not valid_layer:
-        Logger.error(
-            f'Exportable layer must be wrapped using KerasQuantizationWrapper, but layer {layer.name} is of type '
-            f'{type(layer)}') # pragma: no cover
-
-    valid_weights_quantizers = isinstance(layer.weights_quantizers, dict)
-    if not valid_weights_quantizers:
-        Logger.error(
-            f'KerasQuantizationWrapper must have a weights_quantizers but has a '
-            f'{type(layer.weights_quantizers)} object') # pragma: no cover
+        valid_layer = isinstance(layer, KerasQuantizationWrapper)
+        if not valid_layer:
+            Logger.error(
+                f'Exportable layer must be wrapped using KerasQuantizationWrapper, but layer {layer.name} is of type '
+                f'{type(layer)}') # pragma: no cover
 
-    for _, weights_quantizer in layer.weights_quantizers.items():
-        if not isinstance(weights_quantizer, BaseInferableQuantizer):
+        valid_weights_quantizers = isinstance(layer.weights_quantizers, dict)
+        if not valid_weights_quantizers:
             Logger.error(
-                f'weights_quantizer must be a BaseInferableQuantizer object but has a '
-                f'{type(weights_quantizer)} object')  # pragma: no cover
+                f'KerasQuantizationWrapper must have a weights_quantizers but has a '
+                f'{type(layer.weights_quantizers)} object') # pragma: no cover
 
-    valid_activation_quantizers = isinstance(layer.activation_quantizers, list)
-    if not valid_activation_quantizers:
-        Logger.error(
-            f'KerasQuantizationWrapper must have a activation_quantizers list but has a '
-            f'{type(layer.activation_quantizers)} object') # pragma: no cover
+        for _, weights_quantizer in layer.weights_quantizers.items():
+            if not isinstance(weights_quantizer, BaseInferableQuantizer):
+                Logger.error(
+                    f'weights_quantizer must be a BaseInferableQuantizer object but has a '
+                    f'{type(weights_quantizer)} object')  # pragma: no cover
 
-    for activation_quantizers in layer.activation_quantizers:
-        if not isinstance(activation_quantizers, BaseInferableQuantizer):
+        valid_activation_quantizers = isinstance(layer.activation_quantizers, list)
+        if not valid_activation_quantizers:
             Logger.error(
-                f'activation_quantizers must be a BaseInferableQuantizer object but has a '
-                f'{type(activation_quantizers)} object')  # pragma: no cover
+                f'KerasQuantizationWrapper must have a activation_quantizers list but has a '
+                f'{type(layer.activation_quantizers)} object') # pragma: no cover
 
-    quantizers = layer.activation_quantizers + list(layer.weights_quantizers.values())
-    is_valid_quantizers = all([isinstance(x, BaseInferableQuantizer) for x in quantizers])
-    if not is_valid_quantizers:
-        Logger.error(f'Found a quantizer that is not of type BaseInferableQuantizer') # pragma: no cover
+        for activation_quantizers in layer.activation_quantizers:
+            if not isinstance(activation_quantizers, BaseInferableQuantizer):
+                Logger.error(
+                    f'activation_quantizers must be a BaseInferableQuantizer object but has a '
+                    f'{type(activation_quantizers)} object')  # pragma: no cover
+
+        quantizers = layer.activation_quantizers + list(layer.weights_quantizers.values())
+        is_valid_quantizers = all([isinstance(x, BaseInferableQuantizer) for x in quantizers])
+        if not is_valid_quantizers:
+            Logger.error(f'Found a quantizer that is not of type BaseInferableQuantizer') # pragma: no cover
 
-    return True
+        return True
+else:
+    def is_keras_layer_exportable(*args, **kwargs):  # pragma: no cover
+        Logger.error('Installing tensorflow and tensorflow_model_optimization is mandatory '
+                     'when using is_keras_layer_exportable. '
+                     'Could not find Tensorflow package.')
```

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/exporter/model_wrapper/pytorch/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_wrapper/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/common/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/node_to_quantizer.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/node_to_quantizer.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
 from typing import Dict, Any
 
 from model_compression_toolkit.core.common import BaseNode, Logger
-from model_compression_toolkit.core.common.constants import THRESHOLD, SIGNED, RANGE_MIN, RANGE_MAX
+from model_compression_toolkit.core.common.constants import THRESHOLD, SIGNED, RANGE_MIN, RANGE_MAX, \
+    SCALE_PER_CHANNEL, CLUSTER_CENTERS
 from model_compression_toolkit.core.common.target_platform import QuantizationMethod
 from model_compression_toolkit.quantizers_infrastructure import QuantizationTarget
 from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.common.get_quantizers import \
     get_inferable_quantizer_class
 from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.pytorch.quantizers import \
     constants as qi_inferable_quantizers_constants, BasePyTorchInferableQuantizer
 import numpy as np
@@ -41,14 +42,23 @@
 
     elif quantization_method in [QuantizationMethod.UNIFORM]:
         return {qi_inferable_quantizers_constants.NUM_BITS: node_w_qc.weights_n_bits,
                 qi_inferable_quantizers_constants.PER_CHANNEL: node_w_qc.weights_per_channel_threshold,
                 qi_inferable_quantizers_constants.MIN_RANGE: node_w_qc.weights_quantization_params[RANGE_MIN].flatten(),
                 qi_inferable_quantizers_constants.MAX_RANGE: node_w_qc.weights_quantization_params[RANGE_MAX].flatten(),
                 qi_inferable_quantizers_constants.CHANNEL_AXIS: node_w_qc.weights_channels_axis}
+
+    elif quantization_method in [QuantizationMethod.LUT_POT_QUANTIZER, QuantizationMethod.LUT_SYM_QUANTIZER]:
+        return {qi_inferable_quantizers_constants.NUM_BITS: node_w_qc.weights_n_bits,
+                qi_inferable_quantizers_constants.CLUSTER_CENTERS: node_w_qc.weights_quantization_params[CLUSTER_CENTERS].flatten(),
+                qi_inferable_quantizers_constants.THRESHOLD: node_w_qc.weights_quantization_params[SCALE_PER_CHANNEL].flatten(),
+                qi_inferable_quantizers_constants.PER_CHANNEL: node_w_qc.weights_per_channel_threshold,
+                qi_inferable_quantizers_constants.CHANNEL_AXIS: node_w_qc.weights_channels_axis}
+                # TODO: Add MULTIPLIER_N_BITS & EPS to node quantization config
+
     else:
         Logger.critical(f'Not supported quantization method for weights inferable quantizers.')  # pragma: no cover
 
 
 def get_activation_inferable_quantizer_kwargs(node: BaseNode) -> Dict[str, Any]:
     # Get the activation quantization configuration for the node
     node_qc = node.final_activation_quantization_cfg
@@ -61,14 +71,23 @@
                 qi_inferable_quantizers_constants.THRESHOLD: np.asarray([node_qc.activation_quantization_params[THRESHOLD]]),
                 qi_inferable_quantizers_constants.SIGNED: node_qc.activation_quantization_params.get(SIGNED)}
 
     elif quantization_method in [QuantizationMethod.UNIFORM]:
         return {qi_inferable_quantizers_constants.NUM_BITS: node_qc.activation_n_bits,
                 qi_inferable_quantizers_constants.MIN_RANGE: np.asarray([node_qc.activation_quantization_params[RANGE_MIN]]),
                 qi_inferable_quantizers_constants.MAX_RANGE: np.asarray([node_qc.activation_quantization_params[RANGE_MAX]])}
+
+    elif quantization_method in [QuantizationMethod.LUT_POT_QUANTIZER]:
+        return {qi_inferable_quantizers_constants.NUM_BITS: node_qc.activation_n_bits,
+                qi_inferable_quantizers_constants.CLUSTER_CENTERS: np.asarray(
+                    [node_qc.activation_quantization_params[CLUSTER_CENTERS]]),
+                qi_inferable_quantizers_constants.THRESHOLD: np.asarray(
+                    [node_qc.activation_quantization_params[THRESHOLD]]),
+                qi_inferable_quantizers_constants.SIGNED: node_qc.activation_quantization_params.get(SIGNED)}
+        # TODO: Add MULTIPLIER_N_BITS & EPS to node quantization config
     else:
         Logger.critical(f'Not supported quantization method for inferable quantizers.')  # pragma: no cover
 
 
 def get_weights_quantizer_for_node(node: BaseNode) -> BasePyTorchInferableQuantizer:
     """
     Get weights quantizer for a node.
@@ -107,14 +126,14 @@
     """
     if node.final_activation_quantization_cfg is None:
         Logger.critical(f'Can not set quantizer for a node with no final activation quantization configuration')  #
         # pragma: no cover
     node_act_qc = node.final_activation_quantization_cfg
     activation_quantization_method = node_act_qc.activation_quantization_method
 
-    quantier_for_node = get_inferable_quantizer_class(QuantizationTarget.Activation,
-                                                      activation_quantization_method,
-                                                      BasePyTorchInferableQuantizer)
+    quantizer_for_node = get_inferable_quantizer_class(QuantizationTarget.Activation,
+                                                       activation_quantization_method,
+                                                       BasePyTorchInferableQuantizer)
     kwargs = get_activation_inferable_quantizer_kwargs(node)
 
-    return quantier_for_node(**kwargs)
+    return quantizer_for_node(**kwargs)
```

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/node_to_quantizers.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/node_to_quantizers.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/exporter/model_wrapper/pytorch/validate_layer.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_wrapper/pytorch/validate_layer.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,28 +10,35 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from typing import Any
 
-from model_compression_toolkit.quantizers_infrastructure import PytorchQuantizationWrapper
-from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.pytorch.quantizers import \
-    BasePyTorchInferableQuantizer
+from model_compression_toolkit.core.common import Logger
+from model_compression_toolkit.core.common.constants import FOUND_TORCH
 
+if FOUND_TORCH:
+    from model_compression_toolkit.quantizers_infrastructure import PytorchQuantizationWrapper
+    from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.pytorch.quantizers import \
+        BasePyTorchInferableQuantizer
+    def is_pytorch_layer_exportable(layer: Any) -> bool:
+        """
+        Check whether a torch Module is a valid exportable module or not.
 
-def is_pytorch_layer_exportable(layer: Any) -> bool:
-    """
-    Check whether a torch Module is a valid exportable module or not.
+        Args:
+            layer: PyTorch module to check if considered to be valid for exporting.
 
-    Args:
-        layer: PyTorch module to check if considered to be valid for exporting.
-
-    Returns:
-        Check whether a PyTorch layer is a valid exportable layer or not.
-    """
-    if isinstance(layer, PytorchQuantizationWrapper):
-        quantizers = list(layer.weights_quantizers.values())
-        quantizers.extend(layer.activation_quantizers)
-        if all([isinstance(q, BasePyTorchInferableQuantizer) for q in quantizers]):
-            return True
-    return False
+        Returns:
+            Check whether a PyTorch layer is a valid exportable layer or not.
+        """
+        if isinstance(layer, PytorchQuantizationWrapper):
+            quantizers = list(layer.weights_quantizers.values())
+            quantizers.extend(layer.activation_quantizers)
+            if all([isinstance(q, BasePyTorchInferableQuantizer) for q in quantizers]):
+                return True
+        return False
+else:
+    def is_pytorch_layer_exportable(*args, **kwargs):  # pragma: no cover
+        Logger.error('Installing torch is mandatory '
+                     'when using is_pytorch_layer_exportable. '
+                     'Could not find PyTorch package.')
```

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/gptq/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/gptq/common/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/gptq/common/gptq_config.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/common/gptq_config.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,193 +12,165 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from enum import Enum
 from typing import Callable, Any, Dict
 from model_compression_toolkit.core.common.defaultdict import DefaultDict
 from model_compression_toolkit.core import common
-from model_compression_toolkit.gptq.common.gptq_constants import N_BATCHES_STR, QUANT_PARAM_LEARNING_STR, N_EPOCHS_STR, \
-    MAX_LSB_STR
-from model_compression_toolkit.gptq.common.gptq_quantizer_config import GPTQQuantizerConfig, SoftQuantizerConfig
+from model_compression_toolkit.gptq.common.gptq_constants import QUANT_PARAM_LEARNING_STR, MAX_LSB_STR, REG_DEFAULT
 
 
 class RoundingType(Enum):
     """
     An enum for choosing the GPTQ rounding methods
     0. STRAIGHT-THROUGH ESTIMATOR
     1. SoftQuantizer
     """
     STE = 0
     SoftQuantizer = 1
 
 
+class GPTQHessianWeightsConfig:
+    """
+    Configuration to use for computing the Hessian-based weights for GPTQ loss metric.
+    """
+
+    def __init__(self,
+                 hessians_num_samples: int = 16,
+                 norm_weights: bool = True,
+                 log_norm: bool = True,
+                 scale_log_norm: bool = False,
+                 hessians_n_iter: int = 50):
+
+        """
+        Initialize a GPTQHessianWeightsConfig.
+        Args:
+            hessians_num_samples (int): Number of samples to use for computing the Hessian-based weights.
+            norm_weights (bool): Whether to normalize the returned weights (to get values between 0 and 1).
+            log_norm (bool): Whether to use log normalization to the GPTQ Hessian-based weights.
+            scale_log_norm (bool): Whether to scale the final vector of the Hessian weights.
+            hessians_n_iter (int): Number of random iterations to run Hessian approximation for GPTQ weights.
+        """
+
+        self.hessians_num_samples = hessians_num_samples
+        self.norm_weights = norm_weights
+        self.log_norm = log_norm
+        self.scale_log_norm = scale_log_norm
+        self.hessians_n_iter = hessians_n_iter
+
+
 class GradientPTQConfig:
     """
     Configuration to use for quantization with GradientPTQ (experimental).
     """
 
-    def __init__(self,
-                 n_iter: int,
+    def __init__(self, n_iter: int,
                  optimizer: Any,
                  optimizer_rest: Any = None,
                  loss: Callable = None,
                  log_function: Callable = None,
                  train_bias: bool = True,
-                 quantization_parameters_learning: bool = False,
                  rounding_type: RoundingType = RoundingType.SoftQuantizer,
-                 lsb_change_per_bit_width: dict = DefaultDict({}, lambda: 1),
-                 eps: float = 1e-6,
-                 use_jac_based_weights: bool = True,
-                 num_samples_for_loss: int = 16,
-                 norm_weights: bool = False,
+                 use_hessian_based_weights: bool = True,
                  optimizer_quantization_parameter: Any = None,
                  optimizer_bias: Any = None,
-                 log_norm: bool = True,
-                 weights_n_iter: int = 50,
-                 quantizer_config: GPTQQuantizerConfig = SoftQuantizerConfig()):
+                 regularization_factor: float = REG_DEFAULT,
+                 hessian_weights_config: GPTQHessianWeightsConfig = GPTQHessianWeightsConfig(),
+                 gptq_quantizer_params_override: Dict[str, Any] = None):
         """
         Initialize a GradientPTQConfig.
 
         Args:
             n_iter (int): Number of iterations to train.
             optimizer (Any): Optimizer to use.
             optimizer_rest (Any): Optimizer to use for bias and quantizer parameters.
             loss (Callable): The loss to use. should accept 6 lists of tensors. 1st list of quantized tensors, the 2nd list is the float tensors,
              the 3rd is a list of quantized weights, the 4th is a list of float weights, the 5th and 6th lists are the mean and std of the tensors
              accordingly. see example in multiple_tensors_mse_loss
             log_function (Callable): Function to log information about the GPTQ process.
             train_bias (bool): Whether to update the bias during the training or not.
-            quantization_parameters_learning (bool): Whether to update the quantization param during the training or not.
             rounding_type (RoundingType): An enum that defines the rounding type.
-            lsb_change_per_bit_width (dict): Whether to update the bias during the training or not.
-            eps (float): A floating point value for numeric stability.
-            use_jac_based_weights (bool): Whether to use jacobian-based weights for weighted average loss.
-            num_samples_for_loss (int): Number of samples to use for computing the jacobian-based weights.
-            norm_weights (bool): Whether to normalize the returned weights (to get values between 0 and 1).
+            use_hessian_based_weights (bool): Whether to use Hessian-based weights for weighted average loss.
             optimizer_quantization_parameter (Any): Optimizer to override the rest optimizer  for quantizer parameters.
             optimizer_bias (Any): Optimizer to override the rest optimizer for bias.
-            log_norm (bool): Whether to use log normalization to the GPTQ Jacobian-based weights.
-            weights_n_iter (int): Number of random iterations to run Jacobian approximation for GPTQ weights.
-            quantizer_config (GPTQQuantizerConfig): A class that contains the quantizer specific config.
+            regularization_factor (float): A floating point number that defines the regularization factor.
+            hessian_weights_config (GPTQHessianWeightsConfig): A configuration that include all necessary arguments to run a computation of Hessian weights for the GPTQ loss.
+            gptq_quantizer_params_override (dict): A dictionary of parameters to override in GPTQ quantizer instantiation. Defaults to None (no parameters).
 
         """
         self.n_iter = n_iter
         self.optimizer = optimizer
         self.optimizer_rest = optimizer_rest
         self.loss = loss
         self.log_function = log_function
         self.train_bias = train_bias
 
-        if quantization_parameters_learning and rounding_type == RoundingType.STE:
-            common.Logger.error("Quantization parameters learning is not supported with STE rounding.")
-
-        self.quantization_parameters_learning = quantization_parameters_learning
         self.rounding_type = rounding_type
-        self.lsb_change_per_bit_width = lsb_change_per_bit_width
-        self.eps = eps
-        self.use_jac_based_weights = use_jac_based_weights
-        self.num_samples_for_loss = num_samples_for_loss
-        self.norm_weights = norm_weights
+        self.use_hessian_based_weights = use_hessian_based_weights
         self.optimizer_quantization_parameter = optimizer_quantization_parameter
         self.optimizer_bias = optimizer_bias
-        self.log_norm = log_norm
-        self.weights_n_iter = weights_n_iter
+        self.regularization_factor = regularization_factor
+        self.hessian_weights_config = hessian_weights_config
 
-        if self._verify_quantizer_config(quantizer_config, rounding_type):
-            self.quantizer_config = quantizer_config
-        else:
-            common.Logger.error(f"Quantizer config of type {type(quantizer_config)} "
-                                f"is not suitable for rounding type {rounding_type}")
-
-    def _verify_quantizer_config(self, quantizer_config, rounding_type) -> bool:
-        """
-        Verifies that the given quantizer config matches the given rounding type.
-
-        Args:
-            quantizer_config: A quantizer config.
-            rounding_type: A RoundingType.
-
-        Returns: True if the quantizer config matches the rounding type, False otherwise.
-
-        """
-        if rounding_type == RoundingType.SoftQuantizer:
-            return type(quantizer_config) == SoftQuantizerConfig
-
-        # Here, we compare type() and not isinstance to exclude instance equality because of inheritance
-        return type(quantizer_config) == GPTQQuantizerConfig
+        self.gptq_quantizer_params_override = {} if gptq_quantizer_params_override is None \
+            else gptq_quantizer_params_override
 
 
 class GradientPTQConfigV2(GradientPTQConfig):
     """
     Configuration to use for quantization with GradientPTQV2 (experimental).
     """
-    def __init__(self,
-                 n_epochs: int,
+    def __init__(self, n_epochs: int,
                  optimizer: Any,
                  optimizer_rest: Any = None,
                  loss: Callable = None,
                  log_function: Callable = None,
                  train_bias: bool = True,
-                 quantization_parameters_learning: bool = False,
                  rounding_type: RoundingType = RoundingType.SoftQuantizer,
-                 lsb_change_per_bit_width: dict = DefaultDict({}, lambda: 1),
-                 eps: float = 1e-6,
-                 use_jac_based_weights: bool = True,
-                 num_samples_for_loss: int = 16,
-                 norm_weights: bool = False,
+                 use_hessian_based_weights: bool = True,
                  optimizer_quantization_parameter: Any = None,
                  optimizer_bias: Any = None,
-                 log_norm: bool = True,
-                 weights_n_iter: int = 50,
-                 quantizer_config: GPTQQuantizerConfig = SoftQuantizerConfig()):
+                 regularization_factor: float = REG_DEFAULT,
+                 hessian_weights_config: GPTQHessianWeightsConfig = GPTQHessianWeightsConfig(),
+                 gptq_quantizer_params_override: Dict[str, Any] = None):
         """
         Initialize a GradientPTQConfigV2.
 
         Args:
             n_epochs (int): Number of representative dataset epochs to train.
             optimizer (Any): Optimizer to use.
             optimizer_rest (Any): Optimizer to use for bias and quantizer parameters.
             loss (Callable): The loss to use. should accept 6 lists of tensors. 1st list of quantized tensors, the 2nd list is the float tensors,
              the 3rd is a list of quantized weights, the 4th is a list of float weights, the 5th and 6th lists are the mean and std of the tensors
              accordingly. see example in multiple_tensors_mse_loss
             log_function (Callable): Function to log information about the GPTQ process.
             train_bias (bool): Whether to update the bias during the training or not.
-            quantization_parameters_learning (bool): Whether to update the quantization param during the training or not.
             rounding_type (RoundingType): An enum that defines the rounding type.
-            lsb_change_per_bit_width (dict): Whether to update the bias during the training or not.
-            eps (float): A floating point value for numeric stability.
-            use_jac_based_weights (bool): Whether to use jacobian-based weights for weighted average loss.
-            num_samples_for_loss (int): Number of samples to use for computing the jacobian-based weights.
-            norm_weights (bool): Whether to normalize the returned weights (to get values between 0 and 1).
+            use_hessian_based_weights (bool): Whether to use Hessian-based weights for weighted average loss.
             optimizer_quantization_parameter (Any): Optimizer to override the rest optimizer  for quantizer parameters.
             optimizer_bias (Any): Optimizer to override the rest optimizerfor bias.
-            log_norm (bool): Whether to use log normalization to the GPTQ Jacobian-based weights.
-            weights_n_iter (int): Number of random iterations to run Jacobian approximation for GPTQ weights.
-            quantizer_config (Any): A class that contains the quantizer specific config.
+            regularization_factor (float): A floating point number that defines the regularization factor.
+            hessian_weights_config (GPTQHessianWeightsConfig): A configuration that include all necessary arguments to run a computation of Hessian weights for the GPTQ loss.
+            gptq_quantizer_params_override (dict): A dictionary of parameters to override in GPTQ quantizer instantiation. Defaults to None (no parameters).
 
         """
 
         super().__init__(n_iter=None,
                          optimizer=optimizer,
                          optimizer_rest=optimizer_rest,
                          loss=loss,
                          log_function=log_function,
                          train_bias=train_bias,
-                         quantization_parameters_learning=quantization_parameters_learning,
                          rounding_type=rounding_type,
-                         lsb_change_per_bit_width=lsb_change_per_bit_width,
-                         eps=eps,
-                         use_jac_based_weights=use_jac_based_weights,
-                         num_samples_for_loss=num_samples_for_loss,
-                         norm_weights=norm_weights,
+                         use_hessian_based_weights=use_hessian_based_weights,
                          optimizer_quantization_parameter=optimizer_quantization_parameter,
                          optimizer_bias=optimizer_bias,
-                         log_norm=log_norm,
-                         weights_n_iter=weights_n_iter,
-                         quantizer_config=quantizer_config)
+                         regularization_factor=regularization_factor,
+                         hessian_weights_config=hessian_weights_config,
+                         gptq_quantizer_params_override=gptq_quantizer_params_override)
         self.n_epochs = n_epochs
 
     @classmethod
     def from_v1(cls, n_ptq_iter: int, config_v1: GradientPTQConfig):
         """
         Initialize a GradientPTQConfigV2 from GradientPTQConfig instance.
 
@@ -207,26 +179,7 @@
             config_v1 (GradientPTQConfig): A GPTQ config to convert to V2.
 
         """
         n_epochs = int(round(config_v1.n_iter) / n_ptq_iter)
         v1_params = config_v1.__dict__
         v1_params = {k: v for k, v in v1_params.items() if k != 'n_iter'}
         return cls(n_epochs, **v1_params)
-
-    def get_extended_quantizer_parametes(self) -> Dict[str, Any]:
-        """
-        Return a dictionary with a mapping to necessary additional parameters for initializing the GPTQ quantizer.
-
-        Returns: A dictionary with parameters for initializing a quantizer.
-
-        """
-
-        if self.rounding_type == RoundingType.SoftQuantizer:
-            return {N_BATCHES_STR: self.quantizer_config.n_batches,
-                    QUANT_PARAM_LEARNING_STR: self.quantization_parameters_learning,
-                    N_EPOCHS_STR: self.n_epochs}
-        elif self.rounding_type == RoundingType.STE:
-            return {MAX_LSB_STR: self.lsb_change_per_bit_width}
-
-        return {}
-
-
```

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/gptq/common/gptq_constants.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/common/gptq_constants.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,25 @@
 # Parameters names
 AUXVAR = 'auxvar_tensor'
 ITERVAR = 'iteration_variable'
 SCALE_TENSOR = "scale_ptq_tensor"
-GPTQ_ITER = "gptq_iter"
 AUXSHIFT = 'shift'
 WEIGHTS_QUANTIZATION_PARAMS = 'weights_quantization_params'
 PTQ_MIN_RANGE = "min_range"
 PTQ_MAX_RANGE = "max_range"
 PTQ_THRESHOLD = "ptq_threshold"
 SCALE_PTQ = "scale"
 
 # Default quantizer values
-N_EPOCHS = 10000
 N_CYCLES = 4
 MIM_TEMP = 0.5
 MAX_TEMP = 1.0
 REG_DEFAULT = 0.01
-MAX_ITERATIONS_DEFAULT = 10000
 MAX_LSB_CHANGE = 1
 
 # Soft rounding arguments values
 SOFT_ROUNDING_GAMMA = -0.1
 SOFT_ROUNDING_ZETA = 1.1
-SOFT_ROUNDING_BETA = 2 / 3
 
 # GPTQ config constant
-REGULARIZATION_VALUES = "regularization_values"
-N_BATCHES_STR = 'n_batches'
 QUANT_PARAM_LEARNING_STR = 'quantization_parameter_learning'
-N_EPOCHS_STR = 'n_epochs'
 MAX_LSB_STR = 'max_lsbs_change_map'
```

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/gptq/common/gptq_graph.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/common/gptq_graph.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/gptq/common/gptq_training.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/common/gptq_training.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,47 +12,46 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 import copy
 from abc import ABC, abstractmethod
 import numpy as np
 from typing import Callable, List, Any
-from model_compression_toolkit.gptq.common.gptq_config import GradientPTQConfig, RoundingType
+from model_compression_toolkit.gptq.common.gptq_config import GradientPTQConfig
 from model_compression_toolkit.core.common import Graph, Logger, BaseNode
 from model_compression_toolkit.core.common.framework_info import FrameworkInfo
 from model_compression_toolkit.core.common.framework_implementation import FrameworkImplementation
+from model_compression_toolkit.gptq.common.gptq_constants import QUANT_PARAM_LEARNING_STR
 from model_compression_toolkit.gptq.common.gptq_graph import get_compare_points
 from model_compression_toolkit.core.common.model_builder_mode import ModelBuilderMode
 
 
 class GPTQTrainer(ABC):
     """
     Abstract GPTQ training class for fine-tuning a quantized model
     """
 
     def __init__(self,
                  graph_float: Graph,
                  graph_quant: Graph,
                  gptq_config: GradientPTQConfig,
                  fw_impl: FrameworkImplementation,
-                 fw_info: FrameworkInfo,
-                 representative_data_gen: Callable):
+                 fw_info: FrameworkInfo):
         """
         Build two models from a graph: A teacher network (float model) and a student network (quantized model).
         Use the dataset generator to pass images through the teacher and student networks to get intermediate
         layers outputs. Use the outputs to compute the observed loss and to back-propagate the error
         in the student network, to minimize it in the next similar steps.
         All parameters (such as number of iterations, optimizer, etc.) are in GradientPTQConfig.
         Args:
             graph_float: Graph to build a float networks from.
             graph_quant: Graph to build a quantized networks from.
             gptq_config: GradientPTQConfig with parameters about the tuning process.
             fw_impl: Framework implementation
             fw_info: Framework information
-            representative_data_gen: Dataset to use for inputs of the models.
         """
         self.graph_float = copy.deepcopy(graph_float)
         self.graph_quant = copy.deepcopy(graph_quant)
         self.gptq_config = gptq_config
         self.fw_impl = fw_impl
         self.fw_info = fw_info
 
@@ -62,18 +61,14 @@
         self.compare_points, _, self.compare_points_mean, self.compare_points_std = get_compare_points(self.graph_float)
 
         self.float_model, self.float_user_info = fw_impl.model_builder(self.graph_float,
                                                                        mode=ModelBuilderMode.FLOAT,
                                                                        append2output=self.compare_points,
                                                                        fw_info=self.fw_info)
 
-        if self.gptq_config.rounding_type == RoundingType.SoftQuantizer:
-            # dry run on the representative dataset to count number of batches
-            self.count_num_batches_for_training(representative_data_gen)
-
         self.fxp_model, self.gptq_user_info = self.build_gptq_model()
 
     def get_optimizer_with_param(self,
                                  flattened_trainable_weights: List[Any],
                                  flattened_bias_weights: List[Any],
                                  trainable_quantization_parameters: List[Any]) -> List[Any]:
         """
@@ -84,52 +79,61 @@
             trainable_quantization_parameters: list of trainable quantization parameters
         Returns:
             List of Optimizer objects with parameters
         """
 
         w2train = [*flattened_trainable_weights]
 
+        quant_params_learning = self.gptq_config.gptq_quantizer_params_override.get(QUANT_PARAM_LEARNING_STR, False)
+
         optimizer_with_param = [(self.gptq_config.optimizer, w2train)]
-        if self.gptq_config.train_bias or self.gptq_config.quantization_parameters_learning:
+        if self.gptq_config.train_bias or quant_params_learning:
             w2train_res = []
             if self.gptq_config.train_bias:
                 if self.gptq_config.optimizer_bias is not None:
                     optimizer_with_param.append((self.gptq_config.optimizer_bias, flattened_bias_weights))
                 else:
                     w2train_res.extend(flattened_bias_weights)
                     if self.gptq_config.optimizer_rest is None:
                         Logger.error(  # pragma: no cover
                             "To enable bias micro training an additional optimizer is required, please define the optimizer_rest")
-            if self.gptq_config.quantization_parameters_learning:
+            if quant_params_learning:
                 if self.gptq_config.optimizer_quantization_parameter is not None:  # Ability to override optimizer
                     optimizer_with_param.append((self.gptq_config.optimizer_quantization_parameter,
                                                  trainable_quantization_parameters))
                 else:
                     w2train_res.extend(trainable_quantization_parameters)
                 if self.gptq_config.optimizer_rest is None:
                     Logger.error(  # pragma: no cover
-                        "To enable bias micro training an additional optimizer is required, please define the optimizer_rest")
-            optimizer_with_param.append((self.gptq_config.optimizer_rest, w2train_res))
+                        "To enable quantization parameters micro training an additional optimizer is required, please define the optimizer_rest")
+            if len(w2train_res) > 0:
+                # Either bias or quantization parameters are trainable but did not provide a specific optimizer,
+                # so we should use optimizer_rest to train them
+                if self.gptq_config.optimizer_rest is None:
+                    Logger.error(  # pragma: no cover
+                        "To enable bias or quantization parameters micro training an additional optimizer is required, please define the optimizer_rest")
+                optimizer_with_param.append((self.gptq_config.optimizer_rest, w2train_res))
 
         return optimizer_with_param
 
 
-    def compute_jacobian_based_weights(self,
-                                       representative_data_gen: Callable) -> np.ndarray:
+    def compute_hessian_based_weights(self,
+                                      representative_data_gen: Callable) -> np.ndarray:
         """
-        Computes the jacobian-based weights using the framework's model_grad method per batch of images.
+        Computes the Hessian-based weights using the framework's model_grad method per batch of images.
 
         Args:
-            representative_data_gen: Dataset used for inference to compute the jacobian-based weights.
+            representative_data_gen: Dataset used for inference to compute the Hessian-based weights.
 
         Returns: A vector of weights, one for each compare point,
         to be used for the loss metric weighted average computation when running GPTQ training.
         """
-        if self.gptq_config.use_jac_based_weights:
-            images = self._generate_images_batch(representative_data_gen, self.gptq_config.num_samples_for_loss)
+        if self.gptq_config.use_hessian_based_weights:
+            images = self._generate_images_batch(representative_data_gen,
+                                                 self.gptq_config.hessian_weights_config.hessians_num_samples)
 
             model_output_replacement = self._get_model_output_replacement()
 
             points_apprx_jacobians_weights = []
             for i in range(1, images.shape[0] + 1):
                 Logger.info(f"Computing Jacobian-based weights approximation for image sample {i} out of {images.shape[0]}...")
                 # Note that in GPTQ loss weights computation we assume that there aren't replacement output nodes,
@@ -139,25 +143,26 @@
                                                              {inode: self.fw_impl.to_tensor(images[i - 1:i]) for inode
                                                               in
                                                               self.graph_float.get_inputs()},
                                                              self.compare_points,
                                                              output_list=model_output_replacement,
                                                              all_outputs_indices=[],
                                                              alpha=0,
-                                                             norm_weights=self.gptq_config.norm_weights,
-                                                             n_iter=self.gptq_config.weights_n_iter)
+                                                             norm_weights=self.gptq_config.hessian_weights_config.norm_weights,
+                                                             n_iter=self.gptq_config.hessian_weights_config.hessians_n_iter)
                 points_apprx_jacobians_weights.append(image_ip_gradients)
-            if self.gptq_config.log_norm:
+            if self.gptq_config.hessian_weights_config.log_norm:
                 mean_jacobian_weights = np.mean(points_apprx_jacobians_weights, axis=0)
                 mean_jacobian_weights = np.where(mean_jacobian_weights != 0, mean_jacobian_weights,
                                                  np.partition(mean_jacobian_weights, 1)[1])
                 log_weights = np.log10(mean_jacobian_weights)
 
-                # To add scaling to the normalized weights replace return statement with the following line:
-                # return log_weights - np.min(log_weights) / (np.max(log_weights) - np.min(log_weights))
+                if self.gptq_config.hessian_weights_config.scale_log_norm:
+                    return (log_weights - np.min(log_weights)) / (np.max(log_weights) - np.min(log_weights))
+
                 return log_weights - np.min(log_weights)
             else:
                 return np.mean(points_apprx_jacobians_weights, axis=0)
         else:
             num_nodes = len(self.compare_points)
             return np.asarray([1 / num_nodes for _ in range(num_nodes)])
 
@@ -245,29 +250,14 @@
                 prev_node = self.graph_float.get_prev_nodes(n.node)
                 assert len(prev_node) == 1, "A none compatible output node has multiple inputs, " \
                                             "which is incompatible for metric computation."
                 prev_node = prev_node[0]
             replacement_outputs.append(prev_node)
         return replacement_outputs
 
-    def count_num_batches_for_training(self, representative_data_gen):
-        """
-        Runs a "dry-run" of the representative dataset to count the number of batches for each training epoch.
-
-        Args:
-            representative_data_gen: A callable method to retrieve images from Dataset.
-
-        Returns: The number of batches for each training epoch.
-
-        """
-        num_batches = 0
-        for _ in representative_data_gen():
-            num_batches += 1
-        self.gptq_config.quantizer_config.set_num_batches(num_batches)
-
 
 def gptq_training(graph_float: Graph,
                   graph_quant: Graph,
                   gptq_config: GradientPTQConfig,
                   representative_data_gen: Callable,
                   fw_impl: FrameworkImplementation,
                   fw_info: FrameworkInfo) -> Graph:
```

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/gptq/keras/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/gptq/keras/gptq_loss.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/keras/gptq_loss.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/gptq/keras/gptq_training.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/keras/gptq_training.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,48 +8,46 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-from functools import partial
 from typing import Callable, List, Tuple, Union
 
 import tensorflow as tf
 from keras import Model
 from tensorflow.keras.layers import Layer
 from tqdm import tqdm
 
 # As from Tensorflow 2.6, keras is a separate package and some classes should be imported differently.
 from model_compression_toolkit.core.common.user_info import UserInformation
 from model_compression_toolkit.core.keras.back2framework.keras_model_builder import KerasModelBuilder
-from model_compression_toolkit.gptq.common.gptq_constants import REGULARIZATION_VALUES
 from packaging import version
 
 from model_compression_toolkit.gptq.common.gptq_graph import get_kernel_attribute_name_for_gptq
 from model_compression_toolkit.gptq.keras.quantizer.quantization_builder import quantization_builder
 from model_compression_toolkit.quantizers_infrastructure import KerasQuantizationWrapper
 
 if version.parse(tf.__version__) < version.parse("2.6"):
     from tensorflow.python.keras.engine.base_layer import TensorFlowOpLayer
 else:
     from keras.engine.base_layer import TensorFlowOpLayer
 
 from model_compression_toolkit.core import common
 from model_compression_toolkit.gptq.common.gptq_training import GPTQTrainer
-from model_compression_toolkit.gptq.common.gptq_config import GradientPTQConfigV2, RoundingType
+from model_compression_toolkit.gptq.common.gptq_config import GradientPTQConfigV2
 from model_compression_toolkit.core.common import Graph
-from model_compression_toolkit.gptq.keras.graph_info import get_weights_for_loss, \
-    get_soft_rounding_reg, get_gptq_trainable_parameters
+from model_compression_toolkit.gptq.keras.graph_info import get_weights_for_loss, get_gptq_trainable_parameters
+from model_compression_toolkit.gptq.keras.quantizer.regularization_factory import get_regularization
 from model_compression_toolkit.core.common.framework_info import FrameworkInfo
 from model_compression_toolkit.core.common.framework_implementation import FrameworkImplementation
 import numpy as np
 import copy
-from model_compression_toolkit.core.keras.constants import BIAS, USE_BIAS, KERNEL
+from model_compression_toolkit.core.keras.constants import BIAS, USE_BIAS
 from model_compression_toolkit import quantizers_infrastructure as qi
 
 
 class KerasGPTQTrainer(GPTQTrainer):
     """
     Keras GPTQ training class for fine-tuning a quantized model
     """
@@ -75,21 +73,20 @@
             fw_info: Framework information.
             representative_data_gen: Dataset to use for inputs of the models.
         """
         super().__init__(graph_float,
                          graph_quant,
                          gptq_config,
                          fw_impl,
-                         fw_info,
-                         representative_data_gen)
+                         fw_info)
 
         self.loss_list = []
         self.input_scale = 1
 
-        trainable_weights, bias_weights, trainable_threshold, temperature_weights = get_gptq_trainable_parameters(
+        trainable_weights, bias_weights, trainable_threshold = get_gptq_trainable_parameters(
             self.fxp_model,
             fw_info,
             add_bias=gptq_config.train_bias)
 
         self.flp_weights_list, self.fxp_weights_list = get_weights_for_loss(self.fxp_model)
 
         if not (len(self.compare_points) == len(trainable_weights) == len(self.flp_weights_list) == len(
@@ -108,15 +105,17 @@
             [len(optimizer_params_tuple[1]) for optimizer_params_tuple in self.optimizer_with_param]) > 0
 
         if self.float_user_info.input_scale != self.gptq_user_info.input_scale:
             common.Logger.error("Input scale mismatch between float and GPTQ networks")  # pragma: no cover
         else:
             self.input_scale = self.gptq_user_info.input_scale
 
-        self.weights_for_average_loss = self.compute_jacobian_based_weights(representative_data_gen)
+        self.weights_for_average_loss = self.compute_hessian_based_weights(representative_data_gen)
+
+        self.reg_func = get_regularization(self.gptq_config, representative_data_gen)
 
     def _is_gptq_applicable(self,
                             node: common.BaseNode) -> bool:
         """
         A function for deciding if a layer should be fine-tuned during GPTQ.
 
         Args:
@@ -191,17 +190,15 @@
                                                in_y_float,
                                                self.fxp_weights_list,
                                                self.flp_weights_list,
                                                self.compare_points_mean,
                                                self.compare_points_std,
                                                self.weights_for_average_loss)
 
-            reg_value = self.gptq_config.quantizer_config.get_regularization_value(
-                self.fxp_model,
-                **{REGULARIZATION_VALUES: self._get_quantizer_regularization_values(self.gptq_config.rounding_type)})
+            reg_value = self.reg_func(self.fxp_model, self.gptq_config.regularization_factor)
 
             loss_value += reg_value
 
         # Use the gradient tape to automatically retrieve
         # the gradients of the trainable variables with respect to the loss.
         grads = tape.gradient(loss_value, param2grad)
         res = []
@@ -315,22 +312,7 @@
                 if self.gptq_config.train_bias:
                     use_bias = layer.layer.get_config().get(USE_BIAS)
                     if use_bias is not None and use_bias:
                         new_bias = layer.layer.bias.numpy()
                         node.set_weights_by_keys(BIAS, new_bias)
 
         return graph
-
-    def _get_quantizer_regularization_values(self, rounding_type: RoundingType) -> List[tf.Tensor]:
-        """
-        Mapping between a rounding type to its matching regularization method.
-
-        Args:
-            rounding_type: GPTQ rounding type.
-
-        Returns: A regularization computation method.
-
-        """
-        if rounding_type == RoundingType.SoftQuantizer:
-            return get_soft_rounding_reg(self.fxp_model)
-        else:
-            return []
```

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/gptq/keras/graph_info.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/keras/graph_info.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,31 +9,29 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
-
 import tensorflow as tf
 from typing import Tuple, List
-
 from model_compression_toolkit.core.keras.constants import USE_BIAS
 from model_compression_toolkit.core.common.framework_info import FrameworkInfo
 from tensorflow.keras.models import Model
-
 from model_compression_toolkit.core.keras.default_framework_info import DEFAULT_KERAS_INFO
 from model_compression_toolkit.gptq.common.gptq_graph import get_kernel_attribute_name_for_gptq
 from model_compression_toolkit.quantizers_infrastructure import KerasQuantizationWrapper
+from model_compression_toolkit.quantizers_infrastructure.trainable_infrastructure.common.base_trainable_quantizer import VariableGroup
 
 
 def get_gptq_trainable_parameters(fxp_model: Model,
                                   fw_info: FrameworkInfo,
                                   add_bias: bool = False) -> (
-        List[tf.Variable], List[tf.Variable], List[tf.Variable], List[tf.Variable], List[tf.Variable]):
+        List[tf.Variable], List[tf.Variable], List[tf.Variable]):
     """
     Get trainable parameters from all layers in a model
 
     Args:
         fxp_model: Model to get its trainable parameters.
         fw_info: Framework information needed for keras kernel ops list.
         add_bias: Whether to include biases of the model (if there are) or not.
@@ -41,35 +39,34 @@
     Returns:
         A list of trainable variables in a model. Each item is a list of a layers weights.
     """
 
     trainable_weights: List[tf.Tensor] = []
     trainable_threshold: List[tf.Tensor] = []
     bias_weights: List[List[tf.Tensor]] = []
-    temperature_weights: List[tf.Tensor] = []
 
     for layer in fxp_model.layers:
         if isinstance(layer, KerasQuantizationWrapper):
             kernel_attribute = get_kernel_attribute_name_for_gptq(layer_type=type(layer.layer),
                                                                   fw_info=DEFAULT_KERAS_INFO)
 
-            # collect trainable weights per layer
-            layer_trainable_weights = layer.weights_quantizers[kernel_attribute].get_aux_variable()
-            layer_trainable_threshold = layer.weights_quantizers[kernel_attribute].get_quantization_variable()
+            # collect trainable weights per quantizer
+            quantizer_trainable_weights = layer.weights_quantizers[kernel_attribute].get_trainable_variables(VariableGroup.WEIGHTS)
+            quantizer_trainable_threshold = layer.weights_quantizers[kernel_attribute].get_trainable_variables(VariableGroup.QPARAMS)
+            trainable_weights.append(quantizer_trainable_weights)
+            trainable_threshold.extend(quantizer_trainable_threshold)
 
             if add_bias:
                 kernel_ops_attrs = fw_info.kernel_ops_attributes_mapping.get(type(layer.layer))
                 use_bias = kernel_ops_attrs is not None and kernel_ops_attrs[0] is not None \
                            and layer.layer.get_config().get(USE_BIAS)
                 if use_bias is not None and use_bias:
                     bias_weights.append([layer.layer.bias])
-            trainable_weights.append(layer_trainable_weights)
-            trainable_threshold.extend(layer_trainable_threshold)
 
-    return trainable_weights, bias_weights, trainable_threshold, temperature_weights
+    return trainable_weights, bias_weights, trainable_threshold
 
 
 def get_weights_for_loss(fxp_model: Model) -> Tuple[List[list], List[list]]:
     """
     Get all float and quantized kernels for the GPTQ loss
 
     Args:
@@ -91,29 +88,7 @@
                 _layer_flp_weights.append(quantizer_vars)
                 _layer_fxp_weights.append(quantizer(training=False, inputs=quantizer_vars))
 
             flp_weights_list.append(_layer_flp_weights)
             fxp_weights_list.append(_layer_fxp_weights)
 
     return flp_weights_list, fxp_weights_list
-
-
-# TODO: this function need to move to location that is relevant only for soft quantizer -
-#  once deciding how to handle GPTQ quantizers regularization.
-def get_soft_rounding_reg(fxp_model: Model) -> List[tf.Tensor]:
-    """
-    This function returns the soft quantizer regularization values for SoftRounding.
-
-    Args:
-        fxp_model: A model to be quantized with SoftRounding.
-
-    Returns: A list of tensors.
-    """
-
-    soft_reg_aux: List[tf.Tensor] = []
-    for layer in fxp_model.layers:
-        if isinstance(layer, KerasQuantizationWrapper):
-            kernel_attribute = get_kernel_attribute_name_for_gptq(layer_type=type(layer.layer),
-                                                                  fw_info=DEFAULT_KERAS_INFO)
-
-            soft_reg_aux.append(layer.weights_quantizers[kernel_attribute].get_regularization())
-    return soft_reg_aux
```

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/gptq/keras/quantization_facade.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/keras/quantization_facade.py`

 * *Files 3% similar despite different names*

```diff
@@ -81,32 +81,26 @@
             Import MCT and TensorFlow:
 
             >>> import model_compression_toolkit as mct
             >>> import tensorflow as tf
 
             Create a GradientPTQConfigV2 to run for 5 epochs:
 
-            >>> gptq_conf = mct.get_keras_gptq_config(n_epochs=5)
+            >>> gptq_conf = mct.gptq.get_keras_gptq_config(n_epochs=5)
 
             Other Tensorflow optimizers can be passed:
 
-            >>> gptq_conf = mct.get_keras_gptq_config(n_epochs=3, optimizer=tf.keras.optimizers.Nadam())
+            >>> gptq_conf = mct.gptq.get_keras_gptq_config(n_epochs=3, optimizer=tf.keras.optimizers.Nadam())
 
             The configuration can be passed to :func:`~model_compression_toolkit.keras_post_training_quantization` in order to quantize a keras model using gptq.
 
         """
         bias_optimizer = tf.keras.optimizers.SGD(learning_rate=LR_BIAS_DEFAULT, momentum=GPTQ_MOMENTUM)
-        return GradientPTQConfigV2(n_epochs,
-                                   optimizer,
-                                   optimizer_rest=optimizer_rest,
-                                   loss=loss,
-                                   log_function=log_function,
-                                   train_bias=True,
-                                   quantization_parameters_learning=True,
-                                   optimizer_bias=bias_optimizer)
+        return GradientPTQConfigV2(n_epochs, optimizer, optimizer_rest=optimizer_rest, loss=loss,
+                                   log_function=log_function, train_bias=True, optimizer_bias=bias_optimizer)
 
 
     def keras_gradient_post_training_quantization_experimental(in_model: Model,
                                                                representative_data_gen: Callable,
                                                                gptq_config: GradientPTQConfigV2,
                                                                gptq_representative_data_gen: Callable = None,
                                                                target_kpi: KPI = None,
@@ -177,19 +171,19 @@
             that should be quantized (for example, the kernel of Conv2D in Keras will be affected by this value,
             while the bias will not):
 
             >>> kpi = mct.KPI(model.count_params() * 0.75)  # About 0.75 of the model size when quantized with 8 bits.
 
             Create GPTQ config:
 
-            >>> gptq_config = mct.get_keras_gptq_config(n_epochs=1)
+            >>> gptq_config = mct.gptq.get_keras_gptq_config(n_epochs=1)
 
             Pass the model with the representative dataset generator to get a quantized model:
 
-            >>> quantized_model, quantization_info = mct.keras_gradient_post_training_quantization_experimental(model, repr_datagen, gptq_config, target_kpi=kpi, core_config=config)
+            >>> quantized_model, quantization_info = mct.gptq.keras_gradient_post_training_quantization_experimental(model, repr_datagen, gptq_config, target_kpi=kpi, core_config=config)
 
         """
         KerasModelValidation(model=in_model,
                              fw_info=fw_info).validate()
 
         if core_config.mixed_precision_enable:
             if not isinstance(core_config.mixed_precision_config, MixedPrecisionQuantizationConfigV2):
```

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/gptq/keras/quantizer/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/keras/quantizer/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/gptq/keras/quantizer/base_keras_gptq_quantizer.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/keras/quantizer/base_keras_gptq_quantizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,15 +41,14 @@
 
             Args:
                 quantization_config: quantizer config class contains all the information about a quantizer configuration.
             """
 
             super().__init__(quantization_config)
 
-            self.quantizer_parameters = None
 
         def update_layer_quantization_params(self, layer: KerasQuantizationWrapper
                                              ) -> (Dict[str, tf.Tensor], Dict[str, Dict], Dict):
             """
             A Function to calculate the needed change in attributes in NodeQuantizationConfig after retraining.
 
             Args:
```

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/gptq/keras/quantizer/quant_utils.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/keras/quantizer/quant_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/gptq/keras/quantizer/quantization_builder.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/keras/quantizer/quantization_builder.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from typing import Dict, List, Tuple
 
-from model_compression_toolkit import GradientPTQConfigV2
+from model_compression_toolkit.gptq import GradientPTQConfigV2
 from model_compression_toolkit.core import common
 from model_compression_toolkit.core.keras.default_framework_info import DEFAULT_KERAS_INFO
 from model_compression_toolkit.exporter.model_wrapper.keras.builder.node_to_quantizer import \
     get_inferable_quantizer_kwargs
 from model_compression_toolkit.gptq.common.gptq_graph import get_kernel_attribute_name_for_gptq
 from model_compression_toolkit.gptq.keras.quantizer.base_keras_gptq_quantizer import BaseKerasGPTQTrainableQuantizer
 from model_compression_toolkit.quantizers_infrastructure import QuantizationTarget
@@ -57,15 +57,15 @@
                                                         quantizer_type=gptq_config.rounding_type,
                                                         quant_method=quant_method,
                                                         quantizer_base_class=BaseKerasGPTQTrainableQuantizer)
         kernel_attribute = get_kernel_attribute_name_for_gptq(layer_type=n.type,
                                                               fw_info=DEFAULT_KERAS_INFO)
 
         weights_quantizers.update({kernel_attribute: quantizer_class(get_trainable_quantizer_weights_config(n),
-                                                                     **gptq_config.get_extended_quantizer_parametes())})
+                                                                     **gptq_config.gptq_quantizer_params_override)})
 
     activation_quantizers = []
     if n.is_activation_quantization_enabled():
         quant_method = n.final_activation_quantization_cfg.activation_quantization_method
 
         quantizer_class = get_inferable_quantizer_class(quant_target=QuantizationTarget.Activation,
                                                         quant_method=quant_method,
```

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/symmetric_soft_quantizer.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/symmetric_soft_quantizer.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,30 +12,30 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
 import tensorflow as tf
 import numpy as np
 
-from model_compression_toolkit import RoundingType
+from model_compression_toolkit.gptq import RoundingType
 from model_compression_toolkit import quantizers_infrastructure as qi
 from model_compression_toolkit.core.common import max_power_of_two
 from model_compression_toolkit.core.common.target_platform import QuantizationMethod
-from model_compression_toolkit.gptq.common.gptq_constants import PTQ_THRESHOLD, SCALE_PTQ, N_EPOCHS, \
-    MAX_ITERATIONS_DEFAULT, SOFT_ROUNDING_GAMMA, SOFT_ROUNDING_ZETA, SOFT_ROUNDING_BETA, GPTQ_ITER, AUXVAR
+from model_compression_toolkit.gptq.common.gptq_constants import PTQ_THRESHOLD, SCALE_PTQ, \
+    SOFT_ROUNDING_GAMMA, SOFT_ROUNDING_ZETA, AUXVAR
 from model_compression_toolkit.gptq.keras.quantizer import quant_utils as qutils
-from typing import Dict, Any, List
+from typing import Dict, Any
 from model_compression_toolkit.core.common.constants import THRESHOLD, MIN_THRESHOLD
-from model_compression_toolkit.core.common.logger import Logger
 from model_compression_toolkit.gptq.keras.quantizer.base_keras_gptq_quantizer import BaseKerasGPTQTrainableQuantizer
 from model_compression_toolkit.gptq.keras.quantizer.quant_utils import power_of_two_max, clip, calculate_delta
 from model_compression_toolkit.quantizers_infrastructure import TrainableQuantizerWeightsConfig
 from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.common.base_inferable_quantizer import mark_quantizer
 from model_compression_toolkit.quantizers_infrastructure.trainable_infrastructure.common.quant_utils import \
     get_threshold_reshape_shape
+from model_compression_toolkit.quantizers_infrastructure.trainable_infrastructure.common.base_trainable_quantizer import VariableGroup
 
 
 def soft_rounding_symmetric_quantizer(input_tensor: tf.Tensor,
                                       auxvar_tensor: tf.Variable,
                                       threshold_tensor: tf.Tensor,
                                       num_bits: int,
                                       signed: bool,
@@ -62,81 +62,33 @@
     input_tensor_int = tf.floor(input_tensor / delta)
     tensor_q = input_tensor_int + auxvar_tensor
     min_int = -int(signed) * (2 ** (num_bits - int(signed)))
     max_int = (2 ** (num_bits - int(signed))) - 1
     return delta * clip(tensor_q, max_val=max_int, min_val=min_int)
 
 
-class LinearTempDecay:
-    """
-    Annealing process for the soft quantizer regularization temperature term.
-    """
-
-    def __init__(self, t_max: int, rel_start_decay: float = 0.2, start_b: int = 20, end_b: int = 2):
-        """
-        Initializes a LinearTempDecay object.
-
-        Args:
-            t_max: maximal time step.
-            rel_start_decay: Decay step size at the beginning of the process.
-            start_b: Starting value of the regularization term.
-            end_b: Target value of the regularization term.
-        """
-
-        self.t_max = t_max
-        self.start_decay = rel_start_decay * t_max
-        self.start_b = start_b
-        self.end_b = end_b
-
-    def __call__(self, t: int) -> float:
-        """
-        Cosine annealing scheduler for soft quantizer regularization temperature term.
-
-        Args:
-            t: The current time step.
-
-        Returns: Scheduled temperature.
-        """
-
-        is_before_start_decay = tf.cast(t < self.start_decay, tf.float32)
-
-        rel_t = (t - self.start_decay) / (self.t_max - self.start_decay)
-
-        return self.start_b * is_before_start_decay + \
-               (1 - is_before_start_decay) * \
-               (self.end_b + (self.start_b - self.end_b) * tf.math.maximum(0.0, (1 - rel_t)))
-
-
 @mark_quantizer(quantization_target=qi.QuantizationTarget.Weights,
                 quantization_method=[QuantizationMethod.POWER_OF_TWO, QuantizationMethod.SYMMETRIC],
                 quantizer_type=RoundingType.SoftQuantizer)
 class SymmetricSoftRoundingGPTQ(BaseKerasGPTQTrainableQuantizer):
     """
     Trainable symmetric quantizer to optimize the rounding of the quantized values using a soft quantization method.
     """
 
     def __init__(self,
                  quantization_config: TrainableQuantizerWeightsConfig,
-                 n_batches: int = None,
-                 quantization_parameter_learning: bool = False,
-                 n_epochs: int = N_EPOCHS):
+                 quantization_parameter_learning: bool = False):
         """
         Initialize a SymmetricSoftRoundingGPTQ object with parameters to use
         for the quantization.
 
         Args:
             quantization_config: Trainable weights quantizer config.
-            n_batches: The expected number of batches for each training epoch.
             quantization_parameter_learning: Whether to train the quantization threshold.
-            n_epochs: Number of epochs to run training for.
         """
-
-        if n_batches is None:
-            Logger.error("SymmetricSoftRoundingGPTQ got an uninitialized n_batches argument.")
-
         super().__init__(quantization_config)
         self.num_bits = quantization_config.weights_n_bits
         self.per_channel = quantization_config.weights_per_channel_threshold
 
         threshold_values = quantization_config.weights_quantization_params[THRESHOLD]
         self.threshold_shape = np.asarray(threshold_values).shape
         self.threshold_values = np.reshape(np.asarray(threshold_values), [-1]) if self.per_channel else np.asarray(
@@ -144,55 +96,40 @@
 
         self.quantization_axis = quantization_config.weights_channels_axis
         self.power_of_two = quantization_config.weights_quantization_method == QuantizationMethod.POWER_OF_TWO
         self.quantization_parameter_learning = quantization_parameter_learning
         self.num_channels = len(self.threshold_values) if self.per_channel else 1
 
         # gamma and zeta are stretch parameters for computing the rectified sigmoind function.
-        # beta is used to set the regularization term.
         # See: https://arxiv.org/pdf/2004.10568.pdf
         self.gamma = SOFT_ROUNDING_GAMMA
         self.zeta = SOFT_ROUNDING_ZETA
-        self.beta = SOFT_ROUNDING_BETA
 
         self.quantizer_parameters = {}
 
-        # Initializing the temperature decay according to the number of expected gradient steps
-        init_decay = MAX_ITERATIONS_DEFAULT if n_batches is None else n_epochs * n_batches
-        self.linear_decay = LinearTempDecay(init_decay)
-
     def initialize_quantization(self,
                                 tensor_shape: Any,
                                 name: str,
-                                layer: Any) -> Dict[Any, Any]:
+                                layer: Any):
         """
-        Return a dictionary of quantizer parameters and their names.
+        Add quantizer parameters to the quantizer parameters dictionary
 
         Args:
             tensor_shape: tensor shape of the quantized tensor.
             name: Tensor name.
             layer: Layer to quantize.
-
-        Returns:
-            Dictionary of parameters names to the variables.
         """
 
         if self.per_channel:
             reshape_shape = get_threshold_reshape_shape(tensor_shape,
                                                         quant_axis=self.quantization_axis,
                                                         quant_axis_dim=self.num_channels)
         else:
             reshape_shape = [self.num_channels]
 
-        ar_iter = layer.add_weight(
-            f"{name}_{GPTQ_ITER}",
-            shape=(),
-            initializer=tf.keras.initializers.Constant(0.0),
-            trainable=False)
-
         ptq_threshold_tensor = layer.add_weight(
             f"{name}_{PTQ_THRESHOLD}",
             shape=reshape_shape,
             initializer=tf.keras.initializers.Constant(1.0),
             trainable=False)
         ptq_threshold_tensor.assign(self.threshold_values.reshape(reshape_shape))
 
@@ -208,72 +145,36 @@
         rest = (w / delta) - w_floor  # rest of rounding [0, 1)
         # Note that (rest - self.gamma) can't be zero since rest is positive and gamma is negative, so the division
         # is safe
         alpha = -qutils.safe_log((self.zeta - self.gamma) / (rest - self.gamma) - 1, 1e-16)  # => sigmoid(alpha) = rest
 
         auxvar_tensor.assign(alpha)
 
-        self.quantizer_parameters.update({AUXVAR: auxvar_tensor,
-                                          PTQ_THRESHOLD: ptq_threshold_tensor,
-                                          GPTQ_ITER: ar_iter})
+        # Add quantization variables
+        self.add_quantizer_variable(AUXVAR, auxvar_tensor, VariableGroup.WEIGHTS)
+        self.add_quantizer_variable(PTQ_THRESHOLD, ptq_threshold_tensor, VariableGroup.QPARAMS)
 
-        if self.quantization_parameter_learning:
+        if self.quantization_parameter_learning and not self.power_of_two:
             scale = layer.add_weight(
                 f"{name}_{SCALE_PTQ}",
                 shape=self.num_channels,
                 initializer=tf.keras.initializers.Constant(1.0),
                 trainable=True)
-            self.quantizer_parameters.update({SCALE_PTQ: scale})
-
-        return self.quantizer_parameters
-
-    def get_quantization_variable(self) -> List[tf.Tensor]:
-        """
-        This function return a list with the quantizer's quantization parameters variables.
-
-        Returns: A list with the quantization parameters if there are defined parameters.
-
-        """
-
-        if self.quantization_parameter_learning and not self.power_of_two:
-            return [self.quantizer_parameters[SCALE_PTQ]]
-        else:
-            return []
-
-    def get_regularization(self) -> tf.Tensor:
-        """
-        Computes the regularization term for the soft rounding loss.
-
-        Returns:
-            regularization term.
-        """
-
-        st = self.get_soft_targets()
-        b = self.linear_decay(self.ar_iter.value())
-        return tf.reduce_sum(1 - tf.pow(tf.math.abs(st - .5) * 2, b))
+            self.add_quantizer_variable(SCALE_PTQ, scale, VariableGroup.QPARAMS)
 
     def get_soft_targets(self) -> tf.Tensor:
         """
         Computes the rectified sigmoid function for the quantization target parameters.
 
         Returns:
             A tensor with the soft rounding targets values.
 
         """
         return qutils.clip(
-            tf.sigmoid(self.quantizer_parameters[AUXVAR]) * (self.zeta - self.gamma) + self.gamma, 1, 0)
-
-    def get_aux_variable(self) -> List[tf.Tensor]:
-        """
-        This function return a list with the quantizer's quantization auxiliary variables.
-
-        Returns: A list with the quantization auxiliary variables.
-
-        """
-        return [self.quantizer_parameters[AUXVAR]]
+            tf.sigmoid(self.get_quantizer_variable(AUXVAR)) * (self.zeta - self.gamma) + self.gamma, 1, 0)
 
     def __call__(self,
                  inputs: tf.Tensor,
                  training: bool):
         """
         Quantize a tensor.
 
@@ -281,73 +182,75 @@
             inputs: Input tensor to quantize.
             training: Whether the graph is in training mode.
 
         Returns:
             The quantized tensor.
         """
 
-        self.ar_iter = self.quantizer_parameters[GPTQ_ITER]
-        ptq_threshold_tensor = self.quantizer_parameters[PTQ_THRESHOLD]
+        ptq_threshold_tensor = self.get_quantizer_variable(PTQ_THRESHOLD)
+
+        #####################################################
+        # Soft Rounding
+        #####################################################
+        aux_var = self.get_soft_targets()
+        if not training:
+            aux_var = tf.cast(tf.math.greater_equal(aux_var, 0.5), tf.float32)
 
         if self.per_channel:
             reshape_shape = get_threshold_reshape_shape(inputs.shape,
                                                         quant_axis=self.quantization_axis,
                                                         quant_axis_dim=-1)
 
             ##########################################################
             # Calculate soft rounding targets and optimized threshold
             ##########################################################
             ptq_threshold_tensor_hat = tf.reshape(ptq_threshold_tensor, reshape_shape)
-            aux_var = self.get_soft_targets()
-
-            #####################################################
-            # Soft Rounding
-            #####################################################
-            if training:
-                self.ar_iter.assign_add(1.0)
-            else:
-                aux_var = tf.cast(tf.math.greater_equal(aux_var, 0.5), tf.float32)
 
             #####################################################
             # Quantized Input
             #####################################################
             q_tensor = soft_rounding_symmetric_quantizer(input_tensor=inputs,
                                                          auxvar_tensor=aux_var,
                                                          threshold_tensor=ptq_threshold_tensor_hat,
                                                          num_bits=self.num_bits,
                                                          signed=True,
                                                          power_of_two=self.power_of_two)
 
             if self.quantization_parameter_learning and not self.power_of_two:
-                scale = tf.reshape(self.quantizer_parameters[SCALE_PTQ], reshape_shape)
+                scale = tf.reshape(self.get_quantizer_variable(SCALE_PTQ), reshape_shape)
                 q_tensor *= scale
 
-            return q_tensor
         else:
-            return soft_rounding_symmetric_quantizer(input_tensor=inputs,
-                                                     auxvar_tensor=self.quantizer_parameters[AUXVAR],
-                                                     threshold_tensor=ptq_threshold_tensor.value(),
-                                                     num_bits=self.num_bits,
-                                                     signed=True,
-                                                     power_of_two=self.power_of_two)
+            q_tensor = soft_rounding_symmetric_quantizer(input_tensor=inputs,
+                                                         auxvar_tensor=aux_var,
+                                                         threshold_tensor=ptq_threshold_tensor.value(),
+                                                         num_bits=self.num_bits,
+                                                         signed=True,
+                                                         power_of_two=self.power_of_two)
+
+            if self.quantization_parameter_learning and not self.power_of_two:
+                scale = self.get_quantizer_variable(SCALE_PTQ)
+                q_tensor *= scale
+
+        return q_tensor
 
     def get_quant_config(self) -> Dict[str, np.ndarray]:
         """
         Returns the config used to edit NodeQuantizationConfig after GPTQ retraining
 
         Returns:
             A dictionary of attributes the quantize_config retraining has changed during GPTQ retraining.
             Keys must match NodeQuantizationConfig attributes
         """
 
         if self.power_of_two:
-            old_threshold = self.quantizer_parameters[PTQ_THRESHOLD]
+            old_threshold = self.get_quantizer_variable(PTQ_THRESHOLD)
             old_threshold = max_power_of_two(old_threshold, MIN_THRESHOLD)
 
         else:
-            old_threshold = self.quantizer_parameters[PTQ_THRESHOLD]
+            old_threshold = self.get_quantizer_variable(PTQ_THRESHOLD)
             if self.quantization_parameter_learning:
-                scale = tf.reshape(self.quantizer_parameters[SCALE_PTQ], self.threshold_shape)
+                scale = tf.reshape(self.get_quantizer_variable(SCALE_PTQ), self.threshold_shape)
                 old_threshold = old_threshold * scale
             old_threshold = old_threshold.numpy()
         old_threshold = old_threshold.reshape(self.threshold_shape)
         return {THRESHOLD: old_threshold}
```

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/ptq/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/symmetric_ste.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/symmetric_ste.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,31 +9,32 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
-from typing import Dict, Any, List
+from typing import Dict, Any
 
 import numpy as np
 import tensorflow as tf
 
-from model_compression_toolkit import RoundingType
+from model_compression_toolkit.gptq import RoundingType
 from model_compression_toolkit import quantizers_infrastructure as qi
 from model_compression_toolkit.core.common.target_platform import QuantizationMethod
-from model_compression_toolkit.gptq.common.gptq_constants import GPTQ_ITER, AUXVAR, PTQ_THRESHOLD
+from model_compression_toolkit.gptq.common.gptq_constants import AUXVAR, PTQ_THRESHOLD
 from model_compression_toolkit.gptq.keras.quantizer import quant_utils as qutils
 from model_compression_toolkit.core.common.constants import THRESHOLD
 from model_compression_toolkit.core.common.defaultdict import DefaultDict
 from model_compression_toolkit.gptq.keras.quantizer.base_keras_gptq_quantizer import BaseKerasGPTQTrainableQuantizer
 from model_compression_toolkit.quantizers_infrastructure import TrainableQuantizerWeightsConfig
 from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.common.base_inferable_quantizer import mark_quantizer
 from model_compression_toolkit.quantizers_infrastructure.trainable_infrastructure.common.quant_utils import \
     get_threshold_reshape_shape
+from model_compression_toolkit.quantizers_infrastructure.trainable_infrastructure.common.base_trainable_quantizer import VariableGroup
 
 
 def pertubation_symmetric_quantizer(input_tensor: tf.Tensor,
                                     auxvar_tensor: tf.Variable,
                                     max_tensor: tf.Tensor,
                                     num_bits: int,
                                     signed: bool,
@@ -92,38 +93,28 @@
         self.threshold_shape = np.asarray(threshold_values).shape
         self.threshold_values = np.reshape(np.asarray(threshold_values), [-1]) if self.per_channel else float(
             threshold_values)
 
         self.quantization_axis = quantization_config.weights_channels_axis
         self.power_of_two = quantization_config.weights_quantization_method == QuantizationMethod.POWER_OF_TWO
         self.max_lsbs_change = max_lsbs_change_map.get(self.num_bits)
-        self.quantizer_parameters = {}
 
     def initialize_quantization(self,
                                 tensor_shape: Any,
                                 name: str,
-                                layer: Any) -> Dict[Any, Any]:
+                                layer: Any):
         """
-        Return a dictionary of quantizer parameters and their names.
+        Add quantizer parameters to the quantizer parameters dictionary
 
         Args:
             tensor_shape: tensor shape of the quantized tensor.
             name: Tensor name.
             layer: Layer to quantize.
-
-        Returns:
-            Dictionary of parameters names to the variables.
         """
 
-        ar_iter = layer.add_weight(
-            f"{name}_{GPTQ_ITER}",
-            shape=(),
-            initializer=tf.keras.initializers.Constant(0.0),
-            trainable=False)
-
         ptq_threshold_tensor = layer.add_weight(
             f"{name}_{PTQ_THRESHOLD}",
             shape=len(self.threshold_values) if self.per_channel else (),
             initializer=tf.keras.initializers.Constant(1.0),
             trainable=False)
         ptq_threshold_tensor.assign(self.threshold_values)
 
@@ -131,18 +122,16 @@
         auxvar_tensor = layer.add_weight(
             f"{name}_{AUXVAR}",
             shape=list(w.shape),
             initializer=tf.keras.initializers.Constant(0.0),
             trainable=True)
 
         # save the quantizer added parameters for later calculations
-        self.quantizer_parameters = {PTQ_THRESHOLD: ptq_threshold_tensor,
-                                     AUXVAR: auxvar_tensor,
-                                     GPTQ_ITER: ar_iter}
-        return self.quantizer_parameters
+        self.add_quantizer_variable(PTQ_THRESHOLD, ptq_threshold_tensor, VariableGroup.QPARAMS)
+        self.add_quantizer_variable(AUXVAR, auxvar_tensor, VariableGroup.WEIGHTS)
 
     def __call__(self,
                  inputs: tf.Tensor,
                  training: bool):
         """
         Quantize a tensor.
 
@@ -150,16 +139,16 @@
             inputs: Input tensor to quantize.
             training: Whether the graph is in training mode.
 
         Returns:
             The quantized tensor.
         """
 
-        auxvar = self.quantizer_parameters[AUXVAR]
-        ptq_threshold_tensor = self.quantizer_parameters[PTQ_THRESHOLD]
+        auxvar = self.get_quantizer_variable(AUXVAR)
+        ptq_threshold_tensor = self.get_quantizer_variable(PTQ_THRESHOLD)
 
         if self.per_channel:
             reshape_shape = get_threshold_reshape_shape(inputs.shape,
                                                         quant_axis=self.quantization_axis,
                                                         quant_axis_dim=-1)
             ptq_threshold_tensor = tf.reshape(ptq_threshold_tensor, reshape_shape)
             q_tensor = pertubation_symmetric_quantizer(inputs,
@@ -174,38 +163,19 @@
             return pertubation_symmetric_quantizer(inputs,
                                                    auxvar,
                                                    ptq_threshold_tensor,
                                                    self.num_bits,
                                                    signed=True,
                                                    power_of_two=self.power_of_two)
 
-    def get_aux_variable(self) -> List[tf.Tensor]:
-        """
-        This function return a list with the quantizer's quantization auxiliary variables.
-
-        Returns: A list with the quantization auxiliary variables.
-
-        """
-
-        return [self.quantizer_parameters[AUXVAR]]
-
-    def get_quantization_variable(self) -> List[tf.Tensor]:
-        """
-        This function return a list with the quantizer's quantization parameters variables.
-
-        Returns: A list with the quantization parameters.
-
-        """
-
-        return [self.quantizer_parameters[PTQ_THRESHOLD]]
 
     def get_quant_config(self) -> Dict[str, np.ndarray]:
         """
         Returns the config used to edit NodeQuantizationConfig after GPTQ retraining
 
         Returns:
             A dictionary of attributes the quantize_config retraining has changed during GPTQ retraining.
             Keys must match NodeQuantizationConfig attributes
 
         """
-        old_threshold = self.quantizer_parameters[PTQ_THRESHOLD]
+        old_threshold = self.get_quantizer_variable(PTQ_THRESHOLD)
         return {THRESHOLD: old_threshold.numpy().reshape(self.threshold_shape)}
```

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/gptq/pytorch/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/ptq/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/gptq/pytorch/gptq_loss.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/pytorch/gptq_loss.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/gptq/pytorch/gptq_training.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/pytorch/gptq_training.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,25 +19,25 @@
 from tqdm import tqdm
 import copy
 import torch
 from model_compression_toolkit.core.common.logger import Logger
 from model_compression_toolkit.core.pytorch.back2framework.pytorch_model_builder import PyTorchModelBuilder
 from model_compression_toolkit.gptq.common.gptq_graph import get_kernel_attribute_name_for_gptq
 from model_compression_toolkit.gptq.common.gptq_training import GPTQTrainer
-from model_compression_toolkit.gptq.common.gptq_config import GradientPTQConfigV2, RoundingType
+from model_compression_toolkit.gptq.common.gptq_config import GradientPTQConfigV2
 from model_compression_toolkit.core.common import Graph, BaseNode
 from model_compression_toolkit.core.common.framework_info import FrameworkInfo
 from model_compression_toolkit.core.common.framework_implementation import FrameworkImplementation
 from model_compression_toolkit.core.pytorch.constants import BIAS
 from model_compression_toolkit.core.pytorch.utils import to_torch_tensor, set_model, torch_tensor_to_numpy
 from model_compression_toolkit.gptq.pytorch.graph_info import get_gptq_trainable_parameters, \
-    get_weights_for_loss, get_soft_rounding_reg
+    get_weights_for_loss
 from model_compression_toolkit.gptq.pytorch.quantizer.quantization_builder import quantization_builder
-from model_compression_toolkit.gptq.common.gptq_constants import REGULARIZATION_VALUES
 from model_compression_toolkit import quantizers_infrastructure as qi
+from model_compression_toolkit.gptq.pytorch.quantizer.regularization_factory import get_regularization
 from model_compression_toolkit.quantizers_infrastructure import PytorchQuantizationWrapper
 
 
 class PytorchGPTQTrainer(GPTQTrainer):
     """
     Pytorch GPTQ training class for fine-tuning a quantized model
     """
@@ -59,38 +59,40 @@
             graph_float: Graph to build a float networks from.
             graph_quant: Graph to build a quantized networks from.
             gptq_config: GradientPTQConfigV2 with parameters about the tuning process.
             fw_impl: FrameworkImplementation object with a specific framework methods implementation.
             fw_info: Framework information
             representative_data_gen: Dataset to use for inputs of the models.
         """
-        super().__init__(graph_float, graph_quant, gptq_config, fw_impl, fw_info, representative_data_gen)
+        super().__init__(graph_float, graph_quant, gptq_config, fw_impl, fw_info)
         self.loss_list = []
         self.input_scale = 1
         if self.float_user_info.input_scale != self.gptq_user_info.input_scale:
             Logger.error("Input scale mismatch between float and GPTQ networks")  # pragma: no cover
         else:
             self.input_scale = self.gptq_user_info.input_scale
 
-        trainable_weights, trainable_bias, trainable_threshold, trainable_temperature = get_gptq_trainable_parameters(
+        trainable_weights, trainable_bias, trainable_threshold = get_gptq_trainable_parameters(
             self.fxp_model,
             add_bias=self.gptq_config.train_bias)
 
         self.flp_weights_list, self.fxp_weights_list = get_weights_for_loss(self.fxp_model)
         if not (len(self.compare_points) == len(trainable_weights) == len(self.flp_weights_list) == len(
                 self.fxp_weights_list)):
             Logger.error(
                 "GPTQ: Mismatch between number of compare points, number of layers with trainable weights " +
                 "and number of float and quantized weights for loss")
 
         self.optimizer_with_param = self.get_optimizer_with_param(trainable_weights,
                                                                   trainable_bias,
                                                                   trainable_threshold)
 
-        self.weights_for_average_loss = to_torch_tensor(self.compute_jacobian_based_weights(representative_data_gen))
+        self.weights_for_average_loss = to_torch_tensor(self.compute_hessian_based_weights(representative_data_gen))
+
+        self.reg_func = get_regularization(self.gptq_config, representative_data_gen)
 
     def _is_gptq_applicable(self,
                             node: BaseNode) -> bool:
         """
         A function for deciding if a layer should be fine-tuned during GPTQ.
         Args:
             node (BaseNode): Node for quantization decision
@@ -180,17 +182,15 @@
                                            y_float,
                                            self.fxp_weights_list,
                                            self.flp_weights_list,
                                            self.compare_points_mean,
                                            self.compare_points_std,
                                            self.weights_for_average_loss)
 
-        reg_value = self.gptq_config.quantizer_config.get_regularization_value(
-            self.fxp_model,
-            **{REGULARIZATION_VALUES: self._get_quantizer_regularization_values(self.gptq_config.rounding_type)})
+        reg_value = self.reg_func(self.fxp_model, self.gptq_config.regularization_factor)
 
         loss_value += reg_value
 
         # Back-pass
         loss_value.backward()
 
         # Get gradients
@@ -268,22 +268,7 @@
 
         # Fxp model: unfreeze bias trainable parameters
         for layer in self.fxp_model.modules():
             if isinstance(layer, PytorchQuantizationWrapper):
                 if hasattr(layer.layer, BIAS):
                     bias = getattr(layer.layer, BIAS)
                     bias.requires_grad = self.gptq_config.train_bias
-
-    def _get_quantizer_regularization_values(self, rounding_type: RoundingType) -> List[torch.Tensor]:
-        """
-        Mapping between a rounding type to its matching regularization method.
-
-        Args:
-            rounding_type: GPTQ rounding type.
-
-        Returns: A regularization computation method.
-
-        """
-        if rounding_type == RoundingType.SoftQuantizer:
-            return get_soft_rounding_reg(self.fxp_model)
-        else:
-            return []
```

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/gptq/pytorch/quantization_facade.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/pytorch/quantization_facade.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,22 +13,23 @@
 # limitations under the License.
 # ==============================================================================
 from typing import Callable
 from model_compression_toolkit.core import common
 from model_compression_toolkit.core.common.constants import FOUND_TORCH
 from model_compression_toolkit.core.common import Logger
 from model_compression_toolkit.core.common.constants import PYTORCH
-from model_compression_toolkit.gptq.common.gptq_config import GradientPTQConfigV2, RoundingType
+from model_compression_toolkit.gptq.common.gptq_config import GradientPTQConfigV2
 from model_compression_toolkit.core.common.target_platform import TargetPlatformCapabilities
 from model_compression_toolkit.core.common.mixed_precision.kpi_tools.kpi import KPI
 from model_compression_toolkit.core.runner import core_runner, _init_tensorboard_writer
+from model_compression_toolkit.gptq.keras.quantization_facade import GPTQ_MOMENTUM
 from model_compression_toolkit.gptq.runner import gptq_runner
 from model_compression_toolkit.core.exporter import export_model
 from model_compression_toolkit.core.analyzer import analyzer_model_quantization
-from model_compression_toolkit import CoreConfig, GPTQQuantizerConfig
+from model_compression_toolkit import CoreConfig
 from model_compression_toolkit.core.common.mixed_precision.mixed_precision_quantization_config import \
     MixedPrecisionQuantizationConfigV2
 
 LR_DEFAULT = 1e-4
 LR_REST_DEFAULT = 1e-4
 LR_BIAS_DEFAULT = 1e-4
 LR_QUANTIZATION_PARAM_DEFAULT = 1e-4
@@ -67,41 +68,27 @@
             a GradientPTQConfigV2 object to use when fine-tuning the quantized model using gptq.
 
         Examples:
 
             Import MCT and Create a GradientPTQConfigV2 to run for 5 epochs:
 
             >>> import model_compression_toolkit as mct
-            >>> gptq_conf = mct.get_pytorch_gptq_config(n_epochs=5)
+            >>> gptq_conf = mct.gptq.get_pytorch_gptq_config(n_epochs=5)
 
             Other PyTorch optimizers can be passed with dummy params:
 
             >>> import torch
-            >>> gptq_conf = mct.get_pytorch_gptq_config(n_epochs=3, optimizer=torch.optim.Adam([torch.Tensor(1)]))
+            >>> gptq_conf = mct.gptq.get_pytorch_gptq_config(n_epochs=3, optimizer=torch.optim.Adam([torch.Tensor(1)]))
 
             The configuration can be passed to :func:`~model_compression_toolkit.pytorch_post_training_quantization` in order to quantize a pytorch model using gptq.
 
         """
-        bias_optimizer = Adam([torch.Tensor([])], lr=LR_BIAS_DEFAULT)
-        optimizer_quantization_parameter = Adam([torch.Tensor([])], lr=LR_QUANTIZATION_PARAM_DEFAULT)
-        # TODO: Once implementing Soft Quantizer for GPTQ in Pytorch:
-        #  - change default quantization_parameters_learning to True.
-        #  - remove explicit rounding_type and quantizer_config (and let it use the default GradientPTQConfig).
-        return GradientPTQConfigV2(n_epochs,
-                                   optimizer,
-                                   optimizer_rest=optimizer_rest,
-                                   loss=loss,
-                                   log_function=log_function,
-                                   train_bias=True,
-                                   optimizer_quantization_parameter=optimizer_quantization_parameter,
-                                   optimizer_bias=bias_optimizer,
-                                   rounding_type=RoundingType.STE,
-                                   quantizer_config=GPTQQuantizerConfig(),
-                                   quantization_parameters_learning=False,
-                                   )
+        bias_optimizer = torch.optim.SGD([torch.Tensor([])], lr=LR_BIAS_DEFAULT, momentum=GPTQ_MOMENTUM)
+        return GradientPTQConfigV2(n_epochs, optimizer, optimizer_rest=optimizer_rest, loss=loss,
+                                   log_function=log_function, train_bias=True, optimizer_bias=bias_optimizer)
 
 
     def pytorch_gradient_post_training_quantization_experimental(model: Module,
                                                                  representative_data_gen: Callable,
                                                                  target_kpi: KPI = None,
                                                                  core_config: CoreConfig = CoreConfig(),
                                                                  gptq_config: GradientPTQConfigV2 = None,
@@ -155,15 +142,15 @@
 
             Create MCT core configurations with number of calibration iterations set to 1:
 
             >>> config = mct.CoreConfig()
 
             Pass the module, the representative dataset generator and the configuration (optional) to get a quantized module
 
-            >>> quantized_module, quantization_info = mct.pytorch_gradient_post_training_quantization_experimental(module, repr_datagen, core_config=config, gptq_config=gptq_conf)
+            >>> quantized_module, quantization_info = mct.gptq.pytorch_gradient_post_training_quantization_experimental(module, repr_datagen, core_config=config, gptq_config=gptq_conf)
 
         """
 
         if core_config.mixed_precision_enable:
             if not isinstance(core_config.mixed_precision_config, MixedPrecisionQuantizationConfigV2):
                 common.Logger.error("Given quantization config to mixed-precision facade is not of type "
                                     "MixedPrecisionQuantizationConfigV2. Please use keras_post_training_quantization "
```

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/gptq/pytorch/quantizer/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/pytorch/quantizer/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,7 +11,8 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
 import model_compression_toolkit.gptq.pytorch.quantizer.ste_rounding.symmetric_ste
 import model_compression_toolkit.gptq.pytorch.quantizer.soft_rounding.symmetric_soft_quantizer
+import model_compression_toolkit.gptq.pytorch.quantizer.soft_rounding.uniform_soft_quantizer
```

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/gptq/pytorch/quantizer/base_pytorch_gptq_quantizer.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/keras/base_keras_quantizer.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,112 +1,90 @@
-# Copyright 2023 Sony Semiconductor Israel, Inc. All rights reserved.
+# Copyright 2022 Sony Semiconductor Israel, Inc. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-from abc import abstractmethod
-from typing import Union, Dict, List
-
-from model_compression_toolkit.core.common.logger import Logger
-from model_compression_toolkit.core.common.constants import FOUND_TORCH
-from model_compression_toolkit.gptq.common.gptq_constants import WEIGHTS_QUANTIZATION_PARAMS
+from typing import Dict, Any, Union, List
 
+from model_compression_toolkit.core.common import Logger
+from model_compression_toolkit.core.common.constants import FOUND_TF
+from model_compression_toolkit.quantizers_infrastructure.trainable_infrastructure.common.base_trainable_quantizer import VariableGroup
+from model_compression_toolkit.quantizers_infrastructure.trainable_infrastructure.common.base_trainable_quantizer import BaseTrainableQuantizer, VAR, GROUP
 from model_compression_toolkit.quantizers_infrastructure import TrainableQuantizerWeightsConfig, \
     TrainableQuantizerActivationConfig
-from model_compression_toolkit.quantizers_infrastructure.trainable_infrastructure.common.base_trainable_quantizer import \
-    BaseTrainableQuantizer
-from model_compression_toolkit.quantizers_infrastructure.trainable_infrastructure.pytorch.base_pytorch_quantizer import \
-    BasePytorchTrainableQuantizer
-
-if FOUND_TORCH:
-    from torch import Tensor
-    from model_compression_toolkit.quantizers_infrastructure import PytorchQuantizationWrapper
-
-    class BasePytorchGPTQTrainableQuantizer(BasePytorchTrainableQuantizer):
-        """
-        A base class for trainable Pytorch quantizer for GPTQ.
-        """
 
+if FOUND_TF:
+    QUANTIZATION_CONFIG = 'quantization_config'
+    from model_compression_toolkit.quantizers_infrastructure.trainable_infrastructure.keras.config_serialization import config_serialization, \
+        config_deserialization
+    import tensorflow as tf
+
+    class BaseKerasTrainableQuantizer(BaseTrainableQuantizer):
         def __init__(self,
                      quantization_config: Union[TrainableQuantizerWeightsConfig, TrainableQuantizerActivationConfig]):
             """
-            Initializes BasePytorchGPTQTrainableQuantizer object.
-
+            This class is a base quantizer which validates provided quantization config and defines an abstract function which any quantizer needs to implement.
+            This class adds to the base quantizer a get_config and from_config functions to enable loading and saving the keras model.
             Args:
                 quantization_config: quantizer config class contains all the information about a quantizer configuration.
             """
-
             super().__init__(quantization_config)
 
-        def update_layer_quantization_params(self, layer: PytorchQuantizationWrapper
-                                             ) -> (Dict[str, Tensor], Dict[str, Dict], Dict):
+        def get_config(self) -> Dict[str, Any]:
             """
-            A Function to calculate the needed change in attributes in NodeQuantizationConfig after retraining.
 
-            Args:
-                layer: A wrapped Pytorch layer.
-
-            Returns:
-                3 dictionaries describing the change in layer's weights, weights config, activation config
-                that changed during GPTQ retraining.
-                Keys must match NodeQuantizationConfig attributes
+            Returns: Configuration of BaseKerasQuantizer.
 
             """
-            weights = {}
-            for weight, quantizer_vars, quantizer in layer.get_weights_vars():
-                if not isinstance(quantizer, BaseTrainableQuantizer):
-                    Logger.error(f"Expecting a GPTQ trainable quantizer, "  # pragma: no cover
-                                 f"but got {type(quantizer)} which is not callable.")
-                weights.update({weight: quantizer(training=False, inputs=quantizer_vars)})
-
-            quant_config = {WEIGHTS_QUANTIZATION_PARAMS: self.get_quant_config()}
-
-            return weights, quant_config, {}
+            return {QUANTIZATION_CONFIG: config_serialization(self.quantization_config)}
 
-        def get_aux_variable(self) -> List[Tensor]:
+        @classmethod
+        def from_config(cls, config: dict):
             """
-            This function return a list with the quantizer's quantization auxiliary variables.
 
-            Returns: A list with the quantization auxiliary variables.
-
-            """
+            Args:
+                config(dict): dictonory  of  BaseKerasQuantizer Configuration
 
-            return []  # pragma: no cover
+            Returns: A BaseKerasQuantizer
 
-        def get_quantization_variable(self) -> List[Tensor]:
             """
-            This function return a list with the quantizer's quantization parameters variables.
-
-            Returns: A list with the quantization parameters.
+            config = config.copy()
+            quantization_config = config_deserialization(config[QUANTIZATION_CONFIG])
+            # Note that a quantizer only receive quantization config and the rest of define hardcoded inside the speficie quantizer.
+            return cls(quantization_config=quantization_config)
 
+        def get_trainable_variables(self, group: VariableGroup) -> List[tf.Tensor]:
             """
+            Get trainable parameters with specific group from quantizer
 
-            return []  # pragma: no cover
-
-        @abstractmethod
-        def get_quant_config(self):
-            """
-            Returns the config used to edit NodeQuantizationConfig after GPTQ retraining.
+            Args:
+                group: Enum of variable group
 
             Returns:
-                A dictionary of attributes the quantize_config retraining has changed during GPTQ retraining.
-                Keys must match NodeQuantizationConfig attributes.
-
+                List of trainable variables
             """
-            raise NotImplemented(f'{self.__class__.__name__} have to implement the '  # pragma: no cover
-                                 f'quantizer\'s get_quant_config.')
+            quantizer_trainable = []
+            for name, parameter_dict in self.quantizer_parameters.items():
+                quantizer_parameter, parameter_group = parameter_dict[VAR], parameter_dict[GROUP]
+                if quantizer_parameter.trainable and parameter_group == group:
+                    quantizer_trainable.append(quantizer_parameter)
+            return quantizer_trainable
+
 
 else:
-    class BasePytorchGPTQTrainableQuantizer:  # pragma: no cover
-        def __init__(self, *args, **kwargs):
-            Logger.critical('Installing Pytorch is mandatory '
-                            'when using BasePytorchGPTQTrainableQuantizer. '
-                            'Could not find torch package.')  # pragma: no cover
+    class BaseKerasTrainableQuantizer(BaseTrainableQuantizer):
+        def __init__(self,
+                     quantization_config: Union[TrainableQuantizerWeightsConfig, TrainableQuantizerActivationConfig]):
+
+            super().__init__(quantization_config)
+            Logger.critical('Installing tensorflow and tensorflow_model_optimization is mandatory '
+                            'when using BaseKerasQuantizer. '
+                            'Could not find Tensorflow package.')  # pragma: no cover
```

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/gptq/pytorch/quantizer/quant_utils.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/pytorch/quantizer/quant_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,19 +26,28 @@
     return torch.pow(2, ste_ceil(torch.log2(torch.clip(max_tensor, min=MIN_THRESHOLD, max=torch.inf))))
 
 
 def calculate_delta(max_tensor: torch.Tensor,
                     num_bits: int,
                     signed: bool) -> torch.Tensor:
     """
-    Compute the step size for the quantization.
+    Compute the step size for the symmetric quantization.
     """
     return max_tensor / (2 ** (num_bits - int(signed)))
 
 
+def calculate_delta_uniform(min_tensor: torch.Tensor,
+                            max_tensor: torch.Tensor,
+                            num_bits: int) -> torch.Tensor:
+    """
+    Compute the step size for the uniform quantization.
+    """
+    return (max_tensor-min_tensor) / (2 ** num_bits - 1)
+
+
 def ste_ceil(x: torch.Tensor) -> torch.Tensor:
     """
     Return the ceil values of a tensor.
     """
     return (torch.ceil(x) - x).detach() + x
```

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/gptq/pytorch/quantizer/quantization_builder.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/pytorch/quantizer/quantization_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from typing import List, Dict, Tuple
 
-from model_compression_toolkit import GradientPTQConfigV2
+from model_compression_toolkit.gptq import GradientPTQConfigV2
 from model_compression_toolkit.core import common
 from model_compression_toolkit.core.pytorch.constants import KERNEL
 from model_compression_toolkit.exporter.model_wrapper.pytorch.builder.node_to_quantizer import \
     get_activation_inferable_quantizer_kwargs
 from model_compression_toolkit.gptq.pytorch.quantizer.base_pytorch_gptq_quantizer import \
     BasePytorchGPTQTrainableQuantizer
 from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.common.get_quantizers import \
@@ -55,15 +55,15 @@
     if n.is_weights_quantization_enabled():
         quant_method = n.final_weights_quantization_cfg.weights_quantization_method
         quantizer_class = get_trainable_quantizer_class(quant_target=QuantizationTarget.Weights,
                                                         quantizer_type=gptq_config.rounding_type,
                                                         quant_method=quant_method,
                                                         quantizer_base_class=BasePytorchGPTQTrainableQuantizer)
         weights_quantizers.update({KERNEL: quantizer_class(get_trainable_quantizer_weights_config(n),
-                                                           **gptq_config.get_extended_quantizer_parametes())})
+                                                           **gptq_config.gptq_quantizer_params_override)})
     activation_quantizers = []
     if n.is_activation_quantization_enabled():
         quant_method = n.final_activation_quantization_cfg.activation_quantization_method
 
         quantizer_class = get_inferable_quantizer_class(quant_target=QuantizationTarget.Activation,
                                                         quant_method=quant_method,
                                                         quantizer_base_class=BasePyTorchInferableQuantizer)
```

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/symmetric_soft_quantizer.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/symmetric_soft_quantizer.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,32 +10,33 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 import torch
 import torch.nn as nn
-from typing import List, Dict
+from typing import Dict
 import numpy as np
 
-from model_compression_toolkit.core.common import Logger, max_power_of_two
+from model_compression_toolkit.core.common import max_power_of_two
 from model_compression_toolkit import quantizers_infrastructure as qi
 from model_compression_toolkit.core.common.target_platform import QuantizationMethod
 from model_compression_toolkit.gptq.common.gptq_config import RoundingType
 from model_compression_toolkit.gptq.pytorch.quantizer.base_pytorch_gptq_quantizer import \
     BasePytorchGPTQTrainableQuantizer
 from model_compression_toolkit.core.pytorch.utils import to_torch_tensor, torch_tensor_to_numpy
 from model_compression_toolkit.gptq.pytorch.quantizer import quant_utils as qutils
-from model_compression_toolkit.gptq.common.gptq_constants import PTQ_THRESHOLD, SCALE_PTQ, N_EPOCHS, \
-    MAX_ITERATIONS_DEFAULT, SOFT_ROUNDING_GAMMA, SOFT_ROUNDING_ZETA, SOFT_ROUNDING_BETA, GPTQ_ITER, AUXVAR
+from model_compression_toolkit.gptq.common.gptq_constants import PTQ_THRESHOLD, SCALE_PTQ, \
+    SOFT_ROUNDING_GAMMA, SOFT_ROUNDING_ZETA, AUXVAR
 from model_compression_toolkit.core.common.constants import THRESHOLD, MIN_THRESHOLD
 from model_compression_toolkit.quantizers_infrastructure import TrainableQuantizerWeightsConfig
 from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.common.base_inferable_quantizer import mark_quantizer
 from model_compression_toolkit.quantizers_infrastructure.trainable_infrastructure.common.quant_utils import \
     get_threshold_reshape_shape
+from model_compression_toolkit.quantizers_infrastructure.trainable_infrastructure.common.base_trainable_quantizer import VariableGroup
 
 
 def soft_rounding_symmetric_quantizer(input_tensor: torch.Tensor,
                                       auxvar_tensor: torch.Tensor,
                                       threshold_tensor: torch.Tensor,
                                       num_bits: int,
                                       signed: bool,
@@ -63,123 +64,65 @@
     tensor_q = input_tensor_int + auxvar_tensor
     int_threshold = 2 ** (num_bits - int(signed))
     return delta * qutils.ste_clip(tensor_q,
                                    min_val=-int(signed) * int_threshold,
                                    max_val=int_threshold - 1)
 
 
-class LinearTempDecay:
-    """
-    Annealing process for the soft quantizer regularization temperature term.
-    """
-
-    def __init__(self, t_max: int, rel_start_decay: float = 0.2, start_b: int = 20, end_b: int = 2):
-        """
-        Initializes a LinearTempDecay object.
-
-        Args:
-            t_max: maximal time step.
-            rel_start_decay: Decay step size at the beginning of the process.
-            start_b: Starting value of the regularization term.
-            end_b: Target value of the regularization term.
-        """
-
-        self.t_max = t_max
-        self.start_decay = rel_start_decay * t_max
-        self.start_b = start_b
-        self.end_b = end_b
-
-    def __call__(self, t: nn.Parameter) -> float:
-        """
-        Cosine annealing scheduler for soft quantizer regularization temperature term.
-
-        Args:
-            t: The current time step.
-
-        Returns: Scheduled temperature.
-        """
-
-        is_before_start_decay = (t < self.start_decay).to(torch.float32)
-
-        rel_t = (t - self.start_decay) / (self.t_max - self.start_decay)
-
-        return self.start_b * is_before_start_decay + \
-               (1 - is_before_start_decay) * \
-               (self.end_b + (self.start_b - self.end_b) * torch.maximum(to_torch_tensor(np.array([0.0])), (1 - rel_t)))
-
-
 @mark_quantizer(quantization_target=qi.QuantizationTarget.Weights,
                 quantization_method=[QuantizationMethod.POWER_OF_TWO, QuantizationMethod.SYMMETRIC],
                 quantizer_type=RoundingType.SoftQuantizer)
 class SymmetricSoftRoundingGPTQ(BasePytorchGPTQTrainableQuantizer):
     """
     Trainable symmetric quantizer to optimize the rounding of the quantized values using a soft quantization method.
     """
 
     def __init__(self,
                  quantization_config: TrainableQuantizerWeightsConfig,
-                 n_batches: int = None,
-                 quantization_parameter_learning: bool = False,
-                 n_epochs: int = N_EPOCHS):
+                 quantization_parameter_learning: bool = False):
         """
         Construct a Pytorch model that utilize a fake weight quantizer of soft-quantizer for symmetric quantizer.
 
         Args:
             quantization_config: Trainable weights quantizer config.
-            n_batches (int): number of batches in representative dataset
             quantization_parameter_learning (Bool): Whether to learn the threshold or not
-            n_epochs (int): number of epochs the representative dataset is run during fine-tuning
         """
 
-        if n_batches is None:
-            Logger.error("SymmetricSoftRoundingGPTQ got an uninitialized n_batches argument.")
-
         super().__init__(quantization_config)
         self.num_bits = quantization_config.weights_n_bits
         self.per_channel = quantization_config.weights_per_channel_threshold
 
         threshold_values = quantization_config.weights_quantization_params[THRESHOLD]
         self.threshold_shape = np.asarray(threshold_values).shape
         self.threshold_values = np.reshape(np.asarray(threshold_values), [-1]) if self.per_channel else float(
             threshold_values)
 
         self.quantization_axis = quantization_config.weights_channels_axis
         self.power_of_two = quantization_config.weights_quantization_method == QuantizationMethod.POWER_OF_TWO
         self.quantization_parameter_learning = quantization_parameter_learning
 
         # gamma and zeta are stretch parameters for computing the rectified sigmoind function.
-        # beta is used to set the regularization term.
         # See: https://arxiv.org/pdf/2004.10568.pdf
         self.gamma = SOFT_ROUNDING_GAMMA
         self.zeta = SOFT_ROUNDING_ZETA
-        self.beta = SOFT_ROUNDING_BETA
 
         self.quantizer_parameters = {}
 
-        # Initializing the temperature decay according to the number of expected gradient steps
-        num_iterations = MAX_ITERATIONS_DEFAULT if n_batches is None else n_epochs * n_batches
-        self.linear_decay = LinearTempDecay(num_iterations)
-
     def initialize_quantization(self,
                                 tensor_shape: torch.Size,
                                 name: str,
-                                layer: qi.PytorchQuantizationWrapper) -> Dict[str, nn.Parameter]:
+                                layer: qi.PytorchQuantizationWrapper):
         """
-        Return a dictionary of quantizer parameters and their names.
+        Add quantizer parameters to the quantizer parameters dictionary
 
         Args:
             tensor_shape: tensor shape of the quantized tensor.
             name: Tensor name.
             layer: Layer to quantize.
-
-        Returns:
-            Dictionary of parameters names to the variables.
         """
-        layer.register_parameter(f"{name}_{GPTQ_ITER}",
-                                 nn.Parameter(to_torch_tensor(np.array([0])), requires_grad=False))
 
         if self.per_channel:
             threshold_tensor = to_torch_tensor(self.threshold_values)
         else:
             threshold_tensor = torch.tensor(self.threshold_values)
         layer.register_parameter(f"{name}_{PTQ_THRESHOLD}",
                                  nn.Parameter(threshold_tensor, requires_grad=False))
@@ -191,85 +134,54 @@
         # Note that (rest - self.gamma) can't be zero since rest is positive and gamma is negative, so the division
         # is safe
         alpha = -torch.log((self.zeta - self.gamma) / (rest - self.gamma) - 1)  # => sigmoid(alpha) = rest
 
         layer.register_parameter(f"{name}_{AUXVAR}", nn.Parameter(alpha, requires_grad=True))
 
         # save the quantizer added parameters for later calculations
-        self.quantizer_parameters = {PTQ_THRESHOLD: layer.get_parameter(f"{name}_{PTQ_THRESHOLD}"),
-                                     AUXVAR: layer.get_parameter(f"{name}_{AUXVAR}"),
-                                     GPTQ_ITER: layer.get_parameter(f"{name}_{GPTQ_ITER}")}
+        self.add_quantizer_variable(PTQ_THRESHOLD, layer.get_parameter(f"{name}_{PTQ_THRESHOLD}"), VariableGroup.QPARAMS)
+        self.add_quantizer_variable(AUXVAR, layer.get_parameter(f"{name}_{AUXVAR}"), VariableGroup.WEIGHTS)
 
         if self.quantization_parameter_learning:
-            layer.register_parameter(f"{name}_{SCALE_PTQ}",
-                                     nn.Parameter(torch.ones_like(torch.Tensor(self.threshold_values)),
-                                                  requires_grad=True))
-
-            self.quantizer_parameters.update({SCALE_PTQ: layer.get_parameter(f"{name}_{SCALE_PTQ}")})
-
-        return self.quantizer_parameters
-
-    def get_regularization(self) -> torch.Tensor:
-        """
-        Computes the regularization term for the soft rounding loss.
-
-        Returns:
-            regularization term.
-        """
-
-        st = self.get_soft_targets()
-        ar_iter = self.quantizer_parameters[GPTQ_ITER]
-        b = self.linear_decay(ar_iter)
-        return (1 - torch.pow(torch.abs(st - .5) * 2, b)).sum()
+            if self.per_channel:
+                layer.register_parameter(f"{name}_{SCALE_PTQ}",
+                                         nn.Parameter(to_torch_tensor(torch.ones_like(torch.Tensor(self.threshold_values))),
+                                                      requires_grad=True))
+            else:
+                layer.register_parameter(f"{name}_{SCALE_PTQ}",
+                                         nn.Parameter(to_torch_tensor((torch.tensor([1.0], requires_grad=True)))))
+            self.add_quantizer_variable(SCALE_PTQ, layer.get_parameter(f"{name}_{SCALE_PTQ}"), VariableGroup.QPARAMS)
 
     def get_soft_targets(self) -> torch.Tensor:
         """
         Computes the rectified sigmoid function for the quantization target parameters.
 
         Returns:
             A tensor with the soft rounding targets values.
 
         """
-        scaled_sigmoid = torch.sigmoid(self.quantizer_parameters[AUXVAR]) * (self.zeta - self.gamma) + self.gamma
+        scaled_sigmoid = torch.sigmoid(self.get_quantizer_variable(AUXVAR)) * (self.zeta - self.gamma) + self.gamma
         return torch.clip(scaled_sigmoid, min=0, max=1)
 
-    def get_aux_variable(self) -> List[torch.Tensor]:
-        """
-        This function return a list with the quantizer's quantization auxiliary variables.
-
-        Returns: A list with the quantization auxiliary variables.
-        """
-        return [self.quantizer_parameters.get(AUXVAR)]
-
-    def get_quantization_variable(self) -> List[torch.Tensor]:
-        """
-        This function return a list with the quantizer's quantization parameters variables.
-
-        Returns: A list with the quantization parameters.
-        """
-        if self.quantization_parameter_learning and not self.power_of_two:
-            return [self.quantizer_parameters[SCALE_PTQ]]
-        else:
-            return []
-
     def get_quant_config(self) -> Dict[str, np.ndarray]:
         """
         Returns the config used to edit NodeQuantizationConfig after GPTQ retraining
 
         Returns:
             A dictionary of attributes the quantize_config retraining has changed during GPTQ retraining.
             Keys must match NodeQuantizationConfig attributes
 
         """
-        old_threshold = torch_tensor_to_numpy(self.quantizer_parameters[PTQ_THRESHOLD])
+        old_threshold = torch_tensor_to_numpy(self.get_quantizer_variable(PTQ_THRESHOLD))
+        old_threshold = np.resize(old_threshold, self.threshold_shape)
         if self.power_of_two:
             old_threshold = max_power_of_two(old_threshold, MIN_THRESHOLD)
         else:
             if self.quantization_parameter_learning:
-                scale = torch.reshape(self.quantizer_parameters[SCALE_PTQ], self.threshold_shape)
+                scale = torch.reshape(self.get_quantizer_variable(SCALE_PTQ), self.threshold_shape)
                 old_threshold = old_threshold * torch_tensor_to_numpy(scale)
         old_threshold = old_threshold.reshape(self.threshold_shape)
         return {THRESHOLD: old_threshold}
 
     def __call__(self,
                  inputs: nn.Parameter,
                  training: bool) -> torch.Tensor:
@@ -279,25 +191,22 @@
         Args:
             inputs: Input tensor to quantize.
             training: whether in training mode or not
 
         Returns:
             quantized tensor
         """
-        ar_iter = self.quantizer_parameters[GPTQ_ITER]
-        auxvar = self.quantizer_parameters[AUXVAR]
-        ptq_threshold_tensor = self.quantizer_parameters[PTQ_THRESHOLD]
+        auxvar = self.get_quantizer_variable(AUXVAR)
+        ptq_threshold_tensor = self.get_quantizer_variable(PTQ_THRESHOLD)
 
         #####################################################
         # Soft Rounding
         #####################################################
         aux_var = self.get_soft_targets()
-        if training:
-            ar_iter.set_(ar_iter + 1)
-        else:
+        if not training:
             aux_var = (aux_var >= 0.5).to(auxvar.dtype)
 
         if self.per_channel:
             reshape_shape = get_threshold_reshape_shape(inputs.shape,
                                                         quant_axis=self.quantization_axis,
                                                         quant_axis_dim=-1)
 
@@ -313,19 +222,23 @@
                                                          auxvar_tensor=aux_var,
                                                          threshold_tensor=ptq_threshold_tensor_hat,
                                                          num_bits=self.num_bits,
                                                          signed=True,
                                                          power_of_two=self.power_of_two)
 
             if self.quantization_parameter_learning and not self.power_of_two:
-                scale = torch.reshape(self.quantizer_parameters[SCALE_PTQ], reshape_shape)
+                scale = torch.reshape(self.get_quantizer_variable(SCALE_PTQ), reshape_shape)
                 q_tensor *= scale
 
         else:
             q_tensor = soft_rounding_symmetric_quantizer(input_tensor=inputs,
                                                          auxvar_tensor=aux_var,
                                                          threshold_tensor=ptq_threshold_tensor,
                                                          num_bits=self.num_bits,
                                                          signed=True,
                                                          power_of_two=self.power_of_two)
 
+            if self.quantization_parameter_learning and not self.power_of_two:
+                scale = self.get_quantizer_variable(SCALE_PTQ)
+                q_tensor *= scale
+
         return q_tensor
```

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/symmetric_ste.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/symmetric_ste.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 import torch
 import torch.nn as nn
-from typing import List, Dict
+from typing import Dict
 import numpy as np
 from model_compression_toolkit.core.common.defaultdict import DefaultDict
 
 from model_compression_toolkit import quantizers_infrastructure as qi
 from model_compression_toolkit.core.common.target_platform import QuantizationMethod
 from model_compression_toolkit.gptq.common.gptq_config import RoundingType
 from model_compression_toolkit.gptq.pytorch.quantizer.base_pytorch_gptq_quantizer import \
@@ -26,15 +26,15 @@
 from model_compression_toolkit.core.pytorch.utils import to_torch_tensor, torch_tensor_to_numpy
 from model_compression_toolkit.gptq.pytorch.quantizer import quant_utils as qutils
 from model_compression_toolkit.gptq.common.gptq_constants import AUXVAR, PTQ_THRESHOLD, MAX_LSB_CHANGE
 from model_compression_toolkit.core.common.constants import THRESHOLD
 from model_compression_toolkit.quantizers_infrastructure import TrainableQuantizerWeightsConfig
 from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.common.base_inferable_quantizer import \
     mark_quantizer
-
+from model_compression_toolkit.quantizers_infrastructure.trainable_infrastructure.common.base_trainable_quantizer import VariableGroup
 from model_compression_toolkit.quantizers_infrastructure.trainable_infrastructure.common.quant_utils import \
     get_threshold_reshape_shape
 
 
 def pertubation_symmetric_quantizer(input_tensor: torch.Tensor,
                                     auxvar_tensor: nn.Parameter,
                                     max_tensor: torch.Tensor,
@@ -100,73 +100,51 @@
         self.threshold_shape = np.asarray(threshold_values).shape
         self.threshold_values = np.reshape(np.asarray(threshold_values), [-1]) if self.per_channel else float(
             threshold_values)
 
         self.quantization_axis = quantization_config.weights_channels_axis
         self.power_of_two = quantization_config.weights_quantization_method == QuantizationMethod.POWER_OF_TWO
         self.max_lsbs_change = max_lsbs_change_map.get(self.num_bits)
-        self.quantizer_parameters = {}
 
 
     def initialize_quantization(self,
                                 tensor_shape: torch.Size,
                                 name: str,
-                                layer: qi.PytorchQuantizationWrapper) -> Dict[str, nn.Parameter]:
+                                layer: qi.PytorchQuantizationWrapper):
         """
-        Return a dictionary of quantizer parameters and their names.
+        Add quantizer parameters to the quantizer parameters dictionary
 
         Args:
             tensor_shape: tensor shape of the quantized tensor.
             name: Tensor name.
             layer: Layer to quantize.
-
-        Returns:
-            Dictionary of parameters names to the variables.
         """
 
         layer.register_parameter(f"{name}_{PTQ_THRESHOLD}",
                                  nn.Parameter(torch.tensor(self.threshold_values, requires_grad=False)
                                               if not self.per_channel
                                               else to_torch_tensor(self.threshold_values),requires_grad=False))
         layer.register_parameter(f"{name}_{AUXVAR}", nn.Parameter(to_torch_tensor(torch.zeros(self.threshold_shape)),
                                                                   requires_grad=True))
 
         # save the quantizer added parameters for later calculations
-        self.quantizer_parameters = {PTQ_THRESHOLD: layer.get_parameter(f"{name}_{PTQ_THRESHOLD}"),
-                                     AUXVAR: layer.get_parameter(f"{name}_{AUXVAR}")}
-
-        return self.quantizer_parameters
-
-
-    def get_aux_variable(self) -> List[torch.Tensor]:
-        """
-        This function return a list with the quantizer's quantization auxiliary variables.
-
-        Returns: A list with the quantization auxiliary variables.
-        """
-        return [self.quantizer_parameters.get(AUXVAR)]
+        self.add_quantizer_variable(PTQ_THRESHOLD, layer.get_parameter(f"{name}_{PTQ_THRESHOLD}"), VariableGroup.QPARAMS)
+        self.add_quantizer_variable(AUXVAR, layer.get_parameter(f"{name}_{AUXVAR}"), VariableGroup.WEIGHTS)
 
-    def get_quantization_variable(self) -> List[torch.Tensor]:
-        """
-        This function return a list with the quantizer's quantization parameters variables.
-
-        Returns: A list with the quantization parameters.
-        """
-        return [self.quantizer_parameters.get(PTQ_THRESHOLD)]
 
     def get_quant_config(self) -> Dict[str, np.ndarray]:
         """
         Returns the config used to edit NodeQuantizationConfig after GPTQ retraining
 
         Returns:
             A dictionary of attributes the quantize_config retraining has changed during GPTQ retraining.
             Keys must match NodeQuantizationConfig attributes
 
         """
-        old_threshold = self.quantizer_parameters[PTQ_THRESHOLD]
+        old_threshold = self.get_quantizer_variable(PTQ_THRESHOLD)
         return {THRESHOLD: torch_tensor_to_numpy(old_threshold).reshape(self.threshold_shape)}
 
     def __call__(self,
                  inputs: nn.Parameter,
                  training: bool) -> nn.Parameter:
         """
         Quantize a tensor.
@@ -174,16 +152,16 @@
         Args:
             inputs: Input tensor to quantize.
             training: whether in training mode or not
 
         Returns:
             quantized tensor
         """
-        auxvar = self.quantizer_parameters[AUXVAR]
-        ptq_threshold_tensor = self.quantizer_parameters[PTQ_THRESHOLD]
+        auxvar = self.get_quantizer_variable(AUXVAR)
+        ptq_threshold_tensor = self.get_quantizer_variable(PTQ_THRESHOLD)
 
         if self.per_channel:
             reshape_shape = get_threshold_reshape_shape(inputs.shape,
                                                         quant_axis=self.quantization_axis,
                                                         quant_axis_dim=-1)
             ptq_threshold_tensor = torch.reshape(ptq_threshold_tensor, reshape_shape)
```

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/gptq/runner.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/gptq/runner.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/ptq/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/ptq/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/ptq/keras/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/ptq/keras/quantization_facade.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/ptq/keras/quantization_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/ptq/pytorch/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/ptq/pytorch/quantization_facade.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/ptq/pytorch/quantization_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/ptq/runner.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/ptq/runner.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/qat/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/keras/quantizer/ste_rounding/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/qat/common/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/common/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/qat/common/constants.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/common/constants.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/qat/common/qat_config.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/common/qat_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/qat/keras/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/qat/keras/quantization_facade.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/keras/quantization_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/qat/keras/quantizer/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/keras/quantizer/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/qat/keras/quantizer/base_keras_qat_quantizer.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/keras/quantizer/base_keras_qat_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/qat/keras/quantizer/quant_utils.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/keras/quantizer/quant_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/qat/keras/quantizer/quantization_builder.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/keras/quantizer/quantization_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/qat/keras/quantizer/ste_rounding/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-# ==============================================================================
+# ==============================================================================
```

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/qat/keras/quantizer/ste_rounding/symmetric_ste.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/keras/quantizer/ste_rounding/symmetric_ste.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
-from typing import Dict, Union
+from typing import Union
 
 import numpy as np
 import tensorflow as tf
 from tensorflow.python.framework.tensor_shape import TensorShape
 from model_compression_toolkit.core.common.constants import SIGNED
 
 from model_compression_toolkit.core.common.target_platform import QuantizationMethod
@@ -28,14 +28,15 @@
 from model_compression_toolkit.qat.keras.quantizer.base_keras_qat_quantizer import BaseKerasQATTrainableQuantizer
 from model_compression_toolkit.quantizers_infrastructure import TrainableQuantizerWeightsConfig, \
     TrainableQuantizerActivationConfig
 from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.common.base_inferable_quantizer import mark_quantizer
 from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.keras.quantizers import \
     WeightsPOTInferableQuantizer, WeightsSymmetricInferableQuantizer, ActivationPOTInferableQuantizer, \
     ActivationSymmetricInferableQuantizer
+from model_compression_toolkit.quantizers_infrastructure.trainable_infrastructure.common.base_trainable_quantizer import VariableGroup
 
 
 @mark_quantizer(quantization_target=qi.QuantizationTarget.Weights,
                 quantization_method=[QuantizationMethod.POWER_OF_TWO, QuantizationMethod.SYMMETRIC],
                 quantizer_type=TrainingMethod.STE)
 class STEWeightQATQuantizer(BaseKerasQATTrainableQuantizer):
     """
@@ -72,30 +73,27 @@
 
         self.num_bits = self.quantization_config.weights_n_bits
         delta = self.np_threshold_values / np.power(2.0, self.num_bits - int(C.WEIGHTS_SIGNED))
         min_int = -int(C.WEIGHTS_SIGNED) * (2 ** (self.num_bits - int(C.WEIGHTS_SIGNED)))
         max_int = (2 ** (self.num_bits - int(C.WEIGHTS_SIGNED))) - 1
         self.min = delta * min_int
         self.max = delta * max_int
-        self.quantizer_parameters = {}
+
 
     def initialize_quantization(self,
                                 tensor_shape: TensorShape,
                                 name: str,
-                                layer: qi.KerasQuantizationWrapper) -> Dict[str, tf.Variable]:
+                                layer: qi.KerasQuantizationWrapper):
         """
-        Add min and max variables to layer.
-        Args:
-            tensor_shape: Tensor shape the quantizer quantize.
-            name: Prefix of variables names.
-            layer: Layer to add the variables to. The variables are saved
-            in the layer's scope.
+        Add quantizer parameters to the quantizer parameters dictionary
 
-        Returns:
-            Dictionary of new variables.
+        Args:
+            tensor_shape: tensor shape of the quantized tensor.
+            name: Tensor name.
+            layer: Layer to quantize.
         """
         ptq_threshold_tensor = layer.add_weight(
             name + THRESHOLD_TENSOR,
             shape=len(self.np_threshold_values) if self.channel_axis else (),
             initializer=tf.keras.initializers.Constant(1.0),
             trainable=False)
         ptq_threshold_tensor.assign(self.np_threshold_values)
@@ -111,17 +109,17 @@
             name + FQ_MAX,
             shape=len(self.max) if self.channel_axis else (),
             initializer=tf.keras.initializers.Constant(1.0),
             trainable=False)
         fq_max.assign(self.max)
 
         # save the quantizer added parameters for later calculations
-        self.quantizer_parameters = {THRESHOLD_TENSOR: ptq_threshold_tensor,
-                                     FQ_MIN: fq_min, FQ_MAX: fq_max}
-        return self.quantizer_parameters
+        self.add_quantizer_variable(THRESHOLD_TENSOR, ptq_threshold_tensor, VariableGroup.QPARAMS)
+        self.add_quantizer_variable(FQ_MIN, fq_min, VariableGroup.QPARAMS)
+        self.add_quantizer_variable(FQ_MAX, fq_max, VariableGroup.QPARAMS)
 
     def __call__(self,
                  inputs: tf.Tensor,
                  training: bool):
         """
         Quantize a tensor.
         Args:
@@ -130,16 +128,16 @@
             weights: Dictionary of weights the quantizer can use to quantize the tensor.
             **kwargs: Additional variables the quantizer may receive.
 
         Returns:
             The quantized tensor.
         """
 
-        _min = self.quantizer_parameters[FQ_MIN]
-        _max = self.quantizer_parameters[FQ_MAX]
+        _min = self.get_quantizer_variable(FQ_MIN)
+        _max = self.get_quantizer_variable(FQ_MAX)
         if self.channel_axis:
             if self.perm_vec:
                 inputs = tf.transpose(inputs, perm=self.perm_vec)
             q_tensor = tf.quantization.fake_quant_with_min_max_vars_per_channel(inputs, _min, _max,
                                                                                 num_bits=self.num_bits)
             if self.perm_vec:
                 q_tensor = tf.transpose(q_tensor, perm=self.perm_vec)
@@ -153,24 +151,23 @@
         """
         Convert quantizer to inferable quantizer.
 
         Returns:
             BaseKerasInferableQuantizer object.
         """
         if self.power_of_two:
-            pot_threshold = 2 ** np.ceil(np.log2(self.quantizer_parameters[THRESHOLD_TENSOR]))
+            pot_threshold = 2 ** np.ceil(np.log2(self.get_quantizer_variable(THRESHOLD_TENSOR)))
             return WeightsPOTInferableQuantizer(num_bits=self.num_bits,
                                                 threshold=list(pot_threshold.flatten()),
                                                 per_channel=self.per_channel,
                                                 channel_axis=self.channel_axis,
                                                 input_rank=len(self.threshold_shape))
         else:
             return WeightsSymmetricInferableQuantizer(num_bits=self.num_bits,
-                                                      threshold=list(self.quantizer_parameters[
-                                                                         THRESHOLD_TENSOR].numpy().flatten()),
+                                                      threshold=list(self.get_quantizer_variable(THRESHOLD_TENSOR).numpy().flatten()),
                                                       per_channel=self.per_channel,
                                                       channel_axis=self.channel_axis,
                                                       input_rank=len(self.threshold_shape))
 
 
 @mark_quantizer(quantization_target=qi.QuantizationTarget.Activation,
                 quantization_method=[QuantizationMethod.POWER_OF_TWO, QuantizationMethod.SYMMETRIC],
@@ -199,30 +196,26 @@
                                                 np.ceil(np.log2(np.maximum(self.np_threshold_values, C.MIN_THRESHOLD))))
         self.num_bits = quantization_config.activation_n_bits
         delta = self.np_threshold_values / np.power(2.0, self.num_bits - int(self.signed))
         min_int = -int(self.signed) * (2 ** (self.num_bits - int(self.signed)))
         max_int = (2 ** (self.num_bits - int(self.signed))) - 1
         self.min = delta * min_int
         self.max = delta * max_int
-        self.quantizer_parameters = {}
 
     def initialize_quantization(self,
                                 tensor_shape: TensorShape,
                                 name: str,
-                                layer: qi.KerasQuantizationWrapper) -> Dict[str, tf.Variable]:
+                                layer: qi.KerasQuantizationWrapper):
         """
-        Add min and max variables to layer.
-        Args:
-            tensor_shape: Tensor shape the quantizer quantize.
-            name: Prefix of variables names.
-            layer: Layer to add the variables to. The variables are saved
-            in the layer's scope.
+        Add quantizer parameters to the quantizer parameters dictionary
 
-        Returns:
-            Dictionary of new variables.
+        Args:
+            tensor_shape: tensor shape of the quantized tensor.
+            name: Tensor name.
+            layer: Layer to quantize.
         """
         ptq_threshold_tensor = layer.add_weight(
             name + THRESHOLD_TENSOR,
             shape=(),
             initializer=tf.keras.initializers.Constant(1.0),
             trainable=False)
         ptq_threshold_tensor.assign(self.np_threshold_values)
@@ -238,53 +231,53 @@
             name + FQ_MAX,
             shape=(),
             initializer=tf.keras.initializers.Constant(1.0),
             trainable=False)
         fq_max.assign(self.max)
 
         # save the quantizer added parameters for later calculations
-        self.quantizer_parameters = {THRESHOLD_TENSOR: ptq_threshold_tensor,
-                                     FQ_MIN: fq_min, FQ_MAX: fq_max}
-        return self.quantizer_parameters
+        self.add_quantizer_variable(THRESHOLD_TENSOR, ptq_threshold_tensor, VariableGroup.QPARAMS)
+        self.add_quantizer_variable(FQ_MIN, fq_min, VariableGroup.QPARAMS)
+        self.add_quantizer_variable(FQ_MAX, fq_max, VariableGroup.QPARAMS)
+
 
     def __call__(self,
                  inputs: tf.Tensor,
                  training: bool):
         """
         Quantize a tensor.
         Args:
             inputs: Input tensor to quantize.
             training: Whether the graph is in training mode.
 
         Returns:
             The quantized tensor.
         """
 
-        _min = self.quantizer_parameters[FQ_MIN]
-        _max = self.quantizer_parameters[FQ_MAX]
+        _min = self.get_quantizer_variable(FQ_MIN)
+        _max = self.get_quantizer_variable(FQ_MAX)
         q_tensor = tf.quantization.fake_quant_with_min_max_vars(inputs, _min, _max,
                                                                 num_bits=self.num_bits)
 
         return q_tensor
 
     def convert2inferable(self) -> Union[ActivationPOTInferableQuantizer, ActivationSymmetricInferableQuantizer]:
         """
         Convert quantizer to inferable quantizer.
 
         Returns:
             BaseKerasInferableQuantizer object.
         """
 
         if self.power_of_two:
-            pot_threshold = 2 ** np.ceil(np.log2(self.quantizer_parameters[THRESHOLD_TENSOR]))
+            pot_threshold = 2 ** np.ceil(np.log2(self.get_quantizer_variable(THRESHOLD_TENSOR)))
             return ActivationPOTInferableQuantizer(num_bits=self.num_bits,
                                                       # In activation quantization is per-tensor only - thus we pass
                                                       # the threshold as a list with a len of 1
                                                       threshold=[pot_threshold],
                                                       signed=self.signed)
         else:
             return ActivationSymmetricInferableQuantizer(num_bits=self.num_bits,
                                                          # In activation quantization is per-tensor only - thus we
                                                          # pass the threshold as a list with a len of 1
-                                                         threshold=[
-                                                             self.quantizer_parameters[THRESHOLD_TENSOR].numpy()],
+                                                         threshold=[self.get_quantizer_variable(THRESHOLD_TENSOR).numpy()],
                                                          signed=self.signed)
```

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/qat/keras/quantizer/ste_rounding/uniform_ste.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/keras/quantizer/ste_rounding/uniform_ste.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,17 +8,14 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-
-from typing import Dict
-
 import numpy as np
 import tensorflow as tf
 from tensorflow.python.framework.tensor_shape import TensorShape
 from model_compression_toolkit.core.common.constants import RANGE_MIN, RANGE_MAX
 from model_compression_toolkit.core.common.target_platform import QuantizationMethod
 from model_compression_toolkit.qat.common.constants import FQ_MIN, FQ_MAX
 from model_compression_toolkit.qat.keras.quantizer.quant_utils import adjust_range_to_include_zero
@@ -28,14 +25,15 @@
 from model_compression_toolkit.qat.keras.quantizer.base_keras_qat_quantizer import BaseKerasQATTrainableQuantizer
 from model_compression_toolkit.quantizers_infrastructure import TrainableQuantizerWeightsConfig, \
     TrainableQuantizerActivationConfig
 from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.common.base_inferable_quantizer import \
     mark_quantizer
 from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.keras.quantizers import \
     BaseKerasInferableQuantizer, WeightsUniformInferableQuantizer, ActivationUniformInferableQuantizer
+from model_compression_toolkit.quantizers_infrastructure.trainable_infrastructure.common.base_trainable_quantizer import VariableGroup
 
 
 @mark_quantizer(quantization_target=qi.QuantizationTarget.Weights,
                 quantization_method=[QuantizationMethod.UNIFORM],
                 quantizer_type=TrainingMethod.STE)
 class STEUniformWeightQATQuantizer(BaseKerasQATTrainableQuantizer):
     """
@@ -66,30 +64,25 @@
             # need to move the quantization axis to the last axis
             self.perm_vec = list(np.arange(len(self.min_max_shape)))
             self.perm_vec[self.channel_axis] = len(self.min_max_shape) - 1
             self.perm_vec[len(self.min_max_shape) - 1] = self.channel_axis
         else:
             self.perm_vec = None
 
-        self.quantizer_parameters = {}
-
     def initialize_quantization(self,
                                 tensor_shape: TensorShape,
                                 name: str,
-                                layer: qi.KerasQuantizationWrapper) -> Dict[str, tf.Variable]:
+                                layer: qi.KerasQuantizationWrapper):
         """
-        Add min and max variables to layer.
-        Args:
-            tensor_shape: Tensor shape the quantizer quantize.
-            name: Prefix of variables names.
-            layer: Layer to add the variables to. The variables are saved
-            in the layer's scope.
+        Add quantizer parameters to the quantizer parameters dictionary
 
-        Returns:
-            Dictionary of new variables.
+        Args:
+            tensor_shape: tensor shape of the quantized tensor.
+            name: Tensor name.
+            layer: Layer to quantize.
         """
         fq_min = layer.add_weight(
             name + FQ_MIN,
             shape=len(self.min) if self.per_channel else (),
             initializer=tf.keras.initializers.Constant(-1.0),
             trainable=False)
         fq_min.assign(self.min)
@@ -98,31 +91,32 @@
             name + FQ_MAX,
             shape=len(self.max) if self.per_channel else (),
             initializer=tf.keras.initializers.Constant(1.0),
             trainable=False)
         fq_max.assign(self.max)
 
         # save the quantizer added parameters for later calculations
-        self.quantizer_parameters = {FQ_MIN: fq_min, FQ_MAX: fq_max}
-        return self.quantizer_parameters
+        self.add_quantizer_variable(FQ_MIN, fq_min, VariableGroup.QPARAMS)
+        self.add_quantizer_variable(FQ_MAX, fq_max, VariableGroup.QPARAMS)
+
 
     def __call__(self, inputs: tf.Tensor,
                  training: bool):
         """
         Quantize a tensor.
         Args:
             inputs: Input tensor to quantize.
             training: Whether the graph is in training mode.
 
         Returns:
             The quantized tensor.
         """
 
-        _min = self.quantizer_parameters[FQ_MIN]
-        _max = self.quantizer_parameters[FQ_MAX]
+        _min = self.get_quantizer_variable(FQ_MIN)
+        _max = self.get_quantizer_variable(FQ_MAX)
         _min, _max = adjust_range_to_include_zero(_min, _max, self.num_bits)
 
         if self.per_channel:
             if self.perm_vec:
                 inputs = tf.transpose(inputs, perm=self.perm_vec)
 
             q_tensor = tf.quantization.fake_quant_with_min_max_vars_per_channel(inputs, _min, _max,
@@ -138,16 +132,16 @@
     def convert2inferable(self) -> BaseKerasInferableQuantizer:
         """
         Convert quantizer to inferable quantizer.
 
         Returns:
             BaseKerasInferableQuantizer object.
         """
-        min_range, max_range = fix_range_to_include_zero(self.quantizer_parameters[FQ_MIN].numpy(),
-                                                         self.quantizer_parameters[FQ_MAX].numpy(),
+        min_range, max_range = fix_range_to_include_zero(self.get_quantizer_variable(FQ_MIN).numpy(),
+                                                         self.get_quantizer_variable(FQ_MAX).numpy(),
                                                          self.num_bits)
         return WeightsUniformInferableQuantizer(num_bits=self.num_bits,
                                                 min_range=list(min_range.flatten()),
                                                 max_range=list(max_range.flatten()),
                                                 per_channel=self.per_channel,
                                                 channel_axis=self.channel_axis,
                                                 input_rank=len(self.min_max_shape))
@@ -170,30 +164,26 @@
             quantization_config: trainable quantizer config class
         """
         super().__init__(quantization_config)
 
         self.num_bits = quantization_config.activation_n_bits
         self.min_range = quantization_config.activation_quantization_params[C.RANGE_MIN]
         self.max_range = quantization_config.activation_quantization_params[C.RANGE_MAX]
-        self.quantizer_parameters = {}
 
     def initialize_quantization(self,
                                 tensor_shape: TensorShape,
                                 name: str,
-                                layer: qi.KerasQuantizationWrapper) -> Dict[str, tf.Variable]:
+                                layer: qi.KerasQuantizationWrapper):
         """
-        Add min and max variables to layer.
-        Args:
-            tensor_shape: Tensor shape the quantizer quantize.
-            name: Prefix of variables names.
-            layer: Layer to add the variables to. The variables are saved
-            in the layer's scope.
+        Add quantizer parameters to the quantizer parameters dictionary
 
-        Returns:
-            Dictionary of new variables.
+        Args:
+            tensor_shape: tensor shape of the quantized tensor.
+            name: Tensor name.
+            layer: Layer to quantize.
         """
         fq_min = layer.add_weight(
             name + FQ_MIN,
             shape=(),
             initializer=tf.keras.initializers.Constant(-1.0),
             trainable=False)
         fq_min.assign(self.min_range)
@@ -202,46 +192,47 @@
             name + FQ_MAX,
             shape=(),
             initializer=tf.keras.initializers.Constant(1.0),
             trainable=False)
         fq_max.assign(self.max_range)
 
         # save the quantizer added parameters for later calculations
-        self.quantizer_parameters = {FQ_MIN: fq_min, FQ_MAX: fq_max}
-        return self.quantizer_parameters
+        self.add_quantizer_variable(FQ_MIN, fq_min, VariableGroup.QPARAMS)
+        self.add_quantizer_variable(FQ_MAX, fq_max, VariableGroup.QPARAMS)
+
 
     def __call__(self,
                  inputs: tf.Tensor,
                  training: bool):
         """
         Quantize a tensor.
         Args:
             inputs: Input tensor to quantize.
             training: Whether the graph is in training mode.
 
         Returns:
             The quantized tensor.
         """
 
-        _min = self.quantizer_parameters[FQ_MIN]
-        _max = self.quantizer_parameters[FQ_MAX]
+        _min = self.get_quantizer_variable(FQ_MIN)
+        _max = self.get_quantizer_variable(FQ_MAX)
         _min, _max = adjust_range_to_include_zero(_min, _max, self.num_bits)
         q_tensor = tf.quantization.fake_quant_with_min_max_vars(inputs, _min, _max,
                                                                 num_bits=self.num_bits)
 
         return q_tensor
 
     def convert2inferable(self) -> BaseKerasInferableQuantizer:
         """
         Convert quantizer to inferable quantizer.
 
         Returns:
             BaseKerasInferableQuantizer object.
         """
-        min_range, max_range = fix_range_to_include_zero(self.quantizer_parameters[FQ_MIN].numpy(),
-                                                         self.quantizer_parameters[FQ_MAX].numpy(),
+        min_range, max_range = fix_range_to_include_zero(self.get_quantizer_variable(FQ_MIN).numpy(),
+                                                         self.get_quantizer_variable(FQ_MAX).numpy(),
                                                          self.num_bits)
         return ActivationUniformInferableQuantizer(num_bits=self.num_bits,
                                                    # In activation quantization is per-tensor only - thus we pass
                                                    # the min/max as lists with a len of 1
                                                    min_range=[min_range],
                                                    max_range=[max_range])
```

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/qat/pytorch/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/exporter/model_exporter/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,7 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
+
```

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/qat/pytorch/quantization_facade.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/pytorch/quantization_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/qat/pytorch/quantizer/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/pytorch/quantizer/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/qat/pytorch/quantizer/base_pytorch_qat_quantizer.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/pytorch/quantizer/base_pytorch_qat_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/qat/pytorch/quantizer/quantization_builder.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/pytorch/quantizer/quantization_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/qat/pytorch/quantizer/quantizer_utils.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/pytorch/quantizer/quantizer_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/activation_inferable_quantizers/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-# Copyright 2022 Sony Semiconductor Israel, Inc. All rights reserved.
+# Copyright 2023 Sony Semiconductor Israel, Inc. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-# ==============================================================================
+# ==============================================================================
```

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/symmetric_ste.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/symmetric_ste.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-from typing import Dict, Union
+from typing import Union
 
 import numpy as np
 import torch
 import torch.nn as nn
 
 from model_compression_toolkit.core.common.target_platform import QuantizationMethod
 from model_compression_toolkit.qat.common import THRESHOLD_TENSOR
@@ -27,14 +27,15 @@
 from model_compression_toolkit.core.pytorch.utils import to_torch_tensor
 from model_compression_toolkit.qat.pytorch.quantizer.quantizer_utils import ste_round, ste_clip, symmetric_quantizer
 from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.pytorch.quantizers import \
     WeightsPOTInferableQuantizer, WeightsSymmetricInferableQuantizer, ActivationPOTInferableQuantizer, \
     ActivationSymmetricInferableQuantizer
 from model_compression_toolkit.quantizers_infrastructure.trainable_infrastructure.common.trainable_quantizer_config import \
     TrainableQuantizerWeightsConfig, TrainableQuantizerActivationConfig
+from model_compression_toolkit.quantizers_infrastructure.trainable_infrastructure.common.base_trainable_quantizer import VariableGroup
 
 
 @mark_quantizer(quantization_target=qi.QuantizationTarget.Weights,
                 quantization_method=[QuantizationMethod.POWER_OF_TWO, QuantizationMethod.SYMMETRIC],
                 quantizer_type=TrainingMethod.STE)
 class STEWeightQATQuantizer(BasePytorchQATTrainableQuantizer):
     """
@@ -62,40 +63,36 @@
         n_pos_bits = self.num_bits - int(C.WEIGHTS_SIGNED)
         delta = self.np_threshold_values / np.power(2.0, n_pos_bits)
         self.delta_tensor = to_torch_tensor(delta)
         self.min_int = -int(C.WEIGHTS_SIGNED) * (2 ** n_pos_bits)
         self.max_int = (2 ** n_pos_bits) - 1
         self.min = delta * self.min_int
         self.max = delta * self.max_int
-        self.quantizer_parameters = {}
+
 
     def initialize_quantization(self,
                                 tensor_shape: torch.Size,
                                 name: str,
-                                layer: qi.PytorchQuantizationWrapper) -> Dict[str, nn.Parameter]:
+                                layer: qi.PytorchQuantizationWrapper):
         """
-        Add min and max variables to layer.
-        Args:
-            tensor_shape: Tensor shape the quantizer quantize.
-            name: Prefix of variables names.
-            layer: Layer to add the variables to. The variables are saved
-            in the layer's scope.
+        Add quantizer parameters to the quantizer parameters dictionary
 
-        Returns:
-            Dictionary of new variables.
+        Args:
+            tensor_shape: tensor shape of the quantized tensor.
+            name: Tensor name.
+            layer: Layer to quantize.
         """
 
         # Add threshold variables to layer.
         layer.register_parameter(name + "_" + THRESHOLD_TENSOR, nn.Parameter(to_torch_tensor(self.np_threshold_values),
                                                                              requires_grad=False))
 
         # save the quantizer added parameters for later calculations
-        self.quantizer_parameters = {THRESHOLD_TENSOR: layer.get_parameter(name + "_" + THRESHOLD_TENSOR)}
+        self.add_quantizer_variable(THRESHOLD_TENSOR, layer.get_parameter(name + "_" + THRESHOLD_TENSOR), VariableGroup.QPARAMS)
 
-        return self.quantizer_parameters
 
     def __call__(self,
                  inputs: nn.Parameter,
                  training: bool) -> nn.Parameter:
         """
         Quantize a tensor
         Args:
@@ -112,15 +109,15 @@
     def convert2inferable(self) -> Union[WeightsPOTInferableQuantizer, WeightsSymmetricInferableQuantizer]:
         """
         Convert quantizer to inferable quantizer.
 
         Returns:
             A pytorch inferable quanizer object.
         """
-        np_threshold = self.quantizer_parameters[THRESHOLD_TENSOR].cpu().detach().numpy().flatten()
+        np_threshold = self.get_quantizer_variable(THRESHOLD_TENSOR).cpu().detach().numpy().flatten()
         if self.power_of_two:
             pot_threshold = 2 ** np.ceil(np.log2(np_threshold))
             return WeightsPOTInferableQuantizer(num_bits=self.num_bits,
                                                 threshold=pot_threshold,
                                                 per_channel=self.quantization_config.weights_per_channel_threshold,
                                                 channel_axis=self.quantization_config.weights_channels_axis)
         else:
@@ -149,54 +146,57 @@
         """
         super().__init__(quantization_config)
         self.power_of_two = quantization_config.activation_quantization_method == QuantizationMethod.POWER_OF_TWO
         self.sign = quantization_config.activation_quantization_params['is_signed']
         np_threshold_values = quantization_config.activation_quantization_params[C.THRESHOLD]
         self.threshold_tensor = torch.Tensor([np_threshold_values])
         self.num_bits = quantization_config.activation_n_bits
-        self.quantizer_parameters = {}
 
     def initialize_quantization(self,
                                 tensor_shape: torch.Size,
                                 name: str,
-                                layer: qi.PytorchQuantizationWrapper) -> Dict[str, nn.Parameter]:
+                                layer: qi.PytorchQuantizationWrapper):
         """
-        Add threshold variables to layer.
+        Add quantizer parameters to the quantizer parameters dictionary
+
+        Args:
+            tensor_shape: tensor shape of the quantized tensor.
+            name: Tensor name.
+            layer: Layer to quantize.
         """
         layer.register_parameter(name, nn.Parameter(to_torch_tensor(self.threshold_tensor), requires_grad=True))
 
         # save the quantizer added parameters for later calculations
-        self.quantizer_parameters = {THRESHOLD_TENSOR: layer.get_parameter(name)}
-        return self.quantizer_parameters
+        self.add_quantizer_variable(THRESHOLD_TENSOR, layer.get_parameter(name), VariableGroup.QPARAMS)
 
     def __call__(self,
                  inputs: torch.Tensor,
                  training: bool = True) -> torch.Tensor:
         """
         Quantize a tensor.
         Args:
             inputs: Input tensor to quantize.
             training: Whether the graph is in training mode.
 
         Returns:
             The quantized tensor.
         """
 
-        _t = self.quantizer_parameters[THRESHOLD_TENSOR]
+        _t = self.get_quantizer_variable(THRESHOLD_TENSOR)
         q_tensor = symmetric_quantizer(inputs, _t, self.num_bits, sign=self.sign)
         return q_tensor
 
     def convert2inferable(self) -> Union[ActivationPOTInferableQuantizer, ActivationSymmetricInferableQuantizer]:
         """
         Convert quantizer to inferable quantizer.
 
         Returns:
             A pytorch inferable quanizer object.
         """
-        np_threshold = self.quantizer_parameters[THRESHOLD_TENSOR].cpu().detach().numpy()
+        np_threshold = self.get_quantizer_variable(THRESHOLD_TENSOR).cpu().detach().numpy()
         if self.power_of_two:
             pot_threshold = np.power(2.0, np.ceil(np.log2(np_threshold)))
             return ActivationPOTInferableQuantizer(num_bits=self.num_bits,
                                                    threshold=pot_threshold,
                                                    signed=self.sign)
         else:
             return ActivationSymmetricInferableQuantizer(num_bits=self.num_bits,
```

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/uniform_ste.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/uniform_ste.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-from typing import Dict
-
 import numpy as np
 import torch
 import torch.nn as nn
 from torch import Tensor
 
 from model_compression_toolkit.core.common.constants import RANGE_MAX, RANGE_MIN
 from model_compression_toolkit.core.common.target_platform import QuantizationMethod
@@ -28,14 +26,15 @@
 from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.common.base_inferable_quantizer import mark_quantizer
 from model_compression_toolkit.core.pytorch.utils import to_torch_tensor
 from model_compression_toolkit.qat.pytorch.quantizer.quantizer_utils import uniform_quantizer
 from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.pytorch.quantizers import \
     WeightsUniformInferableQuantizer, ActivationUniformInferableQuantizer
 from model_compression_toolkit.quantizers_infrastructure.trainable_infrastructure.common.trainable_quantizer_config import \
     TrainableQuantizerWeightsConfig, TrainableQuantizerActivationConfig
+from model_compression_toolkit.quantizers_infrastructure.trainable_infrastructure.common.base_trainable_quantizer import VariableGroup
 
 
 @mark_quantizer(quantization_target=qi.QuantizationTarget.Weights,
                 quantization_method=[QuantizationMethod.UNIFORM],
                 quantizer_type=TrainingMethod.STE)
 class STEUniformWeightQATQuantizer(BasePytorchQATTrainableQuantizer):
     """
@@ -60,63 +59,59 @@
         self.max = np.reshape(self.max_values,
                               [-1]) if self.quantization_config.weights_per_channel_threshold else float(
             self.max_values)
         self.min = np.reshape(self.min_values,
                               [-1]) if self.quantization_config.weights_per_channel_threshold else float(
             self.min_values)
 
-        self.quantizer_parameters = {}
 
     def initialize_quantization(self,
                                 tensor_shape: torch.Size,
                                 name: str,
-                                layer: qi.PytorchQuantizationWrapper) -> Dict[str, nn.Parameter]:
+                                layer: qi.PytorchQuantizationWrapper):
         """
-        Add min and max variables to layer.
-        Args:
-            tensor_shape: Tensor shape the quantizer quantize.
-            name: Prefix of variables names.
-            layer: Layer to add the variables to. The variables are saved
-            in the layer's scope.
+        Add quantizer parameters to the quantizer parameters dictionary
 
-        Returns:
-            Dictionary of new variables.
+        Args:
+            tensor_shape: tensor shape of the quantized tensor.
+            name: Tensor name.
+            layer: Layer to quantize.
         """
 
         # Add min and max variables to layer.
         layer.register_parameter(name+"_"+FQ_MIN, nn.Parameter(to_torch_tensor(self.min_values), requires_grad=False))
         layer.register_parameter(name+"_"+FQ_MAX, nn.Parameter(to_torch_tensor(self.max_values), requires_grad=False))
 
         # Save the quantizer parameters for later calculations
-        self.quantizer_parameters = {FQ_MIN: layer.get_parameter(name+"_"+FQ_MIN), FQ_MAX: layer.get_parameter(name+"_"+FQ_MAX)}
+        self.add_quantizer_variable(FQ_MIN, layer.get_parameter(name+"_"+FQ_MIN), VariableGroup.QPARAMS)
+        self.add_quantizer_variable(FQ_MAX, layer.get_parameter(name+"_"+FQ_MAX), VariableGroup.QPARAMS)
 
-        return self.quantizer_parameters
 
     def __call__(self,
                  inputs: nn.Parameter,
                  training: bool) -> Tensor:
         """
         Quantize a tensor
         Args:
             inputs: Input tensor to quantize.
             training: whether in training mode or not
         Returns:
             quantized tensor
         """
-        return uniform_quantizer(inputs, self.quantizer_parameters[FQ_MIN], self.quantizer_parameters[FQ_MAX], self.num_bits)
+        return uniform_quantizer(inputs, self.get_quantizer_variable(FQ_MIN), self.get_quantizer_variable(FQ_MAX), self.num_bits)
 
     def convert2inferable(self) -> WeightsUniformInferableQuantizer:
         """
         Convert quantizer to inferable quantizer.
 
         Returns:
             A pytorch inferable quanizer object.
         """
-        _min = self.quantizer_parameters[FQ_MIN].cpu().detach().numpy()
-        _max = self.quantizer_parameters[FQ_MAX].cpu().detach().numpy()
+        _min = self.get_quantizer_variable(FQ_MIN).cpu().detach().numpy()
+        _max = self.get_quantizer_variable(FQ_MAX).cpu().detach().numpy()
 
         return WeightsUniformInferableQuantizer(num_bits=self.num_bits,
                                                 min_range=_min, max_range=_max,
                                                 per_channel=self.quantization_config.weights_per_channel_threshold,
                                                 channel_axis=self.quantization_config.weights_channels_axis)
 
 
@@ -139,53 +134,57 @@
         super().__init__(quantization_config)
 
         np_min_range = quantization_config.activation_quantization_params[C.RANGE_MIN]
         np_max_range = quantization_config.activation_quantization_params[C.RANGE_MAX]
         self.min_range_tensor = torch.Tensor([np_min_range])
         self.max_range_tensor = torch.Tensor([np_max_range])
         self.num_bits = quantization_config.activation_n_bits
-        self.quantizer_parameters = {}
 
     def initialize_quantization(self,
                                 tensor_shape: torch.Size,
                                 name: str,
-                                layer: qi.PytorchQuantizationWrapper) -> Dict[str, nn.Parameter]:
+                                layer: qi.PytorchQuantizationWrapper):
         """
-        Add min and max variables to layer.
+        Add quantizer parameters to the quantizer parameters dictionary
+
+        Args:
+            tensor_shape: tensor shape of the quantized tensor.
+            name: Tensor name.
+            layer: Layer to quantize.
         """
         layer.register_parameter(name+"_"+FQ_MIN, nn.Parameter(to_torch_tensor(self.min_range_tensor), requires_grad=True))
         layer.register_parameter(name+"_"+FQ_MAX, nn.Parameter(to_torch_tensor(self.max_range_tensor), requires_grad=True))
 
         # Save the quantizer parameters for later calculations
-        self.quantizer_parameters = {FQ_MIN: layer.get_parameter(name+"_"+FQ_MIN), FQ_MAX: layer.get_parameter(name+"_"+FQ_MAX)}
-        return self.quantizer_parameters
+        self.add_quantizer_variable(FQ_MIN, layer.get_parameter(name+"_"+FQ_MIN), VariableGroup.QPARAMS)
+        self.add_quantizer_variable(FQ_MAX, layer.get_parameter(name+"_"+FQ_MAX), VariableGroup.QPARAMS)
 
     def __call__(self,
                  inputs: torch.Tensor,
                  training: bool = True) -> torch.Tensor:
         """
         Quantize a tensor.
         Args:
             inputs: Input tensor to quantize.
             training: Whether the graph is in training mode.
 
         Returns:
             The quantized tensor.
         """
 
-        _min = self.quantizer_parameters[FQ_MIN]
-        _max = self.quantizer_parameters[FQ_MAX]
+        _min = self.get_quantizer_variable(FQ_MIN)
+        _max = self.get_quantizer_variable(FQ_MAX)
         q_tensor = uniform_quantizer(inputs, _min, _max, self.num_bits)
         return q_tensor
 
     def convert2inferable(self) -> ActivationUniformInferableQuantizer:
         """
         Convert quantizer to inferable quantizer.
 
         Returns:
             A pytorch inferable quanizer object.
         """
-        _min = self.quantizer_parameters[FQ_MIN].cpu().detach().numpy()
-        _max = self.quantizer_parameters[FQ_MAX].cpu().detach().numpy()
+        _min = self.get_quantizer_variable(FQ_MIN).cpu().detach().numpy()
+        _max = self.get_quantizer_variable(FQ_MAX).cpu().detach().numpy()
 
         return ActivationUniformInferableQuantizer(num_bits=self.num_bits,
                                                    min_range=_min, max_range=_max)
```

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/common/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/common/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/common/activation_lut_pot_inferable_quantizer.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/common/base_inferable_quantizer.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/common/base_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/common/constants.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/common/constants.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/common/get_all_subclasses.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/common/get_all_subclasses.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,9 +24,8 @@
     Args:
         cls: A class object.
 
     Returns: All classes that inherit from cls.
 
     """
 
-    return set(cls.__subclasses__()).union(
-        [s for c in cls.__subclasses__() for s in get_all_subclasses(c)])
+    return set(cls.__subclasses__()).union([s for c in cls.__subclasses__() for s in get_all_subclasses(c)])
```

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/common/get_quantizers.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/common/get_quantizers.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
     Returns: A class of a quantizer that inherits from BaseKerasInferableQuantizer.
 
     """
     qat_quantizer_classes = get_all_subclasses(quantizer_base_class)
     filtered_quantizers = list(filter(lambda q_class: getattr(q_class, QUANTIZATION_TARGET) == quant_target and
                                                       getattr(q_class, QUANTIZATION_METHOD) is not None and
-                                                       quant_method in getattr(q_class, QUANTIZATION_METHOD),
+                                                      quant_method in getattr(q_class, QUANTIZATION_METHOD),
                                       qat_quantizer_classes))
 
     if len(filtered_quantizers) != 1:
         Logger.error(f"Found {len(filtered_quantizers)} quantizer for target {quant_target.value} "
                      f"that matches the requested quantization method {quant_method.name} "
                      f"but there should be exactly one."
                      f"The possible quantizers that were found are {filtered_quantizers}.")
```

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/common/quant_utils.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/common/quant_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/load_model.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/load_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantize_wrapper.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantize_wrapper.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizer_utils.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizer_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,10 +14,14 @@
 # ==============================================================================
 from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.keras.quantizers.base_keras_inferable_quantizer import \
     BaseKerasInferableQuantizer
 
 from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.keras.quantizers.weights_inferable_quantizers.weights_pot_inferable_quantizer import WeightsPOTInferableQuantizer
 from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.keras.quantizers.weights_inferable_quantizers.weights_symmetric_inferable_quantizer import WeightsSymmetricInferableQuantizer
 from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.keras.quantizers.weights_inferable_quantizers.weights_uniform_inferable_quantizer import WeightsUniformInferableQuantizer
+from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.keras.quantizers.weights_inferable_quantizers.weights_lut_symmetric_inferable_quantizer import WeightsLUTSymmetricInferableQuantizer
+from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.keras.quantizers.weights_inferable_quantizers.weights_lut_pot_inferable_quantizer import WeightsLUTPOTInferableQuantizer
+
 from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.keras.quantizers.activation_inferable_quantizers.activation_pot_inferable_quantizer import ActivationPOTInferableQuantizer
 from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.keras.quantizers.activation_inferable_quantizers.activation_symmetric_inferable_quantizer import ActivationSymmetricInferableQuantizer
 from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.keras.quantizers.activation_inferable_quantizers.activation_uniform_inferable_quantizer import ActivationUniformInferableQuantizer
+from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.keras.quantizers.activation_inferable_quantizers.activation_lut_pot_inferable_quantizer import ActivationLutPOTInferableQuantizer
```

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/activation_inferable_quantizers/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/activation_inferable_quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/base_keras_inferable_quantizer.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/base_keras_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/constants.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/constants.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,7 +18,8 @@
 SIGNED = 'signed'
 THRESHOLD = 'threshold'
 PER_CHANNEL = 'per_channel'
 MIN_RANGE = 'min_range'
 MAX_RANGE = 'max_range'
 CHANNEL_AXIS = 'channel_axis'
 INPUT_RANK = 'input_rank'
+CLUSTER_CENTERS = 'cluster_centers'
```

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/weights_inferable_quantizers/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/weights_inferable_quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/validation_functions.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/validation_functions.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantize_wrapper.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantize_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -180,21 +180,19 @@
                 List pf tuples of the wrapped layer's weights variables with weight name, values and assigned quantizer.
 
             """
 
             return self._weights_vars
 
         def forward(self,
-                    x: torch.Tensor,
                     *args: List[Any],
                     **kwargs: Dict[str, Any]) -> Union[torch.Tensor, List[torch.Tensor]]:
             """
             PytorchQuantizationWrapper forward functions
             Args:
-                x: layer's inputs
                 args: arguments to pass to internal layer.
                 kwargs: key-word dictionary to pass to the internal layer.
 
             Returns: a tensor that simulates a quantized layer.
 
             """
 
@@ -214,15 +212,15 @@
                     quantized_weights.update({name: quantized_weight})
 
                 self.set_quantize_weights(quantized_weights)
 
             # ----------------------------------
             # Layer operation
             # ----------------------------------
-            outputs = self.layer(x, *args, **kwargs)
+            outputs = self.layer(*args, **kwargs)
 
             # ----------------------------------
             # Quantize all activations
             # ----------------------------------
             if self.is_activation_quantization:
 
                 if not isinstance(outputs, list):
@@ -236,14 +234,26 @@
                 for quantizer, output in zip(self._activation_vars, outputs):
                     outputs_quantized.append(quantizer(output))
 
                 outputs = outputs_quantized[0] if len(outputs_quantized) == 1 else outputs_quantized
 
             return outputs
 
+        def get_quantized_weights(self) -> Dict[str, torch.Tensor]:
+            """
+
+            Returns: A dictionary of weights attributes to quantized weights.
+
+            """
+            quantized_weights = {}
+            weights_var = self.get_weights_vars()
+            for name, w, quantizer in weights_var:
+                quantized_weights[name] = quantizer(w)
+            return quantized_weights
+
 else:
     class PytorchQuantizationWrapper(object):
         def __init__(self,
                      layer,
                      weight_quantizers: Dict[str, BaseInferableQuantizer] = None,
                      activation_quantizers: List[BaseInferableQuantizer] = None):
             """
```

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizer_utils.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizer_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,15 +15,21 @@
 
 from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.pytorch.quantizers.activation_inferable_quantizers.activation_pot_inferable_quantizer \
     import ActivationPOTInferableQuantizer
 from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.pytorch.quantizers.activation_inferable_quantizers.activation_symmetric_inferable_quantizer \
     import ActivationSymmetricInferableQuantizer
 from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.pytorch.quantizers.activation_inferable_quantizers.activation_uniform_inferable_quantizer \
     import ActivationUniformInferableQuantizer
+from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.pytorch.quantizers.activation_inferable_quantizers.activation_lut_pot_inferable_quantizer \
+    import ActivationLutPOTInferableQuantizer
 from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.pytorch.quantizers.base_pytorch_inferable_quantizer \
     import BasePyTorchInferableQuantizer
 from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.pytorch.quantizers.weights_inferable_quantizers.weights_pot_inferable_quantizer \
     import WeightsPOTInferableQuantizer
 from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.pytorch.quantizers.weights_inferable_quantizers.weights_symmetric_inferable_quantizer \
     import WeightsSymmetricInferableQuantizer
 from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.pytorch.quantizers.weights_inferable_quantizers.weights_uniform_inferable_quantizer \
     import WeightsUniformInferableQuantizer
+from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.pytorch.quantizers.weights_inferable_quantizers.weights_lut_symmetric_inferable_quantizer \
+    import WeightsLUTSymmetricInferableQuantizer
+from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.pytorch.quantizers.weights_inferable_quantizers.weights_lut_pot_inferable_quantizer \
+    import WeightsLUTPOTInferableQuantizer
```

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/activation_inferable_quantizers/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/weights_inferable_quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/base_lut_symmetric_inferable_quantizer.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/base_lut_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/base_pytorch_inferable_quantizer.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/base_pytorch_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/base_symmetric_inferable_quantizer.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/base_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/base_uniform_inferable_quantizer.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/base_uniform_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/constants.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/constants.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,7 +17,10 @@
 NUM_BITS = 'num_bits'
 SIGNED = 'signed'
 THRESHOLD = 'threshold'
 PER_CHANNEL = 'per_channel'
 MIN_RANGE = 'min_range'
 MAX_RANGE = 'max_range'
 CHANNEL_AXIS = 'channel_axis'
+CLUSTER_CENTERS = 'cluster_centers'
+MULTIPLIER_N_BITS = 'multiplier_n_bits'
+EPS = 'eps'
```

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/weights_inferable_quantizers/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-# ==============================================================================
+# ==============================================================================
```

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/common/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/common/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/common/base_trainable_quantizer.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/common/base_trainable_quantizer.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,29 +8,43 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-
-from typing import Union
+from abc import abstractmethod
+from enum import Enum
+from typing import Union, List, Any
 from inspect import signature
 
 from model_compression_toolkit.core import common
 from model_compression_toolkit.core.common import Logger
 
 from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.common.base_inferable_quantizer import BaseInferableQuantizer, \
     QuantizationTarget
 from model_compression_toolkit.quantizers_infrastructure.trainable_infrastructure.common.trainable_quantizer_config import \
     TrainableQuantizerActivationConfig, TrainableQuantizerWeightsConfig
 from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.common.constants import QUANTIZATION_METHOD, \
     QUANTIZATION_TARGET
 
 
+VAR = 'var'
+GROUP = 'group'
+
+class VariableGroup(Enum):
+    """
+    An enum for choosing trainable variable group
+    0. WEIGHTS
+    1. QPARAMS
+    """
+    WEIGHTS = 0
+    QPARAMS = 1
+
+
 class BaseTrainableQuantizer(BaseInferableQuantizer):
     def __init__(self,
                  quantization_config: Union[TrainableQuantizerActivationConfig, TrainableQuantizerWeightsConfig]):
         """
         This class is a base quantizer which validates the provided quantization config and defines an abstract function which any quantizer needs to implment.
 
         Args:
@@ -66,14 +80,16 @@
             if self.quantization_config.activation_quantization_method not in static_quantization_method:
                 common.Logger.error(
                     f'Quantization method mismatch expected: {static_quantization_method} and got  {self.quantization_config.activation_quantization_method}')
         else:
             common.Logger.error(
                 f'Unknown Quantization Part:{static_quantization_target}')  # pragma: no cover
 
+        self.quantizer_parameters = {}
+
     @classmethod
     def get_sig(cls):
         return signature(cls)
 
     def initialize_quantization(self,
                                 tensor_shape,
                                 name: str,
@@ -143,7 +159,42 @@
         """
         Convert quantizer to inferable quantizer.
 
         Returns:
             BaseInferableQuantizer object.
         """
         raise NotImplemented  # pragma: no cover
+
+    def add_quantizer_variable(self, name: str, variable: Any, group: VariableGroup = VariableGroup.WEIGHTS):
+        """
+        Add a quantizer variable to quantizer_parameters dictionary
+        """
+        self.quantizer_parameters.update({name: {VAR: variable, GROUP: group}})
+
+    def get_quantizer_variable(self, name: str) -> Any:
+        """
+        Get a quantizer variable by name
+
+        Args:
+            name: variable name
+
+        Returns:
+            trainable variable
+        """
+        if name in self.quantizer_parameters:
+            return self.quantizer_parameters[name][VAR]
+        else:
+            common.Logger.error(f'Variable {name} is not exist in quantizers parameters!') # pragma: no cover
+
+
+    @abstractmethod
+    def get_trainable_variables(self, group: VariableGroup) -> List[Any]:
+        """
+        Get trainable parameters with specific group from quantizer
+
+        Args:
+            group: Enum of variable group
+
+        Returns:
+            List of trainable variables
+        """
+        raise NotImplemented  # pragma: no cover
```

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/common/get_quantizer_config.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/common/get_quantizer_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/common/get_quantizers.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/common/get_quantizers.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from typing import Union
 
-from model_compression_toolkit import TrainingMethod, RoundingType
+from model_compression_toolkit.gptq import RoundingType
+from model_compression_toolkit import TrainingMethod
 from model_compression_toolkit.core.common import Logger
 from model_compression_toolkit.core.common.target_platform import QuantizationMethod
 from model_compression_toolkit.quantizers_infrastructure import QuantizationTarget
 from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.common.constants \
     import QUANTIZATION_TARGET, QUANTIZATION_METHOD, QUANTIZER_TYPE
 from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.common.get_all_subclasses \
     import get_all_subclasses
```

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/common/quant_utils.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/common/quant_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/common/trainable_quantizer_config.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/common/trainable_quantizer_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/keras/__init__.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/keras/base_keras_quantizer.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/pytorch/base_pytorch_quantizer.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,65 +8,59 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-from typing import Dict, Any, Union
+from typing import Union, List
 
-from model_compression_toolkit.core.common import Logger
-from model_compression_toolkit.core.common.constants import FOUND_TF
-
-from model_compression_toolkit.quantizers_infrastructure.trainable_infrastructure.common.base_trainable_quantizer import BaseTrainableQuantizer
+from model_compression_toolkit.core.common.logger import Logger
+from model_compression_toolkit.core.common.constants import FOUND_TORCH
+from model_compression_toolkit.quantizers_infrastructure.trainable_infrastructure.common.base_trainable_quantizer import VariableGroup
+from model_compression_toolkit.quantizers_infrastructure.trainable_infrastructure.common.base_trainable_quantizer import BaseTrainableQuantizer, VAR, GROUP
 from model_compression_toolkit.quantizers_infrastructure import TrainableQuantizerWeightsConfig, \
     TrainableQuantizerActivationConfig
 
-if FOUND_TF:
-    QUANTIZATION_CONFIG = 'quantization_config'
-    from model_compression_toolkit.quantizers_infrastructure.trainable_infrastructure.keras.config_serialization import config_serialization, \
-        config_deserialization
 
+if FOUND_TORCH:
+
+    import torch
 
-    class BaseKerasTrainableQuantizer(BaseTrainableQuantizer):
+    class BasePytorchTrainableQuantizer(BaseTrainableQuantizer):
         def __init__(self,
                      quantization_config: Union[TrainableQuantizerWeightsConfig, TrainableQuantizerActivationConfig]):
             """
-            This class is a base quantizer which validates provided quantization config and defines an abstract function which any quantizer needs to implement.
-            This class adds to the base quantizer a get_config and from_config functions to enable loading and saving the keras model.
+            This class is a base Pytorch quantizer which validates the provided quantization config and defines an
+            abstract function which any quantizer needs to implement.
+
             Args:
-                quantization_config: quantizer config class contains all the information about a quantizer configuration.
+                quantization_config: quantizer config class contains all the information about the quantizer configuration.
             """
             super().__init__(quantization_config)
 
-        def get_config(self) -> Dict[str, Any]:
-            """
-
-            Returns: Configuration of BaseKerasQuantizer.
 
+        def get_trainable_variables(self, group: VariableGroup) -> List[torch.Tensor]:
             """
-            return {QUANTIZATION_CONFIG: config_serialization(self.quantization_config)}
-
-        @classmethod
-        def from_config(cls, config: dict):
-            """
+            Get trainable parameters with specific group from quantizer
 
             Args:
-                config(dict): dictonory  of  BaseKerasQuantizer Configuration
-
-            Returns: A BaseKerasQuantizer
+                group: Enum of variable group
 
+            Returns:
+                List of trainable variables
             """
-            config = config.copy()
-            quantization_config = config_deserialization(config[QUANTIZATION_CONFIG])
-            # Note that a quantizer only receive quantization config and the rest of define hardcoded inside the speficie quantizer.
-            return cls(quantization_config=quantization_config)
+            quantizer_trainable = []
+            for name, parameter_dict in self.quantizer_parameters.items():
+                quantizer_parameter, parameter_group = parameter_dict[VAR], parameter_dict[GROUP]
+                if quantizer_parameter.requires_grad and parameter_group == group:
+                    quantizer_trainable.append(quantizer_parameter)
+            return quantizer_trainable
 
 else:
-    class BaseKerasTrainableQuantizer(BaseTrainableQuantizer):
+    class BasePytorchTrainableQuantizer(BaseTrainableQuantizer):
         def __init__(self,
                      quantization_config: Union[TrainableQuantizerWeightsConfig, TrainableQuantizerActivationConfig]):
-
             super().__init__(quantization_config)
-            Logger.critical('Installing tensorflow and tensorflow_model_optimization is mandatory '
-                            'when using BaseKerasQuantizer. '
-                            'Could not find Tensorflow package.')  # pragma: no cover
+            Logger.critical('Installing Pytorch is mandatory '
+                            'when using BasePytorchTrainableQuantizer. '
+                            'Could not find torch package.')  # pragma: no cover
```

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/keras/config_serialization.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/keras/config_serialization.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/keras/quantizer_utils.py` & `mct-nightly-1.8.0.9042023.post411/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/keras/quantizer_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9032023.post431/setup.py` & `mct-nightly-1.8.0.9042023.post411/setup.py`

 * *Files identical despite different names*

