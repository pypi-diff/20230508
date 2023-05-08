# Comparing `tmp/bnlearn-0.7.8.tar.gz` & `tmp/bnlearn-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bnlearn-0.7.8.tar", last modified: Sat Oct 22 12:27:12 2022, max compression
+gzip compressed data, was "bnlearn-0.7.9.tar", last modified: Wed Nov 30 18:21:03 2022, max compression
```

## Comparing `bnlearn-0.7.8.tar` & `bnlearn-0.7.9.tar`

### file list

```diff
@@ -1,24 +1,28 @@
-drwxrwxrwx   0        0        0        0 2022-10-22 12:27:12.220898 bnlearn-0.7.8/
--rw-rw-rw-   0        0        0     1231 2022-05-09 18:05:29.000000 bnlearn-0.7.8/LICENSE
--rw-rw-rw-   0        0        0      643 2022-05-09 18:05:29.000000 bnlearn-0.7.8/MANIFEST.in
--rw-rw-rw-   0        0        0    11551 2022-10-22 12:27:12.219570 bnlearn-0.7.8/PKG-INFO
--rw-rw-rw-   0        0        0    10904 2022-05-20 20:28:42.000000 bnlearn-0.7.8/README.md
-drwxrwxrwx   0        0        0        0 2022-10-22 12:27:12.172695 bnlearn-0.7.8/bnlearn/
--rw-rw-rw-   0        0        0     4300 2022-10-22 12:00:55.000000 bnlearn-0.7.8/bnlearn/__init__.py
--rw-rw-rw-   0        0        0    67888 2022-10-22 12:00:25.000000 bnlearn-0.7.8/bnlearn/bnlearn.py
--rw-rw-rw-   0        0        0     1745 2022-05-09 18:05:29.000000 bnlearn-0.7.8/bnlearn/confmatrix.py
-drwxrwxrwx   0        0        0        0 2022-10-22 12:27:12.217374 bnlearn-0.7.8/bnlearn/data/
--rw-rw-rw-   0        0        0        0 2022-05-09 18:05:29.000000 bnlearn-0.7.8/bnlearn/data/__init__.py
--rw-rw-rw-   0        0        0    39918 2022-10-22 12:26:37.000000 bnlearn-0.7.8/bnlearn/examples.py
--rw-rw-rw-   0        0        0     3556 2022-08-05 17:21:16.000000 bnlearn-0.7.8/bnlearn/inference.py
--rw-rw-rw-   0        0        0    16904 2022-05-09 18:05:29.000000 bnlearn-0.7.8/bnlearn/network.py
--rw-rw-rw-   0        0        0     7294 2022-10-22 11:52:54.000000 bnlearn-0.7.8/bnlearn/parameter_learning.py
--rw-rw-rw-   0        0        0    25097 2022-10-22 11:38:13.000000 bnlearn-0.7.8/bnlearn/structure_learning.py
-drwxrwxrwx   0        0        0        0 2022-10-22 12:27:12.214625 bnlearn-0.7.8/bnlearn.egg-info/
--rw-rw-rw-   0        0        0    11551 2022-10-22 12:27:11.000000 bnlearn-0.7.8/bnlearn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      398 2022-10-22 12:27:11.000000 bnlearn-0.7.8/bnlearn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-22 12:27:11.000000 bnlearn-0.7.8/bnlearn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      181 2022-10-22 12:27:11.000000 bnlearn-0.7.8/bnlearn.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2022-10-22 12:27:11.000000 bnlearn-0.7.8/bnlearn.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-10-22 12:27:12.220898 bnlearn-0.7.8/setup.cfg
--rw-rw-rw-   0        0        0     1627 2022-05-09 18:05:30.000000 bnlearn-0.7.8/setup.py
+drwxrwxrwx   0        0        0        0 2022-11-30 18:21:03.121947 bnlearn-0.7.9/
+-rw-rw-rw-   0        0        0     1231 2022-05-09 18:05:29.000000 bnlearn-0.7.9/LICENSE
+-rw-rw-rw-   0        0        0      643 2022-05-09 18:05:29.000000 bnlearn-0.7.9/MANIFEST.in
+-rw-rw-rw-   0        0        0    11694 2022-11-30 18:21:03.121947 bnlearn-0.7.9/PKG-INFO
+-rw-rw-rw-   0        0        0    11047 2022-11-11 13:31:48.000000 bnlearn-0.7.9/README.md
+drwxrwxrwx   0        0        0        0 2022-11-30 18:21:03.022614 bnlearn-0.7.9/bnlearn/
+-rw-rw-rw-   0        0        0     4300 2022-11-30 18:17:50.000000 bnlearn-0.7.9/bnlearn/__init__.py
+-rw-rw-rw-   0        0        0    68464 2022-11-30 18:10:56.000000 bnlearn-0.7.9/bnlearn/bnlearn.py
+-rw-rw-rw-   0        0        0     1745 2022-05-09 18:05:29.000000 bnlearn-0.7.9/bnlearn/confmatrix.py
+drwxrwxrwx   0        0        0        0 2022-11-30 18:21:03.097673 bnlearn-0.7.9/bnlearn/data/
+-rw-rw-rw-   0        0        0        0 2022-05-09 18:05:29.000000 bnlearn-0.7.9/bnlearn/data/__init__.py
+-rw-rw-rw-   0        0        0    40174 2022-11-30 18:11:34.000000 bnlearn-0.7.9/bnlearn/examples.py
+-rw-rw-rw-   0        0        0     3556 2022-08-05 17:21:16.000000 bnlearn-0.7.9/bnlearn/inference.py
+-rw-rw-rw-   0        0        0    16904 2022-05-09 18:05:29.000000 bnlearn-0.7.9/bnlearn/network.py
+-rw-rw-rw-   0        0        0     7294 2022-10-22 11:52:54.000000 bnlearn-0.7.9/bnlearn/parameter_learning.py
+-rw-rw-rw-   0        0        0    25097 2022-10-22 11:38:13.000000 bnlearn-0.7.9/bnlearn/structure_learning.py
+drwxrwxrwx   0        0        0        0 2022-11-30 18:21:03.119898 bnlearn-0.7.9/bnlearn/tests/
+-rw-rw-rw-   0        0        0        0 2022-11-30 17:18:09.000000 bnlearn-0.7.9/bnlearn/tests/__init__.py
+-rw-rw-rw-   0        0        0    13205 2022-11-30 17:18:09.000000 bnlearn-0.7.9/bnlearn/tests/test_bnlearn.py
+-rw-rw-rw-   0        0        0     8222 2022-11-30 17:18:09.000000 bnlearn-0.7.9/bnlearn/tests/test_structure_learning.py
+drwxrwxrwx   0        0        0        0 2022-11-30 18:21:03.082540 bnlearn-0.7.9/bnlearn.egg-info/
+-rw-rw-rw-   0        0        0    11694 2022-11-30 18:21:02.000000 bnlearn-0.7.9/bnlearn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      495 2022-11-30 18:21:02.000000 bnlearn-0.7.9/bnlearn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-11-30 18:21:02.000000 bnlearn-0.7.9/bnlearn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      186 2022-11-30 18:21:02.000000 bnlearn-0.7.9/bnlearn.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2022-11-30 18:21:02.000000 bnlearn-0.7.9/bnlearn.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2022-11-30 18:21:03.122929 bnlearn-0.7.9/setup.cfg
+-rw-rw-rw-   0        0        0     2080 2022-11-30 17:18:09.000000 bnlearn-0.7.9/setup.py
```

### Comparing `bnlearn-0.7.8/LICENSE` & `bnlearn-0.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `bnlearn-0.7.8/MANIFEST.in` & `bnlearn-0.7.9/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `bnlearn-0.7.8/PKG-INFO` & `bnlearn-0.7.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 Metadata-Version: 2.1
 Name: bnlearn
-Version: 0.7.8
+Version: 0.7.9
 Summary: Python package for learning the graphical structure of Bayesian networks, parameter learning, inference and sampling methods.
 Home-page: https://erdogant.github.io/bnlearn
 Author: Erdogan Taskesen
 Author-email: erdogant@gmail.com
 License: UNKNOWN
-Download-URL: https://github.com/erdogant/bnlearn/archive/0.7.8.tar.gz
+Download-URL: https://github.com/erdogant/bnlearn/archive/0.7.9.tar.gz
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # bnlearn - Library for Bayesian network learning and inference
 
 [![Python](https://img.shields.io/pypi/pyversions/bnlearn)](https://img.shields.io/pypi/pyversions/bnlearn)
 [![PyPI Version](https://img.shields.io/pypi/v/bnlearn)](https://pypi.org/project/bnlearn/)
 [![License](https://img.shields.io/badge/license-MIT-green.svg)](https://github.com/erdogant/bnlearn/blob/master/LICENSE)
-[![Github Forks](https://img.shields.io/github/forks/erdogant/bnlearn.svg)](https://github.com/erdogant/bnlearn/network)
-[![GitHub Open Issues](https://img.shields.io/github/issues/erdogant/bnlearn.svg)](https://github.com/erdogant/bnlearn/issues)
+[![Forks](https://img.shields.io/github/forks/erdogant/bnlearn.svg)](https://github.com/erdogant/bnlearn/network)
+[![Open Issues](https://img.shields.io/github/issues/erdogant/bnlearn.svg)](https://github.com/erdogant/bnlearn/issues)
 [![Project Status](http://www.repostatus.org/badges/latest/active.svg)](http://www.repostatus.org/#active)
 [![Downloads](https://pepy.tech/badge/bnlearn/month)](https://pepy.tech/project/bnlearn/)
 [![Downloads](https://pepy.tech/badge/bnlearn)](https://pepy.tech/project/bnlearn)
 [![DOI](https://zenodo.org/badge/231263493.svg)](https://zenodo.org/badge/latestdoi/231263493)
-[![Sphinx](https://img.shields.io/badge/Sphinx-Docs-Green)](https://erdogant.github.io/bnlearn/)
+[![Docs](https://img.shields.io/badge/Sphinx-Docs-Green)](https://erdogant.github.io/bnlearn/)
 [![Medium](https://img.shields.io/badge/Medium-Blog-green)](https://erdogant.github.io/bnlearn/pages/html/Documentation.html#medium-blog)
-[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://erdogant.github.io/bnlearn/pages/html/Documentation.html#colab-notebook)
+[![Donate](https://img.shields.io/badge/Support%20this%20project-grey.svg?logo=github%20sponsors)](https://erdogant.github.io/bnlearn/pages/html/Documentation.html#)
+[![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://erdogant.github.io/bnlearn/pages/html/Documentation.html#colab-notebook)
 <!---[![BuyMeCoffee](https://img.shields.io/badge/buymea-coffee-yellow.svg)](https://www.buymeacoffee.com/erdogant)-->
 <!---[![Coffee](https://img.shields.io/badge/coffee-black-grey.svg)](https://erdogant.github.io/donate/?currency=USD&amount=5)-->
 
 
 ### 
 
 ``bnlearn`` is Python package for learning the graphical structure of Bayesian networks, parameter learning, inference and sampling methods. This work is inspired by the R package (bnlearn.com) that has been very usefull to me for many years. Although there are very good Python packages for probabilistic graphical models, it still can remain difficult (and somethimes unnecessarily) to (re)build certain pipelines. Bnlearn for python (this package) is build on the <a href="https://github.com/pgmpy/pgmpy">pgmpy</a> package and contains the most-wanted pipelines. Navigate to [API documentations](https://erdogant.github.io/bnlearn/) for more detailed information.
```

#### html2text {}

```diff
@@ -1,48 +1,51 @@
-Metadata-Version: 2.1 Name: bnlearn Version: 0.7.8 Summary: Python package for
+Metadata-Version: 2.1 Name: bnlearn Version: 0.7.9 Summary: Python package for
 learning the graphical structure of Bayesian networks, parameter learning,
 inference and sampling methods. Home-page: https://erdogant.github.io/bnlearn
 Author: Erdogan Taskesen Author-email: erdogant@gmail.com License: UNKNOWN
-Download-URL: https://github.com/erdogant/bnlearn/archive/0.7.8.tar.gz
+Download-URL: https://github.com/erdogant/bnlearn/archive/0.7.9.tar.gz
 Platform: UNKNOWN Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3 Description-Content-Type: text/markdown
 License-File: LICENSE # bnlearn - Library for Bayesian network learning and
 inference [![Python](https://img.shields.io/pypi/pyversions/bnlearn)](https://
 img.shields.io/pypi/pyversions/bnlearn) [![PyPI Version](https://
 img.shields.io/pypi/v/bnlearn)](https://pypi.org/project/bnlearn/) [![License]
 (https://img.shields.io/badge/license-MIT-green.svg)](https://github.com/
-erdogant/bnlearn/blob/master/LICENSE) [![Github Forks](https://img.shields.io/
-github/forks/erdogant/bnlearn.svg)](https://github.com/erdogant/bnlearn/
-network) [![GitHub Open Issues](https://img.shields.io/github/issues/erdogant/
-bnlearn.svg)](https://github.com/erdogant/bnlearn/issues) [![Project Status]
-(http://www.repostatus.org/badges/latest/active.svg)](http://
-www.repostatus.org/#active) [![Downloads](https://pepy.tech/badge/bnlearn/
-month)](https://pepy.tech/project/bnlearn/) [![Downloads](https://pepy.tech/
-badge/bnlearn)](https://pepy.tech/project/bnlearn) [![DOI](https://zenodo.org/
-badge/231263493.svg)](https://zenodo.org/badge/latestdoi/231263493) [![Sphinx]
-(https://img.shields.io/badge/Sphinx-Docs-Green)](https://erdogant.github.io/
-bnlearn/) [![Medium](https://img.shields.io/badge/Medium-Blog-green)](https://
-erdogant.github.io/bnlearn/pages/html/Documentation.html#medium-blog) [![Open
-In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://
-erdogant.github.io/bnlearn/pages/html/Documentation.html#colab-notebook)   ###
-``bnlearn`` is Python package for learning the graphical structure of Bayesian
-networks, parameter learning, inference and sampling methods. This work is
-inspired by the R package (bnlearn.com) that has been very usefull to me for
-many years. Although there are very good Python packages for probabilistic
-graphical models, it still can remain difficult (and somethimes unnecessarily)
-to (re)build certain pipelines. Bnlearn for python (this package) is build on
-the pgmpy package and contains the most-wanted pipelines. Navigate to [API
-documentations](https://erdogant.github.io/bnlearn/) for more detailed
-information. # **â­ï¸ Star this repo if you like it â­ï¸** # ### Blogs Read
-the blogs to get a structured overview of bayesian methods and detailed usage
-of ``bnlearn``. * [Step-by-step guide for structure learning.](https://
-erdogant.github.io/bnlearn/pages/html/Documentation.html#medium-blog) * [Step-
-by-step guide for knowledge-driven models.](https://erdogant.github.io/bnlearn/
-pages/html/Documentation.html#medium-blog) # ### [Documentation pages](https://
+erdogant/bnlearn/blob/master/LICENSE) [![Forks](https://img.shields.io/github/
+forks/erdogant/bnlearn.svg)](https://github.com/erdogant/bnlearn/network) [!
+[Open Issues](https://img.shields.io/github/issues/erdogant/bnlearn.svg)]
+(https://github.com/erdogant/bnlearn/issues) [![Project Status](http://
+www.repostatus.org/badges/latest/active.svg)](http://www.repostatus.org/
+#active) [![Downloads](https://pepy.tech/badge/bnlearn/month)](https://
+pepy.tech/project/bnlearn/) [![Downloads](https://pepy.tech/badge/bnlearn)]
+(https://pepy.tech/project/bnlearn) [![DOI](https://zenodo.org/badge/
+231263493.svg)](https://zenodo.org/badge/latestdoi/231263493) [![Docs](https://
+img.shields.io/badge/Sphinx-Docs-Green)](https://erdogant.github.io/bnlearn/)
+[![Medium](https://img.shields.io/badge/Medium-Blog-green)](https://
+erdogant.github.io/bnlearn/pages/html/Documentation.html#medium-blog) [!
+[Donate](https://img.shields.io/badge/Support%20this%20project-
+grey.svg?logo=github%20sponsors)](https://erdogant.github.io/bnlearn/pages/
+html/Documentation.html#) [![Colab](https://colab.research.google.com/assets/
+colab-badge.svg)](https://erdogant.github.io/bnlearn/pages/html/
+Documentation.html#colab-notebook)   ### ``bnlearn`` is Python package for
+learning the graphical structure of Bayesian networks, parameter learning,
+inference and sampling methods. This work is inspired by the R package
+(bnlearn.com) that has been very usefull to me for many years. Although there
+are very good Python packages for probabilistic graphical models, it still can
+remain difficult (and somethimes unnecessarily) to (re)build certain pipelines.
+Bnlearn for python (this package) is build on the pgmpy package and contains
+the most-wanted pipelines. Navigate to [API documentations](https://
+erdogant.github.io/bnlearn/) for more detailed information. # **â­ï¸ Star
+this repo if you like it â­ï¸** # ### Blogs Read the blogs to get a
+structured overview of bayesian methods and detailed usage of ``bnlearn``. *
+[Step-by-step guide for structure learning.](https://erdogant.github.io/
+bnlearn/pages/html/Documentation.html#medium-blog) * [Step-by-step guide for
+knowledge-driven models.](https://erdogant.github.io/bnlearn/pages/html/
+Documentation.html#medium-blog) # ### [Documentation pages](https://
 erdogant.github.io/bnlearn/) On the [documentation pages](https://
 erdogant.github.io/bnlearn/) you can find detailed information about the
 working of the ``bnlearn`` with many examples. # ### Installation ##### It is
 advisable to create a new environment (e.g. with Conda). ```bash conda create -
 n env_bnlearn python=3.8 conda activate env_bnlearn ``` ##### Install bnlearn
 from PyPI ```bash pip install bnlearn ``` ##### The following functions are
 available after installation: ```python # Import library import bnlearn as bn #
```

### Comparing `bnlearn-0.7.8/README.md` & `bnlearn-0.7.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 # bnlearn - Library for Bayesian network learning and inference
 
 [![Python](https://img.shields.io/pypi/pyversions/bnlearn)](https://img.shields.io/pypi/pyversions/bnlearn)
 [![PyPI Version](https://img.shields.io/pypi/v/bnlearn)](https://pypi.org/project/bnlearn/)
 [![License](https://img.shields.io/badge/license-MIT-green.svg)](https://github.com/erdogant/bnlearn/blob/master/LICENSE)
-[![Github Forks](https://img.shields.io/github/forks/erdogant/bnlearn.svg)](https://github.com/erdogant/bnlearn/network)
-[![GitHub Open Issues](https://img.shields.io/github/issues/erdogant/bnlearn.svg)](https://github.com/erdogant/bnlearn/issues)
+[![Forks](https://img.shields.io/github/forks/erdogant/bnlearn.svg)](https://github.com/erdogant/bnlearn/network)
+[![Open Issues](https://img.shields.io/github/issues/erdogant/bnlearn.svg)](https://github.com/erdogant/bnlearn/issues)
 [![Project Status](http://www.repostatus.org/badges/latest/active.svg)](http://www.repostatus.org/#active)
 [![Downloads](https://pepy.tech/badge/bnlearn/month)](https://pepy.tech/project/bnlearn/)
 [![Downloads](https://pepy.tech/badge/bnlearn)](https://pepy.tech/project/bnlearn)
 [![DOI](https://zenodo.org/badge/231263493.svg)](https://zenodo.org/badge/latestdoi/231263493)
-[![Sphinx](https://img.shields.io/badge/Sphinx-Docs-Green)](https://erdogant.github.io/bnlearn/)
+[![Docs](https://img.shields.io/badge/Sphinx-Docs-Green)](https://erdogant.github.io/bnlearn/)
 [![Medium](https://img.shields.io/badge/Medium-Blog-green)](https://erdogant.github.io/bnlearn/pages/html/Documentation.html#medium-blog)
-[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://erdogant.github.io/bnlearn/pages/html/Documentation.html#colab-notebook)
+[![Donate](https://img.shields.io/badge/Support%20this%20project-grey.svg?logo=github%20sponsors)](https://erdogant.github.io/bnlearn/pages/html/Documentation.html#)
+[![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://erdogant.github.io/bnlearn/pages/html/Documentation.html#colab-notebook)
 <!---[![BuyMeCoffee](https://img.shields.io/badge/buymea-coffee-yellow.svg)](https://www.buymeacoffee.com/erdogant)-->
 <!---[![Coffee](https://img.shields.io/badge/coffee-black-grey.svg)](https://erdogant.github.io/donate/?currency=USD&amount=5)-->
 
 
 ### 
 
 ``bnlearn`` is Python package for learning the graphical structure of Bayesian networks, parameter learning, inference and sampling methods. This work is inspired by the R package (bnlearn.com) that has been very usefull to me for many years. Although there are very good Python packages for probabilistic graphical models, it still can remain difficult (and somethimes unnecessarily) to (re)build certain pipelines. Bnlearn for python (this package) is build on the <a href="https://github.com/pgmpy/pgmpy">pgmpy</a> package and contains the most-wanted pipelines. Navigate to [API documentations](https://erdogant.github.io/bnlearn/) for more detailed information.
```

#### html2text {}

```diff
@@ -1,33 +1,35 @@
 # bnlearn - Library for Bayesian network learning and inference [![Python]
 (https://img.shields.io/pypi/pyversions/bnlearn)](https://img.shields.io/pypi/
 pyversions/bnlearn) [![PyPI Version](https://img.shields.io/pypi/v/bnlearn)]
 (https://pypi.org/project/bnlearn/) [![License](https://img.shields.io/badge/
 license-MIT-green.svg)](https://github.com/erdogant/bnlearn/blob/master/
-LICENSE) [![Github Forks](https://img.shields.io/github/forks/erdogant/
-bnlearn.svg)](https://github.com/erdogant/bnlearn/network) [![GitHub Open
-Issues](https://img.shields.io/github/issues/erdogant/bnlearn.svg)](https://
-github.com/erdogant/bnlearn/issues) [![Project Status](http://
-www.repostatus.org/badges/latest/active.svg)](http://www.repostatus.org/
-#active) [![Downloads](https://pepy.tech/badge/bnlearn/month)](https://
-pepy.tech/project/bnlearn/) [![Downloads](https://pepy.tech/badge/bnlearn)]
-(https://pepy.tech/project/bnlearn) [![DOI](https://zenodo.org/badge/
-231263493.svg)](https://zenodo.org/badge/latestdoi/231263493) [![Sphinx](https:
-//img.shields.io/badge/Sphinx-Docs-Green)](https://erdogant.github.io/bnlearn/
-) [![Medium](https://img.shields.io/badge/Medium-Blog-green)](https://
-erdogant.github.io/bnlearn/pages/html/Documentation.html#medium-blog) [![Open
-In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://
-erdogant.github.io/bnlearn/pages/html/Documentation.html#colab-notebook)   ###
-``bnlearn`` is Python package for learning the graphical structure of Bayesian
-networks, parameter learning, inference and sampling methods. This work is
-inspired by the R package (bnlearn.com) that has been very usefull to me for
-many years. Although there are very good Python packages for probabilistic
-graphical models, it still can remain difficult (and somethimes unnecessarily)
-to (re)build certain pipelines. Bnlearn for python (this package) is build on
-the pgmpy package and contains the most-wanted pipelines. Navigate to [API
+LICENSE) [![Forks](https://img.shields.io/github/forks/erdogant/bnlearn.svg)]
+(https://github.com/erdogant/bnlearn/network) [![Open Issues](https://
+img.shields.io/github/issues/erdogant/bnlearn.svg)](https://github.com/
+erdogant/bnlearn/issues) [![Project Status](http://www.repostatus.org/badges/
+latest/active.svg)](http://www.repostatus.org/#active) [![Downloads](https://
+pepy.tech/badge/bnlearn/month)](https://pepy.tech/project/bnlearn/) [!
+[Downloads](https://pepy.tech/badge/bnlearn)](https://pepy.tech/project/
+bnlearn) [![DOI](https://zenodo.org/badge/231263493.svg)](https://zenodo.org/
+badge/latestdoi/231263493) [![Docs](https://img.shields.io/badge/Sphinx-Docs-
+Green)](https://erdogant.github.io/bnlearn/) [![Medium](https://img.shields.io/
+badge/Medium-Blog-green)](https://erdogant.github.io/bnlearn/pages/html/
+Documentation.html#medium-blog) [![Donate](https://img.shields.io/badge/
+Support%20this%20project-grey.svg?logo=github%20sponsors)](https://
+erdogant.github.io/bnlearn/pages/html/Documentation.html#) [![Colab](https://
+colab.research.google.com/assets/colab-badge.svg)](https://erdogant.github.io/
+bnlearn/pages/html/Documentation.html#colab-notebook)   ### ``bnlearn`` is
+Python package for learning the graphical structure of Bayesian networks,
+parameter learning, inference and sampling methods. This work is inspired by
+the R package (bnlearn.com) that has been very usefull to me for many years.
+Although there are very good Python packages for probabilistic graphical
+models, it still can remain difficult (and somethimes unnecessarily) to
+(re)build certain pipelines. Bnlearn for python (this package) is build on the
+pgmpy package and contains the most-wanted pipelines. Navigate to [API
 documentations](https://erdogant.github.io/bnlearn/) for more detailed
 information. # **â­ï¸ Star this repo if you like it â­ï¸** # ### Blogs Read
 the blogs to get a structured overview of bayesian methods and detailed usage
 of ``bnlearn``. * [Step-by-step guide for structure learning.](https://
 erdogant.github.io/bnlearn/pages/html/Documentation.html#medium-blog) * [Step-
 by-step guide for knowledge-driven models.](https://erdogant.github.io/bnlearn/
 pages/html/Documentation.html#medium-blog) # ### [Documentation pages](https://
```

### Comparing `bnlearn-0.7.8/bnlearn/__init__.py` & `bnlearn-0.7.9/bnlearn/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 import bnlearn.inference as inference
 import bnlearn.network as network
 import bnlearn.confmatrix as confmatrix
 from packaging import version
 
 __author__ = 'Erdogan Tasksen'
 __email__ = 'erdogant@gmail.com'
-__version__ = '0.7.8'
+__version__ = '0.7.9'
 
 try:
     import pgmpy
 except:
     raise ImportError('[bnlearn] >Error: pgmpy version "0.1.13" or higher must be installed manually. Try to: <conda install -c ankurankan pgmpy> or <pip install -U pgmpy>=0.1.13>')
 
 # Check version pgmpy
```

### Comparing `bnlearn-0.7.8/bnlearn/bnlearn.py` & `bnlearn-0.7.9/bnlearn/bnlearn.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,15 +104,15 @@
         * 'model_edges': Edges
 
     Examples
     --------
     >>> import bnlearn as bn
     >>> edges = [('A', 'B'), ('A', 'C'), ('A', 'D')]
     >>> DAG = bn.make_DAG(edges, methodtype='naivebayes')
-    >>> bn.plot(DAG)
+    >>> fig = bn.plot(DAG)
 
     """
     if (CPD is not None) and (not isinstance(CPD, list)):
         CPD=[CPD]
 
     if methodtype=='nb': methodtype='naivebayes'
 
@@ -808,19 +808,19 @@
     >>> # Create DAG and store in model
     >>> model = bn.make_DAG(edges)
     >>> node_properties = bn.get_node_properties(model)
     >>> # Adjust the properties
     >>> node_properties['A']['node_size']=2000
     >>> node_properties['A']['node_color']='#000000'
     >>> # Make plot
-    >>> bn.plot(model, interactive=False, node_properties=node_properties)
+    >>> fig = bn.plot(model, interactive=False, node_properties=node_properties)
     >>>
     >>> # Example: Specify all nodes
     >>> node_properties = bn.get_node_properties(model, node_size=1000, node_color='#000000')
-    >>> bn.plot(model, interactive=False, node_properties=node_properties)
+    >>> fig = bn.plot(model, interactive=False, node_properties=node_properties)
 
     """
     # https://networkx.org/documentation/networkx-1.7/reference/generated/networkx.drawing.nx_pylab.draw_networkx_nodes.html
     nodes = {}
     defaults={'node_color': node_color, 'node_size': node_size}
     adjmat = model.get('adjmat', None)
 
@@ -868,29 +868,29 @@
     >>> # Create DAG and store in model
     >>> model = bn.make_DAG(edges)
     >>> edge_properties = bn.get_edge_properties(model)
     >>> # Adjust the properties
     >>> edge_properties[('A', 'B')]['weight']=10
     >>> edge_properties[('A', 'B')]['color']='#8A0707'
     >>> # Make plot
-    >>> bn.plot(model, interactive=False, edge_properties=edge_properties)
+    >>> fig = bn.plot(model, interactive=False, edge_properties=edge_properties)
     >>>
     >>> # Example 2:
     >>>  # Load asia DAG
     >>> df = bn.import_example(data='asia')
     >>> # Structure learning of sampled dataset
     >>> model = bn.structure_learning.fit(df)
     >>> # Compute edge weights based on chi_square test statistic
     >>> model = bn.independence_test(model, df, test='chi_square')
     >>> # Get the edge properties
     >>> edge_properties = bn.get_edge_properties(model)
     >>> # Make adjustments
     >>> edge_properties[('tub', 'either')]['color']='#8A0707'
     >>> # Make plot
-    >>> bn.plot(model, interactive=True, edge_properties=edge_properties)
+    >>> fig = bn.plot(model, interactive=True, edge_properties=edge_properties)
 
     """
     # https://networkx.org/documentation/networkx-1.7/reference/generated/networkx.drawing.nx_pylab.draw_networkx_nodes.html
     edges = {}
     defaults = {'color': color, 'weight': weight}
     adjmat = model.get('independence_test', None)
     # Use edge weights from test statistic
@@ -930,15 +930,15 @@
          interactive=False,
          title='bnlearn_causal_network',
          node_color=None,
          node_size=None,
          node_properties=None,
          edge_properties=None,
          params_interactive={'width': '70%', 'height': '800px', 'notebook': False, 'layout': None, 'font_color': False, 'bgcolor': '#ffffff'},
-         params_static={'minscale': 1, 'maxscale': 10, 'figsize': (15, 10), 'width': None, 'height': None, 'font_size': 14, 'font_family': 'sans-serif', 'alpha': 0.8, 'node_shape': 'o', 'layout': 'spring_layout', 'font_color': '#000000', 'facecolor': 'white', 'edge_alpha': 0.8, 'arrowstyle': '-|>', 'arrowsize': 30},
+         params_static={'minscale': 1, 'maxscale': 10, 'figsize': (15, 10), 'width': None, 'height': None, 'font_size': 14, 'font_family': 'sans-serif', 'alpha': 0.8, 'node_shape': 'o', 'layout': 'spring_layout', 'font_color': '#000000', 'facecolor': 'white', 'edge_alpha': 0.8, 'arrowstyle': '-|>', 'arrowsize': 30, 'visible': True},
          verbose=3):
     """Plot the learned stucture.
 
     Parameters
     ----------
     model : dict
         Learned model from the .fit() function.
@@ -989,48 +989,49 @@
     >>> # Load asia DAG
     >>> df = bn.import_example(data='asia')
     >>>
     >>> # Structure learning of sampled dataset
     >>> model = bn.structure_learning.fit(df)
     >>>
     >>> # plot static
-    >>> G = bn.plot(model)
+    >>> fig = bn.plot(model)
     >>>
     >>> # plot interactive
-    >>> G = bn.plot(model, interactive=True)
+    >>> fig = bn.plot(model, interactive=True)
     >>>
     >>> # plot interactive with various settings
-    >>> bn.plot(model, interactive=True, node_color='#8A0707', node_size=35, params_interactive = {'height':'800px', 'width':'70%', 'bgcolor':'#0f0f0f0f'})
+    >>> fig = bn.plot(model, interactive=True, node_color='#8A0707', node_size=35, params_interactive = {'height':'800px', 'width':'70%', 'bgcolor':'#0f0f0f0f'})
     >>>
     >>> # plot with node properties
     >>> node_properties = bn.get_node_properties(model)
     >>> # Make some changes
     >>> node_properties['xray']['node_color']='#8A0707'
     >>> node_properties['xray']['node_size']=50
     >>> # Plot
-    >>> bn.plot(model, interactive=True, node_properties=node_properties)
+    >>> fig = bn.plot(model, interactive=True, node_properties=node_properties)
     >>>
 
     """
+    ax = None
     # Check whether edges are available
     if model['adjmat'].sum().sum()==0:
         if verbose>=3: print('[bnlearn]> Nothing to plot because no edges are present between nodes. ')
         return None
 
     # Plot properties
     defaults = {'height': '800px', 'width': '70%', 'notebook': False, 'layout': None, 'font_color': False, 'bgcolor': '#ffffff', 'directed': True}
     params_interactive = {**defaults, **params_interactive}
-    defaults = {'minscale': 1, 'maxscale': 10, 'figsize': (15, 10), 'height': None, 'width': None, 'font_size': 14, 'font_family': 'sans-serif', 'alpha': 0.8, 'layout': 'spring_layout', 'font_color': 'k', 'facecolor': '#ffffff', 'node_shape': 'o', 'edge_alpha': 0.8, 'arrowstyle': '-|>', 'arrowsize': 30}
+    defaults = {'minscale': 1, 'maxscale': 10, 'figsize': (15, 10), 'height': None, 'width': None, 'font_size': 14, 'font_family': 'sans-serif', 'alpha': 0.8, 'layout': 'spring_layout', 'font_color': 'k', 'facecolor': '#ffffff', 'node_shape': 'o', 'edge_alpha': 0.8, 'arrowstyle': '-|>', 'arrowsize': 30, 'visible': True}
     params_static = {**defaults, **params_static}
 
-    ##### DEPRECATED IN LATER VERSION #####
+    # DEPRECATED IN LATER VERSION
     if (params_static.get('width') is not None) or (params_static.get('height') is not None):
         # if verbose>=2: print('[bnlearn]> Warning: [height] and [width] will be removed in further version. Please use: params_static={"figsize": (15, 10)}.')
         params_static['figsize'] = (15 if params_static['width'] is None else params_static['width'], 10 if params_static['height'] is None else params_static['height'])
-    ##### END BLOCK #####
+    # END BLOCK
 
     out = {}
     G = nx.DiGraph()  # Directed graph
     node_size_default = 10 if interactive else 800
     if (node_properties is not None) and (node_size is not None):
         if verbose>=2: print('[bnlearn]> Warning: if both "node_size" and "node_properties" are used, "node_size" will be used.')
 
@@ -1069,45 +1070,47 @@
         G = bnlearn.network.adjmat2graph(model['adjmat'])
         # Get positions
         pos = bnlearn.network.graphlayout(G, pos=pos, scale=scale, layout=params_static['layout'], verbose=verbose)
 
     # Plot
     if interactive:
         # Make interactive plot
-        _plot_interactive(model, params_interactive, nodelist, node_colors, node_sizes, edgelist, edge_colors, edge_weights, title, verbose=verbose)
+        ax = _plot_interactive(model, params_interactive, nodelist, node_colors, node_sizes, edgelist, edge_colors, edge_weights, title, verbose=verbose)
     else:
         # Make static plot
-        _plot_static(model, params_static, nodelist, node_colors, node_sizes, G, pos, edge_colors, edge_weights)
+        ax = _plot_static(model, params_static, nodelist, node_colors, node_sizes, G, pos, edge_colors, edge_weights, visible=params_static['visible'])
 
     # Store
+    out['ax']=ax
     out['pos']=pos
     out['G']=G
     out['node_properties']=node_properties
     out['edge_properties']=edge_properties
-    return(out)
+    return out
 
 
 # %% Plot interactive
 # def _plot_static(model, params_static, nodelist, node_colors, node_sizes, title, verbose=3):
-def _plot_static(model, params_static, nodelist, node_colors, node_sizes, G, pos, edge_colors, edge_weights):
+def _plot_static(model, params_static, nodelist, node_colors, node_sizes, G, pos, edge_colors, edge_weights, visible=True):
     # Bootup figure
-    plt.figure(figsize=params_static['figsize'], facecolor=params_static['facecolor'])
+    ax = plt.figure(figsize=params_static['figsize'], facecolor=params_static['facecolor'])
     # nodes
     nx.draw_networkx_nodes(G, pos, nodelist=nodelist, node_size=node_sizes, alpha=params_static['alpha'], node_color=node_colors, node_shape=params_static['node_shape'])
     # edges
     # nx.draw_networkx_edges(G, pos, arrowstyle='-|>', arrowsize=30, edge_color=edge_color, width=edge_weights)
     nx.draw_networkx_edges(G, pos, arrowstyle=params_static['arrowstyle'], arrowsize=params_static['arrowsize'], edge_color=edge_colors, width=edge_weights, alpha=params_static['edge_alpha'])
     # Labels
     nx.draw_networkx_labels(G, pos, font_size=params_static['font_size'], font_family=params_static['font_family'], font_color=params_static['font_color'])
     # Plot text of the weights
     # nx.draw_networkx_edge_labels(G, pos, edge_labels=nx.get_edge_attributes(G, 'weight'), font_color=params_static['font_color'])
     # Making figure nice
-    ax = plt.gca()
-    ax.set_axis_off()
-    plt.show()
+    # ax = plt.gca()
+    # ax.set_axis_off()
+    ax.set_visible(visible)
+    return ax
 
 
 # %% Plot interactive
 def _plot_interactive(model, params_interactive, nodelist, node_colors, node_sizes, edgelist, edge_colors, edge_weights, title, verbose=3):
     try:
         from pyvis.network import Network
         from IPython.core.display import display, HTML
@@ -1134,14 +1137,15 @@
     # Create advanced buttons
     g.show_buttons(filter_=['physics'])
     # Display
     filename = title.strip().replace(' ', '_') + '.html'
     g.show(filename)
     display(HTML(filename))
     # webbrowser.open('bnlearn.html')
+    return os.path.abspath(filename)
 
 
 # %% Plot properties
 def _plot_properties(G, node_properties, edge_properties, node_color, node_size):
     # Set edge properties in Graph G
     # edges=[*bnmodel.edges()]
     edges = list(edge_properties.keys())
@@ -1325,15 +1329,15 @@
         model : BayesianNetwork
         adjmat : Adjacency matrix
 
     Examples
     --------
     >>> import bnlearn as bn
     >>> model = bn.import_DAG('sprinkler')
-    >>> bn.plot(model)
+    >>> fig = bn.plot(model)
 
     """
     PATH_TO_DATA = os.path.join(os.path.dirname(os.path.abspath(__file__)), 'data')
     out={}
     model=None
     filepath=filepath.lower()
     if verbose>=3: print('[bnlearn] >Import <%s>' %(filepath))
@@ -1729,49 +1733,57 @@
 
 # %% Compute structure scores.
 def structure_scores(model, df, scoring_method=['k2', 'bds', 'bic', 'bdeu'], verbose=3, **kwargs):
     """Compute structure scores.
 
     Description
     -----------
-    Uses the standard model scoring methods to give a score for each structure.
-    The score doesn't have very straight forward interpretebility but can be
-    used to compare different models. A higher score represents a better fit.
-    This method only needs the model structure to compute the score and parameters
-    aren't required.
+    Each model can be scored based on its structure. However, the score doesn't have very straight forward
+    interpretebility but can be used to compare different models. A higher score represents a better fit.
+    This method only needs the model structure to compute the score. The structure score functionality
+    can be found here: :func:`bnlearn.bnlearn.structure_scores`.
 
     Parameters
     ----------
-    model: pgmpy.base.DAG or pgmpy.models.BayesianNetwork instance
+    model: The bnlearn instance such as pgmpy.base.DAG or pgmpy.models.BayesianNetwork
         The model whose score needs to be computed.
 
     df: pd.DataFrame instance
         The dataset against which to score the model.
 
     scoring_method: str ( k2 | bdeu | bds | bic )
         The following four scoring methods are supported currently: 1) K2Score
         2) BDeuScore 3) BDsScore 4) BicScore
 
     kwargs: kwargs
         Any additional parameters parameters that needs to be passed to the
-        scoring method. Check pgmpy.estimators.StructureScore for details.
+        scoring method.
 
     Returns
     -------
     Model score: float
         A score value for the model.
 
     Examples
     --------
-    >>> from pgmpy.utils import get_example_model
-    >>> from pgmpy.metrics import structure_score
-    >>> model = get_example_model('alarm')
-    >>> data = model.simulate(int(10000))
-    >>> structure_score(model, data, scoring_method="bic")
-    -106665.9383064447
+    >>> import bnlearn as bn
+    >>> # Load example dataset
+    >>>
+    >>> df = bn.import_example('sprinkler')
+    >>> edges = [('Cloudy', 'Sprinkler'), ('Cloudy', 'Rain'), ('Sprinkler', 'Wet_Grass'), ('Rain', 'Wet_Grass')]
+    >>>
+    >>> # Make the Bayesian DAG
+    >>> DAG = bn.make_DAG(edges)
+    >>> model = bn.parameter_learning.fit(DAG, df)
+    >>>
+    >>> # Structure scores are stored in the model dictionary.
+    >>> model['structure_scores']
+    >>>
+    >>> # Compute the structure score for as specific scoring-method.
+    >>> bn.structure_scores(model, df, scoring_method="bic")
     """
     method = None
     show_message = True
     scores = {}
     # Get models and method
     if isinstance(model, dict):
         method = model.get('config')['method']
```

### Comparing `bnlearn-0.7.8/bnlearn/confmatrix.py` & `bnlearn-0.7.9/bnlearn/confmatrix.py`

 * *Files identical despite different names*

### Comparing `bnlearn-0.7.8/bnlearn/examples.py` & `bnlearn-0.7.9/bnlearn/examples.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,23 @@
 import pandas as pd
 import numpy as np
 from pgmpy.inference import VariableElimination
 from pgmpy.models import BayesianNetwork, NaiveBayes
 from pgmpy.estimators import ExhaustiveSearch, HillClimbSearch, TreeSearch
 from pgmpy.factors.discrete import TabularCPD
 
+# %% Issue 65: return (fig, ax)
+import bnlearn as bn
+model = bn.import_DAG('sprinkler', CPD=True)
+df = bn.sampling(model, n=1000, methodtype='bayes')
+fig = bn.plot(model, params_static={'visible': True})
+
+fig2 = bn.plot(model, interactive=True)
+
+
 # %% Issue Mail:
 # from pgmpy.models import BayesianNetwork
 
 # # create instance
 # hd_bn = BayesianNetwork()
 
 # # create dag
```

### Comparing `bnlearn-0.7.8/bnlearn/inference.py` & `bnlearn-0.7.9/bnlearn/inference.py`

 * *Files identical despite different names*

### Comparing `bnlearn-0.7.8/bnlearn/network.py` & `bnlearn-0.7.9/bnlearn/network.py`

 * *Files identical despite different names*

### Comparing `bnlearn-0.7.8/bnlearn/parameter_learning.py` & `bnlearn-0.7.9/bnlearn/parameter_learning.py`

 * *Files identical despite different names*

### Comparing `bnlearn-0.7.8/bnlearn/structure_learning.py` & `bnlearn-0.7.9/bnlearn/structure_learning.py`

 * *Files identical despite different names*

### Comparing `bnlearn-0.7.8/bnlearn.egg-info/PKG-INFO` & `bnlearn-0.7.9/bnlearn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 Metadata-Version: 2.1
 Name: bnlearn
-Version: 0.7.8
+Version: 0.7.9
 Summary: Python package for learning the graphical structure of Bayesian networks, parameter learning, inference and sampling methods.
 Home-page: https://erdogant.github.io/bnlearn
 Author: Erdogan Taskesen
 Author-email: erdogant@gmail.com
 License: UNKNOWN
-Download-URL: https://github.com/erdogant/bnlearn/archive/0.7.8.tar.gz
+Download-URL: https://github.com/erdogant/bnlearn/archive/0.7.9.tar.gz
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # bnlearn - Library for Bayesian network learning and inference
 
 [![Python](https://img.shields.io/pypi/pyversions/bnlearn)](https://img.shields.io/pypi/pyversions/bnlearn)
 [![PyPI Version](https://img.shields.io/pypi/v/bnlearn)](https://pypi.org/project/bnlearn/)
 [![License](https://img.shields.io/badge/license-MIT-green.svg)](https://github.com/erdogant/bnlearn/blob/master/LICENSE)
-[![Github Forks](https://img.shields.io/github/forks/erdogant/bnlearn.svg)](https://github.com/erdogant/bnlearn/network)
-[![GitHub Open Issues](https://img.shields.io/github/issues/erdogant/bnlearn.svg)](https://github.com/erdogant/bnlearn/issues)
+[![Forks](https://img.shields.io/github/forks/erdogant/bnlearn.svg)](https://github.com/erdogant/bnlearn/network)
+[![Open Issues](https://img.shields.io/github/issues/erdogant/bnlearn.svg)](https://github.com/erdogant/bnlearn/issues)
 [![Project Status](http://www.repostatus.org/badges/latest/active.svg)](http://www.repostatus.org/#active)
 [![Downloads](https://pepy.tech/badge/bnlearn/month)](https://pepy.tech/project/bnlearn/)
 [![Downloads](https://pepy.tech/badge/bnlearn)](https://pepy.tech/project/bnlearn)
 [![DOI](https://zenodo.org/badge/231263493.svg)](https://zenodo.org/badge/latestdoi/231263493)
-[![Sphinx](https://img.shields.io/badge/Sphinx-Docs-Green)](https://erdogant.github.io/bnlearn/)
+[![Docs](https://img.shields.io/badge/Sphinx-Docs-Green)](https://erdogant.github.io/bnlearn/)
 [![Medium](https://img.shields.io/badge/Medium-Blog-green)](https://erdogant.github.io/bnlearn/pages/html/Documentation.html#medium-blog)
-[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://erdogant.github.io/bnlearn/pages/html/Documentation.html#colab-notebook)
+[![Donate](https://img.shields.io/badge/Support%20this%20project-grey.svg?logo=github%20sponsors)](https://erdogant.github.io/bnlearn/pages/html/Documentation.html#)
+[![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://erdogant.github.io/bnlearn/pages/html/Documentation.html#colab-notebook)
 <!---[![BuyMeCoffee](https://img.shields.io/badge/buymea-coffee-yellow.svg)](https://www.buymeacoffee.com/erdogant)-->
 <!---[![Coffee](https://img.shields.io/badge/coffee-black-grey.svg)](https://erdogant.github.io/donate/?currency=USD&amount=5)-->
 
 
 ### 
 
 ``bnlearn`` is Python package for learning the graphical structure of Bayesian networks, parameter learning, inference and sampling methods. This work is inspired by the R package (bnlearn.com) that has been very usefull to me for many years. Although there are very good Python packages for probabilistic graphical models, it still can remain difficult (and somethimes unnecessarily) to (re)build certain pipelines. Bnlearn for python (this package) is build on the <a href="https://github.com/pgmpy/pgmpy">pgmpy</a> package and contains the most-wanted pipelines. Navigate to [API documentations](https://erdogant.github.io/bnlearn/) for more detailed information.
```

#### html2text {}

```diff
@@ -1,48 +1,51 @@
-Metadata-Version: 2.1 Name: bnlearn Version: 0.7.8 Summary: Python package for
+Metadata-Version: 2.1 Name: bnlearn Version: 0.7.9 Summary: Python package for
 learning the graphical structure of Bayesian networks, parameter learning,
 inference and sampling methods. Home-page: https://erdogant.github.io/bnlearn
 Author: Erdogan Taskesen Author-email: erdogant@gmail.com License: UNKNOWN
-Download-URL: https://github.com/erdogant/bnlearn/archive/0.7.8.tar.gz
+Download-URL: https://github.com/erdogant/bnlearn/archive/0.7.9.tar.gz
 Platform: UNKNOWN Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3 Description-Content-Type: text/markdown
 License-File: LICENSE # bnlearn - Library for Bayesian network learning and
 inference [![Python](https://img.shields.io/pypi/pyversions/bnlearn)](https://
 img.shields.io/pypi/pyversions/bnlearn) [![PyPI Version](https://
 img.shields.io/pypi/v/bnlearn)](https://pypi.org/project/bnlearn/) [![License]
 (https://img.shields.io/badge/license-MIT-green.svg)](https://github.com/
-erdogant/bnlearn/blob/master/LICENSE) [![Github Forks](https://img.shields.io/
-github/forks/erdogant/bnlearn.svg)](https://github.com/erdogant/bnlearn/
-network) [![GitHub Open Issues](https://img.shields.io/github/issues/erdogant/
-bnlearn.svg)](https://github.com/erdogant/bnlearn/issues) [![Project Status]
-(http://www.repostatus.org/badges/latest/active.svg)](http://
-www.repostatus.org/#active) [![Downloads](https://pepy.tech/badge/bnlearn/
-month)](https://pepy.tech/project/bnlearn/) [![Downloads](https://pepy.tech/
-badge/bnlearn)](https://pepy.tech/project/bnlearn) [![DOI](https://zenodo.org/
-badge/231263493.svg)](https://zenodo.org/badge/latestdoi/231263493) [![Sphinx]
-(https://img.shields.io/badge/Sphinx-Docs-Green)](https://erdogant.github.io/
-bnlearn/) [![Medium](https://img.shields.io/badge/Medium-Blog-green)](https://
-erdogant.github.io/bnlearn/pages/html/Documentation.html#medium-blog) [![Open
-In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://
-erdogant.github.io/bnlearn/pages/html/Documentation.html#colab-notebook)   ###
-``bnlearn`` is Python package for learning the graphical structure of Bayesian
-networks, parameter learning, inference and sampling methods. This work is
-inspired by the R package (bnlearn.com) that has been very usefull to me for
-many years. Although there are very good Python packages for probabilistic
-graphical models, it still can remain difficult (and somethimes unnecessarily)
-to (re)build certain pipelines. Bnlearn for python (this package) is build on
-the pgmpy package and contains the most-wanted pipelines. Navigate to [API
-documentations](https://erdogant.github.io/bnlearn/) for more detailed
-information. # **â­ï¸ Star this repo if you like it â­ï¸** # ### Blogs Read
-the blogs to get a structured overview of bayesian methods and detailed usage
-of ``bnlearn``. * [Step-by-step guide for structure learning.](https://
-erdogant.github.io/bnlearn/pages/html/Documentation.html#medium-blog) * [Step-
-by-step guide for knowledge-driven models.](https://erdogant.github.io/bnlearn/
-pages/html/Documentation.html#medium-blog) # ### [Documentation pages](https://
+erdogant/bnlearn/blob/master/LICENSE) [![Forks](https://img.shields.io/github/
+forks/erdogant/bnlearn.svg)](https://github.com/erdogant/bnlearn/network) [!
+[Open Issues](https://img.shields.io/github/issues/erdogant/bnlearn.svg)]
+(https://github.com/erdogant/bnlearn/issues) [![Project Status](http://
+www.repostatus.org/badges/latest/active.svg)](http://www.repostatus.org/
+#active) [![Downloads](https://pepy.tech/badge/bnlearn/month)](https://
+pepy.tech/project/bnlearn/) [![Downloads](https://pepy.tech/badge/bnlearn)]
+(https://pepy.tech/project/bnlearn) [![DOI](https://zenodo.org/badge/
+231263493.svg)](https://zenodo.org/badge/latestdoi/231263493) [![Docs](https://
+img.shields.io/badge/Sphinx-Docs-Green)](https://erdogant.github.io/bnlearn/)
+[![Medium](https://img.shields.io/badge/Medium-Blog-green)](https://
+erdogant.github.io/bnlearn/pages/html/Documentation.html#medium-blog) [!
+[Donate](https://img.shields.io/badge/Support%20this%20project-
+grey.svg?logo=github%20sponsors)](https://erdogant.github.io/bnlearn/pages/
+html/Documentation.html#) [![Colab](https://colab.research.google.com/assets/
+colab-badge.svg)](https://erdogant.github.io/bnlearn/pages/html/
+Documentation.html#colab-notebook)   ### ``bnlearn`` is Python package for
+learning the graphical structure of Bayesian networks, parameter learning,
+inference and sampling methods. This work is inspired by the R package
+(bnlearn.com) that has been very usefull to me for many years. Although there
+are very good Python packages for probabilistic graphical models, it still can
+remain difficult (and somethimes unnecessarily) to (re)build certain pipelines.
+Bnlearn for python (this package) is build on the pgmpy package and contains
+the most-wanted pipelines. Navigate to [API documentations](https://
+erdogant.github.io/bnlearn/) for more detailed information. # **â­ï¸ Star
+this repo if you like it â­ï¸** # ### Blogs Read the blogs to get a
+structured overview of bayesian methods and detailed usage of ``bnlearn``. *
+[Step-by-step guide for structure learning.](https://erdogant.github.io/
+bnlearn/pages/html/Documentation.html#medium-blog) * [Step-by-step guide for
+knowledge-driven models.](https://erdogant.github.io/bnlearn/pages/html/
+Documentation.html#medium-blog) # ### [Documentation pages](https://
 erdogant.github.io/bnlearn/) On the [documentation pages](https://
 erdogant.github.io/bnlearn/) you can find detailed information about the
 working of the ``bnlearn`` with many examples. # ### Installation ##### It is
 advisable to create a new environment (e.g. with Conda). ```bash conda create -
 n env_bnlearn python=3.8 conda activate env_bnlearn ``` ##### Install bnlearn
 from PyPI ```bash pip install bnlearn ``` ##### The following functions are
 available after installation: ```python # Import library import bnlearn as bn #
```

### Comparing `bnlearn-0.7.8/setup.py` & `bnlearn-0.7.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,15 +9,33 @@
 else:
     raise RuntimeError("Unable to find version string in %s." % (VERSIONFILE,))
 
 # Setup ------------
 with open("README.md", "r") as fh:
     long_description = fh.read()
 setuptools.setup(
-     install_requires=["pgmpy>=0.1.13", "networkx>=2.7.1","matplotlib>=3.3.4",'numpy','pandas','tqdm','ismember','sklearn','funcsigs','statsmodels','community','packaging','wget','df2onehot','fsspec','pypickle','tabulate','ipywidgets', 'pyvis'],
+     install_requires=["pgmpy>=0.1.18",
+                       "networkx>=2.7.1",
+                       "matplotlib>=3.3.4",
+                       'numpy',
+                       'pandas',
+                       'tqdm',
+                       'ismember',
+                       'sklearn',
+                       'funcsigs',
+                       'statsmodels',
+                       'python-louvain',
+                       'packaging',
+                       'wget',
+                       'df2onehot',
+                       'fsspec',
+                       'pypickle',
+                       'tabulate',
+                       'ipywidgets',
+                       'pyvis'],
      python_requires='>=3',
      name='bnlearn',
      version=new_version,
      author="Erdogan Taskesen",
      author_email="erdogant@gmail.com",
      description="Python package for learning the graphical structure of Bayesian networks, parameter learning, inference and sampling methods.",
      long_description=long_description,
```

