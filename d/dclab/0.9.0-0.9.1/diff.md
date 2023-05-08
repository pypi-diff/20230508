# Comparing `tmp/dclab-0.9.0.tar.gz` & `tmp/dclab-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dclab-0.9.0.tar", last modified: Tue Jan 15 14:24:16 2019, max compression
+gzip compressed data, was "dist/dclab-0.9.1.tar", last modified: Tue Feb 26 13:50:56 2019, max compression
```

## Comparing `dclab-0.9.0.tar` & `dclab-0.9.1.tar`

### file list

```diff
@@ -1,137 +1,137 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-01-15 14:24:16.000000 dclab-0.9.0/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-01-15 14:24:16.000000 dclab-0.9.0/docs/
--rw-rw-r--   0 travis    (2000) travis    (2000)      350 2019-01-15 14:23:07.000000 dclab-0.9.0/docs/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)      110 2019-01-15 14:23:07.000000 dclab-0.9.0/docs/sec_changelog.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      508 2019-01-15 14:23:07.000000 dclab-0.9.0/docs/index.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     3815 2019-01-15 14:23:07.000000 dclab-0.9.0/docs/dclab.bib
--rw-rw-r--   0 travis    (2000) travis    (2000)      276 2019-01-15 14:23:07.000000 dclab-0.9.0/docs/sec_advanced_usage.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      209 2019-01-15 14:23:07.000000 dclab-0.9.0/docs/requirements.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       71 2019-01-15 14:23:07.000000 dclab-0.9.0/docs/sec_z_bib.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     5974 2019-01-15 14:23:07.000000 dclab-0.9.0/docs/sec_getting_started.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     4678 2019-01-15 14:23:07.000000 dclab-0.9.0/docs/sec_av_notation.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     8964 2019-01-15 14:23:07.000000 dclab-0.9.0/docs/sec_av_data.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     3131 2019-01-15 14:23:07.000000 dclab-0.9.0/docs/sec_av_rtdc_dataset.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      113 2019-01-15 14:23:07.000000 dclab-0.9.0/docs/sec_examples.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     4051 2019-01-15 14:23:07.000000 dclab-0.9.0/docs/sec_code_reference.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      332 2019-01-15 14:23:07.000000 dclab-0.9.0/docs/sec_cli.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-01-15 14:24:16.000000 dclab-0.9.0/docs/extensions/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2375 2019-01-15 14:23:07.000000 dclab-0.9.0/docs/extensions/github_changelog.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3123 2019-01-15 14:23:07.000000 dclab-0.9.0/docs/extensions/dclab_defs.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2789 2019-01-15 14:23:07.000000 dclab-0.9.0/docs/extensions/fancy_include.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6838 2019-01-15 14:23:07.000000 dclab-0.9.0/docs/conf.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      425 2019-01-15 14:23:07.000000 dclab-0.9.0/docs/sec_imprint.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-01-15 14:24:16.000000 dclab-0.9.0/dclab/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4989 2019-01-15 14:23:07.000000 dclab-0.9.0/dclab/cli.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      603 2019-01-15 14:23:07.000000 dclab-0.9.0/dclab/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3044 2019-01-15 14:23:07.000000 dclab-0.9.0/dclab/cached.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11984 2019-01-15 14:23:07.000000 dclab-0.9.0/dclab/definitions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5609 2019-01-15 14:23:07.000000 dclab-0.9.0/dclab/downsampling.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       82 2019-01-15 14:23:36.000000 dclab-0.9.0/dclab/_version_save.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6344 2019-01-15 14:23:07.000000 dclab-0.9.0/dclab/statistics.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4915 2019-01-15 14:23:07.000000 dclab-0.9.0/dclab/_version.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1529 2019-01-15 14:23:07.000000 dclab-0.9.0/dclab/parse_funcs.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11637 2019-01-15 14:23:07.000000 dclab-0.9.0/dclab/polygon_filter.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-01-15 14:24:16.000000 dclab-0.9.0/dclab/isoelastics/
--rw-rw-r--   0 travis    (2000) travis    (2000)    15525 2019-01-15 14:23:07.000000 dclab-0.9.0/dclab/isoelastics/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    59891 2019-01-15 14:23:07.000000 dclab-0.9.0/dclab/isoelastics/isoel-numerical-area_um-deform.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)    40138 2019-01-15 14:23:07.000000 dclab-0.9.0/dclab/isoelastics/isoel-analytical-area_um-deform.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     8096 2019-01-15 14:23:07.000000 dclab-0.9.0/dclab/kde_methods.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-01-15 14:24:16.000000 dclab-0.9.0/dclab/rtdc_dataset/
--rw-rw-r--   0 travis    (2000) travis    (2000)    12299 2019-01-15 14:23:07.000000 dclab-0.9.0/dclab/rtdc_dataset/write_hdf5.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8830 2019-01-15 14:23:07.000000 dclab-0.9.0/dclab/rtdc_dataset/load.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-01-15 14:24:16.000000 dclab-0.9.0/dclab/rtdc_dataset/fmt_tdms/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4403 2019-01-15 14:23:07.000000 dclab-0.9.0/dclab/rtdc_dataset/fmt_tdms/naming.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1467 2019-01-15 14:23:07.000000 dclab-0.9.0/dclab/rtdc_dataset/fmt_tdms/event_mask.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3734 2019-01-15 14:23:07.000000 dclab-0.9.0/dclab/rtdc_dataset/fmt_tdms/event_trace.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8819 2019-01-15 14:23:07.000000 dclab-0.9.0/dclab/rtdc_dataset/fmt_tdms/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5750 2019-01-15 14:23:07.000000 dclab-0.9.0/dclab/rtdc_dataset/fmt_tdms/event_contour.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5378 2019-01-15 14:23:07.000000 dclab-0.9.0/dclab/rtdc_dataset/fmt_tdms/event_image.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14618 2019-01-15 14:23:07.000000 dclab-0.9.0/dclab/rtdc_dataset/fmt_hierarchy.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      510 2019-01-15 14:23:07.000000 dclab-0.9.0/dclab/rtdc_dataset/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9860 2019-01-15 14:23:07.000000 dclab-0.9.0/dclab/rtdc_dataset/config.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5220 2019-01-15 14:23:07.000000 dclab-0.9.0/dclab/rtdc_dataset/fmt_hdf5.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15027 2019-01-15 14:23:07.000000 dclab-0.9.0/dclab/rtdc_dataset/core.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-01-15 14:24:16.000000 dclab-0.9.0/dclab/rtdc_dataset/ancillaries/
--rw-rw-r--   0 travis    (2000) travis    (2000)     7732 2019-01-15 14:23:07.000000 dclab-0.9.0/dclab/rtdc_dataset/ancillaries/ancillary_feature.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3795 2019-01-15 14:23:07.000000 dclab-0.9.0/dclab/rtdc_dataset/ancillaries/af_fl_max_ctc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2670 2019-01-15 14:23:07.000000 dclab-0.9.0/dclab/rtdc_dataset/ancillaries/af_image_contour.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      310 2019-01-15 14:23:07.000000 dclab-0.9.0/dclab/rtdc_dataset/ancillaries/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1601 2019-01-15 14:23:07.000000 dclab-0.9.0/dclab/rtdc_dataset/ancillaries/af_emodulus.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1822 2019-01-15 14:23:07.000000 dclab-0.9.0/dclab/rtdc_dataset/ancillaries/af_basic.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1942 2019-01-15 14:23:07.000000 dclab-0.9.0/dclab/rtdc_dataset/util.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12609 2019-01-15 14:23:07.000000 dclab-0.9.0/dclab/rtdc_dataset/export.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1560 2019-01-15 14:23:07.000000 dclab-0.9.0/dclab/rtdc_dataset/fmt_dict.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6292 2019-01-15 14:23:07.000000 dclab-0.9.0/dclab/rtdc_dataset/filter.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-01-15 14:24:16.000000 dclab-0.9.0/dclab/features/
--rw-rw-r--   0 travis    (2000) travis    (2000)     5725 2019-01-15 14:23:07.000000 dclab-0.9.0/dclab/features/volume.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2792 2019-01-15 14:23:07.000000 dclab-0.9.0/dclab/features/fl_crosstalk.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7740 2019-01-15 14:23:07.000000 dclab-0.9.0/dclab/features/emodulus.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2429 2019-01-15 14:23:07.000000 dclab-0.9.0/dclab/features/bright.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      274 2019-01-15 14:23:07.000000 dclab-0.9.0/dclab/features/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10498 2019-01-15 14:23:07.000000 dclab-0.9.0/dclab/features/inert_ratio.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2382 2019-01-15 14:23:07.000000 dclab-0.9.0/dclab/features/emodulus_viscosity.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1908 2019-01-15 14:23:07.000000 dclab-0.9.0/dclab/features/contour.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-01-15 14:24:16.000000 dclab-0.9.0/dclab/features/_skimage_measure/
--rw-rw-r--   0 travis    (2000) travis    (2000)      198 2019-01-15 14:23:07.000000 dclab-0.9.0/dclab/features/_skimage_measure/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7161 2019-01-15 14:23:07.000000 dclab-0.9.0/dclab/features/_skimage_measure/_find_contours_cy.pyx
--rw-rw-r--   0 travis    (2000) travis    (2000)     9340 2019-01-15 14:23:07.000000 dclab-0.9.0/dclab/features/_skimage_measure/_find_contours.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   799126 2019-01-15 14:23:07.000000 dclab-0.9.0/dclab/features/emodulus_lut.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      364 2019-01-15 14:23:07.000000 dclab-0.9.0/dclab/compat.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3163 2019-01-15 14:23:07.000000 dclab-0.9.0/README.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     2794 2019-01-15 14:23:07.000000 dclab-0.9.0/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-01-15 14:24:16.000000 dclab-0.9.0/examples/
--rw-rw-r--   0 travis    (2000) travis    (2000)    54797 2019-01-15 14:23:07.000000 dclab-0.9.0/examples/isoelastics.jpg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1340 2019-01-15 14:23:07.000000 dclab-0.9.0/examples/isoelastics.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      947 2019-01-15 14:23:07.000000 dclab-0.9.0/examples/generate_example_images.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9539 2019-01-15 14:23:07.000000 dclab-0.9.0/CHANGELOG
--rw-rw-r--   0 travis    (2000) travis    (2000)    18131 2019-01-15 14:23:07.000000 dclab-0.9.0/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)       98 2019-01-15 14:24:16.000000 dclab-0.9.0/setup.cfg
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-01-15 14:24:16.000000 dclab-0.9.0/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)      104 2019-01-15 14:23:07.000000 dclab-0.9.0/tests/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)     3511 2019-01-15 14:23:07.000000 dclab-0.9.0/tests/test_statistics.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7767 2019-01-15 14:23:07.000000 dclab-0.9.0/tests/test_export.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1546 2019-01-15 14:23:07.000000 dclab-0.9.0/tests/test_feat_contour.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      876 2019-01-15 14:23:07.000000 dclab-0.9.0/tests/test_feat_bright.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3173 2019-01-15 14:23:07.000000 dclab-0.9.0/tests/test_feat_inert_ratio.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10576 2019-01-15 14:23:07.000000 dclab-0.9.0/tests/test_polygon_filter.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5292 2019-01-15 14:23:07.000000 dclab-0.9.0/tests/test_rtdc_fmt_hierarchy.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1186 2019-01-15 14:23:07.000000 dclab-0.9.0/tests/test_config_value_mapping.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3621 2019-01-15 14:23:07.000000 dclab-0.9.0/tests/test_rtdc_downsampling.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1617 2019-01-15 14:23:07.000000 dclab-0.9.0/tests/test_rtdc_config.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13165 2019-01-15 14:23:07.000000 dclab-0.9.0/tests/test_rtdc_write_hdf5.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2128 2019-01-15 14:23:07.000000 dclab-0.9.0/tests/test_rtdc_limit_events.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13799 2019-01-15 14:23:07.000000 dclab-0.9.0/tests/test_ancillaries.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      937 2019-01-15 14:23:07.000000 dclab-0.9.0/tests/test_rtdc_hash.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1083 2019-01-15 14:23:07.000000 dclab-0.9.0/tests/test_rtdc_filter.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1375 2019-01-15 14:23:07.000000 dclab-0.9.0/tests/test_rtdc_check_dataset.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1480 2019-01-15 14:23:07.000000 dclab-0.9.0/tests/test_rtdc_fmt_dict.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2988 2019-01-15 14:23:07.000000 dclab-0.9.0/tests/helper_methods.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3306 2019-01-15 14:23:07.000000 dclab-0.9.0/tests/test_kde.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2179 2019-01-15 14:23:07.000000 dclab-0.9.0/tests/test_downsampling.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2307 2019-01-15 14:23:07.000000 dclab-0.9.0/tests/test_feat_fl_crosstalk.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6118 2019-01-15 14:23:07.000000 dclab-0.9.0/tests/test_isoelastics.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11768 2019-01-15 14:23:07.000000 dclab-0.9.0/tests/test_rtdc_fmt_tdms.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2170 2019-01-15 14:23:07.000000 dclab-0.9.0/tests/test_rtdc_fmt_hdf5.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1171 2019-01-15 14:23:07.000000 dclab-0.9.0/tests/test_feat_emodulus.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-01-15 14:24:16.000000 dclab-0.9.0/tests/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)    32284 2019-01-15 14:23:07.000000 dclab-0.9.0/tests/data/rtdc_data_traces_2flchan.zip
--rw-rw-r--   0 travis    (2000) travis    (2000)   109451 2019-01-15 14:23:07.000000 dclab-0.9.0/tests/data/rtdc_data_traces_video_large_fov.zip
--rw-rw-r--   0 travis    (2000) travis    (2000)    31147 2019-01-15 14:23:07.000000 dclab-0.9.0/tests/data/rtdc_data_hdf5_contour_image_trace.zip
--rw-rw-r--   0 travis    (2000) travis    (2000)   137752 2019-01-15 14:23:07.000000 dclab-0.9.0/tests/data/rtdc_data_traces_video_bright.zip
--rw-rw-r--   0 travis    (2000) travis    (2000)     7606 2019-01-15 14:23:07.000000 dclab-0.9.0/tests/data/rtdc_data_minimal.zip
--rw-rw-r--   0 travis    (2000) travis    (2000)     1385 2019-01-15 14:23:07.000000 dclab-0.9.0/tests/data/example_isoelastics.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)    31616 2019-01-15 14:23:07.000000 dclab-0.9.0/tests/data/rtdc_data_shapein_v2.0.1.zip
--rw-rw-r--   0 travis    (2000) travis    (2000)   119071 2019-01-15 14:23:07.000000 dclab-0.9.0/tests/data/rtdc_data_hdf5_mask_contour.zip
--rw-rw-r--   0 travis    (2000) travis    (2000)    40059 2019-01-15 14:23:07.000000 dclab-0.9.0/tests/data/rtdc_data_traces_video.zip
--rw-rw-r--   0 travis    (2000) travis    (2000)     2946 2019-01-15 14:23:07.000000 dclab-0.9.0/tests/test_feat_emodulus_viscosity.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1029 2019-01-15 14:23:07.000000 dclab-0.9.0/tests/test_cache.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5244 2019-01-15 14:23:07.000000 dclab-0.9.0/tests/test_feat_volume.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      295 2019-01-15 14:23:07.000000 dclab-0.9.0/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     4510 2019-01-15 14:24:16.000000 dclab-0.9.0/PKG-INFO
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-01-15 14:24:16.000000 dclab-0.9.0/dclab.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)        6 2019-01-15 14:24:16.000000 dclab-0.9.0/dclab.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      159 2019-01-15 14:24:16.000000 dclab-0.9.0/dclab.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     4510 2019-01-15 14:24:16.000000 dclab-0.9.0/dclab.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-01-15 14:24:16.000000 dclab-0.9.0/dclab.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      105 2019-01-15 14:24:16.000000 dclab-0.9.0/dclab.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     3570 2019-01-15 14:24:16.000000 dclab-0.9.0/dclab.egg-info/SOURCES.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-26 13:50:56.000000 dclab-0.9.1/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-26 13:50:56.000000 dclab-0.9.1/docs/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      350 2019-02-26 13:49:43.000000 dclab-0.9.1/docs/README.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)      110 2019-02-26 13:49:43.000000 dclab-0.9.1/docs/sec_changelog.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      508 2019-02-26 13:49:43.000000 dclab-0.9.1/docs/index.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3815 2019-02-26 13:49:43.000000 dclab-0.9.1/docs/dclab.bib
+-rw-rw-r--   0 travis    (2000) travis    (2000)      276 2019-02-26 13:49:43.000000 dclab-0.9.1/docs/sec_advanced_usage.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      209 2019-02-26 13:49:43.000000 dclab-0.9.1/docs/requirements.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       71 2019-02-26 13:49:43.000000 dclab-0.9.1/docs/sec_z_bib.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5974 2019-02-26 13:49:43.000000 dclab-0.9.1/docs/sec_getting_started.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4678 2019-02-26 13:49:43.000000 dclab-0.9.1/docs/sec_av_notation.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8964 2019-02-26 13:49:43.000000 dclab-0.9.1/docs/sec_av_data.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3131 2019-02-26 13:49:43.000000 dclab-0.9.1/docs/sec_av_rtdc_dataset.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      113 2019-02-26 13:49:43.000000 dclab-0.9.1/docs/sec_examples.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4051 2019-02-26 13:49:43.000000 dclab-0.9.1/docs/sec_code_reference.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      332 2019-02-26 13:49:43.000000 dclab-0.9.1/docs/sec_cli.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-26 13:50:56.000000 dclab-0.9.1/docs/extensions/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2375 2019-02-26 13:49:43.000000 dclab-0.9.1/docs/extensions/github_changelog.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3123 2019-02-26 13:49:43.000000 dclab-0.9.1/docs/extensions/dclab_defs.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2789 2019-02-26 13:49:43.000000 dclab-0.9.1/docs/extensions/fancy_include.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6838 2019-02-26 13:49:43.000000 dclab-0.9.1/docs/conf.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      425 2019-02-26 13:49:43.000000 dclab-0.9.1/docs/sec_imprint.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-26 13:50:56.000000 dclab-0.9.1/dclab/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4989 2019-02-26 13:49:43.000000 dclab-0.9.1/dclab/cli.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      603 2019-02-26 13:49:43.000000 dclab-0.9.1/dclab/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3044 2019-02-26 13:49:43.000000 dclab-0.9.1/dclab/cached.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11980 2019-02-26 13:49:43.000000 dclab-0.9.1/dclab/definitions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5609 2019-02-26 13:49:43.000000 dclab-0.9.1/dclab/downsampling.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       82 2019-02-26 13:50:13.000000 dclab-0.9.1/dclab/_version_save.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6344 2019-02-26 13:49:43.000000 dclab-0.9.1/dclab/statistics.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4915 2019-02-26 13:49:43.000000 dclab-0.9.1/dclab/_version.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1529 2019-02-26 13:49:43.000000 dclab-0.9.1/dclab/parse_funcs.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11637 2019-02-26 13:49:43.000000 dclab-0.9.1/dclab/polygon_filter.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-26 13:50:56.000000 dclab-0.9.1/dclab/isoelastics/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15525 2019-02-26 13:49:43.000000 dclab-0.9.1/dclab/isoelastics/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    59891 2019-02-26 13:49:43.000000 dclab-0.9.1/dclab/isoelastics/isoel-numerical-area_um-deform.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)    40138 2019-02-26 13:49:43.000000 dclab-0.9.1/dclab/isoelastics/isoel-analytical-area_um-deform.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8096 2019-02-26 13:49:43.000000 dclab-0.9.1/dclab/kde_methods.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-26 13:50:56.000000 dclab-0.9.1/dclab/rtdc_dataset/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12968 2019-02-26 13:49:43.000000 dclab-0.9.1/dclab/rtdc_dataset/write_hdf5.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9523 2019-02-26 13:49:43.000000 dclab-0.9.1/dclab/rtdc_dataset/load.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-26 13:50:56.000000 dclab-0.9.1/dclab/rtdc_dataset/fmt_tdms/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4900 2019-02-26 13:49:43.000000 dclab-0.9.1/dclab/rtdc_dataset/fmt_tdms/naming.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1467 2019-02-26 13:49:43.000000 dclab-0.9.1/dclab/rtdc_dataset/fmt_tdms/event_mask.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3734 2019-02-26 13:49:43.000000 dclab-0.9.1/dclab/rtdc_dataset/fmt_tdms/event_trace.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9364 2019-02-26 13:49:43.000000 dclab-0.9.1/dclab/rtdc_dataset/fmt_tdms/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5750 2019-02-26 13:49:43.000000 dclab-0.9.1/dclab/rtdc_dataset/fmt_tdms/event_contour.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5378 2019-02-26 13:49:43.000000 dclab-0.9.1/dclab/rtdc_dataset/fmt_tdms/event_image.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14618 2019-02-26 13:49:43.000000 dclab-0.9.1/dclab/rtdc_dataset/fmt_hierarchy.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      510 2019-02-26 13:49:43.000000 dclab-0.9.1/dclab/rtdc_dataset/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9860 2019-02-26 13:49:43.000000 dclab-0.9.1/dclab/rtdc_dataset/config.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5220 2019-02-26 13:49:43.000000 dclab-0.9.1/dclab/rtdc_dataset/fmt_hdf5.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14985 2019-02-26 13:49:43.000000 dclab-0.9.1/dclab/rtdc_dataset/core.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-26 13:50:56.000000 dclab-0.9.1/dclab/rtdc_dataset/ancillaries/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7732 2019-02-26 13:49:43.000000 dclab-0.9.1/dclab/rtdc_dataset/ancillaries/ancillary_feature.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3795 2019-02-26 13:49:43.000000 dclab-0.9.1/dclab/rtdc_dataset/ancillaries/af_fl_max_ctc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2670 2019-02-26 13:49:43.000000 dclab-0.9.1/dclab/rtdc_dataset/ancillaries/af_image_contour.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      310 2019-02-26 13:49:43.000000 dclab-0.9.1/dclab/rtdc_dataset/ancillaries/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1601 2019-02-26 13:49:43.000000 dclab-0.9.1/dclab/rtdc_dataset/ancillaries/af_emodulus.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1822 2019-02-26 13:49:43.000000 dclab-0.9.1/dclab/rtdc_dataset/ancillaries/af_basic.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1942 2019-02-26 13:49:43.000000 dclab-0.9.1/dclab/rtdc_dataset/util.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12609 2019-02-26 13:49:43.000000 dclab-0.9.1/dclab/rtdc_dataset/export.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1560 2019-02-26 13:49:43.000000 dclab-0.9.1/dclab/rtdc_dataset/fmt_dict.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6292 2019-02-26 13:49:43.000000 dclab-0.9.1/dclab/rtdc_dataset/filter.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-26 13:50:56.000000 dclab-0.9.1/dclab/features/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5725 2019-02-26 13:49:43.000000 dclab-0.9.1/dclab/features/volume.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2792 2019-02-26 13:49:43.000000 dclab-0.9.1/dclab/features/fl_crosstalk.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7740 2019-02-26 13:49:43.000000 dclab-0.9.1/dclab/features/emodulus.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2429 2019-02-26 13:49:43.000000 dclab-0.9.1/dclab/features/bright.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      274 2019-02-26 13:49:43.000000 dclab-0.9.1/dclab/features/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10498 2019-02-26 13:49:43.000000 dclab-0.9.1/dclab/features/inert_ratio.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2382 2019-02-26 13:49:43.000000 dclab-0.9.1/dclab/features/emodulus_viscosity.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1908 2019-02-26 13:49:43.000000 dclab-0.9.1/dclab/features/contour.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-26 13:50:56.000000 dclab-0.9.1/dclab/features/_skimage_measure/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      198 2019-02-26 13:49:43.000000 dclab-0.9.1/dclab/features/_skimage_measure/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7161 2019-02-26 13:49:43.000000 dclab-0.9.1/dclab/features/_skimage_measure/_find_contours_cy.pyx
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9340 2019-02-26 13:49:43.000000 dclab-0.9.1/dclab/features/_skimage_measure/_find_contours.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   799126 2019-02-26 13:49:43.000000 dclab-0.9.1/dclab/features/emodulus_lut.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      364 2019-02-26 13:49:43.000000 dclab-0.9.1/dclab/compat.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3165 2019-02-26 13:49:43.000000 dclab-0.9.1/README.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2801 2019-02-26 13:49:43.000000 dclab-0.9.1/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-26 13:50:56.000000 dclab-0.9.1/examples/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    54797 2019-02-26 13:49:43.000000 dclab-0.9.1/examples/isoelastics.jpg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1340 2019-02-26 13:49:43.000000 dclab-0.9.1/examples/isoelastics.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      947 2019-02-26 13:49:43.000000 dclab-0.9.1/examples/generate_example_images.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10167 2019-02-26 13:49:43.000000 dclab-0.9.1/CHANGELOG
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18131 2019-02-26 13:49:43.000000 dclab-0.9.1/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)       98 2019-02-26 13:50:56.000000 dclab-0.9.1/setup.cfg
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-26 13:50:56.000000 dclab-0.9.1/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      104 2019-02-26 13:49:43.000000 dclab-0.9.1/tests/README.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3511 2019-02-26 13:49:43.000000 dclab-0.9.1/tests/test_statistics.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7767 2019-02-26 13:49:43.000000 dclab-0.9.1/tests/test_export.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1546 2019-02-26 13:49:43.000000 dclab-0.9.1/tests/test_feat_contour.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      876 2019-02-26 13:49:43.000000 dclab-0.9.1/tests/test_feat_bright.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3173 2019-02-26 13:49:43.000000 dclab-0.9.1/tests/test_feat_inert_ratio.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10576 2019-02-26 13:49:43.000000 dclab-0.9.1/tests/test_polygon_filter.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5292 2019-02-26 13:49:43.000000 dclab-0.9.1/tests/test_rtdc_fmt_hierarchy.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1186 2019-02-26 13:49:43.000000 dclab-0.9.1/tests/test_config_value_mapping.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3621 2019-02-26 13:49:43.000000 dclab-0.9.1/tests/test_rtdc_downsampling.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1617 2019-02-26 13:49:43.000000 dclab-0.9.1/tests/test_rtdc_config.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13165 2019-02-26 13:49:43.000000 dclab-0.9.1/tests/test_rtdc_write_hdf5.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2128 2019-02-26 13:49:43.000000 dclab-0.9.1/tests/test_rtdc_limit_events.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13799 2019-02-26 13:49:43.000000 dclab-0.9.1/tests/test_ancillaries.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      937 2019-02-26 13:49:43.000000 dclab-0.9.1/tests/test_rtdc_hash.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1083 2019-02-26 13:49:43.000000 dclab-0.9.1/tests/test_rtdc_filter.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1612 2019-02-26 13:49:43.000000 dclab-0.9.1/tests/test_rtdc_check_dataset.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1480 2019-02-26 13:49:43.000000 dclab-0.9.1/tests/test_rtdc_fmt_dict.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2988 2019-02-26 13:49:43.000000 dclab-0.9.1/tests/helper_methods.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3306 2019-02-26 13:49:43.000000 dclab-0.9.1/tests/test_kde.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2179 2019-02-26 13:49:43.000000 dclab-0.9.1/tests/test_downsampling.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2307 2019-02-26 13:49:43.000000 dclab-0.9.1/tests/test_feat_fl_crosstalk.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6118 2019-02-26 13:49:43.000000 dclab-0.9.1/tests/test_isoelastics.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11768 2019-02-26 13:49:43.000000 dclab-0.9.1/tests/test_rtdc_fmt_tdms.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2170 2019-02-26 13:49:43.000000 dclab-0.9.1/tests/test_rtdc_fmt_hdf5.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1171 2019-02-26 13:49:43.000000 dclab-0.9.1/tests/test_feat_emodulus.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-26 13:50:56.000000 dclab-0.9.1/tests/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    32284 2019-02-26 13:49:43.000000 dclab-0.9.1/tests/data/rtdc_data_traces_2flchan.zip
+-rw-rw-r--   0 travis    (2000) travis    (2000)   109451 2019-02-26 13:49:43.000000 dclab-0.9.1/tests/data/rtdc_data_traces_video_large_fov.zip
+-rw-rw-r--   0 travis    (2000) travis    (2000)    31147 2019-02-26 13:49:43.000000 dclab-0.9.1/tests/data/rtdc_data_hdf5_contour_image_trace.zip
+-rw-rw-r--   0 travis    (2000) travis    (2000)   137752 2019-02-26 13:49:43.000000 dclab-0.9.1/tests/data/rtdc_data_traces_video_bright.zip
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7606 2019-02-26 13:49:43.000000 dclab-0.9.1/tests/data/rtdc_data_minimal.zip
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1385 2019-02-26 13:49:43.000000 dclab-0.9.1/tests/data/example_isoelastics.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)    31616 2019-02-26 13:49:43.000000 dclab-0.9.1/tests/data/rtdc_data_shapein_v2.0.1.zip
+-rw-rw-r--   0 travis    (2000) travis    (2000)   119071 2019-02-26 13:49:43.000000 dclab-0.9.1/tests/data/rtdc_data_hdf5_mask_contour.zip
+-rw-rw-r--   0 travis    (2000) travis    (2000)    40059 2019-02-26 13:49:43.000000 dclab-0.9.1/tests/data/rtdc_data_traces_video.zip
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2946 2019-02-26 13:49:43.000000 dclab-0.9.1/tests/test_feat_emodulus_viscosity.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1029 2019-02-26 13:49:43.000000 dclab-0.9.1/tests/test_cache.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5244 2019-02-26 13:49:43.000000 dclab-0.9.1/tests/test_feat_volume.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      295 2019-02-26 13:49:43.000000 dclab-0.9.1/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4512 2019-02-26 13:50:56.000000 dclab-0.9.1/PKG-INFO
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-02-26 13:50:56.000000 dclab-0.9.1/dclab.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        6 2019-02-26 13:50:56.000000 dclab-0.9.1/dclab.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      166 2019-02-26 13:50:56.000000 dclab-0.9.1/dclab.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4512 2019-02-26 13:50:56.000000 dclab-0.9.1/dclab.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-02-26 13:50:56.000000 dclab-0.9.1/dclab.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      105 2019-02-26 13:50:56.000000 dclab-0.9.1/dclab.egg-info/entry_points.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3570 2019-02-26 13:50:56.000000 dclab-0.9.1/dclab.egg-info/SOURCES.txt
```

### Comparing `dclab-0.9.0/docs/dclab.bib` & `dclab-0.9.1/docs/dclab.bib`

 * *Files identical despite different names*

### Comparing `dclab-0.9.0/docs/sec_getting_started.rst` & `dclab-0.9.1/docs/sec_getting_started.rst`

 * *Files identical despite different names*

### Comparing `dclab-0.9.0/docs/sec_av_notation.rst` & `dclab-0.9.1/docs/sec_av_notation.rst`

 * *Files identical despite different names*

### Comparing `dclab-0.9.0/docs/sec_av_data.rst` & `dclab-0.9.1/docs/sec_av_data.rst`

 * *Files identical despite different names*

### Comparing `dclab-0.9.0/docs/sec_av_rtdc_dataset.rst` & `dclab-0.9.1/docs/sec_av_rtdc_dataset.rst`

 * *Files identical despite different names*

### Comparing `dclab-0.9.0/docs/sec_code_reference.rst` & `dclab-0.9.1/docs/sec_code_reference.rst`

 * *Files identical despite different names*

### Comparing `dclab-0.9.0/docs/extensions/github_changelog.py` & `dclab-0.9.1/docs/extensions/github_changelog.py`

 * *Files identical despite different names*

### Comparing `dclab-0.9.0/docs/extensions/dclab_defs.py` & `dclab-0.9.1/docs/extensions/dclab_defs.py`

 * *Files identical despite different names*

### Comparing `dclab-0.9.0/docs/extensions/fancy_include.py` & `dclab-0.9.1/docs/extensions/fancy_include.py`

 * *Files identical despite different names*

### Comparing `dclab-0.9.0/docs/conf.py` & `dclab-0.9.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dclab-0.9.0/dclab/cli.py` & `dclab-0.9.1/dclab/cli.py`

 * *Files identical despite different names*

### Comparing `dclab-0.9.0/dclab/__init__.py` & `dclab-0.9.1/dclab/__init__.py`

 * *Files identical despite different names*

### Comparing `dclab-0.9.0/dclab/cached.py` & `dclab-0.9.1/dclab/cached.py`

 * *Files identical despite different names*

### Comparing `dclab-0.9.0/dclab/definitions.py` & `dclab-0.9.1/dclab/definitions.py`

 * *Files 0% similar despite different names*

```diff
@@ -192,15 +192,15 @@
     ["pos_y", "Position lateral in channel [µm]"],
     ["size_x", "Bounding box size x [µm]"],
     ["size_y", "Bounding box size y [µm]"],
     ["temp", "Sample Temperature [°C]"],
     ["temp_amb", "Ambient Temperature [°C]"],
     ["tilt", "Absolute tilt of raw contour"],
     ["time", "Event time [s]"],
-    ["volume", "Volume [µm³]"],    
+    ["volume", "Volume [µm³]"],
 ]
 # Add userdef features
 for _i in range(10):
     FEATURES_SCALAR.append(["userdef{}".format(_i),
                             "User defined {}".format(_i)
                             ])
```

### Comparing `dclab-0.9.0/dclab/downsampling.py` & `dclab-0.9.1/dclab/downsampling.py`

 * *Files identical despite different names*

### Comparing `dclab-0.9.0/dclab/statistics.py` & `dclab-0.9.1/dclab/statistics.py`

 * *Files identical despite different names*

### Comparing `dclab-0.9.0/dclab/_version.py` & `dclab-0.9.1/dclab/_version.py`

 * *Files identical despite different names*

### Comparing `dclab-0.9.0/dclab/parse_funcs.py` & `dclab-0.9.1/dclab/parse_funcs.py`

 * *Files identical despite different names*

### Comparing `dclab-0.9.0/dclab/polygon_filter.py` & `dclab-0.9.1/dclab/polygon_filter.py`

 * *Files identical despite different names*

### Comparing `dclab-0.9.0/dclab/isoelastics/__init__.py` & `dclab-0.9.1/dclab/isoelastics/__init__.py`

 * *Files identical despite different names*

### Comparing `dclab-0.9.0/dclab/isoelastics/isoel-numerical-area_um-deform.txt` & `dclab-0.9.1/dclab/isoelastics/isoel-numerical-area_um-deform.txt`

 * *Files identical despite different names*

### Comparing `dclab-0.9.0/dclab/isoelastics/isoel-analytical-area_um-deform.txt` & `dclab-0.9.1/dclab/isoelastics/isoel-analytical-area_um-deform.txt`

 * *Files identical despite different names*

### Comparing `dclab-0.9.0/dclab/kde_methods.py` & `dclab-0.9.1/dclab/kde_methods.py`

 * *Files identical despite different names*

### Comparing `dclab-0.9.0/dclab/rtdc_dataset/write_hdf5.py` & `dclab-0.9.1/dclab/rtdc_dataset/write_hdf5.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,19 +41,21 @@
         dset = h5group.create_dataset("image",
                                       data=data,
                                       dtype=np.uint8,
                                       maxshape=maxshape,
                                       chunks=True,
                                       fletcher32=True,
                                       compression=compression)
-        # Create and Set image attributes
-        # HDFView recognizes this as a series of images
-        dset.attrs.create('CLASS', b'IMAGE')
-        dset.attrs.create('IMAGE_VERSION', b'1.2')
-        dset.attrs.create('IMAGE_SUBCLASS', b'IMAGE_GRAYSCALE')
+        # Create and Set image attributes:
+        # HDFView recognizes this as a series of images.
+        # Use np.string_ as per
+        # http://docs.h5py.org/en/stable/strings.html#compatibility
+        dset.attrs.create('CLASS', np.string_('IMAGE'))
+        dset.attrs.create('IMAGE_VERSION', np.string_('1.2'))
+        dset.attrs.create('IMAGE_SUBCLASS', np.string_('IMAGE_GRAYSCALE'))
     else:
         dset = h5group["image"]
         oldsize = dset.shape[0]
         dset.resize(oldsize + data.shape[0], axis=0)
         dset[oldsize:] = data
 
 
@@ -244,22 +246,32 @@
     else:
         if mode == "reset":
             h5mode = "w"
         else:
             h5mode = "a"
         h5obj = h5py.File(path_or_h5file, mode=h5mode)
 
+    # update version
+    # - if it is not already in the hdf5 file (prevent override)
+    # - if it is explicitly given in meta (append to old version string)
+    if ("setup:software version" not in h5obj.attrs
+            or ("setup" in meta and "software version" in meta["setup"])):
+        thisver = "dclab {}".format(version)
+        if "setup" in meta and "software version" in meta["setup"]:
+            oldver = meta["setup"]["software version"]
+            thisver = "{} | {}".format(oldver, thisver)
+        if "setup" not in meta:
+            meta["setup"] = {}
+        meta["setup"]["software version"] = thisver
     # Write meta
     for sec in meta:
         for ck in meta[sec]:
             idk = "{}:{}".format(sec, ck)
             conffunc = dfn.config_funcs[sec][ck]
             h5obj.attrs[idk] = conffunc(meta[sec][ck])
-    # write version
-    h5obj.attrs["setup:software version"] = "dclab {}".format(version)
 
     # Write data
     # create events group
     if "events" not in h5obj:
         h5obj.create_group("events")
     events = h5obj["events"]
     # remove previous data
```

### Comparing `dclab-0.9.0/dclab/rtdc_dataset/load.py` & `dclab-0.9.1/dclab/rtdc_dataset/load.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,14 +132,23 @@
                 kp = "laser {} power".format(ii)
                 if (kl in ds.config["fluorescence"] and
                         kp in ds.config["fluorescence"]):
                     lsc2 += 1
             if lsc1 != lsc2:
                 msg = "Metadata: fluorescence laser count inconsistent"
                 viol.append(msg)
+        # check for samples per event
+        if "samples per event" in ds.config["fluorescence"]:
+            spe = ds.config["fluorescence"]["samples per event"]
+            for key in ds["trace"].keys():
+                spek = ds["trace"][key][0].size
+                if spek != spe:
+                    msg = "Metadata: wrong number of samples per event: " \
+                          + "{} (expected {}, got {}".format(key, spe, spek)
+                    viol.append(msg)
     else:
         info.append("Fluorescence: False")
     # search for missing keys (hard)
     for sec in tocheck:
         if sec not in ds.config:
             viol.append("Metadata: Missing section '{}'".format(sec))
         else:
@@ -178,20 +187,23 @@
             viol.append("Features: Unknown key '{}'".format(feat))
     info.append("Data file format: {}".format(ds.format))
     # hdf5-based checks
     if ds.format == "hdf5":
         # check meta data of images
         if "image" in ds._events:
             imdat = ds["image"]
-            for key, val in [['CLASS', 'IMAGE'],
-                             ['IMAGE_VERSION', '1.2'],
-                             ['IMAGE_SUBCLASS', 'IMAGE_GRAYSCALE']]:
+            for key, val in [['CLASS', b'IMAGE'],
+                             ['IMAGE_VERSION', b'1.2'],
+                             ['IMAGE_SUBCLASS', b'IMAGE_GRAYSCALE']]:
                 if key not in imdat.attrs:
                     aler.append("HDF5: '/image': missing attribute "
                                 + "'{}'".format(key))
+                elif not isinstance(imdat.attrs[key], bytes):
+                    aler.append("HDF5: '/image': attribute '{}' ".format(key)
+                                + "should be fixed-length ASCII string")
                 elif imdat.attrs[key] != val:
                     aler.append("HDF5: '/image': attribute '{}' ".format(key)
                                 + "should have value '{}'".format(val))
         # check length of logs
         with h5py.File(ds.path, mode="r") as h5:
             logs = h5["logs"]
             for logname in logs.keys():
```

### Comparing `dclab-0.9.0/dclab/rtdc_dataset/fmt_tdms/naming.py` & `dclab-0.9.1/dclab/rtdc_dataset/fmt_tdms/naming.py`

 * *Files 7% similar despite different names*

```diff
@@ -72,20 +72,28 @@
         "date": ("General", "Date [YYYY-MM-DD]"),
         "time": ("General", "Start Time [hh:mm:ss]"),
     },
     # All special keywords related to RT-FDC
     "fluorescence": {
         "bit depth": ("FLUOR", "Bitdepthraw"),
         "channel count": ("FLUOR", "FL-Channels"),
+        "channel 1 name": ("FLUOR", "Channel 1 Name"),
+        "channel 2 name": ("FLUOR", "Channel 2 Name"),
+        "channel 3 name": ("FLUOR", "Channel 3 Name"),
+        "channels installed": ("FLUOR", "Channels Installed"),
         "laser 1 power": ("FLUOR", "Laser1 488 nm Power [%]"),
         "laser 2 power": ("FLUOR", "Laser2 561 nm Power [%]"),
         "laser 3 power": ("FLUOR", "Laser3 640 nm Power [%]"),
+        "laser count": ("FLUOR", "Laser Count"),
+        "lasers installed": ("FLUOR", "Lasers Installed"),
         "sample rate": ("FLUOR", "Samplerate [sps]"),
+        "samples per event": ("FLUOR", "Samples Per Event"),
         "signal max": ("FLUOR", "ADCmax [V]"),
         "signal min": ("FLUOR", "ADCmin [V]"),
+        "trace median": ("FLUOR", "Trace Median"),
     },
     # All tdms-related parameters
     "fmt_tdms": {
         "video frame offset": ("General", "video frame offset"),
     },
     # All imaging-related keywords
     "imaging": {
@@ -116,12 +124,13 @@
     # All setup-related keywords, except imaging
     "setup": {
         "channel width": ("General", "Channel width [um]"),
         "chip region": ("General", "Region"),
         "flow rate": ("General", "Flow Rate [ul/s]"),
         "flow rate sample": ("General", "Sample Flow Rate [ul/s]"),
         "flow rate sheath": ("General", "Sheath Flow Rate [ul/s]"),
+        "identifier": ("General", "Identifier"),
         "medium": ("General", "Buffer Medium"),
         "module composition": ("Image", "Setup"),
         "software version": ("General", "Software Version"),
     },
 }
```

### Comparing `dclab-0.9.0/dclab/rtdc_dataset/fmt_tdms/event_mask.py` & `dclab-0.9.1/dclab/rtdc_dataset/fmt_tdms/event_mask.py`

 * *Files identical despite different names*

### Comparing `dclab-0.9.0/dclab/rtdc_dataset/fmt_tdms/event_trace.py` & `dclab-0.9.1/dclab/rtdc_dataset/fmt_tdms/event_trace.py`

 * *Files identical despite different names*

### Comparing `dclab-0.9.0/dclab/rtdc_dataset/fmt_tdms/__init__.py` & `dclab-0.9.1/dclab/rtdc_dataset/fmt_tdms/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # -*- coding: utf-8 -*-
 """RT-DC .tdms file format"""
 from __future__ import division, print_function
 
 import pathlib
 import time
 
-
 from nptdms import TdmsFile
 import numpy as np
 
 from ... import definitions as dfn
 
 from ..config import Configuration
 from ..core import RTDCBase
@@ -109,35 +108,39 @@
         self.config = dclab_config
         self._complete_config_tdms(tdms_config)
 
         self._init_filters()
 
     def _complete_config_tdms(self, residual_config={}):
         # experiment
-        gmtime = time.gmtime(self.path.stat().st_mtime)
+        tse = self.path.stat().st_mtime - self["time"][-1]
+        loct = time.localtime(tse)
         if "date" not in self.config["experiment"]:
             # Date of measurement ('YYYY-MM-DD')
-            datestr = time.strftime("%Y-%m-%d", gmtime)
+            datestr = time.strftime("%Y-%m-%d", loct)
             self.config["experiment"]["date"] = datestr
         if "event count" not in self.config["experiment"]:
             # Number of recorded events
             self.config["experiment"]["event count"] = len(self)
         if "sample" not in self.config["experiment"]:
             # Measured sample or user-defined reference
             sample = get_project_name_from_path(self.path)
             self.config["experiment"]["sample"] = sample
         if "time" not in self.config["experiment"]:
             # Start time of measurement ('HH:MM:SS')
-            timestr = time.strftime("%H:%M:%S", gmtime)
+            timestr = time.strftime("%H:%M:%S", loct)
             self.config["experiment"]["time"] = timestr
         # fluorescence
         if "fluorescence" in self.config:
-            self.config["fluorescence"]["laser 1 lambda"] = 488.
-            self.config["fluorescence"]["laser 2 lambda"] = 561.
-            self.config["fluorescence"]["laser 3 lambda"] = 640.
+            if "laser 1 power" in self.config["fluorescence"]:
+                self.config["fluorescence"]["laser 1 lambda"] = 488.
+            if "laser 2 power" in self.config["fluorescence"]:
+                self.config["fluorescence"]["laser 2 lambda"] = 561.
+            if "laser 3 power" in self.config["fluorescence"]:
+                self.config["fluorescence"]["laser 3 lambda"] = 640.
         # fmt_tdms
         if "video frame offset" not in self.config["fmt_tdms"]:
             self.config["fmt_tdms"]["video frame offset"] = 1
         # setup (compatibility to old tdms formats)
         if "flow rate" not in self.config["setup"]:
             self.config["setup"]["flow rate"] = np.nan
         if "channel width" not in self.config["setup"]:
@@ -151,14 +154,20 @@
         # imaging
         if "pixel size" not in self.config["imaging"]:
             self.config["imaging"]["pixel size"] = 0.34
         # medium convention for CellCarrierB
         if ("medium" in self.config["setup"] and
                 self.config["setup"]["medium"].lower() == "cellcarrier b"):
             self.config["setup"]["medium"] = "CellCarrierB"
+        # replace "+" with ","
+        if "module composition" in self.config["setup"]:
+            mc = self.config["setup"]["module composition"]
+            if mc.count("+"):
+                mc2 = ", ".join([m.strip() for m in mc.split("+")])
+                self.config["setup"]["module composition"] = mc2
 
     @property
     def hash(self):
         """Hash value based on file name and .ini file content"""
         if self._hash is None:
             # Only hash _camera.ini and _para.ini
             fsh = [self.path.with_name(self._mid + "_camera.ini"),
```

### Comparing `dclab-0.9.0/dclab/rtdc_dataset/fmt_tdms/event_contour.py` & `dclab-0.9.1/dclab/rtdc_dataset/fmt_tdms/event_contour.py`

 * *Files identical despite different names*

### Comparing `dclab-0.9.0/dclab/rtdc_dataset/fmt_tdms/event_image.py` & `dclab-0.9.1/dclab/rtdc_dataset/fmt_tdms/event_image.py`

 * *Files identical despite different names*

### Comparing `dclab-0.9.0/dclab/rtdc_dataset/fmt_hierarchy.py` & `dclab-0.9.1/dclab/rtdc_dataset/fmt_hierarchy.py`

 * *Files identical despite different names*

### Comparing `dclab-0.9.0/dclab/rtdc_dataset/config.py` & `dclab-0.9.1/dclab/rtdc_dataset/config.py`

 * *Files identical despite different names*

### Comparing `dclab-0.9.0/dclab/rtdc_dataset/fmt_hdf5.py` & `dclab-0.9.1/dclab/rtdc_dataset/fmt_hdf5.py`

 * *Files identical despite different names*

### Comparing `dclab-0.9.0/dclab/rtdc_dataset/core.py` & `dclab-0.9.1/dclab/rtdc_dataset/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,16 +90,15 @@
                         ct = True
                         break
         return ct
 
     def __getitem__(self, key):
         if key in self._events:
             data = self._events[key]
-            if not np.all(data == 0):
-                return data
+            return data
         # Try to find the feature in the ancillary features
         # (see ancillaries submodule for more information).
         # These features are cached in `self._ancillaries`.
         ancol = AncillaryFeature.available_features(self)
         if key in ancol:
             # The feature is available.
             anhash = ancol[key].hash(self)
```

### Comparing `dclab-0.9.0/dclab/rtdc_dataset/ancillaries/ancillary_feature.py` & `dclab-0.9.1/dclab/rtdc_dataset/ancillaries/ancillary_feature.py`

 * *Files identical despite different names*

### Comparing `dclab-0.9.0/dclab/rtdc_dataset/ancillaries/af_fl_max_ctc.py` & `dclab-0.9.1/dclab/rtdc_dataset/ancillaries/af_fl_max_ctc.py`

 * *Files identical despite different names*

### Comparing `dclab-0.9.0/dclab/rtdc_dataset/ancillaries/af_image_contour.py` & `dclab-0.9.1/dclab/rtdc_dataset/ancillaries/af_image_contour.py`

 * *Files identical despite different names*

### Comparing `dclab-0.9.0/dclab/rtdc_dataset/ancillaries/af_emodulus.py` & `dclab-0.9.1/dclab/rtdc_dataset/ancillaries/af_emodulus.py`

 * *Files identical despite different names*

### Comparing `dclab-0.9.0/dclab/rtdc_dataset/ancillaries/af_basic.py` & `dclab-0.9.1/dclab/rtdc_dataset/ancillaries/af_basic.py`

 * *Files identical despite different names*

### Comparing `dclab-0.9.0/dclab/rtdc_dataset/util.py` & `dclab-0.9.1/dclab/rtdc_dataset/util.py`

 * *Files identical despite different names*

### Comparing `dclab-0.9.0/dclab/rtdc_dataset/export.py` & `dclab-0.9.1/dclab/rtdc_dataset/export.py`

 * *Files identical despite different names*

### Comparing `dclab-0.9.0/dclab/rtdc_dataset/fmt_dict.py` & `dclab-0.9.1/dclab/rtdc_dataset/fmt_dict.py`

 * *Files identical despite different names*

### Comparing `dclab-0.9.0/dclab/rtdc_dataset/filter.py` & `dclab-0.9.1/dclab/rtdc_dataset/filter.py`

 * *Files identical despite different names*

### Comparing `dclab-0.9.0/dclab/features/volume.py` & `dclab-0.9.1/dclab/features/volume.py`

 * *Files identical despite different names*

### Comparing `dclab-0.9.0/dclab/features/fl_crosstalk.py` & `dclab-0.9.1/dclab/features/fl_crosstalk.py`

 * *Files identical despite different names*

### Comparing `dclab-0.9.0/dclab/features/emodulus.py` & `dclab-0.9.1/dclab/features/emodulus.py`

 * *Files identical despite different names*

### Comparing `dclab-0.9.0/dclab/features/bright.py` & `dclab-0.9.1/dclab/features/bright.py`

 * *Files identical despite different names*

### Comparing `dclab-0.9.0/dclab/features/inert_ratio.py` & `dclab-0.9.1/dclab/features/inert_ratio.py`

 * *Files identical despite different names*

### Comparing `dclab-0.9.0/dclab/features/emodulus_viscosity.py` & `dclab-0.9.1/dclab/features/emodulus_viscosity.py`

 * *Files identical despite different names*

### Comparing `dclab-0.9.0/dclab/features/contour.py` & `dclab-0.9.1/dclab/features/contour.py`

 * *Files identical despite different names*

### Comparing `dclab-0.9.0/dclab/features/_skimage_measure/_find_contours_cy.pyx` & `dclab-0.9.1/dclab/features/_skimage_measure/_find_contours_cy.pyx`

 * *Files identical despite different names*

### Comparing `dclab-0.9.0/dclab/features/_skimage_measure/_find_contours.py` & `dclab-0.9.1/dclab/features/_skimage_measure/_find_contours.py`

 * *Files identical despite different names*

### Comparing `dclab-0.9.0/dclab/features/emodulus_lut.txt` & `dclab-0.9.1/dclab/features/emodulus_lut.txt`

 * *Files identical despite different names*

### Comparing `dclab-0.9.0/README.rst` & `dclab-0.9.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -81,17 +81,17 @@
 The `appveyor Shape-Out build <https://ci.appveyor.com/project/paulmueller/ShapeOut>`__
 is automatically triggered after each commit to the Shape-Out repository. At each build,
 the master branch of dclab is checked out and the Shape-Out installer is built with it.
 Therefore, it is not necessary to bump the version of dclab or to upload the latest
 version of dclab to PyPI in order to get your new code into Shape-Out.
 
 
-.. |PyPI Version| image:: http://img.shields.io/pypi/v/dclab.svg
+.. |PyPI Version| image:: https://img.shields.io/pypi/v/dclab.svg
    :target: https://pypi.python.org/pypi/dclab
-.. |Build Status Unix| image:: http://img.shields.io/travis/ZELLMECHANIK-DRESDEN/dclab.svg?label=build_linux_osx
+.. |Build Status Unix| image:: https://img.shields.io/travis/ZELLMECHANIK-DRESDEN/dclab.svg?label=build_linux_osx
    :target: https://travis-ci.org/ZELLMECHANIK-DRESDEN/dclab
 .. |Build Status Win| image:: https://img.shields.io/appveyor/ci/paulmueller/dclab/master.svg?label=build_win
    :target: https://ci.appveyor.com/project/paulmueller/dclab
 .. |Coverage Status| image:: https://img.shields.io/codecov/c/github/ZELLMECHANIK-DRESDEN/dclab/master.svg
    :target: https://codecov.io/gh/ZELLMECHANIK-DRESDEN/dclab
 .. |Docs Status| image:: https://readthedocs.org/projects/dclab/badge/?version=latest
    :target: https://readthedocs.org/projects/dclab/builds/
```

### Comparing `dclab-0.9.0/setup.py` & `dclab-0.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     package_dir={name: name},
     include_package_data=True,
     license="GPL v2",
     description=description,
     long_description=open('README.rst').read() if exists('README.rst') else '',
     install_requires=["fcswrite>=0.4.1",  # required by: fcs export
                       "h5py>=2.8.0",      # required by: rtdc format
-                      "imageio>=2.3.0",   # required by: tdms format, avi export
+                      "imageio>=2.3.0,<2.5.0",   # required by: tdms format, avi export
                       "nptdms",           # required by: tdms format
                       "numpy>=1.10.0",
                       "pathlib;python_version<='3.4'",
                       "scipy>=0.13.0",
                       "statsmodels>=0.5.0",
                       # Additional dependencies of statsmodels which are not
                       # installed automatically due to a developer policy:
```

### Comparing `dclab-0.9.0/examples/isoelastics.jpg` & `dclab-0.9.1/examples/isoelastics.jpg`

 * *Files identical despite different names*

### Comparing `dclab-0.9.0/examples/isoelastics.py` & `dclab-0.9.1/examples/isoelastics.py`

 * *Files identical despite different names*

### Comparing `dclab-0.9.0/examples/generate_example_images.py` & `dclab-0.9.1/examples/generate_example_images.py`

 * *Files identical despite different names*

### Comparing `dclab-0.9.0/CHANGELOG` & `dclab-0.9.1/CHANGELOG`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,20 @@
-0.8.1
+0.9.1
+ - fix: all-zero features were treated as non-existent due to relic
+   from pre-0.3.3 era
+ - fix: correct extraction of start time from tdms format
+   (1h offset from local time and measurement duration offset)
+ - fix: correct extraction of module composition from tdms format
+   (replace "+" with ",")
+ - enh: add configuration key mapping for tdms format to simplify
+   conversion to hdf5 format (see ``fmt_tdms.naming``)
+ - enh: do not add laser info for unused lasers for tdms format
+ - enh: dclab-verify-dataset checks for image attribute dtype
+ - enh: include original software version when exporting to rtdc format
+0.9.0
  - feat: add new feature: gravitational force, temperature,
    and ambient temperature
  - ref: remove unused `has_key` function in
    `rtdc_dataset.config.CaseInsensitiveDict`
  - setup: require numpy>=1.10.0 because of `equal_nan` argument in `allclose`
 0.8.0
  - fix: usage of "xor" (^) instead of "or" (|) in statistics
```

### Comparing `dclab-0.9.0/LICENSE` & `dclab-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dclab-0.9.0/tests/test_statistics.py` & `dclab-0.9.1/tests/test_statistics.py`

 * *Files identical despite different names*

### Comparing `dclab-0.9.0/tests/test_export.py` & `dclab-0.9.1/tests/test_export.py`

 * *Files identical despite different names*

### Comparing `dclab-0.9.0/tests/test_feat_contour.py` & `dclab-0.9.1/tests/test_feat_contour.py`

 * *Files identical despite different names*

### Comparing `dclab-0.9.0/tests/test_feat_bright.py` & `dclab-0.9.1/tests/test_feat_bright.py`

 * *Files identical despite different names*

### Comparing `dclab-0.9.0/tests/test_feat_inert_ratio.py` & `dclab-0.9.1/tests/test_feat_inert_ratio.py`

 * *Files identical despite different names*

### Comparing `dclab-0.9.0/tests/test_polygon_filter.py` & `dclab-0.9.1/tests/test_polygon_filter.py`

 * *Files identical despite different names*

### Comparing `dclab-0.9.0/tests/test_rtdc_fmt_hierarchy.py` & `dclab-0.9.1/tests/test_rtdc_fmt_hierarchy.py`

 * *Files identical despite different names*

### Comparing `dclab-0.9.0/tests/test_config_value_mapping.py` & `dclab-0.9.1/tests/test_config_value_mapping.py`

 * *Files identical despite different names*

### Comparing `dclab-0.9.0/tests/test_rtdc_downsampling.py` & `dclab-0.9.1/tests/test_rtdc_downsampling.py`

 * *Files identical despite different names*

### Comparing `dclab-0.9.0/tests/test_rtdc_config.py` & `dclab-0.9.1/tests/test_rtdc_config.py`

 * *Files identical despite different names*

### Comparing `dclab-0.9.0/tests/test_rtdc_write_hdf5.py` & `dclab-0.9.1/tests/test_rtdc_write_hdf5.py`

 * *Files identical despite different names*

### Comparing `dclab-0.9.0/tests/test_rtdc_limit_events.py` & `dclab-0.9.1/tests/test_rtdc_limit_events.py`

 * *Files identical despite different names*

### Comparing `dclab-0.9.0/tests/test_ancillaries.py` & `dclab-0.9.1/tests/test_ancillaries.py`

 * *Files identical despite different names*

### Comparing `dclab-0.9.0/tests/test_rtdc_hash.py` & `dclab-0.9.1/tests/test_rtdc_hash.py`

 * *Files identical despite different names*

### Comparing `dclab-0.9.0/tests/test_rtdc_filter.py` & `dclab-0.9.1/tests/test_rtdc_filter.py`

 * *Files identical despite different names*

### Comparing `dclab-0.9.0/tests/test_rtdc_check_dataset.py` & `dclab-0.9.1/tests/test_rtdc_check_dataset.py`

 * *Files 23% similar despite different names*

```diff
@@ -18,19 +18,22 @@
     # Metadata: Missing key [fluorescence] 'channels installed'
     # Metadata: Missing key [fluorescence] 'laser count'
     # Metadata: Missing key [fluorescence] 'lasers installed'
     # Metadata: Missing key [fluorescence] 'samples per event'
     # Metadata: Unknown key [imaging] 'exposure time'
     # Metadata: Unknown key [imaging] 'flash current'
     # Metadata: Unknown key [setup] 'temperature'
-    # Metadata: fluorescence channel count inconsitent
+    # Metadata: fluorescence channel count inconsistent
     assert len(viol) == 9
     # Metadata: Missing key [setup] identifier'
     # Metadata: Missing section 'online_contour'
-    assert len(aler) == 2
+    # "HDF5: '/image': attribute 'CLASS' should be fixed-length ASCII string",
+    # "HDF5: '/image': attribute 'IMAGE_SUBCLASS' should be fixed-length ...",
+    # "HDF5: '/image': attribute 'IMAGE_VERSION' should be fixed-length ...",
+    assert len(aler) == 5
     assert "Data file format: hdf5" in info
     assert "Fluorescence: True" in info
     cleanup()
 
 
 if __name__ == "__main__":
     # Run all tests
```

### Comparing `dclab-0.9.0/tests/test_rtdc_fmt_dict.py` & `dclab-0.9.1/tests/test_rtdc_fmt_dict.py`

 * *Files identical despite different names*

### Comparing `dclab-0.9.0/tests/helper_methods.py` & `dclab-0.9.1/tests/helper_methods.py`

 * *Files identical despite different names*

### Comparing `dclab-0.9.0/tests/test_kde.py` & `dclab-0.9.1/tests/test_kde.py`

 * *Files identical despite different names*

### Comparing `dclab-0.9.0/tests/test_downsampling.py` & `dclab-0.9.1/tests/test_downsampling.py`

 * *Files identical despite different names*

### Comparing `dclab-0.9.0/tests/test_feat_fl_crosstalk.py` & `dclab-0.9.1/tests/test_feat_fl_crosstalk.py`

 * *Files identical despite different names*

### Comparing `dclab-0.9.0/tests/test_isoelastics.py` & `dclab-0.9.1/tests/test_isoelastics.py`

 * *Files identical despite different names*

### Comparing `dclab-0.9.0/tests/test_rtdc_fmt_tdms.py` & `dclab-0.9.1/tests/test_rtdc_fmt_tdms.py`

 * *Files identical despite different names*

### Comparing `dclab-0.9.0/tests/test_rtdc_fmt_hdf5.py` & `dclab-0.9.1/tests/test_rtdc_fmt_hdf5.py`

 * *Files identical despite different names*

### Comparing `dclab-0.9.0/tests/test_feat_emodulus.py` & `dclab-0.9.1/tests/test_feat_emodulus.py`

 * *Files identical despite different names*

### Comparing `dclab-0.9.0/tests/data/rtdc_data_traces_2flchan.zip` & `dclab-0.9.1/tests/data/rtdc_data_traces_2flchan.zip`

 * *Files identical despite different names*

### Comparing `dclab-0.9.0/tests/data/rtdc_data_traces_video_large_fov.zip` & `dclab-0.9.1/tests/data/rtdc_data_traces_video_large_fov.zip`

 * *Files identical despite different names*

### Comparing `dclab-0.9.0/tests/data/rtdc_data_hdf5_contour_image_trace.zip` & `dclab-0.9.1/tests/data/rtdc_data_hdf5_contour_image_trace.zip`

 * *Files identical despite different names*

### Comparing `dclab-0.9.0/tests/data/rtdc_data_traces_video_bright.zip` & `dclab-0.9.1/tests/data/rtdc_data_traces_video_bright.zip`

 * *Files identical despite different names*

### Comparing `dclab-0.9.0/tests/data/rtdc_data_minimal.zip` & `dclab-0.9.1/tests/data/rtdc_data_minimal.zip`

 * *Files identical despite different names*

### Comparing `dclab-0.9.0/tests/data/example_isoelastics.txt` & `dclab-0.9.1/tests/data/example_isoelastics.txt`

 * *Files identical despite different names*

### Comparing `dclab-0.9.0/tests/data/rtdc_data_shapein_v2.0.1.zip` & `dclab-0.9.1/tests/data/rtdc_data_shapein_v2.0.1.zip`

 * *Files identical despite different names*

### Comparing `dclab-0.9.0/tests/data/rtdc_data_hdf5_mask_contour.zip` & `dclab-0.9.1/tests/data/rtdc_data_hdf5_mask_contour.zip`

 * *Files identical despite different names*

### Comparing `dclab-0.9.0/tests/data/rtdc_data_traces_video.zip` & `dclab-0.9.1/tests/data/rtdc_data_traces_video.zip`

 * *Files identical despite different names*

### Comparing `dclab-0.9.0/tests/test_feat_emodulus_viscosity.py` & `dclab-0.9.1/tests/test_feat_emodulus_viscosity.py`

 * *Files identical despite different names*

### Comparing `dclab-0.9.0/tests/test_cache.py` & `dclab-0.9.1/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `dclab-0.9.0/tests/test_feat_volume.py` & `dclab-0.9.1/tests/test_feat_volume.py`

 * *Files identical despite different names*

### Comparing `dclab-0.9.0/PKG-INFO` & `dclab-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: dclab
-Version: 0.9.0
+Version: 0.9.1
 Summary: Library for real-time deformability cytometry (RT-DC)
 Home-page: https://github.com/ZELLMECHANIK-DRESDEN/dclab
 Author: Paul Müller
 Author-email: dev@craban.de
 License: GPL v2
 Description: dclab
         =====
@@ -89,17 +89,17 @@
         The `appveyor Shape-Out build <https://ci.appveyor.com/project/paulmueller/ShapeOut>`__
         is automatically triggered after each commit to the Shape-Out repository. At each build,
         the master branch of dclab is checked out and the Shape-Out installer is built with it.
         Therefore, it is not necessary to bump the version of dclab or to upload the latest
         version of dclab to PyPI in order to get your new code into Shape-Out.
         
         
-        .. |PyPI Version| image:: http://img.shields.io/pypi/v/dclab.svg
+        .. |PyPI Version| image:: https://img.shields.io/pypi/v/dclab.svg
            :target: https://pypi.python.org/pypi/dclab
-        .. |Build Status Unix| image:: http://img.shields.io/travis/ZELLMECHANIK-DRESDEN/dclab.svg?label=build_linux_osx
+        .. |Build Status Unix| image:: https://img.shields.io/travis/ZELLMECHANIK-DRESDEN/dclab.svg?label=build_linux_osx
            :target: https://travis-ci.org/ZELLMECHANIK-DRESDEN/dclab
         .. |Build Status Win| image:: https://img.shields.io/appveyor/ci/paulmueller/dclab/master.svg?label=build_win
            :target: https://ci.appveyor.com/project/paulmueller/dclab
         .. |Coverage Status| image:: https://img.shields.io/codecov/c/github/ZELLMECHANIK-DRESDEN/dclab/master.svg
            :target: https://codecov.io/gh/ZELLMECHANIK-DRESDEN/dclab
         .. |Docs Status| image:: https://readthedocs.org/projects/dclab/badge/?version=latest
            :target: https://readthedocs.org/projects/dclab/builds/
```

### Comparing `dclab-0.9.0/dclab.egg-info/PKG-INFO` & `dclab-0.9.1/dclab.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: dclab
-Version: 0.9.0
+Version: 0.9.1
 Summary: Library for real-time deformability cytometry (RT-DC)
 Home-page: https://github.com/ZELLMECHANIK-DRESDEN/dclab
 Author: Paul Müller
 Author-email: dev@craban.de
 License: GPL v2
 Description: dclab
         =====
@@ -89,17 +89,17 @@
         The `appveyor Shape-Out build <https://ci.appveyor.com/project/paulmueller/ShapeOut>`__
         is automatically triggered after each commit to the Shape-Out repository. At each build,
         the master branch of dclab is checked out and the Shape-Out installer is built with it.
         Therefore, it is not necessary to bump the version of dclab or to upload the latest
         version of dclab to PyPI in order to get your new code into Shape-Out.
         
         
-        .. |PyPI Version| image:: http://img.shields.io/pypi/v/dclab.svg
+        .. |PyPI Version| image:: https://img.shields.io/pypi/v/dclab.svg
            :target: https://pypi.python.org/pypi/dclab
-        .. |Build Status Unix| image:: http://img.shields.io/travis/ZELLMECHANIK-DRESDEN/dclab.svg?label=build_linux_osx
+        .. |Build Status Unix| image:: https://img.shields.io/travis/ZELLMECHANIK-DRESDEN/dclab.svg?label=build_linux_osx
            :target: https://travis-ci.org/ZELLMECHANIK-DRESDEN/dclab
         .. |Build Status Win| image:: https://img.shields.io/appveyor/ci/paulmueller/dclab/master.svg?label=build_win
            :target: https://ci.appveyor.com/project/paulmueller/dclab
         .. |Coverage Status| image:: https://img.shields.io/codecov/c/github/ZELLMECHANIK-DRESDEN/dclab/master.svg
            :target: https://codecov.io/gh/ZELLMECHANIK-DRESDEN/dclab
         .. |Docs Status| image:: https://readthedocs.org/projects/dclab/badge/?version=latest
            :target: https://readthedocs.org/projects/dclab/builds/
```

### Comparing `dclab-0.9.0/dclab.egg-info/SOURCES.txt` & `dclab-0.9.1/dclab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

