# Comparing `tmp/cycparser-1.2.8.tar.gz` & `tmp/cycparser-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cycparser-1.2.8.tar", max compression
+gzip compressed data, was "cycparser-1.2.9.tar", max compression
```

## Comparing `cycparser-1.2.8.tar` & `cycparser-1.2.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0    35079 2022-07-18 02:06:37.880768 cycparser-1.2.8/LICENSE
--rw-r--r--   0        0        0     1901 2022-07-18 02:06:37.881768 cycparser-1.2.8/pyproject.toml
--rw-r--r--   0        0        0     3484 2022-07-18 02:06:37.881768 cycparser-1.2.8/src/cycparser/__init__.py
--rw-r--r--   0        0        0     2827 2022-07-18 02:06:37.881768 cycparser-1.2.8/src/cycparser/data.py
--rw-r--r--   0        0        0     6585 2022-07-18 02:06:37.881768 cycparser-1.2.8/src/cycparser/defaults.py
--rw-r--r--   0        0        0     1928 2022-07-18 02:06:37.881768 cycparser-1.2.8/src/cycparser/parsing/__init__.py
--rw-r--r--   0        0        0     3434 2022-07-18 02:06:37.881768 cycparser-1.2.8/src/cycparser/parsing/compounds.py
--rw-r--r--   0        0        0     2510 2022-07-18 02:06:37.881768 cycparser-1.2.8/src/cycparser/parsing/enzymes.py
--rw-r--r--   0        0        0     2747 2022-07-18 02:06:37.881768 cycparser-1.2.8/src/cycparser/parsing/monomer_annotation.py
--rw-r--r--   0        0        0      502 2022-07-18 02:06:37.881768 cycparser-1.2.8/src/cycparser/parsing/monomer_sequences.py
--rw-r--r--   0        0        0     1385 2022-07-18 02:06:37.881768 cycparser-1.2.8/src/cycparser/parsing/protein_complexes.py
--rw-r--r--   0        0        0     6625 2022-07-18 02:06:37.881768 cycparser-1.2.8/src/cycparser/parsing/reactions.py
--rw-r--r--   0        0        0     2038 2022-07-18 02:06:37.881768 cycparser-1.2.8/src/cycparser/parsing/shared.py
--rw-r--r--   0        0        0        0 2022-07-18 02:06:37.881768 cycparser-1.2.8/src/cycparser/py.typed
--rw-r--r--   0        0        0      954 2022-07-18 02:06:37.881768 cycparser-1.2.8/src/cycparser/repairing/__init__.py
--rw-r--r--   0        0        0      289 2022-07-18 02:06:37.881768 cycparser-1.2.8/src/cycparser/repairing/fix_add_important_cpds.py
--rw-r--r--   0        0        0     8538 2022-07-18 02:06:37.881768 cycparser-1.2.8/src/cycparser/repairing/fix_create_compartment_variants.py
--rw-r--r--   0        0        0     2188 2022-07-18 02:06:37.882768 cycparser-1.2.8/src/cycparser/repairing/fix_create_reaction_variants.py
--rw-r--r--   0        0        0      455 2022-07-18 02:06:37.882768 cycparser-1.2.8/src/cycparser/repairing/fix_filter_garbage.py
--rw-r--r--   0        0        0     1144 2022-07-18 02:06:37.882768 cycparser-1.2.8/src/cycparser/repairing/fix_get_gpr_association.py
--rw-r--r--   0        0        0      520 2022-07-18 02:06:37.882768 cycparser-1.2.8/src/cycparser/repairing/fix_get_highest_compound_type.py
--rw-r--r--   0        0        0      525 2022-07-18 02:06:37.882768 cycparser-1.2.8/src/cycparser/repairing/fix_get_kinetic_data.py
--rw-r--r--   0        0        0     1164 2022-07-18 02:06:37.882768 cycparser-1.2.8/src/cycparser/repairing/fix_set_reaction_stoichiometry.py
--rw-r--r--   0        0        0     1772 2022-07-18 02:06:37.882768 cycparser-1.2.8/src/cycparser/repairing/fix_unify_reaction_direction.py
--rw-r--r--   0        0        0     2416 2022-07-18 02:06:37.882768 cycparser-1.2.8/src/cycparser/utils.py
--rw-r--r--   0        0        0      716 1970-01-01 00:00:00.000000 cycparser-1.2.8/setup.py
--rw-r--r--   0        0        0      400 1970-01-01 00:00:00.000000 cycparser-1.2.8/PKG-INFO
+-rw-r--r--   0        0        0    35079 2022-08-01 02:07:03.381614 cycparser-1.2.9/LICENSE
+-rw-r--r--   0        0        0     1901 2022-08-01 02:07:03.382614 cycparser-1.2.9/pyproject.toml
+-rw-r--r--   0        0        0     3484 2022-08-01 02:07:03.382614 cycparser-1.2.9/src/cycparser/__init__.py
+-rw-r--r--   0        0        0     2827 2022-08-01 02:07:03.382614 cycparser-1.2.9/src/cycparser/data.py
+-rw-r--r--   0        0        0     6585 2022-08-01 02:07:03.382614 cycparser-1.2.9/src/cycparser/defaults.py
+-rw-r--r--   0        0        0     1928 2022-08-01 02:07:03.382614 cycparser-1.2.9/src/cycparser/parsing/__init__.py
+-rw-r--r--   0        0        0     3434 2022-08-01 02:07:03.382614 cycparser-1.2.9/src/cycparser/parsing/compounds.py
+-rw-r--r--   0        0        0     2510 2022-08-01 02:07:03.382614 cycparser-1.2.9/src/cycparser/parsing/enzymes.py
+-rw-r--r--   0        0        0     2747 2022-08-01 02:07:03.382614 cycparser-1.2.9/src/cycparser/parsing/monomer_annotation.py
+-rw-r--r--   0        0        0      502 2022-08-01 02:07:03.382614 cycparser-1.2.9/src/cycparser/parsing/monomer_sequences.py
+-rw-r--r--   0        0        0     1385 2022-08-01 02:07:03.382614 cycparser-1.2.9/src/cycparser/parsing/protein_complexes.py
+-rw-r--r--   0        0        0     6625 2022-08-01 02:07:03.382614 cycparser-1.2.9/src/cycparser/parsing/reactions.py
+-rw-r--r--   0        0        0     2038 2022-08-01 02:07:03.382614 cycparser-1.2.9/src/cycparser/parsing/shared.py
+-rw-r--r--   0        0        0        0 2022-08-01 02:07:03.382614 cycparser-1.2.9/src/cycparser/py.typed
+-rw-r--r--   0        0        0      954 2022-08-01 02:07:03.382614 cycparser-1.2.9/src/cycparser/repairing/__init__.py
+-rw-r--r--   0        0        0      289 2022-08-01 02:07:03.382614 cycparser-1.2.9/src/cycparser/repairing/fix_add_important_cpds.py
+-rw-r--r--   0        0        0     8538 2022-08-01 02:07:03.383614 cycparser-1.2.9/src/cycparser/repairing/fix_create_compartment_variants.py
+-rw-r--r--   0        0        0     2188 2022-08-01 02:07:03.383614 cycparser-1.2.9/src/cycparser/repairing/fix_create_reaction_variants.py
+-rw-r--r--   0        0        0      455 2022-08-01 02:07:03.383614 cycparser-1.2.9/src/cycparser/repairing/fix_filter_garbage.py
+-rw-r--r--   0        0        0     1144 2022-08-01 02:07:03.383614 cycparser-1.2.9/src/cycparser/repairing/fix_get_gpr_association.py
+-rw-r--r--   0        0        0      520 2022-08-01 02:07:03.383614 cycparser-1.2.9/src/cycparser/repairing/fix_get_highest_compound_type.py
+-rw-r--r--   0        0        0      525 2022-08-01 02:07:03.383614 cycparser-1.2.9/src/cycparser/repairing/fix_get_kinetic_data.py
+-rw-r--r--   0        0        0     1164 2022-08-01 02:07:03.383614 cycparser-1.2.9/src/cycparser/repairing/fix_set_reaction_stoichiometry.py
+-rw-r--r--   0        0        0     1772 2022-08-01 02:07:03.383614 cycparser-1.2.9/src/cycparser/repairing/fix_unify_reaction_direction.py
+-rw-r--r--   0        0        0     2416 2022-08-01 02:07:03.383614 cycparser-1.2.9/src/cycparser/utils.py
+-rw-r--r--   0        0        0      716 1970-01-01 00:00:00.000000 cycparser-1.2.9/setup.py
+-rw-r--r--   0        0        0      400 1970-01-01 00:00:00.000000 cycparser-1.2.9/PKG-INFO
```

### Comparing `cycparser-1.2.8/LICENSE` & `cycparser-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cycparser-1.2.8/pyproject.toml` & `cycparser-1.2.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cycparser"
-version = "1.2.8"
+version = "1.2.9"
 description = ""
 authors = ["Marvin van Aalst <marvin.vanaalst@gmail.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 gitchangelog = "^3.0.4"
```

### Comparing `cycparser-1.2.8/src/cycparser/__init__.py` & `cycparser-1.2.9/src/cycparser/__init__.py`

 * *Files identical despite different names*

### Comparing `cycparser-1.2.8/src/cycparser/data.py` & `cycparser-1.2.9/src/cycparser/data.py`

 * *Files identical despite different names*

### Comparing `cycparser-1.2.8/src/cycparser/defaults.py` & `cycparser-1.2.9/src/cycparser/defaults.py`

 * *Files identical despite different names*

### Comparing `cycparser-1.2.8/src/cycparser/parsing/__init__.py` & `cycparser-1.2.9/src/cycparser/parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `cycparser-1.2.8/src/cycparser/parsing/compounds.py` & `cycparser-1.2.9/src/cycparser/parsing/compounds.py`

 * *Files identical despite different names*

### Comparing `cycparser-1.2.8/src/cycparser/parsing/enzymes.py` & `cycparser-1.2.9/src/cycparser/parsing/enzymes.py`

 * *Files identical despite different names*

### Comparing `cycparser-1.2.8/src/cycparser/parsing/monomer_annotation.py` & `cycparser-1.2.9/src/cycparser/parsing/monomer_annotation.py`

 * *Files identical despite different names*

### Comparing `cycparser-1.2.8/src/cycparser/parsing/protein_complexes.py` & `cycparser-1.2.9/src/cycparser/parsing/protein_complexes.py`

 * *Files identical despite different names*

### Comparing `cycparser-1.2.8/src/cycparser/parsing/reactions.py` & `cycparser-1.2.9/src/cycparser/parsing/reactions.py`

 * *Files identical despite different names*

### Comparing `cycparser-1.2.8/src/cycparser/parsing/shared.py` & `cycparser-1.2.9/src/cycparser/parsing/shared.py`

 * *Files identical despite different names*

### Comparing `cycparser-1.2.8/src/cycparser/repairing/__init__.py` & `cycparser-1.2.9/src/cycparser/repairing/__init__.py`

 * *Files identical despite different names*

### Comparing `cycparser-1.2.8/src/cycparser/repairing/fix_create_compartment_variants.py` & `cycparser-1.2.9/src/cycparser/repairing/fix_create_compartment_variants.py`

 * *Files identical despite different names*

### Comparing `cycparser-1.2.8/src/cycparser/repairing/fix_create_reaction_variants.py` & `cycparser-1.2.9/src/cycparser/repairing/fix_create_reaction_variants.py`

 * *Files identical despite different names*

### Comparing `cycparser-1.2.8/src/cycparser/repairing/fix_get_gpr_association.py` & `cycparser-1.2.9/src/cycparser/repairing/fix_get_gpr_association.py`

 * *Files identical despite different names*

### Comparing `cycparser-1.2.8/src/cycparser/repairing/fix_get_highest_compound_type.py` & `cycparser-1.2.9/src/cycparser/repairing/fix_get_highest_compound_type.py`

 * *Files identical despite different names*

### Comparing `cycparser-1.2.8/src/cycparser/repairing/fix_get_kinetic_data.py` & `cycparser-1.2.9/src/cycparser/repairing/fix_get_kinetic_data.py`

 * *Files identical despite different names*

### Comparing `cycparser-1.2.8/src/cycparser/repairing/fix_set_reaction_stoichiometry.py` & `cycparser-1.2.9/src/cycparser/repairing/fix_set_reaction_stoichiometry.py`

 * *Files identical despite different names*

### Comparing `cycparser-1.2.8/src/cycparser/repairing/fix_unify_reaction_direction.py` & `cycparser-1.2.9/src/cycparser/repairing/fix_unify_reaction_direction.py`

 * *Files identical despite different names*

### Comparing `cycparser-1.2.8/src/cycparser/utils.py` & `cycparser-1.2.9/src/cycparser/utils.py`

 * *Files identical despite different names*

### Comparing `cycparser-1.2.8/setup.py` & `cycparser-1.2.9/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['gitchangelog>=3.0.4,<4.0.0']
 
 setup_kwargs = {
     'name': 'cycparser',
-    'version': '1.2.8',
+    'version': '1.2.9',
     'description': '',
     'long_description': 'None',
     'author': 'Marvin van Aalst',
     'author_email': 'marvin.vanaalst@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

