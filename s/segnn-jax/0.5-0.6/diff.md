# Comparing `tmp/segnn_jax-0.5.tar.gz` & `tmp/segnn_jax-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "segnn_jax-0.5.tar", last modified: Fri Mar 31 17:39:32 2023, max compression
+gzip compressed data, was "segnn_jax-0.6.tar", last modified: Mon May  8 09:44:50 2023, max compression
```

## Comparing `segnn_jax-0.5.tar` & `segnn_jax-0.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 17:39:32.105700 segnn_jax-0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-03-31 17:39:21.000000 segnn_jax-0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-03-31 17:39:32.105700 segnn_jax-0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-03-31 17:39:21.000000 segnn_jax-0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-03-31 17:39:21.000000 segnn_jax-0.5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 17:39:32.105700 segnn_jax-0.5/segnn_jax/
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-03-31 17:39:21.000000 segnn_jax-0.5/segnn_jax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11495 2023-03-31 17:39:21.000000 segnn_jax-0.5/segnn_jax/blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-03-31 17:39:21.000000 segnn_jax-0.5/segnn_jax/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-03-31 17:39:21.000000 segnn_jax-0.5/segnn_jax/graph_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-03-31 17:39:21.000000 segnn_jax-0.5/segnn_jax/irreps_computer.py
--rw-r--r--   0 runner    (1001) docker     (123)    10815 2023-03-31 17:39:21.000000 segnn_jax-0.5/segnn_jax/segnn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 17:39:32.105700 segnn_jax-0.5/segnn_jax.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-03-31 17:39:32.000000 segnn_jax-0.5/segnn_jax.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-03-31 17:39:32.000000 segnn_jax-0.5/segnn_jax.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 17:39:32.000000 segnn_jax-0.5/segnn_jax.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-31 17:39:32.000000 segnn_jax-0.5/segnn_jax.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-31 17:39:32.000000 segnn_jax-0.5/segnn_jax.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-03-31 17:39:32.109700 segnn_jax-0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-31 17:39:21.000000 segnn_jax-0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 17:39:32.105700 segnn_jax-0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-03-31 17:39:21.000000 segnn_jax-0.5/tests/test_blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-03-31 17:39:21.000000 segnn_jax-0.5/tests/test_segnn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:44:50.580514 segnn_jax-0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-08 09:44:42.000000 segnn_jax-0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-05-08 09:44:50.580514 segnn_jax-0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-05-08 09:44:42.000000 segnn_jax-0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-08 09:44:42.000000 segnn_jax-0.6/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:44:50.580514 segnn_jax-0.6/segnn_jax/
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-08 09:44:42.000000 segnn_jax-0.6/segnn_jax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9786 2023-05-08 09:44:42.000000 segnn_jax-0.6/segnn_jax/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-08 09:44:42.000000 segnn_jax-0.6/segnn_jax/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-05-08 09:44:42.000000 segnn_jax-0.6/segnn_jax/graph_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-05-08 09:44:42.000000 segnn_jax-0.6/segnn_jax/irreps_computer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9733 2023-05-08 09:44:42.000000 segnn_jax-0.6/segnn_jax/segnn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:44:50.580514 segnn_jax-0.6/segnn_jax.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-05-08 09:44:50.000000 segnn_jax-0.6/segnn_jax.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-08 09:44:50.000000 segnn_jax-0.6/segnn_jax.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 09:44:50.000000 segnn_jax-0.6/segnn_jax.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-08 09:44:50.000000 segnn_jax-0.6/segnn_jax.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-08 09:44:50.000000 segnn_jax-0.6/segnn_jax.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-08 09:44:50.580514 segnn_jax-0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-08 09:44:42.000000 segnn_jax-0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:44:50.580514 segnn_jax-0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-05-08 09:44:42.000000 segnn_jax-0.6/tests/test_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-05-08 09:44:42.000000 segnn_jax-0.6/tests/test_segnn.py
```

### Comparing `segnn_jax-0.5/LICENSE` & `segnn_jax-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `segnn_jax-0.5/PKG-INFO` & `segnn_jax-0.6/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: segnn_jax
-Version: 0.5
-Summary: Steerable E(3) GNN in jax
-Author: Gianluca Galletti
-Author-email: g.galletti@tum.de
-Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Steerable E(3) GNN in jax
 Reimplementation of [SEGNN](https://arxiv.org/abs/2110.02905) in jax. Original work by Johannes Brandstetter, Rob Hesselink, Elise van der Pol, Erik Bekkers and Max Welling.
 
 ## Why jax?
 **40-50% faster** inference and training compared to the [original torch implementation](https://github.com/RobDHess/Steerable-E3-GNN). Also JAX-MD.
 
 ## Installation
@@ -24,15 +13,15 @@
 ```
 python -m pip install -e .
 ```
 
 ### GPU support
 Upgrade `jax` to the gpu version
 ```
-pip install --upgrade "jax[cuda]==0.4.1" -f https://storage.googleapis.com/jax-releases/jax_cuda_releases.html
+pip install --upgrade "jax[cuda]==0.4.8" -f https://storage.googleapis.com/jax-releases/jax_cuda_releases.html
 ```
 
 ## Validation
 N-body (charged and gravity) and QM9 datasets are included for completeness from the original paper.
 
 ### Results
 Charged is on 5 bodies, gravity on 100 bodies. QM9 has graphs of variable sizes, so in jax samples are padded to the maximum size. Loss is MSE for Charged and Gravity and MAE for QM9.
@@ -64,34 +53,33 @@
     <td>.265</td>
     <td>60.55</td>
     <td>.264</td>
     <td>41.72</td>
   </tr>
   <tr>
     <td> <code>QM9 (alpha)</code> </td>
-    <td>.075*</td>
+    <td>.066*</td>
     <td>82.53</td>
-    <td>.098</td>
+    <td>.082</td>
     <td>105.98**</td>
   </tr>
 </table>
-* rerun
+* rerun on same conditions
 
 ** padded (naive)
 
 ### Validation install
 
 The experiments are only included in the github repo, so it needs to be cloned first.
 ```
 git clone https://github.com/gerkone/segnn-jax
 ```
 
 They are adapted from the original implementation, so additionally `torch` and `torch_geometric` are needed (cpu versions are enough).
 ```
-pip3 install torch==1.12.1 --extra-index-url https://download.pytorch.org/whl/cpu
 python -m pip install -r experiments/requirements.txt
 ```
 
 ### Datasets
 QM9 is automatically downloaded and processed when running the respective experiment.
 
 The N-body datasets have to be generated locally from the directory [experiments/nbody/data](experiments/nbody/data) (it will take some time, especially n-body `gravity`)
@@ -103,25 +91,25 @@
 ```
 python3 -u generate_dataset.py --simulation=gravity --n-balls=100
 ```
 
 ### Usage
 #### N-body (charged)
 ```
-python main.py --dataset=charged --epochs=200 --max-samples=3000 --lmax-hidden=1 --lmax-attributes=1 --layers=4 --units=64 --norm=none --batch-size=100 --lr=5e-3 --weight-decay=1e-12
+python validate.py --dataset=charged --epochs=200 --max-samples=3000 --lmax-hidden=1 --lmax-attributes=1 --layers=4 --units=64 --norm=none --batch-size=100 --lr=5e-3 --weight-decay=1e-12
 ```
 
 #### N-body (gravity)
 ```
-python main.py --dataset=gravity --epochs=100 --target=pos --max-samples=10000 --lmax-hidden=1 --lmax-attributes=1 --layers=4 --units=64 --norm=none --batch-size=100 --lr=5e-3 --weight-decay=1e-12 --neighbours=5 --n-bodies=100
+python validate.py --dataset=gravity --epochs=100 --target=pos --max-samples=10000 --lmax-hidden=1 --lmax-attributes=1 --layers=4 --units=64 --norm=none --batch-size=100 --lr=5e-3 --weight-decay=1e-12 --neighbours=5 --n-bodies=100
 ```
 
 #### QM9
 ```
-python main.py --dataset=qm9 --epochs=1000 --target=alpha --lmax-hidden=2 --lmax-attributes=3 --layers=7 --units=128 --norm=instance --batch-size=128 --lr=5e-4 --weight-decay=1e-8 --lr-scheduling
+python validate.py --dataset=qm9 --epochs=1000 --target=alpha --lmax-hidden=2 --lmax-attributes=3 --layers=7 --units=128 --norm=instance --batch-size=128 --lr=5e-4 --weight-decay=1e-8 --lr-scheduling
 ```
 
 (configurations used in validation)
 
 
 ## Acknowledgments
 - [e3nn_jax](https://github.com/e3nn/e3nn-jax) made this reimplementation possible.
```

#### html2text {}

```diff
@@ -1,49 +1,45 @@
-Metadata-Version: 2.1 Name: segnn_jax Version: 0.5 Summary: Steerable E(3) GNN
-in jax Author: Gianluca Galletti Author-email: g.galletti@tum.de Classifier:
-Programming Language :: Python :: 3.8 Requires-Python: >=3.8 Description-
-Content-Type: text/markdown License-File: LICENSE # Steerable E(3) GNN in jax
-Reimplementation of [SEGNN](https://arxiv.org/abs/2110.02905) in jax. Original
-work by Johannes Brandstetter, Rob Hesselink, Elise van der Pol, Erik Bekkers
-and Max Welling. ## Why jax? **40-50% faster** inference and training compared
-to the [original torch implementation](https://github.com/RobDHess/Steerable-
-E3-GNN). Also JAX-MD. ## Installation ``` python -m pip install segnn-jax ```
-Or clone this repository and build locally ``` python -m pip install -e . ```
-### GPU support Upgrade `jax` to the gpu version ``` pip install --upgrade "jax
-[cuda]==0.4.1" -f https://storage.googleapis.com/jax-releases/
-jax_cuda_releases.html ``` ## Validation N-body (charged and gravity) and QM9
-datasets are included for completeness from the original paper. ### Results
-Charged is on 5 bodies, gravity on 100 bodies. QM9 has graphs of variable
-sizes, so in jax samples are padded to the maximum size. Loss is MSE for
-Charged and Gravity and MAE for QM9. Times are remeasured on Quadro RTX 4000,
-__model only__ on batches of 100 graphs, in (global) single precision.
+# Steerable E(3) GNN in jax Reimplementation of [SEGNN](https://arxiv.org/abs/
+2110.02905) in jax. Original work by Johannes Brandstetter, Rob Hesselink,
+Elise van der Pol, Erik Bekkers and Max Welling. ## Why jax? **40-50% faster**
+inference and training compared to the [original torch implementation](https://
+github.com/RobDHess/Steerable-E3-GNN). Also JAX-MD. ## Installation ``` python
+-m pip install segnn-jax ``` Or clone this repository and build locally ```
+python -m pip install -e . ``` ### GPU support Upgrade `jax` to the gpu version
+``` pip install --upgrade "jax[cuda]==0.4.8" -f https://storage.googleapis.com/
+jax-releases/jax_cuda_releases.html ``` ## Validation N-body (charged and
+gravity) and QM9 datasets are included for completeness from the original
+paper. ### Results Charged is on 5 bodies, gravity on 100 bodies. QM9 has
+graphs of variable sizes, so in jax samples are padded to the maximum size.
+Loss is MSE for Charged and Gravity and MAE for QM9. Times are remeasured on
+Quadro RTX 4000, __model only__ on batches of 100 graphs, in (global) single
+precision.
                    torch (original)     jax (ours)
                    Loss  Inference [ms] Loss  Inference [ms]
 charged (position) .0043 21.22          .0045 4.47
 gravity (position) .265  60.55          .264  41.72
-QM9 (alpha)        .075* 82.53          .098  105.98**
-* rerun ** padded (naive) ### Validation install The experiments are only
-included in the github repo, so it needs to be cloned first. ``` git clone
-https://github.com/gerkone/segnn-jax ``` They are adapted from the original
-implementation, so additionally `torch` and `torch_geometric` are needed (cpu
-versions are enough). ``` pip3 install torch==1.12.1 --extra-index-url https://
-download.pytorch.org/whl/cpu python -m pip install -r experiments/
+QM9 (alpha)        .066* 82.53          .082  105.98**
+* rerun on same conditions ** padded (naive) ### Validation install The
+experiments are only included in the github repo, so it needs to be cloned
+first. ``` git clone https://github.com/gerkone/segnn-jax ``` They are adapted
+from the original implementation, so additionally `torch` and `torch_geometric`
+are needed (cpu versions are enough). ``` python -m pip install -r experiments/
 requirements.txt ``` ### Datasets QM9 is automatically downloaded and processed
 when running the respective experiment. The N-body datasets have to be
 generated locally from the directory [experiments/nbody/data](experiments/
 nbody/data) (it will take some time, especially n-body `gravity`) #### Charged
 dataset (5 bodies, 10000 training samples) ``` python3 -u generate_dataset.py -
 -simulation=charged ``` #### Gravity dataset (100 bodies, 10000 training
 samples) ``` python3 -u generate_dataset.py --simulation=gravity --n-balls=100
-``` ### Usage #### N-body (charged) ``` python main.py --dataset=charged --
+``` ### Usage #### N-body (charged) ``` python validate.py --dataset=charged --
 epochs=200 --max-samples=3000 --lmax-hidden=1 --lmax-attributes=1 --layers=4 --
 units=64 --norm=none --batch-size=100 --lr=5e-3 --weight-decay=1e-12 ``` ####
-N-body (gravity) ``` python main.py --dataset=gravity --epochs=100 --target=pos
---max-samples=10000 --lmax-hidden=1 --lmax-attributes=1 --layers=4 --units=64 -
--norm=none --batch-size=100 --lr=5e-3 --weight-decay=1e-12 --neighbours=5 --n-
-bodies=100 ``` #### QM9 ``` python main.py --dataset=qm9 --epochs=1000 --
-target=alpha --lmax-hidden=2 --lmax-attributes=3 --layers=7 --units=128 --
-norm=instance --batch-size=128 --lr=5e-4 --weight-decay=1e-8 --lr-scheduling
-``` (configurations used in validation) ## Acknowledgments - [e3nn_jax](https:/
-/github.com/e3nn/e3nn-jax) made this reimplementation possible. - [Artur
-Toshev](https://github.com/arturtoshev) and [Johannes Brandsetter](https://
-github.com/brandstetter-johannes), for support.
+N-body (gravity) ``` python validate.py --dataset=gravity --epochs=100 --
+target=pos --max-samples=10000 --lmax-hidden=1 --lmax-attributes=1 --layers=4 -
+-units=64 --norm=none --batch-size=100 --lr=5e-3 --weight-decay=1e-12 --
+neighbours=5 --n-bodies=100 ``` #### QM9 ``` python validate.py --dataset=qm9 -
+-epochs=1000 --target=alpha --lmax-hidden=2 --lmax-attributes=3 --layers=7 --
+units=128 --norm=instance --batch-size=128 --lr=5e-4 --weight-decay=1e-8 --lr-
+scheduling ``` (configurations used in validation) ## Acknowledgments -
+[e3nn_jax](https://github.com/e3nn/e3nn-jax) made this reimplementation
+possible. - [Artur Toshev](https://github.com/arturtoshev) and [Johannes
+Brandsetter](https://github.com/brandstetter-johannes), for support.
```

### Comparing `segnn_jax-0.5/README.md` & `segnn_jax-0.6/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: segnn_jax
+Version: 0.6
+Summary: Steerable E(3) GNN in jax
+Author: Gianluca Galletti
+Author-email: g.galletti@tum.de
+Classifier: Programming Language :: Python :: 3.8
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Steerable E(3) GNN in jax
 Reimplementation of [SEGNN](https://arxiv.org/abs/2110.02905) in jax. Original work by Johannes Brandstetter, Rob Hesselink, Elise van der Pol, Erik Bekkers and Max Welling.
 
 ## Why jax?
 **40-50% faster** inference and training compared to the [original torch implementation](https://github.com/RobDHess/Steerable-E3-GNN). Also JAX-MD.
 
 ## Installation
@@ -13,15 +24,15 @@
 ```
 python -m pip install -e .
 ```
 
 ### GPU support
 Upgrade `jax` to the gpu version
 ```
-pip install --upgrade "jax[cuda]==0.4.1" -f https://storage.googleapis.com/jax-releases/jax_cuda_releases.html
+pip install --upgrade "jax[cuda]==0.4.8" -f https://storage.googleapis.com/jax-releases/jax_cuda_releases.html
 ```
 
 ## Validation
 N-body (charged and gravity) and QM9 datasets are included for completeness from the original paper.
 
 ### Results
 Charged is on 5 bodies, gravity on 100 bodies. QM9 has graphs of variable sizes, so in jax samples are padded to the maximum size. Loss is MSE for Charged and Gravity and MAE for QM9.
@@ -53,34 +64,33 @@
     <td>.265</td>
     <td>60.55</td>
     <td>.264</td>
     <td>41.72</td>
   </tr>
   <tr>
     <td> <code>QM9 (alpha)</code> </td>
-    <td>.075*</td>
+    <td>.066*</td>
     <td>82.53</td>
-    <td>.098</td>
+    <td>.082</td>
     <td>105.98**</td>
   </tr>
 </table>
-* rerun
+* rerun on same conditions
 
 ** padded (naive)
 
 ### Validation install
 
 The experiments are only included in the github repo, so it needs to be cloned first.
 ```
 git clone https://github.com/gerkone/segnn-jax
 ```
 
 They are adapted from the original implementation, so additionally `torch` and `torch_geometric` are needed (cpu versions are enough).
 ```
-pip3 install torch==1.12.1 --extra-index-url https://download.pytorch.org/whl/cpu
 python -m pip install -r experiments/requirements.txt
 ```
 
 ### Datasets
 QM9 is automatically downloaded and processed when running the respective experiment.
 
 The N-body datasets have to be generated locally from the directory [experiments/nbody/data](experiments/nbody/data) (it will take some time, especially n-body `gravity`)
@@ -92,25 +102,25 @@
 ```
 python3 -u generate_dataset.py --simulation=gravity --n-balls=100
 ```
 
 ### Usage
 #### N-body (charged)
 ```
-python main.py --dataset=charged --epochs=200 --max-samples=3000 --lmax-hidden=1 --lmax-attributes=1 --layers=4 --units=64 --norm=none --batch-size=100 --lr=5e-3 --weight-decay=1e-12
+python validate.py --dataset=charged --epochs=200 --max-samples=3000 --lmax-hidden=1 --lmax-attributes=1 --layers=4 --units=64 --norm=none --batch-size=100 --lr=5e-3 --weight-decay=1e-12
 ```
 
 #### N-body (gravity)
 ```
-python main.py --dataset=gravity --epochs=100 --target=pos --max-samples=10000 --lmax-hidden=1 --lmax-attributes=1 --layers=4 --units=64 --norm=none --batch-size=100 --lr=5e-3 --weight-decay=1e-12 --neighbours=5 --n-bodies=100
+python validate.py --dataset=gravity --epochs=100 --target=pos --max-samples=10000 --lmax-hidden=1 --lmax-attributes=1 --layers=4 --units=64 --norm=none --batch-size=100 --lr=5e-3 --weight-decay=1e-12 --neighbours=5 --n-bodies=100
 ```
 
 #### QM9
 ```
-python main.py --dataset=qm9 --epochs=1000 --target=alpha --lmax-hidden=2 --lmax-attributes=3 --layers=7 --units=128 --norm=instance --batch-size=128 --lr=5e-4 --weight-decay=1e-8 --lr-scheduling
+python validate.py --dataset=qm9 --epochs=1000 --target=alpha --lmax-hidden=2 --lmax-attributes=3 --layers=7 --units=128 --norm=instance --batch-size=128 --lr=5e-4 --weight-decay=1e-8 --lr-scheduling
 ```
 
 (configurations used in validation)
 
 
 ## Acknowledgments
 - [e3nn_jax](https://github.com/e3nn/e3nn-jax) made this reimplementation possible.
```

#### html2text {}

```diff
@@ -1,46 +1,48 @@
-# Steerable E(3) GNN in jax Reimplementation of [SEGNN](https://arxiv.org/abs/
-2110.02905) in jax. Original work by Johannes Brandstetter, Rob Hesselink,
-Elise van der Pol, Erik Bekkers and Max Welling. ## Why jax? **40-50% faster**
-inference and training compared to the [original torch implementation](https://
-github.com/RobDHess/Steerable-E3-GNN). Also JAX-MD. ## Installation ``` python
--m pip install segnn-jax ``` Or clone this repository and build locally ```
-python -m pip install -e . ``` ### GPU support Upgrade `jax` to the gpu version
-``` pip install --upgrade "jax[cuda]==0.4.1" -f https://storage.googleapis.com/
-jax-releases/jax_cuda_releases.html ``` ## Validation N-body (charged and
-gravity) and QM9 datasets are included for completeness from the original
-paper. ### Results Charged is on 5 bodies, gravity on 100 bodies. QM9 has
-graphs of variable sizes, so in jax samples are padded to the maximum size.
-Loss is MSE for Charged and Gravity and MAE for QM9. Times are remeasured on
-Quadro RTX 4000, __model only__ on batches of 100 graphs, in (global) single
-precision.
+Metadata-Version: 2.1 Name: segnn_jax Version: 0.6 Summary: Steerable E(3) GNN
+in jax Author: Gianluca Galletti Author-email: g.galletti@tum.de Classifier:
+Programming Language :: Python :: 3.8 Requires-Python: >=3.8 Description-
+Content-Type: text/markdown License-File: LICENSE # Steerable E(3) GNN in jax
+Reimplementation of [SEGNN](https://arxiv.org/abs/2110.02905) in jax. Original
+work by Johannes Brandstetter, Rob Hesselink, Elise van der Pol, Erik Bekkers
+and Max Welling. ## Why jax? **40-50% faster** inference and training compared
+to the [original torch implementation](https://github.com/RobDHess/Steerable-
+E3-GNN). Also JAX-MD. ## Installation ``` python -m pip install segnn-jax ```
+Or clone this repository and build locally ``` python -m pip install -e . ```
+### GPU support Upgrade `jax` to the gpu version ``` pip install --upgrade "jax
+[cuda]==0.4.8" -f https://storage.googleapis.com/jax-releases/
+jax_cuda_releases.html ``` ## Validation N-body (charged and gravity) and QM9
+datasets are included for completeness from the original paper. ### Results
+Charged is on 5 bodies, gravity on 100 bodies. QM9 has graphs of variable
+sizes, so in jax samples are padded to the maximum size. Loss is MSE for
+Charged and Gravity and MAE for QM9. Times are remeasured on Quadro RTX 4000,
+__model only__ on batches of 100 graphs, in (global) single precision.
                    torch (original)     jax (ours)
                    Loss  Inference [ms] Loss  Inference [ms]
 charged (position) .0043 21.22          .0045 4.47
 gravity (position) .265  60.55          .264  41.72
-QM9 (alpha)        .075* 82.53          .098  105.98**
-* rerun ** padded (naive) ### Validation install The experiments are only
-included in the github repo, so it needs to be cloned first. ``` git clone
-https://github.com/gerkone/segnn-jax ``` They are adapted from the original
-implementation, so additionally `torch` and `torch_geometric` are needed (cpu
-versions are enough). ``` pip3 install torch==1.12.1 --extra-index-url https://
-download.pytorch.org/whl/cpu python -m pip install -r experiments/
+QM9 (alpha)        .066* 82.53          .082  105.98**
+* rerun on same conditions ** padded (naive) ### Validation install The
+experiments are only included in the github repo, so it needs to be cloned
+first. ``` git clone https://github.com/gerkone/segnn-jax ``` They are adapted
+from the original implementation, so additionally `torch` and `torch_geometric`
+are needed (cpu versions are enough). ``` python -m pip install -r experiments/
 requirements.txt ``` ### Datasets QM9 is automatically downloaded and processed
 when running the respective experiment. The N-body datasets have to be
 generated locally from the directory [experiments/nbody/data](experiments/
 nbody/data) (it will take some time, especially n-body `gravity`) #### Charged
 dataset (5 bodies, 10000 training samples) ``` python3 -u generate_dataset.py -
 -simulation=charged ``` #### Gravity dataset (100 bodies, 10000 training
 samples) ``` python3 -u generate_dataset.py --simulation=gravity --n-balls=100
-``` ### Usage #### N-body (charged) ``` python main.py --dataset=charged --
+``` ### Usage #### N-body (charged) ``` python validate.py --dataset=charged --
 epochs=200 --max-samples=3000 --lmax-hidden=1 --lmax-attributes=1 --layers=4 --
 units=64 --norm=none --batch-size=100 --lr=5e-3 --weight-decay=1e-12 ``` ####
-N-body (gravity) ``` python main.py --dataset=gravity --epochs=100 --target=pos
---max-samples=10000 --lmax-hidden=1 --lmax-attributes=1 --layers=4 --units=64 -
--norm=none --batch-size=100 --lr=5e-3 --weight-decay=1e-12 --neighbours=5 --n-
-bodies=100 ``` #### QM9 ``` python main.py --dataset=qm9 --epochs=1000 --
-target=alpha --lmax-hidden=2 --lmax-attributes=3 --layers=7 --units=128 --
-norm=instance --batch-size=128 --lr=5e-4 --weight-decay=1e-8 --lr-scheduling
-``` (configurations used in validation) ## Acknowledgments - [e3nn_jax](https:/
-/github.com/e3nn/e3nn-jax) made this reimplementation possible. - [Artur
-Toshev](https://github.com/arturtoshev) and [Johannes Brandsetter](https://
-github.com/brandstetter-johannes), for support.
+N-body (gravity) ``` python validate.py --dataset=gravity --epochs=100 --
+target=pos --max-samples=10000 --lmax-hidden=1 --lmax-attributes=1 --layers=4 -
+-units=64 --norm=none --batch-size=100 --lr=5e-3 --weight-decay=1e-12 --
+neighbours=5 --n-bodies=100 ``` #### QM9 ``` python validate.py --dataset=qm9 -
+-epochs=1000 --target=alpha --lmax-hidden=2 --lmax-attributes=3 --layers=7 --
+units=128 --norm=instance --batch-size=128 --lr=5e-4 --weight-decay=1e-8 --lr-
+scheduling ``` (configurations used in validation) ## Acknowledgments -
+[e3nn_jax](https://github.com/e3nn/e3nn-jax) made this reimplementation
+possible. - [Artur Toshev](https://github.com/arturtoshev) and [Johannes
+Brandsetter](https://github.com/brandstetter-johannes), for support.
```

### Comparing `segnn_jax-0.5/segnn_jax/blocks.py` & `segnn_jax-0.6/segnn_jax/blocks.py`

 * *Files 13% similar despite different names*

```diff
@@ -27,85 +27,70 @@
     )
 
 
 class O3TensorProduct(hk.Module):
     """
     O(3) equivariant linear parametrized tensor product layer.
 
-    Attributes:
-        left_irreps: Left input representation
-        right_irreps: Right input representation
-        output_irreps: Output representation
-        get_parameter: Haiku parameter getter and init function
-        tensor_product: Tensor product function
-        biases: Bias wrapper function
+    Functionally the same as O3TensorProductLegacy, but around 5-10% faster.
+    FullyConnectedTensorProduct seems faster than tensor_product + linear:
+    https://github.com/e3nn/e3nn-jax/releases/tag/0.14.0
     """
 
     def __init__(
         self,
         output_irreps: e3nn.Irreps,
         *,
-        left_irreps: e3nn.Irreps,
-        right_irreps: Optional[e3nn.Irreps] = None,
         biases: bool = True,
         name: Optional[str] = None,
         init_fn: Optional[InitFn] = None,
         gradient_normalization: Optional[Union[str, float]] = None,
         path_normalization: Optional[Union[str, float]] = None,
     ):
         """Initialize the tensor product.
 
         Args:
             output_irreps: Output representation
-            left_irreps: Left input representation
-            right_irreps: Right input representation (optional, defaults to 1x0e)
             biases: If set ot true will add biases
             name: Name of the linear layer params
             init_fn: Weight initialization function. Default is uniform.
             gradient_normalization: Gradient normalization method. Default is "path"
                 NOTE: gradient_normalization="element" is the default in torch and haiku.
             path_normalization: Path normalization method. Default is "element"
         """
         super().__init__(name)
 
-        if not right_irreps:
-            # NOTE: this is equivalent to a linear recombination of the left vectors
-            right_irreps = e3nn.Irreps("1x0e")
-
         if not isinstance(output_irreps, e3nn.Irreps):
             output_irreps = e3nn.Irreps(output_irreps)
-        if not isinstance(left_irreps, e3nn.Irreps):
-            left_irreps = e3nn.Irreps(left_irreps)
-        if not isinstance(right_irreps, e3nn.Irreps):
-            right_irreps = e3nn.Irreps(right_irreps)
-
         self.output_irreps = output_irreps
 
-        self.right_irreps = right_irreps
-        self.left_irreps = left_irreps
-
+        # tp weight init
         if not init_fn:
             init_fn = uniform_init
-
         self.get_parameter = init_fn
 
         if not gradient_normalization:
             gradient_normalization = config("gradient_normalization")
         if not path_normalization:
             path_normalization = config("path_normalization")
+        self._gradient_normalization = gradient_normalization
+        self._path_normalization = path_normalization
+
+        self.biases = biases and "0e" in self.output_irreps
 
-        # NOTE FunctionalFullyConnectedTensorProduct appears to be faster than combining
-        #  tensor_product+linear: https://github.com/e3nn/e3nn-jax/releases/tag/0.14.0
-        #  Implementation adapted from e3nn.haiku.FullyConnectedTensorProduct
+    def _build_tensor_product(
+        self, left_irreps: e3nn.Irreps, right_irreps: e3nn.Irreps
+    ) -> Callable:
+        """Build the tensor product function."""
         tp = e3nn.FunctionalFullyConnectedTensorProduct(
             left_irreps,
             right_irreps,
-            output_irreps,
-            gradient_normalization=gradient_normalization,
-            path_normalization=path_normalization,
+            self.output_irreps,
+            gradient_normalization=self._gradient_normalization,
+            path_normalization=self._path_normalization,
         )
         ws = [
             self.get_parameter(
                 name=(
                     f"w[{ins.i_in1},{ins.i_in2},{ins.i_out}] "
                     f"{tp.irreps_in1[ins.i_in1]},"
                     f"{tp.irreps_in2[ins.i_in2]},"
@@ -114,43 +99,40 @@
                 path_shape=ins.path_shape,
                 weight_std=ins.weight_std,
             )
             for ins in tp.instructions
         ]
 
         def tensor_product(x, y, **kwargs):
-            return tp.left_right(ws, x, y, **kwargs)._convert(output_irreps)
+            return tp.left_right(ws, x, y, **kwargs)._convert(self.output_irreps)
 
-        self.tensor_product = naive_broadcast_decorator(tensor_product)
-        self.biases = None
+        return naive_broadcast_decorator(tensor_product)
 
-        if biases and "0e" in self.output_irreps:
-            # add biases
-            b = [
-                self.get_parameter(
-                    f"b[{i_out}] {tp.irreps_out[i_out]}",
-                    path_shape=(mul_ir.dim,),
-                    weight_std=1 / jnp.sqrt(mul_ir.dim),
-                )
-                for i_out, mul_ir in enumerate(output_irreps)
-                if mul_ir.ir.is_scalar()
-            ]
-            b = e3nn.IrrepsArray(
-                f"{self.output_irreps.count('0e')}x0e", jnp.concatenate(b)
+    def _build_biases(self) -> Callable:
+        """Build the add bias function."""
+        b = [
+            self.get_parameter(
+                f"b[{i_out}] {self.output_irreps}",
+                path_shape=(mul_ir.dim,),
+                weight_std=1 / jnp.sqrt(mul_ir.dim),
             )
+            for i_out, mul_ir in enumerate(self.output_irreps)
+            if mul_ir.ir.is_scalar()
+        ]
+        b = e3nn.IrrepsArray(f"{self.output_irreps.count('0e')}x0e", jnp.concatenate(b))
 
-            # TODO: could be improved
-            def _wrapper(x: e3nn.IrrepsArray) -> e3nn.IrrepsArray:
-                scalars = x.filter("0e")
-                other = x.filter(drop="0e")
-                return e3nn.concatenate(
-                    [scalars + b.broadcast_to(scalars.shape), other], axis=1
-                )
+        # TODO: could be improved
+        def _wrapper(x: e3nn.IrrepsArray) -> e3nn.IrrepsArray:
+            scalars = x.filter("0e")
+            other = x.filter(drop="0e")
+            return e3nn.concatenate(
+                [scalars + b.broadcast_to(scalars.shape), other], axis=1
+            )
 
-            self.biases = _wrapper
+        return _wrapper
 
     def __call__(
         self, x: e3nn.IrrepsArray, y: Optional[e3nn.IrrepsArray] = None, **kwargs
     ) -> e3nn.IrrepsArray:
         """Applies an O(3) equivariant linear parametrized tensor product layer.
 
         Args:
@@ -158,44 +140,37 @@
             y (IrrepsArray): Right tensor. If None it defaults to np.ones.
 
         Returns:
             The output to the weighted tensor product (IrrepsArray).
         """
 
         if not y:
-            y = e3nn.IrrepsArray("1x0e", jnp.ones((1, 1)))
+            y = e3nn.IrrepsArray("1x0e", jnp.ones((1, 1), dtype=x.dtype))
 
         if x.irreps.lmax == 0 and y.irreps.lmax == 0 and self.output_irreps.lmax > 0:
             warnings.warn(
                 f"The specified output irreps ({self.output_irreps}) are not scalars "
                 "but both operands are. This can have undesired behaviour (NaN). Try "
                 "redistributing them into scalars or choose higher orders."
             )
 
-        assert (
-            x.irreps == self.left_irreps
-        ), f"Left irreps do not match. Got {x.irreps}, expected {self.left_irreps}"
-        assert (
-            y.irreps == self.right_irreps
-        ), f"Right irreps do not match. Got {y.irreps}, expected {self.right_irreps}"
-
-        output = self.tensor_product(x, y, **kwargs)
+        tp = self._build_tensor_product(x.irreps, y.irreps)
+        output = tp(x, y, **kwargs)
 
         if self.biases:
             # add biases
-            return self.biases(output)
+            bias_fn = self._build_biases()
+            return bias_fn(output)
 
         return output
 
 
 def O3TensorProductLegacy(
     output_irreps: e3nn.Irreps,
     *,
-    left_irreps: e3nn.Irreps,
-    right_irreps: Optional[e3nn.Irreps] = None,
     biases: bool = True,
     name: Optional[str] = None,
     init_fn: Optional[InitFn] = None,
     gradient_normalization: Optional[Union[str, float]] = "element",
     path_normalization: Optional[Union[str, float]] = None,
 ):
     """O(3) equivariant linear parametrized tensor product layer.
@@ -211,23 +186,16 @@
             NOTE: gradient_normalization="element" is the default in torch and haiku.
         path_normalization: Path normalization method. Default is "element"
 
     Returns:
         A function that returns the output to the weighted tensor product.
     """
 
-    if not right_irreps:
-        right_irreps = e3nn.Irreps("1x0e")
-
     if not isinstance(output_irreps, e3nn.Irreps):
         output_irreps = e3nn.Irreps(output_irreps)
-    if not isinstance(left_irreps, e3nn.Irreps):
-        left_irreps = e3nn.Irreps(left_irreps)
-    if not isinstance(right_irreps, e3nn.Irreps):
-        right_irreps = e3nn.Irreps(right_irreps)
 
     if not init_fn:
         init_fn = uniform_init
 
     linear = e3nn.haiku.Linear(
         output_irreps,
         get_parameter=init_fn,
@@ -247,45 +215,36 @@
             y (IrrepsArray): Right tensor. If None it defaults to np.ones.
 
         Returns:
             The output to the weighted tensor product (IrrepsArray).
         """
 
         if not y:
-            y = e3nn.IrrepsArray("1x0e", jnp.ones((1, 1)))
+            y = e3nn.IrrepsArray("1x0e", jnp.ones((1, 1), dtype=x.dtype))
 
         if x.irreps.lmax == 0 and y.irreps.lmax == 0 and output_irreps.lmax > 0:
             warnings.warn(
                 f"The specified output irreps ({output_irreps}) are not scalars "
                 "but both operands are. This can have undesired behaviour (NaN). Try "
                 "redistributing them into scalars or choose higher orders."
             )
 
-        assert (
-            x.irreps == left_irreps
-        ), f"Left irreps do not match. Got {x.irreps}, expected {left_irreps}"
-        assert (
-            y.irreps == right_irreps
-        ), f"Right irreps do not match. Got {y.irreps}, expected {right_irreps}"
-
         tp = e3nn.tensor_product(x, y)
 
         return linear(tp)
 
     return _tensor_product
 
 
 O3Layer = O3TensorProduct if config("o3_layer") == "new" else O3TensorProductLegacy
 
 
 def O3TensorProductGate(
     output_irreps: e3nn.Irreps,
     *,
-    left_irreps: e3nn.Irreps,
-    right_irreps: Optional[e3nn.Irreps] = None,
     biases: bool = True,
     scalar_activation: Optional[Callable] = None,
     gate_activation: Optional[Callable] = None,
     name: Optional[str] = None,
     init_fn: Optional[InitFn] = None,
 ) -> TensorProductFn:
     """Non-linear (gated) O(3) equivariant linear tensor product layer.
@@ -308,16 +267,14 @@
 
     # lift output with gating scalars
     gate_irreps = e3nn.Irreps(
         f"{output_irreps.num_irreps - output_irreps.count('0e')}x0e"
     )
     tensor_product = O3Layer(
         (gate_irreps + output_irreps).regroup(),
-        left_irreps=left_irreps,
-        right_irreps=right_irreps,
         biases=biases,
         name=name,
         init_fn=init_fn,
     )
     if not scalar_activation:
         scalar_activation = jax.nn.silu
     if not gate_activation:
```

### Comparing `segnn_jax-0.5/segnn_jax/graph_utils.py` & `segnn_jax-0.6/segnn_jax/graph_utils.py`

 * *Files identical despite different names*

### Comparing `segnn_jax-0.5/segnn_jax/irreps_computer.py` & `segnn_jax-0.6/segnn_jax/irreps_computer.py`

 * *Files identical despite different names*

### Comparing `segnn_jax-0.5/segnn_jax/segnn.py` & `segnn_jax-0.6/segnn_jax/segnn.py`

 * *Files 20% similar despite different names*

```diff
@@ -22,30 +22,25 @@
     Returns:
         Function to embed graph nodes (and optionally edges)
     """
 
     def _embedding(
         st_graph: SteerableGraphsTuple,
     ) -> SteerableGraphsTuple:
-        # TODO update
         graph = st_graph.graph
         nodes = O3Layer(
             embed_irreps,
-            left_irreps=graph.nodes.irreps,
-            right_irreps=st_graph.node_attributes.irreps,
             name="embedding_nodes",
         )(graph.nodes, st_graph.node_attributes)
         st_graph = st_graph._replace(graph=graph._replace(nodes=nodes))
 
         # NOTE edge embedding is not in the original paper but can get good results
         if embed_edges:
             additional_message_features = O3Layer(
                 embed_irreps,
-                left_irreps=graph.nodes.irreps,
-                right_irreps=st_graph.node_attributes.irreps,
                 name="embedding_msg_features",
             )(
                 st_graph.additional_message_features,
                 st_graph.edge_attributes,
             )
             st_graph = st_graph._replace(
                 additional_message_features=additional_message_features
@@ -78,55 +73,42 @@
     assert task in ["node", "graph"], f"Unknown task {task}"
     assert pool in ["avg", "sum", "none", None], f"Unknown pooling '{pool}'"
 
     def _decoder(st_graph: SteerableGraphsTuple):
         nodes = st_graph.graph.nodes
         # pre pool block
         for i in range(blocks):
-            nodes = O3TensorProductGate(
-                latent_irreps,
-                left_irreps=nodes.irreps,
-                right_irreps=st_graph.node_attributes.irreps,
-                name=f"prepool_{i}",
-            )(nodes, st_graph.node_attributes)
+            nodes = O3TensorProductGate(latent_irreps, name=f"prepool_{i}")(
+                nodes, st_graph.node_attributes
+            )
 
         if task == "node":
-            nodes = O3Layer(
-                output_irreps,
-                left_irreps=nodes.irreps,
-                right_irreps=st_graph.node_attributes.irreps,
-                name="output",
-            )(nodes, st_graph.node_attributes)
+            nodes = O3Layer(output_irreps, name="output")(
+                nodes, st_graph.node_attributes
+            )
 
         if task == "graph":
             # pool over graph
             pooled_irreps = (latent_irreps.num_irreps * output_irreps).regroup()
-            nodes = O3Layer(
-                pooled_irreps,
-                left_irreps=nodes.irreps,
-                right_irreps=st_graph.node_attributes.irreps,
-                name=f"prepool_{blocks}",
-            )(nodes, st_graph.node_attributes)
+            nodes = O3Layer(pooled_irreps, name=f"prepool_{blocks}")(
+                nodes, st_graph.node_attributes
+            )
 
             # pooling layer
             if pool == "avg":
                 pool_fn = jraph.segment_mean
             if pool == "sum":
                 pool_fn = jraph.segment_sum
 
             nodes = pooling(st_graph.graph._replace(nodes=nodes), aggregate_fn=pool_fn)
 
             # post pool mlp (not steerable)
             for i in range(blocks):
-                nodes = O3TensorProductGate(
-                    pooled_irreps, left_irreps=nodes.irreps, name=f"postpool_{i}"
-                )(nodes)
-            nodes = O3Layer(output_irreps, left_irreps=nodes.irreps, name="output")(
-                nodes
-            )
+                nodes = O3TensorProductGate(pooled_irreps, name=f"postpool_{i}")(nodes)
+            nodes = O3Layer(output_irreps, name="output")(nodes)
 
         return nodes
 
     return _decoder
 
 
 class SEGNNLayer(hk.Module):
@@ -175,20 +157,17 @@
         _ = edge_features
         # create messages
         msg = e3nn.concatenate([incoming, outgoing], axis=-1)
         if additional_message_features is not None:
             msg = e3nn.concatenate([msg, additional_message_features], axis=-1)
         # message mlp (phi_m in the paper) steered by edge attributeibutes
         for i in range(self._blocks):
-            msg = O3TensorProductGate(
-                self._output_irreps,
-                left_irreps=msg.irreps,
-                right_irreps=getattr(edge_attribute, "irreps", None),
-                name=f"tp_{i}",
-            )(msg, edge_attribute)
+            msg = O3TensorProductGate(self._output_irreps, name=f"tp_{i}")(
+                msg, edge_attribute
+            )
         # NOTE: original implementation only applied batch norm to messages
         if self._norm == "batch":
             msg = e3nn.haiku.BatchNorm(irreps=self._output_irreps)(msg)
         return msg
 
     def _update(
         self,
@@ -200,27 +179,21 @@
     ) -> e3nn.IrrepsArray:
         """Steerable equivariant update function."""
         _ = senders
         _ = globals_
         x = e3nn.concatenate([nodes, msg], axis=-1)
         # update mlp (phi_f in the paper) steered by node attributeibutes
         for i in range(self._blocks - 1):
-            x = O3TensorProductGate(
-                self._output_irreps,
-                left_irreps=x.irreps,
-                right_irreps=getattr(node_attribute, "irreps", None),
-                name=f"tp_{i}",
-            )(x, node_attribute)
+            x = O3TensorProductGate(self._output_irreps, name=f"tp_{i}")(
+                x, node_attribute
+            )
         # last update layer without activation
-        update = O3Layer(
-            self._output_irreps,
-            left_irreps=x.irreps,
-            right_irreps=getattr(node_attribute, "irreps", None),
-            name=f"tp_{self._blocks - 1}",
-        )(x, node_attribute)
+        update = O3Layer(self._output_irreps, name=f"tp_{self._blocks - 1}")(
+            x, node_attribute
+        )
         # residual connection
         nodes += update
         # message norm
         if self._norm in ["batch", "instance"]:
             nodes = e3nn.haiku.BatchNorm(
                 irreps=self._output_irreps,
                 instance=(self._norm == "instance"),
```

### Comparing `segnn_jax-0.5/segnn_jax.egg-info/PKG-INFO` & `segnn_jax-0.6/segnn_jax.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: segnn-jax
-Version: 0.5
+Version: 0.6
 Summary: Steerable E(3) GNN in jax
 Author: Gianluca Galletti
 Author-email: g.galletti@tum.de
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -24,15 +24,15 @@
 ```
 python -m pip install -e .
 ```
 
 ### GPU support
 Upgrade `jax` to the gpu version
 ```
-pip install --upgrade "jax[cuda]==0.4.1" -f https://storage.googleapis.com/jax-releases/jax_cuda_releases.html
+pip install --upgrade "jax[cuda]==0.4.8" -f https://storage.googleapis.com/jax-releases/jax_cuda_releases.html
 ```
 
 ## Validation
 N-body (charged and gravity) and QM9 datasets are included for completeness from the original paper.
 
 ### Results
 Charged is on 5 bodies, gravity on 100 bodies. QM9 has graphs of variable sizes, so in jax samples are padded to the maximum size. Loss is MSE for Charged and Gravity and MAE for QM9.
@@ -64,34 +64,33 @@
     <td>.265</td>
     <td>60.55</td>
     <td>.264</td>
     <td>41.72</td>
   </tr>
   <tr>
     <td> <code>QM9 (alpha)</code> </td>
-    <td>.075*</td>
+    <td>.066*</td>
     <td>82.53</td>
-    <td>.098</td>
+    <td>.082</td>
     <td>105.98**</td>
   </tr>
 </table>
-* rerun
+* rerun on same conditions
 
 ** padded (naive)
 
 ### Validation install
 
 The experiments are only included in the github repo, so it needs to be cloned first.
 ```
 git clone https://github.com/gerkone/segnn-jax
 ```
 
 They are adapted from the original implementation, so additionally `torch` and `torch_geometric` are needed (cpu versions are enough).
 ```
-pip3 install torch==1.12.1 --extra-index-url https://download.pytorch.org/whl/cpu
 python -m pip install -r experiments/requirements.txt
 ```
 
 ### Datasets
 QM9 is automatically downloaded and processed when running the respective experiment.
 
 The N-body datasets have to be generated locally from the directory [experiments/nbody/data](experiments/nbody/data) (it will take some time, especially n-body `gravity`)
@@ -103,25 +102,25 @@
 ```
 python3 -u generate_dataset.py --simulation=gravity --n-balls=100
 ```
 
 ### Usage
 #### N-body (charged)
 ```
-python main.py --dataset=charged --epochs=200 --max-samples=3000 --lmax-hidden=1 --lmax-attributes=1 --layers=4 --units=64 --norm=none --batch-size=100 --lr=5e-3 --weight-decay=1e-12
+python validate.py --dataset=charged --epochs=200 --max-samples=3000 --lmax-hidden=1 --lmax-attributes=1 --layers=4 --units=64 --norm=none --batch-size=100 --lr=5e-3 --weight-decay=1e-12
 ```
 
 #### N-body (gravity)
 ```
-python main.py --dataset=gravity --epochs=100 --target=pos --max-samples=10000 --lmax-hidden=1 --lmax-attributes=1 --layers=4 --units=64 --norm=none --batch-size=100 --lr=5e-3 --weight-decay=1e-12 --neighbours=5 --n-bodies=100
+python validate.py --dataset=gravity --epochs=100 --target=pos --max-samples=10000 --lmax-hidden=1 --lmax-attributes=1 --layers=4 --units=64 --norm=none --batch-size=100 --lr=5e-3 --weight-decay=1e-12 --neighbours=5 --n-bodies=100
 ```
 
 #### QM9
 ```
-python main.py --dataset=qm9 --epochs=1000 --target=alpha --lmax-hidden=2 --lmax-attributes=3 --layers=7 --units=128 --norm=instance --batch-size=128 --lr=5e-4 --weight-decay=1e-8 --lr-scheduling
+python validate.py --dataset=qm9 --epochs=1000 --target=alpha --lmax-hidden=2 --lmax-attributes=3 --layers=7 --units=128 --norm=instance --batch-size=128 --lr=5e-4 --weight-decay=1e-8 --lr-scheduling
 ```
 
 (configurations used in validation)
 
 
 ## Acknowledgments
 - [e3nn_jax](https://github.com/e3nn/e3nn-jax) made this reimplementation possible.
```

#### html2text {}

```diff
@@ -1,49 +1,48 @@
-Metadata-Version: 2.1 Name: segnn-jax Version: 0.5 Summary: Steerable E(3) GNN
+Metadata-Version: 2.1 Name: segnn-jax Version: 0.6 Summary: Steerable E(3) GNN
 in jax Author: Gianluca Galletti Author-email: g.galletti@tum.de Classifier:
 Programming Language :: Python :: 3.8 Requires-Python: >=3.8 Description-
 Content-Type: text/markdown License-File: LICENSE # Steerable E(3) GNN in jax
 Reimplementation of [SEGNN](https://arxiv.org/abs/2110.02905) in jax. Original
 work by Johannes Brandstetter, Rob Hesselink, Elise van der Pol, Erik Bekkers
 and Max Welling. ## Why jax? **40-50% faster** inference and training compared
 to the [original torch implementation](https://github.com/RobDHess/Steerable-
 E3-GNN). Also JAX-MD. ## Installation ``` python -m pip install segnn-jax ```
 Or clone this repository and build locally ``` python -m pip install -e . ```
 ### GPU support Upgrade `jax` to the gpu version ``` pip install --upgrade "jax
-[cuda]==0.4.1" -f https://storage.googleapis.com/jax-releases/
+[cuda]==0.4.8" -f https://storage.googleapis.com/jax-releases/
 jax_cuda_releases.html ``` ## Validation N-body (charged and gravity) and QM9
 datasets are included for completeness from the original paper. ### Results
 Charged is on 5 bodies, gravity on 100 bodies. QM9 has graphs of variable
 sizes, so in jax samples are padded to the maximum size. Loss is MSE for
 Charged and Gravity and MAE for QM9. Times are remeasured on Quadro RTX 4000,
 __model only__ on batches of 100 graphs, in (global) single precision.
                    torch (original)     jax (ours)
                    Loss  Inference [ms] Loss  Inference [ms]
 charged (position) .0043 21.22          .0045 4.47
 gravity (position) .265  60.55          .264  41.72
-QM9 (alpha)        .075* 82.53          .098  105.98**
-* rerun ** padded (naive) ### Validation install The experiments are only
-included in the github repo, so it needs to be cloned first. ``` git clone
-https://github.com/gerkone/segnn-jax ``` They are adapted from the original
-implementation, so additionally `torch` and `torch_geometric` are needed (cpu
-versions are enough). ``` pip3 install torch==1.12.1 --extra-index-url https://
-download.pytorch.org/whl/cpu python -m pip install -r experiments/
+QM9 (alpha)        .066* 82.53          .082  105.98**
+* rerun on same conditions ** padded (naive) ### Validation install The
+experiments are only included in the github repo, so it needs to be cloned
+first. ``` git clone https://github.com/gerkone/segnn-jax ``` They are adapted
+from the original implementation, so additionally `torch` and `torch_geometric`
+are needed (cpu versions are enough). ``` python -m pip install -r experiments/
 requirements.txt ``` ### Datasets QM9 is automatically downloaded and processed
 when running the respective experiment. The N-body datasets have to be
 generated locally from the directory [experiments/nbody/data](experiments/
 nbody/data) (it will take some time, especially n-body `gravity`) #### Charged
 dataset (5 bodies, 10000 training samples) ``` python3 -u generate_dataset.py -
 -simulation=charged ``` #### Gravity dataset (100 bodies, 10000 training
 samples) ``` python3 -u generate_dataset.py --simulation=gravity --n-balls=100
-``` ### Usage #### N-body (charged) ``` python main.py --dataset=charged --
+``` ### Usage #### N-body (charged) ``` python validate.py --dataset=charged --
 epochs=200 --max-samples=3000 --lmax-hidden=1 --lmax-attributes=1 --layers=4 --
 units=64 --norm=none --batch-size=100 --lr=5e-3 --weight-decay=1e-12 ``` ####
-N-body (gravity) ``` python main.py --dataset=gravity --epochs=100 --target=pos
---max-samples=10000 --lmax-hidden=1 --lmax-attributes=1 --layers=4 --units=64 -
--norm=none --batch-size=100 --lr=5e-3 --weight-decay=1e-12 --neighbours=5 --n-
-bodies=100 ``` #### QM9 ``` python main.py --dataset=qm9 --epochs=1000 --
-target=alpha --lmax-hidden=2 --lmax-attributes=3 --layers=7 --units=128 --
-norm=instance --batch-size=128 --lr=5e-4 --weight-decay=1e-8 --lr-scheduling
-``` (configurations used in validation) ## Acknowledgments - [e3nn_jax](https:/
-/github.com/e3nn/e3nn-jax) made this reimplementation possible. - [Artur
-Toshev](https://github.com/arturtoshev) and [Johannes Brandsetter](https://
-github.com/brandstetter-johannes), for support.
+N-body (gravity) ``` python validate.py --dataset=gravity --epochs=100 --
+target=pos --max-samples=10000 --lmax-hidden=1 --lmax-attributes=1 --layers=4 -
+-units=64 --norm=none --batch-size=100 --lr=5e-3 --weight-decay=1e-12 --
+neighbours=5 --n-bodies=100 ``` #### QM9 ``` python validate.py --dataset=qm9 -
+-epochs=1000 --target=alpha --lmax-hidden=2 --lmax-attributes=3 --layers=7 --
+units=128 --norm=instance --batch-size=128 --lr=5e-4 --weight-decay=1e-8 --lr-
+scheduling ``` (configurations used in validation) ## Acknowledgments -
+[e3nn_jax](https://github.com/e3nn/e3nn-jax) made this reimplementation
+possible. - [Artur Toshev](https://github.com/arturtoshev) and [Johannes
+Brandsetter](https://github.com/brandstetter-johannes), for support.
```

### Comparing `segnn_jax-0.5/setup.cfg` & `segnn_jax-0.6/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 	Programming Language :: Python :: 3.8
 
 [options]
 packages = segnn_jax
 python_requires = >=3.8
 install_requires = 
 	dm_haiku==0.0.9
-	e3nn_jax==0.17.0
-	jax==0.4.1
-	jaxlib==0.4.1
+	e3nn_jax==0.17.4
+	jax==0.4.8
+	jaxlib==0.4.8
 	jraph==0.0.6.dev0
 	numpy>=1.23.4
 	optax==0.1.3
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `segnn_jax-0.5/tests/test_blocks.py` & `segnn_jax-0.6/tests/test_blocks.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,17 +4,15 @@
 from e3nn_jax.util import assert_equivariant
 
 from segnn_jax import O3TensorProduct, O3TensorProductGate, O3TensorProductLegacy
 
 
 @pytest.mark.parametrize("biases", [False, True])
 def test_linear(key, biases):
-    f = lambda x1, x2: O3TensorProduct(
-        "1x1o", left_irreps="1x1o", right_irreps="1x1o", biases=biases
-    )(x1, x2)
+    f = lambda x1, x2: O3TensorProduct("1x1o", biases=biases)(x1, x2)
     f = hk.without_apply_rng(hk.transform(f))
 
     v = e3nn.normal("1x1o", key, (5,))
     params = f.init(key, v, v)
 
     wrapper = lambda x1, x2: f.apply(params, x1, x2)
 
@@ -27,17 +25,15 @@
 
 @pytest.mark.parametrize("biases", [False, True])
 def test_gated(key, biases):
     import segnn_jax.blocks
 
     segnn_jax.blocks.O3Layer = segnn_jax.blocks.O3TensorProduct
 
-    f = lambda x1, x2: O3TensorProductGate(
-        "1x1o", left_irreps="1x1o", right_irreps="1x1o", biases=biases
-    )(x1, x2)
+    f = lambda x1, x2: O3TensorProductGate("1x1o", biases=biases)(x1, x2)
     f = hk.without_apply_rng(hk.transform(f))
 
     v = e3nn.normal("1x1o", key, (5,))
     params = f.init(key, v, v)
 
     wrapper = lambda x1, x2: f.apply(params, x1, x2)
 
@@ -46,17 +42,15 @@
         key,
         args_in=(e3nn.normal("1x1o", key, (5,)), e3nn.normal("1x1o", key, (5,))),
     )
 
 
 @pytest.mark.parametrize("biases", [False, True])
 def test_linear_legacy(key, biases):
-    f = lambda x1, x2: O3TensorProductLegacy(
-        "1x1o", left_irreps="1x1o", right_irreps="1x1o", biases=biases
-    )(x1, x2)
+    f = lambda x1, x2: O3TensorProductLegacy("1x1o", biases=biases)(x1, x2)
     f = hk.without_apply_rng(hk.transform(f))
 
     v = e3nn.normal("1x1o", key, (5,))
     params = f.init(key, v, v)
 
     wrapper = lambda x1, x2: f.apply(params, x1, x2)
```

### Comparing `segnn_jax-0.5/tests/test_segnn.py` & `segnn_jax-0.6/tests/test_segnn.py`

 * *Files identical despite different names*

