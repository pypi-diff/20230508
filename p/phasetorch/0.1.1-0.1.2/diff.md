# Comparing `tmp/phasetorch-0.1.1.tar.gz` & `tmp/phasetorch-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phasetorch-0.1.1.tar", last modified: Mon May  8 14:09:25 2023, max compression
+gzip compressed data, was "phasetorch-0.1.2.tar", last modified: Mon May  8 14:41:34 2023, max compression
```

## Comparing `phasetorch-0.1.1.tar` & `phasetorch-0.1.2.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwx------   0 mohan3   (25677) mohan3   (25677)        0 2023-05-08 14:09:25.606858 phasetorch-0.1.1/
--rw-------   0 mohan3   (25677) mohan3   (25677)    17711 2023-05-08 14:08:22.000000 phasetorch-0.1.1/LICENSE
--rw-------   0 mohan3   (25677) mohan3   (25677)       16 2023-05-08 14:07:44.000000 phasetorch-0.1.1/MANIFEST.in
--rw-------   0 mohan3   (25677) mohan3   (25677)     1187 2023-05-08 14:08:22.000000 phasetorch-0.1.1/NOTICE
--rw-------   0 mohan3   (25677) mohan3   (25677)     1149 2023-05-08 14:09:25.605866 phasetorch-0.1.1/PKG-INFO
--rw-------   0 mohan3   (25677) mohan3   (25677)      684 2023-05-08 14:08:22.000000 phasetorch-0.1.1/README.rst
--rw-------   0 mohan3   (25677) mohan3   (25677)        6 2023-05-08 14:08:22.000000 phasetorch-0.1.1/VERSION
-drwx------   0 mohan3   (25677) mohan3   (25677)        0 2023-05-08 14:09:25.564852 phasetorch-0.1.1/phasetorch/
--rw-------   0 mohan3   (25677) mohan3   (25677)        0 2023-03-31 19:38:57.000000 phasetorch-0.1.1/phasetorch/__init__.py
-drwx------   0 mohan3   (25677) mohan3   (25677)        0 2023-05-08 14:09:25.586878 phasetorch-0.1.1/phasetorch/mono/
--rw-------   0 mohan3   (25677) mohan3   (25677)        0 2023-04-29 19:43:30.000000 phasetorch-0.1.1/phasetorch/mono/__init__.py
--rw-------   0 mohan3   (25677) mohan3   (25677)     6510 2023-04-29 19:43:30.000000 phasetorch-0.1.1/phasetorch/mono/_fresmod.py
--rw-------   0 mohan3   (25677) mohan3   (25677)    11487 2023-04-29 19:43:30.000000 phasetorch-0.1.1/phasetorch/mono/_mullpr.py
--rw-------   0 mohan3   (25677) mohan3   (25677)    18231 2023-04-29 19:43:30.000000 phasetorch-0.1.1/phasetorch/mono/_mulmod.py
--rw-------   0 mohan3   (25677) mohan3   (25677)    32588 2023-04-29 19:43:30.000000 phasetorch-0.1.1/phasetorch/mono/_nonlpr.py
--rw-------   0 mohan3   (25677) mohan3   (25677)     4592 2023-04-29 19:43:30.000000 phasetorch-0.1.1/phasetorch/mono/_nonmod.py
--rw-------   0 mohan3   (25677) mohan3   (25677)    13313 2023-04-29 19:43:30.000000 phasetorch-0.1.1/phasetorch/mono/_simtor.py
--rw-------   0 mohan3   (25677) mohan3   (25677)     5830 2023-04-29 19:43:30.000000 phasetorch-0.1.1/phasetorch/mono/_sinlpr.py
--rw-------   0 mohan3   (25677) mohan3   (25677)     1785 2023-04-29 19:43:30.000000 phasetorch-0.1.1/phasetorch/mono/_sinmod.py
--rw-------   0 mohan3   (25677) mohan3   (25677)      550 2023-04-29 19:43:30.000000 phasetorch-0.1.1/phasetorch/mono/eval.py
--rw-------   0 mohan3   (25677) mohan3   (25677)      159 2023-04-29 19:43:30.000000 phasetorch-0.1.1/phasetorch/mono/pr.py
--rw-------   0 mohan3   (25677) mohan3   (25677)      117 2023-04-29 19:43:30.000000 phasetorch-0.1.1/phasetorch/mono/sim.py
-drwx------   0 mohan3   (25677) mohan3   (25677)        0 2023-05-08 14:09:25.588856 phasetorch-0.1.1/phasetorch/opt/
--rw-------   0 mohan3   (25677) mohan3   (25677)        0 2023-04-29 19:43:30.000000 phasetorch-0.1.1/phasetorch/opt/__init__.py
-drwx------   0 mohan3   (25677) mohan3   (25677)        0 2023-05-08 14:09:25.589871 phasetorch-0.1.1/phasetorch/opt/_pytorch_lbfgs/
--rw-------   0 mohan3   (25677) mohan3   (25677)        0 2023-04-29 19:43:30.000000 phasetorch-0.1.1/phasetorch/opt/_pytorch_lbfgs/__init__.py
-drwx------   0 mohan3   (25677) mohan3   (25677)        0 2023-05-08 14:09:25.594850 phasetorch-0.1.1/phasetorch/opt/_pytorch_lbfgs/functions/
--rw-------   0 mohan3   (25677) mohan3   (25677)    43231 2023-04-29 19:43:30.000000 phasetorch-0.1.1/phasetorch/opt/_pytorch_lbfgs/functions/LBFGS.py
--rw-------   0 mohan3   (25677) mohan3   (25677)        0 2023-04-29 19:43:30.000000 phasetorch-0.1.1/phasetorch/opt/_pytorch_lbfgs/functions/__init__.py
--rw-------   0 mohan3   (25677) mohan3   (25677)     6334 2023-04-29 19:43:30.000000 phasetorch-0.1.1/phasetorch/opt/_pytorch_lbfgs/functions/utils.py
-drwx------   0 mohan3   (25677) mohan3   (25677)        0 2023-05-08 14:09:25.604852 phasetorch-0.1.1/phasetorch/util/
--rw-------   0 mohan3   (25677) mohan3   (25677)      190 2023-04-29 19:43:30.000000 phasetorch-0.1.1/phasetorch/util/__init__.py
--rw-------   0 mohan3   (25677) mohan3   (25677)     3447 2023-04-29 19:43:30.000000 phasetorch-0.1.1/phasetorch/util/_check.py
--rw-------   0 mohan3   (25677) mohan3   (25677)     4496 2023-04-29 19:43:30.000000 phasetorch-0.1.1/phasetorch/util/_pad.py
--rw-------   0 mohan3   (25677) mohan3   (25677)     9199 2023-04-29 19:43:30.000000 phasetorch-0.1.1/phasetorch/util/_proc.py
--rw-------   0 mohan3   (25677) mohan3   (25677)     2658 2023-04-29 19:43:30.000000 phasetorch-0.1.1/phasetorch/util/_projs.py
--rw-------   0 mohan3   (25677) mohan3   (25677)     4806 2023-04-29 19:43:30.000000 phasetorch-0.1.1/phasetorch/util/_tutils.py
--rw-------   0 mohan3   (25677) mohan3   (25677)     4657 2023-04-29 19:43:30.000000 phasetorch-0.1.1/phasetorch/util/_utils.py
-drwx------   0 mohan3   (25677) mohan3   (25677)        0 2023-05-08 14:09:25.570858 phasetorch-0.1.1/phasetorch.egg-info/
--rw-------   0 mohan3   (25677) mohan3   (25677)     1149 2023-05-08 14:09:25.000000 phasetorch-0.1.1/phasetorch.egg-info/PKG-INFO
--rw-------   0 mohan3   (25677) mohan3   (25677)     1213 2023-05-08 14:09:25.000000 phasetorch-0.1.1/phasetorch.egg-info/SOURCES.txt
--rw-------   0 mohan3   (25677) mohan3   (25677)        1 2023-05-08 14:09:25.000000 phasetorch-0.1.1/phasetorch.egg-info/dependency_links.txt
--rw-------   0 mohan3   (25677) mohan3   (25677)        1 2023-03-31 19:38:57.000000 phasetorch-0.1.1/phasetorch.egg-info/not-zip-safe
--rw-------   0 mohan3   (25677) mohan3   (25677)       11 2023-05-08 14:09:25.000000 phasetorch-0.1.1/phasetorch.egg-info/top_level.txt
--rw-------   0 mohan3   (25677) mohan3   (25677)       38 2023-05-08 14:09:25.606874 phasetorch-0.1.1/setup.cfg
--rw-------   0 mohan3   (25677) mohan3   (25677)      913 2023-05-08 14:08:22.000000 phasetorch-0.1.1/setup.py
+drwx------   0 mohan3   (25677) mohan3   (25677)        0 2023-05-08 14:41:34.492424 phasetorch-0.1.2/
+-rw-------   0 mohan3   (25677) mohan3   (25677)    17711 2023-05-08 14:36:22.000000 phasetorch-0.1.2/LICENSE
+-rw-------   0 mohan3   (25677) mohan3   (25677)       16 2023-05-08 14:07:44.000000 phasetorch-0.1.2/MANIFEST.in
+-rw-------   0 mohan3   (25677) mohan3   (25677)     1187 2023-05-08 14:36:22.000000 phasetorch-0.1.2/NOTICE
+-rw-------   0 mohan3   (25677) mohan3   (25677)     1095 2023-05-08 14:41:34.491510 phasetorch-0.1.2/PKG-INFO
+-rw-------   0 mohan3   (25677) mohan3   (25677)      684 2023-05-08 14:36:22.000000 phasetorch-0.1.2/README.rst
+-rw-------   0 mohan3   (25677) mohan3   (25677)        6 2023-05-08 14:39:05.000000 phasetorch-0.1.2/VERSION
+drwx------   0 mohan3   (25677) mohan3   (25677)        0 2023-05-08 14:41:34.447401 phasetorch-0.1.2/phasetorch/
+-rw-------   0 mohan3   (25677) mohan3   (25677)        0 2023-03-31 19:38:57.000000 phasetorch-0.1.2/phasetorch/__init__.py
+drwx------   0 mohan3   (25677) mohan3   (25677)        0 2023-05-08 14:41:34.470436 phasetorch-0.1.2/phasetorch/mono/
+-rw-------   0 mohan3   (25677) mohan3   (25677)        0 2023-04-29 19:43:30.000000 phasetorch-0.1.2/phasetorch/mono/__init__.py
+-rw-------   0 mohan3   (25677) mohan3   (25677)     6510 2023-04-29 19:43:30.000000 phasetorch-0.1.2/phasetorch/mono/_fresmod.py
+-rw-------   0 mohan3   (25677) mohan3   (25677)    11487 2023-04-29 19:43:30.000000 phasetorch-0.1.2/phasetorch/mono/_mullpr.py
+-rw-------   0 mohan3   (25677) mohan3   (25677)    18231 2023-04-29 19:43:30.000000 phasetorch-0.1.2/phasetorch/mono/_mulmod.py
+-rw-------   0 mohan3   (25677) mohan3   (25677)    32588 2023-04-29 19:43:30.000000 phasetorch-0.1.2/phasetorch/mono/_nonlpr.py
+-rw-------   0 mohan3   (25677) mohan3   (25677)     4592 2023-04-29 19:43:30.000000 phasetorch-0.1.2/phasetorch/mono/_nonmod.py
+-rw-------   0 mohan3   (25677) mohan3   (25677)    13313 2023-04-29 19:43:30.000000 phasetorch-0.1.2/phasetorch/mono/_simtor.py
+-rw-------   0 mohan3   (25677) mohan3   (25677)     5830 2023-04-29 19:43:30.000000 phasetorch-0.1.2/phasetorch/mono/_sinlpr.py
+-rw-------   0 mohan3   (25677) mohan3   (25677)     1785 2023-04-29 19:43:30.000000 phasetorch-0.1.2/phasetorch/mono/_sinmod.py
+-rw-------   0 mohan3   (25677) mohan3   (25677)      550 2023-04-29 19:43:30.000000 phasetorch-0.1.2/phasetorch/mono/eval.py
+-rw-------   0 mohan3   (25677) mohan3   (25677)      159 2023-04-29 19:43:30.000000 phasetorch-0.1.2/phasetorch/mono/pr.py
+-rw-------   0 mohan3   (25677) mohan3   (25677)      117 2023-04-29 19:43:30.000000 phasetorch-0.1.2/phasetorch/mono/sim.py
+drwx------   0 mohan3   (25677) mohan3   (25677)        0 2023-05-08 14:41:34.471471 phasetorch-0.1.2/phasetorch/opt/
+-rw-------   0 mohan3   (25677) mohan3   (25677)        0 2023-04-29 19:43:30.000000 phasetorch-0.1.2/phasetorch/opt/__init__.py
+drwx------   0 mohan3   (25677) mohan3   (25677)        0 2023-05-08 14:41:34.473426 phasetorch-0.1.2/phasetorch/opt/_pytorch_lbfgs/
+-rw-------   0 mohan3   (25677) mohan3   (25677)        0 2023-04-29 19:43:30.000000 phasetorch-0.1.2/phasetorch/opt/_pytorch_lbfgs/__init__.py
+drwx------   0 mohan3   (25677) mohan3   (25677)        0 2023-05-08 14:41:34.477490 phasetorch-0.1.2/phasetorch/opt/_pytorch_lbfgs/functions/
+-rw-------   0 mohan3   (25677) mohan3   (25677)    43231 2023-04-29 19:43:30.000000 phasetorch-0.1.2/phasetorch/opt/_pytorch_lbfgs/functions/LBFGS.py
+-rw-------   0 mohan3   (25677) mohan3   (25677)        0 2023-04-29 19:43:30.000000 phasetorch-0.1.2/phasetorch/opt/_pytorch_lbfgs/functions/__init__.py
+-rw-------   0 mohan3   (25677) mohan3   (25677)     6334 2023-04-29 19:43:30.000000 phasetorch-0.1.2/phasetorch/opt/_pytorch_lbfgs/functions/utils.py
+drwx------   0 mohan3   (25677) mohan3   (25677)        0 2023-05-08 14:41:34.489445 phasetorch-0.1.2/phasetorch/util/
+-rw-------   0 mohan3   (25677) mohan3   (25677)      190 2023-04-29 19:43:30.000000 phasetorch-0.1.2/phasetorch/util/__init__.py
+-rw-------   0 mohan3   (25677) mohan3   (25677)     3447 2023-04-29 19:43:30.000000 phasetorch-0.1.2/phasetorch/util/_check.py
+-rw-------   0 mohan3   (25677) mohan3   (25677)     4496 2023-04-29 19:43:30.000000 phasetorch-0.1.2/phasetorch/util/_pad.py
+-rw-------   0 mohan3   (25677) mohan3   (25677)     9199 2023-04-29 19:43:30.000000 phasetorch-0.1.2/phasetorch/util/_proc.py
+-rw-------   0 mohan3   (25677) mohan3   (25677)     2658 2023-04-29 19:43:30.000000 phasetorch-0.1.2/phasetorch/util/_projs.py
+-rw-------   0 mohan3   (25677) mohan3   (25677)     4806 2023-04-29 19:43:30.000000 phasetorch-0.1.2/phasetorch/util/_tutils.py
+-rw-------   0 mohan3   (25677) mohan3   (25677)     4657 2023-04-29 19:43:30.000000 phasetorch-0.1.2/phasetorch/util/_utils.py
+drwx------   0 mohan3   (25677) mohan3   (25677)        0 2023-05-08 14:41:34.454390 phasetorch-0.1.2/phasetorch.egg-info/
+-rw-------   0 mohan3   (25677) mohan3   (25677)     1095 2023-05-08 14:41:34.000000 phasetorch-0.1.2/phasetorch.egg-info/PKG-INFO
+-rw-------   0 mohan3   (25677) mohan3   (25677)     1213 2023-05-08 14:41:34.000000 phasetorch-0.1.2/phasetorch.egg-info/SOURCES.txt
+-rw-------   0 mohan3   (25677) mohan3   (25677)        1 2023-05-08 14:41:34.000000 phasetorch-0.1.2/phasetorch.egg-info/dependency_links.txt
+-rw-------   0 mohan3   (25677) mohan3   (25677)        1 2023-03-31 19:38:57.000000 phasetorch-0.1.2/phasetorch.egg-info/not-zip-safe
+-rw-------   0 mohan3   (25677) mohan3   (25677)       11 2023-05-08 14:41:34.000000 phasetorch-0.1.2/phasetorch.egg-info/top_level.txt
+-rw-------   0 mohan3   (25677) mohan3   (25677)       38 2023-05-08 14:41:34.492464 phasetorch-0.1.2/setup.cfg
+-rw-------   0 mohan3   (25677) mohan3   (25677)      843 2023-05-08 14:36:49.000000 phasetorch-0.1.2/setup.py
```

### Comparing `phasetorch-0.1.1/LICENSE` & `phasetorch-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `phasetorch-0.1.1/NOTICE` & `phasetorch-0.1.2/NOTICE`

 * *Files identical despite different names*

### Comparing `phasetorch-0.1.1/PKG-INFO` & `phasetorch-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 Metadata-Version: 2.1
 Name: phasetorch
-Version: 0.1.1
+Version: 0.1.2
 Summary: PhaseTorch is a Python package for phase retrieval in X-ray phase contrast computed tomography (XPCT).
 Home-page: https://github.com/phasetorch/phasetorch
-Author: K. Aditya Mohan
-Author-email: mohan3@llnl.gov
 License: GPL-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: NOTICE
```

### Comparing `phasetorch-0.1.1/README.rst` & `phasetorch-0.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `phasetorch-0.1.1/phasetorch/mono/_fresmod.py` & `phasetorch-0.1.2/phasetorch/mono/_fresmod.py`

 * *Files identical despite different names*

### Comparing `phasetorch-0.1.1/phasetorch/mono/_mullpr.py` & `phasetorch-0.1.2/phasetorch/mono/_mullpr.py`

 * *Files identical despite different names*

### Comparing `phasetorch-0.1.1/phasetorch/mono/_mulmod.py` & `phasetorch-0.1.2/phasetorch/mono/_mulmod.py`

 * *Files identical despite different names*

### Comparing `phasetorch-0.1.1/phasetorch/mono/_nonlpr.py` & `phasetorch-0.1.2/phasetorch/mono/_nonlpr.py`

 * *Files identical despite different names*

### Comparing `phasetorch-0.1.1/phasetorch/mono/_nonmod.py` & `phasetorch-0.1.2/phasetorch/mono/_nonmod.py`

 * *Files identical despite different names*

### Comparing `phasetorch-0.1.1/phasetorch/mono/_simtor.py` & `phasetorch-0.1.2/phasetorch/mono/_simtor.py`

 * *Files identical despite different names*

### Comparing `phasetorch-0.1.1/phasetorch/mono/_sinlpr.py` & `phasetorch-0.1.2/phasetorch/mono/_sinlpr.py`

 * *Files identical despite different names*

### Comparing `phasetorch-0.1.1/phasetorch/mono/_sinmod.py` & `phasetorch-0.1.2/phasetorch/mono/_sinmod.py`

 * *Files identical despite different names*

### Comparing `phasetorch-0.1.1/phasetorch/mono/eval.py` & `phasetorch-0.1.2/phasetorch/mono/eval.py`

 * *Files identical despite different names*

### Comparing `phasetorch-0.1.1/phasetorch/opt/_pytorch_lbfgs/functions/LBFGS.py` & `phasetorch-0.1.2/phasetorch/opt/_pytorch_lbfgs/functions/LBFGS.py`

 * *Files identical despite different names*

### Comparing `phasetorch-0.1.1/phasetorch/opt/_pytorch_lbfgs/functions/utils.py` & `phasetorch-0.1.2/phasetorch/opt/_pytorch_lbfgs/functions/utils.py`

 * *Files identical despite different names*

### Comparing `phasetorch-0.1.1/phasetorch/util/_check.py` & `phasetorch-0.1.2/phasetorch/util/_check.py`

 * *Files identical despite different names*

### Comparing `phasetorch-0.1.1/phasetorch/util/_pad.py` & `phasetorch-0.1.2/phasetorch/util/_pad.py`

 * *Files identical despite different names*

### Comparing `phasetorch-0.1.1/phasetorch/util/_proc.py` & `phasetorch-0.1.2/phasetorch/util/_proc.py`

 * *Files identical despite different names*

### Comparing `phasetorch-0.1.1/phasetorch/util/_projs.py` & `phasetorch-0.1.2/phasetorch/util/_projs.py`

 * *Files identical despite different names*

### Comparing `phasetorch-0.1.1/phasetorch/util/_tutils.py` & `phasetorch-0.1.2/phasetorch/util/_tutils.py`

 * *Files identical despite different names*

### Comparing `phasetorch-0.1.1/phasetorch/util/_utils.py` & `phasetorch-0.1.2/phasetorch/util/_utils.py`

 * *Files identical despite different names*

### Comparing `phasetorch-0.1.1/phasetorch.egg-info/PKG-INFO` & `phasetorch-0.1.2/phasetorch.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 Metadata-Version: 2.1
 Name: phasetorch
-Version: 0.1.1
+Version: 0.1.2
 Summary: PhaseTorch is a Python package for phase retrieval in X-ray phase contrast computed tomography (XPCT).
 Home-page: https://github.com/phasetorch/phasetorch
-Author: K. Aditya Mohan
-Author-email: mohan3@llnl.gov
 License: GPL-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: NOTICE
```

### Comparing `phasetorch-0.1.1/phasetorch.egg-info/SOURCES.txt` & `phasetorch-0.1.2/phasetorch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `phasetorch-0.1.1/setup.py` & `phasetorch-0.1.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 
 setup(name='phasetorch',
       version=version,
       description='PhaseTorch is a Python package for phase retrieval in X-ray phase contrast computed tomography (XPCT).',
       long_description=long_description,
       long_description_content_type="text/x-rst",
       url='https://github.com/phasetorch/phasetorch',
-      author='K. Aditya Mohan',
-      author_email='mohan3@llnl.gov',
       license='GPL-2.0',
       packages=find_packages(where="./"),
       package_dir={"": "./"},
       package_data={"phasetorch": ["./data/*.h5"]},
       setup_requires=[],
       install_requires=[],
       zip_safe=False,
```

