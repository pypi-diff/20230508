# Comparing `tmp/soccer_poisson-0.1.8.tar.gz` & `tmp/soccer_poisson-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/soccer_poisson-0.1.8.tar", last modified: Tue Apr  4 08:36:24 2023, max compression
+gzip compressed data, was "dist/soccer_poisson-0.1.9.tar", last modified: Sun May  7 10:57:49 2023, max compression
```

## Comparing `soccer_poisson-0.1.8.tar` & `soccer_poisson-0.1.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 larslarsson   (501) staff       (20)        0 2023-04-04 08:36:24.000000 soccer_poisson-0.1.8/
--rw-r--r--   0 larslarsson   (501) staff       (20)      486 2023-04-04 08:36:24.000000 soccer_poisson-0.1.8/PKG-INFO
--rw-r--r--   0 larslarsson   (501) staff       (20)       66 2022-02-10 22:12:42.000000 soccer_poisson-0.1.8/README.md
--rw-r--r--   0 larslarsson   (501) staff       (20)       38 2023-04-04 08:36:24.000000 soccer_poisson-0.1.8/setup.cfg
--rw-r--r--   0 larslarsson   (501) staff       (20)      933 2023-04-04 08:36:19.000000 soccer_poisson-0.1.8/setup.py
-drwxr-xr-x   0 larslarsson   (501) staff       (20)        0 2023-04-04 08:36:24.000000 soccer_poisson-0.1.8/soccer_poisson/
--rw-r--r--   0 larslarsson   (501) staff       (20)    29929 2023-04-04 08:35:32.000000 soccer_poisson-0.1.8/soccer_poisson/soccer_pro.py
-drwxr-xr-x   0 larslarsson   (501) staff       (20)        0 2023-04-04 08:36:24.000000 soccer_poisson-0.1.8/soccer_poisson.egg-info/
--rw-r--r--   0 larslarsson   (501) staff       (20)        1 2023-04-04 08:36:24.000000 soccer_poisson-0.1.8/soccer_poisson.egg-info/dependency_links.txt
--rw-r--r--   0 larslarsson   (501) staff       (20)      486 2023-04-04 08:36:24.000000 soccer_poisson-0.1.8/soccer_poisson.egg-info/PKG-INFO
--rw-r--r--   0 larslarsson   (501) staff       (20)      199 2023-04-04 08:36:24.000000 soccer_poisson-0.1.8/soccer_poisson.egg-info/SOURCES.txt
--rw-r--r--   0 larslarsson   (501) staff       (20)       15 2023-04-04 08:36:24.000000 soccer_poisson-0.1.8/soccer_poisson.egg-info/top_level.txt
+drwxr-xr-x   0 larslarsson   (501) staff       (20)        0 2023-05-07 10:57:49.000000 soccer_poisson-0.1.9/
+-rw-r--r--   0 larslarsson   (501) staff       (20)      486 2023-05-07 10:57:49.000000 soccer_poisson-0.1.9/PKG-INFO
+-rw-r--r--   0 larslarsson   (501) staff       (20)       66 2022-02-10 22:12:42.000000 soccer_poisson-0.1.9/README.md
+-rw-r--r--   0 larslarsson   (501) staff       (20)       38 2023-05-07 10:57:49.000000 soccer_poisson-0.1.9/setup.cfg
+-rw-r--r--   0 larslarsson   (501) staff       (20)      933 2023-05-07 10:57:09.000000 soccer_poisson-0.1.9/setup.py
+drwxr-xr-x   0 larslarsson   (501) staff       (20)        0 2023-05-07 10:57:49.000000 soccer_poisson-0.1.9/soccer_poisson/
+-rw-r--r--   0 larslarsson   (501) staff       (20)    30370 2023-05-07 10:56:13.000000 soccer_poisson-0.1.9/soccer_poisson/soccer_pro.py
+drwxr-xr-x   0 larslarsson   (501) staff       (20)        0 2023-05-07 10:57:49.000000 soccer_poisson-0.1.9/soccer_poisson.egg-info/
+-rw-r--r--   0 larslarsson   (501) staff       (20)        1 2023-05-07 10:57:49.000000 soccer_poisson-0.1.9/soccer_poisson.egg-info/dependency_links.txt
+-rw-r--r--   0 larslarsson   (501) staff       (20)      486 2023-05-07 10:57:49.000000 soccer_poisson-0.1.9/soccer_poisson.egg-info/PKG-INFO
+-rw-r--r--   0 larslarsson   (501) staff       (20)      199 2023-05-07 10:57:49.000000 soccer_poisson-0.1.9/soccer_poisson.egg-info/SOURCES.txt
+-rw-r--r--   0 larslarsson   (501) staff       (20)       15 2023-05-07 10:57:49.000000 soccer_poisson-0.1.9/soccer_poisson.egg-info/top_level.txt
```

### Comparing `soccer_poisson-0.1.8/setup.py` & `soccer_poisson-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="soccer_poisson",
-    version="0.1.8",
+    version="0.1.9",
     description="poisson calcs for soccer",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/larssl780/soccer",
     author="larssl780",
     author_email="slick.stash.0m@icloud.com",
     license="MIT",
```

### Comparing `soccer_poisson-0.1.8/soccer_poisson/soccer_pro.py` & `soccer_poisson-0.1.9/soccer_poisson/soccer_pro.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import numpy as np
 from scipy import optimize
 from scipy.stats import skellam
 import pandas as pd
 from thin_wrappers import grid_runner as gr
 from thin_wrappers.utils import find_all_indicies
 import re
+# import pdb
 
 
 def make_pretty(styler, cap=''):
     styler.set_caption(cap)
     # styler.format(precision=3)
     return styler
 
@@ -790,14 +791,21 @@
             self.home_odds, self.draw_odds, self.away_odds)
 
         self.mu1 = mu1
         self.mu2 = mu2
         return probs
 
     @property
+    def inverted_probs(self):
+        out = {}
+        for k, v in self.probs.items():
+            out[-1 * k] = v
+        return out
+
+    @property
     def expected_mov(self):
         # print(self.probs)
         return self.mu1 - self.mu2
 
     def report(self):
         grid = self.grid(apply_max_loss=False)
         grid['fair_odds'] = grid.odds
@@ -813,35 +821,42 @@
                 oppo_fodds.append(np.nan)
                 continue
             oppo_hc = -1 * _tuple.hc
             oppo_hcs.append(oppo_hc)
             oppo_fodds.append(offi)
         grid['opp_odds'] = oppo_fodds
         grid['opp_hc'] = oppo_hcs
+        
         max_loss_prob = self.max_loss_prob * 100
         back_home = grid.query(
             "loss.mul(100) <= @max_loss_prob and fair_odds >1.14", engine='python').copy()
         back_away = grid.query(
             "loss.mul(100) >= (100-@max_loss_prob) and opp_odds > 1.14", engine='python').copy()
         back_away.sort_values(['loss', 'opp_odds'],
                               ascending=[1, 0], inplace=True)
         # pdb.set_trace()
         bets = []
 
         back_home = back_home.iloc[:1]
         for _t in back_home.itertuples():
             raw_odds = np.ceil(_t.fair_odds * 100) / 100
-            bets.append("%.2f @ %.3f (%.2f lp)" %
-                        (_t.hc, raw_odds, 100 * _t.loss))
+
+            # pdb.set_trace()
+            epnl = asian_expected_pnl_clubelo(
+                _t.hc, raw_odds, self.probs) * 1e4
+            bets.append("%.2f @ %.3f (%.2f lp, %.0f ep)" %
+                        (_t.hc, raw_odds, 100 * _t.loss, epnl))
 
             back_away = back_away.iloc[:1]
         for _t in back_away.itertuples():
             raw_odds = np.ceil(_t.opp_odds * 100) / 100
-            bets.append("%.2f @ %.3f (%.2f lp)" %
-                        (_t.opp_hc, raw_odds, 100 * (1 - _t.loss)))
+            epnl = asian_expected_pnl_clubelo(
+                _t.opp_hc, raw_odds, self.inverted_probs) * 1e4
+            bets.append("%.2f @ %.3f (%.2f lp, %.0f ep)" %
+                        (_t.opp_hc, raw_odds, 100 * (1 - _t.loss), epnl))
 
         idx = np.concatenate(
             [np.repeat('H', len(back_home)), np.repeat('A', len(back_away))])
         do_it = pd.DataFrame(bets, columns=['bet'], index=pd.Index(idx))
         ho, do, ao = self.clean_odds
         styler = do_it.style.pipe(make_pretty, 'Bets %s (%.2f-%.2f-%.2f: %.2f)' %
                                   (pd.to_datetime('now').strftime('%H:%M'), ho, do, ao, self.predicted_spread()))
```

