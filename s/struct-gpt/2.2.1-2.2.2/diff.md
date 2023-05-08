# Comparing `tmp/struct_gpt-2.2.1.tar.gz` & `tmp/struct_gpt-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "struct_gpt-2.2.1.tar", last modified: Mon May  8 20:36:36 2023, max compression
+gzip compressed data, was "struct_gpt-2.2.2.tar", last modified: Mon May  8 20:46:55 2023, max compression
```

## Comparing `struct_gpt-2.2.1.tar` & `struct_gpt-2.2.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1076 2023-05-08 20:35:51.100709 struct_gpt-2.2.1/LICENSE
--rw-r--r--   0        0        0     3726 2023-05-08 20:35:51.100709 struct_gpt-2.2.1/README.md
--rw-r--r--   0        0        0      587 2023-05-08 20:36:36.924785 struct_gpt-2.2.1/pyproject.toml
--rw-r--r--   0        0        0       44 2023-05-08 20:35:51.104709 struct_gpt-2.2.1/struct_gpt/__init__.py
--rw-r--r--   0        0        0     4909 2023-05-08 20:35:51.104709 struct_gpt-2.2.1/struct_gpt/models.py
--rw-r--r--   0        0        0     6096 2023-05-08 20:35:51.104709 struct_gpt-2.2.1/tests/test_models.py
--rw-r--r--   0        0        0     5347 1970-01-01 00:00:00.000000 struct_gpt-2.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-05-08 20:46:16.710748 struct_gpt-2.2.2/LICENSE
+-rw-r--r--   0        0        0     3843 2023-05-08 20:46:16.710748 struct_gpt-2.2.2/README.md
+-rw-r--r--   0        0        0      587 2023-05-08 20:46:55.634556 struct_gpt-2.2.2/pyproject.toml
+-rw-r--r--   0        0        0       44 2023-05-08 20:46:16.710748 struct_gpt-2.2.2/struct_gpt/__init__.py
+-rw-r--r--   0        0        0     4909 2023-05-08 20:46:16.710748 struct_gpt-2.2.2/struct_gpt/models.py
+-rw-r--r--   0        0        0     6096 2023-05-08 20:46:16.710748 struct_gpt-2.2.2/tests/test_models.py
+-rw-r--r--   0        0        0     5464 1970-01-01 00:00:00.000000 struct_gpt-2.2.2/PKG-INFO
```

### Comparing `struct_gpt-2.2.1/LICENSE` & `struct_gpt-2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `struct_gpt-2.2.1/README.md` & `struct_gpt-2.2.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -25,19 +25,22 @@
 
 class SentimentSchema(OpenAiBase):
     """
     Determine the sentiment of the given text:
 
     {content}
     """
+    # 👆this becomes the prompt
 
     sentiment: str = Field(description="Either -1, 0, or 1.")
 
 
-print(SentimentSchema.from_openai(content="I love pizza!").json())
+result = SentimentSchema.from_openai(content="I love pizza!").json()
+                                     # 👆this goes in the prompt
+print(result)
 ```
 outputs:
 ```json
 {
   "sentiment": "1"
 }
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `struct_gpt-2.2.1/pyproject.toml` & `struct_gpt-2.2.2/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 dev = [
     "pytest>=7.3.1",
     "coverage>=7.2.5",
 ]
 
 [project]
 name = "struct-gpt"
-version = "2.2.1"
+version = "2.2.2"
 description = "structured llm outputs"
 authors = [
     { name = "Stephan Fitzpatrick", email = "knowsuchagency@gmail.com" },
 ]
 dependencies = [
     "openai>=0.27.6",
     "pydantic>=1.10.7",
```

### Comparing `struct_gpt-2.2.1/struct_gpt/models.py` & `struct_gpt-2.2.2/struct_gpt/models.py`

 * *Files identical despite different names*

### Comparing `struct_gpt-2.2.1/tests/test_models.py` & `struct_gpt-2.2.2/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `struct_gpt-2.2.1/PKG-INFO` & `struct_gpt-2.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: struct-gpt
-Version: 2.2.1
+Version: 2.2.2
 Summary: structured llm outputs
 Author-Email: Stephan Fitzpatrick <knowsuchagency@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Stephan Fitzpatrick
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -58,19 +58,22 @@
 
 class SentimentSchema(OpenAiBase):
     """
     Determine the sentiment of the given text:
 
     {content}
     """
+    # 👆this becomes the prompt
 
     sentiment: str = Field(description="Either -1, 0, or 1.")
 
 
-print(SentimentSchema.from_openai(content="I love pizza!").json())
+result = SentimentSchema.from_openai(content="I love pizza!").json()
+                                     # 👆this goes in the prompt
+print(result)
 ```
 outputs:
 ```json
 {
   "sentiment": "1"
 }
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

