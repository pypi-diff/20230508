# Comparing `tmp/libsa4py-0.3.0.tar.gz` & `tmp/libsa4py-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libsa4py-0.3.0.tar", last modified: Thu Feb 17 09:38:27 2022, max compression
+gzip compressed data, was "libsa4py-0.4.0.tar", last modified: Mon May  8 11:46:43 2023, max compression
```

## Comparing `libsa4py-0.3.0.tar` & `libsa4py-0.4.0.tar`

### file list

```diff
@@ -1,86 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-17 09:38:27.222192 libsa4py-0.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-17 09:38:27.210192 libsa4py-0.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-17 09:38:27.214192 libsa4py-0.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      651 2022-02-17 09:38:15.000000 libsa4py-0.3.0/.github/workflows/libsa4py_test.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      702 2022-02-17 09:38:15.000000 libsa4py-0.3.0/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-02-17 09:38:15.000000 libsa4py-0.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     4882 2022-02-17 09:38:15.000000 libsa4py-0.3.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)     4797 2022-02-17 09:38:15.000000 libsa4py-0.3.0/JSONOutput.md
--rw-r--r--   0 runner    (1001) docker     (121)    11356 2022-02-17 09:38:15.000000 libsa4py-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3948 2022-02-17 09:38:27.218192 libsa4py-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2957 2022-02-17 09:38:15.000000 libsa4py-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-17 09:38:27.214192 libsa4py-0.3.0/libsa4py/
--rw-r--r--   0 runner    (1001) docker     (121)     4270 2022-02-17 09:38:15.000000 libsa4py-0.3.0/libsa4py/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3319 2022-02-17 09:38:15.000000 libsa4py-0.3.0/libsa4py/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2702 2022-02-17 09:38:15.000000 libsa4py-0.3.0/libsa4py/cst_extractor.py
--rw-r--r--   0 runner    (1001) docker     (121)     3678 2022-02-17 09:38:15.000000 libsa4py-0.3.0/libsa4py/cst_lenient_parser.py
--rw-r--r--   0 runner    (1001) docker     (121)    14428 2022-02-17 09:38:15.000000 libsa4py-0.3.0/libsa4py/cst_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (121)    48728 2022-02-17 09:38:15.000000 libsa4py-0.3.0/libsa4py/cst_transformers.py
--rw-r--r--   0 runner    (1001) docker     (121)    34279 2022-02-17 09:38:15.000000 libsa4py-0.3.0/libsa4py/cst_visitor.py
--rw-r--r--   0 runner    (1001) docker     (121)      991 2022-02-17 09:38:15.000000 libsa4py-0.3.0/libsa4py/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)      370 2022-02-17 09:38:15.000000 libsa4py-0.3.0/libsa4py/helper.py
--rw-r--r--   0 runner    (1001) docker     (121)     7476 2022-02-17 09:38:15.000000 libsa4py-0.3.0/libsa4py/merge.py
--rw-r--r--   0 runner    (1001) docker     (121)     9206 2022-02-17 09:38:15.000000 libsa4py-0.3.0/libsa4py/nl_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (121)     2411 2022-02-17 09:38:15.000000 libsa4py-0.3.0/libsa4py/pyre.py
--rw-r--r--   0 runner    (1001) docker     (121)     9284 2022-02-17 09:38:15.000000 libsa4py-0.3.0/libsa4py/representations.py
--rw-r--r--   0 runner    (1001) docker     (121)     2289 2022-02-17 09:38:15.000000 libsa4py-0.3.0/libsa4py/tc_errcodes.toml
--rw-r--r--   0 runner    (1001) docker     (121)     5698 2022-02-17 09:38:15.000000 libsa4py-0.3.0/libsa4py/type_check.py
--rw-r--r--   0 runner    (1001) docker     (121)     3174 2022-02-17 09:38:15.000000 libsa4py-0.3.0/libsa4py/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-17 09:38:27.214192 libsa4py-0.3.0/libsa4py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3948 2022-02-17 09:38:26.000000 libsa4py-0.3.0/libsa4py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2119 2022-02-17 09:38:27.000000 libsa4py-0.3.0/libsa4py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-17 09:38:26.000000 libsa4py-0.3.0/libsa4py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       52 2022-02-17 09:38:27.000000 libsa4py-0.3.0/libsa4py.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       85 2022-02-17 09:38:27.000000 libsa4py-0.3.0/libsa4py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-02-17 09:38:27.000000 libsa4py-0.3.0/libsa4py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       92 2022-02-17 09:38:15.000000 libsa4py-0.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-17 09:38:27.222192 libsa4py-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1584 2022-02-17 09:38:15.000000 libsa4py-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-17 09:38:27.218192 libsa4py-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-17 09:38:15.000000 libsa4py-0.3.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      291 2022-02-17 09:38:15.000000 libsa4py-0.3.0/tests/constans.py
--rw-r--r--   0 runner    (1001) docker     (121)     6170 2022-02-17 09:38:15.000000 libsa4py-0.3.0/tests/example.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-17 09:38:27.218192 libsa4py-0.3.0/tests/examples/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-17 09:38:15.000000 libsa4py-0.3.0/tests/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1062 2022-02-17 09:38:15.000000 libsa4py-0.3.0/tests/examples/assignments.py
--rw-r--r--   0 runner    (1001) docker     (121)      423 2022-02-17 09:38:15.000000 libsa4py-0.3.0/tests/examples/comment_removal.py
--rw-r--r--   0 runner    (1001) docker     (121)     1510 2022-02-17 09:38:15.000000 libsa4py-0.3.0/tests/examples/different_fns.py
--rw-r--r--   0 runner    (1001) docker     (121)     1513 2022-02-17 09:38:15.000000 libsa4py-0.3.0/tests/examples/docstrings.py
--rw-r--r--   0 runner    (1001) docker     (121)      254 2022-02-17 09:38:15.000000 libsa4py-0.3.0/tests/examples/imports.py
--rw-r--r--   0 runner    (1001) docker     (121)      116 2022-02-17 09:38:15.000000 libsa4py-0.3.0/tests/examples/num_removal.py
--rw-r--r--   0 runner    (1001) docker     (121)     1384 2022-02-17 09:38:15.000000 libsa4py-0.3.0/tests/examples/qualified_types.py
--rw-r--r--   0 runner    (1001) docker     (121)      611 2022-02-17 09:38:15.000000 libsa4py-0.3.0/tests/examples/representations.py
--rw-r--r--   0 runner    (1001) docker     (121)     1064 2022-02-17 09:38:15.000000 libsa4py-0.3.0/tests/examples/space_tokens.py
--rw-r--r--   0 runner    (1001) docker     (121)      561 2022-02-17 09:38:15.000000 libsa4py-0.3.0/tests/examples/string_removal.py
--rw-r--r--   0 runner    (1001) docker     (121)      363 2022-02-17 09:38:15.000000 libsa4py-0.3.0/tests/examples/type_annot_count.py
--rw-r--r--   0 runner    (1001) docker     (121)      295 2022-02-17 09:38:15.000000 libsa4py-0.3.0/tests/examples/type_annot_removal.py
--rw-r--r--   0 runner    (1001) docker     (121)    13831 2022-02-17 09:38:15.000000 libsa4py-0.3.0/tests/examples/type_apply_ex.json
--rw-r--r--   0 runner    (1001) docker     (121)      508 2022-02-17 09:38:15.000000 libsa4py-0.3.0/tests/examples/types_prop.py
--rw-r--r--   0 runner    (1001) docker     (121)     2422 2022-02-17 09:38:15.000000 libsa4py-0.3.0/tests/examples/vars_args_occur.py
--rw-r--r--   0 runner    (1001) docker     (121)      476 2022-02-17 09:38:15.000000 libsa4py-0.3.0/tests/examples/vars_types_pyre.py
--rw-r--r--   0 runner    (1001) docker     (121)     9343 2022-02-17 09:38:15.000000 libsa4py-0.3.0/tests/examples/vars_types_pyre_data.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-17 09:38:27.218192 libsa4py-0.3.0/tests/exp_outputs/
--rw-r--r--   0 runner    (1001) docker     (121)     1299 2022-02-17 09:38:15.000000 libsa4py-0.3.0/tests/exp_outputs/added_space.py
--rw-r--r--   0 runner    (1001) docker     (121)    10136 2022-02-17 09:38:15.000000 libsa4py-0.3.0/tests/exp_outputs/extractor_out.json
--rw-r--r--   0 runner    (1001) docker     (121)     9223 2022-02-17 09:38:15.000000 libsa4py-0.3.0/tests/exp_outputs/extractor_out_wo_seq2seq.json
--rw-r--r--   0 runner    (1001) docker     (121)      585 2022-02-17 09:38:15.000000 libsa4py-0.3.0/tests/exp_outputs/normalized_mod_code.txt
--rw-r--r--   0 runner    (1001) docker     (121)      515 2022-02-17 09:38:15.000000 libsa4py-0.3.0/tests/exp_outputs/propagated_types.py
--rw-r--r--   0 runner    (1001) docker     (121)      241 2022-02-17 09:38:15.000000 libsa4py-0.3.0/tests/exp_outputs/removed_com_docs.py
--rw-r--r--   0 runner    (1001) docker     (121)      166 2022-02-17 09:38:15.000000 libsa4py-0.3.0/tests/exp_outputs/removed_num.py
--rw-r--r--   0 runner    (1001) docker     (121)       90 2022-02-17 09:38:15.000000 libsa4py-0.3.0/tests/exp_outputs/removed_str.py
--rw-r--r--   0 runner    (1001) docker     (121)      247 2022-02-17 09:38:15.000000 libsa4py-0.3.0/tests/exp_outputs/removed_type_annot.py
--rw-r--r--   0 runner    (1001) docker     (121)   208584 2022-02-17 09:38:15.000000 libsa4py-0.3.0/tests/exp_outputs/testsexamples.json
--rw-r--r--   0 runner    (1001) docker     (121)   231129 2022-02-17 09:38:15.000000 libsa4py-0.3.0/tests/exp_outputs/testsexamples_nonlp.json
--rw-r--r--   0 runner    (1001) docker     (121)     1954 2022-02-17 09:38:15.000000 libsa4py-0.3.0/tests/test_assignments.py
--rw-r--r--   0 runner    (1001) docker     (121)     5698 2022-02-17 09:38:15.000000 libsa4py-0.3.0/tests/test_cst_transformers.py
--rw-r--r--   0 runner    (1001) docker     (121)     8426 2022-02-17 09:38:15.000000 libsa4py-0.3.0/tests/test_different_fns.py
--rw-r--r--   0 runner    (1001) docker     (121)     3745 2022-02-17 09:38:15.000000 libsa4py-0.3.0/tests/test_docstrings.py
--rw-r--r--   0 runner    (1001) docker     (121)     4288 2022-02-17 09:38:15.000000 libsa4py-0.3.0/tests/test_extractor.py
--rw-r--r--   0 runner    (1001) docker     (121)      729 2022-02-17 09:38:15.000000 libsa4py-0.3.0/tests/test_helper.py
--rw-r--r--   0 runner    (1001) docker     (121)     1532 2022-02-17 09:38:15.000000 libsa4py-0.3.0/tests/test_imports.py
--rw-r--r--   0 runner    (1001) docker     (121)     1679 2022-02-17 09:38:15.000000 libsa4py-0.3.0/tests/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (121)     2746 2022-02-17 09:38:15.000000 libsa4py-0.3.0/tests/test_qualified_types_.py
--rw-r--r--   0 runner    (1001) docker     (121)    14838 2022-02-17 09:38:15.000000 libsa4py-0.3.0/tests/test_representations.py
--rw-r--r--   0 runner    (1001) docker     (121)     3425 2022-02-17 09:38:15.000000 libsa4py-0.3.0/tests/test_type_apply.py
--rw-r--r--   0 runner    (1001) docker     (121)     3586 2022-02-17 09:38:15.000000 libsa4py-0.3.0/tests/test_vars_args_occur.py
--rw-r--r--   0 runner    (1001) docker     (121)      676 2022-02-17 09:38:15.000000 libsa4py-0.3.0/tests/test_visitors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:46:43.342716 libsa4py-0.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:46:43.330716 libsa4py-0.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:46:43.334715 libsa4py-0.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-08 11:46:37.000000 libsa4py-0.4.0/.github/workflows/libsa4py_test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-08 11:46:37.000000 libsa4py-0.4.0/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-08 11:46:37.000000 libsa4py-0.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     5138 2023-05-08 11:46:37.000000 libsa4py-0.4.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-05-08 11:46:37.000000 libsa4py-0.4.0/JSONOutput.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-05-08 11:46:37.000000 libsa4py-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4058 2023-05-08 11:46:43.342716 libsa4py-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-05-08 11:46:37.000000 libsa4py-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:46:43.334715 libsa4py-0.4.0/libsa4py/
+-rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-05-08 11:46:37.000000 libsa4py-0.4.0/libsa4py/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-05-08 11:46:37.000000 libsa4py-0.4.0/libsa4py/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-05-08 11:46:37.000000 libsa4py-0.4.0/libsa4py/cst_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-05-08 11:46:37.000000 libsa4py-0.4.0/libsa4py/cst_lenient_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14428 2023-05-08 11:46:37.000000 libsa4py-0.4.0/libsa4py/cst_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48770 2023-05-08 11:46:37.000000 libsa4py-0.4.0/libsa4py/cst_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34558 2023-05-08 11:46:37.000000 libsa4py-0.4.0/libsa4py/cst_visitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-05-08 11:46:37.000000 libsa4py-0.4.0/libsa4py/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-08 11:46:37.000000 libsa4py-0.4.0/libsa4py/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7476 2023-05-08 11:46:37.000000 libsa4py-0.4.0/libsa4py/merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9206 2023-05-08 11:46:37.000000 libsa4py-0.4.0/libsa4py/nl_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-05-08 11:46:37.000000 libsa4py-0.4.0/libsa4py/pyre.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9284 2023-05-08 11:46:37.000000 libsa4py-0.4.0/libsa4py/representations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-05-08 11:46:37.000000 libsa4py-0.4.0/libsa4py/tc_errcodes.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     5698 2023-05-08 11:46:37.000000 libsa4py-0.4.0/libsa4py/type_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-05-08 11:46:37.000000 libsa4py-0.4.0/libsa4py/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:46:43.334715 libsa4py-0.4.0/libsa4py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4058 2023-05-08 11:46:43.000000 libsa4py-0.4.0/libsa4py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-05-08 11:46:43.000000 libsa4py-0.4.0/libsa4py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 11:46:43.000000 libsa4py-0.4.0/libsa4py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-08 11:46:43.000000 libsa4py-0.4.0/libsa4py.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-08 11:46:43.000000 libsa4py-0.4.0/libsa4py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-08 11:46:43.000000 libsa4py-0.4.0/libsa4py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-08 11:46:37.000000 libsa4py-0.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 11:46:43.342716 libsa4py-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-05-08 11:46:37.000000 libsa4py-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:46:43.338716 libsa4py-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:46:37.000000 libsa4py-0.4.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-05-08 11:46:37.000000 libsa4py-0.4.0/tests/constans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6170 2023-05-08 11:46:37.000000 libsa4py-0.4.0/tests/example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:46:43.338716 libsa4py-0.4.0/tests/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:46:37.000000 libsa4py-0.4.0/tests/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-08 11:46:37.000000 libsa4py-0.4.0/tests/examples/assignments.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-08 11:46:37.000000 libsa4py-0.4.0/tests/examples/comment_removal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-08 11:46:37.000000 libsa4py-0.4.0/tests/examples/different_fns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-05-08 11:46:37.000000 libsa4py-0.4.0/tests/examples/docstrings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-08 11:46:37.000000 libsa4py-0.4.0/tests/examples/imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-08 11:46:37.000000 libsa4py-0.4.0/tests/examples/no_typeslots.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-08 11:46:37.000000 libsa4py-0.4.0/tests/examples/num_removal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-05-08 11:46:37.000000 libsa4py-0.4.0/tests/examples/qualified_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-08 11:46:37.000000 libsa4py-0.4.0/tests/examples/representations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-08 11:46:37.000000 libsa4py-0.4.0/tests/examples/space_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-08 11:46:37.000000 libsa4py-0.4.0/tests/examples/string_removal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-08 11:46:37.000000 libsa4py-0.4.0/tests/examples/type_annot_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-08 11:46:37.000000 libsa4py-0.4.0/tests/examples/type_annot_removal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13831 2023-05-08 11:46:37.000000 libsa4py-0.4.0/tests/examples/type_apply_ex.json
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-08 11:46:37.000000 libsa4py-0.4.0/tests/examples/types_prop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-05-08 11:46:37.000000 libsa4py-0.4.0/tests/examples/vars_args_occur.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-08 11:46:37.000000 libsa4py-0.4.0/tests/examples/vars_types_pyre.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9343 2023-05-08 11:46:37.000000 libsa4py-0.4.0/tests/examples/vars_types_pyre_data.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:46:43.342716 libsa4py-0.4.0/tests/exp_outputs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-05-08 11:46:37.000000 libsa4py-0.4.0/tests/exp_outputs/added_space.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10136 2023-05-08 11:46:37.000000 libsa4py-0.4.0/tests/exp_outputs/extractor_out.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9223 2023-05-08 11:46:37.000000 libsa4py-0.4.0/tests/exp_outputs/extractor_out_wo_seq2seq.json
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-08 11:46:37.000000 libsa4py-0.4.0/tests/exp_outputs/normalized_mod_code.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-08 11:46:37.000000 libsa4py-0.4.0/tests/exp_outputs/propagated_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-08 11:46:37.000000 libsa4py-0.4.0/tests/exp_outputs/removed_com_docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-08 11:46:37.000000 libsa4py-0.4.0/tests/exp_outputs/removed_num.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-08 11:46:37.000000 libsa4py-0.4.0/tests/exp_outputs/removed_str.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-08 11:46:37.000000 libsa4py-0.4.0/tests/exp_outputs/removed_type_annot.py
+-rw-r--r--   0 runner    (1001) docker     (123)   209492 2023-05-08 11:46:37.000000 libsa4py-0.4.0/tests/exp_outputs/testsexamples.json
+-rw-r--r--   0 runner    (1001) docker     (123)   232041 2023-05-08 11:46:37.000000 libsa4py-0.4.0/tests/exp_outputs/testsexamples_nonlp.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-05-08 11:46:37.000000 libsa4py-0.4.0/tests/test_assignments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5698 2023-05-08 11:46:37.000000 libsa4py-0.4.0/tests/test_cst_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8426 2023-05-08 11:46:37.000000 libsa4py-0.4.0/tests/test_different_fns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3745 2023-05-08 11:46:37.000000 libsa4py-0.4.0/tests/test_docstrings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4881 2023-05-08 11:46:37.000000 libsa4py-0.4.0/tests/test_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-08 11:46:37.000000 libsa4py-0.4.0/tests/test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-05-08 11:46:37.000000 libsa4py-0.4.0/tests/test_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-05-08 11:46:37.000000 libsa4py-0.4.0/tests/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-05-08 11:46:37.000000 libsa4py-0.4.0/tests/test_qualified_types_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14838 2023-05-08 11:46:37.000000 libsa4py-0.4.0/tests/test_representations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4519 2023-05-08 11:46:37.000000 libsa4py-0.4.0/tests/test_type_apply.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-05-08 11:46:37.000000 libsa4py-0.4.0/tests/test_vars_args_occur.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-05-08 11:46:37.000000 libsa4py-0.4.0/tests/test_visitors.py
```

### Comparing `libsa4py-0.3.0/.github/workflows/publish.yaml` & `libsa4py-0.4.0/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `libsa4py-0.3.0/CHANGELOG.md` & `libsa4py-0.4.0/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 # Changelog
 All notable changes to the [LibSA4Py](https://github.com/saltudelft/libsa4py) tool will be documented in this file. The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/) and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.4.0] - 2023-05-08
+### Added
+- Adds the `CountParametricTypeDepth` visitor to count the depth of parametric types.
+### Fixed
+- Fixed an issue where type annotations for local variables with the same name in methods were not applied (`TypeAlpplier`).
+
 ## [0.3.0] - 2022-02-17
 ### Added
 - Adding the `--tc` CLI arg for the `process` command to type-check source files in Python projects using mypy.
 - Supporting qualified names for classes by adding the `q_name` field to the JSON output.
 - Adding line and column no. info for the start and end of:
   - Functions definitions
   - Class definitions
```

### Comparing `libsa4py-0.3.0/JSONOutput.md` & `libsa4py-0.4.0/JSONOutput.md`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,16 @@
 - `tc`: Whether the processed file is successfully type-checked or not plus no. of type errors if any. **NOTE:** `[false, none]` means that type-checking failed due to the type checker's exceptions.
 - `no_types_annot`: Type slots stats for the processed module:
   - `U`: No. of types slots w/o a type annotation.
   - `D`: No of type slots w/ developer-provided annotations.
   - `I`: No. of type slots w/ Pyre-inferred annotations.
 - `type_annot_cove`: Type annotations coverage for source code files and the whole project.
 
+> NOTE: For files with no type slots, the value of `type_annot_cove` is 1.0 and the sum of values in `no_types_annot` are 0.
+
 ## Classes
 The following JSON object represents a processed class:
 
 ```json
 {
   "name": "",
   "q_name": "",
```

### Comparing `libsa4py-0.3.0/LICENSE` & `libsa4py-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `libsa4py-0.3.0/PKG-INFO` & `libsa4py-0.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: libsa4py
-Version: 0.3.0
+Version: 0.4.0
 Summary: LibSA4Py: Light-weight static analysis for extracting type hints and features
 Home-page: https://github.com/saltudelft/libsa4py
 Author: Amir M. Mir (TU Delft)
 Author-email: mir-am@hotmail.com
-License: UNKNOWN
 Keywords: libsa4py static analysis features type hints type inference machine learning python pipeline light-weight
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: Unix
@@ -20,14 +18,15 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Intro
 [![PyPI version](https://badge.fury.io/py/libsa4py.svg)](https://badge.fury.io/py/libsa4py) 
 ![GH Workflow](https://github.com/saltudelft/libsa4py/actions/workflows/libsa4py_test.yaml/badge.svg)
+[![codecov](https://codecov.io/gh/saltudelft/libsa4py/branch/master/graph/badge.svg?token=HLCIATJE6C)](https://codecov.io/gh/saltudelft/libsa4py)
 
 `LibSA4Py` is a static analysis library for Python, which extracts type hints and features for training ML-based type inference models.
 
 - [Requirements](#requirements)
 - [Quick Installation](#quick-installation)
 - [Usage](#usage)
   - [Processing projects](#processing-projects)
@@ -84,8 +83,7 @@
 
 Description:
 - `--p $REPOS_PATH`: The path to the Python corpus or dataset.
 - `--o $OUTPUT_PATH`: Path to the processed projects, used in the previous processing step.
 
 # JSON Output
 After processing each project, a JSON-formatted file is produced, which is described [here](https://github.com/saltudelft/light-sa-type-inf/blob/master/JSONOutput.md).
-
```

### Comparing `libsa4py-0.3.0/README.md` & `libsa4py-0.4.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Intro
 [![PyPI version](https://badge.fury.io/py/libsa4py.svg)](https://badge.fury.io/py/libsa4py) 
 ![GH Workflow](https://github.com/saltudelft/libsa4py/actions/workflows/libsa4py_test.yaml/badge.svg)
+[![codecov](https://codecov.io/gh/saltudelft/libsa4py/branch/master/graph/badge.svg?token=HLCIATJE6C)](https://codecov.io/gh/saltudelft/libsa4py)
 
 `LibSA4Py` is a static analysis library for Python, which extracts type hints and features for training ML-based type inference models.
 
 - [Requirements](#requirements)
 - [Quick Installation](#quick-installation)
 - [Usage](#usage)
   - [Processing projects](#processing-projects)
```

### Comparing `libsa4py-0.3.0/libsa4py/__init__.py` & `libsa4py-0.4.0/libsa4py/__init__.py`

 * *Files identical despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.3.0"
+__version__ = "0.4.0"
 
 # Package constants
 DEV_TYPE_ANNOT = 'D'
 INF_TYPE_ANNOT = 'I'
 UNK_TYPE_ANNOT = 'U'
 
 # Maximum time for type checking in sec.
```

### Comparing `libsa4py-0.3.0/libsa4py/__main__.py` & `libsa4py-0.4.0/libsa4py/__main__.py`

 * *Files identical despite different names*

### Comparing `libsa4py-0.3.0/libsa4py/cst_extractor.py` & `libsa4py-0.4.0/libsa4py/cst_extractor.py`

 * *Files identical despite different names*

### Comparing `libsa4py-0.3.0/libsa4py/cst_lenient_parser.py` & `libsa4py-0.4.0/libsa4py/cst_lenient_parser.py`

 * *Files identical despite different names*

### Comparing `libsa4py-0.3.0/libsa4py/cst_pipeline.py` & `libsa4py-0.4.0/libsa4py/cst_pipeline.py`

 * *Files identical despite different names*

### Comparing `libsa4py-0.3.0/libsa4py/cst_transformers.py` & `libsa4py-0.4.0/libsa4py/cst_transformers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1036,21 +1036,21 @@
             if fn_param_type is not None:
                 return updated_node.with_changes(annotation=fn_param_type)
 
         return original_node
 
     def visit_AssignTarget(self, node: cst.AssignTarget):
         if match.matches(node, match.AssignTarget(target=match.Name(value=match.DoNotCare()))):
-            if self.last_visited_assign_t_name == node.target.value:
+            if self.last_visited_assign_t_name == self.__get_qualified_name(node.target):
                 self.last_visited_assign_t_count += 1
             elif self.last_visited_assign_t_count == 0:
                 self.last_visited_assign_t_count = 1
             else:
                 self.last_visited_assign_t_count = 1
-            self.last_visited_assign_t_name = node.target.value
+            self.last_visited_assign_t_name = self.__get_qualified_name(node.target)
 
     def leave_Module(self, original_node: cst.Module, updated_node: cst.Module):
         return updated_node.with_changes(body=self.__get_required_imports() + list(updated_node.body))
 
     # TODO: Check the imported modules before adding new ones
     def __get_required_imports(self):
         def find_required_modules(all_types):
```

### Comparing `libsa4py-0.3.0/libsa4py/cst_visitor.py` & `libsa4py-0.4.0/libsa4py/cst_visitor.py`

 * *Files 1% similar despite different names*

```diff
@@ -746,7 +746,18 @@
         if node.annotation is not None:
             self.total_no_type_annot += 1
         return False
 
     def visit_AnnAssign(self, node: cst.AnnAssign):
         self.total_no_type_annot += 1
         return False
+
+
+class CountParametricTypeDepth(cst.CSTVisitor):
+    """
+    Counts the depth of parametric types. E.g., List[List[int]] has a depth of 2.
+    """
+    def __init__(self):
+        self.type_annot_depth = 0
+
+    def visit_Subscript(self, node):
+        self.type_annot_depth += 1
```

### Comparing `libsa4py-0.3.0/libsa4py/exceptions.py` & `libsa4py-0.4.0/libsa4py/exceptions.py`

 * *Files identical despite different names*

### Comparing `libsa4py-0.3.0/libsa4py/merge.py` & `libsa4py-0.4.0/libsa4py/merge.py`

 * *Files identical despite different names*

### Comparing `libsa4py-0.3.0/libsa4py/nl_preprocessing.py` & `libsa4py-0.4.0/libsa4py/nl_preprocessing.py`

 * *Files identical despite different names*

### Comparing `libsa4py-0.3.0/libsa4py/pyre.py` & `libsa4py-0.4.0/libsa4py/pyre.py`

 * *Files identical despite different names*

### Comparing `libsa4py-0.3.0/libsa4py/representations.py` & `libsa4py-0.4.0/libsa4py/representations.py`

 * *Files identical despite different names*

### Comparing `libsa4py-0.3.0/libsa4py/tc_errcodes.toml` & `libsa4py-0.4.0/libsa4py/tc_errcodes.toml`

 * *Files identical despite different names*

### Comparing `libsa4py-0.3.0/libsa4py/type_check.py` & `libsa4py-0.4.0/libsa4py/type_check.py`

 * *Files identical despite different names*

### Comparing `libsa4py-0.3.0/libsa4py/utils.py` & `libsa4py-0.4.0/libsa4py/utils.py`

 * *Files identical despite different names*

### Comparing `libsa4py-0.3.0/libsa4py.egg-info/PKG-INFO` & `libsa4py-0.4.0/libsa4py.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: libsa4py
-Version: 0.3.0
+Version: 0.4.0
 Summary: LibSA4Py: Light-weight static analysis for extracting type hints and features
 Home-page: https://github.com/saltudelft/libsa4py
 Author: Amir M. Mir (TU Delft)
 Author-email: mir-am@hotmail.com
-License: UNKNOWN
 Keywords: libsa4py static analysis features type hints type inference machine learning python pipeline light-weight
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: Unix
@@ -20,14 +18,15 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Intro
 [![PyPI version](https://badge.fury.io/py/libsa4py.svg)](https://badge.fury.io/py/libsa4py) 
 ![GH Workflow](https://github.com/saltudelft/libsa4py/actions/workflows/libsa4py_test.yaml/badge.svg)
+[![codecov](https://codecov.io/gh/saltudelft/libsa4py/branch/master/graph/badge.svg?token=HLCIATJE6C)](https://codecov.io/gh/saltudelft/libsa4py)
 
 `LibSA4Py` is a static analysis library for Python, which extracts type hints and features for training ML-based type inference models.
 
 - [Requirements](#requirements)
 - [Quick Installation](#quick-installation)
 - [Usage](#usage)
   - [Processing projects](#processing-projects)
@@ -84,8 +83,7 @@
 
 Description:
 - `--p $REPOS_PATH`: The path to the Python corpus or dataset.
 - `--o $OUTPUT_PATH`: Path to the processed projects, used in the previous processing step.
 
 # JSON Output
 After processing each project, a JSON-formatted file is produced, which is described [here](https://github.com/saltudelft/light-sa-type-inf/blob/master/JSONOutput.md).
-
```

### Comparing `libsa4py-0.3.0/libsa4py.egg-info/SOURCES.txt` & `libsa4py-0.4.0/libsa4py.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 tests/test_visitors.py
 tests/examples/__init__.py
 tests/examples/assignments.py
 tests/examples/comment_removal.py
 tests/examples/different_fns.py
 tests/examples/docstrings.py
 tests/examples/imports.py
+tests/examples/no_typeslots.py
 tests/examples/num_removal.py
 tests/examples/qualified_types.py
 tests/examples/representations.py
 tests/examples/space_tokens.py
 tests/examples/string_removal.py
 tests/examples/type_annot_count.py
 tests/examples/type_annot_removal.py
```

### Comparing `libsa4py-0.3.0/setup.py` & `libsa4py-0.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `libsa4py-0.3.0/tests/example.py` & `libsa4py-0.4.0/tests/example.py`

 * *Files identical despite different names*

### Comparing `libsa4py-0.3.0/tests/examples/assignments.py` & `libsa4py-0.4.0/tests/examples/assignments.py`

 * *Files identical despite different names*

### Comparing `libsa4py-0.3.0/tests/examples/different_fns.py` & `libsa4py-0.4.0/tests/examples/different_fns.py`

 * *Files identical despite different names*

### Comparing `libsa4py-0.3.0/tests/examples/docstrings.py` & `libsa4py-0.4.0/tests/examples/docstrings.py`

 * *Files identical despite different names*

### Comparing `libsa4py-0.3.0/tests/examples/qualified_types.py` & `libsa4py-0.4.0/tests/examples/qualified_types.py`

 * *Files identical despite different names*

### Comparing `libsa4py-0.3.0/tests/examples/representations.py` & `libsa4py-0.4.0/tests/examples/representations.py`

 * *Files identical despite different names*

### Comparing `libsa4py-0.3.0/tests/examples/space_tokens.py` & `libsa4py-0.4.0/tests/examples/space_tokens.py`

 * *Files identical despite different names*

### Comparing `libsa4py-0.3.0/tests/examples/string_removal.py` & `libsa4py-0.4.0/tests/examples/string_removal.py`

 * *Files identical despite different names*

### Comparing `libsa4py-0.3.0/tests/examples/type_apply_ex.json` & `libsa4py-0.4.0/tests/examples/type_apply_ex.json`

 * *Files identical despite different names*

### Comparing `libsa4py-0.3.0/tests/examples/vars_args_occur.py` & `libsa4py-0.4.0/tests/examples/vars_args_occur.py`

 * *Files identical despite different names*

### Comparing `libsa4py-0.3.0/tests/examples/vars_types_pyre_data.json` & `libsa4py-0.4.0/tests/examples/vars_types_pyre_data.json`

 * *Files identical despite different names*

### Comparing `libsa4py-0.3.0/tests/exp_outputs/added_space.py` & `libsa4py-0.4.0/tests/exp_outputs/added_space.py`

 * *Files identical despite different names*

### Comparing `libsa4py-0.3.0/tests/exp_outputs/extractor_out.json` & `libsa4py-0.4.0/tests/exp_outputs/extractor_out.json`

 * *Files identical despite different names*

### Comparing `libsa4py-0.3.0/tests/exp_outputs/extractor_out_wo_seq2seq.json` & `libsa4py-0.4.0/tests/exp_outputs/extractor_out_wo_seq2seq.json`

 * *Files identical despite different names*

### Comparing `libsa4py-0.3.0/tests/exp_outputs/normalized_mod_code.txt` & `libsa4py-0.4.0/tests/exp_outputs/normalized_mod_code.txt`

 * *Files identical despite different names*

### Comparing `libsa4py-0.3.0/tests/exp_outputs/propagated_types.py` & `libsa4py-0.4.0/tests/exp_outputs/propagated_types.py`

 * *Files identical despite different names*

### Comparing `libsa4py-0.3.0/tests/exp_outputs/testsexamples.json` & `libsa4py-0.4.0/tests/exp_outputs/testsexamples.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8674896173747276%*

 * *Differences: {"'tests/examples'": "{'src_files': {'libsa4py/tests/examples/qualified_types.py': {'typed_seq': "*

 * *                     "'0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 "*

 * *                     '0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 $typing.Dict$ 0 0 0 0 '*

 * *                     '$typing.List[builtins.str]$ 0 0 0 0 $typing.List[builtins.int]$ 0 0 0 0 0 '*

 * *                     '$typing.List[typing.Tuple[builtins.int,builtins.int]]$ 0 0 0 '*

 * *                     '$typing.Tup […]*

```diff
@@ -1634,14 +1634,40 @@
                     null
                 ],
                 "type_annot_cove": 0.0,
                 "typed_seq": "0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0",
                 "untyped_seq": "[docstring] [EOL] [EOL] import math [EOL] import typing as t [EOL] from os . path import join , split [EOL] from string import * [EOL] from . import assignments [EOL] [EOL] [EOL] def inner_imports ( ) : [EOL] import collections [EOL] collections . Counter ( ) [EOL]",
                 "variables": {}
             },
+            "libsa4py/tests/examples/no_typeslots.py": {
+                "classes": [],
+                "funcs": [],
+                "imports": [
+                    "y",
+                    "x",
+                    "z",
+                    "f"
+                ],
+                "mod_var_ln": {},
+                "mod_var_occur": {},
+                "no_types_annot": {
+                    "D": 0,
+                    "I": 0,
+                    "U": 0
+                },
+                "set": null,
+                "tc": [
+                    false,
+                    null
+                ],
+                "type_annot_cove": 1.0,
+                "typed_seq": "0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0",
+                "untyped_seq": "[docstring] [EOL] [EOL] from y . x import * [EOL] from z import * [EOL] from f import * [EOL]",
+                "variables": {}
+            },
             "libsa4py/tests/examples/num_removal.py": {
                 "classes": [],
                 "funcs": [],
                 "imports": [],
                 "mod_var_ln": {
                     "b": [
                         [
@@ -2232,14 +2258,15 @@
                     "relative_i": [],
                     "rl": [],
                     "s": [],
                     "t_a": [],
                     "t_e": [
                         "u",
                         "foo",
+                        "foo",
                         "e",
                         "foo",
                         "foo",
                         "foo",
                         "e",
                         "foo",
                         "type",
@@ -2263,15 +2290,15 @@
                 },
                 "set": null,
                 "tc": [
                     false,
                     null
                 ],
                 "type_annot_cove": 0.93,
-                "typed_seq": "0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 $typing.Dict$ 0 0 0 0 $typing.List[builtins.str]$ 0 0 0 0 $typing.List[builtins.int]$ 0 0 0 0 0 $typing.List[typing.Tuple[builtins.int,builtins.int]]$ 0 0 0 $typing.Tuple[typing.Any,...]$ 0 0 0 0 $typing.Union[typing.List[typing.Tuple[builtins.str,builtins.int]],typing.Tuple[typing.Any],typing.Tuple[typing.List[typing.Tuple[typing.Set[builtins.int]]]]]$ 0 0 0 $typing.Callable[...,typing.List]$ 0 0 0 $typing.Callable[[typing.List,typing.Dict],builtins.int]$ 0 0 0 $typing.Type[typing.List]$ 0 0 0 0 0 $libsa4py.cst_transformers.TypeQualifierResolver$ 0 0 0 0 0 $typing.Literal[\"123\"]$ 0 0 0 $[]$ 0 0 0 0 0 0 0 $typing.Union[typing.List,None]$ 0 0 0 0 $representations.Bar$ 0 0 0 0 0 $True$ 0 0 0 $test_imports.TestImports$ 0 0 0 0 0 0 0 0 0 0 $collections.abc.Sequence$ 0 0 0 0 0 0 0 0 0 $typing.Tuple$ 0 $typing.Pattern$ 0 0 0 0 0 0 0 0 0 0 0 0 0 $typing.Tuple$ 0 $typing.Tuple$ 0 $numpy.int$ 0 0 0 0 0 0 0 0 $Delta$ 0 0 0 0 0 0 0 $numpy.array$ 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 $builtins.str$ 0 0 0 0 0 0 0 $builtins.str$ 0 0 0 0 0 0 0 0 $\"Foo\"$ 0 0 0 $typing.Tuple[typing.Any,...]$ 0 0 $Foo$ 0 0 0 $typing.Tuple[typing.Any,...]$ 0 0 $typing.Tuple[Foo,libsa4py.cst_transformers.TypeQualifierResolver]$ 0 0 0 0 $typing.Tuple[typing.Any,...]$ 0 0 0 0 0 0 0",
+                "typed_seq": "0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 $typing.Dict$ 0 0 0 0 $typing.List[builtins.str]$ 0 0 0 0 $typing.List[builtins.int]$ 0 0 0 0 0 $typing.List[typing.Tuple[builtins.int,builtins.int]]$ 0 0 0 $typing.Tuple[typing.Any,...]$ 0 0 0 0 $typing.Union[typing.List[typing.Tuple[builtins.str,builtins.int]],typing.Tuple[typing.Any],typing.Tuple[typing.List[typing.Tuple[typing.Set[builtins.int]]]]]$ 0 0 0 $typing.Callable[...,typing.List]$ 0 0 0 $typing.Callable[[typing.List,typing.Dict],builtins.int]$ 0 0 0 $typing.Type[typing.List]$ 0 0 0 0 0 $libsa4py.cst_transformers.TypeQualifierResolver$ 0 0 0 0 0 $typing.Literal[\"123\"]$ 0 0 0 $[]$ 0 0 0 0 0 0 0 $typing.Union[typing.List,None]$ 0 0 0 0 $representations.Bar$ 0 0 0 0 0 $True$ 0 0 0 $test_imports.TestImports$ 0 0 0 0 0 0 0 0 0 0 $collections.abc.Sequence$ 0 0 0 0 0 0 0 0 0 $typing.Tuple$ 0 $typing.Pattern$ 0 0 0 0 0 0 0 0 0 0 0 0 0 $typing.Tuple$ 0 $typing.Tuple$ 0 $numpy.int$ 0 0 0 0 0 0 0 0 $Delta$ 0 0 0 0 0 0 0 $numpy.array$ 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 $builtins.str$ 0 0 0 0 0 0 0 $builtins.str$ 0 0 0 0 0 0 0 0 $Foo$ 0 0 0 $typing.Tuple[typing.Any,...]$ 0 0 $Foo$ 0 0 0 $typing.Tuple[typing.Any,...]$ 0 0 $typing.Tuple[Foo,libsa4py.cst_transformers.TypeQualifierResolver]$ 0 0 0 0 $typing.Tuple[typing.Any,...]$ 0 0 0 0 0 0 0",
                 "untyped_seq": "from typing import Dict as _Dict [EOL] from typing import Tuple , Union [EOL] from libsa4py . cst_transformers import TypeQualifierResolver [EOL] from . representations import Bar [EOL] from . . test_imports import TestImports [EOL] import typing as t [EOL] import typing [EOL] from collections . abc import Sequence [EOL] from builtins import str [EOL] import numpy as np [EOL] import builtins [EOL] [EOL] d = { } [EOL] l = [ ] [EOL] q_v = [ [number] ] [EOL] l_n = ... [EOL] t_e = ( ) [EOL] u_d = None [EOL] c = None [EOL] c_h = None [EOL] t_a = t . List [EOL] tqr = TypeQualifierResolver ( ) [EOL] lt = [string] [EOL] s = [ [number] , [number] ] [EOL] N = [ ] [EOL] rl = Bar ( ) [EOL] b = True [EOL] relative_i = TestImports ( ) [EOL] [EOL] class Foo : [EOL] foo_seq = [ ] [EOL] def __init__ ( self , x , y = None ) : [EOL] class Delta : [EOL] pass [EOL] self . x = x [EOL] n = np . int ( [number] ) [EOL] d = Delta ( ) [EOL] [EOL] def bar ( self ) : [EOL] return np . array ( [ [number] , [number] , [number] ] ) [EOL] [EOL] def shadow_qn ( self ) : [EOL] sq = [string] [EOL] [EOL] for str in sq : [EOL] print ( str ) [EOL] [EOL] u = Foo ( t_e ) [EOL] foo = Foo ( t_e ) [EOL] foo_t = ( Foo ( t_e ) , TypeQualifierResolver ( ) ) [EOL]",
                 "variables": {
                     "b": "True",
                     "c": "typing.Callable[..., typing.List]",
                     "c h": "typing.Callable[[typing.List, typing.Dict], builtins.int]",
                     "d": "typing.Dict",
                     "foo": "Foo",
@@ -2283,15 +2310,15 @@
                     "q v": "typing.List[builtins.int]",
                     "relative i": "test_imports.TestImports",
                     "rl": "representations.Bar",
                     "s": "[]",
                     "t a": "typing.Type[typing.List]",
                     "t e": "typing.Tuple[typing.Any, ...]",
                     "tqr": "libsa4py.cst_transformers.TypeQualifierResolver",
-                    "u": "\"Foo\"",
+                    "u": "Foo",
                     "u d": "typing.Union[typing.List[typing.Tuple[builtins.str, builtins.int]], typing.Tuple[typing.Any], typing.Tuple[typing.List[typing.Tuple[typing.Set[builtins.int]]]]]"
                 }
             },
             "libsa4py/tests/examples/representations.py": {
                 "classes": [
                     {
                         "cls_lc": [
@@ -5017,10 +5044,10 @@
                     "no": "builtins.int",
                     "pi": "",
                     "x": "",
                     "y": ""
                 }
             }
         },
-        "type_annot_cove": 0.4
+        "type_annot_cove": 0.43
     }
 }
```

### Comparing `libsa4py-0.3.0/tests/exp_outputs/testsexamples_nonlp.json` & `libsa4py-0.4.0/tests/exp_outputs/testsexamples_nonlp.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8674895053964569%*

 * *Differences: {"'tests/examples'": "{'src_files': {'libsa4py/tests/examples/qualified_types.py': {'typed_seq': "*

 * *                     "'0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 "*

 * *                     '0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 $typing.Dict$ 0 0 0 0 '*

 * *                     '$typing.List[builtins.str]$ 0 0 0 0 $typing.List[builtins.int]$ 0 0 0 0 0 '*

 * *                     '$typing.List[typing.Tuple[builtins.int,builtins.int]]$ 0 0 0 '*

 * *                     '$typing.Tup […]*

```diff
@@ -1724,14 +1724,40 @@
                     null
                 ],
                 "type_annot_cove": 0.0,
                 "typed_seq": "0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0",
                 "untyped_seq": "[docstring] [EOL] [EOL] import math [EOL] import typing as t [EOL] from os . path import join , split [EOL] from string import * [EOL] from . import assignments [EOL] [EOL] [EOL] def inner_imports ( ) : [EOL] import collections [EOL] collections . Counter ( ) [EOL]",
                 "variables": {}
             },
+            "libsa4py/tests/examples/no_typeslots.py": {
+                "classes": [],
+                "funcs": [],
+                "imports": [
+                    "y",
+                    "x",
+                    "z",
+                    "f"
+                ],
+                "mod_var_ln": {},
+                "mod_var_occur": {},
+                "no_types_annot": {
+                    "D": 0,
+                    "I": 0,
+                    "U": 0
+                },
+                "set": null,
+                "tc": [
+                    false,
+                    null
+                ],
+                "type_annot_cove": 1.0,
+                "typed_seq": "0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0",
+                "untyped_seq": "[docstring] [EOL] [EOL] from y . x import * [EOL] from z import * [EOL] from f import * [EOL]",
+                "variables": {}
+            },
             "libsa4py/tests/examples/num_removal.py": {
                 "classes": [],
                 "funcs": [],
                 "imports": [],
                 "mod_var_ln": {
                     "b": [
                         [
@@ -2337,14 +2363,15 @@
                     "rl": [],
                     "s": [],
                     "t_a": [],
                     "t_e": [
                         [
                             "u",
                             "Foo",
+                            "Foo",
                             "t_e"
                         ],
                         [
                             "foo",
                             "Foo",
                             "Foo",
                             "t_e"
@@ -2373,15 +2400,15 @@
                 },
                 "set": null,
                 "tc": [
                     false,
                     null
                 ],
                 "type_annot_cove": 0.93,
-                "typed_seq": "0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 $typing.Dict$ 0 0 0 0 $typing.List[builtins.str]$ 0 0 0 0 $typing.List[builtins.int]$ 0 0 0 0 0 $typing.List[typing.Tuple[builtins.int,builtins.int]]$ 0 0 0 $typing.Tuple[typing.Any,...]$ 0 0 0 0 $typing.Union[typing.List[typing.Tuple[builtins.str,builtins.int]],typing.Tuple[typing.Any],typing.Tuple[typing.List[typing.Tuple[typing.Set[builtins.int]]]]]$ 0 0 0 $typing.Callable[...,typing.List]$ 0 0 0 $typing.Callable[[typing.List,typing.Dict],builtins.int]$ 0 0 0 $typing.Type[typing.List]$ 0 0 0 0 0 $libsa4py.cst_transformers.TypeQualifierResolver$ 0 0 0 0 0 $typing.Literal[\"123\"]$ 0 0 0 $[]$ 0 0 0 0 0 0 0 $typing.Union[typing.List,None]$ 0 0 0 0 $representations.Bar$ 0 0 0 0 0 $True$ 0 0 0 $test_imports.TestImports$ 0 0 0 0 0 0 0 0 0 0 $collections.abc.Sequence$ 0 0 0 0 0 0 0 0 0 $typing.Tuple$ 0 $typing.Pattern$ 0 0 0 0 0 0 0 0 0 0 0 0 0 $typing.Tuple$ 0 $typing.Tuple$ 0 $numpy.int$ 0 0 0 0 0 0 0 0 $Delta$ 0 0 0 0 0 0 0 $numpy.array$ 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 $builtins.str$ 0 0 0 0 0 0 0 $builtins.str$ 0 0 0 0 0 0 0 0 $\"Foo\"$ 0 0 0 $typing.Tuple[typing.Any,...]$ 0 0 $Foo$ 0 0 0 $typing.Tuple[typing.Any,...]$ 0 0 $typing.Tuple[Foo,libsa4py.cst_transformers.TypeQualifierResolver]$ 0 0 0 0 $typing.Tuple[typing.Any,...]$ 0 0 0 0 0 0 0",
+                "typed_seq": "0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 $typing.Dict$ 0 0 0 0 $typing.List[builtins.str]$ 0 0 0 0 $typing.List[builtins.int]$ 0 0 0 0 0 $typing.List[typing.Tuple[builtins.int,builtins.int]]$ 0 0 0 $typing.Tuple[typing.Any,...]$ 0 0 0 0 $typing.Union[typing.List[typing.Tuple[builtins.str,builtins.int]],typing.Tuple[typing.Any],typing.Tuple[typing.List[typing.Tuple[typing.Set[builtins.int]]]]]$ 0 0 0 $typing.Callable[...,typing.List]$ 0 0 0 $typing.Callable[[typing.List,typing.Dict],builtins.int]$ 0 0 0 $typing.Type[typing.List]$ 0 0 0 0 0 $libsa4py.cst_transformers.TypeQualifierResolver$ 0 0 0 0 0 $typing.Literal[\"123\"]$ 0 0 0 $[]$ 0 0 0 0 0 0 0 $typing.Union[typing.List,None]$ 0 0 0 0 $representations.Bar$ 0 0 0 0 0 $True$ 0 0 0 $test_imports.TestImports$ 0 0 0 0 0 0 0 0 0 0 $collections.abc.Sequence$ 0 0 0 0 0 0 0 0 0 $typing.Tuple$ 0 $typing.Pattern$ 0 0 0 0 0 0 0 0 0 0 0 0 0 $typing.Tuple$ 0 $typing.Tuple$ 0 $numpy.int$ 0 0 0 0 0 0 0 0 $Delta$ 0 0 0 0 0 0 0 $numpy.array$ 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 $builtins.str$ 0 0 0 0 0 0 0 $builtins.str$ 0 0 0 0 0 0 0 0 $Foo$ 0 0 0 $typing.Tuple[typing.Any,...]$ 0 0 $Foo$ 0 0 0 $typing.Tuple[typing.Any,...]$ 0 0 $typing.Tuple[Foo,libsa4py.cst_transformers.TypeQualifierResolver]$ 0 0 0 0 $typing.Tuple[typing.Any,...]$ 0 0 0 0 0 0 0",
                 "untyped_seq": "from typing import Dict as _Dict [EOL] from typing import Tuple , Union [EOL] from libsa4py . cst_transformers import TypeQualifierResolver [EOL] from . representations import Bar [EOL] from . . test_imports import TestImports [EOL] import typing as t [EOL] import typing [EOL] from collections . abc import Sequence [EOL] from builtins import str [EOL] import numpy as np [EOL] import builtins [EOL] [EOL] d = { } [EOL] l = [ ] [EOL] q_v = [ [number] ] [EOL] l_n = ... [EOL] t_e = ( ) [EOL] u_d = None [EOL] c = None [EOL] c_h = None [EOL] t_a = t . List [EOL] tqr = TypeQualifierResolver ( ) [EOL] lt = [string] [EOL] s = [ [number] , [number] ] [EOL] N = [ ] [EOL] rl = Bar ( ) [EOL] b = True [EOL] relative_i = TestImports ( ) [EOL] [EOL] class Foo : [EOL] foo_seq = [ ] [EOL] def __init__ ( self , x , y = None ) : [EOL] class Delta : [EOL] pass [EOL] self . x = x [EOL] n = np . int ( [number] ) [EOL] d = Delta ( ) [EOL] [EOL] def bar ( self ) : [EOL] return np . array ( [ [number] , [number] , [number] ] ) [EOL] [EOL] def shadow_qn ( self ) : [EOL] sq = [string] [EOL] [EOL] for str in sq : [EOL] print ( str ) [EOL] [EOL] u = Foo ( t_e ) [EOL] foo = Foo ( t_e ) [EOL] foo_t = ( Foo ( t_e ) , TypeQualifierResolver ( ) ) [EOL]",
                 "variables": {
                     "N": "typing.Union[typing.List, None]",
                     "b": "True",
                     "c": "typing.Callable[..., typing.List]",
                     "c_h": "typing.Callable[[typing.List, typing.Dict], builtins.int]",
                     "d": "typing.Dict",
@@ -2393,15 +2420,15 @@
                     "q_v": "typing.List[builtins.int]",
                     "relative_i": "test_imports.TestImports",
                     "rl": "representations.Bar",
                     "s": "[]",
                     "t_a": "typing.Type[typing.List]",
                     "t_e": "typing.Tuple[typing.Any, ...]",
                     "tqr": "libsa4py.cst_transformers.TypeQualifierResolver",
-                    "u": "\"Foo\"",
+                    "u": "Foo",
                     "u_d": "typing.Union[typing.List[typing.Tuple[builtins.str, builtins.int]], typing.Tuple[typing.Any], typing.Tuple[typing.List[typing.Tuple[typing.Set[builtins.int]]]]]"
                 }
             },
             "libsa4py/tests/examples/representations.py": {
                 "classes": [
                     {
                         "cls_lc": [
@@ -5509,10 +5536,10 @@
                     "PI": "",
                     "X": "",
                     "Y": "",
                     "no": "builtins.int"
                 }
             }
         },
-        "type_annot_cove": 0.4
+        "type_annot_cove": 0.43
     }
 }
```

### Comparing `libsa4py-0.3.0/tests/test_assignments.py` & `libsa4py-0.4.0/tests/test_assignments.py`

 * *Files identical despite different names*

### Comparing `libsa4py-0.3.0/tests/test_cst_transformers.py` & `libsa4py-0.4.0/tests/test_cst_transformers.py`

 * *Files identical despite different names*

### Comparing `libsa4py-0.3.0/tests/test_different_fns.py` & `libsa4py-0.4.0/tests/test_different_fns.py`

 * *Files identical despite different names*

### Comparing `libsa4py-0.3.0/tests/test_docstrings.py` & `libsa4py-0.4.0/tests/test_docstrings.py`

 * *Files identical despite different names*

### Comparing `libsa4py-0.3.0/tests/test_extractor.py` & `libsa4py-0.4.0/tests/test_extractor.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,14 +15,15 @@
         self.maxDiff = None
 
     @classmethod
     def setUpClass(cls):
         cls.extractor_out = Extractor().extract(read_file('./examples/representations.py'))
         cls.extractor_out_wo_seq2seq = Extractor().extract(read_file('./examples/representations.py'),
                                                            include_seq2seq=False)
+        cls.extractor_out_no_typeslots = Extractor().extract(read_file('./examples/no_typeslots.py')).to_dict()
 
     def test_extractor_output(self):
         #save_json('./exp_outputs/extractor_out.json', self.extractor_out.to_dict())
         expected_out = load_json('./exp_outputs/extractor_out.json')
 
         expected_out = ModuleInfo.from_dict(expected_out)
 
@@ -32,14 +33,23 @@
         #save_json('./exp_outputs/extractor_out_wo_seq2seq.json', self.extractor_out_wo_seq2seq.to_dict())
         expected_out_wo_seq2seq = load_json('./exp_outputs/extractor_out_wo_seq2seq.json')
 
         expected_out = ModuleInfo.from_dict(expected_out_wo_seq2seq)
 
         self.assertEqual(expected_out, self.extractor_out_wo_seq2seq)
 
+    def test_extractor_no_typeslots(self):
+        """
+        Tests the default behaviour of Extractor when calculating type annotation coverage for files without type slots
+        """
+        expected_type_annot_cove = 1.0
+        expected_num_type_annot = 0
+
+        self.assertEqual(expected_type_annot_cove, self.extractor_out_no_typeslots['type_annot_cove'])
+        self.assertEqual(expected_num_type_annot, sum(self.extractor_out_no_typeslots['no_types_annot'].values()))
 
 class TestExtractorPyre(unittest.TestCase):
     """
     It tests the CST extractor of LibSA4Py while incorporating Pyre's inferred types.
     """
 
     def __init__(self, *args, **kwargs):
```

### Comparing `libsa4py-0.3.0/tests/test_helper.py` & `libsa4py-0.4.0/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `libsa4py-0.3.0/tests/test_imports.py` & `libsa4py-0.4.0/tests/test_imports.py`

 * *Files identical despite different names*

### Comparing `libsa4py-0.3.0/tests/test_pipeline.py` & `libsa4py-0.4.0/tests/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `libsa4py-0.3.0/tests/test_qualified_types_.py` & `libsa4py-0.4.0/tests/test_qualified_types_.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
                       'u_d': 'typing.Union[typing.List[typing.Tuple[builtins.str, builtins.int]], '
                              'typing.Tuple[typing.Any], typing.Tuple[typing.List[typing.Tuple[typing.Set[builtins.int]]]]]',
                       'c': 'typing.Callable[..., typing.List]',
                       't_a': 'typing.Type[typing.List]',
                       'tqr': 'libsa4py.cst_transformers.TypeQualifierResolver',
                       'lt': 'typing.Literal["123"]',
                       'c_h': 'typing.Callable[[typing.List, typing.Dict], builtins.int]',
-                      's': '[]', 'u': '"Foo"', 'foo': 'Foo', 'b': 'True',
+                      's': '[]', 'u': 'Foo', 'foo': 'Foo', 'b': 'True',
                       'foo_t': 'typing.Tuple[Foo, libsa4py.cst_transformers.TypeQualifierResolver]',
                       'N': 'typing.Union[typing.List, None]',
                       'rl': 'representations.Bar',
                       'relative_i': 'test_imports.TestImports'}
 
         self.assertDictEqual(exp_q_type, self.processed_f['variables'])
```

### Comparing `libsa4py-0.3.0/tests/test_representations.py` & `libsa4py-0.4.0/tests/test_representations.py`

 * *Files identical despite different names*

### Comparing `libsa4py-0.3.0/tests/test_type_apply.py` & `libsa4py-0.4.0/tests/test_type_apply.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 from libsa4py.utils import mk_dir_not_exist, write_file, read_file, save_json
 from libsa4py.cst_pipeline import TypeAnnotatingProjects
+from libsa4py.cst_extractor import Extractor
+from libsa4py.cst_transformers import TypeAnnotationRemover, TypeApplier
 from collections import Counter
 import unittest
 import shutil
+import libcst
 
 test_file = """from pathlib import Path
 x: int = 12
 l = [(1, 2)]
 c = defaultdict(int)
 df = pd.DataFrame([2, 3])
 dff = pd.DataFrame([1,2])
@@ -75,14 +78,22 @@
     foo_v = "No"
 def Bar(x: typing.List[builtins.str]=['apple', 'orange'], *, c)-> typing.List[builtins.str]:
     v: typing.List[builtins.str] = x
     l = lambda e: e+1
     return v
 """
 
+test_local_vars = """
+def f():
+    x: builtin.int = 10
+
+def g():
+    x: builtin.str = "Hello World"
+"""
+
 
 class TestTypeAnnotatingProjects(unittest.TestCase):
     """
     It tests applying inferred type annotations to projects.
     """
 
     def __init__(self, *args, **kwargs):
@@ -105,10 +116,28 @@
         exp = """{}""".format("\n".join(exp_split[7:]))
         out = """{}""".format("\n".join(out_split[7:]))
 
         self.assertEqual(exp, out)
         # The imported types from typing
         self.assertEqual(Counter(" ".join(exp_split[0:7])), Counter(" ".join(out_split[0:7])))
 
+    def test_type_apply_local_vars(self):
+        """
+        This tests whether type annotations for local variables with the same names are applied correctly.
+        """
+        mod = libcst.parse_module(test_local_vars)
+        annot_org = Extractor.extract(mod.code).to_dict()
+
+        annot_less = mod.visit(TypeAnnotationRemover())
+        annot_new = libcst.metadata.MetadataWrapper(annot_less,
+                                                    unsafe_skip_copy=True).visit(TypeApplier(annot_org,
+                                                                                             apply_nlp=False))
+        exp_split = mod.code.splitlines()
+        out_split = annot_new.code.splitlines()
+
+        exp = """{}""".format("\n".join(exp_split[1:]))
+        out = """{}""".format("\n".join(out_split[2:]))
+        self.assertEqual(exp, out)
+
     @classmethod
     def tearDownClass(cls):
         shutil.rmtree("./tmp_ta/")
```

### Comparing `libsa4py-0.3.0/tests/test_vars_args_occur.py` & `libsa4py-0.4.0/tests/test_vars_args_occur.py`

 * *Files identical despite different names*

