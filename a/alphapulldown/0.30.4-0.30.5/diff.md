# Comparing `tmp/alphapulldown-0.30.4.tar.gz` & `tmp/alphapulldown-0.30.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alphapulldown-0.30.4.tar", last modified: Wed Apr  5 12:59:25 2023, max compression
+gzip compressed data, was "alphapulldown-0.30.5.tar", last modified: Mon May  8 11:31:44 2023, max compression
```

## Comparing `alphapulldown-0.30.4.tar` & `alphapulldown-0.30.5.tar`

### file list

```diff
@@ -1,152 +1,231 @@
-drwxr-xr-x   0    24600      721        0 2023-04-05 12:59:25.000000 alphapulldown-0.30.4/
--rw-r--r--   0    24600      721    35149 2022-08-09 10:02:13.000000 alphapulldown-0.30.4/LICENSE
--rw-r--r--   0    24600      721       39 2022-06-20 09:13:18.000000 alphapulldown-0.30.4/MANIFEST.in
--rw-r--r--   0    24600      721      428 2023-04-05 12:59:25.000000 alphapulldown-0.30.4/PKG-INFO
--rw-r--r--   0    24600      721     5261 2023-03-14 10:54:09.000000 alphapulldown-0.30.4/README.md
-drwxr-xr-x   0    24600      721        0 2023-04-05 12:58:35.000000 alphapulldown-0.30.4/alphapulldown/
-drwxr-xr-x   0    24600      721        0 2023-04-05 12:58:36.000000 alphapulldown-0.30.4/alphapulldown/analysis_pipeline/
--rw-r--r--   0    24600      721     5510 2023-01-27 13:03:03.000000 alphapulldown-0.30.4/alphapulldown/analysis_pipeline/create_notebook.py
--rwxr-xr-x   0    24600      721    10571 2023-04-05 12:41:41.000000 alphapulldown-0.30.4/alphapulldown/create_individual_features.py
--rwxr-xr-x   0    24600      721     1166 2023-03-14 16:09:44.000000 alphapulldown-0.30.4/alphapulldown/prepare_seq_names.py
--rwxr-xr-x   0    24600      721     1261 2023-03-14 16:09:44.000000 alphapulldown-0.30.4/alphapulldown/rename_colab_search_a3m.py
--rw-r--r--   0    24600      721    11187 2023-03-14 16:09:44.000000 alphapulldown-0.30.4/alphapulldown/run_multimer_jobs.py
--rw-r--r--   0    24600      721      140 2023-04-05 11:02:03.000000 alphapulldown-0.30.4/pyproject.toml
--rw-r--r--   0    24600      721     1064 2023-04-05 12:59:25.000000 alphapulldown-0.30.4/setup.cfg
--rw-r--r--   0    24600      721       36 2023-03-16 13:53:42.000000 alphapulldown-0.30.4/setup.py
-drwxr-xr-x   0    24600      721        0 2023-04-05 12:58:31.000000 alphapulldown-0.30.4/src/
-drwxr-xr-x   0    24600      721        0 2023-04-05 12:58:37.000000 alphapulldown-0.30.4/src/af2plots/
--rw-r--r--   0    24600      721        0 2022-08-03 11:05:46.000000 alphapulldown-0.30.4/src/af2plots/__init__.py
--rw-r--r--   0    24600      721    11001 2022-08-03 11:05:57.000000 alphapulldown-0.30.4/src/af2plots/plotter.py
-drwxr-xr-x   0    24600      721        0 2023-04-05 12:58:38.000000 alphapulldown-0.30.4/src/alphafold/
--rw-r--r--   0    24600      721      663 2023-04-04 09:47:45.000000 alphapulldown-0.30.4/src/alphafold/__init__.py
-drwxr-xr-x   0    24600      721        0 2023-04-05 12:58:40.000000 alphapulldown-0.30.4/src/alphafold/common/
--rw-r--r--   0    24600      721      655 2023-04-04 09:47:46.000000 alphapulldown-0.30.4/src/alphafold/common/__init__.py
--rw-r--r--   0    24600      721     6066 2023-04-04 09:47:46.000000 alphapulldown-0.30.4/src/alphafold/common/confidence.py
--rw-r--r--   0    24600      721     9959 2023-04-04 09:47:46.000000 alphapulldown-0.30.4/src/alphafold/common/protein.py
--rw-r--r--   0    24600      721     4594 2023-04-04 09:47:46.000000 alphapulldown-0.30.4/src/alphafold/common/protein_test.py
--rw-r--r--   0    24600      721    34974 2023-04-04 09:47:46.000000 alphapulldown-0.30.4/src/alphafold/common/residue_constants.py
--rw-r--r--   0    24600      721     9256 2023-04-04 09:47:47.000000 alphapulldown-0.30.4/src/alphafold/common/residue_constants_test.py
-drwxr-xr-x   0    24600      721        0 2023-04-05 12:58:43.000000 alphapulldown-0.30.4/src/alphafold/data/
--rw-r--r--   0    24600      721      634 2023-04-04 09:47:47.000000 alphapulldown-0.30.4/src/alphafold/data/__init__.py
--rw-r--r--   0    24600      721     8575 2023-04-04 09:47:48.000000 alphapulldown-0.30.4/src/alphafold/data/feature_processing.py
--rw-r--r--   0    24600      721    14182 2023-04-04 09:47:48.000000 alphapulldown-0.30.4/src/alphafold/data/mmcif_parsing.py
--rw-r--r--   0    24600      721     2966 2023-04-04 09:47:48.000000 alphapulldown-0.30.4/src/alphafold/data/msa_identifiers.py
--rw-r--r--   0    24600      721    17220 2023-04-04 09:47:48.000000 alphapulldown-0.30.4/src/alphafold/data/msa_pairing.py
--rw-r--r--   0    24600      721    21397 2023-04-04 09:47:48.000000 alphapulldown-0.30.4/src/alphafold/data/parsers.py
--rw-r--r--   0    24600      721    10419 2023-04-04 09:47:48.000000 alphapulldown-0.30.4/src/alphafold/data/pipeline.py
--rw-r--r--   0    24600      721    11126 2023-04-04 09:47:48.000000 alphapulldown-0.30.4/src/alphafold/data/pipeline_multimer.py
--rw-r--r--   0    24600      721    40677 2023-04-04 09:47:49.000000 alphapulldown-0.30.4/src/alphafold/data/templates.py
-drwxr-xr-x   0    24600      721        0 2023-04-05 12:58:47.000000 alphapulldown-0.30.4/src/alphafold/data/tools/
--rw-r--r--   0    24600      721      639 2023-04-04 09:47:49.000000 alphapulldown-0.30.4/src/alphafold/data/tools/__init__.py
--rw-r--r--   0    24600      721     5504 2023-04-04 09:47:49.000000 alphapulldown-0.30.4/src/alphafold/data/tools/hhblits.py
--rw-r--r--   0    24600      721     3601 2023-04-04 09:47:49.000000 alphapulldown-0.30.4/src/alphafold/data/tools/hhsearch.py
--rw-r--r--   0    24600      721     4576 2023-04-04 09:47:49.000000 alphapulldown-0.30.4/src/alphafold/data/tools/hmmbuild.py
--rw-r--r--   0    24600      721     4556 2023-04-04 09:47:50.000000 alphapulldown-0.30.4/src/alphafold/data/tools/hmmsearch.py
--rw-r--r--   0    24600      721     8386 2023-04-04 09:47:50.000000 alphapulldown-0.30.4/src/alphafold/data/tools/jackhmmer.py
--rw-r--r--   0    24600      721     3387 2023-04-04 09:47:50.000000 alphapulldown-0.30.4/src/alphafold/data/tools/kalign.py
--rw-r--r--   0    24600      721     1223 2023-04-04 09:47:50.000000 alphapulldown-0.30.4/src/alphafold/data/tools/utils.py
-drwxr-xr-x   0    24600      721        0 2023-04-05 12:58:56.000000 alphapulldown-0.30.4/src/alphafold/model/
--rw-r--r--   0    24600      721      617 2023-04-04 09:47:50.000000 alphapulldown-0.30.4/src/alphafold/model/__init__.py
--rw-r--r--   0    24600      721    47028 2023-04-04 09:47:51.000000 alphapulldown-0.30.4/src/alphafold/model/all_atom.py
--rw-r--r--   0    24600      721    40145 2023-04-04 09:47:51.000000 alphapulldown-0.30.4/src/alphafold/model/all_atom_multimer.py
--rw-r--r--   0    24600      721     4706 2023-04-04 09:47:51.000000 alphapulldown-0.30.4/src/alphafold/model/all_atom_test.py
--rw-r--r--   0    24600      721     5957 2023-04-04 09:47:51.000000 alphapulldown-0.30.4/src/alphafold/model/common_modules.py
--rw-r--r--   0    24600      721    26814 2023-04-04 09:47:51.000000 alphapulldown-0.30.4/src/alphafold/model/config.py
--rw-r--r--   0    24600      721     1097 2023-04-04 09:47:51.000000 alphapulldown-0.30.4/src/alphafold/model/data.py
--rw-r--r--   0    24600      721     3692 2023-04-04 09:47:52.000000 alphapulldown-0.30.4/src/alphafold/model/features.py
--rw-r--r--   0    24600      721    37264 2023-04-04 09:47:52.000000 alphapulldown-0.30.4/src/alphafold/model/folding.py
--rw-r--r--   0    24600      721    42498 2023-04-04 09:47:52.000000 alphapulldown-0.30.4/src/alphafold/model/folding_multimer.py
-drwxr-xr-x   0    24600      721        0 2023-04-05 12:58:58.000000 alphapulldown-0.30.4/src/alphafold/model/geometry/
--rw-r--r--   0    24600      721     1172 2023-04-04 09:47:52.000000 alphapulldown-0.30.4/src/alphafold/model/geometry/__init__.py
--rw-r--r--   0    24600      721     4148 2023-04-04 09:47:52.000000 alphapulldown-0.30.4/src/alphafold/model/geometry/rigid_matrix_vector.py
--rw-r--r--   0    24600      721     5751 2023-04-04 09:47:52.000000 alphapulldown-0.30.4/src/alphafold/model/geometry/rotation_matrix.py
--rw-r--r--   0    24600      721     7745 2023-04-04 09:47:53.000000 alphapulldown-0.30.4/src/alphafold/model/geometry/struct_of_array.py
--rw-r--r--   0    24600      721     4166 2023-04-04 09:47:53.000000 alphapulldown-0.30.4/src/alphafold/model/geometry/test_utils.py
--rw-r--r--   0    24600      721      853 2023-04-04 09:47:53.000000 alphapulldown-0.30.4/src/alphafold/model/geometry/utils.py
--rw-r--r--   0    24600      721     6896 2023-04-04 09:47:53.000000 alphapulldown-0.30.4/src/alphafold/model/geometry/vector.py
--rw-r--r--   0    24600      721     9134 2023-04-04 09:47:53.000000 alphapulldown-0.30.4/src/alphafold/model/layer_stack.py
--rw-r--r--   0    24600      721    10315 2023-04-04 09:47:53.000000 alphapulldown-0.30.4/src/alphafold/model/layer_stack_test.py
--rw-r--r--   0    24600      721     3505 2023-04-04 09:47:54.000000 alphapulldown-0.30.4/src/alphafold/model/lddt.py
--rw-r--r--   0    24600      721     2384 2023-04-04 09:47:54.000000 alphapulldown-0.30.4/src/alphafold/model/lddt_test.py
--rw-r--r--   0    24600      721     7963 2023-04-04 09:47:54.000000 alphapulldown-0.30.4/src/alphafold/model/mapping.py
--rw-r--r--   0    24600      721     6613 2023-04-04 09:47:54.000000 alphapulldown-0.30.4/src/alphafold/model/model.py
--rw-r--r--   0    24600      721    74120 2023-04-04 09:47:54.000000 alphapulldown-0.30.4/src/alphafold/model/modules.py
--rw-r--r--   0    24600      721    42228 2023-04-04 09:47:54.000000 alphapulldown-0.30.4/src/alphafold/model/modules_multimer.py
--rw-r--r--   0    24600      721     1978 2023-04-04 09:47:55.000000 alphapulldown-0.30.4/src/alphafold/model/prng.py
--rw-r--r--   0    24600      721     1250 2023-04-04 09:47:55.000000 alphapulldown-0.30.4/src/alphafold/model/prng_test.py
--rw-r--r--   0    24600      721    17388 2023-04-04 09:47:55.000000 alphapulldown-0.30.4/src/alphafold/model/quat_affine.py
--rw-r--r--   0    24600      721     5038 2023-04-04 09:47:55.000000 alphapulldown-0.30.4/src/alphafold/model/quat_affine_test.py
--rw-r--r--   0    24600      721    10935 2023-04-04 09:47:55.000000 alphapulldown-0.30.4/src/alphafold/model/r3.py
-drwxr-xr-x   0    24600      721        0 2023-04-05 12:59:02.000000 alphapulldown-0.30.4/src/alphafold/model/tf/
--rw-r--r--   0    24600      721      633 2023-04-04 09:47:55.000000 alphapulldown-0.30.4/src/alphafold/model/tf/__init__.py
--rw-r--r--   0    24600      721    21428 2023-04-04 09:47:56.000000 alphapulldown-0.30.4/src/alphafold/model/tf/data_transforms.py
--rw-r--r--   0    24600      721     5357 2023-04-04 09:47:56.000000 alphapulldown-0.30.4/src/alphafold/model/tf/input_pipeline.py
--rw-r--r--   0    24600      721     5051 2023-04-04 09:47:56.000000 alphapulldown-0.30.4/src/alphafold/model/tf/protein_features.py
--rw-r--r--   0    24600      721     1822 2023-04-04 09:47:56.000000 alphapulldown-0.30.4/src/alphafold/model/tf/protein_features_test.py
--rw-r--r--   0    24600      721     6344 2023-04-04 09:47:56.000000 alphapulldown-0.30.4/src/alphafold/model/tf/proteins_dataset.py
--rw-r--r--   0    24600      721     1415 2023-04-04 09:47:56.000000 alphapulldown-0.30.4/src/alphafold/model/tf/shape_helpers.py
--rw-r--r--   0    24600      721     1318 2023-04-04 09:47:57.000000 alphapulldown-0.30.4/src/alphafold/model/tf/shape_helpers_test.py
--rw-r--r--   0    24600      721      812 2023-04-04 09:47:57.000000 alphapulldown-0.30.4/src/alphafold/model/tf/shape_placeholders.py
--rw-r--r--   0    24600      721     1276 2023-04-04 09:47:57.000000 alphapulldown-0.30.4/src/alphafold/model/tf/utils.py
--rw-r--r--   0    24600      721     5328 2023-04-04 09:47:57.000000 alphapulldown-0.30.4/src/alphafold/model/utils.py
-drwxr-xr-x   0    24600      721        0 2023-04-05 12:59:03.000000 alphapulldown-0.30.4/src/alphafold/notebooks/
--rw-r--r--   0    24600      721      626 2023-04-04 09:47:57.000000 alphapulldown-0.30.4/src/alphafold/notebooks/__init__.py
--rw-r--r--   0    24600      721     7520 2023-04-04 09:47:58.000000 alphapulldown-0.30.4/src/alphafold/notebooks/notebook_utils.py
--rw-r--r--   0    24600      721     9571 2023-04-04 09:47:58.000000 alphapulldown-0.30.4/src/alphafold/notebooks/notebook_utils_test.py
-drwxr-xr-x   0    24600      721        0 2023-04-05 12:59:07.000000 alphapulldown-0.30.4/src/alphafold/relax/
--rw-r--r--   0    24600      721      618 2023-04-04 09:47:58.000000 alphapulldown-0.30.4/src/alphafold/relax/__init__.py
--rw-r--r--   0    24600      721    19061 2023-04-04 09:47:58.000000 alphapulldown-0.30.4/src/alphafold/relax/amber_minimize.py
--rw-r--r--   0    24600      721     4348 2023-04-04 09:47:58.000000 alphapulldown-0.30.4/src/alphafold/relax/amber_minimize_test.py
--rw-r--r--   0    24600      721     4832 2023-04-04 09:47:59.000000 alphapulldown-0.30.4/src/alphafold/relax/cleanup.py
--rw-r--r--   0    24600      721     6170 2023-04-04 09:47:59.000000 alphapulldown-0.30.4/src/alphafold/relax/cleanup_test.py
--rw-r--r--   0    24600      721     3288 2023-04-04 09:47:59.000000 alphapulldown-0.30.4/src/alphafold/relax/relax.py
--rw-r--r--   0    24600      721     3827 2023-04-04 09:47:59.000000 alphapulldown-0.30.4/src/alphafold/relax/relax_test.py
--rw-r--r--   0    24600      721     2501 2023-04-04 09:48:00.000000 alphapulldown-0.30.4/src/alphafold/relax/utils.py
--rw-r--r--   0    24600      721     1996 2023-04-04 09:48:00.000000 alphapulldown-0.30.4/src/alphafold/relax/utils_test.py
--rw-r--r--   0    24600      721    19606 2023-04-05 12:46:17.000000 alphapulldown-0.30.4/src/alphafold/run_alphafold.py
-drwxr-xr-x   0    24600      721        0 2023-04-05 12:59:14.000000 alphapulldown-0.30.4/src/alphapulldown/
--rw-r--r--   0    24600      721        0 2022-06-17 12:38:21.000000 alphapulldown-0.30.4/src/alphapulldown/__init__.py
--rw-r--r--   0    24600      721     3944 2023-04-03 15:02:10.000000 alphapulldown-0.30.4/src/alphapulldown/colab_batch_no_prediction.py
--rw-r--r--   0    24600      721    10571 2023-04-03 15:02:10.000000 alphapulldown-0.30.4/src/alphapulldown/create_individual_features.py
--rw-r--r--   0    24600      721    22205 2023-04-03 15:02:10.000000 alphapulldown-0.30.4/src/alphapulldown/objects.py
--rw-r--r--   0    24600      721     1822 2023-04-03 15:02:10.000000 alphapulldown-0.30.4/src/alphapulldown/plot_pae.py
--rw-r--r--   0    24600      721     7433 2023-04-03 15:02:11.000000 alphapulldown-0.30.4/src/alphapulldown/predict_structure.py
--rwxr-xr-x   0    24600      721     1166 2023-04-03 15:02:11.000000 alphapulldown-0.30.4/src/alphapulldown/prepare_seq_names.py
--rwxr-xr-x   0    24600      721     1261 2023-04-03 15:02:11.000000 alphapulldown-0.30.4/src/alphapulldown/rename_colab_search_a3m.py
--rw-r--r--   0    24600      721    11187 2023-04-03 15:02:11.000000 alphapulldown-0.30.4/src/alphapulldown/run_multimer_jobs.py
--rw-r--r--   0    24600      721       63 2023-04-03 15:02:11.000000 alphapulldown-0.30.4/src/alphapulldown/test_global.py
--rw-r--r--   0    24600      721    10992 2023-04-03 15:02:12.000000 alphapulldown-0.30.4/src/alphapulldown/utils.py
-drwxr-xr-x   0    24600      721        0 2023-04-05 12:59:16.000000 alphapulldown-0.30.4/src/alphapulldown.egg-info/
--rw-r--r--   0    24600      721      428 2023-04-05 12:58:25.000000 alphapulldown-0.30.4/src/alphapulldown.egg-info/PKG-INFO
--rw-r--r--   0    24600      721     4502 2023-04-05 12:58:26.000000 alphapulldown-0.30.4/src/alphapulldown.egg-info/SOURCES.txt
--rw-r--r--   0    24600      721        1 2023-04-05 12:58:25.000000 alphapulldown-0.30.4/src/alphapulldown.egg-info/dependency_links.txt
--rw-r--r--   0    24600      721      262 2023-04-05 12:58:26.000000 alphapulldown-0.30.4/src/alphapulldown.egg-info/requires.txt
--rw-r--r--   0    24600      721       61 2023-04-05 12:58:26.000000 alphapulldown-0.30.4/src/alphapulldown.egg-info/top_level.txt
-drwxr-xr-x   0    24600      721        0 2023-04-05 12:59:18.000000 alphapulldown-0.30.4/src/analysis_pipeline/
--rw-r--r--   0    24600      721        0 2022-07-11 13:06:01.000000 alphapulldown-0.30.4/src/analysis_pipeline/__init__.py
--rw-r--r--   0    24600      721     7268 2023-02-20 12:54:45.000000 alphapulldown-0.30.4/src/analysis_pipeline/af2_3dmol.py
--rw-rw-r--   0    24600      721     4967 2022-07-21 11:40:49.000000 alphapulldown-0.30.4/src/analysis_pipeline/calculate_mpdockq.py
--rw-r--r--   0    24600      721     5510 2022-10-13 12:19:42.000000 alphapulldown-0.30.4/src/analysis_pipeline/create_notebook.py
--rw-rw-r--   0    24600      721     6253 2022-08-02 12:32:15.000000 alphapulldown-0.30.4/src/analysis_pipeline/get_good_inter_pae.py
--rw-r--r--   0    24600      721      962 2022-08-29 13:35:59.000000 alphapulldown-0.30.4/src/analysis_pipeline/utils.py
-drwxr-xr-x   0    24600      721        0 2023-04-05 12:59:22.000000 alphapulldown-0.30.4/src/colabfold/
--rw-r--r--   0    24600      721        0 2022-09-22 14:05:14.000000 alphapulldown-0.30.4/src/colabfold/__init__.py
-drwxr-xr-x   0    24600      721        0 2023-04-05 12:59:23.000000 alphapulldown-0.30.4/src/colabfold/alphafold/
--rw-r--r--   0    24600      721        0 2022-09-22 14:05:14.000000 alphapulldown-0.30.4/src/colabfold/alphafold/__init__.py
--rw-r--r--   0    24600      721     5923 2022-09-22 14:05:14.000000 alphapulldown-0.30.4/src/colabfold/alphafold/models.py
--rw-r--r--   0    24600      721     1565 2022-09-22 14:05:14.000000 alphapulldown-0.30.4/src/colabfold/alphafold/msa.py
--rw-r--r--   0    24600      721    65347 2022-09-22 14:05:14.000000 alphapulldown-0.30.4/src/colabfold/batch.py
--rw-r--r--   0    24600      721     5988 2022-09-22 14:05:14.000000 alphapulldown-0.30.4/src/colabfold/citations.py
--rw-r--r--   0    24600      721    24980 2022-09-22 14:05:15.000000 alphapulldown-0.30.4/src/colabfold/colabfold.py
--rw-r--r--   0    24600      721    32656 2022-09-22 14:05:15.000000 alphapulldown-0.30.4/src/colabfold/colabfold_alphafold.py
--rw-r--r--   0    24600      721     1982 2022-09-22 14:05:15.000000 alphapulldown-0.30.4/src/colabfold/download.py
-drwxr-xr-x   0    24600      721        0 2023-04-05 12:59:24.000000 alphapulldown-0.30.4/src/colabfold/mmseqs/
--rw-r--r--   0    24600      721        0 2022-09-22 14:05:15.000000 alphapulldown-0.30.4/src/colabfold/mmseqs/__init__.py
--rw-r--r--   0    24600      721     1933 2022-09-22 14:05:15.000000 alphapulldown-0.30.4/src/colabfold/mmseqs/merge_and_split_msas.py
--rw-r--r--   0    24600      721    18799 2022-09-22 14:05:16.000000 alphapulldown-0.30.4/src/colabfold/mmseqs/search.py
--rw-r--r--   0    24600      721     1429 2022-09-22 14:05:16.000000 alphapulldown-0.30.4/src/colabfold/mmseqs/split_msas.py
--rw-r--r--   0    24600      721     2120 2022-09-22 14:05:16.000000 alphapulldown-0.30.4/src/colabfold/pdb.py
--rw-r--r--   0    24600      721     3419 2022-09-22 14:05:17.000000 alphapulldown-0.30.4/src/colabfold/plot.py
--rw-r--r--   0    24600      721     9954 2022-09-22 14:05:17.000000 alphapulldown-0.30.4/src/colabfold/utils.py
-drwxr-xr-x   0    24600      721        0 2023-04-05 12:59:24.000000 alphapulldown-0.30.4/test/
--rw-r--r--   0    24600      721     4546 2023-04-05 12:41:41.000000 alphapulldown-0.30.4/test/test_create_objects.py
+drwxr-xr-x   0    24600      721        0 2023-05-08 11:31:43.000000 alphapulldown-0.30.5/
+-rw-r--r--   0    24600      721    35149 2022-08-09 10:02:13.000000 alphapulldown-0.30.5/LICENSE
+-rw-r--r--   0    24600      721       70 2023-04-18 11:12:17.000000 alphapulldown-0.30.5/MANIFEST.in
+-rw-r--r--   0    24600      721      428 2023-05-08 11:31:43.000000 alphapulldown-0.30.5/PKG-INFO
+-rw-r--r--   0    24600      721     5265 2023-05-08 11:10:52.000000 alphapulldown-0.30.5/README.md
+drwxr-xr-x   0    24600      721        0 2023-05-08 11:30:16.000000 alphapulldown-0.30.5/alphafold/
+-rw-r--r--   0    24600      721      663 2023-04-19 11:33:22.000000 alphapulldown-0.30.5/alphafold/__init__.py
+drwxr-xr-x   0    24600      721        0 2023-05-08 11:30:16.000000 alphapulldown-0.30.5/alphafold/alphafold/
+-rw-r--r--   0    24600      721      663 2023-04-18 13:00:43.000000 alphapulldown-0.30.5/alphafold/alphafold/__init__.py
+drwxr-xr-x   0    24600      721        0 2023-05-08 11:30:19.000000 alphapulldown-0.30.5/alphafold/alphafold/common/
+-rw-r--r--   0    24600      721      655 2023-04-18 13:00:43.000000 alphapulldown-0.30.5/alphafold/alphafold/common/__init__.py
+-rw-r--r--   0    24600      721     6066 2023-04-18 13:00:44.000000 alphapulldown-0.30.5/alphafold/alphafold/common/confidence.py
+-rw-r--r--   0    24600      721     9959 2023-04-18 13:00:44.000000 alphapulldown-0.30.5/alphafold/alphafold/common/protein.py
+-rw-r--r--   0    24600      721     4594 2023-04-18 13:00:44.000000 alphapulldown-0.30.5/alphafold/alphafold/common/protein_test.py
+-rw-r--r--   0    24600      721    34974 2023-04-18 13:00:44.000000 alphapulldown-0.30.5/alphafold/alphafold/common/residue_constants.py
+-rw-r--r--   0    24600      721     9256 2023-04-18 13:00:44.000000 alphapulldown-0.30.5/alphafold/alphafold/common/residue_constants_test.py
+drwxr-xr-x   0    24600      721        0 2023-05-08 11:30:22.000000 alphapulldown-0.30.5/alphafold/alphafold/data/
+-rw-r--r--   0    24600      721      634 2023-04-18 13:00:45.000000 alphapulldown-0.30.5/alphafold/alphafold/data/__init__.py
+-rw-r--r--   0    24600      721     8575 2023-04-18 13:00:46.000000 alphapulldown-0.30.5/alphafold/alphafold/data/feature_processing.py
+-rw-r--r--   0    24600      721    14182 2023-04-18 13:00:46.000000 alphapulldown-0.30.5/alphafold/alphafold/data/mmcif_parsing.py
+-rw-r--r--   0    24600      721     3229 2023-04-18 13:11:35.000000 alphapulldown-0.30.5/alphafold/alphafold/data/msa_identifiers.py
+-rw-r--r--   0    24600      721    17220 2023-04-18 13:00:46.000000 alphapulldown-0.30.5/alphafold/alphafold/data/msa_pairing.py
+-rw-r--r--   0    24600      721    21397 2023-04-18 13:00:46.000000 alphapulldown-0.30.5/alphafold/alphafold/data/parsers.py
+-rw-r--r--   0    24600      721    10419 2023-04-18 13:00:46.000000 alphapulldown-0.30.5/alphafold/alphafold/data/pipeline.py
+-rw-r--r--   0    24600      721    11126 2023-04-18 13:00:47.000000 alphapulldown-0.30.5/alphafold/alphafold/data/pipeline_multimer.py
+-rw-r--r--   0    24600      721    40677 2023-04-18 13:00:47.000000 alphapulldown-0.30.5/alphafold/alphafold/data/templates.py
+drwxr-xr-x   0    24600      721        0 2023-05-08 11:30:26.000000 alphapulldown-0.30.5/alphafold/alphafold/data/tools/
+-rw-r--r--   0    24600      721      639 2023-04-18 13:00:47.000000 alphapulldown-0.30.5/alphafold/alphafold/data/tools/__init__.py
+-rw-r--r--   0    24600      721     5504 2023-04-18 13:00:47.000000 alphapulldown-0.30.5/alphafold/alphafold/data/tools/hhblits.py
+-rw-r--r--   0    24600      721     3601 2023-04-18 13:00:47.000000 alphapulldown-0.30.5/alphafold/alphafold/data/tools/hhsearch.py
+-rw-r--r--   0    24600      721     4576 2023-04-18 13:00:48.000000 alphapulldown-0.30.5/alphafold/alphafold/data/tools/hmmbuild.py
+-rw-r--r--   0    24600      721     4556 2023-04-18 13:00:48.000000 alphapulldown-0.30.5/alphafold/alphafold/data/tools/hmmsearch.py
+-rw-r--r--   0    24600      721     8386 2023-04-18 13:00:48.000000 alphapulldown-0.30.5/alphafold/alphafold/data/tools/jackhmmer.py
+-rw-r--r--   0    24600      721     3387 2023-04-18 13:00:48.000000 alphapulldown-0.30.5/alphafold/alphafold/data/tools/kalign.py
+-rw-r--r--   0    24600      721     1223 2023-04-18 13:00:48.000000 alphapulldown-0.30.5/alphafold/alphafold/data/tools/utils.py
+drwxr-xr-x   0    24600      721        0 2023-05-08 11:30:42.000000 alphapulldown-0.30.5/alphafold/alphafold/model/
+-rw-r--r--   0    24600      721      617 2023-04-18 13:00:48.000000 alphapulldown-0.30.5/alphafold/alphafold/model/__init__.py
+-rw-r--r--   0    24600      721    47028 2023-04-18 13:00:49.000000 alphapulldown-0.30.5/alphafold/alphafold/model/all_atom.py
+-rw-r--r--   0    24600      721    40145 2023-04-18 13:00:49.000000 alphapulldown-0.30.5/alphafold/alphafold/model/all_atom_multimer.py
+-rw-r--r--   0    24600      721     4706 2023-04-18 13:00:49.000000 alphapulldown-0.30.5/alphafold/alphafold/model/all_atom_test.py
+-rw-r--r--   0    24600      721     5957 2023-04-18 13:00:49.000000 alphapulldown-0.30.5/alphafold/alphafold/model/common_modules.py
+-rw-r--r--   0    24600      721    26814 2023-04-18 13:00:49.000000 alphapulldown-0.30.5/alphafold/alphafold/model/config.py
+-rw-r--r--   0    24600      721     1097 2023-04-18 13:00:49.000000 alphapulldown-0.30.5/alphafold/alphafold/model/data.py
+-rw-r--r--   0    24600      721     3692 2023-04-18 13:00:50.000000 alphapulldown-0.30.5/alphafold/alphafold/model/features.py
+-rw-r--r--   0    24600      721    37264 2023-04-18 13:00:50.000000 alphapulldown-0.30.5/alphafold/alphafold/model/folding.py
+-rw-r--r--   0    24600      721    42498 2023-04-18 13:00:50.000000 alphapulldown-0.30.5/alphafold/alphafold/model/folding_multimer.py
+drwxr-xr-x   0    24600      721        0 2023-05-08 11:30:46.000000 alphapulldown-0.30.5/alphafold/alphafold/model/geometry/
+-rw-r--r--   0    24600      721     1172 2023-04-18 13:00:50.000000 alphapulldown-0.30.5/alphafold/alphafold/model/geometry/__init__.py
+-rw-r--r--   0    24600      721     4148 2023-04-18 13:00:50.000000 alphapulldown-0.30.5/alphafold/alphafold/model/geometry/rigid_matrix_vector.py
+-rw-r--r--   0    24600      721     5751 2023-04-18 13:00:51.000000 alphapulldown-0.30.5/alphafold/alphafold/model/geometry/rotation_matrix.py
+-rw-r--r--   0    24600      721     7745 2023-04-18 13:00:51.000000 alphapulldown-0.30.5/alphafold/alphafold/model/geometry/struct_of_array.py
+-rw-r--r--   0    24600      721     4166 2023-04-18 13:00:51.000000 alphapulldown-0.30.5/alphafold/alphafold/model/geometry/test_utils.py
+-rw-r--r--   0    24600      721      853 2023-04-18 13:00:51.000000 alphapulldown-0.30.5/alphafold/alphafold/model/geometry/utils.py
+-rw-r--r--   0    24600      721     6896 2023-04-18 13:00:51.000000 alphapulldown-0.30.5/alphafold/alphafold/model/geometry/vector.py
+-rw-r--r--   0    24600      721     9134 2023-04-18 13:00:51.000000 alphapulldown-0.30.5/alphafold/alphafold/model/layer_stack.py
+-rw-r--r--   0    24600      721    10315 2023-04-18 13:00:52.000000 alphapulldown-0.30.5/alphafold/alphafold/model/layer_stack_test.py
+-rw-r--r--   0    24600      721     3505 2023-04-18 13:00:52.000000 alphapulldown-0.30.5/alphafold/alphafold/model/lddt.py
+-rw-r--r--   0    24600      721     2384 2023-04-18 13:00:52.000000 alphapulldown-0.30.5/alphafold/alphafold/model/lddt_test.py
+-rw-r--r--   0    24600      721     7963 2023-04-18 13:00:52.000000 alphapulldown-0.30.5/alphafold/alphafold/model/mapping.py
+-rw-r--r--   0    24600      721     6613 2023-04-18 13:00:52.000000 alphapulldown-0.30.5/alphafold/alphafold/model/model.py
+-rw-r--r--   0    24600      721    74120 2023-04-18 13:00:52.000000 alphapulldown-0.30.5/alphafold/alphafold/model/modules.py
+-rw-r--r--   0    24600      721    42228 2023-04-18 13:00:52.000000 alphapulldown-0.30.5/alphafold/alphafold/model/modules_multimer.py
+-rw-r--r--   0    24600      721     1978 2023-04-18 13:00:53.000000 alphapulldown-0.30.5/alphafold/alphafold/model/prng.py
+-rw-r--r--   0    24600      721     1250 2023-04-18 13:00:53.000000 alphapulldown-0.30.5/alphafold/alphafold/model/prng_test.py
+-rw-r--r--   0    24600      721    17388 2023-04-18 13:00:53.000000 alphapulldown-0.30.5/alphafold/alphafold/model/quat_affine.py
+-rw-r--r--   0    24600      721     5038 2023-04-18 13:00:53.000000 alphapulldown-0.30.5/alphafold/alphafold/model/quat_affine_test.py
+-rw-r--r--   0    24600      721    10935 2023-04-18 13:00:53.000000 alphapulldown-0.30.5/alphafold/alphafold/model/r3.py
+drwxr-xr-x   0    24600      721        0 2023-05-08 11:30:49.000000 alphapulldown-0.30.5/alphafold/alphafold/model/tf/
+-rw-r--r--   0    24600      721      633 2023-04-18 13:00:53.000000 alphapulldown-0.30.5/alphafold/alphafold/model/tf/__init__.py
+-rw-r--r--   0    24600      721    21428 2023-04-18 13:00:54.000000 alphapulldown-0.30.5/alphafold/alphafold/model/tf/data_transforms.py
+-rw-r--r--   0    24600      721     5357 2023-04-18 13:00:54.000000 alphapulldown-0.30.5/alphafold/alphafold/model/tf/input_pipeline.py
+-rw-r--r--   0    24600      721     5051 2023-04-18 13:00:54.000000 alphapulldown-0.30.5/alphafold/alphafold/model/tf/protein_features.py
+-rw-r--r--   0    24600      721     1822 2023-04-18 13:00:54.000000 alphapulldown-0.30.5/alphafold/alphafold/model/tf/protein_features_test.py
+-rw-r--r--   0    24600      721     6344 2023-04-18 13:00:54.000000 alphapulldown-0.30.5/alphafold/alphafold/model/tf/proteins_dataset.py
+-rw-r--r--   0    24600      721     1415 2023-04-18 13:00:54.000000 alphapulldown-0.30.5/alphafold/alphafold/model/tf/shape_helpers.py
+-rw-r--r--   0    24600      721     1318 2023-04-18 13:00:55.000000 alphapulldown-0.30.5/alphafold/alphafold/model/tf/shape_helpers_test.py
+-rw-r--r--   0    24600      721      812 2023-04-18 13:00:55.000000 alphapulldown-0.30.5/alphafold/alphafold/model/tf/shape_placeholders.py
+-rw-r--r--   0    24600      721     1276 2023-04-18 13:00:55.000000 alphapulldown-0.30.5/alphafold/alphafold/model/tf/utils.py
+-rw-r--r--   0    24600      721     5328 2023-04-18 13:00:55.000000 alphapulldown-0.30.5/alphafold/alphafold/model/utils.py
+drwxr-xr-x   0    24600      721        0 2023-05-08 11:30:51.000000 alphapulldown-0.30.5/alphafold/alphafold/notebooks/
+-rw-r--r--   0    24600      721      626 2023-04-18 13:00:55.000000 alphapulldown-0.30.5/alphafold/alphafold/notebooks/__init__.py
+-rw-r--r--   0    24600      721     7520 2023-04-18 13:00:55.000000 alphapulldown-0.30.5/alphafold/alphafold/notebooks/notebook_utils.py
+-rw-r--r--   0    24600      721     9571 2023-04-18 13:00:56.000000 alphapulldown-0.30.5/alphafold/alphafold/notebooks/notebook_utils_test.py
+drwxr-xr-x   0    24600      721        0 2023-05-08 11:30:54.000000 alphapulldown-0.30.5/alphafold/alphafold/relax/
+-rw-r--r--   0    24600      721      618 2023-04-18 13:00:56.000000 alphapulldown-0.30.5/alphafold/alphafold/relax/__init__.py
+-rw-r--r--   0    24600      721    19061 2023-04-18 13:00:56.000000 alphapulldown-0.30.5/alphafold/alphafold/relax/amber_minimize.py
+-rw-r--r--   0    24600      721     4348 2023-04-18 13:00:56.000000 alphapulldown-0.30.5/alphafold/alphafold/relax/amber_minimize_test.py
+-rw-r--r--   0    24600      721     4832 2023-04-18 13:00:57.000000 alphapulldown-0.30.5/alphafold/alphafold/relax/cleanup.py
+-rw-r--r--   0    24600      721     6170 2023-04-18 13:00:57.000000 alphapulldown-0.30.5/alphafold/alphafold/relax/cleanup_test.py
+-rw-r--r--   0    24600      721     3288 2023-04-18 13:00:57.000000 alphapulldown-0.30.5/alphafold/alphafold/relax/relax.py
+-rw-r--r--   0    24600      721     3827 2023-04-18 13:00:57.000000 alphapulldown-0.30.5/alphafold/alphafold/relax/relax_test.py
+-rw-r--r--   0    24600      721     2501 2023-04-18 13:00:58.000000 alphapulldown-0.30.5/alphafold/alphafold/relax/utils.py
+-rw-r--r--   0    24600      721     1996 2023-04-18 13:00:59.000000 alphapulldown-0.30.5/alphafold/alphafold/relax/utils_test.py
+drwxr-xr-x   0    24600      721        0 2023-05-08 11:30:56.000000 alphapulldown-0.30.5/alphafold/common/
+-rw-r--r--   0    24600      721      655 2023-04-19 11:33:22.000000 alphapulldown-0.30.5/alphafold/common/__init__.py
+-rw-r--r--   0    24600      721     6066 2023-04-19 11:33:23.000000 alphapulldown-0.30.5/alphafold/common/confidence.py
+-rw-r--r--   0    24600      721     9959 2023-04-19 11:33:23.000000 alphapulldown-0.30.5/alphafold/common/protein.py
+-rw-r--r--   0    24600      721     4594 2023-04-19 11:33:23.000000 alphapulldown-0.30.5/alphafold/common/protein_test.py
+-rw-r--r--   0    24600      721    34974 2023-04-19 11:33:24.000000 alphapulldown-0.30.5/alphafold/common/residue_constants.py
+-rw-r--r--   0    24600      721     9256 2023-04-19 11:33:24.000000 alphapulldown-0.30.5/alphafold/common/residue_constants_test.py
+drwxr-xr-x   0    24600      721        0 2023-05-08 11:30:59.000000 alphapulldown-0.30.5/alphafold/data/
+-rw-r--r--   0    24600      721      634 2023-04-19 11:33:26.000000 alphapulldown-0.30.5/alphafold/data/__init__.py
+-rw-r--r--   0    24600      721     8575 2023-04-19 11:33:26.000000 alphapulldown-0.30.5/alphafold/data/feature_processing.py
+-rw-r--r--   0    24600      721    14182 2023-04-19 11:33:26.000000 alphapulldown-0.30.5/alphafold/data/mmcif_parsing.py
+-rw-r--r--   0    24600      721     2966 2023-04-19 11:33:27.000000 alphapulldown-0.30.5/alphafold/data/msa_identifiers.py
+-rw-r--r--   0    24600      721    17220 2023-04-19 11:33:27.000000 alphapulldown-0.30.5/alphafold/data/msa_pairing.py
+-rw-r--r--   0    24600      721    21397 2023-04-19 11:33:28.000000 alphapulldown-0.30.5/alphafold/data/parsers.py
+-rw-r--r--   0    24600      721    10419 2023-04-19 11:33:28.000000 alphapulldown-0.30.5/alphafold/data/pipeline.py
+-rw-r--r--   0    24600      721    11126 2023-04-19 11:33:28.000000 alphapulldown-0.30.5/alphafold/data/pipeline_multimer.py
+-rw-r--r--   0    24600      721    40677 2023-04-19 11:33:29.000000 alphapulldown-0.30.5/alphafold/data/templates.py
+drwxr-xr-x   0    24600      721        0 2023-05-08 11:31:03.000000 alphapulldown-0.30.5/alphafold/data/tools/
+-rw-r--r--   0    24600      721      639 2023-04-19 11:33:29.000000 alphapulldown-0.30.5/alphafold/data/tools/__init__.py
+-rw-r--r--   0    24600      721     5504 2023-04-19 11:33:29.000000 alphapulldown-0.30.5/alphafold/data/tools/hhblits.py
+-rw-r--r--   0    24600      721     3601 2023-04-19 11:33:30.000000 alphapulldown-0.30.5/alphafold/data/tools/hhsearch.py
+-rw-r--r--   0    24600      721     4576 2023-04-19 11:33:30.000000 alphapulldown-0.30.5/alphafold/data/tools/hmmbuild.py
+-rw-r--r--   0    24600      721     4556 2023-04-19 11:33:31.000000 alphapulldown-0.30.5/alphafold/data/tools/hmmsearch.py
+-rw-r--r--   0    24600      721     8386 2023-04-19 11:33:31.000000 alphapulldown-0.30.5/alphafold/data/tools/jackhmmer.py
+-rw-r--r--   0    24600      721     3387 2023-04-19 11:33:31.000000 alphapulldown-0.30.5/alphafold/data/tools/kalign.py
+-rw-r--r--   0    24600      721     1223 2023-04-19 11:33:31.000000 alphapulldown-0.30.5/alphafold/data/tools/utils.py
+drwxr-xr-x   0    24600      721        0 2023-05-08 11:31:14.000000 alphapulldown-0.30.5/alphafold/model/
+-rw-r--r--   0    24600      721      617 2023-04-19 11:33:32.000000 alphapulldown-0.30.5/alphafold/model/__init__.py
+-rw-r--r--   0    24600      721    47028 2023-04-19 11:33:32.000000 alphapulldown-0.30.5/alphafold/model/all_atom.py
+-rw-r--r--   0    24600      721    40145 2023-04-19 11:33:33.000000 alphapulldown-0.30.5/alphafold/model/all_atom_multimer.py
+-rw-r--r--   0    24600      721     4706 2023-04-19 11:33:33.000000 alphapulldown-0.30.5/alphafold/model/all_atom_test.py
+-rw-r--r--   0    24600      721     5957 2023-04-19 11:33:33.000000 alphapulldown-0.30.5/alphafold/model/common_modules.py
+-rw-r--r--   0    24600      721    26814 2023-04-19 11:33:34.000000 alphapulldown-0.30.5/alphafold/model/config.py
+-rw-r--r--   0    24600      721     1097 2023-04-19 11:33:34.000000 alphapulldown-0.30.5/alphafold/model/data.py
+-rw-r--r--   0    24600      721     3692 2023-04-19 11:33:34.000000 alphapulldown-0.30.5/alphafold/model/features.py
+-rw-r--r--   0    24600      721    37264 2023-04-19 11:33:35.000000 alphapulldown-0.30.5/alphafold/model/folding.py
+-rw-r--r--   0    24600      721    42498 2023-04-19 11:33:35.000000 alphapulldown-0.30.5/alphafold/model/folding_multimer.py
+drwxr-xr-x   0    24600      721        0 2023-05-08 11:31:17.000000 alphapulldown-0.30.5/alphafold/model/geometry/
+-rw-r--r--   0    24600      721     1172 2023-04-19 11:33:36.000000 alphapulldown-0.30.5/alphafold/model/geometry/__init__.py
+-rw-r--r--   0    24600      721     4148 2023-04-19 11:33:36.000000 alphapulldown-0.30.5/alphafold/model/geometry/rigid_matrix_vector.py
+-rw-r--r--   0    24600      721     5751 2023-04-19 11:33:37.000000 alphapulldown-0.30.5/alphafold/model/geometry/rotation_matrix.py
+-rw-r--r--   0    24600      721     7745 2023-04-19 11:33:37.000000 alphapulldown-0.30.5/alphafold/model/geometry/struct_of_array.py
+-rw-r--r--   0    24600      721     4166 2023-04-19 11:33:37.000000 alphapulldown-0.30.5/alphafold/model/geometry/test_utils.py
+-rw-r--r--   0    24600      721      853 2023-04-19 11:33:38.000000 alphapulldown-0.30.5/alphafold/model/geometry/utils.py
+-rw-r--r--   0    24600      721     6896 2023-04-19 11:33:38.000000 alphapulldown-0.30.5/alphafold/model/geometry/vector.py
+-rw-r--r--   0    24600      721     9134 2023-04-19 11:33:38.000000 alphapulldown-0.30.5/alphafold/model/layer_stack.py
+-rw-r--r--   0    24600      721    10315 2023-04-19 11:33:39.000000 alphapulldown-0.30.5/alphafold/model/layer_stack_test.py
+-rw-r--r--   0    24600      721     3505 2023-04-19 11:33:39.000000 alphapulldown-0.30.5/alphafold/model/lddt.py
+-rw-r--r--   0    24600      721     2384 2023-04-19 11:33:39.000000 alphapulldown-0.30.5/alphafold/model/lddt_test.py
+-rw-r--r--   0    24600      721     7963 2023-04-19 11:33:40.000000 alphapulldown-0.30.5/alphafold/model/mapping.py
+-rw-r--r--   0    24600      721     6613 2023-04-19 11:33:40.000000 alphapulldown-0.30.5/alphafold/model/model.py
+-rw-r--r--   0    24600      721    74120 2023-04-19 11:33:40.000000 alphapulldown-0.30.5/alphafold/model/modules.py
+-rw-r--r--   0    24600      721    42228 2023-04-19 11:33:41.000000 alphapulldown-0.30.5/alphafold/model/modules_multimer.py
+-rw-r--r--   0    24600      721     1978 2023-04-19 11:33:41.000000 alphapulldown-0.30.5/alphafold/model/prng.py
+-rw-r--r--   0    24600      721     1250 2023-04-19 11:33:41.000000 alphapulldown-0.30.5/alphafold/model/prng_test.py
+-rw-r--r--   0    24600      721    17388 2023-04-19 11:33:42.000000 alphapulldown-0.30.5/alphafold/model/quat_affine.py
+-rw-r--r--   0    24600      721     5038 2023-04-19 11:33:42.000000 alphapulldown-0.30.5/alphafold/model/quat_affine_test.py
+-rw-r--r--   0    24600      721    10935 2023-04-19 11:33:42.000000 alphapulldown-0.30.5/alphafold/model/r3.py
+drwxr-xr-x   0    24600      721        0 2023-05-08 11:31:21.000000 alphapulldown-0.30.5/alphafold/model/tf/
+-rw-r--r--   0    24600      721      633 2023-04-19 11:33:43.000000 alphapulldown-0.30.5/alphafold/model/tf/__init__.py
+-rw-r--r--   0    24600      721    21428 2023-04-19 11:33:43.000000 alphapulldown-0.30.5/alphafold/model/tf/data_transforms.py
+-rw-r--r--   0    24600      721     5357 2023-04-19 11:33:44.000000 alphapulldown-0.30.5/alphafold/model/tf/input_pipeline.py
+-rw-r--r--   0    24600      721     5051 2023-04-19 11:33:44.000000 alphapulldown-0.30.5/alphafold/model/tf/protein_features.py
+-rw-r--r--   0    24600      721     1822 2023-04-19 11:33:44.000000 alphapulldown-0.30.5/alphafold/model/tf/protein_features_test.py
+-rw-r--r--   0    24600      721     6344 2023-04-19 11:33:45.000000 alphapulldown-0.30.5/alphafold/model/tf/proteins_dataset.py
+-rw-r--r--   0    24600      721     1415 2023-04-19 11:33:45.000000 alphapulldown-0.30.5/alphafold/model/tf/shape_helpers.py
+-rw-r--r--   0    24600      721     1318 2023-04-19 11:33:45.000000 alphapulldown-0.30.5/alphafold/model/tf/shape_helpers_test.py
+-rw-r--r--   0    24600      721      812 2023-04-19 11:33:46.000000 alphapulldown-0.30.5/alphafold/model/tf/shape_placeholders.py
+-rw-r--r--   0    24600      721     1276 2023-04-19 11:33:46.000000 alphapulldown-0.30.5/alphafold/model/tf/utils.py
+-rw-r--r--   0    24600      721     5328 2023-04-19 11:33:46.000000 alphapulldown-0.30.5/alphafold/model/utils.py
+drwxr-xr-x   0    24600      721        0 2023-05-08 11:31:22.000000 alphapulldown-0.30.5/alphafold/notebooks/
+-rw-r--r--   0    24600      721      626 2023-04-19 11:33:46.000000 alphapulldown-0.30.5/alphafold/notebooks/__init__.py
+-rw-r--r--   0    24600      721     7520 2023-04-19 11:33:47.000000 alphapulldown-0.30.5/alphafold/notebooks/notebook_utils.py
+-rw-r--r--   0    24600      721     9571 2023-04-19 11:33:47.000000 alphapulldown-0.30.5/alphafold/notebooks/notebook_utils_test.py
+drwxr-xr-x   0    24600      721        0 2023-05-08 11:31:25.000000 alphapulldown-0.30.5/alphafold/relax/
+-rw-r--r--   0    24600      721      618 2023-04-19 11:33:48.000000 alphapulldown-0.30.5/alphafold/relax/__init__.py
+-rw-r--r--   0    24600      721    19061 2023-04-19 11:33:48.000000 alphapulldown-0.30.5/alphafold/relax/amber_minimize.py
+-rw-r--r--   0    24600      721     4348 2023-04-19 11:33:48.000000 alphapulldown-0.30.5/alphafold/relax/amber_minimize_test.py
+-rw-r--r--   0    24600      721     4832 2023-04-19 11:33:49.000000 alphapulldown-0.30.5/alphafold/relax/cleanup.py
+-rw-r--r--   0    24600      721     6170 2023-04-19 11:33:49.000000 alphapulldown-0.30.5/alphafold/relax/cleanup_test.py
+-rw-r--r--   0    24600      721     3288 2023-04-19 11:33:49.000000 alphapulldown-0.30.5/alphafold/relax/relax.py
+-rw-r--r--   0    24600      721     3827 2023-04-19 11:33:50.000000 alphapulldown-0.30.5/alphafold/relax/relax_test.py
+-rw-r--r--   0    24600      721     2501 2023-04-19 11:33:52.000000 alphapulldown-0.30.5/alphafold/relax/utils.py
+-rw-r--r--   0    24600      721     1996 2023-04-19 11:33:52.000000 alphapulldown-0.30.5/alphafold/relax/utils_test.py
+-rw-r--r--   0    24600      721    19606 2023-04-19 11:33:53.000000 alphapulldown-0.30.5/alphafold/run_alphafold.py
+-rw-r--r--   0    24600      721     3814 2023-04-18 13:01:10.000000 alphapulldown-0.30.5/alphafold/run_alphafold_test.py
+-rw-r--r--   0    24600      721     2064 2023-04-18 13:01:11.000000 alphapulldown-0.30.5/alphafold/setup.py
+drwxr-xr-x   0    24600      721        0 2023-05-08 11:31:29.000000 alphapulldown-0.30.5/alphapulldown/
+-rw-r--r--   0    24600      721        0 2023-01-27 13:02:50.000000 alphapulldown-0.30.5/alphapulldown/__init__.py
+-rw-r--r--   0    24600      721     3944 2023-03-14 16:09:43.000000 alphapulldown-0.30.5/alphapulldown/colab_batch_no_prediction.py
+-rwxr-xr-x   0    24600      721    10571 2023-04-19 11:33:53.000000 alphapulldown-0.30.5/alphapulldown/create_individual_features.py
+-rw-r--r--   0    24600      721    22205 2023-04-19 11:33:53.000000 alphapulldown-0.30.5/alphapulldown/objects.py
+-rw-r--r--   0    24600      721     1822 2023-03-14 16:09:43.000000 alphapulldown-0.30.5/alphapulldown/plot_pae.py
+-rw-r--r--   0    24600      721     8878 2023-04-18 11:12:23.000000 alphapulldown-0.30.5/alphapulldown/predict_structure.py
+-rwxr-xr-x   0    24600      721     1166 2023-03-14 16:09:44.000000 alphapulldown-0.30.5/alphapulldown/prepare_seq_names.py
+-rwxr-xr-x   0    24600      721     1261 2023-03-14 16:09:44.000000 alphapulldown-0.30.5/alphapulldown/rename_colab_search_a3m.py
+-rw-r--r--   0    24600      721    11611 2023-04-18 11:12:24.000000 alphapulldown-0.30.5/alphapulldown/run_multimer_jobs.py
+-rw-r--r--   0    24600      721       63 2023-03-14 16:09:45.000000 alphapulldown-0.30.5/alphapulldown/test_global.py
+-rw-r--r--   0    24600      721    11544 2023-05-08 11:10:53.000000 alphapulldown-0.30.5/alphapulldown/utils.py
+drwxr-xr-x   0    24600      721        0 2023-05-08 11:31:31.000000 alphapulldown-0.30.5/alphapulldown.egg-info/
+-rw-r--r--   0    24600      721      428 2023-05-08 11:30:07.000000 alphapulldown-0.30.5/alphapulldown.egg-info/PKG-INFO
+-rw-r--r--   0    24600      721     7553 2023-05-08 11:30:08.000000 alphapulldown-0.30.5/alphapulldown.egg-info/SOURCES.txt
+-rw-r--r--   0    24600      721        1 2023-05-08 11:30:07.000000 alphapulldown-0.30.5/alphapulldown.egg-info/dependency_links.txt
+-rw-r--r--   0    24600      721      262 2023-05-08 11:30:07.000000 alphapulldown-0.30.5/alphapulldown.egg-info/requires.txt
+-rw-r--r--   0    24600      721       52 2023-05-08 11:30:08.000000 alphapulldown-0.30.5/alphapulldown.egg-info/top_level.txt
+drwxr-xr-x   0    24600      721        0 2023-05-08 11:31:33.000000 alphapulldown-0.30.5/analysis_pipeline/
+-rw-r--r--   0    24600      721        0 2023-04-18 11:12:25.000000 alphapulldown-0.30.5/analysis_pipeline/__init__.py
+-rw-r--r--   0    24600      721     7268 2023-04-18 11:12:25.000000 alphapulldown-0.30.5/analysis_pipeline/af2_3dmol.py
+-rw-r--r--   0    24600      721     4967 2023-04-18 11:12:25.000000 alphapulldown-0.30.5/analysis_pipeline/calculate_mpdockq.py
+-rw-r--r--   0    24600      721     5510 2023-04-18 11:12:26.000000 alphapulldown-0.30.5/analysis_pipeline/create_notebook.py
+-rw-r--r--   0    24600      721     6253 2023-04-18 11:12:26.000000 alphapulldown-0.30.5/analysis_pipeline/get_good_inter_pae.py
+-rw-r--r--   0    24600      721      962 2023-04-18 11:12:26.000000 alphapulldown-0.30.5/analysis_pipeline/utils.py
+drwxr-xr-x   0    24600      721        0 2023-05-08 11:31:40.000000 alphapulldown-0.30.5/colabfold/
+-rw-r--r--   0    24600      721        0 2023-04-06 09:21:34.000000 alphapulldown-0.30.5/colabfold/__init__.py
+drwxr-xr-x   0    24600      721        0 2023-05-08 11:31:41.000000 alphapulldown-0.30.5/colabfold/alphafold/
+-rw-r--r--   0    24600      721        0 2023-04-06 09:21:34.000000 alphapulldown-0.30.5/colabfold/alphafold/__init__.py
+-rw-r--r--   0    24600      721     5923 2023-04-06 09:21:34.000000 alphapulldown-0.30.5/colabfold/alphafold/models.py
+-rw-r--r--   0    24600      721     1565 2023-04-06 09:21:34.000000 alphapulldown-0.30.5/colabfold/alphafold/msa.py
+-rw-r--r--   0    24600      721    65347 2023-04-06 09:21:34.000000 alphapulldown-0.30.5/colabfold/batch.py
+-rw-r--r--   0    24600      721     5988 2023-04-06 09:21:34.000000 alphapulldown-0.30.5/colabfold/citations.py
+-rw-r--r--   0    24600      721    24980 2023-04-06 09:21:34.000000 alphapulldown-0.30.5/colabfold/colabfold.py
+-rw-r--r--   0    24600      721    32656 2023-04-06 09:21:34.000000 alphapulldown-0.30.5/colabfold/colabfold_alphafold.py
+-rw-r--r--   0    24600      721     1982 2023-04-06 09:21:34.000000 alphapulldown-0.30.5/colabfold/download.py
+drwxr-xr-x   0    24600      721        0 2023-05-08 11:31:42.000000 alphapulldown-0.30.5/colabfold/mmseqs/
+-rw-r--r--   0    24600      721        0 2023-04-06 09:21:34.000000 alphapulldown-0.30.5/colabfold/mmseqs/__init__.py
+-rw-r--r--   0    24600      721     1933 2023-04-06 09:21:34.000000 alphapulldown-0.30.5/colabfold/mmseqs/merge_and_split_msas.py
+-rw-r--r--   0    24600      721    18799 2023-04-06 09:21:34.000000 alphapulldown-0.30.5/colabfold/mmseqs/search.py
+-rw-r--r--   0    24600      721     1429 2023-04-06 09:21:34.000000 alphapulldown-0.30.5/colabfold/mmseqs/split_msas.py
+-rw-r--r--   0    24600      721     2120 2023-04-06 09:21:34.000000 alphapulldown-0.30.5/colabfold/pdb.py
+-rw-r--r--   0    24600      721     3419 2023-04-06 09:21:35.000000 alphapulldown-0.30.5/colabfold/plot.py
+-rw-r--r--   0    24600      721     9954 2023-04-06 09:21:35.000000 alphapulldown-0.30.5/colabfold/utils.py
+-rw-r--r--   0    24600      721      140 2023-04-05 11:02:03.000000 alphapulldown-0.30.5/pyproject.toml
+-rw-r--r--   0    24600      721     1164 2023-05-08 11:31:44.000000 alphapulldown-0.30.5/setup.cfg
+-rwxr-xr-x   0    24600      721       67 2023-04-18 11:12:27.000000 alphapulldown-0.30.5/setup.py
+-rw-r--r--   0    24600      721     9119 2023-04-18 11:12:28.000000 alphapulldown-0.30.5/stereo_chemical_props.txt
+drwxr-xr-x   0    24600      721        0 2023-05-08 11:31:43.000000 alphapulldown-0.30.5/test/
+-rw-r--r--   0    24600      721     4546 2023-04-19 11:33:54.000000 alphapulldown-0.30.5/test/test_create_objects.py
+-rwxr-xr-x   0    24600      721    11179 2023-05-08 11:07:26.000000 alphapulldown-0.30.5/test/test_predict_structure.py
```

### Comparing `alphapulldown-0.30.4/LICENSE` & `alphapulldown-0.30.5/LICENSE`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/README.md` & `alphapulldown-0.30.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         uniref90.fasta
  ```
 
 ## Installation 
 
 **Firstly**, install [Anaconda](https://www.anaconda.com/) and create AlphaPulldown environment, gathering necessary dependencies 
 ```bash
-conda create -n AlphaPulldown -c omnia -c bioconda -c conda-forge python==3.8 openmm=7.5.1 pdbfixer kalign2=2.04 cctbx-base
+conda create -n AlphaPulldown -c omnia -c bioconda -c conda-forge python==3.8 openmm=7.5.1 pdbfixer=1.6 kalign2=2.04 cctbx-base
 ```
 
 **Secondly**, activate the AlphaPulldown environment and install AlphaPulldown
 ```bash
 source activate AlphaPulldown
 python3 -m pip install alphapulldown==0.30.1
 pip install -q "jax[cuda]==0.3.25" -f https://storage.googleapis.com/jax-releases/jax_cuda_releases.html
```

### Comparing `alphapulldown-0.30.4/alphapulldown/analysis_pipeline/create_notebook.py` & `alphapulldown-0.30.5/analysis_pipeline/create_notebook.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/alphapulldown/create_individual_features.py` & `alphapulldown-0.30.5/alphapulldown/create_individual_features.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/alphapulldown/prepare_seq_names.py` & `alphapulldown-0.30.5/alphapulldown/prepare_seq_names.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/alphapulldown/rename_colab_search_a3m.py` & `alphapulldown-0.30.5/alphapulldown/rename_colab_search_a3m.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/alphapulldown/run_multimer_jobs.py` & `alphapulldown-0.30.5/alphapulldown/run_multimer_jobs.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 
 # Author: Dingquan Yu
 # A script to create region information for create_multimer_features.py
 # #
 
 
 import itertools
-from re import I
 from absl import app, flags, logging
 from alphapulldown.utils import *
 from itertools import combinations
 from alphapulldown.objects import MultimericObject
 import os
-import shutil
 from pathlib import Path
-from alphapulldown.predict_structure import predict
+from alphapulldown.predict_structure import predict, ModelsToRelax
 
 
 
+run_af = get_run_alphafold()
+flags = run_af.flags
 
 flags.DEFINE_enum(
     "mode",
     "pulldown",
     ["pulldown", "all_vs_all", "homo-oligomer", "custom"],
     "choose the mode of running multimer jobs",
 )
@@ -32,62 +32,69 @@
 flags.DEFINE_string("oligomer_state_file", None, "path to oligomer state files")
 flags.DEFINE_list(
     "monomer_objects_dir",
     None,
     "a list of directories where monomer objects are stored",
 )
 flags.DEFINE_list("protein_lists", None, "protein list files")
+
+delattr(flags.FLAGS, "data_dir")
 flags.DEFINE_string("data_dir", None, "Path to params directory")
-flags.DEFINE_boolean(
-    "random_seed",
-    False,
-    "Run multiple JAX model evaluations "
-    "to obtain a timing that excludes the compilation time, "
-    "which should be more indicative of the time required for "
-    "inferencing many proteins.",
-)
+
 flags.DEFINE_integer("num_cycle", 3, help="number of recycles")
-flags.DEFINE_boolean(
-    "amber_relax",
-    False,
-    "Run multiple JAX model evaluations "
-    "to obtain a timing that excludes the compilation time, "
-    "which should be more indicative of the time required for "
-    "inferencing many proteins.",
-)
-flags.DEFINE_boolean(
-    "benchmark",
-    False,
-    "Run multiple JAX model evaluations "
-    "to obtain a timing that excludes the compilation time, "
-    "which should be more indicative of the time required for "
-    "inferencing many proteins.",
-)
-flags.DEFINE_enum(
-    "model_preset",
-    "multimer",
-    ["monomer", "monomer_casp14", "monomer_ptm", "multimer"],
-    "Choose preset model configuration - the monomer model, "
-    "the monomer model with extra ensembling, monomer model with "
-    "pTM head, or multimer model",
-)
 flags.DEFINE_integer(
     "num_predictions_per_model", 1, "How many predictions per model. Default is 1"
 )
 flags.DEFINE_integer(
     "job_index", None, "index of sequence in the fasta file, starting from 1"
 )
 flags.DEFINE_boolean(
     "no_pair_msa", False, "do not pair the MSAs when constructing multimer objects"
 )
 flags.mark_flag_as_required("output_path")
-FLAGS = flags.FLAGS
 
+delattr(flags.FLAGS, "models_to_relax")
+flags.DEFINE_enum_class('models_to_relax', ModelsToRelax.NONE, ModelsToRelax,
+                        'The models to run the final relaxation step on. '
+                        'If `all`, all models are relaxed, which may be time '
+                        'consuming. If `best`, only the most confident model '
+                        'is relaxed. If `none`, relaxation is not run. Turning '
+                        'off relaxation might result in predictions with '
+                        'distracting stereochemical violations but might help '
+                        'in case you are having issues with the relaxation '
+                        'stage.')
+
+unused_flags = (
+    'bfd_database_path',
+    'db_preset',
+    'fasta_paths',
+    'hhblits_binary_path',
+    'hhsearch_binary_path',
+    'hmmbuild_binary_path',
+    'hmmsearch_binary_path',
+    'jackhmmer_binary_path',
+    'kalign_binary_path',
+    'max_template_date',
+    'mgnify_database_path',
+    'num_multimer_predictions_per_model',
+    'obsolete_pdbs_path',
+    'output_dir',
+    'pdb70_database_path',
+    'pdb_seqres_database_path',
+    'small_bfd_database_path',
+    'template_mmcif_dir',
+    'uniprot_database_path',
+    'uniref30_database_path',
+    'uniref90_database_path',
+)
 
+for flag in unused_flags:
+    delattr(flags.FLAGS, flag)
 
+FLAGS = flags.FLAGS
 
 def create_pulldown_info(
     bait_proteins: list, candidate_proteins: list, job_index=None
 ) -> dict:
     """
     A function to create apms info
 
@@ -243,21 +250,22 @@
             lines = lines + list(f.readlines())
             f.close()
     if job_index is not None:
         job_idxes = [job_index - 1]
     else:
         job_idxes = list(range(len(lines)))
 
-
+    multimers = []
     for job_idx in job_idxes:
         l = lines[job_idx]
         if len(l.strip()) > 0:
             all_proteins = read_custom(l)
             data = create_custom_info(all_proteins)
-            multimers = create_multimer_objects(data, monomer_objects_dir, pair_msa=pair_msa)
+            multimer = create_multimer_objects(data, monomer_objects_dir, pair_msa=pair_msa)
+            multimers += multimer
     return multimers
 
 
 
 
 def predict_individual_jobs(multimer_object, output_path, model_runners, random_seed):
     output_path = os.path.join(output_path, multimer_object.description)
@@ -272,15 +280,15 @@
     predict(
         model_runners,
         output_path,
         multimer_object.feature_dict,
         random_seed,
         FLAGS.benchmark,
         fasta_name=multimer_object.description,
-        amber_relaxer=FLAGS.amber_relax,
+        models_to_relax=FLAGS.models_to_relax,
         seqs=multimer_object.input_seqs,
     )
     create_and_save_pae_plots(multimer_object, output_path)
```

### Comparing `alphapulldown-0.30.4/src/alphafold/__init__.py` & `alphapulldown-0.30.5/alphafold/__init__.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/src/alphafold/common/__init__.py` & `alphapulldown-0.30.5/alphafold/alphafold/common/__init__.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/src/alphafold/common/confidence.py` & `alphapulldown-0.30.5/alphafold/alphafold/common/confidence.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/src/alphafold/common/protein.py` & `alphapulldown-0.30.5/alphafold/alphafold/common/protein.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/src/alphafold/common/protein_test.py` & `alphapulldown-0.30.5/alphafold/alphafold/common/protein_test.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/src/alphafold/common/residue_constants.py` & `alphapulldown-0.30.5/alphafold/alphafold/common/residue_constants.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/src/alphafold/common/residue_constants_test.py` & `alphapulldown-0.30.5/alphafold/alphafold/common/residue_constants_test.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/src/alphafold/data/__init__.py` & `alphapulldown-0.30.5/alphafold/alphafold/data/__init__.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/src/alphafold/data/feature_processing.py` & `alphapulldown-0.30.5/alphafold/alphafold/data/feature_processing.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/src/alphafold/data/mmcif_parsing.py` & `alphapulldown-0.30.5/alphafold/alphafold/data/mmcif_parsing.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/src/alphafold/data/msa_identifiers.py` & `alphapulldown-0.30.5/alphafold/data/msa_identifiers.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/src/alphafold/data/msa_pairing.py` & `alphapulldown-0.30.5/alphafold/alphafold/data/msa_pairing.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/src/alphafold/data/parsers.py` & `alphapulldown-0.30.5/alphafold/alphafold/data/parsers.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/src/alphafold/data/pipeline.py` & `alphapulldown-0.30.5/alphafold/alphafold/data/pipeline.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/src/alphafold/data/pipeline_multimer.py` & `alphapulldown-0.30.5/alphafold/alphafold/data/pipeline_multimer.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/src/alphafold/data/templates.py` & `alphapulldown-0.30.5/alphafold/alphafold/data/templates.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/src/alphafold/data/tools/__init__.py` & `alphapulldown-0.30.5/alphafold/alphafold/data/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/src/alphafold/data/tools/hhblits.py` & `alphapulldown-0.30.5/alphafold/alphafold/data/tools/hhblits.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/src/alphafold/data/tools/hhsearch.py` & `alphapulldown-0.30.5/alphafold/alphafold/data/tools/hhsearch.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/src/alphafold/data/tools/hmmbuild.py` & `alphapulldown-0.30.5/alphafold/alphafold/data/tools/hmmbuild.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/src/alphafold/data/tools/hmmsearch.py` & `alphapulldown-0.30.5/alphafold/alphafold/data/tools/hmmsearch.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/src/alphafold/data/tools/jackhmmer.py` & `alphapulldown-0.30.5/alphafold/alphafold/data/tools/jackhmmer.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/src/alphafold/data/tools/kalign.py` & `alphapulldown-0.30.5/alphafold/alphafold/data/tools/kalign.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/src/alphafold/data/tools/utils.py` & `alphapulldown-0.30.5/alphafold/alphafold/data/tools/utils.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/src/alphafold/model/__init__.py` & `alphapulldown-0.30.5/alphafold/alphafold/model/__init__.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/src/alphafold/model/all_atom.py` & `alphapulldown-0.30.5/alphafold/alphafold/model/all_atom.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/src/alphafold/model/all_atom_multimer.py` & `alphapulldown-0.30.5/alphafold/alphafold/model/all_atom_multimer.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/src/alphafold/model/all_atom_test.py` & `alphapulldown-0.30.5/alphafold/alphafold/model/all_atom_test.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/src/alphafold/model/common_modules.py` & `alphapulldown-0.30.5/alphafold/alphafold/model/common_modules.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/src/alphafold/model/config.py` & `alphapulldown-0.30.5/alphafold/alphafold/model/config.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/src/alphafold/model/data.py` & `alphapulldown-0.30.5/alphafold/alphafold/model/data.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/src/alphafold/model/features.py` & `alphapulldown-0.30.5/alphafold/alphafold/model/features.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/src/alphafold/model/folding.py` & `alphapulldown-0.30.5/alphafold/alphafold/model/folding.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/src/alphafold/model/folding_multimer.py` & `alphapulldown-0.30.5/alphafold/alphafold/model/folding_multimer.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/src/alphafold/model/geometry/__init__.py` & `alphapulldown-0.30.5/alphafold/alphafold/model/geometry/__init__.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/src/alphafold/model/geometry/rigid_matrix_vector.py` & `alphapulldown-0.30.5/alphafold/alphafold/model/geometry/rigid_matrix_vector.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/src/alphafold/model/geometry/rotation_matrix.py` & `alphapulldown-0.30.5/alphafold/alphafold/model/geometry/rotation_matrix.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/src/alphafold/model/geometry/struct_of_array.py` & `alphapulldown-0.30.5/alphafold/alphafold/model/geometry/struct_of_array.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/src/alphafold/model/geometry/test_utils.py` & `alphapulldown-0.30.5/alphafold/alphafold/model/geometry/test_utils.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/src/alphafold/model/geometry/utils.py` & `alphapulldown-0.30.5/alphafold/alphafold/model/geometry/utils.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/src/alphafold/model/geometry/vector.py` & `alphapulldown-0.30.5/alphafold/alphafold/model/geometry/vector.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/src/alphafold/model/layer_stack.py` & `alphapulldown-0.30.5/alphafold/alphafold/model/layer_stack.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/src/alphafold/model/layer_stack_test.py` & `alphapulldown-0.30.5/alphafold/alphafold/model/layer_stack_test.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/src/alphafold/model/lddt.py` & `alphapulldown-0.30.5/alphafold/alphafold/model/lddt.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/src/alphafold/model/lddt_test.py` & `alphapulldown-0.30.5/alphafold/alphafold/model/lddt_test.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/src/alphafold/model/mapping.py` & `alphapulldown-0.30.5/alphafold/alphafold/model/mapping.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/src/alphafold/model/model.py` & `alphapulldown-0.30.5/alphafold/alphafold/model/model.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/src/alphafold/model/modules.py` & `alphapulldown-0.30.5/alphafold/alphafold/model/modules.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/src/alphafold/model/modules_multimer.py` & `alphapulldown-0.30.5/alphafold/alphafold/model/modules_multimer.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/src/alphafold/model/prng.py` & `alphapulldown-0.30.5/alphafold/alphafold/model/prng.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/src/alphafold/model/prng_test.py` & `alphapulldown-0.30.5/alphafold/alphafold/model/prng_test.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/src/alphafold/model/quat_affine.py` & `alphapulldown-0.30.5/alphafold/alphafold/model/quat_affine.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/src/alphafold/model/quat_affine_test.py` & `alphapulldown-0.30.5/alphafold/alphafold/model/quat_affine_test.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/src/alphafold/model/r3.py` & `alphapulldown-0.30.5/alphafold/alphafold/model/r3.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/src/alphafold/model/tf/__init__.py` & `alphapulldown-0.30.5/alphafold/alphafold/model/tf/__init__.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/src/alphafold/model/tf/data_transforms.py` & `alphapulldown-0.30.5/alphafold/alphafold/model/tf/data_transforms.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/src/alphafold/model/tf/input_pipeline.py` & `alphapulldown-0.30.5/alphafold/alphafold/model/tf/input_pipeline.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/src/alphafold/model/tf/protein_features.py` & `alphapulldown-0.30.5/alphafold/alphafold/model/tf/protein_features.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/src/alphafold/model/tf/protein_features_test.py` & `alphapulldown-0.30.5/alphafold/alphafold/model/tf/protein_features_test.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/src/alphafold/model/tf/proteins_dataset.py` & `alphapulldown-0.30.5/alphafold/alphafold/model/tf/proteins_dataset.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/src/alphafold/model/tf/shape_helpers.py` & `alphapulldown-0.30.5/alphafold/alphafold/model/tf/shape_helpers.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/src/alphafold/model/tf/shape_helpers_test.py` & `alphapulldown-0.30.5/alphafold/alphafold/model/tf/shape_helpers_test.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/src/alphafold/model/tf/shape_placeholders.py` & `alphapulldown-0.30.5/alphafold/alphafold/model/tf/shape_placeholders.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/src/alphafold/model/tf/utils.py` & `alphapulldown-0.30.5/alphafold/alphafold/model/tf/utils.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/src/alphafold/model/utils.py` & `alphapulldown-0.30.5/alphafold/alphafold/model/utils.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/src/alphafold/notebooks/__init__.py` & `alphapulldown-0.30.5/alphafold/alphafold/notebooks/__init__.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/src/alphafold/notebooks/notebook_utils.py` & `alphapulldown-0.30.5/alphafold/alphafold/notebooks/notebook_utils.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/src/alphafold/notebooks/notebook_utils_test.py` & `alphapulldown-0.30.5/alphafold/alphafold/notebooks/notebook_utils_test.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/src/alphafold/relax/__init__.py` & `alphapulldown-0.30.5/alphafold/alphafold/relax/__init__.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/src/alphafold/relax/amber_minimize.py` & `alphapulldown-0.30.5/alphafold/alphafold/relax/amber_minimize.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/src/alphafold/relax/amber_minimize_test.py` & `alphapulldown-0.30.5/alphafold/alphafold/relax/amber_minimize_test.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/src/alphafold/relax/cleanup.py` & `alphapulldown-0.30.5/alphafold/alphafold/relax/cleanup.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/src/alphafold/relax/cleanup_test.py` & `alphapulldown-0.30.5/alphafold/alphafold/relax/cleanup_test.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/src/alphafold/relax/relax.py` & `alphapulldown-0.30.5/alphafold/alphafold/relax/relax.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/src/alphafold/relax/relax_test.py` & `alphapulldown-0.30.5/alphafold/alphafold/relax/relax_test.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/src/alphafold/relax/utils.py` & `alphapulldown-0.30.5/alphafold/alphafold/relax/utils.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/src/alphafold/relax/utils_test.py` & `alphapulldown-0.30.5/alphafold/alphafold/relax/utils_test.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/src/alphafold/run_alphafold.py` & `alphapulldown-0.30.5/alphafold/run_alphafold.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/src/alphapulldown/colab_batch_no_prediction.py` & `alphapulldown-0.30.5/alphapulldown/colab_batch_no_prediction.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/src/alphapulldown/create_individual_features.py` & `alphapulldown-0.30.5/alphafold/data/pipeline.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,288 +1,243 @@
-#!/usr/bin/env python3
+# Copyright 2021 DeepMind Technologies Limited
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#      http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 
-# Author Dingquan Yu
-# This script is just to create msa and structural features for each sequences and store them in pickle
-# #
+"""Functions for building the input features for the AlphaFold model."""
 
 import os
-import pickle
-import sys
-from alphapulldown.objects import MonomericObject
-import importlib
-from absl import app
-from absl import flags
+from typing import Any, Mapping, MutableMapping, Optional, Sequence, Union
 from absl import logging
-
-from alphafold.data.pipeline import DataPipeline
-from alphafold.data.tools import hmmsearch
+from alphafold.common import residue_constants
+from alphafold.data import msa_identifiers
+from alphafold.data import parsers
 from alphafold.data import templates
+from alphafold.data.tools import hhblits
+from alphafold.data.tools import hhsearch
+from alphafold.data.tools import hmmsearch
+from alphafold.data.tools import jackhmmer
 import numpy as np
-import os
-from absl import logging, app
-import numpy as np
-from alphapulldown.utils import *
-import contextlib
-from datetime import datetime
-import alphafold
-from pathlib import Path
-from colabfold.utils import DEFAULT_API_SERVER
-
-@contextlib.contextmanager
-def output_meta_file(file_path):
-    """function that create temp file"""
-    with open(file_path, "w") as outfile:
-        yield outfile.name
-
-
-def load_module(file_name, module_name):
-    spec = importlib.util.spec_from_file_location(module_name, file_name)
-    module = importlib.util.module_from_spec(spec)
-    sys.modules[module_name] = module
-    spec.loader.exec_module(module)
-    return module
-
-
-PATH_TO_RUN_ALPHAFOLD = os.path.join(
-    os.path.dirname(alphafold.__file__), "run_alphafold.py"
-)
-
-try:
-    run_af = load_module(PATH_TO_RUN_ALPHAFOLD, "run_alphafold")
-except FileNotFoundError:
-    PATH_TO_RUN_ALPHAFOLD = os.path.join(
-        os.path.dirname(os.path.dirname(alphafold.__file__)), "run_alphafold.py"
-    )
-
-    run_af = load_module(PATH_TO_RUN_ALPHAFOLD, "run_alphafold")
-
-
-flags = run_af.flags
-flags.DEFINE_bool("save_msa_files", False, "save msa output or not")
-flags.DEFINE_bool(
-    "skip_existing", False, "skip existing monomer feature pickles or not"
-)
-flags.DEFINE_integer(
-    "seq_index", None, "index of sequence in the fasta file, starting from 1"
-)
-flags.DEFINE_string(
-    "new_uniclust_dir", None, "directory where new version of uniclust is stored"
-)
-flags.DEFINE_bool("use_mmseqs2",False,"Use mmseqs2 remotely or not. Default is False")
-
-FLAGS = flags.FLAGS
-MAX_TEMPLATE_HITS = 20
-
-flags_dict = FLAGS.flag_values_dict()
-
-def create_global_arguments(flags_dict):
-    global uniref90_database_path
-    global mgnify_database_path
-    global bfd_database_path
-    global small_bfd_database_path
-    global pdb_seqres_database_path
-    global template_mmcif_dir
-    global obsolete_pdbs_path
-    global pdb70_database_path
-    global use_small_bfd
-    global uniref30_database_path
-
-    # Path to the Uniref30 database for use by HHblits.
-    if FLAGS.uniref30_database_path is None:
-        uniref30_database_path = os.path.join(
-            FLAGS.data_dir, "uniref30", "UniRef30_2021_03"
-        )
-    else:
-        uniref30_database_path = FLAGS.uniref30_database_path
-    flags_dict.update({"uniref30_database_path": uniref30_database_path})
 
-    if FLAGS.uniref90_database_path is None:
-        uniref90_database_path = os.path.join(
-            FLAGS.data_dir, "uniref90", "uniref90.fasta"
-        )
-    else:
-        uniref90_database_path = FLAGS.uniref90_database_path
+# Internal import (7716).
 
-    flags_dict.update({"uniref90_database_path": uniref90_database_path})
+FeatureDict = MutableMapping[str, np.ndarray]
+TemplateSearcher = Union[hhsearch.HHSearch, hmmsearch.Hmmsearch]
 
-    # Path to the MGnify database for use by JackHMMER.
-    if FLAGS.mgnify_database_path is None:
-        mgnify_database_path = os.path.join(
-            FLAGS.data_dir, "mgnify", "mgy_clusters_2022_05.fa"
-        )
-    else:
-        mgnify_database_path = FLAGS.mgnify_database_path
-    flags_dict.update({"mgnify_database_path": mgnify_database_path})
 
-    # Path to the BFD database for use by HHblits.
-    if FLAGS.bfd_database_path is None:
-        bfd_database_path = os.path.join(
-            FLAGS.data_dir,
-            "bfd",
-            "bfd_metaclust_clu_complete_id30_c90_final_seq.sorted_opt",
-        )
-    else:
-        bfd_database_path = FLAGS.bfd_database_path
-    flags_dict.update({"bfd_database_path": bfd_database_path})
-
-    # Path to the Small BFD database for use by JackHMMER.
-    if FLAGS.small_bfd_database_path is None:
-        small_bfd_database_path = os.path.join(
-            FLAGS.data_dir, "small_bfd", "bfd-first_non_consensus_sequences.fasta"
-        )
-    else:
-        small_bfd_database_path = FLAGS.small_bfd_database_path
-    flags_dict.update({"small_bfd_database_path": small_bfd_database_path})
-
-    if FLAGS.pdb_seqres_database_path is None:
-        pdb_seqres_database_path = os.path.join(
-            FLAGS.data_dir, "pdb_seqres", "pdb_seqres.txt"
-        )
-    else:
-        pdb_seqres_database_path = FLAGS.pdb_seqres_database_path
-    flags_dict.update({"pdb_seqres_database_path": pdb_seqres_database_path})
-
-    # Path to a directory with template mmCIF structures, each named <pdb_id>.cif.
-    if FLAGS.template_mmcif_dir is None:
-        template_mmcif_dir = os.path.join(FLAGS.data_dir, "pdb_mmcif", "mmcif_files")
-    else:
-        template_mmcif_dir = FLAGS.template_mmcif_dir
-    flags_dict.update({"template_mmcif_dir": template_mmcif_dir})
-
-    # Path to a file mapping obsolete PDB IDs to their replacements.
-    if FLAGS.obsolete_pdbs_path is None:
-        obsolete_pdbs_path = os.path.join(FLAGS.data_dir, "pdb_mmcif", "obsolete.dat")
-    else:
-        obsolete_pdbs_path = FLAGS.obsolete_pdbs_path
-    flags_dict.update({"obsolete_pdbs_path": obsolete_pdbs_path})
-
-    # Path to pdb70 database
-    if FLAGS.pdb70_database_path is None:
-        pdb70_database_path = os.path.join(FLAGS.data_dir, "pdb70", "pdb70")
-    else:
-        pdb70_database_path = FLAGS.pdb70_database_path
-    flags_dict.update({"pdb70_database_path": pdb70_database_path})
-    use_small_bfd = FLAGS.db_preset == "reduced_dbs"
-
-def create_pipeline():
-    monomer_data_pipeline = DataPipeline(
-        jackhmmer_binary_path=FLAGS.jackhmmer_binary_path,
-        hhblits_binary_path=FLAGS.hhblits_binary_path,
-        uniref90_database_path=uniref90_database_path,
-        mgnify_database_path=mgnify_database_path,
-        bfd_database_path=bfd_database_path,
-        uniref30_database_path=uniref30_database_path,
-        small_bfd_database_path=small_bfd_database_path,
-        use_small_bfd=use_small_bfd,
-        use_precomputed_msas=FLAGS.use_precomputed_msas,
-        template_searcher=hmmsearch.Hmmsearch(
-            binary_path=FLAGS.hmmsearch_binary_path,
-            hmmbuild_binary_path=FLAGS.hmmbuild_binary_path,
-            database_path=pdb_seqres_database_path,
-        ),
-        template_featurizer=templates.HmmsearchHitFeaturizer(
-            mmcif_dir=template_mmcif_dir,
-            max_template_date=FLAGS.max_template_date,
-            max_hits=MAX_TEMPLATE_HITS,
-            kalign_binary_path=FLAGS.kalign_binary_path,
-            obsolete_pdbs_path=obsolete_pdbs_path,
-            release_dates_path=None,
-        ),
-    )
-    return monomer_data_pipeline
-
-
-def check_existing_objects(output_dir, pickle_name):
-    """check whether the wanted monomer object already exists in the output_dir"""
-    return os.path.isfile(os.path.join(output_dir, pickle_name))
-
-
-def create_and_save_monomer_objects(m, pipeline, flags_dict,use_mmseqs2=False):
-    logging.info("You are using the new version")
-    if FLAGS.skip_existing and check_existing_objects(
-        FLAGS.output_dir, f"{m.description}.pkl"
-    ):
-        logging.info(f"Already found {m.description}.pkl in {FLAGS.output_dir} Skipped")
-        pass
-    else:
-        metadata_output_path = os.path.join(
-            FLAGS.output_dir,
-            f"{m.description}_feature_metadata_{datetime.date(datetime.now())}.txt",
-        )
-        with output_meta_file(metadata_output_path) as meta_data_outfile:
-            save_meta_data(flags_dict, meta_data_outfile)
-
-        if not use_mmseqs2:
-            m.make_features(
-                pipeline,
-                output_dir=FLAGS.output_dir,
-                use_precomputed_msa=FLAGS.use_precomputed_msas,
-                save_msa=FLAGS.save_msa_files,
-            )
-        else:
-            logging.info("running mmseq now")
-            m.make_mmseq_features(DEFAULT_API_SERVER=DEFAULT_API_SERVER,
-            pdb70_database_path=pdb70_database_path,
-            template_mmcif_dir=template_mmcif_dir,
-            max_template_date=FLAGS.max_template_date,
-            output_dir=FLAGS.output_dir,
-            obsolete_pdbs_path=FLAGS.obsolete_pdbs_path
-            )
-        pickle.dump(m, open(f"{FLAGS.output_dir}/{m.description}.pkl", "wb"))
-        del m
-
-
-def iter_seqs(fasta_fns):
-    for fasta_path in fasta_fns:
-        with open(fasta_path, "r") as f:
-            sequences, descriptions = parse_fasta(f.read())
-            for seq, desc in zip(sequences, descriptions):
-                yield seq, desc
-
-def main(argv):
-    try:
-        Path(FLAGS.output_dir).mkdir(parents=True, exist_ok=True)
-    except FileExistsError:
-        logging.info("Multiple processes are trying to create the same folder now.")
-
-    flags_dict = FLAGS.flag_values_dict()
-    create_global_arguments(flags_dict)
-    if not FLAGS.use_mmseqs2:
-        if not FLAGS.max_template_date:
-            logging.info("You have not provided a max_template_date. Please specify a date and run again.")
-            sys.exit()
-        else:
-            pipeline = create_pipeline()
-            uniprot_database_path = os.path.join(FLAGS.data_dir, "uniprot/uniprot.fasta")
-            flags_dict.update({"uniprot_database_path": uniprot_database_path})
-            if os.path.isfile(uniprot_database_path):
-                uniprot_runner = create_uniprot_runner(
-                    FLAGS.jackhmmer_binary_path, uniprot_database_path
-                )
-            else:
-                logging.info(
-                    f"Failed to find uniprot.fasta under {uniprot_database_path}. Please make sure your data_dir has been configured correctly."
-                )
-                sys.exit()
-    else:
+def make_sequence_features(
+    sequence: str, description: str, num_res: int) -> FeatureDict:
+  """Constructs a feature dict of sequence features."""
+  features = {}
+  features['aatype'] = residue_constants.sequence_to_onehot(
+      sequence=sequence,
+      mapping=residue_constants.restype_order_with_x,
+      map_unknown_to_x=True)
+  features['between_segment_residues'] = np.zeros((num_res,), dtype=np.int32)
+  features['domain_name'] = np.array([description.encode('utf-8')],
+                                     dtype=np.object_)
+  features['residue_index'] = np.array(range(num_res), dtype=np.int32)
+  features['seq_length'] = np.array([num_res] * num_res, dtype=np.int32)
+  features['sequence'] = np.array([sequence.encode('utf-8')], dtype=np.object_)
+  return features
+
+
+def make_msa_features(msas: Sequence[parsers.Msa]) -> FeatureDict:
+  """Constructs a feature dict of MSA features."""
+  if not msas:
+    raise ValueError('At least one MSA must be provided.')
+
+  int_msa = []
+  deletion_matrix = []
+  species_ids = []
+  seen_sequences = set()
+  for msa_index, msa in enumerate(msas):
+    if not msa:
+      raise ValueError(f'MSA {msa_index} must contain at least one sequence.')
+    for sequence_index, sequence in enumerate(msa.sequences):
+      if sequence in seen_sequences:
+        continue
+      seen_sequences.add(sequence)
+      int_msa.append(
+          [residue_constants.HHBLITS_AA_TO_ID[res] for res in sequence])
+      deletion_matrix.append(msa.deletion_matrix[sequence_index])
+      identifiers = msa_identifiers.get_identifiers(
+          msa.descriptions[sequence_index])
+      species_ids.append(identifiers.species_id.encode('utf-8'))
+
+  num_res = len(msas[0].sequences[0])
+  num_alignments = len(int_msa)
+  features = {}
+  features['deletion_matrix_int'] = np.array(deletion_matrix, dtype=np.int32)
+  features['msa'] = np.array(int_msa, dtype=np.int32)
+  features['num_alignments'] = np.array(
+      [num_alignments] * num_res, dtype=np.int32)
+  features['msa_species_identifiers'] = np.array(species_ids, dtype=np.object_)
+  return features
+
+
+def run_msa_tool(msa_runner, input_fasta_path: str, msa_out_path: str,
+                 msa_format: str, use_precomputed_msas: bool,
+                 max_sto_sequences: Optional[int] = None
+                 ) -> Mapping[str, Any]:
+  """Runs an MSA tool, checking if output already exists first."""
+  if not use_precomputed_msas or not os.path.exists(msa_out_path):
+    if msa_format == 'sto' and max_sto_sequences is not None:
+      result = msa_runner.query(input_fasta_path, max_sto_sequences)[0]  # pytype: disable=wrong-arg-count
+    else:
+      result = msa_runner.query(input_fasta_path)[0]
+    with open(msa_out_path, 'w') as f:
+      f.write(result[msa_format])
+  else:
+    logging.warning('Reading MSA from file %s', msa_out_path)
+    if msa_format == 'sto' and max_sto_sequences is not None:
+      precomputed_msa = parsers.truncate_stockholm_msa(
+          msa_out_path, max_sto_sequences)
+      result = {'sto': precomputed_msa}
+    else:
+      with open(msa_out_path, 'r') as f:
+        result = {msa_format: f.read()}
+  return result
+
+
+class DataPipeline:
+  """Runs the alignment tools and assembles the input features."""
+
+  def __init__(self,
+               jackhmmer_binary_path: str,
+               hhblits_binary_path: str,
+               uniref90_database_path: str,
+               mgnify_database_path: str,
+               bfd_database_path: Optional[str],
+               uniref30_database_path: Optional[str],
+               small_bfd_database_path: Optional[str],
+               template_searcher: TemplateSearcher,
+               template_featurizer: templates.TemplateHitFeaturizer,
+               use_small_bfd: bool,
+               mgnify_max_hits: int = 501,
+               uniref_max_hits: int = 10000,
+               use_precomputed_msas: bool = False):
+    """Initializes the data pipeline."""
+    self._use_small_bfd = use_small_bfd
+    self.jackhmmer_uniref90_runner = jackhmmer.Jackhmmer(
+        binary_path=jackhmmer_binary_path,
+        database_path=uniref90_database_path)
+    if use_small_bfd:
+      self.jackhmmer_small_bfd_runner = jackhmmer.Jackhmmer(
+          binary_path=jackhmmer_binary_path,
+          database_path=small_bfd_database_path)
+    else:
+      self.hhblits_bfd_uniref_runner = hhblits.HHBlits(
+          binary_path=hhblits_binary_path,
+          databases=[bfd_database_path, uniref30_database_path])
+    self.jackhmmer_mgnify_runner = jackhmmer.Jackhmmer(
+        binary_path=jackhmmer_binary_path,
+        database_path=mgnify_database_path)
+    self.template_searcher = template_searcher
+    self.template_featurizer = template_featurizer
+    self.mgnify_max_hits = mgnify_max_hits
+    self.uniref_max_hits = uniref_max_hits
+    self.use_precomputed_msas = use_precomputed_msas
+
+  def process(self, input_fasta_path: str, msa_output_dir: str) -> FeatureDict:
+    """Runs alignment tools on the input sequence and creates features."""
+    with open(input_fasta_path) as f:
+      input_fasta_str = f.read()
+    input_seqs, input_descs = parsers.parse_fasta(input_fasta_str)
+    if len(input_seqs) != 1:
+      raise ValueError(
+          f'More than one input sequence found in {input_fasta_path}.')
+    input_sequence = input_seqs[0]
+    input_description = input_descs[0]
+    num_res = len(input_sequence)
+
+    uniref90_out_path = os.path.join(msa_output_dir, 'uniref90_hits.sto')
+    jackhmmer_uniref90_result = run_msa_tool(
+        msa_runner=self.jackhmmer_uniref90_runner,
+        input_fasta_path=input_fasta_path,
+        msa_out_path=uniref90_out_path,
+        msa_format='sto',
+        use_precomputed_msas=self.use_precomputed_msas,
+        max_sto_sequences=self.uniref_max_hits)
+    mgnify_out_path = os.path.join(msa_output_dir, 'mgnify_hits.sto')
+    jackhmmer_mgnify_result = run_msa_tool(
+        msa_runner=self.jackhmmer_mgnify_runner,
+        input_fasta_path=input_fasta_path,
+        msa_out_path=mgnify_out_path,
+        msa_format='sto',
+        use_precomputed_msas=self.use_precomputed_msas,
+        max_sto_sequences=self.mgnify_max_hits)
+
+    msa_for_templates = jackhmmer_uniref90_result['sto']
+    msa_for_templates = parsers.deduplicate_stockholm_msa(msa_for_templates)
+    msa_for_templates = parsers.remove_empty_columns_from_stockholm_msa(
+        msa_for_templates)
+
+    if self.template_searcher.input_format == 'sto':
+      pdb_templates_result = self.template_searcher.query(msa_for_templates)
+    elif self.template_searcher.input_format == 'a3m':
+      uniref90_msa_as_a3m = parsers.convert_stockholm_to_a3m(msa_for_templates)
+      pdb_templates_result = self.template_searcher.query(uniref90_msa_as_a3m)
+    else:
+      raise ValueError('Unrecognized template input format: '
+                       f'{self.template_searcher.input_format}')
+
+    pdb_hits_out_path = os.path.join(
+        msa_output_dir, f'pdb_hits.{self.template_searcher.output_format}')
+    with open(pdb_hits_out_path, 'w') as f:
+      f.write(pdb_templates_result)
+
+    uniref90_msa = parsers.parse_stockholm(jackhmmer_uniref90_result['sto'])
+    mgnify_msa = parsers.parse_stockholm(jackhmmer_mgnify_result['sto'])
+
+    pdb_template_hits = self.template_searcher.get_template_hits(
+        output_string=pdb_templates_result, input_sequence=input_sequence)
+
+    if self._use_small_bfd:
+      bfd_out_path = os.path.join(msa_output_dir, 'small_bfd_hits.sto')
+      jackhmmer_small_bfd_result = run_msa_tool(
+          msa_runner=self.jackhmmer_small_bfd_runner,
+          input_fasta_path=input_fasta_path,
+          msa_out_path=bfd_out_path,
+          msa_format='sto',
+          use_precomputed_msas=self.use_precomputed_msas)
+      bfd_msa = parsers.parse_stockholm(jackhmmer_small_bfd_result['sto'])
+    else:
+      bfd_out_path = os.path.join(msa_output_dir, 'bfd_uniref_hits.a3m')
+      hhblits_bfd_uniref_result = run_msa_tool(
+          msa_runner=self.hhblits_bfd_uniref_runner,
+          input_fasta_path=input_fasta_path,
+          msa_out_path=bfd_out_path,
+          msa_format='a3m',
+          use_precomputed_msas=self.use_precomputed_msas)
+      bfd_msa = parsers.parse_a3m(hhblits_bfd_uniref_result['a3m'])
+
+    templates_result = self.template_featurizer.get_templates(
+        query_sequence=input_sequence,
+        hits=pdb_template_hits)
+
+    sequence_features = make_sequence_features(
+        sequence=input_sequence,
+        description=input_description,
+        num_res=num_res)
+
+    msa_features = make_msa_features((uniref90_msa, bfd_msa, mgnify_msa))
+
+    logging.info('Uniref90 MSA size: %d sequences.', len(uniref90_msa))
+    logging.info('BFD MSA size: %d sequences.', len(bfd_msa))
+    logging.info('MGnify MSA size: %d sequences.', len(mgnify_msa))
+    logging.info('Final (deduplicated) MSA size: %d sequences.',
+                 msa_features['num_alignments'][0])
+    logging.info('Total number of templates (NB: this can include bad '
+                 'templates and is later filtered to top 4): %d.',
+                 templates_result.features['template_domain_names'].shape[0])
 
-        pipeline=None
-        uniprot_runner=None
-        flags_dict=FLAGS.flag_values_dict()
-
-    seq_idx = 0
-    for curr_seq, curr_desc in iter_seqs(FLAGS.fasta_paths):
-        seq_idx = seq_idx + 1 #yes, we're counting from 1
-        if FLAGS.seq_index is None or \
-            (FLAGS.seq_index == seq_idx):
-                if curr_desc and not curr_desc.isspace():
-                    curr_monomer = MonomericObject(curr_desc, curr_seq)
-                    curr_monomer.uniprot_runner = uniprot_runner
-                    create_and_save_monomer_objects(curr_monomer, pipeline,
-                    flags_dict,use_mmseqs2=FLAGS.use_mmseqs2)
-
-
-if __name__ == "__main__":
-    flags.mark_flags_as_required(
-        ["fasta_paths", "output_dir","max_template_date","data_dir"]
-    )
-    app.run(main)
+    return {**sequence_features, **msa_features, **templates_result.features}
```

### Comparing `alphapulldown-0.30.4/src/alphapulldown/objects.py` & `alphapulldown-0.30.5/alphapulldown/objects.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/src/alphapulldown/plot_pae.py` & `alphapulldown-0.30.5/alphapulldown/plot_pae.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/src/alphapulldown/predict_structure.py` & `alphapulldown-0.30.5/alphapulldown/predict_structure.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,193 +1,246 @@
 #
-# Authorship belongs to DeepMind
-# based on run_alphafold.py from https://github.com/deepmind/alphafold
+# This script is
+# based on run_alphafold.py by DeepMind from https://github.com/deepmind/alphafold
+# and contains code copied from the script run_alphafold.py.
 # #
 import json
 import os
 import pickle
 import time
 from absl import logging
 from alphafold.common import protein
 from alphafold.common import residue_constants
+from alphafold.relax import relax
 import numpy as np
-import json
+from alphapulldown.utils import get_run_alphafold
+
+run_af = get_run_alphafold()
+
+RELAX_MAX_ITERATIONS = run_af.RELAX_MAX_ITERATIONS
+RELAX_ENERGY_TOLERANCE = run_af.RELAX_ENERGY_TOLERANCE
+RELAX_STIFFNESS = run_af.RELAX_STIFFNESS
+RELAX_EXCLUDE_RESIDUES = run_af.RELAX_EXCLUDE_RESIDUES
+RELAX_MAX_OUTER_ITERATIONS = run_af.RELAX_MAX_OUTER_ITERATIONS
+
+ModelsToRelax = run_af.ModelsToRelax
+
+def get_score_from_result_pkl(pkl_path):
+    """Get the score from the model result pkl file"""
+
+    with open(pkl_path, "rb") as f:
+        result = pickle.load(f)
+    if "iptm" in result:
+        score_type = "iptm+ptm"
+        score = 0.8 * result["iptm"] + 0.2 * result["ptm"]
+    else:
+        score_type = "plddt"
+        score = result["plddt"]
+
+    return score_type, score
+
+def get_existing_model_info(output_dir, model_runners):
+    ranking_confidences = {}
+    unrelaxed_proteins = {}
+    unrelaxed_pdbs = {}
+    processed_models = 0
+
+    for model_name, _ in model_runners.items():
+        pdb_path = os.path.join(output_dir, f"unrelaxed_{model_name}.pdb")
+        pkl_path = os.path.join(output_dir, f"result_{model_name}.pkl")
+
+        if not (os.path.exists(pdb_path) and os.path.exists(pkl_path)):
+            break
+
+        try:
+            with open(pkl_path, "rb") as f:
+                result = pickle.load(f)
+        except (EOFError, pickle.UnpicklingError):
+            break
 
-MAX_TEMPLATE_HITS = 20
-RELAX_MAX_ITERATIONS = 0
-RELAX_ENERGY_TOLERANCE = 2.39
-RELAX_STIFFNESS = 10.0
-RELAX_EXCLUDE_RESIDUES = []
-RELAX_MAX_OUTER_ITERATIONS = 3
+        score_name, score = get_score_from_result_pkl(pkl_path)
+        ranking_confidences[model_name] = score
 
+        with open(pdb_path, "r") as f:
+            unrelaxed_pdb_str = f.read()
+        unrelaxed_proteins[model_name] = protein.from_pdb_string(unrelaxed_pdb_str)
+        unrelaxed_pdbs[model_name] = unrelaxed_pdb_str
+
+        processed_models += 1
+
+    return ranking_confidences, unrelaxed_proteins, unrelaxed_pdbs, processed_models
 
 def predict(
     model_runners,
     output_dir,
     feature_dict,
     random_seed,
     benchmark,
-    amber_relaxer,
+    models_to_relax: ModelsToRelax,
     fasta_name,
     allow_resume=True,
     seqs=[],
+    use_gpu_relax=True
 ):
     timings = {}
     unrelaxed_pdbs = {}
     relaxed_pdbs = {}
+    relax_metrics = {}
     ranking_confidences = {}
     unrelaxed_proteins = {}
+    START = 0
+    ranking_output_path = os.path.join(output_dir, "ranking_debug.json")
+    temp_timings_output_path = os.path.join(output_dir, "timings_temp.json") #To keep track of timings in case of crash and resume
+
     if allow_resume:
-        logging.info("Checking for %s", os.path.join(output_dir, "ranking_debug.json"))
-    if (
-        not os.path.exists(os.path.join(output_dir, "ranking_debug.json"))
-        or not allow_resume
-    ):
-        # Run the models.
-        num_models = len(model_runners)
-        for model_index, (model_name, model_runner) in enumerate(model_runners.items()):
-            logging.info("Running model %s on %s", model_name, fasta_name)
-            t_0 = time.time()
-            model_random_seed = model_index + random_seed * num_models
-            processed_feature_dict = model_runner.process_features(
-                feature_dict, random_seed=model_random_seed
+        logging.info("Checking for existing results")
+        ranking_confidences, unrelaxed_proteins, unrelaxed_pdbs, START = get_existing_model_info(output_dir, model_runners)
+
+        if os.path.exists(ranking_output_path) and len(unrelaxed_pdbs) == len(model_runners):
+            logging.info(
+                "ranking_debug.json exists. Skipping prediction. Restoring unrelaxed predictions and ranked order"
             )
-            timings[f"process_features_{model_name}"] = time.time() - t_0
+            START = len(model_runners)
+        elif START > 0:
+            logging.info("Found existing results, continuing from there.")
+
+    num_models = len(model_runners)
+    for model_index, (model_name, model_runner) in enumerate(model_runners.items()):
+        if model_index < START:
+            continue
+        logging.info("Running model %s on %s", model_name, fasta_name)
+        t_0 = time.time()
+        model_random_seed = model_index + random_seed * num_models
+        processed_feature_dict = model_runner.process_features(
+            feature_dict, random_seed=model_random_seed
+        )
+        timings[f"process_features_{model_name}"] = time.time() - t_0
+
+        t_0 = time.time()
+        prediction_result = model_runner.predict(
+            processed_feature_dict, random_seed=model_random_seed
+        )
+
+        # update prediction_result with input seqs
+        prediction_result.update({"seqs": seqs})
 
+        t_diff = time.time() - t_0
+        timings[f"predict_and_compile_{model_name}"] = t_diff
+        logging.info(
+            "Total JAX model %s on %s predict time (includes compilation time, see --benchmark): %.1fs",
+            model_name,
+            fasta_name,
+            t_diff,
+        )
+
+        if benchmark:
             t_0 = time.time()
-            prediction_result = model_runner.predict(
+            model_runner.predict(
                 processed_feature_dict, random_seed=model_random_seed
             )
-
-            # update prediction_result with input seqs
-            prediction_result.update({"seqs": seqs})
             t_diff = time.time() - t_0
-            timings[f"predict_and_compile_{model_name}"] = t_diff
+            timings[f"predict_benchmark_{model_name}"] = t_diff
             logging.info(
-                "Total JAX model %s on %s predict time (includes compilation time, see --benchmark): %.1fs",
+                "Total JAX model %s on %s predict time (excludes compilation time): %.1fs",
                 model_name,
                 fasta_name,
                 t_diff,
             )
 
-            if benchmark:
-                t_0 = time.time()
-                model_runner.predict(
-                    processed_feature_dict, random_seed=model_random_seed
-                )
-                t_diff = time.time() - t_0
-                timings[f"predict_benchmark_{model_name}"] = t_diff
-                logging.info(
-                    "Total JAX model %s on %s predict time (excludes compilation time): %.1fs",
-                    model_name,
-                    fasta_name,
-                    t_diff,
-                )
-
-            plddt = prediction_result["plddt"]
-            ranking_confidences[model_name] = prediction_result["ranking_confidence"]
+        plddt = prediction_result["plddt"]
+        ranking_confidences[model_name] = prediction_result["ranking_confidence"]
 
-            result_output_path = os.path.join(output_dir, f"result_{model_name}.pkl")
-            with open(result_output_path, "wb") as f:
-                pickle.dump(prediction_result, f, protocol=4)
+        result_output_path = os.path.join(output_dir, f"result_{model_name}.pkl")
+        with open(result_output_path, "wb") as f:
+            pickle.dump(prediction_result, f, protocol=4)
 
-            plddt_b_factors = np.repeat(
-                plddt[:, None], residue_constants.atom_type_num, axis=-1
-            )
-            unrelaxed_protein = protein.from_prediction(
-                features=processed_feature_dict,
-                result=prediction_result,
-                b_factors=plddt_b_factors,
-                remove_leading_feature_dimension=not model_runner.multimer_mode,
-            )
-
-            unrelaxed_pdbs[model_name] = protein.to_pdb(unrelaxed_protein)
-            unrelaxed_pdb_path = os.path.join(output_dir, f"unrelaxed_{model_name}.pdb")
-            with open(unrelaxed_pdb_path, "w") as f:
-                f.write(unrelaxed_pdbs[model_name])
-
-            if amber_relaxer:
-                # Relax the prediction.
-                t_0 = time.time()
-                relaxed_pdb_str, _, _ = amber_relaxer.process(prot=unrelaxed_protein)
-                timings[f"relax_{model_name}"] = time.time() - t_0
-
-                relaxed_pdbs[model_name] = relaxed_pdb_str
-
-                # Save the relaxed PDB.
-                relaxed_output_path = os.path.join(
-                    output_dir, f"relaxed_{model_name}.pdb"
-                )
-                with open(relaxed_output_path, "w") as f:
-                    f.write(relaxed_pdb_str)
-        restored = False
-    else:
-        logging.info(
-            "ranking_debug.json exists. Skipped prediction. Restoring unrelaxed predictions and ranked order"
+        plddt_b_factors = np.repeat(
+            plddt[:, None], residue_constants.atom_type_num, axis=-1
+        )
+        unrelaxed_protein = protein.from_prediction(
+            features=processed_feature_dict,
+            result=prediction_result,
+            b_factors=plddt_b_factors,
+            remove_leading_feature_dimension=not model_runner.multimer_mode,
         )
-        ranking_file = open(os.path.join(output_dir, "ranking_debug.json"))
-        ranking_confidences_data = json.load(ranking_file)
-        ranking_confidences = ranking_confidences_data[
-            list(ranking_confidences_data.keys())[0]
-        ]
-        for model_index, (model_name, model_runner) in enumerate(model_runners.items()):
-            unrelaxed_pdb_path = os.path.join(output_dir, f"unrelaxed_{model_name}.pdb")
-            logging.info("Restored pdb %s ", unrelaxed_pdb_path)
-            logging.info(
-                "Restored confidence for model %s: %s",
-                model_name,
-                ranking_confidences[model_name],
-            )
-            with open(unrelaxed_pdb_path, "r") as f:
-                unrelaxed_pdb_str = f.read()
-            unrelaxed_proteins[model_name] = protein.from_pdb_string(unrelaxed_pdb_str)
-            unrelaxed_pdbs[model_name] = unrelaxed_pdb_str
-        logging.info("Finished restoring unrelaxed PDBs.")
-        restored = True
-        if amber_relaxer:
-            for model_index, (model_name, model_runner) in enumerate(
-                model_runners.items()
-            ):
-                # Relax the prediction.
-                t_0 = time.time()
-                relaxed_pdb_str, _, _ = amber_relaxer.process(
-                    prot=unrelaxed_proteins[model_name]
-                )
-                timings[f"relax_{model_name}"] = time.time() - t_0
-
-                relaxed_pdbs[model_name] = relaxed_pdb_str
 
-                # Save the relaxed PDB.
-                relaxed_output_path = os.path.join(
-                    output_dir, f"relaxed_{model_name}.pdb"
-                )
-                with open(relaxed_output_path, "w") as f:
-                    f.write(relaxed_pdb_str)
-    # Rank by model confidence and write out relaxed PDBs in rank order.
-    ranked_order = []
-    # pDockq_scores = {}
-    for idx, (model_name, _) in enumerate(
-        sorted(ranking_confidences.items(), key=lambda x: x[1], reverse=True)
-    ):
-        ranked_order.append(model_name)
-        ranked_output_path = os.path.join(output_dir, f"ranked_{idx}.pdb")
-        with open(ranked_output_path, "w") as f:
-            if amber_relaxer:
+        unrelaxed_proteins[model_name] = unrelaxed_protein
+        unrelaxed_pdbs[model_name] = protein.to_pdb(unrelaxed_protein)
+        unrelaxed_pdb_path = os.path.join(output_dir, f"unrelaxed_{model_name}.pdb")
+        with open(unrelaxed_pdb_path, "w") as f:
+            f.write(unrelaxed_pdbs[model_name])
+
+        with open(temp_timings_output_path, "w") as f:
+            f.write(json.dumps(timings, indent=4))
+
+
+    # Rank by model confidence.
+    ranked_order = [
+        model_name for model_name, confidence in
+        sorted(ranking_confidences.items(), key=lambda x: x[1], reverse=True)]
+
+    # Relax predictions.
+    amber_relaxer = relax.AmberRelaxation(
+        max_iterations=RELAX_MAX_ITERATIONS,
+        tolerance=RELAX_ENERGY_TOLERANCE,
+        stiffness=RELAX_STIFFNESS,
+        exclude_residues=RELAX_EXCLUDE_RESIDUES,
+        max_outer_iterations=RELAX_MAX_OUTER_ITERATIONS,
+        use_gpu=use_gpu_relax)
+
+    if models_to_relax == ModelsToRelax.BEST:
+        to_relax = [ranked_order[0]]
+    elif models_to_relax == ModelsToRelax.ALL:
+        to_relax = ranked_order
+    elif models_to_relax == ModelsToRelax.NONE:
+        to_relax = []
+
+    for model_name in to_relax:
+        t_0 = time.time()
+        relaxed_pdb_str, _, violations = amber_relaxer.process(
+            prot=unrelaxed_proteins[model_name])
+        relax_metrics[model_name] = {
+            'remaining_violations': violations,
+            'remaining_violations_count': sum(violations)
+        }
+        timings[f'relax_{model_name}'] = time.time() - t_0
+
+        relaxed_pdbs[model_name] = relaxed_pdb_str
+
+        # Save the relaxed PDB.
+        relaxed_output_path = os.path.join(
+            output_dir, f'relaxed_{model_name}.pdb')
+        with open(relaxed_output_path, 'w') as f:
+            f.write(relaxed_pdb_str)
+
+    # Write out relaxed PDBs in rank order.
+    for idx, model_name in enumerate(ranked_order):
+        ranked_output_path = os.path.join(output_dir, f'ranked_{idx}.pdb')
+        with open(ranked_output_path, 'w') as f:
+            if model_name in relaxed_pdbs:
                 f.write(relaxed_pdbs[model_name])
             else:
                 f.write(unrelaxed_pdbs[model_name])
 
-    ranking_output_path = os.path.join(output_dir, "ranking_debug.json")
-    if not restored:  # already exists if restored.
+    if not os.path.exists(ranking_output_path):  # already exists if restored.
         with open(ranking_output_path, "w") as f:
             label = "iptm+ptm" if "iptm" in prediction_result else "plddts"
             f.write(
                 json.dumps(
                     {label: ranking_confidences, "order": ranked_order}, indent=4
                 )
             )
 
     logging.info("Final timings for %s: %s", fasta_name, timings)
-
     timings_output_path = os.path.join(output_dir, "timings.json")
     with open(timings_output_path, "w") as f:
         f.write(json.dumps(timings, indent=4))
+    if models_to_relax != ModelsToRelax.NONE:
+        relax_metrics_path = os.path.join(output_dir, 'relax_metrics.json')
+        with open(relax_metrics_path, 'w') as f:
+            f.write(json.dumps(relax_metrics, indent=4))
+
+    if os.path.exists(temp_timings_output_path): #should not happen at this stage but just in case
+        try:
+            os.remove(temp_timings_output_path)
+        except OSError:
+            pass
```

### Comparing `alphapulldown-0.30.4/src/alphapulldown/utils.py` & `alphapulldown-0.30.5/alphapulldown/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,14 +15,17 @@
 from alphafold.model import data
 from alphafold.data import templates
 import random
 import sys
 from alphafold.data import parsers
 from pathlib import Path
 import numpy as np
+import importlib
+import alphafold
+import sys
 
 def create_uniprot_runner(jackhmmer_binary_path, uniprot_database_path):
     """create a uniprot runner object"""
     return jackhmmer.Jackhmmer(
         binary_path=jackhmmer_binary_path, database_path=uniprot_database_path
     )
 
@@ -51,15 +54,14 @@
     """
     Modified based upon colabfold mk_mock_template():
     https://github.com/sokrypton/ColabFold/blob/05c0cb38d002180da3b58cdc53ea45a6b2a62d31/colabfold/batch.py#L121-L155
     """
     num_temp=1 # number of fake templates
     ln = feature_dict['aatype'].shape[0]
     output_templates_sequence = "A" * ln
-    output_confidence_scores = np.full(ln, 1.0)
 
 
     templates_all_atom_positions = np.zeros(
         (ln, templates.residue_constants.atom_type_num, 3)
     )
     templates_all_atom_masks = np.zeros((ln, templates.residue_constants.atom_type_num))
     templates_aatype = templates.residue_constants.sequence_to_onehot(
@@ -70,19 +72,15 @@
             templates_all_atom_positions[None], [num_temp, 1, 1, 1]
         ),
         "template_all_atom_masks": np.tile(
             templates_all_atom_masks[None], [num_temp, 1, 1]
         ),
         "template_sequence": [f"none".encode()] * num_temp,
         "template_aatype": np.tile(np.array(templates_aatype)[None], [num_temp, 1, 1]),
-        "template_confidence_scores": np.tile(
-            output_confidence_scores[None], [num_temp, 1]
-        ),
         "template_domain_names": [f"none".encode()] * num_temp,
-        "template_release_date": [f"none".encode()] * num_temp,
         "template_sum_probs": np.zeros([num_temp], dtype=np.float32),
     }
     feature_dict.update(template_features)
     return feature_dict
 
 def load_monomer_objects(monomer_dir_dict, protein_name):
     """
@@ -299,7 +297,30 @@
             sequences.append("")
             continue
         elif not line:
             continue  # Skip blank lines.
         sequences[index] += line
 
     return sequences, descriptions
+
+def load_module(file_name, module_name):
+    spec = importlib.util.spec_from_file_location(module_name, file_name)
+    module = importlib.util.module_from_spec(spec)
+    sys.modules[module_name] = module
+    spec.loader.exec_module(module)
+    return module
+
+def get_run_alphafold():
+    PATH_TO_RUN_ALPHAFOLD = os.path.join(
+        os.path.dirname(alphafold.__file__), "run_alphafold.py"
+    )
+
+    try:
+        run_af = load_module(PATH_TO_RUN_ALPHAFOLD, "run_alphafold")
+    except FileNotFoundError:
+        PATH_TO_RUN_ALPHAFOLD = os.path.join(
+            os.path.dirname(os.path.dirname(alphafold.__file__)), "run_alphafold.py"
+        )
+
+        run_af = load_module(PATH_TO_RUN_ALPHAFOLD, "run_alphafold")
+
+    return run_af
```

### Comparing `alphapulldown-0.30.4/src/analysis_pipeline/af2_3dmol.py` & `alphapulldown-0.30.5/analysis_pipeline/af2_3dmol.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/src/analysis_pipeline/calculate_mpdockq.py` & `alphapulldown-0.30.5/analysis_pipeline/calculate_mpdockq.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/src/analysis_pipeline/get_good_inter_pae.py` & `alphapulldown-0.30.5/analysis_pipeline/get_good_inter_pae.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/src/analysis_pipeline/utils.py` & `alphapulldown-0.30.5/analysis_pipeline/utils.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/src/colabfold/alphafold/models.py` & `alphapulldown-0.30.5/colabfold/alphafold/models.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/src/colabfold/alphafold/msa.py` & `alphapulldown-0.30.5/colabfold/alphafold/msa.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/src/colabfold/batch.py` & `alphapulldown-0.30.5/colabfold/batch.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/src/colabfold/citations.py` & `alphapulldown-0.30.5/colabfold/citations.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/src/colabfold/colabfold.py` & `alphapulldown-0.30.5/colabfold/colabfold.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/src/colabfold/colabfold_alphafold.py` & `alphapulldown-0.30.5/colabfold/colabfold_alphafold.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/src/colabfold/download.py` & `alphapulldown-0.30.5/colabfold/download.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/src/colabfold/mmseqs/merge_and_split_msas.py` & `alphapulldown-0.30.5/colabfold/mmseqs/merge_and_split_msas.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/src/colabfold/mmseqs/search.py` & `alphapulldown-0.30.5/colabfold/mmseqs/search.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/src/colabfold/mmseqs/split_msas.py` & `alphapulldown-0.30.5/colabfold/mmseqs/split_msas.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/src/colabfold/pdb.py` & `alphapulldown-0.30.5/colabfold/pdb.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/src/colabfold/plot.py` & `alphapulldown-0.30.5/colabfold/plot.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/src/colabfold/utils.py` & `alphapulldown-0.30.5/colabfold/utils.py`

 * *Files identical despite different names*

### Comparing `alphapulldown-0.30.4/test/test_create_objects.py` & `alphapulldown-0.30.5/test/test_create_objects.py`

 * *Files identical despite different names*

