# Comparing `tmp/heudiconv-0.8.0.tar.gz` & `tmp/heudiconv-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/heudiconv-0.8.0.tar", last modified: Thu Apr 16 02:56:36 2020, max compression
+gzip compressed data, was "heudiconv-0.9.0.tar", last modified: Wed Dec 23 15:35:33 2020, max compression
```

## Comparing `heudiconv-0.8.0.tar` & `heudiconv-0.9.0.tar`

### file list

```diff
@@ -1,110 +1,113 @@
-drwx--S---   0 yoh      (47521) yoh      (47522)        0 2020-04-16 02:56:36.000000 heudiconv-0.8.0/
--rw-------   0 yoh      (47521) yoh      (47522)       47 2019-01-05 04:43:21.000000 heudiconv-0.8.0/.coveragerc
--rw-------   0 yoh      (47521) yoh      (47522)       17 2019-01-12 15:48:20.000000 heudiconv-0.8.0/.dockerignore
-drwx--S---   0 yoh      (47521) yoh      (47522)        0 2020-04-16 02:56:36.000000 heudiconv-0.8.0/.github/
--rw-------   0 yoh      (47521) yoh      (47522)      597 2019-12-16 20:13:34.000000 heudiconv-0.8.0/.github/ISSUE_TEMPLATE.md
--rwx------   0 yoh      (47521) yoh      (47522)       58 2019-12-16 20:13:34.000000 heudiconv-0.8.0/.gitignore
--rw-------   0 yoh      (47521) yoh      (47522)      377 2019-01-05 04:43:21.000000 heudiconv-0.8.0/.mailmap
--rw-------   0 yoh      (47521) yoh      (47522)     1200 2020-04-16 02:56:20.000000 heudiconv-0.8.0/.travis.yml
--rw-------   0 yoh      (47521) yoh      (47522)    13846 2020-04-16 02:56:20.000000 heudiconv-0.8.0/CHANGELOG.md
--rw-------   0 yoh      (47521) yoh      (47522)     4963 2019-12-16 20:13:34.000000 heudiconv-0.8.0/Dockerfile
--rw-------   0 yoh      (47521) yoh      (47522)      597 2019-01-05 04:43:21.000000 heudiconv-0.8.0/LICENSE
--rw-------   0 yoh      (47521) yoh      (47522)      119 2020-04-16 02:56:20.000000 heudiconv-0.8.0/Makefile
--rw-------   0 yoh      (47521) yoh      (47522)       47 2019-01-05 04:43:21.000000 heudiconv-0.8.0/NOTES
--rw-------   0 yoh      (47521) yoh      (47522)      876 2020-04-16 02:56:36.000000 heudiconv-0.8.0/PKG-INFO
--rw-------   0 yoh      (47521) yoh      (47522)     1529 2020-04-16 02:56:20.000000 heudiconv-0.8.0/README.rst
-drwx--S---   0 yoh      (47521) yoh      (47522)        0 2020-04-16 02:56:36.000000 heudiconv-0.8.0/custom/
-drwx--S---   0 yoh      (47521) yoh      (47522)        0 2020-04-16 02:56:36.000000 heudiconv-0.8.0/custom/dbic/
--rw-------   0 yoh      (47521) yoh      (47522)      227 2019-01-05 04:43:21.000000 heudiconv-0.8.0/custom/dbic/README
--rw-------   0 yoh      (47521) yoh      (47522)     2655 2019-01-05 04:43:21.000000 heudiconv-0.8.0/custom/dbic/singularity-env.def
--rw-------   0 yoh      (47521) yoh      (47522)      118 2019-12-16 20:13:34.000000 heudiconv-0.8.0/dev-requirements.txt
-drwx--S---   0 yoh      (47521) yoh      (47522)        0 2020-04-16 02:56:36.000000 heudiconv-0.8.0/docs/
--rw-------   0 yoh      (47521) yoh      (47522)      580 2019-12-16 20:13:34.000000 heudiconv-0.8.0/docs/Makefile
-drwx--S---   0 yoh      (47521) yoh      (47522)        0 2020-04-16 02:56:36.000000 heudiconv-0.8.0/docs/api/
--rw-------   0 yoh      (47521) yoh      (47522)       47 2019-12-16 20:13:34.000000 heudiconv-0.8.0/docs/api/bids.rst
--rw-------   0 yoh      (47521) yoh      (47522)       68 2019-12-16 20:13:34.000000 heudiconv-0.8.0/docs/api/convert.rst
--rw-------   0 yoh      (47521) yoh      (47522)       55 2019-12-16 20:13:34.000000 heudiconv-0.8.0/docs/api/dicoms.rst
--rw-------   0 yoh      (47521) yoh      (47522)       58 2019-12-16 20:13:34.000000 heudiconv-0.8.0/docs/api/parser.rst
--rw-------   0 yoh      (47521) yoh      (47522)       75 2019-12-16 20:13:34.000000 heudiconv-0.8.0/docs/api/queue.rst
--rw-------   0 yoh      (47521) yoh      (47522)       57 2019-12-16 20:13:34.000000 heudiconv-0.8.0/docs/api/utils.rst
--rw-------   0 yoh      (47521) yoh      (47522)      154 2019-12-16 20:13:34.000000 heudiconv-0.8.0/docs/api.rst
--rw-------   0 yoh      (47521) yoh      (47522)       56 2019-12-16 20:13:34.000000 heudiconv-0.8.0/docs/changes.rst
--rw-------   0 yoh      (47521) yoh      (47522)     5350 2020-04-16 02:56:20.000000 heudiconv-0.8.0/docs/conf.py
--rw-------   0 yoh      (47521) yoh      (47522)     3117 2020-04-16 02:56:20.000000 heudiconv-0.8.0/docs/heuristics.rst
--rw-------   0 yoh      (47521) yoh      (47522)      367 2019-12-16 20:13:34.000000 heudiconv-0.8.0/docs/index.rst
--rw-------   0 yoh      (47521) yoh      (47522)     1216 2020-04-16 02:56:20.000000 heudiconv-0.8.0/docs/installation.rst
--rw-------   0 yoh      (47521) yoh      (47522)       47 2019-12-16 20:13:34.000000 heudiconv-0.8.0/docs/requirements.txt
--rw-------   0 yoh      (47521) yoh      (47522)      880 2020-04-16 02:56:20.000000 heudiconv-0.8.0/docs/tutorials.rst
--rw-------   0 yoh      (47521) yoh      (47522)     3081 2020-04-16 02:56:20.000000 heudiconv-0.8.0/docs/usage.rst
-drwx--S---   0 yoh      (47521) yoh      (47522)        0 2020-04-16 02:56:36.000000 heudiconv-0.8.0/heudiconv/
--rw-------   0 yoh      (47521) yoh      (47522)      367 2019-01-05 04:43:21.000000 heudiconv-0.8.0/heudiconv/__init__.py
--rw-------   0 yoh      (47521) yoh      (47522)    18618 2020-04-16 02:56:20.000000 heudiconv-0.8.0/heudiconv/bids.py
-drwx--S---   0 yoh      (47521) yoh      (47522)        0 2020-04-16 02:56:36.000000 heudiconv-0.8.0/heudiconv/cli/
--rw-------   0 yoh      (47521) yoh      (47522)        0 2019-01-05 04:43:21.000000 heudiconv-0.8.0/heudiconv/cli/__init__.py
--rw-------   0 yoh      (47521) yoh      (47522)     5551 2019-01-05 04:43:21.000000 heudiconv-0.8.0/heudiconv/cli/monitor.py
--rw-------   0 yoh      (47521) yoh      (47522)    16946 2020-04-16 02:56:20.000000 heudiconv-0.8.0/heudiconv/cli/run.py
--rw-------   0 yoh      (47521) yoh      (47522)    26416 2020-04-16 02:56:20.000000 heudiconv-0.8.0/heudiconv/convert.py
--rw-------   0 yoh      (47521) yoh      (47522)    18703 2020-04-16 02:56:20.000000 heudiconv-0.8.0/heudiconv/dicoms.py
-drwx--S---   0 yoh      (47521) yoh      (47522)        0 2020-04-16 02:56:36.000000 heudiconv-0.8.0/heudiconv/external/
--rw-------   0 yoh      (47521) yoh      (47522)        0 2019-01-05 04:43:21.000000 heudiconv-0.8.0/heudiconv/external/__init__.py
--rw-------   0 yoh      (47521) yoh      (47522)      910 2019-12-16 20:13:34.000000 heudiconv-0.8.0/heudiconv/external/dcmstack.py
--rw-------   0 yoh      (47521) yoh      (47522)     6843 2020-04-16 02:56:20.000000 heudiconv-0.8.0/heudiconv/external/dlad.py
--rw-------   0 yoh      (47521) yoh      (47522)      255 2019-01-05 04:43:21.000000 heudiconv-0.8.0/heudiconv/external/pydicom.py
-drwx--S---   0 yoh      (47521) yoh      (47522)        0 2020-04-16 02:56:36.000000 heudiconv-0.8.0/heudiconv/external/tests/
--rw-------   0 yoh      (47521) yoh      (47522)        0 2019-01-05 04:43:21.000000 heudiconv-0.8.0/heudiconv/external/tests/__init__.py
--rw-------   0 yoh      (47521) yoh      (47522)      702 2020-04-16 02:56:20.000000 heudiconv-0.8.0/heudiconv/external/tests/test_dlad.py
-drwx--S---   0 yoh      (47521) yoh      (47522)        0 2020-04-16 02:56:36.000000 heudiconv-0.8.0/heudiconv/heuristics/
--rw-------   0 yoh      (47521) yoh      (47522)        0 2019-01-05 04:43:21.000000 heudiconv-0.8.0/heudiconv/heuristics/__init__.py
--rw-------   0 yoh      (47521) yoh      (47522)     4183 2019-01-05 04:43:21.000000 heudiconv-0.8.0/heudiconv/heuristics/banda-bids.py
--rw-------   0 yoh      (47521) yoh      (47522)      939 2019-12-16 20:13:34.000000 heudiconv-0.8.0/heudiconv/heuristics/bids_ME.py
--rw-------   0 yoh      (47521) yoh      (47522)     3146 2019-01-05 04:43:21.000000 heudiconv-0.8.0/heudiconv/heuristics/bids_with_ses.py
--rw-------   0 yoh      (47521) yoh      (47522)     4114 2019-01-05 04:43:21.000000 heudiconv-0.8.0/heudiconv/heuristics/cmrr_heuristic.py
--rw-------   0 yoh      (47521) yoh      (47522)     1235 2019-01-05 04:43:21.000000 heudiconv-0.8.0/heudiconv/heuristics/convertall.py
--rw-------   0 yoh      (47521) yoh      (47522)     3871 2019-01-05 04:43:21.000000 heudiconv-0.8.0/heudiconv/heuristics/example.py
--rw-------   0 yoh      (47521) yoh      (47522)     2501 2019-01-05 04:43:21.000000 heudiconv-0.8.0/heudiconv/heuristics/multires_7Tbold.py
--rw-------   0 yoh      (47521) yoh      (47522)    41592 2020-04-16 02:56:20.000000 heudiconv-0.8.0/heudiconv/heuristics/reproin.py
--rw-------   0 yoh      (47521) yoh      (47522)      682 2020-04-16 02:56:20.000000 heudiconv-0.8.0/heudiconv/heuristics/reproin_validator.cfg
--rw-------   0 yoh      (47521) yoh      (47522)     1644 2019-01-05 04:43:21.000000 heudiconv-0.8.0/heudiconv/heuristics/studyforrest_phase2.py
--rw-------   0 yoh      (47521) yoh      (47522)     7355 2020-04-16 02:56:20.000000 heudiconv-0.8.0/heudiconv/heuristics/test_reproin.py
--rw-------   0 yoh      (47521) yoh      (47522)     2498 2019-01-05 04:43:21.000000 heudiconv-0.8.0/heudiconv/heuristics/uc_bids.py
--rw-------   0 yoh      (47521) yoh      (47522)     1349 2020-04-16 02:56:20.000000 heudiconv-0.8.0/heudiconv/info.py
--rw-------   0 yoh      (47521) yoh      (47522)     9251 2020-04-16 02:56:20.000000 heudiconv-0.8.0/heudiconv/parser.py
--rw-------   0 yoh      (47521) yoh      (47522)     3180 2019-12-16 20:13:34.000000 heudiconv-0.8.0/heudiconv/queue.py
-drwx--S---   0 yoh      (47521) yoh      (47522)        0 2020-04-16 02:56:36.000000 heudiconv-0.8.0/heudiconv/tests/
--rw-------   0 yoh      (47521) yoh      (47522)        0 2019-01-05 04:43:21.000000 heudiconv-0.8.0/heudiconv/tests/__init__.py
--rwx------   0 yoh      (47521) yoh      (47522)      305 2019-01-05 04:43:21.000000 heudiconv-0.8.0/heudiconv/tests/anonymize_script.py
-drwx--S---   0 yoh      (47521) yoh      (47522)        0 2020-04-16 02:56:36.000000 heudiconv-0.8.0/heudiconv/tests/data/
-drwx--S---   0 yoh      (47521) yoh      (47522)        0 2020-04-16 02:56:36.000000 heudiconv-0.8.0/heudiconv/tests/data/01-anat-scout/
--rw-------   0 yoh      (47521) yoh      (47522)   174070 2019-01-05 04:43:21.000000 heudiconv-0.8.0/heudiconv/tests/data/01-anat-scout/0001.dcm
-drwx--S---   0 yoh      (47521) yoh      (47522)        0 2020-04-16 02:56:36.000000 heudiconv-0.8.0/heudiconv/tests/data/01-fmap_acq-3mm/
--rw-------   0 yoh      (47521) yoh      (47522)   122162 2019-01-05 04:43:21.000000 heudiconv-0.8.0/heudiconv/tests/data/01-fmap_acq-3mm/1.3.12.2.1107.5.2.43.66112.2016101409263663466202201.dcm
--rw-------   0 yoh      (47521) yoh      (47522)   383456 2019-01-05 04:43:21.000000 heudiconv-0.8.0/heudiconv/tests/data/axasc35.dcm
--rw-------   0 yoh      (47521) yoh      (47522)   162304 2020-04-16 02:56:20.000000 heudiconv-0.8.0/heudiconv/tests/data/phantom.dcm
--rw-------   0 yoh      (47521) yoh      (47522)     2234 2020-04-16 02:56:20.000000 heudiconv-0.8.0/heudiconv/tests/test_dicoms.py
--rw-------   0 yoh      (47521) yoh      (47522)     5271 2019-12-16 20:13:34.000000 heudiconv-0.8.0/heudiconv/tests/test_heuristics.py
--rw-------   0 yoh      (47521) yoh      (47522)    10304 2020-04-16 02:56:20.000000 heudiconv-0.8.0/heudiconv/tests/test_main.py
--rw-------   0 yoh      (47521) yoh      (47522)     4057 2019-01-05 04:43:21.000000 heudiconv-0.8.0/heudiconv/tests/test_monitor.py
--rw-------   0 yoh      (47521) yoh      (47522)     2531 2019-12-16 20:13:34.000000 heudiconv-0.8.0/heudiconv/tests/test_queue.py
--rw-------   0 yoh      (47521) yoh      (47522)     4082 2020-04-16 02:56:20.000000 heudiconv-0.8.0/heudiconv/tests/test_regression.py
--rw-------   0 yoh      (47521) yoh      (47522)      981 2019-01-05 04:43:21.000000 heudiconv-0.8.0/heudiconv/tests/test_tarballs.py
--rw-------   0 yoh      (47521) yoh      (47522)     2757 2019-12-16 20:13:34.000000 heudiconv-0.8.0/heudiconv/tests/test_utils.py
--rw-------   0 yoh      (47521) yoh      (47522)     3561 2020-04-16 02:56:20.000000 heudiconv-0.8.0/heudiconv/tests/utils.py
--rw-------   0 yoh      (47521) yoh      (47522)    15263 2020-04-16 02:56:20.000000 heudiconv-0.8.0/heudiconv/utils.py
-drwx--S---   0 yoh      (47521) yoh      (47522)        0 2020-04-16 02:56:36.000000 heudiconv-0.8.0/heudiconv.egg-info/
--rw-------   0 yoh      (47521) yoh      (47522)      876 2020-04-16 02:56:36.000000 heudiconv-0.8.0/heudiconv.egg-info/PKG-INFO
--rw-------   0 yoh      (47521) yoh      (47522)     2320 2020-04-16 02:56:36.000000 heudiconv-0.8.0/heudiconv.egg-info/SOURCES.txt
--rw-------   0 yoh      (47521) yoh      (47522)        1 2020-04-16 02:56:36.000000 heudiconv-0.8.0/heudiconv.egg-info/dependency_links.txt
--rw-------   0 yoh      (47521) yoh      (47522)      101 2020-04-16 02:56:36.000000 heudiconv-0.8.0/heudiconv.egg-info/entry_points.txt
--rw-------   0 yoh      (47521) yoh      (47522)      296 2020-04-16 02:56:36.000000 heudiconv-0.8.0/heudiconv.egg-info/requires.txt
--rw-------   0 yoh      (47521) yoh      (47522)       10 2020-04-16 02:56:36.000000 heudiconv-0.8.0/heudiconv.egg-info/top_level.txt
--rw-------   0 yoh      (47521) yoh      (47522)      186 2019-01-05 04:43:21.000000 heudiconv-0.8.0/pytest.ini
--rw-------   0 yoh      (47521) yoh      (47522)        7 2019-01-05 04:43:21.000000 heudiconv-0.8.0/requirements.txt
--rw-------   0 yoh      (47521) yoh      (47522)       38 2020-04-16 02:56:36.000000 heudiconv-0.8.0/setup.cfg
--rwx------   0 yoh      (47521) yoh      (47522)     2289 2019-12-16 20:13:34.000000 heudiconv-0.8.0/setup.py
--rw-------   0 yoh      (47521) yoh      (47522)      139 2019-01-05 04:43:21.000000 heudiconv-0.8.0/tox.ini
-drwx--S---   0 yoh      (47521) yoh      (47522)        0 2020-04-16 02:56:36.000000 heudiconv-0.8.0/utils/
--rw-------   0 yoh      (47521) yoh      (47522)      658 2019-01-05 04:43:21.000000 heudiconv-0.8.0/utils/gen-docker-image.sh
--rwx------   0 yoh      (47521) yoh      (47522)      446 2019-12-16 20:13:34.000000 heudiconv-0.8.0/utils/link_issues_CHANGELOG
--rwx------   0 yoh      (47521) yoh      (47522)      386 2020-04-16 02:56:20.000000 heudiconv-0.8.0/utils/prep_release
--rwx------   0 yoh      (47521) yoh      (47522)     1838 2019-12-16 20:13:34.000000 heudiconv-0.8.0/utils/test-compare-two-versions.sh
--rw-------   0 yoh      (47521) yoh      (47522)     1593 2019-01-05 04:43:21.000000 heudiconv-0.8.0/utils/update_changes.sh
+drwx--S---   0 yoh      (47521) yoh      (47522)        0 2020-12-23 15:35:33.488483 heudiconv-0.9.0/
+-rw-------   0 yoh      (47521) yoh      (47522)       47 2019-01-05 04:43:21.000000 heudiconv-0.9.0/.coveragerc
+-rw-------   0 yoh      (47521) yoh      (47522)       17 2019-01-12 15:48:20.000000 heudiconv-0.9.0/.dockerignore
+drwx--S---   0 yoh      (47521) yoh      (47522)        0 2020-12-23 15:35:33.476483 heudiconv-0.9.0/.github/
+-rw-------   0 yoh      (47521) yoh      (47522)      597 2019-12-16 20:13:34.000000 heudiconv-0.9.0/.github/ISSUE_TEMPLATE.md
+-rwx------   0 yoh      (47521) yoh      (47522)       58 2019-12-16 20:13:34.000000 heudiconv-0.9.0/.gitignore
+-rw-------   0 yoh      (47521) yoh      (47522)      377 2019-01-05 04:43:21.000000 heudiconv-0.9.0/.mailmap
+-rw-------   0 yoh      (47521) yoh      (47522)     1200 2020-07-29 16:27:07.000000 heudiconv-0.9.0/.travis.yml
+-rw-------   0 yoh      (47521) yoh      (47522)    15442 2020-12-23 15:35:32.000000 heudiconv-0.9.0/CHANGELOG.md
+-rw-------   0 yoh      (47521) yoh      (47522)     4963 2019-12-16 20:13:34.000000 heudiconv-0.9.0/Dockerfile
+-rw-------   0 yoh      (47521) yoh      (47522)      597 2019-01-05 04:43:21.000000 heudiconv-0.9.0/LICENSE
+-rw-------   0 yoh      (47521) yoh      (47522)      370 2020-12-23 15:33:22.000000 heudiconv-0.9.0/Makefile
+-rw-------   0 yoh      (47521) yoh      (47522)       47 2019-01-05 04:43:21.000000 heudiconv-0.9.0/NOTES
+-rw-------   0 yoh      (47521) yoh      (47522)      876 2020-12-23 15:35:33.484483 heudiconv-0.9.0/PKG-INFO
+-rw-------   0 yoh      (47521) yoh      (47522)     1897 2020-12-22 22:19:56.000000 heudiconv-0.9.0/README.rst
+drwx--S---   0 yoh      (47521) yoh      (47522)        0 2020-12-23 15:35:33.476483 heudiconv-0.9.0/custom/
+drwx--S---   0 yoh      (47521) yoh      (47522)        0 2020-12-23 15:35:33.476483 heudiconv-0.9.0/custom/dbic/
+-rw-------   0 yoh      (47521) yoh      (47522)      227 2019-01-05 04:43:21.000000 heudiconv-0.9.0/custom/dbic/README
+-rw-------   0 yoh      (47521) yoh      (47522)     2655 2019-01-05 04:43:21.000000 heudiconv-0.9.0/custom/dbic/singularity-env.def
+-rw-------   0 yoh      (47521) yoh      (47522)      118 2019-12-16 20:13:34.000000 heudiconv-0.9.0/dev-requirements.txt
+drwx--S---   0 yoh      (47521) yoh      (47522)        0 2020-12-23 15:35:33.476483 heudiconv-0.9.0/docs/
+-rw-------   0 yoh      (47521) yoh      (47522)      580 2019-12-16 20:13:34.000000 heudiconv-0.9.0/docs/Makefile
+drwx--S---   0 yoh      (47521) yoh      (47522)        0 2020-12-23 15:35:33.476483 heudiconv-0.9.0/docs/api/
+-rw-------   0 yoh      (47521) yoh      (47522)       47 2019-12-16 20:13:34.000000 heudiconv-0.9.0/docs/api/bids.rst
+-rw-------   0 yoh      (47521) yoh      (47522)       68 2019-12-16 20:13:34.000000 heudiconv-0.9.0/docs/api/convert.rst
+-rw-------   0 yoh      (47521) yoh      (47522)       55 2019-12-16 20:13:34.000000 heudiconv-0.9.0/docs/api/dicoms.rst
+-rw-------   0 yoh      (47521) yoh      (47522)       58 2019-12-16 20:13:34.000000 heudiconv-0.9.0/docs/api/parser.rst
+-rw-------   0 yoh      (47521) yoh      (47522)       75 2019-12-16 20:13:34.000000 heudiconv-0.9.0/docs/api/queue.rst
+-rw-------   0 yoh      (47521) yoh      (47522)       57 2019-12-16 20:13:34.000000 heudiconv-0.9.0/docs/api/utils.rst
+-rw-------   0 yoh      (47521) yoh      (47522)      154 2019-12-16 20:13:34.000000 heudiconv-0.9.0/docs/api.rst
+-rw-------   0 yoh      (47521) yoh      (47522)       56 2019-12-16 20:13:34.000000 heudiconv-0.9.0/docs/changes.rst
+-rw-------   0 yoh      (47521) yoh      (47522)     5350 2020-12-23 15:35:32.000000 heudiconv-0.9.0/docs/conf.py
+-rw-------   0 yoh      (47521) yoh      (47522)     3117 2020-07-29 16:27:07.000000 heudiconv-0.9.0/docs/heuristics.rst
+-rw-------   0 yoh      (47521) yoh      (47522)      367 2019-12-16 20:13:34.000000 heudiconv-0.9.0/docs/index.rst
+-rw-------   0 yoh      (47521) yoh      (47522)     1208 2020-12-23 15:35:32.000000 heudiconv-0.9.0/docs/installation.rst
+-rw-------   0 yoh      (47521) yoh      (47522)       47 2019-12-16 20:13:34.000000 heudiconv-0.9.0/docs/requirements.txt
+-rw-------   0 yoh      (47521) yoh      (47522)     1388 2020-07-29 16:27:07.000000 heudiconv-0.9.0/docs/tutorials.rst
+-rw-------   0 yoh      (47521) yoh      (47522)     3081 2020-12-23 15:35:32.000000 heudiconv-0.9.0/docs/usage.rst
+drwx--S---   0 yoh      (47521) yoh      (47522)        0 2020-12-23 15:35:33.480483 heudiconv-0.9.0/heudiconv/
+-rw-------   0 yoh      (47521) yoh      (47522)      367 2019-01-05 04:43:21.000000 heudiconv-0.9.0/heudiconv/__init__.py
+-rw-------   0 yoh      (47521) yoh      (47522)    18532 2020-12-23 15:13:14.000000 heudiconv-0.9.0/heudiconv/bids.py
+drwx--S---   0 yoh      (47521) yoh      (47522)        0 2020-12-23 15:35:33.480483 heudiconv-0.9.0/heudiconv/cli/
+-rw-------   0 yoh      (47521) yoh      (47522)        0 2019-01-05 04:43:21.000000 heudiconv-0.9.0/heudiconv/cli/__init__.py
+-rw-------   0 yoh      (47521) yoh      (47522)     5551 2019-01-05 04:43:21.000000 heudiconv-0.9.0/heudiconv/cli/monitor.py
+-rwx------   0 yoh      (47521) yoh      (47522)     6855 2020-12-23 15:13:14.000000 heudiconv-0.9.0/heudiconv/cli/run.py
+-rw-------   0 yoh      (47521) yoh      (47522)    30403 2020-12-23 15:13:15.000000 heudiconv-0.9.0/heudiconv/convert.py
+-rw-------   0 yoh      (47521) yoh      (47522)    18639 2020-07-29 16:27:07.000000 heudiconv-0.9.0/heudiconv/dicoms.py
+-rw-------   0 yoh      (47521) yoh      (47522)     2018 2020-12-22 22:19:56.000000 heudiconv-0.9.0/heudiconv/due.py
+drwx--S---   0 yoh      (47521) yoh      (47522)        0 2020-12-23 15:35:33.480483 heudiconv-0.9.0/heudiconv/external/
+-rw-------   0 yoh      (47521) yoh      (47522)        0 2019-01-05 04:43:21.000000 heudiconv-0.9.0/heudiconv/external/__init__.py
+-rw-------   0 yoh      (47521) yoh      (47522)      910 2019-12-16 20:13:34.000000 heudiconv-0.9.0/heudiconv/external/dcmstack.py
+-rw-------   0 yoh      (47521) yoh      (47522)     6827 2020-12-22 22:19:56.000000 heudiconv-0.9.0/heudiconv/external/dlad.py
+-rw-------   0 yoh      (47521) yoh      (47522)      255 2019-01-05 04:43:21.000000 heudiconv-0.9.0/heudiconv/external/pydicom.py
+drwx--S---   0 yoh      (47521) yoh      (47522)        0 2020-12-23 15:35:33.480483 heudiconv-0.9.0/heudiconv/external/tests/
+-rw-------   0 yoh      (47521) yoh      (47522)        0 2019-01-05 04:43:21.000000 heudiconv-0.9.0/heudiconv/external/tests/__init__.py
+-rw-------   0 yoh      (47521) yoh      (47522)      703 2020-12-22 22:19:56.000000 heudiconv-0.9.0/heudiconv/external/tests/test_dlad.py
+drwx--S---   0 yoh      (47521) yoh      (47522)        0 2020-12-23 15:35:33.480483 heudiconv-0.9.0/heudiconv/heuristics/
+-rw-------   0 yoh      (47521) yoh      (47522)        0 2019-01-05 04:43:21.000000 heudiconv-0.9.0/heudiconv/heuristics/__init__.py
+-rw-------   0 yoh      (47521) yoh      (47522)     4183 2019-01-05 04:43:21.000000 heudiconv-0.9.0/heudiconv/heuristics/banda-bids.py
+-rw-------   0 yoh      (47521) yoh      (47522)      939 2019-12-16 20:13:34.000000 heudiconv-0.9.0/heudiconv/heuristics/bids_ME.py
+-rw-------   0 yoh      (47521) yoh      (47522)     3146 2019-01-05 04:43:21.000000 heudiconv-0.9.0/heudiconv/heuristics/bids_with_ses.py
+-rw-------   0 yoh      (47521) yoh      (47522)     4114 2019-01-05 04:43:21.000000 heudiconv-0.9.0/heudiconv/heuristics/cmrr_heuristic.py
+-rw-------   0 yoh      (47521) yoh      (47522)     1235 2019-01-05 04:43:21.000000 heudiconv-0.9.0/heudiconv/heuristics/convertall.py
+-rw-------   0 yoh      (47521) yoh      (47522)     3871 2019-01-05 04:43:21.000000 heudiconv-0.9.0/heudiconv/heuristics/example.py
+-rw-------   0 yoh      (47521) yoh      (47522)     2501 2019-01-05 04:43:21.000000 heudiconv-0.9.0/heudiconv/heuristics/multires_7Tbold.py
+-rw-------   0 yoh      (47521) yoh      (47522)    41796 2020-12-22 22:19:56.000000 heudiconv-0.9.0/heudiconv/heuristics/reproin.py
+-rw-------   0 yoh      (47521) yoh      (47522)      682 2020-07-29 16:27:07.000000 heudiconv-0.9.0/heudiconv/heuristics/reproin_validator.cfg
+-rw-------   0 yoh      (47521) yoh      (47522)     1644 2019-01-05 04:43:21.000000 heudiconv-0.9.0/heudiconv/heuristics/studyforrest_phase2.py
+-rw-------   0 yoh      (47521) yoh      (47522)     7355 2020-07-29 16:27:07.000000 heudiconv-0.9.0/heudiconv/heuristics/test_reproin.py
+-rw-------   0 yoh      (47521) yoh      (47522)     2498 2019-01-05 04:43:21.000000 heudiconv-0.9.0/heudiconv/heuristics/uc_bids.py
+-rw-------   0 yoh      (47521) yoh      (47522)     1345 2020-12-23 15:35:32.000000 heudiconv-0.9.0/heudiconv/info.py
+-rw-------   0 yoh      (47521) yoh      (47522)    15480 2020-12-23 15:13:14.000000 heudiconv-0.9.0/heudiconv/main.py
+-rw-------   0 yoh      (47521) yoh      (47522)     9368 2020-12-23 15:13:15.000000 heudiconv-0.9.0/heudiconv/parser.py
+-rw-------   0 yoh      (47521) yoh      (47522)     3180 2019-12-16 20:13:34.000000 heudiconv-0.9.0/heudiconv/queue.py
+drwx--S---   0 yoh      (47521) yoh      (47522)        0 2020-12-23 15:35:33.484483 heudiconv-0.9.0/heudiconv/tests/
+-rw-------   0 yoh      (47521) yoh      (47522)        0 2019-01-05 04:43:21.000000 heudiconv-0.9.0/heudiconv/tests/__init__.py
+-rwx------   0 yoh      (47521) yoh      (47522)      305 2019-01-05 04:43:21.000000 heudiconv-0.9.0/heudiconv/tests/anonymize_script.py
+drwx--S---   0 yoh      (47521) yoh      (47522)        0 2020-12-23 15:35:33.484483 heudiconv-0.9.0/heudiconv/tests/data/
+drwx--S---   0 yoh      (47521) yoh      (47522)        0 2020-12-23 15:35:33.484483 heudiconv-0.9.0/heudiconv/tests/data/01-anat-scout/
+-rw-------   0 yoh      (47521) yoh      (47522)   174070 2019-01-05 04:43:21.000000 heudiconv-0.9.0/heudiconv/tests/data/01-anat-scout/0001.dcm
+drwx--S---   0 yoh      (47521) yoh      (47522)        0 2020-12-23 15:35:33.484483 heudiconv-0.9.0/heudiconv/tests/data/01-fmap_acq-3mm/
+-rw-------   0 yoh      (47521) yoh      (47522)   122162 2019-01-05 04:43:21.000000 heudiconv-0.9.0/heudiconv/tests/data/01-fmap_acq-3mm/1.3.12.2.1107.5.2.43.66112.2016101409263663466202201.dcm
+-rw-------   0 yoh      (47521) yoh      (47522)   383456 2019-01-05 04:43:21.000000 heudiconv-0.9.0/heudiconv/tests/data/axasc35.dcm
+-rw-------   0 yoh      (47521) yoh      (47522)   162304 2020-07-29 16:27:07.000000 heudiconv-0.9.0/heudiconv/tests/data/phantom.dcm
+-rw-------   0 yoh      (47521) yoh      (47522)     3285 2020-12-22 22:19:56.000000 heudiconv-0.9.0/heudiconv/tests/test_convert.py
+-rw-------   0 yoh      (47521) yoh      (47522)     2234 2020-07-29 16:27:07.000000 heudiconv-0.9.0/heudiconv/tests/test_dicoms.py
+-rw-------   0 yoh      (47521) yoh      (47522)     5279 2020-07-29 16:27:07.000000 heudiconv-0.9.0/heudiconv/tests/test_heuristics.py
+-rw-------   0 yoh      (47521) yoh      (47522)    10256 2020-12-23 15:13:14.000000 heudiconv-0.9.0/heudiconv/tests/test_main.py
+-rw-------   0 yoh      (47521) yoh      (47522)     4057 2019-01-05 04:43:21.000000 heudiconv-0.9.0/heudiconv/tests/test_monitor.py
+-rw-------   0 yoh      (47521) yoh      (47522)     2531 2019-12-16 20:13:34.000000 heudiconv-0.9.0/heudiconv/tests/test_queue.py
+-rw-------   0 yoh      (47521) yoh      (47522)     4082 2020-07-29 16:27:07.000000 heudiconv-0.9.0/heudiconv/tests/test_regression.py
+-rw-------   0 yoh      (47521) yoh      (47522)      981 2019-01-05 04:43:21.000000 heudiconv-0.9.0/heudiconv/tests/test_tarballs.py
+-rw-------   0 yoh      (47521) yoh      (47522)     3092 2020-12-23 15:13:14.000000 heudiconv-0.9.0/heudiconv/tests/test_utils.py
+-rw-------   0 yoh      (47521) yoh      (47522)     3561 2020-07-29 16:27:07.000000 heudiconv-0.9.0/heudiconv/tests/utils.py
+-rw-------   0 yoh      (47521) yoh      (47522)    16763 2020-12-23 15:13:15.000000 heudiconv-0.9.0/heudiconv/utils.py
+drwx--S---   0 yoh      (47521) yoh      (47522)        0 2020-12-23 15:35:33.480483 heudiconv-0.9.0/heudiconv.egg-info/
+-rw-------   0 yoh      (47521) yoh      (47522)      876 2020-12-23 15:35:33.000000 heudiconv-0.9.0/heudiconv.egg-info/PKG-INFO
+-rw-------   0 yoh      (47521) yoh      (47522)     2387 2020-12-23 15:35:33.000000 heudiconv-0.9.0/heudiconv.egg-info/SOURCES.txt
+-rw-------   0 yoh      (47521) yoh      (47522)        1 2020-12-23 15:35:33.000000 heudiconv-0.9.0/heudiconv.egg-info/dependency_links.txt
+-rw-------   0 yoh      (47521) yoh      (47522)      101 2020-12-23 15:35:33.000000 heudiconv-0.9.0/heudiconv.egg-info/entry_points.txt
+-rw-------   0 yoh      (47521) yoh      (47522)      223 2020-12-23 15:35:33.000000 heudiconv-0.9.0/heudiconv.egg-info/requires.txt
+-rw-------   0 yoh      (47521) yoh      (47522)       10 2020-12-23 15:35:33.000000 heudiconv-0.9.0/heudiconv.egg-info/top_level.txt
+-rw-------   0 yoh      (47521) yoh      (47522)      186 2019-01-05 04:43:21.000000 heudiconv-0.9.0/pytest.ini
+-rw-------   0 yoh      (47521) yoh      (47522)        7 2019-01-05 04:43:21.000000 heudiconv-0.9.0/requirements.txt
+-rw-------   0 yoh      (47521) yoh      (47522)       38 2020-12-23 15:35:33.488483 heudiconv-0.9.0/setup.cfg
+-rwx------   0 yoh      (47521) yoh      (47522)     2162 2020-07-29 16:27:07.000000 heudiconv-0.9.0/setup.py
+-rw-------   0 yoh      (47521) yoh      (47522)      139 2019-01-05 04:43:21.000000 heudiconv-0.9.0/tox.ini
+drwx--S---   0 yoh      (47521) yoh      (47522)        0 2020-12-23 15:35:33.484483 heudiconv-0.9.0/utils/
+-rw-------   0 yoh      (47521) yoh      (47522)      658 2019-01-05 04:43:21.000000 heudiconv-0.9.0/utils/gen-docker-image.sh
+-rwx------   0 yoh      (47521) yoh      (47522)      446 2019-12-16 20:13:34.000000 heudiconv-0.9.0/utils/link_issues_CHANGELOG
+-rwx------   0 yoh      (47521) yoh      (47522)      416 2020-12-23 15:35:20.000000 heudiconv-0.9.0/utils/prep_release
+-rwx------   0 yoh      (47521) yoh      (47522)     2020 2020-12-22 22:19:56.000000 heudiconv-0.9.0/utils/test-compare-two-versions.sh
+-rw-------   0 yoh      (47521) yoh      (47522)     1593 2019-01-05 04:43:21.000000 heudiconv-0.9.0/utils/update_changes.sh
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `heudiconv-0.8.0/.github/ISSUE_TEMPLATE.md` & `heudiconv-0.9.0/.github/ISSUE_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `heudiconv-0.8.0/.travis.yml` & `heudiconv-0.9.0/.travis.yml`

 * *Files identical despite different names*

### Comparing `heudiconv-0.8.0/CHANGELOG.md` & `heudiconv-0.9.0/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,51 @@
 # Changelog
 All notable changes to this project will be documented (for humans) in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
 and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
 
+## [0.9.0] - 2020-12-23
+
+Various improvements and compatibility/support (dcm2niix, datalad,
+duecredit) changes.  Major change is placement of output files to the
+target output directory during conversion.
+
+### Added
+
+- #454 zenodo referencing in README.rst and support for ducredit for
+  heudiconv and reproin heuristic
+- #445 more tutorial references in README.md
+
+### Changed
+
+- [#485][] placed files during conversion right away into the target
+  directory (with a `_heudiconv???` suffix, renamed into ultimate target
+  name later on), which avoids hitting file size limits of /tmp ([#481][]) and
+  helped to avoid a regression in dcm2nixx 1.0.20201102
+- #477 replaced `rec-<magnitude|phase>` with `part-<mag|phase>` now
+  that BIDS supports the part entity
+- #473 made default for CogAtlasID to be a TODO URL
+- #459 made AcquisitionTime used for acq_time scans file field
+- #451 retained sub-second resolution in scans files
+- #442 refactored code so there is now heudiconv.main.workflow for
+  more convenient use as a Python module
+
+### Fixed
+
+- minimal version of nipype set to 1.2.3 to guarantee correct handling
+  of DWI files ([#480][])
+- `heudiconvDCM*` temporary directories are removed now ([#462][])
+- compatibility with DataLad 0.13 ([#464][])
+
+### Removed
+
+- #443 pathlib as a dependency (we are Python3 only now)
+
+
 ## [0.8.0] - 2020-04-15
 
 ### Enhancements
 
 - Centralized saving of .json files.  Indentation of some files could
   change now from previous versions where it could have used `3`
   spaces. Now indentation should be consistently `2` for .json files
@@ -307,14 +345,15 @@
 [#354]: https://github.com/nipy/heudiconv/issues/354
 [#357]: https://github.com/nipy/heudiconv/issues/357
 [#358]: https://github.com/nipy/heudiconv/issues/358
 [#347]: https://github.com/nipy/heudiconv/issues/347
 [#366]: https://github.com/nipy/heudiconv/issues/366
 [#368]: https://github.com/nipy/heudiconv/issues/368
 [#373]: https://github.com/nipy/heudiconv/issues/373
+[#485]: https://github.com/nipy/heudiconv/issues/485
 [#293]: https://github.com/nipy/heudiconv/issues/293
 [#304]: https://github.com/nipy/heudiconv/issues/304
 [#306]: https://github.com/nipy/heudiconv/issues/306
 [#310]: https://github.com/nipy/heudiconv/issues/310
 [#327]: https://github.com/nipy/heudiconv/issues/327
 [#328]: https://github.com/nipy/heudiconv/issues/328
 [#334]: https://github.com/nipy/heudiconv/issues/334
@@ -344,7 +383,11 @@
 [#420]: https://github.com/nipy/heudiconv/issues/420
 [#425]: https://github.com/nipy/heudiconv/issues/425
 [#430]: https://github.com/nipy/heudiconv/issues/430
 [#432]: https://github.com/nipy/heudiconv/issues/432
 [#434]: https://github.com/nipy/heudiconv/issues/434
 [#436]: https://github.com/nipy/heudiconv/issues/436
 [#437]: https://github.com/nipy/heudiconv/issues/437
+[#462]: https://github.com/nipy/heudiconv/issues/462
+[#464]: https://github.com/nipy/heudiconv/issues/464
+[#480]: https://github.com/nipy/heudiconv/issues/480
+[#481]: https://github.com/nipy/heudiconv/issues/481
```

### Comparing `heudiconv-0.8.0/Dockerfile` & `heudiconv-0.9.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `heudiconv-0.8.0/LICENSE` & `heudiconv-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `heudiconv-0.8.0/PKG-INFO` & `heudiconv-0.9.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heudiconv
-Version: 0.8.0
+Version: 0.9.0
 Summary: Heuristic DICOM Converter
 Home-page: UNKNOWN
 Author: HeuDiConv team and contributors
 License: Apache 2.0
 Description: Convert DICOM dirs based on heuristic info - HeuDiConv
         uses the dcmstack package and dcm2niix tool to convert DICOM directories or
         tarballs into collections of NIfTI files following pre-defined heuristic(s).
@@ -13,11 +13,11 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.5
-Provides-Extra: tests
-Provides-Extra: extras
-Provides-Extra: datalad
 Provides-Extra: all
+Provides-Extra: datalad
+Provides-Extra: extras
+Provides-Extra: tests
```

### Comparing `heudiconv-0.8.0/README.rst` & `heudiconv-0.9.0/README.rst`

 * *Files 21% similar despite different names*

```diff
@@ -16,20 +16,31 @@
   :target: https://codecov.io/gh/nipy/heudiconv
   :alt: CodeCoverage
 
 .. image:: https://readthedocs.org/projects/heudiconv/badge/?version=latest
   :target: http://heudiconv.readthedocs.io/en/latest/?badge=latest
   :alt: Readthedocs
 
+.. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.1012598.svg
+  :target: https://doi.org/10.5281/zenodo.1012598
+  :alt: Zenodo (latest)
+
 About
 -----
 
 ``heudiconv`` is a flexible DICOM converter for organizing brain imaging data
 into structured directory layouts.
 
 - it allows flexible directory layouts and naming schemes through customizable heuristics implementations
 - it only converts the necessary DICOMs, not everything in a directory
 - you can keep links to DICOM files in the participant layout
 - using dcm2niix under the hood, it's fast
 - it can track the provenance of the conversion from DICOM to NIfTI in W3C PROV format
 - it provides assistance in converting to `BIDS <http://bids.neuroimaging.io/>`_.
 - it integrates with `DataLad <https://www.datalad.org/>`_ to place converted and original data under git/git-annex version control, while automatically annotating files with sensitive information (e.g., non-defaced anatomicals, etc)
+
+How to cite
+-----------
+
+Please use `Zenodo record <https://doi.org/10.5281/zenodo.1012598>`_ for
+your specific version of HeuDiConv.  We also support gathering
+all relevant citations via `DueCredit <http://duecredit.org>`_.
```

### Comparing `heudiconv-0.8.0/custom/dbic/singularity-env.def` & `heudiconv-0.9.0/custom/dbic/singularity-env.def`

 * *Files identical despite different names*

### Comparing `heudiconv-0.8.0/docs/Makefile` & `heudiconv-0.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `heudiconv-0.8.0/docs/conf.py` & `heudiconv-0.9.0/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 project = 'heudiconv'
 copyright = '2019, Heudiconv team'
 author = 'Heudiconv team'
 
 # The short X.Y version
 version = ''
 # The full version, including alpha/beta/rc tags
-release = '0.8.0'
+release = '0.9.0'
 
 
 # -- General configuration ---------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 # needs_sphinx = '1.0'
```

### Comparing `heudiconv-0.8.0/docs/heuristics.rst` & `heudiconv-0.9.0/docs/heuristics.rst`

 * *Files identical despite different names*

### Comparing `heudiconv-0.8.0/docs/installation.rst` & `heudiconv-0.9.0/docs/installation.rst`

 * *Files 15% similar despite different names*

```diff
@@ -3,36 +3,36 @@
 ============
 
 ``Heudiconv`` is packaged and available from many different sources.
 
 
 Local
 =====
-Released versions of HeuDiConv are available on `PyPI <https://pypi.org/project/heudiconv/>`_ 
-and `conda <https://github.com/conda-forge/heudiconv-feedstock#installing-heudiconv>`_. 
+Released versions of HeuDiConv are available on `PyPI <https://pypi.org/project/heudiconv/>`_
+and `conda <https://github.com/conda-forge/heudiconv-feedstock#installing-heudiconv>`_.
 If installing through ``PyPI``, eg::
 
     pip install heudiconv[all]
 
-Manual installation of `dcm2niix <https://github.com/rordenlab/dcm2niix#install>`_ 
+Manual installation of `dcm2niix <https://github.com/rordenlab/dcm2niix#install>`_
 is required.
 
-On Debian-based systems we recommend using `NeuroDebian <http://neuro.debian.net>`_ 
+On Debian-based systems we recommend using `NeuroDebian <http://neuro.debian.net>`_
 which provides the `heudiconv package <http://neuro.debian.net/pkgs/heudiconv.html>`_.
 
 
 Docker
 ======
-If `Docker <https://docs.docker.com/install/>`_ is available on your system, you 
-can visit `our page on Docker Hub <https://hub.docker.com/r/nipy/heudiconv/tags>`_ 
+If `Docker <https://docs.docker.com/install/>`_ is available on your system, you
+can visit `our page on Docker Hub <https://hub.docker.com/r/nipy/heudiconv/tags>`_
 to view available releases. To pull the latest release, run::
 
-    $ docker pull nipy/heudiconv:0.8.0
+    $ docker pull nipy/heudiconv:0.9.0
 
 
 Singularity
 ===========
-If `Singularity <https://www.sylabs.io/singularity/>`_ is available on your system, 
-you can use it to pull and convert our Docker images! For example, to pull and 
+If `Singularity <https://www.sylabs.io/singularity/>`_ is available on your system,
+you can use it to pull and convert our Docker images! For example, to pull and
 build the latest release, you can run::
 
-    $ singularity pull docker://nipy/heudiconv:0.8.0
+    $ singularity pull docker://nipy/heudiconv:0.9.0
```

### Comparing `heudiconv-0.8.0/docs/tutorials.rst` & `heudiconv-0.9.0/docs/tutorials.rst`

 * *Files 26% similar despite different names*

```diff
@@ -9,10 +9,18 @@
 
 - `Walkthrough <http://reproducibility.stanford.edu/bids-tutorial-series-part-2a/>`_ by the `Stanford Center for Reproducible Neuroscience <http://reproducibility.stanford.edu/>`_.
 
 - `U of A Neuroimaging Core <https://neuroimaging-core-docs.readthedocs.io/en/latest/pages/heudiconv.html>`_ by `Dianne Patterson <https://github.com/dkp>`_.
 
 - `Sample Conversion: Coastal Coding 2019 <http://www.repronim.org/coco2019-training/presentations/heudiconv/#1>`_.
 
+- `A joined DataLad and HeuDiConv tutorial for reproducible fMRI studies <http://www.repronim.org/coco2019-training/04-02-reproin/>`_.
+
+- `The ReproIn conversion workflow overview <https://github.com/repronim/reproin#conversion>`_.
+
+- `Slides <https://docs.google.com/presentation/d/14UNWQVY49c9Xc-7sj1FkoILXnt-wYjW404oqT-FtCW8/edit#slide=id.p>`_ and
+  `recording <https://www.youtube.com/watch?v=j2SKX37-w4c&list=PLs3CA4ShM1DUX0nTMKfoB8Z6kdrZpByLa&index=5&t=0s>`_
+  of a ReproNim Webinar on ``heudiconv``.
+
 .. caution::
     Some of these tutorials may not be up to date with 
     the latest releases of ``heudiconv``.
```

### Comparing `heudiconv-0.8.0/docs/usage.rst` & `heudiconv-0.9.0/docs/usage.rst`

 * *Files 0% similar despite different names*

```diff
@@ -78,28 +78,28 @@
 
     OUTDIR=${1}
     # receive all directories, and index them per job array
     DCMDIRS=(${@:2})
     DCMDIR=${DCMDIRS[${SLURM_ARRAY_TASK_ID}]}
     echo Submitted directory: ${DCMDIR}
 
-    IMG="/singularity-images/heudiconv-0.8.0-dev.sif"
+    IMG="/singularity-images/heudiconv-0.9.0-dev.sif"
     CMD="singularity run -B ${DCMDIR}:/dicoms:ro -B ${OUTDIR}:/output -e ${IMG} --files /dicoms/ -o /output -f reproin -c dcm2niix -b notop --minmeta -l ."
 
     printf "Command:\n${CMD}\n"
     ${CMD}
     echo "Successful process"
 
 This script creates the top-level bids files (e.g.,
 ``dataset_description.json``)
 
 ..code:: shell
     #!/bin/bash
     set -eu
 
     OUTDIR=${1}
-    IMG="/singularity-images/heudiconv-0.8.0-dev.sif"
+    IMG="/singularity-images/heudiconv-0.9.0-dev.sif"
     CMD="singularity run -B ${OUTDIR}:/output -e ${IMG} --files /output -f reproin --command populate-templates"
 
     printf "Command:\n${CMD}\n"
     ${CMD}
     echo "Successful process"
```

### Comparing `heudiconv-0.8.0/heudiconv/bids.py` & `heudiconv-0.9.0/heudiconv/bids.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,33 +17,50 @@
 from .utils import (
     load_json,
     save_json,
     create_file_if_missing,
     json_dumps_pretty,
     set_readonly,
     is_readonly,
+    get_datetime,
 )
 
 lgr = logging.getLogger(__name__)
 
+# Fields to be populated in _scans files. Order matters
+SCANS_FILE_FIELDS = OrderedDict([
+    ("filename", OrderedDict([
+        ("Description", "Name of the nifti file")])),
+    ("acq_time", OrderedDict([
+        ("LongName", "Acquisition time"),
+        ("Description", "Acquisition time of the particular scan")])),
+    ("operator", OrderedDict([
+        ("Description", "Name of the operator")])),
+    ("randstr", OrderedDict([
+        ("LongName", "Random string"),
+        ("Description", "md5 hash of UIDs")])),
+])
 
 class BIDSError(Exception):
     pass
 
 
+BIDS_VERSION = "1.4.1"
+
+
 def populate_bids_templates(path, defaults={}):
     """Premake BIDS text files with templates"""
 
     lgr.info("Populating template files under %s", path)
     descriptor = op.join(path, 'dataset_description.json')
     if not op.lexists(descriptor):
         save_json(descriptor,
               OrderedDict([
                   ('Name', "TODO: name of the dataset"),
-                  ('BIDSVersion', "1.0.1"),
+                  ('BIDSVersion', BIDS_VERSION),
                   ('License', defaults.get('License',
                         "TODO: choose a license, e.g. PDDL "
                         "(http://opendatacommons.org/licenses/pddl/)")),
                   ('Authors', defaults.get('Authors',
                         ["TODO:", "First1 Last1", "First2 Last2", "..."])),
                   ('Acknowledgements', defaults.get('Acknowledgements',
                         'TODO: whom you want to acknowledge')),
@@ -154,15 +171,15 @@
         # See https://github.com/nipy/heudiconv/issues/277 for a usecase/bug
         # when we didn't touch existing one.
         # But the fields we enter (TaskName and CogAtlasID) might need need
         # to be populated from the file if it already exists
         placeholders = {
             "TaskName": ("TODO: full task name for %s" %
                          task_acq.split('_')[0].split('-')[1]),
-            "CogAtlasID": "TODO",
+            "CogAtlasID": "http://www.cognitiveatlas.org/task/id/TODO",
         }
         if op.lexists(task_file):
             j = load_json(task_file)
             # Retain possibly modified placeholder fields
             for f in placeholders:
                 if f in j:
                     placeholders[f] = j[f]
@@ -355,30 +372,17 @@
         os.unlink(fn)
     else:
         fnames2info = newrows
         # Populate _scans.json (an optional file to describe column names in
         # _scans.tsv). This auto generation will make BIDS-validator happy.
         scans_json = '.'.join(fn.split('.')[:-1] + ['json'])
         if not op.lexists(scans_json):
-            save_json(scans_json,
-                OrderedDict([
-                    ("filename", OrderedDict([
-                        ("Description", "Name of the nifti file")])),
-                    ("acq_time", OrderedDict([
-                        ("LongName", "Acquisition time"),
-                        ("Description", "Acquisition time of the particular scan")])),
-                    ("operator", OrderedDict([
-                        ("Description", "Name of the operator")])),
-                    ("randstr", OrderedDict([
-                        ("LongName", "Random string"),
-                        ("Description", "md5 hash of UIDs")])),
-                ]),
-                sort_keys=False)
+            save_json(scans_json, SCANS_FILE_FIELDS, sort_keys=False)
 
-    header = ['filename', 'acq_time', 'operator', 'randstr']
+    header = SCANS_FILE_FIELDS
     # prepare all the data rows
     data_rows = [[k] + v for k, v in fnames2info.items()]
     # sort by the date/filename
     try:
         data_rows_sorted = sorted(data_rows, key=lambda x: (x[1], x[0]))
     except TypeError as exc:
         lgr.warning("Sorting scans by date failed: %s", str(exc))
@@ -399,20 +403,19 @@
     -------
     row: list
         [ISO acquisition time, performing physician name, random string]
 
     """
     dcm_data = dcm.read_file(dcm_fn, stop_before_pixels=True, force=True)
     # we need to store filenames and acquisition times
-    # parse date and time and get it into isoformat
+    # parse date and time of start of run acquisition and get it into isoformat
     try:
-        date = dcm_data.ContentDate
-        time = dcm_data.ContentTime.split('.')[0]
-        td = time + date
-        acq_time = datetime.strptime(td, '%H%M%S%Y%m%d').isoformat()
+        date = dcm_data.AcquisitionDate
+        time = dcm_data.AcquisitionTime
+        acq_time = get_datetime(date, time)
     except (AttributeError, ValueError) as exc:
         lgr.warning("Failed to get date/time for the content: %s", str(exc))
         acq_time = ''
     # add random string
     # But let's make it reproducible by using all UIDs
     # (might change across versions?)
     randcontent = u''.join(
```

### Comparing `heudiconv-0.8.0/heudiconv/cli/monitor.py` & `heudiconv-0.9.0/heudiconv/cli/monitor.py`

 * *Files identical despite different names*

### Comparing `heudiconv-0.8.0/heudiconv/cli/run.py` & `heudiconv-0.9.0/heudiconv/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,377 +1,555 @@
-#!/usr/bin/env python
-
+"""Utility objects and functions"""
+import hashlib
 import os
-import os.path as op
-from argparse import ArgumentParser
+import tempfile
+import json
+import re
 import sys
+import shutil
+import copy
+import stat
+import os.path as op
+from pathlib import Path
+from collections import namedtuple
+from glob import glob
+from subprocess import check_output
+from datetime import datetime
 
-from .. import __version__, __packagename__
-from ..parser import get_study_sessions
-from ..utils import load_heuristic, anonymize_sid, treat_infofile, SeqInfo
-from ..convert import prep_conversion
-from ..bids import populate_bids_templates, tuneup_bids_json_files
-from ..queue import queue_conversion
+from nipype.utils.filemanip import which
 
-import inspect
 import logging
 lgr = logging.getLogger(__name__)
 
-INIT_MSG = "Running {packname} version {version} latest {latest}".format
+from json.decoder import JSONDecodeError
 
 
-def is_interactive():
-   """Return True if all in/outs are tty"""
-   # TODO: check on windows if hasattr check would work correctly and add value:
-   return sys.stdin.isatty() and sys.stdout.isatty() and sys.stderr.isatty()
+seqinfo_fields = [
+    'total_files_till_now',  # 0
+    'example_dcm_file',      # 1
+    'series_id',             # 2
+    'dcm_dir_name',          # 3
+    'series_files',          # 4
+    'unspecified',           # 5
+    'dim1', 'dim2', 'dim3', 'dim4', # 6, 7, 8, 9
+    'TR', 'TE',              # 10, 11
+    'protocol_name',         # 12
+    'is_motion_corrected',   # 13
+    'is_derived',            # 14
+    'patient_id',            # 15
+    'study_description',     # 16
+    'referring_physician_name', # 17
+    'series_description',    # 18
+    'sequence_name',         # 19
+    'image_type',            # 20
+    'accession_number',      # 21
+    'patient_age',           # 22
+    'patient_sex',           # 23
+    'date',                  # 24
+    'series_uid',            # 25
+ ]
+
+SeqInfo = namedtuple('SeqInfo', seqinfo_fields)
+
+StudySessionInfo = namedtuple(
+    'StudySessionInfo',
+    [
+        'locator',  # possible prefix identifying the study, e.g.
+                    # PI/dataset or just a dataset or empty (default)
+                    # Note that ATM there should be no multiple DICOMs with the
+                    # same StudyInstanceUID which would collide, i.e point to
+                    # the same subject/session. So 'locator' is pretty much an
+                    # assignment from StudyInstanceUID into some place within
+                    # hierarchy
+        'session',  # could be None
+        'subject',  # should be some ID defined either in cmdline or deduced
+    ]
+)
+
+
+class TempDirs(object):
+    """A helper to centralize handling and cleanup of dirs"""
+
+    def __init__(self):
+        self.dirs = []
+        self.exists = op.exists
+        self.lgr = logging.getLogger('tempdirs')
+
+    def __call__(self, prefix=None):
+        tmpdir = tempfile.mkdtemp(prefix=prefix)
+        self.dirs.append(tmpdir)
+        return tmpdir
+
+    def __del__(self):
+        try:
+            self.cleanup()
+        except AttributeError:
+            pass
+
+    def cleanup(self):
+        self.lgr.debug("Removing %d temporary directories", len(self.dirs))
+        for t in self.dirs[:]:
+            self.lgr.debug("Removing %s", t)
+            if self:
+                self.rmtree(t)
+        self.dirs = []
+
+    def rmtree(self, tmpdir):
+        if self.exists(tmpdir):
+            shutil.rmtree(tmpdir)
+        if tmpdir in self.dirs:
+            self.dirs.remove(tmpdir)
+
+
+def docstring_parameter(*sub):
+    """ Borrowed from https://stackoverflow.com/a/10308363/6145776 """
+    def dec(obj):
+        obj.__doc__ = obj.__doc__.format(*sub)
+        return obj
+    return dec
 
 
-def setup_exceptionhook():
-    """
-    Overloads default sys.excepthook with our exceptionhook handler.
+def anonymize_sid(sid, anon_sid_cmd):
+
+    cmd = [anon_sid_cmd, sid]
+    shell_return = check_output(cmd)
+
+    if isinstance(shell_return, bytes) and isinstance(sid, str):
+        anon_sid = shell_return.decode()
+    else:
+        anon_sid = shell_return
+
+    return anon_sid.strip()
+
+
+def create_file_if_missing(filename, content):
+    """Create file if missing, so we do not
+    override any possibly introduced changes"""
+    if op.lexists(filename):
+        return False
+    dirname = op.dirname(filename)
+    if not op.exists(dirname):
+        os.makedirs(dirname)
+    with open(filename, 'w') as f:
+        f.write(content)
+    return True
+
 
-    If interactive, our exceptionhook handler will invoke pdb.post_mortem;
-    if not interactive, then invokes default handler.
+def read_config(infile):
+    with open(infile, 'rt') as fp:
+        info = eval(fp.read())
+    return info
+
+
+def write_config(outfile, info):
+    from pprint import PrettyPrinter
+    with open(outfile, 'wt') as fp:
+        fp.writelines(PrettyPrinter().pformat(info))
+
+
+def _canonical_dumps(json_obj, **kwargs):
+    """ Dump `json_obj` to string, allowing for Python newline bug
+
+    Runs ``json.dumps(json_obj, \*\*kwargs), then removes trailing whitespaces
+    added when doing indent in some Python versions. See
+    https://bugs.python.org/issue16333. Bug seems to be fixed in 3.4, for now
+    fixing manually not only for aestetics but also to guarantee the same
+    result across versions of Python.
     """
-    def _pdb_excepthook(type, value, tb):
-        if is_interactive():
-            import traceback
-            import pdb
-            traceback.print_exception(type, value, tb)
-            # print()
-            pdb.post_mortem(tb)
-        else:
-            lgr.warning(
-              "We cannot setup exception hook since not in interactive mode")
+    out = json.dumps(json_obj, **kwargs)
+    if 'indent' in kwargs:
+        out = out.replace(' \n', '\n')
+    return out
 
-    sys.excepthook = _pdb_excepthook
 
+def load_json(filename):
+    """Load data from a json file
 
-def process_extra_commands(outdir, args):
+    Parameters
+    ----------
+    filename : str
+        Filename to load data from.
+
+    Returns
+    -------
+    data : dict
     """
-    Perform custom command instead of regular operations. Supported commands:
-    ['treat-json', 'ls', 'populate-templates']
+    try:
+        with open(filename, 'r') as fp:
+            data = json.load(fp)
+    except JSONDecodeError:
+        lgr.error("{fname} is not a valid json file".format(fname=filename))
+        raise
+
+    return data
+    
+
+def assure_no_file_exists(path):
+    """Check if file or symlink (git-annex?) exists, and if so -- remove"""
+    if os.path.lexists(path):
+        os.unlink(path)
+
+
+def save_json(filename, data, indent=2, sort_keys=True, pretty=False):
+    """Save data to a json file
 
     Parameters
     ----------
-    outdir : String
-        Output directory
-    args : Namespace
-        arguments
-    """
-    if args.command == 'treat-jsons':
-        for f in args.files:
-            treat_infofile(f)
-    elif args.command == 'ls':
-        ensure_heuristic_arg(args)
-        heuristic = load_heuristic(args.heuristic)
-        heuristic_ls = getattr(heuristic, 'ls', None)
-        for f in args.files:
-            study_sessions = get_study_sessions(
-                args.dicom_dir_template, [f], heuristic, outdir,
-                args.session, args.subjs, grouping=args.grouping)
-            print(f)
-            for study_session, sequences in study_sessions.items():
-                suf = ''
-                if heuristic_ls:
-                    suf += heuristic_ls(study_session, sequences)
-                print(
-                    "\t%s %d sequences%s"
-                    % (str(study_session), len(sequences), suf)
-                )
-    elif args.command == 'populate-templates':
-        ensure_heuristic_arg(args)
-        heuristic = load_heuristic(args.heuristic)
-        for f in args.files:
-            populate_bids_templates(f, getattr(heuristic, 'DEFAULT_FIELDS', {}))
-    elif args.command == 'sanitize-jsons':
-        tuneup_bids_json_files(args.files)
-    elif args.command == 'heuristics':
-        from ..utils import get_known_heuristics_with_descriptions
-        for name_desc in get_known_heuristics_with_descriptions().items():
-            print("- %s: %s" % name_desc)
-    elif args.command == 'heuristic-info':
-        ensure_heuristic_arg(args)
-        from ..utils import get_heuristic_description
-        print(get_heuristic_description(args.heuristic, full=True))
-    else:
-        raise ValueError("Unknown command %s", args.command)
-    return
+    filename : str
+        Filename to save data in.
+    data : dict
+        Dictionary to save in json file.
+    indent : int, optional
+    sort_keys : bool, optional
+    pretty : bool, optional
+
+    """
+    assure_no_file_exists(filename)
+    dumps_kw = dict(sort_keys=sort_keys, indent=indent)
+    j = None
+    if pretty:
+        try:
+            j = json_dumps_pretty(data, **dumps_kw)
+        except AssertionError as exc:
+            pretty = False
+            lgr.warning(
+                "Prettyfication of .json failed (%s).  "
+                "Original .json will be kept as is.  Please share (if you "
+                "could) "
+                "that file (%s) with HeuDiConv developers"
+                % (str(exc), filename)
+            )
+    if not pretty:
+        j = _canonical_dumps(data, **dumps_kw)
+    assert j is not None  # one way or another it should have been set to a str
+    with open(filename, 'w') as fp:
+        fp.write(j)
+
+
+def json_dumps_pretty(j, indent=2, sort_keys=True):
+    """Given a json structure, pretty print it by colliding numeric arrays
+    into a line.
 
+    If resultant structure differs from original -- throws exception
+    """
+    js = _canonical_dumps(j, indent=indent, sort_keys=sort_keys)
+    # trim away \n and spaces between entries of numbers
+    js_ = re.sub(
+        '[\n ]+("?[-+.0-9e]+"?,?) *\n(?= *"?[-+.0-9e]+"?)', r' \1',
+        js, flags=re.MULTILINE)
+    # uniform no spaces before ]
+    js_ = re.sub(" *\]", "]", js_)
+    # uniform spacing before numbers
+    # But that thing could screw up dates within strings which would have 2 spaces
+    # in a date like Mar  3 2017, so we do negative lookahead to avoid changing
+    # in those cases
+    #import pdb; pdb.set_trace()
+    js_ = re.sub(
+        '(?<!\w{3})'    # negative lookbehind for the month
+        '  *("?[-+.0-9e]+"?)'
+        '(?! [123]\d{3})'  # negative lookahead for a year
+        '(?P<space> ?)[ \n]*',
+        r' \1\g<space>', js_)
+    # no spaces after [
+    js_ = re.sub('\[ ', '[', js_)
+    # the load from the original dump and reload from tuned up
+    # version should result in identical values since no value
+    # must be changed, just formatting.
+    j_just_reloaded = json.loads(js)
+    j_tuned = json.loads(js_)
+
+    assert j_just_reloaded == j_tuned, \
+       "Values differed when they should have not. "\
+       "Report to the heudiconv developers"
+
+    return js_
+
+
+def treat_infofile(filename):
+    """Tune up generated .json file (slim down, pretty-print for humans).
+    """
+    j = load_json(filename)
+    j_slim = slim_down_info(j)
+    save_json(filename, j_slim, sort_keys=True, pretty=True)
+    set_readonly(filename)
 
-def ensure_heuristic_arg(args):
-    from ..utils import get_known_heuristic_names
-    if not args.heuristic:
-        raise ValueError("Specify heuristic using -f. Known are: %s"
-                         % ', '.join(get_known_heuristic_names()))
-
-
-def main(argv=None):
-    parser = get_parser()
-    args = parser.parse_args(argv)
-    # exit if nothing to be done
-    if not args.files and not args.dicom_dir_template and not args.command:
-        lgr.warning("Nothing to be done - displaying usage help")
-        parser.print_help()
-        sys.exit(1)
-    # To be done asap so anything random is deterministic
-    if args.random_seed is not None:
-        import random
-        random.seed(args.random_seed)
-        import numpy
-        numpy.random.seed(args.random_seed)
-    # Ensure only supported bids options are passed
-    if args.debug:
-        lgr.setLevel(logging.DEBUG)
-    # Should be possible but only with a single subject -- will be used to
-    # override subject deduced from the DICOMs
-    if args.files and args.subjs and len(args.subjs) > 1:
-        raise ValueError(
-            "Unable to processes multiple `--subjects` with files"
+
+def slim_down_info(j):
+    """Given an aggregated info structure, removes excessive details
+
+    Such as CSA fields, and SourceImageSequence which on Siemens files could be
+    huge and not providing any additional immediately usable information.
+    If needed, could be recovered from stored DICOMs
+    """
+    j = copy.deepcopy(j)  # we will do in-place modification on a copy
+    dicts = []
+    # poor man programming for now
+    if 'const' in j.get('global', {}):
+        dicts.append(j['global']['const'])
+    if 'samples' in j.get('time', {}):
+        dicts.append(j['time']['samples'])
+    for d in dicts:
+        for k in list(d.keys()):
+            if k.startswith('Csa') or k.lower() in {'sourceimagesequence'}:
+                del d[k]
+    return j
+
+
+def get_known_heuristic_names():
+    """Return a list of heuristic names present under heudiconv/heuristics"""
+    import heudiconv.heuristics
+    candidates = {
+        op.splitext(op.basename(x))[0]
+        for hp in heudiconv.heuristics.__path__
+        for x in glob(op.join(hp, '*.py')) + glob(op.join(hp, '*.py[co]'))
+    }
+    return sorted(
+        filter(
+            lambda c: not (c.startswith('test_') or c.startswith('_')),
+            candidates
         )
+    )
+
 
-    if args.debug:
-        setup_exceptionhook()
-    process_args(args)
-
-
-def get_parser():
-    docstr = ("""Example:
-             heudiconv -d 'rawdata/{subject}' -o . -f heuristic.py -s s1 s2 s3""")
-    parser = ArgumentParser(description=docstr)
-    parser.add_argument('--version', action='version', version=__version__)
-    group = parser.add_mutually_exclusive_group()
-    group.add_argument('-d', '--dicom_dir_template', dest='dicom_dir_template',
-                       help='location of dicomdir that can be indexed with '
-                       'subject id {subject} and session {session}. Tarballs '
-                       '(can be compressed) are supported in addition to '
-                       'directory. All matching tarballs for a subject are '
-                       'extracted and their content processed in a single '
-                       'pass. If multiple tarballs are found, each is '
-                       'assumed to be a separate session and the --ses '
-                       'argument is ignored. Note that you might need to '
-                       'surround the value with quotes to avoid {...} being '
-                       'considered by shell')
-    group.add_argument('--files', nargs='*',
-                       help='Files (tarballs, dicoms) or directories '
-                       'containing files to process. Cannot be provided if '
-                       'using --dicom_dir_template.')
-    parser.add_argument('-s', '--subjects', dest='subjs', type=str, nargs='*',
-                        help='list of subjects - required for dicom template. '
-                        'If not provided, DICOMS would first be "sorted" and '
-                        'subject IDs deduced by the heuristic')
-    parser.add_argument('-c', '--converter',
-                        choices=('dcm2niix', 'none'), default='dcm2niix',
-                        help='tool to use for DICOM conversion. Setting to '
-                        '"none" disables the actual conversion step -- useful'
-                        'for testing heuristics.')
-    parser.add_argument('-o', '--outdir', default=os.getcwd(),
-                        help='output directory for conversion setup (for '
-                        'further customization and future reference. This '
-                        'directory will refer to non-anonymized subject IDs')
-    parser.add_argument('-l', '--locator', default=None,
-                        help='study path under outdir.  If provided, '
-                        'it overloads the value provided by the heuristic. '
-                        'If --datalad is enabled, every directory within '
-                        'locator becomes a super-dataset thus establishing a '
-                        'hierarchy. Setting to "unknown" will skip that dataset')
-    parser.add_argument('-a', '--conv-outdir', default=None,
-                        help='output directory for converted files. By default '
-                        'this is identical to --outdir. This option is most '
-                        'useful in combination with --anon-cmd')
-    parser.add_argument('--anon-cmd', default=None,
-                        help='command to run to convert subject IDs used for '
-                        'DICOMs to anonymized IDs. Such command must take a '
-                        'single argument and return a single anonymized ID. '
-                        'Also see --conv-outdir')
-    parser.add_argument('-f', '--heuristic', dest='heuristic',
-                        help='Name of a known heuristic or path to the Python'
-                             'script containing heuristic')
-    parser.add_argument('-p', '--with-prov', action='store_true',
-                        help='Store additional provenance information. '
-                        'Requires python-rdflib.')
-    parser.add_argument('-ss', '--ses', dest='session', default=None,
-                        help='session for longitudinal study_sessions, default '
-                        'is none')
-    parser.add_argument('-b', '--bids', nargs='*',
-                        metavar=('BIDSOPTION1', 'BIDSOPTION2'),
-                        choices=['notop'],
-                        dest='bids_options',
-                        help='flag for output into BIDS structure. Can also '
-                        'take bids specific options, e.g., --bids notop.'
-                        'The only currently supported options is'
-                        '"notop", which skips creation of top-level bids '
-                        'files. This is useful when running in batch mode to '
-                        'prevent possible race conditions.')
-    parser.add_argument('--overwrite', action='store_true', default=False,
-                        help='flag to allow overwriting existing converted files')
-    parser.add_argument('--datalad', action='store_true',
-                        help='Store the entire collection as DataLad '
-                        'dataset(s). Small files will be committed directly to '
-                        'git, while large to annex. New version (6) of annex '
-                        'repositories will be used in a "thin" mode so it '
-                        'would look to mortals as just any other regular '
-                        'directory (i.e. no symlinks to under .git/annex).  '
-                        'For now just for BIDS mode.')
-    parser.add_argument('--dbg', action='store_true', dest='debug',
-                        help='Do not catch exceptions and show exception '
-                        'traceback')
-    parser.add_argument('--command',
-                        choices=(
-                            'heuristics', 'heuristic-info',
-                            'ls', 'populate-templates',
-                            'sanitize-jsons', 'treat-jsons',
-                        ),
-                        help='custom actions to be performed on provided '
-                        'files instead of regular operation.')
-    parser.add_argument('-g', '--grouping', default='studyUID',
-                        choices=('studyUID', 'accession_number', 'all', 'custom'),
-                        help='How to group dicoms (default: by studyUID)')
-    parser.add_argument('--minmeta', action='store_true',
-                        help='Exclude dcmstack meta information in sidecar '
-                        'jsons')
-    parser.add_argument('--random-seed', type=int, default=None,
-                        help='Random seed to initialize RNG')
-    parser.add_argument('--dcmconfig', default=None,
-                        help='JSON file for additional dcm2niix configuration')
-    submission = parser.add_argument_group('Conversion submission options')
-    submission.add_argument('-q', '--queue', choices=("SLURM", None),
-                            default=None,
-                            help='batch system to submit jobs in parallel')
-    submission.add_argument('--queue-args', dest='queue_args', default=None,
-                            help='Additional queue arguments passed as '
-                            'single string of Argument=Value pairs space '
-                            'separated.')
-    return parser
-
-
-def process_args(args):
-    """Given a structure of arguments from the parser perform computation"""
-
-    # Deal with provided files or templates
-    # pre-process provided list of files and possibly sort into groups/sessions
-    # Group files per each study/sid/session
+def load_heuristic(heuristic):
+    """Load heuristic from the file, return the module
+    """
+    if os.path.sep in heuristic or os.path.lexists(heuristic):
+        heuristic_file = op.realpath(heuristic)
+        path, fname = op.split(heuristic_file)
+        try:
+            old_syspath = sys.path[:]
+            sys.path.insert(0, path)
+            mod = __import__(fname.split('.')[0])
+            mod.filename = heuristic_file
+        finally:
+            sys.path = old_syspath
+    else:
+        from importlib import import_module
+        try:
+            mod = import_module('heudiconv.heuristics.%s' % heuristic)
+            mod.filename = mod.__file__.rstrip('co')  # remove c or o from pyc/pyo
+        except Exception as exc:
+            raise ImportError(
+                "Failed to import heuristic %s: %s"
+                % (heuristic, exc)
+            )
+    return mod
 
-    outdir = op.abspath(args.outdir)
 
+def get_heuristic_description(name, full=False):
     try:
-        import etelemetry
-        latest = etelemetry.get_project("nipy/heudiconv")
-    except Exception as e:
-        lgr.warning("Could not check for version updates: %s", str(e))
-        latest = {"version": 'Unknown'}
-
-    lgr.info(INIT_MSG(packname=__packagename__,
-                      version=__version__,
-                      latest=latest["version"]))
+        mod = load_heuristic(name)
+        desc = (getattr(mod, '__doc__', '') or '').strip()
+        return desc.split(os.linesep)[0] if not full else desc
+    except Exception as exc:
+        return "Failed to load: %s" % exc
+
+
+def get_known_heuristics_with_descriptions():
+    from collections import OrderedDict
+    heuristics = OrderedDict()
+    for name in get_known_heuristic_names():
+        heuristics[name] = get_heuristic_description(name, full=False)
+    return heuristics
+
+
+def safe_copyfile(src, dest, overwrite=False):
+    """Copy file but blow if destination name already exists"""
+    return _safe_op_file(src, dest, "copyfile", overwrite=overwrite)
+
 
-    if args.command:
-        process_extra_commands(outdir, args)
+def safe_movefile(src, dest, overwrite=False):
+    """Move file but blow if destination name already exists"""
+    return _safe_op_file(src, dest, "move", overwrite=overwrite)
+
+
+def _safe_op_file(src, dest, operation, overwrite=False):
+    """Copy or move file but blow if destination name already exists
+
+    Parameters
+    ----------
+    operation: str, {copyfile, move}
+    """
+    if op.isdir(dest):
+        dest = op.join(dest, op.basename(src))
+    if op.realpath(src) == op.realpath(dest):
+        lgr.debug("Source %s = destination %s", src, dest)
+        return
+    if op.lexists(dest):
+        if not overwrite:
+            raise RuntimeError(
+                "was asked to %s %s but destination already exists: %s"
+                % (operation, src, dest)
+            )
+        os.unlink(dest)
+    getattr(shutil, operation)(src, dest)
+
+
+# Globals to check filewriting permissions
+ALL_CAN_WRITE = (stat.S_IWUSR | stat.S_IWGRP | stat.S_IWOTH)
+ALL_CAN_READ = (stat.S_IRUSR | stat.S_IRGRP | stat.S_IROTH)
+assert ALL_CAN_READ >> 1 == ALL_CAN_WRITE  # Assumption in the code
+
+def set_readonly(path, read_only=True):
+    """Make file read only or writeable while preserving "access levels"
+
+    So if file was not readable by others, it should remain not readable by
+    others.
+
+    Parameters
+    ----------
+    path : str
+    read_only : bool, optional
+        If True (default) - would make it read-only. If False, would make it
+        writeable for levels where it is readable
+
+    """
+
+    # get current permissions
+    perms = stat.S_IMODE(os.lstat(path).st_mode)
+    # set new permissions
+    if read_only:
+        new_perms = perms & (~ALL_CAN_WRITE)
+    else:
+        # need to set only for those which had read bit set
+        # read bit is <<1 away from write bit
+        whocanread = perms & ALL_CAN_READ
+        thosecanwrite = whocanread >> 1
+        new_perms = perms | thosecanwrite
+    # apply and return those target permissions
+    os.chmod(path, new_perms)
+    return new_perms
+
+
+def is_readonly(path):
+    """Return True if it is a fully read-only file (dereferences the symlink)
+    """
+    # get current permissions
+    perms = stat.S_IMODE(os.lstat(os.path.realpath(path)).st_mode)
+    # should be true if anyone is allowed to write
+    return not bool(perms & ALL_CAN_WRITE)
+
+
+def clear_temp_dicoms(item_dicoms):
+    """Ensures DICOM temporary directories are safely cleared"""
+    try:
+        tmp = Path(op.commonprefix(item_dicoms)).parents[1]
+    except IndexError:
         return
-    #
-    # Load heuristic -- better do it asap to make sure it loads correctly
-    #
-    if not args.heuristic:
-        raise RuntimeError("No heuristic specified - add to arguments and rerun")
-
-    if args.queue:
-        lgr.info("Queuing %s conversion", args.queue)
-        iterarg, iterables = ("files", len(args.files)) if args.files else \
-                             ("subjects", len(args.subjs))
-        queue_conversion(args.queue, iterarg, iterables, args.queue_args)
-        sys.exit(0)
-
-    heuristic = load_heuristic(args.heuristic)
-
-    study_sessions = get_study_sessions(args.dicom_dir_template, args.files,
-                                        heuristic, outdir, args.session,
-                                        args.subjs, grouping=args.grouping)
-
-    # extract tarballs, and replace their entries with expanded lists of files
-    # TODO: we might need to sort so sessions are ordered???
-    lgr.info("Need to process %d study sessions", len(study_sessions))
-
-    # processed_studydirs = set()
-
-    for (locator, session, sid), files_or_seqinfo in study_sessions.items():
-
-        # Allow for session to be overloaded from command line
-        if args.session is not None:
-            session = args.session
-        if args.locator is not None:
-            locator = args.locator
-        if not len(files_or_seqinfo):
-            raise ValueError("nothing to process?")
-        # that is how life is ATM :-/ since we don't do sorting if subj
-        # template is provided
-        if isinstance(files_or_seqinfo, dict):
-            assert(isinstance(list(files_or_seqinfo.keys())[0], SeqInfo))
-            dicoms = None
-            seqinfo = files_or_seqinfo
+    if (str(tmp.parent) == tempfile.gettempdir()
+        and str(tmp.stem).startswith('heudiconvDCM')
+        and op.exists(str(tmp))):
+        # clean up directory holding dicoms
+        shutil.rmtree(str(tmp))
+
+
+def file_md5sum(filename):
+    with open(filename, 'rb') as f:
+        return hashlib.md5(f.read()).hexdigest()
+
+
+# Borrowed from DataLad (MIT license), with "archives" functionality commented
+# out
+class File(object):
+    """Helper for a file entry in the create_tree/@with_tree
+
+    It allows to define additional settings for entries
+    """
+    def __init__(self, name, executable=False):
+        """
+
+        Parameters
+        ----------
+        name : str
+          Name of the file
+        executable: bool, optional
+          Make it executable
+        """
+        self.name = name
+        self.executable = executable
+
+    def __str__(self):
+        return self.name
+
+
+def create_tree(path, tree, archives_leading_dir=True):
+    """Given a list of tuples (name, load) or a dict create such a tree
+
+    if load is a tuple or a dict itself -- that would create either a subtree
+    or an archive with that content and place it into the tree if name ends
+    with .tar.gz
+    """
+    lgr.log(5, "Creating a tree under %s", path)
+    if not op.exists(path):
+        os.makedirs(path)
+
+    if isinstance(tree, dict):
+        tree = tree.items()
+
+    for file_, load in tree:
+        if isinstance(file_, File):
+            executable = file_.executable
+            name = file_.name
+        else:
+            executable = False
+            name = file_
+        full_name = op.join(path, name)
+        if isinstance(load, (tuple, list, dict)):
+            # if name.endswith('.tar.gz') or name.endswith('.tar') or name.endswith('.zip'):
+            #     create_tree_archive(path, name, load, archives_leading_dir=archives_leading_dir)
+            # else:
+            create_tree(full_name, load, archives_leading_dir=archives_leading_dir)
         else:
-            dicoms = files_or_seqinfo
-            seqinfo = None
+            with open(full_name, 'w') as f:
+                f.write(load)
+        if executable:
+            os.chmod(full_name, os.stat(full_name).st_mode | stat.S_IEXEC)
 
-        if locator == 'unknown':
-            lgr.warning("Skipping unknown locator dataset")
-            continue
-
-        anon_sid = anonymize_sid(sid, args.anon_cmd) if args.anon_cmd else None
-        if args.anon_cmd:
-            lgr.info('Anonymized {} to {}'.format(sid, anon_sid))
-
-        study_outdir = op.join(outdir, locator or '')
-        anon_outdir = args.conv_outdir or outdir
-        anon_study_outdir = op.join(anon_outdir, locator or '')
-
-        # TODO: --datalad  cmdline option, which would take care about initiating
-        # the outdir -> study_outdir datasets if not yet there
-        if args.datalad:
-            from ..external.dlad import prepare_datalad
-            dlad_sid = sid if not anon_sid else anon_sid
-            dl_msg = prepare_datalad(anon_study_outdir, anon_outdir, dlad_sid,
-                                     session, seqinfo, dicoms,
-                                     args.bids_options)
-
-        lgr.info("PROCESSING STARTS: {0}".format(
-            str(dict(subject=sid, outdir=study_outdir, session=session))))
-
-        prep_conversion(sid,
-                        dicoms,
-                        study_outdir,
-                        heuristic,
-                        converter=args.converter,
-                        anon_sid=anon_sid,
-                        anon_outdir=anon_study_outdir,
-                        with_prov=args.with_prov,
-                        ses=session,
-                        bids_options=args.bids_options,
-                        seqinfo=seqinfo,
-                        min_meta=args.minmeta,
-                        overwrite=args.overwrite,
-                        dcmconfig=args.dcmconfig,
-                        grouping=args.grouping,)
-
-        lgr.info("PROCESSING DONE: {0}".format(
-            str(dict(subject=sid, outdir=study_outdir, session=session))))
-
-        if args.datalad:
-            from ..external.dlad import add_to_datalad
-            msg = "Converted subject %s" % dl_msg
-            # TODO:  whenever propagate to supers work -- do just
-            # ds.save(msg=msg)
-            #  also in batch mode might fail since we have no locking ATM
-            #  and theoretically no need actually to save entire study
-            #  we just need that
-            add_to_datalad(outdir, study_outdir, msg, args.bids_options)
-
-    # if args.bids:
-    #     # Let's populate BIDS templates for folks to take care about
-    #     for study_outdir in processed_studydirs:
-    #         populate_bids_templates(study_outdir)
-    #
-    # TODO: record_collection of the sid/session although that information
-    # is pretty much present in .heudiconv/SUBJECT/info so we could just poke there
 
+def get_typed_attr(obj, attr, _type, default=None):
+    """
+    Typecasts an object's named attribute. If the attribute cannot be
+    converted, the default value is returned instead.
 
-if __name__ == "__main__":
-    main()
+    Parameters
+    ----------
+    obj: Object
+    attr: Attribute
+    _type: Type
+    default: value, optional
+    """
+    try:
+        val = _type(getattr(obj, attr, default))
+    except (TypeError, ValueError):
+        return default
+    return val
+
+
+def get_datetime(date, time, *, microseconds=True):
+    """
+    Combine date and time from dicom to isoformat.
+
+    Parameters
+    ----------
+    date : str
+        Date in YYYYMMDD format.
+    time : str
+        Time in either HHMMSS.ffffff format or HHMMSS format.
+    microseconds: bool, optional
+        Either to include microseconds in the output
+
+    Returns
+    -------
+    datetime_str : str
+        Combined date and time in ISO format, with microseconds as
+        if fraction was provided in 'time', and 'microseconds' was
+        True.
+    """
+    if '.' not in time:
+        # add dummy microseconds if not available for strptime to parse
+        time += '.000000'
+    td = time + ':' + date
+    datetime_str = datetime.strptime(td, '%H%M%S.%f:%Y%m%d').isoformat()
+    if not microseconds:
+        datetime_str = datetime_str.split('.', 1)[0]
+    return datetime_str
```

### Comparing `heudiconv-0.8.0/heudiconv/convert.py` & `heudiconv-0.9.0/heudiconv/convert.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,37 +1,42 @@
 import filelock
 import os
 import os.path as op
 import logging
 from math import nan
 import shutil
 import sys
+import random
 import re
 
+from .due import due, Doi
+
 from .utils import (
     read_config,
     load_json,
     save_json,
     write_config,
     TempDirs,
     safe_copyfile,
+    safe_movefile,
     treat_infofile,
     set_readonly,
     clear_temp_dicoms,
     seqinfo_fields,
     assure_no_file_exists,
     file_md5sum
 )
 from .bids import (
     convert_sid_bids,
     populate_bids_templates,
     save_scans_key,
     tuneup_bids_json_files,
     add_participant_record,
-    BIDSError
+    BIDSError,
+    BIDS_VERSION,
 )
 from .dicoms import (
     group_dicoms_into_seqinfos,
     embed_metadata_from_dicoms,
     compress_dicoms
 )
 
@@ -78,15 +83,15 @@
                 outprefix = template.format(**parameters)
                 convert_info.append((op.join(outpath, outprefix),
                                     outtype, files))
     return convert_info
 
 
 def prep_conversion(sid, dicoms, outdir, heuristic, converter, anon_sid,
-                    anon_outdir, with_prov, ses, bids_options, seqinfo, 
+                    anon_outdir, with_prov, ses, bids_options, seqinfo,
                     min_meta, overwrite, dcmconfig, grouping):
     if dicoms:
         lgr.info("Processing %d dicoms", len(dicoms))
     elif seqinfo:
         lgr.info("Processing %d pre-sorted seqinfo entries", len(seqinfo))
     else:
         raise ValueError("neither dicoms nor seqinfo dict was provided")
@@ -229,14 +234,168 @@
                                        anon_sid,
                                        keys[0].patient_age,
                                        keys[0].patient_sex)
             populate_bids_templates(anon_outdir,
                                     getattr(heuristic, 'DEFAULT_FIELDS', {}))
 
 
+def update_complex_name(metadata, filename, suffix):
+    """
+    Insert `_part-<mag|phase>` entity into filename if data are from a
+    sequence with magnitude/phase part.
+
+    Parameters
+    ----------
+    metadata : dict
+        Scan metadata dictionary from BIDS sidecar file.
+    filename : str
+        Incoming filename
+    suffix : str
+        An index used for cases where a single scan produces multiple files,
+        but the differences between those files are unknown.
+
+    Returns
+    -------
+    filename : str
+        Updated filename with rec entity added in appropriate position.
+    """
+    # Some scans separate magnitude/phase differently
+    # A small note: _phase is deprecated, but this may add part-mag to
+    # magnitude data while leaving phase data with a separate suffix,
+    # depending on how one sets up their heuristic.
+    unsupported_types = ['_phase',
+                         '_magnitude', '_magnitude1', '_magnitude2',
+                         '_phasediff', '_phase1', '_phase2']
+    if any(ut in filename for ut in unsupported_types):
+        return filename
+
+    # Check to see if it is magnitude or phase part:
+    if 'M' in metadata.get('ImageType'):
+        mag_or_phase = 'mag'
+    elif 'P' in metadata.get('ImageType'):
+        mag_or_phase = 'phase'
+    else:
+        mag_or_phase = suffix
+
+    # Determine scan suffix
+    filetype = '_' + filename.split('_')[-1]
+
+    # Insert rec label
+    if not ('_part-%s' % mag_or_phase) in filename:
+        # If "_part-" is specified, prepend the 'mag_or_phase' value.
+        if '_part-' in filename:
+            raise BIDSError(
+                "Part label for images will be automatically set, "
+                "remove from heuristic"
+            )
+
+        # Insert it **before** the following string(s), whichever appears first.
+        for label in ['_recording', '_proc', '_space', filetype]:
+            if (label == filetype) or (label in filename):
+                filename = filename.replace(
+                    label, "_part-%s%s" % (mag_or_phase, label)
+                )
+                break
+
+    return filename
+
+
+def update_multiecho_name(metadata, filename, echo_times):
+    """
+    Insert `_echo-<num>` entity into filename if data are from a multi-echo
+    sequence.
+
+    Parameters
+    ----------
+    metadata : dict
+        Scan metadata dictionary from BIDS sidecar file.
+    filename : str
+        Incoming filename
+    echo_times : list
+        List of all echo times from scan. Used to determine the echo *number*
+        (i.e., index) if field is missing from metadata.
+
+    Returns
+    -------
+    filename : str
+        Updated filename with echo entity added, if appropriate.
+    """
+    # Field maps separate echoes differently
+    unsupported_types = [
+        '_magnitude', '_magnitude1', '_magnitude2',
+        '_phasediff', '_phase1', '_phase2', '_fieldmap'
+    ]
+    if any(ut in filename for ut in unsupported_types):
+        return filename
+
+    # Get the EchoNumber from json file info.  If not present, use EchoTime
+    if 'EchoNumber' in metadata.keys():
+        echo_number = metadata['EchoNumber']
+    else:
+        echo_number = echo_times.index(metadata['EchoTime']) + 1
+
+    # Determine scan suffix
+    filetype = '_' + filename.split('_')[-1]
+
+    # Insert it **before** the following string(s), whichever appears first.
+    for label in ['_recording', '_proc', '_space', filetype]:
+        if (label == filetype) or (label in filename):
+            filename = filename.replace(
+                label, "_echo-%s%s" % (echo_number, label)
+            )
+            break
+
+    return filename
+
+
+def update_uncombined_name(metadata, filename, channel_names):
+    """
+    Insert `_ch-<num>` entity into filename if data are from a sequence
+    with "save uncombined".
+
+    Parameters
+    ----------
+    metadata : dict
+        Scan metadata dictionary from BIDS sidecar file.
+    filename : str
+        Incoming filename
+    channel_names : list
+        List of all channel names from scan. Used to determine the channel
+        *number* (i.e., index) if field is missing from metadata.
+
+    Returns
+    -------
+    filename : str
+        Updated filename with ch entity added, if appropriate.
+    """
+    # In case any scan types separate channels differently
+    unsupported_types = []
+    if any(ut in filename for ut in unsupported_types):
+        return filename
+
+    # Determine the channel number
+    channel_number = ''.join([c for c in metadata['CoilString'] if c.isdigit()])
+    if not channel_number:
+        channel_number = channel_names.index(metadata['CoilString']) + 1
+    channel_number = str(channel_number).zfill(2)
+
+    # Determine scan suffix
+    filetype = '_' + filename.split('_')[-1]
+
+    # Insert it **before** the following string(s), whichever appears first.
+    # Choosing to put channel near the end since it's not in the specification yet.
+    for label in ['_recording', '_proc', '_space', filetype]:
+        if (label == filetype) or (label in filename):
+            filename = filename.replace(
+                label, "_ch-%s%s" % (channel_number, label)
+            )
+            break
+    return filename
+
+
 def convert(items, converter, scaninfo_suffix, custom_callable, with_prov,
             bids_options, outdir, min_meta, overwrite, symlink=True, prov_file=None,
             dcmconfig=None):
     """Perform actual conversion (calls to converter etc) given info from
     heuristic's `infotodict`
 
     Parameters
@@ -255,14 +414,28 @@
     Returns
     -------
     None
     """
     prov_files = []
     tempdirs = TempDirs()
 
+    if bids_options is not None:
+        due.cite(
+            # doi matches the BIDS_VERSION
+            Doi("10.5281/zenodo.4085321"),
+            description="Brain Imaging Data Structure (BIDS) Specification",
+            path="bids",
+            version=BIDS_VERSION,
+            tags=["implementation"])
+        due.cite(
+            Doi("10.1038/sdata.2016.44"),
+            description="Brain Imaging Data Structure (BIDS), Original paper",
+            path="bids",
+            tags=["documentation"])
+
     for item_idx, item in enumerate(items):
 
         prefix, outtypes, item_dicoms = item[:3]
         if not isinstance(outtypes, (list, tuple)):
             outtypes = (outtypes,)
 
         prefix_dirname = op.dirname(prefix)
@@ -439,28 +612,32 @@
     fromfile = dcmconfig if dcmconfig else None
     if fromfile:
         lgr.info("Using custom config file %s", fromfile)
 
     convertnode = Node(Dcm2niix(from_file=fromfile), name='convert')
     convertnode.base_dir = tmpdir
     convertnode.inputs.source_names = item_dicoms
-    convertnode.inputs.out_filename = prefix
+    convertnode.inputs.out_filename = op.basename(prefix) + "_heudiconv%03d" % random.randint(0, 999)
+    prefix_dir = op.dirname(prefix)
+    # if provided prefix had a path in it -- pass is as output_dir instead of default curdir
+    if prefix_dir:
+        convertnode.inputs.output_dir = prefix_dir
 
     if nipype.__version__.split('.')[0] == '0':
         # deprecated since 1.0, might be needed(?) before
         convertnode.inputs.terminal_output = 'allatonce'
     else:
         convertnode.terminal_output = 'allatonce'
     convertnode.inputs.bids_format = bids_options is not None
     eg = convertnode.run()
 
     # prov information
     prov_file = prefix + '_prov.ttl' if with_prov else None
     if prov_file:
-        safe_copyfile(op.join(convertnode.base_dir,
+        safe_movefile(op.join(convertnode.base_dir,
                               convertnode.name,
                               'provenance.ttl'),
                       prov_file)
 
     return eg, prov_file
 
 
@@ -494,16 +671,16 @@
 
     if not len(res_files):
         lgr.debug("DICOMs {} were not converted".format(item_dicoms))
         return
 
     if isdefined(res.outputs.bvecs) and isdefined(res.outputs.bvals):
         outname_bvecs, outname_bvals = prefix + '.bvec', prefix + '.bval'
-        safe_copyfile(res.outputs.bvecs, outname_bvecs, overwrite)
-        safe_copyfile(res.outputs.bvals, outname_bvals, overwrite)
+        safe_movefile(res.outputs.bvecs, outname_bvecs, overwrite)
+        safe_movefile(res.outputs.bvals, outname_bvals, overwrite)
 
     if isinstance(res_files, list):
         res_files = sorted(res_files)
         # we should provide specific handling for fmap,
         # dwi etc which might spit out multiple files
 
         suffixes = ([str(i+1) for i in range(len(res_files))]
@@ -530,116 +707,76 @@
         #   (e.g. MGH ME-MPRAGE). They do set a 'EchoNumber', but not for the
         #   first echo.  To compound the problem, the echoes are NOT in order,
         #   so the first NIfTI file does not correspond to echo-1, etc. So, we
         #   need to know, beforehand, whether we are dealing with a multi-echo
         #   series. To do that, the most straightforward way is to read the
         #   echo times for all bids_files and see if they are all the same or not.
 
-        # Check for varying echo times
-        echo_times = sorted(list(set(
-            b.get('EchoTime', nan)
-            for b in bids_metas
-            if b
-        )))
-
-        is_multiecho = len(echo_times) > 1
+        # Collect some metadata across all images
+        echo_times, channel_names, image_types = set(), set(), set()
+        for metadata in bids_metas:
+            if not metadata:
+                continue
+            echo_times.add(metadata.get('EchoTime', nan))
+            channel_names.add(metadata.get('CoilString', nan))
+            image_types.update(metadata.get('ImageType', [nan]))
+        is_multiecho = len(set(filter(bool, echo_times))) > 1  # Check for varying echo times
+        is_uncombined = len(set(filter(bool, channel_names))) > 1  # Check for uncombined data
+        is_complex = 'M' in image_types and 'P' in image_types  # Determine if data are complex (magnitude + phase)
 
         ### Loop through the bids_files, set the output name and save files
         for fl, suffix, bids_file, bids_meta in zip(res_files, suffixes, bids_files, bids_metas):
 
             # TODO: monitor conversion duration
 
             # set the prefix basename for this specific file (we'll modify it,
             # and we don't want to modify it for all the bids_files):
             this_prefix_basename = prefix_basename
 
-            # _sbref sequences reconstructing magnitude and phase generate
-            # two NIfTI files IN THE SAME SERIES, so we cannot just add
-            # the suffix, if we want to be bids compliant:
-            if bids_meta and this_prefix_basename.endswith('_sbref') \
-                    and len(suffixes) > len(echo_times):
-                if len(suffixes) != len(echo_times)*2:
-                    lgr.warning(
-                        "Got %d suffixes for %d echo times, which isn't "
-                        "multiple of two as if it was magnitude + phase pairs",
-                        len(suffixes), len(echo_times)
+            # Update name for certain criteria
+            if bids_file:
+                if is_multiecho:
+                    this_prefix_basename = update_multiecho_name(
+                        bids_meta, this_prefix_basename, echo_times
                     )
-                # Check to see if it is magnitude or phase reconstruction:
-                if 'M' in bids_meta.get('ImageType'):
-                    mag_or_phase = 'magnitude'
-                elif 'P' in bids_meta.get('ImageType'):
-                    mag_or_phase = 'phase'
-                else:
-                    mag_or_phase = suffix
-
-                # Insert reconstruction label
-                if not ("_rec-%s" % mag_or_phase) in this_prefix_basename:
 
-                    # If "_rec-" is specified, prepend the 'mag_or_phase' value.
-                    if ('_rec-' in this_prefix_basename):
-                        raise BIDSError(
-                        "Reconstruction label for multi-echo single-band"
-                        " reference images will be automatically set, remove"
-                        " from heuristic"
-                        )
-
-                    # If not, insert "_rec-" + 'mag_or_phase' into the prefix_basename
-                    #   **before** "_run", "_echo" or "_sbref", whichever appears first:
-                    for label in ['_run', '_echo', '_sbref']:
-                        if (label in this_prefix_basename):
-                            this_prefix_basename = this_prefix_basename.replace(
-                                label, "_rec-%s%s" % (mag_or_phase, label)
-                            )
-                            break
-
-            # Now check if this run is multi-echo
-            # (Note: it can be _sbref and multiecho, so don't use "elif"):
-            # For multi-echo sequences, we have to specify the echo number in
-            # the file name:
-            if bids_meta and is_multiecho:
-                # Get the EchoNumber from json file info.  If not present, use EchoTime
-                if 'EchoNumber' in bids_meta:
-                    echo_number = bids_meta['EchoNumber']
-                else:
-                    echo_number = echo_times.index(bids_meta['EchoTime']) + 1
+                if is_complex:
+                    this_prefix_basename = update_complex_name(
+                        bids_meta, this_prefix_basename, suffix
+                    )
 
-                supported_multiecho = ['_bold', '_phase', '_epi', '_sbref', '_T1w', '_PDT2']
-                # Now, decide where to insert it.
-                # Insert it **before** the following string(s), whichever appears first.
-                for imgtype in supported_multiecho:
-                    if (imgtype in this_prefix_basename):
-                        this_prefix_basename = this_prefix_basename.replace(
-                            imgtype, "_echo-%d%s" % (echo_number, imgtype)
-                        )
-                        break
+                if is_uncombined:
+                    this_prefix_basename = update_uncombined_name(
+                        bids_meta, this_prefix_basename, channel_names
+                    )
 
             # Fallback option:
             # If we have failed to modify this_prefix_basename, because it didn't fall
             #   into any of the options above, just add the suffix at the end:
             if this_prefix_basename == prefix_basename:
                 this_prefix_basename += suffix
 
             # Finally, form the outname by stitching the directory and outtype:
             outname = op.join(prefix_dirname, this_prefix_basename)
             outfile = outname + '.' + outtype
 
             # Write the files needed:
-            safe_copyfile(fl, outfile, overwrite)
+            safe_movefile(fl, outfile, overwrite)
             if bids_file:
                 outname_bids_file = "%s.json" % (outname)
-                safe_copyfile(bids_file, outname_bids_file, overwrite)
+                safe_movefile(bids_file, outname_bids_file, overwrite)
                 bids_outfiles.append(outname_bids_file)
 
     # res_files is not a list
     else:
         outname = "{}.{}".format(prefix, outtype)
-        safe_copyfile(res_files, outname, overwrite)
+        safe_movefile(res_files, outname, overwrite)
         if isdefined(res.outputs.bids):
             try:
-                safe_copyfile(res.outputs.bids, outname_bids, overwrite)
+                safe_movefile(res.outputs.bids, outname_bids, overwrite)
                 bids_outfiles.append(outname_bids)
             except TypeError as exc:  ##catch lists
                 raise TypeError("Multiple BIDS sidecars detected.")
     return bids_outfiles
 
 
 def  add_taskname_to_infofile(infofiles):
```

### Comparing `heudiconv-0.8.0/heudiconv/dicoms.py` & `heudiconv-0.9.0/heudiconv/dicoms.py`

 * *Files 0% similar despite different names*

```diff
@@ -472,15 +472,14 @@
     tmpdir = tempdirs(prefix='embedmeta')
 
     # We need to assure that paths are absolute if they are relative
     item_dicoms = list(map(op.abspath, item_dicoms))
 
     embedfunc = Node(Function(input_names=['dcmfiles', 'niftifile', 'infofile',
                                            'bids_info',],
-                              output_names=['outfile', 'meta'],
                               function=embed_dicom_and_nifti_metadata),
                      name='embedder')
     embedfunc.inputs.dcmfiles = item_dicoms
     embedfunc.inputs.niftifile = op.abspath(outname)
     embedfunc.inputs.infofile = op.abspath(scaninfo)
     embedfunc.inputs.bids_info = load_json(op.abspath(outname_bids)) if (bids_options is not None) else None
     embedfunc.base_dir = tmpdir
```

### Comparing `heudiconv-0.8.0/heudiconv/external/dcmstack.py` & `heudiconv-0.9.0/heudiconv/external/dcmstack.py`

 * *Files identical despite different names*

### Comparing `heudiconv-0.8.0/heudiconv/external/dlad.py` & `heudiconv-0.9.0/heudiconv/external/dlad.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from glob import glob
 from os import path as op
 
 from ..utils import create_file_if_missing
 
 lgr = logging.getLogger(__name__)
 
-MIN_VERSION = '0.12.4'
+from ..info import MIN_DATALAD_VERSION as MIN_VERSION
 
 
 def prepare_datalad(studydir, outdir, sid, session, seqinfo, dicoms, bids):
     """ Prepare data for datalad """
     from datalad.api import Dataset
     datalad_msg_suf = ' %s' % sid
     if session:
@@ -101,33 +101,32 @@
     if op.lexists(op.join(ds.path, '.heudiconv')):
         dsh_path = op.join(ds.path, '.heudiconv')
         dsh = Dataset(dsh_path)
         if not dsh.is_installed():
             # Previously we did not have it as a submodule, and since no
             # automagic migration is implemented, we just need to check first
             # if any path under .heudiconv is already under git control
-            if any(x[0].startswith('.heudiconv/') for x in
-                   ds.repo.repo.index.entries.keys()):
+            if any(x.startswith('.heudiconv/') for x in ds.repo.get_files()):
                 lgr.warning("%s has .heudiconv not as a submodule from previous"
                             " versions of heudiconv. No automagic migration is "
                             "yet provided", ds)
             else:
                 dsh = ds.create(path='.heudiconv',
                                 force=True,
                                 # shared_access='all'
                                 )
         # Since .heudiconv could contain sensitive information
         # we place all files under annex and then add
         if create_file_if_missing(op.join(dsh_path, '.gitattributes'),
                                   """* annex.largefiles=anything"""):
-            ds.add('.heudiconv/.gitattributes',
+            ds.save('.heudiconv/.gitattributes',
                    to_git=True,
                    message="Added gitattributes to place all .heudiconv content"
                            " under annex")
-    ds.add('.', recursive=True, save=False,
+    ds.save('.', recursive=True
            # not in effect! ?
            #annex_add_opts=['--include-dotfiles']
            )
 
     # TODO: filter for only changed files?
     # Provide metadata for sensitive information
     mark_sensitive(ds, 'sourcedata')
```

### Comparing `heudiconv-0.8.0/heudiconv/external/tests/test_dlad.py` & `heudiconv-0.9.0/heudiconv/external/tests/test_dlad.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,14 @@
         {
             'f1': 'd1',
             'f2': 'd2',
             'g1': 'd3',
             'g2': 'd1',
          }
     )
-    ds.add('.')
+    ds.save('.')
     mark_sensitive(ds, 'f*')
     all_meta = dict(ds.repo.get_metadata('.'))
     target_rec = {'distribution-restrictions': ['sensitive']}
     # g2 since the same content
     assert not all_meta.pop('g1', None)  # nothing or empty record
     assert all_meta == {'f1': target_rec, 'f2': target_rec, 'g2': target_rec}
```

### Comparing `heudiconv-0.8.0/heudiconv/heuristics/banda-bids.py` & `heudiconv-0.9.0/heudiconv/heuristics/banda-bids.py`

 * *Files identical despite different names*

### Comparing `heudiconv-0.8.0/heudiconv/heuristics/bids_ME.py` & `heudiconv-0.9.0/heudiconv/heuristics/bids_ME.py`

 * *Files identical despite different names*

### Comparing `heudiconv-0.8.0/heudiconv/heuristics/bids_with_ses.py` & `heudiconv-0.9.0/heudiconv/heuristics/bids_with_ses.py`

 * *Files identical despite different names*

### Comparing `heudiconv-0.8.0/heudiconv/heuristics/cmrr_heuristic.py` & `heudiconv-0.9.0/heudiconv/heuristics/cmrr_heuristic.py`

 * *Files identical despite different names*

### Comparing `heudiconv-0.8.0/heudiconv/heuristics/convertall.py` & `heudiconv-0.9.0/heudiconv/heuristics/convertall.py`

 * *Files identical despite different names*

### Comparing `heudiconv-0.8.0/heudiconv/heuristics/example.py` & `heudiconv-0.9.0/heudiconv/heuristics/example.py`

 * *Files identical despite different names*

### Comparing `heudiconv-0.8.0/heudiconv/heuristics/multires_7Tbold.py` & `heudiconv-0.9.0/heudiconv/heuristics/multires_7Tbold.py`

 * *Files identical despite different names*

### Comparing `heudiconv-0.8.0/heudiconv/heuristics/reproin.py` & `heudiconv-0.9.0/heudiconv/heuristics/reproin.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,14 +119,16 @@
 
 import os
 import re
 from collections import OrderedDict
 import hashlib
 from glob import glob
 
+from heudiconv.due import due, Doi
+
 import logging
 lgr = logging.getLogger('heudiconv')
 
 # pythons before 3.7 didn't have re.Pattern, it was some protected
 # _sre.SRE_Pattern, so let's just sample a class of the compiled regex
 re_Pattern = re.compile('.').__class__
 
@@ -463,14 +465,18 @@
     # seqinfo = sequences.keys()[0]
     return ' study hash: %s' % get_study_hash(seqinfo)
 
 
 # XXX we killed session indicator!  what should we do now?!!!
 # WE DON:T NEED IT -- it will be provided into conversion_info as `session`
 # So we just need subdir and file_suffix!
+@due.dcite(
+    Doi('10.5281/zenodo.1207117'),
+    path='heudiconv.heuristics.reproin',
+    description='ReproIn heudiconv heuristic for turnkey conversion into BIDS')
 def infotodict(seqinfo):
     """Heuristic evaluator for determining which runs belong where
 
     allowed template fields - follow python string module:
 
     item: index within category
     subject: participant id
```

### Comparing `heudiconv-0.8.0/heudiconv/heuristics/reproin_validator.cfg` & `heudiconv-0.9.0/heudiconv/heuristics/reproin_validator.cfg`

 * *Files identical despite different names*

### Comparing `heudiconv-0.8.0/heudiconv/heuristics/studyforrest_phase2.py` & `heudiconv-0.9.0/heudiconv/heuristics/studyforrest_phase2.py`

 * *Files identical despite different names*

### Comparing `heudiconv-0.8.0/heudiconv/heuristics/test_reproin.py` & `heudiconv-0.9.0/heudiconv/heuristics/test_reproin.py`

 * *Files identical despite different names*

### Comparing `heudiconv-0.8.0/heudiconv/heuristics/uc_bids.py` & `heudiconv-0.9.0/heudiconv/heuristics/uc_bids.py`

 * *Files identical despite different names*

### Comparing `heudiconv-0.8.0/heudiconv/info.py` & `heudiconv-0.9.0/heudiconv/info.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.8.0"
+__version__ = "0.9.0"
 __author__ = "HeuDiConv team and contributors"
 __url__ = "https://github.com/nipy/heudiconv"
 __packagename__ = 'heudiconv'
 __description__ = "Heuristic DICOM Converter"
 __license__ = "Apache 2.0"
 __longdesc__ = """Convert DICOM dirs based on heuristic info - HeuDiConv
 uses the dcmstack package and dcm2niix tool to convert DICOM directories or
@@ -19,31 +19,32 @@
 ]
 
 PYTHON_REQUIRES = ">=3.5"
 
 REQUIRES = [
     'nibabel',
     'pydicom',
-    'nipype >=1.0.0; python_version > "3.0"',
-    'nipype >=1.0.0,!=1.2.1,!=1.2.2; python_version == "2.7"',
-    'pathlib',
+    'nipype >=1.2.3',
     'dcmstack>=0.8',
     'etelemetry',
     'filelock>=3.0.12',
 ]
 
 TESTS_REQUIRES = [
     'six',
     'pytest',
     'mock',
     'tinydb',
     'inotify',
 ]
 
+MIN_DATALAD_VERSION = '0.12.4'
 EXTRA_REQUIRES = {
     'tests': TESTS_REQUIRES,
-    'extras': [],  # Requires patched version ATM ['dcmstack'],
-    'datalad': ['datalad >=0.12.3']
+    'extras': [
+        'duecredit',  # optional dependency
+    ],  # Requires patched version ATM ['dcmstack'],
+    'datalad': ['datalad >=%s' % MIN_DATALAD_VERSION]
 }
 
 # Flatten the lists
 EXTRA_REQUIRES['all'] = sum(EXTRA_REQUIRES.values(), [])
```

### Comparing `heudiconv-0.8.0/heudiconv/parser.py` & `heudiconv-0.9.0/heudiconv/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import atexit
 import logging
 import os
 import os.path as op
 from glob import glob
 import re
 
 from collections import defaultdict
@@ -9,17 +10,21 @@
 import tarfile
 from tempfile import mkdtemp
 
 from .dicoms import group_dicoms_into_seqinfos
 from .utils import (
     docstring_parameter,
     StudySessionInfo,
+    TempDirs,
 )
 
 lgr = logging.getLogger(__name__)
+tempdirs = TempDirs()
+# Ensure they are cleaned up upon exit
+atexit.register(tempdirs.cleanup)
 
 _VCS_REGEX = '%s\.(?:git|gitattributes|svn|bzr|hg)(?:%s|$)' % (op.sep, op.sep)
 
 @docstring_parameter(_VCS_REGEX)
 def find_files(regex, topdir=op.curdir, exclude=None,
                exclude_vcs=True, dirs=False):
     """Generator to find files matching regex
@@ -62,15 +67,15 @@
 
     # tarfiles already know what they contain, and often the filenames
     # are unique, or at least in a unqiue subdir per session
     # strategy: extract everything in a temp dir and assemble a list
     # of all files in all tarballs
 
     # cannot use TempDirs since will trigger cleanup with __del__
-    tmpdir = mkdtemp(prefix='heudiconvDCM')
+    tmpdir = tempdirs('heudiconvDCM')
 
     sessions = defaultdict(list)
     session = 0
     if not isinstance(fl, (list, tuple)):
         fl = list(fl)
 
     # needs sorting to keep the generated "session" label deterministic
```

### Comparing `heudiconv-0.8.0/heudiconv/queue.py` & `heudiconv-0.9.0/heudiconv/queue.py`

 * *Files identical despite different names*

### Comparing `heudiconv-0.8.0/heudiconv/tests/data/01-anat-scout/0001.dcm` & `heudiconv-0.9.0/heudiconv/tests/data/01-anat-scout/0001.dcm`

 * *Files identical despite different names*

### Comparing `heudiconv-0.8.0/heudiconv/tests/data/01-fmap_acq-3mm/1.3.12.2.1107.5.2.43.66112.2016101409263663466202201.dcm` & `heudiconv-0.9.0/heudiconv/tests/data/01-fmap_acq-3mm/1.3.12.2.1107.5.2.43.66112.2016101409263663466202201.dcm`

 * *Files identical despite different names*

### Comparing `heudiconv-0.8.0/heudiconv/tests/data/axasc35.dcm` & `heudiconv-0.9.0/heudiconv/tests/data/axasc35.dcm`

 * *Files identical despite different names*

### Comparing `heudiconv-0.8.0/heudiconv/tests/data/phantom.dcm` & `heudiconv-0.9.0/heudiconv/tests/data/phantom.dcm`

 * *Files identical despite different names*

### Comparing `heudiconv-0.8.0/heudiconv/tests/test_dicoms.py` & `heudiconv-0.9.0/heudiconv/tests/test_dicoms.py`

 * *Files identical despite different names*

### Comparing `heudiconv-0.8.0/heudiconv/tests/test_heuristics.py` & `heudiconv-0.9.0/heudiconv/tests/test_heuristics.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,15 +112,15 @@
         for i, row in enumerate(reader):
             if i == 0:
                 assert(row == ['filename', 'acq_time', 'operator', 'randstr'])
             assert(len(row) == 4)
             if i != 0:
                 assert(os.path.exists(pjoin(dirname(scans_keys[0]), row[0])))
                 assert(re.match(
-                    '^[\d]{4}-[\d]{2}-[\d]{2}T[\d]{2}:[\d]{2}:[\d]{2}$',
+                    '^[\d]{4}-[\d]{2}-[\d]{2}T[\d]{2}:[\d]{2}:[\d]{2}.[\d]{6}$',
                     row[1]))
 
 
 @patch('sys.stdout', new_callable=StringIO)
 def test_ls(stdout):
     args = (
             "-f reproin --command ls --files %s"
```

### Comparing `heudiconv-0.8.0/heudiconv/tests/test_main.py` & `heudiconv-0.9.0/heudiconv/tests/test_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 # TODO: break this up by modules
 
-from heudiconv.cli.run import (
-    main as runner,
-    process_args,
-)
+from heudiconv.cli.run import main as runner
+from heudiconv.main import workflow
 from heudiconv import __version__
 from heudiconv.utils import (create_file_if_missing,
                              set_readonly,
                              is_readonly)
 from heudiconv.bids import (populate_bids_templates,
                             add_participant_record,
                             get_formatted_scans_key_row,
@@ -145,15 +143,15 @@
     old_hexsha = ds.repo.get_hexsha()
     # Now let's check that if we had previously converted data so that
     # .heudiconv was not a submodule, we still would not fail
     dsh_path = os.path.join(ds.path, '.heudiconv')
     dummy_path = os.path.join(dsh_path, 'dummy.nii.gz')
 
     create_file_if_missing(dummy_path, '')
-    ds.add(dummy_path, message="added a dummy file")
+    ds.save(dummy_path, message="added a dummy file")
     # next call must not fail, should just issue a warning
     add_to_datalad(str(tmpdir), studydir_, None, False)
     ds.repo.is_under_annex(dummy_path)
     assert not ds.repo.dirty
     assert '.heudiconv/dummy.nii.gz' in ds.repo.get_files()
 
     # Let's now roll back and make it a proper submodule
@@ -169,15 +167,15 @@
 def test_get_formatted_scans_key_row():
     dcm_fn = \
         '%s/01-fmap_acq-3mm/1.3.12.2.1107.5.2.43.66112.2016101409263663466202201.dcm' \
          % TESTS_DATA_PATH
 
     row1 = get_formatted_scans_key_row(dcm_fn)
     assert len(row1) == 3
-    assert row1[0] == '2016-10-14T09:26:36'
+    assert row1[0] == '2016-10-14T09:26:34.692500'
     assert row1[1] == 'n/a'
     prandstr1 = row1[2]
 
     # if we rerun - should be identical!
     row2 = get_formatted_scans_key_row(dcm_fn)
     prandstr2 = row2[2]
     assert(prandstr1 == prandstr2)
@@ -284,16 +282,11 @@
     assert (cachedir / 'dicominfo.tsv').exists()
     assert (cachedir / 'S01.auto.txt').exists()
     assert (cachedir / 'S01.edit.txt').exists()
 
 
 def test_no_etelemetry():
     # smoke test at large - just verifying that no crash if no etelemetry
-    class args:
-        outdir = '/dev/null'
-        command = 'ls'
-        heuristic = 'reproin'
-        files = []  # Nothing to list
-
     # must not fail if etelemetry no found
     with patch.dict('sys.modules', {'etelemetry': None}):
-        process_args(args)
+        workflow(outdir='/dev/null', command='ls',
+                 heuristic='reproin', files=[])
```

### Comparing `heudiconv-0.8.0/heudiconv/tests/test_monitor.py` & `heudiconv-0.9.0/heudiconv/tests/test_monitor.py`

 * *Files identical despite different names*

### Comparing `heudiconv-0.8.0/heudiconv/tests/test_queue.py` & `heudiconv-0.9.0/heudiconv/tests/test_queue.py`

 * *Files identical despite different names*

### Comparing `heudiconv-0.8.0/heudiconv/tests/test_regression.py` & `heudiconv-0.9.0/heudiconv/tests/test_regression.py`

 * *Files identical despite different names*

### Comparing `heudiconv-0.8.0/heudiconv/tests/test_tarballs.py` & `heudiconv-0.9.0/heudiconv/tests/test_tarballs.py`

 * *Files identical despite different names*

### Comparing `heudiconv-0.8.0/heudiconv/tests/test_utils.py` & `heudiconv-0.9.0/heudiconv/tests/test_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     get_known_heuristics_with_descriptions,
     get_heuristic_description,
     load_heuristic,
     json_dumps_pretty,
     load_json,
     create_tree,
     save_json,
+    get_datetime,
     JSONDecodeError)
 
 import pytest
 from .utils import HEURISTICS_PATH
 
 
 def test_get_known_heuristics_with_descriptions():
@@ -81,7 +82,16 @@
     # test valid json
     vcontent = {"secret": "spy"}
     vfname = "valid.json"
     valid_json_file = str(tmpdir / vfname)
     save_json(valid_json_file, vcontent)
     
     assert load_json(valid_json_file) == vcontent
+
+
+def test_get_datetime():
+    """
+    Test utils.get_datetime()
+    """
+    assert get_datetime('20200512', '162130') == '2020-05-12T16:21:30'
+    assert get_datetime('20200512', '162130.5') == '2020-05-12T16:21:30.500000'
+    assert get_datetime('20200512', '162130.5', microseconds=False) == '2020-05-12T16:21:30'
```

### Comparing `heudiconv-0.8.0/heudiconv/tests/utils.py` & `heudiconv-0.9.0/heudiconv/tests/utils.py`

 * *Files identical despite different names*

### Comparing `heudiconv-0.8.0/heudiconv.egg-info/PKG-INFO` & `heudiconv-0.9.0/heudiconv.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heudiconv
-Version: 0.8.0
+Version: 0.9.0
 Summary: Heuristic DICOM Converter
 Home-page: UNKNOWN
 Author: HeuDiConv team and contributors
 License: Apache 2.0
 Description: Convert DICOM dirs based on heuristic info - HeuDiConv
         uses the dcmstack package and dcm2niix tool to convert DICOM directories or
         tarballs into collections of NIfTI files following pre-defined heuristic(s).
@@ -13,11 +13,11 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.5
-Provides-Extra: tests
-Provides-Extra: extras
-Provides-Extra: datalad
 Provides-Extra: all
+Provides-Extra: datalad
+Provides-Extra: extras
+Provides-Extra: tests
```

### Comparing `heudiconv-0.8.0/heudiconv.egg-info/SOURCES.txt` & `heudiconv-0.9.0/heudiconv.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,17 @@
 docs/api/parser.rst
 docs/api/queue.rst
 docs/api/utils.rst
 heudiconv/__init__.py
 heudiconv/bids.py
 heudiconv/convert.py
 heudiconv/dicoms.py
+heudiconv/due.py
 heudiconv/info.py
+heudiconv/main.py
 heudiconv/parser.py
 heudiconv/queue.py
 heudiconv/utils.py
 heudiconv.egg-info/PKG-INFO
 heudiconv.egg-info/SOURCES.txt
 heudiconv.egg-info/dependency_links.txt
 heudiconv.egg-info/entry_points.txt
@@ -67,14 +69,15 @@
 heudiconv/heuristics/reproin.py
 heudiconv/heuristics/reproin_validator.cfg
 heudiconv/heuristics/studyforrest_phase2.py
 heudiconv/heuristics/test_reproin.py
 heudiconv/heuristics/uc_bids.py
 heudiconv/tests/__init__.py
 heudiconv/tests/anonymize_script.py
+heudiconv/tests/test_convert.py
 heudiconv/tests/test_dicoms.py
 heudiconv/tests/test_heuristics.py
 heudiconv/tests/test_main.py
 heudiconv/tests/test_monitor.py
 heudiconv/tests/test_queue.py
 heudiconv/tests/test_regression.py
 heudiconv/tests/test_tarballs.py
```

### Comparing `heudiconv-0.8.0/setup.py` & `heudiconv-0.9.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,17 +15,15 @@
 
     thispath = op.dirname(__file__)
     ldict = locals()
 
     # Get version and release info, which is all stored in heudiconv/info.py
     info_file = op.join(thispath, 'heudiconv', 'info.py')
     with open(info_file) as infofile:
-        # exec(infofile.read(), globals(), ldict)
-        # Workaround for python 2.7 prior 2.7.8
-        eval(compile(infofile.read(), '<string>', 'exec'), globals(), ldict)
+        exec(infofile.read(), globals(), ldict)
 
 
     def findsome(subdir, extensions):
         """Find files under subdir having specified extensions
 
         Leading directory (datalad) gets stripped
         """
```

### Comparing `heudiconv-0.8.0/utils/gen-docker-image.sh` & `heudiconv-0.9.0/utils/gen-docker-image.sh`

 * *Files identical despite different names*

### Comparing `heudiconv-0.8.0/utils/test-compare-two-versions.sh` & `heudiconv-0.9.0/utils/test-compare-two-versions.sh`

 * *Files 6% similar despite different names*

```diff
@@ -22,14 +22,18 @@
 function run() {
    heudiconvdir="$1"
    out=$outdir/$2
    shift
    shift
    source $heudiconvdir/venvs/dev3/bin/activate
    whichheudiconv=$(which heudiconv)
+   # to get "reproducible" dataset UUIDs (might be detremental if we had multiple datalad calls
+   # but since we use python API for datalad, should be Ok)
+   export DATALAD_SEED=1
+
 
    if [ ! -e "$out" ]; then
 	  # just do full conversion
 	  echo "Running $whichheudiconv with log in $out.log"
 	  $RUN heudiconv --random-seed 1 -o $out "$@" >| $out.log 2>&1 \
 	  || {
 		  echo "Exited with $?  Check $out.log" >&2
```

### Comparing `heudiconv-0.8.0/utils/update_changes.sh` & `heudiconv-0.9.0/utils/update_changes.sh`

 * *Files identical despite different names*

