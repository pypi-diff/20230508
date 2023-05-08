# Comparing `tmp/pasmopy-0.4.4.tar.gz` & `tmp/pasmopy-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pasmopy-0.4.4.tar", last modified: Thu Feb  9 04:06:11 2023, max compression
+gzip compressed data, was "pasmopy-0.5.0.tar", last modified: Mon May  8 08:51:46 2023, max compression
```

## Comparing `pasmopy-0.4.4.tar` & `pasmopy-0.5.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-09 04:06:11.090765 pasmopy-0.4.4/
--rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-02-09 04:05:50.000000 pasmopy-0.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       59 2023-02-09 04:05:50.000000 pasmopy-0.4.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    19727 2023-02-09 04:06:11.090765 pasmopy-0.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5406 2023-02-09 04:05:50.000000 pasmopy-0.4.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-09 04:06:11.090765 pasmopy-0.4.4/pasmopy/
--rw-r--r--   0 runner    (1001) docker     (122)      407 2023-02-09 04:05:50.000000 pasmopy-0.4.4/pasmopy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6482 2023-02-09 04:05:50.000000 pasmopy-0.4.4/pasmopy/individualization.py
--rw-r--r--   0 runner    (1001) docker     (122)    14657 2023-02-09 04:05:50.000000 pasmopy-0.4.4/pasmopy/patient_model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-09 04:06:11.090765 pasmopy-0.4.4/pasmopy/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (122)       48 2023-02-09 04:05:50.000000 pasmopy-0.4.4/pasmopy/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5178 2023-02-09 04:05:50.000000 pasmopy-0.4.4/pasmopy/preprocessing/weighting_factors.py
--rw-r--r--   0 runner    (1001) docker     (122)    12334 2023-02-09 04:05:50.000000 pasmopy-0.4.4/pasmopy/validation.py
--rw-r--r--   0 runner    (1001) docker     (122)       22 2023-02-09 04:05:50.000000 pasmopy-0.4.4/pasmopy/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-09 04:06:11.090765 pasmopy-0.4.4/pasmopy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    19727 2023-02-09 04:06:11.000000 pasmopy-0.4.4/pasmopy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      456 2023-02-09 04:06:11.000000 pasmopy-0.4.4/pasmopy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-02-09 04:06:11.000000 pasmopy-0.4.4/pasmopy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      250 2023-02-09 04:06:11.000000 pasmopy-0.4.4/pasmopy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        8 2023-02-09 04:06:11.000000 pasmopy-0.4.4/pasmopy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     2261 2023-02-09 04:05:50.000000 pasmopy-0.4.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      176 2023-02-09 04:06:11.090765 pasmopy-0.4.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-09 04:06:11.090765 pasmopy-0.4.4/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     8308 2023-02-09 04:05:50.000000 pasmopy-0.4.4/tests/test_breast_cancer.py
--rw-r--r--   0 runner    (1001) docker     (122)     1432 2023-02-09 04:05:50.000000 pasmopy-0.4.4/tests/test_drug_response.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 08:51:46.505062 pasmopy-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-05-08 08:51:31.000000 pasmopy-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       59 2023-05-08 08:51:31.000000 pasmopy-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     6815 2023-05-08 08:51:46.505062 pasmopy-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5406 2023-05-08 08:51:31.000000 pasmopy-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 08:51:46.505062 pasmopy-0.5.0/pasmopy/
+-rw-r--r--   0 runner    (1001) docker     (122)      399 2023-05-08 08:51:31.000000 pasmopy-0.5.0/pasmopy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6480 2023-05-08 08:51:31.000000 pasmopy-0.5.0/pasmopy/individualization.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14657 2023-05-08 08:51:31.000000 pasmopy-0.5.0/pasmopy/patient_model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 08:51:46.505062 pasmopy-0.5.0/pasmopy/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (122)       48 2023-05-08 08:51:31.000000 pasmopy-0.5.0/pasmopy/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5178 2023-05-08 08:51:31.000000 pasmopy-0.5.0/pasmopy/preprocessing/weighting_factors.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12334 2023-05-08 08:51:31.000000 pasmopy-0.5.0/pasmopy/validation.py
+-rw-r--r--   0 runner    (1001) docker     (122)       22 2023-05-08 08:51:31.000000 pasmopy-0.5.0/pasmopy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 08:51:46.505062 pasmopy-0.5.0/pasmopy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     6815 2023-05-08 08:51:46.000000 pasmopy-0.5.0/pasmopy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      456 2023-05-08 08:51:46.000000 pasmopy-0.5.0/pasmopy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-08 08:51:46.000000 pasmopy-0.5.0/pasmopy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      246 2023-05-08 08:51:46.000000 pasmopy-0.5.0/pasmopy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        8 2023-05-08 08:51:46.000000 pasmopy-0.5.0/pasmopy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     2298 2023-05-08 08:51:31.000000 pasmopy-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      176 2023-05-08 08:51:46.505062 pasmopy-0.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 08:51:46.505062 pasmopy-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     8308 2023-05-08 08:51:31.000000 pasmopy-0.5.0/tests/test_breast_cancer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1432 2023-05-08 08:51:31.000000 pasmopy-0.5.0/tests/test_drug_response.py
```

### Comparing `pasmopy-0.4.4/LICENSE` & `pasmopy-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pasmopy-0.4.4/README.md` & `pasmopy-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `pasmopy-0.4.4/pasmopy/individualization.py` & `pasmopy-0.5.0/pasmopy/individualization.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,15 +133,15 @@
 
         Returns
         -------
         weighted_sum : Dict[str, float]
             Estimated protein levels after incorporating transcriptomic data.
         """
         weighted_sum = dict.fromkeys(self.gene_expression, 0.0)
-        for (protein, genes) in self.gene_expression.items():
+        for protein, genes in self.gene_expression.items():
             for gene in genes:
                 weighted_sum[protein] += (
                     x[self.parameters.index(self.prefix + gene)]
                     * self.expression_level.at[gene, id]
                 )
         return weighted_sum
```

### Comparing `pasmopy-0.4.4/pasmopy/patient_model.py` & `pasmopy-0.5.0/pasmopy/patient_model.py`

 * *Files identical despite different names*

### Comparing `pasmopy-0.4.4/pasmopy/preprocessing/weighting_factors.py` & `pasmopy-0.5.0/pasmopy/preprocessing/weighting_factors.py`

 * *Files identical despite different names*

### Comparing `pasmopy-0.4.4/pasmopy/validation.py` & `pasmopy-0.5.0/pasmopy/validation.py`

 * *Files identical despite different names*

### Comparing `pasmopy-0.4.4/pyproject.toml` & `pasmopy-0.5.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -2,32 +2,33 @@
 requires = ["setuptools >= 61.1.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pasmopy"
 description = "Patient-Specific Modeling in Python"
 readme = "README.md"
-license = {file = "LICENSE"}
+license = {text = "Apache-2.0"}
 authors = [
     {name = "Hiroaki Imoto"},
 ]
 maintainers = [
-    {name = "Hiroaki Imoto", email = "himoto@protein.osaka-u.ac.jp"},
+    {name = "Hiroaki Imoto", email = "hiroaki.imoto@ucd.ie"},
 ]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Science/Research",
     "Intended Audience :: Healthcare Industry",
     "License :: OSI Approved :: Apache Software License",
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Topic :: Scientific/Engineering",
     "Topic :: Scientific/Engineering :: Bio-Informatics",
     "Topic :: Scientific/Engineering :: Medical Science Apps.",
     "Topic :: Software Development",
     "Topic :: Software Development :: Libraries",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
@@ -40,22 +41,22 @@
     "scipy>=1.6",
     "tqdm>=4.50.2",
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 dev = [
-    "black==22.12.0",
+    "black==23.3.0",
     "flake8==6.0.0",
     "isort==5.12.0",
     "pre-commit",
     "pytest",
 ]
 docs = [
-    "sphinx>=5.1.1,<6",
+    "sphinx>=5.1.1",
     "sphinx_rtd_theme",
     "sphinx_autodoc_typehints>=1.10.3",
     "sphinxcontrib-bibtex>=2.2.0",
 ]
 
 [project.urls]
 repository = "https://github.com/pasmopy/pasmopy"
```

### Comparing `pasmopy-0.4.4/tests/test_breast_cancer.py` & `pasmopy-0.5.0/tests/test_breast_cancer.py`

 * *Files identical despite different names*

### Comparing `pasmopy-0.4.4/tests/test_drug_response.py` & `pasmopy-0.5.0/tests/test_drug_response.py`

 * *Files identical despite different names*

