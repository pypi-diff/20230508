# Comparing `tmp/pineappl-0.6.0a8.tar.gz` & `tmp/pineappl-0.6.0a9.tar.gz`

## Comparing `pineappl-0.6.0a8.tar` & `pineappl-0.6.0a9.tar`

### file list

```diff
@@ -1,59 +1,59 @@
--rw-r--r--   0        0        0      714 1970-01-01 00:00:00.000000 pineappl-0.6.0a8/local_dependencies/pineappl/Cargo.toml
--rw-r--r--   0     1001      123      594 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/local_dependencies/pineappl/README.md
--rw-r--r--   0     1001      123    37886 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/local_dependencies/pineappl/src/bin.rs
--rw-r--r--   0     1001      123      256 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/local_dependencies/pineappl/src/convert.rs
--rw-r--r--   0     1001      123     2962 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/local_dependencies/pineappl/src/empty_subgrid.rs
--rw-r--r--   0     1001      123    22471 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/local_dependencies/pineappl/src/evolution.rs
--rw-r--r--   0     1001      123    15042 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/local_dependencies/pineappl/src/fk_table.rs
--rw-r--r--   0     1001      123    96582 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/local_dependencies/pineappl/src/grid.rs
--rw-r--r--   0     1001      123    25442 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/local_dependencies/pineappl/src/import_only_subgrid.rs
--rw-r--r--   0     1001      123    43946 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/local_dependencies/pineappl/src/lagrange_subgrid.rs
--rw-r--r--   0     1001      123      471 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/local_dependencies/pineappl/src/lib.rs
--rw-r--r--   0     1001      123    16120 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/local_dependencies/pineappl/src/lumi.rs
--rw-r--r--   0     1001      123     4853 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/local_dependencies/pineappl/src/ntuple_subgrid.rs
--rw-r--r--   0     1001      123     7912 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/local_dependencies/pineappl/src/pids.rs
--rw-r--r--   0     1001      123    36204 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/local_dependencies/pineappl/src/sparse_array3.rs
--rw-r--r--   0     1001      123    10342 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/local_dependencies/pineappl/src/subgrid.rs
--rw-r--r--   0     1001      123    16425 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/local_dependencies/pineappl/tests/drell_yan_lo.rs
--rw-r--r--   0        0        0      786 1970-01-01 00:00:00.000000 pineappl-0.6.0a8/Cargo.toml
--rw-r--r--   0     1001      123      352 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/.gitignore
--rw-r--r--   0     1001      123      783 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/README.md
--rw-r--r--   0     1001      123      235 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/docs/.gitignore
--rw-r--r--   0     1001      123      876 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/docs/Makefile
--rw-r--r--   0     1001      123      804 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/docs/make.bat
--rw-r--r--   0     1001      123        0 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/docs/source/_static/.gitkeep
--rw-r--r--   0     1001      123     6097 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/docs/source/conf.py
--rw-r--r--   0     1001      123      886 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/docs/source/implementation.rst
--rw-r--r--   0     1001      123     1295 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/docs/source/index.rst
--rw-r--r--   0     1001      123       91 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/docs/source/indices.rst
--rw-r--r--   0     1001      123     1148 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/docs/source/installation.rst
--rw-r--r--   0     1001      123     2534 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/docs/source/recipes.rst
--rw-r--r--   0     1001      123        0 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/docs/source/refs.bib
--rw-r--r--   0     1001      123      951 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/docs/source/shared/roles.rst
--rw-r--r--   0     1001      123      893 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/package/Containerfile
--rw-r--r--   0     1001      123     3584 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/package/README.md
--rwxr-xr-x   0     1001      123      219 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/package/maturin
--rw-r--r--   0     1001      123      115 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/pineappl/__init__.py
--rw-r--r--   0     1001      123      516 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/pineappl/bin.py
--rw-r--r--   0     1001      123     1688 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/pineappl/fk_table.py
--rw-r--r--   0     1001      123    12505 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/pineappl/grid.py
--rw-r--r--   0     1001      123      762 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/pineappl/import_only_subgrid.py
--rw-r--r--   0     1001      123      379 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/pineappl/lumi.py
--rw-r--r--   0     1001      123      254 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/pineappl/subgrid.py
--rw-r--r--   0     1001      123      430 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/pineappl/utils.py
--rw-r--r--   0     1001      123     1141 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/pyproject.toml
--rw-r--r--   0     1001      123      674 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/src/bin.rs
--rw-r--r--   0     1001      123     1078 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/src/evolution.rs
--rw-r--r--   0     1001      123     6438 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/src/fk_table.rs
--rw-r--r--   0     1001      123    22338 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/src/grid.rs
--rw-r--r--   0     1001      123     1799 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/src/import_only_subgrid.rs
--rw-r--r--   0     1001      123      874 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/src/lib.rs
--rw-r--r--   0     1001      123     1109 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/src/lumi.rs
--rw-r--r--   0     1001      123     4261 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/src/subgrid.rs
--rw-r--r--   0     1001      123      324 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/tests/conftest.py
--rw-r--r--   0     1001      123      355 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/tests/test_bin.py
--rw-r--r--   0     1001      123     6124 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/tests/test_grid.py
--rw-r--r--   0     1001      123      237 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/tests/test_lumi.py
--rw-r--r--   0     1001      123      868 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/tests/test_sugrid.py
--rw-r--r--   0     1001      123    44398 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/Cargo.lock
--rw-r--r--   0        0        0     2373 1970-01-01 00:00:00.000000 pineappl-0.6.0a8/PKG-INFO
+-rw-r--r--   0        0        0      714 1970-01-01 00:00:00.000000 pineappl-0.6.0a9/local_dependencies/pineappl/Cargo.toml
+-rw-r--r--   0     1001      123      594 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/local_dependencies/pineappl/README.md
+-rw-r--r--   0     1001      123    37886 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/local_dependencies/pineappl/src/bin.rs
+-rw-r--r--   0     1001      123      256 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/local_dependencies/pineappl/src/convert.rs
+-rw-r--r--   0     1001      123     2962 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/local_dependencies/pineappl/src/empty_subgrid.rs
+-rw-r--r--   0     1001      123    22471 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/local_dependencies/pineappl/src/evolution.rs
+-rw-r--r--   0     1001      123    15042 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/local_dependencies/pineappl/src/fk_table.rs
+-rw-r--r--   0     1001      123    96582 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/local_dependencies/pineappl/src/grid.rs
+-rw-r--r--   0     1001      123    25442 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/local_dependencies/pineappl/src/import_only_subgrid.rs
+-rw-r--r--   0     1001      123    43946 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/local_dependencies/pineappl/src/lagrange_subgrid.rs
+-rw-r--r--   0     1001      123      471 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/local_dependencies/pineappl/src/lib.rs
+-rw-r--r--   0     1001      123    16120 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/local_dependencies/pineappl/src/lumi.rs
+-rw-r--r--   0     1001      123     4853 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/local_dependencies/pineappl/src/ntuple_subgrid.rs
+-rw-r--r--   0     1001      123    17098 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/local_dependencies/pineappl/src/pids.rs
+-rw-r--r--   0     1001      123    36204 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/local_dependencies/pineappl/src/sparse_array3.rs
+-rw-r--r--   0     1001      123    10342 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/local_dependencies/pineappl/src/subgrid.rs
+-rw-r--r--   0     1001      123    16425 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/local_dependencies/pineappl/tests/drell_yan_lo.rs
+-rw-r--r--   0        0        0      786 1970-01-01 00:00:00.000000 pineappl-0.6.0a9/Cargo.toml
+-rw-r--r--   0     1001      123      352 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/.gitignore
+-rw-r--r--   0     1001      123      783 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/README.md
+-rw-r--r--   0     1001      123      235 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/docs/.gitignore
+-rw-r--r--   0     1001      123      876 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/docs/Makefile
+-rw-r--r--   0     1001      123      804 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/docs/make.bat
+-rw-r--r--   0     1001      123        0 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/docs/source/_static/.gitkeep
+-rw-r--r--   0     1001      123     6097 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/docs/source/conf.py
+-rw-r--r--   0     1001      123      886 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/docs/source/implementation.rst
+-rw-r--r--   0     1001      123     1295 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/docs/source/index.rst
+-rw-r--r--   0     1001      123       91 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/docs/source/indices.rst
+-rw-r--r--   0     1001      123     1148 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/docs/source/installation.rst
+-rw-r--r--   0     1001      123     2534 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/docs/source/recipes.rst
+-rw-r--r--   0     1001      123        0 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/docs/source/refs.bib
+-rw-r--r--   0     1001      123      951 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/docs/source/shared/roles.rst
+-rw-r--r--   0     1001      123      893 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/package/Containerfile
+-rw-r--r--   0     1001      123     3584 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/package/README.md
+-rwxr-xr-x   0     1001      123      219 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/package/maturin
+-rw-r--r--   0     1001      123      115 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/pineappl/__init__.py
+-rw-r--r--   0     1001      123      516 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/pineappl/bin.py
+-rw-r--r--   0     1001      123     1688 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/pineappl/fk_table.py
+-rw-r--r--   0     1001      123    12585 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/pineappl/grid.py
+-rw-r--r--   0     1001      123      762 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/pineappl/import_only_subgrid.py
+-rw-r--r--   0     1001      123      379 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/pineappl/lumi.py
+-rw-r--r--   0     1001      123      254 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/pineappl/subgrid.py
+-rw-r--r--   0     1001      123      430 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/pineappl/utils.py
+-rw-r--r--   0     1001      123     1141 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/pyproject.toml
+-rw-r--r--   0     1001      123      674 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/src/bin.rs
+-rw-r--r--   0     1001      123     1078 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/src/evolution.rs
+-rw-r--r--   0     1001      123     6438 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/src/fk_table.rs
+-rw-r--r--   0     1001      123    22338 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/src/grid.rs
+-rw-r--r--   0     1001      123     1799 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/src/import_only_subgrid.rs
+-rw-r--r--   0     1001      123      874 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/src/lib.rs
+-rw-r--r--   0     1001      123     1109 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/src/lumi.rs
+-rw-r--r--   0     1001      123     4261 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/src/subgrid.rs
+-rw-r--r--   0     1001      123      324 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/tests/conftest.py
+-rw-r--r--   0     1001      123      355 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/tests/test_bin.py
+-rw-r--r--   0     1001      123     6124 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/tests/test_grid.py
+-rw-r--r--   0     1001      123      237 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/tests/test_lumi.py
+-rw-r--r--   0     1001      123      868 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/tests/test_sugrid.py
+-rw-r--r--   0     1001      123    44640 2023-04-25 14:33:15.000000 pineappl-0.6.0a9/Cargo.lock
+-rw-r--r--   0        0        0     2373 1970-01-01 00:00:00.000000 pineappl-0.6.0a9/PKG-INFO
```

### Comparing `pineappl-0.6.0a8/local_dependencies/pineappl/Cargo.toml` & `pineappl-0.6.0a9/local_dependencies/pineappl/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 categories= ["science"]
 edition= "2021"
 keywords= ["high-energy-physics", "physics"]
 license= "GPL-3.0-or-later"
 repository= "https://github.com/NNPDF/pineappl"
 rust-version= "1.64.0"
-version= "0.6.0-alpha.8"
+version= "0.6.0-alpha.9"
 
 [dependencies]
 arrayvec = "0.7.2"
 bincode = "1.3.3"
 enum_dispatch = "0.3.7"
 float-cmp = "0.9.0"
 git-version = "0.3.5"
```

### Comparing `pineappl-0.6.0a8/local_dependencies/pineappl/README.md` & `pineappl-0.6.0a9/local_dependencies/pineappl/README.md`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a8/local_dependencies/pineappl/src/bin.rs` & `pineappl-0.6.0a9/local_dependencies/pineappl/src/bin.rs`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a8/local_dependencies/pineappl/src/empty_subgrid.rs` & `pineappl-0.6.0a9/local_dependencies/pineappl/src/empty_subgrid.rs`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a8/local_dependencies/pineappl/src/evolution.rs` & `pineappl-0.6.0a9/local_dependencies/pineappl/src/evolution.rs`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a8/local_dependencies/pineappl/src/fk_table.rs` & `pineappl-0.6.0a9/local_dependencies/pineappl/src/fk_table.rs`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a8/local_dependencies/pineappl/src/grid.rs` & `pineappl-0.6.0a9/local_dependencies/pineappl/src/grid.rs`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a8/local_dependencies/pineappl/src/import_only_subgrid.rs` & `pineappl-0.6.0a9/local_dependencies/pineappl/src/import_only_subgrid.rs`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a8/local_dependencies/pineappl/src/lagrange_subgrid.rs` & `pineappl-0.6.0a9/local_dependencies/pineappl/src/lagrange_subgrid.rs`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a8/local_dependencies/pineappl/src/lumi.rs` & `pineappl-0.6.0a9/local_dependencies/pineappl/src/lumi.rs`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a8/local_dependencies/pineappl/src/ntuple_subgrid.rs` & `pineappl-0.6.0a9/local_dependencies/pineappl/src/ntuple_subgrid.rs`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a8/local_dependencies/pineappl/src/sparse_array3.rs` & `pineappl-0.6.0a9/local_dependencies/pineappl/src/sparse_array3.rs`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a8/local_dependencies/pineappl/src/subgrid.rs` & `pineappl-0.6.0a9/local_dependencies/pineappl/src/subgrid.rs`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a8/local_dependencies/pineappl/tests/drell_yan_lo.rs` & `pineappl-0.6.0a9/local_dependencies/pineappl/tests/drell_yan_lo.rs`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a8/Cargo.toml` & `pineappl-0.6.0a9/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -10,22 +10,22 @@
 
 categories= ["science"]
 edition= "2021"
 keywords= ["high-energy-physics", "physics"]
 license= "GPL-3.0-or-later"
 repository= "https://github.com/NNPDF/pineappl"
 rust-version= "1.64.0"
-version= "0.6.0-alpha.8"
+version= "0.6.0-alpha.9"
 
 [package.metadata.maturin]
 name = "pineappl"
 
 [lib]
 name = "pineappl"
 crate-type = ["cdylib"]
 
 [dependencies]
 itertools = "0.10.1"
 ndarray = "0.15.4"
 numpy = "0.16.2"
-pineappl = { path = "local_dependencies/pineappl", version = "0.6.0-alpha.8" }
+pineappl = { path = "local_dependencies/pineappl", version = "0.6.0-alpha.9" }
 pyo3 = { features = ["extension-module"], version = "0.16.4" }
```

### Comparing `pineappl-0.6.0a8/README.md` & `pineappl-0.6.0a9/README.md`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a8/docs/Makefile` & `pineappl-0.6.0a9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a8/docs/make.bat` & `pineappl-0.6.0a9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a8/docs/source/conf.py` & `pineappl-0.6.0a9/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a8/docs/source/implementation.rst` & `pineappl-0.6.0a9/docs/source/implementation.rst`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a8/docs/source/index.rst` & `pineappl-0.6.0a9/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a8/docs/source/installation.rst` & `pineappl-0.6.0a9/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a8/docs/source/recipes.rst` & `pineappl-0.6.0a9/docs/source/recipes.rst`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a8/docs/source/shared/roles.rst` & `pineappl-0.6.0a9/docs/source/shared/roles.rst`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a8/package/Containerfile` & `pineappl-0.6.0a9/package/Containerfile`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a8/package/README.md` & `pineappl-0.6.0a9/package/README.md`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a8/pineappl/bin.py` & `pineappl-0.6.0a9/pineappl/bin.py`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a8/pineappl/fk_table.py` & `pineappl-0.6.0a9/pineappl/fk_table.py`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a8/pineappl/grid.py` & `pineappl-0.6.0a9/pineappl/grid.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,35 +21,37 @@
             power of :math:`\log(\xi_f)`
     """
 
     def __init__(self, alphas, alpha, logxir, logxif):
         self._raw = PyOrder(alphas, alpha, logxir, logxif)
 
     @staticmethod
-    def create_mask(orders, max_as, max_al):
+    def create_mask(orders, max_as, max_al, logs):
         r"""
         Return a mask suitable to pass as the `order_mask` parameter of
         :meth:`Grid.convolute`.
 
         Parameters
         ----------
         orders : list(Order)
             list of available orders
         max_as : int
             maximum power of :math:`\alpha_s`
         max_al : int
             maximum power of :math:`\alpha`
+        logs : bool
+            whether to include log grids or not
 
         Returns
         -------
         list(bool)
             boolean mask
 
         """
-        return PyOrder.create_mask([o._raw for o in orders], max_as, max_al)
+        return PyOrder.create_mask([o._raw for o in orders], max_as, max_al, logs)
 
 
 class Grid(PyWrapper):
     r"""
     Python wrapper object to interface :class:`~pineappl.pineappl.PyGrid`.
 
     To create an object, you should call either :meth:`create`
```

### Comparing `pineappl-0.6.0a8/pineappl/import_only_subgrid.py` & `pineappl-0.6.0a9/pineappl/import_only_subgrid.py`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a8/pyproject.toml` & `pineappl-0.6.0a9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a8/src/bin.rs` & `pineappl-0.6.0a9/src/bin.rs`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a8/src/evolution.rs` & `pineappl-0.6.0a9/src/evolution.rs`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a8/src/fk_table.rs` & `pineappl-0.6.0a9/src/fk_table.rs`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a8/src/grid.rs` & `pineappl-0.6.0a9/src/grid.rs`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a8/src/import_only_subgrid.rs` & `pineappl-0.6.0a9/src/import_only_subgrid.rs`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a8/src/lib.rs` & `pineappl-0.6.0a9/src/lib.rs`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a8/src/lumi.rs` & `pineappl-0.6.0a9/src/lumi.rs`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a8/src/subgrid.rs` & `pineappl-0.6.0a9/src/subgrid.rs`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a8/tests/test_grid.py` & `pineappl-0.6.0a9/tests/test_grid.py`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a8/tests/test_sugrid.py` & `pineappl-0.6.0a9/tests/test_sugrid.py`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a8/Cargo.lock` & `pineappl-0.6.0a9/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -100,14 +100,20 @@
 [[package]]
 name = "autocfg"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
 
 [[package]]
+name = "base64"
+version = "0.21.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a4a4ddaa51a5bc52a6948f74c06d20aaaddb71924eab79b8c97a8c556e942d6a"
+
+[[package]]
 name = "bincode"
 version = "1.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b1f45e9417d87227c7a56d22e471c6206462cba514c7590c09aff4cf6d1ddcad"
 dependencies = [
  "serde",
 ]
@@ -405,14 +411,17 @@
 checksum = "fea41bba32d969b513997752735605054bc0dfa92b4c56bf1189f2e174be7a10"
 
 [[package]]
 name = "either"
 version = "1.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "90e5c1c8368803113bf0c9584fc495a58b86dc8a29edbf8fe877d21d9507e797"
+dependencies = [
+ "serde",
+]
 
 [[package]]
 name = "encode_unicode"
 version = "0.3.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a357d28ed41a50f9c765dbfe56cbc04a64e53e5fc58ba79fbc34c10ef3df831f"
 
@@ -971,15 +980,15 @@
  "once_cell",
  "pest",
  "sha1",
 ]
 
 [[package]]
 name = "pineappl"
-version = "0.6.0-alpha.8"
+version = "0.6.0-alpha.9"
 dependencies = [
  "anyhow",
  "arrayvec",
  "bincode",
  "enum_dispatch",
  "float-cmp",
  "git-version",
@@ -995,39 +1004,41 @@
  "serde",
  "serde_yaml",
  "thiserror",
 ]
 
 [[package]]
 name = "pineappl_applgrid"
-version = "0.6.0-alpha.8"
+version = "0.6.0-alpha.9"
 dependencies = [
  "cc",
  "cxx",
  "cxx-build",
 ]
 
 [[package]]
 name = "pineappl_capi"
-version = "0.6.0-alpha.8"
+version = "0.6.0-alpha.9"
 dependencies = [
  "itertools",
  "pineappl",
 ]
 
 [[package]]
 name = "pineappl_cli"
-version = "0.6.0-alpha.8"
+version = "0.6.0-alpha.9"
 dependencies = [
  "anyhow",
  "assert_cmd",
  "assert_fs",
+ "base64",
  "clap",
  "clap_mangen",
  "cxx",
+ "either",
  "enum_dispatch",
  "flate2",
  "float-cmp",
  "git-version",
  "itertools",
  "lhapdf",
  "libc",
@@ -1043,23 +1054,23 @@
  "serde",
  "serde_yaml",
  "tar",
 ]
 
 [[package]]
 name = "pineappl_fastnlo"
-version = "0.6.0-alpha.8"
+version = "0.6.0-alpha.9"
 dependencies = [
  "cxx",
  "cxx-build",
 ]
 
 [[package]]
 name = "pineappl_py"
-version = "0.6.0-alpha.8"
+version = "0.6.0-alpha.9"
 dependencies = [
  "itertools",
  "ndarray",
  "numpy",
  "pineappl",
  "pyo3",
 ]
```

### Comparing `pineappl-0.6.0a8/PKG-INFO` & `pineappl-0.6.0a9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 Metadata-Version: 2.1
 Name: pineappl
-Version: 0.6.0a8
+Version: 0.6.0a9
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Rust
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Dist: numpy>=1.16.0,<2.0.0
-Requires-Dist: pytest; extra == 'test'
-Requires-Dist: pytest-cov; extra == 'test'
 Requires-Dist: sphinx; extra == 'docs'
 Requires-Dist: sphinx_rtd_theme; extra == 'docs'
 Requires-Dist: sphinxcontrib-bibtex; extra == 'docs'
 Requires-Dist: nbsphinx; extra == 'docs'
-Provides-Extra: test
+Requires-Dist: pytest; extra == 'test'
+Requires-Dist: pytest-cov; extra == 'test'
 Provides-Extra: docs
+Provides-Extra: test
 Summary: Python bindings to PineAPPL
 Keywords: high-energy-physics,physics
 Author: Christopher Schwan <handgranaten-herbert@posteo.de>, Alessandro Candido <candido.ale@gmail.com>, Felix Hekhorn <felix.hekhorn@mi.infn.it>
 Author-email: Christopher Schwan <handgranaten-herbert@posteo.de>, Alessandro Candido <candido.ale@gmail.com>, Felix Hekhorn <felix.hekhorn@mi.infn.it>
 License: GPL-3.0-or-later
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
+Project-URL: changelog, https://github.com/NNPDF/pineappl/blob/master/CHANGELOG.md
 Project-URL: documentation, https://pineappl.readthedocs.io/
 Project-URL: homepage, https://n3pdf.github.io/pineappl/
-Project-URL: changelog, https://github.com/NNPDF/pineappl/blob/master/CHANGELOG.md
 
 [![PyPI version](https://badge.fury.io/py/pineappl.svg)](https://badge.fury.io/py/pineappl)
 [![Anaconda-Server Badge](https://anaconda.org/conda-forge/pineappl/badges/installer/conda.svg)](https://anaconda.org/conda-forge/pineappl)
 [![AUR](https://img.shields.io/aur/version/pineappl)](https://aur.archlinux.org/packages/pineappl)
 [![Documentation Status](https://readthedocs.org/projects/pineappl/badge/?version=latest)](https://pineappl.readthedocs.io/en/latest/?badge=latest)
 
 # Python bindings for PineAPPL
```

