# Comparing `tmp/threadsafe_shell-1.0.0.tar.gz` & `tmp/threadsafe_shell-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "threadsafe_shell-1.0.0.tar", last modified: Sat Nov  5 20:46:50 2022, max compression
+gzip compressed data, was "threadsafe_shell-1.1.0.tar", last modified: Mon May  8 19:54:19 2023, max compression
```

## Comparing `threadsafe_shell-1.0.0.tar` & `threadsafe_shell-1.1.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 kalamari  (1000) kalamari  (1001)        0 2022-11-05 20:46:50.209898 threadsafe_shell-1.0.0/
--rw-r--r--   0 kalamari  (1000) kalamari  (1001)     1071 2022-11-05 20:17:37.000000 threadsafe_shell-1.0.0/LICENSE
--rw-r--r--   0 kalamari  (1000) kalamari  (1001)      668 2022-11-05 20:46:50.209898 threadsafe_shell-1.0.0/PKG-INFO
--rw-r--r--   0 kalamari  (1000) kalamari  (1001)       88 2022-11-05 20:23:15.000000 threadsafe_shell-1.0.0/README.md
--rw-r--r--   0 kalamari  (1000) kalamari  (1001)      565 2022-11-05 20:45:25.000000 threadsafe_shell-1.0.0/pyproject.toml
--rw-r--r--   0 kalamari  (1000) kalamari  (1001)       38 2022-11-05 20:46:50.209898 threadsafe_shell-1.0.0/setup.cfg
-drwxr-xr-x   0 kalamari  (1000) kalamari  (1001)        0 2022-11-05 20:46:50.209898 threadsafe_shell-1.0.0/threadsafe_shell.egg-info/
--rw-r--r--   0 kalamari  (1000) kalamari  (1001)      668 2022-11-05 20:46:50.000000 threadsafe_shell-1.0.0/threadsafe_shell.egg-info/PKG-INFO
--rw-r--r--   0 kalamari  (1000) kalamari  (1001)      212 2022-11-05 20:46:50.000000 threadsafe_shell-1.0.0/threadsafe_shell.egg-info/SOURCES.txt
--rw-r--r--   0 kalamari  (1000) kalamari  (1001)        1 2022-11-05 20:46:50.000000 threadsafe_shell-1.0.0/threadsafe_shell.egg-info/dependency_links.txt
--rw-r--r--   0 kalamari  (1000) kalamari  (1001)       17 2022-11-05 20:46:50.000000 threadsafe_shell-1.0.0/threadsafe_shell.egg-info/top_level.txt
--rw-r--r--   0 kalamari  (1000) kalamari  (1001)     6144 2022-11-05 18:08:26.000000 threadsafe_shell-1.0.0/threadsafe_shell.py
+drwxr-xr-x   0 kalamari  (1000) kalamari  (1001)        0 2023-05-08 19:54:19.034354 threadsafe_shell-1.1.0/
+-rw-r--r--   0 kalamari  (1000) kalamari  (1001)     1071 2022-11-05 20:17:37.000000 threadsafe_shell-1.1.0/LICENSE
+-rw-r--r--   0 kalamari  (1000) kalamari  (1001)      668 2023-05-08 19:54:19.034354 threadsafe_shell-1.1.0/PKG-INFO
+-rw-r--r--   0 kalamari  (1000) kalamari  (1001)       88 2022-11-05 20:23:15.000000 threadsafe_shell-1.1.0/README.md
+-rw-r--r--   0 kalamari  (1000) kalamari  (1001)      565 2023-05-08 19:50:47.000000 threadsafe_shell-1.1.0/pyproject.toml
+-rw-r--r--   0 kalamari  (1000) kalamari  (1001)       38 2023-05-08 19:54:19.034354 threadsafe_shell-1.1.0/setup.cfg
+drwxr-xr-x   0 kalamari  (1000) kalamari  (1001)        0 2023-05-08 19:54:19.034354 threadsafe_shell-1.1.0/threadsafe_shell.egg-info/
+-rw-r--r--   0 kalamari  (1000) kalamari  (1001)      668 2023-05-08 19:54:19.000000 threadsafe_shell-1.1.0/threadsafe_shell.egg-info/PKG-INFO
+-rw-r--r--   0 kalamari  (1000) kalamari  (1001)      212 2023-05-08 19:54:19.000000 threadsafe_shell-1.1.0/threadsafe_shell.egg-info/SOURCES.txt
+-rw-r--r--   0 kalamari  (1000) kalamari  (1001)        1 2023-05-08 19:54:19.000000 threadsafe_shell-1.1.0/threadsafe_shell.egg-info/dependency_links.txt
+-rw-r--r--   0 kalamari  (1000) kalamari  (1001)       17 2023-05-08 19:54:19.000000 threadsafe_shell-1.1.0/threadsafe_shell.egg-info/top_level.txt
+-rw-r--r--   0 kalamari  (1000) kalamari  (1001)     6421 2023-05-08 19:48:37.000000 threadsafe_shell-1.1.0/threadsafe_shell.py
```

### Comparing `threadsafe_shell-1.0.0/LICENSE` & `threadsafe_shell-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `threadsafe_shell-1.0.0/PKG-INFO` & `threadsafe_shell-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threadsafe_shell
-Version: 1.0.0
+Version: 1.1.0
 Summary: A pure-python, thread-safe, queue-based logging and user input module
 Author-email: Calico Kalamari <kalamariking@proton.me>
 Project-URL: Homepage, https://github.com/KalamariKing/threadsafe-shell
 Project-URL: Bug Tracker, https://github.com/KalamariKing/threadsafe-shell/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `threadsafe_shell-1.0.0/pyproject.toml` & `threadsafe_shell-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "threadsafe_shell"
-version = "1.0.0"
+version = "1.1.0"
 authors = [
   { name="Calico Kalamari", email="kalamariking@proton.me" },
 ]
 description = "A pure-python, thread-safe, queue-based logging and user input module"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `threadsafe_shell-1.0.0/threadsafe_shell.egg-info/PKG-INFO` & `threadsafe_shell-1.1.0/threadsafe_shell.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threadsafe-shell
-Version: 1.0.0
+Version: 1.1.0
 Summary: A pure-python, thread-safe, queue-based logging and user input module
 Author-email: Calico Kalamari <kalamariking@proton.me>
 Project-URL: Homepage, https://github.com/KalamariKing/threadsafe-shell
 Project-URL: Bug Tracker, https://github.com/KalamariKing/threadsafe-shell/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `threadsafe_shell-1.0.0/threadsafe_shell.py` & `threadsafe_shell-1.1.0/threadsafe_shell.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,17 +28,18 @@
     
     
     def __init__(self, log_file=None, error_file=None, debug_level=3):
         # io
         self.__log_file = log_file
         self.__error_file = error_file
         self.DEBUG_LEVEL = debug_level
+        self.__is_debug_active = True
         # threading
         self.__queue = deque()
-        self.write_loop().start()
+        self.__get_write_loop_thread().start()
         self.__queue_lock = threading.Lock()
         self.__file_lock = threading.Lock()
         self.__input_lock = threading.Lock()
 
     
     def __handle_to_file(self, data:dict={}) -> None:
         if "text" not in data: raise KeyError("Key 'text' not found")
@@ -68,28 +69,34 @@
      
     def __write_loop(self):
         while True:
             if len(self.__queue):
                 with self.__queue_lock: val = self.__queue.popleft()
                 self.__handle_to_file(val)
     
-    def write_loop(self):
+    def __get_write_loop_thread(self):
         try:
             return self.thread
         except AttributeError:
             self.thread = threading.Thread(target=self.__write_loop, name="ShellWriteLoop-Daemon", daemon=True)
             return self.thread
     
     
     @staticmethod
     def highlight(obj: object, color:str=colors.PURPLE) -> str:
         return color + str(obj) + "\033[0m"
+    
+    def set_debug_level(self, level:int):
+        self.DEBUG_LEVEL = level
+    
+    def set_debug_active(self, is_debug_active:bool):
+        self.__is_debug_active = is_debug_active
 
     def debug(self, *args, level:int=3, **kwargs):
-        if level >= self.DEBUG_LEVEL:
+        if level >= self.DEBUG_LEVEL and self.is_debug_active:
             self.__add_to_queue("\033[30mDEBUG  ", *args, **kwargs)
     
     def log(self, *args, **kwargs):      self.__add_to_queue("\033[34mLOG    ", *args, **kwargs)
     def success(self, *args, **kwargs):  self.__add_to_queue("\033[32mPASS   ", *args, **kwargs)
     def warn(self, *args, **kwargs):     self.__add_to_queue("\033[33mWARN   ", *args, is_error=True, **kwargs)
     def error(self, *args, **kwargs):    self.__add_to_queue("\033[31mERROR  ", *args, is_error=True, **kwargs)
```

