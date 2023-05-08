# Comparing `tmp/python_opensky-0.0.5.tar.gz` & `tmp/python_opensky-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_opensky-0.0.5.tar", max compression
+gzip compressed data, was "python_opensky-0.0.6.tar", max compression
```

## Comparing `python_opensky-0.0.5.tar` & `python_opensky-0.0.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1077 2023-05-07 22:20:29.800087 python_opensky-0.0.5/LICENSE.md
--rw-r--r--   0        0        0     5324 2023-05-07 22:20:29.800087 python_opensky-0.0.5/README.md
--rw-r--r--   0        0        0     3659 2023-05-07 22:20:51.844076 python_opensky-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      444 2023-05-07 22:20:29.804087 python_opensky-0.0.5/src/python_opensky/__init__.py
--rw-r--r--   0        0        0      753 2023-05-07 22:20:29.804087 python_opensky-0.0.5/src/python_opensky/const.py
--rw-r--r--   0        0        0      202 2023-05-07 22:20:29.804087 python_opensky-0.0.5/src/python_opensky/exceptions.py
--rw-r--r--   0        0        0     2822 2023-05-07 22:20:29.804087 python_opensky-0.0.5/src/python_opensky/models.py
--rw-r--r--   0        0        0     4499 2023-05-07 22:20:29.804087 python_opensky-0.0.5/src/python_opensky/opensky.py
--rw-r--r--   0        0        0        0 2023-05-07 22:20:29.804087 python_opensky-0.0.5/src/python_opensky/py.typed
--rw-r--r--   0        0        0     6726 1970-01-01 00:00:00.000000 python_opensky-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-05-08 15:43:19.410883 python_opensky-0.0.6/LICENSE.md
+-rw-r--r--   0        0        0     5328 2023-05-08 15:43:19.410883 python_opensky-0.0.6/README.md
+-rw-r--r--   0        0        0     3659 2023-05-08 15:43:45.228431 python_opensky-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      444 2023-05-08 15:43:19.414884 python_opensky-0.0.6/src/python_opensky/__init__.py
+-rw-r--r--   0        0        0      849 2023-05-08 15:43:19.414884 python_opensky-0.0.6/src/python_opensky/const.py
+-rw-r--r--   0        0        0      384 2023-05-08 15:43:19.414884 python_opensky-0.0.6/src/python_opensky/exceptions.py
+-rw-r--r--   0        0        0     3573 2023-05-08 15:43:19.414884 python_opensky-0.0.6/src/python_opensky/models.py
+-rw-r--r--   0        0        0     7400 2023-05-08 15:43:19.414884 python_opensky-0.0.6/src/python_opensky/opensky.py
+-rw-r--r--   0        0        0        0 2023-05-08 15:43:19.414884 python_opensky-0.0.6/src/python_opensky/py.typed
+-rw-r--r--   0        0        0     6730 1970-01-01 00:00:00.000000 python_opensky-0.0.6/PKG-INFO
```

### Comparing `python_opensky-0.0.5/LICENSE.md` & `python_opensky-0.0.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `python_opensky-0.0.5/README.md` & `python_opensky-0.0.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 from python_opensky import OpenSky, StatesResponse
 
 
 async def main() -> None:
     """Show example of fetching all flight states."""
     async with OpenSky() as opensky:
-        states: StatesResponse = await opensky.states()
+        states: StatesResponse = await opensky.get_states()
         print(states)
 
 
 if __name__ == "__main__":
     asyncio.run(main())
 ```
```

### Comparing `python_opensky-0.0.5/pyproject.toml` & `python_opensky-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python_opensky"
-version = "0.0.5"
+version = "0.0.6"
 description = "Asynchronous Python client for Opensky API."
 authors = ["Joost Lekkerkerker <joostlek@outlook.com>"]
 maintainers = ["Joost Lekkerkerker <joostlek@outlook.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/joostlek/python-opensky"
 repository = "https://github.com/joostlek/python-opensky"
```

### Comparing `python_opensky-0.0.5/src/python_opensky/const.py` & `python_opensky-0.0.6/src/python_opensky/const.py`

 * *Files 14% similar despite different names*

```diff
@@ -31,7 +31,13 @@
     UNMANNED_AERIAL_VEHICLE = 14
     SPACE_VEHICLE = 15
     EMERGENCY_VEHICLE = 16
     SERVICE_VEHICLE = 17
     POINT_OBSTACLE = 18
     CLUSTER_OBSTACLE = 19
     LINE_OBSTACLE = 20
+
+
+MIN_LATITUDE = "lamin"
+MAX_LATITUDE = "lamax"
+MIN_LONGITUDE = "lomin"
+MAX_LONGITUDE = "lomax"
```

### Comparing `python_opensky-0.0.5/PKG-INFO` & `python_opensky-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-opensky
-Version: 0.0.5
+Version: 0.0.6
 Summary: Asynchronous Python client for Opensky API.
 Home-page: https://github.com/joostlek/python-opensky
 License: MIT
 Keywords: opensky,api,async,client
 Author: Joost Lekkerkerker
 Author-email: joostlek@outlook.com
 Maintainer: Joost Lekkerkerker
@@ -62,15 +62,15 @@
 
 from python_opensky import OpenSky, StatesResponse
 
 
 async def main() -> None:
     """Show example of fetching all flight states."""
     async with OpenSky() as opensky:
-        states: StatesResponse = await opensky.states()
+        states: StatesResponse = await opensky.get_states()
         print(states)
 
 
 if __name__ == "__main__":
     asyncio.run(main())
 ```
```

