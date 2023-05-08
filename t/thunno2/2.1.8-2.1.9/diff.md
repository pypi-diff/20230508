# Comparing `tmp/thunno2-2.1.8.tar.gz` & `tmp/thunno2-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thunno2-2.1.8.tar", last modified: Mon May  1 12:44:16 2023, max compression
+gzip compressed data, was "thunno2-2.1.9.tar", last modified: Sat May  6 17:05:22 2023, max compression
```

## Comparing `thunno2-2.1.8.tar` & `thunno2-2.1.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-05-01 12:44:16.085301 thunno2-2.1.8/
--rw-r--r--   0 nayak      (501) staff       (20)      959 2023-05-01 12:44:16.085177 thunno2-2.1.8/PKG-INFO
--rw-r--r--   0 nayak      (501) staff       (20)       38 2023-05-01 12:44:16.085340 thunno2-2.1.8/setup.cfg
--rw-r--r--   0 nayak      (501) staff       (20)     1314 2023-04-16 17:25:02.000000 thunno2-2.1.8/setup.py
-drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-05-01 12:44:16.084342 thunno2-2.1.8/thunno2/
--rw-r--r--   0 nayak      (501) staff       (20)       22 2023-05-01 12:43:53.000000 thunno2-2.1.8/thunno2/__init__.py
--rw-r--r--   0 nayak      (501) staff       (20)      760 2023-04-30 09:02:54.000000 thunno2-2.1.8/thunno2/autoexplanation.py
--rw-r--r--   0 nayak      (501) staff       (20)     1393 2023-04-16 17:25:02.000000 thunno2-2.1.8/thunno2/codepage.py
--rw-r--r--   0 nayak      (501) staff       (20)    51654 2023-05-01 10:45:28.000000 thunno2-2.1.8/thunno2/commands.py
--rw-r--r--   0 nayak      (501) staff       (20)     2950 2023-04-16 17:25:02.000000 thunno2-2.1.8/thunno2/constants.py
--rw-r--r--   0 nayak      (501) staff       (20)   245360 2023-04-16 17:25:02.000000 thunno2-2.1.8/thunno2/dictionary.py
--rw-r--r--   0 nayak      (501) staff       (20)     7174 2023-04-27 10:00:16.000000 thunno2-2.1.8/thunno2/flags.py
--rw-r--r--   0 nayak      (501) staff       (20)    51729 2023-05-01 10:45:28.000000 thunno2-2.1.8/thunno2/helpers.py
--rw-r--r--   0 nayak      (501) staff       (20)    27697 2023-05-01 08:58:11.000000 thunno2-2.1.8/thunno2/interpreter.py
--rw-r--r--   0 nayak      (501) staff       (20)    23408 2023-04-27 13:07:04.000000 thunno2-2.1.8/thunno2/lexer.py
--rw-r--r--   0 nayak      (501) staff       (20)     1998 2023-05-01 08:52:47.000000 thunno2-2.1.8/thunno2/run.py
--rw-r--r--   0 nayak      (501) staff       (20)    72542 2023-04-30 14:45:33.000000 thunno2-2.1.8/thunno2/tests.py
--rw-r--r--   0 nayak      (501) staff       (20)     4019 2023-04-29 16:25:56.000000 thunno2-2.1.8/thunno2/tokens.py
--rw-r--r--   0 nayak      (501) staff       (20)       97 2023-05-01 12:43:42.000000 thunno2-2.1.8/thunno2/version.py
-drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-05-01 12:44:16.085009 thunno2-2.1.8/thunno2.egg-info/
--rw-r--r--   0 nayak      (501) staff       (20)      959 2023-05-01 12:44:16.000000 thunno2-2.1.8/thunno2.egg-info/PKG-INFO
--rw-r--r--   0 nayak      (501) staff       (20)      441 2023-05-01 12:44:16.000000 thunno2-2.1.8/thunno2.egg-info/SOURCES.txt
--rw-r--r--   0 nayak      (501) staff       (20)        1 2023-05-01 12:44:16.000000 thunno2-2.1.8/thunno2.egg-info/dependency_links.txt
--rw-r--r--   0 nayak      (501) staff       (20)       54 2023-05-01 12:44:16.000000 thunno2-2.1.8/thunno2.egg-info/entry_points.txt
--rw-r--r--   0 nayak      (501) staff       (20)        8 2023-05-01 12:44:16.000000 thunno2-2.1.8/thunno2.egg-info/top_level.txt
+drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-05-06 17:05:22.361474 thunno2-2.1.9/
+-rw-r--r--   0 nayak      (501) staff       (20)      959 2023-05-06 17:05:22.361361 thunno2-2.1.9/PKG-INFO
+-rw-r--r--   0 nayak      (501) staff       (20)       38 2023-05-06 17:05:22.361512 thunno2-2.1.9/setup.cfg
+-rw-r--r--   0 nayak      (501) staff       (20)     1314 2023-04-16 17:25:02.000000 thunno2-2.1.9/setup.py
+drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-05-06 17:05:22.360674 thunno2-2.1.9/thunno2/
+-rw-r--r--   0 nayak      (501) staff       (20)       22 2023-05-01 12:43:53.000000 thunno2-2.1.9/thunno2/__init__.py
+-rw-r--r--   0 nayak      (501) staff       (20)      760 2023-04-30 09:02:54.000000 thunno2-2.1.9/thunno2/autoexplanation.py
+-rw-r--r--   0 nayak      (501) staff       (20)     1393 2023-04-16 17:25:02.000000 thunno2-2.1.9/thunno2/codepage.py
+-rw-r--r--   0 nayak      (501) staff       (20)    52857 2023-05-04 17:16:06.000000 thunno2-2.1.9/thunno2/commands.py
+-rw-r--r--   0 nayak      (501) staff       (20)     2950 2023-04-16 17:25:02.000000 thunno2-2.1.9/thunno2/constants.py
+-rw-r--r--   0 nayak      (501) staff       (20)   245360 2023-04-16 17:25:02.000000 thunno2-2.1.9/thunno2/dictionary.py
+-rw-r--r--   0 nayak      (501) staff       (20)     7174 2023-04-27 10:00:16.000000 thunno2-2.1.9/thunno2/flags.py
+-rw-r--r--   0 nayak      (501) staff       (20)    52884 2023-05-04 17:18:41.000000 thunno2-2.1.9/thunno2/helpers.py
+-rw-r--r--   0 nayak      (501) staff       (20)    30385 2023-05-06 17:04:50.000000 thunno2-2.1.9/thunno2/interpreter.py
+-rw-r--r--   0 nayak      (501) staff       (20)    24717 2023-05-06 17:04:50.000000 thunno2-2.1.9/thunno2/lexer.py
+-rw-r--r--   0 nayak      (501) staff       (20)     1998 2023-05-01 08:52:47.000000 thunno2-2.1.9/thunno2/run.py
+-rw-r--r--   0 nayak      (501) staff       (20)    76149 2023-05-04 17:17:09.000000 thunno2-2.1.9/thunno2/tests.py
+-rw-r--r--   0 nayak      (501) staff       (20)     4019 2023-04-29 16:25:56.000000 thunno2-2.1.9/thunno2/tokens.py
+-rw-r--r--   0 nayak      (501) staff       (20)       97 2023-05-06 17:04:40.000000 thunno2-2.1.9/thunno2/version.py
+drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-05-06 17:05:22.361210 thunno2-2.1.9/thunno2.egg-info/
+-rw-r--r--   0 nayak      (501) staff       (20)      959 2023-05-06 17:05:22.000000 thunno2-2.1.9/thunno2.egg-info/PKG-INFO
+-rw-r--r--   0 nayak      (501) staff       (20)      441 2023-05-06 17:05:22.000000 thunno2-2.1.9/thunno2.egg-info/SOURCES.txt
+-rw-r--r--   0 nayak      (501) staff       (20)        1 2023-05-06 17:05:22.000000 thunno2-2.1.9/thunno2.egg-info/dependency_links.txt
+-rw-r--r--   0 nayak      (501) staff       (20)       54 2023-05-06 17:05:22.000000 thunno2-2.1.9/thunno2.egg-info/entry_points.txt
+-rw-r--r--   0 nayak      (501) staff       (20)        8 2023-05-06 17:05:22.000000 thunno2-2.1.9/thunno2.egg-info/top_level.txt
```

### Comparing `thunno2-2.1.8/PKG-INFO` & `thunno2-2.1.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: thunno2
-Version: 2.1.8
+Version: 2.1.9
 Summary: A golfing language
 Home-page: https://github.com/Thunno/Thunno2
 Author: Rujul Nayak
 Author-email: rujulnayak@outlook.com
 License: MIT
-Download-URL: https://github.com/Thunno/Thunno2/archive/refs/tags/v2.1.8.tar.gz
+Download-URL: https://github.com/Thunno/Thunno2/archive/refs/tags/v2.1.9.tar.gz
 Keywords: golfing,code-golf,language
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `thunno2-2.1.8/setup.py` & `thunno2-2.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.1.8/thunno2/autoexplanation.py` & `thunno2-2.1.9/thunno2/autoexplanation.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.1.8/thunno2/codepage.py` & `thunno2-2.1.9/thunno2/codepage.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.1.8/thunno2/commands.py` & `thunno2-2.1.9/thunno2/commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -1122,17 +1122,20 @@
             ((int, float, str), (int, float, str), list): list_transliterate_overload_3,
         },
         0,
         ("transliterate",),
     ),
     "Ọ": Overload(
         2,
-        {(Any[0], Any[0]): logical_or},
-        0,
-        ("non_vectorised_or", "non_vectorised_logical_or"),
+        {
+            (Number[0], Number[0]): dyadic_minimum,
+            (Any[0], Any[0]): string_dyadic_minimum,
+        },
+        2,
+        ("dyadic_minimum",),
     ),
     "Ṛ": Overload(
         2,
         {
             (Number[0], Iterable[0]): combinations_with_replacement1,
             (Iterable[0], Number[0]): combinations_with_replacement2,
             (Number[0], Number[0]): combinations_with_replacement3,
@@ -1203,17 +1206,20 @@
     ),
     "¶": Overload(0, {Any: (lambda: "\n")}, 0, ("newline",)),
     "¬": Overload(
         1, {Any: logical_not}, 0, ("non_vectorised_not", "non_vectorised_logical_not")
     ),
     "§": Overload(
         2,
-        {(Any[0], Any[0]): logical_and},
-        0,
-        ("non_vectorised_and", "non_vectorised_logical_and"),
+        {
+            (Number[0], Number[0]): dyadic_maximum,
+            (Any[0], Any[0]): string_dyadic_maximum,
+        },
+        2,
+        ("dyadic_maximum",),
     ),
     "½": Overload(1, {Number: halve, str: chunk_halve}, 1, ("halve",)),
     "Ƈ": Overload(
         2,
         {
             (Number[0], Number[0]): nPr,
             (Any, str): string_contains,
@@ -1458,14 +1464,17 @@
     ),
 }
 
 list_digraphs = {
     "C": Overload(
         1, {((int, float, str),): pass_, list: centre_list}, 0, ("center", "centre")
     ),
+    "D": Overload(1, {Any: depth}, 0, ("depth",)),
+    "G": Overload(1, {((int, float, str),): pass_, list: longest}, 0, ("longest",)),
+    "M": Overload(1, {((int, float, str),): pass_, list: shortest}, 0, ("shortest",)),
     ".": Overload(
         2, {(list, list): dot_product, (Any[0], Any[0]): pass_}, 0, ("dot_product",)
     ),
     "\\": Overload(
         1, {((int, float, str),): pass_, list: main_diagonal}, 0, ("main_diagonal",)
     ),
     "/": Overload(
@@ -1483,33 +1492,57 @@
 }
 
 random_digraphs_1 = {
     "C": Overload(1, {Any: cosine}, 1, ("cosine", "cos")),
     "D": Overload(1, {Any: degrees}, 1, ("degrees",)),
     "E": Overload(1, {Any: exponent}, 1, ("exponent",)),
     "F": Overload(1, {Any: nth_fibonacci_number}, 1, ("nth_fibonacci_number",)),
+    "H": Overload(2, {(Any[0], Any[0]): hypotenuse}, 2, ("hypot", "hypotenuse")),
     "P": Overload(1, {Any: nth_prime}, 1, ("nth_prime",)),
     "R": Overload(1, {Any: radians}, 1, ("radians",)),
     "S": Overload(1, {Any: sine}, 1, ("sine", "sin")),
     "T": Overload(1, {Any: tangent}, 1, ("tangent", "tan")),
     "c": Overload(1, {Any: arc_cosine}, 1, ("arc_cosine", "arccos")),
     "s": Overload(1, {Any: arc_sine}, 1, ("arc_sine", "arcsin")),
     "t": Overload(1, {Any: arc_tangent}, 1, ("arc_tangent", "arctan")),
+    "&": Overload(2, {(Any[0], Any[0]): bitwise_and}, 2, ("bitwise_and",)),
+    "|": Overload(2, {(Any[0], Any[0]): bitwise_or}, 2, ("bitwise_or",)),
+    "^": Overload(2, {(Any[0], Any[0]): bitwise_xor}, 2, ("bitwise_xor",)),
+    "~": Overload(1, {Any: bitwise_not}, 1, ("bitwise_not",)),
 }
 
 random_digraphs_2 = {
     "R": Overload(
         1, {Number: to_roman_numerals, str: from_roman_numerals}, 1, ("roman_numerals",)
     ),
+    "T": Overload(1, {Any: type_of}, 0, ("type",)),
     "r": Overload(
         1,
         {Number: range_shuffle, str: str_shuffle, list: shuffle},
         0,
         ("random_shuffle",),
     ),
+    "&": Overload(
+        2,
+        {(Any[0], Any[0]): logical_and},
+        0,
+        ("non_vectorised_and", "non_vectorised_logical_and"),
+    ),
+    "|": Overload(
+        2,
+        {(Any[0], Any[0]): logical_or},
+        0,
+        ("non_vectorised_or", "non_vectorised_logical_or"),
+    ),
+    "^": Overload(
+        2,
+        {(Any[0], Any[0]): logical_xor},
+        0,
+        ("non_vectorised_xor", "non_vectorised_logical_xor"),
+    ),
 }
 
 
 def get_a_function(command):
     if not command:
         return Void
     if len(command) == 1:
```

### Comparing `thunno2-2.1.8/thunno2/constants.py` & `thunno2-2.1.9/thunno2/constants.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.1.8/thunno2/dictionary.py` & `thunno2-2.1.9/thunno2/dictionary.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.1.8/thunno2/flags.py` & `thunno2-2.1.9/thunno2/flags.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.1.8/thunno2/helpers.py` & `thunno2-2.1.9/thunno2/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,25 +141,25 @@
 
 
 def try_int_conversion(func):
     def wrapper(*args, fn=func):
         try:
             return fn(*map(int, args))
         except:
-            return args
+            return [*args]
 
     return wrapper
 
 
 def try_float_conversion(func):
     def wrapper(*args, fn=func):
         try:
             return fn(*map(float, args))
         except:
-            return args
+            return [*args]
 
     return wrapper
 
 
 def safe_max_len(*lsts):
     m = 0
     for lst in lsts:
@@ -2772,7 +2772,80 @@
     if not l:
         return []
     r = [[] for _ in range(len(l) + min(map(len, l)) - 1)]
     for i, x in enumerate(l):
         for j in range(min(map(len, l))):
             r[((-i) - j + min(len(l), min(map(len, l))) - 1) % len(r)].append(x[j])
     return r
+
+
+def longest(l):
+    if not l:
+        return []
+    return max(l, key=lambda x: len(_digits(x)))
+
+
+def shortest(l):
+    if not l:
+        return []
+    return min(l, key=lambda x: len(_digits(x)))
+
+
+def dyadic_maximum(x, y):
+    return max(y, x)
+
+
+def dyadic_minimum(x, y):
+    return min(y, x)
+
+
+def string_dyadic_maximum(x, y):
+    return x if str(x) > str(y) else y
+
+
+def string_dyadic_minimum(x, y):
+    return x if str(x) < str(y) else y
+
+
+@try_int_conversion
+def bitwise_and(x, y):
+    return y & x
+
+
+@try_int_conversion
+def bitwise_or(x, y):
+    return y | x
+
+
+@try_int_conversion
+def bitwise_xor(x, y):
+    return y ^ x
+
+
+@try_int_conversion
+def bitwise_not(x):
+    return ~x
+
+
+def depth(lst, curr=0):
+    if isinstance(lst, list):
+        if not lst:
+            return curr + 1
+        return max(depth(i, curr + 1) for i in lst)
+    return curr
+
+
+def type_of(x):
+    if isinstance(x, int):
+        return 0
+    if isinstance(x, float):
+        return 1
+    if isinstance(x, str):
+        return 2
+    if isinstance(x, list):
+        return 3
+    return -1
+
+
+@try_float_conversion
+def hypotenuse(a, b):
+    return math.sqrt(a**2 + b**2)
```

### Comparing `thunno2-2.1.8/thunno2/interpreter.py` & `thunno2-2.1.9/thunno2/interpreter.py`

 * *Files 5% similar despite different names*

```diff
@@ -563,14 +563,80 @@
                     ctx.stack.push(r[-1])
                     ctx.stack.push(j)
                     run(info, n=j, iteration_index=i)
                     r.append(next(ctx.stack.rmv(1)))
                 ctx.stack.push(r)
             else:
                 ctx.stack.push([])
+        elif desc == "single function reduce by":
+            a = next(ctx.stack.rmv(1))
+            x = listify(a)
+            old_stack = Stack(copy.deepcopy(list(ctx.stack).copy()))
+            func = info
+            if func != Void:
+                if x:
+                    r = [x.pop(0)]
+                    for i, j in enumerate(x):
+                        ctx.stack = Stack(copy.deepcopy(old_stack))
+                        ctx.stack.push(r[-1])
+                        ctx.stack.push(j)
+                        for k in func():
+                            r.append(k)
+                    ctx.stack.push(r[-1])
+                else:
+                    ctx.stack.push([])
+        elif desc == "single function right reduce by":
+            a = next(ctx.stack.rmv(1))
+            x = listify(a)[::-1]
+            old_stack = Stack(copy.deepcopy(list(ctx.stack).copy()))
+            func = info
+            if func != Void:
+                if x:
+                    r = [x.pop(0)]
+                    for i, j in enumerate(x):
+                        ctx.stack = Stack(copy.deepcopy(old_stack))
+                        ctx.stack.push(r[-1])
+                        ctx.stack.push(j)
+                        for k in func():
+                            r.append(k)
+                    ctx.stack.push(r[-1])
+                else:
+                    ctx.stack.push([])
+        elif desc == "single function right cumulative reduce by":
+            a = next(ctx.stack.rmv(1))
+            x = listify(a)[::-1]
+            old_stack = Stack(copy.deepcopy(list(ctx.stack).copy()))
+            func = info
+            if func != Void:
+                if x:
+                    r = [x.pop(0)]
+                    for i, j in enumerate(x):
+                        ctx.stack = Stack(copy.deepcopy(old_stack))
+                        ctx.stack.push(r[-1])
+                        ctx.stack.push(j)
+                        for k in func():
+                            r.append(k)
+                    ctx.stack.push(r)
+                else:
+                    ctx.stack.push([])
+        elif desc == "right reduce by":
+            a = next(ctx.stack.rmv(1))
+            x = listify(a)[::-1]
+            old_stack = Stack(copy.deepcopy(list(ctx.stack).copy()))
+            if x:
+                r = [x.pop(0)]
+                for i, j in enumerate(x):
+                    ctx.stack = Stack(copy.deepcopy(old_stack))
+                    ctx.stack.push(r[-1])
+                    ctx.stack.push(j)
+                    run(info, n=j, iteration_index=i)
+                    r.append(next(ctx.stack.rmv(1)))
+                ctx.stack.push(r[-1])
+            else:
+                ctx.stack.push([])
         elif desc == "for loop":
             a = next(ctx.stack.rmv(1))
             x = listify(a)
             for i, j in enumerate(x):
                 if not isinstance(a, (int, float)):
                     ctx.stack.push(j)
                 run(info, n=j, iteration_index=i)
```

### Comparing `thunno2-2.1.8/thunno2/lexer.py` & `thunno2-2.1.9/thunno2/lexer.py`

 * *Files 8% similar despite different names*

```diff
@@ -143,14 +143,44 @@
                 y = char + x
                 if y == "µµ":
                     i, r = tokenise(code[index + 1 :], expected_end=";")
                     index += i
                     ret.append((y, "recursive environment", r))
                 elif y == "µ£":
                     ret.append((y, "print each", 0))
+                elif y == "µƲ":
+                    index += 1
+                    cmd = code[index]
+                    if cmd in DIGRAPHS:
+                        index += 1
+                        cmd += code[index]
+                    func = get_a_function(cmd)
+                    ret.append((char + cmd, "single function reduce by", func))
+                elif y == "µɼ":
+                    index += 1
+                    cmd = code[index]
+                    if cmd in DIGRAPHS:
+                        index += 1
+                        cmd += code[index]
+                    func = get_a_function(cmd)
+                    ret.append((char + cmd, "single function right reduce by", func))
+                elif y == "µƇ":
+                    index += 1
+                    cmd = code[index]
+                    if cmd in DIGRAPHS:
+                        index += 1
+                        cmd += code[index]
+                    func = get_a_function(cmd)
+                    ret.append(
+                        (char + cmd, "single function right cumulative reduce by", func)
+                    )
+                elif y == "µʋ":
+                    i, r = tokenise(code[index + 1 :], expected_end=";")
+                    index += i
+                    ret.append((y, "right reduce by", r))
                 else:
                     ret.append((y, "digraph", get_a_function(y)))
             except:
                 pass
         elif char in "0123456789.":
             s = char
             index += 1
```

### Comparing `thunno2-2.1.8/thunno2/run.py` & `thunno2-2.1.9/thunno2/run.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.1.8/thunno2/tests.py` & `thunno2-2.1.9/thunno2/tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -1539,22 +1539,27 @@
     call("Ṇ", "abc", 123, ["1", "9", "4", "7", "8", "5", "6", "2", "3"]),
     ["a", "9", "4", "7", "8", "5", "6", "b", "c"],
 )
 assert_eq(call("Ṇ", 456, [1, "y", 3], "123xyz"), "426x5z")
 
 # Ọ
 
-assert_eq(call("Ọ", 123, 456), 456)
-assert_eq(call("Ọ", 123, 0), 123)
+assert_eq(call("Ọ", 123, 456), 123)
+assert_eq(call("Ọ", -1.23, -4.56), -4.56)
 
-assert_eq(call("Ọ", -123, "abc"), "abc")
-assert_eq(call("Ọ", "xyz", 0), "xyz")
+assert_eq(call("Ọ", "abcd", "efgh"), "abcd")
+assert_eq(call("Ọ", "abc", "aac"), "aac")
 
-assert_eq(call("Ọ", [-1, 0, 1], ["abc", "def", ""]), ["abc", "def", ""])
-assert_eq(call("Ọ", 5, []), 5)
+assert_eq(call("Ọ", "abc", 123), 123)
+assert_eq(call("Ọ", 123, ""), "")
+
+assert_eq(
+    call("Ọ", [1, 2, 3, 4, 5, 6, 7, 8, 9, 10], [10, 9, 8, 7, 6, 5, 4, 3, 2, 1]),
+    [1, 2, 3, 4, 5, 5, 4, 3, 2, 1],
+)
 
 # Ṛ
 
 assert_eq(call("Ṛ", 3, 2), [[1, 1], [1, 2], [2, 2]])
 
 assert_eq(
     call("Ṛ", "xyz", 2),
@@ -2153,22 +2158,27 @@
 assert_eq(call("¬", ""), 1)
 
 assert_eq(call("¬", [-1, 0, 1, 2, "", "a"]), 0)
 assert_eq(call("¬", []), 1)
 
 # §
 
-assert_eq(call("§", 123, 456), 123)
-assert_eq(call("§", 123, 0), 0)
+assert_eq(call("§", 123, 456), 456)
+assert_eq(call("§", -1.23, -4.56), -1.23)
+
+assert_eq(call("§", "abcd", "efgh"), "efgh")
+assert_eq(call("§", "abc", "aac"), "abc")
 
-assert_eq(call("§", -123, "abc"), -123)
-assert_eq(call("§", "xyz", 0), 0)
+assert_eq(call("§", "abc", 123), "abc")
+assert_eq(call("§", 123, ""), 123)
 
-assert_eq(call("§", [-1, 0, 1], ["abc", "def", ""]), [-1, 0, 1])
-assert_eq(call("§", 5, []), [])
+assert_eq(
+    call("§", [1, 2, 3, 4, 5, 6, 7, 8, 9, 10], [10, 9, 8, 7, 6, 5, 4, 3, 2, 1]),
+    [10, 9, 8, 7, 6, 6, 7, 8, 9, 10],
+)
 
 # Ä
 
 assert_eq(call("Ä", 10), "J")
 assert_eq(call("Ä", [20, 8, 21, 14, 14, 15]), ["T", "H", "U", "N", "N", "O"])
 
 assert_eq(call("Ä", "Abc"), [1, 2, 3])
@@ -2721,14 +2731,45 @@
 
 assert_eq(call("ØC", [123, 4567, 8, 90]), "123 \n4567\n 8  \n 90 ")
 assert_eq(
     call("ØC", ["abc", 1234, "xy", 56789, "z"]), " abc \n 1234\n  xy \n56789\n  z  "
 )
 assert_eq(call("ØC", []), "")
 
+# ØD
+
+assert_eq(call("ØD", 123), 0)
+assert_eq(call("ØD", -4.56), 0)
+assert_eq(call("ØD", "abc"), 0)
+
+assert_eq(call("ØD", [1, 2, 3]), 1)
+assert_eq(call("ØD", [["abc", "def", "ghi"], 123, 456, 789]), 2)
+assert_eq(call("ØD", [1, [2, [3, [4, [5, [6, [7, [8, [9, [10]]]]]]]]]]), 10)
+
+assert_eq(call("ØD", []), 1)
+assert_eq(call("ØD", [[[[[[[[[[]]]]]]]]]]), 10)
+
+# ØG
+
+assert_eq(call("ØG", [123, 4567, 89]), 4567)
+assert_eq(call("ØG", ["abcd", "ef", "ghi"]), "abcd")
+assert_eq(call("ØG", []), [])
+
+assert_eq(call("ØG", 123), 123)
+assert_eq(call("ØG", "abc"), "abc")
+
+# ØM
+
+assert_eq(call("ØM", [123, 4567, 89]), 89)
+assert_eq(call("ØM", ["abcd", "ef", "ghi"]), "ef")
+assert_eq(call("ØM", []), [])
+
+assert_eq(call("ØM", 123), 123)
+assert_eq(call("ØM", "abc"), "abc")
+
 # Ø.
 
 assert_eq(call("Ø.", [1, 2, 3], [4, 5, 6]), 32)
 assert_eq(call("Ø.", [123], [456, 789]), 56088)
 assert_eq(call("Ø.", [], [123, 456, 789]), 0)
 
 assert_eq(
@@ -2806,14 +2847,22 @@
 # ÆF
 
 assert_eq(call("ÆF", 0), 0)
 assert_eq(call("ÆF", 5), 5)
 assert_eq(call("ÆF", 1.23), 1)
 assert_eq(call("ÆF", [10, 11, 12, 13, 14]), [55, 89, 144, 233, 377])
 
+# ÆH
+
+assert_eq(call("ÆH", 3, 4), 5.0)
+assert_eq(call("ÆH", 12, 5), 13.0)
+assert_eq(call("ÆH", 7, 24), 25.0)
+
+assert_eq(call("ÆH", 123, "abc"), [123, "abc"])
+
 # ÆP
 
 assert_eq(call("ÆP", 0), 2)
 assert_eq(call("ÆP", 5), 13)
 assert_eq(call("ÆP", 1.23), 3)
 assert_eq(call("ÆP", [10, 11, 12, 13, 14]), [31, 37, 41, 43, 47])
 
@@ -2851,27 +2900,126 @@
 # # Æt
 #
 # assert_eq(call("Æt", 0), 0.0)  # ~ 0
 # assert_eq(call("Æt", 0.577), 0.5233360338618205)  # ~ pi/6
 # assert_eq(call("Æt", 1), 0.7853981633974483)  # ~ pi/4
 # assert_eq(call("Æt", 1.732), 1.0471848490249274)  # ~ pi/3
 
+# Æ&
+
+assert_eq(call("Æ&", 123, 456), 72)
+assert_eq(call("Æ&", -12.34, 56.78), 48)
+
+assert_eq(
+    call("Æ&", 100, [0, 10, 20, 30, 40, 50, 60, 70, 80, 90, 100]),
+    [0, 0, 4, 4, 32, 32, 36, 68, 64, 64, 100],
+)
+assert_eq(call("Æ&", [12, 34, 56, 78, 90], [2, 4, 6, 8, 10]), [0, 0, 0, 8, 10])
+
+assert_eq(call("Æ&", "abc", 123), ["abc", 123])
+
+# Æ|
+
+assert_eq(call("Æ|", 123, 456), 507)
+assert_eq(call("Æ|", -12.34, 56.78), -4)
+
+assert_eq(
+    call("Æ|", 100, [0, 10, 20, 30, 40, 50, 60, 70, 80, 90, 100]),
+    [100, 110, 116, 126, 108, 118, 124, 102, 116, 126, 100],
+)
+assert_eq(call("Æ|", [12, 34, 56, 78, 90], [2, 4, 6, 8, 10]), [14, 38, 62, 78, 90])
+
+assert_eq(call("Æ|", "abc", 123), ["abc", 123])
+
+# Æ^
+
+assert_eq(call("Æ^", 123, 456), 435)
+assert_eq(call("Æ^", -12.34, 56.78), -52)
+
+assert_eq(
+    call("Æ^", 100, [0, 10, 20, 30, 40, 50, 60, 70, 80, 90, 100]),
+    [100, 110, 112, 122, 76, 86, 88, 34, 52, 62, 0],
+)
+assert_eq(call("Æ^", [12, 34, 56, 78, 90], [2, 4, 6, 8, 10]), [14, 38, 62, 70, 80])
+
+assert_eq(call("Æ^", "abc", 123), ["abc", 123])
+
+# Æ~
+
+assert_eq(call("Æ~", 123), -124)
+assert_eq(call("Æ~", 12.34), -13)
+assert_eq(call("Æ~", -1.23), 0)
+
+assert_eq(
+    call("Æ~", [11, 12, 13, 14, 15, 16, 17, 18, 19, 20]),
+    [-12, -13, -14, -15, -16, -17, -18, -19, -20, -21],
+)
+
+assert_eq(call("Æ~", "abc"), ["abc"])
+
 # µR
 
 assert_eq(call("µR", 12), "XII")
 assert_eq(call("µR", -4.56), "-IV")
 assert_eq(
     call("µR", [123, 456, 789, 1234, 5678, 9012]),
     ["CXXIII", "CDLVI", "DCCLXXXIX", "MCCXXXIV", "MMMMMDCLXXVIII", "MMMMMMMMMXII"],
 )
 
 assert_eq(call("µR", "CMXCIX"), 999)
 assert_eq(call("µR", ""), 0)
 assert_eq(call("µR", "abcdef"), 0)
 
+# µT
+
+assert_eq(call("µT", 123), 0)
+assert_eq(call("µT", -456), 0)
+
+assert_eq(call("µT", 1.23), 1)
+assert_eq(call("µT", -4.56), 1)
+
+assert_eq(call("µT", "abc"), 2)
+assert_eq(call("µT", ""), 2)
+
+assert_eq(call("µT", [123, 456, 789]), 3)
+assert_eq(call("µT", []), 3)
+
+# µ&
+
+assert_eq(call("µ&", 123, 456), 123)
+assert_eq(call("µ&", 123, 0), 0)
+
+assert_eq(call("µ&", -123, "abc"), -123)
+assert_eq(call("µ&", "xyz", 0), 0)
+
+assert_eq(call("µ&", [-1, 0, 1], ["abc", "def", ""]), [-1, 0, 1])
+assert_eq(call("µ&", 5, []), [])
+
+# µ|
+
+assert_eq(call("µ|", 123, 456), 456)
+assert_eq(call("µ|", 123, 0), 123)
+
+assert_eq(call("µ|", -123, "abc"), "abc")
+assert_eq(call("µ|", "xyz", 0), "xyz")
+
+assert_eq(call("µ|", [-1, 0, 1], ["abc", "def", ""]), ["abc", "def", ""])
+assert_eq(call("µ|", 5, []), 5)
+
+# µ^
+
+assert_eq(call("µ^", 123, 456), 0)
+assert_eq(call("µ^", 123, 0), 1)
+
+assert_eq(call("µ^", -123, "abc"), 0)
+assert_eq(call("µ^", "xyz", 0), 1)
+
+assert_eq(call("µ^", [-1, 0, 1], ["abc", "def", ""]), 0)
+assert_eq(call("µ^", 5, []), 1)
+
 # After all the tests
 
 all_commands = (
     [*commands]
     + ["ø" + cmd1 for cmd1 in string_digraphs]
     + ["Ø" + cmd2 for cmd2 in list_digraphs]
     + ["Æ" + cmd3 for cmd3 in random_digraphs_1]
```

### Comparing `thunno2-2.1.8/thunno2/tokens.py` & `thunno2-2.1.9/thunno2/tokens.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.1.8/thunno2.egg-info/PKG-INFO` & `thunno2-2.1.9/thunno2.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: thunno2
-Version: 2.1.8
+Version: 2.1.9
 Summary: A golfing language
 Home-page: https://github.com/Thunno/Thunno2
 Author: Rujul Nayak
 Author-email: rujulnayak@outlook.com
 License: MIT
-Download-URL: https://github.com/Thunno/Thunno2/archive/refs/tags/v2.1.8.tar.gz
+Download-URL: https://github.com/Thunno/Thunno2/archive/refs/tags/v2.1.9.tar.gz
 Keywords: golfing,code-golf,language
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

