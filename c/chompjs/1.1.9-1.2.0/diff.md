# Comparing `tmp/chompjs-1.1.9.tar.gz` & `tmp/chompjs-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chompjs-1.1.9.tar", last modified: Thu Nov 17 00:23:52 2022, max compression
+gzip compressed data, was "chompjs-1.2.0.tar", last modified: Mon May  8 04:46:39 2023, max compression
```

## Comparing `chompjs-1.1.9.tar` & `chompjs-1.2.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 mariusz   (1000) mariusz   (1000)        0 2022-11-17 00:23:52.065678 chompjs-1.1.9/
--rw-r--r--   0 mariusz   (1000) mariusz   (1000)     1062 2020-02-27 18:25:01.000000 chompjs-1.1.9/LICENSE
--rw-rw-r--   0 mariusz   (1000) mariusz   (1000)       15 2022-08-22 13:00:05.000000 chompjs-1.1.9/MANIFEST.in
--rw-rw-r--   0 mariusz   (1000) mariusz   (1000)     7383 2022-11-17 00:23:52.065678 chompjs-1.1.9/PKG-INFO
--rw-rw-r--   0 mariusz   (1000) mariusz   (1000)     6571 2021-12-02 14:53:00.000000 chompjs-1.1.9/README.md
-drwxrwxr-x   0 mariusz   (1000) mariusz   (1000)        0 2022-11-17 00:23:52.061678 chompjs-1.1.9/_chompjs/
--rw-rw-r--   0 mariusz   (1000) mariusz   (1000)     1533 2022-10-15 10:06:35.000000 chompjs-1.1.9/_chompjs/buffer.c
--rw-rw-r--   0 mariusz   (1000) mariusz   (1000)      853 2022-10-15 10:06:25.000000 chompjs-1.1.9/_chompjs/buffer.h
--rw-rw-r--   0 mariusz   (1000) mariusz   (1000)     1968 2021-07-29 16:38:19.000000 chompjs-1.1.9/_chompjs/module.c
--rw-rw-r--   0 mariusz   (1000) mariusz   (1000)    11620 2022-10-16 02:04:13.000000 chompjs-1.1.9/_chompjs/parser.c
--rw-rw-r--   0 mariusz   (1000) mariusz   (1000)     2791 2022-10-15 10:05:50.000000 chompjs-1.1.9/_chompjs/parser.h
-drwxrwxr-x   0 mariusz   (1000) mariusz   (1000)        0 2022-11-17 00:23:52.061678 chompjs-1.1.9/chompjs/
--rw-r--r--   0 mariusz   (1000) mariusz   (1000)       38 2021-04-03 13:26:09.000000 chompjs-1.1.9/chompjs/__init__.py
--rw-rw-r--   0 mariusz   (1000) mariusz   (1000)      634 2022-08-22 10:20:52.000000 chompjs-1.1.9/chompjs/chompjs.py
--rw-rw-r--   0 mariusz   (1000) mariusz   (1000)     7875 2022-10-15 10:16:26.000000 chompjs-1.1.9/chompjs/test_parser.py
-drwxrwxr-x   0 mariusz   (1000) mariusz   (1000)        0 2022-11-17 00:23:52.061678 chompjs-1.1.9/chompjs.egg-info/
--rw-rw-r--   0 mariusz   (1000) mariusz   (1000)     7383 2022-11-17 00:23:52.000000 chompjs-1.1.9/chompjs.egg-info/PKG-INFO
--rw-rw-r--   0 mariusz   (1000) mariusz   (1000)      314 2022-11-17 00:23:52.000000 chompjs-1.1.9/chompjs.egg-info/SOURCES.txt
--rw-rw-r--   0 mariusz   (1000) mariusz   (1000)        1 2022-11-17 00:23:52.000000 chompjs-1.1.9/chompjs.egg-info/dependency_links.txt
--rw-rw-r--   0 mariusz   (1000) mariusz   (1000)       17 2022-11-17 00:23:52.000000 chompjs-1.1.9/chompjs.egg-info/top_level.txt
--rw-rw-r--   0 mariusz   (1000) mariusz   (1000)       38 2022-11-17 00:23:52.065678 chompjs-1.1.9/setup.cfg
--rw-rw-r--   0 mariusz   (1000) mariusz   (1000)     1634 2022-11-17 00:21:49.000000 chompjs-1.1.9/setup.py
+drwxrwxr-x   0 mariusz   (1000) mariusz   (1000)        0 2023-05-08 04:46:39.510076 chompjs-1.2.0/
+-rw-r--r--   0 mariusz   (1000) mariusz   (1000)     1062 2020-02-27 18:25:01.000000 chompjs-1.2.0/LICENSE
+-rw-rw-r--   0 mariusz   (1000) mariusz   (1000)       15 2022-08-22 13:00:05.000000 chompjs-1.2.0/MANIFEST.in
+-rw-rw-r--   0 mariusz   (1000) mariusz   (1000)    10541 2023-05-08 04:46:39.510076 chompjs-1.2.0/PKG-INFO
+-rw-rw-r--   0 mariusz   (1000) mariusz   (1000)     7742 2023-05-08 04:36:34.000000 chompjs-1.2.0/README.md
+drwxrwxr-x   0 mariusz   (1000) mariusz   (1000)        0 2023-05-08 04:46:39.510076 chompjs-1.2.0/_chompjs/
+-rw-rw-r--   0 mariusz   (1000) mariusz   (1000)     1735 2023-04-21 12:26:12.000000 chompjs-1.2.0/_chompjs/buffer.c
+-rw-rw-r--   0 mariusz   (1000) mariusz   (1000)      976 2023-04-21 12:26:15.000000 chompjs-1.2.0/_chompjs/buffer.h
+-rw-rw-r--   0 mariusz   (1000) mariusz   (1000)     5289 2023-05-08 02:40:08.000000 chompjs-1.2.0/_chompjs/module.c
+-rw-rw-r--   0 mariusz   (1000) mariusz   (1000)    12315 2023-05-08 02:40:08.000000 chompjs-1.2.0/_chompjs/parser.c
+-rw-rw-r--   0 mariusz   (1000) mariusz   (1000)     3132 2023-05-08 02:40:08.000000 chompjs-1.2.0/_chompjs/parser.h
+drwxrwxr-x   0 mariusz   (1000) mariusz   (1000)        0 2023-05-08 04:46:39.510076 chompjs-1.2.0/chompjs/
+-rw-rw-r--   0 mariusz   (1000) mariusz   (1000)       55 2023-05-08 02:17:42.000000 chompjs-1.2.0/chompjs/__init__.py
+-rw-rw-r--   0 mariusz   (1000) mariusz   (1000)     3468 2023-05-08 04:32:36.000000 chompjs-1.2.0/chompjs/chompjs.py
+-rw-rw-r--   0 mariusz   (1000) mariusz   (1000)    10944 2023-05-08 03:23:28.000000 chompjs-1.2.0/chompjs/test_parser.py
+drwxrwxr-x   0 mariusz   (1000) mariusz   (1000)        0 2023-05-08 04:46:39.510076 chompjs-1.2.0/chompjs.egg-info/
+-rw-rw-r--   0 mariusz   (1000) mariusz   (1000)    10541 2023-05-08 04:46:39.000000 chompjs-1.2.0/chompjs.egg-info/PKG-INFO
+-rw-rw-r--   0 mariusz   (1000) mariusz   (1000)      314 2023-05-08 04:46:39.000000 chompjs-1.2.0/chompjs.egg-info/SOURCES.txt
+-rw-rw-r--   0 mariusz   (1000) mariusz   (1000)        1 2023-05-08 04:46:39.000000 chompjs-1.2.0/chompjs.egg-info/dependency_links.txt
+-rw-rw-r--   0 mariusz   (1000) mariusz   (1000)       17 2023-05-08 04:46:39.000000 chompjs-1.2.0/chompjs.egg-info/top_level.txt
+-rw-rw-r--   0 mariusz   (1000) mariusz   (1000)       38 2023-05-08 04:46:39.510076 chompjs-1.2.0/setup.cfg
+-rw-rw-r--   0 mariusz   (1000) mariusz   (1000)     1764 2023-05-08 04:45:20.000000 chompjs-1.2.0/setup.py
```

### Comparing `chompjs-1.1.9/LICENSE` & `chompjs-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `chompjs-1.1.9/PKG-INFO` & `chompjs-1.2.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,55 +1,60 @@
-Metadata-Version: 2.1
-Name: chompjs
-Version: 1.1.9
-Summary: Parsing JavaScript objects into Python dictionaries
-Home-page: https://github.com/Nykakin/chompjs
-Author: Mariusz Obajtek
-Author-email: nykakin@gmail.com
-License: UNKNOWN
-Keywords: parsing parser JavaScript json
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: JavaScript
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Text Processing :: General
-Classifier: Topic :: Text Processing :: Linguistic
-Description-Content-Type: text/markdown
-License-File: LICENSE
+# Chompjs
 
-# Usage
+![license](https://img.shields.io/github/license/Nykakin/chompjs?style=flat-square)
+![pypi version](https://img.shields.io/pypi/v/chompjs.svg)
+![python version](https://img.shields.io/pypi/pyversions/chompjs.svg)
+![downloads](https://img.shields.io/pypi/dm/chompjs.svg)
 
-`chompjs` can be used in web scrapping for turning JavaScript objects embedded in pages into valid Python dictionaries.
+Transforms JavaScript objects into Python dictionaries.
+
+In web scraping, you sometimes need to transform Javascript objects embedded in HTML pages into valid Python dictionaries. `chompjs` is a library designed to be a more powerful replacement of standard `json.loads`.
 
 ```python
->>> import chompjs
->>> chompjs.parse_js_object('{"my_data": "test"}')
-{u'my_data': u'test'}
+>>> chompjs.parse_js_object("{a: 100}")
+{'a': 100}
+>>>
+>>> json_lines = """
+... {'a': 12}
+... {'b': 13}
+... {'c': 14}
+... """
+>>> for entry in chompjs.parse_js_objects(json_lines):
+...     print(entry)
+... 
+{'a': 12}
+{'b': 13}
+{'c': 14}
 ```
 
-Think of it as a more powerful `json.loads`. For example, it can handle JSON objects containing embedded methods by storing their code in a string:
+[Reference documentation](https://nykakin.github.io/chompjs/)
 
-```python
->>> import chompjs
->>> js = """
-... var myObj = {
-...     myMethod: function(params) {
-...         // ...
-...     },
-...     myValue: 100
-... }
-... """
->>> chompjs.parse_js_object(js, json_params={'strict': False})
-{'myMethod': 'function(params) {\n        // ...\n    }', 'myValue': 100}
+## Quickstart
+
+**1. installation**
+
+```
+> pip install chompjs
 ```
 
+or build from source:
+
+```bash
+$ git clone https://github.com/Nykakin/chompjs
+$ cd chompjs
+$ python setup.py build
+$ python setup.py install
+```
+
+## Features
+
+There are two functions available:
+* `parse_js_object` - try reading first encountered JSON-like object. Raises `ValueError` on failure
+* `parse_js_objects` - returns a generator yielding all encountered JSON-like objects. Can be used to read [JSON Lines](https://jsonlines.org/)
+
 An example usage with `scrapy`:
 
 ```python
 import chompjs
 import scrapy
 
 
@@ -67,26 +72,40 @@
         except ValueError:
             self.log('Failed to extract data from {}'.format(response.url))
             return
 
         # work on json_data
 ```
 
-If the input string is not yet escaped and contains a lot of `\\` characters, then `unicode_escape=True` argument might help to sanitize it:
+Parsing of [JSON5 objects](https://json5.org/) is supported:
 
 ```python
->>> chompjs.parse_js_object('{\\\"a\\\": 12}', unicode_escape=True)
-{u'a': 12}
+>>> data = """
+... {
+...   // comments
+...   unquoted: 'and you can quote me on that',
+...   singleQuotes: 'I can use "double quotes" here',
+...   lineBreaks: "Look, Mom! \
+... No \\n's!",
+...   hexadecimal: 0xdecaf,
+...   leadingDecimalPoint: .8675309, andTrailing: 8675309.,
+...   positiveSign: +1,
+...   trailingComma: 'in objects', andIn: ['arrays',],
+...   "backwardsCompatible": "with JSON",
+... }
+... """
+>>> chompjs.parse_js_object(data)
+{'unquoted': 'and you can quote me on that', 'singleQuotes': 'I can use "double quotes" here', 'lineBreaks': "Look, Mom! No \n's!", 'hexadecimal': 912559, 'leadingDecimalPoint': 0.8675309, 'andTrailing': 8675309.0, 'positiveSign': '+1', 'trailingComma': 'in objects', 'andIn': ['arrays'], 'backwardsCompatible': 'with JSON'}
 ```
 
-`jsonlines=True` can be used to parse JSON Lines:
+If the input string is not yet escaped and contains a lot of `\\` characters, then `unicode_escape=True` argument might help to sanitize it:
 
 ```python
->>> chompjs.parse_js_object('[1,2]\n[2,3]\n[3,4]', jsonlines=True)
-[[1, 2], [2, 3], [3, 4]]
+>>> chompjs.parse_js_object('{\\\"a\\\": 12}', unicode_escape=True)
+{'a': 12}
 ```
 
 By default `chompjs` tries to start with first `{` or `[` character it founds, omitting the rest:
 
 ```python
 >>> chompjs.parse_js_object('<div>...</div><script>foo = [1, 2, 3];</script><div>...</div>')
 [1, 2, 3]
@@ -135,39 +154,39 @@
 
 As a result, `json.loads` fail to extract any of those:
 
 ```
 >>> json.loads("{'a': 'b'}")
 Traceback (most recent call last):
   File "<console>", line 1, in <module>
-  File "/usr/lib/python2.7/json/__init__.py", line 339, in loads
+  File "/usr/lib/python3.10/json/__init__.py", line 339, in loads
     return _default_decoder.decode(s)
-  File "/usr/lib/python2.7/json/decoder.py", line 364, in decode
+  File "/usr/lib/python3.10/json/decoder.py", line 364, in decode
     obj, end = self.raw_decode(s, idx=_w(s, 0).end())
-  File "/usr/lib/python2.7/json/decoder.py", line 380, in raw_decode
+  File "/usr/lib/python3.10/json/decoder.py", line 380, in raw_decode
     obj, end = self.scan_once(s, idx)
 ValueError: Expecting property name: line 1 column 2 (char 1)
 >>> json.loads('{a: "b"}')
 Traceback (most recent call last):
   File "<console>", line 1, in <module>
-  File "/usr/lib/python2.7/json/__init__.py", line 339, in loads
+  File "/usr/lib/python3.10/json/__init__.py", line 339, in loads
     return _default_decoder.decode(s)
-  File "/usr/lib/python2.7/json/decoder.py", line 364, in decode
+  File "/usr/lib/python3.10/json/decoder.py", line 364, in decode
     obj, end = self.raw_decode(s, idx=_w(s, 0).end())
-  File "/usr/lib/python2.7/json/decoder.py", line 380, in raw_decode
+  File "/usr/lib/python3.10/json/decoder.py", line 380, in raw_decode
     obj, end = self.scan_once(s, idx)
 ValueError: Expecting property name: line 1 column 2 (char 1)
 >>> json.loads('{"a": [1, 2, 3,]}')
 Traceback (most recent call last):
   File "<console>", line 1, in <module>
-  File "/usr/lib/python2.7/json/__init__.py", line 339, in loads
+  File "/usr/lib/python3.10/json/__init__.py", line 339, in loads
     return _default_decoder.decode(s)
-  File "/usr/lib/python2.7/json/decoder.py", line 364, in decode
+  File "/usr/lib/python3.10/json/decoder.py", line 364, in decode
     obj, end = self.raw_decode(s, idx=_w(s, 0).end())
-  File "/usr/lib/python2.7/json/decoder.py", line 382, in raw_decode
+  File "/usr/lib/python3.10/json/decoder.py", line 382, in raw_decode
     raise ValueError("No JSON object could be decoded")
 ValueError: No JSON object could be decoded
 >>> json.loads('{"a": .99}')
 Traceback (most recent call last):
   File "<stdin>", line 1, in <module>
   File "/usr/lib/python3.7/json/__init__.py", line 348, in loads
     return _default_decoder.decode(s)
@@ -201,30 +220,15 @@
 '{"a":1}'
 >>> json.loads(_)
 {u'a': 1}
 >>> chompjs.parse_js_object('{"a": .99}')
 {'a': 0.99}
 ```
 
-# Installation
-From PIP:
-
-```bash
-$ python3 -m venv venv
-$ . venv/bin/activate
-# pip install chompjs
-```
-From sources:
-```bash
-$ git clone https://github.com/Nykakin/chompjs
-$ cd chompjs
-$ python setup.py build
-$ python setup.py install
-```
+# Development
+Pull requests are welcome. 
 
 To run unittests
 
 ```
-$ python -m unittest
+$ tox
 ```
-
-
```

### Comparing `chompjs-1.1.9/_chompjs/buffer.h` & `chompjs-1.2.0/_chompjs/buffer.h`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /*
- * Copyright 2020-2021 Mariusz Obajtek. All rights reserved.
+ * Copyright 2020-2023 Mariusz Obajtek. All rights reserved.
  * License: https://github.com/Nykakin/chompjs/blob/master/LICENSE
  */
 
 #ifndef CHOMPJS_BUFFER_H
 #define CHOMPJS_BUFFER_H
 
 #include <stdbool.h>
@@ -18,18 +18,22 @@
     size_t index;
 };
 
 void init_char_buffer(struct CharBuffer* buffer, size_t initial_depth_buffer_size);
 
 void release_char_buffer(struct CharBuffer* buffer);
 
+void check_capacity(struct CharBuffer* buffer, size_t to_save);
+
 void push(struct CharBuffer* buffer, char value);
 
 void push_string(struct CharBuffer* buffer, const char* value, size_t len);
 
+void push_number(struct CharBuffer* buffer, long value);
+
 void pop(struct CharBuffer* buffer);
 
 char top(struct CharBuffer* buffer);
 
 bool empty(struct CharBuffer* buffer);
 
 void clear(struct CharBuffer* buffer);
```

### Comparing `chompjs-1.1.9/_chompjs/parser.c` & `chompjs-1.2.0/_chompjs/parser.c`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /*
- * Copyright 2020-2021 Mariusz Obajtek. All rights reserved.
+ * Copyright 2020-2023 Mariusz Obajtek. All rights reserved.
  * License: https://github.com/Nykakin/chompjs/blob/master/LICENSE
  */
 
 #include "parser.h"
 
 #include <stdio.h>
 #include <stdlib.h>
@@ -62,30 +62,41 @@
     lexer->input_position += size;   
 }
 
 void emit_string_in_place(const char *s, size_t size, struct Lexer* lexer) {
     push_string(&lexer->output, s, size);
 }
 
-void init_lexer(struct Lexer* lexer, const char* string, bool is_jsonlines) {
+void emit_number_in_place(long value, struct Lexer* lexer) {
+    push_number(&lexer->output, value);
+}
+
+void init_lexer(struct Lexer* lexer, const char* string) {
     lexer->input = string;
     // allocate in advance more memory for output than for input because we might need
     // to add extra characters
     // for example `{a: undefined}` will be translated as `{"a": "undefined"}`
     lexer->output_size = 2 * strlen(string);
     init_char_buffer(&lexer->output, lexer->output_size);
     lexer->input_position = 0;
     init_char_buffer(&lexer->nesting_depth, INITIAL_NESTING_DEPTH);
     lexer->unrecognized_nesting_depth = 0;
     lexer->lexer_status = CAN_ADVANCE;
     lexer->state = &states[BEGIN_STATE];
-    lexer->is_jsonlines = is_jsonlines;
     lexer->is_key = false;
 }
 
+void reset_lexer_output(struct Lexer* lexer) {
+    clear(&lexer->output);
+    lexer->lexer_status = CAN_ADVANCE;
+    lexer->state = &states[BEGIN_STATE];
+    lexer->is_key = false;
+    lexer->input_position -= 1;
+}
+
 void release_lexer(struct Lexer* lexer) {
     release_char_buffer(&lexer->output);
 }
 
 struct State* begin(struct Lexer* lexer) {
     // Ignoring characters until either '{' or '[' appears
     for(;;) {
@@ -120,36 +131,26 @@
             if(last_char(lexer) == ',') {
                 unemit(lexer);
             }
             pop(&lexer->nesting_depth);
             lexer->is_key = top(&lexer->nesting_depth) == '{';
             emit('}', lexer);
             if(size(&lexer->nesting_depth) <= 0) {
-                if(lexer->is_jsonlines) {
-                    emit_in_place('\0', lexer);
-                    return &states[BEGIN_STATE];
-                } else {
-                    return &states[END_STATE];
-                }
+                return &states[END_STATE];
             }
         break;
         case ']':
             if(last_char(lexer) == ',') {
                 unemit(lexer);
             }
             pop(&lexer->nesting_depth);
             lexer->is_key = top(&lexer->nesting_depth) == '{';
             emit(']', lexer);
             if(size(&lexer->nesting_depth) <= 0) {
-                if(lexer->is_jsonlines) {
-                    emit_in_place('\0', lexer);
-                    return &states[BEGIN_STATE];
-                } else {
-                    return &states[END_STATE];
-                }
+                return &states[END_STATE];
             }
         break;
         case ':':
             lexer->is_key = false;
             emit(':', lexer);
         break;
         case ',':
@@ -216,17 +217,15 @@
         return handle_unrecognized(lexer);
     }
 
     return &states[JSON_STATE];
 }
 
 struct State* end(struct Lexer* lexer) {
-    if(!lexer->is_jsonlines) {
-        emit('\0', lexer);
-    }
+    emit('\0', lexer);
     lexer->lexer_status = FINISHED;
     return lexer->state;
 }
 
 struct State* error(struct Lexer* lexer) {
     emit('\0', lexer);
     lexer->lexer_status = ERROR;
@@ -270,49 +269,64 @@
     }
             
     return &states[ERROR_STATE];
 }
 
 struct State* handle_numeric(struct Lexer* lexer) {
     char c = next_char(lexer);
-    if(c == '-') {
-        emit('-', lexer);
-        c = next_char(lexer);
-    }
-    if(c == '.') {
-        emit_in_place('0', lexer);
-    }
-
-    bool to_be_quoted = false;
-    c = next_char(lexer);
-    if(c == '0') {
-        char next_c = tolower(lexer->input[lexer->input_position+1]);
-        if(next_c == 'x' || next_c == 'b' || next_c == 'o' || isdigit(next_c)) {
-            to_be_quoted = true;
-            emit_in_place('"', lexer);
-            emit('0', lexer);
-            emit(next_c, lexer);
+    if(c >= 49 && c <= 57) { // 1-9 range
+        do {
+            if(c != '_') {
+                emit(c, lexer);
+            } else {
+                lexer->input_position += 1;
+            }
             c = tolower(lexer->input[lexer->input_position]);
+        } while(isdigit(c) || c == '.' || c == 'e' || c == 'E' || c == '+' || c =='-' || c == '_');
+        if(last_char(lexer) == '.') {
+            emit_in_place('0', lexer);
         }
-    }
-
-    do {
-        if(c != '_') {
-            emit(c, lexer);
+    } else if(c == '.') {
+        emit_in_place('0', lexer);
+        emit('.', lexer);
+        return handle_numeric(lexer);
+    } else if(c == '-') {
+        emit('-', lexer);
+        return handle_numeric(lexer);
+    } else if(c == '0') {
+        char nc = tolower(lexer->input[lexer->input_position+1]);
+        if(nc == '.') {
+            emit('0', lexer);
+            emit('.', lexer);
+            return handle_numeric(lexer);
+        } else if(nc == 'x' || nc == 'X') {
+            return handle_numeric_non_standard_base(lexer, 16);
+        } else if(nc == 'o' || nc == 'O') {
+            lexer->input_position += 2;
+            return handle_numeric_non_standard_base(lexer, 8);
+        } else if(isdigit(nc)) {
+            return handle_numeric_non_standard_base(lexer, 8);
+        } else if(nc == 'b' || nc == 'B') {
+            lexer->input_position += 2;
+            return handle_numeric_non_standard_base(lexer, 2);
         } else {
-            lexer->input_position += 1;
+            emit('0', lexer);
+            return &states[JSON_STATE];
         }
-        c = tolower(lexer->input[lexer->input_position]);
-    // [97, 102] is ASCII range for a-f, for hex digits
-    } while(isdigit(c) || c == '.' || c == '_' || (c >= 97 && c <= 102));
-
-    if(to_be_quoted) {
-        emit_in_place('"', lexer);
+    } else {
+        return &states[ERROR_STATE];
     }
+    return &states[JSON_STATE];
+}
 
+struct State* handle_numeric_non_standard_base(struct Lexer* lexer, int base) {
+    char* end;
+    long n = strtol(lexer->input + lexer->input_position, &end, base);
+    emit_number_in_place(n, lexer);
+    lexer->input_position = end - lexer->input;
     return &states[JSON_STATE];
 }
 
 struct State* handle_unrecognized(struct Lexer* lexer) {
     emit_in_place('"', lexer);
     char currently_quoted_with = '\0';
```

### Comparing `chompjs-1.1.9/_chompjs/parser.h` & `chompjs-1.2.0/_chompjs/parser.h`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /*
- * Copyright 2020-2021 Mariusz Obajtek. All rights reserved.
+ * Copyright 2020-2023 Mariusz Obajtek. All rights reserved.
  * License: https://github.com/Nykakin/chompjs/blob/master/LICENSE
  */
 
 #ifndef CHOMPJS_PARSER_H
 #define CHOMPJS_PARSER_H
 
 #include <stddef.h>
@@ -27,18 +27,20 @@
 struct State* end(struct Lexer* lexer);
 struct State* error(struct Lexer* lexer);
 
 /*
     Helper functions used in "value" state
     * handle_quoted - handles quoted strings
     * handle_numeric - handle numbers
+    * handle_numeric_non_standard_base - handle numbers in non-standard bases (hex, oct)
     * handle_unrecognized - save all unrecognized data as a string
 */
 struct State* handle_quoted(struct Lexer* lexer);
 struct State* handle_numeric(struct Lexer* lexer);
+struct State* handle_numeric_non_standard_base(struct Lexer* lexer, int base);
 struct State* handle_unrecognized(struct Lexer* lexer);
 
 /**
     State wrapper
 */
 struct State {
     struct State* (*change)(struct Lexer *);
@@ -58,15 +60,14 @@
     struct CharBuffer output;
     size_t input_position;
     size_t output_position;
     LexerStatus lexer_status;
     struct State* state;
     struct CharBuffer nesting_depth;
     size_t unrecognized_nesting_depth;
-    bool is_jsonlines;
     bool is_key;
 };
 
 /** Switch state of internal state machine */
 void advance(struct Lexer* lexer);
 
 /** Get next char, ignore whitespaces */
@@ -86,17 +87,23 @@
 
 /** Send string to output buffer, advance input position */
 void emit_string(const char *s, size_t size, struct Lexer* lexer);
 
 /** Send string to output buffer, keep old input position */
 void emit_string_in_place(const char *s, size_t size, struct Lexer* lexer);
 
+/** Send number to output buffer, keep old input position */
+void emit_number_in_place(long value, struct Lexer* lexer);
+
 /** Handle comments in JSON body */
 void handle_comments(struct Lexer* lexer);
 
-/** Initialize main lexer object*/
-void init_lexer(struct Lexer* lexer, const char* string, bool is_jsonlines);
+/** Initialize main lexer object */
+void init_lexer(struct Lexer* lexer, const char* string);
+
+/** Reset main lexer object output buffer */
+void reset_lexer_output(struct Lexer* lexer);
 
 /** Release main lexer object and its memory */
 void release_lexer(struct Lexer* lexer);
 
 #endif
```

### Comparing `chompjs-1.1.9/chompjs/test_parser.py` & `chompjs-1.2.0/chompjs/test_parser.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 from __future__ import unicode_literals
 
 import functools
 import math
 import unittest
 
-from chompjs import parse_js_object
+from chompjs import parse_js_object, parse_js_objects
 
 
 def parametrize_test(*arguments_list):
     def decorate(func):
         @functools.wraps(func)
         def wrapper(self, *args, **kwargs):
             for arguments in arguments_list:
@@ -71,15 +71,14 @@
         ("[12, -323, 0.32, -32.22, .2, - 4]", [12, -323, 0.32, -32.22, 0.2, -4]),
         ('{"a": -12, "b": - 5}', {'a': -12, 'b': -5}),
         ("{'a': true, 'b': false, 'c': null}", {'a': True, 'b': False, 'c': None}),
         ("[\"\\uD834\\uDD1E\"]", [u'𝄞']),
         ("{'a': '123\\'456\\n'}", {'a': "123'456\n"}),
         ("['\u00E9']", ['é']),
         ('{"cache":{"\u002Ftest\u002F": 0}}', {'cache': {'/test/': 0}}),
-        ('{"a": 12_12}', {'a': 1212}),
         ('{"a": 3.125e7}', {'a': 3.125e7}),
         ('''{"a": "b\\'"}''', {'a': "b'"}),
         ('{"a": .99, "b": -.1}', {"a": 0.99, "b": -.1}),
         ('["/* ... */", "// ..."]', ["/* ... */", "// ..."]),
         ('{"inclusions":["/*","/"]}', {'inclusions': ['/*', '/']}),
     )
     def test_parse_standard_values(self, in_data, expected_data):
@@ -101,18 +100,18 @@
         (
             "{\"abc\": function() {return '])))))))))))))))';}}",
             {"abc": "function() {return '])))))))))))))))';}"},
         ),
         ('{"a": undefined}', {"a": "undefined"}),
         ('[undefined, undefined]', ["undefined", "undefined"]),
         ("{_a: 1, $b: 2}", {"_a": 1, "$b": 2}),
-        ("[0x12, 0xAB, 051, 0o51, 0b111]", ["0x12", "0xab", "051", "0o51", "0b111"]),
         ("{regex: /a[^d]{1,12}/i}", {'regex': '/a[^d]{1,12}/i'}),
         ("{'a': function(){return '\"'}}", {'a': 'function(){return \'"\'}'}),
         ("{1: 1, 2: 2, 3: 3, 4: 4}", {'1': 1, '2': 2, '3': 3, '4': 4}),
+        ("{'a': 121.}", {'a': 121.0})
     )
     def test_parse_strange_values(self, in_data, expected_data):
         result = parse_js_object(in_data)
         self.assertEqual(result, expected_data)
 
     @parametrize_test(
         ('{"a": {"b": [12, 13, 14]}}text text', {"a": {"b": [12, 13, 14]}}),
@@ -122,14 +121,71 @@
         ("{truefalse: 0, falsefalse: 1, nullnull: 2}", {'truefalse': 0, 'falsefalse': 1, 'nullnull': 2}),
     )
     def test_strange_input(self, in_data, expected_data):
         result = parse_js_object(in_data)
         self.assertEqual(result, expected_data)
 
     @parametrize_test(
+        ("[0]", [0]),
+        ("[1]", [1]),
+        ("[12]", [12]),
+        ("[12_12]", [1212]),
+        ("[0x12]", [18]),
+        ("[0xab]", [171]),
+        ("[0xAB]", [171]),
+        ("[0X12]", [18]),
+        ("[0Xab]", [171]),
+        ("[0XAB]", [171]),
+        ("[01234]", [668]),
+        ("[0o1234]", [668]),
+        ("[0O1234]", [668]),
+        ("[0b1111]", [15]),
+        ("[0B1111]", [15]),
+        ("[-0]", [-0]),
+        ("[-1]", [-1]),
+        ("[-12]", [-12]),
+        ("[-12_12]", [-1212]),
+        ("[-0x12]", [-18]),
+        ("[-0xab]", [-171]),
+        ("[-0xAB]", [-171]),
+        ("[-0X12]", [-18]),
+        ("[-0Xab]", [-171]),
+        ("[-0XAB]", [-171]),
+        ("[-01234]", [-668]),
+        ("[-0o1234]", [-668]),
+        ("[-0O1234]", [-668]),
+        ("[-0b1111]", [-15]),
+        ("[-0B1111]", [-15]),
+    )
+    def test_integer_numeric_values(self, in_data, expected_data):
+        result = parse_js_object(in_data)
+        self.assertEqual(result, expected_data)
+
+    @parametrize_test(
+        ("[0.32]", [0.32]),
+        ("[-0.32]", [-0.32]),
+        ("[.32]", [0.32]),
+        ("[-.32]", [-0.32]),
+        ("[12.]", [12.0]),
+        ("[-12.]", [-12.0]),
+        ("[12.32]", [12.32]),
+        ("[-12.12]", [-12.12]),
+        ("[3.1415926]", [3.1415926]),
+        ("[.123456789]", [.123456789]),
+        ("[3.1E+12]", [3.1E+12]),
+        ("[3.1e+12]", [3.1E+12]),
+        ("[.1e-23]", [.1e-23]),
+        ("[.1e-23]", [.1e-23]),
+    )
+    def test_float_numeric_values(self, in_data, expected_data):
+        result = parse_js_object(in_data)
+        self.assertEqual(result, expected_data)
+
+
+    @parametrize_test(
         (
             """
                 var obj = {
                     // Comment
                     x: "X", // Comment
                 };
             """,
@@ -153,15 +209,15 @@
         result = parse_js_object(in_data)
         self.assertEqual(result, expected_data)
 
     @parametrize_test(
         ('["Test\\nDrive"]\n{"Test": "Drive"}', [['Test\nDrive'], {'Test': 'Drive'}]),
     )
     def test_jsonlines(self, in_data, expected_data):
-        result = parse_js_object(in_data, jsonlines=True)
+        result = list(parse_js_objects(in_data))
         self.assertEqual(result, expected_data)
 
 
 class TestParserExceptions(unittest.TestCase):
     @parametrize_test(
         ('}{', ValueError),
         ('', ValueError),
@@ -212,9 +268,50 @@
         ),
     )
     def test_json_non_strict(self, in_data, expected_data):
         result = parse_js_object(in_data, json_params={'strict': False})
         self.assertEqual(result, expected_data)
 
 
+
+class TestParseJsonObjects(unittest.TestCase):
+    @parametrize_test(
+        ("", []),
+        ("aaaaaaaaaaaaaaaa", []),
+        ("         ", []),
+        ("      {'a': 12}", [{'a': 12}]),
+        ("[1, 2, 3, 4]xxxxxxxxxxxxxxxxxxxxxxxx", [[1, 2, 3, 4]]),
+        ("[12] [13] [14]", [[12], [13], [14]]),
+        ("[10] {'a': [1, 1, 1,]}", [[10], {'a': [1, 1, 1]}]),
+        ("[1][1][1]", [[1], [1], [1]]),
+        ("[1] [2] {'a': ", [[1], [2]]),
+        ("[]", [[]]),
+        ("[][][][]", [[], [], [], []]),
+        ("{}", [{}]),
+        ("{}{}{}{}", [{}, {}, {}, {}]),
+        ("{{}}{{}}", []),
+        ("[[]][[]]", [[[]], [[]]]),
+        ("{am: 'ab'}\n{'ab': 'xx'}", [{'am': 'ab'}, {'ab': 'xx'}]),
+        (
+            'function(a, b, c){ /* ... */ }({"a": 12}, Null, [1, 2, 3])',
+            [{}, {'a': 12}, [1, 2, 3]],
+        ),
+        ('{"a": 12, broken}{"c": 100}', [{'c': 100}]),
+        ('[12,,,,21][211,,,][12,12][12,,,21]', [[12, 12]]),
+    )
+    def test_parse_json_objects(self, in_data, expected_data):
+        result = list(parse_js_objects(in_data))
+        self.assertEqual(result, expected_data)
+
+    @parametrize_test(
+        ("[1][][2]", [[1], [2]]),
+        ("{'a': 12}{}{'b': 13}", [{'a': 12}, {'b': 13}]),
+        ("[][][][][][][][][]", []),
+        ("{}{}{}{}{}{}{}{}{}", []),
+    )
+    def test_parse_json_objects_without_empty(self, in_data, expected_data):
+        result = list(parse_js_objects(in_data, omitempty=True))
+        self.assertEqual(result, expected_data)
+
+
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `chompjs-1.1.9/setup.py` & `chompjs-1.2.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -22,30 +22,33 @@
     sources=['_chompjs/module.c', '_chompjs/parser.c', '_chompjs/buffer.c'],
     extra_compile_args=extra_compile_args,
     extra_link_args=extra_link_args,
 )
 
 setup(
     name='chompjs',
-    version='1.1.9',
+    version='1.2.0',
     description='Parsing JavaScript objects into Python dictionaries',
     author='Mariusz Obajtek',
     author_email='nykakin@gmail.com',
-    keywords='parsing parser JavaScript json',
+    keywords='parsing parser JavaScript json json5 webscrapping',
+    python_requires='>=3',
     ext_modules=[chompjs_extension],
     classifiers=[
-        "Programming Language :: Python :: 2",
         "Programming Language :: Python :: 3",
         "Programming Language :: JavaScript",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Topic :: Text Processing :: General",
         "Topic :: Text Processing :: Linguistic",
+        "Development Status :: 5 - Production/Stable",
+        "Environment :: Console",
+        "Environment :: Web Environment",
     ],
     url='https://github.com/Nykakin/chompjs',
     long_description=long_description,
     long_description_content_type='text/markdown',
     include_package_data=True,
     packages=['chompjs'],
 )
```

