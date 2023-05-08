# Comparing `tmp/pywry-0.5.2.tar.gz` & `tmp/pywry-0.5.3.tar.gz`

## Comparing `pywry-0.5.2.tar` & `pywry-0.5.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      883 1970-01-01 00:00:00.000000 pywry-0.5.2/pyproject.toml
--rw-r--r--   0        0        0      733 1970-01-01 00:00:00.000000 pywry-0.5.2/rust_src/pywry/Cargo.toml
--rw-r--r--   0     1001      123     1063 2023-05-07 21:47:45.000000 pywry-0.5.2/rust_src/pywry/LICENSE
--rw-r--r--   0     1001      123     2678 2023-05-07 21:47:45.000000 pywry-0.5.2/rust_src/pywry/README.md
--rw-r--r--   0     1001      123     2149 2023-05-07 21:47:45.000000 pywry-0.5.2/rust_src/pywry/src/constants.rs
--rw-r--r--   0     1001      123     1223 2023-05-07 21:47:45.000000 pywry-0.5.2/rust_src/pywry/src/lib.rs
--rw-r--r--   0     1001      123     1085 2023-05-07 21:47:45.000000 pywry-0.5.2/rust_src/pywry/src/pipe.rs
--rw-r--r--   0     1001      123     4737 2023-05-07 21:47:45.000000 pywry-0.5.2/rust_src/pywry/src/structs.rs
--rw-r--r--   0     1001      123    22038 2023-05-07 21:47:45.000000 pywry-0.5.2/rust_src/pywry/src/window.rs
--rw-r--r--   0     1001      123    60354 2023-05-07 21:47:45.000000 pywry-0.5.2/Cargo.lock
--rw-r--r--   0     1001      123      985 2023-05-07 21:47:45.000000 pywry-0.5.2/python/pywry/backend.py
--rw-r--r--   0     1001      123        0 2023-05-07 21:47:45.000000 pywry-0.5.2/python/pywry/py.typed
--rw-r--r--   0     1001      123      154 2023-05-07 21:47:45.000000 pywry-0.5.2/python/pywry/pywry.pyi
--rw-r--r--   0     1001      123    12959 2023-05-07 21:47:45.000000 pywry-0.5.2/python/pywry/core.py
--rw-r--r--   0     1001      123      180 2023-05-07 21:47:45.000000 pywry-0.5.2/python/pywry/__init__.py
--rw-r--r--   0     1001      123      733 2023-05-07 21:47:45.000000 pywry-0.5.2/Cargo.toml
--rw-r--r--   0     1001      123     2149 2023-05-07 21:47:45.000000 pywry-0.5.2/src/constants.rs
--rw-r--r--   0     1001      123     1223 2023-05-07 21:47:45.000000 pywry-0.5.2/src/lib.rs
--rw-r--r--   0     1001      123     1085 2023-05-07 21:47:45.000000 pywry-0.5.2/src/pipe.rs
--rw-r--r--   0     1001      123     4737 2023-05-07 21:47:45.000000 pywry-0.5.2/src/structs.rs
--rw-r--r--   0     1001      123    22038 2023-05-07 21:47:45.000000 pywry-0.5.2/src/window.rs
--rw-r--r--   0        0        0     3280 1970-01-01 00:00:00.000000 pywry-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0      883 1970-01-01 00:00:00.000000 pywry-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0      733 1970-01-01 00:00:00.000000 pywry-0.5.3/rust_src/pywry/Cargo.toml
+-rw-r--r--   0     1001      123     1063 2023-05-08 13:47:48.000000 pywry-0.5.3/rust_src/pywry/LICENSE
+-rw-r--r--   0     1001      123     4870 2023-05-08 13:47:48.000000 pywry-0.5.3/rust_src/pywry/README.md
+-rw-r--r--   0     1001      123     2149 2023-05-08 13:47:48.000000 pywry-0.5.3/rust_src/pywry/src/constants.rs
+-rw-r--r--   0     1001      123     1223 2023-05-08 13:47:48.000000 pywry-0.5.3/rust_src/pywry/src/lib.rs
+-rw-r--r--   0     1001      123     1085 2023-05-08 13:47:48.000000 pywry-0.5.3/rust_src/pywry/src/pipe.rs
+-rw-r--r--   0     1001      123     4737 2023-05-08 13:47:48.000000 pywry-0.5.3/rust_src/pywry/src/structs.rs
+-rw-r--r--   0     1001      123    22038 2023-05-08 13:47:48.000000 pywry-0.5.3/rust_src/pywry/src/window.rs
+-rw-r--r--   0     1001      123    60354 2023-05-08 13:47:48.000000 pywry-0.5.3/Cargo.lock
+-rw-r--r--   0     1001      123      985 2023-05-08 13:47:48.000000 pywry-0.5.3/python/pywry/backend.py
+-rw-r--r--   0     1001      123        0 2023-05-08 13:47:48.000000 pywry-0.5.3/python/pywry/py.typed
+-rw-r--r--   0     1001      123      154 2023-05-08 13:47:48.000000 pywry-0.5.3/python/pywry/pywry.pyi
+-rw-r--r--   0     1001      123    12974 2023-05-08 13:47:48.000000 pywry-0.5.3/python/pywry/core.py
+-rw-r--r--   0     1001      123      180 2023-05-08 13:47:48.000000 pywry-0.5.3/python/pywry/__init__.py
+-rw-r--r--   0     1001      123      733 2023-05-08 13:47:48.000000 pywry-0.5.3/Cargo.toml
+-rw-r--r--   0     1001      123     2149 2023-05-08 13:47:48.000000 pywry-0.5.3/src/constants.rs
+-rw-r--r--   0     1001      123     1223 2023-05-08 13:47:48.000000 pywry-0.5.3/src/lib.rs
+-rw-r--r--   0     1001      123     1085 2023-05-08 13:47:48.000000 pywry-0.5.3/src/pipe.rs
+-rw-r--r--   0     1001      123     4737 2023-05-08 13:47:48.000000 pywry-0.5.3/src/structs.rs
+-rw-r--r--   0     1001      123    22038 2023-05-08 13:47:48.000000 pywry-0.5.3/src/window.rs
+-rw-r--r--   0        0        0     5472 1970-01-01 00:00:00.000000 pywry-0.5.3/PKG-INFO
```

### Comparing `pywry-0.5.2/pyproject.toml` & `pywry-0.5.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pywry"
-version = "0.5.2"
+version = "0.5.3"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "Operating System :: POSIX",
     "Operating System :: Microsoft :: Windows",
```

### Comparing `pywry-0.5.2/rust_src/pywry/Cargo.toml` & `pywry-0.5.3/rust_src/pywry/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "pywry"
-version = "0.5.2"
+version = "0.5.3"
 edition = "2021"
 include = ["src/", "Cargo.toml", "LICENSE", "README.md"]
 
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "pywry"
```

### Comparing `pywry-0.5.2/rust_src/pywry/LICENSE` & `pywry-0.5.3/rust_src/pywry/LICENSE`

 * *Files identical despite different names*

### Comparing `pywry-0.5.2/rust_src/pywry/src/constants.rs` & `pywry-0.5.3/rust_src/pywry/src/constants.rs`

 * *Files identical despite different names*

### Comparing `pywry-0.5.2/rust_src/pywry/src/lib.rs` & `pywry-0.5.3/rust_src/pywry/src/lib.rs`

 * *Files identical despite different names*

### Comparing `pywry-0.5.2/rust_src/pywry/src/pipe.rs` & `pywry-0.5.3/rust_src/pywry/src/pipe.rs`

 * *Files identical despite different names*

### Comparing `pywry-0.5.2/rust_src/pywry/src/structs.rs` & `pywry-0.5.3/rust_src/pywry/src/structs.rs`

 * *Files identical despite different names*

### Comparing `pywry-0.5.2/rust_src/pywry/src/window.rs` & `pywry-0.5.3/rust_src/pywry/src/window.rs`

 * *Files identical despite different names*

### Comparing `pywry-0.5.2/Cargo.lock` & `pywry-0.5.3/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1481,15 +1481,15 @@
 checksum = "a915bd72824962bf190bbd3e8a044cccb695d1409f73ff5493712eda5136c7a8"
 dependencies = [
  "cc",
 ]
 
 [[package]]
 name = "pywry"
-version = "0.5.2"
+version = "0.5.3"
 dependencies = [
  "image",
  "mime_guess",
  "open",
  "pyo3",
  "serde",
  "serde_json",
```

### Comparing `pywry-0.5.2/python/pywry/backend.py` & `pywry-0.5.3/python/pywry/backend.py`

 * *Files identical despite different names*

### Comparing `pywry-0.5.2/python/pywry/core.py` & `pywry-0.5.3/python/pywry/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,22 +23,22 @@
     TimeoutError,
     ConnectionResetError,
 )
 
 
 ACCEPTED_KEYS_TYPES = {
     "html_str": str,
-    "html_path": Union[str, Path],
+    "html_path": (str, Path),
     "title": str,
-    "icon": Union[str, Path],
-    "json_data": Union[dict, str],
+    "icon": (str, Path),
+    "json_data": (dict, str),
     "height": int,
     "width": int,
-    "download_path": Union[str, Path],
-    "export_image": Union[str, Path],
+    "download_path": (str, Path),
+    "export_image": (str, Path),
 }
 
 
 class BackendFailedToStart(Exception):
     """Raised when the backend fails to start"""
 
     def __init__(self, message: str):
@@ -176,17 +176,17 @@
                     raise ValueError(f"Invalid key: {key}")
                 if not isinstance(value, ACCEPTED_KEYS_TYPES[key]):
                     raise TypeError(
                         f"Invalid type for {key}. "
                         f"Expected {ACCEPTED_KEYS_TYPES[key]}, got {type(value)}"
                     )
                 if isinstance(value, Path):
-                    if not value.exists():
+                    if value.is_file() and not value.exists() and key != "export_image":
                         raise FileNotFoundError(value)
-                    value = value.resolve().as_posix()
+                    value = str(value.resolve())
             except Exception:
                 self.print_debug()
                 continue
 
             output[key] = value
 
         return output
```

### Comparing `pywry-0.5.2/Cargo.toml` & `pywry-0.5.3/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "pywry"
-version = "0.5.2"
+version = "0.5.3"
 edition = "2021"
 include = ["src/", "Cargo.toml", "LICENSE", "README.md"]
 
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "pywry"
```

### Comparing `pywry-0.5.2/src/constants.rs` & `pywry-0.5.3/src/constants.rs`

 * *Files identical despite different names*

### Comparing `pywry-0.5.2/src/lib.rs` & `pywry-0.5.3/src/lib.rs`

 * *Files identical despite different names*

### Comparing `pywry-0.5.2/src/pipe.rs` & `pywry-0.5.3/src/pipe.rs`

 * *Files identical despite different names*

### Comparing `pywry-0.5.2/src/structs.rs` & `pywry-0.5.3/src/structs.rs`

 * *Files identical despite different names*

### Comparing `pywry-0.5.2/src/window.rs` & `pywry-0.5.3/src/window.rs`

 * *Files identical despite different names*

