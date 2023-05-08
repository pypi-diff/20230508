# Comparing `tmp/visual_graph_datasets-0.8.0.tar.gz` & `tmp/visual_graph_datasets-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "visual_graph_datasets-0.8.0.tar", max compression
+gzip compressed data, was "visual_graph_datasets-0.9.0.tar", max compression
```

## Comparing `visual_graph_datasets-0.8.0.tar` & `visual_graph_datasets-0.9.0.tar`

### file list

```diff
@@ -1,43 +1,51 @@
--rwxr-xr-x   0        0        0     8367 2022-12-29 07:58:07.514976 visual_graph_datasets-0.8.0/README.rst
--rwxr-xr-x   0        0        0     1197 2022-12-30 09:19:29.127832 visual_graph_datasets-0.8.0/pyproject.toml
--rwxr-xr-x   0        0        0        5 2022-12-30 09:19:29.131832 visual_graph_datasets-0.8.0/visual_graph_datasets/VERSION
--rwxr-xr-x   0        0        0        0 2022-12-15 14:44:46.036582 visual_graph_datasets-0.8.0/visual_graph_datasets/__init__.py
--rwxr-xr-x   0        0        0     9153 2022-12-15 14:59:02.005409 visual_graph_datasets-0.8.0/visual_graph_datasets/cli.py
--rwxr-xr-x   0        0        0     4832 2022-12-15 14:44:46.036582 visual_graph_datasets-0.8.0/visual_graph_datasets/config.py
--rwxr-xr-x   0        0        0     7475 2022-12-15 14:44:46.036582 visual_graph_datasets-0.8.0/visual_graph_datasets/data.py
--rw-r--r--   0        0        0        0 2022-12-29 07:58:07.514976 visual_graph_datasets-0.8.0/visual_graph_datasets/examples/__init__.py
--rw-r--r--   0        0        0     2247 2022-12-29 07:58:07.514976 visual_graph_datasets-0.8.0/visual_graph_datasets/examples/readme_00.py
--rwxr-xr-x   0        0        0    10885 2022-12-16 10:21:27.893145 visual_graph_datasets-0.8.0/visual_graph_datasets/experiments/generate_benzene_solubility_from_csv.py
--rwxr-xr-x   0        0        0     7240 2022-12-29 07:58:07.514976 visual_graph_datasets-0.8.0/visual_graph_datasets/experiments/generate_mock.py
--rwxr-xr-x   0        0        0    10840 2022-12-16 13:14:14.800720 visual_graph_datasets-0.8.0/visual_graph_datasets/experiments/generate_molecule_dataset_from_csv.py
--rw-r--r--   0        0        0    18712 2022-12-30 09:18:58.499653 visual_graph_datasets-0.8.0/visual_graph_datasets/experiments/generate_molecule_multitask_dataset_from_csv.py
--rw-r--r--   0        0        0    19401 2022-12-30 09:10:33.320580 visual_graph_datasets-0.8.0/visual_graph_datasets/experiments/generate_molecule_solubility_12.py
--rwxr-xr-x   0        0        0     4655 2022-12-16 10:21:27.889145 visual_graph_datasets-0.8.0/visual_graph_datasets/experiments/update_rb_colors.py
--rwxr-xr-x   0        0        0        0 2022-12-15 14:44:46.036582 visual_graph_datasets-0.8.0/visual_graph_datasets/generation/__init__.py
--rw-r--r--   0        0        0      179 2022-12-15 20:08:26.689851 visual_graph_datasets-0.8.0/visual_graph_datasets/generation/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0    10417 2022-12-15 20:08:26.693851 visual_graph_datasets-0.8.0/visual_graph_datasets/generation/__pycache__/graph.cpython-310.pyc
--rwxr-xr-x   0        0        0    18432 2022-12-15 14:44:46.036582 visual_graph_datasets-0.8.0/visual_graph_datasets/generation/graph.py
--rwxr-xr-x   0        0        0        0 2022-12-15 14:44:46.036582 visual_graph_datasets-0.8.0/visual_graph_datasets/processing/__init__.py
--rw-r--r--   0        0        0      179 2022-12-16 12:03:43.415661 visual_graph_datasets-0.8.0/visual_graph_datasets/processing/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      500 2022-12-16 12:03:43.415661 visual_graph_datasets-0.8.0/visual_graph_datasets/processing/__pycache__/base.cpython-310.pyc
--rw-r--r--   0        0        0     3563 2022-12-16 12:03:43.415661 visual_graph_datasets-0.8.0/visual_graph_datasets/processing/__pycache__/molecules.cpython-310.pyc
--rwxr-xr-x   0        0        0      166 2022-12-15 14:44:46.036582 visual_graph_datasets-0.8.0/visual_graph_datasets/processing/base.py
--rwxr-xr-x   0        0        0     3057 2022-12-15 14:44:46.036582 visual_graph_datasets-0.8.0/visual_graph_datasets/processing/molecules.py
--rwxr-xr-x   0        0        0      599 2022-12-15 14:44:46.036582 visual_graph_datasets-0.8.0/visual_graph_datasets/templates/config.yaml.j2
--rwxr-xr-x   0        0        0      678 2022-12-15 14:44:46.036582 visual_graph_datasets-0.8.0/visual_graph_datasets/templates/list.out.j2
--rw-r--r--   0        0        0     1856 2022-12-15 20:08:26.373849 visual_graph_datasets-0.8.0/visual_graph_datasets/testing.py
--rwxr-xr-x   0        0        0     1351 2022-12-15 14:44:46.036582 visual_graph_datasets-0.8.0/visual_graph_datasets/typing.py
--rwxr-xr-x   0        0        0     4285 2022-12-16 11:19:28.306359 visual_graph_datasets-0.8.0/visual_graph_datasets/util.py
--rwxr-xr-x   0        0        0        0 2022-12-15 14:44:46.036582 visual_graph_datasets-0.8.0/visual_graph_datasets/visualization/__init__.py
--rw-r--r--   0        0        0      182 2022-12-15 20:08:26.697851 visual_graph_datasets-0.8.0/visual_graph_datasets/visualization/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3570 2022-12-29 08:20:38.939899 visual_graph_datasets-0.8.0/visual_graph_datasets/visualization/__pycache__/base.cpython-310.pyc
--rw-r--r--   0        0        0     3794 2022-12-15 20:08:26.865852 visual_graph_datasets-0.8.0/visual_graph_datasets/visualization/__pycache__/colors.cpython-310.pyc
--rw-r--r--   0        0        0     4544 2022-12-29 08:15:10.441913 visual_graph_datasets-0.8.0/visual_graph_datasets/visualization/__pycache__/importances.cpython-310.pyc
--rw-r--r--   0        0        0     2716 2022-12-15 20:08:26.913852 visual_graph_datasets-0.8.0/visual_graph_datasets/visualization/__pycache__/molecules.cpython-310.pyc
--rwxr-xr-x   0        0        0     4059 2022-12-29 07:58:07.518976 visual_graph_datasets-0.8.0/visual_graph_datasets/visualization/base.py
--rwxr-xr-x   0        0        0     4316 2022-12-15 14:44:46.036582 visual_graph_datasets-0.8.0/visual_graph_datasets/visualization/colors.py
--rwxr-xr-x   0        0        0     9962 2022-12-29 07:58:07.518976 visual_graph_datasets-0.8.0/visual_graph_datasets/visualization/importances.py
--rwxr-xr-x   0        0        0     3502 2022-12-15 14:44:46.036582 visual_graph_datasets-0.8.0/visual_graph_datasets/visualization/molecules.py
--rwxr-xr-x   0        0        0     7741 2022-12-29 07:58:07.518976 visual_graph_datasets-0.8.0/visual_graph_datasets/web.py
--rw-r--r--   0        0        0     9840 1970-01-01 00:00:00.000000 visual_graph_datasets-0.8.0/setup.py
--rw-r--r--   0        0        0     9605 1970-01-01 00:00:00.000000 visual_graph_datasets-0.8.0/PKG-INFO
+-rwxr-xr-x   0        0        0    11081 2023-01-29 15:40:21.336433 visual_graph_datasets-0.9.0/README.rst
+-rwxr-xr-x   0        0        0     1197 2023-01-29 15:44:11.790936 visual_graph_datasets-0.9.0/pyproject.toml
+-rwxr-xr-x   0        0        0        5 2022-12-30 09:19:29.131832 visual_graph_datasets-0.9.0/visual_graph_datasets/VERSION
+-rwxr-xr-x   0        0        0        0 2022-12-15 14:44:46.036582 visual_graph_datasets-0.9.0/visual_graph_datasets/__init__.py
+-rwxr-xr-x   0        0        0    12642 2022-12-30 14:30:48.020328 visual_graph_datasets-0.9.0/visual_graph_datasets/cli.py
+-rwxr-xr-x   0        0        0     4970 2022-12-30 13:08:45.623425 visual_graph_datasets-0.9.0/visual_graph_datasets/config.py
+-rwxr-xr-x   0        0        0    16653 2022-12-30 13:40:35.187393 visual_graph_datasets-0.9.0/visual_graph_datasets/data.py
+-rw-r--r--   0        0        0        0 2022-12-29 07:58:07.514976 visual_graph_datasets-0.9.0/visual_graph_datasets/examples/__init__.py
+-rw-r--r--   0        0        0     2247 2022-12-29 07:58:07.514976 visual_graph_datasets-0.9.0/visual_graph_datasets/examples/readme_00.py
+-rw-r--r--   0        0        0      852 2023-01-22 14:35:11.789504 visual_graph_datasets-0.9.0/visual_graph_datasets/experiments/README.rst
+-rw-r--r--   0        0        0    10896 2023-01-28 11:27:37.329856 visual_graph_datasets-0.9.0/visual_graph_datasets/experiments/__pycache__/generate_molecule_dataset_from_csv.cpython-310.pyc
+-rw-r--r--   0        0        0     2641 2023-01-27 16:57:37.904481 visual_graph_datasets-0.9.0/visual_graph_datasets/experiments/__pycache__/generate_molecule_dataset_from_csv_multitask.cpython-310.pyc
+-rw-r--r--   0        0        0     1279 2023-01-23 13:39:59.247590 visual_graph_datasets-0.9.0/visual_graph_datasets/experiments/_aqsoldb_csv.py
+-rw-r--r--   0        0        0   946376 2023-01-23 13:39:59.451591 visual_graph_datasets-0.9.0/visual_graph_datasets/experiments/aqsoldb.csv
+-rwxr-xr-x   0        0        0  3750208 2022-05-29 06:44:36.465000 visual_graph_datasets-0.9.0/visual_graph_datasets/experiments/aqsoldb_full.csv
+-rwxr-xr-x   0        0        0   196843 2022-09-15 11:20:25.457000 visual_graph_datasets-0.9.0/visual_graph_datasets/experiments/dataset-E.csv
+-rwxr-xr-x   0        0        0     7240 2022-12-29 07:58:07.514976 visual_graph_datasets-0.9.0/visual_graph_datasets/experiments/generate_mock.py
+-rwxr-xr-x   0        0        0    22049 2023-01-29 15:43:22.030244 visual_graph_datasets-0.9.0/visual_graph_datasets/experiments/generate_molecule_dataset_from_csv.py
+-rw-r--r--   0        0        0     1676 2023-01-23 19:12:40.774422 visual_graph_datasets-0.9.0/visual_graph_datasets/experiments/generate_molecule_dataset_from_csv_aqsoldb.py
+-rw-r--r--   0        0        0     8087 2023-01-28 11:49:00.769381 visual_graph_datasets-0.9.0/visual_graph_datasets/experiments/generate_molecule_dataset_from_csv_multitask.py
+-rw-r--r--   0        0        0    18712 2022-12-30 09:18:58.499653 visual_graph_datasets-0.9.0/visual_graph_datasets/experiments/generate_molecule_multitask_dataset_from_csv.py
+-rw-r--r--   0        0        0    18556 2022-12-30 15:29:02.361942 visual_graph_datasets-0.9.0/visual_graph_datasets/experiments/generate_tadf_multi.py
+-rwxr-xr-x   0        0        0     4655 2022-12-16 10:21:27.889145 visual_graph_datasets-0.9.0/visual_graph_datasets/experiments/update_rb_colors.py
+-rwxr-xr-x   0        0        0        0 2022-12-15 14:44:46.036582 visual_graph_datasets-0.9.0/visual_graph_datasets/generation/__init__.py
+-rw-r--r--   0        0        0      179 2022-12-15 20:08:26.689851 visual_graph_datasets-0.9.0/visual_graph_datasets/generation/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0    10417 2022-12-15 20:08:26.693851 visual_graph_datasets-0.9.0/visual_graph_datasets/generation/__pycache__/graph.cpython-310.pyc
+-rwxr-xr-x   0        0        0    18432 2022-12-15 14:44:46.036582 visual_graph_datasets-0.9.0/visual_graph_datasets/generation/graph.py
+-rwxr-xr-x   0        0        0        0 2022-12-15 14:44:46.036582 visual_graph_datasets-0.9.0/visual_graph_datasets/processing/__init__.py
+-rw-r--r--   0        0        0      179 2022-12-16 12:03:43.415661 visual_graph_datasets-0.9.0/visual_graph_datasets/processing/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      500 2022-12-16 12:03:43.415661 visual_graph_datasets-0.9.0/visual_graph_datasets/processing/__pycache__/base.cpython-310.pyc
+-rw-r--r--   0        0        0     3563 2022-12-16 12:03:43.415661 visual_graph_datasets-0.9.0/visual_graph_datasets/processing/__pycache__/molecules.cpython-310.pyc
+-rwxr-xr-x   0        0        0      166 2022-12-15 14:44:46.036582 visual_graph_datasets-0.9.0/visual_graph_datasets/processing/base.py
+-rwxr-xr-x   0        0        0     3057 2022-12-15 14:44:46.036582 visual_graph_datasets-0.9.0/visual_graph_datasets/processing/molecules.py
+-rwxr-xr-x   0        0        0      599 2022-12-15 14:44:46.036582 visual_graph_datasets-0.9.0/visual_graph_datasets/templates/config.yaml.j2
+-rwxr-xr-x   0        0        0     1073 2022-12-30 14:24:48.162185 visual_graph_datasets-0.9.0/visual_graph_datasets/templates/list.out.j2
+-rw-r--r--   0        0        0     1856 2022-12-15 20:08:26.373849 visual_graph_datasets-0.9.0/visual_graph_datasets/testing.py
+-rwxr-xr-x   0        0        0     2849 2022-12-30 11:11:49.762991 visual_graph_datasets-0.9.0/visual_graph_datasets/typing.py
+-rwxr-xr-x   0        0        0     4285 2022-12-16 11:19:28.306359 visual_graph_datasets-0.9.0/visual_graph_datasets/util.py
+-rwxr-xr-x   0        0        0        0 2022-12-15 14:44:46.036582 visual_graph_datasets-0.9.0/visual_graph_datasets/visualization/__init__.py
+-rw-r--r--   0        0        0      182 2022-12-15 20:08:26.697851 visual_graph_datasets-0.9.0/visual_graph_datasets/visualization/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3570 2022-12-29 08:20:38.939899 visual_graph_datasets-0.9.0/visual_graph_datasets/visualization/__pycache__/base.cpython-310.pyc
+-rw-r--r--   0        0        0     3794 2022-12-15 20:08:26.865852 visual_graph_datasets-0.9.0/visual_graph_datasets/visualization/__pycache__/colors.cpython-310.pyc
+-rw-r--r--   0        0        0     4544 2022-12-29 08:15:10.441913 visual_graph_datasets-0.9.0/visual_graph_datasets/visualization/__pycache__/importances.cpython-310.pyc
+-rw-r--r--   0        0        0     2716 2022-12-15 20:08:26.913852 visual_graph_datasets-0.9.0/visual_graph_datasets/visualization/__pycache__/molecules.cpython-310.pyc
+-rwxr-xr-x   0        0        0     4059 2022-12-29 07:58:07.518976 visual_graph_datasets-0.9.0/visual_graph_datasets/visualization/base.py
+-rwxr-xr-x   0        0        0     4316 2022-12-15 14:44:46.036582 visual_graph_datasets-0.9.0/visual_graph_datasets/visualization/colors.py
+-rwxr-xr-x   0        0        0     9962 2022-12-29 07:58:07.518976 visual_graph_datasets-0.9.0/visual_graph_datasets/visualization/importances.py
+-rwxr-xr-x   0        0        0     3502 2022-12-15 14:44:46.036582 visual_graph_datasets-0.9.0/visual_graph_datasets/visualization/molecules.py
+-rwxr-xr-x   0        0        0     7741 2022-12-29 07:58:07.518976 visual_graph_datasets-0.9.0/visual_graph_datasets/web.py
+-rw-r--r--   0        0        0    12596 1970-01-01 00:00:00.000000 visual_graph_datasets-0.9.0/setup.py
+-rw-r--r--   0        0        0    12319 1970-01-01 00:00:00.000000 visual_graph_datasets-0.9.0/PKG-INFO
```

### Comparing `visual_graph_datasets-0.8.0/README.rst` & `visual_graph_datasets-0.9.0/README.rst`

 * *Files 17% similar despite different names*

```diff
@@ -145,53 +145,95 @@
     fig_path = os.path.join(os.getcwd(), 'importances.pdf')
     fig.savefig(fig_path)
 
 
 Dataset Format
 ==============
 
+Visual Graph Datasets are represented as *folders* containing multiple files. The primary content of these
+dataset folders is made up of *2* files per element in the dataset:
+
+- **A PNG file**. This is the canonical visualization of the graph which can subsequently be used to create
+  explanation visualizations as well. The pixel position of each node in the graph is attached as metadata
+  of the graph representation.
+
+- **A JSON file**. Primarily contains the *full* graph representation consisting of node attributes, edge
+  attributes, an edge list etc. May also contain custom metadata for each graph depending on the dataset.
+
+Optionally, a dataset folder may also contain a ``.meta.yml`` file which contains additional metadata about
+the dataset as a whole.
+
+Element Metadata JSON
+---------------------
+
+One such metadata file belonging to one element of the dataset may have the following nested structure:
+
+- ``target``: a 1d array containing the target values for the element. For classification this usually
+  a one-hot encoded vector of classes already. For multi-task regression this vector may have an
+  arbitrary number of continuous regression targets. For single-task regression this will still be a
+  vector, albeit with the shape (1, )
+- ``index``: The canonical index of this element within the dataset
+- (``train_split`` *optional*) A list of int indices, where each index represents a different split.
+  if the number "1" is for example part of this list, that means that the corresponding element is
+  considered to be part of the training set of split "1". What each particular split is may be described
+  in the documentation of the dataset.
+- (``test_split`` *optional*) A list of int indices, where each index represents a different split.
+  if the number "1" is for example part of this list, that means that the corresponding element is
+  considered to be part of the test set of the split "1".
+- ``graph``: A dictionary which contains the entire graph representation of this element.
+
+    - ``node_indices``: array of shape (V, 1) with the integer node indices.
+    - ``node_attributes``: array of shape (V, N)
+    - ``edge_indices``: array of shape (E, 2) which are the tuples of integer node indices that
+      determine edges
+    - ``edge_attributes``: array of shape (E, M)
+    - ``node_positions`` array of shape (V, 2) which are the xy positions of each node in pixel
+      values within the corresponding image visualization of the element. This is the crucial
+      information which is required to use the existing image representations to visualize attributional
+      explanations!
+    - (``node_importances_{K}_{suffix}`` *optional*) array of shape (V, K) containing ground truth node importance
+      explanations, which assign an importance value of 0 to 1 to each node of the graph across K channels.
+      One dataset element may have none or multiple such annotations with different suffixes
+      determining the number of explanation channels and origin.
+    - (``edge_importances_{K}_{suffix}`` *optional*) array of shape (E, K) containing ground truth edge importance
+      explanations, which assign an importance value of 0 to 1 to each edge of the graph across K channels.
+      One dataset element may have none or multiple such annotations with different suffixes
+      determining the number of explanation channels and origin.
+
 Assuming the following shape definitions:
 
 - V - the number of nodes in a graph
 - E - the number of edges in a graph
 - N - the number of node attributes / features associated with each node
 - M - the number of edge attributes / features associated with each edge
 - K - the number of importance channels
 
-One such content dictionary which are the values of the two dicts returned by the function have the
-following nested dictionary structure:
+Dataset Metadata YML
+--------------------
 
-- ``image_path``: The absolute path to the image file that visualizes this element
-- ``metadata_path``: the absolute path to the metadata file
-- ``metadata``: A dict which contains all the metadata for that element
-    - ``target``: a 1d array containing the target values for the element. For classification this usually
-      a one-hot encoded class vector already.
-    - ``index``: The canonical index of this element within the dataset
-    - ``graph``: A dictionary which contains the entire graph representation of this element.
-        - ``node_indices``: array of shape (V, 1) with the integer node indices.
-        - ``node_attributes``: array of shape (V, N)
-        - ``edge_indices``: array of shape (E, 2) which are the tuples of integer node indices that
-          determine edges
-        - ``edge_attributes``: array of shape (E, M)
-        - ``node_positions`` array of shape (V, 2) which are the xy positions of each node in pixel
-          values within the corresponding image visualization of the element. This is the crucial
-          information which is required to use the existing image representations to visualize attributional
-          explanations!
-        - (``node_importances_{K}_{suffix}``) array of shape (V, K) containing ground truth node importance
-          explanations, which assign an importance value of 0 to 1 to each node of the graph across K channels.
-          One dataset element may have none or multiple such annotations with different suffixes
-          determining the number of explanation channels and origin.
-        - (``edge_importances_{K}_{suffix}``) array of shape (E, K) containing ground truth edge importance
-          explanations, which assign an importance value of 0 to 1 to each edge of the graph across K channels.
-          One dataset element may have none or multiple such annotations with different suffixes
-          determining the number of explanation channels and origin.
+One such metadata file may have the following nested structure. Additionally, it may also contain custom
+additional fields depending on each dataset.
 
+- ``version``: A string determining the current version of the dataset
+- ``description``: Short string description of what the dataset is about (for example where the data came
+  from, what types of graphs it consists of, what the prediction target is etc.)
+- ``visualization_description``: String description of what can be seen in the visualization of the graph.
+  There are many different types of graphs out there which may have very domain specific visualizations.
+  This string should provide a short description of how the visualizations may be interpreted.
+- ``references``: A list of strings, where each string is a short description of online resources which are
+  relevant to the dataset, usually including a URL. This could for example include references to scientific
+  publications where a dataset was first introduced.
+- ``file_size``: The integer *accumulated* size of all the files that make up the dataset in bytes.
+- ``num_elements``: The integer number of elements in the dataset
+- ``num_targets``: The size of the prediction target vector
+- ``num_node_attributes``: The size of the node attribute vector
+- ``num_edge_attributes``: The size of the edge attribute vector
 
 Datasets
 ========
 
-Here is a list of the datasets currently included.
+Here is a list of the datasets currently uploaded on the main file share provider.
 
 For more information about the individual datasets use the ``list`` command in the CLI (see above).
 
 * TO BE DONE
```

### Comparing `visual_graph_datasets-0.8.0/pyproject.toml` & `visual_graph_datasets-0.9.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.2.0b2"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "visual_graph_datasets"
-version = "0.8.0"
+version = "0.9.0"
 description = "Datasets for the training of graph neural networks (GNNs) and subsequent visualization of attributional explanations of XAI methods"
 license = "MIT"
 authors = ["awa59kst120df <awa59kst120df@gmail.com>"]
 maintainers = ["awa59kst120df <awa59kst120df@gmail.com>"]
 readme = "README.rst"
 keywords = ["graph neural networks", "datasets", "explainable AI"]
 packages = [
```

### Comparing `visual_graph_datasets-0.8.0/visual_graph_datasets/cli.py` & `visual_graph_datasets-0.9.0/visual_graph_datasets/cli.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 import shutil
+import tempfile
+
 import click
 import os
 import json
+import yaml
 import typing as t
 
 from visual_graph_datasets.config import CONFIG_PATH
 from visual_graph_datasets.config import Config
 from visual_graph_datasets.util import TEMPLATE_ENV
 from visual_graph_datasets.util import get_version
 from visual_graph_datasets.util import sanitize_input
 from visual_graph_datasets.util import ensure_folder, open_editor
 from visual_graph_datasets.data import create_datasets_metadata
+from visual_graph_datasets.data import gather_visual_graph_dataset_metadata
+from visual_graph_datasets.data import load_visual_graph_dataset_metadata
 from visual_graph_datasets.web import AbstractFileShare, PROVIDER_CLASS_MAP, get_file_share
 
 # == CLI UTILS ==
 
 CM = u'✓'
 
 
@@ -53,15 +58,19 @@
 @click.command('bundle', short_help='bundle all datasets in a folder to make them ready for upload')
 @click.argument('path', type=click.Path(dir_okay=True, exists=True))
 @click.option('-f', '--force', is_flag=True,
               help='Replaces existing files')
 @click.option('--no-compress', is_flag=True,
               help='Skips the compression of the dataset folders itself and only does metadata')
 @click.pass_context
-def bundle(ctx, path: str, force: bool, no_compress: bool):
+def bundle(ctx,
+           path: str,
+           force: bool,
+           no_compress: bool,
+           ) -> None:
     """
     Will interpret all the folders within the given directory PATH as visual graph datasets. These datasets
     will be processed such that they can be uploaded to the remote file share location. This mainly includes
     two steps:
 
     (1) a new metadata.json file for the remote file share location is created from all the datasets.
 
@@ -70,23 +79,25 @@
     By default, operations will be skipped when the corresponding files already exist. Use the --force flag
     to force a replacement
     """
     config = ctx.obj
 
     # ~ creating the metadata file for all the datasets in that path
     echo_info('creating metadata for all datasets')
-    metadata = create_datasets_metadata(path)
     metadata_path = os.path.join(path, 'metadata.json')
-    if os.path.exists(metadata_path) and not force:
-        echo_info('metadata already exists, skipping ...')
-    else:
-        with open(metadata_path, mode='w') as file:
-            json.dump(metadata, file, indent=4)
+    metadata = {}
+    if os.path.exists(metadata_path):
+        with open(metadata_path, mode='r') as file:
+            metadata.update(json.load(file))
+
+    metadata.update(create_datasets_metadata(path))
+    with open(metadata_path, mode='w') as file:
+        json.dump(metadata, file, indent=4, sort_keys=False)
 
-        echo_success(f'created metadata.json @ {metadata_path}')
+    echo_success(f'created metadata.json @ {metadata_path}')
 
     # ~ compressing all the datasets into ZIP which can then be directly uploaded to the remote fileshare
     if no_compress:
         echo_info('skipping zip archiving...')
     else:
         echo_info('packing datasets into ZIP archives')
         members: t.List[str] = os.listdir(path)  # list of file and folder names in the given folder path
@@ -104,14 +115,55 @@
                         format='zip',
                         root_dir=path,
                         base_dir=member
                     )
                     echo_success(f'created "{member}" archive @ {zip_path}')
 
 
+@click.command('gather', short_help='gathers the metadata for a single dataset folder')
+@click.argument('path', type=click.Path(exists=True, dir_okay=True, file_okay=False))
+@click.option('--no-validate', is_flag=True,
+              help='do not raise an error when a problem with dataset is detected during calculation of '
+                   'metadata properties')
+@click.pass_context
+def gather_dataset(ctx,
+                   path: str,
+                   no_validate: bool,
+                   ) -> None:
+    """
+    Gathers all metadata information for a visual graph dataset given the string PATH to the dataset folder.
+    """
+    config = ctx.obj
+
+    dataset_name = os.path.basename(path)
+
+    # This function does all the heavy lifting for this command already: First it loads the entire dataset
+    # including the existing metadata, then it calculates the metadata properties freshly from the dataset
+    # elements itself and then merges the generated properties with the existing ones that were loaded.
+    # It returns the already updated dict
+    echo_info(f'gathering metadata for: {dataset_name}')
+    metadata_map = gather_visual_graph_dataset_metadata(
+        path,
+        logger=config.logger,
+        validate=not no_validate,
+    )
+    print(metadata_map)
+
+    metadata_path = os.path.join(path, '.meta.yaml')
+    with open(metadata_path, mode='w') as file:
+        yaml.dump(metadata_map, file, sort_keys=False)
+
+    with open(metadata_path, mode='r') as file:
+        content = file.read()
+
+    echo_success('gathered metadata:')
+    click.echo(content)
+    echo_success(f'updated file: {metadata_path}')
+
+
 @click.command('config', short_help='open the config file in editor')
 @click.option('-f', '--force', is_flag=True,
               help='replaces the config file if one already exists')
 @click.pass_context
 def edit_config(ctx, force: bool):
     """
     Opens the config file in the systems default text editor
@@ -164,14 +216,30 @@
 
     echo_info(f'using file share provider: {provider}', verbose)
     file_share: AbstractFileShare = get_file_share(config, provider)
     echo_info(f'downloading dataset metadata from file share', verbose)
     metadata = file_share.download_metadata()
     echo_success(f'downloaded metadata:', verbose)
 
+    # Here we iterate through all the datasets listed in the remote metadata file and check if they are
+    # also already available on the local machine, since this is very relevant information to the user
+    # to judge whether a dataset still needs to be downloaded or not.
+    # Additionally, we load the local metadata file to display the local version string so that it can be
+    # compared to the remote version string - Another important information to judge whether a
+    # re-download is necessary!
+    for dataset_name, dataset_meta in metadata['datasets'].items():
+        dataset_path = os.path.join(datasets_path, dataset_name)
+        if os.path.exists(dataset_path):
+            dataset_meta['__exists'] = True
+            dataset_meta['__location'] = dataset_path
+
+            local_meta, _ = load_visual_graph_dataset_metadata(dataset_path)
+            if 'version' in local_meta:
+                dataset_meta['__version'] = local_meta['version']
+
     template = TEMPLATE_ENV.get_template('list.out.j2')
     content = template.render(**{
         'metadata': metadata,
         'datasets_path': datasets_path
     })
 
     click.secho(content)
@@ -222,15 +290,32 @@
     echo_info(f'using file share provider: {provider}')
     file_share: AbstractFileShare = get_file_share(config, provider)
     file_share.download_dataset(dataset_name, datasets_path)
 
     echo_success(f'downloaded dataset "{dataset_name}" @ {dataset_path}')
 
 
+@click.command('info', short_help='display metadata information about an available dataset')
+@click.argument('dataset_name', type=click.STRING)
+@click.option('-p', '--provider', type=click.STRING, default='main')
+@click.pass_context
+def info_dataset(ctx,
+                 dataset_name: str,
+                 provider: str,
+                 ) -> None:
+    config = ctx.obj
+    file_share: AbstractFileShare = get_file_share(config, provider)
+
+    with tempfile.TemporaryDirectory() as folder_path:
+        file_share.download_file(f'dataset_name')
+
+
 cli.add_command(edit_config)
 cli.add_command(download_dataset)
 cli.add_command(bundle)
 cli.add_command(list_datasets)
+cli.add_command(gather_dataset)
+cli.add_command(info_dataset)
 
 
 if __name__ == '__main__':
     cli()
```

### Comparing `visual_graph_datasets-0.8.0/visual_graph_datasets/config.py` & `visual_graph_datasets-0.9.0/visual_graph_datasets/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 Some of the things that are done in this module would semantically fit better into a "utils" module, such
 as the Singleton class. The problem is however, that almost all other parts of the program need access to
 the config singleton, including the utils module. This means that this module here cannot have any other
 project internal dependencies as that would lead to circular dependencies with all the other modules needing
 to access the config...
 """
 import os
+import sys
+import logging
+
 import yaml
 import pathlib
 import platform
 import typing as t
 
 HOME_PATH = pathlib.Path.home()
 FOLDER_PATH = os.path.join(HOME_PATH, '.visual_graph_datasets')
@@ -79,14 +82,16 @@
 
     The data from the config file is not loaded by default, only after invoking ``load`` method. Each
     call to that method will freshly load the data from the file.
     """
     def __init__(self):
         self.data = {}
         self.path: t.Optional[str] = None
+        self.logger = logging.Logger('MAIN')
+        self.logger.addHandler(logging.StreamHandler(sys.stdout))
 
     def load(self, path: str = CONFIG_PATH):
         self.path = path
         self.data = load_config(path=path)
 
     def get_folder_path(self) -> t.Optional[str]:
         return os.path.dirname(self.path)
```

### Comparing `visual_graph_datasets-0.8.0/visual_graph_datasets/examples/readme_00.py` & `visual_graph_datasets-0.9.0/visual_graph_datasets/examples/readme_00.py`

 * *Files identical despite different names*

### Comparing `visual_graph_datasets-0.8.0/visual_graph_datasets/experiments/generate_mock.py` & `visual_graph_datasets-0.9.0/visual_graph_datasets/experiments/generate_mock.py`

 * *Files identical despite different names*

### Comparing `visual_graph_datasets-0.8.0/visual_graph_datasets/experiments/generate_molecule_multitask_dataset_from_csv.py` & `visual_graph_datasets-0.9.0/visual_graph_datasets/experiments/generate_molecule_multitask_dataset_from_csv.py`

 * *Files identical despite different names*

### Comparing `visual_graph_datasets-0.8.0/visual_graph_datasets/experiments/generate_molecule_solubility_12.py` & `visual_graph_datasets-0.9.0/visual_graph_datasets/experiments/generate_tadf_multi.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,20 @@
 """
-Generates a single molecule-based "visual graph dataset2 by merging multiple CSV files containing molecular
-SMILES codes and target value annotations.
+Generates a single molecule-based "visual graph dataset" by merging multiple CSV files containing molecular
+SMILES codes and target value annotations. More specifically, the outcome of this experiment is a visual
+graph dataset whose elements and visualizations represent molecules. The target will be a multitask
+regression problem, where every molecule is associated with a vector of multiple cont. regression targets.
+
+**CHANGELOG**
+
+0.1.0 - 16.12.2022 - Initial version
+
+0.1.1 - 30.12.2022 - Fixed a bug, where smiles representing single atoms were able to enter the dataset.
+These single node graphs would cause problems down the line for graph neural networks since they do not
+include any edges at all. Such molecules are now filtered and NOT added to the final VGD.
 """
 import os
 import shutil
 import sys
 import json
 import csv
 import typing as t
@@ -30,14 +40,15 @@
 from visual_graph_datasets.processing.molecules import mol_from_smiles
 from visual_graph_datasets.processing.molecules import OneHotEncoder
 from visual_graph_datasets.visualization.base import create_frameless_figure
 from visual_graph_datasets.visualization.molecules import visualize_molecular_graph_from_mol
 from visual_graph_datasets.data import NumericJsonEncoder
 from visual_graph_datasets.data import load_visual_graph_dataset
 
+VERSION = '0.1.1'
 SHORT_DESCRIPTION = (
     'Generates a single molecule-based "visual graph dataset" by merging multiple CSV files containing '
     'molecular SMILES codes and target values annotations.'
 )
 
 # == SOURCE PARAMETERS ==
 # This section contains the parameters which define the source CSV files which are to be used as the basis
@@ -51,60 +62,30 @@
 # files
 FILE_SHARE_PROVIDER: str = 'main'
 # The keys of this dictionary should be unique keys which identify the theme of each CSV file to be used in
 # the subsequent merge. The values should be paths to the CSV files. If local files are to be used,
 # the absolute(!) paths have to be supplied. Alternatively, if the paths cannot be found on the local system,
 # they will be interpreted as path relative to the remote file share provider and it is attempted to
 # download those files from there.
-BASE = '/home/jonas/Downloads/12_datasets'
 CSV_FILE_NAME_MAP: t.Dict[str, str] = {
-    'water': os.path.join(BASE, 'water_solubility_data.csv'),
-    'aqua': os.path.join(BASE, 'aqua_cure.csv'),
-    'aqsol': os.path.join(BASE, 'aqsol_cure.csv'),
-    'aqueous_sol': os.path.join(BASE, 'AqueousSolu.csv'),
-    'esol': os.path.join(BASE, 'esol_cure.csv'),
-    'curated': os.path.join(BASE, 'curated_solubility_dataset.csv'),
-    'delany': os.path.join(BASE, 'delaney.csv'),
-    'ochem': os.path.join(BASE, 'ochem_cure.csv'),
-    'phys': os.path.join(BASE, 'phys_cure.csv'),
-    'benzene': os.path.join(BASE, 'benzene_solubility_data.csv'),
-    'acetone': os.path.join(BASE, 'acetone_solubility_data.csv'),
-    'ethanol': os.path.join(BASE, 'ethanol_solubility_data.csv'),
+    'tadf': 'source/tadf.csv',
 }
 # The keys should be the same keys as defined above for each of the CSV files and the values should be the
 # string names of the columns of each file, which contain the SMILES string.
 SMILES_COLUMN_NAME_MAP: t.Dict[str, str] = {
-    'water': 'SMILES',
-    'aqua': 'SMILES',
-    'aqsol': 'SMILES',
-    'aqueous_sol': 'SMILES',
-    'esol': 'SMILES',
-    'curated': 'SMILES',
-    'delany': 'SMILES',
-    'ochem': 'SMILES',
-    'phys': 'SMILES',
-    'benzene': 'SMILES',
-    'acetone': 'SMILES',
-    'ethanol': 'SMILES',
+    'tadf': 'smiles',
 }
 # THe keys should be the same as defined above for each of the CSV files and the values should be lists
 # containing all the string column names which contain the target values of the corresponding dataset.
 TARGET_COLUMN_NAME_MAP: t.Dict[str, t.List[str]] = {
-    'water': ['LogS'],
-    'aqua': ['LogS'],
-    'aqsol': ['LogS'],
-    'aqueous_sol': ['LogS'],
-    'esol': ['LogS'],
-    'curated': ['LogS'],
-    'delany': ['LogS'],
-    'ochem': ['LogS'],
-    'phys': ['LogS'],
-    'benzene': ['LogS'],
-    'acetone': ['LogS'],
-    'ethanol': ['LogS'],
+    'tadf': [
+        'splitting',   # singlet-triplet splitting energy gap E_st
+        'strength',    # The oscillator strength f_osc
+        'absorption',  # k_tadf
+    ],
 }
 SOURCE_KEYS = list(CSV_FILE_NAME_MAP.keys())  # do not modify
 
 # == PROCESSING PARAMETERS ==
 # This section contains the parameters for the processing pipeline. These for example
 
 # boolean flag whether to represent undirected edges as two directed edges in opposite directions.
@@ -175,41 +156,28 @@
 }
 
 # == DATASET PARAMETERS ==
 # This section defines parameters for the creation of the visual graph dataset.
 
 # This will be the name of the finished visual graph dataset folder. This dataset folder can be found in the
 # archive folder of the experiment run.
-DATASET_NAME: str = 'solubility_12'
+DATASET_NAME: str = 'tadf_multi'
 # The width and height (in pixels) with which the visualizations will be created.
 IMAGE_WIDTH: int = 1000
 IMAGE_HEIGHT: int = 1000
 
-
-def is_graph_invalid(g: tc.GraphDict) -> bool:
-    only_single_atom = len(g['node_indices']) == 1
-    edge_indices_shape_invalid = len(g['edge_indices'].shape) != 2
-    edge_attributes_shape_invalid = len(g['edge_attributes'].shape) != 2
-
-    return any([
-        only_single_atom,
-        edge_indices_shape_invalid,
-        edge_attributes_shape_invalid
-    ])
-
-
 # == EVALUATION PARAMETERS ==
 EVAL_LOG_STEP = 100
 NUM_BINS = 10
 PLOT_COLOR = 'gray'
 
 # == EXPERIMENT PARAMETERS ==
 DEBUG = True
 BASE_PATH = os.getcwd()
-NAMESPACE = 'results/generate_molecule_multitask_dataset_from_csv/solubility_12'
+NAMESPACE = 'results/generate_molecule_multitask_dataset_from_csv/tadf_multi'
 with Skippable(), (e := Experiment(base_path=BASE_PATH, namespace=NAMESPACE, glob=globals())):
     e.info('generating a molecule visual graph dataset from CSV source file...')
     config = Config()
     config.load()
 
     # -- get source datasets --
     # As for the sources there are two possibilities: Either we use local files or we download the files
@@ -302,15 +270,14 @@
     e['dataset_path'] = dataset_path
 
     e.info('creating visual graph dataset...')
     for c, (index, d) in enumerate(index_data_map.items()):
         # ~ Convert the Mol object into a GraphDict
         data: dict = d['data']
         mol: Chem.Mol = d['mol']
-        smiles: str = data['smiles']
         atoms = mol.GetAtoms()
         bonds = mol.GetBonds()
 
         g = {}
         target = data['target']
         g['graph_labels'] = np.array(target)
```

### Comparing `visual_graph_datasets-0.8.0/visual_graph_datasets/experiments/update_rb_colors.py` & `visual_graph_datasets-0.9.0/visual_graph_datasets/experiments/update_rb_colors.py`

 * *Files identical despite different names*

### Comparing `visual_graph_datasets-0.8.0/visual_graph_datasets/generation/__pycache__/graph.cpython-310.pyc` & `visual_graph_datasets-0.9.0/visual_graph_datasets/generation/__pycache__/graph.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `visual_graph_datasets-0.8.0/visual_graph_datasets/generation/graph.py` & `visual_graph_datasets-0.9.0/visual_graph_datasets/generation/graph.py`

 * *Files identical despite different names*

### Comparing `visual_graph_datasets-0.8.0/visual_graph_datasets/processing/__pycache__/molecules.cpython-310.pyc` & `visual_graph_datasets-0.9.0/visual_graph_datasets/processing/__pycache__/molecules.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `visual_graph_datasets-0.8.0/visual_graph_datasets/processing/molecules.py` & `visual_graph_datasets-0.9.0/visual_graph_datasets/processing/molecules.py`

 * *Files identical despite different names*

### Comparing `visual_graph_datasets-0.8.0/visual_graph_datasets/templates/config.yaml.j2` & `visual_graph_datasets-0.9.0/visual_graph_datasets/templates/config.yaml.j2`

 * *Files identical despite different names*

### Comparing `visual_graph_datasets-0.8.0/visual_graph_datasets/testing.py` & `visual_graph_datasets-0.9.0/visual_graph_datasets/testing.py`

 * *Files identical despite different names*

### Comparing `visual_graph_datasets-0.8.0/visual_graph_datasets/util.py` & `visual_graph_datasets-0.9.0/visual_graph_datasets/util.py`

 * *Files identical despite different names*

### Comparing `visual_graph_datasets-0.8.0/visual_graph_datasets/visualization/__pycache__/base.cpython-310.pyc` & `visual_graph_datasets-0.9.0/visual_graph_datasets/visualization/__pycache__/base.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `visual_graph_datasets-0.8.0/visual_graph_datasets/visualization/__pycache__/colors.cpython-310.pyc` & `visual_graph_datasets-0.9.0/visual_graph_datasets/visualization/__pycache__/colors.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `visual_graph_datasets-0.8.0/visual_graph_datasets/visualization/__pycache__/importances.cpython-310.pyc` & `visual_graph_datasets-0.9.0/visual_graph_datasets/visualization/__pycache__/importances.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `visual_graph_datasets-0.8.0/visual_graph_datasets/visualization/__pycache__/molecules.cpython-310.pyc` & `visual_graph_datasets-0.9.0/visual_graph_datasets/visualization/__pycache__/molecules.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `visual_graph_datasets-0.8.0/visual_graph_datasets/visualization/base.py` & `visual_graph_datasets-0.9.0/visual_graph_datasets/visualization/base.py`

 * *Files identical despite different names*

### Comparing `visual_graph_datasets-0.8.0/visual_graph_datasets/visualization/colors.py` & `visual_graph_datasets-0.9.0/visual_graph_datasets/visualization/colors.py`

 * *Files identical despite different names*

### Comparing `visual_graph_datasets-0.8.0/visual_graph_datasets/visualization/importances.py` & `visual_graph_datasets-0.9.0/visual_graph_datasets/visualization/importances.py`

 * *Files identical despite different names*

### Comparing `visual_graph_datasets-0.8.0/visual_graph_datasets/visualization/molecules.py` & `visual_graph_datasets-0.9.0/visual_graph_datasets/visualization/molecules.py`

 * *Files identical despite different names*

### Comparing `visual_graph_datasets-0.8.0/visual_graph_datasets/web.py` & `visual_graph_datasets-0.9.0/visual_graph_datasets/web.py`

 * *Files identical despite different names*

### Comparing `visual_graph_datasets-0.8.0/setup.py` & `visual_graph_datasets-0.9.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -26,17 +26,17 @@
  'pycomex>=0.6.1',
  'pytest>=7.2.0',
  'pyyaml>=0.6.0',
  'rdkit>=2022.9.0']
 
 setup_kwargs = {
     'name': 'visual-graph-datasets',
-    'version': '0.8.0',
+    'version': '0.9.0',
     'description': 'Datasets for the training of graph neural networks (GNNs) and subsequent visualization of attributional explanations of XAI methods',
-    'long_description': '|made-with-python| |python-version| |os-linux|\n\n.. |os-linux| image:: https://img.shields.io/badge/os-linux-orange.svg\n   :target: https://www.python.org/\n\n.. |python-version| image:: https://img.shields.io/badge/Python-3.8.0-green.svg\n   :target: https://www.python.org/\n\n.. |made-with-kgcnn| image:: https://img.shields.io/badge/Made%20with-KGCNN-blue.svg\n   :target: https://github.com/aimat-lab/gcnn_keras\n\n.. |made-with-python| image:: https://img.shields.io/badge/Made%20with-Python-1f425f.svg\n   :target: https://www.python.org/\n\n=====================\nVisual Graph Datasets\n=====================\n\nThis package supplies management and utilities for **graph datasets** used to train **graph neural networks**\nand more specifically aimed at **explainable AI (XAI)** methods\n\nW.r.t to the structure and management of these datasets this package employs a different philosophy. Instead of the\nusual minimal packaging to CSV files, a visual graph dataset (VGD) represents each **dataset as a folder** where\neach element is represented by two files:\n\n- A ``json`` file containing metadata information, including the **full graph representation**\n- A ``png`` file containing a canonical visualization of the graph.\n\nWe believe that providing a canonical graph representation as well as a canonical visualization will help to\nmake AI methods trained on such datasets more comparable. The canonical visualization and standard utilities for\nthe visualization of attributional XAI explanations specifically are aimed to improve the comparability and\nreproducability of XAI methods in the future.\n\nInstallation\n============\n\nFirst clone this repository:\n\n.. code-block:: console\n\n    git clone https://github/username/visual_graph_datasets.git\n\nThen install it like this:\n\n.. code-block:: console\n\n    cd visual_graph_datasets\n    pip3 install -e .\n\nCommand Line Interface\n======================\n\nDownload datasets\n-----------------\n\n    **NOTE**: We *strongly* encourage to store datasets on an SSD instead of an HDD, as this can make a\n    difference of multiple hours(!) when loading especially large datasets.\n\nDatasets can simply be downloaded by name by using the ``download`` command:\n\n.. code-block:: console\n\n    // Example for the dataset \'rb_dual_motifs\'\n    python3 -m visual_graph_datasets.cli download "rb_dual_motifs"\n\nBy default this dataset will be downloaded into the folder ``$HOME/.visual_graph_datasets/datasets``\nwhere HOME is the current users home directory.\n\nThe dataset download destination can be changed in a config file by using the ``config`` command:\n\n.. code-block:: console\n\n    python3 -m visual_graph_datasets.cli config\n\nThis command will open the config file at ``$HOME/.visual_graph_datasets/config.yaml`` using the systems\ndefault text editor.\n\nList available datasets\n-----------------------\n\nYou can display a list of all the currently available datasets of the current remote file share provider\nand some metadata information about them by using the command ``list``:\n\n.. code-block:: console\n\n    python3 -m visual_graph_datasets.cli list\n\nQuickstart\n==========\n\nThe datasets are mainly intended to be used in combination with other packages, but this package provides\nsome basic utilities to load and explore the datasets themselves within python programs.\n\n.. code-block:: python\n\n    import os\n    import typing as t\n    import matplotlib.pyplot as plt\n\n    from visual_graph_datasets.config import Config\n    from visual_graph_datasets.web import ensure_dataset\n    from visual_graph_datasets.data import load_visual_graph_dataset\n    from visual_graph_datasets.visualization.base import draw_image\n    from visual_graph_datasets.visualization.importances import plot_node_importances_border\n    from visual_graph_datasets.visualization.importances import plot_edge_importances_border\n\n    # This object will load the settings from the main config file. This config file contains options\n    # such as changing the default datasets folder and defining custom alternative file share providers\n    config = Config()\n    config.load()\n\n    # First of all we need to make sure that the dataset exists locally, this function will download it from\n    # the default file share provider if it does not exist.\n    ensure_dataset(\'rb_dual_motifs\', config)\n\n    # Afterwards we can be sure that the datasets exists and can now load it from the default datasets path.\n    # The data will be loaded as a dictionary whose int keys are the indices of the corresponding elements\n    # and the values are dictionaries which contain all the relevant data about the dataset element,\n    # (Dataset format is explained below)\n    dataset_path = os.path.join(config.get_datasets_path(), \'rb_dual_motifs\')\n    data_index_map: t.Dict[int, dict] = {}\n    _, data_index_map = load_visual_graph_dataset(dataset_path)\n\n    # Using this information we can visualize the ground truth importance explanation annotations for one\n    # element of the dataset like this.\n    index = 0\n    data = data_index_map[index]\n    # This is the dictionary which represents the graph structure of the dataset element. Descriptive\n    # string keys and numpy array values.\n    g = data[\'metadata\'][\'graph\']\n    fig, ax = plt.subplots(ncols=1, nrows=1, figsize=(10, 10))\n    draw_image(ax, image_path=data[\'image_path\'])\n    plot_node_importances_border(\n        ax=ax,\n        g=g,\n        node_positions=g[\'image_node_positions\'],\n        node_importances=g[\'node_importances_2\'][:, 0],\n    )\n    plot_edge_importances_border(\n        ax=ax,\n        g=g,\n        node_positions=g[\'image_node_positions\'],\n        edge_importances=g[\'edge_importances_2\'][:, 0],\n    )\n    fig_path = os.path.join(os.getcwd(), \'importances.pdf\')\n    fig.savefig(fig_path)\n\n\nDataset Format\n==============\n\nAssuming the following shape definitions:\n\n- V - the number of nodes in a graph\n- E - the number of edges in a graph\n- N - the number of node attributes / features associated with each node\n- M - the number of edge attributes / features associated with each edge\n- K - the number of importance channels\n\nOne such content dictionary which are the values of the two dicts returned by the function have the\nfollowing nested dictionary structure:\n\n- ``image_path``: The absolute path to the image file that visualizes this element\n- ``metadata_path``: the absolute path to the metadata file\n- ``metadata``: A dict which contains all the metadata for that element\n    - ``target``: a 1d array containing the target values for the element. For classification this usually\n      a one-hot encoded class vector already.\n    - ``index``: The canonical index of this element within the dataset\n    - ``graph``: A dictionary which contains the entire graph representation of this element.\n        - ``node_indices``: array of shape (V, 1) with the integer node indices.\n        - ``node_attributes``: array of shape (V, N)\n        - ``edge_indices``: array of shape (E, 2) which are the tuples of integer node indices that\n          determine edges\n        - ``edge_attributes``: array of shape (E, M)\n        - ``node_positions`` array of shape (V, 2) which are the xy positions of each node in pixel\n          values within the corresponding image visualization of the element. This is the crucial\n          information which is required to use the existing image representations to visualize attributional\n          explanations!\n        - (``node_importances_{K}_{suffix}``) array of shape (V, K) containing ground truth node importance\n          explanations, which assign an importance value of 0 to 1 to each node of the graph across K channels.\n          One dataset element may have none or multiple such annotations with different suffixes\n          determining the number of explanation channels and origin.\n        - (``edge_importances_{K}_{suffix}``) array of shape (E, K) containing ground truth edge importance\n          explanations, which assign an importance value of 0 to 1 to each edge of the graph across K channels.\n          One dataset element may have none or multiple such annotations with different suffixes\n          determining the number of explanation channels and origin.\n\n\nDatasets\n========\n\nHere is a list of the datasets currently included.\n\nFor more information about the individual datasets use the ``list`` command in the CLI (see above).\n\n* TO BE DONE\n\n',
+    'long_description': '|made-with-python| |python-version| |os-linux|\n\n.. |os-linux| image:: https://img.shields.io/badge/os-linux-orange.svg\n   :target: https://www.python.org/\n\n.. |python-version| image:: https://img.shields.io/badge/Python-3.8.0-green.svg\n   :target: https://www.python.org/\n\n.. |made-with-kgcnn| image:: https://img.shields.io/badge/Made%20with-KGCNN-blue.svg\n   :target: https://github.com/aimat-lab/gcnn_keras\n\n.. |made-with-python| image:: https://img.shields.io/badge/Made%20with-Python-1f425f.svg\n   :target: https://www.python.org/\n\n=====================\nVisual Graph Datasets\n=====================\n\nThis package supplies management and utilities for **graph datasets** used to train **graph neural networks**\nand more specifically aimed at **explainable AI (XAI)** methods\n\nW.r.t to the structure and management of these datasets this package employs a different philosophy. Instead of the\nusual minimal packaging to CSV files, a visual graph dataset (VGD) represents each **dataset as a folder** where\neach element is represented by two files:\n\n- A ``json`` file containing metadata information, including the **full graph representation**\n- A ``png`` file containing a canonical visualization of the graph.\n\nWe believe that providing a canonical graph representation as well as a canonical visualization will help to\nmake AI methods trained on such datasets more comparable. The canonical visualization and standard utilities for\nthe visualization of attributional XAI explanations specifically are aimed to improve the comparability and\nreproducability of XAI methods in the future.\n\nInstallation\n============\n\nFirst clone this repository:\n\n.. code-block:: console\n\n    git clone https://github/username/visual_graph_datasets.git\n\nThen install it like this:\n\n.. code-block:: console\n\n    cd visual_graph_datasets\n    pip3 install -e .\n\nCommand Line Interface\n======================\n\nDownload datasets\n-----------------\n\n    **NOTE**: We *strongly* encourage to store datasets on an SSD instead of an HDD, as this can make a\n    difference of multiple hours(!) when loading especially large datasets.\n\nDatasets can simply be downloaded by name by using the ``download`` command:\n\n.. code-block:: console\n\n    // Example for the dataset \'rb_dual_motifs\'\n    python3 -m visual_graph_datasets.cli download "rb_dual_motifs"\n\nBy default this dataset will be downloaded into the folder ``$HOME/.visual_graph_datasets/datasets``\nwhere HOME is the current users home directory.\n\nThe dataset download destination can be changed in a config file by using the ``config`` command:\n\n.. code-block:: console\n\n    python3 -m visual_graph_datasets.cli config\n\nThis command will open the config file at ``$HOME/.visual_graph_datasets/config.yaml`` using the systems\ndefault text editor.\n\nList available datasets\n-----------------------\n\nYou can display a list of all the currently available datasets of the current remote file share provider\nand some metadata information about them by using the command ``list``:\n\n.. code-block:: console\n\n    python3 -m visual_graph_datasets.cli list\n\nQuickstart\n==========\n\nThe datasets are mainly intended to be used in combination with other packages, but this package provides\nsome basic utilities to load and explore the datasets themselves within python programs.\n\n.. code-block:: python\n\n    import os\n    import typing as t\n    import matplotlib.pyplot as plt\n\n    from visual_graph_datasets.config import Config\n    from visual_graph_datasets.web import ensure_dataset\n    from visual_graph_datasets.data import load_visual_graph_dataset\n    from visual_graph_datasets.visualization.base import draw_image\n    from visual_graph_datasets.visualization.importances import plot_node_importances_border\n    from visual_graph_datasets.visualization.importances import plot_edge_importances_border\n\n    # This object will load the settings from the main config file. This config file contains options\n    # such as changing the default datasets folder and defining custom alternative file share providers\n    config = Config()\n    config.load()\n\n    # First of all we need to make sure that the dataset exists locally, this function will download it from\n    # the default file share provider if it does not exist.\n    ensure_dataset(\'rb_dual_motifs\', config)\n\n    # Afterwards we can be sure that the datasets exists and can now load it from the default datasets path.\n    # The data will be loaded as a dictionary whose int keys are the indices of the corresponding elements\n    # and the values are dictionaries which contain all the relevant data about the dataset element,\n    # (Dataset format is explained below)\n    dataset_path = os.path.join(config.get_datasets_path(), \'rb_dual_motifs\')\n    data_index_map: t.Dict[int, dict] = {}\n    _, data_index_map = load_visual_graph_dataset(dataset_path)\n\n    # Using this information we can visualize the ground truth importance explanation annotations for one\n    # element of the dataset like this.\n    index = 0\n    data = data_index_map[index]\n    # This is the dictionary which represents the graph structure of the dataset element. Descriptive\n    # string keys and numpy array values.\n    g = data[\'metadata\'][\'graph\']\n    fig, ax = plt.subplots(ncols=1, nrows=1, figsize=(10, 10))\n    draw_image(ax, image_path=data[\'image_path\'])\n    plot_node_importances_border(\n        ax=ax,\n        g=g,\n        node_positions=g[\'image_node_positions\'],\n        node_importances=g[\'node_importances_2\'][:, 0],\n    )\n    plot_edge_importances_border(\n        ax=ax,\n        g=g,\n        node_positions=g[\'image_node_positions\'],\n        edge_importances=g[\'edge_importances_2\'][:, 0],\n    )\n    fig_path = os.path.join(os.getcwd(), \'importances.pdf\')\n    fig.savefig(fig_path)\n\n\nDataset Format\n==============\n\nVisual Graph Datasets are represented as *folders* containing multiple files. The primary content of these\ndataset folders is made up of *2* files per element in the dataset:\n\n- **A PNG file**. This is the canonical visualization of the graph which can subsequently be used to create\n  explanation visualizations as well. The pixel position of each node in the graph is attached as metadata\n  of the graph representation.\n\n- **A JSON file**. Primarily contains the *full* graph representation consisting of node attributes, edge\n  attributes, an edge list etc. May also contain custom metadata for each graph depending on the dataset.\n\nOptionally, a dataset folder may also contain a ``.meta.yml`` file which contains additional metadata about\nthe dataset as a whole.\n\nElement Metadata JSON\n---------------------\n\nOne such metadata file belonging to one element of the dataset may have the following nested structure:\n\n- ``target``: a 1d array containing the target values for the element. For classification this usually\n  a one-hot encoded vector of classes already. For multi-task regression this vector may have an\n  arbitrary number of continuous regression targets. For single-task regression this will still be a\n  vector, albeit with the shape (1, )\n- ``index``: The canonical index of this element within the dataset\n- (``train_split`` *optional*) A list of int indices, where each index represents a different split.\n  if the number "1" is for example part of this list, that means that the corresponding element is\n  considered to be part of the training set of split "1". What each particular split is may be described\n  in the documentation of the dataset.\n- (``test_split`` *optional*) A list of int indices, where each index represents a different split.\n  if the number "1" is for example part of this list, that means that the corresponding element is\n  considered to be part of the test set of the split "1".\n- ``graph``: A dictionary which contains the entire graph representation of this element.\n\n    - ``node_indices``: array of shape (V, 1) with the integer node indices.\n    - ``node_attributes``: array of shape (V, N)\n    - ``edge_indices``: array of shape (E, 2) which are the tuples of integer node indices that\n      determine edges\n    - ``edge_attributes``: array of shape (E, M)\n    - ``node_positions`` array of shape (V, 2) which are the xy positions of each node in pixel\n      values within the corresponding image visualization of the element. This is the crucial\n      information which is required to use the existing image representations to visualize attributional\n      explanations!\n    - (``node_importances_{K}_{suffix}`` *optional*) array of shape (V, K) containing ground truth node importance\n      explanations, which assign an importance value of 0 to 1 to each node of the graph across K channels.\n      One dataset element may have none or multiple such annotations with different suffixes\n      determining the number of explanation channels and origin.\n    - (``edge_importances_{K}_{suffix}`` *optional*) array of shape (E, K) containing ground truth edge importance\n      explanations, which assign an importance value of 0 to 1 to each edge of the graph across K channels.\n      One dataset element may have none or multiple such annotations with different suffixes\n      determining the number of explanation channels and origin.\n\nAssuming the following shape definitions:\n\n- V - the number of nodes in a graph\n- E - the number of edges in a graph\n- N - the number of node attributes / features associated with each node\n- M - the number of edge attributes / features associated with each edge\n- K - the number of importance channels\n\nDataset Metadata YML\n--------------------\n\nOne such metadata file may have the following nested structure. Additionally, it may also contain custom\nadditional fields depending on each dataset.\n\n- ``version``: A string determining the current version of the dataset\n- ``description``: Short string description of what the dataset is about (for example where the data came\n  from, what types of graphs it consists of, what the prediction target is etc.)\n- ``visualization_description``: String description of what can be seen in the visualization of the graph.\n  There are many different types of graphs out there which may have very domain specific visualizations.\n  This string should provide a short description of how the visualizations may be interpreted.\n- ``references``: A list of strings, where each string is a short description of online resources which are\n  relevant to the dataset, usually including a URL. This could for example include references to scientific\n  publications where a dataset was first introduced.\n- ``file_size``: The integer *accumulated* size of all the files that make up the dataset in bytes.\n- ``num_elements``: The integer number of elements in the dataset\n- ``num_targets``: The size of the prediction target vector\n- ``num_node_attributes``: The size of the node attribute vector\n- ``num_edge_attributes``: The size of the edge attribute vector\n\nDatasets\n========\n\nHere is a list of the datasets currently uploaded on the main file share provider.\n\nFor more information about the individual datasets use the ``list`` command in the CLI (see above).\n\n* TO BE DONE\n\n',
     'author': 'awa59kst120df',
     'author_email': 'awa59kst120df@gmail.com',
     'maintainer': 'awa59kst120df',
     'maintainer_email': 'awa59kst120df@gmail.com',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `visual_graph_datasets-0.8.0/PKG-INFO` & `visual_graph_datasets-0.9.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: visual-graph-datasets
-Version: 0.8.0
+Version: 0.9.0
 Summary: Datasets for the training of graph neural networks (GNNs) and subsequent visualization of attributional explanations of XAI methods
 License: MIT
 Keywords: graph neural networks,datasets,explainable AI
 Author: awa59kst120df
 Author-email: awa59kst120df@gmail.com
 Maintainer: awa59kst120df
 Maintainer-email: awa59kst120df@gmail.com
@@ -178,54 +178,96 @@
     fig_path = os.path.join(os.getcwd(), 'importances.pdf')
     fig.savefig(fig_path)
 
 
 Dataset Format
 ==============
 
+Visual Graph Datasets are represented as *folders* containing multiple files. The primary content of these
+dataset folders is made up of *2* files per element in the dataset:
+
+- **A PNG file**. This is the canonical visualization of the graph which can subsequently be used to create
+  explanation visualizations as well. The pixel position of each node in the graph is attached as metadata
+  of the graph representation.
+
+- **A JSON file**. Primarily contains the *full* graph representation consisting of node attributes, edge
+  attributes, an edge list etc. May also contain custom metadata for each graph depending on the dataset.
+
+Optionally, a dataset folder may also contain a ``.meta.yml`` file which contains additional metadata about
+the dataset as a whole.
+
+Element Metadata JSON
+---------------------
+
+One such metadata file belonging to one element of the dataset may have the following nested structure:
+
+- ``target``: a 1d array containing the target values for the element. For classification this usually
+  a one-hot encoded vector of classes already. For multi-task regression this vector may have an
+  arbitrary number of continuous regression targets. For single-task regression this will still be a
+  vector, albeit with the shape (1, )
+- ``index``: The canonical index of this element within the dataset
+- (``train_split`` *optional*) A list of int indices, where each index represents a different split.
+  if the number "1" is for example part of this list, that means that the corresponding element is
+  considered to be part of the training set of split "1". What each particular split is may be described
+  in the documentation of the dataset.
+- (``test_split`` *optional*) A list of int indices, where each index represents a different split.
+  if the number "1" is for example part of this list, that means that the corresponding element is
+  considered to be part of the test set of the split "1".
+- ``graph``: A dictionary which contains the entire graph representation of this element.
+
+    - ``node_indices``: array of shape (V, 1) with the integer node indices.
+    - ``node_attributes``: array of shape (V, N)
+    - ``edge_indices``: array of shape (E, 2) which are the tuples of integer node indices that
+      determine edges
+    - ``edge_attributes``: array of shape (E, M)
+    - ``node_positions`` array of shape (V, 2) which are the xy positions of each node in pixel
+      values within the corresponding image visualization of the element. This is the crucial
+      information which is required to use the existing image representations to visualize attributional
+      explanations!
+    - (``node_importances_{K}_{suffix}`` *optional*) array of shape (V, K) containing ground truth node importance
+      explanations, which assign an importance value of 0 to 1 to each node of the graph across K channels.
+      One dataset element may have none or multiple such annotations with different suffixes
+      determining the number of explanation channels and origin.
+    - (``edge_importances_{K}_{suffix}`` *optional*) array of shape (E, K) containing ground truth edge importance
+      explanations, which assign an importance value of 0 to 1 to each edge of the graph across K channels.
+      One dataset element may have none or multiple such annotations with different suffixes
+      determining the number of explanation channels and origin.
+
 Assuming the following shape definitions:
 
 - V - the number of nodes in a graph
 - E - the number of edges in a graph
 - N - the number of node attributes / features associated with each node
 - M - the number of edge attributes / features associated with each edge
 - K - the number of importance channels
 
-One such content dictionary which are the values of the two dicts returned by the function have the
-following nested dictionary structure:
+Dataset Metadata YML
+--------------------
 
-- ``image_path``: The absolute path to the image file that visualizes this element
-- ``metadata_path``: the absolute path to the metadata file
-- ``metadata``: A dict which contains all the metadata for that element
-    - ``target``: a 1d array containing the target values for the element. For classification this usually
-      a one-hot encoded class vector already.
-    - ``index``: The canonical index of this element within the dataset
-    - ``graph``: A dictionary which contains the entire graph representation of this element.
-        - ``node_indices``: array of shape (V, 1) with the integer node indices.
-        - ``node_attributes``: array of shape (V, N)
-        - ``edge_indices``: array of shape (E, 2) which are the tuples of integer node indices that
-          determine edges
-        - ``edge_attributes``: array of shape (E, M)
-        - ``node_positions`` array of shape (V, 2) which are the xy positions of each node in pixel
-          values within the corresponding image visualization of the element. This is the crucial
-          information which is required to use the existing image representations to visualize attributional
-          explanations!
-        - (``node_importances_{K}_{suffix}``) array of shape (V, K) containing ground truth node importance
-          explanations, which assign an importance value of 0 to 1 to each node of the graph across K channels.
-          One dataset element may have none or multiple such annotations with different suffixes
-          determining the number of explanation channels and origin.
-        - (``edge_importances_{K}_{suffix}``) array of shape (E, K) containing ground truth edge importance
-          explanations, which assign an importance value of 0 to 1 to each edge of the graph across K channels.
-          One dataset element may have none or multiple such annotations with different suffixes
-          determining the number of explanation channels and origin.
+One such metadata file may have the following nested structure. Additionally, it may also contain custom
+additional fields depending on each dataset.
 
+- ``version``: A string determining the current version of the dataset
+- ``description``: Short string description of what the dataset is about (for example where the data came
+  from, what types of graphs it consists of, what the prediction target is etc.)
+- ``visualization_description``: String description of what can be seen in the visualization of the graph.
+  There are many different types of graphs out there which may have very domain specific visualizations.
+  This string should provide a short description of how the visualizations may be interpreted.
+- ``references``: A list of strings, where each string is a short description of online resources which are
+  relevant to the dataset, usually including a URL. This could for example include references to scientific
+  publications where a dataset was first introduced.
+- ``file_size``: The integer *accumulated* size of all the files that make up the dataset in bytes.
+- ``num_elements``: The integer number of elements in the dataset
+- ``num_targets``: The size of the prediction target vector
+- ``num_node_attributes``: The size of the node attribute vector
+- ``num_edge_attributes``: The size of the edge attribute vector
 
 Datasets
 ========
 
-Here is a list of the datasets currently included.
+Here is a list of the datasets currently uploaded on the main file share provider.
 
 For more information about the individual datasets use the ``list`` command in the CLI (see above).
 
 * TO BE DONE
```

