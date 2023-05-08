# Comparing `tmp/forust-0.2.4.tar.gz` & `tmp/forust-0.2.5.tar.gz`

## Comparing `forust-0.2.4.tar` & `forust-0.2.5.tar`

### file list

```diff
@@ -1,41 +1,42 @@
--rw-r--r--   0        0        0      745 1970-01-01 00:00:00.000000 forust-0.2.4/local_dependencies/forust-ml/Cargo.toml
--rw-r--r--   0      501       20     5608 2023-05-06 22:11:27.000000 forust-0.2.4/local_dependencies/forust-ml/.github/workflows/CI.yml
--rw-r--r--   0      501       20      262 2023-05-06 22:11:27.000000 forust-0.2.4/local_dependencies/forust-ml/.gitignore
--rw-r--r--   0      501       20      320 2023-05-06 22:11:27.000000 forust-0.2.4/local_dependencies/forust-ml/.pre-commit-config.yaml
--rw-r--r--   0      501       20    11341 2023-05-06 22:11:27.000000 forust-0.2.4/local_dependencies/forust-ml/LICENSE
--rw-r--r--   0      501       20    11917 2023-05-06 22:11:27.000000 forust-0.2.4/local_dependencies/forust-ml/README.md
--rw-r--r--   0      501       20     4100 2023-05-06 22:11:27.000000 forust-0.2.4/local_dependencies/forust-ml/benches/forust_benchmarks.rs
--rw-r--r--   0      501       20   416799 2023-05-06 22:15:57.000000 forust-0.2.4/local_dependencies/forust-ml/dist/forust-0.2.4-cp310-cp310-macosx_10_7_x86_64.whl
--rw-r--r--   0      501       20   751559 2023-05-06 22:14:53.000000 forust-0.2.4/local_dependencies/forust-ml/dist/forust-0.2.4.tar.gz
--rw-r--r--   0      501       20    16121 2023-05-06 22:11:27.000000 forust-0.2.4/local_dependencies/forust-ml/resources/pdp_plot_age.png
--rw-r--r--   0      501       20    10758 2023-05-06 22:11:27.000000 forust-0.2.4/local_dependencies/forust-ml/resources/pdp_plot_age_mono.png
--rw-r--r--   0      501       20    57018 2023-05-06 22:11:27.000000 forust-0.2.4/local_dependencies/forust-ml/resources/titanic.csv
--rw-r--r--   0      501       20   655700 2023-05-06 22:11:27.000000 forust-0.2.4/local_dependencies/forust-ml/resources/tree-image-crop.png
--rw-r--r--   0      501       20     2556 2023-05-06 22:11:27.000000 forust-0.2.4/local_dependencies/forust-ml/rs-example.md
--rw-r--r--   0      501       20     1179 2023-05-06 22:11:27.000000 forust-0.2.4/local_dependencies/forust-ml/scripts/make_resources.py
--rw-r--r--   0      501       20       53 2023-05-06 22:11:27.000000 forust-0.2.4/local_dependencies/forust-ml/scripts/run-python-tests.ps1
--rw-r--r--   0      501       20       53 2023-05-06 22:11:27.000000 forust-0.2.4/local_dependencies/forust-ml/scripts/run-python-tests.sh
--rw-r--r--   0      501       20     5610 2023-05-06 22:11:27.000000 forust-0.2.4/local_dependencies/forust-ml/src/binning.rs
--rw-r--r--   0      501       20      248 2023-05-06 22:11:27.000000 forust-0.2.4/local_dependencies/forust-ml/src/constraints.rs
--rw-r--r--   0      501       20     8384 2023-05-06 22:11:27.000000 forust-0.2.4/local_dependencies/forust-ml/src/data.rs
--rw-r--r--   0      501       20      585 2023-05-06 22:11:27.000000 forust-0.2.4/local_dependencies/forust-ml/src/errors.rs
--rw-r--r--   0      501       20    24537 2023-05-06 22:11:27.000000 forust-0.2.4/local_dependencies/forust-ml/src/gradientbooster.rs
--rw-r--r--   0      501       20     9357 2023-05-06 22:11:27.000000 forust-0.2.4/local_dependencies/forust-ml/src/histogram.rs
--rw-r--r--   0      501       20      318 2023-05-06 22:11:27.000000 forust-0.2.4/local_dependencies/forust-ml/src/lib.rs
--rw-r--r--   0      501       20     6060 2023-05-06 22:11:27.000000 forust-0.2.4/local_dependencies/forust-ml/src/node.rs
--rw-r--r--   0      501       20     4125 2023-05-06 22:11:27.000000 forust-0.2.4/local_dependencies/forust-ml/src/objective.rs
--rw-r--r--   0      501       20     4054 2023-05-06 22:11:27.000000 forust-0.2.4/local_dependencies/forust-ml/src/partial_dependence.rs
--rw-r--r--   0      501       20    34423 2023-05-06 22:11:27.000000 forust-0.2.4/local_dependencies/forust-ml/src/splitter.rs
--rw-r--r--   0      501       20    17831 2023-05-06 22:11:27.000000 forust-0.2.4/local_dependencies/forust-ml/src/tree.rs
--rw-r--r--   0      501       20    29472 2023-05-06 22:11:27.000000 forust-0.2.4/local_dependencies/forust-ml/src/utils.rs
--rw-r--r--   0        0        0      391 1970-01-01 00:00:00.000000 forust-0.2.4/Cargo.toml
--rw-r--r--   0      501       20      685 2023-05-06 22:11:27.000000 forust-0.2.4/.gitignore
--rw-r--r--   0      501       20    11917 2023-05-06 22:12:03.000000 forust-0.2.4/README.md
--rw-r--r--   0      501       20    18185 2023-05-06 22:11:27.000000 forust-0.2.4/forust/__init__.py
--rw-r--r--   0      501       20      785 2023-05-06 22:11:27.000000 forust-0.2.4/pyproject.toml
--rw-r--r--   0      501       20     7353 2023-05-06 22:11:27.000000 forust-0.2.4/scratch.py
--rw-r--r--   0      501       20     9433 2023-05-06 22:11:27.000000 forust-0.2.4/src/lib.rs
--rw-r--r--   0      501       20    12380 2023-05-06 22:11:27.000000 forust-0.2.4/tests/test_booster.py
--rw-r--r--   0      501       20    11341 2023-05-06 22:12:03.000000 forust-0.2.4/LICENSE
--rw-r--r--   0      501       20    11917 2023-05-06 22:12:03.000000 forust-0.2.4/README.md
--rw-r--r--   0        0        0    12701 1970-01-01 00:00:00.000000 forust-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0      745 1970-01-01 00:00:00.000000 forust-0.2.5/local_dependencies/forust-ml/Cargo.toml
+-rw-r--r--   0     1001      123     5608 2023-05-08 01:09:39.000000 forust-0.2.5/local_dependencies/forust-ml/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123      262 2023-05-08 01:09:39.000000 forust-0.2.5/local_dependencies/forust-ml/.gitignore
+-rw-r--r--   0     1001      123      320 2023-05-08 01:09:39.000000 forust-0.2.5/local_dependencies/forust-ml/.pre-commit-config.yaml
+-rw-r--r--   0     1001      123    11341 2023-05-08 01:09:39.000000 forust-0.2.5/local_dependencies/forust-ml/LICENSE
+-rw-r--r--   0     1001      123    12305 2023-05-08 01:09:39.000000 forust-0.2.5/local_dependencies/forust-ml/README.md
+-rw-r--r--   0     1001      123     4100 2023-05-08 01:09:39.000000 forust-0.2.5/local_dependencies/forust-ml/benches/forust_benchmarks.rs
+-rw-r--r--   0     1001      123   466303 2023-05-08 01:14:21.000000 forust-0.2.5/local_dependencies/forust-ml/dist/forust-0.2.5-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl
+-rw-r--r--   0     1001      123   753297 2023-05-08 01:13:37.000000 forust-0.2.5/local_dependencies/forust-ml/dist/forust-0.2.5.tar.gz
+-rw-r--r--   0     1001      123    16121 2023-05-08 01:09:39.000000 forust-0.2.5/local_dependencies/forust-ml/resources/pdp_plot_age.png
+-rw-r--r--   0     1001      123    10758 2023-05-08 01:09:39.000000 forust-0.2.5/local_dependencies/forust-ml/resources/pdp_plot_age_mono.png
+-rw-r--r--   0     1001      123    57018 2023-05-08 01:09:39.000000 forust-0.2.5/local_dependencies/forust-ml/resources/titanic.csv
+-rw-r--r--   0     1001      123   655700 2023-05-08 01:09:39.000000 forust-0.2.5/local_dependencies/forust-ml/resources/tree-image-crop.png
+-rw-r--r--   0     1001      123     2556 2023-05-08 01:09:39.000000 forust-0.2.5/local_dependencies/forust-ml/rs-example.md
+-rwxr-xr-x   0     1001      123     1137 2023-05-08 01:14:30.000000 forust-0.2.5/local_dependencies/forust-ml/run-maturin-action.sh
+-rw-r--r--   0     1001      123     1179 2023-05-08 01:09:39.000000 forust-0.2.5/local_dependencies/forust-ml/scripts/make_resources.py
+-rw-r--r--   0     1001      123       53 2023-05-08 01:09:39.000000 forust-0.2.5/local_dependencies/forust-ml/scripts/run-python-tests.ps1
+-rw-r--r--   0     1001      123       53 2023-05-08 01:09:39.000000 forust-0.2.5/local_dependencies/forust-ml/scripts/run-python-tests.sh
+-rw-r--r--   0     1001      123     5610 2023-05-08 01:09:39.000000 forust-0.2.5/local_dependencies/forust-ml/src/binning.rs
+-rw-r--r--   0     1001      123      248 2023-05-08 01:09:39.000000 forust-0.2.5/local_dependencies/forust-ml/src/constraints.rs
+-rw-r--r--   0     1001      123     8384 2023-05-08 01:09:39.000000 forust-0.2.5/local_dependencies/forust-ml/src/data.rs
+-rw-r--r--   0     1001      123      585 2023-05-08 01:09:39.000000 forust-0.2.5/local_dependencies/forust-ml/src/errors.rs
+-rw-r--r--   0     1001      123    26609 2023-05-08 01:09:39.000000 forust-0.2.5/local_dependencies/forust-ml/src/gradientbooster.rs
+-rw-r--r--   0     1001      123     9357 2023-05-08 01:09:39.000000 forust-0.2.5/local_dependencies/forust-ml/src/histogram.rs
+-rw-r--r--   0     1001      123      318 2023-05-08 01:09:39.000000 forust-0.2.5/local_dependencies/forust-ml/src/lib.rs
+-rw-r--r--   0     1001      123     6060 2023-05-08 01:09:39.000000 forust-0.2.5/local_dependencies/forust-ml/src/node.rs
+-rw-r--r--   0     1001      123     4125 2023-05-08 01:09:39.000000 forust-0.2.5/local_dependencies/forust-ml/src/objective.rs
+-rw-r--r--   0     1001      123     4054 2023-05-08 01:09:39.000000 forust-0.2.5/local_dependencies/forust-ml/src/partial_dependence.rs
+-rw-r--r--   0     1001      123    34685 2023-05-08 01:09:39.000000 forust-0.2.5/local_dependencies/forust-ml/src/splitter.rs
+-rw-r--r--   0     1001      123    21765 2023-05-08 01:09:39.000000 forust-0.2.5/local_dependencies/forust-ml/src/tree.rs
+-rw-r--r--   0     1001      123    29472 2023-05-08 01:09:39.000000 forust-0.2.5/local_dependencies/forust-ml/src/utils.rs
+-rw-r--r--   0        0        0      391 1970-01-01 00:00:00.000000 forust-0.2.5/Cargo.toml
+-rw-r--r--   0     1001      123      685 2023-05-08 01:09:39.000000 forust-0.2.5/.gitignore
+-rw-r--r--   0     1001      123    12305 2023-05-08 01:10:06.000000 forust-0.2.5/README.md
+-rw-r--r--   0     1001      123    18941 2023-05-08 01:09:39.000000 forust-0.2.5/forust/__init__.py
+-rw-r--r--   0     1001      123      785 2023-05-08 01:09:39.000000 forust-0.2.5/pyproject.toml
+-rw-r--r--   0     1001      123     7353 2023-05-08 01:09:39.000000 forust-0.2.5/scratch.py
+-rw-r--r--   0     1001      123     9818 2023-05-08 01:09:39.000000 forust-0.2.5/src/lib.rs
+-rw-r--r--   0     1001      123    12380 2023-05-08 01:09:39.000000 forust-0.2.5/tests/test_booster.py
+-rw-r--r--   0     1001      123    11341 2023-05-08 01:10:06.000000 forust-0.2.5/LICENSE
+-rw-r--r--   0     1001      123    12305 2023-05-08 01:10:06.000000 forust-0.2.5/README.md
+-rw-r--r--   0        0        0    13089 1970-01-01 00:00:00.000000 forust-0.2.5/PKG-INFO
```

### Comparing `forust-0.2.4/local_dependencies/forust-ml/Cargo.toml` & `forust-0.2.5/local_dependencies/forust-ml/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "forust-ml"
-version = "0.2.4"
+version = "0.2.5"
 edition = "2021"
 authors = ["James Inlow <james.d.inlow@gmail.com>"]
 homepage = "https://github.com/jinlow/forust"
 description = "A lightweight gradient boosting implementation in Rust."
 license-file = "LICENSE"
 readme = "README.md"
 repository = "https://github.com/jinlow/forust"
```

### Comparing `forust-0.2.4/local_dependencies/forust-ml/.github/workflows/CI.yml` & `forust-0.2.5/local_dependencies/forust-ml/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `forust-0.2.4/local_dependencies/forust-ml/LICENSE` & `forust-0.2.5/local_dependencies/forust-ml/LICENSE`

 * *Files identical despite different names*

### Comparing `forust-0.2.4/local_dependencies/forust-ml/README.md` & `forust-0.2.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,28 @@
+Metadata-Version: 2.1
+Name: forust
+Version: 0.2.5
+Classifier: Programming Language :: Rust
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Requires-Dist: numpy>=1.21
+Requires-Dist: pandas>=1.3
+Requires-Dist: maturin; extra == 'dev'
+Requires-Dist: pytest; extra == 'dev'
+Requires-Dist: seaborn; extra == 'dev'
+Requires-Dist: xgboost==1.6.1; extra == 'dev'
+Requires-Dist: scikit-learn; extra == 'dev'
+Provides-Extra: dev
+License-File: LICENSE
+Summary: A lightweight gradient boosting implementation in Rust.
+Keywords: rust,forust,machine learning,xgboost,tree model,decision tree
+Author: James Inlow
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
+
 <p align="center">
   <img  height="340" src="https://github.com/jinlow/forust/raw/main/resources/tree-image-crop.png">
 </p>
 
 
 <div align="center">
 
@@ -22,15 +43,15 @@
 The package can be installed directly from [pypi](https://pypi.org/project/forust/).
 ```shell
 pip install forust
 ```
 
 To use in a rust project add the following to your Cargo.toml file.
 ```toml
-forust-ml = "0.2.4"
+forust-ml = "0.2.5"
 ```
 
 ## Usage
 The `GradientBooster` class is currently the only public facing class in the package, and can be used to train gradient boosted decision tree ensembles with multiple objective functions.
 
 It can be initialized with the following arguments.
 
@@ -98,33 +119,25 @@
 #       [ 1.05406709,  0.08825999,  0.21662544, -0.12083538,  0.35209258,
 #        -1.07720813],
 ```
 
 The `fit` method accepts the following arguments.
  - `X` ***(FrameLike)***: Either a pandas DataFrame, or a 2 dimensional numpy array, with numeric data.
  - `y` ***(ArrayLike)***: Either a pandas Series, or a 1 dimensional numpy array. If "LogLoss" was
-   the objective type specified, then this should only contain 1 or 0 values, where 1 is the positive class being predicted. If "SquaredLoss" is the objective type, then any continuous variable can be
-   provided.
- - `sample_weight` ***(Optional[ArrayLike], optional)***: Instance weights to use when
-    training the model. If None is passed, a weight of 1 will be used for every record.
-    Defaults to None.
+   the objective type specified, then this should only contain 1 or 0 values, where 1 is the positive class being predicted. If "SquaredLoss" is the objective type, then any continuous variable can be provided.
+ - `sample_weight` ***(Optional[ArrayLike], optional)***: Instance weights to use when training the model. If None is passed, a weight of 1 will be used for every record. Defaults to None.
 
 The predict method accepts the following arguments.
  - `X` ***(FrameLike)***: Either a pandas DataFrame, or a 2 dimensional numpy array, with numeric data.
- - `parallel` ***(Optional[bool], optional)***: Optionally specify if the predict
-   function should run in parallel on multiple threads. If `None` is
-   passed, the `parallel` attribute of the booster will be used.
-   Defaults to `None`.
+ - `parallel` ***(Optional[bool], optional)***: Optionally specify if the predict function should run in parallel on multiple threads. If `None` is passed, the `parallel` attribute of the booster will be used. Defaults to `None`.
 
 The `predict_contributions` method will predict with the fitted booster on new data, returning the feature contribution matrix. The last column is the bias term.
  - `X` ***(FrameLike)***: Either a pandas DataFrame, or a 2 dimensional numpy array, with numeric data.
- - `parallel` ***(Optional[bool], optional)***: Optionally specify if the predict
-   function should run in parallel on multiple threads. If `None` is
-   passed, the `parallel` attribute of the booster will be used.
-   Defaults to `None`.
+ - `method` ***(str, optional)***: Method to calculate the contributions, if "average" is specified, the average internal node values are calculated, this is equivalent to the `approx_contribs` parameter in XGBoost. The other supported method is "weight", this will use the internal leaf weights, to calculate the contributions. This is the same as what is described by Saabas [here](https://blog.datadive.net/interpreting-random-forests/).
+ - `parallel` ***(Optional[bool], optional)***: Optionally specify if the predict function should run in parallel on multiple threads. If `None` is passed, the `parallel` attribute of the booster will be used. Defaults to `None`.
 
 ### Inspecting the Model
 
 Once the booster has been fit, each individual tree structure can be retrieved in text form, using the `text_dump` method. This method returns a list, the same length as the number of trees in the model.
 
 ```python
 model.text_dump()[0]
@@ -138,20 +151,16 @@
 
 The `json_dump` method performs the same action, but returns the model as a json representation rather than a text string.
 
 To see an estimate for how a given feature is used in the model, the `partial_dependence` method is provided. This method calculates the partial dependence values of a feature. For each unique value of the feature, this gives the estimate of the predicted value for that feature, with the effects of all features averaged out. This information gives an estimate of how a given feature impacts the model.
 
 The `partial_dependence` method takes the following parameters...
 
- - `X` ***(FrameLike)***: Either a pandas DataFrame, or a 2 dimensional numpy array.
-      This should be the same data passed into the models fit, or predict,
-      with the columns in the same order.
- - `feature` ***(Union[str, int])***: The feature for which to calculate the partial
-      dependence values. This can be the name of a column, if the provided
-      X is a pandas DataFrame, or the index of the feature.
+ - `X` ***(FrameLike)***: Either a pandas DataFrame, or a 2 dimensional numpy array. This should be the same data passed into the models fit, or predict, with the columns in the same order.
+ - `feature` ***(Union[str, int])***: The feature for which to calculate the partial dependence values. This can be the name of a column, if the provided X is a pandas DataFrame, or the index of the feature.
 
 This method returns a 2 dimensional numpy array, where the first column is the sorted unique values of the feature, and then the second column is the partial dependence values for each feature value.
 
 This information can be plotted to visualize how a feature is used in the model, like so.
 
 ```python
 from seaborn import lineplot
@@ -191,7 +200,8 @@
 
 ```python
 trained_model.save_booster("model_path.json")
 
 # To load a model from a json path.
 loaded_model = GradientBooster.load_model("model_path.json")
 ```
+
```

#### html2text {}

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1 Name: forust Version: 0.2.5 Classifier: Programming
+Language :: Rust Classifier: Programming Language :: Python :: Implementation
+:: CPython Classifier: Programming Language :: Python :: Implementation :: PyPy
+Requires-Dist: numpy>=1.21 Requires-Dist: pandas>=1.3 Requires-Dist: maturin;
+extra == 'dev' Requires-Dist: pytest; extra == 'dev' Requires-Dist: seaborn;
+extra == 'dev' Requires-Dist: xgboost==1.6.1; extra == 'dev' Requires-Dist:
+scikit-learn; extra == 'dev' Provides-Extra: dev License-File: LICENSE Summary:
+A lightweight gradient boosting implementation in Rust. Keywords:
+rust,forust,machine learning,xgboost,tree model,decision tree Author: James
+Inlow Requires-Python: >=3.8 Description-Content-Type: text/markdown;
+charset=UTF-8; variant=GFM
    [https://github.com/jinlow/forust/raw/main/resources/tree-image-crop.png]
  ![PyPI](https://img.shields.io/pypi/v/forust?color=gr&style=for-the-badge) !
  [Crates.io](https://img.shields.io/crates/v/forust-ml?color=gr&style=for-the-
                                     badge)
 # Forust ## _A lightweight gradient boosting package_ Forust, is a lightweight
 package for building gradient boosted decision tree ensembles. All of the
 algorithm code is written in [Rust](https://www.rust-lang.org/), with a python
@@ -13,15 +24,15 @@
 understand the XGBoost algorithm, additionally to have a fun project to work on
 in rust, and because I wanted to be able to experiment with adding new features
 to the algorithm in a smaller simpler codebase. All of the rust code for the
 package can be found in the [src](src/) directory, while all of the python
 wrapper code is in the [py-forust](py-forust/) directory. ## Installation The
 package can be installed directly from [pypi](https://pypi.org/project/forust/
 ). ```shell pip install forust ``` To use in a rust project add the following
-to your Cargo.toml file. ```toml forust-ml = "0.2.4" ``` ## Usage The
+to your Cargo.toml file. ```toml forust-ml = "0.2.5" ``` ## Usage The
 `GradientBooster` class is currently the only public facing class in the
 package, and can be used to train gradient boosted decision tree ensembles with
 multiple objective functions. It can be initialized with the following
 arguments. - `objective_type` ***(str, optional)***: The name of objective
 function used to optimize. Valid options include "LogLoss" to use logistic loss
 as the objective function (binary classification), or "SquaredLoss" to use
 Squared Error as the objective function (continuous regression). Defaults to
@@ -99,21 +110,27 @@
 Either a pandas DataFrame, or a 2 dimensional numpy array, with numeric data. -
 `parallel` ***(Optional[bool], optional)***: Optionally specify if the predict
 function should run in parallel on multiple threads. If `None` is passed, the
 `parallel` attribute of the booster will be used. Defaults to `None`. The
 `predict_contributions` method will predict with the fitted booster on new
 data, returning the feature contribution matrix. The last column is the bias
 term. - `X` ***(FrameLike)***: Either a pandas DataFrame, or a 2 dimensional
-numpy array, with numeric data. - `parallel` ***(Optional[bool], optional)***:
-Optionally specify if the predict function should run in parallel on multiple
-threads. If `None` is passed, the `parallel` attribute of the booster will be
-used. Defaults to `None`. ### Inspecting the Model Once the booster has been
-fit, each individual tree structure can be retrieved in text form, using the
-`text_dump` method. This method returns a list, the same length as the number
-of trees in the model. ```python model.text_dump()[0] # 0:[0 < 3]
+numpy array, with numeric data. - `method` ***(str, optional)***: Method to
+calculate the contributions, if "average" is specified, the average internal
+node values are calculated, this is equivalent to the `approx_contribs`
+parameter in XGBoost. The other supported method is "weight", this will use the
+internal leaf weights, to calculate the contributions. This is the same as what
+is described by Saabas [here](https://blog.datadive.net/interpreting-random-
+forests/). - `parallel` ***(Optional[bool], optional)***: Optionally specify if
+the predict function should run in parallel on multiple threads. If `None` is
+passed, the `parallel` attribute of the booster will be used. Defaults to
+`None`. ### Inspecting the Model Once the booster has been fit, each individual
+tree structure can be retrieved in text form, using the `text_dump` method.
+This method returns a list, the same length as the number of trees in the
+model. ```python model.text_dump()[0] # 0:[0 < 3]
 yes=1,no=2,missing=2,gain=91.50833,cover=209.388307 # 1:[4 < 13.7917]
 yes=3,no=4,missing=4,gain=28.185467,cover=94.00148 # 3:[1 < 18]
 yes=7,no=8,missing=8,gain=1.4576768,cover=22.090348 # 7:[1 < 17]
 yes=15,no=16,missing=16,gain=0.691266,cover=0.705011 # 15:leaf=-
 0.15120,cover=0.23500 # 16:leaf=0.154097,cover=0.470007 ``` The `json_dump`
 method performs the same action, but returns the model as a json representation
 rather than a text string. To see an estimate for how a given feature is used
```

### Comparing `forust-0.2.4/local_dependencies/forust-ml/benches/forust_benchmarks.rs` & `forust-0.2.5/local_dependencies/forust-ml/benches/forust_benchmarks.rs`

 * *Files identical despite different names*

### Comparing `forust-0.2.4/local_dependencies/forust-ml/resources/pdp_plot_age.png` & `forust-0.2.5/local_dependencies/forust-ml/resources/pdp_plot_age.png`

 * *Files identical despite different names*

### Comparing `forust-0.2.4/local_dependencies/forust-ml/resources/pdp_plot_age_mono.png` & `forust-0.2.5/local_dependencies/forust-ml/resources/pdp_plot_age_mono.png`

 * *Files identical despite different names*

### Comparing `forust-0.2.4/local_dependencies/forust-ml/resources/titanic.csv` & `forust-0.2.5/local_dependencies/forust-ml/resources/titanic.csv`

 * *Files identical despite different names*

### Comparing `forust-0.2.4/local_dependencies/forust-ml/resources/tree-image-crop.png` & `forust-0.2.5/local_dependencies/forust-ml/resources/tree-image-crop.png`

 * *Files identical despite different names*

### Comparing `forust-0.2.4/local_dependencies/forust-ml/rs-example.md` & `forust-0.2.5/local_dependencies/forust-ml/rs-example.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ## A Complete Rust Example
 
 To run this example, add the following code to your `Cargo.toml` file.
 ```toml
 [dependencies]
-forust-ml = "0.2.4"
+forust-ml = "0.2.5"
 polars = "0.24"
 reqwest = { version = "0.11", features = ["blocking"] }
 ```
 
 The following is a runable example using `polars` for data processing. The actual data manipulation can be performed with any tool, the only vital part, is the data be in column major format.
 ```rust
 use forust_ml::{GradientBooster, Matrix};
```

### Comparing `forust-0.2.4/local_dependencies/forust-ml/scripts/make_resources.py` & `forust-0.2.5/local_dependencies/forust-ml/scripts/make_resources.py`

 * *Files identical despite different names*

### Comparing `forust-0.2.4/local_dependencies/forust-ml/src/binning.rs` & `forust-0.2.5/local_dependencies/forust-ml/src/binning.rs`

 * *Files identical despite different names*

### Comparing `forust-0.2.4/local_dependencies/forust-ml/src/data.rs` & `forust-0.2.5/local_dependencies/forust-ml/src/data.rs`

 * *Files identical despite different names*

### Comparing `forust-0.2.4/local_dependencies/forust-ml/src/errors.rs` & `forust-0.2.5/local_dependencies/forust-ml/src/errors.rs`

 * *Files identical despite different names*

### Comparing `forust-0.2.4/local_dependencies/forust-ml/src/gradientbooster.rs` & `forust-0.2.5/local_dependencies/forust-ml/src/gradientbooster.rs`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,20 @@
 use crate::tree::Tree;
 use rand::rngs::StdRng;
 use rand::SeedableRng;
 use rayon::prelude::*;
 use serde::{Deserialize, Deserializer, Serialize};
 use std::collections::HashMap;
 use std::fs;
+
+pub enum ContributionsMethod {
+    Weight,
+    Average,
+}
+
 /// Gradient Booster object
 ///
 /// * `objective_type` - The name of objective function used to optimize.
 ///   Valid options include "LogLoss" to use logistic loss as the objective function,
 ///   or "SquaredLoss" to use Squared Error as the objective function.
 /// * `iterations` - Total number of trees to train in the ensemble.
 /// * `learning_rate` - Step size to use at each iteration. Each
@@ -302,18 +308,71 @@
     //                 *p += t.predict_row_from_row_slice(&pred_row);
     //             }
     //         });
     //     }
     //     init_preds
     // }
 
+    pub fn predict_contributions(
+        &self,
+        data: &Matrix<f64>,
+        method: ContributionsMethod,
+        parallel: bool,
+    ) -> Vec<f64> {
+        match method {
+            ContributionsMethod::Average => self.predict_contributions_average(data, parallel),
+            ContributionsMethod::Weight => self.predict_contributions_weight(data, parallel),
+        }
+    }
+
+    fn predict_contributions_weight(&self, data: &Matrix<f64>, parallel: bool) -> Vec<f64> {
+        let mut contribs = vec![0.; (data.cols + 1) * data.rows];
+
+        // Add the bias term to every bias value...
+        let bias_idx = data.cols + 1;
+        contribs
+            .iter_mut()
+            .skip(bias_idx - 1)
+            .step_by(bias_idx)
+            .for_each(|v| *v += self.base_score);
+
+        // Clean this up..
+        // materializing a row, and then passing that to all of the
+        // trees seems to be the fastest approach (5X faster), we should test
+        // something like this for normal predictions.
+        if parallel {
+            data.index
+                .par_iter()
+                .zip(contribs.par_chunks_mut(data.cols + 1))
+                .for_each(|(row, c)| {
+                    let r_ = data.get_row(*row);
+                    self.trees.iter().for_each(|t| {
+                        t.predict_contributions_row_weight(&r_, c, &self.missing);
+                    });
+                });
+        } else {
+            data.index
+                .iter()
+                .zip(contribs.chunks_mut(data.cols + 1))
+                .for_each(|(row, c)| {
+                    let r_ = data.get_row(*row);
+                    self.trees.iter().for_each(|t| {
+                        t.predict_contributions_row_weight(&r_, c, &self.missing);
+                    });
+                });
+        }
+
+        contribs
+    }
+
     /// Generate predictions on data using the gradient booster.
+    /// This is equivalent to the XGBoost predict contributions with approx_contribs
     ///
     /// * `data` -  Either a pandas DataFrame, or a 2 dimensional numpy array.
-    pub fn predict_contributions(&self, data: &Matrix<f64>, parallel: bool) -> Vec<f64> {
+    fn predict_contributions_average(&self, data: &Matrix<f64>, parallel: bool) -> Vec<f64> {
         let weights: Vec<Vec<f64>> = if parallel {
             self.trees
                 .par_iter()
                 .map(|t| t.distribute_leaf_weights())
                 .collect()
         } else {
             self.trees
@@ -338,25 +397,25 @@
         if parallel {
             data.index
                 .par_iter()
                 .zip(contribs.par_chunks_mut(data.cols + 1))
                 .for_each(|(row, c)| {
                     let r_ = data.get_row(*row);
                     self.trees.iter().zip(weights.iter()).for_each(|(t, w)| {
-                        t.predict_contributions_row(&r_, c, w, &self.missing);
+                        t.predict_contributions_row_average(&r_, c, w, &self.missing);
                     });
                 });
         } else {
             data.index
                 .iter()
                 .zip(contribs.chunks_mut(data.cols + 1))
                 .for_each(|(row, c)| {
                     let r_ = data.get_row(*row);
                     self.trees.iter().zip(weights.iter()).for_each(|(t, w)| {
-                        t.predict_contributions_row(&r_, c, w, &self.missing);
+                        t.predict_contributions_row_average(&r_, c, w, &self.missing);
                     });
                 });
         }
 
         contribs
     }
 
@@ -566,15 +625,15 @@
         booster.iterations = 10;
         booster.nbins = 300;
         booster.max_depth = 3;
         booster.subsample = 0.5;
         let sample_weight = vec![1.; y.len()];
         booster.fit(&data, &y, &sample_weight).unwrap();
         let preds = booster.predict(&data, false);
-        let contribs = booster.predict_contributions(&data, false);
+        let contribs = booster.predict_contributions(&data, ContributionsMethod::Average, false);
         assert_eq!(contribs.len(), (data.cols + 1) * data.rows);
         println!("{}", booster.trees[0]);
         println!("{}", booster.trees[0].nodes.len());
         println!("{}", booster.trees.last().unwrap().nodes.len());
         println!("{:?}", &preds[0..10]);
     }
 
@@ -595,15 +654,15 @@
         let mut booster = GradientBooster::default();
         booster.iterations = 10;
         booster.nbins = 300;
         booster.max_depth = 3;
         let sample_weight = vec![1.; y.len()];
         booster.fit(&data, &y, &sample_weight).unwrap();
         let preds = booster.predict(&data, false);
-        let contribs = booster.predict_contributions(&data, false);
+        let contribs = booster.predict_contributions(&data, ContributionsMethod::Average, false);
         assert_eq!(contribs.len(), (data.cols + 1) * data.rows);
         println!("{}", booster.trees[0]);
         println!("{}", booster.trees[0].nodes.len());
         println!("{}", booster.trees.last().unwrap().nodes.len());
         println!("{:?}", &preds[0..10]);
     }
```

### Comparing `forust-0.2.4/local_dependencies/forust-ml/src/histogram.rs` & `forust-0.2.5/local_dependencies/forust-ml/src/histogram.rs`

 * *Files identical despite different names*

### Comparing `forust-0.2.4/local_dependencies/forust-ml/src/node.rs` & `forust-0.2.5/local_dependencies/forust-ml/src/node.rs`

 * *Files identical despite different names*

### Comparing `forust-0.2.4/local_dependencies/forust-ml/src/objective.rs` & `forust-0.2.5/local_dependencies/forust-ml/src/objective.rs`

 * *Files identical despite different names*

### Comparing `forust-0.2.4/local_dependencies/forust-ml/src/partial_dependence.rs` & `forust-0.2.5/local_dependencies/forust-ml/src/partial_dependence.rs`

 * *Files identical despite different names*

### Comparing `forust-0.2.4/local_dependencies/forust-ml/src/splitter.rs` & `forust-0.2.5/local_dependencies/forust-ml/src/splitter.rs`

 * *Files 1% similar despite different names*

```diff
@@ -372,19 +372,24 @@
         parallel: bool,
     ) -> Vec<SplittableNode> {
         let missing_child = *n_nodes;
         let left_child = missing_child + 1;
         let right_child = missing_child + 2;
         node.update_children(missing_child, left_child, right_child, &split_info);
 
-        let (missing_is_leaf, missing_info) = match split_info.missing_node {
+        let (missing_is_leaf, mut missing_info) = match split_info.missing_node {
             MissingInfo::Branch(i) => (false, i),
             MissingInfo::Leaf(i) => (true, i),
             _ => unreachable!(),
         };
+        // Set missing weight to parent weight value...
+        // This essentially neutralizes missing.
+        // Manually calculating it, was leading to some small numeric
+        // rounding differences...
+        missing_info.weight = node.weight_value;
 
         // We need to move all of the index's above and below our
         // split value.
         // pivot the sub array that this node has on our split value
         // Missing all falls to the bottom.
         let (mut missing_split_idx, mut split_idx) = pivot_on_split_exclude_missing(
             &mut index[node.start_idx..node.stop_idx],
@@ -866,15 +871,14 @@
         let d = vec![4., 2., 3., 4., 5., 1., 4.];
         let data = Matrix::new(&d, 7, 1);
         let y = vec![0., 0., 0., 1., 1., 0., 1.];
         let yhat = vec![0.; 7];
         let w = vec![1.; y.len()];
         let grad = LogLoss::calc_grad(&y, &yhat, &w);
         let hess = LogLoss::calc_hess(&y, &yhat, &w);
-
         let b = bin_matrix(&data, &w, 10, f64::NAN).unwrap();
         let bdata = Matrix::new(&b.binned_data, data.rows, data.cols);
         let index = data.index.to_owned();
         let hists = HistogramMatrix::new(&bdata, &b.cuts, &grad, &hess, &index, true, true);
         let splitter = MissingImputerSplitter {
             l2: 0.0,
             gamma: 0.0,
```

### Comparing `forust-0.2.4/local_dependencies/forust-ml/src/tree.rs` & `forust-0.2.5/local_dependencies/forust-ml/src/tree.rs`

 * *Files 10% similar despite different names*

```diff
@@ -145,15 +145,85 @@
                     if !n.is_missing_leaf {
                         growable.push_front(n)
                     }
                 }
             }
         }
     }
-    pub fn predict_contributions_row(
+
+    pub fn predict_contributions_row_weight(
+        &self,
+        row: &[f64],
+        contribs: &mut [f64],
+        missing: &f64,
+    ) {
+        // Add the bias term first...
+        contribs[contribs.len() - 1] += self.nodes[0].weight_value as f64;
+        let mut node_idx = 0;
+        loop {
+            let node = &self.nodes[node_idx];
+            if node.is_leaf {
+                break;
+            }
+            // Get change of weight given child's weight.
+            let child_idx = node.get_child_idx(&row[node.split_feature], missing);
+            let node_weight = self.nodes[node_idx].weight_value as f64;
+            let child_weight = self.nodes[child_idx].weight_value as f64;
+            let delta = child_weight - node_weight;
+            contribs[node.split_feature] += delta;
+            node_idx = child_idx
+        }
+    }
+
+    fn predict_contributions_single_threaded_weight(
+        &self,
+        data: &Matrix<f64>,
+        contribs: &mut [f64],
+        missing: &f64,
+    ) {
+        // There needs to always be at least 2 trees
+        data.index
+            .iter()
+            .zip(contribs.chunks_mut(data.cols + 1))
+            .for_each(|(row, contribs)| {
+                self.predict_contributions_row_weight(&data.get_row(*row), contribs, missing)
+            })
+    }
+
+    fn predict_contributions_parallel_weight(
+        &self,
+        data: &Matrix<f64>,
+        contribs: &mut [f64],
+        missing: &f64,
+    ) {
+        // There needs to always be at least 2 trees
+        data.index
+            .par_iter()
+            .zip(contribs.par_chunks_mut(data.cols + 1))
+            .for_each(|(row, contribs)| {
+                self.predict_contributions_row_weight(&data.get_row(*row), contribs, missing)
+            })
+    }
+
+    pub fn predict_contributions_weight(
+        &self,
+        data: &Matrix<f64>,
+        contribs: &mut [f64],
+        parallel: bool,
+        missing: &f64,
+    ) {
+        if parallel {
+            self.predict_contributions_parallel_weight(data, contribs, missing)
+        } else {
+            self.predict_contributions_single_threaded_weight(data, contribs, missing)
+        }
+    }
+
+    /// This is the method that XGBoost uses.
+    pub fn predict_contributions_row_average(
         &self,
         row: &[f64],
         contribs: &mut [f64],
         weights: &[f64],
         missing: &f64,
     ) {
         // Add the bias term first...
@@ -170,58 +240,68 @@
             let child_weight = weights[child_idx];
             let delta = child_weight - node_weight;
             contribs[node.split_feature] += delta;
             node_idx = child_idx
         }
     }
 
-    fn predict_contributions_single_threaded(
+    fn predict_contributions_single_threaded_average(
         &self,
         data: &Matrix<f64>,
         contribs: &mut [f64],
         weights: &[f64],
         missing: &f64,
     ) {
         // There needs to always be at least 2 trees
         data.index
             .iter()
             .zip(contribs.chunks_mut(data.cols + 1))
             .for_each(|(row, contribs)| {
-                self.predict_contributions_row(&data.get_row(*row), contribs, weights, missing)
+                self.predict_contributions_row_average(
+                    &data.get_row(*row),
+                    contribs,
+                    weights,
+                    missing,
+                )
             })
     }
 
-    fn predict_contributions_parallel(
+    fn predict_contributions_parallel_average(
         &self,
         data: &Matrix<f64>,
         contribs: &mut [f64],
         weights: &[f64],
         missing: &f64,
     ) {
         // There needs to always be at least 2 trees
         data.index
             .par_iter()
             .zip(contribs.par_chunks_mut(data.cols + 1))
             .for_each(|(row, contribs)| {
-                self.predict_contributions_row(&data.get_row(*row), contribs, weights, missing)
+                self.predict_contributions_row_average(
+                    &data.get_row(*row),
+                    contribs,
+                    weights,
+                    missing,
+                )
             })
     }
 
-    pub fn predict_contributions(
+    pub fn predict_contributions_average(
         &self,
         data: &Matrix<f64>,
         contribs: &mut [f64],
         weights: &[f64],
         parallel: bool,
         missing: &f64,
     ) {
         if parallel {
-            self.predict_contributions_parallel(data, contribs, weights, missing)
+            self.predict_contributions_parallel_average(data, contribs, weights, missing)
         } else {
-            self.predict_contributions_single_threaded(data, contribs, weights, missing)
+            self.predict_contributions_single_threaded_average(data, contribs, weights, missing)
         }
     }
 
     fn predict_row(&self, data: &Matrix<f64>, row: usize, missing: &f64) -> f64 {
         let mut node_idx = 0;
         loop {
             let node = &self.nodes[node_idx];
@@ -418,15 +498,33 @@
         // println!("{}", tree);
         // let preds = tree.predict(&data, false);
         // println!("{:?}", &preds[0..10]);
         assert_eq!(25, tree.nodes.len());
         // Test contributions prediction...
         let weights = tree.distribute_leaf_weights();
         let mut contribs = vec![0.; (data.cols + 1) * data.rows];
-        tree.predict_contributions(&data, &mut contribs, &weights, false, &f64::NAN);
+        tree.predict_contributions_average(&data, &mut contribs, &weights, false, &f64::NAN);
+        let full_preds = tree.predict(&data, true, &f64::NAN);
+        assert_eq!(contribs.len(), (data.cols + 1) * data.rows);
+
+        let contribs_preds: Vec<f64> = contribs
+            .chunks(data.cols + 1)
+            .map(|i| i.iter().sum())
+            .collect();
+        println!("{:?}", &contribs[0..10]);
+        println!("{:?}", &contribs_preds[0..10]);
+
+        assert_eq!(contribs_preds.len(), full_preds.len());
+        for (i, j) in full_preds.iter().zip(contribs_preds) {
+            assert_eq!(precision_round(*i, 7), precision_round(j, 7));
+        }
+
+        // Weight contributions
+        let mut contribs = vec![0.; (data.cols + 1) * data.rows];
+        tree.predict_contributions_weight(&data, &mut contribs, false, &f64::NAN);
         let full_preds = tree.predict(&data, true, &f64::NAN);
         assert_eq!(contribs.len(), (data.cols + 1) * data.rows);
 
         let contribs_preds: Vec<f64> = contribs
             .chunks(data.cols + 1)
             .map(|i| i.iter().sum())
             .collect();
@@ -491,16 +589,31 @@
 
         let preds = tree.predict(&pred_data, false, &f64::NAN);
         let increasing = preds.windows(2).all(|a| a[0] >= a[1]);
         assert!(increasing);
 
         let weights = tree.distribute_leaf_weights();
 
+        // Average contributions
+        let mut contribs = vec![0.; (data.cols + 1) * data.rows];
+        tree.predict_contributions_average(&data, &mut contribs, &weights, false, &f64::NAN);
+        let full_preds = tree.predict(&data, true, &f64::NAN);
+        assert_eq!(contribs.len(), (data.cols + 1) * data.rows);
+        let contribs_preds: Vec<f64> = contribs
+            .chunks(data.cols + 1)
+            .map(|i| i.iter().sum())
+            .collect();
+        assert_eq!(contribs_preds.len(), full_preds.len());
+        for (i, j) in full_preds.iter().zip(contribs_preds) {
+            assert_eq!(precision_round(*i, 7), precision_round(j, 7));
+        }
+
+        // Weight contributions
         let mut contribs = vec![0.; (data.cols + 1) * data.rows];
-        tree.predict_contributions(&data, &mut contribs, &weights, false, &f64::NAN);
+        tree.predict_contributions_weight(&data, &mut contribs, false, &f64::NAN);
         let full_preds = tree.predict(&data, true, &f64::NAN);
         assert_eq!(contribs.len(), (data.cols + 1) * data.rows);
         let contribs_preds: Vec<f64> = contribs
             .chunks(data.cols + 1)
             .map(|i| i.iter().sum())
             .collect();
         assert_eq!(contribs_preds.len(), full_preds.len());
```

### Comparing `forust-0.2.4/local_dependencies/forust-ml/src/utils.rs` & `forust-0.2.5/local_dependencies/forust-ml/src/utils.rs`

 * *Files identical despite different names*

### Comparing `forust-0.2.4/.gitignore` & `forust-0.2.5/.gitignore`

 * *Files identical despite different names*

### Comparing `forust-0.2.4/README.md` & `forust-0.2.5/local_dependencies/forust-ml/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 The package can be installed directly from [pypi](https://pypi.org/project/forust/).
 ```shell
 pip install forust
 ```
 
 To use in a rust project add the following to your Cargo.toml file.
 ```toml
-forust-ml = "0.2.4"
+forust-ml = "0.2.5"
 ```
 
 ## Usage
 The `GradientBooster` class is currently the only public facing class in the package, and can be used to train gradient boosted decision tree ensembles with multiple objective functions.
 
 It can be initialized with the following arguments.
 
@@ -98,33 +98,25 @@
 #       [ 1.05406709,  0.08825999,  0.21662544, -0.12083538,  0.35209258,
 #        -1.07720813],
 ```
 
 The `fit` method accepts the following arguments.
  - `X` ***(FrameLike)***: Either a pandas DataFrame, or a 2 dimensional numpy array, with numeric data.
  - `y` ***(ArrayLike)***: Either a pandas Series, or a 1 dimensional numpy array. If "LogLoss" was
-   the objective type specified, then this should only contain 1 or 0 values, where 1 is the positive class being predicted. If "SquaredLoss" is the objective type, then any continuous variable can be
-   provided.
- - `sample_weight` ***(Optional[ArrayLike], optional)***: Instance weights to use when
-    training the model. If None is passed, a weight of 1 will be used for every record.
-    Defaults to None.
+   the objective type specified, then this should only contain 1 or 0 values, where 1 is the positive class being predicted. If "SquaredLoss" is the objective type, then any continuous variable can be provided.
+ - `sample_weight` ***(Optional[ArrayLike], optional)***: Instance weights to use when training the model. If None is passed, a weight of 1 will be used for every record. Defaults to None.
 
 The predict method accepts the following arguments.
  - `X` ***(FrameLike)***: Either a pandas DataFrame, or a 2 dimensional numpy array, with numeric data.
- - `parallel` ***(Optional[bool], optional)***: Optionally specify if the predict
-   function should run in parallel on multiple threads. If `None` is
-   passed, the `parallel` attribute of the booster will be used.
-   Defaults to `None`.
+ - `parallel` ***(Optional[bool], optional)***: Optionally specify if the predict function should run in parallel on multiple threads. If `None` is passed, the `parallel` attribute of the booster will be used. Defaults to `None`.
 
 The `predict_contributions` method will predict with the fitted booster on new data, returning the feature contribution matrix. The last column is the bias term.
  - `X` ***(FrameLike)***: Either a pandas DataFrame, or a 2 dimensional numpy array, with numeric data.
- - `parallel` ***(Optional[bool], optional)***: Optionally specify if the predict
-   function should run in parallel on multiple threads. If `None` is
-   passed, the `parallel` attribute of the booster will be used.
-   Defaults to `None`.
+ - `method` ***(str, optional)***: Method to calculate the contributions, if "average" is specified, the average internal node values are calculated, this is equivalent to the `approx_contribs` parameter in XGBoost. The other supported method is "weight", this will use the internal leaf weights, to calculate the contributions. This is the same as what is described by Saabas [here](https://blog.datadive.net/interpreting-random-forests/).
+ - `parallel` ***(Optional[bool], optional)***: Optionally specify if the predict function should run in parallel on multiple threads. If `None` is passed, the `parallel` attribute of the booster will be used. Defaults to `None`.
 
 ### Inspecting the Model
 
 Once the booster has been fit, each individual tree structure can be retrieved in text form, using the `text_dump` method. This method returns a list, the same length as the number of trees in the model.
 
 ```python
 model.text_dump()[0]
@@ -138,20 +130,16 @@
 
 The `json_dump` method performs the same action, but returns the model as a json representation rather than a text string.
 
 To see an estimate for how a given feature is used in the model, the `partial_dependence` method is provided. This method calculates the partial dependence values of a feature. For each unique value of the feature, this gives the estimate of the predicted value for that feature, with the effects of all features averaged out. This information gives an estimate of how a given feature impacts the model.
 
 The `partial_dependence` method takes the following parameters...
 
- - `X` ***(FrameLike)***: Either a pandas DataFrame, or a 2 dimensional numpy array.
-      This should be the same data passed into the models fit, or predict,
-      with the columns in the same order.
- - `feature` ***(Union[str, int])***: The feature for which to calculate the partial
-      dependence values. This can be the name of a column, if the provided
-      X is a pandas DataFrame, or the index of the feature.
+ - `X` ***(FrameLike)***: Either a pandas DataFrame, or a 2 dimensional numpy array. This should be the same data passed into the models fit, or predict, with the columns in the same order.
+ - `feature` ***(Union[str, int])***: The feature for which to calculate the partial dependence values. This can be the name of a column, if the provided X is a pandas DataFrame, or the index of the feature.
 
 This method returns a 2 dimensional numpy array, where the first column is the sorted unique values of the feature, and then the second column is the partial dependence values for each feature value.
 
 This information can be plotted to visualize how a feature is used in the model, like so.
 
 ```python
 from seaborn import lineplot
```

#### html2text {}

```diff
@@ -13,15 +13,15 @@
 understand the XGBoost algorithm, additionally to have a fun project to work on
 in rust, and because I wanted to be able to experiment with adding new features
 to the algorithm in a smaller simpler codebase. All of the rust code for the
 package can be found in the [src](src/) directory, while all of the python
 wrapper code is in the [py-forust](py-forust/) directory. ## Installation The
 package can be installed directly from [pypi](https://pypi.org/project/forust/
 ). ```shell pip install forust ``` To use in a rust project add the following
-to your Cargo.toml file. ```toml forust-ml = "0.2.4" ``` ## Usage The
+to your Cargo.toml file. ```toml forust-ml = "0.2.5" ``` ## Usage The
 `GradientBooster` class is currently the only public facing class in the
 package, and can be used to train gradient boosted decision tree ensembles with
 multiple objective functions. It can be initialized with the following
 arguments. - `objective_type` ***(str, optional)***: The name of objective
 function used to optimize. Valid options include "LogLoss" to use logistic loss
 as the objective function (binary classification), or "SquaredLoss" to use
 Squared Error as the objective function (continuous regression). Defaults to
@@ -99,21 +99,27 @@
 Either a pandas DataFrame, or a 2 dimensional numpy array, with numeric data. -
 `parallel` ***(Optional[bool], optional)***: Optionally specify if the predict
 function should run in parallel on multiple threads. If `None` is passed, the
 `parallel` attribute of the booster will be used. Defaults to `None`. The
 `predict_contributions` method will predict with the fitted booster on new
 data, returning the feature contribution matrix. The last column is the bias
 term. - `X` ***(FrameLike)***: Either a pandas DataFrame, or a 2 dimensional
-numpy array, with numeric data. - `parallel` ***(Optional[bool], optional)***:
-Optionally specify if the predict function should run in parallel on multiple
-threads. If `None` is passed, the `parallel` attribute of the booster will be
-used. Defaults to `None`. ### Inspecting the Model Once the booster has been
-fit, each individual tree structure can be retrieved in text form, using the
-`text_dump` method. This method returns a list, the same length as the number
-of trees in the model. ```python model.text_dump()[0] # 0:[0 < 3]
+numpy array, with numeric data. - `method` ***(str, optional)***: Method to
+calculate the contributions, if "average" is specified, the average internal
+node values are calculated, this is equivalent to the `approx_contribs`
+parameter in XGBoost. The other supported method is "weight", this will use the
+internal leaf weights, to calculate the contributions. This is the same as what
+is described by Saabas [here](https://blog.datadive.net/interpreting-random-
+forests/). - `parallel` ***(Optional[bool], optional)***: Optionally specify if
+the predict function should run in parallel on multiple threads. If `None` is
+passed, the `parallel` attribute of the booster will be used. Defaults to
+`None`. ### Inspecting the Model Once the booster has been fit, each individual
+tree structure can be retrieved in text form, using the `text_dump` method.
+This method returns a list, the same length as the number of trees in the
+model. ```python model.text_dump()[0] # 0:[0 < 3]
 yes=1,no=2,missing=2,gain=91.50833,cover=209.388307 # 1:[4 < 13.7917]
 yes=3,no=4,missing=4,gain=28.185467,cover=94.00148 # 3:[1 < 18]
 yes=7,no=8,missing=8,gain=1.4576768,cover=22.090348 # 7:[1 < 17]
 yes=15,no=16,missing=16,gain=0.691266,cover=0.705011 # 15:leaf=-
 0.15120,cover=0.23500 # 16:leaf=0.154097,cover=0.470007 ``` The `json_dump`
 method performs the same action, but returns the model as a json representation
 rather than a text string. To see an estimate for how a given feature is used
```

### Comparing `forust-0.2.4/forust/__init__.py` & `forust-0.2.5/forust/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -36,14 +36,15 @@
         raise NotImplementedError()
 
     def predict_contributions(
         self,
         flat_data: np.ndarray,
         rows: int,
         cols: int,
+        method: str,
         parallel: bool = True,
     ) -> np.ndarray:
         raise NotImplementedError
 
     def value_partial_dependence(
         self,
         feature: int,
@@ -196,14 +197,35 @@
         self.allow_missing_splits = allow_missing_splits
         self.monotone_constraints = monotone_constraints_
         self.subsample = subsample
         self.seed = seed
         self.missing = missing
         self.create_missing_branch = create_missing_branch
 
+    def _convert_input_frame(
+        self, X: FrameLike
+    ) -> tuple[list[str], int, int, np.ndarray]:
+        """Convert data to format needed by booster.
+
+        Returns:
+            tuple[list[str], int, int, np.ndarray]: Return column names, number of rows, and number of columns, and flat data.
+        """
+        if isinstance(X, pd.DataFrame):
+            X_ = X.to_numpy()
+            features_ = X.columns.to_list()
+        else:
+            # Assume it's a numpy array.
+            X_ = X
+            features_ = []
+        if not np.issubdtype(X_.dtype, "float64"):
+            X_ = X_.astype(dtype="float64", copy=False)
+        flat_data = X_.ravel(order="F")
+        rows, cols = X_.shape
+        return features_, rows, cols, flat_data
+
     def fit(
         self,
         X: FrameLike,
         y: ArrayLike,
         sample_weight: Union[ArrayLike, None] = None,
     ):
         """Fit the gradient booster on a provided dataset.
@@ -214,23 +236,19 @@
                 was the objective type specified, then this should only contain 1 or 0 values,
                 where 1 is the positive class being predicted. If "SquaredLoss" is the
                 objective type, then any continuous variable can be provided.
             sample_weight (Union[ArrayLike, None], optional): Instance weights to use when
                 training the model. If None is passed, a weight of 1 will be used for every record.
                 Defaults to None.
         """
-        if isinstance(X, pd.DataFrame):
-            X_ = X.to_numpy()
-            self.feature_names_in_ = X.columns.to_list()
+
+        features_, rows, cols, flat_data = self._convert_input_frame(X)
+        if len(features_) > 0:
+            self.feature_names_in_ = features_
             self.insert_metadata("feature_names_in_", str(self.feature_names_in_))
-        else:
-            # Assume it's a numpy array.
-            X_ = X
-        if not np.issubdtype(X_.dtype, "float64"):
-            X_ = X_.astype(dtype="float64", copy=False)
 
         y_ = y.to_numpy() if isinstance(y, pd.Series) else y
 
         if not np.issubdtype(y_.dtype, "float64"):
             y_ = y_.astype(dtype="float64", copy=False)
 
         if sample_weight is None:
@@ -245,16 +263,14 @@
             sample_weight_ = sample_weight_.astype("float64", copy=False)
 
         # Convert the monotone constraints into the form needed
         # by the rust code.
         monotone_constraints_ = self._standardize_monotonicity_map(X)
         self.booster.monotone_constraints = monotone_constraints_
 
-        flat_data = X_.ravel(order="F")
-        rows, cols = X_.shape
         self.booster.fit(
             flat_data=flat_data,
             rows=rows,
             cols=cols,
             y=y_,
             sample_weight=sample_weight_,
         )
@@ -268,58 +284,55 @@
                 function should run in parallel on multiple threads. If `None` is
                 passed, the `parallel` attribute of the booster will be used.
                 Defaults to `None`.
 
         Returns:
             np.ndarray: Returns a numpy array of the predictions.
         """
-        X_ = X.to_numpy() if isinstance(X, pd.DataFrame) else X
-        if not np.issubdtype(X_.dtype, "float64"):
-            X_ = X_.astype(dtype="float64", copy=False)
-
+        features_, rows, cols, flat_data = self._convert_input_frame(X)
         parallel_ = self.parallel if parallel is None else parallel
-        flat_data = X_.ravel(order="F")
-        rows, cols = X_.shape
         return self.booster.predict(
             flat_data=flat_data,
             rows=rows,
             cols=cols,
             parallel=parallel_,
         )
 
     def predict_contributions(
-        self, X: FrameLike, parallel: Union[bool, None] = None
+        self, X: FrameLike, method: str = "average", parallel: Union[bool, None] = None
     ) -> np.ndarray:
         """Predict with the fitted booster on new data, returning the feature
         contribution matrix. The last column is the bias term.
 
         Args:
             X (FrameLike): Either a pandas DataFrame, or a 2 dimensional numpy array.
+            method (str, optional): Method to calculate the contributions, if "average"
+                is specified, the average internal node values are calculated, this is
+                equivalent to the `approx_contribs` parameter in XGBoost. The other supported
+                method is "weight", this will use the internal leaf weights, to calculate the
+                contributions. This is the same as what is described by Saabas [here](https://blog.datadive.net/interpreting-random-forests/).
             parallel (Union[bool, None], optional): Optionally specify if the predict
                 function should run in parallel on multiple threads. If `None` is
                 passed, the `parallel` attribute of the booster will be used.
                 Defaults to `None`.
 
         Returns:
             np.ndarray: Returns a numpy array of the predictions.
         """
-        X_ = X.to_numpy() if isinstance(X, pd.DataFrame) else X
-        if not np.issubdtype(X_.dtype, "float64"):
-            X_ = X_.astype(dtype="float64", copy=False)
-
+        features_, rows, cols, flat_data = self._convert_input_frame(X)
         parallel_ = self.parallel if parallel is None else parallel
-        flat_data = X_.ravel(order="F")
-        rows, cols = X_.shape
+
         contributions = self.booster.predict_contributions(
             flat_data=flat_data,
             rows=rows,
             cols=cols,
+            method=method,
             parallel=parallel_,
         )
-        return np.reshape(contributions, (X_.shape[0], X_.shape[1] + 1))
+        return np.reshape(contributions, (rows, cols + 1))
 
     def partial_dependence(self, X: FrameLike, feature: Union[str, int]) -> np.ndarray:
         """Calculate the partial dependence values of a feature. For each unique
         value of the feature, this gives the estimate of the predicted value for that
         feature, with the effects of all features averaged out. This information gives
         an estimate of how a given feature impacts the model.
```

### Comparing `forust-0.2.4/pyproject.toml` & `forust-0.2.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `forust-0.2.4/scratch.py` & `forust-0.2.5/scratch.py`

 * *Files identical despite different names*

### Comparing `forust-0.2.4/src/lib.rs` & `forust-0.2.5/src/lib.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 use forust_ml::constraints::{Constraint, ConstraintMap};
 use forust_ml::data::Matrix;
-use forust_ml::gradientbooster::GradientBooster as CrateGradientBooster;
+use forust_ml::gradientbooster::{ContributionsMethod, GradientBooster as CrateGradientBooster};
 use forust_ml::objective::ObjectiveType;
 use forust_ml::utils::percentiles as crate_percentiles;
 use numpy::{IntoPyArray, PyArray1, PyReadonlyArray1};
 use pyo3::exceptions::{PyKeyError, PyValueError};
 use pyo3::prelude::*;
 use pyo3::types::IntoPyDict;
 use pyo3::types::PyType;
@@ -122,22 +122,28 @@
     }
     pub fn predict_contributions<'py>(
         &self,
         py: Python<'py>,
         flat_data: PyReadonlyArray1<f64>,
         rows: usize,
         cols: usize,
+        method: &str,
         parallel: Option<bool>,
     ) -> PyResult<&'py PyArray1<f64>> {
         let flat_data = flat_data.as_slice()?;
         let data = Matrix::new(flat_data, rows, cols);
         let parallel = parallel.unwrap_or(true);
+        let method_ = match method {
+            "weight" => Ok(ContributionsMethod::Weight),
+            "average" => Ok(ContributionsMethod::Average),
+            _ => Err(PyValueError::new_err(format!("Not a valid contributions method passed, expected one of 'weight', 'average', but '{}' was provided.", method))),
+        }?;
         Ok(self
             .booster
-            .predict_contributions(&data, parallel)
+            .predict_contributions(&data, method_, parallel)
             .into_pyarray(py))
     }
 
     pub fn value_partial_dependence(&self, feature: usize, value: f64) -> PyResult<f64> {
         Ok(self.booster.value_partial_dependence(feature, value))
     }
```

### Comparing `forust-0.2.4/tests/test_booster.py` & `forust-0.2.5/tests/test_booster.py`

 * *Files identical despite different names*

### Comparing `forust-0.2.4/LICENSE` & `forust-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `forust-0.2.4/PKG-INFO` & `forust-0.2.5/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,7 @@
-Metadata-Version: 2.1
-Name: forust
-Version: 0.2.4
-Classifier: Programming Language :: Rust
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Dist: numpy>=1.21
-Requires-Dist: pandas>=1.3
-Requires-Dist: maturin; extra == 'dev'
-Requires-Dist: pytest; extra == 'dev'
-Requires-Dist: seaborn; extra == 'dev'
-Requires-Dist: xgboost==1.6.1; extra == 'dev'
-Requires-Dist: scikit-learn; extra == 'dev'
-Provides-Extra: dev
-License-File: LICENSE
-Summary: A lightweight gradient boosting implementation in Rust.
-Keywords: rust,forust,machine learning,xgboost,tree model,decision tree
-Author: James Inlow
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-
 <p align="center">
   <img  height="340" src="https://github.com/jinlow/forust/raw/main/resources/tree-image-crop.png">
 </p>
 
 
 <div align="center">
 
@@ -43,15 +22,15 @@
 The package can be installed directly from [pypi](https://pypi.org/project/forust/).
 ```shell
 pip install forust
 ```
 
 To use in a rust project add the following to your Cargo.toml file.
 ```toml
-forust-ml = "0.2.4"
+forust-ml = "0.2.5"
 ```
 
 ## Usage
 The `GradientBooster` class is currently the only public facing class in the package, and can be used to train gradient boosted decision tree ensembles with multiple objective functions.
 
 It can be initialized with the following arguments.
 
@@ -119,33 +98,25 @@
 #       [ 1.05406709,  0.08825999,  0.21662544, -0.12083538,  0.35209258,
 #        -1.07720813],
 ```
 
 The `fit` method accepts the following arguments.
  - `X` ***(FrameLike)***: Either a pandas DataFrame, or a 2 dimensional numpy array, with numeric data.
  - `y` ***(ArrayLike)***: Either a pandas Series, or a 1 dimensional numpy array. If "LogLoss" was
-   the objective type specified, then this should only contain 1 or 0 values, where 1 is the positive class being predicted. If "SquaredLoss" is the objective type, then any continuous variable can be
-   provided.
- - `sample_weight` ***(Optional[ArrayLike], optional)***: Instance weights to use when
-    training the model. If None is passed, a weight of 1 will be used for every record.
-    Defaults to None.
+   the objective type specified, then this should only contain 1 or 0 values, where 1 is the positive class being predicted. If "SquaredLoss" is the objective type, then any continuous variable can be provided.
+ - `sample_weight` ***(Optional[ArrayLike], optional)***: Instance weights to use when training the model. If None is passed, a weight of 1 will be used for every record. Defaults to None.
 
 The predict method accepts the following arguments.
  - `X` ***(FrameLike)***: Either a pandas DataFrame, or a 2 dimensional numpy array, with numeric data.
- - `parallel` ***(Optional[bool], optional)***: Optionally specify if the predict
-   function should run in parallel on multiple threads. If `None` is
-   passed, the `parallel` attribute of the booster will be used.
-   Defaults to `None`.
+ - `parallel` ***(Optional[bool], optional)***: Optionally specify if the predict function should run in parallel on multiple threads. If `None` is passed, the `parallel` attribute of the booster will be used. Defaults to `None`.
 
 The `predict_contributions` method will predict with the fitted booster on new data, returning the feature contribution matrix. The last column is the bias term.
  - `X` ***(FrameLike)***: Either a pandas DataFrame, or a 2 dimensional numpy array, with numeric data.
- - `parallel` ***(Optional[bool], optional)***: Optionally specify if the predict
-   function should run in parallel on multiple threads. If `None` is
-   passed, the `parallel` attribute of the booster will be used.
-   Defaults to `None`.
+ - `method` ***(str, optional)***: Method to calculate the contributions, if "average" is specified, the average internal node values are calculated, this is equivalent to the `approx_contribs` parameter in XGBoost. The other supported method is "weight", this will use the internal leaf weights, to calculate the contributions. This is the same as what is described by Saabas [here](https://blog.datadive.net/interpreting-random-forests/).
+ - `parallel` ***(Optional[bool], optional)***: Optionally specify if the predict function should run in parallel on multiple threads. If `None` is passed, the `parallel` attribute of the booster will be used. Defaults to `None`.
 
 ### Inspecting the Model
 
 Once the booster has been fit, each individual tree structure can be retrieved in text form, using the `text_dump` method. This method returns a list, the same length as the number of trees in the model.
 
 ```python
 model.text_dump()[0]
@@ -159,20 +130,16 @@
 
 The `json_dump` method performs the same action, but returns the model as a json representation rather than a text string.
 
 To see an estimate for how a given feature is used in the model, the `partial_dependence` method is provided. This method calculates the partial dependence values of a feature. For each unique value of the feature, this gives the estimate of the predicted value for that feature, with the effects of all features averaged out. This information gives an estimate of how a given feature impacts the model.
 
 The `partial_dependence` method takes the following parameters...
 
- - `X` ***(FrameLike)***: Either a pandas DataFrame, or a 2 dimensional numpy array.
-      This should be the same data passed into the models fit, or predict,
-      with the columns in the same order.
- - `feature` ***(Union[str, int])***: The feature for which to calculate the partial
-      dependence values. This can be the name of a column, if the provided
-      X is a pandas DataFrame, or the index of the feature.
+ - `X` ***(FrameLike)***: Either a pandas DataFrame, or a 2 dimensional numpy array. This should be the same data passed into the models fit, or predict, with the columns in the same order.
+ - `feature` ***(Union[str, int])***: The feature for which to calculate the partial dependence values. This can be the name of a column, if the provided X is a pandas DataFrame, or the index of the feature.
 
 This method returns a 2 dimensional numpy array, where the first column is the sorted unique values of the feature, and then the second column is the partial dependence values for each feature value.
 
 This information can be plotted to visualize how a feature is used in the model, like so.
 
 ```python
 from seaborn import lineplot
@@ -212,8 +179,7 @@
 
 ```python
 trained_model.save_booster("model_path.json")
 
 # To load a model from a json path.
 loaded_model = GradientBooster.load_model("model_path.json")
 ```
-
```

#### html2text {}

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1 Name: forust Version: 0.2.4 Classifier: Programming
-Language :: Rust Classifier: Programming Language :: Python :: Implementation
-:: CPython Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Dist: numpy>=1.21 Requires-Dist: pandas>=1.3 Requires-Dist: maturin;
-extra == 'dev' Requires-Dist: pytest; extra == 'dev' Requires-Dist: seaborn;
-extra == 'dev' Requires-Dist: xgboost==1.6.1; extra == 'dev' Requires-Dist:
-scikit-learn; extra == 'dev' Provides-Extra: dev License-File: LICENSE Summary:
-A lightweight gradient boosting implementation in Rust. Keywords:
-rust,forust,machine learning,xgboost,tree model,decision tree Author: James
-Inlow Requires-Python: >=3.8 Description-Content-Type: text/markdown;
-charset=UTF-8; variant=GFM
    [https://github.com/jinlow/forust/raw/main/resources/tree-image-crop.png]
  ![PyPI](https://img.shields.io/pypi/v/forust?color=gr&style=for-the-badge) !
  [Crates.io](https://img.shields.io/crates/v/forust-ml?color=gr&style=for-the-
                                     badge)
 # Forust ## _A lightweight gradient boosting package_ Forust, is a lightweight
 package for building gradient boosted decision tree ensembles. All of the
 algorithm code is written in [Rust](https://www.rust-lang.org/), with a python
@@ -24,15 +13,15 @@
 understand the XGBoost algorithm, additionally to have a fun project to work on
 in rust, and because I wanted to be able to experiment with adding new features
 to the algorithm in a smaller simpler codebase. All of the rust code for the
 package can be found in the [src](src/) directory, while all of the python
 wrapper code is in the [py-forust](py-forust/) directory. ## Installation The
 package can be installed directly from [pypi](https://pypi.org/project/forust/
 ). ```shell pip install forust ``` To use in a rust project add the following
-to your Cargo.toml file. ```toml forust-ml = "0.2.4" ``` ## Usage The
+to your Cargo.toml file. ```toml forust-ml = "0.2.5" ``` ## Usage The
 `GradientBooster` class is currently the only public facing class in the
 package, and can be used to train gradient boosted decision tree ensembles with
 multiple objective functions. It can be initialized with the following
 arguments. - `objective_type` ***(str, optional)***: The name of objective
 function used to optimize. Valid options include "LogLoss" to use logistic loss
 as the objective function (binary classification), or "SquaredLoss" to use
 Squared Error as the objective function (continuous regression). Defaults to
@@ -110,21 +99,27 @@
 Either a pandas DataFrame, or a 2 dimensional numpy array, with numeric data. -
 `parallel` ***(Optional[bool], optional)***: Optionally specify if the predict
 function should run in parallel on multiple threads. If `None` is passed, the
 `parallel` attribute of the booster will be used. Defaults to `None`. The
 `predict_contributions` method will predict with the fitted booster on new
 data, returning the feature contribution matrix. The last column is the bias
 term. - `X` ***(FrameLike)***: Either a pandas DataFrame, or a 2 dimensional
-numpy array, with numeric data. - `parallel` ***(Optional[bool], optional)***:
-Optionally specify if the predict function should run in parallel on multiple
-threads. If `None` is passed, the `parallel` attribute of the booster will be
-used. Defaults to `None`. ### Inspecting the Model Once the booster has been
-fit, each individual tree structure can be retrieved in text form, using the
-`text_dump` method. This method returns a list, the same length as the number
-of trees in the model. ```python model.text_dump()[0] # 0:[0 < 3]
+numpy array, with numeric data. - `method` ***(str, optional)***: Method to
+calculate the contributions, if "average" is specified, the average internal
+node values are calculated, this is equivalent to the `approx_contribs`
+parameter in XGBoost. The other supported method is "weight", this will use the
+internal leaf weights, to calculate the contributions. This is the same as what
+is described by Saabas [here](https://blog.datadive.net/interpreting-random-
+forests/). - `parallel` ***(Optional[bool], optional)***: Optionally specify if
+the predict function should run in parallel on multiple threads. If `None` is
+passed, the `parallel` attribute of the booster will be used. Defaults to
+`None`. ### Inspecting the Model Once the booster has been fit, each individual
+tree structure can be retrieved in text form, using the `text_dump` method.
+This method returns a list, the same length as the number of trees in the
+model. ```python model.text_dump()[0] # 0:[0 < 3]
 yes=1,no=2,missing=2,gain=91.50833,cover=209.388307 # 1:[4 < 13.7917]
 yes=3,no=4,missing=4,gain=28.185467,cover=94.00148 # 3:[1 < 18]
 yes=7,no=8,missing=8,gain=1.4576768,cover=22.090348 # 7:[1 < 17]
 yes=15,no=16,missing=16,gain=0.691266,cover=0.705011 # 15:leaf=-
 0.15120,cover=0.23500 # 16:leaf=0.154097,cover=0.470007 ``` The `json_dump`
 method performs the same action, but returns the model as a json representation
 rather than a text string. To see an estimate for how a given feature is used
```

