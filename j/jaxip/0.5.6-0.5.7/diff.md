# Comparing `tmp/jaxip-0.5.6.tar.gz` & `tmp/jaxip-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaxip-0.5.6.tar", last modified: Sat May  6 13:11:24 2023, max compression
+gzip compressed data, was "jaxip-0.5.7.tar", last modified: Mon May  8 16:52:51 2023, max compression
```

## Comparing `jaxip-0.5.6.tar` & `jaxip-0.5.7.tar`

### file list

```diff
@@ -1,139 +1,140 @@
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-06 13:11:24.739946 jaxip-0.5.6/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      166 2022-12-07 19:09:20.000000 jaxip-0.5.6/AUTHORS.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     3491 2023-04-26 21:18:43.000000 jaxip-0.5.6/CONTRIBUTING.rst
--rw-r--r--   0 hossein   (1000) hossein   (1000)      569 2023-03-02 17:04:49.000000 jaxip-0.5.6/HISTORY.rst
--rw-r--r--   0 hossein   (1000) hossein   (1000)     1523 2023-01-05 20:40:22.000000 jaxip-0.5.6/LICENSE
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      262 2022-12-07 20:18:56.000000 jaxip-0.5.6/MANIFEST.in
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     5283 2023-05-06 13:11:24.739946 jaxip-0.5.6/PKG-INFO
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     4696 2023-05-05 21:35:14.000000 jaxip-0.5.6/README.rst
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-06 13:11:24.723946 jaxip-0.5.6/docs/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      606 2023-02-01 19:45:48.000000 jaxip-0.5.6/docs/Makefile
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-06 13:11:24.715947 jaxip-0.5.6/docs/_build/
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-06 13:11:24.715947 jaxip-0.5.6/docs/_build/doctrees/
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-06 13:11:24.723946 jaxip-0.5.6/docs/_build/doctrees/nbsphinx/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    15512 2023-05-06 13:07:08.000000 jaxip-0.5.6/docs/_build/doctrees/nbsphinx/notebooks_potential_training_29_21.png
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    11011 2023-05-06 13:07:09.000000 jaxip-0.5.6/docs/_build/doctrees/nbsphinx/notebooks_tutorials_38_0.png
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    12610 2023-05-06 13:07:09.000000 jaxip-0.5.6/docs/_build/doctrees/nbsphinx/notebooks_tutorials_45_0.png
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    12610 2023-05-06 13:07:09.000000 jaxip-0.5.6/docs/_build/doctrees/nbsphinx/notebooks_tutorials_51_0.png
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-06 13:11:24.719947 jaxip-0.5.6/docs/_build/html/
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-06 13:11:24.723946 jaxip-0.5.6/docs/_build/html/_images/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    15512 2023-05-06 13:07:08.000000 jaxip-0.5.6/docs/_build/html/_images/notebooks_potential_training_29_21.png
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    11011 2023-05-06 13:07:09.000000 jaxip-0.5.6/docs/_build/html/_images/notebooks_tutorials_38_0.png
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    12610 2023-05-06 13:07:09.000000 jaxip-0.5.6/docs/_build/html/_images/notebooks_tutorials_45_0.png
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    12610 2023-05-06 13:07:09.000000 jaxip-0.5.6/docs/_build/html/_images/notebooks_tutorials_51_0.png
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-06 13:11:24.723946 jaxip-0.5.6/docs/_build/html/_static/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      286 2023-04-26 21:14:06.000000 jaxip-0.5.6/docs/_build/html/_static/file.png
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       90 2023-04-26 21:14:06.000000 jaxip-0.5.6/docs/_build/html/_static/minus.png
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       90 2023-04-26 21:14:06.000000 jaxip-0.5.6/docs/_build/html/_static/plus.png
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       28 2022-12-28 08:07:09.000000 jaxip-0.5.6/docs/authors.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     6406 2023-05-01 12:49:56.000000 jaxip-0.5.6/docs/conf.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       33 2022-12-07 19:09:20.000000 jaxip-0.5.6/docs/contributing.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       81 2023-05-01 12:51:50.000000 jaxip-0.5.6/docs/examples.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       28 2022-12-07 19:09:20.000000 jaxip-0.5.6/docs/history.rst
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-06 13:11:24.723946 jaxip-0.5.6/docs/images/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    44314 2023-03-28 20:24:39.000000 jaxip-0.5.6/docs/images/flowchart.drawio.png
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    96759 2023-02-06 19:53:40.000000 jaxip-0.5.6/docs/images/water.png
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      315 2023-05-04 21:58:24.000000 jaxip-0.5.6/docs/index.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1864 2023-04-26 21:18:43.000000 jaxip-0.5.6/docs/installation.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      760 2023-05-01 12:13:59.000000 jaxip-0.5.6/docs/jaxip.atoms.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      653 2023-05-01 12:13:59.000000 jaxip-0.5.6/docs/jaxip.datasets.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1095 2023-05-01 12:13:59.000000 jaxip-0.5.6/docs/jaxip.descriptors.acsf.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      595 2023-05-01 12:13:59.000000 jaxip-0.5.6/docs/jaxip.descriptors.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      635 2023-05-01 12:13:59.000000 jaxip-0.5.6/docs/jaxip.models.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1129 2023-05-01 12:41:07.000000 jaxip-0.5.6/docs/jaxip.potentials.nnp.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      616 2023-05-01 12:41:07.000000 jaxip-0.5.6/docs/jaxip.potentials.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      935 2023-05-06 13:07:01.000000 jaxip-0.5.6/docs/jaxip.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      915 2023-05-01 12:14:00.000000 jaxip-0.5.6/docs/jaxip.utils.rst
--rw-r--r--   0 hossein   (1000) hossein   (1000)      803 2023-01-05 20:40:22.000000 jaxip-0.5.6/docs/make.bat
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       52 2023-05-06 13:07:01.000000 jaxip-0.5.6/docs/modules.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       27 2022-12-20 21:49:36.000000 jaxip-0.5.6/docs/readme.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     3833 2023-05-05 21:13:22.000000 jaxip-0.5.6/docs/theory.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1158 2023-04-26 21:18:43.000000 jaxip-0.5.6/docs/usage.rst
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-06 13:11:24.727946 jaxip-0.5.6/jaxip/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      575 2023-05-04 21:42:07.000000 jaxip-0.5.6/jaxip/__init__.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      294 2023-05-06 13:06:00.000000 jaxip-0.5.6/jaxip/_version.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-06 13:11:24.727946 jaxip-0.5.6/jaxip/atoms/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      174 2023-05-01 12:41:07.000000 jaxip-0.5.6/jaxip/atoms/__init__.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      355 2023-05-01 12:41:07.000000 jaxip-0.5.6/jaxip/atoms/_box.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      779 2023-05-01 12:41:07.000000 jaxip-0.5.6/jaxip/atoms/_neighbor.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1342 2023-05-01 12:41:07.000000 jaxip-0.5.6/jaxip/atoms/_structure.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     3593 2023-05-01 12:41:07.000000 jaxip-0.5.6/jaxip/atoms/box.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     5034 2023-05-01 06:50:37.000000 jaxip-0.5.6/jaxip/atoms/element.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     2865 2023-05-01 12:41:07.000000 jaxip-0.5.6/jaxip/atoms/neighbor.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    16306 2023-05-06 13:01:56.000000 jaxip-0.5.6/jaxip/atoms/structure.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     2589 2023-02-08 21:09:37.000000 jaxip-0.5.6/jaxip/base.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1131 2023-05-01 12:41:07.000000 jaxip-0.5.6/jaxip/config.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-06 13:11:24.727946 jaxip-0.5.6/jaxip/datasets/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      154 2023-05-01 12:41:07.000000 jaxip-0.5.6/jaxip/datasets/__init__.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      444 2023-05-04 19:02:08.000000 jaxip-0.5.6/jaxip/datasets/base.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     6391 2023-05-04 21:19:36.000000 jaxip-0.5.6/jaxip/datasets/runner.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1021 2023-05-01 12:41:07.000000 jaxip-0.5.6/jaxip/datasets/transformer.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-06 13:11:24.731946 jaxip-0.5.6/jaxip/descriptors/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      130 2023-05-01 12:41:07.000000 jaxip-0.5.6/jaxip/descriptors/__init__.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-06 13:11:24.731946 jaxip-0.5.6/jaxip/descriptors/acsf/
--rw-r--r--   0 hossein   (1000) hossein   (1000)      400 2023-01-05 20:40:22.000000 jaxip-0.5.6/jaxip/descriptors/acsf/__init__.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     5275 2023-05-06 12:28:36.000000 jaxip-0.5.6/jaxip/descriptors/acsf/_acsf.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     7581 2023-05-01 12:41:07.000000 jaxip-0.5.6/jaxip/descriptors/acsf/acsf.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     2226 2023-03-23 20:22:06.000000 jaxip-0.5.6/jaxip/descriptors/acsf/angular.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     2474 2023-03-23 20:22:06.000000 jaxip-0.5.6/jaxip/descriptors/acsf/cutoff.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1352 2023-03-23 20:22:06.000000 jaxip-0.5.6/jaxip/descriptors/acsf/radial.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1011 2023-05-01 12:41:07.000000 jaxip-0.5.6/jaxip/descriptors/acsf/symmetry.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      765 2023-05-01 09:07:44.000000 jaxip-0.5.6/jaxip/descriptors/base.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     7476 2023-05-01 12:41:07.000000 jaxip-0.5.6/jaxip/descriptors/scaler.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     3739 2023-05-01 12:41:07.000000 jaxip-0.5.6/jaxip/logger.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-06 13:11:24.731946 jaxip-0.5.6/jaxip/models/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      170 2023-05-01 12:41:07.000000 jaxip-0.5.6/jaxip/models/__init__.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1125 2023-05-01 12:41:07.000000 jaxip-0.5.6/jaxip/models/activation.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      604 2023-03-14 20:01:39.000000 jaxip-0.5.6/jaxip/models/initializer.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     2846 2023-05-01 12:41:07.000000 jaxip-0.5.6/jaxip/models/nn.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-06 13:11:24.731946 jaxip-0.5.6/jaxip/potentials/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      196 2023-05-01 12:41:07.000000 jaxip-0.5.6/jaxip/potentials/__init__.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1949 2023-05-01 12:41:07.000000 jaxip-0.5.6/jaxip/potentials/_energy.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      866 2023-05-01 12:41:07.000000 jaxip-0.5.6/jaxip/potentials/_force.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1799 2023-05-01 12:41:07.000000 jaxip-0.5.6/jaxip/potentials/atomic_potential.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      644 2023-05-01 12:41:07.000000 jaxip-0.5.6/jaxip/potentials/base.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-06 13:11:24.735946 jaxip-0.5.6/jaxip/potentials/nnp/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      196 2023-05-01 12:41:07.000000 jaxip-0.5.6/jaxip/potentials/nnp/__init__.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     9053 2023-05-01 12:41:07.000000 jaxip-0.5.6/jaxip/potentials/nnp/gradient_descent.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     9264 2023-05-02 06:46:19.000000 jaxip-0.5.6/jaxip/potentials/nnp/kalman_filter.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     2576 2023-05-01 12:41:07.000000 jaxip-0.5.6/jaxip/potentials/nnp/metrics.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    18936 2023-05-05 07:59:16.000000 jaxip-0.5.6/jaxip/potentials/nnp/potential.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    11326 2023-05-01 12:41:07.000000 jaxip-0.5.6/jaxip/potentials/nnp/settings.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      643 2023-01-25 20:59:12.000000 jaxip-0.5.6/jaxip/types.py
--rw-r--r--   0 hossein   (1000) hossein   (1000)      200 2023-01-05 20:40:22.000000 jaxip-0.5.6/jaxip/units.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-06 13:11:24.735946 jaxip-0.5.6/jaxip/utils/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       73 2023-05-01 12:41:07.000000 jaxip-0.5.6/jaxip/utils/__init__.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1427 2023-02-18 20:52:11.000000 jaxip-0.5.6/jaxip/utils/attribute.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      585 2023-05-01 12:41:07.000000 jaxip-0.5.6/jaxip/utils/batch.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     2008 2023-03-23 20:22:06.000000 jaxip-0.5.6/jaxip/utils/compare.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     4410 2023-05-01 12:41:07.000000 jaxip-0.5.6/jaxip/utils/profiler.py
--rw-r--r--   0 hossein   (1000) hossein   (1000)      670 2023-01-18 21:30:52.000000 jaxip-0.5.6/jaxip/utils/tokenize.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-06 13:11:24.727946 jaxip-0.5.6/jaxip.egg-info/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     5283 2023-05-06 13:11:24.000000 jaxip-0.5.6/jaxip.egg-info/PKG-INFO
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     3121 2023-05-06 13:11:24.000000 jaxip-0.5.6/jaxip.egg-info/SOURCES.txt
--rw-rw-r--   0 hossein   (1000) hossein   (1000)        1 2023-05-06 13:11:24.000000 jaxip-0.5.6/jaxip.egg-info/dependency_links.txt
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       41 2023-05-06 13:11:24.000000 jaxip-0.5.6/jaxip.egg-info/entry_points.txt
--rw-rw-r--   0 hossein   (1000) hossein   (1000)        1 2023-05-06 13:11:24.000000 jaxip-0.5.6/jaxip.egg-info/not-zip-safe
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       85 2023-05-06 13:11:24.000000 jaxip-0.5.6/jaxip.egg-info/requires.txt
--rw-rw-r--   0 hossein   (1000) hossein   (1000)        6 2023-05-06 13:11:24.000000 jaxip-0.5.6/jaxip.egg-info/top_level.txt
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      137 2023-05-06 13:11:24.739946 jaxip-0.5.6/setup.cfg
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1661 2023-03-22 21:56:02.000000 jaxip-0.5.6/setup.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-06 13:11:24.739946 jaxip-0.5.6/tests/
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-06 13:11:24.739946 jaxip-0.5.6/tests/.ipynb_checkpoints/
--rw-r--r--   0 hossein   (1000) hossein   (1000)     3632 2022-12-27 18:25:19.000000 jaxip-0.5.6/tests/.ipynb_checkpoints/h2o-checkpoint.data
--rw-r--r--   0 hossein   (1000) hossein   (1000)     9543 2023-01-26 17:53:14.000000 jaxip-0.5.6/tests/.ipynb_checkpoints/h2o-checkpoint.json
--rw-r--r--   0 hossein   (1000) hossein   (1000)     3632 2022-12-26 17:32:00.000000 jaxip-0.5.6/tests/.ipynb_checkpoints/input.h2o-checkpoint.data
--rw-r--r--   0 hossein   (1000) hossein   (1000)    23707 2023-03-19 08:54:39.000000 jaxip-0.5.6/tests/.ipynb_checkpoints/test-checkpoint.ipynb
--rw-r--r--   0 hossein   (1000) hossein   (1000)       35 2023-01-05 20:40:22.000000 jaxip-0.5.6/tests/__init__.py
--rw-r--r--   0 hossein   (1000) hossein   (1000)     3632 2022-12-27 18:25:19.000000 jaxip-0.5.6/tests/h2o.data
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     2063 2023-03-14 20:01:39.000000 jaxip-0.5.6/tests/h2o.json
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      384 2023-05-06 13:06:50.000000 jaxip-0.5.6/tests/scaling.001.data
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      480 2023-05-06 13:06:50.000000 jaxip-0.5.6/tests/scaling.008.data
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     5117 2023-03-14 20:00:37.000000 jaxip-0.5.6/tests/test_acsf.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     4105 2023-02-06 19:57:38.000000 jaxip-0.5.6/tests/test_nn.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     3420 2023-05-01 12:41:07.000000 jaxip-0.5.6/tests/test_nnp.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     4816 2023-05-01 12:41:07.000000 jaxip-0.5.6/tests/test_runner.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     2859 2023-05-01 12:41:07.000000 jaxip-0.5.6/tests/test_scaler.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     4937 2023-04-24 20:54:27.000000 jaxip-0.5.6/tests/test_structure.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      793 2023-05-06 13:06:50.000000 jaxip-0.5.6/tests/weights.001.pkl
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      813 2023-05-06 13:06:50.000000 jaxip-0.5.6/tests/weights.008.pkl
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-08 16:52:51.187937 jaxip-0.5.7/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      166 2022-12-07 19:09:20.000000 jaxip-0.5.7/AUTHORS.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     3491 2023-04-26 21:18:43.000000 jaxip-0.5.7/CONTRIBUTING.rst
+-rw-r--r--   0 hossein   (1000) hossein   (1000)      569 2023-03-02 17:04:49.000000 jaxip-0.5.7/HISTORY.rst
+-rw-r--r--   0 hossein   (1000) hossein   (1000)     1523 2023-01-05 20:40:22.000000 jaxip-0.5.7/LICENSE
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      262 2022-12-07 20:18:56.000000 jaxip-0.5.7/MANIFEST.in
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     5342 2023-05-08 16:52:51.187937 jaxip-0.5.7/PKG-INFO
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     4755 2023-05-08 16:51:03.000000 jaxip-0.5.7/README.rst
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-08 16:52:51.163937 jaxip-0.5.7/docs/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      606 2023-02-01 19:45:48.000000 jaxip-0.5.7/docs/Makefile
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-08 16:52:51.155937 jaxip-0.5.7/docs/_build/
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-08 16:52:51.155937 jaxip-0.5.7/docs/_build/doctrees/
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-08 16:52:51.163937 jaxip-0.5.7/docs/_build/doctrees/nbsphinx/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    15512 2023-05-08 16:43:13.000000 jaxip-0.5.7/docs/_build/doctrees/nbsphinx/notebooks_potential_training_29_21.png
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    11011 2023-05-08 16:43:14.000000 jaxip-0.5.7/docs/_build/doctrees/nbsphinx/notebooks_tutorials_38_0.png
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    12610 2023-05-08 16:43:14.000000 jaxip-0.5.7/docs/_build/doctrees/nbsphinx/notebooks_tutorials_45_0.png
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    12610 2023-05-08 16:43:14.000000 jaxip-0.5.7/docs/_build/doctrees/nbsphinx/notebooks_tutorials_51_0.png
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-08 16:52:51.155937 jaxip-0.5.7/docs/_build/html/
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-08 16:52:51.167937 jaxip-0.5.7/docs/_build/html/_images/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    15512 2023-05-08 16:43:13.000000 jaxip-0.5.7/docs/_build/html/_images/notebooks_potential_training_29_21.png
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    11011 2023-05-08 16:43:14.000000 jaxip-0.5.7/docs/_build/html/_images/notebooks_tutorials_38_0.png
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    12610 2023-05-08 16:43:14.000000 jaxip-0.5.7/docs/_build/html/_images/notebooks_tutorials_45_0.png
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    12610 2023-05-08 16:43:14.000000 jaxip-0.5.7/docs/_build/html/_images/notebooks_tutorials_51_0.png
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-08 16:52:51.167937 jaxip-0.5.7/docs/_build/html/_static/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      286 2023-04-26 21:14:06.000000 jaxip-0.5.7/docs/_build/html/_static/file.png
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       90 2023-04-26 21:14:06.000000 jaxip-0.5.7/docs/_build/html/_static/minus.png
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       90 2023-04-26 21:14:06.000000 jaxip-0.5.7/docs/_build/html/_static/plus.png
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       28 2022-12-28 08:07:09.000000 jaxip-0.5.7/docs/authors.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     6406 2023-05-01 12:49:56.000000 jaxip-0.5.7/docs/conf.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       33 2022-12-07 19:09:20.000000 jaxip-0.5.7/docs/contributing.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       81 2023-05-01 12:51:50.000000 jaxip-0.5.7/docs/examples.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       28 2022-12-07 19:09:20.000000 jaxip-0.5.7/docs/history.rst
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-08 16:52:51.167937 jaxip-0.5.7/docs/images/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    44314 2023-03-28 20:24:39.000000 jaxip-0.5.7/docs/images/flowchart.drawio.png
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    96759 2023-02-06 19:53:40.000000 jaxip-0.5.7/docs/images/water.png
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      315 2023-05-06 13:11:44.000000 jaxip-0.5.7/docs/index.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1864 2023-04-26 21:18:43.000000 jaxip-0.5.7/docs/installation.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      760 2023-05-08 16:43:07.000000 jaxip-0.5.7/docs/jaxip.atoms.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      507 2023-05-08 16:51:03.000000 jaxip-0.5.7/docs/jaxip.datasets.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1095 2023-05-08 16:43:07.000000 jaxip-0.5.7/docs/jaxip.descriptors.acsf.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      595 2023-05-08 16:43:07.000000 jaxip-0.5.7/docs/jaxip.descriptors.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      686 2023-05-08 16:51:03.000000 jaxip-0.5.7/docs/jaxip.models.nn.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      234 2023-05-08 16:51:03.000000 jaxip-0.5.7/docs/jaxip.models.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1129 2023-05-08 16:43:07.000000 jaxip-0.5.7/docs/jaxip.potentials.nnp.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      464 2023-05-08 16:51:03.000000 jaxip-0.5.7/docs/jaxip.potentials.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      935 2023-05-08 16:43:07.000000 jaxip-0.5.7/docs/jaxip.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      915 2023-05-08 16:43:07.000000 jaxip-0.5.7/docs/jaxip.utils.rst
+-rw-r--r--   0 hossein   (1000) hossein   (1000)      803 2023-01-05 20:40:22.000000 jaxip-0.5.7/docs/make.bat
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       52 2023-05-08 16:43:07.000000 jaxip-0.5.7/docs/modules.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       27 2022-12-20 21:49:36.000000 jaxip-0.5.7/docs/readme.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     3833 2023-05-06 13:11:44.000000 jaxip-0.5.7/docs/theory.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1158 2023-04-26 21:18:43.000000 jaxip-0.5.7/docs/usage.rst
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-08 16:52:51.171937 jaxip-0.5.7/jaxip/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      575 2023-05-06 13:11:44.000000 jaxip-0.5.7/jaxip/__init__.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      294 2023-05-08 16:51:03.000000 jaxip-0.5.7/jaxip/_version.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-08 16:52:51.175937 jaxip-0.5.7/jaxip/atoms/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      174 2023-05-01 12:41:07.000000 jaxip-0.5.7/jaxip/atoms/__init__.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      355 2023-05-01 12:41:07.000000 jaxip-0.5.7/jaxip/atoms/_box.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      779 2023-05-01 12:41:07.000000 jaxip-0.5.7/jaxip/atoms/_neighbor.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1342 2023-05-01 12:41:07.000000 jaxip-0.5.7/jaxip/atoms/_structure.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     3593 2023-05-01 12:41:07.000000 jaxip-0.5.7/jaxip/atoms/box.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     5034 2023-05-01 06:50:37.000000 jaxip-0.5.7/jaxip/atoms/element.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     2865 2023-05-01 12:41:07.000000 jaxip-0.5.7/jaxip/atoms/neighbor.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    16306 2023-05-06 13:11:44.000000 jaxip-0.5.7/jaxip/atoms/structure.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     2589 2023-02-08 21:09:37.000000 jaxip-0.5.7/jaxip/base.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1131 2023-05-01 12:41:07.000000 jaxip-0.5.7/jaxip/config.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-08 16:52:51.175937 jaxip-0.5.7/jaxip/datasets/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      154 2023-05-01 12:41:07.000000 jaxip-0.5.7/jaxip/datasets/__init__.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     6668 2023-05-08 16:51:03.000000 jaxip-0.5.7/jaxip/datasets/runner.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1021 2023-05-01 12:41:07.000000 jaxip-0.5.7/jaxip/datasets/transformer.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-08 16:52:51.175937 jaxip-0.5.7/jaxip/descriptors/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      130 2023-05-01 12:41:07.000000 jaxip-0.5.7/jaxip/descriptors/__init__.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-08 16:52:51.175937 jaxip-0.5.7/jaxip/descriptors/acsf/
+-rw-r--r--   0 hossein   (1000) hossein   (1000)      400 2023-01-05 20:40:22.000000 jaxip-0.5.7/jaxip/descriptors/acsf/__init__.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     5275 2023-05-06 13:11:44.000000 jaxip-0.5.7/jaxip/descriptors/acsf/_acsf.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     7581 2023-05-01 12:41:07.000000 jaxip-0.5.7/jaxip/descriptors/acsf/acsf.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     2226 2023-03-23 20:22:06.000000 jaxip-0.5.7/jaxip/descriptors/acsf/angular.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     2874 2023-05-08 16:51:03.000000 jaxip-0.5.7/jaxip/descriptors/acsf/cutoff.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1352 2023-03-23 20:22:06.000000 jaxip-0.5.7/jaxip/descriptors/acsf/radial.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1011 2023-05-01 12:41:07.000000 jaxip-0.5.7/jaxip/descriptors/acsf/symmetry.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      765 2023-05-01 09:07:44.000000 jaxip-0.5.7/jaxip/descriptors/base.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     7476 2023-05-01 12:41:07.000000 jaxip-0.5.7/jaxip/descriptors/scaler.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     3739 2023-05-01 12:41:07.000000 jaxip-0.5.7/jaxip/logger.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-08 16:52:51.175937 jaxip-0.5.7/jaxip/models/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       88 2023-05-08 16:51:03.000000 jaxip-0.5.7/jaxip/models/__init__.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-08 16:52:51.179937 jaxip-0.5.7/jaxip/models/nn/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      181 2023-05-08 16:51:03.000000 jaxip-0.5.7/jaxip/models/nn/__init__.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1125 2023-05-08 16:51:03.000000 jaxip-0.5.7/jaxip/models/nn/activation.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      604 2023-05-08 16:51:03.000000 jaxip-0.5.7/jaxip/models/nn/initializer.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     2849 2023-05-08 16:51:03.000000 jaxip-0.5.7/jaxip/models/nn/network.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-08 16:52:51.179937 jaxip-0.5.7/jaxip/potentials/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      196 2023-05-01 12:41:07.000000 jaxip-0.5.7/jaxip/potentials/__init__.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1949 2023-05-01 12:41:07.000000 jaxip-0.5.7/jaxip/potentials/_energy.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      866 2023-05-01 12:41:07.000000 jaxip-0.5.7/jaxip/potentials/_force.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1807 2023-05-08 16:51:03.000000 jaxip-0.5.7/jaxip/potentials/atomic_potential.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-08 16:52:51.179937 jaxip-0.5.7/jaxip/potentials/nnp/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      196 2023-05-01 12:41:07.000000 jaxip-0.5.7/jaxip/potentials/nnp/__init__.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     9589 2023-05-08 16:51:03.000000 jaxip-0.5.7/jaxip/potentials/nnp/gradient_descent.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     9747 2023-05-08 16:51:03.000000 jaxip-0.5.7/jaxip/potentials/nnp/kalman_filter.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     2576 2023-05-01 12:41:07.000000 jaxip-0.5.7/jaxip/potentials/nnp/metrics.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    19255 2023-05-08 16:51:03.000000 jaxip-0.5.7/jaxip/potentials/nnp/potential.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    11326 2023-05-01 12:41:07.000000 jaxip-0.5.7/jaxip/potentials/nnp/settings.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      643 2023-05-07 09:13:07.000000 jaxip-0.5.7/jaxip/types.py
+-rw-r--r--   0 hossein   (1000) hossein   (1000)      200 2023-01-05 20:40:22.000000 jaxip-0.5.7/jaxip/units.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-08 16:52:51.183937 jaxip-0.5.7/jaxip/utils/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       73 2023-05-01 12:41:07.000000 jaxip-0.5.7/jaxip/utils/__init__.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1427 2023-02-18 20:52:11.000000 jaxip-0.5.7/jaxip/utils/attribute.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      585 2023-05-01 12:41:07.000000 jaxip-0.5.7/jaxip/utils/batch.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     2008 2023-03-23 20:22:06.000000 jaxip-0.5.7/jaxip/utils/compare.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     4410 2023-05-01 12:41:07.000000 jaxip-0.5.7/jaxip/utils/profiler.py
+-rw-r--r--   0 hossein   (1000) hossein   (1000)      670 2023-01-18 21:30:52.000000 jaxip-0.5.7/jaxip/utils/tokenize.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-08 16:52:51.171937 jaxip-0.5.7/jaxip.egg-info/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     5342 2023-05-08 16:52:51.000000 jaxip-0.5.7/jaxip.egg-info/PKG-INFO
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     3140 2023-05-08 16:52:51.000000 jaxip-0.5.7/jaxip.egg-info/SOURCES.txt
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)        1 2023-05-08 16:52:51.000000 jaxip-0.5.7/jaxip.egg-info/dependency_links.txt
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       41 2023-05-08 16:52:51.000000 jaxip-0.5.7/jaxip.egg-info/entry_points.txt
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)        1 2023-05-08 16:52:51.000000 jaxip-0.5.7/jaxip.egg-info/not-zip-safe
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       85 2023-05-08 16:52:51.000000 jaxip-0.5.7/jaxip.egg-info/requires.txt
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)        6 2023-05-08 16:52:51.000000 jaxip-0.5.7/jaxip.egg-info/top_level.txt
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      137 2023-05-08 16:52:51.187937 jaxip-0.5.7/setup.cfg
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1661 2023-03-22 21:56:02.000000 jaxip-0.5.7/setup.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-08 16:52:51.183937 jaxip-0.5.7/tests/
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-08 16:52:51.183937 jaxip-0.5.7/tests/.ipynb_checkpoints/
+-rw-r--r--   0 hossein   (1000) hossein   (1000)     3632 2022-12-27 18:25:19.000000 jaxip-0.5.7/tests/.ipynb_checkpoints/h2o-checkpoint.data
+-rw-r--r--   0 hossein   (1000) hossein   (1000)     9543 2023-01-26 17:53:14.000000 jaxip-0.5.7/tests/.ipynb_checkpoints/h2o-checkpoint.json
+-rw-r--r--   0 hossein   (1000) hossein   (1000)     3632 2022-12-26 17:32:00.000000 jaxip-0.5.7/tests/.ipynb_checkpoints/input.h2o-checkpoint.data
+-rw-r--r--   0 hossein   (1000) hossein   (1000)    23707 2023-03-19 08:54:39.000000 jaxip-0.5.7/tests/.ipynb_checkpoints/test-checkpoint.ipynb
+-rw-r--r--   0 hossein   (1000) hossein   (1000)       35 2023-01-05 20:40:22.000000 jaxip-0.5.7/tests/__init__.py
+-rw-r--r--   0 hossein   (1000) hossein   (1000)     3632 2022-12-27 18:25:19.000000 jaxip-0.5.7/tests/h2o.data
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     2063 2023-03-14 20:01:39.000000 jaxip-0.5.7/tests/h2o.json
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      384 2023-05-08 16:42:40.000000 jaxip-0.5.7/tests/scaling.001.data
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      480 2023-05-08 16:42:40.000000 jaxip-0.5.7/tests/scaling.008.data
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     5117 2023-05-07 11:23:30.000000 jaxip-0.5.7/tests/test_acsf.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     4116 2023-05-08 16:51:03.000000 jaxip-0.5.7/tests/test_nn.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     3420 2023-05-01 12:41:07.000000 jaxip-0.5.7/tests/test_nnp.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     4816 2023-05-01 12:41:07.000000 jaxip-0.5.7/tests/test_runner.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     2859 2023-05-01 12:41:07.000000 jaxip-0.5.7/tests/test_scaler.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     4937 2023-04-24 20:54:27.000000 jaxip-0.5.7/tests/test_structure.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      793 2023-05-08 16:42:40.000000 jaxip-0.5.7/tests/weights.001.pkl
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      813 2023-05-08 16:42:40.000000 jaxip-0.5.7/tests/weights.008.pkl
```

### Comparing `jaxip-0.5.6/CONTRIBUTING.rst` & `jaxip-0.5.7/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.6/HISTORY.rst` & `jaxip-0.5.7/HISTORY.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.6/LICENSE` & `jaxip-0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.6/PKG-INFO` & `jaxip-0.5.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaxip
-Version: 0.5.6
+Version: 0.5.7
 Summary: JAX-based Interatomic Potential
 Home-page: https://github.com/hghcomphys/jaxip
 Author: Hossein Ghorbanfekr
 Author-email: hgh.comphys@gmail.com
 License: GNU General Public License v3
 Keywords: jaxip
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -154,8 +154,8 @@
         nnp.compute_force(structure)
 
 
 License
 -------
 
 This project is licensed under the GNU General Public License (GPL) version 3 - 
-see the LICENSE file for details.
+see the `LICENSE <https://github.com/hghcomphys/jaxip/blob/main/LICENSE>`_ file for details.
```

### Comparing `jaxip-0.5.6/README.rst` & `jaxip-0.5.7/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -136,8 +136,8 @@
         nnp.compute_force(structure)
 
 
 License
 -------
 
 This project is licensed under the GNU General Public License (GPL) version 3 - 
-see the LICENSE file for details.
+see the `LICENSE <https://github.com/hghcomphys/jaxip/blob/main/LICENSE>`_ file for details.
```

### Comparing `jaxip-0.5.6/docs/Makefile` & `jaxip-0.5.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.6/docs/_build/doctrees/nbsphinx/notebooks_potential_training_29_21.png` & `jaxip-0.5.7/docs/_build/doctrees/nbsphinx/notebooks_potential_training_29_21.png`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.6/docs/_build/doctrees/nbsphinx/notebooks_tutorials_38_0.png` & `jaxip-0.5.7/docs/_build/doctrees/nbsphinx/notebooks_tutorials_38_0.png`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.6/docs/_build/doctrees/nbsphinx/notebooks_tutorials_45_0.png` & `jaxip-0.5.7/docs/_build/doctrees/nbsphinx/notebooks_tutorials_45_0.png`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.6/docs/_build/doctrees/nbsphinx/notebooks_tutorials_51_0.png` & `jaxip-0.5.7/docs/_build/doctrees/nbsphinx/notebooks_tutorials_51_0.png`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.6/docs/_build/html/_images/notebooks_potential_training_29_21.png` & `jaxip-0.5.7/docs/_build/html/_images/notebooks_potential_training_29_21.png`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.6/docs/_build/html/_images/notebooks_tutorials_38_0.png` & `jaxip-0.5.7/docs/_build/html/_images/notebooks_tutorials_38_0.png`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.6/docs/_build/html/_images/notebooks_tutorials_45_0.png` & `jaxip-0.5.7/docs/_build/html/_images/notebooks_tutorials_45_0.png`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.6/docs/_build/html/_images/notebooks_tutorials_51_0.png` & `jaxip-0.5.7/docs/_build/html/_images/notebooks_tutorials_51_0.png`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.6/docs/conf.py` & `jaxip-0.5.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.6/docs/images/flowchart.drawio.png` & `jaxip-0.5.7/docs/images/flowchart.drawio.png`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.6/docs/images/water.png` & `jaxip-0.5.7/docs/images/water.png`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.6/docs/installation.rst` & `jaxip-0.5.7/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.6/docs/jaxip.atoms.rst` & `jaxip-0.5.7/docs/jaxip.atoms.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.6/docs/jaxip.datasets.rst` & `jaxip-0.5.7/docs/jaxip.utils.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,53 @@
-jaxip.datasets package
-======================
+jaxip.utils package
+===================
 
 Submodules
 ----------
 
-jaxip.datasets.base module
+jaxip.utils.attribute module
+----------------------------
+
+.. automodule:: jaxip.utils.attribute
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
+jaxip.utils.batch module
+------------------------
+
+.. automodule:: jaxip.utils.batch
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
+jaxip.utils.compare module
 --------------------------
 
-.. automodule:: jaxip.datasets.base
+.. automodule:: jaxip.utils.compare
    :members:
    :undoc-members:
    :show-inheritance:
 
-jaxip.datasets.runner module
-----------------------------
+jaxip.utils.profiler module
+---------------------------
 
-.. automodule:: jaxip.datasets.runner
+.. automodule:: jaxip.utils.profiler
    :members:
    :undoc-members:
    :show-inheritance:
 
-jaxip.datasets.transformer module
----------------------------------
+jaxip.utils.tokenize module
+---------------------------
 
-.. automodule:: jaxip.datasets.transformer
+.. automodule:: jaxip.utils.tokenize
    :members:
    :undoc-members:
    :show-inheritance:
 
 Module contents
 ---------------
 
-.. automodule:: jaxip.datasets
+.. automodule:: jaxip.utils
    :members:
    :undoc-members:
    :show-inheritance:
```

### Comparing `jaxip-0.5.6/docs/jaxip.descriptors.acsf.rst` & `jaxip-0.5.7/docs/jaxip.descriptors.acsf.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.6/docs/jaxip.descriptors.rst` & `jaxip-0.5.7/docs/jaxip.descriptors.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.6/docs/jaxip.models.rst` & `jaxip-0.5.7/docs/jaxip.models.nn.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-jaxip.models package
-====================
+jaxip.models.nn package
+=======================
 
 Submodules
 ----------
 
-jaxip.models.activation module
-------------------------------
+jaxip.models.nn.activation module
+---------------------------------
 
-.. automodule:: jaxip.models.activation
+.. automodule:: jaxip.models.nn.activation
    :members:
    :undoc-members:
    :show-inheritance:
 
-jaxip.models.initializer module
--------------------------------
+jaxip.models.nn.initializer module
+----------------------------------
 
-.. automodule:: jaxip.models.initializer
+.. automodule:: jaxip.models.nn.initializer
    :members:
    :undoc-members:
    :show-inheritance:
 
-jaxip.models.nn module
-----------------------
+jaxip.models.nn.network module
+------------------------------
 
-.. automodule:: jaxip.models.nn
+.. automodule:: jaxip.models.nn.network
    :members:
    :undoc-members:
    :show-inheritance:
 
 Module contents
 ---------------
 
-.. automodule:: jaxip.models
+.. automodule:: jaxip.models.nn
    :members:
    :undoc-members:
    :show-inheritance:
```

### Comparing `jaxip-0.5.6/docs/jaxip.potentials.nnp.rst` & `jaxip-0.5.7/docs/jaxip.potentials.nnp.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.6/docs/jaxip.rst` & `jaxip-0.5.7/docs/jaxip.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.6/docs/make.bat` & `jaxip-0.5.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.6/docs/theory.rst` & `jaxip-0.5.7/docs/theory.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.6/docs/usage.rst` & `jaxip-0.5.7/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.6/jaxip/__init__.py` & `jaxip-0.5.7/jaxip/__init__.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.6/jaxip/atoms/_neighbor.py` & `jaxip-0.5.7/jaxip/atoms/_neighbor.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.6/jaxip/atoms/_structure.py` & `jaxip-0.5.7/jaxip/atoms/_structure.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.6/jaxip/atoms/box.py` & `jaxip-0.5.7/jaxip/atoms/box.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.6/jaxip/atoms/element.py` & `jaxip-0.5.7/jaxip/atoms/element.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.6/jaxip/atoms/neighbor.py` & `jaxip-0.5.7/jaxip/atoms/neighbor.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.6/jaxip/atoms/structure.py` & `jaxip-0.5.7/jaxip/atoms/structure.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.6/jaxip/base.py` & `jaxip-0.5.7/jaxip/base.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.6/jaxip/config.py` & `jaxip-0.5.7/jaxip/config.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.6/jaxip/datasets/runner.py` & `jaxip-0.5.7/jaxip/datasets/runner.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,36 @@
 from __future__ import annotations
 
 from collections import defaultdict
 from pathlib import Path
-from typing import DefaultDict, Dict, List, Optional, TextIO
+from typing import DefaultDict, Dict, List, Optional, Protocol, TextIO
 
 from jaxip.atoms.structure import Structure
-from jaxip.datasets.base import StructureDataset
 from jaxip.datasets.transformer import ToStructure, Transformer
 from jaxip.logger import logger
 from jaxip.utils.tokenize import tokenize
 
 
-class RunnerDataset(StructureDataset):
+class Dataset(Protocol):
+    """
+    A data container for atom data structure.
+
+    Features:
+
+    * it must access data item in a lazy mode.
+    * it should be able to cache data via a `persist` input flag.
+    """
+
+    def __len__(self) -> int:
+        ...
+
+    def __getitem__(self, index: int) -> Structure:
+        ...
+
+class RunnerDataset(Dataset):
     """
     Dataset for `RuNNer`_ data file format.
 
     The input structure file contains atom info and simulation box.
     Each snapshot contains two per-atom and collective properties as follows:
 
     * `per-atom` properties include the element name, positions, energy, charge, force components, etc.
```

### Comparing `jaxip-0.5.6/jaxip/datasets/transformer.py` & `jaxip-0.5.7/jaxip/datasets/transformer.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.6/jaxip/descriptors/acsf/_acsf.py` & `jaxip-0.5.7/jaxip/descriptors/acsf/_acsf.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.6/jaxip/descriptors/acsf/acsf.py` & `jaxip-0.5.7/jaxip/descriptors/acsf/acsf.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.6/jaxip/descriptors/acsf/angular.py` & `jaxip-0.5.7/jaxip/descriptors/acsf/angular.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.6/jaxip/descriptors/acsf/cutoff.py` & `jaxip-0.5.7/jaxip/descriptors/acsf/cutoff.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import functools
 import math
 from dataclasses import dataclass
 from typing import Callable, Optional
 
 import jax
 import jax.numpy as jnp
 
@@ -20,26 +21,36 @@
 
     .. _`cutoff function`: https://compphysvienna.github.io/n2p2/api/cutoff_functions.html?highlight=cutoff#
     .. _`cutoff type`: https://compphysvienna.github.io/n2p2/topics/keywords.html?highlight=cutoff_type
     """
 
     r_cutoff: float
     cutoff_type: str = "tanh"
-    cutoff_function: Optional[Callable] = None  # lambda r: r
+    cutoff_function: Optional[Callable] = None
 
     def __post_init__(self) -> None:
         self.cutoff_type = self.cutoff_type.lower()
         if self.cutoff_function is None:
             try:
                 self.cutoff_function = getattr(self, f"{self.cutoff_type}")
             except AttributeError:
                 logger.error(
                     f"'{self.__class__.__name__}' has no cutoff function '{self.cutoff_type}'",
                     exception=NotImplementedError,
                 )
+        self._check_jit_attributes()
+
+    @classmethod
+    def _check_jit_attributes(cls) -> None:
+        """An optional check to ensure jit static and dynamics attributes are correctly identified."""
+        assert cls._get_jit_dynamic_attributes() == tuple()
+        assert (
+            cls._get_jit_static_attributes() == \
+            ('r_cutoff', 'cutoff_type', 'cutoff_function')
+        )
 
     def __hash__(self) -> int:
         """Enforce to use the parent class's hash method (JIT)."""
         return super().__hash__()
 
     @jax.jit
     def __call__(self, r: Array) -> Array:
```

### Comparing `jaxip-0.5.6/jaxip/descriptors/acsf/radial.py` & `jaxip-0.5.7/jaxip/descriptors/acsf/radial.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.6/jaxip/descriptors/acsf/symmetry.py` & `jaxip-0.5.7/jaxip/descriptors/acsf/symmetry.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.6/jaxip/descriptors/base.py` & `jaxip-0.5.7/jaxip/descriptors/base.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.6/jaxip/descriptors/scaler.py` & `jaxip-0.5.7/jaxip/descriptors/scaler.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.6/jaxip/logger.py` & `jaxip-0.5.7/jaxip/logger.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.6/jaxip/models/activation.py` & `jaxip-0.5.7/jaxip/models/nn/activation.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.6/jaxip/models/initializer.py` & `jaxip-0.5.7/jaxip/models/nn/initializer.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.6/jaxip/models/nn.py` & `jaxip-0.5.7/jaxip/models/nn/network.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 from typing import Callable, List, Tuple
 
 from flax import linen as nn
 from frozendict import frozendict
 
 from jaxip.logger import logger
-from jaxip.models.activation import _activation_function_map
+from jaxip.models.nn.activation import _activation_function_map
 from jaxip.types import Array, Dtype
 from jaxip.types import dtype as _dtype
 
 
 class NeuralNetworkModel(nn.Module):
     """Neural network model that outputs energy."""
```

### Comparing `jaxip-0.5.6/jaxip/potentials/_energy.py` & `jaxip-0.5.7/jaxip/potentials/_energy.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.6/jaxip/potentials/_force.py` & `jaxip-0.5.7/jaxip/potentials/_force.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.6/jaxip/potentials/atomic_potential.py` & `jaxip-0.5.7/jaxip/potentials/atomic_potential.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from dataclasses import dataclass
 
 from frozendict import frozendict
 
 from jaxip.atoms.structure import Structure
 from jaxip.descriptors.base import Descriptor
 from jaxip.descriptors.scaler import Scaler
-from jaxip.models.nn import NeuralNetworkModel
+from jaxip.models.nn.network import NeuralNetworkModel
 from jaxip.potentials._energy import _compute_atomic_energy
 from jaxip.types import Array, Element
 
 
 @dataclass(frozen=True)
 class AtomicPotential:
     """
```

### Comparing `jaxip-0.5.6/jaxip/potentials/nnp/gradient_descent.py` & `jaxip-0.5.7/jaxip/potentials/nnp/gradient_descent.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,59 @@
 from __future__ import annotations
 
 import math
 import random
 from collections import defaultdict
-from typing import Any, Callable, Dict, List, Tuple
+from typing import Any, Callable, Dict, List, Protocol, Tuple
 
 import jax.numpy as jnp
 import numpy as np
 import optax
 from flax.training.train_state import TrainState
 from frozendict import frozendict
 from jax import value_and_grad
 from optax import GradientTransformation
 from tqdm import tqdm
 
 from jaxip.atoms.structure import Structure
-from jaxip.datasets.base import StructureDataset
 from jaxip.logger import logger
 from jaxip.potentials._energy import _energy_fn
 from jaxip.potentials._force import _compute_force
-from jaxip.potentials.base import Potential, Updater
+from jaxip.potentials.atomic_potential import AtomicPotential
 from jaxip.potentials.nnp.metrics import ErrorMetric
 from jaxip.potentials.nnp.settings import PotentialSettings
 from jaxip.types import Array, Element
 
 
 def _mse_loss(*, logits: Array, targets: Array) -> Array:
     return ((targets - logits) ** 2).mean()
 
+class StructureDataset(Protocol):
+    """A data container for atom data structure."""
+
+    def __len__(self) -> int:
+        ...
+
+    def __getitem__(self, index: int) -> Structure:
+        ...
+
+class Updater(Protocol):
+    """Interface for potential weight updaters."""
+
+    def fit(self, dataset: StructureDataset) -> Dict:
+        ...
+
+
+class Potential(Protocol):
+    """Interface for Potential."""
+
+    settings: PotentialSettings
+    elements: Tuple[Element, ...]
+    atomic_potential: Dict[Element, AtomicPotential]
+    model_params: Dict[Element, frozendict]
 
 # @dataclass
 class GradientDescentUpdater(Updater):
     """
     A trainer class to fit a generic NNP potential weights using target values of the total
     energy and force components.
```

### Comparing `jaxip-0.5.6/jaxip/potentials/nnp/kalman_filter.py` & `jaxip-0.5.7/jaxip/potentials/nnp/kalman_filter.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,57 @@
 import random
 from collections import defaultdict
-from typing import Callable, Dict
+from typing import Callable, Dict, Protocol, Tuple
 
 import jax
 import jax.numpy as jnp
 import numpy as np
 from frozendict import frozendict
 from jax import flatten_util
 from tqdm import tqdm
 
 from jaxip.atoms.structure import Structure
-from jaxip.datasets.base import StructureDataset
 from jaxip.logger import logger
 from jaxip.potentials._energy import _compute_energy
 from jaxip.potentials._force import _compute_force
 from jaxip.potentials.atomic_potential import AtomicPotential
-from jaxip.potentials.base import Potential, Updater
 from jaxip.potentials.nnp.settings import PotentialSettings
 from jaxip.types import Array, Element
 from jaxip.types import dtype as default_dtype
 
 
 def _tree_flatten(pytree: Dict) -> Array:
     return flatten_util.ravel_pytree(pytree)[0].reshape(-1, 1)  # type: ignore
 
 
+class StructureDataset(Protocol):
+    """A data container for atom data structure."""
+
+    def __len__(self) -> int:
+        ...
+
+    def __getitem__(self, index: int) -> Structure:
+        ...
+
+class Updater(Protocol):
+    """Interface for potential weight updaters."""
+
+    def fit(self, dataset: StructureDataset) -> Dict:
+        ...
+
+
+class Potential(Protocol):
+    """Interface for Potential."""
+
+    settings: PotentialSettings
+    elements: Tuple[Element, ...]
+    atomic_potential: Dict[Element, AtomicPotential]
+    model_params: Dict[Element, frozendict]
+
+
 class KalmanFilterUpdater(Updater):
     """
     A potential trainer which uses Kalman filter to update model weights (see this_).
 
     .. _this: https://pubs.acs.org/doi/10.1021/acs.jctc.8b01092
     """
```

### Comparing `jaxip-0.5.6/jaxip/potentials/nnp/metrics.py` & `jaxip-0.5.7/jaxip/potentials/nnp/metrics.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.6/jaxip/potentials/nnp/potential.py` & `jaxip-0.5.7/jaxip/potentials/nnp/potential.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 from collections import defaultdict
 from dataclasses import dataclass, field
 from pathlib import Path
-from typing import Dict, Optional, Tuple
+from typing import Dict, Optional, Protocol, Tuple
 
 import jax.numpy as jnp
 from ase import data
 from frozendict import frozendict
 from jax import random
 from tqdm import tqdm
 
@@ -16,26 +16,41 @@
 from jaxip.datasets.runner import RunnerDataset
 from jaxip.descriptors.acsf.acsf import ACSF
 from jaxip.descriptors.acsf.angular import G3, G9
 from jaxip.descriptors.acsf.cutoff import CutoffFunction
 from jaxip.descriptors.acsf.radial import G1, G2
 from jaxip.descriptors.scaler import Scaler
 from jaxip.logger import logger
-from jaxip.models.initializer import UniformInitializer
-from jaxip.models.nn import NeuralNetworkModel
+from jaxip.models.nn.initializer import UniformInitializer
+from jaxip.models.nn.network import NeuralNetworkModel
 from jaxip.potentials._energy import _compute_energy
 from jaxip.potentials._force import _compute_force
 from jaxip.potentials.atomic_potential import AtomicPotential
-from jaxip.potentials.base import Updater
 from jaxip.potentials.nnp.gradient_descent import GradientDescentUpdater
 from jaxip.potentials.nnp.kalman_filter import KalmanFilterUpdater
 from jaxip.potentials.nnp.settings import PotentialSettings
 from jaxip.types import Array, Element
 
 
+class StructureDataset(Protocol):
+    """A data container for atom data structure."""
+
+    def __len__(self) -> int:
+        ...
+
+    def __getitem__(self, index: int) -> Structure:
+        ...
+
+class Updater(Protocol):
+    """Interface for potential weight updaters."""
+
+    def fit(self, dataset: StructureDataset) -> Dict:
+        ...
+
+
 @dataclass
 class NeuralNetworkPotential:
     """
     High-dimensional neural network potential (HDNNP) - second generation.
 
     It contains all the required descriptors, scalers, and neural networks for each element,
     and an updater to fit the potential model using the reference structure data.
```

### Comparing `jaxip-0.5.6/jaxip/potentials/nnp/settings.py` & `jaxip-0.5.7/jaxip/potentials/nnp/settings.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.6/jaxip/types.py` & `jaxip-0.5.7/jaxip/types.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.6/jaxip/utils/attribute.py` & `jaxip-0.5.7/jaxip/utils/attribute.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.6/jaxip/utils/batch.py` & `jaxip-0.5.7/jaxip/utils/batch.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.6/jaxip/utils/compare.py` & `jaxip-0.5.7/jaxip/utils/compare.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.6/jaxip/utils/profiler.py` & `jaxip-0.5.7/jaxip/utils/profiler.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.6/jaxip/utils/tokenize.py` & `jaxip-0.5.7/jaxip/utils/tokenize.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.6/jaxip.egg-info/PKG-INFO` & `jaxip-0.5.7/jaxip.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaxip
-Version: 0.5.6
+Version: 0.5.7
 Summary: JAX-based Interatomic Potential
 Home-page: https://github.com/hghcomphys/jaxip
 Author: Hossein Ghorbanfekr
 Author-email: hgh.comphys@gmail.com
 License: GNU General Public License v3
 Keywords: jaxip
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -154,8 +154,8 @@
         nnp.compute_force(structure)
 
 
 License
 -------
 
 This project is licensed under the GNU General Public License (GPL) version 3 - 
-see the LICENSE file for details.
+see the `LICENSE <https://github.com/hghcomphys/jaxip/blob/main/LICENSE>`_ file for details.
```

### Comparing `jaxip-0.5.6/jaxip.egg-info/SOURCES.txt` & `jaxip-0.5.7/jaxip.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 docs/history.rst
 docs/index.rst
 docs/installation.rst
 docs/jaxip.atoms.rst
 docs/jaxip.datasets.rst
 docs/jaxip.descriptors.acsf.rst
 docs/jaxip.descriptors.rst
+docs/jaxip.models.nn.rst
 docs/jaxip.models.rst
 docs/jaxip.potentials.nnp.rst
 docs/jaxip.potentials.rst
 docs/jaxip.rst
 docs/jaxip.utils.rst
 docs/make.bat
 docs/modules.rst
@@ -60,36 +61,35 @@
 jaxip/atoms/_neighbor.py
 jaxip/atoms/_structure.py
 jaxip/atoms/box.py
 jaxip/atoms/element.py
 jaxip/atoms/neighbor.py
 jaxip/atoms/structure.py
 jaxip/datasets/__init__.py
-jaxip/datasets/base.py
 jaxip/datasets/runner.py
 jaxip/datasets/transformer.py
 jaxip/descriptors/__init__.py
 jaxip/descriptors/base.py
 jaxip/descriptors/scaler.py
 jaxip/descriptors/acsf/__init__.py
 jaxip/descriptors/acsf/_acsf.py
 jaxip/descriptors/acsf/acsf.py
 jaxip/descriptors/acsf/angular.py
 jaxip/descriptors/acsf/cutoff.py
 jaxip/descriptors/acsf/radial.py
 jaxip/descriptors/acsf/symmetry.py
 jaxip/models/__init__.py
-jaxip/models/activation.py
-jaxip/models/initializer.py
-jaxip/models/nn.py
+jaxip/models/nn/__init__.py
+jaxip/models/nn/activation.py
+jaxip/models/nn/initializer.py
+jaxip/models/nn/network.py
 jaxip/potentials/__init__.py
 jaxip/potentials/_energy.py
 jaxip/potentials/_force.py
 jaxip/potentials/atomic_potential.py
-jaxip/potentials/base.py
 jaxip/potentials/nnp/__init__.py
 jaxip/potentials/nnp/gradient_descent.py
 jaxip/potentials/nnp/kalman_filter.py
 jaxip/potentials/nnp/metrics.py
 jaxip/potentials/nnp/potential.py
 jaxip/potentials/nnp/settings.py
 jaxip/utils/__init__.py
```

### Comparing `jaxip-0.5.6/setup.py` & `jaxip-0.5.7/setup.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.6/tests/.ipynb_checkpoints/h2o-checkpoint.data` & `jaxip-0.5.7/tests/.ipynb_checkpoints/h2o-checkpoint.data`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.6/tests/.ipynb_checkpoints/h2o-checkpoint.json` & `jaxip-0.5.7/tests/.ipynb_checkpoints/h2o-checkpoint.json`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.6/tests/.ipynb_checkpoints/input.h2o-checkpoint.data` & `jaxip-0.5.7/tests/.ipynb_checkpoints/input.h2o-checkpoint.data`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.6/tests/.ipynb_checkpoints/test-checkpoint.ipynb` & `jaxip-0.5.7/tests/.ipynb_checkpoints/test-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.6/tests/h2o.data` & `jaxip-0.5.7/tests/h2o.data`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.6/tests/h2o.json` & `jaxip-0.5.7/tests/h2o.json`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.6/tests/test_acsf.py` & `jaxip-0.5.7/tests/test_acsf.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.6/tests/test_nn.py` & `jaxip-0.5.7/tests/test_nn.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 os.environ["JAX_PLATFORM_NAME"] = "cpu"
 
 import jax
 import jax.numpy as jnp
 import pytest
 from frozendict import frozendict
 
-from jaxip.models.initializer import UniformInitializer
-from jaxip.models.nn import NeuralNetworkModel
+from jaxip.models.nn.initializer import UniformInitializer
+from jaxip.models.nn.network import NeuralNetworkModel
 from jaxip.types import dtype as _dtype
 
 
 class TestNeuralNetworkModel:
 
     nn_1: NeuralNetworkModel = NeuralNetworkModel(hidden_layers=((2, "tanh"),))
     nn_2: NeuralNetworkModel = NeuralNetworkModel(
```

### Comparing `jaxip-0.5.6/tests/test_nnp.py` & `jaxip-0.5.7/tests/test_nnp.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.6/tests/test_runner.py` & `jaxip-0.5.7/tests/test_runner.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.6/tests/test_scaler.py` & `jaxip-0.5.7/tests/test_scaler.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.6/tests/test_structure.py` & `jaxip-0.5.7/tests/test_structure.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.6/tests/weights.001.pkl` & `jaxip-0.5.7/tests/weights.001.pkl`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.6/tests/weights.008.pkl` & `jaxip-0.5.7/tests/weights.008.pkl`

 * *Files identical despite different names*

