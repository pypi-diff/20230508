# Comparing `tmp/flgo-0.0.3.tar.gz` & `tmp/flgo-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flgo-0.0.3.tar", last modified: Tue Mar 28 05:18:22 2023, max compression
+gzip compressed data, was "flgo-0.0.4.tar", last modified: Wed Mar 29 15:17:31 2023, max compression
```

## Comparing `flgo-0.0.3.tar` & `flgo-0.0.4.tar`

### file list

```diff
@@ -1,183 +1,183 @@
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-28 05:18:22.731575 flgo-0.0.3/
--rw-rw-r--   0 wz        (1001) wz        (1001)     1091 2023-03-21 13:46:37.000000 flgo-0.0.3/LICENSE
--rw-rw-r--   0 wz        (1001) wz        (1001)      486 2023-03-28 05:18:22.731575 flgo-0.0.3/PKG-INFO
--rw-rw-r--   0 wz        (1001) wz        (1001)        0 2023-03-21 13:46:37.000000 flgo-0.0.3/README.md
--rw-rw-r--   0 wz        (1001) wz        (1001)      591 2023-03-28 05:16:57.000000 flgo-0.0.3/pyproject.toml
--rw-rw-r--   0 wz        (1001) wz        (1001)       38 2023-03-28 05:18:22.731575 flgo-0.0.3/setup.cfg
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-28 05:18:22.719575 flgo-0.0.3/src/
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-28 05:18:22.719575 flgo-0.0.3/src/flgo/
--rw-rw-r--   0 wz        (1001) wz        (1001)      474 2023-03-28 05:15:37.000000 flgo-0.0.3/src/flgo/__init__.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-28 05:18:22.723575 flgo-0.0.3/src/flgo/algorithm/
--rw-rw-r--   0 wz        (1001) wz        (1001)     3744 2023-03-28 05:15:37.000000 flgo-0.0.3/src/flgo/algorithm/TiFL.py
--rw-rw-r--   0 wz        (1001) wz        (1001)        0 2023-03-28 05:15:37.000000 flgo-0.0.3/src/flgo/algorithm/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     3330 2023-03-28 05:15:37.000000 flgo-0.0.3/src/flgo/algorithm/afl.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     2208 2023-03-28 05:15:37.000000 flgo-0.0.3/src/flgo/algorithm/fedasync.py
--rw-rw-r--   0 wz        (1001) wz        (1001)       86 2023-03-28 05:15:37.000000 flgo-0.0.3/src/flgo/algorithm/fedavg.py
--rw-rw-r--   0 wz        (1001) wz        (1001)    26808 2023-03-28 05:15:37.000000 flgo-0.0.3/src/flgo/algorithm/fedbase.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     2554 2023-03-28 05:15:37.000000 flgo-0.0.3/src/flgo/algorithm/fedbuff.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     2690 2023-03-28 05:15:37.000000 flgo-0.0.3/src/flgo/algorithm/fedmgda+.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     1226 2023-03-28 05:15:37.000000 flgo-0.0.3/src/flgo/algorithm/fedprox.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     1800 2023-03-28 05:15:37.000000 flgo-0.0.3/src/flgo/algorithm/mifa.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     1485 2023-03-28 05:15:37.000000 flgo-0.0.3/src/flgo/algorithm/powerofchoice.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     1035 2023-03-28 05:15:37.000000 flgo-0.0.3/src/flgo/algorithm/qfedavg.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     3252 2023-03-28 05:15:37.000000 flgo-0.0.3/src/flgo/algorithm/scaffold.py
--rw-rw-r--   0 wz        (1001) wz        (1001)    11783 2023-03-28 05:15:37.000000 flgo-0.0.3/src/flgo/algorithm/vflbase.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-28 05:18:22.723575 flgo-0.0.3/src/flgo/benchmark/
--rw-rw-r--   0 wz        (1001) wz        (1001)       41 2023-03-28 05:15:37.000000 flgo-0.0.3/src/flgo/benchmark/__init__.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-28 05:18:22.723575 flgo-0.0.3/src/flgo/benchmark/cifar100_classification/
--rw-rw-r--   0 wz        (1001) wz        (1001)     1526 2023-03-28 05:15:38.000000 flgo-0.0.3/src/flgo/benchmark/cifar100_classification/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      845 2023-03-28 05:15:38.000000 flgo-0.0.3/src/flgo/benchmark/cifar100_classification/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-28 05:18:22.723575 flgo-0.0.3/src/flgo/benchmark/cifar100_classification/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      957 2023-03-28 05:15:39.000000 flgo-0.0.3/src/flgo/benchmark/cifar100_classification/model/cnn.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     5298 2023-03-28 05:15:39.000000 flgo-0.0.3/src/flgo/benchmark/cifar100_classification/model/resnet18.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-28 05:18:22.723575 flgo-0.0.3/src/flgo/benchmark/cifar10_classification/
--rw-rw-r--   0 wz        (1001) wz        (1001)     1690 2023-03-28 05:15:38.000000 flgo-0.0.3/src/flgo/benchmark/cifar10_classification/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      829 2023-03-28 05:15:38.000000 flgo-0.0.3/src/flgo/benchmark/cifar10_classification/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-28 05:18:22.723575 flgo-0.0.3/src/flgo/benchmark/cifar10_classification/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      895 2023-03-28 05:15:39.000000 flgo-0.0.3/src/flgo/benchmark/cifar10_classification/model/cnn.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      897 2023-03-28 05:15:39.000000 flgo-0.0.3/src/flgo/benchmark/cifar10_classification/model/mlp.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-28 05:18:22.723575 flgo-0.0.3/src/flgo/benchmark/citeseer_link_prediction/
--rw-rw-r--   0 wz        (1001) wz        (1001)       82 2023-03-28 05:15:38.000000 flgo-0.0.3/src/flgo/benchmark/citeseer_link_prediction/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      748 2023-03-28 05:15:38.000000 flgo-0.0.3/src/flgo/benchmark/citeseer_link_prediction/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-28 05:18:22.723575 flgo-0.0.3/src/flgo/benchmark/citeseer_link_prediction/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      825 2023-03-28 05:15:39.000000 flgo-0.0.3/src/flgo/benchmark/citeseer_link_prediction/model/GCN.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-28 05:18:22.723575 flgo-0.0.3/src/flgo/benchmark/citeseer_node_classification/
--rw-rw-r--   0 wz        (1001) wz        (1001)       86 2023-03-28 05:15:38.000000 flgo-0.0.3/src/flgo/benchmark/citeseer_node_classification/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      807 2023-03-28 05:15:38.000000 flgo-0.0.3/src/flgo/benchmark/citeseer_node_classification/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-28 05:18:22.723575 flgo-0.0.3/src/flgo/benchmark/citeseer_node_classification/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      727 2023-03-28 05:15:39.000000 flgo-0.0.3/src/flgo/benchmark/citeseer_node_classification/model/GCN.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-28 05:18:22.723575 flgo-0.0.3/src/flgo/benchmark/cora_link_prediction/
--rw-rw-r--   0 wz        (1001) wz        (1001)       78 2023-03-28 05:15:38.000000 flgo-0.0.3/src/flgo/benchmark/cora_link_prediction/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      736 2023-03-28 05:15:38.000000 flgo-0.0.3/src/flgo/benchmark/cora_link_prediction/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-28 05:18:22.723575 flgo-0.0.3/src/flgo/benchmark/cora_link_prediction/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      825 2023-03-28 05:15:39.000000 flgo-0.0.3/src/flgo/benchmark/cora_link_prediction/model/GCN.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-28 05:18:22.723575 flgo-0.0.3/src/flgo/benchmark/cora_node_classification/
--rw-rw-r--   0 wz        (1001) wz        (1001)       82 2023-03-28 05:15:38.000000 flgo-0.0.3/src/flgo/benchmark/cora_node_classification/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      794 2023-03-28 05:15:38.000000 flgo-0.0.3/src/flgo/benchmark/cora_node_classification/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-28 05:18:22.723575 flgo-0.0.3/src/flgo/benchmark/cora_node_classification/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      727 2023-03-28 05:15:39.000000 flgo-0.0.3/src/flgo/benchmark/cora_node_classification/model/GCN.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      730 2023-03-28 05:15:39.000000 flgo-0.0.3/src/flgo/benchmark/cora_node_classification/model/GraphSAGE_1.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     4070 2023-03-28 05:15:39.000000 flgo-0.0.3/src/flgo/benchmark/cora_node_classification/model/GraphSage.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-28 05:18:22.723575 flgo-0.0.3/src/flgo/benchmark/emnist_classification/
--rw-rw-r--   0 wz        (1001) wz        (1001)      195 2023-03-28 05:15:38.000000 flgo-0.0.3/src/flgo/benchmark/emnist_classification/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     1148 2023-03-28 05:15:38.000000 flgo-0.0.3/src/flgo/benchmark/emnist_classification/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-28 05:18:22.723575 flgo-0.0.3/src/flgo/benchmark/emnist_classification/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)     1037 2023-03-28 05:15:39.000000 flgo-0.0.3/src/flgo/benchmark/emnist_classification/model/cnn.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      709 2023-03-28 05:15:39.000000 flgo-0.0.3/src/flgo/benchmark/emnist_classification/model/mlp.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-28 05:18:22.723575 flgo-0.0.3/src/flgo/benchmark/enzymes_graph_classification/
--rw-rw-r--   0 wz        (1001) wz        (1001)       86 2023-03-28 05:15:38.000000 flgo-0.0.3/src/flgo/benchmark/enzymes_graph_classification/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      748 2023-03-28 05:15:38.000000 flgo-0.0.3/src/flgo/benchmark/enzymes_graph_classification/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-28 05:18:22.723575 flgo-0.0.3/src/flgo/benchmark/enzymes_graph_classification/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)     1258 2023-03-28 05:15:39.000000 flgo-0.0.3/src/flgo/benchmark/enzymes_graph_classification/model/GCN.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     1581 2023-03-28 05:15:39.000000 flgo-0.0.3/src/flgo/benchmark/enzymes_graph_classification/model/GIN.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-28 05:18:22.723575 flgo-0.0.3/src/flgo/benchmark/fashion_classification/
--rw-rw-r--   0 wz        (1001) wz        (1001)      194 2023-03-28 05:15:38.000000 flgo-0.0.3/src/flgo/benchmark/fashion_classification/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      818 2023-03-28 05:15:38.000000 flgo-0.0.3/src/flgo/benchmark/fashion_classification/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-28 05:18:22.723575 flgo-0.0.3/src/flgo/benchmark/fashion_classification/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      578 2023-03-28 05:15:39.000000 flgo-0.0.3/src/flgo/benchmark/fashion_classification/model/lr.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-28 05:18:22.723575 flgo-0.0.3/src/flgo/benchmark/femnist_classification/
--rw-rw-r--   0 wz        (1001) wz        (1001)        0 2023-03-28 05:15:38.000000 flgo-0.0.3/src/flgo/benchmark/femnist_classification/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     5750 2023-03-28 05:15:38.000000 flgo-0.0.3/src/flgo/benchmark/femnist_classification/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-28 05:18:22.723575 flgo-0.0.3/src/flgo/benchmark/leaf_reddit/
--rw-rw-r--   0 wz        (1001) wz        (1001)       87 2023-03-28 05:15:38.000000 flgo-0.0.3/src/flgo/benchmark/leaf_reddit/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)    10069 2023-03-28 05:15:38.000000 flgo-0.0.3/src/flgo/benchmark/leaf_reddit/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-28 05:18:22.723575 flgo-0.0.3/src/flgo/benchmark/leaf_reddit/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      980 2023-03-28 05:15:39.000000 flgo-0.0.3/src/flgo/benchmark/leaf_reddit/model/stackedlstm.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-28 05:18:22.723575 flgo-0.0.3/src/flgo/benchmark/leaf_sent140/
--rw-rw-r--   0 wz        (1001) wz        (1001)       86 2023-03-28 05:15:38.000000 flgo-0.0.3/src/flgo/benchmark/leaf_sent140/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)    11301 2023-03-28 05:15:38.000000 flgo-0.0.3/src/flgo/benchmark/leaf_sent140/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-28 05:18:22.723575 flgo-0.0.3/src/flgo/benchmark/leaf_sent140/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)     1278 2023-03-28 05:15:39.000000 flgo-0.0.3/src/flgo/benchmark/leaf_sent140/model/stackedlstm.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-28 05:18:22.727575 flgo-0.0.3/src/flgo/benchmark/mnist_classification/
--rw-rw-r--   0 wz        (1001) wz        (1001)     1668 2023-03-28 05:15:38.000000 flgo-0.0.3/src/flgo/benchmark/mnist_classification/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      809 2023-03-28 05:15:38.000000 flgo-0.0.3/src/flgo/benchmark/mnist_classification/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-28 05:18:22.727575 flgo-0.0.3/src/flgo/benchmark/mnist_classification/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)     1031 2023-03-28 05:15:39.000000 flgo-0.0.3/src/flgo/benchmark/mnist_classification/model/cnn.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      801 2023-03-28 05:15:39.000000 flgo-0.0.3/src/flgo/benchmark/mnist_classification/model/mlp.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-28 05:18:22.727575 flgo-0.0.3/src/flgo/benchmark/mutag_graph_classification/
--rw-rw-r--   0 wz        (1001) wz        (1001)       84 2023-03-28 05:15:38.000000 flgo-0.0.3/src/flgo/benchmark/mutag_graph_classification/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      742 2023-03-28 05:15:38.000000 flgo-0.0.3/src/flgo/benchmark/mutag_graph_classification/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-28 05:18:22.727575 flgo-0.0.3/src/flgo/benchmark/mutag_graph_classification/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)     1260 2023-03-28 05:15:39.000000 flgo-0.0.3/src/flgo/benchmark/mutag_graph_classification/model/GCN.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-28 05:18:22.727575 flgo-0.0.3/src/flgo/benchmark/pubmed_link_prediction/
--rw-rw-r--   0 wz        (1001) wz        (1001)       80 2023-03-28 05:15:38.000000 flgo-0.0.3/src/flgo/benchmark/pubmed_link_prediction/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      742 2023-03-28 05:15:38.000000 flgo-0.0.3/src/flgo/benchmark/pubmed_link_prediction/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-28 05:18:22.727575 flgo-0.0.3/src/flgo/benchmark/pubmed_link_prediction/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      824 2023-03-28 05:15:39.000000 flgo-0.0.3/src/flgo/benchmark/pubmed_link_prediction/model/GCN.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-28 05:18:22.727575 flgo-0.0.3/src/flgo/benchmark/pubmed_node_classification/
--rw-rw-r--   0 wz        (1001) wz        (1001)       84 2023-03-28 05:15:38.000000 flgo-0.0.3/src/flgo/benchmark/pubmed_node_classification/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      801 2023-03-28 05:15:38.000000 flgo-0.0.3/src/flgo/benchmark/pubmed_node_classification/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-28 05:18:22.727575 flgo-0.0.3/src/flgo/benchmark/pubmed_node_classification/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      726 2023-03-28 05:15:39.000000 flgo-0.0.3/src/flgo/benchmark/pubmed_node_classification/model/GCN.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-28 05:18:22.727575 flgo-0.0.3/src/flgo/benchmark/shakespeare_classification/
--rw-rw-r--   0 wz        (1001) wz        (1001)      100 2023-03-28 05:15:38.000000 flgo-0.0.3/src/flgo/benchmark/shakespeare_classification/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)    15287 2023-03-28 05:15:38.000000 flgo-0.0.3/src/flgo/benchmark/shakespeare_classification/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-28 05:18:22.727575 flgo-0.0.3/src/flgo/benchmark/shakespeare_classification/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)     2169 2023-03-28 05:15:39.000000 flgo-0.0.3/src/flgo/benchmark/shakespeare_classification/model/stackedlstm.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-28 05:18:22.727575 flgo-0.0.3/src/flgo/benchmark/synthetic_regression/
--rw-rw-r--   0 wz        (1001) wz        (1001)       76 2023-03-28 05:15:38.000000 flgo-0.0.3/src/flgo/benchmark/synthetic_regression/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     3927 2023-03-28 05:15:38.000000 flgo-0.0.3/src/flgo/benchmark/synthetic_regression/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-28 05:18:22.727575 flgo-0.0.3/src/flgo/benchmark/synthetic_regression/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      555 2023-03-28 05:15:39.000000 flgo-0.0.3/src/flgo/benchmark/synthetic_regression/model/lr.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-28 05:18:22.727575 flgo-0.0.3/src/flgo/benchmark/toolkits/
--rw-rw-r--   0 wz        (1001) wz        (1001)      108 2023-03-28 05:15:38.000000 flgo-0.0.3/src/flgo/benchmark/toolkits/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)    12872 2023-03-28 05:15:38.000000 flgo-0.0.3/src/flgo/benchmark/toolkits/base.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-28 05:18:22.727575 flgo-0.0.3/src/flgo/benchmark/toolkits/cv/
--rw-rw-r--   0 wz        (1001) wz        (1001)        0 2023-03-28 05:15:39.000000 flgo-0.0.3/src/flgo/benchmark/toolkits/cv/__init__.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-28 05:18:22.727575 flgo-0.0.3/src/flgo/benchmark/toolkits/cv/centralize/
--rw-rw-r--   0 wz        (1001) wz        (1001)        0 2023-03-28 05:15:39.000000 flgo-0.0.3/src/flgo/benchmark/toolkits/cv/centralize/__init__.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-28 05:18:22.727575 flgo-0.0.3/src/flgo/benchmark/toolkits/cv/horizontal/
--rw-rw-r--   0 wz        (1001) wz        (1001)        0 2023-03-28 05:15:39.000000 flgo-0.0.3/src/flgo/benchmark/toolkits/cv/horizontal/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     6442 2023-03-28 05:15:39.000000 flgo-0.0.3/src/flgo/benchmark/toolkits/cv/horizontal/image_classification.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-28 05:18:22.727575 flgo-0.0.3/src/flgo/benchmark/toolkits/cv/vertical/
--rw-rw-r--   0 wz        (1001) wz        (1001)        0 2023-03-28 05:15:39.000000 flgo-0.0.3/src/flgo/benchmark/toolkits/cv/vertical/__init__.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-28 05:18:22.727575 flgo-0.0.3/src/flgo/benchmark/toolkits/graph/
--rw-rw-r--   0 wz        (1001) wz        (1001)        0 2023-03-28 05:15:39.000000 flgo-0.0.3/src/flgo/benchmark/toolkits/graph/__init__.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-28 05:18:22.727575 flgo-0.0.3/src/flgo/benchmark/toolkits/graph/horizontal/
--rw-rw-r--   0 wz        (1001) wz        (1001)        0 2023-03-28 05:15:39.000000 flgo-0.0.3/src/flgo/benchmark/toolkits/graph/horizontal/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     5621 2023-03-28 05:15:39.000000 flgo-0.0.3/src/flgo/benchmark/toolkits/graph/horizontal/graph_classification.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     7709 2023-03-28 05:15:39.000000 flgo-0.0.3/src/flgo/benchmark/toolkits/graph/horizontal/link_prediction.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     7346 2023-03-28 05:15:39.000000 flgo-0.0.3/src/flgo/benchmark/toolkits/graph/horizontal/node_classification.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-28 05:18:22.727575 flgo-0.0.3/src/flgo/benchmark/toolkits/nlp/
--rw-rw-r--   0 wz        (1001) wz        (1001)        0 2023-03-28 05:15:39.000000 flgo-0.0.3/src/flgo/benchmark/toolkits/nlp/__init__.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-28 05:18:22.727575 flgo-0.0.3/src/flgo/benchmark/toolkits/nlp/horizontal/
--rw-rw-r--   0 wz        (1001) wz        (1001)        0 2023-03-28 05:15:39.000000 flgo-0.0.3/src/flgo/benchmark/toolkits/nlp/horizontal/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)        0 2023-03-28 05:15:39.000000 flgo-0.0.3/src/flgo/benchmark/toolkits/nlp/horizontal/text_prediction.py
--rw-rw-r--   0 wz        (1001) wz        (1001)    19844 2023-03-28 05:15:38.000000 flgo-0.0.3/src/flgo/benchmark/toolkits/partition.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-28 05:18:22.727575 flgo-0.0.3/src/flgo/benchmark/toolkits/tabular/
--rw-rw-r--   0 wz        (1001) wz        (1001)        0 2023-03-28 05:15:39.000000 flgo-0.0.3/src/flgo/benchmark/toolkits/tabular/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     2085 2023-03-28 05:15:38.000000 flgo-0.0.3/src/flgo/benchmark/toolkits/visualization.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-28 05:18:22.727575 flgo-0.0.3/src/flgo/benchmark/vertical_mnist_classification/
--rw-rw-r--   0 wz        (1001) wz        (1001)       87 2023-03-28 05:15:38.000000 flgo-0.0.3/src/flgo/benchmark/vertical_mnist_classification/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     7198 2023-03-28 05:15:38.000000 flgo-0.0.3/src/flgo/benchmark/vertical_mnist_classification/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-28 05:18:22.727575 flgo-0.0.3/src/flgo/benchmark/vertical_mnist_classification/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)     1162 2023-03-28 05:15:39.000000 flgo-0.0.3/src/flgo/benchmark/vertical_mnist_classification/model/mlp.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-28 05:18:22.727575 flgo-0.0.3/src/flgo/experiment/
--rw-rw-r--   0 wz        (1001) wz        (1001)        0 2023-03-28 05:15:38.000000 flgo-0.0.3/src/flgo/experiment/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)    19947 2023-03-28 05:15:38.000000 flgo-0.0.3/src/flgo/experiment/analyzer.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     4344 2023-03-28 05:15:38.000000 flgo-0.0.3/src/flgo/experiment/device_scheduler.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-28 05:18:22.727575 flgo-0.0.3/src/flgo/experiment/logger/
--rw-rw-r--   0 wz        (1001) wz        (1001)    87090 2023-03-28 05:15:39.000000 flgo-0.0.3/src/flgo/experiment/logger/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)    36840 2023-03-28 05:15:38.000000 flgo-0.0.3/src/flgo/experiment/logger/config.py
--rw-rw-r--   0 wz        (1001) wz        (1001)    59395 2023-03-28 05:15:38.000000 flgo-0.0.3/src/flgo/experiment/logger/handlers.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     1485 2023-03-28 05:15:38.000000 flgo-0.0.3/src/flgo/experiment/logger/simple_logger.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     1077 2023-03-28 05:15:39.000000 flgo-0.0.3/src/flgo/experiment/logger/tune_logger.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      959 2023-03-28 05:15:39.000000 flgo-0.0.3/src/flgo/experiment/logger/vertical_logger.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     8668 2023-03-28 05:15:38.000000 flgo-0.0.3/src/flgo/experiment/runner.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-28 05:18:22.731575 flgo-0.0.3/src/flgo/system_simulator/
--rw-rw-r--   0 wz        (1001) wz        (1001)     3016 2023-03-28 05:15:38.000000 flgo-0.0.3/src/flgo/system_simulator/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)    18458 2023-03-28 05:15:38.000000 flgo-0.0.3/src/flgo/system_simulator/base.py
--rw-rw-r--   0 wz        (1001) wz        (1001)    15544 2023-03-28 05:15:38.000000 flgo-0.0.3/src/flgo/system_simulator/default_simulator.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     1037 2023-03-28 05:15:38.000000 flgo-0.0.3/src/flgo/system_simulator/my_simulator.py
--rw-rw-r--   0 wz        (1001) wz        (1001)    17529 2023-03-28 05:15:38.000000 flgo-0.0.3/src/flgo/system_simulator/phone_simulator.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-28 05:18:22.731575 flgo-0.0.3/src/flgo/utils/
--rw-rw-r--   0 wz        (1001) wz        (1001)        0 2023-03-28 05:15:38.000000 flgo-0.0.3/src/flgo/utils/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)    38670 2023-03-28 05:15:38.000000 flgo-0.0.3/src/flgo/utils/fflow.py
--rw-rw-r--   0 wz        (1001) wz        (1001)    16169 2023-03-28 05:15:38.000000 flgo-0.0.3/src/flgo/utils/fmodule.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-28 05:18:22.719575 flgo-0.0.3/src/flgo.egg-info/
--rw-rw-r--   0 wz        (1001) wz        (1001)      486 2023-03-28 05:18:22.000000 flgo-0.0.3/src/flgo.egg-info/PKG-INFO
--rw-rw-r--   0 wz        (1001) wz        (1001)     5677 2023-03-28 05:18:22.000000 flgo-0.0.3/src/flgo.egg-info/SOURCES.txt
--rw-rw-r--   0 wz        (1001) wz        (1001)        1 2023-03-28 05:18:22.000000 flgo-0.0.3/src/flgo.egg-info/dependency_links.txt
--rw-rw-r--   0 wz        (1001) wz        (1001)        5 2023-03-28 05:18:22.000000 flgo-0.0.3/src/flgo.egg-info/top_level.txt
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-28 05:18:22.731575 flgo-0.0.3/tests/
--rw-rw-r--   0 wz        (1001) wz        (1001)      947 2023-03-21 13:46:37.000000 flgo-0.0.3/tests/test.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-29 15:17:31.924306 flgo-0.0.4/
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1091 2023-03-21 13:46:37.000000 flgo-0.0.4/LICENSE
+-rw-rw-r--   0 wz        (1001) wz        (1001)      486 2023-03-29 15:17:31.924306 flgo-0.0.4/PKG-INFO
+-rw-rw-r--   0 wz        (1001) wz        (1001)        0 2023-03-21 13:46:37.000000 flgo-0.0.4/README.md
+-rw-rw-r--   0 wz        (1001) wz        (1001)      591 2023-03-29 15:14:22.000000 flgo-0.0.4/pyproject.toml
+-rw-rw-r--   0 wz        (1001) wz        (1001)       38 2023-03-29 15:17:31.924306 flgo-0.0.4/setup.cfg
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-29 15:17:31.904306 flgo-0.0.4/src/
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-29 15:17:31.908306 flgo-0.0.4/src/flgo/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      474 2023-03-29 15:13:14.000000 flgo-0.0.4/src/flgo/__init__.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-29 15:17:31.912306 flgo-0.0.4/src/flgo/algorithm/
+-rw-rw-r--   0 wz        (1001) wz        (1001)     3744 2023-03-29 15:13:14.000000 flgo-0.0.4/src/flgo/algorithm/TiFL.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)        0 2023-03-29 15:13:15.000000 flgo-0.0.4/src/flgo/algorithm/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     3322 2023-03-29 15:13:14.000000 flgo-0.0.4/src/flgo/algorithm/afl.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     2208 2023-03-29 15:13:14.000000 flgo-0.0.4/src/flgo/algorithm/fedasync.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)       86 2023-03-29 15:13:14.000000 flgo-0.0.4/src/flgo/algorithm/fedavg.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)    26968 2023-03-29 15:13:14.000000 flgo-0.0.4/src/flgo/algorithm/fedbase.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     2554 2023-03-29 15:13:14.000000 flgo-0.0.4/src/flgo/algorithm/fedbuff.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     2690 2023-03-29 15:13:14.000000 flgo-0.0.4/src/flgo/algorithm/fedmgda+.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1226 2023-03-29 15:13:14.000000 flgo-0.0.4/src/flgo/algorithm/fedprox.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1800 2023-03-29 15:13:14.000000 flgo-0.0.4/src/flgo/algorithm/mifa.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1485 2023-03-29 15:13:14.000000 flgo-0.0.4/src/flgo/algorithm/powerofchoice.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1035 2023-03-29 15:13:14.000000 flgo-0.0.4/src/flgo/algorithm/qfedavg.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     3252 2023-03-29 15:13:14.000000 flgo-0.0.4/src/flgo/algorithm/scaffold.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)    11783 2023-03-29 15:13:14.000000 flgo-0.0.4/src/flgo/algorithm/vflbase.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-29 15:17:31.912306 flgo-0.0.4/src/flgo/benchmark/
+-rw-rw-r--   0 wz        (1001) wz        (1001)       41 2023-03-29 15:13:15.000000 flgo-0.0.4/src/flgo/benchmark/__init__.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-29 15:17:31.912306 flgo-0.0.4/src/flgo/benchmark/cifar100_classification/
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1526 2023-03-29 15:13:15.000000 flgo-0.0.4/src/flgo/benchmark/cifar100_classification/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      845 2023-03-29 15:13:15.000000 flgo-0.0.4/src/flgo/benchmark/cifar100_classification/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-29 15:17:31.912306 flgo-0.0.4/src/flgo/benchmark/cifar100_classification/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      957 2023-03-29 15:13:16.000000 flgo-0.0.4/src/flgo/benchmark/cifar100_classification/model/cnn.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     5298 2023-03-29 15:13:16.000000 flgo-0.0.4/src/flgo/benchmark/cifar100_classification/model/resnet18.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-29 15:17:31.912306 flgo-0.0.4/src/flgo/benchmark/cifar10_classification/
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1690 2023-03-29 15:13:15.000000 flgo-0.0.4/src/flgo/benchmark/cifar10_classification/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      829 2023-03-29 15:13:15.000000 flgo-0.0.4/src/flgo/benchmark/cifar10_classification/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-29 15:17:31.912306 flgo-0.0.4/src/flgo/benchmark/cifar10_classification/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      895 2023-03-29 15:13:16.000000 flgo-0.0.4/src/flgo/benchmark/cifar10_classification/model/cnn.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      897 2023-03-29 15:13:16.000000 flgo-0.0.4/src/flgo/benchmark/cifar10_classification/model/mlp.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-29 15:17:31.912306 flgo-0.0.4/src/flgo/benchmark/citeseer_link_prediction/
+-rw-rw-r--   0 wz        (1001) wz        (1001)       82 2023-03-29 15:13:15.000000 flgo-0.0.4/src/flgo/benchmark/citeseer_link_prediction/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      748 2023-03-29 15:13:15.000000 flgo-0.0.4/src/flgo/benchmark/citeseer_link_prediction/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-29 15:17:31.912306 flgo-0.0.4/src/flgo/benchmark/citeseer_link_prediction/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      825 2023-03-29 15:13:16.000000 flgo-0.0.4/src/flgo/benchmark/citeseer_link_prediction/model/GCN.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-29 15:17:31.916306 flgo-0.0.4/src/flgo/benchmark/citeseer_node_classification/
+-rw-rw-r--   0 wz        (1001) wz        (1001)       86 2023-03-29 15:13:15.000000 flgo-0.0.4/src/flgo/benchmark/citeseer_node_classification/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      807 2023-03-29 15:13:15.000000 flgo-0.0.4/src/flgo/benchmark/citeseer_node_classification/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-29 15:17:31.916306 flgo-0.0.4/src/flgo/benchmark/citeseer_node_classification/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      727 2023-03-29 15:13:16.000000 flgo-0.0.4/src/flgo/benchmark/citeseer_node_classification/model/GCN.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-29 15:17:31.916306 flgo-0.0.4/src/flgo/benchmark/cora_link_prediction/
+-rw-rw-r--   0 wz        (1001) wz        (1001)       78 2023-03-29 15:13:15.000000 flgo-0.0.4/src/flgo/benchmark/cora_link_prediction/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      736 2023-03-29 15:13:15.000000 flgo-0.0.4/src/flgo/benchmark/cora_link_prediction/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-29 15:17:31.916306 flgo-0.0.4/src/flgo/benchmark/cora_link_prediction/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      825 2023-03-29 15:13:16.000000 flgo-0.0.4/src/flgo/benchmark/cora_link_prediction/model/GCN.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-29 15:17:31.916306 flgo-0.0.4/src/flgo/benchmark/cora_node_classification/
+-rw-rw-r--   0 wz        (1001) wz        (1001)       82 2023-03-29 15:13:15.000000 flgo-0.0.4/src/flgo/benchmark/cora_node_classification/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      794 2023-03-29 15:13:15.000000 flgo-0.0.4/src/flgo/benchmark/cora_node_classification/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-29 15:17:31.916306 flgo-0.0.4/src/flgo/benchmark/cora_node_classification/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      727 2023-03-29 15:13:16.000000 flgo-0.0.4/src/flgo/benchmark/cora_node_classification/model/GCN.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      730 2023-03-29 15:13:16.000000 flgo-0.0.4/src/flgo/benchmark/cora_node_classification/model/GraphSAGE_1.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     4070 2023-03-29 15:13:16.000000 flgo-0.0.4/src/flgo/benchmark/cora_node_classification/model/GraphSage.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-29 15:17:31.916306 flgo-0.0.4/src/flgo/benchmark/emnist_classification/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      195 2023-03-29 15:13:15.000000 flgo-0.0.4/src/flgo/benchmark/emnist_classification/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1148 2023-03-29 15:13:15.000000 flgo-0.0.4/src/flgo/benchmark/emnist_classification/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-29 15:17:31.916306 flgo-0.0.4/src/flgo/benchmark/emnist_classification/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1037 2023-03-29 15:13:16.000000 flgo-0.0.4/src/flgo/benchmark/emnist_classification/model/cnn.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      709 2023-03-29 15:13:16.000000 flgo-0.0.4/src/flgo/benchmark/emnist_classification/model/mlp.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-29 15:17:31.916306 flgo-0.0.4/src/flgo/benchmark/enzymes_graph_classification/
+-rw-rw-r--   0 wz        (1001) wz        (1001)       86 2023-03-29 15:13:15.000000 flgo-0.0.4/src/flgo/benchmark/enzymes_graph_classification/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      748 2023-03-29 15:13:15.000000 flgo-0.0.4/src/flgo/benchmark/enzymes_graph_classification/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-29 15:17:31.916306 flgo-0.0.4/src/flgo/benchmark/enzymes_graph_classification/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1258 2023-03-29 15:13:16.000000 flgo-0.0.4/src/flgo/benchmark/enzymes_graph_classification/model/GCN.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1581 2023-03-29 15:13:16.000000 flgo-0.0.4/src/flgo/benchmark/enzymes_graph_classification/model/GIN.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-29 15:17:31.916306 flgo-0.0.4/src/flgo/benchmark/fashion_classification/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      194 2023-03-29 15:13:15.000000 flgo-0.0.4/src/flgo/benchmark/fashion_classification/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      818 2023-03-29 15:13:15.000000 flgo-0.0.4/src/flgo/benchmark/fashion_classification/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-29 15:17:31.916306 flgo-0.0.4/src/flgo/benchmark/fashion_classification/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      578 2023-03-29 15:13:16.000000 flgo-0.0.4/src/flgo/benchmark/fashion_classification/model/lr.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-29 15:17:31.916306 flgo-0.0.4/src/flgo/benchmark/femnist_classification/
+-rw-rw-r--   0 wz        (1001) wz        (1001)        0 2023-03-29 15:13:15.000000 flgo-0.0.4/src/flgo/benchmark/femnist_classification/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     5750 2023-03-29 15:13:15.000000 flgo-0.0.4/src/flgo/benchmark/femnist_classification/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-29 15:17:31.916306 flgo-0.0.4/src/flgo/benchmark/leaf_reddit/
+-rw-rw-r--   0 wz        (1001) wz        (1001)       87 2023-03-29 15:13:15.000000 flgo-0.0.4/src/flgo/benchmark/leaf_reddit/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)    10069 2023-03-29 15:13:15.000000 flgo-0.0.4/src/flgo/benchmark/leaf_reddit/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-29 15:17:31.916306 flgo-0.0.4/src/flgo/benchmark/leaf_reddit/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      980 2023-03-29 15:13:16.000000 flgo-0.0.4/src/flgo/benchmark/leaf_reddit/model/stackedlstm.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-29 15:17:31.916306 flgo-0.0.4/src/flgo/benchmark/leaf_sent140/
+-rw-rw-r--   0 wz        (1001) wz        (1001)       86 2023-03-29 15:13:15.000000 flgo-0.0.4/src/flgo/benchmark/leaf_sent140/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)    11301 2023-03-29 15:13:15.000000 flgo-0.0.4/src/flgo/benchmark/leaf_sent140/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-29 15:17:31.916306 flgo-0.0.4/src/flgo/benchmark/leaf_sent140/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1278 2023-03-29 15:13:16.000000 flgo-0.0.4/src/flgo/benchmark/leaf_sent140/model/stackedlstm.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-29 15:17:31.916306 flgo-0.0.4/src/flgo/benchmark/mnist_classification/
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1668 2023-03-29 15:13:15.000000 flgo-0.0.4/src/flgo/benchmark/mnist_classification/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      809 2023-03-29 15:13:15.000000 flgo-0.0.4/src/flgo/benchmark/mnist_classification/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-29 15:17:31.916306 flgo-0.0.4/src/flgo/benchmark/mnist_classification/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1031 2023-03-29 15:13:16.000000 flgo-0.0.4/src/flgo/benchmark/mnist_classification/model/cnn.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      801 2023-03-29 15:13:16.000000 flgo-0.0.4/src/flgo/benchmark/mnist_classification/model/mlp.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-29 15:17:31.920306 flgo-0.0.4/src/flgo/benchmark/mutag_graph_classification/
+-rw-rw-r--   0 wz        (1001) wz        (1001)       84 2023-03-29 15:13:15.000000 flgo-0.0.4/src/flgo/benchmark/mutag_graph_classification/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      742 2023-03-29 15:13:15.000000 flgo-0.0.4/src/flgo/benchmark/mutag_graph_classification/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-29 15:17:31.920306 flgo-0.0.4/src/flgo/benchmark/mutag_graph_classification/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1260 2023-03-29 15:13:16.000000 flgo-0.0.4/src/flgo/benchmark/mutag_graph_classification/model/GCN.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-29 15:17:31.920306 flgo-0.0.4/src/flgo/benchmark/pubmed_link_prediction/
+-rw-rw-r--   0 wz        (1001) wz        (1001)       80 2023-03-29 15:13:15.000000 flgo-0.0.4/src/flgo/benchmark/pubmed_link_prediction/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      742 2023-03-29 15:13:15.000000 flgo-0.0.4/src/flgo/benchmark/pubmed_link_prediction/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-29 15:17:31.920306 flgo-0.0.4/src/flgo/benchmark/pubmed_link_prediction/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      824 2023-03-29 15:13:16.000000 flgo-0.0.4/src/flgo/benchmark/pubmed_link_prediction/model/GCN.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-29 15:17:31.920306 flgo-0.0.4/src/flgo/benchmark/pubmed_node_classification/
+-rw-rw-r--   0 wz        (1001) wz        (1001)       84 2023-03-29 15:13:15.000000 flgo-0.0.4/src/flgo/benchmark/pubmed_node_classification/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      801 2023-03-29 15:13:15.000000 flgo-0.0.4/src/flgo/benchmark/pubmed_node_classification/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-29 15:17:31.920306 flgo-0.0.4/src/flgo/benchmark/pubmed_node_classification/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      726 2023-03-29 15:13:16.000000 flgo-0.0.4/src/flgo/benchmark/pubmed_node_classification/model/GCN.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-29 15:17:31.920306 flgo-0.0.4/src/flgo/benchmark/shakespeare_classification/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      100 2023-03-29 15:13:15.000000 flgo-0.0.4/src/flgo/benchmark/shakespeare_classification/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)    15287 2023-03-29 15:13:15.000000 flgo-0.0.4/src/flgo/benchmark/shakespeare_classification/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-29 15:17:31.920306 flgo-0.0.4/src/flgo/benchmark/shakespeare_classification/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)     2169 2023-03-29 15:13:16.000000 flgo-0.0.4/src/flgo/benchmark/shakespeare_classification/model/stackedlstm.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-29 15:17:31.920306 flgo-0.0.4/src/flgo/benchmark/synthetic_regression/
+-rw-rw-r--   0 wz        (1001) wz        (1001)       76 2023-03-29 15:13:15.000000 flgo-0.0.4/src/flgo/benchmark/synthetic_regression/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     3927 2023-03-29 15:13:15.000000 flgo-0.0.4/src/flgo/benchmark/synthetic_regression/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-29 15:17:31.920306 flgo-0.0.4/src/flgo/benchmark/synthetic_regression/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      555 2023-03-29 15:13:16.000000 flgo-0.0.4/src/flgo/benchmark/synthetic_regression/model/lr.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-29 15:17:31.920306 flgo-0.0.4/src/flgo/benchmark/toolkits/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      108 2023-03-29 15:13:15.000000 flgo-0.0.4/src/flgo/benchmark/toolkits/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)    12872 2023-03-29 15:13:15.000000 flgo-0.0.4/src/flgo/benchmark/toolkits/base.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-29 15:17:31.920306 flgo-0.0.4/src/flgo/benchmark/toolkits/cv/
+-rw-rw-r--   0 wz        (1001) wz        (1001)        0 2023-03-29 15:13:16.000000 flgo-0.0.4/src/flgo/benchmark/toolkits/cv/__init__.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-29 15:17:31.920306 flgo-0.0.4/src/flgo/benchmark/toolkits/cv/centralize/
+-rw-rw-r--   0 wz        (1001) wz        (1001)        0 2023-03-29 15:13:16.000000 flgo-0.0.4/src/flgo/benchmark/toolkits/cv/centralize/__init__.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-29 15:17:31.920306 flgo-0.0.4/src/flgo/benchmark/toolkits/cv/horizontal/
+-rw-rw-r--   0 wz        (1001) wz        (1001)        0 2023-03-29 15:13:16.000000 flgo-0.0.4/src/flgo/benchmark/toolkits/cv/horizontal/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     6479 2023-03-29 15:13:16.000000 flgo-0.0.4/src/flgo/benchmark/toolkits/cv/horizontal/image_classification.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-29 15:17:31.920306 flgo-0.0.4/src/flgo/benchmark/toolkits/cv/vertical/
+-rw-rw-r--   0 wz        (1001) wz        (1001)        0 2023-03-29 15:13:16.000000 flgo-0.0.4/src/flgo/benchmark/toolkits/cv/vertical/__init__.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-29 15:17:31.920306 flgo-0.0.4/src/flgo/benchmark/toolkits/graph/
+-rw-rw-r--   0 wz        (1001) wz        (1001)        0 2023-03-29 15:13:16.000000 flgo-0.0.4/src/flgo/benchmark/toolkits/graph/__init__.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-29 15:17:31.920306 flgo-0.0.4/src/flgo/benchmark/toolkits/graph/horizontal/
+-rw-rw-r--   0 wz        (1001) wz        (1001)        0 2023-03-29 15:13:16.000000 flgo-0.0.4/src/flgo/benchmark/toolkits/graph/horizontal/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     5621 2023-03-29 15:13:16.000000 flgo-0.0.4/src/flgo/benchmark/toolkits/graph/horizontal/graph_classification.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     7709 2023-03-29 15:13:16.000000 flgo-0.0.4/src/flgo/benchmark/toolkits/graph/horizontal/link_prediction.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     7346 2023-03-29 15:13:16.000000 flgo-0.0.4/src/flgo/benchmark/toolkits/graph/horizontal/node_classification.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-29 15:17:31.920306 flgo-0.0.4/src/flgo/benchmark/toolkits/nlp/
+-rw-rw-r--   0 wz        (1001) wz        (1001)        0 2023-03-29 15:13:16.000000 flgo-0.0.4/src/flgo/benchmark/toolkits/nlp/__init__.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-29 15:17:31.920306 flgo-0.0.4/src/flgo/benchmark/toolkits/nlp/horizontal/
+-rw-rw-r--   0 wz        (1001) wz        (1001)        0 2023-03-29 15:13:16.000000 flgo-0.0.4/src/flgo/benchmark/toolkits/nlp/horizontal/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)        0 2023-03-29 15:13:16.000000 flgo-0.0.4/src/flgo/benchmark/toolkits/nlp/horizontal/text_prediction.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)    19844 2023-03-29 15:13:15.000000 flgo-0.0.4/src/flgo/benchmark/toolkits/partition.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-29 15:17:31.920306 flgo-0.0.4/src/flgo/benchmark/toolkits/tabular/
+-rw-rw-r--   0 wz        (1001) wz        (1001)        0 2023-03-29 15:13:16.000000 flgo-0.0.4/src/flgo/benchmark/toolkits/tabular/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     2085 2023-03-29 15:13:15.000000 flgo-0.0.4/src/flgo/benchmark/toolkits/visualization.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-29 15:17:31.920306 flgo-0.0.4/src/flgo/benchmark/vertical_mnist_classification/
+-rw-rw-r--   0 wz        (1001) wz        (1001)       87 2023-03-29 15:13:15.000000 flgo-0.0.4/src/flgo/benchmark/vertical_mnist_classification/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     7198 2023-03-29 15:13:15.000000 flgo-0.0.4/src/flgo/benchmark/vertical_mnist_classification/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-29 15:17:31.920306 flgo-0.0.4/src/flgo/benchmark/vertical_mnist_classification/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1162 2023-03-29 15:13:16.000000 flgo-0.0.4/src/flgo/benchmark/vertical_mnist_classification/model/mlp.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-29 15:17:31.920306 flgo-0.0.4/src/flgo/experiment/
+-rw-rw-r--   0 wz        (1001) wz        (1001)        0 2023-03-29 15:13:15.000000 flgo-0.0.4/src/flgo/experiment/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)    20163 2023-03-29 15:13:15.000000 flgo-0.0.4/src/flgo/experiment/analyzer.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     4344 2023-03-29 15:13:15.000000 flgo-0.0.4/src/flgo/experiment/device_scheduler.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-29 15:17:31.924306 flgo-0.0.4/src/flgo/experiment/logger/
+-rw-rw-r--   0 wz        (1001) wz        (1001)    87090 2023-03-29 15:13:16.000000 flgo-0.0.4/src/flgo/experiment/logger/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)    36840 2023-03-29 15:13:15.000000 flgo-0.0.4/src/flgo/experiment/logger/config.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)    59395 2023-03-29 15:13:15.000000 flgo-0.0.4/src/flgo/experiment/logger/handlers.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1485 2023-03-29 15:13:16.000000 flgo-0.0.4/src/flgo/experiment/logger/simple_logger.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1077 2023-03-29 15:13:16.000000 flgo-0.0.4/src/flgo/experiment/logger/tune_logger.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      959 2023-03-29 15:13:16.000000 flgo-0.0.4/src/flgo/experiment/logger/vertical_logger.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     8668 2023-03-29 15:13:15.000000 flgo-0.0.4/src/flgo/experiment/runner.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-29 15:17:31.924306 flgo-0.0.4/src/flgo/system_simulator/
+-rw-rw-r--   0 wz        (1001) wz        (1001)     3016 2023-03-29 15:13:15.000000 flgo-0.0.4/src/flgo/system_simulator/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)    18458 2023-03-29 15:13:15.000000 flgo-0.0.4/src/flgo/system_simulator/base.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)    15544 2023-03-29 15:13:15.000000 flgo-0.0.4/src/flgo/system_simulator/default_simulator.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1037 2023-03-29 15:13:15.000000 flgo-0.0.4/src/flgo/system_simulator/my_simulator.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)    17529 2023-03-29 15:13:15.000000 flgo-0.0.4/src/flgo/system_simulator/phone_simulator.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-29 15:17:31.924306 flgo-0.0.4/src/flgo/utils/
+-rw-rw-r--   0 wz        (1001) wz        (1001)        0 2023-03-29 15:13:15.000000 flgo-0.0.4/src/flgo/utils/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)    38807 2023-03-29 15:13:15.000000 flgo-0.0.4/src/flgo/utils/fflow.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)    16169 2023-03-29 15:13:15.000000 flgo-0.0.4/src/flgo/utils/fmodule.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-29 15:17:31.912306 flgo-0.0.4/src/flgo.egg-info/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      486 2023-03-29 15:17:31.000000 flgo-0.0.4/src/flgo.egg-info/PKG-INFO
+-rw-rw-r--   0 wz        (1001) wz        (1001)     5677 2023-03-29 15:17:31.000000 flgo-0.0.4/src/flgo.egg-info/SOURCES.txt
+-rw-rw-r--   0 wz        (1001) wz        (1001)        1 2023-03-29 15:17:31.000000 flgo-0.0.4/src/flgo.egg-info/dependency_links.txt
+-rw-rw-r--   0 wz        (1001) wz        (1001)        5 2023-03-29 15:17:31.000000 flgo-0.0.4/src/flgo.egg-info/top_level.txt
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-03-29 15:17:31.924306 flgo-0.0.4/tests/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      947 2023-03-21 13:46:37.000000 flgo-0.0.4/tests/test.py
```

### Comparing `flgo-0.0.3/LICENSE` & `flgo-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `flgo-0.0.3/pyproject.toml` & `flgo-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "setuptools>=61.0", 
 ]
 build-backend = "setuptools.build_meta"
 [project]
 name = "flgo"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Zheng Wang", email="zwang@stu.xmu.edu.cn" },
 ]
 description = "A Research-oriented FL Platform. "
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `flgo-0.0.3/src/flgo/algorithm/TiFL.py` & `flgo-0.0.4/src/flgo/algorithm/TiFL.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.3/src/flgo/algorithm/afl.py` & `flgo-0.0.4/src/flgo/algorithm/afl.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,25 +43,25 @@
             if (u[i] + (1.0 / (i + 1)) * (1 - np.sum(np.asarray(u)[:i + 1]))) > 0:
                 rho = i + 1
         lmbd = (1.0 / rho) * (1 - np.sum(np.asarray(u)[:rho]))
         for i in range(len(p)):
             res.append(max(p[i] + lmbd, 0))
         return res
 
-    def global_test(self, dataflag='valid'):
+    def global_test(self, flag='valid'):
         """
         Validate accuracies and losses on clients' local datasets
         :param
             dataflag: choose train data or valid data to evaluate
         :return
             metrics: a dict contains the lists of each metric_value of the clients
         """
         all_metrics = collections.defaultdict(list)
         for c in self.clients:
-            client_metrics = c.test(self.result_model, dataflag)
+            client_metrics = c.test(self.result_model, flag)
             for met_name, met_val in client_metrics.items():
                 all_metrics[met_name].append(met_val)
         return all_metrics
 
     def test(self, model=None, flag='test'):
         if model == None: model = self.result_model
         data = self.test_data if flag=='test' else self.valid_data
```

### Comparing `flgo-0.0.3/src/flgo/algorithm/fedasync.py` & `flgo-0.0.4/src/flgo/algorithm/fedasync.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.3/src/flgo/algorithm/fedbase.py` & `flgo-0.0.4/src/flgo/algorithm/fedbase.py`

 * *Files 1% similar despite different names*

```diff
@@ -314,25 +314,25 @@
             return (1.0-sum(p))*self.model + w
         else:
             p = [1.0 * local_data_vols[cid] / total_data_vol for cid in self.received_clients]
             sump = sum(p)
             p = [pk/sump for pk in p]
             return fmodule._model_sum([model_k * pk for model_k, pk in zip(models, p)])
 
-    def global_test(self, dataflag='valid'):
+    def global_test(self, flag='valid'):
         """
         Validate accuracies and losses on clients' local datasets
         :param
             dataflag (str): choose train data or valid data to evaluate
         :return
             metrics (dict): a dict contains the lists of each metric_value of the clients
         """
         all_metrics = collections.defaultdict(list)
         for c in self.clients:
-            client_metrics = c.test(self.model, dataflag)
+            client_metrics = c.test(self.model, flag)
             for met_name, met_val in client_metrics.items():
                 all_metrics[met_name].append(met_val)
         return all_metrics
 
     def test(self, model=None, flag='test'):
         """
         Evaluate the model on the test dataset owned by the server.
@@ -341,15 +341,15 @@
         :return:
             metrics (dict): specified by the task during running time (e.g. metric = [mean_accuracy, mean_loss] when the task is classification)
         """
         if model is None: model=self.model
         data = self.test_data if flag=='test' else self.valid_data
         if data is None: return {}
         else:
-            return self.calculator.test(model, self.test_data, batch_size = self.option['test_batch_size'])
+            return self.calculator.test(model, data, batch_size = self.option['test_batch_size'], num_workers = self.option['num_workers'], pin_memory = self.option['pin_memory'])
 
     def init_algo_para(self, algo_para: dict):
         """
         Initialize the algorithm-dependent hyper-parameters for the server and all the clients.
         :param
             algo_paras (dict): the dict that defines the hyper-parameters (i.e. name, value and type) for the algorithm.
 
@@ -438,14 +438,15 @@
         self.current_steps = 0
         # system setting
         self._effective_num_steps = self.num_steps
         self._latency = 0
         # server
         self.server = None
         # actions of different message type
+        self.option = option
         self.actions = {0: self.reply}
 
     def initialize(self):
         # to be implemented for customized initializing operations
         return
 
     @ss.with_completeness
@@ -477,15 +478,15 @@
             model (FModule):
             dataflag (str): choose the dataset to be evaluated on
         :return:
             metric (dict): specified by the task during running time (e.g. metric = [mean_accuracy, mean_loss] when the task is classification)
         """
         dataset = self.train_data if dataflag=='train' else self.valid_data
         if dataset is not None:
-            return self.calculator.test(model, dataset, self.test_batch_size)
+            return self.calculator.test(model, dataset, self.test_batch_size, self.option['num_workers'])
         else:
             return {}
 
     def unpack(self, received_pkg):
         """
         Unpack the package received from the server
         :param
@@ -606,15 +607,15 @@
         Get the batch of data
         :return:
             a batch of data
         """
         try:
             batch_data = next(self.data_loader)
         except Exception as e:
-            self.data_loader = iter(self.calculator.get_dataloader(self.train_data, batch_size=self.batch_size, num_workers=self.loader_num_workers))
+            self.data_loader = iter(self.calculator.get_dataloader(self.train_data, batch_size=self.batch_size, num_workers=self.loader_num_workers, pin_memory=self.option['pin_memory']))
             batch_data = next(self.data_loader)
         # clear local DataLoader when finishing local training
         self.current_steps = (self.current_steps+1) % self.num_steps
         if self.current_steps == 0:self.data_loader = None
         return batch_data
 
     def update_device(self, dev):
```

### Comparing `flgo-0.0.3/src/flgo/algorithm/fedbuff.py` & `flgo-0.0.4/src/flgo/algorithm/fedbuff.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.3/src/flgo/algorithm/fedmgda+.py` & `flgo-0.0.4/src/flgo/algorithm/fedmgda+.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.3/src/flgo/algorithm/fedprox.py` & `flgo-0.0.4/src/flgo/algorithm/fedprox.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.3/src/flgo/algorithm/mifa.py` & `flgo-0.0.4/src/flgo/algorithm/mifa.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.3/src/flgo/algorithm/powerofchoice.py` & `flgo-0.0.4/src/flgo/algorithm/powerofchoice.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.3/src/flgo/algorithm/qfedavg.py` & `flgo-0.0.4/src/flgo/algorithm/qfedavg.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.3/src/flgo/algorithm/scaffold.py` & `flgo-0.0.4/src/flgo/algorithm/scaffold.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.3/src/flgo/algorithm/vflbase.py` & `flgo-0.0.4/src/flgo/algorithm/vflbase.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.3/src/flgo/benchmark/cifar100_classification/__init__.py` & `flgo-0.0.4/src/flgo/benchmark/cifar100_classification/__init__.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.3/src/flgo/benchmark/cifar100_classification/core.py` & `flgo-0.0.4/src/flgo/benchmark/cifar100_classification/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.3/src/flgo/benchmark/cifar100_classification/model/cnn.py` & `flgo-0.0.4/src/flgo/benchmark/cifar100_classification/model/cnn.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.3/src/flgo/benchmark/cifar100_classification/model/resnet18.py` & `flgo-0.0.4/src/flgo/benchmark/cifar100_classification/model/resnet18.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.3/src/flgo/benchmark/cifar10_classification/__init__.py` & `flgo-0.0.4/src/flgo/benchmark/cifar10_classification/__init__.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.3/src/flgo/benchmark/cifar10_classification/core.py` & `flgo-0.0.4/src/flgo/benchmark/cifar10_classification/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.3/src/flgo/benchmark/cifar10_classification/model/cnn.py` & `flgo-0.0.4/src/flgo/benchmark/cifar10_classification/model/cnn.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.3/src/flgo/benchmark/cifar10_classification/model/mlp.py` & `flgo-0.0.4/src/flgo/benchmark/cifar10_classification/model/mlp.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.3/src/flgo/benchmark/citeseer_link_prediction/core.py` & `flgo-0.0.4/src/flgo/benchmark/citeseer_link_prediction/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.3/src/flgo/benchmark/citeseer_link_prediction/model/GCN.py` & `flgo-0.0.4/src/flgo/benchmark/citeseer_link_prediction/model/GCN.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.3/src/flgo/benchmark/citeseer_node_classification/core.py` & `flgo-0.0.4/src/flgo/benchmark/citeseer_node_classification/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.3/src/flgo/benchmark/citeseer_node_classification/model/GCN.py` & `flgo-0.0.4/src/flgo/benchmark/citeseer_node_classification/model/GCN.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.3/src/flgo/benchmark/cora_link_prediction/core.py` & `flgo-0.0.4/src/flgo/benchmark/cora_link_prediction/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.3/src/flgo/benchmark/cora_link_prediction/model/GCN.py` & `flgo-0.0.4/src/flgo/benchmark/cora_link_prediction/model/GCN.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.3/src/flgo/benchmark/cora_node_classification/core.py` & `flgo-0.0.4/src/flgo/benchmark/cora_node_classification/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.3/src/flgo/benchmark/cora_node_classification/model/GCN.py` & `flgo-0.0.4/src/flgo/benchmark/cora_node_classification/model/GCN.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.3/src/flgo/benchmark/cora_node_classification/model/GraphSAGE_1.py` & `flgo-0.0.4/src/flgo/benchmark/cora_node_classification/model/GraphSAGE_1.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.3/src/flgo/benchmark/cora_node_classification/model/GraphSage.py` & `flgo-0.0.4/src/flgo/benchmark/cora_node_classification/model/GraphSage.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.3/src/flgo/benchmark/emnist_classification/core.py` & `flgo-0.0.4/src/flgo/benchmark/emnist_classification/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.3/src/flgo/benchmark/emnist_classification/model/cnn.py` & `flgo-0.0.4/src/flgo/benchmark/emnist_classification/model/cnn.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.3/src/flgo/benchmark/emnist_classification/model/mlp.py` & `flgo-0.0.4/src/flgo/benchmark/emnist_classification/model/mlp.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.3/src/flgo/benchmark/enzymes_graph_classification/core.py` & `flgo-0.0.4/src/flgo/benchmark/enzymes_graph_classification/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.3/src/flgo/benchmark/enzymes_graph_classification/model/GCN.py` & `flgo-0.0.4/src/flgo/benchmark/enzymes_graph_classification/model/GCN.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.3/src/flgo/benchmark/enzymes_graph_classification/model/GIN.py` & `flgo-0.0.4/src/flgo/benchmark/enzymes_graph_classification/model/GIN.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.3/src/flgo/benchmark/fashion_classification/core.py` & `flgo-0.0.4/src/flgo/benchmark/fashion_classification/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.3/src/flgo/benchmark/fashion_classification/model/lr.py` & `flgo-0.0.4/src/flgo/benchmark/fashion_classification/model/lr.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.3/src/flgo/benchmark/femnist_classification/core.py` & `flgo-0.0.4/src/flgo/benchmark/femnist_classification/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.3/src/flgo/benchmark/leaf_reddit/core.py` & `flgo-0.0.4/src/flgo/benchmark/leaf_reddit/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.3/src/flgo/benchmark/leaf_reddit/model/stackedlstm.py` & `flgo-0.0.4/src/flgo/benchmark/leaf_reddit/model/stackedlstm.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.3/src/flgo/benchmark/leaf_sent140/core.py` & `flgo-0.0.4/src/flgo/benchmark/leaf_sent140/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.3/src/flgo/benchmark/leaf_sent140/model/stackedlstm.py` & `flgo-0.0.4/src/flgo/benchmark/leaf_sent140/model/stackedlstm.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.3/src/flgo/benchmark/mnist_classification/__init__.py` & `flgo-0.0.4/src/flgo/benchmark/mnist_classification/__init__.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.3/src/flgo/benchmark/mnist_classification/core.py` & `flgo-0.0.4/src/flgo/benchmark/mnist_classification/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.3/src/flgo/benchmark/mnist_classification/model/cnn.py` & `flgo-0.0.4/src/flgo/benchmark/mnist_classification/model/cnn.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.3/src/flgo/benchmark/mnist_classification/model/mlp.py` & `flgo-0.0.4/src/flgo/benchmark/mnist_classification/model/mlp.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.3/src/flgo/benchmark/mutag_graph_classification/core.py` & `flgo-0.0.4/src/flgo/benchmark/mutag_graph_classification/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.3/src/flgo/benchmark/mutag_graph_classification/model/GCN.py` & `flgo-0.0.4/src/flgo/benchmark/mutag_graph_classification/model/GCN.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.3/src/flgo/benchmark/pubmed_link_prediction/core.py` & `flgo-0.0.4/src/flgo/benchmark/pubmed_link_prediction/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.3/src/flgo/benchmark/pubmed_link_prediction/model/GCN.py` & `flgo-0.0.4/src/flgo/benchmark/pubmed_link_prediction/model/GCN.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.3/src/flgo/benchmark/pubmed_node_classification/core.py` & `flgo-0.0.4/src/flgo/benchmark/pubmed_node_classification/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.3/src/flgo/benchmark/pubmed_node_classification/model/GCN.py` & `flgo-0.0.4/src/flgo/benchmark/pubmed_node_classification/model/GCN.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.3/src/flgo/benchmark/shakespeare_classification/core.py` & `flgo-0.0.4/src/flgo/benchmark/shakespeare_classification/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.3/src/flgo/benchmark/shakespeare_classification/model/stackedlstm.py` & `flgo-0.0.4/src/flgo/benchmark/shakespeare_classification/model/stackedlstm.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.3/src/flgo/benchmark/synthetic_regression/core.py` & `flgo-0.0.4/src/flgo/benchmark/synthetic_regression/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.3/src/flgo/benchmark/synthetic_regression/model/lr.py` & `flgo-0.0.4/src/flgo/benchmark/synthetic_regression/model/lr.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.3/src/flgo/benchmark/toolkits/base.py` & `flgo-0.0.4/src/flgo/benchmark/toolkits/base.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.3/src/flgo/benchmark/toolkits/cv/horizontal/image_classification.py` & `flgo-0.0.4/src/flgo/benchmark/toolkits/cv/horizontal/image_classification.py`

 * *Files 4% similar despite different names*

```diff
@@ -78,45 +78,44 @@
         """
         tdata = self.to_device(data)
         outputs = model(tdata[0])
         loss = self.criterion(outputs, tdata[-1])
         return {'loss': loss}
 
     @torch.no_grad()
-    def test(self, model, dataset, batch_size=64, num_workers=0):
+    def test(self, model, dataset, batch_size=64, num_workers=0, pin_memory=False):
         """
         Metric = [mean_accuracy, mean_loss]
         :param model:
         :param dataset:
         :param batch_size:
         :return: [mean_accuracy, mean_loss]
         """
-        with torch.no_grad():
-            model.eval()
-            if batch_size==-1:batch_size=len(dataset)
-            data_loader = self.get_dataloader(dataset, batch_size=batch_size, num_workers=num_workers)
-            total_loss = 0.0
-            num_correct = 0
-            for batch_id, batch_data in enumerate(data_loader):
-                batch_data = self.to_device(batch_data)
-                outputs = model(batch_data[0])
-                batch_mean_loss = self.criterion(outputs, batch_data[-1]).item()
-                y_pred = outputs.data.max(1, keepdim=True)[1]
-                correct = y_pred.eq(batch_data[-1].data.view_as(y_pred)).long().cpu().sum()
-                num_correct += correct.item()
-                total_loss += batch_mean_loss * len(batch_data[-1])
+        model.eval()
+        if batch_size==-1:batch_size=len(dataset)
+        data_loader = self.get_dataloader(dataset, batch_size=batch_size, num_workers=num_workers, pin_memory=pin_memory)
+        total_loss = 0.0
+        num_correct = 0
+        for batch_id, batch_data in enumerate(data_loader):
+            batch_data = self.to_device(batch_data)
+            outputs = model(batch_data[0])
+            batch_mean_loss = self.criterion(outputs, batch_data[-1]).item()
+            y_pred = outputs.data.max(1, keepdim=True)[1]
+            correct = y_pred.eq(batch_data[-1].data.view_as(y_pred)).long().cpu().sum()
+            num_correct += correct.item()
+            total_loss += batch_mean_loss * len(batch_data[-1])
         return {'accuracy': 1.0*num_correct/len(dataset), 'loss':total_loss/len(dataset)}
 
     def to_device(self, data):
         return data[0].to(self.device), data[1].to(self.device)
 
-    def get_dataloader(self, dataset, batch_size=64, shuffle=True, num_workers=0):
+    def get_dataloader(self, dataset, batch_size=64, shuffle=True, num_workers=0, pin_memory=False, drop_last=False):
         if self.DataLoader == None:
             raise NotImplementedError("DataLoader Not Found.")
-        return self.DataLoader(dataset, batch_size=batch_size, shuffle=shuffle, num_workers=num_workers)
+        return self.DataLoader(dataset, batch_size=batch_size, shuffle=shuffle, num_workers=num_workers, pin_memory=pin_memory, drop_last=drop_last)
 
 class GeneralGenerator(BasicTaskGenerator):
     def __init__(self, benchmark, rawdata_path):
         super(GeneralGenerator, self).__init__(benchmark, rawdata_path)
         return
 
     def load_data(self):
```

### Comparing `flgo-0.0.3/src/flgo/benchmark/toolkits/graph/horizontal/graph_classification.py` & `flgo-0.0.4/src/flgo/benchmark/toolkits/graph/horizontal/graph_classification.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.3/src/flgo/benchmark/toolkits/graph/horizontal/link_prediction.py` & `flgo-0.0.4/src/flgo/benchmark/toolkits/graph/horizontal/link_prediction.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.3/src/flgo/benchmark/toolkits/graph/horizontal/node_classification.py` & `flgo-0.0.4/src/flgo/benchmark/toolkits/graph/horizontal/node_classification.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.3/src/flgo/benchmark/toolkits/partition.py` & `flgo-0.0.4/src/flgo/benchmark/toolkits/partition.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.3/src/flgo/benchmark/toolkits/visualization.py` & `flgo-0.0.4/src/flgo/benchmark/toolkits/visualization.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.3/src/flgo/benchmark/vertical_mnist_classification/core.py` & `flgo-0.0.4/src/flgo/benchmark/vertical_mnist_classification/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.3/src/flgo/benchmark/vertical_mnist_classification/model/mlp.py` & `flgo-0.0.4/src/flgo/benchmark/vertical_mnist_classification/model/mlp.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.3/src/flgo/experiment/analyzer.py` & `flgo-0.0.4/src/flgo/experiment/analyzer.py`

 * *Files 4% similar despite different names*

```diff
@@ -97,16 +97,22 @@
                 x.append(round)
             if self.data['option']['early_stop'] > 0 and 'valid_loss' in self.data.keys() and len(x) >= len(self.data['valid_loss']):
                 break
         self.data['communication_round'] = x
 
     def set_client_id(self):
         with open(os.path.join(self.task, 'info')) as inf:
-            num_clients = json.load(inf)['num_clients']
-        self.data['client_id'] = [cid for cid in range(int(num_clients))]
+            task_info = json.load(inf)
+            if 'num_clients' in task_info.keys():
+                N = int(task_info['num_clients'])
+            elif 'num_parties' in task_info.keys():
+                N = int(task_info['num_parties'])
+            else:
+                N = 0
+        self.data['client_id'] = [cid for cid in range(N)]
 
     def set_legend(self, legend_with = []):
         if len(legend_with)==0: self.data['label'] = []
         self.data['label'] = [self.name[:self.name.find('_M')]]
         for key in legend_with:
             val = key + self.get_key_from_name(key)
             self.data['label'].append(val)
```

### Comparing `flgo-0.0.3/src/flgo/experiment/device_scheduler.py` & `flgo-0.0.4/src/flgo/experiment/device_scheduler.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.3/src/flgo/experiment/logger/__init__.py` & `flgo-0.0.4/src/flgo/experiment/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.3/src/flgo/experiment/logger/config.py` & `flgo-0.0.4/src/flgo/experiment/logger/config.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.3/src/flgo/experiment/logger/handlers.py` & `flgo-0.0.4/src/flgo/experiment/logger/handlers.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.3/src/flgo/experiment/logger/simple_logger.py` & `flgo-0.0.4/src/flgo/experiment/logger/simple_logger.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.3/src/flgo/experiment/logger/tune_logger.py` & `flgo-0.0.4/src/flgo/experiment/logger/tune_logger.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.3/src/flgo/experiment/logger/vertical_logger.py` & `flgo-0.0.4/src/flgo/experiment/logger/vertical_logger.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.3/src/flgo/experiment/runner.py` & `flgo-0.0.4/src/flgo/experiment/runner.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.3/src/flgo/system_simulator/__init__.py` & `flgo-0.0.4/src/flgo/system_simulator/__init__.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.3/src/flgo/system_simulator/base.py` & `flgo-0.0.4/src/flgo/system_simulator/base.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.3/src/flgo/system_simulator/default_simulator.py` & `flgo-0.0.4/src/flgo/system_simulator/default_simulator.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.3/src/flgo/system_simulator/my_simulator.py` & `flgo-0.0.4/src/flgo/system_simulator/my_simulator.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.3/src/flgo/system_simulator/phone_simulator.py` & `flgo-0.0.4/src/flgo/system_simulator/phone_simulator.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.3/src/flgo/utils/fflow.py` & `flgo-0.0.4/src/flgo/utils/fflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 import yaml
 import queue
 import sys
 
 sample_list=['uniform', 'md', 'full', 'uniform_available', 'md_available', 'full_available']
 agg_list=['uniform', 'weighted_scale', 'weighted_com']
 optimizer_list=['SGD', 'Adam', 'RMSprop', 'Adagrad']
-default_option_dict = {'pretrain': '', 'sample': 'md', 'aggregate': 'uniform', 'num_rounds': 20, 'proportion': 0.2, 'learning_rate_decay': 0.998, 'lr_scheduler': -1, 'early_stop': -1, 'num_epochs': 5, 'num_steps': -1, 'learning_rate': 0.1, 'batch_size': 64.0, 'optimizer': 'SGD', 'momentum': 0, 'weight_decay': 0, 'algo_para': [], 'train_holdout': 0.1, 'test_holdout': 0.0, 'seed': 0, 'gpu': [], 'server_with_cpu': False, 'num_parallels': 1, 'num_workers': 0, 'test_batch_size': 512, 'simulator': 'default_simulator', 'availability': 'IDL', 'connectivity': 'IDL', 'completeness': 'IDL', 'responsiveness': 'IDL', 'logger': 'basic_logger', 'log_level': 'INFO', 'log_file': False, 'no_log_console': False, 'no_overwrite': False, 'eval_interval': 1}
+default_option_dict = {'pretrain': '', 'sample': 'md', 'aggregate': 'uniform', 'num_rounds': 20, 'proportion': 0.2, 'learning_rate_decay': 0.998, 'lr_scheduler': -1, 'early_stop': -1, 'num_epochs': 5, 'num_steps': -1, 'learning_rate': 0.1, 'batch_size': 64.0, 'optimizer': 'SGD', 'momentum': 0, 'weight_decay': 0, 'algo_para': [], 'train_holdout': 0.1, 'test_holdout': 0.0, 'seed': 0, 'gpu': [], 'server_with_cpu': False, 'num_parallels': 1, 'num_workers': 0, 'pin_memory':False,'test_batch_size': 512, 'simulator': 'default_simulator', 'availability': 'IDL', 'connectivity': 'IDL', 'completeness': 'IDL', 'responsiveness': 'IDL', 'logger': 'basic_logger', 'log_level': 'INFO', 'log_file': False, 'no_log_console': False, 'no_overwrite': False, 'eval_interval': 1}
 
 class GlobalVariable:
     """this class is to create a buffer space for sharing variables across different parties for each runner respectively in a single machine"""
     def __init__(self):
         self.logger = None
         self.simulator = None
         self.clock = None
@@ -95,14 +95,15 @@
     parser.add_argument('--test_holdout', help='the rate of holding out the validation dataset from the training datasets', type=float, default=0.0)
     # realistic machine config
     parser.add_argument('--seed', help='seed for random initialization;', type=int, default=0)
     parser.add_argument('--gpu', nargs='*', help='GPU IDs and empty input is equal to using CPU', type=int)
     parser.add_argument('--server_with_cpu', help='seed for random initialization;', action="store_true", default=False)
     parser.add_argument('--num_parallels', help="the number of parallels in the clients computing session", type=int, default=1)
     parser.add_argument('--num_workers', help='the number of workers of DataLoader', type=int, default=0)
+    parser.add_argument('--pin_memory', help='pin_memory of DataLoader', action="store_true", default=False)
     parser.add_argument('--test_batch_size', help='the batch_size used in testing phase;', type=int, default=512)
 
     """Simulator Options"""
     # the simulating systemic configuration of clients and the server that helps constructing the heterogeity in the network condition & computing power
     parser.add_argument('--availability', help="client availability mode", type=str, default = 'IDL')
     parser.add_argument('--connectivity', help="client connectivity mode", type=str, default = 'IDL')
     parser.add_argument('--completeness', help="client completeness mode", type=str, default = 'IDL')
@@ -612,15 +613,15 @@
             default_args = [None, None, default_option_dict, None, flgo.experiment.logger.simple_logger.SimpleLogger, flgo.system_simulator.DefaultSimulator, 'horizontal']
             for aid in range(len(a)):
                 if aid==0:
                     default_args[aid] = a[aid]
                 if aid==1:
                     algorithm = a[aid]
                     algorithm_name = algorithm.__name__ if (not hasattr(algorithm, '__module__') and hasattr(algorithm, '__name__')) else algorithm
-                    default_args[aid] = a[aid]
+                    default_args[aid] = algorithm_name
                 elif aid==2:
                     option = a[aid]
                     default_option = read_option_from_command()
                     for op_key in option:
                         if op_key in default_option.keys():
                             op_type = type(default_option[op_key])
                             if op_type == type(option[op_key]):
```

### Comparing `flgo-0.0.3/src/flgo/utils/fmodule.py` & `flgo-0.0.4/src/flgo/utils/fmodule.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.3/src/flgo.egg-info/SOURCES.txt` & `flgo-0.0.4/src/flgo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flgo-0.0.3/tests/test.py` & `flgo-0.0.4/tests/test.py`

 * *Files identical despite different names*

