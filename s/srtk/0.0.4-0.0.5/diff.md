# Comparing `tmp/srtk-0.0.4.tar.gz` & `tmp/srtk-0.0.5.tar.gz`

## Comparing `srtk-0.0.4.tar` & `srtk-0.0.5.tar`

### file list

```diff
@@ -1,81 +1,83 @@
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 srtk-0.0.4/.readthedocs.yaml
--rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 srtk-0.0.4/bs.py
--rw-r--r--   0        0        0    64070 2020-02-02 00:00:00.000000 srtk-0.0.4/coverage.svg
--rw-r--r--   0        0        0     7241 2020-02-02 00:00:00.000000 srtk-0.0.4/elegant_retrieve.py
--rw-r--r--   0        0        0    29013 2020-02-02 00:00:00.000000 srtk-0.0.4/experiments.ipynb
--rw-r--r--   0        0        0     3893 2020-02-02 00:00:00.000000 srtk-0.0.4/filter.ipynb
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 srtk-0.0.4/linked.jsonl
--rw-r--r--   0        0        0    75653 2020-02-02 00:00:00.000000 srtk-0.0.4/paper-graphs.ipynb
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 srtk-0.0.4/question.jsonl
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 srtk-0.0.4/readme.ipynb
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 srtk-0.0.4/requirements.txt
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 srtk-0.0.4/subgraph.jsonl
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 srtk-0.0.4/.github/workflows/pytest.yml
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 srtk-0.0.4/docs/Makefile
--rw-r--r--   0        0        0     9781 2020-02-02 00:00:00.000000 srtk-0.0.4/docs/cli.rst
--rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 srtk-0.0.4/docs/conf.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 srtk-0.0.4/docs/getting_started.md
--rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 srtk-0.0.4/docs/index.md
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 srtk-0.0.4/docs/install.md
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 srtk-0.0.4/docs/make.bat
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 srtk-0.0.4/docs/requirements.txt
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 srtk-0.0.4/docs/srtk.knowledge_graph.rst
--rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 srtk-0.0.4/docs/srtk.preprocessing.rst
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 srtk-0.0.4/docs/srtk.rst
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 srtk-0.0.4/docs/srtk.scorer.rst
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 srtk-0.0.4/docs/tutorials.md
--rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 srtk-0.0.4/docs/setups/setup_freebase.md
--rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 srtk-0.0.4/docs/setups/setup_qendpoint_rootless.md
--rw-r--r--   0        0        0     3918 2020-02-02 00:00:00.000000 srtk-0.0.4/docs/setups/setup_wikidata.md
--rw-r--r--   0        0        0    64488 2020-02-02 00:00:00.000000 srtk-0.0.4/examples/srtk_retrieve.svg
--rw-r--r--   0        0        0     7877 2020-02-02 00:00:00.000000 srtk-0.0.4/right-samples/mkqa_-252130520118561472.html
--rw-r--r--   0        0        0     4459 2020-02-02 00:00:00.000000 srtk-0.0.4/right-samples/mkqa_-4482246352718211871.html
--rw-r--r--   0        0        0     7345 2020-02-02 00:00:00.000000 srtk-0.0.4/right-samples/mkqa_-5779087988204512933.html
--rw-r--r--   0        0        0     6383 2020-02-02 00:00:00.000000 srtk-0.0.4/right-samples/mkqa_-7896195082647149010.html
--rw-r--r--   0        0        0     4510 2020-02-02 00:00:00.000000 srtk-0.0.4/right-samples/mkqa_164657081694304046.html
--rw-r--r--   0        0        0     7213 2020-02-02 00:00:00.000000 srtk-0.0.4/right-samples/mkqa_2009481386569838770.html
--rw-r--r--   0        0        0     6149 2020-02-02 00:00:00.000000 srtk-0.0.4/right-samples/mkqa_5967381679542830494.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 srtk-0.0.4/src/srtk/__init__.py
--rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 srtk-0.0.4/src/srtk/cli.py
--rw-r--r--   0        0        0     3444 2020-02-02 00:00:00.000000 srtk-0.0.4/src/srtk/link.py
--rw-r--r--   0        0        0     5521 2020-02-02 00:00:00.000000 srtk-0.0.4/src/srtk/preprocess.py
--rw-r--r--   0        0        0    15809 2020-02-02 00:00:00.000000 srtk-0.0.4/src/srtk/retrieve.py
--rw-r--r--   0        0        0     6596 2020-02-02 00:00:00.000000 srtk-0.0.4/src/srtk/train.py
--rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 srtk-0.0.4/src/srtk/utils.py
--rw-r--r--   0        0        0     4726 2020-02-02 00:00:00.000000 srtk-0.0.4/src/srtk/visualize.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 srtk-0.0.4/src/srtk/entity_linking/__init__.py
--rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 srtk-0.0.4/src/srtk/entity_linking/dbpedia.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 srtk-0.0.4/src/srtk/entity_linking/freebase.py
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 srtk-0.0.4/src/srtk/entity_linking/linker_base.py
--rw-r--r--   0        0        0     2077 2020-02-02 00:00:00.000000 srtk-0.0.4/src/srtk/entity_linking/wikidata.py
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 srtk-0.0.4/src/srtk/knowledge_graph/__init__.py
--rw-r--r--   0        0        0     8061 2020-02-02 00:00:00.000000 srtk-0.0.4/src/srtk/knowledge_graph/dbpedia.py
--rw-r--r--   0        0        0     8254 2020-02-02 00:00:00.000000 srtk-0.0.4/src/srtk/knowledge_graph/freebase.py
--rw-r--r--   0        0        0     2877 2020-02-02 00:00:00.000000 srtk-0.0.4/src/srtk/knowledge_graph/graph_base.py
--rw-r--r--   0        0        0    10620 2020-02-02 00:00:00.000000 srtk-0.0.4/src/srtk/knowledge_graph/wikidata.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 srtk-0.0.4/src/srtk/preprocessing/__init__.py
--rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 srtk-0.0.4/src/srtk/preprocessing/load_dataset.py
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 srtk-0.0.4/src/srtk/preprocessing/merge_ground.py
--rw-r--r--   0        0        0    10223 2020-02-02 00:00:00.000000 srtk-0.0.4/src/srtk/preprocessing/negative_sampling.py
--rw-r--r--   0        0        0     4111 2020-02-02 00:00:00.000000 srtk-0.0.4/src/srtk/preprocessing/score_path.py
--rw-r--r--   0        0        0     3786 2020-02-02 00:00:00.000000 srtk-0.0.4/src/srtk/preprocessing/search_path.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 srtk-0.0.4/src/srtk/scorer/__init__.py
--rw-r--r--   0        0        0    10741 2020-02-02 00:00:00.000000 srtk-0.0.4/src/srtk/scorer/encoder.py
--rw-r--r--   0        0        0     3400 2020-02-02 00:00:00.000000 srtk-0.0.4/src/srtk/scorer/scorer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 srtk-0.0.4/tests/__init__.py
--rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 srtk-0.0.4/tests/test_dbpedia.py
--rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 srtk-0.0.4/tests/test_encoder.py
--rw-r--r--   0        0        0     2991 2020-02-02 00:00:00.000000 srtk-0.0.4/tests/test_freebase.py
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 srtk-0.0.4/tests/test_link.py
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 srtk-0.0.4/tests/test_scorer.py
--rw-r--r--   0        0        0     2617 2020-02-02 00:00:00.000000 srtk-0.0.4/tests/test_wikidata.py
--rw-r--r--   0        0        0    25547 2020-02-02 00:00:00.000000 srtk-0.0.4/tutorials/2.end_to_end_subgraph_retrieval.ipynb
--rw-r--r--   0        0        0    24937 2020-02-02 00:00:00.000000 srtk-0.0.4/tutorials/3.weak_train_wikidata.ipynb
--rw-r--r--   0        0        0    17127 2020-02-02 00:00:00.000000 srtk-0.0.4/tutorials/4.weak_train_freebase.ipynb
--rw-r--r--   0        0        0    22909 2020-02-02 00:00:00.000000 srtk-0.0.4/tutorials/5.supervised_train_wikidata.ipynb
--rw-r--r--   0        0        0    16988 2020-02-02 00:00:00.000000 srtk-0.0.4/tutorials/6.extend_to_new_kg.ipynb
--rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 srtk-0.0.4/.gitignore
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 srtk-0.0.4/LICENSE
--rw-r--r--   0        0        0     5707 2020-02-02 00:00:00.000000 srtk-0.0.4/README.md
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 srtk-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     6520 2020-02-02 00:00:00.000000 srtk-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 srtk-0.0.5/.readthedocs.yaml
+-rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 srtk-0.0.5/bs.py
+-rw-r--r--   0        0        0    64070 2020-02-02 00:00:00.000000 srtk-0.0.5/coverage.svg
+-rw-r--r--   0        0        0     7241 2020-02-02 00:00:00.000000 srtk-0.0.5/elegant_retrieve.py
+-rw-r--r--   0        0        0    29013 2020-02-02 00:00:00.000000 srtk-0.0.5/experiments.ipynb
+-rw-r--r--   0        0        0     3893 2020-02-02 00:00:00.000000 srtk-0.0.5/filter.ipynb
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 srtk-0.0.5/linked.jsonl
+-rw-r--r--   0        0        0    75653 2020-02-02 00:00:00.000000 srtk-0.0.5/paper-graphs.ipynb
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 srtk-0.0.5/question.jsonl
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 srtk-0.0.5/readme.ipynb
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 srtk-0.0.5/requirements.txt
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 srtk-0.0.5/subgraph.jsonl
+-rw-r--r--   0        0        0    12586 2020-02-02 00:00:00.000000 srtk-0.0.5/train_dbpedia.ipynb
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 srtk-0.0.5/.github/workflows/pytest.yml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 srtk-0.0.5/docs/Makefile
+-rw-r--r--   0        0        0    10189 2020-02-02 00:00:00.000000 srtk-0.0.5/docs/cli.rst
+-rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 srtk-0.0.5/docs/conf.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 srtk-0.0.5/docs/getting_started.md
+-rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 srtk-0.0.5/docs/index.md
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 srtk-0.0.5/docs/install.md
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 srtk-0.0.5/docs/make.bat
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 srtk-0.0.5/docs/requirements.txt
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 srtk-0.0.5/docs/srtk.knowledge_graph.rst
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 srtk-0.0.5/docs/srtk.preprocessing.rst
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 srtk-0.0.5/docs/srtk.rst
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 srtk-0.0.5/docs/srtk.scorer.rst
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 srtk-0.0.5/docs/tutorials.md
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 srtk-0.0.5/docs/setups/setup_freebase.md
+-rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 srtk-0.0.5/docs/setups/setup_qendpoint_rootless.md
+-rw-r--r--   0        0        0     3918 2020-02-02 00:00:00.000000 srtk-0.0.5/docs/setups/setup_wikidata.md
+-rw-r--r--   0        0        0    64488 2020-02-02 00:00:00.000000 srtk-0.0.5/examples/srtk_retrieve.svg
+-rw-r--r--   0        0        0     7877 2020-02-02 00:00:00.000000 srtk-0.0.5/right-samples/mkqa_-252130520118561472.html
+-rw-r--r--   0        0        0     4459 2020-02-02 00:00:00.000000 srtk-0.0.5/right-samples/mkqa_-4482246352718211871.html
+-rw-r--r--   0        0        0     7345 2020-02-02 00:00:00.000000 srtk-0.0.5/right-samples/mkqa_-5779087988204512933.html
+-rw-r--r--   0        0        0     6383 2020-02-02 00:00:00.000000 srtk-0.0.5/right-samples/mkqa_-7896195082647149010.html
+-rw-r--r--   0        0        0     4510 2020-02-02 00:00:00.000000 srtk-0.0.5/right-samples/mkqa_164657081694304046.html
+-rw-r--r--   0        0        0     7213 2020-02-02 00:00:00.000000 srtk-0.0.5/right-samples/mkqa_2009481386569838770.html
+-rw-r--r--   0        0        0     6149 2020-02-02 00:00:00.000000 srtk-0.0.5/right-samples/mkqa_5967381679542830494.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 srtk-0.0.5/src/srtk/__init__.py
+-rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 srtk-0.0.5/src/srtk/cli.py
+-rw-r--r--   0        0        0     3444 2020-02-02 00:00:00.000000 srtk-0.0.5/src/srtk/link.py
+-rw-r--r--   0        0        0     5521 2020-02-02 00:00:00.000000 srtk-0.0.5/src/srtk/preprocess.py
+-rw-r--r--   0        0        0    15833 2020-02-02 00:00:00.000000 srtk-0.0.5/src/srtk/retrieve.py
+-rw-r--r--   0        0        0     6596 2020-02-02 00:00:00.000000 srtk-0.0.5/src/srtk/train.py
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 srtk-0.0.5/src/srtk/utils.py
+-rw-r--r--   0        0        0     4708 2020-02-02 00:00:00.000000 srtk-0.0.5/src/srtk/visualize.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 srtk-0.0.5/src/srtk/entity_linking/__init__.py
+-rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 srtk-0.0.5/src/srtk/entity_linking/dbpedia.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 srtk-0.0.5/src/srtk/entity_linking/freebase.py
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 srtk-0.0.5/src/srtk/entity_linking/linker_base.py
+-rw-r--r--   0        0        0     2077 2020-02-02 00:00:00.000000 srtk-0.0.5/src/srtk/entity_linking/wikidata.py
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 srtk-0.0.5/src/srtk/knowledge_graph/__init__.py
+-rw-r--r--   0        0        0     8552 2020-02-02 00:00:00.000000 srtk-0.0.5/src/srtk/knowledge_graph/dbpedia.py
+-rw-r--r--   0        0        0     8254 2020-02-02 00:00:00.000000 srtk-0.0.5/src/srtk/knowledge_graph/freebase.py
+-rw-r--r--   0        0        0     2877 2020-02-02 00:00:00.000000 srtk-0.0.5/src/srtk/knowledge_graph/graph_base.py
+-rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 srtk-0.0.5/src/srtk/knowledge_graph/utils.py
+-rw-r--r--   0        0        0    10620 2020-02-02 00:00:00.000000 srtk-0.0.5/src/srtk/knowledge_graph/wikidata.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 srtk-0.0.5/src/srtk/preprocessing/__init__.py
+-rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 srtk-0.0.5/src/srtk/preprocessing/load_dataset.py
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 srtk-0.0.5/src/srtk/preprocessing/merge_ground.py
+-rw-r--r--   0        0        0    10288 2020-02-02 00:00:00.000000 srtk-0.0.5/src/srtk/preprocessing/negative_sampling.py
+-rw-r--r--   0        0        0     4094 2020-02-02 00:00:00.000000 srtk-0.0.5/src/srtk/preprocessing/score_path.py
+-rw-r--r--   0        0        0     3769 2020-02-02 00:00:00.000000 srtk-0.0.5/src/srtk/preprocessing/search_path.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 srtk-0.0.5/src/srtk/scorer/__init__.py
+-rw-r--r--   0        0        0    10741 2020-02-02 00:00:00.000000 srtk-0.0.5/src/srtk/scorer/encoder.py
+-rw-r--r--   0        0        0     3400 2020-02-02 00:00:00.000000 srtk-0.0.5/src/srtk/scorer/scorer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 srtk-0.0.5/tests/__init__.py
+-rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 srtk-0.0.5/tests/test_dbpedia.py
+-rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 srtk-0.0.5/tests/test_encoder.py
+-rw-r--r--   0        0        0     2991 2020-02-02 00:00:00.000000 srtk-0.0.5/tests/test_freebase.py
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 srtk-0.0.5/tests/test_link.py
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 srtk-0.0.5/tests/test_scorer.py
+-rw-r--r--   0        0        0     2617 2020-02-02 00:00:00.000000 srtk-0.0.5/tests/test_wikidata.py
+-rw-r--r--   0        0        0    25547 2020-02-02 00:00:00.000000 srtk-0.0.5/tutorials/2.end_to_end_subgraph_retrieval.ipynb
+-rw-r--r--   0        0        0    24937 2020-02-02 00:00:00.000000 srtk-0.0.5/tutorials/3.weak_train_wikidata.ipynb
+-rw-r--r--   0        0        0    17127 2020-02-02 00:00:00.000000 srtk-0.0.5/tutorials/4.weak_train_freebase.ipynb
+-rw-r--r--   0        0        0    22909 2020-02-02 00:00:00.000000 srtk-0.0.5/tutorials/5.supervised_train_wikidata.ipynb
+-rw-r--r--   0        0        0    16988 2020-02-02 00:00:00.000000 srtk-0.0.5/tutorials/6.extend_to_new_kg.ipynb
+-rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 srtk-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 srtk-0.0.5/LICENSE
+-rw-r--r--   0        0        0     5811 2020-02-02 00:00:00.000000 srtk-0.0.5/README.md
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 srtk-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     6624 2020-02-02 00:00:00.000000 srtk-0.0.5/PKG-INFO
```

### Comparing `srtk-0.0.4/.readthedocs.yaml` & `srtk-0.0.5/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `srtk-0.0.4/bs.py` & `srtk-0.0.5/bs.py`

 * *Files identical despite different names*

### Comparing `srtk-0.0.4/coverage.svg` & `srtk-0.0.5/coverage.svg`

 * *Files identical despite different names*

### Comparing `srtk-0.0.4/elegant_retrieve.py` & `srtk-0.0.5/elegant_retrieve.py`

 * *Files identical despite different names*

### Comparing `srtk-0.0.4/experiments.ipynb` & `srtk-0.0.5/experiments.ipynb`

 * *Files identical despite different names*

### Comparing `srtk-0.0.4/filter.ipynb` & `srtk-0.0.5/filter.ipynb`

 * *Files identical despite different names*

### Comparing `srtk-0.0.4/paper-graphs.ipynb` & `srtk-0.0.5/paper-graphs.ipynb`

 * *Files identical despite different names*

### Comparing `srtk-0.0.4/readme.ipynb` & `srtk-0.0.5/readme.ipynb`

 * *Files identical despite different names*

### Comparing `srtk-0.0.4/.github/workflows/pytest.yml` & `srtk-0.0.5/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `srtk-0.0.4/docs/Makefile` & `srtk-0.0.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `srtk-0.0.4/docs/cli.rst` & `srtk-0.0.5/docs/cli.rst`

 * *Files 21% similar despite different names*

```diff
@@ -10,42 +10,44 @@
 Create the training data to train a retriever from the grounded questions.
 
 Usage: 
 
 .. code-block:: bash
 
  srtk preprocess [-h] -i INPUT -o OUTPUT [--intermediate-dir INTERMEDIATE_DIR]
-                 -e SPARQL_ENDPOINT -kg {wikidata,freebase} [--search-path]
+                 -e SPARQL_ENDPOINT -kg {wikidata,freebase,dbpedia} [--search-path]
                  [--metric {jaccard,recall}] [--num-negative NUM_NEGATIVE]
                  [--positive-threshold POSITIVE_THRESHOLD]
 
 Options:
 
   -h, --help            show this help message and exit
   -i INPUT, --input INPUT
                         The grounded questions file with question, question & answer entities
   -o OUTPUT, --output OUTPUT
                         The output path where the final training data will be saved.
   --intermediate-dir INTERMEDIATE_DIR
-                        The directory to save intermediate files. If not specified, the intermediate files will be saved in the same directory as the
-                        output file, with the name paths.jsonl and scores.jsonl
+                        The directory to save intermediate files. If not specified, the intermediate files will be saved in the
+                        same directory as the output file, with the name paths.jsonl and scores.jsonl
   -e SPARQL_ENDPOINT, --sparql-endpoint SPARQL_ENDPOINT
-                        SPARQL endpoint URL for either Wikidata or Freebase (e.g., 'http://localhost:1234/api/endpoint/sparql' for default local
-                        qEndpoint)
-  -kg {wikidata,freebase}, --knowledge-graph {wikidata,freebase}
+                        SPARQL endpoint URL for either Wikidata or Freebase (e.g., 'http://localhost:1234/api/endpoint/sparql' for
+                        default local qEndpoint)
+  -kg {wikidata,freebase,dbpedia}, --knowledge-graph {wikidata,freebase,dbpedia}
                         knowledge graph name, either wikidata or freebase
-  --search-path         Whether to search paths between question and answer entities. If not specified, paths and scores fields must present in the
-                        input file. You **have to** specify this for weakly supervised learning. (default: False)
+  --search-path         Whether to search paths between question and answer entities. If not specified, paths and scores fields
+                        must present in the input file. You **have to** specify this for weakly supervised learning. (default:
+                        False)
   --metric {jaccard,recall}
-                        The metric used to score the paths. recall will usually result in a lager size of training dataset. (default: jaccard))
+                        The metric used to score the paths. recall will usually result in a lager size of training dataset.
+                        (default: jaccard))
   --num-negative NUM_NEGATIVE
                         The number of negative relations to sample for each positive relation. (default: 15)
   --positive-threshold POSITIVE_THRESHOLD
-                        The threshold to determine whether a path is positive or negative. If you want to use a larger training dataset, you can set
-                        this value to a smaller value. (default: 0.5)
+                        The threshold to determine whether a path is positive or negative. If you want to use a larger training
+                        dataset, you can set this value to a smaller value. (default: 0.5)
 
 
 srtk train
 --------------
 
 Train a retriever model.
 
@@ -59,63 +61,68 @@
              [--batch-size BATCH_SIZE] [--max-epochs MAX_EPOCHS] [--accelerator ACCELERATOR]
              [--fast-dev-run]
 
 Options:
 
   -h, --help            show this help message and exit
   -t TRAIN_DATASET, --train-dataset TRAIN_DATASET
-                        path to the training dataset. It should be a JSONL file with fields:
-                        query, positive, negatives
+                        path to the training dataset. It should be a JSONL file with fields: query, positive, negatives
   -v VALIDATION_DATASET, --validation-dataset VALIDATION_DATASET
-                        path to the validation dataset. If not provided, 5 percent of the training
-                        data will be used as validation data. (default: None)
+                        path to the validation dataset. If not provided, 5 percent of the training data will be used as validation
+                        data. (default: None)
   -o OUTPUT_DIR, --output-dir OUTPUT_DIR
-                        output model path. the model will be saved in the format of huggingface
-                        models, which can be uploaded to the huggingface hub and shared with the
-                        community. (default: artifacts/scorer)
-  --model-name-or-path MODEL_NAME_OR_PATH
-                        pretrained model name or path. It is fully compatible with HuggingFace
-                        models. You can specify either a local path where a model is saved, or an
-                        encoder model identifier from huggingface hub. (default:
+                        output model path. the model will be saved in the format of huggingface models, which can be uploaded to
+                        the huggingface hub and shared with the community. (default: artifacts/scorer)
+  -m MODEL_NAME_OR_PATH, --model-name-or-path MODEL_NAME_OR_PATH
+                        pretrained model name or path. It is fully compatible with HuggingFace models. You can specify either a
+                        local path where a model is saved, or an encoder model identifier from huggingface hub. (default:
                         intfloat/e5-small)
   -lr LEARNING_RATE, --learning-rate LEARNING_RATE
                         learning rate (default: 5e-5)
   --batch-size BATCH_SIZE
                         batch size (default: 16)
+  --loss {cross_entropy,contrastive}
+                        loss function, can be cross_entropy or contrastive (default: cross_entropy)
   --max-epochs MAX_EPOCHS
                         max epochs (default: 10)
   --accelerator ACCELERATOR
                         accelerator, can be cpu, gpu, or tpu (default: gpu)
   --fast-dev-run        fast dev run for debugging, only use 1 batch for training and validation
+  --wandb-project WANDB_PROJECT
+                        wandb project name (default: retrieval)
+  --wandb-group WANDB_GROUP
+                        wandb group name (default: contrastive)
+  --wandb-savedir WANDB_SAVEDIR
+                        wandb save directory (default: artifacts)
 
 
 srtk link
 -------------------
 
 Entity linking. The input is a jsonl file. The field of interest is specified by the argument --ground-on. The output is a jsonl file, each line is a dict with keys: id,
 question_entities, spans, entity_names. Currently, only Wikidata is supported out of the box.
 
 Usage:
 
 .. code-block:: bash
 
-  srtk link [-h] [-i INPUT] [-o OUTPUT] [-e EL_ENDPOINT] [-kg {wikidata}]
+  srtk link [-h] [-i INPUT] [-o OUTPUT] [-e EL_ENDPOINT] [-kg {wikidata,dbpedia}]
             [--wikimapper-db WIKIMAPPER_DB] [--ground-on GROUND_ON]
 
 
 Options:
 
   -h, --help            show this help message and exit
   -i INPUT, --input INPUT
                         Input file path, in which the question is stored
   -o OUTPUT, --output OUTPUT
                         Output file path, in which the entity linking result is stored
   -e EL_ENDPOINT, --el-endpoint EL_ENDPOINT
-                        REL endpoint
-  -kg {wikidata}, --knowledge-graph {wikidata}
+                        Entity linking endpoint (default: http://127.0.0.1:1235 <local REL endpoint>)
+  -kg {wikidata,dbpedia}, --knowledge-graph {wikidata,dbpedia}
                         Knowledge graph to link to, only wikidata is supported now
   --wikimapper-db WIKIMAPPER_DB
                         Wikimapper database path
   --ground-on GROUND_ON
                         The key to ground on, the corresponding text will be sent to the REL endpoint for entity linking
 
 srtk retrieve
@@ -132,77 +139,69 @@
 
 
 
 Usage:
 
 .. code-block:: bash
 
-  srtk retrieve [-h] -i INPUT -o OUTPUT [-e SPARQL_ENDPOINT] -kg {freebase,wikidata}
-                --scorer-model-path SCORER_MODEL_PATH [--beam-width BEAM_WIDTH]
-                [--max-depth MAX_DEPTH] [--evaluate] [--include-qualifiers]
+  srtk retrieve [-h] -i INPUT -o OUTPUT [-e SPARQL_ENDPOINT] -kg {freebase,wikidata,dbpedia}
+                -m SCORER_MODEL_PATH [--beam-width BEAM_WIDTH] [--max-depth MAX_DEPTH]
+                [--evaluate] [--include-qualifiers]
 
 
 Options:
 
   -h, --help            show this help message and exit
   -i INPUT, --input INPUT
-                        path to input jsonl file. it should contain at least ``question`` and
-                        ``question_entities`` fields.
+                        path to input jsonl file. it should contain at least ``question`` and ``question_entities`` fields.
   -o OUTPUT, --output OUTPUT
                         output file path for storing retrieved triplets.
   -e SPARQL_ENDPOINT, --sparql-endpoint SPARQL_ENDPOINT
                         SPARQL endpoint for Wikidata or Freebase services.
-  -kg {freebase,wikidata}, --knowledge-graph {freebase,wikidata}
-                        choose the knowledge graph: currently supports ``freebase`` and
-                        ``wikidata``.
-  --scorer-model-path SCORER_MODEL_PATH
-                        Path to the scorer model, containing both the saved model and its
-                        tokenizer in the Huggingface models format. Such a model is saved
-                        automatically when using the ``srtk train`` command. Alternatively,
-                        provide a pre-trained model name from the Hugging Face model hub. In
-                        practice it supports any Huggingface transformers encoder model, though
-                        models that do not use [CLS] tokens may require modifications on
+  -kg {freebase,wikidata,dbpedia}, --knowledge-graph {freebase,wikidata,dbpedia}
+                        choose the knowledge graph: currently supports ``freebase``, ``wikidata`` and ``dbpedia``.
+  -m SCORER_MODEL_PATH, --scorer-model-path SCORER_MODEL_PATH
+                        Path to the scorer model, containing both the saved model and its tokenizer in the Huggingface models
+                        format. Such a model is saved automatically when using the ``srtk train`` command. Alternatively, provide
+                        a pre-trained model name from the Hugging Face model hub. In practice it supports any Huggingface
+                        transformers encoder model, though models that do not use [CLS] tokens may require modifications on
                         similarity function.
   --beam-width BEAM_WIDTH
                         beam width for beam search (default: 10).
   --max-depth MAX_DEPTH
                         maximum depth for beam search (default: 2).
-  --evaluate            Evaluate the retriever model. When the answer entities are known, the
-                        recall can be evluated as the number of samples that any of the answer
-                        entities are retrieved in the subgraph by the number of all samples. This
-                        equires `answer_entities` field in the input jsonl.
-  --include-qualifiers  Include qualifiers from the retrieved triplets. Qualifiers are
-                        informations represented in non-entity form, like date, count etc. This is
-                        only relevant for Wikidata.
+  --evaluate            Evaluate the retriever model. When the answer entities are known, the recall can be evluated as the number
+                        of samples that any of the answer entities are retrieved in the subgraph by the number of all samples.
+                        This equires `answer_entities` field in the input jsonl.
+  --include-qualifiers  Include qualifiers from the retrieved triplets. Qualifiers are informations represented in non-entity
+                        form, like date, count etc. This is only relevant for Wikidata.
 
 
 srtk visualize
 ------------------
 
 Visualize the graph (represented as a set of triplets) using pyvis.
 
 
 Usage:
 
 .. code-block:: bash
 
-  srtk visualize [-h] -i INPUT -o OUTPUT_DIR [-e SPARQL_ENDPOINT] [-kg {wikidata,freebase}]
-                 [--max-output MAX_OUTPUT]
+  srtk visualize [-h] -i INPUT -o OUTPUT_DIR [-e SPARQL_ENDPOINT]
+                 [-kg {wikidata,freebase,dbpedia}][--max-output MAX_OUTPUT]
 
 
 
 Options:
 
   -h, --help            show this help message and exit
   -i INPUT, --input INPUT
                         The input subgraph file path.
   -o OUTPUT_DIR, --output-dir OUTPUT_DIR
                         The output directory path.
   -e SPARQL_ENDPOINT, --sparql-endpoint SPARQL_ENDPOINT
-                        SPARQL endpoint for Wikidata or Freebase services. In this step, it is
-                        used to get the labels of entities. (Default:
-                        http://localhost:1234/api/endpoint/sparql)
-  -kg {wikidata,freebase}, --knowledge-graph {wikidata,freebase}
+                        SPARQL endpoint for Wikidata or Freebase services. In this step, it is used to get the labels of entities.
+                        (Default: http://localhost:1234/api/endpoint/sparql)
+  -kg {wikidata,freebase,dbpedia}, --knowledge-graph {wikidata,freebase,dbpedia}
                         The knowledge graph type to use. (Default: wikidata)
   --max-output MAX_OUTPUT
-                        The maximum number of graphs to output. This is useful for debugging.
-                        (Default: 1000)
+                        The maximum number of graphs to output. This is useful for debugging. (Default: 1000)
```

### Comparing `srtk-0.0.4/docs/conf.py` & `srtk-0.0.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `srtk-0.0.4/docs/index.md` & `srtk-0.0.5/docs/index.md`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 - `train`: Train a subgraph retrieval model on a preprocessed dataset.
 - `link`: Link entity mentions in a text to a knowledge graph. Currently only Wikidata is supported out of the box.
 - `retrieve`: Retrieve a semantic-relevant subgraph from a knowledge graph with a trained retriever. It can also be used to evaluate a trained retriever.
 - `visualize`: Visualize a retrieved subgraph using a graph visualization tool.
 
 ```{toctree}
 :caption: 'Contents:'
+:maxdepth: 2
 
 getting_started
 cli
 ```
 
 Besides, `srtk` can also be used as a python library.
```

### Comparing `srtk-0.0.4/docs/make.bat` & `srtk-0.0.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `srtk-0.0.4/docs/srtk.knowledge_graph.rst` & `srtk-0.0.5/docs/srtk.knowledge_graph.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 srtk.knowledge\_graph package
 =============================
 
-Submodules
-----------
 
 srtk.knowledge\_graph.freebase module
 -------------------------------------
 
 .. automodule:: srtk.knowledge_graph.freebase
    :members:
    :undoc-members:
@@ -24,14 +22,7 @@
 -------------------------------------
 
 .. automodule:: srtk.knowledge_graph.wikidata
    :members:
    :undoc-members:
    :show-inheritance:
 
-Module contents
----------------
-
-.. automodule:: srtk.knowledge_graph
-   :members:
-   :undoc-members:
-   :show-inheritance:
```

### Comparing `srtk-0.0.4/docs/srtk.preprocessing.rst` & `srtk-0.0.5/docs/srtk.preprocessing.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 srtk.preprocessing package
 ==========================
 
-Submodules
-----------
 
 srtk.preprocessing.load\_dataset module
 ---------------------------------------
 
 .. automodule:: srtk.preprocessing.load_dataset
    :members:
    :undoc-members:
@@ -39,15 +37,7 @@
 srtk.preprocessing.search\_path module
 --------------------------------------
 
 .. automodule:: srtk.preprocessing.search_path
    :members:
    :undoc-members:
    :show-inheritance:
-
-Module contents
----------------
-
-.. automodule:: srtk.preprocessing
-   :members:
-   :undoc-members:
-   :show-inheritance:
```

### Comparing `srtk-0.0.4/docs/srtk.rst` & `srtk-0.0.5/docs/srtk.rst`

 * *Files 8% similar despite different names*

```diff
@@ -7,16 +7,14 @@
 .. toctree::
    :maxdepth: 3
 
    srtk.knowledge_graph
    srtk.preprocessing
    srtk.scorer
 
-Submodules
-----------
 
 srtk.link\_wikidata module
 --------------------------
 
 .. automodule:: srtk.link
    :members:
 
@@ -40,14 +38,8 @@
    :undoc-members:
    :show-inheritance:
 
 srtk.visualize module
 ---------------------
 
 .. automodule:: srtk.visualize
-   :members:
-
-Module contents
----------------
-
-.. automodule:: srtk
    :members:
```

### Comparing `srtk-0.0.4/docs/tutorials.md` & `srtk-0.0.5/docs/tutorials.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # Tutorials
 
 We also provide tutorials in the form of jupyter notebooks.
 
 - [End-to-end Subgraph Retrieval](https://github.com/happen2me/subgraph-retrieval-toolkit/blob/main/tutorials/2.end_to_end_subgraph_retrieval.ipynb)
 - [Train a Retriever on Wikidata with Weak Supervision](https://github.com/happen2me/subgraph-retrieval-toolkit/blob/main/tutorials/3.weak_train_wikidata.ipynb)
 - [Train a Retriever on Freebase with Weak Supervision](https://github.com/happen2me/subgraph-retrieval-toolkit/blob/main/tutorials/4.weak_train_freebase.ipynb)
-- [Supervised Training with Wikidata Simple Questions](https://github.com/happen2me/subgraph-retrieval-toolkit/blob/main/tutorials/5.supervised_train_wikidata.ipynb)
+- [Supervised Training with Wikidata Simple Questions](https://github.com/happen2me/subgraph-retrieval-toolkit/blob/main/tutorials/5.supervised_train_wikidata.ipynb)
+- [Extend SRTK to other Knowledge Graphs](https://github.com/happen2me/subgraph-retrieval-toolkit/blob/main/tutorials/6.extend_to_new_kg.ipynb)
```

### Comparing `srtk-0.0.4/docs/setups/setup_freebase.md` & `srtk-0.0.5/docs/setups/setup_freebase.md`

 * *Files identical despite different names*

### Comparing `srtk-0.0.4/docs/setups/setup_qendpoint_rootless.md` & `srtk-0.0.5/docs/setups/setup_qendpoint_rootless.md`

 * *Files identical despite different names*

### Comparing `srtk-0.0.4/docs/setups/setup_wikidata.md` & `srtk-0.0.5/docs/setups/setup_wikidata.md`

 * *Files identical despite different names*

### Comparing `srtk-0.0.4/examples/srtk_retrieve.svg` & `srtk-0.0.5/examples/srtk_retrieve.svg`

 * *Files identical despite different names*

### Comparing `srtk-0.0.4/right-samples/mkqa_-252130520118561472.html` & `srtk-0.0.5/right-samples/mkqa_-252130520118561472.html`

 * *Files identical despite different names*

### Comparing `srtk-0.0.4/right-samples/mkqa_-4482246352718211871.html` & `srtk-0.0.5/right-samples/mkqa_-4482246352718211871.html`

 * *Files identical despite different names*

### Comparing `srtk-0.0.4/right-samples/mkqa_-5779087988204512933.html` & `srtk-0.0.5/right-samples/mkqa_-5779087988204512933.html`

 * *Files identical despite different names*

### Comparing `srtk-0.0.4/right-samples/mkqa_-7896195082647149010.html` & `srtk-0.0.5/right-samples/mkqa_-7896195082647149010.html`

 * *Files identical despite different names*

### Comparing `srtk-0.0.4/right-samples/mkqa_164657081694304046.html` & `srtk-0.0.5/right-samples/mkqa_164657081694304046.html`

 * *Files identical despite different names*

### Comparing `srtk-0.0.4/right-samples/mkqa_2009481386569838770.html` & `srtk-0.0.5/right-samples/mkqa_2009481386569838770.html`

 * *Files identical despite different names*

### Comparing `srtk-0.0.4/right-samples/mkqa_5967381679542830494.html` & `srtk-0.0.5/right-samples/mkqa_5967381679542830494.html`

 * *Files identical despite different names*

### Comparing `srtk-0.0.4/src/srtk/cli.py` & `srtk-0.0.5/src/srtk/cli.py`

 * *Files identical despite different names*

### Comparing `srtk-0.0.4/src/srtk/link.py` & `srtk-0.0.5/src/srtk/link.py`

 * *Files identical despite different names*

### Comparing `srtk-0.0.4/src/srtk/preprocess.py` & `srtk-0.0.5/src/srtk/preprocess.py`

 * *Files identical despite different names*

### Comparing `srtk-0.0.4/src/srtk/retrieve.py` & `srtk-0.0.5/src/srtk/retrieve.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,17 +16,16 @@
 from collections import namedtuple
 from typing import List, Any, Dict
 
 import srsly
 import torch
 from tqdm import tqdm
 
-from .knowledge_graph import KnowledgeGraphBase
+from .knowledge_graph import KnowledgeGraphBase, get_knowledge_graph
 from .scorer import Scorer
-from .utils import get_knowledge_graph
 
 
 END_REL = 'END OF HOP'
 
 
 # Path collects the information at each traversal step
 # - prev_relations stores the relations that have been traversed
@@ -111,15 +110,15 @@
         Args:
             identifier (str): the identifier of an entity or a relation
 
         Returns:
             str: the label of the entity or the relation
         """
         # For freebase, the relation identifier contains enough information
-        if self.kg.name == 'freebase':
+        if self.kg.name == 'freebase' or self.kg.name == 'dbpedia':
             return identifier
         if identifier == END_REL:
             return END_REL
         label =  self.kg.get_label(identifier)
         if label is None:
             return identifier
         return label
@@ -314,15 +313,15 @@
     When ``--evaluate`` is set, a metric file will also be saved to the same directory as the output JSONL file.
     '''
     parser.add_argument('-i', '--input', type=str, required=True, help='path to input jsonl file. it should contain at least \
                         ``question`` and ``question_entities`` fields.')
     parser.add_argument('-o', '--output', type=str, required=True, help='output file path for storing retrieved triplets.')
     parser.add_argument('-e', '--sparql-endpoint', type=str, help='SPARQL endpoint for Wikidata or Freebase services.')
     parser.add_argument('-kg', '--knowledge-graph', type=str, required=True, choices=('freebase', 'wikidata', 'dbpedia'),
-                        help='choose the knowledge graph: currently supports ``freebase`` and ``wikidata``.')
+                        help='choose the knowledge graph: currently supports ``freebase``, ``wikidata`` and ``dbpedia``.')
     parser.add_argument('-m', '--scorer-model-path', type=str, required=True, help='Path to the scorer model, containing \
                         both the saved model and its tokenizer in the Huggingface models format.\
                         Such a model is saved automatically when using the ``srtk train`` command.\
                         Alternatively, provide a pre-trained model name from the Hugging Face model hub.\
                         In practice it supports any Huggingface transformers encoder model, though models that do not use [CLS] \
                         tokens may require modifications on similarity function.')
     parser.add_argument('--beam-width', type=int, default=10, help='beam width for beam search (default: 10).')
```

### Comparing `srtk-0.0.4/src/srtk/train.py` & `srtk-0.0.5/src/srtk/train.py`

 * *Files identical despite different names*

### Comparing `srtk-0.0.4/src/srtk/visualize.py` & `srtk-0.0.5/src/srtk/visualize.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,15 @@
 from pathlib import Path
 
 import srsly
 from pyvis.network import Network
 from tqdm import tqdm
 from bs4 import BeautifulSoup as Soup
 
-from .knowledge_graph import KnowledgeGraphBase
-from .utils import get_knowledge_graph
+from .knowledge_graph import KnowledgeGraphBase, get_knowledge_graph
 
 
 def visualize_subgraph(sample, kg: KnowledgeGraphBase):
     """Visualize the subgraph. It returns an html string.
     """
     net = Network(directed=True, font_color='#000000')
     net.barnes_hut()
```

### Comparing `srtk-0.0.4/src/srtk/entity_linking/dbpedia.py` & `srtk-0.0.5/src/srtk/entity_linking/dbpedia.py`

 * *Files identical despite different names*

### Comparing `srtk-0.0.4/src/srtk/entity_linking/linker_base.py` & `srtk-0.0.5/src/srtk/entity_linking/linker_base.py`

 * *Files identical despite different names*

### Comparing `srtk-0.0.4/src/srtk/entity_linking/wikidata.py` & `srtk-0.0.5/src/srtk/entity_linking/wikidata.py`

 * *Files identical despite different names*

### Comparing `srtk-0.0.4/src/srtk/knowledge_graph/dbpedia.py` & `srtk-0.0.5/src/srtk/knowledge_graph/dbpedia.py`

 * *Files 5% similar despite different names*

```diff
@@ -70,14 +70,28 @@
                 }}
                 """
         paths = self.queryDBPedia(query)
         # Keep only identifiers in the paths
         paths = [[self.get_id_from_uri(path['r1']['value']), self.get_id_from_uri(path['r2']['value'])] for path in paths]
         return paths
 
+    def escape_entity(self, entity):
+        """Escape brackets in the entity ID.
+
+        Args:
+            entity (str): entity identifier
+
+        Returns:
+            str: the bracket-escaped entity identifier
+        """
+        # entity = entity.replace('(', r'\(').replace(')', r'\)')
+        entity = entity.replace('"', r'\"')
+        entity = f"<http://dbpedia.org/resource/{entity}>"
+        return entity
+
     def deduce_leaves(self, src: str, path: List[str], limit: int) -> List[str]:
         """Deduce leave entities from source entity following the path.
 
         Args:
             src_entity (str): source entity
             path (tuple[str]): path from source entity to destination entity
             limit (int, optional): limit of the number of leaves.
@@ -86,27 +100,28 @@
             list[str]: list of leaves. Each leaf is a ID.
         """
         if len(path) > 3:
             raise NotImplementedError('Deduce leaves for paths longer than 3 is not implemented.')
         
         if len(path) == 0:
             return [src]
-        
+
+        src = self.escape_entity(src)
         if len(path) == 1:
             query = f"""
                 SELECT DISTINCT ?dst WHERE {{
-                    dbr:{src} dbo:{path[0]} ?dst.
+                    {src} dbo:{path[0]} ?dst.
                     FILTER(STRSTARTS(str(?dst), "http://dbpedia.org/resource/"))
                 }}
                 LIMIT {limit}
                 """
         else:
             query = f"""
                 SELECT DISTINCT ?dst WHERE {{
-                    dbr:{src} dbo:{path[0]} ?mid.
+                    {src} dbo:{path[0]} ?mid.
                     ?mid dbo:{path[1]} ?dst.
                     FILTER(STRSTARTS(str(?dst), "http://dbpedia.org/resource/"))
                 }}
                 LIMIT {limit}
                 """
         leaves = self.queryDBPedia(query)
         leaves = [self.get_id_from_uri(leaf['dst']['value']) for leaf in leaves]
@@ -126,17 +141,18 @@
         if len(path) >= 2:
             raise NotImplementedError(f'Currenly only support paths with length less than 2, got {len(path)}')
         if len(path) == 0:
             return srcs
         if len(srcs) == 0:
             return []
 
+        srcs = [self.escape_entity(src) for src in srcs]
         query = f"""
             SELECT DISTINCT ?x WHERE {{
-                VALUES ?src {{dbr:{' dbr:'.join(srcs)}}}
+                VALUES ?src {{ {' '.join(srcs)} }}
                 ?src dbo:{path[0]} ?x.
                 FILTER(STRSTARTS(str(?x), "http://dbpedia.org/resource/"))
             }}
             LIMIT {limit}
             """
         if self.prepend_prefixes:
             query = self.PREFIXES + query
```

### Comparing `srtk-0.0.4/src/srtk/knowledge_graph/freebase.py` & `srtk-0.0.5/src/srtk/knowledge_graph/freebase.py`

 * *Files identical despite different names*

### Comparing `srtk-0.0.4/src/srtk/knowledge_graph/graph_base.py` & `srtk-0.0.5/src/srtk/knowledge_graph/graph_base.py`

 * *Files identical despite different names*

### Comparing `srtk-0.0.4/src/srtk/knowledge_graph/wikidata.py` & `srtk-0.0.5/src/srtk/knowledge_graph/wikidata.py`

 * *Files identical despite different names*

### Comparing `srtk-0.0.4/src/srtk/preprocessing/load_dataset.py` & `srtk-0.0.5/src/srtk/preprocessing/load_dataset.py`

 * *Files identical despite different names*

### Comparing `srtk-0.0.4/src/srtk/preprocessing/merge_ground.py` & `srtk-0.0.5/src/srtk/preprocessing/merge_ground.py`

 * *Files identical despite different names*

### Comparing `srtk-0.0.4/src/srtk/preprocessing/negative_sampling.py` & `srtk-0.0.5/src/srtk/preprocessing/negative_sampling.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 from collections import defaultdict
 from functools import lru_cache
 
 import srsly
 from tqdm import tqdm
 
 sys.path.append(os.path.abspath(os.path.join(os.path.dirname(__file__), '..', )))
-from knowledge_graph import KnowledgeGraphBase
-from utils import get_knowledge_graph
+from knowledge_graph import KnowledgeGraphBase, get_knowledge_graph
+
 
 END_REL = "END OF HOP"
 
 
 def sample_negative_relations(soruce_entities, prev_path, positive_connections,
                               num_negative, kg: KnowledgeGraphBase):
     """A helper function to sample negative relations.
@@ -140,14 +140,16 @@
 def convert_records_relation_id_to_lable(records, kg):
     """Convert relation ids to relation labels in each record.
     """
     processed_records = []
 
     @lru_cache
     def get_label(rel):
+        if kg.name == 'dbpedia' or kg.name == 'freebase':
+            return rel
         if rel == END_REL:
             return END_REL
         return kg.get_relation_label(rel) or rel
 
     for record in tqdm(records, desc='Converting relation ids to labels'):
         record['prev_path'] = [get_label(rel) for rel in record['prev_path']]
         record['positive_relation'] = get_label(record['positive_relation'])
```

### Comparing `srtk-0.0.4/src/srtk/preprocessing/score_path.py` & `srtk-0.0.5/src/srtk/preprocessing/score_path.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,16 +17,15 @@
 import sys
 import argparse
 
 import srsly
 from tqdm import tqdm
 
 sys.path.append(os.path.abspath(os.path.join(os.path.dirname(__file__), '..', )))
-from knowledge_graph import KnowledgeGraphBase
-from utils import get_knowledge_graph
+from knowledge_graph import KnowledgeGraphBase, get_knowledge_graph
 
 
 def score_path(kg: KnowledgeGraphBase, src, path, answers, metric='jaccard'):
     """Calculate the HIT score of a given path.
     
     Args:
         kg (KnowledgeGraphBase): knowledge graph instance
```

### Comparing `srtk-0.0.4/src/srtk/preprocessing/search_path.py` & `srtk-0.0.5/src/srtk/preprocessing/search_path.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,16 +9,15 @@
 import os
 import argparse
 
 import srsly
 from tqdm import tqdm
 
 sys.path.append(os.path.abspath(os.path.join(os.path.dirname(__file__), '..', )))
-from knowledge_graph import KnowledgeGraphBase
-from utils import get_knowledge_graph
+from knowledge_graph import KnowledgeGraphBase, get_knowledge_graph
 
 
 def generate_paths(src_entities, dst_entities, kg: KnowledgeGraphBase, max_path=50):
     """Generate paths from question entities to answer entities.
     """
     paths = []
     for src in src_entities:
```

### Comparing `srtk-0.0.4/src/srtk/scorer/encoder.py` & `srtk-0.0.5/src/srtk/scorer/encoder.py`

 * *Files identical despite different names*

### Comparing `srtk-0.0.4/src/srtk/scorer/scorer.py` & `srtk-0.0.5/src/srtk/scorer/scorer.py`

 * *Files identical despite different names*

### Comparing `srtk-0.0.4/tests/test_dbpedia.py` & `srtk-0.0.5/tests/test_dbpedia.py`

 * *Files identical despite different names*

### Comparing `srtk-0.0.4/tests/test_encoder.py` & `srtk-0.0.5/tests/test_encoder.py`

 * *Files identical despite different names*

### Comparing `srtk-0.0.4/tests/test_freebase.py` & `srtk-0.0.5/tests/test_freebase.py`

 * *Files identical despite different names*

### Comparing `srtk-0.0.4/tests/test_link.py` & `srtk-0.0.5/tests/test_link.py`

 * *Files identical despite different names*

### Comparing `srtk-0.0.4/tests/test_scorer.py` & `srtk-0.0.5/tests/test_scorer.py`

 * *Files identical despite different names*

### Comparing `srtk-0.0.4/tests/test_wikidata.py` & `srtk-0.0.5/tests/test_wikidata.py`

 * *Files identical despite different names*

### Comparing `srtk-0.0.4/tutorials/2.end_to_end_subgraph_retrieval.ipynb` & `srtk-0.0.5/tutorials/2.end_to_end_subgraph_retrieval.ipynb`

 * *Files identical despite different names*

### Comparing `srtk-0.0.4/tutorials/3.weak_train_wikidata.ipynb` & `srtk-0.0.5/tutorials/3.weak_train_wikidata.ipynb`

 * *Files identical despite different names*

### Comparing `srtk-0.0.4/tutorials/4.weak_train_freebase.ipynb` & `srtk-0.0.5/tutorials/4.weak_train_freebase.ipynb`

 * *Files identical despite different names*

### Comparing `srtk-0.0.4/tutorials/5.supervised_train_wikidata.ipynb` & `srtk-0.0.5/tutorials/5.supervised_train_wikidata.ipynb`

 * *Files identical despite different names*

### Comparing `srtk-0.0.4/tutorials/6.extend_to_new_kg.ipynb` & `srtk-0.0.5/tutorials/6.extend_to_new_kg.ipynb`

 * *Files identical despite different names*

### Comparing `srtk-0.0.4/.gitignore` & `srtk-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `srtk-0.0.4/LICENSE` & `srtk-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `srtk-0.0.4/README.md` & `srtk-0.0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 [![PyPi](https://img.shields.io/pypi/v/srtk)](https://pypi.org/project/srtk/)
 [![Documentation Status](https://readthedocs.org/projects/srtk/badge/?version=latest)](https://srtk.readthedocs.io/en/latest/?badge=latest)
 [![PytestStatus](https://github.com/happen2me/subgraph-retrieval-wikidata/actions/workflows/pytest.yml/badge.svg)](https://github.com/happen2me/subgraph-retrieval-toolkit/actions/workflows/pytest.yml)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![DOI](https://zenodo.org/badge/622648166.svg)](https://zenodo.org/badge/latestdoi/622648166)
 
 
-**SRTK** is a toolkit for semantic-relevant subgraph retrieval from large-scale knowledge graphs. It currently supports Wikidata, Freebase and DBPedia.
+**SRTK** is a toolkit for semantic-relevant subgraph retrieval from large-scale knowledge graphs. It currently supports Wikidata, Freebase and DBpedia.
 
 A minimum walkthrough of the retrieve process:
 
 ![retrieve example](examples/srtk_retrieve.svg)
 
 <img width="400rem" src="https://i.imgur.com/jG7nZuo.png" alt="Visualized subgraph"/>
 
@@ -21,24 +21,25 @@
 
 ```bash
 pip install srtk
 ```
 
 ### Local Deployment of Knowledge Graphs
 
-- [Setup Wikidata locally](https://srtk.readthedocs.io/en/latest/setup_wikidata.html)
-- [Setup Freebase locally](https://srtk.readthedocs.io/en/latest/setup_freebase.html)
+- [Setup Wikidata locally](https://srtk.readthedocs.io/en/latest/setups/setup_wikidata.html)
+- [Setup Freebase locally](https://srtk.readthedocs.io/en/latest/setups/setup_freebase.html)
+- [Setup DBpedia locally](https://github.com/dbpedia/virtuoso-sparql-endpoint-quickstart)
 
 ## Usage
 
 There are mainly five subcommands of SRTK, which covers the whole pipeline of subgraph retrieval.
 
 For retrieval:
 
-- `srtk link`: Link entity mentions in texts to a knowledge graph. Currently Wikidata and DBPedia are supported out of the box.
+- `srtk link`: Link entity mentions in texts to a knowledge graph. Currently Wikidata and DBpedia are supported out of the box.
 - `srtk retrieve`: Retrieve semantic-relevant subgraphs from a knowledge graph with a trained retriever. It can also be used to evaluate a trained retriever.
 - `srtk visualize`: Visualize retrieved subgraphs using a graph visualization tool.
 
 For training a retriever:
 
 - `srtk preprocess`: Preprocess a dataset for training a subgraph retrieval model.
 - `srtk train`: Train a subgraph retrieval model on a preprocessed dataset.
```

### Comparing `srtk-0.0.4/pyproject.toml` & `srtk-0.0.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "hatch-requirements-txt"]
 build-backend = "hatchling.build"
 
 [project]
 name = "srtk"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Yuanchun Shen", email="y.c.shen@tum.de" },
 ]
 description = "A toolkit for semantic-relevant subgraph retrieval from large-scale knowledge graphs."
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `srtk-0.0.4/PKG-INFO` & `srtk-0.0.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: srtk
-Version: 0.0.4
+Version: 0.0.5
 Summary: A toolkit for semantic-relevant subgraph retrieval from large-scale knowledge graphs.
 Project-URL: Homepage, https://github.com/happen2me/subgraph-retrieval-toolkit
 Project-URL: Bug Tracker, https://github.com/happen2me/subgraph-retrieval-toolkit/issues
 Author-email: Yuanchun Shen <y.c.shen@tum.de>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -26,15 +26,15 @@
 [![PyPi](https://img.shields.io/pypi/v/srtk)](https://pypi.org/project/srtk/)
 [![Documentation Status](https://readthedocs.org/projects/srtk/badge/?version=latest)](https://srtk.readthedocs.io/en/latest/?badge=latest)
 [![PytestStatus](https://github.com/happen2me/subgraph-retrieval-wikidata/actions/workflows/pytest.yml/badge.svg)](https://github.com/happen2me/subgraph-retrieval-toolkit/actions/workflows/pytest.yml)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![DOI](https://zenodo.org/badge/622648166.svg)](https://zenodo.org/badge/latestdoi/622648166)
 
 
-**SRTK** is a toolkit for semantic-relevant subgraph retrieval from large-scale knowledge graphs. It currently supports Wikidata, Freebase and DBPedia.
+**SRTK** is a toolkit for semantic-relevant subgraph retrieval from large-scale knowledge graphs. It currently supports Wikidata, Freebase and DBpedia.
 
 A minimum walkthrough of the retrieve process:
 
 ![retrieve example](examples/srtk_retrieve.svg)
 
 <img width="400rem" src="https://i.imgur.com/jG7nZuo.png" alt="Visualized subgraph"/>
 
@@ -44,24 +44,25 @@
 
 ```bash
 pip install srtk
 ```
 
 ### Local Deployment of Knowledge Graphs
 
-- [Setup Wikidata locally](https://srtk.readthedocs.io/en/latest/setup_wikidata.html)
-- [Setup Freebase locally](https://srtk.readthedocs.io/en/latest/setup_freebase.html)
+- [Setup Wikidata locally](https://srtk.readthedocs.io/en/latest/setups/setup_wikidata.html)
+- [Setup Freebase locally](https://srtk.readthedocs.io/en/latest/setups/setup_freebase.html)
+- [Setup DBpedia locally](https://github.com/dbpedia/virtuoso-sparql-endpoint-quickstart)
 
 ## Usage
 
 There are mainly five subcommands of SRTK, which covers the whole pipeline of subgraph retrieval.
 
 For retrieval:
 
-- `srtk link`: Link entity mentions in texts to a knowledge graph. Currently Wikidata and DBPedia are supported out of the box.
+- `srtk link`: Link entity mentions in texts to a knowledge graph. Currently Wikidata and DBpedia are supported out of the box.
 - `srtk retrieve`: Retrieve semantic-relevant subgraphs from a knowledge graph with a trained retriever. It can also be used to evaluate a trained retriever.
 - `srtk visualize`: Visualize retrieved subgraphs using a graph visualization tool.
 
 For training a retriever:
 
 - `srtk preprocess`: Preprocess a dataset for training a subgraph retrieval model.
 - `srtk train`: Train a subgraph retrieval model on a preprocessed dataset.
```

