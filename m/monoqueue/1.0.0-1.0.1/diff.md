# Comparing `tmp/monoqueue-1.0.0.tar.gz` & `tmp/monoqueue-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monoqueue-1.0.0.tar", last modified: Sat May  6 23:57:48 2023, max compression
+gzip compressed data, was "monoqueue-1.0.1.tar", last modified: Mon May  8 19:54:44 2023, max compression
```

## Comparing `monoqueue-1.0.0.tar` & `monoqueue-1.0.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 curtis    (1000) curtis    (1000)        0 2023-05-06 23:57:48.633030 monoqueue-1.0.0/
--rw-rw-r--   0 curtis    (1000) curtis    (1000)     7747 2023-05-06 23:57:48.633030 monoqueue-1.0.0/PKG-INFO
--rw-rw-r--   0 curtis    (1000) curtis    (1000)     6538 2023-04-30 03:14:32.000000 monoqueue-1.0.0/README.md
--rw-rw-r--   0 curtis    (1000) curtis    (1000)     1503 2023-05-06 23:53:32.000000 monoqueue-1.0.0/pyproject.toml
--rw-rw-r--   0 curtis    (1000) curtis    (1000)       38 2023-05-06 23:57:48.633030 monoqueue-1.0.0/setup.cfg
-drwxrwxr-x   0 curtis    (1000) curtis    (1000)        0 2023-05-06 23:57:48.633030 monoqueue-1.0.0/src/
-drwxrwxr-x   0 curtis    (1000) curtis    (1000)        0 2023-05-06 23:57:48.633030 monoqueue-1.0.0/src/monoqueue/
--rw-rw-r--   0 curtis    (1000) curtis    (1000)    10198 2023-05-06 23:47:21.000000 monoqueue-1.0.0/src/monoqueue/__init__.py
--rw-rw-r--   0 curtis    (1000) curtis    (1000)      423 2023-04-27 20:42:24.000000 monoqueue-1.0.0/src/monoqueue/__main__.py
--rw-rw-r--   0 curtis    (1000) curtis    (1000)     2680 2023-05-06 23:47:56.000000 monoqueue-1.0.0/src/monoqueue/cli.py
--rw-rw-r--   0 curtis    (1000) curtis    (1000)     3426 2023-04-27 20:42:24.000000 monoqueue-1.0.0/src/monoqueue/discourse.py
--rw-rw-r--   0 curtis    (1000) curtis    (1000)     2924 2023-05-06 17:41:10.000000 monoqueue-1.0.0/src/monoqueue/firefox.py
--rw-rw-r--   0 curtis    (1000) curtis    (1000)     2903 2023-04-27 20:42:24.000000 monoqueue-1.0.0/src/monoqueue/github.py
--rw-rw-r--   0 curtis    (1000) curtis    (1000)      548 2023-04-27 20:42:24.000000 monoqueue-1.0.0/src/monoqueue/log.py
--rw-rw-r--   0 curtis    (1000) curtis    (1000)     7617 2023-04-29 18:07:24.000000 monoqueue-1.0.0/src/monoqueue/parse.py
--rw-rw-r--   0 curtis    (1000) curtis    (1000)     2811 2023-05-06 17:41:10.000000 monoqueue-1.0.0/src/monoqueue/time.py
--rw-rw-r--   0 curtis    (1000) curtis    (1000)     4409 2023-05-06 23:49:09.000000 monoqueue-1.0.0/src/monoqueue/ui.py
-drwxrwxr-x   0 curtis    (1000) curtis    (1000)        0 2023-05-06 23:57:48.633030 monoqueue-1.0.0/src/monoqueue.egg-info/
--rw-rw-r--   0 curtis    (1000) curtis    (1000)     7747 2023-05-06 23:57:48.000000 monoqueue-1.0.0/src/monoqueue.egg-info/PKG-INFO
--rw-rw-r--   0 curtis    (1000) curtis    (1000)      503 2023-05-06 23:57:48.000000 monoqueue-1.0.0/src/monoqueue.egg-info/SOURCES.txt
--rw-rw-r--   0 curtis    (1000) curtis    (1000)        1 2023-05-06 23:57:48.000000 monoqueue-1.0.0/src/monoqueue.egg-info/dependency_links.txt
--rw-rw-r--   0 curtis    (1000) curtis    (1000)       42 2023-05-06 23:57:48.000000 monoqueue-1.0.0/src/monoqueue.egg-info/entry_points.txt
--rw-rw-r--   0 curtis    (1000) curtis    (1000)       22 2023-05-06 23:57:48.000000 monoqueue-1.0.0/src/monoqueue.egg-info/requires.txt
--rw-rw-r--   0 curtis    (1000) curtis    (1000)       10 2023-05-06 23:57:48.000000 monoqueue-1.0.0/src/monoqueue.egg-info/top_level.txt
-drwxrwxr-x   0 curtis    (1000) curtis    (1000)        0 2023-05-06 23:57:48.633030 monoqueue-1.0.0/tests/
--rw-rw-r--   0 curtis    (1000) curtis    (1000)     2756 2023-04-29 16:19:18.000000 monoqueue-1.0.0/tests/test_parse.py
+drwxrwxr-x   0 curtis    (1000) curtis    (1000)        0 2023-05-08 19:54:44.215310 monoqueue-1.0.1/
+-rw-rw-r--   0 curtis    (1000) curtis    (1000)     7747 2023-05-08 19:54:44.215310 monoqueue-1.0.1/PKG-INFO
+-rw-rw-r--   0 curtis    (1000) curtis    (1000)     6538 2023-04-30 03:14:32.000000 monoqueue-1.0.1/README.md
+-rw-rw-r--   0 curtis    (1000) curtis    (1000)     1503 2023-05-08 19:54:30.000000 monoqueue-1.0.1/pyproject.toml
+-rw-rw-r--   0 curtis    (1000) curtis    (1000)       38 2023-05-08 19:54:44.215310 monoqueue-1.0.1/setup.cfg
+drwxrwxr-x   0 curtis    (1000) curtis    (1000)        0 2023-05-08 19:54:44.215310 monoqueue-1.0.1/src/
+drwxrwxr-x   0 curtis    (1000) curtis    (1000)        0 2023-05-08 19:54:44.215310 monoqueue-1.0.1/src/monoqueue/
+-rw-rw-r--   0 curtis    (1000) curtis    (1000)    10187 2023-05-08 15:53:41.000000 monoqueue-1.0.1/src/monoqueue/__init__.py
+-rw-rw-r--   0 curtis    (1000) curtis    (1000)      423 2023-04-27 20:42:24.000000 monoqueue-1.0.1/src/monoqueue/__main__.py
+-rw-rw-r--   0 curtis    (1000) curtis    (1000)     2680 2023-05-06 23:47:56.000000 monoqueue-1.0.1/src/monoqueue/cli.py
+-rw-rw-r--   0 curtis    (1000) curtis    (1000)     3429 2023-05-08 15:53:58.000000 monoqueue-1.0.1/src/monoqueue/discourse.py
+-rw-rw-r--   0 curtis    (1000) curtis    (1000)     2927 2023-05-08 15:54:00.000000 monoqueue-1.0.1/src/monoqueue/firefox.py
+-rw-rw-r--   0 curtis    (1000) curtis    (1000)     2906 2023-05-08 15:54:04.000000 monoqueue-1.0.1/src/monoqueue/github.py
+-rw-rw-r--   0 curtis    (1000) curtis    (1000)      548 2023-04-27 20:42:24.000000 monoqueue-1.0.1/src/monoqueue/log.py
+-rw-rw-r--   0 curtis    (1000) curtis    (1000)     7617 2023-04-29 18:07:24.000000 monoqueue-1.0.1/src/monoqueue/parse.py
+-rw-rw-r--   0 curtis    (1000) curtis    (1000)     2811 2023-05-06 17:41:10.000000 monoqueue-1.0.1/src/monoqueue/time.py
+-rw-rw-r--   0 curtis    (1000) curtis    (1000)     4409 2023-05-06 23:49:09.000000 monoqueue-1.0.1/src/monoqueue/ui.py
+drwxrwxr-x   0 curtis    (1000) curtis    (1000)        0 2023-05-08 19:54:44.215310 monoqueue-1.0.1/src/monoqueue.egg-info/
+-rw-rw-r--   0 curtis    (1000) curtis    (1000)     7747 2023-05-08 19:54:44.000000 monoqueue-1.0.1/src/monoqueue.egg-info/PKG-INFO
+-rw-rw-r--   0 curtis    (1000) curtis    (1000)      503 2023-05-08 19:54:44.000000 monoqueue-1.0.1/src/monoqueue.egg-info/SOURCES.txt
+-rw-rw-r--   0 curtis    (1000) curtis    (1000)        1 2023-05-08 19:54:44.000000 monoqueue-1.0.1/src/monoqueue.egg-info/dependency_links.txt
+-rw-rw-r--   0 curtis    (1000) curtis    (1000)       42 2023-05-08 19:54:44.000000 monoqueue-1.0.1/src/monoqueue.egg-info/entry_points.txt
+-rw-rw-r--   0 curtis    (1000) curtis    (1000)       22 2023-05-08 19:54:44.000000 monoqueue-1.0.1/src/monoqueue.egg-info/requires.txt
+-rw-rw-r--   0 curtis    (1000) curtis    (1000)       10 2023-05-08 19:54:44.000000 monoqueue-1.0.1/src/monoqueue.egg-info/top_level.txt
+drwxrwxr-x   0 curtis    (1000) curtis    (1000)        0 2023-05-08 19:54:44.215310 monoqueue-1.0.1/tests/
+-rw-rw-r--   0 curtis    (1000) curtis    (1000)     2756 2023-04-29 16:19:18.000000 monoqueue-1.0.1/tests/test_parse.py
```

### Comparing `monoqueue-1.0.0/PKG-INFO` & `monoqueue-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monoqueue
-Version: 1.0.0
+Version: 1.0.1
 Summary: Fight burnout. Stay organized.
 Author-email: Curtis Rueden <ctrueden@wisc.edu>
 License: The Unlicense
 Project-URL: homepage, https://github.com/ctrueden/monoqueue
 Project-URL: documentation, https://github.com/ctrueden/monoqueue/blob/main/README.md
 Project-URL: source, https://github.com/ctrueden/monoqueue
 Project-URL: download, https://pypi.org/project/monoqueue/
```

### Comparing `monoqueue-1.0.0/README.md` & `monoqueue-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `monoqueue-1.0.0/pyproject.toml` & `monoqueue-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "monoqueue"
-version = "1.0.0"
+version = "1.0.1"
 description = "Fight burnout. Stay organized."
 license = {text = "The Unlicense"}
 authors = [{name = "Curtis Rueden", email = "ctrueden@wisc.edu"}]
 readme = "README.md"
 keywords = ["support", "queue"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
```

### Comparing `monoqueue-1.0.0/src/monoqueue/__init__.py` & `monoqueue-1.0.1/src/monoqueue/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     _DEFAULT_METADATA_PATH = Path("~/.local/share/monoqueue/metadata.json").expanduser()
 
     def __init__(self, config: Dict = None):
         if config is None:
             config = configparser.ConfigParser()
             config.read(Monoqueue._DEFAULT_CONFIG_PATH)
         self.config = config
-        self._items = {}
+        self.items = {}
         self._impact = {}
         self._metadata = {}
         self.progress = None
 
         # load rules from config
         self.rules = []
         for k, v in config["rules"].items():
@@ -62,34 +62,34 @@
             self.rules.append((expression, consequence))
         log.debug("Parsed %d rules", len(self.rules))
 
     def load(self,
         items_path: Path = _DEFAULT_ITEMS_PATH,
         metadata_path: Path = _DEFAULT_METADATA_PATH
     ) -> None:
-        self._items = self._load(items_path)
+        self.items = self._load(items_path)
         self._metadata = self._load(metadata_path)
-        if self._items: self._score()
+        if self.items: self._score()
 
     def save(self,
         items_path: Path = _DEFAULT_ITEMS_PATH,
         metadata_path: Path = _DEFAULT_METADATA_PATH
     ) -> None:
-        self._save(self._items, items_path)
+        self._save(self.items, items_path)
         self._save(self._metadata, metadata_path)
 
     def urls(self, active_only=True) -> List[str]:
         """
         Get the list of action item URLs, ordered by impact score.
         """
         urls = []
         urls.extend(
-            (url for url in self._items if self.active(url))
+            (url for url in self.items if self.active(url))
             if active_only
-            else self._items
+            else self.items
         )
         urls.sort(key=lambda url: self.impact(url).value, reverse=True)
         return urls
 
     def update(self) -> None:
         """
         Update the queue from its sources.
@@ -108,15 +108,15 @@
             if not handler in HANDLERS:
                 raise f"Unsupported source type: {handler}"
 
             # Execute the handler's update function.
             update = HANDLERS[handler]
             if update is not None: update(self, config)
 
-            log.debug("Action item count -> %d", len(self._items))
+            log.debug("Action item count -> %d", len(self.items))
 
         # Recalculate item scores.
         self._score()
 
     def item(self, url: str) -> Optional[Dict[str, Any]]:
         """
         Get action item data for the given URL.
@@ -125,15 +125,15 @@
         unlike mq.metadata(url), which is locally managed info.
 
         :param url:
             The URL of the action item data to retrieve.
         :return:
             Information relating to the action item, or None if no such item.
         """
-        return self._items.get(url)
+        return self.items.get(url)
 
     def metadata(self, url: str) -> Dict[str, Any]:
         """
         Get metadata (e.g. deferrals) for the given URL.
 
         Unlike mq.item(url), metadata is managed locally
         rather than being retrieved from remote sources.
@@ -165,15 +165,15 @@
         If it was previously deferred until later, and the deferral
         time has not yet come to pass, then the URL will be inactive.
         :param url:
             The action item URL to check if active.
         :return:
             True if the action item is currently active, False if not.
         """
-        if url not in self._items: return False
+        if url not in self.items: return False
         metadata = self.metadata(url)
         if metadata is None or "deferred_until" not in metadata: return True
 
         item = self.item(url)
         if "deferred_at" in metadata and "updated" in metadata:
             # Check whether item has changed since deferral occurred.
             deferred_at = time.str2dt(metadata["deferred_at"])
@@ -212,27 +212,27 @@
             json.dump(data, f, indent=2)
 
     def _score(self):
         log.debug("Scoring action items...")
 
         # Compute time-sensitive age fields.
         now = time.now()
-        for item in self._items.values():
+        for item in self.items.values():
             if "created" in item:
                 created_age = time.age(item["created"])
                 item["seconds_since_creation"] = created_age.total_seconds()
             if "updated" in item:
                 updated_age = time.age(item["updated"])
                 item["seconds_since_update"] = updated_age.total_seconds()
 
         # Initially, each rule has not applied to any action items.
         unused_rules = set(consequence for _, consequence in self.rules)
 
         self._impact.clear()
-        for url, info in self._items.items():
+        for url, info in self.items.items():
             score_value = 1
             score_rules = []
             for expression, consequence in self.rules:
                 # Try to apply the rule to this action item.
                 applies = evaluate(expression, info)
                 if not applies: continue # Rule does not apply.
```

### Comparing `monoqueue-1.0.0/src/monoqueue/cli.py` & `monoqueue-1.0.1/src/monoqueue/cli.py`

 * *Files identical despite different names*

### Comparing `monoqueue-1.0.0/src/monoqueue/discourse.py` & `monoqueue-1.0.1/src/monoqueue/discourse.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,18 +36,18 @@
 
     search = DiscourseSearch(baseurl=baseurl, username=username, key=key)
     search._progress = mq.progress
     search.download(query)
 
     for topic in search.topics:
         url = f"{baseurl}/t/{topic['id']}"
-        if not url in mq.data:
-            mq.data[url] = {}
+        if not url in mq.items:
+            mq.items[url] = {}
 
-        mq.data[url].update({
+        mq.items[url].update({
             "title": topic["title"],
             "created": topic["created_at"],
             "updated": topic["last_posted_at"],
             "topic": topic
         })
```

### Comparing `monoqueue-1.0.0/src/monoqueue/firefox.py` & `monoqueue-1.0.1/src/monoqueue/firefox.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 
 from . import time
 
 
 def update(mq, config):
     for bookmark in bookmarks(config["folder"]):
         url = bookmark["url"]
-        if not url in mq.data:
-            mq.data[url] = {}
+        if not url in mq.items:
+            mq.items[url] = {}
 
-        mq.data[url].update({
+        mq.items[url].update({
             "title": bookmark["title"],
             "created": bookmark["dateAdded"],
             "updated": bookmark["lastModified"],
             "bookmark": bookmark
         })
```

### Comparing `monoqueue-1.0.0/src/monoqueue/github.py` & `monoqueue-1.0.1/src/monoqueue/github.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,18 +22,18 @@
 
     ghi = GitHubIssues(token=token)
     ghi._progress = mq.progress
     ghi.download(query)
 
     for issue in ghi.issues:
         url = issue["html_url"]
-        if not url in mq.data:
-            mq.data[url] = {}
+        if not url in mq.items:
+            mq.items[url] = {}
 
-        mq.data[url].update({
+        mq.items[url].update({
             "title": issue["title"],
             "created": issue["created_at"],
             "updated": issue["updated_at"],
             "issue": issue
         })
```

### Comparing `monoqueue-1.0.0/src/monoqueue/log.py` & `monoqueue-1.0.1/src/monoqueue/log.py`

 * *Files identical despite different names*

### Comparing `monoqueue-1.0.0/src/monoqueue/parse.py` & `monoqueue-1.0.1/src/monoqueue/parse.py`

 * *Files identical despite different names*

### Comparing `monoqueue-1.0.0/src/monoqueue/time.py` & `monoqueue-1.0.1/src/monoqueue/time.py`

 * *Files identical despite different names*

### Comparing `monoqueue-1.0.0/src/monoqueue/ui.py` & `monoqueue-1.0.1/src/monoqueue/ui.py`

 * *Files identical despite different names*

### Comparing `monoqueue-1.0.0/src/monoqueue.egg-info/PKG-INFO` & `monoqueue-1.0.1/src/monoqueue.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monoqueue
-Version: 1.0.0
+Version: 1.0.1
 Summary: Fight burnout. Stay organized.
 Author-email: Curtis Rueden <ctrueden@wisc.edu>
 License: The Unlicense
 Project-URL: homepage, https://github.com/ctrueden/monoqueue
 Project-URL: documentation, https://github.com/ctrueden/monoqueue/blob/main/README.md
 Project-URL: source, https://github.com/ctrueden/monoqueue
 Project-URL: download, https://pypi.org/project/monoqueue/
```

### Comparing `monoqueue-1.0.0/tests/test_parse.py` & `monoqueue-1.0.1/tests/test_parse.py`

 * *Files identical despite different names*

