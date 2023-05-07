# Comparing `tmp/no-teg-0.2.0.tar.gz` & `tmp/no-teg-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "no-teg-0.2.0.tar", last modified: Tue Mar 28 21:34:23 2023, max compression
+gzip compressed data, was "no-teg-0.2.1.tar", last modified: Sun May  7 23:54:53 2023, max compression
```

## Comparing `no-teg-0.2.0.tar` & `no-teg-0.2.1.tar`

### file list

```diff
@@ -1,23 +1,45 @@
-drwxrwxrwx   0        0        0        0 2023-03-28 21:34:23.323217 no-teg-0.2.0/
--rw-rw-rw-   0        0        0      307 2023-03-28 21:29:44.000000 no-teg-0.2.0/.bumpversion.cfg
--rw-rw-rw-   0        0        0      187 2023-03-26 15:43:31.000000 no-teg-0.2.0/CONTRIBUTING.md
--rw-rw-rw-   0        0        0    11558 2023-02-19 17:46:54.000000 no-teg-0.2.0/LICENSE
--rw-rw-rw-   0        0        0      384 2023-03-26 15:43:31.000000 no-teg-0.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2314 2023-03-26 15:43:31.000000 no-teg-0.2.0/Makefile
--rw-rw-rw-   0        0        0    16500 2023-03-28 21:34:23.322198 no-teg-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     2493 2023-03-28 19:00:13.000000 no-teg-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-03-28 21:34:23.265872 no-teg-0.2.0/no_teg/
--rw-rw-rw-   0        0        0       48 2023-03-28 21:29:44.000000 no-teg-0.2.0/no_teg/__init__.py
--rw-rw-rw-   0        0        0      116 2023-03-26 15:43:31.000000 no-teg-0.2.0/no_teg/__main__.py
--rw-rw-rw-   0        0        0     9619 2023-03-28 21:25:02.000000 no-teg-0.2.0/no_teg/no_teg.py
-drwxrwxrwx   0        0        0        0 2023-03-28 21:34:23.318676 no-teg-0.2.0/no_teg/tests/
--rw-rw-rw-   0        0        0     7970 2023-03-28 21:23:20.000000 no-teg-0.2.0/no_teg/tests/test_all.py
-drwxrwxrwx   0        0        0        0 2023-03-28 21:34:23.314481 no-teg-0.2.0/no_teg.egg-info/
--rw-rw-rw-   0        0        0    16500 2023-03-28 21:34:22.000000 no-teg-0.2.0/no_teg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      324 2023-03-28 21:34:22.000000 no-teg-0.2.0/no_teg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-28 21:34:22.000000 no-teg-0.2.0/no_teg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      162 2023-03-28 21:34:22.000000 no-teg-0.2.0/no_teg.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-03-28 21:34:22.000000 no-teg-0.2.0/no_teg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2268 2023-03-28 21:29:44.000000 no-teg-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-28 21:34:23.324443 no-teg-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0       43 2023-03-26 15:43:31.000000 no-teg-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-07 23:54:53.975771 no-teg-0.2.1/
+-rw-rw-rw-   0        0        0      307 2023-05-07 23:48:56.000000 no-teg-0.2.1/.bumpversion.cfg
+-rw-rw-rw-   0        0        0      187 2023-03-26 15:43:31.000000 no-teg-0.2.1/CONTRIBUTING.md
+-rw-rw-rw-   0        0        0    11558 2023-02-19 17:46:54.000000 no-teg-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0      552 2023-05-07 23:19:01.000000 no-teg-0.2.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2316 2023-05-07 23:19:01.000000 no-teg-0.2.1/Makefile
+-rw-rw-rw-   0        0        0    16600 2023-05-07 23:54:53.970560 no-teg-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2593 2023-05-07 23:19:01.000000 no-teg-0.2.1/README.md
+-rw-rw-rw-   0        0        0      121 2023-05-07 23:48:56.000000 no-teg-0.2.1/doc_requirements.txt
+drwxrwxrwx   0        0        0        0 2023-05-07 23:54:53.796448 no-teg-0.2.1/docs/
+-rw-rw-rw-   0        0        0      654 2023-05-07 23:19:01.000000 no-teg-0.2.1/docs/Makefile
+-rw-rw-rw-   0        0        0     1673 2023-05-07 23:54:42.000000 no-teg-0.2.1/docs/conf.py
+-rw-rw-rw-   0        0        0     1915 2023-05-07 23:19:01.000000 no-teg-0.2.1/docs/index.md
+-rwxrwxrwx   0        0        0      800 2023-05-07 23:19:01.000000 no-teg-0.2.1/docs/make.bat
+-rw-rw-rw-   0        0        0       62 2023-05-07 23:19:01.000000 no-teg-0.2.1/docs/modules.rst
+-rw-rw-rw-   0        0        0      347 2023-05-07 23:48:56.000000 no-teg-0.2.1/docs/no_teg.games.rst
+-rw-rw-rw-   0        0        0      319 2023-05-07 23:19:01.000000 no-teg-0.2.1/docs/no_teg.rst
+-rw-rw-rw-   0        0        0      924 2023-05-07 23:48:56.000000 no-teg-0.2.1/docs/no_teg.tests.rst
+-rw-rw-rw-   0        0        0      591 2023-05-07 23:48:56.000000 no-teg-0.2.1/docs/no_teg.tourneys.rst
+drwxrwxrwx   0        0        0        0 2023-05-07 23:54:53.812230 no-teg-0.2.1/no_teg/
+-rw-rw-rw-   0        0        0       48 2023-05-07 23:48:56.000000 no-teg-0.2.1/no_teg/__init__.py
+-rw-rw-rw-   0        0        0      116 2023-03-26 15:43:31.000000 no-teg-0.2.1/no_teg/__main__.py
+drwxrwxrwx   0        0        0        0 2023-05-07 23:54:53.922057 no-teg-0.2.1/no_teg/games/
+-rw-rw-rw-   0        0        0        0 2023-05-07 23:19:01.000000 no-teg-0.2.1/no_teg/games/__init__.py
+-rw-rw-rw-   0        0        0      281 2023-05-07 23:19:01.000000 no-teg-0.2.1/no_teg/games/fifa.py
+-rw-rw-rw-   0        0        0     9525 2023-05-07 23:19:01.000000 no-teg-0.2.1/no_teg/no_teg.py
+drwxrwxrwx   0        0        0        0 2023-05-07 23:54:53.955643 no-teg-0.2.1/no_teg/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-07 23:19:01.000000 no-teg-0.2.1/no_teg/tests/__init__.py
+-rw-rw-rw-   0        0        0      534 2023-05-07 23:19:01.000000 no-teg-0.2.1/no_teg/tests/conftest.py
+-rw-rw-rw-   0        0        0     6826 2023-05-07 23:46:30.000000 no-teg-0.2.1/no_teg/tests/test_all.py
+-rw-rw-rw-   0        0        0     2573 2023-05-07 23:19:01.000000 no-teg-0.2.1/no_teg/tests/test_round_robin.py
+-rw-rw-rw-   0        0        0     5739 2023-05-07 23:19:01.000000 no-teg-0.2.1/no_teg/tests/test_single_elimination.py
+drwxrwxrwx   0        0        0        0 2023-05-07 23:54:53.965033 no-teg-0.2.1/no_teg/tourneys/
+-rw-rw-rw-   0        0        0        0 2023-05-07 23:19:01.000000 no-teg-0.2.1/no_teg/tourneys/__init__.py
+-rw-rw-rw-   0        0        0     3465 2023-05-07 23:19:01.000000 no-teg-0.2.1/no_teg/tourneys/round_robin.py
+-rw-rw-rw-   0        0        0     4704 2023-05-07 23:19:01.000000 no-teg-0.2.1/no_teg/tourneys/single_elimination.py
+drwxrwxrwx   0        0        0        0 2023-05-07 23:54:53.920230 no-teg-0.2.1/no_teg.egg-info/
+-rw-rw-rw-   0        0        0    16600 2023-05-07 23:54:53.000000 no-teg-0.2.1/no_teg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      768 2023-05-07 23:54:53.000000 no-teg-0.2.1/no_teg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 23:54:53.000000 no-teg-0.2.1/no_teg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      162 2023-05-07 23:54:53.000000 no-teg-0.2.1/no_teg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-07 23:54:53.000000 no-teg-0.2.1/no_teg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2268 2023-05-07 23:48:56.000000 no-teg-0.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-07 23:54:53.976404 no-teg-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0       43 2023-03-26 15:43:31.000000 no-teg-0.2.1/setup.py
```

### Comparing `no-teg-0.2.0/LICENSE` & `no-teg-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `no-teg-0.2.0/Makefile` & `no-teg-0.2.1/Makefile`

 * *Files 0% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 
 # Alias
 checks: check
 
 annotate:  ## run type checking
 	python -m mypy ./no_teg
 
+
 #########
 # TESTS #
 #########
 test: ## clean and run unit tests
 	python -m pytest -v no_teg/tests
 
 coverage:  ## clean and run unit tests with coverage
```

### Comparing `no-teg-0.2.0/PKG-INFO` & `no-teg-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: no-teg
-Version: 0.2.0
+Version: 0.2.1
 Summary: A quick and easy tournament manager
 Author-email: Aaron Ashery <aaron.ashery1@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -224,14 +224,15 @@
 A library for running tournaments
 
 ![license](https://img.shields.io/github/license/aaronashery/no-teg)
 ![issues](https://img.shields.io/github/issues/AaronAshery/no-teg)
 [![Build Status](https://github.com/ColumbiaOSS/example-project-python/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/AaronAshery/no-teg/actions?query=workflow%3A%22Build+Status%22)
 [![codecov](https://codecov.io/gh/AaronAshery/no-teg/branch/main/graph/badge.svg)](https://codecov.io/gh/ColumbiaOSS/example-project-python)
 [![PyPI](https://img.shields.io/pypi/v/no-teg)](https://pypi.org/project/no-teg/)
+[![Docs](https://img.shields.io/readthedocs/no-teg.svg)](https://no-teg.readthedocs.io/en/latest/)
 
 ## Overview
 'no-teg' (get-on backwards) is a library for running tournaments. In the beginning it will be simple i.e. setting up and advancing through different tournament styles. Eventually if things go smoothly the library will also compute data on the tournaments and players. Being open-source, I hope that people will add tournament styles and different analysis that are dependent on different games.
 
 ## Install:
 
 `pip install no-teg`
```

### Comparing `no-teg-0.2.0/README.md` & `no-teg-0.2.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 A library for running tournaments
 
 ![license](https://img.shields.io/github/license/aaronashery/no-teg)
 ![issues](https://img.shields.io/github/issues/AaronAshery/no-teg)
 [![Build Status](https://github.com/ColumbiaOSS/example-project-python/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/AaronAshery/no-teg/actions?query=workflow%3A%22Build+Status%22)
 [![codecov](https://codecov.io/gh/AaronAshery/no-teg/branch/main/graph/badge.svg)](https://codecov.io/gh/ColumbiaOSS/example-project-python)
 [![PyPI](https://img.shields.io/pypi/v/no-teg)](https://pypi.org/project/no-teg/)
+[![Docs](https://img.shields.io/readthedocs/no-teg.svg)](https://no-teg.readthedocs.io/en/latest/)
 
 ## Overview
 'no-teg' (get-on backwards) is a library for running tournaments. In the beginning it will be simple i.e. setting up and advancing through different tournament styles. Eventually if things go smoothly the library will also compute data on the tournaments and players. Being open-source, I hope that people will add tournament styles and different analysis that are dependent on different games.
 
 ## Install:
 
 `pip install no-teg`
```

### Comparing `no-teg-0.2.0/no_teg/no_teg.py` & `no-teg-0.2.1/no_teg/no_teg.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,278 +1,452 @@
 from __future__ import annotations
 import numpy as np
 
-# import pandas as pd
 
-# no-teg is quick and dirty, in the future could evolve to a full scale tournament API
+class Game:
+    """
+    A class to represent a game.
 
+    ...
 
-# game could be reduced to a pd df
-# each game just a new row with their specs
+    Attributes
+    ----------
+    name : str
+        name of the game
+    rec_players : int
+        amount of players recommended
+    rec_tourney : Tourney
+        tournament type recommended
+
+    Methods
+    -------
+    set_name(name):
+        Sets the name of the game.
+    set_rec_players(rec_players):
+        Sets the recommended amount of players.
+    set_rec_tourney(rec_tourney):
+        Sets the recommended tournament type.
+    set_labels(labels):
+        Sets the labels for additional stat tracking for the game.
+    get_labels():
+        Gets the labels for the game.
+    """
 
+    def __init__(self):
+        """
+        Constructs the attributes of the Game class.
 
-# game interface
-class Game:
-    """Initialize new game"""
+        Everything is empty upon construction and will need to be set with the class methods.
+
+        Parameters
+        ----------
+        None
+        """
 
-    def __init__(self):
         self.name = None
         self.rec_players = None
         self.rec_tourney = None
         self.labels = []
 
     def set_name(self, name: str):
+        """
+        Sets the name of the game.
+
+        Parameters
+        ----------
+        name : str
+            the name of the person
+
+        Returns
+        -------
+        None
+        """
+
         self.name = name
 
     def set_rec_players(self, rec_players: int):
+        """
+        Sets the recommended amount of players.
+
+        Parameters
+        ----------
+        rec_players : int
+            the recommended amount of players
+
+        Returns
+        -------
+        None
+        """
         self.rec_players = rec_players
 
     def set_rec_tourney(self, rec_tourney):
+        """
+        Sets the recommended tournament type.
+
+        Parameters
+        ----------
+        rec_tourney : Tourney
+            the recommended tournament type
+
+        Returns
+        -------
+        None
+        """
         self.rec_tourney = rec_tourney
 
     def set_labels(self, labels: list[str]):
+        """
+        Sets the labels for additional stat tracking for the game.
+
+        Parameters
+        ----------
+        labels : list of str
+            the labels for additional stat tracking
+
+        Returns
+        -------
+        None
+        """
         self.labels = labels
 
     def get_labels(self):
+        """
+        Gets the labels for the game.
+
+        Parameters
+        ----------
+        None
+
+        Returns
+        -------
+        self.labels : list of str
+            the labels for additional stat tracking
+        """
         return self.labels
 
 
-class FIFA(Game):
-    def __init__(self):
-        self.name = "FIFA"
-        self.rec_players = 8  # useless?
-        self.rec_tourney = "Single_Elimination"
-        self.labels = []
+class Tourney:
+    """
+    A interface-like class to represent a tournament.
 
+    ...
+
+    Attributes
+    ----------
+    game : Game
+        the game the tournament is managing
+    players : list of Player/Team
+        the players or teams that the tournament is managing
+    matchups : dict of {int : dict}
+        the matchups and associated data
+
+    Methods
+    -------
+    add_player(player):
+        adds a player or team to the tournament
+    add_players(players):
+        sets the players or teams of the tournament
+    randomize_matchups():
+        randomizes the order of the players
+    start():
+        starts the tournament by initializing all the matchups
+    input_result():
+        inputs the result of concluded matchup
+    get_matchups():
+        returns the tournament matchups
+    print_matchups():
+        prints the tournament matchups
+    print_results():
+        prints just the concluded tournament matchups
+    """
 
-# interface
-class Tourney:
     def __init__(self, game):
+        """
+        Constructs the attributes of the Tourney class.
+
+        Players and matchups are empty upon construction.
+
+        Parameters
+        ----------
+        game : Game
+            the game the tournament is managing
+        """
+
         self.game = game
         self.players = []
         self.matchups = {}
 
     def add_player(self, player: Player / Team):
+        """
+        Adds a player or team to the tournament.
+
+        Parameters
+        ----------
+        player : Player / Team
+            the player or team to be added
+
+        Returns
+        -------
+        None
+        """
+
         self.players.append(player)
 
     def add_players(self, players: list[Player / Team]):
+        """
+        Sets the players or teams of the tournament.
+
+        Parameters
+        ----------
+        players : list of Player / Team
+            the players or teams to be set in the tournament
+
+        Returns
+        -------
+        None
+        """
+
         self.players = players
 
     def randomize_matchups(self):
+        """
+        Randomizes the order of the players.
+
+        Parameters
+        ----------
+        None
+
+        Returns
+        -------
+        None
+        """
         np.random.shuffle(self.players)
 
-    def start(self, additional_stats=None):
-        """Set all matchups"""
+    def start(self):
+        """
+        Starts the tournament by initializing all the matchups.
+
+        Function specifics differ per tournament subclass.
+
+        Parameters
+        ----------
+        None
+
+        Returns
+        -------
+        None
+        """
         pass  # pragma: no cover
 
     def input_result(self):
+        """
+        Inputs the result of concluded matchup.
+
+        Function specifics differ per tournament subclass.
+
+        Parameters
+        ----------
+        None
+
+        Returns
+        -------
+        None
+        """
+
         pass  # pragma: no cover
 
     def get_matchups(self):
+        """
+        Returns the tournaments matchups.
+
+        Parameters
+        ----------
+        None
+
+        Returns
+        -------
+        self.matchups : dict of {int : dict}
+        """
         return self.matchups
 
     # can take in a round to print the round
     def print_matchups(self):
-        pass  # pragma: no cover
+        """
+        Prints the tournament matchups.
 
-    def print_results(self):
-        pass  # pragma: no cover
+        Function specifics differ per tournament subclass.
 
+        Parameters
+        ----------
+        None
+
+        Returns
+        -------
+        None
+        """
 
-class Single_Elimination(Tourney):
-    # ex matchups 4 person SE {
-    #    1:{Home: "Aaron", Away: "Xandra", Next: 3, Home_Score: 2, Away_Score: 1},
-    #    2:{Home: "Tiffany", Away: "Lucas", Next: 3, Home_Score: 4, Away_Score: 0},
-    #    3:{Home: "Aaron", Away: "Lucas", Next: None, Home_Score: None, Away_Score: None}
-    #   }
-    def start(self):
-        extra_labels = self.game.get_labels()
-        # print("EXTRA LABELS: " + str(extra_labels))
-        # set entire bracket
-        # assume number of participants is a power of 2
-        self.started = True
-        # total_matches = len(self.players) - 1
-        num_rounds = np.ceil(np.log2(len(self.players)))
-        # num_byes = num_rounds**2 - len(self.players)
-        matchup_counter = 1
-        p1 = 0
-        p2 = 1
-        round_matches = len(self.players) // 2  # players power of 2
-        round = 1
-        updating_round_matches = 0
-        while round_matches > 0:
-            updating_round_matches += round_matches
-            for i in range(round_matches):
-                if round == 1:
-                    home, away = self.players[p1].get_name(), self.players[p2].get_name()
-                else:
-                    home, away = None, None
-                if round != num_rounds:
-                    next = updating_round_matches + (i // 2) + 1
-                else:
-                    next = None
-                self.matchups[matchup_counter] = {
-                    "Home": home,
-                    "Away": away,
-                    "Next": next,
-                    "Home_Score": None,
-                    "Away_Score": None,
-                }
-                for stat in extra_labels:
-                    self.matchups[matchup_counter][stat] = None
-                matchup_counter += 1
-                p1 += 2
-                p2 += 2
-            round_matches = round_matches // 2
-            round += 1
-
-    def input_result(self, matchup_id, away_score, home_score, extra_stats=[]):
-        self.matchups[matchup_id]["Home_Score"] = home_score
-        self.matchups[matchup_id]["Away_Score"] = away_score
-        home = self.matchups[matchup_id]["Home"]
-        away = self.matchups[matchup_id]["Away"]
-        if home_score > away_score:
-            winner = home
-        elif away_score > home_score:
-            winner = away
-        else:
-            winner = "Tie"
-            print("This format does not support ties")  # dont let ties be input
-            return False
-        next = self.matchups[matchup_id]["Next"]
-        if next is not None:
-            if matchup_id % 2 == 0:
-                self.matchups[next]["Home"] = winner
-            else:
-                self.matchups[next]["Away"] = winner
-        extra_labels = self.game.get_labels()
-        if len(extra_stats) == len(extra_labels):
-            for i in range(len(extra_stats)):
-                self.matchups[matchup_id][extra_labels[i]] = extra_stats[i]
+        pass  # pragma: no cover
 
-    def print_matchups(self):
-        for i in range(len(self.matchups)):
-            matchup_id = i + 1
-            home = self.matchups[matchup_id]["Home"]
-            away = self.matchups[matchup_id]["Away"]
-            if home is not None and away is not None:
-                print("{:d}: {:s} (A) vs {:s} (H)".format(matchup_id, away, home))
-
-    def print_results(self):  # pragma: no cover
-        for i in range(len(self.matchups)):
-            matchup_id = i + 1
-            home = self.matchups[matchup_id]["Home"]
-            away = self.matchups[matchup_id]["Away"]
-            home_score = self.matchups[matchup_id]["Home_Score"]
-            away_score = self.matchups[matchup_id]["Away_Score"]
-            if home is not None and away is not None and home_score is not None and away_score is not None:
-                print("{:d}: {:s} ({:d}) vs {:s} ({:d})".format(matchup_id, away, away_score, home, home_score))
+    def print_results(self):
+        """
+        Prints just the concluded tournament matchups.
 
+        Function specifics differ per tournament subclass.
 
-# circle algorithm
-class Round_Robin(Tourney):
-    def start(self):
-        extra_labels = self.game.get_labels()
-        self.started = True
-        matchup_counter = 1
-
-        if len(self.players) % 2 == 1:
-            num_players = len(self.players) + 1
-            players = self.players + [Player('dummy')]
-        else:
-            num_players = len(self.players)
-            players = self.players
-        num_rounds = num_players - 1
-        num_matches_per_round = num_players // 2
-
-        # rounds not currently used but could be in the future
-        rounds = []
-        for round_number in range(num_rounds):
-            matches = []
-            for match in range(num_matches_per_round):
-                home = players[match].get_name()
-                away = players[-(match + 1)].get_name()
-                if home != 'dummy' and away != 'dummy':
-                    self.matchups[matchup_counter] = {
-                        "Home": home,
-                        "Away": away,
-                        "Home_Score": None,
-                        "Away_Score": None,
-                    }
-                    for stat in extra_labels:
-                        self.matchups[matchup_counter][stat] = None
-                    matchup_counter += 1
+        Parameters
+        ----------
+        None
+
+        Returns
+        -------
+        None
+        """
+        pass  # pragma: no cover
 
-            rounds.append(matches)
-            players.insert(1, players.pop())
 
-    def print_matchups(self):
-        for i in range(len(self.matchups)):
-            matchup_id = i + 1
-            home = self.matchups[matchup_id]["Home"]
-            away = self.matchups[matchup_id]["Away"]
-            if home is not None and away is not None:
-                print("{:d}: {:s} (A) vs {:s} (H)".format(matchup_id, away, home))
-
-    def print_results(self):  # pragma: no cover
-        for i in range(len(self.matchups)):
-            matchup_id = i + 1
-            home = self.matchups[matchup_id]["Home"]
-            away = self.matchups[matchup_id]["Away"]
-            home_score = self.matchups[matchup_id]["Home_Score"]
-            away_score = self.matchups[matchup_id]["Away_Score"]
-            if home is not None and away is not None and home_score is not None and away_score is not None:
-                print("{:d}: {:s} ({:d}) vs {:s} ({:d})".format(matchup_id, away, away_score, home, home_score))
-
-    def input_result(self, matchup_id, away_score, home_score, extra_stats=[]):
-        self.matchups[matchup_id]["Home_Score"] = home_score
-        self.matchups[matchup_id]["Away_Score"] = away_score
-        extra_labels = self.game.get_labels()
-        if len(extra_stats) == len(extra_labels):
-            for i in range(len(extra_stats)):
-                self.matchups[matchup_id][extra_labels[i]] = extra_stats[i]
+class Player:
+    """
+    A class to represent a player.
 
+    ...
+
+    Attributes
+    ----------
+    name : str
+        the name of the player
+    age : int
+        the age of the player
+
+    Methods
+    -------
+    set_age(age):
+        sets the age of the player
+    get_name():
+        returns the name of the player
+    """
 
-class Player:
     def __init__(self, name):
+        """
+        Constructs the attributes of the Player class.
+        """
+
         self.name = name
         self.age = None
 
-    def set_age(self, age):  # DOB?
+    def set_age(self, age):
+        """
+        Sets the age of the player.
+
+        Parameters
+        ----------
+        age : int
+            the age of the player
+
+        Returns
+        -------
+        None
+        """
+
         self.age = age
 
     def get_name(self):
+        """ "
+        Returns the name of the player.
+
+        Parameters
+        ----------
+        None
+
+        Returns
+        -------
+        self.name : str
+        """
         return self.name
 
 
 class Team:
+    """
+    A class to represent a Team of Players.
+
+    ...
+
+    Attributes
+    ----------
+    name : str
+        the name of the team
+    players : list of Player
+        the players on the team
+
+    Methods
+    -------
+    add_player(player):
+        adds a player to the team
+    add_players(players):
+        sets the players of the team
+    get_name():
+        returns the name of the team
+    get_players():
+        returns the players of the team
+    """
+
     def __init__(self, name: str):
+        """
+        Constructs the attributes of the Team class.
+        """
+
         self.name = name
         self.players = []
 
     def add_player(self, player: Player):
+        """
+        Adds a player to the team.
+
+        Parameters
+        ----------
+        player : Player
+            the player to be added
+
+        Returns
+        -------
+        None
+        """
+
         self.players.append(player)
 
     def add_players(self, players: list[Player]):
+        """
+        Set the players of the team.
+
+        Parameters
+        ----------
+        players : list of Player
+            the players to be set on the team
+
+        Returns
+        -------
+        None
+        """
+
         self.players = players
 
     def get_name(self):
         return self.name
 
     def get_players(self):
         return self.players
 
 
-def example1():
-    MyTourney = Single_Elimination(FIFA())
-    p1 = Player("Aaron")
-    p2 = Player("Xandra")
-    p3 = Player("Lucas")
-    p4 = Player("Tiffany")
-    MyTourney.add_players([p1, p2, p3, p4])
-    MyTourney.randomize_matchups()
-    MyTourney.start()
-    MyTourney.print_matchups()
-    MyTourney.input_result(1, 2, 3)
-    MyTourney.input_result(2, 10, 1)
-    MyTourney.input_result(3, 4, 1)
-    MyTourney.print_results()
+def example1():  # pragma: no cover
+    # MyTourney = Single_Elimination(FIFA())
+    # p1 = Player("Aaron")
+    # p2 = Player("Xandra")
+    # p3 = Player("Lucas")
+    # p4 = Player("Tiffany")
+    # MyTourney.add_players([p1, p2, p3, p4])
+    # MyTourney.randomize_matchups()
+    # MyTourney.start()
+    # MyTourney.print_matchups()
+    # MyTourney.input_result(1, 2, 3)
+    # MyTourney.input_result(2, 10, 1)
+    # MyTourney.input_result(3, 4, 1)
+    # MyTourney.print_results()
+    return 0
```

### Comparing `no-teg-0.2.0/no_teg/tests/test_all.py` & `no-teg-0.2.1/no_teg/tests/test_all.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from no_teg import *
 from unittest.mock import patch
-
+from ..games import fifa
+from ..tourneys import round_robin as rr, single_elimination as se
 
 ### UNIT TESTS ###
 
-TestTourney1 = Single_Elimination(FIFA())
+TestTourney1 = se.Single_Elimination(fifa.FIFA())
 p1 = Player("Aaron")
 p2 = Player("Xandra")
 p3 = Player("Lucas")
 p4 = Player("Tiffany")
 
 
 def test_Player_get_name():
@@ -18,15 +19,15 @@
 
 def test_Player_set_age():
     p1.set_age(22)
     assert p1.age == 22
 
 
 def test_Tourney_add_player():
-    TestTourney2 = Single_Elimination(FIFA())
+    TestTourney2 = se.Single_Elimination(fifa.FIFA())
     p1 = Player("Aaron")
     TestTourney2.add_player(p1)
     assert TestTourney2.players == [p1]
 
 
 def test_Tourney_add_players():
     TestTourney1.add_players([p1, p2, p3, p4])
@@ -50,50 +51,62 @@
             expected * error
         )
     expected = trials / 24  # 4!
     error = 0.2
     assert times_in_order > expected - (expected * error) and times_in_order < expected + (expected * error)
 
 
-TestTourneyOrdered = Single_Elimination(FIFA())
+TestTourneyOrdered = se.Single_Elimination(fifa.FIFA())
 p5 = Player("Aaron")
 p6 = Player("Xandra")
 p7 = Player("Lucas")
 p8 = Player("Tiffany")
 
 
-def test_SE_start():
-    TestTourneyOrdered.add_players([p1, p2, p3, p4])
-    TestTourneyOrdered.start()
-    assert TestTourneyOrdered.matchups[1]["Away"] == "Xandra"
-    assert TestTourneyOrdered.matchups[1]["Home"] == "Aaron"
-    assert TestTourneyOrdered.matchups[1]["Home_Score"] == None
-    assert TestTourneyOrdered.matchups[1]["Away_Score"] == None
-    assert TestTourneyOrdered.matchups[1]["Next"] == 3
-    assert TestTourneyOrdered.matchups[2]["Away"] == "Tiffany"
-    assert TestTourneyOrdered.matchups[2]["Home"] == "Lucas"
-    assert TestTourneyOrdered.matchups[3]["Home"] == None
-    assert TestTourneyOrdered.matchups[3]["Away"] == None
-
-
-def test_SE_get_matchups():
-    assert TestTourneyOrdered.get_matchups() == TestTourneyOrdered.matchups
-
-
-def test_SE_input_result():
-    TestTourneyOrdered.input_result(1, 0, 1)
-    assert TestTourneyOrdered.matchups[1]["Away_Score"] == 0
-    assert TestTourneyOrdered.matchups[1]["Home_Score"] == 1
-    assert TestTourneyOrdered.matchups[3]["Away"] == "Aaron"
-    TestTourneyOrdered.input_result(2, 4, 2)
-    assert TestTourneyOrdered.matchups[2]["Away_Score"] == 4
-    assert TestTourneyOrdered.matchups[2]["Home_Score"] == 2
-    assert TestTourneyOrdered.matchups[3]["Home"] == "Tiffany"
-    assert TestTourneyOrdered.matchups[3]["Next"] == None
-    assert TestTourneyOrdered.input_result(3, 1, 1) == False
+# def test_SE_start():
+#     TestTourneyOrdered.add_players([p1, p2, p3, p4])
+#     TestTourneyOrdered.start()
+#     assert TestTourneyOrdered.matchups[1]["Away"] == "Xandra"
+#     assert TestTourneyOrdered.matchups[1]["Home"] == "Aaron"
+#     assert TestTourneyOrdered.matchups[1]["Home_Score"] == None
+#     assert TestTourneyOrdered.matchups[1]["Away_Score"] == None
+#     assert TestTourneyOrdered.matchups[1]["Next"] == 3
+#     assert TestTourneyOrdered.matchups[2]["Away"] == "Tiffany"
+#     assert TestTourneyOrdered.matchups[2]["Home"] == "Lucas"
+#     assert TestTourneyOrdered.matchups[3]["Home"] == None
+#     assert TestTourneyOrdered.matchups[3]["Away"] == None
+
+
+# def test_SE_get_matchups():
+#     assert TestTourneyOrdered.get_matchups() == TestTourneyOrdered.matchups
+
+
+# def test_SE_input_result():
+#     TestTourneyOrdered.input_result(1, 0, 1, [])
+#     assert TestTourneyOrdered.matchups[1]["Away_Score"] == 0
+#     assert TestTourneyOrdered.matchups[1]["Home_Score"] == 1
+#     assert TestTourneyOrdered.matchups[3]["Away"] == "Aaron"
+#     TestTourneyOrdered.input_result(2, 4, 2, [])
+#     assert TestTourneyOrdered.matchups[2]["Away_Score"] == 4
+#     assert TestTourneyOrdered.matchups[2]["Home_Score"] == 2
+#     assert TestTourneyOrdered.matchups[3]["Home"] == "Tiffany"
+#     assert TestTourneyOrdered.matchups[3]["Next"] == None
+#     assert TestTourneyOrdered.input_result(3, 1, 1, []) == False
+
+
+TourneyByes = se.Single_Elimination(fifa.FIFA())
+
+
+# def test_byes():
+#     TourneyByes.add_players([p1, p2, p3, p4, p5, p6])
+#     assert len(TourneyByes.players) == 6
+#     TourneyByes.start()
+#     assert len(TourneyByes.players) == 8
+#     matchups = TourneyByes.get_matchups()
+#     assert matchups[1]['Home'] == 'Bye'
 
 
 myGame = Game()
 
 
 def test_game():
     assert myGame.name == None
@@ -109,16 +122,16 @@
 
 def test_game_set_rec_players():
     myGame.set_rec_players(2)
     assert myGame.rec_players == 2
 
 
 def test_game_set_rec_tourney():
-    myGame.set_rec_tourney(Single_Elimination)
-    assert myGame.rec_tourney == Single_Elimination
+    myGame.set_rec_tourney(se.Single_Elimination)
+    assert myGame.rec_tourney == se.Single_Elimination
 
 
 def test_game_set_labels():
     myGame.set_labels(["Total Jokers Used"])
     assert myGame.labels == ["Total Jokers Used"]
 
 
@@ -166,15 +179,15 @@
     Team6 = Team("t6")
     Team6.add_players([p11, p12])
     Team7 = Team("t7")
     Team7.add_players([p13, p14])
     Team8 = Team("t8")
     Team8.add_players([p15, p16])
 
-    Tourney2v2 = Single_Elimination(MyGame)
+    Tourney2v2 = se.Single_Elimination(MyGame)
     Tourney2v2.add_players([Team1, Team2, Team3, Team4, Team5, Team6, Team7, Team8])
     Tourney2v2.start()
     assert Tourney2v2.matchups[1]["Home"] == "t1"
     assert Tourney2v2.matchups[1]["Away"] == "t2"
     assert Tourney2v2.matchups[1]["Next"] == 5
     assert Tourney2v2.matchups[1]["Home Fouls"] == None
     Tourney2v2.input_result(1, 21, 14, [2, 4])
@@ -191,65 +204,14 @@
     assert Tourney2v2.matchups[7]["Away"] == "t2"
     assert Tourney2v2.matchups[7]["Next"] == None
     assert Tourney2v2.matchups[6]["Away Fouls"] == 9
     Tourney2v2.input_result(7, 21, 16, [3, 2])
     assert Tourney2v2.matchups[7]["Away_Score"] > Tourney2v2.matchups[7]["Home_Score"]
 
 
-def test_RR_even():
-    p1 = Player("Aaron")
-    p2 = Player("Xandra")
-    p3 = Player("Lucas")
-    p4 = Player("Tiffany")
-    MyGame = Game()
-    TourneyRR = Round_Robin(MyGame)
-    TourneyRR.add_players([p1, p2, p3, p4])
-    TourneyRR.start()
-    matchups = TourneyRR.get_matchups()
-    assert len(matchups) == 6  # summation(num_players - 1) == 6
-    # test everyone has same number of games
-    games = {'Aaron': 0, 'Xandra': 0, 'Lucas': 0, 'Tiffany': 0}
-    for v in matchups.values():
-        games[v['Home']] += 1
-        games[v['Away']] += 1
-    assert games['Aaron'] == 3
-    assert games['Xandra'] == 3
-    assert games['Lucas'] == 3
-    assert games['Tiffany'] == 3
-    TourneyRR.input_result(1, 2, 1)
-    print(matchups)
-    assert matchups[1]["Away_Score"] == 2
-    assert matchups[1]["Home_Score"] == 1
-
-
-def test_RR_odd():
-    p1 = Player("Aaron")
-    p2 = Player("Xandra")
-    p3 = Player("Lucas")
-    p4 = Player("Tiffany")
-    p5 = Player("Rhea")
-    MyGame = Game()
-    TourneyRR = Round_Robin(MyGame)
-    TourneyRR.add_players([p1, p2, p3, p4, p5])
-    TourneyRR.start()
-    matchups = TourneyRR.get_matchups()
-    TourneyRR.print_matchups()
-    assert len(matchups) == 10  # summation(num_players - 1) == 1 + 2 + 3 + 4 == 10
-    # test everyone has same number of games
-    games = {'Aaron': 0, 'Xandra': 0, 'Lucas': 0, 'Tiffany': 0, 'Rhea': 0}
-    for v in matchups.values():
-        games[v['Home']] += 1
-        games[v['Away']] += 1
-    assert games['Aaron'] == 4
-    assert games['Xandra'] == 4
-    assert games['Lucas'] == 4
-    assert games['Tiffany'] == 4
-    assert games['Rhea'] == 4
-
-
 ####Test Classes####
 
 
 class TestPlayer:
     def test_age(self):
         p1 = Player("Aaron")
         p1.set_age(22)
```

### Comparing `no-teg-0.2.0/no_teg.egg-info/PKG-INFO` & `no-teg-0.2.1/no_teg.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: no-teg
-Version: 0.2.0
+Version: 0.2.1
 Summary: A quick and easy tournament manager
 Author-email: Aaron Ashery <aaron.ashery1@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -224,14 +224,15 @@
 A library for running tournaments
 
 ![license](https://img.shields.io/github/license/aaronashery/no-teg)
 ![issues](https://img.shields.io/github/issues/AaronAshery/no-teg)
 [![Build Status](https://github.com/ColumbiaOSS/example-project-python/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/AaronAshery/no-teg/actions?query=workflow%3A%22Build+Status%22)
 [![codecov](https://codecov.io/gh/AaronAshery/no-teg/branch/main/graph/badge.svg)](https://codecov.io/gh/ColumbiaOSS/example-project-python)
 [![PyPI](https://img.shields.io/pypi/v/no-teg)](https://pypi.org/project/no-teg/)
+[![Docs](https://img.shields.io/readthedocs/no-teg.svg)](https://no-teg.readthedocs.io/en/latest/)
 
 ## Overview
 'no-teg' (get-on backwards) is a library for running tournaments. In the beginning it will be simple i.e. setting up and advancing through different tournament styles. Eventually if things go smoothly the library will also compute data on the tournaments and players. Being open-source, I hope that people will add tournament styles and different analysis that are dependent on different games.
 
 ## Install:
 
 `pip install no-teg`
```

### Comparing `no-teg-0.2.0/pyproject.toml` & `no-teg-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 build-backend="setuptools.build_meta"
 
 [project]
 name = "no-teg"
 authors = [{name = "Aaron Ashery", email = "aaron.ashery1@gmail.com"}]
 description="A quick and easy tournament manager"
 readme = "README.md"
-version = "0.2.0"
+version = "0.2.1"
 requires-python = ">=3.7"
 
 dependencies = [
     "numpy",
 ]
 
 classifiers = [
```

