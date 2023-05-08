# Comparing `tmp/khloraascaf-1.6.0.tar.gz` & `tmp/khloraascaf-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "khloraascaf-1.6.0.tar", last modified: Sun May  7 15:16:58 2023, max compression
+gzip compressed data, was "khloraascaf-1.7.0.tar", last modified: Mon May  8 18:23:05 2023, max compression
```

## Comparing `khloraascaf-1.6.0.tar` & `khloraascaf-1.7.0.tar`

### file list

```diff
@@ -1,45 +1,46 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 15:16:58.924577 khloraascaf-1.6.0/
--rw-rw-rw-   0 root         (0) root         (0)    34916 2023-05-07 15:16:39.000000 khloraascaf-1.6.0/LICENCE
--rw-r--r--   0 root         (0) root         (0)    45914 2023-05-07 15:16:58.923661 khloraascaf-1.6.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4534 2023-05-07 15:16:39.000000 khloraascaf-1.6.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1339 2023-05-07 15:16:39.000000 khloraascaf-1.6.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-07 15:16:58.924577 khloraascaf-1.6.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 15:16:58.908993 khloraascaf-1.6.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 15:16:58.916327 khloraascaf-1.6.0/src/khloraascaf/
--rw-rw-rw-   0 root         (0) root         (0)      646 2023-05-07 15:16:39.000000 khloraascaf-1.6.0/src/khloraascaf/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1760 2023-05-07 15:16:39.000000 khloraascaf-1.6.0/src/khloraascaf/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)    12600 2023-05-07 15:16:39.000000 khloraascaf-1.6.0/src/khloraascaf/assembly_graph.py
--rw-rw-rw-   0 root         (0) root         (0)     5619 2023-05-07 15:16:39.000000 khloraascaf-1.6.0/src/khloraascaf/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     5070 2023-05-07 15:16:39.000000 khloraascaf-1.6.0/src/khloraascaf/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 15:16:58.921827 khloraascaf-1.6.0/src/khloraascaf/ilp/
--rw-rw-rw-   0 root         (0) root         (0)      372 2023-05-07 15:16:39.000000 khloraascaf-1.6.0/src/khloraascaf/ilp/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11068 2023-05-07 15:16:39.000000 khloraascaf-1.6.0/src/khloraascaf/ilp/dirf_sets.py
--rw-rw-rw-   0 root         (0) root         (0)    10725 2023-05-07 15:16:39.000000 khloraascaf-1.6.0/src/khloraascaf/ilp/invf_sets.py
--rw-rw-rw-   0 root         (0) root         (0)     4901 2023-05-07 15:16:39.000000 khloraascaf-1.6.0/src/khloraascaf/ilp/pulp_circuit.py
--rw-rw-rw-   0 root         (0) root         (0)     3418 2023-05-07 15:16:39.000000 khloraascaf-1.6.0/src/khloraascaf/ilp/pulp_max_dirf.py
--rw-rw-rw-   0 root         (0) root         (0)     3402 2023-05-07 15:16:39.000000 khloraascaf-1.6.0/src/khloraascaf/ilp/pulp_max_invf.py
--rw-rw-rw-   0 root         (0) root         (0)     3738 2023-05-07 15:16:39.000000 khloraascaf-1.6.0/src/khloraascaf/ilp/pulp_max_presscore.py
--rw-rw-rw-   0 root         (0) root         (0)    12009 2023-05-07 15:16:39.000000 khloraascaf-1.6.0/src/khloraascaf/ilp/pulp_repeated_fragments.py
--rw-rw-rw-   0 root         (0) root         (0)     3027 2023-05-07 15:16:39.000000 khloraascaf-1.6.0/src/khloraascaf/ilp/pulp_to_solver.py
--rw-rw-rw-   0 root         (0) root         (0)    10512 2023-05-07 15:16:39.000000 khloraascaf-1.6.0/src/khloraascaf/ilp/pulp_var_db.py
--rw-rw-rw-   0 root         (0) root         (0)     4402 2023-05-07 15:16:39.000000 khloraascaf-1.6.0/src/khloraascaf/inputs.py
--rw-rw-rw-   0 root         (0) root         (0)     1124 2023-05-07 15:16:39.000000 khloraascaf-1.6.0/src/khloraascaf/lib.py
--rw-rw-rw-   0 root         (0) root         (0)    12867 2023-05-07 15:16:39.000000 khloraascaf-1.6.0/src/khloraascaf/multiplied_doubled_contig_graph.py
--rw-rw-rw-   0 root         (0) root         (0)     8309 2023-05-07 15:16:39.000000 khloraascaf-1.6.0/src/khloraascaf/outputs.py
--rw-rw-rw-   0 root         (0) root         (0)      157 2023-05-07 15:16:39.000000 khloraascaf-1.6.0/src/khloraascaf/py.typed
--rw-rw-rw-   0 root         (0) root         (0)    21836 2023-05-07 15:16:39.000000 khloraascaf-1.6.0/src/khloraascaf/result.py
--rw-rw-rw-   0 root         (0) root         (0)    27071 2023-05-07 15:16:39.000000 khloraascaf-1.6.0/src/khloraascaf/run_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)    21539 2023-05-07 15:16:39.000000 khloraascaf-1.6.0/src/khloraascaf/scaffolding_methods.py
--rw-rw-rw-   0 root         (0) root         (0)     7146 2023-05-07 15:16:39.000000 khloraascaf-1.6.0/src/khloraascaf/utils_debug.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 15:16:58.917244 khloraascaf-1.6.0/src/khloraascaf.egg-info/
--rw-r--r--   0 root         (0) root         (0)    45914 2023-05-07 15:16:58.000000 khloraascaf-1.6.0/src/khloraascaf.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1148 2023-05-07 15:16:58.000000 khloraascaf-1.6.0/src/khloraascaf.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-07 15:16:58.000000 khloraascaf-1.6.0/src/khloraascaf.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       77 2023-05-07 15:16:58.000000 khloraascaf-1.6.0/src/khloraascaf.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-05-07 15:16:58.000000 khloraascaf-1.6.0/src/khloraascaf.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 15:16:58.923661 khloraascaf-1.6.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)    13426 2023-05-07 15:16:39.000000 khloraascaf-1.6.0/tests/test_assembly_graph.py
--rw-rw-rw-   0 root         (0) root         (0)     3038 2023-05-07 15:16:39.000000 khloraascaf-1.6.0/tests/test_exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)       63 2023-05-07 15:16:39.000000 khloraascaf-1.6.0/tests/test_outputs.py
--rw-rw-rw-   0 root         (0) root         (0)    22601 2023-05-07 15:16:39.000000 khloraascaf-1.6.0/tests/test_toy_examples.py
--rw-rw-rw-   0 root         (0) root         (0)     2986 2023-05-07 15:16:39.000000 khloraascaf-1.6.0/tests/test_utils_debug.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 18:23:05.330433 khloraascaf-1.7.0/
+-rw-rw-rw-   0 root         (0) root         (0)    34916 2023-05-08 18:22:40.000000 khloraascaf-1.7.0/LICENCE
+-rw-r--r--   0 root         (0) root         (0)    46361 2023-05-08 18:23:05.329433 khloraascaf-1.7.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4981 2023-05-08 18:22:40.000000 khloraascaf-1.7.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1339 2023-05-08 18:22:40.000000 khloraascaf-1.7.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-08 18:23:05.330433 khloraascaf-1.7.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 18:23:05.312432 khloraascaf-1.7.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 18:23:05.320433 khloraascaf-1.7.0/src/khloraascaf/
+-rw-rw-rw-   0 root         (0) root         (0)     1579 2023-05-08 18:22:40.000000 khloraascaf-1.7.0/src/khloraascaf/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1760 2023-05-08 18:22:40.000000 khloraascaf-1.7.0/src/khloraascaf/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13402 2023-05-08 18:22:40.000000 khloraascaf-1.7.0/src/khloraascaf/assembly_graph.py
+-rw-rw-rw-   0 root         (0) root         (0)     5619 2023-05-08 18:22:40.000000 khloraascaf-1.7.0/src/khloraascaf/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     5600 2023-05-08 18:22:40.000000 khloraascaf-1.7.0/src/khloraascaf/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 18:23:05.326433 khloraascaf-1.7.0/src/khloraascaf/ilp/
+-rw-rw-rw-   0 root         (0) root         (0)      372 2023-05-08 18:22:40.000000 khloraascaf-1.7.0/src/khloraascaf/ilp/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11068 2023-05-08 18:22:40.000000 khloraascaf-1.7.0/src/khloraascaf/ilp/dirf_sets.py
+-rw-rw-rw-   0 root         (0) root         (0)    10725 2023-05-08 18:22:40.000000 khloraascaf-1.7.0/src/khloraascaf/ilp/invf_sets.py
+-rw-rw-rw-   0 root         (0) root         (0)     4901 2023-05-08 18:22:40.000000 khloraascaf-1.7.0/src/khloraascaf/ilp/pulp_circuit.py
+-rw-rw-rw-   0 root         (0) root         (0)     3418 2023-05-08 18:22:40.000000 khloraascaf-1.7.0/src/khloraascaf/ilp/pulp_max_dirf.py
+-rw-rw-rw-   0 root         (0) root         (0)     3402 2023-05-08 18:22:40.000000 khloraascaf-1.7.0/src/khloraascaf/ilp/pulp_max_invf.py
+-rw-rw-rw-   0 root         (0) root         (0)     3738 2023-05-08 18:22:40.000000 khloraascaf-1.7.0/src/khloraascaf/ilp/pulp_max_presscore.py
+-rw-rw-rw-   0 root         (0) root         (0)    12009 2023-05-08 18:22:40.000000 khloraascaf-1.7.0/src/khloraascaf/ilp/pulp_repeated_fragments.py
+-rw-rw-rw-   0 root         (0) root         (0)     3027 2023-05-08 18:22:40.000000 khloraascaf-1.7.0/src/khloraascaf/ilp/pulp_to_solver.py
+-rw-rw-rw-   0 root         (0) root         (0)    10512 2023-05-08 18:22:40.000000 khloraascaf-1.7.0/src/khloraascaf/ilp/pulp_var_db.py
+-rw-rw-rw-   0 root         (0) root         (0)     4402 2023-05-08 18:22:40.000000 khloraascaf-1.7.0/src/khloraascaf/inputs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1124 2023-05-08 18:22:40.000000 khloraascaf-1.7.0/src/khloraascaf/lib.py
+-rw-rw-rw-   0 root         (0) root         (0)    12867 2023-05-08 18:22:40.000000 khloraascaf-1.7.0/src/khloraascaf/multiplied_doubled_contig_graph.py
+-rw-rw-rw-   0 root         (0) root         (0)     8323 2023-05-08 18:22:40.000000 khloraascaf-1.7.0/src/khloraascaf/outputs.py
+-rw-rw-rw-   0 root         (0) root         (0)      157 2023-05-08 18:22:40.000000 khloraascaf-1.7.0/src/khloraascaf/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)    21836 2023-05-08 18:22:40.000000 khloraascaf-1.7.0/src/khloraascaf/result.py
+-rw-rw-rw-   0 root         (0) root         (0)    28116 2023-05-08 18:22:40.000000 khloraascaf-1.7.0/src/khloraascaf/run_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)    21539 2023-05-08 18:22:40.000000 khloraascaf-1.7.0/src/khloraascaf/scaffolding_methods.py
+-rw-rw-rw-   0 root         (0) root         (0)     7160 2023-05-08 18:22:40.000000 khloraascaf-1.7.0/src/khloraascaf/utils_debug.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 18:23:05.322433 khloraascaf-1.7.0/src/khloraascaf.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    46361 2023-05-08 18:23:05.000000 khloraascaf-1.7.0/src/khloraascaf.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1174 2023-05-08 18:23:05.000000 khloraascaf-1.7.0/src/khloraascaf.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-08 18:23:05.000000 khloraascaf-1.7.0/src/khloraascaf.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       77 2023-05-08 18:23:05.000000 khloraascaf-1.7.0/src/khloraascaf.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-05-08 18:23:05.000000 khloraascaf-1.7.0/src/khloraascaf.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 18:23:05.329433 khloraascaf-1.7.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)    13219 2023-05-08 18:22:40.000000 khloraascaf-1.7.0/tests/test_assembly_graph.py
+-rw-rw-rw-   0 root         (0) root         (0)     3186 2023-05-08 18:22:40.000000 khloraascaf-1.7.0/tests/test_exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)       63 2023-05-08 18:22:40.000000 khloraascaf-1.7.0/tests/test_outputs.py
+-rw-rw-rw-   0 root         (0) root         (0)    14876 2023-05-08 18:22:40.000000 khloraascaf-1.7.0/tests/test_run_metdata.py
+-rw-rw-rw-   0 root         (0) root         (0)    22601 2023-05-08 18:22:40.000000 khloraascaf-1.7.0/tests/test_toy_examples.py
+-rw-rw-rw-   0 root         (0) root         (0)     2989 2023-05-08 18:22:40.000000 khloraascaf-1.7.0/tests/test_utils_debug.py
```

### Comparing `khloraascaf-1.6.0/LICENCE` & `khloraascaf-1.7.0/LICENCE`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.6.0/PKG-INFO` & `khloraascaf-1.7.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: khloraascaf
-Version: 1.6.0
+Version: 1.7.0
 Summary: A python package that takes an assembly result of a chloroplast genome and continues it by computing the scaffolding stage.
 Author-email: vepain <victor.epain@laposte.net>
 License: ### GNU GENERAL PUBLIC LICENSE
         
         Version 3, 29 June 2007
         
         Copyright (C) 2007 Free Software Foundation, Inc.
@@ -725,22 +725,20 @@
 
 
 ## Quick usage example
 
 ```python
 from pathlib import Path
 
-from khloraascaf import IR_REGION_ID, SC_REGION_ID, scaffolding
-from khloraascaf.inputs import INSTANCE_NAME_DEF, SOLVER_CBC
-from khloraascaf.outputs import (
-    fmt_contigs_of_regions_filename,
-    fmt_map_of_regions_filename,
-)
-from khloraascaf.run_metadata import IOConfig, MetadataAllSolutions
+from khloraascaf import IOConfig, MetadataAllSolutions, scaffolding
+from khloraascaf.inputs import SOLVER_CBC
 
+# ------------------------------------------------------------------------ #
+# Run the example
+# ------------------------------------------------------------------------ #
 #
 # Prepare the scaffolding result directory
 #
 outdir = Path('scaffolding_result')
 outdir.mkdir(exist_ok=True)
 #
 # Compute the scaffolding using the assembly data
@@ -749,36 +747,47 @@
     Path('tests/data/ir_sc/contig_attrs.tsv'),
     Path('tests/data/ir_sc/contig_links.tsv'),
     'C0',
     solver=SOLVER_CBC,
     outdir=outdir,
 )
 #
-# khloraascaf creates a directory with a single copy name
+# khloraascaf creates a directory with a unique name
 #   to put all the files it has created
 #
 assert outdir_gen in outdir.glob('*')
 print(outdir_gen)
+
+# ------------------------------------------------------------------------ #
+# Dive into the results
+# ------------------------------------------------------------------------ #
+#
+# Use metadata class to easily dive into the results
+# (you can also see by hand the solutions.yaml file that has been produced)
+#
+all_solutions_metadata = MetadataAllSolutions.from_run_directory(outdir_gen)
+#
+# * How many solutions the scaffolding has produced?
+#
+print(len(all_solutions_metadata.solutions()))
+#   = 1, let pick its metadata
+sol_metadata = all_solutions_metadata.solutions()[0]
 #
 # See which files the scaffolding has produced:
 #
 files = set(outdir_gen.glob('*'))
 assert len(files) == 4
 #
 # * The list of oriented contigs for each region
 #
-assert outdir_gen / fmt_contigs_of_regions_filename(
-    INSTANCE_NAME_DEF, [IR_REGION_ID, SC_REGION_ID],
-) in files
+assert outdir_gen / sol_metadata.contigs_of_regions() in files
 #
 # * The list of oriented regions
 #
-assert outdir_gen / fmt_map_of_regions_filename(
-    INSTANCE_NAME_DEF, [IR_REGION_ID, SC_REGION_ID],
-) in files
+assert outdir_gen / sol_metadata.map_of_regions() in files
 #
 # * YAML file containing all the arguments and options you used
 #   to run khloraascaf
 #
 assert outdir_gen / IOConfig.YAML_FILE in files
 #
 # * YAML file that contains metadata on the solutions
```

### Comparing `khloraascaf-1.6.0/README.md` & `khloraascaf-1.7.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -29,22 +29,20 @@
 
 
 ## Quick usage example
 
 ```python
 from pathlib import Path
 
-from khloraascaf import IR_REGION_ID, SC_REGION_ID, scaffolding
-from khloraascaf.inputs import INSTANCE_NAME_DEF, SOLVER_CBC
-from khloraascaf.outputs import (
-    fmt_contigs_of_regions_filename,
-    fmt_map_of_regions_filename,
-)
-from khloraascaf.run_metadata import IOConfig, MetadataAllSolutions
+from khloraascaf import IOConfig, MetadataAllSolutions, scaffolding
+from khloraascaf.inputs import SOLVER_CBC
 
+# ------------------------------------------------------------------------ #
+# Run the example
+# ------------------------------------------------------------------------ #
 #
 # Prepare the scaffolding result directory
 #
 outdir = Path('scaffolding_result')
 outdir.mkdir(exist_ok=True)
 #
 # Compute the scaffolding using the assembly data
@@ -53,36 +51,47 @@
     Path('tests/data/ir_sc/contig_attrs.tsv'),
     Path('tests/data/ir_sc/contig_links.tsv'),
     'C0',
     solver=SOLVER_CBC,
     outdir=outdir,
 )
 #
-# khloraascaf creates a directory with a single copy name
+# khloraascaf creates a directory with a unique name
 #   to put all the files it has created
 #
 assert outdir_gen in outdir.glob('*')
 print(outdir_gen)
+
+# ------------------------------------------------------------------------ #
+# Dive into the results
+# ------------------------------------------------------------------------ #
+#
+# Use metadata class to easily dive into the results
+# (you can also see by hand the solutions.yaml file that has been produced)
+#
+all_solutions_metadata = MetadataAllSolutions.from_run_directory(outdir_gen)
+#
+# * How many solutions the scaffolding has produced?
+#
+print(len(all_solutions_metadata.solutions()))
+#   = 1, let pick its metadata
+sol_metadata = all_solutions_metadata.solutions()[0]
 #
 # See which files the scaffolding has produced:
 #
 files = set(outdir_gen.glob('*'))
 assert len(files) == 4
 #
 # * The list of oriented contigs for each region
 #
-assert outdir_gen / fmt_contigs_of_regions_filename(
-    INSTANCE_NAME_DEF, [IR_REGION_ID, SC_REGION_ID],
-) in files
+assert outdir_gen / sol_metadata.contigs_of_regions() in files
 #
 # * The list of oriented regions
 #
-assert outdir_gen / fmt_map_of_regions_filename(
-    INSTANCE_NAME_DEF, [IR_REGION_ID, SC_REGION_ID],
-) in files
+assert outdir_gen / sol_metadata.map_of_regions() in files
 #
 # * YAML file containing all the arguments and options you used
 #   to run khloraascaf
 #
 assert outdir_gen / IOConfig.YAML_FILE in files
 #
 # * YAML file that contains metadata on the solutions
```

### Comparing `khloraascaf-1.6.0/pyproject.toml` & `khloraascaf-1.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 
 name = "khloraascaf"
-version = "1.6.0"
+version = "1.7.0"
 authors = [{ name = "vepain", email = "victor.epain@laposte.net" }]
 description = "A python package that takes an assembly result of a chloroplast genome and continues it by computing the scaffolding stage."
 keywords = ["Scaffolding", "Chloroplast", "Assembly", "DNA repeats"]
 readme = "README.md"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
```

### Comparing `khloraascaf-1.6.0/src/khloraascaf/__main__.py` & `khloraascaf-1.7.0/src/khloraascaf/__main__.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.6.0/src/khloraascaf/assembly_graph.py` & `khloraascaf-1.7.0/src/khloraascaf/assembly_graph.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # -*- coding=utf-8 -*-
 
 """Module for assembly graph and multiple solution generator."""
 
+from __future__ import annotations
 
 from collections.abc import Iterable, Iterator
 from pathlib import Path
 from queue import LifoQueue
 
 from bitarray import bitarray
 from revsymg.graphs import RevSymGraph
@@ -25,14 +26,15 @@
     ORC_ID_IND,
     ORC_OR_IND,
     ORIENT_INT_STR,
     OrCT,
     read_contigs_of_regions,
     read_map_of_regions,
 )
+from khloraascaf.run_metadata import MetadataSolution
 
 
 # DOCU: all assembly graph
 # DOCU: tuto for assembly graph
 # ============================================================================ #
 #                                   CONSTANTS                                  #
 # ============================================================================ #
@@ -57,29 +59,50 @@
 
 # ============================================================================ #
 #                                     CLASS                                    #
 # ============================================================================ #
 class AssemblyGraph():
     """Khloraascaf assembly graph."""
 
+    @classmethod
+    def from_solution_metadata(
+            cls, solution_metadata: MetadataSolution) -> AssemblyGraph:
+        """Instantiate an AssemblyGraph object from a solution metadata.
+
+        Parameters
+        ----------
+        solution_metadata : MetadataSolution
+            Solution metadata
+
+        Returns
+        -------
+        AssemblyGraph
+            Assembly graph associated to the solution
+        """
+        outdir = solution_metadata.solution_directory()
+        return cls(
+            outdir / solution_metadata.map_of_regions(),
+            outdir / solution_metadata.contigs_of_regions(),
+        )
+
     def __init__(self, map_of_regions_path: Path,
                  contigs_of_regions_path: Path):
         """The Initializer."""
         self.__graph: RevSymGraph = RevSymGraph()
-        self.__regions_contigs: list[list[OrCT]] = []
+        self.__regions_contigs: list[tuple[OrCT, ...]] = []
         self.__region_path_length: int = 0
         self.__read_regions_contigs(contigs_of_regions_path)
         self.__add_regions_links(map_of_regions_path)
 
-    def all_region_paths(self) -> Iterator[list[IndOrT]]:  # noqa
+    def all_region_paths(self) -> Iterator[tuple[IndOrT, ...]]:  # noqa
         """Iterate over all the paths of oriented regions.
 
         Yields
         ------
-        list of IndOrT
+        tuple of IndOrT
             Path of oriented regions
         """
         edges = self.__graph.edges()
 
         used_edges: bitarray = bitarray('0') * (
             edges.biggest_edge_index() + 1)
 
@@ -91,15 +114,15 @@
         # The lifo contains the number of elements to keep to continue
         #   at the next remaning branch (first IndexT value)
         #
         lifo: LifoQueue[tuple[IndexT, IndOrT, IndexT]] = LifoQueue()
 
         for v, e_ind in edges.succs(starter):
             if v[IND] == starter[IND]:
-                yield path
+                yield tuple(path)
             else:
                 lifo.put((1, v, e_ind))
 
         while not lifo.empty():
             _, v, e_ind = lifo.get()
             path.append(v)
             eind_path.append(e_ind)
@@ -111,37 +134,37 @@
                     vw_not_used.append((w, f_ind))
 
             if vw_not_used:
                 for w, f_ind in vw_not_used:
                     lifo.put((len(path), w, f_ind))
             else:
                 if len(path) == self.__region_path_length:
-                    yield path
+                    yield tuple(path)
                 #
                 # Back to the next branching vertex
                 #
                 if not lifo.empty():
                     branch_src_succ_eind = lifo.get()
                     lifo.put(branch_src_succ_eind)
                     for _ in range(len(path) - branch_src_succ_eind[0]):
                         path.pop()
                         used_edges[eind_path.pop()] = False
 
-    def all_oriented_contig_paths(self) -> Iterator[list[OrCT]]:
+    def all_oriented_contig_paths(self) -> Iterator[tuple[OrCT, ...]]:
         """Iterate over all the paths of oriented contigs.
 
         Yields
         ------
-        list of IndOrT
+        tuple of IndOrT
             Path of oriented contigs
         """
         # TODO don't use self method, to avoid verify path validity
         # (because it is known valid)
         for region_path in self.all_region_paths():
-            yield list(self.region_path_to_oriented_contigs(region_path))
+            yield tuple(self.region_path_to_oriented_contigs(region_path))
 
     def region_path_to_oriented_contigs(
             self, region_path: Iterable[IndOrT]) -> Iterator[OrCT]:
         """Iterate over the oriented contigs of a given region path.
 
         Parameters
         ----------
@@ -255,44 +278,44 @@
     """
     return oriented_contig[ORC_ID_IND], ORIENT_REV[oriented_contig[ORC_OR_IND]]
 
 
 # ---------------------------------------------------------------------------- #
 #                               Region Paths File                              #
 # ---------------------------------------------------------------------------- #
-def write_region_paths(region_paths: Iterable[list[IndOrT]],
+def write_region_paths(region_paths: Iterable[Iterable[IndOrT]],
                        region_paths_file: Path):
     """Write the region paths file.
 
     Parameters
     ----------
-    region_paths : iterable of list of IndOrT
+    region_paths : iterable of iterable of IndOrT
         Region paths
     region_paths_file : Path
         Region paths file path
     """
     with open(region_paths_file, 'w', encoding='utf-8') as f_out:
         for region_path in region_paths:
             line: str = ''
             for reg_ind, reg_or in region_path:
                 line += f'{reg_ind}\t{ORIENT_INT_STR[reg_or]}\t'
             f_out.write(line[:-1] + '\n')
 
 
-def read_region_paths(region_paths_file: Path) -> Iterator[list[IndOrT]]:
+def read_region_paths(region_paths_file: Path) -> Iterator[tuple[IndOrT, ...]]:
     """Read region paths from file.
 
     Parameters
     ----------
     region_paths_file : Path
         Region paths file path
 
     Yields
     ------
-    list of IndOrT
+    tuple of IndOrT
         Region path
     """
     with open(region_paths_file, 'r', encoding='utf-8') as regpaths_in:
         for line in regpaths_in:
             region_path = []
             l_regindor = line.split()
             k = 0
@@ -300,15 +323,15 @@
                 region_path.append(
                     (
                         IndexT(l_regindor[k]),
                         STR_ORIENT[l_regindor[k + 1]],  # type: ignore
                     ),
                 )
                 k += 2
-            yield region_path
+            yield tuple(region_path)
 
 
 def fmt_region_paths_filename(instance_name: str,
                               ilp_combination: Iterable[RegionIDT]) -> str:
     """Format the region paths filename.
 
     Parameters
@@ -329,45 +352,45 @@
         f'.{REGION_PATHS_EXT}'
     )
 
 
 # ---------------------------------------------------------------------------- #
 #                          Oriented Contig Paths File                          #
 # ---------------------------------------------------------------------------- #
-def write_oriented_contig_paths(oriented_contig_paths: Iterable[list[OrCT]],
+def write_oriented_contig_paths(oriented_contig_paths: Iterable[Iterable[OrCT]],
                                 oriented_contig_paths_file: Path):
     """Write the oriented contig paths file.
 
     Parameters
     ----------
-    oriented_contig_paths : iterable of list of OrCT
+    oriented_contig_paths : iterable of iterable of OrCT
         Region paths
     oriented_contig_paths_file : Path
         Region paths file path
     """
     with open(oriented_contig_paths_file, 'w', encoding='utf-8') as f_out:
         for oriented_contig_path in oriented_contig_paths:
             line: str = ''
             for c_id, c_or in oriented_contig_path:
                 line += f'{c_id}\t{ORIENT_INT_STR[c_or]}\t'
             f_out.write(line[:-1] + '\n')
 
 
 def read_oriented_contig_paths(oriented_contig_paths_file: Path) -> (
-        Iterator[list[OrCT]]):
+        Iterator[tuple[OrCT, ...]]):
     """Read region paths from file.
 
     Parameters
     ----------
     oriented_contig_paths_file : Path
         Region paths file path
 
     Yields
     ------
-    list of OrCT
+    tuple of OrCT
         Oriented contig path
     """
     with open(oriented_contig_paths_file, 'r', encoding='utf-8') as regpaths_in:
         for line in regpaths_in:
             oriented_contig_path = []
             l_orc = line.split()
             k = 0
@@ -375,15 +398,15 @@
                 oriented_contig_path.append(
                     (
                         l_orc[k],
                         STR_ORIENT[l_orc[k + 1]],  # type: ignore
                     ),
                 )
                 k += 2
-            yield oriented_contig_path
+            yield tuple(oriented_contig_path)
 
 
 def fmt_oriented_contig_paths_filename(
         instance_name: str,
         ilp_combination: Iterable[RegionIDT]) -> str:
     """Format the oriented contig paths filename.
```

### Comparing `khloraascaf-1.6.0/src/khloraascaf/cli.py` & `khloraascaf-1.7.0/src/khloraascaf/cli.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.6.0/src/khloraascaf/exceptions.py` & `khloraascaf-1.7.0/src/khloraascaf/exceptions.py`

 * *Files 8% similar despite different names*

```diff
@@ -163,7 +163,25 @@
 
         Returns
         -------
         str
             Exception message
         """
         return 'The found path is not a circuit'
+
+
+# ---------------------------------------------------------------------------- #
+#                            Run Metadata Exception                            #
+# ---------------------------------------------------------------------------- #
+# TOTEST run metadata exc.
+class NoSolution(Exception):
+    """No solution exception."""
+
+    def __str__(self) -> str:
+        """Print the exception message.
+
+        Returns
+        -------
+        str
+            Exception message
+        """
+        return 'There is no solution'
```

### Comparing `khloraascaf-1.6.0/src/khloraascaf/ilp/dirf_sets.py` & `khloraascaf-1.7.0/src/khloraascaf/ilp/dirf_sets.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.6.0/src/khloraascaf/ilp/invf_sets.py` & `khloraascaf-1.7.0/src/khloraascaf/ilp/invf_sets.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.6.0/src/khloraascaf/ilp/pulp_circuit.py` & `khloraascaf-1.7.0/src/khloraascaf/ilp/pulp_circuit.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.6.0/src/khloraascaf/ilp/pulp_max_dirf.py` & `khloraascaf-1.7.0/src/khloraascaf/ilp/pulp_max_dirf.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.6.0/src/khloraascaf/ilp/pulp_max_invf.py` & `khloraascaf-1.7.0/src/khloraascaf/ilp/pulp_max_invf.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.6.0/src/khloraascaf/ilp/pulp_max_presscore.py` & `khloraascaf-1.7.0/src/khloraascaf/ilp/pulp_max_presscore.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.6.0/src/khloraascaf/ilp/pulp_repeated_fragments.py` & `khloraascaf-1.7.0/src/khloraascaf/ilp/pulp_repeated_fragments.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.6.0/src/khloraascaf/ilp/pulp_to_solver.py` & `khloraascaf-1.7.0/src/khloraascaf/ilp/pulp_to_solver.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.6.0/src/khloraascaf/ilp/pulp_var_db.py` & `khloraascaf-1.7.0/src/khloraascaf/ilp/pulp_var_db.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.6.0/src/khloraascaf/inputs.py` & `khloraascaf-1.7.0/src/khloraascaf/inputs.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.6.0/src/khloraascaf/lib.py` & `khloraascaf-1.7.0/src/khloraascaf/lib.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.6.0/src/khloraascaf/multiplied_doubled_contig_graph.py` & `khloraascaf-1.7.0/src/khloraascaf/multiplied_doubled_contig_graph.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.6.0/src/khloraascaf/outputs.py` & `khloraascaf-1.7.0/src/khloraascaf/outputs.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,38 +133,38 @@
                 else:
                     line += f'\t{occorc[CIND_IND]}'
                 line += f'{ORIENT_INT_STR[occorc[COR_IND]]}\t'
             f_out.write(line[:-1] + '\n')
 
 
 def read_contigs_of_regions(contigs_of_regions_path: Path) -> (
-        Iterator[list[OrCT]]):
+        Iterator[tuple[OrCT, ...]]):
     """Read the regions' contigs file.
 
     Parameters
     ----------
     contigs_of_regions_path : Path
         List of oriented contigs for each region
 
     Yields
     ------
-    list of OrCT
+    tuple of OrCT
         List of oriented contigs for one region
     """
     with open(contigs_of_regions_path, 'r', encoding='utf-8') as cor_in:
         for line in cor_in:
             orc_of_region: list[OrCT] = []
             l_orc = line.split()
             k = 0
             while k < len(l_orc) - 1:
                 orc_of_region.append(
                     (l_orc[k], STR_ORIENT[l_orc[k + 1]]),  # type: ignore
                 )
                 k += 2
-            yield orc_of_region
+            yield tuple(orc_of_region)
 
 
 def fmt_contigs_of_regions_filename(
         instance_name: str, ilp_combination: Iterable[RegionIDT]) -> str:
     """Format the contigs of regions filename.
 
     Parameters
```

### Comparing `khloraascaf-1.6.0/src/khloraascaf/result.py` & `khloraascaf-1.7.0/src/khloraascaf/result.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.6.0/src/khloraascaf/run_metadata.py` & `khloraascaf-1.7.0/src/khloraascaf/run_metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     OPT_INSTANCE_NAME,
     OPT_MULT_UPB,
     OPT_OUTDEBUG,
     OPT_OUTDIR,
     OPT_PRESSCORE_UPB,
     OPT_SOLVER,
 )
+from khloraascaf.exceptions import NoSolution
 from khloraascaf.inputs import STR_ORIENT, IdCT, MultT, PresScoreT
 from khloraascaf.lib import DR_REGION_ID, IR_REGION_ID, RegionIDT
 from khloraascaf.multiplied_doubled_contig_graph import (
     CIND_IND,
     COCC_IND,
     COR_IND,
     OccOrCT,
@@ -274,30 +275,54 @@
 
     YAML_FILE: str = 'solution.yaml'
     """Solution metadata file name."""
 
     KEY_ILP_COMBINATION = 'ilp_combination'
 
     @classmethod
+    def there_is_a_solution(cls, dir_path: Path) -> bool:
+        """Answer "is there a solution in the directory?".
+
+        Parameters
+        ----------
+        dir_path : Path
+            Directory path
+
+        Returns
+        -------
+        bool
+            True if there is a solution, else False
+        """
+        return (dir_path / cls.YAML_FILE).exists()
+
+    @classmethod
     def from_run_directory(cls, yaml_dir: Path) -> MetadataSolution:
         """Intitialise MetadataSolution from the YAML's directory.
 
         Parameters
         ----------
         yaml_dir : Path
             Solution metadata YAML directory
 
         Returns
         -------
         MetadataSolution
             Solution metadata
+
+        Raises
+        ------
+        NoSolution
+            There is no solution
         """
-        with open(yaml_dir / cls.YAML_FILE,
-                  'r', encoding='utf-8') as f_in:
+        if not (yaml_dir / cls.YAML_FILE).exists():
+            raise NoSolution()
+
+        with open(yaml_dir / cls.YAML_FILE, 'r', encoding='utf-8') as f_in:
             sol_dict: dict[str, Any] = yaml.load(f_in, yaml.Loader)
+
         return cls(
             yaml_dir,
             sol_dict[cls.KEY_ILP_COMBINATION],
             Path(sol_dict[CONTIGS_OF_REGIONS_PREFIX]),
             Path(sol_dict[MAP_OF_REGIONS_PREFIX]),
         )
 
@@ -405,29 +430,46 @@
 
     YAML_FILE: str = 'solutions.yaml'
     """All solutions metadata file name."""
 
     KEY_ILP_COMBINATION = 'ilp_combination'
 
     @classmethod
+    def there_is_a_solution(cls, dir_path: Path) -> bool:
+        """Answer "is there a solution in the directory?".
+
+        Parameters
+        ----------
+        dir_path : Path
+            Directory path
+
+        Returns
+        -------
+        bool
+            True if there is a solution, else False
+        """
+        return (dir_path / cls.YAML_FILE).exists()
+
+    @classmethod
     def from_run_directory(cls, yaml_dir: Path) -> MetadataAllSolutions:
         """Intitialise MetadataAllSolutions from the YAML's directory.
 
         Parameters
         ----------
         yaml_dir : Path
             Solution metadata YAML directory
 
         Returns
         -------
         MetadataAllSolutions
             Solutions metadata
         """
-        with open(yaml_dir / cls.YAML_FILE,
-                  'r', encoding='utf-8') as f_in:
+        if not (yaml_dir / cls.YAML_FILE).exists():
+            return cls(yaml_dir, ())
+        with open(yaml_dir / cls.YAML_FILE, 'r', encoding='utf-8') as f_in:
             sol_list: list[dict[str, Any]] = yaml.load(f_in, yaml.Loader)
         return cls(
             yaml_dir,
             (
                 MetadataSolution(
                     yaml_dir, sol_dict[cls.KEY_ILP_COMBINATION],
                     Path(sol_dict[CONTIGS_OF_REGIONS_PREFIX]),
@@ -608,15 +650,15 @@
         self.__opt_value: float | None = opt_value
         self.__vertices_of_regions_path: Path | None = vertices_of_regions_path
         self.__map_of_regions_path: Path | None = map_of_regions_path
         self.__repeat_fragments_path: Path | None = repeat_fragments_path
 
     # ~*~ Getter ~*~
 
-    def run_dir(self) -> Path:
+    def run_directory(self) -> Path:
         """Run directory path.
 
         Returns
         -------
         Path
             Run directory path
         """
```

### Comparing `khloraascaf-1.6.0/src/khloraascaf/scaffolding_methods.py` & `khloraascaf-1.7.0/src/khloraascaf/scaffolding_methods.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.6.0/src/khloraascaf/utils_debug.py` & `khloraascaf-1.7.0/src/khloraascaf/utils_debug.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,25 +71,25 @@
             line: str = ''
             for v_ind, v_or, v_occ in result.region_occorc(region_index):
                 line += f'{v_ind}\t{ORIENT_INT_STR[v_or]}\t{v_occ}\t'
             f_out.write(line[:-1] + '\n')
 
 
 def read_vertices_of_regions(vertices_of_regions_path: Path) -> (
-        Iterator[list[OccOrCT]]):
+        Iterator[tuple[OccOrCT, ...]]):
     """Read the regions' vertices file.
 
     Parameters
     ----------
     vertices_of_regions_path : Path
         Path of the file containing the regions' vertices
 
     Yields
     ------
-    list of OccOrCT
+    tuple of OccOrCT
         List of vertices of one region
     """
     with open(vertices_of_regions_path, 'r', encoding='utf-8') as f_in:
         for line in f_in:
             vertices_of_region: list[OccOrCT] = []
             l_occorcstr = line.split('\t')
             k = 0
@@ -98,15 +98,15 @@
                     (
                         IndexT(l_occorcstr[k]),
                         STR_ORIENT[l_occorcstr[k + 1]],  # type: ignore
                         IndexT(l_occorcstr[k + 2]),
                     ),
                 )
                 k += 3
-            yield vertices_of_region
+            yield tuple(vertices_of_region)
 
 
 def fmt_vertices_of_regions_filename(
         instance_name: str,
         ilp_combination: Iterable[RegionIDT]) -> str:
     """Format the vertices of regions file name.
```

### Comparing `khloraascaf-1.6.0/src/khloraascaf.egg-info/PKG-INFO` & `khloraascaf-1.7.0/src/khloraascaf.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: khloraascaf
-Version: 1.6.0
+Version: 1.7.0
 Summary: A python package that takes an assembly result of a chloroplast genome and continues it by computing the scaffolding stage.
 Author-email: vepain <victor.epain@laposte.net>
 License: ### GNU GENERAL PUBLIC LICENSE
         
         Version 3, 29 June 2007
         
         Copyright (C) 2007 Free Software Foundation, Inc.
@@ -725,22 +725,20 @@
 
 
 ## Quick usage example
 
 ```python
 from pathlib import Path
 
-from khloraascaf import IR_REGION_ID, SC_REGION_ID, scaffolding
-from khloraascaf.inputs import INSTANCE_NAME_DEF, SOLVER_CBC
-from khloraascaf.outputs import (
-    fmt_contigs_of_regions_filename,
-    fmt_map_of_regions_filename,
-)
-from khloraascaf.run_metadata import IOConfig, MetadataAllSolutions
+from khloraascaf import IOConfig, MetadataAllSolutions, scaffolding
+from khloraascaf.inputs import SOLVER_CBC
 
+# ------------------------------------------------------------------------ #
+# Run the example
+# ------------------------------------------------------------------------ #
 #
 # Prepare the scaffolding result directory
 #
 outdir = Path('scaffolding_result')
 outdir.mkdir(exist_ok=True)
 #
 # Compute the scaffolding using the assembly data
@@ -749,36 +747,47 @@
     Path('tests/data/ir_sc/contig_attrs.tsv'),
     Path('tests/data/ir_sc/contig_links.tsv'),
     'C0',
     solver=SOLVER_CBC,
     outdir=outdir,
 )
 #
-# khloraascaf creates a directory with a single copy name
+# khloraascaf creates a directory with a unique name
 #   to put all the files it has created
 #
 assert outdir_gen in outdir.glob('*')
 print(outdir_gen)
+
+# ------------------------------------------------------------------------ #
+# Dive into the results
+# ------------------------------------------------------------------------ #
+#
+# Use metadata class to easily dive into the results
+# (you can also see by hand the solutions.yaml file that has been produced)
+#
+all_solutions_metadata = MetadataAllSolutions.from_run_directory(outdir_gen)
+#
+# * How many solutions the scaffolding has produced?
+#
+print(len(all_solutions_metadata.solutions()))
+#   = 1, let pick its metadata
+sol_metadata = all_solutions_metadata.solutions()[0]
 #
 # See which files the scaffolding has produced:
 #
 files = set(outdir_gen.glob('*'))
 assert len(files) == 4
 #
 # * The list of oriented contigs for each region
 #
-assert outdir_gen / fmt_contigs_of_regions_filename(
-    INSTANCE_NAME_DEF, [IR_REGION_ID, SC_REGION_ID],
-) in files
+assert outdir_gen / sol_metadata.contigs_of_regions() in files
 #
 # * The list of oriented regions
 #
-assert outdir_gen / fmt_map_of_regions_filename(
-    INSTANCE_NAME_DEF, [IR_REGION_ID, SC_REGION_ID],
-) in files
+assert outdir_gen / sol_metadata.map_of_regions() in files
 #
 # * YAML file containing all the arguments and options you used
 #   to run khloraascaf
 #
 assert outdir_gen / IOConfig.YAML_FILE in files
 #
 # * YAML file that contains metadata on the solutions
```

### Comparing `khloraascaf-1.6.0/src/khloraascaf.egg-info/SOURCES.txt` & `khloraascaf-1.7.0/src/khloraascaf.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -29,9 +29,10 @@
 src/khloraascaf/ilp/pulp_max_presscore.py
 src/khloraascaf/ilp/pulp_repeated_fragments.py
 src/khloraascaf/ilp/pulp_to_solver.py
 src/khloraascaf/ilp/pulp_var_db.py
 tests/test_assembly_graph.py
 tests/test_exceptions.py
 tests/test_outputs.py
+tests/test_run_metdata.py
 tests/test_toy_examples.py
 tests/test_utils_debug.py
```

### Comparing `khloraascaf-1.6.0/tests/test_assembly_graph.py` & `khloraascaf-1.7.0/tests/test_assembly_graph.py`

 * *Files 10% similar despite different names*

```diff
@@ -78,18 +78,17 @@
         (
             (0, FORWARD_INT),
             (1, FORWARD_INT),
             (2, REVERSE_INT),
             (1, REVERSE_INT),
         ),
     }
-    asm_graph_paths = [tuple(l) for l in asm_graph.all_region_paths()]
+    asm_graph_paths = tuple(asm_graph.all_region_paths())
     assert len(asm_graph_paths) == len(s_region_paths)
-    for reg_path in asm_graph_paths:
-        assert reg_path in s_region_paths
+    assert set(asm_graph_paths) == s_region_paths
 
 
 def test_all_region_paths_dr_sc():
     """Test all_region_paths method for DR-SC."""
     # TOTEST use fixture for assembly graph
     asm_graph = AssemblyGraph(
         _DR_SC_SOL_REGMAP,
@@ -99,18 +98,17 @@
         (
             (0, FORWARD_INT),
             (1, FORWARD_INT),
             (2, FORWARD_INT),
             (1, FORWARD_INT),
         ),
     }
-    asm_graph_paths = [tuple(l) for l in asm_graph.all_region_paths()]
+    asm_graph_paths = tuple(asm_graph.all_region_paths())
     assert len(asm_graph_paths) == len(s_region_paths)
-    for reg_path in asm_graph_paths:
-        assert reg_path in s_region_paths
+    assert set(asm_graph_paths) == s_region_paths
 
 
 # TOTEST test_all_regions_paths_sc
 def test_all_region_paths_sc():
     """Test all_region_paths method for SC."""
     # TOTEST use fixture for assembly graph
     asm_graph = AssemblyGraph(
@@ -118,18 +116,17 @@
         _SC_SOL_REGCTG,
     )
     s_region_paths: set[tuple[IndOrT, ...]] = {
         (
             (0, FORWARD_INT),
         ),
     }
-    asm_graph_paths = [tuple(l) for l in asm_graph.all_region_paths()]
+    asm_graph_paths = tuple(asm_graph.all_region_paths())
     assert len(asm_graph_paths) == len(s_region_paths)
-    for reg_path in asm_graph_paths:
-        assert reg_path in s_region_paths
+    assert set(asm_graph_paths) == s_region_paths
 
 
 # ---------------------------------------------------------------------------- #
 #                           All_oriented_contig_paths                          #
 # ---------------------------------------------------------------------------- #
 def test_all_oriented_contig_paths_ir_sc():
     """Test all_oriented_contig_paths method for IR-SC."""
@@ -154,21 +151,20 @@
             ('C2', REVERSE_INT),
             ('C3', FORWARD_INT),
             ('C4', FORWARD_INT),
             ('C3', REVERSE_INT),
             ('C2', FORWARD_INT),
         ),
     }
-    asm_graph_paths = [tuple(l) for l in asm_graph.all_oriented_contig_paths()]
+    asm_graph_paths = tuple(asm_graph.all_oriented_contig_paths())
     assert len(asm_graph_paths) == len(s_orc_paths)
-    for reg_path in asm_graph_paths:
-        assert reg_path in s_orc_paths
+    assert set(asm_graph_paths) == s_orc_paths
 
 
-def test_all_oriented_contig_paths_dr():
+def test_all_oriented_contig_paths_dr_sc():
     """Test all_oriented_contig_paths method for DR-SC."""
     # TOTEST use fixture for assembly graph
     asm_graph = AssemblyGraph(
         _DR_SC_SOL_REGMAP,
         _DR_SC_SOL_REGCTG,
     )
     s_orc_paths: set[tuple[OrCT, ...]] = {
@@ -178,18 +174,17 @@
             ('C2', REVERSE_INT),
             ('C3', FORWARD_INT),
             ('C4', FORWARD_INT),
             ('C2', REVERSE_INT),
             ('C3', FORWARD_INT),
         ),
     }
-    asm_graph_paths = [tuple(l) for l in asm_graph.all_oriented_contig_paths()]
+    asm_graph_paths = tuple(asm_graph.all_oriented_contig_paths())
     assert len(asm_graph_paths) == len(s_orc_paths)
-    for reg_path in asm_graph_paths:
-        assert reg_path in s_orc_paths
+    assert set(asm_graph_paths) == s_orc_paths
 
 
 # ---------------------------------------------------------------------------- #
 #                                    Revsymg                                   #
 # ---------------------------------------------------------------------------- #
 def test_getter_revsymg():
     """Test getter revsymg."""
```

### Comparing `khloraascaf-1.6.0/tests/test_exceptions.py` & `khloraascaf-1.7.0/tests/test_exceptions.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 from pathlib import Path
 
 from pulp import LpStatus, LpStatusInfeasible
 
 from khloraascaf.exceptions import (
     CombineScaffoldingError,
+    NoSolution,
     NotACircuit,
     RepeatScaffoldingError,
     ScaffoldingError,
     SingleCopyScaffoldingError,
     UnfeasibleDR,
     UnfeasibleIR,
     UnfeasibleSC,
@@ -101,7 +102,13 @@
     )
 
 
 def test_not_a_circuit():
     """Test NotACircuit exception."""
     exc = NotACircuit()
     assert str(exc) == 'The found path is not a circuit'
+
+
+def test_no_solution():
+    """Test NoSolution exception."""
+    exc = NoSolution()
+    assert str(exc) == 'There is no solution'
```

### Comparing `khloraascaf-1.6.0/tests/test_toy_examples.py` & `khloraascaf-1.7.0/tests/test_toy_examples.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.6.0/tests/test_utils_debug.py` & `khloraascaf-1.7.0/tests/test_utils_debug.py`

 * *Files 12% similar despite different names*

```diff
@@ -43,20 +43,20 @@
 def test_read_vertices_of_regions():
     """Test for read_vertices_of_regions."""
     assert tuple(
         read_vertices_of_regions(
             _VERTICES_OF_REGION_PATH,
         ),
     ) == (
-        [(0, FORWARD_INT, 0), (1, REVERSE_INT, 0)],
-        [(2, FORWARD_INT, 1), (3, REVERSE_INT, 1)],
-        [(4, FORWARD_INT, 0)],
-        [(5, FORWARD_INT, 0), (6, REVERSE_INT, 1), (7, REVERSE_INT, 1)],
-        [(8, REVERSE_INT, 0)],
-        [(9, FORWARD_INT, 0)],
+        ((0, FORWARD_INT, 0), (1, REVERSE_INT, 0)),
+        ((2, FORWARD_INT, 1), (3, REVERSE_INT, 1)),
+        ((4, FORWARD_INT, 0),),
+        ((5, FORWARD_INT, 0), (6, REVERSE_INT, 1), (7, REVERSE_INT, 1)),
+        ((8, REVERSE_INT, 0),),
+        ((9, FORWARD_INT, 0),),
     )
 
 
 def test_fmt_vertices_of_regions_filename():
     """Test for fmt_vertices_of_regions_filename."""
     assert fmt_vertices_of_regions_filename(
         INSTANCE_NAME_DEF, (IR_REGION_ID, DR_REGION_ID, SC_REGION_ID),
```

