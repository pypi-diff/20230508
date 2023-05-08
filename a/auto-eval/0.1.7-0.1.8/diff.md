# Comparing `tmp/auto-eval-0.1.7.tar.gz` & `tmp/auto-eval-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto-eval-0.1.7.tar", last modified: Mon May  8 13:26:10 2023, max compression
+gzip compressed data, was "auto-eval-0.1.8.tar", last modified: Mon May  8 13:28:27 2023, max compression
```

## Comparing `auto-eval-0.1.7.tar` & `auto-eval-0.1.8.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-08 13:26:10.009259 auto-eval-0.1.7/
--rw-r--r--   0 zhangchong   (501) staff       (20)     1071 2023-04-28 07:53:45.000000 auto-eval-0.1.7/LICENSE
--rw-r--r--   0 zhangchong   (501) staff       (20)    11522 2023-05-08 13:26:10.008997 auto-eval-0.1.7/PKG-INFO
--rw-r--r--   0 zhangchong   (501) staff       (20)    11096 2023-05-08 02:17:16.000000 auto-eval-0.1.7/README.md
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-08 13:26:10.006930 auto-eval-0.1.7/auto_eval.egg-info/
--rw-r--r--   0 zhangchong   (501) staff       (20)    11522 2023-05-08 13:26:09.000000 auto-eval-0.1.7/auto_eval.egg-info/PKG-INFO
--rw-r--r--   0 zhangchong   (501) staff       (20)      433 2023-05-08 13:26:09.000000 auto-eval-0.1.7/auto_eval.egg-info/SOURCES.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)        1 2023-05-08 13:26:09.000000 auto-eval-0.1.7/auto_eval.egg-info/dependency_links.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)       59 2023-05-08 13:26:09.000000 auto-eval-0.1.7/auto_eval.egg-info/entry_points.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)       49 2023-05-08 13:26:09.000000 auto-eval-0.1.7/auto_eval.egg-info/requires.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)        5 2023-05-08 13:26:09.000000 auto-eval-0.1.7/auto_eval.egg-info/top_level.txt
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-08 13:26:10.007205 auto-eval-0.1.7/eval/
--rw-r--r--   0 zhangchong   (501) staff       (20)      136 2023-05-08 07:54:51.000000 auto-eval-0.1.7/eval/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     7011 2023-05-08 13:00:48.000000 auto-eval-0.1.7/eval/auto_llms_eval.py
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-08 13:26:10.007476 auto-eval-0.1.7/eval/commands/
--rw-r--r--   0 zhangchong   (501) staff       (20)        0 2023-04-28 08:32:15.000000 auto-eval-0.1.7/eval/commands/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     3928 2023-05-08 07:55:11.000000 auto-eval-0.1.7/eval/commands/auto_eval.py
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-08 13:26:10.008244 auto-eval-0.1.7/eval/prompt_template/
--rw-r--r--   0 zhangchong   (501) staff       (20)       44 2023-05-05 07:40:16.000000 auto-eval-0.1.7/eval/prompt_template/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     3092 2023-05-08 13:10:10.000000 auto-eval-0.1.7/eval/prompt_template/prompter.py
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-08 13:26:10.008745 auto-eval-0.1.7/eval/utils/
--rw-r--r--   0 zhangchong   (501) staff       (20)       26 2023-04-28 09:40:19.000000 auto-eval-0.1.7/eval/utils/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     3108 2023-05-08 13:22:30.000000 auto-eval-0.1.7/eval/utils/data_utils.py
--rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-05-08 13:26:10.009314 auto-eval-0.1.7/setup.cfg
--rw-r--r--   0 zhangchong   (501) staff       (20)      950 2023-05-08 07:57:24.000000 auto-eval-0.1.7/setup.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-08 13:28:27.824972 auto-eval-0.1.8/
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1071 2023-04-28 07:53:45.000000 auto-eval-0.1.8/LICENSE
+-rw-r--r--   0 zhangchong   (501) staff       (20)    11522 2023-05-08 13:28:27.824711 auto-eval-0.1.8/PKG-INFO
+-rw-r--r--   0 zhangchong   (501) staff       (20)    11096 2023-05-08 02:17:16.000000 auto-eval-0.1.8/README.md
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-08 13:28:27.821655 auto-eval-0.1.8/auto_eval.egg-info/
+-rw-r--r--   0 zhangchong   (501) staff       (20)    11522 2023-05-08 13:28:27.000000 auto-eval-0.1.8/auto_eval.egg-info/PKG-INFO
+-rw-r--r--   0 zhangchong   (501) staff       (20)      480 2023-05-08 13:28:27.000000 auto-eval-0.1.8/auto_eval.egg-info/SOURCES.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)        1 2023-05-08 13:28:27.000000 auto-eval-0.1.8/auto_eval.egg-info/dependency_links.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)       59 2023-05-08 13:28:27.000000 auto-eval-0.1.8/auto_eval.egg-info/entry_points.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)       49 2023-05-08 13:28:27.000000 auto-eval-0.1.8/auto_eval.egg-info/requires.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)        5 2023-05-08 13:28:27.000000 auto-eval-0.1.8/auto_eval.egg-info/top_level.txt
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-08 13:28:27.822258 auto-eval-0.1.8/eval/
+-rw-r--r--   0 zhangchong   (501) staff       (20)      136 2023-05-08 07:54:51.000000 auto-eval-0.1.8/eval/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     7011 2023-05-08 13:00:48.000000 auto-eval-0.1.8/eval/auto_llms_eval.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-08 13:28:27.822755 auto-eval-0.1.8/eval/commands/
+-rw-r--r--   0 zhangchong   (501) staff       (20)        0 2023-04-28 08:32:15.000000 auto-eval-0.1.8/eval/commands/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     3928 2023-05-08 07:55:11.000000 auto-eval-0.1.8/eval/commands/auto_eval.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-08 13:28:27.823827 auto-eval-0.1.8/eval/prompt_template/
+-rw-r--r--   0 zhangchong   (501) staff       (20)       44 2023-05-05 07:40:16.000000 auto-eval-0.1.8/eval/prompt_template/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)      775 2023-05-06 02:34:00.000000 auto-eval-0.1.8/eval/prompt_template/eval_prompt_template.json
+-rw-r--r--   0 zhangchong   (501) staff       (20)     3092 2023-05-08 13:10:10.000000 auto-eval-0.1.8/eval/prompt_template/prompter.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-08 13:28:27.824425 auto-eval-0.1.8/eval/utils/
+-rw-r--r--   0 zhangchong   (501) staff       (20)       26 2023-04-28 09:40:19.000000 auto-eval-0.1.8/eval/utils/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     3108 2023-05-08 13:22:30.000000 auto-eval-0.1.8/eval/utils/data_utils.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-05-08 13:28:27.825025 auto-eval-0.1.8/setup.cfg
+-rw-r--r--   0 zhangchong   (501) staff       (20)      950 2023-05-08 13:28:24.000000 auto-eval-0.1.8/setup.py
```

### Comparing `auto-eval-0.1.7/LICENSE` & `auto-eval-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `auto-eval-0.1.7/PKG-INFO` & `auto-eval-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-eval
-Version: 0.1.7
+Version: 0.1.8
 Summary: Using only one line of commmands to evaluate multiple models
 Home-page: https://github.com/muximus3/Auto-Eval
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `auto-eval-0.1.7/README.md` & `auto-eval-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `auto-eval-0.1.7/auto_eval.egg-info/PKG-INFO` & `auto-eval-0.1.8/auto_eval.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-eval
-Version: 0.1.7
+Version: 0.1.8
 Summary: Using only one line of commmands to evaluate multiple models
 Home-page: https://github.com/muximus3/Auto-Eval
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `auto-eval-0.1.7/eval/auto_llms_eval.py` & `auto-eval-0.1.8/eval/auto_llms_eval.py`

 * *Files identical despite different names*

### Comparing `auto-eval-0.1.7/eval/commands/auto_eval.py` & `auto-eval-0.1.8/eval/commands/auto_eval.py`

 * *Files identical despite different names*

### Comparing `auto-eval-0.1.7/eval/prompt_template/prompter.py` & `auto-eval-0.1.8/eval/prompt_template/prompter.py`

 * *Files identical despite different names*

### Comparing `auto-eval-0.1.7/eval/utils/data_utils.py` & `auto-eval-0.1.8/eval/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `auto-eval-0.1.7/setup.py` & `auto-eval-0.1.8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 setup(
     name="auto-eval",
-    version="0.1.7",
+    version="0.1.8",
     packages=find_packages(),
     package_data={
-      "eval/prompt_template":["eval_prompt_template.json"]  
+      "eval":["prompt_template/eval_prompt_template.json"]  
     },
     install_requires=[
         # Add your library's dependencies here
         "one-api-tool",
         "pandas",
         "openpyxl",
         "tabulate",
```

