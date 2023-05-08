# Comparing `tmp/nonebot-plugin-cqsat-0.1.3.tar.gz` & `tmp/nonebot-plugin-cqsat-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-cqsat-0.1.3.tar", last modified: Fri Dec 23 13:37:50 2022, max compression
+gzip compressed data, was "nonebot-plugin-cqsat-0.1.4.tar", last modified: Mon May  8 05:57:48 2023, max compression
```

## Comparing `nonebot-plugin-cqsat-0.1.3.tar` & `nonebot-plugin-cqsat-0.1.4.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 13:37:50.319700 nonebot-plugin-cqsat-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2022-12-23 13:37:40.000000 nonebot-plugin-cqsat-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      145 2022-12-23 13:37:40.000000 nonebot-plugin-cqsat-0.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6980 2022-12-23 13:37:50.319700 nonebot-plugin-cqsat-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6457 2022-12-23 13:37:40.000000 nonebot-plugin-cqsat-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 13:37:50.307700 nonebot-plugin-cqsat-0.1.3/cqsat/
--rw-r--r--   0 runner    (1001) docker     (123)      258 2022-12-23 13:37:40.000000 nonebot-plugin-cqsat-0.1.3/cqsat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 13:37:50.303700 nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 13:37:50.307700 nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/
--rw-r--r--   0 runner    (1001) docker     (123)   161387 2022-12-23 13:37:40.000000 nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/A.json
--rw-r--r--   0 runner    (1001) docker     (123)   282636 2022-12-23 13:37:40.000000 nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/B.json
--rw-r--r--   0 runner    (1001) docker     (123)   442381 2022-12-23 13:37:40.000000 nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/C.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 13:37:50.315700 nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/
--rw-r--r--   0 runner    (1001) docker     (123)     5673 2022-12-23 13:37:40.000000 nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0497.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     6223 2022-12-23 13:37:40.000000 nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0498.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     6505 2022-12-23 13:37:40.000000 nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0499.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     6082 2022-12-23 13:37:40.000000 nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0500.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     5961 2022-12-23 13:37:40.000000 nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0501.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     8308 2022-12-23 13:37:40.000000 nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0502.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    17027 2022-12-23 13:37:40.000000 nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0503.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     5919 2022-12-23 13:37:40.000000 nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0504.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     8296 2022-12-23 13:37:40.000000 nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0505.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     7772 2022-12-23 13:37:40.000000 nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0506.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    10149 2022-12-23 13:37:40.000000 nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0507.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     7333 2022-12-23 13:37:40.000000 nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0508.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     7225 2022-12-23 13:37:40.000000 nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0509.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     7051 2022-12-23 13:37:40.000000 nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0510.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     7777 2022-12-23 13:37:40.000000 nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0511.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    13831 2022-12-23 13:37:40.000000 nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0594.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     9478 2022-12-23 13:37:40.000000 nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0595.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     9566 2022-12-23 13:37:40.000000 nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0596.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    11788 2022-12-23 13:37:40.000000 nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0597.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    11752 2022-12-23 13:37:40.000000 nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0598.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    13054 2022-12-23 13:37:40.000000 nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0599.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    11683 2022-12-23 13:37:40.000000 nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0600.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    13050 2022-12-23 13:37:40.000000 nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0601.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    12037 2022-12-23 13:37:40.000000 nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0602.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    12424 2022-12-23 13:37:40.000000 nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0603.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    37302 2022-12-23 13:37:40.000000 nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0604.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    68550 2022-12-23 13:37:40.000000 nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0605.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    52089 2022-12-23 13:37:40.000000 nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0606.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    45355 2022-12-23 13:37:40.000000 nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0607.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    52629 2022-12-23 13:37:40.000000 nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0608.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    43611 2022-12-23 13:37:40.000000 nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0609.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    18311 2022-12-23 13:37:40.000000 nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0610.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    47079 2022-12-23 13:37:40.000000 nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0611.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    26943 2022-12-23 13:37:40.000000 nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0612.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    60117 2022-12-23 13:37:40.000000 nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0613.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    33774 2022-12-23 13:37:40.000000 nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0614.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    62805 2022-12-23 13:37:40.000000 nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0734.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    52168 2022-12-23 13:37:40.000000 nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0735.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    55498 2022-12-23 13:37:40.000000 nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0736.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    58412 2022-12-23 13:37:40.000000 nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0740.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    57669 2022-12-23 13:37:40.000000 nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0741.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    56133 2022-12-23 13:37:40.000000 nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0742.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    57173 2022-12-23 13:37:40.000000 nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0743.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    56601 2022-12-23 13:37:40.000000 nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0744.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    55239 2022-12-23 13:37:40.000000 nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0745.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   107908 2022-12-23 13:37:40.000000 nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0927.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   107610 2022-12-23 13:37:40.000000 nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0928.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    95560 2022-12-23 13:37:40.000000 nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0938.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    28026 2022-12-23 13:37:40.000000 nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0941.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    72144 2022-12-23 13:37:40.000000 nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0942.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   127576 2022-12-23 13:37:40.000000 nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0943.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    73505 2022-12-23 13:37:40.000000 nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0944.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   126097 2022-12-23 13:37:40.000000 nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0945.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 13:37:50.315700 nonebot-plugin-cqsat-0.1.3/cqsat/exercise/
--rw-r--r--   0 runner    (1001) docker     (123)     7336 2022-12-23 13:37:40.000000 nonebot-plugin-cqsat-0.1.3/cqsat/exercise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12944 2022-12-23 13:37:40.000000 nonebot-plugin-cqsat-0.1.3/cqsat/exercise/exam.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2022-12-23 13:37:40.000000 nonebot-plugin-cqsat-0.1.3/cqsat/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 13:37:50.315700 nonebot-plugin-cqsat-0.1.3/cqsat/mgsl/
--rw-r--r--   0 runner    (1001) docker     (123)     2582 2022-12-23 13:37:40.000000 nonebot-plugin-cqsat-0.1.3/cqsat/mgsl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2022-12-23 13:37:40.000000 nonebot-plugin-cqsat-0.1.3/cqsat/mgsl/calculate_mgsl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2022-12-23 13:37:40.000000 nonebot-plugin-cqsat-0.1.3/cqsat/path.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 13:37:50.315700 nonebot-plugin-cqsat-0.1.3/cqsat/pre/
--rw-r--r--   0 runner    (1001) docker     (123)   121993 2022-12-23 13:37:40.000000 nonebot-plugin-cqsat-0.1.3/cqsat/pre/A.txt
--rw-r--r--   0 runner    (1001) docker     (123)   207947 2022-12-23 13:37:40.000000 nonebot-plugin-cqsat-0.1.3/cqsat/pre/B.txt
--rw-r--r--   0 runner    (1001) docker     (123)   326871 2022-12-23 13:37:40.000000 nonebot-plugin-cqsat-0.1.3/cqsat/pre/C.txt
--rw-r--r--   0 runner    (1001) docker     (123)      163 2022-12-23 13:37:40.000000 nonebot-plugin-cqsat-0.1.3/cqsat/pre/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2022-12-23 13:37:40.000000 nonebot-plugin-cqsat-0.1.3/cqsat/pre/pre.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 13:37:50.315700 nonebot-plugin-cqsat-0.1.3/cqsat/sat/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2022-12-23 13:37:40.000000 nonebot-plugin-cqsat-0.1.3/cqsat/sat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3572 2022-12-23 13:37:40.000000 nonebot-plugin-cqsat-0.1.3/cqsat/sat/calculate_sat.py
--rw-r--r--   0 runner    (1001) docker     (123)    14790 2022-12-23 13:37:40.000000 nonebot-plugin-cqsat-0.1.3/cqsat/sat/sat_handle.py
--rw-r--r--   0 runner    (1001) docker     (123)     6396 2022-12-23 13:37:40.000000 nonebot-plugin-cqsat-0.1.3/cqsat/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 13:37:50.319700 nonebot-plugin-cqsat-0.1.3/nonebot_plugin_cqsat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6980 2022-12-23 13:37:50.000000 nonebot-plugin-cqsat-0.1.3/nonebot_plugin_cqsat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2022-12-23 13:37:50.000000 nonebot-plugin-cqsat-0.1.3/nonebot_plugin_cqsat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-23 13:37:50.000000 nonebot-plugin-cqsat-0.1.3/nonebot_plugin_cqsat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      124 2022-12-23 13:37:50.000000 nonebot-plugin-cqsat-0.1.3/nonebot_plugin_cqsat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2022-12-23 13:37:50.000000 nonebot-plugin-cqsat-0.1.3/nonebot_plugin_cqsat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-23 13:37:50.319700 nonebot-plugin-cqsat-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2022-12-23 13:37:40.000000 nonebot-plugin-cqsat-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 05:57:48.175416 nonebot-plugin-cqsat-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-08 05:57:36.000000 nonebot-plugin-cqsat-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-08 05:57:36.000000 nonebot-plugin-cqsat-0.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6980 2023-05-08 05:57:48.171416 nonebot-plugin-cqsat-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6457 2023-05-08 05:57:36.000000 nonebot-plugin-cqsat-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 05:57:48.155416 nonebot-plugin-cqsat-0.1.4/cqsat/
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-08 05:57:36.000000 nonebot-plugin-cqsat-0.1.4/cqsat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 05:57:48.155416 nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 05:57:48.159416 nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/
+-rw-r--r--   0 runner    (1001) docker     (123)   161387 2023-05-08 05:57:36.000000 nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/A.json
+-rw-r--r--   0 runner    (1001) docker     (123)   282636 2023-05-08 05:57:36.000000 nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/B.json
+-rw-r--r--   0 runner    (1001) docker     (123)   442381 2023-05-08 05:57:36.000000 nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/C.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 05:57:48.171416 nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/
+-rw-r--r--   0 runner    (1001) docker     (123)     5673 2023-05-08 05:57:36.000000 nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0497.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     6223 2023-05-08 05:57:36.000000 nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0498.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     6505 2023-05-08 05:57:36.000000 nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0499.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     6082 2023-05-08 05:57:36.000000 nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0500.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-05-08 05:57:36.000000 nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0501.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     8308 2023-05-08 05:57:36.000000 nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0502.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    17027 2023-05-08 05:57:36.000000 nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0503.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     5919 2023-05-08 05:57:36.000000 nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0504.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     8296 2023-05-08 05:57:36.000000 nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0505.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     7772 2023-05-08 05:57:36.000000 nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0506.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    10149 2023-05-08 05:57:36.000000 nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0507.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     7333 2023-05-08 05:57:36.000000 nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0508.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     7225 2023-05-08 05:57:36.000000 nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0509.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     7051 2023-05-08 05:57:36.000000 nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0510.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     7777 2023-05-08 05:57:36.000000 nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0511.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    13831 2023-05-08 05:57:36.000000 nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0594.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     9478 2023-05-08 05:57:36.000000 nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0595.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     9566 2023-05-08 05:57:36.000000 nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0596.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    11788 2023-05-08 05:57:36.000000 nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0597.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    11752 2023-05-08 05:57:36.000000 nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0598.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    13054 2023-05-08 05:57:36.000000 nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0599.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    11683 2023-05-08 05:57:36.000000 nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0600.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    13050 2023-05-08 05:57:36.000000 nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0601.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    12037 2023-05-08 05:57:36.000000 nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0602.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    12424 2023-05-08 05:57:36.000000 nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0603.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    37302 2023-05-08 05:57:36.000000 nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0604.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    68550 2023-05-08 05:57:36.000000 nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0605.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    52089 2023-05-08 05:57:36.000000 nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0606.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    45355 2023-05-08 05:57:36.000000 nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0607.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    52629 2023-05-08 05:57:36.000000 nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0608.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    43611 2023-05-08 05:57:36.000000 nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0609.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    18311 2023-05-08 05:57:36.000000 nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0610.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    47079 2023-05-08 05:57:36.000000 nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0611.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    26943 2023-05-08 05:57:36.000000 nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0612.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    60117 2023-05-08 05:57:36.000000 nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0613.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    33774 2023-05-08 05:57:36.000000 nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0614.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    62805 2023-05-08 05:57:36.000000 nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0734.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    52168 2023-05-08 05:57:36.000000 nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0735.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    55498 2023-05-08 05:57:36.000000 nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0736.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    58412 2023-05-08 05:57:36.000000 nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0740.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    57669 2023-05-08 05:57:36.000000 nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0741.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    56133 2023-05-08 05:57:36.000000 nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0742.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    57173 2023-05-08 05:57:36.000000 nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0743.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    56601 2023-05-08 05:57:36.000000 nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0744.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    55239 2023-05-08 05:57:36.000000 nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0745.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   107908 2023-05-08 05:57:36.000000 nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0927.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   107610 2023-05-08 05:57:36.000000 nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0928.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    95560 2023-05-08 05:57:36.000000 nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0938.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    28026 2023-05-08 05:57:36.000000 nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0941.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    72144 2023-05-08 05:57:36.000000 nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0942.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   127576 2023-05-08 05:57:36.000000 nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0943.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    73505 2023-05-08 05:57:36.000000 nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0944.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   126097 2023-05-08 05:57:36.000000 nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0945.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 05:57:48.171416 nonebot-plugin-cqsat-0.1.4/cqsat/exercise/
+-rw-r--r--   0 runner    (1001) docker     (123)     7336 2023-05-08 05:57:36.000000 nonebot-plugin-cqsat-0.1.4/cqsat/exercise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12944 2023-05-08 05:57:36.000000 nonebot-plugin-cqsat-0.1.4/cqsat/exercise/exam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-08 05:57:36.000000 nonebot-plugin-cqsat-0.1.4/cqsat/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 05:57:48.171416 nonebot-plugin-cqsat-0.1.4/cqsat/mgsl/
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-05-08 05:57:36.000000 nonebot-plugin-cqsat-0.1.4/cqsat/mgsl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-05-08 05:57:36.000000 nonebot-plugin-cqsat-0.1.4/cqsat/mgsl/calculate_mgsl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-08 05:57:36.000000 nonebot-plugin-cqsat-0.1.4/cqsat/path.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 05:57:48.171416 nonebot-plugin-cqsat-0.1.4/cqsat/pre/
+-rw-r--r--   0 runner    (1001) docker     (123)   121993 2023-05-08 05:57:36.000000 nonebot-plugin-cqsat-0.1.4/cqsat/pre/A.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   207947 2023-05-08 05:57:36.000000 nonebot-plugin-cqsat-0.1.4/cqsat/pre/B.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   326871 2023-05-08 05:57:36.000000 nonebot-plugin-cqsat-0.1.4/cqsat/pre/C.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-08 05:57:36.000000 nonebot-plugin-cqsat-0.1.4/cqsat/pre/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-08 05:57:36.000000 nonebot-plugin-cqsat-0.1.4/cqsat/pre/pre.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 05:57:48.171416 nonebot-plugin-cqsat-0.1.4/cqsat/sat/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-08 05:57:36.000000 nonebot-plugin-cqsat-0.1.4/cqsat/sat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-05-08 05:57:36.000000 nonebot-plugin-cqsat-0.1.4/cqsat/sat/calculate_sat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14857 2023-05-08 05:57:36.000000 nonebot-plugin-cqsat-0.1.4/cqsat/sat/sat_handle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6396 2023-05-08 05:57:36.000000 nonebot-plugin-cqsat-0.1.4/cqsat/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 05:57:48.171416 nonebot-plugin-cqsat-0.1.4/nonebot_plugin_cqsat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6980 2023-05-08 05:57:48.000000 nonebot-plugin-cqsat-0.1.4/nonebot_plugin_cqsat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-05-08 05:57:48.000000 nonebot-plugin-cqsat-0.1.4/nonebot_plugin_cqsat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 05:57:48.000000 nonebot-plugin-cqsat-0.1.4/nonebot_plugin_cqsat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-08 05:57:48.000000 nonebot-plugin-cqsat-0.1.4/nonebot_plugin_cqsat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-08 05:57:48.000000 nonebot-plugin-cqsat-0.1.4/nonebot_plugin_cqsat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 05:57:48.175416 nonebot-plugin-cqsat-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-05-08 05:57:36.000000 nonebot-plugin-cqsat-0.1.4/setup.py
```

### Comparing `nonebot-plugin-cqsat-0.1.3/LICENSE` & `nonebot-plugin-cqsat-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.3/PKG-INFO` & `nonebot-plugin-cqsat-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-cqsat
-Version: 0.1.3
+Version: 0.1.4
 Summary: nonebot2 业余无线电卫星
 Home-page: https://github.com/yzyyz1387/cqsat
 Author: yzyyz1387
 Author-email: youzyyz1384@gmail.com
 Keywords: ham,nonebot2,nonebot,radio,nonebot_plugin
 Platform: any
 Classifier: Programming Language :: Python :: 3
```

### Comparing `nonebot-plugin-cqsat-0.1.3/README.md` & `nonebot-plugin-cqsat-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/A.json` & `nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/A.json`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/B.json` & `nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/B.json`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/C.json` & `nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/C.json`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0497.jpg` & `nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0497.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0498.jpg` & `nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0498.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0499.jpg` & `nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0499.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0500.jpg` & `nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0500.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0501.jpg` & `nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0501.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0502.jpg` & `nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0502.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0503.jpg` & `nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0503.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0504.jpg` & `nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0504.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0505.jpg` & `nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0505.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0506.jpg` & `nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0506.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0507.jpg` & `nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0507.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0508.jpg` & `nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0508.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0509.jpg` & `nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0509.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0510.jpg` & `nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0510.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0511.jpg` & `nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0511.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0594.jpg` & `nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0594.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0595.jpg` & `nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0595.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0596.jpg` & `nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0596.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0597.jpg` & `nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0597.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0598.jpg` & `nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0598.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0599.jpg` & `nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0599.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0600.jpg` & `nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0600.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0601.jpg` & `nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0601.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0602.jpg` & `nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0602.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0603.jpg` & `nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0603.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0604.jpg` & `nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0604.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0605.jpg` & `nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0605.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0606.jpg` & `nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0606.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0607.jpg` & `nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0607.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0608.jpg` & `nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0608.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0609.jpg` & `nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0609.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0610.jpg` & `nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0610.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0611.jpg` & `nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0611.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0612.jpg` & `nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0612.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0613.jpg` & `nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0613.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0614.jpg` & `nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0614.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0734.jpg` & `nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0734.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0735.jpg` & `nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0735.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0736.jpg` & `nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0736.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0740.jpg` & `nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0740.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0741.jpg` & `nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0741.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0742.jpg` & `nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0742.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0743.jpg` & `nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0743.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0744.jpg` & `nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0744.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0745.jpg` & `nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0745.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0927.jpg` & `nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0927.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0928.jpg` & `nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0928.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0938.jpg` & `nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0938.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0941.jpg` & `nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0941.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0942.jpg` & `nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0942.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0943.jpg` & `nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0943.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0944.jpg` & `nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0944.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.3/cqsat/cqsat_resource/bank/imgs/LK0945.jpg` & `nonebot-plugin-cqsat-0.1.4/cqsat/cqsat_resource/bank/imgs/LK0945.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.3/cqsat/exercise/__init__.py` & `nonebot-plugin-cqsat-0.1.4/cqsat/exercise/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.3/cqsat/exercise/exam.py` & `nonebot-plugin-cqsat-0.1.4/cqsat/exercise/exam.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.3/cqsat/log.py` & `nonebot-plugin-cqsat-0.1.4/cqsat/log.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.3/cqsat/mgsl/__init__.py` & `nonebot-plugin-cqsat-0.1.4/cqsat/mgsl/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.3/cqsat/mgsl/calculate_mgsl.py` & `nonebot-plugin-cqsat-0.1.4/cqsat/mgsl/calculate_mgsl.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.3/cqsat/path.py` & `nonebot-plugin-cqsat-0.1.4/cqsat/path.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.3/cqsat/pre/A.txt` & `nonebot-plugin-cqsat-0.1.4/cqsat/pre/A.txt`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.3/cqsat/pre/B.txt` & `nonebot-plugin-cqsat-0.1.4/cqsat/pre/B.txt`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.3/cqsat/pre/C.txt` & `nonebot-plugin-cqsat-0.1.4/cqsat/pre/C.txt`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.3/cqsat/pre/pre.py` & `nonebot-plugin-cqsat-0.1.4/cqsat/pre/pre.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.3/cqsat/sat/calculate_sat.py` & `nonebot-plugin-cqsat-0.1.4/cqsat/sat/calculate_sat.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.3/cqsat/sat/sat_handle.py` & `nonebot-plugin-cqsat-0.1.4/cqsat/sat/sat_handle.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,15 +88,15 @@
         await sub.finish("没有找到QTH文件，请发送【绑定位置】来绑定QTH\n绑定后可以发送【订阅卫星】来订阅卫星")
     if qq in qth:
         if sat == "天宫" or sat == "中国空间站" or sat in ["TIANGONG", "tiangong"]:
             state["sat"] = ["天宫"]
         else:
             user_sat = sat.split(" ")
             if len(user_sat) == 1:
-                if sat.upper() in sat_s:
+                if sat or sat.upper() in sat_s:
                     state["sat"] = [sat.upper()]
                 else:
                     await sub.reject_arg("Sat", f"没有找到{sat},请重新输入：")
             else:
                 temp = []
                 for sat_ in user_sat:
                     if sat_ == "天宫" or sat == "中国空间站" or sat in ["TIANGONG", "tiangong"]:
@@ -243,23 +243,26 @@
         add = int(input_arg[1])
     except IndexError:
         add = 0
         await specified.send(f"你没有发送时间，将计算 {sat} 现在的状态")
     time = (datetime.utcnow() + timedelta(minutes=add)).strftime("%Y-%m-%d %H:%M:%S")
     send_time = (datetime.now() + timedelta(minutes=add)).strftime("%Y-%m-%d %H:%M:%S")
     if not isChinese(sat):
-        sat = sat.upper()
+        sat_ = sat.upper()
     else:
         sat_dict = (await get_tian_gong())
+    reply = "{sat}不存在"
     if sat in sat_dict:
         out = await calculate(sat, qth, time=time)
+    elif sat_ in sat_dict:
+        out = await calculate(sat_, qth, time=time)
+    if out:
         reply = f"对于QTH:：{qth}\n{sat} 在 {send_time} ：\n仰角为：{round(float(out[1]), 2)}°\n方位角:{round(float(out[0]), 2)}°\n相对速率为：{round(float(out[2]), 2)} "
-        await specified.send(reply)
-    else:
-        await specified.send(f"{sat}不存在")
+    await specified.send(reply)
+
 
 
 async def aps():
     if not Path.exists(CONFIG):
         return
     elif read_all(CONFIG) == "":
         return
```

### Comparing `nonebot-plugin-cqsat-0.1.3/cqsat/utils.py` & `nonebot-plugin-cqsat-0.1.4/cqsat/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.3/nonebot_plugin_cqsat.egg-info/PKG-INFO` & `nonebot-plugin-cqsat-0.1.4/nonebot_plugin_cqsat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-cqsat
-Version: 0.1.3
+Version: 0.1.4
 Summary: nonebot2 业余无线电卫星
 Home-page: https://github.com/yzyyz1387/cqsat
 Author: yzyyz1387
 Author-email: youzyyz1384@gmail.com
 Keywords: ham,nonebot2,nonebot,radio,nonebot_plugin
 Platform: any
 Classifier: Programming Language :: Python :: 3
```

### Comparing `nonebot-plugin-cqsat-0.1.3/nonebot_plugin_cqsat.egg-info/SOURCES.txt` & `nonebot-plugin-cqsat-0.1.4/nonebot_plugin_cqsat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-cqsat-0.1.3/setup.py` & `nonebot-plugin-cqsat-0.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8", errors="ignore") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="nonebot-plugin-cqsat",
-    version="0.1.3",
+    version="0.1.4",
     author="yzyyz1387",
     author_email="youzyyz1384@gmail.com",
     keywords=("ham", "nonebot2", "nonebot", "radio", "nonebot_plugin"),
     description="""nonebot2 业余无线电卫星""",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/yzyyz1387/cqsat",
```

