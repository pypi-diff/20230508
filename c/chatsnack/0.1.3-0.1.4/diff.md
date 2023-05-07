# Comparing `tmp/chatsnack-0.1.3.tar.gz` & `tmp/chatsnack-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatsnack-0.1.3.tar", max compression
+gzip compressed data, was "chatsnack-0.1.4.tar", max compression
```

## Comparing `chatsnack-0.1.3.tar` & `chatsnack-0.1.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     3795 2023-04-15 22:05:43.794976 chatsnack-0.1.3/chatsnack/__init__.py
--rw-r--r--   0        0        0     5793 2023-04-23 19:18:42.180282 chatsnack-0.1.3/chatsnack/aiwrapper.py
--rw-r--r--   0        0        0     1498 2023-04-09 18:26:53.563580 chatsnack-0.1.3/chatsnack/asynchelpers.py
--rw-r--r--   0        0        0     4486 2023-04-29 02:58:40.680324 chatsnack-0.1.3/chatsnack/chat/__init__.py
--rw-r--r--   0        0        0     6844 2023-04-29 03:01:10.662761 chatsnack-0.1.3/chatsnack/chat/mixin_messages.py
--rw-r--r--   0        0        0     4948 2023-04-29 14:36:32.098051 chatsnack-0.1.3/chatsnack/chat/mixin_params.py
--rw-r--r--   0        0        0     6966 2023-04-29 03:01:48.045271 chatsnack-0.1.3/chatsnack/chat/mixin_query.py
--rw-r--r--   0        0        0     3345 2023-04-23 15:02:14.751611 chatsnack-0.1.3/chatsnack/chat/mixin_serialization.py
--rw-r--r--   0        0        0      929 2023-04-09 15:02:47.382274 chatsnack-0.1.3/chatsnack/defaults.py
--rw-r--r--   0        0        0     1306 2023-04-09 15:11:16.782131 chatsnack-0.1.3/chatsnack/fillings.py
--rw-r--r--   0        0        0       25 2023-04-09 16:04:20.190406 chatsnack-0.1.3/chatsnack/packs/__init__.py
--rw-r--r--   0        0        0    19461 2023-04-14 02:01:22.528095 chatsnack-0.1.3/chatsnack/packs/default_packs/ChatsnackHelper.yml
--rw-r--r--   0        0        0      762 2023-04-14 02:00:30.545934 chatsnack-0.1.3/chatsnack/packs/default_packs/Chester.yml
--rw-r--r--   0        0        0      811 2023-04-14 01:57:06.309659 chatsnack-0.1.3/chatsnack/packs/default_packs/Confectioner.yml
--rw-r--r--   0        0        0      889 2023-04-14 01:57:06.272212 chatsnack-0.1.3/chatsnack/packs/default_packs/Data.yml
--rw-r--r--   0        0        0      736 2023-04-14 01:57:06.293264 chatsnack-0.1.3/chatsnack/packs/default_packs/Jane.yml
--rw-r--r--   0        0        0      905 2023-04-14 01:57:06.327853 chatsnack-0.1.3/chatsnack/packs/default_packs/Jolly.yml
--rw-r--r--   0        0        0     1244 2023-04-23 18:55:56.684760 chatsnack-0.1.3/chatsnack/packs/default_packs/Summarizer.yml
--rw-r--r--   0        0        0     2877 2023-05-03 23:27:38.108990 chatsnack-0.1.3/chatsnack/packs/module_help_vendor.py
--rw-r--r--   0        0        0     4028 2023-04-20 15:50:28.683064 chatsnack-0.1.3/chatsnack/packs/snackpacks.py
--rw-r--r--   0        0        0     1229 2023-04-06 15:39:54.021402 chatsnack-0.1.3/chatsnack/txtformat.py
--rw-r--r--   0        0        0     3976 2023-04-20 00:41:01.746999 chatsnack-0.1.3/chatsnack/yamlformat.py
--rw-r--r--   0        0        0     1091 2023-04-14 18:33:08.190283 chatsnack-0.1.3/LICENSE
--rw-r--r--   0        0        0     1005 2023-05-04 00:35:40.333918 chatsnack-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     9186 2023-04-29 00:10:57.640242 chatsnack-0.1.3/README.md
--rw-r--r--   0        0        0    10107 1970-01-01 00:00:00.000000 chatsnack-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     3795 2023-04-15 22:05:43.794976 chatsnack-0.1.4/chatsnack/__init__.py
+-rw-r--r--   0        0        0     5793 2023-04-23 19:18:42.180282 chatsnack-0.1.4/chatsnack/aiwrapper.py
+-rw-r--r--   0        0        0     1498 2023-04-09 18:26:53.563580 chatsnack-0.1.4/chatsnack/asynchelpers.py
+-rw-r--r--   0        0        0     4486 2023-04-29 02:58:40.680324 chatsnack-0.1.4/chatsnack/chat/__init__.py
+-rw-r--r--   0        0        0     6844 2023-04-29 03:01:10.662761 chatsnack-0.1.4/chatsnack/chat/mixin_messages.py
+-rw-r--r--   0        0        0     4959 2023-05-07 23:04:09.343669 chatsnack-0.1.4/chatsnack/chat/mixin_params.py
+-rw-r--r--   0        0        0     6966 2023-04-29 03:01:48.045271 chatsnack-0.1.4/chatsnack/chat/mixin_query.py
+-rw-r--r--   0        0        0     3345 2023-04-23 15:02:14.751611 chatsnack-0.1.4/chatsnack/chat/mixin_serialization.py
+-rw-r--r--   0        0        0      929 2023-04-09 15:02:47.382274 chatsnack-0.1.4/chatsnack/defaults.py
+-rw-r--r--   0        0        0     1306 2023-04-09 15:11:16.782131 chatsnack-0.1.4/chatsnack/fillings.py
+-rw-r--r--   0        0        0       25 2023-04-09 16:04:20.190406 chatsnack-0.1.4/chatsnack/packs/__init__.py
+-rw-r--r--   0        0        0    19461 2023-04-14 02:01:22.528095 chatsnack-0.1.4/chatsnack/packs/default_packs/ChatsnackHelper.yml
+-rw-r--r--   0        0        0      762 2023-04-14 02:00:30.545934 chatsnack-0.1.4/chatsnack/packs/default_packs/Chester.yml
+-rw-r--r--   0        0        0      811 2023-04-14 01:57:06.309659 chatsnack-0.1.4/chatsnack/packs/default_packs/Confectioner.yml
+-rw-r--r--   0        0        0      889 2023-04-14 01:57:06.272212 chatsnack-0.1.4/chatsnack/packs/default_packs/Data.yml
+-rw-r--r--   0        0        0      736 2023-04-14 01:57:06.293264 chatsnack-0.1.4/chatsnack/packs/default_packs/Jane.yml
+-rw-r--r--   0        0        0      905 2023-04-14 01:57:06.327853 chatsnack-0.1.4/chatsnack/packs/default_packs/Jolly.yml
+-rw-r--r--   0        0        0     1244 2023-04-23 18:55:56.684760 chatsnack-0.1.4/chatsnack/packs/default_packs/Summarizer.yml
+-rw-r--r--   0        0        0     2877 2023-05-03 23:27:38.108990 chatsnack-0.1.4/chatsnack/packs/module_help_vendor.py
+-rw-r--r--   0        0        0     4028 2023-04-20 15:50:28.683064 chatsnack-0.1.4/chatsnack/packs/snackpacks.py
+-rw-r--r--   0        0        0     1229 2023-04-06 15:39:54.021402 chatsnack-0.1.4/chatsnack/txtformat.py
+-rw-r--r--   0        0        0     3976 2023-04-20 00:41:01.746999 chatsnack-0.1.4/chatsnack/yamlformat.py
+-rw-r--r--   0        0        0     1091 2023-04-14 18:33:08.190283 chatsnack-0.1.4/LICENSE
+-rw-r--r--   0        0        0     1005 2023-05-07 23:05:00.479706 chatsnack-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     9186 2023-04-29 00:10:57.640242 chatsnack-0.1.4/README.md
+-rw-r--r--   0        0        0    10107 1970-01-01 00:00:00.000000 chatsnack-0.1.4/PKG-INFO
```

### Comparing `chatsnack-0.1.3/chatsnack/__init__.py` & `chatsnack-0.1.4/chatsnack/__init__.py`

 * *Files identical despite different names*

### Comparing `chatsnack-0.1.3/chatsnack/aiwrapper.py` & `chatsnack-0.1.4/chatsnack/aiwrapper.py`

 * *Files identical despite different names*

### Comparing `chatsnack-0.1.3/chatsnack/asynchelpers.py` & `chatsnack-0.1.4/chatsnack/asynchelpers.py`

 * *Files identical despite different names*

### Comparing `chatsnack-0.1.3/chatsnack/chat/__init__.py` & `chatsnack-0.1.4/chatsnack/chat/__init__.py`

 * *Files identical despite different names*

### Comparing `chatsnack-0.1.3/chatsnack/chat/mixin_messages.py` & `chatsnack-0.1.4/chatsnack/chat/mixin_messages.py`

 * *Files identical despite different names*

### Comparing `chatsnack-0.1.3/chatsnack/chat/mixin_params.py` & `chatsnack-0.1.4/chatsnack/chat/mixin_params.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,15 +91,15 @@
         return pattern
     def filter_by_pattern(self, text: str) -> Optional[str]:
         """ Filters the response given a regex pattern.  """
         if self.pattern is None:
             return text
         return ChatParamsMixin._search_pattern(self.pattern, text)
     def _search_pattern(pattern: str, text: str) -> Optional[str]:
-        matches = re.finditer(pattern, text)
+        matches = re.finditer(pattern, text, re.DOTALL)
 
         try:
             first_match = next(matches)
         except StopIteration:
             return None
 
         if len(first_match.groups()) > 0:
```

### Comparing `chatsnack-0.1.3/chatsnack/chat/mixin_query.py` & `chatsnack-0.1.4/chatsnack/chat/mixin_query.py`

 * *Files identical despite different names*

### Comparing `chatsnack-0.1.3/chatsnack/chat/mixin_serialization.py` & `chatsnack-0.1.4/chatsnack/chat/mixin_serialization.py`

 * *Files identical despite different names*

### Comparing `chatsnack-0.1.3/chatsnack/defaults.py` & `chatsnack-0.1.4/chatsnack/defaults.py`

 * *Files identical despite different names*

### Comparing `chatsnack-0.1.3/chatsnack/fillings.py` & `chatsnack-0.1.4/chatsnack/fillings.py`

 * *Files identical despite different names*

### Comparing `chatsnack-0.1.3/chatsnack/packs/default_packs/ChatsnackHelper.yml` & `chatsnack-0.1.4/chatsnack/packs/default_packs/ChatsnackHelper.yml`

 * *Files identical despite different names*

### Comparing `chatsnack-0.1.3/chatsnack/packs/default_packs/Chester.yml` & `chatsnack-0.1.4/chatsnack/packs/default_packs/Chester.yml`

 * *Files identical despite different names*

### Comparing `chatsnack-0.1.3/chatsnack/packs/default_packs/Confectioner.yml` & `chatsnack-0.1.4/chatsnack/packs/default_packs/Confectioner.yml`

 * *Files identical despite different names*

### Comparing `chatsnack-0.1.3/chatsnack/packs/default_packs/Data.yml` & `chatsnack-0.1.4/chatsnack/packs/default_packs/Data.yml`

 * *Files identical despite different names*

### Comparing `chatsnack-0.1.3/chatsnack/packs/default_packs/Jane.yml` & `chatsnack-0.1.4/chatsnack/packs/default_packs/Jane.yml`

 * *Files identical despite different names*

### Comparing `chatsnack-0.1.3/chatsnack/packs/default_packs/Jolly.yml` & `chatsnack-0.1.4/chatsnack/packs/default_packs/Jolly.yml`

 * *Files identical despite different names*

### Comparing `chatsnack-0.1.3/chatsnack/packs/default_packs/Summarizer.yml` & `chatsnack-0.1.4/chatsnack/packs/default_packs/Summarizer.yml`

 * *Files identical despite different names*

### Comparing `chatsnack-0.1.3/chatsnack/packs/module_help_vendor.py` & `chatsnack-0.1.4/chatsnack/packs/module_help_vendor.py`

 * *Files identical despite different names*

### Comparing `chatsnack-0.1.3/chatsnack/packs/snackpacks.py` & `chatsnack-0.1.4/chatsnack/packs/snackpacks.py`

 * *Files identical despite different names*

### Comparing `chatsnack-0.1.3/chatsnack/txtformat.py` & `chatsnack-0.1.4/chatsnack/txtformat.py`

 * *Files identical despite different names*

### Comparing `chatsnack-0.1.3/chatsnack/yamlformat.py` & `chatsnack-0.1.4/chatsnack/yamlformat.py`

 * *Files identical despite different names*

### Comparing `chatsnack-0.1.3/LICENSE` & `chatsnack-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `chatsnack-0.1.3/pyproject.toml` & `chatsnack-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chatsnack"
-version = "0.1.3"
+version = "0.1.4"
 description = "chatsnack is the easiest Python library for rapid development with OpenAI's ChatGPT API. It provides an intuitive interface for creating and managing chat-based prompts and responses, making it convenient to build complex, interactive conversations with AI."
 authors = ["Mattie Casper"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `chatsnack-0.1.3/README.md` & `chatsnack-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `chatsnack-0.1.3/PKG-INFO` & `chatsnack-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatsnack
-Version: 0.1.3
+Version: 0.1.4
 Summary: chatsnack is the easiest Python library for rapid development with OpenAI's ChatGPT API. It provides an intuitive interface for creating and managing chat-based prompts and responses, making it convenient to build complex, interactive conversations with AI.
 License: MIT
 Author: Mattie Casper
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

