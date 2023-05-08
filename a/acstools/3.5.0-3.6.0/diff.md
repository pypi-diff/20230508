# Comparing `tmp/acstools-3.5.0.tar.gz` & `tmp/acstools-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acstools-3.5.0.tar", last modified: Tue Dec  6 20:23:13 2022, max compression
+gzip compressed data, was "acstools-3.6.0.tar", last modified: Mon May  8 21:39:46 2023, max compression
```

## Comparing `acstools-3.5.0.tar` & `acstools-3.6.0.tar`

### file list

```diff
@@ -1,96 +1,106 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 20:23:13.196243 acstools-3.5.0/
--rw-r--r--   0 runner    (1001) docker     (122)       33 2022-12-06 20:22:32.000000 acstools-3.5.0/.bandit.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 20:23:13.172244 acstools-3.5.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 20:23:13.176244 acstools-3.5.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (122)     2040 2022-12-06 20:22:32.000000 acstools-3.5.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (122)      922 2022-12-06 20:22:32.000000 acstools-3.5.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (122)     1447 2022-12-06 20:22:32.000000 acstools-3.5.0/.github/ISSUE_TEMPLATE/question.md
--rw-r--r--   0 runner    (1001) docker     (122)     1189 2022-12-06 20:22:32.000000 acstools-3.5.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (122)      145 2022-12-06 20:22:32.000000 acstools-3.5.0/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (122)      774 2022-12-06 20:22:32.000000 acstools-3.5.0/.github/labeler.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 20:23:13.176244 acstools-3.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     3452 2022-12-06 20:22:32.000000 acstools-3.5.0/.github/workflows/ci_workflows.yml
--rw-r--r--   0 runner    (1001) docker     (122)     2414 2022-12-06 20:22:32.000000 acstools-3.5.0/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1193 2022-12-06 20:22:32.000000 acstools-3.5.0/.github/workflows/open_actions.yml
--rw-r--r--   0 runner    (1001) docker     (122)      681 2022-12-06 20:22:32.000000 acstools-3.5.0/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (122)      470 2022-12-06 20:22:32.000000 acstools-3.5.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)      503 2022-12-06 20:22:32.000000 acstools-3.5.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       56 2022-12-06 20:22:32.000000 acstools-3.5.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (122)      288 2022-12-06 20:22:32.000000 acstools-3.5.0/CITATION.md
--rw-r--r--   0 runner    (1001) docker     (122)     3207 2022-12-06 20:22:32.000000 acstools-3.5.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (122)     1539 2022-12-06 20:22:32.000000 acstools-3.5.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (122)      179 2022-12-06 20:22:32.000000 acstools-3.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1235 2022-12-06 20:23:13.196243 acstools-3.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      675 2022-12-06 20:22:32.000000 acstools-3.5.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 20:23:13.180244 acstools-3.5.0/acstools/
--rw-r--r--   0 runner    (1001) docker     (122)      618 2022-12-06 20:22:32.000000 acstools-3.5.0/acstools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3338 2022-12-06 20:22:32.000000 acstools-3.5.0/acstools/acs2d.py
--rw-r--r--   0 runner    (1001) docker     (122)    38670 2022-12-06 20:22:32.000000 acstools-3.5.0/acstools/acs_destripe.py
--rw-r--r--   0 runner    (1001) docker     (122)    26899 2022-12-06 20:22:32.000000 acstools-3.5.0/acstools/acs_destripe_plus.py
--rw-r--r--   0 runner    (1001) docker     (122)     3046 2022-12-06 20:22:32.000000 acstools-3.5.0/acstools/acsccd.py
--rw-r--r--   0 runner    (1001) docker     (122)     2845 2022-12-06 20:22:32.000000 acstools-3.5.0/acstools/acscte.py
--rw-r--r--   0 runner    (1001) docker     (122)     3290 2022-12-06 20:22:32.000000 acstools-3.5.0/acstools/acscteforwardmodel.py
--rw-r--r--   0 runner    (1001) docker     (122)    10606 2022-12-06 20:22:32.000000 acstools-3.5.0/acstools/acsphotcte.py
--rw-r--r--   0 runner    (1001) docker     (122)     5738 2022-12-06 20:22:32.000000 acstools-3.5.0/acstools/acsrej.py
--rw-r--r--   0 runner    (1001) docker     (122)     2492 2022-12-06 20:22:32.000000 acstools-3.5.0/acstools/acssum.py
--rw-r--r--   0 runner    (1001) docker     (122)    13234 2022-12-06 20:22:32.000000 acstools-3.5.0/acstools/acszpt.py
--rw-r--r--   0 runner    (1001) docker     (122)     2345 2022-12-06 20:22:32.000000 acstools-3.5.0/acstools/calacs.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 20:23:13.184244 acstools-3.5.0/acstools/data/
--rw-r--r--   0 runner    (1001) docker     (122)     2043 2022-12-06 20:22:32.000000 acstools-3.5.0/acstools/data/polarizer_tables.yaml
--rw-r--r--   0 runner    (1001) docker     (122)    16594 2022-12-06 20:22:32.000000 acstools-3.5.0/acstools/polarization_tools.py
--rw-r--r--   0 runner    (1001) docker     (122)    36791 2022-12-06 20:22:32.000000 acstools-3.5.0/acstools/satdet.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 20:23:13.188244 acstools-3.5.0/acstools/tests/
--rw-r--r--   0 runner    (1001) docker     (122)       44 2022-12-06 20:22:32.000000 acstools-3.5.0/acstools/tests/.gitattributes
--rw-r--r--   0 runner    (1001) docker     (122)       31 2022-12-06 20:22:32.000000 acstools-3.5.0/acstools/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 20:23:13.168244 acstools-3.5.0/acstools/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 20:23:13.188244 acstools-3.5.0/acstools/tests/data/input/
--rw-r--r--   0 runner    (1001) docker     (122)      133 2022-12-06 20:22:32.000000 acstools-3.5.0/acstools/tests/data/input/ja0x03ojq_flt.fits
--rw-r--r--   0 runner    (1001) docker     (122)      134 2022-12-06 20:22:32.000000 acstools-3.5.0/acstools/tests/data/input/jb5g05ubq_flt.fits
--rw-r--r--   0 runner    (1001) docker     (122)      134 2022-12-06 20:22:32.000000 acstools-3.5.0/acstools/tests/data/input/jc2z03cvq_blv_tmp.fits
--rw-r--r--   0 runner    (1001) docker     (122)      133 2022-12-06 20:22:32.000000 acstools-3.5.0/acstools/tests/data/input/jc5001soq_flt.fits
--rw-r--r--   0 runner    (1001) docker     (122)      134 2022-12-06 20:22:32.000000 acstools-3.5.0/acstools/tests/data/input/jc8m10syq_flc.fits
--rw-r--r--   0 runner    (1001) docker     (122)      134 2022-12-06 20:22:32.000000 acstools-3.5.0/acstools/tests/data/input/jc8o04ghq_flt.fits
--rw-r--r--   0 runner    (1001) docker     (122)      133 2022-12-06 20:22:32.000000 acstools-3.5.0/acstools/tests/data/input/jc8o04ghq_mask1.fits
--rw-r--r--   0 runner    (1001) docker     (122)      133 2022-12-06 20:22:32.000000 acstools-3.5.0/acstools/tests/data/input/jc8o04ghq_mask2.fits
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 20:23:13.192243 acstools-3.5.0/acstools/tests/data/truth/
--rw-r--r--   0 runner    (1001) docker     (122)      133 2022-12-06 20:22:32.000000 acstools-3.5.0/acstools/tests/data/truth/ja0x03ojq_flt_ref.fits
--rw-r--r--   0 runner    (1001) docker     (122)      134 2022-12-06 20:22:32.000000 acstools-3.5.0/acstools/tests/data/truth/jb5g05ubq_flt_ref.fits
--rw-r--r--   0 runner    (1001) docker     (122)      134 2022-12-06 20:22:32.000000 acstools-3.5.0/acstools/tests/data/truth/jc2z03cvq_blv_tmp_ref.fits
--rw-r--r--   0 runner    (1001) docker     (122)      133 2022-12-06 20:22:32.000000 acstools-3.5.0/acstools/tests/data/truth/jc5001soq_flt_ref.fits
--rw-r--r--   0 runner    (1001) docker     (122)      134 2022-12-06 20:22:32.000000 acstools-3.5.0/acstools/tests/data/truth/jc8m10syq_flc_ref.fits
--rw-r--r--   0 runner    (1001) docker     (122)      134 2022-12-06 20:22:32.000000 acstools-3.5.0/acstools/tests/data/truth/jc8o04ghq_flt_ref.fits
--rw-r--r--   0 runner    (1001) docker     (122)     6444 2022-12-06 20:22:32.000000 acstools-3.5.0/acstools/tests/helpers.py
--rw-r--r--   0 runner    (1001) docker     (122)     1875 2022-12-06 20:22:32.000000 acstools-3.5.0/acstools/tests/test_polarization.py
--rw-r--r--   0 runner    (1001) docker     (122)     2604 2022-12-06 20:22:32.000000 acstools-3.5.0/acstools/tests/test_wfc_destripe.py
--rw-r--r--   0 runner    (1001) docker     (122)      950 2022-12-06 20:22:32.000000 acstools-3.5.0/acstools/tests/test_wfc_satdet.py
--rw-r--r--   0 runner    (1001) docker     (122)    16780 2022-12-06 20:22:32.000000 acstools-3.5.0/acstools/utils_calib.py
--rw-r--r--   0 runner    (1001) docker     (122)      176 2022-12-06 20:22:42.000000 acstools-3.5.0/acstools/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 20:23:13.184244 acstools-3.5.0/acstools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1235 2022-12-06 20:22:42.000000 acstools-3.5.0/acstools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2302 2022-12-06 20:23:13.000000 acstools-3.5.0/acstools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-06 20:22:42.000000 acstools-3.5.0/acstools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      112 2022-12-06 20:22:42.000000 acstools-3.5.0/acstools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-06 20:22:42.000000 acstools-3.5.0/acstools.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      209 2022-12-06 20:22:42.000000 acstools-3.5.0/acstools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2022-12-06 20:22:42.000000 acstools-3.5.0/acstools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      823 2022-12-06 20:22:32.000000 acstools-3.5.0/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 20:23:13.192243 acstools-3.5.0/doc/
--rw-r--r--   0 runner    (1001) docker     (122)     3137 2022-12-06 20:22:32.000000 acstools-3.5.0/doc/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)     3079 2022-12-06 20:22:32.000000 acstools-3.5.0/doc/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 20:23:13.196243 acstools-3.5.0/doc/source/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 20:23:13.196243 acstools-3.5.0/doc/source/_static/
--rw-r--r--   0 runner    (1001) docker     (122)    65413 2022-12-06 20:22:32.000000 acstools-3.5.0/doc/source/_static/stsci_pri_combo_mark_white.png
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 20:23:13.196243 acstools-3.5.0/doc/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-06 20:22:32.000000 acstools-3.5.0/doc/source/_templates/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)      375 2022-12-06 20:22:32.000000 acstools-3.5.0/doc/source/acs_destripe.rst
--rw-r--r--   0 runner    (1001) docker     (122)      143 2022-12-06 20:22:32.000000 acstools-3.5.0/doc/source/acsphotcte.rst
--rw-r--r--   0 runner    (1001) docker     (122)      157 2022-12-06 20:22:32.000000 acstools-3.5.0/doc/source/acszpt.rst
--rw-r--r--   0 runner    (1001) docker     (122)     9803 2022-12-06 20:22:32.000000 acstools-3.5.0/doc/source/calacs.rst
--rw-r--r--   0 runner    (1001) docker     (122)     7379 2022-12-06 20:22:32.000000 acstools-3.5.0/doc/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)      996 2022-12-06 20:22:32.000000 acstools-3.5.0/doc/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)      160 2022-12-06 20:22:32.000000 acstools-3.5.0/doc/source/polarization_tools.rst
--rw-r--r--   0 runner    (1001) docker     (122)      173 2022-12-06 20:22:32.000000 acstools-3.5.0/doc/source/satdet.rst
--rw-r--r--   0 runner    (1001) docker     (122)      150 2022-12-06 20:22:32.000000 acstools-3.5.0/doc/source/utils_calib.rst
--rw-r--r--   0 runner    (1001) docker     (122)      140 2022-12-06 20:22:32.000000 acstools-3.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)     2265 2022-12-06 20:23:13.196243 acstools-3.5.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)      800 2022-12-06 20:22:32.000000 acstools-3.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:39:46.274543 acstools-3.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-08 21:39:07.000000 acstools-3.6.0/.bandit.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:39:46.254543 acstools-3.6.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:39:46.254543 acstools-3.6.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-05-08 21:39:07.000000 acstools-3.6.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-08 21:39:07.000000 acstools-3.6.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-08 21:39:07.000000 acstools-3.6.0/.github/ISSUE_TEMPLATE/question.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-05-08 21:39:07.000000 acstools-3.6.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-08 21:39:07.000000 acstools-3.6.0/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-08 21:39:07.000000 acstools-3.6.0/.github/labeler.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:39:46.254543 acstools-3.6.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-05-08 21:39:07.000000 acstools-3.6.0/.github/workflows/ci_workflows.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-05-08 21:39:07.000000 acstools-3.6.0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-05-08 21:39:07.000000 acstools-3.6.0/.github/workflows/open_actions.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-08 21:39:07.000000 acstools-3.6.0/.github/workflows/predeps_workflows.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-08 21:39:07.000000 acstools-3.6.0/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-08 21:39:07.000000 acstools-3.6.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-08 21:39:07.000000 acstools-3.6.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-08 21:39:07.000000 acstools-3.6.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-08 21:39:07.000000 acstools-3.6.0/CITATION.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-05-08 21:39:07.000000 acstools-3.6.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-05-08 21:39:07.000000 acstools-3.6.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-08 21:39:07.000000 acstools-3.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-05-08 21:39:46.274543 acstools-3.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-08 21:39:07.000000 acstools-3.6.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:39:46.262543 acstools-3.6.0/acstools/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-08 21:39:07.000000 acstools-3.6.0/acstools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-05-08 21:39:07.000000 acstools-3.6.0/acstools/acs2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38670 2023-05-08 21:39:07.000000 acstools-3.6.0/acstools/acs_destripe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26899 2023-05-08 21:39:07.000000 acstools-3.6.0/acstools/acs_destripe_plus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-05-08 21:39:07.000000 acstools-3.6.0/acstools/acsccd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-05-08 21:39:07.000000 acstools-3.6.0/acstools/acscte.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-05-08 21:39:07.000000 acstools-3.6.0/acstools/acscteforwardmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10631 2023-05-08 21:39:07.000000 acstools-3.6.0/acstools/acsphotcte.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5738 2023-05-08 21:39:07.000000 acstools-3.6.0/acstools/acsrej.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-05-08 21:39:07.000000 acstools-3.6.0/acstools/acssum.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13247 2023-05-08 21:39:07.000000 acstools-3.6.0/acstools/acszpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-05-08 21:39:07.000000 acstools-3.6.0/acstools/calacs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:39:46.262543 acstools-3.6.0/acstools/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-05-08 21:39:07.000000 acstools-3.6.0/acstools/data/polarizer_tables.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-05-08 21:39:07.000000 acstools-3.6.0/acstools/data/rt_line_kernel_width15.fits
+-rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-05-08 21:39:07.000000 acstools-3.6.0/acstools/data/rt_line_kernel_width3.fits
+-rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-05-08 21:39:07.000000 acstools-3.6.0/acstools/data/rt_line_kernel_width7.fits
+-rw-r--r--   0 runner    (1001) docker     (123)    52685 2023-05-08 21:39:07.000000 acstools-3.6.0/acstools/findsat_mrt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16594 2023-05-08 21:39:07.000000 acstools-3.6.0/acstools/polarization_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35084 2023-05-08 21:39:07.000000 acstools-3.6.0/acstools/satdet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:39:46.266543 acstools-3.6.0/acstools/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-08 21:39:07.000000 acstools-3.6.0/acstools/tests/.gitattributes
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-08 21:39:07.000000 acstools-3.6.0/acstools/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:39:46.246543 acstools-3.6.0/acstools/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:39:46.266543 acstools-3.6.0/acstools/tests/data/input/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-08 21:39:07.000000 acstools-3.6.0/acstools/tests/data/input/ja0x03ojq_flt.fits
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-08 21:39:07.000000 acstools-3.6.0/acstools/tests/data/input/jb5g05ubq_flt.fits
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-08 21:39:07.000000 acstools-3.6.0/acstools/tests/data/input/jc2z03cvq_blv_tmp.fits
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-08 21:39:07.000000 acstools-3.6.0/acstools/tests/data/input/jc5001soq_flt.fits
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-08 21:39:07.000000 acstools-3.6.0/acstools/tests/data/input/jc8m10syq_flc.fits
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-08 21:39:07.000000 acstools-3.6.0/acstools/tests/data/input/jc8m32j5q_flc.fits
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-08 21:39:07.000000 acstools-3.6.0/acstools/tests/data/input/jc8o04ghq_flt.fits
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-08 21:39:07.000000 acstools-3.6.0/acstools/tests/data/input/jc8o04ghq_mask1.fits
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-08 21:39:07.000000 acstools-3.6.0/acstools/tests/data/input/jc8o04ghq_mask2.fits
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:39:46.270543 acstools-3.6.0/acstools/tests/data/truth/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-08 21:39:07.000000 acstools-3.6.0/acstools/tests/data/truth/ja0x03ojq_flt_ref.fits
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-08 21:39:07.000000 acstools-3.6.0/acstools/tests/data/truth/jb5g05ubq_flt_ref.fits
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-08 21:39:07.000000 acstools-3.6.0/acstools/tests/data/truth/jc2z03cvq_blv_tmp_ref.fits
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-08 21:39:07.000000 acstools-3.6.0/acstools/tests/data/truth/jc5001soq_flt_ref.fits
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-08 21:39:07.000000 acstools-3.6.0/acstools/tests/data/truth/jc8m10syq_flc_ref.fits
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-08 21:39:07.000000 acstools-3.6.0/acstools/tests/data/truth/jc8m32j5q_flc_mask_ref.fits
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-08 21:39:07.000000 acstools-3.6.0/acstools/tests/data/truth/jc8o04ghq_flt_ref.fits
+-rw-r--r--   0 runner    (1001) docker     (123)     6444 2023-05-08 21:39:07.000000 acstools-3.6.0/acstools/tests/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-05-08 21:39:07.000000 acstools-3.6.0/acstools/tests/test_polarization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-05-08 21:39:07.000000 acstools-3.6.0/acstools/tests/test_wfc_destripe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-08 21:39:07.000000 acstools-3.6.0/acstools/tests/test_wfc_findsat_mrt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-08 21:39:07.000000 acstools-3.6.0/acstools/tests/test_wfc_satdet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16780 2023-05-08 21:39:07.000000 acstools-3.6.0/acstools/utils_calib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48734 2023-05-08 21:39:07.000000 acstools-3.6.0/acstools/utils_findsat_mrt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-08 21:39:17.000000 acstools-3.6.0/acstools/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:39:46.262543 acstools-3.6.0/acstools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-05-08 21:39:17.000000 acstools-3.6.0/acstools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-05-08 21:39:46.000000 acstools-3.6.0/acstools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 21:39:17.000000 acstools-3.6.0/acstools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-08 21:39:17.000000 acstools-3.6.0/acstools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 21:39:17.000000 acstools-3.6.0/acstools.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-08 21:39:17.000000 acstools-3.6.0/acstools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-08 21:39:17.000000 acstools-3.6.0/acstools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-05-08 21:39:07.000000 acstools-3.6.0/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:39:46.270543 acstools-3.6.0/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-05-08 21:39:07.000000 acstools-3.6.0/doc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-05-08 21:39:07.000000 acstools-3.6.0/doc/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:39:46.274543 acstools-3.6.0/doc/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:39:46.274543 acstools-3.6.0/doc/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    65413 2023-05-08 21:39:07.000000 acstools-3.6.0/doc/source/_static/stsci_pri_combo_mark_white.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:39:46.274543 acstools-3.6.0/doc/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 21:39:07.000000 acstools-3.6.0/doc/source/_templates/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-08 21:39:07.000000 acstools-3.6.0/doc/source/acs_destripe.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-08 21:39:07.000000 acstools-3.6.0/doc/source/acsphotcte.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-08 21:39:07.000000 acstools-3.6.0/doc/source/acszpt.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9803 2023-05-08 21:39:07.000000 acstools-3.6.0/doc/source/calacs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7380 2023-05-08 21:39:07.000000 acstools-3.6.0/doc/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-08 21:39:07.000000 acstools-3.6.0/doc/source/findsat_mrt.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-08 21:39:07.000000 acstools-3.6.0/doc/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-08 21:39:07.000000 acstools-3.6.0/doc/source/polarization_tools.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-08 21:39:07.000000 acstools-3.6.0/doc/source/satdet.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-08 21:39:07.000000 acstools-3.6.0/doc/source/utils_calib.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-08 21:39:07.000000 acstools-3.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-05-08 21:39:46.274543 acstools-3.6.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      800 2023-05-08 21:39:07.000000 acstools-3.6.0/setup.py
```

### Comparing `acstools-3.5.0/.github/ISSUE_TEMPLATE/bug_report.md` & `acstools-3.6.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `acstools-3.5.0/.github/ISSUE_TEMPLATE/feature_request.md` & `acstools-3.6.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `acstools-3.5.0/.github/ISSUE_TEMPLATE/question.md` & `acstools-3.6.0/.github/ISSUE_TEMPLATE/question.md`

 * *Files identical despite different names*

### Comparing `acstools-3.5.0/.github/PULL_REQUEST_TEMPLATE.md` & `acstools-3.6.0/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `acstools-3.5.0/.github/labeler.yml` & `acstools-3.6.0/.github/labeler.yml`

 * *Files identical despite different names*

### Comparing `acstools-3.5.0/.github/workflows/ci_workflows.yml` & `acstools-3.6.0/.github/workflows/ci_workflows.yml`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,17 @@
     # * is a special character in YAML so you have to quote this string
     - cron: '0 6 * * 2'
 
 concurrency:
   group: ${{ github.workflow }}-${{ github.ref }}
   cancel-in-progress: true
 
+permissions:
+  contents: read
+
 env:
   jref: "https://ssb.stsci.edu/trds_open/jref"
 
 jobs:
   initial_checks:
     name: Mandatory checks before CI
     runs-on: ubuntu-latest
@@ -40,15 +43,15 @@
     needs: initial_checks
     steps:
     - name: Checkout code
       uses: actions/checkout@v3
       with:
         fetch-depth: 0
     - name: Set up Python
-      uses: actions/setup-python@v3
+      uses: actions/setup-python@v4
       with:
         python-version: '3.x'
     - name: Lint with flake8
       run: |
         python -m pip install --upgrade pip flake8
         flake8 acstools --count
     # Make sure that packaging will work
@@ -68,17 +71,17 @@
     steps:
     - name: Checkout code
       uses: actions/checkout@v3
       with:
         fetch-depth: 0
         lfs: true
     - name: Set up Python
-      uses: actions/setup-python@v3
+      uses: actions/setup-python@v4
       with:
-        python-version: '3.8'
+        python-version: '3.9'
     - name: Install and build
       run: |
         python -m pip install --upgrade pip setuptools wheel
         pip install git+https://github.com/spacetelescope/ci_watson.git --upgrade --no-deps
         python -m pip install -e .[test,all]
     - name: Test
       run: pytest --remote-data -v
@@ -89,17 +92,17 @@
     steps:
     - name: Checkout code
       uses: actions/checkout@v3
       with:
         fetch-depth: 0
         lfs: true
     - name: Set up Python
-      uses: actions/setup-python@v3
+      uses: actions/setup-python@v4
       with:
-        python-version: '3.10'
+        python-version: '3.11'
     - name: Install and build
       run: |
         python -m pip install --upgrade pip setuptools wheel
         pip install git+https://github.com/astropy/astropy.git#egg=astropy --upgrade --no-deps
         pip install git+https://github.com/spacetelescope/ci_watson.git --upgrade --no-deps
         python -m pip install -e .[test,all]
     - name: Test
@@ -108,15 +111,15 @@
   link_check:
     runs-on: ubuntu-latest
     needs: initial_checks
     steps:
     - name: Checkout code
       uses: actions/checkout@v3
     - name: Set up Python
-      uses: actions/setup-python@v3
+      uses: actions/setup-python@v4
       with:
         python-version: '3.x'
     - name: Install and build
       run: |
         python -m pip install --upgrade pip setuptools wheel
         python -m pip install -e .[docs]
     - name: Docs link check
```

### Comparing `acstools-3.5.0/.github/workflows/codeql-analysis.yml` & `acstools-3.6.0/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `acstools-3.5.0/.github/workflows/open_actions.yml` & `acstools-3.6.0/.github/workflows/open_actions.yml`

 * *Files identical despite different names*

### Comparing `acstools-3.5.0/.github/workflows/publish-to-pypi.yml` & `acstools-3.6.0/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `acstools-3.5.0/CODE_OF_CONDUCT.md` & `acstools-3.6.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `acstools-3.5.0/LICENSE.md` & `acstools-3.6.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `acstools-3.5.0/PKG-INFO` & `acstools-3.6.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: acstools
-Version: 3.5.0
+Version: 3.6.0
 Summary: Python Tools for HST ACS
 Home-page: https://github.com/spacetelescope/acstools
-Author: Matt Davis, Warren Hack, Norman Grogin, Pey Lian Lim, Sara Ogaz, Leonardo Ubeda, Mihai Cara, David Borncamp, Nathan Miles, Tyler Desjardins, Jenna Ryon
+Author: Matt Davis, Warren Hack, Norman Grogin, Pey Lian Lim, Sara Ogaz, Leonardo Ubeda, Mihai Cara, David Borncamp, Nathan Miles, Tyler Desjardins, Jenna Ryon, David Stark
 Author-email: help@stsci.edu
 License: BSD
 Project-URL: Bug Reports, https://github.com/spacetelescope/acstools/issues/
 Project-URL: Source, https://github.com/spacetelescope/acstools/
 Project-URL: Help, https://hsthelp.stsci.edu
 Keywords: astronomy,astrophysics,calibration
 Classifier: Intended Audience :: Science/Research
```

### Comparing `acstools-3.5.0/README.rst` & `acstools-3.6.0/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,26 @@
 ACSTOOLS
 ========
 
 .. image:: https://img.shields.io/badge/ascl-2011.024-blue.svg?colorB=262255
     :target: https://ascl.net/2011.024
     :alt: ascl:2011.024
 
-.. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.3728240.svg
-   :alt: zenodo.3728240
-   :target: https://doi.org/10.5281/zenodo.3728240
-
 .. image:: https://readthedocs.org/projects/acstools/badge/?version=latest
     :alt: Documentation Status
     :target: https://acstools.readthedocs.io/en/latest/?badge=latest
 
 .. image:: https://github.com/spacetelescope/acstools/workflows/CI/badge.svg
     :target: https://github.com/spacetelescope/acstools/actions?query=workflow%3ACI
     :alt: Github Actions CI Status
+
+For v3.5 or later:
+
+.. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.7406933.svg
+   :alt: zenodo.7406933
+   :target: https://doi.org/10.5281/zenodo.7406933
+
+For older versions:
+
+.. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.3728240.svg
+   :alt: zenodo.3728240
+   :target: https://doi.org/10.5281/zenodo.3728240
```

### Comparing `acstools-3.5.0/acstools/__init__.py` & `acstools-3.6.0/acstools/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,7 +15,9 @@
 from . import acs2d  # noqa
 from . import acsrej  # noqa
 from . import acssum  # noqa
 from . import acszpt  # noqa
 from . import acsphotcte  # noqa
 from . import satdet  # noqa
 from . import utils_calib  # noqa
+from . import findsat_mrt  # noqa
+from . import utils_findsat_mrt  # noqa
```

### Comparing `acstools-3.5.0/acstools/acs2d.py` & `acstools-3.6.0/acstools/acs2d.py`

 * *Files identical despite different names*

### Comparing `acstools-3.5.0/acstools/acs_destripe.py` & `acstools-3.6.0/acstools/acs_destripe.py`

 * *Files identical despite different names*

### Comparing `acstools-3.5.0/acstools/acs_destripe_plus.py` & `acstools-3.6.0/acstools/acs_destripe_plus.py`

 * *Files identical despite different names*

### Comparing `acstools-3.5.0/acstools/acsccd.py` & `acstools-3.6.0/acstools/acsccd.py`

 * *Files identical despite different names*

### Comparing `acstools-3.5.0/acstools/acscte.py` & `acstools-3.6.0/acstools/acscte.py`

 * *Files identical despite different names*

### Comparing `acstools-3.5.0/acstools/acscteforwardmodel.py` & `acstools-3.6.0/acstools/acscteforwardmodel.py`

 * *Files identical despite different names*

### Comparing `acstools-3.5.0/acstools/acsphotcte.py` & `acstools-3.6.0/acstools/acsphotcte.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 """
 The ACS Photometric CTE API is a programmatic interface for the
 `ACS Photometric CTE Webtool <https://acsphotometriccte.stsci.edu>`_.
 The API is a cloud-based service that employs a serverless approach on AWS
 with API Gateway and Lambda to compute the photometric CTE corrections
-using the model described in `ACS ISR 2012-05 <https://ui.adsabs.harvard.edu/abs/2012acs..rept....5C/abstract>`_.
+using the model described in `ACS ISR 2022-06 <https://ui.adsabs.harvard.edu/abs/2022acs..rept....6C/abstract>`_.
 The model corrects ACS/WFC aperture photometry extracted from FLT images for
 CTE losses. It is only calibrated for photometry obtained after SM4 in May
 2009. For pre-SM4 data, please see `ACS ISR 2009-01 <https://ui.adsabs.harvard.edu/abs/2009acs..rept....1C/abstract>`_, or use
 pixel-based CTE-corrected files obtained from MAST. Currently, only 3 and 5
 pixel aperture radii are supported. The model is designed to compute the
 CTE losses as a function of the number of Y transfers, sky background,
 source flux, and observation date.
@@ -134,15 +134,16 @@
         content :
             Body of the response object
         """
 
         response = requests.post(
             self._api_url,
             data=json.dumps(data),
-            headers=self._api_credentials
+            headers=self._api_credentials,
+            timeout=100
         )
 
         status_code = response.status_code
         content = json.loads(response.content)
         if status_code > 400:
             content = (f"Status Code: {status_code}\n"
                        f"Message: {content['message']}")
```

### Comparing `acstools-3.5.0/acstools/acsrej.py` & `acstools-3.6.0/acstools/acsrej.py`

 * *Files identical despite different names*

### Comparing `acstools-3.5.0/acstools/acssum.py` & `acstools-3.6.0/acstools/acssum.py`

 * *Files identical despite different names*

### Comparing `acstools-3.5.0/acstools/acszpt.py` & `acstools-3.6.0/acstools/acszpt.py`

 * *Files 0% similar despite different names*

```diff
@@ -296,15 +296,15 @@
                 body = '{"date": "%s", "detector": "%s", "filter": "%s"}' % (self.date, self.detector, self.filt)
 
             # send request to APIGateway with try/except clauses
             help_desk_string = ("\nIf this error persists, please contact the HST Help Desk at \n"
                                 "https://stsci.service-now.com/hst")
 
             try:
-                response = requests.post(invokeURL, data=body)
+                response = requests.post(invokeURL, data=body, timeout=100)
 
             except requests.exceptions.HTTPError:
                 raise ACSZeropointQueryError(f"HTTP Error to AWS API Gateway:{help_desk_string}") from None
 
             except requests.exceptions.ConnectionError:
                 raise ACSZeropointQueryError(f"Error Connecting to AWS API Gateway:{help_desk_string}") from None
```

### Comparing `acstools-3.5.0/acstools/calacs.py` & `acstools-3.6.0/acstools/calacs.py`

 * *Files identical despite different names*

### Comparing `acstools-3.5.0/acstools/data/polarizer_tables.yaml` & `acstools-3.6.0/acstools/data/polarizer_tables.yaml`

 * *Files identical despite different names*

### Comparing `acstools-3.5.0/acstools/polarization_tools.py` & `acstools-3.6.0/acstools/polarization_tools.py`

 * *Files identical despite different names*

### Comparing `acstools-3.5.0/acstools/satdet.py` & `acstools-3.6.0/acstools/satdet.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,16 @@
     not matter since :func:`detsat` only provides crude
     approximation of the actual trail(s).
 
     Performance is faster when ``plot=False``, where applicable.
 
 Examples
 --------
->>> from acstools.satdet import detsat, make_mask, update_dq
+>>> from acstools.satdet import detsat, make_mask
+>>> from acstools.utils_findsat_mrt import update_dq
 
 Find trail segments for a single image and extension without multiprocessing,
 and display plots (not shown) and verbose information:
 
 >>> results, errors = detsat(
 ...     'jc8m10syq_flc.fits', chips=[4], n_processes=1,
 ...     plot=True, verbose=True)
@@ -168,15 +169,15 @@
     plt = None
     warnings.warn('matplotlib not found, plotting is disabled',
                   AstropyUserWarning)
 
 __version__ = '0.3.3'
 __vdate__ = '11-Jul-2017'
 __author__ = 'David Borncamp, Pey Lian Lim'
-__all__ = ['detsat', 'make_mask', 'update_dq']
+__all__ = ['detsat', 'make_mask']
 
 
 def _detsat_one(filename, ext, sigma=2.0, low_thresh=0.1, h_thresh=0.5,
                 small_edge=60, line_len=200, line_gap=75,
                 percentile=(4.5, 93.0), buf=200, plot=False, verbose=False):
     """Called by :func:`detsat`."""
     if verbose:
@@ -525,15 +526,16 @@
 
     return (newx, newy)
 
 
 def make_mask(filename, ext, trail_coords, sublen=75, subwidth=200, order=3,
               sigma=4, pad=10, plot=False, verbose=False):
     """Create DQ mask for an image for a given satellite trail.
-    This mask can be added to existing DQ data using :func:`update_dq`.
+    This mask can be added to existing DQ data using
+    :func:`acstools.utils_findsat_mrt.update_dq`.
 
     .. note::
 
         Unlike :func:`detsat`, multiprocessing is not available for
         this function.
 
     Parameters
@@ -863,66 +865,14 @@
     if verbose:
         t_end = time.time()
         print(f'Run time: {t_end - t_beg} s')
 
     return mask
 
 
-def update_dq(filename, ext, mask, dqval=16384, verbose=True):
-    """Update the given image and DQ extension with the given
-    satellite trails mask and flag.
-
-    Parameters
-    ----------
-    filename : str
-        FITS image filename to update.
-
-    ext : int, str, or tuple
-        DQ extension, as accepted by ``astropy.io.fits``, to update.
-
-    mask : ndarray
-        Boolean mask, with `True` marking the satellite trail(s).
-        This can be the result(s) from :func:`make_mask`.
-
-    dqval : int, optional
-        DQ value to use for the trail. Default value of 16384 is
-        tailored for ACS/WFC.
-
-    verbose : bool, optional
-        Print extra information to the terminal.
-
-    """
-    with fits.open(filename, mode='update') as pf:
-        dqarr = pf[ext].data
-        old_mask = (dqval & dqarr) != 0  # Existing flagged trails
-        new_mask = mask & ~old_mask  # Only flag previously unflagged trails
-        npix_updated = np.count_nonzero(new_mask)
-
-        # Update DQ extension only if necessary
-        if npix_updated > 0:
-            pf[ext].data[new_mask] += dqval
-            pf['PRIMARY'].header.add_history(
-                f'{time.ctime()} satdet v{__version__}({__vdate__})')
-            pf['PRIMARY'].header.add_history(
-                f'  Updated {npix_updated} px in EXT {ext} with DQ={dqval}')
-
-    if verbose:
-        fname = f'{filename}[{ext}]'
-
-        print(f'DQ flag value is {dqval}\n'
-              f'Input... flagged NPIX={np.count_nonzero(mask)}\n'
-              f'Existing flagged NPIX={np.count_nonzero(old_mask)}\n'
-              f'Newly... flagged NPIX={npix_updated}')
-
-        if npix_updated > 0:
-            print(f'{fname} updated')
-        else:
-            print(f'No updates necessary for {fname}')
-
-
 # ############################ from decttest.py ############################# #
 # Multiprocessing for multiple input files.
 # This is for detection only, not for mask.
 
 def _satdet_worker(work_queue, done_queue, sigma=2.0, low_thresh=0.1,
                    h_thresh=0.5, small_edge=60, line_len=200, line_gap=75,
                    percentile=(4.5, 93.0), buf=200):
```

### Comparing `acstools-3.5.0/acstools/tests/helpers.py` & `acstools-3.6.0/acstools/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `acstools-3.5.0/acstools/tests/test_polarization.py` & `acstools-3.6.0/acstools/tests/test_polarization.py`

 * *Files identical despite different names*

### Comparing `acstools-3.5.0/acstools/tests/test_wfc_destripe.py` & `acstools-3.6.0/acstools/tests/test_wfc_destripe.py`

 * *Files identical despite different names*

### Comparing `acstools-3.5.0/acstools/tests/test_wfc_satdet.py` & `acstools-3.6.0/acstools/tests/test_wfc_satdet.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Test satellite trail detection.
 
 .. note:: Cannot test ``detsat()`` because PHT results change from run to run!
 
 """
 from acstools import satdet
+from acstools.utils_findsat_mrt import update_dq
 from acstools.tests.helpers import BaseACSTOOLS
 
 
 class TestSatDet(BaseACSTOOLS):
     detector = 'wfc'
 
     def test_trail_mask(self):
@@ -22,11 +23,11 @@
 
         # Satellite trail masking.
         sciext = 4
         dqext = 6
         trail = ((1199, 1357), (2841, 1023))
         mask = satdet.make_mask(inputfile, sciext, trail, plot=False,
                                 verbose=False)
-        satdet.update_dq(inputfile, dqext, mask, verbose=False)
+        update_dq(inputfile, dqext, mask, verbose=False)
 
         # Compare results.
         self.compare_outputs([(inputfile, truthfile)])
```

### Comparing `acstools-3.5.0/acstools/utils_calib.py` & `acstools-3.6.0/acstools/utils_calib.py`

 * *Files identical despite different names*

### Comparing `acstools-3.5.0/acstools.egg-info/PKG-INFO` & `acstools-3.6.0/acstools.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: acstools
-Version: 3.5.0
+Version: 3.6.0
 Summary: Python Tools for HST ACS
 Home-page: https://github.com/spacetelescope/acstools
-Author: Matt Davis, Warren Hack, Norman Grogin, Pey Lian Lim, Sara Ogaz, Leonardo Ubeda, Mihai Cara, David Borncamp, Nathan Miles, Tyler Desjardins, Jenna Ryon
+Author: Matt Davis, Warren Hack, Norman Grogin, Pey Lian Lim, Sara Ogaz, Leonardo Ubeda, Mihai Cara, David Borncamp, Nathan Miles, Tyler Desjardins, Jenna Ryon, David Stark
 Author-email: help@stsci.edu
 License: BSD
 Project-URL: Bug Reports, https://github.com/spacetelescope/acstools/issues/
 Project-URL: Source, https://github.com/spacetelescope/acstools/
 Project-URL: Help, https://hsthelp.stsci.edu
 Keywords: astronomy,astrophysics,calibration
 Classifier: Intended Audience :: Science/Research
```

### Comparing `acstools-3.5.0/acstools.egg-info/SOURCES.txt` & `acstools-3.6.0/acstools.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -16,65 +16,75 @@
 .github/labeler.yml
 .github/ISSUE_TEMPLATE/bug_report.md
 .github/ISSUE_TEMPLATE/feature_request.md
 .github/ISSUE_TEMPLATE/question.md
 .github/workflows/ci_workflows.yml
 .github/workflows/codeql-analysis.yml
 .github/workflows/open_actions.yml
+.github/workflows/predeps_workflows.yml
 .github/workflows/publish-to-pypi.yml
 acstools/__init__.py
 acstools/acs2d.py
 acstools/acs_destripe.py
 acstools/acs_destripe_plus.py
 acstools/acsccd.py
 acstools/acscte.py
 acstools/acscteforwardmodel.py
 acstools/acsphotcte.py
 acstools/acsrej.py
 acstools/acssum.py
 acstools/acszpt.py
 acstools/calacs.py
+acstools/findsat_mrt.py
 acstools/polarization_tools.py
 acstools/satdet.py
 acstools/utils_calib.py
+acstools/utils_findsat_mrt.py
 acstools/version.py
 acstools.egg-info/PKG-INFO
 acstools.egg-info/SOURCES.txt
 acstools.egg-info/dependency_links.txt
 acstools.egg-info/entry_points.txt
 acstools.egg-info/not-zip-safe
 acstools.egg-info/requires.txt
 acstools.egg-info/top_level.txt
 acstools/data/polarizer_tables.yaml
+acstools/data/rt_line_kernel_width15.fits
+acstools/data/rt_line_kernel_width3.fits
+acstools/data/rt_line_kernel_width7.fits
 acstools/tests/.gitattributes
 acstools/tests/__init__.py
 acstools/tests/helpers.py
 acstools/tests/test_polarization.py
 acstools/tests/test_wfc_destripe.py
+acstools/tests/test_wfc_findsat_mrt.py
 acstools/tests/test_wfc_satdet.py
 acstools/tests/data/input/ja0x03ojq_flt.fits
 acstools/tests/data/input/jb5g05ubq_flt.fits
 acstools/tests/data/input/jc2z03cvq_blv_tmp.fits
 acstools/tests/data/input/jc5001soq_flt.fits
 acstools/tests/data/input/jc8m10syq_flc.fits
+acstools/tests/data/input/jc8m32j5q_flc.fits
 acstools/tests/data/input/jc8o04ghq_flt.fits
 acstools/tests/data/input/jc8o04ghq_mask1.fits
 acstools/tests/data/input/jc8o04ghq_mask2.fits
 acstools/tests/data/truth/ja0x03ojq_flt_ref.fits
 acstools/tests/data/truth/jb5g05ubq_flt_ref.fits
 acstools/tests/data/truth/jc2z03cvq_blv_tmp_ref.fits
 acstools/tests/data/truth/jc5001soq_flt_ref.fits
 acstools/tests/data/truth/jc8m10syq_flc_ref.fits
+acstools/tests/data/truth/jc8m32j5q_flc_mask_ref.fits
 acstools/tests/data/truth/jc8o04ghq_flt_ref.fits
 doc/Makefile
 doc/make.bat
 doc/source/acs_destripe.rst
 doc/source/acsphotcte.rst
 doc/source/acszpt.rst
 doc/source/calacs.rst
 doc/source/conf.py
+doc/source/findsat_mrt.rst
 doc/source/index.rst
 doc/source/polarization_tools.rst
 doc/source/satdet.rst
 doc/source/utils_calib.rst
 doc/source/_static/stsci_pri_combo_mark_white.png
 doc/source/_templates/.gitignore
```

### Comparing `acstools-3.5.0/conftest.py` & `acstools-3.6.0/conftest.py`

 * *Files identical despite different names*

### Comparing `acstools-3.5.0/doc/Makefile` & `acstools-3.6.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `acstools-3.5.0/doc/make.bat` & `acstools-3.6.0/doc/make.bat`

 * *Files identical despite different names*

### Comparing `acstools-3.5.0/doc/source/_static/stsci_pri_combo_mark_white.png` & `acstools-3.6.0/doc/source/_static/stsci_pri_combo_mark_white.png`

 * *Files identical despite different names*

### Comparing `acstools-3.5.0/doc/source/calacs.rst` & `acstools-3.6.0/doc/source/calacs.rst`

 * *Files identical despite different names*

### Comparing `acstools-3.5.0/doc/source/conf.py` & `acstools-3.6.0/doc/source/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -199,20 +199,20 @@
 #latex_use_modindex = True
 
 # Configuration for intersphinx: refer to the Python standard library.
 intersphinx_mapping = {
     'python': ('https://docs.python.org/', None),
     'numpy': ('https://docs.scipy.org/doc/numpy/', None),
     'scipy': ('https://docs.scipy.org/doc/scipy/reference/', None),
-    'skimage': ('https://scikit-image.org/docs/0.11.x/', None),
+    'skimage': ('https://scikit-image.org/docs/stable/', None),
     'matplotlib': ('https://matplotlib.org/', None),
     'astropy': ('https://docs.astropy.org/en/stable/', None)
 }
 
 # -- Options for linkcheck output ---------------------------------------------
 linkcheck_retry = 5
 linkcheck_ignore = ['https://hsthelp.stsci.edu', 'https://acszeropoints.stsci.edu']
 linkcheck_timeout = 180
 linkcheck_anchors = False
 
 # Enable nitpicky mode - which ensures that all references in the docs resolve.
-nitpicky = False
+nitpicky = False
```

### Comparing `acstools-3.5.0/doc/source/index.rst` & `acstools-3.6.0/doc/source/index.rst`

 * *Files 6% similar despite different names*

```diff
@@ -36,14 +36,15 @@
    :maxdepth: 2
 
    calacs
    acs_destripe
    acszpt
    acsphotcte
    satdet
+   findsat_mrt
    polarization_tools
    utils_calib
 
 ******************
 Indices and tables
 ******************
```

### Comparing `acstools-3.5.0/setup.cfg` & `acstools-3.6.0/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [metadata]
 name = acstools
 description = Python Tools for HST ACS
 long_description = Python Tools for HST ACS (Advanced Camera for Surveys) Data
 long_description_content_type = text/plain
 keywords = astronomy, astrophysics, calibration
-author = Matt Davis, Warren Hack, Norman Grogin, Pey Lian Lim, Sara Ogaz, Leonardo Ubeda, Mihai Cara, David Borncamp, Nathan Miles, Tyler Desjardins, Jenna Ryon
+author = Matt Davis, Warren Hack, Norman Grogin, Pey Lian Lim, Sara Ogaz, Leonardo Ubeda, Mihai Cara, David Borncamp, Nathan Miles, Tyler Desjardins, Jenna Ryon, David Stark
 author_email = help@stsci.edu
 license = BSD
 license_file = LICENSE.md
 url = https://github.com/spacetelescope/acstools
 edit_on_github = False
 github_project = spacetelescope/acstools
 classifier = 
@@ -40,14 +40,15 @@
 [options.extras_require]
 all = 
 	matplotlib
 	scipy
 	scikit-image
 	stsci.tools
 	stsci.imagestats
+	photutils
 test = 
 	pytest
 	pytest-astropy-header
 	pytest-remotedata
 	ci-watson
 docs = 
 	sphinx-automodapi
@@ -73,14 +74,17 @@
 xfail_strict = true
 filterwarnings = 
 	error
 	ignore:numpy\.ndarray size changed:RuntimeWarning
 	ignore:unclosed file:ResourceWarning
 	ignore:distutils Version classes are deprecated:DeprecationWarning
 	ignore:Deprecation Warning.*timeout.*parameter no longer needed:UserWarning
+	ignore:.*np\.bool8.*is a deprecated alias:DeprecationWarning
+	ignore:Deprecated call to.*pkg_resources\.declare_namespace.*:DeprecationWarning
+	ignore:pkg_resources is deprecated as an API:DeprecationWarning
 
 [flake8]
 ignore = E221,E226,E262,E265,E501,E704,W504
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `acstools-3.5.0/setup.py` & `acstools-3.6.0/setup.py`

 * *Files identical despite different names*

