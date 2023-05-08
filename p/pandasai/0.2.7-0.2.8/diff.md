# Comparing `tmp/pandasai-0.2.7.tar.gz` & `tmp/pandasai-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandasai-0.2.7.tar", max compression
+gzip compressed data, was "pandasai-0.2.8.tar", max compression
```

## Comparing `pandasai-0.2.7.tar` & `pandasai-0.2.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1055 2023-04-24 05:55:05.323190 pandasai-0.2.7/LICENSE
--rw-r--r--   0        0        0     5641 2023-05-07 22:56:45.170152 pandasai-0.2.7/README.md
--rw-r--r--   0        0        0     7591 2023-05-07 22:54:48.892595 pandasai-0.2.7/pandasai/__init__.py
--rw-r--r--   0        0        0      166 2023-05-08 09:22:18.023055 pandasai-0.2.7/pandasai/constants.py
--rw-r--r--   0        0        0      884 2023-05-02 20:00:39.808655 pandasai-0.2.7/pandasai/exceptions.py
--rw-r--r--   0        0        0        0 2023-05-03 14:53:42.378883 pandasai-0.2.7/pandasai/helpers/__init__.py
--rw-r--r--   0        0        0     4646 2023-05-06 22:56:45.185822 pandasai-0.2.7/pandasai/helpers/anonymizer.py
--rw-r--r--   0        0        0     1505 2023-05-03 14:53:42.379406 pandasai-0.2.7/pandasai/helpers/notebook.py
--rw-r--r--   0        0        0        0 2023-04-30 09:49:31.456755 pandasai-0.2.7/pandasai/llm/__init__.py
--rw-r--r--   0        0        0     1493 2023-05-07 12:19:23.603585 pandasai-0.2.7/pandasai/llm/alpaca.py
--rw-r--r--   0        0        0     3539 2023-05-08 09:22:18.023356 pandasai-0.2.7/pandasai/llm/base.py
--rw-r--r--   0        0        0     1409 2023-05-07 12:19:27.955602 pandasai-0.2.7/pandasai/llm/base_hf.py
--rw-r--r--   0        0        0      505 2023-05-07 12:19:34.602219 pandasai-0.2.7/pandasai/llm/fake.py
--rw-r--r--   0        0        0      755 2023-05-06 12:44:40.587293 pandasai-0.2.7/pandasai/llm/open_assistant.py
--rw-r--r--   0        0        0     3851 2023-05-07 12:17:45.967747 pandasai-0.2.7/pandasai/llm/openai.py
--rw-r--r--   0        0        0      689 2023-05-07 10:03:05.449931 pandasai-0.2.7/pandasai/llm/starcoder.py
--rw-r--r--   0        0        0      728 2023-05-08 09:23:23.460361 pandasai-0.2.7/pyproject.toml
--rw-r--r--   0        0        0     6450 1970-01-01 00:00:00.000000 pandasai-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0     1055 2023-04-24 05:55:05.323190 pandasai-0.2.8/LICENSE
+-rw-r--r--   0        0        0     5641 2023-05-07 22:56:45.170152 pandasai-0.2.8/README.md
+-rw-r--r--   0        0        0     7616 2023-05-08 14:49:29.162424 pandasai-0.2.8/pandasai/__init__.py
+-rw-r--r--   0        0        0      166 2023-05-08 09:22:18.023055 pandasai-0.2.8/pandasai/constants.py
+-rw-r--r--   0        0        0      884 2023-05-02 20:00:39.808655 pandasai-0.2.8/pandasai/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-03 14:53:42.378883 pandasai-0.2.8/pandasai/helpers/__init__.py
+-rw-r--r--   0        0        0     4646 2023-05-06 22:56:45.185822 pandasai-0.2.8/pandasai/helpers/anonymizer.py
+-rw-r--r--   0        0        0     1505 2023-05-03 14:53:42.379406 pandasai-0.2.8/pandasai/helpers/notebook.py
+-rw-r--r--   0        0        0        0 2023-04-30 09:49:31.456755 pandasai-0.2.8/pandasai/llm/__init__.py
+-rw-r--r--   0        0        0     1493 2023-05-07 12:19:23.603585 pandasai-0.2.8/pandasai/llm/alpaca.py
+-rw-r--r--   0        0        0     3539 2023-05-08 09:22:18.023356 pandasai-0.2.8/pandasai/llm/base.py
+-rw-r--r--   0        0        0     1409 2023-05-07 12:19:27.955602 pandasai-0.2.8/pandasai/llm/base_hf.py
+-rw-r--r--   0        0        0      505 2023-05-07 12:19:34.602219 pandasai-0.2.8/pandasai/llm/fake.py
+-rw-r--r--   0        0        0      755 2023-05-06 12:44:40.587293 pandasai-0.2.8/pandasai/llm/open_assistant.py
+-rw-r--r--   0        0        0     3851 2023-05-07 12:17:45.967747 pandasai-0.2.8/pandasai/llm/openai.py
+-rw-r--r--   0        0        0      689 2023-05-07 10:03:05.449931 pandasai-0.2.8/pandasai/llm/starcoder.py
+-rw-r--r--   0        0        0      728 2023-05-08 14:49:36.490884 pandasai-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0     6450 1970-01-01 00:00:00.000000 pandasai-0.2.8/PKG-INFO
```

### Comparing `pandasai-0.2.7/LICENSE` & `pandasai-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pandasai-0.2.7/README.md` & `pandasai-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `pandasai-0.2.7/pandasai/__init__.py` & `pandasai-0.2.8/pandasai/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """ PandasAI is a wrapper around a LLM to make dataframes convesational """
 import io
-import sys
+from contextlib import redirect_stdout
 from datetime import date
 from typing import Optional
 
 import pandas as pd
 
 from .constants import END_CODE_TAG, START_CODE_TAG
 from .exceptions import LLMNotFoundError
@@ -166,46 +166,42 @@
         df: pd.DataFrame,  # pylint: disable=W0613 disable=C0103
         use_error_correction_framework: bool = True,
     ) -> str:
         # pylint: disable=W0122 disable=W0123 disable=W0702:bare-except
         """Run the code in the current context and return the result"""
 
         # Redirect standard output to a StringIO buffer
-        output = io.StringIO()
-        sys.stdout = output
+        with redirect_stdout(io.StringIO()) as output:
+            # Execute the code
+            count = 0
+            code_to_run = code
+            while count < self._max_retries:
+                try:
+                    exec(code_to_run)
+                    code = code_to_run
+                    break
+                except Exception as e:  # pylint: disable=W0718 disable=C0103
+                    if not use_error_correction_framework:
+                        raise e
+
+                    count += 1
+                    error_correcting_instruction = self._error_correct_instruction.format(
+                        today_date=date.today(),
+                        code=code,
+                        error_returned=e,
+                        START_CODE_TAG=START_CODE_TAG,
+                        END_CODE_TAG=END_CODE_TAG,
+                        question=self._original_instructions["question"],
+                        df_head=self._original_instructions["df_head"],
+                        num_rows=self._original_instructions["num_rows"],
+                        num_columns=self._original_instructions["num_columns"],
+                        rows_to_display=self._original_instructions["rows_to_display"],
+                    )
+                    code_to_run = self._llm.generate_code(error_correcting_instruction, "")
 
-        # Execute the code
-        count = 0
-        code_to_run = code
-        while count < self._max_retries:
-            try:
-                exec(code_to_run)
-                code = code_to_run
-                break
-            except Exception as e:  # pylint: disable=W0718 disable=C0103
-                if not use_error_correction_framework:
-                    raise e
-
-                count += 1
-                error_correcting_instruction = self._error_correct_instruction.format(
-                    today_date=date.today(),
-                    code=code,
-                    error_returned=e,
-                    START_CODE_TAG=START_CODE_TAG,
-                    END_CODE_TAG=END_CODE_TAG,
-                    question=self._original_instructions["question"],
-                    df_head=self._original_instructions["df_head"],
-                    num_rows=self._original_instructions["num_rows"],
-                    num_columns=self._original_instructions["num_columns"],
-                    rows_to_display=self._original_instructions["rows_to_display"],
-                )
-                code_to_run = self._llm.generate_code(error_correcting_instruction, "")
-
-        # Restore standard output and get the captured output
-        sys.stdout = sys.__stdout__
         captured_output = output.getvalue()
 
         # Evaluate the last line and return its value or the captured output
         lines = code.strip().split("\n")
         last_line = lines[-1].strip()
         if last_line.startswith("print(") and last_line.endswith(")"):
             last_line = last_line[6:-1]
```

### Comparing `pandasai-0.2.7/pandasai/exceptions.py` & `pandasai-0.2.8/pandasai/exceptions.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.2.7/pandasai/helpers/anonymizer.py` & `pandasai-0.2.8/pandasai/helpers/anonymizer.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.2.7/pandasai/helpers/notebook.py` & `pandasai-0.2.8/pandasai/helpers/notebook.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.2.7/pandasai/llm/alpaca.py` & `pandasai-0.2.8/pandasai/llm/alpaca.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.2.7/pandasai/llm/base.py` & `pandasai-0.2.8/pandasai/llm/base.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.2.7/pandasai/llm/base_hf.py` & `pandasai-0.2.8/pandasai/llm/base_hf.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.2.7/pandasai/llm/open_assistant.py` & `pandasai-0.2.8/pandasai/llm/open_assistant.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.2.7/pandasai/llm/openai.py` & `pandasai-0.2.8/pandasai/llm/openai.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.2.7/pandasai/llm/starcoder.py` & `pandasai-0.2.8/pandasai/llm/starcoder.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.2.7/pyproject.toml` & `pandasai-0.2.8/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pandasai"
-version = "0.2.7"
+version = "0.2.8"
 description = "Pandas AI is a Python library that integrates generative artificial intelligence capabilities into Pandas, making dataframes conversational."
 authors = ["Gabriele Venturi"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pandasai"}]
 
 [tool.poetry.dependencies]
```

### Comparing `pandasai-0.2.7/PKG-INFO` & `pandasai-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandasai
-Version: 0.2.7
+Version: 0.2.8
 Summary: Pandas AI is a Python library that integrates generative artificial intelligence capabilities into Pandas, making dataframes conversational.
 License: MIT
 Author: Gabriele Venturi
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

