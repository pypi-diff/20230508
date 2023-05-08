# Comparing `tmp/optinist-0.3.2.tar.gz` & `tmp/optinist-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optinist-0.3.2.tar", last modified: Mon May  8 09:31:17 2023, max compression
+gzip compressed data, was "optinist-0.3.3.tar", last modified: Mon May  8 10:31:11 2023, max compression
```

## Comparing `optinist-0.3.2.tar` & `optinist-0.3.3.tar`

### file list

```diff
@@ -1,230 +1,230 @@
-drwxr-xr-x   0 rei_hashimoto   (501) staff       (20)        0 2023-05-08 09:31:17.532123 optinist-0.3.2/
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)    35149 2023-04-03 06:29:38.000000 optinist-0.3.2/LICENSE
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)       24 2023-04-03 06:29:38.000000 optinist-0.3.2/MANIFEST.in
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)     6471 2023-05-08 09:31:17.532231 optinist-0.3.2/PKG-INFO
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)     5764 2023-04-03 06:29:38.000000 optinist-0.3.2/README.md
-drwxr-xr-x   0 rei_hashimoto   (501) staff       (20)        0 2023-05-08 09:31:17.408744 optinist-0.3.2/optinist/
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)     1442 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/Snakefile
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)        0 2023-04-27 06:46:09.000000 optinist-0.3.2/optinist/__init__.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)      106 2023-05-08 09:22:45.000000 optinist-0.3.2/optinist/__main__.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)     2797 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/__main_unit__.py
-drwxr-xr-x   0 rei_hashimoto   (501) staff       (20)        0 2023-05-08 09:31:17.430176 optinist-0.3.2/optinist/api/
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)        0 2023-04-03 06:29:38.000000 optinist-0.3.2/optinist/api/__init__.py
-drwxr-xr-x   0 rei_hashimoto   (501) staff       (20)        0 2023-05-08 09:31:17.433918 optinist-0.3.2/optinist/api/config/
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)        0 2023-04-03 06:29:38.000000 optinist-0.3.2/optinist/api/config/__init__.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)      251 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/api/config/config_reader.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)      312 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/api/config/config_writer.py
-drwxr-xr-x   0 rei_hashimoto   (501) staff       (20)        0 2023-05-08 09:31:17.445499 optinist-0.3.2/optinist/api/dataclass/
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)        0 2023-04-26 03:06:45.000000 optinist-0.3.2/optinist/api/dataclass/__init__.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)      966 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/api/dataclass/bar.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)      209 2023-04-27 06:43:36.000000 optinist-0.3.2/optinist/api/dataclass/base.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)      382 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/api/dataclass/caiman.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)     1148 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/api/dataclass/csv.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)     1003 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/api/dataclass/dataclass.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)      786 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/api/dataclass/heatmap.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)      438 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/api/dataclass/html.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)     2268 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/api/dataclass/image.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)      190 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/api/dataclass/iscell.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)      369 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/api/dataclass/lccd.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)       61 2023-04-27 06:43:48.000000 optinist-0.3.2/optinist/api/dataclass/nwb.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)      543 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/api/dataclass/scatter.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)      375 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/api/dataclass/suite2p.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)     2323 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/api/dataclass/timeseries.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)      473 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/api/dataclass/utils.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)      873 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/api/dir_path.py
-drwxr-xr-x   0 rei_hashimoto   (501) staff       (20)        0 2023-05-08 09:31:17.448752 optinist-0.3.2/optinist/api/edit_ROI/
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)      212 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/api/edit_ROI/__init__.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)     3660 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/api/edit_ROI/edit_ROI.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)      662 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/api/edit_ROI/utils.py
-drwxr-xr-x   0 rei_hashimoto   (501) staff       (20)        0 2023-05-08 09:31:17.449169 optinist-0.3.2/optinist/api/edit_ROI/wrappers/
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)     1476 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/api/edit_ROI/wrappers/__init__.py
-drwxr-xr-x   0 rei_hashimoto   (501) staff       (20)        0 2023-05-08 09:31:17.450523 optinist-0.3.2/optinist/api/edit_ROI/wrappers/caiman_edit_roi/
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)      331 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/api/edit_ROI/wrappers/caiman_edit_roi/__init__.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)     1861 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/api/edit_ROI/wrappers/caiman_edit_roi/add_roi.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)     1047 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/api/edit_ROI/wrappers/caiman_edit_roi/delete_roi.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)     1711 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/api/edit_ROI/wrappers/caiman_edit_roi/merge_roi.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)     1223 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/api/edit_ROI/wrappers/caiman_edit_roi/utils.py
-drwxr-xr-x   0 rei_hashimoto   (501) staff       (20)        0 2023-05-08 09:31:17.451670 optinist-0.3.2/optinist/api/edit_ROI/wrappers/lccd_edit_roi/
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)      325 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/api/edit_ROI/wrappers/lccd_edit_roi/__init__.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)     2346 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/api/edit_ROI/wrappers/lccd_edit_roi/add_roi.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)     2238 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/api/edit_ROI/wrappers/lccd_edit_roi/delete_roi.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)     2515 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/api/edit_ROI/wrappers/lccd_edit_roi/merge_roi.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)      975 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/api/edit_ROI/wrappers/lccd_edit_roi/utils.py
-drwxr-xr-x   0 rei_hashimoto   (501) staff       (20)        0 2023-05-08 09:31:17.452799 optinist-0.3.2/optinist/api/edit_ROI/wrappers/suite2p_edit_roi/
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)      334 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/api/edit_ROI/wrappers/suite2p_edit_roi/__init__.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)     1989 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/api/edit_ROI/wrappers/suite2p_edit_roi/add_roi.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)     1017 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/api/edit_ROI/wrappers/suite2p_edit_roi/delete_roi.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)     4066 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/api/edit_ROI/wrappers/suite2p_edit_roi/merge_roi.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)     5580 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/api/edit_ROI/wrappers/suite2p_edit_roi/utils.py
-drwxr-xr-x   0 rei_hashimoto   (501) staff       (20)        0 2023-05-08 09:31:17.453960 optinist-0.3.2/optinist/api/experiment/
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)        0 2023-04-27 06:43:59.000000 optinist-0.3.2/optinist/api/experiment/__init__.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)      526 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/api/experiment/experiment.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)     1803 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/api/experiment/experiment_builder.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)     2650 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/api/experiment/experiment_reader.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)     2580 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/api/experiment/experiment_writer.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)     1610 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/api/logger.py
-drwxr-xr-x   0 rei_hashimoto   (501) staff       (20)        0 2023-05-08 09:31:17.459025 optinist-0.3.2/optinist/api/nwb/
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)        0 2023-04-03 06:29:38.000000 optinist-0.3.2/optinist/api/nwb/__init__.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)      344 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/api/nwb/nwb.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)    14552 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/api/nwb/nwb_creater.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)     1169 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/api/nwb/optinist_data.py
-drwxr-xr-x   0 rei_hashimoto   (501) staff       (20)        0 2023-05-08 09:31:17.460611 optinist-0.3.2/optinist/api/pickle/
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)        0 2023-04-27 06:44:16.000000 optinist-0.3.2/optinist/api/pickle/__init__.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)      156 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/api/pickle/pickle_reader.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)      687 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/api/pickle/pickle_writer.py
-drwxr-xr-x   0 rei_hashimoto   (501) staff       (20)        0 2023-05-08 09:31:17.465688 optinist-0.3.2/optinist/api/rules/
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)        0 2023-04-27 06:44:21.000000 optinist-0.3.2/optinist/api/rules/__init__.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)      171 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/api/rules/const.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)     1441 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/api/rules/data.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)      452 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/api/rules/edit_ROI.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)     2399 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/api/rules/file_writer.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)      867 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/api/rules/func.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)     3746 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/api/rules/runner.py
-drwxr-xr-x   0 rei_hashimoto   (501) staff       (20)        0 2023-05-08 09:31:17.470166 optinist-0.3.2/optinist/api/snakemake/
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)        0 2023-04-27 06:44:37.000000 optinist-0.3.2/optinist/api/snakemake/__init__.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)      631 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/api/snakemake/smk.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)     1476 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/api/snakemake/smk_builder.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)     1718 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/api/snakemake/smk_utils.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)     1723 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/api/snakemake/snakemake_executor.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)      814 2023-04-26 03:08:45.000000 optinist-0.3.2/optinist/api/snakemake/snakemake_reader.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)     2919 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/api/snakemake/snakemake_rule.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)      598 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/api/snakemake/snakemake_writer.py
-drwxr-xr-x   0 rei_hashimoto   (501) staff       (20)        0 2023-05-08 09:31:17.470804 optinist-0.3.2/optinist/api/utils/
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)        0 2023-04-03 06:29:38.000000 optinist-0.3.2/optinist/api/utils/__init__.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)      661 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/api/utils/filepath_creater.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)     1110 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/api/utils/json_writer.py
-drwxr-xr-x   0 rei_hashimoto   (501) staff       (20)        0 2023-05-08 09:31:17.471836 optinist-0.3.2/optinist/api/workflow/
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)        0 2023-04-03 06:29:38.000000 optinist-0.3.2/optinist/api/workflow/__init__.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)     1659 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/api/workflow/workflow.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)     1389 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/api/workflow/workflow_params.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)     5921 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/api/workflow/workflow_result.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)     4567 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/api/workflow/workflow_runner.py
-drwxr-xr-x   0 rei_hashimoto   (501) staff       (20)        0 2023-05-08 09:31:17.472103 optinist-0.3.2/optinist/app_config/
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)      139 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/app_config/logging.yaml
-drwxr-xr-x   0 rei_hashimoto   (501) staff       (20)        0 2023-05-08 09:31:17.473199 optinist-0.3.2/optinist/conda/
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)      124 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/conda/caiman_env.yaml
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)      153 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/conda/lccd_env.yaml
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)      117 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/conda/optinist_env.yaml
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)      202 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/conda/suite2p_env.yaml
-drwxr-xr-x   0 rei_hashimoto   (501) staff       (20)        0 2023-05-08 09:31:17.480158 optinist-0.3.2/optinist/config/
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)      110 2023-04-03 06:29:38.000000 optinist-0.3.2/optinist/config/caiman_cnmf.yaml
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)      362 2023-04-03 06:29:38.000000 optinist-0.3.2/optinist/config/caiman_mc.yaml
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)      224 2023-04-03 06:29:38.000000 optinist-0.3.2/optinist/config/cca.yaml
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)       59 2023-04-03 06:29:38.000000 optinist-0.3.2/optinist/config/cell_grouping.yaml
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)       15 2023-04-03 06:29:38.000000 optinist-0.3.2/optinist/config/correlation.yaml
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)      284 2023-04-03 06:29:38.000000 optinist-0.3.2/optinist/config/cross_correlation.yaml
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)       14 2023-04-03 06:29:38.000000 optinist-0.3.2/optinist/config/dummy_image2image.yaml
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)      149 2023-04-03 06:29:38.000000 optinist-0.3.2/optinist/config/eta.yaml
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)      232 2023-04-03 06:29:38.000000 optinist-0.3.2/optinist/config/glm.yaml
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)      521 2023-04-03 06:29:38.000000 optinist-0.3.2/optinist/config/granger.yaml
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)      280 2023-04-03 06:29:38.000000 optinist-0.3.2/optinist/config/lccd_cell_detection.yaml
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)      564 2023-04-03 06:29:38.000000 optinist-0.3.2/optinist/config/lda.yaml
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)      626 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/config/nwb.yaml
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)      223 2023-04-03 06:29:38.000000 optinist-0.3.2/optinist/config/pca.yaml
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)       71 2023-04-12 06:11:01.000000 optinist-0.3.2/optinist/config/snakemake.yaml
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)     6823 2023-04-03 06:29:38.000000 optinist-0.3.2/optinist/config/suite2p.yaml
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)       78 2023-04-03 06:29:38.000000 optinist-0.3.2/optinist/config/suite2p_file_convert.yaml
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)      385 2023-04-03 06:29:38.000000 optinist-0.3.2/optinist/config/suite2p_registration.yaml
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)     1520 2023-04-03 06:29:38.000000 optinist-0.3.2/optinist/config/suite2p_roi.yaml
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)      314 2023-04-03 06:29:38.000000 optinist-0.3.2/optinist/config/suite2p_spike_deconv.yaml
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)     1352 2023-04-03 06:29:38.000000 optinist-0.3.2/optinist/config/svm.yaml
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)      394 2023-04-03 06:29:38.000000 optinist-0.3.2/optinist/config/tsne.yaml
-drwxr-xr-x   0 rei_hashimoto   (501) staff       (20)        0 2023-05-08 09:31:17.397055 optinist-0.3.2/optinist/frontend/
-drwxr-xr-x   0 rei_hashimoto   (501) staff       (20)        0 2023-05-08 09:31:17.480816 optinist-0.3.2/optinist/frontend/build/
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)     1297 2023-05-08 09:31:08.000000 optinist-0.3.2/optinist/frontend/build/asset-manifest.json
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)     3044 2023-05-08 09:31:08.000000 optinist-0.3.2/optinist/frontend/build/index.html
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)       67 2023-05-08 09:31:08.000000 optinist-0.3.2/optinist/frontend/build/robots.txt
-drwxr-xr-x   0 rei_hashimoto   (501) staff       (20)        0 2023-05-08 09:31:17.481242 optinist-0.3.2/optinist/frontend/build/static/
-drwxr-xr-x   0 rei_hashimoto   (501) staff       (20)        0 2023-05-08 09:31:17.482072 optinist-0.3.2/optinist/frontend/build/static/css/
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)     2422 2023-05-08 09:31:08.000000 optinist-0.3.2/optinist/frontend/build/static/css/2.dab0dc93.chunk.css
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)     4696 2023-05-08 09:31:08.000000 optinist-0.3.2/optinist/frontend/build/static/css/2.dab0dc93.chunk.css.map
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)     1339 2023-05-08 09:31:08.000000 optinist-0.3.2/optinist/frontend/build/static/css/main.08a92549.chunk.css
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)     2652 2023-05-08 09:31:08.000000 optinist-0.3.2/optinist/frontend/build/static/css/main.08a92549.chunk.css.map
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)    16958 2023-05-08 09:31:08.000000 optinist-0.3.2/optinist/frontend/build/static/favicon.ico
-drwxr-xr-x   0 rei_hashimoto   (501) staff       (20)        0 2023-05-08 09:31:17.519161 optinist-0.3.2/optinist/frontend/build/static/js/
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)  5146283 2023-05-08 09:31:08.000000 optinist-0.3.2/optinist/frontend/build/static/js/2.d6a78225.chunk.js
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)     3922 2023-05-08 09:31:08.000000 optinist-0.3.2/optinist/frontend/build/static/js/2.d6a78225.chunk.js.LICENSE.txt
--rw-r--r--   0 rei_hashimoto   (501) staff       (20) 18935319 2023-05-08 09:31:08.000000 optinist-0.3.2/optinist/frontend/build/static/js/2.d6a78225.chunk.js.map
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)     4384 2023-05-08 09:31:08.000000 optinist-0.3.2/optinist/frontend/build/static/js/3.e6a5ade8.chunk.js
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)     9612 2023-05-08 09:31:08.000000 optinist-0.3.2/optinist/frontend/build/static/js/3.e6a5ade8.chunk.js.map
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)   178350 2023-05-08 09:31:08.000000 optinist-0.3.2/optinist/frontend/build/static/js/main.08115825.chunk.js
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)   644102 2023-05-08 09:31:08.000000 optinist-0.3.2/optinist/frontend/build/static/js/main.08115825.chunk.js.map
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)     2358 2023-05-08 09:31:08.000000 optinist-0.3.2/optinist/frontend/build/static/js/runtime-main.6a23d4cb.js
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)    12470 2023-05-08 09:31:08.000000 optinist-0.3.2/optinist/frontend/build/static/js/runtime-main.6a23d4cb.js.map
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)      290 2023-05-08 09:31:08.000000 optinist-0.3.2/optinist/frontend/build/static/manifest.json
-drwxr-xr-x   0 rei_hashimoto   (501) staff       (20)        0 2023-05-08 09:31:17.519399 optinist-0.3.2/optinist/frontend/build/static/media/
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)    80977 2023-05-08 09:31:08.000000 optinist-0.3.2/optinist/frontend/build/static/media/optinist.e44efe32.png
-drwxr-xr-x   0 rei_hashimoto   (501) staff       (20)        0 2023-05-08 09:31:17.522440 optinist-0.3.2/optinist/routers/
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)        0 2023-04-03 06:29:38.000000 optinist-0.3.2/optinist/routers/__init__.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)     2769 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/routers/algolist.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)      193 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/routers/const.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)     3367 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/routers/experiment.py
-drwxr-xr-x   0 rei_hashimoto   (501) staff       (20)        0 2023-05-08 09:31:17.522835 optinist-0.3.2/optinist/routers/fileIO/
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)        0 2023-04-03 06:29:38.000000 optinist-0.3.2/optinist/routers/fileIO/__init__.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)     1095 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/routers/fileIO/file_reader.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)     2888 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/routers/files.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)     2301 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/routers/hdf5.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)     2403 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/routers/model.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)     5735 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/routers/outputs.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)      961 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/routers/params.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)     1089 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/routers/run.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)      407 2023-05-08 09:22:45.000000 optinist-0.3.2/optinist/version.py
-drwxr-xr-x   0 rei_hashimoto   (501) staff       (20)        0 2023-05-08 09:31:17.523388 optinist-0.3.2/optinist/wrappers/
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)      564 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/wrappers/__init__.py
-drwxr-xr-x   0 rei_hashimoto   (501) staff       (20)        0 2023-05-08 09:31:17.524273 optinist-0.3.2/optinist/wrappers/caiman_wrapper/
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)      488 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/wrappers/caiman_wrapper/__init__.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)     7402 2023-05-08 07:31:55.000000 optinist-0.3.2/optinist/wrappers/caiman_wrapper/cnmf.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)     2321 2023-05-08 07:31:49.000000 optinist-0.3.2/optinist/wrappers/caiman_wrapper/motion_correction.py
-drwxr-xr-x   0 rei_hashimoto   (501) staff       (20)        0 2023-05-08 09:31:17.524788 optinist-0.3.2/optinist/wrappers/dummy_wrapper/
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)     1457 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/wrappers/dummy_wrapper/__init__.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)     5130 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/wrappers/dummy_wrapper/dummy.py
-drwxr-xr-x   0 rei_hashimoto   (501) staff       (20)        0 2023-05-08 09:31:17.525225 optinist-0.3.2/optinist/wrappers/lccd_wrapper/
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)      273 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/wrappers/lccd_wrapper/__init__.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)     3100 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/wrappers/lccd_wrapper/lccd_detection.py
-drwxr-xr-x   0 rei_hashimoto   (501) staff       (20)        0 2023-05-08 09:31:17.526633 optinist-0.3.2/optinist/wrappers/lccd_wrapper/lccd_python/
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)        0 2023-04-26 03:02:01.000000 optinist-0.3.2/optinist/wrappers/lccd_wrapper/lccd_python/__init__.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)     3534 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/wrappers/lccd_wrapper/lccd_python/blob_detector.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)     1837 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/wrappers/lccd_wrapper/lccd_python/lccd.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)     1916 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/wrappers/lccd_wrapper/lccd_python/oval_filter.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)     6128 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/wrappers/lccd_wrapper/lccd_python/roi_integration.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)     7279 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/wrappers/lccd_wrapper/lccd_python/utils.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)      391 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/wrappers/optinist_exception.py
-drwxr-xr-x   0 rei_hashimoto   (501) staff       (20)        0 2023-05-08 09:31:17.527081 optinist-0.3.2/optinist/wrappers/optinist_wrapper/
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)      769 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/wrappers/optinist_wrapper/__init__.py
-drwxr-xr-x   0 rei_hashimoto   (501) staff       (20)        0 2023-05-08 09:31:17.527781 optinist-0.3.2/optinist/wrappers/optinist_wrapper/basic_neural_analysis/
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)      330 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/wrappers/optinist_wrapper/basic_neural_analysis/__init__.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)      735 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/wrappers/optinist_wrapper/basic_neural_analysis/cell_grouping.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)     3444 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/wrappers/optinist_wrapper/basic_neural_analysis/eta.py
-drwxr-xr-x   0 rei_hashimoto   (501) staff       (20)        0 2023-05-08 09:31:17.528824 optinist-0.3.2/optinist/wrappers/optinist_wrapper/dimension_reduction/
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)      533 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/wrappers/optinist_wrapper/dimension_reduction/__init__.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)     2066 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/wrappers/optinist_wrapper/dimension_reduction/cca.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)     2090 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/wrappers/optinist_wrapper/dimension_reduction/pca.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)     1095 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/wrappers/optinist_wrapper/dimension_reduction/tsne.py
-drwxr-xr-x   0 rei_hashimoto   (501) staff       (20)        0 2023-05-08 09:31:17.529764 optinist-0.3.2/optinist/wrappers/optinist_wrapper/neural_decoding/
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)      513 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/wrappers/optinist_wrapper/neural_decoding/__init__.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)     3040 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/wrappers/optinist_wrapper/neural_decoding/glm.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)     2148 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/wrappers/optinist_wrapper/neural_decoding/lda.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)     2590 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/wrappers/optinist_wrapper/neural_decoding/svm.py
-drwxr-xr-x   0 rei_hashimoto   (501) staff       (20)        0 2023-05-08 09:31:17.530714 optinist-0.3.2/optinist/wrappers/optinist_wrapper/neural_population_analysis/
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)      659 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/wrappers/optinist_wrapper/neural_population_analysis/__init__.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)      938 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/wrappers/optinist_wrapper/neural_population_analysis/correlation.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)     3209 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/wrappers/optinist_wrapper/neural_population_analysis/cross_correlation.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)     6227 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/wrappers/optinist_wrapper/neural_population_analysis/granger.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)      184 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/wrappers/optinist_wrapper/utils.py
-drwxr-xr-x   0 rei_hashimoto   (501) staff       (20)        0 2023-05-08 09:31:17.531927 optinist-0.3.2/optinist/wrappers/suite2p_wrapper/
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)     1031 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/wrappers/suite2p_wrapper/__init__.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)     1236 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/wrappers/suite2p_wrapper/file_convert.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)      968 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/wrappers/suite2p_wrapper/registration.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)     3605 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/wrappers/suite2p_wrapper/roi.py
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)     1660 2023-05-08 04:38:25.000000 optinist-0.3.2/optinist/wrappers/suite2p_wrapper/spike_deconv.py
-drwxr-xr-x   0 rei_hashimoto   (501) staff       (20)        0 2023-05-08 09:31:17.426870 optinist-0.3.2/optinist.egg-info/
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)     6471 2023-05-08 09:31:17.000000 optinist-0.3.2/optinist.egg-info/PKG-INFO
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)     7657 2023-05-08 09:31:17.000000 optinist-0.3.2/optinist.egg-info/SOURCES.txt
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)        1 2023-05-08 09:31:17.000000 optinist-0.3.2/optinist.egg-info/dependency_links.txt
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)       56 2023-05-08 09:31:17.000000 optinist-0.3.2/optinist.egg-info/entry_points.txt
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)        1 2023-05-08 09:26:05.000000 optinist-0.3.2/optinist.egg-info/not-zip-safe
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)      171 2023-05-08 09:31:17.000000 optinist-0.3.2/optinist.egg-info/requires.txt
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)       19 2023-05-08 09:31:17.000000 optinist-0.3.2/optinist.egg-info/top_level.txt
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)      171 2023-05-08 04:38:25.000000 optinist-0.3.2/requirements.txt
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)      115 2023-05-08 09:31:17.532655 optinist-0.3.2/setup.cfg
--rw-r--r--   0 rei_hashimoto   (501) staff       (20)     2101 2023-05-08 09:22:45.000000 optinist-0.3.2/setup.py
+drwxr-xr-x   0 rei_hashimoto   (501) staff       (20)        0 2023-05-08 10:31:11.781785 optinist-0.3.3/
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)    35149 2023-04-03 06:29:38.000000 optinist-0.3.3/LICENSE
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)       24 2023-04-03 06:29:38.000000 optinist-0.3.3/MANIFEST.in
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)     6471 2023-05-08 10:31:11.781887 optinist-0.3.3/PKG-INFO
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)     5764 2023-04-03 06:29:38.000000 optinist-0.3.3/README.md
+drwxr-xr-x   0 rei_hashimoto   (501) staff       (20)        0 2023-05-08 10:31:11.725254 optinist-0.3.3/optinist/
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)     1442 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/Snakefile
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)        0 2023-04-27 06:46:09.000000 optinist-0.3.3/optinist/__init__.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)      106 2023-05-08 09:22:45.000000 optinist-0.3.3/optinist/__main__.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)     2797 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/__main_unit__.py
+drwxr-xr-x   0 rei_hashimoto   (501) staff       (20)        0 2023-05-08 10:31:11.727565 optinist-0.3.3/optinist/api/
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)        0 2023-04-03 06:29:38.000000 optinist-0.3.3/optinist/api/__init__.py
+drwxr-xr-x   0 rei_hashimoto   (501) staff       (20)        0 2023-05-08 10:31:11.728222 optinist-0.3.3/optinist/api/config/
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)        0 2023-04-03 06:29:38.000000 optinist-0.3.3/optinist/api/config/__init__.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)      251 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/api/config/config_reader.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)      312 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/api/config/config_writer.py
+drwxr-xr-x   0 rei_hashimoto   (501) staff       (20)        0 2023-05-08 10:31:11.732180 optinist-0.3.3/optinist/api/dataclass/
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)        0 2023-04-26 03:06:45.000000 optinist-0.3.3/optinist/api/dataclass/__init__.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)      966 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/api/dataclass/bar.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)      209 2023-04-27 06:43:36.000000 optinist-0.3.3/optinist/api/dataclass/base.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)      382 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/api/dataclass/caiman.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)     1148 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/api/dataclass/csv.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)     1003 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/api/dataclass/dataclass.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)      786 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/api/dataclass/heatmap.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)      438 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/api/dataclass/html.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)     2268 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/api/dataclass/image.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)      190 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/api/dataclass/iscell.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)      369 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/api/dataclass/lccd.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)       61 2023-04-27 06:43:48.000000 optinist-0.3.3/optinist/api/dataclass/nwb.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)      543 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/api/dataclass/scatter.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)      375 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/api/dataclass/suite2p.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)     2323 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/api/dataclass/timeseries.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)      473 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/api/dataclass/utils.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)      873 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/api/dir_path.py
+drwxr-xr-x   0 rei_hashimoto   (501) staff       (20)        0 2023-05-08 10:31:11.732838 optinist-0.3.3/optinist/api/edit_ROI/
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)      212 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/api/edit_ROI/__init__.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)     3660 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/api/edit_ROI/edit_ROI.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)      662 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/api/edit_ROI/utils.py
+drwxr-xr-x   0 rei_hashimoto   (501) staff       (20)        0 2023-05-08 10:31:11.733109 optinist-0.3.3/optinist/api/edit_ROI/wrappers/
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)     1476 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/api/edit_ROI/wrappers/__init__.py
+drwxr-xr-x   0 rei_hashimoto   (501) staff       (20)        0 2023-05-08 10:31:11.734230 optinist-0.3.3/optinist/api/edit_ROI/wrappers/caiman_edit_roi/
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)      331 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/api/edit_ROI/wrappers/caiman_edit_roi/__init__.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)     1861 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/api/edit_ROI/wrappers/caiman_edit_roi/add_roi.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)     1047 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/api/edit_ROI/wrappers/caiman_edit_roi/delete_roi.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)     1711 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/api/edit_ROI/wrappers/caiman_edit_roi/merge_roi.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)     1223 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/api/edit_ROI/wrappers/caiman_edit_roi/utils.py
+drwxr-xr-x   0 rei_hashimoto   (501) staff       (20)        0 2023-05-08 10:31:11.735357 optinist-0.3.3/optinist/api/edit_ROI/wrappers/lccd_edit_roi/
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)      325 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/api/edit_ROI/wrappers/lccd_edit_roi/__init__.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)     2346 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/api/edit_ROI/wrappers/lccd_edit_roi/add_roi.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)     2238 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/api/edit_ROI/wrappers/lccd_edit_roi/delete_roi.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)     2515 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/api/edit_ROI/wrappers/lccd_edit_roi/merge_roi.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)      975 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/api/edit_ROI/wrappers/lccd_edit_roi/utils.py
+drwxr-xr-x   0 rei_hashimoto   (501) staff       (20)        0 2023-05-08 10:31:11.736482 optinist-0.3.3/optinist/api/edit_ROI/wrappers/suite2p_edit_roi/
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)      334 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/api/edit_ROI/wrappers/suite2p_edit_roi/__init__.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)     1989 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/api/edit_ROI/wrappers/suite2p_edit_roi/add_roi.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)     1017 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/api/edit_ROI/wrappers/suite2p_edit_roi/delete_roi.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)     4066 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/api/edit_ROI/wrappers/suite2p_edit_roi/merge_roi.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)     5580 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/api/edit_ROI/wrappers/suite2p_edit_roi/utils.py
+drwxr-xr-x   0 rei_hashimoto   (501) staff       (20)        0 2023-05-08 10:31:11.738260 optinist-0.3.3/optinist/api/experiment/
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)        0 2023-04-27 06:43:59.000000 optinist-0.3.3/optinist/api/experiment/__init__.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)      526 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/api/experiment/experiment.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)     1803 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/api/experiment/experiment_builder.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)     2650 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/api/experiment/experiment_reader.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)     2580 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/api/experiment/experiment_writer.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)     1610 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/api/logger.py
+drwxr-xr-x   0 rei_hashimoto   (501) staff       (20)        0 2023-05-08 10:31:11.739082 optinist-0.3.3/optinist/api/nwb/
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)        0 2023-04-03 06:29:38.000000 optinist-0.3.3/optinist/api/nwb/__init__.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)      344 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/api/nwb/nwb.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)    14552 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/api/nwb/nwb_creater.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)     1169 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/api/nwb/optinist_data.py
+drwxr-xr-x   0 rei_hashimoto   (501) staff       (20)        0 2023-05-08 10:31:11.739847 optinist-0.3.3/optinist/api/pickle/
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)        0 2023-04-27 06:44:16.000000 optinist-0.3.3/optinist/api/pickle/__init__.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)      156 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/api/pickle/pickle_reader.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)      687 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/api/pickle/pickle_writer.py
+drwxr-xr-x   0 rei_hashimoto   (501) staff       (20)        0 2023-05-08 10:31:11.741433 optinist-0.3.3/optinist/api/rules/
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)        0 2023-04-27 06:44:21.000000 optinist-0.3.3/optinist/api/rules/__init__.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)      171 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/api/rules/const.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)     1441 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/api/rules/data.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)      452 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/api/rules/edit_ROI.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)     2399 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/api/rules/file_writer.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)      867 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/api/rules/func.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)     3746 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/api/rules/runner.py
+drwxr-xr-x   0 rei_hashimoto   (501) staff       (20)        0 2023-05-08 10:31:11.743137 optinist-0.3.3/optinist/api/snakemake/
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)        0 2023-04-27 06:44:37.000000 optinist-0.3.3/optinist/api/snakemake/__init__.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)      631 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/api/snakemake/smk.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)     1476 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/api/snakemake/smk_builder.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)     1718 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/api/snakemake/smk_utils.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)     1723 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/api/snakemake/snakemake_executor.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)      814 2023-04-26 03:08:45.000000 optinist-0.3.3/optinist/api/snakemake/snakemake_reader.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)     2919 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/api/snakemake/snakemake_rule.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)      598 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/api/snakemake/snakemake_writer.py
+drwxr-xr-x   0 rei_hashimoto   (501) staff       (20)        0 2023-05-08 10:31:11.743708 optinist-0.3.3/optinist/api/utils/
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)        0 2023-04-03 06:29:38.000000 optinist-0.3.3/optinist/api/utils/__init__.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)      661 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/api/utils/filepath_creater.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)     1110 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/api/utils/json_writer.py
+drwxr-xr-x   0 rei_hashimoto   (501) staff       (20)        0 2023-05-08 10:31:11.745202 optinist-0.3.3/optinist/api/workflow/
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)        0 2023-04-03 06:29:38.000000 optinist-0.3.3/optinist/api/workflow/__init__.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)     1659 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/api/workflow/workflow.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)     1389 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/api/workflow/workflow_params.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)     5921 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/api/workflow/workflow_result.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)     4567 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/api/workflow/workflow_runner.py
+drwxr-xr-x   0 rei_hashimoto   (501) staff       (20)        0 2023-05-08 10:31:11.745420 optinist-0.3.3/optinist/app_config/
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)      139 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/app_config/logging.yaml
+drwxr-xr-x   0 rei_hashimoto   (501) staff       (20)        0 2023-05-08 10:31:11.746624 optinist-0.3.3/optinist/conda/
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)      124 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/conda/caiman_env.yaml
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)      153 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/conda/lccd_env.yaml
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)      117 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/conda/optinist_env.yaml
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)      202 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/conda/suite2p_env.yaml
+drwxr-xr-x   0 rei_hashimoto   (501) staff       (20)        0 2023-05-08 10:31:11.752727 optinist-0.3.3/optinist/config/
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)      110 2023-04-03 06:29:38.000000 optinist-0.3.3/optinist/config/caiman_cnmf.yaml
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)      362 2023-04-03 06:29:38.000000 optinist-0.3.3/optinist/config/caiman_mc.yaml
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)      224 2023-04-03 06:29:38.000000 optinist-0.3.3/optinist/config/cca.yaml
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)       59 2023-04-03 06:29:38.000000 optinist-0.3.3/optinist/config/cell_grouping.yaml
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)       15 2023-04-03 06:29:38.000000 optinist-0.3.3/optinist/config/correlation.yaml
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)      284 2023-04-03 06:29:38.000000 optinist-0.3.3/optinist/config/cross_correlation.yaml
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)       14 2023-04-03 06:29:38.000000 optinist-0.3.3/optinist/config/dummy_image2image.yaml
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)      149 2023-04-03 06:29:38.000000 optinist-0.3.3/optinist/config/eta.yaml
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)      232 2023-04-03 06:29:38.000000 optinist-0.3.3/optinist/config/glm.yaml
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)      521 2023-04-03 06:29:38.000000 optinist-0.3.3/optinist/config/granger.yaml
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)      280 2023-04-03 06:29:38.000000 optinist-0.3.3/optinist/config/lccd_cell_detection.yaml
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)      564 2023-04-03 06:29:38.000000 optinist-0.3.3/optinist/config/lda.yaml
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)      626 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/config/nwb.yaml
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)      223 2023-04-03 06:29:38.000000 optinist-0.3.3/optinist/config/pca.yaml
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)       71 2023-04-12 06:11:01.000000 optinist-0.3.3/optinist/config/snakemake.yaml
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)     6823 2023-04-03 06:29:38.000000 optinist-0.3.3/optinist/config/suite2p.yaml
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)       78 2023-04-03 06:29:38.000000 optinist-0.3.3/optinist/config/suite2p_file_convert.yaml
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)      385 2023-04-03 06:29:38.000000 optinist-0.3.3/optinist/config/suite2p_registration.yaml
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)     1520 2023-04-03 06:29:38.000000 optinist-0.3.3/optinist/config/suite2p_roi.yaml
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)      314 2023-04-03 06:29:38.000000 optinist-0.3.3/optinist/config/suite2p_spike_deconv.yaml
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)     1352 2023-04-03 06:29:38.000000 optinist-0.3.3/optinist/config/svm.yaml
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)      394 2023-04-03 06:29:38.000000 optinist-0.3.3/optinist/config/tsne.yaml
+drwxr-xr-x   0 rei_hashimoto   (501) staff       (20)        0 2023-05-08 10:31:11.717384 optinist-0.3.3/optinist/frontend/
+drwxr-xr-x   0 rei_hashimoto   (501) staff       (20)        0 2023-05-08 10:31:11.753409 optinist-0.3.3/optinist/frontend/build/
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)     1297 2023-05-08 10:31:11.000000 optinist-0.3.3/optinist/frontend/build/asset-manifest.json
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)     3044 2023-05-08 10:31:11.000000 optinist-0.3.3/optinist/frontend/build/index.html
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)       67 2023-05-08 10:31:11.000000 optinist-0.3.3/optinist/frontend/build/robots.txt
+drwxr-xr-x   0 rei_hashimoto   (501) staff       (20)        0 2023-05-08 10:31:11.753860 optinist-0.3.3/optinist/frontend/build/static/
+drwxr-xr-x   0 rei_hashimoto   (501) staff       (20)        0 2023-05-08 10:31:11.754802 optinist-0.3.3/optinist/frontend/build/static/css/
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)     2422 2023-05-08 10:31:11.000000 optinist-0.3.3/optinist/frontend/build/static/css/2.dab0dc93.chunk.css
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)     4696 2023-05-08 10:31:11.000000 optinist-0.3.3/optinist/frontend/build/static/css/2.dab0dc93.chunk.css.map
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)     1339 2023-05-08 10:31:11.000000 optinist-0.3.3/optinist/frontend/build/static/css/main.08a92549.chunk.css
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)     2652 2023-05-08 10:31:11.000000 optinist-0.3.3/optinist/frontend/build/static/css/main.08a92549.chunk.css.map
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)    16958 2023-05-08 10:31:11.000000 optinist-0.3.3/optinist/frontend/build/static/favicon.ico
+drwxr-xr-x   0 rei_hashimoto   (501) staff       (20)        0 2023-05-08 10:31:11.769644 optinist-0.3.3/optinist/frontend/build/static/js/
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)  5146283 2023-05-08 10:31:11.000000 optinist-0.3.3/optinist/frontend/build/static/js/2.d6a78225.chunk.js
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)     3922 2023-05-08 10:31:11.000000 optinist-0.3.3/optinist/frontend/build/static/js/2.d6a78225.chunk.js.LICENSE.txt
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20) 18935319 2023-05-08 10:31:11.000000 optinist-0.3.3/optinist/frontend/build/static/js/2.d6a78225.chunk.js.map
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)     4384 2023-05-08 10:31:11.000000 optinist-0.3.3/optinist/frontend/build/static/js/3.e6a5ade8.chunk.js
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)     9612 2023-05-08 10:31:11.000000 optinist-0.3.3/optinist/frontend/build/static/js/3.e6a5ade8.chunk.js.map
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)   178350 2023-05-08 10:31:11.000000 optinist-0.3.3/optinist/frontend/build/static/js/main.08115825.chunk.js
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)   644102 2023-05-08 10:31:11.000000 optinist-0.3.3/optinist/frontend/build/static/js/main.08115825.chunk.js.map
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)     2358 2023-05-08 10:31:11.000000 optinist-0.3.3/optinist/frontend/build/static/js/runtime-main.6a23d4cb.js
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)    12470 2023-05-08 10:31:11.000000 optinist-0.3.3/optinist/frontend/build/static/js/runtime-main.6a23d4cb.js.map
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)      290 2023-05-08 10:31:11.000000 optinist-0.3.3/optinist/frontend/build/static/manifest.json
+drwxr-xr-x   0 rei_hashimoto   (501) staff       (20)        0 2023-05-08 10:31:11.769902 optinist-0.3.3/optinist/frontend/build/static/media/
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)    80977 2023-05-08 10:31:11.000000 optinist-0.3.3/optinist/frontend/build/static/media/optinist.e44efe32.png
+drwxr-xr-x   0 rei_hashimoto   (501) staff       (20)        0 2023-05-08 10:31:11.772243 optinist-0.3.3/optinist/routers/
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)        0 2023-04-03 06:29:38.000000 optinist-0.3.3/optinist/routers/__init__.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)     2769 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/routers/algolist.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)      193 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/routers/const.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)     3367 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/routers/experiment.py
+drwxr-xr-x   0 rei_hashimoto   (501) staff       (20)        0 2023-05-08 10:31:11.772669 optinist-0.3.3/optinist/routers/fileIO/
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)        0 2023-04-03 06:29:38.000000 optinist-0.3.3/optinist/routers/fileIO/__init__.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)     1095 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/routers/fileIO/file_reader.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)     2888 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/routers/files.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)     2301 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/routers/hdf5.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)     2403 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/routers/model.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)     5735 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/routers/outputs.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)      961 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/routers/params.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)     1089 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/routers/run.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)      407 2023-05-08 10:30:03.000000 optinist-0.3.3/optinist/version.py
+drwxr-xr-x   0 rei_hashimoto   (501) staff       (20)        0 2023-05-08 10:31:11.773034 optinist-0.3.3/optinist/wrappers/
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)      564 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/wrappers/__init__.py
+drwxr-xr-x   0 rei_hashimoto   (501) staff       (20)        0 2023-05-08 10:31:11.773673 optinist-0.3.3/optinist/wrappers/caiman_wrapper/
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)      488 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/wrappers/caiman_wrapper/__init__.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)     7402 2023-05-08 07:31:55.000000 optinist-0.3.3/optinist/wrappers/caiman_wrapper/cnmf.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)     2321 2023-05-08 07:31:49.000000 optinist-0.3.3/optinist/wrappers/caiman_wrapper/motion_correction.py
+drwxr-xr-x   0 rei_hashimoto   (501) staff       (20)        0 2023-05-08 10:31:11.774068 optinist-0.3.3/optinist/wrappers/dummy_wrapper/
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)     1457 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/wrappers/dummy_wrapper/__init__.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)     5130 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/wrappers/dummy_wrapper/dummy.py
+drwxr-xr-x   0 rei_hashimoto   (501) staff       (20)        0 2023-05-08 10:31:11.774507 optinist-0.3.3/optinist/wrappers/lccd_wrapper/
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)      273 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/wrappers/lccd_wrapper/__init__.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)     3100 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/wrappers/lccd_wrapper/lccd_detection.py
+drwxr-xr-x   0 rei_hashimoto   (501) staff       (20)        0 2023-05-08 10:31:11.775708 optinist-0.3.3/optinist/wrappers/lccd_wrapper/lccd_python/
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)        0 2023-04-26 03:02:01.000000 optinist-0.3.3/optinist/wrappers/lccd_wrapper/lccd_python/__init__.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)     3534 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/wrappers/lccd_wrapper/lccd_python/blob_detector.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)     1837 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/wrappers/lccd_wrapper/lccd_python/lccd.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)     1916 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/wrappers/lccd_wrapper/lccd_python/oval_filter.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)     6128 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/wrappers/lccd_wrapper/lccd_python/roi_integration.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)     7279 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/wrappers/lccd_wrapper/lccd_python/utils.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)      391 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/wrappers/optinist_exception.py
+drwxr-xr-x   0 rei_hashimoto   (501) staff       (20)        0 2023-05-08 10:31:11.776070 optinist-0.3.3/optinist/wrappers/optinist_wrapper/
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)      769 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/wrappers/optinist_wrapper/__init__.py
+drwxr-xr-x   0 rei_hashimoto   (501) staff       (20)        0 2023-05-08 10:31:11.777628 optinist-0.3.3/optinist/wrappers/optinist_wrapper/basic_neural_analysis/
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)      330 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/wrappers/optinist_wrapper/basic_neural_analysis/__init__.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)      735 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/wrappers/optinist_wrapper/basic_neural_analysis/cell_grouping.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)     3444 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/wrappers/optinist_wrapper/basic_neural_analysis/eta.py
+drwxr-xr-x   0 rei_hashimoto   (501) staff       (20)        0 2023-05-08 10:31:11.778545 optinist-0.3.3/optinist/wrappers/optinist_wrapper/dimension_reduction/
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)      533 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/wrappers/optinist_wrapper/dimension_reduction/__init__.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)     2066 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/wrappers/optinist_wrapper/dimension_reduction/cca.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)     2090 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/wrappers/optinist_wrapper/dimension_reduction/pca.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)     1095 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/wrappers/optinist_wrapper/dimension_reduction/tsne.py
+drwxr-xr-x   0 rei_hashimoto   (501) staff       (20)        0 2023-05-08 10:31:11.779675 optinist-0.3.3/optinist/wrappers/optinist_wrapper/neural_decoding/
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)      513 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/wrappers/optinist_wrapper/neural_decoding/__init__.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)     3040 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/wrappers/optinist_wrapper/neural_decoding/glm.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)     2148 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/wrappers/optinist_wrapper/neural_decoding/lda.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)     2590 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/wrappers/optinist_wrapper/neural_decoding/svm.py
+drwxr-xr-x   0 rei_hashimoto   (501) staff       (20)        0 2023-05-08 10:31:11.780697 optinist-0.3.3/optinist/wrappers/optinist_wrapper/neural_population_analysis/
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)      659 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/wrappers/optinist_wrapper/neural_population_analysis/__init__.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)      938 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/wrappers/optinist_wrapper/neural_population_analysis/correlation.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)     3209 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/wrappers/optinist_wrapper/neural_population_analysis/cross_correlation.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)     6227 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/wrappers/optinist_wrapper/neural_population_analysis/granger.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)      184 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/wrappers/optinist_wrapper/utils.py
+drwxr-xr-x   0 rei_hashimoto   (501) staff       (20)        0 2023-05-08 10:31:11.781639 optinist-0.3.3/optinist/wrappers/suite2p_wrapper/
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)     1031 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/wrappers/suite2p_wrapper/__init__.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)     1236 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/wrappers/suite2p_wrapper/file_convert.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)      968 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/wrappers/suite2p_wrapper/registration.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)     3605 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/wrappers/suite2p_wrapper/roi.py
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)     1660 2023-05-08 04:38:25.000000 optinist-0.3.3/optinist/wrappers/suite2p_wrapper/spike_deconv.py
+drwxr-xr-x   0 rei_hashimoto   (501) staff       (20)        0 2023-05-08 10:31:11.727003 optinist-0.3.3/optinist.egg-info/
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)     6471 2023-05-08 10:31:11.000000 optinist-0.3.3/optinist.egg-info/PKG-INFO
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)     7657 2023-05-08 10:31:11.000000 optinist-0.3.3/optinist.egg-info/SOURCES.txt
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)        1 2023-05-08 10:31:11.000000 optinist-0.3.3/optinist.egg-info/dependency_links.txt
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)       56 2023-05-08 10:31:11.000000 optinist-0.3.3/optinist.egg-info/entry_points.txt
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)        1 2023-05-08 10:30:58.000000 optinist-0.3.3/optinist.egg-info/not-zip-safe
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)      171 2023-05-08 10:31:11.000000 optinist-0.3.3/optinist.egg-info/requires.txt
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)       19 2023-05-08 10:31:11.000000 optinist-0.3.3/optinist.egg-info/top_level.txt
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)      171 2023-05-08 04:38:25.000000 optinist-0.3.3/requirements.txt
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)      115 2023-05-08 10:31:11.782297 optinist-0.3.3/setup.cfg
+-rw-r--r--   0 rei_hashimoto   (501) staff       (20)     2101 2023-05-08 09:22:45.000000 optinist-0.3.3/setup.py
```

### Comparing `optinist-0.3.2/LICENSE` & `optinist-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/PKG-INFO` & `optinist-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optinist
-Version: 0.3.2
+Version: 0.3.3
 Summary: Calcium Imaging Pipeline Tool
 Home-page: https://github.com/oist/optinist
 Author: OIST
 License: GPL3.0
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: optinist Version: 0.3.2 Summary: Calcium Imaging
+Metadata-Version: 2.1 Name: optinist Version: 0.3.3 Summary: Calcium Imaging
 Pipeline Tool Home-page: https://github.com/oist/optinist Author: OIST License:
 GPL3.0 Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: Education Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Operating System :: POSIX ::
 Linux Classifier: Operating System :: Microsoft :: Windows Classifier:
```

### Comparing `optinist-0.3.2/README.md` & `optinist-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/Snakefile` & `optinist-0.3.3/optinist/Snakefile`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/__main_unit__.py` & `optinist-0.3.3/optinist/__main_unit__.py`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/api/dataclass/bar.py` & `optinist-0.3.3/optinist/api/dataclass/bar.py`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/api/dataclass/csv.py` & `optinist-0.3.3/optinist/api/dataclass/csv.py`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/api/dataclass/dataclass.py` & `optinist-0.3.3/optinist/api/dataclass/dataclass.py`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/api/dataclass/heatmap.py` & `optinist-0.3.3/optinist/api/dataclass/heatmap.py`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/api/dataclass/image.py` & `optinist-0.3.3/optinist/api/dataclass/image.py`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/api/dataclass/scatter.py` & `optinist-0.3.3/optinist/api/dataclass/scatter.py`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/api/dataclass/timeseries.py` & `optinist-0.3.3/optinist/api/dataclass/timeseries.py`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/api/dir_path.py` & `optinist-0.3.3/optinist/api/dir_path.py`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/api/edit_ROI/edit_ROI.py` & `optinist-0.3.3/optinist/api/edit_ROI/edit_ROI.py`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/api/edit_ROI/utils.py` & `optinist-0.3.3/optinist/api/edit_ROI/utils.py`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/api/edit_ROI/wrappers/__init__.py` & `optinist-0.3.3/optinist/api/edit_ROI/wrappers/__init__.py`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/api/edit_ROI/wrappers/caiman_edit_roi/add_roi.py` & `optinist-0.3.3/optinist/api/edit_ROI/wrappers/caiman_edit_roi/add_roi.py`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/api/edit_ROI/wrappers/caiman_edit_roi/delete_roi.py` & `optinist-0.3.3/optinist/api/edit_ROI/wrappers/caiman_edit_roi/delete_roi.py`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/api/edit_ROI/wrappers/caiman_edit_roi/merge_roi.py` & `optinist-0.3.3/optinist/api/edit_ROI/wrappers/caiman_edit_roi/merge_roi.py`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/api/edit_ROI/wrappers/caiman_edit_roi/utils.py` & `optinist-0.3.3/optinist/api/edit_ROI/wrappers/caiman_edit_roi/utils.py`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/api/edit_ROI/wrappers/lccd_edit_roi/add_roi.py` & `optinist-0.3.3/optinist/api/edit_ROI/wrappers/lccd_edit_roi/add_roi.py`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/api/edit_ROI/wrappers/lccd_edit_roi/delete_roi.py` & `optinist-0.3.3/optinist/api/edit_ROI/wrappers/lccd_edit_roi/delete_roi.py`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/api/edit_ROI/wrappers/lccd_edit_roi/merge_roi.py` & `optinist-0.3.3/optinist/api/edit_ROI/wrappers/lccd_edit_roi/merge_roi.py`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/api/edit_ROI/wrappers/lccd_edit_roi/utils.py` & `optinist-0.3.3/optinist/api/edit_ROI/wrappers/lccd_edit_roi/utils.py`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/api/edit_ROI/wrappers/suite2p_edit_roi/add_roi.py` & `optinist-0.3.3/optinist/api/edit_ROI/wrappers/suite2p_edit_roi/add_roi.py`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/api/edit_ROI/wrappers/suite2p_edit_roi/delete_roi.py` & `optinist-0.3.3/optinist/api/edit_ROI/wrappers/suite2p_edit_roi/delete_roi.py`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/api/edit_ROI/wrappers/suite2p_edit_roi/merge_roi.py` & `optinist-0.3.3/optinist/api/edit_ROI/wrappers/suite2p_edit_roi/merge_roi.py`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/api/edit_ROI/wrappers/suite2p_edit_roi/utils.py` & `optinist-0.3.3/optinist/api/edit_ROI/wrappers/suite2p_edit_roi/utils.py`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/api/experiment/experiment.py` & `optinist-0.3.3/optinist/api/experiment/experiment.py`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/api/experiment/experiment_builder.py` & `optinist-0.3.3/optinist/api/experiment/experiment_builder.py`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/api/experiment/experiment_reader.py` & `optinist-0.3.3/optinist/api/experiment/experiment_reader.py`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/api/experiment/experiment_writer.py` & `optinist-0.3.3/optinist/api/experiment/experiment_writer.py`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/api/logger.py` & `optinist-0.3.3/optinist/api/logger.py`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/api/nwb/nwb_creater.py` & `optinist-0.3.3/optinist/api/nwb/nwb_creater.py`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/api/nwb/optinist_data.py` & `optinist-0.3.3/optinist/api/nwb/optinist_data.py`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/api/pickle/pickle_writer.py` & `optinist-0.3.3/optinist/api/pickle/pickle_writer.py`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/api/rules/data.py` & `optinist-0.3.3/optinist/api/rules/data.py`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/api/rules/file_writer.py` & `optinist-0.3.3/optinist/api/rules/file_writer.py`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/api/rules/func.py` & `optinist-0.3.3/optinist/api/rules/func.py`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/api/rules/runner.py` & `optinist-0.3.3/optinist/api/rules/runner.py`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/api/snakemake/smk.py` & `optinist-0.3.3/optinist/api/snakemake/smk.py`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/api/snakemake/smk_builder.py` & `optinist-0.3.3/optinist/api/snakemake/smk_builder.py`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/api/snakemake/smk_utils.py` & `optinist-0.3.3/optinist/api/snakemake/smk_utils.py`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/api/snakemake/snakemake_executor.py` & `optinist-0.3.3/optinist/api/snakemake/snakemake_executor.py`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/api/snakemake/snakemake_reader.py` & `optinist-0.3.3/optinist/api/snakemake/snakemake_reader.py`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/api/snakemake/snakemake_rule.py` & `optinist-0.3.3/optinist/api/snakemake/snakemake_rule.py`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/api/snakemake/snakemake_writer.py` & `optinist-0.3.3/optinist/api/snakemake/snakemake_writer.py`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/api/utils/filepath_creater.py` & `optinist-0.3.3/optinist/api/utils/filepath_creater.py`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/api/utils/json_writer.py` & `optinist-0.3.3/optinist/api/utils/json_writer.py`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/api/workflow/workflow.py` & `optinist-0.3.3/optinist/api/workflow/workflow.py`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/api/workflow/workflow_params.py` & `optinist-0.3.3/optinist/api/workflow/workflow_params.py`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/api/workflow/workflow_result.py` & `optinist-0.3.3/optinist/api/workflow/workflow_result.py`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/api/workflow/workflow_runner.py` & `optinist-0.3.3/optinist/api/workflow/workflow_runner.py`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/config/granger.yaml` & `optinist-0.3.3/optinist/config/granger.yaml`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/config/lda.yaml` & `optinist-0.3.3/optinist/config/lda.yaml`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/config/nwb.yaml` & `optinist-0.3.3/optinist/config/nwb.yaml`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/config/suite2p.yaml` & `optinist-0.3.3/optinist/config/suite2p.yaml`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/config/suite2p_roi.yaml` & `optinist-0.3.3/optinist/config/suite2p_roi.yaml`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/config/svm.yaml` & `optinist-0.3.3/optinist/config/svm.yaml`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/frontend/build/asset-manifest.json` & `optinist-0.3.3/optinist/frontend/build/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/frontend/build/index.html` & `optinist-0.3.3/optinist/frontend/build/index.html`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/frontend/build/static/css/2.dab0dc93.chunk.css` & `optinist-0.3.3/optinist/frontend/build/static/css/2.dab0dc93.chunk.css`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/frontend/build/static/css/2.dab0dc93.chunk.css.map` & `optinist-0.3.3/optinist/frontend/build/static/css/2.dab0dc93.chunk.css.map`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/frontend/build/static/css/main.08a92549.chunk.css` & `optinist-0.3.3/optinist/frontend/build/static/css/main.08a92549.chunk.css`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/frontend/build/static/css/main.08a92549.chunk.css.map` & `optinist-0.3.3/optinist/frontend/build/static/css/main.08a92549.chunk.css.map`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/frontend/build/static/favicon.ico` & `optinist-0.3.3/optinist/frontend/build/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/frontend/build/static/js/2.d6a78225.chunk.js` & `optinist-0.3.3/optinist/frontend/build/static/js/2.d6a78225.chunk.js`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/frontend/build/static/js/2.d6a78225.chunk.js.LICENSE.txt` & `optinist-0.3.3/optinist/frontend/build/static/js/2.d6a78225.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/frontend/build/static/js/2.d6a78225.chunk.js.map` & `optinist-0.3.3/optinist/frontend/build/static/js/2.d6a78225.chunk.js.map`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/frontend/build/static/js/3.e6a5ade8.chunk.js` & `optinist-0.3.3/optinist/frontend/build/static/js/3.e6a5ade8.chunk.js`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/frontend/build/static/js/3.e6a5ade8.chunk.js.map` & `optinist-0.3.3/optinist/frontend/build/static/js/3.e6a5ade8.chunk.js.map`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/frontend/build/static/js/main.08115825.chunk.js` & `optinist-0.3.3/optinist/frontend/build/static/js/main.08115825.chunk.js`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/frontend/build/static/js/main.08115825.chunk.js.map` & `optinist-0.3.3/optinist/frontend/build/static/js/main.08115825.chunk.js.map`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/frontend/build/static/js/runtime-main.6a23d4cb.js` & `optinist-0.3.3/optinist/frontend/build/static/js/runtime-main.6a23d4cb.js`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/frontend/build/static/js/runtime-main.6a23d4cb.js.map` & `optinist-0.3.3/optinist/frontend/build/static/js/runtime-main.6a23d4cb.js.map`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/frontend/build/static/media/optinist.e44efe32.png` & `optinist-0.3.3/optinist/frontend/build/static/media/optinist.e44efe32.png`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/routers/algolist.py` & `optinist-0.3.3/optinist/routers/algolist.py`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/routers/experiment.py` & `optinist-0.3.3/optinist/routers/experiment.py`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/routers/fileIO/file_reader.py` & `optinist-0.3.3/optinist/routers/fileIO/file_reader.py`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/routers/files.py` & `optinist-0.3.3/optinist/routers/files.py`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/routers/hdf5.py` & `optinist-0.3.3/optinist/routers/hdf5.py`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/routers/model.py` & `optinist-0.3.3/optinist/routers/model.py`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/routers/outputs.py` & `optinist-0.3.3/optinist/routers/outputs.py`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/routers/params.py` & `optinist-0.3.3/optinist/routers/params.py`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/routers/run.py` & `optinist-0.3.3/optinist/routers/run.py`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/wrappers/__init__.py` & `optinist-0.3.3/optinist/wrappers/__init__.py`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/wrappers/caiman_wrapper/cnmf.py` & `optinist-0.3.3/optinist/wrappers/caiman_wrapper/cnmf.py`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/wrappers/caiman_wrapper/motion_correction.py` & `optinist-0.3.3/optinist/wrappers/caiman_wrapper/motion_correction.py`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/wrappers/dummy_wrapper/__init__.py` & `optinist-0.3.3/optinist/wrappers/dummy_wrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/wrappers/dummy_wrapper/dummy.py` & `optinist-0.3.3/optinist/wrappers/dummy_wrapper/dummy.py`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/wrappers/lccd_wrapper/lccd_detection.py` & `optinist-0.3.3/optinist/wrappers/lccd_wrapper/lccd_detection.py`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/wrappers/lccd_wrapper/lccd_python/blob_detector.py` & `optinist-0.3.3/optinist/wrappers/lccd_wrapper/lccd_python/blob_detector.py`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/wrappers/lccd_wrapper/lccd_python/lccd.py` & `optinist-0.3.3/optinist/wrappers/lccd_wrapper/lccd_python/lccd.py`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/wrappers/lccd_wrapper/lccd_python/oval_filter.py` & `optinist-0.3.3/optinist/wrappers/lccd_wrapper/lccd_python/oval_filter.py`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/wrappers/lccd_wrapper/lccd_python/roi_integration.py` & `optinist-0.3.3/optinist/wrappers/lccd_wrapper/lccd_python/roi_integration.py`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/wrappers/lccd_wrapper/lccd_python/utils.py` & `optinist-0.3.3/optinist/wrappers/lccd_wrapper/lccd_python/utils.py`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/wrappers/optinist_wrapper/__init__.py` & `optinist-0.3.3/optinist/wrappers/optinist_wrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/wrappers/optinist_wrapper/basic_neural_analysis/cell_grouping.py` & `optinist-0.3.3/optinist/wrappers/optinist_wrapper/basic_neural_analysis/cell_grouping.py`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/wrappers/optinist_wrapper/basic_neural_analysis/eta.py` & `optinist-0.3.3/optinist/wrappers/optinist_wrapper/basic_neural_analysis/eta.py`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/wrappers/optinist_wrapper/dimension_reduction/__init__.py` & `optinist-0.3.3/optinist/wrappers/optinist_wrapper/dimension_reduction/__init__.py`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/wrappers/optinist_wrapper/dimension_reduction/cca.py` & `optinist-0.3.3/optinist/wrappers/optinist_wrapper/dimension_reduction/cca.py`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/wrappers/optinist_wrapper/dimension_reduction/pca.py` & `optinist-0.3.3/optinist/wrappers/optinist_wrapper/dimension_reduction/pca.py`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/wrappers/optinist_wrapper/dimension_reduction/tsne.py` & `optinist-0.3.3/optinist/wrappers/optinist_wrapper/dimension_reduction/tsne.py`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/wrappers/optinist_wrapper/neural_decoding/__init__.py` & `optinist-0.3.3/optinist/wrappers/optinist_wrapper/neural_decoding/__init__.py`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/wrappers/optinist_wrapper/neural_decoding/glm.py` & `optinist-0.3.3/optinist/wrappers/optinist_wrapper/neural_decoding/glm.py`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/wrappers/optinist_wrapper/neural_decoding/lda.py` & `optinist-0.3.3/optinist/wrappers/optinist_wrapper/neural_decoding/lda.py`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/wrappers/optinist_wrapper/neural_decoding/svm.py` & `optinist-0.3.3/optinist/wrappers/optinist_wrapper/neural_decoding/svm.py`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/wrappers/optinist_wrapper/neural_population_analysis/__init__.py` & `optinist-0.3.3/optinist/wrappers/optinist_wrapper/neural_population_analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/wrappers/optinist_wrapper/neural_population_analysis/correlation.py` & `optinist-0.3.3/optinist/wrappers/optinist_wrapper/neural_population_analysis/correlation.py`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/wrappers/optinist_wrapper/neural_population_analysis/cross_correlation.py` & `optinist-0.3.3/optinist/wrappers/optinist_wrapper/neural_population_analysis/cross_correlation.py`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/wrappers/optinist_wrapper/neural_population_analysis/granger.py` & `optinist-0.3.3/optinist/wrappers/optinist_wrapper/neural_population_analysis/granger.py`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/wrappers/suite2p_wrapper/__init__.py` & `optinist-0.3.3/optinist/wrappers/suite2p_wrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/wrappers/suite2p_wrapper/file_convert.py` & `optinist-0.3.3/optinist/wrappers/suite2p_wrapper/file_convert.py`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/wrappers/suite2p_wrapper/registration.py` & `optinist-0.3.3/optinist/wrappers/suite2p_wrapper/registration.py`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/wrappers/suite2p_wrapper/roi.py` & `optinist-0.3.3/optinist/wrappers/suite2p_wrapper/roi.py`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist/wrappers/suite2p_wrapper/spike_deconv.py` & `optinist-0.3.3/optinist/wrappers/suite2p_wrapper/spike_deconv.py`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/optinist.egg-info/PKG-INFO` & `optinist-0.3.3/optinist.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optinist
-Version: 0.3.2
+Version: 0.3.3
 Summary: Calcium Imaging Pipeline Tool
 Home-page: https://github.com/oist/optinist
 Author: OIST
 License: GPL3.0
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: optinist Version: 0.3.2 Summary: Calcium Imaging
+Metadata-Version: 2.1 Name: optinist Version: 0.3.3 Summary: Calcium Imaging
 Pipeline Tool Home-page: https://github.com/oist/optinist Author: OIST License:
 GPL3.0 Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: Education Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Operating System :: POSIX ::
 Linux Classifier: Operating System :: Microsoft :: Windows Classifier:
```

### Comparing `optinist-0.3.2/optinist.egg-info/SOURCES.txt` & `optinist-0.3.3/optinist.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `optinist-0.3.2/setup.py` & `optinist-0.3.3/setup.py`

 * *Files identical despite different names*

