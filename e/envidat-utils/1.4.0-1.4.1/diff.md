# Comparing `tmp/envidat-utils-1.4.0.tar.gz` & `tmp/envidat-utils-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "envidat-utils-1.4.0.tar", last modified: Wed May  3 18:12:35 2023, max compression
+gzip compressed data, was "envidat-utils-1.4.1.tar", last modified: Mon May  8 14:27:41 2023, max compression
```

## Comparing `envidat-utils-1.4.0.tar` & `envidat-utils-1.4.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     9547 2023-05-03 13:23:42.890763 envidat-utils-1.4.0/CHANGELOG.md
--rw-r--r--   0        0        0     1063 2023-02-27 14:54:50.816189 envidat-utils-1.4.0/LICENCE
--rw-r--r--   0        0        0     1662 2023-02-27 14:54:50.816189 envidat-utils-1.4.0/README.md
--rw-r--r--   0        0        0       67 2023-02-27 14:54:50.816189 envidat-utils-1.4.0/envidat/__init__.py
--rw-r--r--   0        0        0       43 2023-05-03 13:23:42.890763 envidat-utils-1.4.0/envidat/__version__.py
--rw-r--r--   0        0        0       37 2023-02-27 14:54:50.816189 envidat-utils-1.4.0/envidat/api/__init__.py
--rw-r--r--   0        0        0     9122 2023-05-03 18:00:21.076933 envidat-utils-1.4.0/envidat/api/v1.py
--rw-r--r--   0        0        0     3161 2023-03-14 10:34:09.273358 envidat-utils-1.4.0/envidat/config/config_converters.json
--rw-r--r--   0        0        0       69 2023-02-27 14:54:50.816189 envidat-utils-1.4.0/envidat/converters/__init__.py
--rw-r--r--   0        0        0     2319 2023-02-27 14:54:50.816189 envidat-utils-1.4.0/envidat/converters/bibtex_converter.py
--rw-r--r--   0        0        0    48992 2023-05-03 18:00:21.076933 envidat-utils-1.4.0/envidat/converters/datacite_converter.py
--rw-r--r--   0        0        0    13207 2023-05-03 16:14:00.341772 envidat-utils-1.4.0/envidat/converters/dcat_ap_converter.py
--rw-r--r--   0        0        0    27401 2023-05-03 13:18:42.987030 envidat-utils-1.4.0/envidat/converters/dif_converter.py
--rw-r--r--   0        0        0    24536 2023-05-03 13:18:42.987030 envidat-utils-1.4.0/envidat/converters/iso_converter.py
--rw-r--r--   0        0        0     2622 2023-02-27 14:54:50.816189 envidat-utils-1.4.0/envidat/converters/ris_converter.py
--rw-r--r--   0        0        0     1486 2023-05-03 13:18:42.987030 envidat-utils-1.4.0/envidat/converters/xml_converter.py
--rw-r--r--   0        0        0       73 2023-04-04 10:16:28.915663 envidat-utils-1.4.0/envidat/doi/__init__.py
--rw-r--r--   0        0        0     6881 2023-05-03 18:00:21.076933 envidat-utils-1.4.0/envidat/doi/datacite_publisher.py
--rw-r--r--   0        0        0    10657 2023-05-03 18:00:21.076933 envidat-utils-1.4.0/envidat/doi/datacite_updater.py
--rw-r--r--   0        0        0     8529 2023-05-03 16:14:00.341772 envidat-utils-1.4.0/envidat/metadata.py
--rw-r--r--   0        0        0       20 2023-02-27 14:54:50.816189 envidat-utils-1.4.0/envidat/s3/__init__.py
--rw-r--r--   0        0        0    42309 2023-05-03 16:14:00.345772 envidat-utils-1.4.0/envidat/s3/bucket.py
--rw-r--r--   0        0        0     3118 2023-02-27 14:54:50.816189 envidat-utils-1.4.0/envidat/s3/exceptions.py
--rw-r--r--   0        0        0     6662 2023-05-03 18:09:51.816011 envidat-utils-1.4.0/envidat/utils.py
--rw-r--r--   0        0        0     2173 2023-05-03 18:09:51.816011 envidat-utils-1.4.0/pyproject.toml
--rw-r--r--   0        0        0       38 2023-02-27 14:54:50.820189 envidat-utils-1.4.0/tests/__init__.py
--rw-r--r--   0        0        0    22302 2023-05-03 16:14:00.345772 envidat-utils-1.4.0/tests/conftest.py
--rw-r--r--   0        0        0      177 2023-02-27 14:54:50.820189 envidat-utils-1.4.0/tests/test_api.py
--rw-r--r--   0        0        0    14075 2023-02-27 14:54:50.820189 envidat-utils-1.4.0/tests/test_bucket_io.py
--rw-r--r--   0        0        0     5101 2023-05-03 13:18:42.987030 envidat-utils-1.4.0/tests/test_bucket_utils.py
--rw-r--r--   0        0        0    16141 2023-05-03 16:14:00.345772 envidat-utils-1.4.0/tests/test_converters.py
--rw-r--r--   0        0        0     3794 2023-05-03 16:14:00.345772 envidat-utils-1.4.0/tests/test_metadata.py
--rw-r--r--   0        0        0     2356 1970-01-01 00:00:00.000000 envidat-utils-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0     9626 2023-05-08 14:25:45.994832 envidat-utils-1.4.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1063 2023-02-27 15:51:29.521721 envidat-utils-1.4.1/LICENCE
+-rw-r--r--   0        0        0     2034 2023-05-08 14:25:45.994832 envidat-utils-1.4.1/README.md
+-rw-r--r--   0        0        0       67 2023-02-27 15:51:29.525721 envidat-utils-1.4.1/envidat/__init__.py
+-rw-r--r--   0        0        0       43 2023-05-08 14:25:45.994832 envidat-utils-1.4.1/envidat/__version__.py
+-rw-r--r--   0        0        0       37 2023-02-27 15:51:29.525721 envidat-utils-1.4.1/envidat/api/__init__.py
+-rw-r--r--   0        0        0     9116 2023-05-08 14:25:45.994832 envidat-utils-1.4.1/envidat/api/v1.py
+-rw-r--r--   0        0        0     3161 2023-05-03 16:04:39.414812 envidat-utils-1.4.1/envidat/config/config_converters.json
+-rw-r--r--   0        0        0       69 2023-02-27 15:51:29.525721 envidat-utils-1.4.1/envidat/converters/__init__.py
+-rw-r--r--   0        0        0     2319 2023-02-27 15:51:29.525721 envidat-utils-1.4.1/envidat/converters/bibtex_converter.py
+-rw-r--r--   0        0        0    48986 2023-05-08 14:25:45.994832 envidat-utils-1.4.1/envidat/converters/datacite_converter.py
+-rw-r--r--   0        0        0    13207 2023-05-03 16:04:39.414812 envidat-utils-1.4.1/envidat/converters/dcat_ap_converter.py
+-rw-r--r--   0        0        0    27401 2023-05-03 16:04:39.414812 envidat-utils-1.4.1/envidat/converters/dif_converter.py
+-rw-r--r--   0        0        0    24536 2023-05-03 16:04:39.414812 envidat-utils-1.4.1/envidat/converters/iso_converter.py
+-rw-r--r--   0        0        0     2622 2023-02-27 15:51:29.525721 envidat-utils-1.4.1/envidat/converters/ris_converter.py
+-rw-r--r--   0        0        0     1486 2023-05-03 16:04:39.414812 envidat-utils-1.4.1/envidat/converters/xml_converter.py
+-rw-r--r--   0        0        0       73 2023-05-03 16:04:39.414812 envidat-utils-1.4.1/envidat/doi/__init__.py
+-rw-r--r--   0        0        0     6875 2023-05-08 14:25:45.994832 envidat-utils-1.4.1/envidat/doi/datacite_publisher.py
+-rw-r--r--   0        0        0    10651 2023-05-08 14:25:45.994832 envidat-utils-1.4.1/envidat/doi/datacite_updater.py
+-rw-r--r--   0        0        0     8529 2023-05-03 16:04:39.414812 envidat-utils-1.4.1/envidat/metadata.py
+-rw-r--r--   0        0        0       20 2023-02-27 15:51:29.525721 envidat-utils-1.4.1/envidat/s3/__init__.py
+-rw-r--r--   0        0        0    42309 2023-05-03 16:04:39.414812 envidat-utils-1.4.1/envidat/s3/bucket.py
+-rw-r--r--   0        0        0     3118 2023-02-27 15:51:29.525721 envidat-utils-1.4.1/envidat/s3/exceptions.py
+-rw-r--r--   0        0        0     6976 2023-05-08 14:25:45.994832 envidat-utils-1.4.1/envidat/utils.py
+-rw-r--r--   0        0        0     2173 2023-05-08 14:25:45.994832 envidat-utils-1.4.1/pyproject.toml
+-rw-r--r--   0        0        0       38 2023-02-27 15:51:29.525721 envidat-utils-1.4.1/tests/__init__.py
+-rw-r--r--   0        0        0    22302 2023-05-03 16:04:39.418812 envidat-utils-1.4.1/tests/conftest.py
+-rw-r--r--   0        0        0      177 2023-02-27 15:51:29.525721 envidat-utils-1.4.1/tests/test_api.py
+-rw-r--r--   0        0        0    14075 2023-02-27 15:51:29.525721 envidat-utils-1.4.1/tests/test_bucket_io.py
+-rw-r--r--   0        0        0     5101 2023-05-03 16:04:39.418812 envidat-utils-1.4.1/tests/test_bucket_utils.py
+-rw-r--r--   0        0        0    16141 2023-05-03 16:04:39.418812 envidat-utils-1.4.1/tests/test_converters.py
+-rw-r--r--   0        0        0     3794 2023-05-03 16:04:39.418812 envidat-utils-1.4.1/tests/test_metadata.py
+-rw-r--r--   0        0        0     2728 1970-01-01 00:00:00.000000 envidat-utils-1.4.1/PKG-INFO
```

### Comparing `envidat-utils-1.4.0/CHANGELOG.md` & `envidat-utils-1.4.1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # CHANGELOG
 
+## 1.4.1 (2023-05-06)
+
+### Fix
+
+- dotenv debug mode function graceful failure
+
 ## 1.4.0 (2023-05-03)
 
 ### Feat
 
 - finish script datacite_updater_records.py
 - add function to update just some records in DataCite in datacite_updater.py
 - start working on new script to update some records in DataCite
```

### Comparing `envidat-utils-1.4.0/LICENCE` & `envidat-utils-1.4.1/LICENCE`

 * *Files identical despite different names*

### Comparing `envidat-utils-1.4.0/envidat/api/v1.py` & `envidat-utils-1.4.1/envidat/api/v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import os
 
 from envidat.utils import get_url, get_url_response, load_dotenv_if_in_debug_mode
 
 log = logging.getLogger(__name__)
 
 # Load config from environment variables
-load_dotenv_if_in_debug_mode(".env")
+load_dotenv_if_in_debug_mode()
 
 
 def get_metadata_list(
     host: str = "https://www.envidat.ch", sort_result: bool = None
 ) -> list:
     """Get package/metadata list from API.
```

### Comparing `envidat-utils-1.4.0/envidat/config/config_converters.json` & `envidat-utils-1.4.1/envidat/config/config_converters.json`

 * *Files identical despite different names*

### Comparing `envidat-utils-1.4.0/envidat/converters/bibtex_converter.py` & `envidat-utils-1.4.1/envidat/converters/bibtex_converter.py`

 * *Files identical despite different names*

### Comparing `envidat-utils-1.4.0/envidat/converters/datacite_converter.py` & `envidat-utils-1.4.1/envidat/converters/datacite_converter.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 from envidat.utils import get_url, load_dotenv_if_in_debug_mode
 
 log = getLogger(__name__)
 
 
 # Load config from environment variables
-load_dotenv_if_in_debug_mode(".env")
+load_dotenv_if_in_debug_mode()
 
 # TODO add return type hints to functions
 
 def convert_datacite(metadata_record: dict) -> str | None:
     """Generate XML formatted string in DataCite format.
 
     Note:
```

### Comparing `envidat-utils-1.4.0/envidat/converters/dcat_ap_converter.py` & `envidat-utils-1.4.1/envidat/converters/dcat_ap_converter.py`

 * *Files identical despite different names*

### Comparing `envidat-utils-1.4.0/envidat/converters/dif_converter.py` & `envidat-utils-1.4.1/envidat/converters/dif_converter.py`

 * *Files identical despite different names*

### Comparing `envidat-utils-1.4.0/envidat/converters/iso_converter.py` & `envidat-utils-1.4.1/envidat/converters/iso_converter.py`

 * *Files identical despite different names*

### Comparing `envidat-utils-1.4.0/envidat/converters/ris_converter.py` & `envidat-utils-1.4.1/envidat/converters/ris_converter.py`

 * *Files identical despite different names*

### Comparing `envidat-utils-1.4.0/envidat/converters/xml_converter.py` & `envidat-utils-1.4.1/envidat/converters/xml_converter.py`

 * *Files identical despite different names*

### Comparing `envidat-utils-1.4.0/envidat/doi/datacite_publisher.py` & `envidat-utils-1.4.1/envidat/doi/datacite_publisher.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from envidat.converters.datacite_converter import convert_datacite
 from envidat.utils import load_dotenv_if_in_debug_mode
 
 log = getLogger(__name__)
 
 # Load config from environment variables
-load_dotenv_if_in_debug_mode(".env")
+load_dotenv_if_in_debug_mode()
 
 
 # TODO review if DOIs should continue to be reserved in CKAN database!!!!
 
 # TODO note in documentation for config that environment variables with a hash
 #   must be enclosed in quotes
```

### Comparing `envidat-utils-1.4.0/envidat/doi/datacite_updater.py` & `envidat-utils-1.4.1/envidat/doi/datacite_updater.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 # TODO implement name of log file as command line argument, assign default name
 fileHandler = logging.FileHandler(filename="./logs/datacite_updater.log")
 fileHandler.setFormatter(logFileFormatter)
 fileHandler.setLevel(level=logging.INFO)
 log.addHandler(fileHandler)
 
 # Load config from environment variables
-load_dotenv_if_in_debug_mode(".env")
+load_dotenv_if_in_debug_mode()
 
 
 def datacite_update_all_records():
     """Updates existing DOIs for all EnviDat records on DataCite.
 
     Function converts all EnviDat records to DataCite Metadata Schema 4.4,
     for documentation: https://schema.datacite.org/meta/kernel-4.4/
```

### Comparing `envidat-utils-1.4.0/envidat/metadata.py` & `envidat-utils-1.4.1/envidat/metadata.py`

 * *Files identical despite different names*

### Comparing `envidat-utils-1.4.0/envidat/s3/bucket.py` & `envidat-utils-1.4.1/envidat/s3/bucket.py`

 * *Files identical despite different names*

### Comparing `envidat-utils-1.4.0/envidat/s3/exceptions.py` & `envidat-utils-1.4.1/envidat/s3/exceptions.py`

 * *Files identical despite different names*

### Comparing `envidat-utils-1.4.0/envidat/utils.py` & `envidat-utils-1.4.1/envidat/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,56 +18,72 @@
     Returns:
         bool: if a debug trace is present or not.
     """
     gettrace = getattr(sys, "gettrace", lambda: None)
     return gettrace() is not None
 
 
-def load_dotenv_if_in_debug_mode(env_file: Union[Path, str]) -> NoReturn:
+def _is_docker() -> bool:
+    """Check to see if running in a docker container.
+
+    Returns:
+    -------
+        bool: if a docker related components present on filesystem.
+    """
+    path = "/proc/self/cgroup"
+    return (
+        os.path.exists("/.dockerenv")
+        or os.path.isfile(path)
+        and any("docker" in line for line in open(path))
+    )
+
+
+def load_dotenv_if_in_debug_mode(
+    env_file: Union[Path, str] = os.getenv("DOTENV_PATH", default=".env")
+) -> NoReturn:
     """Load secret .env variables from repo for debugging.
 
     Args:
         env_file (Union[Path, str]): String or Path like object pointer to
             secret dot env file to read.
     """
     if not _debugger_is_active():
         return
 
+    is_docker_from_env = os.getenv("IS_DOCKER", default=False)
+    if _is_docker() or is_docker_from_env:
+        return
+
     try:
         from dotenv import load_dotenv
     except ImportError as e:
         log.error(
             """
             Unable to import dotenv.
             Note: The logger should be invoked after reading the dotenv file
             so that the debug level is by the environment.
             """
         )
         log.error(e)
-        raise ImportError from e(
-            """
-            Unable to import dotenv, is python-dotenv installed?
-            Try installing this package using pip install envidat[dotenv].
-            """
-        )
 
     secret_env = Path(env_file)
     if not secret_env.is_file():
         log.error(
             """
             Attempted to import dotenv, but the file does not exist.
             Note: The logger should be invoked after reading the dotenv file
             so that the debug level is by the environment.
             """
         )
-        raise FileNotFoundError from None(
-            f"Attempted to import dotenv, but the file does not exist: {env_file}"
-        )
     else:
-        load_dotenv(secret_env)
+        try:
+            load_dotenv(secret_env)
+        except Exception as e:
+            log.error(e)
+            log.error(f"Failed to load dotenv file: {secret_env}")
 
 
 def get_logger() -> logging.basicConfig:
     """Set logger parameters with log level from environment.
 
     Note:
         Defaults to DEBUG level, unless specified by LOG_LEVEL env var.
@@ -92,15 +108,15 @@
     api_host: str,
     api_path: str,
     query: dict | None = None,
     api_key: str | None = None,
     status_code: int = 200,
 ) -> dict | None:
     """Get response JSON from EnviDat."""
-    load_dotenv_if_in_debug_mode(".env")
+    load_dotenv_if_in_debug_mode()
 
     key = None
     # Extract environment variables needed to call API URL
     try:
         host = os.environ(api_host)
         path = os.environ(api_path)
         if api_key:
```

### Comparing `envidat-utils-1.4.0/pyproject.toml` & `envidat-utils-1.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 ]
 classifiers = [
     "Topic :: Utilities",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.10",
 ]
-version = "1.4.0"
+version = "1.4.1"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 homepage = "https://www.envidat.ch"
 documentation = "https://envidat.gitlab-pages.wsl.ch/envidat-python-utils"
@@ -71,15 +71,15 @@
     "mkdocs>=1.1",
     "mkdocs-material>=7.3",
     "mkgendocs>=0.9.0",
 ]
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "1.4.0"
+version = "1.4.1"
 version_files = [
     "pyproject.toml:version",
     "envidat/__version__.py",
 ]
 
 [tool.pytest.ini_options]
 addopts = "-ra -q"
```

### Comparing `envidat-utils-1.4.0/tests/conftest.py` & `envidat-utils-1.4.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `envidat-utils-1.4.0/tests/test_bucket_io.py` & `envidat-utils-1.4.1/tests/test_bucket_io.py`

 * *Files identical despite different names*

### Comparing `envidat-utils-1.4.0/tests/test_bucket_utils.py` & `envidat-utils-1.4.1/tests/test_bucket_utils.py`

 * *Files identical despite different names*

### Comparing `envidat-utils-1.4.0/tests/test_converters.py` & `envidat-utils-1.4.1/tests/test_converters.py`

 * *Files identical despite different names*

### Comparing `envidat-utils-1.4.0/tests/test_metadata.py` & `envidat-utils-1.4.1/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `envidat-utils-1.4.0/PKG-INFO` & `envidat-utils-1.4.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: envidat-utils
-Version: 1.4.0
+Version: 1.4.1
 Summary: Utilities in Python for the WSL EnviDat project.
 License: MIT
 Keywords: envidat,s3,ckan,wsl
 Author-email: Sam Woodcock <samuel.woodcock@wsl.ch>,Rebecca Kurup Buchholz <rebecca.kurup@wsl.ch>
 Requires-Python: >=3.9,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -62,7 +62,20 @@
 
 ```python
 from envidat.utils import get_logger
 from envidat.s3 import Bucket
 from envidat.api.v1 import get_package_list
 ```
 
+## Config
+
+Environment variables:
+
+- LOG_LEVEL: Logging level, default INFO
+- DOTENV_PATH: Path to dotenv file if in debug mode, default=.env.
+- API_URL: URL root for the API to call, default=https://www.envidat.ch
+- TEMP_DIR: Temporary path for S3 downloads, default=/tmp
+- AWS_ENDPOINT: For S3.
+- AWS_REGION: For S3.
+- AWS_ACCESS_KEY: For S3.
+- AWS_SECRET_KEY: For S3.
+
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: envidat-utils Version: 1.4.0 Summary: Utilities in
+Metadata-Version: 2.1 Name: envidat-utils Version: 1.4.1 Summary: Utilities in
 Python for the WSL EnviDat project. License: MIT Keywords: envidat,s3,ckan,wsl
 Author-email: Sam Woodcock
 woodcock@wsl.ch>,Rebecca Kurup Buchholz
 kurup@wsl.ch> Requires-Python: >=3.9,<3.11 Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Topic :: Utilities Provides-Extra: dotenv Project-URL: documentation, https://
 envidat.gitlab-pages.wsl.ch/envidat-python-utils Project-URL: homepage, https:/
@@ -15,8 +15,13 @@
 --- **Documentation**: https://envidat.gitlab-pages.wsl.ch/envidat-python-
 utils/ **Source Code**: https://gitlabext.wsl.ch/EnviDat/envidat-python-utils -
 -- ## PyPi Package - This package aims to speed up EnviDat python workflows -
 Contains: - Backend API function wrappers. - S3 bucket class, with configurable
 endpoint. - Utils to use in multiple projects (e.g. consistent logger setup).
 ## Install ```bash $ pip install -U pip $ pip install envidat-utils ``` ##
 Usage ```python from envidat.utils import get_logger from envidat.s3 import
-Bucket from envidat.api.v1 import get_package_list ```
+Bucket from envidat.api.v1 import get_package_list ``` ## Config Environment
+variables: - LOG_LEVEL: Logging level, default INFO - DOTENV_PATH: Path to
+dotenv file if in debug mode, default=.env. - API_URL: URL root for the API to
+call, default=https://www.envidat.ch - TEMP_DIR: Temporary path for S3
+downloads, default=/tmp - AWS_ENDPOINT: For S3. - AWS_REGION: For S3. -
+AWS_ACCESS_KEY: For S3. - AWS_SECRET_KEY: For S3.
```

