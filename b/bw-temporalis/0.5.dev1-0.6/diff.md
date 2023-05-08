# Comparing `tmp/bw_temporalis-0.5.dev1.tar.gz` & `tmp/bw_temporalis-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bw_temporalis-0.5.dev1.tar", last modified: Mon May  1 08:05:06 2023, max compression
+gzip compressed data, was "bw_temporalis-0.6.tar", last modified: Mon May  8 08:49:50 2023, max compression
```

## Comparing `bw_temporalis-0.5.dev1.tar` & `bw_temporalis-0.6.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:05:06.291406 bw_temporalis-0.5.dev1/
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-01 08:04:52.000000 bw_temporalis-0.5.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-01 08:04:52.000000 bw_temporalis-0.5.dev1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-05-01 08:05:06.291406 bw_temporalis-0.5.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-05-01 08:04:52.000000 bw_temporalis-0.5.dev1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:05:06.287406 bw_temporalis-0.5.dev1/bw_temporalis/
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-01 08:04:52.000000 bw_temporalis-0.5.dev1/bw_temporalis/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-01 08:04:52.000000 bw_temporalis-0.5.dev1/bw_temporalis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-05-01 08:04:52.000000 bw_temporalis-0.5.dev1/bw_temporalis/convolution.py
--rw-r--r--   0 runner    (1001) docker     (123)     7980 2023-05-01 08:04:52.000000 bw_temporalis-0.5.dev1/bw_temporalis/lca.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:05:06.287406 bw_temporalis-0.5.dev1/bw_temporalis/lcia/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-01 08:04:52.000000 bw_temporalis-0.5.dev1/bw_temporalis/lcia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-05-01 08:04:52.000000 bw_temporalis-0.5.dev1/bw_temporalis/lcia/climate.py
--rw-r--r--   0 runner    (1001) docker     (123)     6123 2023-05-01 08:04:52.000000 bw_temporalis-0.5.dev1/bw_temporalis/temporal_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     7029 2023-05-01 08:04:52.000000 bw_temporalis-0.5.dev1/bw_temporalis/timeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-05-01 08:04:52.000000 bw_temporalis-0.5.dev1/bw_temporalis/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:05:06.291406 bw_temporalis-0.5.dev1/bw_temporalis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-05-01 08:05:06.000000 bw_temporalis-0.5.dev1/bw_temporalis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-01 08:05:06.000000 bw_temporalis-0.5.dev1/bw_temporalis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 08:05:06.000000 bw_temporalis-0.5.dev1/bw_temporalis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 08:05:06.000000 bw_temporalis-0.5.dev1/bw_temporalis.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-01 08:05:06.000000 bw_temporalis-0.5.dev1/bw_temporalis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-01 08:05:06.000000 bw_temporalis-0.5.dev1/bw_temporalis.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:05:06.287406 bw_temporalis-0.5.dev1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-01 08:04:52.000000 bw_temporalis-0.5.dev1/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:05:06.287406 bw_temporalis-0.5.dev1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-05-01 08:04:52.000000 bw_temporalis-0.5.dev1/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4350 2023-05-01 08:04:52.000000 bw_temporalis-0.5.dev1/examples/ia.py
--rw-r--r--   0 runner    (1001) docker     (123)     6149 2023-05-01 08:04:52.000000 bw_temporalis-0.5.dev1/examples/inv.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-01 08:04:52.000000 bw_temporalis-0.5.dev1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-05-01 08:05:06.291406 bw_temporalis-0.5.dev1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 08:05:06.291406 bw_temporalis-0.5.dev1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     8786 2023-05-01 08:04:52.000000 bw_temporalis-0.5.dev1/tests/test_convolution.py
--rw-r--r--   0 runner    (1001) docker     (123)     8567 2023-05-01 08:04:52.000000 bw_temporalis-0.5.dev1/tests/test_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     4227 2023-05-01 08:04:52.000000 bw_temporalis-0.5.dev1/tests/test_td.py
--rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-05-01 08:04:52.000000 bw_temporalis-0.5.dev1/tests/test_timeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-05-01 08:04:52.000000 bw_temporalis-0.5.dev1/tests/test_utils.py
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-05-08 08:49:50.739924 bw_temporalis-0.6/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1456 2023-04-23 13:14:37.000000 bw_temporalis-0.6/LICENSE
+-rw-r--r--   0 chrismutel   (501) staff       (20)       30 2023-04-23 13:14:37.000000 bw_temporalis-0.6/MANIFEST.in
+-rw-r--r--   0 chrismutel   (501) staff       (20)     3026 2023-05-08 08:49:50.739986 bw_temporalis-0.6/PKG-INFO
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1955 2023-04-23 13:14:37.000000 bw_temporalis-0.6/README.md
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-05-08 08:49:50.737599 bw_temporalis-0.6/bw_temporalis/
+-rw-r--r--   0 chrismutel   (501) staff       (20)        4 2023-05-08 08:40:52.000000 bw_temporalis-0.6/bw_temporalis/VERSION
+-rw-r--r--   0 chrismutel   (501) staff       (20)      608 2023-05-01 16:31:17.000000 bw_temporalis-0.6/bw_temporalis/__init__.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     3287 2023-05-01 16:31:04.000000 bw_temporalis-0.6/bw_temporalis/convolution.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     8241 2023-05-08 08:37:38.000000 bw_temporalis-0.6/bw_temporalis/lca.py
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-05-08 08:49:50.736585 bw_temporalis-0.6/bw_temporalis/lcia/
+-rw-r--r--   0 chrismutel   (501) staff       (20)       60 2023-04-30 15:06:21.000000 bw_temporalis-0.6/bw_temporalis/lcia/__init__.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     4752 2023-04-30 15:06:26.000000 bw_temporalis-0.6/bw_temporalis/lcia/climate.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     8862 2023-05-03 18:06:46.000000 bw_temporalis-0.6/bw_temporalis/temporal_distribution.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     7106 2023-05-07 20:04:42.000000 bw_temporalis-0.6/bw_temporalis/timeline.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     9820 2023-05-07 20:05:01.000000 bw_temporalis-0.6/bw_temporalis/utils.py
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-05-08 08:49:50.738350 bw_temporalis-0.6/bw_temporalis.egg-info/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     3026 2023-05-08 08:49:50.000000 bw_temporalis-0.6/bw_temporalis.egg-info/PKG-INFO
+-rw-r--r--   0 chrismutel   (501) staff       (20)      737 2023-05-08 08:49:50.000000 bw_temporalis-0.6/bw_temporalis.egg-info/SOURCES.txt
+-rw-r--r--   0 chrismutel   (501) staff       (20)        1 2023-05-08 08:49:50.000000 bw_temporalis-0.6/bw_temporalis.egg-info/dependency_links.txt
+-rw-r--r--   0 chrismutel   (501) staff       (20)        1 2023-04-26 11:46:09.000000 bw_temporalis-0.6/bw_temporalis.egg-info/not-zip-safe
+-rw-r--r--   0 chrismutel   (501) staff       (20)      174 2023-05-08 08:49:50.000000 bw_temporalis-0.6/bw_temporalis.egg-info/requires.txt
+-rw-r--r--   0 chrismutel   (501) staff       (20)       37 2023-05-08 08:49:50.000000 bw_temporalis-0.6/bw_temporalis.egg-info/top_level.txt
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-05-08 08:49:50.736822 bw_temporalis-0.6/docs/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1151 2023-04-23 13:14:37.000000 bw_temporalis-0.6/docs/conf.py
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-05-08 08:49:50.737382 bw_temporalis-0.6/examples/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1500 2023-04-26 18:20:47.000000 bw_temporalis-0.6/examples/__init__.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     4350 2023-04-26 18:20:47.000000 bw_temporalis-0.6/examples/ia.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     6149 2023-04-27 11:45:54.000000 bw_temporalis-0.6/examples/inv.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)       87 2023-04-23 13:14:37.000000 bw_temporalis-0.6/pyproject.toml
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1754 2023-05-08 08:49:50.740367 bw_temporalis-0.6/setup.cfg
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-05-08 08:49:50.739566 bw_temporalis-0.6/tests/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     8786 2023-04-30 15:06:08.000000 bw_temporalis-0.6/tests/test_convolution.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     8567 2023-04-27 11:45:54.000000 bw_temporalis-0.6/tests/test_fixtures.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     7855 2023-05-08 08:38:16.000000 bw_temporalis-0.6/tests/test_lca.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     5952 2023-05-08 08:37:38.000000 bw_temporalis-0.6/tests/test_td.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     4301 2023-05-07 20:05:01.000000 bw_temporalis-0.6/tests/test_timeline.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)    13141 2023-05-07 20:05:16.000000 bw_temporalis-0.6/tests/test_utils.py
```

### Comparing `bw_temporalis-0.5.dev1/LICENSE` & `bw_temporalis-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `bw_temporalis-0.5.dev1/PKG-INFO` & `bw_temporalis-0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bw_temporalis
-Version: 0.5.dev1
+Version: 0.6
 Summary: Revision of bw2temporalis for modern Brightway
 Home-page: https://github.com/brightway-lca/bw_temporalis
 Author: Chris Mutel
 Author-email: <cmutel@gmail.com>
 Maintainer: Chris Mutel
 Maintainer-email: <cmutel@gmail.com>
 License: BSD-3-Clause
```

### Comparing `bw_temporalis-0.5.dev1/README.md` & `bw_temporalis-0.6/README.md`

 * *Files identical despite different names*

### Comparing `bw_temporalis-0.5.dev1/bw_temporalis/convolution.py` & `bw_temporalis-0.6/bw_temporalis/convolution.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import numpy as np
 import numpy.typing as npt
 from scipy.sparse import csr_array
 
-
 OFFSET = 31536000000000
 datetime_type = np.dtype("datetime64[s]")
 timedelta_type = np.dtype("timedelta64[s]")
 time_types = {datetime_type, timedelta_type}
 
 
 def consolidate(
```

### Comparing `bw_temporalis-0.5.dev1/bw_temporalis/lca.py` & `bw_temporalis-0.6/bw_temporalis/lca.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from heapq import heappop, heappush
 
 import bw2data as bd
 import numpy as np
 from bw2calc import LCA
 from bw2data.backends import ActivityDataset as AD
 from bw2data.backends import ExchangeDataset as ED
-from bw_graph_tools import GraphTraversal
+from bw_graph_tools import NewNodeEachVisitGraphTraversal
 
 from .temporal_distribution import TemporalDistribution as TD
 from .timeline import Timeline
 
 
 class MultipleTechnosphereExchanges(Exception):
     pass
@@ -57,30 +57,32 @@
         Total number of LCA inventory calculations to perform during graph traversal
     static_activity_indices : set[int]
         Activity `id` values where graph traversal will stop
     skip_coproducts : bool
         Should we also traverse edges for the other products in multioutput activities?
     functional_unit_unique_id : int
         The unique id of the functional unit. Strongly recommended to leave as default.
-    graph_traversal : bw_graph_tools.GraphTraversal
-        Optional subclass of `GraphTraversal` for advanced usage
+    graph_traversal : bw_graph_tools.NewNodeEachVisitGraphTraversal
+        Optional subclass of `NewNodeEachVisitGraphTraversal` for advanced usage
 
     """
 
     def __init__(
         self,
         lca_object: LCA,
         starting_datetime: datetime | str = "now",
-        cutoff: float | None = 5e-3,
-        biosphere_cutoff: float | None = 1e-5,
+        cutoff: float | None = 5e-4,
+        biosphere_cutoff: float | None = 1e-6,
         max_calc: int | None = 2e3,
         static_activity_indices: set[int] | None = set(),
         skip_coproducts: bool | None = False,
         functional_unit_unique_id: int | None = -1,
-        graph_traversal: GraphTraversal | None = GraphTraversal,
+        graph_traversal: (
+            NewNodeEachVisitGraphTraversal | None
+        ) = NewNodeEachVisitGraphTraversal,
     ):
         self.lca_object = lca_object
         self.unique_id = functional_unit_unique_id
         self.t0 = TD(
             np.array([np.datetime64(starting_datetime)]),
             np.array([1]),
         )
@@ -102,31 +104,30 @@
             biosphere_cutoff=biosphere_cutoff,
             separate_biosphere_flows=True,
             skip_coproducts=skip_coproducts,
             functional_unit_unique_id=functional_unit_unique_id,
         )
         print("Calculation count:", gt["calculation_count"])
         self.nodes = gt["nodes"]
-
         self.edges = gt["edges"]
         self.edge_mapping = defaultdict(list)
         for edge in self.edges:
-            self.edge_mapping[edge.consumer_id].append(edge)
+            self.edge_mapping[edge.consumer_unique_id].append(edge)
 
         self.flows = gt["flows"]
         self.flow_mapping = defaultdict(list)
         for flow in self.flows:
             self.flow_mapping[flow.activity_unique_id].append(flow)
 
     def build_timeline(self) -> Timeline:
         heap = []
         timeline = Timeline()
 
         for edge in self.edge_mapping[self.unique_id]:
-            node = self.nodes[edge.producer_id]
+            node = self.nodes[edge.producer_unique_id]
             heappush(
                 heap,
                 (
                     1 / node.cumulative_score,
                     self.t0 * edge.amount,
                     node,
                 ),
@@ -134,44 +135,50 @@
 
         while heap:
             _, td, node = heappop(heap)
             for flow in self.flow_mapping.get(node.unique_id, []):
                 for exchange in self.get_biosphere_exchanges(
                     flow.flow_datapackage_id, node.activity_datapackage_id
                 ):
-                    value = (
-                        exchange.data.get("temporal_distribution")
-                        or exchange.data["amount"]
-                    )
+                    value = self._exchange_value(exchange)
                     timeline.add_flow_temporal_distribution(
-                        td=td * value,
+                        td=(td * value).simplify(),
                         flow=flow.flow_datapackage_id,
                         activity=node.activity_datapackage_id,
                     )
 
             for edge in self.edge_mapping[node.unique_id]:
                 exchange = self.get_technosphere_exchange(
-                    input_id=self.nodes[edge.producer_id].activity_datapackage_id,
+                    input_id=self.nodes[
+                        edge.producer_unique_id
+                    ].activity_datapackage_id,
                     output_id=node.activity_datapackage_id,
                 )
                 value = (
-                    exchange.data.get("temporal_distribution")
-                    or exchange.data["amount"]
-                ) / node.reference_product_production_amount
-                producer = self.nodes[edge.producer_id]
+                    self._exchange_value(exchange)
+                    / node.reference_product_production_amount
+                )
+                producer = self.nodes[edge.producer_unique_id]
                 heappush(
                     heap,
                     (
                         1 / node.cumulative_score,
-                        td * value,
+                        (td * value).simplify(),
                         producer,
                     ),
                 )
         return timeline
 
+    def _exchange_value(self, exchange):
+        td = exchange.data.get("temporal_distribution")
+        if td is None:
+            return exchange.data["amount"]
+        else:
+            return td * exchange.data["amount"]
+
     def _exchange_iterator(self, input_id: int, output_id: int) -> list[ED]:
         inp = AD.get(AD.id == input_id)
         outp = AD.get(AD.id == output_id)
         return list(
             ED.select().where(
                 ED.input_code == inp.code,
                 ED.input_database == inp.database,
@@ -182,23 +189,25 @@
 
     def get_biosphere_exchanges(self, flow_id: int, activity_id: int) -> Iterable[ED]:
         exchanges = self._exchange_iterator(flow_id, activity_id)
         if len(exchanges) > 1:
             total = sum(exc.data["amount"] for exc in exchanges)
             for exc in exchanges:
                 exc.data["amount"] /= total
-                if "temporal_distribution" in exc.data:
-                    exc.data["temporal_distribution"] /= total
                 yield exc
         else:
             yield from exchanges
 
     def get_technosphere_exchange(self, input_id: int, output_id: int) -> ED:
+        def printer(x):
+            return "{}|{}|{}".format(x.database, x.name, x.code)
+
         exchanges = self._exchange_iterator(input_id, output_id)
         if len(exchanges) > 1:
-            _ = lambda x: "{}|{}|{}".format(x.database, x.name, x.code)
             raise MultipleTechnosphereExchanges(
                 "Found {} exchanges for link between {} and {}".format(
-                    len(exchanges), _(inp), _(outp)
+                    len(exchanges),
+                    printer(exchanges[0].input),
+                    printer(exchanges[0].output),
                 )
             )
         return exchanges[0]
```

### Comparing `bw_temporalis-0.5.dev1/bw_temporalis/lcia/climate.py` & `bw_temporalis-0.6/bw_temporalis/lcia/climate.py`

 * *Files identical despite different names*

### Comparing `bw_temporalis-0.5.dev1/bw_temporalis/timeline.py` & `bw_temporalis-0.6/bw_temporalis/timeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,14 +66,17 @@
         --------
         bw_temporalis.temporal_distribution.TemporalDistribution: A container for a series of values spread over time.
         """
         self.data.append(
             FlowTD(distribution=td.nonzero(), flow=flow, activity=activity)
         )
 
+    def __len__(self):
+        return len(self.date)
+
     def build_dataframe(self) -> None:
         """
         Build a Pandas DataFrame from the Timeline.data object and store it as a Timeline.pd object.
 
         Returns
         -------
         None, creates class attribute Pandas DataFrame `df` with the following columns:
@@ -110,14 +113,15 @@
                 "amount": pd.Series(data=amount, dtype="float64"),
                 "flow": pd.Series(data=flow, dtype="int"),
                 "activity": pd.Series(data=activity, dtype="int"),
             }
         )
         self.df.sort_values(by="date", ascending=True, inplace=True)
         self.df.reset_index(drop=True, inplace=True)
+        return self.df
 
     def characterize_dataframe(
         self,
         characterization_function: Callable,
         flow: set[int] | None = None,
         activity: set[int] | None = None,
         cumsum: bool | None = True,
```

### Comparing `bw_temporalis-0.5.dev1/bw_temporalis.egg-info/PKG-INFO` & `bw_temporalis-0.6/bw_temporalis.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bw-temporalis
-Version: 0.5.dev1
+Version: 0.6
 Summary: Revision of bw2temporalis for modern Brightway
 Home-page: https://github.com/brightway-lca/bw_temporalis
 Author: Chris Mutel
 Author-email: <cmutel@gmail.com>
 Maintainer: Chris Mutel
 Maintainer-email: <cmutel@gmail.com>
 License: BSD-3-Clause
```

### Comparing `bw_temporalis-0.5.dev1/bw_temporalis.egg-info/SOURCES.txt` & `bw_temporalis-0.6/bw_temporalis.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -20,10 +20,11 @@
 bw_temporalis.egg-info/SOURCES.txt
 bw_temporalis.egg-info/dependency_links.txt
 bw_temporalis.egg-info/not-zip-safe
 bw_temporalis.egg-info/requires.txt
 bw_temporalis.egg-info/top_level.txt
 tests/test_convolution.py
 tests/test_fixtures.py
+tests/test_lca.py
 tests/test_td.py
 tests/test_timeline.py
 tests/test_utils.py
```

### Comparing `bw_temporalis-0.5.dev1/docs/conf.py` & `bw_temporalis-0.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bw_temporalis-0.5.dev1/examples/__init__.py` & `bw_temporalis-0.6/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `bw_temporalis-0.5.dev1/examples/ia.py` & `bw_temporalis-0.6/examples/ia.py`

 * *Files identical despite different names*

### Comparing `bw_temporalis-0.5.dev1/examples/inv.py` & `bw_temporalis-0.6/examples/inv.py`

 * *Files identical despite different names*

### Comparing `bw_temporalis-0.5.dev1/setup.cfg` & `bw_temporalis-0.6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 python_requires = >=3.8
 install_requires = 
 	bw2calc >=2.0.dev12
 	bw2data >=4.0.dev18
 	bw_graph_tools
 	numpy
 	pandas
+	scipy
 	tqdm
 
 [options.packages.find]
 where = .
 exclude = 
 	tests
```

### Comparing `bw_temporalis-0.5.dev1/tests/test_convolution.py` & `bw_temporalis-0.6/tests/test_convolution.py`

 * *Files identical despite different names*

### Comparing `bw_temporalis-0.5.dev1/tests/test_fixtures.py` & `bw_temporalis-0.6/tests/test_fixtures.py`

 * *Files identical despite different names*

### Comparing `bw_temporalis-0.5.dev1/tests/test_timeline.py` & `bw_temporalis-0.6/tests/test_timeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import numpy as np
 import pandas as pd
 import pytest
 
 from bw_temporalis.temporal_distribution import TemporalDistribution
-from bw_temporalis.timeline import EmptyTimeline, FlowTD, Timeline
+from bw_temporalis.timeline import EmptyTimeline, Timeline
 
 
 def test_empty_timeline_build_dataframe_missing():
     tl = Timeline()
     with pytest.raises(EmptyTimeline):
         tl.build_dataframe()
```

