# Comparing `tmp/nsdotpy-1.1.3.tar.gz` & `tmp/nsdotpy-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nsdotpy-1.1.3.tar", max compression
+gzip compressed data, was "nsdotpy-1.1.4.tar", max compression
```

## Comparing `nsdotpy-1.1.3.tar` & `nsdotpy-1.1.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35005 2023-04-26 23:31:32.556941 nsdotpy-1.1.3/LICENSE.md
--rw-r--r--   0        0        0      805 2023-05-06 06:05:20.689321 nsdotpy-1.1.3/nsdotpy/__init__.py
--rw-r--r--   0        0        0    36937 2023-05-08 03:40:29.548242 nsdotpy-1.1.3/nsdotpy/session.py
--rw-r--r--   0        0        0     2400 2023-05-06 06:05:24.536374 nsdotpy-1.1.3/nsdotpy/valid_tags.py
--rw-r--r--   0        0        0      667 2023-05-08 03:44:44.215911 nsdotpy-1.1.3/pyproject.toml
--rw-r--r--   0        0        0     2454 2023-05-08 03:53:02.121422 nsdotpy-1.1.3/README.md
--rw-r--r--   0        0        0     3279 1970-01-01 00:00:00.000000 nsdotpy-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0    35005 2023-04-26 23:31:32.556941 nsdotpy-1.1.4/LICENSE.md
+-rw-r--r--   0        0        0      805 2023-05-06 06:05:20.689321 nsdotpy-1.1.4/nsdotpy/__init__.py
+-rw-r--r--   0        0        0    36960 2023-05-08 07:41:28.765764 nsdotpy-1.1.4/nsdotpy/session.py
+-rw-r--r--   0        0        0     2400 2023-05-06 06:05:24.536374 nsdotpy-1.1.4/nsdotpy/valid_tags.py
+-rw-r--r--   0        0        0      667 2023-05-08 07:41:35.119119 nsdotpy-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2458 2023-05-08 04:15:34.807948 nsdotpy-1.1.4/README.md
+-rw-r--r--   0        0        0     3283 1970-01-01 00:00:00.000000 nsdotpy-1.1.4/PKG-INFO
```

### Comparing `nsdotpy-1.1.3/LICENSE.md` & `nsdotpy-1.1.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `nsdotpy-1.1.3/nsdotpy/__init__.py` & `nsdotpy-1.1.4/nsdotpy/__init__.py`

 * *Files identical despite different names*

### Comparing `nsdotpy-1.1.3/nsdotpy/session.py` & `nsdotpy-1.1.4/nsdotpy/session.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
             script_version (str): Version number of your script
             script_author (str): Author of your script
             script_user (str): Nation name of the user running your script
             keybind (str, optional): Keybind to count as a user click. Defaults to "space".
             link_to_src (str, optional): Link to the source code of your script.
             logger (logging.Logger | None, optional): Logger to use. Will create its own with name "NSDotPy" if none is specified. Defaults to None.
         """
-        self.VERSION = "1.1.3"
+        self.VERSION = "1.1.4"
         # Initialize logger
         if not logger:
             self._init_logger()
         else:
             self.logger = logger
         # Attach the tendo singleton to the session object so it can
         # only be run once at a time, avoiding simultaneity issues
@@ -125,15 +125,15 @@
         if localid := soup.find("input", {"name": "localid"}):
             self.localid = localid["value"].strip()  # type: ignore
         if pin := self._session.cookies.get("pin"):
             # you should never really need the pin but just in case i'll store it
             self.pin = pin
         if soup.find("a", {"class": "STANDOUT"}):
             self.region = canonicalize(
-                soup.find_all("a", {"class": "STANDOUT"})[1].text
+                soup.find_all("a", {"class": "STANDOUT"})[1].attrs["href"].split("=")[1]
             )
 
     def _refresh_auth_values(self):
         response = self.request(
             f"https://www.nationstates.net/page=display_region/region={self._auth_region}",
             data={"theme": "century"},
         )
```

### Comparing `nsdotpy-1.1.3/nsdotpy/valid_tags.py` & `nsdotpy-1.1.4/nsdotpy/valid_tags.py`

 * *Files identical despite different names*

### Comparing `nsdotpy-1.1.3/pyproject.toml` & `nsdotpy-1.1.4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nsdotpy"
-version = "1.1.3"
+version = "1.1.4"
 description = "A wrapper around requests that abstracts away interacting with the HTML nationstates.net site. Focused on legality, correctness, and ease of use."
 authors = ["audrey <audreyreal@proton.me>"]
 license = "AGPL-3.0-or-later"
 readme = "README.md"
 repository = "https://github.com/sw33ze/NSDotPy"
 
 [tool.poetry.dependencies]
```

### Comparing `nsdotpy-1.1.3/README.md` & `nsdotpy-1.1.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 - Dossier and reports handling
 - More fleshed out API Client
 - Cards support
 - Migrate automatic docs generation, code formatting, and PyPI uploading to GitHub Actions for better CI
 
 ## Docs
 
-https://sw33ze.github.io/NSDotPy/src/session.html#NSSession
+https://sw33ze.github.io/NSDotPy/nsdotpy/session.html#NSSession
 
 ## Generating Docs
 
 1. [Ensure poetry is installed](https://python-poetry.org/docs/#installation), or your system's package manager if applicable.
 2. Run `poetry install` in the root directory of the project to install dependencies if you haven't already.
 3. Run `poetry run pdoc nsdotpy/session.py -d=google -o=docs/` to generate the docs
```

### Comparing `nsdotpy-1.1.3/PKG-INFO` & `nsdotpy-1.1.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nsdotpy
-Version: 1.1.3
+Version: 1.1.4
 Summary: A wrapper around requests that abstracts away interacting with the HTML nationstates.net site. Focused on legality, correctness, and ease of use.
 Home-page: https://github.com/sw33ze/NSDotPy
 License: AGPL-3.0-or-later
 Author: audrey
 Author-email: audreyreal@proton.me
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
@@ -41,15 +41,15 @@
 - Dossier and reports handling
 - More fleshed out API Client
 - Cards support
 - Migrate automatic docs generation, code formatting, and PyPI uploading to GitHub Actions for better CI
 
 ## Docs
 
-https://sw33ze.github.io/NSDotPy/src/session.html#NSSession
+https://sw33ze.github.io/NSDotPy/nsdotpy/session.html#NSSession
 
 ## Generating Docs
 
 1. [Ensure poetry is installed](https://python-poetry.org/docs/#installation), or your system's package manager if applicable.
 2. Run `poetry install` in the root directory of the project to install dependencies if you haven't already.
 3. Run `poetry run pdoc nsdotpy/session.py -d=google -o=docs/` to generate the docs
```

