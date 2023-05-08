# Comparing `tmp/classeval-0.2.0.tar.gz` & `tmp/classeval-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "classeval-0.2.0.tar", last modified: Thu Dec  1 19:12:20 2022, max compression
+gzip compressed data, was "classeval-0.2.1.tar", last modified: Mon May  8 17:31:38 2023, max compression
```

## Comparing `classeval-0.2.0.tar` & `classeval-0.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2022-12-01 19:12:20.056708 classeval-0.2.0/
--rw-rw-rw-   0        0        0     1122 2021-01-19 08:31:31.000000 classeval-0.2.0/LICENSE
--rw-rw-rw-   0        0        0       62 2021-01-19 08:31:31.000000 classeval-0.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0     5290 2022-12-01 19:12:20.056708 classeval-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     4737 2022-12-01 18:55:41.000000 classeval-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2022-12-01 19:12:20.048728 classeval-0.2.0/classeval/
--rw-rw-rw-   0        0        0    10775 2021-01-19 08:31:31.000000 classeval-0.2.0/classeval/ROC.py
--rw-rw-rw-   0        0        0     1758 2022-12-01 19:00:55.000000 classeval-0.2.0/classeval/__init__.py
--rw-rw-rw-   0        0        0    27963 2022-12-01 19:00:34.000000 classeval-0.2.0/classeval/classeval.py
--rw-rw-rw-   0        0        0     5138 2021-01-19 11:43:18.000000 classeval-0.2.0/classeval/confmatrix.py
-drwxrwxrwx   0        0        0        0 2022-12-01 19:12:20.056473 classeval-0.2.0/classeval/data/
--rw-rw-rw-   0        0        0        0 2021-01-19 08:31:31.000000 classeval-0.2.0/classeval/data/__init__.py
--rw-rw-rw-   0        0        0     3374 2022-12-01 18:59:06.000000 classeval-0.2.0/classeval/examples.py
-drwxrwxrwx   0        0        0        0 2022-12-01 19:12:20.055744 classeval-0.2.0/classeval.egg-info/
--rw-rw-rw-   0        0        0     5290 2022-12-01 19:12:19.000000 classeval-0.2.0/classeval.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      337 2022-12-01 19:12:19.000000 classeval-0.2.0/classeval.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-01 19:12:19.000000 classeval-0.2.0/classeval.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2022-12-01 19:12:19.000000 classeval-0.2.0/classeval.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2022-12-01 19:12:19.000000 classeval-0.2.0/classeval.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-12-01 19:12:20.057720 classeval-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1368 2022-03-11 12:58:52.000000 classeval-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 17:31:38.438897 classeval-0.2.1/
+-rw-rw-rw-   0        0        0     1122 2021-01-19 08:31:31.000000 classeval-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0       62 2021-01-19 08:31:31.000000 classeval-0.2.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     5249 2023-05-08 17:31:38.437908 classeval-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4737 2022-12-01 18:55:41.000000 classeval-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-08 17:31:38.424954 classeval-0.2.1/classeval/
+-rw-rw-rw-   0        0        0    10775 2021-01-19 08:31:31.000000 classeval-0.2.1/classeval/ROC.py
+-rw-rw-rw-   0        0        0     1758 2023-05-08 17:30:45.000000 classeval-0.2.1/classeval/__init__.py
+-rw-rw-rw-   0        0        0    27963 2022-12-01 19:00:34.000000 classeval-0.2.1/classeval/classeval.py
+-rw-rw-rw-   0        0        0     5138 2021-01-19 11:43:18.000000 classeval-0.2.1/classeval/confmatrix.py
+drwxrwxrwx   0        0        0        0 2023-05-08 17:31:38.436935 classeval-0.2.1/classeval/data/
+-rw-rw-rw-   0        0        0        0 2021-01-19 08:31:31.000000 classeval-0.2.1/classeval/data/__init__.py
+-rw-rw-rw-   0        0        0     3434 2023-05-08 17:29:54.000000 classeval-0.2.1/classeval/examples.py
+drwxrwxrwx   0        0        0        0 2023-05-08 17:31:38.432911 classeval-0.2.1/classeval.egg-info/
+-rw-rw-rw-   0        0        0     5249 2023-05-08 17:31:38.000000 classeval-0.2.1/classeval.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      337 2023-05-08 17:31:38.000000 classeval-0.2.1/classeval.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 17:31:38.000000 classeval-0.2.1/classeval.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2023-05-08 17:31:38.000000 classeval-0.2.1/classeval.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-08 17:31:38.000000 classeval-0.2.1/classeval.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-08 17:31:38.438897 classeval-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1392 2023-05-08 17:27:19.000000 classeval-0.2.1/setup.py
```

### Comparing `classeval-0.2.0/LICENSE` & `classeval-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `classeval-0.2.0/PKG-INFO` & `classeval-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: classeval
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python package classeval
 Home-page: https://erdogant.github.io/classeval/
-Download-URL: https://github.com/erdogant/classeval/archive/0.2.0.tar.gz
+Download-URL: https://github.com/erdogant/classeval/archive/0.2.1.tar.gz
 Author: Erdogan Taskesen
 Author-email: erdogant@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -107,9 +105,7 @@
 ### Citation
 Please cite ``classeval`` in your publications if this is useful for your research. See column right for citation information.
 
 ### Maintainer
 * Erdogan Taskesen, github: [erdogant](https://github.com/erdogant)
 * Contributions are welcome.
 * If you wish to buy me a <a href="https://erdogant.github.io/donate/?currency=USD&amount=5">Coffee</a> for this work, it is very appreciated :)
-
-
```

#### html2text {}

```diff
@@ -1,28 +1,27 @@
-Metadata-Version: 2.1 Name: classeval Version: 0.2.0 Summary: Python package
+Metadata-Version: 2.1 Name: classeval Version: 0.2.1 Summary: Python package
 classeval Home-page: https://erdogant.github.io/classeval/ Download-URL: https:
-//github.com/erdogant/classeval/archive/0.2.0.tar.gz Author: Erdogan Taskesen
-Author-email: erdogant@gmail.com License: UNKNOWN Platform: UNKNOWN Classifier:
-Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
-License Classifier: Operating System :: OS Independent Requires-Python: >=3
-Description-Content-Type: text/markdown License-File: LICENSE # classeval [!
-[Python](https://img.shields.io/pypi/pyversions/classeval)](https://
-img.shields.io/pypi/pyversions/classeval) [![PyPI Version](https://
-img.shields.io/pypi/v/classeval)](https://pypi.org/project/classeval/) [!
-[License](https://img.shields.io/badge/license-MIT-green.svg)](https://
-github.com/erdogant/classeval/blob/master/LICENSE) [![Forks](https://
-img.shields.io/github/forks/erdogant/classeval.svg)](https://github.com/
-erdogant/classeval/network) [![Open Issues](https://img.shields.io/github/
-issues/erdogant/classeval.svg)](https://github.com/erdogant/classeval/issues)
-[![Project Status](http://www.repostatus.org/badges/latest/active.svg)](http://
-www.repostatus.org/#active) [![Downloads](https://pepy.tech/badge/classeval/
-month)](https://pepy.tech/project/classeval/) [![Downloads](https://pepy.tech/
-badge/classeval)](https://pepy.tech/project/classeval) [![DOI](https://
-zenodo.org/badge/246504758.svg)](https://zenodo.org/badge/latestdoi/246504758)
-[![Docs](https://img.shields.io/badge/Sphinx-Docs-Green)](https://
+//github.com/erdogant/classeval/archive/0.2.1.tar.gz Author: Erdogan Taskesen
+Author-email: erdogant@gmail.com Classifier: Programming Language :: Python ::
+3 Classifier: License :: OSI Approved :: MIT License Classifier: Operating
+System :: OS Independent Requires-Python: >=3 Description-Content-Type: text/
+markdown License-File: LICENSE # classeval [![Python](https://img.shields.io/
+pypi/pyversions/classeval)](https://img.shields.io/pypi/pyversions/classeval)
+[![PyPI Version](https://img.shields.io/pypi/v/classeval)](https://pypi.org/
+project/classeval/) [![License](https://img.shields.io/badge/license-MIT-
+green.svg)](https://github.com/erdogant/classeval/blob/master/LICENSE) [!
+[Forks](https://img.shields.io/github/forks/erdogant/classeval.svg)](https://
+github.com/erdogant/classeval/network) [![Open Issues](https://img.shields.io/
+github/issues/erdogant/classeval.svg)](https://github.com/erdogant/classeval/
+issues) [![Project Status](http://www.repostatus.org/badges/latest/active.svg)]
+(http://www.repostatus.org/#active) [![Downloads](https://pepy.tech/badge/
+classeval/month)](https://pepy.tech/project/classeval/) [![Downloads](https://
+pepy.tech/badge/classeval)](https://pepy.tech/project/classeval) [![DOI](https:
+//zenodo.org/badge/246504758.svg)](https://zenodo.org/badge/latestdoi/
+246504758) [![Docs](https://img.shields.io/badge/Sphinx-Docs-Green)](https://
 erdogant.github.io/classeval/) [![Donate](https://img.shields.io/badge/
 Support%20this%20project-grey.svg?logo=github%20sponsors)](https://
 erdogant.github.io/classeval/pages/html/Documentation.html#)   The library
 ``classeval`` is developed to evaluate the models performance of any kind of
 **two-class** or **multi-class** model. ``classeval`` computes many scoring
 measures in case of a two-class clasification model. Some measures are utilized
 from ``sklearn``, among them AUC, MCC, Cohen kappa score, matthews correlation
```

### Comparing `classeval-0.2.0/README.md` & `classeval-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `classeval-0.2.0/classeval/ROC.py` & `classeval-0.2.1/classeval/ROC.py`

 * *Files identical despite different names*

### Comparing `classeval-0.2.0/classeval/__init__.py` & `classeval-0.2.1/classeval/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 )
 
 import classeval.confmatrix as confmatrix
 import classeval.ROC as ROC
 
 __author__ = 'Erdogan Tasksen'
 __email__ = 'erdogant@gmail.com'
-__version__ = '0.2.0'
+__version__ = '0.2.1'
 
 # module level doc-string
 __doc__ = """
 classeval
 =============================
 
 Description
```

### Comparing `classeval-0.2.0/classeval/classeval.py` & `classeval-0.2.1/classeval/classeval.py`

 * *Files identical despite different names*

### Comparing `classeval-0.2.0/classeval/confmatrix.py` & `classeval-0.2.1/classeval/confmatrix.py`

 * *Files identical despite different names*

### Comparing `classeval-0.2.0/classeval/examples.py` & `classeval-0.2.1/classeval/examples.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,29 +7,31 @@
 # %% Import example dataset
 from sklearn.model_selection import train_test_split
 from sklearn.ensemble import GradientBoostingClassifier
 gb = GradientBoostingClassifier()
 
 
 # %% cross validation example
+import classeval as clf
 X, y = clf.load_example('breast')
 out = {}
 for i in range(0,10):
     X_train, X_test, y_train, y_true = train_test_split(X, y, test_size=0.2)
     # Train model
     model = gb.fit(X_train, y_train)
     y_proba = model.predict_proba(X_test)[:,1]
     y_pred = model.predict(X_test)
     # Evaluate model
     out['cross ' +str(i)] = clf.eval(y_true, y_proba, y_pred=y_pred, pos_label='malignant')
 
-clf.plot_cross(out, title='crossvalidation')
+fig, ax = clf.plot_cross(out, title='crossvalidation')
 
 
 # %% Two-class
+import classeval as clf
 X, y = clf.load_example('breast')
 X_train, X_test, y_train, y_true = train_test_split(X, y, test_size=0.2)
 
 # Prediction
 model = gb.fit(X_train, y_train)
 y_proba = model.predict_proba(X_test)[:,1]
 y_pred = model.predict(X_test)
```

### Comparing `classeval-0.2.0/classeval.egg-info/PKG-INFO` & `classeval-0.2.1/classeval.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: classeval
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python package classeval
 Home-page: https://erdogant.github.io/classeval/
-Download-URL: https://github.com/erdogant/classeval/archive/0.2.0.tar.gz
+Download-URL: https://github.com/erdogant/classeval/archive/0.2.1.tar.gz
 Author: Erdogan Taskesen
 Author-email: erdogant@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -107,9 +105,7 @@
 ### Citation
 Please cite ``classeval`` in your publications if this is useful for your research. See column right for citation information.
 
 ### Maintainer
 * Erdogan Taskesen, github: [erdogant](https://github.com/erdogant)
 * Contributions are welcome.
 * If you wish to buy me a <a href="https://erdogant.github.io/donate/?currency=USD&amount=5">Coffee</a> for this work, it is very appreciated :)
-
-
```

#### html2text {}

```diff
@@ -1,28 +1,27 @@
-Metadata-Version: 2.1 Name: classeval Version: 0.2.0 Summary: Python package
+Metadata-Version: 2.1 Name: classeval Version: 0.2.1 Summary: Python package
 classeval Home-page: https://erdogant.github.io/classeval/ Download-URL: https:
-//github.com/erdogant/classeval/archive/0.2.0.tar.gz Author: Erdogan Taskesen
-Author-email: erdogant@gmail.com License: UNKNOWN Platform: UNKNOWN Classifier:
-Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
-License Classifier: Operating System :: OS Independent Requires-Python: >=3
-Description-Content-Type: text/markdown License-File: LICENSE # classeval [!
-[Python](https://img.shields.io/pypi/pyversions/classeval)](https://
-img.shields.io/pypi/pyversions/classeval) [![PyPI Version](https://
-img.shields.io/pypi/v/classeval)](https://pypi.org/project/classeval/) [!
-[License](https://img.shields.io/badge/license-MIT-green.svg)](https://
-github.com/erdogant/classeval/blob/master/LICENSE) [![Forks](https://
-img.shields.io/github/forks/erdogant/classeval.svg)](https://github.com/
-erdogant/classeval/network) [![Open Issues](https://img.shields.io/github/
-issues/erdogant/classeval.svg)](https://github.com/erdogant/classeval/issues)
-[![Project Status](http://www.repostatus.org/badges/latest/active.svg)](http://
-www.repostatus.org/#active) [![Downloads](https://pepy.tech/badge/classeval/
-month)](https://pepy.tech/project/classeval/) [![Downloads](https://pepy.tech/
-badge/classeval)](https://pepy.tech/project/classeval) [![DOI](https://
-zenodo.org/badge/246504758.svg)](https://zenodo.org/badge/latestdoi/246504758)
-[![Docs](https://img.shields.io/badge/Sphinx-Docs-Green)](https://
+//github.com/erdogant/classeval/archive/0.2.1.tar.gz Author: Erdogan Taskesen
+Author-email: erdogant@gmail.com Classifier: Programming Language :: Python ::
+3 Classifier: License :: OSI Approved :: MIT License Classifier: Operating
+System :: OS Independent Requires-Python: >=3 Description-Content-Type: text/
+markdown License-File: LICENSE # classeval [![Python](https://img.shields.io/
+pypi/pyversions/classeval)](https://img.shields.io/pypi/pyversions/classeval)
+[![PyPI Version](https://img.shields.io/pypi/v/classeval)](https://pypi.org/
+project/classeval/) [![License](https://img.shields.io/badge/license-MIT-
+green.svg)](https://github.com/erdogant/classeval/blob/master/LICENSE) [!
+[Forks](https://img.shields.io/github/forks/erdogant/classeval.svg)](https://
+github.com/erdogant/classeval/network) [![Open Issues](https://img.shields.io/
+github/issues/erdogant/classeval.svg)](https://github.com/erdogant/classeval/
+issues) [![Project Status](http://www.repostatus.org/badges/latest/active.svg)]
+(http://www.repostatus.org/#active) [![Downloads](https://pepy.tech/badge/
+classeval/month)](https://pepy.tech/project/classeval/) [![Downloads](https://
+pepy.tech/badge/classeval)](https://pepy.tech/project/classeval) [![DOI](https:
+//zenodo.org/badge/246504758.svg)](https://zenodo.org/badge/latestdoi/
+246504758) [![Docs](https://img.shields.io/badge/Sphinx-Docs-Green)](https://
 erdogant.github.io/classeval/) [![Donate](https://img.shields.io/badge/
 Support%20this%20project-grey.svg?logo=github%20sponsors)](https://
 erdogant.github.io/classeval/pages/html/Documentation.html#)   The library
 ``classeval`` is developed to evaluate the models performance of any kind of
 **two-class** or **multi-class** model. ``classeval`` computes many scoring
 measures in case of a two-class clasification model. Some measures are utilized
 from ``sklearn``, among them AUC, MCC, Cohen kappa score, matthews correlation
```

### Comparing `classeval-0.2.0/setup.py` & `classeval-0.2.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 else:
     raise RuntimeError("Unable to find version string in %s." % (VERSIONFILE,))
 
 # Setup ------------
 with open("README.md", "r") as fh:
     long_description = fh.read()
 setuptools.setup(
-     install_requires=['matplotlib','numpy','funcsigs','sklearn','colourmap'],
+     install_requires=['matplotlib','numpy','funcsigs','sklearn','colourmap','scikit-learn','pandas'],
      python_requires='>=3',
      name='classeval',
      version=new_version,
      author="Erdogan Taskesen",
      author_email="erdogant@gmail.com",
      description="Python package classeval",
      long_description=long_description,
```

