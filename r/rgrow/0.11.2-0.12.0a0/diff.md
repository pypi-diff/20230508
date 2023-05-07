# Comparing `tmp/rgrow-0.11.2.tar.gz` & `tmp/rgrow-0.12.0a0.tar.gz`

## Comparing `rgrow-0.11.2.tar` & `rgrow-0.12.0a0.tar`

### file list

```diff
@@ -1,20 +1,105 @@
--rw-r--r--   0        0        0      756 1970-01-01 00:00:00.000000 rgrow-0.11.2/Cargo.toml
--rw-r--r--   0     1000     1000       96 2022-10-29 14:17:16.000000 rgrow-0.11.2/.gitignore
--rw-r--r--   0     1000     1000     1151 2022-08-12 18:13:11.000000 rgrow-0.11.2/.gitlab-ci.yml
--rw-r--r--   0     1000     1000      126 2022-08-12 18:13:11.000000 rgrow-0.11.2/.pre-commit-config.yaml
--rw-r--r--   0     1000     1000       45 2022-11-11 21:09:33.000000 rgrow-0.11.2/.vscode/settings.json
--rw-r--r--   0     1000     1000     1074 2022-08-12 18:13:11.000000 rgrow-0.11.2/LICENSE
--rw-r--r--   0     1000     1000      634 2022-08-12 18:13:11.000000 rgrow-0.11.2/Makefile
--rw-r--r--   0     1000     1000      162 2022-11-12 00:42:53.000000 rgrow-0.11.2/README.md
--rw-r--r--   0     1000     1000     2007 2022-08-12 18:13:11.000000 rgrow-0.11.2/conf.py
--rw-r--r--   0     1000     1000      736 2022-08-12 18:13:11.000000 rgrow-0.11.2/index.rst
--rw-r--r--   0     1000     1000    17490 2022-10-25 17:31:42.000000 rgrow-0.11.2/old/lib_old.rs
--rw-r--r--   0     1000     1000    70410 2022-10-25 17:31:18.000000 rgrow-0.11.2/old/lib_old_2.rs
--rw-r--r--   0     1000     1000    10562 2022-11-11 22:18:46.000000 rgrow-0.11.2/old/utils.py
--rw-r--r--   0     1000     1000      129 2022-11-12 00:33:13.000000 rgrow-0.11.2/pyproject.toml
--rw-r--r--   0     1000     1000       98 2022-10-25 17:45:37.000000 rgrow-0.11.2/rgrow/__init__.py
--rw-r--r--   0     1000     1000        0 2022-11-11 22:09:01.000000 rgrow-0.11.2/rgrow/py.typed
--rw-r--r--   0     1000     1000     4117 2022-11-11 22:04:06.000000 rgrow-0.11.2/rgrow/rgrow.pyi
--rw-r--r--   0     1000     1000      497 2022-11-11 22:08:48.000000 rgrow-0.11.2/src/lib.rs
--rw-r--r--   0     1000     1000    15835 2022-11-11 22:06:20.000000 rgrow-0.11.2/src/tileset.rs
--rw-r--r--   0        0        0      539 1970-01-01 00:00:00.000000 rgrow-0.11.2/PKG-INFO
+-rw-r--r--   0        0        0     1860 1970-01-01 00:00:00.000000 rgrow-0.12.0a0/local_dependencies/rgrow/Cargo.toml
+-rw-r--r--   0     1001      123     3565 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/local_dependencies/rgrow/benches/ratestore.rs
+-rw-r--r--   0     1001      123     1875 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/local_dependencies/rgrow/benches/sierpinski.rs
+-rw-r--r--   0     1001      123      664 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/local_dependencies/rgrow/benches/ui.rs
+-rw-r--r--   0     1001      123     3224 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/local_dependencies/rgrow/examples/barish-perfect-sc.yaml
+-rwxr-xr-x   0     1001      123     5881 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/local_dependencies/rgrow/examples/barish-perfect.yaml
+-rw-r--r--   0     1001      123      150 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/local_dependencies/rgrow/examples/fission-small-ribbon.yaml
+-rw-r--r--   0     1001      123     1718 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/local_dependencies/rgrow/examples/sierpinski.yaml
+-rw-r--r--   0     1001      123      401 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/local_dependencies/rgrow/examples/tube.yaml
+-rwxr-xr-x   0     1001      123      212 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/local_dependencies/rgrow/examples/xgrow-format/1dXOR.tiles
+-rwxr-xr-x   0     1001      123      478 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/local_dependencies/rgrow/examples/xgrow-format/9-square.tiles
+-rwxr-xr-x   0     1001      123      165 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/local_dependencies/rgrow/examples/xgrow-format/AB.tiles
+-rwxr-xr-x   0     1001      123      137 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/local_dependencies/rgrow/examples/xgrow-format/ABdiff.tiles
+-rwxr-xr-x   0     1001      123      554 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/local_dependencies/rgrow/examples/xgrow-format/BarishSeed.tiles
+-rwxr-xr-x   0     1001      123      240 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/local_dependencies/rgrow/examples/xgrow-format/BinaryCounter.tiles
+-rwxr-xr-x   0     1001      123     1357 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/local_dependencies/rgrow/examples/xgrow-format/BinaryCounterSquare.tiles
+-rwxr-xr-x   0     1001      123     2661 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/local_dependencies/rgrow/examples/xgrow-format/BinaryTree.tiles
+-rwxr-xr-x   0     1001      123     3149 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/local_dependencies/rgrow/examples/xgrow-format/BusyBeaver3Square.tiles
+-rwxr-xr-x   0     1001      123      171 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/local_dependencies/rgrow/examples/xgrow-format/COPY.tiles
+-rwxr-xr-x   0     1001      123      215 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/local_dependencies/rgrow/examples/xgrow-format/COPYseed.tiles
+-rwxr-xr-x   0     1001      123      245 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/local_dependencies/rgrow/examples/xgrow-format/CombSquare.tiles
+-rwxr-xr-x   0     1001      123      927 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/local_dependencies/rgrow/examples/xgrow-format/DiamondSet.tiles
+-rwxr-xr-x   0     1001      123      534 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/local_dependencies/rgrow/examples/xgrow-format/DiamondSet_patrick_mullins.tiles
+-rwxr-xr-x   0     1001      123      544 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/local_dependencies/rgrow/examples/xgrow-format/Rule110.tiles
+-rwxr-xr-x   0     1001      123      643 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/local_dependencies/rgrow/examples/xgrow-format/Rule110D.tiles
+-rwxr-xr-x   0     1001      123      674 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/local_dependencies/rgrow/examples/xgrow-format/Rule110Drandom.tiles
+-rwxr-xr-x   0     1001      123      712 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/local_dependencies/rgrow/examples/xgrow-format/Rule110V.tiles
+-rwxr-xr-x   0     1001      123     2686 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/local_dependencies/rgrow/examples/xgrow-format/TwoCounterSquareCapped.tiles
+-rwxr-xr-x   0     1001      123     3177 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/local_dependencies/rgrow/examples/xgrow-format/UL.seed
+-rwxr-xr-x   0     1001      123     3041 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/local_dependencies/rgrow/examples/xgrow-format/ULcounter.seed
+-rwxr-xr-x   0     1001      123      327 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/local_dependencies/rgrow/examples/xgrow-format/UnarySquare.tiles
+-rwxr-xr-x   0     1001      123      535 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/local_dependencies/rgrow/examples/xgrow-format/UnarySquareBig.tiles
+-rwxr-xr-x   0     1001      123      561 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/local_dependencies/rgrow/examples/xgrow-format/XOR.tiles
+-rwxr-xr-x   0     1001      123      801 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/local_dependencies/rgrow/examples/xgrow-format/asyncdemo.tiles
+-rwxr-xr-x   0     1001      123      185 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/local_dependencies/rgrow/examples/xgrow-format/barcode.tiles
+-rwxr-xr-x   0     1001      123      229 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/local_dependencies/rgrow/examples/xgrow-format/barseed.tiles
+-rwxr-xr-x   0     1001      123      528 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/local_dependencies/rgrow/examples/xgrow-format/chunk-test.tiles
+-rwxr-xr-x   0     1001      123     7278 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/local_dependencies/rgrow/examples/xgrow-format/counter2x2indestructible_seed.tiles
+-rwxr-xr-x   0     1001      123     2491 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/local_dependencies/rgrow/examples/xgrow-format/counter3x3heal_perfect.tiles
+-rwxr-xr-x   0     1001      123      852 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/local_dependencies/rgrow/examples/xgrow-format/crosshatch.tiles
+-rwxr-xr-x   0     1001      123      131 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/local_dependencies/rgrow/examples/xgrow-format/diagonal.tiles
+-rwxr-xr-x   0     1001      123      145 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/local_dependencies/rgrow/examples/xgrow-format/linear1.tiles
+-rwxr-xr-x   0     1001      123      187 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/local_dependencies/rgrow/examples/xgrow-format/linear2.tiles
+-rwxr-xr-x   0     1001      123      204 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/local_dependencies/rgrow/examples/xgrow-format/linear3.tiles
+-rwxr-xr-x   0     1001      123      172 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/local_dependencies/rgrow/examples/xgrow-format/lines1.tiles
+-rwxr-xr-x   0     1001      123      184 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/local_dependencies/rgrow/examples/xgrow-format/lines2.tiles
+-rwxr-xr-x   0     1001      123      600 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/local_dependencies/rgrow/examples/xgrow-format/reversibleXOR.tiles
+-rwxr-xr-x   0     1001      123      840 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/local_dependencies/rgrow/examples/xgrow-format/sierpinski.tiles
+-rwxr-xr-x   0     1001      123     1561 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/local_dependencies/rgrow/examples/xgrow-format/sierpinski1x1_wb.tiles
+-rwxr-xr-x   0     1001      123      737 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/local_dependencies/rgrow/examples/xgrow-format/sierpinski2x2.tiles
+-rwxr-xr-x   0     1001      123     6791 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/local_dependencies/rgrow/examples/xgrow-format/sierpinski2x2indestructible_seed.tiles
+-rwxr-xr-x   0     1001      123     2503 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/local_dependencies/rgrow/examples/xgrow-format/sierpinski3x3_wb.tiles
+-rwxr-xr-x   0     1001      123     2491 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/local_dependencies/rgrow/examples/xgrow-format/sierpinski3x3heal_perfect.tiles
+-rwxr-xr-x   0     1001      123      874 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/local_dependencies/rgrow/examples/xgrow-format/sierpinski_diag.tiles
+-rwxr-xr-x   0     1001      123      700 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/local_dependencies/rgrow/examples/xgrow-format/spiral.tiles
+-rw-r--r--   0     1001      123      364 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/local_dependencies/rgrow/examples/xgrow-format/zig-zag-3w.tiles
+-rwxr-xr-x   0     1001      123      614 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/local_dependencies/rgrow/examples/xgrow-format/zig-zag-5w-2.5-4.9.tiles
+-rw-r--r--   0     1001      123     2134 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/local_dependencies/rgrow/src/arcsim.rs
+-rw-r--r--   0     1001      123     1616 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/local_dependencies/rgrow/src/base.rs
+-rw-r--r--   0     1001      123    19255 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/local_dependencies/rgrow/src/canvas.rs
+-rw-r--r--   0     1001      123     4516 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/local_dependencies/rgrow/src/cffi.rs
+-rw-r--r--   0     1001      123    30787 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/local_dependencies/rgrow/src/colors.rs
+-rw-r--r--   0     1001      123    19915 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/local_dependencies/rgrow/src/ffs.rs
+-rw-r--r--   0     1001      123      497 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/local_dependencies/rgrow/src/lib.rs
+-rw-r--r--   0     1001      123     2591 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/local_dependencies/rgrow/src/main.rs
+-rw-r--r--   0     1001      123    30026 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/local_dependencies/rgrow/src/models/atam.rs
+-rw-r--r--   0     1001      123    14351 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/local_dependencies/rgrow/src/models/covers.rs
+-rw-r--r--   0     1001      123    56483 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/local_dependencies/rgrow/src/models/ktam.rs
+-rw-r--r--   0     1001      123    13221 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/local_dependencies/rgrow/src/models/ktam_fission.rs
+-rw-r--r--   0     1001      123      111 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/local_dependencies/rgrow/src/models/mod.rs
+-rw-r--r--   0     1001      123    32018 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/local_dependencies/rgrow/src/models/oldktam.rs
+-rw-r--r--   0     1001      123    12402 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/local_dependencies/rgrow/src/models/oldktam_fission.rs
+-rw-r--r--   0     1001      123    11057 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/local_dependencies/rgrow/src/parser_xgrow.rs
+-rw-r--r--   0     1001      123     7539 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/local_dependencies/rgrow/src/ratestore.rs
+-rw-r--r--   0     1001      123     7226 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/local_dependencies/rgrow/src/simulation.rs
+-rw-r--r--   0     1001      123    10948 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/local_dependencies/rgrow/src/state.rs
+-rw-r--r--   0     1001      123    15647 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/local_dependencies/rgrow/src/system.rs
+-rw-r--r--   0     1001      123    33582 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/local_dependencies/rgrow/src/tileset.rs
+-rw-r--r--   0     1001      123     3760 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/local_dependencies/rgrow/src/ui.rs
+-rw-r--r--   0     1001      123     6376 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/local_dependencies/rgrow/tests/main.rs
+-rw-r--r--   0        0        0      837 1970-01-01 00:00:00.000000 rgrow-0.12.0a0/Cargo.toml
+-rw-r--r--   0     1001      123     1074 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/LICENSE
+-rw-r--r--   0     1001      123      634 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/Makefile
+-rw-r--r--   0     1001      123      162 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/README.md
+-rw-r--r--   0     1001      123     2007 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/conf.py
+-rw-r--r--   0     1001      123       20 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/docs/.gitignore
+-rw-r--r--   0     1001      123      638 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/docs/Makefile
+-rw-r--r--   0     1001      123      491 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/docs/requirements-docs.txt
+-rw-r--r--   0     1001      123     1867 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/docs/source/conf.py
+-rw-r--r--   0     1001      123      498 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/docs/source/index.rst
+-rw-r--r--   0     1001      123      135 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/docs/source/reference/ffs.rst
+-rw-r--r--   0     1001      123      729 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/docs/source/reference/simulation.rst
+-rw-r--r--   0     1001      123      385 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/docs/source/reference/tileset.rst
+-rw-r--r--   0     1001      123      736 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/index.rst
+-rw-r--r--   0     1001      123    17490 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/old/lib_old.rs
+-rw-r--r--   0     1001      123    70410 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/old/lib_old_2.rs
+-rw-r--r--   0     1001      123    10492 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/old/utils.py
+-rw-r--r--   0     1001      123      155 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/pyproject.toml
+-rw-r--r--   0     1001      123      267 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/rgrow/__init__.py
+-rw-r--r--   0     1001      123        0 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/rgrow/py.typed
+-rw-r--r--   0     1001      123     4252 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/rgrow/rgrow.pyi
+-rw-r--r--   0     1001      123      498 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/src/lib.rs
+-rw-r--r--   0     1001      123    28221 2023-05-07 22:56:24.000000 rgrow-0.12.0a0/src/tileset.rs
+-rw-r--r--   0     1001      123    52932 2023-05-07 22:57:47.000000 rgrow-0.12.0a0/Cargo.lock
+-rw-r--r--   0        0        0      560 1970-01-01 00:00:00.000000 rgrow-0.12.0a0/PKG-INFO
```

### Comparing `rgrow-0.11.2/LICENSE` & `rgrow-0.12.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `rgrow-0.11.2/Makefile` & `rgrow-0.12.0a0/Makefile`

 * *Files identical despite different names*

### Comparing `rgrow-0.11.2/conf.py` & `rgrow-0.12.0a0/conf.py`

 * *Files identical despite different names*

### Comparing `rgrow-0.11.2/index.rst` & `rgrow-0.12.0a0/index.rst`

 * *Files identical despite different names*

### Comparing `rgrow-0.11.2/old/lib_old.rs` & `rgrow-0.12.0a0/old/lib_old.rs`

 * *Files identical despite different names*

### Comparing `rgrow-0.11.2/old/lib_old_2.rs` & `rgrow-0.12.0a0/old/lib_old_2.rs`

 * *Files identical despite different names*

### Comparing `rgrow-0.11.2/old/utils.py` & `rgrow-0.12.0a0/old/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 from typing import List, Optional, Tuple, Union, cast, Callable
-from numpy.core.fromnumeric import var
 # import statsmodels
 # import statsmodels.stats.proportion
-from numpy import isin, ndarray
+from numpy import ndarray
 import numpy as np
 import pandas as pd
 import rgrow.rgrow as rg
-import dataclasses
 import multiprocessing
 import multiprocessing.pool
 from . import rgrow
 
 
 def _ffs_extract_trajectories(backlist: List[List[int]]) -> ndarray:
     ntraj = len(backlist[-1])
@@ -95,15 +93,15 @@
 
     def seeds_of_trajectories(self, ts: rgrow.TileSet,
                               pool: Optional[multiprocessing.pool.Pool]
                               = None, proppool=False, ci_width=0.1,
                               min=0.4, max=0.6, ci_pct=0.95, max_events=10_000_000) -> pd.DataFrame:
         trajs = self.trajectory_configs
 
-        sim = ts.to_simulation()
+        ts.to_simulation()
 
         if proppool or (pool is None):
             seeds = []
             seedinfos = []
             for i, trajectory in enumerate(trajs):
                 seed, seedinfo = trajectory_seed(system, trajectory, ci_width,
                                                  min, max, ci_pct, max_events, pool)
```

### Comparing `rgrow-0.11.2/rgrow/rgrow.pyi` & `rgrow-0.12.0a0/rgrow/rgrow.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 import numpy as np
 
+class EvolveOutcome(object):
+    ...
+
 class FFSLevel(object):
     @property
     def configs(self) -> list[np.ndarray]:
         """List of configurations at this level, as arrays (not full states)."""
         ...
     @property
     def previous_indices(self) -> list[int]:
@@ -19,15 +22,15 @@
         total_events: int | None = None,
         for_time: float | None = None,
         total_time: float | None = None,
         size_min: float | None = None,
         size_max: float | None = None,
         for_wall_time: float | None = None,
         require_strong_bound: bool = True
-    ) -> None: 
+    ) -> EvolveOutcome: 
         """Evolve a particular state, with index `state_index`,
         subject to some bounds.  Runs state 0 by default.
 
         By default, this requires a strong bound (the simulation
         will eventually end, eg, not a size or other potentially
         unreachable bound).
         
@@ -41,15 +44,15 @@
         total_events: int | None = None,
         for_time: float | None = None,
         total_time: float | None = None,
         size_min: float | None = None,
         size_max: float | None = None,
         for_wall_time: float | None = None,
         require_strong_bound: bool = True
-    ):
+    ) -> list[EvolveOutcome]:
         """Evolve *all* states, stopping each as they reach the
         boundary conditions.  Runs multithreaded using available
         cores.  Runs state 0 by default.
         """
         ...
 
     def canvas_copy(
@@ -131,7 +134,13 @@
         surface_init_size: int = 3,
         max_init_events: int = 10_000,
         max_subseq_events: int = 1_000_000,
         max_init_time: float | None = None,
         max_subseq_time: float | None = None,
         keep_surface_configs: bool = False,
     ) -> FFSResult: ...
+
+class Tile(object):
+    ...
+
+class FFSRunConfig(object):
+    ...
```

### Comparing `rgrow-0.11.2/PKG-INFO` & `rgrow-0.12.0a0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: rgrow
-Version: 0.11.2
+Version: 0.12.0a0
 Requires-Dist: numpy
 License-File: LICENSE
 Summary: Python interface to rgrow.
-Author: Constantine Evans <cevans@costi.eu>
-Author-email: Constantine Evans <cevans@costi.eu>
+Author: Constantine Evans <const@costi.eu>
+Author-email: Constantine Evans <const@costi.eu>
 License: BSD-3-Clause
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Project-URL: Source Code, https://github.com/evansfmm/pyrgrow
+Project-URL: Source Code, https://github.com/evansfmm/rgrow
 
 Rgrow is a tile assembly model simulator, primarily built as a fast
 implementation of kinetic models, inspired by Xgrow; this is the
 Python interface for rgrow.
```

