# Comparing `tmp/conda_package_streaming-0.7.0.tar.gz` & `tmp/conda_package_streaming-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conda_package_streaming-0.7.0.tar", last modified: Sat Nov 19 20:24:31 2022, max compression
+gzip compressed data, was "conda_package_streaming-0.8.0.tar", last modified: Mon May  8 18:40:36 2023, max compression
```

## Comparing `conda_package_streaming-0.7.0.tar` & `conda_package_streaming-0.8.0.tar`

### file list

```diff
@@ -1,40 +1,12 @@
--rw-r--r--   0        0        0       31 2022-11-18 18:29:35.281136 conda_package_streaming-0.7.0/.flake8
--rw-r--r--   0        0        0      458 2022-11-18 18:29:35.281347 conda_package_streaming-0.7.0/.github/workflows/main.yml
--rw-r--r--   0        0        0     1045 2022-11-18 18:29:35.281461 conda_package_streaming-0.7.0/.github/workflows/sphinx.yml
--rw-r--r--   0        0        0       77 2022-11-18 18:29:35.281545 conda_package_streaming-0.7.0/.gitignore
--rw-r--r--   0        0        0      945 2022-11-18 18:29:35.281673 conda_package_streaming-0.7.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2670 2022-11-18 18:29:35.281806 conda_package_streaming-0.7.0/LICENSE
--rw-r--r--   0        0        0      678 2022-11-18 18:29:35.281933 conda_package_streaming-0.7.0/Makefile
--rw-r--r--   0        0        0     2722 2022-11-18 18:29:35.282042 conda_package_streaming-0.7.0/README.md
--rw-r--r--   0        0        0     1201 2022-11-18 18:29:35.282220 conda_package_streaming-0.7.0/conda.recipe/meta.yaml
--rw-r--r--   0        0        0       22 2022-11-19 20:24:25.721321 conda_package_streaming-0.7.0/conda_package_streaming/__init__.py
--rw-r--r--   0        0        0      677 2022-11-18 18:29:35.282511 conda_package_streaming-0.7.0/conda_package_streaming/exceptions.py
--rw-r--r--   0        0        0     2539 2022-11-19 20:24:25.721699 conda_package_streaming-0.7.0/conda_package_streaming/extract.py
--rw-r--r--   0        0        0     9450 2022-11-18 18:29:35.282755 conda_package_streaming-0.7.0/conda_package_streaming/lazy_wheel.py
--rw-r--r--   0        0        0     3733 2022-11-19 20:24:25.722002 conda_package_streaming-0.7.0/conda_package_streaming/package_streaming.py
--rw-r--r--   0        0        0     2286 2022-11-18 18:29:35.282962 conda_package_streaming-0.7.0/conda_package_streaming/s3.py
--rw-r--r--   0        0        0     4733 2022-11-19 20:24:25.722308 conda_package_streaming-0.7.0/conda_package_streaming/transmute.py
--rw-r--r--   0        0        0     2462 2022-11-18 18:29:35.283188 conda_package_streaming-0.7.0/conda_package_streaming/url.py
--rw-r--r--   0        0        0     1879 2022-11-18 18:29:35.283411 conda_package_streaming-0.7.0/docs/conf.py
--rw-r--r--   0        0        0      176 2022-11-18 18:29:35.283522 conda_package_streaming-0.7.0/docs/extract.rst
--rw-r--r--   0        0        0     1368 2022-11-19 20:24:25.722674 conda_package_streaming-0.7.0/docs/index.md
--rw-r--r--   0        0        0      798 2022-11-18 18:29:35.283731 conda_package_streaming-0.7.0/docs/lazy_wheel.md
--rw-r--r--   0        0        0     2724 2022-11-18 18:29:35.283929 conda_package_streaming-0.7.0/docs/modules.md
--rw-r--r--   0        0        0      165 2022-11-18 18:29:35.284023 conda_package_streaming-0.7.0/docs/package_streaming.rst
--rw-r--r--   0        0        0      342 2022-11-18 18:29:35.284111 conda_package_streaming-0.7.0/docs/s3.md
--rw-r--r--   0        0        0      139 2022-11-18 18:29:35.284205 conda_package_streaming-0.7.0/docs/transmute.rst
--rw-r--r--   0        0        0      133 2022-11-18 18:29:35.284277 conda_package_streaming-0.7.0/docs/url.rst
--rw-r--r--   0        0        0      804 2022-11-18 18:29:35.284355 conda_package_streaming-0.7.0/make.bat
--rw-r--r--   0        0        0      225 2022-11-18 18:29:35.284469 conda_package_streaming-0.7.0/noxfile.py
--rw-r--r--   0        0        0     1254 2022-11-19 20:24:25.723027 conda_package_streaming-0.7.0/pyproject.toml
--rw-r--r--   0        0        0      127 2022-11-18 18:29:35.284654 conda_package_streaming-0.7.0/renovate.json
--rw-r--r--   0        0        0      157 2022-11-18 18:29:35.284742 conda_package_streaming-0.7.0/requirements.txt
--rw-r--r--   0        0        0      477 2022-11-18 18:29:35.284950 conda_package_streaming-0.7.0/tests/conftest.py
--rw-r--r--   0        0        0     2473 2022-11-18 18:29:35.285065 conda_package_streaming-0.7.0/tests/server.py
--rw-r--r--   0        0        0     1531 2022-11-18 18:29:35.285194 conda_package_streaming-0.7.0/tests/test_degraded.py
--rw-r--r--   0        0        0     2847 2022-11-18 18:29:35.285326 conda_package_streaming-0.7.0/tests/test_extract.py
--rw-r--r--   0        0        0     1152 2022-11-18 18:29:35.285421 conda_package_streaming-0.7.0/tests/test_s3.py
--rw-r--r--   0        0        0     1121 2022-11-19 20:24:25.723400 conda_package_streaming-0.7.0/tests/test_streaming.py
--rw-r--r--   0        0        0     3136 2022-11-18 18:29:35.285619 conda_package_streaming-0.7.0/tests/test_transmute.py
--rw-r--r--   0        0        0     4962 2022-11-18 18:29:35.285745 conda_package_streaming-0.7.0/tests/test_url.py
--rw-r--r--   0        0        0     3932 1970-01-01 00:00:00.000000 conda_package_streaming-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     2670 2023-05-08 18:38:19.008597 conda_package_streaming-0.8.0/LICENSE
+-rw-r--r--   0        0        0     3165 2023-05-08 18:38:19.008779 conda_package_streaming-0.8.0/README.md
+-rw-r--r--   0        0        0       22 2023-05-08 18:38:19.009078 conda_package_streaming-0.8.0/conda_package_streaming/__init__.py
+-rw-r--r--   0        0        0      677 2023-05-08 18:38:19.009179 conda_package_streaming-0.8.0/conda_package_streaming/exceptions.py
+-rw-r--r--   0        0        0     2538 2023-05-08 18:38:19.009288 conda_package_streaming-0.8.0/conda_package_streaming/extract.py
+-rw-r--r--   0        0        0     9449 2023-05-08 18:38:19.009415 conda_package_streaming-0.8.0/conda_package_streaming/lazy_wheel.py
+-rw-r--r--   0        0        0     3733 2023-05-08 18:38:19.009640 conda_package_streaming-0.8.0/conda_package_streaming/package_streaming.py
+-rw-r--r--   0        0        0     2286 2023-05-08 18:38:19.009804 conda_package_streaming-0.8.0/conda_package_streaming/s3.py
+-rw-r--r--   0        0        0     5663 2023-05-08 18:38:19.009938 conda_package_streaming-0.8.0/conda_package_streaming/transmute.py
+-rw-r--r--   0        0        0     2707 2023-05-08 18:38:19.010056 conda_package_streaming-0.8.0/conda_package_streaming/url.py
+-rw-r--r--   0        0        0     1314 2023-05-08 18:38:19.011624 conda_package_streaming-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     4491 1970-01-01 00:00:00.000000 conda_package_streaming-0.8.0/PKG-INFO
```

### Comparing `conda_package_streaming-0.7.0/LICENSE` & `conda_package_streaming-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `conda_package_streaming-0.7.0/README.md` & `conda_package_streaming-0.8.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # conda-package-streaming
 
+[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/conda/conda-package-streaming/main.svg)](https://results.pre-commit.ci/latest/github/conda/conda-package-streaming/main)
+
+An efficient library to read from new and old format .conda and .tar.bz2 conda
+packages.
+
 Download conda metadata from packages without transferring entire file. Get
 metadata from local `.tar.bz2` packages without reading entire files.
 
 Uses enhanced pip `lazy_wheel` to fetch a file out of `.conda` with no more than
 3 range requests, but usually 2.
 
 Uses `tar = tarfile.open(fileobj=...)` to stream remote `.tar.bz2`. Closes the
@@ -60,14 +65,18 @@
 with closing(conda):
     for tar, member in stream_conda_component(filename, conda, component="info"):
         if member.name == "info/index.json":
             index_json = json.load(tar.extractfile(member))
             break
 ```
 
+If you need the entire package, download it first and use the file-based APIs.
+The URL-based APIs are more efficient if you only need to access package
+metadata.
+
 # Package goals
 
 * Extract conda packages (both formats)
 * Easy to install from pypi or conda
 * Do the least amount of I/O possible (no temporary files, transfer partial packages)
 * Open files from the network / standard HTTP / s3
```

### Comparing `conda_package_streaming-0.7.0/conda_package_streaming/exceptions.py` & `conda_package_streaming-0.8.0/conda_package_streaming/exceptions.py`

 * *Files identical despite different names*

### Comparing `conda_package_streaming-0.7.0/conda_package_streaming/extract.py` & `conda_package_streaming-0.8.0/conda_package_streaming/extract.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,14 @@
 
     def is_within_dest_dir(name):
         abs_target = os.path.realpath(os.path.join(dest_dir, name))
         prefix = os.path.commonpath((dest_dir, abs_target))
         return prefix == dest_dir
 
     for tar_file, _ in stream:
-
         # careful not to seek backwards
         def checked_members():
             # from conda_package_handling
             for member in tar_file:
                 if not is_within_dest_dir(member.name):
                     raise exceptions.SafetyError(f"contains unsafe path: {member.name}")
                 yield member
```

### Comparing `conda_package_streaming-0.7.0/conda_package_streaming/lazy_wheel.py` & `conda_package_streaming-0.8.0/conda_package_streaming/lazy_wheel.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,14 @@
     supported by the server, raise HTTPRangeRequestUnsupported
     during initialization.
     """
 
     def __init__(
         self, url: str, session: Session, chunk_size: int = CONTENT_CHUNK_SIZE
     ) -> None:
-
         # if CONTENT_CHUNK_SIZE is bigger than the file:
         # In [8]: response.headers["Content-Range"]
         # Out[8]: 'bytes 0-3133374/3133375'
 
         self._request_count = 0
 
         self._session, self._url, self._chunk_size = session, url, chunk_size
```

### Comparing `conda_package_streaming-0.7.0/conda_package_streaming/package_streaming.py` & `conda_package_streaming-0.8.0/conda_package_streaming/package_streaming.py`

 * *Files identical despite different names*

### Comparing `conda_package_streaming-0.7.0/conda_package_streaming/s3.py` & `conda_package_streaming-0.8.0/conda_package_streaming/s3.py`

 * *Files identical despite different names*

### Comparing `conda_package_streaming-0.7.0/conda_package_streaming/transmute.py` & `conda_package_streaming-0.8.0/conda_package_streaming/transmute.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,111 +9,133 @@
 
 Conda packages created this way will also have `info-*` as the last element in
 the `ZipFile`, instead of the first for normal conda packages.
 """
 
 from __future__ import annotations
 
-import io
 import json
 import os
+import shutil
 import tarfile
+import tempfile
 import zipfile
+from pathlib import Path
 from typing import Callable
 
 import zstandard
 
 # streams everything in .tar.bz2 mode
 from .package_streaming import CondaComponent, stream_conda_component
 
-# increase to reduce speed and increase compression (22 = conda's default)
-ZSTD_COMPRESS_LEVEL = 22
+# increase to reduce speed and increase compression (levels above 19 use much
+# more memory)
+ZSTD_COMPRESS_LEVEL = 19
 # increase to reduce compression and increase speed
 ZSTD_COMPRESS_THREADS = 1
 
+CONDA_PACKAGE_FORMAT_VERSION = 2
+
 
 def transmute(
     package,
     path,
     *,
     compressor: Callable[
         [], zstandard.ZstdCompressor
     ] = lambda: zstandard.ZstdCompressor(
         level=ZSTD_COMPRESS_LEVEL, threads=ZSTD_COMPRESS_THREADS
     ),
     is_info: Callable[[str], bool] = lambda filename: filename.startswith("info/"),
-):
+) -> Path:
     """
     Convert .tar.bz2 conda :package to .conda-format under path.
 
     :param package: path to .tar.bz2 conda package
     :param path: destination path for transmuted .conda package
     :param compressor: A function that creates instances of
         ``zstandard.ZstdCompressor()`` to override defaults.
     :param is_info: A function that returns True if a file belongs in the
         ``info`` component of a `.conda` package.  ``conda-package-handling``
         (not this package ``conda-package-streaming``) uses a set of regular
         expressions to keep expected items in the info- component, while other
         items starting with ``info/`` wind up in the pkg- component.
+
+    :return: Path to transmuted package.
     """
     assert package.endswith(".tar.bz2"), "can only convert .tar.bz2 to .conda"
     assert os.path.isdir(path)
     file_id = os.path.basename(package)[: -len(".tar.bz2")]
+    output_path = Path(path, f"{file_id}.conda")
 
-    # x to not append to existing
-    with zipfile.ZipFile(
-        os.path.join(path, f"{file_id}.conda"), "x", compresslevel=zipfile.ZIP_STORED
-    ) as conda_file:
-
-        info_compress = compressor()
-        data_compress = compressor()
-
-        # in theory, info_tar could grow uncomfortably big, in which case we would
-        # rather swap it to disk
-        info_io = io.BytesIO()
-        info_stream = info_compress.stream_writer(info_io, closefd=False)
-        info_tar = tarfile.TarFile(fileobj=info_stream, mode="w")
-
-        conda_file.writestr(
-            "metadata.json", json.dumps({"conda_pkg_format_version": 2})
-        )
-
-        with conda_file.open(f"pkg-{file_id}.tar.zst", "w") as pkg_file:
-            pkg_stream = data_compress.stream_writer(pkg_file, closefd=False)
-            pkg_tar = tarfile.TarFile(fileobj=pkg_stream, mode="w")
-
+    with tempfile.SpooledTemporaryFile() as info_file, tempfile.SpooledTemporaryFile() as pkg_file:
+        with tarfile.TarFile(fileobj=info_file, mode="w") as info_tar, tarfile.TarFile(
+            fileobj=pkg_file, mode="w"
+        ) as pkg_tar:
+            # If we wanted to compress these at a low setting to save temporary
+            # space, we could insert a file object that counts bytes written in
+            # front of a zstd (level between 1..3) compressor.
             stream = iter(stream_conda_component(package))
             for tar, member in stream:
                 tar_get = info_tar if is_info(member.name) else pkg_tar
                 if member.isfile():
                     tar_get.addfile(member, tar.extractfile(member))
                 else:
                     tar_get.addfile(member)
 
+            info_tar.close()
             pkg_tar.close()
-            pkg_stream.close()
 
-            info_tar.close()
-            info_stream.close()
+            info_size = info_file.tell()
+            pkg_size = pkg_file.tell()
+
+            info_file.seek(0)
+            pkg_file.seek(0)
 
-        with conda_file.open(f"info-{file_id}.tar.zst", "w") as info_file:
-            info_file.write(info_io.getvalue())
+        with zipfile.ZipFile(
+            output_path,
+            "x",  # x to not append to existing
+            compresslevel=zipfile.ZIP_STORED,
+        ) as conda_file:
+            # Use a maximum of one Zstd compressor, stream_writer at a time to save memory.
+            data_compress = compressor()
+
+            pkg_metadata = {"conda_pkg_format_version": CONDA_PACKAGE_FORMAT_VERSION}
+            conda_file.writestr("metadata.json", json.dumps(pkg_metadata))
+
+            with conda_file.open(
+                f"pkg-{file_id}.tar.zst", "w"
+            ) as pkg_file_zip, data_compress.stream_writer(
+                pkg_file_zip, size=pkg_size, closefd=False
+            ) as pkg_stream:
+                shutil.copyfileobj(pkg_file._file, pkg_stream)
+
+            with conda_file.open(
+                f"info-{file_id}.tar.zst", "w"
+            ) as info_file_zip, data_compress.stream_writer(
+                info_file_zip, size=info_size, closefd=False
+            ) as info_stream:
+                shutil.copyfileobj(info_file._file, info_stream)
+
+    return output_path
 
 
 def transmute_tar_bz2(
-    package,
+    package: str,
     path,
-):
+) -> Path:
     """
     Convert .conda :package to .tar.bz2 format under path.
 
     Can recompress .tar.bz2 packages.
 
     :param package: path to `.conda` or `.tar.bz2` package.
     :param path: destination path for transmuted package.
+
+    :return: Path to transmuted package.
     """
     assert package.endswith((".tar.bz2", ".conda")), "Unknown extension"
     assert os.path.isdir(path)
 
     incoming_format = ".conda" if package.endswith(".conda") else ".tar.bz2"
 
     file_id = os.path.basename(package)[: -len(incoming_format)]
@@ -121,17 +143,19 @@
     if incoming_format == ".conda":
         # .tar.bz2 MUST place info/ first.
         components = [CondaComponent.info, CondaComponent.pkg]
     else:
         # .tar.bz2 doesn't filter by component
         components = [CondaComponent.pkg]
 
-    with open(package, "rb") as fileobj, tarfile.open(
-        os.path.join(path, f"{file_id}.tar.bz2"), "x:bz2"
-    ) as pkg_tar:
+    output_path = Path(path, f"{file_id}.tar.bz2")
+
+    with open(package, "rb") as fileobj, tarfile.open(output_path, "x:bz2") as pkg_tar:
         for component in components:
             stream = iter(stream_conda_component(package, fileobj, component=component))
             for tar, member in stream:
                 if member.isfile():
                     pkg_tar.addfile(member, tar.extractfile(member))
                 else:
                     pkg_tar.addfile(member)
+
+    return output_path
```

### Comparing `conda_package_streaming-0.7.0/conda_package_streaming/url.py` & `conda_package_streaming-0.8.0/conda_package_streaming/url.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 """
 Fetch metadata from remote .conda or .tar.bz2 package.
 
 Try to fetch less than the whole file if possible.
+
+This module should only be used to make *partial* reads against a remote
+package, typically just the ``info`` portion. If a full ``.conda`` format
+package is needed, it is more efficient to download locally first and then use
+the file-based API.
 """
 
 import logging
 import sys
 import urllib.parse
 from pathlib import Path
 
@@ -28,15 +33,15 @@
 def extract_conda_info(url, destdir, checklist=METADATA_CHECKLIST, session=session):
     """
     Extract info/index.json and info/recipe/meta.yaml from url to destdir; close
     url as soon as those files are found.
     """
     checklist = set(checklist)
     stream = stream_conda_info(url, session=session)
-    for (tar, member) in stream:
+    for tar, member in stream:
         if member.name in checklist:
             tar.extract(member, destdir)
             checklist.remove(member.name)
         if not checklist:
             stream.close()
             # next iteraton of for loop raises GeneratorExit in stream
```

### Comparing `conda_package_streaming-0.7.0/pyproject.toml` & `conda_package_streaming-0.8.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "conda_package_streaming"
 authors = [
   { name = "Anaconda, Inc. & Contributors", email = "conda@continuum.io" },
 ]
-description = "Download metadata from conda packages without transferring entire file."
+description = "An efficient library to read from new and old format .conda and .tar.bz2 conda packages."
 license = { file = "LICENSE" }
 readme = "README.md"
 classifiers = [
   "License :: OSI Approved :: BSD License",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
@@ -30,14 +30,16 @@
 test = [
   "pytest >=7",
   "pytest-cov",
   "pytest-mock",
   "boto3",
   "boto3-stubs[essential]",
   "bottle",
+  "conda",
+  "conda-package-handling >=2",
 ]
 docs = ["furo", "sphinx", "myst-parser", "mdit-py-plugins>=0.3.0"]
 
 [project.urls]
 Home = "https://github.com/conda/conda-package-streaming"
 Documentation = "https://conda.github.io/conda-package-streaming/"
```

### Comparing `conda_package_streaming-0.7.0/PKG-INFO` & `conda_package_streaming-0.8.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: conda_package_streaming
-Version: 0.7.0
-Summary: Download metadata from conda packages without transferring entire file.
+Version: 0.8.0
+Summary: An efficient library to read from new and old format .conda and .tar.bz2 conda packages.
 Author-email: "Anaconda, Inc. & Contributors" <conda@continuum.io>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
@@ -17,21 +17,28 @@
 Requires-Dist: mdit-py-plugins>=0.3.0 ; extra == "docs"
 Requires-Dist: pytest >=7 ; extra == "test"
 Requires-Dist: pytest-cov ; extra == "test"
 Requires-Dist: pytest-mock ; extra == "test"
 Requires-Dist: boto3 ; extra == "test"
 Requires-Dist: boto3-stubs[essential] ; extra == "test"
 Requires-Dist: bottle ; extra == "test"
+Requires-Dist: conda ; extra == "test"
+Requires-Dist: conda-package-handling >=2 ; extra == "test"
 Project-URL: Documentation, https://conda.github.io/conda-package-streaming/
 Project-URL: Home, https://github.com/conda/conda-package-streaming
 Provides-Extra: docs
 Provides-Extra: test
 
 # conda-package-streaming
 
+[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/conda/conda-package-streaming/main.svg)](https://results.pre-commit.ci/latest/github/conda/conda-package-streaming/main)
+
+An efficient library to read from new and old format .conda and .tar.bz2 conda
+packages.
+
 Download conda metadata from packages without transferring entire file. Get
 metadata from local `.tar.bz2` packages without reading entire files.
 
 Uses enhanced pip `lazy_wheel` to fetch a file out of `.conda` with no more than
 3 range requests, but usually 2.
 
 Uses `tar = tarfile.open(fileobj=...)` to stream remote `.tar.bz2`. Closes the
@@ -88,14 +95,18 @@
 with closing(conda):
     for tar, member in stream_conda_component(filename, conda, component="info"):
         if member.name == "info/index.json":
             index_json = json.load(tar.extractfile(member))
             break
 ```
 
+If you need the entire package, download it first and use the file-based APIs.
+The URL-based APIs are more efficient if you only need to access package
+metadata.
+
 # Package goals
 
 * Extract conda packages (both formats)
 * Easy to install from pypi or conda
 * Do the least amount of I/O possible (no temporary files, transfer partial packages)
 * Open files from the network / standard HTTP / s3
```

