# Comparing `tmp/chatplayground-1.0.1.tar.gz` & `tmp/chatplayground-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatplayground-1.0.1.tar", max compression
+gzip compressed data, was "chatplayground-1.0.2.tar", max compression
```

## Comparing `chatplayground-1.0.1.tar` & `chatplayground-1.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    34523 2023-05-08 19:28:30.338983 chatplayground-1.0.1/LICENSE
--rw-r--r--   0        0        0     4471 2023-05-08 19:28:30.338983 chatplayground-1.0.1/README.md
--rw-r--r--   0        0        0       17 2023-05-08 19:28:30.342984 chatplayground-1.0.1/chatplayground/.gitignore
--rw-r--r--   0        0        0       22 2023-05-08 19:28:30.342984 chatplayground-1.0.1/chatplayground/__init__.py
--rw-r--r--   0        0        0        0 2023-05-08 19:28:30.342984 chatplayground-1.0.1/chatplayground/app/__init__.py
--rw-r--r--   0        0        0   104390 2023-05-08 19:28:30.342984 chatplayground-1.0.1/chatplayground/app/app.py
--rw-r--r--   0        0        0    15406 2023-05-08 19:28:30.342984 chatplayground-1.0.1/chatplayground/assets/favicon.ico
--rw-r--r--   0        0        0     1281 2023-05-08 19:28:30.342984 chatplayground-1.0.1/chatplayground/assets/react-json-view-lite.css
--rw-r--r--   0        0        0   178190 2023-05-08 19:28:30.342984 chatplayground-1.0.1/chatplayground/message_threads/faust_in_oxford_1683330128.209918.json
--rw-r--r--   0        0        0      756 2023-05-08 19:28:30.342984 chatplayground-1.0.1/chatplayground/pcconfig.py
--rw-r--r--   0        0        0     3081 2023-05-08 19:28:30.366984 chatplayground-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     6838 1970-01-01 00:00:00.000000 chatplayground-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-05-08 19:47:46.220814 chatplayground-1.0.2/LICENSE
+-rw-r--r--   0        0        0     4471 2023-05-08 19:47:46.220814 chatplayground-1.0.2/README.md
+-rw-r--r--   0        0        0       17 2023-05-08 19:47:46.220814 chatplayground-1.0.2/chatplayground/.gitignore
+-rw-r--r--   0        0        0       22 2023-05-08 19:47:46.220814 chatplayground-1.0.2/chatplayground/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-08 19:47:46.220814 chatplayground-1.0.2/chatplayground/app/__init__.py
+-rw-r--r--   0        0        0   104390 2023-05-08 19:47:46.220814 chatplayground-1.0.2/chatplayground/app/app.py
+-rw-r--r--   0        0        0    15406 2023-05-08 19:47:46.220814 chatplayground-1.0.2/chatplayground/assets/favicon.ico
+-rw-r--r--   0        0        0     1281 2023-05-08 19:47:46.220814 chatplayground-1.0.2/chatplayground/assets/react-json-view-lite.css
+-rw-r--r--   0        0        0   178190 2023-05-08 19:47:46.220814 chatplayground-1.0.2/chatplayground/message_threads/faust_in_oxford_1683330128.209918.json
+-rw-r--r--   0        0        0      850 2023-05-08 19:47:46.220814 chatplayground-1.0.2/chatplayground/pcconfig.py
+-rw-r--r--   0        0        0     3081 2023-05-08 19:47:46.244814 chatplayground-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     6838 1970-01-01 00:00:00.000000 chatplayground-1.0.2/PKG-INFO
```

### Comparing `chatplayground-1.0.1/LICENSE` & `chatplayground-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `chatplayground-1.0.1/README.md` & `chatplayground-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `chatplayground-1.0.1/chatplayground/app/app.py` & `chatplayground-1.0.2/chatplayground/app/app.py`

 * *Files identical despite different names*

### Comparing `chatplayground-1.0.1/chatplayground/assets/favicon.ico` & `chatplayground-1.0.2/chatplayground/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `chatplayground-1.0.1/chatplayground/assets/react-json-view-lite.css` & `chatplayground-1.0.2/chatplayground/assets/react-json-view-lite.css`

 * *Files identical despite different names*

### Comparing `chatplayground-1.0.1/chatplayground/message_threads/faust_in_oxford_1683330128.209918.json` & `chatplayground-1.0.2/chatplayground/message_threads/faust_in_oxford_1683330128.209918.json`

 * *Files identical despite different names*

### Comparing `chatplayground-1.0.1/chatplayground/pcconfig.py` & `chatplayground-1.0.2/chatplayground/pcconfig.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,13 +20,14 @@
 
 def main():
     """This is the entry point for the CLI."""
     # Add the chatplayground directory to PYTHONPATH and change directories into it
     os.environ["PYTHONPATH"] = os.path.abspath(os.path.dirname(__file__))
     os.chdir(os.path.dirname(__file__))
     print(os.getcwd())
-    subprocess.run(["pc", "init"])
+    # execute `pc init` in the current directory as a subprocess
+    subprocess.run(["pc", "init"], check=True, cwd=os.getcwd())
     cli.main(["run"] + sys.argv[1:])
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `chatplayground-1.0.1/pyproject.toml` & `chatplayground-1.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "chatplayground"
-version = "1.0.1"
+version = "1.0.2"
 homepage = "https://github.com/blackhc/chatplayground"
 description = "ChatPlayground for LLMs"
 authors = ["Andreas Kirsch <blackhc@gmail.com>"]
 readme = "README.md"
 license =  "GPL-3.0-only"
 classifiers=[
     'Development Status :: 4 - Beta',
```

### Comparing `chatplayground-1.0.1/PKG-INFO` & `chatplayground-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatplayground
-Version: 1.0.1
+Version: 1.0.2
 Summary: ChatPlayground for LLMs
 Home-page: https://github.com/blackhc/chatplayground
 License: GPL-3.0-only
 Author: Andreas Kirsch
 Author-email: blackhc@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
```

