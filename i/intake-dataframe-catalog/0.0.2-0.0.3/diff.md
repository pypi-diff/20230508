# Comparing `tmp/intake_dataframe_catalog-0.0.2.tar.gz` & `tmp/intake_dataframe_catalog-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "intake_dataframe_catalog-0.0.2.tar", last modified: Fri May  5 05:52:13 2023, max compression
+gzip compressed data, was "intake_dataframe_catalog-0.0.3.tar", last modified: Mon May  8 07:46:50 2023, max compression
```

## Comparing `intake_dataframe_catalog-0.0.2.tar` & `intake_dataframe_catalog-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:52:13.756201 intake_dataframe_catalog-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-05 05:52:05.000000 intake_dataframe_catalog-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-05 05:52:13.756201 intake_dataframe_catalog-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-05-05 05:52:05.000000 intake_dataframe_catalog-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-05 05:52:13.756201 intake_dataframe_catalog-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-05-05 05:52:05.000000 intake_dataframe_catalog-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:52:13.756201 intake_dataframe_catalog-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:52:13.756201 intake_dataframe_catalog-0.0.2/src/intake_dataframe_catalog/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-05 05:52:05.000000 intake_dataframe_catalog-0.0.2/src/intake_dataframe_catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-05-05 05:52:05.000000 intake_dataframe_catalog-0.0.2/src/intake_dataframe_catalog/_search.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-05 05:52:13.756201 intake_dataframe_catalog-0.0.2/src/intake_dataframe_catalog/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    21064 2023-05-05 05:52:05.000000 intake_dataframe_catalog-0.0.2/src/intake_dataframe_catalog/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:52:13.756201 intake_dataframe_catalog-0.0.2/src/intake_dataframe_catalog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-05 05:52:13.000000 intake_dataframe_catalog-0.0.2/src/intake_dataframe_catalog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-05 05:52:13.000000 intake_dataframe_catalog-0.0.2/src/intake_dataframe_catalog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 05:52:13.000000 intake_dataframe_catalog-0.0.2/src/intake_dataframe_catalog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-05 05:52:13.000000 intake_dataframe_catalog-0.0.2/src/intake_dataframe_catalog.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-05 05:52:13.000000 intake_dataframe_catalog-0.0.2/src/intake_dataframe_catalog.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-05 05:52:13.000000 intake_dataframe_catalog-0.0.2/src/intake_dataframe_catalog.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    83780 2023-05-05 05:52:05.000000 intake_dataframe_catalog-0.0.2/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:46:50.525992 intake_dataframe_catalog-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-08 07:46:36.000000 intake_dataframe_catalog-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4314 2023-05-08 07:46:50.525992 intake_dataframe_catalog-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-05-08 07:46:36.000000 intake_dataframe_catalog-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-08 07:46:36.000000 intake_dataframe_catalog-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-08 07:46:50.525992 intake_dataframe_catalog-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-08 07:46:36.000000 intake_dataframe_catalog-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:46:50.521992 intake_dataframe_catalog-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:46:50.525992 intake_dataframe_catalog-0.0.3/src/intake_dataframe_catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-08 07:46:36.000000 intake_dataframe_catalog-0.0.3/src/intake_dataframe_catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-05-08 07:46:36.000000 intake_dataframe_catalog-0.0.3/src/intake_dataframe_catalog/_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-08 07:46:50.525992 intake_dataframe_catalog-0.0.3/src/intake_dataframe_catalog/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21064 2023-05-08 07:46:36.000000 intake_dataframe_catalog-0.0.3/src/intake_dataframe_catalog/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:46:50.525992 intake_dataframe_catalog-0.0.3/src/intake_dataframe_catalog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4314 2023-05-08 07:46:50.000000 intake_dataframe_catalog-0.0.3/src/intake_dataframe_catalog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-08 07:46:50.000000 intake_dataframe_catalog-0.0.3/src/intake_dataframe_catalog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 07:46:50.000000 intake_dataframe_catalog-0.0.3/src/intake_dataframe_catalog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-08 07:46:50.000000 intake_dataframe_catalog-0.0.3/src/intake_dataframe_catalog.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-08 07:46:50.000000 intake_dataframe_catalog-0.0.3/src/intake_dataframe_catalog.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-08 07:46:50.000000 intake_dataframe_catalog-0.0.3/src/intake_dataframe_catalog.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:46:50.525992 intake_dataframe_catalog-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    21272 2023-05-08 07:46:36.000000 intake_dataframe_catalog-0.0.3/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9900 2023-05-08 07:46:36.000000 intake_dataframe_catalog-0.0.3/tests/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83780 2023-05-08 07:46:36.000000 intake_dataframe_catalog-0.0.3/versioneer.py
```

### Comparing `intake_dataframe_catalog-0.0.2/LICENSE` & `intake_dataframe_catalog-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `intake_dataframe_catalog-0.0.2/README.md` & `intake_dataframe_catalog-0.0.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -3,39 +3,42 @@
 A simple intake plugin for a searchable table of intake catalogs and associated metadata.
 __________
 
 | Documentation | [![docs][docs-badge]][docs-link] |
 | :---: |  :---: |
 | **Package** | [![PyPI][PyPI-badge]][PyPI-link] |
 | **CI** | [![tests][ci-tests-badge]][ci-tests-link] [![pre-commit][ci-precommit-badge]][ci-precommit-link] |
+| **CD** | [![build distribution][cd-badge]][cd-link] |
 | **Development** | [![codecov][codecov-badge]][codecov-link] [![black][black-badge]][black-link] |
 | **License** | [![License][license-badge]][license-link] |
 
 Overview
 --------
 
 intake-dataframe-catalog is a simple intake plugin for a searchable table of intake catalogs.
 The table is represented in memory as a pandas DataFrame and can be serialized and shared as
-a CSV file. Each row in the dataframe catalog corresponds to another intake catalog (refered
-to in this documentation as a "subcatalog") and the columns contain metadata associated with
+a CSV file. Each row in the dataframe catalog corresponds to another intake catalog (referred
+to in the context of intake-dataframe-catlog as a "subcatalog") and the columns contain metadata associated with
 each subcatalog that a user may want to peruse and/or search. The original use-case for
 intake-dataframe-catalog was to provide a user-friendly catalog of a large number
-`intake-esm <https://intake-esm.readthedocs.io/en/stable/>`_ catalogs. intake-dataframe-catalog
+[intake-esm](https://intake-esm.readthedocs.io/en/stable/) catalogs. intake-dataframe-catalog
 enables users to peruse and search on core metadata from each intake-esm subcatalog to find
 the subcatalogs that are most relevant to their work (e.g. "which subcatalogs contain model
 X and variable Y?"). Once a users has found the subcatalog(s) that interest them, they can
 load those subcatalogs and access the data they reference.
 
+See [the documentation](https://intake-dataframe-catalog.readthedocs.io/en/latest/?badge=latest) for more information.
+
 Why?
 ----
 
 Intake already provides the ability to
-`nest catalogs <https://intake.readthedocs.io/en/latest/catalog.html#catalog-nesting>`_ and
+[nest catalogs](https://intake.readthedocs.io/en/latest/catalog.html#catalog-nesting) and
 search across them. However, data discoverability is limited in the case of very large numbers
-of nested catalogs, and the search functionality does readily provide the ability to execute
+of nested catalogs, and the search functionality does not readily provide the ability to execute
 complex searches on nested catalog metadata. intake-dataframe-catalog aims to provide a very
 simple catalog of subcatalogs that emphasises subcatalog search and discoverability.
 
 ## Installation
 
 To install using the [pip](https://pypi.org/project/pip/) package manager:
 
@@ -47,13 +50,15 @@
 [docs-link]: https://intake-dataframe-catalog.readthedocs.io/en/latest/?badge=latest
 [PyPI-badge]: https://img.shields.io/pypi/v/intake-dataframe-catalog
 [PyPI-link]: https://pypi.org/project/intake-dataframe-catalog/
 [ci-tests-badge]: https://github.com/ACCESS-NRI/intake-dataframe-catalog/actions/workflows/tests.yml/badge.svg
 [ci-tests-link]: https://github.com/ACCESS-NRI/intake-dataframe-catalog/actions/workflows/tests.yml
 [ci-precommit-badge]: https://github.com/ACCESS-NRI/intake-dataframe-catalog/actions/workflows/pre-commit.yml/badge.svg
 [ci-precommit-link]: https://github.com/ACCESS-NRI/intake-dataframe-catalog/actions/workflows/pre-commit.yml
+[cd-badge]: https://github.com/ACCESS-NRI/intake-dataframe-catalog/actions/workflows/release.yml/badge.svg
+[cd-link]: https://github.com/ACCESS-NRI/intake-dataframe-catalog/actions/workflows/release.yml
 [codecov-badge]: https://codecov.io/gh/ACCESS-NRI/intake-dataframe-catalog/branch/main/graph/badge.svg?token=4EZNH1HYAN
 [codecov-link]: https://codecov.io/gh/ACCESS-NRI/intake-dataframe-catalog
 [black-badge]: https://img.shields.io/badge/code%20style-black-000000.svg
 [black-link]: https://github.com/python/black
 [license-badge]: https://img.shields.io/github/license/ACCESS-NRI/intake-dataframe-catalog
 [license-link]: https://github.com/ACCESS-NRI/intake-dataframe-catalog/blob/main/LICENSE
```

### Comparing `intake_dataframe_catalog-0.0.2/src/intake_dataframe_catalog/_search.py` & `intake_dataframe_catalog-0.0.3/src/intake_dataframe_catalog/_search.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # Copyright 2023 ACCESS-NRI and contributors. See the top-level COPYRIGHT file for details.
 # SPDX-License-Identifier: Apache-2.0
 
 # Stolen and adapted from https://github.com/intake/intake-esm/blob/main/intake_esm/_search.py
 
 import re
 import typing
+import itertools
 
 import numpy as np
 import pandas as pd
 
 
-def is_pattern(value: typing.Union[str, typing.Pattern]) -> bool:
+def _is_pattern(value: typing.Union[str, typing.Pattern]) -> bool:
     """
     Check whether the passed value is a pattern
 
     Parameters
     ----------
     value: str or Pattern
         The value to check
@@ -30,15 +31,15 @@
     except (TypeError, AttributeError):
         return False
 
 
 def _match_iterables(strings, pattern, regex):
     """
     Given an iterable of strings, return all that match the provided pattern
-    as a list.
+    as a set.
     """
     matches = []
     for string in strings:
         if regex:
             match = re.match(pattern, string, flags=0)
         else:
             match = pattern == string
@@ -71,58 +72,78 @@
         If True, groupby name_column and return only entries that match
         for all elements in each group
     Returns
     -------
     dataframe: :py:class:`~pandas.DataFrame`
             A new dataframe with the entries satisfying the query criteria.
     """
+
     df = df.copy()
-    groups = df[name_column]
-    n_groups = groups.nunique()
+
     if not query:
-        return pd.DataFrame(columns=df.columns)
-    global_mask = np.ones(len(df), dtype=bool)
-    has_all_mask = np.ones(n_groups, dtype=bool)
-    for column, values in query.items():
-        local_mask = np.zeros(len(df), dtype=bool)
-        has_mask = np.zeros(n_groups, dtype=bool)
-        column_is_stringtype = isinstance(
-            df[column].dtype, (object, pd.core.arrays.string_.StringDtype)
-        )
-        column_has_iterables = column in columns_with_iterables
-
-        if column_has_iterables:
-            matched_iterables = pd.Series(np.empty((len(df), 0)).tolist(), name=column)
-
-        for value in values:
-            if column_has_iterables:
-                matched = df[column].apply(
-                    lambda iters: _match_iterables(iters, value, is_pattern(value))
-                )
-                mask = matched.astype(bool)
-                matched_iterables += matched
-            elif column_is_stringtype and is_pattern(value):
-                mask = df[column].str.contains(value, regex=True, case=True, flags=0)
+        return df
+
+    # 1. First create a mask for each query
+    searches = [(key, val) for key, vals in query.items() for val in vals]
+    search_matches = {column: {} for column in query.keys()}
+
+    matched_iterables = pd.DataFrame()
+
+    for (column, value) in searches:
+
+        is_pattern = _is_pattern(value)
+
+        if column in columns_with_iterables:
+            matches = df[column].apply(
+                lambda values: _match_iterables(values, value, is_pattern)
+            )
+            match = matches.astype(bool)
+
+            # Keep track of which iterables matched
+            if column in matched_iterables.columns:
+                matched_iterables[column] = matched_iterables[column] + matches
             else:
-                mask = df[column] == value
-            local_mask = local_mask + mask
-            has_mask = has_mask + mask.groupby(groups).any().astype(int)
-
-        mask = has_mask == len(values)
-        has_all_mask = has_all_mask & mask
-
-        if column_has_iterables:
-            # Overwrite iterable entries with subset found
-            cast_type = type(df[column].iloc[0])
-            df.loc[
-                matched_iterables.loc[local_mask].index, column
-            ] = matched_iterables.loc[local_mask].apply(cast_type)
+                matched_iterables[column] = matches
+
+        elif is_pattern:
+            match = df[column].str.contains(value, regex=True, case=True, flags=0)
+        else:
+            match = df[column] == value
+
+        search_matches[column][value] = match
+
+    # 2. Now combine the masks
+    conditions = set(itertools.product(*[tuple(v) for v in query.values()]))
+
+    groups = df[name_column]
+
+    global_match = np.zeros(len(df), dtype=bool)
+    n_conditions_in_group = np.zeros(groups.nunique(), dtype=bool)
+
+    for condition in conditions:
+
+        condition_match = np.ones(len(df), dtype=bool)
+
+        for column, value in zip(query.keys(), condition):
+
+            condition_match = condition_match & search_matches[column][value]
+
+        n_conditions_in_group = n_conditions_in_group + condition_match.groupby(
+            groups
+        ).any().astype(int)
+
+        global_match = global_match | condition_match
 
-        global_mask = global_mask & local_mask
+    # 3. Replace queried columns with iterables with reduced versions
+    if not matched_iterables.empty:
+        types = {col: type(df[col].iloc[0]) for col in matched_iterables.columns}
+        df[matched_iterables.columns] = matched_iterables.apply(types)
 
     if require_all:
+        has_all = n_conditions_in_group == len(conditions)
         # Expand has_all_mask across all groups
-        has_all_mask = has_all_mask.loc[groups].reset_index(drop=True)
-        global_mask = global_mask & has_all_mask
+        has_all = has_all.loc[groups].reset_index(drop=True)
+        global_match = global_match & has_all
+    else:
+        global_match = global_match
 
-    results = df.loc[global_mask]
-    return results.reset_index(drop=True)
+    return df.loc[global_match]
```

### Comparing `intake_dataframe_catalog-0.0.2/src/intake_dataframe_catalog/core.py` & `intake_dataframe_catalog-0.0.3/src/intake_dataframe_catalog/core.py`

 * *Files identical despite different names*

### Comparing `intake_dataframe_catalog-0.0.2/src/intake_dataframe_catalog.egg-info/SOURCES.txt` & `intake_dataframe_catalog-0.0.3/src/intake_dataframe_catalog.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 LICENSE
 README.md
+pyproject.toml
 setup.cfg
 setup.py
 versioneer.py
 src/intake_dataframe_catalog/__init__.py
 src/intake_dataframe_catalog/_search.py
 src/intake_dataframe_catalog/_version.py
 src/intake_dataframe_catalog/core.py
 src/intake_dataframe_catalog.egg-info/PKG-INFO
 src/intake_dataframe_catalog.egg-info/SOURCES.txt
 src/intake_dataframe_catalog.egg-info/dependency_links.txt
 src/intake_dataframe_catalog.egg-info/entry_points.txt
 src/intake_dataframe_catalog.egg-info/requires.txt
-src/intake_dataframe_catalog.egg-info/top_level.txt
+src/intake_dataframe_catalog.egg-info/top_level.txt
+tests/test_core.py
+tests/test_search.py
```

### Comparing `intake_dataframe_catalog-0.0.2/versioneer.py` & `intake_dataframe_catalog-0.0.3/versioneer.py`

 * *Files identical despite different names*

