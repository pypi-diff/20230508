# Comparing `tmp/pyjourney-0.1.3.tar.gz` & `tmp/pyjourney-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjourney-0.1.3.tar", max compression
+gzip compressed data, was "pyjourney-0.1.4.tar", max compression
```

## Comparing `pyjourney-0.1.3.tar` & `pyjourney-0.1.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      285 2023-05-08 18:47:43.793002 pyjourney-0.1.3/pyjourney/__init__.py
--rw-r--r--   0        0        0     3962 2023-05-08 19:24:30.985472 pyjourney-0.1.3/pyjourney/api.py
--rw-r--r--   0        0        0      421 2023-05-08 18:47:43.703228 pyjourney-0.1.3/pyjourney/exceptions.py
--rw-r--r--   0        0        0     2095 2023-05-08 19:32:20.598400 pyjourney-0.1.3/pyjourney/models.py
--rw-r--r--   0        0        0      651 2023-05-08 19:35:29.821050 pyjourney-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1332 2023-05-08 19:15:06.713347 pyjourney-0.1.3/README.md
--rw-r--r--   0        0        0     2035 1970-01-01 00:00:00.000000 pyjourney-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      285 2023-05-08 18:47:43.793002 pyjourney-0.1.4/pyjourney/__init__.py
+-rw-r--r--   0        0        0     3915 2023-05-08 19:37:06.751509 pyjourney-0.1.4/pyjourney/api.py
+-rw-r--r--   0        0        0      421 2023-05-08 18:47:43.703228 pyjourney-0.1.4/pyjourney/exceptions.py
+-rw-r--r--   0        0        0     2095 2023-05-08 19:32:20.598400 pyjourney-0.1.4/pyjourney/models.py
+-rw-r--r--   0        0        0      651 2023-05-08 19:37:15.002859 pyjourney-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1332 2023-05-08 19:15:06.713347 pyjourney-0.1.4/README.md
+-rw-r--r--   0        0        0     2035 1970-01-01 00:00:00.000000 pyjourney-0.1.4/PKG-INFO
```

### Comparing `pyjourney-0.1.3/pyjourney/api.py` & `pyjourney-0.1.4/pyjourney/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,21 +23,19 @@
             "authority": "www.midjourney.com",
             "accept": "*/*",
             "accept-language": "en-US,en;q=0.9",
             "dnt": "1",
             "referer": "https://www.midjourney.com/app/"
         }
 
-        self.session = self.get_session_from_env()
-        self.user_id = user_id
-
         if not cookie:
             cookie = os.getenv("MIDJOURNEY_COOKIE")
-        
-        self.get_session_from_env(cookie)
+
+        self.session = self.get_session_from_env(cookie)
+        self.user_id = user_id
 
     def get_session_from_env(self, cookie: str):
         """Returns a session from the environment variables
 
         Arguments:
             env_var {str} -- The name of the environment variable us for sessions
```

### Comparing `pyjourney-0.1.3/pyjourney/models.py` & `pyjourney-0.1.4/pyjourney/models.py`

 * *Files identical despite different names*

### Comparing `pyjourney-0.1.3/pyproject.toml` & `pyjourney-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyjourney"
-version = "0.1.3"
+version = "0.1.4"
 description = "Python module for interacting with the MidJourney API"
 authors = ["agentd00nut <agentd00nut@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/agentd00nut/pyjourney"
 repository = "https://github.com/agentd00nut/pyjourney"
 keywords = ["journey", "midjourney", "api", "python"]
```

### Comparing `pyjourney-0.1.3/README.md` & `pyjourney-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `pyjourney-0.1.3/PKG-INFO` & `pyjourney-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjourney
-Version: 0.1.3
+Version: 0.1.4
 Summary: Python module for interacting with the MidJourney API
 Home-page: https://github.com/agentd00nut/pyjourney
 License: MIT
 Keywords: journey,midjourney,api,python
 Author: agentd00nut
 Author-email: agentd00nut@gmail.com
 Requires-Python: >=3.10,<4.0
```

