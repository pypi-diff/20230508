# Comparing `tmp/unpast-0.1.0.6.tar.gz` & `tmp/unpast-0.1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unpast-0.1.0.6.tar", max compression
+gzip compressed data, was "unpast-0.1.0.7.tar", max compression
```

## Comparing `unpast-0.1.0.6.tar` & `unpast-0.1.0.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    35149 2023-05-08 14:23:44.608899 unpast-0.1.0.6/LICENSE
--rw-r--r--   0        0        0     2782 2023-05-08 14:23:44.608899 unpast-0.1.0.6/README.md
--rw-r--r--   0        0        0      749 2023-05-08 18:08:05.278242 unpast-0.1.0.6/pyproject.toml
--rw-r--r--   0        0        0    56649 2023-05-08 16:15:10.047152 unpast-0.1.0.6/renv.lock
--rw-r--r--   0        0        0        0 2023-05-08 14:23:44.608899 unpast-0.1.0.6/unpast/__init__.py
--rw-r--r--   0        0        0    36567 2023-05-08 14:23:44.716900 unpast-0.1.0.6/unpast/method.py
--rw-r--r--   0        0        0    96439 2023-05-08 14:23:44.608899 unpast-0.1.0.6/unpast/notebooks/consensus.ipynb
--rw-r--r--   0        0        0   203026 2023-05-08 14:23:44.712900 unpast-0.1.0.6/unpast/notebooks/evaluation_on_real_data.ipynb
--rw-r--r--   0        0        0    47339 2023-05-08 14:23:44.716900 unpast-0.1.0.6/unpast/notebooks/evaluation_on_simulated_data.ipynb
--rw-r--r--   0        0        0    12705 2023-05-08 14:23:44.768901 unpast-0.1.0.6/unpast/notebooks/run_unpast_on_subsampled.ipynb
--rw-r--r--   0        0        0   397753 2023-05-08 14:23:44.768901 unpast-0.1.0.6/unpast/notebooks/survival_and_association_with_sex.ipynb
--rw-r--r--   0        0        0      146 2023-05-08 17:57:44.956465 unpast-0.1.0.6/unpast/restore_renv.R
--rw-r--r--   0        0        0      198 2023-05-08 18:03:57.263932 unpast-0.1.0.6/unpast/restore_renv.py
--rw-r--r--   0        0        0     4473 2023-05-08 17:57:19.040224 unpast-0.1.0.6/unpast/run_desmond.py
--rwxr-xr-x   0        0        0    12110 2023-05-08 18:07:55.646152 unpast-0.1.0.6/unpast/run_unpast.py
--rw-r--r--   0        0        0        0 2023-05-08 15:54:16.915484 unpast-0.1.0.6/unpast/utils/.Rhistory
--rw-r--r--   0        0        0        0 2023-05-08 14:23:44.768901 unpast-0.1.0.6/unpast/utils/__init__.py
--rw-r--r--   0        0        0      163 2023-05-08 15:31:35.482806 unpast-0.1.0.6/unpast/utils/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0    33532 2023-05-08 15:31:35.490806 unpast-0.1.0.6/unpast/utils/__pycache__/method.cpython-39.pyc
--rw-r--r--   0        0        0    25724 2023-05-08 14:23:44.768901 unpast-0.1.0.6/unpast/utils/eval.py
--rw-r--r--   0        0        0    57918 2023-05-08 14:23:44.768901 unpast-0.1.0.6/unpast/utils/method.py
--rw-r--r--   0        0        0    19957 2023-05-08 14:23:44.768901 unpast-0.1.0.6/unpast/utils/pgm.py
--rw-r--r--   0        0        0     1757 2023-05-08 14:23:44.768901 unpast-0.1.0.6/unpast/utils/run_WGCNA.R
--rw-r--r--   0        0        0     3890 1970-01-01 00:00:00.000000 unpast-0.1.0.6/setup.py
--rw-r--r--   0        0        0     3539 1970-01-01 00:00:00.000000 unpast-0.1.0.6/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-08 14:23:44.608899 unpast-0.1.0.7/LICENSE
+-rw-r--r--   0        0        0     2782 2023-05-08 14:23:44.608899 unpast-0.1.0.7/README.md
+-rw-r--r--   0        0        0      749 2023-05-08 18:10:41.095692 unpast-0.1.0.7/pyproject.toml
+-rw-r--r--   0        0        0    56649 2023-05-08 16:15:10.047152 unpast-0.1.0.7/renv.lock
+-rw-r--r--   0        0        0        0 2023-05-08 14:23:44.608899 unpast-0.1.0.7/unpast/__init__.py
+-rw-r--r--   0        0        0    36567 2023-05-08 14:23:44.716900 unpast-0.1.0.7/unpast/method.py
+-rw-r--r--   0        0        0    96439 2023-05-08 14:23:44.608899 unpast-0.1.0.7/unpast/notebooks/consensus.ipynb
+-rw-r--r--   0        0        0   203026 2023-05-08 14:23:44.712900 unpast-0.1.0.7/unpast/notebooks/evaluation_on_real_data.ipynb
+-rw-r--r--   0        0        0    47339 2023-05-08 14:23:44.716900 unpast-0.1.0.7/unpast/notebooks/evaluation_on_simulated_data.ipynb
+-rw-r--r--   0        0        0    12705 2023-05-08 14:23:44.768901 unpast-0.1.0.7/unpast/notebooks/run_unpast_on_subsampled.ipynb
+-rw-r--r--   0        0        0   397753 2023-05-08 14:23:44.768901 unpast-0.1.0.7/unpast/notebooks/survival_and_association_with_sex.ipynb
+-rw-r--r--   0        0        0      146 2023-05-08 17:57:44.956465 unpast-0.1.0.7/unpast/restore_renv.R
+-rw-r--r--   0        0        0      245 2023-05-08 18:10:32.099609 unpast-0.1.0.7/unpast/restore_renv.py
+-rw-r--r--   0        0        0     4473 2023-05-08 17:57:19.040224 unpast-0.1.0.7/unpast/run_desmond.py
+-rwxr-xr-x   0        0        0    12110 2023-05-08 18:07:55.646152 unpast-0.1.0.7/unpast/run_unpast.py
+-rw-r--r--   0        0        0        0 2023-05-08 15:54:16.915484 unpast-0.1.0.7/unpast/utils/.Rhistory
+-rw-r--r--   0        0        0        0 2023-05-08 14:23:44.768901 unpast-0.1.0.7/unpast/utils/__init__.py
+-rw-r--r--   0        0        0      163 2023-05-08 15:31:35.482806 unpast-0.1.0.7/unpast/utils/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0    33532 2023-05-08 15:31:35.490806 unpast-0.1.0.7/unpast/utils/__pycache__/method.cpython-39.pyc
+-rw-r--r--   0        0        0    25724 2023-05-08 14:23:44.768901 unpast-0.1.0.7/unpast/utils/eval.py
+-rw-r--r--   0        0        0    57918 2023-05-08 14:23:44.768901 unpast-0.1.0.7/unpast/utils/method.py
+-rw-r--r--   0        0        0    19957 2023-05-08 14:23:44.768901 unpast-0.1.0.7/unpast/utils/pgm.py
+-rw-r--r--   0        0        0     1757 2023-05-08 14:23:44.768901 unpast-0.1.0.7/unpast/utils/run_WGCNA.R
+-rw-r--r--   0        0        0     3890 1970-01-01 00:00:00.000000 unpast-0.1.0.7/setup.py
+-rw-r--r--   0        0        0     3539 1970-01-01 00:00:00.000000 unpast-0.1.0.7/PKG-INFO
```

### Comparing `unpast-0.1.0.6/LICENSE` & `unpast-0.1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `unpast-0.1.0.6/README.md` & `unpast-0.1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `unpast-0.1.0.6/pyproject.toml` & `unpast-0.1.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "unpast"
-version = "0.1.0.6"
+version = "0.1.0.7"
 description = "A novel method for unsupervised patient stratification."
 authors = []
 readme = "README.md"
 license = "GPL-3.0"
 include = ["renv.lock", "unpast/restore_renv.R"]
 
 [tool.poetry.dependencies]
```

### Comparing `unpast-0.1.0.6/renv.lock` & `unpast-0.1.0.7/renv.lock`

 * *Files identical despite different names*

### Comparing `unpast-0.1.0.6/unpast/method.py` & `unpast-0.1.0.7/unpast/method.py`

 * *Files identical despite different names*

### Comparing `unpast-0.1.0.6/unpast/notebooks/consensus.ipynb` & `unpast-0.1.0.7/unpast/notebooks/consensus.ipynb`

 * *Files identical despite different names*

### Comparing `unpast-0.1.0.6/unpast/notebooks/evaluation_on_real_data.ipynb` & `unpast-0.1.0.7/unpast/notebooks/evaluation_on_real_data.ipynb`

 * *Files identical despite different names*

### Comparing `unpast-0.1.0.6/unpast/notebooks/evaluation_on_simulated_data.ipynb` & `unpast-0.1.0.7/unpast/notebooks/evaluation_on_simulated_data.ipynb`

 * *Files identical despite different names*

### Comparing `unpast-0.1.0.6/unpast/notebooks/run_unpast_on_subsampled.ipynb` & `unpast-0.1.0.7/unpast/notebooks/run_unpast_on_subsampled.ipynb`

 * *Files identical despite different names*

### Comparing `unpast-0.1.0.6/unpast/notebooks/survival_and_association_with_sex.ipynb` & `unpast-0.1.0.7/unpast/notebooks/survival_and_association_with_sex.ipynb`

 * *Files identical despite different names*

### Comparing `unpast-0.1.0.6/unpast/run_desmond.py` & `unpast-0.1.0.7/unpast/run_desmond.py`

 * *Files identical despite different names*

### Comparing `unpast-0.1.0.6/unpast/run_unpast.py` & `unpast-0.1.0.7/unpast/run_unpast.py`

 * *Files identical despite different names*

### Comparing `unpast-0.1.0.6/unpast/utils/__pycache__/method.cpython-39.pyc` & `unpast-0.1.0.7/unpast/utils/__pycache__/method.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `unpast-0.1.0.6/unpast/utils/eval.py` & `unpast-0.1.0.7/unpast/utils/eval.py`

 * *Files identical despite different names*

### Comparing `unpast-0.1.0.6/unpast/utils/method.py` & `unpast-0.1.0.7/unpast/utils/method.py`

 * *Files identical despite different names*

### Comparing `unpast-0.1.0.6/unpast/utils/pgm.py` & `unpast-0.1.0.7/unpast/utils/pgm.py`

 * *Files identical despite different names*

### Comparing `unpast-0.1.0.6/unpast/utils/run_WGCNA.R` & `unpast-0.1.0.7/unpast/utils/run_WGCNA.R`

 * *Files identical despite different names*

### Comparing `unpast-0.1.0.6/setup.py` & `unpast-0.1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 entry_points = \
 {'console_scripts': ['restore_renv = unpast.restore_renv:main',
                      'run_desmond = unpast.run_desmond:main',
                      'run_unpast = unpast.run_unpast:main']}
 
 setup_kwargs = {
     'name': 'unpast',
-    'version': '0.1.0.6',
+    'version': '0.1.0.7',
     'description': 'A novel method for unsupervised patient stratification.',
     'long_description': '# UnPaSt\n\nUnPaSt is a novel method for identification of differentially expressed biclusters in gene expression matrix. It searches for gene sets up- or down-regulated in subsets of samples:\n\n![alt text](./poster/DESMOND2_steps2.png)\n\n\nWebserver: https://unpast.zbh.uni-hamburg.de/\n\n\n## Requirements:\n<pre>\nPython:\n    fisher==0.1.9\n    jenkspy==0.2.0\n    pandas==1.4.2\n    python-louvain==0.15\n    matplotlib-venn==0.11.6\n    numba==0.51.2\n    numpy==1.22.3\n    scikit-learn==0.23.1\n    scikit-network==0.24.0\n    scipy==1.7.1\n    statsmodels==0.13.2\n\nR:\n    WGCNA==1.70-3\n</pre>\n\n## Examples\n* UnPaSt requires a tab-separated file with standardized expressions of genes (or transcripts) in rows, and samples in columns. Gene and sample names must be unique. \n* A subset of 200 randomly chosen samples from TCGA-BRCA and UnPaSt output:\n[test data](https://drive.google.com/file/d/1GXR_1ErIPtQkEOxE66at0uqQN76qNG7a/view?usp=sharing)\n\n<pre>\n# running UnPaSt with default parameters and example data\npython run_unpast.py --exprs TCGA_200.exprs_z.tsv --basename TCGA_200_results\n\n# with different binarization and clustering methods\npython run_unpast.py --exprs TCGA_200.exprs_z.tsv --basename results --binarization ward --clustering WGCNA\n\n# help\npython run_unpast.py -h\n</pre>\n\n## Outputs\n* \\<basename\\>.bin=[GMM|Jenks],clust=[Louvain|WGCNA|DESMOND].biclusters.tsv - a .tsv table with found biclsuters, where \n    - avgSNR is average SNR over all genes in the biclusters\n    - columns "n_genes" and "n_samples" provide the numbers of genes and samples, respectively \n    - "gene","sample" contain gene and sample names respectively\n    - "gene_indexes" and  "sample_indexes" - 0-based gene and sample indexes in the input matrix.\n* binarized expressions, background distributions of SNR for each bicluster size and binarization statistics [if clustering is WGCNA,  or  \'--save_binary\' flag is added]\n* modules found by WGCNA [if clustering is WGCNA]\n\n## About \nUnPaSt is an unconstrained version of DESMOND method ([repository](https://github.com/ozolotareva/DESMOND), [publication](https://academic.oup.com/bioinformatics/article/37/12/1691/6039116?login=true))\n\nMajor modifications:\n * it does not require the network of gene interactions \n * UnPaSt clusters individual genes instead of gene pairs\n * uses Gaussian mixture models or Jenks method for binarization of individual gene expressions\n * SNR threshold is authomatically determined; it depends on bicluster size in samples and user-defined p-value cutoff\n \n## License\nFree for non-for-profit use. For commercial use please contact the developers. \n\n### Poster CDCS workshop\'22\n![./poster/DESMOND2_poster_v5.png](./poster/DESMOND2_poster_v5.png)\n### Poster ISMB and MCCMB\'21\n![./poster/DESMOND2.pdf](./poster/DESMOND2.png)\n',
     'author': 'None',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `unpast-0.1.0.6/PKG-INFO` & `unpast-0.1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unpast
-Version: 0.1.0.6
+Version: 0.1.0.7
 Summary: A novel method for unsupervised patient stratification.
 License: GPL-3.0
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

