# Comparing `tmp/cagraph-0.0.1-py3-none-any.whl.zip` & `tmp/cagraph-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,12 @@
-Zip file size: 12824 bytes, number of entries: 9
+Zip file size: 18641 bytes, number of entries: 10
 -rw-r--r--  2.0 unx     6148 b- defN 20-Feb-02 00:00 cagraph/.DS_Store
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 cagraph/__init__.py
--rw-r--r--  2.0 unx    18904 b- defN 20-Feb-02 00:00 cagraph/cagraph.py
--rw-r--r--  2.0 unx    10069 b- defN 20-Feb-02 00:00 cagraph/preprocess.py
--rw-r--r--  2.0 unx     9593 b- defN 20-Feb-02 00:00 cagraph/visualization.py
-?rw-r--r--  2.0 unx      906 b- defN 20-Feb-02 00:00 cagraph-0.0.1.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 cagraph-0.0.1.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1073 b- defN 20-Feb-02 00:00 cagraph-0.0.1.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx      685 b- defN 20-Feb-02 00:00 cagraph-0.0.1.dist-info/RECORD
-9 files, 47465 bytes uncompressed, 11658 bytes compressed:  75.4%
+-rw-r--r--  2.0 unx    45484 b- defN 20-Feb-02 00:00 cagraph/cagraph.py
+-rw-r--r--  2.0 unx    16835 b- defN 20-Feb-02 00:00 cagraph/preprocess.py
+-rw-r--r--  2.0 unx    12493 b- defN 20-Feb-02 00:00 cagraph/visualization.py
+?rw-r--r--  2.0 unx      857 b- defN 20-Feb-02 00:00 cagraph-0.0.2.dist-info/METADATA
+?rw-r--r--  2.0 unx       83 b- defN 20-Feb-02 00:00 cagraph-0.0.2.dist-info/WHEEL
+?rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 cagraph-0.0.2.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     1073 b- defN 20-Feb-02 00:00 cagraph-0.0.2.dist-info/license_files/LICENSE
+?rw-r--r--  2.0 unx      785 b- defN 20-Feb-02 00:00 cagraph-0.0.2.dist-info/RECORD
+10 files, 83758 bytes uncompressed, 17309 bytes compressed:  79.3%
```

## zipnote {}

```diff
@@ -9,20 +9,23 @@
 
 Filename: cagraph/preprocess.py
 Comment: 
 
 Filename: cagraph/visualization.py
 Comment: 
 
-Filename: cagraph-0.0.1.dist-info/METADATA
+Filename: cagraph-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: cagraph-0.0.1.dist-info/WHEEL
+Filename: cagraph-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: cagraph-0.0.1.dist-info/licenses/LICENSE
+Filename: cagraph-0.0.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: cagraph-0.0.1.dist-info/RECORD
+Filename: cagraph-0.0.2.dist-info/license_files/LICENSE
+Comment: 
+
+Filename: cagraph-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cagraph/cagraph.py

```diff
@@ -1,546 +1,1148 @@
 # CaGraph imports
+import preprocess as prep
 import numpy as np
 import networkx as nx
 import matplotlib.pyplot as plt
 import seaborn as sns
 from pynwb import NWBHDF5IO
-from statsmodels.tsa.stattools import grangercausalitytests
+import pandas as pd
+import os
 
-# %% CaGraph class
 
+# %% CaGraph class
 class CaGraph:
     """
-    Published: XX/XX/XXXX
-    Author: Veronica Porubsky [Github: https://github.com/vporubsky][ORCID: https://orcid.org/0000-0001-7216-3368]
+    Author: Veronica Porubsky
+    Author Github: https://github.com/vporubsky
+    Author ORCID: https://orcid.org/0000-0001-7216-3368
 
-    Class: CaGraph(data_file, identifiers=None)
+    Class: CaGraph(data_file, node_labels=None, node_metadata=None, dataset_id=None, threshold=None)
     =====================
 
     This class provides functionality to easily visualize time-series data of
     neuronal activity and to compute correlation metrics of neuronal networks,
     and generate graph objects which can be analyzed using graph theory.
     There are several graph theoretical metrics for further analysis of
     neuronal network connectivity patterns.
 
     Attributes
     ----------
-    data_file : str
-        A string pointing to the file to be used for data analysis.
-    labels: list
-        A list of identifiers for each row of calcium imaging data in
-        the data_file passed to CaGraph.
+    data : str or numpy.ndarray
+        A string pointing to the file to be used for data analysis, or a numpy.ndarray containing data loaded into
+        memory. The first (idx 0) row must contain timepoints, the subsequent rows each represent a single neuron timeseries
+        of calcium fluorescence data sampled at the timepoints specified in the first row.
+    node_labels: list
+        A list of identifiers for each row of calcium imaging data (each neuron) in the data_file passed to CaGraph.
+    node_metadata: dict
+        Contains metadata which is associated with neurons in the network. Each key in the dictionary will be added as an
+        attribute to the CaGraph object, and the associated value will be .
+        Each value
     dataset_id: str
+        A unique identifier can be added to the CaGraph object.
     threshold: float
-
+        Sets a threshold to be used for thresholded graph.
     """
 
-    def __init__(self, data_file, labels=None, dataset_id=None, threshold=None):
+    def __init__(self, data, node_labels=None, node_metadata=None, dataset_id=None, threshold=None):
         """
-
-        :param data_file: str
-        :param labels:
+        :param data: str
+        :param node_labels: list
+        :param node_metadata: dict
         :param dataset_id: str
+        :param threshold: float
         """
-        if isinstance(data_file, np.ndarray):
-            self.data = data_file
-            self.time = self.data[0, :]
-            self.neuron_dynamics = self.data[1:len(self.data), :]
-        elif data_file.endswith('csv'):
-            self.data = np.genfromtxt(data_file, delimiter=",")
-            self.time = self.data[0, :]
-            self.neuron_dynamics = self.data[1:len(self.data), :]
-        elif data_file.endswith('nwb'):
-            with NWBHDF5IO(data_file, 'r') as io:
-                nwbfile_read = io.read()
-                nwb_acquisition_key = list(nwbfile_read.acquisition.keys())[0]
-                ca_from_nwb = nwbfile_read.acquisition[nwb_acquisition_key]
-                self.neuron_dynamics = ca_from_nwb.data[:]
-                self.time = ca_from_nwb.timestamps[:]
+        # Check that the input data is in the correct format and load dataset
+        if isinstance(data, np.ndarray):
+            self._data = data
+            self._time = self._data[0, :]
+            self._neuron_dynamics = self._data[1:len(self._data), :]
+        elif isinstance(data, str):
+            if data.endswith('csv'):
+                self._data = np.genfromtxt(data, delimiter=",")
+                self._time = self._data[0, :]
+                self._neuron_dynamics = self._data[1:len(self._data), :]
+            elif data.endswith('nwb'):
+                with NWBHDF5IO(data, 'r') as io:
+                    nwbfile_read = io.read()
+                    nwb_acquisition_key = list(nwbfile_read.acquisition.keys())[0]
+                    ca_from_nwb = nwbfile_read.acquisition[nwb_acquisition_key]
+                    self._neuron_dynamics = ca_from_nwb.data[:]
+                    self._time = ca_from_nwb.timestamps[:]
+                    self._data = np.vstack((self._time, self._neuron_dynamics))
+            else:
+                raise TypeError('File path must have a .csv or .nwb file to load.')
         else:
-            print('Data must be passed as a .csv or .nwb file, or as numpy.ndarray.')
-            raise TypeError
+            raise TypeError('Data must be passed as a str containing a .csv or .nwb file, or as numpy.ndarray.')
+
+        # Add dataset identifier
         if dataset_id is not None:
-            self.data_id = dataset_id
-        self.data_filename = str(data_file)
-        self.time = self.data[0, :]
-        self.dt = self.time[1] - self.time[0]
-        self.neuron_dynamics = self.data[1:len(self.data), :]
-        self.num_neurons = np.shape(self.neuron_dynamics)[0]
-        if labels is None:
-            self.labels = np.linspace(0, np.shape(self.neuron_dynamics)[0] - 1,
-                                      np.shape(self.neuron_dynamics)[0]).astype(int)
+            self._data_id = dataset_id
+
+        # Compute time interval and number of neurons
+        self._dt = self._time[1] - self._time[0]
+        self._num_neurons = np.shape(self._neuron_dynamics)[0]
+
+        # Generate node labels
+        if node_labels is None:
+            self._node_labels = np.linspace(0, np.shape(self._neuron_dynamics)[0] - 1,
+                                            np.shape(self._neuron_dynamics)[0]).astype(int)
         else:
-            self.labels = labels
-        self.pearsons_correlation_matrix = np.nan_to_num(np.corrcoef(self.neuron_dynamics))
+            self._node_labels = node_labels
+
+        # Initialize correlation matrix, threshold, and graph
+        self._pearsons_correlation_matrix = self.get_pearsons_correlation_matrix()
         if threshold is not None:
-            self.threshold = threshold
+            self._threshold = threshold
         else:
-            self.threshold = self.__generate_threshold()
-
-
-    def __generate_threshold(self):
-        """
-        Future version will implement preprocessing threshold auto-detection.
-
-        """
-        # prep.generate_threshold(data=tmp)
-        return 0.3
-
-    def get_laplacian_matrix(self, graph=None):
-        """
-        Returns the Laplacian matrix of the specified graph.
-
-        :param graph:
-        :return:
-        """
-        if graph is None:
-            graph = self.get_network_graph_from_matrix()
-        return nx.laplacian_matrix(graph)
-
-    def get_network_graph_from_matrix(self, weighted=False):
-        """
-        Automatically generate graph object from numpy adjacency matrix.
+            self._threshold = self.__generate_threshold()
+        self._graph = self.get_graph()
 
-        :param weighted:
-        :return:
-        """
-        if not weighted:
-            return nx.from_numpy_array(self.get_adjacency_matrix())
-        return nx.from_numpy_array(self.get_weight_matrix())
+        # Store initial settings to reset attributes after modification
+        self.__init_threshold = self._threshold
+        self.__init_pearsons_correlation_matrix = self._pearsons_correlation_matrix
+        self.__init_graph = self._graph
+
+        # Initialize subclass objects
+        self.graph_theory = self.GraphTheory(neuron_dynamics=self._neuron_dynamics, time=self._time,
+                                             num_neurons=self._num_neurons,
+                                             pearsons_correlation_matrix=self._pearsons_correlation_matrix,
+                                             graph=self._graph, labels=self._node_labels)
+
+        self.plotting = self.Plotting(neuron_dynamics=self._neuron_dynamics, time=self._time,
+                                      num_neurons=self._num_neurons,
+                                      pearsons_correlation_matrix=self._pearsons_correlation_matrix, graph=self._graph)
+
+        # Initialize base graph theory analyses
+        self._degree = self.graph_theory.get_degree(return_type='dict')
+        self._clustering_coefficient = self.graph_theory.get_clustering_coefficient(return_type='dict')
+        self._correlated_pair_ratio = self.graph_theory.get_correlated_pair_ratio(return_type='dict')
+        self._communities = self.graph_theory.get_communities(return_type='dict')
+        self._hubs = self.graph_theory.get_hubs(return_type='dict')
+        self._hits = self.graph_theory.get_hits_values(return_type='dict')
+        self._eigenvector_centrality = self.graph_theory.get_eigenvector_centrality(return_type='dict')
+
+        # Build private attribute dictionary
+        self.__attribute_dictionary = {'hubs': self.hubs, 'degree': self.degree,
+                                       'clustering coefficient': self.clustering_coefficient,
+                                       'communities': self.communities,
+                                       'eigenvector centrality': self.eigenvector_centrality,
+                                       'correlated pair ratio': self.correlated_pair_ratio, 'HITS': self.hits}
+
+        # Add node metadata
+        if node_metadata is not None:
+            for key in node_metadata.keys():
+                if type(node_metadata[key]) is list or np.ndarray:
+                    if len(node_metadata[key]) != len(self._node_labels):
+                        raise ValueError('Each key-value pair in the node_metadata dictionary must have a value to be '
+                                         'associated with every node.')
+                    node_metadata_dict = {}
+                    for i, value in enumerate(node_metadata[key]):
+                        node_metadata_dict[self._node_labels[i]] = value
+                    self.__attribute_dictionary[key] = node_metadata_dict
+                    setattr(self, key, node_metadata_dict)
+                elif type(node_metadata[key]) is dict:
+                    self.__attribute_dictionary[key] = node_metadata
+                    setattr(self, key, node_metadata[key])
+                else:
+                    raise AttributeError('Each key-value pair in the node_metadata dictionary must have a value'
+                                         'supplied as type list, one-dimensional numpy.ndarray, or as a dictionary'
+                                         'where each key is a node and each value is the metadata value for that node.')
+
+    # Private utility methods
+    @property
+    def data(self):
+        return self._data
+
+    @property
+    def time(self):
+        return self._time
+
+    @property
+    def neuron_dynamics(self):
+        return self._neuron_dynamics
+
+    @property
+    def dt(self):
+        return self._dt
+
+    @property
+    def num_neurons(self):
+        return self._num_neurons
+
+    @property
+    def data_id(self):
+        return self._data_id
+
+    @property
+    def node_labels(self):
+        return self._node_labels
+
+    @property
+    def pearsons_correlation_matrix(self):
+        return self._pearsons_correlation_matrix
+
+    @property
+    def graph(self):
+        return self._graph
+
+    @property
+    def degree(self):
+        return self._degree
+
+    @property
+    def clustering_coefficient(self):
+        return self._clustering_coefficient
+
+    @property
+    def correlated_pair_ratio(self):
+        return self._correlated_pair_ratio
+
+    @property
+    def communities(self):
+        return self._communities
+
+    @property
+    def hubs(self):
+        return self._hubs
+
+    @property
+    def hits(self):
+        return self._hits
+
+    @property
+    def eigenvector_centrality(self):
+        return self._eigenvector_centrality
+
+    @property
+    def threshold(self):
+        return self._threshold
+
+    @threshold.setter
+    def threshold(self, value):
+        self._threshold = value
+        self._pearsons_correlation_matrix = self.get_pearsons_correlation_matrix()
+        self._graph = self.get_graph()
+        self._degree = self.graph_theory.get_degree(return_type='dict')
+        self._clustering_coefficient = self.graph_theory.get_clustering_coefficient(return_type='dict')
+        self._correlated_pair_ratio = self.graph_theory.get_correlated_pair_ratio(return_type='dict')
+        self._communities = self.graph_theory.get_communities(return_type='dict')
+        self._hubs = self.graph_theory.get_hubs(return_type='dict')
+        self._hits = self.graph_theory.get_hits_values(return_type='dict')
+        self._eigenvector_centrality = self.graph_theory.get_eigenvector_centrality(return_type='dict')
+
+    def __generate_threshold(self) -> float:
+        """
+        Generates a threshold for the provided dataset as described in the preprocess module.
+
+        :return: float
+        """
+        return prep.generate_threshold(data=self._neuron_dynamics)
+
+    def __parse_by_node(self, node_data, node_list) -> list:
+        """
+        Method to parse report analyses using only a subset of nodes.
+
+        :param node_data: list
+        :param node_list: list
+        :return: list
+        """
+        return [node_data[i] for i in node_list if i < len(node_data)]
+
+    # Public utility methods
+    def reset(self):
+        """
+        Resets the CaGraph object graph attribute to the original state at the time the object was created.
+        """
+        self._pearsons_correlation_matrix = self.__init_pearsons_correlation_matrix
+        self._threshold = self.__init_threshold
+        self._graph = self.__init_graph
+
+        # Re-initialize base graph theory analyses
+        self._degree = self.graph_theory.get_degree()
+        self._clustering_coefficient = self.graph_theory.get_clustering_coefficient()
+        self._correlated_pair_ratio = self.graph_theory.get_correlated_pair_ratio()
+        self._communities = self.graph_theory.get_communities()
+        self._hubs = self.graph_theory.get_hubs()
 
-    def get_pearsons_correlation_matrix(self, data_matrix=None, time_points=None):
+    # Statistics and linear algebra methods
+    def get_pearsons_correlation_matrix(self, data_matrix=None) -> np.ndarray:
         """
         Returns the Pearson's correlation for all neuron pairs.
 
-        :param data_matrix:
-        :param time_points: tuple
+        A loaded numpy.ndarray dataset can be passed to the method for analysis, otherwise
+        the dataset passed to the CaGraph object constructor will be used.
+
+        :param data_matrix: numpy.ndarray
         :return:
         """
         if data_matrix is None:
-            data_matrix = self.neuron_dynamics
-        if time_points:
-            data_matrix = data_matrix[:, time_points[0]:time_points[1]]
+            data_matrix = self._neuron_dynamics
         return np.nan_to_num(np.corrcoef(data_matrix, rowvar=True))
 
-    def get_time_subsampled_graphs(self, subsample_indices, weighted=False):
-        """
 
-        :param weighted:
-        :param subsample_indices: list of tuples
-        :return:
+    def get_adjacency_matrix(self) -> np.ndarray:
         """
-        subsampled_graphs = []
-        for time_idx in subsample_indices:
-            subsampled_graphs.append(
-                self.get_network_graph(corr_mat=self.get_pearsons_correlation_matrix(time_points=time_idx),
-                                       weighted=weighted))
-        return subsampled_graphs
+        Returns the adjacency matrix of a graph where edges exist when greater than the provided threshold.
 
-    def get_time_subsampled_correlation_matrices(self, subsample_indices):
-        """
-        Samples the timeseries using provided indices to generate correlation matrices for
-        defined periods.
+        Uses the Pearson's correlation matrix.
 
-        :param subsample_indices: list of tuples
-        :return:
-        """
-        subsampled_corr_mat = []
-        for time_idx in subsample_indices:
-            subsampled_corr_mat.append(self.get_pearsons_correlation_matrix(time_points=time_idx))
-        return subsampled_corr_mat
-
-    def get_granger_causality_scores_matrix(self):
-        """
-        Returns Granger causality chi-square values.
-
-        :return:
+        :return: numpy.ndarray
         """
-        r, c = np.shape(self.neuron_dynamics)
-        gc_matrix = np.zeros((r, r))
-        for row in range(r):
-            for col in range(r):
-                gc_test_dict = grangercausalitytests(np.transpose(self.neuron_dynamics[[row, col], :]),
-                                                     maxlag=1, verbose=False)[1][0]
-                gc_matrix[row, col] = gc_test_dict['ssr_chi2test'][1]
-        return gc_matrix
+        adj_mat = (self._pearsons_correlation_matrix > self._threshold).astype(int)
+        np.fill_diagonal(adj_mat, 0)
+        return adj_mat
 
-    def get_adjacency_matrix(self):
+    def get_laplacian_matrix(self, graph=None) -> np.ndarray:
         """
-        Returns the adjacency matrix.
+        Returns the Laplacian matrix of the specified graph.
 
+        :param graph: networkx.Graph object
         :return:
         """
-        adj_mat = (self.pearsons_correlation_matrix > self.threshold)
-        np.fill_diagonal(adj_mat, 0)
-        return adj_mat.astype(int)
+        if graph is None:
+            graph = self.get_graph()
+        return nx.laplacian_matrix(graph).toarray()
 
-    def get_weight_matrix(self):
+    def get_weight_matrix(self) -> np.ndarray:
         """
         Returns a weighted connectivity matrix with zero along the diagonal. No threshold is applied.
 
-        :return:
+        :return: numpy.ndarray
         """
-        weight_matrix = self.pearsons_correlation_matrix
+        weight_matrix = self._pearsons_correlation_matrix
         np.fill_diagonal(weight_matrix, 0)
         return weight_matrix
 
-    def plot_correlation_heatmap(self, correlation_matrix=None, show_plot=True):
+    # Graph construction methods
+    def get_graph(self, weighted=False) -> nx.Graph:
         """
-        Plots a heatmap of the correlation matrix.
+        Automatically generate graph object from numpy adjacency matrix.
 
-        :param show_plot:
-        :param correlation_matrix:
-        :return:
+        :param weighted: bool
+        :return: networkx.Graph object
         """
-        if correlation_matrix is None:
-            correlation_matrix = self.get_pearsons_correlation_matrix()
-        sns.heatmap(correlation_matrix, vmin=0, vmax=1)
-        if show_plot:
-            plt.show()
-        return
+        if not weighted:
+            return nx.from_numpy_array(self.get_adjacency_matrix())
+        return nx.from_numpy_array(self.get_weight_matrix())
 
-    def get_single_neuron_timecourse(self, neuron_trace_number):
+    def get_random_graph(self, graph=None) -> nx.Graph:
         """
-        Return time vector stacked on the recorded neuron of interest.
+        Generates a random graph. The nx.algorithms.smallworld.random_reference is adapted from the
+        Maslov and Sneppen (2002) algorithm. It randomizes the existing graph.
 
-        :param neuron_trace_number:
-        :return:
+        :type graph: networkx.Graph object
+        :return: networkx.Graph object
         """
-        neuron_timecourse_selection = neuron_trace_number
-        return np.vstack((self.time, self.neuron_dynamics[neuron_timecourse_selection, :]))
+        if graph is None:
+            graph = self.get_graph()
+        graph = nx.algorithms.smallworld.random_reference(graph)
+        return graph
 
-    def plot_single_neuron_timecourse(self, neuron_trace_number, title=None):
+    def get_erdos_renyi_graph(self, graph=None) -> nx.Graph:
         """
+        Generates an Erdos-Renyi random graph using a graph edge density metric computed from the graph to be randomized.
 
-        :param title:
-        :param neuron_trace_number:
-        :return:
+        :param graph:
+        :return: networkx.Graph object
         """
-        neuron_timecourse_selection = neuron_trace_number
-        count = 1
-        x_tick_array = []
-        for i in range(len(self.time)):
-            if count % (len(self.time) / 20) == 0:
-                x_tick_array.append(self.time[i])
-            count += 1
-        plt.figure(num=1, figsize=(10, 2))
-        plt.plot(self.time, self.neuron_dynamics[neuron_timecourse_selection, :],
-                 linewidth=1)  # add option : 'xkcd:olive',
-        plt.xticks(x_tick_array)
-        plt.xlim(0, self.time[-1])
-        plt.ylabel('ΔF/F')
-        plt.xlabel('Time (s)')
-        if title is None:
-            plt.title(f'{self.data_id} neuron {neuron_timecourse_selection}')
+        if graph is None:
+            num_nodes = self._num_neurons
+            con_probability = self.graph_theory.get_graph_density()
         else:
-            plt.title(title)
-        plt.show()
+            num_nodes = len(graph.nodes)
+            con_probability = self.graph_theory.get_graph_density(graph=graph)
+        return nx.erdos_renyi_graph(n=num_nodes, p=con_probability)
 
-    def plot_multi_neuron_timecourse(self, neuron_trace_labels, title=None, palette=None, show=False):
+    def draw_graph(self, graph=None, position=None, node_size=25, node_color='b', alpha=0.5):
         """
-        Plots multiple individual calcium fluorescence traces, stacked vertically.
+        Draws a simple graph.
 
-        :param show:
-        :param palette:
-        :param neuron_trace_labels:
-        :param title:
+        :param graph: networkx.Graph object
+        :param position: dict
+        :param node_size: int
+        :param node_color: str
+        :param alpha: float
         :return:
         """
-        count = 0
-        if palette is None:
-            palette = sns.color_palette('husl', len(neuron_trace_labels))
-        for idx, neuron in enumerate(neuron_trace_labels):
-            y = self.neuron_dynamics[neuron, :].copy() / max(self.neuron_dynamics[neuron, :])
-            y = [x + 1.05 * count for x in y]
-            plt.plot(self.time, y, c=palette[idx], linewidth=1)
-            plt.xticks([])
-            plt.yticks([])
-            count += 1
-        plt.ylabel('ΔF/F')
-        plt.xlabel('Time (s)')
-        if title:
-            plt.title(title)
-        if show:
-            plt.show()
-
-    def plot_subnetworks_timecourses(self, graph=None, palette=None, title=None):
-        """
+        if graph is None:
+            graph = self._graph
+        if position is None:
+            position = nx.spring_layout(graph)
+        nx.draw(graph, pos=position, node_size=node_size, node_color=node_color, alpha=alpha)
 
-        :param palette:
-        :param graph:
-        :param title:
-        :return:
+    def get_report(self, parsing_nodes=None, parse_by_attribute=None, parsing_operation=None,
+                   parsing_value=None, save_report=False, save_path=None, save_filename=None, save_filetype=None):
         """
-        subnetworks = self.get_subnetworks(graph=graph)
-        if palette is None:
-            palette = sns.color_palette('husl', self.num_neurons)
-        for idx, subnetwork in enumerate(subnetworks):
-            count = 0
-            for neuron in subnetwork:
-                y = self.neuron_dynamics[neuron, :].copy() / max(self.neuron_dynamics[neuron, :])
-                for j in range(len(y)):
-                    y[j] = y[j] + 1.05 * count
-                plt.plot(self.time, y, c=palette[idx], linewidth=1)
-                plt.xticks([])
-                plt.yticks([])
+        :param save_filetype:
+        :param save_filename:
+        :param save_path:
+        :param save_report:
+        :param parsing_nodes:
+        :param parse_by_attribute: str
+        :param parsing_operation: str
+        :param parsing_value: float
+        :return: dict
+        """
+        # Set up parsing
+        if parse_by_attribute is not None:
+            # identify nodes that meet the parsing criteria
+            if parsing_operation == '>':
+                parsing_nodes = [key for key, value in self.__attribute_dictionary[parse_by_attribute].items() if
+                                 value > parsing_value]
+            elif parsing_operation == '<':
+                parsing_nodes = [key for key, value in self.__attribute_dictionary[parse_by_attribute].items() if
+                                 value < parsing_value]
+            elif parsing_operation == '<=':
+                parsing_nodes = [key for key, value in self.__attribute_dictionary[parse_by_attribute].items() if
+                                 value <= parsing_value]
+            elif parsing_operation == '>=':
+                parsing_nodes = [key for key, value in self.__attribute_dictionary[parse_by_attribute].items() if
+                                 value >= parsing_value]
+            elif parsing_operation == '==':
+                parsing_nodes = [key for key, value in self.__attribute_dictionary[parse_by_attribute].items() if
+                                 value == parsing_value]
+            elif parsing_operation == '!=':
+                parsing_nodes = [key for key, value in self.__attribute_dictionary[parse_by_attribute].items() if
+                                 value != parsing_value]
+
+        # Individual node analyses
+        if parsing_nodes is None:
+            parsing_nodes = self._node_labels
+        report_dict = {}
+        for key in self.__attribute_dictionary.keys():
+            report_dict[key] = self.__parse_by_node(node_data=self.__attribute_dictionary[key], node_list=parsing_nodes)
+
+        # Construct report dataframe
+        report_df = pd.DataFrame.from_dict(report_dict, orient='columns')
+        report_df.index = parsing_nodes
+
+        # Save report
+        if save_report:
+            if save_filename is None:
+                save_filename = 'report'
+            if save_path is None:
+                save_path = os.getcwd() + '/'
+            if save_filetype is None or save_filetype == 'csv':
+                report_df.to_csv(save_path + save_filename + '.csv', index=True)
+            elif save_filetype == 'HDF5':
+                report_df.to_hdf(save_path + save_filename + '.h5', key=save_filename, mode='w')
+            elif save_filetype == 'xlsx':
+                report_df.to_excel(save_path + save_filename + 'xlsx', index=True)
+        return report_df
+
+    class GraphTheory:
+        def __init__(self, neuron_dynamics, time, pearsons_correlation_matrix, graph, num_neurons, labels):
+            self._time = time
+            self._neuron_dynamics = neuron_dynamics
+            self._num_neurons = num_neurons
+            self._pearsons_correlation_matrix = pearsons_correlation_matrix
+            self._graph = graph
+            self._node_labels = labels
+
+        # Private utility methods
+        @property
+        def time(self):
+            return self._time
+
+        @property
+        def neuron_dynamics(self):
+            return self._neuron_dynamics
+
+        @property
+        def num_neurons(self):
+            return self._num_neurons
+
+        @property
+        def graph(self):
+            return self._graph
+
+        @property
+        def node_labels(self):
+            return self._node_labels
+
+        @property
+        def pearsons_correlation_matrix(self):
+            return self._pearsons_correlation_matrix
+
+        # Graph theory analysis
+        def get_hubs(self, graph=None, return_type='list'):
+            """
+            Computes hub nodes in the graph using the HITS algorithm. Hubs are identified by finding
+            those nodes which have a hub value greater than the median of the hubs values plus 2.5 time the standard deviation.
+
+            :param graph: networkx.Graph object
+            :param return_type: str
+            """
+            if graph is None:
+                hubs, authorities = nx.hits(self._graph, max_iter=500)
+            else:
+                hubs, authorities = nx.hits(graph, max_iter=500)
+            med_hubs = np.median(list(hubs.values()))
+            std_hubs = np.std(list(hubs.values()))
+            hubs_threshold = med_hubs + 2.5 * std_hubs
+            hubs_list = []
+            [hubs_list.append(x) for x in hubs.keys() if hubs[x] > hubs_threshold]
+            hub_dict = {i: 1 if i in list(set(hubs_list) & set(self._node_labels)) else 0 for i in self._node_labels}
+            if return_type == 'dict':
+                return hub_dict
+            if return_type == 'list':
+                return list(hub_dict.values())
+
+        def get_hits_values(self, graph=None, return_type='list'):
+            """
+            Computes hub nodes in the graph and returns a list of nodes identified as hubs.
+            HITS and authorities values match due to bidirectional edges.
+
+            :param graph: networkx.Graph object
+            :param return_type: str
+            """
+            if graph is None:
+                graph = self._graph
+            hits_dict, authorities_dict = nx.hits(graph, max_iter=500)
+            if return_type == 'dict':
+                return hits_dict
+            if return_type == 'list':
+                return list(hits_dict.values())
+
+        def get_connected_components(self, graph=None) -> list:
+            """
+            Returns connected components with more than one node.
+
+            :param graph: networkx.Graph object
+            :return: list
+            """
+            if graph is None:
+                connected_components_with_orphan = list(nx.connected_components(self._graph))
+            else:
+                connected_components_with_orphan = list(nx.connected_components(graph))
+            connected_components = []
+            [connected_components.append(list(map(int, x))) for x in connected_components_with_orphan if len(x) > 1]
+            return connected_components
+
+        def get_largest_connected_component(self, graph=None) -> nx.Graph:
+            """
+            Returns a subgraph containing the largest connected component.
+
+            :param graph: networkx.Graph object
+            :return: networkx.Graph object
+            """
+            if graph is None:
+                graph = self._graph
+            largest_component = max(nx.connected_components(graph), key=len)
+            return graph.subgraph(largest_component)
+
+        def get_clustering_coefficient(self, graph=None, return_type='list'):
+            """
+            Returns a list of clustering coefficient values for each node.
+
+            :param graph: networkx.Graph object
+            :param return_type: str
+            """
+            if graph is None:
+                graph = self._graph
+            degree_view = nx.clustering(graph)
+            clustering_coefficient = []
+            [clustering_coefficient.append(degree_view[node]) for node in graph.nodes()]
+            clustering_dict = dict(zip(self._node_labels, clustering_coefficient))
+            if return_type == 'dict':
+                return clustering_dict
+            if return_type == 'list':
+                return list(clustering_dict.values())
+
+        def get_degree(self, graph=None, return_type='list'):
+            """
+            Returns iterator object of (node, degree) pairs.
+
+            :param graph: networkx.Graph object
+            :param return_type: str
+            """
+            if graph is None:
+                graph = self._graph
+            degree_dict = dict(graph.degree)
+            if return_type == 'dict':
+                return degree_dict
+            if return_type == 'list':
+                return list(degree_dict.values())
+
+        def get_correlated_pair_ratio(self, graph=None, return_type='list'):
+            """
+            Computes the number of connections each neuron has, divided by the nuber of cells in the field of view.
+            This method is described in Jimenez et al. 2020: https://www.nature.com/articles/s41467-020-17270-w#Sec8
+
+            :param graph: networkx.Graph object
+            :param return_type: str
+            """
+            if graph is None:
+                graph = self._graph
+            degree_view = self.get_degree(graph)
+            correlated_pair_ratio = []
+            [correlated_pair_ratio.append(degree_view[node] / self._num_neurons) for node in graph.nodes()]
+            correlated_pair_ratio_dict = dict(zip(self._node_labels, correlated_pair_ratio))
+            if return_type == 'dict':
+                return correlated_pair_ratio_dict
+            if return_type == 'list':
+                return list(correlated_pair_ratio_dict.values())
+
+        def get_graph_density(self, graph=None):
+            """
+            Returns the ratio of edges present in the graph out of the total possible edges.
+            The equation used to calculate this ratio is only relevant to undirected graphs.
+
+            :param graph: networkx.Graph object
+            :return: float
+            """
+            possible_edges = (self._num_neurons * (self._num_neurons - 1)) / 2
+            if graph is None:
+                graph = self._graph
+            return len(graph.edges) / possible_edges
+
+        def get_eigenvector_centrality(self, graph=None, return_type='list'):
+            """
+            Compute the eigenvector centrality of all graph nodes, the
+            measure of influence each node has on the graph.
+
+            :param graph: networkx.Graph object
+            :param return_type: str
+            """
+            if graph is None:
+                graph = self._graph
+            eigenvector_centrality = nx.eigenvector_centrality(graph)
+            if return_type == 'dict':
+                return eigenvector_centrality
+            if return_type == 'list':
+                return list(eigenvector_centrality.values())
+
+        def get_communities(self, graph=None, return_type='list'):
+            """
+            Returns a list of communities, composed of a group of nodes.
+
+            :param return_type: list
+            :param graph: networkx.Graph object
+            :return: node_groups: list
+            """
+            if graph is None:
+                graph = self._graph
+            communities = list(nx.algorithms.community.greedy_modularity_communities(graph))
+            sorted(communities)
+            community_id = {}
+            for i in range(len(communities)):
+                for j in list(communities[i]):
+                    community_id[j] = i
+            if return_type == 'dict':
+                return community_id
+            if return_type == 'list':
+                return list(community_id.values())
+
+        def get_smallworld_largest_subnetwork(self, graph=None) -> float:
+            """
+
+            :param graph: networkx.Graph object
+            :return: float
+            """
+            if graph is None:
+                graph = self.get_largest_connected_component()
+            else:
+                graph = self.get_largest_connected_component(graph=graph)
+            if len(graph.nodes()) >= 4:
+                return nx.algorithms.smallworld.sigma(graph)
+            else:
+                raise RuntimeError(
+                    'Largest subgraph has less than four nodes. networkx.algorithms.smallworld.sigma cannot be computed.')
+
+
+    class Plotting:
+        def __init__(self, neuron_dynamics, time, pearsons_correlation_matrix, graph, num_neurons):
+            self._num_neurons = num_neurons
+            self._time = time
+            self._neuron_dynamics = neuron_dynamics
+            self._pearsons_correlation_matrix = pearsons_correlation_matrix
+            self._graph = graph
+
+        # Private utility methods
+        @property
+        def time(self):
+            return self._time
+
+        @property
+        def neuron_dynamics(self):
+            return self._neuron_dynamics
+
+        @property
+        def num_neurons(self):
+            return self._num_neurons
+
+        @property
+        def graph(self):
+            return self._graph
+
+        @property
+        def pearsons_correlation_matrix(self):
+            return self._pearsons_correlation_matrix
+
+        def plot_correlation_heatmap(self, correlation_matrix=None, title=None, y_label=None, x_label=None,
+                                     show_plot=True,
+                                     save_plot=False, save_path=None, dpi=300, save_format='png'):
+            """
+            Plots a heatmap of the correlation matrix.
+
+            :param save_format:
+            :param correlation_matrix:
+            :param title:
+            :param y_label:
+            :param x_label:
+            :param show_plot:
+            :param save_plot:
+            :param save_path:
+            :param dpi:
+            :return:
+            """
+            if correlation_matrix is None:
+                correlation_matrix = self._pearsons_correlation_matrix()
+            sns.heatmap(correlation_matrix, vmin=0, vmax=1)
+            if title is not None:
+                plt.title(title)
+            if y_label is not None:
+                plt.ylabel(y_label)
+            if x_label is not None:
+                plt.xlabel(x_label)
+            if show_plot:
+                plt.show()
+            if save_plot:
+                if save_path is None:
+                    save_path = os.getcwd() + f'fig'
+                plt.savefig(fname=save_path, dpi=dpi, format=save_format)
+
+        def get_single_neuron_timecourse(self, neuron_trace_number) -> np.ndarray:
+            """
+            Return time vector stacked on the recorded calcium fluorescence for the neuron of interest.
+
+            :param neuron_trace_number: int
+            :return: numpy.ndarray
+            """
+            neuron_timecourse_selection = neuron_trace_number
+            return np.vstack((self._time, self._neuron_dynamics[neuron_timecourse_selection, :]))
+
+        def plot_single_neuron_timecourse(self, neuron_trace_number, title=None, y_label=None, x_label=None,
+                                          show_plot=True,
+                                          save_plot=False, save_path=None, dpi=300, save_format='png'):
+            """
+
+            :param save_format:
+            :param neuron_trace_number: int
+            :param title:
+            :param y_label:
+            :param x_label:
+            :param show_plot:
+            :param save_plot:
+            :param save_path:
+            :param dpi:
+            :return:
+            """
+            neuron_timecourse_selection = neuron_trace_number
+            count = 1
+            x_tick_array = []
+            for i in range(len(self._time)):
+                if count % (len(self._time) / 20) == 0:
+                    x_tick_array.append(self._time[i])
                 count += 1
-            plt.ylabel('ΔF/F')
-            plt.xlabel('Time (s)')
-            if title:
+            plt.figure(num=1, figsize=(10, 2))
+            plt.plot(self._time, self._neuron_dynamics[neuron_timecourse_selection, :],
+                     linewidth=1)  # add option : 'xkcd:olive',
+            plt.xticks(x_tick_array)
+            plt.xlim(0, self._time[-1])
+            if title is not None:
                 plt.title(title)
-            plt.show()
-
-    def plot_multi_neurons_timecourses(self, graph=None, title=None):
-        """
-
-        :param graph:
-        :param title:
-        :return:
-        """
-        subnetworks = self.get_subnetworks(graph=graph)
-        for subnetwork in subnetworks:
+            if y_label is not None:
+                plt.ylabel(y_label)
+            else:
+                plt.ylabel('ΔF/F')
+            if x_label is not None:
+                plt.xlabel(x_label)
+            else:
+                plt.xlabel('Time')
+            if show_plot:
+                plt.show()
+            if save_plot:
+                if save_path is None:
+                    save_path = os.getcwd() + f'fig'
+                plt.savefig(fname=save_path, dpi=dpi, format=save_format)
+
+        def plot_multi_neuron_timecourse(self, neuron_trace_labels, palette=None, title=None, y_label=None,
+                                         x_label=None,
+                                         show_plot=True, save_plot=False, save_path=None, dpi=300, save_format='png'):
+            """
+            Plots multiple individual calcium fluorescence traces, stacked vertically.
+
+
+            :param save_format:
+            :param neuron_trace_labels: list
+            :param palette: list
+            :param title:
+            :param y_label:
+            :param x_label:
+            :param show_plot:
+            :param save_plot:
+            :param save_path:
+            :param dpi:
+            :return:
+            """
             count = 0
-            for neuron in subnetwork:
-                y = self.neuron_dynamics[neuron, :].copy() / max(self.neuron_dynamics[neuron, :])
-                for j in range(len(y)):
-                    y[j] = y[j] + 1.05 * count
-                plt.plot(self.time, y, 'k', linewidth=1)
+            if palette is None:
+                palette = sns.color_palette('husl', len(neuron_trace_labels))
+            for idx, neuron in enumerate(neuron_trace_labels):
+                y = self._neuron_dynamics[neuron, :].copy() / max(self._neuron_dynamics[neuron, :])
+                y = [x + 1.05 * count for x in y]
+                plt.plot(self._time, y, c=palette[idx], linewidth=1)
                 plt.xticks([])
                 plt.yticks([])
                 count += 1
-            plt.ylabel('ΔF/F')
-            plt.xlabel('Time (s)')
-            if title:
+            if title is not None:
                 plt.title(title)
-            plt.show()
+            if y_label is not None:
+                plt.ylabel(y_label)
+            else:
+                plt.ylabel('ΔF/F')
+            if x_label is not None:
+                plt.xlabel(x_label)
+            else:
+                plt.xlabel('Time')
+            if show_plot:
+                plt.show()
+            if save_plot:
+                if save_path is None:
+                    save_path = os.getcwd() + f'fig'
+                plt.savefig(fname=save_path, dpi=dpi, format=save_format)
+
+        def plot_all_neurons_timecourse(self, title=None, y_label=None, x_label=None, show_plot=True, save_plot=False,
+                                        save_path=None, dpi=300, save_format='png'):
+            """
+            :param save_format:
+            :param title:
+            :param y_label:
+            :param x_label:
+            :param show_plot:
+            :param save_plot:
+            :param save_path:
+            :param dpi:
+            """
+            plt.figure(num=2, figsize=(10, 2))
+            count = 1
+            x_tick_array = []
+            for i in range(len(self._time)):
+                if count % (len(self._time) / 20) == 0:
+                    x_tick_array.append(self._time[i])
+                count += 1
+            for i in range(len(self._neuron_dynamics) - 1):
+                plt.plot(self._time, self._neuron_dynamics[i, :], linewidth=0.5)
+                plt.xticks(x_tick_array)
+                plt.xlim(0, self._time[-1])
+            if title is not None:
+                plt.title(title)
+            if y_label is not None:
+                plt.ylabel(y_label)
+            else:
+                plt.ylabel('ΔF/F')
+            if x_label is not None:
+                plt.xlabel(x_label)
+            else:
+                plt.xlabel('Time')
+            if show_plot:
+                plt.show()
+            if save_plot:
+                if save_path is None:
+                    save_path = os.getcwd() + f'fig'
+                plt.savefig(fname=save_path, dpi=dpi, format=save_format)
 
-    def plot_all_neurons_timecourse(self):
-        """
 
+# %% Time samples
+class CaGraphTimeSamples:
+    """
+    Class for running time-sample analyses on a single dataset.
+    """
+    def __init__(self, data, time_samples=None, condition_labels=None, node_labels=None, node_metadata=None,
+                 dataset_id=None,
+                 threshold=None):
+        """
+        :param data: str
+        :param time_samples:
+        :param condition_labels:
+        :param node_labels: list
+        :param node_metadata: dict
+        :param dataset_id: str
+        :param threshold: float
         """
-        plt.figure(num=2, figsize=(10, 2))
-        count = 1
-        x_tick_array = []
-        for i in range(len(self.time)):
-            if count % (len(self.time) / 20) == 0:
-                x_tick_array.append(self.time[i])
-            count += 1
-        for i in range(len(self.neuron_dynamics) - 1):
-            plt.plot(self.time, self.neuron_dynamics[i, :], linewidth=0.5)
-            plt.xticks(x_tick_array)
-            plt.xlim(0, self.time[-1])
-            plt.ylabel('ΔF/F')
-            plt.xlabel('Time (s)')
-            plt.title(f'{self.data_id}')
-        plt.show()
+        # Check that the input data is in the correct format and load dataset
+        if isinstance(data, np.ndarray):
+            self._data = data
+        elif isinstance(data, str):
+            if data.endswith('csv'):
+                self._data = np.genfromtxt(data, delimiter=",")
+            elif data.endswith('nwb'):
+                with NWBHDF5IO(data, 'r') as io:
+                    nwbfile_read = io.read()
+                    nwb_acquisition_key = list(nwbfile_read.acquisition.keys())[0]
+                    ca_from_nwb = nwbfile_read.acquisition[nwb_acquisition_key]
+                    self._data = np.vstack((ca_from_nwb.timestamps[:], ca_from_nwb.data[:]))
+            else:
+                raise TypeError('File path must have a .csv or .nwb file to load.')
+        else:
+            raise TypeError('Data must be passed as a str containing a .csv or .nwb file, or as numpy.ndarray.')
 
-    def get_network_graph(self, corr_mat=None, weighted=False):
-        """
-        Must pass a np.ndarray type object to corr_mat, or the Pearsons
-        correlation matrix for the full dataset will be used.
+        # Add dataset identifier
+        if dataset_id is not None:
+            self._data_id = dataset_id
 
-        :param corr_mat:
-        :param weighted:
-        :return:
-        """
-        if not isinstance(corr_mat, np.ndarray):
-            corr_mat = self.pearsons_correlation_matrix  # update to include other correlation metrics
-        graph = nx.Graph()
-        if weighted:
-            for i in range(len(self.labels)):
-                graph.add_node(str(self.labels[i]))
-                for j in range(len(self.labels)):
-                    if not i == j:
-                        graph.add_edge(str(self.labels[i]), str(self.labels[j]), weight=corr_mat[i, j])
+        self._condition_identifiers = condition_labels
+
+        # Compute time interval and number of neurons
+        self._dt = self.data[0, 1] - self.data[0, 0]
+        self._num_neurons = np.shape(self.data)[0]
+        if threshold is not None:
+            self._threshold = threshold
         else:
-            for i in range(len(self.labels)):
-                graph.add_node(str(self.labels[i]))
-                for j in range(len(self.labels)):
-                    if not i == j and corr_mat[i, j] > self.threshold:
-                        graph.add_edge(str(self.labels[i]), str(self.labels[j]))
-        return graph
+            self._threshold = self.__generate_threshold()
 
-    def get_random_graph(self, graph=None):
-        """
-        Generates a random graph. The nx.algorithms.smallworld.random_reference is adapted from the
-        Maslov and Sneppen (2002) algorithm. It randomizes the existing graph.
+        # Generate node labels
+        if node_labels is None:
+            self._node_labels = np.linspace(0, np.shape(self.data)[0] - 2,
+                                            np.shape(self.data)[0] - 1).astype(int)
+        else:
+            self._node_labels = node_labels
 
-        :return:
-        """
-        if graph is None:
-            graph = self.get_network_graph()
-        graph = nx.algorithms.smallworld.random_reference(graph)
-        return graph
+        # Add a series of private attributes which are CaGraph objects
+        for i, sample in enumerate(time_samples):
+            setattr(self, f'__{condition_labels[i]}_cagraph',
+                    CaGraph(data=self._data[:, sample[0]:sample[1]], node_labels=self._node_labels,
+                            node_metadata=node_metadata, threshold=self._threshold))
 
-    def get_erdos_renyi_graph(self, graph=None):
-        """
-        Generates an Erdos-Renyi random graph using a network edge coverage metric computed from the graph to be randomized.
+    # Private utility methods
+    @property
+    def data(self):
+        return self._data
 
-        :param graph:
-        :return:
-        """
-        if graph is None:
-            num_nodes = self.num_neurons
-            con_probability = self.get_network_coverage()
-        else:
-            num_nodes = len(graph.nodes)
-            con_probability = self.get_network_coverage(graph=graph)
-        return nx.erdos_renyi_graph(n=num_nodes, p=con_probability)
+    @property
+    def dt(self):
+        return self._dt
 
-    def plot_graph_network(self, graph, show_labels=True, position=None):
-        """
+    @property
+    def num_neurons(self):
+        return self._num_neurons
 
-        :param show_labels:
-        :param graph:
-        :param position:
-        :return:
-        """
-        if not position:
-            position = nx.spring_layout(graph)
-        nx.draw_networkx_nodes(graph, pos=position, node_color='b', node_size=100)
-        nx.draw_networkx_edges(graph, pos=position, edge_color='b', )
-        if show_labels:
-            nx.draw_networkx_labels(graph, pos=position, font_size=6, font_color='w', font_family='sans-serif')
-        plt.axis('off')
-        plt.show()
-        return
+    @property
+    def data_id(self):
+        return self._data_id
 
-    def get_hubs(self, graph=None):
-        """
-        Computes hub nodes in the graph and returns a list of nodes identified as hubs.
+    @property
+    def node_labels(self):
+        return self._node_labels
 
-        :param graph:
-        :return:
-        """
-        if graph is None:
-            hubs, authorities = nx.hits(self.get_network_graph())
-        else:
-            hubs, authorities = nx.hits(graph)
-        med_hubs = np.median(list(hubs.values()))
-        std_hubs = np.std(list(hubs.values()))
-        hubs_threshold = med_hubs + 2.5 * std_hubs
-        hubs_list = []
-        [hubs_list.append(x) for x in hubs.keys() if hubs[x] > hubs_threshold]
-        return hubs_list, hubs
+    @property
+    def threshold(self):
+        return self._threshold
+
+    @property
+    def condition_identifiers(self):
+        return self._condition_identifiers
 
-    def get_subnetworks(self, graph=None):
+    def __generate_threshold(self) -> float:
         """
+        Generates a threshold for the provided dataset as described in the preprocess module.
+        This threshold generation will use the full dataset.
 
-        :param graph:
-        :return:
+        :return: float
         """
-        if graph is None:
-            connected_components = list(nx.connected_components(self.get_network_graph()))
-        else:
-            connected_components = list(nx.connected_components(graph))
-        subnetworks = []
-        [subnetworks.append(list(map(int, x))) for x in connected_components if len(x) > 1]
-        return subnetworks
+        return prep.generate_threshold(data=self.data)
 
-    def get_largest_subnetwork_graph(self, graph=None):
+    # Public utility methods
+    def get_cagraph(self, condition_label):
         """
 
-        :param graph:
+        :param condition_label:
         :return:
         """
-        if graph is None:
-            graph = self.get_network_graph()
-        largest_component = max(nx.connected_components(graph), key=len)
-        return graph.subgraph(largest_component)
+        return getattr(self, f'__{condition_label}_cagraph')
 
-    def get_clustering_coefficient(self, graph=None) -> list:
+    def get_full_report(self, save_report=False, save_path=None, save_filename=None, save_filetype=None):
         """
-        Returns a list of clustering coefficient values for each node.
+        Generates an organized report of all data in the batched sample. It will report on the
+        base analyses included in the CaGraph object get_report() method, and output a single
+        pandas DataFrame or file which includes these analyses for all datasets in a tabular structure.
 
-        :param graph:
+        :param save_report:
+        :param save_path:
+        :param save_filename:
+        :param save_filetype:
         :return:
         """
-        if graph is None:
-            graph = self.get_network_graph_from_matrix()
-        degree_view = nx.clustering(graph)
-        clustering_coefficient = []
-        [clustering_coefficient.append(degree_view[node]) for node in graph.nodes()]
-        return clustering_coefficient
+        store_reports = {}
+        for key in self._condition_identifiers:
+            cagraph_obj = self.get_cagraph(key)
+            store_reports[key] = cagraph_obj.get_report()
 
-    def get_degree(self, graph=None):
-        """
-        Returns iterator object of (node, degree) pairs.
+        # For each column in the individual reports, append to the full report
+        full_report_df = pd.DataFrame()
+        for col in store_reports[key].columns:
+            for key in store_reports.keys():
+                df = store_reports[key]
+                df = df.rename(columns={col: f'{key}_{col}'})
+                full_report_df = pd.concat([full_report_df, df[f'{key}_{col}']], axis=1)
 
-        :return:
-        """
-        if graph is None:
-            return self.get_network_graph_from_matrix()
-        else:
-            return graph.degree
+        # Save the report
+        if save_report:
+            if save_filename is None:
+                save_filename = 'report'
+            if save_path is None:
+                save_path = os.getcwd() + '/'
+            if save_filetype is None or save_filetype == 'csv':
+                full_report_df.to_csv(save_path + save_filename + '.csv', index=True)
+            elif save_filetype == 'HDF5':
+                full_report_df.to_hdf(save_path + save_filename + '.h5', key=save_filename, mode='w')
+            elif save_filetype == 'xlsx':
+                full_report_df.to_excel(save_path + save_filename + 'xlsx', index=True)
+        return full_report_df
 
-    def get_correlated_pair_ratio(self, graph=None):
-        """
-        Computes the number of connections each neuron has, divided by the nuber of cells in the field of view.
-        This method is described in: https://www.nature.com/articles/s41467-020-17270-w#Sec8
 
-        :param graph:
-        :return:
-        """
-        if graph is None:
-            graph = self.get_network_graph_from_matrix()
-        degree_view = self.get_degree(graph)
-        correlated_pair_ratio = []
-        [correlated_pair_ratio.append(degree_view[node] / self.num_neurons) for node in graph.nodes()]
-        return correlated_pair_ratio
+# %% Batched analyses
+class CaGraphBatch:
+    """
+    Class for running batched analyses.
 
-    def get_network_coverage(self, graph=None):
-        """
-        Returns the percentage of edges present in the network out of the total possible edges.
+    Only directories can be passed to CaGraphBatch. Node metadata cannot be added to CaGraph objects in the batched
+    analysis. Future versions will include the node_metadata attribute.
+    """
 
-        :param graph:
-        :return:
+    def __init__(self, data_path, group_id=None, threshold=None, threshold_averaged=False):
         """
-        possible_edges = (self.num_neurons * (self.num_neurons - 1)) / 2
-        if graph is None:
-            graph = self.get_network_graph()
-        return len(graph.edges) / possible_edges
+        Path to data must be specified with data_path. A group identifier can optionally be specified with group_id.
+        The threshold can be set in three ways - 1. manually set by the user at the time of object creation,
+        2. if not set manually, all
 
-    def get_eigenvector_centrality(self, graph=None):
+        :param group_id: str
+        :param threshold: float
         """
-        Compute the eigenvector centrality of all network nodes, the
-        measure of influence each node has on the network.
+        if not os.path.exists(os.path.dirname(data_path)):
+            raise ValueError('Path provided for data_path parameter does not exist.')
+        data_list = os.listdir(data_path)
+
+        # Set threshold
+        if threshold is not None:
+            self._threshold = threshold
+        elif threshold_averaged:
+            threshold_keys = []
+            for dataset in data_list:
+                if dataset.endswith(".csv"):
+                    threshold_keys.append(dataset[:-4])
+            self._threshold = self.__generate_averaged_threshold(data_path=data_path, dataset_keys=threshold_keys)
+        else:
+            self._threshold = None
+        if group_id is not None:
+            self._group_id = group_id
+
+        # Construct CaGraph objects for each dataset
+        self._dataset_identifiers = []
+        for dataset in data_list:
+            if dataset.endswith(".csv"):
+                data = np.genfromtxt(data_path + dataset, delimiter=",")
+                try:
+                    setattr(self, f'__{dataset[:-4]}_cagraph', CaGraph(data=data, threshold=self._threshold))
+                    self._dataset_identifiers.append(dataset[:-4])
+                except Exception as e:
+                    print(f"Exception occurred for dataset {dataset[:-4]}: " + repr(e))
+
+    # Private utility methods
+    @property
+    def group_id(self):
+        return self._group_id
+
+    @property
+    def threshold(self):
+        return self._threshold
+
+    @property
+    def dataset_identifiers(self):
+        return self._dataset_identifiers
+
+    def __generate_averaged_threshold(self, data_path, dataset_keys):
+        """
+        Computes an averaged threshold by computing the mean of the recommended thresholds for each individual dataset.
+
+        :param data_path:
+        :param dataset_keys:
+        :return:
+        """
+        store_thresholds = []
+        for dataset in dataset_keys:
+            data = np.genfromtxt(f'{data_path}{dataset}.csv', delimiter=",")
+            store_thresholds.append(prep.generate_threshold(data=data))
+        return np.mean(store_thresholds)
+
+    # Public utility methods
+    def get_cagraph(self, condition_label) -> CaGraph:
+        """
+        Return a CaGraph object for the specified dataset condition_label
+
+        :param condition_label: str
+        :return: CaGraph
+        """
+        return getattr(self, f'__{condition_label}_cagraph')
+
+    def get_full_report(self, save_report=False, save_path=None, save_filename=None, save_filetype=None):
+        """
+        Generates an organized report of all data in the batched sample. It will report on the
+        base analyses included in the CaGraph object get_report() method, and output a single
+        pandas DataFrame or file which includes these analyses for all datasets in a tabular structure.
+
+        :param save_report:
+        :param save_path:
+        :param save_filename:
+        :param save_filetype:
+        :return:
+        """
+        store_reports = {}
+        for key in self.dataset_identifiers:
+            cagraph_obj = self.get_cagraph(key)
+            store_reports[key] = cagraph_obj.get_report()
+
+        # For each column in the individual reports, append to the full report
+        full_report_df = pd.DataFrame()
+        for col in store_reports[key].columns:
+            for key in store_reports.keys():
+                df = store_reports[key]
+                df = df.rename(columns={col: f'{key}_{col}'})
+                full_report_df = pd.concat([full_report_df, df[f'{key}_{col}']], axis=1)
+
+        # Save the report
+        if save_report:
+            if save_filename is None:
+                save_filename = 'report'
+            if save_path is None:
+                save_path = os.getcwd() + '/'
+            if save_filetype is None or save_filetype == 'csv':
+                full_report_df.to_csv(save_path + save_filename + '.csv', index=True)
+            elif save_filetype == 'HDF5':
+                full_report_df.to_hdf(save_path + save_filename + '.h5', key=save_filename, mode='w')
+            elif save_filetype == 'xlsx':
+                full_report_df.to_excel(save_path + save_filename + 'xlsx', index=True)
+        return full_report_df
+
+    def save_individual_dataset_reports(self, save_path=None, save_filetype=None):
+        """
+        Saves individual reports for each of the specified datasets.
+        Individual filenames will be generated using the filename name of the dataset from which the analysis is derived.
+
+        This will result in the same analysis that can be done by creating a CaGraph object using a single dataset.
+
+        :param save_path: str
+        :param save_filetype: str ('csv', 'HDF5', 'xlsx')
+        :return:
+        """
+        # Iterate through all datasets and save report for each
+        for key in self.dataset_identifiers:
+            cagraph_obj = self.get_cagraph(key)
+            cagraph_obj.get_report(save_report=True, save_path=save_path, save_filename=key + '_report',
+                                   save_filetype=save_filetype)
 
-        :param graph:
-        :return:
-        """
-        if graph is None:
-            graph = self.get_network_graph_from_matrix()
-        centrality = nx.eigenvector_centrality(graph)
-        return centrality
 
-    def get_communities(self, graph=None) -> list:
-        """
-        Returns a list of communities, composed of a group of nodes.
 
-        :param graph:
-        :return: node_groups:
-        """
-        if graph is None:
-            graph = self.get_network_graph_from_matrix()
-        communities = nx.algorithms.community.centrality.girvan_newman(graph)
-        node_groups = []
-        for community in next(communities):
-            node_groups.append(list(community))
-        return node_groups
 
-    def draw_network(self, graph=None, position=None, node_size=25, node_color='b', alpha=0.5):
-        """
-        Draws a simple network.
 
-        :param graph:
-        :param position:
-        :param node_size:
-        :param node_color:
-        :param alpha:
-        :return:
-        """
-        if graph is None:
-            graph = self.get_network_graph()
-        if position is None:
-            position = nx.spring_layout(graph)
-        nx.draw(graph, pos=position, node_size=node_size, node_color=node_color, alpha=alpha)
```

## cagraph/preprocess.py

```diff
@@ -1,133 +1,201 @@
 """
 Developer Name: Veronica Porubsky
 Developer ORCID: 0000-0001-7216-3368
 Developer GitHub Username: vporubsky
 Developer Email: verosky@uw.edu
 
-File Creation Date: 
-
-Description: 
+Description: a preprocessing module to process the uploaded calcium imaging datasets before they are used in the
+the CaGraph class to perform graph theory analysis.
 """
 # Imports
-from cagraph.cagraph import CaGraph
 import random
+
+import numpy
 import numpy as np
 import matplotlib.pyplot as plt
 import scipy
+import warnings
+import os
 
-#%% Clean data in preprocessing step
-def remove_quiescent(data, event_data, event_num_threshold=5):
+
+def get_pearsons_correlation_matrix(data):
     """
-    data: numpy.ndarray
-    event_bins: numpy.ndarray
+    Returns the Pearson's correlation for all neuron pairs.
 
-    Removes inactive neurons from the dataset using event_data which the user must pass.
+    :param data: numpy.ndarray
+    :param time_points: tuple
+    :return: numpy.ndarray
     """
-    binarized_event_data = np.where(event_data > 0.0005, 1, 0)
-    new_event_data = np.zeros((1, np.shape(event_data)[1]))
-    new_data = np.zeros((1, np.shape(data)[1]))
-    for row in range(np.shape(binarized_event_data)[0]):
-        if np.sum(binarized_event_data[row, :]) <= event_num_threshold:
-            continue
-        else:
-            new_event_data = np.vstack((new_event_data, event_data[row, :]))
-            new_data = np.vstack((new_data, data[row, :]))
-    return new_data[1:, :], new_event_data[1:, :]
+    return np.nan_to_num(np.corrcoef(data, rowvar=True))
+
+
+# ---------------- Clean data --------------------------------------
+def get_events(data):
+    """
+    Generates event data using smoothed calcium imaging trace.
+
+    :param data: numpy.ndarray
+    :return: numpy.ndarray
+    """
+    event_data = data[0, :]
+    for i in range(1, np.shape(data)[0]):
+        event_row = get_row_event_data(row_data=data[i])
+        event_data = np.vstack((event_data, event_row))
+    return event_data
+
 
-def __count_sign_switch(row_data):
+def get_row_event_data(row_data):
+    """
+
+
+    :param row_data: numpy.ndarray
+    :return: numpy.ndarray
+    """
+    subtract = row_data[0:len(row_data) - 1] - row_data[1:]
+    a = subtract
+    asign = np.sign(a)
+    signchange = ((np.roll(asign, 1) - asign) != 0).astype(int)
+
+    # get indices where sign change occurs in timeseries
+    sign_idx = [i for i, x in enumerate(signchange) if x]
+
+    # remove duplicate spikes
+    sign_idx = np.array(sign_idx)
+    duplicate_finder = sign_idx[1:] - sign_idx[0:len(sign_idx) - 1]
+    duplicates = [i for i, x in enumerate(duplicate_finder) if x == 1]
+    removed_duplicates = list(sign_idx)
+    for index in sorted(duplicates, reverse=True):
+        del removed_duplicates[index]
+
+    # build event row
+    event_row = np.zeros(len(row_data))
+    for index in removed_duplicates:
+        event_row[index] = 1
+    return event_row
+
+
+def _count_sign_switch(row_data):
     """
     Searches time-series data for points at which the time-series changes from increasing to
     decreasing or from decreasing to increasing.
 
+    :param row_data: numpy.ndarray
+    :return: numpy.ndarray
     """
     subtract = row_data[0:len(row_data) - 1] - row_data[1:]
     a = subtract
     asign = np.sign(a)
     signchange = ((np.roll(asign, 1) - asign) != 0).astype(int)
     return np.sum(signchange)
 
+
 def remove_low_activity(data, event_data, event_num_threshold=5):
     """
     Removes neurons with fewer than event_num_threshold events.
-
     Returns a new array of data without neurons that have low activity.
+
+    :param data: numpy.ndarray
+    :param event_data: numpy.ndarray
+    :param event_num_threshold: int
+    :return: numpy.ndarray
     """
     # apply activity treshold
     new_event_data = np.zeros((1, np.shape(event_data)[1]))
     new_data = np.zeros((1, np.shape(data)[1]))
     for row in range(np.shape(data)[0]):
-        if __count_sign_switch(row_data=data[row, :]) <= 5 and not row == 0:
+        if _count_sign_switch(row_data=data[row, :]) <= 5 and not row == 0:
+            continue
+        else:
+            new_event_data = np.vstack((new_event_data, event_data[row, :]))
+            new_data = np.vstack((new_data, data[row, :]))
+    return new_data[1:, :], new_event_data[1:, :]
+
+def remove_quiescent(data, event_data, event_num_threshold=5):
+    """
+    Removes inactive neurons from the dataset using event_data which the user must pass.
+
+    :param data: numpy.ndarray
+    :param event_data: numpy.ndarray
+    :param event_num_threshold: int
+    """
+    binarized_event_data = np.where(event_data > 0.0005, 1, 0)
+    new_event_data = np.zeros((1, np.shape(event_data)[1]))
+    new_data = np.zeros((1, np.shape(data)[1]))
+    for row in range(np.shape(binarized_event_data)[0]):
+        if np.sum(binarized_event_data[row, :]) <= event_num_threshold:
             continue
         else:
             new_event_data = np.vstack((new_event_data, event_data[row, :]))
             new_data = np.vstack((new_data, data[row, :]))
     return new_data[1:, :], new_event_data[1:, :]
 
-#%% Generate suggested threshold value
-def __bins(lst, n):
+
+# %% Suitability for graph theory analysis
+def _bins(data_row, bin_size):
     """
-    Yield successive n-sized chunks from lst.
+    Return successive bin_size-sized chunks from data_row.
+
+    :param data_row: numpy.ndarry or list
+    :param bin_size: int
+    :return: list
     """
-    lst = list(lst)
+    data_row = list(data_row)
     build_binned_list = []
-    for i in range(0, len(lst), n):
-        build_binned_list.append(lst[i:i + n])
+    for i in range(0, len(data_row), bin_size):
+        build_binned_list.append(data_row[i:i + bin_size])
     return build_binned_list
 
 
-def generate_randomized_timeseries_matrix(data: list) -> np.ndarray:
+def generate_noise_shuffle(data: list) -> np.ndarray:
     """
-    data: list
-
-    Parameter data should contain a list of np.ndarray objects.
+    Shuffle every data point randomly within each neuron's calcium fluorescence timeseries.
 
-    Return a numpy array or NWB file.
+    :param data: list
+    :return: numpy.ndarray
     """
     time = data[0, :].copy()
     for row in range(np.shape(data)[0]):
         np.random.shuffle(data[row, :])
-    data[0, :] = time.copy()
+    data[0, :] = time.copy()  # reset time row to original sampling
     return data
 
 
-def generate_randomized_timeseries_binned(data: list, bin_size: int) -> np.ndarray:
+def generate_binned_shuffle(data: list, bin_size: int) -> np.ndarray:
     """
-    data: list
+    Shuffle bin_size-sized bins randomly within each neuron's calcium fluorescence timeseries.
 
-    Parameter data should contain a list of np.ndarray objects.
-
-    Return a numpy array or NWB file.
+    :param data: numpy.ndarray
+    :param bin_size: int
+    :return: numpy.ndarray
     """
     time = data[0, :].copy()
-    build_new_array = np.array(__bins(lst=data[1, :], n=bin_size))
-
+    build_new_array = np.array(_bins(data=data[1, :], bin_size=bin_size))
     # build binned dist
     for row in range(np.shape(data[2:, :])[0]):
-        binned_row = __bins(lst=data[row + 2, :], n=bin_size)
+        binned_row = _bins(data=data[row + 2, :], bin_size=bin_size)
         build_new_array = np.vstack([build_new_array, binned_row])
-
     for row in range(np.shape(build_new_array)[0]):
         np.random.shuffle(build_new_array[row, :])
-
     flatten_array = time.copy()
     for row in range(np.shape(build_new_array)[0]):
         flat_row = [item for sublist in build_new_array[row, :] for item in sublist]
         flatten_array = np.vstack([flatten_array, flat_row])
-
     return flatten_array
 
 
-def __event_bins(data, events):
+def _event_bins(data_row, events):
     """
-    :param data:
-    :param events: single events timecourse
-    :return:
+    Generates a shuffled row of calcium fluorescence data, breaking the timeseries using predetermined events.
+
+    :param data: numpy.ndarray
+    :param events: list
+    :return: list
     """
-    data = list(data)
+    data = list(data_row)
     build_binned_list = []
     event_idx = list(np.nonzero(events)[0])
     if event_idx[-1] != len(data):
         event_idx.append(len(data))
     start_val = 0
     for idx in event_idx:
         build_binned_list.append(data[start_val:idx])
@@ -135,54 +203,51 @@
     np.random.shuffle(build_binned_list)
     flat_random_binned_list = [item for sublist in build_binned_list for item in sublist]
     threshold = 0.01
     flat_random_binned_list = [0 if value < threshold else value for value in flat_random_binned_list]
     return flat_random_binned_list
 
 
-def generate_event_shuffle(data: list, event_data: list) -> np.ndarray:
+def generate_event_shuffle(data: numpy.ndarray, event_data: list) -> np.ndarray:
     """
-    data: list
-
-    Parameter data should contain a list of np.ndarray objects.
+    Generates a shuffled dataset using events to break each neuron's calcium fluorescence timeseries.
 
-    Return a numpy array or NWB file.
+    :param data: numpy.ndarray
+    :param event_data: list
+    :return numpy.ndarray
     """
     time = data[0, :].copy()
-
-    # build binned dist
+    # build event-binned array
     flatten_array = time.copy()
     for row in range(np.shape(data[1:, :])[0]):
-        binned_row = __event_bins(data=data[row + 1, :], events=event_data[row + 1, :])
+        binned_row = _event_bins(data_row=data[row + 1, :], events=event_data[row + 1, :])
         flatten_array = np.vstack([flatten_array, binned_row])
-
     return flatten_array
 
 
-def generate_randomized(data: list, bin_size: int) -> np.ndarray:
+def generate_randomized(data: numpy.ndarray, bin_size: int) -> np.ndarray:
     """
-    data: list
+    Shuffle bin_size-sized bins randomly within each neuron's calcium fluorescence timeseries.
 
-    Parameter data should contain a list of np.ndarray objects.
-
-    Return a numpy array or NWB file.
+    :param data: numpy.ndarray
+    :param bin_size: int
+    :return: numpy.ndarray
     """
     time = data[0, :].copy()
-
     # build binned dist
     flatten_array = time.copy()
     for row in range(np.shape(data[2:, :])[0]):
-        binned_row = __bins(lst=data[row + 2, :], n=bin_size)
+        binned_row = _bins(data_row=data[row + 2, :], bin_size=bin_size)
         flatten_array = np.vstack([flatten_array, binned_row])
-
     return flatten_array
 
 
 def generate_population_event_shuffle(data: np.ndarray, event_data: np.ndarray) -> np.ndarray:
     """
+    Shuffle event bins randomly across all neuron's calcium fluorescence timeseries.
 
     :param data:
     :param event_data:
     :return:
     """
     time = data[0, :].copy()
 
@@ -213,25 +278,27 @@
         end_idx += len(time)
 
     return shuffled_data
 
 
 def plot_shuffle_example(data, shuffled_data=None, event_data=None, show_plot=True):
     """
+    Plot shuffled distribution.
 
-    :param shuffled_data:
-    :param data:
-    :param event_data:
-    :param show_plot:
+    :param data: numpy.ndarray
+    :param shuffled_data: numpy.ndarray
+    :param event_data: list
+    :param show_plot: bool
     :return:
     """
     if shuffled_data is None and event_data is not None:
         shuffled_data = generate_event_shuffle(data=data, event_data=event_data)
     elif shuffled_data is None and event_data is None:
-        raise AttributeError
+        event_data = get_events(data=data)
+        shuffled_data = generate_event_shuffle(data=data, event_data=event_data)
     neuron_idx = random.randint(1, np.shape(data)[0] - 1)
     plt.figure(figsize=(10, 5))
     plt.subplot(211)
     plt.plot(data[0, :], data[neuron_idx, :], c='blue', label='ground truth')
     plt.ylabel('ΔF/F')
     plt.legend()
     plt.subplot(212)
@@ -240,78 +307,199 @@
     plt.ylabel('ΔF/F')
     plt.xlabel('Time')
     plt.legend()
     if show_plot:
         plt.show()
 
 
-def generate_threshold(data, shuffled_data=None, event_data=None):
+def generate_threshold(data, shuffled_data=None, event_data=None, report_threshold=False, report_test=False):
     """
-    Analyzes a shuffled dataset to propose a threshold to use to construct graph objects.
+    Compares provided dataset and a shuffled dataset to propose a threshold to use to construct graph objects.
 
-    :param data:
-    :param shuffled_data:
+    Provides warning if the correlation distribution of the provided dataset is not statistically different from that of
+    the shuffled dataset.
+
+    :param data: numpy.ndarray
+    :param shuffled_data: numpy.ndarray
     :param event_data:
-    :return:
+    :param report_test: bool
+    :return: float or dict
     """
     if shuffled_data is None and event_data is not None:
         shuffled_data = generate_event_shuffle(data=data, event_data=event_data)
     elif shuffled_data is None and event_data is None:
-        raise AttributeError
-    random_cg = CaGraph(shuffled_data)
-    x = random_cg.pearsons_correlation_matrix
+        event_data = get_events(data=data)
+        shuffled_data = generate_event_shuffle(data=data, event_data=event_data)
+    x = get_pearsons_correlation_matrix(data=shuffled_data)
     np.fill_diagonal(x, 0)
     Q1 = np.percentile(x, 25, interpolation='midpoint')
     Q3 = np.percentile(x, 75, interpolation='midpoint')
 
     IQR = Q3 - Q1
-    outlier_threshold = Q3 + 1.5 * IQR
+    outlier_threshold = round(Q3 + 1.5 * IQR, 2)
 
-    ground_truth_cg = CaGraph(data)
-    y = ground_truth_cg.pearsons_correlation_matrix
+    y = get_pearsons_correlation_matrix(data=data)
     np.fill_diagonal(y, 0)
 
     random_vals = np.tril(x).flatten()
     data_vals = np.tril(y).flatten()
-    print(f"KS-statistic: {scipy.stats.ks_2samp(random_vals, data_vals)}")
-    print(f"The threshold is: {outlier_threshold}")
+    ks_statistic = scipy.stats.ks_2samp(random_vals, data_vals)
+    p_val = ks_statistic.pvalue
+    if p_val < 0.05 and report_threshold:
+        print(f"The threshold is: {outlier_threshold:.2f}")
+    else:
+        warnings.warn(
+            'The KS-test performed on the shuffled and ground truth datasets show that the p-value is greater '
+            'than a 5% significance level. Confirm that correlations in dataset are differentiable from random correlations '
+            'before setting a threshold.')
+    if report_test:
+        print(f"KS-statistic: {ks_statistic.statistic}")
+        print(f"P-val: {p_val}")
+        threshold_dict = {"KS-statistic": ks_statistic.statistic}
+        threshold_dict["P-val"] = p_val
+        threshold_dict["threshold"] = outlier_threshold
+        return threshold_dict
     return outlier_threshold
 
-
 def plot_threshold(data, shuffled_data=None, event_data=None, show_plot=True):
     """
+    Plots the correlation distributions of the dataset and the shuffled dataset, along with the identified threshold value.
 
-    :param data:
-    :param shuffled_data:
-    :param event_data:
-    :param show_plot:
+    :param data: numpy.ndarray
+    :param shuffled_data: numpy.ndarray
+    :param event_data: list
+    :param show_plot: bool
     :return:
     """
     if shuffled_data is None and event_data is not None:
         shuffled_data = generate_event_shuffle(data=data, event_data=event_data)
     elif shuffled_data is None and event_data is None:
-        raise AttributeError('Must provide either a pre-processed shuffled dataset or event data to perform the shuffle.')
-    random_cg = CaGraph(shuffled_data)
-    x = random_cg.pearsons_correlation_matrix
+        event_data = get_events(data=data)
+        shuffled_data = generate_event_shuffle(data=data, event_data=event_data)
+
+    x = get_pearsons_correlation_matrix(data=shuffled_data)
     np.fill_diagonal(x, 0)
     Q1 = np.percentile(x, 25, interpolation='midpoint')
     Q3 = np.percentile(x, 75, interpolation='midpoint')
 
     IQR = Q3 - Q1
     outlier_threshold = Q3 + 1.5 * IQR
 
-    ground_truth_cg = CaGraph(data)
-    y = ground_truth_cg.pearsons_correlation_matrix
+    y = get_pearsons_correlation_matrix(data=data)
     np.fill_diagonal(y, 0)
 
-    plt.ylim(0, 100)
-    plt.hist(np.tril(x).flatten(), bins=50, color='grey', alpha=0.3)
-    plt.hist(np.tril(y).flatten(), bins=50, color='blue', alpha=0.3)
+    # specify the bin width
+    bin_width = 0.01
+
+    # calculate the number of bins
+    x_bins = int(np.ceil((x.max() - x.min()) / bin_width))
+    y_bins = int(np.ceil((y.max() - y.min()) / bin_width))
+
+    plt.hist(np.tril(x).flatten(), bins=x_bins, color='grey', alpha=0.3)
+    plt.hist(np.tril(y).flatten(), bins=y_bins, color='blue', alpha=0.3)
     plt.axvline(x=outlier_threshold, color='red')
-    plt.legend(['threshold (Q3 + 1.5*IQR)', 'shuffled', 'ground truth', ])
+    plt.legend(['threshold', 'shuffled', 'ground truth', ])
     plt.xlabel("Pearson's r-value")
     plt.ylabel("Frequency")
     if show_plot:
         plt.show()
 
+def plot_histogram(data, colors, legend=None, title=None, y_label=None, x_label=None, show_plot=True, save_plot=False,
+                   save_path=None, dpi=300, format='png'):
+    """
+    Plot histograms of the provided datasets.
+
+    :param data: list
+    :param colors: list
+    :param legend: list
+    :param title:
+    :param y_label:
+    :param x_label:
+    :param show_plot:
+    :param save_plot:
+    :param save_path:
+    :param dpi:
+    :param format:
+    :return:
+    """
+    # specify the bin width
+    bin_width = 0.01
+
+    for dataset in data:
+        # calculate the number of bins
+        dataset_bins = int(np.ceil((dataset.max() - dataset.min()) / bin_width))
+
+        # plot histogram
+        plt.hist(dataset, bins=dataset_bins, color=colors[0], alpha=0.3)
+
+    if legend is not None:
+        plt.legend(legend)
+    if title is not None:
+        plt.title(title)
+    if y_label is not None:
+        plt.ylabel(y_label)
+    if x_label is not None:
+        plt.xlabel(x_label)
+    else:
+        plt.ylabel("Frequency")
+    if show_plot:
+        plt.show()
+    if save_plot:
+        if save_path is None:
+            save_path = os.getcwd() + f'fig'
+        plt.savefig(fname=save_path, dpi=dpi, format=format)
+
+
+def plot_correlation_hist(data, colors, legend=None, title=None, y_label=None, x_label=None, show_plot=True,
+                          save_plot=False, save_path=None, dpi=300, format='png'):
+    """
+    Plot histograms of the Pearson's correlation coefficient distributions for the provided datasets.
+
+    :param data: list
+    :param colors: list
+    :param legend: list
+    :param title:
+    :param y_label:
+    :param x_label:
+    :param show_plot:
+    :param save_plot:
+    :param save_path:
+    :param dpi:
+    :param format:
+    :return:
+    """
+    x = get_pearsons_correlation_matrix(data=data[0])
+    np.fill_diagonal(x, 0)
+
+    y = get_pearsons_correlation_matrix(data=data[1])
+    np.fill_diagonal(y, 0)
+
+    x = np.tril(x).flatten()
+    y = np.tril(y).flatten()
+
+    # specify the bin width
+    bin_width = 0.01
+
+    # calculate the number of bins
+    x_bins = int(np.ceil((x.max() - x.min()) / bin_width))
+    y_bins = int(np.ceil((y.max() - y.min()) / bin_width))
+
+    # plot histograms
+    plt.hist(x, bins=x_bins, color=colors[0], alpha=0.3)
+    plt.hist(y, bins=y_bins, color=colors[1], alpha=0.3)
+    if legend is not None:
+        plt.legend(legend)
+    if title is not None:
+        plt.title(title)
+    if y_label is not None:
+        plt.ylabel(y_label)
+    if x_label is not None:
+        plt.xlabel(x_label)
+    else:
+        plt.ylabel("Frequency")
+    if show_plot:
+        plt.show()
+    if save_plot:
+        if save_path is None:
+            save_path = os.getcwd() + f'fig'
+        plt.savefig(fname=save_path, dpi=dpi, format=format)
 
-#%% Sensitivity analysis
```

## cagraph/visualization.py

```diff
@@ -1,85 +1,110 @@
 """
 Developer Name: Veronica Porubsky
 Developer ORCID: 0000-0001-7216-3368
 Developer GitHub Username: vporubsky
 Developer Email: verosky@uw.edu
 
-File Creation Date:
-
-Description:
+Description: a visualization module to generate interactive graph visuals and plot graph theory analyses generated using
+the cagraph module.
 """
-# General mports
+# General imports
 import networkx as nx
 import numpy as np
 import matplotlib.pyplot as plt
+plt.style.use('CaGraph.mplstyle')
 import seaborn as sns
 from scipy import stats
 import pandas as pd
 import os
 
 # Bokeh imports
+import bokeh
 from bokeh.io import show, save, output_notebook
 from bokeh.models import Range1d, Circle, MultiLine
 from bokeh.plotting import figure
 from bokeh.plotting import from_networkx
-from bokeh.palettes import Blues8
 from bokeh.transform import linear_cmap
 
-
-
-def interactive_network(ca_graph_obj, graph=None, attributes=['degree', 'HITS', 'hubs', 'CPR', 'communities'],
+def interactive_network(cagraph_obj, graph=None,
+                        attributes=['degree', 'HITS', 'hubs', 'CPR', 'communities', 'clustering'],
+                        additional_attributes = None,
+                        hover_attributes=None,
                         adjust_node_size=5, adjust_size_by='degree', adjust_color_by='communities',
-                        palette=Blues8,
-                        hover_attributes=['degree', 'HITS', 'hubs', 'CPR', 'communities'], title=None,
-                        show_plot=True, show_in_notebook=False, save_plot=False, save_path=None):
+                        palette='Blues8',
+                        position = None, return_position = False,
+                        title=None, show_plot=True, show_in_notebook=False, save_plot=False, save_path=None):
     """
-    Generates an interactived Bokeh.io plot of the graph network.
+    Generates an interactive Bokeh.io plot of the graph network.
 
-    palette: a color palette which can be passed as a tuple: palette = ('grey', 'red', 'blue')
+    :param: cagraph_obj: CaGraph object
+    :param: graph: networkx.Graph object
+    :param: attributes: list
+    :param: additional_attributes: dict
+    :param: hover_attributes: list
+    :param: adjust_node_size: int
+    :param: adjust_size_by: str
+    :param: adjust_color_by: str
+    :param: palette: tuple a color palette which can be passed as a tuple: palette = ('grey', 'red', 'blue')
+    :param: position: dict
+    :param: return_position: bool
+    :param: title: str
+    :param: show_plot: bool
+    :param: show_in_notebook: bool
+    :param: save_plot: bool
+    :param: save_path: str
 
     """
-    # initialize graph information
-    cg = ca_graph_obj
+    # Initialize cagraph and graph
+    cg = cagraph_obj
     if graph is None:
-        G = cg.get_network_graph()
+        G = cg.graph
     else:
         G = graph
-    label_keys = list(map(str, list(cg.labels)))
+    label_keys = cg.node_labels
 
     #  Build attributes dictionary
     attribute_dict = {}
     for attribute in attributes:
+
         if attribute == 'degree':
             # Compute the degree of each node and add attribute
-            attribute_dict['degree'] = dict(nx.degree(G))
+            attribute_dict['degree'] = cg.graph_theory.get_degree(return_type='dict')
+
         elif attribute == 'HITS':
             # Add HITS attribute
-            hub_list, hit_vals = cg.get_hubs(graph=G)
-            attribute_dict['HITS'] = hit_vals
+            attribute_dict['HITS'] = cg.graph_theory.get_hits_values(return_type='dict')
+
         elif attribute == 'hubs':
             # Add hubs attribute
-            attribute_dict['hubs'] = {i: 1 if i in list(set(hub_list) & set(label_keys)) else 0 for i in
-                                      label_keys}
+            attribute_dict['hubs'] = cg.graph_theory.get_hubs(return_type='dict')
+
         elif attribute == 'CPR':
             # Add correlated pairs attribute
-            corr_pair = cg.get_correlated_pair_ratio(graph=G)
-            attribute_dict['CPR'] = {i: j for i, j in zip(label_keys, corr_pair)}
+            attribute_dict['CPR'] = cg.graph_theory.get_correlated_pair_ratio(return_type='dict')
+
         elif attribute == 'communities':
             # Add communities
-            c = list(nx.algorithms.community.greedy_modularity_communities(G))
-            sorted(c)
-            community_id = {}
-            for i in range(len(c)):
-                for j in list(c[i]):
-                    community_id[j] = i
-            attribute_dict['communities'] = community_id
+            attribute_dict['communities'] = cg.graph_theory.get_communities(return_type='dict')
+
+        elif attribute == 'clustering':
+            # Add clustering coefficient
+            attribute_dict['clustering'] = cg.graph_theory.get_clustering_coefficient(return_type='dict')
+
         else:
             raise AttributeError('Invalid attribute key entered.')
 
+    add_hover_attributes = []
+    if additional_attributes is not None:
+        for key in additional_attributes.keys():
+            # parse attribute
+            attribute_dict[key] = {i: j for i, j in zip(label_keys, additional_attributes[key])} # Must be same length
+            # store key value
+            add_hover_attributes += [key]
+
     # Set node attributes
     for key, value in attribute_dict.items():
         nx.set_node_attributes(G, name=key, values=value)
 
     # Adjusted node size
     if adjust_node_size is not None:
         # Adjust node size
@@ -87,29 +112,39 @@
             [(node, value + adjust_node_size) for node, value in attribute_dict[adjust_size_by].items()])
         nx.set_node_attributes(G, name='adjusted_node_size', values=adjusted_node_size)
         size_by_this_attribute = 'adjusted_node_size'
 
     # Adjust node color
     color_by_this_attribute = adjust_color_by
 
-    # Pick a color palette — Blues8, Reds8, Purples8, Oranges8, Viridis8
-    color_palette = palette
+    # Generate color palette
+    palettes = [attr for attr in dir(bokeh.palettes) if
+                not callable(getattr(bokeh.palettes, attr)) and not attr.startswith("__")]
+    if isinstance(palette, str) and palette in palettes:
+        color_palette = getattr(bokeh.palettes, palette)
+    elif isinstance(palette, tuple):
+        color_palette = palette
+    else:
+        raise AttributeError('Must specify color palette as type string using an existing bokeh.palettes palette or generate a tuple containing hex codes.')
 
     # Establish which categories will appear when hovering over each node
+    if hover_attributes is None:
+        hover_attributes = ['degree', 'HITS', 'hubs', 'CPR', 'communities', 'clustering'] + add_hover_attributes
     HOVER_TOOLTIPS = [("Neuron", "@index")]
     for value in hover_attributes:
         HOVER_TOOLTIPS.append((value, "@" + value))
 
     # Create a plot with set dimensions, toolbar, and title
     plot = figure(tooltips=HOVER_TOOLTIPS,
                   tools="pan,wheel_zoom,save,reset", active_scroll='wheel_zoom',
                   x_range=Range1d(-10.1, 10.1), y_range=Range1d(-10.1, 10.1), title=title)
 
     # Create a network graph object
-    position = nx.spring_layout(G)
+    if position is None:
+        position = nx.spring_layout(G)
     network_graph = from_networkx(G, position, scale=10, center=(0, 0))
 
     # Set node sizes and colors according to node degree (color as spectrum of color palette)
     minimum_value_color = min(network_graph.node_renderer.data_source.data[color_by_this_attribute])
     maximum_value_color = max(network_graph.node_renderer.data_source.data[color_by_this_attribute])
     network_graph.node_renderer.glyph = Circle(size=size_by_this_attribute,
                                                fill_color=linear_cmap(color_by_this_attribute, color_palette,
@@ -127,16 +162,18 @@
 
     if save_plot:
         if save_path is not None:
             save(plot, filename=save_path)
         else:
             save(plot, filename=os.path.join(os.getcwd(), f"bokeh_graph_visualization.html"))
 
+    if return_position:
+        return position
 
-def plot_CDF(data=None, color='black', marker='o', x_label='', y_label='CDF', show_plot=False):
+def plot_CDF(data=None, color='black', marker='o', x_label='', y_label='CDF', show_plot=True, save_plot=False, save_path=None, dpi=300, format='png'):
     """
     Plots the cumulative distribution function of the provided list of data.
 
     :param data: list of float values
     :param color: str matplotlib color style
     :param marker: str matplotlib marker style
     :param x_label: str
@@ -154,95 +191,121 @@
     plt.plot(sorted_data, cdf, color=color, marker=marker)
     plt.xlabel(x_label)
     plt.ylabel(y_label)
 
     if show_plot:
         plt.show()
 
+    if save_plot:
+        if save_path is None:
+            save_path = os.getcwd() + f'fig'
+        plt.savefig(fname=save_path, dpi=dpi, format=format)
+
 
-def plot_CDF_compare_two_samples(data_list=None, color_list=['black', 'black'], marker='o', x_label='',
-                                 y_label='CDF', show_plot=False):
+def plot_CDFs(data_list=None, colors=['black', 'black'], marker='o', x_label='',
+                                 y_label='CDF', legend=None, show_plot=True, save_plot=False, save_path=None, dpi=300, format='png'):
     """
     Plots the cumulative distribution function of the provided datasets and prints the associated P-value for assessing
     the Kolmogorov-Smirnov distance between the distributions.
 
     :param data_list: list of lists containing float values to compare with KS-test
-    :param color_list: list of str containing matplotlib color styles
+    :param colors: list of str containing matplotlib color styles
     :param marker: str matplotlib marker style
     :param x_label: str
     :param y_label: str
     :param show_plot: bool
     """
-
     # Evaluate KS-test statistic
     stat_level = stats.ks_2samp(data_list[0], data_list[1])
 
     for idx, data in enumerate(data_list):
         # sort the dataset in ascending order
         sorted_data = np.sort(data)
 
         # get the cdf values of dataset
         cdf = np.arange(len(data)) / float(len(data))
 
         # plotting
-        plt.plot(sorted_data, cdf, color=color_list[idx], marker=marker)
+        plt.plot(sorted_data, cdf, color=colors[idx], marker=marker)
 
+    if legend is not None:
+        plt.legend([legend[0], legend[1]])
     plt.ylabel(y_label)
     plt.xlabel(x_label)
     plt.title(f'P value: {stat_level.pvalue:.2e}')
 
     if show_plot:
         plt.show()
 
+    if save_plot:
+        if save_path is None:
+            save_path = os.getcwd() + f'fig'
+        plt.savefig(fname=save_path, dpi=dpi, format=format)
 
-
-def plot_histograms(data_list=None, color_list=['black', 'black'], x_label='',
-                    y_label='count', bin_size=20, show_plot=True):
+def plot_histograms(data_list=None, colors=['black', 'black'], x_label='',
+                    y_label='count', bin_size=20, show_plot=True, save_plot=False, save_path=None, dpi=300, format='png'):
     """
     Plots histograms of the provided data and prints the associated P-value for assessing
     the Kolmogorov-Smirnov distance between the distributions.
 
     :param data_list: list of lists containing float values to compare with KS-test
-    :param color_list: list of str containing matplotlib color styles
+    :param colors: list of str containing matplotlib color styles
     :param marker: str matplotlib marker style
     :param x_label: str
     :param y_label: str
+    :param bin_size: int
     :param show_plot: bool
+    :param save_plot: bool
+    :param save_path: str
+    :param dpi: int
+    :param format: str
     """
 
     # Evaluate KS-test statistic
     stat_level = stats.ks_2samp(data_list[0], data_list[1])
 
     for idx, data in enumerate(data_list):
         # plotting
-        plt.hist(data, color=color_list[idx], bins=bin_size, alpha=0.4)
+        plt.hist(data, color=colors[idx], bins=bin_size, alpha=0.4)
 
     plt.ylabel(y_label)
     plt.xlabel(x_label)
     plt.title(f'P value: {stat_level.pvalue:.2e}')
 
     if show_plot:
         plt.show()
-
-
-def plot_matched_data(sample_1, sample_2, labels, value_label=None, colors=['grey', 'grey'], show_plot=True):
+    if save_plot:
+        if save_path is None:
+            save_path = os.getcwd() + f'fig'
+        plt.savefig(fname=save_path, dpi=dpi, format=format)
+
+def plot_matched_data(sample_1: list, sample_2: list, labels: list, colors=['grey', 'grey'],
+                      x_label=None, y_label=None, show_plot=True, save_plot=False, save_path=None,
+                      dpi=300, format='png'):
     """
     Plots two samples of matched data. Each sample will be plotted as points stacked vertically within condition.
     Lines will be drawn to connect the matching pairs.
 
+    :param sample_1:
+    :param sample_2:
+    :param colors: list of str containing matplotlib color styles
+    :param x_label: str
+    :param y_label: str
+    :param show_plot: bool
+    :param save_plot: bool
+    :param dpi: int
+    :param format: str containing file extension supported by matplotlib.pyplot.savefig
     """
     # Put into dataframe
     df = pd.DataFrame({labels[0]: sample_1, labels[1]: sample_2})
     data = pd.melt(df)
 
     # Plot
     fig, ax = plt.subplots()
     sns.swarmplot(data=data, x='variable', y='value', ax=ax, size=0)
-
-    # Find idx0 and idx1 by inspecting the elements returned from ax.get_children()
     idx0 = 0
     idx1 = 1
     locs1 = ax.get_children()[idx0].get_offsets()
     locs2 = ax.get_children()[idx1].get_offsets()
 
     y_all = np.zeros(2)
     for i in range(locs1.shape[0]):
@@ -254,13 +317,19 @@
         data = [locs1[:, 1], locs2[:, 1]]
         ax.boxplot(data, positions=[0, 1], capprops=dict(linewidth=0.5, color='k'),
                    whiskerprops=dict(linewidth=0.5, color='k'),
                    boxprops=dict(linewidth=0.5, color='k'),
                    medianprops=dict(color='k'))
         plt.xticks([])
         y_all = np.vstack((y_all, y))
-    if value_label is not None:
-        plt.ylabel(value_label)
-    plt.xlabel(f'P-value = {stats.ttest_rel(sample_1, sample_2).pvalue:.3}')
+
+    if y_label is not None:
+        plt.ylabel(y_label)
+    if x_label is None:
+        plt.xlabel(f'P-value = {stats.ttest_rel(sample_1, sample_2).pvalue:.3}')
 
     if show_plot:
-        plt.show()
+        plt.show()
+    if save_plot:
+        if save_path is None:
+            save_path = os.getcwd() + f'fig'
+        plt.savefig(fname=save_path, dpi=dpi, format=format)
```

### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

## Comparing `cagraph-0.0.1.dist-info/METADATA` & `cagraph-0.0.2.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 Metadata-Version: 2.1
 Name: cagraph
-Version: 0.0.1
+Version: 0.0.2
 Summary: A package to generate graphs from calcium imaging data of neural activity.
-Project-URL: Homepage, https://github.com/vporubsky/CaGraph
 Project-URL: Bug Tracker, https://github.com/vporubsky/CaGraph/issues
+Project-URL: Homepage, https://github.com/vporubsky/CaGraph
 Author-email: Veronica Porubsky <verosky@uw.edu>
-License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Requires-Dist: bokeh<=2.4.3
 Requires-Dist: matplotlib
 Requires-Dist: networkx
 Requires-Dist: numpy
 Requires-Dist: pynwb
 Requires-Dist: scipy
 Requires-Dist: seaborn
-Requires-Dist: statsmodels
 Description-Content-Type: text/markdown
 
 # cagraph
 
 This package is designed to process calcium imaging 
 data recorded from neuronal populations into graphs to
 be analyzed for functional connectivity patterns.
```

## Comparing `cagraph-0.0.1.dist-info/licenses/LICENSE` & `cagraph-0.0.2.dist-info/license_files/LICENSE`

 * *Files identical despite different names*

## Comparing `cagraph-0.0.1.dist-info/RECORD` & `cagraph-0.0.2.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 cagraph/.DS_Store,sha256=miFyUUD0rBMgEbDHTE_cVbqveCIbeiZTgFbnWFSF9Kc,6148
 cagraph/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-cagraph/cagraph.py,sha256=_GFLaacwQ4YjchU3i3k5rN3BdCBndnEPzLt6pCAzoc8,18904
-cagraph/preprocess.py,sha256=KH_z23OxyGLP9G1Uz4yU0SrZXR_wQtr3LLjTUqptEyc,10069
-cagraph/visualization.py,sha256=6UotHvC2hKsHXEq7WOrXoX7lLLC4jPXilNfTou_fcjE,9593
-cagraph-0.0.1.dist-info/METADATA,sha256=1OubruMV5M42H2sQzkHKCwSbpTK6VtEdYO4Pw5VqZS4,906
-cagraph-0.0.1.dist-info/WHEEL,sha256=Fd6mP6ydyRguakwUJ05oBE7fh2IPxgtDN9IwHJ9OqJQ,87
-cagraph-0.0.1.dist-info/licenses/LICENSE,sha256=2bm9uFabQZ3Ykb_SaSU_uUbAj2-htc6WJQmS_65qD00,1073
-cagraph-0.0.1.dist-info/RECORD,,
+cagraph/cagraph.py,sha256=hcKphF5k1VY90Ba6yla6WntXRPdHXBzCr1KruUY7iD4,45484
+cagraph/preprocess.py,sha256=b7BmczNajKIynwEbkAVzcNqyXvqKgL2m5ylnv3CarHc,16835
+cagraph/visualization.py,sha256=FC1Nc80_Je-4T3PrsdPfBmJJDzEWqsDHwawGoCB5HwY,12493
+cagraph-0.0.2.dist-info/METADATA,sha256=PEL5O97ddzvPDJo_XeqJ7oXDlTiOe4iSIssQrdfAkIE,857
+cagraph-0.0.2.dist-info/WHEEL,sha256=sb4ZHsmozXdkdXRvpMHZmhxsxQvL8DERDUEGA9tAfc8,83
+cagraph-0.0.2.dist-info/entry_points.txt,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+cagraph-0.0.2.dist-info/license_files/LICENSE,sha256=2bm9uFabQZ3Ykb_SaSU_uUbAj2-htc6WJQmS_65qD00,1073
+cagraph-0.0.2.dist-info/RECORD,,
```

