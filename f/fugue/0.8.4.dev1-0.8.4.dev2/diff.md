# Comparing `tmp/fugue-0.8.4.dev1.tar.gz` & `tmp/fugue-0.8.4.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fugue-0.8.4.dev1.tar", last modified: Wed May  3 06:43:09 2023, max compression
+gzip compressed data, was "fugue-0.8.4.dev2.tar", last modified: Mon May  8 16:09:17 2023, max compression
```

## Comparing `fugue-0.8.4.dev1.tar` & `fugue-0.8.4.dev2.tar`

### file list

```diff
@@ -1,323 +1,325 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.099465 fugue-0.8.4.dev1/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17156 2023-05-03 06:43:09.099465 fugue-0.8.4.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13928 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.075465 fugue-0.8.4.dev1/fugue/
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.075465 fugue-0.8.4.dev1/fugue/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/_utils/display.py
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/_utils/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/_utils/interfaceless.py
--rw-r--r--   0 runner    (1001) docker     (123)     9104 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/_utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/_utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/_utils/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.075465 fugue-0.8.4.dev1/fugue/bag/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/bag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/bag/array_bag.py
--rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/bag/bag.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.075465 fugue-0.8.4.dev1/fugue/collections/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/collections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17248 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/collections/partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/collections/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/collections/yielded.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.079465 fugue-0.8.4.dev1/fugue/column/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/column/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26544 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/column/expressions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9774 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/column/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    17391 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/column/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.079465 fugue-0.8.4.dev1/fugue/dataframe/
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/dataframe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9862 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/dataframe/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4447 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/dataframe/array_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    12098 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/dataframe/arrow_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    17247 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/dataframe/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     7255 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/dataframe/dataframe_iterable_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/dataframe/dataframes.py
--rw-r--r--   0 runner    (1001) docker     (123)    13505 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/dataframe/function_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4627 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/dataframe/iterable_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    10453 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/dataframe/pandas_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    10508 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/dataframe/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.079465 fugue-0.8.4.dev1/fugue/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/dataset/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/dataset/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/dev.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.079465 fugue-0.8.4.dev1/fugue/execution/
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/execution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39818 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/execution/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    49152 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/execution/execution_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)    21003 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/execution/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    13205 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/execution/native_execution_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.079465 fugue-0.8.4.dev1/fugue/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.079465 fugue-0.8.4.dev1/fugue/extensions/_builtins/
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/extensions/_builtins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/extensions/_builtins/creators.py
--rw-r--r--   0 runner    (1001) docker     (123)     6892 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/extensions/_builtins/outputters.py
--rw-r--r--   0 runner    (1001) docker     (123)    14517 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/extensions/_builtins/processors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/extensions/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/extensions/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.079465 fugue-0.8.4.dev1/fugue/extensions/creator/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/extensions/creator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7297 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/extensions/creator/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/extensions/creator/creator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.079465 fugue-0.8.4.dev1/fugue/extensions/outputter/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/extensions/outputter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6939 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/extensions/outputter/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/extensions/outputter/outputter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.079465 fugue-0.8.4.dev1/fugue/extensions/processor/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/extensions/processor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/extensions/processor/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/extensions/processor/processor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.079465 fugue-0.8.4.dev1/fugue/extensions/transformer/
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/extensions/transformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/extensions/transformer/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    23380 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/extensions/transformer/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     9098 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/extensions/transformer/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.083465 fugue-0.8.4.dev1/fugue/rpc/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/rpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8470 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/rpc/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/rpc/flask.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.083465 fugue-0.8.4.dev1/fugue/sql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/sql/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    33844 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/sql/_visitors.py
--rw-r--r--   0 runner    (1001) docker     (123)    10050 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/sql/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/sql/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.083465 fugue-0.8.4.dev1/fugue/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/workflow/_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)    11826 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/workflow/_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/workflow/_workflow_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    12495 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/workflow/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/workflow/input.py
--rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/workflow/module.py
--rw-r--r--   0 runner    (1001) docker     (123)    88219 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue/workflow/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.075465 fugue-0.8.4.dev1/fugue.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17156 2023-05-03 06:43:08.000000 fugue-0.8.4.dev1/fugue.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8231 2023-05-03 06:43:09.000000 fugue-0.8.4.dev1/fugue.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 06:43:08.000000 fugue-0.8.4.dev1/fugue.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-03 06:43:08.000000 fugue-0.8.4.dev1/fugue.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-03 06:43:08.000000 fugue-0.8.4.dev1/fugue.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-03 06:43:08.000000 fugue-0.8.4.dev1/fugue.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.083465 fugue-0.8.4.dev1/fugue_contrib/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_contrib/contrib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.083465 fugue-0.8.4.dev1/fugue_contrib/seaborn/
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_contrib/seaborn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.083465 fugue-0.8.4.dev1/fugue_contrib/viz/
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_contrib/viz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_contrib/viz/_ext.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.083465 fugue-0.8.4.dev1/fugue_dask/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_dask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_dask/_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_dask/_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_dask/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11801 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_dask/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    18309 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_dask/execution_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_dask/ibis_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_dask/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.083465 fugue-0.8.4.dev1/fugue_duckdb/
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_duckdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8880 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_duckdb/_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     4870 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_duckdb/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_duckdb/dask.py
--rw-r--r--   0 runner    (1001) docker     (123)     6076 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_duckdb/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    20479 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_duckdb/execution_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_duckdb/ibis_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_duckdb/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.083465 fugue-0.8.4.dev1/fugue_ibis/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_ibis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_ibis/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_ibis/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7302 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_ibis/dataframe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.087465 fugue-0.8.4.dev1/fugue_ibis/execution/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_ibis/execution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_ibis/execution/ibis_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_ibis/execution/pandas_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    18540 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_ibis/execution_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     6905 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_ibis/extensions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.087465 fugue-0.8.4.dev1/fugue_notebook/
--rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_notebook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_notebook/env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.087465 fugue-0.8.4.dev1/fugue_notebook/nbextension/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_notebook/nbextension/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_notebook/nbextension/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_notebook/nbextension/description.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_notebook/nbextension/main.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.087465 fugue-0.8.4.dev1/fugue_polars/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_polars/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_polars/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6916 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_polars/polars_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_polars/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.087465 fugue-0.8.4.dev1/fugue_ray/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_ray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_ray/_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.087465 fugue-0.8.4.dev1/fugue_ray/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_ray/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_ray/_utils/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_ray/_utils/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     8737 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_ray/_utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    10377 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_ray/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    12170 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_ray/execution_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_ray/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.087465 fugue-0.8.4.dev1/fugue_spark/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_spark/_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.087465 fugue-0.8.4.dev1/fugue_spark/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_spark/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6527 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_spark/_utils/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     5527 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_spark/_utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_spark/_utils/partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     9393 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_spark/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    31733 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_spark/execution_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_spark/ibis_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_spark/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.087465 fugue-0.8.4.dev1/fugue_sql/
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_sql/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.087465 fugue-0.8.4.dev1/fugue_test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_test/bag_suite.py
--rw-r--r--   0 runner    (1001) docker     (123)    75748 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_test/builtin_suite.py
--rw-r--r--   0 runner    (1001) docker     (123)    19082 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_test/dataframe_suite.py
--rw-r--r--   0 runner    (1001) docker     (123)    50559 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_test/execution_suite.py
--rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_test/ibis_suite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.087465 fugue-0.8.4.dev1/fugue_version/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/fugue_version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-03 06:43:09.099465 fugue-0.8.4.dev1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.087465 fugue-0.8.4.dev1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.087465 fugue-0.8.4.dev1/tests/fugue/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.087465 fugue-0.8.4.dev1/tests/fugue/bag/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/bag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/bag/test_array_bag.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.091466 fugue-0.8.4.dev1/tests/fugue/collections/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/collections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8852 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/collections/test_partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/collections/test_sql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.091466 fugue-0.8.4.dev1/tests/fugue/column/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/column/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8037 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/column/test_expressions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/column/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8954 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/column/test_sql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.091466 fugue-0.8.4.dev1/tests/fugue/dataframe/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/dataframe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6009 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/dataframe/test_array_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/dataframe/test_arrow_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/dataframe/test_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/dataframe/test_dataframe_iterable_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/dataframe/test_dataframes.py
--rw-r--r--   0 runner    (1001) docker     (123)     8608 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/dataframe/test_function_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/dataframe/test_iterable_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     7255 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/dataframe/test_pandas_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     7981 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/dataframe/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.091466 fugue-0.8.4.dev1/tests/fugue/execution/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/execution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/execution/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/execution/test_execution_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)    10284 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/execution/test_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/execution/test_ibis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/execution/test_naive_execution_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.091466 fugue-0.8.4.dev1/tests/fugue/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.091466 fugue-0.8.4.dev1/tests/fugue/extensions/creator/
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/extensions/creator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/extensions/creator/test_convert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.091466 fugue-0.8.4.dev1/tests/fugue/extensions/outputter/
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/extensions/outputter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5470 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/extensions/outputter/test_convert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.091466 fugue-0.8.4.dev1/tests/fugue/extensions/processor/
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/extensions/processor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6456 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/extensions/processor/test_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     4915 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/extensions/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.091466 fugue-0.8.4.dev1/tests/fugue/extensions/transformer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/extensions/transformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/extensions/transformer/test_convert_cotransformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/extensions/transformer/test_convert_output_cotransformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/extensions/transformer/test_convert_output_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7357 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/extensions/transformer/test_convert_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.091466 fugue-0.8.4.dev1/tests/fugue/rpc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/rpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/rpc/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/rpc/test_flask.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/rpc/test_func.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.091466 fugue-0.8.4.dev1/tests/fugue/sql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/sql/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6816 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/sql/test_visitors.py
--rw-r--r--   0 runner    (1001) docker     (123)    11133 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/sql/test_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)    23329 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/sql/test_workflow_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/test_interfaceless.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.095466 fugue-0.8.4.dev1/tests/fugue/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/utils/test_interfaceless.py
--rw-r--r--   0 runner    (1001) docker     (123)     8170 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/utils/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/utils/test_misc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.095466 fugue-0.8.4.dev1/tests/fugue/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5303 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/workflow/test_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/workflow/test_runtime_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     7292 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/workflow/test_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     8295 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/workflow/test_workflow_determinism.py
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue/workflow/test_workflow_parallel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.095466 fugue-0.8.4.dev1/tests/fugue_dask/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue_dask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8244 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue_dask/test_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     7762 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue_dask/test_execution_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue_dask/test_ibis.py
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue_dask/test_importless.py
--rw-r--r--   0 runner    (1001) docker     (123)     4514 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue_dask/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue_dask/test_sql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.095466 fugue-0.8.4.dev1/tests/fugue_duckdb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue_duckdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue_duckdb/test_dask.py
--rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue_duckdb/test_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     7093 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue_duckdb/test_execution_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue_duckdb/test_ibis.py
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue_duckdb/test_importless.py
--rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue_duckdb/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.095466 fugue-0.8.4.dev1/tests/fugue_ibis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue_ibis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.095466 fugue-0.8.4.dev1/tests/fugue_ibis/mock/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue_ibis/mock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue_ibis/mock/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue_ibis/mock/execution_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue_ibis/test_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue_ibis/test_execution_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue_ibis/test_extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue_ibis/test_importless.py
--rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue_ibis/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.095466 fugue-0.8.4.dev1/tests/fugue_notebook/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue_notebook/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.095466 fugue-0.8.4.dev1/tests/fugue_polars/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue_polars/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue_polars/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue_polars/test_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue_polars/test_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.095466 fugue-0.8.4.dev1/tests/fugue_ray/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue_ray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue_ray/test_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     8689 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue_ray/test_execution_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue_ray/test_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue_ray/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.099465 fugue-0.8.4.dev1/tests/fugue_spark/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue_spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue_spark/test_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    14805 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue_spark/test_execution_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue_spark/test_ibis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue_spark/test_importless.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue_spark/test_sql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:43:09.099465 fugue-0.8.4.dev1/tests/fugue_spark/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue_spark/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue_spark/utils/test_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue_spark/utils/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     4726 2023-05-03 06:40:55.000000 fugue-0.8.4.dev1/tests/fugue_spark/utils/test_partition.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.931146 fugue-0.8.4.dev2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17156 2023-05-08 16:09:17.931146 fugue-0.8.4.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13928 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.911146 fugue-0.8.4.dev2/fugue/
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.911146 fugue-0.8.4.dev2/fugue/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/_utils/display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/_utils/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/_utils/interfaceless.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9104 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/_utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/_utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/_utils/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.911146 fugue-0.8.4.dev2/fugue/bag/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/bag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/bag/array_bag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/bag/bag.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.911146 fugue-0.8.4.dev2/fugue/collections/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/collections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17248 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/collections/partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/collections/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/collections/yielded.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.911146 fugue-0.8.4.dev2/fugue/column/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/column/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26544 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/column/expressions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9774 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/column/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17391 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/column/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.915146 fugue-0.8.4.dev2/fugue/dataframe/
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/dataframe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9862 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/dataframe/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4447 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/dataframe/array_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12098 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/dataframe/arrow_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17247 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/dataframe/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7255 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/dataframe/dataframe_iterable_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/dataframe/dataframes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13505 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/dataframe/function_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4627 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/dataframe/iterable_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10453 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/dataframe/pandas_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10508 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/dataframe/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.915146 fugue-0.8.4.dev2/fugue/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/dataset/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/dataset/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/dev.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.915146 fugue-0.8.4.dev2/fugue/execution/
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/execution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39818 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/execution/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49152 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/execution/execution_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21003 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/execution/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13205 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/execution/native_execution_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.915146 fugue-0.8.4.dev2/fugue/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.915146 fugue-0.8.4.dev2/fugue/extensions/_builtins/
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/extensions/_builtins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/extensions/_builtins/creators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6892 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/extensions/_builtins/outputters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14517 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/extensions/_builtins/processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/extensions/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/extensions/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.915146 fugue-0.8.4.dev2/fugue/extensions/creator/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/extensions/creator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7297 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/extensions/creator/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/extensions/creator/creator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.915146 fugue-0.8.4.dev2/fugue/extensions/outputter/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/extensions/outputter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6939 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/extensions/outputter/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/extensions/outputter/outputter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.915146 fugue-0.8.4.dev2/fugue/extensions/processor/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/extensions/processor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/extensions/processor/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/extensions/processor/processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.915146 fugue-0.8.4.dev2/fugue/extensions/transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/extensions/transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/extensions/transformer/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23380 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/extensions/transformer/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9098 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/extensions/transformer/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.915146 fugue-0.8.4.dev2/fugue/rpc/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/rpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8470 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/rpc/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/rpc/flask.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.915146 fugue-0.8.4.dev2/fugue/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/sql/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33844 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/sql/_visitors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10050 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/sql/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/sql/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.919146 fugue-0.8.4.dev2/fugue/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/workflow/_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11826 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/workflow/_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/workflow/_workflow_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12495 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/workflow/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/workflow/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/workflow/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88219 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue/workflow/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.911146 fugue-0.8.4.dev2/fugue.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17156 2023-05-08 16:09:17.000000 fugue-0.8.4.dev2/fugue.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8298 2023-05-08 16:09:17.000000 fugue-0.8.4.dev2/fugue.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 16:09:17.000000 fugue-0.8.4.dev2/fugue.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-08 16:09:17.000000 fugue-0.8.4.dev2/fugue.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-08 16:09:17.000000 fugue-0.8.4.dev2/fugue.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-08 16:09:17.000000 fugue-0.8.4.dev2/fugue.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.919146 fugue-0.8.4.dev2/fugue_contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_contrib/contrib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.919146 fugue-0.8.4.dev2/fugue_contrib/seaborn/
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_contrib/seaborn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.919146 fugue-0.8.4.dev2/fugue_contrib/viz/
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_contrib/viz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_contrib/viz/_ext.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.919146 fugue-0.8.4.dev2/fugue_dask/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_dask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_dask/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_dask/_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4476 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_dask/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11801 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_dask/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18462 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_dask/execution_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_dask/ibis_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_dask/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.919146 fugue-0.8.4.dev2/fugue_duckdb/
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_duckdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8880 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_duckdb/_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4870 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_duckdb/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_duckdb/dask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6076 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_duckdb/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20479 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_duckdb/execution_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_duckdb/ibis_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_duckdb/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.919146 fugue-0.8.4.dev2/fugue_ibis/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_ibis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_ibis/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_ibis/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7302 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_ibis/dataframe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.919146 fugue-0.8.4.dev2/fugue_ibis/execution/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_ibis/execution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_ibis/execution/ibis_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_ibis/execution/pandas_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18540 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_ibis/execution_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6905 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_ibis/extensions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.919146 fugue-0.8.4.dev2/fugue_notebook/
+-rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_notebook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4773 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_notebook/env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.919146 fugue-0.8.4.dev2/fugue_notebook/nbextension/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_notebook/nbextension/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_notebook/nbextension/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_notebook/nbextension/description.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_notebook/nbextension/main.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.919146 fugue-0.8.4.dev2/fugue_polars/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_polars/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_polars/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6916 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_polars/polars_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_polars/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.923146 fugue-0.8.4.dev2/fugue_ray/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_ray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_ray/_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.923146 fugue-0.8.4.dev2/fugue_ray/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_ray/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_ray/_utils/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_ray/_utils/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8737 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_ray/_utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10377 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_ray/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12596 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_ray/execution_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_ray/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.923146 fugue-0.8.4.dev2/fugue_spark/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_spark/_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.923146 fugue-0.8.4.dev2/fugue_spark/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_spark/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6552 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_spark/_utils/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5527 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_spark/_utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_spark/_utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_spark/_utils/partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9510 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_spark/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32541 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_spark/execution_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_spark/ibis_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_spark/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.923146 fugue-0.8.4.dev2/fugue_sql/
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_sql/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.923146 fugue-0.8.4.dev2/fugue_test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_test/bag_suite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75748 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_test/builtin_suite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19082 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_test/dataframe_suite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50559 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_test/execution_suite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_test/ibis_suite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.923146 fugue-0.8.4.dev2/fugue_version/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/fugue_version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-08 16:09:17.935146 fugue-0.8.4.dev2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.923146 fugue-0.8.4.dev2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.923146 fugue-0.8.4.dev2/tests/fugue/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.923146 fugue-0.8.4.dev2/tests/fugue/bag/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/bag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/bag/test_array_bag.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.923146 fugue-0.8.4.dev2/tests/fugue/collections/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/collections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8852 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/collections/test_partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/collections/test_sql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.923146 fugue-0.8.4.dev2/tests/fugue/column/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/column/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8037 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/column/test_expressions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/column/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8954 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/column/test_sql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.927146 fugue-0.8.4.dev2/tests/fugue/dataframe/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/dataframe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6009 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/dataframe/test_array_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/dataframe/test_arrow_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/dataframe/test_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/dataframe/test_dataframe_iterable_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/dataframe/test_dataframes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8608 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/dataframe/test_function_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/dataframe/test_iterable_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7255 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/dataframe/test_pandas_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7981 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/dataframe/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.927146 fugue-0.8.4.dev2/tests/fugue/execution/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/execution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/execution/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/execution/test_execution_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10284 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/execution/test_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/execution/test_ibis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/execution/test_naive_execution_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.927146 fugue-0.8.4.dev2/tests/fugue/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.927146 fugue-0.8.4.dev2/tests/fugue/extensions/creator/
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/extensions/creator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/extensions/creator/test_convert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.927146 fugue-0.8.4.dev2/tests/fugue/extensions/outputter/
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/extensions/outputter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5470 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/extensions/outputter/test_convert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.927146 fugue-0.8.4.dev2/tests/fugue/extensions/processor/
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/extensions/processor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6456 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/extensions/processor/test_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4915 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/extensions/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.927146 fugue-0.8.4.dev2/tests/fugue/extensions/transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/extensions/transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/extensions/transformer/test_convert_cotransformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/extensions/transformer/test_convert_output_cotransformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/extensions/transformer/test_convert_output_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7357 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/extensions/transformer/test_convert_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.927146 fugue-0.8.4.dev2/tests/fugue/rpc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/rpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/rpc/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/rpc/test_flask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/rpc/test_func.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.927146 fugue-0.8.4.dev2/tests/fugue/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/sql/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6816 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/sql/test_visitors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11133 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/sql/test_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23329 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/sql/test_workflow_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/test_interfaceless.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.927146 fugue-0.8.4.dev2/tests/fugue/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/utils/test_interfaceless.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8170 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/utils/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/utils/test_misc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.927146 fugue-0.8.4.dev2/tests/fugue/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5303 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/workflow/test_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/workflow/test_runtime_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7292 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/workflow/test_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8295 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/workflow/test_workflow_determinism.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue/workflow/test_workflow_parallel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.931146 fugue-0.8.4.dev2/tests/fugue_dask/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue_dask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8244 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue_dask/test_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8296 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue_dask/test_execution_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue_dask/test_ibis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue_dask/test_importless.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4514 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue_dask/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue_dask/test_sql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.931146 fugue-0.8.4.dev2/tests/fugue_duckdb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue_duckdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue_duckdb/test_dask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue_duckdb/test_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7093 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue_duckdb/test_execution_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue_duckdb/test_ibis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue_duckdb/test_importless.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue_duckdb/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.931146 fugue-0.8.4.dev2/tests/fugue_ibis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue_ibis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.931146 fugue-0.8.4.dev2/tests/fugue_ibis/mock/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue_ibis/mock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue_ibis/mock/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue_ibis/mock/execution_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue_ibis/test_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue_ibis/test_execution_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue_ibis/test_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue_ibis/test_importless.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue_ibis/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.931146 fugue-0.8.4.dev2/tests/fugue_notebook/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue_notebook/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.931146 fugue-0.8.4.dev2/tests/fugue_polars/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue_polars/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue_polars/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue_polars/test_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue_polars/test_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.931146 fugue-0.8.4.dev2/tests/fugue_ray/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue_ray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue_ray/test_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8689 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue_ray/test_execution_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue_ray/test_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue_ray/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.931146 fugue-0.8.4.dev2/tests/fugue_spark/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue_spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue_spark/test_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14844 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue_spark/test_execution_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue_spark/test_ibis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue_spark/test_importless.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue_spark/test_spark_connect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue_spark/test_sql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:09:17.931146 fugue-0.8.4.dev2/tests/fugue_spark/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue_spark/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue_spark/utils/test_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue_spark/utils/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4726 2023-05-08 16:06:56.000000 fugue-0.8.4.dev2/tests/fugue_spark/utils/test_partition.py
```

### Comparing `fugue-0.8.4.dev1/LICENSE` & `fugue-0.8.4.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/PKG-INFO` & `fugue-0.8.4.dev2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fugue
-Version: 0.8.4.dev1
+Version: 0.8.4.dev2
 Summary: An abstraction layer for distributed computation
 Home-page: http://github.com/fugue-project/fugue
 Author: The Fugue Development Team
 Author-email: hello@fugue.ai
 License: Apache-2.0
 Description: # Fugue
```

### Comparing `fugue-0.8.4.dev1/README.md` & `fugue-0.8.4.dev2/README.md`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue/__init__.py` & `fugue-0.8.4.dev2/fugue/__init__.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue/_utils/display.py` & `fugue-0.8.4.dev2/fugue/_utils/display.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue/_utils/exception.py` & `fugue-0.8.4.dev2/fugue/_utils/exception.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue/_utils/interfaceless.py` & `fugue-0.8.4.dev2/fugue/_utils/interfaceless.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue/_utils/io.py` & `fugue-0.8.4.dev2/fugue/_utils/io.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue/api.py` & `fugue-0.8.4.dev2/fugue/api.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue/bag/array_bag.py` & `fugue-0.8.4.dev2/fugue/bag/array_bag.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue/bag/bag.py` & `fugue-0.8.4.dev2/fugue/bag/bag.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue/collections/partition.py` & `fugue-0.8.4.dev2/fugue/collections/partition.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue/collections/sql.py` & `fugue-0.8.4.dev2/fugue/collections/sql.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue/collections/yielded.py` & `fugue-0.8.4.dev2/fugue/collections/yielded.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue/column/expressions.py` & `fugue-0.8.4.dev2/fugue/column/expressions.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue/column/functions.py` & `fugue-0.8.4.dev2/fugue/column/functions.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue/column/sql.py` & `fugue-0.8.4.dev2/fugue/column/sql.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue/constants.py` & `fugue-0.8.4.dev2/fugue/constants.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue/dataframe/__init__.py` & `fugue-0.8.4.dev2/fugue/dataframe/__init__.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue/dataframe/api.py` & `fugue-0.8.4.dev2/fugue/dataframe/api.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue/dataframe/array_dataframe.py` & `fugue-0.8.4.dev2/fugue/dataframe/array_dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue/dataframe/arrow_dataframe.py` & `fugue-0.8.4.dev2/fugue/dataframe/arrow_dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue/dataframe/dataframe.py` & `fugue-0.8.4.dev2/fugue/dataframe/dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue/dataframe/dataframe_iterable_dataframe.py` & `fugue-0.8.4.dev2/fugue/dataframe/dataframe_iterable_dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue/dataframe/dataframes.py` & `fugue-0.8.4.dev2/fugue/dataframe/dataframes.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue/dataframe/function_wrapper.py` & `fugue-0.8.4.dev2/fugue/dataframe/function_wrapper.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue/dataframe/iterable_dataframe.py` & `fugue-0.8.4.dev2/fugue/dataframe/iterable_dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue/dataframe/pandas_dataframe.py` & `fugue-0.8.4.dev2/fugue/dataframe/pandas_dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue/dataframe/utils.py` & `fugue-0.8.4.dev2/fugue/dataframe/utils.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue/dataset/api.py` & `fugue-0.8.4.dev2/fugue/dataset/api.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue/dataset/dataset.py` & `fugue-0.8.4.dev2/fugue/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue/dev.py` & `fugue-0.8.4.dev2/fugue/dev.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue/exceptions.py` & `fugue-0.8.4.dev2/fugue/exceptions.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue/execution/api.py` & `fugue-0.8.4.dev2/fugue/execution/api.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue/execution/execution_engine.py` & `fugue-0.8.4.dev2/fugue/execution/execution_engine.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue/execution/factory.py` & `fugue-0.8.4.dev2/fugue/execution/factory.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue/execution/native_execution_engine.py` & `fugue-0.8.4.dev2/fugue/execution/native_execution_engine.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue/extensions/__init__.py` & `fugue-0.8.4.dev2/fugue/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue/extensions/_builtins/__init__.py` & `fugue-0.8.4.dev2/fugue/extensions/_builtins/__init__.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue/extensions/_builtins/creators.py` & `fugue-0.8.4.dev2/fugue/extensions/_builtins/creators.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue/extensions/_builtins/outputters.py` & `fugue-0.8.4.dev2/fugue/extensions/_builtins/outputters.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue/extensions/_builtins/processors.py` & `fugue-0.8.4.dev2/fugue/extensions/_builtins/processors.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue/extensions/_utils.py` & `fugue-0.8.4.dev2/fugue/extensions/_utils.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue/extensions/context.py` & `fugue-0.8.4.dev2/fugue/extensions/context.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue/extensions/creator/convert.py` & `fugue-0.8.4.dev2/fugue/extensions/creator/convert.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue/extensions/creator/creator.py` & `fugue-0.8.4.dev2/fugue/extensions/creator/creator.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue/extensions/outputter/convert.py` & `fugue-0.8.4.dev2/fugue/extensions/outputter/convert.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue/extensions/outputter/outputter.py` & `fugue-0.8.4.dev2/fugue/extensions/outputter/outputter.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue/extensions/processor/convert.py` & `fugue-0.8.4.dev2/fugue/extensions/processor/convert.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue/extensions/processor/processor.py` & `fugue-0.8.4.dev2/fugue/extensions/processor/processor.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue/extensions/transformer/convert.py` & `fugue-0.8.4.dev2/fugue/extensions/transformer/convert.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue/extensions/transformer/transformer.py` & `fugue-0.8.4.dev2/fugue/extensions/transformer/transformer.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue/plugins.py` & `fugue-0.8.4.dev2/fugue/plugins.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue/registry.py` & `fugue-0.8.4.dev2/fugue/registry.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue/rpc/base.py` & `fugue-0.8.4.dev2/fugue/rpc/base.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue/rpc/flask.py` & `fugue-0.8.4.dev2/fugue/rpc/flask.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue/sql/_utils.py` & `fugue-0.8.4.dev2/fugue/sql/_utils.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue/sql/_visitors.py` & `fugue-0.8.4.dev2/fugue/sql/_visitors.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue/sql/api.py` & `fugue-0.8.4.dev2/fugue/sql/api.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue/sql/workflow.py` & `fugue-0.8.4.dev2/fugue/sql/workflow.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue/workflow/_checkpoint.py` & `fugue-0.8.4.dev2/fugue/workflow/_checkpoint.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue/workflow/_tasks.py` & `fugue-0.8.4.dev2/fugue/workflow/_tasks.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue/workflow/_workflow_context.py` & `fugue-0.8.4.dev2/fugue/workflow/_workflow_context.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue/workflow/api.py` & `fugue-0.8.4.dev2/fugue/workflow/api.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue/workflow/module.py` & `fugue-0.8.4.dev2/fugue/workflow/module.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue/workflow/workflow.py` & `fugue-0.8.4.dev2/fugue/workflow/workflow.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue.egg-info/PKG-INFO` & `fugue-0.8.4.dev2/fugue.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fugue
-Version: 0.8.4.dev1
+Version: 0.8.4.dev2
 Summary: An abstraction layer for distributed computation
 Home-page: http://github.com/fugue-project/fugue
 Author: The Fugue Development Team
 Author-email: hello@fugue.ai
 License: Apache-2.0
 Description: # Fugue
```

### Comparing `fugue-0.8.4.dev1/fugue.egg-info/SOURCES.txt` & `fugue-0.8.4.dev2/fugue.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -142,14 +142,15 @@
 fugue_spark/dataframe.py
 fugue_spark/execution_engine.py
 fugue_spark/ibis_engine.py
 fugue_spark/registry.py
 fugue_spark/_utils/__init__.py
 fugue_spark/_utils/convert.py
 fugue_spark/_utils/io.py
+fugue_spark/_utils/misc.py
 fugue_spark/_utils/partition.py
 fugue_sql/__init__.py
 fugue_sql/exceptions.py
 fugue_test/__init__.py
 fugue_test/bag_suite.py
 fugue_test/builtin_suite.py
 fugue_test/dataframe_suite.py
@@ -250,12 +251,13 @@
 tests/fugue_ray/test_registry.py
 tests/fugue_ray/test_utils.py
 tests/fugue_spark/__init__.py
 tests/fugue_spark/test_dataframe.py
 tests/fugue_spark/test_execution_engine.py
 tests/fugue_spark/test_ibis.py
 tests/fugue_spark/test_importless.py
+tests/fugue_spark/test_spark_connect.py
 tests/fugue_spark/test_sql.py
 tests/fugue_spark/utils/__init__.py
 tests/fugue_spark/utils/test_convert.py
 tests/fugue_spark/utils/test_io.py
 tests/fugue_spark/utils/test_partition.py
```

### Comparing `fugue-0.8.4.dev1/fugue.egg-info/requires.txt` & `fugue-0.8.4.dev2/fugue.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue_contrib/seaborn/__init__.py` & `fugue-0.8.4.dev2/fugue_contrib/seaborn/__init__.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue_contrib/viz/__init__.py` & `fugue-0.8.4.dev2/fugue_contrib/viz/__init__.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue_contrib/viz/_ext.py` & `fugue-0.8.4.dev2/fugue_contrib/viz/_ext.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from abc import ABC, abstractmethod
+from typing import Any
 
 import pandas as pd
 from triad import assert_or_throw
 
 from fugue import DataFrames, Outputter
 from fugue.exceptions import FugueWorkflowError
 
@@ -21,13 +22,18 @@
         if len(presort_keys) > 0:
             df = df.sort_values(presort_keys, ascending=presort_asc).reset_index(
                 drop=True
             )
         if len(self.partition_spec.partition_by) == 0:
             self._plot(df)
         else:
-            for _, gp in df.groupby(self.partition_spec.partition_by, dropna=False):
+            keys: Any = (  # avoid pandas warning
+                self.partition_spec.partition_by
+                if len(self.partition_spec.partition_by) > 1
+                else self.partition_spec.partition_by[0]
+            )
+            for _, gp in df.groupby(keys, dropna=False):
                 self._plot(gp.reset_index(drop=True))
 
     @abstractmethod
     def _plot(self, df: pd.DataFrame) -> None:  # pragma: no cover
         raise NotImplementedError
```

### Comparing `fugue-0.8.4.dev1/fugue_dask/_io.py` & `fugue-0.8.4.dev2/fugue_dask/_io.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue_dask/_utils.py` & `fugue-0.8.4.dev2/fugue_dask/_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -82,28 +82,34 @@
         no longer be `int64`
         This method does not enforce struct and list types
         """
         if not null_safe:
             return df.astype(dtype=to_pandas_dtype(schema))
         for v in schema:
             s = df[v.name]
-            if pa.types.is_string(v.type):
+            if pa.types.is_string(v.type) and not pandas.api.types.is_string_dtype(
+                s.dtype
+            ):
                 ns = s.isnull()
                 s = s.astype(str).mask(ns, None)
-            elif pa.types.is_boolean(v.type):
+            elif pa.types.is_boolean(v.type) and not pandas.api.types.is_bool_dtype(
+                s.dtype
+            ):
                 ns = s.isnull()
                 if pandas.api.types.is_string_dtype(s.dtype):
                     try:
                         s = s.str.lower() == "true"
                     except AttributeError:
                         s = s.fillna(0).astype(bool)
                 else:
                     s = s.fillna(0).astype(bool)
-                s = s.mask(ns, None)
-            elif pa.types.is_integer(v.type):
+                s = s.mask(ns, None).astype("boolean")
+            elif pa.types.is_integer(v.type) and not pandas.api.types.is_integer_dtype(
+                s.dtype
+            ):
                 ns = s.isnull()
                 s = s.fillna(0).astype(v.type.to_pandas_dtype()).mask(ns, None)
             elif not pa.types.is_struct(v.type) and not pa.types.is_list(v.type):
                 s = s.astype(v.type.to_pandas_dtype())
             df[v.name] = s
         return df
```

### Comparing `fugue-0.8.4.dev1/fugue_dask/dataframe.py` & `fugue-0.8.4.dev2/fugue_dask/dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue_dask/execution_engine.py` & `fugue-0.8.4.dev2/fugue_dask/execution_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -275,30 +275,30 @@
         key_schema, output_schema = get_join_schemas(df1, df2, how=how, on=on)
         d = self.pl_utils.join(
             self.to_df(df1).native,
             self.to_df(df2).native,
             join_type=how,
             on=key_schema.names,
         )
-        return DaskDataFrame(d, output_schema)
+        return DaskDataFrame(d, output_schema, type_safe=False)
 
     def union(
         self,
         df1: DataFrame,
         df2: DataFrame,
         distinct: bool = True,
     ) -> DataFrame:
         assert_or_throw(
             df1.schema == df2.schema,
             lambda: ValueError(f"{df1.schema} != {df2.schema}"),
         )
         d = self.pl_utils.union(
             self.to_df(df1).native, self.to_df(df2).native, unique=distinct
         )
-        return DaskDataFrame(d, df1.schema)
+        return DaskDataFrame(d, df1.schema, type_safe=False)
 
     def subtract(
         self,
         df1: DataFrame,
         df2: DataFrame,
         distinct: bool = True,
     ) -> DataFrame:
@@ -308,15 +308,15 @@
         assert_or_throw(
             df1.schema == df2.schema,
             lambda: ValueError(f"{df1.schema} != {df2.schema}"),
         )
         d = self.pl_utils.except_df(
             self.to_df(df1).native, self.to_df(df2).native, unique=distinct
         )
-        return DaskDataFrame(d, df1.schema)
+        return DaskDataFrame(d, df1.schema, type_safe=False)
 
     def intersect(
         self,
         df1: DataFrame,
         df2: DataFrame,
         distinct: bool = True,
     ) -> DataFrame:
@@ -326,19 +326,19 @@
         assert_or_throw(
             df1.schema == df2.schema,
             lambda: ValueError(f"{df1.schema} != {df2.schema}"),
         )
         d = self.pl_utils.intersect(
             self.to_df(df1).native, self.to_df(df2).native, unique=distinct
         )
-        return DaskDataFrame(d, df1.schema)
+        return DaskDataFrame(d, df1.schema, type_safe=False)
 
     def distinct(self, df: DataFrame) -> DataFrame:
         d = self.pl_utils.drop_duplicates(self.to_df(df).native)
-        return DaskDataFrame(d, df.schema)
+        return DaskDataFrame(d, df.schema, type_safe=False)
 
     def dropna(
         self,
         df: DataFrame,
         how: str = "any",
         thresh: int = None,
         subset: List[str] = None,
@@ -347,15 +347,15 @@
         if thresh is not None:
             kw["thresh"] = thresh
         if subset is not None:
             kw["subset"] = subset
         if how == "any" and thresh is not None:
             del kw["how"]  # to deal with a dask logic flaw
         d = self.to_df(df).native.dropna(**kw)
-        return DaskDataFrame(d, df.schema)
+        return DaskDataFrame(d, df.schema, type_safe=False)
 
     def fillna(self, df: DataFrame, value: Any, subset: List[str] = None) -> DataFrame:
         assert_or_throw(
             (not isinstance(value, list)) and (value is not None),
             ValueError("fillna value can not be a list or None"),
         )
         if isinstance(value, dict):
@@ -367,15 +367,15 @@
             )
             mapping = value
         else:
             # If subset is none, apply to all columns
             subset = subset or df.columns
             mapping = {col: value for col in subset}
         d = self.to_df(df).native.fillna(mapping)
-        return DaskDataFrame(d, df.schema)
+        return DaskDataFrame(d, df.schema, type_safe=False)
 
     def sample(
         self,
         df: DataFrame,
         n: Optional[int] = None,
         frac: Optional[float] = None,
         replace: bool = False,
@@ -385,15 +385,15 @@
             (n is None and frac is not None) or (n is not None and frac is None),
             ValueError("one and only one of n and frac should be set"),
         )
         # TODO: dask does not support sample by number of rows
         d = self.to_df(df).native.sample(
             n=n, frac=frac, replace=replace, random_state=seed
         )
-        return DaskDataFrame(d, df.schema)
+        return DaskDataFrame(d, df.schema, type_safe=False)
 
     def take(
         self,
         df: DataFrame,
         n: int,
         presort: str,
         na_position: str = "last",
@@ -441,15 +441,15 @@
         else:
             d = (
                 d.groupby(partition_spec.partition_by, dropna=False)
                 .apply(_partition_take, n=n, presort=_presort, meta=meta)
                 .reset_index(drop=True)
             )
 
-        return DaskDataFrame(d, df.schema)
+        return DaskDataFrame(d, df.schema, type_safe=False)
 
     def load_df(
         self,
         path: Union[str, List[str]],
         format_hint: Any = None,
         columns: Any = None,
         **kwargs: Any,
```

### Comparing `fugue-0.8.4.dev1/fugue_dask/ibis_engine.py` & `fugue-0.8.4.dev2/fugue_dask/ibis_engine.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue_dask/registry.py` & `fugue-0.8.4.dev2/fugue_dask/registry.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue_duckdb/_io.py` & `fugue-0.8.4.dev2/fugue_duckdb/_io.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue_duckdb/_utils.py` & `fugue-0.8.4.dev2/fugue_duckdb/_utils.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue_duckdb/dask.py` & `fugue-0.8.4.dev2/fugue_duckdb/dask.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue_duckdb/dataframe.py` & `fugue-0.8.4.dev2/fugue_duckdb/dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue_duckdb/execution_engine.py` & `fugue-0.8.4.dev2/fugue_duckdb/execution_engine.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue_duckdb/ibis_engine.py` & `fugue-0.8.4.dev2/fugue_duckdb/ibis_engine.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue_duckdb/registry.py` & `fugue-0.8.4.dev2/fugue_duckdb/registry.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue_ibis/_utils.py` & `fugue-0.8.4.dev2/fugue_ibis/_utils.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue_ibis/dataframe.py` & `fugue-0.8.4.dev2/fugue_ibis/dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue_ibis/execution/ibis_engine.py` & `fugue-0.8.4.dev2/fugue_ibis/execution/ibis_engine.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue_ibis/execution/pandas_backend.py` & `fugue-0.8.4.dev2/fugue_ibis/execution/pandas_backend.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue_ibis/execution_engine.py` & `fugue-0.8.4.dev2/fugue_ibis/execution_engine.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue_ibis/extensions.py` & `fugue-0.8.4.dev2/fugue_ibis/extensions.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue_notebook/__init__.py` & `fugue-0.8.4.dev2/fugue_notebook/__init__.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue_notebook/env.py` & `fugue-0.8.4.dev2/fugue_notebook/env.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,22 @@
 # pylint: disable=W0611,W0613
 import html
 import json
 from typing import Any, Dict, List, Optional
 
-from IPython.core.magic import Magics, cell_magic, magics_class, needs_local_scope
 from IPython import get_ipython
+from IPython.core.magic import Magics, cell_magic, magics_class, needs_local_scope
 from IPython.display import HTML, display
 from triad import ParamDict
 from triad.utils.convert import to_instance
 from triad.utils.pyarrow import _field_to_expression
 
-import fugue_sql
-from fugue import (
-    DataFrame,
-    DataFrameDisplay,
-    ExecutionEngine,
-    get_dataset_display,
-    make_execution_engine,
-)
+from fugue import DataFrame, DataFrameDisplay, ExecutionEngine
+from fugue import fsql as fugue_sql
+from fugue import get_dataset_display, make_execution_engine
 from fugue.dataframe import YieldedDataFrame
 from fugue.exceptions import FugueSQLSyntaxError
 
 
 class NotebookSetup(object):
     """Jupyter notebook environment customization template."""
 
@@ -54,15 +49,15 @@
         self._post_conf = post_conf
         self._fsql_ignore_case = fsql_ignore_case
 
     @needs_local_scope
     @cell_magic("fsql")
     def fsql(self, line: str, cell: str, local_ns: Any = None) -> None:
         try:
-            dag = fugue_sql.fsql(
+            dag = fugue_sql(
                 "\n" + cell, local_ns, fsql_ignore_case=self._fsql_ignore_case
             )
         except FugueSQLSyntaxError as ex:
             raise FugueSQLSyntaxError(str(ex)).with_traceback(None) from None
         dag.run(self.get_engine(line, {} if local_ns is None else local_ns))
         for k, v in dag.yields.items():
             if isinstance(v, YieldedDataFrame):
```

### Comparing `fugue-0.8.4.dev1/fugue_notebook/nbextension/main.js` & `fugue-0.8.4.dev2/fugue_notebook/nbextension/main.js`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue_polars/_utils.py` & `fugue-0.8.4.dev2/fugue_polars/_utils.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue_polars/polars_dataframe.py` & `fugue-0.8.4.dev2/fugue_polars/polars_dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue_polars/registry.py` & `fugue-0.8.4.dev2/fugue_polars/registry.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue_ray/_constants.py` & `fugue-0.8.4.dev2/fugue_ray/_constants.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue_ray/_utils/cluster.py` & `fugue-0.8.4.dev2/fugue_ray/_utils/cluster.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue_ray/_utils/dataframe.py` & `fugue-0.8.4.dev2/fugue_ray/_utils/dataframe.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 
 def get_dataset_format(df: rd.Dataset) -> Optional[str]:
     df.fully_executed()
     if df.count() == 0:
         return None
     if hasattr(df, "_dataset_format"):  # pragma: no cover
         return df._dataset_format()  # ray<2.2
+    ctx = rd.context.DatasetContext.get_current()
+    ctx.use_streaming_executor = False
     return df.dataset_format()  # ray>=2.2
 
 
 def build_empty(schema: Schema) -> rd.Dataset:
     return rd.from_arrow(_build_empty_arrow(schema))
```

### Comparing `fugue-0.8.4.dev1/fugue_ray/_utils/io.py` & `fugue-0.8.4.dev2/fugue_ray/_utils/io.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue_ray/dataframe.py` & `fugue-0.8.4.dev2/fugue_ray/dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue_ray/execution_engine.py` & `fugue-0.8.4.dev2/fugue_ray/execution_engine.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from fugue.constants import KEYWORD_PARALLELISM, KEYWORD_ROWCOUNT
 from fugue.dataframe.arrow_dataframe import _build_empty_arrow
 from fugue_duckdb.dataframe import DuckDataFrame
 from fugue_duckdb.execution_engine import DuckExecutionEngine
 
 from ._constants import FUGUE_RAY_DEFAULT_BATCH_SIZE, FUGUE_RAY_ZERO_COPY
 from ._utils.cluster import get_default_partitions, get_default_shuffle_partitions
-from ._utils.dataframe import add_partition_key, add_coarse_partition_key
+from ._utils.dataframe import add_coarse_partition_key, add_partition_key
 from ._utils.io import RayIO
 from .dataframe import RayDataFrame
 
 _RAY_PARTITION_KEY = "__ray_partition_key__"
 
 
 class RayMapEngine(MapEngine):
@@ -211,14 +211,15 @@
     """
 
     def __init__(
         self, conf: Any = None, connection: Optional[DuckDBPyConnection] = None
     ):
         if not ray.is_initialized():  # pragma: no cover
             ray.init()
+
         super().__init__(conf, connection)
         self._io = RayIO(self)
 
     def __repr__(self) -> str:
         return "RayExecutionEngine"
 
     @property
@@ -276,14 +277,24 @@
         return df  # pragma: no cover
 
     def convert_yield_dataframe(self, df: DataFrame, as_local: bool) -> DataFrame:
         if isinstance(df, RayDataFrame):
             return df if not as_local else df.as_local()
         return super().convert_yield_dataframe(df, as_local)
 
+    def union(self, df1: DataFrame, df2: DataFrame, distinct: bool = True) -> DataFrame:
+        if distinct:
+            return super().union(df1, df2, distinct)
+        assert_or_throw(
+            df1.schema == df2.schema, ValueError(f"{df1.schema} != {df2.schema}")
+        )
+        tdf1 = self._to_ray_df(df1)
+        tdf2 = self._to_ray_df(df2)
+        return RayDataFrame(tdf1.native.union(tdf2.native), df1.schema)
+
     def load_df(  # type:ignore
         self,
         path: Union[str, List[str]],
         format_hint: Any = None,
         columns: Any = None,
         **kwargs: Any,
     ) -> DataFrame:
```

### Comparing `fugue-0.8.4.dev1/fugue_ray/registry.py` & `fugue-0.8.4.dev2/fugue_ray/registry.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue_spark/_utils/convert.py` & `fugue-0.8.4.dev2/fugue_spark/_utils/convert.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,30 +7,31 @@
 import pyspark.sql.types as pt
 from pyarrow.types import is_list, is_struct, is_timestamp
 from pyspark.sql.pandas.types import from_arrow_type, to_arrow_type
 from triad.collections import Schema
 from triad.utils.assertion import assert_arg_not_none, assert_or_throw
 from triad.utils.pyarrow import TRIAD_DEFAULT_TIMESTAMP
 from triad.utils.schema import quote_name
+from .misc import is_spark_dataframe
 
 
 def to_spark_schema(obj: Any) -> pt.StructType:
     assert_arg_not_none(obj, "schema")
     if isinstance(obj, pt.StructType):
         return obj
-    if isinstance(obj, ps.DataFrame):
+    if is_spark_dataframe(obj):
         return obj.schema
     return _from_arrow_schema(Schema(obj).pa_schema)
 
 
 def to_schema(obj: Any) -> Schema:
     assert_arg_not_none(obj, "obj")
     if isinstance(obj, pt.StructType):
         return Schema(_to_arrow_schema(obj))
-    if isinstance(obj, ps.DataFrame):
+    if is_spark_dataframe(obj):
         return to_schema(obj.schema)
     return Schema(obj)
 
 
 def to_cast_expression(
     schema1: Any, schema2: Any, allow_name_mismatch: bool
 ) -> Tuple[bool, List[str]]:
```

### Comparing `fugue-0.8.4.dev1/fugue_spark/_utils/io.py` & `fugue-0.8.4.dev2/fugue_spark/_utils/io.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue_spark/_utils/partition.py` & `fugue-0.8.4.dev2/fugue_spark/_utils/partition.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-import random
 from typing import Any, Iterable, List
 
 import pyspark.sql as ps
+import pyspark.sql.functions as psf
 from pyspark import RDD
 from pyspark.sql import SparkSession
-from pyspark.sql.functions import lit
-
-from fugue_spark._utils.convert import to_schema, to_spark_schema
+import warnings
+from .convert import to_schema, to_spark_schema
+from .misc import is_spark_connect
 
 _PARTITION_DUMMY_KEY = "__partition_dummy_key__"
 
 
 def hash_repartition(
     session: SparkSession, df: ps.DataFrame, num: int, cols: List[Any]
 ) -> ps.DataFrame:
@@ -25,31 +25,28 @@
 
 def rand_repartition(
     session: SparkSession, df: ps.DataFrame, num: int, cols: List[Any]
 ) -> ps.DataFrame:
     if len(cols) > 0 or num <= 1:
         return hash_repartition(session, df, num, cols)
 
-    def _rand(rows: Iterable[Any], n: int) -> Iterable[Any]:  # pragma: no cover
-        for row in rows:
-            yield (random.randint(0, n - 1), row)
-
-    rdd = (
-        df.rdd.mapPartitions(lambda r: _rand(r, num))
-        .partitionBy(num, lambda k: k)
-        .mapPartitions(_to_rows)
+    tdf = df.withColumn(
+        _PARTITION_DUMMY_KEY, (psf.rand(0) * psf.lit(2**15 - 1)).cast("long")
     )
-    return session.createDataFrame(rdd, df.schema)
+    return tdf.repartition(num, _PARTITION_DUMMY_KEY)[df.schema.names]
 
 
 def even_repartition(
     session: SparkSession, df: ps.DataFrame, num: int, cols: List[Any]
 ) -> ps.DataFrame:
     if num == 1:
         return _single_repartition(df)
+    if is_spark_connect(session):  # pragma: no cover
+        warnings.warn("Even repartitioning is not supported by Spark Connect")
+        return hash_repartition(session, df, num, cols)
     if len(cols) == 0:
         if num == 0:
             return df
         rdd = (
             _zipWithIndex(df.rdd).partitionBy(num, lambda k: k).mapPartitions(_to_rows)
         )
         return session.createDataFrame(rdd, df.schema)
@@ -79,30 +76,25 @@
             .mapPartitions(_to_rows)
         )
         return session.createDataFrame(rdd, df.schema)
 
 
 def _single_repartition(df: ps.DataFrame) -> ps.DataFrame:
     return (
-        df.withColumn(_PARTITION_DUMMY_KEY, lit(0))
+        df.withColumn(_PARTITION_DUMMY_KEY, psf.lit(0))
         .repartition(_PARTITION_DUMMY_KEY)
         .drop(_PARTITION_DUMMY_KEY)
     )
 
 
 def _to_rows(rdd: Iterable[Any]) -> Iterable[Any]:  # pragma: no cover
     for item in rdd:
         yield item[1]
 
 
-def _to_rows_with_key(rdd: Iterable[Any]) -> Iterable[Any]:  # pragma: no cover
-    for item in rdd:
-        yield list(item[1]) + [item[0]]
-
-
 def _zipWithIndex(rdd: RDD, to_rows: bool = False) -> RDD:
     """
     Modified from
     https://github.com/davies/spark/blob/cebe5bfe263baf3349353f1473f097396821514a/python/pyspark/rdd.py
 
     """
     starts = [0]
```

### Comparing `fugue-0.8.4.dev1/fugue_spark/dataframe.py` & `fugue-0.8.4.dev2/fugue_spark/dataframe.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,20 +26,17 @@
     is_bounded,
     is_df,
     is_empty,
     is_local,
     rename,
     select_columns,
 )
-from fugue_spark._utils.convert import (
-    to_cast_expression,
-    to_pandas,
-    to_schema,
-    to_type_safe_input,
-)
+
+from ._utils.convert import to_cast_expression, to_pandas, to_schema, to_type_safe_input
+from ._utils.misc import is_spark_connect, is_spark_dataframe
 
 
 class SparkDataFrame(DataFrame):
     """DataFrame that wraps Spark DataFrame. Please also read
     |DataFrameTutorial| to understand this Fugue concept
 
     :param df: :class:`spark:pyspark.sql.DataFrame`
@@ -52,20 +49,20 @@
           instead of construction it by yourself.
         * If ``schema`` is set, then there will be type cast on the Spark DataFrame if
           the schema is different.
     """
 
     def __init__(self, df: Any = None, schema: Any = None):  # noqa: C901
         self._lock = SerializableRLock()
-        if isinstance(df, ps.DataFrame):
+        if is_spark_dataframe(df):
             if schema is not None:
                 schema = to_schema(schema).assert_not_empty()
                 has_cast, expr = to_cast_expression(df, schema, True)
                 if has_cast:
-                    df = df.selectExpr(*expr)
+                    df = df.selectExpr(*expr)  # type: ignore
             else:
                 schema = to_schema(df).assert_not_empty()
             self._native = df
             super().__init__(schema)
         else:  # pragma: no cover
             assert_or_throw(schema is not None, SchemaError("schema is None"))
             schema = to_schema(schema).assert_not_empty()
@@ -151,14 +148,17 @@
     ) -> List[Any]:
         sdf = self._select_columns(columns)
         return sdf.as_local().as_array(type_safe=type_safe)
 
     def as_array_iterable(
         self, columns: Optional[List[str]] = None, type_safe: bool = False
     ) -> Iterable[Any]:
+        if is_spark_connect(self.native):  # pragma: no cover
+            yield from self.as_array(columns, type_safe=type_safe)
+            return
         sdf = self._select_columns(columns)
         if not type_safe:
             for row in to_type_safe_input(sdf.native.rdd.toLocalIterator(), sdf.schema):
                 yield row
         else:
             df = IterableDataFrame(sdf.as_array_iterable(type_safe=False), sdf.schema)
             for row in df.as_array_iterable(type_safe=True):
@@ -183,87 +183,87 @@
 
     def _select_columns(self, columns: Optional[List[str]]) -> "SparkDataFrame":
         if columns is None:
             return self
         return SparkDataFrame(self.native.select(*columns))
 
 
-@is_df.candidate(lambda df: isinstance(df, ps.DataFrame))
+@is_df.candidate(lambda df: is_spark_dataframe(df))
 def _spark_is_df(df: ps.DataFrame) -> bool:
     return True
 
 
-@get_num_partitions.candidate(lambda df: isinstance(df, ps.DataFrame))
+@get_num_partitions.candidate(lambda df: is_spark_dataframe(df))
 def _spark_num_partitions(df: ps.DataFrame) -> int:
     return df.rdd.getNumPartitions()
 
 
-@count.candidate(lambda df: isinstance(df, ps.DataFrame))
+@count.candidate(lambda df: is_spark_dataframe(df))
 def _spark_df_count(df: ps.DataFrame) -> int:
     return df.count()
 
 
-@is_bounded.candidate(lambda df: isinstance(df, ps.DataFrame))
+@is_bounded.candidate(lambda df: is_spark_dataframe(df))
 def _spark_df_is_bounded(df: ps.DataFrame) -> bool:
     return True
 
 
-@is_empty.candidate(lambda df: isinstance(df, ps.DataFrame))
+@is_empty.candidate(lambda df: is_spark_dataframe(df))
 def _spark_df_is_empty(df: ps.DataFrame) -> bool:
     return df.first() is None
 
 
-@is_local.candidate(lambda df: isinstance(df, ps.DataFrame))
+@is_local.candidate(lambda df: is_spark_dataframe(df))
 def _spark_df_is_local(df: ps.DataFrame) -> bool:
     return False
 
 
-@as_local_bounded.candidate(lambda df: isinstance(df, ps.DataFrame))
+@as_local_bounded.candidate(lambda df: is_spark_dataframe(df))
 def _spark_df_as_local(df: ps.DataFrame) -> pd.DataFrame:
     return to_pandas(df)
 
 
-@get_column_names.candidate(lambda df: isinstance(df, ps.DataFrame))
+@get_column_names.candidate(lambda df: is_spark_dataframe(df))
 def _get_spark_df_columns(df: ps.DataFrame) -> List[Any]:
     return df.columns
 
 
-@rename.candidate(lambda df, *args, **kwargs: isinstance(df, ps.DataFrame))
+@rename.candidate(lambda df, *args, **kwargs: is_spark_dataframe(df))
 def _rename_spark_df(
     df: ps.DataFrame, columns: Dict[str, Any], as_fugue: bool = False
 ) -> ps.DataFrame:
     if len(columns) == 0:
         return df
     _assert_no_missing(df, columns.keys())
     return _adjust_df(_rename_spark_dataframe(df, columns), as_fugue=as_fugue)
 
 
-@drop_columns.candidate(lambda df, *args, **kwargs: isinstance(df, ps.DataFrame))
+@drop_columns.candidate(lambda df, *args, **kwargs: is_spark_dataframe(df))
 def _drop_spark_df_columns(
     df: ps.DataFrame, columns: List[str], as_fugue: bool = False
 ) -> Any:
     cols = [x for x in df.columns if x not in columns]
     if len(cols) == 0:
         raise FugueDataFrameOperationError("cannot drop all columns")
     if len(cols) + len(columns) != len(df.columns):
         _assert_no_missing(df, columns)
     return _adjust_df(df[cols], as_fugue=as_fugue)
 
 
-@select_columns.candidate(lambda df, *args, **kwargs: isinstance(df, ps.DataFrame))
+@select_columns.candidate(lambda df, *args, **kwargs: is_spark_dataframe(df))
 def _select_spark_df_columns(
     df: ps.DataFrame, columns: List[Any], as_fugue: bool = False
 ) -> Any:
     if len(columns) == 0:
         raise FugueDataFrameOperationError("must select at least one column")
     _assert_no_missing(df, columns)
     return _adjust_df(df[columns], as_fugue=as_fugue)
 
 
-@head.candidate(lambda df, *args, **kwargs: isinstance(df, ps.DataFrame))
+@head.candidate(lambda df, *args, **kwargs: is_spark_dataframe(df))
 def _spark_df_head(
     df: ps.DataFrame,
     n: int,
     columns: Optional[List[str]] = None,
     as_fugue: bool = False,
 ) -> pd.DataFrame:
     if columns is not None:
```

### Comparing `fugue-0.8.4.dev1/fugue_spark/execution_engine.py` & `fugue-0.8.4.dev2/fugue_spark/execution_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 from fugue.dataframe.utils import get_join_schemas
 from fugue.exceptions import FugueDataFrameInitError
 from fugue.execution.execution_engine import ExecutionEngine, MapEngine, SQLEngine
 
 from ._constants import FUGUE_SPARK_CONF_USE_PANDAS_UDF, FUGUE_SPARK_DEFAULT_CONF
 from ._utils.convert import to_schema, to_spark_schema, to_type_safe_input
 from ._utils.io import SparkIO
+from ._utils.misc import is_spark_connect as _is_spark_connect, is_spark_dataframe
 from ._utils.partition import even_repartition, hash_repartition, rand_repartition
 from .dataframe import SparkDataFrame
 
 _TO_SPARK_JOIN_MAP: Dict[str, str] = {
     "inner": "inner",
     "leftouter": "left_outer",
     "rightouter": "right_outer",
@@ -92,15 +93,22 @@
 
 
 class SparkMapEngine(MapEngine):
     @property
     def is_distributed(self) -> bool:
         return True
 
+    @property
+    def is_spark_connect(self) -> bool:
+        """Whether the spark session is created by spark connect"""
+        return self.execution_engine.is_spark_connect  # type:ignore
+
     def _should_use_pandas_udf(self, schema: Schema) -> bool:
+        if self.is_spark_connect:  # pragma: no cover
+            return True
         possible = hasattr(ps.DataFrame, "mapInPandas")  # must be new version of Spark
         # else:  # this condition seems to be unnecessary
         #    possible &= self.execution_engine.conf.get(
         #        "spark.sql.execution.arrow.pyspark.enabled", False
         #    )
         enabled = self.execution_engine.conf.get_or_throw(
             FUGUE_SPARK_CONF_USE_PANDAS_UDF, bool
@@ -133,15 +141,15 @@
                         df,
                         map_func=map_func,
                         output_schema=output_schema,
                         partition_spec=partition_spec,
                         on_init=on_init,
                         map_func_format_hint=map_func_format_hint,
                     )
-                elif partition_spec.algo != "even":
+                elif partition_spec.algo != "even" or self.is_spark_connect:
                     return self._group_map_by_pandas_udf(
                         df,
                         map_func=map_func,
                         output_schema=output_schema,
                         partition_spec=partition_spec,
                         on_init=on_init,
                         map_func_format_hint=map_func_format_hint,
@@ -311,15 +319,18 @@
     """
 
     def __init__(self, spark_session: Optional[SparkSession] = None, conf: Any = None):
         if spark_session is None:
             spark_session = SparkSession.builder.getOrCreate()
         self._spark_session = spark_session
         cf = dict(FUGUE_SPARK_DEFAULT_CONF)
-        cf.update({x[0]: x[1] for x in spark_session.sparkContext.getConf().getAll()})
+        if not self.is_spark_connect:
+            cf.update(
+                {x[0]: x[1] for x in spark_session.sparkContext.getConf().getAll()}
+            )
         cf.update(ParamDict(conf))
         super().__init__(cf)
         self._lock = SerializableRLock()
         self._fs = FileSystem()
         self._log = logging.getLogger()
         self._broadcast_func = RunOnce(
             self._broadcast, lambda *args, **kwargs: id(args[0])
@@ -339,14 +350,18 @@
         """
         assert_or_throw(
             self._spark_session is not None, "SparkExecutionEngine is not started"
         )
         return self._spark_session
 
     @property
+    def is_spark_connect(self) -> bool:
+        return _is_spark_connect(self.spark_session)
+
+    @property
     def is_distributed(self) -> bool:
         return True
 
     @property
     def log(self) -> logging.Logger:
         return self._log
 
@@ -358,14 +373,19 @@
         return SparkSQLEngine(self)
 
     def create_default_map_engine(self) -> MapEngine:
         return SparkMapEngine(self)
 
     def get_current_parallelism(self) -> int:
         spark = self.spark_session
+        if self.is_spark_connect:  # pragma: no cover
+            num = spark.conf.get("spark.default.parallelism", "")
+            if num != "":
+                return int(num)
+            return int(spark.conf.get("spark.sql.shuffle.partitions", "200"))
         e_cores = int(spark.conf.get("spark.executor.cores", "1"))
         tc = int(spark.conf.get("spark.task.cpus", "1"))
         sc = spark._jsc.sc()
         try:
             return spark.sparkContext.defaultParallelism // tc
         except Exception:  # pragma: no cover
             # for pyspark < 3.1.1
@@ -731,15 +751,15 @@
                         df.as_array(type_safe=True), to_spark_schema(df.schema)
                     )
                 else:
                     sdf = self.spark_session.createDataFrame(
                         df.as_pandas(), to_spark_schema(df.schema)
                     )
                 return SparkDataFrame(sdf, df.schema)
-            if isinstance(df, ps.DataFrame):
+            if is_spark_dataframe(df):
                 return SparkDataFrame(df, None if schema is None else to_schema(schema))
             if isinstance(df, RDD):
                 assert_arg_not_none(schema, "schema")
                 sdf = self.spark_session.createDataFrame(df, to_spark_schema(schema))
                 return SparkDataFrame(sdf, to_schema(schema))
             if isinstance(df, pd.DataFrame):
                 if PD_UTILS.empty(df):
```

### Comparing `fugue-0.8.4.dev1/fugue_spark/ibis_engine.py` & `fugue-0.8.4.dev2/fugue_spark/ibis_engine.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue_spark/registry.py` & `fugue-0.8.4.dev2/fugue_spark/registry.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,26 +14,32 @@
     is_pandas_or,
 )
 from fugue.extensions import namespace_candidate
 from fugue.plugins import as_fugue_dataset, infer_execution_engine, parse_creator
 from fugue_spark.dataframe import SparkDataFrame
 from fugue_spark.execution_engine import SparkExecutionEngine
 
+from ._utils.misc import SparkConnectDataFrame, SparkConnectSession, is_spark_dataframe
+
 _is_sparksql = namespace_candidate("sparksql", lambda x: isinstance(x, str))
 
 
 @infer_execution_engine.candidate(
-    lambda objs: is_pandas_or(objs, (ps.DataFrame, SparkDataFrame))
+    lambda objs: (
+        is_pandas_or(objs, (ps.DataFrame, SparkConnectDataFrame, SparkDataFrame))
+        if SparkConnectDataFrame is not None
+        else is_pandas_or(objs, (ps.DataFrame, SparkDataFrame))
+    )
     or any(_is_sparksql(obj) for obj in objs)
 )
 def _infer_spark_client(obj: Any) -> Any:
     return SparkSession.builder.getOrCreate()
 
 
-@as_fugue_dataset.candidate(lambda df, **kwargs: isinstance(df, ps.DataFrame))
+@as_fugue_dataset.candidate(lambda df, **kwargs: is_spark_dataframe(df))
 def _spark_as_fugue_df(df: ps.DataFrame, **kwargs: Any) -> SparkDataFrame:
     return SparkDataFrame(df, **kwargs)
 
 
 @parse_creator.candidate(_is_sparksql)
 def _parse_sparksql_creator(sql: Tuple[str, str]):
     def _run_sql(spark: SparkSession) -> ps.DataFrame:
@@ -49,14 +55,20 @@
         on_dup="ignore",
     )
     register_execution_engine(
         SparkSession,
         lambda session, conf, **kwargs: SparkExecutionEngine(session, conf=conf),
         on_dup="ignore",
     )
+    if SparkConnectSession is not None:
+        register_execution_engine(
+            SparkConnectSession,
+            lambda session, conf, **kwargs: SparkExecutionEngine(session, conf=conf),
+            on_dup="ignore",
+        )
 
 
 @fugue_annotated_param(SparkExecutionEngine)
 class _SparkExecutionEngineParam(ExecutionEngineParam):
     pass
 
 
@@ -77,15 +89,15 @@
 @fugue_annotated_param(ps.DataFrame)
 class _SparkDataFrameParam(DataFrameParam):
     def to_input_data(self, df: DataFrame, ctx: Any) -> Any:
         assert isinstance(ctx, SparkExecutionEngine)
         return ctx.to_df(df).native
 
     def to_output_df(self, output: Any, schema: Any, ctx: Any) -> DataFrame:
-        assert isinstance(output, ps.DataFrame)
+        assert is_spark_dataframe(output)
         assert isinstance(ctx, SparkExecutionEngine)
         return ctx.to_df(output, schema=schema)
 
     def count(self, df: Any) -> int:  # pragma: no cover
         raise NotImplementedError("not allowed")
```

### Comparing `fugue-0.8.4.dev1/fugue_test/bag_suite.py` & `fugue-0.8.4.dev2/fugue_test/bag_suite.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue_test/builtin_suite.py` & `fugue-0.8.4.dev2/fugue_test/builtin_suite.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue_test/dataframe_suite.py` & `fugue-0.8.4.dev2/fugue_test/dataframe_suite.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue_test/execution_suite.py` & `fugue-0.8.4.dev2/fugue_test/execution_suite.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/fugue_test/ibis_suite.py` & `fugue-0.8.4.dev2/fugue_test/ibis_suite.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/setup.cfg` & `fugue-0.8.4.dev2/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 	--cov=fugue_test
 	--cov=fugue_spark
 	--cov=fugue_dask
 	--cov=fugue_ray
 	--cov=fugue_duckdb
 	--cov=fugue_ibis
 	--cov=fugue_polars
+	--ignore=tests/fugue_spark/test_spark_connect.py
 	--cov-report=term-missing:skip-covered
 	-vvv
 spark_options = 
 	spark.master: local[*]
 	spark.sql.catalogImplementation: in-memory
 	spark.sql.shuffle.partitions: 4
 	spark.default.parallelism: 4
```

### Comparing `fugue-0.8.4.dev1/setup.py` & `fugue-0.8.4.dev2/setup.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/tests/fugue/bag/test_array_bag.py` & `fugue-0.8.4.dev2/tests/fugue/bag/test_array_bag.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/tests/fugue/collections/test_partition.py` & `fugue-0.8.4.dev2/tests/fugue/collections/test_partition.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/tests/fugue/collections/test_sql.py` & `fugue-0.8.4.dev2/tests/fugue/collections/test_sql.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/tests/fugue/column/test_expressions.py` & `fugue-0.8.4.dev2/tests/fugue/column/test_expressions.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/tests/fugue/column/test_functions.py` & `fugue-0.8.4.dev2/tests/fugue/column/test_functions.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/tests/fugue/column/test_sql.py` & `fugue-0.8.4.dev2/tests/fugue/column/test_sql.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/tests/fugue/dataframe/test_array_dataframe.py` & `fugue-0.8.4.dev2/tests/fugue/dataframe/test_array_dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/tests/fugue/dataframe/test_arrow_dataframe.py` & `fugue-0.8.4.dev2/tests/fugue/dataframe/test_arrow_dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/tests/fugue/dataframe/test_dataframe.py` & `fugue-0.8.4.dev2/tests/fugue/dataframe/test_dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/tests/fugue/dataframe/test_dataframe_iterable_dataframe.py` & `fugue-0.8.4.dev2/tests/fugue/dataframe/test_dataframe_iterable_dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/tests/fugue/dataframe/test_dataframes.py` & `fugue-0.8.4.dev2/tests/fugue/dataframe/test_dataframes.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/tests/fugue/dataframe/test_function_wrapper.py` & `fugue-0.8.4.dev2/tests/fugue/dataframe/test_function_wrapper.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/tests/fugue/dataframe/test_iterable_dataframe.py` & `fugue-0.8.4.dev2/tests/fugue/dataframe/test_iterable_dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/tests/fugue/dataframe/test_pandas_dataframe.py` & `fugue-0.8.4.dev2/tests/fugue/dataframe/test_pandas_dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/tests/fugue/dataframe/test_utils.py` & `fugue-0.8.4.dev2/tests/fugue/dataframe/test_utils.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/tests/fugue/execution/test_api.py` & `fugue-0.8.4.dev2/tests/fugue/execution/test_api.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/tests/fugue/execution/test_execution_engine.py` & `fugue-0.8.4.dev2/tests/fugue/execution/test_execution_engine.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/tests/fugue/execution/test_factory.py` & `fugue-0.8.4.dev2/tests/fugue/execution/test_factory.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/tests/fugue/execution/test_ibis.py` & `fugue-0.8.4.dev2/tests/fugue/execution/test_ibis.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/tests/fugue/execution/test_naive_execution_engine.py` & `fugue-0.8.4.dev2/tests/fugue/execution/test_naive_execution_engine.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/tests/fugue/extensions/creator/__init__.py` & `fugue-0.8.4.dev2/tests/fugue/extensions/creator/__init__.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/tests/fugue/extensions/creator/test_convert.py` & `fugue-0.8.4.dev2/tests/fugue/extensions/creator/test_convert.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/tests/fugue/extensions/outputter/__init__.py` & `fugue-0.8.4.dev2/tests/fugue/extensions/outputter/__init__.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/tests/fugue/extensions/outputter/test_convert.py` & `fugue-0.8.4.dev2/tests/fugue/extensions/outputter/test_convert.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/tests/fugue/extensions/processor/__init__.py` & `fugue-0.8.4.dev2/tests/fugue/extensions/processor/__init__.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/tests/fugue/extensions/processor/test_convert.py` & `fugue-0.8.4.dev2/tests/fugue/extensions/processor/test_convert.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/tests/fugue/extensions/test_utils.py` & `fugue-0.8.4.dev2/tests/fugue/extensions/test_utils.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/tests/fugue/extensions/transformer/test_convert_cotransformer.py` & `fugue-0.8.4.dev2/tests/fugue/extensions/transformer/test_convert_cotransformer.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/tests/fugue/extensions/transformer/test_convert_output_cotransformer.py` & `fugue-0.8.4.dev2/tests/fugue/extensions/transformer/test_convert_output_cotransformer.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/tests/fugue/extensions/transformer/test_convert_output_transformer.py` & `fugue-0.8.4.dev2/tests/fugue/extensions/transformer/test_convert_output_transformer.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/tests/fugue/extensions/transformer/test_convert_transformer.py` & `fugue-0.8.4.dev2/tests/fugue/extensions/transformer/test_convert_transformer.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/tests/fugue/rpc/test_base.py` & `fugue-0.8.4.dev2/tests/fugue/rpc/test_base.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/tests/fugue/rpc/test_flask.py` & `fugue-0.8.4.dev2/tests/fugue/rpc/test_flask.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/tests/fugue/rpc/test_func.py` & `fugue-0.8.4.dev2/tests/fugue/rpc/test_func.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/tests/fugue/sql/test_utils.py` & `fugue-0.8.4.dev2/tests/fugue/sql/test_utils.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/tests/fugue/sql/test_visitors.py` & `fugue-0.8.4.dev2/tests/fugue/sql/test_visitors.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/tests/fugue/sql/test_workflow.py` & `fugue-0.8.4.dev2/tests/fugue/sql/test_workflow.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/tests/fugue/sql/test_workflow_parse.py` & `fugue-0.8.4.dev2/tests/fugue/sql/test_workflow_parse.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/tests/fugue/test_interfaceless.py` & `fugue-0.8.4.dev2/tests/fugue/test_interfaceless.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/tests/fugue/utils/test_interfaceless.py` & `fugue-0.8.4.dev2/tests/fugue/utils/test_interfaceless.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/tests/fugue/utils/test_io.py` & `fugue-0.8.4.dev2/tests/fugue/utils/test_io.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/tests/fugue/workflow/test_module.py` & `fugue-0.8.4.dev2/tests/fugue/workflow/test_module.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/tests/fugue/workflow/test_runtime_exception.py` & `fugue-0.8.4.dev2/tests/fugue/workflow/test_runtime_exception.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/tests/fugue/workflow/test_workflow.py` & `fugue-0.8.4.dev2/tests/fugue/workflow/test_workflow.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/tests/fugue/workflow/test_workflow_determinism.py` & `fugue-0.8.4.dev2/tests/fugue/workflow/test_workflow_determinism.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/tests/fugue/workflow/test_workflow_parallel.py` & `fugue-0.8.4.dev2/tests/fugue/workflow/test_workflow_parallel.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/tests/fugue_dask/test_dataframe.py` & `fugue-0.8.4.dev2/tests/fugue_dask/test_dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/tests/fugue_dask/test_execution_engine.py` & `fugue-0.8.4.dev2/tests/fugue_dask/test_execution_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,17 +117,19 @@
         assert isinstance(infer_execution_engine([fdf]), Client)
 
 
 class DaskExecutionEngineBuiltInTests(BuiltInTests.Tests):
     @classmethod
     def setUpClass(cls):
         cls._engine = cls.make_engine(cls)
+        fa.set_global_engine(cls._engine)
 
     @classmethod
     def tearDownClass(cls):
+        fa.clear_global_engine()
         cls._engine.dask_client.close()
 
     def make_engine(self):
         e = DaskExecutionEngine(conf=dict(test=True, **_CONF))
         return e
 
     def test_yield_table(self):
@@ -149,14 +151,26 @@
 
         with FugueWorkflow() as dag:
             df = dag.create(m_c).process(m_p)
             df.assert_eq(dag.df([[0]], "a:long"))
             df.output(m_o)
         dag.run(self.engine)
 
+    def test_bool_bytes_union(self):
+        # this is to verify a bug in enforce type is fixed
+        def tr(df: pd.DataFrame) -> pd.DataFrame:
+            return df.assign(data=b"asdf")
+
+        df = pd.DataFrame(dict(a=[True, False], b=[1, 2]))
+
+        r1 = fa.transform(df, tr, schema="*,data:bytes", as_fugue=True)
+        r2 = fa.transform(df, tr, schema="*,data:bytes", as_fugue=True)
+        r3 = fa.union(r1, r2, distinct=False)
+        r3.show()
+
     def test_coarse_partition(self):
         def verify_coarse_partition(df: pd.DataFrame) -> List[List[Any]]:
             ct = df.a.nunique()
             s = df.a * 1000 + df.b
             ordered = ((s - s.shift(1)).dropna() >= 0).all(axis=None)
             return [[ct, ordered]]
```

### Comparing `fugue-0.8.4.dev1/tests/fugue_dask/test_importless.py` & `fugue-0.8.4.dev2/tests/fugue_dask/test_importless.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/tests/fugue_dask/test_io.py` & `fugue-0.8.4.dev2/tests/fugue_dask/test_io.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/tests/fugue_dask/test_sql.py` & `fugue-0.8.4.dev2/tests/fugue_dask/test_sql.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/tests/fugue_duckdb/test_dask.py` & `fugue-0.8.4.dev2/tests/fugue_duckdb/test_dask.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/tests/fugue_duckdb/test_dataframe.py` & `fugue-0.8.4.dev2/tests/fugue_duckdb/test_dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/tests/fugue_duckdb/test_execution_engine.py` & `fugue-0.8.4.dev2/tests/fugue_duckdb/test_execution_engine.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/tests/fugue_duckdb/test_ibis.py` & `fugue-0.8.4.dev2/tests/fugue_duckdb/test_ibis.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/tests/fugue_duckdb/test_importless.py` & `fugue-0.8.4.dev2/tests/fugue_duckdb/test_importless.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/tests/fugue_duckdb/test_utils.py` & `fugue-0.8.4.dev2/tests/fugue_duckdb/test_utils.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/tests/fugue_ibis/mock/dataframe.py` & `fugue-0.8.4.dev2/tests/fugue_ibis/mock/dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/tests/fugue_ibis/mock/execution_engine.py` & `fugue-0.8.4.dev2/tests/fugue_ibis/mock/execution_engine.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/tests/fugue_ibis/test_dataframe.py` & `fugue-0.8.4.dev2/tests/fugue_ibis/test_dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/tests/fugue_ibis/test_execution_engine.py` & `fugue-0.8.4.dev2/tests/fugue_ibis/test_execution_engine.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/tests/fugue_ibis/test_extensions.py` & `fugue-0.8.4.dev2/tests/fugue_ibis/test_extensions.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/tests/fugue_ibis/test_utils.py` & `fugue-0.8.4.dev2/tests/fugue_ibis/test_utils.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/tests/fugue_polars/test_dataframe.py` & `fugue-0.8.4.dev2/tests/fugue_polars/test_dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/tests/fugue_polars/test_transform.py` & `fugue-0.8.4.dev2/tests/fugue_polars/test_transform.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/tests/fugue_ray/test_dataframe.py` & `fugue-0.8.4.dev2/tests/fugue_ray/test_dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/tests/fugue_ray/test_execution_engine.py` & `fugue-0.8.4.dev2/tests/fugue_ray/test_execution_engine.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/tests/fugue_ray/test_registry.py` & `fugue-0.8.4.dev2/tests/fugue_ray/test_registry.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/tests/fugue_ray/test_utils.py` & `fugue-0.8.4.dev2/tests/fugue_ray/test_utils.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/tests/fugue_spark/test_dataframe.py` & `fugue-0.8.4.dev2/tests/fugue_spark/test_dataframe.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/tests/fugue_spark/test_execution_engine.py` & `fugue-0.8.4.dev2/tests/fugue_spark/test_execution_engine.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     PandasDataFrame,
 )
 from fugue.dataframe.utils import _df_eq as df_eq
 from fugue.extensions.transformer import Transformer, transformer
 from fugue.plugins import infer_execution_engine
 from fugue.workflow.workflow import FugueWorkflow
 from fugue_spark._utils.convert import to_pandas
+from fugue_spark._utils.misc import is_spark_dataframe, is_spark_session
 from fugue_spark.dataframe import SparkDataFrame
 from fugue_spark.execution_engine import SparkExecutionEngine
 from fugue_test.builtin_suite import BuiltInTests
 from fugue_test.execution_suite import ExecutionEngineTests
 
 
 class SparkExecutionEngineTests(ExecutionEngineTests.Tests):
@@ -117,18 +118,18 @@
             engine.sample(a, n=90, replace=True)
 
         b = engine.sample(a, n=90)
         assert abs(len(b.as_array()) - 90) < 2
 
     def test_infer_engine(self):
         df = self.spark_session.createDataFrame(pd.DataFrame([[0]], columns=["a"]))
-        assert isinstance(infer_execution_engine([df]), SparkSession)
+        assert is_spark_session(infer_execution_engine([df]))
 
         fdf = SparkDataFrame(df)
-        assert isinstance(infer_execution_engine([fdf]), SparkSession)
+        assert is_spark_session(infer_execution_engine([fdf]))
 
 
 class SparkExecutionEnginePandasUDFTests(ExecutionEngineTests.Tests):
     @pytest.fixture(autouse=True)
     def init_session(self, spark_session):
         self.spark_session = spark_session
 
@@ -294,28 +295,28 @@
                 params=dict(rc=partition_num, n=gps, check_ordered=True),
             )
         dag.run(self.engine)
 
     def test_session_as_engine(self):
         dag = FugueWorkflow()
         a = dag.df([[p, 0] for p in range(100)], "a:int,b:int")
-        a.partition(algo="even", by=["a"]).transform(AssertMaxNTransform).persist()
+        # a.partition(algo="even", by=["a"]).transform(AssertMaxNTransform).persist()
         dag.run(self.spark_session)
 
     def test_interfaceless(self):
         sdf = self.spark_session.createDataFrame(
             [[1, 10], [0, 0], [1, 1], [0, 20]], "a int,b int"
         )
 
         # schema:*
         def f1(df: pd.DataFrame) -> pd.DataFrame:
             return df.sort_values("b").head(1)
 
         result = transform(sdf, f1, partition=dict(by=["a"]), engine=self.engine)
-        assert isinstance(result, SDataFrame)
+        assert is_spark_dataframe(result)
         assert to_pandas(result).sort_values(["a"]).values.tolist() == [[0, 0], [1, 1]]
 
     def test_annotation_1(self):
         def m_c(engine: SparkExecutionEngine) -> ps.DataFrame:
             return engine.spark_session.createDataFrame([[0]], "a:long")
 
         def m_p(engine: SparkExecutionEngine, df: ps.DataFrame) -> ps.DataFrame:
@@ -331,19 +332,19 @@
         dag.run(self.engine)
 
     def test_annotation_2(self):
         def m_c(session: SparkSession) -> ps.DataFrame:
             return session.createDataFrame([[0]], "a:long")
 
         def m_p(session: SparkSession, df: ps.DataFrame) -> ps.DataFrame:
-            assert isinstance(session, SparkSession)
+            assert is_spark_session(session)
             return df
 
         def m_o(session: SparkSession, df: ps.DataFrame) -> None:
-            assert isinstance(session, SparkSession)
+            assert is_spark_session(session)
             assert 1 == to_pandas(df).shape[0]
 
         with FugueWorkflow() as dag:
             df = dag.create(m_c).process(m_p)
             df.assert_eq(dag.df([[0]], "a:long"))
             df.output(m_o)
         dag.run(self.engine)
```

### Comparing `fugue-0.8.4.dev1/tests/fugue_spark/test_ibis.py` & `fugue-0.8.4.dev2/tests/fugue_spark/test_ibis.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/tests/fugue_spark/test_importless.py` & `fugue-0.8.4.dev2/tests/fugue_spark/test_importless.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/tests/fugue_spark/test_sql.py` & `fugue-0.8.4.dev2/tests/fugue_spark/test_sql.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/tests/fugue_spark/utils/test_convert.py` & `fugue-0.8.4.dev2/tests/fugue_spark/utils/test_convert.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/tests/fugue_spark/utils/test_io.py` & `fugue-0.8.4.dev2/tests/fugue_spark/utils/test_io.py`

 * *Files identical despite different names*

### Comparing `fugue-0.8.4.dev1/tests/fugue_spark/utils/test_partition.py` & `fugue-0.8.4.dev2/tests/fugue_spark/utils/test_partition.py`

 * *Files identical despite different names*

