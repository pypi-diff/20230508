# Comparing `tmp/semsim-0.0.0.tar.gz` & `tmp/semsim-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semsim-0.0.0.tar", last modified: Thu May  4 08:46:46 2023, max compression
+gzip compressed data, was "semsim-1.1.0.tar", last modified: Mon May  8 18:46:01 2023, max compression
```

## Comparing `semsim-0.0.0.tar` & `semsim-1.1.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 mathematician  (1000) mathematician  (1000)        0 2023-05-04 08:46:46.483886 semsim-0.0.0/
--rw-r--r--   0 mathematician  (1000) mathematician  (1000)     1518 2023-05-03 16:49:49.000000 semsim-0.0.0/LICENSE
--rw-r--r--   0 mathematician  (1000) mathematician  (1000)       23 2023-05-03 17:18:32.000000 semsim-0.0.0/MANIFEST.in
--rw-r--r--   0 mathematician  (1000) mathematician  (1000)      703 2023-05-04 08:46:46.483886 semsim-0.0.0/PKG-INFO
--rw-r--r--   0 mathematician  (1000) mathematician  (1000)        0 2023-05-04 08:35:45.000000 semsim-0.0.0/README.md
--rw-r--r--   0 mathematician  (1000) mathematician  (1000)        0 2023-05-04 08:15:32.000000 semsim-0.0.0/pypi_readme.md
--rw-r--r--   0 mathematician  (1000) mathematician  (1000)       98 2023-05-04 08:14:24.000000 semsim-0.0.0/pyproject.toml
-drwxr-xr-x   0 mathematician  (1000) mathematician  (1000)        0 2023-05-04 08:46:46.278907 semsim-0.0.0/semsim/
--rw-r--r--   0 mathematician  (1000) mathematician  (1000)     1212 2023-05-03 17:31:10.000000 semsim-0.0.0/semsim/__init__.py
-drwxr-xr-x   0 mathematician  (1000) mathematician  (1000)        0 2023-05-04 08:46:46.449311 semsim-0.0.0/semsim/algo/
--rw-r--r--   0 mathematician  (1000) mathematician  (1000)     1233 2023-05-03 17:31:10.000000 semsim-0.0.0/semsim/algo/__init__.py
--rw-r--r--   0 mathematician  (1000) mathematician  (1000)    16136 2023-05-03 17:31:10.000000 semsim-0.0.0/semsim/algo/default.py
--rw-r--r--   0 mathematician  (1000) mathematician  (1000)     4721 2023-05-03 17:31:10.000000 semsim-0.0.0/semsim/algo/engine.py
--rw-r--r--   0 mathematician  (1000) mathematician  (1000)     1761 2023-05-03 17:31:10.000000 semsim-0.0.0/semsim/algo/filter.py
--rw-r--r--   0 mathematician  (1000) mathematician  (1000)     3739 2023-05-03 17:31:10.000000 semsim-0.0.0/semsim/algo/heuristic.py
--rw-r--r--   0 mathematician  (1000) mathematician  (1000)    25092 2023-05-03 17:31:10.000000 semsim-0.0.0/semsim/algo/kernel.py
--rw-r--r--   0 mathematician  (1000) mathematician  (1000)     9969 2023-05-03 17:31:10.000000 semsim-0.0.0/semsim/algo/neural.py
--rw-r--r--   0 mathematician  (1000) mathematician  (1000)     3913 2023-05-03 17:31:10.000000 semsim-0.0.0/semsim/algo/parser.py
--rw-r--r--   0 mathematician  (1000) mathematician  (1000)     6306 2023-05-03 17:31:10.000000 semsim-0.0.0/semsim/algo/representation.py
--rw-r--r--   0 mathematician  (1000) mathematician  (1000)     4895 2023-05-03 17:31:10.000000 semsim-0.0.0/semsim/algo/tag.py
--rw-r--r--   0 mathematician  (1000) mathematician  (1000)    11441 2023-05-03 17:31:10.000000 semsim-0.0.0/semsim/algo/tree.py
--rw-r--r--   0 mathematician  (1000) mathematician  (1000)     3767 2023-05-03 17:31:10.000000 semsim-0.0.0/semsim/download.py
--rw-r--r--   0 mathematician  (1000) mathematician  (1000)      687 2023-05-03 17:31:10.000000 semsim-0.0.0/semsim/exception.py
-drwxr-xr-x   0 mathematician  (1000) mathematician  (1000)        0 2023-05-04 08:46:46.468900 semsim-0.0.0/semsim/interface/
--rw-r--r--   0 mathematician  (1000) mathematician  (1000)      105 2023-05-03 17:31:10.000000 semsim-0.0.0/semsim/interface/__init__.py
--rw-r--r--   0 mathematician  (1000) mathematician  (1000)    11156 2023-05-03 17:31:10.000000 semsim-0.0.0/semsim/interface/cli.py
--rw-r--r--   0 mathematician  (1000) mathematician  (1000)     1873 2023-05-03 17:31:10.000000 semsim-0.0.0/semsim/logger.py
-drwxr-xr-x   0 mathematician  (1000) mathematician  (1000)        0 2023-05-04 08:46:46.329201 semsim-0.0.0/semsim.egg-info/
--rw-r--r--   0 mathematician  (1000) mathematician  (1000)      703 2023-05-04 08:46:46.000000 semsim-0.0.0/semsim.egg-info/PKG-INFO
--rw-r--r--   0 mathematician  (1000) mathematician  (1000)      639 2023-05-04 08:46:46.000000 semsim-0.0.0/semsim.egg-info/SOURCES.txt
--rw-r--r--   0 mathematician  (1000) mathematician  (1000)        1 2023-05-04 08:46:46.000000 semsim-0.0.0/semsim.egg-info/dependency_links.txt
--rw-r--r--   0 mathematician  (1000) mathematician  (1000)       52 2023-05-04 08:46:46.000000 semsim-0.0.0/semsim.egg-info/entry_points.txt
--rw-r--r--   0 mathematician  (1000) mathematician  (1000)      163 2023-05-04 08:46:46.000000 semsim-0.0.0/semsim.egg-info/requires.txt
--rw-r--r--   0 mathematician  (1000) mathematician  (1000)        7 2023-05-04 08:46:46.000000 semsim-0.0.0/semsim.egg-info/top_level.txt
--rw-r--r--   0 mathematician  (1000) mathematician  (1000)     1590 2023-05-04 08:46:46.488915 semsim-0.0.0/setup.cfg
--rw-r--r--   0 mathematician  (1000) mathematician  (1000)       38 2023-03-06 10:25:28.000000 semsim-0.0.0/setup.py
+drwxr-xr-x   0 mathematician  (1000) mathematician  (1000)        0 2023-05-08 18:46:01.736634 semsim-1.1.0/
+-rw-r--r--   0 mathematician  (1000) mathematician  (1000)     1518 2023-05-03 16:49:49.000000 semsim-1.1.0/LICENSE
+-rw-r--r--   0 mathematician  (1000) mathematician  (1000)       23 2023-05-03 17:18:32.000000 semsim-1.1.0/MANIFEST.in
+-rw-r--r--   0 mathematician  (1000) mathematician  (1000)     2838 2023-05-08 18:46:01.736634 semsim-1.1.0/PKG-INFO
+-rw-r--r--   0 mathematician  (1000) mathematician  (1000)     2134 2023-05-04 16:12:09.000000 semsim-1.1.0/README.md
+-rw-r--r--   0 mathematician  (1000) mathematician  (1000)     2134 2023-05-04 16:12:14.000000 semsim-1.1.0/pypi_readme.md
+-rw-r--r--   0 mathematician  (1000) mathematician  (1000)       98 2023-05-04 08:14:24.000000 semsim-1.1.0/pyproject.toml
+drwxr-xr-x   0 mathematician  (1000) mathematician  (1000)        0 2023-05-08 18:46:01.531517 semsim-1.1.0/semsim/
+-rw-r--r--   0 mathematician  (1000) mathematician  (1000)     1212 2023-05-03 17:31:10.000000 semsim-1.1.0/semsim/__init__.py
+drwxr-xr-x   0 mathematician  (1000) mathematician  (1000)        0 2023-05-08 18:46:01.701511 semsim-1.1.0/semsim/algo/
+-rw-r--r--   0 mathematician  (1000) mathematician  (1000)     1233 2023-05-03 17:31:10.000000 semsim-1.1.0/semsim/algo/__init__.py
+-rw-r--r--   0 mathematician  (1000) mathematician  (1000)    16136 2023-05-08 16:32:01.000000 semsim-1.1.0/semsim/algo/default.py
+-rw-r--r--   0 mathematician  (1000) mathematician  (1000)     4697 2023-05-08 16:42:55.000000 semsim-1.1.0/semsim/algo/engine.py
+-rw-r--r--   0 mathematician  (1000) mathematician  (1000)     1761 2023-05-03 17:31:10.000000 semsim-1.1.0/semsim/algo/filter.py
+-rw-r--r--   0 mathematician  (1000) mathematician  (1000)     3739 2023-05-03 17:31:10.000000 semsim-1.1.0/semsim/algo/heuristic.py
+-rw-r--r--   0 mathematician  (1000) mathematician  (1000)    25182 2023-05-08 16:20:36.000000 semsim-1.1.0/semsim/algo/kernel.py
+-rw-r--r--   0 mathematician  (1000) mathematician  (1000)    10557 2023-05-08 16:22:29.000000 semsim-1.1.0/semsim/algo/neural.py
+-rw-r--r--   0 mathematician  (1000) mathematician  (1000)     3913 2023-05-03 17:31:10.000000 semsim-1.1.0/semsim/algo/parser.py
+-rw-r--r--   0 mathematician  (1000) mathematician  (1000)     6306 2023-05-03 17:31:10.000000 semsim-1.1.0/semsim/algo/representation.py
+-rw-r--r--   0 mathematician  (1000) mathematician  (1000)     4895 2023-05-03 17:31:10.000000 semsim-1.1.0/semsim/algo/tag.py
+-rw-r--r--   0 mathematician  (1000) mathematician  (1000)    11441 2023-05-03 17:31:10.000000 semsim-1.1.0/semsim/algo/tree.py
+-rw-r--r--   0 mathematician  (1000) mathematician  (1000)     3958 2023-05-08 16:16:57.000000 semsim-1.1.0/semsim/download.py
+-rw-r--r--   0 mathematician  (1000) mathematician  (1000)      687 2023-05-03 17:31:10.000000 semsim-1.1.0/semsim/exception.py
+drwxr-xr-x   0 mathematician  (1000) mathematician  (1000)        0 2023-05-08 18:46:01.721794 semsim-1.1.0/semsim/interface/
+-rw-r--r--   0 mathematician  (1000) mathematician  (1000)      105 2023-05-03 17:31:10.000000 semsim-1.1.0/semsim/interface/__init__.py
+-rw-r--r--   0 mathematician  (1000) mathematician  (1000)    11156 2023-05-03 17:31:10.000000 semsim-1.1.0/semsim/interface/cli.py
+-rw-r--r--   0 mathematician  (1000) mathematician  (1000)     1873 2023-05-03 17:31:10.000000 semsim-1.1.0/semsim/logger.py
+drwxr-xr-x   0 mathematician  (1000) mathematician  (1000)        0 2023-05-08 18:46:01.581477 semsim-1.1.0/semsim.egg-info/
+-rw-r--r--   0 mathematician  (1000) mathematician  (1000)     2838 2023-05-08 18:46:01.000000 semsim-1.1.0/semsim.egg-info/PKG-INFO
+-rw-r--r--   0 mathematician  (1000) mathematician  (1000)      639 2023-05-08 18:46:01.000000 semsim-1.1.0/semsim.egg-info/SOURCES.txt
+-rw-r--r--   0 mathematician  (1000) mathematician  (1000)        1 2023-05-08 18:46:01.000000 semsim-1.1.0/semsim.egg-info/dependency_links.txt
+-rw-r--r--   0 mathematician  (1000) mathematician  (1000)       52 2023-05-08 18:46:01.000000 semsim-1.1.0/semsim.egg-info/entry_points.txt
+-rw-r--r--   0 mathematician  (1000) mathematician  (1000)      163 2023-05-08 18:46:01.000000 semsim-1.1.0/semsim.egg-info/requires.txt
+-rw-r--r--   0 mathematician  (1000) mathematician  (1000)        7 2023-05-08 18:46:01.000000 semsim-1.1.0/semsim.egg-info/top_level.txt
+-rwxrwxrwx   0 mathematician  (1000) mathematician  (1000)     1590 2023-05-08 18:46:01.741680 semsim-1.1.0/setup.cfg
+-rw-r--r--   0 mathematician  (1000) mathematician  (1000)       38 2023-03-06 10:25:28.000000 semsim-1.1.0/setup.py
```

### Comparing `semsim-0.0.0/LICENSE` & `semsim-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `semsim-0.0.0/semsim/__init__.py` & `semsim-1.1.0/semsim/__init__.py`

 * *Files identical despite different names*

### Comparing `semsim-0.0.0/semsim/algo/__init__.py` & `semsim-1.1.0/semsim/algo/__init__.py`

 * *Files identical despite different names*

### Comparing `semsim-0.0.0/semsim/algo/default.py` & `semsim-1.1.0/semsim/algo/default.py`

 * *Files identical despite different names*

### Comparing `semsim-0.0.0/semsim/algo/engine.py` & `semsim-1.1.0/semsim/algo/engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing import Any
 
 import attr
 from attr import validators
 from tqdm import tqdm
 
 from .heuristic import BaseOrderHeuristic, PairwiseOrderHeuristic
-from .kernel import BaseKernel, AssignmentKernel
+from .kernel import BaseKernel, TABK
 from ..logger import LoggerMixin, get_logger
 from .representation import TextEngine, TextRepr
 from .tree import Tree
 
 
 __all__ = (
     'SemSimEngine',
@@ -33,15 +33,15 @@
 
 
 @attr.s(slots=True, kw_only=True, init=False)
 class SemSimEngine(LoggerMixin):
     '''Main class for comparing texts.'''
 
     engine: TextEngine = attr.ib()
-    kernel: BaseKernel = attr.ib(factory=AssignmentKernel)
+    kernel: BaseKernel = attr.ib(factory=TABK)
     heuristic: BaseOrderHeuristic = attr.ib()
 
     max_out_pairs: int = attr.ib(default=100, validator=validators.gt(0))
     max_process_pairs: int = attr.ib(default=10_000, validator=validators.gt(0))
 
     def __init__(self, *, verbose: bool = True, **kwargs: Any):
         '''
```

### Comparing `semsim-0.0.0/semsim/algo/filter.py` & `semsim-1.1.0/semsim/algo/filter.py`

 * *Files identical despite different names*

### Comparing `semsim-0.0.0/semsim/algo/heuristic.py` & `semsim-1.1.0/semsim/algo/heuristic.py`

 * *Files identical despite different names*

### Comparing `semsim-0.0.0/semsim/algo/kernel.py` & `semsim-1.1.0/semsim/algo/kernel.py`

 * *Files 3% similar despite different names*

```diff
@@ -233,15 +233,15 @@
 
 @attr.s(slots=True, kw_only=True, init=False)
 class AdditiveKernel(BigramKernel, ABC):  # type: ignore[override]
     '''Base class for additive bigram kernels.'''
 
     gamma: float = attr.ib(validator=validators.and_(validators.gt(0), validators.le(1)))
 
-    def __init__(self, gamma: float = 0.5, **kwargs: Any):
+    def __init__(self, gamma: float = 0.15, **kwargs: Any):
         r'''
         Additive kernel initialization.
 
         :param gamma: $\gamma$ value for post-calibrating similarity scores
         '''
 
         if not 0 < gamma <= 1:
@@ -262,16 +262,18 @@
             return 0
         if lhs == rhs:
             return 1
 
         self._precompute(lhs, rhs)
         sim = 0.
         for dep_left in lhs:
+            if dep_left.parent is None:
+                continue
             for dep_right in rhs:
-                if (dep_left.parent is not None and dep_right.parent is not None):
+                if dep_right.parent is not None:
                     sim += self._sim(dep_left, dep_right)
         denom = self._denominator(lhs, rhs)
         result = sim / denom if denom else 0
         return result ** self.gamma
 
     def _precompute(self, lhs: Tree, rhs: Tree) -> None:
         pass
@@ -327,28 +329,31 @@
     _rhs_tf: dict[str, int] = attr.ib(factory=dict, init=False, repr=False)
 
     def __init__(
         self,
         *,
         idf: dict[str, float] | None = None,
         use_lemma: bool = True,
-        unknown_idf: float = 1,
+        unknown_idf: float | None = None,
         **kwargs: Any,
     ):
         '''
         TF-IDF based approximate bigram kernel initialization.
 
         :param idf: IDF dictionary
         :param use_lemma: whether to use lemmas instead of tokens for lookups in IDF dictionary
         :param unknown_idf: default IDF values for unknown dictionary entries
         '''
 
         AdditiveKernel.__init__(self, **kwargs)
+
         self.idf = idf or {}
         self.use_lemma = use_lemma
+        if unknown_idf is None:
+            unknown_idf = 1 + np.log(len(idf)) if idf is not None else 1
         self.unknown_idf = unknown_idf
 
     def _precompute(self, lhs: Tree, rhs: Tree) -> None:
         self._lhs_tf = self._compute_tf(lhs)
         self._rhs_tf = self._compute_tf(rhs)
 
     def _compute_tf(self, tree: Tree) -> dict[str, int]:
@@ -384,15 +389,15 @@
 
         return s, s_hat
 
 
 def resolve_alpha_nu(alpha: float | None, nu: float | None) -> tuple[float, float]:
     if alpha is None:
         if nu is None:
-            alpha = 0.9
+            alpha = 0.25
             nu = 1 - alpha
         elif 0 <= nu < 1:
             alpha = 1 - nu
         else:
             raise ArgumentError('Parameter "nu" should be in range [0; 1).')
     elif nu is not None:
         raise ArgumentError(
@@ -434,15 +439,18 @@
 
     def _precompute(self, lhs: Tree, rhs: Tree) -> None:
         self._dp = [
             [None] * rhs.size for _ in range(lhs.size)
         ]
 
     def _sim(self, lhs: Node, rhs: Node) -> float:
-        return self._subtree_sim(lhs.parent, rhs.parent)  # type: ignore
+        sim = self._node_sim(lhs.parent, rhs.parent)  # type: ignore
+        sim *= self._deprel_sim(lhs.deprel, rhs.deprel)
+        sim *= self._subtree_sim(lhs, rhs)
+        return sim
 
     def _subtree_sim(self, lhs: Node, rhs: Node) -> float:
         lhs_idx = lhs.idx - 1
         rhs_idx = rhs.idx - 1
         sim = self._dp[lhs_idx][rhs_idx]
         if sim is not None:
             return sim
@@ -460,15 +468,15 @@
         self._dp[lhs_idx][rhs_idx] = sim
         return sim
 
 
 def resolve_beta_delta(beta: float | None, delta: float | None) -> tuple[float, float]:
     if beta is None:
         if delta is None:
-            beta = 0.1
+            beta = 0.6
             delta = 1 - beta
         elif 0 <= delta < 1:
             beta = 1 - delta
         else:
             raise ArgumentError('Parameter "delta" should be in range [0; 1].')
     elif delta is not None:
         raise ArgumentError(
@@ -490,19 +498,19 @@
     delta: float = attr.ib(validator=validators.and_(validators.ge(0), validators.le(1)))
     tabk: TABK = attr.ib()
     msk: MSK = attr.ib()
 
     def __init__(
         self,
         *,
-        gamma: float = 0.5,
+        gamma: float = 0.15,
 
         idf: dict[str, float] | None = None,
         use_lemma: bool = True,
-        unknown_idf: float = 1,
+        unknown_idf: float | None = None,
 
         alpha: float | None = None,
         nu: float | None = None,
 
         beta: float | None = None,
         delta: float | None = None,
         **kwargs: Any,
@@ -609,15 +617,15 @@
         for left in top_nodes:
             right = matches.get(left)
             if right is not None:
                 score += -2 * graph[left][right]['weight']
         return score
 
 
-DEFAULT_BATCH_SIZE = 32
+DEFAULT_BATCH_SIZE = 64
 
 
 @attr.s(slots=True, kw_only=True, init=False)
 class NeuralKernel(BaseKernel):
     '''Neural kernel based on graph neural networks.'''
 
     model: nn.Module = attr.ib()
@@ -632,53 +640,49 @@
         self,
         *,
         model: nn.Module | None = None,
         model_path: str | Path | None = None,
         model_type: str | None = None,
         device: torch.device | str = 'cpu',
         batch_size: int = DEFAULT_BATCH_SIZE,
+        **kwargs: Any,
     ):
         '''
         Neural kernel initialization.
 
         :param model: graph neural network model (torch_geometric)
         :param model_path: path to GNN model checkpoint
-        :param model_type: type of GNN to instantiate (GCN or GAT)
+        :param model_type: type of GNN to instantiate ('gcn' or 'gat')
         :param device: device to run GNN on ('cpu', 'gpu'/'cuda', 'mps')
         :param batch_size: batch size for batched processing mode
+        :param kwargs: other arguments to initialize PyTorch GNN model
         '''
 
         if model is not None:
             if model_path is not None or model_type is not None:
                 raise ArgumentError(
                     'You cannot specify both graph NN model '
                     'and one of the parameters "model_path" and "model_type".'
                 )
             device = next(model.parameters()).device
-        elif model_path is not None:
-            if model_type is not None:
-                raise ArgumentError(
-                    'You should specify either "model_path" or "model_type" '
-                    'parameter, but not both.'
-                )
-            model = nn.Module()
-            model.load_state_dict(torch.load(model_path))  # ???
         elif model_type is not None:
             if model_type == 'gcn':
-                model = GCN()  # default params
-                path = get_model_path('gcn')
-                model.load_state_dict(torch.load(path))
+                model = GCN(**kwargs)
             elif model_type == 'gat':
-                model = GAT()  # default params
-                path = get_model_path('gat')
-                model.load_state_dict(torch.load(path))
+                model = GAT(**kwargs)
             else:
                 raise ArgumentError(f'Unknown GNN model type "{model_type}".')
+            path = model_path or get_model_path(model_type)
+            model.load_state_dict(torch.load(path))
+        elif model_path is not None:
+            raise ArgumentError(
+                'You should specify "model_type" parameter to use "model_path".'
+            )
         else:
-            model = GCN()  # default params
+            model = GCN(**kwargs)
             path = get_model_path('gcn')
             model.load_state_dict(torch.load(path))
 
         model.eval()
         self.__attrs_init__(
             model=model,
             device=device,
@@ -689,20 +693,21 @@
         '''
         Compute similarity score for given tree pairs.
 
         :param tree_pairs: list of pairs of attributed sentence trees
         :return: list of tree similarity score values
         '''
 
+        self.model.eval()
         dataset = build_pyg_dataset(tree_pairs)
         loader = DataLoader(dataset, batch_size=self.batch_size, shuffle=False)
         predictions = []
         for batch in loader:
             y_pred = self.model(batch.to(self.device)).detach()
-            predictions.extend(y_pred[:, 1])
+            predictions.extend(y_pred[:, 0])
         return predictions
 
     def compute(self, lhs: Tree, rhs: Tree) -> float:
         '''
         Compute similarity score for two given trees.
 
         :param lhs: left-hand side operand, attributed tree of a sentence
```

### Comparing `semsim-0.0.0/semsim/algo/neural.py` & `semsim-1.1.0/semsim/algo/neural.py`

 * *Files 12% similar despite different names*

```diff
@@ -103,32 +103,30 @@
         )
         dataset.append(data)
 
     return dataset
 
 
 class GCN(nn.Module):
-    '''Graph convolutional classification network implementation.'''
+    '''Graph convolutional binary classification network implementation.'''
 
     def __init__(
         self,
         *,
         input_dim: int = 300,
         hidden_dim: int = 64,
-        output_dim: int = 2,
-        num_layers: int = 8,
+        num_layers: int = 1,
         dropout: float = 0,
         edge_dim: int | None = None,
     ):
         '''
         GCN initialization.
 
         :param input_dim: dimensionality of an input vector
         :param hidden_dim: dimensionality of vectors in hidden layers
-        :param output_dim: number of classes
         :param num_layers: number of hidden convolutional layers
         :param dropout: dropout rate
         :param edge_dim: dimensionality of edge attribute vectors
         '''
 
         super().__init__()
 
@@ -140,23 +138,24 @@
             self.convs.append(pyg_nn.Sequential('x, edge_index', [
                 (pyg_nn.convs.GCNConv(
                     in_dim,
                     hidden_dim,
                     concat=False,
                     edge_dim=edge_dim,
                 ), 'x, edge_index -> x'),
+                pyg_nn.norm.GraphNorm(in_channels=hidden_dim),
                 nn.PReLU(num_parameters=hidden_dim),
             ]))
 
         self.post_mp = nn.Sequential(
             nn.Linear(hidden_dim, hidden_dim),
             nn.Dropout(dropout),
             nn.PReLU(num_parameters=hidden_dim),
-            nn.Linear(hidden_dim, output_dim),
-            nn.Softmax(dim=-1),
+            nn.Linear(hidden_dim, 1),
+            nn.Sigmoid(),
         )
 
     def forward(self, data: DataBatch) -> Tensor:
         '''
         Apply a forward pass for a data batch.
 
         :param data: torch_geometric.data.batch.DataBatch instance to process
@@ -170,34 +169,32 @@
         x = pyg_nn.global_max_pool(x, batch)
         x = self.post_mp(x)
 
         return x
 
 
 class GAT(nn.Module):
-    '''Graph attention classification network implementation.'''
+    '''Graph attention binary classification network implementation.'''
 
     def __init__(
         self,
         *,
         input_dim: int = 300,
         hidden_dim: int = 64,
-        output_dim: int = 2,
-        num_heads: int = 8,
-        num_layers: int = 8,
+        num_heads: int = 1,
+        num_layers: int = 1,
         dropout: float = 0,
-        negative_slope: float = 0.1,
+        negative_slope: float = 0.2,
         edge_dim: int | None = None,
     ):
         '''
         GAT initialization.
 
         :param input_dim: dimensionality of an input vector
         :param hidden_dim: dimensionality of vectors in hidden layers
-        :param output_dim: number of classes
         :param num_heads: number of attention heads
         :param num_layers: number of hidden convolutional layers (per each attention head)
         :param dropout: dropout rate
         :param negative_slope: slope coefficient for LeakyReLU layers of attention heads
         :param edge_dim: dimensionality of edge attribute vectors
         '''
 
@@ -213,23 +210,24 @@
                     in_dim,
                     hidden_dim,
                     num_heads,
                     concat=False,
                     edge_dim=edge_dim,
                     negative_slope=negative_slope,
                 ), 'x, edge_index, edge_attr -> x'),
+                pyg_nn.norm.GraphNorm(in_channels=hidden_dim),
                 nn.PReLU(num_parameters=hidden_dim),
             ]))
 
         self.post_mp = nn.Sequential(
             nn.Linear(hidden_dim, hidden_dim),
             nn.Dropout(dropout),
             nn.PReLU(num_parameters=hidden_dim),
-            nn.Linear(hidden_dim, output_dim),
-            nn.Softmax(dim=-1),
+            nn.Linear(hidden_dim, 1),
+            nn.Sigmoid(),
         )
 
     def forward(self, data: DataBatch) -> Tensor:
         '''
         Apply a forward pass for a data batch.
 
         :param data: torch_geometric.data.batch.DataBatch instance to process
@@ -248,69 +246,83 @@
 
 def train_gnn(
     model: nn.Module,
     train_loader: DataLoader,
     n_epochs: int,
     optimizer: Optimizer,
     scheduler: LRScheduler | None = None,
-    eval_loss: Callable[[Tensor, Tensor], Tensor] = fn.cross_entropy,
+    eval_loss: Callable[[Tensor, Tensor], Tensor] = fn.binary_cross_entropy,
     val_loader: DataLoader | None = None,
     *,
     verbose: bool = True,
-) -> tuple[nn.Module, list[float], list[float]]:
+) -> tuple[nn.Module, list[float], list[float], list[float]]:
     '''
     Train a graph neural network classifier.
 
     :param model: model to train
     :param train_loader: data loader for training
     :param n_epochs: number of epochs to train a model for
     :param optimizer: PyTorch Optimizer instance
     :param scheduler: PyTorch LRScheduler instance
     :param eval_loss: callback to evaluate loss function on a data batch
     :param val_loader: data loader for validation
     :param verbose: verbosity flag
-    :return: trained model, list of mean batch loss per training epoch, and list of validation accuracy values
+    :return: trained model, list of mean batch loss per training epoch, \
+        list of train accuracy values, and list of validation accuracy values
     '''
 
     train_loss = []
+    train_accuracy = []
     val_accuracy = []
 
     device = next(model.parameters()).device
+    train_size = len(train_loader.dataset)
     val_size = len(val_loader.dataset) if val_loader is not None else 0
 
     with tqdm(range(n_epochs), desc='Training GNN...', total=n_epochs, disable=not verbose) as bar:
         for epoch in bar:
             batch_train_loss = []
+            batch_train_accuracy = 0
             batch_val_accuracy = 0
 
             model.train()
             for batch in train_loader:
                 batch = batch.to(device)
-                logits = model(batch)
-                labels = batch.y
+                logits = model(batch)[:, 0]
+                labels = batch.y.type(torch.float)
 
                 loss = eval_loss(logits, labels)
 
                 loss.backward()
                 optimizer.step()
                 if scheduler is not None:
                     scheduler.step()
                 optimizer.zero_grad()
 
                 batch_train_loss.append(float(loss.data.numpy()))
+                pred = (logits > 0.5)
+                batch_train_accuracy += (labels == pred).numpy().sum()
             train_loss.append(float(np.mean(batch_train_loss)))
+            train_accuracy.append(batch_train_accuracy / train_size)
 
             if val_loader is not None:
                 model.eval()
                 for batch in val_loader:
                     batch = batch.to(device)
-                    logits = model(batch)
-                    pred = torch.argmax(logits, dim=1)
-                    labels = batch.y
+                    logits = model(batch)[:, 0]
+                    labels = batch.y.type(torch.float)
+                    pred = (logits > 0.5)
                     batch_val_accuracy += (labels == pred).numpy().sum()
                 val_accuracy.append(batch_val_accuracy / val_size)
 
-                bar.set_postfix(loss=f'{train_loss[-1]:.4f}', acc=f'{val_accuracy[-1] * 100:.4f}')
+                bar.set_postfix(
+                    loss=f'{train_loss[-1]:.4f}',
+                    train_acc=f'{train_accuracy[-1] * 100:.4f}',
+                    val_acc=f'{val_accuracy[-1] * 100:.4f}',
+                )
             else:
-                bar.set_postfix(loss=f'{train_loss[-1]:.4f}')
+                bar.set_postfix(
+                    loss=f'{train_loss[-1]:.4f}',
+                    train_acc=f'{train_accuracy[-1] * 100:.4f}',
+                )
 
-    return model, train_loss, val_accuracy
+    return model, train_loss, train_accuracy, val_accuracy
```

### Comparing `semsim-0.0.0/semsim/algo/parser.py` & `semsim-1.1.0/semsim/algo/parser.py`

 * *Files identical despite different names*

### Comparing `semsim-0.0.0/semsim/algo/representation.py` & `semsim-1.1.0/semsim/algo/representation.py`

 * *Files identical despite different names*

### Comparing `semsim-0.0.0/semsim/algo/tag.py` & `semsim-1.1.0/semsim/algo/tag.py`

 * *Files identical despite different names*

### Comparing `semsim-0.0.0/semsim/algo/tree.py` & `semsim-1.1.0/semsim/algo/tree.py`

 * *Files identical despite different names*

### Comparing `semsim-0.0.0/semsim/download.py` & `semsim-1.1.0/semsim/download.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,24 +28,24 @@
 
 BASE_URL = 'https://cloud-api.yandex.net/v1/disk/public/resources/download?'
 FILE_NAMES = {
     'udpipe': 'russian-syntagrus-ud-2.5-191206.udpipe',
     'cbow': 'ruwikiruscorpora_upos_cbow_300_2021.txt',
     'elmo1024': 'ruwikiruscorpora_lemmas_elmo_1024_2019.zip',
     'elmo2048': 'araneum_lemmas_elmo_2048_2020.zip',
-    'gcn': '',
-    'gat': '',
+    'gcn': 'gcn_model.pth',
+    'gat': 'gat_model.pth',
 }
 FILE_URLS = {
     'udpipe': 'https://disk.yandex.ru/d/Pz17-vtNeasApg',
     'cbow': 'https://disk.yandex.ru/d/6dXzkn0r9Otjnw',
     'elmo1024': 'https://disk.yandex.ru/d/mIZRldOR6B16rw',
     'elmo2048': 'https://disk.yandex.ru/d/fAl1ON3JKmWwDQ',
-    'gcn': '',  # TODO
-    'gat': '',  # TODO
+    'gcn': 'https://disk.yandex.ru/d/kI010Uqj2F51zw',
+    'gat': 'https://disk.yandex.ru/d/9_0I88hnEz2G0w',
 }
 CHUNK_SIZE = 8_192
 
 
 def get_model_path(file: str) -> Path:
     '''
     Get path to a built-in model if present.
@@ -108,14 +108,19 @@
     :param force: whether to force downloading existing files
     :return: None
     '''
 
     if file == 'elmo':
         download('elmo1024')
         download('elmo2048')
+        return
+    if file == 'neural':
+        download('gcn')
+        download('gat')
+        return
 
     MODELS_DIR.mkdir(exist_ok=True)
     path = get_model_path(file)
     if not path.exists() or force:
         if verbose:
             logger.info(f'Downloading "{file}"...')
```

### Comparing `semsim-0.0.0/semsim/exception.py` & `semsim-1.1.0/semsim/exception.py`

 * *Files identical despite different names*

### Comparing `semsim-0.0.0/semsim/interface/cli.py` & `semsim-1.1.0/semsim/interface/cli.py`

 * *Files identical despite different names*

### Comparing `semsim-0.0.0/semsim/logger.py` & `semsim-1.1.0/semsim/logger.py`

 * *Files identical despite different names*

### Comparing `semsim-0.0.0/semsim.egg-info/SOURCES.txt` & `semsim-1.1.0/semsim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `semsim-0.0.0/setup.cfg` & `semsim-1.1.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 allow_untyped_decorators = True
 
 [tool:pytest]
 timeout = 60
 
 [metadata]
 name = semsim
-version = 0.0.0
+version = 1.1.0
 author = David Avagyan
 author_email = david_avagyan@list.ru
 description = A free tool for sentence similarity evaluation
 long_description = file: pypi_readme.md
 long_description_content_type = text/markdown
 keywords = NLP, dependency parsing, CoNLL-U, sentence similarity
 url = https://gitlab.com/Mathematician2000/semsim
```

