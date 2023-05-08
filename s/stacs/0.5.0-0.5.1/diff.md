# Comparing `tmp/stacs-0.5.0.tar.gz` & `tmp/stacs-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stacs-0.5.0.tar", last modified: Sat Apr 29 15:12:35 2023, max compression
+gzip compressed data, was "stacs-0.5.1.tar", last modified: Mon May  8 16:32:23 2023, max compression
```

## Comparing `stacs-0.5.0.tar` & `stacs-0.5.1.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:12:35.401892 stacs-0.5.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:12:35.393892 stacs-0.5.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-29 15:12:20.000000 stacs-0.5.0/.github/CODEOWNERS
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:12:35.393892 stacs-0.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-04-29 15:12:20.000000 stacs-0.5.0/.github/workflows/check.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-04-29 15:12:20.000000 stacs-0.5.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-04-29 15:12:20.000000 stacs-0.5.0/.github/workflows/publish_to_testing.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-04-29 15:12:20.000000 stacs-0.5.0/.github/workflows/update.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-04-29 15:12:20.000000 stacs-0.5.0/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:12:35.393892 stacs-0.5.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-29 15:12:20.000000 stacs-0.5.0/.vscode/c_cpp_properties.json
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-29 15:12:20.000000 stacs-0.5.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-04-29 15:12:20.000000 stacs-0.5.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-04-29 15:12:20.000000 stacs-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8163 2023-04-29 15:12:35.401892 stacs-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7827 2023-04-29 15:12:20.000000 stacs-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:12:35.389892 stacs-0.5.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:12:35.393892 stacs-0.5.0/docs/images/
--rwxr-xr-x   0 runner    (1001) docker     (123)    31469 2023-04-29 15:12:20.000000 stacs-0.5.0/docs/images/Human-Output-Example.png
--rw-r--r--   0 runner    (1001) docker     (123)   605164 2023-04-29 15:12:20.000000 stacs-0.5.0/docs/images/SARIF-Viewer-Example.png
--rw-r--r--   0 runner    (1001) docker     (123)    15785 2023-04-29 15:12:20.000000 stacs-0.5.0/docs/images/STACS-Logo-RGB.png
--rw-r--r--   0 runner    (1001) docker     (123)    26956 2023-04-29 15:12:20.000000 stacs-0.5.0/docs/images/STACS-Logo-RGB.small.png
--rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-04-29 15:12:20.000000 stacs-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 15:12:35.401892 stacs-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-04-29 15:12:20.000000 stacs-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:12:35.393892 stacs-0.5.0/stacs/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-29 15:12:20.000000 stacs-0.5.0/stacs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:12:35.389892 stacs-0.5.0/stacs/native/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:12:35.389892 stacs-0.5.0/stacs/native/archive/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:12:35.393892 stacs-0.5.0/stacs/native/archive/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-04-29 15:12:20.000000 stacs-0.5.0/stacs/native/archive/src/archive.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-29 15:12:20.000000 stacs-0.5.0/stacs/native/archive/src/archiveentry.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-29 15:12:20.000000 stacs-0.5.0/stacs/native/archive/src/archiveentry.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-04-29 15:12:20.000000 stacs-0.5.0/stacs/native/archive/src/archivereader.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-04-29 15:12:20.000000 stacs-0.5.0/stacs/native/archive/src/archivereader.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:12:35.393892 stacs-0.5.0/stacs/scan/
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-29 15:12:20.000000 stacs-0.5.0/stacs/scan/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-29 15:12:20.000000 stacs-0.5.0/stacs/scan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-29 15:12:20.000000 stacs-0.5.0/stacs/scan/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:12:35.397892 stacs-0.5.0/stacs/scan/entrypoint/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-29 15:12:20.000000 stacs-0.5.0/stacs/scan/entrypoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5776 2023-04-29 15:12:20.000000 stacs-0.5.0/stacs/scan/entrypoint/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-29 15:12:20.000000 stacs-0.5.0/stacs/scan/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:12:35.397892 stacs-0.5.0/stacs/scan/filter/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-29 15:12:20.000000 stacs-0.5.0/stacs/scan/filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-04-29 15:12:20.000000 stacs-0.5.0/stacs/scan/filter/ignore_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-04-29 15:12:20.000000 stacs-0.5.0/stacs/scan/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:12:35.397892 stacs-0.5.0/stacs/scan/loader/
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-29 15:12:20.000000 stacs-0.5.0/stacs/scan/loader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17021 2023-04-29 15:12:20.000000 stacs-0.5.0/stacs/scan/loader/archive.py
--rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-04-29 15:12:20.000000 stacs-0.5.0/stacs/scan/loader/filepath.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:12:35.397892 stacs-0.5.0/stacs/scan/loader/format/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-29 15:12:20.000000 stacs-0.5.0/stacs/scan/loader/format/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-04-29 15:12:20.000000 stacs-0.5.0/stacs/scan/loader/format/dmg.py
--rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-04-29 15:12:20.000000 stacs-0.5.0/stacs/scan/loader/format/xar.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-29 15:12:20.000000 stacs-0.5.0/stacs/scan/loader/manifest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:12:35.397892 stacs-0.5.0/stacs/scan/model/
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-29 15:12:20.000000 stacs-0.5.0/stacs/scan/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-04-29 15:12:20.000000 stacs-0.5.0/stacs/scan/model/finding.py
--rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-04-29 15:12:20.000000 stacs-0.5.0/stacs/scan/model/ignore_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-04-29 15:12:20.000000 stacs-0.5.0/stacs/scan/model/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-04-29 15:12:20.000000 stacs-0.5.0/stacs/scan/model/pack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:12:35.397892 stacs-0.5.0/stacs/scan/output/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-29 15:12:20.000000 stacs-0.5.0/stacs/scan/output/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-29 15:12:20.000000 stacs-0.5.0/stacs/scan/output/markdown.py
--rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-04-29 15:12:20.000000 stacs-0.5.0/stacs/scan/output/pretty.py
--rw-r--r--   0 runner    (1001) docker     (123)     8154 2023-04-29 15:12:20.000000 stacs-0.5.0/stacs/scan/output/sarif.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:12:35.397892 stacs-0.5.0/stacs/scan/scanner/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-29 15:12:20.000000 stacs-0.5.0/stacs/scan/scanner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7861 2023-04-29 15:12:20.000000 stacs-0.5.0/stacs/scan/scanner/rules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:12:35.393892 stacs-0.5.0/stacs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8163 2023-04-29 15:12:35.000000 stacs-0.5.0/stacs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-04-29 15:12:35.000000 stacs-0.5.0/stacs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 15:12:35.000000 stacs-0.5.0/stacs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-29 15:12:35.000000 stacs-0.5.0/stacs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-29 15:12:35.000000 stacs-0.5.0/stacs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-29 15:12:35.000000 stacs-0.5.0/stacs.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:12:35.397892 stacs-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 15:12:20.000000 stacs-0.5.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:12:35.397892 stacs-0.5.0/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 15:12:20.000000 stacs-0.5.0/tests/fixtures/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:12:35.397892 stacs-0.5.0/tests/fixtures/findings/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-29 15:12:20.000000 stacs-0.5.0/tests/fixtures/findings/001.txt
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-29 15:12:20.000000 stacs-0.5.0/tests/fixtures/findings/002.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-29 15:12:20.000000 stacs-0.5.0/tests/fixtures/findings/003.txt
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-29 15:12:20.000000 stacs-0.5.0/tests/fixtures/findings/004.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:12:35.401892 stacs-0.5.0/tests/fixtures/ignore_list/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-29 15:12:20.000000 stacs-0.5.0/tests/fixtures/ignore_list/001-simple.valid.json
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-29 15:12:20.000000 stacs-0.5.0/tests/fixtures/ignore_list/002-framework.valid.json
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-29 15:12:20.000000 stacs-0.5.0/tests/fixtures/ignore_list/002-project.valid.json
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-29 15:12:20.000000 stacs-0.5.0/tests/fixtures/ignore_list/002-system.valid.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:12:35.401892 stacs-0.5.0/tests/fixtures/pack/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-29 15:12:20.000000 stacs-0.5.0/tests/fixtures/pack/001-simple.valid.json
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-29 15:12:20.000000 stacs-0.5.0/tests/fixtures/pack/002-cloud.valid.json
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-29 15:12:20.000000 stacs-0.5.0/tests/fixtures/pack/002-parent.valid.json
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-29 15:12:20.000000 stacs-0.5.0/tests/fixtures/pack/002-pki-dsa.valid.json
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-29 15:12:20.000000 stacs-0.5.0/tests/fixtures/pack/002-pki-rsa.valid.json
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-29 15:12:20.000000 stacs-0.5.0/tests/fixtures/pack/002-pki.valid.json
--rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-04-29 15:12:20.000000 stacs-0.5.0/tests/test_filter_ignore_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-29 15:12:20.000000 stacs-0.5.0/tests/test_loader_filepath.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-29 15:12:20.000000 stacs-0.5.0/tests/test_model_ignore_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-04-29 15:12:20.000000 stacs-0.5.0/tests/test_model_pack.py
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-04-29 15:12:20.000000 stacs-0.5.0/tests/test_output_sarif.py
--rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-04-29 15:12:20.000000 stacs-0.5.0/tests/test_scanner_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:12:35.401892 stacs-0.5.0/wrapper/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1219 2023-04-29 15:12:20.000000 stacs-0.5.0/wrapper/stacs-scan
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:32:23.326103 stacs-0.5.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:32:23.318103 stacs-0.5.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-08 16:32:07.000000 stacs-0.5.1/.github/CODEOWNERS
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:32:23.318103 stacs-0.5.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-05-08 16:32:07.000000 stacs-0.5.1/.github/workflows/check.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-05-08 16:32:07.000000 stacs-0.5.1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-05-08 16:32:07.000000 stacs-0.5.1/.github/workflows/publish_to_testing.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-05-08 16:32:07.000000 stacs-0.5.1/.github/workflows/update.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-05-08 16:32:07.000000 stacs-0.5.1/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:32:23.318103 stacs-0.5.1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-08 16:32:07.000000 stacs-0.5.1/.vscode/c_cpp_properties.json
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-08 16:32:07.000000 stacs-0.5.1/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-05-08 16:32:07.000000 stacs-0.5.1/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-05-08 16:32:07.000000 stacs-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8163 2023-05-08 16:32:23.326103 stacs-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7827 2023-05-08 16:32:07.000000 stacs-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:32:23.314103 stacs-0.5.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:32:23.318103 stacs-0.5.1/docs/images/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    31469 2023-05-08 16:32:07.000000 stacs-0.5.1/docs/images/Human-Output-Example.png
+-rw-r--r--   0 runner    (1001) docker     (123)   605164 2023-05-08 16:32:07.000000 stacs-0.5.1/docs/images/SARIF-Viewer-Example.png
+-rw-r--r--   0 runner    (1001) docker     (123)    15785 2023-05-08 16:32:07.000000 stacs-0.5.1/docs/images/STACS-Logo-RGB.png
+-rw-r--r--   0 runner    (1001) docker     (123)    26956 2023-05-08 16:32:07.000000 stacs-0.5.1/docs/images/STACS-Logo-RGB.small.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-05-08 16:32:07.000000 stacs-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 16:32:23.326103 stacs-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-05-08 16:32:07.000000 stacs-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:32:23.318103 stacs-0.5.1/stacs/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-08 16:32:07.000000 stacs-0.5.1/stacs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:32:23.314103 stacs-0.5.1/stacs/native/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:32:23.314103 stacs-0.5.1/stacs/native/archive/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:32:23.318103 stacs-0.5.1/stacs/native/archive/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-05-08 16:32:07.000000 stacs-0.5.1/stacs/native/archive/src/archive.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-08 16:32:07.000000 stacs-0.5.1/stacs/native/archive/src/archiveentry.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-08 16:32:07.000000 stacs-0.5.1/stacs/native/archive/src/archiveentry.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-05-08 16:32:07.000000 stacs-0.5.1/stacs/native/archive/src/archivereader.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-08 16:32:07.000000 stacs-0.5.1/stacs/native/archive/src/archivereader.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:32:23.322103 stacs-0.5.1/stacs/scan/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-08 16:32:07.000000 stacs-0.5.1/stacs/scan/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-08 16:32:07.000000 stacs-0.5.1/stacs/scan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-08 16:32:07.000000 stacs-0.5.1/stacs/scan/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:32:23.322103 stacs-0.5.1/stacs/scan/entrypoint/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-08 16:32:07.000000 stacs-0.5.1/stacs/scan/entrypoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5776 2023-05-08 16:32:07.000000 stacs-0.5.1/stacs/scan/entrypoint/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-05-08 16:32:07.000000 stacs-0.5.1/stacs/scan/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:32:23.322103 stacs-0.5.1/stacs/scan/filter/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-08 16:32:07.000000 stacs-0.5.1/stacs/scan/filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-05-08 16:32:07.000000 stacs-0.5.1/stacs/scan/filter/ignore_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-05-08 16:32:07.000000 stacs-0.5.1/stacs/scan/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:32:23.322103 stacs-0.5.1/stacs/scan/loader/
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-08 16:32:07.000000 stacs-0.5.1/stacs/scan/loader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17021 2023-05-08 16:32:07.000000 stacs-0.5.1/stacs/scan/loader/archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-05-08 16:32:07.000000 stacs-0.5.1/stacs/scan/loader/filepath.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:32:23.322103 stacs-0.5.1/stacs/scan/loader/format/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-08 16:32:07.000000 stacs-0.5.1/stacs/scan/loader/format/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-05-08 16:32:07.000000 stacs-0.5.1/stacs/scan/loader/format/dmg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-05-08 16:32:07.000000 stacs-0.5.1/stacs/scan/loader/format/xar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-08 16:32:07.000000 stacs-0.5.1/stacs/scan/loader/manifest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:32:23.322103 stacs-0.5.1/stacs/scan/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-08 16:32:07.000000 stacs-0.5.1/stacs/scan/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-05-08 16:32:07.000000 stacs-0.5.1/stacs/scan/model/finding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-05-08 16:32:07.000000 stacs-0.5.1/stacs/scan/model/ignore_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-08 16:32:07.000000 stacs-0.5.1/stacs/scan/model/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-05-08 16:32:07.000000 stacs-0.5.1/stacs/scan/model/pack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:32:23.322103 stacs-0.5.1/stacs/scan/output/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-08 16:32:07.000000 stacs-0.5.1/stacs/scan/output/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-08 16:32:07.000000 stacs-0.5.1/stacs/scan/output/markdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-05-08 16:32:07.000000 stacs-0.5.1/stacs/scan/output/pretty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8154 2023-05-08 16:32:07.000000 stacs-0.5.1/stacs/scan/output/sarif.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:32:23.322103 stacs-0.5.1/stacs/scan/scanner/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-08 16:32:07.000000 stacs-0.5.1/stacs/scan/scanner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7861 2023-05-08 16:32:07.000000 stacs-0.5.1/stacs/scan/scanner/rules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:32:23.318103 stacs-0.5.1/stacs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8163 2023-05-08 16:32:23.000000 stacs-0.5.1/stacs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-05-08 16:32:23.000000 stacs-0.5.1/stacs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 16:32:23.000000 stacs-0.5.1/stacs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-08 16:32:23.000000 stacs-0.5.1/stacs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-08 16:32:23.000000 stacs-0.5.1/stacs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-08 16:32:23.000000 stacs-0.5.1/stacs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:32:23.326103 stacs-0.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 16:32:07.000000 stacs-0.5.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:32:23.326103 stacs-0.5.1/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 16:32:07.000000 stacs-0.5.1/tests/fixtures/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:32:23.326103 stacs-0.5.1/tests/fixtures/findings/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-08 16:32:07.000000 stacs-0.5.1/tests/fixtures/findings/001.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-08 16:32:07.000000 stacs-0.5.1/tests/fixtures/findings/002.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-08 16:32:07.000000 stacs-0.5.1/tests/fixtures/findings/003.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-08 16:32:07.000000 stacs-0.5.1/tests/fixtures/findings/004.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:32:23.326103 stacs-0.5.1/tests/fixtures/ignore_list/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-08 16:32:07.000000 stacs-0.5.1/tests/fixtures/ignore_list/001-simple.valid.json
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-08 16:32:07.000000 stacs-0.5.1/tests/fixtures/ignore_list/002-framework.valid.json
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-08 16:32:07.000000 stacs-0.5.1/tests/fixtures/ignore_list/002-project.valid.json
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-08 16:32:07.000000 stacs-0.5.1/tests/fixtures/ignore_list/002-system.valid.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:32:23.326103 stacs-0.5.1/tests/fixtures/pack/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-08 16:32:07.000000 stacs-0.5.1/tests/fixtures/pack/001-simple.valid.json
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-08 16:32:07.000000 stacs-0.5.1/tests/fixtures/pack/002-cloud.valid.json
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-08 16:32:07.000000 stacs-0.5.1/tests/fixtures/pack/002-parent.valid.json
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-08 16:32:07.000000 stacs-0.5.1/tests/fixtures/pack/002-pki-dsa.valid.json
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-08 16:32:07.000000 stacs-0.5.1/tests/fixtures/pack/002-pki-rsa.valid.json
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-08 16:32:07.000000 stacs-0.5.1/tests/fixtures/pack/002-pki.valid.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-05-08 16:32:07.000000 stacs-0.5.1/tests/test_filter_ignore_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-08 16:32:07.000000 stacs-0.5.1/tests/test_loader_filepath.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-08 16:32:07.000000 stacs-0.5.1/tests/test_model_ignore_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-08 16:32:07.000000 stacs-0.5.1/tests/test_model_pack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-05-08 16:32:07.000000 stacs-0.5.1/tests/test_output_sarif.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-05-08 16:32:07.000000 stacs-0.5.1/tests/test_scanner_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:32:23.326103 stacs-0.5.1/wrapper/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1219 2023-05-08 16:32:07.000000 stacs-0.5.1/wrapper/stacs-scan
```

### Comparing `stacs-0.5.0/.github/workflows/check.yml` & `stacs-0.5.1/.github/workflows/check.yml`

 * *Files identical despite different names*

### Comparing `stacs-0.5.0/.github/workflows/publish.yml` & `stacs-0.5.1/.github/workflows/publish.yml`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 jobs:
   build_wheels:
     name: Build wheels on ${{ matrix.os }}
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
-        os: [ubuntu-22.04, ubuntu-20.04, macos-10.15, macos-11, macos-12]
+        os: [ubuntu-22.04, ubuntu-20.04, macos-11, macos-12]
 
     steps:
       - uses: actions/checkout@v2
         with:
           ref: ${{ github.event.inputs.release }}
 
       - name: Configure Python
```

### Comparing `stacs-0.5.0/.github/workflows/publish_to_testing.yml` & `stacs-0.5.1/.github/workflows/publish_to_testing.yml`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 jobs:
   build_wheels:
     name: Build wheels on ${{ matrix.os }}
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
-        os: [ubuntu-22.04, ubuntu-20.04, macos-10.15, macos-11, macos-12]
+        os: [ubuntu-22.04, ubuntu-20.04, macos-11, macos-12]
 
     steps:
       - uses: actions/checkout@v2
         with:
           ref: ${{ github.event.inputs.release }}
 
       - name: Configure Python
```

### Comparing `stacs-0.5.0/.github/workflows/update.yml` & `stacs-0.5.1/.github/workflows/update.yml`

 * *Files identical despite different names*

### Comparing `stacs-0.5.0/.gitignore` & `stacs-0.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `stacs-0.5.0/Dockerfile` & `stacs-0.5.1/Dockerfile`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 LABEL org.opencontainers.image.title="STACS"
 LABEL org.opencontainers.image.description="Static Token And Credential Scanner"
 LABEL org.opencontainers.image.url="https://www.github.com/stacscan/stacs"
 LABEL org.opencontainers.image.version=$VERSION
 
 # Install STACS into the container.
 WORKDIR /opt/stacs
-COPY requirements.txt setup.py setup.cfg ./
 COPY wrapper/stacs-scan /usr/bin
 
 RUN apk add --no-cache git gcc musl-dev zstd && \
     pip install --no-cache-dir stacs==$STACS_BUILD
 
 # Clone the latest STACS rules into the rules directory to enable out of the box use.
 # This can be mounted over using a volume mount to allow more specific rules to be
```

### Comparing `stacs-0.5.0/LICENSE` & `stacs-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `stacs-0.5.0/PKG-INFO` & `stacs-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stacs
-Version: 0.5.0
+Version: 0.5.1
 Summary: Static Token And Credential Scanner.
 Author: Peter Adkins
 License: BSD-3-Clause
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Natural Language :: English
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `stacs-0.5.0/README.md` & `stacs-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `stacs-0.5.0/docs/images/Human-Output-Example.png` & `stacs-0.5.1/docs/images/Human-Output-Example.png`

 * *Files identical despite different names*

### Comparing `stacs-0.5.0/docs/images/SARIF-Viewer-Example.png` & `stacs-0.5.1/docs/images/SARIF-Viewer-Example.png`

 * *Files identical despite different names*

### Comparing `stacs-0.5.0/docs/images/STACS-Logo-RGB.png` & `stacs-0.5.1/docs/images/STACS-Logo-RGB.png`

 * *Files identical despite different names*

### Comparing `stacs-0.5.0/docs/images/STACS-Logo-RGB.small.png` & `stacs-0.5.1/docs/images/STACS-Logo-RGB.small.png`

 * *Files identical despite different names*

### Comparing `stacs-0.5.0/pyproject.toml` & `stacs-0.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 license = {text = "BSD-3-Clause"}
 classifiers = [
     "Programming Language :: Python :: 3.8",
     "Natural Language :: English",
 ]
 dependencies = [
     "click>=8.1.0,<9.0",
-    "yara-python>=4.2.0,<5.0",
+    "yara-python==4.2.3",
     "pydantic>=1.10.0,<2.0",
     "colorama>=0.4.0,<1.0",
     "zstandard>=0.18.0,<1.0",
 ]
 
 [project.optional-dependencies]
 tests = [
```

### Comparing `stacs-0.5.0/setup.py` & `stacs-0.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `stacs-0.5.0/stacs/native/archive/src/archive.cpp` & `stacs-0.5.1/stacs/native/archive/src/archive.cpp`

 * *Files identical despite different names*

### Comparing `stacs-0.5.0/stacs/native/archive/src/archiveentry.cpp` & `stacs-0.5.1/stacs/native/archive/src/archiveentry.cpp`

 * *Files identical despite different names*

### Comparing `stacs-0.5.0/stacs/native/archive/src/archivereader.cpp` & `stacs-0.5.1/stacs/native/archive/src/archivereader.cpp`

 * *Files identical despite different names*

### Comparing `stacs-0.5.0/stacs/native/archive/src/archivereader.hpp` & `stacs-0.5.1/stacs/native/archive/src/archivereader.hpp`

 * *Files identical despite different names*

### Comparing `stacs-0.5.0/stacs/scan/constants.py` & `stacs-0.5.1/stacs/scan/constants.py`

 * *Files identical despite different names*

### Comparing `stacs-0.5.0/stacs/scan/entrypoint/cli.py` & `stacs-0.5.1/stacs/scan/entrypoint/cli.py`

 * *Files identical despite different names*

### Comparing `stacs-0.5.0/stacs/scan/exceptions.py` & `stacs-0.5.1/stacs/scan/exceptions.py`

 * *Files identical despite different names*

### Comparing `stacs-0.5.0/stacs/scan/filter/ignore_list.py` & `stacs-0.5.1/stacs/scan/filter/ignore_list.py`

 * *Files identical despite different names*

### Comparing `stacs-0.5.0/stacs/scan/helper.py` & `stacs-0.5.1/stacs/scan/helper.py`

 * *Files identical despite different names*

### Comparing `stacs-0.5.0/stacs/scan/loader/archive.py` & `stacs-0.5.1/stacs/scan/loader/archive.py`

 * *Files identical despite different names*

### Comparing `stacs-0.5.0/stacs/scan/loader/filepath.py` & `stacs-0.5.1/stacs/scan/loader/filepath.py`

 * *Files identical despite different names*

### Comparing `stacs-0.5.0/stacs/scan/loader/format/dmg.py` & `stacs-0.5.1/stacs/scan/loader/format/dmg.py`

 * *Files identical despite different names*

### Comparing `stacs-0.5.0/stacs/scan/loader/format/xar.py` & `stacs-0.5.1/stacs/scan/loader/format/xar.py`

 * *Files identical despite different names*

### Comparing `stacs-0.5.0/stacs/scan/model/finding.py` & `stacs-0.5.1/stacs/scan/model/finding.py`

 * *Files identical despite different names*

### Comparing `stacs-0.5.0/stacs/scan/model/ignore_list.py` & `stacs-0.5.1/stacs/scan/model/ignore_list.py`

 * *Files identical despite different names*

### Comparing `stacs-0.5.0/stacs/scan/model/manifest.py` & `stacs-0.5.1/stacs/scan/model/manifest.py`

 * *Files identical despite different names*

### Comparing `stacs-0.5.0/stacs/scan/model/pack.py` & `stacs-0.5.1/stacs/scan/model/pack.py`

 * *Files identical despite different names*

### Comparing `stacs-0.5.0/stacs/scan/output/pretty.py` & `stacs-0.5.1/stacs/scan/output/pretty.py`

 * *Files identical despite different names*

### Comparing `stacs-0.5.0/stacs/scan/output/sarif.py` & `stacs-0.5.1/stacs/scan/output/sarif.py`

 * *Files identical despite different names*

### Comparing `stacs-0.5.0/stacs/scan/scanner/rules.py` & `stacs-0.5.1/stacs/scan/scanner/rules.py`

 * *Files identical despite different names*

### Comparing `stacs-0.5.0/stacs.egg-info/PKG-INFO` & `stacs-0.5.1/stacs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stacs
-Version: 0.5.0
+Version: 0.5.1
 Summary: Static Token And Credential Scanner.
 Author: Peter Adkins
 License: BSD-3-Clause
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Natural Language :: English
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `stacs-0.5.0/stacs.egg-info/SOURCES.txt` & `stacs-0.5.1/stacs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stacs-0.5.0/tests/fixtures/ignore_list/002-system.valid.json` & `stacs-0.5.1/tests/fixtures/ignore_list/002-system.valid.json`

 * *Files identical despite different names*

### Comparing `stacs-0.5.0/tests/test_filter_ignore_list.py` & `stacs-0.5.1/tests/test_filter_ignore_list.py`

 * *Files identical despite different names*

### Comparing `stacs-0.5.0/tests/test_model_ignore_list.py` & `stacs-0.5.1/tests/test_model_ignore_list.py`

 * *Files identical despite different names*

### Comparing `stacs-0.5.0/tests/test_model_pack.py` & `stacs-0.5.1/tests/test_model_pack.py`

 * *Files identical despite different names*

### Comparing `stacs-0.5.0/tests/test_output_sarif.py` & `stacs-0.5.1/tests/test_output_sarif.py`

 * *Files identical despite different names*

### Comparing `stacs-0.5.0/tests/test_scanner_rule.py` & `stacs-0.5.1/tests/test_scanner_rule.py`

 * *Files identical despite different names*

### Comparing `stacs-0.5.0/wrapper/stacs-scan` & `stacs-0.5.1/wrapper/stacs-scan`

 * *Files identical despite different names*

