# Comparing `tmp/scGPT-0.1.1.tar.gz` & `tmp/scGPT-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scGPT-0.1.1.tar", max compression
+gzip compressed data, was "scGPT-0.1.2.tar", max compression
```

## Comparing `scGPT-0.1.1.tar` & `scGPT-0.1.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1062 2023-05-02 17:04:22.123385 scGPT-0.1.1/LICENSE
--rw-r--r--   0        0        0     2521 2023-05-08 16:12:32.952102 scGPT-0.1.1/README.md
--rw-r--r--   0        0        0      904 2023-05-08 16:50:40.355285 scGPT-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      580 2023-05-02 19:00:34.630742 scGPT-0.1.1/scgpt/__init__.py
--rw-r--r--   0        0        0     7497 2023-05-02 17:04:22.215385 scGPT-0.1.1/scgpt/data_collator.py
--rw-r--r--   0        0        0     3573 2023-05-02 17:04:22.191385 scGPT-0.1.1/scgpt/data_sampler.py
--rw-r--r--   0        0        0     1068 2023-05-02 17:04:22.219385 scGPT-0.1.1/scgpt/loss.py
--rw-r--r--   0        0        0      222 2023-05-02 17:04:22.151385 scGPT-0.1.1/scgpt/model/__init__.py
--rw-r--r--   0        0        0     2393 2023-05-02 17:04:22.155385 scGPT-0.1.1/scgpt/model/dsbn.py
--rw-r--r--   0        0        0    16188 2023-05-02 22:28:23.358872 scGPT-0.1.1/scgpt/model/generation_model.py
--rw-r--r--   0        0        0      469 2023-05-02 17:04:22.159385 scGPT-0.1.1/scgpt/model/grad_reverse.py
--rw-r--r--   0        0        0    39049 2023-05-06 15:06:34.399248 scGPT-0.1.1/scgpt/model/model.py
--rw-r--r--   0        0        0    10954 2023-05-02 17:12:48.502508 scGPT-0.1.1/scgpt/preprocess.py
--rw-r--r--   0        0        0      611 2023-05-02 17:04:22.203385 scGPT-0.1.1/scgpt/scbank/__init__.py
--rw-r--r--   0        0        0     4044 2023-05-02 17:04:22.207385 scGPT-0.1.1/scgpt/scbank/data.py
--rw-r--r--   0        0        0    29625 2023-05-02 17:14:04.842980 scGPT-0.1.1/scgpt/scbank/databank.py
--rw-r--r--   0        0        0      129 2023-05-02 17:04:22.211385 scGPT-0.1.1/scgpt/scbank/monitor.py
--rw-r--r--   0        0        0      844 2023-05-02 17:04:22.203385 scGPT-0.1.1/scgpt/scbank/setting.py
--rw-r--r--   0        0        0       30 2023-05-02 17:04:22.167385 scGPT-0.1.1/scgpt/tokenizer/__init__.py
--rw-r--r--   0        0        0   761373 2023-05-02 17:04:22.175385 scGPT-0.1.1/scgpt/tokenizer/default_cellxgene_vocab.json
--rw-r--r--   0        0        0   940574 2023-05-02 17:04:22.179385 scGPT-0.1.1/scgpt/tokenizer/default_gene_vocab.json
--rw-r--r--   0        0        0    13901 2023-05-02 17:04:22.163385 scGPT-0.1.1/scgpt/tokenizer/gene_tokenizer.py
--rw-r--r--   0        0        0        0 2023-05-02 17:04:22.223385 scGPT-0.1.1/scgpt/trainer.py
--rw-r--r--   0        0        0       20 2023-05-02 17:04:22.227385 scGPT-0.1.1/scgpt/utils/__init__.py
--rw-r--r--   0        0        0    10070 2023-05-02 17:15:21.375451 scGPT-0.1.1/scgpt/utils/util.py
--rw-r--r--   0        0        0     3667 1970-01-01 00:00:00.000000 scGPT-0.1.1/setup.py
--rw-r--r--   0        0        0     3573 1970-01-01 00:00:00.000000 scGPT-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-05-02 17:04:22.123385 scGPT-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2760 2023-05-08 17:56:27.925486 scGPT-0.1.2/README.md
+-rw-r--r--   0        0        0      956 2023-05-08 19:02:52.267665 scGPT-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      638 2023-05-08 18:47:06.997466 scGPT-0.1.2/scgpt/__init__.py
+-rw-r--r--   0        0        0     7497 2023-05-02 17:04:22.215385 scGPT-0.1.2/scgpt/data_collator.py
+-rw-r--r--   0        0        0     3573 2023-05-02 17:04:22.191385 scGPT-0.1.2/scgpt/data_sampler.py
+-rw-r--r--   0        0        0     1068 2023-05-02 17:04:22.219385 scGPT-0.1.2/scgpt/loss.py
+-rw-r--r--   0        0        0      222 2023-05-02 17:04:22.151385 scGPT-0.1.2/scgpt/model/__init__.py
+-rw-r--r--   0        0        0     2393 2023-05-02 17:04:22.155385 scGPT-0.1.2/scgpt/model/dsbn.py
+-rw-r--r--   0        0        0    16188 2023-05-02 22:28:23.358872 scGPT-0.1.2/scgpt/model/generation_model.py
+-rw-r--r--   0        0        0      469 2023-05-02 17:04:22.159385 scGPT-0.1.2/scgpt/model/grad_reverse.py
+-rw-r--r--   0        0        0    39049 2023-05-08 18:55:29.408763 scGPT-0.1.2/scgpt/model/model.py
+-rw-r--r--   0        0        0    10954 2023-05-02 17:12:48.502508 scGPT-0.1.2/scgpt/preprocess.py
+-rw-r--r--   0        0        0      611 2023-05-02 17:04:22.203385 scGPT-0.1.2/scgpt/scbank/__init__.py
+-rw-r--r--   0        0        0     4044 2023-05-02 17:04:22.207385 scGPT-0.1.2/scgpt/scbank/data.py
+-rw-r--r--   0        0        0    29625 2023-05-02 17:14:04.842980 scGPT-0.1.2/scgpt/scbank/databank.py
+-rw-r--r--   0        0        0      129 2023-05-02 17:04:22.211385 scGPT-0.1.2/scgpt/scbank/monitor.py
+-rw-r--r--   0        0        0      844 2023-05-02 17:04:22.203385 scGPT-0.1.2/scgpt/scbank/setting.py
+-rw-r--r--   0        0        0       30 2023-05-02 17:04:22.167385 scGPT-0.1.2/scgpt/tokenizer/__init__.py
+-rw-r--r--   0        0        0   761373 2023-05-02 17:04:22.175385 scGPT-0.1.2/scgpt/tokenizer/default_cellxgene_vocab.json
+-rw-r--r--   0        0        0   940574 2023-05-02 17:04:22.179385 scGPT-0.1.2/scgpt/tokenizer/default_gene_vocab.json
+-rw-r--r--   0        0        0    13901 2023-05-02 17:04:22.163385 scGPT-0.1.2/scgpt/tokenizer/gene_tokenizer.py
+-rw-r--r--   0        0        0        0 2023-05-02 17:04:22.223385 scGPT-0.1.2/scgpt/trainer.py
+-rw-r--r--   0        0        0       20 2023-05-02 17:04:22.227385 scGPT-0.1.2/scgpt/utils/__init__.py
+-rw-r--r--   0        0        0    10070 2023-05-02 17:15:21.375451 scGPT-0.1.2/scgpt/utils/util.py
+-rw-r--r--   0        0        0     3951 1970-01-01 00:00:00.000000 scGPT-0.1.2/setup.py
+-rw-r--r--   0        0        0     3986 1970-01-01 00:00:00.000000 scGPT-0.1.2/PKG-INFO
```

### Comparing `scGPT-0.1.1/LICENSE` & `scGPT-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `scGPT-0.1.1/README.md` & `scGPT-0.1.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,47 @@
 # scGPT
 
 This is the official codebase for **scGPT: Towards Building a Foundation Model for Single-Cell Multi-omics Using Generative AI**.
 
 ## Installation
 
+scGPT is available on PyPI. To install scGPT, run the following command:
+
+```bash
+$ pip install scgpt
+```
+
+[Optional] We recommend using [wandb](https://wandb.ai/) for logging and visualization.
+
+```bash
+$ pip install wandb
+```
+
 For developing, we are using the [Poetry](https://python-poetry.org/) package manager. To install Poetry, follow the instructions [here](https://python-poetry.org/docs/#installation).
 
 ```bash
 $ git clone this-repo-url
 $ cd scGPT
 $ poetry install
 ```
 
-The `flash-attn` dependency usually requires specific GPU and CUDA version. If you encounter any issues, please refer to the [flash-attn](https://github.com/HazyResearch/flash-attention/tree/main) repository for installation instructions.
+**Note**: The `flash-attn` dependency usually requires specific GPU and CUDA version. If you encounter any issues, please refer to the [flash-attn](https://github.com/HazyResearch/flash-attention/tree/main) repository for installation instructions.
 
 ## Pretrained scGPT checkpoints
 
 Please download the pretrained scGPT checkpoints from [here](https://drive.google.com/drive/folders/1kkug5C7NjvXIwQGGaGoqXTk_Lb_pDrBU?usp=sharing).
 
 ## Fine-tune scGPT for scRNA-seq integration
 
 Please see our example code in [examples/finetune_integration.py](examples/finetune_integration.py). By default, the script assumes the scGPT checkpoint folder stored in the `examples/save` directory.
 
 ## To-do-list
 
 - [x] Upload the pretrained model checkpoint
-- [ ] Publish to pypi
+- [x] Publish to pypi
 - [ ] Provide the pretraining code with generative attention masking
 - [ ] Finetuning examples for multi-omics integration, cell tyep annotation, perturbation prediction, cell generation
 - [ ] Example code for Gene Regulatory Network analysis
 - [ ] Documentation website with readthedocs
 - [ ] Bump up to pytorch 2.0
 - [ ] New pretraining on larger datasets
 - [ ] Reference mapping example
```

### Comparing `scGPT-0.1.1/pyproject.toml` & `scGPT-0.1.2/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "scGPT"
-version = "0.1.1"
+version = "0.1.2"
 description = "Large-scale generative pretrain of single cell using transformer."
+license = "MIT"
 authors = ["Haotian <subercui@gmail.com>"]
+repository = "https://github.com/bowang-lab/scGPT"
+homepage = "https://github.com/bowang-lab/scGPT"
 readme = "README.md"
 
-[project.urls]
-"Homepage" = "https:github.com/bowang-lab/scGPT"
-
 [tool.poetry.dependencies]
-python = ">=3.7.1,<3.11"
+python = ">=3.7.13,<3.11"
 pandas = "1.3.5"
 scvi-tools = "^0.16.0"
 llvmlite = "^0.38.0"
-scanpy = "^1.9.1"
+scanpy = "~1.9.1"
 torch = "1.13.0"
 torchtext = "0.14.0"
 transformers = "^4.18.0"
 numba = "^0.55.1"
 scikit-misc = "^0.1.4"
 umap-learn = "^0.5.3"
 leidenalg = "^0.8.10"
```

### Comparing `scGPT-0.1.1/scgpt/__init__.py` & `scGPT-0.1.2/scgpt/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-__version__ = "0.1.0"
+__version__ = "0.1.2"
 import logging
 import sys
 
 logger = logging.getLogger("scGPT")
 # check if logger has been initialized
-if not logger.hasHandlers():
+if not logger.hasHandlers() or len(logger.handlers) == 0:
+    logger.propagate = False
     logger.setLevel(logging.INFO)
     handler = logging.StreamHandler(sys.stdout)
     handler.setLevel(logging.INFO)
     formatter = logging.Formatter(
         "%(name)s - %(levelname)s - %(message)s", datefmt="%H:%M:%S"
     )
     handler.setFormatter(formatter)
```

### Comparing `scGPT-0.1.1/scgpt/data_collator.py` & `scGPT-0.1.2/scgpt/data_collator.py`

 * *Files identical despite different names*

### Comparing `scGPT-0.1.1/scgpt/data_sampler.py` & `scGPT-0.1.2/scgpt/data_sampler.py`

 * *Files identical despite different names*

### Comparing `scGPT-0.1.1/scgpt/loss.py` & `scGPT-0.1.2/scgpt/loss.py`

 * *Files identical despite different names*

### Comparing `scGPT-0.1.1/scgpt/model/dsbn.py` & `scGPT-0.1.2/scgpt/model/dsbn.py`

 * *Files identical despite different names*

### Comparing `scGPT-0.1.1/scgpt/model/generation_model.py` & `scGPT-0.1.2/scgpt/model/generation_model.py`

 * *Files identical despite different names*

### Comparing `scGPT-0.1.1/scgpt/model/model.py` & `scGPT-0.1.2/scgpt/model/model.py`

 * *Files identical despite different names*

### Comparing `scGPT-0.1.1/scgpt/preprocess.py` & `scGPT-0.1.2/scgpt/preprocess.py`

 * *Files identical despite different names*

### Comparing `scGPT-0.1.1/scgpt/scbank/__init__.py` & `scGPT-0.1.2/scgpt/scbank/__init__.py`

 * *Files identical despite different names*

### Comparing `scGPT-0.1.1/scgpt/scbank/data.py` & `scGPT-0.1.2/scgpt/scbank/data.py`

 * *Files identical despite different names*

### Comparing `scGPT-0.1.1/scgpt/scbank/databank.py` & `scGPT-0.1.2/scgpt/scbank/databank.py`

 * *Files identical despite different names*

### Comparing `scGPT-0.1.1/scgpt/scbank/setting.py` & `scGPT-0.1.2/scgpt/scbank/setting.py`

 * *Files identical despite different names*

### Comparing `scGPT-0.1.1/scgpt/tokenizer/default_cellxgene_vocab.json` & `scGPT-0.1.2/scgpt/tokenizer/default_cellxgene_vocab.json`

 * *Files identical despite different names*

### Comparing `scGPT-0.1.1/scgpt/tokenizer/default_gene_vocab.json` & `scGPT-0.1.2/scgpt/tokenizer/default_gene_vocab.json`

 * *Files identical despite different names*

### Comparing `scGPT-0.1.1/scgpt/tokenizer/gene_tokenizer.py` & `scGPT-0.1.2/scgpt/tokenizer/gene_tokenizer.py`

 * *Files identical despite different names*

### Comparing `scGPT-0.1.1/scgpt/utils/util.py` & `scGPT-0.1.2/scgpt/utils/util.py`

 * *Files identical despite different names*

### Comparing `scGPT-0.1.1/setup.py` & `scGPT-0.1.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,35 +10,35 @@
 install_requires = \
 ['datasets>=2.3.0,<3.0.0',
  'flash-attn==1.0.1',
  'leidenalg>=0.8.10,<0.9.0',
  'llvmlite>=0.38.0,<0.39.0',
  'numba>=0.55.1,<0.56.0',
  'pandas==1.3.5',
- 'scanpy>=1.9.1,<2.0.0',
+ 'scanpy>=1.9.1,<1.10.0',
  'scib>=1.0.3,<2.0.0',
  'scikit-misc>=0.1.4,<0.2.0',
  'scvi-tools>=0.16.0,<0.17.0',
  'torch==1.13.0',
  'torchtext==0.14.0',
  'transformers>=4.18.0,<5.0.0',
  'typing-extensions>=4.2.0,<5.0.0',
  'umap-learn>=0.5.3,<0.6.0']
 
 setup_kwargs = {
     'name': 'scgpt',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': 'Large-scale generative pretrain of single cell using transformer.',
-    'long_description': '# scGPT\n\nThis is the official codebase for **scGPT: Towards Building a Foundation Model for Single-Cell Multi-omics Using Generative AI**.\n\n## Installation\n\nFor developing, we are using the [Poetry](https://python-poetry.org/) package manager. To install Poetry, follow the instructions [here](https://python-poetry.org/docs/#installation).\n\n```bash\n$ git clone this-repo-url\n$ cd scGPT\n$ poetry install\n```\n\nThe `flash-attn` dependency usually requires specific GPU and CUDA version. If you encounter any issues, please refer to the [flash-attn](https://github.com/HazyResearch/flash-attention/tree/main) repository for installation instructions.\n\n## Pretrained scGPT checkpoints\n\nPlease download the pretrained scGPT checkpoints from [here](https://drive.google.com/drive/folders/1kkug5C7NjvXIwQGGaGoqXTk_Lb_pDrBU?usp=sharing).\n\n## Fine-tune scGPT for scRNA-seq integration\n\nPlease see our example code in [examples/finetune_integration.py](examples/finetune_integration.py). By default, the script assumes the scGPT checkpoint folder stored in the `examples/save` directory.\n\n## To-do-list\n\n- [x] Upload the pretrained model checkpoint\n- [ ] Publish to pypi\n- [ ] Provide the pretraining code with generative attention masking\n- [ ] Finetuning examples for multi-omics integration, cell tyep annotation, perturbation prediction, cell generation\n- [ ] Example code for Gene Regulatory Network analysis\n- [ ] Documentation website with readthedocs\n- [ ] Bump up to pytorch 2.0\n- [ ] New pretraining on larger datasets\n- [ ] Reference mapping example\n- [ ] Finetuning with LORA\n- [ ] Publish to huggingface model hub\n\n## Contributing\n\nWe greatly welcome contributions to scGPT. Please submit a pull request if you have any ideas or bug fixes. We also welcome any issues you encounter while using scGPT.\n\n## Acknowledgements\n\nWe sincerely thank the authors of following open-source projects:\n\n- [flash-attention](https://github.com/HazyResearch/flash-attention)\n- [scanpy](https://github.com/scverse/scanpy)\n- [scvi-tools](https://github.com/scverse/scvi-tools)\n- [scib](https://github.com/theislab/scib)\n- [datasets](https://github.com/huggingface/datasets)\n- [transformers](https://github.com/huggingface/transformers)\n\n## Citing scGPT\n\n```bibtex\n@article{cui2023scGPT,\ntitle={scGPT: Towards Building a Foundation Model for Single-Cell Multi-omics Using Generative AI},\nauthor={Cui, Haotian and Wang, Chloe and Maan, Hassaan and Wang, Bo},\njournal={bioRxiv},\nyear={2023},\npublisher={Cold Spring Harbor Laboratory}\n}\n```\n',
+    'long_description': '# scGPT\n\nThis is the official codebase for **scGPT: Towards Building a Foundation Model for Single-Cell Multi-omics Using Generative AI**.\n\n## Installation\n\nscGPT is available on PyPI. To install scGPT, run the following command:\n\n```bash\n$ pip install scgpt\n```\n\n[Optional] We recommend using [wandb](https://wandb.ai/) for logging and visualization.\n\n```bash\n$ pip install wandb\n```\n\nFor developing, we are using the [Poetry](https://python-poetry.org/) package manager. To install Poetry, follow the instructions [here](https://python-poetry.org/docs/#installation).\n\n```bash\n$ git clone this-repo-url\n$ cd scGPT\n$ poetry install\n```\n\n**Note**: The `flash-attn` dependency usually requires specific GPU and CUDA version. If you encounter any issues, please refer to the [flash-attn](https://github.com/HazyResearch/flash-attention/tree/main) repository for installation instructions.\n\n## Pretrained scGPT checkpoints\n\nPlease download the pretrained scGPT checkpoints from [here](https://drive.google.com/drive/folders/1kkug5C7NjvXIwQGGaGoqXTk_Lb_pDrBU?usp=sharing).\n\n## Fine-tune scGPT for scRNA-seq integration\n\nPlease see our example code in [examples/finetune_integration.py](examples/finetune_integration.py). By default, the script assumes the scGPT checkpoint folder stored in the `examples/save` directory.\n\n## To-do-list\n\n- [x] Upload the pretrained model checkpoint\n- [x] Publish to pypi\n- [ ] Provide the pretraining code with generative attention masking\n- [ ] Finetuning examples for multi-omics integration, cell tyep annotation, perturbation prediction, cell generation\n- [ ] Example code for Gene Regulatory Network analysis\n- [ ] Documentation website with readthedocs\n- [ ] Bump up to pytorch 2.0\n- [ ] New pretraining on larger datasets\n- [ ] Reference mapping example\n- [ ] Finetuning with LORA\n- [ ] Publish to huggingface model hub\n\n## Contributing\n\nWe greatly welcome contributions to scGPT. Please submit a pull request if you have any ideas or bug fixes. We also welcome any issues you encounter while using scGPT.\n\n## Acknowledgements\n\nWe sincerely thank the authors of following open-source projects:\n\n- [flash-attention](https://github.com/HazyResearch/flash-attention)\n- [scanpy](https://github.com/scverse/scanpy)\n- [scvi-tools](https://github.com/scverse/scvi-tools)\n- [scib](https://github.com/theislab/scib)\n- [datasets](https://github.com/huggingface/datasets)\n- [transformers](https://github.com/huggingface/transformers)\n\n## Citing scGPT\n\n```bibtex\n@article{cui2023scGPT,\ntitle={scGPT: Towards Building a Foundation Model for Single-Cell Multi-omics Using Generative AI},\nauthor={Cui, Haotian and Wang, Chloe and Maan, Hassaan and Wang, Bo},\njournal={bioRxiv},\nyear={2023},\npublisher={Cold Spring Harbor Laboratory}\n}\n```\n',
     'author': 'Haotian',
     'author_email': 'subercui@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
-    'url': 'None',
+    'url': 'https://github.com/bowang-lab/scGPT',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.7.1,<3.11',
+    'python_requires': '>=3.7.13,<3.11',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `scGPT-0.1.1/PKG-INFO` & `scGPT-0.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,63 +1,79 @@
 Metadata-Version: 2.1
 Name: scgpt
-Version: 0.1.1
+Version: 0.1.2
 Summary: Large-scale generative pretrain of single cell using transformer.
+Home-page: https://github.com/bowang-lab/scGPT
+License: MIT
 Author: Haotian
 Author-email: subercui@gmail.com
-Requires-Python: >=3.7.1,<3.11
+Requires-Python: >=3.7.13,<3.11
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: datasets (>=2.3.0,<3.0.0)
 Requires-Dist: flash-attn (==1.0.1)
 Requires-Dist: leidenalg (>=0.8.10,<0.9.0)
 Requires-Dist: llvmlite (>=0.38.0,<0.39.0)
 Requires-Dist: numba (>=0.55.1,<0.56.0)
 Requires-Dist: pandas (==1.3.5)
-Requires-Dist: scanpy (>=1.9.1,<2.0.0)
+Requires-Dist: scanpy (>=1.9.1,<1.10.0)
 Requires-Dist: scib (>=1.0.3,<2.0.0)
 Requires-Dist: scikit-misc (>=0.1.4,<0.2.0)
 Requires-Dist: scvi-tools (>=0.16.0,<0.17.0)
 Requires-Dist: torch (==1.13.0)
 Requires-Dist: torchtext (==0.14.0)
 Requires-Dist: transformers (>=4.18.0,<5.0.0)
 Requires-Dist: typing-extensions (>=4.2.0,<5.0.0)
 Requires-Dist: umap-learn (>=0.5.3,<0.6.0)
+Project-URL: Repository, https://github.com/bowang-lab/scGPT
 Description-Content-Type: text/markdown
 
 # scGPT
 
 This is the official codebase for **scGPT: Towards Building a Foundation Model for Single-Cell Multi-omics Using Generative AI**.
 
 ## Installation
 
+scGPT is available on PyPI. To install scGPT, run the following command:
+
+```bash
+$ pip install scgpt
+```
+
+[Optional] We recommend using [wandb](https://wandb.ai/) for logging and visualization.
+
+```bash
+$ pip install wandb
+```
+
 For developing, we are using the [Poetry](https://python-poetry.org/) package manager. To install Poetry, follow the instructions [here](https://python-poetry.org/docs/#installation).
 
 ```bash
 $ git clone this-repo-url
 $ cd scGPT
 $ poetry install
 ```
 
-The `flash-attn` dependency usually requires specific GPU and CUDA version. If you encounter any issues, please refer to the [flash-attn](https://github.com/HazyResearch/flash-attention/tree/main) repository for installation instructions.
+**Note**: The `flash-attn` dependency usually requires specific GPU and CUDA version. If you encounter any issues, please refer to the [flash-attn](https://github.com/HazyResearch/flash-attention/tree/main) repository for installation instructions.
 
 ## Pretrained scGPT checkpoints
 
 Please download the pretrained scGPT checkpoints from [here](https://drive.google.com/drive/folders/1kkug5C7NjvXIwQGGaGoqXTk_Lb_pDrBU?usp=sharing).
 
 ## Fine-tune scGPT for scRNA-seq integration
 
 Please see our example code in [examples/finetune_integration.py](examples/finetune_integration.py). By default, the script assumes the scGPT checkpoint folder stored in the `examples/save` directory.
 
 ## To-do-list
 
 - [x] Upload the pretrained model checkpoint
-- [ ] Publish to pypi
+- [x] Publish to pypi
 - [ ] Provide the pretraining code with generative attention masking
 - [ ] Finetuning examples for multi-omics integration, cell tyep annotation, perturbation prediction, cell generation
 - [ ] Example code for Gene Regulatory Network analysis
 - [ ] Documentation website with readthedocs
 - [ ] Bump up to pytorch 2.0
 - [ ] New pretraining on larger datasets
 - [ ] Reference mapping example
```

