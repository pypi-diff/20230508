# Comparing `tmp/cherche-1.0.1.tar.gz` & `tmp/cherche-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cherche-1.0.1.tar", last modified: Thu Oct 27 10:44:36 2022, max compression
+gzip compressed data, was "cherche-2.0.0.tar", last modified: Mon May  8 16:19:38 2023, max compression
```

## Comparing `cherche-1.0.1.tar` & `cherche-2.0.0.tar`

### file list

```diff
@@ -1,93 +1,70 @@
-drwxr-xr-x   0 raphaelsourty   (501) staff       (20)        0 2022-10-27 10:44:36.995318 cherche-1.0.1/
--rw-r--r--   0 raphaelsourty   (501) staff       (20)     1071 2022-10-16 14:01:11.000000 cherche-1.0.1/LICENSE
--rw-r--r--   0 raphaelsourty   (501) staff       (20)     9440 2022-10-27 10:44:36.995415 cherche-1.0.1/PKG-INFO
--rw-r--r--   0 raphaelsourty   (501) staff       (20)     8749 2022-10-26 23:15:27.000000 cherche-1.0.1/README.md
-drwxr-xr-x   0 raphaelsourty   (501) staff       (20)        0 2022-10-27 10:44:36.949766 cherche-1.0.1/cherche/
--rw-r--r--   0 raphaelsourty   (501) staff       (20)      208 2022-10-26 22:59:46.000000 cherche-1.0.1/cherche/__init__.py
--rw-r--r--   0 raphaelsourty   (501) staff       (20)       63 2022-10-27 10:40:50.000000 cherche-1.0.1/cherche/__version__.py
-drwxr-xr-x   0 raphaelsourty   (501) staff       (20)        0 2022-10-27 10:44:36.951727 cherche-1.0.1/cherche/compose/
--rw-r--r--   0 raphaelsourty   (501) staff       (20)      144 2022-10-16 14:01:11.000000 cherche-1.0.1/cherche/compose/__init__.py
--rw-r--r--   0 raphaelsourty   (501) staff       (20)     1792 2022-10-26 22:59:46.000000 cherche-1.0.1/cherche/compose/base.py
--rw-r--r--   0 raphaelsourty   (501) staff       (20)    23086 2022-10-26 22:59:46.000000 cherche-1.0.1/cherche/compose/pipeline.py
--rw-r--r--   0 raphaelsourty   (501) staff       (20)     5035 2022-10-26 22:59:46.000000 cherche-1.0.1/cherche/compose/test_compose.py
--rw-r--r--   0 raphaelsourty   (501) staff       (20)     7201 2022-10-26 22:59:46.000000 cherche-1.0.1/cherche/compose/test_union_inter.py
--rw-r--r--   0 raphaelsourty   (501) staff       (20)     2052 2022-10-26 22:59:46.000000 cherche-1.0.1/cherche/compose/test_vote.py
--rw-r--r--   0 raphaelsourty   (501) staff       (20)    11380 2022-10-26 22:59:46.000000 cherche-1.0.1/cherche/compose/union_inter_vote.py
-drwxr-xr-x   0 raphaelsourty   (501) staff       (20)        0 2022-10-27 10:44:36.962050 cherche-1.0.1/cherche/data/
--rw-r--r--   0 raphaelsourty   (501) staff       (20)      104 2022-10-16 14:01:11.000000 cherche-1.0.1/cherche/data/__init__.py
--rw-r--r--   0 raphaelsourty   (501) staff       (20)  6488666 2022-10-16 14:01:11.000000 cherche-1.0.1/cherche/data/norvig.txt
-drwxr-xr-x   0 raphaelsourty   (501) staff       (20)        0 2022-10-27 10:44:36.971974 cherche-1.0.1/cherche/data/semanlink/
--rw-r--r--   0 raphaelsourty   (501) staff       (20)   899186 2022-10-16 14:01:11.000000 cherche-1.0.1/cherche/data/semanlink/arxiv.json
--rw-r--r--   0 raphaelsourty   (501) staff       (20)  8324401 2022-10-16 14:01:11.000000 cherche-1.0.1/cherche/data/semanlink/docs.json
--rw-r--r--   0 raphaelsourty   (501) staff       (20)  4587473 2022-10-16 14:01:11.000000 cherche-1.0.1/cherche/data/semanlink/tags.json
--rw-r--r--   0 raphaelsourty   (501) staff       (20)     3013 2022-10-26 22:59:46.000000 cherche-1.0.1/cherche/data/semanlink.py
--rw-r--r--   0 raphaelsourty   (501) staff       (20)    29097 2022-10-16 14:01:11.000000 cherche-1.0.1/cherche/data/towns.json
--rw-r--r--   0 raphaelsourty   (501) staff       (20)     1577 2022-10-16 14:01:11.000000 cherche-1.0.1/cherche/data/towns.py
-drwxr-xr-x   0 raphaelsourty   (501) staff       (20)        0 2022-10-27 10:44:36.983504 cherche-1.0.1/cherche/eval/
--rw-r--r--   0 raphaelsourty   (501) staff       (20)       43 2022-10-16 14:01:11.000000 cherche-1.0.1/cherche/eval/__init__.py
--rw-r--r--   0 raphaelsourty   (501) staff       (20)     6490 2022-10-26 22:59:46.000000 cherche-1.0.1/cherche/eval/eval.py
-drwxr-xr-x   0 raphaelsourty   (501) staff       (20)        0 2022-10-27 10:44:36.984634 cherche-1.0.1/cherche/generate/
--rw-r--r--   0 raphaelsourty   (501) staff       (20)       40 2022-10-16 14:01:11.000000 cherche-1.0.1/cherche/generate/__init__.py
--rw-r--r--   0 raphaelsourty   (501) staff       (20)     1462 2022-10-16 14:01:11.000000 cherche-1.0.1/cherche/generate/base.py
--rw-r--r--   0 raphaelsourty   (501) staff       (20)     6096 2022-10-26 22:59:46.000000 cherche-1.0.1/cherche/generate/rag.py
-drwxr-xr-x   0 raphaelsourty   (501) staff       (20)        0 2022-10-27 10:44:36.985945 cherche-1.0.1/cherche/index/
--rw-r--r--   0 raphaelsourty   (501) staff       (20)       82 2022-10-26 22:59:46.000000 cherche-1.0.1/cherche/index/__init__.py
--rw-r--r--   0 raphaelsourty   (501) staff       (20)    13748 2022-10-26 22:59:46.000000 cherche-1.0.1/cherche/index/milvus.py
--rw-r--r--   0 raphaelsourty   (501) staff       (20)     3939 2022-10-26 22:59:46.000000 cherche-1.0.1/cherche/index/tree.py
-drwxr-xr-x   0 raphaelsourty   (501) staff       (20)        0 2022-10-27 10:44:36.988263 cherche-1.0.1/cherche/onnx/
--rw-r--r--   0 raphaelsourty   (501) staff       (20)      143 2022-10-16 14:22:16.000000 cherche-1.0.1/cherche/onnx/__init__.py
--rw-r--r--   0 raphaelsourty   (501) staff       (20)      404 2022-10-16 14:22:16.000000 cherche-1.0.1/cherche/onnx/base.py
--rw-r--r--   0 raphaelsourty   (501) staff       (20)     6365 2022-10-26 22:59:46.000000 cherche-1.0.1/cherche/onnx/qa.py
--rw-r--r--   0 raphaelsourty   (501) staff       (20)     7791 2022-10-26 22:59:46.000000 cherche-1.0.1/cherche/onnx/sentence_transformers.py
-drwxr-xr-x   0 raphaelsourty   (501) staff       (20)        0 2022-10-27 10:44:36.988589 cherche-1.0.1/cherche/qa/
--rw-r--r--   0 raphaelsourty   (501) staff       (20)       37 2022-10-16 14:01:11.000000 cherche-1.0.1/cherche/qa/__init__.py
--rw-r--r--   0 raphaelsourty   (501) staff       (20)     4178 2022-10-26 22:59:46.000000 cherche-1.0.1/cherche/qa/qa.py
-drwxr-xr-x   0 raphaelsourty   (501) staff       (20)        0 2022-10-27 10:44:36.990727 cherche-1.0.1/cherche/query/
--rw-r--r--   0 raphaelsourty   (501) staff       (20)      110 2022-10-16 14:01:11.000000 cherche-1.0.1/cherche/query/__init__.py
--rw-r--r--   0 raphaelsourty   (501) staff       (20)     1077 2022-10-16 14:01:11.000000 cherche-1.0.1/cherche/query/base.py
--rw-r--r--   0 raphaelsourty   (501) staff       (20)     4582 2022-10-26 22:59:46.000000 cherche-1.0.1/cherche/query/norvig.py
--rw-r--r--   0 raphaelsourty   (501) staff       (20)     4488 2022-10-26 22:59:46.000000 cherche-1.0.1/cherche/query/prf.py
-drwxr-xr-x   0 raphaelsourty   (501) staff       (20)        0 2022-10-27 10:44:36.991702 cherche-1.0.1/cherche/rank/
--rw-r--r--   0 raphaelsourty   (501) staff       (20)      205 2022-10-26 22:59:46.000000 cherche-1.0.1/cherche/rank/__init__.py
--rw-r--r--   0 raphaelsourty   (501) staff       (20)     6553 2022-10-26 22:59:46.000000 cherche-1.0.1/cherche/rank/base.py
--rw-r--r--   0 raphaelsourty   (501) staff       (20)     3741 2022-10-26 22:59:46.000000 cherche-1.0.1/cherche/rank/dpr.py
--rw-r--r--   0 raphaelsourty   (501) staff       (20)     3685 2022-10-26 22:59:46.000000 cherche-1.0.1/cherche/rank/encoder.py
--rw-r--r--   0 raphaelsourty   (501) staff       (20)     7223 2022-10-26 22:59:46.000000 cherche-1.0.1/cherche/rank/recommend.py
--rw-r--r--   0 raphaelsourty   (501) staff       (20)     3204 2022-10-26 22:59:46.000000 cherche-1.0.1/cherche/rank/test_rank.py
--rw-r--r--   0 raphaelsourty   (501) staff       (20)     4734 2022-10-26 22:59:46.000000 cherche-1.0.1/cherche/rank/zero_shot.py
-drwxr-xr-x   0 raphaelsourty   (501) staff       (20)        0 2022-10-27 10:44:36.993792 cherche-1.0.1/cherche/retrieve/
--rw-r--r--   0 raphaelsourty   (501) staff       (20)      545 2022-10-26 22:59:46.000000 cherche-1.0.1/cherche/retrieve/__init__.py
--rw-r--r--   0 raphaelsourty   (501) staff       (20)     2238 2022-10-26 22:59:46.000000 cherche-1.0.1/cherche/retrieve/base.py
--rw-r--r--   0 raphaelsourty   (501) staff       (20)     8945 2022-10-26 22:59:46.000000 cherche-1.0.1/cherche/retrieve/bm25.py
--rw-r--r--   0 raphaelsourty   (501) staff       (20)     3925 2022-10-26 22:59:46.000000 cherche-1.0.1/cherche/retrieve/dpr.py
--rw-r--r--   0 raphaelsourty   (501) staff       (20)     4300 2022-10-26 22:59:46.000000 cherche-1.0.1/cherche/retrieve/elastic.py
--rw-r--r--   0 raphaelsourty   (501) staff       (20)     3577 2022-10-26 22:59:46.000000 cherche-1.0.1/cherche/retrieve/encoder.py
--rw-r--r--   0 raphaelsourty   (501) staff       (20)     4188 2022-10-26 22:59:46.000000 cherche-1.0.1/cherche/retrieve/flash.py
--rw-r--r--   0 raphaelsourty   (501) staff       (20)     5446 2022-10-26 22:59:46.000000 cherche-1.0.1/cherche/retrieve/fuzz.py
--rw-r--r--   0 raphaelsourty   (501) staff       (20)     3065 2022-10-26 22:59:46.000000 cherche-1.0.1/cherche/retrieve/lunr.py
--rw-r--r--   0 raphaelsourty   (501) staff       (20)     3982 2022-10-26 22:59:46.000000 cherche-1.0.1/cherche/retrieve/meilisearch.py
--rw-r--r--   0 raphaelsourty   (501) staff       (20)     6930 2022-10-26 22:59:46.000000 cherche-1.0.1/cherche/retrieve/recommend.py
--rw-r--r--   0 raphaelsourty   (501) staff       (20)     6052 2022-10-26 22:59:46.000000 cherche-1.0.1/cherche/retrieve/test_retrieve.py
--rw-r--r--   0 raphaelsourty   (501) staff       (20)     3860 2022-10-26 22:59:46.000000 cherche-1.0.1/cherche/retrieve/tfidf.py
--rw-r--r--   0 raphaelsourty   (501) staff       (20)     3542 2022-10-26 22:59:46.000000 cherche-1.0.1/cherche/retrieve/tpsense.py
-drwxr-xr-x   0 raphaelsourty   (501) staff       (20)        0 2022-10-27 10:44:36.994124 cherche-1.0.1/cherche/similarity/
--rw-r--r--   0 raphaelsourty   (501) staff       (20)       65 2022-10-16 14:01:11.000000 cherche-1.0.1/cherche/similarity/__init__.py
--rw-r--r--   0 raphaelsourty   (501) staff       (20)     2062 2022-10-26 22:59:46.000000 cherche-1.0.1/cherche/similarity/similarity.py
-drwxr-xr-x   0 raphaelsourty   (501) staff       (20)        0 2022-10-27 10:44:36.994484 cherche-1.0.1/cherche/summary/
--rw-r--r--   0 raphaelsourty   (501) staff       (20)       52 2022-10-16 14:01:11.000000 cherche-1.0.1/cherche/summary/__init__.py
--rw-r--r--   0 raphaelsourty   (501) staff       (20)     3644 2022-10-26 22:59:46.000000 cherche-1.0.1/cherche/summary/summary.py
-drwxr-xr-x   0 raphaelsourty   (501) staff       (20)        0 2022-10-27 10:44:36.994742 cherche-1.0.1/cherche/translate/
--rw-r--r--   0 raphaelsourty   (501) staff       (20)       92 2022-10-16 14:01:11.000000 cherche-1.0.1/cherche/translate/__init__.py
--rw-r--r--   0 raphaelsourty   (501) staff       (20)     6022 2022-10-26 22:59:46.000000 cherche-1.0.1/cherche/translate/translate.py
-drwxr-xr-x   0 raphaelsourty   (501) staff       (20)        0 2022-10-27 10:44:36.995200 cherche-1.0.1/cherche/utils/
--rw-r--r--   0 raphaelsourty   (501) staff       (20)      119 2022-10-26 22:59:46.000000 cherche-1.0.1/cherche/utils/__init__.py
--rw-r--r--   0 raphaelsourty   (501) staff       (20)     1643 2022-10-16 14:22:16.000000 cherche-1.0.1/cherche/utils/quantize.py
--rw-r--r--   0 raphaelsourty   (501) staff       (20)     1324 2022-10-26 22:59:46.000000 cherche-1.0.1/cherche/utils/recommend.py
-drwxr-xr-x   0 raphaelsourty   (501) staff       (20)        0 2022-10-27 10:44:36.950477 cherche-1.0.1/cherche.egg-info/
--rw-r--r--   0 raphaelsourty   (501) staff       (20)     9440 2022-10-27 10:44:36.000000 cherche-1.0.1/cherche.egg-info/PKG-INFO
--rw-r--r--   0 raphaelsourty   (501) staff       (20)     1911 2022-10-27 10:44:36.000000 cherche-1.0.1/cherche.egg-info/SOURCES.txt
--rw-r--r--   0 raphaelsourty   (501) staff       (20)        1 2022-10-27 10:44:36.000000 cherche-1.0.1/cherche.egg-info/dependency_links.txt
--rw-r--r--   0 raphaelsourty   (501) staff       (20)     2048 2022-10-27 10:44:36.000000 cherche-1.0.1/cherche.egg-info/requires.txt
--rw-r--r--   0 raphaelsourty   (501) staff       (20)        8 2022-10-27 10:44:36.000000 cherche-1.0.1/cherche.egg-info/top_level.txt
--rw-r--r--   0 raphaelsourty   (501) staff       (20)       79 2022-10-27 10:44:36.995695 cherche-1.0.1/setup.cfg
--rw-r--r--   0 raphaelsourty   (501) staff       (20)     2086 2022-10-27 10:38:47.000000 cherche-1.0.1/setup.py
+drwxr-xr-x   0 raphaelsourty   (501) staff       (20)        0 2023-05-08 16:19:38.172320 cherche-2.0.0/
+-rw-r--r--   0 raphaelsourty   (501) staff       (20)     1071 2023-01-07 22:47:32.000000 cherche-2.0.0/LICENSE
+-rw-r--r--   0 raphaelsourty   (501) staff       (20)     8363 2023-05-08 16:19:38.172445 cherche-2.0.0/PKG-INFO
+-rw-r--r--   0 raphaelsourty   (501) staff       (20)     7726 2023-05-08 16:13:17.000000 cherche-2.0.0/README.md
+drwxr-xr-x   0 raphaelsourty   (501) staff       (20)        0 2023-05-08 16:19:38.140000 cherche-2.0.0/cherche/
+-rw-r--r--   0 raphaelsourty   (501) staff       (20)      134 2023-05-06 16:03:36.000000 cherche-2.0.0/cherche/__init__.py
+-rw-r--r--   0 raphaelsourty   (501) staff       (20)       63 2023-05-08 16:13:17.000000 cherche-2.0.0/cherche/__version__.py
+drwxr-xr-x   0 raphaelsourty   (501) staff       (20)        0 2023-05-08 16:19:38.142793 cherche-2.0.0/cherche/compose/
+-rw-r--r--   0 raphaelsourty   (501) staff       (20)      151 2023-05-01 21:17:44.000000 cherche-2.0.0/cherche/compose/__init__.py
+-rw-r--r--   0 raphaelsourty   (501) staff       (20)     6368 2023-05-07 23:19:39.000000 cherche-2.0.0/cherche/compose/base.py
+-rw-r--r--   0 raphaelsourty   (501) staff       (20)     8798 2023-05-07 17:58:57.000000 cherche-2.0.0/cherche/compose/intersection_union_vote.py
+-rw-r--r--   0 raphaelsourty   (501) staff       (20)    18160 2023-05-07 17:57:07.000000 cherche-2.0.0/cherche/compose/pipeline.py
+-rw-r--r--   0 raphaelsourty   (501) staff       (20)     4608 2023-05-02 22:18:05.000000 cherche-2.0.0/cherche/compose/test_compose.py
+-rw-r--r--   0 raphaelsourty   (501) staff       (20)     6904 2023-05-02 22:22:08.000000 cherche-2.0.0/cherche/compose/test_union_inter.py
+-rw-r--r--   0 raphaelsourty   (501) staff       (20)     1980 2023-05-02 22:24:13.000000 cherche-2.0.0/cherche/compose/test_vote.py
+drwxr-xr-x   0 raphaelsourty   (501) staff       (20)        0 2023-05-08 16:19:38.143996 cherche-2.0.0/cherche/data/
+-rw-r--r--   0 raphaelsourty   (501) staff       (20)      104 2023-04-30 19:26:48.000000 cherche-2.0.0/cherche/data/__init__.py
+drwxr-xr-x   0 raphaelsourty   (501) staff       (20)        0 2023-05-08 16:19:38.152688 cherche-2.0.0/cherche/data/semanlink/
+-rw-r--r--   0 raphaelsourty   (501) staff       (20)   899186 2023-01-07 22:47:32.000000 cherche-2.0.0/cherche/data/semanlink/arxiv.json
+-rw-r--r--   0 raphaelsourty   (501) staff       (20)  8324401 2023-01-07 22:47:32.000000 cherche-2.0.0/cherche/data/semanlink/docs.json
+-rw-r--r--   0 raphaelsourty   (501) staff       (20)  4587473 2023-01-07 22:47:32.000000 cherche-2.0.0/cherche/data/semanlink/tags.json
+-rw-r--r--   0 raphaelsourty   (501) staff       (20)     3013 2023-01-07 22:47:32.000000 cherche-2.0.0/cherche/data/semanlink.py
+-rw-r--r--   0 raphaelsourty   (501) staff       (20)    29097 2023-01-07 22:47:32.000000 cherche-2.0.0/cherche/data/towns.json
+-rw-r--r--   0 raphaelsourty   (501) staff       (20)     1577 2023-01-07 22:47:32.000000 cherche-2.0.0/cherche/data/towns.py
+drwxr-xr-x   0 raphaelsourty   (501) staff       (20)        0 2023-05-08 16:19:38.161212 cherche-2.0.0/cherche/evaluate/
+-rw-r--r--   0 raphaelsourty   (501) staff       (20)       59 2023-05-08 15:34:32.000000 cherche-2.0.0/cherche/evaluate/__init__.py
+-rw-r--r--   0 raphaelsourty   (501) staff       (20)     4141 2023-05-08 15:34:21.000000 cherche-2.0.0/cherche/evaluate/evaluate.py
+drwxr-xr-x   0 raphaelsourty   (501) staff       (20)        0 2023-05-08 16:19:38.163622 cherche-2.0.0/cherche/index/
+-rw-r--r--   0 raphaelsourty   (501) staff       (20)       52 2023-04-30 13:03:44.000000 cherche-2.0.0/cherche/index/__init__.py
+-rw-r--r--   0 raphaelsourty   (501) staff       (20)     5056 2023-05-06 22:32:07.000000 cherche-2.0.0/cherche/index/faiss_index.py
+drwxr-xr-x   0 raphaelsourty   (501) staff       (20)        0 2023-05-08 16:19:38.164490 cherche-2.0.0/cherche/qa/
+-rw-r--r--   0 raphaelsourty   (501) staff       (20)       37 2023-01-07 22:47:32.000000 cherche-2.0.0/cherche/qa/__init__.py
+-rw-r--r--   0 raphaelsourty   (501) staff       (20)     6442 2023-05-07 14:50:43.000000 cherche-2.0.0/cherche/qa/qa.py
+drwxr-xr-x   0 raphaelsourty   (501) staff       (20)        0 2023-05-08 16:19:38.165498 cherche-2.0.0/cherche/query/
+-rw-r--r--   0 raphaelsourty   (501) staff       (20)      110 2023-01-07 22:47:32.000000 cherche-2.0.0/cherche/query/__init__.py
+-rw-r--r--   0 raphaelsourty   (501) staff       (20)     1153 2023-05-06 21:29:37.000000 cherche-2.0.0/cherche/query/base.py
+-rw-r--r--   0 raphaelsourty   (501) staff       (20)     4455 2023-05-06 22:43:31.000000 cherche-2.0.0/cherche/query/norvig.py
+-rw-r--r--   0 raphaelsourty   (501) staff       (20)     5074 2023-05-06 22:43:33.000000 cherche-2.0.0/cherche/query/prf.py
+drwxr-xr-x   0 raphaelsourty   (501) staff       (20)        0 2023-05-08 16:19:38.167411 cherche-2.0.0/cherche/rank/
+-rw-r--r--   0 raphaelsourty   (501) staff       (20)      217 2023-05-02 22:07:38.000000 cherche-2.0.0/cherche/rank/__init__.py
+-rw-r--r--   0 raphaelsourty   (501) staff       (20)    10310 2023-05-08 16:13:17.000000 cherche-2.0.0/cherche/rank/base.py
+-rw-r--r--   0 raphaelsourty   (501) staff       (20)     6692 2023-05-07 21:46:45.000000 cherche-2.0.0/cherche/rank/cross_encoder.py
+-rw-r--r--   0 raphaelsourty   (501) staff       (20)     4155 2023-05-08 16:13:17.000000 cherche-2.0.0/cherche/rank/dpr.py
+-rw-r--r--   0 raphaelsourty   (501) staff       (20)     4767 2023-05-07 14:33:29.000000 cherche-2.0.0/cherche/rank/embedding.py
+-rw-r--r--   0 raphaelsourty   (501) staff       (20)     3805 2023-05-08 16:13:17.000000 cherche-2.0.0/cherche/rank/encoder.py
+-rw-r--r--   0 raphaelsourty   (501) staff       (20)     3867 2023-05-06 13:01:19.000000 cherche-2.0.0/cherche/rank/test_rank.py
+drwxr-xr-x   0 raphaelsourty   (501) staff       (20)        0 2023-05-08 16:19:38.170548 cherche-2.0.0/cherche/retrieve/
+-rw-r--r--   0 raphaelsourty   (501) staff       (20)      332 2023-04-30 19:33:52.000000 cherche-2.0.0/cherche/retrieve/__init__.py
+-rw-r--r--   0 raphaelsourty   (501) staff       (20)     2438 2023-05-07 14:03:51.000000 cherche-2.0.0/cherche/retrieve/base.py
+-rw-r--r--   0 raphaelsourty   (501) staff       (20)     4513 2023-05-08 16:13:17.000000 cherche-2.0.0/cherche/retrieve/dpr.py
+-rw-r--r--   0 raphaelsourty   (501) staff       (20)     4597 2023-05-08 12:44:27.000000 cherche-2.0.0/cherche/retrieve/embedding.py
+-rw-r--r--   0 raphaelsourty   (501) staff       (20)     4371 2023-05-08 16:13:17.000000 cherche-2.0.0/cherche/retrieve/encoder.py
+-rw-r--r--   0 raphaelsourty   (501) staff       (20)     4750 2023-05-07 14:04:15.000000 cherche-2.0.0/cherche/retrieve/flash.py
+-rw-r--r--   0 raphaelsourty   (501) staff       (20)     4951 2023-05-07 14:04:03.000000 cherche-2.0.0/cherche/retrieve/fuzz.py
+-rw-r--r--   0 raphaelsourty   (501) staff       (20)     3380 2023-05-07 14:03:59.000000 cherche-2.0.0/cherche/retrieve/lunr.py
+-rw-r--r--   0 raphaelsourty   (501) staff       (20)     4139 2023-05-06 21:28:01.000000 cherche-2.0.0/cherche/retrieve/test_retrieve.py
+-rw-r--r--   0 raphaelsourty   (501) staff       (20)     5742 2023-05-08 16:13:17.000000 cherche-2.0.0/cherche/retrieve/tfidf.py
+drwxr-xr-x   0 raphaelsourty   (501) staff       (20)        0 2023-05-08 16:19:38.172075 cherche-2.0.0/cherche/utils/
+-rw-r--r--   0 raphaelsourty   (501) staff       (20)      174 2023-05-07 22:35:18.000000 cherche-2.0.0/cherche/utils/__init__.py
+-rw-r--r--   0 raphaelsourty   (501) staff       (20)     1180 2023-05-07 22:35:03.000000 cherche-2.0.0/cherche/utils/batch.py
+-rw-r--r--   0 raphaelsourty   (501) staff       (20)     1754 2023-05-01 20:27:11.000000 cherche-2.0.0/cherche/utils/quantize.py
+-rw-r--r--   0 raphaelsourty   (501) staff       (20)     1983 2023-05-06 22:14:34.000000 cherche-2.0.0/cherche/utils/topk.py
+drwxr-xr-x   0 raphaelsourty   (501) staff       (20)        0 2023-05-08 16:19:38.140852 cherche-2.0.0/cherche.egg-info/
+-rw-r--r--   0 raphaelsourty   (501) staff       (20)     8363 2023-05-08 16:19:38.000000 cherche-2.0.0/cherche.egg-info/PKG-INFO
+-rw-r--r--   0 raphaelsourty   (501) staff       (20)     1437 2023-05-08 16:19:38.000000 cherche-2.0.0/cherche.egg-info/SOURCES.txt
+-rw-r--r--   0 raphaelsourty   (501) staff       (20)        1 2023-05-08 16:19:38.000000 cherche-2.0.0/cherche.egg-info/dependency_links.txt
+-rw-r--r--   0 raphaelsourty   (501) staff       (20)      736 2023-05-08 16:19:38.000000 cherche-2.0.0/cherche.egg-info/requires.txt
+-rw-r--r--   0 raphaelsourty   (501) staff       (20)        8 2023-05-08 16:19:38.000000 cherche-2.0.0/cherche.egg-info/top_level.txt
+-rw-r--r--   0 raphaelsourty   (501) staff       (20)       79 2023-05-08 16:19:38.172747 cherche-2.0.0/setup.cfg
+-rw-r--r--   0 raphaelsourty   (501) staff       (20)     1745 2023-05-08 16:13:17.000000 cherche-2.0.0/setup.py
```

### Comparing `cherche-1.0.1/LICENSE` & `cherche-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cherche-1.0.1/PKG-INFO` & `cherche-2.0.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,69 +1,80 @@
 Metadata-Version: 2.1
 Name: cherche
-Version: 1.0.1
+Version: 2.0.0
 Summary: Neural Search
 Home-page: https://github.com/raphaelsty/cherche
 Download-URL: https://github.com/user/cherche/archive/v_01.tar.gz
 Author: Raphael Sourty
 Author-email: raphael.sourty@gmail.com
 License: MIT
-Keywords: neural,search,question,answering,summarization,collaborative filtering
+Keywords: neural search,information retrieval,question answering,semantic search
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Provides-Extra: recommend
-Provides-Extra: onnx
-Provides-Extra: onnxgpu
-Provides-Extra: doc
-Provides-Extra: milvus
+Provides-Extra: cpu
+Provides-Extra: gpu
+Provides-Extra: dev
 License-File: LICENSE
 
 <div align="center">
   <h1>Cherche</h1>
   <p>Neural search</p>
 </div>
-<br>
+
+<p align="center"><img width=300 src="docs/img/logo.png"/></p>
 
 <div align="center">
   <!-- Documentation -->
   <a href="https://raphaelsty.github.io/cherche/"><img src="https://img.shields.io/website?label=docs&style=flat-square&url=https%3A%2F%2Fraphaelsty.github.io/cherche/%2F" alt="documentation"></a>
   <!-- Demo -->
-  <a href="https://huggingface.co/spaces/raphaelsty/games"><img src="https://img.shields.io/badge/demo-running-blueviolet?style=flat-square" alt="Demo"></a>
+  <a href="https://raphaelsty.github.io/knowledge/?query=cherche%20neural%20search"><img src="https://img.shields.io/badge/demo-running-blueviolet?style=flat-square" alt="Demo"></a>
   <!-- License -->
   <a href="https://opensource.org/licenses/MIT"><img src="https://img.shields.io/badge/License-MIT-blue.svg?style=flat-square" alt="license"></a>
 </div>
-<br>
 
-Cherche allows the creation of efficient neural search pipelines using retrievers and pre-trained language models as rankers. Cherche's main strength is its ability to build diverse and end-to-end pipelines from lexical matching, semantic matching, and collaborative filtering-based models.
+
+Cherche enables the development of a neural search pipeline that employs retrievers and pre-trained language models both as retrievers and rankers. The primary advantage of Cherche lies in its capacity to construct end-to-end pipelines. Additionally, Cherche is well-suited for offline semantic search due to its compatibility with batch computation.
+
+[Live demo of a NLP search engine powered by Cherche](https://raphaelsty.github.io/knowledge/?query=cherche%20neural%20search)
 
 ![Alt text](docs/img/explain.png)
 
 ## Installation 🤖
 
+To install Cherche for use with a simple retriever on CPU, such as TfIdf, Flash, Lunr, Fuzz, use the following command:
+
+```sh
+pip install cherche
+```
+
+To install Cherche for use with any semantic retriever or ranker on CPU, use the following command:
+
 ```sh
-pip install cherche --upgrade
+pip install "cherche[cpu]"
 ```
 
-To install the development version:
+Finally, if you plan to use any semantic retriever or ranker on GPU, use the following command:
 
 ```sh
-pip install git+https://github.com/raphaelsty/cherche
+pip install "cherche[gpu]"
 ```
 
-## [Documentation](https://raphaelsty.github.io/cherche/) 📜
+By following these installation instructions, you will be able to use Cherche with the appropriate requirements for your needs.
+
+### Documentation
 
 Documentation is available [here](https://raphaelsty.github.io/cherche/). It provides details
-about retrievers, rankers, pipelines, question answering, summarization, and examples.
+about retrievers, rankers, pipelines and examples.
 
-## QuickStart 💨
+## QuickStart 📑
 
-### Documents 📑
+### Documents
 
 Cherche allows findings the right document within a list of objects. Here is an example of a corpus.
 
 ```python
 from cherche import data
 
 documents = data.load_towns()
@@ -80,17 +91,17 @@
  {'id': 2,
   'title': 'Paris',
   'url': 'https://en.wikipedia.org/wiki/Paris',
   'article': 'The City of Paris is the centre and seat of government of the region and province of Île-de-France.'
   }]
 ```
 
-### Retriever ranker 🔍
+### Retriever ranker
 
-Here is an example of a neural search pipeline composed of a TF-IDF that quickly retrieves documents, followed by a ranking model. The ranking model sorts the documents produced by the retriever based on the semantic similarity between the query and the documents.
+Here is an example of a neural search pipeline composed of a TF-IDF that quickly retrieves documents, followed by a ranking model. The ranking model sorts the documents produced by the retriever based on the semantic similarity between the query and the documents. We can call the pipeline using a list of queries and get relevant documents for each query.
 
 ```python
 from cherche import data, retrieve, rank
 from sentence_transformers import SentenceTransformer
 
 # List of dicts
 documents = data.load_towns()
@@ -107,108 +118,106 @@
 )
 
 # Pipeline creation
 search = retriever + ranker
 
 search.add(documents=documents)
 
-search("Bordeaux")
-[{'id': 57, 'similarity': 0.69513476},
- {'id': 63, 'similarity': 0.6214991},
- {'id': 65, 'similarity': 0.61809057}]
+# Search documents for 3 queries.
+search(["Bordeaux", "Paris", "Toulouse"])
+[[{'id': 57, 'similarity': 0.69513524},
+  {'id': 63, 'similarity': 0.6214994},
+  {'id': 65, 'similarity': 0.61809087}],
+ [{'id': 16, 'similarity': 0.59158516},
+  {'id': 0, 'similarity': 0.58217555},
+  {'id': 1, 'similarity': 0.57944715}],
+ [{'id': 26, 'similarity': 0.6925601},
+  {'id': 37, 'similarity': 0.63977146},
+  {'id': 28, 'similarity': 0.62772334}]]
 ```
 
-Map the index to the documents to access their contents.
+We can map the index to the documents to access their contents using pipelines:
 
 ```python
 search += documents
-search("Bordeaux")
-[{'id': 57,
-  'title': 'Bordeaux',
-  'url': 'https://en.wikipedia.org/wiki/Bordeaux',
-  'article': 'Bordeaux ( bor-DOH, French: [bɔʁdo] (listen); Gascon Occitan: Bordèu [buɾˈðɛw]) is a port city on the river Garonne in the Gironde department, Southwestern France.',
-  'similarity': 0.69513476},
- {'id': 63,
-  'title': 'Bordeaux',
-  'url': 'https://en.wikipedia.org/wiki/Bordeaux',
-  'article': 'The term "Bordelais" may also refer to the city and its surrounding region.',
-  'similarity': 0.6214991},
- {'id': 65,
-  'title': 'Bordeaux',
-  'url': 'https://en.wikipedia.org/wiki/Bordeaux',
-  'article': "Bordeaux is a world capital of wine, with its castles and vineyards of the Bordeaux region that stand on the hillsides of the Gironde and is home to the world's main wine fair, Vinexpo.",
-  'similarity': 0.61809057}]
+search(["Bordeaux", "Paris", "Toulouse"])
+[[{'id': 57,
+   'title': 'Bordeaux',
+   'url': 'https://en.wikipedia.org/wiki/Bordeaux',
+   'similarity': 0.69513524},
+  {'id': 63,
+   'title': 'Bordeaux',
+   'similarity': 0.6214994},
+  {'id': 65,
+   'title': 'Bordeaux',
+   'url': 'https://en.wikipedia.org/wiki/Bordeaux',
+   'similarity': 0.61809087}],
+ [{'id': 16,
+   'title': 'Paris',
+   'url': 'https://en.wikipedia.org/wiki/Paris',
+   'article': 'Paris received 12.',
+   'similarity': 0.59158516},
+  {'id': 0,
+   'title': 'Paris',
+   'url': 'https://en.wikipedia.org/wiki/Paris',
+   'similarity': 0.58217555},
+  {'id': 1,
+   'title': 'Paris',
+   'url': 'https://en.wikipedia.org/wiki/Paris',
+   'similarity': 0.57944715}],
+ [{'id': 26,
+   'title': 'Toulouse',
+   'url': 'https://en.wikipedia.org/wiki/Toulouse',
+   'similarity': 0.6925601},
+  {'id': 37,
+   'title': 'Toulouse',
+   'url': 'https://en.wikipedia.org/wiki/Toulouse',
+   'similarity': 0.63977146},
+  {'id': 28,
+   'title': 'Toulouse',
+   'url': 'https://en.wikipedia.org/wiki/Toulouse',
+   'similarity': 0.62772334}]]
 ```
 
-## Retrieve 👻
+## Retrieve
 
-Cherche provides different [retrievers](https://raphaelsty.github.io/cherche/retrieve/retrieve/) that filter input documents based on a query.
+Cherche provides [retrievers](https://raphaelsty.github.io/cherche/retrieve/retrieve/) that filter input documents based on a query.
 
-- retrieve.Elastic
 - retrieve.TfIdf
 - retrieve.Lunr
-- retrieve.BM25Okapi
-- retrieve.BM25L
 - retrieve.Flash
 - retrieve.Encoder
 - retrieve.DPR
 - retrieve.Fuzz
-- retrieve.Meilisearch
-- retrieve.TypeSense
-- retrieve.Recommend
-
-## Rank 🤗
+- retrieve.Embedding
 
-Cherche rankers are compatible with [SentenceTransformers](https://www.sbert.net/docs/pretrained_models.html) models, [Hugging Face sentence similarity](https://huggingface.co/models?pipeline_tag=zero-shot-classification&sort=downloads) models, [Hugging Face zero shot classification](https://huggingface.co/models?pipeline_tag=zero-shot-classification&sort=downloads) models, and of course with your own models.
+## Rank
 
-## Summarization and question answering
+Cherche provides [rankers](https://raphaelsty.github.io/cherche/rank/rank/) that filter documents in output of retrievers.
 
-Cherche provides modules dedicated to summarization and question answering. These modules are compatible with Hugging Face's pre-trained models and fully integrated into neural search pipelines.
+Cherche rankers are compatible with [SentenceTransformers](https://www.sbert.net/docs/pretrained_models.html) models which are available on [Hugging Face hub](https://huggingface.co/models?pipeline_tag=zero-shot-classification&sort=downloads).
 
-## Translation
+- rank.Encoder
+- rank.DPR
+- rank.CrossEncoder
+- rank.Embedding
 
-Hugging Face's translation models can be fully integrated into the neural search pipeline to translate queries, documents, or answers.
+## Question answering
 
-## Collaborative filtering
+Cherche provides modules dedicated to question answering. These modules are compatible with Hugging Face's pre-trained models and fully integrated into neural search pipelines.
 
-Search is fully compatible with the collaborative filtering library [Implicit](https://github.com/benfred/implicit). It is advantageous if you have a history associated with users and you want to retrieve / re-rank documents based on user preferences.
-
-|            | **Document 1** | **Document 2** | **Document 3** | **Document 4** |
-|:----------:|:--------------:|:--------------:|:--------------:|:--------------:|
-| **User 1** |        1       |        0       |        0       |        1       |
-| **User 2** |        0       |        1       |        0       |        0       |
-| **User 3** |        0       |        4       |        1       |        0       |
-
-
-## Deploy
-
-We provide a minimalist API to deploy our neural search pipeline with FastAPI and Docker; information is available in the [documentation](https://raphaelsty.github.io/cherche/deployment/deployment/).
-
-## Hugging Face Space
-
-A running demo is available on [Hugging Face](https://huggingface.co/spaces/raphaelsty/games).
 ## Contributors 🤝
 Cherche was created for/by Renault and is now available to all.
 We welcome all contributions.
 
 <p align="center"><img src="docs/img/renault.jpg"/></p>
 
 ## Acknowledgements 👏
 
-The BM25 models available in Cherche are wrappers around [rank_bm25](https://github.com/dorianbrown/rank_bm25). Elastic retriever is a wrapper around [Python Elasticsearch Client](https://elasticsearch-py.readthedocs.io/en/v7.15.2/). TfIdf retriever is a wrapper around [scikit-learn's TfidfVectorizer](https://scikit-learn.org/stable/modules/generated/sklearn.feature_extraction.text.TfidfVectorizer.html). Lunr retriever is a wrapper around [Lunr.py](https://github.com/yeraydiazdiaz/lunr.py). Flash retriever is a wrapper around [FlashText](https://github.com/vi3k6i5/flashtext). DPR and Encode rankers are wrappers dedicated to the use of the pre-trained models of [SentenceTransformers](https://www.sbert.net/docs/pretrained_models.html) in a neural search pipeline. ZeroShot ranker is a wrapper dedicated to the use of the zero-shot sequence classifiers of [Hugging Face](https://huggingface.co/models?pipeline_tag=zero-shot-classification&sort=downloads) in a neural search pipeline.
-
-## See also 👀
-
-Cherche is a minimalist solution and meets a need for modularity. Cherche is the way to go if we start with a list of documents as JSON with multiple fields to search on and create pipelines. Also, Cherche is well suited for middle-sized corpora.
-
-Do not hesitate to look at Jina, Haystack, or TxtAi, which offer advanced neural search solutions.
-
-- [Haystack](https://github.com/deepset-ai/haystack)
-- [Jina](https://github.com/jina-ai/jina)
-- [txtai](https://github.com/neuml/txtai)
+TfIdf retriever is a wrapper around [scikit-learn's TfidfVectorizer](https://scikit-learn.org/stable/modules/generated/sklearn.feature_extraction.text.TfidfVectorizer.html). Lunr retriever is a wrapper around [Lunr.py](https://github.com/yeraydiazdiaz/lunr.py). Flash retriever is a wrapper around [FlashText](https://github.com/vi3k6i5/flashtext). DPR, Encode and CrossEncoder rankers are wrappers dedicated to the use of the pre-trained models of [SentenceTransformers](https://www.sbert.net/docs/pretrained_models.html) in a neural search pipeline.
 
 ## Citations
 
 If you use cherche to produce results for your scientific publication, please refer to our SIGIR paper:
 
 ```
 @inproceedings{Sourty2022sigir,
```

#### html2text {}

```diff
@@ -1,119 +1,103 @@
-Metadata-Version: 2.1 Name: cherche Version: 1.0.1 Summary: Neural Search Home-
+Metadata-Version: 2.1 Name: cherche Version: 2.0.0 Summary: Neural Search Home-
 page: https://github.com/raphaelsty/cherche Download-URL: https://github.com/
 user/cherche/archive/v_01.tar.gz Author: Raphael Sourty Author-email:
-raphael.sourty@gmail.com License: MIT Keywords:
-neural,search,question,answering,summarization,collaborative filtering
-Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
-Approved :: MIT License Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6 Description-Content-Type: text/markdown Provides-Extra:
-recommend Provides-Extra: onnx Provides-Extra: onnxgpu Provides-Extra: doc
-Provides-Extra: milvus License-File: LICENSE
+raphael.sourty@gmail.com License: MIT Keywords: neural search,information
+retrieval,question answering,semantic search Classifier: Programming Language
+:: Python :: 3 Classifier: License :: OSI Approved :: MIT License Classifier:
+Operating System :: OS Independent Requires-Python: >=3.6 Description-Content-
+Type: text/markdown Provides-Extra: cpu Provides-Extra: gpu Provides-Extra: dev
+License-File: LICENSE
                              ****** Cherche ******
                                  Neural search
-
+                              [docs/img/logo.png]
                        [documentation]  [Demo]  [license]
-
-Cherche allows the creation of efficient neural search pipelines using
-retrievers and pre-trained language models as rankers. Cherche's main strength
-is its ability to build diverse and end-to-end pipelines from lexical matching,
-semantic matching, and collaborative filtering-based models. ![Alt text](docs/
-img/explain.png) ## Installation ð¤ ```sh pip install cherche --upgrade ```
-To install the development version: ```sh pip install git+https://github.com/
-raphaelsty/cherche ``` ## [Documentation](https://raphaelsty.github.io/cherche/
-) ð Documentation is available [here](https://raphaelsty.github.io/cherche/
-). It provides details about retrievers, rankers, pipelines, question
-answering, summarization, and examples. ## QuickStart ð¨ ### Documents ð
-Cherche allows findings the right document within a list of objects. Here is an
-example of a corpus. ```python from cherche import data documents =
-data.load_towns() documents[:3] [{'id': 0, 'title': 'Paris', 'url': 'https://
-en.wikipedia.org/wiki/Paris', 'article': 'Paris is the capital and most
-populous city of France.'}, {'id': 1, 'title': 'Paris', 'url': 'https://
-en.wikipedia.org/wiki/Paris', 'article': "Since the 17th century, Paris has
-been one of Europe's major centres of science, and arts."}, {'id': 2, 'title':
-'Paris', 'url': 'https://en.wikipedia.org/wiki/Paris', 'article': 'The City of
-Paris is the centre and seat of government of the region and province of Ãle-
-de-France.' }] ``` ### Retriever ranker ð Here is an example of a neural
-search pipeline composed of a TF-IDF that quickly retrieves documents, followed
-by a ranking model. The ranking model sorts the documents produced by the
-retriever based on the semantic similarity between the query and the documents.
+Cherche enables the development of a neural search pipeline that employs
+retrievers and pre-trained language models both as retrievers and rankers. The
+primary advantage of Cherche lies in its capacity to construct end-to-end
+pipelines. Additionally, Cherche is well-suited for offline semantic search due
+to its compatibility with batch computation. [Live demo of a NLP search engine
+powered by Cherche](https://raphaelsty.github.io/knowledge/
+?query=cherche%20neural%20search) ![Alt text](docs/img/explain.png) ##
+Installation ð¤ To install Cherche for use with a simple retriever on CPU,
+such as TfIdf, Flash, Lunr, Fuzz, use the following command: ```sh pip install
+cherche ``` To install Cherche for use with any semantic retriever or ranker on
+CPU, use the following command: ```sh pip install "cherche[cpu]" ``` Finally,
+if you plan to use any semantic retriever or ranker on GPU, use the following
+command: ```sh pip install "cherche[gpu]" ``` By following these installation
+instructions, you will be able to use Cherche with the appropriate requirements
+for your needs. ### Documentation Documentation is available [here](https://
+raphaelsty.github.io/cherche/). It provides details about retrievers, rankers,
+pipelines and examples. ## QuickStart ð ### Documents Cherche allows
+findings the right document within a list of objects. Here is an example of a
+corpus. ```python from cherche import data documents = data.load_towns()
+documents[:3] [{'id': 0, 'title': 'Paris', 'url': 'https://en.wikipedia.org/
+wiki/Paris', 'article': 'Paris is the capital and most populous city of
+France.'}, {'id': 1, 'title': 'Paris', 'url': 'https://en.wikipedia.org/wiki/
+Paris', 'article': "Since the 17th century, Paris has been one of Europe's
+major centres of science, and arts."}, {'id': 2, 'title': 'Paris', 'url':
+'https://en.wikipedia.org/wiki/Paris', 'article': 'The City of Paris is the
+centre and seat of government of the region and province of Ãle-de-France.' }]
+``` ### Retriever ranker Here is an example of a neural search pipeline
+composed of a TF-IDF that quickly retrieves documents, followed by a ranking
+model. The ranking model sorts the documents produced by the retriever based on
+the semantic similarity between the query and the documents. We can call the
+pipeline using a list of queries and get relevant documents for each query.
 ```python from cherche import data, retrieve, rank from sentence_transformers
 import SentenceTransformer # List of dicts documents = data.load_towns() #
 Retrieve on fields title and article retriever = retrieve.TfIdf(key="id", on=
 ["title", "article"], documents=documents, k=30) # Rank on fields title and
 article ranker = rank.Encoder( key = "id", on = ["title", "article"], encoder =
 SentenceTransformer("sentence-transformers/all-mpnet-base-v2").encode, k = 3, )
 # Pipeline creation search = retriever + ranker search.add(documents=documents)
-search("Bordeaux") [{'id': 57, 'similarity': 0.69513476}, {'id': 63,
-'similarity': 0.6214991}, {'id': 65, 'similarity': 0.61809057}] ``` Map the
-index to the documents to access their contents. ```python search += documents
-search("Bordeaux") [{'id': 57, 'title': 'Bordeaux', 'url': 'https://
-en.wikipedia.org/wiki/Bordeaux', 'article': 'Bordeaux ( bor-DOH, French:
-[bÉÊdo] (listen); Gascon Occitan: BordÃ¨u [buÉ¾ËÃ°Éw]) is a port city on
-the river Garonne in the Gironde department, Southwestern France.',
-'similarity': 0.69513476}, {'id': 63, 'title': 'Bordeaux', 'url': 'https://
-en.wikipedia.org/wiki/Bordeaux', 'article': 'The term "Bordelais" may also
-refer to the city and its surrounding region.', 'similarity': 0.6214991},
-{'id': 65, 'title': 'Bordeaux', 'url': 'https://en.wikipedia.org/wiki/
-Bordeaux', 'article': "Bordeaux is a world capital of wine, with its castles
-and vineyards of the Bordeaux region that stand on the hillsides of the Gironde
-and is home to the world's main wine fair, Vinexpo.", 'similarity':
-0.61809057}] ``` ## Retrieve ð» Cherche provides different [retrievers]
-(https://raphaelsty.github.io/cherche/retrieve/retrieve/) that filter input
-documents based on a query. - retrieve.Elastic - retrieve.TfIdf - retrieve.Lunr
-- retrieve.BM25Okapi - retrieve.BM25L - retrieve.Flash - retrieve.Encoder -
-retrieve.DPR - retrieve.Fuzz - retrieve.Meilisearch - retrieve.TypeSense -
-retrieve.Recommend ## Rank ð¤ Cherche rankers are compatible with
+# Search documents for 3 queries. search(["Bordeaux", "Paris", "Toulouse"]) [[
+{'id': 57, 'similarity': 0.69513524}, {'id': 63, 'similarity': 0.6214994},
+{'id': 65, 'similarity': 0.61809087}], [{'id': 16, 'similarity': 0.59158516},
+{'id': 0, 'similarity': 0.58217555}, {'id': 1, 'similarity': 0.57944715}], [
+{'id': 26, 'similarity': 0.6925601}, {'id': 37, 'similarity': 0.63977146},
+{'id': 28, 'similarity': 0.62772334}]] ``` We can map the index to the
+documents to access their contents using pipelines: ```python search +=
+documents search(["Bordeaux", "Paris", "Toulouse"]) [[{'id': 57, 'title':
+'Bordeaux', 'url': 'https://en.wikipedia.org/wiki/Bordeaux', 'similarity':
+0.69513524}, {'id': 63, 'title': 'Bordeaux', 'similarity': 0.6214994}, {'id':
+65, 'title': 'Bordeaux', 'url': 'https://en.wikipedia.org/wiki/Bordeaux',
+'similarity': 0.61809087}], [{'id': 16, 'title': 'Paris', 'url': 'https://
+en.wikipedia.org/wiki/Paris', 'article': 'Paris received 12.', 'similarity':
+0.59158516}, {'id': 0, 'title': 'Paris', 'url': 'https://en.wikipedia.org/wiki/
+Paris', 'similarity': 0.58217555}, {'id': 1, 'title': 'Paris', 'url': 'https://
+en.wikipedia.org/wiki/Paris', 'similarity': 0.57944715}], [{'id': 26, 'title':
+'Toulouse', 'url': 'https://en.wikipedia.org/wiki/Toulouse', 'similarity':
+0.6925601}, {'id': 37, 'title': 'Toulouse', 'url': 'https://en.wikipedia.org/
+wiki/Toulouse', 'similarity': 0.63977146}, {'id': 28, 'title': 'Toulouse',
+'url': 'https://en.wikipedia.org/wiki/Toulouse', 'similarity': 0.62772334}]]
+``` ## Retrieve Cherche provides [retrievers](https://raphaelsty.github.io/
+cherche/retrieve/retrieve/) that filter input documents based on a query. -
+retrieve.TfIdf - retrieve.Lunr - retrieve.Flash - retrieve.Encoder -
+retrieve.DPR - retrieve.Fuzz - retrieve.Embedding ## Rank Cherche provides
+[rankers](https://raphaelsty.github.io/cherche/rank/rank/) that filter
+documents in output of retrievers. Cherche rankers are compatible with
 [SentenceTransformers](https://www.sbert.net/docs/pretrained_models.html)
-models, [Hugging Face sentence similarity](https://huggingface.co/
-models?pipeline_tag=zero-shot-classification&sort=downloads) models, [Hugging
-Face zero shot classification](https://huggingface.co/models?pipeline_tag=zero-
-shot-classification&sort=downloads) models, and of course with your own models.
-## Summarization and question answering Cherche provides modules dedicated to
-summarization and question answering. These modules are compatible with Hugging
-Face's pre-trained models and fully integrated into neural search pipelines. ##
-Translation Hugging Face's translation models can be fully integrated into the
-neural search pipeline to translate queries, documents, or answers. ##
-Collaborative filtering Search is fully compatible with the collaborative
-filtering library [Implicit](https://github.com/benfred/implicit). It is
-advantageous if you have a history associated with users and you want to
-retrieve / re-rank documents based on user preferences. | | **Document 1** |
-**Document 2** | **Document 3** | **Document 4** | |:----------:|:-------------
--:|:--------------:|:--------------:|:--------------:| | **User 1** | 1 | 0 | 0
-| 1 | | **User 2** | 0 | 1 | 0 | 0 | | **User 3** | 0 | 4 | 1 | 0 | ## Deploy
-We provide a minimalist API to deploy our neural search pipeline with FastAPI
-and Docker; information is available in the [documentation](https://
-raphaelsty.github.io/cherche/deployment/deployment/). ## Hugging Face Space A
-running demo is available on [Hugging Face](https://huggingface.co/spaces/
-raphaelsty/games). ## Contributors ð¤ Cherche was created for/by Renault and
-is now available to all. We welcome all contributions.
+models which are available on [Hugging Face hub](https://huggingface.co/
+models?pipeline_tag=zero-shot-classification&sort=downloads). - rank.Encoder -
+rank.DPR - rank.CrossEncoder - rank.Embedding ## Question answering Cherche
+provides modules dedicated to question answering. These modules are compatible
+with Hugging Face's pre-trained models and fully integrated into neural search
+pipelines. ## Contributors ð¤ Cherche was created for/by Renault and is now
+available to all. We welcome all contributions.
                             [docs/img/renault.jpg]
-## Acknowledgements ð The BM25 models available in Cherche are wrappers
-around [rank_bm25](https://github.com/dorianbrown/rank_bm25). Elastic retriever
-is a wrapper around [Python Elasticsearch Client](https://elasticsearch-
-py.readthedocs.io/en/v7.15.2/). TfIdf retriever is a wrapper around [scikit-
-learn's TfidfVectorizer](https://scikit-learn.org/stable/modules/generated/
+## Acknowledgements ð TfIdf retriever is a wrapper around [scikit-learn's
+TfidfVectorizer](https://scikit-learn.org/stable/modules/generated/
 sklearn.feature_extraction.text.TfidfVectorizer.html). Lunr retriever is a
 wrapper around [Lunr.py](https://github.com/yeraydiazdiaz/lunr.py). Flash
 retriever is a wrapper around [FlashText](https://github.com/vi3k6i5/
-flashtext). DPR and Encode rankers are wrappers dedicated to the use of the
-pre-trained models of [SentenceTransformers](https://www.sbert.net/docs/
-pretrained_models.html) in a neural search pipeline. ZeroShot ranker is a
-wrapper dedicated to the use of the zero-shot sequence classifiers of [Hugging
-Face](https://huggingface.co/models?pipeline_tag=zero-shot-
-classification&sort=downloads) in a neural search pipeline. ## See also ð
-Cherche is a minimalist solution and meets a need for modularity. Cherche is
-the way to go if we start with a list of documents as JSON with multiple fields
-to search on and create pipelines. Also, Cherche is well suited for middle-
-sized corpora. Do not hesitate to look at Jina, Haystack, or TxtAi, which offer
-advanced neural search solutions. - [Haystack](https://github.com/deepset-ai/
-haystack) - [Jina](https://github.com/jina-ai/jina) - [txtai](https://
-github.com/neuml/txtai) ## Citations If you use cherche to produce results for
-your scientific publication, please refer to our SIGIR paper: ```
-@inproceedings{Sourty2022sigir, author = {Raphael Sourty and Jose G. Moreno and
-Lynda Tamine and Francois-Paul Servant}, title = {CHERCHE: A new tool to
-rapidly implement pipelines in information retrieval}, booktitle = {Proceedings
-of SIGIR 2022}, year = {2022} } ``` ## Dev Team ð¾ The Cherche dev team is
-made up of [RaphaÃ«l Sourty](https://github.com/raphaelsty), [FranÃ§ois-Paul
-Servant](https://github.com/fpservant), [Nicolas Bizzozzero](https://
-github.com/NicolasBizzozzero), [Jose G Moreno](https://scholar.google.com/
-citations?user=4BZFUw8AAAAJ&hl=fr). ð¥³
+flashtext). DPR, Encode and CrossEncoder rankers are wrappers dedicated to the
+use of the pre-trained models of [SentenceTransformers](https://www.sbert.net/
+docs/pretrained_models.html) in a neural search pipeline. ## Citations If you
+use cherche to produce results for your scientific publication, please refer to
+our SIGIR paper: ``` @inproceedings{Sourty2022sigir, author = {Raphael Sourty
+and Jose G. Moreno and Lynda Tamine and Francois-Paul Servant}, title =
+{CHERCHE: A new tool to rapidly implement pipelines in information retrieval},
+booktitle = {Proceedings of SIGIR 2022}, year = {2022} } ``` ## Dev Team ð¾
+The Cherche dev team is made up of [RaphaÃ«l Sourty](https://github.com/
+raphaelsty), [FranÃ§ois-Paul Servant](https://github.com/fpservant), [Nicolas
+Bizzozzero](https://github.com/NicolasBizzozzero), [Jose G Moreno](https://
+scholar.google.com/citations?user=4BZFUw8AAAAJ&hl=fr). ð¥³
```

### Comparing `cherche-1.0.1/README.md` & `cherche-2.0.0/cherche.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,47 +1,80 @@
+Metadata-Version: 2.1
+Name: cherche
+Version: 2.0.0
+Summary: Neural Search
+Home-page: https://github.com/raphaelsty/cherche
+Download-URL: https://github.com/user/cherche/archive/v_01.tar.gz
+Author: Raphael Sourty
+Author-email: raphael.sourty@gmail.com
+License: MIT
+Keywords: neural search,information retrieval,question answering,semantic search
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+Provides-Extra: cpu
+Provides-Extra: gpu
+Provides-Extra: dev
+License-File: LICENSE
+
 <div align="center">
   <h1>Cherche</h1>
   <p>Neural search</p>
 </div>
-<br>
+
+<p align="center"><img width=300 src="docs/img/logo.png"/></p>
 
 <div align="center">
   <!-- Documentation -->
   <a href="https://raphaelsty.github.io/cherche/"><img src="https://img.shields.io/website?label=docs&style=flat-square&url=https%3A%2F%2Fraphaelsty.github.io/cherche/%2F" alt="documentation"></a>
   <!-- Demo -->
-  <a href="https://huggingface.co/spaces/raphaelsty/games"><img src="https://img.shields.io/badge/demo-running-blueviolet?style=flat-square" alt="Demo"></a>
+  <a href="https://raphaelsty.github.io/knowledge/?query=cherche%20neural%20search"><img src="https://img.shields.io/badge/demo-running-blueviolet?style=flat-square" alt="Demo"></a>
   <!-- License -->
   <a href="https://opensource.org/licenses/MIT"><img src="https://img.shields.io/badge/License-MIT-blue.svg?style=flat-square" alt="license"></a>
 </div>
-<br>
 
-Cherche allows the creation of efficient neural search pipelines using retrievers and pre-trained language models as rankers. Cherche's main strength is its ability to build diverse and end-to-end pipelines from lexical matching, semantic matching, and collaborative filtering-based models.
+
+Cherche enables the development of a neural search pipeline that employs retrievers and pre-trained language models both as retrievers and rankers. The primary advantage of Cherche lies in its capacity to construct end-to-end pipelines. Additionally, Cherche is well-suited for offline semantic search due to its compatibility with batch computation.
+
+[Live demo of a NLP search engine powered by Cherche](https://raphaelsty.github.io/knowledge/?query=cherche%20neural%20search)
 
 ![Alt text](docs/img/explain.png)
 
 ## Installation 🤖
 
+To install Cherche for use with a simple retriever on CPU, such as TfIdf, Flash, Lunr, Fuzz, use the following command:
+
 ```sh
-pip install cherche --upgrade
+pip install cherche
 ```
 
-To install the development version:
+To install Cherche for use with any semantic retriever or ranker on CPU, use the following command:
 
 ```sh
-pip install git+https://github.com/raphaelsty/cherche
+pip install "cherche[cpu]"
 ```
 
-## [Documentation](https://raphaelsty.github.io/cherche/) 📜
+Finally, if you plan to use any semantic retriever or ranker on GPU, use the following command:
+
+```sh
+pip install "cherche[gpu]"
+```
+
+By following these installation instructions, you will be able to use Cherche with the appropriate requirements for your needs.
+
+### Documentation
 
 Documentation is available [here](https://raphaelsty.github.io/cherche/). It provides details
-about retrievers, rankers, pipelines, question answering, summarization, and examples.
+about retrievers, rankers, pipelines and examples.
 
-## QuickStart 💨
+## QuickStart 📑
 
-### Documents 📑
+### Documents
 
 Cherche allows findings the right document within a list of objects. Here is an example of a corpus.
 
 ```python
 from cherche import data
 
 documents = data.load_towns()
@@ -58,17 +91,17 @@
  {'id': 2,
   'title': 'Paris',
   'url': 'https://en.wikipedia.org/wiki/Paris',
   'article': 'The City of Paris is the centre and seat of government of the region and province of Île-de-France.'
   }]
 ```
 
-### Retriever ranker 🔍
+### Retriever ranker
 
-Here is an example of a neural search pipeline composed of a TF-IDF that quickly retrieves documents, followed by a ranking model. The ranking model sorts the documents produced by the retriever based on the semantic similarity between the query and the documents.
+Here is an example of a neural search pipeline composed of a TF-IDF that quickly retrieves documents, followed by a ranking model. The ranking model sorts the documents produced by the retriever based on the semantic similarity between the query and the documents. We can call the pipeline using a list of queries and get relevant documents for each query.
 
 ```python
 from cherche import data, retrieve, rank
 from sentence_transformers import SentenceTransformer
 
 # List of dicts
 documents = data.load_towns()
@@ -85,108 +118,106 @@
 )
 
 # Pipeline creation
 search = retriever + ranker
 
 search.add(documents=documents)
 
-search("Bordeaux")
-[{'id': 57, 'similarity': 0.69513476},
- {'id': 63, 'similarity': 0.6214991},
- {'id': 65, 'similarity': 0.61809057}]
+# Search documents for 3 queries.
+search(["Bordeaux", "Paris", "Toulouse"])
+[[{'id': 57, 'similarity': 0.69513524},
+  {'id': 63, 'similarity': 0.6214994},
+  {'id': 65, 'similarity': 0.61809087}],
+ [{'id': 16, 'similarity': 0.59158516},
+  {'id': 0, 'similarity': 0.58217555},
+  {'id': 1, 'similarity': 0.57944715}],
+ [{'id': 26, 'similarity': 0.6925601},
+  {'id': 37, 'similarity': 0.63977146},
+  {'id': 28, 'similarity': 0.62772334}]]
 ```
 
-Map the index to the documents to access their contents.
+We can map the index to the documents to access their contents using pipelines:
 
 ```python
 search += documents
-search("Bordeaux")
-[{'id': 57,
-  'title': 'Bordeaux',
-  'url': 'https://en.wikipedia.org/wiki/Bordeaux',
-  'article': 'Bordeaux ( bor-DOH, French: [bɔʁdo] (listen); Gascon Occitan: Bordèu [buɾˈðɛw]) is a port city on the river Garonne in the Gironde department, Southwestern France.',
-  'similarity': 0.69513476},
- {'id': 63,
-  'title': 'Bordeaux',
-  'url': 'https://en.wikipedia.org/wiki/Bordeaux',
-  'article': 'The term "Bordelais" may also refer to the city and its surrounding region.',
-  'similarity': 0.6214991},
- {'id': 65,
-  'title': 'Bordeaux',
-  'url': 'https://en.wikipedia.org/wiki/Bordeaux',
-  'article': "Bordeaux is a world capital of wine, with its castles and vineyards of the Bordeaux region that stand on the hillsides of the Gironde and is home to the world's main wine fair, Vinexpo.",
-  'similarity': 0.61809057}]
+search(["Bordeaux", "Paris", "Toulouse"])
+[[{'id': 57,
+   'title': 'Bordeaux',
+   'url': 'https://en.wikipedia.org/wiki/Bordeaux',
+   'similarity': 0.69513524},
+  {'id': 63,
+   'title': 'Bordeaux',
+   'similarity': 0.6214994},
+  {'id': 65,
+   'title': 'Bordeaux',
+   'url': 'https://en.wikipedia.org/wiki/Bordeaux',
+   'similarity': 0.61809087}],
+ [{'id': 16,
+   'title': 'Paris',
+   'url': 'https://en.wikipedia.org/wiki/Paris',
+   'article': 'Paris received 12.',
+   'similarity': 0.59158516},
+  {'id': 0,
+   'title': 'Paris',
+   'url': 'https://en.wikipedia.org/wiki/Paris',
+   'similarity': 0.58217555},
+  {'id': 1,
+   'title': 'Paris',
+   'url': 'https://en.wikipedia.org/wiki/Paris',
+   'similarity': 0.57944715}],
+ [{'id': 26,
+   'title': 'Toulouse',
+   'url': 'https://en.wikipedia.org/wiki/Toulouse',
+   'similarity': 0.6925601},
+  {'id': 37,
+   'title': 'Toulouse',
+   'url': 'https://en.wikipedia.org/wiki/Toulouse',
+   'similarity': 0.63977146},
+  {'id': 28,
+   'title': 'Toulouse',
+   'url': 'https://en.wikipedia.org/wiki/Toulouse',
+   'similarity': 0.62772334}]]
 ```
 
-## Retrieve 👻
+## Retrieve
 
-Cherche provides different [retrievers](https://raphaelsty.github.io/cherche/retrieve/retrieve/) that filter input documents based on a query.
+Cherche provides [retrievers](https://raphaelsty.github.io/cherche/retrieve/retrieve/) that filter input documents based on a query.
 
-- retrieve.Elastic
 - retrieve.TfIdf
 - retrieve.Lunr
-- retrieve.BM25Okapi
-- retrieve.BM25L
 - retrieve.Flash
 - retrieve.Encoder
 - retrieve.DPR
 - retrieve.Fuzz
-- retrieve.Meilisearch
-- retrieve.TypeSense
-- retrieve.Recommend
-
-## Rank 🤗
+- retrieve.Embedding
 
-Cherche rankers are compatible with [SentenceTransformers](https://www.sbert.net/docs/pretrained_models.html) models, [Hugging Face sentence similarity](https://huggingface.co/models?pipeline_tag=zero-shot-classification&sort=downloads) models, [Hugging Face zero shot classification](https://huggingface.co/models?pipeline_tag=zero-shot-classification&sort=downloads) models, and of course with your own models.
+## Rank
 
-## Summarization and question answering
+Cherche provides [rankers](https://raphaelsty.github.io/cherche/rank/rank/) that filter documents in output of retrievers.
 
-Cherche provides modules dedicated to summarization and question answering. These modules are compatible with Hugging Face's pre-trained models and fully integrated into neural search pipelines.
+Cherche rankers are compatible with [SentenceTransformers](https://www.sbert.net/docs/pretrained_models.html) models which are available on [Hugging Face hub](https://huggingface.co/models?pipeline_tag=zero-shot-classification&sort=downloads).
 
-## Translation
+- rank.Encoder
+- rank.DPR
+- rank.CrossEncoder
+- rank.Embedding
 
-Hugging Face's translation models can be fully integrated into the neural search pipeline to translate queries, documents, or answers.
+## Question answering
 
-## Collaborative filtering
+Cherche provides modules dedicated to question answering. These modules are compatible with Hugging Face's pre-trained models and fully integrated into neural search pipelines.
 
-Search is fully compatible with the collaborative filtering library [Implicit](https://github.com/benfred/implicit). It is advantageous if you have a history associated with users and you want to retrieve / re-rank documents based on user preferences.
-
-|            | **Document 1** | **Document 2** | **Document 3** | **Document 4** |
-|:----------:|:--------------:|:--------------:|:--------------:|:--------------:|
-| **User 1** |        1       |        0       |        0       |        1       |
-| **User 2** |        0       |        1       |        0       |        0       |
-| **User 3** |        0       |        4       |        1       |        0       |
-
-
-## Deploy
-
-We provide a minimalist API to deploy our neural search pipeline with FastAPI and Docker; information is available in the [documentation](https://raphaelsty.github.io/cherche/deployment/deployment/).
-
-## Hugging Face Space
-
-A running demo is available on [Hugging Face](https://huggingface.co/spaces/raphaelsty/games).
 ## Contributors 🤝
 Cherche was created for/by Renault and is now available to all.
 We welcome all contributions.
 
 <p align="center"><img src="docs/img/renault.jpg"/></p>
 
 ## Acknowledgements 👏
 
-The BM25 models available in Cherche are wrappers around [rank_bm25](https://github.com/dorianbrown/rank_bm25). Elastic retriever is a wrapper around [Python Elasticsearch Client](https://elasticsearch-py.readthedocs.io/en/v7.15.2/). TfIdf retriever is a wrapper around [scikit-learn's TfidfVectorizer](https://scikit-learn.org/stable/modules/generated/sklearn.feature_extraction.text.TfidfVectorizer.html). Lunr retriever is a wrapper around [Lunr.py](https://github.com/yeraydiazdiaz/lunr.py). Flash retriever is a wrapper around [FlashText](https://github.com/vi3k6i5/flashtext). DPR and Encode rankers are wrappers dedicated to the use of the pre-trained models of [SentenceTransformers](https://www.sbert.net/docs/pretrained_models.html) in a neural search pipeline. ZeroShot ranker is a wrapper dedicated to the use of the zero-shot sequence classifiers of [Hugging Face](https://huggingface.co/models?pipeline_tag=zero-shot-classification&sort=downloads) in a neural search pipeline.
-
-## See also 👀
-
-Cherche is a minimalist solution and meets a need for modularity. Cherche is the way to go if we start with a list of documents as JSON with multiple fields to search on and create pipelines. Also, Cherche is well suited for middle-sized corpora.
-
-Do not hesitate to look at Jina, Haystack, or TxtAi, which offer advanced neural search solutions.
-
-- [Haystack](https://github.com/deepset-ai/haystack)
-- [Jina](https://github.com/jina-ai/jina)
-- [txtai](https://github.com/neuml/txtai)
+TfIdf retriever is a wrapper around [scikit-learn's TfidfVectorizer](https://scikit-learn.org/stable/modules/generated/sklearn.feature_extraction.text.TfidfVectorizer.html). Lunr retriever is a wrapper around [Lunr.py](https://github.com/yeraydiazdiaz/lunr.py). Flash retriever is a wrapper around [FlashText](https://github.com/vi3k6i5/flashtext). DPR, Encode and CrossEncoder rankers are wrappers dedicated to the use of the pre-trained models of [SentenceTransformers](https://www.sbert.net/docs/pretrained_models.html) in a neural search pipeline.
 
 ## Citations
 
 If you use cherche to produce results for your scientific publication, please refer to our SIGIR paper:
 
 ```
 @inproceedings{Sourty2022sigir,
```

#### html2text {}

```diff
@@ -1,109 +1,103 @@
+Metadata-Version: 2.1 Name: cherche Version: 2.0.0 Summary: Neural Search Home-
+page: https://github.com/raphaelsty/cherche Download-URL: https://github.com/
+user/cherche/archive/v_01.tar.gz Author: Raphael Sourty Author-email:
+raphael.sourty@gmail.com License: MIT Keywords: neural search,information
+retrieval,question answering,semantic search Classifier: Programming Language
+:: Python :: 3 Classifier: License :: OSI Approved :: MIT License Classifier:
+Operating System :: OS Independent Requires-Python: >=3.6 Description-Content-
+Type: text/markdown Provides-Extra: cpu Provides-Extra: gpu Provides-Extra: dev
+License-File: LICENSE
                              ****** Cherche ******
                                  Neural search
-
+                              [docs/img/logo.png]
                        [documentation]  [Demo]  [license]
-
-Cherche allows the creation of efficient neural search pipelines using
-retrievers and pre-trained language models as rankers. Cherche's main strength
-is its ability to build diverse and end-to-end pipelines from lexical matching,
-semantic matching, and collaborative filtering-based models. ![Alt text](docs/
-img/explain.png) ## Installation ð¤ ```sh pip install cherche --upgrade ```
-To install the development version: ```sh pip install git+https://github.com/
-raphaelsty/cherche ``` ## [Documentation](https://raphaelsty.github.io/cherche/
-) ð Documentation is available [here](https://raphaelsty.github.io/cherche/
-). It provides details about retrievers, rankers, pipelines, question
-answering, summarization, and examples. ## QuickStart ð¨ ### Documents ð
-Cherche allows findings the right document within a list of objects. Here is an
-example of a corpus. ```python from cherche import data documents =
-data.load_towns() documents[:3] [{'id': 0, 'title': 'Paris', 'url': 'https://
-en.wikipedia.org/wiki/Paris', 'article': 'Paris is the capital and most
-populous city of France.'}, {'id': 1, 'title': 'Paris', 'url': 'https://
-en.wikipedia.org/wiki/Paris', 'article': "Since the 17th century, Paris has
-been one of Europe's major centres of science, and arts."}, {'id': 2, 'title':
-'Paris', 'url': 'https://en.wikipedia.org/wiki/Paris', 'article': 'The City of
-Paris is the centre and seat of government of the region and province of Ãle-
-de-France.' }] ``` ### Retriever ranker ð Here is an example of a neural
-search pipeline composed of a TF-IDF that quickly retrieves documents, followed
-by a ranking model. The ranking model sorts the documents produced by the
-retriever based on the semantic similarity between the query and the documents.
+Cherche enables the development of a neural search pipeline that employs
+retrievers and pre-trained language models both as retrievers and rankers. The
+primary advantage of Cherche lies in its capacity to construct end-to-end
+pipelines. Additionally, Cherche is well-suited for offline semantic search due
+to its compatibility with batch computation. [Live demo of a NLP search engine
+powered by Cherche](https://raphaelsty.github.io/knowledge/
+?query=cherche%20neural%20search) ![Alt text](docs/img/explain.png) ##
+Installation ð¤ To install Cherche for use with a simple retriever on CPU,
+such as TfIdf, Flash, Lunr, Fuzz, use the following command: ```sh pip install
+cherche ``` To install Cherche for use with any semantic retriever or ranker on
+CPU, use the following command: ```sh pip install "cherche[cpu]" ``` Finally,
+if you plan to use any semantic retriever or ranker on GPU, use the following
+command: ```sh pip install "cherche[gpu]" ``` By following these installation
+instructions, you will be able to use Cherche with the appropriate requirements
+for your needs. ### Documentation Documentation is available [here](https://
+raphaelsty.github.io/cherche/). It provides details about retrievers, rankers,
+pipelines and examples. ## QuickStart ð ### Documents Cherche allows
+findings the right document within a list of objects. Here is an example of a
+corpus. ```python from cherche import data documents = data.load_towns()
+documents[:3] [{'id': 0, 'title': 'Paris', 'url': 'https://en.wikipedia.org/
+wiki/Paris', 'article': 'Paris is the capital and most populous city of
+France.'}, {'id': 1, 'title': 'Paris', 'url': 'https://en.wikipedia.org/wiki/
+Paris', 'article': "Since the 17th century, Paris has been one of Europe's
+major centres of science, and arts."}, {'id': 2, 'title': 'Paris', 'url':
+'https://en.wikipedia.org/wiki/Paris', 'article': 'The City of Paris is the
+centre and seat of government of the region and province of Ãle-de-France.' }]
+``` ### Retriever ranker Here is an example of a neural search pipeline
+composed of a TF-IDF that quickly retrieves documents, followed by a ranking
+model. The ranking model sorts the documents produced by the retriever based on
+the semantic similarity between the query and the documents. We can call the
+pipeline using a list of queries and get relevant documents for each query.
 ```python from cherche import data, retrieve, rank from sentence_transformers
 import SentenceTransformer # List of dicts documents = data.load_towns() #
 Retrieve on fields title and article retriever = retrieve.TfIdf(key="id", on=
 ["title", "article"], documents=documents, k=30) # Rank on fields title and
 article ranker = rank.Encoder( key = "id", on = ["title", "article"], encoder =
 SentenceTransformer("sentence-transformers/all-mpnet-base-v2").encode, k = 3, )
 # Pipeline creation search = retriever + ranker search.add(documents=documents)
-search("Bordeaux") [{'id': 57, 'similarity': 0.69513476}, {'id': 63,
-'similarity': 0.6214991}, {'id': 65, 'similarity': 0.61809057}] ``` Map the
-index to the documents to access their contents. ```python search += documents
-search("Bordeaux") [{'id': 57, 'title': 'Bordeaux', 'url': 'https://
-en.wikipedia.org/wiki/Bordeaux', 'article': 'Bordeaux ( bor-DOH, French:
-[bÉÊdo] (listen); Gascon Occitan: BordÃ¨u [buÉ¾ËÃ°Éw]) is a port city on
-the river Garonne in the Gironde department, Southwestern France.',
-'similarity': 0.69513476}, {'id': 63, 'title': 'Bordeaux', 'url': 'https://
-en.wikipedia.org/wiki/Bordeaux', 'article': 'The term "Bordelais" may also
-refer to the city and its surrounding region.', 'similarity': 0.6214991},
-{'id': 65, 'title': 'Bordeaux', 'url': 'https://en.wikipedia.org/wiki/
-Bordeaux', 'article': "Bordeaux is a world capital of wine, with its castles
-and vineyards of the Bordeaux region that stand on the hillsides of the Gironde
-and is home to the world's main wine fair, Vinexpo.", 'similarity':
-0.61809057}] ``` ## Retrieve ð» Cherche provides different [retrievers]
-(https://raphaelsty.github.io/cherche/retrieve/retrieve/) that filter input
-documents based on a query. - retrieve.Elastic - retrieve.TfIdf - retrieve.Lunr
-- retrieve.BM25Okapi - retrieve.BM25L - retrieve.Flash - retrieve.Encoder -
-retrieve.DPR - retrieve.Fuzz - retrieve.Meilisearch - retrieve.TypeSense -
-retrieve.Recommend ## Rank ð¤ Cherche rankers are compatible with
+# Search documents for 3 queries. search(["Bordeaux", "Paris", "Toulouse"]) [[
+{'id': 57, 'similarity': 0.69513524}, {'id': 63, 'similarity': 0.6214994},
+{'id': 65, 'similarity': 0.61809087}], [{'id': 16, 'similarity': 0.59158516},
+{'id': 0, 'similarity': 0.58217555}, {'id': 1, 'similarity': 0.57944715}], [
+{'id': 26, 'similarity': 0.6925601}, {'id': 37, 'similarity': 0.63977146},
+{'id': 28, 'similarity': 0.62772334}]] ``` We can map the index to the
+documents to access their contents using pipelines: ```python search +=
+documents search(["Bordeaux", "Paris", "Toulouse"]) [[{'id': 57, 'title':
+'Bordeaux', 'url': 'https://en.wikipedia.org/wiki/Bordeaux', 'similarity':
+0.69513524}, {'id': 63, 'title': 'Bordeaux', 'similarity': 0.6214994}, {'id':
+65, 'title': 'Bordeaux', 'url': 'https://en.wikipedia.org/wiki/Bordeaux',
+'similarity': 0.61809087}], [{'id': 16, 'title': 'Paris', 'url': 'https://
+en.wikipedia.org/wiki/Paris', 'article': 'Paris received 12.', 'similarity':
+0.59158516}, {'id': 0, 'title': 'Paris', 'url': 'https://en.wikipedia.org/wiki/
+Paris', 'similarity': 0.58217555}, {'id': 1, 'title': 'Paris', 'url': 'https://
+en.wikipedia.org/wiki/Paris', 'similarity': 0.57944715}], [{'id': 26, 'title':
+'Toulouse', 'url': 'https://en.wikipedia.org/wiki/Toulouse', 'similarity':
+0.6925601}, {'id': 37, 'title': 'Toulouse', 'url': 'https://en.wikipedia.org/
+wiki/Toulouse', 'similarity': 0.63977146}, {'id': 28, 'title': 'Toulouse',
+'url': 'https://en.wikipedia.org/wiki/Toulouse', 'similarity': 0.62772334}]]
+``` ## Retrieve Cherche provides [retrievers](https://raphaelsty.github.io/
+cherche/retrieve/retrieve/) that filter input documents based on a query. -
+retrieve.TfIdf - retrieve.Lunr - retrieve.Flash - retrieve.Encoder -
+retrieve.DPR - retrieve.Fuzz - retrieve.Embedding ## Rank Cherche provides
+[rankers](https://raphaelsty.github.io/cherche/rank/rank/) that filter
+documents in output of retrievers. Cherche rankers are compatible with
 [SentenceTransformers](https://www.sbert.net/docs/pretrained_models.html)
-models, [Hugging Face sentence similarity](https://huggingface.co/
-models?pipeline_tag=zero-shot-classification&sort=downloads) models, [Hugging
-Face zero shot classification](https://huggingface.co/models?pipeline_tag=zero-
-shot-classification&sort=downloads) models, and of course with your own models.
-## Summarization and question answering Cherche provides modules dedicated to
-summarization and question answering. These modules are compatible with Hugging
-Face's pre-trained models and fully integrated into neural search pipelines. ##
-Translation Hugging Face's translation models can be fully integrated into the
-neural search pipeline to translate queries, documents, or answers. ##
-Collaborative filtering Search is fully compatible with the collaborative
-filtering library [Implicit](https://github.com/benfred/implicit). It is
-advantageous if you have a history associated with users and you want to
-retrieve / re-rank documents based on user preferences. | | **Document 1** |
-**Document 2** | **Document 3** | **Document 4** | |:----------:|:-------------
--:|:--------------:|:--------------:|:--------------:| | **User 1** | 1 | 0 | 0
-| 1 | | **User 2** | 0 | 1 | 0 | 0 | | **User 3** | 0 | 4 | 1 | 0 | ## Deploy
-We provide a minimalist API to deploy our neural search pipeline with FastAPI
-and Docker; information is available in the [documentation](https://
-raphaelsty.github.io/cherche/deployment/deployment/). ## Hugging Face Space A
-running demo is available on [Hugging Face](https://huggingface.co/spaces/
-raphaelsty/games). ## Contributors ð¤ Cherche was created for/by Renault and
-is now available to all. We welcome all contributions.
+models which are available on [Hugging Face hub](https://huggingface.co/
+models?pipeline_tag=zero-shot-classification&sort=downloads). - rank.Encoder -
+rank.DPR - rank.CrossEncoder - rank.Embedding ## Question answering Cherche
+provides modules dedicated to question answering. These modules are compatible
+with Hugging Face's pre-trained models and fully integrated into neural search
+pipelines. ## Contributors ð¤ Cherche was created for/by Renault and is now
+available to all. We welcome all contributions.
                             [docs/img/renault.jpg]
-## Acknowledgements ð The BM25 models available in Cherche are wrappers
-around [rank_bm25](https://github.com/dorianbrown/rank_bm25). Elastic retriever
-is a wrapper around [Python Elasticsearch Client](https://elasticsearch-
-py.readthedocs.io/en/v7.15.2/). TfIdf retriever is a wrapper around [scikit-
-learn's TfidfVectorizer](https://scikit-learn.org/stable/modules/generated/
+## Acknowledgements ð TfIdf retriever is a wrapper around [scikit-learn's
+TfidfVectorizer](https://scikit-learn.org/stable/modules/generated/
 sklearn.feature_extraction.text.TfidfVectorizer.html). Lunr retriever is a
 wrapper around [Lunr.py](https://github.com/yeraydiazdiaz/lunr.py). Flash
 retriever is a wrapper around [FlashText](https://github.com/vi3k6i5/
-flashtext). DPR and Encode rankers are wrappers dedicated to the use of the
-pre-trained models of [SentenceTransformers](https://www.sbert.net/docs/
-pretrained_models.html) in a neural search pipeline. ZeroShot ranker is a
-wrapper dedicated to the use of the zero-shot sequence classifiers of [Hugging
-Face](https://huggingface.co/models?pipeline_tag=zero-shot-
-classification&sort=downloads) in a neural search pipeline. ## See also ð
-Cherche is a minimalist solution and meets a need for modularity. Cherche is
-the way to go if we start with a list of documents as JSON with multiple fields
-to search on and create pipelines. Also, Cherche is well suited for middle-
-sized corpora. Do not hesitate to look at Jina, Haystack, or TxtAi, which offer
-advanced neural search solutions. - [Haystack](https://github.com/deepset-ai/
-haystack) - [Jina](https://github.com/jina-ai/jina) - [txtai](https://
-github.com/neuml/txtai) ## Citations If you use cherche to produce results for
-your scientific publication, please refer to our SIGIR paper: ```
-@inproceedings{Sourty2022sigir, author = {Raphael Sourty and Jose G. Moreno and
-Lynda Tamine and Francois-Paul Servant}, title = {CHERCHE: A new tool to
-rapidly implement pipelines in information retrieval}, booktitle = {Proceedings
-of SIGIR 2022}, year = {2022} } ``` ## Dev Team ð¾ The Cherche dev team is
-made up of [RaphaÃ«l Sourty](https://github.com/raphaelsty), [FranÃ§ois-Paul
-Servant](https://github.com/fpservant), [Nicolas Bizzozzero](https://
-github.com/NicolasBizzozzero), [Jose G Moreno](https://scholar.google.com/
-citations?user=4BZFUw8AAAAJ&hl=fr). ð¥³
+flashtext). DPR, Encode and CrossEncoder rankers are wrappers dedicated to the
+use of the pre-trained models of [SentenceTransformers](https://www.sbert.net/
+docs/pretrained_models.html) in a neural search pipeline. ## Citations If you
+use cherche to produce results for your scientific publication, please refer to
+our SIGIR paper: ``` @inproceedings{Sourty2022sigir, author = {Raphael Sourty
+and Jose G. Moreno and Lynda Tamine and Francois-Paul Servant}, title =
+{CHERCHE: A new tool to rapidly implement pipelines in information retrieval},
+booktitle = {Proceedings of SIGIR 2022}, year = {2022} } ``` ## Dev Team ð¾
+The Cherche dev team is made up of [RaphaÃ«l Sourty](https://github.com/
+raphaelsty), [FranÃ§ois-Paul Servant](https://github.com/fpservant), [Nicolas
+Bizzozzero](https://github.com/NicolasBizzozzero), [Jose G Moreno](https://
+scholar.google.com/citations?user=4BZFUw8AAAAJ&hl=fr). ð¥³
```

### Comparing `cherche-1.0.1/cherche/compose/test_compose.py` & `cherche-2.0.0/cherche/compose/test_compose.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,57 +1,45 @@
 import pytest
 
 from .. import rank, retrieve
 
 
-def cherche_retrievers(key: str, on: str, k: int = None):
+def cherche_retrievers(key: str, on: str):
     """List of retrievers available in cherche."""
     yield from [
-        retrieve.TfIdf(key=key, on=on, documents=documents(), k=k),
-        retrieve.BM25Okapi(key=key, on=on, documents=documents(), k=k),
-        retrieve.BM25L(key=key, on=on, documents=documents(), k=k),
-        retrieve.Lunr(key=key, on=on, documents=documents(), k=k),
+        retrieve.TfIdf(key=key, on=on, documents=documents()),
+        retrieve.Lunr(key=key, on=on, documents=documents()),
     ]
 
 
-def cherche_rankers(key: str, on: str, k: int = None, path: str = None):
+def cherche_rankers(key: str, on: str):
     """List of rankers available in cherche."""
-    from sentence_transformers import SentenceTransformer
-    from transformers import pipeline
+    from sentence_transformers import CrossEncoder, SentenceTransformer
 
     yield from [
         rank.DPR(
             key=key,
             on=on,
             encoder=SentenceTransformer(
                 "facebook-dpr-ctx_encoder-single-nq-base"
             ).encode,
             query_encoder=SentenceTransformer(
                 "facebook-dpr-question_encoder-single-nq-base"
             ).encode,
-            k=k,
-            path=path,
         ),
         rank.Encoder(
             key=key,
             on="title",
             encoder=SentenceTransformer(
                 "sentence-transformers/all-mpnet-base-v2"
             ).encode,
-            k=k,
-            path=path,
         ),
-        rank.ZeroShot(
-            key=key,
+        rank.CrossEncoder(
             on=on,
-            encoder=pipeline(
-                "zero-shot-classification",
-                model="typeform/distilbert-base-uncased-mnli",
-            ),
-            k=k,
+            encoder=CrossEncoder("cross-encoder/mmarco-mMiniLMv2-L12-H384-v1").predict,
         ),
     ]
 
 
 def documents():
     return [
         {
@@ -93,71 +81,71 @@
 
 
 @pytest.mark.parametrize(
     "search, documents, k",
     [
         pytest.param(
             retriever + ranker + documents()
-            if not isinstance(ranker, rank.ZeroShot)
+            if not isinstance(ranker, rank.CrossEncoder)
             else retriever + documents() + ranker,
             documents(),
             k,
             id=f"retriever: {retriever.__class__.__name__}, ranker: {ranker.__class__.__name__}, k: {k}",
         )
-        for k in [None, 0, 2, 4]
-        for ranker in cherche_rankers(key="url", on="title", k=k, path=None)
-        for retriever in cherche_retrievers(key="url", on="title", k=k)
+        for k in [None, 2, 4]
+        for ranker in cherche_rankers(key="url", on="title")
+        for retriever in cherche_retrievers(key="url", on="title")
     ],
 )
 def test_retriever_ranker(search, documents: list, k: int):
     """Test retriever ranker pipeline. Test if the number of retrieved documents is coherent.
     Check if the number of documents asked is higher than the actual number of documents retrieved.
     Check if the retriever do not find any document.
     """
     search = search.add(documents)
 
-    answers = search(q="Github library with PyTorch and Transformers")
+    answers = search(q="Github library with PyTorch and Transformers", k=k)
     for index in range(len(documents) if k is None else k):
         if index in [0, 1]:
             assert (
                 answers[index]["title"]
                 == "Github library with Pytorch and Transformers."
             )
         elif index in [2]:
             assert answers[index]["title"] == "Github Library with PyTorch."
 
-    answers = search(q="Github")
+    answers = search(q="Github", k=k)
     if k is None:
         assert len(answers) == len(documents)
     else:
         assert len(answers) == min(k, len(documents))
 
     for sample in answers:
         for key in ["url", "title", "date"]:
             assert key in sample
 
 
 @pytest.mark.parametrize(
     "search, documents, k",
     [
         pytest.param(
-            retrieve.Flash(key="uri", on="tags", k=k) + ranker + tags()
-            if not isinstance(ranker, rank.ZeroShot)
-            else retrieve.Flash(key="uri", on="tags", k=k) + tags() + ranker,
+            retrieve.Flash(key="uri", on="tags") + ranker + tags()
+            if not isinstance(ranker, rank.CrossEncoder)
+            else retrieve.Flash(key="uri", on="tags") + tags() + ranker,
             tags(),
             k,
             id=f"retriever: Flash, ranker: {ranker.__class__.__name__}, k: {k}",
         )
         for k in [None, 0, 2, 4]
-        for ranker in cherche_rankers(key="uri", on="title", k=k, path=None)
+        for ranker in cherche_rankers(key="uri", on="title")
     ],
 )
 def test_flash_ranker(search, documents: list, k: int):
     search = search.add(documents)
-    answers = search(q="Github ( git ) is a great tool")
+    answers = search(q="Github ( git ) is a great tool", k=k)
     if k is None:
         assert len(answers) == 2
     else:
         assert len(answers) == min(k, 2)
     for sample in answers:
         for key in ["tags", "title", "uri"]:
             assert key in sample
```

### Comparing `cherche-1.0.1/cherche/compose/test_union_inter.py` & `cherche-2.0.0/cherche/compose/test_union_inter.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,59 +1,47 @@
 import pytest
 
 from .. import rank, retrieve
 
 
-def cherche_retrievers(key: str, on: str, k: int = None):
+def cherche_retrievers(key: str, on: str):
     """List of retrievers available in cherche."""
     for retriever in [
         retrieve.TfIdf,
-        retrieve.BM25Okapi,
-        retrieve.BM25L,
         retrieve.Lunr,
     ]:
-        yield retriever(key=key, on=on, documents=documents(), k=k)
+        yield retriever(key=key, on=on, documents=documents())
 
 
-def cherche_rankers(key: str, on: str, k: int = None, path: str = None):
+def cherche_rankers(key: str, on: str):
     """List of rankers available in cherche."""
-    from sentence_transformers import SentenceTransformer
+    from sentence_transformers import CrossEncoder, SentenceTransformer
     from transformers import pipeline
 
     yield from [
         rank.DPR(
             encoder=SentenceTransformer(
                 "facebook-dpr-ctx_encoder-single-nq-base",
             ).encode,
             query_encoder=SentenceTransformer(
                 "facebook-dpr-question_encoder-single-nq-base",
             ).encode,
             key=key,
             on=on,
-            k=k,
-            path=path,
         ),
         rank.Encoder(
             encoder=SentenceTransformer(
                 "sentence-transformers/all-mpnet-base-v2",
             ).encode,
             key=key,
             on=on,
-            k=k,
-            path=path,
         ),
-        rank.ZeroShot(
-            encoder=pipeline(
-                "zero-shot-classification",
-                model="typeform/distilbert-base-uncased-mnli",
-                cache="cache",
-            ),
-            key=key,
+        rank.CrossEncoder(
             on=on,
-            k=k,
+            encoder=CrossEncoder("cross-encoder/mmarco-mMiniLMv2-L12-H384-v1").predict,
         ),
     ]
 
 
 def documents():
     return [
         {
@@ -83,32 +71,32 @@
         pytest.param(
             (retriever_a | retriever_b | retriever_c) + documents(),
             documents(),
             k,
             id=f"Union retrievers: {retriever_a.__class__.__name__} | {retriever_b.__class__.__name__} | {retriever_c.__class__.__name__} k: {k}",
         )
         for k in [None, 3, 4]
-        for retriever_c in cherche_retrievers(key="id", on="title", k=k)
-        for retriever_b in cherche_retrievers(key="id", on="article", k=k)
-        for retriever_a in cherche_retrievers(key="id", on="author", k=k)
+        for retriever_c in cherche_retrievers(key="id", on="title")
+        for retriever_b in cherche_retrievers(key="id", on="article")
+        for retriever_a in cherche_retrievers(key="id", on="author")
     ],
 )
 def test_retriever_union(search, documents: list, k: int):
     """Test retriever union operator."""
     # Empty documents
     search = search.add(documents)
 
-    answers = search(q="France")
+    answers = search(q="France", k=k)
     assert len(answers) == min(k, 1) if k is not None else 1
 
     for sample in answers:
         for key in ["title", "article", "author"]:
             assert key in sample
 
-    answers = search(q="Wikipedia")
+    answers = search(q="Wikipedia", k=k)
     assert len(answers) == min(k, len(documents)) if k is not None else len(documents)
 
     answers = search(q="Unknown")
     assert len(answers) == 0
 
 
 @pytest.mark.parametrize(
@@ -117,39 +105,39 @@
         pytest.param(
             (retriever_a & retriever_b & retriever_c) + documents(),
             documents(),
             k,
             id=f"Intersection retrievers: {retriever_a.__class__.__name__} & {retriever_b.__class__.__name__}, & {retriever_c.__class__.__name__},  k: {k}",
         )
         for k in [None, 3, 4]
-        for retriever_c in cherche_retrievers(key="id", on="title", k=k)
-        for retriever_b in cherche_retrievers(key="id", on="article", k=k)
-        for retriever_a in cherche_retrievers(key="id", on="author", k=k)
+        for retriever_c in cherche_retrievers(key="id", on="title")
+        for retriever_b in cherche_retrievers(key="id", on="article")
+        for retriever_a in cherche_retrievers(key="id", on="author")
     ],
 )
 def test_retriever_intersection(search, documents: list, k: int):
     """Test retriever intersection operator."""
     # Empty documents
     search = search.add(documents)
 
-    answers = search(q="Paris tower capital Montreal Canada France Wikipedia")
+    answers = search(q="Paris tower capital Montreal Canada France Wikipedia", k=k)
     if k is not None and k < len(documents):
         assert len(answers) >= (k // 3)
     else:
         assert len(answers) == len(documents)
     assert len(answers) <= len(documents)
 
     for sample in answers:
         for key in ["title", "article", "author"]:
             assert key in sample
 
-    answers = search(q="is Wikipedia")
+    answers = search(q="is Wikipedia", k=k)
     assert len(answers) == 0
 
-    answers = search(q="Paris capital France Wikipedia")
+    answers = search(q="Paris capital France Wikipedia", k=k)
     if k is None or k >= 1:
         assert len(answers) == 1
     else:
         assert len(answers) == 0
 
 
 @pytest.mark.parametrize(
@@ -158,87 +146,85 @@
         pytest.param(
             ranker_a | ranker_b,
             documents(),
             k,
             id=f"Union rankers: {ranker_a.__class__.__name__} | {ranker_b.__class__.__name__} k: {k}",
         )
         for k in [None, 3, 4]
-        for ranker_b in cherche_rankers(key="id", on="article", k=k)
-        for ranker_a in cherche_rankers(key="id", on="title", k=k)
+        for ranker_b in cherche_rankers(key="id", on="article")
+        for ranker_a in cherche_rankers(key="id", on="title")
     ],
 )
 def test_ranker_union(search, documents: list, k: int):
     """Test retriever union operator."""
     search.add(documents)
-    answers = search(q="Eiffel tower France", documents=documents)
+    answers = search(q="Eiffel tower France", documents=documents, k=k)
 
     if k is not None:
         assert len(answers) == min(k, len(documents))
     else:
         assert len(answers) == len(documents)
 
     for index, sample in enumerate(answers):
-
         for key in ["title", "article", "author"]:
             assert key in sample
 
         if index == 0:
             assert sample["title"] == "Eiffel tower"
 
-    answers = search(q="Canada", documents=documents)
+    answers = search(q="Canada", documents=documents, k=k)
 
     if k is None:
         assert answers[0]["title"] == "Montreal"
     elif k >= 1:
         assert answers[0]["title"] == "Montreal"
     else:
         assert len(answers) == 0
 
     # Empty documents.
-    answers = search(q="Paris", documents=[])
+    answers = search(q="Paris", documents=[], k=k)
     assert len(answers) == 0
 
 
 @pytest.mark.parametrize(
     "search, documents, k",
     [
         pytest.param(
             ranker_a & ranker_b,
             documents(),
             k,
             id=f"Intersection rankers: {ranker_a.__class__.__name__} | {ranker_b.__class__.__name__} k: {k}",
         )
         for k in [None, 3, 4]
-        for ranker_b in cherche_rankers(key="id", on="article", k=k)
-        for ranker_a in cherche_rankers(key="id", on="title", k=k)
+        for ranker_b in cherche_rankers(key="id", on="article")
+        for ranker_a in cherche_rankers(key="id", on="title")
     ],
 )
 def test_ranker_intersection(search, documents: list, k: int):
     """Test retriever intersection operator."""
     search.add(documents)
-    answers = search(q="Eiffel tower France", documents=documents)
+    answers = search(q="Eiffel tower France", documents=documents, k=k)
 
     if k is not None:
         assert len(answers) == min(k, len(documents))
     else:
         assert len(answers) == len(documents)
 
     for index, sample in enumerate(answers):
-
         for key in ["title", "article", "author"]:
             assert key in sample
 
         if index == 0:
             assert sample["title"] == "Eiffel tower"
 
-    answers = search(q="Canada", documents=documents)
+    answers = search(q="Canada", documents=documents, k=k)
 
     if k is None:
         assert answers[0]["title"] == "Montreal"
     elif k >= 1:
         assert answers[0]["title"] == "Montreal"
     else:
         assert len(answers) == 0
 
     # Empty documents.
-    answers = search(q="Paris", documents=[])
+    answers = search(q="Paris", documents=[], k=k)
     assert len(answers) == 0
```

### Comparing `cherche-1.0.1/cherche/compose/test_vote.py` & `cherche-2.0.0/cherche/compose/test_vote.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 import pytest
 
 from .. import rank, retrieve
 
 
-def cherche_retrievers(key: str, on: str, k: int = None):
+def cherche_retrievers(key: str, on: str):
     """List of retrievers available in cherche."""
     for retriever in [
         retrieve.TfIdf,
-        retrieve.BM25Okapi,
-        retrieve.BM25L,
         retrieve.Lunr,
     ]:
-        yield retriever(key=key, on=on, documents=documents(), k=k)
+        yield retriever(key=key, on=on, documents=documents())
 
 
 def documents():
     return [
         {
             "id": 0,
             "title": "Paris",
@@ -43,29 +41,29 @@
         pytest.param(
             (retriever_a * retriever_b * retriever_c) + documents(),
             documents(),
             k,
             id=f"Union retrievers: {retriever_a.__class__.__name__} | {retriever_b.__class__.__name__} | {retriever_c.__class__.__name__} k: {k}",
         )
         for k in [None, 3, 4]
-        for retriever_c in cherche_retrievers(key="id", on="title", k=k)
-        for retriever_b in cherche_retrievers(key="id", on="article", k=k)
-        for retriever_a in cherche_retrievers(key="id", on="author", k=k)
+        for retriever_c in cherche_retrievers(key="id", on="title")
+        for retriever_b in cherche_retrievers(key="id", on="article")
+        for retriever_a in cherche_retrievers(key="id", on="author")
     ],
 )
 def test_retriever_union(search, documents: list, k: int):
     """Test retriever union operator."""
     # Empty documents
     search = search.add(documents)
 
-    answers = search(q="France")
+    answers = search(q="France", k=k)
     assert len(answers) == min(k, 1) if k is not None else 1
 
     for sample in answers:
         for key in ["title", "article", "author"]:
             assert key in sample
 
-    answers = search(q="Wikipedia")
+    answers = search(q="Wikipedia", k=k)
     assert len(answers) == min(k, len(documents)) if k is not None else len(documents)
 
-    answers = search(q="Unknown")
+    answers = search(q="Unknown", k=k)
     assert len(answers) == 0
```

### Comparing `cherche-1.0.1/cherche/data/semanlink/arxiv.json` & `cherche-2.0.0/cherche/data/semanlink/arxiv.json`

 * *Files identical despite different names*

### Comparing `cherche-1.0.1/cherche/data/semanlink/docs.json` & `cherche-2.0.0/cherche/data/semanlink/docs.json`

 * *Files identical despite different names*

### Comparing `cherche-1.0.1/cherche/data/semanlink/tags.json` & `cherche-2.0.0/cherche/data/semanlink/tags.json`

 * *Files identical despite different names*

### Comparing `cherche-1.0.1/cherche/data/semanlink.py` & `cherche-2.0.0/cherche/data/semanlink.py`

 * *Files identical despite different names*

### Comparing `cherche-1.0.1/cherche/data/towns.json` & `cherche-2.0.0/cherche/data/towns.json`

 * *Files identical despite different names*

### Comparing `cherche-1.0.1/cherche/data/towns.py` & `cherche-2.0.0/cherche/data/towns.py`

 * *Files identical despite different names*

### Comparing `cherche-1.0.1/cherche/generate/base.py` & `cherche-2.0.0/cherche/retrieve/base.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,58 +1,85 @@
 import abc
 import typing
 
-from ..compose import Pipeline
+from ..compose import Intersection, Pipeline, Union, Vote
 
+__all__ = ["Retriever"]
 
-class Generation(abc.ABC):
-    """Generation base class.
+
+class Retriever(abc.ABC):
+    """Retriever base class.
 
     Parameters
     ----------
     key
         Field identifier of each document.
     on
         Fields to use to match the query to the documents.
-    k
-        Number of documents to retrieve. Default is None, i.e all documents that match the query
-        will be retrieved.
-
     """
 
     def __init__(
         self,
+        key: str,
         on: typing.Union[str, list],
-        tokenizer,
-        model,
-        k: int,
-        num_beams: int,
-        min_length: int,
-        max_length: int,
+        k: typing.Optional[int],
+        batch_size: int,
     ) -> None:
         super().__init__()
-        self.on = on
-        self.tokenizer = tokenizer
-        self.model = model
+        self.key = key
+        self.on = on if isinstance(on, list) else [on]
+        self.documents = None
         self.k = k
-        self.num_beams = num_beams
-        self.min_length = min_length
-        self.max_length = max_length
+        self.batch_size = batch_size
 
     def __repr__(self) -> str:
-        repr = "Base Generation"
+        repr = f"{self.__class__.__name__} retriever"
+        repr += f"\n\tkey      : {self.key}"
+        repr += f"\n\ton       : {', '.join(self.on)}"
+        repr += f"\n\tdocuments: {len(self)}"
         return repr
 
+    @abc.abstractclassmethod
+    def __call__(
+        self,
+        q: typing.Union[typing.List[str], str],
+        k: typing.Optional[int],
+        batch_size: typing.Optional[int],
+        **kwargs,
+    ) -> typing.Union[
+        typing.List[typing.List[typing.Dict[str, str]]],
+        typing.List[typing.Dict[str, str]],
+    ]:
+        """Retrieve documents from the index."""
+        return []
+
+    def __len__(self):
+        return len(self.documents) if self.documents is not None else 0
+
     def __add__(self, other) -> Pipeline:
-        """Custom operator to make pipeline."""
+        """Pipeline operator."""
         if isinstance(other, Pipeline):
-            return Pipeline(models=other.models + [self])
-        else:
-            return Pipeline(models=[other, self])
-
-    def __or__(self) -> None:
-        """Or operator is only available on retrievers and rankers."""
-        raise NotImplementedError
-
-    def __and__(self) -> None:
-        """And operator is only available on retrievers and rankers."""
-        raise NotImplementedError
+            return Pipeline(self, other.models)
+        elif isinstance(other, list):
+            # Documents are part of the pipeline.
+            return Pipeline(
+                [self, {document[self.key]: document for document in other}]
+            )
+        return Pipeline([self, other])
+
+    def __or__(self, other) -> Union:
+        """Union operator."""
+        if isinstance(other, Union):
+            return Union([self] + other.models)
+        return Union([self, other])
+
+    def __and__(self, other) -> Intersection:
+        """Intersection operator."""
+        if isinstance(other, Intersection):
+            return Intersection([self] + other.models)
+        return Intersection([self, other])
+
+    def __mul__(self, other) -> Vote:
+        """Voting operator."""
+        if isinstance(other, Vote):
+            return Vote([self] + other.models)
+        return Vote([self, other])
```

### Comparing `cherche-1.0.1/cherche/index/tree.py` & `cherche-2.0.0/cherche/index/faiss_index.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,13 @@
-import faiss
+import typing
+
 import numpy as np
 
+from ..utils import yield_batch
+
 __all__ = ["Faiss"]
 
 
 class Faiss:
     """Faiss index dedicated to vector search.
 
     Parameters
@@ -12,130 +15,154 @@
     key
         Identifier field for each document.
     index
         Faiss index to use.
 
     Examples
     --------
+    >>> from pprint import pprint as print
     >>> from cherche import index
     >>> from sentence_transformers import SentenceTransformer
-    >>> from pprint import pprint as print
 
     >>> documents = [
-    ...    {"id": 0, "title": "Paris"},
-    ...    {"id": 1, "title": "Madrid"},
-    ...    {"id": 2, "title": "Paris"}
+    ...    {"id": 0, "title": "Paris France"},
+    ...    {"id": 1, "title": "Madrid Spain"},
+    ...    {"id": 2, "title": "Montreal Canada"}
     ... ]
 
     >>> encoder = SentenceTransformer("sentence-transformers/all-mpnet-base-v2")
 
     >>> faiss_index = index.Faiss(key="id")
     >>> faiss_index = faiss_index.add(
     ...    documents = documents,
     ...    embeddings = encoder.encode([document["title"] for document in documents]),
     ... )
 
-    >>> print(faiss_index(embedding = encoder.encode(["Spain"])))
-    [{'id': 1, 'similarity': 1.5076334135501044},
-     {'id': 2, 'similarity': 0.9021741164485997},
-     {'id': 0, 'similarity': 0.9021741164485997}]
+    >>> print(faiss_index(embeddings=encoder.encode(["Spain", "Montreal"])))
+    [[{'id': 1, 'similarity': 0.6544566197822951},
+      {'id': 0, 'similarity': 0.5405466290777285},
+      {'id': 2, 'similarity': 0.48717489472604614}],
+     [{'id': 2, 'similarity': 0.7372165680578416},
+      {'id': 0, 'similarity': 0.5185646665953703},
+      {'id': 1, 'similarity': 0.4834444940712032}]]
 
     >>> documents = [
-    ...    {"id": 3, "title": "Paris"},
-    ...    {"id": 4, "title": "Madrid"},
-    ...    {"id": 5, "title": "Paris"}
+    ...    {"id": 3, "title": "Paris France"},
+    ...    {"id": 4, "title": "Madrid Spain"},
+    ...    {"id": 5, "title": "Montreal Canada"}
     ... ]
 
     >>> faiss_index = faiss_index.add(
     ...    documents = documents,
     ...    embeddings = encoder.encode([document["title"] for document in documents]),
     ... )
 
-    >>> print(faiss_index(embedding = encoder.encode(["Spain"]), k=4))
-    [{'id': 1, 'similarity': 1.5076334135501044},
-     {'id': 4, 'similarity': 1.5076334135501044},
-     {'id': 2, 'similarity': 0.9021741164485997},
-     {'id': 3, 'similarity': 0.9021741164485997}]
+    >>> print(faiss_index(embeddings=encoder.encode(["Spain", "Montreal"]), k=4))
+    [[{'id': 1, 'similarity': 0.6544566197822951},
+      {'id': 4, 'similarity': 0.6544566197822951},
+      {'id': 0, 'similarity': 0.5405466290777285},
+      {'id': 3, 'similarity': 0.5405466290777285}],
+     [{'id': 2, 'similarity': 0.7372165680578416},
+      {'id': 5, 'similarity': 0.7372165680578416},
+      {'id': 0, 'similarity': 0.5185646665953703},
+      {'id': 3, 'similarity': 0.5185646665953703}]]
+
 
     References
     ----------
     1. [Faiss](https://github.com/facebookresearch/faiss)
 
     """
 
-    def __init__(self, key, index=None) -> None:
+    def __init__(self, key, index=None, normalize: bool = True) -> None:
+        import faiss
+
         self.key = key
         self.index = index
-        self.ids: dict = {}
-        self.documents: dict = {}
+        self.documents = []
+        self.normalize = normalize
 
     def __len__(self) -> int:
-        return len(self.ids)
+        return len(self.documents)
 
-    def _build(self, embeddings: np.ndarray) -> faiss.IndexFlatL2:
+    def _build(self, embeddings: np.ndarray):
         """Build faiss index.
 
         Parameters
         ----------
         index
             faiss index.
         embeddings
             Embeddings of the documents.
 
         """
-        array = np.array(embeddings).astype(np.float32)
-
-        if self.index is None and embeddings:
-            self.index = faiss.IndexFlatL2(array.shape[1])
+        if self.index is None:
+            try:
+                import faiss
+
+                self.index = faiss.IndexIDMap(faiss.IndexFlatIP(embeddings.shape[1]))
+            except:
+                raise ImportError(
+                    'Run pip install "cherche[cpu]" or pip install "cherche[gpu]" to run on GPU to install faiss.'
+                )
+            self.index = faiss.IndexFlatL2(embeddings.shape[1])
 
         if not self.index.is_trained and embeddings:
-            self.index.train(array)
-
-        if embeddings:
-            self.index.add(array)
+            self.index.train(embeddings)
 
+        self.index.add(embeddings)
         return self.index
 
     def add(self, documents: list, embeddings: np.ndarray) -> "Faiss":
         """Add documents to the faiss index and export embeddings if the path is provided.
         Streaming friendly.
 
         Parameters
         ----------
         documents
             List of documents as json or list of string to pre-compute queries embeddings.
 
         """
-        n = 0
-        index = len(self.documents)
         array = []
-
         for document, embedding in zip(documents, embeddings):
-            # Skip the document if its id already exist.
-            if document[self.key] in self.ids:
-                continue
-
-            self.documents[index + n] = {self.key: document[self.key]}
-            self.ids[document[self.key]] = True
+            self.documents.append({self.key: document[self.key]})
             array.append(embedding)
-            n += 1
 
-        self.index = self._build(embeddings=array)
+        embeddings = np.array(array)
+        if self.normalize:
+            embeddings = embeddings / np.linalg.norm(embeddings, axis=-1)[:, None]
+        self.index = self._build(embeddings=embeddings)
         return self
 
-    def __call__(self, embedding: np.ndarray, k: int = None, **kwargs) -> list:
+    def __call__(
+        self,
+        embeddings: np.ndarray,
+        k: typing.Optional[int] = None,
+    ) -> typing.Union[
+        typing.List[typing.List[typing.Dict[str, typing.Any]]],
+        typing.List[typing.Dict[str, typing.Any]],
+    ]:
         if k is None:
             k = len(self)
 
-        distances, indexes = self.index.search(embedding, k)
+        if self.normalize:
+            embeddings = embeddings / np.linalg.norm(embeddings, axis=-1)[:, None]
 
-        ranked = []
-        for idx, distance in zip(indexes[0], distances[0]):
+        distances, indexes = self.index.search(embeddings, k)
 
-            if idx < 0:
-                continue
+        # Filter -1 indexes
+        matchs = np.take(self.documents, np.where(indexes < 0, 0, indexes))
 
-            document = self.documents[idx]
-            document["similarity"] = float(1 / distance) if distance > 0 else 0.0
-            ranked.append(document)
+        rank = []
+        for distance, index, match in zip(distances, indexes, matchs):
+            rank.append(
+                [
+                    {
+                        **m,
+                        "similarity": 1 / (1 + d),
+                    }
+                    for d, idx, m in zip(distance, index, match)
+                    if idx > -1
+                ]
+            )
 
-        return ranked
+        return rank
```

### Comparing `cherche-1.0.1/cherche/query/base.py` & `cherche-2.0.0/cherche/query/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,16 +17,18 @@
         return "query"
 
     def __repr__(self) -> str:
         repr = f"Query {self.__class__.__name__}"
         return repr
 
     @abc.abstractmethod
-    def __call__(self, q: str, **kwargs) -> str:
-        return self
+    def __call__(
+        self, q: typing.Union[typing.List[str], str], **kwargs
+    ) -> typing.Union[typing.List[str], str]:
+        return []
 
     def __add__(self, other) -> Pipeline:
         """Pipeline operator."""
         if isinstance(other, Pipeline):
             return Pipeline(models=[self] + other.models)
         return Pipeline(models=[self, other])
```

### Comparing `cherche-1.0.1/cherche/query/norvig.py` & `cherche-2.0.0/cherche/query/norvig.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 import collections
 import pathlib
 import re
 import string
 import typing
 
+from ..utils import yield_batch_single
 from .base import Query
 
 __all__ = ["Norvig"]
 
 
 class Norvig(Query):
     """Spelling corrector written by Peter Norvig:
     [How to Write a Spelling Corrector](https://norvig.com/spell-correct.html)
 
     Parameters
     ----------
     on
         Fields to use for fitting the spelling corrector on.
-    big
-        Use the big.txt provided by the Norvig spelling corrector. Contains
-        english books from the Gutenberg project.
 
     Examples
     --------
 
     >>> from cherche import query, data
 
     >>> documents = data.load_towns()
@@ -33,54 +31,49 @@
     >>> corrector.add(documents)
     Query Norvig
          Vocabulary: 967
 
     >>> corrector(q="tha citi af Parisa is in Fronce")
     'the city of paris is in france'
 
-    >>> corrector = query.Norvig(big=True, on=["title", "article"], lower=False)
-
-    >>> corrector.add(documents)
-    Query Norvig
-         Vocabulary: 32790
-
-    >>> corrector(q="tha citi af Parisa is in Fronce")
-    'the city of Paris is in France'
+    >>> corrector(q=["tha citi af Parisa is in Fronce", "parisa"])
+    ['the city of paris is in france', 'paris']
 
     References
     ----------
     1. [How to Write a Spelling Corrector](https://norvig.com/spell-correct.html)
 
     """
 
     def __init__(
         self,
         on: typing.Union[str, typing.List],
         lower: bool = True,
-        big: bool = False,
     ) -> None:
         super().__init__(on=on)
 
         self.occurrences = collections.Counter()
         self.lower = lower
 
-        if big:
-            path_big = pathlib.Path(__file__).parent.parent.joinpath("data/norvig.txt")
-            self._update_from_file(path_file=path_big)
-
     def __repr__(self) -> str:
         repr = super().__repr__()
         repr += f"\n\t Vocabulary: {len(self.occurrences)}"
         return repr
 
-    def __call__(self, q: str, **kwargs) -> str:
+    def __call__(
+        self, q: typing.Union[typing.List[str], str], **kwargs
+    ) -> typing.Union[typing.List[str], str]:
         """Correct spelling errors in a given query."""
-        if len(self.occurrences) == 0:
-            return q
-        return " ".join(map(self.correct, q.split(" ")))
+        queries = []
+        for batch in yield_batch_single(q, desc="Spelling-correction"):
+            if len(self.occurrences) == 0:
+                queries.append(batch)
+            else:
+                queries.append(" ".join(map(self.correct, batch.split(" "))))
+        return queries[0] if isinstance(q, str) else queries
 
     def correct(self, word: str) -> float:
         """Most probable spelling correction for word."""
         return max(
             self._candidates(word),
             key=lambda w: self._probability(w.lower() if self.lower else w),
         )
```

### Comparing `cherche-1.0.1/cherche/query/prf.py` & `cherche-2.0.0/cherche/query/prf.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import typing
 
 import numpy as np
 import sklearn
 from sklearn.feature_extraction.text import TfidfVectorizer
 from sklearn.metrics.pairwise import cosine_similarity
 
+from ..utils import yield_batch_single
 from .base import Query
 
 __all__ = ["PRF"]
 
 
 class PRF(Query):
     """Pseudo (or blind) Relevance-Feedback module. The Query-Augmentation method applies a fast
@@ -31,25 +32,32 @@
     Examples
     --------
 
     >>> from cherche import query, data
 
     >>> documents = data.load_towns()
 
-    >>> prf = query.PRF(on=["title", "article"], nb_docs=8, nb_terms_per_doc=1, documents=documents)
+    >>> prf = query.PRF(
+    ...     on=["title", "article"],
+    ...     nb_docs=8, nb_terms_per_doc=1,
+    ...     documents=documents
+    ... )
 
     >>> prf
     Query PRF
-         On: title, article
-         Documents: 8
-         Terms: 1
+        on       : title, article
+        documents: 8
+        terms    : 1
 
     >>> prf(q="Europe")
     'Europe art metro space science bordeaux paris university significance'
 
+    >>> prf(q=["Europe", "Paris"])
+    ['Europe art metro space science bordeaux paris university significance', 'Paris received paris club subway billion source tour tournament']
+
     References
     ----------
     1. [Relevance feedback and pseudo relevance feedback](https://nlp.stanford.edu/IR-book/html/htmledition/relevance-feedback-and-pseudo-relevance-feedback-1.html)
     2. [Blind Feedback](https://en.wikipedia.org/wiki/Relevance_feedback#Blind_feedback)
 
     """
 
@@ -72,27 +80,33 @@
 
         self.tf = tf
         self.matrix = self.tf.fit_transform(documents)
         self.vocabulary = self.tf.get_feature_names_out()
 
     def __repr__(self) -> str:
         repr = super().__repr__()
-        repr += f"\n\t On: {', '.join(self.on)}"
-        repr += f"\n\t Documents: {self.nb_docs}"
-        repr += f"\n\t Terms: {self.nb_terms_per_doc}"
+        repr += f"\n\t on       : {', '.join(self.on)}"
+        repr += f"\n\t documents: {self.nb_docs}"
+        repr += f"\n\t terms    : {self.nb_terms_per_doc}"
         return repr
 
-    def __call__(self, q: str, **kwargs) -> str:
+    def __call__(
+        self, q: typing.Union[typing.List[str], str], **kwargs
+    ) -> typing.Union[typing.List[str], str]:
         """Augment a given query with new terms."""
         # Extract top terms from the documents wrt. a given query
-        top_terms = self._retrieve_top_terms(q=q)
-
-        # Augment the query
-        q += " " + " ".join([term for term in top_terms if term not in q.split(" ")])
-        return q
+        queries = []
+        for batch in yield_batch_single(q, desc="Query-augmentation"):
+            top_terms = self._retrieve_top_terms(q=batch)
+            # Augment the query
+            batch += " " + " ".join(
+                [term for term in top_terms if term not in batch.split(" ")]
+            )
+            queries.append(batch)
+        return queries[0] if isinstance(q, str) else queries
 
     def _retrieve_top_terms(self, q: str) -> typing.List[str]:
         """Retrieve new terms to augment a given query. Disregard dupes terms."""
         query = self.tf.transform([q])
         # First, retrieve top documents wrt. a given query
         idx_documents = self._retrieve_documents(matrix=self.matrix, query=query)
```

### Comparing `cherche-1.0.1/cherche/rank/encoder.py` & `cherche-2.0.0/cherche/rank/encoder.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,130 +1,134 @@
-from __future__ import annotations
-
 __all__ = ["Encoder"]
 
 import typing
 
-from ..similarity import cosine
 from .base import MemoryStore, Ranker
 
 
 class Encoder(Ranker):
-    """SentenceBert Ranker.
+    """Sentence Transformer as a ranker. This ranker is compatible with any SentenceTransformer.
 
     Parameters
     ----------
     key
         Field identifier of each document.
     on
-        Fields to use to match the query to the documents.
+        Fields on wich encoder will perform similarity matching.
     encoder
-        Encoding function dedicated to documents and query.
-    k
-        Number of documents to reorder. The default value is None, i.e. all documents will be
-        reordered and returned.
-    similarity
-        Similarity measure to compare documents embeddings and query embedding (similarity.cosine
-        or similarity.dot).
+        Encoding function dedicated to both documents and queries.
+    normalize
+        If set to True, the similarity measure is cosine similarity, if set to False, similarity
+        measure is dot product.
 
     Examples
     --------
-
     >>> from pprint import pprint as print
     >>> from cherche import rank
     >>> from sentence_transformers import SentenceTransformer
 
     >>> documents = [
-    ...    {"id": 0, "title": "Paris", "article": "This town is the capital of France", "author": "Wiki"},
-    ...    {"id": 1, "title": "Eiffel tower", "article": "Eiffel tower is based in Paris", "author": "Wiki"},
-    ...    {"id": 2, "title": "Montreal", "article": "Montreal is in Canada.", "author": "Wiki"},
+    ...    {"id": 0, "title": "Paris France"},
+    ...    {"id": 1, "title": "Madrid Spain"},
+    ...    {"id": 2, "title": "Montreal Canada"}
     ... ]
 
     >>> ranker = rank.Encoder(
     ...    encoder = SentenceTransformer("sentence-transformers/all-mpnet-base-v2").encode,
     ...    key = "id",
-    ...    on = ["title", "article"],
-    ...    k = 2,
+    ...    on = ["title"],
     ... )
 
     >>> ranker.add(documents=documents)
     Encoder ranker
-        key: id
-        on: title, article
-        k: 2
-        similarity: cosine
-        Embeddings pre-computed: 3
-
-    >>> print(ranker(q="Paris", documents=[{"id": 0}, {"id": 1}, {"id": 2}]))
-    [{'id': 0, 'similarity': 0.6605141758918762},
-     {'id': 1, 'similarity': 0.5142566561698914}]
-
-    >>> print(ranker(q="Paris", documents=documents))
-    [{'article': 'This town is the capital of France',
-      'author': 'Wiki',
-      'id': 0,
-      'similarity': 0.6605141758918762,
-      'title': 'Paris'},
-     {'article': 'Eiffel tower is based in Paris',
-      'author': 'Wiki',
-      'id': 1,
-      'similarity': 0.5142566561698914,
-      'title': 'Eiffel tower'}]
-
-
-    >>> ranker += documents
-
-    >>> print(ranker(q="Paris", documents=[{"id": 0}, {"id": 1}, {"id": 2}]))
-    [{'article': 'This town is the capital of France',
-      'author': 'Wiki',
-      'id': 0,
-      'similarity': 0.6605141758918762,
-      'title': 'Paris'},
-     {'article': 'Eiffel tower is based in Paris',
-      'author': 'Wiki',
-      'id': 1,
-      'similarity': 0.5142566561698914,
-      'title': 'Eiffel tower'}]
+        key       : id
+        on        : title
+        normalize : True
+        embeddings: 3
+
+    >>> match = ranker(
+    ...     q="Paris",
+    ...     documents=documents
+    ... )
+
+    >>> print(match)
+    [{'id': 0, 'similarity': 0.7127624, 'title': 'Paris France'},
+     {'id': 1, 'similarity': 0.5497405, 'title': 'Madrid Spain'},
+     {'id': 2, 'similarity': 0.50252455, 'title': 'Montreal Canada'}]
+
+    >>> match = ranker(
+    ...     q=["Paris France", "Madrid Spain"],
+    ...     documents=[documents + [{"id": 3, "title": "Paris"}]] * 2,
+    ...     k=2,
+    ... )
+
+    >>> print(match)
+    [[{'id': 0, 'similarity': 0.99999994, 'title': 'Paris France'},
+      {'id': 1, 'similarity': 0.856435, 'title': 'Madrid Spain'}],
+     [{'id': 1, 'similarity': 1.0, 'title': 'Madrid Spain'},
+      {'id': 0, 'similarity': 0.856435, 'title': 'Paris France'}]]
 
     """
 
     def __init__(
         self,
-        on: str | list,
+        on: typing.Union[str, typing.List[str]],
         key: str,
         encoder,
-        k: int | typing.Optionnal = None,
-        similarity=cosine,
-        store=MemoryStore(),
-        path: str | typing.Optionnal = None,
+        normalize: bool = True,
+        k: typing.Optional[int] = None,
+        batch_size: int = 64,
     ) -> None:
         super().__init__(
             key=key,
             on=on,
             encoder=encoder,
+            normalize=normalize,
             k=k,
-            similarity=similarity,
-            store=store,
+            batch_size=batch_size,
         )
 
-    def __call__(self, q: str, documents: list, **kwargs) -> list:
+    def __call__(
+        self,
+        q: typing.Union[typing.List[str], str],
+        documents: typing.Union[
+            typing.List[typing.List[typing.Dict[str, str]]],
+            typing.List[typing.Dict[str, str]],
+        ],
+        k: typing.Optional[int] = None,
+        batch_size: typing.Optional[int] = None,
+        **kwargs
+    ) -> typing.Union[
+        typing.List[typing.List[typing.Dict[str, str]]],
+        typing.List[typing.Dict[str, str]],
+    ]:
         """Encode input query and ranks documents based on the similarity between the query and
         the selected field of the documents.
 
-        https://pymilvus.readthedocs.io/en/latest/tutorial.html
-        status, documents = client.get_entity_by_id(collection_name, [id_1, id_2])
-
         Parameters
         ----------
         q
             Input query.
         documents
             List of documents to rank.
 
         """
-        if not documents:
+        if k is None:
+            k = self.k
+
+        if k is None:
+            k = len(self)
+
+        if not documents and isinstance(q, str):
             return []
 
-        return self.rank(
-            query_embedding=self.encoder(q),
-            documents=documents,
+        if not documents and isinstance(q, list):
+            return [[]]
+
+        rank = self.encode_rank(
+            embeddings_queries=self.encoder([q] if isinstance(q, str) else q),
+            documents=[documents] if isinstance(q, str) else documents,
+            k=k,
+            batch_size=batch_size if batch_size is not None else self.batch_size,
         )
+
+        return rank[0] if isinstance(q, str) else rank
```

### Comparing `cherche-1.0.1/cherche/rank/recommend.py` & `cherche-2.0.0/cherche/rank/embedding.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,236 +1,178 @@
 from __future__ import annotations
 
 import typing
 
 import numpy as np
 
-from ..index import Milvus
-from ..similarity import cosine
 from .base import MemoryStore, Ranker
 
-__all__ = ["Recommend"]
+__all__ = ["Embedding"]
 
 
-class Recommend(Ranker):
+class Embedding(Ranker):
     """Collaborative filtering as a ranker. Recommend is compatible with the library [Implicit](https://github.com/benfred/implicit).
 
     Parameters
     ----------
     key
         Field identifier of each document.
-    k
-        Number of documents to retrieve. Default is `None`, i.e all documents that match the query
-        will be retrieved.
-    index
-        Index that will store the embeddings of documents and perform the similarity search.
-        The default index is Faiss. We can choose index.Milvus also.
-    store
-        Index that will store the embeddings of users. By default, it store users embeddings in
-        memory. We can choose index.Milvus also.
+    normalize
+        If set to True, the similarity measure is cosine similarity, if set to False, similarity
+        measure is dot product.
 
     Examples
     --------
-
     >>> from pprint import pprint as print
-    >>> from cherche import rank, utils
-    >>> from implicit.nearest_neighbours import bm25_weight
-    >>> from implicit.als import AlternatingLeastSquares
+    >>> from cherche import rank
+    >>> from sentence_transformers import SentenceTransformer
 
     >>> documents = [
-    ...    {"id": "a", "title": "Paris", "author": "Paris"},
-    ...    {"id": "b", "title": "Madrid", "author": "Madrid"},
-    ...    {"id": "c", "title": "Montreal", "author": "Montreal"},
+    ...    {"id": "a", "title": "Paris"},
+    ...    {"id": "b", "title": "Madrid"},
+    ...    {"id": "c", "title": "Montreal"},
     ... ]
 
-    >>> ratings = {
-    ...    "Max": {"a": 1, "c": 1},
-    ...    "Adil": {"b": 1, "d": 2},
-    ...    "Robin": {"b": 1, "d": 1},
-    ...    "Geoffrey": {"a": 1, "c": 1},
-    ... }
-
-    >>> index_users, index_documents, sparse_ratings = utils.users_items_sparse(ratings=ratings)
-
-    >>> model = AlternatingLeastSquares(
-    ...     factors=64,
-    ...     regularization=0.05,
-    ...     alpha=2.0,
-    ...     iterations=100,
-    ...     random_state=42,
-    ... )
-
-    >>> model.fit(sparse_ratings)
+    >>> encoder = SentenceTransformer("sentence-transformers/all-mpnet-base-v2")
+    >>> embeddings_documents = encoder.encode([
+    ...    document["title"] for document in documents
+    ... ])
 
-    >>> embeddings_users = {
-    ...    user: embedding for user, embedding in zip(index_users, model.user_factors)
-    ... }
-
-    >>> embeddings_documents = {
-    ...    document: embedding
-    ...    for document, embedding in zip(index_documents, model.item_factors)
-    ... }
-
-    >>> recommend = rank.Recommend(
+    >>> recommend = rank.Embedding(
     ...    key="id",
-    ...    k = 10,
     ... )
 
     >>> recommend.add(
     ...    documents=documents,
     ...    embeddings_documents=embeddings_documents,
-    ...    embeddings_users=embeddings_users,
     ... )
-    Recommend ranker
-        key: id
-        Users: 4
-        Documents: 3
-
-    >>> print(recommend(user="Geoffrey", documents=documents))
-    [{'author': 'Paris',
-      'id': 'a',
-      'similarity': 1.0000001192092896,
-      'title': 'Paris'},
-     {'author': 'Montreal',
-      'id': 'c',
-      'similarity': 0.9999998807907104,
-      'title': 'Montreal'},
-     {'author': 'Madrid',
-      'id': 'b',
-      'similarity': 4.273452987035853e-07,
-      'title': 'Madrid'}]
-
-    >>> recommend(user="Geoffrey", documents=[{"id": "unknown", "title": "unknown", "author": "unknown"}])
-    [{'id': 'unknown', 'title': 'unknown', 'author': 'unknown', 'similarity': 0}]
-
-    >>> print(recommend(user="unknown", documents=documents))
-    [{'author': 'Paris', 'id': 'a', 'similarity': 0, 'title': 'Paris'},
-     {'author': 'Madrid', 'id': 'b', 'similarity': 0, 'title': 'Madrid'},
-     {'author': 'Montreal', 'id': 'c', 'similarity': 0, 'title': 'Montreal'}]
+    Embedding ranker
+        key      : id
+        documents: 3
+        normalize: True
+
+    >>> match = recommend(
+    ...     q=encoder.encode("Paris"),
+    ...     documents=documents,
+    ...     k=2
+    ... )
 
-    References
-    ----------
-    1. [Implicit](https://github.com/benfred/implicit)
-    2. [Implicit documentation](https://benfred.github.io/implicit/)
-    3. [Logistic Matrix Factorization for Implicit Feedback Data](https://web.stanford.edu/~rezab/nips2014workshop/submits/logmat.pdf)
-    4. [BPR: Bayesian Personalized Ranking from Implicit Feedback](https://arxiv.org/pdf/1205.2618.pdf)
-    5. [Collaborative Filtering for Implicit Feedback Datasets](http://yifanhu.net/PUB/cf.pdf)
+    >>> print(match)
+    [{'id': 'a', 'similarity': 1.0, 'title': 'Paris'},
+     {'id': 'c', 'similarity': 0.57165134, 'title': 'Montreal'}]
+
+    >>> queries = [
+    ...    "Paris",
+    ...    "Madrid",
+    ...    "Montreal"
+    ... ]
+
+    >>> match = recommend(
+    ...     q=encoder.encode(queries),
+    ...     documents=[documents] * 3,
+    ...     k=2
+    ... )
+
+    >>> print(match)
+    [[{'id': 'a', 'similarity': 1.0, 'title': 'Paris'},
+      {'id': 'c', 'similarity': 0.57165134, 'title': 'Montreal'}],
+     [{'id': 'b', 'similarity': 1.0, 'title': 'Madrid'},
+      {'id': 'a', 'similarity': 0.49815434, 'title': 'Paris'}],
+     [{'id': 'c', 'similarity': 0.9999999, 'title': 'Montreal'},
+      {'id': 'a', 'similarity': 0.5716514, 'title': 'Paris'}]]
 
     """
 
     def __init__(
         self,
         key: str,
-        k: int = None,
-        similarity=cosine,
-        store_items=MemoryStore(),
-        store_users=MemoryStore(),
+        normalize: bool = True,
+        k: typing.Optional[int] = None,
+        batch_size: int = 1024,
     ) -> None:
         super().__init__(
             key=key,
             on="",
             encoder=None,
+            normalize=normalize,
             k=k,
-            similarity=similarity,
-            store=store_items,
+            batch_size=batch_size,
         )
 
-        self.store_users = store_users
-
     def __repr__(self) -> str:
         repr = f"{self.__class__.__name__} ranker"
-        repr += f"\n \t key: {self.key}"
-        repr += f"\n \t Users: {len(self.store_users)}"
-        repr += f"\n \t Documents: {len(self.store)}"
+        repr += f"\n\tkey      : {self.key}"
+        repr += f"\n\tdocuments: {len(self)}"
+        repr += f"\n\tnormalize: {self.normalize}"
         return repr
 
     def add(
         self,
         documents: list,
-        embeddings_documents: dict,
-        embeddings_users: dict,
+        embeddings_documents: typing.List[np.ndarray],
         **kwargs,
-    ) -> "Recommend":
+    ) -> "Embedding":
         """Add embeddings both documents and users.
 
         Parameters
         ----------
         documents
             List of documents.
         embeddings_documents
             Embeddings of the documents ordered as the list of documents.
         users
             List of users.
         embeddings_users
             Embeddings of the users ordered as the list of users.
 
         """
-        index = {document[self.key]: document for document in documents}
-
         self.store.add(
-            documents=[
-                index[key] for key in embeddings_documents.keys() if key in index
-            ],
-            embeddings=np.array(
-                [
-                    embedding
-                    for key, embedding in embeddings_documents.items()
-                    if key in index
-                ]
-            ),
+            documents=documents,
+            embeddings=embeddings_documents,
             key=self.key,
         )
 
-        self.store_users.add(
-            users=[key for key in embeddings_users.keys()],
-            embeddings=[embedding for embedding in embeddings_users.values()],
-        )
         return self
 
     def __call__(
         self,
-        user: typing.Union[str, int],
-        documents: list,
-        expr: str = None,
-        consistency_level: str = None,
-        partition_names: list = None,
+        q: np.ndarray,
+        documents: typing.Union[
+            typing.List[typing.List[typing.Dict[str, str]]],
+            typing.List[typing.Dict[str, str]],
+        ],
+        k: typing.Optional[int] = None,
+        batch_size: typing.Optional[int] = None,
         **kwargs,
-    ) -> list:
+    ) -> typing.Union[
+        typing.List[typing.List[typing.Dict[str, str]]],
+        typing.List[typing.Dict[str, str]],
+    ]:
         """Retrieve documents from user id.
 
         Parameters
         ----------
         user
             User id.
         documents
             List of documents to rank.
         """
-        known_user, embedding_user, unknown_user = self.store_users.get(values=[user])
+        if k is None:
+            k = self.k
+
+        if k is None:
+            k = len(self)
 
-        # Unknown user.
-        if not known_user:
-            return [{**document, "similarity": 0} for document in documents]
-
-        known, embeddings, unknown = self.store.get(
-            **{
-                "key": self.key,
-                "values": [document[self.key] for document in documents],
-            }
+        documents = [documents] if len(q.shape) == 1 else documents
+        known, embeddings, _ = self.store.get(documents=documents)
+
+        ranked = self.rank(
+            embeddings_queries=q,
+            embeddings_documents={
+                key: embedding for key, embedding in zip(known, embeddings)
+            },
+            documents=documents,
+            k=k,
+            batch_size=batch_size if batch_size is not None else self.batch_size,
         )
 
-        # Unknown documents.
-        if not known:
-            return [{**document, "similarity": 0} for document in documents]
-
-        index = {document[self.key]: document for document in documents}
-        index_known = {i: key  for i, key in enumerate(known)}
-
-        ranked = [
-            {**index[index_known[key]], "similarity": similarity}
-            for key, similarity in self.similarity(
-                emb_q=embedding_user[0], emb_documents=embeddings
-            )
-        ]
-
-        # Addind unknown documents
-        ranked += [{**index[key], "similarity": 0} for key in unknown]
-        return ranked[:self.k] if self.k is not None else ranked
+        return ranked[0] if len(q.shape) == 1 else ranked
```

### Comparing `cherche-1.0.1/cherche/rank/test_rank.py` & `cherche-2.0.0/cherche/rank/test_rank.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,46 +1,37 @@
 import pytest
-from cherche.rank.zero_shot import ZeroShot
 
 from .. import rank
 
 
-def cherche_rankers(key: str, on: str, k: int = None):
+def cherche_rankers(key: str, on: str):
     """List of rankers available in cherche."""
-    from sentence_transformers import SentenceTransformer
-    from transformers import pipeline
+    from sentence_transformers import CrossEncoder, SentenceTransformer
 
     yield from [
         rank.DPR(
             key=key,
             on=on,
             encoder=SentenceTransformer(
                 "facebook-dpr-ctx_encoder-single-nq-base"
             ).encode,
             query_encoder=SentenceTransformer(
                 "facebook-dpr-question_encoder-single-nq-base"
             ).encode,
-            k=k,
         ),
         rank.Encoder(
             key=key,
             on=on,
             encoder=SentenceTransformer(
                 "sentence-transformers/all-mpnet-base-v2"
             ).encode,
-            k=k,
         ),
-        rank.ZeroShot(
-            key=key,
+        rank.CrossEncoder(
             on=on,
-            encoder=pipeline(
-                "zero-shot-classification",
-                model="typeform/distilbert-base-uncased-mnli",
-            ),
-            k=k,
+            encoder=CrossEncoder("cross-encoder/mmarco-mMiniLMv2-L12-H384-v1").predict,
         ),
     ]
 
 
 def documents():
     return [
         {
@@ -57,61 +48,90 @@
             "title": "Montreal",
             "article": "Montreal is in Canada.",
             "author": "Wikipedia",
         },
     ]
 
 
+def missing_documents():
+    return []
+
+
 @pytest.mark.parametrize(
     "ranker, documents, key, k",
     [
         pytest.param(
             ranker,
             documents(),
             "title",
             k,
             id=f"Ranker: {ranker.__class__.__name__}, k: {k}",
         )
-        for k in [None, 0, 2, 4]
-        for ranker in cherche_rankers(key="title", on="article", k=k)
+        for k in [None, 2, 4]
+        for ranker in cherche_rankers(key="title", on="article")
     ],
 )
 def test_ranker(ranker, documents: list, key: str, k: int):
     """Test ranker. Test if the number of ranked documents is coherent.
     Check for empty retrieved documents should returns an empty list.
     """
-    if not isinstance(ranker, ZeroShot):
+    if not isinstance(ranker, rank.CrossEncoder):
         ranker.add(documents)
 
-    # Zero shot needs all the fields
-    if not isinstance(ranker, ZeroShot):
+    # CrossEncoder shot needs all the fields
+    if not isinstance(ranker, rank.CrossEncoder):
         ranker += documents
         # Convert inputs document to a list of id [{"id": 0}, {"id": 1}, {"id": 2}]
         documents = [{key: document[key]} for document in documents]
 
-    answers = ranker(q="Eiffel tower France", documents=documents)
+    answers = ranker(q="Eiffel tower France", documents=documents, k=k)
 
     if k is not None:
         assert len(answers) == min(k, len(documents))
     else:
         assert len(answers) == len(documents)
 
     for index, sample in enumerate(answers):
-
         for key in ["title", "article", "author"]:
             assert key in sample
 
         if index == 0:
             assert sample["title"] == "Eiffel tower"
 
-    answers = ranker(q="Canada", documents=documents)
+    answers = ranker(q="Canada", documents=documents, k=k)
 
     if k is None:
         assert answers[0]["title"] == "Montreal"
     elif k >= 1:
         assert answers[0]["title"] == "Montreal"
     else:
         assert len(answers) == 0
 
     # Unknown token.
-    answers = ranker(q="Paris", documents=[])
+    answers = ranker(q="Paris", documents=[], k=k)
     assert len(answers) == 0
+
+
+@pytest.mark.parametrize(
+    "ranker, documents, key, k",
+    [
+        pytest.param(
+            ranker,
+            missing_documents(),
+            "title",
+            5,
+            id=f"Ranker: {ranker.__class__.__name__}, missing documents, k: 5",
+        )
+        for ranker in cherche_rankers(key="title", on="article")
+    ],
+)
+def test_ranker_missing_documents(ranker, documents: list, key: str, k: int):
+    """Test ranker when retriever do not returns any documents."""
+    answers = ranker(q="Eiffel tower France", documents=documents, k=k)
+    assert len(answers) == 0
+
+    answers = ranker(
+        q=["Eiffel tower France", "Montreal Canada"],
+        documents=[documents, documents],
+        k=k,
+    )
+    assert len(answers) == 2 and len(answers[0]) == 0 and len(answers[1]) == 0
```

### Comparing `cherche-1.0.1/cherche/rank/zero_shot.py` & `cherche-2.0.0/cherche/retrieve/flash.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,153 +1,154 @@
-from __future__ import annotations
-
-__all__ = ["ZeroShot"]
+__all__ = ["Flash"]
 
+import collections
 import typing
+from itertools import chain
+
+from flashtext import KeywordProcessor
 
-from ..compose import Intersection, Pipeline, Union, Vote
+from ..utils import yield_batch_single
+from .base import Retriever
 
 
-class ZeroShot:
-    """ZeroShot classifier for ranking. Zero shot does not pre-compute embeddings, it needs the
-    fields to rank the input documents.
+class Flash(Retriever):
+    """FlashText Retriever. Flash aims to find documents that contain keywords such as a list of
+    tags for example.
 
     Parameters
     ----------
+    key
+        Field identifier of each document.
     on
         Fields to use to match the query to the documents.
-    encoder
-        Zero shot classifier to use for ranking
-    k
-        Number of documents to reorder. The default value is None, i.e. all documents will be
-        reordered and returned.
-    multi_class
-        If more than one candidate label can be correct, pass multi_class=True to calculate each
-        class independently.
+    keywords
+        Keywords extractor from [FlashText](https://github.com/vi3k6i5/flashtext). If set to None,
+        a default one is created.
 
     Examples
     --------
-
     >>> from pprint import pprint as print
-    >>> from cherche import rank
-    >>> from transformers import pipeline
-    >>> from sentence_transformers import SentenceTransformer
+    >>> from cherche import retrieve
 
     >>> documents = [
-    ...    {"id": 0, "title": "Paris", "article": "This town is the capital of France", "author": "Wiki"},
-    ...    {"id": 1, "title": "Eiffel tower", "article": "Eiffel tower is based in Paris", "author": "Wiki"},
-    ...    {"id": 2, "title": "Montreal", "article": "Montreal is in Canada.", "author": "Wiki"},
+    ...     {"id": 0, "title": "paris", "article": "eiffel tower"},
+    ...     {"id": 1, "title": "paris", "article": "paris"},
+    ...     {"id": 2, "title": "montreal", "article": "montreal is in canada"},
     ... ]
 
-    >>> ranker = rank.ZeroShot(
-    ...     key = "id",
-    ...     on = ["title", "article"],
-    ...     encoder = pipeline("zero-shot-classification", model="typeform/distilbert-base-uncased-mnli"),
-    ...     k = 2,
-    ... )
-
-    >>> ranker
-    Zero Shot Classifier
-        key: id
-        on: title, article
-        k: 2
-        multi class: True
-
-    >>> print(ranker(q="Paris", documents=documents))
-    [{'article': 'This town is the capital of France',
-      'author': 'Wiki',
-      'id': 0,
-      'similarity': 0.44725653529167175,
-      'title': 'Paris'},
-     {'article': 'Eiffel tower is based in Paris',
-      'author': 'Wiki',
-      'id': 1,
-      'similarity': 0.31512802839279175,
-      'title': 'Eiffel tower'}]
+    >>> retriever = retrieve.Flash(key="id", on=["title", "article"])
 
+    >>> retriever.add(documents=documents)
+    Flash retriever
+        key      : id
+        on       : title, article
+        documents: 4
+
+    >>> print(retriever(q="paris", k=2))
+    [{'id': 1, 'similarity': 0.6666666666666666},
+     {'id': 0, 'similarity': 0.3333333333333333}]
+
+    [{'id': 0, 'similarity': 1}, {'id': 1, 'similarity': 1}]
+
+    >>> print(retriever(q=["paris", "montreal"]))
+    [[{'id': 1, 'similarity': 0.6666666666666666},
+      {'id': 0, 'similarity': 0.3333333333333333}],
+     [{'id': 2, 'similarity': 1.0}]]
 
     References
     ----------
-    1. [New pipeline for zero-shot text classification](https://discuss.huggingface.co/t/new-pipeline-for-zero-shot-text-classification/681)
-    2. [NLI models](https://huggingface.co/models?pipeline_tag=zero-shot-classification&sort=downloads)
+    1. [FlashText](https://github.com/vi3k6i5/flashtext)
+    2. [Replace or Retrieve Keywords In Documents at Scale](https://arxiv.org/abs/1711.00046)
 
     """
 
     def __init__(
         self,
         key: str,
-        on: str | list,
-        encoder,
-        k: int | typing.Optionnal = None,
-        multi_class: bool = True,
-    ):
-        self.key = key
-        self.on = on if isinstance(on, list) else [on]
-        self.encoder = encoder
-        self.k = k
-        self.multi_class = multi_class
-
-    def __repr__(self) -> str:
-        repr = "Zero Shot Classifier"
-        repr += f"\n\t key: {self.key}"
-        repr += f"\n\t on: {', '.join(self.on)}"
-        repr += f"\n\t k: {self.k}"
-        repr += f"\n\t multi class: {self.multi_class}"
-        return repr
+        on: typing.Union[str, list],
+        keywords: KeywordProcessor = None,
+        lowercase: bool = True,
+        k: typing.Optional[int] = None,
+    ) -> None:
+        super().__init__(key=key, on=on, k=k, batch_size=1)
+        self.documents = collections.defaultdict(list)
+        self.keywords = KeywordProcessor() if keywords is None else keywords
+        self.lowercase = lowercase
 
-    def __call__(self, q: str, documents: list, **kwargs) -> list:
-        """Rank inputs documents based on query.
+    def add(self, documents: typing.List[typing.Dict[str, str]], **kwargs) -> "Flash":
+        """Add keywords to the retriever.
 
         Parameters
         ----------
-        q
-            Inputs query.
         documents
-            List of documents to rank.
+            List of documents to add to the retriever.
+
+        """
+        for document in documents:
+            for field in self.on:
+                if field not in document:
+                    continue
+
+                if isinstance(document[field], str):
+                    words = document[field]
+                    if self.lowercase:
+                        words = words.lower()
+                    self.documents[words].append({self.key: document[self.key]})
+                    self.keywords.add_keyword(words)
+
+                elif isinstance(document[field], list):
+                    words = document[field]
+                    if self.lowercase:
+                        words = [word.lower() for word in words]
+
+                    for word in words:
+                        self.documents[word].append({self.key: document[self.key]})
+                    self.keywords.add_keywords_from_list(words)
+
+        return self
 
+    def __call__(
+        self,
+        q: typing.Union[typing.List[str], str],
+        k: typing.Optional[int] = None,
+        **kwargs,
+    ) -> list:
+        """Retrieve documents from the index.
+
+        Parameters
+        ----------
+        q
+            Either a single query or a list of queries.
+        k
+            Number of documents to retrieve. Default is `None`, i.e all documents that match the
+            query will be retrieved.
         """
-        if not documents:
-            return []
+        rank = []
+
+        for batch in yield_batch_single(q, desc=f"{self.__class__.__name__} retriever"):
+            if self.lowercase:
+                batch = batch.lower()
+
+            match = list(
+                chain.from_iterable(
+                    [
+                        self.documents[tag]
+                        for tag in self.keywords.extract_keywords(batch)
+                    ]
+                )
+            )
+
+            scores = collections.defaultdict(int)
+            for document in match:
+                scores[document[self.key]] += 1
+
+            total = len(match)
+
+            documents = [
+                {self.key: key, "similarity": scores[key] / total}
+                for key in sorted(scores, key=scores.get, reverse=True)
+            ]
+
+            documents = documents[:k] if k is not None else documents
+            rank.append(documents)
 
-        scores = self.encoder(
-            q,
-            [
-                " ".join([document.get(field, "") for field in self.on])
-                for document in documents
-            ],
-            multi_label=self.multi_class,
-        )
-
-        ranked = []
-        for label, score in zip(scores["labels"], scores["scores"]):
-            for document in documents:
-                content = " ".join([document.get(field, "") for field in self.on])
-                if content == label:
-                    ranked.append(document)
-                    document.update({"similarity": score})
-                    break
-        return ranked[: self.k] if self.k is not None else ranked
-
-    def __add__(self, other) -> Pipeline:
-        """Custom operator to make pipeline."""
-        if isinstance(other, Pipeline):
-            return other + self
-        else:
-            return Pipeline(models=[other, self])
-
-    def __or__(self, other) -> Union:
-        """Union operator."""
-        if isinstance(other, Union):
-            return Union([self] + other.models)
-        return Union([self, other])
-
-    def __and__(self, other) -> Intersection:
-        """Intersection operator."""
-        if isinstance(other, Intersection):
-            return Intersection([self] + other.models)
-        return Intersection([self, other])
-
-    def __mul__(self, other) -> Vote:
-        """Voting operator."""
-        if isinstance(other, Vote):
-            return Vote([self] + other.models)
-        return Vote([self, other])
+        return rank[0] if isinstance(q, str) else rank
```

### Comparing `cherche-1.0.1/cherche/retrieve/elastic.py` & `cherche-2.0.0/cherche/retrieve/encoder.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,148 +1,159 @@
-__all__ = ["Elastic"]
+__all__ = ["Encoder"]
 
 import typing
 
-import more_itertools
 import tqdm
-from elasticsearch import Elasticsearch, helpers
 
+from ..index import Faiss
+from ..utils import yield_batch
 from .base import Retriever
 
 
-class Elastic(Retriever):
-    """ElasticSearch retriever based on the [Python client of Elasticsearch](https://elasticsearch-py.readthedocs.io/en/v7.15.1/).
+class Encoder(Retriever):
+    """Encoder as a retriever using Faiss Index.
 
     Parameters
     ----------
+    key
+        Field identifier of each document.
     on
-        Fields to use to match the query to the documents.
-    k
-        Number of documents to retrieve. Default is `None`, i.e all documents that match the query
-         will be retrieved.
-    es
-        ElasticSearch Python client. The default configuration is used if set to None.
+        Field to use to retrieve documents.
     index
-        Elasticsearch index to use to index documents. Elastic will create the index if it does not
-        exist.
+        Faiss index that will store the embeddings and perform the similarity search.
+    normalize
+        Whether to normalize the embeddings before adding them to the index in order to measure
+        cosine similarity.
 
     Examples
     --------
-
     >>> from pprint import pprint as print
-    >>> from elasticsearch import Elasticsearch
-    >>> from cherche import retrieve, rank
+    >>> from cherche import retrieve
     >>> from sentence_transformers import SentenceTransformer
 
-    >>> es = Elasticsearch(hosts="http://localhost:9200")
-
-    >>> if es.ping():
-    ...    retriever = retrieve.Elastic(key="id", on=["title", "author"], k=2, es=es, index="test")
-    ...
-    ...    documents = [
-    ...         {"id": 0, "title": "Paris", "author": "Wiki"},
-    ...         {"id": 1, "title": "Eiffel tower", "author": "Wiki"},
-    ...         {"id": 2, "title": "Montreal", "author": "Wiki"},
-    ...    ]
-    ...
-    ...    retriever = retriever.add(documents=documents)
-    ...    candidates = retriever(q="paris")
-
-    References
-    ----------
-    1. [Python Elasticsearch Client](https://elasticsearch-py.readthedocs.io/en/v7.15.1/)
+    >>> documents = [
+    ...    {"id": 0, "title": "Paris France"},
+    ...    {"id": 1, "title": "Madrid Spain"},
+    ...    {"id": 2, "title": "Montreal Canada"}
+    ... ]
+
+    >>> retriever = retrieve.Encoder(
+    ...    encoder = SentenceTransformer("sentence-transformers/all-mpnet-base-v2").encode,
+    ...    key = "id",
+    ...    on = ["title"],
+    ... )
+
+    >>> retriever.add(documents, batch_size=1)
+    Encoder retriever
+        key      : id
+        on       : title
+        documents: 3
+
+    >>> print(retriever("Spain", k=2))
+    [{'id': 1, 'similarity': 0.6544566453117681},
+     {'id': 0, 'similarity': 0.5405465419981407}]
+
+    >>> print(retriever(["Spain", "Montreal"], k=2))
+    [[{'id': 1, 'similarity': 0.6544566453117681},
+      {'id': 0, 'similarity': 0.54054659424589}],
+     [{'id': 2, 'similarity': 0.7372165680578416},
+      {'id': 0, 'similarity': 0.5185645704259234}]]
 
     """
 
     def __init__(
         self,
+        encoder,
         key: str,
         on: typing.Union[str, list],
-        k: int = None,
-        es: Elasticsearch = None,
-        index: str = "cherche",
+        normalize: bool = True,
+        k: typing.Optional[int] = None,
+        batch_size: int = 64,
+        index=None,
     ) -> None:
-        self.key = key
-        self.on = on if isinstance(on, list) else [on]
-        self.k = k
-        self.es = Elasticsearch() if es is None else es
-        self.index = index
+        super().__init__(
+            key=key,
+            on=on,
+            k=k,
+            batch_size=batch_size,
+        )
+        self.encoder = encoder
 
-        if not self.es.indices.exists(index=self.index):
-            self.es.indices.create(index=self.index)
+        if index is None:
+            self.index = Faiss(key=self.key, normalize=normalize)
+        else:
+            self.index = Faiss(key=self.key, index=index, normalize=normalize)
 
     def __len__(self) -> int:
-        return int(self.es.cat.count(self.index, params={"format": "json"})[0]["count"])
+        return len(self.index)
 
-    def add(self, documents: list, batch_size=128, **kwargs) -> "Elastic":
-        """ElasticSearch bulk indexing.
+    def add(
+        self,
+        documents: typing.List[typing.Dict[str, str]],
+        batch_size: int = 64,
+        **kwargs,
+    ) -> "Encoder":
+        """Add documents to the index.
 
         Parameters
         ----------
         documents
-            List of documents to upload to Elasticsearch.
-
+            List of documents to add to the index.
+        batch_size
+            Number of documents to encode at once.
         """
-        documents = [
-            {
-                "_id": doc[self.key],
-                "_index": self.index,
-                "_source": doc,
-            }
-            for doc in documents
-        ]
-
-        for batch in tqdm.tqdm(
-            more_itertools.chunked(documents, batch_size),
-            position=0,
-            desc="Elasticsearch indexing.",
-            total=1 + len(documents) // batch_size,
-        ):
 
-            helpers.bulk(self.es, batch)
-            self.es.indices.refresh(index=self.index)
+        for batch in yield_batch(
+            array=documents,
+            batch_size=batch_size,
+            desc=f"{self.__class__.__name__} index creation",
+        ):
+            self.index.add(
+                documents=batch,
+                embeddings=self.encoder(
+                    [
+                        " ".join([document.get(field, "") for field in self.on])
+                        for document in batch
+                    ]
+                ),
+            )
 
         return self
 
-    def __call__(self, q: str, query: str = None, **kwargs) -> list:
-        """ElasticSearch query.
+    def __call__(
+        self,
+        q: typing.Union[typing.List[str], str],
+        k: typing.Optional[int] = None,
+        batch_size: typing.Optional[int] = None,
+        **kwargs,
+    ) -> typing.Union[
+        typing.List[typing.List[typing.Dict[str, str]]],
+        typing.List[typing.Dict[str, str]],
+    ]:
+        """Retrieve documents from the index.
 
         Parameters
         ----------
-
-            q: User query.
-            query: Custom ElasticSearch query.
-
+        q
+            Either a single query or a list of queries.
+        k
+            Number of documents to retrieve. Default is `None`, i.e all documents that match the
+            query will be retrieved.
+        batch_size
+            Number of queries to encode at once.
         """
-        if query is None:
-            query = {
-                "query": {
-                    "multi_match": {
-                        "query": q,
-                        "type": "most_fields",
-                        "fields": self.on,
-                        "operator": "or",
-                    }
-                },
-            }
-
-        if self.k is not None:
-            query["size"] = self.k
-
-        documents = self.es.search(
-            index=self.index,
-            body=query,
-        )
+        k = k if k is not None else len(self)
 
-        ranked = []
-        for document in documents["hits"]["hits"]:
-            document = {**document["_source"], "similarity": float(document["_score"])}
-            ranked.append(document)
-
-        return ranked
-
-    def reset(self) -> "Elastic":
-        """Delete the selected index from ElasticSearch."""
-        if self.es.indices.exists(index=self.index):
-            self.es.delete_by_query(index=self.index, body={"query": {"match_all": {}}})
-            self.es.indices.refresh(index=self.index)
-        return self
+        rank = []
+        for batch in yield_batch(
+            array=q,
+            batch_size=batch_size if batch_size is not None else self.batch_size,
+            desc=f"{self.__class__.__name__} retriever",
+        ):
+            rank.extend(
+                self.index(
+                    embeddings=self.encoder(batch),
+                    k=k,
+                )
+            )
+
+        return rank[0] if isinstance(q, str) else rank
```

### Comparing `cherche-1.0.1/cherche/retrieve/flash.py` & `cherche-2.0.0/cherche/retrieve/embedding.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,132 +1,163 @@
-__all__ = ["Flash"]
-
-import collections
 import typing
-from itertools import chain
 
-from flashtext import KeywordProcessor
+import numpy as np
 
+from ..index import Faiss
+from ..utils import yield_batch
 from .base import Retriever
 
+__all__ = ["Embedding"]
+
 
-class Flash(Retriever):
-    """FlashText Retriever. Flash aims to find documents that contain keywords such as a list of
-    tags for example.
+class Embedding(Retriever):
+    """The Embedding retriever is dedicated to perform IR on embeddings calculated by the user
+    rather than Cherche.
 
     Parameters
     ----------
     key
         Field identifier of each document.
-    on
-        Fields to use to match the query to the documents.
-    k
-        Number of documents to retrieve. Default is `None`, i.e all documents that match the query
-        will be retrieved.
-    keywords
-        Keywords extractor from [FlashText](https://github.com/vi3k6i5/flashtext). If set to None,
-        a default one is created.
+    index
+        Faiss index that will store the embeddings and perform the similarity search.
+    normalize
+        Whether to normalize the embeddings before adding them to the index in order to measure
+        cosine similarity.
 
     Examples
     --------
-
     >>> from pprint import pprint as print
     >>> from cherche import retrieve
+    >>> from sentence_transformers import SentenceTransformer
+
+    >>> recommend = retrieve.Embedding(
+    ...    key="id",
+    ... )
 
     >>> documents = [
-    ...    {"id": 0, "title": "Paris", "article": "This town is the capital of France", "author": "Wiki", "tags": ["paris", "capital"]},
-    ...    {"id": 1, "title": "Eiffel tower", "article": "Eiffel tower is based in Paris", "author": "Wiki", "tags": ["paris", "eiffel", "tower"]},
-    ...    {"id": 2, "title": "Montreal", "article": "Montreal is in Canada.", "author": "Wiki", "tags": ["canada", "montreal"]},
+    ...    {"id": "a", "title": "Paris", "author": "Paris"},
+    ...    {"id": "b", "title": "Madrid", "author": "Madrid"},
+    ...    {"id": "c", "title": "Montreal", "author": "Montreal"},
     ... ]
 
-    >>> retriever = retrieve.Flash(key="id", on="tags", k=2)
-
-    >>> retriever.add(documents=documents)
-    Flash retriever
-         key: id
-         on: tags
-         documents: 6
-
-    >>> print(retriever(q="paris"))
-    [{'id': 0, 'similarity': 1}, {'id': 1, 'similarity': 1}]
-
-    >>> retriever += documents
-
-    >>> print(retriever(q="paris"))
-    [{'article': 'This town is the capital of France',
-      'author': 'Wiki',
-      'id': 0,
-      'similarity': 1,
-      'tags': ['paris', 'capital'],
-      'title': 'Paris'},
-     {'article': 'Eiffel tower is based in Paris',
-      'author': 'Wiki',
-      'id': 1,
-      'similarity': 1,
-      'tags': ['paris', 'eiffel', 'tower'],
-      'title': 'Eiffel tower'}]
-
+    >>> encoder = SentenceTransformer("sentence-transformers/all-mpnet-base-v2")
+    >>> embeddings_documents = encoder.encode([
+    ...    document["title"] for document in documents
+    ... ])
+
+    >>> recommend.add(
+    ...    documents=documents,
+    ...    embeddings_documents=embeddings_documents,
+    ... )
+    Embedding retriever
+        key      : id
+        documents: 3
+
+    >>> queries = [
+    ...    "Paris",
+    ...    "Madrid",
+    ...    "Montreal"
+    ... ]
 
-    References
-    ----------
-    1. [FlashText](https://github.com/vi3k6i5/flashtext)
-    2. [Replace or Retrieve Keywords In Documents at Scale](https://arxiv.org/abs/1711.00046)
+    >>> embeddings_queries = encoder.encode(queries)
+    >>> print(recommend(embeddings_queries, k=2))
+    [[{'id': 'a', 'similarity': 1.0},
+      {'id': 'c', 'similarity': 0.5385907831761005}],
+     [{'id': 'b', 'similarity': 1.0},
+      {'id': 'a', 'similarity': 0.4990788711758875}],
+     [{'id': 'c', 'similarity': 1.0},
+      {'id': 'a', 'similarity': 0.5385907831761005}]]
+
+    >>> embeddings_queries = encoder.encode("Paris")
+    >>> print(recommend(embeddings_queries, k=2))
+    [{'id': 'a', 'similarity': 0.9999999999989104},
+     {'id': 'c', 'similarity': 0.5385907485958683}]
 
     """
 
     def __init__(
         self,
         key: str,
-        on: typing.Union[str, list],
-        k: int = None,
-        keywords: KeywordProcessor = None,
+        index=None,
+        normalize: bool = True,
+        k: typing.Optional[int] = None,
+        batch_size: int = 1024,
     ) -> None:
-        super().__init__(key=key, on=on, k=k)
-        self.documents = collections.defaultdict(list)
-        self.keywords = KeywordProcessor() if keywords is None else keywords
+        super().__init__(key=key, on="", k=k, batch_size=batch_size)
+
+        if index is None:
+            self.index = Faiss(key=self.key, normalize=normalize)
+        else:
+            self.index = Faiss(key=self.key, index=index, normalize=normalize)
+
+    def __repr__(self) -> str:
+        repr = f"{self.__class__.__name__} retriever"
+        repr += f"\n\tkey      : {self.key}"
+        repr += f"\n\tdocuments: {len(self)}"
+        return repr
+
+    def __len__(self) -> int:
+        return len(self.index)
 
-    def add(self, documents: list, **kwargs) -> "Flash":
-        """Add keywords to the retriever. Streaming friendly.
+    def add(
+        self,
+        documents: list,
+        embeddings_documents: np.ndarray,
+        **kwargs,
+    ) -> "Embedding":
+        """Add embeddings both documents and users.
 
         Parameters
         ----------
         documents
-            List of documents to add to the retriever.
+            List of documents to add to the index.
 
+        embeddings_documents
+            Embeddings of the documents ordered as the list of documents.
         """
-        for document in documents:
-            for field in self.on:
-                if field not in document:
-                    continue
-                if isinstance(document[field], list):
-                    for tag in document[field]:
-                        self.documents[tag].append({self.key: document[self.key]})
-                else:
-                    self.documents[document[field]].append(
-                        {self.key: document[self.key]}
-                    )
-                self._add(document=document[field])
+        self.index.add(
+            documents=documents,
+            embeddings=embeddings_documents,
+        )
         return self
 
-    def _add(self, document: typing.Union[list, str]) -> "Flash":
-        """Update keywords using dict, list or string."""
-        if isinstance(document, list):
-            self.keywords.add_keywords_from_list(document)
-        elif isinstance(document, str):
-            self.keywords.add_keyword(document)
-        return self
+    def __call__(
+        self,
+        q: np.ndarray,
+        k: typing.Optional[int] = None,
+        batch_size: typing.Optional[int] = None,
+        **kwargs,
+    ) -> typing.Union[
+        typing.List[typing.List[typing.Dict[str, str]]],
+        typing.List[typing.Dict[str, str]],
+    ]:
+        """Retrieve documents from the index.
+
+        Parameters
+        ----------
+        q
+            Either a single query or a list of queries.
+        k
+            Number of documents to retrieve. Default is `None`, i.e all documents that match the
+            query will be retrieved.
+        batch_size
+            Number of queries to encode at once.
+        """
+        k = k if k is not None else len(self)
 
-    def __call__(self, q: str, **kwargs) -> list:
-        """Retrieve tags."""
-        documents = list(
-            chain.from_iterable(
-                [self.documents[tag] for tag in self.keywords.extract_keywords(q)]
+        if len(q.shape) == 1:
+            q = q.reshape(1, -1)
+
+        rank = []
+        for batch in yield_batch(
+            array=q,
+            batch_size=batch_size if batch_size is not None else self.batch_size,
+            desc=f"{self.__class__.__name__} retriever",
+        ):
+            rank.extend(
+                self.index(
+                    embeddings=batch,
+                    k=k,
+                )
             )
-        )
 
-        # Remove duplicates documents
-        documents = [
-            {**{"similarity": 1}, **doc}
-            for n, doc in enumerate(documents)
-            if doc not in documents[n + 1 :]
-        ]
-        return documents[: self.k] if self.k is not None else documents
+        return rank[0] if len(q) == 1 else rank
```

### Comparing `cherche-1.0.1/cherche/retrieve/fuzz.py` & `cherche-2.0.0/cherche/retrieve/fuzz.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 __all__ = ["Fuzz"]
 
 import collections
 import typing
 
 from rapidfuzz import fuzz, process, utils
 
+from ..utils import yield_batch_single
 from .base import Retriever
 
 
 class Fuzz(Retriever):
     """[RapidFuzz](https://github.com/maxbachmann/RapidFuzz) wrapper. Rapid fuzzy string matching in Python and C++ using the Levenshtein Distance.
 
     Parameters
     ----------
     key
         Field identifier of each document.
     on
         Fields to use to match the query to the documents.
-    k
-        Number of documents to retrieve. Default is `None`, i.e all documents that match the query
-        will be retrieved.
     fuzzer
         [RapidFuzz scorer](https://maxbachmann.github.io/RapidFuzz/Usage/fuzz.html): fuzz.ratio,
         fuzz.partial_ratio, fuzz.token_set_ratio, fuzz.partial_token_set_ratio,
         fuzz.token_sort_ratio, fuzz.partial_token_sort_ratio, fuzz.token_ratio,
         fuzz.partial_token_ratio, fuzz.WRatio, fuzz.QRatio, string_metric.levenshtein,
         string_metric.normalized_levenshtein
     default_process
@@ -34,103 +32,72 @@
     --------
 
     >>> from pprint import pprint as print
     >>> from cherche import retrieve
     >>> from rapidfuzz import fuzz
 
     >>> documents = [
-    ...    {"id": 0, "title": "Paris", "article": "This town is the capital of France", "author": "Wiki", "tags": ["paris", "capital"]},
-    ...    {"id": 1, "title": "Eiffel tower", "article": "Eiffel tower is based in Paris", "author": "Wiki", "tags": ["paris", "eiffel", "tower"]},
-    ...    {"id": 2, "title": "Montreal", "article": "Montreal is in Canada.", "author": "Wiki", "tags": ["canada", "montreal"]},
+    ...     {"id": 0, "title": "Paris", "article": "Eiffel tower"},
+    ...     {"id": 1, "title": "Paris", "article": "Paris is in France."},
+    ...     {"id": 2, "title": "Montreal", "article": "Montreal is in Canada."},
     ... ]
 
     >>> retriever = retrieve.Fuzz(
     ...    key = "id",
     ...    on = ["title", "article"],
-    ...    k = 2,
     ...    fuzzer = fuzz.partial_ratio,
     ... )
 
     >>> retriever.add(documents=documents)
     Fuzz retriever
-         key: id
-         on: title, article
-         documents: 3
-         fuzzer: partial_ratio
+        key      : id
+        on       : title, article
+        documents: 3
 
-    >>> retriever("Paris")
+    >>> print(retriever(q="paris", k=2))
     [{'id': 0, 'similarity': 100.0}, {'id': 1, 'similarity': 100.0}]
 
-    >>> documents = [
-    ...    {"id": 0, "title": "Paris", "article": "Paris", "author": "Wiki", "tags": ["paris", "capital"]},
-    ...    {"id": 1, "title": "Eiffel tower", "article": "Paris", "author": "Wiki", "tags": ["paris", "eiffel", "tower"]},
-    ...    {"id": 2, "title": "Montreal", "article": "Canada.", "author": "Wiki", "tags": ["canada", "montreal"]},
-    ... ]
-
-    >>> retriever.add(documents=documents)
-    Fuzz retriever
-         key: id
-         on: title, article
-         documents: 3
-         fuzzer: partial_ratio
-
-    >>> retriever("Paris")
-    [{'id': 0, 'similarity': 100.0}, {'id': 1, 'similarity': 100.0}]
-
-    >>> documents = [
-    ...    {"id": 3, "title": "Paris", "article": "Paris", "author": "Wiki", "tags": ["paris", "capital"]},
-    ...    {"id": 4, "title": "Paris", "article": "Paris", "author": "Wiki", "tags": ["paris", "eiffel", "tower"]},
-    ... ]
-
-    >>> retriever.add(documents = documents)
-    Fuzz retriever
-         key: id
-         on: title, article
-         documents: 5
-         fuzzer: partial_ratio
-
-    >>> retriever("Paris")
-    [{'id': 0, 'similarity': 100.0}, {'id': 1, 'similarity': 100.0}]
+    >>> print(retriever(q=["paris", "montreal"], k=2))
+    [[{'id': 0, 'similarity': 100.0}, {'id': 1, 'similarity': 100.0}],
+     [{'id': 2, 'similarity': 100.0}, {'id': 1, 'similarity': 37.5}]]
+
+    >>> print(retriever(q=["unknown", "montreal"], k=2))
+    [[{'id': 2, 'similarity': 40.0}, {'id': 0, 'similarity': 36.36363636363637}],
+     [{'id': 2, 'similarity': 100.0}, {'id': 1, 'similarity': 37.5}]]
 
     References
     ----------
     1. [RapidFuzz](https://github.com/maxbachmann/RapidFuzz)
 
     """
 
     def __init__(
         self,
         key: str,
         on: typing.Union[str, list],
-        k: int,
         fuzzer=fuzz.partial_ratio,
         default_process: bool = True,
+        k: typing.Optional[int] = None,
     ) -> None:
-        super().__init__(key=key, on=on, k=k)
+        super().__init__(key=key, on=on, k=k, batch_size=1)
         self.fuzzer = fuzzer
         self.documents = collections.OrderedDict()
         self.index = {}
         self.default_process = default_process
 
-    def __repr__(self):
-        repr = super().__repr__()
-        repr += f"\n\t fuzzer: {self.fuzzer.__name__}"
-        return repr
-
-    def add(self, documents: list, **kwargs) -> "Fuzz":
+    def add(self, documents: typing.List[typing.Dict[str, str]], **kwargs) -> "Fuzz":
         """Fuzz is streaming friendly.
 
         Parameters
         ----------
         documents
             List of documents to add to the index.
 
         """
         for doc in documents:
-
             idx = len(self.documents)
 
             content = " ".join([doc.get(field, "") for field in self.on])
             if self.default_process:
                 content = utils.default_process(content)
 
             if doc[self.key] not in self.index:
@@ -145,25 +112,44 @@
                 self.documents[self.index[doc[self.key]]] = {
                     self.key: doc[self.key],
                     "fuzzer": content,
                 }
 
         return self
 
-    def __call__(self, q: str, **kwargs) -> dict:
-        """Retrieve documents using Fuzz.
+    def __call__(
+        self,
+        q: typing.Union[typing.List[str], str],
+        k: typing.Optional[int] = None,
+        **kwargs,
+    ) -> dict:
+        """Retrieve documents from the index.
 
         Parameters
         ----------
         q
-            Input query.
-
+            Either a single query or a list of queries.
+        k
+            Number of documents to retrieve. Default is `None`, i.e all documents that match the
+            query will be retrieved.
         """
-        return [
-            {self.key: self.documents[idx][self.key], "similarity": float(similarity)}
-            for _, similarity, idx in process.extract(
-                q,
-                [doc["fuzzer"] for doc in self.documents.values()],
-                scorer=self.fuzzer,
-                limit=self.k,
+        if k is None:
+            k = len(self.documents)
+
+        rank = []
+
+        for batch in yield_batch_single(
+            array=q, desc=f"{self.__class__.__name__} retriever"
+        ):
+            rank.append(
+                [
+                    {self.key: self.documents[idx][self.key], "similarity": similarity}
+                    for _, similarity, idx in process.extract(
+                        batch,
+                        [doc["fuzzer"] for doc in self.documents.values()],
+                        scorer=self.fuzzer,
+                        limit=k,
+                    )
+                ]
             )
-        ]
+
+        return rank[0] if isinstance(q, str) else rank
```

### Comparing `cherche-1.0.1/cherche/retrieve/lunr.py` & `cherche-2.0.0/cherche/retrieve/lunr.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 __all__ = ["Lunr"]
 
+import re
 import typing
 
-try:
-    from lunr import lunr
-except ImportError:
-    print("Unable to import Lunar")
+from lunr import lunr
 
+from ..utils import yield_batch_single
 from .base import Retriever
 
 
 class Lunr(Retriever):
     """Lunr is a Python implementation of Lunr.js by Oliver Nightingale. Lunr is a retriever
     dedicated for small and middle size corpus.
 
@@ -19,85 +18,103 @@
     key
         Field identifier of each document.
     on
         Fields to use to match the query to the documents.
     documents
         Documents in Lunr retriever are static. The retriever must be reseted to index new
         documents.
-    k
-        Number of documents to retrieve. Default is `None`, i.e all documents that match the query
-        will be retrieved.
 
     Examples
     --------
-
     >>> from pprint import pprint as print
     >>> from cherche import retrieve
 
     >>> documents = [
-    ...    {"id": 0, "title": "Paris", "article": "This town is the capital of France", "author": "Wiki"},
-    ...    {"id": 1, "title": "Eiffel tower", "article": "Eiffel tower is based in Paris", "author": "Wiki"},
-    ...    {"id": 2, "title": "Montreal", "article": "Montreal is in Canada.", "author": "Wiki"},
+    ...     {"id": 0, "title": "Paris", "article": "Eiffel tower"},
+    ...     {"id": 1, "title": "Paris", "article": "Paris is in France."},
+    ...     {"id": 2, "title": "Montreal", "article": "Montreal is in Canada."},
     ... ]
 
-    >>> retriever = retrieve.Lunr(key="id", on=["title", "article"], documents=documents, k=3)
+    >>> retriever = retrieve.Lunr(
+    ...     key="id",
+    ...     on=["title", "article"],
+    ...     documents=documents,
+    ... )
 
     >>> retriever
     Lunr retriever
-         key: id
-         on: title, article
-         documents: 3
-
-    >>> print(retriever(q="paris"))
-    [{'id': 0, 'similarity': 0.524}, {'id': 1, 'similarity': 0.414}]
-
-    >>> retriever += documents
-
-    >>> print(retriever(q="paris"))
-    [{'article': 'This town is the capital of France',
-      'author': 'Wiki',
-      'id': 0,
-      'similarity': 0.524,
-      'title': 'Paris'},
-     {'article': 'Eiffel tower is based in Paris',
-      'author': 'Wiki',
-      'id': 1,
-      'similarity': 0.414,
-      'title': 'Eiffel tower'}]
+        key      : id
+        on       : title, article
+        documents: 3
+
+    >>> print(retriever(q="paris", k=2))
+    [{'id': 1, 'similarity': 0.268}, {'id': 0, 'similarity': 0.134}]
+
+    >>> print(retriever(q=["paris", "montreal"], k=2))
+    [[{'id': 1, 'similarity': 0.268}, {'id': 0, 'similarity': 0.134}],
+     [{'id': 2, 'similarity': 0.94}]]
+
 
     References
     ----------
     1. [Lunr.py](https://github.com/yeraydiazdiaz/lunr.py)
     2. [Lunr.js](https://lunrjs.com)
     2. [Solr](https://solr.apache.org)
 
     """
 
     def __init__(
-        self, key: str, on: typing.Union[str, list], documents: list, k: int = None
+        self,
+        key: str,
+        on: typing.Union[str, list],
+        documents: list,
+        k: typing.Optional[int] = None,
     ) -> None:
-        super().__init__(key=key, on=on, k=k)
+        super().__init__(key=key, on=on, k=k, batch_size=1)
 
         self.documents = {
             str(document[self.key]): {self.key: document[self.key]}
             for document in documents
         }
 
         self.idx = lunr(
             ref=self.key,
             fields=tuple(self.on),
-            # Lunr does not handle missing fields.
             documents=[
-                {field: doc.get(field, "") for field in [self.key] + self.on}
-                for doc in documents
+                {field: document.get(field, "") for field in [self.key] + self.on}
+                for document in documents
             ],
         )
 
-    def __call__(self, q: str, **kwargs) -> list:
-        """Retrieve the right document."""
-        # We do not handle all Lunr possibilites right now.
-        q = q.replace(":", "").replace("-", "")
-        documents = [
-            {**self.documents[match["ref"]], "similarity": float(match["score"])}
-            for match in self.idx.search(q)
-        ]
-        return documents[: self.k] if self.k is not None else documents
+    def __call__(
+        self,
+        q: typing.Union[str, typing.List[str]],
+        k: typing.Optional[int] = None,
+        **kwargs,
+    ) -> typing.Union[
+        typing.List[typing.List[typing.Dict[str, str]]],
+        typing.List[typing.Dict[str, str]],
+    ]:
+        """Retrieve documents from the index.
+
+        Parameters
+        ----------
+        q
+            Either a single query or a list of queries.
+        k
+            Number of documents to retrieve. Default is `None`, i.e all documents that match the
+            query will be retrieved.
+        """
+        rank = []
+
+        for batch in yield_batch_single(
+            array=q, desc=f"{self.__class__.__name__} retriever"
+        ):
+            batch = re.sub("[^a-zA-Z0-9 \n\.]", " ", batch)
+            documents = [
+                {**self.documents[match["ref"]], "similarity": match["score"]}
+                for match in self.idx.search(batch)
+            ]
+            documents = documents[:k] if k is not None else documents
+            rank.append(documents)
+
+        return rank[0] if isinstance(q, str) else rank
```

### Comparing `cherche-1.0.1/cherche/retrieve/recommend.py` & `cherche-2.0.0/cherche/rank/cross_encoder.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,244 +1,217 @@
+__all__ = ["CrossEncoder"]
+
+import collections
 import typing
 
-import faiss
 import numpy as np
 
-from ..index import Faiss, Milvus
-from .base import Retriever
-
-__all__ = ["Recommend"]
-
-
-class MemoryStore:
-    """Store user embeddings in memory."""
-
-    def __init__(self):
-        self.embeddings = {}
-
-    def __len__(self):
-        return len(self.embeddings)
-
-    def add(self, users: list, embeddings: np.ndarray):
-        for user, embedding in zip(users, embeddings):
-            self.embeddings[user] = np.array(embedding)
-        return self
-
-    def get(self, values: list, **kwargs) -> typing.Tuple[list, list, list]:
-        """Get users embeddings from memory.
-
-        Parameters
-        ----------
-        values
-            List of user ids.
-
-        """
-        known, user_embeddings, unknown = [], [], []
-        for user in values:
-            embedding = self.embeddings.get(user, None)
-            if embedding is not None:
-                known.append(user)
-                user_embeddings.append(embedding)
-            else:
-                unknown.append(user)
-        return known, user_embeddings, unknown
+from ..compose import Intersection, Pipeline, Union, Vote
+from ..utils import yield_batch
 
 
-class Recommend(Retriever):
-    """Collaborative filtering as a retriever. Recommend is compatible with the library [Implicit](https://github.com/benfred/implicit).
+class CrossEncoder:
+    """Cross-Encoder as a ranker. CrossEncoder takes both the query and the document as input
+    and outputs a score. The score is a similarity score between the query and the document. The CrossEncoder cannot pre-compute the embeddings of the documents since it need both the query
+    and the document.
 
     Parameters
     ----------
-    key
-        Field identifier of each document.
-    k
-        Number of documents to retrieve. Default is `None`, i.e all documents that match the query
-        will be retrieved.
-    index
-        Index that will store the embeddings of documents and perform the similarity search.
-        The default index is Faiss. We can choose index.Milvus also.
-    store
-        Index that will store the embeddings of users. By default, it store users embeddings in
-        memory. We can choose index.Milvus also.
+    on
+        Fields to use to match the query to the documents.
+    encoder
+        Sentence Transformer cross-encoder.
 
     Examples
     --------
-
     >>> from pprint import pprint as print
-    >>> from cherche import retrieve, utils
-    >>> from implicit.nearest_neighbours import bm25_weight
-    >>> from implicit.als import AlternatingLeastSquares
-
-    >>> documents = [
-    ...    {"id": "a", "title": "Paris", "author": "Paris"},
-    ...    {"id": "b", "title": "Madrid", "author": "Madrid"},
-    ...    {"id": "c", "title": "Montreal", "author": "Montreal"},
-    ... ]
-
-    >>> ratings = {
-    ...    "Max": {"a": 1, "c": 1},
-    ...    "Adil": {"b": 1, "d": 2},
-    ...    "Robin": {"b": 1, "d": 1},
-    ...    "Geoffrey": {"a": 1, "c": 1},
-    ... }
-
-    >>> index_users, index_documents, sparse_ratings = utils.users_items_sparse(ratings=ratings)
-
-    >>> model = AlternatingLeastSquares(
-    ...     factors=64,
-    ...     regularization=0.05,
-    ...     alpha=2.0,
-    ...     iterations=100,
-    ...     random_state=42,
-    ... )
+    >>> from cherche import retrieve, rank, evaluate, data
+    >>> from sentence_transformers import CrossEncoder
 
-    >>> model.fit(sparse_ratings)
-
-    >>> embeddings_users = {
-    ...    user: embedding for user, embedding in zip(index_users, model.user_factors)
-    ... }
-
-    >>> embeddings_documents = {
-    ...    document: embedding
-    ...    for document, embedding in zip(index_documents, model.item_factors)
-    ... }
-
-    >>> recommend = retrieve.Recommend(
-    ...    key="id",
-    ...    k = 10,
+    >>> documents, query_answers = data.arxiv_tags(
+    ...    arxiv_title=True, arxiv_summary=False, comment=False
     ... )
 
-    >>> recommend.add(
+    >>> retriever = retrieve.TfIdf(
+    ...    key="uri",
+    ...    on=["prefLabel_text", "altLabel_text"],
     ...    documents=documents,
-    ...    embeddings_documents=embeddings_documents,
-    ...    embeddings_users=embeddings_users,
+    ...    k=100,
+    ... )
+
+    >>> ranker = rank.CrossEncoder(
+    ...     on = ["prefLabel_text", "altLabel_text"],
+    ...     encoder = CrossEncoder("cross-encoder/mmarco-mMiniLMv2-L12-H384-v1").predict,
     ... )
-    Recommend retriever
-        key: id
-        Users: 4
-        Documents: 3
-
-    >>> recommend += documents
-
-    >>> print(recommend(user="Geoffrey"))
-    [{'author': 'Montreal',
-      'id': 'c',
-      'similarity': 21229.834241369794,
-      'title': 'Montreal'},
-     {'author': 'Paris',
-      'id': 'a',
-      'similarity': 21229.634204933023,
-      'title': 'Paris'},
-     {'author': 'Madrid',
-      'id': 'b',
-      'similarity': 0.5075642957423536,
-      'title': 'Madrid'}]
 
+    >>> pipeline = retriever + documents + ranker
+
+    >>> match = pipeline("graph neural network", k=5)
+
+    >>> for m in match:
+    ...     print(m.get("uri", ""))
+    'http://www.semanlink.net/tag/graph_neural_networks'
+    'http://www.semanlink.net/tag/artificial_neural_network'
+    'http://www.semanlink.net/tag/dans_deep_averaging_neural_networks'
+    'http://www.semanlink.net/tag/recurrent_neural_network'
+    'http://www.semanlink.net/tag/convolutional_neural_network'
 
     References
     ----------
-    1. [Implicit](https://github.com/benfred/implicit)
-    2. [Implicit documentation](https://benfred.github.io/implicit/)
-    3. [Logistic Matrix Factorization for Implicit Feedback Data](https://web.stanford.edu/~rezab/nips2014workshop/submits/logmat.pdf)
-    4. [BPR: Bayesian Personalized Ranking from Implicit Feedback](https://arxiv.org/pdf/1205.2618.pdf)
-    5. [Collaborative Filtering for Implicit Feedback Datasets](http://yifanhu.net/PUB/cf.pdf)
+    1. [Sentence Transformers Cross-Encoders](https://www.sbert.net/examples/applications/cross-encoder/README.html)
+    2. [Cross-Encoders Hub](https://huggingface.co/cross-encoder)
 
     """
 
     def __init__(
         self,
-        key: str,
-        k: int = None,
-        index=None,
-        store=MemoryStore(),
-    ) -> None:
-        super().__init__(key=key, on="", k=k)
-
-        if index is None:
-            self.index = Faiss(key=self.key)
-        elif isinstance(index, Milvus) or isinstance(index, Faiss):
-            self.index = index
-        else:
-            self.index = Faiss(key=self.key, index=index)
-
-        self.store = store
+        on: typing.Union[typing.List[str], str],
+        encoder,
+        k: typing.Optional[int] = None,
+        batch_size: int = 64,
+    ):
+        self.on = on if isinstance(on, list) else [on]
+        self.encoder = encoder
+        self.k = k
+        self.batch_size = batch_size
 
     def __repr__(self) -> str:
-        repr = f"{self.__class__.__name__} retriever"
-        repr += f"\n \t key: {self.key}"
-        repr += f"\n \t Users: {len(self.store)}"
-        repr += f"\n \t Documents: {len(self.index)}"
+        repr = "Cross-encoder"
+        repr += f"\n\ton: {', '.join(self.on)}"
         return repr
 
-    def add(
+    def __call__(
         self,
+        q: str,
         documents: list,
-        embeddings_documents: dict,
-        embeddings_users: dict,
+        batch_size: typing.Optional[int] = None,
+        k: typing.Optional[int] = None,
         **kwargs,
-    ) -> "Recommend":
-        """Add embeddings both documents and users.
+    ) -> list:
+        """Rank inputs documents based on query.
 
         Parameters
         ----------
+        q
+            Inputs query.
         documents
-            List of documents.
-        embeddings_documents
-            Embeddings of the documents ordered as the list of documents.
-        users
-            List of users.
-        embeddings_users
-            Embeddings of the users ordered as the list of users.
+            List of documents to rank.
 
         """
-        index = {document[self.key]: document for document in documents}
+        if k is None:
+            k = self.k
 
-        self.index.add(
-            documents=[
-                index[key] for key in embeddings_documents.keys() if key in index
-            ],
-            embeddings=np.array(
+        if isinstance(q, str) and not documents:
+            return []
+
+        if isinstance(q, list) and not documents:
+            return [[]]
+
+        if isinstance(q, str):
+            queries = [q]
+            documents = [documents]
+        else:
+            queries = q
+
+        pairs = self._get_pairs(queries=queries, documents=documents)
+        scores = self._get_scores(
+            pairs=pairs,
+            batch_size=batch_size if batch_size is not None else self.batch_size,
+        )
+        ranked = self._get_rank(documents=documents, scores=scores, k=k)
+        return ranked[0] if isinstance(q, str) else ranked
+
+    def _get_pairs(
+        self,
+        queries: typing.List[str],
+        documents: typing.List[typing.List[typing.Dict[str, str]]],
+    ) -> typing.List[typing.Tuple[str, str]]:
+        """Format input pairs of documents and queries to feed the cross-encoder."""
+        pairs = []
+        for query, documents_query in zip(queries, documents):
+            pairs.extend(
                 [
-                    embedding
-                    for key, embedding in embeddings_documents.items()
-                    if key in index
+                    (query, " ".join([document.get(field, "") for field in self.on]))
+                    for document in documents_query
                 ]
-            ),
-        )
+            )
 
-        self.store.add(
-            users=[key for key in embeddings_users.keys()],
-            embeddings=[embedding for embedding in embeddings_users.values()],
-        )
+        return pairs
 
-        return self
+    def _get_scores(
+        self, pairs: typing.List[typing.Tuple[str, str]], batch_size: int
+    ) -> collections.deque:
+        """Compute scores for each pair of query and document."""
+        scores = []
+        for batch in yield_batch(
+            array=pairs,
+            batch_size=batch_size,
+            desc=f"{self.__class__.__name__} ranker",
+        ):
+            scores.extend(self.encoder(batch))
+        return collections.deque(scores)
 
-    def __call__(
+    def _get_rank(
         self,
-        user: typing.Union[str, int],
-        expr: str = None,
-        consistency_level: str = None,
-        partition_names: list = None,
-        **kwargs,
-    ) -> list:
-        """Retrieve documents from user id.
+        documents: typing.List[typing.List[typing.Dict[str, str]]],
+        scores: collections.deque,
+        k: int,
+    ):
+        """Rank documents based on scores."""
+        ranked = []
+
+        for n_query, documents_query in enumerate(documents):
+            # Extract scores for current query
+            array_scores = np.array(
+                [scores.popleft() for n_document in range(len(documents_query))]
+            ).reshape(1, -1)
+
+            # Sort scores ascending order
+            match = np.argsort(array_scores, axis=1)
+
+            # Keep top last k scores
+            if k is not None:
+                match = match[:, -k:]
 
-        Parameters
-        ----------
-        user
-            User id.
-        """
-        known, embedding, _ = self.store.get(values=[user])
+            # Reverse order
+            match = np.fliplr(match)
 
-        if not known:
-            return []
+            # Extract scores in the same order
+            array_scores = np.take_along_axis(array_scores, match, axis=1)
 
-        return self.index(
-            **{
-                "embedding": np.array(embedding),
-                "k": self.k,
-                "key": self.key,
-                "expr": expr,
-                "consistency_level": consistency_level,
-                "partition_names": partition_names,
-            }
-        )
+            # Append ranked documents
+            ranked.append(
+                [
+                    {**document, "similarity": similarity}
+                    for document, similarity in zip(
+                        np.take(documents_query, match.flatten(), axis=-1),
+                        array_scores.flatten(),
+                    )
+                ]
+            )
+
+        return ranked
+
+    def __add__(self, other) -> Pipeline:
+        """Custom operator to make pipeline."""
+        if isinstance(other, Pipeline):
+            return other + self
+        else:
+            return Pipeline(models=[other, self])
+
+    def __or__(self, other) -> Union:
+        """Union operator."""
+        if isinstance(other, Union):
+            return Union([self] + other.models)
+        return Union([self, other])
+
+    def __and__(self, other) -> Intersection:
+        """Intersection operator."""
+        if isinstance(other, Intersection):
+            return Intersection([self] + other.models)
+        return Intersection([self, other])
+
+    def __mul__(self, other) -> Vote:
+        """Voting operator."""
+        if isinstance(other, Vote):
+            return Vote([self] + other.models)
+        return Vote([self, other])
```

### Comparing `cherche-1.0.1/cherche/retrieve/test_retrieve.py` & `cherche-2.0.0/cherche/retrieve/test_retrieve.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 import pytest
 
-from .. import rank, retrieve
+from .. import retrieve
 
 
-def cherche_retrievers(on: str, k: int = None):
+def cherche_retrievers(on: str):
     """List of retrievers available in cherche."""
     yield from [
-        retrieve.TfIdf(key="title", on=on, documents=documents(), k=k),
-        retrieve.BM25Okapi(key="title", on=on, documents=documents(), k=k),
-        retrieve.BM25L(key="title", on=on, documents=documents(), k=k),
-        retrieve.Lunr(key="title", on=on, documents=documents(), k=k),
+        retrieve.TfIdf(key="title", on=on, documents=documents()),
+        retrieve.Lunr(key="title", on=on, documents=documents()),
     ]
 
 
 def documents():
     return [
         {
             "title": "Paris",
@@ -38,42 +36,42 @@
     [
         pytest.param(
             retriever,
             documents(),
             k,
             id=f"retriever: {retriever.__class__.__name__}, k: {k}",
         )
-        for k in [None, 0, 2, 4]
-        for retriever in cherche_retrievers(on="article", k=k)
+        for k in [None, 2, 4]
+        for retriever in cherche_retrievers(on="article")
     ],
 )
 def test_retriever(retriever, documents: list, k: int):
     """Test retriever. Test if the number of retrieved documents is coherent.
     Check for unknown tokens in the corpus, should returns an empty list.
     """
     retriever = retriever + documents
     retriever.add(documents)
 
     # A single document contains town.
-    answers = retriever(q="town")
+    answers = retriever(q="town", k=k)
     if k is None or k >= 1:
-        assert len(answers) == 1
+        assert len(answers) >= 1
     else:
         assert len(answers) == 0
 
     for sample in answers:
         for key in ["title", "article", "author"]:
             assert key in sample
 
     # Unknown token.
-    answers = retriever(q="Unknown")
+    answers = retriever(q="un", k=k)
     assert len(answers) == 0
 
     # All documents contains "Montreal Eiffel France"
-    answers = retriever(q="Montreal Eiffel France")
+    answers = retriever(q="Montreal Eiffel France", k=k)
     if k is None or k >= len(documents):
         assert len(answers) == len(documents)
     else:
         assert len(answers) == k
 
 
 @pytest.mark.parametrize(
@@ -81,39 +79,39 @@
     [
         pytest.param(
             retriever,
             documents(),
             k,
             id=f"Multiple fields retriever: {retriever.__class__.__name__}, k: {k}",
         )
-        for k in [None, 0, 2, 4]
-        for retriever in cherche_retrievers(on=["article", "title", "author"], k=k)
+        for k in [None, 2, 4]
+        for retriever in cherche_retrievers(on=["article", "title", "author"])
     ],
 )
 def test_fields_retriever(retriever, documents: list, k: int):
     """Test retriever when providing multiples fields."""
     retriever = retriever + documents
 
     # All documents have Wikipedia as author.
-    answers = retriever(q="Wikipedia")
+    answers = retriever(q="Wikipedia", k=k)
     if k is None or k >= len(documents):
         assert len(answers) == len(documents)
     else:
         assert len(answers) == max(k, 0)
 
     for sample in answers:
         for key in ["title", "article", "author"]:
             assert key in sample
 
     # Unknown token.
-    answers = retriever(q="Unknown")
+    answers = retriever(q="un")
     assert len(answers) == 0
 
     # Two documents contains paris
-    answers = retriever(q="Paris")
+    answers = retriever(q="Paris", k=k)
 
     if k is None or k >= 2:
         assert len(answers) == 2
     else:
         assert len(answers) == max(k, 0)
 
 
@@ -121,97 +119,38 @@
     "documents, k",
     [
         pytest.param(
             documents(),
             k,
             id=f"retriever: Flash, k: {k}",
         )
-        for k in [None, 0, 2, 4]
+        for k in [None, 2, 4]
     ],
 )
 def test_flash(documents: list, k: int):
     """Test Flash retriever."""
     # Reset retriever
-    retriever = retrieve.Flash(key="title", k=k, on="title") + documents
+    retriever = retrieve.Flash(key="title", on="title") + documents
     retriever.add(documents)
 
     # A single document contains town.
-    answers = retriever(q="Paris")
+    answers = retriever(q="paris", k=k)
     if k is None or k >= 1:
         assert len(answers) == 1
     else:
         assert len(answers) == 0
 
     for sample in answers:
         for key in ["title", "article", "author"]:
             assert key in sample
 
     # Unknown token.
-    answers = retriever(q="Unknown")
+    answers = retriever(q="Unknown", k=k)
     assert len(answers) == 0
 
     # All documents contains is
-    answers = retriever(q="Paris Eiffel tower Montreal")
+    answers = retriever(q="Paris Eiffel tower Montreal", k=k)
 
     if k is None or k >= len(documents):
         assert len(answers) == len(documents)
     else:
         assert len(answers) == k
-
-
-@pytest.mark.parametrize(
-    "documents, k",
-    [
-        pytest.param(
-            documents(),
-            k,
-            id=f"retriever: ElasticSearch, k: {k}",
-        )
-        for k in [None, 0, 2, 4]
-    ],
-)
-def test_elastic(documents, k):
-    """Test Elasticsearch if elastic server is running. Test elasticsearch as a retriever for a
-    single field and multiple fields. Test if storing"""
-    from elasticsearch import Elasticsearch
-    from sentence_transformers import SentenceTransformer
-
-    es = Elasticsearch("http://localhost:9200")
-
-    if es.ping():
-
-        ranker = rank.Encoder(
-            key="title",
-            encoder=SentenceTransformer(
-                "sentence-transformers/all-mpnet-base-v2",
-            ).encode,
-            on=["title", "article", "author"],
-            k=k,
-        )
-
-        retriever = retrieve.Elastic(
-            key="title", on="article", k=k, es=es, index="test_cherche"
-        )
-        retriever.reset()
-        retriever.add(documents)
-        test_retriever(retriever=retriever, documents=documents, k=k)
-
-        retriever = retrieve.Elastic(
-            key="title",
-            on=["title", "article", "author"],
-            k=k,
-            es=es,
-            index="test_cherche",
-        )
-        retriever.reset()
-        retriever.add(documents)
-        test_fields_retriever(retriever, documents=documents, k=k)
-
-        # Store embeddings using Elasticsearch
-        retriever.reset()
-        retriever.add_embeddings(documents=documents, ranker=ranker)
-        pipeline = retriever + ranker
-        answers = pipeline("Paris")
-        if k is None or k >= 2:
-            assert len(answers) == 2
-        else:
-            assert len(answers) == max(k, 0)
```

### Comparing `cherche-1.0.1/cherche.egg-info/SOURCES.txt` & `cherche-2.0.0/cherche.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -7,68 +7,50 @@
 cherche.egg-info/PKG-INFO
 cherche.egg-info/SOURCES.txt
 cherche.egg-info/dependency_links.txt
 cherche.egg-info/requires.txt
 cherche.egg-info/top_level.txt
 cherche/compose/__init__.py
 cherche/compose/base.py
+cherche/compose/intersection_union_vote.py
 cherche/compose/pipeline.py
 cherche/compose/test_compose.py
 cherche/compose/test_union_inter.py
 cherche/compose/test_vote.py
-cherche/compose/union_inter_vote.py
 cherche/data/__init__.py
-cherche/data/norvig.txt
 cherche/data/semanlink.py
 cherche/data/towns.json
 cherche/data/towns.py
 cherche/data/semanlink/arxiv.json
 cherche/data/semanlink/docs.json
 cherche/data/semanlink/tags.json
-cherche/eval/__init__.py
-cherche/eval/eval.py
-cherche/generate/__init__.py
-cherche/generate/base.py
-cherche/generate/rag.py
+cherche/evaluate/__init__.py
+cherche/evaluate/evaluate.py
 cherche/index/__init__.py
-cherche/index/milvus.py
-cherche/index/tree.py
-cherche/onnx/__init__.py
-cherche/onnx/base.py
-cherche/onnx/qa.py
-cherche/onnx/sentence_transformers.py
+cherche/index/faiss_index.py
 cherche/qa/__init__.py
 cherche/qa/qa.py
 cherche/query/__init__.py
 cherche/query/base.py
 cherche/query/norvig.py
 cherche/query/prf.py
 cherche/rank/__init__.py
 cherche/rank/base.py
+cherche/rank/cross_encoder.py
 cherche/rank/dpr.py
+cherche/rank/embedding.py
 cherche/rank/encoder.py
-cherche/rank/recommend.py
 cherche/rank/test_rank.py
-cherche/rank/zero_shot.py
 cherche/retrieve/__init__.py
 cherche/retrieve/base.py
-cherche/retrieve/bm25.py
 cherche/retrieve/dpr.py
-cherche/retrieve/elastic.py
+cherche/retrieve/embedding.py
 cherche/retrieve/encoder.py
 cherche/retrieve/flash.py
 cherche/retrieve/fuzz.py
 cherche/retrieve/lunr.py
-cherche/retrieve/meilisearch.py
-cherche/retrieve/recommend.py
 cherche/retrieve/test_retrieve.py
 cherche/retrieve/tfidf.py
-cherche/retrieve/tpsense.py
-cherche/similarity/__init__.py
-cherche/similarity/similarity.py
-cherche/summary/__init__.py
-cherche/summary/summary.py
-cherche/translate/__init__.py
-cherche/translate/translate.py
 cherche/utils/__init__.py
+cherche/utils/batch.py
 cherche/utils/quantize.py
-cherche/utils/recommend.py
+cherche/utils/topk.py
```

### Comparing `cherche-1.0.1/setup.py` & `cherche-2.0.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,77 +2,61 @@
 
 from cherche.__version__ import __version__
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 base_packages = [
-    "elasticsearch >= 7.10.0",
-    "faiss-cpu >= 1.7.1.post3",
+    "numpy >= 1.24.3",
+    "scikit-learn >= 1.2.2",
+    "lunr >= 0.6.2",
+    "rapidfuzz >= 3.0.0",
     "flashtext >= 2.7",
-    "implicit >= 0.6.1",
-    "lunr >= 0.6.1",
-    "meilisearch >= 0.22.1",
-    "more-itertools >= 9.0.0",
-    "numpy >= 1.19.0",
-    "rank-bm25 == 0.2.1",
-    "rapidfuzz >= 1.9.1",
-    "river >= 0.8.0",
-    "scikit-learn >= 1.0",
-    "scipy >= 1.7.3",
-    "sentence-transformers >= 2.1.0",
-    "transformers >= 4.12.0",
     "tqdm >= 4.62.3",
-    "typesense >= 0.14.0",
+    "scipy >= 1.7.3",
 ]
 
-milvus = ["pymilvus >= 2.1.3"]
-
-onnx = ["onnx >= 1.10.2", "onnxruntime >= 1.9.0"]
-
-onnxgpu = ["onnx >= 1.10.2", "onnxruntime-gpu >= 1.9.0"]
-
-doc = [
+cpu = ["sentence-transformers >= 2.2.2", "faiss-cpu >= 1.7.4"]
+gpu = ["sentence-transformers >= 2.2.2", "faiss-gpu >= 1.7.4"]
+dev = [
     "numpydoc >= 1.4.0",
     "mkdocs_material >= 8.3.5",
     "mkdocs-awesome-pages-plugin >= 2.7.0",
     "mkdocs-jupyter >= 0.21.0",
+    "pytest-cov >= 4.0.0",
+    "pytest >= 7.3.1",
+    "isort >= 5.12.0",
+    "ipywidgets >= 8.0.6",
 ]
 
 setuptools.setup(
     name="cherche",
     version=f"{__version__}",
     license="MIT",
     author="Raphael Sourty",
     author_email="raphael.sourty@gmail.com",
     description="Neural Search",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/raphaelsty/cherche",
     download_url="https://github.com/user/cherche/archive/v_01.tar.gz",
     keywords=[
-        "neural",
-        "search",
-        "question",
-        "answering",
-        "summarization",
-        "collaborative filtering",
+        "neural search",
+        "information retrieval",
+        "question answering",
+        "semantic search",
     ],
     packages=setuptools.find_packages(),
     install_requires=base_packages,
     extras_require={
-        "recommend": base_packages,
-        "onnx": base_packages + onnx,
-        "onnxgpu": base_packages + onnxgpu,
-        "doc": base_packages + doc,
-        "milvus": base_packages + milvus,
-    },
-    package_data={
-        "cherche": ["data/towns.json", "data/semanlink/*.json", "data/norvig.txt"]
+        "cpu": base_packages + cpu,
+        "gpu": base_packages + gpu,
+        "dev": base_packages + cpu + dev,
     },
+    package_data={"cherche": ["data/towns.json", "data/semanlink/*.json"]},
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.6",
 )
```

