# Comparing `tmp/idf-build-apps-0.6.0.tar.gz` & `tmp/idf-build-apps-0.6.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idf-build-apps-0.6.0.tar", last modified: Mon May  8 05:24:22 2023, max compression
+gzip compressed data, was "idf-build-apps-0.6.0rc0.tar", last modified: Thu Apr 13 04:29:49 2023, max compression
```

## Comparing `idf-build-apps-0.6.0.tar` & `idf-build-apps-0.6.0rc0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0      351 2023-05-08 05:24:15.121875 idf-build-apps-0.6.0/.editorconfig
--rw-r--r--   0        0        0      123 2023-05-08 05:24:15.121875 idf-build-apps-0.6.0/.git-blame-ignore-revs
--rw-r--r--   0        0        0       25 2023-05-08 05:24:15.121875 idf-build-apps-0.6.0/.gitattributes
--rw-r--r--   0        0        0      253 2023-05-08 05:24:15.121875 idf-build-apps-0.6.0/.github/workflows/check-pre-commit.yml
--rw-r--r--   0        0        0      675 2023-05-08 05:24:15.121875 idf-build-apps-0.6.0/.github/workflows/issue_comment.yml
--rw-r--r--   0        0        0      620 2023-05-08 05:24:15.121875 idf-build-apps-0.6.0/.github/workflows/new_issues.yml
--rw-r--r--   0        0        0      796 2023-05-08 05:24:15.121875 idf-build-apps-0.6.0/.github/workflows/new_prs.yml
--rw-r--r--   0        0        0      438 2023-05-08 05:24:15.121875 idf-build-apps-0.6.0/.github/workflows/publish-pypi.yml
--rw-r--r--   0        0        0      521 2023-05-08 05:24:15.121875 idf-build-apps-0.6.0/.github/workflows/test-build-docs.yml
--rw-r--r--   0        0        0     3707 2023-05-08 05:24:15.121875 idf-build-apps-0.6.0/.github/workflows/test-build-idf-apps.yml
--rw-r--r--   0        0        0     3076 2023-05-08 05:24:15.121875 idf-build-apps-0.6.0/.gitignore
--rw-r--r--   0        0        0     1077 2023-05-08 05:24:15.121875 idf-build-apps-0.6.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      383 2023-05-08 05:24:15.121875 idf-build-apps-0.6.0/.readthedocs.yml
--rw-r--r--   0        0        0     4013 2023-05-08 05:24:15.121875 idf-build-apps-0.6.0/CHANGELOG.md
--rw-r--r--   0        0        0     1834 2023-05-08 05:24:15.121875 idf-build-apps-0.6.0/CONTRIBUTING.md
--rw-r--r--   0        0        0    11358 2023-05-08 05:24:15.121875 idf-build-apps-0.6.0/LICENSE
--rw-r--r--   0        0        0     3843 2023-05-08 05:24:15.125875 idf-build-apps-0.6.0/README.md
--rw-r--r--   0        0        0       33 2023-05-08 05:24:15.125875 idf-build-apps-0.6.0/docs/CHANGELOG.md
--rw-r--r--   0        0        0       36 2023-05-08 05:24:15.125875 idf-build-apps-0.6.0/docs/CONTRIBUTING.md
--rw-r--r--   0        0        0      634 2023-05-08 05:24:15.125875 idf-build-apps-0.6.0/docs/Makefile
--rw-r--r--   0        0        0     6947 2023-05-08 05:24:15.125875 idf-build-apps-0.6.0/docs/_static/espressif-logo.svg
--rw-r--r--   0        0        0      942 2023-05-08 05:24:15.125875 idf-build-apps-0.6.0/docs/_static/theme_overrides.css
--rw-r--r--   0        0        0      119 2023-05-08 05:24:15.125875 idf-build-apps-0.6.0/docs/_templates/layout.html
--rw-r--r--   0        0        0      490 2023-05-08 05:24:15.125875 idf-build-apps-0.6.0/docs/api.rst
--rw-r--r--   0        0        0     1449 2023-05-08 05:24:15.125875 idf-build-apps-0.6.0/docs/conf.py
--rw-r--r--   0        0        0     2652 2023-05-08 05:24:15.125875 idf-build-apps-0.6.0/docs/config_file.md
--rw-r--r--   0        0        0    10368 2023-05-08 05:24:15.125875 idf-build-apps-0.6.0/docs/find_build.md
--rw-r--r--   0        0        0      474 2023-05-08 05:24:15.125875 idf-build-apps-0.6.0/docs/index.rst
--rw-r--r--   0        0        0     3651 2023-05-08 05:24:15.125875 idf-build-apps-0.6.0/docs/manifest.md
--rw-r--r--   0        0        0      481 2023-05-08 05:24:15.125875 idf-build-apps-0.6.0/idf_build_apps/__init__.py
--rw-r--r--   0        0        0      182 2023-05-08 05:24:15.125875 idf-build-apps-0.6.0/idf_build_apps/__main__.py
--rw-r--r--   0        0        0    22146 2023-05-08 05:24:15.125875 idf-build-apps-0.6.0/idf_build_apps/app.py
--rw-r--r--   0        0        0     2768 2023-05-08 05:24:15.125875 idf-build-apps-0.6.0/idf_build_apps/config.py
--rw-r--r--   0        0        0     2187 2023-05-08 05:24:15.125875 idf-build-apps-0.6.0/idf_build_apps/constants.py
--rw-r--r--   0        0        0     6026 2023-05-08 05:24:15.125875 idf-build-apps-0.6.0/idf_build_apps/finder.py
--rw-r--r--   0        0        0     2220 2023-05-08 05:24:15.125875 idf-build-apps-0.6.0/idf_build_apps/log.py
--rw-r--r--   0        0        0    31784 2023-05-08 05:24:15.125875 idf-build-apps-0.6.0/idf_build_apps/main.py
--rw-r--r--   0        0        0      133 2023-05-08 05:24:15.125875 idf-build-apps-0.6.0/idf_build_apps/manifest/__init__.py
--rw-r--r--   0        0        0     6144 2023-05-08 05:24:15.125875 idf-build-apps-0.6.0/idf_build_apps/manifest/if_parser.py
--rw-r--r--   0        0        0     5695 2023-05-08 05:24:15.125875 idf-build-apps-0.6.0/idf_build_apps/manifest/manifest.py
--rw-r--r--   0        0        0     3423 2023-05-08 05:24:15.125875 idf-build-apps-0.6.0/idf_build_apps/manifest/soc_header.py
--rw-r--r--   0        0        0     6577 2023-05-08 05:24:15.125875 idf-build-apps-0.6.0/idf_build_apps/utils.py
--rw-r--r--   0        0        0      101 2023-05-08 05:24:15.125875 idf-build-apps-0.6.0/license_header.txt
--rw-r--r--   0        0        0     1860 2023-05-08 05:24:15.125875 idf-build-apps-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     1221 2023-05-08 05:24:15.125875 idf-build-apps-0.6.0/tests/conftest.py
--rw-r--r--   0        0        0     2181 2023-05-08 05:24:15.125875 idf-build-apps-0.6.0/tests/test_build.py
--rw-r--r--   0        0        0    10242 2023-05-08 05:24:15.125875 idf-build-apps-0.6.0/tests/test_finder.py
--rw-r--r--   0        0        0      995 2023-05-08 05:24:15.125875 idf-build-apps-0.6.0/tests/test_manifest.py
--rw-r--r--   0        0        0     2394 2023-05-08 05:24:15.125875 idf-build-apps-0.6.0/tests/test_utils.py
--rw-r--r--   0        0        0     1066 1970-01-01 00:00:00.000000 idf-build-apps-0.6.0/setup.py
--rw-r--r--   0        0        0     5473 1970-01-01 00:00:00.000000 idf-build-apps-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0      351 2023-04-13 04:29:42.130566 idf-build-apps-0.6.0rc0/.editorconfig
+-rw-r--r--   0        0        0      123 2023-04-13 04:29:42.130566 idf-build-apps-0.6.0rc0/.git-blame-ignore-revs
+-rw-r--r--   0        0        0       25 2023-04-13 04:29:42.130566 idf-build-apps-0.6.0rc0/.gitattributes
+-rw-r--r--   0        0        0      253 2023-04-13 04:29:42.130566 idf-build-apps-0.6.0rc0/.github/workflows/check-pre-commit.yml
+-rw-r--r--   0        0        0      675 2023-04-13 04:29:42.130566 idf-build-apps-0.6.0rc0/.github/workflows/issue_comment.yml
+-rw-r--r--   0        0        0      620 2023-04-13 04:29:42.130566 idf-build-apps-0.6.0rc0/.github/workflows/new_issues.yml
+-rw-r--r--   0        0        0      796 2023-04-13 04:29:42.130566 idf-build-apps-0.6.0rc0/.github/workflows/new_prs.yml
+-rw-r--r--   0        0        0      438 2023-04-13 04:29:42.130566 idf-build-apps-0.6.0rc0/.github/workflows/publish-pypi.yml
+-rw-r--r--   0        0        0      521 2023-04-13 04:29:42.130566 idf-build-apps-0.6.0rc0/.github/workflows/test-build-docs.yml
+-rw-r--r--   0        0        0     3707 2023-04-13 04:29:42.130566 idf-build-apps-0.6.0rc0/.github/workflows/test-build-idf-apps.yml
+-rw-r--r--   0        0        0     3076 2023-04-13 04:29:42.130566 idf-build-apps-0.6.0rc0/.gitignore
+-rw-r--r--   0        0        0     1077 2023-04-13 04:29:42.130566 idf-build-apps-0.6.0rc0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      383 2023-04-13 04:29:42.130566 idf-build-apps-0.6.0rc0/.readthedocs.yml
+-rw-r--r--   0        0        0     3562 2023-04-13 04:29:42.130566 idf-build-apps-0.6.0rc0/CHANGELOG.md
+-rw-r--r--   0        0        0     1834 2023-04-13 04:29:42.130566 idf-build-apps-0.6.0rc0/CONTRIBUTING.md
+-rw-r--r--   0        0        0    11358 2023-04-13 04:29:42.130566 idf-build-apps-0.6.0rc0/LICENSE
+-rw-r--r--   0        0        0     3843 2023-04-13 04:29:42.130566 idf-build-apps-0.6.0rc0/README.md
+-rw-r--r--   0        0        0       33 2023-04-13 04:29:42.130566 idf-build-apps-0.6.0rc0/docs/CHANGELOG.md
+-rw-r--r--   0        0        0       36 2023-04-13 04:29:42.130566 idf-build-apps-0.6.0rc0/docs/CONTRIBUTING.md
+-rw-r--r--   0        0        0      634 2023-04-13 04:29:42.130566 idf-build-apps-0.6.0rc0/docs/Makefile
+-rw-r--r--   0        0        0     6947 2023-04-13 04:29:42.130566 idf-build-apps-0.6.0rc0/docs/_static/espressif-logo.svg
+-rw-r--r--   0        0        0      942 2023-04-13 04:29:42.130566 idf-build-apps-0.6.0rc0/docs/_static/theme_overrides.css
+-rw-r--r--   0        0        0      119 2023-04-13 04:29:42.130566 idf-build-apps-0.6.0rc0/docs/_templates/layout.html
+-rw-r--r--   0        0        0      490 2023-04-13 04:29:42.130566 idf-build-apps-0.6.0rc0/docs/api.rst
+-rw-r--r--   0        0        0     1449 2023-04-13 04:29:42.130566 idf-build-apps-0.6.0rc0/docs/conf.py
+-rw-r--r--   0        0        0     2652 2023-04-13 04:29:42.130566 idf-build-apps-0.6.0rc0/docs/config_file.md
+-rw-r--r--   0        0        0    10368 2023-04-13 04:29:42.130566 idf-build-apps-0.6.0rc0/docs/find_build.md
+-rw-r--r--   0        0        0      474 2023-04-13 04:29:42.134566 idf-build-apps-0.6.0rc0/docs/index.rst
+-rw-r--r--   0        0        0     3651 2023-04-13 04:29:42.134566 idf-build-apps-0.6.0rc0/docs/manifest.md
+-rw-r--r--   0        0        0      487 2023-04-13 04:29:42.134566 idf-build-apps-0.6.0rc0/idf_build_apps/__init__.py
+-rw-r--r--   0        0        0      182 2023-04-13 04:29:42.134566 idf-build-apps-0.6.0rc0/idf_build_apps/__main__.py
+-rw-r--r--   0        0        0    21914 2023-04-13 04:29:42.134566 idf-build-apps-0.6.0rc0/idf_build_apps/app.py
+-rw-r--r--   0        0        0     2768 2023-04-13 04:29:42.134566 idf-build-apps-0.6.0rc0/idf_build_apps/config.py
+-rw-r--r--   0        0        0     2187 2023-04-13 04:29:42.134566 idf-build-apps-0.6.0rc0/idf_build_apps/constants.py
+-rw-r--r--   0        0        0     6026 2023-04-13 04:29:42.134566 idf-build-apps-0.6.0rc0/idf_build_apps/finder.py
+-rw-r--r--   0        0        0     1359 2023-04-13 04:29:42.134566 idf-build-apps-0.6.0rc0/idf_build_apps/log.py
+-rw-r--r--   0        0        0    28666 2023-04-13 04:29:42.134566 idf-build-apps-0.6.0rc0/idf_build_apps/main.py
+-rw-r--r--   0        0        0      133 2023-04-13 04:29:42.134566 idf-build-apps-0.6.0rc0/idf_build_apps/manifest/__init__.py
+-rw-r--r--   0        0        0     5547 2023-04-13 04:29:42.134566 idf-build-apps-0.6.0rc0/idf_build_apps/manifest/if_parser.py
+-rw-r--r--   0        0        0     5322 2023-04-13 04:29:42.134566 idf-build-apps-0.6.0rc0/idf_build_apps/manifest/manifest.py
+-rw-r--r--   0        0        0     3423 2023-04-13 04:29:42.134566 idf-build-apps-0.6.0rc0/idf_build_apps/manifest/soc_header.py
+-rw-r--r--   0        0        0     7473 2023-04-13 04:29:42.134566 idf-build-apps-0.6.0rc0/idf_build_apps/utils.py
+-rw-r--r--   0        0        0      101 2023-04-13 04:29:42.134566 idf-build-apps-0.6.0rc0/license_header.txt
+-rw-r--r--   0        0        0     1860 2023-04-13 04:29:42.134566 idf-build-apps-0.6.0rc0/pyproject.toml
+-rw-r--r--   0        0        0     1221 2023-04-13 04:29:42.134566 idf-build-apps-0.6.0rc0/tests/conftest.py
+-rw-r--r--   0        0        0     2181 2023-04-13 04:29:42.134566 idf-build-apps-0.6.0rc0/tests/test_build.py
+-rw-r--r--   0        0        0     7948 2023-04-13 04:29:42.134566 idf-build-apps-0.6.0rc0/tests/test_finder.py
+-rw-r--r--   0        0        0      995 2023-04-13 04:29:42.134566 idf-build-apps-0.6.0rc0/tests/test_manifest.py
+-rw-r--r--   0        0        0     2394 2023-04-13 04:29:42.134566 idf-build-apps-0.6.0rc0/tests/test_utils.py
+-rw-r--r--   0        0        0     1069 1970-01-01 00:00:00.000000 idf-build-apps-0.6.0rc0/setup.py
+-rw-r--r--   0        0        0     5476 1970-01-01 00:00:00.000000 idf-build-apps-0.6.0rc0/PKG-INFO
```

### Comparing `idf-build-apps-0.6.0/.github/workflows/issue_comment.yml` & `idf-build-apps-0.6.0rc0/.github/workflows/issue_comment.yml`

 * *Files identical despite different names*

### Comparing `idf-build-apps-0.6.0/.github/workflows/new_issues.yml` & `idf-build-apps-0.6.0rc0/.github/workflows/new_issues.yml`

 * *Files identical despite different names*

### Comparing `idf-build-apps-0.6.0/.github/workflows/new_prs.yml` & `idf-build-apps-0.6.0rc0/.github/workflows/new_prs.yml`

 * *Files identical despite different names*

### Comparing `idf-build-apps-0.6.0/.github/workflows/test-build-docs.yml` & `idf-build-apps-0.6.0rc0/.github/workflows/test-build-docs.yml`

 * *Files identical despite different names*

### Comparing `idf-build-apps-0.6.0/.github/workflows/test-build-idf-apps.yml` & `idf-build-apps-0.6.0rc0/.github/workflows/test-build-idf-apps.yml`

 * *Files identical despite different names*

### Comparing `idf-build-apps-0.6.0/.gitignore` & `idf-build-apps-0.6.0rc0/.gitignore`

 * *Files identical despite different names*

### Comparing `idf-build-apps-0.6.0/.pre-commit-config.yaml` & `idf-build-apps-0.6.0rc0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `idf-build-apps-0.6.0/CONTRIBUTING.md` & `idf-build-apps-0.6.0rc0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `idf-build-apps-0.6.0/LICENSE` & `idf-build-apps-0.6.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `idf-build-apps-0.6.0/README.md` & `idf-build-apps-0.6.0rc0/README.md`

 * *Files identical despite different names*

### Comparing `idf-build-apps-0.6.0/docs/Makefile` & `idf-build-apps-0.6.0rc0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `idf-build-apps-0.6.0/docs/_static/espressif-logo.svg` & `idf-build-apps-0.6.0rc0/docs/_static/espressif-logo.svg`

 * *Files identical despite different names*

### Comparing `idf-build-apps-0.6.0/docs/_static/theme_overrides.css` & `idf-build-apps-0.6.0rc0/docs/_static/theme_overrides.css`

 * *Files identical despite different names*

### Comparing `idf-build-apps-0.6.0/docs/conf.py` & `idf-build-apps-0.6.0rc0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `idf-build-apps-0.6.0/docs/config_file.md` & `idf-build-apps-0.6.0rc0/docs/config_file.md`

 * *Files identical despite different names*

### Comparing `idf-build-apps-0.6.0/docs/find_build.md` & `idf-build-apps-0.6.0rc0/docs/find_build.md`

 * *Files identical despite different names*

### Comparing `idf-build-apps-0.6.0/docs/manifest.md` & `idf-build-apps-0.6.0rc0/docs/manifest.md`

 * *Files identical despite different names*

### Comparing `idf-build-apps-0.6.0/idf_build_apps/app.py` & `idf-build-apps-0.6.0rc0/idf_build_apps/app.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,15 +51,14 @@
 
 class App(object):
     TARGET_PLACEHOLDER = '@t'  # replace it with self.target
     WILDCARD_PLACEHOLDER = '@w'  # replace it with the wildcard, usually the sdkconfig
     NAME_PLACEHOLDER = '@n'  # replace it with self.name
     FULL_NAME_PLACEHOLDER = '@f'  # replace it with escaped self.app_dir
     INDEX_PLACEHOLDER = '@i'  # replace it with the build index
-    PARALLEL_INDEX_PLACEHOLDER = '@p'  # replace it with the parallel index
 
     BUILD_SYSTEM = 'unknown'
 
     SDKCONFIG_LINE_REGEX = re.compile(r"^([^=]+)=\"?([^\"\n]*)\"?\n*$")
 
     # could be assigned later, used for filtering out apps by supported_targets
     MANIFEST = None  # type: Manifest | None
@@ -100,19 +99,14 @@
         self.check_warnings = check_warnings
         self.preserve = preserve
 
         # Some miscellaneous build properties which are set later, at the build stage
         self.dry_run = False
         self.index = None
         self.verbose = False
-        self.parallel_index = 1
-        self.parallel_count = 1
-
-        self._collect_app_info = None
-        self._collect_size_info = None
 
         # sdkconfig attrs, use properties instead
         self._sdkconfig_defaults = self._get_sdkconfig_defaults(sdkconfig_defaults_str)
         self._sdkconfig_files = None
         self._sdkconfig_files_defined_target = None
 
         self._process_sdkconfig_files()
@@ -184,15 +178,14 @@
         Internal method, expands any of the placeholders in {app,work,build} paths.
         """
         if not path:
             return path
 
         if self.index is not None:
             path = path.replace(self.INDEX_PLACEHOLDER, str(self.index))
-        path = path.replace(self.PARALLEL_INDEX_PLACEHOLDER, str(self.parallel_index))
         path = path.replace(self.TARGET_PLACEHOLDER, self.target)
         path = path.replace(self.NAME_PLACEHOLDER, self.name)
         if self.FULL_NAME_PLACEHOLDER in path:  # to avoid recursion to the call to app_dir in the next line:
             path = path.replace(self.FULL_NAME_PLACEHOLDER, self.app_dir.replace(os.path.sep, '_'))
         wildcard_pos = path.find(self.WILDCARD_PLACEHOLDER)
         if wildcard_pos != -1:
             if self.config_name:
@@ -245,28 +238,14 @@
     @property
     def size_json_path(self):
         if self._size_json_path:
             return os.path.join(self.build_path, self._expand(self._size_json_path))
 
         return None
 
-    @property
-    def collect_app_info(self):
-        if self._collect_app_info:
-            return self._expand(self._collect_app_info)
-
-        return None
-
-    @property
-    def collect_size_info(self):
-        if self._collect_size_info:
-            return self._expand(self._collect_size_info)
-
-        return None
-
     def _process_sdkconfig_files(self):
         """
         Expand environment variables in default sdkconfig files and remove some CI
         related settings.
         """
         res = []
 
@@ -351,29 +330,25 @@
             return self.MANIFEST.requires_components(self.app_dir)
 
         return []
 
     @property
     def supported_targets(self):
         if self.MANIFEST:
-            return self.MANIFEST.enable_build_targets(
-                self.app_dir, self.sdkconfig_files_defined_idf_target, self.config_name
-            )
+            return self.MANIFEST.enable_build_targets(self.app_dir, self.sdkconfig_files_defined_idf_target)
 
         if self.sdkconfig_files_defined_idf_target:
             return [self.sdkconfig_files_defined_idf_target]
 
         return FolderRule.DEFAULT_BUILD_TARGETS
 
     @property
     def verified_targets(self):
         if self.MANIFEST:
-            return self.MANIFEST.enable_test_targets(
-                self.app_dir, self.sdkconfig_files_defined_idf_target, self.config_name
-            )
+            return self.MANIFEST.enable_test_targets(self.app_dir, self.sdkconfig_files_defined_idf_target)
 
         return []
 
     @abstractmethod
     def build(
         self,
         depends_on_components=None,  # type: list[str] | str | None
@@ -403,14 +378,27 @@
                     map_file,
                 ]
             ),
             check=True,
         )
         LOGGER.info('=> Generated size info to %s', self.size_json_path)
 
+    def collect_size_info(self, output_fs):  # type: (t.TextIO) -> None
+        if not os.path.isfile(self.size_json_path):
+            self.write_size_json()
+
+        size_info_dict = {
+            'app_name': self.name,
+            'config_name': self.config_name,
+            'target': self.target,
+            'path': self.size_json_path,
+        }
+        output_fs.write(json.dumps(size_info_dict) + '\n')
+        LOGGER.info('=> Recorded size info file path in %s', output_fs.name)
+
     def to_json(self):
         # keeping backward compatibility, only provide these stuffs
         return json.dumps(
             {
                 'build_system': self.BUILD_SYSTEM,
                 'app_dir': self.app_dir,
                 'work_dir': self.work_dir,
```

### Comparing `idf-build-apps-0.6.0/idf_build_apps/config.py` & `idf-build-apps-0.6.0rc0/idf_build_apps/config.py`

 * *Files identical despite different names*

### Comparing `idf-build-apps-0.6.0/idf_build_apps/constants.py` & `idf-build-apps-0.6.0rc0/idf_build_apps/constants.py`

 * *Files identical despite different names*

### Comparing `idf-build-apps-0.6.0/idf_build_apps/finder.py` & `idf-build-apps-0.6.0rc0/idf_build_apps/finder.py`

 * *Files identical despite different names*

### Comparing `idf-build-apps-0.6.0/idf_build_apps/main.py` & `idf-build-apps-0.6.0rc0/idf_build_apps/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 # SPDX-FileCopyrightText: 2022-2023 Espressif Systems (Shanghai) CO LTD
 # SPDX-License-Identifier: Apache-2.0
 
 import argparse
-import io
-import json
 import os
 import re
 import shutil
 import sys
 import textwrap
-import warnings
 from pathlib import (
     Path,
 )
 
 from . import (
     LOGGER,
 )
@@ -25,26 +22,24 @@
 )
 from .constants import (
     ALL_TARGETS,
 )
 from .finder import (
     _find_apps,
 )
-from .log import (
-    setup_logging,
-)
 from .manifest.manifest import (
     FolderRule,
     Manifest,
 )
 from .utils import (
     BuildError,
     InvalidCommand,
     files_matches_patterns,
     get_parallel_start_stop,
+    setup_logging,
     to_list,
 )
 
 try:
     import typing as t
 except ImportError:
     pass
@@ -192,16 +187,16 @@
 def build_apps(
     apps,  # type: list[App] | App
     build_verbose=False,  # type: bool
     parallel_count=1,  # type: int
     parallel_index=1,  # type: int
     dry_run=False,  # type: bool
     keep_going=False,  # type: bool
-    collect_size_info=None,  # type: str | t.TextIO | None
-    collect_app_info=None,  # type: str | t.TextIO | None
+    collect_size_info=None,  # type: t.TextIO | None
+    collect_app_info=None,  # type: t.TextIO | None
     ignore_warning_strs=None,  # type: list[str] | None
     ignore_warning_file=None,  # type: t.TextIO | None
     copy_sdkconfig=False,  # type: bool
     depends_on_components=None,  # type: list[str] | str | None
     manifest_rootpath=None,  # type: str | None
     ignore_component_dependencies_file_patterns=None,  # type: list[str] | str | None
     depends_on_files=None,  # type: list[str] | str | None
@@ -245,15 +240,15 @@
         ``ignore_component_dependencies_file_patterns``
     :type depends_on_files: list[str] | str | None
     :return: exit_code, built_apps if specified ``depends_on_components``
     :rtype: int, list[App]
     :return: exit_code if not specified ``depends_on_components``
     :rtype: int
     """
-    apps = to_list(apps)  # type: list[App]
+    apps = to_list(apps)
 
     ignore_warnings_regexes = []
     if ignore_warning_strs:
         for s in ignore_warning_strs:
             ignore_warnings_regexes.append(re.compile(s))
     if ignore_warning_file:
         for s in ignore_warning_file:
@@ -289,52 +284,14 @@
     LOGGER.info('Building the following apps:')
     if apps[start - 1 : stop]:
         for app in apps[start - 1 : stop]:
             LOGGER.info('  %s (preserve: %s)', app, app.preserve)
     else:
         LOGGER.info('  parallel count is too large. build nothing...')
 
-    # cleanup collect files if exists at this early-stage
-    collect_files = []
-    for app in apps[start - 1 : stop]:  # we use 1-based
-        app.parallel_index = parallel_index
-        app.parallel_count = parallel_count
-
-        if collect_app_info:
-            if isinstance(collect_app_info, io.TextIOWrapper):
-                warnings.warn(
-                    '"collect_app_info" does not support file stream in idf-build-apps 1.0.0, Please use str instead',
-                    DeprecationWarning,
-                )
-                app._collect_app_info = collect_app_info.name
-            else:
-                app._collect_app_info = collect_app_info
-
-            if app.collect_app_info not in collect_files:
-                collect_files.append(app.collect_app_info)
-
-        if collect_size_info:
-            if isinstance(collect_size_info, io.TextIOWrapper):
-                warnings.warn(
-                    '"collect_size_info" does not support file stream in idf-build-apps 1.0.0, Please use str instead',
-                    DeprecationWarning,
-                )
-                app._collect_size_info = collect_size_info.name
-            else:
-                app._collect_size_info = collect_size_info
-
-            if app.collect_size_info not in collect_files:
-                collect_files.append(app.collect_size_info)
-
-    for f in collect_files:
-        if os.path.isfile(f):
-            os.remove(f)
-            LOGGER.info('=> Remove existing collect file %s', f)
-        Path(f).touch()
-
     actual_built_apps = []
     for i, app in enumerate(apps):
         index = i + 1  # we use 1-based
         if index < start or index > stop:
             continue
 
         # attrs
@@ -359,40 +316,25 @@
                     return 1, actual_built_apps
                 else:
                     return 1
         finally:
             if is_built:
                 actual_built_apps.append(app)
 
-                if app.collect_app_info:
-                    with open(app.collect_app_info, 'a') as fw:
-                        fw.write(app.to_json() + '\n')
-                    LOGGER.info('=> Recorded app info in %s', app.collect_app_info)
+                if collect_app_info:
+                    collect_app_info.write(app.to_json() + '\n')
+                    LOGGER.info('=> Recorded app info in %s', collect_app_info.name)
 
-                if app.collect_size_info and app.size_json_path:
+                if collect_size_info:
                     try:
-                        if not os.path.isfile(app.size_json_path):
-                            app.write_size_json()
+                        app.collect_size_info(collect_size_info)
                     except Exception as e:
                         LOGGER.warning('Adding size info for app %s failed:', app.name)
                         LOGGER.warning(e)
-                    else:
-                        with open(app.collect_size_info, 'a') as fw:
-                            fw.write(
-                                json.dumps(
-                                    {
-                                        'app_name': app.name,
-                                        'config_name': app.config_name,
-                                        'target': app.target,
-                                        'path': app.size_json_path,
-                                    }
-                                )
-                                + '\n'
-                            )
-                        LOGGER.info('=> Recorded size info file path in %s', app.collect_size_info)
+                        pass
 
                 if copy_sdkconfig:
                     try:
                         shutil.copy(
                             os.path.join(app.work_dir, 'sdkconfig'),
                             os.path.join(app.build_path, 'sdkconfig'),
                         )
@@ -426,15 +368,15 @@
         return textwrap.wrap(text, width) + parts[1:]
 
     def _get_help_string(self, action):
         """
         Add the default value to the option help message.
 
         ArgumentDefaultsHelpFormatter and BooleanOptionalAction when it isn't
-        already present. This code will do that, detecting corner cases to
+        already present. This code will do that, detecting cornercases to
         prevent duplicates or cases where it wouldn't make sense to the end
         user.
         """
         _help = action.help
         if _help is None:
             _help = ''
 
@@ -466,24 +408,23 @@
 
             _help += '{} - config name: {}'.format(self.LINE_SEP, action.dest)
             _help += '{} - config type: {}'.format(self.LINE_SEP, _type)
 
         return _help
 
 
-def get_parser():  # type: () -> argparse.ArgumentParser
+def main():
     parser = argparse.ArgumentParser(
         description='Tools for building ESP-IDF related apps.'
         'Some CLI options can be expanded by the following placeholders, like "--work-dir", "--build-dir", etc.:\n'
         '- @t: would be replaced by the target chip type\n'
         '- @w: would be replaced by the wildcard, usually the sdkconfig\n'
         '- @n: would be replaced by the app name\n'
         '- @f: would be replaced by the escaped app path (replaced "/" to "_")\n'
-        '- @i: would be replaced by the build index\n'
-        '- @p: would be replaced by the parallel index',
+        '- @i: would be replaced by the build index',
         formatter_class=argparse.RawDescriptionHelpFormatter,
     )
     actions = parser.add_subparsers(dest='action')
 
     common_args = argparse.ArgumentParser(add_help=False)
     common_args.add_argument(
         '-c',
@@ -546,14 +487,15 @@
         default=0,
         action='count',
         help='Increase the logging level of the whole process. Can be specified multiple times. '
         'By default set to WARNING level. Specify once to set to INFO level. Specify twice or more to set to DEBUG level',
     )
     common_args.add_argument(
         '--log-file',
+        type=argparse.FileType('w'),
         help='Write the log to the specified file, instead of stderr',
     )
     common_args.add_argument(
         '--check-warnings', action='store_true', help='If set, fail the build if warnings are found'
     )
     common_args.add_argument(
         '--manifest-file',
@@ -563,20 +505,16 @@
     common_args.add_argument(
         '--manifest-rootpath',
         help='Root directory for calculating the realpath of the relative path defined in the manifest files. '
         'Would use the current directory if not set',
     )
     common_args.add_argument(
         '--default-build-targets',
-        nargs='+',
-        help='space-separated list of supported targets. Targets supported in current ESP-IDF branch '
-        '(except preview ones) would be used if this option is not set.'
-        '{} ! DeprecationWarning: comma-separated list support will be removed in idf-build-apps 1.0.0 version'.format(
-            IdfBuildAppsCliFormatter.LINE_SEP
-        ),
+        help='comma-separated list of supported targets. Targets supported in current ESP-IDF branch '
+        '(except preview ones) would be used if this option is not set',
     )
     common_args.add_argument(
         '--depends-on-components',
         nargs='*',
         default=None,
         help='space-separated components list, app with `requires_components` set in the corresponding manifest files '
         'would only be built if depends on any of the specified components',
@@ -639,19 +577,21 @@
     build_parser.add_argument(
         '--no-preserve',
         action='store_true',
         help="Don't preserve the build directory after a successful build",
     )
     build_parser.add_argument(
         '--collect-size-info',
-        help='write size info json file while building into the specified file. each line is a json object. Can expand placeholders',
+        type=argparse.FileType('w'),
+        help='write size info json file while building into the specified file. each line is a json object',
     )
     build_parser.add_argument(
         '--collect-app-info',
-        help='write app info json file while building into the specified file. each line is a json object. Can expand placeholders',
+        type=argparse.FileType('w'),
+        help='write app info json file while building into the specified file. each line is a json object',
     )
     build_parser.add_argument(
         '--ignore-warning-str',
         action='append',
         help='Ignore the warning string that match the specified regex in the build output',
     )
     build_parser.add_argument(
@@ -661,89 +601,74 @@
     )
     build_parser.add_argument(
         '--copy-sdkconfig',
         action='store_true',
         help='Copy the sdkconfig file to the build directory',
     )
 
-    return parser
-
+    args = parser.parse_args()
 
-def validate_args(parser, args):  # type: (argparse.ArgumentParser, argparse.Namespace) -> None
     # validate cli subcommands
     if args.action not in ['find', 'build']:
         parser.print_help()
         raise InvalidCommand('subcommand is required. {find, build}')
 
+    # support toml config file
+    config_dict = get_valid_config(custom_path=args.config_file)
+    if config_dict:
+        for k, v in config_dict.items():
+            setattr(args, k, v)
+
     if not args.paths:
         raise InvalidCommand(
             'Must specify at least one path to search for the apps ' 'with CLI option "-p <path>" or "--path <path>"'
         )
 
     if not args.target:
         raise InvalidCommand(
             'Must specify current build target with CLI option "-t <target>" or "--target <target>". '
             '(choices: [{}]'.format(','.join(ALL_TARGETS + ['all']))
         )
 
     default_build_targets = []
     if args.default_build_targets:
-        for target in args.default_build_targets:
-            t_list = [_t.strip() for _t in target.split(',')] if ',' in target else [target.strip()]
-            for _t in t_list:
-                if _t not in ALL_TARGETS:
-                    raise InvalidCommand(
-                        'Unrecognizable target {} specified with "--default-build-targets". '
-                        'Current ESP-IDF available targets: {}'.format(_t, ALL_TARGETS)
-                    )
-
-                if _t not in default_build_targets:
-                    default_build_targets.append(_t)
+        for target in args.default_build_targets.split(','):
+            target = target.strip()
+            if target not in ALL_TARGETS:
+                raise InvalidCommand(
+                    'Unrecognizable target {} specified with "--default-build-targets". '
+                    'Current ESP-IDF available targets: {}'.format(target, ALL_TARGETS)
+                )
 
-    args.default_build_targets = default_build_targets
+            if target not in default_build_targets:
+                default_build_targets.append(target)
 
     if (args.ignore_component_dependencies_file_patterns is None) != (args.depends_on_files is None):
         raise InvalidCommand(
             'Must specify both "--ignore-component-dependencies-file-patterns" and "--depends-on-files" '
             'or neither of them'
         )
 
-
-def apply_config_args(args):  # type: (argparse.Namespace) -> None
-    # support toml config file
-    config_dict = get_valid_config(custom_path=args.config_file)
-    if config_dict:
-        for k, v in config_dict.items():
-            setattr(args, k, v)
-
+    # real call starts here
     setup_logging(args.verbose, args.log_file, not args.no_color)
 
-
-def main():
-    parser = get_parser()
-    args = parser.parse_args()
-
-    apply_config_args(args)
-    validate_args(parser, args)
-
-    # real call starts here
     apps = find_apps(
         args.paths,
         args.target,
         build_system=args.build_system,
         recursive=args.recursive,
         exclude_list=args.exclude or [],
         work_dir=args.work_dir,
         build_dir=args.build_dir or 'build',
         config_rules_str=args.config,
         build_log_path=args.build_log,
         size_json_path=args.size_file,
         check_warnings=args.check_warnings,
         manifest_files=args.manifest_file,
-        default_build_targets=args.default_build_targets,
+        default_build_targets=default_build_targets,
         depends_on_components=args.depends_on_components,
         manifest_rootpath=args.manifest_rootpath,
         ignore_component_dependencies_file_patterns=args.ignore_component_dependencies_file_patterns,
         depends_on_files=args.depends_on_files,
         sdkconfig_defaults=args.sdkconfig_defaults,
     )
```

### Comparing `idf-build-apps-0.6.0/idf_build_apps/manifest/if_parser.py` & `idf-build-apps-0.6.0rc0/idf_build_apps/manifest/if_parser.py`

 * *Files 17% similar despite different names*

```diff
@@ -30,43 +30,41 @@
 
 
 class Stmt:
     """
     Statement
     """
 
-    def get_value(self, target, config_name):  # type: (str, str) -> any
+    def get_value(self, target):  # type: (str) -> any
         """
         Lazy calculated. All subclasses of `Stmt` should implement this function.
 
         :param target: ESP-IDF target
         :type target: str
-        :param config_name: config name
-        :type target: str
         :return: the value of the statement
         """
         raise NotImplementedError('Please implement this function in sub classes')
 
 
 class ChipAttr(Stmt):
     """
-    Attributes defined in SOC Header Files and other keywords as followed:
+    Attributes defined in SOC Header Files and some other keywords
 
+    Supported keywords:
     - IDF_TARGET: target
     - INCLUDE_DEFAULT: take the default build targets into account or not
     - IDF_VERSION_MAJOR: major version of ESP-IDF
     - IDF_VERSION_MINOR: minor version of ESP-IDF
     - IDF_VERSION_PATCH: patch version of ESP-IDF
-    - CONFIG_NAME: config name defined in the config rules
     """
 
     def __init__(self, t):
         self.attr = t[0]
 
-    def get_value(self, target, config_name):  # type: (str, str) -> any
+    def get_value(self, target):  # type: (str) -> any
         from .manifest import FolderRule  # lazy-load
 
         if self.attr == 'IDF_TARGET':
             return target
 
         if self.attr == 'INCLUDE_DEFAULT':
             return 1 if target in FolderRule.DEFAULT_BUILD_TARGETS else 0
@@ -76,101 +74,98 @@
 
         if self.attr == 'IDF_VERSION_MINOR':
             return IDF_VERSION_MINOR
 
         if self.attr == 'IDF_VERSION_PATCH':
             return IDF_VERSION_PATCH
 
-        if self.attr == 'CONFIG_NAME':
-            return config_name
-
         if self.attr in SOC_HEADERS[target]:
             return SOC_HEADERS[target][self.attr]
 
         return 0  # default return 0 as false
 
 
 class Integer(Stmt):
     def __init__(self, t):
         self.expr = t[0]
 
-    def get_value(self, target, config_name):  # type: (str, str) -> any
+    def get_value(self, target):  # type: (str) -> any
         return literal_eval(self.expr)
 
 
 class String(Stmt):
     def __init__(self, t):
         self.expr = t[0]
 
-    def get_value(self, target, config_name):  # type: (str, str) -> any
+    def get_value(self, target):  # type: (str) -> any
         return literal_eval('"{}"'.format(self.expr))  # double quotes is swallowed by QuotedString
 
 
 class List_(Stmt):
     def __init__(self, t):
         self.expr = t
 
-    def get_value(self, target, config_name):  # type: (str, str) -> any
-        return [item.get_value(target, config_name) for item in self.expr]
+    def get_value(self, target):  # type: (str) -> any
+        return [item.get_value(target) for item in self.expr]
 
 
 class BoolStmt(Stmt):
     def __init__(self, t):
         self.left = t[0]  # type: Stmt
         self.comparison = t[1]  # type: str
         self.right = t[2]  # type: Stmt
 
-    def get_value(self, target, config_name):  # type: (str, str) -> any
+    def get_value(self, target):  # type: (str) -> any
         if self.comparison == '==':
-            return self.left.get_value(target, config_name) == self.right.get_value(target, config_name)
+            return self.left.get_value(target) == self.right.get_value(target)
 
         if self.comparison == '!=':
-            return self.left.get_value(target, config_name) != self.right.get_value(target, config_name)
+            return self.left.get_value(target) != self.right.get_value(target)
 
         if self.comparison == '>':
-            return self.left.get_value(target, config_name) > self.right.get_value(target, config_name)
+            return self.left.get_value(target) > self.right.get_value(target)
 
         if self.comparison == '>=':
-            return self.left.get_value(target, config_name) >= self.right.get_value(target, config_name)
+            return self.left.get_value(target) >= self.right.get_value(target)
 
         if self.comparison == '<':
-            return self.left.get_value(target, config_name) < self.right.get_value(target, config_name)
+            return self.left.get_value(target) < self.right.get_value(target)
 
         if self.comparison == '<=':
-            return self.left.get_value(target, config_name) <= self.right.get_value(target, config_name)
+            return self.left.get_value(target) <= self.right.get_value(target)
 
         if self.comparison == 'not in':
-            return self.left.get_value(target, config_name) not in self.right.get_value(target, config_name)
+            return self.left.get_value(target) not in self.right.get_value(target)
 
         if self.comparison == 'in':
-            return self.left.get_value(target, config_name) in self.right.get_value(target, config_name)
+            return self.left.get_value(target) in self.right.get_value(target)
 
         raise ValueError('Unsupported comparison operator: "{}"'.format(self.comparison))
 
 
 class BoolExpr(Stmt):
     pass
 
 
 class BoolAnd(BoolExpr):
     def __init__(self, t):
         self.left = t[0][0]  # type: BoolStmt
         self.right = t[0][2]  # type: BoolStmt
 
-    def get_value(self, target, config_name):  # type: (str, str) -> any
-        return self.left.get_value(target, config_name) and self.right.get_value(target, config_name)
+    def get_value(self, target):  # type: (str) -> any
+        return self.left.get_value(target) and self.right.get_value(target)
 
 
 class BoolOr(BoolExpr):
     def __init__(self, t):
         self.left = t[0][0]  # type: BoolStmt
         self.right = t[0][2]  # type: BoolStmt
 
-    def get_value(self, target, config_name):  # type: (str, str) -> any
-        return self.left.get_value(target, config_name) or self.right.get_value(target, config_name)
+    def get_value(self, target):  # type: (str) -> any
+        return self.left.get_value(target) or self.right.get_value(target)
 
 
 CAP_WORD = Word(alphas.upper(), nums + alphas.upper() + '_').setParseAction(ChipAttr)
 
 DECIMAL_NUMBER = Word(nums)
 HEX_NUMBER = Literal('0x') + Word(hexnums)
 INTEGER = (HEX_NUMBER | DECIMAL_NUMBER).setParseAction(Integer)
```

### Comparing `idf-build-apps-0.6.0/idf_build_apps/manifest/soc_header.py` & `idf-build-apps-0.6.0rc0/idf_build_apps/manifest/soc_header.py`

 * *Files identical despite different names*

### Comparing `idf-build-apps-0.6.0/idf_build_apps/utils.py` & `idf-build-apps-0.6.0rc0/idf_build_apps/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 # SPDX-FileCopyrightText: 2022-2023 Espressif Systems (Shanghai) CO LTD
 # SPDX-License-Identifier: Apache-2.0
 
 import fnmatch
+import logging
 import os
 import shutil
 import subprocess
 import sys
 from copy import (
     deepcopy,
 )
 from pathlib import (
     Path,
 )
 
 from . import (
     LOGGER,
 )
+from .log import (
+    ColoredFormatter,
+)
 
 try:
     import typing as t
 except ImportError:
     pass
 
 
@@ -60,14 +64,46 @@
     for rule_str in to_list(rule_strings):
         items = rule_str.split('=', 2)
         rules.append(ConfigRule(items[0], items[1] if len(items) == 2 else None))
     # '' is the default config, sort this one to the front
     return sorted(rules, key=lambda x: x.file_name)
 
 
+def setup_logging(verbose=0, log_file=None, colored=True):  # type: (int, str | None, bool) -> None
+    """
+    Setup logging stream handler
+
+    :param verbose: 0 - WARNING, 1 - INFO, 2+ - DEBUG
+    :type verbose: int
+    :param log_file: log file path
+    :type log_file: str
+    :param colored: colored output or not
+    :type colored: bool
+    :return: None
+    :rtype: None
+    """
+    if not verbose:
+        level = logging.WARNING
+    elif verbose == 1:
+        level = logging.INFO
+    else:
+        level = logging.DEBUG
+
+    LOGGER.setLevel(level)
+    if log_file:
+        stream = open(log_file, 'w')
+    else:
+        stream = sys.stderr
+    handler = logging.StreamHandler(stream)
+    handler.setLevel(level)
+    handler.setFormatter(ColoredFormatter(colored))
+    LOGGER.handlers = [handler]
+    LOGGER.propagate = False
+
+
 def get_parallel_start_stop(total, parallel_count, parallel_index):  # type: (int, int, int) -> (int, int)
     """
     Calculate the start and stop indices for a parallel task (1-based).
 
     :param total: total number of tasks
     :type total: int
     :param parallel_count: number of parallel tasks to run
```

### Comparing `idf-build-apps-0.6.0/pyproject.toml` & `idf-build-apps-0.6.0rc0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `idf-build-apps-0.6.0/tests/conftest.py` & `idf-build-apps-0.6.0rc0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `idf-build-apps-0.6.0/tests/test_build.py` & `idf-build-apps-0.6.0rc0/tests/test_build.py`

 * *Files identical despite different names*

### Comparing `idf-build-apps-0.6.0/tests/test_finder.py` & `idf-build-apps-0.6.0rc0/tests/test_finder.py`

 * *Files 17% similar despite different names*

```diff
@@ -167,29 +167,29 @@
         finally:
             try:
                 os.remove(_default_sdkconfig_path)
                 logging.info('Removed temp %s %s', DEFAULT_SDKCONFIG, _default_sdkconfig_path)
             except:  # noqa
                 pass
 
-    def test_with_config_rules(self, tmp_path, monkeypatch):
+    def test_with_config_rules(self, tmp_path):
         create_project('test1', tmp_path)
 
         (tmp_path / 'test1' / 'sdkconfig.defaults').touch()
         (tmp_path / 'test1' / 'sdkconfig.defaults_new').touch()
         (tmp_path / 'test1' / 'sdkconfig.ci.foo').touch()
 
         apps = find_apps(str(tmp_path / 'test1'), 'esp32', recursive=True, config_rules_str='sdkconfig.ci.*=')
         assert len(apps) == 1
         assert apps[0].sdkconfig_files == [
             str(tmp_path / 'test1' / 'sdkconfig.defaults'),
             str(tmp_path / 'test1' / 'sdkconfig.ci.foo'),
         ]
 
-        monkeypatch.setenv('SDKCONFIG_DEFAULTS', 'sdkconfig.defaults_new')
+        os.environ['SDKCONFIG_DEFAULTS'] = 'sdkconfig.defaults_new'
         apps = find_apps(str(tmp_path / 'test1'), 'esp32', recursive=True, config_rules_str='sdkconfig.ci.*=')
         assert len(apps) == 1
         assert apps[0].sdkconfig_files == [
             str(tmp_path / 'test1' / 'sdkconfig.defaults_new'),
             str(tmp_path / 'test1' / 'sdkconfig.ci.foo'),
         ]
 
@@ -227,71 +227,7 @@
             'build_esp32_foo',
             'sdkconfig.ci.foo',
         )
 
         monkeypatch.setenv('TEST_TARGET', 'esp32s2')
         apps = find_apps('test1', 'esp32', recursive=True, config_rules_str='sdkconfig.ci.*=')
         assert len(apps) == 0
-
-    def test_config_name_in_manifest(self, tmp_path):
-        create_project('test1', tmp_path)
-
-        (tmp_path / 'test1' / 'sdkconfig.defaults').touch()
-        (tmp_path / 'test1' / 'sdkconfig.ci').touch()
-        (tmp_path / 'test1' / 'sdkconfig.ci.foo').touch()
-        (tmp_path / 'test1' / 'sdkconfig.ci.bar').touch()
-
-        yaml_file = tmp_path / 'test.yml'
-        yaml_file.write_text(
-            f'''
-{tmp_path}:
-    enable:
-    - if: CONFIG_NAME == "foo" and IDF_TARGET == "esp32"
-    - if: CONFIG_NAME == "bar" and IDF_TARGET == "esp32s2"
-    - if: CONFIG_NAME == "default" and IDF_TARGET == "esp32s3"
-''',
-            encoding='utf8',
-        )
-
-        apps = find_apps(
-            str(tmp_path / 'test1'),
-            'esp32',
-            recursive=True,
-            config_rules_str=['sdkconfig.ci.*=', 'sdkconfig.ci=default'],
-            manifest_files=yaml_file,
-        )
-        assert len(apps) == 1
-        assert apps[0].sdkconfig_files == [
-            str(tmp_path / 'test1' / 'sdkconfig.defaults'),
-            str(tmp_path / 'test1' / 'sdkconfig.ci.foo'),
-        ]
-        apps = find_apps(
-            str(tmp_path / 'test1'),
-            'esp32s2',
-            recursive=True,
-            config_rules_str=['sdkconfig.ci.*=', 'sdkconfig.ci=default'],
-            manifest_files=yaml_file,
-        )
-        assert len(apps) == 1
-        assert apps[0].sdkconfig_files == [
-            str(tmp_path / 'test1' / 'sdkconfig.defaults'),
-            str(tmp_path / 'test1' / 'sdkconfig.ci.bar'),
-        ]
-        apps = find_apps(
-            str(tmp_path / 'test1'),
-            'esp32s3',
-            recursive=True,
-            config_rules_str=['sdkconfig.ci.*=', 'sdkconfig.ci=default'],
-            manifest_files=yaml_file,
-        )
-        assert len(apps) == 1
-        assert apps[0].sdkconfig_files == [
-            str(tmp_path / 'test1' / 'sdkconfig.defaults'),
-            str(tmp_path / 'test1' / 'sdkconfig.ci'),
-        ]
-        apps = find_apps(
-            str(tmp_path / 'test1'), 'esp32s3', recursive=True, config_rules_str=['=default'], manifest_files=yaml_file
-        )
-        assert len(apps) == 1
-        assert apps[0].sdkconfig_files == [
-            str(tmp_path / 'test1' / 'sdkconfig.defaults'),
-        ]
```

### Comparing `idf-build-apps-0.6.0/tests/test_manifest.py` & `idf-build-apps-0.6.0rc0/tests/test_manifest.py`

 * *Files identical despite different names*

### Comparing `idf-build-apps-0.6.0/tests/test_utils.py` & `idf-build-apps-0.6.0rc0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `idf-build-apps-0.6.0/setup.py` & `idf-build-apps-0.6.0rc0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,15 +22,15 @@
          'sphinxcontrib-mermaid'],
  'test': ['pytest', 'pytest-cov']}
 
 entry_points = \
 {'console_scripts': ['idf-build-apps = idf_build_apps:main.main']}
 
 setup(name='idf-build-apps',
-      version='0.6.0',
+      version='0.6.0rc0',
       description='Tools for building ESP-IDF related apps.',
       author=None,
       author_email='Fu Hanxi <fuhanxi@espressif.com>',
       url=None,
       packages=packages,
       package_data=package_data,
       install_requires=install_requires,
```

### Comparing `idf-build-apps-0.6.0/PKG-INFO` & `idf-build-apps-0.6.0rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idf-build-apps
-Version: 0.6.0
+Version: 0.6.0rc0
 Summary: Tools for building ESP-IDF related apps.
 Author-email: Fu Hanxi <fuhanxi@espressif.com>
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 2.7
```

