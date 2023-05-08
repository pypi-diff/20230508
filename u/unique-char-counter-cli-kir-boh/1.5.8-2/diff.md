# Comparing `tmp/unique_char_counter_cli_kir_boh-1.5.8.tar.gz` & `tmp/unique_char_counter_cli_kir_boh-2.tar.gz`

## Comparing `unique_char_counter_cli_kir_boh-1.5.8.tar` & `unique_char_counter_cli_kir_boh-2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0    53248 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.8/.coverage
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.8/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.8/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.8/.pytest_cache/README.md
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.8/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.8/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.8/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.8/src/unique_char_counter_cli_kir_boh/__init__.py
--rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.8/src/unique_char_counter_cli_kir_boh/unique_char_counter_cli.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.8/src/unique_char_counter_cli_kir_boh/tests/__init__.py
--rw-r--r--   0        0        0     1963 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.8/src/unique_char_counter_cli_kir_boh/tests/test_unique_char_counter_cli.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.8/src/unique_char_counter_cli_kir_boh/tests/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.8/src/unique_char_counter_cli_kir_boh/tests/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.8/src/unique_char_counter_cli_kir_boh/tests/.pytest_cache/README.md
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.8/src/unique_char_counter_cli_kir_boh/tests/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.8/src/unique_char_counter_cli_kir_boh/tests/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.8/src/unique_char_counter_cli_kir_boh/tests/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.8/.gitignore
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.8/LICENSE
--rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.8/README.md
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.8/pyproject.toml
--rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.8/PKG-INFO
+-rw-r--r--   0        0        0    53248 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-2/.coverage
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-2/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-2/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-2/.pytest_cache/README.md
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-2/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-2/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-2/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-2/src/unique_char_counter_cli_kir_boh/__init__.py
+-rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-2/src/unique_char_counter_cli_kir_boh/unique_char_counter_cli.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-2/src/unique_char_counter_cli_kir_boh/tests/__init__.py
+-rw-r--r--   0        0        0     1963 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-2/src/unique_char_counter_cli_kir_boh/tests/test_unique_char_counter_cli.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-2/src/unique_char_counter_cli_kir_boh/tests/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-2/src/unique_char_counter_cli_kir_boh/tests/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-2/src/unique_char_counter_cli_kir_boh/tests/.pytest_cache/README.md
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-2/src/unique_char_counter_cli_kir_boh/tests/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-2/src/unique_char_counter_cli_kir_boh/tests/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-2/src/unique_char_counter_cli_kir_boh/tests/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-2/.gitignore
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-2/LICENSE
+-rw-r--r--   0        0        0     2869 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-2/README.md
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-2/pyproject.toml
+-rw-r--r--   0        0        0     3364 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-2/PKG-INFO
```

### Comparing `unique_char_counter_cli_kir_boh-1.5.8/.coverage` & `unique_char_counter_cli_kir_boh-2/.coverage`

 * *Files identical despite different names*

### Comparing `unique_char_counter_cli_kir_boh-1.5.8/.pytest_cache/v/cache/nodeids` & `unique_char_counter_cli_kir_boh-2/.pytest_cache/v/cache/nodeids`

 * *Files identical despite different names*

### Comparing `unique_char_counter_cli_kir_boh-1.5.8/src/unique_char_counter_cli_kir_boh/unique_char_counter_cli.py` & `unique_char_counter_cli_kir_boh-2/src/unique_char_counter_cli_kir_boh/unique_char_counter_cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,15 +22,16 @@
     group.add_argument("-s", "--string", action="store_true", help="Your string")
     group.add_argument("-f", "--file", action="store_true", help="Your file")
     parser.add_argument("hashable_obj", help="The string you wish to count")
     args = parser.parse_args()
     return args
 
 
-def read_file_in_chunks(file_path, chunk_size=1000):
+def read_file_in_chunks(file_path):
+    chunk_size = 1000
     data = ""
     with open(file_path, "r") as f:
         while True:
             chunk = f.read(chunk_size)
             if not chunk:
                 break
             data += chunk
```

### Comparing `unique_char_counter_cli_kir_boh-1.5.8/src/unique_char_counter_cli_kir_boh/tests/test_unique_char_counter_cli.py` & `unique_char_counter_cli_kir_boh-2/src/unique_char_counter_cli_kir_boh/tests/test_unique_char_counter_cli.py`

 * *Files identical despite different names*

### Comparing `unique_char_counter_cli_kir_boh-1.5.8/src/unique_char_counter_cli_kir_boh/tests/.pytest_cache/v/cache/nodeids` & `unique_char_counter_cli_kir_boh-2/src/unique_char_counter_cli_kir_boh/tests/.pytest_cache/v/cache/nodeids`

 * *Files identical despite different names*

### Comparing `unique_char_counter_cli_kir_boh-1.5.8/LICENSE` & `unique_char_counter_cli_kir_boh-2/LICENSE`

 * *Files identical despite different names*

### Comparing `unique_char_counter_cli_kir_boh-1.5.8/README.md` & `unique_char_counter_cli_kir_boh-2/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -15,24 +15,28 @@
     
     read_file_in_chunks - reed file in chanks not to take a lot memory, gets two atrib 'path_to_file' (hasahable_obj) and
         chunck_size (by defoult chunck_size=1000)
     
     main - gets args from 'get_obj_from_cli', wich should be either file or string and hashable obj, then if it's fille,
         it will execute 'read_file_in_chunks' then 'return_amount_once_occured_items' to return and print result
 
-Hint: To use main you should import main from unique_char_counter_cli.py and run 'python main.py -s <hasable object>' 
-in the sane directory      
+Hint: To use main from venv: python -m env_name\lib\site-packages\unique_char_counter_cli_kir_boh\unique_char_counter_cli.py -s 'f'   
+      If you did't use venv: python -m path\shown\after\innstaling\unique_char_counter_cli_kir_boh\unique_char_counter_cli.py -s 'f' 
 ```
 #tests package:
 ```
 By imorting tests_unique_char_counter_cli.py from unique_char_counter_cli_kir_boh.tests you get the pyton file with 
 TestUniqueCharCounterCli class wich inheritate from unittest.TestCase. After imporing, it is used as parent class
         
     The test_return_amount_once_occured_items_with_string, test_return_amount_once_occured_items_with_empty_string,
         test_return_amount_once_occured_items_with_space, and test_return_amount_once_occured_items_with_unhashable_obj 
         methods test the return_amount_once_occured_items function with different inputs.
         
     The `test_main_with_mock_file` methods test the `main` function with different inputs using the `mock_open` and 
         `mock_get_obj_from_cli` decorators.
         
     The `test_read_file_in_chunks` method tests the `read_file_in_chunks` function with a file input.
+    
+Hint: To use unittests from venv: python -m env_name\lib\site-packages\unique_char_counter_cli_kir_boh\tests\test_unique_char_counter_cli.py
+      If you did't use venv: python -m path\shown\after\innstaling\unique_char_counter_cli_kir_boh\tests\test_unique_char_counter_cli.py
+      To use with coverage: coverage run -m unittest discover -s path\shown\after\innstaling\unique_char_counter_cli_kir_boh\tests
 ```
```

### Comparing `unique_char_counter_cli_kir_boh-1.5.8/pyproject.toml` & `unique_char_counter_cli_kir_boh-2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 
 [project]
 name = "unique_char_counter_cli_kir_boh"
-version = "1.5.8"
+version = "2"
 authors = [
   { name="Kiril Bogatiuk", email="kirillbogatu2005@gmail.com" },
 ]
 maintainers = [
-    {name ="Stanislav Hrytsyshyn", email="kirillbogatu2005@gmail.com"},
+    {name ="Stanislav Hrytsyshyn", email="NeZnavVashMail@gmail.com"},
 ]
 description = "Project gets hashable obj from cli an returns uniqe items amount, other funcs desribed in README.md"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `unique_char_counter_cli_kir_boh-1.5.8/PKG-INFO` & `unique_char_counter_cli_kir_boh-2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: unique_char_counter_cli_kir_boh
-Version: 1.5.8
+Version: 2
 Summary: Project gets hashable obj from cli an returns uniqe items amount, other funcs desribed in README.md
 Author-email: Kiril Bogatiuk <kirillbogatu2005@gmail.com>
-Maintainer-email: Stanislav Hrytsyshyn <kirillbogatu2005@gmail.com>
+Maintainer-email: Stanislav Hrytsyshyn <NeZnavVashMail@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
@@ -28,24 +28,28 @@
     
     read_file_in_chunks - reed file in chanks not to take a lot memory, gets two atrib 'path_to_file' (hasahable_obj) and
         chunck_size (by defoult chunck_size=1000)
     
     main - gets args from 'get_obj_from_cli', wich should be either file or string and hashable obj, then if it's fille,
         it will execute 'read_file_in_chunks' then 'return_amount_once_occured_items' to return and print result
 
-Hint: To use main you should import main from unique_char_counter_cli.py and run 'python main.py -s <hasable object>' 
-in the sane directory      
+Hint: To use main from venv: python -m env_name\lib\site-packages\unique_char_counter_cli_kir_boh\unique_char_counter_cli.py -s 'f'   
+      If you did't use venv: python -m path\shown\after\innstaling\unique_char_counter_cli_kir_boh\unique_char_counter_cli.py -s 'f' 
 ```
 #tests package:
 ```
 By imorting tests_unique_char_counter_cli.py from unique_char_counter_cli_kir_boh.tests you get the pyton file with 
 TestUniqueCharCounterCli class wich inheritate from unittest.TestCase. After imporing, it is used as parent class
         
     The test_return_amount_once_occured_items_with_string, test_return_amount_once_occured_items_with_empty_string,
         test_return_amount_once_occured_items_with_space, and test_return_amount_once_occured_items_with_unhashable_obj 
         methods test the return_amount_once_occured_items function with different inputs.
         
     The `test_main_with_mock_file` methods test the `main` function with different inputs using the `mock_open` and 
         `mock_get_obj_from_cli` decorators.
         
     The `test_read_file_in_chunks` method tests the `read_file_in_chunks` function with a file input.
+    
+Hint: To use unittests from venv: python -m env_name\lib\site-packages\unique_char_counter_cli_kir_boh\tests\test_unique_char_counter_cli.py
+      If you did't use venv: python -m path\shown\after\innstaling\unique_char_counter_cli_kir_boh\tests\test_unique_char_counter_cli.py
+      To use with coverage: coverage run -m unittest discover -s path\shown\after\innstaling\unique_char_counter_cli_kir_boh\tests
 ```
```

