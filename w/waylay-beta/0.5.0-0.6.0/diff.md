# Comparing `tmp/waylay-beta-0.5.0.tar.gz` & `tmp/waylay-beta-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waylay-beta-0.5.0.tar", last modified: Fri Sep  2 13:27:59 2022, max compression
+gzip compressed data, was "waylay-beta-0.6.0.tar", last modified: Mon May  8 16:09:56 2023, max compression
```

## Comparing `waylay-beta-0.5.0.tar` & `waylay-beta-0.6.0.tar`

### file list

```diff
@@ -1,100 +1,104 @@
-drwxr-xr-x   0 thomas_installer   (502) staff       (20)        0 2022-09-02 13:27:59.975869 waylay-beta-0.5.0/
--rw-r--r--   0 thomas_installer   (502) staff       (20)      746 2020-09-01 13:46:52.000000 waylay-beta-0.5.0/LICENSE.txt
--rw-r--r--   0 thomas_installer   (502) staff       (20)      214 2021-10-12 13:27:30.000000 waylay-beta-0.5.0/MANIFEST.in
--rw-r--r--   0 thomas_installer   (502) staff       (20)     3953 2022-09-02 13:27:59.976091 waylay-beta-0.5.0/PKG-INFO
--rw-r--r--   0 thomas_installer   (502) staff       (20)     2385 2022-09-02 13:10:45.000000 waylay-beta-0.5.0/README.md
-drwxr-xr-x   0 thomas_installer   (502) staff       (20)        0 2022-09-02 13:27:59.862204 waylay-beta-0.5.0/doc/
--rw-r--r--   0 thomas_installer   (502) staff       (20)     1825 2022-09-02 13:10:45.000000 waylay-beta-0.5.0/doc/byoml_runtimes.json
--rw-r--r--   0 thomas_installer   (502) staff       (20)     2803 2022-09-02 13:10:45.000000 waylay-beta-0.5.0/doc/dist.README.md
--rw-r--r--   0 thomas_installer   (502) staff       (20)     1300 2022-09-02 13:27:59.983250 waylay-beta-0.5.0/setup.cfg
--rw-r--r--   0 thomas_installer   (502) staff       (20)     2839 2022-09-02 13:10:45.000000 waylay-beta-0.5.0/setup.py
--rw-r--r--   0 thomas_installer   (502) staff       (20)    81180 2022-09-02 13:10:45.000000 waylay-beta-0.5.0/versioneer.py
-drwxr-xr-x   0 thomas_installer   (502) staff       (20)        0 2022-09-02 13:27:59.984826 waylay-beta-0.5.0/waylay/
--rw-r--r--   0 thomas_installer   (502) staff       (20)      272 2022-09-02 13:10:45.000000 waylay-beta-0.5.0/waylay/__init__.py
--rw-r--r--   0 thomas_installer   (502) staff       (20)      498 2022-09-02 13:27:59.984955 waylay-beta-0.5.0/waylay/_version.py
--rw-r--r--   0 thomas_installer   (502) staff       (20)    16411 2022-09-02 13:10:45.000000 waylay-beta-0.5.0/waylay/auth.py
--rw-r--r--   0 thomas_installer   (502) staff       (20)     7542 2022-09-02 13:10:45.000000 waylay-beta-0.5.0/waylay/auth_interactive.py
-drwxr-xr-x   0 thomas_installer   (502) staff       (20)        0 2022-09-02 13:27:59.892657 waylay-beta-0.5.0/waylay/cli/
--rw-r--r--   0 thomas_installer   (502) staff       (20)       30 2021-02-16 12:31:38.000000 waylay-beta-0.5.0/waylay/cli/__init__.py
--rw-r--r--   0 thomas_installer   (502) staff       (20)       78 2021-02-15 13:59:29.000000 waylay-beta-0.5.0/waylay/cli/__main__.py
--rw-r--r--   0 thomas_installer   (502) staff       (20)      680 2021-10-26 07:36:37.000000 waylay-beta-0.5.0/waylay/cli/_decorators.py
--rw-r--r--   0 thomas_installer   (502) staff       (20)     5916 2022-09-02 13:10:45.000000 waylay-beta-0.5.0/waylay/cli/configcli.py
--rw-r--r--   0 thomas_installer   (502) staff       (20)    18872 2022-09-02 13:10:45.000000 waylay-beta-0.5.0/waylay/cli/seriescli.py
--rw-r--r--   0 thomas_installer   (502) staff       (20)     3377 2022-09-02 13:10:45.000000 waylay-beta-0.5.0/waylay/cli/servicecli.py
--rw-r--r--   0 thomas_installer   (502) staff       (20)     2251 2022-09-02 13:10:45.000000 waylay-beta-0.5.0/waylay/cli/waylaycli.py
--rw-r--r--   0 thomas_installer   (502) staff       (20)     6835 2022-09-02 13:10:45.000000 waylay-beta-0.5.0/waylay/client.py
--rw-r--r--   0 thomas_installer   (502) staff       (20)    12476 2022-09-02 13:10:45.000000 waylay-beta-0.5.0/waylay/config.py
--rw-r--r--   0 thomas_installer   (502) staff       (20)     2598 2021-06-30 08:38:13.000000 waylay-beta-0.5.0/waylay/exceptions.py
--rw-r--r--   0 thomas_installer   (502) staff       (20)        0 2020-09-01 13:46:52.000000 waylay-beta-0.5.0/waylay/py.typed
-drwxr-xr-x   0 thomas_installer   (502) staff       (20)        0 2022-09-02 13:27:59.894900 waylay-beta-0.5.0/waylay/service/
--rw-r--r--   0 thomas_installer   (502) staff       (20)      617 2022-09-02 13:10:45.000000 waylay-beta-0.5.0/waylay/service/__init__.py
--rw-r--r--   0 thomas_installer   (502) staff       (20)    16253 2022-09-02 13:10:45.000000 waylay-beta-0.5.0/waylay/service/_base.py
--rw-r--r--   0 thomas_installer   (502) staff       (20)     9925 2022-09-02 13:10:45.000000 waylay-beta-0.5.0/waylay/service/_decorators.py
-drwxr-xr-x   0 thomas_installer   (502) staff       (20)        0 2022-09-02 13:27:59.896071 waylay-beta-0.5.0/waylay/service/analytics/
--rw-r--r--   0 thomas_installer   (502) staff       (20)      554 2022-09-02 13:10:45.000000 waylay-beta-0.5.0/waylay/service/analytics/__init__.py
-drwxr-xr-x   0 thomas_installer   (502) staff       (20)        0 2022-09-02 13:27:59.905520 waylay-beta-0.5.0/waylay/service/byoml/
--rw-r--r--   0 thomas_installer   (502) staff       (20)      176 2022-09-02 13:10:45.000000 waylay-beta-0.5.0/waylay/service/byoml/__init__.py
--rw-r--r--   0 thomas_installer   (502) staff       (20)     6508 2022-09-02 13:10:45.000000 waylay-beta-0.5.0/waylay/service/byoml/_decorators.py
--rw-r--r--   0 thomas_installer   (502) staff       (20)      784 2022-09-02 13:10:45.000000 waylay-beta-0.5.0/waylay/service/byoml/_exceptions.py
--rw-r--r--   0 thomas_installer   (502) staff       (20)     8648 2021-10-12 13:27:30.000000 waylay-beta-0.5.0/waylay/service/byoml/_model_archive.py
--rw-r--r--   0 thomas_installer   (502) staff       (20)      748 2022-09-02 13:10:45.000000 waylay-beta-0.5.0/waylay/service/byoml/_service.py
--rw-r--r--   0 thomas_installer   (502) staff       (20)      549 2021-02-15 13:59:29.000000 waylay-beta-0.5.0/waylay/service/byoml/about.py
--rw-r--r--   0 thomas_installer   (502) staff       (20)     3583 2022-09-02 13:10:45.000000 waylay-beta-0.5.0/waylay/service/byoml/framework.py
--rw-r--r--   0 thomas_installer   (502) staff       (20)    19282 2022-09-02 13:10:45.000000 waylay-beta-0.5.0/waylay/service/byoml/model.py
--rw-r--r--   0 thomas_installer   (502) staff       (20)     1829 2022-09-02 13:10:45.000000 waylay-beta-0.5.0/waylay/service/byoml/runtime.py
-drwxr-xr-x   0 thomas_installer   (502) staff       (20)        0 2022-09-02 13:27:59.908164 waylay-beta-0.5.0/waylay/service/data/
--rw-r--r--   0 thomas_installer   (502) staff       (20)       76 2021-06-02 13:37:00.000000 waylay-beta-0.5.0/waylay/service/data/__init__.py
--rw-r--r--   0 thomas_installer   (502) staff       (20)      565 2022-09-02 13:10:45.000000 waylay-beta-0.5.0/waylay/service/data/_service.py
--rw-r--r--   0 thomas_installer   (502) staff       (20)     2390 2022-09-02 13:10:45.000000 waylay-beta-0.5.0/waylay/service/data/events.py
--rw-r--r--   0 thomas_installer   (502) staff       (20)     5542 2022-09-02 13:10:45.000000 waylay-beta-0.5.0/waylay/service/data/series.py
-drwxr-xr-x   0 thomas_installer   (502) staff       (20)        0 2022-09-02 13:27:59.910002 waylay-beta-0.5.0/waylay/service/etl/
--rw-r--r--   0 thomas_installer   (502) staff       (20)       86 2021-02-26 10:02:48.000000 waylay-beta-0.5.0/waylay/service/etl/__init__.py
--rw-r--r--   0 thomas_installer   (502) staff       (20)      456 2022-09-02 13:10:45.000000 waylay-beta-0.5.0/waylay/service/etl/_service.py
--rw-r--r--   0 thomas_installer   (502) staff       (20)      956 2022-09-02 13:10:45.000000 waylay-beta-0.5.0/waylay/service/etl/import_.py
-drwxr-xr-x   0 thomas_installer   (502) staff       (20)        0 2022-09-02 13:27:59.920989 waylay-beta-0.5.0/waylay/service/queries/
--rw-r--r--   0 thomas_installer   (502) staff       (20)      115 2022-09-02 13:10:45.000000 waylay-beta-0.5.0/waylay/service/queries/__init__.py
--rw-r--r--   0 thomas_installer   (502) staff       (20)     5337 2022-09-02 13:10:45.000000 waylay-beta-0.5.0/waylay/service/queries/_decorators.py
--rw-r--r--   0 thomas_installer   (502) staff       (20)      907 2022-09-02 13:10:45.000000 waylay-beta-0.5.0/waylay/service/queries/_exceptions.py
--rw-r--r--   0 thomas_installer   (502) staff       (20)      703 2022-09-02 13:10:45.000000 waylay-beta-0.5.0/waylay/service/queries/_service.py
-drwxr-xr-x   0 thomas_installer   (502) staff       (20)        0 2022-09-02 13:27:59.924433 waylay-beta-0.5.0/waylay/service/queries/_util/
--rw-r--r--   0 thomas_installer   (502) staff       (20)      152 2022-09-02 13:10:45.000000 waylay-beta-0.5.0/waylay/service/queries/_util/__init__.py
--rw-r--r--   0 thomas_installer   (502) staff       (20)    24251 2022-09-02 13:10:45.000000 waylay-beta-0.5.0/waylay/service/queries/_util/df_parser.py
--rw-r--r--   0 thomas_installer   (502) staff       (20)    11006 2022-09-02 13:10:45.000000 waylay-beta-0.5.0/waylay/service/queries/_util/parse_util.py
--rw-r--r--   0 thomas_installer   (502) staff       (20)      540 2022-09-02 13:10:45.000000 waylay-beta-0.5.0/waylay/service/queries/about.py
--rw-r--r--   0 thomas_installer   (502) staff       (20)     7801 2022-09-02 13:10:45.000000 waylay-beta-0.5.0/waylay/service/queries/query.py
-drwxr-xr-x   0 thomas_installer   (502) staff       (20)        0 2022-09-02 13:27:59.931232 waylay-beta-0.5.0/waylay/service/resources/
--rw-r--r--   0 thomas_installer   (502) staff       (20)       76 2022-09-02 13:10:45.000000 waylay-beta-0.5.0/waylay/service/resources/__init__.py
--rw-r--r--   0 thomas_installer   (502) staff       (20)      686 2022-09-02 13:10:45.000000 waylay-beta-0.5.0/waylay/service/resources/_service.py
--rw-r--r--   0 thomas_installer   (502) staff       (20)     3386 2022-09-02 13:10:45.000000 waylay-beta-0.5.0/waylay/service/resources/resource.py
--rw-r--r--   0 thomas_installer   (502) staff       (20)     3218 2022-09-02 13:10:45.000000 waylay-beta-0.5.0/waylay/service/resources/resource_type.py
-drwxr-xr-x   0 thomas_installer   (502) staff       (20)        0 2022-09-02 13:27:59.949422 waylay-beta-0.5.0/waylay/service/storage/
--rw-r--r--   0 thomas_installer   (502) staff       (20)       94 2021-02-26 10:02:48.000000 waylay-beta-0.5.0/waylay/service/storage/__init__.py
--rw-r--r--   0 thomas_installer   (502) staff       (20)      957 2022-09-02 13:10:45.000000 waylay-beta-0.5.0/waylay/service/storage/_service.py
--rw-r--r--   0 thomas_installer   (502) staff       (20)     1290 2021-09-02 13:41:04.000000 waylay-beta-0.5.0/waylay/service/storage/about.py
--rw-r--r--   0 thomas_installer   (502) staff       (20)     1797 2022-09-02 13:10:45.000000 waylay-beta-0.5.0/waylay/service/storage/bucket.py
--rw-r--r--   0 thomas_installer   (502) staff       (20)     7351 2022-09-02 13:10:45.000000 waylay-beta-0.5.0/waylay/service/storage/content.py
--rw-r--r--   0 thomas_installer   (502) staff       (20)    10922 2022-09-02 13:10:45.000000 waylay-beta-0.5.0/waylay/service/storage/object.py
--rw-r--r--   0 thomas_installer   (502) staff       (20)     5066 2022-09-02 13:10:45.000000 waylay-beta-0.5.0/waylay/service/storage/subscription.py
-drwxr-xr-x   0 thomas_installer   (502) staff       (20)        0 2022-09-02 13:27:59.957297 waylay-beta-0.5.0/waylay/service/timeseries/
--rw-r--r--   0 thomas_installer   (502) staff       (20)      223 2021-02-26 10:19:33.000000 waylay-beta-0.5.0/waylay/service/timeseries/__init__.py
--rw-r--r--   0 thomas_installer   (502) staff       (20)      741 2022-09-02 13:10:45.000000 waylay-beta-0.5.0/waylay/service/timeseries/_service.py
-drwxr-xr-x   0 thomas_installer   (502) staff       (20)        0 2022-09-02 13:27:59.965676 waylay-beta-0.5.0/waylay/service/timeseries/parser/
--rw-r--r--   0 thomas_installer   (502) staff       (20)     4745 2022-09-02 13:10:45.000000 waylay-beta-0.5.0/waylay/service/timeseries/parser/__init__.py
--rw-r--r--   0 thomas_installer   (502) staff       (20)     8852 2021-10-21 09:40:02.000000 waylay-beta-0.5.0/waylay/service/timeseries/parser/etlfile.py
--rw-r--r--   0 thomas_installer   (502) staff       (20)    16870 2021-10-26 07:36:37.000000 waylay-beta-0.5.0/waylay/service/timeseries/parser/export_series.py
--rw-r--r--   0 thomas_installer   (502) staff       (20)    22637 2022-09-02 13:25:52.000000 waylay-beta-0.5.0/waylay/service/timeseries/parser/import_csv.py
--rw-r--r--   0 thomas_installer   (502) staff       (20)    12581 2022-09-02 13:10:45.000000 waylay-beta-0.5.0/waylay/service/timeseries/parser/import_dataframe.py
--rw-r--r--   0 thomas_installer   (502) staff       (20)    31049 2022-09-02 13:10:45.000000 waylay-beta-0.5.0/waylay/service/timeseries/parser/model.py
--rw-r--r--   0 thomas_installer   (502) staff       (20)      844 2021-10-12 13:18:01.000000 waylay-beta-0.5.0/waylay/service/timeseries/parser/util.py
--rw-r--r--   0 thomas_installer   (502) staff       (20)    23168 2022-09-02 13:10:45.000000 waylay-beta-0.5.0/waylay/service/timeseries/tool.py
-drwxr-xr-x   0 thomas_installer   (502) staff       (20)        0 2022-09-02 13:27:59.968264 waylay-beta-0.5.0/waylay/service/util/
--rw-r--r--   0 thomas_installer   (502) staff       (20)       81 2021-02-26 10:02:48.000000 waylay-beta-0.5.0/waylay/service/util/__init__.py
--rw-r--r--   0 thomas_installer   (502) staff       (20)      644 2022-09-02 13:10:45.000000 waylay-beta-0.5.0/waylay/service/util/_service.py
--rw-r--r--   0 thomas_installer   (502) staff       (20)     5331 2022-09-02 13:10:45.000000 waylay-beta-0.5.0/waylay/service/util/info.py
-drwxr-xr-x   0 thomas_installer   (502) staff       (20)        0 2022-09-02 13:27:59.975405 waylay-beta-0.5.0/waylay_beta.egg-info/
--rw-r--r--   0 thomas_installer   (502) staff       (20)     3953 2022-09-02 13:27:59.000000 waylay-beta-0.5.0/waylay_beta.egg-info/PKG-INFO
--rw-r--r--   0 thomas_installer   (502) staff       (20)     2532 2022-09-02 13:27:59.000000 waylay-beta-0.5.0/waylay_beta.egg-info/SOURCES.txt
--rw-r--r--   0 thomas_installer   (502) staff       (20)        1 2022-09-02 13:27:59.000000 waylay-beta-0.5.0/waylay_beta.egg-info/dependency_links.txt
--rw-r--r--   0 thomas_installer   (502) staff       (20)      106 2022-09-02 13:27:59.000000 waylay-beta-0.5.0/waylay_beta.egg-info/entry_points.txt
--rw-r--r--   0 thomas_installer   (502) staff       (20)     1120 2022-09-02 13:27:59.000000 waylay-beta-0.5.0/waylay_beta.egg-info/requires.txt
--rw-r--r--   0 thomas_installer   (502) staff       (20)       64 2022-09-02 13:27:59.000000 waylay-beta-0.5.0/waylay_beta.egg-info/top_level.txt
+drwxr-xr-x   0 thomas_installer   (502) staff       (20)        0 2023-05-08 16:09:56.899879 waylay-beta-0.6.0/
+-rw-r--r--   0 thomas_installer   (502) staff       (20)      746 2020-09-01 13:46:52.000000 waylay-beta-0.6.0/LICENSE.txt
+-rw-r--r--   0 thomas_installer   (502) staff       (20)      214 2021-10-12 13:27:30.000000 waylay-beta-0.6.0/MANIFEST.in
+-rw-r--r--   0 thomas_installer   (502) staff       (20)     3677 2023-05-08 16:09:56.900056 waylay-beta-0.6.0/PKG-INFO
+-rw-r--r--   0 thomas_installer   (502) staff       (20)     2281 2023-05-08 15:55:01.000000 waylay-beta-0.6.0/README.md
+drwxr-xr-x   0 thomas_installer   (502) staff       (20)        0 2023-05-08 16:09:56.759672 waylay-beta-0.6.0/doc/
+-rw-r--r--   0 thomas_installer   (502) staff       (20)     1825 2022-09-02 13:10:45.000000 waylay-beta-0.6.0/doc/byoml_runtimes.json
+-rw-r--r--   0 thomas_installer   (502) staff       (20)     2530 2023-05-08 15:52:40.000000 waylay-beta-0.6.0/doc/dist.README.md
+drwxr-xr-x   0 thomas_installer   (502) staff       (20)        0 2023-05-08 16:09:56.767061 waylay-beta-0.6.0/my_notes/
+-rw-r--r--   0 thomas_installer   (502) staff       (20)     2015 2023-05-04 16:29:22.000000 waylay-beta-0.6.0/my_notes/client_from_token_test.py
+-rw-r--r--   0 thomas_installer   (502) staff       (20)     1037 2022-09-06 15:32:56.000000 waylay-beta-0.6.0/my_notes/route_csv.py
+-rw-r--r--   0 thomas_installer   (502) staff       (20)        0 2022-09-06 14:38:40.000000 waylay-beta-0.6.0/my_notes/routes_csv.py
+-rw-r--r--   0 thomas_installer   (502) staff       (20)     1300 2023-05-08 16:09:56.901918 waylay-beta-0.6.0/setup.cfg
+-rw-r--r--   0 thomas_installer   (502) staff       (20)     2979 2023-05-08 15:19:23.000000 waylay-beta-0.6.0/setup.py
+-rw-r--r--   0 thomas_installer   (502) staff       (20)    81180 2022-09-02 13:10:45.000000 waylay-beta-0.6.0/versioneer.py
+drwxr-xr-x   0 thomas_installer   (502) staff       (20)        0 2023-05-08 16:09:56.903673 waylay-beta-0.6.0/waylay/
+-rw-r--r--   0 thomas_installer   (502) staff       (20)      272 2022-09-02 13:10:45.000000 waylay-beta-0.6.0/waylay/__init__.py
+-rw-r--r--   0 thomas_installer   (502) staff       (20)      498 2023-05-08 16:09:56.903790 waylay-beta-0.6.0/waylay/_version.py
+-rw-r--r--   0 thomas_installer   (502) staff       (20)    16504 2023-05-04 16:11:37.000000 waylay-beta-0.6.0/waylay/auth.py
+-rw-r--r--   0 thomas_installer   (502) staff       (20)     7484 2023-05-08 12:58:01.000000 waylay-beta-0.6.0/waylay/auth_interactive.py
+drwxr-xr-x   0 thomas_installer   (502) staff       (20)        0 2023-05-08 16:09:56.830044 waylay-beta-0.6.0/waylay/cli/
+-rw-r--r--   0 thomas_installer   (502) staff       (20)       30 2021-02-16 12:31:38.000000 waylay-beta-0.6.0/waylay/cli/__init__.py
+-rw-r--r--   0 thomas_installer   (502) staff       (20)       78 2021-02-15 13:59:29.000000 waylay-beta-0.6.0/waylay/cli/__main__.py
+-rw-r--r--   0 thomas_installer   (502) staff       (20)      680 2021-10-26 07:36:37.000000 waylay-beta-0.6.0/waylay/cli/_decorators.py
+-rw-r--r--   0 thomas_installer   (502) staff       (20)     6014 2023-05-04 14:42:20.000000 waylay-beta-0.6.0/waylay/cli/configcli.py
+-rw-r--r--   0 thomas_installer   (502) staff       (20)    18872 2022-09-02 13:10:45.000000 waylay-beta-0.6.0/waylay/cli/seriescli.py
+-rw-r--r--   0 thomas_installer   (502) staff       (20)     3856 2023-05-08 13:00:00.000000 waylay-beta-0.6.0/waylay/cli/servicecli.py
+-rw-r--r--   0 thomas_installer   (502) staff       (20)     2251 2022-09-02 13:10:45.000000 waylay-beta-0.6.0/waylay/cli/waylaycli.py
+-rw-r--r--   0 thomas_installer   (502) staff       (20)     7653 2023-05-08 11:54:54.000000 waylay-beta-0.6.0/waylay/client.py
+-rw-r--r--   0 thomas_installer   (502) staff       (20)    13194 2023-05-08 12:59:48.000000 waylay-beta-0.6.0/waylay/config.py
+-rw-r--r--   0 thomas_installer   (502) staff       (20)     2598 2021-06-30 08:38:13.000000 waylay-beta-0.6.0/waylay/exceptions.py
+-rw-r--r--   0 thomas_installer   (502) staff       (20)        0 2020-09-01 13:46:52.000000 waylay-beta-0.6.0/waylay/py.typed
+drwxr-xr-x   0 thomas_installer   (502) staff       (20)        0 2023-05-08 16:09:56.835433 waylay-beta-0.6.0/waylay/service/
+-rw-r--r--   0 thomas_installer   (502) staff       (20)      617 2022-09-02 13:10:45.000000 waylay-beta-0.6.0/waylay/service/__init__.py
+-rw-r--r--   0 thomas_installer   (502) staff       (20)    16572 2023-05-08 12:58:01.000000 waylay-beta-0.6.0/waylay/service/_base.py
+-rw-r--r--   0 thomas_installer   (502) staff       (20)     9925 2022-09-02 13:10:45.000000 waylay-beta-0.6.0/waylay/service/_decorators.py
+drwxr-xr-x   0 thomas_installer   (502) staff       (20)        0 2023-05-08 16:09:56.836616 waylay-beta-0.6.0/waylay/service/analytics/
+-rw-r--r--   0 thomas_installer   (502) staff       (20)      554 2022-09-02 13:10:45.000000 waylay-beta-0.6.0/waylay/service/analytics/__init__.py
+drwxr-xr-x   0 thomas_installer   (502) staff       (20)        0 2023-05-08 16:09:56.846190 waylay-beta-0.6.0/waylay/service/byoml/
+-rw-r--r--   0 thomas_installer   (502) staff       (20)      176 2022-09-02 13:10:45.000000 waylay-beta-0.6.0/waylay/service/byoml/__init__.py
+-rw-r--r--   0 thomas_installer   (502) staff       (20)     6511 2023-05-03 15:07:46.000000 waylay-beta-0.6.0/waylay/service/byoml/_decorators.py
+-rw-r--r--   0 thomas_installer   (502) staff       (20)      784 2022-09-02 13:10:45.000000 waylay-beta-0.6.0/waylay/service/byoml/_exceptions.py
+-rw-r--r--   0 thomas_installer   (502) staff       (20)     8648 2021-10-12 13:27:30.000000 waylay-beta-0.6.0/waylay/service/byoml/_model_archive.py
+-rw-r--r--   0 thomas_installer   (502) staff       (20)      699 2023-05-08 11:54:54.000000 waylay-beta-0.6.0/waylay/service/byoml/_service.py
+-rw-r--r--   0 thomas_installer   (502) staff       (20)      549 2021-02-15 13:59:29.000000 waylay-beta-0.6.0/waylay/service/byoml/about.py
+-rw-r--r--   0 thomas_installer   (502) staff       (20)     3753 2023-05-08 12:59:13.000000 waylay-beta-0.6.0/waylay/service/byoml/framework.py
+-rw-r--r--   0 thomas_installer   (502) staff       (20)    19669 2023-05-08 12:59:13.000000 waylay-beta-0.6.0/waylay/service/byoml/model.py
+-rw-r--r--   0 thomas_installer   (502) staff       (20)     1937 2023-05-08 12:59:13.000000 waylay-beta-0.6.0/waylay/service/byoml/runtime.py
+drwxr-xr-x   0 thomas_installer   (502) staff       (20)        0 2023-05-08 16:09:56.850340 waylay-beta-0.6.0/waylay/service/data/
+-rw-r--r--   0 thomas_installer   (502) staff       (20)       76 2021-06-02 13:37:00.000000 waylay-beta-0.6.0/waylay/service/data/__init__.py
+-rw-r--r--   0 thomas_installer   (502) staff       (20)      517 2023-05-08 11:54:54.000000 waylay-beta-0.6.0/waylay/service/data/_service.py
+-rw-r--r--   0 thomas_installer   (502) staff       (20)     2528 2023-05-08 12:59:13.000000 waylay-beta-0.6.0/waylay/service/data/events.py
+-rw-r--r--   0 thomas_installer   (502) staff       (20)     5713 2023-05-08 12:59:13.000000 waylay-beta-0.6.0/waylay/service/data/series.py
+drwxr-xr-x   0 thomas_installer   (502) staff       (20)        0 2023-05-08 16:09:56.854780 waylay-beta-0.6.0/waylay/service/etl/
+-rw-r--r--   0 thomas_installer   (502) staff       (20)       86 2021-02-26 10:02:48.000000 waylay-beta-0.6.0/waylay/service/etl/__init__.py
+-rw-r--r--   0 thomas_installer   (502) staff       (20)      405 2023-05-08 11:54:54.000000 waylay-beta-0.6.0/waylay/service/etl/_service.py
+-rw-r--r--   0 thomas_installer   (502) staff       (20)      956 2022-09-02 13:10:45.000000 waylay-beta-0.6.0/waylay/service/etl/import_.py
+drwxr-xr-x   0 thomas_installer   (502) staff       (20)        0 2023-05-08 16:09:56.859858 waylay-beta-0.6.0/waylay/service/queries/
+-rw-r--r--   0 thomas_installer   (502) staff       (20)      115 2022-09-02 13:10:45.000000 waylay-beta-0.6.0/waylay/service/queries/__init__.py
+-rw-r--r--   0 thomas_installer   (502) staff       (20)     5337 2023-05-03 13:54:02.000000 waylay-beta-0.6.0/waylay/service/queries/_decorators.py
+-rw-r--r--   0 thomas_installer   (502) staff       (20)      907 2022-09-02 13:10:45.000000 waylay-beta-0.6.0/waylay/service/queries/_exceptions.py
+-rw-r--r--   0 thomas_installer   (502) staff       (20)      645 2023-05-08 11:54:54.000000 waylay-beta-0.6.0/waylay/service/queries/_service.py
+drwxr-xr-x   0 thomas_installer   (502) staff       (20)        0 2023-05-08 16:09:56.863105 waylay-beta-0.6.0/waylay/service/queries/_util/
+-rw-r--r--   0 thomas_installer   (502) staff       (20)      152 2022-09-02 13:10:45.000000 waylay-beta-0.6.0/waylay/service/queries/_util/__init__.py
+-rw-r--r--   0 thomas_installer   (502) staff       (20)    24251 2022-09-02 13:10:45.000000 waylay-beta-0.6.0/waylay/service/queries/_util/df_parser.py
+-rw-r--r--   0 thomas_installer   (502) staff       (20)    11006 2022-09-02 13:10:45.000000 waylay-beta-0.6.0/waylay/service/queries/_util/parse_util.py
+-rw-r--r--   0 thomas_installer   (502) staff       (20)      540 2022-09-02 13:10:45.000000 waylay-beta-0.6.0/waylay/service/queries/about.py
+-rw-r--r--   0 thomas_installer   (502) staff       (20)     9246 2023-05-08 12:59:13.000000 waylay-beta-0.6.0/waylay/service/queries/query.py
+drwxr-xr-x   0 thomas_installer   (502) staff       (20)        0 2023-05-08 16:09:56.868710 waylay-beta-0.6.0/waylay/service/resources/
+-rw-r--r--   0 thomas_installer   (502) staff       (20)       76 2022-09-02 13:10:45.000000 waylay-beta-0.6.0/waylay/service/resources/__init__.py
+-rw-r--r--   0 thomas_installer   (502) staff       (20)      586 2023-05-08 11:54:54.000000 waylay-beta-0.6.0/waylay/service/resources/_service.py
+-rw-r--r--   0 thomas_installer   (502) staff       (20)     3622 2023-05-08 12:59:13.000000 waylay-beta-0.6.0/waylay/service/resources/resource.py
+-rw-r--r--   0 thomas_installer   (502) staff       (20)     3454 2023-05-08 12:59:13.000000 waylay-beta-0.6.0/waylay/service/resources/resource_type.py
+drwxr-xr-x   0 thomas_installer   (502) staff       (20)        0 2023-05-08 16:09:56.876415 waylay-beta-0.6.0/waylay/service/storage/
+-rw-r--r--   0 thomas_installer   (502) staff       (20)       94 2021-02-26 10:02:48.000000 waylay-beta-0.6.0/waylay/service/storage/__init__.py
+-rw-r--r--   0 thomas_installer   (502) staff       (20)      906 2023-05-08 11:54:54.000000 waylay-beta-0.6.0/waylay/service/storage/_service.py
+-rw-r--r--   0 thomas_installer   (502) staff       (20)     1096 2023-05-08 12:59:13.000000 waylay-beta-0.6.0/waylay/service/storage/about.py
+-rw-r--r--   0 thomas_installer   (502) staff       (20)     1554 2023-05-08 12:59:13.000000 waylay-beta-0.6.0/waylay/service/storage/bucket.py
+-rw-r--r--   0 thomas_installer   (502) staff       (20)     7348 2023-05-03 15:07:46.000000 waylay-beta-0.6.0/waylay/service/storage/content.py
+-rw-r--r--   0 thomas_installer   (502) staff       (20)     9415 2023-05-08 12:59:13.000000 waylay-beta-0.6.0/waylay/service/storage/object.py
+-rw-r--r--   0 thomas_installer   (502) staff       (20)     4187 2023-05-08 12:59:13.000000 waylay-beta-0.6.0/waylay/service/storage/subscription.py
+drwxr-xr-x   0 thomas_installer   (502) staff       (20)        0 2023-05-08 16:09:56.879105 waylay-beta-0.6.0/waylay/service/timeseries/
+-rw-r--r--   0 thomas_installer   (502) staff       (20)      223 2021-02-26 10:19:33.000000 waylay-beta-0.6.0/waylay/service/timeseries/__init__.py
+-rw-r--r--   0 thomas_installer   (502) staff       (20)      741 2022-09-02 13:10:45.000000 waylay-beta-0.6.0/waylay/service/timeseries/_service.py
+drwxr-xr-x   0 thomas_installer   (502) staff       (20)        0 2023-05-08 16:09:56.886538 waylay-beta-0.6.0/waylay/service/timeseries/parser/
+-rw-r--r--   0 thomas_installer   (502) staff       (20)     4745 2022-09-02 13:10:45.000000 waylay-beta-0.6.0/waylay/service/timeseries/parser/__init__.py
+-rw-r--r--   0 thomas_installer   (502) staff       (20)     8852 2021-10-21 09:40:02.000000 waylay-beta-0.6.0/waylay/service/timeseries/parser/etlfile.py
+-rw-r--r--   0 thomas_installer   (502) staff       (20)    16870 2021-10-26 07:36:37.000000 waylay-beta-0.6.0/waylay/service/timeseries/parser/export_series.py
+-rw-r--r--   0 thomas_installer   (502) staff       (20)    22637 2022-09-02 13:25:52.000000 waylay-beta-0.6.0/waylay/service/timeseries/parser/import_csv.py
+-rw-r--r--   0 thomas_installer   (502) staff       (20)    12577 2023-05-04 14:44:08.000000 waylay-beta-0.6.0/waylay/service/timeseries/parser/import_dataframe.py
+-rw-r--r--   0 thomas_installer   (502) staff       (20)    31210 2023-05-03 15:07:35.000000 waylay-beta-0.6.0/waylay/service/timeseries/parser/model.py
+-rw-r--r--   0 thomas_installer   (502) staff       (20)      844 2021-10-12 13:18:01.000000 waylay-beta-0.6.0/waylay/service/timeseries/parser/util.py
+-rw-r--r--   0 thomas_installer   (502) staff       (20)    23358 2023-05-03 15:07:35.000000 waylay-beta-0.6.0/waylay/service/timeseries/tool.py
+drwxr-xr-x   0 thomas_installer   (502) staff       (20)        0 2023-05-08 16:09:56.889656 waylay-beta-0.6.0/waylay/service/util/
+-rw-r--r--   0 thomas_installer   (502) staff       (20)       81 2021-02-26 10:02:48.000000 waylay-beta-0.6.0/waylay/service/util/__init__.py
+-rw-r--r--   0 thomas_installer   (502) staff       (20)      644 2022-09-02 13:10:45.000000 waylay-beta-0.6.0/waylay/service/util/_service.py
+-rw-r--r--   0 thomas_installer   (502) staff       (20)     6160 2023-05-03 15:07:46.000000 waylay-beta-0.6.0/waylay/service/util/info.py
+drwxr-xr-x   0 thomas_installer   (502) staff       (20)        0 2023-05-08 16:09:56.899417 waylay-beta-0.6.0/waylay_beta.egg-info/
+-rw-r--r--   0 thomas_installer   (502) staff       (20)     3677 2023-05-08 16:09:56.000000 waylay-beta-0.6.0/waylay_beta.egg-info/PKG-INFO
+-rw-r--r--   0 thomas_installer   (502) staff       (20)     2612 2023-05-08 16:09:56.000000 waylay-beta-0.6.0/waylay_beta.egg-info/SOURCES.txt
+-rw-r--r--   0 thomas_installer   (502) staff       (20)        1 2023-05-08 16:09:56.000000 waylay-beta-0.6.0/waylay_beta.egg-info/dependency_links.txt
+-rw-r--r--   0 thomas_installer   (502) staff       (20)      106 2023-05-08 16:09:56.000000 waylay-beta-0.6.0/waylay_beta.egg-info/entry_points.txt
+-rw-r--r--   0 thomas_installer   (502) staff       (20)     1181 2023-05-08 16:09:56.000000 waylay-beta-0.6.0/waylay_beta.egg-info/requires.txt
+-rw-r--r--   0 thomas_installer   (502) staff       (20)       69 2023-05-08 16:09:56.000000 waylay-beta-0.6.0/waylay_beta.egg-info/top_level.txt
```

### Comparing `waylay-beta-0.5.0/LICENSE.txt` & `waylay-beta-0.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `waylay-beta-0.5.0/PKG-INFO` & `waylay-beta-0.6.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: waylay-beta
-Version: 0.5.0
+Version: 0.6.0
 Summary: beta release of the Waylay Python SDK
-Home-page: https://docs-io.waylay.io/#/api/sdk/python
+Home-page: https://docs.waylay.io/#/api/sdk/python
 Author: Waylay
 Author-email: info@waylay.io
 License: ISC
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: dev-3.7
@@ -39,15 +39,15 @@
 * importing and querying _timeseries_ data.
 * uploading your own _machine learning models_ for usage in the _Waylay Rule Engine_
 * provisioning waylay _resources_ and _resource types_.
 
 The SDK is optimised for interactive usage in [Jupyter Notebooks](https://jupyter.org/).
 
 ## Prerequisites
-This package requires a python runtime `3.7` or higher (validated up to `3.10`). 
+This package requires a python runtime `3.7` or higher (validated up to `3.11`). 
 For datascience purposes you typically want to prepare an anaconda environment:
 ```bash
 conda create --name my_waylay_env python=3.8
 conda activate my_waylay_env
 conda install jupyter
 pip install waylay-beta
 jupyter notebook 
@@ -57,21 +57,21 @@
 
 ```bash
 pip install waylay-beta
 ```
 
 ### BYOML dependencies
 
-If you want to prepare BYOML models ([Enterprise](http://docs.waylay.io/#/features/byoml/)|[IO](http://docs-io.waylay.io/#/features/byoml/)), _extra_ dependency configurations are available, that will check or install framework-specific dependencies.
+If you want to prepare BYOML models ([Enterprise](http://docs.waylay.io/#/features/byoml/)), _extra_ dependency configurations are available, that will check or install framework-specific dependencies.
 
 Either for a specific runtime:
-> byoml-xgboost-1.3, byoml-sklearn-0.24, byoml-xgboost-1.0, byoml-pytorch-1.4, byoml-custom-1.0, byoml-tensorflow-2.1, byoml-pytorch-1.5, byoml-pytorch-1.8, byoml-sklearn-0.22, byoml-tensorflow-2.4
+> byoml-pytorch-1.4, byoml-pytorch-1.5, byoml-pytorch-1.8, byoml-tensorflow-2.4, byoml-sklearn-0.24, byoml-tensorflow-2.1, byoml-xgboost-1.0, byoml-sklearn-0.22, byoml-xgboost-1.3, byoml-custom-1.0
 
 or for the default runtime of one of the supported frameworks:
-> byoml-sklearn, byoml-tensorflow, byoml-custom, byoml-pytorch, byoml-xgboost
+> byoml-tensorflow, byoml-xgboost, byoml-pytorch, byoml-sklearn, byoml-custom
 
 E.g. to install with sklearn dependencies for byoml:
 ```bash
 pip install waylay-beta['byoml-sklearn-0.24']
 ```
 or
 ```bash
@@ -84,27 +84,24 @@
 > waylay_client.byoml.runtimes.get('byoml-pytorch-1.8')
 {'framework': 'pytorch', 'framework_version': '1.8', 'name': 'byoml-pytorch-1.8', 'python_version': '3.7'}
 ```
 
 ## Quickstart
 
 * Login to the waylay console, and get hold of an _API key, API secret_ pair \[*>Settings>Authentication keys*\] 
-  > `[Enterprise]` [https:://console.waylay.io](https://console.waylay.io/administration/settings/keys) <br>
-  > `[IO]` [https:://console-io.waylay.io](https://console-io.waylay.io/administration/settings/keys)
+  > `[Enterprise]` [https:://console.waylay.io](https://console.waylay.io/administration/settings/keys)
 
 * Create an SDK client
   ```python
   from waylay import WaylayConfig, WaylayClient
   waylay_client = WaylayClient.from_profile()
   ```
   On first usage, this will prompt for a gateway endpoint,
-  > `[Enterprise]` api.waylay.io (default)<br> 
-  > `[IO]` api-io.waylay.io
+  > `[Enterprise]` api.waylay.io (default)
 
   and your _API key/API secret_ credentials. 
 
 For more details see 
-> `[Enterprise]` [https://docs.waylay.io](https://docs.waylay.io/api/sdk/python/)<br>
-> `[IO]` [https://docs-io.waylay.io](https://docs-io.waylay.io/#/api/sdk/python)
+> `[Enterprise]` [https://docs.waylay.io](https://docs.waylay.io/#/api/sdk/python)
 
 ## Usage Examples
 See [demo notebooks](https://github.com/waylayio/demo-general/tree/master/python-sdk) for the usage examples supported in the current release.
```

### Comparing `waylay-beta-0.5.0/README.md` & `waylay-beta-0.6.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 ```
 ### from [this repository](https://github.com/waylayio/waylay-py)
 ```bash
 pip install git+https://github.com/waylayio/waylay-py@v0.4.0
 ```
 
 ### BYOML runtime dependencies
-If you want to prepare BYOML models ([Enterprise](http://docs.waylay.io/#/features/byoml/)|[IO](http://docs-io.waylay.io/#/features/byoml/)),
+If you want to prepare BYOML models ([Enterprise](http://docs.waylay.io/#/features/byoml/)),
 _extra_ dependency configurations are available, that will check or install runtime-specific dependencies.
 
 Use the label `byoml-<framework>-<framework-version>` for a specific runtime version, or
 `byoml-<framework>` for the current default for a given framework. 
 
 See [byoml_runtimes.json](doc/byoml_runtimes.json) for the list of supported runtimes.
 
@@ -55,16 +55,15 @@
 git clone https://github.com/waylayio/waylay-py
 pip install -e ./waylay-py
 ```
 See [Development Manual](doc/dev.md) for more details.
 
 ## User Documentation
 
-> `[SaaS]` https://docs.waylay.io/api/sdk/python/<br>
-> `[io]` https://docs-io.waylay.io/#/api/sdk/python<br>
+> `[Enterprise]` https://docs.waylay.io/api/sdk/python
 
 ## Usage
 See [demo notebooks](https://github.com/waylayio/demo-general/tree/master/python-sdk) for usage examples.
 
 ## Development
 See [Development Manual](doc/dev.md)
```

### Comparing `waylay-beta-0.5.0/doc/byoml_runtimes.json` & `waylay-beta-0.6.0/doc/byoml_runtimes.json`

 * *Files identical despite different names*

### Comparing `waylay-beta-0.5.0/doc/dist.README.md` & `waylay-beta-0.6.0/doc/dist.README.md`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 * importing and querying _timeseries_ data.
 * uploading your own _machine learning models_ for usage in the _Waylay Rule Engine_
 * provisioning waylay _resources_ and _resource types_.
 
 The SDK is optimised for interactive usage in [Jupyter Notebooks](https://jupyter.org/).
 
 ## Prerequisites
-This package requires a python runtime `3.7` or higher (validated up to `3.10`). 
+This package requires a python runtime `3.7` or higher (validated up to `3.11`). 
 For datascience purposes you typically want to prepare an anaconda environment:
 ```bash
 conda create --name my_waylay_env python=3.8
 conda activate my_waylay_env
 conda install jupyter
 pip install waylay-beta
 jupyter notebook 
@@ -25,15 +25,15 @@
 
 ```bash
 pip install waylay-beta
 ```
 
 ### BYOML dependencies
 
-If you want to prepare BYOML models ([Enterprise](http://docs.waylay.io/#/features/byoml/)|[IO](http://docs-io.waylay.io/#/features/byoml/)), _extra_ dependency configurations are available, that will check or install framework-specific dependencies.
+If you want to prepare BYOML models ([Enterprise](http://docs.waylay.io/#/features/byoml/)), _extra_ dependency configurations are available, that will check or install framework-specific dependencies.
 
 Either for a specific runtime:
 > $RUNTIME_EXTRA_LIST
 
 or for the default runtime of one of the supported frameworks:
 > $FRAMEWORK_EXTRA_LIST
 
@@ -52,27 +52,24 @@
 > waylay_client.byoml.runtimes.get('byoml-pytorch-1.8')
 {'framework': 'pytorch', 'framework_version': '1.8', 'name': 'byoml-pytorch-1.8', 'python_version': '3.7'}
 ```
 
 ## Quickstart
 
 * Login to the waylay console, and get hold of an _API key, API secret_ pair \[*>Settings>Authentication keys*\] 
-  > `[Enterprise]` [https:://console.waylay.io](https://console.waylay.io/administration/settings/keys) <br>
-  > `[IO]` [https:://console-io.waylay.io](https://console-io.waylay.io/administration/settings/keys)
+  > `[Enterprise]` [https:://console.waylay.io](https://console.waylay.io/administration/settings/keys)
 
 * Create an SDK client
   ```python
   from waylay import WaylayConfig, WaylayClient
   waylay_client = WaylayClient.from_profile()
   ```
   On first usage, this will prompt for a gateway endpoint,
-  > `[Enterprise]` api.waylay.io (default)<br> 
-  > `[IO]` api-io.waylay.io
+  > `[Enterprise]` api.waylay.io (default)
 
   and your _API key/API secret_ credentials. 
 
 For more details see 
-> `[Enterprise]` [https://docs.waylay.io](https://docs.waylay.io/api/sdk/python/)<br>
-> `[IO]` [https://docs-io.waylay.io](https://docs-io.waylay.io/#/api/sdk/python)
+> `[Enterprise]` [https://docs.waylay.io](https://docs.waylay.io/#/api/sdk/python)
 
 ## Usage Examples
 See [demo notebooks](https://github.com/waylayio/demo-general/tree/master/python-sdk) for the usage examples supported in the current release.
```

### Comparing `waylay-beta-0.5.0/setup.cfg` & `waylay-beta-0.6.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `waylay-beta-0.5.0/setup.py` & `waylay-beta-0.6.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,28 +32,28 @@
 setup(
     name='waylay-beta',
     description='beta release of the Waylay Python SDK',
     long_description=long_description,
     long_description_content_type='text/markdown',
     version=versioneer.get_version(),
     cmdclass=versioneer.get_cmdclass(),
-    url='https://docs-io.waylay.io/#/api/sdk/python',
+    url='https://docs.waylay.io/#/api/sdk/python',
     author='Waylay',
     author_email='info@waylay.io',
     license='ISC',
     license_file='LICENSE.txt',
     packages=find_namespace_packages(),
     package_data={"waylay": ["py.typed"]},
     include_package_data=True,
     install_requires=[
         'httpx',
         'simple-rest-client',
         'appdirs',
         'python-jose',
-        'pandas',
+        'pandas<2',
         'isodate',
         'joblib',
         'tqdm',  # progres bar
         'tenacity',
         'tabulate',
     ],
     extras_require={
@@ -62,32 +62,37 @@
             'pytest-cov',
             'pytest-mock',
             'mock',
             'pylint',
             'pycodestyle',
             'pydocstyle',
             'autopep8',
-            'mypy',
+            'mypy<0.990',
             'typing-inspect',
             'types-pytz',
             'types-setuptools',
             'types-tabulate',
             'pdoc',
         ],
         'dev-3.7': [
         ],
         'dev-3.8': [
         ],
         'dev-3.9': [
+            # used for releases
+            'build',
         ],
         'dev-3.10': [
         ],
         ':python_version == "3.7"': [
             'typing_extensions'
         ],
+        ':python_version < "3.10"': [
+            'importlib_metadata'
+        ],
         **runtime_requirements
     },
     setup_requires=[
         'setuptools-pep8',
         'PyYAML',
     ],
     python_requires='>=3.7',
```

### Comparing `waylay-beta-0.5.0/versioneer.py` & `waylay-beta-0.6.0/versioneer.py`

 * *Files identical despite different names*

### Comparing `waylay-beta-0.5.0/waylay/auth.py` & `waylay-beta-0.6.0/waylay/auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,18 @@
     """
 
     CLIENT = 'client_credentials'
     APPLICATION = 'application_credentials'
     TOKEN = 'token'
     CALLBACK = 'interactive'
 
+    def __str__(self):
+        """Get the string representation."""
+        return self.value
+
 
 DEFAULT_GATEWAY_URL = 'https://api.waylay.io'
 DEFAULT_ACCOUNTS_URL = 'https://accounts-api.waylay.io'
 TokenString = str
 
 
 class WaylayCredentials(abc.ABC):
@@ -153,15 +157,15 @@
     """Represents that credentials can be asked via (interactive) callback when required."""
 
     credentials_type: ClassVar[CredentialsType] = CredentialsType.CALLBACK
 
     def to_dict(self, obfuscate=True):  # pylint: disable=unused-argument
         """Convert the credentials to a json-serialisable representation."""
         return dict(
-            type=self.credentials_type.value,
+            type=str(self.credentials_type),
             gateway_url=self.gateway_url,
             accounts_url=self.accounts_url
         )
 
     def is_well_formed(self) -> bool:
         """Validate that these credentials are well-formed."""
         return True
@@ -210,15 +214,15 @@
             return f'[{token.domain}] {token.subject}'
         except AuthError as exc:
             return f'INVALID_TOKEN({exc})'
 
     def to_dict(self, obfuscate=True):
         """Get the credential attributes."""
         return dict(
-            type=self.credentials_type.value,
+            type=str(self.credentials_type),
             token='*********' if obfuscate else self.token,
             gateway_url=self.gateway_url,
             accounts_url=self.accounts_url
         )
 
     def is_well_formed(self) -> bool:
         """Validate that these credentials are well-formed."""
```

### Comparing `waylay-beta-0.5.0/waylay/auth_interactive.py` & `waylay-beta-0.6.0/waylay/auth_interactive.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,21 +21,24 @@
 
 
 def tell(message: str):
     """Show an interactive authentication message."""
     print(message)
 
 
-def ask(prompt: str, secret: bool = False) -> str:
-    """Prompt user for credential information."""
-    if secret:
-        return getpass(prompt=prompt)
+def ask(prompt: str) -> str:
+    """Prompt user for information."""
     return input(prompt)
 
 
+def ask_secret(prompt: str) -> str:
+    """Prompt user for credential information."""
+    return getpass(prompt=prompt)
+
+
 def ask_yes_no(prompt: str, default: Optional[bool] = None) -> bool:
     """Keep prompting the user until response starts with a true or false character."""
     while True:
         resp = ask(prompt)
         if not resp and default is not None:
             return default
         resp_char = resp.lower()[0]
@@ -49,15 +52,14 @@
     """Ask for the gateway api in an interactive dialog."""
     gateway_url: str = _gateway_url_for(default_gateway_url)
     gateway_validated = False
     while not gateway_validated:
         tell(f'Proposed api gateway: {gateway_url}')
         tell('Please confirm, or specify a gateway by platform id, hostname or url.')
         tell("""Examples:
-    'io' (or 'api-io.waylay.io') for the IO platform,
     'enterprise' (or 'api.waylay.io') for the Enterprise platform,
     'https://waylay-api.mycompany.com' as a custom endpoint url
         """)
         gateway_url = ask(
             f'> Press enter to confirm, or specify an alternate gateway [{gateway_url}]: '
         ) or gateway_url
         gateway_url = _gateway_url_for(gateway_url)
@@ -100,16 +102,16 @@
     """
     tell("Authenticating to the Waylay Platform")
     gateway_url = ask_gateway(default_gateway_url)
     tell("Please provide client credentials for the waylay data client.")
     credentials = ClientCredentials(api_key='', api_secret='', gateway_url=gateway_url)
     retry = 0
     while not credentials.is_well_formed() and retry < 3:
-        api_key = ask(prompt='> apiKey : ', secret=False).strip()
-        api_secret = ask(prompt='> apiSecret : ', secret=True).strip()
+        api_key = ask(prompt='> apiKey : ').strip()
+        api_secret = ask_secret(prompt='> apiSecret : ').strip()
         credentials = ClientCredentials(
             api_key=api_key, api_secret=api_secret, gateway_url=gateway_url
         )
         if not credentials.is_well_formed():
             retry += 1
             if retry >= 3:
                 tell('Too many attempts, failing authentication')
@@ -142,16 +144,16 @@
         else:
             tell(f"Cannot connect to '{accounts_url}': {accounts_status_resp.reason_phrase}")
 
     tell("Please provide client credentials for the waylay data client.")
     credentials = ClientCredentials(api_key='', api_secret='', accounts_url=accounts_url)
     retry = 0
     while not credentials.is_well_formed() and retry < 3:
-        api_key = ask(prompt='> apiKey : ', secret=False).strip()
-        api_secret = ask(prompt='> apiSecret : ', secret=True).strip()
+        api_key = ask(prompt='> apiKey : ').strip()
+        api_secret = ask_secret(prompt='> apiSecret : ').strip()
         credentials = ClientCredentials(
             api_key=api_key, api_secret=api_secret, accounts_url=accounts_url
         )
         if not credentials.is_well_formed():
             retry += 1
             if retry >= 3:
                 tell('Too many attempts, failing authentication')
```

### Comparing `waylay-beta-0.5.0/waylay/cli/_decorators.py` & `waylay-beta-0.6.0/waylay/cli/_decorators.py`

 * *Files identical despite different names*

### Comparing `waylay-beta-0.5.0/waylay/cli/configcli.py` & `waylay-beta-0.6.0/waylay/cli/configcli.py`

 * *Files 5% similar despite different names*

```diff
@@ -80,20 +80,20 @@
         "profile", "current", "credential", "id", "cluster"
     ]
     current_profile = args.profile or DEFAULT_PROFILE
     table = [
         [
             profile,
             '*' if profile == current_profile else '',
-            config.credentials.credentials_type,
-            config.credentials.id,
-            config.gateway_url or config.accounts_url
+            config.credentials.credentials_type if config else '*invalid*',
+            config.credentials.id if config else '*invalid*',
+            config.gateway_url or config.accounts_url if config else '*invalid*'
         ]
         for profile in WaylayConfig.list_profiles()
-        for config in [WaylayConfig.load(profile, interactive=False)]
+        for config in [WaylayConfig.load(profile, interactive=False, skip_error=True)]
     ]
     print(tabulate(table, headers=header, tablefmt='github'))
 
 
 def handle_config_show_cmd(args: Namespace):
     """Execute the config show command."""
     current_profile = args.profile or DEFAULT_PROFILE
```

### Comparing `waylay-beta-0.5.0/waylay/cli/seriescli.py` & `waylay-beta-0.6.0/waylay/cli/seriescli.py`

 * *Files identical despite different names*

### Comparing `waylay-beta-0.5.0/waylay/cli/servicecli.py` & `waylay-beta-0.6.0/waylay/cli/servicecli.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 """Cli support for the 'service' command."""
 
 from argparse import ArgumentParser, Namespace
 import sys
 import json
 from tabulate import tabulate
 from ..client import WaylayClient
+from ..service.util.info import DESC_LEVELS
 
 COMMANDS = [LIST, DOC] = ['list', 'doc']
 
 
 def init_srv_parser(parser: ArgumentParser):
     """Initialize parser for the service command."""
     cmd_parsers = parser.add_subparsers(dest='srv_cmd', description='Inspect service definitions.')
@@ -44,14 +45,24 @@
     parser.add_argument(
         '-l', '--link', dest='doc_link', nargs='*', help='Filter doc sites links.', default=None
     )
     parser.add_argument(
         '-d', '--doc_url', dest='doc_url',
         help='Set the root of the documentation site.', default='https://docs.waylay.io/#'
     )
+    parser.add_argument(
+        '-a', '--apidoc_url', dest='apidoc_url',
+        help='Set the root of the api documentation site.', default='https://docs.waylay.io/openapi/public/redocly'
+    )
+    parser.add_argument(
+        '--desc-level', dest='desc_lvl', nargs='*',
+        help='Specify the included descriptions.',
+        choices=DESC_LEVELS,
+        default=None
+    )
     return parser
 
 
 def handle_srv_cmd(waylay: WaylayClient, args: Namespace) -> bool:
     """Execute a service command."""
     if args.srv_cmd is None:
         handle_srv_list_cmd(waylay, Namespace(format_json=False, profile=None, format='github'))
@@ -64,17 +75,17 @@
         return True
 
     return False
 
 
 def handle_doc_cmd(client: WaylayClient, args: Namespace) -> bool:
     """Execute documentation generation."""
-    client.config.set_local_settings(doc_url=args.doc_url)
+    client.config.set_local_settings(doc_url=args.doc_url, apidoc_url=args.apidoc_url)
     print(client.util.info.action_info_html(
-        service=args.doc_service, resource=args.doc_resource, links=args.doc_link
+        service=args.doc_service, resource=args.doc_resource, links=args.doc_link, desc_levels=args.desc_lvl
     ))
     return True
 
 
 def handle_srv_list_cmd(waylay: WaylayClient, args: Namespace):
     """Execute the service list command."""
     if args.format_json:
```

### Comparing `waylay-beta-0.5.0/waylay/cli/waylaycli.py` & `waylay-beta-0.6.0/waylay/cli/waylaycli.py`

 * *Files identical despite different names*

### Comparing `waylay-beta-0.5.0/waylay/client.py` & `waylay-beta-0.6.0/waylay/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 """REST client for the Waylay Platform."""
 
 from collections import defaultdict
 from typing import (
     Optional, TypeVar, List, Mapping, Type, Iterable, Dict
 )
-
-import pkg_resources
+import logging
+import sys
+if sys.version_info < (3, 10):
+    from importlib_metadata import entry_points
+else:
+    from importlib.metadata import entry_points
 
 from .service import (
     WaylayService,
     WaylayRESTService,
     WaylayServiceContext,
     ByomlService,
     TimeSeriesService,
@@ -23,24 +27,25 @@
 )
 
 from .service.analytics import AnalyticsServiceLegacy
 from .exceptions import ConfigError
 
 from .config import (
     WaylayConfig,
-    DEFAULT_PROFILE
+    TenantSettings,
+    DEFAULT_PROFILE,
+    SERVICE_KEY_GATEWAY,
+    SERVICE_KEY_ACCOUNTS
 )
 from .auth import (
     WaylayCredentials,
     ClientCredentials,
     TokenCredentials,
 )
 
-import logging
-
 S = TypeVar('S', bound=WaylayService)
 logger = logging.getLogger(__name__)
 
 
 class WaylayClient():
     """REST client for the Waylay Platform."""
 
@@ -66,34 +71,44 @@
         """
         return cls(WaylayConfig.load(
             profile, interactive=interactive, gateway_url=gateway_url
         ))
 
     @classmethod
     def from_client_credentials(
-        cls, api_key: str, api_secret: str, *, gateway_url=None, accounts_url=None
+        cls, api_key: str, api_secret: str, *,
+        gateway_url=None, accounts_url=None,
+        settings: TenantSettings = None
     ):
         """Create a WaylayClient using the given client credentials."""
-        return cls.from_credentials(
-            ClientCredentials(api_key, api_secret, gateway_url=gateway_url, accounts_url=accounts_url)
+        credentials = ClientCredentials(
+            api_key, api_secret, **_auth_urls(gateway_url, accounts_url, settings)
         )
+        return cls.from_credentials(credentials, settings=settings)
 
     @classmethod
     def from_token(
-        cls, token_string: str, *, gateway_url=None, accounts_url=None
+        cls, token_string: str, *,
+        gateway_url=None, accounts_url=None, settings: TenantSettings = None
     ):
         """Create a WaylayClient using a waylay token."""
-        return cls.from_credentials(TokenCredentials(token_string, gateway_url=gateway_url, accounts_url=accounts_url))
+        credentials = TokenCredentials(
+            token_string, **_auth_urls(gateway_url, accounts_url, settings)
+        )
+        return cls.from_credentials(credentials, settings=settings)
 
     @classmethod
     def from_credentials(
-        cls, credentials: WaylayCredentials
+        cls, credentials: WaylayCredentials, settings: TenantSettings = None
     ):
         """Create a WaylayClient using the given client credentials."""
-        return cls(WaylayConfig(credentials))
+        return cls(WaylayConfig(
+            credentials,
+            settings=settings
+        ))
 
     def __init__(self, config: WaylayConfig):
         """Create a WaylayConfig instance."""
         self._services: List[WaylayService] = []
         self.config = config
         self.load_services()
 
@@ -129,23 +144,24 @@
             ")>"
         )
 
     def load_services(self):
         """Load all services that are registered with the `waylay_services` entry point."""
         registered_service_classes = [
             srv_class
-            for entry_point in pkg_resources.iter_entry_points('waylay_services')
+            for entry_point in entry_points(group='waylay_services')
             for srv_class in entry_point.load()
         ]
         if not registered_service_classes:
             logger.warning(
-                f"The package {__package__} "
+                "The package %s "
                 "seems not to be installed properly. "
                 "If it was installed during this runtime session, "
-                "please restart the runtime before continuing."
+                "please restart the runtime before continuing.",
+                __package__
             )
             registered_service_classes = SERVICES
         self.register_service(*registered_service_classes)
 
     def register_service(self, *service_class: Type[S]) -> Iterable[S]:
         """Create and initialize one or more service of the given class.
 
@@ -204,7 +220,14 @@
 
     def list(self) -> List[WaylayService]:
         """List all registered Services.
 
         Implements the `WaylayServiceContext.list` protocol.
         """
         return list(self._services)
+
+
+def _auth_urls(gateway_url=None, accounts_url=None, settings: TenantSettings = None):
+    if settings:
+        gateway_url = gateway_url or settings.get(SERVICE_KEY_GATEWAY)
+        accounts_url = accounts_url or settings.get(SERVICE_KEY_ACCOUNTS)
+    return {'gateway_url': gateway_url, 'accounts_url': accounts_url}
```

### Comparing `waylay-beta-0.5.0/waylay/config.py` & `waylay-beta-0.6.0/waylay/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,17 +15,15 @@
     WaylayCredentials,
     NoCredentials,
     WaylayTokenAuth, WaylayToken,
     CredentialsCallback,
     parse_credentials,
 )
 from .auth_interactive import (
-    ask,
     ask_gateway,
-    ask_yes_no,
     request_client_credentials_interactive,
     request_migrate_to_gateway_interactive,
     request_store_config_interactive,
     _root_url_for
 )
 from .exceptions import AuthError, ConfigError
 
@@ -40,16 +38,20 @@
 
 
 TenantSettings = Mapping[str, str]
 Settings = MutableMapping[str, str]
 
 DEFAULT_PROFILE = '_default_'
 SERVICE_KEY_API = 'waylay_api'
+SERVICE_KEY_GATEWAY = 'waylay_gateway'
+SERVICE_KEY_ACCOUNTS = 'waylay_accounts'
 DEFAULT_DOC_URL: str = 'https://docs.waylay.io/#'
+DEFAULT_APIDOC_URL: str = 'https://docs.waylay.io/openapi/public/redocly'
 DOC_URL_KEY: str = 'doc_url'
+APIDOC_URL_KEY: str = 'apidoc_url'
 
 
 class WaylayConfig():
     """Manages the authentication and endpoint configuration for the Waylay Platform."""
 
     profile: str
     _auth: WaylayTokenAuth
@@ -96,19 +98,22 @@
         # only resolve remote settings if no gateway available
         use_gateway = gateway_root_path is not None and self.gateway_url is not None
         default_url = (
             f'{self.gateway_url}{gateway_root_path}'
             if use_gateway
             else default_root_url
         )
-        settings = (
-            self.local_settings
-            if use_gateway
-            else self.get_settings(resolve=resolve_settings)
-        )
+        settings = self.local_settings
+        if not use_gateway:
+            resolve_settings = (
+                resolve_settings
+                # do not lookup settings for the bootstrap services
+                and config_key not in (SERVICE_KEY_ACCOUNTS, SERVICE_KEY_API)
+            )
+            settings = self.get_settings(resolve=resolve_settings)
         url_override = settings.get(config_key)
         if url_override is not None:
             url_override = _root_url_for(url_override)
             if url_override.endswith(default_root_path):
                 return url_override
             else:
                 return (f'{url_override}{default_root_path}')
@@ -143,14 +148,19 @@
 
     @property
     def doc_url(self) -> str:
         """Get the root url of the documentation site."""
         return self.settings.get(DOC_URL_KEY, DEFAULT_DOC_URL)
 
     @property
+    def apidoc_url(self) -> str:
+        """Get the root url of the api documentation site."""
+        return self.settings.get(APIDOC_URL_KEY, DEFAULT_APIDOC_URL)
+
+    @property
     def tenant_settings(self) -> TenantSettings:
         """Get the tenant settings as stored on accounts.
 
         Will fetch settings when not present and initialised with 'fetch_tenant_settings=True'.
         """
         if self._tenant_settings is None:
             self._tenant_settings = self._request_settings()
@@ -249,34 +259,38 @@
 
     @classmethod
     def load(
         cls,
         profile: str = DEFAULT_PROFILE,
         *,
         interactive: bool = True,
+        skip_error: bool = False,
         gateway_url: str = DEFAULT_GATEWAY_URL
     ):
         """Load a stored waylay configuration."""
         profile = DEFAULT_PROFILE if profile is None else profile
         try:
-            with open(cls.config_file_path(profile), mode='r') as config_file:
+            with open(cls.config_file_path(profile), mode='r', encoding='utf-8') as config_file:
                 config_json = json.load(config_file)
             waylay_config = cls.from_dict(config_json)
             if not waylay_config.gateway_url:
                 msg = f"WaylayConfig profile '{profile}' uses a legacy accounts endpoint {waylay_config.accounts_url}."
                 if interactive:
                     if request_migrate_to_gateway_interactive(profile, msg):
                         gateway_url = ask_gateway(waylay_config.accounts_url)
                         waylay_config.credentials.gateway_url = gateway_url
                         waylay_config.save()
                 else:
                     log.warning(msg)
             return waylay_config
-        except FileNotFoundError as exc:
-            msg = f"Config profile '{profile}' not found"
+        except (FileNotFoundError, ValueError) as exc:
+            msg = f"Config profile '{profile}' not found or invalid."
+            if skip_error:
+                log.warning(msg)
+                return None
             if not interactive:
                 raise ConfigError(msg) from exc
             credentials = request_client_credentials_interactive(default_gateway_url=gateway_url)
             instance = cls(
                 credentials,
                 profile=profile
             )
```

### Comparing `waylay-beta-0.5.0/waylay/exceptions.py` & `waylay-beta-0.6.0/waylay/exceptions.py`

 * *Files identical despite different names*

### Comparing `waylay-beta-0.5.0/waylay/service/__init__.py` & `waylay-beta-0.6.0/waylay/service/__init__.py`

 * *Files identical despite different names*

### Comparing `waylay-beta-0.5.0/waylay/service/_base.py` & `waylay-beta-0.6.0/waylay/service/_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -308,14 +308,15 @@
         """Get the root urls for documentation links if this resource."""
         return {
             link: Template(
                 href_root
             ).safe_substitute(
                 root_url=self.api_root_url,
                 doc_url=self.service.config.doc_url,
+                apidoc_url=self.service.config.apidoc_url,
             )
             for link, href_root in self.link_roots.items()
         }
 
     def doc_links(self, action: Optional[str]) -> Dict[str, Dict[str, str]]:
         """Create a HAL `_links` representation for (documentation) links.
 
@@ -329,20 +330,34 @@
         return {
             link_rel: dict(
                 href=Template(
                     href_root + hrefs.get(link_rel, '')
                 ).safe_substitute(
                     root_url=self.api_root_url,
                     doc_url=self.service.config.doc_url,
+                    apidoc_url=self.service.config.apidoc_url,
                 )
             )
             for link_rel, href_root in self.link_roots.items()
             if link_rel in hrefs
         }
 
+    # override
+    def get_action_full_url(self, action_name, *parts):
+        """Override the regular url computation when not using api gateway."""
+        if (self.api_root_url is None):
+            srv = self.service
+            raise ConfigError(
+                f'The service `{srv.service_key}` has no url configuration. '
+                f'Please provide a endpoint using a setting with key `{srv.config_key}`,'
+                'or request your tenant administrator '
+                f'to configure the global setting `waylay_{srv.config_key}`.'
+            )
+        return super().get_action_full_url(action_name, *parts)
+
 
 class WaylayService():
     """Client object representing a Waylay Tool."""
 
     resource_definitions: Mapping[str, Type[Resource]]
     config: WaylayConfig
     service_key: str = ''
@@ -420,15 +435,14 @@
     """Client object representing a Waylay Service.
 
     A collection of Resources with their operations.
     """
 
     # class variables
     config_key: str = 'api'
-    default_root_url: Optional[str] = None
     default_root_path: str = ''
     link_templates: Dict[str, str] = {}
 
     def __init__(self, *args, **kwargs):
         """Create a WaylayRESTService."""
         timeout = kwargs.pop('timeout', DEFAULT_SERVICE_TIMEOUT)
         json_encode_body = kwargs.pop('json_encode_body', True)
@@ -445,37 +459,29 @@
         """Set the root url and reconfigure the service."""
         self.config.set_root_url(self.config_key, root_url)
         self.reconfigure()
 
     def get_root_url(self) -> Optional[str]:
         """Get the root url."""
         if self.config is None:
-            return self.default_root_url
+            return None
         return self.config.get_root_url(
             self.config_key,
             gateway_root_path=self.gateway_root_path,
-            default_root_url=self.default_root_url,
             default_root_path=self.default_root_path
         )
 
     def reconfigure(self: RS) -> RS:
         """Configure endpoints and authentication with current configuration.
 
         Returns self
         """
         if self.config is None:
             return self
         root_url = self.get_root_url()
-        if not root_url:
-            raise ConfigError(
-                f'The service `{self.service_key}` has no url configuration. '
-                f'Please provide a endpoint using a setting with key `{self.config_key}`,'
-                'or request your tenant administrator '
-                f'to configure the global setting `waylay_{self.config_key}`.'
-            )
         for resource in self._resources.values():
             resource.api_root_url = root_url
             resource.client.auth = self.config.auth
         return self
 
     def __repr__(self):
         """Get a technical string representation of this service."""
@@ -490,10 +496,11 @@
 
     def doc_links(self) -> Dict[str, Dict[str, str]]:
         """Create a HAL `_links` representation for the documentation links."""
         return {
             rel: dict(href=Template(href).safe_substitute(
                 root_url=self.root_url,
                 doc_url=self.config.doc_url,
+                apidoc_url=self.config.apidoc_url,
             ))
             for rel, href in self.link_templates.items()
         }
```

### Comparing `waylay-beta-0.5.0/waylay/service/_decorators.py` & `waylay-beta-0.6.0/waylay/service/_decorators.py`

 * *Files identical despite different names*

### Comparing `waylay-beta-0.5.0/waylay/service/analytics/__init__.py` & `waylay-beta-0.6.0/waylay/service/analytics/__init__.py`

 * *Files identical despite different names*

### Comparing `waylay-beta-0.5.0/waylay/service/byoml/_decorators.py` & `waylay-beta-0.6.0/waylay/service/byoml/_decorators.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     "min": 4,
     "max": 32
 }
 DEFAULT_RETRY_ATTEMPTS = 20
 DEFAULT_RETRY_MAX_DELAY = 180
 
 
-def before_sleep_logger(service_name, action_method, logger=None, level=logging.INFO):
+def before_sleep_logger(service_name, action_method, logger=None, level=logging.WARNING):
     """Create a before-sleep log function for tenacity.Retrying."""
     logger = logger or logging.getLogger(
         f'waylay.{service_name}.{action_method.resource_name}.{action_method.action_name}'
     )
 
     def _log_before_sleep(retry_state: RetryCallState) -> None:
         next_action = retry_state.next_action
```

### Comparing `waylay-beta-0.5.0/waylay/service/byoml/_exceptions.py` & `waylay-beta-0.6.0/waylay/service/byoml/_exceptions.py`

 * *Files identical despite different names*

### Comparing `waylay-beta-0.5.0/waylay/service/byoml/_model_archive.py` & `waylay-beta-0.6.0/waylay/service/byoml/_model_archive.py`

 * *Files identical despite different names*

### Comparing `waylay-beta-0.5.0/waylay/service/byoml/_service.py` & `waylay-beta-0.6.0/waylay/service/byoml/_service.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 
 
 class ByomlService(WaylayRESTService):
     """REST client for the Waylay BYOML Service."""
 
     service_key = 'byoml'
     config_key = 'byoml'
-    default_root_url = 'https://byoml.waylay.io'
     gateway_root_path = '/ml/v1'
 
     resource_definitions = {
         'model': ModelResource,
         'about': AboutResource,
         'framework': FrameworkResource,
         'runtime': RuntimeResource
```

### Comparing `waylay-beta-0.5.0/waylay/service/byoml/about.py` & `waylay-beta-0.6.0/waylay/service/byoml/about.py`

 * *Files identical despite different names*

### Comparing `waylay-beta-0.5.0/waylay/service/byoml/framework.py` & `waylay-beta-0.6.0/waylay/service/byoml/framework.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,15 +34,16 @@
 }
 
 
 class FrameworkResource(WaylayResource):
     """REST Inspect supported runtimes for a given framework."""
 
     link_roots = {
-        'doc': '${doc_url}/api/byoml/?id='
+        'doc': '${doc_url}/api/byoml/?id=',
+        'apidoc': '${apidoc_url}/byoml.html'
     }
 
     actions = {
         'list': {
             'method': 'GET',
             'url': '/frameworks',
             'returns': [
@@ -50,57 +51,61 @@
             ],
             'decorators': [
                 byoml_exception_decorator,
                 return_path_decorator(['frameworks'])
             ],
             'description': 'Frameworks and supported runtimes.',
             'links': {
-                'doc': 'runtimes'
+                'doc': 'runtimes',
+                'apidoc': '',
             },
         },
         'get': {
             'method': 'GET',
             'url': '/frameworks/{}',
             'arguments': [FRAMEWORK_ARG],
             'decorators': [
                 byoml_exception_decorator,
                 byoml_retry_decorator,
                 return_body_decorator,
             ],
             'description': 'Get the default runtime for a framework.',
             'links': {
-                'doc': 'runtimes'
+                'doc': 'runtimes',
+                'apidoc': '',
             },
         },
         'list_versions': {
             'method': 'GET',
             'url': '/frameworks/{}/versions',
             'arguments': [FRAMEWORK_ARG],
             'decorators': [
                 byoml_exception_decorator,
                 byoml_retry_decorator,
                 return_body_decorator,
             ],
             'description': 'Get the runtimes for a framework.',
             'links': {
-                'doc': 'runtimes'
+                'doc': 'runtimes',
+                'apidoc': '',
             },
         },
         'get_version': {
             'method': 'GET',
             'url': '/frameworks/{}/versions/{}',
             'arguments': [FRAMEWORK_ARG, FRAMEWORK_VERSION_ARG],
             'decorators': [
                 byoml_exception_decorator,
                 byoml_retry_decorator,
                 return_body_decorator,
             ],
             'description': 'Get the runtime for a given framework and framework version.',
             'links': {
-                'doc': 'runtimes'
+                'doc': 'runtimes',
+                'apidoc': '',
             },
         }
     }
 
     def find_runtime(self, framework: str, framework_version: Optional[str]) -> Dict:
         """Get the byoml plug runtime for this framework and version (default version if not specified).
```

### Comparing `waylay-beta-0.5.0/waylay/service/byoml/model.py` & `waylay-beta-0.6.0/waylay/service/byoml/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -128,15 +128,16 @@
 
 class ModelResource(WaylayResource):
     """REST Resource for the 'model' entity of the 'byoml' service."""
 
     service: WaylayRESTService
 
     link_roots = {
-        'doc': '${doc_url}/api/byoml/?id='
+        'doc': '${doc_url}/api/byoml/?id=',
+        'apidoc': '${apidoc_url}/byoml.html'
     }
 
     actions = {
         'list': {
             'method': 'GET',
             'url': '/models',
             'returns': [
@@ -149,15 +150,16 @@
             'decorators': [
                 byoml_server_timing_decorator,
                 byoml_exception_decorator,
                 return_path_decorator(['available_models'])
             ],
             'description': 'List the metadata of the deployed <em>BYOML Models</em>',
             'links': {
-                'doc': 'overview-of-the-api'
+                'doc': 'overview-of-the-api',
+                'apidoc': '',
             },
         },
         'list_names': {
             'method': 'GET',
             'url': '/models',
             'decorators': [
                 byoml_server_timing_decorator,
@@ -169,15 +171,16 @@
                     'name': 'model_names',
                     'type': 'List[str]',
                     'description': 'A list of names of deployed models.'
                 }
             ],
             'description': 'List the names of deployed <em>BYOML Models</em>',
             'links': {
-                'doc': 'overview-of-the-api'
+                'doc': 'overview-of-the-api',
+                'apidoc': '',
             },
         },
         '_create': {
             'method': 'POST',
             'url': '/models',
             'decorators': [
                 byoml_server_timing_decorator,
@@ -186,15 +189,16 @@
                 byoml_retry_upload_after_deletion_decorator,
                 return_body_decorator,
             ],
             'description': (
                 'Build and create a new <em>BYOML Model</em> as specified in the request'
             ),
             'links': {
-                'doc': 'how-to-upload-your-model'
+                'doc': 'how-to-upload-your-model',
+                'apidoc': '',
             },
         },
         'upload': {
             'wrapped_actions': ['_create']
         },
         '_replace': {
             'method': 'PUT',
@@ -204,15 +208,16 @@
                 byoml_server_timing_decorator,
                 byoml_exception_decorator,
                 default_timeout_decorator(DEFAULT_MODEL_UPLOAD_TIMEOUT),
                 return_body_decorator,
             ],
             'description': 'Build and replace the named <em>BYOML Model</em>',
             'links': {
-                'doc': 'overwriting-a-model'
+                'doc': 'overwriting-a-model',
+                'apidoc': '',
             },
         },
         'replace': {
             'wrapped_actions': ['_replace']
         },
         'get': {
             'method': 'GET',
@@ -224,15 +229,16 @@
                 byoml_exception_decorator,
                 byoml_raise_not_ready_get,
                 byoml_retry_decorator,
                 return_body_decorator,
             ],
             'description': 'Fetch the metadata of the named <em>BYOML Model</em>',
             'links': {
-                'doc': 'checking-out-your-model'
+                'doc': 'checking-out-your-model',
+                'apidoc': '',
             },
         },
         'update': {
             'method': 'PATCH',
             'url': '/models/{}',
             'arguments': [
                 MODEL_NAME_ARG,
@@ -251,15 +257,16 @@
                 return_body_decorator,
             ],
             'description': (
                 'Update the metadata of the named <em>BYOML Model</em>.\n'
                 'Only metadata attributes can be modified.'
             ),
             'links': {
-                'doc': 'update-metadata-for-a-model'
+                'doc': 'update-metadata-for-a-model',
+                'apidoc': '',
             },
         },
         # ## not yet supported on plug-registry
         # 'get_content': {
         #     'method': 'GET',
         #     'url': '/models/{}/content',
         #     'arguments': [
@@ -293,68 +300,73 @@
                 byoml_retry_decorator,
                 return_path_decorator(['example_payloads'])
             ],
             'description': (
                 'Fetch the <em>example request input</em> of the named <em>BYOML Model</em>'
             ),
             'links': {
-                'doc': 'example-input'
+                'doc': 'example-input',
+                'apidoc': '',
             },
         },
         'predict': {
             'method': 'POST',
             'url': '/models/{}/predict',
             'arguments': [MODEL_NAME_ARG],
             'returns': [MODEL_INFERENCE_RESULT],
             'decorators': _execute_model_decorators('predictions'),
             'description': (
                 'Execute the <em>predict</em> capability of the named <em>BYOML Model</em>'
             ),
             'links': {
-                'doc': 'predictions'
+                'doc': 'predictions',
+                'apidoc': '',
             },
         },
         'regress': {
             'method': 'POST',
             'url': '/models/{}/regress',
             'arguments': [MODEL_NAME_ARG],
             'returns': [MODEL_INFERENCE_RESULT],
             'decorators': _execute_model_decorators('result'),
             'description': (
                 'Execute the <em>regress</em> capability of the named  <em>BYOML Model</em>'
             ),
             'links': {
-                'doc': 'predictions'
+                'doc': 'predictions',
+                'apidoc': '',
             },
         },
         'classify': {
             'method': 'POST',
             'url': '/models/{}/classify',
             'arguments': [MODEL_NAME_ARG],
             'returns': [MODEL_INFERENCE_RESULT],
             'decorators': _execute_model_decorators('result'),
             'description': (
                 'Execute the <em>classification</em> capability of the named <em>BYOML Model</em>'
             ),
             'links': {
-                'doc': 'predictions'
+                'doc': 'predictions',
+                'apidoc': '',
             },
         },
         'remove': {
             'method': 'DELETE',
             'url': '/models/{}',
             'arguments': [MODEL_NAME_ARG],
             'decorators': [
                 byoml_server_timing_decorator,
                 byoml_exception_decorator,
                 return_body_decorator,
             ],
             'description': 'Remove the named <em>BYOML Model</em>',
             'links': {
-                'doc': 'deleting-a-model'
+                'doc': 'deleting-a-model',
+                'apidoc': '',
             },
         },
     }
 
     def __init__(self, *args, **kwargs):
         """Create a ModelResource."""
         kwargs.pop('timeout', None)
```

### Comparing `waylay-beta-0.5.0/waylay/service/byoml/runtime.py` & `waylay-beta-0.6.0/waylay/service/byoml/runtime.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,41 +29,44 @@
 }
 
 
 class RuntimeResource(WaylayResource):
     """REST Resource for the 'runtime' entity of the 'byoml' service."""
 
     link_roots = {
-        'doc': '${doc_url}/api/byoml/?id='
+        'doc': '${doc_url}/api/byoml/?id=',
+        'apidoc': '${apidoc_url}/byoml.html'
     }
 
     actions = {
         'list': {
             'method': 'GET',
             'url': '/runtimes',
             'returns': [RUNTIME_LIST_RETURN],
             'decorators': [
                 byoml_exception_decorator,
                 byoml_retry_decorator,
                 return_path_decorator(['runtimes'])
             ],
             'description': 'List runtimes (framework and framework version).',
             'links': {
-                'doc': 'runtimes'
+                'doc': 'runtimes',
+                'apidoc': '',
             },
         },
         'get': {
             'method': 'GET',
             'url': '/runtimes/{}',
             'arguments': [RUNTIME_ARG],
             'returns': [RUNTIME_RETURN],
             'decorators': [
                 byoml_exception_decorator,
                 byoml_retry_decorator,
                 return_body_decorator,
             ],
             'description': 'Get a supported runtime.',
             'links': {
-                'doc': 'runtimes'
+                'doc': 'runtimes',
+                'apidoc': '',
             },
         }
     }
```

### Comparing `waylay-beta-0.5.0/waylay/service/data/_service.py` & `waylay-beta-0.6.0/waylay/service/data/_service.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 
 
 class DataService(WaylayRESTService):
     """REST client for the Waylay Data Service (broker)."""
 
     config_key = 'data'
     service_key = 'data'
-    default_root_url = 'https://data.waylay.io'
     gateway_root_path = '/data/v1'
     resource_definitions = {
         'series': SeriesResource,
         'events': EventsResource,
     }
 
     series: SeriesResource
```

### Comparing `waylay-beta-0.5.0/waylay/service/data/events.py` & `waylay-beta-0.6.0/waylay/service/data/events.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 }
 
 
 class EventsResource(WaylayResource):
     """REST Resource for the 'events' ingestion of the 'data' service."""
 
     link_roots = {
-        'doc': '${doc_url}/api/broker/?id='
+        'doc': '${doc_url}/api/broker/?id=',
+        'apidoc': '${apidoc_url}/broker.html'
     }
 
     actions = {
         'post': {
             'method': 'POST', 'url': '/events/{}',
             'arguments': [RESOURCE_ARG],
             'decorators': [
@@ -28,40 +29,43 @@
                 decorators.return_path_decorator([]),
             ],
             'description': (
                 'Forward a json message to the rule engine, '
                 'time series database and/or document store for a given resource.'
             ),
             'links': {
-                'doc': 'posting-data-to-the-storage-and-rule-engine'
+                'doc': 'posting-data-to-the-storage-and-rule-engine',
+                'apidoc': '',
             },
         },
         'bulk': {
-            'method': 'POST', 'url': '/messages',
+            'method': 'POST', 'url': '/events',
             'returns': [
             ],
             'decorators': [
                 decorators.exception_decorator,
                 decorators.return_path_decorator([])
             ],
             'description': (
                 'Forward an array of json messages to the rule engine, '
                 'time series database and/or document store.'
             ),
             'links': {
-                'doc': 'posting-array-of-data'
+                'doc': 'posting-array-of-data',
+                'apidoc': '',
             },
         },
         'remove': {
             'method': 'DELETE', 'url': '/{}',
             'arguments': [RESOURCE_ARG],
             'decorators': DEFAULT_DECORATORS,
             'description': 'Remove all data for a resource.',
             'links': {
-                'doc': 'all-data-for-a-resource'
+                'doc': 'all-data-for-a-resource',
+                'apidoc': '',
             },
         },
     }
 
     def get_action_full_url(self, action_name, *parts):
         """Override the regular url computation when not using api gateway."""
         via_gateway = '/data/v1' in self.api_root_url
```

### Comparing `waylay-beta-0.5.0/waylay/service/data/series.py` & `waylay-beta-0.6.0/waylay/service/data/series.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,16 @@
 }
 
 
 class SeriesResource(WaylayResource):
     """REST Resource for the 'series' entity of the 'data' service."""
 
     link_roots = {
-        'doc': '${doc_url}/api/broker/?id='
+        'doc': '${doc_url}/api/broker/?id=',
+        'apidoc': '${apidoc_url}/broker.html'
     }
 
     actions = {
         'data': {
             'method': 'GET', 'url': '/series/{}/{}',
             'arguments': [
                 RESOURCE_ARG, METRIC_ARG, ADDITIONAL_PARAMS_ARG
@@ -55,27 +56,29 @@
             'decorators': [
                 decorators.default_params_decorator({'metadata': 'true'}),
                 decorators.exception_decorator,
                 decorators.return_path_decorator([]),
             ],
             'description': 'Retrieve a list of series and their latest value for a given resource.',
             'links': {
-                'doc': 'metadata'
+                'doc': 'metadata',
+                'apidoc': '',
             },
         },
         'latest': {
             'method': 'GET', 'url': '/series/{}/{}/latest',
             'arguments': [RESOURCE_ARG, METRIC_ARG],
             'decorators': [
                 decorators.exception_decorator,
                 decorators.return_path_decorator([])
             ],
             'description': 'Fetch the latest value for a series.',
             'links': {
-                'doc': 'latest-value-for-a-series'
+                'doc': 'latest-value-for-a-series',
+                'apidoc': '',
             },
         },
         'query': {
             'method': 'POST', 'url': '/series/query',
             'arguments': [{
                 'name': 'body',
                 'type': 'Dict',
@@ -83,15 +86,16 @@
             }],
             'description': 'Execute a broker query document to retrieve aggregated timeseries.',
             'decorators': [
                 decorators.exception_decorator,
                 decorators.return_path_decorator(['series'])
             ],
             'links': {
-                'doc': 'post-timeseries-query'
+                'doc': 'post-timeseries-query',
+                'apidoc': '',
             },
         },
         'export': {
             'method': 'GET',
             'url': '/series/{}/{}/raw',
             'arguments': [RESOURCE_ARG, METRIC_ARG, ADDITIONAL_PARAMS_ARG],
             'description': 'Export a single series using paging with HAL links.',
@@ -99,15 +103,16 @@
                 decorators.exception_decorator,
                 decorators.default_params_decorator(
                     {'from': 0, 'limit': DEFAULT_EXPORT_PAGE_SIZE, 'order': 'ascending'}),
                 decorators.default_header_decorator({'Accept': 'application/hal+json'}),
                 decorators.return_path_decorator(['series']),
             ],
             'links': {
-                'doc': 'getting-time-series-data'
+                'doc': 'getting-time-series-data',
+                'apidoc': '',
             },
         }
     }
 
     def iter_export(
         self, resource_id: str, metric: str,
         page_size: Optional[int] = None,
```

### Comparing `waylay-beta-0.5.0/waylay/service/etl/import_.py` & `waylay-beta-0.6.0/waylay/service/etl/import_.py`

 * *Files identical despite different names*

### Comparing `waylay-beta-0.5.0/waylay/service/queries/_decorators.py` & `waylay-beta-0.6.0/waylay/service/queries/_decorators.py`

 * *Files identical despite different names*

### Comparing `waylay-beta-0.5.0/waylay/service/queries/_exceptions.py` & `waylay-beta-0.6.0/waylay/service/queries/_exceptions.py`

 * *Files identical despite different names*

### Comparing `waylay-beta-0.5.0/waylay/service/queries/_util/df_parser.py` & `waylay-beta-0.6.0/waylay/service/queries/_util/df_parser.py`

 * *Files identical despite different names*

### Comparing `waylay-beta-0.5.0/waylay/service/queries/_util/parse_util.py` & `waylay-beta-0.6.0/waylay/service/queries/_util/parse_util.py`

 * *Files identical despite different names*

### Comparing `waylay-beta-0.5.0/waylay/service/queries/about.py` & `waylay-beta-0.6.0/waylay/service/queries/about.py`

 * *Files identical despite different names*

### Comparing `waylay-beta-0.5.0/waylay/service/queries/query.py` & `waylay-beta-0.6.0/waylay/service/queries/query.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 )
 from ._decorators import (
     query_exception_decorator,
     query_return_dataframe_decorator,
     MultiFrameHandling,
 )
 from ._exceptions import (
-    QueryRequestError
+    QueryRequestError, RestResponseError
 )
 
 
 CONFIG_ENTITY_DECORATORS = [
     query_exception_decorator,
     return_path_decorator(['query'])
 ]
@@ -111,15 +111,15 @@
 
 
 class QueryResource(WaylayResource):
     """REST Resource for the 'query' entity of the 'queries' Service."""
 
     link_roots = {
         'doc': '${doc_url}/api/query/',
-        'apidoc':  '${root_url}/apidocs/'
+        'apidoc':  '${apidoc_url}/queries.html'
     }
 
     actions = {
         'list': {
             'method': 'GET',
             'url': '/query',
             'arguments': [ADDITIONAL_PARAMS_ARG],
@@ -176,15 +176,15 @@
             }
         },
         'replace': {
             'method': 'PUT',
             'url': '/query/{}',
             'arguments': [QUERY_NAME_ARG, QUERY_ENTITY_OR_DEFINITION_BODY],
             'decorators': CONFIG_ENTITY_DECORATORS,
-            'description': 'Create or replace the named query defition.',
+            'description': 'Replace the named query defition.',
             'links': {
                 'doc': '?id=replace',
                 'apidoc': '#/query%20config/put_config_query__query_name_'
             }
         },
         '_execute_by_name': {
             'method': 'GET',
@@ -221,21 +221,57 @@
                 'type': 'pandas.DataFrame',
                 'description': (
                     "A Pandas Dataframe containing the data, "
                     "unless 'response_constructor' specifies otherwise."
                 )
             }],
             'wrapped_actions': ['_execute_by_name', '_execute_by_definition']
+        },
+        'create_or_replace': {
+            'arguments': [
+                {
+                    'name': 'name',
+                    'type': 'Optional[str]',
+                    'description': 'Query name, if not given in body argument.'
+                },
+                QUERY_ENTITY_OR_DEFINITION_BODY,
+                ADDITIONAL_PARAMS_ARG
+            ],
+            'wrapped_actions': ['create', 'replace']
         }
     }
 
-    def execute(self, name_or_query: Union[str, Dict] = None, *, body: Dict = None, **kwargs):
+    def execute(self, name_or_query: Union[str, Dict, None] = None, *, body: Dict = None, **kwargs):
         """Execute a timeseries query by name (string) or definition (object)."""
         if isinstance(name_or_query, str):
             return self._execute_by_name(name_or_query, **kwargs)  # pylint:disable=no-member
 
         # support query to be specified in the `body` argument
         query = name_or_query or body
         if isinstance(query, Dict):
             return self._execute_by_definition(body=query, **kwargs)  # pylint:disable=no-member
 
         raise QueryRequestError('The first argument should be a query name or definition.')
+
+    def create_or_replace(
+        self, name_or_query: Union[str, Dict, None] = None, *, body: Dict = None, **kwargs
+    ):
+        """Create or replace a query definition."""
+        name = None
+        if isinstance(name_or_query, str):
+            name = name_or_query
+        else:
+            body = body or name_or_query
+        if not body:
+            raise QueryRequestError('Missing `body` argument with a query definition.')
+        name = name or body.get('name')
+        if not name:
+            raise QueryRequestError(
+                'Missing `name` as first argument or as property of the `body`.'
+            )
+        try:
+            return self.replace(name, body=body, **kwargs)  # pylint:disable=no-member
+        except RestResponseError as exc:
+            if exc.response.status_code != 404:
+                raise exc
+            body = body if 'query' in body else dict(name=name, query=body)
+            return self.create(body=body, **kwargs)  # pylint:disable=no-member
```

### Comparing `waylay-beta-0.5.0/waylay/service/resources/resource.py` & `waylay-beta-0.6.0/waylay/service/resources/resource.py`

 * *Files 27% similar despite different names*

```diff
@@ -29,78 +29,85 @@
 }
 
 
 class ResourceResource(WaylayResource):
     """REST Resource for the `resource` entity of the `api` (resource provisioning) service."""
 
     link_roots = {
-        'doc': '${doc_url}/api/resources/?id='
+        'doc': '${doc_url}/api/resources/?id=',
+        'apidoc': '${apidoc_url}/resources.html'
     }
 
     actions = {
         'get': {
             'method': 'GET',
             'url': '/resources/{}',
             'arguments': [RESOURCE_ID_ARG],
             'decorators': DEFAULT_DECORATORS,
             'description': 'Retrieve a `resource` representation.',
             'links': {
-                'doc': 'retrieve-resource'
+                'doc': 'retrieve-resource',
+                'apidoc': '',
             },
         },
         'create': {
             'method': 'POST',
             'url': '/resources',
             'arguments': [RESOURCE_BODY_ARG],
             'decorators': [
                 decorators.exception_decorator,
                 decorators.return_path_decorator(['entity'])
             ],
             'description': 'Create a `resource` entity.',
             'links': {
-                'doc': 'create-resource'
+                'doc': 'create-resource',
+                'apidoc': '',
             },
         },
         'update': {
             'method': 'PATCH',
             'url': '/resources/{}',
             'arguments': [RESOURCE_ID_ARG, RESOURCE_BODY_ARG],
             'decorators': DEFAULT_DECORATORS,
             'description': '(Partially) update a `resource` representation.',
             'links': {
-                'doc': 'partial-resource-update'
+                'doc': 'partial-resource-update',
+                'apidoc': '',
             },
         },
         'replace': {
             'method': 'PUT',
             'url': '/resources/{}',
             'arguments': [RESOURCE_ID_ARG, RESOURCE_BODY_ARG],
             'decorators': DEFAULT_DECORATORS,
             'description': 'Replace a `resource` representation.',
             'links': {
-                'doc': 'update-resource'
+                'doc': 'update-resource',
+                'apidoc': '',
             },
         },
         'remove': {
             'method': 'DELETE',
             'url': '/resources/{}',
             'arguments': [RESOURCE_ID_ARG],
             'decorators': DEFAULT_DECORATORS,
             'description': 'Delete a `resource` entity.',
             'links': {
-                'doc': 'delete-resource'
+                'doc': 'delete-resource',
+                'apidoc': '',
             },
         },
         'list': {
             'method': 'GET',
             'url': '/resources',
             'arguments': [ADDITIONAL_PARAMS_ARG],
             'decorators': [
                 decorators.exception_decorator,
                 decorators.return_path_decorator(['values'])
             ],
             'description': 'Query `resource` entities.',
             'links': {
-                'doc': 'query-resources'
+                'doc': 'query-resources',
+                'apidoc': '',
             },
         },
     }
```

### Comparing `waylay-beta-0.5.0/waylay/service/resources/resource_type.py` & `waylay-beta-0.6.0/waylay/service/resources/resource_type.py`

 * *Files 14% similar despite different names*

```diff
@@ -27,72 +27,79 @@
 }
 
 
 class ResourceTypeResource(WaylayResource):
     """REST Resource for the 'resource_type' entity of the 'api' resource provisioning service."""
 
     link_roots = {
-        'doc': '${doc_url}/api/resources/?id='
+        'doc': '${doc_url}/api/resources/?id=',
+        'apidoc': '${apidoc_url}/resources.html'
     }
 
     actions = {
         'create': {
             'method': 'POST',
             'url': '/resourcetypes',
             'arguments': [RESOURCE_TYPE_BODY_ARG],
             'decorators': DEFAULT_DECORATORS,
             'description': 'Create a `resource type` entity.',
             'links': {
-                'doc': 'create-resource-type'
+                'doc': 'create-resource-type',
+                'apidoc': '',
             },
         },
         'remove': {
             'method': 'DELETE',
             'url': '/resourcetypes/{}',
             'arguments': [RESOURCE_TYPE_ID_ARG],
             'decorators': DEFAULT_DECORATORS,
             'description': 'Delete a `resource type` entity.',
             'links': {
-                'doc': 'delete-resource-type'
+                'doc': 'delete-resource-type',
+                'apidoc': '',
             },
         },
         'replace': {
             'method': 'PUT',
             'url': '/resourcetypes/{}',
             'arguments': [RESOURCE_TYPE_ID_ARG, RESOURCE_TYPE_BODY_ARG],
             'decorators': DEFAULT_DECORATORS,
             'description': 'Replace a `resource type` representation.',
             'links': {
-                'doc': 'update-resource-type'
+                'doc': 'update-resource-type',
+                'apidoc': '',
             },
         },
         'update': {
             'method': 'PATCH',
             'url': '/resourcetypes/{}',
             'arguments': [RESOURCE_TYPE_ID_ARG, RESOURCE_TYPE_BODY_ARG],
             'decorators': DEFAULT_DECORATORS,
             'description': '(Partially) update a `resource type` representation.',
             'links': {
-                'doc': 'partial-resource-type-update'
+                'doc': 'partial-resource-type-update',
+                'apidoc': '',
             },
         },
         'get': {
             'method': 'GET',
             'url': '/resourcetypes/{}',
             'arguments': [RESOURCE_TYPE_ID_ARG],
             'decorators': DEFAULT_DECORATORS,
             'description': 'Retrieve a `resource type` representation.',
             'links': {
-                'doc': 'retrieve-resource-type'
+                'doc': 'retrieve-resource-type',
+                'apidoc': '',
             },
         },
         'list': {
             'method': 'GET',
             'url': '/resourcetypes',
             'arguments': [ADDITIONAL_PARAMS_ARG],
             'decorators': DEFAULT_DECORATORS,
             'description': 'Query `resource type` entities.',
             'links': {
-                'doc': 'query-resource-types'
+                'doc': 'query-resource-types',
+                'apidoc': '',
             },
         },
     }
```

### Comparing `waylay-beta-0.5.0/waylay/service/storage/_service.py` & `waylay-beta-0.6.0/waylay/service/storage/_service.py`

 * *Files 19% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 
 
 class StorageService(WaylayRESTService):
     """REST client for the Waylay Storage Service."""
 
     config_key = 'storage'
     service_key = 'storage'
-    default_root_url = 'https://storage.waylay.io'
     gateway_root_path = '/storage/v1'
 
     resource_definitions = {
         'bucket': BucketResource,
         'object': ObjectResource,
         'folder': FolderResource,
         'subscription': SubscriptionResource,
```

### Comparing `waylay-beta-0.5.0/waylay/service/storage/about.py` & `waylay-beta-0.6.0/waylay/service/storage/about.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,35 +6,32 @@
 
 
 class AboutResource(WaylayResource):
     """Static information about version."""
 
     link_roots = {
         'doc': '${doc_url}/api/storage/?id=',
-        'apidoc':  '${root_url}/docs#/status/',
-        'openapi': '${root_url}/openapi.json'
+        'apidoc': '${apidoc_url}/storage.html'
     }
 
     actions = {
         'version': {
             'method': 'GET',
             'url': '/',
             'decorators': DEFAULT_DECORATORS,
             'description': 'Application version',
             'links': {
                 'doc': 'version',
-                'apidoc': 'version__get',
-                'openapi': f"#/paths/{quote('/')}/get",
+                'apidoc': '',
             },
         },
         'status': {
             'method': 'GET',
             'url': '/status',
             'decorators': DEFAULT_DECORATORS,
             'description': 'Validation and statistics on the buckets and policies for this tenant.',
             'links': {
                 'doc': 'tenant-status',
-                'apidoc': 'status_status_get',
-                'openapi': f"#/paths/{quote('/status')}/get",
+                'apidoc': '',
             },
         },
     }
```

### Comparing `waylay-beta-0.5.0/waylay/service/storage/bucket.py` & `waylay-beta-0.6.0/waylay/service/storage/bucket.py`

 * *Files 26% similar despite different names*

```diff
@@ -17,38 +17,35 @@
 
 
 class BucketResource(WaylayResource):
     """REST Resource for the 'bucket' entity of the 'storage' service."""
 
     link_roots = {
         'doc': '${doc_url}/api/storage/?id=',
-        'apidoc':  '${root_url}/docs#/storage/',
-        'openapi': '${root_url}/openapi.json'
+        'apidoc': '${apidoc_url}/storage.html'
     }
 
     actions = {
         'list': {
             'method': 'GET', 'url': '/bucket', 'decorators': [
                 decorators.exception_decorator,
                 decorators.return_path_decorator(['buckets']),
             ],
             'description': 'List available bucket aliases',
             'links': {
                 'doc': 'list-bucket',
-                'apidoc': 'list_buckets_bucket__get',
-                'openapi': f"#/paths/{quote('/bucket')}/get"
+                'apidoc': '',
             }
         },
         'get': {
             'method': 'GET', 'url': '/bucket/{}', 'decorators': [
                 decorators.exception_decorator,
                 decorators.return_body_decorator,
             ],
             'arguments': [BUCKET_NAME_ARG],
             'description': 'Get metadata for a specific bucket alias',
             'links': {
                 'doc': 'get-bucket',
-                'apidoc': 'get_bucket_bucket__bucket_name__get',
-                'openapi': f"#/paths/{quote('/bucket/{bucket_name}')}/get"
+                'apidoc': '',
             }
         },
     }
```

### Comparing `waylay-beta-0.5.0/waylay/service/storage/content.py` & `waylay-beta-0.6.0/waylay/service/storage/content.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         json: Any = None,
         from_file: Optional[Union[str, os.PathLike]] = None,
         progress: bool = True,
         headers: Optional[_http_types.HeaderTypes] = None,
         raw: bool = False,
         **kwargs
     ) -> Union[_http.Response, str]:
-        """Retrieve the content of a storage object.
+        """Store the content of a storage object.
 
 Content can be specified with (exactly) one of the attributes 'from_file', 'content' or 'json'.
 
 This method gets a signed url (see storage.object.sign_put),
 and uploads the object content to the object store.
 
 Arguments:
```

### Comparing `waylay-beta-0.5.0/waylay/service/storage/subscription.py` & `waylay-beta-0.6.0/waylay/service/storage/subscription.py`

 * *Files 21% similar despite different names*

```diff
@@ -34,91 +34,84 @@
 
 
 class SubscriptionResource(WaylayResource):
     """REST Resource for the 'subscription' entity of the 'storage' service."""
 
     link_roots = {
         'doc': '${doc_url}/api/storage/?id=',
-        'apidoc':  '${root_url}/docs#/subscription/',
-        'openapi': '${root_url}/openapi.json'
+        'apidoc':  '${apidoc_url}/storage.html',
     }
     actions = {
         'list': {
             'method': 'GET', 'url': '/subscription/{}', 'decorators': [
                 decorators.exception_decorator,
                 decorators.return_path_decorator(['subscriptions']),
             ],
             'arguments': [BUCKET_NAME_ARG, ADDITIONAL_FILTER_PARAMS_ARG],
             'description': 'List available subscriptions for a given bucket.',
             'links': {
                 'doc': 'list-bucket-subscriptions',
-                'apidoc': 'query_subscriptions_subscription__bucket_name__get',
-                'openapi': f"#/paths/{quote('/subscription/{bucket_name}')}/get"
+                'apidoc': '',
             }
         },
         'get': {
             'method': 'GET', 'url': '/subscription/{}/{}', 'decorators': [
                 decorators.exception_decorator,
                 decorators.return_body_decorator,
             ],
             'arguments': [BUCKET_NAME_ARG, SUBSCRIPTION_ID_ARG],
             'description': 'Retrieve the representation of a notification subscription.',
             'links': {
                 'doc': 'get-subscription',
-                'apidoc': 'get_subscription_subscription__bucket_name___id__get',
-                'openapi': f"#/paths/{quote('/subscription/{bucket_name}/{id}')}/get"
+                'apidoc': '',
             }
         },
         'create': {
             'method': 'POST', 'url': '/subscription/{}', 'decorators': [
                 decorators.exception_decorator,
                 decorators.return_body_decorator,
             ],
             'arguments': [BUCKET_NAME_ARG, SUBSCRIPTION_ENTITY_BODY],
             'description': 'Create a new notification subscription.',
             'links': {
                 'doc': 'create-subscription',
-                'apidoc': 'post_subscription_subscription__bucket_name__post',
-                'openapi': f"#/paths/{quote('/subscription/{bucket_name}/{id}')}/post"
+                'apidoc': '',
             }
         },
         'replace': {
             'method': 'PUT', 'url': '/subscription/{}/{}', 'decorators': [
                 decorators.exception_decorator,
                 decorators.return_body_decorator,
             ],
             'arguments': [BUCKET_NAME_ARG, SUBSCRIPTION_ID_ARG, SUBSCRIPTION_ENTITY_BODY],
             'description': 'Create or Replace the definition of a notification subscription.',
             'links': {
                 'doc': 'update-subscription',
-                'apidoc': 'put_subscription_subscription__bucket_name___id__put',
-                'openapi': f"#/paths/{quote('/subscription/{bucket_name}/{id}')}/put"
+                'apidoc': '',
             }
         },
         'remove': {
             'method': 'DELETE', 'url': '/subscription/{}/{}', 'decorators': [
                 decorators.exception_decorator,
                 decorators.return_body_decorator,
             ],
             'arguments': [BUCKET_NAME_ARG, SUBSCRIPTION_ID_ARG],
             'description': 'Remove a notification subscription.',
             'links': {
                 'doc': 'delete-subscription',
-                'apidoc': 'delete_subscription_subscription__bucket_name___id__delete',
-                'openapi': f"#/paths/{quote('/subscription/{bucket_name}/{id}')}/delete"
+                'apidoc': '',
             }
 
         },
         'remove_all': {
             'method': 'DELETE', 'url': '/subscription/{}', 'decorators': [
                 decorators.exception_decorator,
                 decorators.return_body_decorator,
             ],
             'arguments': [BUCKET_NAME_ARG, ADDITIONAL_FILTER_PARAMS_ARG],
             'description': 'Remove all notification subscription that satisfy a query.',
             'links': {
                 'doc': 'delete-subscriptions',
-                'apidoc': 'delete_subscriptions_subscription__bucket_name__delete',
-                'openapi': f"#/paths/{quote('/subscription/{bucket_name}')}/delete"
+                'apidoc': '',
             }
         },
     }
```

### Comparing `waylay-beta-0.5.0/waylay/service/timeseries/_service.py` & `waylay-beta-0.6.0/waylay/service/timeseries/_service.py`

 * *Files identical despite different names*

### Comparing `waylay-beta-0.5.0/waylay/service/timeseries/parser/__init__.py` & `waylay-beta-0.6.0/waylay/service/timeseries/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `waylay-beta-0.5.0/waylay/service/timeseries/parser/etlfile.py` & `waylay-beta-0.6.0/waylay/service/timeseries/parser/etlfile.py`

 * *Files identical despite different names*

### Comparing `waylay-beta-0.5.0/waylay/service/timeseries/parser/export_series.py` & `waylay-beta-0.6.0/waylay/service/timeseries/parser/export_series.py`

 * *Files identical despite different names*

### Comparing `waylay-beta-0.5.0/waylay/service/timeseries/parser/import_csv.py` & `waylay-beta-0.6.0/waylay/service/timeseries/parser/import_csv.py`

 * *Files identical despite different names*

### Comparing `waylay-beta-0.5.0/waylay/service/timeseries/parser/import_dataframe.py` & `waylay-beta-0.6.0/waylay/service/timeseries/parser/import_dataframe.py`

 * *Files 0% similar despite different names*

```diff
@@ -221,15 +221,15 @@
         raise ParserRequestError('NOT YET SUPPORTED: variable resource and metric by row')
     if settings.value_column:
         column_series_iter = iter([
             (settings.value_column, input_data[settings.value_column])
         ])
         series_count = 1
     else:
-        column_series_iter = input_data.iteritems()
+        column_series_iter = input_data.items()
         series_count = len(input_data.columns)
     if progress and series_count > 1:
         with tqdm(total=series_count, unit_scale=True, unit_divisor=1, unit="series") as tqdm_progress:
             for column, series in column_series_iter:
                 resource_column, metric_key = key_lambda(column)
                 metric = settings.metric_by_key(metric_key)
                 resource = settings.resource_by_key(resource_column)
```

### Comparing `waylay-beta-0.5.0/waylay/service/timeseries/parser/model.py` & `waylay-beta-0.6.0/waylay/service/timeseries/parser/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -373,15 +373,15 @@
     )
     AUTO = (
         'auto', 'Parse numeric value as unix epoch or ISO. Render ISO timestamp',
         '2020-09-17T01:38:59+00:00', r'^auto.*',
         parse_timestamp_auto,
         lambda t: t.isoformat(),
     )
-    value: str
+
     description: str
     example: Any
     _spec_matcher: Pattern
     # wrapping in a tuple to avoid mypy interpreting callable members as methods
     _parse: Tuple[Callable[[Any], datetime]]
     _format: Tuple[Callable[[datetime], Any]]
     _timezone_dependent: bool
@@ -448,14 +448,18 @@
         formatter = self._format[0]
         if not self._timezone_dependent:
             return formatter
 
         timezone = self._parse_tz(tz)
         return lambda ts: formatter(ts.astimezone(timezone))
 
+    def __str__(self):
+        """Get the string representation."""
+        return self.value
+
 
 @dataclass
 class SeriesSettings:
     """Settings for the mapping of an input (import) or CSV output (export).
 
     Attributes:
         metric_column:
@@ -800,15 +804,14 @@
     TarFile
 ]
 
 
 class ArchiveType(str, Enum):
     """Typed enumeration of supported archive import and export types."""
 
-    value: str
     description: str
     supports_multiple_files: bool
     expected_suffixes: List[str]
     excluded_suffixes: List[str]
     is_dir_type: bool
 
     def __new__(
@@ -837,14 +840,18 @@
     DIR = ('dir', 'Directory with csv text files.', True, None, None, True)
     DIR_GZ = ('dirgz', 'Directory with compressed csv text files.', True, None, None, True)
     ZIP = ('zip', 'Zip archive of csv text files.', True, ['.zip'])
     GZ = ('gz', 'Single compressed csv text file.', False, ['.gz'], ['.tar'])
     TAR = ('tar', 'Tar archive of csv text files.', True, ['.tar'], ['.gz'])
     TAR_GZ = ('targz', 'Compressed Tar archive of csv text files.', True, ['.tar', '.gz'])
 
+    def __str__(self):
+        """Get the string representation."""
+        return self.value
+
     @classmethod
     def lookup(cls, value: Optional[str]) -> Optional['ArchiveType']:
         """Lookup an enum object from a str value."""
         if value is None:
             return None
         # workaround for lint and typing issues with replaced __new__ for enums
         # pylint: disable=no-value-for-parameter
```

### Comparing `waylay-beta-0.5.0/waylay/service/timeseries/parser/util.py` & `waylay-beta-0.6.0/waylay/service/timeseries/parser/util.py`

 * *Files identical despite different names*

### Comparing `waylay-beta-0.5.0/waylay/service/timeseries/tool.py` & `waylay-beta-0.6.0/waylay/service/timeseries/tool.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,28 +60,36 @@
 class ResourceUpdateLevel(str, Enum):
     """The possible detail levels at which Waylay Resources can be updated during an ETL import job."""
 
     NONE = 'none'
     ID = 'id'
     ALL = 'all'
 
+    def __str__(self):
+        """Get the string representation."""
+        return self.value
+
 
 class ETLImportStatus(str, Enum):
     """The possible states of an ETL import job.
 
     These correspond to the subfolders of the 'etl-import' bucket (except for 'not_found').
     """
 
     UPLOAD = 'upload'
     BUSY = 'busy'
     FAILED = 'failed'
     IGNORED = 'ignored'
     DONE = 'done'
     NOT_FOUND = 'not_found'
 
+    def __str__(self):
+        """Get the string representation."""
+        return self.value
+
 
 ETL_IMPORT_STATUS_MESSAGE = {
     ETLImportStatus.UPLOAD:
     'The upload has not been picked up by the ETL process. '
     'Please contact support if this persists.',
     ETLImportStatus.BUSY:
     'The upload is being processed by the ETL process.',
```

### Comparing `waylay-beta-0.5.0/waylay/service/util/_service.py` & `waylay-beta-0.6.0/waylay/service/util/_service.py`

 * *Files identical despite different names*

### Comparing `waylay-beta-0.5.0/waylay_beta.egg-info/PKG-INFO` & `waylay-beta-0.6.0/waylay_beta.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: waylay-beta
-Version: 0.5.0
+Version: 0.6.0
 Summary: beta release of the Waylay Python SDK
-Home-page: https://docs-io.waylay.io/#/api/sdk/python
+Home-page: https://docs.waylay.io/#/api/sdk/python
 Author: Waylay
 Author-email: info@waylay.io
 License: ISC
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: dev-3.7
@@ -39,15 +39,15 @@
 * importing and querying _timeseries_ data.
 * uploading your own _machine learning models_ for usage in the _Waylay Rule Engine_
 * provisioning waylay _resources_ and _resource types_.
 
 The SDK is optimised for interactive usage in [Jupyter Notebooks](https://jupyter.org/).
 
 ## Prerequisites
-This package requires a python runtime `3.7` or higher (validated up to `3.10`). 
+This package requires a python runtime `3.7` or higher (validated up to `3.11`). 
 For datascience purposes you typically want to prepare an anaconda environment:
 ```bash
 conda create --name my_waylay_env python=3.8
 conda activate my_waylay_env
 conda install jupyter
 pip install waylay-beta
 jupyter notebook 
@@ -57,21 +57,21 @@
 
 ```bash
 pip install waylay-beta
 ```
 
 ### BYOML dependencies
 
-If you want to prepare BYOML models ([Enterprise](http://docs.waylay.io/#/features/byoml/)|[IO](http://docs-io.waylay.io/#/features/byoml/)), _extra_ dependency configurations are available, that will check or install framework-specific dependencies.
+If you want to prepare BYOML models ([Enterprise](http://docs.waylay.io/#/features/byoml/)), _extra_ dependency configurations are available, that will check or install framework-specific dependencies.
 
 Either for a specific runtime:
-> byoml-xgboost-1.3, byoml-sklearn-0.24, byoml-xgboost-1.0, byoml-pytorch-1.4, byoml-custom-1.0, byoml-tensorflow-2.1, byoml-pytorch-1.5, byoml-pytorch-1.8, byoml-sklearn-0.22, byoml-tensorflow-2.4
+> byoml-pytorch-1.4, byoml-pytorch-1.5, byoml-pytorch-1.8, byoml-tensorflow-2.4, byoml-sklearn-0.24, byoml-tensorflow-2.1, byoml-xgboost-1.0, byoml-sklearn-0.22, byoml-xgboost-1.3, byoml-custom-1.0
 
 or for the default runtime of one of the supported frameworks:
-> byoml-sklearn, byoml-tensorflow, byoml-custom, byoml-pytorch, byoml-xgboost
+> byoml-tensorflow, byoml-xgboost, byoml-pytorch, byoml-sklearn, byoml-custom
 
 E.g. to install with sklearn dependencies for byoml:
 ```bash
 pip install waylay-beta['byoml-sklearn-0.24']
 ```
 or
 ```bash
@@ -84,27 +84,24 @@
 > waylay_client.byoml.runtimes.get('byoml-pytorch-1.8')
 {'framework': 'pytorch', 'framework_version': '1.8', 'name': 'byoml-pytorch-1.8', 'python_version': '3.7'}
 ```
 
 ## Quickstart
 
 * Login to the waylay console, and get hold of an _API key, API secret_ pair \[*>Settings>Authentication keys*\] 
-  > `[Enterprise]` [https:://console.waylay.io](https://console.waylay.io/administration/settings/keys) <br>
-  > `[IO]` [https:://console-io.waylay.io](https://console-io.waylay.io/administration/settings/keys)
+  > `[Enterprise]` [https:://console.waylay.io](https://console.waylay.io/administration/settings/keys)
 
 * Create an SDK client
   ```python
   from waylay import WaylayConfig, WaylayClient
   waylay_client = WaylayClient.from_profile()
   ```
   On first usage, this will prompt for a gateway endpoint,
-  > `[Enterprise]` api.waylay.io (default)<br> 
-  > `[IO]` api-io.waylay.io
+  > `[Enterprise]` api.waylay.io (default)
 
   and your _API key/API secret_ credentials. 
 
 For more details see 
-> `[Enterprise]` [https://docs.waylay.io](https://docs.waylay.io/api/sdk/python/)<br>
-> `[IO]` [https://docs-io.waylay.io](https://docs-io.waylay.io/#/api/sdk/python)
+> `[Enterprise]` [https://docs.waylay.io](https://docs.waylay.io/#/api/sdk/python)
 
 ## Usage Examples
 See [demo notebooks](https://github.com/waylayio/demo-general/tree/master/python-sdk) for the usage examples supported in the current release.
```

### Comparing `waylay-beta-0.5.0/waylay_beta.egg-info/SOURCES.txt` & `waylay-beta-0.6.0/waylay_beta.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -2,14 +2,17 @@
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 versioneer.py
 doc/byoml_runtimes.json
 doc/dist.README.md
+my_notes/client_from_token_test.py
+my_notes/route_csv.py
+my_notes/routes_csv.py
 waylay/__init__.py
 waylay/_version.py
 waylay/auth.py
 waylay/auth_interactive.py
 waylay/client.py
 waylay/config.py
 waylay/exceptions.py
```

### Comparing `waylay-beta-0.5.0/waylay_beta.egg-info/requires.txt` & `waylay-beta-0.6.0/waylay_beta.egg-info/requires.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 httpx
 simple-rest-client
 appdirs
 python-jose
-pandas
+pandas<2
 isodate
 joblib
 tqdm
 tenacity
 tabulate
 
+[:python_version < "3.10"]
+importlib_metadata
+
 [:python_version == "3.7"]
 typing_extensions
 
 [byoml-custom]
 dill==0.3.4
 
 [byoml-custom-1.0]
@@ -81,21 +84,22 @@
 pytest-cov
 pytest-mock
 mock
 pylint
 pycodestyle
 pydocstyle
 autopep8
-mypy
+mypy<0.990
 typing-inspect
 types-pytz
 types-setuptools
 types-tabulate
 pdoc
 
 [dev-3.10]
 
 [dev-3.7]
 
 [dev-3.8]
 
 [dev-3.9]
+build
```

