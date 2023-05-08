# Comparing `tmp/trialbot-0.3.9.1.tar.gz` & `tmp/trialbot-0.3.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/trialbot-0.3.9.1.tar", last modified: Fri Nov  4 09:31:27 2022, max compression
+gzip compressed data, was "dist/trialbot-0.3.9.2.tar", last modified: Fri Nov  4 13:11:01 2022, max compression
```

## Comparing `trialbot-0.3.9.1.tar` & `trialbot-0.3.9.2.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 zxarukas   (501) staff       (20)        0 2022-11-04 09:31:27.447601 trialbot-0.3.9.1/
--rw-r--r--   0 zxarukas   (501) staff       (20)      526 2022-11-04 09:31:27.447340 trialbot-0.3.9.1/PKG-INFO
--rw-r--r--   0 zxarukas   (501) staff       (20)       69 2021-06-24 13:24:41.000000 trialbot-0.3.9.1/README.md
--rw-r--r--   0 zxarukas   (501) staff       (20)       38 2022-11-04 09:31:27.447682 trialbot-0.3.9.1/setup.cfg
--rw-r--r--   0 zxarukas   (501) staff       (20)      652 2021-06-24 13:24:41.000000 trialbot-0.3.9.1/setup.py
-drwxr-xr-x   0 zxarukas   (501) staff       (20)        0 2022-11-04 09:31:27.431433 trialbot-0.3.9.1/trialbot/
--rw-r--r--   0 zxarukas   (501) staff       (20)       48 2022-11-04 09:30:54.000000 trialbot-0.3.9.1/trialbot/__init__.py
-drwxr-xr-x   0 zxarukas   (501) staff       (20)        0 2022-11-04 09:31:27.435680 trialbot-0.3.9.1/trialbot/data/
--rw-r--r--   0 zxarukas   (501) staff       (20)     1229 2021-08-05 08:16:04.000000 trialbot-0.3.9.1/trialbot/data/__init__.py
--rw-r--r--   0 zxarukas   (501) staff       (20)      564 2021-06-24 13:24:41.000000 trialbot-0.3.9.1/trialbot/data/_translation_base.py
--rw-r--r--   0 zxarukas   (501) staff       (20)     4030 2021-06-24 13:24:41.000000 trialbot-0.3.9.1/trialbot/data/dataset.py
-drwxr-xr-x   0 zxarukas   (501) staff       (20)        0 2022-11-04 09:31:27.438979 trialbot-0.3.9.1/trialbot/data/datasets/
--rw-r--r--   0 zxarukas   (501) staff       (20)        0 2021-06-24 13:24:41.000000 trialbot-0.3.9.1/trialbot/data/datasets/__init__.py
--rw-r--r--   0 zxarukas   (501) staff       (20)      539 2021-06-24 13:24:41.000000 trialbot-0.3.9.1/trialbot/data/datasets/consecutive_lines_dataset.py
--rw-r--r--   0 zxarukas   (501) staff       (20)     1015 2021-06-24 13:24:41.000000 trialbot-0.3.9.1/trialbot/data/datasets/file_dataset.py
--rw-r--r--   0 zxarukas   (501) staff       (20)      357 2021-06-24 13:24:41.000000 trialbot-0.3.9.1/trialbot/data/datasets/index_dataset.py
--rw-r--r--   0 zxarukas   (501) staff       (20)      223 2021-06-24 13:24:41.000000 trialbot-0.3.9.1/trialbot/data/datasets/json_dataset.py
--rw-r--r--   0 zxarukas   (501) staff       (20)      205 2021-06-24 13:24:41.000000 trialbot-0.3.9.1/trialbot/data/datasets/jsonl_dataset.py
--rw-r--r--   0 zxarukas   (501) staff       (20)     2244 2021-06-24 13:24:41.000000 trialbot-0.3.9.1/trialbot/data/datasets/pickle_dataset.py
--rw-r--r--   0 zxarukas   (501) staff       (20)     1821 2021-06-24 13:24:41.000000 trialbot-0.3.9.1/trialbot/data/datasets/redis_dataset.py
--rw-r--r--   0 zxarukas   (501) staff       (20)      436 2021-06-24 13:24:41.000000 trialbot-0.3.9.1/trialbot/data/datasets/seq2dict_dataset.py
--rw-r--r--   0 zxarukas   (501) staff       (20)      246 2021-06-24 13:24:41.000000 trialbot-0.3.9.1/trialbot/data/datasets/tabular_dataset.py
--rw-r--r--   0 zxarukas   (501) staff       (20)      908 2021-06-24 13:24:41.000000 trialbot-0.3.9.1/trialbot/data/datasets/tsv_dataset.py
--rw-r--r--   0 zxarukas   (501) staff       (20)      880 2021-06-24 13:24:41.000000 trialbot-0.3.9.1/trialbot/data/field.py
-drwxr-xr-x   0 zxarukas   (501) staff       (20)        0 2022-11-04 09:31:27.439679 trialbot-0.3.9.1/trialbot/data/fields/
--rw-r--r--   0 zxarukas   (501) staff       (20)       31 2021-06-24 13:24:41.000000 trialbot-0.3.9.1/trialbot/data/fields/__init__.py
--rw-r--r--   0 zxarukas   (501) staff       (20)     2889 2021-06-24 13:24:41.000000 trialbot-0.3.9.1/trialbot/data/fields/seq_field.py
--rw-r--r--   0 zxarukas   (501) staff       (20)     3246 2021-06-24 13:24:41.000000 trialbot-0.3.9.1/trialbot/data/iterator.py
-drwxr-xr-x   0 zxarukas   (501) staff       (20)        0 2022-11-04 09:31:27.440844 trialbot-0.3.9.1/trialbot/data/iterators/
--rw-r--r--   0 zxarukas   (501) staff       (20)      134 2021-06-24 13:24:41.000000 trialbot-0.3.9.1/trialbot/data/iterators/__init__.py
--rw-r--r--   0 zxarukas   (501) staff       (20)     3367 2021-06-24 13:24:41.000000 trialbot-0.3.9.1/trialbot/data/iterators/bucket_iterator.py
--rw-r--r--   0 zxarukas   (501) staff       (20)     1354 2021-06-24 13:24:41.000000 trialbot-0.3.9.1/trialbot/data/iterators/cluster_iterator.py
--rw-r--r--   0 zxarukas   (501) staff       (20)     3580 2021-06-25 08:26:10.000000 trialbot-0.3.9.1/trialbot/data/iterators/random_iterator.py
--rw-r--r--   0 zxarukas   (501) staff       (20)    28102 2021-06-24 13:24:41.000000 trialbot-0.3.9.1/trialbot/data/ns_vocabulary.py
--rw-r--r--   0 zxarukas   (501) staff       (20)     2328 2021-08-05 07:16:06.000000 trialbot-0.3.9.1/trialbot/data/translator.py
-drwxr-xr-x   0 zxarukas   (501) staff       (20)        0 2022-11-04 09:31:27.441783 trialbot-0.3.9.1/trialbot/data/translators/
--rw-r--r--   0 zxarukas   (501) staff       (20)       56 2021-08-05 08:16:04.000000 trialbot-0.3.9.1/trialbot/data/translators/__init__.py
--rw-r--r--   0 zxarukas   (501) staff       (20)     2029 2021-08-05 08:20:44.000000 trialbot-0.3.9.1/trialbot/data/translators/known_field_translator.py
-drwxr-xr-x   0 zxarukas   (501) staff       (20)        0 2022-11-04 09:31:27.444340 trialbot-0.3.9.1/trialbot/training/
--rw-r--r--   0 zxarukas   (501) staff       (20)      265 2021-06-24 13:24:41.000000 trialbot-0.3.9.1/trialbot/training/__init__.py
--rw-r--r--   0 zxarukas   (501) staff       (20)     8700 2021-06-24 13:24:41.000000 trialbot-0.3.9.1/trialbot/training/event_engine.py
--rw-r--r--   0 zxarukas   (501) staff       (20)     2557 2022-11-04 09:30:54.000000 trialbot-0.3.9.1/trialbot/training/extensions.py
--rw-r--r--   0 zxarukas   (501) staff       (20)     1199 2021-11-10 05:47:23.000000 trialbot-0.3.9.1/trialbot/training/hparamset.py
--rw-r--r--   0 zxarukas   (501) staff       (20)     1195 2021-11-08 13:15:31.000000 trialbot-0.3.9.1/trialbot/training/opt_parser.py
--rw-r--r--   0 zxarukas   (501) staff       (20)    13697 2022-11-04 09:30:54.000000 trialbot-0.3.9.1/trialbot/training/trial_bot.py
--rw-r--r--   0 zxarukas   (501) staff       (20)     1724 2021-06-24 13:24:41.000000 trialbot-0.3.9.1/trialbot/training/trial_registry.py
--rw-r--r--   0 zxarukas   (501) staff       (20)     1815 2021-06-24 13:24:41.000000 trialbot-0.3.9.1/trialbot/training/updater.py
-drwxr-xr-x   0 zxarukas   (501) staff       (20)        0 2022-11-04 09:31:27.445263 trialbot-0.3.9.1/trialbot/training/updaters/
--rw-r--r--   0 zxarukas   (501) staff       (20)        0 2021-06-24 13:24:41.000000 trialbot-0.3.9.1/trialbot/training/updaters/__init__.py
--rw-r--r--   0 zxarukas   (501) staff       (20)     1689 2021-11-08 13:15:31.000000 trialbot-0.3.9.1/trialbot/training/updaters/testing_updater.py
--rw-r--r--   0 zxarukas   (501) staff       (20)     3154 2021-11-10 05:47:23.000000 trialbot-0.3.9.1/trialbot/training/updaters/training_updater.py
-drwxr-xr-x   0 zxarukas   (501) staff       (20)        0 2022-11-04 09:31:27.446974 trialbot-0.3.9.1/trialbot/utils/
--rw-r--r--   0 zxarukas   (501) staff       (20)        0 2021-06-24 13:24:41.000000 trialbot-0.3.9.1/trialbot/utils/__init__.py
--rw-r--r--   0 zxarukas   (501) staff       (20)     1075 2021-06-24 13:24:41.000000 trialbot-0.3.9.1/trialbot/utils/file_reader.py
--rw-r--r--   0 zxarukas   (501) staff       (20)      256 2021-06-24 13:24:41.000000 trialbot-0.3.9.1/trialbot/utils/fix_seed.py
--rw-r--r--   0 zxarukas   (501) staff       (20)     1737 2021-06-24 13:24:41.000000 trialbot-0.3.9.1/trialbot/utils/grid_search_helper.py
--rw-r--r--   0 zxarukas   (501) staff       (20)     1180 2021-06-24 13:24:41.000000 trialbot-0.3.9.1/trialbot/utils/move_to_device.py
--rw-r--r--   0 zxarukas   (501) staff       (20)     1119 2021-06-24 13:24:41.000000 trialbot-0.3.9.1/trialbot/utils/root_finder.py
-drwxr-xr-x   0 zxarukas   (501) staff       (20)        0 2022-11-04 09:31:27.432488 trialbot-0.3.9.1/trialbot.egg-info/
--rw-r--r--   0 zxarukas   (501) staff       (20)      526 2022-11-04 09:31:27.000000 trialbot-0.3.9.1/trialbot.egg-info/PKG-INFO
--rw-r--r--   0 zxarukas   (501) staff       (20)     1704 2022-11-04 09:31:27.000000 trialbot-0.3.9.1/trialbot.egg-info/SOURCES.txt
--rw-r--r--   0 zxarukas   (501) staff       (20)        1 2022-11-04 09:31:27.000000 trialbot-0.3.9.1/trialbot.egg-info/dependency_links.txt
--rw-r--r--   0 zxarukas   (501) staff       (20)        9 2022-11-04 09:31:27.000000 trialbot-0.3.9.1/trialbot.egg-info/top_level.txt
+drwxr-xr-x   0 zxarukas   (501) staff       (20)        0 2022-11-04 13:11:01.502401 trialbot-0.3.9.2/
+-rw-r--r--   0 zxarukas   (501) staff       (20)      526 2022-11-04 13:11:01.501751 trialbot-0.3.9.2/PKG-INFO
+-rw-r--r--   0 zxarukas   (501) staff       (20)       69 2021-06-24 13:24:41.000000 trialbot-0.3.9.2/README.md
+-rw-r--r--   0 zxarukas   (501) staff       (20)       38 2022-11-04 13:11:01.502592 trialbot-0.3.9.2/setup.cfg
+-rw-r--r--   0 zxarukas   (501) staff       (20)      652 2021-06-24 13:24:41.000000 trialbot-0.3.9.2/setup.py
+drwxr-xr-x   0 zxarukas   (501) staff       (20)        0 2022-11-04 13:11:01.486135 trialbot-0.3.9.2/trialbot/
+-rw-r--r--   0 zxarukas   (501) staff       (20)       48 2022-11-04 13:10:37.000000 trialbot-0.3.9.2/trialbot/__init__.py
+drwxr-xr-x   0 zxarukas   (501) staff       (20)        0 2022-11-04 13:11:01.489961 trialbot-0.3.9.2/trialbot/data/
+-rw-r--r--   0 zxarukas   (501) staff       (20)     1229 2021-08-05 08:16:04.000000 trialbot-0.3.9.2/trialbot/data/__init__.py
+-rw-r--r--   0 zxarukas   (501) staff       (20)      564 2021-06-24 13:24:41.000000 trialbot-0.3.9.2/trialbot/data/_translation_base.py
+-rw-r--r--   0 zxarukas   (501) staff       (20)     4030 2021-06-24 13:24:41.000000 trialbot-0.3.9.2/trialbot/data/dataset.py
+drwxr-xr-x   0 zxarukas   (501) staff       (20)        0 2022-11-04 13:11:01.493733 trialbot-0.3.9.2/trialbot/data/datasets/
+-rw-r--r--   0 zxarukas   (501) staff       (20)        0 2021-06-24 13:24:41.000000 trialbot-0.3.9.2/trialbot/data/datasets/__init__.py
+-rw-r--r--   0 zxarukas   (501) staff       (20)      539 2021-06-24 13:24:41.000000 trialbot-0.3.9.2/trialbot/data/datasets/consecutive_lines_dataset.py
+-rw-r--r--   0 zxarukas   (501) staff       (20)     1015 2021-06-24 13:24:41.000000 trialbot-0.3.9.2/trialbot/data/datasets/file_dataset.py
+-rw-r--r--   0 zxarukas   (501) staff       (20)      357 2021-06-24 13:24:41.000000 trialbot-0.3.9.2/trialbot/data/datasets/index_dataset.py
+-rw-r--r--   0 zxarukas   (501) staff       (20)      223 2021-06-24 13:24:41.000000 trialbot-0.3.9.2/trialbot/data/datasets/json_dataset.py
+-rw-r--r--   0 zxarukas   (501) staff       (20)      205 2021-06-24 13:24:41.000000 trialbot-0.3.9.2/trialbot/data/datasets/jsonl_dataset.py
+-rw-r--r--   0 zxarukas   (501) staff       (20)     2244 2021-06-24 13:24:41.000000 trialbot-0.3.9.2/trialbot/data/datasets/pickle_dataset.py
+-rw-r--r--   0 zxarukas   (501) staff       (20)     1821 2021-06-24 13:24:41.000000 trialbot-0.3.9.2/trialbot/data/datasets/redis_dataset.py
+-rw-r--r--   0 zxarukas   (501) staff       (20)      436 2021-06-24 13:24:41.000000 trialbot-0.3.9.2/trialbot/data/datasets/seq2dict_dataset.py
+-rw-r--r--   0 zxarukas   (501) staff       (20)      246 2021-06-24 13:24:41.000000 trialbot-0.3.9.2/trialbot/data/datasets/tabular_dataset.py
+-rw-r--r--   0 zxarukas   (501) staff       (20)      908 2021-06-24 13:24:41.000000 trialbot-0.3.9.2/trialbot/data/datasets/tsv_dataset.py
+-rw-r--r--   0 zxarukas   (501) staff       (20)      880 2021-06-24 13:24:41.000000 trialbot-0.3.9.2/trialbot/data/field.py
+drwxr-xr-x   0 zxarukas   (501) staff       (20)        0 2022-11-04 13:11:01.494389 trialbot-0.3.9.2/trialbot/data/fields/
+-rw-r--r--   0 zxarukas   (501) staff       (20)       31 2021-06-24 13:24:41.000000 trialbot-0.3.9.2/trialbot/data/fields/__init__.py
+-rw-r--r--   0 zxarukas   (501) staff       (20)     2889 2021-06-24 13:24:41.000000 trialbot-0.3.9.2/trialbot/data/fields/seq_field.py
+-rw-r--r--   0 zxarukas   (501) staff       (20)     3246 2021-06-24 13:24:41.000000 trialbot-0.3.9.2/trialbot/data/iterator.py
+drwxr-xr-x   0 zxarukas   (501) staff       (20)        0 2022-11-04 13:11:01.495618 trialbot-0.3.9.2/trialbot/data/iterators/
+-rw-r--r--   0 zxarukas   (501) staff       (20)      134 2021-06-24 13:24:41.000000 trialbot-0.3.9.2/trialbot/data/iterators/__init__.py
+-rw-r--r--   0 zxarukas   (501) staff       (20)     3367 2021-06-24 13:24:41.000000 trialbot-0.3.9.2/trialbot/data/iterators/bucket_iterator.py
+-rw-r--r--   0 zxarukas   (501) staff       (20)     1354 2021-06-24 13:24:41.000000 trialbot-0.3.9.2/trialbot/data/iterators/cluster_iterator.py
+-rw-r--r--   0 zxarukas   (501) staff       (20)     3580 2021-06-25 08:26:10.000000 trialbot-0.3.9.2/trialbot/data/iterators/random_iterator.py
+-rw-r--r--   0 zxarukas   (501) staff       (20)    28102 2021-06-24 13:24:41.000000 trialbot-0.3.9.2/trialbot/data/ns_vocabulary.py
+-rw-r--r--   0 zxarukas   (501) staff       (20)     2328 2021-08-05 07:16:06.000000 trialbot-0.3.9.2/trialbot/data/translator.py
+drwxr-xr-x   0 zxarukas   (501) staff       (20)        0 2022-11-04 13:11:01.496203 trialbot-0.3.9.2/trialbot/data/translators/
+-rw-r--r--   0 zxarukas   (501) staff       (20)       56 2021-08-05 08:16:04.000000 trialbot-0.3.9.2/trialbot/data/translators/__init__.py
+-rw-r--r--   0 zxarukas   (501) staff       (20)     2029 2021-08-05 08:20:44.000000 trialbot-0.3.9.2/trialbot/data/translators/known_field_translator.py
+drwxr-xr-x   0 zxarukas   (501) staff       (20)        0 2022-11-04 13:11:01.498258 trialbot-0.3.9.2/trialbot/training/
+-rw-r--r--   0 zxarukas   (501) staff       (20)      265 2021-06-24 13:24:41.000000 trialbot-0.3.9.2/trialbot/training/__init__.py
+-rw-r--r--   0 zxarukas   (501) staff       (20)     8700 2021-06-24 13:24:41.000000 trialbot-0.3.9.2/trialbot/training/event_engine.py
+-rw-r--r--   0 zxarukas   (501) staff       (20)     2478 2022-11-04 13:10:37.000000 trialbot-0.3.9.2/trialbot/training/extensions.py
+-rw-r--r--   0 zxarukas   (501) staff       (20)     1199 2021-11-10 05:47:23.000000 trialbot-0.3.9.2/trialbot/training/hparamset.py
+-rw-r--r--   0 zxarukas   (501) staff       (20)     1195 2021-11-08 13:15:31.000000 trialbot-0.3.9.2/trialbot/training/opt_parser.py
+-rw-r--r--   0 zxarukas   (501) staff       (20)    13697 2022-11-04 09:30:54.000000 trialbot-0.3.9.2/trialbot/training/trial_bot.py
+-rw-r--r--   0 zxarukas   (501) staff       (20)     1724 2021-06-24 13:24:41.000000 trialbot-0.3.9.2/trialbot/training/trial_registry.py
+-rw-r--r--   0 zxarukas   (501) staff       (20)     1815 2021-06-24 13:24:41.000000 trialbot-0.3.9.2/trialbot/training/updater.py
+drwxr-xr-x   0 zxarukas   (501) staff       (20)        0 2022-11-04 13:11:01.498973 trialbot-0.3.9.2/trialbot/training/updaters/
+-rw-r--r--   0 zxarukas   (501) staff       (20)        0 2021-06-24 13:24:41.000000 trialbot-0.3.9.2/trialbot/training/updaters/__init__.py
+-rw-r--r--   0 zxarukas   (501) staff       (20)     1689 2021-11-08 13:15:31.000000 trialbot-0.3.9.2/trialbot/training/updaters/testing_updater.py
+-rw-r--r--   0 zxarukas   (501) staff       (20)     3154 2021-11-10 05:47:23.000000 trialbot-0.3.9.2/trialbot/training/updaters/training_updater.py
+drwxr-xr-x   0 zxarukas   (501) staff       (20)        0 2022-11-04 13:11:01.500786 trialbot-0.3.9.2/trialbot/utils/
+-rw-r--r--   0 zxarukas   (501) staff       (20)        0 2021-06-24 13:24:41.000000 trialbot-0.3.9.2/trialbot/utils/__init__.py
+-rw-r--r--   0 zxarukas   (501) staff       (20)     1075 2021-06-24 13:24:41.000000 trialbot-0.3.9.2/trialbot/utils/file_reader.py
+-rw-r--r--   0 zxarukas   (501) staff       (20)      256 2021-06-24 13:24:41.000000 trialbot-0.3.9.2/trialbot/utils/fix_seed.py
+-rw-r--r--   0 zxarukas   (501) staff       (20)     1737 2021-06-24 13:24:41.000000 trialbot-0.3.9.2/trialbot/utils/grid_search_helper.py
+-rw-r--r--   0 zxarukas   (501) staff       (20)     1180 2021-06-24 13:24:41.000000 trialbot-0.3.9.2/trialbot/utils/move_to_device.py
+-rw-r--r--   0 zxarukas   (501) staff       (20)     1119 2021-06-24 13:24:41.000000 trialbot-0.3.9.2/trialbot/utils/root_finder.py
+drwxr-xr-x   0 zxarukas   (501) staff       (20)        0 2022-11-04 13:11:01.487753 trialbot-0.3.9.2/trialbot.egg-info/
+-rw-r--r--   0 zxarukas   (501) staff       (20)      526 2022-11-04 13:11:01.000000 trialbot-0.3.9.2/trialbot.egg-info/PKG-INFO
+-rw-r--r--   0 zxarukas   (501) staff       (20)     1704 2022-11-04 13:11:01.000000 trialbot-0.3.9.2/trialbot.egg-info/SOURCES.txt
+-rw-r--r--   0 zxarukas   (501) staff       (20)        1 2022-11-04 13:11:01.000000 trialbot-0.3.9.2/trialbot.egg-info/dependency_links.txt
+-rw-r--r--   0 zxarukas   (501) staff       (20)        9 2022-11-04 13:11:01.000000 trialbot-0.3.9.2/trialbot.egg-info/top_level.txt
```

### Comparing `trialbot-0.3.9.1/PKG-INFO` & `trialbot-0.3.9.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trialbot
-Version: 0.3.9.1
+Version: 0.3.9.2
 Summary: A lightweight training framework for PyTorch
 Home-page: https://github.com/zxteloiv/trialbot
 Author: zxteloiv
 Author-email: zxteloiv@gmail.com
 License: UNKNOWN
 Description: # TrialBot
         A lightweight framework for training networks in pytorch.
```

### Comparing `trialbot-0.3.9.1/setup.py` & `trialbot-0.3.9.2/setup.py`

 * *Files identical despite different names*

### Comparing `trialbot-0.3.9.1/trialbot/data/__init__.py` & `trialbot-0.3.9.2/trialbot/data/__init__.py`

 * *Files identical despite different names*

### Comparing `trialbot-0.3.9.1/trialbot/data/_translation_base.py` & `trialbot-0.3.9.2/trialbot/data/_translation_base.py`

 * *Files identical despite different names*

### Comparing `trialbot-0.3.9.1/trialbot/data/dataset.py` & `trialbot-0.3.9.2/trialbot/data/dataset.py`

 * *Files identical despite different names*

### Comparing `trialbot-0.3.9.1/trialbot/data/datasets/consecutive_lines_dataset.py` & `trialbot-0.3.9.2/trialbot/data/datasets/consecutive_lines_dataset.py`

 * *Files identical despite different names*

### Comparing `trialbot-0.3.9.1/trialbot/data/datasets/file_dataset.py` & `trialbot-0.3.9.2/trialbot/data/datasets/file_dataset.py`

 * *Files identical despite different names*

### Comparing `trialbot-0.3.9.1/trialbot/data/datasets/pickle_dataset.py` & `trialbot-0.3.9.2/trialbot/data/datasets/pickle_dataset.py`

 * *Files identical despite different names*

### Comparing `trialbot-0.3.9.1/trialbot/data/datasets/redis_dataset.py` & `trialbot-0.3.9.2/trialbot/data/datasets/redis_dataset.py`

 * *Files identical despite different names*

### Comparing `trialbot-0.3.9.1/trialbot/data/datasets/tsv_dataset.py` & `trialbot-0.3.9.2/trialbot/data/datasets/tsv_dataset.py`

 * *Files identical despite different names*

### Comparing `trialbot-0.3.9.1/trialbot/data/field.py` & `trialbot-0.3.9.2/trialbot/data/field.py`

 * *Files identical despite different names*

### Comparing `trialbot-0.3.9.1/trialbot/data/fields/seq_field.py` & `trialbot-0.3.9.2/trialbot/data/fields/seq_field.py`

 * *Files identical despite different names*

### Comparing `trialbot-0.3.9.1/trialbot/data/iterator.py` & `trialbot-0.3.9.2/trialbot/data/iterator.py`

 * *Files identical despite different names*

### Comparing `trialbot-0.3.9.1/trialbot/data/iterators/bucket_iterator.py` & `trialbot-0.3.9.2/trialbot/data/iterators/bucket_iterator.py`

 * *Files identical despite different names*

### Comparing `trialbot-0.3.9.1/trialbot/data/iterators/cluster_iterator.py` & `trialbot-0.3.9.2/trialbot/data/iterators/cluster_iterator.py`

 * *Files identical despite different names*

### Comparing `trialbot-0.3.9.1/trialbot/data/iterators/random_iterator.py` & `trialbot-0.3.9.2/trialbot/data/iterators/random_iterator.py`

 * *Files identical despite different names*

### Comparing `trialbot-0.3.9.1/trialbot/data/ns_vocabulary.py` & `trialbot-0.3.9.2/trialbot/data/ns_vocabulary.py`

 * *Files identical despite different names*

### Comparing `trialbot-0.3.9.1/trialbot/data/translator.py` & `trialbot-0.3.9.2/trialbot/data/translator.py`

 * *Files identical despite different names*

### Comparing `trialbot-0.3.9.1/trialbot/data/translators/known_field_translator.py` & `trialbot-0.3.9.2/trialbot/data/translators/known_field_translator.py`

 * *Files identical despite different names*

### Comparing `trialbot-0.3.9.1/trialbot/training/event_engine.py` & `trialbot-0.3.9.2/trialbot/training/event_engine.py`

 * *Files identical despite different names*

### Comparing `trialbot-0.3.9.1/trialbot/training/extensions.py` & `trialbot-0.3.9.2/trialbot/training/extensions.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import datetime
 import torch
 import math
 import os.path
-from trialbot.training.trial_bot import TrialBot
 
 
 def ext_write_info(bot, msg):
     bot.logger.info(msg)
 
 
 def current_epoch_logger(bot):
@@ -51,32 +50,32 @@
     bot.logger.info(f"Hyperparamset Used: {bot.args.hparamset}\n{str(bot.hparams)}")
 
 
 def print_snaptshot_path(bot):
     bot.logger.info("Snapshot Dir: " + bot.savepath)
 
 
-def print_models(bot: TrialBot):
+def print_models(bot):
     bot.logger.info("Model Specs:\n" + str(bot.models))
 
 
-def collect_garbage(bot: TrialBot):
+def collect_garbage(bot):
     import gc
     for optim in bot.updater._optims:
         optim.zero_grad()
 
     if hasattr(bot.state, "output") and bot.state.output is not None:
         bot.state.output = None
     gc.collect()
     if bot.args.device >= 0:
         import torch.cuda
         torch.cuda.empty_cache()
 
 
-def end_with_nan_loss(bot: TrialBot):
+def end_with_nan_loss(bot):
     import numpy as np
     output = getattr(bot.state, 'output', None)
     if output is None:
         return
     loss = output["loss"]
 
     def _isnan(x):
```

### Comparing `trialbot-0.3.9.1/trialbot/training/hparamset.py` & `trialbot-0.3.9.2/trialbot/training/hparamset.py`

 * *Files identical despite different names*

### Comparing `trialbot-0.3.9.1/trialbot/training/opt_parser.py` & `trialbot-0.3.9.2/trialbot/training/opt_parser.py`

 * *Files identical despite different names*

### Comparing `trialbot-0.3.9.1/trialbot/training/trial_bot.py` & `trialbot-0.3.9.2/trialbot/training/trial_bot.py`

 * *Files identical despite different names*

### Comparing `trialbot-0.3.9.1/trialbot/training/trial_registry.py` & `trialbot-0.3.9.2/trialbot/training/trial_registry.py`

 * *Files identical despite different names*

### Comparing `trialbot-0.3.9.1/trialbot/training/updater.py` & `trialbot-0.3.9.2/trialbot/training/updater.py`

 * *Files identical despite different names*

### Comparing `trialbot-0.3.9.1/trialbot/training/updaters/testing_updater.py` & `trialbot-0.3.9.2/trialbot/training/updaters/testing_updater.py`

 * *Files identical despite different names*

### Comparing `trialbot-0.3.9.1/trialbot/training/updaters/training_updater.py` & `trialbot-0.3.9.2/trialbot/training/updaters/training_updater.py`

 * *Files identical despite different names*

### Comparing `trialbot-0.3.9.1/trialbot/utils/file_reader.py` & `trialbot-0.3.9.2/trialbot/utils/file_reader.py`

 * *Files identical despite different names*

### Comparing `trialbot-0.3.9.1/trialbot/utils/grid_search_helper.py` & `trialbot-0.3.9.2/trialbot/utils/grid_search_helper.py`

 * *Files identical despite different names*

### Comparing `trialbot-0.3.9.1/trialbot/utils/move_to_device.py` & `trialbot-0.3.9.2/trialbot/utils/move_to_device.py`

 * *Files identical despite different names*

### Comparing `trialbot-0.3.9.1/trialbot/utils/root_finder.py` & `trialbot-0.3.9.2/trialbot/utils/root_finder.py`

 * *Files identical despite different names*

### Comparing `trialbot-0.3.9.1/trialbot.egg-info/PKG-INFO` & `trialbot-0.3.9.2/trialbot.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trialbot
-Version: 0.3.9.1
+Version: 0.3.9.2
 Summary: A lightweight training framework for PyTorch
 Home-page: https://github.com/zxteloiv/trialbot
 Author: zxteloiv
 Author-email: zxteloiv@gmail.com
 License: UNKNOWN
 Description: # TrialBot
         A lightweight framework for training networks in pytorch.
```

### Comparing `trialbot-0.3.9.1/trialbot.egg-info/SOURCES.txt` & `trialbot-0.3.9.2/trialbot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

