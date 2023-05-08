# Comparing `tmp/hfmirror-0.0.4.tar.gz` & `tmp/hfmirror-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hfmirror-0.0.4.tar", last modified: Mon May  8 09:27:39 2023, max compression
+gzip compressed data, was "hfmirror-0.0.5.tar", last modified: Mon May  8 11:17:56 2023, max compression
```

## Comparing `hfmirror-0.0.4.tar` & `hfmirror-0.0.5.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:27:39.014018 hfmirror-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-08 09:27:02.000000 hfmirror-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-08 09:27:02.000000 hfmirror-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7551 2023-05-08 09:27:39.014018 hfmirror-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6670 2023-05-08 09:27:02.000000 hfmirror-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:27:39.010018 hfmirror-0.0.4/hfmirror/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-08 09:27:02.000000 hfmirror-0.0.4/hfmirror/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:27:39.010018 hfmirror-0.0.4/hfmirror/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 09:27:02.000000 hfmirror-0.0.4/hfmirror/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-08 09:27:02.000000 hfmirror-0.0.4/hfmirror/config/meta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:27:39.010018 hfmirror-0.0.4/hfmirror/resource/
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-05-08 09:27:02.000000 hfmirror-0.0.4/hfmirror/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-05-08 09:27:02.000000 hfmirror-0.0.4/hfmirror/resource/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     5803 2023-05-08 09:27:02.000000 hfmirror-0.0.4/hfmirror/resource/item.py
--rw-r--r--   0 runner    (1001) docker     (123)     7809 2023-05-08 09:27:02.000000 hfmirror-0.0.4/hfmirror/resource/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-05-08 09:27:02.000000 hfmirror-0.0.4/hfmirror/resource/sourceforge.py
--rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-05-08 09:27:02.000000 hfmirror-0.0.4/hfmirror/resource/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:27:39.014018 hfmirror-0.0.4/hfmirror/storage/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-08 09:27:02.000000 hfmirror-0.0.4/hfmirror/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-08 09:27:02.000000 hfmirror-0.0.4/hfmirror/storage/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8195 2023-05-08 09:27:02.000000 hfmirror-0.0.4/hfmirror/storage/huggingface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-05-08 09:27:02.000000 hfmirror-0.0.4/hfmirror/storage/local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:27:39.014018 hfmirror-0.0.4/hfmirror/sync/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-08 09:27:02.000000 hfmirror-0.0.4/hfmirror/sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-05-08 09:27:02.000000 hfmirror-0.0.4/hfmirror/sync/sync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:27:39.014018 hfmirror-0.0.4/hfmirror/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-08 09:27:02.000000 hfmirror-0.0.4/hfmirror/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-05-08 09:27:02.000000 hfmirror-0.0.4/hfmirror/utils/download.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-08 09:27:02.000000 hfmirror-0.0.4/hfmirror/utils/hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-08 09:27:02.000000 hfmirror-0.0.4/hfmirror/utils/segments.py
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-05-08 09:27:02.000000 hfmirror-0.0.4/hfmirror/utils/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-05-08 09:27:02.000000 hfmirror-0.0.4/hfmirror/utils/text.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:27:39.010018 hfmirror-0.0.4/hfmirror.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7551 2023-05-08 09:27:38.000000 hfmirror-0.0.4/hfmirror.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-08 09:27:39.000000 hfmirror-0.0.4/hfmirror.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 09:27:38.000000 hfmirror-0.0.4/hfmirror.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-08 09:27:38.000000 hfmirror-0.0.4/hfmirror.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-08 09:27:38.000000 hfmirror-0.0.4/hfmirror.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-08 09:27:02.000000 hfmirror-0.0.4/requirements-doc.txt
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-08 09:27:02.000000 hfmirror-0.0.4/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-08 09:27:02.000000 hfmirror-0.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 09:27:39.014018 hfmirror-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-05-08 09:27:02.000000 hfmirror-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:17:56.348106 hfmirror-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-08 11:17:22.000000 hfmirror-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-08 11:17:22.000000 hfmirror-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7551 2023-05-08 11:17:56.348106 hfmirror-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6670 2023-05-08 11:17:22.000000 hfmirror-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:17:56.344106 hfmirror-0.0.5/hfmirror/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-08 11:17:22.000000 hfmirror-0.0.5/hfmirror/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:17:56.348106 hfmirror-0.0.5/hfmirror/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:17:22.000000 hfmirror-0.0.5/hfmirror/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-08 11:17:22.000000 hfmirror-0.0.5/hfmirror/config/meta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:17:56.348106 hfmirror-0.0.5/hfmirror/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-05-08 11:17:22.000000 hfmirror-0.0.5/hfmirror/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-05-08 11:17:22.000000 hfmirror-0.0.5/hfmirror/resource/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5803 2023-05-08 11:17:22.000000 hfmirror-0.0.5/hfmirror/resource/item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7809 2023-05-08 11:17:22.000000 hfmirror-0.0.5/hfmirror/resource/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-05-08 11:17:22.000000 hfmirror-0.0.5/hfmirror/resource/sourceforge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-05-08 11:17:22.000000 hfmirror-0.0.5/hfmirror/resource/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:17:56.348106 hfmirror-0.0.5/hfmirror/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-08 11:17:22.000000 hfmirror-0.0.5/hfmirror/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-08 11:17:22.000000 hfmirror-0.0.5/hfmirror/storage/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8195 2023-05-08 11:17:22.000000 hfmirror-0.0.5/hfmirror/storage/huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-05-08 11:17:22.000000 hfmirror-0.0.5/hfmirror/storage/local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:17:56.348106 hfmirror-0.0.5/hfmirror/sync/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-08 11:17:22.000000 hfmirror-0.0.5/hfmirror/sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-05-08 11:17:22.000000 hfmirror-0.0.5/hfmirror/sync/sync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:17:56.348106 hfmirror-0.0.5/hfmirror/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-08 11:17:22.000000 hfmirror-0.0.5/hfmirror/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-05-08 11:17:22.000000 hfmirror-0.0.5/hfmirror/utils/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-08 11:17:22.000000 hfmirror-0.0.5/hfmirror/utils/hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-08 11:17:22.000000 hfmirror-0.0.5/hfmirror/utils/segments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-05-08 11:17:22.000000 hfmirror-0.0.5/hfmirror/utils/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-05-08 11:17:22.000000 hfmirror-0.0.5/hfmirror/utils/text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:17:56.348106 hfmirror-0.0.5/hfmirror.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7551 2023-05-08 11:17:56.000000 hfmirror-0.0.5/hfmirror.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-08 11:17:56.000000 hfmirror-0.0.5/hfmirror.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 11:17:56.000000 hfmirror-0.0.5/hfmirror.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-08 11:17:56.000000 hfmirror-0.0.5/hfmirror.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-08 11:17:56.000000 hfmirror-0.0.5/hfmirror.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-08 11:17:22.000000 hfmirror-0.0.5/requirements-doc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-08 11:17:22.000000 hfmirror-0.0.5/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-08 11:17:22.000000 hfmirror-0.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 11:17:56.348106 hfmirror-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-05-08 11:17:22.000000 hfmirror-0.0.5/setup.py
```

### Comparing `hfmirror-0.0.4/LICENSE` & `hfmirror-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `hfmirror-0.0.4/PKG-INFO` & `hfmirror-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hfmirror
-Version: 0.0.4
+Version: 0.0.5
 Summary: Mirror for resources to local and huggingface.
 Home-page: https://github.com/narugo1992/hfmirror
 Author: narugo1992
 Author-email: narugo@126.com
 License: Apache License, Version 2.0
 Keywords: A simple tool for automatic parameter tuning.
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `hfmirror-0.0.4/README.md` & `hfmirror-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `hfmirror-0.0.4/hfmirror/resource/github.py` & `hfmirror-0.0.5/hfmirror/resource/github.py`

 * *Files 12% similar despite different names*

```diff
@@ -44,18 +44,22 @@
         for release in repo_tqdm:
             release: GitRelease
             tag_name = self._tag_filter(release.tag_name)
             repo_tqdm.set_description(tag_name)
             if not tag_name:
                 continue
 
-            yield 'version', tag_name, tag_name
-            release_metadata = {'version': release.tag_name, 'title': release.title, 'url': release.html_url}
-            yield 'metadata', release_metadata, tag_name
+            has_file = False
             for asset in release.get_assets():
                 filename = self._filename_filter(tag_name, asset.name)
                 if not filename:
                     continue
 
                 download_url = asset.browser_download_url
                 metadata = {'tag': release.tag_name, 'filename': asset.name}
                 yield 'remote', download_url, f'{tag_name}/{filename}', metadata
+                has_file = True
+
+            if has_file:
+                yield 'version', tag_name, tag_name
+                release_metadata = {'version': release.tag_name, 'title': release.title, 'url': release.html_url}
+                yield 'metadata', release_metadata, tag_name
```

### Comparing `hfmirror-0.0.4/hfmirror/resource/item.py` & `hfmirror-0.0.5/hfmirror/resource/item.py`

 * *Files identical despite different names*

### Comparing `hfmirror-0.0.4/hfmirror/resource/resource.py` & `hfmirror-0.0.5/hfmirror/resource/resource.py`

 * *Files identical despite different names*

### Comparing `hfmirror-0.0.4/hfmirror/resource/sourceforge.py` & `hfmirror-0.0.5/hfmirror/resource/sourceforge.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,15 @@
     def grab_for_items(self) -> Iterable[Union[
         Tuple[str, Any, TargetPathType, Mapping],
         Tuple[str, Any, TargetPathType],
     ]]:
         yield 'metadata', {'source': self.root_url}, ''
         session = get_requests_session()
         for type_, segments, download_url in self._walk_on_sourceforge(self.root_url, [], session):
-            version = self._get_version(type_, segments)
-            if version is not None:
-                yield 'version', version, segments
-
             if type_ == 'file':
                 yield 'wget', download_url, segments
             else:  # directory
                 yield 'metadata', {'page_url': download_url}, segments
+
+            version = self._get_version(type_, segments)
+            if version is not None:
+                yield 'version', version, segments
```

### Comparing `hfmirror-0.0.4/hfmirror/resource/version.py` & `hfmirror-0.0.5/hfmirror/resource/version.py`

 * *Files identical despite different names*

### Comparing `hfmirror-0.0.4/hfmirror/storage/base.py` & `hfmirror-0.0.5/hfmirror/storage/base.py`

 * *Files identical despite different names*

### Comparing `hfmirror-0.0.4/hfmirror/storage/huggingface.py` & `hfmirror-0.0.5/hfmirror/storage/huggingface.py`

 * *Files identical despite different names*

### Comparing `hfmirror-0.0.4/hfmirror/storage/local.py` & `hfmirror-0.0.5/hfmirror/storage/local.py`

 * *Files identical despite different names*

### Comparing `hfmirror-0.0.4/hfmirror/sync/sync.py` & `hfmirror-0.0.5/hfmirror/sync/sync.py`

 * *Files identical despite different names*

### Comparing `hfmirror-0.0.4/hfmirror/utils/download.py` & `hfmirror-0.0.5/hfmirror/utils/download.py`

 * *Files identical despite different names*

### Comparing `hfmirror-0.0.4/hfmirror/utils/hash.py` & `hfmirror-0.0.5/hfmirror/utils/hash.py`

 * *Files identical despite different names*

### Comparing `hfmirror-0.0.4/hfmirror/utils/segments.py` & `hfmirror-0.0.5/hfmirror/utils/segments.py`

 * *Files identical despite different names*

### Comparing `hfmirror-0.0.4/hfmirror/utils/session.py` & `hfmirror-0.0.5/hfmirror/utils/session.py`

 * *Files identical despite different names*

### Comparing `hfmirror-0.0.4/hfmirror/utils/text.py` & `hfmirror-0.0.5/hfmirror/utils/text.py`

 * *Files identical despite different names*

### Comparing `hfmirror-0.0.4/hfmirror.egg-info/PKG-INFO` & `hfmirror-0.0.5/hfmirror.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hfmirror
-Version: 0.0.4
+Version: 0.0.5
 Summary: Mirror for resources to local and huggingface.
 Home-page: https://github.com/narugo1992/hfmirror
 Author: narugo1992
 Author-email: narugo@126.com
 License: Apache License, Version 2.0
 Keywords: A simple tool for automatic parameter tuning.
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `hfmirror-0.0.4/hfmirror.egg-info/SOURCES.txt` & `hfmirror-0.0.5/hfmirror.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hfmirror-0.0.4/hfmirror.egg-info/requires.txt` & `hfmirror-0.0.5/hfmirror.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `hfmirror-0.0.4/setup.py` & `hfmirror-0.0.5/setup.py`

 * *Files identical despite different names*

