# Comparing `tmp/ibpmodel-1.1.2.tar.gz` & `tmp/ibpmodel-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ibpmodel-1.1.2.tar", last modified: Thu Mar 30 13:47:49 2023, max compression
+gzip compressed data, was "ibpmodel-1.2.0.tar", last modified: Mon May  8 10:09:12 2023, max compression
```

## Comparing `ibpmodel-1.1.2.tar` & `ibpmodel-1.2.0.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxrwxr-x   0 iw01      (1000) iw01      (1000)        0 2023-03-30 13:47:49.491185 ibpmodel-1.1.2/
--rw-rw-r--   0 iw01      (1000) iw01      (1000)       93 2023-03-29 07:21:17.000000 ibpmodel-1.1.2/.gitignore
--rw-rw-r--   0 iw01      (1000) iw01      (1000)      672 2023-03-29 11:58:52.000000 ibpmodel-1.1.2/.readthedocs.yml
--rw-rw-r--   0 iw01      (1000) iw01      (1000)      617 2023-03-30 10:54:42.000000 ibpmodel-1.1.2/CHANGELOG.rst
--rw-rw-r--   0 iw01      (1000) iw01      (1000)     1067 2023-03-02 13:04:40.000000 ibpmodel-1.1.2/LICENSE
--rw-rw-r--   0 iw01      (1000) iw01      (1000)     4610 2023-03-30 13:47:49.491185 ibpmodel-1.1.2/PKG-INFO
--rw-rw-r--   0 iw01      (1000) iw01      (1000)     3398 2023-03-30 10:05:42.000000 ibpmodel-1.1.2/README.rst
-drwxrwxr-x   0 iw01      (1000) iw01      (1000)        0 2023-03-30 13:47:49.487185 ibpmodel-1.1.2/docs/
--rw-rw-r--   0 iw01      (1000) iw01      (1000)      638 2023-03-02 13:04:40.000000 ibpmodel-1.1.2/docs/Makefile
--rw-rw-r--   0 iw01      (1000) iw01      (1000)      804 2023-03-02 13:04:40.000000 ibpmodel-1.1.2/docs/make.bat
-drwxrwxr-x   0 iw01      (1000) iw01      (1000)        0 2023-03-30 13:47:49.487185 ibpmodel-1.1.2/docs/source/
-drwxrwxr-x   0 iw01      (1000) iw01      (1000)        0 2023-03-30 13:47:49.491185 ibpmodel-1.1.2/docs/source/_static/
--rw-rw-r--   0 iw01      (1000) iw01      (1000)  3933900 2023-03-02 13:04:40.000000 ibpmodel-1.1.2/docs/source/_static/8thSwarmDataQualityWorkshop_slides.pdf
--rw-rw-r--   0 iw01      (1000) iw01      (1000)    81773 2023-03-29 12:42:24.000000 ibpmodel-1.1.2/docs/source/_static/example_plotButterfly.png
--rw-rw-r--   0 iw01      (1000) iw01      (1000)    67180 2023-03-29 13:41:06.000000 ibpmodel-1.1.2/docs/source/_static/example_plotIBP.png
--rw-rw-r--   0 iw01      (1000) iw01      (1000)     1600 2023-03-30 08:50:26.000000 ibpmodel-1.1.2/docs/source/conf.py
--rw-rw-r--   0 iw01      (1000) iw01      (1000)      317 2023-03-02 13:04:40.000000 ibpmodel-1.1.2/docs/source/ibpmodel.rst
--rw-rw-r--   0 iw01      (1000) iw01      (1000)      503 2023-03-30 10:20:17.000000 ibpmodel-1.1.2/docs/source/index.rst
--rw-rw-r--   0 iw01      (1000) iw01      (1000)      605 2023-03-29 09:12:35.000000 ibpmodel-1.1.2/docs/source/installation.rst
--rw-rw-r--   0 iw01      (1000) iw01      (1000)      111 2023-03-02 13:04:40.000000 ibpmodel-1.1.2/docs/source/modules.rst
--rw-rw-r--   0 iw01      (1000) iw01      (1000)      112 2023-03-02 13:04:40.000000 ibpmodel-1.1.2/docs/source/reference.rst
--rw-rw-r--   0 iw01      (1000) iw01      (1000)       74 2023-03-29 13:46:43.000000 ibpmodel-1.1.2/docs/source/requirements.txt
--rw-rw-r--   0 iw01      (1000) iw01      (1000)     3038 2023-03-30 13:39:45.000000 ibpmodel-1.1.2/docs/source/usage.rst
--rw-rw-r--   0 iw01      (1000) iw01      (1000)     1577 2023-03-30 13:35:51.000000 ibpmodel-1.1.2/pyproject.toml
--rw-rw-r--   0 iw01      (1000) iw01      (1000)     1208 2023-03-28 08:37:39.000000 ibpmodel-1.1.2/requirements.txt
--rw-rw-r--   0 iw01      (1000) iw01      (1000)       38 2023-03-30 13:47:49.491185 ibpmodel-1.1.2/setup.cfg
-drwxrwxr-x   0 iw01      (1000) iw01      (1000)        0 2023-03-30 13:47:49.487185 ibpmodel-1.1.2/src/
-drwxrwxr-x   0 iw01      (1000) iw01      (1000)        0 2023-03-30 13:47:49.491185 ibpmodel-1.1.2/src/ibpmodel/
--rw-rw-r--   0 iw01      (1000) iw01      (1000)  1212651 2023-03-22 11:18:00.000000 ibpmodel-1.1.2/src/ibpmodel/SW_OPER_IBP_CLI_2__00000000T000000_99999999T999999_0002.cdf
--rw-rw-r--   0 iw01      (1000) iw01      (1000)      325 2023-03-30 08:50:04.000000 ibpmodel-1.1.2/src/ibpmodel/__init__.py
--rw-rw-r--   0 iw01      (1000) iw01      (1000)    22961 2023-03-22 14:00:40.000000 ibpmodel-1.1.2/src/ibpmodel/ibpcalc.py
--rw-rw-r--   0 iw01      (1000) iw01      (1000)     6706 2023-03-30 08:36:25.000000 ibpmodel-1.1.2/src/ibpmodel/ibpforward.py
-drwxrwxr-x   0 iw01      (1000) iw01      (1000)        0 2023-03-30 13:47:49.491185 ibpmodel-1.1.2/src/ibpmodel.egg-info/
--rw-rw-r--   0 iw01      (1000) iw01      (1000)     4610 2023-03-30 13:47:49.000000 ibpmodel-1.1.2/src/ibpmodel.egg-info/PKG-INFO
--rw-rw-r--   0 iw01      (1000) iw01      (1000)      826 2023-03-30 13:47:49.000000 ibpmodel-1.1.2/src/ibpmodel.egg-info/SOURCES.txt
--rw-rw-r--   0 iw01      (1000) iw01      (1000)        1 2023-03-30 13:47:49.000000 ibpmodel-1.1.2/src/ibpmodel.egg-info/dependency_links.txt
--rw-rw-r--   0 iw01      (1000) iw01      (1000)       65 2023-03-30 13:47:49.000000 ibpmodel-1.1.2/src/ibpmodel.egg-info/requires.txt
--rw-rw-r--   0 iw01      (1000) iw01      (1000)        9 2023-03-30 13:47:49.000000 ibpmodel-1.1.2/src/ibpmodel.egg-info/top_level.txt
-drwxrwxr-x   0 iw01      (1000) iw01      (1000)        0 2023-03-30 13:47:49.491185 ibpmodel-1.1.2/tests/
--rw-rw-r--   0 iw01      (1000) iw01      (1000)        0 2023-03-02 13:04:40.000000 ibpmodel-1.1.2/tests/conftest.py
--rw-rw-r--   0 iw01      (1000) iw01      (1000)      802 2023-03-30 10:07:02.000000 ibpmodel-1.1.2/tests/test_ibp.py
+drwxrwxr-x   0 iw01      (1000) iw01      (1000)        0 2023-05-08 10:09:12.730227 ibpmodel-1.2.0/
+-rw-rw-r--   0 iw01      (1000) iw01      (1000)       93 2023-03-29 07:21:17.000000 ibpmodel-1.2.0/.gitignore
+-rw-rw-r--   0 iw01      (1000) iw01      (1000)      672 2023-03-29 11:58:52.000000 ibpmodel-1.2.0/.readthedocs.yml
+-rw-rw-r--   0 iw01      (1000) iw01      (1000)      617 2023-03-30 10:54:42.000000 ibpmodel-1.2.0/CHANGELOG.rst
+-rw-rw-r--   0 iw01      (1000) iw01      (1000)     1067 2023-03-02 13:04:40.000000 ibpmodel-1.2.0/LICENSE
+-rw-rw-r--   0 iw01      (1000) iw01      (1000)     5398 2023-05-08 10:09:12.730227 ibpmodel-1.2.0/PKG-INFO
+-rw-rw-r--   0 iw01      (1000) iw01      (1000)     4186 2023-04-13 08:01:15.000000 ibpmodel-1.2.0/README.rst
+drwxrwxr-x   0 iw01      (1000) iw01      (1000)        0 2023-05-08 10:09:12.722227 ibpmodel-1.2.0/docs/
+-rw-rw-r--   0 iw01      (1000) iw01      (1000)      638 2023-03-02 13:04:40.000000 ibpmodel-1.2.0/docs/Makefile
+-rw-rw-r--   0 iw01      (1000) iw01      (1000)      804 2023-03-02 13:04:40.000000 ibpmodel-1.2.0/docs/make.bat
+drwxrwxr-x   0 iw01      (1000) iw01      (1000)        0 2023-05-08 10:09:12.722227 ibpmodel-1.2.0/docs/source/
+drwxrwxr-x   0 iw01      (1000) iw01      (1000)        0 2023-05-08 10:09:12.726227 ibpmodel-1.2.0/docs/source/_static/
+-rw-rw-r--   0 iw01      (1000) iw01      (1000)  3933900 2023-03-02 13:04:40.000000 ibpmodel-1.2.0/docs/source/_static/8thSwarmDataQualityWorkshop_slides.pdf
+-rw-rw-r--   0 iw01      (1000) iw01      (1000)    81773 2023-03-29 12:42:24.000000 ibpmodel-1.2.0/docs/source/_static/example_plotButterfly.png
+-rw-rw-r--   0 iw01      (1000) iw01      (1000)    67180 2023-03-29 13:41:06.000000 ibpmodel-1.2.0/docs/source/_static/example_plotIBP.png
+-rw-rw-r--   0 iw01      (1000) iw01      (1000)   158206 2023-05-08 06:38:12.000000 ibpmodel-1.2.0/docs/source/_static/example_subplot.png
+-rw-rw-r--   0 iw01      (1000) iw01      (1000)       32 2023-03-30 10:10:13.000000 ibpmodel-1.2.0/docs/source/changelog.rst
+-rw-rw-r--   0 iw01      (1000) iw01      (1000)     1658 2023-04-18 05:52:28.000000 ibpmodel-1.2.0/docs/source/conf.py
+-rw-rw-r--   0 iw01      (1000) iw01      (1000)      317 2023-03-02 13:04:40.000000 ibpmodel-1.2.0/docs/source/ibpmodel.rst
+-rw-rw-r--   0 iw01      (1000) iw01      (1000)      503 2023-03-30 10:20:17.000000 ibpmodel-1.2.0/docs/source/index.rst
+-rw-rw-r--   0 iw01      (1000) iw01      (1000)      588 2023-04-13 06:57:00.000000 ibpmodel-1.2.0/docs/source/installation.rst
+-rw-rw-r--   0 iw01      (1000) iw01      (1000)      111 2023-03-02 13:04:40.000000 ibpmodel-1.2.0/docs/source/modules.rst
+-rw-rw-r--   0 iw01      (1000) iw01      (1000)      112 2023-03-02 13:04:40.000000 ibpmodel-1.2.0/docs/source/reference.rst
+-rw-rw-r--   0 iw01      (1000) iw01      (1000)       89 2023-04-12 12:08:33.000000 ibpmodel-1.2.0/docs/source/requirements.txt
+-rw-rw-r--   0 iw01      (1000) iw01      (1000)     2195 2023-05-08 06:38:12.000000 ibpmodel-1.2.0/docs/source/usage.rst
+-rw-rw-r--   0 iw01      (1000) iw01      (1000)     1577 2023-03-30 13:35:51.000000 ibpmodel-1.2.0/pyproject.toml
+-rw-rw-r--   0 iw01      (1000) iw01      (1000)     1173 2023-04-13 08:08:08.000000 ibpmodel-1.2.0/requirements.txt
+-rw-rw-r--   0 iw01      (1000) iw01      (1000)       38 2023-05-08 10:09:12.730227 ibpmodel-1.2.0/setup.cfg
+drwxrwxr-x   0 iw01      (1000) iw01      (1000)        0 2023-05-08 10:09:12.722227 ibpmodel-1.2.0/src/
+drwxrwxr-x   0 iw01      (1000) iw01      (1000)        0 2023-05-08 10:09:12.726227 ibpmodel-1.2.0/src/ibpmodel/
+-rw-rw-r--   0 iw01      (1000) iw01      (1000)  1212651 2023-03-22 11:18:00.000000 ibpmodel-1.2.0/src/ibpmodel/SW_OPER_IBP_CLI_2__00000000T000000_99999999T999999_0002.cdf
+-rw-rw-r--   0 iw01      (1000) iw01      (1000)      325 2023-04-13 09:35:36.000000 ibpmodel-1.2.0/src/ibpmodel/__init__.py
+-rw-rw-r--   0 iw01      (1000) iw01      (1000)    22302 2023-05-08 07:46:52.000000 ibpmodel-1.2.0/src/ibpmodel/ibpcalc.py
+-rw-rw-r--   0 iw01      (1000) iw01      (1000)    10169 2023-05-08 06:38:12.000000 ibpmodel-1.2.0/src/ibpmodel/ibpforward.py
+drwxrwxr-x   0 iw01      (1000) iw01      (1000)        0 2023-05-08 10:09:12.730227 ibpmodel-1.2.0/src/ibpmodel.egg-info/
+-rw-rw-r--   0 iw01      (1000) iw01      (1000)     5398 2023-05-08 10:09:12.000000 ibpmodel-1.2.0/src/ibpmodel.egg-info/PKG-INFO
+-rw-rw-r--   0 iw01      (1000) iw01      (1000)      900 2023-05-08 10:09:12.000000 ibpmodel-1.2.0/src/ibpmodel.egg-info/SOURCES.txt
+-rw-rw-r--   0 iw01      (1000) iw01      (1000)        1 2023-05-08 10:09:12.000000 ibpmodel-1.2.0/src/ibpmodel.egg-info/dependency_links.txt
+-rw-rw-r--   0 iw01      (1000) iw01      (1000)       65 2023-05-08 10:09:12.000000 ibpmodel-1.2.0/src/ibpmodel.egg-info/requires.txt
+-rw-rw-r--   0 iw01      (1000) iw01      (1000)        9 2023-05-08 10:09:12.000000 ibpmodel-1.2.0/src/ibpmodel.egg-info/top_level.txt
+drwxrwxr-x   0 iw01      (1000) iw01      (1000)        0 2023-05-08 10:09:12.730227 ibpmodel-1.2.0/template/
+-rw-rw-r--   0 iw01      (1000) iw01      (1000)  1189939 2023-05-08 09:55:14.000000 ibpmodel-1.2.0/template/IBP_CLI_2_bubble-probability.ipynb
```

### Comparing `ibpmodel-1.1.2/.readthedocs.yml` & `ibpmodel-1.2.0/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `ibpmodel-1.1.2/CHANGELOG.rst` & `ibpmodel-1.2.0/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `ibpmodel-1.1.2/LICENSE` & `ibpmodel-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ibpmodel-1.1.2/PKG-INFO` & `ibpmodel-1.2.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibpmodel
-Version: 1.1.2
+Version: 1.2.0
 Summary: Ionospheric Bubble Probability
 Author: Martin Rother
 Maintainer-email: Ina Wehner <wehner@iap-kborn.de>
 License: MIT License
 Project-URL: homepage, https://igit.iap-kborn.de/ibp/ibp-model.git
 Project-URL: documentation, https://ibp-model.readthedocs.io
 Project-URL: repository, https://igit.iap-kborn.de/ibp/ibp-model.git
@@ -69,15 +69,15 @@
 ^^^^^
 The return value of the function *ibpmodel.calculateIBPindex()* is of type pandas.DataFrame.
 
 
 .. code-block:: python
 
     >>> from ibpmodel import *
-    >>> calculateIBPindex(day_month=15,    # Day of Year or Month 
+    >>> calculateIBPindex(day_month=15,               # Day of Year or Month 
                   longitude=0,                        # Longitude in degree
                   local_time=20.9,                    # Local time in hours 
                   f107=150)                           # F10.7 cm Solar Flux index
        Doy  Month  Lon    LT  F10.7     IBP
     0   15      1    0  20.9    150  0.3547
 
 .. code-block:: python
@@ -126,8 +126,40 @@
 
 *Stolle et al.*, `An empirical climatological model of the occurrence of F region equatorial plasma irregularities <https://igit.iap-kborn.de/ibp/ibp-model/-/raw/main/docs/source/_static/8thSwarmDataQualityWorkshop_slides.pdf>`_, 8th Swarm data quality workshop at ESA/ESRIN, October 2017. 
 
 *Lucas Schreiter*, Anwendungsorientierte Modellierung der Auftretenswahrscheinlichkeit und relativen Häufigkeit von äquatorialen Plasmabubbles,  Master's thesis, Institute of Mathematics, University of Potsdam, 2016. (in German only.)
 
 .. inclusion-marker-acknow
 
+Information for developers
+--------------------------
 
+Setup environment
+^^^^^^^^^^^^^^^^^
+
+.. code-block:: console
+
+    $ git clone https://igit.iap-kborn.de/ibp/ibp-model.git
+    $ cd ibp-model
+    $ pip install -r requirements.txt
+    $ pip install -e .
+
+Test of package using doctest
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+.. code-block:: console
+
+    $ python src/ibpmodel/ibpcalc.py
+
+No error should occur.
+
+
+Test run of the documentation
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+.. code-block:: console
+
+    $ cd docs
+    $ make clean && make html
+
+The *docs/build/html/* directory contains the html files. Open *index.html* in browser. 
+The results of the code examples on the usage page are generated automatically. Therefore the ibpmodel package must be installed (*pip install -e .*).
```

### Comparing `ibpmodel-1.1.2/README.rst` & `ibpmodel-1.2.0/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 ^^^^^
 The return value of the function *ibpmodel.calculateIBPindex()* is of type pandas.DataFrame.
 
 
 .. code-block:: python
 
     >>> from ibpmodel import *
-    >>> calculateIBPindex(day_month=15,    # Day of Year or Month 
+    >>> calculateIBPindex(day_month=15,               # Day of Year or Month 
                   longitude=0,                        # Longitude in degree
                   local_time=20.9,                    # Local time in hours 
                   f107=150)                           # F10.7 cm Solar Flux index
        Doy  Month  Lon    LT  F10.7     IBP
     0   15      1    0  20.9    150  0.3547
 
 .. code-block:: python
@@ -98,8 +98,40 @@
 
 *Stolle et al.*, `An empirical climatological model of the occurrence of F region equatorial plasma irregularities <https://igit.iap-kborn.de/ibp/ibp-model/-/raw/main/docs/source/_static/8thSwarmDataQualityWorkshop_slides.pdf>`_, 8th Swarm data quality workshop at ESA/ESRIN, October 2017. 
 
 *Lucas Schreiter*, Anwendungsorientierte Modellierung der Auftretenswahrscheinlichkeit und relativen Häufigkeit von äquatorialen Plasmabubbles,  Master's thesis, Institute of Mathematics, University of Potsdam, 2016. (in German only.)
 
 .. inclusion-marker-acknow
 
+Information for developers
+--------------------------
 
+Setup environment
+^^^^^^^^^^^^^^^^^
+
+.. code-block:: console
+
+    $ git clone https://igit.iap-kborn.de/ibp/ibp-model.git
+    $ cd ibp-model
+    $ pip install -r requirements.txt
+    $ pip install -e .
+
+Test of package using doctest
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+.. code-block:: console
+
+    $ python src/ibpmodel/ibpcalc.py
+
+No error should occur.
+
+
+Test run of the documentation
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+.. code-block:: console
+
+    $ cd docs
+    $ make clean && make html
+
+The *docs/build/html/* directory contains the html files. Open *index.html* in browser. 
+The results of the code examples on the usage page are generated automatically. Therefore the ibpmodel package must be installed (*pip install -e .*).
```

### Comparing `ibpmodel-1.1.2/docs/Makefile` & `ibpmodel-1.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ibpmodel-1.1.2/docs/make.bat` & `ibpmodel-1.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ibpmodel-1.1.2/docs/source/_static/8thSwarmDataQualityWorkshop_slides.pdf` & `ibpmodel-1.2.0/docs/source/_static/8thSwarmDataQualityWorkshop_slides.pdf`

 * *Files identical despite different names*

### Comparing `ibpmodel-1.1.2/docs/source/_static/example_plotButterfly.png` & `ibpmodel-1.2.0/docs/source/_static/example_plotButterfly.png`

 * *Files identical despite different names*

### Comparing `ibpmodel-1.1.2/docs/source/_static/example_plotIBP.png` & `ibpmodel-1.2.0/docs/source/_static/example_plotIBP.png`

 * *Files identical despite different names*

### Comparing `ibpmodel-1.1.2/docs/source/conf.py` & `ibpmodel-1.2.0/docs/source/conf.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # -- Path setup --------------------------------------------------------------
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 #
 import os
 import sys
+
 sys.path.insert(0, os.path.abspath('../../src'))
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 from ibpmodel import __version__ as ibp_version
 
@@ -25,17 +26,18 @@
 
 extensions = [
     'sphinx_rtd_theme',
     'sphinx.ext.duration',
     'sphinx.ext.autodoc',
     'sphinx.ext.autosummary',
     'sphinx.ext.napoleon',
-    'sphinx.ext.viewcode' 
+    'sphinx.ext.viewcode',
+    'sphinx_autorun'
 ]
-
+#extensions.append('sphinx_autorun')
 templates_path = ['_templates']
 exclude_patterns = []
 autodoc_mock_imports = ['numpy', 'pandas', 'cdflib','matplotlib','scipy']
 
 
 
 # -- Options for HTML output -------------------------------------------------
```

### Comparing `ibpmodel-1.1.2/docs/source/installation.rst` & `ibpmodel-1.2.0/docs/source/installation.rst`

 * *Files 20% similar despite different names*

```diff
@@ -21,10 +21,10 @@
 
 ibpmodel can also be installed directly from source. The source code can then be downloaded from IAP GitLab and installed:
 
 .. code-block:: console
 
    $ git clone https://igit.iap-kborn.de/ibp/ibp-model.git
    $ cd ibpmodel 
-   $ python setup.py install --user
+   $ pip install .
```

### Comparing `ibpmodel-1.1.2/docs/source/usage.rst` & `ibpmodel-1.2.0/docs/source/usage.rst`

 * *Files 24% similar despite different names*

```diff
@@ -2,74 +2,42 @@
 =====
 
 Calculation of IBP Index
 ------------------------
 
 To calculate the IBP index use :py:func:`ibpmodel.ibpforward.calculateIBPindex()` function. It returns a pandas.DataFrame:
 
-.. code-block:: python
+.. runblock:: pycon
 
    >>> from ibpmodel import calculateIBPindex
    >>> calculateIBPindex(day_month=15, longitude=0, local_time=20.9, f107=150)                           
-       Doy  Month  Lon    LT  F10.7     IBP
-   0   15      1    0  20.9    150  0.3547
 
-  
-.. code-block:: python
+.. runblock:: pycon
 
+   >>> from ibpmodel import calculateIBPindex
    >>> calculateIBPindex(day_month=['Jan','Feb','Mar'], local_time=22)
-        Doy  Month  Lon  LT  F10.7     IBP
-   0     15      1 -180  22    150  0.0739
-   1     15      1 -175  22    150  0.0722
-   2     15      1 -170  22    150  0.0717
-   3     15      1 -165  22    150  0.0728
-   4     15      1 -160  22    150  0.0771
-   ..   ...    ...  ...  ..    ...     ...
-   211   74      3  155  22    150  0.2061
-   212   74      3  160  22    150  0.2025
-   213   74      3  165  22    150  0.1994
-   214   74      3  170  22    150  0.1967
-   215   74      3  175  22    150  0.1943
 
-   [216 rows x 6 columns]
+.. runblock:: pycon
 
-  
-.. code-block:: python
+   >>> from ibpmodel import calculateIBPindex
+   >>> calculateIBPindex(day_month=[1,15,31], longitude=[-170,175,170], local_time=0, f107=120)
 
-   >>> calculateIBPindex(day_month=[1,15,31], longitude=[-170,175,170], 
-      local_time=0, f107=120)
-      Doy  Month  Lon  LT  F10.7     IBP
-   0    1      1 -170   0    120  0.0274
-   1    1      1  175   0    120  0.0304
-   2    1      1  170   0    120  0.0324
-   3   15      1 -170   0    120  0.0293
-   4   15      1  175   0    120  0.0325
-   5   15      1  170   0    120  0.0347
-   6   31      1 -170   0    120  0.0341
-   7   31      1  175   0    120  0.0378
-   8   31      1  170   0    120  0.0403
 
 Read coefficient file
 ---------------------
 
 You can load the coefficient file. :py:func:`ibpmodel.ibpcalc.read_model_file()`:
 
-.. code-block:: python
+.. runblock:: pycon
 
    >>> from ibpmodel import read_model_file
    >>> c = read_model_file()
    >>> c.keys()
-   dict_keys(['Parameters', 'Intensity', 'Monthly_LT_Shift', 'Density_Estimators', 
-      'Density_Estimator_Lons'])
-   >>> c['Intensity']
-   array([  -6.99518975,   -0.93264132,   96.49049553,    8.81167779,
-         -135.50937181])
-
-
 
+   >>> c['Intensity']
 
 
 Plotting of the probability
 ---------------------------
 
 There are two functions to plot IBP index. function :py:func:`ibpmodel.ibpforward.plotIBPindex()` and :py:func:`ibpmodel.ibpforward.plotButterflyData()`.
 By default, the plot is displayed immediately. If you want to make changes or additions, the parameter getFig must be set equal to ``True``. 
@@ -89,12 +57,20 @@
 
 .. image:: _static/example_plotButterfly.png
    :alt: Contour plot of result from function ButterflyData() 
    :align: center
 
 .. code-block:: python
    
+   >>> import ibpmodel as ibp
    >>> import matplotlib.pyplot as plt
-   >>> ax=ibp.plotIBPindex(310,getFig=True)
+   >>> doys = [349, 15]
+   >>> fig, axes = plt.subplots(len(doys),1, layout='constrained',figsize=(9, 7))
+   >>> for d, ax in zip(doys, axes):
+   ...     ax, scalarmap = ibp.plotIBPindex(d, ax=ax)
+   >>> ibp.ibpforward.setcolorbar(scalarmap, fig, axes, fraction=0.05)
    >>> plt.show()
 
-
+.. image:: _static/example_subplot.png
+   :alt: Subplot of IBP index
+   :align: center
+
```

### Comparing `ibpmodel-1.1.2/pyproject.toml` & `ibpmodel-1.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ibpmodel-1.1.2/requirements.txt` & `ibpmodel-1.2.0/requirements.txt`

 * *Files 18% similar despite different names*

```diff
@@ -5,61 +5,59 @@
 cdflib==0.4.9
 certifi==2022.12.7
 cffi==1.15.1
 charset-normalizer==3.1.0
 contourpy==1.0.7
 cryptography==40.0.1
 cycler==0.11.0
-distlib==0.3.6
 docutils==0.18.1
-filelock==3.10.7
-fonttools==4.39.2
+fonttools==4.39.3
 idna==3.4
 imagesize==1.4.1
-importlib-metadata==6.1.0
+importlib-metadata==6.3.0
 jaraco.classes==3.2.3
 jeepney==0.8.0
 Jinja2==3.1.2
 keyring==23.13.1
 kiwisolver==1.4.4
 markdown-it-py==2.2.0
 MarkupSafe==2.1.2
 matplotlib==3.7.1
 mdurl==0.1.2
 more-itertools==9.1.0
 numpy==1.24.2
 numpydoc==1.5.0
-packaging==23.0
-pandas==1.5.3
-Pillow==9.4.0
+packaging==23.1
+pandas==2.0.0
+Pillow==9.5.0
 pkginfo==1.9.6
-platformdirs==3.2.0
 pycparser==2.21
-Pygments==2.14.0
+Pygments==2.15.0
 pyparsing==3.0.9
 pyproject_hooks==1.0.0
 python-dateutil==2.8.2
-pytz==2023.2
+pytz==2023.3
 readme-renderer==37.3
 requests==2.28.2
 requests-toolbelt==0.10.1
 rfc3986==2.0.0
-rich==13.3.3
+rich==13.3.4
 scipy==1.10.1
 SecretStorage==3.3.3
 six==1.16.0
 snowballstemmer==2.2.0
 Sphinx==6.1.3
+sphinx-autorun==1.1.1
 sphinx-rtd-theme==1.2.0
 sphinxcontrib-applehelp==1.0.4
 sphinxcontrib-devhelp==1.0.2
 sphinxcontrib-htmlhelp==2.0.1
 sphinxcontrib-jquery==4.1
 sphinxcontrib-jsmath==1.0.1
 sphinxcontrib-qthelp==1.0.3
 sphinxcontrib-serializinghtml==1.1.5
 tomli==2.0.1
 twine==4.0.2
+tzdata==2023.3
 urllib3==1.26.15
-virtualenv==20.21.0
 webencodings==0.5.1
 zipp==3.15.0
```

### Comparing `ibpmodel-1.1.2/src/ibpmodel/SW_OPER_IBP_CLI_2__00000000T000000_99999999T999999_0002.cdf` & `ibpmodel-1.2.0/src/ibpmodel/SW_OPER_IBP_CLI_2__00000000T000000_99999999T999999_0002.cdf`

 * *Files identical despite different names*

### Comparing `ibpmodel-1.1.2/src/ibpmodel/ibpcalc.py` & `ibpmodel-1.2.0/src/ibpmodel/ibpcalc.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,22 +29,21 @@
         A list of ordered combination of the input arguments.
 
     Examples
     --------
 
     >>> from ibpmodel import ibpcalc
     >>> ibpcalc.tiler([1, 2, 3],['A', 'B'])
-    [array([1, 1, 2, 2, 3, 3]), 
-     array(['A', 'B', 'A', 'B', 'A', 'B'], dtype='<U1')]
+    [array([1, 1, 2, 2, 3, 3]), array(['A', 'B', 'A', 'B', 'A', 'B'], dtype='<U1')]
 
     >>> ibpcalc.tiler([17,13],[1, 2, 3],['A', 'B'])
-    [array([17, 17, 17, 17, 17, 17, 13, 13, 13, 13, 13, 13]), 
-     array([1, 1, 2, 2, 3, 3, 1, 1, 2, 2, 3, 3]), 
-     array(['A', 'B', 'A', 'B', 'A', 'B', 'A', 'B', 'A', 'B', 'A', 'B'], 
-           dtype='<U1')]
+    [array([17, 17, 17, 17, 17, 17, 13, 13, 13, 13, 13, 13]), \
+array([1, 1, 2, 2, 3, 3, 1, 1, 2, 2, 3, 3]), \
+array(['A', 'B', 'A', 'B', 'A', 'B', 'A', 'B', 'A', 'B', 'A', 'B'],
+          dtype='<U1')]
 
     """
 
     arg_number = len(args)
     if arg_number < 1:
         return None
     elif arg_number == 1:
@@ -83,19 +82,19 @@
     >>> from ibpmodel import ibpcalc
     >>> ibpcalc.tile_aggregate(np.array([3,2,3,3,2,1,2,1]), [10,12], [20,21,22,24])
     (10, 12, array([2.75, 1.5 ]))
     
     >>> ibpcalc.tile_aggregate(np.array([3,2]), np.array([12]), np.array([20,21]))
     (12, array([2.5]))
     
-    >>> ibpcalc.tile_aggregate(
-        np.array([3,2,2,1,4,2,3,3,1,4,8,5,9,6,7,4,5,2,1,6,7,9,5,7]), 
-        [9,10,11], [20,21]), [7,8,5,6])
-    (array([ 9,  9, 10, 10, 11, 11]), array([20, 21, 20, 21, 20, 21]), 
-    array([2. , 3. , 4.5, 6.5, 3.5, 7. ]))
+    >>> ibpcalc.tile_aggregate(\
+np.array([3,2,2,1,4,2,3,3,1,4,8,5,9,6,7,4,5,2,1,6,7,9,5,7]), \
+[9,10,11], [20,21], [7,8,5,6])
+    (array([ 9,  9, 10, 10, 11, 11]), array([20, 21, 20, 21, 20, 21]), \
+array([2. , 3. , 4.5, 6.5, 3.5, 7. ]))
 
     """
     if len(args) <= 1:
         return aggregator(result)
     *preserved, collapesed = args
     reshaped= result.reshape(np.product(list(map(len,preserved))),len(collapesed))
     return (*tiler(*preserved), aggregator(reshaped, axis=1))
@@ -112,14 +111,15 @@
     -------
     int
         Day of year.
 
     Example
     -------
 
+    >>> from ibpmodel import ibpcalc
     >>> ibpcalc.doyFromMonth(7)
     196
 
     '''
     doy_month = [15, 46, 74, 105, 135, 166, 196, 227, 258, 288, 319, 349]
     if isinstance(month, (int,np.integer)) and month in range(1,13):
         return doy_month[month-1]
@@ -138,14 +138,15 @@
     -------
     int
         Value as the month in the year, with january being month 1.
 
     Example
     -------
 
+    >>> from ibpmodel import ibpcalc
     >>> ibpcalc.monthFromDoy(275)
     10
     '''
     if isinstance(doy, (int,np.integer)) and doy in range(1,366):
         return int(datetime.strptime(str(doy), '%j').month) 
     else:
         raise ValueError("Value " + str(doy) + " out of range or wrong type!")
@@ -162,14 +163,15 @@
     -------
     int
         Value as the month in the year, with january being month 1.
 
     Example
     -------
 
+    >>> from ibpmodel import ibpcalc
     >>> ibpcalc.monthfromString('Mar')
     3
     '''
     months = [ datetime(2000,m,1).strftime("%b") for m in range(1,13) ]
     if isinstance(month_str, str) and month_str in months:
         return months.index(month_str)+1
     else:
@@ -187,17 +189,18 @@
     -------
     doy_out : list of int(s)
         list of days of the year
 
     Example
     -------
 
+    >>> from ibpmodel import ibpcalc
     >>> ibpcalc.checkDoyMonth(['Mar',200,1])
     [74, 200, 1]
-    
+
     >>> ibpcalc.checkDoyMonth('Dec')
     [349]
     '''
     if not isinstance(day_month, list):
         day_month = [day_month]
     
     doy_out = []
@@ -225,14 +228,15 @@
     -------
     numpy.array
         Numpy.array contains *para*.
 
     Example
     -------
 
+    >>> from ibpmodel import ibpcalc
     >>> ibpcalc.checkParameter(3,range(0,5))
     array([3])
     
     >>> ibpcalc.checkParameter([0,1,2,3,4],range(0,5))
     array([0, 1, 2, 3, 4])
     '''
     if isinstance(para, (list,np.ndarray)) and not False in list(map(lambda i: True if para_range[0] <= i <= para_range[-1] else False, para)):
@@ -449,32 +453,32 @@
     float or ndarray of floats
 
     Examples
     --------
 
     >>> from ibpmodel import ibpcalc
     >>> import numpy as np
-    >>> ibpcalc.compute_lambda(1,[-232.54229262, 4.67324294], 123.4, 17.3, 
-        np.array([2.1,3.0]) )
+    >>> ibpcalc.compute_lambda(1,[-232.54229262, 4.67324294], 123.4, 17.3, \
+np.array([2.1,3.0]))
     1084.307658528
 
     >>> params = np.array([-232.54229262, 4.67324294, 1.34695254, -1.31448553, 1.09712955])
     >>> densi_once = np.sin(np.arange(360)*np.pi/180) * 3 + 5
-    >>> ibpcalc.compute_lambda(1,[-232.54229262, 4.67324294], 123.4, 17.3, densi_once )
+    >>> ibpcalc.compute_lambda(1,[-232.54229262, 4.67324294], 123.4, 17.3, densi_once)
     1788.2556529203105
     
-    >>> densi_year = np.array([ (densi_once -3)* np.cos(month*np.pi/6) 
-        + 8 for month in range(12)])
-    >>> ibpcalc.compute_lambda(1,[-232.54229262, 4.67324294], 123.4, 17.3, densi_year, 
-        month=5)
+    >>> densi_year = np.array([ (densi_once -3)* np.cos(month*np.pi/6) \
++ 8 for month in range(12)])
+    >>> ibpcalc.compute_lambda(1,[-232.54229262, 4.67324294], 123.4, 17.3, densi_year, \
+month=5)
     1851.5944384882494
     
     >>> months = np.array((np.sin(np.arange(20))+1) % 12, dtype='int')
-    >>> ibpcalc.compute_lambda(1,[-232.54229262, 4.67324294], 123.4, 17.3, 
-        densi_year[:,months], month=months)
+    >>> ibpcalc.compute_lambda(1,[-232.54229262, 4.67324294], 123.4, 17.3, \
+densi_year[:,months], month=months)
     array([2149.6915391, 2149.6915391, 2149.6915391, 2149.6915391,
            2149.6915391, 2149.6915391, 2149.6915391, 2149.6915391,
            2149.6915391, 2149.6915391, 2149.6915391, 2149.6915391,
            2149.6915391, 2149.6915391, 2149.6915391, 2149.6915391,
            2149.6915391, 2149.6915391, 2149.6915391, 2149.6915391])
 
     """
@@ -493,15 +497,15 @@
 
 def align_time_of_year(day_of_year, month):
     """Guess day of year and month from each other.
     
     Parameters
     ----------
     day_of_year : int or ndarray of ints
-        Time as the day of year, restricted to ``0 < day_of_year <= 356``,
+        Time as the day of year, restricted to ``0 < day_of_year <= 365``,
         with the value 0 meaning it should be calculated based on `month`
         (which gives the median day of the `month`).
     month : int or ndarray of ints
         Time as the month in the year, with january being month 1,
         so ``0 < month <= 12``.
     
     Returns
@@ -514,26 +518,21 @@
     Examples
     --------
 
     >>> from ibpmodel import ibpcalc
     >>> import numpy as np
     >>> ibpcalc.align_time_of_year(0,6)
     (166, 6)
-
     >>> ibpcalc.align_time_of_year(162,3)
     (162, 6)
-
     >>> ibpcalc.align_time_of_year(0,np.arange(12)+1)
-    (array([ 16,  45,  75, 105, 136, 166, 197, 228, 258, 289, 319, 350]), 
-     array([ 1,  2,  3,  4,  5,  6,  7,  8,  9, 10, 11, 12]))
+    (array([ 16,  45,  75, 105, 136, 166, 197, 228, 258, 289, 319, 350]), array([ 1,  2,  3,  4,  5,  6,  7,  8,  9, 10, 11, 12]))
 
-    >>> ibpcalc.align_time_of_year(
-        np.array([0,33,21,17,267,0,115,96,315,0,172,256]),np.arange(12)+1)
-    (array([ 16,  33,  21,  17, 267, 166, 115,  96, 315, 289, 172, 256]), 
-     array([ 1,  2,  1,  1,  9,  6,  4,  4, 11, 10,  6,  9]))
+    >>> ibpcalc.align_time_of_year(np.array([0,33,21,17,267,0,115,96,315,0,172,256]),np.arange(12)+1)
+    (array([ 16,  33,  21,  17, 267, 166, 115,  96, 315, 289, 172, 256]), array([ 1,  2,  1,  1,  9,  6,  4,  4, 11, 10,  6,  9]))
     
     """
 
     # This is a side-effect free version by Ask Neve Gamby.
     #
     # 2019-03-05: Now always recalculating 'month' (clumsy type handling?),
     #             Martin Rother (rother@gfz-potsdam.de).
@@ -603,31 +602,19 @@
         
     Examples
     --------
 
     >>> from ibpmodel import ibpcalc
     >>> import numpy as np
     >>> data = ibpcalc.read_model_file()
-    >>> ibpcalc.compute_probability_exp(0, 3, 12, 2, 17.3, data)
-    0.0016535983798842135
-    
-    >>> ibpcalc.compute_probability_exp(0, 2, 12, 2, 17.3, data)
-    0.0
+    >>> ibpcalc.compute_probability_exp(0, 3, 12, 2, 150, data)
+    0.04537450559812162
     
-    >>> parts = ibpcalc.tiler(np.arange(2,5), np.array([12,124]), np.arange(6))
-    >>> ibpcalc.compute_probability_exp(0, *parts, f107=17.3, data=data)
-    array([0.00000000e+00, 0.00000000e+00, 0.00000000e+00, 0.00000000e+00,
-           0.00000000e+00, 0.00000000e+00, 0.00000000e+00, 0.00000000e+00,
-           0.00000000e+00, 0.00000000e+00, 0.00000000e+00, 0.00000000e+00,
-           7.24797932e-03, 3.47038779e-03, 1.65359838e-03, 7.87395045e-04,
-           3.74847713e-04, 1.78430902e-04, 2.71409055e-03, 1.30214944e-03,
-           6.20242441e-04, 2.95263158e-04, 1.40545020e-04, 6.68965929e-05,
-           0.00000000e+00, 0.00000000e+00, 0.00000000e+00, 0.00000000e+00,
-           0.00000000e+00, 0.00000000e+00, 0.00000000e+00, 0.00000000e+00,
-           0.00000000e+00, 0.00000000e+00, 0.00000000e+00, 0.00000000e+00])
+    >>> ibpcalc.compute_probability_exp(0, 2, 12, 2, 150, data)
+    0.03213949936284399
     
     Note
     ----
     Rearranged/rewritten and optimized by 
     Ask Neve Gamby <aknvg@space.dtu.dk>.
 
     The resolution of the function `gosc` is higher than monthly.
@@ -682,7 +669,11 @@
         lambda0,
         params[2],
         params[3] + shifttime,
         params[4]
 
     )
 #===============================================================================
+
+if __name__ == "__main__": 
+    import doctest
+    doctest.testmod()
```

### Comparing `ibpmodel-1.1.2/src/ibpmodel/ibpforward.py` & `ibpmodel-1.2.0/src/ibpmodel/ibpforward.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 #!/usr/bin/env python3
 """This module contains the application functions for the calculation of the IBP index as well as the graphical visualization.
 """
 from .ibpcalc import *
 import numpy as np
 import pandas as pd
+import matplotlib as mpl
 import matplotlib.pyplot as plt
-from   matplotlib import cm
+import matplotlib.ticker as mticker
 
-def calculateIBPindex(day_month=0, longitude=list(range(-180,180,5)), local_time=np.arange(-6,6.1,0.1), f107=150):
+def calculateIBPindex(day_month=0, longitude=list(range(-180,180,5)), local_time=np.arange(-6,6.1,0.1), f107=150, coeff=None):
     '''Calculates the Ionospheric Bubble propability index based on the input parameters. 
     Returns a *pandas.DataFrame* with input parameters and IBP index. 
 
     Parameters
     ----------
     day_month : int or str or list, optional
         Day of year (*int*) or the month of the year (*str*). 
@@ -20,14 +21,17 @@
         The default is 0.
     longitude : int or list of ints, optional
         The geographical longitude(s), ``-180 <= longitude <= 180``. The default is `list(range(-180,181,5))`.
     local_time : int or float or list, optional
         The local time, ``-6.0 <= local_time <= 24``. The default is `np.arange(-6,6.1,0.1)`.
     f107 : int or float or list, optional
         The Solar Radio Flux (F10.7 index), ``0.0 <= f107 <= 200.0``. The default is 150.
+    coeff : None or str, optional
+        Name of the coefficient file.
+        The default is None.
 
     Returns
     -------
     df : pandas.DataFrame
         contains the columns: Doy (Day(s) of the year), Month (Month(s) from the day of the year), 
         Lon (Longitude(s)), LT (Local Time(s)), F10.7 (solar index(es)), IBP (Ionospheric Bubble Index, value(s) between 0.0 and 1.0).
     '''
@@ -46,15 +50,15 @@
 
     local_time_range = range(-6,25)
     local_time = checkParameter(local_time, local_time_range) 
 
     f107_range = range(0,201)
     f107 = checkParameter(f107, f107_range)
 
-    data = read_model_file()
+    data = read_model_file(coeff)
 
     parts = tiler(day_of_year, longitude, local_time, f107)
 
     for i, c in enumerate(['Doy', 'Lon', 'LT', 'F10.7']):
         df[c] = parts[i]
 
     df['Month'] = [ monthFromDoy(i) for i in df['Doy'] ]
@@ -67,15 +71,15 @@
         df['F10.7'].to_numpy(),
         data=data)
 
     df['IBP'] = df['IBP'].round(4)
 
     return df
 
-def butterflyData(f107=150):
+def butterflyData(f107=150, coeff=None):
     '''Calculates the Ionospheric Bubble Propability Index for all months (using the center DOY of each month) and all integer longitudes (resolution of 5 degree)
     using Local_Time of range -5 to 1 and a fixed value of F10.7. IBP index is then averaged from the Local_Times.
 
     Parameters
     ----------
     f107 : int, optional
         The Solar Radio Flux (F10.7 index). The default is 150.
@@ -89,111 +93,204 @@
     month_range       = np.arange(   1,  13,    1)
     longitude_range   = np.arange(-180, 179,  5.0)
     local_time_range  = np.arange(  -5,   1, 0.01)
 
     month, longitude, local_time = tiler(
         np.array(month_range,dtype='int'),longitude_range,local_time_range)
 
-    data = read_model_file()
+    data = read_model_file(coeff)
     
     day_of_year = np.array([ doyFromMonth(t) for t in month ])
     result = compute_probability_exp(
         day_of_year,month,longitude,local_time,f107,data)
 
     out_data = np.array(tile_aggregate(result,month_range,longitude_range,local_time_range)).transpose()
     
     return out_data
     
-def plotIBPindex(doy, f107=150, getFig=False):
-    '''Create a contour plot of IBP index for the given day. The resolution along the longitude is 5 degree. Local time spans from 6 pm to 6 am with a resolution of 0.1 hours. 
+def getcolorbar(cmap, level=np.arange(0.0, 1.0, 0.05)):
+    '''Applies level to colormap.
+    
+    Parameters
+    ----------
+    cmap : matplotlib.colors.Colormap
+
+    level : array-like
+    
+    Returns
+    -------
+    matplotlib.cm.ScalarMappable
+    '''
+    norm = mpl.colors.BoundaryNorm(level, cmap.N)
+    return mpl.cm.ScalarMappable(norm=norm, cmap=cmap)
+ 
+def setcolorbar(scalarmap, fig, ax, **kwargs):
+    '''Sets colorbar to figure on the specified axis.
+
+    Parameters
+    ----------
+    scalarmap : matplotlib.cm.ScalarMappable
+
+    fig : matplotlib.figure.Figure
+
+    ax : matplotlib.axes
+
+    Returns
+    -------
+    colorbar
+    '''
+    cbar = fig.colorbar(scalarmap, ax=ax, label='Ionospheric Bubble Probability', **kwargs)
+    return cbar
+
+def checkcmap(cmap):
+    '''Check if variable is a color map.
+
+    Parameters
+    ----------
+    cmap : str or matplotlib.colors.Colormap
+
+    Returns
+    -------
+    matplotlib.colors.Colormap
+
+    '''
+    try:
+        if isinstance(cmap, str):
+            cmap = mpl.colormaps[cmap]
+        if not isinstance(cmap, (mpl.colors.LinearSegmentedColormap, mpl.colors.ListedColormap)):
+            raise ValueError(f"'{cmap}' of type {type(cmap)} is not a valid for colormap")
+    except Exception as err:
+            print(err)
+            print("Default colormap 'viridis' is used!")
+            cmap = mpl.colormaps['viridis']
+ 
+    return cmap
+
+
+def plotIBPindex(doy, f107=150, ax=None, coeff=None, cmap='coolwarm', colors='b', linewidths=0.2, **kwargs):
+    '''Create a contour plot of IBP index for the given day. The resolution along the longitude is 5 degree. Local time spans from 6 pm to 6 am with a resolution of 0.1 hours. Default colormap is 'coolwarm'. 
 
     Parameters
     ----------
-    doy : int
-        Day of the year.
+    doy : int or str
+        Day of year (*int*) or the month of the year (*str*). 
+        *int*: Day of the year, ``0 <= doy <= 365``. The value 0 means it should be calculated based on every month.
+        *str*: Abbreviated month name. ['Jan', 'Feb', 'Mar', 'Apr', 'May', 'Jun', 'Jul', 'Aug', 'Sep', 'Oct', 'Nov', 'Dec']
     f107 : int, optional
         The Solar Radio Flux (F10.7 index). The default is 150.
-    getFig : bool, optional
-        True: return matplotlib.axes, False: show picture. The default is False.
+    ax : matplotlib.axes, optional
+        The Axes object in which the plot will be drawn. The default is None.
+    coeff : str, optional
+        Path of coefficient file. The default is None.
+    cmap : str or Colormap, optional
+        The colormap instance or registered colormap name to use. The default is 'coolwarm'.
+    colors : color string or sequence of colors, optional
+        The color of the contour lines. The default is 'blue'.
+    linewidths : float, optional
+        The line width of the contour lines. The default is 0.2.
 
     Returns
     -------
-    matplotlib.axes or bool
+    matplotlib.axes, matplotlib.cm.ScalarMappable
 
     '''
-    df = calculateIBPindex(day_month=doy, f107=f107)
+
+    if isinstance(doy, (int, str)):
+        doy = checkDoyMonth(doy)[0]
+    else:
+        raise ValueError(f"'{doy}' must be of type int or str, not  {type(doy)}")
+
+    df = calculateIBPindex(day_month=doy, f107=f107, coeff=coeff)
     
     value_size = np.unique(df['Lon'].to_numpy(), return_counts=True)
     value_size = ( len(value_size[0]), value_size[1][0] )
     
     x = np.transpose(df['Lon'].to_numpy().reshape(value_size))
     y = np.transpose(df['LT'].to_numpy().reshape(value_size))
     z = np.transpose(df['IBP'].to_numpy().reshape(value_size))
     
-    levels = np.arange(0.0, 1.0, 0.05)
+    if ax == None:
+        fig, ax = plt.subplots(figsize = (9, 4))
+        pltshow = True
+    else:
+        pltshow = False
     
-    fig, ax = plt.subplots(figsize = (6.4, 3.0))
-    CS = ax.contourf(x, y, z, levels, cmap=cm.coolwarm)
+    cmap = checkcmap(cmap)
+
+    levels = np.arange(0.0, 1.0, 0.05)
+    scalarmap = getcolorbar(cmap, levels)
     
-    CS2 = ax.contour(CS, levels, colors = 'b', linewidths = 0.2)
+    ax.contourf(x, y, z, levels=levels, cmap=cmap, **kwargs)
+    ax.contour(x, y, z, levels=levels, colors=colors, linewidths=linewidths, **kwargs)
+
+    ticks_loc = ax.get_yticks().tolist()
+    ax.yaxis.set_major_locator(mticker.FixedLocator(ticks_loc))
+    ax.set_yticklabels([f"{int(24+i)}:00" if i < 0 else f"0{int(i)}:00" for i in ticks_loc]) 
 
     ax.set_title('IBP index at doy ' + str(doy)+' with F10.7 = ' + str(f107))
     ax.set_xlabel('Longitude in degree')
-    ax.set_ylabel('Hours to Midnight')
+    ax.set_ylabel('Local Time')
 
-    cbar = fig.colorbar(CS)
-    cbar.ax.set_ylabel('Ionospheric Bubble Probability')
-    
-    if getFig:
-        return ax
-    elif getFig == False:
+    if pltshow:
+        setcolorbar(scalarmap, fig, ax)
+        
+        plt.subplots_adjust(right=1, bottom=0.15)
         plt.show()
-        return True
     else:
-        return False
-    
-def plotButterflyData(f107=150, getFig=False):
-    '''Create a contour plot of the result from function butterflyData(). 
+        return (ax, scalarmap)
+
+def plotButterflyData(f107=150, ax=None, coeff=None, cmap='plasma_r', colors='#999900', linewidths=0.2, **kwargs):
+    '''Create a contour plot of the result from function butterflyData(). Default colormap is 'plasma_r'. 
 
     Parameters
     ----------
     f107 : int, optional
         The Solar Radio Flux (F10.7 index). The default is 150.
-    getFig : bool, optional
-        True: return matplotlib.axes, False: show picture. The default is False.
+    ax : matplotlib.axes, optional
+        The Axes object in which the plot will be drawn. The default is None.
+    coeff : str, optional
+        Path of coefficient file. The default is None.
+    cmap : str or Colormap, optional
+        The colormap instance or registered colormap name to use. The default is 'plasma_r'.
+    colors : color string or sequence of colors, optional
+        The color of the contour lines. The default is '#999900'.
+    linewidths : float, optional
+        The line width of the contour lines. The default is 0.2.
 
     Returns
     -------
-    matplotlib.axes or bool
+    matplotlib.axes, matplotlib.cm.ScalarMappable
 
     '''
-    d = butterflyData(f107)
+    d = butterflyData(f107, coeff)
     
     y = np.transpose(np.reshape(d[:, 0], (12, 72)))
     x = np.transpose(np.reshape(d[:, 1], (12, 72)))
     z = np.transpose(np.reshape(d[:, 2], (12, 72)))
-    
+
     l = np.arange(0.0, 0.8, 0.05)
+
+    if ax == None:
+        fig, ax = plt.subplots(figsize = (6.2, 5.0))
+        pltshow = True
+    else:
+        pltshow = False
     
-    fig, ax = plt.subplots(figsize = (6.2, 5.0))
-        
-    C = ax.contourf(x, y, z, l, cmap = cm.plasma_r)
-    CS2 = ax.contour(C, levels=np.arange(0.05, 0.8, 0.05), colors = '#999900', linewidths = 0.2)
+    cmap = checkcmap(cmap)
+    
+    scalarmap = getcolorbar(cmap, l)
+           
+    ax.contourf(x, y, z, l, cmap = cmap, **kwargs)
+    ax.contour(x, y, z, levels=l, colors = colors, linewidths = linewidths, **kwargs)
     
     ax.set_title('Monthly IBP index with F10.7 = '+str(f107))
     ax.set_xlabel('Longitude in degree')
     ax.set_ylabel('Month')
     
-    cbar = fig.colorbar(C)
-    cbar.ax.set_ylabel('Ionospheric Bubble Probability')
-    
-    if getFig:
-        return ax
-    elif getFig == False:
+    if pltshow:
+        setcolorbar(scalarmap, fig, ax)        
         plt.show()
-        return True
     else:
-        return False
+        return ax, scalarmap
+
+
     
-if __name__ == "__main__":
-    print("Laeuft!")
-
```

### Comparing `ibpmodel-1.1.2/src/ibpmodel.egg-info/PKG-INFO` & `ibpmodel-1.2.0/src/ibpmodel.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibpmodel
-Version: 1.1.2
+Version: 1.2.0
 Summary: Ionospheric Bubble Probability
 Author: Martin Rother
 Maintainer-email: Ina Wehner <wehner@iap-kborn.de>
 License: MIT License
 Project-URL: homepage, https://igit.iap-kborn.de/ibp/ibp-model.git
 Project-URL: documentation, https://ibp-model.readthedocs.io
 Project-URL: repository, https://igit.iap-kborn.de/ibp/ibp-model.git
@@ -69,15 +69,15 @@
 ^^^^^
 The return value of the function *ibpmodel.calculateIBPindex()* is of type pandas.DataFrame.
 
 
 .. code-block:: python
 
     >>> from ibpmodel import *
-    >>> calculateIBPindex(day_month=15,    # Day of Year or Month 
+    >>> calculateIBPindex(day_month=15,               # Day of Year or Month 
                   longitude=0,                        # Longitude in degree
                   local_time=20.9,                    # Local time in hours 
                   f107=150)                           # F10.7 cm Solar Flux index
        Doy  Month  Lon    LT  F10.7     IBP
     0   15      1    0  20.9    150  0.3547
 
 .. code-block:: python
@@ -126,8 +126,40 @@
 
 *Stolle et al.*, `An empirical climatological model of the occurrence of F region equatorial plasma irregularities <https://igit.iap-kborn.de/ibp/ibp-model/-/raw/main/docs/source/_static/8thSwarmDataQualityWorkshop_slides.pdf>`_, 8th Swarm data quality workshop at ESA/ESRIN, October 2017. 
 
 *Lucas Schreiter*, Anwendungsorientierte Modellierung der Auftretenswahrscheinlichkeit und relativen Häufigkeit von äquatorialen Plasmabubbles,  Master's thesis, Institute of Mathematics, University of Potsdam, 2016. (in German only.)
 
 .. inclusion-marker-acknow
 
+Information for developers
+--------------------------
 
+Setup environment
+^^^^^^^^^^^^^^^^^
+
+.. code-block:: console
+
+    $ git clone https://igit.iap-kborn.de/ibp/ibp-model.git
+    $ cd ibp-model
+    $ pip install -r requirements.txt
+    $ pip install -e .
+
+Test of package using doctest
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+.. code-block:: console
+
+    $ python src/ibpmodel/ibpcalc.py
+
+No error should occur.
+
+
+Test run of the documentation
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+.. code-block:: console
+
+    $ cd docs
+    $ make clean && make html
+
+The *docs/build/html/* directory contains the html files. Open *index.html* in browser. 
+The results of the code examples on the usage page are generated automatically. Therefore the ibpmodel package must be installed (*pip install -e .*).
```

### Comparing `ibpmodel-1.1.2/src/ibpmodel.egg-info/SOURCES.txt` & `ibpmodel-1.2.0/src/ibpmodel.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -3,29 +3,30 @@
 CHANGELOG.rst
 LICENSE
 README.rst
 pyproject.toml
 requirements.txt
 docs/Makefile
 docs/make.bat
+docs/source/changelog.rst
 docs/source/conf.py
 docs/source/ibpmodel.rst
 docs/source/index.rst
 docs/source/installation.rst
 docs/source/modules.rst
 docs/source/reference.rst
 docs/source/requirements.txt
 docs/source/usage.rst
 docs/source/_static/8thSwarmDataQualityWorkshop_slides.pdf
 docs/source/_static/example_plotButterfly.png
 docs/source/_static/example_plotIBP.png
+docs/source/_static/example_subplot.png
 src/ibpmodel/SW_OPER_IBP_CLI_2__00000000T000000_99999999T999999_0002.cdf
 src/ibpmodel/__init__.py
 src/ibpmodel/ibpcalc.py
 src/ibpmodel/ibpforward.py
 src/ibpmodel.egg-info/PKG-INFO
 src/ibpmodel.egg-info/SOURCES.txt
 src/ibpmodel.egg-info/dependency_links.txt
 src/ibpmodel.egg-info/requires.txt
 src/ibpmodel.egg-info/top_level.txt
-tests/conftest.py
-tests/test_ibp.py
+template/IBP_CLI_2_bubble-probability.ipynb
```

