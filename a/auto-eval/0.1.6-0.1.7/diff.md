# Comparing `tmp/auto-eval-0.1.6.tar.gz` & `tmp/auto-eval-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto-eval-0.1.6.tar", last modified: Sat May  6 02:35:57 2023, max compression
+gzip compressed data, was "auto-eval-0.1.7.tar", last modified: Mon May  8 13:26:10 2023, max compression
```

## Comparing `auto-eval-0.1.6.tar` & `auto-eval-0.1.7.tar`

### file list

```diff
@@ -1,26 +1,25 @@
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-06 02:35:57.660247 auto-eval-0.1.6/
--rw-r--r--   0 zhangchong   (501) staff       (20)     1071 2023-04-28 07:53:45.000000 auto-eval-0.1.6/LICENSE
--rw-r--r--   0 zhangchong   (501) staff       (20)    11478 2023-05-06 02:35:57.660019 auto-eval-0.1.6/PKG-INFO
--rw-r--r--   0 zhangchong   (501) staff       (20)    11052 2023-05-05 09:05:05.000000 auto-eval-0.1.6/README.md
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-06 02:35:57.657363 auto-eval-0.1.6/auto_eval.egg-info/
--rw-r--r--   0 zhangchong   (501) staff       (20)    11478 2023-05-06 02:35:57.000000 auto-eval-0.1.6/auto_eval.egg-info/PKG-INFO
--rw-r--r--   0 zhangchong   (501) staff       (20)      445 2023-05-06 02:35:57.000000 auto-eval-0.1.6/auto_eval.egg-info/SOURCES.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)        1 2023-05-06 02:35:57.000000 auto-eval-0.1.6/auto_eval.egg-info/dependency_links.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)       54 2023-05-06 02:35:57.000000 auto-eval-0.1.6/auto_eval.egg-info/entry_points.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)       49 2023-05-06 02:35:57.000000 auto-eval-0.1.6/auto_eval.egg-info/requires.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)       36 2023-05-06 02:35:57.000000 auto-eval-0.1.6/auto_eval.egg-info/top_level.txt
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-06 02:35:57.657621 auto-eval-0.1.6/commands/
--rw-r--r--   0 zhangchong   (501) staff       (20)        0 2023-04-28 08:32:15.000000 auto-eval-0.1.6/commands/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     3909 2023-05-06 02:28:33.000000 auto-eval-0.1.6/commands/auto_eval.py
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-06 02:35:57.658261 auto-eval-0.1.6/eval/
--rw-r--r--   0 zhangchong   (501) staff       (20)      131 2023-05-05 08:11:08.000000 auto-eval-0.1.6/eval/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     7001 2023-05-06 02:22:59.000000 auto-eval-0.1.6/eval/auto_llms_eval.py
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-06 02:35:57.659140 auto-eval-0.1.6/prompt_template/
--rw-r--r--   0 zhangchong   (501) staff       (20)       44 2023-05-05 07:40:16.000000 auto-eval-0.1.6/prompt_template/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)      775 2023-05-06 02:34:00.000000 auto-eval-0.1.6/prompt_template/eval_prompt_template.json
--rw-r--r--   0 zhangchong   (501) staff       (20)     2949 2023-05-06 02:34:42.000000 auto-eval-0.1.6/prompt_template/prompter.py
--rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-05-06 02:35:57.660297 auto-eval-0.1.6/setup.cfg
--rw-r--r--   0 zhangchong   (501) staff       (20)      940 2023-05-06 02:35:01.000000 auto-eval-0.1.6/setup.py
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-06 02:35:57.659644 auto-eval-0.1.6/utils/
--rw-r--r--   0 zhangchong   (501) staff       (20)       26 2023-04-28 09:40:19.000000 auto-eval-0.1.6/utils/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     2911 2023-05-05 09:52:25.000000 auto-eval-0.1.6/utils/data_utils.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-08 13:26:10.009259 auto-eval-0.1.7/
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1071 2023-04-28 07:53:45.000000 auto-eval-0.1.7/LICENSE
+-rw-r--r--   0 zhangchong   (501) staff       (20)    11522 2023-05-08 13:26:10.008997 auto-eval-0.1.7/PKG-INFO
+-rw-r--r--   0 zhangchong   (501) staff       (20)    11096 2023-05-08 02:17:16.000000 auto-eval-0.1.7/README.md
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-08 13:26:10.006930 auto-eval-0.1.7/auto_eval.egg-info/
+-rw-r--r--   0 zhangchong   (501) staff       (20)    11522 2023-05-08 13:26:09.000000 auto-eval-0.1.7/auto_eval.egg-info/PKG-INFO
+-rw-r--r--   0 zhangchong   (501) staff       (20)      433 2023-05-08 13:26:09.000000 auto-eval-0.1.7/auto_eval.egg-info/SOURCES.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)        1 2023-05-08 13:26:09.000000 auto-eval-0.1.7/auto_eval.egg-info/dependency_links.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)       59 2023-05-08 13:26:09.000000 auto-eval-0.1.7/auto_eval.egg-info/entry_points.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)       49 2023-05-08 13:26:09.000000 auto-eval-0.1.7/auto_eval.egg-info/requires.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)        5 2023-05-08 13:26:09.000000 auto-eval-0.1.7/auto_eval.egg-info/top_level.txt
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-08 13:26:10.007205 auto-eval-0.1.7/eval/
+-rw-r--r--   0 zhangchong   (501) staff       (20)      136 2023-05-08 07:54:51.000000 auto-eval-0.1.7/eval/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     7011 2023-05-08 13:00:48.000000 auto-eval-0.1.7/eval/auto_llms_eval.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-08 13:26:10.007476 auto-eval-0.1.7/eval/commands/
+-rw-r--r--   0 zhangchong   (501) staff       (20)        0 2023-04-28 08:32:15.000000 auto-eval-0.1.7/eval/commands/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     3928 2023-05-08 07:55:11.000000 auto-eval-0.1.7/eval/commands/auto_eval.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-08 13:26:10.008244 auto-eval-0.1.7/eval/prompt_template/
+-rw-r--r--   0 zhangchong   (501) staff       (20)       44 2023-05-05 07:40:16.000000 auto-eval-0.1.7/eval/prompt_template/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     3092 2023-05-08 13:10:10.000000 auto-eval-0.1.7/eval/prompt_template/prompter.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-08 13:26:10.008745 auto-eval-0.1.7/eval/utils/
+-rw-r--r--   0 zhangchong   (501) staff       (20)       26 2023-04-28 09:40:19.000000 auto-eval-0.1.7/eval/utils/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     3108 2023-05-08 13:22:30.000000 auto-eval-0.1.7/eval/utils/data_utils.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-05-08 13:26:10.009314 auto-eval-0.1.7/setup.cfg
+-rw-r--r--   0 zhangchong   (501) staff       (20)      950 2023-05-08 07:57:24.000000 auto-eval-0.1.7/setup.py
```

### Comparing `auto-eval-0.1.6/LICENSE` & `auto-eval-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `auto-eval-0.1.6/PKG-INFO` & `auto-eval-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-eval
-Version: 0.1.6
+Version: 0.1.7
 Summary: Using only one line of commmands to evaluate multiple models
 Home-page: https://github.com/muximus3/Auto-Eval
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -129,18 +129,25 @@
 
 </details>
 
 
 #### Evaluate files
 ```sh
 auto-eval file --config_file CHANGE_TO_YOUR_CONFIG_PATH \
---eval_data_path model_a_pred.json model_b_pred.json  \
+--eval_data_path model_a_pred.json model_b_pred.json model_c_pred.json \
 --output_path eval_result_path.xlsx \
 --model gpt-4 
 ```
+
+**Input file format:**<br>
+The input file currently supports files with .json, .jsonl, .csv, and .xlsx extensions. The headers(column names) of the file can be one of the following types: `{'instruction', 'input', ‘output’}`, `{'prompt', 'output'}`, `{'question', 'answer'}`, or `{'question', 'output'}`.
+
+**Output File format:**<br>
+The output file can be specified as a .json, .jsonl, .csv or.xlsx extension. If it contains a field called "model", scores and statistics will be grouped based on this field. If it also contains fields called "model" and "category", scores and statistics will be grouped based on both fields. Any other fields will not be processed; the output will include all columns from the original input along with evaluation scores and explanations.
+
 <details open> <summary>log output example:</summary>
 
 <br>
 prompts and responses detail...
 
 -------------------- Scores by Model --------------------
 | model                      | score   |
@@ -187,34 +194,31 @@
 
 `--max_new_tokens` integer ${\color{grey}\text{Optional}}$ Defaults to 2048 <br>
 The maximum number of tokens to generate in the chat completion.
 The total length of input tokens and generated tokens is limited by the model's context length.
 
 ### Evaluate one sample arguments
 
-
 `--prompt` string ${\color{orange}\text{Required}}$ <br>
 The question that predicted by LLMs, e.g., A math question would be like: "1+1=?".
 
 `--answers` array ${\color{orange}\text{Required}}$ <br>
 LLMs outputs correspond to the question in the prompt, answers must be separated by space. e.g., A set of four answers would look like this: 1 0 -1 2
 
 `--target` ${\color{grey}\text{Optional}}$ Defaults to \'\'<br> The correct answer for the question. The prompt will be different depending on whether the target is provided, e.g., if no target is provided, the model is asked to solve the question first and then evaluate each candidate answer.
 
 ### Evaluate file arguments
 
 `--eval_data_path`: string ${\color{orange}\text{Required}}$ <br>This refers to the file paths of the input data that will be evaluated. If multiple paths are provided, please ensure that they have identical column names.
 
-**Input file format:**
-The input file currently supports files with .json, .jsonl, .csv, and .xlsx extensions. The header of the file can be one of the following types: `{'instruction', 'input', ‘output’}`, `{'prompt', 'output'}`, `{'question', 'answer'}`, or `{'question', 'output'}`.
+
 
 `--output_path`: string ${\color{orange}\text{Required}}$ <br>The output file path for evaluation results.
 
-**Output File format:**
-The output file can be specified as a .json, .jsonl, .csv or.xlsx extension. If it contains a field called "model", scores and statistics will be grouped based on this field. If it also contains fields called "model" and "category", scores and statistics will be grouped based on both fields. Any other fields will not be processed; the output will include all columns from the original input along with evaluation scores and explanations.
+
 
 `--eval_categories`: array ${\color{grey}\text{Optional}}$ Defaults to null <br> Choose specific types of question categories to evaluate. This only works when the input file contains a "category" column corresponding to each question.
 
 `--sample_num`: number ${\color{grey}\text{Optional}}$ Defaults to 0<br>Sample number of prompt-answer pairs to evaluate.
 
 `--interval`: number ${\color{grey}\text{Optional}}$ Defaults to 1 <br> Sleep interval in seconds between each request to avoid exceeding the request rate limit. A larger value like 10 is recommended for GPT-4.
```

### Comparing `auto-eval-0.1.6/README.md` & `auto-eval-0.1.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -117,18 +117,25 @@
 
 </details>
 
 
 #### Evaluate files
 ```sh
 auto-eval file --config_file CHANGE_TO_YOUR_CONFIG_PATH \
---eval_data_path model_a_pred.json model_b_pred.json  \
+--eval_data_path model_a_pred.json model_b_pred.json model_c_pred.json \
 --output_path eval_result_path.xlsx \
 --model gpt-4 
 ```
+
+**Input file format:**<br>
+The input file currently supports files with .json, .jsonl, .csv, and .xlsx extensions. The headers(column names) of the file can be one of the following types: `{'instruction', 'input', ‘output’}`, `{'prompt', 'output'}`, `{'question', 'answer'}`, or `{'question', 'output'}`.
+
+**Output File format:**<br>
+The output file can be specified as a .json, .jsonl, .csv or.xlsx extension. If it contains a field called "model", scores and statistics will be grouped based on this field. If it also contains fields called "model" and "category", scores and statistics will be grouped based on both fields. Any other fields will not be processed; the output will include all columns from the original input along with evaluation scores and explanations.
+
 <details open> <summary>log output example:</summary>
 
 <br>
 prompts and responses detail...
 
 -------------------- Scores by Model --------------------
 | model                      | score   |
@@ -175,34 +182,31 @@
 
 `--max_new_tokens` integer ${\color{grey}\text{Optional}}$ Defaults to 2048 <br>
 The maximum number of tokens to generate in the chat completion.
 The total length of input tokens and generated tokens is limited by the model's context length.
 
 ### Evaluate one sample arguments
 
-
 `--prompt` string ${\color{orange}\text{Required}}$ <br>
 The question that predicted by LLMs, e.g., A math question would be like: "1+1=?".
 
 `--answers` array ${\color{orange}\text{Required}}$ <br>
 LLMs outputs correspond to the question in the prompt, answers must be separated by space. e.g., A set of four answers would look like this: 1 0 -1 2
 
 `--target` ${\color{grey}\text{Optional}}$ Defaults to \'\'<br> The correct answer for the question. The prompt will be different depending on whether the target is provided, e.g., if no target is provided, the model is asked to solve the question first and then evaluate each candidate answer.
 
 ### Evaluate file arguments
 
 `--eval_data_path`: string ${\color{orange}\text{Required}}$ <br>This refers to the file paths of the input data that will be evaluated. If multiple paths are provided, please ensure that they have identical column names.
 
-**Input file format:**
-The input file currently supports files with .json, .jsonl, .csv, and .xlsx extensions. The header of the file can be one of the following types: `{'instruction', 'input', ‘output’}`, `{'prompt', 'output'}`, `{'question', 'answer'}`, or `{'question', 'output'}`.
+
 
 `--output_path`: string ${\color{orange}\text{Required}}$ <br>The output file path for evaluation results.
 
-**Output File format:**
-The output file can be specified as a .json, .jsonl, .csv or.xlsx extension. If it contains a field called "model", scores and statistics will be grouped based on this field. If it also contains fields called "model" and "category", scores and statistics will be grouped based on both fields. Any other fields will not be processed; the output will include all columns from the original input along with evaluation scores and explanations.
+
 
 `--eval_categories`: array ${\color{grey}\text{Optional}}$ Defaults to null <br> Choose specific types of question categories to evaluate. This only works when the input file contains a "category" column corresponding to each question.
 
 `--sample_num`: number ${\color{grey}\text{Optional}}$ Defaults to 0<br>Sample number of prompt-answer pairs to evaluate.
 
 `--interval`: number ${\color{grey}\text{Optional}}$ Defaults to 1 <br> Sleep interval in seconds between each request to avoid exceeding the request rate limit. A larger value like 10 is recommended for GPT-4.
```

### Comparing `auto-eval-0.1.6/auto_eval.egg-info/PKG-INFO` & `auto-eval-0.1.7/auto_eval.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-eval
-Version: 0.1.6
+Version: 0.1.7
 Summary: Using only one line of commmands to evaluate multiple models
 Home-page: https://github.com/muximus3/Auto-Eval
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -129,18 +129,25 @@
 
 </details>
 
 
 #### Evaluate files
 ```sh
 auto-eval file --config_file CHANGE_TO_YOUR_CONFIG_PATH \
---eval_data_path model_a_pred.json model_b_pred.json  \
+--eval_data_path model_a_pred.json model_b_pred.json model_c_pred.json \
 --output_path eval_result_path.xlsx \
 --model gpt-4 
 ```
+
+**Input file format:**<br>
+The input file currently supports files with .json, .jsonl, .csv, and .xlsx extensions. The headers(column names) of the file can be one of the following types: `{'instruction', 'input', ‘output’}`, `{'prompt', 'output'}`, `{'question', 'answer'}`, or `{'question', 'output'}`.
+
+**Output File format:**<br>
+The output file can be specified as a .json, .jsonl, .csv or.xlsx extension. If it contains a field called "model", scores and statistics will be grouped based on this field. If it also contains fields called "model" and "category", scores and statistics will be grouped based on both fields. Any other fields will not be processed; the output will include all columns from the original input along with evaluation scores and explanations.
+
 <details open> <summary>log output example:</summary>
 
 <br>
 prompts and responses detail...
 
 -------------------- Scores by Model --------------------
 | model                      | score   |
@@ -187,34 +194,31 @@
 
 `--max_new_tokens` integer ${\color{grey}\text{Optional}}$ Defaults to 2048 <br>
 The maximum number of tokens to generate in the chat completion.
 The total length of input tokens and generated tokens is limited by the model's context length.
 
 ### Evaluate one sample arguments
 
-
 `--prompt` string ${\color{orange}\text{Required}}$ <br>
 The question that predicted by LLMs, e.g., A math question would be like: "1+1=?".
 
 `--answers` array ${\color{orange}\text{Required}}$ <br>
 LLMs outputs correspond to the question in the prompt, answers must be separated by space. e.g., A set of four answers would look like this: 1 0 -1 2
 
 `--target` ${\color{grey}\text{Optional}}$ Defaults to \'\'<br> The correct answer for the question. The prompt will be different depending on whether the target is provided, e.g., if no target is provided, the model is asked to solve the question first and then evaluate each candidate answer.
 
 ### Evaluate file arguments
 
 `--eval_data_path`: string ${\color{orange}\text{Required}}$ <br>This refers to the file paths of the input data that will be evaluated. If multiple paths are provided, please ensure that they have identical column names.
 
-**Input file format:**
-The input file currently supports files with .json, .jsonl, .csv, and .xlsx extensions. The header of the file can be one of the following types: `{'instruction', 'input', ‘output’}`, `{'prompt', 'output'}`, `{'question', 'answer'}`, or `{'question', 'output'}`.
+
 
 `--output_path`: string ${\color{orange}\text{Required}}$ <br>The output file path for evaluation results.
 
-**Output File format:**
-The output file can be specified as a .json, .jsonl, .csv or.xlsx extension. If it contains a field called "model", scores and statistics will be grouped based on this field. If it also contains fields called "model" and "category", scores and statistics will be grouped based on both fields. Any other fields will not be processed; the output will include all columns from the original input along with evaluation scores and explanations.
+
 
 `--eval_categories`: array ${\color{grey}\text{Optional}}$ Defaults to null <br> Choose specific types of question categories to evaluate. This only works when the input file contains a "category" column corresponding to each question.
 
 `--sample_num`: number ${\color{grey}\text{Optional}}$ Defaults to 0<br>Sample number of prompt-answer pairs to evaluate.
 
 `--interval`: number ${\color{grey}\text{Optional}}$ Defaults to 1 <br> Sleep interval in seconds between each request to avoid exceeding the request rate limit. A larger value like 10 is recommended for GPT-4.
```

### Comparing `auto-eval-0.1.6/commands/auto_eval.py` & `auto-eval-0.1.7/eval/commands/auto_eval.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import sys
 import argparse
 from oneapi import OneAPITool
-sys.path.append(os.path.normpath(f"{os.path.dirname(os.path.abspath(__file__))}/.."))
+sys.path.append(os.path.normpath(f"{os.path.dirname(os.path.abspath(__file__))}/../../"))
 from eval import eval_one_group, eval_one_qa, eval_groups, EvalConfig
-from utils.data_utils import df_reader
-import prompt_template
+from eval.utils.data_utils import df_reader
+from eval import prompt_template
     
 def add_shared_arguments(parser):
     parser.add_argument("-c", "--config_file", type=str, help="config file path", required=True)
     parser.add_argument("-tp", "--template_path", type=str, default=None, help="eval prompt template path", required=False)
     parser.add_argument("-v", "--verbose", type=bool, default=True, help="print every prompt and response detail", required=False)
     parser.add_argument("-m", "--model", type=str, default="", help="evaluate model name, e.g., gpt-35-turbo, gpt-4", required=False)
     parser.add_argument("-te", "--temperature", type=float, default=0.1, help="0-1, higher temperature more random result", required=False)
```

### Comparing `auto-eval-0.1.6/eval/auto_llms_eval.py` & `auto-eval-0.1.7/eval/auto_llms_eval.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 from tqdm import tqdm
 from typing import Optional, Tuple
 import time
 import sys
 from dataclasses import dataclass
 from oneapi import OneAPITool
 sys.path.append(os.path.normpath(f'{os.path.dirname(os.path.abspath(__file__))}/..'))
-from utils import df_saver, df_reader
-from prompt_template import Prompter
+from eval.utils import df_saver, df_reader
+from eval.prompt_template import Prompter
 
 
 def eval_one_qa(
              api_tool: OneAPITool,
              eval_prompter: Prompter,
              question: str,
              candidate_answers: List[str],
```

### Comparing `auto-eval-0.1.6/prompt_template/prompter.py` & `auto-eval-0.1.7/eval/prompt_template/prompter.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 from typing import List
 import abc
 import json
-from utils import load_json, generate_letters, extract_last_json, extract_numbers
+from eval.utils import load_json, generate_letters, extract_last_json, extract_scores
 
 class Prompter(abc.ABC):
     @abc.abstractmethod
     def generate_prompt(**kwargs):
         raise NotImplementedError
     
     @abc.abstractmethod
@@ -62,10 +62,13 @@
         """
         Extract the result (scores) from the given model response.
         """
         if self._verbose:
             print(
                 f"{'-'*20} response detail ⭐️ {'-'*20}\n\n{response}\n\n{'-'*20} response end {'-'*20}\n"
             )
-        result_json = extract_last_json(response.strip())
+        try:
+            result_json = extract_last_json(response.strip())
+        except (AttributeError, json.decoder.JSONDecodeError):
+            result_json = extract_scores(response.strip())
         scores = list(map(lambda x: float(x), result_json.values()))
         return scores
```

### Comparing `auto-eval-0.1.6/setup.py` & `auto-eval-0.1.7/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from setuptools import setup, find_packages
 
 setup(
     name="auto-eval",
-    version="0.1.6",
+    version="0.1.7",
     packages=find_packages(),
     package_data={
-      "prompt_template":["eval_prompt_template.json"]  
+      "eval/prompt_template":["eval_prompt_template.json"]  
     },
     install_requires=[
         # Add your library's dependencies here
         "one-api-tool",
         "pandas",
         "openpyxl",
         "tabulate",
         "XlsxWriter"
     ],
     entry_points={
         "console_scripts": [
-            "auto-eval=commands.auto_eval:main",
+            "auto-eval=eval.commands.auto_eval:main",
         ]
     },
     description="Using only one line of commmands to evaluate multiple models",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/muximus3/Auto-Eval",
     classifiers=[
```

### Comparing `auto-eval-0.1.6/utils/data_utils.py` & `auto-eval-0.1.7/eval/utils/data_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,14 +43,21 @@
         return single_dict
 
 def extract_last_json(text) -> dict:
     json_str = re.search(r'\{[^}]*\}(?=[^{}]*$)', text).group()
     json_data = json.loads(json_str)
     return json_data
 
+def extract_scores(text) -> dict:
+    pattern = r"([A-Z])'?[:.]\s*([\d.]+)"
+    result = re.findall(pattern, text)
+    scores = {item[0]: float(item[1]) for item in result}    
+    return scores
+
+
 def extract_numbers(text):
     numbers = re.findall(r'\d+', text)
     numbers = [float(number) for number in numbers]
 
 
 def df2xlsx(df: pd.DataFrame, save_path: str, sheet_name='Sheet1', mode='w', index=False):
     if mode not in ['w', 'a']:
```

