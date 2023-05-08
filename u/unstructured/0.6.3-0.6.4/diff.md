# Comparing `tmp/unstructured-0.6.3.tar.gz` & `tmp/unstructured-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unstructured-0.6.3.tar", last modified: Thu May  4 20:26:31 2023, max compression
+gzip compressed data, was "unstructured-0.6.4.tar", last modified: Mon May  8 17:58:20 2023, max compression
```

## Comparing `unstructured-0.6.3.tar` & `unstructured-0.6.4.tar`

### file list

```diff
@@ -1,107 +1,108 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:26:31.823834 unstructured-0.6.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-05-04 20:26:22.000000 unstructured-0.6.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)    21094 2023-05-04 20:26:31.823834 unstructured-0.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16837 2023-05-04 20:26:22.000000 unstructured-0.6.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-04 20:26:31.823834 unstructured-0.6.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-05-04 20:26:22.000000 unstructured-0.6.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:26:31.807834 unstructured-0.6.3/test_unstructured/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 20:26:22.000000 unstructured-0.6.3/test_unstructured/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:26:31.807834 unstructured-0.6.3/test_unstructured/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 20:26:22.000000 unstructured-0.6.3/test_unstructured/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-04 20:26:22.000000 unstructured-0.6.3/test_unstructured/nlp/mock_nltk.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-04 20:26:22.000000 unstructured-0.6.3/test_unstructured/nlp/test_partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-05-04 20:26:22.000000 unstructured-0.6.3/test_unstructured/nlp/test_tokenize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-05-04 20:26:22.000000 unstructured-0.6.3/test_unstructured/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:26:31.811833 unstructured-0.6.3/unstructured/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:26:31.811833 unstructured-0.6.3/unstructured/cleaners/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/cleaners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8620 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/cleaners/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/cleaners/extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/cleaners/translate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:26:31.811833 unstructured-0.6.3/unstructured/documents/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/documents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/documents/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/documents/elements.py
--rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/documents/email_elements.py
--rw-r--r--   0 runner    (1001) docker     (123)    15004 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/documents/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/documents/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:26:31.811833 unstructured-0.6.3/unstructured/file_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/file_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/file_utils/exploration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/file_utils/file_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)    10794 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/file_utils/filetype.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/file_utils/google_filetype.py
--rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/file_utils/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:26:31.811833 unstructured-0.6.3/unstructured/ingest/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/ingest/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:26:31.811833 unstructured-0.6.3/unstructured/ingest/connector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/ingest/connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/ingest/connector/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)    10204 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/ingest/connector/biomed.py
--rw-r--r--   0 runner    (1001) docker     (123)     6851 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/ingest/connector/fsspec.py
--rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/ingest/connector/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/ingest/connector/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/ingest/connector/gitlab.py
--rw-r--r--   0 runner    (1001) docker     (123)    11172 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/ingest/connector/google_drive.py
--rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/ingest/connector/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/ingest/connector/reddit.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/ingest/connector/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     7517 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/ingest/connector/slack.py
--rw-r--r--   0 runner    (1001) docker     (123)     5411 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/ingest/connector/wikipedia.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:26:31.815834 unstructured-0.6.3/unstructured/ingest/doc_processor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/ingest/doc_processor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/ingest/doc_processor/generalized.py
--rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/ingest/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/ingest/logger.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    27999 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/ingest/main.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:26:31.815834 unstructured-0.6.3/unstructured/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:26:31.819834 unstructured-0.6.3/unstructured/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  4472047 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/nlp/english-words.txt
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/nlp/english_words.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/nlp/partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/nlp/patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/nlp/tokenize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:26:31.819834 unstructured-0.6.3/unstructured/partition/
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/partition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6220 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/partition/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7732 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/partition/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/partition/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/partition/doc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/partition/docx.py
--rw-r--r--   0 runner    (1001) docker     (123)     9408 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/partition/email.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/partition/epub.py
--rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/partition/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/partition/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/partition/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/partition/md.py
--rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/partition/msg.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/partition/odt.py
--rw-r--r--   0 runner    (1001) docker     (123)    12665 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/partition/pdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/partition/ppt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/partition/pptx.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/partition/rtf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/partition/text.py
--rw-r--r--   0 runner    (1001) docker     (123)    11064 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/partition/text_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:26:31.819834 unstructured-0.6.3/unstructured/staging/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/staging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/staging/argilla.py
--rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/staging/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/staging/baseplate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/staging/datasaur.py
--rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/staging/huggingface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/staging/label_box.py
--rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/staging/label_studio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/staging/prodigy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-05-04 20:26:22.000000 unstructured-0.6.3/unstructured/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:26:31.811833 unstructured-0.6.3/unstructured.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21094 2023-05-04 20:26:31.000000 unstructured-0.6.3/unstructured.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-05-04 20:26:31.000000 unstructured-0.6.3/unstructured.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 20:26:31.000000 unstructured-0.6.3/unstructured.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-04 20:26:31.000000 unstructured-0.6.3/unstructured.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-04 20:26:31.000000 unstructured-0.6.3/unstructured.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-04 20:26:31.000000 unstructured-0.6.3/unstructured.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:58:20.158476 unstructured-0.6.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-05-08 17:58:11.000000 unstructured-0.6.4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    21142 2023-05-08 17:58:20.158476 unstructured-0.6.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16877 2023-05-08 17:58:11.000000 unstructured-0.6.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-08 17:58:20.158476 unstructured-0.6.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-05-08 17:58:12.000000 unstructured-0.6.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:58:20.146476 unstructured-0.6.4/test_unstructured/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 17:58:12.000000 unstructured-0.6.4/test_unstructured/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:58:20.146476 unstructured-0.6.4/test_unstructured/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 17:58:12.000000 unstructured-0.6.4/test_unstructured/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-08 17:58:12.000000 unstructured-0.6.4/test_unstructured/nlp/mock_nltk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-08 17:58:12.000000 unstructured-0.6.4/test_unstructured/nlp/test_partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-05-08 17:58:12.000000 unstructured-0.6.4/test_unstructured/nlp/test_tokenize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-05-08 17:58:12.000000 unstructured-0.6.4/test_unstructured/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:58:20.146476 unstructured-0.6.4/unstructured/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:58:20.146476 unstructured-0.6.4/unstructured/cleaners/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/cleaners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8620 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/cleaners/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/cleaners/extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/cleaners/translate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:58:20.146476 unstructured-0.6.4/unstructured/documents/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/documents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/documents/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/documents/elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/documents/email_elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15004 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/documents/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/documents/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:58:20.150476 unstructured-0.6.4/unstructured/file_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/file_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/file_utils/exploration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/file_utils/file_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10794 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/file_utils/filetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/file_utils/google_filetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/file_utils/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:58:20.150476 unstructured-0.6.4/unstructured/ingest/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/ingest/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:58:20.150476 unstructured-0.6.4/unstructured/ingest/connector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/ingest/connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/ingest/connector/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10204 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/ingest/connector/biomed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6851 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/ingest/connector/fsspec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/ingest/connector/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/ingest/connector/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/ingest/connector/gitlab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11172 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/ingest/connector/google_drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/ingest/connector/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/ingest/connector/reddit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/ingest/connector/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7517 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/ingest/connector/slack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5411 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/ingest/connector/wikipedia.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:58:20.150476 unstructured-0.6.4/unstructured/ingest/doc_processor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/ingest/doc_processor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/ingest/doc_processor/generalized.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/ingest/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/ingest/logger.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    27999 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/ingest/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:58:20.150476 unstructured-0.6.4/unstructured/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:58:20.154476 unstructured-0.6.4/unstructured/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  4472047 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/nlp/english-words.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/nlp/english_words.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/nlp/partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/nlp/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/nlp/tokenize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:58:20.158476 unstructured-0.6.4/unstructured/partition/
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/partition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6220 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/partition/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7732 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/partition/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/partition/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/partition/doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/partition/docx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9408 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/partition/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/partition/epub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/partition/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/partition/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/partition/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/partition/md.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/partition/msg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/partition/odt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12410 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/partition/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/partition/ppt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/partition/pptx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/partition/rtf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4266 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/partition/strategies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/partition/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11064 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/partition/text_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:58:20.158476 unstructured-0.6.4/unstructured/staging/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/staging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/staging/argilla.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/staging/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/staging/baseplate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/staging/datasaur.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/staging/huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/staging/label_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/staging/label_studio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/staging/prodigy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:58:20.146476 unstructured-0.6.4/unstructured.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21142 2023-05-08 17:58:20.000000 unstructured-0.6.4/unstructured.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-05-08 17:58:20.000000 unstructured-0.6.4/unstructured.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 17:58:20.000000 unstructured-0.6.4/unstructured.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-08 17:58:20.000000 unstructured-0.6.4/unstructured.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-08 17:58:20.000000 unstructured-0.6.4/unstructured.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-08 17:58:20.000000 unstructured-0.6.4/unstructured.egg-info/top_level.txt
```

### Comparing `unstructured-0.6.3/LICENSE.md` & `unstructured-0.6.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.3/PKG-INFO` & `unstructured-0.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unstructured
-Version: 0.6.3
+Version: 0.6.4
 Summary: A library that prepares raw documents for downstream ML tasks.
 Home-page: https://github.com/Unstructured-IO/unstructured
 Author: Unstructured Technologies
 Author-email: devops@unstructuredai.io
 License: Apache-2.0
 Description: <h3 align="center">
           <img
@@ -79,14 +79,15 @@
           Depending on what document types you're parsing, you may not need all of these.
             - `libmagic-dev` (filetype detection)
             - `poppler-utils` (images and PDFs)
             - `tesseract-ocr` (images and PDFs)
             - `libreoffice` (MS Office docs)
         - If you are parsing PDFs, run the following to install the `detectron2` model, which
           `unstructured` uses for layout detection:
+            - `pip install tensorboard>=2.12.2`
             - `pip install "detectron2@git+https://github.com/facebookresearch/detectron2.git@e2ce8dc#egg=detectron2"`
         
         At this point, you should be able to run the following code:
         
         ```python
         from unstructured.partition.auto import partition
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: unstructured Version: 0.6.3 Summary: A library that
+Metadata-Version: 2.1 Name: unstructured Version: 0.6.4 Summary: A library that
 prepares raw documents for downstream ML tasks. Home-page: https://github.com/
 Unstructured-IO/unstructured Author: Unstructured Technologies Author-email:
 devops@unstructuredai.io License: Apache-2.0 Description:
 **** [https://raw.githubusercontent.com/Unstructured-IO/unstructured/main/img/
                           unstructured_logo.png] ****
  ![https://pypi.python.org/pypi/unstructured/](https://img.shields.io/pypi/l/
    unstructured.svg) ![https://pypi.python.org/pypi/unstructured/](https://
@@ -46,59 +46,59 @@
 need to process PDFs or images, you can run `pip install unstructured` -
 Install the following system dependencies if they are not already available on
 your system. Depending on what document types you're parsing, you may not need
 all of these. - `libmagic-dev` (filetype detection) - `poppler-utils` (images
 and PDFs) - `tesseract-ocr` (images and PDFs) - `libreoffice` (MS Office docs)
 - If you are parsing PDFs, run the following to install the `detectron2` model,
 which `unstructured` uses for layout detection: - `pip install
-"detectron2@git+https://github.com/facebookresearch/
-detectron2.git@e2ce8dc#egg=detectron2"` At this point, you should be able to
-run the following code: ```python from unstructured.partition.auto import
-partition elements = partition(filename="example-docs/fake-email.eml") print
-("\n\n".join([str(el) for el in elements])) ``` And if you installed with
-`local-inference`, you should be able to run this as well: ```python from
-unstructured.partition.auto import partition elements = partition("example-
-docs/layout-parser-paper.pdf") print("\n\n".join([str(el) for el in elements]))
-``` ## :dizzy: Instructions for using the docker image The following
-instructions are intended to help you get up and running using Docker to
-interact with `unstructured`. See [here](https://docs.docker.com/get-docker/
-) if you don't already have docker installed on your machine. NOTE: we build
-multi-platform images to support both x86_64 and Apple silicon hardware.
-`docker pull` should download the corresponding image for your architecture,
-but you can specify with `--platform` (e.g. `--platform linux/amd64`) if
-needed. We build Docker images for all pushes to `main`. We tag each image with
-the corresponding short commit hash (e.g. `fbc7a69`) and the application
-version (e.g. `0.5.5-dev1`). We also tag the most recent image with `latest`.
-To leverage this, `docker pull` from our image repository. ```bash docker pull
-quay.io/unstructured-io/unstructured:latest ``` Once pulled, you can create a
-container from this image and shell to it. ```bash # create the container
-docker run -dt --name unstructured quay.io/unstructured-io/unstructured:latest
-# this will drop you into a bash shell where the Docker image is running docker
-exec -it unstructured bash ``` You can also build your own Docker image. If you
-only plan on parsing one type of data you can speed up building the image by
-commenting out some of the packages/requirements necessary for other data
-types. See Dockerfile to know which lines are necessary for your use case.
-```bash make docker-build # this will drop you into a bash shell where the
-Docker image is running make docker-start-bash ``` Once in the running
-container, you can try things out directly in Python interpreter's interactive
-mode. ```bash # this will drop you into a python console so you can run the
-below partition functions python3 >>> from unstructured.partition.pdf import
-partition_pdf >>> elements = partition_pdf(filename="example-docs/layout-
-parser-paper-fast.pdf") >>> from unstructured.partition.text import
-partition_text >>> elements = partition_text(filename="example-docs/fake-
-text.txt") ``` ## :coffee: Installation Instructions for Local Development The
-following instructions are intended to help you get up and running with
-`unstructured` locally if you are planning to contribute to the project. *
-Using `pyenv` to manage virtualenv's is recommended but not necessary * Mac
-install instructions. See [here](https://github.com/Unstructured-IO/
-community#mac--homebrew) for more detailed instructions. * `brew install pyenv-
-virtualenv` * `pyenv install 3.8.15` * Linux instructions are available [here]
-(https://github.com/Unstructured-IO/community#linux). * Create a virtualenv to
-work in and activate it, e.g. for one named `unstructured`: `pyenv virtualenv
-3.8.15 unstructured`
+tensorboard>=2.12.2` - `pip install "detectron2@git+https://github.com/
+facebookresearch/detectron2.git@e2ce8dc#egg=detectron2"` At this point, you
+should be able to run the following code: ```python from
+unstructured.partition.auto import partition elements = partition
+(filename="example-docs/fake-email.eml") print("\n\n".join([str(el) for el in
+elements])) ``` And if you installed with `local-inference`, you should be able
+to run this as well: ```python from unstructured.partition.auto import
+partition elements = partition("example-docs/layout-parser-paper.pdf") print
+("\n\n".join([str(el) for el in elements])) ``` ## :dizzy: Instructions for
+using the docker image The following instructions are intended to help you get
+up and running using Docker to interact with `unstructured`. See [here](https:/
+/docs.docker.com/get-docker/) if you don't already have docker installed on
+your machine. NOTE: we build multi-platform images to support both x86_64 and
+Apple silicon hardware. `docker pull` should download the corresponding image
+for your architecture, but you can specify with `--platform` (e.g. `--platform
+linux/amd64`) if needed. We build Docker images for all pushes to `main`. We
+tag each image with the corresponding short commit hash (e.g. `fbc7a69`) and
+the application version (e.g. `0.5.5-dev1`). We also tag the most recent image
+with `latest`. To leverage this, `docker pull` from our image repository.
+```bash docker pull quay.io/unstructured-io/unstructured:latest ``` Once
+pulled, you can create a container from this image and shell to it. ```bash #
+create the container docker run -dt --name unstructured quay.io/unstructured-
+io/unstructured:latest # this will drop you into a bash shell where the Docker
+image is running docker exec -it unstructured bash ``` You can also build your
+own Docker image. If you only plan on parsing one type of data you can speed up
+building the image by commenting out some of the packages/requirements
+necessary for other data types. See Dockerfile to know which lines are
+necessary for your use case. ```bash make docker-build # this will drop you
+into a bash shell where the Docker image is running make docker-start-bash ```
+Once in the running container, you can try things out directly in Python
+interpreter's interactive mode. ```bash # this will drop you into a python
+console so you can run the below partition functions python3 >>> from
+unstructured.partition.pdf import partition_pdf >>> elements = partition_pdf
+(filename="example-docs/layout-parser-paper-fast.pdf") >>> from
+unstructured.partition.text import partition_text >>> elements = partition_text
+(filename="example-docs/fake-text.txt") ``` ## :coffee: Installation
+Instructions for Local Development The following instructions are intended to
+help you get up and running with `unstructured` locally if you are planning to
+contribute to the project. * Using `pyenv` to manage virtualenv's is
+recommended but not necessary * Mac install instructions. See [here](https://
+github.com/Unstructured-IO/community#mac--homebrew) for more detailed
+instructions. * `brew install pyenv-virtualenv` * `pyenv install 3.8.15` *
+Linux instructions are available [here](https://github.com/Unstructured-IO/
+community#linux). * Create a virtualenv to work in and activate it, e.g. for
+one named `unstructured`: `pyenv virtualenv 3.8.15 unstructured`
 `pyenv activate unstructured` * Run `make install` * Optional: * To install
 models and dependencies for processing images and PDFs locally, run `make
 install-local-inference`. * For processing image files, `tesseract` is
 required. See [here](https://tesseract-ocr.github.io/tessdoc/Installation.html)
 for installation instructions. * For processing PDF files, `tesseract` and
 `poppler` are required. The [pdf2image docs](https://pdf2image.readthedocs.io/
 en/latest/installation.html) have instructions on installing `poppler` across
```

### Comparing `unstructured-0.6.3/README.md` & `unstructured-0.6.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -71,14 +71,15 @@
   Depending on what document types you're parsing, you may not need all of these.
     - `libmagic-dev` (filetype detection)
     - `poppler-utils` (images and PDFs)
     - `tesseract-ocr` (images and PDFs)
     - `libreoffice` (MS Office docs)
 - If you are parsing PDFs, run the following to install the `detectron2` model, which
   `unstructured` uses for layout detection:
+    - `pip install tensorboard>=2.12.2`
     - `pip install "detectron2@git+https://github.com/facebookresearch/detectron2.git@e2ce8dc#egg=detectron2"`
 
 At this point, you should be able to run the following code:
 
 ```python
 from unstructured.partition.auto import partition
```

#### html2text {}

```diff
@@ -42,59 +42,59 @@
 need to process PDFs or images, you can run `pip install unstructured` -
 Install the following system dependencies if they are not already available on
 your system. Depending on what document types you're parsing, you may not need
 all of these. - `libmagic-dev` (filetype detection) - `poppler-utils` (images
 and PDFs) - `tesseract-ocr` (images and PDFs) - `libreoffice` (MS Office docs)
 - If you are parsing PDFs, run the following to install the `detectron2` model,
 which `unstructured` uses for layout detection: - `pip install
-"detectron2@git+https://github.com/facebookresearch/
-detectron2.git@e2ce8dc#egg=detectron2"` At this point, you should be able to
-run the following code: ```python from unstructured.partition.auto import
-partition elements = partition(filename="example-docs/fake-email.eml") print
-("\n\n".join([str(el) for el in elements])) ``` And if you installed with
-`local-inference`, you should be able to run this as well: ```python from
-unstructured.partition.auto import partition elements = partition("example-
-docs/layout-parser-paper.pdf") print("\n\n".join([str(el) for el in elements]))
-``` ## :dizzy: Instructions for using the docker image The following
-instructions are intended to help you get up and running using Docker to
-interact with `unstructured`. See [here](https://docs.docker.com/get-docker/
-) if you don't already have docker installed on your machine. NOTE: we build
-multi-platform images to support both x86_64 and Apple silicon hardware.
-`docker pull` should download the corresponding image for your architecture,
-but you can specify with `--platform` (e.g. `--platform linux/amd64`) if
-needed. We build Docker images for all pushes to `main`. We tag each image with
-the corresponding short commit hash (e.g. `fbc7a69`) and the application
-version (e.g. `0.5.5-dev1`). We also tag the most recent image with `latest`.
-To leverage this, `docker pull` from our image repository. ```bash docker pull
-quay.io/unstructured-io/unstructured:latest ``` Once pulled, you can create a
-container from this image and shell to it. ```bash # create the container
-docker run -dt --name unstructured quay.io/unstructured-io/unstructured:latest
-# this will drop you into a bash shell where the Docker image is running docker
-exec -it unstructured bash ``` You can also build your own Docker image. If you
-only plan on parsing one type of data you can speed up building the image by
-commenting out some of the packages/requirements necessary for other data
-types. See Dockerfile to know which lines are necessary for your use case.
-```bash make docker-build # this will drop you into a bash shell where the
-Docker image is running make docker-start-bash ``` Once in the running
-container, you can try things out directly in Python interpreter's interactive
-mode. ```bash # this will drop you into a python console so you can run the
-below partition functions python3 >>> from unstructured.partition.pdf import
-partition_pdf >>> elements = partition_pdf(filename="example-docs/layout-
-parser-paper-fast.pdf") >>> from unstructured.partition.text import
-partition_text >>> elements = partition_text(filename="example-docs/fake-
-text.txt") ``` ## :coffee: Installation Instructions for Local Development The
-following instructions are intended to help you get up and running with
-`unstructured` locally if you are planning to contribute to the project. *
-Using `pyenv` to manage virtualenv's is recommended but not necessary * Mac
-install instructions. See [here](https://github.com/Unstructured-IO/
-community#mac--homebrew) for more detailed instructions. * `brew install pyenv-
-virtualenv` * `pyenv install 3.8.15` * Linux instructions are available [here]
-(https://github.com/Unstructured-IO/community#linux). * Create a virtualenv to
-work in and activate it, e.g. for one named `unstructured`: `pyenv virtualenv
-3.8.15 unstructured`
+tensorboard>=2.12.2` - `pip install "detectron2@git+https://github.com/
+facebookresearch/detectron2.git@e2ce8dc#egg=detectron2"` At this point, you
+should be able to run the following code: ```python from
+unstructured.partition.auto import partition elements = partition
+(filename="example-docs/fake-email.eml") print("\n\n".join([str(el) for el in
+elements])) ``` And if you installed with `local-inference`, you should be able
+to run this as well: ```python from unstructured.partition.auto import
+partition elements = partition("example-docs/layout-parser-paper.pdf") print
+("\n\n".join([str(el) for el in elements])) ``` ## :dizzy: Instructions for
+using the docker image The following instructions are intended to help you get
+up and running using Docker to interact with `unstructured`. See [here](https:/
+/docs.docker.com/get-docker/) if you don't already have docker installed on
+your machine. NOTE: we build multi-platform images to support both x86_64 and
+Apple silicon hardware. `docker pull` should download the corresponding image
+for your architecture, but you can specify with `--platform` (e.g. `--platform
+linux/amd64`) if needed. We build Docker images for all pushes to `main`. We
+tag each image with the corresponding short commit hash (e.g. `fbc7a69`) and
+the application version (e.g. `0.5.5-dev1`). We also tag the most recent image
+with `latest`. To leverage this, `docker pull` from our image repository.
+```bash docker pull quay.io/unstructured-io/unstructured:latest ``` Once
+pulled, you can create a container from this image and shell to it. ```bash #
+create the container docker run -dt --name unstructured quay.io/unstructured-
+io/unstructured:latest # this will drop you into a bash shell where the Docker
+image is running docker exec -it unstructured bash ``` You can also build your
+own Docker image. If you only plan on parsing one type of data you can speed up
+building the image by commenting out some of the packages/requirements
+necessary for other data types. See Dockerfile to know which lines are
+necessary for your use case. ```bash make docker-build # this will drop you
+into a bash shell where the Docker image is running make docker-start-bash ```
+Once in the running container, you can try things out directly in Python
+interpreter's interactive mode. ```bash # this will drop you into a python
+console so you can run the below partition functions python3 >>> from
+unstructured.partition.pdf import partition_pdf >>> elements = partition_pdf
+(filename="example-docs/layout-parser-paper-fast.pdf") >>> from
+unstructured.partition.text import partition_text >>> elements = partition_text
+(filename="example-docs/fake-text.txt") ``` ## :coffee: Installation
+Instructions for Local Development The following instructions are intended to
+help you get up and running with `unstructured` locally if you are planning to
+contribute to the project. * Using `pyenv` to manage virtualenv's is
+recommended but not necessary * Mac install instructions. See [here](https://
+github.com/Unstructured-IO/community#mac--homebrew) for more detailed
+instructions. * `brew install pyenv-virtualenv` * `pyenv install 3.8.15` *
+Linux instructions are available [here](https://github.com/Unstructured-IO/
+community#linux). * Create a virtualenv to work in and activate it, e.g. for
+one named `unstructured`: `pyenv virtualenv 3.8.15 unstructured`
 `pyenv activate unstructured` * Run `make install` * Optional: * To install
 models and dependencies for processing images and PDFs locally, run `make
 install-local-inference`. * For processing image files, `tesseract` is
 required. See [here](https://tesseract-ocr.github.io/tessdoc/Installation.html)
 for installation instructions. * For processing PDF files, `tesseract` and
 `poppler` are required. The [pdf2image docs](https://pdf2image.readthedocs.io/
 en/latest/installation.html) have instructions on installing `poppler` across
```

### Comparing `unstructured-0.6.3/setup.py` & `unstructured-0.6.4/setup.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.3/test_unstructured/nlp/mock_nltk.py` & `unstructured-0.6.4/test_unstructured/nlp/mock_nltk.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.3/test_unstructured/nlp/test_tokenize.py` & `unstructured-0.6.4/test_unstructured/nlp/test_tokenize.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.3/test_unstructured/test_utils.py` & `unstructured-0.6.4/test_unstructured/test_utils.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.3/unstructured/cleaners/core.py` & `unstructured-0.6.4/unstructured/cleaners/core.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.3/unstructured/cleaners/extract.py` & `unstructured-0.6.4/unstructured/cleaners/extract.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.3/unstructured/cleaners/translate.py` & `unstructured-0.6.4/unstructured/cleaners/translate.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.3/unstructured/documents/base.py` & `unstructured-0.6.4/unstructured/documents/base.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.3/unstructured/documents/elements.py` & `unstructured-0.6.4/unstructured/documents/elements.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.3/unstructured/documents/email_elements.py` & `unstructured-0.6.4/unstructured/documents/email_elements.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.3/unstructured/documents/html.py` & `unstructured-0.6.4/unstructured/documents/html.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.3/unstructured/documents/xml.py` & `unstructured-0.6.4/unstructured/documents/xml.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.3/unstructured/file_utils/exploration.py` & `unstructured-0.6.4/unstructured/file_utils/exploration.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.3/unstructured/file_utils/file_conversion.py` & `unstructured-0.6.4/unstructured/file_utils/file_conversion.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.3/unstructured/file_utils/filetype.py` & `unstructured-0.6.4/unstructured/file_utils/filetype.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.3/unstructured/file_utils/metadata.py` & `unstructured-0.6.4/unstructured/file_utils/metadata.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.3/unstructured/ingest/connector/azure.py` & `unstructured-0.6.4/unstructured/ingest/connector/azure.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.3/unstructured/ingest/connector/biomed.py` & `unstructured-0.6.4/unstructured/ingest/connector/biomed.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.3/unstructured/ingest/connector/fsspec.py` & `unstructured-0.6.4/unstructured/ingest/connector/fsspec.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.3/unstructured/ingest/connector/git.py` & `unstructured-0.6.4/unstructured/ingest/connector/git.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.3/unstructured/ingest/connector/github.py` & `unstructured-0.6.4/unstructured/ingest/connector/github.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.3/unstructured/ingest/connector/gitlab.py` & `unstructured-0.6.4/unstructured/ingest/connector/gitlab.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.3/unstructured/ingest/connector/google_drive.py` & `unstructured-0.6.4/unstructured/ingest/connector/google_drive.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.3/unstructured/ingest/connector/local.py` & `unstructured-0.6.4/unstructured/ingest/connector/local.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.3/unstructured/ingest/connector/reddit.py` & `unstructured-0.6.4/unstructured/ingest/connector/reddit.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.3/unstructured/ingest/connector/s3.py` & `unstructured-0.6.4/unstructured/ingest/connector/s3.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.3/unstructured/ingest/connector/slack.py` & `unstructured-0.6.4/unstructured/ingest/connector/slack.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.3/unstructured/ingest/connector/wikipedia.py` & `unstructured-0.6.4/unstructured/ingest/connector/wikipedia.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.3/unstructured/ingest/doc_processor/generalized.py` & `unstructured-0.6.4/unstructured/ingest/doc_processor/generalized.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.3/unstructured/ingest/interfaces.py` & `unstructured-0.6.4/unstructured/ingest/interfaces.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.3/unstructured/ingest/main.py` & `unstructured-0.6.4/unstructured/ingest/main.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.3/unstructured/nlp/english-words.txt` & `unstructured-0.6.4/unstructured/nlp/english-words.txt`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.3/unstructured/nlp/english_words.py` & `unstructured-0.6.4/unstructured/nlp/english_words.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.3/unstructured/nlp/patterns.py` & `unstructured-0.6.4/unstructured/nlp/patterns.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.3/unstructured/nlp/tokenize.py` & `unstructured-0.6.4/unstructured/nlp/tokenize.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.3/unstructured/partition/__init__.py` & `unstructured-0.6.4/unstructured/partition/__init__.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.3/unstructured/partition/api.py` & `unstructured-0.6.4/unstructured/partition/api.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.3/unstructured/partition/auto.py` & `unstructured-0.6.4/unstructured/partition/auto.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.3/unstructured/partition/common.py` & `unstructured-0.6.4/unstructured/partition/common.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.3/unstructured/partition/doc.py` & `unstructured-0.6.4/unstructured/partition/doc.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.3/unstructured/partition/docx.py` & `unstructured-0.6.4/unstructured/partition/docx.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.3/unstructured/partition/email.py` & `unstructured-0.6.4/unstructured/partition/email.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.3/unstructured/partition/epub.py` & `unstructured-0.6.4/unstructured/partition/epub.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.3/unstructured/partition/html.py` & `unstructured-0.6.4/unstructured/partition/html.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.3/unstructured/partition/image.py` & `unstructured-0.6.4/unstructured/partition/image.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,12 @@
 from typing import List, Optional
 
-import pytesseract
-from PIL import Image
-
 from unstructured.documents.elements import Element
 from unstructured.partition.common import exactly_one
 from unstructured.partition.pdf import partition_pdf_or_image
-from unstructured.partition.text import partition_text
-
-VALID_STRATEGIES = ["hi_res", "ocr_only"]
 
 
 def partition_image(
     filename: str = "",
     file: Optional[bytes] = None,
     url: Optional[str] = None,
     template: Optional[str] = None,
@@ -38,39 +32,26 @@
     token
         A string defining the authentication token for a self-host url, if applicable.
     ocr_languages
         The languages to use for the Tesseract agent. To use a language, you'll first need
         to install the appropriate Tesseract language pack.
     strategy
         The strategy to use for partitioning the PDF. Valid strategies are "hi_res" and
-        "ocr_only". When using the "hi_res" strategy, the function  ses a layout detection
-        model if to identify document elements. When using the "ocr_only strategy",
-        partition_image simply extracts the text from the document and processes it.
+        "ocr_only". When using the "hi_res" strategy, the function uses a layout detection
+        model if to identify document elements. When using the "ocr_only" strategy,
+        partition_image simply extracts the text from the document using OCR and processes it.
     """
     exactly_one(filename=filename, file=file)
 
-    if strategy == "hi_res":
-        if template is None:
-            template = "layout/image"
-        return partition_pdf_or_image(
-            filename=filename,
-            file=file,
-            url=url,
-            template=template,
-            token=token,
-            include_page_breaks=include_page_breaks,
-            ocr_languages=ocr_languages,
-        )
-
-    elif strategy == "ocr_only":
-        if file is not None:
-            image = Image.open(file)
-            text = pytesseract.image_to_string(image, config=f"-l '{ocr_languages}'")
-        else:
-            text = pytesseract.image_to_string(filename, config=f"-l '{ocr_languages}'")
-        return partition_text(text=text)
-
-    else:
-        raise ValueError(
-            f"{strategy} is not a valid strategy for partition_image. "
-            f"Choose one of {VALID_STRATEGIES}.",
-        )
+    if template is None:
+        template = "layout/image"
+
+    return partition_pdf_or_image(
+        filename=filename,
+        file=file,
+        url=url,
+        template=template,
+        token=token,
+        include_page_breaks=include_page_breaks,
+        ocr_languages=ocr_languages,
+        strategy=strategy,
+    )
```

### Comparing `unstructured-0.6.3/unstructured/partition/json.py` & `unstructured-0.6.4/unstructured/partition/json.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.3/unstructured/partition/md.py` & `unstructured-0.6.4/unstructured/partition/md.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.3/unstructured/partition/msg.py` & `unstructured-0.6.4/unstructured/partition/msg.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.3/unstructured/partition/odt.py` & `unstructured-0.6.4/unstructured/partition/odt.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.3/unstructured/partition/pdf.py` & `unstructured-0.6.4/unstructured/partition/pdf.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 import re
 import warnings
 from typing import BinaryIO, List, Optional, cast
 
+import pdf2image
+import pytesseract
 from pdfminer.high_level import extract_pages
-from pdfminer.pdfpage import PDFPage, PDFTextExtractionNotAllowed
 from pdfminer.utils import open_filename
+from PIL import Image
 
 from unstructured.cleaners.core import clean_extra_whitespace
 from unstructured.documents.elements import Element, ElementMetadata, PageBreak
-from unstructured.logger import logger
 from unstructured.nlp.patterns import PARAGRAPH_PATTERN
 from unstructured.partition import _partition_via_api
 from unstructured.partition.common import (
     add_element_metadata,
     document_to_element_list,
     exactly_one,
 )
+from unstructured.partition.strategies import determine_pdf_or_image_strategy
 from unstructured.partition.text import partition_text
-from unstructured.utils import dependency_exists, requires_dependencies
+from unstructured.utils import requires_dependencies
 
 
 def partition_pdf(
     filename: str = "",
     file: Optional[bytes] = None,
     url: Optional[str] = None,
     template: str = "layout/pdf",
@@ -44,17 +46,20 @@
         if using the API).
     url
         A string endpoint to self-host an inference API, if desired. If None, local inference will
         be used.
     token
         A string defining the authentication token for a self-host url, if applicable.
     strategy
-        The strategy to use for partitioning the PDF. Uses a layout detection model if set
-        to 'hi_res', otherwise partition_pdf simply extracts the text from the document
-        and processes it.
+        The strategy to use for partitioning the PDF. Valid strategies are "hi_res",
+        "ocr_only", and "fast". When using the "hi_res" strategy, the function uses
+        a layout detection model to identify document elements. When using the
+        "ocr_only" strategy, partition_image simply extracts the text from the
+        document using OCR and processes it. If the "fast" strategy is used, the text
+        is extracted directly from the PDF.
     infer_table_structure
         Only applicable if `strategy=hi_res`.
         If True, any Table elements that are extracted will also have a metadata field
         named "text_as_html" where the table's text content is rendered into an html string.
         I.e., rows and cells are preserved.
         Whether True or False, the "text" field is always present in any Table element
         and is the text content of the table (no structure).
@@ -100,78 +105,53 @@
         # function.
         route_args = template.strip("/").split("/")
         is_image = route_args[-1] == "image"
         out_template: Optional[str] = template
         if route_args[0] == "layout":
             out_template = None
 
-        fallback_to_fast = False
-        fallback_to_hi_res = False
-
-        detectron2_installed = dependency_exists("detectron2")
-        if is_image:
-            pdf_text_extractable = False
-        else:
-            pdf_text_extractable = is_pdf_text_extractable(filename=filename, file=file)
-            if file is not None:
-                file.seek(0)  # type: ignore
-
-        if not detectron2_installed and not pdf_text_extractable:
-            raise ValueError(
-                "detectron2 is not installed and the text of the PDF is not extractable. "
-                "To process this file, install detectron2 or remove copy protection from the PDF.",
-            )
-
-        if not pdf_text_extractable:
-            fallback_to_hi_res = strategy == "fast"
-
-        if not detectron2_installed:
-            fallback_to_fast = strategy == "hi_res"
-
-        if (strategy == "hi_res" or fallback_to_hi_res) and not fallback_to_fast:
-            if strategy == "fast":
-                logger.warning(
-                    "PDF text is not extractable. Cannot use the fast partitioning "
-                    "strategy. Falling back to partitioning with the hi_res strategy.",
-                )
+        strategy = determine_pdf_or_image_strategy(
+            strategy,
+            filename=filename,
+            file=file,
+            is_image=is_image,
+        )
 
+        if strategy == "hi_res":
             # NOTE(robinson): Catches a UserWarning that occurs when detectron is called
             with warnings.catch_warnings():
                 warnings.simplefilter("ignore")
                 layout_elements = _partition_pdf_or_image_local(
                     filename=filename,
                     file=file,
                     template=out_template,
                     is_image=is_image,
                     infer_table_structure=infer_table_structure,
                     include_page_breaks=True,
                     ocr_languages=ocr_languages,
                 )
 
-        elif (strategy == "fast" or fallback_to_fast) and not fallback_to_hi_res:
-            if strategy == "hi_res":
-                logger.warning(
-                    "detectron2 is not installed. Cannot use the hi_res partitioning "
-                    "strategy. Falling back to partitioning with the fast strategy.",
-                )
-            if infer_table_structure:
-                logger.warning(
-                    "Table extraction was selected, but is being ignored while using the fast "
-                    "strategy.",
-                )
-
+        elif strategy == "fast":
             return _partition_pdf_with_pdfminer(
                 filename=filename,
                 file=file,
                 include_page_breaks=include_page_breaks,
                 encoding=encoding,
             )
 
-        else:
-            raise ValueError(f"{strategy} is an invalid parsing strategy for PDFs")
+        elif strategy == "ocr_only":
+            # NOTE(robinson): Catches file conversion warnings when running with PDFs
+            with warnings.catch_warnings():
+                return _partition_pdf_or_image_with_ocr(
+                    filename=filename,
+                    file=file,
+                    include_page_breaks=include_page_breaks,
+                    ocr_languages=ocr_languages,
+                    is_image=is_image,
+                )
 
     else:
         # NOTE(alan): Remove these lines after different models are handled by routing
         if template == "checkbox":
             template = "layout/pdf"
         # NOTE(alan): Remove after different models are handled by routing
         data = {"model": "checkbox"} if (template == "checkbox") else None
@@ -314,27 +294,43 @@
 
         if include_page_breaks:
             elements.append(PageBreak())
 
     return elements
 
 
-def is_pdf_text_extractable(filename: str = "", file: Optional[bytes] = None):
-    """Checks to see if the text from a PDF document is extractable. Sometimes the
-    text is not extractable due to PDF security settings."""
-    exactly_one(filename=filename, file=file)
+def _partition_pdf_or_image_with_ocr(
+    filename: str = "",
+    file: Optional[bytes] = None,
+    include_page_breaks: bool = False,
+    ocr_languages: str = "eng",
+    is_image: bool = False,
+):
+    """Partitions and image or PDF using Tesseract OCR. For PDFs, each page is converted
+    to an image prior to processing."""
+    if is_image:
+        if file is not None:
+            image = Image.open(file)
+            text = pytesseract.image_to_string(image, config=f"-l '{ocr_languages}'")
+        else:
+            text = pytesseract.image_to_string(filename, config=f"-l '{ocr_languages}'")
+        elements = partition_text(text=text)
+    else:
+        elements = []
+        if file is not None:
+            document = pdf2image.convert_from_bytes(file.read())  # type: ignore
+            file.seek(0)  # type: ignore
+        else:
+            document = pdf2image.convert_from_path(filename)
 
-    def _fp_is_extractable(fp):
-        try:
-            next(PDFPage.get_pages(fp, check_extractable=True))
-            extractable = True
-        except PDFTextExtractionNotAllowed:
-            extractable = False
-        return extractable
+        for i, image in enumerate(document):
+            metadata = ElementMetadata(filename=filename, page_number=i + 1)
+            text = pytesseract.image_to_string(image, config=f"-l '{ocr_languages}'")
+
+            _elements = partition_text(text=text)
+            for element in _elements:
+                element.metadata = metadata
+                elements.append(element)
 
-    if filename:
-        with open_filename(filename, "rb") as fp:
-            fp = cast(BinaryIO, fp)
-            return _fp_is_extractable(fp)
-    elif file:
-        fp = cast(BinaryIO, file)
-        return _fp_is_extractable(fp)
+            if include_page_breaks:
+                elements.append(PageBreak())
+    return elements
```

### Comparing `unstructured-0.6.3/unstructured/partition/ppt.py` & `unstructured-0.6.4/unstructured/partition/ppt.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.3/unstructured/partition/pptx.py` & `unstructured-0.6.4/unstructured/partition/pptx.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.3/unstructured/partition/rtf.py` & `unstructured-0.6.4/unstructured/partition/rtf.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.3/unstructured/partition/text.py` & `unstructured-0.6.4/unstructured/partition/text.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.3/unstructured/partition/text_type.py` & `unstructured-0.6.4/unstructured/partition/text_type.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.3/unstructured/staging/argilla.py` & `unstructured-0.6.4/unstructured/staging/argilla.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.3/unstructured/staging/base.py` & `unstructured-0.6.4/unstructured/staging/base.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.3/unstructured/staging/baseplate.py` & `unstructured-0.6.4/unstructured/staging/baseplate.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.3/unstructured/staging/datasaur.py` & `unstructured-0.6.4/unstructured/staging/datasaur.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.3/unstructured/staging/huggingface.py` & `unstructured-0.6.4/unstructured/staging/huggingface.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.3/unstructured/staging/label_box.py` & `unstructured-0.6.4/unstructured/staging/label_box.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.3/unstructured/staging/label_studio.py` & `unstructured-0.6.4/unstructured/staging/label_studio.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.3/unstructured/staging/prodigy.py` & `unstructured-0.6.4/unstructured/staging/prodigy.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.3/unstructured/utils.py` & `unstructured-0.6.4/unstructured/utils.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.3/unstructured.egg-info/PKG-INFO` & `unstructured-0.6.4/unstructured.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unstructured
-Version: 0.6.3
+Version: 0.6.4
 Summary: A library that prepares raw documents for downstream ML tasks.
 Home-page: https://github.com/Unstructured-IO/unstructured
 Author: Unstructured Technologies
 Author-email: devops@unstructuredai.io
 License: Apache-2.0
 Description: <h3 align="center">
           <img
@@ -79,14 +79,15 @@
           Depending on what document types you're parsing, you may not need all of these.
             - `libmagic-dev` (filetype detection)
             - `poppler-utils` (images and PDFs)
             - `tesseract-ocr` (images and PDFs)
             - `libreoffice` (MS Office docs)
         - If you are parsing PDFs, run the following to install the `detectron2` model, which
           `unstructured` uses for layout detection:
+            - `pip install tensorboard>=2.12.2`
             - `pip install "detectron2@git+https://github.com/facebookresearch/detectron2.git@e2ce8dc#egg=detectron2"`
         
         At this point, you should be able to run the following code:
         
         ```python
         from unstructured.partition.auto import partition
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: unstructured Version: 0.6.3 Summary: A library that
+Metadata-Version: 2.1 Name: unstructured Version: 0.6.4 Summary: A library that
 prepares raw documents for downstream ML tasks. Home-page: https://github.com/
 Unstructured-IO/unstructured Author: Unstructured Technologies Author-email:
 devops@unstructuredai.io License: Apache-2.0 Description:
 **** [https://raw.githubusercontent.com/Unstructured-IO/unstructured/main/img/
                           unstructured_logo.png] ****
  ![https://pypi.python.org/pypi/unstructured/](https://img.shields.io/pypi/l/
    unstructured.svg) ![https://pypi.python.org/pypi/unstructured/](https://
@@ -46,59 +46,59 @@
 need to process PDFs or images, you can run `pip install unstructured` -
 Install the following system dependencies if they are not already available on
 your system. Depending on what document types you're parsing, you may not need
 all of these. - `libmagic-dev` (filetype detection) - `poppler-utils` (images
 and PDFs) - `tesseract-ocr` (images and PDFs) - `libreoffice` (MS Office docs)
 - If you are parsing PDFs, run the following to install the `detectron2` model,
 which `unstructured` uses for layout detection: - `pip install
-"detectron2@git+https://github.com/facebookresearch/
-detectron2.git@e2ce8dc#egg=detectron2"` At this point, you should be able to
-run the following code: ```python from unstructured.partition.auto import
-partition elements = partition(filename="example-docs/fake-email.eml") print
-("\n\n".join([str(el) for el in elements])) ``` And if you installed with
-`local-inference`, you should be able to run this as well: ```python from
-unstructured.partition.auto import partition elements = partition("example-
-docs/layout-parser-paper.pdf") print("\n\n".join([str(el) for el in elements]))
-``` ## :dizzy: Instructions for using the docker image The following
-instructions are intended to help you get up and running using Docker to
-interact with `unstructured`. See [here](https://docs.docker.com/get-docker/
-) if you don't already have docker installed on your machine. NOTE: we build
-multi-platform images to support both x86_64 and Apple silicon hardware.
-`docker pull` should download the corresponding image for your architecture,
-but you can specify with `--platform` (e.g. `--platform linux/amd64`) if
-needed. We build Docker images for all pushes to `main`. We tag each image with
-the corresponding short commit hash (e.g. `fbc7a69`) and the application
-version (e.g. `0.5.5-dev1`). We also tag the most recent image with `latest`.
-To leverage this, `docker pull` from our image repository. ```bash docker pull
-quay.io/unstructured-io/unstructured:latest ``` Once pulled, you can create a
-container from this image and shell to it. ```bash # create the container
-docker run -dt --name unstructured quay.io/unstructured-io/unstructured:latest
-# this will drop you into a bash shell where the Docker image is running docker
-exec -it unstructured bash ``` You can also build your own Docker image. If you
-only plan on parsing one type of data you can speed up building the image by
-commenting out some of the packages/requirements necessary for other data
-types. See Dockerfile to know which lines are necessary for your use case.
-```bash make docker-build # this will drop you into a bash shell where the
-Docker image is running make docker-start-bash ``` Once in the running
-container, you can try things out directly in Python interpreter's interactive
-mode. ```bash # this will drop you into a python console so you can run the
-below partition functions python3 >>> from unstructured.partition.pdf import
-partition_pdf >>> elements = partition_pdf(filename="example-docs/layout-
-parser-paper-fast.pdf") >>> from unstructured.partition.text import
-partition_text >>> elements = partition_text(filename="example-docs/fake-
-text.txt") ``` ## :coffee: Installation Instructions for Local Development The
-following instructions are intended to help you get up and running with
-`unstructured` locally if you are planning to contribute to the project. *
-Using `pyenv` to manage virtualenv's is recommended but not necessary * Mac
-install instructions. See [here](https://github.com/Unstructured-IO/
-community#mac--homebrew) for more detailed instructions. * `brew install pyenv-
-virtualenv` * `pyenv install 3.8.15` * Linux instructions are available [here]
-(https://github.com/Unstructured-IO/community#linux). * Create a virtualenv to
-work in and activate it, e.g. for one named `unstructured`: `pyenv virtualenv
-3.8.15 unstructured`
+tensorboard>=2.12.2` - `pip install "detectron2@git+https://github.com/
+facebookresearch/detectron2.git@e2ce8dc#egg=detectron2"` At this point, you
+should be able to run the following code: ```python from
+unstructured.partition.auto import partition elements = partition
+(filename="example-docs/fake-email.eml") print("\n\n".join([str(el) for el in
+elements])) ``` And if you installed with `local-inference`, you should be able
+to run this as well: ```python from unstructured.partition.auto import
+partition elements = partition("example-docs/layout-parser-paper.pdf") print
+("\n\n".join([str(el) for el in elements])) ``` ## :dizzy: Instructions for
+using the docker image The following instructions are intended to help you get
+up and running using Docker to interact with `unstructured`. See [here](https:/
+/docs.docker.com/get-docker/) if you don't already have docker installed on
+your machine. NOTE: we build multi-platform images to support both x86_64 and
+Apple silicon hardware. `docker pull` should download the corresponding image
+for your architecture, but you can specify with `--platform` (e.g. `--platform
+linux/amd64`) if needed. We build Docker images for all pushes to `main`. We
+tag each image with the corresponding short commit hash (e.g. `fbc7a69`) and
+the application version (e.g. `0.5.5-dev1`). We also tag the most recent image
+with `latest`. To leverage this, `docker pull` from our image repository.
+```bash docker pull quay.io/unstructured-io/unstructured:latest ``` Once
+pulled, you can create a container from this image and shell to it. ```bash #
+create the container docker run -dt --name unstructured quay.io/unstructured-
+io/unstructured:latest # this will drop you into a bash shell where the Docker
+image is running docker exec -it unstructured bash ``` You can also build your
+own Docker image. If you only plan on parsing one type of data you can speed up
+building the image by commenting out some of the packages/requirements
+necessary for other data types. See Dockerfile to know which lines are
+necessary for your use case. ```bash make docker-build # this will drop you
+into a bash shell where the Docker image is running make docker-start-bash ```
+Once in the running container, you can try things out directly in Python
+interpreter's interactive mode. ```bash # this will drop you into a python
+console so you can run the below partition functions python3 >>> from
+unstructured.partition.pdf import partition_pdf >>> elements = partition_pdf
+(filename="example-docs/layout-parser-paper-fast.pdf") >>> from
+unstructured.partition.text import partition_text >>> elements = partition_text
+(filename="example-docs/fake-text.txt") ``` ## :coffee: Installation
+Instructions for Local Development The following instructions are intended to
+help you get up and running with `unstructured` locally if you are planning to
+contribute to the project. * Using `pyenv` to manage virtualenv's is
+recommended but not necessary * Mac install instructions. See [here](https://
+github.com/Unstructured-IO/community#mac--homebrew) for more detailed
+instructions. * `brew install pyenv-virtualenv` * `pyenv install 3.8.15` *
+Linux instructions are available [here](https://github.com/Unstructured-IO/
+community#linux). * Create a virtualenv to work in and activate it, e.g. for
+one named `unstructured`: `pyenv virtualenv 3.8.15 unstructured`
 `pyenv activate unstructured` * Run `make install` * Optional: * To install
 models and dependencies for processing images and PDFs locally, run `make
 install-local-inference`. * For processing image files, `tesseract` is
 required. See [here](https://tesseract-ocr.github.io/tessdoc/Installation.html)
 for installation instructions. * For processing PDF files, `tesseract` and
 `poppler` are required. The [pdf2image docs](https://pdf2image.readthedocs.io/
 en/latest/installation.html) have instructions on installing `poppler` across
```

### Comparing `unstructured-0.6.3/unstructured.egg-info/SOURCES.txt` & `unstructured-0.6.4/unstructured.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -74,14 +74,15 @@
 unstructured/partition/md.py
 unstructured/partition/msg.py
 unstructured/partition/odt.py
 unstructured/partition/pdf.py
 unstructured/partition/ppt.py
 unstructured/partition/pptx.py
 unstructured/partition/rtf.py
+unstructured/partition/strategies.py
 unstructured/partition/text.py
 unstructured/partition/text_type.py
 unstructured/staging/__init__.py
 unstructured/staging/argilla.py
 unstructured/staging/base.py
 unstructured/staging/baseplate.py
 unstructured/staging/datasaur.py
```

