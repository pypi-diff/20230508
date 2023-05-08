# Comparing `tmp/pepotron-0.8.0.tar.gz` & `tmp/pepotron-0.9.0.tar.gz`

## Comparing `pepotron-0.8.0.tar` & `pepotron-0.9.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 pepotron-0.8.0/.coveragerc
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 pepotron-0.8.0/.editorconfig
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 pepotron-0.8.0/.flake8
--rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 pepotron-0.8.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 pepotron-0.8.0/RELEASING.md
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 pepotron-0.8.0/tox.ini
--rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 pepotron-0.8.0/.github/labels.yml
--rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 pepotron-0.8.0/.github/release-drafter.yml
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 pepotron-0.8.0/.github/renovate.json
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 pepotron-0.8.0/.github/workflows/deploy.yml
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 pepotron-0.8.0/.github/workflows/labels.yml
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 pepotron-0.8.0/.github/workflows/lint.yml
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 pepotron-0.8.0/.github/workflows/release-drafter.yml
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 pepotron-0.8.0/.github/workflows/require-pr-label.yml
--rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 pepotron-0.8.0/.github/workflows/test.yml
--rw-r--r--   0        0        0     3560 2020-02-02 00:00:00.000000 pepotron-0.8.0/src/pepotron/__init__.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 pepotron-0.8.0/src/pepotron/__main__.py
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 pepotron-0.8.0/src/pepotron/_cache.py
--rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 pepotron-0.8.0/src/pepotron/cli.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pepotron-0.8.0/src/pepotron/scripts/__init__.py
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 pepotron-0.8.0/src/pepotron/scripts/run_command.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pepotron-0.8.0/tests/__init__.py
--rw-r--r--   0        0        0     2898 2020-02-02 00:00:00.000000 pepotron-0.8.0/tests/test_cache.py
--rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 pepotron-0.8.0/tests/test_pepotron.py
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 pepotron-0.8.0/.gitignore
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 pepotron-0.8.0/LICENSE.txt
--rw-r--r--   0        0        0     4224 2020-02-02 00:00:00.000000 pepotron-0.8.0/README.md
--rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 pepotron-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     5750 2020-02-02 00:00:00.000000 pepotron-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 pepotron-0.9.0/.coveragerc
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 pepotron-0.9.0/.editorconfig
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 pepotron-0.9.0/.flake8
+-rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 pepotron-0.9.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 pepotron-0.9.0/RELEASING.md
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 pepotron-0.9.0/tox.ini
+-rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 pepotron-0.9.0/.github/labels.yml
+-rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 pepotron-0.9.0/.github/release-drafter.yml
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 pepotron-0.9.0/.github/renovate.json
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 pepotron-0.9.0/.github/workflows/deploy.yml
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 pepotron-0.9.0/.github/workflows/labels.yml
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 pepotron-0.9.0/.github/workflows/lint.yml
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 pepotron-0.9.0/.github/workflows/release-drafter.yml
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 pepotron-0.9.0/.github/workflows/require-pr-label.yml
+-rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 pepotron-0.9.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0     3583 2020-02-02 00:00:00.000000 pepotron-0.9.0/src/pepotron/__init__.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 pepotron-0.9.0/src/pepotron/__main__.py
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 pepotron-0.9.0/src/pepotron/_cache.py
+-rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 pepotron-0.9.0/src/pepotron/cli.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pepotron-0.9.0/src/pepotron/scripts/__init__.py
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 pepotron-0.9.0/src/pepotron/scripts/run_command.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pepotron-0.9.0/tests/__init__.py
+-rw-r--r--   0        0        0     2898 2020-02-02 00:00:00.000000 pepotron-0.9.0/tests/test_cache.py
+-rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 pepotron-0.9.0/tests/test_pepotron.py
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 pepotron-0.9.0/.gitignore
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 pepotron-0.9.0/LICENSE.txt
+-rw-r--r--   0        0        0     4733 2020-02-02 00:00:00.000000 pepotron-0.9.0/README.md
+-rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 pepotron-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     6259 2020-02-02 00:00:00.000000 pepotron-0.9.0/PKG-INFO
```

### Comparing `pepotron-0.8.0/.pre-commit-config.yaml` & `pepotron-0.9.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pepotron-0.8.0/RELEASING.md` & `pepotron-0.9.0/RELEASING.md`

 * *Files identical despite different names*

### Comparing `pepotron-0.8.0/.github/labels.yml` & `pepotron-0.9.0/.github/labels.yml`

 * *Files identical despite different names*

### Comparing `pepotron-0.8.0/.github/release-drafter.yml` & `pepotron-0.9.0/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `pepotron-0.8.0/.github/workflows/deploy.yml` & `pepotron-0.9.0/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `pepotron-0.8.0/.github/workflows/release-drafter.yml` & `pepotron-0.9.0/.github/workflows/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `pepotron-0.8.0/.github/workflows/test.yml` & `pepotron-0.9.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `pepotron-0.8.0/src/pepotron/__init__.py` & `pepotron-0.9.0/src/pepotron/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -102,33 +102,35 @@
 def pep_url(search: str | None, base_url: str = BASE_URL, pr: int | None = None) -> str:
     """Get PEP URL"""
     if pr:
         base_url = f"https://pep-previews--{pr}.org.readthedocs.build"
 
     result = base_url.rstrip("/")
 
-    if search:
-        if search.lower() in TOPICS:
-            result += f"/topic/{search}/"
-            return result
+    if not search:
+        return result
 
-        try:
-            # pep 8
-            number = int(search)
-        except ValueError:
-            try:
-                # pep 3.11
-                number = VERSION_TO_PEP[search]
-            except KeyError:
-                # pep "dead batteries"
-                number = word_search(search)
+    if search.lower() in ("topic", "topics"):
+        return result + "/topic/"
+
+    if search.lower() in TOPICS:
+        return result + f"/topic/{search}/"
 
-        result += f"/pep-{number:0>4}/"
+    try:
+        # pep 8
+        number = int(search)
+    except ValueError:
+        try:
+            # pep 3.11
+            number = VERSION_TO_PEP[search]
+        except KeyError:
+            # pep "dead batteries"
+            number = word_search(search)
 
-    return result
+    return result + f"/pep-{number:0>4}/"
 
 
 def open_pep(
     search: str, base_url: str = BASE_URL, pr: int | None = None, dry_run: bool = False
 ) -> str:
     """Open this PEP in the browser"""
     url = pep_url(search, base_url, pr)
```

### Comparing `pepotron-0.8.0/src/pepotron/_cache.py` & `pepotron-0.9.0/src/pepotron/_cache.py`

 * *Files identical despite different names*

### Comparing `pepotron-0.8.0/src/pepotron/cli.py` & `pepotron-0.9.0/src/pepotron/cli.py`

 * *Files identical despite different names*

### Comparing `pepotron-0.8.0/src/pepotron/scripts/run_command.py` & `pepotron-0.9.0/src/pepotron/scripts/run_command.py`

 * *Files identical despite different names*

### Comparing `pepotron-0.8.0/tests/test_cache.py` & `pepotron-0.9.0/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `pepotron-0.8.0/tests/test_pepotron.py` & `pepotron-0.9.0/tests/test_pepotron.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,14 +14,16 @@
         ("8", "https://peps.python.org/pep-0008/"),
         ("12", "https://peps.python.org/pep-0012/"),
         ("2.7", "https://peps.python.org/pep-0373/"),
         (None, "https://peps.python.org"),
         ("dead batteries", "https://peps.python.org/pep-0594/"),
         ("release", "https://peps.python.org/topic/release/"),
         ("typing", "https://peps.python.org/topic/typing/"),
+        ("topics", "https://peps.python.org/topic/"),
+        ("topic", "https://peps.python.org/topic/"),
     ],
 )
 def test_url(search: str, expected_url: str) -> None:
     # Act
     pep_url = pepotron.pep_url(search)
     # Assert
     assert pep_url == expected_url
```

### Comparing `pepotron-0.8.0/.gitignore` & `pepotron-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pepotron-0.8.0/LICENSE.txt` & `pepotron-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pepotron-0.8.0/README.md` & `pepotron-0.9.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -86,14 +86,50 @@
 ```console
 $ pep governance
 https://peps.python.org/topic/governance/
 ```
 
 <!-- [[[end]]] -->
 
+<!-- [[[cog run("pep packaging") ]]] -->
+
+```console
+$ pep packaging
+https://peps.python.org/topic/packaging/
+```
+
+<!-- [[[end]]] -->
+
+<!-- [[[cog run("pep release") ]]] -->
+
+```console
+$ pep release
+https://peps.python.org/topic/release/
+```
+
+<!-- [[[end]]] -->
+
+<!-- [[[cog run("pep typing") ]]] -->
+
+```console
+$ pep typing
+https://peps.python.org/topic/typing/
+```
+
+<!-- [[[end]]] -->
+
+<!-- [[[cog run("pep topics") ]]] -->
+
+```console
+$ pep topics
+https://peps.python.org/topic/
+```
+
+<!-- [[[end]]] -->
+
 ### Open a build preview of a python/peps PR
 
 <!-- [[[cog run("pep 594 --pr 2440") ]]] -->
 
 ```console
 $ pep 594 --pr 2440
 https://pep-previews--2440.org.readthedocs.build/pep-0594/
```

### Comparing `pepotron-0.8.0/pyproject.toml` & `pepotron-0.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pepotron-0.8.0/PKG-INFO` & `pepotron-0.9.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pepotron
-Version: 0.8.0
+Version: 0.9.0
 Summary: CLI to open PEPs in your browser
 Project-URL: Changelog, https://github.com/hugovk/pepotron/releases
 Project-URL: Homepage, https://github.com/hugovk/pepotron
 Project-URL: Source, https://github.com/hugovk/pepotron
 Author: Hugo van Kemenade
 License: MIT
 License-File: LICENSE.txt
@@ -124,14 +124,50 @@
 ```console
 $ pep governance
 https://peps.python.org/topic/governance/
 ```
 
 <!-- [[[end]]] -->
 
+<!-- [[[cog run("pep packaging") ]]] -->
+
+```console
+$ pep packaging
+https://peps.python.org/topic/packaging/
+```
+
+<!-- [[[end]]] -->
+
+<!-- [[[cog run("pep release") ]]] -->
+
+```console
+$ pep release
+https://peps.python.org/topic/release/
+```
+
+<!-- [[[end]]] -->
+
+<!-- [[[cog run("pep typing") ]]] -->
+
+```console
+$ pep typing
+https://peps.python.org/topic/typing/
+```
+
+<!-- [[[end]]] -->
+
+<!-- [[[cog run("pep topics") ]]] -->
+
+```console
+$ pep topics
+https://peps.python.org/topic/
+```
+
+<!-- [[[end]]] -->
+
 ### Open a build preview of a python/peps PR
 
 <!-- [[[cog run("pep 594 --pr 2440") ]]] -->
 
 ```console
 $ pep 594 --pr 2440
 https://pep-previews--2440.org.readthedocs.build/pep-0594/
```

