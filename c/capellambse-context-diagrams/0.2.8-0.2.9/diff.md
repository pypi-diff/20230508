# Comparing `tmp/capellambse-context-diagrams-0.2.8.tar.gz` & `tmp/capellambse-context-diagrams-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "capellambse-context-diagrams-0.2.8.tar", last modified: Mon Dec  5 13:36:53 2022, max compression
+gzip compressed data, was "capellambse-context-diagrams-0.2.9.tar", last modified: Tue Jan 17 16:17:42 2023, max compression
```

## Comparing `capellambse-context-diagrams-0.2.8.tar` & `capellambse-context-diagrams-0.2.9.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-05 13:36:53.132012 capellambse-context-diagrams-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (122)      748 2022-12-05 13:36:38.000000 capellambse-context-diagrams-0.2.8/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-05 13:36:53.124012 capellambse-context-diagrams-0.2.8/.github/
--rw-r--r--   0 runner    (1001) docker     (122)      217 2022-12-05 13:36:38.000000 capellambse-context-diagrams-0.2.8/.github/CODEOWNERS
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-05 13:36:53.124012 capellambse-context-diagrams-0.2.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     2262 2022-12-05 13:36:38.000000 capellambse-context-diagrams-0.2.8/.github/workflows/build-test-publish.yml
--rw-r--r--   0 runner    (1001) docker     (122)      643 2022-12-05 13:36:38.000000 capellambse-context-diagrams-0.2.8/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1091 2022-12-05 13:36:38.000000 capellambse-context-diagrams-0.2.8/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (122)     5269 2022-12-05 13:36:38.000000 capellambse-context-diagrams-0.2.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     2094 2022-12-05 13:36:38.000000 capellambse-context-diagrams-0.2.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     8926 2022-12-05 13:36:38.000000 capellambse-context-diagrams-0.2.8/CONTRIBUTING.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-05 13:36:53.124012 capellambse-context-diagrams-0.2.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (122)    11358 2022-12-05 13:36:38.000000 capellambse-context-diagrams-0.2.8/LICENSES/Apache-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (122)     7048 2022-12-05 13:36:38.000000 capellambse-context-diagrams-0.2.8/LICENSES/CC0-1.0.txt
--rw-r--r--   0 runner    (1001) docker     (122)    14197 2022-12-05 13:36:38.000000 capellambse-context-diagrams-0.2.8/LICENSES/EPL-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (122)    17333 2022-12-05 13:36:53.132012 capellambse-context-diagrams-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3176 2022-12-05 13:36:38.000000 capellambse-context-diagrams-0.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-05 13:36:53.124012 capellambse-context-diagrams-0.2.8/capellambse_context_diagrams/
--rw-r--r--   0 runner    (1001) docker     (122)     4995 2022-12-05 13:36:38.000000 capellambse-context-diagrams-0.2.8/capellambse_context_diagrams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8922 2022-12-05 13:36:38.000000 capellambse-context-diagrams-0.2.8/capellambse_context_diagrams/_elkjs.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-05 13:36:53.128012 capellambse-context-diagrams-0.2.8/capellambse_context_diagrams/collectors/
--rw-r--r--   0 runner    (1001) docker     (122)     1333 2022-12-05 13:36:38.000000 capellambse-context-diagrams-0.2.8/capellambse_context_diagrams/collectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5535 2022-12-05 13:36:38.000000 capellambse-context-diagrams-0.2.8/capellambse_context_diagrams/collectors/default.py
--rw-r--r--   0 runner    (1001) docker     (122)    10890 2022-12-05 13:36:38.000000 capellambse-context-diagrams-0.2.8/capellambse_context_diagrams/collectors/exchanges.py
--rw-r--r--   0 runner    (1001) docker     (122)     5869 2022-12-05 13:36:38.000000 capellambse-context-diagrams-0.2.8/capellambse_context_diagrams/collectors/generic.py
--rw-r--r--   0 runner    (1001) docker     (122)     3530 2022-12-05 13:36:38.000000 capellambse-context-diagrams-0.2.8/capellambse_context_diagrams/collectors/makers.py
--rw-r--r--   0 runner    (1001) docker     (122)     6148 2022-12-05 13:36:38.000000 capellambse-context-diagrams-0.2.8/capellambse_context_diagrams/collectors/portless.py
--rw-r--r--   0 runner    (1001) docker     (122)    10626 2022-12-05 13:36:38.000000 capellambse-context-diagrams-0.2.8/capellambse_context_diagrams/context.py
--rw-r--r--   0 runner    (1001) docker     (122)      548 2022-12-05 13:36:38.000000 capellambse-context-diagrams-0.2.8/capellambse_context_diagrams/elk.js
--rw-r--r--   0 runner    (1001) docker     (122)      815 2022-12-05 13:36:38.000000 capellambse-context-diagrams-0.2.8/capellambse_context_diagrams/elkgraph-json.js
--rw-r--r--   0 runner    (1001) docker     (122)     7597 2022-12-05 13:36:38.000000 capellambse-context-diagrams-0.2.8/capellambse_context_diagrams/elkgraph-to-sprotty.js
--rw-r--r--   0 runner    (1001) docker     (122)     3206 2022-12-05 13:36:38.000000 capellambse-context-diagrams-0.2.8/capellambse_context_diagrams/filters.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-05 13:36:38.000000 capellambse-context-diagrams-0.2.8/capellambse_context_diagrams/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)     8776 2022-12-05 13:36:38.000000 capellambse-context-diagrams-0.2.8/capellambse_context_diagrams/serializers.py
--rw-r--r--   0 runner    (1001) docker     (122)     1672 2022-12-05 13:36:38.000000 capellambse-context-diagrams-0.2.8/capellambse_context_diagrams/styling.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-05 13:36:53.124012 capellambse-context-diagrams-0.2.8/capellambse_context_diagrams.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    17333 2022-12-05 13:36:53.000000 capellambse-context-diagrams-0.2.8/capellambse_context_diagrams.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2237 2022-12-05 13:36:53.000000 capellambse-context-diagrams-0.2.8/capellambse_context_diagrams.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-05 13:36:53.000000 capellambse-context-diagrams-0.2.8/capellambse_context_diagrams.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       84 2022-12-05 13:36:53.000000 capellambse-context-diagrams-0.2.8/capellambse_context_diagrams.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-05 13:36:52.000000 capellambse-context-diagrams-0.2.8/capellambse_context_diagrams.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      224 2022-12-05 13:36:53.000000 capellambse-context-diagrams-0.2.8/capellambse_context_diagrams.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       55 2022-12-05 13:36:53.000000 capellambse-context-diagrams-0.2.8/capellambse_context_diagrams.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-05 13:36:53.128012 capellambse-context-diagrams-0.2.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-05 13:36:53.120012 capellambse-context-diagrams-0.2.8/docs/assets/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-05 13:36:53.128012 capellambse-context-diagrams-0.2.8/docs/assets/images/
--rw-r--r--   0 runner    (1001) docker     (122)    27083 2022-12-05 13:36:38.000000 capellambse-context-diagrams-0.2.8/docs/assets/images/Context of Left.svg
--rw-r--r--   0 runner    (1001) docker     (122)    31464 2022-12-05 13:36:38.000000 capellambse-context-diagrams-0.2.8/docs/assets/images/Interface Context of Left to right.svg
--rw-r--r--   0 runner    (1001) docker     (122)    15086 2022-12-05 13:36:38.000000 capellambse-context-diagrams-0.2.8/docs/assets/images/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (122)      136 2022-12-05 13:36:38.000000 capellambse-context-diagrams-0.2.8/docs/assets/images/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (122)      924 2022-12-05 13:36:38.000000 capellambse-context-diagrams-0.2.8/docs/assets/images/favicon.png
--rw-r--r--   0 runner    (1001) docker     (122)      136 2022-12-05 13:36:38.000000 capellambse-context-diagrams-0.2.8/docs/assets/images/favicon.png.license
--rw-r--r--   0 runner    (1001) docker     (122)      536 2022-12-05 13:36:38.000000 capellambse-context-diagrams-0.2.8/docs/credits.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-05 13:36:53.128012 capellambse-context-diagrams-0.2.8/docs/css/
--rw-r--r--   0 runner    (1001) docker     (122)      465 2022-12-05 13:36:38.000000 capellambse-context-diagrams-0.2.8/docs/css/base.css
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-05 13:36:53.128012 capellambse-context-diagrams-0.2.8/docs/extras/
--rw-r--r--   0 runner    (1001) docker     (122)     3440 2022-12-05 13:36:38.000000 capellambse-context-diagrams-0.2.8/docs/extras/filters.md
--rw-r--r--   0 runner    (1001) docker     (122)     4860 2022-12-05 13:36:38.000000 capellambse-context-diagrams-0.2.8/docs/extras/styling.md
--rw-r--r--   0 runner    (1001) docker     (122)     3752 2022-12-05 13:36:38.000000 capellambse-context-diagrams-0.2.8/docs/gen_images.py
--rw-r--r--   0 runner    (1001) docker     (122)     1193 2022-12-05 13:36:38.000000 capellambse-context-diagrams-0.2.8/docs/gen_ref_pages.py
--rw-r--r--   0 runner    (1001) docker     (122)     8340 2022-12-05 13:36:38.000000 capellambse-context-diagrams-0.2.8/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (122)      194 2022-12-05 13:36:38.000000 capellambse-context-diagrams-0.2.8/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (122)      768 2022-12-05 13:36:38.000000 capellambse-context-diagrams-0.2.8/docs/quickstart.md
--rw-r--r--   0 runner    (1001) docker     (122)      136 2022-12-05 13:36:38.000000 capellambse-context-diagrams-0.2.8/license_header.txt
--rw-r--r--   0 runner    (1001) docker     (122)     2612 2022-12-05 13:36:38.000000 capellambse-context-diagrams-0.2.8/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-05 13:36:53.120012 capellambse-context-diagrams-0.2.8/overrides/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-05 13:36:53.120012 capellambse-context-diagrams-0.2.8/overrides/.icons/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-05 13:36:53.128012 capellambse-context-diagrams-0.2.8/overrides/.icons/custom/
--rw-r--r--   0 runner    (1001) docker     (122)     1451 2022-12-05 13:36:38.000000 capellambse-context-diagrams-0.2.8/overrides/.icons/custom/db.svg
--rw-r--r--   0 runner    (1001) docker     (122)     4810 2022-12-05 13:36:38.000000 capellambse-context-diagrams-0.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-12-05 13:36:53.132012 capellambse-context-diagrams-0.2.8/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)      202 2022-12-05 13:36:38.000000 capellambse-context-diagrams-0.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-05 13:36:53.128012 capellambse-context-diagrams-0.2.8/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      539 2022-12-05 13:36:38.000000 capellambse-context-diagrams-0.2.8/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-05 13:36:53.132012 capellambse-context-diagrams-0.2.8/tests/data/
--rw-r--r--   0 runner    (1001) docker     (122)      209 2022-12-05 13:36:38.000000 capellambse-context-diagrams-0.2.8/tests/data/.project
--rw-r--r--   0 runner    (1001) docker     (122)      136 2022-12-05 13:36:38.000000 capellambse-context-diagrams-0.2.8/tests/data/.project.license
--rw-r--r--   0 runner    (1001) docker     (122)      577 2022-12-05 13:36:38.000000 capellambse-context-diagrams-0.2.8/tests/data/ContextDiagram.afm
--rw-r--r--   0 runner    (1001) docker     (122)      136 2022-12-05 13:36:38.000000 capellambse-context-diagrams-0.2.8/tests/data/ContextDiagram.afm.license
--rw-r--r--   0 runner    (1001) docker     (122)   930500 2022-12-05 13:36:38.000000 capellambse-context-diagrams-0.2.8/tests/data/ContextDiagram.aird
--rw-r--r--   0 runner    (1001) docker     (122)      136 2022-12-05 13:36:38.000000 capellambse-context-diagrams-0.2.8/tests/data/ContextDiagram.aird.license
--rw-r--r--   0 runner    (1001) docker     (122)   359009 2022-12-05 13:36:38.000000 capellambse-context-diagrams-0.2.8/tests/data/ContextDiagram.capella
--rw-r--r--   0 runner    (1001) docker     (122)      136 2022-12-05 13:36:38.000000 capellambse-context-diagrams-0.2.8/tests/data/ContextDiagram.capella.license
--rw-r--r--   0 runner    (1001) docker     (122)      813 2022-12-05 13:36:38.000000 capellambse-context-diagrams-0.2.8/tests/test_capability_diagrams.py
--rw-r--r--   0 runner    (1001) docker     (122)     3845 2022-12-05 13:36:38.000000 capellambse-context-diagrams-0.2.8/tests/test_context_diagrams.py
--rw-r--r--   0 runner    (1001) docker     (122)     4804 2022-12-05 13:36:38.000000 capellambse-context-diagrams-0.2.8/tests/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (122)      766 2022-12-05 13:36:38.000000 capellambse-context-diagrams-0.2.8/tests/test_interface_diagrams.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 16:17:42.092424 capellambse-context-diagrams-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-01-17 16:17:23.000000 capellambse-context-diagrams-0.2.9/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 16:17:42.084424 capellambse-context-diagrams-0.2.9/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-01-17 16:17:23.000000 capellambse-context-diagrams-0.2.9/.github/CODEOWNERS
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 16:17:42.084424 capellambse-context-diagrams-0.2.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-01-17 16:17:23.000000 capellambse-context-diagrams-0.2.9/.github/workflows/build-test-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-01-17 16:17:23.000000 capellambse-context-diagrams-0.2.9/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-01-17 16:17:23.000000 capellambse-context-diagrams-0.2.9/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-01-17 16:17:23.000000 capellambse-context-diagrams-0.2.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-01-17 16:17:23.000000 capellambse-context-diagrams-0.2.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8926 2023-01-17 16:17:23.000000 capellambse-context-diagrams-0.2.9/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 16:17:42.084424 capellambse-context-diagrams-0.2.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-01-17 16:17:23.000000 capellambse-context-diagrams-0.2.9/LICENSES/Apache-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-01-17 16:17:23.000000 capellambse-context-diagrams-0.2.9/LICENSES/CC0-1.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14197 2023-01-17 16:17:23.000000 capellambse-context-diagrams-0.2.9/LICENSES/EPL-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    17333 2023-01-17 16:17:42.092424 capellambse-context-diagrams-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-01-17 16:17:23.000000 capellambse-context-diagrams-0.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 16:17:42.084424 capellambse-context-diagrams-0.2.9/capellambse_context_diagrams/
+-rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-01-17 16:17:23.000000 capellambse-context-diagrams-0.2.9/capellambse_context_diagrams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8922 2023-01-17 16:17:23.000000 capellambse-context-diagrams-0.2.9/capellambse_context_diagrams/_elkjs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 16:17:42.084424 capellambse-context-diagrams-0.2.9/capellambse_context_diagrams/collectors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-01-17 16:17:23.000000 capellambse-context-diagrams-0.2.9/capellambse_context_diagrams/collectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5535 2023-01-17 16:17:23.000000 capellambse-context-diagrams-0.2.9/capellambse_context_diagrams/collectors/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10890 2023-01-17 16:17:23.000000 capellambse-context-diagrams-0.2.9/capellambse_context_diagrams/collectors/exchanges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-01-17 16:17:23.000000 capellambse-context-diagrams-0.2.9/capellambse_context_diagrams/collectors/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-01-17 16:17:23.000000 capellambse-context-diagrams-0.2.9/capellambse_context_diagrams/collectors/makers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-01-17 16:17:23.000000 capellambse-context-diagrams-0.2.9/capellambse_context_diagrams/collectors/portless.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10667 2023-01-17 16:17:23.000000 capellambse-context-diagrams-0.2.9/capellambse_context_diagrams/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-01-17 16:17:23.000000 capellambse-context-diagrams-0.2.9/capellambse_context_diagrams/elk.js
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-01-17 16:17:23.000000 capellambse-context-diagrams-0.2.9/capellambse_context_diagrams/elkgraph-json.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7597 2023-01-17 16:17:23.000000 capellambse-context-diagrams-0.2.9/capellambse_context_diagrams/elkgraph-to-sprotty.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-01-17 16:17:23.000000 capellambse-context-diagrams-0.2.9/capellambse_context_diagrams/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-17 16:17:23.000000 capellambse-context-diagrams-0.2.9/capellambse_context_diagrams/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-01-17 16:17:23.000000 capellambse-context-diagrams-0.2.9/capellambse_context_diagrams/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-01-17 16:17:23.000000 capellambse-context-diagrams-0.2.9/capellambse_context_diagrams/styling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 16:17:42.084424 capellambse-context-diagrams-0.2.9/capellambse_context_diagrams.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17333 2023-01-17 16:17:42.000000 capellambse-context-diagrams-0.2.9/capellambse_context_diagrams.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-01-17 16:17:42.000000 capellambse-context-diagrams-0.2.9/capellambse_context_diagrams.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-17 16:17:42.000000 capellambse-context-diagrams-0.2.9/capellambse_context_diagrams.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-01-17 16:17:42.000000 capellambse-context-diagrams-0.2.9/capellambse_context_diagrams.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-17 16:17:41.000000 capellambse-context-diagrams-0.2.9/capellambse_context_diagrams.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-01-17 16:17:42.000000 capellambse-context-diagrams-0.2.9/capellambse_context_diagrams.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-01-17 16:17:42.000000 capellambse-context-diagrams-0.2.9/capellambse_context_diagrams.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 16:17:42.088424 capellambse-context-diagrams-0.2.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 16:17:42.080424 capellambse-context-diagrams-0.2.9/docs/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 16:17:42.088424 capellambse-context-diagrams-0.2.9/docs/assets/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    27083 2023-01-17 16:17:23.000000 capellambse-context-diagrams-0.2.9/docs/assets/images/Context of Left.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    31464 2023-01-17 16:17:23.000000 capellambse-context-diagrams-0.2.9/docs/assets/images/Interface Context of Left to right.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-01-17 16:17:23.000000 capellambse-context-diagrams-0.2.9/docs/assets/images/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-01-17 16:17:23.000000 capellambse-context-diagrams-0.2.9/docs/assets/images/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-01-17 16:17:23.000000 capellambse-context-diagrams-0.2.9/docs/assets/images/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-01-17 16:17:23.000000 capellambse-context-diagrams-0.2.9/docs/assets/images/favicon.png.license
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-01-17 16:17:23.000000 capellambse-context-diagrams-0.2.9/docs/credits.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 16:17:42.088424 capellambse-context-diagrams-0.2.9/docs/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-01-17 16:17:23.000000 capellambse-context-diagrams-0.2.9/docs/css/base.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 16:17:42.088424 capellambse-context-diagrams-0.2.9/docs/extras/
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-01-17 16:17:23.000000 capellambse-context-diagrams-0.2.9/docs/extras/filters.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-01-17 16:17:23.000000 capellambse-context-diagrams-0.2.9/docs/extras/styling.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-01-17 16:17:23.000000 capellambse-context-diagrams-0.2.9/docs/gen_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-01-17 16:17:23.000000 capellambse-context-diagrams-0.2.9/docs/gen_ref_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8340 2023-01-17 16:17:23.000000 capellambse-context-diagrams-0.2.9/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-01-17 16:17:23.000000 capellambse-context-diagrams-0.2.9/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-01-17 16:17:23.000000 capellambse-context-diagrams-0.2.9/docs/quickstart.md
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-01-17 16:17:23.000000 capellambse-context-diagrams-0.2.9/license_header.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-01-17 16:17:23.000000 capellambse-context-diagrams-0.2.9/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 16:17:42.080424 capellambse-context-diagrams-0.2.9/overrides/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 16:17:42.080424 capellambse-context-diagrams-0.2.9/overrides/.icons/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 16:17:42.088424 capellambse-context-diagrams-0.2.9/overrides/.icons/custom/
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-01-17 16:17:23.000000 capellambse-context-diagrams-0.2.9/overrides/.icons/custom/db.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4810 2023-01-17 16:17:23.000000 capellambse-context-diagrams-0.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-17 16:17:42.092424 capellambse-context-diagrams-0.2.9/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      202 2023-01-17 16:17:23.000000 capellambse-context-diagrams-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 16:17:42.088424 capellambse-context-diagrams-0.2.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-01-17 16:17:23.000000 capellambse-context-diagrams-0.2.9/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 16:17:42.092424 capellambse-context-diagrams-0.2.9/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-01-17 16:17:23.000000 capellambse-context-diagrams-0.2.9/tests/data/.project
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-01-17 16:17:23.000000 capellambse-context-diagrams-0.2.9/tests/data/.project.license
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-01-17 16:17:23.000000 capellambse-context-diagrams-0.2.9/tests/data/ContextDiagram.afm
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-01-17 16:17:23.000000 capellambse-context-diagrams-0.2.9/tests/data/ContextDiagram.afm.license
+-rw-r--r--   0 runner    (1001) docker     (123)   930500 2023-01-17 16:17:23.000000 capellambse-context-diagrams-0.2.9/tests/data/ContextDiagram.aird
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-01-17 16:17:23.000000 capellambse-context-diagrams-0.2.9/tests/data/ContextDiagram.aird.license
+-rw-r--r--   0 runner    (1001) docker     (123)   359009 2023-01-17 16:17:23.000000 capellambse-context-diagrams-0.2.9/tests/data/ContextDiagram.capella
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-01-17 16:17:23.000000 capellambse-context-diagrams-0.2.9/tests/data/ContextDiagram.capella.license
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-01-17 16:17:23.000000 capellambse-context-diagrams-0.2.9/tests/test_capability_diagrams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-01-17 16:17:23.000000 capellambse-context-diagrams-0.2.9/tests/test_context_diagrams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4834 2023-01-17 16:17:23.000000 capellambse-context-diagrams-0.2.9/tests/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-01-17 16:17:23.000000 capellambse-context-diagrams-0.2.9/tests/test_interface_diagrams.py
```

### Comparing `capellambse-context-diagrams-0.2.8/.gitattributes` & `capellambse-context-diagrams-0.2.9/.gitattributes`

 * *Files identical despite different names*

### Comparing `capellambse-context-diagrams-0.2.8/.github/workflows/build-test-publish.yml` & `capellambse-context-diagrams-0.2.9/.github/workflows/build-test-publish.yml`

 * *Files identical despite different names*

### Comparing `capellambse-context-diagrams-0.2.8/.github/workflows/docs.yml` & `capellambse-context-diagrams-0.2.9/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `capellambse-context-diagrams-0.2.8/.github/workflows/lint.yml` & `capellambse-context-diagrams-0.2.9/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `capellambse-context-diagrams-0.2.8/.gitignore` & `capellambse-context-diagrams-0.2.9/.gitignore`

 * *Files identical despite different names*

### Comparing `capellambse-context-diagrams-0.2.8/.pre-commit-config.yaml` & `capellambse-context-diagrams-0.2.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `capellambse-context-diagrams-0.2.8/CONTRIBUTING.md` & `capellambse-context-diagrams-0.2.9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `capellambse-context-diagrams-0.2.8/LICENSES/Apache-2.0.txt` & `capellambse-context-diagrams-0.2.9/LICENSES/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `capellambse-context-diagrams-0.2.8/LICENSES/CC0-1.0.txt` & `capellambse-context-diagrams-0.2.9/LICENSES/CC0-1.0.txt`

 * *Files identical despite different names*

### Comparing `capellambse-context-diagrams-0.2.8/LICENSES/EPL-2.0.txt` & `capellambse-context-diagrams-0.2.9/LICENSES/EPL-2.0.txt`

 * *Files identical despite different names*

### Comparing `capellambse-context-diagrams-0.2.8/PKG-INFO` & `capellambse-context-diagrams-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: capellambse-context-diagrams
-Version: 0.2.8
+Version: 0.2.9
 Summary: Extension for python-capella-mbse that adds automatically generated context diagrams for arbitrary model elements.
 Author: DB Netz AG
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `capellambse-context-diagrams-0.2.8/README.md` & `capellambse-context-diagrams-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `capellambse-context-diagrams-0.2.8/capellambse_context_diagrams/__init__.py` & `capellambse-context-diagrams-0.2.9/capellambse_context_diagrams/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from __future__ import annotations
 
 import collections.abc as cabc
 import logging
 import typing as t
 from importlib import metadata
 
-from capellambse.aird import COLORS, CSSdef, capstyle
+from capellambse.diagram import COLORS, CSSdef, capstyle
 from capellambse.model import common
 from capellambse.model.crosslayer import fa
 from capellambse.model.layers import ctx, la, oa, pa
 from capellambse.model.modeltypes import DiagramType
 
 from . import context
```

### Comparing `capellambse-context-diagrams-0.2.8/capellambse_context_diagrams/_elkjs.py` & `capellambse-context-diagrams-0.2.9/capellambse_context_diagrams/_elkjs.py`

 * *Files identical despite different names*

### Comparing `capellambse-context-diagrams-0.2.8/capellambse_context_diagrams/collectors/__init__.py` & `capellambse-context-diagrams-0.2.9/capellambse_context_diagrams/collectors/__init__.py`

 * *Files identical despite different names*

### Comparing `capellambse-context-diagrams-0.2.8/capellambse_context_diagrams/collectors/default.py` & `capellambse-context-diagrams-0.2.9/capellambse_context_diagrams/collectors/default.py`

 * *Files identical despite different names*

### Comparing `capellambse-context-diagrams-0.2.8/capellambse_context_diagrams/collectors/exchanges.py` & `capellambse-context-diagrams-0.2.9/capellambse_context_diagrams/collectors/exchanges.py`

 * *Files identical despite different names*

### Comparing `capellambse-context-diagrams-0.2.8/capellambse_context_diagrams/collectors/generic.py` & `capellambse-context-diagrams-0.2.9/capellambse_context_diagrams/collectors/generic.py`

 * *Files identical despite different names*

### Comparing `capellambse-context-diagrams-0.2.8/capellambse_context_diagrams/collectors/makers.py` & `capellambse-context-diagrams-0.2.9/capellambse_context_diagrams/collectors/makers.py`

 * *Files identical despite different names*

### Comparing `capellambse-context-diagrams-0.2.8/capellambse_context_diagrams/collectors/portless.py` & `capellambse-context-diagrams-0.2.9/capellambse_context_diagrams/collectors/portless.py`

 * *Files identical despite different names*

### Comparing `capellambse-context-diagrams-0.2.8/capellambse_context_diagrams/context.py` & `capellambse-context-diagrams-0.2.9/capellambse_context_diagrams/context.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from __future__ import annotations
 
 import collections.abc as cabc
 import json
 import logging
 import typing as t
 
-from capellambse import aird
+from capellambse import diagram as cdiagram
 from capellambse.model import common, diagram, modeltypes
 
 from . import _elkjs, filters, serializers, styling
 from .collectors import exchanges, get_elkdata
 
 logger = logging.getLogger(__name__)
 
@@ -136,19 +136,19 @@
     display_symbols_as_boxes
         Display objects that are normally displayed as symbol as a
         simple box instead, with the symbol being the box' icon. This
         avoids the object of interest to become one giant, oversized
         symbol in the middle of the diagram, and instead keeps the
         symbol small and only enlarges the surrounding box.
     serializer
-        The serializer builds an `aird.Diagram` via
+        The serializer builds a `diagram.Diagram` via
         [`serializers.DiagramSerializer.make_diagram`][capellambse_context_diagrams.serializers.DiagramSerializer.make_diagram]
         by converting every
         [`_elkjs.ELKOutputChild`][capellambse_context_diagrams._elkjs.ELKOutputChild]
-        into an `aird.Box`, `aird.Edge` or `aird.Circle`.
+        into a `diagram.Box`, `diagram.Edge` or `diagram.Circle`.
     filters
         A list of filter names that are applied during collection of
         context. Currently this is only done in
         [`collectors.exchange_data_collector`][capellambse_context_diagrams.collectors.generic.exchange_data_collector].
     """
 
     def __init__(
@@ -187,15 +187,15 @@
             logger.warning("Unknown diagram type %r", self.styleclass)
             return modeltypes.DiagramType.UNKNOWN
 
     @property
     def nodes(self) -> common.MixedElementList:
         """Return a list of all nodes visible in this diagram."""
         adiagram = self.render(None)
-        assert isinstance(adiagram, aird.Diagram)
+        assert isinstance(adiagram, cdiagram.Diagram)
         allids = {e.uuid for e in iter(adiagram)}
         assert None not in allids
         elems = []
         for elemid in allids:
             assert elemid is not None
             try:
                 elem = self._model._loader[elemid]
@@ -244,15 +244,15 @@
         def __len__(self) -> int:
             return self._set.__len__()
 
     def _create_diagram(
         self,
         params: dict[str, t.Any],
         elkdata: _elkjs.ELKInputData | None = None,
-    ) -> aird.Diagram:
+    ) -> cdiagram.Diagram:
         try:
             data = elkdata or get_elkdata(self, params)
             layout = _elkjs.call_elkjs(data)
         except json.JSONDecodeError as error:
             logger.error(json.dumps(data, indent=4))
             raise error
         return self.serializer.make_diagram(layout)
@@ -279,15 +279,15 @@
     def name(self) -> str:  # type: ignore
         return f"Interface Context of {self.target.name}"
 
     def _create_diagram(
         self,
         params: dict[str, t.Any],
         elkdata: _elkjs.ELKInputData | None = None,
-    ) -> aird.Diagram:
+    ) -> cdiagram.Diagram:
         return super()._create_diagram(
             params,
             elkdata
             or exchanges.get_elkdata_for_exchanges(
                 self, exchanges.InterfaceContextCollector
             ),
         )
@@ -302,15 +302,15 @@
     def name(self) -> str:  # type: ignore
         return f"Interface Context of {self.target.name}"
 
     def _create_diagram(
         self,
         params: dict[str, t.Any],
         elkdata: _elkjs.ELKInputData | None = None,
-    ) -> aird.Diagram:
+    ) -> cdiagram.Diagram:
         return super()._create_diagram(
             params,
             elkdata
             or exchanges.get_elkdata_for_exchanges(
                 self, exchanges.FunctionalContextCollector
             ),
         )
```

### Comparing `capellambse-context-diagrams-0.2.8/capellambse_context_diagrams/elk.js` & `capellambse-context-diagrams-0.2.9/capellambse_context_diagrams/elk.js`

 * *Files identical despite different names*

### Comparing `capellambse-context-diagrams-0.2.8/capellambse_context_diagrams/elkgraph-json.js` & `capellambse-context-diagrams-0.2.9/capellambse_context_diagrams/elkgraph-json.js`

 * *Files identical despite different names*

### Comparing `capellambse-context-diagrams-0.2.8/capellambse_context_diagrams/elkgraph-to-sprotty.js` & `capellambse-context-diagrams-0.2.9/capellambse_context_diagrams/elkgraph-to-sprotty.js`

 * *Files identical despite different names*

### Comparing `capellambse-context-diagrams-0.2.8/capellambse_context_diagrams/filters.py` & `capellambse-context-diagrams-0.2.9/capellambse_context_diagrams/filters.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
 
 def exchange_items(obj: common.GenericElement) -> str:
     """Return `obj`'s `ExchangeItem`s wrapped in [E1,...] and separated
     by ','.
     """
     stringifier = importlib.import_module(
-        "capellambse.aird.parser._filters.global"
+        "capellambse.aird._filters.global"
     )._stringify_exchange_items
     return stringifier(obj, obj._model._loader)
 
 
 def exchange_name_and_items(
     obj: common.GenericElement, label: str | None = None
 ) -> str:
@@ -80,15 +80,15 @@
 def sort_exchange_items_label(
     value: bool,
     exchange: common.GenericElement,
     adjustments: dict[str, t.Any],
 ) -> None:
     """Sort the exchange items in the exchange label if value is true."""
     global_filters = importlib.import_module(
-        "capellambse.aird.parser._filters.global"
+        "capellambse.aird._filters.global"
     )
     adjustments["labels_text"] = global_filters._stringify_exchange_items(
         exchange, exchange._model._loader, value
     )
 
 
 RENDER_ADJUSTERS: dict[
```

### Comparing `capellambse-context-diagrams-0.2.8/capellambse_context_diagrams/serializers.py` & `capellambse-context-diagrams-0.2.9/capellambse_context_diagrams/serializers.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 # SPDX-FileCopyrightText: 2022 Copyright DB Netz AG and the capellambse-context-diagrams contributors
 # SPDX-License-Identifier: Apache-2.0
 
-"""This submodule provides a serializer that transform data from an ELK-
+"""This submodule provides a serializer that transforms data from an ELK-
 layouted diagram [_elkjs.ELKOutputData][capellambse_context_diagrams._elkjs.ELKOutputData]
 according to [_elkjs.ELKInputData][capellambse_context_diagrams._elkjs.ELKInputData].
 The pre-layouted data was collected with the functions from
 [collectors][capellambse_context_diagrams.collectors].
 """
 from __future__ import annotations
 
 import logging
 
-from capellambse import aird
-from capellambse.model import common
+from capellambse import diagram
 
 from . import _elkjs, collectors, context
 
 logger = logging.getLogger(__name__)
 
 ElkChildType = str
 """
@@ -28,86 +27,86 @@
 * `edge`
 * `junction`.
 """
 
 
 class DiagramSerializer:
     """Serialize an ``elk_diagram`` into an
-    [`aird.Diagram`][capellambse.aird.diagram.Diagram].
+    [`diagram.Diagram`][capellambse.diagram.Diagram].
 
     Attributes
     ----------
     model
         The [`MelodyModel`][capellambse.model.MelodyModel] instance.
-    aird_diagram
-        The created [`aird.Diagram`][capellambse.aird.diagram.Diagram]
+    diagram
+        The created [`diagram.Diagram`][capellambse.diagram.Diagram]
         instance.
     """
 
-    aird_diagram: aird.Diagram
+    diagram: diagram.Diagram
 
     def __init__(self, elk_diagram: context.ContextDiagram) -> None:
         self.model = elk_diagram.target._model
         self._diagram = elk_diagram
-        self._cache: dict[str, aird.Box] = {}
+        self._cache: dict[str, diagram.Box] = {}
 
-    def make_diagram(self, data: _elkjs.ELKOutputData) -> aird.Diagram:
-        """Transform a layouted diagram into an `aird.Diagram`.
+    def make_diagram(self, data: _elkjs.ELKOutputData) -> diagram.Diagram:
+        """Transform a layouted diagram into an `diagram.Diagram`.
 
         Parameters
         ----------
         data
             The diagram, including layouting information.
 
         Returns
         -------
         diagram
-            A [`aird.Diagram`][capellambse.aird.diagram.Diagram] constructed
+            A [`diagram.Diagram`][capellambse.diagram.Diagram] constructed
             from the input data.
         """
-        self.aird_diagram = aird.Diagram(
+        self.diagram = diagram.Diagram(
             self._diagram.name, styleclass=self._diagram.styleclass
         )
         for child in data["children"]:
-            self.deserialize_child(child, aird.Vector2D(), None)
+            self.deserialize_child(child, diagram.Vector2D(), None)
 
-        self.aird_diagram.calculate_viewport()
-        return self.aird_diagram
+        self.diagram.calculate_viewport()
+        return self.diagram
 
     def deserialize_child(
         self,
         child: _elkjs.ELKOutputChild,
-        ref: aird.Vector2D,
-        parent: aird.Box | aird.Edge | None,
+        ref: diagram.Vector2D,
+        parent: diagram.Box | diagram.Edge | None,
     ) -> None:
         """Converts a `child` into aird elements and adds it to the
         diagram.
 
         Parameters
         ----------
-        child : _elkjs.ELKOutputChild
+        child
             The child to deserialize.
-        ref : aird.Vector2D
+        ref
             The reference point of the child.
-        parent : aird.Box | aird.Edge | None
+        parent
             The parent of the child. This is either a box or an edge.
 
         See Also
         --------
-        [`aird.Box`][capellambse.aird.diagram.Box] : Box class type.
-        [`aird.Edge`][capellambse.aird.diagram.Edge] : Edge class type.
-        [`aird.Circle`][capellambse.aird.diagram.Circle] : Circle class
+        [`diagram.Box`][capellambse.diagram.Box] : Box class type.
+        [`diagram.Edge`][capellambse.diagram.Edge] : Edge class type.
+        [`diagram.Circle`][capellambse.diagram.Circle] : Circle class
             type.
-        [`aird.Diagram`][capellambse.aird.diagram.Diagram] : Diagram
+        [`diagram.Diagram`][capellambse.diagram.Diagram] : Diagram
             class type that stores all previously named classes.
         """
         styleclass: str | None = self.get_styleclass(child["id"])
-        element: aird.Box | aird.Edge
+        element: diagram.Box | diagram.Edge
         if child["type"] in {"node", "port"}:
-            assert parent is None or isinstance(parent, aird.Box)
+            assert parent is None or isinstance(parent, diagram.Box)
             has_symbol_cls = False
             try:
                 obj = self.model.by_uuid(child["id"])
                 has_symbol_cls = collectors.makers.is_symbol(obj)
             except KeyError:
                 logger.error(
                     "ModelObject could not be found: '%s'", child["id"]
@@ -119,96 +118,96 @@
                 or has_symbol_cls
                 and not self._diagram.target == obj
                 and not self._diagram.display_symbols_as_boxes
             ]
 
             ref += (child["position"]["x"], child["position"]["y"])  # type: ignore
             size = (child["size"]["width"], child["size"]["height"])  # type: ignore
-            element = aird.Box(
+            element = diagram.Box(
                 ref,
                 size,
                 uuid=child["id"],
                 parent=parent,
                 port=is_port,
                 styleclass=styleclass,
                 styleoverrides=self.get_styleoverrides(child),
             )
             element.JSON_TYPE = box_type
-            self.aird_diagram.add_element(element)
+            self.diagram.add_element(element)
             self._cache[child["id"]] = element
         elif child["type"] == "edge":
-            element = aird.Edge(
+            element = diagram.Edge(
                 [
                     ref + (point["x"], point["y"])
                     for point in child["routingPoints"]
                 ],
                 uuid=child["id"],
-                source=self.aird_diagram[child["sourceId"]],
-                target=self.aird_diagram[child["targetId"]],
+                source=self.diagram[child["sourceId"]],
+                target=self.diagram[child["targetId"]],
                 styleclass=styleclass,
                 styleoverrides=self.get_styleoverrides(child),
             )
-            self.aird_diagram.add_element(element)
+            self.diagram.add_element(element)
             self._cache[child["id"]] = element
         elif child["type"] == "label":
             assert parent is not None
-            if isinstance(parent, aird.Box) and not parent.port:
+            if isinstance(parent, diagram.Box) and not parent.port:
                 if parent.JSON_TYPE != "symbol":
                     parent.label = child["text"]
                 else:
-                    parent.label = aird.Box(
+                    parent.label = diagram.Box(
                         ref + (child["position"]["x"], child["position"]["y"]),
                         (child["size"]["width"], child["size"]["height"]),
                         label=child["text"],
                         # parent=parent,
                     )
             else:
-                assert isinstance(parent, aird.Edge)
+                assert isinstance(parent, diagram.Edge)
                 parent.labels = [
-                    aird.Box(
+                    diagram.Box(
                         ref + (child["position"]["x"], child["position"]["y"]),
                         (child["size"]["width"], child["size"]["height"]),
                         label=child["text"],
                         styleoverrides=self.get_styleoverrides(child),
                     )
                 ]
 
             element = parent
         elif child["type"] == "junction":
             uuid = child["id"].split("_", maxsplit=1)[0]
-            element = aird.Circle(
-                aird.Vector2D(**child["position"]),
+            element = diagram.Circle(
+                diagram.Vector2D(**child["position"]),
                 5,
                 uuid=child["id"],
                 styleclass=self.get_styleclass(uuid),
                 styleoverrides=self.get_styleoverrides(child),
             )
-            self.aird_diagram.add_element(element)
+            self.diagram.add_element(element)
         else:
             logger.warning("Received unknown type %s", child["type"])
             return
 
         for i in child.get("children", []):  # type: ignore
             self.deserialize_child(i, ref, element)
 
     def get_styleclass(self, uuid: str) -> str | None:
         """Return the style-class string from a given
         [`_elkjs.ELKOutputChild`][capellambse_context_diagrams._elkjs.ELKOutputChild].
         """
         styleclass: str | None
         try:
             melodyobj = self._diagram._model.by_uuid(uuid)
-            styleclass = get_styleclass(melodyobj)
+            styleclass = diagram.get_styleclass(melodyobj)
         except KeyError:
             styleclass = None
         return styleclass
 
     def get_styleoverrides(
         self, child: _elkjs.ELKOutputChild
-    ) -> aird.diagram._StyleOverrides | None:
+    ) -> diagram.StyleOverrides | None:
         """Return
         [`styling.CSSStyles`][capellambse_context_diagrams.styling.CSSStyles]
         from a given
         [`_elkjs.ELKOutputChild`][capellambse_context_diagrams._elkjs.ELKOutputChild].
         """
         style_condition = self._diagram.render_styles.get(child["type"])
         styleoverrides = None
@@ -216,33 +215,7 @@
             if child["type"] != "junction":
                 obj = self._diagram._model.by_uuid(child["id"])
             else:
                 obj = None
 
             styleoverrides = style_condition(obj)
         return styleoverrides
-
-
-def get_styleclass(obj: common.GenericElement) -> str:
-    """Return the styleclass for a given `obj`."""
-    styleclass = obj.__class__.__name__
-    styleclass = (
-        aird.parser._semantic.STYLECLASS_LOOKUP.get(
-            styleclass, (styleclass, None)
-        )[0]
-        or styleclass
-    )
-    if styleclass.endswith("Component"):
-        styleclass = "".join(
-            (
-                styleclass[: -len("Component")],
-                "Human" * obj.is_human,
-                obj.nature.name.capitalize() if hasattr(obj, "nature") else "",
-                ("Component", "Actor")[obj.is_actor],
-            )
-        )
-    elif styleclass == "CP":
-        try:
-            styleclass += f'_{obj._element.attrib["orientation"]}'
-        except KeyError:
-            styleclass = "CP_UNSET"
-    return styleclass
```

### Comparing `capellambse-context-diagrams-0.2.8/capellambse_context_diagrams/styling.py` & `capellambse-context-diagrams-0.2.9/capellambse_context_diagrams/styling.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,47 +1,48 @@
 # SPDX-FileCopyrightText: 2022 Copyright DB Netz AG and the capellambse-context-diagrams contributors
 # SPDX-License-Identifier: Apache-2.0
 """Functions for style overrides of diagram elements."""
 from __future__ import annotations
 
 import typing as t
 
-from capellambse import aird
+from capellambse import diagram
+from capellambse.diagram import capstyle
 from capellambse.model import common
 
-CSSStyles = t.Union[aird.diagram._StyleOverrides, None]
+CSSStyles = t.Union[diagram.StyleOverrides, None]
 """
 A dictionary with CSS styles. The keys are the attribute names and the
 values can be of the types `str`, `aird.RGB` and even
 `t.Sequence[aird.RGB]` for coloring a
 [`common.GenericElement`][capellambse.model.common.element.GenericElement]
 with a gradient.
 
 See also
 --------
 [parent_is_actor_fills_blue][capellambse_context_diagrams.styling.parent_is_actor_fills_blue]
 """
 Styler = t.Callable[
-    [common.GenericElement], t.Union[aird.diagram._StyleOverrides, None]
+    [common.GenericElement], t.Union[diagram.StyleOverrides, None]
 ]
 """Function that produces `CSSStyles` for given obj."""
 
 
 def parent_is_actor_fills_blue(obj: common.GenericElement) -> CSSStyles:
     """
     Returns `CSSStyles` for given obj (i.e. `common.GenericElement`).
     """
     try:
         if obj.owner.is_actor:
             return {
                 "fill": [
-                    aird.capstyle.COLORS["_CAP_Actor_Blue_min"],
-                    aird.capstyle.COLORS["_CAP_Actor_Blue"],
+                    capstyle.COLORS["_CAP_Actor_Blue_min"],
+                    capstyle.COLORS["_CAP_Actor_Blue"],
                 ],
-                "stroke": aird.capstyle.COLORS["_CAP_Actor_Border_Blue"],
+                "stroke": capstyle.COLORS["_CAP_Actor_Border_Blue"],
             }
     except AttributeError:
         pass
 
     return None
```

### Comparing `capellambse-context-diagrams-0.2.8/capellambse_context_diagrams.egg-info/PKG-INFO` & `capellambse-context-diagrams-0.2.9/capellambse_context_diagrams.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: capellambse-context-diagrams
-Version: 0.2.8
+Version: 0.2.9
 Summary: Extension for python-capella-mbse that adds automatically generated context diagrams for arbitrary model elements.
 Author: DB Netz AG
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `capellambse-context-diagrams-0.2.8/capellambse_context_diagrams.egg-info/SOURCES.txt` & `capellambse-context-diagrams-0.2.9/capellambse_context_diagrams.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `capellambse-context-diagrams-0.2.8/docs/assets/images/Context of Left.svg` & `capellambse-context-diagrams-0.2.9/docs/assets/images/Context of Left.svg`

 * *Files identical despite different names*

### Comparing `capellambse-context-diagrams-0.2.8/docs/assets/images/Interface Context of Left to right.svg` & `capellambse-context-diagrams-0.2.9/docs/assets/images/Interface Context of Left to right.svg`

 * *Files identical despite different names*

### Comparing `capellambse-context-diagrams-0.2.8/docs/assets/images/favicon.ico` & `capellambse-context-diagrams-0.2.9/docs/assets/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `capellambse-context-diagrams-0.2.8/docs/assets/images/favicon.png` & `capellambse-context-diagrams-0.2.9/docs/assets/images/favicon.png`

 * *Files identical despite different names*

### Comparing `capellambse-context-diagrams-0.2.8/docs/credits.md` & `capellambse-context-diagrams-0.2.9/docs/credits.md`

 * *Files identical despite different names*

### Comparing `capellambse-context-diagrams-0.2.8/docs/extras/filters.md` & `capellambse-context-diagrams-0.2.9/docs/extras/filters.md`

 * *Files identical despite different names*

### Comparing `capellambse-context-diagrams-0.2.8/docs/extras/styling.md` & `capellambse-context-diagrams-0.2.9/docs/extras/styling.md`

 * *Files identical despite different names*

### Comparing `capellambse-context-diagrams-0.2.8/docs/gen_images.py` & `capellambse-context-diagrams-0.2.9/docs/gen_images.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from __future__ import annotations
 
 import logging
 import pathlib
 
 import mkdocs_gen_files
-from capellambse import MelodyModel, aird
+from capellambse import MelodyModel, diagram
 
 from capellambse_context_diagrams import context, filters, styling
 
 logging.basicConfig()
 
 dest = pathlib.Path("assets") / "images"
 model_path = pathlib.Path(__file__).parent.parent / "tests" / "data"
@@ -94,12 +94,12 @@
 generate_filter_image(lost, filters.FEX_EX_ITEMS, "fex and ex")
 generate_filter_image(lost, filters.FEX_OR_EX_ITEMS, "fex or ex")
 
 generate_styling_image(
     lost,
     dict(
         styling.BLUE_ACTOR_FNCS,
-        **{"junction": lambda _: {"fill": aird.RGB(220, 20, 60)}},  # type: ignore
+        **{"junction": lambda _: {"fill": diagram.RGB(220, 20, 60)}},  # type: ignore
     ),
     "red junction",
 )
 generate_styling_image(wizard, {}, "no_styles")
```

### Comparing `capellambse-context-diagrams-0.2.8/docs/gen_ref_pages.py` & `capellambse-context-diagrams-0.2.9/docs/gen_ref_pages.py`

 * *Files identical despite different names*

### Comparing `capellambse-context-diagrams-0.2.8/docs/index.md` & `capellambse-context-diagrams-0.2.9/docs/index.md`

 * *Files identical despite different names*

### Comparing `capellambse-context-diagrams-0.2.8/docs/quickstart.md` & `capellambse-context-diagrams-0.2.9/docs/quickstart.md`

 * *Files identical despite different names*

### Comparing `capellambse-context-diagrams-0.2.8/mkdocs.yml` & `capellambse-context-diagrams-0.2.9/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `capellambse-context-diagrams-0.2.8/overrides/.icons/custom/db.svg` & `capellambse-context-diagrams-0.2.9/overrides/.icons/custom/db.svg`

 * *Files identical despite different names*

### Comparing `capellambse-context-diagrams-0.2.8/pyproject.toml` & `capellambse-context-diagrams-0.2.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `capellambse-context-diagrams-0.2.8/tests/conftest.py` & `capellambse-context-diagrams-0.2.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `capellambse-context-diagrams-0.2.8/tests/data/ContextDiagram.afm` & `capellambse-context-diagrams-0.2.9/tests/data/ContextDiagram.afm`

 * *Files identical despite different names*

### Comparing `capellambse-context-diagrams-0.2.8/tests/data/ContextDiagram.aird` & `capellambse-context-diagrams-0.2.9/tests/data/ContextDiagram.aird`

 * *Files identical despite different names*

### Comparing `capellambse-context-diagrams-0.2.8/tests/data/ContextDiagram.capella` & `capellambse-context-diagrams-0.2.9/tests/data/ContextDiagram.capella`

 * *Files identical despite different names*

### Comparing `capellambse-context-diagrams-0.2.8/tests/test_capability_diagrams.py` & `capellambse-context-diagrams-0.2.9/tests/test_capability_diagrams.py`

 * *Files identical despite different names*

### Comparing `capellambse-context-diagrams-0.2.8/tests/test_context_diagrams.py` & `capellambse-context-diagrams-0.2.9/tests/test_context_diagrams.py`

 * *Files identical despite different names*

### Comparing `capellambse-context-diagrams-0.2.8/tests/test_filters.py` & `capellambse-context-diagrams-0.2.9/tests/test_filters.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from __future__ import annotations
 
 import re
 import typing as t
 
 import pytest
-from capellambse import MelodyModel, aird
+from capellambse import MelodyModel, diagram
 from capellambse.model import crosslayer
 
 from capellambse_context_diagrams import context, filters
 
 EX_PTRN = re.compile(r"\[(.*?)\]")
 CAP_EXPLOIT = "4513c8cd-b94b-4bde-bd00-4c18aaf600ff"
 
@@ -31,47 +31,47 @@
     exploitation = model.by_uuid(CAP_EXPLOIT)
 
     assert filters.uuid_filter(exploitation, label) == expected
 
 
 def start_filter_apply_test(
     model: MelodyModel, filter_name: str, **render_params: t.Any
-) -> tuple[list[crosslayer.fa.FunctionalExchange], aird.Diagram]:
+) -> tuple[list[crosslayer.fa.FunctionalExchange], diagram.Diagram]:
     """StartUp for every filter test case."""
     obj = model.by_uuid("a5642060-c9cc-4d49-af09-defaa3024bae")
     diag: context.ContextDiagram = obj.context_diagram
     diag.filters.add(filter_name)
     edges = [
         elt
         for elt in diag.nodes
         if isinstance(elt, crosslayer.fa.FunctionalExchange)
     ]
     return edges, diag.render(None, **render_params)
 
 
-def get_ExchangeItems(edge: aird.Edge) -> list[str]:
+def get_ExchangeItems(edge: diagram.Edge) -> list[str]:
     assert isinstance(edge.labels[0].label, str)
     match = EX_PTRN.match(edge.labels[0].label)
     assert match is not None
     return match.group(1).split(", ")
 
 
-def has_sorted_ExchangeItems(edge: aird.Edge) -> bool:
+def has_sorted_ExchangeItems(edge: diagram.Edge) -> bool:
     exitems = get_ExchangeItems(edge)
     return exitems == sorted(exitems)
 
 
 def test_EX_ITEMS_is_applied(model: MelodyModel) -> None:
     edges, aird_diag = start_filter_apply_test(model, filters.EX_ITEMS)
 
     for edge in edges:
         aedge = aird_diag[edge.uuid]
         expected = (ex.name for ex in edge.exchange_items)
 
-        assert isinstance(aedge, aird.Edge)
+        assert isinstance(aedge, diagram.Edge)
         if aedge.labels:
             assert get_ExchangeItems(aedge) == list(expected)
 
 
 @pytest.mark.parametrize("sort", [False, True])
 def test_context_diagrams_ExchangeItems_sorting(
     model: MelodyModel, sort: bool
@@ -79,15 +79,15 @@
     edges, aird_diag = start_filter_apply_test(
         model, filters.EX_ITEMS, sorted_exchangedItems=sort
     )
 
     all_sorted = True
     for edge in edges:
         aedge = aird_diag[edge.uuid]
-        assert isinstance(aedge, aird.Edge)
+        assert isinstance(aedge, diagram.Edge)
         if aedge.labels and not has_sorted_ExchangeItems(aedge):
             all_sorted = False
             break
 
     assert all_sorted == sort
 
 
@@ -99,29 +99,29 @@
     for edge in edges:
         aedge = aird_diag[edge.uuid]
         expected_label = edge.name
         eitems = ", ".join((exi.name for exi in edge.exchange_items))
         if eitems:
             expected_label += f" [{eitems}]"
 
-        assert isinstance(aedge, aird.Edge)
+        assert isinstance(aedge, diagram.Edge)
         assert len(aedge.labels) == 1
         assert isinstance(aedge.labels[0].label, str)
         assert aedge.labels[0].label == expected_label
 
 
 def test_context_diagrams_FEX_OR_EX_ITEMS_is_applied(
     model: MelodyModel,
 ) -> None:
     edges, aird_diag = start_filter_apply_test(model, filters.FEX_OR_EX_ITEMS)
 
     for edge in edges:
         aedge = aird_diag[edge.uuid]
 
-        assert isinstance(aedge, aird.Edge)
+        assert isinstance(aedge, diagram.Edge)
 
         label = aedge.labels[0].label
         if edge.exchange_items:
             eitem_label_frag = ", ".join(
                 (exi.name for exi in edge.exchange_items)
             )
 
@@ -136,22 +136,22 @@
     obj = model.by_uuid("9390b7d5-598a-42db-bef8-23677e45ba06")
     diag: context.ContextDiagram = obj.context_diagram
 
     diag.filters.add(filters.NO_UUID)
     aird_diag = diag.render(None)
     aedge = aird_diag[CAP_EXPLOIT]
 
-    assert isinstance(aedge, aird.Edge)
+    assert isinstance(aedge, diagram.Edge)
     assert aedge.labels[0].label == "[CapabilityExploitation] to Capability"
 
 
 def test_context_diagrams_no_edgelabels_render_param_is_applied(
     model: MelodyModel,
 ) -> None:
     obj = model.by_uuid("a5642060-c9cc-4d49-af09-defaa3024bae")
     diag: context.ContextDiagram = obj.context_diagram
 
     adiag = diag.render(None, no_edgelabels=True)
 
     for aedge in adiag:
-        if isinstance(aedge, aird.Edge):
+        if isinstance(aedge, diagram.Edge):
             assert not aedge.labels
```

### Comparing `capellambse-context-diagrams-0.2.8/tests/test_interface_diagrams.py` & `capellambse-context-diagrams-0.2.9/tests/test_interface_diagrams.py`

 * *Files identical despite different names*

