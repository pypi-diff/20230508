# Comparing `tmp/iga-0.0.8.tar.gz` & `tmp/iga-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iga-0.0.8.tar", last modified: Thu May  4 22:43:34 2023, max compression
+gzip compressed data, was "iga-0.0.9.tar", last modified: Mon May  8 19:00:54 2023, max compression
```

## Comparing `iga-0.0.8.tar` & `iga-0.0.9.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-05-04 22:43:34.066073 iga-0.0.8/
--rw-r--r--   0 mhucka     (503) staff       (20)     1527 2023-03-16 00:12:10.000000 iga-0.0.8/LICENSE
--rw-r--r--   0 mhucka     (503) staff       (20)    27417 2023-05-04 22:43:34.066186 iga-0.0.8/PKG-INFO
--rw-r--r--   0 mhucka     (503) staff       (20)    26511 2023-05-04 22:41:49.000000 iga-0.0.8/README.md
-drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-05-04 22:43:34.060634 iga-0.0.8/iga/
--rw-r--r--   0 mhucka     (503) staff       (20)     1458 2023-05-04 22:42:09.000000 iga-0.0.8/iga/__init__.py
--rw-r--r--   0 mhucka     (503) staff       (20)      905 2023-03-16 00:12:36.000000 iga-0.0.8/iga/__main__.py
--rw-r--r--   0 mhucka     (503) staff       (20)    32771 2023-05-04 22:41:49.000000 iga-0.0.8/iga/cli.py
--rw-r--r--   0 mhucka     (503) staff       (20)     3317 2023-03-27 20:05:34.000000 iga-0.0.8/iga/data_utils.py
--rw-r--r--   0 mhucka     (503) staff       (20)     2859 2023-04-10 21:11:51.000000 iga-0.0.8/iga/doi.py
--rw-r--r--   0 mhucka     (503) staff       (20)     1179 2023-04-25 22:30:46.000000 iga-0.0.8/iga/exceptions.py
--rw-r--r--   0 mhucka     (503) staff       (20)     1447 2023-03-28 00:40:16.000000 iga-0.0.8/iga/exit_codes.py
--rw-r--r--   0 mhucka     (503) staff       (20)    15031 2023-04-20 00:58:38.000000 iga-0.0.8/iga/github.py
--rw-r--r--   0 mhucka     (503) staff       (20)     4901 2023-04-26 04:08:12.000000 iga-0.0.8/iga/id_utils.py
--rw-r--r--   0 mhucka     (503) staff       (20)    16908 2023-04-25 22:30:46.000000 iga-0.0.8/iga/invenio.py
--rw-r--r--   0 mhucka     (503) staff       (20)     2058 2023-04-20 00:58:38.000000 iga-0.0.8/iga/json_utils.py
--rw-r--r--   0 mhucka     (503) staff       (20)   242887 2023-03-08 23:12:16.000000 iga-0.0.8/iga/licenses.py
--rw-r--r--   0 mhucka     (503) staff       (20)    69419 2023-05-04 22:41:49.000000 iga-0.0.8/iga/metadata.py
--rw-r--r--   0 mhucka     (503) staff       (20)    14563 2023-04-26 04:08:12.000000 iga-0.0.8/iga/name_utils.py
--rw-r--r--   0 mhucka     (503) staff       (20)     5273 2023-04-08 02:44:39.000000 iga-0.0.8/iga/orcid.py
--rw-r--r--   0 mhucka     (503) staff       (20)     5147 2023-04-08 02:44:39.000000 iga-0.0.8/iga/reference.py
--rw-r--r--   0 mhucka     (503) staff       (20)     3969 2023-04-08 02:44:39.000000 iga-0.0.8/iga/ror.py
--rw-r--r--   0 mhucka     (503) staff       (20)     1624 2023-04-08 02:44:39.000000 iga-0.0.8/iga/text_utils.py
-drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-05-04 22:43:34.063622 iga-0.0.8/iga.egg-info/
--rw-r--r--   0 mhucka     (503) staff       (20)    27417 2023-05-04 22:43:34.000000 iga-0.0.8/iga.egg-info/PKG-INFO
--rw-r--r--   0 mhucka     (503) staff       (20)      930 2023-05-04 22:43:34.000000 iga-0.0.8/iga.egg-info/SOURCES.txt
--rw-r--r--   0 mhucka     (503) staff       (20)        1 2023-05-04 22:43:34.000000 iga-0.0.8/iga.egg-info/dependency_links.txt
--rw-r--r--   0 mhucka     (503) staff       (20)       58 2023-05-04 22:43:34.000000 iga-0.0.8/iga.egg-info/entry_points.txt
--rw-r--r--   0 mhucka     (503) staff       (20)        1 2023-05-04 22:43:34.000000 iga-0.0.8/iga.egg-info/not-zip-safe
--rw-r--r--   0 mhucka     (503) staff       (20)      657 2023-05-04 22:43:34.000000 iga-0.0.8/iga.egg-info/requires.txt
--rw-r--r--   0 mhucka     (503) staff       (20)        4 2023-05-04 22:43:34.000000 iga-0.0.8/iga.egg-info/top_level.txt
--rw-r--r--   0 mhucka     (503) staff       (20)     1095 2023-05-04 22:43:34.066542 iga-0.0.8/setup.cfg
--rwxr-xr-x   0 mhucka     (503) staff       (20)     1708 2023-04-08 01:05:22.000000 iga-0.0.8/setup.py
-drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-05-04 22:43:34.065959 iga-0.0.8/tests/
--rw-r--r--   0 mhucka     (503) staff       (20)     5734 2023-04-25 22:30:46.000000 iga-0.0.8/tests/test_cli.py
--rw-r--r--   0 mhucka     (503) staff       (20)     4481 2023-03-27 19:38:15.000000 iga-0.0.8/tests/test_data_utils.py
--rw-r--r--   0 mhucka     (503) staff       (20)     1417 2023-03-17 23:21:28.000000 iga-0.0.8/tests/test_doi.py
--rw-r--r--   0 mhucka     (503) staff       (20)      686 2023-03-02 15:36:12.000000 iga-0.0.8/tests/test_exceptions.py
--rw-r--r--   0 mhucka     (503) staff       (20)      177 2023-01-13 03:19:50.000000 iga-0.0.8/tests/test_exit_codes.py
--rw-r--r--   0 mhucka     (503) staff       (20)     1446 2023-04-07 01:26:59.000000 iga-0.0.8/tests/test_github.py
--rw-r--r--   0 mhucka     (503) staff       (20)     3015 2023-04-07 01:20:36.000000 iga-0.0.8/tests/test_github_mocks.py
--rw-r--r--   0 mhucka     (503) staff       (20)     3666 2023-04-26 04:08:12.000000 iga-0.0.8/tests/test_id_utils.py
--rw-r--r--   0 mhucka     (503) staff       (20)      641 2022-12-08 00:11:08.000000 iga-0.0.8/tests/test_init.py
--rw-r--r--   0 mhucka     (503) staff       (20)    49214 2023-04-20 00:58:38.000000 iga-0.0.8/tests/test_is_person.py
--rw-r--r--   0 mhucka     (503) staff       (20)      912 2023-03-02 15:16:32.000000 iga-0.0.8/tests/test_licenses.py
--rw-r--r--   0 mhucka     (503) staff       (20)     4408 2023-04-20 00:58:38.000000 iga-0.0.8/tests/test_name_splitting.py
--rw-r--r--   0 mhucka     (503) staff       (20)     1829 2023-04-20 00:58:38.000000 iga-0.0.8/tests/test_name_utils.py
--rw-r--r--   0 mhucka     (503) staff       (20)     1054 2023-03-18 00:09:09.000000 iga-0.0.8/tests/test_orcid.py
--rw-r--r--   0 mhucka     (503) staff       (20)     1935 2023-04-08 01:31:14.000000 iga-0.0.8/tests/test_record_from_codemeta.py
--rw-r--r--   0 mhucka     (503) staff       (20)     6026 2023-03-02 23:04:18.000000 iga-0.0.8/tests/test_reference.py
--rw-r--r--   0 mhucka     (503) staff       (20)      947 2023-03-18 00:05:51.000000 iga-0.0.8/tests/test_ror.py
--rw-r--r--   0 mhucka     (503) staff       (20)     1375 2023-04-06 22:54:59.000000 iga-0.0.8/tests/test_text_utils.py
+drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-05-08 19:00:54.305955 iga-0.0.9/
+-rw-r--r--   0 mhucka     (503) staff       (20)     1527 2023-03-16 00:12:10.000000 iga-0.0.9/LICENSE
+-rw-r--r--   0 mhucka     (503) staff       (20)    29356 2023-05-08 19:00:54.306050 iga-0.0.9/PKG-INFO
+-rw-r--r--   0 mhucka     (503) staff       (20)    28450 2023-05-08 18:59:03.000000 iga-0.0.9/README.md
+drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-05-08 19:00:54.302799 iga-0.0.9/iga/
+-rw-r--r--   0 mhucka     (503) staff       (20)     1458 2023-05-08 19:00:02.000000 iga-0.0.9/iga/__init__.py
+-rw-r--r--   0 mhucka     (503) staff       (20)      905 2023-03-16 00:12:36.000000 iga-0.0.9/iga/__main__.py
+-rw-r--r--   0 mhucka     (503) staff       (20)    32900 2023-05-08 18:59:03.000000 iga-0.0.9/iga/cli.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     3317 2023-03-27 20:05:34.000000 iga-0.0.9/iga/data_utils.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     2859 2023-04-10 21:11:51.000000 iga-0.0.9/iga/doi.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1179 2023-04-25 22:30:46.000000 iga-0.0.9/iga/exceptions.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1447 2023-03-28 00:40:16.000000 iga-0.0.9/iga/exit_codes.py
+-rw-r--r--   0 mhucka     (503) staff       (20)    15031 2023-04-20 00:58:38.000000 iga-0.0.9/iga/github.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     4901 2023-04-26 04:08:12.000000 iga-0.0.9/iga/id_utils.py
+-rw-r--r--   0 mhucka     (503) staff       (20)    16908 2023-04-25 22:30:46.000000 iga-0.0.9/iga/invenio.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     2058 2023-04-20 00:58:38.000000 iga-0.0.9/iga/json_utils.py
+-rw-r--r--   0 mhucka     (503) staff       (20)   242887 2023-03-08 23:12:16.000000 iga-0.0.9/iga/licenses.py
+-rw-r--r--   0 mhucka     (503) staff       (20)    69659 2023-05-08 18:59:03.000000 iga-0.0.9/iga/metadata.py
+-rw-r--r--   0 mhucka     (503) staff       (20)    14563 2023-04-26 04:08:12.000000 iga-0.0.9/iga/name_utils.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     5273 2023-04-08 02:44:39.000000 iga-0.0.9/iga/orcid.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     5147 2023-04-08 02:44:39.000000 iga-0.0.9/iga/reference.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     3969 2023-04-08 02:44:39.000000 iga-0.0.9/iga/ror.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1624 2023-04-08 02:44:39.000000 iga-0.0.9/iga/text_utils.py
+drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-05-08 19:00:54.303680 iga-0.0.9/iga.egg-info/
+-rw-r--r--   0 mhucka     (503) staff       (20)    29356 2023-05-08 19:00:54.000000 iga-0.0.9/iga.egg-info/PKG-INFO
+-rw-r--r--   0 mhucka     (503) staff       (20)      930 2023-05-08 19:00:54.000000 iga-0.0.9/iga.egg-info/SOURCES.txt
+-rw-r--r--   0 mhucka     (503) staff       (20)        1 2023-05-08 19:00:54.000000 iga-0.0.9/iga.egg-info/dependency_links.txt
+-rw-r--r--   0 mhucka     (503) staff       (20)       58 2023-05-08 19:00:54.000000 iga-0.0.9/iga.egg-info/entry_points.txt
+-rw-r--r--   0 mhucka     (503) staff       (20)        1 2023-05-08 19:00:54.000000 iga-0.0.9/iga.egg-info/not-zip-safe
+-rw-r--r--   0 mhucka     (503) staff       (20)      657 2023-05-08 19:00:54.000000 iga-0.0.9/iga.egg-info/requires.txt
+-rw-r--r--   0 mhucka     (503) staff       (20)        4 2023-05-08 19:00:54.000000 iga-0.0.9/iga.egg-info/top_level.txt
+-rw-r--r--   0 mhucka     (503) staff       (20)     1095 2023-05-08 19:00:54.306393 iga-0.0.9/setup.cfg
+-rwxr-xr-x   0 mhucka     (503) staff       (20)     1708 2023-04-08 01:05:22.000000 iga-0.0.9/setup.py
+drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-05-08 19:00:54.305851 iga-0.0.9/tests/
+-rw-r--r--   0 mhucka     (503) staff       (20)     5734 2023-04-25 22:30:46.000000 iga-0.0.9/tests/test_cli.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     4481 2023-03-27 19:38:15.000000 iga-0.0.9/tests/test_data_utils.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1417 2023-03-17 23:21:28.000000 iga-0.0.9/tests/test_doi.py
+-rw-r--r--   0 mhucka     (503) staff       (20)      686 2023-03-02 15:36:12.000000 iga-0.0.9/tests/test_exceptions.py
+-rw-r--r--   0 mhucka     (503) staff       (20)      177 2023-01-13 03:19:50.000000 iga-0.0.9/tests/test_exit_codes.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1446 2023-04-07 01:26:59.000000 iga-0.0.9/tests/test_github.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     3015 2023-04-07 01:20:36.000000 iga-0.0.9/tests/test_github_mocks.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     3666 2023-04-26 04:08:12.000000 iga-0.0.9/tests/test_id_utils.py
+-rw-r--r--   0 mhucka     (503) staff       (20)      641 2022-12-08 00:11:08.000000 iga-0.0.9/tests/test_init.py
+-rw-r--r--   0 mhucka     (503) staff       (20)    49214 2023-04-20 00:58:38.000000 iga-0.0.9/tests/test_is_person.py
+-rw-r--r--   0 mhucka     (503) staff       (20)      912 2023-03-02 15:16:32.000000 iga-0.0.9/tests/test_licenses.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     4408 2023-04-20 00:58:38.000000 iga-0.0.9/tests/test_name_splitting.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1829 2023-04-20 00:58:38.000000 iga-0.0.9/tests/test_name_utils.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1054 2023-03-18 00:09:09.000000 iga-0.0.9/tests/test_orcid.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1935 2023-04-08 01:31:14.000000 iga-0.0.9/tests/test_record_from_codemeta.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     6026 2023-03-02 23:04:18.000000 iga-0.0.9/tests/test_reference.py
+-rw-r--r--   0 mhucka     (503) staff       (20)      947 2023-03-18 00:05:51.000000 iga-0.0.9/tests/test_ror.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1375 2023-04-06 22:54:59.000000 iga-0.0.9/tests/test_text_utils.py
```

### Comparing `iga-0.0.8/LICENSE` & `iga-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `iga-0.0.8/PKG-INFO` & `iga-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iga
-Version: 0.0.8
+Version: 0.0.9
 Summary: InvenioRDM GitHub Archiver
 Home-page: https://github.com/caltechlibrary/iga
 Author: Michael Hucka
 Author-email: helpdesk@library.caltech.edu
 License: https://github.com/caltechlibrary/iga/blob/main/LICENSE
 Project-URL: Source Code, https://github.com/caltechlibrary/iga
 Project-URL: Bug Tracker, https://github.com/caltechlibrary/iga/issues
@@ -32,70 +32,81 @@
 [![PyPI](https://img.shields.io/pypi/v/iga.svg?style=flat-square&color=orange&label=PyPI)](https://pypi.org/project/iga/)
 
 
 ## Table of contents
 
 * [Introduction](#introduction)
 * [Installation](#installation)
+* [Quick start](#quick-start)
 * [Usage](#usage)
 * [Known issues and limitations](#known-issues-and-limitations)
 * [Getting help](#getting-help)
 * [Contributing](#contributing)
 * [License](#license)
 * [Acknowledgments](#authors-and-acknowledgments)
 
 
 ## Introduction
 
-[InvenioRDM](https://inveniosoftware.org/products/rdm/) is a research data management (RDM) repository platform based on the [Invenio Framework](https://inveniosoftware.org/products/framework/) and [Zenodo](https://www.zenodo.org). At institutions like Caltech, InvenioRDM is used as the basis for institutional repositories such as [CaltechDATA](https://data.caltech.edu). Of particular interest to software developers is that a repository like [CaltechDATA](https://data.caltech.edu) offers the means to preserve software projects in a long-term archive managed by their institution.
+[InvenioRDM](https://inveniosoftware.org/products/rdm/) is the basis for many institutional repositories such as [CaltechDATA](https://data.caltech.edu) that enable users to preserve software and datasets in long-term archive. Though such repositories are critical resources, creating detailed records and uploading assets can be a tedious and error-prone process if done manually. This is where the InvenioRDM GitHub Archiver (IGA) comes in.
 
-The _InvenioRDM GitHub Archiver_ (IGA) is a tool for sending software releases from GitHub to an InvenioRDM-based repository server. IGA can be invoked from the command line; it also can be set up as a [GitHub Action](https://docs.github.com/en/actions) to automate the archiving of GitHub software releases in an InvenioRDM repository. Here are some of IGA's other notable features:
-* Automatic extraction of metadata from the GitHub release, the GitHub repository, and [`codemeta.json`](https://codemeta.github.io) and/or [`CITATION.cff`](https://citation-file-format.github.io) files if they exist in the repository
-* Thorough coverage of [InvenioRDM record metadata](https://inveniordm.docs.cern.ch/reference/metadata) using painstaking procedures
-* Automatic recognition of common identifier types that often appear CodeMeta and CFF files, such as [ORCID](https://orcid.org), [ROR](https://ror.org), [DOI](https://www.doi.org), [arXiV](https://arxiv.org), [PMCID/PMID](https://www.ncbi.nlm.nih.gov/pmc/about/public-access-info/), and others
-* Automatic lookup of human names in [ORCID.org](https://orcid.org) if needed (assuming ORCID id's are provided)
-* Automatic lookup of organization names in [ROR](https://ror.org) (assuming ROR id's are provided)
+IGA creates metadata records and sends releases from GitHub to an InvenioRDM-based repository server. IGA can be invoked from the command line; it also can be set up as a [GitHub Action](https://docs.github.com/en/actions) to archive GitHub releases automatically for a repository each time they are made.
+
+<p align=center>
+<img align="middle" src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/example-github-release.jpg" width="40%">
+<span style="font-size: 150%">➜</span>
+<img align="middle" src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/example-record-landing-page.jpg" width="40%">
+</p>
+
+IGA offers many notable features:
+* Automatic metadata extraction from GitHub releases plus [`codemeta.json`](https://codemeta.github.io) and [`CITATION.cff`](https://citation-file-format.github.io) files
+* Thorough coverage of [InvenioRDM record metadata fields](https://inveniordm.docs.cern.ch/reference/metadata) using painstaking procedures
+* Recognition of id's that appear in CodeMeta & CFF files: [ORCID](https://orcid.org), [ROR](https://ror.org), [DOI](https://www.doi.org), [arXiv](https://arxiv.org),  [PMCID](https://www.ncbi.nlm.nih.gov/pmc/about/public-access-info/), and more
 * Automatic lookup of publication data in [DOI.org](https://www.doi.org), [PubMed]((https://www.ncbi.nlm.nih.gov/pmc/about/public-access-info/)), Google Books, & other sources if needed
-* Automatic splitting of human names into family and given names using [ML](https://en.wikipedia.org/wiki/Machine_learning)-based methods, if necessary, to comply with InvenioRDM requirements
-* Support for overriding the metadata record it creates, for complete control if you need it
+* Automatic lookup of organization names in [ROR](https://ror.org) (assuming ROR id's are provided)
+* Automatic lookup of human names in [ORCID.org](https://orcid.org) if needed (assuming ORCID id's are provided)
+* Automatic splitting of human names into family and given names using [ML](https://en.wikipedia.org/wiki/Machine_learning)-based methods
 * Support for InvenioRDM [communities](https://invenio-communities.readthedocs.io/en/latest/)
-* Ability to use the GitHub API without a [GitHub access token](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token) in many cases
+* Support for overriding the metadata record that IGA creates, for complete control if you need it
+* Support for using the GitHub API without a [GitHub access token](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token) in simple cases
 * Extensive use of logging so you can see what's going on under the hood
 
 
 ## Installation
 
-(Note: at this time, only the command-line version of IGA is available.) There are multiple ways of installing IGA.  Please choose the alternative that suits you.
+### As a standalone command-line program
+
+There are multiple ways of installing IGA.  Please choose the alternative that suits you.
 
-### _Alternative 1: installing IGA using `pipx`_
+#### _Alternative 1: installing IGA using `pipx`_
 
 [Pipx](https://pypa.github.io/pipx/) lets you install Python programs in a way that isolates Python dependencies, and yet the resulting `iga` command can be run from any shell and directory &ndash; like any normal program on your computer. If you use `pipx` on your system, you can install IGA with the following command:
 ```sh
 pipx install iga
 ```
 
 Pipx can also let you run IGA directly using `pipx run iga`, although in that case, you must always prefix every IGA command with `pipx run`.  Consult the [documentation for `pipx run`](https://github.com/pypa/pipx#walkthrough-running-an-application-in-a-temporary-virtual-environment) for more information.
 
 
-### _Alternative 2: installing IGA using `pip`_
+#### _Alternative 2: installing IGA using `pip`_
 
 You should be able to install `iga` with [`pip`](https://pip.pypa.io/en/stable/installing/) for Python&nbsp;3.  To install `iga` from the [Python package repository (PyPI)](https://pypi.org), run the following command:
 ```sh
 python3 -m pip install iga
 ```
 
 As an alternative to getting it from [PyPI](https://pypi.org), you can use `pip` to install `iga` directly from GitHub:
 ```sh
 python3 -m pip install git+https://github.com/caltechlibrary/iga.git
 ```
 
 _If you already installed IGA once before_, and want to update to the latest version, add `--upgrade` to the end of either command line above.
 
 
-### _Alternative 3: installing IGA from sources_
+#### _Alternative 3: installing IGA from sources_
 
 If  you prefer to install IGA directly from the source code, you can do that too. To get a copy of the files, you can clone the GitHub repository:
 ```sh
 git clone https://github.com/caltechlibrary/iga
 ```
 
 Alternatively, you can download the software source files as a ZIP archive directly from your browser using this link: <https://github.com/caltechlibrary/iga/archive/refs/heads/main.zip>
@@ -103,23 +114,70 @@
 Next, after getting a copy of the files,  run `setup.py` inside the code directory:
 ```sh
 cd iga
 python3 setup.py install
 ```
 
 
-## Usage
+### As a GitHub Action
+
+[...forthcoming...]
 
-IGA creates a metadata record in an InvenioRDM server and attaches a GitHub release archive to the record. The GitHub release can be specified using _either_ a full release URL, _or_ a combination of GitHub account + repository + tag. Different command-line options can be used to adjust this behavior.
 
-If the installation process described above is successful, you should end up with a program named `iga` in a location where software is normally installed on your computer.  Running `iga` should be as simple as running any other command-line program. For example, the following command should print a helpful message to your terminal:
+## Quick start
+
+After a successful [installation](#installation) of IGA, here is how you can get started quickly.
+
+### Command-line use
+
+If the [installation](#installation) process described above is successful, you should end up with a program named `iga` in a location where software is normally installed on your computer.  Running `iga` should be as simple as running any other command-line program. For example, the following command should print a helpful message to your terminal:
 ```shell
 iga --help
 ```
 
+IGA's main purpose is to create a metadata record in an InvenioRDM server and attach a GitHub release archive to the record. IGA needs 4 pieces of information to do its work, though for simple repositories you can often get by with just 3:
+1. (Required) The identity of the GitHub release to be archived
+2. (Required) The address of the destination InvenioRDM server
+3. (Required) A Personal Access Token (PAT) for the InvenioRDM server
+4. (Optional) A Personal Access Token for GitHub
+
+The first one (the identity of the GitHub release) is given as arguments to IGA on the command line; the rest can be provided either via command-line options or by setting environment variables. A common way of configuring IGA is to set environment variables in your shell script or your interactive shell. Here is an example using Bash shell syntax, with realistic-looking but fake token values:
+```shell
+export INVENIO_SERVER=https://data.caltech.edu
+export INVENIO_TOKEN=qKLoOH0KYf4D98PGYQGnC09hiuqw3Y1SZllYnonRVzGJbWz2
+export GITHUB_TOKEN=ghp_wQXp6sy3AsKyyEo4l9esHNxOdo6T34Zsthz
+```
+
+Once these environment variables set in your shell, you can more easily invoke IGA. Usage can be as simple as providing a URL for a release in GitHub. For example:
+```shell
+iga https://github.com/mhucka/taupe/releases/tag/v1.2.0
+```
+
+If you give the option `--open` (or `-o` for short) to IGA, it will open the newly-created InvenioRDM entry in your default web browser when it's done:
+```shell
+iga -o https://github.com/mhucka/taupe/releases/tag/v1.2.0
+```
+
+If you want the record to be only a draft and not a final version (perhaps so that you can inspect the result and edit it before finalizing it), use the option `--draft` (or `-d` for short):
+```shell
+iga -d -o https://github.com/mhucka/taupe/releases/tag/v1.2.0
+```
+
+More options and examples can be found in the section on [detailed usage information](#usage) below.
+
+
+### GitHub Action use
+
+[...forthcoming...]
+
+
+## Usage
+
+This section provides detailed information about IGA's operation and options to control it.
+
 ### Identifying the InvenioRDM server
 
 The server address must be provided either as the value of the option `--invenio-server` or in an environment variable named `INVENIO_SERVER`.  If the server address does not begin with `https://`, IGA will prepend it automatically.
 
 ### Providing an InvenioRDM access token
 
 A Personal Access Token (PAT) for making API calls to the InvenioRDM server must be also supplied when invoking IGA. The preferred method is to set the value of the environment variable `INVENIO_TOKEN`. Alternatively, you can use the option `--invenio-token` to pass the token on the command line, but **you are strongly advised to avoid this practice because it is insecure**.
```

### Comparing `iga-0.0.8/README.md` & `iga-0.0.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -8,70 +8,81 @@
 [![PyPI](https://img.shields.io/pypi/v/iga.svg?style=flat-square&color=orange&label=PyPI)](https://pypi.org/project/iga/)
 
 
 ## Table of contents
 
 * [Introduction](#introduction)
 * [Installation](#installation)
+* [Quick start](#quick-start)
 * [Usage](#usage)
 * [Known issues and limitations](#known-issues-and-limitations)
 * [Getting help](#getting-help)
 * [Contributing](#contributing)
 * [License](#license)
 * [Acknowledgments](#authors-and-acknowledgments)
 
 
 ## Introduction
 
-[InvenioRDM](https://inveniosoftware.org/products/rdm/) is a research data management (RDM) repository platform based on the [Invenio Framework](https://inveniosoftware.org/products/framework/) and [Zenodo](https://www.zenodo.org). At institutions like Caltech, InvenioRDM is used as the basis for institutional repositories such as [CaltechDATA](https://data.caltech.edu). Of particular interest to software developers is that a repository like [CaltechDATA](https://data.caltech.edu) offers the means to preserve software projects in a long-term archive managed by their institution.
+[InvenioRDM](https://inveniosoftware.org/products/rdm/) is the basis for many institutional repositories such as [CaltechDATA](https://data.caltech.edu) that enable users to preserve software and datasets in long-term archive. Though such repositories are critical resources, creating detailed records and uploading assets can be a tedious and error-prone process if done manually. This is where the InvenioRDM GitHub Archiver (IGA) comes in.
 
-The _InvenioRDM GitHub Archiver_ (IGA) is a tool for sending software releases from GitHub to an InvenioRDM-based repository server. IGA can be invoked from the command line; it also can be set up as a [GitHub Action](https://docs.github.com/en/actions) to automate the archiving of GitHub software releases in an InvenioRDM repository. Here are some of IGA's other notable features:
-* Automatic extraction of metadata from the GitHub release, the GitHub repository, and [`codemeta.json`](https://codemeta.github.io) and/or [`CITATION.cff`](https://citation-file-format.github.io) files if they exist in the repository
-* Thorough coverage of [InvenioRDM record metadata](https://inveniordm.docs.cern.ch/reference/metadata) using painstaking procedures
-* Automatic recognition of common identifier types that often appear CodeMeta and CFF files, such as [ORCID](https://orcid.org), [ROR](https://ror.org), [DOI](https://www.doi.org), [arXiV](https://arxiv.org), [PMCID/PMID](https://www.ncbi.nlm.nih.gov/pmc/about/public-access-info/), and others
-* Automatic lookup of human names in [ORCID.org](https://orcid.org) if needed (assuming ORCID id's are provided)
-* Automatic lookup of organization names in [ROR](https://ror.org) (assuming ROR id's are provided)
+IGA creates metadata records and sends releases from GitHub to an InvenioRDM-based repository server. IGA can be invoked from the command line; it also can be set up as a [GitHub Action](https://docs.github.com/en/actions) to archive GitHub releases automatically for a repository each time they are made.
+
+<p align=center>
+<img align="middle" src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/example-github-release.jpg" width="40%">
+<span style="font-size: 150%">➜</span>
+<img align="middle" src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/example-record-landing-page.jpg" width="40%">
+</p>
+
+IGA offers many notable features:
+* Automatic metadata extraction from GitHub releases plus [`codemeta.json`](https://codemeta.github.io) and [`CITATION.cff`](https://citation-file-format.github.io) files
+* Thorough coverage of [InvenioRDM record metadata fields](https://inveniordm.docs.cern.ch/reference/metadata) using painstaking procedures
+* Recognition of id's that appear in CodeMeta & CFF files: [ORCID](https://orcid.org), [ROR](https://ror.org), [DOI](https://www.doi.org), [arXiv](https://arxiv.org),  [PMCID](https://www.ncbi.nlm.nih.gov/pmc/about/public-access-info/), and more
 * Automatic lookup of publication data in [DOI.org](https://www.doi.org), [PubMed]((https://www.ncbi.nlm.nih.gov/pmc/about/public-access-info/)), Google Books, & other sources if needed
-* Automatic splitting of human names into family and given names using [ML](https://en.wikipedia.org/wiki/Machine_learning)-based methods, if necessary, to comply with InvenioRDM requirements
-* Support for overriding the metadata record it creates, for complete control if you need it
+* Automatic lookup of organization names in [ROR](https://ror.org) (assuming ROR id's are provided)
+* Automatic lookup of human names in [ORCID.org](https://orcid.org) if needed (assuming ORCID id's are provided)
+* Automatic splitting of human names into family and given names using [ML](https://en.wikipedia.org/wiki/Machine_learning)-based methods
 * Support for InvenioRDM [communities](https://invenio-communities.readthedocs.io/en/latest/)
-* Ability to use the GitHub API without a [GitHub access token](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token) in many cases
+* Support for overriding the metadata record that IGA creates, for complete control if you need it
+* Support for using the GitHub API without a [GitHub access token](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token) in simple cases
 * Extensive use of logging so you can see what's going on under the hood
 
 
 ## Installation
 
-(Note: at this time, only the command-line version of IGA is available.) There are multiple ways of installing IGA.  Please choose the alternative that suits you.
+### As a standalone command-line program
+
+There are multiple ways of installing IGA.  Please choose the alternative that suits you.
 
-### _Alternative 1: installing IGA using `pipx`_
+#### _Alternative 1: installing IGA using `pipx`_
 
 [Pipx](https://pypa.github.io/pipx/) lets you install Python programs in a way that isolates Python dependencies, and yet the resulting `iga` command can be run from any shell and directory &ndash; like any normal program on your computer. If you use `pipx` on your system, you can install IGA with the following command:
 ```sh
 pipx install iga
 ```
 
 Pipx can also let you run IGA directly using `pipx run iga`, although in that case, you must always prefix every IGA command with `pipx run`.  Consult the [documentation for `pipx run`](https://github.com/pypa/pipx#walkthrough-running-an-application-in-a-temporary-virtual-environment) for more information.
 
 
-### _Alternative 2: installing IGA using `pip`_
+#### _Alternative 2: installing IGA using `pip`_
 
 You should be able to install `iga` with [`pip`](https://pip.pypa.io/en/stable/installing/) for Python&nbsp;3.  To install `iga` from the [Python package repository (PyPI)](https://pypi.org), run the following command:
 ```sh
 python3 -m pip install iga
 ```
 
 As an alternative to getting it from [PyPI](https://pypi.org), you can use `pip` to install `iga` directly from GitHub:
 ```sh
 python3 -m pip install git+https://github.com/caltechlibrary/iga.git
 ```
 
 _If you already installed IGA once before_, and want to update to the latest version, add `--upgrade` to the end of either command line above.
 
 
-### _Alternative 3: installing IGA from sources_
+#### _Alternative 3: installing IGA from sources_
 
 If  you prefer to install IGA directly from the source code, you can do that too. To get a copy of the files, you can clone the GitHub repository:
 ```sh
 git clone https://github.com/caltechlibrary/iga
 ```
 
 Alternatively, you can download the software source files as a ZIP archive directly from your browser using this link: <https://github.com/caltechlibrary/iga/archive/refs/heads/main.zip>
@@ -79,23 +90,70 @@
 Next, after getting a copy of the files,  run `setup.py` inside the code directory:
 ```sh
 cd iga
 python3 setup.py install
 ```
 
 
-## Usage
+### As a GitHub Action
+
+[...forthcoming...]
 
-IGA creates a metadata record in an InvenioRDM server and attaches a GitHub release archive to the record. The GitHub release can be specified using _either_ a full release URL, _or_ a combination of GitHub account + repository + tag. Different command-line options can be used to adjust this behavior.
 
-If the installation process described above is successful, you should end up with a program named `iga` in a location where software is normally installed on your computer.  Running `iga` should be as simple as running any other command-line program. For example, the following command should print a helpful message to your terminal:
+## Quick start
+
+After a successful [installation](#installation) of IGA, here is how you can get started quickly.
+
+### Command-line use
+
+If the [installation](#installation) process described above is successful, you should end up with a program named `iga` in a location where software is normally installed on your computer.  Running `iga` should be as simple as running any other command-line program. For example, the following command should print a helpful message to your terminal:
 ```shell
 iga --help
 ```
 
+IGA's main purpose is to create a metadata record in an InvenioRDM server and attach a GitHub release archive to the record. IGA needs 4 pieces of information to do its work, though for simple repositories you can often get by with just 3:
+1. (Required) The identity of the GitHub release to be archived
+2. (Required) The address of the destination InvenioRDM server
+3. (Required) A Personal Access Token (PAT) for the InvenioRDM server
+4. (Optional) A Personal Access Token for GitHub
+
+The first one (the identity of the GitHub release) is given as arguments to IGA on the command line; the rest can be provided either via command-line options or by setting environment variables. A common way of configuring IGA is to set environment variables in your shell script or your interactive shell. Here is an example using Bash shell syntax, with realistic-looking but fake token values:
+```shell
+export INVENIO_SERVER=https://data.caltech.edu
+export INVENIO_TOKEN=qKLoOH0KYf4D98PGYQGnC09hiuqw3Y1SZllYnonRVzGJbWz2
+export GITHUB_TOKEN=ghp_wQXp6sy3AsKyyEo4l9esHNxOdo6T34Zsthz
+```
+
+Once these environment variables set in your shell, you can more easily invoke IGA. Usage can be as simple as providing a URL for a release in GitHub. For example:
+```shell
+iga https://github.com/mhucka/taupe/releases/tag/v1.2.0
+```
+
+If you give the option `--open` (or `-o` for short) to IGA, it will open the newly-created InvenioRDM entry in your default web browser when it's done:
+```shell
+iga -o https://github.com/mhucka/taupe/releases/tag/v1.2.0
+```
+
+If you want the record to be only a draft and not a final version (perhaps so that you can inspect the result and edit it before finalizing it), use the option `--draft` (or `-d` for short):
+```shell
+iga -d -o https://github.com/mhucka/taupe/releases/tag/v1.2.0
+```
+
+More options and examples can be found in the section on [detailed usage information](#usage) below.
+
+
+### GitHub Action use
+
+[...forthcoming...]
+
+
+## Usage
+
+This section provides detailed information about IGA's operation and options to control it.
+
 ### Identifying the InvenioRDM server
 
 The server address must be provided either as the value of the option `--invenio-server` or in an environment variable named `INVENIO_SERVER`.  If the server address does not begin with `https://`, IGA will prepend it automatically.
 
 ### Providing an InvenioRDM access token
 
 A Personal Access Token (PAT) for making API calls to the InvenioRDM server must be also supplied when invoking IGA. The preferred method is to set the value of the environment variable `INVENIO_TOKEN`. Alternatively, you can use the option `--invenio-token` to pass the token on the command line, but **you are strongly advised to avoid this practice because it is insecure**.
```

### Comparing `iga-0.0.8/iga/__init__.py` & `iga-0.0.9/iga/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # .............................................................................
 #
 #  ╭────────────────────── Notice ── Notice ── Notice ─────────────────────╮
 #  |    The following values are automatically updated at every release    |
 #  |    by the Makefile. Manual changes to these values will be lost.      |
 #  ╰────────────────────── Notice ── Notice ── Notice ─────────────────────╯
 
-__version__     = '0.0.8'
+__version__     = '0.0.9'
 __description__ = 'InvenioRDM GitHub Archiver'
 __url__         = 'https://github.com/caltechlibrary/iga'
 __author__      = 'Michael Hucka'
 __email__       = 'helpdesk@library.caltech.edu'
 __license__     = 'https://github.com/caltechlibrary/iga/blob/main/LICENSE'
```

### Comparing `iga-0.0.8/iga/__main__.py` & `iga-0.0.9/iga/__main__.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.8/iga/cli.py` & `iga-0.0.9/iga/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -702,15 +702,17 @@
             log(f'exiting due to {error_type}: {str(ex)}')
             _alert(ctx, 'IGA experienced an error. Please report this to the'
                    f' developers. Your version of IGA is {iga.__version__}.'
                    f' For information about how to report errors, please see'
                    f' {iga.__url__}/.\n\n{error_type}: {str(ex)}', False)
             exit_code = ExitCode.exception
 
-        if os.environ.get('IGA_RUN_MODE') == 'debug':
+        # If mode is debug, drop into pdb unless we're running as a GHA.
+        if (os.environ.get('IGA_RUN_MODE') == 'debug'
+                and 'GITHUB_ACTION' not in os.environ):
             import pdb
             import traceback
             exception = sys.exc_info()
             details = ''.join(traceback.format_exception(*exception))
             log(f'{ex.__class__.__name__}: ' + str(ex) + '\n\n' + details)
             Console().print_exception()
             pdb.post_mortem(exception[2])
```

### Comparing `iga-0.0.8/iga/data_utils.py` & `iga-0.0.9/iga/data_utils.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.8/iga/doi.py` & `iga-0.0.9/iga/doi.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.8/iga/exceptions.py` & `iga-0.0.9/iga/exceptions.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.8/iga/exit_codes.py` & `iga-0.0.9/iga/exit_codes.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.8/iga/github.py` & `iga-0.0.9/iga/github.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.8/iga/id_utils.py` & `iga-0.0.9/iga/id_utils.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.8/iga/invenio.py` & `iga-0.0.9/iga/invenio.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.8/iga/json_utils.py` & `iga-0.0.9/iga/json_utils.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.8/iga/licenses.py` & `iga-0.0.9/iga/licenses.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.8/iga/metadata.py` & `iga-0.0.9/iga/metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -1137,14 +1137,21 @@
 
         # Add repo languages as topics too.
         if languages := github_repo_languages(repo):
             log('adding GitHub repo languages to "subjects"')
         for lang in languages:
             subjects.add(lang)
 
+    # Always add GitHub as a tag.
+    subjects.add('GitHub')
+
+    # Always add a tag about IGA. Users are free to edit it out, but it helps
+    # repository maintainers to gauge manual vs automated record creation.
+    subjects.add('IGA')
+
     return [{'subject': x} for x in sorted(subjects, key=str.lower)]
 
 
 def title(repo, release, include_all):
     '''Return InvenioRDM "title".
     https://inveniordm.docs.cern.ch/reference/metadata/#title-1
     '''
```

### Comparing `iga-0.0.8/iga/name_utils.py` & `iga-0.0.9/iga/name_utils.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.8/iga/orcid.py` & `iga-0.0.9/iga/orcid.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.8/iga/reference.py` & `iga-0.0.9/iga/reference.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.8/iga/ror.py` & `iga-0.0.9/iga/ror.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.8/iga/text_utils.py` & `iga-0.0.9/iga/text_utils.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.8/iga.egg-info/PKG-INFO` & `iga-0.0.9/iga.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iga
-Version: 0.0.8
+Version: 0.0.9
 Summary: InvenioRDM GitHub Archiver
 Home-page: https://github.com/caltechlibrary/iga
 Author: Michael Hucka
 Author-email: helpdesk@library.caltech.edu
 License: https://github.com/caltechlibrary/iga/blob/main/LICENSE
 Project-URL: Source Code, https://github.com/caltechlibrary/iga
 Project-URL: Bug Tracker, https://github.com/caltechlibrary/iga/issues
@@ -32,70 +32,81 @@
 [![PyPI](https://img.shields.io/pypi/v/iga.svg?style=flat-square&color=orange&label=PyPI)](https://pypi.org/project/iga/)
 
 
 ## Table of contents
 
 * [Introduction](#introduction)
 * [Installation](#installation)
+* [Quick start](#quick-start)
 * [Usage](#usage)
 * [Known issues and limitations](#known-issues-and-limitations)
 * [Getting help](#getting-help)
 * [Contributing](#contributing)
 * [License](#license)
 * [Acknowledgments](#authors-and-acknowledgments)
 
 
 ## Introduction
 
-[InvenioRDM](https://inveniosoftware.org/products/rdm/) is a research data management (RDM) repository platform based on the [Invenio Framework](https://inveniosoftware.org/products/framework/) and [Zenodo](https://www.zenodo.org). At institutions like Caltech, InvenioRDM is used as the basis for institutional repositories such as [CaltechDATA](https://data.caltech.edu). Of particular interest to software developers is that a repository like [CaltechDATA](https://data.caltech.edu) offers the means to preserve software projects in a long-term archive managed by their institution.
+[InvenioRDM](https://inveniosoftware.org/products/rdm/) is the basis for many institutional repositories such as [CaltechDATA](https://data.caltech.edu) that enable users to preserve software and datasets in long-term archive. Though such repositories are critical resources, creating detailed records and uploading assets can be a tedious and error-prone process if done manually. This is where the InvenioRDM GitHub Archiver (IGA) comes in.
 
-The _InvenioRDM GitHub Archiver_ (IGA) is a tool for sending software releases from GitHub to an InvenioRDM-based repository server. IGA can be invoked from the command line; it also can be set up as a [GitHub Action](https://docs.github.com/en/actions) to automate the archiving of GitHub software releases in an InvenioRDM repository. Here are some of IGA's other notable features:
-* Automatic extraction of metadata from the GitHub release, the GitHub repository, and [`codemeta.json`](https://codemeta.github.io) and/or [`CITATION.cff`](https://citation-file-format.github.io) files if they exist in the repository
-* Thorough coverage of [InvenioRDM record metadata](https://inveniordm.docs.cern.ch/reference/metadata) using painstaking procedures
-* Automatic recognition of common identifier types that often appear CodeMeta and CFF files, such as [ORCID](https://orcid.org), [ROR](https://ror.org), [DOI](https://www.doi.org), [arXiV](https://arxiv.org), [PMCID/PMID](https://www.ncbi.nlm.nih.gov/pmc/about/public-access-info/), and others
-* Automatic lookup of human names in [ORCID.org](https://orcid.org) if needed (assuming ORCID id's are provided)
-* Automatic lookup of organization names in [ROR](https://ror.org) (assuming ROR id's are provided)
+IGA creates metadata records and sends releases from GitHub to an InvenioRDM-based repository server. IGA can be invoked from the command line; it also can be set up as a [GitHub Action](https://docs.github.com/en/actions) to archive GitHub releases automatically for a repository each time they are made.
+
+<p align=center>
+<img align="middle" src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/example-github-release.jpg" width="40%">
+<span style="font-size: 150%">➜</span>
+<img align="middle" src="https://github.com/caltechlibrary/iga/raw/main/docs/_static/media/example-record-landing-page.jpg" width="40%">
+</p>
+
+IGA offers many notable features:
+* Automatic metadata extraction from GitHub releases plus [`codemeta.json`](https://codemeta.github.io) and [`CITATION.cff`](https://citation-file-format.github.io) files
+* Thorough coverage of [InvenioRDM record metadata fields](https://inveniordm.docs.cern.ch/reference/metadata) using painstaking procedures
+* Recognition of id's that appear in CodeMeta & CFF files: [ORCID](https://orcid.org), [ROR](https://ror.org), [DOI](https://www.doi.org), [arXiv](https://arxiv.org),  [PMCID](https://www.ncbi.nlm.nih.gov/pmc/about/public-access-info/), and more
 * Automatic lookup of publication data in [DOI.org](https://www.doi.org), [PubMed]((https://www.ncbi.nlm.nih.gov/pmc/about/public-access-info/)), Google Books, & other sources if needed
-* Automatic splitting of human names into family and given names using [ML](https://en.wikipedia.org/wiki/Machine_learning)-based methods, if necessary, to comply with InvenioRDM requirements
-* Support for overriding the metadata record it creates, for complete control if you need it
+* Automatic lookup of organization names in [ROR](https://ror.org) (assuming ROR id's are provided)
+* Automatic lookup of human names in [ORCID.org](https://orcid.org) if needed (assuming ORCID id's are provided)
+* Automatic splitting of human names into family and given names using [ML](https://en.wikipedia.org/wiki/Machine_learning)-based methods
 * Support for InvenioRDM [communities](https://invenio-communities.readthedocs.io/en/latest/)
-* Ability to use the GitHub API without a [GitHub access token](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token) in many cases
+* Support for overriding the metadata record that IGA creates, for complete control if you need it
+* Support for using the GitHub API without a [GitHub access token](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token) in simple cases
 * Extensive use of logging so you can see what's going on under the hood
 
 
 ## Installation
 
-(Note: at this time, only the command-line version of IGA is available.) There are multiple ways of installing IGA.  Please choose the alternative that suits you.
+### As a standalone command-line program
+
+There are multiple ways of installing IGA.  Please choose the alternative that suits you.
 
-### _Alternative 1: installing IGA using `pipx`_
+#### _Alternative 1: installing IGA using `pipx`_
 
 [Pipx](https://pypa.github.io/pipx/) lets you install Python programs in a way that isolates Python dependencies, and yet the resulting `iga` command can be run from any shell and directory &ndash; like any normal program on your computer. If you use `pipx` on your system, you can install IGA with the following command:
 ```sh
 pipx install iga
 ```
 
 Pipx can also let you run IGA directly using `pipx run iga`, although in that case, you must always prefix every IGA command with `pipx run`.  Consult the [documentation for `pipx run`](https://github.com/pypa/pipx#walkthrough-running-an-application-in-a-temporary-virtual-environment) for more information.
 
 
-### _Alternative 2: installing IGA using `pip`_
+#### _Alternative 2: installing IGA using `pip`_
 
 You should be able to install `iga` with [`pip`](https://pip.pypa.io/en/stable/installing/) for Python&nbsp;3.  To install `iga` from the [Python package repository (PyPI)](https://pypi.org), run the following command:
 ```sh
 python3 -m pip install iga
 ```
 
 As an alternative to getting it from [PyPI](https://pypi.org), you can use `pip` to install `iga` directly from GitHub:
 ```sh
 python3 -m pip install git+https://github.com/caltechlibrary/iga.git
 ```
 
 _If you already installed IGA once before_, and want to update to the latest version, add `--upgrade` to the end of either command line above.
 
 
-### _Alternative 3: installing IGA from sources_
+#### _Alternative 3: installing IGA from sources_
 
 If  you prefer to install IGA directly from the source code, you can do that too. To get a copy of the files, you can clone the GitHub repository:
 ```sh
 git clone https://github.com/caltechlibrary/iga
 ```
 
 Alternatively, you can download the software source files as a ZIP archive directly from your browser using this link: <https://github.com/caltechlibrary/iga/archive/refs/heads/main.zip>
@@ -103,23 +114,70 @@
 Next, after getting a copy of the files,  run `setup.py` inside the code directory:
 ```sh
 cd iga
 python3 setup.py install
 ```
 
 
-## Usage
+### As a GitHub Action
+
+[...forthcoming...]
 
-IGA creates a metadata record in an InvenioRDM server and attaches a GitHub release archive to the record. The GitHub release can be specified using _either_ a full release URL, _or_ a combination of GitHub account + repository + tag. Different command-line options can be used to adjust this behavior.
 
-If the installation process described above is successful, you should end up with a program named `iga` in a location where software is normally installed on your computer.  Running `iga` should be as simple as running any other command-line program. For example, the following command should print a helpful message to your terminal:
+## Quick start
+
+After a successful [installation](#installation) of IGA, here is how you can get started quickly.
+
+### Command-line use
+
+If the [installation](#installation) process described above is successful, you should end up with a program named `iga` in a location where software is normally installed on your computer.  Running `iga` should be as simple as running any other command-line program. For example, the following command should print a helpful message to your terminal:
 ```shell
 iga --help
 ```
 
+IGA's main purpose is to create a metadata record in an InvenioRDM server and attach a GitHub release archive to the record. IGA needs 4 pieces of information to do its work, though for simple repositories you can often get by with just 3:
+1. (Required) The identity of the GitHub release to be archived
+2. (Required) The address of the destination InvenioRDM server
+3. (Required) A Personal Access Token (PAT) for the InvenioRDM server
+4. (Optional) A Personal Access Token for GitHub
+
+The first one (the identity of the GitHub release) is given as arguments to IGA on the command line; the rest can be provided either via command-line options or by setting environment variables. A common way of configuring IGA is to set environment variables in your shell script or your interactive shell. Here is an example using Bash shell syntax, with realistic-looking but fake token values:
+```shell
+export INVENIO_SERVER=https://data.caltech.edu
+export INVENIO_TOKEN=qKLoOH0KYf4D98PGYQGnC09hiuqw3Y1SZllYnonRVzGJbWz2
+export GITHUB_TOKEN=ghp_wQXp6sy3AsKyyEo4l9esHNxOdo6T34Zsthz
+```
+
+Once these environment variables set in your shell, you can more easily invoke IGA. Usage can be as simple as providing a URL for a release in GitHub. For example:
+```shell
+iga https://github.com/mhucka/taupe/releases/tag/v1.2.0
+```
+
+If you give the option `--open` (or `-o` for short) to IGA, it will open the newly-created InvenioRDM entry in your default web browser when it's done:
+```shell
+iga -o https://github.com/mhucka/taupe/releases/tag/v1.2.0
+```
+
+If you want the record to be only a draft and not a final version (perhaps so that you can inspect the result and edit it before finalizing it), use the option `--draft` (or `-d` for short):
+```shell
+iga -d -o https://github.com/mhucka/taupe/releases/tag/v1.2.0
+```
+
+More options and examples can be found in the section on [detailed usage information](#usage) below.
+
+
+### GitHub Action use
+
+[...forthcoming...]
+
+
+## Usage
+
+This section provides detailed information about IGA's operation and options to control it.
+
 ### Identifying the InvenioRDM server
 
 The server address must be provided either as the value of the option `--invenio-server` or in an environment variable named `INVENIO_SERVER`.  If the server address does not begin with `https://`, IGA will prepend it automatically.
 
 ### Providing an InvenioRDM access token
 
 A Personal Access Token (PAT) for making API calls to the InvenioRDM server must be also supplied when invoking IGA. The preferred method is to set the value of the environment variable `INVENIO_TOKEN`. Alternatively, you can use the option `--invenio-token` to pass the token on the command line, but **you are strongly advised to avoid this practice because it is insecure**.
```

### Comparing `iga-0.0.8/iga.egg-info/SOURCES.txt` & `iga-0.0.9/iga.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `iga-0.0.8/iga.egg-info/requires.txt` & `iga-0.0.9/iga.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `iga-0.0.8/setup.cfg` & `iga-0.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = iga
-version = 0.0.8
+version = 0.0.9
 description = InvenioRDM GitHub Archiver
 author = Michael Hucka
 author_email = helpdesk@library.caltech.edu
 license = https://github.com/caltechlibrary/iga/blob/main/LICENSE
 license_files = LICENSE
 url = https://github.com/caltechlibrary/iga
 project_urls =
```

### Comparing `iga-0.0.8/setup.py` & `iga-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.8/tests/test_cli.py` & `iga-0.0.9/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.8/tests/test_data_utils.py` & `iga-0.0.9/tests/test_data_utils.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.8/tests/test_doi.py` & `iga-0.0.9/tests/test_doi.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.8/tests/test_exceptions.py` & `iga-0.0.9/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.8/tests/test_github.py` & `iga-0.0.9/tests/test_github.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.8/tests/test_github_mocks.py` & `iga-0.0.9/tests/test_github_mocks.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.8/tests/test_id_utils.py` & `iga-0.0.9/tests/test_id_utils.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.8/tests/test_init.py` & `iga-0.0.9/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.8/tests/test_is_person.py` & `iga-0.0.9/tests/test_is_person.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.8/tests/test_licenses.py` & `iga-0.0.9/tests/test_licenses.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.8/tests/test_name_splitting.py` & `iga-0.0.9/tests/test_name_splitting.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.8/tests/test_name_utils.py` & `iga-0.0.9/tests/test_name_utils.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.8/tests/test_orcid.py` & `iga-0.0.9/tests/test_orcid.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.8/tests/test_record_from_codemeta.py` & `iga-0.0.9/tests/test_record_from_codemeta.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.8/tests/test_reference.py` & `iga-0.0.9/tests/test_reference.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.8/tests/test_ror.py` & `iga-0.0.9/tests/test_ror.py`

 * *Files identical despite different names*

### Comparing `iga-0.0.8/tests/test_text_utils.py` & `iga-0.0.9/tests/test_text_utils.py`

 * *Files identical despite different names*

