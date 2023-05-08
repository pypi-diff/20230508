# Comparing `tmp/finetune_eval_harness-0.5.0.dev0.tar.gz` & `tmp/finetune_eval_harness-0.6.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finetune_eval_harness-0.5.0.dev0.tar", last modified: Mon May  8 21:07:57 2023, max compression
+gzip compressed data, was "finetune_eval_harness-0.6.0.dev0.tar", last modified: Mon May  8 21:37:54 2023, max compression
```

## Comparing `finetune_eval_harness-0.5.0.dev0.tar` & `finetune_eval_harness-0.6.0.dev0.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:07:57.719720 finetune_eval_harness-0.5.0.dev0/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-08 21:07:57.000000 finetune_eval_harness-0.5.0.dev0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-08 21:07:57.719720 finetune_eval_harness-0.5.0.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-05-08 21:07:57.000000 finetune_eval_harness-0.5.0.dev0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:07:57.715720 finetune_eval_harness-0.5.0.dev0/finetune_eval_harness.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-08 21:07:57.000000 finetune_eval_harness-0.5.0.dev0/finetune_eval_harness.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-08 21:07:57.000000 finetune_eval_harness-0.5.0.dev0/finetune_eval_harness.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-08 21:07:57.000000 finetune_eval_harness-0.5.0.dev0/finetune_eval_harness.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-08 21:07:57.000000 finetune_eval_harness-0.5.0.dev0/finetune_eval_harness.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-08 21:07:57.000000 finetune_eval_harness-0.5.0.dev0/finetune_eval_harness.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:07:57.715720 finetune_eval_harness-0.5.0.dev0/hf_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 21:07:57.000000 finetune_eval_harness-0.5.0.dev0/hf_scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9405 2023-05-08 21:07:57.000000 finetune_eval_harness-0.5.0.dev0/hf_scripts/data_trainining_args.py
--rw-r--r--   0 runner    (1001) docker     (123)     9381 2023-05-08 21:07:57.000000 finetune_eval_harness-0.5.0.dev0/hf_scripts/hgf_fine_tune_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     7260 2023-05-08 21:07:57.000000 finetune_eval_harness-0.5.0.dev0/hf_scripts/hgf_fine_tune_ner.py
--rw-r--r--   0 runner    (1001) docker     (123)    11455 2023-05-08 21:07:57.000000 finetune_eval_harness-0.5.0.dev0/hf_scripts/hgf_fine_tune_qa.py
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-08 21:07:57.000000 finetune_eval_harness-0.5.0.dev0/hf_scripts/initial_arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-05-08 21:07:57.000000 finetune_eval_harness-0.5.0.dev0/hf_scripts/model_args.py
--rw-r--r--   0 runner    (1001) docker     (123)    48785 2023-05-08 21:07:57.000000 finetune_eval_harness-0.5.0.dev0/hf_scripts/trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-05-08 21:07:57.000000 finetune_eval_harness-0.5.0.dev0/hf_scripts/trainer_qa.py
--rw-r--r--   0 runner    (1001) docker     (123)    53665 2023-05-08 21:07:57.000000 finetune_eval_harness-0.5.0.dev0/hf_scripts/utility_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    23681 2023-05-08 21:07:57.000000 finetune_eval_harness-0.5.0.dev0/hf_scripts/utils_qa.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-08 21:07:57.000000 finetune_eval_harness-0.5.0.dev0/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-05-08 21:07:57.000000 finetune_eval_harness-0.5.0.dev0/process_args.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 21:07:57.719720 finetune_eval_harness-0.5.0.dev0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-05-08 21:07:57.000000 finetune_eval_harness-0.5.0.dev0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:07:57.719720 finetune_eval_harness-0.5.0.dev0/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-05-08 21:07:57.000000 finetune_eval_harness-0.5.0.dev0/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-08 21:07:57.000000 finetune_eval_harness-0.5.0.dev0/tasks/classification.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-08 21:07:57.000000 finetune_eval_harness-0.5.0.dev0/tasks/german_europarl.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-08 21:07:57.000000 finetune_eval_harness-0.5.0.dev0/tasks/german_ner.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-08 21:07:57.000000 finetune_eval_harness-0.5.0.dev0/tasks/german_quad.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-08 21:07:57.000000 finetune_eval_harness-0.5.0.dev0/tasks/germeval2017.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-08 21:07:57.000000 finetune_eval_harness-0.5.0.dev0/tasks/germeval2018.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-08 21:07:57.000000 finetune_eval_harness-0.5.0.dev0/tasks/gnad10.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-08 21:07:57.000000 finetune_eval_harness-0.5.0.dev0/tasks/ner.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-08 21:07:57.000000 finetune_eval_harness-0.5.0.dev0/tasks/qa.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:07:57.719720 finetune_eval_harness-0.5.0.dev0/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 21:07:57.000000 finetune_eval_harness-0.5.0.dev0/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-08 21:07:57.000000 finetune_eval_harness-0.5.0.dev0/templates/new_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-05-08 21:07:57.000000 finetune_eval_harness-0.5.0.dev0/templates/new_task_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:07:57.719720 finetune_eval_harness-0.5.0.dev0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 21:07:57.000000 finetune_eval_harness-0.5.0.dev0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-08 21:07:57.000000 finetune_eval_harness-0.5.0.dev0/tests/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-05-08 21:07:57.000000 finetune_eval_harness-0.5.0.dev0/tests/test_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-08 21:07:57.000000 finetune_eval_harness-0.5.0.dev0/tests/test_stability.py
--rw-r--r--   0 runner    (1001) docker     (123)     7372 2023-05-08 21:07:57.000000 finetune_eval_harness-0.5.0.dev0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:37:54.652788 finetune_eval_harness-0.6.0.dev0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-08 21:37:53.000000 finetune_eval_harness-0.6.0.dev0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-05-08 21:37:54.652788 finetune_eval_harness-0.6.0.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-05-08 21:37:53.000000 finetune_eval_harness-0.6.0.dev0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:37:54.648788 finetune_eval_harness-0.6.0.dev0/finetune_eval_harness.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-05-08 21:37:54.000000 finetune_eval_harness-0.6.0.dev0/finetune_eval_harness.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-08 21:37:54.000000 finetune_eval_harness-0.6.0.dev0/finetune_eval_harness.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-08 21:37:54.000000 finetune_eval_harness-0.6.0.dev0/finetune_eval_harness.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-08 21:37:54.000000 finetune_eval_harness-0.6.0.dev0/finetune_eval_harness.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-08 21:37:54.000000 finetune_eval_harness-0.6.0.dev0/finetune_eval_harness.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:37:54.652788 finetune_eval_harness-0.6.0.dev0/hf_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 21:37:53.000000 finetune_eval_harness-0.6.0.dev0/hf_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9405 2023-05-08 21:37:53.000000 finetune_eval_harness-0.6.0.dev0/hf_scripts/data_trainining_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9381 2023-05-08 21:37:53.000000 finetune_eval_harness-0.6.0.dev0/hf_scripts/hgf_fine_tune_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7260 2023-05-08 21:37:53.000000 finetune_eval_harness-0.6.0.dev0/hf_scripts/hgf_fine_tune_ner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11455 2023-05-08 21:37:53.000000 finetune_eval_harness-0.6.0.dev0/hf_scripts/hgf_fine_tune_qa.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-08 21:37:53.000000 finetune_eval_harness-0.6.0.dev0/hf_scripts/initial_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-05-08 21:37:53.000000 finetune_eval_harness-0.6.0.dev0/hf_scripts/model_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48785 2023-05-08 21:37:53.000000 finetune_eval_harness-0.6.0.dev0/hf_scripts/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-05-08 21:37:53.000000 finetune_eval_harness-0.6.0.dev0/hf_scripts/trainer_qa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53665 2023-05-08 21:37:53.000000 finetune_eval_harness-0.6.0.dev0/hf_scripts/utility_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23681 2023-05-08 21:37:53.000000 finetune_eval_harness-0.6.0.dev0/hf_scripts/utils_qa.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-08 21:37:53.000000 finetune_eval_harness-0.6.0.dev0/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-05-08 21:37:53.000000 finetune_eval_harness-0.6.0.dev0/process_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 21:37:54.652788 finetune_eval_harness-0.6.0.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-05-08 21:37:53.000000 finetune_eval_harness-0.6.0.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:37:54.652788 finetune_eval_harness-0.6.0.dev0/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-05-08 21:37:53.000000 finetune_eval_harness-0.6.0.dev0/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-08 21:37:53.000000 finetune_eval_harness-0.6.0.dev0/tasks/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-08 21:37:53.000000 finetune_eval_harness-0.6.0.dev0/tasks/german_europarl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-08 21:37:53.000000 finetune_eval_harness-0.6.0.dev0/tasks/german_ner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-08 21:37:53.000000 finetune_eval_harness-0.6.0.dev0/tasks/german_quad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-08 21:37:53.000000 finetune_eval_harness-0.6.0.dev0/tasks/germeval2017.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-08 21:37:53.000000 finetune_eval_harness-0.6.0.dev0/tasks/germeval2018.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-08 21:37:53.000000 finetune_eval_harness-0.6.0.dev0/tasks/gnad10.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-08 21:37:53.000000 finetune_eval_harness-0.6.0.dev0/tasks/ner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-08 21:37:53.000000 finetune_eval_harness-0.6.0.dev0/tasks/qa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:37:54.652788 finetune_eval_harness-0.6.0.dev0/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 21:37:53.000000 finetune_eval_harness-0.6.0.dev0/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-08 21:37:53.000000 finetune_eval_harness-0.6.0.dev0/templates/new_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-05-08 21:37:53.000000 finetune_eval_harness-0.6.0.dev0/templates/new_task_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:37:54.652788 finetune_eval_harness-0.6.0.dev0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 21:37:53.000000 finetune_eval_harness-0.6.0.dev0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-08 21:37:53.000000 finetune_eval_harness-0.6.0.dev0/tests/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-05-08 21:37:53.000000 finetune_eval_harness-0.6.0.dev0/tests/test_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-08 21:37:53.000000 finetune_eval_harness-0.6.0.dev0/tests/test_stability.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7372 2023-05-08 21:37:53.000000 finetune_eval_harness-0.6.0.dev0/tests/test_utils.py
```

### Comparing `finetune_eval_harness-0.5.0.dev0/LICENSE` & `finetune_eval_harness-0.6.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.5.0.dev0/README.md` & `finetune_eval_harness-0.6.0.dev0/README.md`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.5.0.dev0/finetune_eval_harness.egg-info/SOURCES.txt` & `finetune_eval_harness-0.6.0.dev0/finetune_eval_harness.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.5.0.dev0/hf_scripts/data_trainining_args.py` & `finetune_eval_harness-0.6.0.dev0/hf_scripts/data_trainining_args.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.5.0.dev0/hf_scripts/hgf_fine_tune_class.py` & `finetune_eval_harness-0.6.0.dev0/hf_scripts/hgf_fine_tune_class.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.5.0.dev0/hf_scripts/hgf_fine_tune_ner.py` & `finetune_eval_harness-0.6.0.dev0/hf_scripts/hgf_fine_tune_ner.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.5.0.dev0/hf_scripts/hgf_fine_tune_qa.py` & `finetune_eval_harness-0.6.0.dev0/hf_scripts/hgf_fine_tune_qa.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.5.0.dev0/hf_scripts/model_args.py` & `finetune_eval_harness-0.6.0.dev0/hf_scripts/model_args.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.5.0.dev0/hf_scripts/trainer.py` & `finetune_eval_harness-0.6.0.dev0/hf_scripts/trainer.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.5.0.dev0/hf_scripts/trainer_qa.py` & `finetune_eval_harness-0.6.0.dev0/hf_scripts/trainer_qa.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.5.0.dev0/hf_scripts/utility_functions.py` & `finetune_eval_harness-0.6.0.dev0/hf_scripts/utility_functions.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.5.0.dev0/hf_scripts/utils_qa.py` & `finetune_eval_harness-0.6.0.dev0/hf_scripts/utils_qa.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.5.0.dev0/process_args.py` & `finetune_eval_harness-0.6.0.dev0/process_args.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.5.0.dev0/setup.py` & `finetune_eval_harness-0.6.0.dev0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from setuptools import find_packages, setup
 
 setup(
     name = "finetune_eval_harness",
-    version="0.5.0.dev0",
+    version="0.6.0.dev0",
     description="Finetune_Eval_Harness",
-    #long_description=open("README.md", "r", encoding="utf-8").read(),
+    long_description=open("README.md", "r", encoding="utf-8").read(),
+    long_description_content_type="text/markdown",
     keywords="deep learning",
     author="DFKI Berlin",
     author_email="akga01@dfki.de",
     #url="https://github.com/malteos/finetune-evaluation-harness",
     #package_dir={"":""},
     packages=[
             'hf_scripts',
```

### Comparing `finetune_eval_harness-0.5.0.dev0/tasks/__init__.py` & `finetune_eval_harness-0.6.0.dev0/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.5.0.dev0/tasks/classification.py` & `finetune_eval_harness-0.6.0.dev0/tasks/classification.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.5.0.dev0/tasks/german_europarl.py` & `finetune_eval_harness-0.6.0.dev0/tasks/german_europarl.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.5.0.dev0/tasks/germeval2017.py` & `finetune_eval_harness-0.6.0.dev0/tasks/germeval2017.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.5.0.dev0/tasks/germeval2018.py` & `finetune_eval_harness-0.6.0.dev0/tasks/germeval2018.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.5.0.dev0/tasks/gnad10.py` & `finetune_eval_harness-0.6.0.dev0/tasks/gnad10.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.5.0.dev0/tasks/ner.py` & `finetune_eval_harness-0.6.0.dev0/tasks/ner.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.5.0.dev0/templates/new_task.py` & `finetune_eval_harness-0.6.0.dev0/templates/new_task.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.5.0.dev0/templates/new_task_type.py` & `finetune_eval_harness-0.6.0.dev0/templates/new_task_type.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.5.0.dev0/tests/test_eval.py` & `finetune_eval_harness-0.6.0.dev0/tests/test_eval.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.5.0.dev0/tests/test_stability.py` & `finetune_eval_harness-0.6.0.dev0/tests/test_stability.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.5.0.dev0/tests/test_utils.py` & `finetune_eval_harness-0.6.0.dev0/tests/test_utils.py`

 * *Files identical despite different names*

