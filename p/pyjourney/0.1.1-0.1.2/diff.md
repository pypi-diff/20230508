# Comparing `tmp/pyjourney-0.1.1.tar.gz` & `tmp/pyjourney-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjourney-0.1.1.tar", max compression
+gzip compressed data, was "pyjourney-0.1.2.tar", max compression
```

## Comparing `pyjourney-0.1.1.tar` & `pyjourney-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      285 2023-05-08 18:47:43.793002 pyjourney-0.1.1/pyjourney/__init__.py
--rw-r--r--   0        0        0     3892 2023-05-08 18:54:08.141626 pyjourney-0.1.1/pyjourney/api.py
--rw-r--r--   0        0        0      421 2023-05-08 18:47:43.703228 pyjourney-0.1.1/pyjourney/exceptions.py
--rw-r--r--   0        0        0     2090 2023-05-08 18:54:28.738020 pyjourney-0.1.1/pyjourney/models.py
--rw-r--r--   0        0        0      651 2023-05-08 19:08:42.264374 pyjourney-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1287 2023-05-08 18:37:05.761070 pyjourney-0.1.1/README.md
--rw-r--r--   0        0        0     1990 1970-01-01 00:00:00.000000 pyjourney-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      285 2023-05-08 18:47:43.793002 pyjourney-0.1.2/pyjourney/__init__.py
+-rw-r--r--   0        0        0     3962 2023-05-08 19:24:30.985472 pyjourney-0.1.2/pyjourney/api.py
+-rw-r--r--   0        0        0      421 2023-05-08 18:47:43.703228 pyjourney-0.1.2/pyjourney/exceptions.py
+-rw-r--r--   0        0        0     2090 2023-05-08 18:54:28.738020 pyjourney-0.1.2/pyjourney/models.py
+-rw-r--r--   0        0        0      651 2023-05-08 19:25:28.664421 pyjourney-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1332 2023-05-08 19:15:06.713347 pyjourney-0.1.2/README.md
+-rw-r--r--   0        0        0     2035 1970-01-01 00:00:00.000000 pyjourney-0.1.2/PKG-INFO
```

### Comparing `pyjourney-0.1.1/pyjourney/api.py` & `pyjourney-0.1.2/pyjourney/api.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from pyjourney.models import GetJobsArgs
 
 
 class MidjourneyAPI:
     """Class for interacting with the Midjourney API
     """
 
-    def __init__(self, user_id: str = None):
+    def __init__(self, user_id: str = None, cookie=None):
         self.logger = logging.getLogger(__name__)
         self.logger.setLevel(logging.DEBUG)
         self.logger.addHandler(logging.StreamHandler())
         self.logger.debug("MidjourneyAPI initialized")
 
         self.root_url = "https://www.midjourney.com"
 
@@ -26,37 +26,40 @@
             "dnt": "1",
             "referer": "https://www.midjourney.com/app/"
         }
 
         self.session = self.get_session_from_env()
         self.user_id = user_id
 
-    def get_session_from_env(self, env_var: str = "MIDJOURNEY_COOKIE"):
+        if not cookie:
+            cookie = os.getenv("MIDJOURNEY_COOKIE")
+        
+        self.get_session_from_env(cookie)
+
+    def get_session_from_env(self, cookie: str):
         """Returns a session from the environment variables
 
         Arguments:
             env_var {str} -- The name of the environment variable us for sessions
 
         Returns:
             requests.Session -- The session
 
         Raises:
             SessionException -- If the environment variable is not found
         """
-
-        cookie_string = os.getenv(env_var)
-
-        if not cookie_string:
+        
+        if not cookie:
             raise SessionException(
                 "Session file not found and no session in environment variables did you set the MIDJOURNEY_COOKIE environment variable?"
             )
 
         # https://stackoverflow.com/questions/17224054/how-to-add-a-cookie-to-the-cookiejar-in-python-requests-library
         cookiejar_dict = {}
-        for cookie_string in cookie_string.split(";"):
+        for cookie_string in cookie.split(";"):
             # maxsplit=1 because cookie value may have "="
             cookie_key, cookie_value = cookie_string.strip().split("=", maxsplit=1)
             cookiejar_dict[cookie_key] = cookie_value
 
         if cookiejar_dict == {}:
             raise SessionException(
                 "Session file found, but no cookies in file")
```

### Comparing `pyjourney-0.1.1/pyjourney/models.py` & `pyjourney-0.1.2/pyjourney/models.py`

 * *Files identical despite different names*

### Comparing `pyjourney-0.1.1/pyproject.toml` & `pyjourney-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyjourney"
-version = "0.1.1"
+version = "0.1.2"
 description = "Python module for interacting with the MidJourney API"
 authors = ["agentd00nut <agentd00nut@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/agentd00nut/pyjourney"
 repository = "https://github.com/agentd00nut/pyjourney"
 keywords = ["journey", "midjourney", "api", "python"]
```

### Comparing `pyjourney-0.1.1/README.md` & `pyjourney-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # PyJourney
 
 A python module for calling the Midjourney API to get job details and for creating jobs.
 
 Currently just trying to fix [midjourney-graph](https://github.com/agentd00nut/midjourney-graph) and figured i'd break out the api calls into a module.
 
+[pypi](https://pypi.org/project/pyjourney/)
+
 ## TODO
 
 - [ ] more than 35 jobs at a time.
 - [ ] jobs by date range, type, and for other users
 - [ ] get sepcific job details for a job and a list of jobs
 - [ ] get the list of community jobs by hot, new, trending, etc.
 - [ ] Searching for jobs by title, description, and tags
```

### Comparing `pyjourney-0.1.1/PKG-INFO` & `pyjourney-0.1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjourney
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python module for interacting with the MidJourney API
 Home-page: https://github.com/agentd00nut/pyjourney
 License: MIT
 Keywords: journey,midjourney,api,python
 Author: agentd00nut
 Author-email: agentd00nut@gmail.com
 Requires-Python: >=3.10,<4.0
@@ -19,14 +19,16 @@
 
 # PyJourney
 
 A python module for calling the Midjourney API to get job details and for creating jobs.
 
 Currently just trying to fix [midjourney-graph](https://github.com/agentd00nut/midjourney-graph) and figured i'd break out the api calls into a module.
 
+[pypi](https://pypi.org/project/pyjourney/)
+
 ## TODO
 
 - [ ] more than 35 jobs at a time.
 - [ ] jobs by date range, type, and for other users
 - [ ] get sepcific job details for a job and a list of jobs
 - [ ] get the list of community jobs by hot, new, trending, etc.
 - [ ] Searching for jobs by title, description, and tags
```

