# Comparing `tmp/board-game-recommender-3.3.0.tar.gz` & `tmp/board-game-recommender-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "board-game-recommender-3.3.0.tar", last modified: Sat May  6 19:41:30 2023, max compression
+gzip compressed data, was "board-game-recommender-3.4.0.tar", last modified: Mon May  8 19:07:24 2023, max compression
```

## Comparing `board-game-recommender-3.3.0.tar` & `board-game-recommender-3.4.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 markus     (501) staff       (20)        0 2023-05-06 19:41:30.912780 board-game-recommender-3.3.0/
--rw-r--r--   0 markus     (501) staff       (20)     1072 2020-09-18 05:15:08.000000 board-game-recommender-3.3.0/LICENSE
--rw-r--r--   0 markus     (501) staff       (20)       26 2021-11-28 20:14:53.000000 board-game-recommender-3.3.0/MANIFEST.in
--rw-r--r--   0 markus     (501) staff       (20)     4074 2023-05-06 19:41:30.912400 board-game-recommender-3.3.0/PKG-INFO
--rw-r--r--   0 markus     (501) staff       (20)     2704 2021-05-19 13:26:08.000000 board-game-recommender-3.3.0/README.md
-drwxr-xr-x   0 markus     (501) staff       (20)        0 2023-05-06 19:41:30.909205 board-game-recommender-3.3.0/board_game_recommender/
--rw-r--r--   0 markus     (501) staff       (20)      429 2023-04-11 10:14:59.000000 board-game-recommender-3.3.0/board_game_recommender/__init__.py
--rw-r--r--   0 markus     (501) staff       (20)     5544 2023-05-01 18:48:43.000000 board-game-recommender-3.3.0/board_game_recommender/__main__.py
--rw-r--r--   0 markus     (501) staff       (20)       78 2023-05-06 19:40:57.000000 board-game-recommender-3.3.0/board_game_recommender/__version__.py
--rw-r--r--   0 markus     (501) staff       (20)     2124 2023-04-30 20:00:56.000000 board-game-recommender-3.3.0/board_game_recommender/base.py
--rw-r--r--   0 markus     (501) staff       (20)     7041 2023-05-02 19:45:34.000000 board-game-recommender-3.3.0/board_game_recommender/baseline.py
--rw-r--r--   0 markus     (501) staff       (20)     3043 2023-05-06 19:40:40.000000 board-game-recommender-3.3.0/board_game_recommender/evaluation.py
--rw-r--r--   0 markus     (501) staff       (20)     9584 2023-05-01 20:18:49.000000 board-game-recommender-3.3.0/board_game_recommender/hyperparameter.py
--rw-r--r--   0 markus     (501) staff       (20)    10190 2023-05-06 19:40:40.000000 board-game-recommender-3.3.0/board_game_recommender/light.py
--rw-r--r--   0 markus     (501) staff       (20)     4766 2023-04-11 10:14:59.000000 board-game-recommender-3.3.0/board_game_recommender/rankings.py
--rw-r--r--   0 markus     (501) staff       (20)    33402 2023-05-02 19:47:04.000000 board-game-recommender-3.3.0/board_game_recommender/recommend.py
--rw-r--r--   0 markus     (501) staff       (20)     2099 2023-04-11 10:14:59.000000 board-game-recommender-3.3.0/board_game_recommender/trust.py
--rw-r--r--   0 markus     (501) staff       (20)     3767 2023-04-30 20:37:05.000000 board-game-recommender-3.3.0/board_game_recommender/utils.py
-drwxr-xr-x   0 markus     (501) staff       (20)        0 2023-05-06 19:41:30.911793 board-game-recommender-3.3.0/board_game_recommender.egg-info/
--rw-r--r--   0 markus     (501) staff       (20)     4074 2023-05-06 19:41:30.000000 board-game-recommender-3.3.0/board_game_recommender.egg-info/PKG-INFO
--rw-r--r--   0 markus     (501) staff       (20)      686 2023-05-06 19:41:30.000000 board-game-recommender-3.3.0/board_game_recommender.egg-info/SOURCES.txt
--rw-r--r--   0 markus     (501) staff       (20)        1 2023-05-06 19:41:30.000000 board-game-recommender-3.3.0/board_game_recommender.egg-info/dependency_links.txt
--rw-r--r--   0 markus     (501) staff       (20)       99 2023-05-06 19:41:30.000000 board-game-recommender-3.3.0/board_game_recommender.egg-info/requires.txt
--rw-r--r--   0 markus     (501) staff       (20)       23 2023-05-06 19:41:30.000000 board-game-recommender-3.3.0/board_game_recommender.egg-info/top_level.txt
--rw-r--r--   0 markus     (501) staff       (20)       38 2023-05-06 19:41:30.912912 board-game-recommender-3.3.0/setup.cfg
--rwxr-xr-x   0 markus     (501) staff       (20)     4993 2023-04-30 20:00:56.000000 board-game-recommender-3.3.0/setup.py
+drwxr-xr-x   0 markus     (501) staff       (20)        0 2023-05-08 19:07:24.006185 board-game-recommender-3.4.0/
+-rw-r--r--   0 markus     (501) staff       (20)     1072 2020-09-18 05:15:08.000000 board-game-recommender-3.4.0/LICENSE
+-rw-r--r--   0 markus     (501) staff       (20)       26 2021-11-28 20:14:53.000000 board-game-recommender-3.4.0/MANIFEST.in
+-rw-r--r--   0 markus     (501) staff       (20)     4074 2023-05-08 19:07:24.005760 board-game-recommender-3.4.0/PKG-INFO
+-rw-r--r--   0 markus     (501) staff       (20)     2704 2021-05-19 13:26:08.000000 board-game-recommender-3.4.0/README.md
+drwxr-xr-x   0 markus     (501) staff       (20)        0 2023-05-08 19:07:24.001628 board-game-recommender-3.4.0/board_game_recommender/
+-rw-r--r--   0 markus     (501) staff       (20)      429 2023-04-11 10:14:59.000000 board-game-recommender-3.4.0/board_game_recommender/__init__.py
+-rw-r--r--   0 markus     (501) staff       (20)     5544 2023-05-01 18:48:43.000000 board-game-recommender-3.4.0/board_game_recommender/__main__.py
+-rw-r--r--   0 markus     (501) staff       (20)       78 2023-05-08 19:07:00.000000 board-game-recommender-3.4.0/board_game_recommender/__version__.py
+-rw-r--r--   0 markus     (501) staff       (20)     2124 2023-04-30 20:00:56.000000 board-game-recommender-3.4.0/board_game_recommender/base.py
+-rw-r--r--   0 markus     (501) staff       (20)     8072 2023-05-08 19:06:12.000000 board-game-recommender-3.4.0/board_game_recommender/baseline.py
+-rw-r--r--   0 markus     (501) staff       (20)     4994 2023-05-08 11:42:39.000000 board-game-recommender-3.4.0/board_game_recommender/evaluation.py
+-rw-r--r--   0 markus     (501) staff       (20)     9584 2023-05-01 20:18:49.000000 board-game-recommender-3.4.0/board_game_recommender/hyperparameter.py
+-rw-r--r--   0 markus     (501) staff       (20)    10733 2023-05-08 19:06:12.000000 board-game-recommender-3.4.0/board_game_recommender/light.py
+-rw-r--r--   0 markus     (501) staff       (20)     4766 2023-04-11 10:14:59.000000 board-game-recommender-3.4.0/board_game_recommender/rankings.py
+-rw-r--r--   0 markus     (501) staff       (20)    33402 2023-05-02 19:47:04.000000 board-game-recommender-3.4.0/board_game_recommender/recommend.py
+-rw-r--r--   0 markus     (501) staff       (20)     2099 2023-04-11 10:14:59.000000 board-game-recommender-3.4.0/board_game_recommender/trust.py
+-rw-r--r--   0 markus     (501) staff       (20)     3767 2023-04-30 20:37:05.000000 board-game-recommender-3.4.0/board_game_recommender/utils.py
+drwxr-xr-x   0 markus     (501) staff       (20)        0 2023-05-08 19:07:24.005128 board-game-recommender-3.4.0/board_game_recommender.egg-info/
+-rw-r--r--   0 markus     (501) staff       (20)     4074 2023-05-08 19:07:23.000000 board-game-recommender-3.4.0/board_game_recommender.egg-info/PKG-INFO
+-rw-r--r--   0 markus     (501) staff       (20)      686 2023-05-08 19:07:23.000000 board-game-recommender-3.4.0/board_game_recommender.egg-info/SOURCES.txt
+-rw-r--r--   0 markus     (501) staff       (20)        1 2023-05-08 19:07:23.000000 board-game-recommender-3.4.0/board_game_recommender.egg-info/dependency_links.txt
+-rw-r--r--   0 markus     (501) staff       (20)       99 2023-05-08 19:07:23.000000 board-game-recommender-3.4.0/board_game_recommender.egg-info/requires.txt
+-rw-r--r--   0 markus     (501) staff       (20)       23 2023-05-08 19:07:23.000000 board-game-recommender-3.4.0/board_game_recommender.egg-info/top_level.txt
+-rw-r--r--   0 markus     (501) staff       (20)       38 2023-05-08 19:07:24.006324 board-game-recommender-3.4.0/setup.cfg
+-rwxr-xr-x   0 markus     (501) staff       (20)     4993 2023-04-30 20:00:56.000000 board-game-recommender-3.4.0/setup.py
```

### Comparing `board-game-recommender-3.3.0/LICENSE` & `board-game-recommender-3.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `board-game-recommender-3.3.0/PKG-INFO` & `board-game-recommender-3.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: board-game-recommender
-Version: 3.3.0
+Version: 3.4.0
 Summary: Board games recommender engine
 Home-page: https://recommend.games/
 Author: Markus Shepherd
 Author-email: markus@recommend.games
 License: MIT
 Project-URL: Documentation, https://gitlab.com/recommend.games/board-game-recommender/blob/master/README.md
 Project-URL: Funding, https://paypal.me/mschepke
```

### Comparing `board-game-recommender-3.3.0/README.md` & `board-game-recommender-3.4.0/README.md`

 * *Files identical despite different names*

### Comparing `board-game-recommender-3.3.0/board_game_recommender/__main__.py` & `board-game-recommender-3.4.0/board_game_recommender/__main__.py`

 * *Files identical despite different names*

### Comparing `board-game-recommender-3.3.0/board_game_recommender/base.py` & `board-game-recommender-3.4.0/board_game_recommender/base.py`

 * *Files identical despite different names*

### Comparing `board-game-recommender-3.3.0/board_game_recommender/baseline.py` & `board-game-recommender-3.4.0/board_game_recommender/baseline.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Baseline recommender models."""
 
 import logging
 import os
-from typing import Any, FrozenSet, Iterable, List, Optional, Union
+from collections import defaultdict
+from typing import Any, Dict, FrozenSet, Iterable, List, Optional, Tuple, Union
 
 import numpy as np
 import pandas as pd
 
 from board_game_recommender.base import BaseGamesRecommender
 
 LOGGER = logging.getLogger(__name__)
@@ -92,18 +93,36 @@
 class PopularGamesRecommender(BaseGamesRecommender):
     """Popular games recommender."""
 
     id_field: str = "bgg_id"
     user_id_field: str = "bgg_user_name"
     rating_id_field: str = "bgg_user_rating"
 
+    scores: Dict[int, float]
+    raw_scores: np.ndarray
+    default_value: float
+    game_ids: Tuple[int, ...]
+
     _known_games: Optional[FrozenSet[int]] = None
 
-    def __init__(self, data: pd.Series) -> None:
-        self.data = data
+    def __init__(
+        self,
+        game_ids: Iterable[int],
+        scores: np.ndarray,
+        default_value: Optional[float] = None,
+    ) -> None:
+        self.default_value = (
+            default_value if default_value is not None else scores.mean()
+        )
+        self.raw_scores = scores
+        self.game_ids = tuple(game_ids)
+        self.scores = defaultdict(
+            self.default_factory,
+            zip(self.game_ids, self.raw_scores),
+        )
 
     @classmethod
     def train(cls, ratings: pd.DataFrame) -> "PopularGamesRecommender":
         """Train the recommender from ratings data."""
         raise NotImplementedError
 
     @classmethod
@@ -134,47 +153,55 @@
             ]
         )
 
     @property
     def known_games(self) -> FrozenSet[int]:
         if self._known_games is not None:
             return self._known_games
-        self._known_games = frozenset(self.data.index)
+        self._known_games = frozenset(self.game_ids)
         return self._known_games
 
     @property
     def rated_games(self) -> FrozenSet[int]:
         return self.known_games
 
     @property
     def num_games(self) -> int:
-        return len(self.data)
+        return len(self.game_ids)
 
     @property
     def known_users(self) -> FrozenSet[str]:
         return frozenset()
 
+    def default_factory(self) -> float:
+        """Default value for unknown games."""
+        return self.default_value
+
     def _recommendation_scores(
         self,
         users: int,
         games: Optional[List[int]] = None,
     ) -> np.ndarray:
         """Popularity scores."""
-        scores = self.data.loc[games] if games else self.data
-        return np.tile(scores.to_numpy(), [users, 1])
+        scores = (
+            np.array([self.scores[game_id] for game_id in games])
+            if games
+            else self.raw_scores
+        )
+        return np.tile(scores, [users, 1])
 
     def recommend(
         self,
         users: Iterable[str],
         **kwargs,
     ) -> pd.DataFrame:
         """Popular recommendations for certain users."""
         users = list(users)
         scores = self._recommendation_scores(users=len(users))
-        return dataframe_from_scores(users, self.data.index, scores)
+        return dataframe_from_scores(users, self.game_ids, scores)
 
     def recommend_as_numpy(
         self,
         users: Iterable[str],
         games: Iterable[int],
     ) -> np.ndarray:
         """Random recommendations for certain users and games as a numpy array."""
@@ -191,15 +218,19 @@
 
 class PopularMeanGamesRecommender(PopularGamesRecommender):
     """Recommend games by their mean rating score."""
 
     @classmethod
     def train(cls, ratings: pd.DataFrame) -> "PopularMeanGamesRecommender":
         data = ratings.groupby(cls.id_field, sort=False)[cls.rating_id_field].mean()
-        return cls(data=data)
+        return cls(
+            game_ids=data.index,
+            scores=data.to_numpy(),
+            default_value=ratings[cls.rating_id_field].mean(),
+        )
 
 
 class PopularBayesianGamesRecommender(PopularGamesRecommender):
     """Recommend games by their Bayesian average rating score."""
 
     ratings_per_dummy: float = 10_000
     dummy_rating: Optional[float] = 5.5
@@ -220,17 +251,21 @@
             cls.rating_id_field
         ].agg(["size", "mean"])
 
         data = (stats["mean"] * stats["size"] + dummy_rating * num_dummies) / (
             stats["size"] + num_dummies
         )
 
-        return cls(data=data)
+        return cls(
+            game_ids=data.index,
+            scores=data.to_numpy(),
+            default_value=dummy_rating,
+        )
 
 
 class PopularNumRatingsGamesRecommender(PopularGamesRecommender):
     """Recommend games by their number of ratings."""
 
     @classmethod
     def train(cls, ratings: pd.DataFrame) -> "PopularNumRatingsGamesRecommender":
         data = ratings.groupby(cls.id_field, sort=False).size()
-        return cls(data=data)
+        return cls(game_ids=data.index, scores=data.to_numpy())
```

### Comparing `board-game-recommender-3.3.0/board_game_recommender/hyperparameter.py` & `board-game-recommender-3.4.0/board_game_recommender/hyperparameter.py`

 * *Files identical despite different names*

### Comparing `board-game-recommender-3.3.0/board_game_recommender/light.py` & `board-game-recommender-3.4.0/board_game_recommender/light.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Light recommender model, without the heavy Turi Create dependency."""
 
 import logging
+from collections import defaultdict
 from dataclasses import asdict, dataclass
 from pathlib import Path
 from typing import TYPE_CHECKING, FrozenSet, Iterable, List, Optional, Type, Union
 
 import numpy as np
 import pandas as pd
 
@@ -69,25 +70,43 @@
 
     def __init__(
         self: "LightGamesRecommender",
         data: CollaborativeFilteringData,
     ) -> None:
         self.data = data
 
+        assert data.users_factors.shape[-1] == data.items_factors.shape[0]
+        num_factors = data.items_factors.shape[0]
+        # TODO check other dimensions as well (num_users and num_items)
+
         self.intercept: float = data.intercept
 
+        num_users = len(data.users_labels)
         self.users_labels: List[str] = list(data.users_labels)
-        self.users_indexes = dict(zip(data.users_labels, range(len(data.users_labels))))
-        self.users_linear_terms = data.users_linear_terms
-        self.users_factors = data.users_factors
+        self.users_indexes = defaultdict(
+            lambda: -1,
+            zip(data.users_labels, range(num_users)),
+        )
+        self.users_linear_terms = np.concatenate((data.users_linear_terms, np.zeros(1)))
+        self.users_factors = np.concatenate(
+            (data.users_factors, np.zeros((1, num_factors))),
+            axis=0,
+        )
 
+        num_items = len(data.items_labels)
         self.items_labels: List[int] = list(data.items_labels)
-        self.items_indexes = dict(zip(data.items_labels, range(len(data.items_labels))))
-        self.items_linear_terms = data.items_linear_terms
-        self.items_factors = data.items_factors
+        self.items_indexes = defaultdict(
+            lambda: -1,
+            zip(data.items_labels, range(num_items)),
+        )
+        self.items_linear_terms = np.concatenate((data.items_linear_terms, np.zeros(1)))
+        self.items_factors = np.concatenate(
+            (data.items_factors, np.zeros((num_factors, 1))),
+            axis=1,
+        )
 
         LOGGER.info(
             "Loaded light recommender with %d users and %d items",
             len(self.users_labels),
             len(self.items_labels),
         )
 
@@ -147,32 +166,30 @@
         users: Optional[List[str]] = None,
         games: Optional[List[int]] = None,
     ) -> np.ndarray:
         """Calculate recommendations scores for certain users and games."""
 
         if users:
             user_ids = np.array([self.users_indexes[user] for user in users])
-            user_factors = self.users_factors[user_ids]
+            users_factors = self.users_factors[user_ids]
             users_linear_terms = self.users_linear_terms[user_ids].reshape(-1, 1)
         else:
-            user_factors = self.users_factors
-            users_linear_terms = self.users_linear_terms.reshape(-1, 1)
+            users_factors = self.users_factors[:-1, :]
+            users_linear_terms = self.users_linear_terms[:-1].reshape(-1, 1)
 
         if games:
-            # TODO Unknown games will cause a key error. Instead, use the user's
-            # average predicted rating (user + global bias) for unknown games. (#57)
             game_ids = np.array([self.items_indexes[game] for game in games])
             items_factors = self.items_factors[:, game_ids]
             items_linear_terms = self.items_linear_terms[game_ids].reshape(1, -1)
         else:
-            items_factors = self.items_factors
-            items_linear_terms = self.items_linear_terms.reshape(1, -1)
+            items_factors = self.items_factors[:, :-1]
+            items_linear_terms = self.items_linear_terms[:-1].reshape(1, -1)
 
         return (
-            user_factors @ items_factors  # (num_users, num_items)
+            users_factors @ items_factors  # (num_users, num_items)
             + users_linear_terms  # (num_users, 1)
             + items_linear_terms  # (1, num_items)
             + self.intercept  # (1,)
         )
 
     def recommend(
         self: "LightGamesRecommender",
@@ -205,15 +222,17 @@
         Recommend games similar to the given games based on cosine similarity of latent factors.
         """
 
         games = list(games)
         game_ids = np.array([self.items_indexes[game] for game in games])
         game_factors = self.items_factors[:, game_ids]
 
-        scores = cosine_similarity(game_factors, self.items_factors).mean(axis=0)
+        scores = cosine_similarity(game_factors, self.items_factors[:, :-1]).mean(
+            axis=0
+        )
 
         result = pd.DataFrame(index=self.items_labels, data={"score": scores})
         result["rank"] = result["score"].rank(method="min", ascending=False).astype(int)
         result.sort_values("rank", inplace=True)
 
         return result
 
@@ -224,15 +243,15 @@
     ) -> pd.DataFrame:
         """Find games similar to the given games based on cosine similarity of latent factors."""
 
         games = list(games)
         game_ids = np.array([self.items_indexes[game] for game in games])
         game_factors = self.items_factors[:, game_ids]
 
-        scores = cosine_similarity(game_factors, self.items_factors)
+        scores = cosine_similarity(game_factors, self.items_factors[:, :-1])
         return dataframe_from_scores(games, self.items_labels, scores)
 
 
 def cosine_similarity(matrix_1: np.ndarray, matrix_2: np.ndarray) -> np.ndarray:
     """
     Calculates the cosine similarity between two matrices.
```

### Comparing `board-game-recommender-3.3.0/board_game_recommender/rankings.py` & `board-game-recommender-3.4.0/board_game_recommender/rankings.py`

 * *Files identical despite different names*

### Comparing `board-game-recommender-3.3.0/board_game_recommender/recommend.py` & `board-game-recommender-3.4.0/board_game_recommender/recommend.py`

 * *Files identical despite different names*

### Comparing `board-game-recommender-3.3.0/board_game_recommender/trust.py` & `board-game-recommender-3.4.0/board_game_recommender/trust.py`

 * *Files identical despite different names*

### Comparing `board-game-recommender-3.3.0/board_game_recommender/utils.py` & `board-game-recommender-3.4.0/board_game_recommender/utils.py`

 * *Files identical despite different names*

### Comparing `board-game-recommender-3.3.0/board_game_recommender.egg-info/PKG-INFO` & `board-game-recommender-3.4.0/board_game_recommender.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: board-game-recommender
-Version: 3.3.0
+Version: 3.4.0
 Summary: Board games recommender engine
 Home-page: https://recommend.games/
 Author: Markus Shepherd
 Author-email: markus@recommend.games
 License: MIT
 Project-URL: Documentation, https://gitlab.com/recommend.games/board-game-recommender/blob/master/README.md
 Project-URL: Funding, https://paypal.me/mschepke
```

### Comparing `board-game-recommender-3.3.0/board_game_recommender.egg-info/SOURCES.txt` & `board-game-recommender-3.4.0/board_game_recommender.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `board-game-recommender-3.3.0/setup.py` & `board-game-recommender-3.4.0/setup.py`

 * *Files identical despite different names*

