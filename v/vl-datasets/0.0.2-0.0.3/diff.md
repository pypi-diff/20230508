# Comparing `tmp/vl_datasets-0.0.2-py3.9-none-any.whl.zip` & `tmp/vl_datasets-0.0.3-py3.9-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 10574 bytes, number of entries: 8
--rw-r--r--  2.0 unx       79 b- defN 23-May-08 07:03 vl_datasets/__init__.py
--rw-r--r--  2.0 unx     2351 b- defN 23-May-08 07:03 vl_datasets/filtered_dataset.py
--rw-r--r--  2.0 unx     3127 b- defN 23-May-08 07:03 vl_datasets/food101.py
--rw-r--r--  2.0 unx    11357 b- defN 23-May-08 07:03 vl_datasets-0.0.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     9654 b- defN 23-May-08 07:03 vl_datasets-0.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx      108 b- defN 23-May-08 07:03 vl_datasets-0.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-May-08 07:03 vl_datasets-0.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      653 b- defN 23-May-08 07:03 vl_datasets-0.0.2.dist-info/RECORD
-8 files, 27341 bytes uncompressed, 9434 bytes compressed:  65.5%
+Zip file size: 10782 bytes, number of entries: 8
+-rw-r--r--  2.0 unx      102 b- defN 23-May-08 11:34 vl_datasets/__init__.py
+-rw-r--r--  2.0 unx     2351 b- defN 23-May-08 11:34 vl_datasets/filtered_dataset.py
+-rw-r--r--  2.0 unx     3127 b- defN 23-May-08 11:34 vl_datasets/food101.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-May-08 11:34 vl_datasets-0.0.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx    10118 b- defN 23-May-08 11:34 vl_datasets-0.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx      108 b- defN 23-May-08 11:34 vl_datasets-0.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-May-08 11:34 vl_datasets-0.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      655 b- defN 23-May-08 11:34 vl_datasets-0.0.3.dist-info/RECORD
+8 files, 27830 bytes uncompressed, 9642 bytes compressed:  65.4%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: vl_datasets/filtered_dataset.py
 Comment: 
 
 Filename: vl_datasets/food101.py
 Comment: 
 
-Filename: vl_datasets-0.0.2.dist-info/LICENSE
+Filename: vl_datasets-0.0.3.dist-info/LICENSE
 Comment: 
 
-Filename: vl_datasets-0.0.2.dist-info/METADATA
+Filename: vl_datasets-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: vl_datasets-0.0.2.dist-info/WHEEL
+Filename: vl_datasets-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: vl_datasets-0.0.2.dist-info/top_level.txt
+Filename: vl_datasets-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: vl_datasets-0.0.2.dist-info/RECORD
+Filename: vl_datasets-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## vl_datasets/__init__.py

```diff
@@ -1,2 +1,3 @@
+__version__ = '0.0.3'
 from .filtered_dataset import FilteredDataset
-from .food101 import CleanFood101
+from .food101 import CleanFood101
```

## Comparing `vl_datasets-0.0.2.dist-info/LICENSE` & `vl_datasets-0.0.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `vl_datasets-0.0.2.dist-info/METADATA` & `vl_datasets-0.0.3.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vl-datasets
-Version: 0.0.2
+Version: 0.0.3
 Summary: Clean datasets for computer vision.
 Home-page: https://github.com/visual-layer/vl-datasets
 Author: Visual Layer
 Author-email: info@visual-layer.com
 License: Apache-2.0
 Keywords: machine learning,computer vision,data-centric
 Platform: UNKNOWN
@@ -18,15 +18,14 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: torch
 Requires-Dist: torchvision
 Requires-Dist: pandas
 
 
-
 <!-- PROJECT LOGO -->
 <br />
 <div align="center">
 
 <a href="https://www.visual-layer.com">
   <img alt="Visual Layer Logo" src="https://raw.githubusercontent.com/visual-layer/fastdup/main/gallery/visual_layer_logo.png" alt="Logo" width="400">
 </a>
@@ -49,15 +48,15 @@
     <a href="https://visual-layer.com/" target="_blank" rel="noopener noreferrer">About Us</a>
     <br />
     <br /> 
     <a href="https://visualdatabase.slack.com/join/shared_invite/zt-19jaydbjn-lNDEDkgvSI1QwbTXSY6dlA#/shared-invite/email" target="_blank" rel="noopener noreferrer">
     <img src="https://img.shields.io/badge/JOIN US ON SLACK-4A154B?style=for-the-badge&logo=slack&logoColor=white" alt="Logo">
     </a>
     <a href="https://visual-layer.readme.io/discuss" target="_blank" rel="noopener noreferrer">
-    <img src="https://img.shields.io/badge/Discussion-%20Forum-brightgreen?style=for-the-badge&logo=discourse&logoColor=white" alt="Logo">
+    <img src="https://img.shields.io/badge/DISCUSSION%20FORUM-brightgreen?style=for-the-badge&logo=discourse&logoWidth=20" alt="Logo">
     </a>
     <a href="https://www.linkedin.com/company/visual-layer/" target="_blank" rel="noopener noreferrer">
     <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="Logo">
     </a>
     <a href="https://twitter.com/visual_layer" target="_blank" rel="noopener noreferrer">
     <img src="https://img.shields.io/badge/Twitter-1DA1F2?style=for-the-badge&logo=twitter&logoColor=white" alt="Logo">
     </a>
@@ -82,15 +81,15 @@
 We hope this effort will also help the community train better models and mitigate various model biases.
 
 The cleaned image dataset should be free from most if not all of the following issues:
 
 + Duplicates.
 + Broken images.
 + Outliers.
-+ Low information images (dark/bright/blurry images).
++ Dark/Bright/Blurry images.
 
 ## Datasets
 
 Here are some of the datasets we are currently working on. 
 
 | Dataset | Issues |
 | -------- | -------- |
@@ -103,24 +102,44 @@
 | KITTI   | <ul><li>Duplicates - 0.24% (12,345)</li><li>Outliers - 0.85% (456)</li><li>Broken - 0.85% (456)</li><li>Blur - 0.85% (456)</li><li>Dark - 0.85% (456)</li><li>Bright - 0.85% (456)</li></ul> |
 | DeepFashion   | <ul><li>Duplicates - 0.24% (12,345)</li><li>Outliers - 0.85% (456)</li><li>Broken - 0.85% (456)</li><li>Blur - 0.85% (456)</li><li>Dark - 0.85% (456)</li><li>Bright - 0.85% (456)</li></ul> |
 | Places365-standard   | <ul><li>Duplicates - 0.24% (12,345)</li><li>Outliers - 0.85% (456)</li><li>Broken - 0.85% (456)</li><li>Blur - 0.85% (456)</li><li>Dark - 0.85% (456)</li><li>Bright - 0.85% (456)</li></ul> |
 | CelebA-HQ   | <ul><li>Duplicates - 0.24% (12,345)</li><li>Outliers - 0.85% (456)</li><li>Broken - 0.85% (456)</li><li>Blur - 0.85% (456)</li><li>Dark - 0.85% (456)</li><li>Bright - 0.85% (456)</li></ul> |
 | ADE20K   | <ul><li>Duplicates - 0.24% (12,345)</li><li>Outliers - 0.85% (456)</li><li>Broken - 0.85% (456)</li><li>Blur - 0.85% (456)</li><li>Dark - 0.85% (456)</li><li>Bright - 0.85% (456)</li></ul> |
 | COCO   | <ul><li>Duplicates - 0.24% (12,345)</li><li>Outliers - 0.85% (456)</li><li>Broken - 0.85% (456)</li><li>Blur - 0.85% (456)</li><li>Dark - 0.85% (456)</li><li>Bright - 0.85% (456)</li></ul> |
 
+## Setting Up
 
+### Prerequisites 
 
-## Getting Started
+Supported `Python` versions:
+
+
+![Supported Python: Ubuntu](https://img.shields.io/badge/Python-3.9%20%7C%203.10-blue?style=for-the-badge)
+
+
+Supported operating systems:
+
+![Supported OS: Ubuntu](https://img.shields.io/badge/Supported%20OS-Ubuntu-orange.svg?style=for-the-badge)
 
-Install `vl_datasets` package from PyPI.
+
+### Installation
+
+**Option 1** - Install `vl_datasets` package from PyPI.
 
 ```shell
 pip install vl-datasets
 ```
 
+**Option 2** - Install the bleeding edge version on GitHub
+```
+pip install git+https://github.com/visual-layer/vl-datasets.git@master --upgrade
+```
+
+## Getting Started
+
 Import the clean version of dataset.
 
 ```python
 from vl_datasets import CleanFood101
 ```
 
 Load the dataset into a PyTorch `DataLoader`.
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vl-datasets Version: 0.0.2 Summary: Clean datasets
+Metadata-Version: 2.1 Name: vl-datasets Version: 0.0.3 Summary: Clean datasets
 for computer vision. Home-page: https://github.com/visual-layer/vl-datasets
 Author: Visual Layer Author-email: info@visual-layer.com License: Apache-2.0
 Keywords: machine learning,computer vision,data-centric Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Operating System :: OS
@@ -22,17 +22,17 @@
 remains an issue that's mainly overlooked. Training models will erroneours data
 impacts model accuracy, incurs costs in time, storage and computational
 resources. ## How? In this repo we share clean version of various computer
 vision datasets. The datasets are cleaned using a free tool we released -
 [fastdup](https://github.com/visual-layer/fastdup). We hope this effort will
 also help the community train better models and mitigate various model biases.
 The cleaned image dataset should be free from most if not all of the following
-issues: + Duplicates. + Broken images. + Outliers. + Low information images
-(dark/bright/blurry images). ## Datasets Here are some of the datasets we are
-currently working on. | Dataset | Issues | | -------- | -------- | | Food-101 |
+issues: + Duplicates. + Broken images. + Outliers. + Dark/Bright/Blurry images.
+## Datasets Here are some of the datasets we are currently working on. |
+Dataset | Issues | | -------- | -------- | | Food-101 |
     * Duplicates - 0.24% (12,345)
     * Outliers - 0.85% (456)
     * Broken - 0.85% (456)
     * Blur - 0.85% (456)
     * Dark - 0.85% (456)
     * Bright - 0.85% (456)
 | | Oxford Pets |
@@ -108,21 +108,27 @@
 | | COCO |
     * Duplicates - 0.24% (12,345)
     * Outliers - 0.85% (456)
     * Broken - 0.85% (456)
     * Blur - 0.85% (456)
     * Dark - 0.85% (456)
     * Bright - 0.85% (456)
-| ## Getting Started Install `vl_datasets` package from PyPI. ```shell pip
-install vl-datasets ``` Import the clean version of dataset. ```python from
-vl_datasets import CleanFood101 ``` Load the dataset into a PyTorch
-`DataLoader`. ```python train_dataset = CleanFood101('./', split='train',
-exclude_csv='food_101_vl-datasets_analysis.csv', transform=train_transform)
-valid_dataset = CleanFood101('./', split='test', exclude_csv='food_101_vl-
-datasets_analysis.csv', transform=valid_transform) ``` Now you can use the
-dataset in a PyTorch training loop. Refer to our sample training notebooks for
-details. Sample training notebooks: + [PyTorch](./notebooks/train-clean-
-pytorch.ipynb) + [fast.ai](./notebooks/train-fastai.ipynb)   ## Disclaimer You
-are bound to the usage license of the original dataset. It is your
-responsibility to determine whether you have permission to use the dataset
-under the dataset's license. We provide no warranty or guarantee of accuracy or
-completeness.
+| ## Setting Up ### Prerequisites Supported `Python` versions: ![Supported
+Python: Ubuntu](https://img.shields.io/badge/Python-3.9%20%7C%203.10-
+blue?style=for-the-badge) Supported operating systems: ![Supported OS: Ubuntu]
+(https://img.shields.io/badge/Supported%20OS-Ubuntu-orange.svg?style=for-the-
+badge) ### Installation **Option 1** - Install `vl_datasets` package from PyPI.
+```shell pip install vl-datasets ``` **Option 2** - Install the bleeding edge
+version on GitHub ``` pip install git+https://github.com/visual-layer/vl-
+datasets.git@master --upgrade ``` ## Getting Started Import the clean version
+of dataset. ```python from vl_datasets import CleanFood101 ``` Load the dataset
+into a PyTorch `DataLoader`. ```python train_dataset = CleanFood101('./',
+split='train', exclude_csv='food_101_vl-datasets_analysis.csv',
+transform=train_transform) valid_dataset = CleanFood101('./', split='test',
+exclude_csv='food_101_vl-datasets_analysis.csv', transform=valid_transform) ```
+Now you can use the dataset in a PyTorch training loop. Refer to our sample
+training notebooks for details. Sample training notebooks: + [PyTorch](./
+notebooks/train-clean-pytorch.ipynb) + [fast.ai](./notebooks/train-
+fastai.ipynb)   ## Disclaimer You are bound to the usage license of the
+original dataset. It is your responsibility to determine whether you have
+permission to use the dataset under the dataset's license. We provide no
+warranty or guarantee of accuracy or completeness.
```

## Comparing `vl_datasets-0.0.2.dist-info/RECORD` & `vl_datasets-0.0.3.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-vl_datasets/__init__.py,sha256=riettKJPkFqBWVD3mfNfVTJCHsoIbKR9d6rQ8Bq_BaY,79
+vl_datasets/__init__.py,sha256=aV3CzU-ljxrcUGQywh6y_10i63_o94_4_QPppBxRmNs,102
 vl_datasets/filtered_dataset.py,sha256=oztag31D7N3ufP6ETJgBVZ5aPbOvWSQUlpT35tbDtaA,2351
 vl_datasets/food101.py,sha256=TZF_VUPC2-jTYd5pQ7NAiH-i4fIPB-fpqypiV79QQjE,3127
-vl_datasets-0.0.2.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-vl_datasets-0.0.2.dist-info/METADATA,sha256=ouO3TLjR5k0R3yP1WtakkrN-7yWeie7TvdiJrk5vh8s,9654
-vl_datasets-0.0.2.dist-info/WHEEL,sha256=YT1wPceIeW2Q5XD-ypzUqEKq0BMVsXhboTN8eU2aMIk,108
-vl_datasets-0.0.2.dist-info/top_level.txt,sha256=XbUC34rGj0OLHbugO4YnVobn0t02Nc-NM3F4pwV-j8g,12
-vl_datasets-0.0.2.dist-info/RECORD,,
+vl_datasets-0.0.3.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+vl_datasets-0.0.3.dist-info/METADATA,sha256=Jtmtv5p5mLkoLRsujMHtjYrQzqYzJMuC45FeOwY2DFU,10118
+vl_datasets-0.0.3.dist-info/WHEEL,sha256=YT1wPceIeW2Q5XD-ypzUqEKq0BMVsXhboTN8eU2aMIk,108
+vl_datasets-0.0.3.dist-info/top_level.txt,sha256=XbUC34rGj0OLHbugO4YnVobn0t02Nc-NM3F4pwV-j8g,12
+vl_datasets-0.0.3.dist-info/RECORD,,
```

