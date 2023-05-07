# Comparing `tmp/pandasai-0.2.5.tar.gz` & `tmp/pandasai-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandasai-0.2.5.tar", max compression
+gzip compressed data, was "pandasai-0.2.6.tar", max compression
```

## Comparing `pandasai-0.2.5.tar` & `pandasai-0.2.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1055 2023-04-24 05:55:05.323190 pandasai-0.2.5/LICENSE
--rw-r--r--   0        0        0     5641 2023-05-06 14:25:32.707401 pandasai-0.2.5/README.md
--rw-r--r--   0        0        0     6656 2023-05-06 14:25:32.707820 pandasai-0.2.5/pandasai/__init__.py
--rw-r--r--   0        0        0      107 2023-05-06 12:44:40.585715 pandasai-0.2.5/pandasai/constants.py
--rw-r--r--   0        0        0      884 2023-05-02 20:00:39.808655 pandasai-0.2.5/pandasai/exceptions.py
--rw-r--r--   0        0        0        0 2023-05-03 14:53:42.378883 pandasai-0.2.5/pandasai/helpers/__init__.py
--rw-r--r--   0        0        0     4513 2023-05-06 14:25:32.708135 pandasai-0.2.5/pandasai/helpers/anonymizer.py
--rw-r--r--   0        0        0     1505 2023-05-03 14:53:42.379406 pandasai-0.2.5/pandasai/helpers/notebook.py
--rw-r--r--   0        0        0        0 2023-04-30 09:49:31.456755 pandasai-0.2.5/pandasai/llm/__init__.py
--rw-r--r--   0        0        0     1466 2023-05-06 14:21:04.361561 pandasai-0.2.5/pandasai/llm/alpaca.py
--rw-r--r--   0        0        0     3210 2023-05-06 12:44:40.586309 pandasai-0.2.5/pandasai/llm/base.py
--rw-r--r--   0        0        0     1373 2023-05-06 12:44:40.586634 pandasai-0.2.5/pandasai/llm/base_hf.py
--rw-r--r--   0        0        0      478 2023-05-04 23:23:32.559995 pandasai-0.2.5/pandasai/llm/fake.py
--rw-r--r--   0        0        0      755 2023-05-06 12:44:40.587293 pandasai-0.2.5/pandasai/llm/open_assistant.py
--rw-r--r--   0        0        0     3815 2023-05-05 23:28:00.731241 pandasai-0.2.5/pandasai/llm/openai.py
--rw-r--r--   0        0        0      668 2023-05-06 12:44:40.587820 pandasai-0.2.5/pandasai/llm/starcoder.py
--rw-r--r--   0        0        0      695 2023-05-06 14:25:48.769779 pandasai-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     6450 1970-01-01 00:00:00.000000 pandasai-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1055 2023-04-24 05:55:05.323190 pandasai-0.2.6/LICENSE
+-rw-r--r--   0        0        0     5641 2023-05-07 22:56:45.170152 pandasai-0.2.6/README.md
+-rw-r--r--   0        0        0     7591 2023-05-07 22:54:48.892595 pandasai-0.2.6/pandasai/__init__.py
+-rw-r--r--   0        0        0      107 2023-05-06 12:44:40.585715 pandasai-0.2.6/pandasai/constants.py
+-rw-r--r--   0        0        0      884 2023-05-02 20:00:39.808655 pandasai-0.2.6/pandasai/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-03 14:53:42.378883 pandasai-0.2.6/pandasai/helpers/__init__.py
+-rw-r--r--   0        0        0     4646 2023-05-06 22:56:45.185822 pandasai-0.2.6/pandasai/helpers/anonymizer.py
+-rw-r--r--   0        0        0     1505 2023-05-03 14:53:42.379406 pandasai-0.2.6/pandasai/helpers/notebook.py
+-rw-r--r--   0        0        0        0 2023-04-30 09:49:31.456755 pandasai-0.2.6/pandasai/llm/__init__.py
+-rw-r--r--   0        0        0     1493 2023-05-07 12:19:23.603585 pandasai-0.2.6/pandasai/llm/alpaca.py
+-rw-r--r--   0        0        0     3399 2023-05-07 22:56:45.176242 pandasai-0.2.6/pandasai/llm/base.py
+-rw-r--r--   0        0        0     1409 2023-05-07 12:19:27.955602 pandasai-0.2.6/pandasai/llm/base_hf.py
+-rw-r--r--   0        0        0      505 2023-05-07 12:19:34.602219 pandasai-0.2.6/pandasai/llm/fake.py
+-rw-r--r--   0        0        0      755 2023-05-06 12:44:40.587293 pandasai-0.2.6/pandasai/llm/open_assistant.py
+-rw-r--r--   0        0        0     3851 2023-05-07 12:17:45.967747 pandasai-0.2.6/pandasai/llm/openai.py
+-rw-r--r--   0        0        0      689 2023-05-07 10:03:05.449931 pandasai-0.2.6/pandasai/llm/starcoder.py
+-rw-r--r--   0        0        0      728 2023-05-07 23:01:59.186432 pandasai-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0     6450 1970-01-01 00:00:00.000000 pandasai-0.2.6/PKG-INFO
```

### Comparing `pandasai-0.2.5/LICENSE` & `pandasai-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pandasai-0.2.5/README.md` & `pandasai-0.2.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -128,10 +128,10 @@
 
 ### Todo
 
 - [ ] Add support for more LLMs
 - [ ] Make PandasAI available from a CLI
 - [ ] Create a web interface for PandasAI
 - [ ] Add unit tests
-- [ ] Add contributing guidelines
+- [x] Add contributing guidelines
 - [x] Add CI
 - [x] Add support for conversational responses
```

### Comparing `pandasai-0.2.5/pandasai/__init__.py` & `pandasai-0.2.6/pandasai/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """ PandasAI is a wrapper around a LLM to make dataframes convesational """
 import io
 import sys
+from datetime import date
 from typing import Optional
 
 import pandas as pd
 
 from .constants import END_CODE_TAG, START_CODE_TAG
 from .exceptions import LLMNotFoundError
 from .helpers.anonymizer import anonymize_dataframe_head
@@ -13,46 +14,59 @@
 
 
 # pylint: disable=too-many-instance-attributes disable=too-many-arguments
 class PandasAI:
     """PandasAI is a wrapper around a LLM to make dataframes conversational"""
 
     _task_instruction: str = """
-There is a dataframe in pandas (python).
-The name of the dataframe is `df`.
+Today is {today_date}.
+You are provided with a pandas dataframe (df) with {num_rows} rows and {num_columns} columns.
 This is the result of `print(df.head({rows_to_display}))`:
 {df_head}.
 
-Return the python code (do not import anything) and make sure to prefix the python code with {START_CODE_TAG} exactly and suffix the code with {END_CODE_TAG} exactly 
-to get the answer to the following question :
+Return the python code (do not import anything) and make sure to prefix the requested python code with {START_CODE_TAG} exactly and suffix the code with {END_CODE_TAG} exactly to get the answer to the following question:
 """
     _response_instruction: str = """
 Question: {question}
 Answer: {answer}
 
 Rewrite the answer to the question in a conversational way.
 """
 
     _error_correct_instruction: str = """
-    For the task defined below:
-    {orig_task}
-    you generated this python code:
-    {code}
-    and this fails with the following error:
-    {error_returned}
-    Correct the python code and return a new python code (do not import anything) that fixes the above mentioned error.
-    Make sure to prefix the python code with {START_CODE_TAG} exactly and suffix the code with {END_CODE_TAG} exactly.
+Today is {today_date}.
+You are provided with a pandas dataframe (df) with {num_rows} rows and {num_columns} columns.
+This is the result of `print(df.head({rows_to_display}))`:
+{df_head}.
+
+The user asked the following question:
+{question}
+
+You generated this python code:
+{code}
+
+It fails with the following error:
+{error_returned}
+
+Correct the python code and return a new python code (do not import anything) that fixes the above mentioned error. Do not generate the same code again.
+Make sure to prefix the requested python code with {START_CODE_TAG} exactly and suffix the code with {END_CODE_TAG} exactly.
     """
     _llm: LLM
     _verbose: bool = False
     _is_conversational_answer: bool = True
     _enforce_privacy: bool = False
     _max_retries: int = 3
-    _original_instruction_and_prompt = None
     _is_notebook: bool = False
+    _original_instructions: dict = {
+        "question": None,
+        "df_head": None,
+        "num_rows": None,
+        "num_columns": None,
+        "rows_to_display": None,
+    }
     last_code_generated: Optional[str] = None
     code_output: Optional[str] = None
 
     def __init__(
         self,
         llm=None,
         conversational=True,
@@ -86,100 +100,109 @@
     def run(
         self,
         data_frame: pd.DataFrame,
         prompt: str,
         is_conversational_answer: bool = None,
         show_code: bool = False,
         anonymize_df: bool = True,
+        use_error_correction_framework: bool = True,
     ) -> str:
         """Run the LLM with the given prompt"""
         self.log(f"Running PandasAI with {self._llm.type} LLM...")
 
         rows_to_display = 0 if self._enforce_privacy else 5
 
         df_head = data_frame.head(rows_to_display)
         if anonymize_df:
             df_head = anonymize_dataframe_head(df_head)
 
         code = self._llm.generate_code(
             self._task_instruction.format(
+                today_date=date.today(),
                 df_head=df_head,
+                num_rows=data_frame.shape[0],
+                num_columns=data_frame.shape[1],
                 rows_to_display=rows_to_display,
                 START_CODE_TAG=START_CODE_TAG,
                 END_CODE_TAG=END_CODE_TAG,
             ),
             prompt,
         )
-        self._original_instruction_and_prompt = (
-            self._task_instruction.format(
-                df_head=df_head,
-                rows_to_display=rows_to_display,
-                START_CODE_TAG=START_CODE_TAG,
-                END_CODE_TAG=END_CODE_TAG,
-            )
-            + prompt
-        )
+        self._original_instructions = {
+            "question": prompt,
+            "df_head": df_head,
+            "num_rows": data_frame.shape[0],
+            "num_columns": data_frame.shape[1],
+            "rows_to_display": rows_to_display,
+        }
         self.last_code_generated = code
         self.log(
             f"""
 Code generated:
 ```
 {code}
 ```"""
         )
         if show_code and self._in_notebook:
             self.notebook.create_new_cell(code)
 
-        answer = self.run_code(code, data_frame, False)
+        answer = self.run_code(
+            code,
+            data_frame,
+            use_error_correction_framework=use_error_correction_framework,
+        )
         self.code_output = answer
         self.log(f"Answer: {answer}")
 
         if is_conversational_answer is None:
             is_conversational_answer = self._is_conversational_answer
         if is_conversational_answer:
             answer = self.conversational_answer(prompt, code, answer)
             self.log(f"Conversational answer: {answer}")
         return answer
 
     def run_code(
         self,
         code: str,
         df: pd.DataFrame,  # pylint: disable=W0613 disable=C0103
-        use_error_correction_framework: bool = False,
+        use_error_correction_framework: bool = True,
     ) -> str:
         # pylint: disable=W0122 disable=W0123 disable=W0702:bare-except
         """Run the code in the current context and return the result"""
 
         # Redirect standard output to a StringIO buffer
         output = io.StringIO()
         sys.stdout = output
 
         # Execute the code
-        if use_error_correction_framework:
-            count = 0
-            code_to_run = code
-            while count < self._max_retries:
-                try:
-                    exec(code_to_run)
-                    code = code_to_run
-                    break
-                except Exception as e:  # pylint: disable=W0718 disable=C0103
-                    count += 1
-                    error_correcting_instruction = (
-                        self._error_correct_instruction.format(
-                            orig_task=self._original_instruction_and_prompt,
-                            code=code,
-                            error_returned=e,
-                        )
-                    )
-                    code_to_run = self._llm.generate_code(
-                        error_correcting_instruction, ""
-                    )
-        else:
-            exec(code)
+        count = 0
+        code_to_run = code
+        while count < self._max_retries:
+            try:
+                exec(code_to_run)
+                code = code_to_run
+                break
+            except Exception as e:  # pylint: disable=W0718 disable=C0103
+                if not use_error_correction_framework:
+                    raise e
+
+                count += 1
+                error_correcting_instruction = self._error_correct_instruction.format(
+                    today_date=date.today(),
+                    code=code,
+                    error_returned=e,
+                    START_CODE_TAG=START_CODE_TAG,
+                    END_CODE_TAG=END_CODE_TAG,
+                    question=self._original_instructions["question"],
+                    df_head=self._original_instructions["df_head"],
+                    num_rows=self._original_instructions["num_rows"],
+                    num_columns=self._original_instructions["num_columns"],
+                    rows_to_display=self._original_instructions["rows_to_display"],
+                )
+                code_to_run = self._llm.generate_code(error_correcting_instruction, "")
 
         # Restore standard output and get the captured output
         sys.stdout = sys.__stdout__
         captured_output = output.getvalue()
 
         # Evaluate the last line and return its value or the captured output
         lines = code.strip().split("\n")
```

### Comparing `pandasai-0.2.5/pandasai/exceptions.py` & `pandasai-0.2.6/pandasai/exceptions.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.2.5/pandasai/helpers/anonymizer.py` & `pandasai-0.2.6/pandasai/helpers/anonymizer.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,48 +6,48 @@
 import random
 import re
 import string
 
 import pandas as pd
 
 
-def is_valid_email(email):
+def is_valid_email(email: str) -> bool:
     """
     Check if the given email is valid based on regex pattern.
 
     :param email: str, email address to be checked
     :return: bool, True if the email is valid, otherwise False
     """
     email_regex = r"^[a-zA-Z0-9._%+-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,}$"
-    return re.match(email_regex, email)
+    return re.match(email_regex, email) is not None
 
 
-def is_valid_phone_number(phone_number):
+def is_valid_phone_number(phone_number: str) -> bool:
     """
     Check if the given phone number is valid based on regex pattern.
 
     :param phone_number: str, phone number to be checked
     :return: bool, True if the phone number is valid, otherwise False
     """
     pattern = r"\b(?:\+?\d{1,3}[- ]?)?\(?\d{3}\)?[- ]?\d{3}[- ]?\d{4}\b"
-    return re.search(pattern, phone_number)
+    return re.search(pattern, phone_number) is not None
 
 
-def is_valid_credit_card(credit_card_number):
+def is_valid_credit_card(credit_card_number: str) -> bool:
     """
     Check if the given credit card number is valid based on regex pattern.
 
     :param credit_card_number: str, credit card number to be checked
     :return: bool, True if the credit card number is valid, otherwise False
     """
     pattern = r"^\d{4}[- ]?\d{4}[- ]?\d{4}[- ]?\d{4}$"
-    return re.search(pattern, credit_card_number)
+    return re.search(pattern, credit_card_number) is not None
 
 
-def generate_random_email():
+def generate_random_email() -> str:
     """
     Generate a random email address using predefined domains.
 
     :return: str, generated random email address
     """
     domains = [
         "gmail.com",
@@ -63,15 +63,15 @@
     domain = random.choice(domains)
     letters = string.ascii_lowercase + string.digits + "-_"
     username = "".join(random.choice(letters) for i in range(name_length))
     email = username + "@" + domain
     return email
 
 
-def generate_random_phone_number(original_field):
+def generate_random_phone_number(original_field: str) -> str:
     """
     Generate a random phone number with country code if originally present.
 
     :param original_field: str, original phone number field
     :return: str, generated random phone number
     """
     if original_field.startswith("+"):
@@ -86,39 +86,39 @@
         phone_number = f"{country_code} {number}"
     else:
         phone_number = number
 
     return phone_number
 
 
-def generate_random_credit_card():
+def generate_random_credit_card() -> str:
     """
     Generate a random credit card number.
 
     :return: str, generated random credit card number
     """
     groups = []
     for _i in range(4):
         group = "".join(random.choices("0123456789", k=4))
         groups.append(group)
     separator = random.choice(["-", " "])
     return separator.join(groups)
 
 
-def copy_head(data_frame: pd.DataFrame):
+def copy_head(data_frame: pd.DataFrame) -> pd.DataFrame:
     """
     Copy the head of a DataFrame.
 
     :param data_frame: pd.DataFrame, the DataFrame to copy the head from
     :return: pd.DataFrame, copied head of the DataFrame
     """
     return data_frame.head().copy()
 
 
-def anonymize_dataframe_head(data_frame: pd.DataFrame):
+def anonymize_dataframe_head(data_frame: pd.DataFrame) -> pd.DataFrame:
     """
     Anonymize the head of a given DataFrame by replacing sensitive data.
 
     :param data_frame: pd.DataFrame, the DataFrame to anonymize the head
     :return: pd.DataFrame, anonymized head of the DataFrame
     """
     data_frame = copy_head(data_frame)
```

### Comparing `pandasai-0.2.5/pandasai/helpers/notebook.py` & `pandasai-0.2.6/pandasai/helpers/notebook.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.2.5/pandasai/llm/alpaca.py` & `pandasai-0.2.6/pandasai/llm/alpaca.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,17 +28,17 @@
             "top_k",
             "beams",
         ]
         for key, value in kwargs.items():
             if key in valid_params:
                 setattr(self, key, value)
 
-    def call(self, instruction: str, value: str) -> str:
+    def call(self, instruction: str, value: str, suffix: str = "") -> str:
         """Call Alpaca LLM"""
-        self.last_prompt = str(instruction) + str(value)
+        self.last_prompt = str(instruction) + str(value) + suffix
 
         response = requests.post(
             "https://tloen-alpaca-lora.hf.space/run/predict",
             json={
                 "data": [
                     instruction,
                     value,
```

### Comparing `pandasai-0.2.5/pandasai/llm/base.py` & `pandasai-0.2.6/pandasai/llm/base.py`

 * *Files 26% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         tree = ast.parse(code)
         new_body = [
             node
             for node in tree.body
             if not isinstance(node, (ast.Import, ast.ImportFrom))
         ]
         new_tree = ast.Module(body=new_body)
-        return astor.to_source(new_tree)
+        return astor.to_source(new_tree).strip()
 
     def _polish_code(self, code: str) -> str:
         """
         Polish the code by removing the leading "python" or "py",  \
         removing the imports and removing trailing spaces and new lines.
 
         Args:
@@ -53,16 +53,16 @@
         Returns:
             str: Polished code
         """
         if re.match(r"^(python|py)", code):
             code = re.sub(r"^(python|py)", "", code)
         if re.match(r"^`.*`$", code):
             code = re.sub(r"^`(.*)`$", r"\1", code)
-        self._remove_imports(code)
         code = code.strip()
+        code = self._remove_imports(code)
         return code
 
     def _is_python_code(self, string):
         try:
             ast.parse(string)
             return True
         except SyntaxError:
@@ -79,39 +79,44 @@
         Raises:
             NoCodeFoundError: No code found in the response
 
         Returns:
             str: Extracted code from the response
         """
         code = response
-        if len(response.split(separator)) > 1:
-            code = response.split(separator)[1]
-        match = re.search(rf"{START_CODE_TAG}(.*){END_CODE_TAG}", code, re.DOTALL)
+        match = re.search(
+            rf"{START_CODE_TAG}(.*)({END_CODE_TAG}|{END_CODE_TAG.replace('<', '</')})",
+            code,
+            re.DOTALL,
+        )
         if match:
             code = match.group(1).strip()
+        if len(code.split(separator)) > 1:
+            code = code.split(separator)[1]
         code = self._polish_code(code)
         if not self._is_python_code(code):
             raise NoCodeFoundError("No code found in the response")
 
         return code
 
-    def call(self, instruction: str, value: str) -> None:
+    def call(self, instruction: str, value: str, suffix: str = "") -> str:
         """
         Execute the LLM with given prompt.
 
         Args:
             instruction (str): Prompt
             value (str): Value
+            suffix (str, optional): Suffix. Defaults to "".
 
         Raises:
             MethodNotImplementedError: Call method has not been implemented
         """
         raise MethodNotImplementedError("Call method has not been implemented")
 
     def generate_code(self, instruction: str, prompt: str) -> str:
         """
         Generate the code based on the instruction and the given prompt.
 
         Returns:
             str: Code
         """
-        return self._extract_code(self.call(instruction, prompt))
+        return self._extract_code(self.call(instruction, prompt, suffix="\n\nCode:\n"))
```

### Comparing `pandasai-0.2.5/pandasai/llm/base_hf.py` & `pandasai-0.2.6/pandasai/llm/base_hf.py`

 * *Files 16% similar despite different names*

```diff
@@ -26,23 +26,23 @@
 
         response = requests.post(
             self._api_url, headers=headers, json=payload, timeout=60
         )
 
         return response.json()[0]["generated_text"]
 
-    def call(self, instruction: str, value: str) -> str:
+    def call(self, instruction: str, value: str, suffix: str = "") -> str:
         """Call the LLM"""
 
-        payload = instruction + value
+        payload = instruction + value + suffix
 
         # sometimes the API doesn't return a valid response, so we retry passing the
         # output generated from the previous call as the input
         for _i in range(self._max_retries):
             response = self.query({"inputs": payload})
             payload = response
             if response.count("<endCode>") >= 2:
                 break
 
         # replace instruction + value from the inputs to avoid showing it in the output
-        output = response.replace(instruction + value, "")
+        output = response.replace(instruction + value + suffix, "")
         return output
```

### Comparing `pandasai-0.2.5/pandasai/llm/open_assistant.py` & `pandasai-0.2.6/pandasai/llm/open_assistant.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.2.5/pandasai/llm/openai.py` & `pandasai-0.2.6/pandasai/llm/openai.py`

 * *Files 3% similar despite different names*

```diff
@@ -115,15 +115,15 @@
         if self.stop is not None:
             params["stop"] = [self.stop]
 
         response = openai.ChatCompletion.create(**params)
 
         return response["choices"][0]["message"]["content"]
 
-    def call(self, instruction: str, value: str) -> str:
+    def call(self, instruction: str, value: str, suffix: str = "") -> str:
         """
         Call the OpenAI LLM.
 
         Args:
             instruction (str): Instruction to pass
             value (str): Value to pass
 
@@ -132,17 +132,17 @@
 
         Returns:
             str: Response
         """
         self.last_prompt = str(instruction) + str(value)
 
         if self.model in self._supported_completion_models:
-            response = self.completion(str(instruction) + str(value))
+            response = self.completion(str(instruction) + str(value) + suffix)
         elif self.model in self._supported_chat_models:
-            response = self.chat_completion(str(instruction) + str(value))
+            response = self.chat_completion(str(instruction) + str(value) + suffix)
         else:
             raise UnsupportedOpenAIModelError("Unsupported model")
 
         return response
 
     @property
     def type(self) -> str:
```

### Comparing `pandasai-0.2.5/pandasai/llm/starcoder.py` & `pandasai-0.2.6/pandasai/llm/starcoder.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,16 +12,17 @@
 
 
 class Starcoder(HuggingFaceLLM):
     """Starcoder LLM"""
 
     api_token: str
     _api_url: str = "https://api-inference.huggingface.co/models/bigcode/starcoder"
+    _max_retries: int = 5
 
     def __init__(self, api_token: Optional[str] = None):
         self.api_token = api_token or os.getenv("HUGGINGFACE_API_KEY")
         if self.api_token is None:
             raise APIKeyNotFoundError("HuggingFace Hub API key is required")
 
     @property
     def type(self) -> str:
-        return "open-assistant"
+        return "starcoder"
```

### Comparing `pandasai-0.2.5/pyproject.toml` & `pandasai-0.2.6/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pandasai"
-version = "0.2.5"
+version = "0.2.6"
 description = "Pandas AI is a Python library that integrates generative artificial intelligence capabilities into Pandas, making dataframes conversational."
 authors = ["Gabriele Venturi"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pandasai"}]
 
 [tool.poetry.dependencies]
@@ -23,7 +23,10 @@
 pylint = "^2.17.3"
 pytest = "^7.3.1"
 isort = "^5.12.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.pylint]
+ignore = "tests_*"
```

### Comparing `pandasai-0.2.5/PKG-INFO` & `pandasai-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandasai
-Version: 0.2.5
+Version: 0.2.6
 Summary: Pandas AI is a Python library that integrates generative artificial intelligence capabilities into Pandas, making dataframes conversational.
 License: MIT
 Author: Gabriele Venturi
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -148,11 +148,11 @@
 
 ### Todo
 
 - [ ] Add support for more LLMs
 - [ ] Make PandasAI available from a CLI
 - [ ] Create a web interface for PandasAI
 - [ ] Add unit tests
-- [ ] Add contributing guidelines
+- [x] Add contributing guidelines
 - [x] Add CI
 - [x] Add support for conversational responses
```

