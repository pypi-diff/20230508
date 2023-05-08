# Comparing `tmp/kiara_plugin.tabular-0.4.8.tar.gz` & `tmp/kiara_plugin.tabular-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kiara_plugin.tabular-0.4.8.tar", last modified: Thu Jul  7 11:50:34 2022, max compression
+gzip compressed data, was "kiara_plugin.tabular-0.4.9.tar", last modified: Sun Jul 10 20:57:52 2022, max compression
```

## Comparing `kiara_plugin.tabular-0.4.8.tar` & `kiara_plugin.tabular-0.4.9.tar`

### file list

```diff
@@ -1,82 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-07 11:50:34.057962 kiara_plugin.tabular-0.4.8/
--rw-r--r--   0 runner    (1001) docker     (121)      704 2022-07-07 11:49:29.000000 kiara_plugin.tabular-0.4.8/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (121)      139 2022-07-07 11:49:29.000000 kiara_plugin.tabular-0.4.8/.envrc.disabled
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-07-07 11:49:29.000000 kiara_plugin.tabular-0.4.8/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-07-07 11:49:29.000000 kiara_plugin.tabular-0.4.8/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-07 11:50:34.049962 kiara_plugin.tabular-0.4.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-07 11:50:34.053962 kiara_plugin.tabular-0.4.8/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      834 2022-07-07 11:49:29.000000 kiara_plugin.tabular-0.4.8/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (121)      900 2022-07-07 11:49:29.000000 kiara_plugin.tabular-0.4.8/.github/ISSUE_TEMPLATE/suggest-a-module.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-07 11:50:34.053962 kiara_plugin.tabular-0.4.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      881 2022-07-07 11:49:29.000000 kiara_plugin.tabular-0.4.8/.github/workflows/build-darwin.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     8152 2022-07-07 11:49:29.000000 kiara_plugin.tabular-0.4.8/.github/workflows/build-linux.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      682 2022-07-07 11:49:29.000000 kiara_plugin.tabular-0.4.8/.github/workflows/build-windows.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      759 2022-07-07 11:49:29.000000 kiara_plugin.tabular-0.4.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1834 2022-07-07 11:49:29.000000 kiara_plugin.tabular-0.4.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       53 2022-07-07 11:49:29.000000 kiara_plugin.tabular-0.4.8/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (121)      102 2022-07-07 11:49:29.000000 kiara_plugin.tabular-0.4.8/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)    16725 2022-07-07 11:49:29.000000 kiara_plugin.tabular-0.4.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      387 2022-07-07 11:49:29.000000 kiara_plugin.tabular-0.4.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2233 2022-07-07 11:49:29.000000 kiara_plugin.tabular-0.4.8/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)     5448 2022-07-07 11:50:34.057962 kiara_plugin.tabular-0.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4568 2022-07-07 11:49:29.000000 kiara_plugin.tabular-0.4.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-07 11:50:34.049962 kiara_plugin.tabular-0.4.8/ci/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-07 11:50:34.053962 kiara_plugin.tabular-0.4.8/ci/conda/
--rwxr-xr-x   0 runner    (1001) docker     (121)     7458 2022-07-07 11:49:29.000000 kiara_plugin.tabular-0.4.8/ci/conda/build-conda-packages.sh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-07 11:50:34.053962 kiara_plugin.tabular-0.4.8/ci/conda/kiara_plugin.tabular/
--rw-r--r--   0 runner    (1001) docker     (121)      921 2022-07-07 11:49:29.000000 kiara_plugin.tabular-0.4.8/ci/conda/kiara_plugin.tabular/meta.yaml.template
--rw-r--r--   0 runner    (1001) docker     (121)       64 2022-07-07 11:49:29.000000 kiara_plugin.tabular-0.4.8/commitlint.config.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-07 11:50:34.053962 kiara_plugin.tabular-0.4.8/docs/
--rw-r--r--   0 runner    (1001) docker     (121)       97 2022-07-07 11:49:29.000000 kiara_plugin.tabular-0.4.8/docs/SUMMARY.md
--rw-r--r--   0 runner    (1001) docker     (121)      861 2022-07-07 11:49:29.000000 kiara_plugin.tabular-0.4.8/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-07 11:50:34.053962 kiara_plugin.tabular-0.4.8/docs/stylesheets/
--rw-r--r--   0 runner    (1001) docker     (121)      144 2022-07-07 11:49:29.000000 kiara_plugin.tabular-0.4.8/docs/stylesheets/extra.css
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-07-07 11:49:29.000000 kiara_plugin.tabular-0.4.8/docs/usage.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-07 11:50:34.049962 kiara_plugin.tabular-0.4.8/examples/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-07 11:50:34.053962 kiara_plugin.tabular-0.4.8/examples/data/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-07 11:49:29.000000 kiara_plugin.tabular-0.4.8/examples/data/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (121)     1412 2022-07-07 11:49:29.000000 kiara_plugin.tabular-0.4.8/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)      362 2022-07-07 11:49:29.000000 kiara_plugin.tabular-0.4.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-07 11:50:34.049962 kiara_plugin.tabular-0.4.8/scripts/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-07 11:50:34.053962 kiara_plugin.tabular-0.4.8/scripts/documentation/
--rw-r--r--   0 runner    (1001) docker     (121)      865 2022-07-07 11:49:29.000000 kiara_plugin.tabular-0.4.8/scripts/documentation/gen_api_doc_pages.py
--rw-r--r--   0 runner    (1001) docker     (121)      568 2022-07-07 11:49:29.000000 kiara_plugin.tabular-0.4.8/scripts/documentation/gen_info_pages.py
--rw-r--r--   0 runner    (1001) docker     (121)     1852 2022-07-07 11:49:29.000000 kiara_plugin.tabular-0.4.8/scripts/documentation/gen_module_doc.py
--rw-r--r--   0 runner    (1001) docker     (121)     3745 2022-07-07 11:50:34.061962 kiara_plugin.tabular-0.4.8/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     1393 2022-07-07 11:49:29.000000 kiara_plugin.tabular-0.4.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-07 11:50:34.049962 kiara_plugin.tabular-0.4.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-07 11:50:34.049962 kiara_plugin.tabular-0.4.8/src/kiara_plugin/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-07 11:50:34.057962 kiara_plugin.tabular-0.4.8/src/kiara_plugin/tabular/
--rw-r--r--   0 runner    (1001) docker     (121)     2165 2022-07-07 11:49:29.000000 kiara_plugin.tabular-0.4.8/src/kiara_plugin/tabular/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-07 11:50:34.057962 kiara_plugin.tabular-0.4.8/src/kiara_plugin/tabular/data_types/
--rw-r--r--   0 runner    (1001) docker     (121)      131 2022-07-07 11:49:29.000000 kiara_plugin.tabular-0.4.8/src/kiara_plugin/tabular/data_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3651 2022-07-07 11:49:29.000000 kiara_plugin.tabular-0.4.8/src/kiara_plugin/tabular/data_types/db.py
--rw-r--r--   0 runner    (1001) docker     (121)     9251 2022-07-07 11:49:29.000000 kiara_plugin.tabular-0.4.8/src/kiara_plugin/tabular/data_types/table.py
--rw-r--r--   0 runner    (1001) docker     (121)     2530 2022-07-07 11:49:29.000000 kiara_plugin.tabular-0.4.8/src/kiara_plugin/tabular/defaults.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-07 11:50:34.057962 kiara_plugin.tabular-0.4.8/src/kiara_plugin/tabular/models/
--rw-r--r--   0 runner    (1001) docker     (121)     1670 2022-07-07 11:49:29.000000 kiara_plugin.tabular-0.4.8/src/kiara_plugin/tabular/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10222 2022-07-07 11:49:29.000000 kiara_plugin.tabular-0.4.8/src/kiara_plugin/tabular/models/db.py
--rw-r--r--   0 runner    (1001) docker     (121)     9150 2022-07-07 11:49:29.000000 kiara_plugin.tabular-0.4.8/src/kiara_plugin/tabular/models/table.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-07 11:50:34.057962 kiara_plugin.tabular-0.4.8/src/kiara_plugin/tabular/pipelines/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-07 11:49:29.000000 kiara_plugin.tabular-0.4.8/src/kiara_plugin/tabular/pipelines/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (121)      124 2022-07-07 11:49:29.000000 kiara_plugin.tabular-0.4.8/src/kiara_plugin/tabular/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      536 2022-07-07 11:49:29.000000 kiara_plugin.tabular-0.4.8/src/kiara_plugin/tabular/pipelines/load.table.yaml
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-07 11:49:29.000000 kiara_plugin.tabular-0.4.8/src/kiara_plugin/tabular/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-07 11:50:34.057962 kiara_plugin.tabular-0.4.8/src/kiara_plugin/tabular/resources/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-07 11:49:29.000000 kiara_plugin.tabular-0.4.8/src/kiara_plugin/tabular/resources/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-07 11:50:34.057962 kiara_plugin.tabular-0.4.8/src/kiara_plugin/tabular/tabular/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-07 11:49:29.000000 kiara_plugin.tabular-0.4.8/src/kiara_plugin/tabular/tabular/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9574 2022-07-07 11:49:29.000000 kiara_plugin.tabular-0.4.8/src/kiara_plugin/tabular/tabular/db.py
--rw-r--r--   0 runner    (1001) docker     (121)     9396 2022-07-07 11:49:29.000000 kiara_plugin.tabular-0.4.8/src/kiara_plugin/tabular/tabular/table.py
--rw-r--r--   0 runner    (1001) docker     (121)     7439 2022-07-07 11:49:29.000000 kiara_plugin.tabular-0.4.8/src/kiara_plugin/tabular/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-07 11:50:34.057962 kiara_plugin.tabular-0.4.8/src/kiara_plugin.tabular.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5448 2022-07-07 11:50:33.000000 kiara_plugin.tabular-0.4.8/src/kiara_plugin.tabular.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1814 2022-07-07 11:50:34.000000 kiara_plugin.tabular-0.4.8/src/kiara_plugin.tabular.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-07 11:50:33.000000 kiara_plugin.tabular-0.4.8/src/kiara_plugin.tabular.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      266 2022-07-07 11:50:33.000000 kiara_plugin.tabular-0.4.8/src/kiara_plugin.tabular.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-07 11:50:27.000000 kiara_plugin.tabular-0.4.8/src/kiara_plugin.tabular.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)     1768 2022-07-07 11:50:33.000000 kiara_plugin.tabular-0.4.8/src/kiara_plugin.tabular.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-07-07 11:50:33.000000 kiara_plugin.tabular-0.4.8/src/kiara_plugin.tabular.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-07 11:50:34.057962 kiara_plugin.tabular-0.4.8/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      274 2022-07-07 11:49:29.000000 kiara_plugin.tabular-0.4.8/tests/conftest.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      227 2022-07-07 11:49:29.000000 kiara_plugin.tabular-0.4.8/tests/test_kiara_modules_default.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-10 20:57:52.840224 kiara_plugin.tabular-0.4.9/
+-rw-r--r--   0 runner    (1001) docker     (121)      704 2022-07-10 20:57:03.000000 kiara_plugin.tabular-0.4.9/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (121)      139 2022-07-10 20:57:03.000000 kiara_plugin.tabular-0.4.9/.envrc.disabled
+-rw-r--r--   0 runner    (1001) docker     (121)       23 2022-07-10 20:57:03.000000 kiara_plugin.tabular-0.4.9/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       32 2022-07-10 20:57:03.000000 kiara_plugin.tabular-0.4.9/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-10 20:57:52.828224 kiara_plugin.tabular-0.4.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-10 20:57:52.832224 kiara_plugin.tabular-0.4.9/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      834 2022-07-10 20:57:03.000000 kiara_plugin.tabular-0.4.9/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (121)      900 2022-07-10 20:57:03.000000 kiara_plugin.tabular-0.4.9/.github/ISSUE_TEMPLATE/suggest-a-module.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-10 20:57:52.836224 kiara_plugin.tabular-0.4.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)      881 2022-07-10 20:57:03.000000 kiara_plugin.tabular-0.4.9/.github/workflows/build-darwin.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     8152 2022-07-10 20:57:03.000000 kiara_plugin.tabular-0.4.9/.github/workflows/build-linux.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      682 2022-07-10 20:57:03.000000 kiara_plugin.tabular-0.4.9/.github/workflows/build-windows.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      759 2022-07-10 20:57:03.000000 kiara_plugin.tabular-0.4.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1834 2022-07-10 20:57:03.000000 kiara_plugin.tabular-0.4.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)       53 2022-07-10 20:57:03.000000 kiara_plugin.tabular-0.4.9/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (121)      102 2022-07-10 20:57:03.000000 kiara_plugin.tabular-0.4.9/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (121)    16725 2022-07-10 20:57:03.000000 kiara_plugin.tabular-0.4.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      387 2022-07-10 20:57:03.000000 kiara_plugin.tabular-0.4.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     2233 2022-07-10 20:57:03.000000 kiara_plugin.tabular-0.4.9/Makefile
+-rw-r--r--   0 runner    (1001) docker     (121)     5448 2022-07-10 20:57:52.840224 kiara_plugin.tabular-0.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4568 2022-07-10 20:57:03.000000 kiara_plugin.tabular-0.4.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-10 20:57:52.828224 kiara_plugin.tabular-0.4.9/ci/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-10 20:57:52.836224 kiara_plugin.tabular-0.4.9/ci/conda/
+-rwxr-xr-x   0 runner    (1001) docker     (121)     7458 2022-07-10 20:57:03.000000 kiara_plugin.tabular-0.4.9/ci/conda/build-conda-packages.sh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-10 20:57:52.836224 kiara_plugin.tabular-0.4.9/ci/conda/kiara_plugin.tabular/
+-rw-r--r--   0 runner    (1001) docker     (121)      943 2022-07-10 20:57:03.000000 kiara_plugin.tabular-0.4.9/ci/conda/kiara_plugin.tabular/meta.yaml.template
+-rw-r--r--   0 runner    (1001) docker     (121)       64 2022-07-10 20:57:03.000000 kiara_plugin.tabular-0.4.9/commitlint.config.js
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-10 20:57:52.836224 kiara_plugin.tabular-0.4.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (121)      129 2022-07-10 20:57:03.000000 kiara_plugin.tabular-0.4.9/docs/SUMMARY.md
+-rw-r--r--   0 runner    (1001) docker     (121)      861 2022-07-10 20:57:03.000000 kiara_plugin.tabular-0.4.9/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-10 20:57:52.836224 kiara_plugin.tabular-0.4.9/docs/stylesheets/
+-rw-r--r--   0 runner    (1001) docker     (121)      144 2022-07-10 20:57:03.000000 kiara_plugin.tabular-0.4.9/docs/stylesheets/extra.css
+-rw-r--r--   0 runner    (1001) docker     (121)       21 2022-07-10 20:57:03.000000 kiara_plugin.tabular-0.4.9/docs/usage.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-10 20:57:52.828224 kiara_plugin.tabular-0.4.9/examples/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-10 20:57:52.836224 kiara_plugin.tabular-0.4.9/examples/data/
+-rw-r--r--   0 runner    (1001) docker     (121)      142 2022-07-10 20:57:03.000000 kiara_plugin.tabular-0.4.9/examples/data/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-10 20:57:52.836224 kiara_plugin.tabular-0.4.9/examples/data/journals/
+-rw-r--r--   0 runner    (1001) docker     (121)     2667 2022-07-10 20:57:03.000000 kiara_plugin.tabular-0.4.9/examples/data/journals/JournalEdges1902.csv
+-rw-r--r--   0 runner    (1001) docker     (121)    33121 2022-07-10 20:57:03.000000 kiara_plugin.tabular-0.4.9/examples/data/journals/JournalNodes1902.csv
+-rw-r--r--   0 runner    (1001) docker     (121)       58 2022-07-10 20:57:03.000000 kiara_plugin.tabular-0.4.9/examples/data/journals/Readme.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1412 2022-07-10 20:57:03.000000 kiara_plugin.tabular-0.4.9/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      362 2022-07-10 20:57:03.000000 kiara_plugin.tabular-0.4.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-10 20:57:52.828224 kiara_plugin.tabular-0.4.9/scripts/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-10 20:57:52.836224 kiara_plugin.tabular-0.4.9/scripts/documentation/
+-rw-r--r--   0 runner    (1001) docker     (121)      865 2022-07-10 20:57:03.000000 kiara_plugin.tabular-0.4.9/scripts/documentation/gen_api_doc_pages.py
+-rw-r--r--   0 runner    (1001) docker     (121)      568 2022-07-10 20:57:03.000000 kiara_plugin.tabular-0.4.9/scripts/documentation/gen_info_pages.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1852 2022-07-10 20:57:03.000000 kiara_plugin.tabular-0.4.9/scripts/documentation/gen_module_doc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3762 2022-07-10 20:57:52.840224 kiara_plugin.tabular-0.4.9/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1393 2022-07-10 20:57:03.000000 kiara_plugin.tabular-0.4.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-10 20:57:52.828224 kiara_plugin.tabular-0.4.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-10 20:57:52.828224 kiara_plugin.tabular-0.4.9/src/kiara_plugin/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-10 20:57:52.836224 kiara_plugin.tabular-0.4.9/src/kiara_plugin/tabular/
+-rw-r--r--   0 runner    (1001) docker     (121)     2165 2022-07-10 20:57:03.000000 kiara_plugin.tabular-0.4.9/src/kiara_plugin/tabular/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-10 20:57:52.836224 kiara_plugin.tabular-0.4.9/src/kiara_plugin/tabular/data_types/
+-rw-r--r--   0 runner    (1001) docker     (121)      131 2022-07-10 20:57:03.000000 kiara_plugin.tabular-0.4.9/src/kiara_plugin/tabular/data_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3651 2022-07-10 20:57:03.000000 kiara_plugin.tabular-0.4.9/src/kiara_plugin/tabular/data_types/db.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9251 2022-07-10 20:57:03.000000 kiara_plugin.tabular-0.4.9/src/kiara_plugin/tabular/data_types/table.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2530 2022-07-10 20:57:03.000000 kiara_plugin.tabular-0.4.9/src/kiara_plugin/tabular/defaults.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-10 20:57:52.836224 kiara_plugin.tabular-0.4.9/src/kiara_plugin/tabular/models/
+-rw-r--r--   0 runner    (1001) docker     (121)     1670 2022-07-10 20:57:03.000000 kiara_plugin.tabular-0.4.9/src/kiara_plugin/tabular/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10222 2022-07-10 20:57:03.000000 kiara_plugin.tabular-0.4.9/src/kiara_plugin/tabular/models/db.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9211 2022-07-10 20:57:03.000000 kiara_plugin.tabular-0.4.9/src/kiara_plugin/tabular/models/table.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-10 20:57:52.836224 kiara_plugin.tabular-0.4.9/src/kiara_plugin/tabular/modules/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-10 20:57:03.000000 kiara_plugin.tabular-0.4.9/src/kiara_plugin/tabular/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-10 20:57:52.836224 kiara_plugin.tabular-0.4.9/src/kiara_plugin/tabular/modules/array/
+-rw-r--r--   0 runner    (1001) docker     (121)     3896 2022-07-10 20:57:03.000000 kiara_plugin.tabular-0.4.9/src/kiara_plugin/tabular/modules/array/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-10 20:57:52.836224 kiara_plugin.tabular-0.4.9/src/kiara_plugin/tabular/modules/db/
+-rw-r--r--   0 runner    (1001) docker     (121)     9574 2022-07-10 20:57:03.000000 kiara_plugin.tabular-0.4.9/src/kiara_plugin/tabular/modules/db/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-10 20:57:52.836224 kiara_plugin.tabular-0.4.9/src/kiara_plugin/tabular/modules/table/
+-rw-r--r--   0 runner    (1001) docker     (121)    11396 2022-07-10 20:57:03.000000 kiara_plugin.tabular-0.4.9/src/kiara_plugin/tabular/modules/table/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-10 20:57:52.840224 kiara_plugin.tabular-0.4.9/src/kiara_plugin/tabular/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-10 20:57:03.000000 kiara_plugin.tabular-0.4.9/src/kiara_plugin/tabular/pipelines/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (121)      124 2022-07-10 20:57:03.000000 kiara_plugin.tabular-0.4.9/src/kiara_plugin/tabular/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      552 2022-07-10 20:57:03.000000 kiara_plugin.tabular-0.4.9/src/kiara_plugin/tabular/pipelines/extract_date_array.from.table.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      534 2022-07-10 20:57:03.000000 kiara_plugin.tabular-0.4.9/src/kiara_plugin/tabular/pipelines/import.table.from.csv_file.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      628 2022-07-10 20:57:03.000000 kiara_plugin.tabular-0.4.9/src/kiara_plugin/tabular/pipelines/import.table.from.text_file_bundle.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-10 20:57:03.000000 kiara_plugin.tabular-0.4.9/src/kiara_plugin/tabular/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-10 20:57:52.840224 kiara_plugin.tabular-0.4.9/src/kiara_plugin/tabular/resources/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-10 20:57:03.000000 kiara_plugin.tabular-0.4.9/src/kiara_plugin/tabular/resources/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (121)     7439 2022-07-10 20:57:03.000000 kiara_plugin.tabular-0.4.9/src/kiara_plugin/tabular/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-10 20:57:52.836224 kiara_plugin.tabular-0.4.9/src/kiara_plugin.tabular.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     5448 2022-07-10 20:57:52.000000 kiara_plugin.tabular-0.4.9/src/kiara_plugin.tabular.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2166 2022-07-10 20:57:52.000000 kiara_plugin.tabular-0.4.9/src/kiara_plugin.tabular.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-10 20:57:52.000000 kiara_plugin.tabular-0.4.9/src/kiara_plugin.tabular.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      266 2022-07-10 20:57:52.000000 kiara_plugin.tabular-0.4.9/src/kiara_plugin.tabular.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-10 20:57:48.000000 kiara_plugin.tabular-0.4.9/src/kiara_plugin.tabular.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)     1784 2022-07-10 20:57:52.000000 kiara_plugin.tabular-0.4.9/src/kiara_plugin.tabular.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       13 2022-07-10 20:57:52.000000 kiara_plugin.tabular-0.4.9/src/kiara_plugin.tabular.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-10 20:57:52.840224 kiara_plugin.tabular-0.4.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)      274 2022-07-10 20:57:03.000000 kiara_plugin.tabular-0.4.9/tests/conftest.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      227 2022-07-10 20:57:03.000000 kiara_plugin.tabular-0.4.9/tests/test_kiara_modules_default.py
```

### Comparing `kiara_plugin.tabular-0.4.8/.cruft.json` & `kiara_plugin.tabular-0.4.9/.cruft.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'commit'": "'354cdab3971a38fb68606d865d6136f4a6405958'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "checkout": null,
-    "commit": "0c580d788287fc1473eb6eec350dce0e0b54fec2",
+    "commit": "354cdab3971a38fb68606d865d6136f4a6405958",
     "context": {
         "cookiecutter": {
             "_extensions": [
                 "cookiecutter.extensions.JsonifyExtension"
             ],
             "_template": "https://github.com/DHARPA-Project/kiara_plugin.develop.git",
             "anaconda_user": "dharpa",
```

### Comparing `kiara_plugin.tabular-0.4.8/.github/ISSUE_TEMPLATE/bug_report.md` & `kiara_plugin.tabular-0.4.9/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.tabular-0.4.8/.github/ISSUE_TEMPLATE/suggest-a-module.md` & `kiara_plugin.tabular-0.4.9/.github/ISSUE_TEMPLATE/suggest-a-module.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.tabular-0.4.8/.github/workflows/build-darwin.yaml` & `kiara_plugin.tabular-0.4.9/.github/workflows/build-darwin.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.tabular-0.4.8/.github/workflows/build-linux.yaml` & `kiara_plugin.tabular-0.4.9/.github/workflows/build-linux.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.tabular-0.4.8/.github/workflows/build-windows.yaml` & `kiara_plugin.tabular-0.4.9/.github/workflows/build-windows.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.tabular-0.4.8/.gitignore` & `kiara_plugin.tabular-0.4.9/.gitignore`

 * *Files identical despite different names*

### Comparing `kiara_plugin.tabular-0.4.8/.pre-commit-config.yaml` & `kiara_plugin.tabular-0.4.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.tabular-0.4.8/LICENSE` & `kiara_plugin.tabular-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `kiara_plugin.tabular-0.4.8/Makefile` & `kiara_plugin.tabular-0.4.9/Makefile`

 * *Files identical despite different names*

### Comparing `kiara_plugin.tabular-0.4.8/PKG-INFO` & `kiara_plugin.tabular-0.4.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiara_plugin.tabular
-Version: 0.4.8
+Version: 0.4.9
 Summary: A set of modules (and pipelines) for Kiara.
 Home-page: https://github.com/DHARPA-Project/kiara_plugin.tabular
 Author: Markus Binsteiner
 Author-email: markus@frkl.io
 License: MPL-2.0
 Platform: any
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `kiara_plugin.tabular-0.4.8/README.md` & `kiara_plugin.tabular-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.tabular-0.4.8/ci/conda/build-conda-packages.sh` & `kiara_plugin.tabular-0.4.9/ci/conda/build-conda-packages.sh`

 * *Files identical despite different names*

### Comparing `kiara_plugin.tabular-0.4.8/ci/conda/kiara_plugin.tabular/meta.yaml.template` & `kiara_plugin.tabular-0.4.9/ci/conda/kiara_plugin.tabular/meta.yaml.template`

 * *Files 14% similar despite different names*

```diff
@@ -18,17 +18,18 @@
 requirements:
   host:
     - pip
     - python
     - setuptools_scm
     - setuptools_scm_git_archive
   run:
+    - polars>=0.13.52
     - python-duckdb>=0.3.4
     - python
-    - kiara>=0.4.13
+    - kiara>=0.4.14
     - pyarrow>=7.0.0
     - sqlite-utils>=3.20
 
 about:
   home: https://github.com/DHARPA-Project/kiara_plugin.tabular
   license: "Mozilla Public 2.0 (MPL 2.0)"
   license_family: MOZILLA
```

### Comparing `kiara_plugin.tabular-0.4.8/docs/index.md` & `kiara_plugin.tabular-0.4.9/docs/index.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.tabular-0.4.8/mkdocs.yml` & `kiara_plugin.tabular-0.4.9/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.tabular-0.4.8/scripts/documentation/gen_api_doc_pages.py` & `kiara_plugin.tabular-0.4.9/scripts/documentation/gen_api_doc_pages.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.tabular-0.4.8/scripts/documentation/gen_info_pages.py` & `kiara_plugin.tabular-0.4.9/scripts/documentation/gen_info_pages.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.tabular-0.4.8/scripts/documentation/gen_module_doc.py` & `kiara_plugin.tabular-0.4.9/scripts/documentation/gen_module_doc.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.tabular-0.4.8/setup.cfg` & `kiara_plugin.tabular-0.4.9/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -18,16 +18,17 @@
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 
 [options]
 packages = find_namespace:
 install_requires = 
 	duckdb>=0.3.4
-	kiara>=0.4.13
+	kiara>=0.4.14
 	pandas>=1.4.0
+	polars>=0.13.52
 	pyarrow>=7.0.0
 	sqlite-utils>=3.20
 python_requires = >=3.8
 include_package_data = True
 package_dir = 
 	=src
 setup_requires =
```

### Comparing `kiara_plugin.tabular-0.4.8/setup.py` & `kiara_plugin.tabular-0.4.9/setup.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.tabular-0.4.8/src/kiara_plugin/tabular/__init__.py` & `kiara_plugin.tabular-0.4.9/src/kiara_plugin/tabular/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     },
     "tags": ["tabular"],
     "labels": {"package": "kiara_plugin.tabular"},
 }
 
 find_modules: KiaraEntryPointItem = (
     find_kiara_modules_under,
-    "kiara_plugin.tabular.tabular",
+    "kiara_plugin.tabular.modules",
 )
 find_model_classes: KiaraEntryPointItem = (
     find_kiara_model_classes_under,
     "kiara_plugin.tabular.models",
 )
 find_data_types: KiaraEntryPointItem = (
     find_data_types_under,
```

### Comparing `kiara_plugin.tabular-0.4.8/src/kiara_plugin/tabular/data_types/db.py` & `kiara_plugin.tabular-0.4.9/src/kiara_plugin/tabular/data_types/db.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.tabular-0.4.8/src/kiara_plugin/tabular/data_types/table.py` & `kiara_plugin.tabular-0.4.9/src/kiara_plugin/tabular/data_types/table.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from kiara.defaults import DEFAULT_PRETTY_PRINT_CONFIG
 from kiara.models.values.value import SerializationResult, SerializedData, Value
 from kiara.utils.hashing import compute_cid
 from kiara.utils.output import ArrowTabularWrap
 from mmh3 import hash_from_buffer
 
 from kiara_plugin.tabular.models.table import KiaraArray, KiaraTable
-from kiara_plugin.tabular.tabular.table import EMPTY_COLUMN_NAME_MARKER
+from kiara_plugin.tabular.modules.table import EMPTY_COLUMN_NAME_MARKER
 
 if TYPE_CHECKING:
     import pyarrow as pa
 
 
 def store_array(array_obj: "pa.Array", file_name: str, column_name: "str" = "array"):
     """Utility methdo to stora an array to a file."""
```

### Comparing `kiara_plugin.tabular-0.4.8/src/kiara_plugin/tabular/defaults.py` & `kiara_plugin.tabular-0.4.9/src/kiara_plugin/tabular/defaults.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.tabular-0.4.8/src/kiara_plugin/tabular/models/__init__.py` & `kiara_plugin.tabular-0.4.9/src/kiara_plugin/tabular/models/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.tabular-0.4.8/src/kiara_plugin/tabular/models/db.py` & `kiara_plugin.tabular-0.4.9/src/kiara_plugin/tabular/models/db.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.tabular-0.4.8/src/kiara_plugin/tabular/models/table.py` & `kiara_plugin.tabular-0.4.9/src/kiara_plugin/tabular/models/table.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,14 +69,17 @@
     )
 
     _array_obj: pa.Array = PrivateAttr(default=None)
 
     def _retrieve_data_to_hash(self) -> Any:
         raise NotImplementedError()
 
+    def __len__(self):
+        return len(self.arrow_array)
+
     @property
     def arrow_array(self) -> pa.Array:
 
         if self._array_obj is not None:
             return self._array_obj
 
         if not self.data_path:
```

### Comparing `kiara_plugin.tabular-0.4.8/src/kiara_plugin/tabular/pipelines/load.table.yaml` & `kiara_plugin.tabular-0.4.9/src/kiara_plugin/tabular/pipelines/import.table.from.csv_file.yaml`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.925%*

 * *Differences: {"'output_aliases'": "{'create_table_from_file.table': 'table', delete: "*

 * *                     "['create_table_from_files.table']}",*

 * * "'steps'": "{1: {'step_id': 'create_table_from_file'}}"}*

```diff
@@ -1,24 +1,24 @@
 {
     "doc": "Load a table from a csv file.",
     "input_aliases": {
         "import_file.path": "path"
     },
     "output_aliases": {
-        "create_table_from_files.table": "table",
+        "create_table_from_file.table": "table",
         "import_file.file": "imported_file"
     },
     "pipeline_name": "import.table.from.csv_file",
     "steps": [
         {
             "module_type": "import.file",
             "step_id": "import_file"
         },
         {
             "input_links": {
                 "csv_file": "import_file.file"
             },
             "module_type": "create.table.from.csv_file",
-            "step_id": "create_table_from_files"
+            "step_id": "create_table_from_file"
         }
     ]
 }
```

### Comparing `kiara_plugin.tabular-0.4.8/src/kiara_plugin/tabular/tabular/db.py` & `kiara_plugin.tabular-0.4.9/src/kiara_plugin/tabular/modules/db/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.tabular-0.4.8/src/kiara_plugin/tabular/tabular/table.py` & `kiara_plugin.tabular-0.4.9/src/kiara_plugin/tabular/modules/table/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from kiara.models.filesystem import (
     FILE_BUNDLE_IMPORT_AVAILABLE_COLUMNS,
     FileBundle,
     FileModel,
 )
 from kiara.models.module import KiaraModuleConfig
 from kiara.models.values.value import SerializedData, Value, ValueMap
+from kiara.models.values.value_schema import ValueSchema
 from kiara.modules import ValueSetSchema
 from kiara.modules.included_core_modules.create_from import (
     CreateFromModule,
     CreateFromModuleConfig,
 )
 from kiara.modules.included_core_modules.export_as import DataExportModule
 from kiara.modules.included_core_modules.serialization import DeserializeValueModule
@@ -78,47 +79,14 @@
 
                 tabular.setdefault(column, []).append(_value)
 
         table = pa.Table.from_pydict(tabular)
         return KiaraTable.create_table(table)
 
 
-class DeserializeArrayModule(DeserializeValueModule):
-
-    _module_type_name = "load.array"
-
-    @classmethod
-    def retrieve_supported_target_profiles(cls) -> Mapping[str, Type]:
-        return {"python_object": KiaraArray}
-
-    @classmethod
-    def retrieve_serialized_value_type(cls) -> str:
-        return "array"
-
-    @classmethod
-    def retrieve_supported_serialization_profile(cls) -> str:
-        return "feather"
-
-    def to__python_object(self, data: SerializedData, **config: Any):
-
-        assert "array.arrow" in data.get_keys() and len(list(data.get_keys())) == 1
-
-        chunks = data.get_serialized_data("array.arrow")
-
-        # TODO: support multiple chunks
-        assert chunks.get_number_of_chunks() == 1
-        files = list(chunks.get_chunks(as_files=True, symlink_ok=True))
-        assert len(files) == 1
-
-        array_file = files[0]
-
-        array = KiaraArray(data_path=array_file)
-        return array
-
-
 class DeserializeTableModule(DeserializeValueModule):
 
     _module_type_name = "load.table"
 
     @classmethod
     def retrieve_supported_target_profiles(cls) -> Mapping[str, Type]:
         return {"python_object": KiaraTable}
@@ -206,14 +174,106 @@
 
         table: pa.Table = table_value.data.arrow_table
         column = table.column(column_name)
 
         outputs.set_value("array", column)
 
 
+class MergeTableConfig(KiaraModuleConfig):
+
+    inputs_schema: Dict[str, ValueSchema] = Field(
+        description="A dict describing the inputs for this merge process."
+    )
+
+
+class MergeTableModule(KiaraModule):
+    """Create a table from other tables and/or arrays."""
+
+    _module_type_name = "table.merge"
+    _config_cls = MergeTableConfig
+
+    def create_inputs_schema(
+        self,
+    ) -> ValueSetSchema:
+
+        input_schema_dict = self.get_config_value("inputs_schema")
+        return input_schema_dict
+
+    def create_outputs_schema(
+        self,
+    ) -> ValueSetSchema:
+
+        outputs = {
+            "table": {
+                "type": "table",
+                "doc": "The merged table, including all source tables and columns.",
+            }
+        }
+        return outputs
+
+    def process(self, inputs: ValueMap, outputs: ValueMap) -> None:
+
+        import pyarrow as pa
+
+        inputs_schema: Dict[str, Any] = self.get_config_value("inputs_schema")
+
+        sources = {}
+        for field_name in inputs_schema.keys():
+            sources[field_name] = inputs.get_value_data(field_name)
+
+        len_dict = {}
+        arrays = []
+        column_names = []
+        for source_key, table_or_column in sources.items():
+
+            if isinstance(table_or_column, KiaraTable):
+                rows = table_or_column.num_rows
+                for name in table_or_column.column_names:
+                    column = table_or_column.arrow_table.column(name)
+                    arrays.append(column)
+                    if name in column_names:
+                        raise KiaraProcessingException(
+                            f"Can't merge table: duplicate column name '{name}'."
+                        )
+                    column_names.append(name)
+
+            elif isinstance(table_or_column, KiaraArray):
+                rows = len(table_or_column)
+                arrays.append(table_or_column.arrow_array)
+                column_names.append(source_key)
+            else:
+                raise KiaraProcessingException(
+                    f"Can't merge table: invalid type '{type(table_or_column)}' for source '{source_key}'."
+                )
+
+            len_dict[source_key] = rows
+
+        all_rows = None
+        for source_key, rows in len_dict.items():
+            if all_rows is None:
+                all_rows = rows
+            else:
+                if all_rows != rows:
+                    all_rows = None
+                    break
+
+        if all_rows is None:
+            len_str = ""
+            for name, rows in len_dict.items():
+                len_str = f" {name} ({rows})"
+
+            raise KiaraProcessingException(
+                f"Can't merge table, sources have different lengths:{len_str}"
+            )
+
+        table = pa.Table.from_arrays(arrays=arrays, names=column_names)
+
+        outputs.set_value("table", table)
+
+
 class QueryTableSQLModuleConfig(KiaraModuleConfig):
 
     query: Optional[str] = Field(
         description="The query to execute. If not specified, the user will be able to provide their own.",
         default=None,
     )
     relation_name: Optional[str] = Field(
```

### Comparing `kiara_plugin.tabular-0.4.8/src/kiara_plugin/tabular/utils.py` & `kiara_plugin.tabular-0.4.9/src/kiara_plugin/tabular/utils.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.tabular-0.4.8/src/kiara_plugin.tabular.egg-info/PKG-INFO` & `kiara_plugin.tabular-0.4.9/src/kiara_plugin.tabular.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiara-plugin.tabular
-Version: 0.4.8
+Version: 0.4.9
 Summary: A set of modules (and pipelines) for Kiara.
 Home-page: https://github.com/DHARPA-Project/kiara_plugin.tabular
 Author: Markus Binsteiner
 Author-email: markus@frkl.io
 License: MPL-2.0
 Platform: any
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `kiara_plugin.tabular-0.4.8/src/kiara_plugin.tabular.egg-info/SOURCES.txt` & `kiara_plugin.tabular-0.4.9/src/kiara_plugin.tabular.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -22,15 +22,18 @@
 .github/workflows/build-windows.yaml
 ci/conda/build-conda-packages.sh
 ci/conda/kiara_plugin.tabular/meta.yaml.template
 docs/SUMMARY.md
 docs/index.md
 docs/usage.md
 docs/stylesheets/extra.css
-examples/data/.gitkeep
+examples/data/Readme.md
+examples/data/journals/JournalEdges1902.csv
+examples/data/journals/JournalNodes1902.csv
+examples/data/journals/Readme.md
 scripts/documentation/gen_api_doc_pages.py
 scripts/documentation/gen_info_pages.py
 scripts/documentation/gen_module_doc.py
 src/kiara_plugin.tabular.egg-info/PKG-INFO
 src/kiara_plugin.tabular.egg-info/SOURCES.txt
 src/kiara_plugin.tabular.egg-info/dependency_links.txt
 src/kiara_plugin.tabular.egg-info/entry_points.txt
@@ -43,16 +46,19 @@
 src/kiara_plugin/tabular/utils.py
 src/kiara_plugin/tabular/data_types/__init__.py
 src/kiara_plugin/tabular/data_types/db.py
 src/kiara_plugin/tabular/data_types/table.py
 src/kiara_plugin/tabular/models/__init__.py
 src/kiara_plugin/tabular/models/db.py
 src/kiara_plugin/tabular/models/table.py
+src/kiara_plugin/tabular/modules/__init__.py
+src/kiara_plugin/tabular/modules/array/__init__.py
+src/kiara_plugin/tabular/modules/db/__init__.py
+src/kiara_plugin/tabular/modules/table/__init__.py
 src/kiara_plugin/tabular/pipelines/.gitkeep
 src/kiara_plugin/tabular/pipelines/__init__.py
-src/kiara_plugin/tabular/pipelines/load.table.yaml
+src/kiara_plugin/tabular/pipelines/extract_date_array.from.table.yaml
+src/kiara_plugin/tabular/pipelines/import.table.from.csv_file.yaml
+src/kiara_plugin/tabular/pipelines/import.table.from.text_file_bundle.yaml
 src/kiara_plugin/tabular/resources/.gitkeep
-src/kiara_plugin/tabular/tabular/__init__.py
-src/kiara_plugin/tabular/tabular/db.py
-src/kiara_plugin/tabular/tabular/table.py
 tests/conftest.py
 tests/test_kiara_modules_default.py
```

### Comparing `kiara_plugin.tabular-0.4.8/src/kiara_plugin.tabular.egg-info/requires.txt` & `kiara_plugin.tabular-0.4.9/src/kiara_plugin.tabular.egg-info/requires.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,73 +1,74 @@
 duckdb>=0.3.4
-kiara>=0.4.13
+kiara>=0.4.14
 pandas>=1.4.0
+polars>=0.13.52
 pyarrow>=7.0.0
 sqlite-utils>=3.20
 
 [all]
 
 [all_dev]
-setup-cfg-fmt>=1.16.0
-types-python-dateutil
-ipython
-wheel
-pp-ez>=0.2.0
-mike>=1.0.1
-tox>=3.21.2
+pre-commit>=2.9.3
 pytest>=6.2.2
-flake8>=3.8.4
+types-python-dateutil
 pytest-cov>=2.11.1
-mkdocstrings-python-legacy
-mkdocs-macros-plugin<0.6.0,>=0.5.0
-mkdocs-section-index>0.3.0
 types-pkg-resources
+flake8>=3.8.4
 mkdocs-literate-nav>=0.4.0
-mypy>=0.800
+cruft>=2.6.0
+mkdocs-section-index>0.3.0
+wheel
+mike>=1.0.1
+mknotebooks>=0.7.0
+pp-ez>=0.2.0
+setup-cfg-fmt>=1.16.0
+ipython
+black
+tox>=3.21.2
+pip-licenses>=3.3.0
 coveralls>=3.2.0
-watchgod>=0.6
-pre-commit>=2.9.3
-icecream>=2.1.0
 mkdocs-awesome-pages-plugin>=2.5.0
+mkdocs-macros-plugin<0.6.0,>=0.5.0
+icecream>=2.1.0
+watchgod>=0.6
+mkdocstrings-python-legacy
 mkdocs-material>=8.0.0
-pip-licenses>=3.3.0
-black
-cruft>=2.6.0
-mknotebooks>=0.7.0
+mypy>=0.800
 
 [all_dev:python_version >= "3.7"]
 mkdocs-gen-files>=0.3.1
 
 [dev_all]
-setup-cfg-fmt>=1.16.0
-types-python-dateutil
-ipython
-wheel
-pp-ez>=0.2.0
-mike>=1.0.1
-tox>=3.21.2
+pre-commit>=2.9.3
 pytest>=6.2.2
-flake8>=3.8.4
+types-python-dateutil
 pytest-cov>=2.11.1
-mkdocstrings-python-legacy
-mkdocs-macros-plugin<0.6.0,>=0.5.0
-mkdocs-section-index>0.3.0
 types-pkg-resources
+flake8>=3.8.4
 mkdocs-literate-nav>=0.4.0
-mypy>=0.800
+cruft>=2.6.0
+mkdocs-section-index>0.3.0
+wheel
+mike>=1.0.1
+mknotebooks>=0.7.0
+pp-ez>=0.2.0
+setup-cfg-fmt>=1.16.0
+ipython
+black
+tox>=3.21.2
+pip-licenses>=3.3.0
 coveralls>=3.2.0
-watchgod>=0.6
-pre-commit>=2.9.3
-icecream>=2.1.0
 mkdocs-awesome-pages-plugin>=2.5.0
+mkdocs-macros-plugin<0.6.0,>=0.5.0
+icecream>=2.1.0
+watchgod>=0.6
+mkdocstrings-python-legacy
 mkdocs-material>=8.0.0
-pip-licenses>=3.3.0
-black
-cruft>=2.6.0
-mknotebooks>=0.7.0
+mypy>=0.800
 
 [dev_all:python_version >= "3.7"]
 mkdocs-gen-files>=0.3.1
 
 [dev_documentation]
 icecream>=2.1.0
 mike>=1.0.1
```

