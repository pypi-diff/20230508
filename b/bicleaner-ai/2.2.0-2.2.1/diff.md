# Comparing `tmp/bicleaner-ai-2.2.0.tar.gz` & `tmp/bicleaner-ai-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bicleaner-ai-2.2.0.tar", last modified: Mon Mar 27 16:16:54 2023, max compression
+gzip compressed data, was "bicleaner-ai-2.2.1.tar", last modified: Mon May  8 09:15:30 2023, max compression
```

## Comparing `bicleaner-ai-2.2.0.tar` & `bicleaner-ai-2.2.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-27 16:16:54.352971 bicleaner-ai-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (122)    35147 2023-03-27 16:16:41.000000 bicleaner-ai-2.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)    65558 2023-03-27 16:16:54.348971 bicleaner-ai-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    24077 2023-03-27 16:16:41.000000 bicleaner-ai-2.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     2039 2023-03-27 16:16:41.000000 bicleaner-ai-2.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-03-27 16:16:54.352971 bicleaner-ai-2.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-27 16:16:54.344971 bicleaner-ai-2.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-27 16:16:54.348971 bicleaner-ai-2.2.0/src/bicleaner_ai/
--rwxr-xr-x   0 runner    (1001) docker     (122)      112 2023-03-27 16:16:41.000000 bicleaner-ai-2.2.0/src/bicleaner_ai/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     4547 2023-03-27 16:16:41.000000 bicleaner-ai-2.2.0/src/bicleaner_ai/bicleaner_ai_classifier.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     3580 2023-03-27 16:16:41.000000 bicleaner-ai-2.2.0/src/bicleaner_ai/bicleaner_ai_download.py
--rwxr-xr-x   0 runner    (1001) docker     (122)      624 2023-03-27 16:16:41.000000 bicleaner-ai-2.2.0/src/bicleaner_ai/bicleaner_ai_download_hf.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    16502 2023-03-27 16:16:41.000000 bicleaner-ai-2.2.0/src/bicleaner_ai/bicleaner_ai_train.py
--rw-r--r--   0 runner    (1001) docker     (122)     2964 2023-03-27 16:16:41.000000 bicleaner-ai-2.2.0/src/bicleaner_ai/calibrate.py
--rw-r--r--   0 runner    (1001) docker     (122)    13926 2023-03-27 16:16:41.000000 bicleaner-ai-2.2.0/src/bicleaner_ai/classify.py
--rw-r--r--   0 runner    (1001) docker     (122)     6479 2023-03-27 16:16:41.000000 bicleaner-ai-2.2.0/src/bicleaner_ai/datagen.py
--rw-r--r--   0 runner    (1001) docker     (122)     7456 2023-03-27 16:16:41.000000 bicleaner-ai-2.2.0/src/bicleaner_ai/decomposable_attention.py
--rw-r--r--   0 runner    (1001) docker     (122)     3927 2023-03-27 16:16:41.000000 bicleaner-ai-2.2.0/src/bicleaner_ai/layers.py
--rw-r--r--   0 runner    (1001) docker     (122)     2283 2023-03-27 16:16:41.000000 bicleaner-ai-2.2.0/src/bicleaner_ai/losses.py
--rw-r--r--   0 runner    (1001) docker     (122)     6372 2023-03-27 16:16:41.000000 bicleaner-ai-2.2.0/src/bicleaner_ai/metrics.py
--rw-r--r--   0 runner    (1001) docker     (122)    25236 2023-03-27 16:16:41.000000 bicleaner-ai-2.2.0/src/bicleaner_ai/models.py
--rw-r--r--   0 runner    (1001) docker     (122)     4101 2023-03-27 16:16:41.000000 bicleaner-ai-2.2.0/src/bicleaner_ai/models_util.py
--rw-r--r--   0 runner    (1001) docker     (122)     1197 2023-03-27 16:16:41.000000 bicleaner-ai-2.2.0/src/bicleaner_ai/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (122)    13140 2023-03-27 16:16:41.000000 bicleaner-ai-2.2.0/src/bicleaner_ai/training.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     4004 2023-03-27 16:16:41.000000 bicleaner-ai-2.2.0/src/bicleaner_ai/util.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1351 2023-03-27 16:16:41.000000 bicleaner-ai-2.2.0/src/bicleaner_ai/word_freqs_list.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     3123 2023-03-27 16:16:41.000000 bicleaner-ai-2.2.0/src/bicleaner_ai/word_freqs_zipf.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1082 2023-03-27 16:16:41.000000 bicleaner-ai-2.2.0/src/bicleaner_ai/word_freqs_zipf_double_linked.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-27 16:16:54.348971 bicleaner-ai-2.2.0/src/bicleaner_ai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    65558 2023-03-27 16:16:54.000000 bicleaner-ai-2.2.0/src/bicleaner_ai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      950 2023-03-27 16:16:54.000000 bicleaner-ai-2.2.0/src/bicleaner_ai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-27 16:16:54.000000 bicleaner-ai-2.2.0/src/bicleaner_ai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      276 2023-03-27 16:16:54.000000 bicleaner-ai-2.2.0/src/bicleaner_ai.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      293 2023-03-27 16:16:54.000000 bicleaner-ai-2.2.0/src/bicleaner_ai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       13 2023-03-27 16:16:54.000000 bicleaner-ai-2.2.0/src/bicleaner_ai.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 09:15:30.465664 bicleaner-ai-2.2.1/
+-rw-r--r--   0 runner    (1001) docker     (122)    35147 2023-05-08 09:15:15.000000 bicleaner-ai-2.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)    65558 2023-05-08 09:15:30.465664 bicleaner-ai-2.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    24077 2023-05-08 09:15:15.000000 bicleaner-ai-2.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     2039 2023-05-08 09:15:15.000000 bicleaner-ai-2.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-08 09:15:30.465664 bicleaner-ai-2.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 09:15:30.461664 bicleaner-ai-2.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 09:15:30.465664 bicleaner-ai-2.2.1/src/bicleaner_ai/
+-rwxr-xr-x   0 runner    (1001) docker     (122)      112 2023-05-08 09:15:15.000000 bicleaner-ai-2.2.1/src/bicleaner_ai/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     4547 2023-05-08 09:15:15.000000 bicleaner-ai-2.2.1/src/bicleaner_ai/bicleaner_ai_classifier.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     3607 2023-05-08 09:15:15.000000 bicleaner-ai-2.2.1/src/bicleaner_ai/bicleaner_ai_download.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)      642 2023-05-08 09:15:15.000000 bicleaner-ai-2.2.1/src/bicleaner_ai/bicleaner_ai_download_hf.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    16502 2023-05-08 09:15:15.000000 bicleaner-ai-2.2.1/src/bicleaner_ai/bicleaner_ai_train.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2964 2023-05-08 09:15:15.000000 bicleaner-ai-2.2.1/src/bicleaner_ai/calibrate.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13926 2023-05-08 09:15:15.000000 bicleaner-ai-2.2.1/src/bicleaner_ai/classify.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6479 2023-05-08 09:15:15.000000 bicleaner-ai-2.2.1/src/bicleaner_ai/datagen.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7456 2023-05-08 09:15:15.000000 bicleaner-ai-2.2.1/src/bicleaner_ai/decomposable_attention.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3927 2023-05-08 09:15:15.000000 bicleaner-ai-2.2.1/src/bicleaner_ai/layers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2283 2023-05-08 09:15:15.000000 bicleaner-ai-2.2.1/src/bicleaner_ai/losses.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6372 2023-05-08 09:15:15.000000 bicleaner-ai-2.2.1/src/bicleaner_ai/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25236 2023-05-08 09:15:15.000000 bicleaner-ai-2.2.1/src/bicleaner_ai/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4101 2023-05-08 09:15:15.000000 bicleaner-ai-2.2.1/src/bicleaner_ai/models_util.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1197 2023-05-08 09:15:15.000000 bicleaner-ai-2.2.1/src/bicleaner_ai/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13140 2023-05-08 09:15:15.000000 bicleaner-ai-2.2.1/src/bicleaner_ai/training.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     4004 2023-05-08 09:15:15.000000 bicleaner-ai-2.2.1/src/bicleaner_ai/util.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1351 2023-05-08 09:15:15.000000 bicleaner-ai-2.2.1/src/bicleaner_ai/word_freqs_list.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     3123 2023-05-08 09:15:15.000000 bicleaner-ai-2.2.1/src/bicleaner_ai/word_freqs_zipf.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1082 2023-05-08 09:15:15.000000 bicleaner-ai-2.2.1/src/bicleaner_ai/word_freqs_zipf_double_linked.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 09:15:30.465664 bicleaner-ai-2.2.1/src/bicleaner_ai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    65558 2023-05-08 09:15:30.000000 bicleaner-ai-2.2.1/src/bicleaner_ai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      950 2023-05-08 09:15:30.000000 bicleaner-ai-2.2.1/src/bicleaner_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-08 09:15:30.000000 bicleaner-ai-2.2.1/src/bicleaner_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      276 2023-05-08 09:15:30.000000 bicleaner-ai-2.2.1/src/bicleaner_ai.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      293 2023-05-08 09:15:30.000000 bicleaner-ai-2.2.1/src/bicleaner_ai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-05-08 09:15:30.000000 bicleaner-ai-2.2.1/src/bicleaner_ai.egg-info/top_level.txt
```

### Comparing `bicleaner-ai-2.2.0/LICENSE` & `bicleaner-ai-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bicleaner-ai-2.2.0/PKG-INFO` & `bicleaner-ai-2.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bicleaner-ai
-Version: 2.2.0
+Version: 2.2.1
 Summary: Parallel corpus classifier, indicating the likelihood of a pair of sentences being mutual translations or not (neural version)
 Author-email: Prompsit Language Engineering <info@prompsit.com>
 Maintainer-email: Jaume Zaragoza <jzaragoza@prompsit.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
```

### Comparing `bicleaner-ai-2.2.0/README.md` & `bicleaner-ai-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `bicleaner-ai-2.2.0/pyproject.toml` & `bicleaner-ai-2.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "bicleaner-ai"
-version = "2.2.0"
+version = "2.2.1"
 license = {file = "LICENSE"}
 authors = [
     { "name" = "Prompsit Language Engineering", "email" = "info@prompsit.com" }
 ]
 maintainers = [
     { "name" = "Jaume Zaragoza", "email" = "jzaragoza@prompsit.com" }
 ]
@@ -15,15 +15,15 @@
     "scikit-learn>=0.22.1",
     "PyYAML>=5.1.2",
     "numpy",
     "pytest",
     "toolwrapper",
     "joblib",
     "sacremoses",
-    "bicleaner-hardrules==2.8.0",
+    "bicleaner-hardrules==2.8.1",
     "sentencepiece",
     "tensorflow>=2.6.5,<2.12",
     "bicleaner-ai-glove==0.2.1",
     "fuzzywuzzy",
     "python-Levenshtein",
     "transformers==4.26",
     "huggingface-hub>=0.13,<0.14",
```

### Comparing `bicleaner-ai-2.2.0/src/bicleaner_ai/bicleaner_ai_classifier.py` & `bicleaner-ai-2.2.1/src/bicleaner_ai/bicleaner_ai_classifier.py`

 * *Files identical despite different names*

### Comparing `bicleaner-ai-2.2.0/src/bicleaner_ai/bicleaner_ai_download.py` & `bicleaner-ai-2.2.1/src/bicleaner_ai/bicleaner_ai_download.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     h = logging.StreamHandler(sys.stderr)
     h.setFormatter(logging.Formatter('%(asctime)s - %(levelname)s - %(message)s'))
     logger.addHandler(h)
 
 
 def main():
     parser = ArgumentParser(
-            description='Download Bicleaner AI models from the Hugging Face Hub')
+            description='Download Bicleaner AI models from the HuggingFace Hub or GitHub')
     parser.add_argument('src_lang', type=str,
                         help='Source language')
     parser.add_argument('trg_lang', type=str,
                         help='Target language')
     parser.add_argument('model_type', type=str, choices=['full', 'lite'],
                         help='Download lite or full model')
     parser.add_argument('download_path', type=str, nargs='?',
@@ -47,15 +47,15 @@
         raise Exception("Lite models need a download path")
 
     if args.model_type == 'full':
         #TODO fallback to github if does not exist?
         name = f'bitextor/bicleaner-ai-full-{args.src_lang}-{args.trg_lang}'
         logging.info(f'Downloading {name}')
         try:
-            snapshot_download(name, use_auth_token=args.auth_token)
+            snapshot_download(name, use_auth_token=args.auth_token, etag_timeout=100)
             return
         except RepositoryNotFoundError:
             if not args.download_path:
                 logging.error(f"Model repository {name} not found at HuggingFace," \
                               + "please provide a path to download old model from Github")
             logging.warning(f"Model repository {name} not found, trying Github old models...")
```

### Comparing `bicleaner-ai-2.2.0/src/bicleaner_ai/bicleaner_ai_download_hf.py` & `bicleaner-ai-2.2.1/src/bicleaner_ai/bicleaner_ai_download_hf.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,11 +5,11 @@
 def main():
     parser = ArgumentParser(description='Download Bicleaner AI full models from the Hugging Face Hub')
     parser.add_argument('model', type=str, help='Hugging Face Bicleaner AI model identifier (e.g. "bitextor/bicleaner-ai-full-en-fr")')
     parser.add_argument('-t', '--auth_token', default=None, type=str, help='Authentication token for private models downloading')
 
     args = parser.parse_args()
 
-    snapshot_download(args.model, use_auth_token=args.auth_token)
+    snapshot_download(args.model, use_auth_token=args.auth_token, etag_timeout=100)
 
 if __name__ == "__main__":
     main()
```

### Comparing `bicleaner-ai-2.2.0/src/bicleaner_ai/bicleaner_ai_train.py` & `bicleaner-ai-2.2.1/src/bicleaner_ai/bicleaner_ai_train.py`

 * *Files identical despite different names*

### Comparing `bicleaner-ai-2.2.0/src/bicleaner_ai/calibrate.py` & `bicleaner-ai-2.2.1/src/bicleaner_ai/calibrate.py`

 * *Files identical despite different names*

### Comparing `bicleaner-ai-2.2.0/src/bicleaner_ai/classify.py` & `bicleaner-ai-2.2.1/src/bicleaner_ai/classify.py`

 * *Files identical despite different names*

### Comparing `bicleaner-ai-2.2.0/src/bicleaner_ai/datagen.py` & `bicleaner-ai-2.2.1/src/bicleaner_ai/datagen.py`

 * *Files identical despite different names*

### Comparing `bicleaner-ai-2.2.0/src/bicleaner_ai/decomposable_attention.py` & `bicleaner-ai-2.2.1/src/bicleaner_ai/decomposable_attention.py`

 * *Files identical despite different names*

### Comparing `bicleaner-ai-2.2.0/src/bicleaner_ai/layers.py` & `bicleaner-ai-2.2.1/src/bicleaner_ai/layers.py`

 * *Files identical despite different names*

### Comparing `bicleaner-ai-2.2.0/src/bicleaner_ai/losses.py` & `bicleaner-ai-2.2.1/src/bicleaner_ai/losses.py`

 * *Files identical despite different names*

### Comparing `bicleaner-ai-2.2.0/src/bicleaner_ai/metrics.py` & `bicleaner-ai-2.2.1/src/bicleaner_ai/metrics.py`

 * *Files identical despite different names*

### Comparing `bicleaner-ai-2.2.0/src/bicleaner_ai/models.py` & `bicleaner-ai-2.2.1/src/bicleaner_ai/models.py`

 * *Files identical despite different names*

### Comparing `bicleaner-ai-2.2.0/src/bicleaner_ai/models_util.py` & `bicleaner-ai-2.2.1/src/bicleaner_ai/models_util.py`

 * *Files identical despite different names*

### Comparing `bicleaner-ai-2.2.0/src/bicleaner_ai/tokenizer.py` & `bicleaner-ai-2.2.1/src/bicleaner_ai/tokenizer.py`

 * *Files identical despite different names*

### Comparing `bicleaner-ai-2.2.0/src/bicleaner_ai/training.py` & `bicleaner-ai-2.2.1/src/bicleaner_ai/training.py`

 * *Files identical despite different names*

### Comparing `bicleaner-ai-2.2.0/src/bicleaner_ai/util.py` & `bicleaner-ai-2.2.1/src/bicleaner_ai/util.py`

 * *Files identical despite different names*

### Comparing `bicleaner-ai-2.2.0/src/bicleaner_ai/word_freqs_list.py` & `bicleaner-ai-2.2.1/src/bicleaner_ai/word_freqs_list.py`

 * *Files identical despite different names*

### Comparing `bicleaner-ai-2.2.0/src/bicleaner_ai/word_freqs_zipf.py` & `bicleaner-ai-2.2.1/src/bicleaner_ai/word_freqs_zipf.py`

 * *Files identical despite different names*

### Comparing `bicleaner-ai-2.2.0/src/bicleaner_ai/word_freqs_zipf_double_linked.py` & `bicleaner-ai-2.2.1/src/bicleaner_ai/word_freqs_zipf_double_linked.py`

 * *Files identical despite different names*

### Comparing `bicleaner-ai-2.2.0/src/bicleaner_ai.egg-info/PKG-INFO` & `bicleaner-ai-2.2.1/src/bicleaner_ai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bicleaner-ai
-Version: 2.2.0
+Version: 2.2.1
 Summary: Parallel corpus classifier, indicating the likelihood of a pair of sentences being mutual translations or not (neural version)
 Author-email: Prompsit Language Engineering <info@prompsit.com>
 Maintainer-email: Jaume Zaragoza <jzaragoza@prompsit.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
```

### Comparing `bicleaner-ai-2.2.0/src/bicleaner_ai.egg-info/SOURCES.txt` & `bicleaner-ai-2.2.1/src/bicleaner_ai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

