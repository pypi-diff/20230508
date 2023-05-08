# Comparing `tmp/transphone-1.3.9.tar.gz` & `tmp/transphone-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/transphone-1.3.9.tar", last modified: Sat Mar 25 01:51:33 2023, max compression
+gzip compressed data, was "dist/transphone-1.4.0.tar", last modified: Mon May  8 16:32:49 2023, max compression
```

## Comparing `transphone-1.3.9.tar` & `transphone-1.4.0.tar`

### file list

```diff
@@ -1,60 +1,66 @@
-drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-03-25 01:51:33.000000 transphone-1.3.9/
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1072 2022-10-27 20:49:08.000000 transphone-1.3.9/LICENSE
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      260 2023-03-25 01:51:33.000000 transphone-1.3.9/PKG-INFO
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     7080 2023-03-06 21:54:56.000000 transphone-1.3.9/README.md
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)       38 2023-03-25 01:51:33.000000 transphone-1.3.9/setup.cfg
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      387 2023-03-25 01:51:01.000000 transphone-1.3.9/setup.py
-drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-03-25 01:51:33.000000 transphone-1.3.9/test/
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     2587 2023-03-25 01:51:01.000000 transphone-1.3.9/test/test_tokenizer.py
-drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-03-25 01:51:33.000000 transphone-1.3.9/transphone/
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)       47 2022-11-23 17:53:06.000000 transphone-1.3.9/transphone/__init__.py
-drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-03-25 01:51:33.000000 transphone-1.3.9/transphone/bin/
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        0 2022-09-08 17:58:22.000000 transphone-1.3.9/transphone/bin/__init__.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1414 2022-09-08 18:29:41.000000 transphone-1.3.9/transphone/bin/download_model.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      331 2023-01-10 23:31:10.000000 transphone-1.3.9/transphone/config.py
-drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-03-25 01:51:33.000000 transphone-1.3.9/transphone/data/
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        0 2022-09-08 17:58:30.000000 transphone-1.3.9/transphone/data/__init__.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     5540 2022-09-08 18:03:50.000000 transphone-1.3.9/transphone/data/dataset.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1782 2022-09-08 18:03:50.000000 transphone-1.3.9/transphone/data/grapheme.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      408 2022-09-08 18:03:50.000000 transphone-1.3.9/transphone/data/loader.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      851 2022-09-08 18:03:50.000000 transphone-1.3.9/transphone/data/utils.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1046 2023-03-06 21:54:56.000000 transphone-1.3.9/transphone/data/vocab.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     8363 2023-03-06 21:54:56.000000 transphone-1.3.9/transphone/g2p.py
-drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-03-25 01:51:33.000000 transphone-1.3.9/transphone/lang/
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        0 2022-11-23 19:17:09.000000 transphone-1.3.9/transphone/lang/__init__.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1037 2023-01-10 23:31:10.000000 transphone-1.3.9/transphone/lang/base_tokenizer.py
-drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-03-25 01:51:33.000000 transphone-1.3.9/transphone/lang/cmn/
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        0 2022-11-23 19:17:09.000000 transphone-1.3.9/transphone/lang/cmn/__init__.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)    55821 2022-11-24 02:03:19.000000 transphone-1.3.9/transphone/lang/cmn/normalizer.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1605 2023-01-10 23:31:10.000000 transphone-1.3.9/transphone/lang/cmn/tokenizer.py
-drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-03-25 01:51:33.000000 transphone-1.3.9/transphone/lang/eng/
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        0 2022-11-23 19:17:09.000000 transphone-1.3.9/transphone/lang/eng/__init__.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1374 2022-11-29 19:11:51.000000 transphone-1.3.9/transphone/lang/eng/normalizer.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     2099 2023-01-10 23:31:10.000000 transphone-1.3.9/transphone/lang/eng/tokenizer.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     6499 2023-01-27 23:36:45.000000 transphone-1.3.9/transphone/lang/epitran_tokenizer.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1643 2023-02-14 03:41:43.000000 transphone-1.3.9/transphone/lang/g2p_tokenizer.py
-drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-03-25 01:51:33.000000 transphone-1.3.9/transphone/lang/jpn/
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        0 2022-11-23 19:17:09.000000 transphone-1.3.9/transphone/lang/jpn/__init__.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     9740 2022-11-25 20:08:08.000000 transphone-1.3.9/transphone/lang/jpn/conv_table.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)    15327 2022-11-25 20:04:35.000000 transphone-1.3.9/transphone/lang/jpn/jaconv.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     8088 2022-11-25 20:07:49.000000 transphone-1.3.9/transphone/lang/jpn/kana2phoneme.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     4336 2023-03-25 01:51:01.000000 transphone-1.3.9/transphone/lang/jpn/normalizer.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     2453 2023-03-25 01:51:01.000000 transphone-1.3.9/transphone/lang/jpn/tokenizer.py
-drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-03-25 01:51:33.000000 transphone-1.3.9/transphone/model/
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        0 2022-09-08 17:58:35.000000 transphone-1.3.9/transphone/model/__init__.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)    13153 2022-09-08 18:47:07.000000 transphone-1.3.9/transphone/model/checkpoint_utils.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     5388 2022-03-13 19:18:49.000000 transphone-1.3.9/transphone/model/ensemble.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     8330 2022-01-29 01:24:49.000000 transphone-1.3.9/transphone/model/lstm.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     7471 2023-02-14 03:41:43.000000 transphone-1.3.9/transphone/model/transformer.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     2393 2022-09-08 22:46:21.000000 transphone-1.3.9/transphone/model/utils.py
-drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-03-25 01:51:33.000000 transphone-1.3.9/transphone/pretrained/
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        0 2022-09-08 18:28:14.000000 transphone-1.3.9/transphone/pretrained/__init__.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     2408 2022-11-23 18:14:37.000000 transphone-1.3.9/transphone/run.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     3713 2023-03-06 21:54:56.000000 transphone-1.3.9/transphone/tokenizer.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      489 2023-01-10 21:01:40.000000 transphone-1.3.9/transphone/utils.py
-drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-03-25 01:51:33.000000 transphone-1.3.9/transphone.egg-info/
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      260 2023-03-25 01:51:33.000000 transphone-1.3.9/transphone.egg-info/PKG-INFO
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1302 2023-03-25 01:51:33.000000 transphone-1.3.9/transphone.egg-info/SOURCES.txt
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        1 2023-03-25 01:51:33.000000 transphone-1.3.9/transphone.egg-info/dependency_links.txt
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      111 2023-03-25 01:51:33.000000 transphone-1.3.9/transphone.egg-info/requires.txt
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)       11 2023-03-25 01:51:33.000000 transphone-1.3.9/transphone.egg-info/top_level.txt
+drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-08 16:32:49.000000 transphone-1.4.0/
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1072 2022-10-27 20:49:08.000000 transphone-1.4.0/LICENSE
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      260 2023-05-08 16:32:49.000000 transphone-1.4.0/PKG-INFO
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     7611 2023-05-08 16:31:27.000000 transphone-1.4.0/README.md
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)       38 2023-05-08 16:32:49.000000 transphone-1.4.0/setup.cfg
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      387 2023-05-08 16:31:27.000000 transphone-1.4.0/setup.py
+drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-08 16:32:49.000000 transphone-1.4.0/test/
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     2730 2023-05-08 16:31:27.000000 transphone-1.4.0/test/test_tokenizer.py
+drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-08 16:32:49.000000 transphone-1.4.0/transphone/
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)       47 2022-11-23 17:53:06.000000 transphone-1.4.0/transphone/__init__.py
+drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-08 16:32:49.000000 transphone-1.4.0/transphone/bin/
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        0 2022-09-08 17:58:22.000000 transphone-1.4.0/transphone/bin/__init__.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1545 2023-05-08 16:31:27.000000 transphone-1.4.0/transphone/bin/download_model.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     3451 2023-05-08 16:31:27.000000 transphone-1.4.0/transphone/bin/eval_epitran.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     3551 2023-05-08 16:31:27.000000 transphone-1.4.0/transphone/bin/eval_g2p.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     3634 2023-05-08 16:31:27.000000 transphone-1.4.0/transphone/bin/eval_zsl_g2p.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     2844 2023-05-08 16:31:27.000000 transphone-1.4.0/transphone/bin/g2p.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     2679 2023-05-08 16:31:27.000000 transphone-1.4.0/transphone/bin/tokenize.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     3816 2023-05-08 16:31:27.000000 transphone-1.4.0/transphone/bin/train_g2p.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1618 2023-05-08 16:31:27.000000 transphone-1.4.0/transphone/bin/update_model.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      325 2023-05-08 16:31:27.000000 transphone-1.4.0/transphone/config.py
+drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-08 16:32:49.000000 transphone-1.4.0/transphone/data/
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        0 2022-09-08 17:58:30.000000 transphone-1.4.0/transphone/data/__init__.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     9103 2023-05-08 16:31:27.000000 transphone-1.4.0/transphone/g2p.py
+drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-08 16:32:49.000000 transphone-1.4.0/transphone/lang/
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        0 2022-11-23 19:17:09.000000 transphone-1.4.0/transphone/lang/__init__.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1359 2023-05-08 16:31:27.000000 transphone-1.4.0/transphone/lang/base_tokenizer.py
+drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-08 16:32:49.000000 transphone-1.4.0/transphone/lang/cmn/
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        0 2022-11-23 19:17:09.000000 transphone-1.4.0/transphone/lang/cmn/__init__.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)    55821 2022-11-24 02:03:19.000000 transphone-1.4.0/transphone/lang/cmn/normalizer.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1605 2023-01-10 23:31:10.000000 transphone-1.4.0/transphone/lang/cmn/tokenizer.py
+drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-08 16:32:49.000000 transphone-1.4.0/transphone/lang/eng/
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        0 2022-11-23 19:17:09.000000 transphone-1.4.0/transphone/lang/eng/__init__.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     3341 2023-05-08 16:31:27.000000 transphone-1.4.0/transphone/lang/eng/normalizer.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     2099 2023-01-10 23:31:10.000000 transphone-1.4.0/transphone/lang/eng/tokenizer.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     6499 2023-01-27 23:36:45.000000 transphone-1.4.0/transphone/lang/epitran_tokenizer.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1645 2023-05-08 16:31:27.000000 transphone-1.4.0/transphone/lang/g2p_tokenizer.py
+drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-08 16:32:49.000000 transphone-1.4.0/transphone/lang/jpn/
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        0 2022-11-23 19:17:09.000000 transphone-1.4.0/transphone/lang/jpn/__init__.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     9740 2022-11-25 20:08:08.000000 transphone-1.4.0/transphone/lang/jpn/conv_table.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)    15327 2022-11-25 20:04:35.000000 transphone-1.4.0/transphone/lang/jpn/jaconv.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     9520 2023-05-08 16:31:27.000000 transphone-1.4.0/transphone/lang/jpn/kana2phoneme.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     5192 2023-05-08 16:31:27.000000 transphone-1.4.0/transphone/lang/jpn/normalizer.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     2637 2023-05-08 16:31:27.000000 transphone-1.4.0/transphone/lang/jpn/tokenizer.py
+drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-08 16:32:49.000000 transphone-1.4.0/transphone/model/
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        0 2022-09-08 17:58:35.000000 transphone-1.4.0/transphone/model/__init__.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)    13693 2023-05-08 16:31:27.000000 transphone-1.4.0/transphone/model/checkpoint_utils.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     6628 2023-05-08 16:31:27.000000 transphone-1.4.0/transphone/model/dataset.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     5388 2022-03-13 19:18:49.000000 transphone-1.4.0/transphone/model/ensemble.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1782 2023-05-08 16:31:27.000000 transphone-1.4.0/transphone/model/grapheme.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      409 2023-05-08 16:31:27.000000 transphone-1.4.0/transphone/model/loader.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     8331 2023-05-08 16:31:27.000000 transphone-1.4.0/transphone/model/lstm.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     7420 2023-05-08 16:31:27.000000 transphone-1.4.0/transphone/model/transformer.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1722 2023-05-08 16:31:27.000000 transphone-1.4.0/transphone/model/utils.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1046 2023-05-08 16:31:27.000000 transphone-1.4.0/transphone/model/vocab.py
+drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-08 16:32:49.000000 transphone-1.4.0/transphone/pretrained/
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        0 2022-09-08 18:28:14.000000 transphone-1.4.0/transphone/pretrained/__init__.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     2536 2023-05-08 16:31:27.000000 transphone-1.4.0/transphone/run.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     3764 2023-05-08 16:31:27.000000 transphone-1.4.0/transphone/tokenizer.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      491 2023-05-08 16:31:27.000000 transphone-1.4.0/transphone/utils.py
+drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-08 16:32:49.000000 transphone-1.4.0/transphone.egg-info/
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      260 2023-05-08 16:32:49.000000 transphone-1.4.0/transphone.egg-info/PKG-INFO
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1478 2023-05-08 16:32:49.000000 transphone-1.4.0/transphone.egg-info/SOURCES.txt
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        1 2023-05-08 16:32:49.000000 transphone-1.4.0/transphone.egg-info/dependency_links.txt
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      111 2023-05-08 16:32:49.000000 transphone-1.4.0/transphone.egg-info/requires.txt
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)       11 2023-05-08 16:32:49.000000 transphone-1.4.0/transphone.egg-info/top_level.txt
```

### Comparing `transphone-1.3.9/LICENSE` & `transphone-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `transphone-1.3.9/README.md` & `transphone-1.4.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
 ### Tokenizer interface
 
 The tokenizer converts a string into each languages' phonemes
 
 It will use the following strategy to decide pronunciation
 
-- it will first lookup lexicon dictionary for pronunciation (from Wikitionary)
+- it will first lookup lexicon dictionary for pronunciation (from Wikitionary, cmudict, and other sources)
 - try identifying rule-based transducer from [Epitran](https://github.com/dmort27/epitran) if supported.
 - fall back to the G2P engine if both previous options are not available.  
 
 Currently, more than 200 languages have lexicon available inside, about 100 languages have epitran supported. Other languages will use G2P instead.
 
 ```python
 In [1]: from transphone import read_tokenizer                                                                                                  
@@ -128,17 +128,21 @@
 gwe   ['t', 'l', 'a', 'n', 's', 'f', 'o', 'n', 'e']
 ibo   ['t', 'l', 'a', 'n', 's', 'p', 'o', 'n', 'e']
 kam   ['t', 'l', 'a', 'n', 's', 'f', 'o', 'n', 'e']
 kik   ['t', 'l', 'a', 'n', 's', 'f', 'ɔ', 'n', 'ɛ']
 Out[5]: ['t', 'l', 'a', 'n', 's', 'f', 'o', 'n', 'e']
 ```
 
-## Models
+## G2P Models
 
-| model | # supported languages |       description        |
-| :----: |:---------------------:|:------------------------:|
-| latest |          ~8k          | based on our work at [1] |
+You can see the G2P evaluation over 1k languages on the [performance doc](./doc/performance/README.md)
+
+Note this is the pure G2P evaluation on unseen words. The tokenizer combines other existing resources (i.e. lexicon) as well, so the tokenizer's performance is expected to be much better than this. 
+
+|        model         | # supported languages | supervised language PER | zero-shot language PER |       description        |
+|:--------------------:|:---------------------:|:-----------------------:|:----------------------:|:------------------------:|
+| 042801_base (latest) |          ~8k          |           13%           |          31%           | based on our work at [1] |
 
 ## Reference
 
 - [1] Li, Xinjian, et al. "Zero-shot Learning for Grapheme to Phoneme Conversion with Language Ensemble." Findings of the Association for Computational Linguistics: ACL 2022. 2022.
-- [2] Li, Xinjian, et al. "Phone Inventories and Recognition for Every Language" LREC 2022. 2022
+- [2] Li, Xinjian, et al. "Phone Inventories and Recognition for Every Language" LREC 2022. 2022
```

### Comparing `transphone-1.3.9/test/test_tokenizer.py` & `transphone-1.4.0/test/test_tokenizer.py`

 * *Files 19% similar despite different names*

```diff
@@ -12,14 +12,15 @@
         self.assertEqual(eng.tokenize('hello world'), ['h', 'ʌ', 'l', 'o', 'w', 'w', 'ɹ̩', 'l', 'd'])
 
     def test_jpn_tokenizer(self):
         jpn = read_tokenizer('jpn')
         self.assertEqual(jpn.tokenize_words('こんにちは世界'), ['こんにちは', '世界'])
         self.assertEqual(jpn.tokenize('こんにちは世界'), ['k', 'o', 'N', 'n', 'i', 'ch', 'i', 'w', 'a', 's', 'e', 'k', 'a', 'i'])
         self.assertEqual(jpn.tokenize('2023年'), ['n', 'i', 's', 'e', 'N', 'n', 'i', 'j', 'u', 'u', 's', 'a', 'N', 'n', 'e', 'N'])
+        self.assertEqual(jpn.tokenize('ＵTＦとABC。'),  ['y', 'uː', 't', 'iː', 'e', 'f', 'u', 't', 'o', 'eː', 'b', 'iː', 'sh', 'iː'])
 
     def test_spa_tokenizer(self):
 
         spa = read_tokenizer('spa')
         self.assertEqual(spa.tokenize('hola hola'), ['o', 'l', 'a', 'o', 'l', 'a'])
         self.assertEqual(spa.tokenize('español'),  ['e', 's', 'p', 'a', 'ɲ', 'o', 'l'])
```

### Comparing `transphone-1.3.9/transphone/bin/download_model.py` & `transphone-1.4.0/transphone/bin/download_model.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 from pathlib import Path
 import tarfile
 from urllib.request import urlopen
 import io
 import argparse
 import os
+from transphone.config import TransphoneConfig
+from transphone.model.utils import resolve_model_name
 
 
 def download_model(model_name=None, alt_model_path=None):
 
     if model_name is None:
         model_name = 'latest'
     if alt_model_path:
         model_dir = alt_model_path
     else:
-        model_dir = (Path(__file__).parent.parent) / 'pretrained' / 'model'
+        model_dir = TransphoneConfig.data_path / 'model'
         model_dir.mkdir(parents=True, exist_ok=True)
 
+    model_name = resolve_model_name(model_name)
+
     if not (model_dir / model_name).exists():
 
         try:
             url = 'https://github.com/xinjli/transphone/releases/download/v1.0/' + model_name + '.tar.gz'
             print("downloading model ", model_name)
             print("from: ", url)
             print("to:   ", str(model_dir))
```

### Comparing `transphone-1.3.9/transphone/data/grapheme.py` & `transphone-1.4.0/transphone/model/grapheme.py`

 * *Files identical despite different names*

### Comparing `transphone-1.3.9/transphone/data/vocab.py` & `transphone-1.4.0/transphone/model/vocab.py`

 * *Files identical despite different names*

### Comparing `transphone-1.3.9/transphone/g2p.py` & `transphone-1.4.0/transphone/g2p.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,90 +1,108 @@
-from phonepiece.iso import normalize_lang_id
+from phonepiece.lang import normalize_lang_id
 from transphone.model.checkpoint_utils import torch_load
 from transphone.model.transformer import TransformerG2P
 from transphone.model.ensemble import ensemble
 from transphone.bin.download_model import download_model
 from transphone.config import TransphoneConfig
-from transphone.data.vocab import Vocab
+from transphone.model.checkpoint_utils import find_topk_models
+from transphone.model.vocab import Vocab
+from transphone.model.utils import read_model_config
 from transphone.utils import Singleton
-from phonepiece.tree import read_tree
+from phonepiece.lang import read_tree
 from phonepiece.inventory import read_inventory
+from pathlib import Path
 import torch
 import unidecode
 from itertools import groupby
+from transphone.model.utils import resolve_model_name
 
 
-def read_g2p(model_name='latest', device=None, alt_model_path=None):
+def read_g2p(model_name='latest', device=None, checkpoint=None):
 
     if device is not None:
         assert device in ['cpu', 'cuda']
         TransphoneConfig.device = device
 
-    if alt_model_path:
-        # check whether a customized path is used or not
-        model_path = alt_model_path
-    else:
+    model_name = resolve_model_name(model_name)
+    cache_path = None
+
+    if checkpoint is None:
         model_path = TransphoneConfig.data_path / 'model' / model_name
 
-    # if not exists, we try to download the model
-    if not model_path.exists():
-        download_model(model_name)
+        # if not exists, we try to download the model
+        if not model_path.exists():
+            download_model(model_name)
+
+        if not model_path.exists():
+            raise ValueError(f"could not download or read {model_name} model")
+
+        if (model_path / "model.pt").exists():
+            checkpoint = model_path / "model.pt"
+        else:
+            checkpoint = find_topk_models(model_path)[0]
+
+        if (model_path / 'cache').exists():
+            cache_path = model_path / 'cache'
+        else:
+            cache_path = None
 
-    if not model_path.exists():
-        raise ValueError(f"could not download or read {model_name} inventory")
+    config = read_model_config(model_name)
 
-    model = G2P(model_path, {})
+    model = G2P(checkpoint, cache_path, config)
 
     return model
 
 
 class G2P(metaclass=Singleton):
 
-    def __init__(self, model_path, inference_config):
+    def __init__(self, checkpoint, cache_path, config):
 
-        self.model_path = model_path
-        self.grapheme_vocab = Vocab.read(model_path / 'grapheme.vocab')
-        self.phoneme_vocab = Vocab.read(model_path / 'phoneme.vocab')
-        self.inference_config = inference_config
+        self.model_path = Path(checkpoint).parent
+        self.grapheme_vocab = Vocab.read(self.model_path / 'grapheme.vocab')
+        self.phoneme_vocab = Vocab.read(self.model_path / 'phoneme.vocab')
+        self.config = config
+        self.checkpoint = checkpoint
+        self.cache_path = cache_path
 
         # setup available languages
         self.supervised_langs = []
         for word in self.grapheme_vocab.words[2:]:
             if len(word) == 5 and word[0] == '<' and word[-1] == '>':
                 self.supervised_langs.append(word[1:-1])
 
-
         # cache to find proper supervised language
         self.lang_map = {}
 
         # inventory
         self.lang2inv = {}
 
+        # lang2cache
+        self.lang2cache = {}
+
         # tree to estimate language's similarity
         self.tree = read_tree()
         self.tree.setup_target_langs(self.supervised_langs)
         self.supervised_langs = set(self.supervised_langs)
 
-
         SRC_VOCAB_SIZE = len(self.grapheme_vocab)+1
         TGT_VOCAB_SIZE = len(self.phoneme_vocab)+1
 
-        EMB_SIZE = 512
-        NHEAD = 8
-        FFN_HID_DIM = 512
-        NUM_ENCODER_LAYERS = 4
-        NUM_DECODER_LAYERS = 4
-        torch.manual_seed(0)
+        EMB_SIZE = config.embed_size
+        NHEAD = config.num_head
+        FFN_HID_DIM = config.hidden_size
+        NUM_ENCODER_LAYERS = config.num_encoder
+        NUM_DECODER_LAYERS = config.num_decoder
 
+        torch.manual_seed(0)
 
         self.model = TransformerG2P(NUM_ENCODER_LAYERS, NUM_DECODER_LAYERS, EMB_SIZE,
                             NHEAD, SRC_VOCAB_SIZE, TGT_VOCAB_SIZE, FFN_HID_DIM).to(TransphoneConfig.device)
 
-
-        torch_load(self.model, model_path / "model.pt")
+        torch_load(self.model, self.checkpoint)
 
 
     def get_target_langs(self, lang_id, num_lang=10, verbose=False, force_approximate=False):
 
         if lang_id in self.lang_map:
             target_langs = self.lang_map[lang_id]
         else:
```

### Comparing `transphone-1.3.9/transphone/lang/base_tokenizer.py` & `transphone-1.4.0/transphone/lang/base_tokenizer.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,23 +10,30 @@
 
         if g2p_model is None:
             self.g2p = None
         else:
             self.g2p = read_g2p(g2p_model, device)
 
         self.cache = {}
+
+        if self.g2p is not None and self.g2p.cache_path is not None:
+            lang_cache_path = self.g2p.cache_path / f"{lang_id}.txt"
+            if lang_cache_path.exists():
+                for line in open(lang_cache_path, 'r'):
+                    fields = line.strip().split()
+                    self.cache[fields[0]] = fields[1:]
+
         self.punctuation = '!"#$%&\'()*+,-./:;<=>?@[\\]^_`{|}~'
         self.logger = TransphoneConfig.logger
 
     def tokenize(self, text: str):
         raise NotImplementedError
 
     def tokenize_words(self, text:str):
         text = text.translate(str.maketrans('', '', self.punctuation)).lower()
-        result = []
 
         return text.split()
 
     def convert_tokens_to_ids(self, lst):
         lst = list(filter(lambda s: s!='<SPACE>', lst))
 
         return self.inventory.phoneme.atoi(lst)
```

### Comparing `transphone-1.3.9/transphone/lang/cmn/normalizer.py` & `transphone-1.4.0/transphone/lang/cmn/normalizer.py`

 * *Files identical despite different names*

### Comparing `transphone-1.3.9/transphone/lang/cmn/tokenizer.py` & `transphone-1.4.0/transphone/lang/cmn/tokenizer.py`

 * *Files identical despite different names*

### Comparing `transphone-1.3.9/transphone/lang/eng/tokenizer.py` & `transphone-1.4.0/transphone/lang/eng/tokenizer.py`

 * *Files identical despite different names*

### Comparing `transphone-1.3.9/transphone/lang/epitran_tokenizer.py` & `transphone-1.4.0/transphone/lang/epitran_tokenizer.py`

 * *Files identical despite different names*

### Comparing `transphone-1.3.9/transphone/lang/g2p_tokenizer.py` & `transphone-1.4.0/transphone/lang/g2p_tokenizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-from phonepiece.iso import normalize_lang_id
+from phonepiece.lang import normalize_lang_id
 from phonepiece.lexicon import read_lexicon
 from transphone.lang.base_tokenizer import BaseTokenizer
 
 
 class G2PTokenizer(BaseTokenizer):
 
     def __init__(self, lang_id, g2p_model='latest', device=None):
         super().__init__(lang_id, g2p_model, device)
 
         self.lexicon = read_lexicon(lang_id)
 
+
     def tokenize(self, text, use_g2p=True, use_space=False, verbose=False):
 
         norm_text = text.translate(str.maketrans('', '', self.punctuation)).lower()
         log = f"normalization: {text} -> {norm_text}"
         self.logger.info(log)
 
         if verbose:
```

### Comparing `transphone-1.3.9/transphone/lang/jpn/conv_table.py` & `transphone-1.4.0/transphone/lang/jpn/conv_table.py`

 * *Files identical despite different names*

### Comparing `transphone-1.3.9/transphone/lang/jpn/jaconv.py` & `transphone-1.4.0/transphone/lang/jpn/jaconv.py`

 * *Files identical despite different names*

### Comparing `transphone-1.3.9/transphone/lang/jpn/kana2phoneme.py` & `transphone-1.4.0/transphone/lang/jpn/kana2phoneme.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 from .conv_table import FULL_KANA
+from phonepiece.inventory import read_inventory
+from transphone.config import TransphoneConfig
 
 _kana2phonemes = {
     'ア': 'a',
     'イ': 'i',
     'ウ': 'u',
     'エ': 'e',
     'オ': 'o',
@@ -144,14 +146,17 @@
     'ー': 'ː'
 }
 
 import re
 
 class Kana2Phoneme:
     def __init__(self):
+
+        self.phoneme_set = set(read_inventory('jpn').phoneme.elems)
+
         self._dict1 = {
             'キャ': 'ky a ',
             'キュ': 'ky u ',
             'キョ': 'ky o ',
             'ギャ': 'gy a ',
             'ギュ': 'gy u ',
             'ギョ': 'gy o ',
@@ -288,14 +293,42 @@
             'ヲ': 'o ',
             'ヤ': 'y a ',
             'ユ': 'y u ',
             'ヨ': 'y o ',
             'ン': 'N ',
             'ッ': 'q ',
             'ー': 'ː ',
+            'ァ': 'a ',
+            'ィ': 'i ',
+            'ゥ': 'u ',
+            'ェ': 'e ',
+            'ォ': 'o ',
+            'ャ': 'y a ',
+            'ュ': 'y u ',
+            'ョ': 'y o ',
+            'ヮ': 'w a ',
+            'ヵ': 'k a ',
+            'ヶ': 'k e ',
+            'ヰ': 'i ',
+            'ヱ': 'e ',
+            'ヴ': 'b u ',
+            'ヽ': '',  # this should not reach here though
+            'ヾ': '',  # this should not reach here though
+            'ヷ': 'w a ',
+            'ヸ': 'i ',
+            'ヹ': 'e ',
+            'ヺ': 'o ',
+            'ヿ': '',  # this should not reach here though
+            '゛': '',  # this should not reach here though
+            '゜': '',  # this should not reach here though
+            'ヽ': '',  # this should not reach here though
+            'ヾ': '',  # this should not reach here though
+            'ゝ': '',  # this should not reach here though
+            'ゞ': '',  # this should not reach here though
+            '〆': '',  # this should not reach here though
             '々': '',  # this should not reach here though
         }
         self._regex1 = re.compile(u"(%s)" % u"|".join(map(re.escape, self._dict1.keys())))
         self._regex2 = re.compile(u"(%s)" % u"|".join(map(re.escape, self._dict2.keys())))
 
     def validate(self, text):
         for word in text.strip():
@@ -315,14 +348,17 @@
         ret = self._regex2.sub(lambda m: self._dict2[m.string[m.start():m.end()]], ret)
 
         temp_phonemes = ret.split()
 
         phonemes = []
         for temp_phoneme in temp_phonemes:
             if temp_phoneme == 'ː':
-                if len(phonemes) > 0:
+                if len(phonemes) > 0 and phonemes[-1] in ['a', 'i', 'u', 'e', 'o']:
                     phonemes[-1] = phonemes[-1]+'ː'
                 continue
 
-            phonemes.append(temp_phoneme)
+            if temp_phoneme in self.phoneme_set:
+                phonemes.append(temp_phoneme)
+            else:
+                TransphoneConfig.logger.error("Unknown phoneme: %s" % temp_phoneme)
 
         return phonemes
```

### Comparing `transphone-1.3.9/transphone/lang/jpn/normalizer.py` & `transphone-1.4.0/transphone/lang/jpn/normalizer.py`

 * *Files 27% similar despite different names*

```diff
@@ -100,14 +100,51 @@
                 read_list.append(sokuon_unit[n-i-1])
             else:
                 read_list.append(unit[n - i - 1])
     read_str = "".join(read_list)
     return read_str
 
 
+def parse_jpn_alphabet(text):
+
+    katakana_dict = {
+        'A': 'エー',
+        'B': 'ビー',
+        'C': 'シー',
+        'D': 'ディー',
+        'E': 'イー',
+        'F': 'エフ',
+        'G': 'ジー',
+        'H': 'エイチ',
+        'I': 'アイ',
+        'J': 'ジェー',
+        'K': 'ケー',
+        'L': 'エル',
+        'M': 'エム',
+        'N': 'エヌ',
+        'O': 'オー',
+        'P': 'ピー',
+        'Q': 'キュー',
+        'R': 'アール',
+        'S': 'エス',
+        'T': 'ティー',
+        'U': 'ユー',
+        'V': 'ブイ',
+        'W': 'ダブリュー',
+        'X': 'エックス',
+        'Y': 'ワイ',
+        'Z': 'ゼット',
+    }
+
+    katakana_text = ''
+    for char in text.upper():
+        if char in katakana_dict:
+            katakana_text += katakana_dict[char]
+    return katakana_text
+
 def parse_jpn_number(num):
 
     num_size = len(str(num))
     if num_size <= 4:
         return parse_small_jpn_number(num)
     elif num_size <= 8:
         low_digit = num%10000
```

### Comparing `transphone-1.3.9/transphone/lang/jpn/tokenizer.py` & `transphone-1.4.0/transphone/lang/jpn/tokenizer.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from transphone.utils import import_with_auto_install
 from transphone.lang.jpn.kana2phoneme import Kana2Phoneme
 from transphone.g2p import read_g2p
 from phonepiece.inventory import read_inventory
 from transphone.lang.jpn import jaconv
 from transphone.lang.base_tokenizer import BaseTokenizer
-from transphone.lang.jpn.normalizer import normalize_neologd, parse_jpn_number
+from transphone.lang.jpn.normalizer import normalize_neologd, parse_jpn_number, parse_jpn_alphabet
 
 class JPNTokenizer(BaseTokenizer):
 
     def __init__(self, lang_id, g2p_model='latest', device=None):
 
         super().__init__(lang_id, g2p_model, device)
 
@@ -29,15 +29,14 @@
         # exclude the last EOS word
         for word in raw_words[:-2]:
             raw = word.split('\t')[0]
             result.append(raw)
 
         return result
 
-
     def tokenize(self, text, use_g2p=True, use_space=False, verbose=False):
 
         text = normalize_neologd(text)
 
         raw_words = self.tagger.parse(text).split('\n')
 
         result = []
@@ -48,14 +47,18 @@
             kana = word.split('\t')[1]
             raw = word.split('\t')[0]
 
             if str.isdigit(raw):
                 hankaku_num = jaconv.z2h(kana)
                 kana = jaconv.hira2kata(parse_jpn_number(hankaku_num))
 
+            # interestingly, isalpha also return true for kana
+            if str.isalpha(raw) and str.isascii(raw):
+                kana = parse_jpn_alphabet(raw)
+
             res = self.kana2phoneme.convert(kana)
 
             if res == ['*'] and self.kana2phoneme.validate(raw):
                 res = self.kana2phoneme.convert(raw)
 
             if verbose:
                 print(kana, res)
```

### Comparing `transphone-1.3.9/transphone/model/checkpoint_utils.py` & `transphone-1.4.0/transphone/model/checkpoint_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,33 @@
 import re
 import traceback
 import shutil
 
 import torch
 from torch.serialization import default_restore_location
 from pathlib import Path
+from transphone.config import TransphoneConfig
+
+
+def find_topk_models(exp_name, topk=1):
+
+    if isinstance(exp_name, str):
+        exp_dir = TransphoneConfig.data_path / 'model' / exp_name
+    else:
+        assert isinstance(exp_name, Path)
+        exp_dir = exp_name
+
+    model_lst = []
+    for model_path in exp_dir.glob('model_*.pt'):
+        perf = model_path.stem.split('_')[1]
+        model_lst.append((float(perf), model_path))
+
+    model_lst.sort()
+    topk_models = [model[1] for model in model_lst[:topk]]
+    return topk_models
 
 
 def torch_save(model, path):
     """Save torch model states.
 
     Args:
         path (str): Model path to be saved.
```

### Comparing `transphone-1.3.9/transphone/model/ensemble.py` & `transphone-1.4.0/transphone/model/ensemble.py`

 * *Files identical despite different names*

### Comparing `transphone-1.3.9/transphone/model/lstm.py` & `transphone-1.4.0/transphone/model/lstm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import torch
 import torch.nn as nn
-from transphone.data.utils import pad_sos_eos
+from transphone.model.utils import pad_sos_eos
 import torch.nn.functional as F
 import math
 import numpy as np
 
 class Encoder(nn.Module):
 
     def __init__(self, vocab_size, hidden_size, layer_size):
```

### Comparing `transphone-1.3.9/transphone/model/transformer.py` & `transphone-1.4.0/transphone/model/transformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from torch import Tensor
 import torch
 import torch.nn as nn
 from torch.nn import Transformer
 import math
-from transphone.data.utils import pad_sos_eos
+from transphone.model.utils import pad_sos_eos
 from transphone.config import TransphoneConfig
 
 UNK_IDX, PAD_IDX, BOS_IDX, EOS_IDX = 0, 0, 1, 1
 
 def generate_square_subsequent_mask(sz):
     mask = (torch.triu(torch.ones((sz, sz), device=TransphoneConfig.device)) == 1).transpose(0, 1)
     mask = mask.float().masked_fill(mask == 0, float('-inf')).masked_fill(mask == 1, float(0.0))
@@ -64,15 +64,15 @@
                  num_decoder_layers: int,
                  emb_size: int,
                  nhead: int,
                  src_vocab_size: int,
                  tgt_vocab_size: int,
                  dim_feedforward: int = 512,
                  dropout: float = 0.1):
-        super(TransformerG2P, self).__init__()
+        super().__init__()
         self.transformer = Transformer(d_model=emb_size,
                                        nhead=nhead,
                                        num_encoder_layers=num_encoder_layers,
                                        num_decoder_layers=num_decoder_layers,
                                        dim_feedforward=dim_feedforward,
                                        dropout=dropout)
         self.generator = nn.Linear(emb_size, tgt_vocab_size)
@@ -104,15 +104,14 @@
     def decode(self, tgt: Tensor, memory: Tensor, tgt_mask: Tensor):
         return self.transformer.decoder(self.positional_encoding(self.tgt_tok_emb(tgt)), memory,tgt_mask)
 
 
     def train_step(self, x,y):
 
         self.train()
-        batch_size = x.shape[0]
 
         ys_in, ys_out = pad_sos_eos(y, 1, 1)
 
         # T,B
         tgt_input = ys_in.transpose(1,0)
         tgt_out = ys_out.transpose(1,0)
```

### Comparing `transphone-1.3.9/transphone/run.py` & `transphone-1.4.0/transphone/bin/g2p.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,69 +1,81 @@
-from transphone.g2p import read_g2p
 from transphone.bin.download_model import download_model
-from transphone.model.utils import get_all_models, resolve_model_name
+from transphone.model.utils import resolve_model_name
+from transphone.tokenizer import read_tokenizer
 from pathlib import Path
+from transphone.g2p import read_g2p
 import argparse
+import tqdm
 
-if __name__ == '__main__':
-
-    parser = argparse.ArgumentParser('running transphone g2p model')
-    parser.add_argument('-m', '--model', type=str, default='latest', help='specify which model to use. default is to use the latest local model')
-    parser.add_argument('-l', '--lang', type=str,  default='ipa',help='specify which language inventory to use for recognition. default is to use all phone inventory')
-    parser.add_argument('-i', '--input', type=str, required=True, help='specify your input wav file/directory')
-    parser.add_argument('-o', '--output', type=str, default='stdout', help='specify output file. the default will be stdout')
-    parser.add_argument('-c', '--combine', type=bool, default=False, help='write outputs by including both grapheme inputs and phonemes in the same line, delimited by space')
-
-    args = parser.parse_args()
+def run_g2p(model_name, lang, input, output, checkpoint=None, file_format='text', combine=False, ensemble=10, force_approximate=False):
 
     # download specified model automatically if no model exists
-    if len(get_all_models()) == 0:
-        download_model('latest')
-
-    # resolve model's name
-    model_name = resolve_model_name(args.model)
-    if model_name == "none":
-        print("Model ", model_name, " does not exist. Please download this model or use an existing model in list_model")
-        exit(0)
-
-    args.model = model_name
+    download_model(model_name)
 
     # create model
-    g2p = read_g2p(model_name)
+    model = read_g2p(model_name, checkpoint=checkpoint)
 
     # output file descriptor
     output_fd = None
-    if args.output != 'stdout':
-        output_fd = open(args.output, 'w', encoding='utf-8')
-
-    # cache infered words
-    word_cache = {}
+    if output != 'stdout':
+        output_fd = open(output, 'w', encoding='utf-8')
 
     # input file/path
-    input_path = Path(args.input)
+    input_path = Path(input)
 
-    for line in open(input_path, 'r'):
-        words = line.strip().split()
-        phoneme_lst = []
-
-        for word in words:
-            if word in word_cache:
-                phonemes = word_cache[word]
-            else:
-                phonemes = g2p.inference(word, args.lang)
+    for line in tqdm.tqdm(open(input_path, 'r').readlines(), disable=output=='stdout'):
+        fields = line.strip().split()
 
-            phoneme_lst.extend(phonemes)
-
-        if args.combine:
-            line_output = ' '.join(words)+' '+' '.join(phoneme_lst)
+        utt_id = None
 
+        if file_format == 'text':
+            text = ' '.join(fields)
         else:
-            line_output = ' '.join(phoneme_lst)
+            text = ' '.join(fields[1:])
+            utt_id = fields[0]
+
+        phonemes = model.inference_word_batch(text, lang_id=lang, num_lang=ensemble, force_approximate=force_approximate)
+
+        line_output = ' '.join(phonemes)
+
+        if combine:
+            line_output = text + '\t' + line_output
+
+        if utt_id is not None:
+            line_output = utt_id + ' ' + line_output
 
         if output_fd:
-            output_fd.write(line_output+'\n')
+            output_fd.write(line_output + '\n')
         else:
             print(line_output)
 
-
     if output_fd:
-        output_fd.close()
+        output_fd.close()
+
+
+
+if __name__ == '__main__':
+
+    parser = argparse.ArgumentParser('running transphone g2p model')
+    parser.add_argument('-m', '--model', type=str, default='latest',
+                        help='specify which model to use. default is to use the latest local model')
+    parser.add_argument('-l', '--lang', type=str, default='eng',
+                        help='specify which language inventory to use for recognition. default is to use all phone inventory')
+    parser.add_argument('-i', '--input', type=str, required=True, help='specify your input wav file/directory')
+    parser.add_argument('-o', '--output', type=str, default='stdout',
+                        help='specify output file. the default will be stdout')
+    parser.add_argument('-f', '--format', type=str, default='text', help='kaldi or text')
+    parser.add_argument('-c', '--combine', type=bool, default=False,
+                        help='write outputs by including both grapheme inputs and phonemes in the same line, delimited by space')
+
+    args = parser.parse_args()
+
+    # resolve model's name
+    model_name = resolve_model_name(args.model)
+
+    # format
+    file_format = args.format
+
+    if args.combine:
+        assert file_format == 'text'
+
+    run_g2p(model_name, args.lang, args.input, args.output, file_format, args.combine)
```

### Comparing `transphone-1.3.9/transphone/tokenizer.py` & `transphone-1.4.0/transphone/tokenizer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from phonepiece.iso import normalize_lang_id
+from phonepiece.lang import normalize_lang_id
 from phonepiece.lexicon import read_lexicon
 from transphone.lang.base_tokenizer import BaseTokenizer
 from transphone.lang.eng.tokenizer import ENGTokenizer
 from transphone.lang.cmn.tokenizer import CMNTokenizer
 from transphone.lang.jpn.tokenizer import JPNTokenizer
 from transphone.lang.g2p_tokenizer import G2PTokenizer
 from transphone.lang.epitran_tokenizer import read_raw_epitran_tokenizer, read_customized_epitran_tokenizer
@@ -110,25 +110,25 @@
      'zul': 'zul-Latn',
      'gan': 'gan-Latn',
      'sqi': 'sqi-Latn',
      'lij': 'lij-Latn'
 }
 
 
-def read_tokenizer(lang_id, g2p_model='latest', device=None, use_lexicon=True):
+def read_tokenizer(lang_id, g2p_model='latest', device=None, use_lexicon=True, use_epitran=True):
 
     lang_id = normalize_lang_id(lang_id)
 
     if lang_id == 'eng':
         tokenizer = ENGTokenizer(lang_id, g2p_model, device)
     elif lang_id == 'cmn':
         tokenizer = CMNTokenizer(lang_id, g2p_model, device)
     elif lang_id == 'jpn':
         tokenizer = JPNTokenizer(lang_id, g2p_model, device)
-    elif lang_id in customized_epitran_dict:
+    elif lang_id in customized_epitran_dict and use_epitran:
         tokenizer = read_customized_epitran_tokenizer(customized_epitran_dict[lang_id], use_lexicon=use_lexicon)
-    elif lang_id in raw_epitran_dict:
+    elif lang_id in raw_epitran_dict and use_epitran:
         tokenizer = read_raw_epitran_tokenizer(raw_epitran_dict[lang_id], use_lexicon=use_lexicon)
     else:
         tokenizer = G2PTokenizer(lang_id, g2p_model, device)
 
     return tokenizer
```

### Comparing `transphone-1.3.9/transphone.egg-info/SOURCES.txt` & `transphone-1.4.0/transphone.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -11,20 +11,22 @@
 transphone.egg-info/PKG-INFO
 transphone.egg-info/SOURCES.txt
 transphone.egg-info/dependency_links.txt
 transphone.egg-info/requires.txt
 transphone.egg-info/top_level.txt
 transphone/bin/__init__.py
 transphone/bin/download_model.py
+transphone/bin/eval_epitran.py
+transphone/bin/eval_g2p.py
+transphone/bin/eval_zsl_g2p.py
+transphone/bin/g2p.py
+transphone/bin/tokenize.py
+transphone/bin/train_g2p.py
+transphone/bin/update_model.py
 transphone/data/__init__.py
-transphone/data/dataset.py
-transphone/data/grapheme.py
-transphone/data/loader.py
-transphone/data/utils.py
-transphone/data/vocab.py
 transphone/lang/__init__.py
 transphone/lang/base_tokenizer.py
 transphone/lang/epitran_tokenizer.py
 transphone/lang/g2p_tokenizer.py
 transphone/lang/cmn/__init__.py
 transphone/lang/cmn/normalizer.py
 transphone/lang/cmn/tokenizer.py
@@ -35,12 +37,16 @@
 transphone/lang/jpn/conv_table.py
 transphone/lang/jpn/jaconv.py
 transphone/lang/jpn/kana2phoneme.py
 transphone/lang/jpn/normalizer.py
 transphone/lang/jpn/tokenizer.py
 transphone/model/__init__.py
 transphone/model/checkpoint_utils.py
+transphone/model/dataset.py
 transphone/model/ensemble.py
+transphone/model/grapheme.py
+transphone/model/loader.py
 transphone/model/lstm.py
 transphone/model/transformer.py
 transphone/model/utils.py
+transphone/model/vocab.py
 transphone/pretrained/__init__.py
```

