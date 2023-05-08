# Comparing `tmp/x-transformers-1.9.1.tar.gz` & `tmp/x-transformers-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "x-transformers-1.9.1.tar", last modified: Mon Feb 13 17:32:33 2023, max compression
+gzip compressed data, was "x-transformers-1.9.2.tar", last modified: Mon Feb 13 18:26:03 2023, max compression
```

## Comparing `x-transformers-1.9.1.tar` & `x-transformers-1.9.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 17:32:33.019171 x-transformers-1.9.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-02-13 17:32:20.000000 x-transformers-1.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-02-13 17:32:33.019171 x-transformers-1.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    58796 2023-02-13 17:32:20.000000 x-transformers-1.9.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-13 17:32:33.019171 x-transformers-1.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-02-13 17:32:20.000000 x-transformers-1.9.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 17:32:33.019171 x-transformers-1.9.1/x_transformers/
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-02-13 17:32:20.000000 x-transformers-1.9.1/x_transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-02-13 17:32:20.000000 x-transformers-1.9.1/x_transformers/autoregressive_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-02-13 17:32:20.000000 x-transformers-1.9.1/x_transformers/continuous_autoregressive_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    10414 2023-02-13 17:32:20.000000 x-transformers-1.9.1/x_transformers/nonautoregressive_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    53236 2023-02-13 17:32:20.000000 x-transformers-1.9.1/x_transformers/x_transformers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 17:32:33.019171 x-transformers-1.9.1/x_transformers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-02-13 17:32:32.000000 x-transformers-1.9.1/x_transformers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-02-13 17:32:32.000000 x-transformers-1.9.1/x_transformers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-13 17:32:32.000000 x-transformers-1.9.1/x_transformers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-02-13 17:32:32.000000 x-transformers-1.9.1/x_transformers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-02-13 17:32:32.000000 x-transformers-1.9.1/x_transformers.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 18:26:03.418202 x-transformers-1.9.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-02-13 18:25:53.000000 x-transformers-1.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-02-13 18:26:03.418202 x-transformers-1.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    58817 2023-02-13 18:25:53.000000 x-transformers-1.9.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-13 18:26:03.418202 x-transformers-1.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-02-13 18:25:54.000000 x-transformers-1.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 18:26:03.414203 x-transformers-1.9.2/x_transformers/
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-02-13 18:25:54.000000 x-transformers-1.9.2/x_transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-02-13 18:25:54.000000 x-transformers-1.9.2/x_transformers/autoregressive_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-02-13 18:25:54.000000 x-transformers-1.9.2/x_transformers/continuous_autoregressive_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10414 2023-02-13 18:25:54.000000 x-transformers-1.9.2/x_transformers/nonautoregressive_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53140 2023-02-13 18:25:54.000000 x-transformers-1.9.2/x_transformers/x_transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 18:26:03.414203 x-transformers-1.9.2/x_transformers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-02-13 18:26:03.000000 x-transformers-1.9.2/x_transformers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-02-13 18:26:03.000000 x-transformers-1.9.2/x_transformers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-13 18:26:03.000000 x-transformers-1.9.2/x_transformers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-02-13 18:26:03.000000 x-transformers-1.9.2/x_transformers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-02-13 18:26:03.000000 x-transformers-1.9.2/x_transformers.egg-info/top_level.txt
```

### Comparing `x-transformers-1.9.1/LICENSE` & `x-transformers-1.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `x-transformers-1.9.1/PKG-INFO` & `x-transformers-1.9.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: x-transformers
-Version: 1.9.1
+Version: 1.9.2
 Summary: X-Transformers - Pytorch
 Home-page: https://github.com/lucidrains/x-transformers
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,transformers
 Classifier: Development Status :: 4 - Beta
```

### Comparing `x-transformers-1.9.1/README.md` & `x-transformers-1.9.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1120,15 +1120,15 @@
 
 x = torch.randint(0, 20000, (1, 1024))
 model(x)
 ```
 
 <img src="./images/qknorm-analysis.png" width="450px"></img>
 
-Update: Google Brain has proven out cosine sim attention in <a href="https://arxiv.org/abs/2302.05442">a 22B parameter model</a>. In their papers, they have analysis showing that the normalization resulted in not only extra stability, but also better results in the end (due to less need to adjust learning rate when increasing parameter count).
+Update: Google Brain has proven out something similar to cosine sim attention in <a href="https://arxiv.org/abs/2302.05442">a 22B parameter model</a>. In their papers, they have analysis showing that the normalization resulted in not only extra stability, but also better results in the end (due to less need to adjust learning rate when increasing parameter count).
 
 We are nearing the point of wiping out a source of transformer training instability with one simple intervention, in my opinion. The only slight difference in the paper is that they still have a learned scale across the feature dimension (per use of rmsnorm). Not sure how critical this is, but just to make sure we don't miss anything, I will include this here. You can use this by setting `qk_norm_dim_scale = True`
 
 ```python
 import torch
 from x_transformers import TransformerWrapper, Decoder
```

#### html2text {}

```diff
@@ -420,167 +420,168 @@
 Another update: Simply scaling the cosine similarity (group of 1) with a fixed
 constant (10) may work too ```python import torch from x_transformers import
 TransformerWrapper, Decoder model = TransformerWrapper( num_tokens = 20000,
 max_seq_len = 1024, attn_layers = Decoder( dim = 512, depth = 6, heads = 8,
 attn_qk_norm = True, # set to True attn_qk_norm_scale = 10 # new scale on the
 similarity, with groups of 1 ) ) x = torch.randint(0, 20000, (1, 1024)) model
 (x) ``` [./images/qknorm-analysis.png] Update: Google Brain has proven out
-cosine sim attention in a_22B_parameter_model. In their papers, they have
-analysis showing that the normalization resulted in not only extra stability,
-but also better results in the end (due to less need to adjust learning rate
-when increasing parameter count). We are nearing the point of wiping out a
-source of transformer training instability with one simple intervention, in my
-opinion. The only slight difference in the paper is that they still have a
-learned scale across the feature dimension (per use of rmsnorm). Not sure how
-critical this is, but just to make sure we don't miss anything, I will include
-this here. You can use this by setting `qk_norm_dim_scale = True` ```python
-import torch from x_transformers import TransformerWrapper, Decoder model =
-TransformerWrapper( num_tokens = 20000, max_seq_len = 1024, attn_layers =
-Decoder( dim = 512, depth = 12, heads = 8, attn_qk_norm = True,
-attn_qk_norm_dim_scale = True # set this to True, in addition to `attn_qk_norm
-= True` ) ) x = torch.randint(0, 256, (1, 1024)) model(x) ``` ### Turning off
-absolute positional embedding A number of papers have hinted that causal
-transformers (`Decoder`) can learn absolute positions in the absence of added
-embeddings of any sort. This was recently thoroughly investigated here. You can
-turn off the absolute positional embedding by setting `use_abs_pos_emb = False`
-in the `TransformerWrapper` Given PaLM, the trend going forward may be to forgo
-absolute positional embedding (again, for causal transformers only), and add
-relative positional embeddings with RoPE, ALiBi, etc. ```python import torch
-from x_transformers import TransformerWrapper, Decoder model =
-TransformerWrapper( num_tokens = 20000, max_seq_len = 1024, use_abs_pos_emb =
-False, # set this to False attn_layers = Decoder( dim = 512, depth = 6, heads =
-8, ) ) x = torch.randint(0, 20000, (1, 1024)) model(x) ``` ### Forgetful Causal
-Mask [./images/fcm.png] This_paper shows convincing results that one can
-combine masking (from masked language modeling) with autoregressive training,
-leading to significantly better results. You can use this by setting the
-`mask_prob` on the `AutoregressiveWrapper` class ```python import torch from
-x_transformers import TransformerWrapper, Decoder, AutoregressiveWrapper model
-= TransformerWrapper( num_tokens = 20000, max_seq_len = 1024, attn_layers =
-Decoder( dim = 512, depth = 12, heads = 8 ) ) model = AutoregressiveWrapper
-( model, mask_prob = 0.15 # in paper, they use 15%, same as BERT ).cuda() #
-mock data x = torch.randint(0, 20000, (1, 1024)).cuda() # derive cross entropy
-loss, masking all taken care of loss = model(x) loss.backward() ``` ##
-Miscellaneous Cross Attention ```python import torch from x_transformers import
-Encoder, CrossAttender enc = Encoder(dim = 512, depth = 6) model =
-CrossAttender(dim = 512, depth = 6) nodes = torch.randn(1, 1, 512) node_masks =
-torch.ones(1, 1).bool() neighbors = torch.randn(1, 5, 512) neighbor_masks =
-torch.ones(1, 5).bool() encoded_neighbors = enc(neighbors, mask =
-neighbor_masks) model(nodes, context = encoded_neighbors, mask = node_masks,
-context_mask = neighbor_masks) # (1, 1, 512) ``` Pass in continuous values
-```python import torch from x_transformers import ContinuousTransformerWrapper,
-Decoder model = ContinuousTransformerWrapper( dim_in = 32, dim_out = 100,
-max_seq_len = 1024, attn_layers = Decoder( dim = 512, depth = 12, heads = 8 ) )
-x = torch.randn((1, 1024, 32)) model(x) # (1, 1024, 100) ``` You can also train
-a transformer that accepts continuous values autoregressively easily, in the
-same scheme as done successfully in this_paper ```python import torch from
-x_transformers import ContinuousTransformerWrapper, Decoder from x_transformers
-import ContinuousAutoregressiveWrapper model = ContinuousTransformerWrapper
-( dim_in = 777, dim_out = 777, max_seq_len = 1024, attn_layers = Decoder( dim =
-512, depth = 12, heads = 8 ) ) # wrap it with the continuous autoregressive
-wrapper model = ContinuousAutoregressiveWrapper(model) # mock data x =
-torch.randn((1, 1024, 777)) mask = torch.ones(1, 1024).bool() # train on a lot
-of data above loss = model(x, mask = mask) loss.backward # then generate
-start_emb = torch.randn(1, 777) generated = model.generate(start_emb, 17) #
-(17, 777) ``` ## Citations ```bibtex @misc{vaswani2017attention, title =
-{Attention Is All You Need}, author = {Ashish Vaswani and Noam Shazeer and Niki
-Parmar and Jakob Uszkoreit and Llion Jones and Aidan N. Gomez and Lukasz Kaiser
-and Illia Polosukhin}, year = {2017}, eprint = {1706.03762}, archivePrefix =
-{arXiv}, primaryClass = {cs.CL} } ``` ```bibtex @article{DBLP:journals/corr/
-abs-1907-01470, author = {Sainbayar Sukhbaatar and Edouard Grave and Guillaume
-Lample and Herv{\'{e}} J{\'{e}}gou and Armand Joulin}, title = {Augmenting
-Self-attention with Persistent Memory}, journal = {CoRR}, volume = {abs/
-1907.01470}, year = {2019}, url = {http://arxiv.org/abs/1907.01470} } ```
-```bibtex @article{1910.05895, author = {Toan Q. Nguyen and Julian Salazar},
-title = {Transformers without Tears: Improving the Normalization of Self-
-Attention}, year = {2019}, eprint = {arXiv:1910.05895}, doi = {10.5281/
-zenodo.3525484}, } ``` ```bibtex @misc{shazeer2020glu, title = {GLU Variants
-Improve Transformer}, author = {Noam Shazeer}, year = {2020}, url = {https://
-arxiv.org/abs/2002.05202} } ``` ```bibtex @misc{bhojanapalli2020lowrank, title
-= {Low-Rank Bottleneck in Multi-head Attention Models}, author = {Srinadh
-Bhojanapalli and Chulhee Yun and Ankit Singh Rawat and Sashank J. Reddi and
-Sanjiv Kumar}, year = {2020}, eprint = {2002.07028} } ``` ```bibtex @misc
-{burtsev2020memory, title = {Memory Transformer}, author = {Mikhail S. Burtsev
-and Grigory V. Sapunov}, year = {2020}, eprint = {2006.11527}, archivePrefix =
-{arXiv}, primaryClass = {cs.CL} } ``` ```bibtex @misc{zhao2019explicit, title =
-{Explicit Sparse Transformer: Concentrated Attention Through Explicit
-Selection}, author = {Guangxiang Zhao and Junyang Lin and Zhiyuan Zhang and
-Xuancheng Ren and Qi Su and Xu Sun}, year = {2019}, eprint = {1912.11637},
-archivePrefix = {arXiv}, primaryClass = {cs.CL} } ``` ```bibtex @misc
-{correia2019adaptively, title = {Adaptively Sparse Transformers}, author =
-{GonÃ§alo M. Correia and Vlad Niculae and AndrÃ© F. T. Martins}, year = {2019},
-eprint = {1909.00015}, archivePrefix = {arXiv}, primaryClass = {cs.CL} } ```
-```bibtex @misc{shazeer2020talkingheads, title = {Talking-Heads Attention},
-author = {Noam Shazeer and Zhenzhong Lan and Youlong Cheng and Nan Ding and Le
-Hou}, year = {2020}, eprint = {2003.02436}, archivePrefix = {arXiv},
-primaryClass = {cs.LG} } ``` ```bibtex @misc{press2020improving, title =
-{Improving Transformer Models by Reordering their Sublayers}, author = {Ofir
-Press and Noah A. Smith and Omer Levy}, year = {2020}, eprint = {1911.03864},
-archivePrefix = {arXiv}, primaryClass = {cs.CL} } ``` ```bibtex @misc
-{lu2019understanding, title = {Understanding and Improving Transformer From a
-Multi-Particle Dynamic System Point of View}, author = {Yiping Lu and Zhuohan
-Li and Di He and Zhiqing Sun and Bin Dong and Tao Qin and Liwei Wang and Tie-
-Yan Liu}, year = {2019}, eprint = {1906.02762}, archivePrefix = {arXiv},
-primaryClass = {cs.LG} } ``` ```bibtex @misc{ke2020rethinking, title =
-{Rethinking Positional Encoding in Language Pre-training}, author = {Guolin Ke
-and Di He and Tie-Yan Liu}, year = {2020}, eprint = {2006.15595}, archivePrefix
-= {arXiv}, primaryClass = {cs.CL} } ``` ```bibtex @misc{dosovitskiy2020image,
-title = {An Image is Worth 16x16 Words: Transformers for Image Recognition at
-Scale}, author = {Alexey Dosovitskiy and Lucas Beyer and Alexander Kolesnikov
-and Dirk Weissenborn and Xiaohua Zhai and Thomas Unterthiner and Mostafa
-Dehghani and Matthias Minderer and Georg Heigold and Sylvain Gelly and Jakob
-Uszkoreit and Neil Houlsby}, year = {2020}, eprint = {2010.11929},
-archivePrefix = {arXiv}, primaryClass = {cs.CV} } ``` ```bibtex @misc
-{huang2019attention, title = {Attention on Attention for Image Captioning},
-author = {Lun Huang and Wenmin Wang and Jie Chen and Xiao-Yong Wei}, year =
-{2019}, eprint = {1908.06954}, archivePrefix = {arXiv}, primaryClass = {cs.CV}
-} ``` ```bibtex @misc{raffel2020exploring, title = {Exploring the Limits of
-Transfer Learning with a Unified Text-to-Text Transformer}, author = {Colin
-Raffel and Noam Shazeer and Adam Roberts and Katherine Lee and Sharan Narang
-and Michael Matena and Yanqi Zhou and Wei Li and Peter J. Liu}, year = {2020},
-eprint = {1910.10683}, archivePrefix = {arXiv}, primaryClass = {cs.LG} } ```
-```bibtex @inproceedings{martins-etal-2020-sparse, title = "Sparse Text
-Generation", author = "Martins, Pedro Henrique and Marinho, Zita and Martins,
-Andr{\'e} F. T.", booktitle = "Proceedings of the 2020 Conference on Empirical
-Methods in Natural Language Processing (EMNLP)", month = nov, year = "2020",
-address = "Online", publisher = "Association for Computational Linguistics",
-url = "https://www.aclweb.org/anthology/2020.emnlp-main.348" } ``` ```bibtex
-@misc{he2020realformer, title = {RealFormer: Transformer Likes Residual
-Attention}, author = {Ruining He and Anirudh Ravula and Bhargav Kanagal and
-Joshua Ainslie}, year = {2020}, eprint = {2012.11747}, archivePrefix = {arXiv},
-primaryClass = {cs.LG} } ``` ```bibtex @misc{carion2020endtoend, title = {End-
-to-End Object Detection with Transformers}, author = {Nicolas Carion and
-Francisco Massa and Gabriel Synnaeve and Nicolas Usunier and Alexander Kirillov
-and Sergey Zagoruyko}, year = {2020}, eprint = {2005.12872}, archivePrefix =
-{arXiv}, primaryClass = {cs.CV} } ``` ```bibtex @misc{press2021ALiBi, title =
-{Train Short, Test Long: Attention with Linear Biases Enable Input Length
-Extrapolation}, author = {Ofir Press and Noah A. Smith and Mike Lewis}, year =
-{2021}, url = {https://ofir.io/train_short_test_long.pdf} } ``` ```bibtex @misc
-{parisotto2019stabilizing, title = {Stabilizing Transformers for Reinforcement
-Learning}, author = {Emilio Parisotto and H. Francis Song and Jack W. Rae and
-Razvan Pascanu and Caglar Gulcehre and Siddhant M. Jayakumar and Max Jaderberg
-and Raphael Lopez Kaufman and Aidan Clark and Seb Noury and Matthew M.
-Botvinick and Nicolas Heess and Raia Hadsell}, year = {2019}, eprint =
-{1910.06764}, archivePrefix = {arXiv}, primaryClass = {cs.LG} } ``` ```bibtex
-@misc{narang2021transformer, title = {Do Transformer Modifications Transfer
-Across Implementations and Applications?}, author = {Sharan Narang and Hyung
-Won Chung and Yi Tay and William Fedus and Thibault Fevry and Michael Matena
-and Karishma Malkan and Noah Fiedel and Noam Shazeer and Zhenzhong Lan and
-Yanqi Zhou and Wei Li and Nan Ding and Jake Marcus and Adam Roberts and Colin
-Raffel}, year = {2021}, eprint = {2102.11972}, archivePrefix = {arXiv},
-primaryClass = {cs.LG} } ``` ```bibtex @misc{zhang2019root, title = {Root Mean
-Square Layer Normalization}, author = {Biao Zhang and Rico Sennrich}, year =
-{2019}, eprint = {1910.07467}, archivePrefix = {arXiv}, primaryClass = {cs.LG}
-} ``` ```bibtex @misc{su2021roformer, title = {RoFormer: Enhanced Transformer
-with Rotary Position Embedding}, author = {Jianlin Su and Yu Lu and Shengfeng
-Pan and Bo Wen and Yunfeng Liu}, year = {2021}, eprint = {2104.09864},
-archivePrefix = {arXiv}, primaryClass = {cs.CL} } ``` ```bibtex @inproceedings
-{Sun2022ALT, title = {A Length-Extrapolatable Transformer}, author = {Yutao Sun
-and Li Dong and Barun Patra and Shuming Ma and Shaohan Huang and Alon Benhaim
-and Vishrav Chaudhary and Xia Song and Furu Wei}, year = {2022} } ``` ```bibtex
-@Article{AlphaFold2021, author = {Jumper, John and Evans, Richard and Pritzel,
+something similar to cosine sim attention in a_22B_parameter_model. In their
+papers, they have analysis showing that the normalization resulted in not only
+extra stability, but also better results in the end (due to less need to adjust
+learning rate when increasing parameter count). We are nearing the point of
+wiping out a source of transformer training instability with one simple
+intervention, in my opinion. The only slight difference in the paper is that
+they still have a learned scale across the feature dimension (per use of
+rmsnorm). Not sure how critical this is, but just to make sure we don't miss
+anything, I will include this here. You can use this by setting
+`qk_norm_dim_scale = True` ```python import torch from x_transformers import
+TransformerWrapper, Decoder model = TransformerWrapper( num_tokens = 20000,
+max_seq_len = 1024, attn_layers = Decoder( dim = 512, depth = 12, heads = 8,
+attn_qk_norm = True, attn_qk_norm_dim_scale = True # set this to True, in
+addition to `attn_qk_norm = True` ) ) x = torch.randint(0, 256, (1, 1024))
+model(x) ``` ### Turning off absolute positional embedding A number of papers
+have hinted that causal transformers (`Decoder`) can learn absolute positions
+in the absence of added embeddings of any sort. This was recently thoroughly
+investigated here. You can turn off the absolute positional embedding by
+setting `use_abs_pos_emb = False` in the `TransformerWrapper` Given PaLM, the
+trend going forward may be to forgo absolute positional embedding (again, for
+causal transformers only), and add relative positional embeddings with RoPE,
+ALiBi, etc. ```python import torch from x_transformers import
+TransformerWrapper, Decoder model = TransformerWrapper( num_tokens = 20000,
+max_seq_len = 1024, use_abs_pos_emb = False, # set this to False attn_layers =
+Decoder( dim = 512, depth = 6, heads = 8, ) ) x = torch.randint(0, 20000, (1,
+1024)) model(x) ``` ### Forgetful Causal Mask [./images/fcm.png] This_paper
+shows convincing results that one can combine masking (from masked language
+modeling) with autoregressive training, leading to significantly better
+results. You can use this by setting the `mask_prob` on the
+`AutoregressiveWrapper` class ```python import torch from x_transformers import
+TransformerWrapper, Decoder, AutoregressiveWrapper model = TransformerWrapper
+( num_tokens = 20000, max_seq_len = 1024, attn_layers = Decoder( dim = 512,
+depth = 12, heads = 8 ) ) model = AutoregressiveWrapper( model, mask_prob =
+0.15 # in paper, they use 15%, same as BERT ).cuda() # mock data x =
+torch.randint(0, 20000, (1, 1024)).cuda() # derive cross entropy loss, masking
+all taken care of loss = model(x) loss.backward() ``` ## Miscellaneous Cross
+Attention ```python import torch from x_transformers import Encoder,
+CrossAttender enc = Encoder(dim = 512, depth = 6) model = CrossAttender(dim =
+512, depth = 6) nodes = torch.randn(1, 1, 512) node_masks = torch.ones(1,
+1).bool() neighbors = torch.randn(1, 5, 512) neighbor_masks = torch.ones(1,
+5).bool() encoded_neighbors = enc(neighbors, mask = neighbor_masks) model
+(nodes, context = encoded_neighbors, mask = node_masks, context_mask =
+neighbor_masks) # (1, 1, 512) ``` Pass in continuous values ```python import
+torch from x_transformers import ContinuousTransformerWrapper, Decoder model =
+ContinuousTransformerWrapper( dim_in = 32, dim_out = 100, max_seq_len = 1024,
+attn_layers = Decoder( dim = 512, depth = 12, heads = 8 ) ) x = torch.randn((1,
+1024, 32)) model(x) # (1, 1024, 100) ``` You can also train a transformer that
+accepts continuous values autoregressively easily, in the same scheme as done
+successfully in this_paper ```python import torch from x_transformers import
+ContinuousTransformerWrapper, Decoder from x_transformers import
+ContinuousAutoregressiveWrapper model = ContinuousTransformerWrapper( dim_in =
+777, dim_out = 777, max_seq_len = 1024, attn_layers = Decoder( dim = 512, depth
+= 12, heads = 8 ) ) # wrap it with the continuous autoregressive wrapper model
+= ContinuousAutoregressiveWrapper(model) # mock data x = torch.randn((1, 1024,
+777)) mask = torch.ones(1, 1024).bool() # train on a lot of data above loss =
+model(x, mask = mask) loss.backward # then generate start_emb = torch.randn(1,
+777) generated = model.generate(start_emb, 17) # (17, 777) ``` ## Citations
+```bibtex @misc{vaswani2017attention, title = {Attention Is All You Need},
+author = {Ashish Vaswani and Noam Shazeer and Niki Parmar and Jakob Uszkoreit
+and Llion Jones and Aidan N. Gomez and Lukasz Kaiser and Illia Polosukhin},
+year = {2017}, eprint = {1706.03762}, archivePrefix = {arXiv}, primaryClass =
+{cs.CL} } ``` ```bibtex @article{DBLP:journals/corr/abs-1907-01470, author =
+{Sainbayar Sukhbaatar and Edouard Grave and Guillaume Lample and Herv{\'{e}} J
+{\'{e}}gou and Armand Joulin}, title = {Augmenting Self-attention with
+Persistent Memory}, journal = {CoRR}, volume = {abs/1907.01470}, year = {2019},
+url = {http://arxiv.org/abs/1907.01470} } ``` ```bibtex @article{1910.05895,
+author = {Toan Q. Nguyen and Julian Salazar}, title = {Transformers without
+Tears: Improving the Normalization of Self-Attention}, year = {2019}, eprint =
+{arXiv:1910.05895}, doi = {10.5281/zenodo.3525484}, } ``` ```bibtex @misc
+{shazeer2020glu, title = {GLU Variants Improve Transformer}, author = {Noam
+Shazeer}, year = {2020}, url = {https://arxiv.org/abs/2002.05202} } ```
+```bibtex @misc{bhojanapalli2020lowrank, title = {Low-Rank Bottleneck in Multi-
+head Attention Models}, author = {Srinadh Bhojanapalli and Chulhee Yun and
+Ankit Singh Rawat and Sashank J. Reddi and Sanjiv Kumar}, year = {2020}, eprint
+= {2002.07028} } ``` ```bibtex @misc{burtsev2020memory, title = {Memory
+Transformer}, author = {Mikhail S. Burtsev and Grigory V. Sapunov}, year =
+{2020}, eprint = {2006.11527}, archivePrefix = {arXiv}, primaryClass = {cs.CL}
+} ``` ```bibtex @misc{zhao2019explicit, title = {Explicit Sparse Transformer:
+Concentrated Attention Through Explicit Selection}, author = {Guangxiang Zhao
+and Junyang Lin and Zhiyuan Zhang and Xuancheng Ren and Qi Su and Xu Sun}, year
+= {2019}, eprint = {1912.11637}, archivePrefix = {arXiv}, primaryClass =
+{cs.CL} } ``` ```bibtex @misc{correia2019adaptively, title = {Adaptively Sparse
+Transformers}, author = {GonÃ§alo M. Correia and Vlad Niculae and AndrÃ© F. T.
+Martins}, year = {2019}, eprint = {1909.00015}, archivePrefix = {arXiv},
+primaryClass = {cs.CL} } ``` ```bibtex @misc{shazeer2020talkingheads, title =
+{Talking-Heads Attention}, author = {Noam Shazeer and Zhenzhong Lan and Youlong
+Cheng and Nan Ding and Le Hou}, year = {2020}, eprint = {2003.02436},
+archivePrefix = {arXiv}, primaryClass = {cs.LG} } ``` ```bibtex @misc
+{press2020improving, title = {Improving Transformer Models by Reordering their
+Sublayers}, author = {Ofir Press and Noah A. Smith and Omer Levy}, year =
+{2020}, eprint = {1911.03864}, archivePrefix = {arXiv}, primaryClass = {cs.CL}
+} ``` ```bibtex @misc{lu2019understanding, title = {Understanding and Improving
+Transformer From a Multi-Particle Dynamic System Point of View}, author =
+{Yiping Lu and Zhuohan Li and Di He and Zhiqing Sun and Bin Dong and Tao Qin
+and Liwei Wang and Tie-Yan Liu}, year = {2019}, eprint = {1906.02762},
+archivePrefix = {arXiv}, primaryClass = {cs.LG} } ``` ```bibtex @misc
+{ke2020rethinking, title = {Rethinking Positional Encoding in Language Pre-
+training}, author = {Guolin Ke and Di He and Tie-Yan Liu}, year = {2020},
+eprint = {2006.15595}, archivePrefix = {arXiv}, primaryClass = {cs.CL} } ```
+```bibtex @misc{dosovitskiy2020image, title = {An Image is Worth 16x16 Words:
+Transformers for Image Recognition at Scale}, author = {Alexey Dosovitskiy and
+Lucas Beyer and Alexander Kolesnikov and Dirk Weissenborn and Xiaohua Zhai and
+Thomas Unterthiner and Mostafa Dehghani and Matthias Minderer and Georg Heigold
+and Sylvain Gelly and Jakob Uszkoreit and Neil Houlsby}, year = {2020}, eprint
+= {2010.11929}, archivePrefix = {arXiv}, primaryClass = {cs.CV} } ``` ```bibtex
+@misc{huang2019attention, title = {Attention on Attention for Image
+Captioning}, author = {Lun Huang and Wenmin Wang and Jie Chen and Xiao-Yong
+Wei}, year = {2019}, eprint = {1908.06954}, archivePrefix = {arXiv},
+primaryClass = {cs.CV} } ``` ```bibtex @misc{raffel2020exploring, title =
+{Exploring the Limits of Transfer Learning with a Unified Text-to-Text
+Transformer}, author = {Colin Raffel and Noam Shazeer and Adam Roberts and
+Katherine Lee and Sharan Narang and Michael Matena and Yanqi Zhou and Wei Li
+and Peter J. Liu}, year = {2020}, eprint = {1910.10683}, archivePrefix =
+{arXiv}, primaryClass = {cs.LG} } ``` ```bibtex @inproceedings{martins-etal-
+2020-sparse, title = "Sparse Text Generation", author = "Martins, Pedro
+Henrique and Marinho, Zita and Martins, Andr{\'e} F. T.", booktitle =
+"Proceedings of the 2020 Conference on Empirical Methods in Natural Language
+Processing (EMNLP)", month = nov, year = "2020", address = "Online", publisher
+= "Association for Computational Linguistics", url = "https://www.aclweb.org/
+anthology/2020.emnlp-main.348" } ``` ```bibtex @misc{he2020realformer, title =
+{RealFormer: Transformer Likes Residual Attention}, author = {Ruining He and
+Anirudh Ravula and Bhargav Kanagal and Joshua Ainslie}, year = {2020}, eprint =
+{2012.11747}, archivePrefix = {arXiv}, primaryClass = {cs.LG} } ``` ```bibtex
+@misc{carion2020endtoend, title = {End-to-End Object Detection with
+Transformers}, author = {Nicolas Carion and Francisco Massa and Gabriel
+Synnaeve and Nicolas Usunier and Alexander Kirillov and Sergey Zagoruyko}, year
+= {2020}, eprint = {2005.12872}, archivePrefix = {arXiv}, primaryClass =
+{cs.CV} } ``` ```bibtex @misc{press2021ALiBi, title = {Train Short, Test Long:
+Attention with Linear Biases Enable Input Length Extrapolation}, author = {Ofir
+Press and Noah A. Smith and Mike Lewis}, year = {2021}, url = {https://ofir.io/
+train_short_test_long.pdf} } ``` ```bibtex @misc{parisotto2019stabilizing,
+title = {Stabilizing Transformers for Reinforcement Learning}, author = {Emilio
+Parisotto and H. Francis Song and Jack W. Rae and Razvan Pascanu and Caglar
+Gulcehre and Siddhant M. Jayakumar and Max Jaderberg and Raphael Lopez Kaufman
+and Aidan Clark and Seb Noury and Matthew M. Botvinick and Nicolas Heess and
+Raia Hadsell}, year = {2019}, eprint = {1910.06764}, archivePrefix = {arXiv},
+primaryClass = {cs.LG} } ``` ```bibtex @misc{narang2021transformer, title = {Do
+Transformer Modifications Transfer Across Implementations and Applications?},
+author = {Sharan Narang and Hyung Won Chung and Yi Tay and William Fedus and
+Thibault Fevry and Michael Matena and Karishma Malkan and Noah Fiedel and Noam
+Shazeer and Zhenzhong Lan and Yanqi Zhou and Wei Li and Nan Ding and Jake
+Marcus and Adam Roberts and Colin Raffel}, year = {2021}, eprint =
+{2102.11972}, archivePrefix = {arXiv}, primaryClass = {cs.LG} } ``` ```bibtex
+@misc{zhang2019root, title = {Root Mean Square Layer Normalization}, author =
+{Biao Zhang and Rico Sennrich}, year = {2019}, eprint = {1910.07467},
+archivePrefix = {arXiv}, primaryClass = {cs.LG} } ``` ```bibtex @misc
+{su2021roformer, title = {RoFormer: Enhanced Transformer with Rotary Position
+Embedding}, author = {Jianlin Su and Yu Lu and Shengfeng Pan and Bo Wen and
+Yunfeng Liu}, year = {2021}, eprint = {2104.09864}, archivePrefix = {arXiv},
+primaryClass = {cs.CL} } ``` ```bibtex @inproceedings{Sun2022ALT, title = {A
+Length-Extrapolatable Transformer}, author = {Yutao Sun and Li Dong and Barun
+Patra and Shuming Ma and Shaohan Huang and Alon Benhaim and Vishrav Chaudhary
+and Xia Song and Furu Wei}, year = {2022} } ``` ```bibtex @Article
+{AlphaFold2021, author = {Jumper, John and Evans, Richard and Pritzel,
 Alexander and Green, Tim and Figurnov, Michael and Ronneberger, Olaf and
 Tunyasuvunakool, Kathryn and Bates, Russ and {\v{Z}}{\'\i}dek, Augustin and
 Potapenko, Anna and Bridgland, Alex and Meyer, Clemens and Kohl, Simon A A and
 Ballard, Andrew J and Cowie, Andrew and Romera-Paredes, Bernardino and Nikolov,
 Stanislav and Jain, Rishub and Adler, Jonas and Back, Trevor and Petersen, Stig
 and Reiman, David and Clancy, Ellen and Zielinski, Michal and Steinegger,
 Martin and Pacholska, Michalina and Berghammer, Tamas and Bodenstein, Sebastian
```

### Comparing `x-transformers-1.9.1/setup.py` & `x-transformers-1.9.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'x-transformers',
   packages = find_packages(exclude=['examples']),
-  version = '1.9.1',
+  version = '1.9.2',
   license='MIT',
   description = 'X-Transformers - Pytorch',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   url = 'https://github.com/lucidrains/x-transformers',
   long_description_content_type = 'text/markdown',
   keywords = [
```

### Comparing `x-transformers-1.9.1/x_transformers/autoregressive_wrapper.py` & `x-transformers-1.9.2/x_transformers/autoregressive_wrapper.py`

 * *Files identical despite different names*

### Comparing `x-transformers-1.9.1/x_transformers/continuous_autoregressive_wrapper.py` & `x-transformers-1.9.2/x_transformers/continuous_autoregressive_wrapper.py`

 * *Files identical despite different names*

### Comparing `x-transformers-1.9.1/x_transformers/nonautoregressive_wrapper.py` & `x-transformers-1.9.2/x_transformers/nonautoregressive_wrapper.py`

 * *Files identical despite different names*

### Comparing `x-transformers-1.9.1/x_transformers/x_transformers.py` & `x-transformers-1.9.2/x_transformers/x_transformers.py`

 * *Files 0% similar despite different names*

```diff
@@ -642,22 +642,21 @@
             nn.init.constant_(self.to_v_gate.bias, 1)
 
         # cosine sim attention
         self.qk_norm = qk_norm
         self.qk_norm_groups = qk_norm_groups
         self.qk_norm_scale = qk_norm_scale
 
-        # whether to use the rmsnorm (equivalent to cosine sim attention with learned scale on feature dimension) - https://arxiv.org/abs/2302.05442
+        # whether to use the rmsnorm (equivalent to cosine sim attention when scale is equal to 1) - https://arxiv.org/abs/2302.05442
         self.qk_norm_dim_scale = qk_norm_dim_scale
 
         self.qk_norm_q_scale = self.qk_norm_k_scale = 1
         if qk_norm and qk_norm_dim_scale:
-            self.qk_norm_q_scale = nn.Parameter(torch.ones(dim_head) * qk_norm_scale ** 0.5)
-            self.qk_norm_k_scale = nn.Parameter(torch.ones(dim_head) * qk_norm_scale ** 0.5)
-            self.qk_norm_scale = 1
+            self.qk_norm_q_scale = nn.Parameter(torch.ones(dim_head))
+            self.qk_norm_k_scale = nn.Parameter(torch.ones(dim_head))
 
         assert (not qk_norm) or (dim_head % qk_norm_groups) == 0, 'dimension per attention head must be divisible by the qk norm groups'
         assert not (qk_norm and (dim_head // qk_norm_groups) <= 2), 'the group dimension may be too small (2 was too small in my tests, but 4 still works, surprisingly)'
 
         # talking heads
         self.talking_heads = talking_heads
         if talking_heads:
```

### Comparing `x-transformers-1.9.1/x_transformers.egg-info/PKG-INFO` & `x-transformers-1.9.2/x_transformers.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: x-transformers
-Version: 1.9.1
+Version: 1.9.2
 Summary: X-Transformers - Pytorch
 Home-page: https://github.com/lucidrains/x-transformers
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,transformers
 Classifier: Development Status :: 4 - Beta
```

