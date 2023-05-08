# Comparing `tmp/dbis-er-diagram-1.0.5.tar.gz` & `tmp/dbis-er-diagram-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbis-er-diagram-1.0.5.tar", last modified: Wed May  3 14:36:43 2023, max compression
+gzip compressed data, was "dbis-er-diagram-1.0.6.tar", last modified: Mon May  8 16:16:32 2023, max compression
```

## Comparing `dbis-er-diagram-1.0.5.tar` & `dbis-er-diagram-1.0.6.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-05-03 14:36:43.581057 dbis-er-diagram-1.0.5/
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    11357 2023-05-03 13:33:48.000000 dbis-er-diagram-1.0.5/LICENSE
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    15713 2023-05-03 14:36:43.581057 dbis-er-diagram-1.0.5/PKG-INFO
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    15133 2023-05-03 13:33:48.000000 dbis-er-diagram-1.0.5/README.md
-drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-05-03 14:36:43.580057 dbis-er-diagram-1.0.5/dbis_er_diagram.egg-info/
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    15713 2023-05-03 14:36:43.000000 dbis-er-diagram-1.0.5/dbis_er_diagram.egg-info/PKG-INFO
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      565 2023-05-03 14:36:43.000000 dbis-er-diagram-1.0.5/dbis_er_diagram.egg-info/SOURCES.txt
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)        1 2023-05-03 14:36:43.000000 dbis-er-diagram-1.0.5/dbis_er_diagram.egg-info/dependency_links.txt
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)       48 2023-05-03 14:36:43.000000 dbis-er-diagram-1.0.5/dbis_er_diagram.egg-info/requires.txt
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)       10 2023-05-03 14:36:43.000000 dbis-er-diagram-1.0.5/dbis_er_diagram.egg-info/top_level.txt
-drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-05-03 14:36:43.580057 dbis-er-diagram-1.0.5/erdiagram/
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      246 2023-05-03 13:33:48.000000 dbis-er-diagram-1.0.5/erdiagram/__init__.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     7697 2023-05-03 13:33:48.000000 dbis-er-diagram-1.0.5/erdiagram/drawing.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    38914 2023-05-03 13:33:48.000000 dbis-er-diagram-1.0.5/erdiagram/er.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    31969 2023-05-03 14:36:33.000000 dbis-er-diagram-1.0.5/erdiagram/grading.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     6591 2023-05-03 13:33:48.000000 dbis-er-diagram-1.0.5/erdiagram/merging.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      306 2023-05-03 13:33:48.000000 dbis-er-diagram-1.0.5/erdiagram/node_type.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      881 2023-05-03 14:36:33.000000 dbis-er-diagram-1.0.5/pyproject.toml
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)       38 2023-05-03 14:36:43.581057 dbis-er-diagram-1.0.5/setup.cfg
-drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-05-03 14:36:43.580057 dbis-er-diagram-1.0.5/tests/
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     5117 2023-05-03 13:33:48.000000 dbis-er-diagram-1.0.5/tests/test_adders.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1728 2023-05-03 13:33:48.000000 dbis-er-diagram-1.0.5/tests/test_drawing.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    11855 2023-05-03 13:33:48.000000 dbis-er-diagram-1.0.5/tests/test_getters.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1916 2023-05-03 13:33:48.000000 dbis-er-diagram-1.0.5/tests/test_grading_components.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     7118 2023-05-03 13:33:48.000000 dbis-er-diagram-1.0.5/tests/test_grading_diagrams.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     3617 2023-05-03 14:36:33.000000 dbis-er-diagram-1.0.5/tests/test_grading_special_cases.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1148 2023-05-03 13:33:48.000000 dbis-er-diagram-1.0.5/tests/test_merging.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1035 2023-05-03 13:33:48.000000 dbis-er-diagram-1.0.5/tests/test_other_methods.py
+drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-05-08 16:16:32.493008 dbis-er-diagram-1.0.6/
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    11357 2023-05-03 13:33:48.000000 dbis-er-diagram-1.0.6/LICENSE
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    15713 2023-05-08 16:16:32.493008 dbis-er-diagram-1.0.6/PKG-INFO
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    15133 2023-05-03 13:33:48.000000 dbis-er-diagram-1.0.6/README.md
+drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-05-08 16:16:32.492008 dbis-er-diagram-1.0.6/dbis_er_diagram.egg-info/
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    15713 2023-05-08 16:16:32.000000 dbis-er-diagram-1.0.6/dbis_er_diagram.egg-info/PKG-INFO
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      565 2023-05-08 16:16:32.000000 dbis-er-diagram-1.0.6/dbis_er_diagram.egg-info/SOURCES.txt
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)        1 2023-05-08 16:16:32.000000 dbis-er-diagram-1.0.6/dbis_er_diagram.egg-info/dependency_links.txt
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)       48 2023-05-08 16:16:32.000000 dbis-er-diagram-1.0.6/dbis_er_diagram.egg-info/requires.txt
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)       10 2023-05-08 16:16:32.000000 dbis-er-diagram-1.0.6/dbis_er_diagram.egg-info/top_level.txt
+drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-05-08 16:16:32.493008 dbis-er-diagram-1.0.6/erdiagram/
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      246 2023-05-03 13:33:48.000000 dbis-er-diagram-1.0.6/erdiagram/__init__.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     7697 2023-05-03 13:33:48.000000 dbis-er-diagram-1.0.6/erdiagram/drawing.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    38914 2023-05-03 13:33:48.000000 dbis-er-diagram-1.0.6/erdiagram/er.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    30589 2023-05-08 16:14:48.000000 dbis-er-diagram-1.0.6/erdiagram/grading.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     6591 2023-05-03 13:33:48.000000 dbis-er-diagram-1.0.6/erdiagram/merging.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      306 2023-05-03 13:33:48.000000 dbis-er-diagram-1.0.6/erdiagram/node_type.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      881 2023-05-08 16:14:48.000000 dbis-er-diagram-1.0.6/pyproject.toml
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)       38 2023-05-08 16:16:32.493008 dbis-er-diagram-1.0.6/setup.cfg
+drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-05-08 16:16:32.493008 dbis-er-diagram-1.0.6/tests/
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     5117 2023-05-03 13:33:48.000000 dbis-er-diagram-1.0.6/tests/test_adders.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1728 2023-05-03 13:33:48.000000 dbis-er-diagram-1.0.6/tests/test_drawing.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    11855 2023-05-03 13:33:48.000000 dbis-er-diagram-1.0.6/tests/test_getters.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1916 2023-05-04 14:27:55.000000 dbis-er-diagram-1.0.6/tests/test_grading_components.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     7118 2023-05-03 13:33:48.000000 dbis-er-diagram-1.0.6/tests/test_grading_diagrams.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    10304 2023-05-08 16:14:48.000000 dbis-er-diagram-1.0.6/tests/test_grading_special_cases.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1148 2023-05-03 13:33:48.000000 dbis-er-diagram-1.0.6/tests/test_merging.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1035 2023-05-03 13:33:48.000000 dbis-er-diagram-1.0.6/tests/test_other_methods.py
```

### Comparing `dbis-er-diagram-1.0.5/LICENSE` & `dbis-er-diagram-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dbis-er-diagram-1.0.5/PKG-INFO` & `dbis-er-diagram-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbis-er-diagram
-Version: 1.0.5
+Version: 1.0.6
 Summary: RWTH Aachen Computer Science i5/dbis assets for Lecture Datenbanken und Informationssysteme
 Author-email: Michal Slupczynski <slupczynski@dbis.rwth-aachen.de>, Beyza Akyüz <beyza.akyuez@rwth-aachen.de>, Til Mohr <til.mohr@rwth-aachen.de>
 Project-URL: Homepage, https://git.rwth-aachen.de/i5/teaching/dbis/dbis-er-diagram
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `dbis-er-diagram-1.0.5/README.md` & `dbis-er-diagram-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `dbis-er-diagram-1.0.5/dbis_er_diagram.egg-info/PKG-INFO` & `dbis-er-diagram-1.0.6/dbis_er_diagram.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbis-er-diagram
-Version: 1.0.5
+Version: 1.0.6
 Summary: RWTH Aachen Computer Science i5/dbis assets for Lecture Datenbanken und Informationssysteme
 Author-email: Michal Slupczynski <slupczynski@dbis.rwth-aachen.de>, Beyza Akyüz <beyza.akyuez@rwth-aachen.de>, Til Mohr <til.mohr@rwth-aachen.de>
 Project-URL: Homepage, https://git.rwth-aachen.de/i5/teaching/dbis/dbis-er-diagram
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `dbis-er-diagram-1.0.5/dbis_er_diagram.egg-info/SOURCES.txt` & `dbis-er-diagram-1.0.6/dbis_er_diagram.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbis-er-diagram-1.0.5/erdiagram/drawing.py` & `dbis-er-diagram-1.0.6/erdiagram/drawing.py`

 * *Files identical despite different names*

### Comparing `dbis-er-diagram-1.0.5/erdiagram/er.py` & `dbis-er-diagram-1.0.6/erdiagram/er.py`

 * *Files identical despite different names*

### Comparing `dbis-er-diagram-1.0.5/erdiagram/grading.py` & `dbis-er-diagram-1.0.6/erdiagram/grading.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 from typeguard import typechecked
 from Levenshtein import ratio, setratio
 from typing import Optional, Any
+import copy
 
 import erdiagram
 
 scores = dict()
 ratio_threshold = 0
 
 
@@ -206,37 +207,57 @@
         log += f"\t✗ Entity '{solution_label}' not found in submission. ({scores['missing_entity']})\n"
         score += scores["missing_entity"]
 
     return score, log
 
 
 @typechecked
-def __parse_cardinality(s: str) -> int | str | tuple[int | str, int | str]:
+def __parse_cardinality(s: str) -> Optional[int | str | tuple[int | str, int | str]]:
     """
     Parses a string and returns the corresponding value.
+
+    Parameters
+    ----------
+    s : str
+        The string to parse.
+
+    Returns
+    -------
+    Optional[int | str | tuple[int | str, int | str]]
+        The parsed value. None if the string could not be parsed.
     """
     # Remove any whitespace from the string
-    s = s.strip()
+    s = s.replace(" ", "")
+
+    # To lowercase
+    s = s.lower()
 
     if s.isdigit():
         # The string represents an integer
         return int(s)
     elif s.isalpha():
         # The string represents a single character string
         return s
     elif s.startswith("(") and s.endswith(")"):
         # The string represents a tuple of two values
         parts = s[1:-1].split(",")
         if len(parts) != 2:
-            raise ValueError("String does not represent a tuple of two values.")
+            return None
         val1 = parts[0].strip()
         val2 = parts[1].strip()
-        return (val1, val2)
+        if val1.isdigit() and val2.isdigit():
+            return (int(val1), int(val2))
+        elif val1.isdigit() and val2.isalpha():
+            return (int(val1), val2)
+        elif val1.isalpha() and val2.isdigit():
+            return (val1, int(val2))
+        else:
+            return (val1, val2)
     else:
-        raise ValueError("String could not be parsed.")
+        return None
 
 
 @typechecked
 def _grade_relation_pair(
     relation_pair: tuple[dict[str, Any], dict[str, Any]],
     solution: erdiagram.ER,
     submission: erdiagram.ER,
@@ -277,185 +298,168 @@
     from_entities_solution = transform_dict_to_list(solution_relation["from_entities"])
     from_entities_submission = transform_dict_to_list(
         submission_relation["from_entities"]
     )
     to_entities_solution = transform_dict_to_list(solution_relation["to_entities"])
     to_entities_submission = transform_dict_to_list(submission_relation["to_entities"])
 
-    # match from entities based on highest label ratio as tuples (solution, submission)
-    from_entity_pairs = []
-    for solution_from_entity in from_entities_solution:
-        from_entity_pairs.append(
-            (
-                solution_from_entity,
-                max(
-                    from_entities_submission,
-                    key=lambda submission_from_entity: ratio(
-                        sanitize(solution_from_entity["label"]),
-                        sanitize(submission_from_entity["label"]),
-                    ),
-                ),
-            )
-        )
-    to_entity_pairs = []
-    for solution_to_entity in to_entities_solution:
-        to_entity_pairs.append(
-            (
-                solution_to_entity,
-                max(
-                    to_entities_submission,
-                    key=lambda submission_to_entity: ratio(
-                        sanitize(solution_to_entity["label"]),
-                        sanitize(submission_to_entity["label"]),
-                    ),
-                ),
-            )
-        )
-
-    cardinality_letter_map = dict()
+    entities_solution = from_entities_solution + to_entities_solution
+    entities_submission = from_entities_submission + to_entities_submission
 
-    for solution_from_entity, submission_from_entity in from_entity_pairs:
-        original_solution_from_entity_label = solution_from_entity["label"]
-        original_submission_from_entity_label = submission_from_entity["label"]
-        solution_from_entity_label = sanitize(original_solution_from_entity_label)
-        submission_from_entity_label = sanitize(original_submission_from_entity_label)
-        label_ratio = ratio(solution_from_entity_label, submission_from_entity_label)
-        if label_ratio < ratio_threshold:
-            score += scores["missing_relation_property"] * 3
-            log += f"\t✗ Relation '{original_solution_label}' should have a from entity '{original_solution_from_entity_label}'. ({scores['missing_relation_property'] * 3})\n"
-            continue
+    entity_pairs_dict = (
+        list()
+    )  # from solution entity find all possible submission entities
+    for solution_entity in entities_solution:
+        candidates = []
+        for submission_entity in entities_submission:
+            if (
+                ratio(
+                    sanitize(solution_entity["label"]),
+                    sanitize(submission_entity["label"]),
+                )
+                > 0.8
+            ):
+                candidates.append(submission_entity)
+        entity_pairs_dict.append((solution_entity, candidates))
+
+    # sort above dictionary by length of value list, ascending, to a list of tuple(key, list)
+    entity_pairs = sorted(entity_pairs_dict, key=lambda x: len(x[1]))
+
+    def grade_relation_entity_pair(
+        solution_entity: dict[str, Any],
+        submission_entity: dict[str, Any],
+        cardinality_letter_map: dict[str, str],
+    ) -> tuple[tuple[float, str], dict[str, str]]:
+        score = 0.0
+        log = ""
+        cardinality_letter_map = copy.deepcopy(cardinality_letter_map)
+
+        original_solution_entity_label = solution_entity["label"]
+        original_submission_entity_label = submission_entity["label"]
+        solution_entity_label = sanitize(original_solution_entity_label)
+        submission_entity_label = sanitize(original_submission_entity_label)
+        label_ratio = ratio(solution_entity_label, submission_entity_label)
 
-        log += f"\t✓ Relation '{original_solution_label}' has a from entity '{original_solution_from_entity_label}' comparable to '{original_submission_from_entity_label}' with a label ratio of {label_ratio:.2f}.\n"
+        log += f"\t✓ Relation '{original_solution_label}' has an entity '{original_solution_entity_label}' comparable to '{original_submission_entity_label}' with a label ratio of {label_ratio:.2f}.\n"
 
         # check for the same cardinality
-        solution_from_entity_cardinality = __parse_cardinality(
-            str(solution_from_entity["cardinality"]).replace(" ", "")
+        solution_entity_cardinality = __parse_cardinality(
+            str(solution_entity["cardinality"])
         )
-        submission_from_entity_cardinality = __parse_cardinality(
-            str(submission_from_entity["cardinality"]).replace(" ", "")
+        submission_entity_cardinality = __parse_cardinality(
+            str(submission_entity["cardinality"])
         )
 
-        # if both are strings
-        if isinstance(solution_from_entity_cardinality, str) and isinstance(
-            submission_from_entity_cardinality, str
+        # check if we can map the cardinality letter to the solution cardinality, and if so, map it
+        if isinstance(solution_entity_cardinality, str) and isinstance(
+            submission_entity_cardinality, str
         ):
-            # check if there exists a cardinality letter mapping for the solution cardinality
-            if submission_from_entity_cardinality not in cardinality_letter_map:
+            if submission_entity_cardinality not in cardinality_letter_map:
                 cardinality_letter_map[
-                    submission_from_entity_cardinality
-                ] = solution_from_entity_cardinality
-
-            submission_from_entity_cardinality = cardinality_letter_map[
-                submission_from_entity_cardinality
+                    submission_entity_cardinality
+                ] = solution_entity_cardinality
+            submission_entity_cardinality = cardinality_letter_map[
+                submission_entity_cardinality
             ]
-
-        # if both a tuples
-        if isinstance(solution_from_entity_cardinality, tuple) and isinstance(
-            submission_from_entity_cardinality, tuple
+        elif isinstance(solution_entity_cardinality, tuple) and isinstance(
+            submission_entity_cardinality, tuple
         ):
-            # do the above, but for each index
-            assert (
-                len(solution_from_entity_cardinality)
-                == len(submission_from_entity_cardinality)
-                == 2
-            )
             new_submission_cardinality_tuple = []
             for index in range(2):
-                if (
-                    submission_from_entity_cardinality[index]
-                    not in cardinality_letter_map
-                ):
-                    cardinality_letter_map[
-                        submission_from_entity_cardinality[index]
-                    ] = solution_from_entity_cardinality[index]
-                new_submission_cardinality_tuple.append(
-                    cardinality_letter_map[submission_from_entity_cardinality[index]]
-                )
-            submission_from_entity_cardinality = tuple(new_submission_cardinality_tuple)
+                sol_idx = solution_entity_cardinality[index]
+                sub_idx = submission_entity_cardinality[index]
+                if isinstance(sol_idx, str) and isinstance(sub_idx, str):
+                    if sub_idx not in cardinality_letter_map:
+                        cardinality_letter_map[sub_idx] = sol_idx
+                    new_submission_cardinality_tuple.append(
+                        cardinality_letter_map[sub_idx]
+                    )
+                else:
+                    new_submission_cardinality_tuple.append(sub_idx)
+            submission_entity_cardinality = tuple(new_submission_cardinality_tuple)
 
-        if solution_from_entity_cardinality != submission_from_entity_cardinality:
+        # Check if the cardinality is the same
+        if solution_entity_cardinality != submission_entity_cardinality:
             score += scores["missing_relation_property"]
-            log += f"\t✗ Relation '{original_solution_label}' should have a from entity '{original_solution_from_entity_label}' with cardinality '{solution_from_entity_cardinality}', but has '{submission_from_entity_cardinality}'. ({scores['missing_relation_property']})\n"
+            log += f"\t✗ Relation '{original_solution_label}' should have an entity '{original_solution_entity_label}' with cardinality '{solution_entity_cardinality}', but has '{submission_entity_cardinality}'. ({scores['missing_relation_property']})\n"
 
         # check for the same is_weak
-        solution_from_entity_is_weak = solution_from_entity["is_weak"]
-        submission_from_entity_is_weak = submission_from_entity["is_weak"]
-        if solution_from_entity_is_weak != submission_from_entity_is_weak:
+        solution_entity_is_weak = solution_entity["is_weak"]
+        submission_entity_is_weak = submission_entity["is_weak"]
+        if solution_entity_is_weak != submission_entity_is_weak:
             score += scores["missing_relation_property"]
-            log += f"\t✗ Relation '{original_solution_label}' should have a from entity '{original_solution_from_entity_label}' {'weak' if solution_from_entity_is_weak else 'not weak'}, but is {'weak' if submission_from_entity_is_weak else 'not weak'}. ({scores['missing_relation_property']})\n"
-
-    for solution_to_entity, submission_to_entity in to_entity_pairs:
-        original_solution_to_entity_label = solution_to_entity["label"]
-        original_submission_to_entity_label = submission_to_entity["label"]
-        solution_to_entity_label = sanitize(original_solution_to_entity_label)
-        submission_to_entity_label = sanitize(original_submission_to_entity_label)
-        label_ratio = ratio(solution_to_entity_label, submission_to_entity_label)
-        if label_ratio < ratio_threshold:
-            score += scores["missing_relation_property"] * 3
-            log += f"\t✗ Relation '{original_solution_label}' should have a to entity '{original_solution_to_entity_label}'. ({scores['missing_relation_property'] * 3})\n"
-            continue
+            log += f"\t✗ Relation '{original_solution_label}' should be connected to entity '{original_solution_entity_label}' {'weak' if solution_entity_is_weak else 'not weak'}, but is {'weak' if submission_entity_is_weak else 'not weak'}. ({scores['missing_relation_property']})\n"
 
-        log += f"\t✓ Relation '{original_solution_label}' has a to entity '{original_solution_to_entity_label}' comparable to '{original_submission_to_entity_label}' with a label ratio of {label_ratio:.2f}.\n"
+        return ((score, log), cardinality_letter_map)
 
-        # check for the same cardinality
-        solution_to_entity_cardinality = __parse_cardinality(
-            str(solution_to_entity["cardinality"]).replace(" ", "")
-        )
-        submission_to_entity_cardinality = __parse_cardinality(
-            str(submission_to_entity["cardinality"]).replace(" ", "")
-        )
+    def grade_all_relation_entity_pairs(
+        entity_pairs: list[tuple[dict[str, Any], list[dict[str, Any]]]],
+        already_matched_submission_entities: list[dict[str, Any]],
+        cardinality_letter_map: dict[str, str],
+    ) -> tuple[float, str]:
+        entity_pairs = copy.deepcopy(entity_pairs)
+        already_matched_submission_entities = copy.deepcopy(
+            already_matched_submission_entities
+        )
+        score = 0.0
+        log = ""
+        cardinality_letter_map = copy.deepcopy(cardinality_letter_map)
+
+        if len(entity_pairs) == 0:
+            return (score, log)
+
+        # pop first pair
+        solution_entity, submission_entities = entity_pairs.pop(0)
+        original_solution_entity_label = solution_entity["label"]
+
+        # remove alrady matched entities from submission_entities
+        submission_entities = [
+            entity
+            for entity in submission_entities
+            if entity not in already_matched_submission_entities
+        ]
 
-        # if both are strings
-        if isinstance(solution_to_entity_cardinality, str) and isinstance(
-            submission_to_entity_cardinality, str
-        ):
-            # check if there exists a cardinality letter mapping for the solution cardinality
-            if submission_to_entity_cardinality not in cardinality_letter_map:
-                cardinality_letter_map[
-                    submission_to_entity_cardinality
-                ] = solution_to_entity_cardinality
+        if len(submission_entities) == 0:
+            score += scores["missing_relation_property"] * 3
+            log += f"\t✗ Relation '{original_solution_label}' should have an entity '{original_solution_entity_label}'. ({scores['missing_relation_property'] * 3})\n"
+            remaining_score, remaining_log = grade_all_relation_entity_pairs(
+                entity_pairs,
+                already_matched_submission_entities,
+                cardinality_letter_map,
+            )
+            return (score + remaining_score, log + remaining_log)
 
-            submission_to_entity_cardinality = cardinality_letter_map[
-                submission_to_entity_cardinality
-            ]
+        branches = []
+        for submission_entity in submission_entities:
+            branch = grade_relation_entity_pair(
+                solution_entity, submission_entity, cardinality_letter_map
+            )
+            branches.append((branch, submission_entity))
 
-        # if both a tuples
-        if isinstance(solution_to_entity_cardinality, tuple) and isinstance(
-            submission_to_entity_cardinality, tuple
-        ):
-            # do the above, but for each index
-            assert (
-                len(solution_to_entity_cardinality)
-                == len(submission_to_entity_cardinality)
-                == 2
+        # grade remaining entity pairs recursively
+        graded_branches = []
+        for (
+            (current_score, current_log),
+            current_cardinality_letter_map,
+        ), submission_entity in list(branches):
+            remaining_score, remaining_log = grade_all_relation_entity_pairs(
+                entity_pairs,
+                already_matched_submission_entities + [submission_entity],
+                current_cardinality_letter_map,
+            )
+            graded_branches.append(
+                (current_score + remaining_score, current_log + remaining_log)
             )
-            new_submission_cardinality_tuple = []
-            for index in range(2):
-                if (
-                    submission_to_entity_cardinality[index]
-                    not in cardinality_letter_map
-                ):
-                    cardinality_letter_map[
-                        submission_to_entity_cardinality[index]
-                    ] = solution_to_entity_cardinality[index]
-                new_submission_cardinality_tuple.append(
-                    cardinality_letter_map[submission_to_entity_cardinality[index]]
-                )
-            submission_to_entity_cardinality = tuple(new_submission_cardinality_tuple)
 
-        if solution_to_entity_cardinality != submission_to_entity_cardinality:
-            score += scores["missing_relation_property"]
-            log += f"\t✗ Relation '{original_solution_label}' should have a to entity '{original_solution_to_entity_label}' with cardinality '{solution_to_entity_cardinality}', but has '{submission_to_entity_cardinality}'. ({scores['missing_relation_property']})\n"
+        # get best branch by min score
+        best_branch = min(graded_branches, key=lambda x: x[0])
 
-        # check for the same is_weak
-        solution_to_entity_is_weak = solution_to_entity["is_weak"]
-        submission_to_entity_is_weak = submission_to_entity["is_weak"]
-        if solution_to_entity_is_weak != submission_to_entity_is_weak:
-            score += scores["missing_relation_property"]
-            log += f"\t✗ Relation '{original_solution_label}' should have a to entity '{original_solution_to_entity_label}' {'weak' if solution_to_entity_is_weak else 'not weak'}, but is {'weak' if submission_to_entity_is_weak else 'not weak'}. ({scores['missing_relation_property']})\n"
+        return best_branch
+
+    score, log = grade_all_relation_entity_pairs(entity_pairs, list(), dict())
 
     return score, log
 
 
 @typechecked
 def _grade_relations(
     solution: erdiagram.ER, submission: erdiagram.ER
@@ -708,15 +712,18 @@
         # check if `is_pk`, `is_multiple`, and `is_weak` are the same
         if solution_attribute["is_pk"] != submission_attribute[0]["is_pk"]:
             log += f"\t✗ The attribute {solution_attribute_label} of {str(solution_parent_type).lower()} {solution_parent_label} should{'' if solution_attribute['is_pk'] else ' not'} be a primary key. ({scores['missing_attribute_property']})\n"
             score += scores["missing_attribute_property"]
         if solution_attribute["is_multiple"] != submission_attribute[0]["is_multiple"]:
             log += f"\t✗ The attribute {solution_attribute_label} of {str(solution_parent_type).lower()} {solution_parent_label} should{'' if solution_attribute['is_multiple'] else ' not'} be multiple. ({scores['missing_attribute_property']})\n"
             score += scores["missing_attribute_property"]
-        if solution_attribute["is_weak"] != submission_attribute[0]["is_weak"]:
+        if (
+            solution_attribute["is_pk"]
+            and solution_attribute["is_weak"] != submission_attribute[0]["is_weak"]
+        ):
             log += f"\t✗ The attribute {solution_attribute_label} of {str(solution_parent_type).lower()} {solution_parent_label} should{'' if solution_attribute['is_weak'] else ' not'} be weak. ({scores['missing_attribute_property']})\n"
             score += scores["missing_attribute_property"]
 
         solution_composed_attribute_labels = [
             sanitize(solution.get_label_by_id(composed_attribute_id))
             for composed_attribute_id in solution_attribute["composed_of_attribute_ids"]
         ]
```

### Comparing `dbis-er-diagram-1.0.5/erdiagram/merging.py` & `dbis-er-diagram-1.0.6/erdiagram/merging.py`

 * *Files identical despite different names*

### Comparing `dbis-er-diagram-1.0.5/pyproject.toml` & `dbis-er-diagram-1.0.6/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dbis-er-diagram"
-version = "1.0.5"
+version = "1.0.6"
 description = "RWTH Aachen Computer Science i5/dbis assets for Lecture Datenbanken und Informationssysteme"
 authors = [
 	{ name = "Michal Slupczynski", email = "slupczynski@dbis.rwth-aachen.de" },
 	{ name = "Beyza Akyüz", email = "beyza.akyuez@rwth-aachen.de" },
 	{ name = "Til Mohr", email = "til.mohr@rwth-aachen.de" },
 ]
 readme = "README.md"
```

### Comparing `dbis-er-diagram-1.0.5/tests/test_adders.py` & `dbis-er-diagram-1.0.6/tests/test_adders.py`

 * *Files identical despite different names*

### Comparing `dbis-er-diagram-1.0.5/tests/test_drawing.py` & `dbis-er-diagram-1.0.6/tests/test_drawing.py`

 * *Files identical despite different names*

### Comparing `dbis-er-diagram-1.0.5/tests/test_getters.py` & `dbis-er-diagram-1.0.6/tests/test_getters.py`

 * *Files identical despite different names*

### Comparing `dbis-er-diagram-1.0.5/tests/test_grading_components.py` & `dbis-er-diagram-1.0.6/tests/test_grading_components.py`

 * *Files identical despite different names*

### Comparing `dbis-er-diagram-1.0.5/tests/test_grading_diagrams.py` & `dbis-er-diagram-1.0.6/tests/test_grading_diagrams.py`

 * *Files identical despite different names*

### Comparing `dbis-er-diagram-1.0.5/tests/test_merging.py` & `dbis-er-diagram-1.0.6/tests/test_merging.py`

 * *Files identical despite different names*

### Comparing `dbis-er-diagram-1.0.5/tests/test_other_methods.py` & `dbis-er-diagram-1.0.6/tests/test_other_methods.py`

 * *Files identical despite different names*

