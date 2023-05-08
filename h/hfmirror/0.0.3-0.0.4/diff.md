# Comparing `tmp/hfmirror-0.0.3.tar.gz` & `tmp/hfmirror-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hfmirror-0.0.3.tar", last modified: Sat Apr 15 11:27:23 2023, max compression
+gzip compressed data, was "hfmirror-0.0.4.tar", last modified: Mon May  8 09:27:39 2023, max compression
```

## Comparing `hfmirror-0.0.3.tar` & `hfmirror-0.0.4.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 11:27:23.290458 hfmirror-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-15 11:26:43.000000 hfmirror-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-15 11:26:43.000000 hfmirror-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7550 2023-04-15 11:27:23.290458 hfmirror-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6669 2023-04-15 11:26:43.000000 hfmirror-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 11:27:23.290458 hfmirror-0.0.3/hfmirror/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-15 11:26:43.000000 hfmirror-0.0.3/hfmirror/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 11:27:23.290458 hfmirror-0.0.3/hfmirror/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 11:26:43.000000 hfmirror-0.0.3/hfmirror/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-15 11:26:43.000000 hfmirror-0.0.3/hfmirror/config/meta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 11:27:23.290458 hfmirror-0.0.3/hfmirror/resource/
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-15 11:26:43.000000 hfmirror-0.0.3/hfmirror/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-04-15 11:26:43.000000 hfmirror-0.0.3/hfmirror/resource/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     5803 2023-04-15 11:26:43.000000 hfmirror-0.0.3/hfmirror/resource/item.py
--rw-r--r--   0 runner    (1001) docker     (123)     7809 2023-04-15 11:26:43.000000 hfmirror-0.0.3/hfmirror/resource/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-04-15 11:26:43.000000 hfmirror-0.0.3/hfmirror/resource/sourceforge.py
--rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-04-15 11:26:43.000000 hfmirror-0.0.3/hfmirror/resource/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 11:27:23.290458 hfmirror-0.0.3/hfmirror/storage/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-15 11:26:43.000000 hfmirror-0.0.3/hfmirror/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-15 11:26:43.000000 hfmirror-0.0.3/hfmirror/storage/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7786 2023-04-15 11:26:43.000000 hfmirror-0.0.3/hfmirror/storage/huggingface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-04-15 11:26:43.000000 hfmirror-0.0.3/hfmirror/storage/local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 11:27:23.290458 hfmirror-0.0.3/hfmirror/sync/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-15 11:26:43.000000 hfmirror-0.0.3/hfmirror/sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-04-15 11:26:43.000000 hfmirror-0.0.3/hfmirror/sync/sync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 11:27:23.290458 hfmirror-0.0.3/hfmirror/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-15 11:26:43.000000 hfmirror-0.0.3/hfmirror/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-04-15 11:26:43.000000 hfmirror-0.0.3/hfmirror/utils/download.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-15 11:26:43.000000 hfmirror-0.0.3/hfmirror/utils/hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-15 11:26:43.000000 hfmirror-0.0.3/hfmirror/utils/segments.py
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-04-15 11:26:43.000000 hfmirror-0.0.3/hfmirror/utils/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-04-15 11:26:43.000000 hfmirror-0.0.3/hfmirror/utils/text.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 11:27:23.290458 hfmirror-0.0.3/hfmirror.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7550 2023-04-15 11:27:23.000000 hfmirror-0.0.3/hfmirror.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-04-15 11:27:23.000000 hfmirror-0.0.3/hfmirror.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 11:27:23.000000 hfmirror-0.0.3/hfmirror.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-15 11:27:23.000000 hfmirror-0.0.3/hfmirror.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-15 11:27:23.000000 hfmirror-0.0.3/hfmirror.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-15 11:26:43.000000 hfmirror-0.0.3/requirements-doc.txt
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-15 11:26:43.000000 hfmirror-0.0.3/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-15 11:26:43.000000 hfmirror-0.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 11:27:23.290458 hfmirror-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-04-15 11:26:43.000000 hfmirror-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:27:39.014018 hfmirror-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-08 09:27:02.000000 hfmirror-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-08 09:27:02.000000 hfmirror-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7551 2023-05-08 09:27:39.014018 hfmirror-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6670 2023-05-08 09:27:02.000000 hfmirror-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:27:39.010018 hfmirror-0.0.4/hfmirror/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-08 09:27:02.000000 hfmirror-0.0.4/hfmirror/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:27:39.010018 hfmirror-0.0.4/hfmirror/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 09:27:02.000000 hfmirror-0.0.4/hfmirror/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-08 09:27:02.000000 hfmirror-0.0.4/hfmirror/config/meta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:27:39.010018 hfmirror-0.0.4/hfmirror/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-05-08 09:27:02.000000 hfmirror-0.0.4/hfmirror/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-05-08 09:27:02.000000 hfmirror-0.0.4/hfmirror/resource/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5803 2023-05-08 09:27:02.000000 hfmirror-0.0.4/hfmirror/resource/item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7809 2023-05-08 09:27:02.000000 hfmirror-0.0.4/hfmirror/resource/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-05-08 09:27:02.000000 hfmirror-0.0.4/hfmirror/resource/sourceforge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-05-08 09:27:02.000000 hfmirror-0.0.4/hfmirror/resource/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:27:39.014018 hfmirror-0.0.4/hfmirror/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-08 09:27:02.000000 hfmirror-0.0.4/hfmirror/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-08 09:27:02.000000 hfmirror-0.0.4/hfmirror/storage/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8195 2023-05-08 09:27:02.000000 hfmirror-0.0.4/hfmirror/storage/huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-05-08 09:27:02.000000 hfmirror-0.0.4/hfmirror/storage/local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:27:39.014018 hfmirror-0.0.4/hfmirror/sync/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-08 09:27:02.000000 hfmirror-0.0.4/hfmirror/sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-05-08 09:27:02.000000 hfmirror-0.0.4/hfmirror/sync/sync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:27:39.014018 hfmirror-0.0.4/hfmirror/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-08 09:27:02.000000 hfmirror-0.0.4/hfmirror/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-05-08 09:27:02.000000 hfmirror-0.0.4/hfmirror/utils/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-08 09:27:02.000000 hfmirror-0.0.4/hfmirror/utils/hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-08 09:27:02.000000 hfmirror-0.0.4/hfmirror/utils/segments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-05-08 09:27:02.000000 hfmirror-0.0.4/hfmirror/utils/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-05-08 09:27:02.000000 hfmirror-0.0.4/hfmirror/utils/text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:27:39.010018 hfmirror-0.0.4/hfmirror.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7551 2023-05-08 09:27:38.000000 hfmirror-0.0.4/hfmirror.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-08 09:27:39.000000 hfmirror-0.0.4/hfmirror.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 09:27:38.000000 hfmirror-0.0.4/hfmirror.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-08 09:27:38.000000 hfmirror-0.0.4/hfmirror.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-08 09:27:38.000000 hfmirror-0.0.4/hfmirror.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-08 09:27:02.000000 hfmirror-0.0.4/requirements-doc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-08 09:27:02.000000 hfmirror-0.0.4/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-08 09:27:02.000000 hfmirror-0.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 09:27:39.014018 hfmirror-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-05-08 09:27:02.000000 hfmirror-0.0.4/setup.py
```

### Comparing `hfmirror-0.0.3/LICENSE` & `hfmirror-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hfmirror-0.0.3/PKG-INFO` & `hfmirror-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hfmirror
-Version: 0.0.3
+Version: 0.0.4
 Summary: Mirror for resources to local and huggingface.
 Home-page: https://github.com/narugo1992/hfmirror
 Author: narugo1992
 Author-email: narugo@126.com
 License: Apache License, Version 2.0
 Keywords: A simple tool for automatic parameter tuning.
 Classifier: Development Status :: 5 - Production/Stable
@@ -45,15 +45,15 @@
 Mirror for resources to local and huggingface.
 
 ## Installation
 
 You can simply install it with `pip` command line from the official PyPI site.
 
 ```bash
-pip install hbutils
+pip install hfmirror
 ```
 
 For more information about installation, you can refer to [Installation](https://narugo1992.github.io/hfmirror/main/tutorials/installation/index.html).
 
 ## Quick Start
 
 ### Mirror Github Releases to Your Disk
```

### Comparing `hfmirror-0.0.3/README.md` & `hfmirror-0.0.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 Mirror for resources to local and huggingface.
 
 ## Installation
 
 You can simply install it with `pip` command line from the official PyPI site.
 
 ```bash
-pip install hbutils
+pip install hfmirror
 ```
 
 For more information about installation, you can refer to [Installation](https://narugo1992.github.io/hfmirror/main/tutorials/installation/index.html).
 
 ## Quick Start
 
 ### Mirror Github Releases to Your Disk
```

### Comparing `hfmirror-0.0.3/hfmirror/resource/github.py` & `hfmirror-0.0.4/hfmirror/resource/github.py`

 * *Files identical despite different names*

### Comparing `hfmirror-0.0.3/hfmirror/resource/item.py` & `hfmirror-0.0.4/hfmirror/resource/item.py`

 * *Files identical despite different names*

### Comparing `hfmirror-0.0.3/hfmirror/resource/resource.py` & `hfmirror-0.0.4/hfmirror/resource/resource.py`

 * *Files identical despite different names*

### Comparing `hfmirror-0.0.3/hfmirror/resource/sourceforge.py` & `hfmirror-0.0.4/hfmirror/resource/sourceforge.py`

 * *Files identical despite different names*

### Comparing `hfmirror-0.0.3/hfmirror/resource/version.py` & `hfmirror-0.0.4/hfmirror/resource/version.py`

 * *Files identical despite different names*

### Comparing `hfmirror-0.0.3/hfmirror/storage/base.py` & `hfmirror-0.0.4/hfmirror/storage/base.py`

 * *Files identical despite different names*

### Comparing `hfmirror-0.0.3/hfmirror/storage/huggingface.py` & `hfmirror-0.0.4/hfmirror/storage/huggingface.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,27 @@
 import datetime
 import os
 import warnings
+from functools import partial, lru_cache
 from hashlib import sha256, sha1
-from typing import List, Tuple, Optional, Union
+from typing import List, Tuple, Optional, Union, Dict
 
-from huggingface_hub import HfApi, hf_hub_url, CommitOperationAdd, CommitOperationDelete
+from huggingface_hub import HfApi, hf_hub_url, CommitOperationAdd, CommitOperationDelete, configure_http_backend
 
 from .base import BaseStorage
 from ..utils import to_segments, srequest, get_requests_session
 
+DEFAULT_TIMEOUT: int = 10
+
+
+@lru_cache()
+def _register_session_for_hf(max_retries: int = 5, timeout: int = DEFAULT_TIMEOUT,
+                             headers: Optional[Dict[str, str]] = None):
+    configure_http_backend(backend_factory=partial(get_requests_session, max_retries, timeout, headers))
+
 
 def _single_resource_is_duplicated(local_filename: str, is_lfs: bool, oid: str, filesize: int,
                                    chunk_for_hash: int = 1 << 20) -> bool:
     if filesize != os.path.getsize(local_filename):
         return False
 
     if is_lfs:
@@ -121,14 +130,16 @@
         else:  # network error
             resp.raise_for_status()  # pragma: no cover
 
     def read_text(self, file: List[str], encoding: str = 'utf-8') -> str:
         return srequest(self.session, 'GET', self._file_url(file)).content.decode(encoding=encoding)
 
     def batch_change_files(self, changes: List[Tuple[Optional[str], List[str]]]):
+        _register_session_for_hf()
+
         _map_changes = {}
         for local_filename, file_in_repo in changes:
             sg = tuple(file_in_repo)
             if sg in _map_changes:
                 fip = self.path_join(*file_in_repo)
                 if _map_changes[sg] is None:
                     warnings.warn(f'Deletion of resource {fip!r} is not necessary, will be ignored.')
```

### Comparing `hfmirror-0.0.3/hfmirror/storage/local.py` & `hfmirror-0.0.4/hfmirror/storage/local.py`

 * *Files identical despite different names*

### Comparing `hfmirror-0.0.3/hfmirror/sync/sync.py` & `hfmirror-0.0.4/hfmirror/sync/sync.py`

 * *Files identical despite different names*

### Comparing `hfmirror-0.0.3/hfmirror/utils/download.py` & `hfmirror-0.0.4/hfmirror/utils/download.py`

 * *Files identical despite different names*

### Comparing `hfmirror-0.0.3/hfmirror/utils/hash.py` & `hfmirror-0.0.4/hfmirror/utils/hash.py`

 * *Files identical despite different names*

### Comparing `hfmirror-0.0.3/hfmirror/utils/segments.py` & `hfmirror-0.0.4/hfmirror/utils/segments.py`

 * *Files identical despite different names*

### Comparing `hfmirror-0.0.3/hfmirror/utils/session.py` & `hfmirror-0.0.4/hfmirror/utils/session.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,17 +24,16 @@
 
 
 def get_requests_session(max_retries: int = 5, timeout: int = DEFAULT_TIMEOUT,
                          headers: Optional[Dict[str, str]] = None) -> requests.Session:
     session = requests.session()
     retries = Retry(
         total=max_retries, backoff_factor=1,
-        # status_forcelist=[500, 501, 502, 503, 504, 505, 506, 507, 509, 510, 511],
-        status_forcelist=[429, 500, 502, 503, 504],
-        allowed_methods=["HEAD", "GET", "OPTIONS"],
+        status_forcelist=[413, 429, 500, 501, 502, 503, 504, 505, 506, 507, 509, 510, 511],
+        allowed_methods=["HEAD", "GET", "POST", "PUT", "DELETE", "OPTIONS", "TRACE"],
     )
     adapter = TimeoutHTTPAdapter(max_retries=retries, timeout=timeout)
     session.mount('http://', adapter)
     session.mount('https://', adapter)
     session.headers.update({
         "User-Agent": "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 "
                       "(KHTML, like Gecko) Chrome/108.0.0.0 Safari/537.36",
```

### Comparing `hfmirror-0.0.3/hfmirror/utils/text.py` & `hfmirror-0.0.4/hfmirror/utils/text.py`

 * *Files identical despite different names*

### Comparing `hfmirror-0.0.3/hfmirror.egg-info/PKG-INFO` & `hfmirror-0.0.4/hfmirror.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hfmirror
-Version: 0.0.3
+Version: 0.0.4
 Summary: Mirror for resources to local and huggingface.
 Home-page: https://github.com/narugo1992/hfmirror
 Author: narugo1992
 Author-email: narugo@126.com
 License: Apache License, Version 2.0
 Keywords: A simple tool for automatic parameter tuning.
 Classifier: Development Status :: 5 - Production/Stable
@@ -45,15 +45,15 @@
 Mirror for resources to local and huggingface.
 
 ## Installation
 
 You can simply install it with `pip` command line from the official PyPI site.
 
 ```bash
-pip install hbutils
+pip install hfmirror
 ```
 
 For more information about installation, you can refer to [Installation](https://narugo1992.github.io/hfmirror/main/tutorials/installation/index.html).
 
 ## Quick Start
 
 ### Mirror Github Releases to Your Disk
```

### Comparing `hfmirror-0.0.3/hfmirror.egg-info/SOURCES.txt` & `hfmirror-0.0.4/hfmirror.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hfmirror-0.0.3/hfmirror.egg-info/requires.txt` & `hfmirror-0.0.4/hfmirror.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-hbutils>=0.8.6
+hbutils>=0.9.0
 tqdm>=4.0.0
 click>=7.0.0
 requests
 pyquery
 pygithub
 huggingface_hub
```

### Comparing `hfmirror-0.0.3/setup.py` & `hfmirror-0.0.4/setup.py`

 * *Files identical despite different names*

