# Comparing `tmp/scGPT-0.1.0.tar.gz` & `tmp/scGPT-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scGPT-0.1.0.tar", max compression
+gzip compressed data, was "scGPT-0.1.1.tar", max compression
```

## Comparing `scGPT-0.1.0.tar` & `scGPT-0.1.1.tar`

### file list

```diff
@@ -1,26 +1,27 @@
--rw-r--r--   0        0        0     1062 2023-05-02 17:04:22.123385 scGPT-0.1.0/LICENSE
--rw-r--r--   0        0        0      818 2023-05-02 21:56:49.466732 scGPT-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      580 2023-05-02 19:00:34.630742 scGPT-0.1.0/scgpt/__init__.py
--rw-r--r--   0        0        0     7497 2023-05-02 17:04:22.215385 scGPT-0.1.0/scgpt/data_collator.py
--rw-r--r--   0        0        0     3573 2023-05-02 17:04:22.191385 scGPT-0.1.0/scgpt/data_sampler.py
--rw-r--r--   0        0        0     1068 2023-05-02 17:04:22.219385 scGPT-0.1.0/scgpt/loss.py
--rw-r--r--   0        0        0      222 2023-05-02 17:04:22.151385 scGPT-0.1.0/scgpt/model/__init__.py
--rw-r--r--   0        0        0     2393 2023-05-02 17:04:22.155385 scGPT-0.1.0/scgpt/model/dsbn.py
--rw-r--r--   0        0        0    16188 2023-05-02 22:28:23.358872 scGPT-0.1.0/scgpt/model/generation_model.py
--rw-r--r--   0        0        0      469 2023-05-02 17:04:22.159385 scGPT-0.1.0/scgpt/model/grad_reverse.py
--rw-r--r--   0        0        0    39049 2023-05-06 15:06:34.399248 scGPT-0.1.0/scgpt/model/model.py
--rw-r--r--   0        0        0    10954 2023-05-02 17:12:48.502508 scGPT-0.1.0/scgpt/preprocess.py
--rw-r--r--   0        0        0      611 2023-05-02 17:04:22.203385 scGPT-0.1.0/scgpt/scbank/__init__.py
--rw-r--r--   0        0        0     4044 2023-05-02 17:04:22.207385 scGPT-0.1.0/scgpt/scbank/data.py
--rw-r--r--   0        0        0    29625 2023-05-02 17:14:04.842980 scGPT-0.1.0/scgpt/scbank/databank.py
--rw-r--r--   0        0        0      129 2023-05-02 17:04:22.211385 scGPT-0.1.0/scgpt/scbank/monitor.py
--rw-r--r--   0        0        0      844 2023-05-02 17:04:22.203385 scGPT-0.1.0/scgpt/scbank/setting.py
--rw-r--r--   0        0        0       30 2023-05-02 17:04:22.167385 scGPT-0.1.0/scgpt/tokenizer/__init__.py
--rw-r--r--   0        0        0   761373 2023-05-02 17:04:22.175385 scGPT-0.1.0/scgpt/tokenizer/default_cellxgene_vocab.json
--rw-r--r--   0        0        0   940574 2023-05-02 17:04:22.179385 scGPT-0.1.0/scgpt/tokenizer/default_gene_vocab.json
--rw-r--r--   0        0        0    13901 2023-05-02 17:04:22.163385 scGPT-0.1.0/scgpt/tokenizer/gene_tokenizer.py
--rw-r--r--   0        0        0        0 2023-05-02 17:04:22.223385 scGPT-0.1.0/scgpt/trainer.py
--rw-r--r--   0        0        0       20 2023-05-02 17:04:22.227385 scGPT-0.1.0/scgpt/utils/__init__.py
--rw-r--r--   0        0        0    10070 2023-05-02 17:15:21.375451 scGPT-0.1.0/scgpt/utils/util.py
--rw-r--r--   0        0        0     1086 1970-01-01 00:00:00.000000 scGPT-0.1.0/setup.py
--rw-r--r--   0        0        0     1010 1970-01-01 00:00:00.000000 scGPT-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-05-02 17:04:22.123385 scGPT-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2521 2023-05-08 16:12:32.952102 scGPT-0.1.1/README.md
+-rw-r--r--   0        0        0      904 2023-05-08 16:50:40.355285 scGPT-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      580 2023-05-02 19:00:34.630742 scGPT-0.1.1/scgpt/__init__.py
+-rw-r--r--   0        0        0     7497 2023-05-02 17:04:22.215385 scGPT-0.1.1/scgpt/data_collator.py
+-rw-r--r--   0        0        0     3573 2023-05-02 17:04:22.191385 scGPT-0.1.1/scgpt/data_sampler.py
+-rw-r--r--   0        0        0     1068 2023-05-02 17:04:22.219385 scGPT-0.1.1/scgpt/loss.py
+-rw-r--r--   0        0        0      222 2023-05-02 17:04:22.151385 scGPT-0.1.1/scgpt/model/__init__.py
+-rw-r--r--   0        0        0     2393 2023-05-02 17:04:22.155385 scGPT-0.1.1/scgpt/model/dsbn.py
+-rw-r--r--   0        0        0    16188 2023-05-02 22:28:23.358872 scGPT-0.1.1/scgpt/model/generation_model.py
+-rw-r--r--   0        0        0      469 2023-05-02 17:04:22.159385 scGPT-0.1.1/scgpt/model/grad_reverse.py
+-rw-r--r--   0        0        0    39049 2023-05-06 15:06:34.399248 scGPT-0.1.1/scgpt/model/model.py
+-rw-r--r--   0        0        0    10954 2023-05-02 17:12:48.502508 scGPT-0.1.1/scgpt/preprocess.py
+-rw-r--r--   0        0        0      611 2023-05-02 17:04:22.203385 scGPT-0.1.1/scgpt/scbank/__init__.py
+-rw-r--r--   0        0        0     4044 2023-05-02 17:04:22.207385 scGPT-0.1.1/scgpt/scbank/data.py
+-rw-r--r--   0        0        0    29625 2023-05-02 17:14:04.842980 scGPT-0.1.1/scgpt/scbank/databank.py
+-rw-r--r--   0        0        0      129 2023-05-02 17:04:22.211385 scGPT-0.1.1/scgpt/scbank/monitor.py
+-rw-r--r--   0        0        0      844 2023-05-02 17:04:22.203385 scGPT-0.1.1/scgpt/scbank/setting.py
+-rw-r--r--   0        0        0       30 2023-05-02 17:04:22.167385 scGPT-0.1.1/scgpt/tokenizer/__init__.py
+-rw-r--r--   0        0        0   761373 2023-05-02 17:04:22.175385 scGPT-0.1.1/scgpt/tokenizer/default_cellxgene_vocab.json
+-rw-r--r--   0        0        0   940574 2023-05-02 17:04:22.179385 scGPT-0.1.1/scgpt/tokenizer/default_gene_vocab.json
+-rw-r--r--   0        0        0    13901 2023-05-02 17:04:22.163385 scGPT-0.1.1/scgpt/tokenizer/gene_tokenizer.py
+-rw-r--r--   0        0        0        0 2023-05-02 17:04:22.223385 scGPT-0.1.1/scgpt/trainer.py
+-rw-r--r--   0        0        0       20 2023-05-02 17:04:22.227385 scGPT-0.1.1/scgpt/utils/__init__.py
+-rw-r--r--   0        0        0    10070 2023-05-02 17:15:21.375451 scGPT-0.1.1/scgpt/utils/util.py
+-rw-r--r--   0        0        0     3667 1970-01-01 00:00:00.000000 scGPT-0.1.1/setup.py
+-rw-r--r--   0        0        0     3573 1970-01-01 00:00:00.000000 scGPT-0.1.1/PKG-INFO
```

### Comparing `scGPT-0.1.0/LICENSE` & `scGPT-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scGPT-0.1.0/pyproject.toml` & `scGPT-0.1.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 [tool.poetry]
 name = "scGPT"
-version = "0.1.0"
+version = "0.1.1"
 description = "Large-scale generative pretrain of single cell using transformer."
 authors = ["Haotian <subercui@gmail.com>"]
+readme = "README.md"
+
+[project.urls]
+"Homepage" = "https:github.com/bowang-lab/scGPT"
 
 [tool.poetry.dependencies]
 python = ">=3.7.1,<3.11"
 pandas = "1.3.5"
 scvi-tools = "^0.16.0"
 llvmlite = "^0.38.0"
 scanpy = "^1.9.1"
```

### Comparing `scGPT-0.1.0/scgpt/__init__.py` & `scGPT-0.1.1/scgpt/__init__.py`

 * *Files identical despite different names*

### Comparing `scGPT-0.1.0/scgpt/data_collator.py` & `scGPT-0.1.1/scgpt/data_collator.py`

 * *Files identical despite different names*

### Comparing `scGPT-0.1.0/scgpt/data_sampler.py` & `scGPT-0.1.1/scgpt/data_sampler.py`

 * *Files identical despite different names*

### Comparing `scGPT-0.1.0/scgpt/loss.py` & `scGPT-0.1.1/scgpt/loss.py`

 * *Files identical despite different names*

### Comparing `scGPT-0.1.0/scgpt/model/dsbn.py` & `scGPT-0.1.1/scgpt/model/dsbn.py`

 * *Files identical despite different names*

### Comparing `scGPT-0.1.0/scgpt/model/generation_model.py` & `scGPT-0.1.1/scgpt/model/generation_model.py`

 * *Files identical despite different names*

### Comparing `scGPT-0.1.0/scgpt/model/model.py` & `scGPT-0.1.1/scgpt/model/model.py`

 * *Files identical despite different names*

### Comparing `scGPT-0.1.0/scgpt/preprocess.py` & `scGPT-0.1.1/scgpt/preprocess.py`

 * *Files identical despite different names*

### Comparing `scGPT-0.1.0/scgpt/scbank/__init__.py` & `scGPT-0.1.1/scgpt/scbank/__init__.py`

 * *Files identical despite different names*

### Comparing `scGPT-0.1.0/scgpt/scbank/data.py` & `scGPT-0.1.1/scgpt/scbank/data.py`

 * *Files identical despite different names*

### Comparing `scGPT-0.1.0/scgpt/scbank/databank.py` & `scGPT-0.1.1/scgpt/scbank/databank.py`

 * *Files identical despite different names*

### Comparing `scGPT-0.1.0/scgpt/scbank/setting.py` & `scGPT-0.1.1/scgpt/scbank/setting.py`

 * *Files identical despite different names*

### Comparing `scGPT-0.1.0/scgpt/tokenizer/default_cellxgene_vocab.json` & `scGPT-0.1.1/scgpt/tokenizer/default_cellxgene_vocab.json`

 * *Files identical despite different names*

### Comparing `scGPT-0.1.0/scgpt/tokenizer/default_gene_vocab.json` & `scGPT-0.1.1/scgpt/tokenizer/default_gene_vocab.json`

 * *Files identical despite different names*

### Comparing `scGPT-0.1.0/scgpt/tokenizer/gene_tokenizer.py` & `scGPT-0.1.1/scgpt/tokenizer/gene_tokenizer.py`

 * *Files identical despite different names*

### Comparing `scGPT-0.1.0/scgpt/utils/util.py` & `scGPT-0.1.1/scgpt/utils/util.py`

 * *Files identical despite different names*

