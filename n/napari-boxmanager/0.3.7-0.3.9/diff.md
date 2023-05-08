# Comparing `tmp/napari_boxmanager-0.3.7.tar.gz` & `tmp/napari_boxmanager-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari_boxmanager-0.3.7.tar", last modified: Fri Feb 17 13:45:46 2023, max compression
+gzip compressed data, was "napari_boxmanager-0.3.9.tar", last modified: Fri Feb 17 15:40:24 2023, max compression
```

## Comparing `napari_boxmanager-0.3.7.tar` & `napari_boxmanager-0.3.9.tar`

### file list

```diff
@@ -1,154 +1,154 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 13:45:46.340174 napari_boxmanager-0.3.7/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 13:45:46.312173 napari_boxmanager-0.3.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 13:45:46.320174 napari_boxmanager-0.3.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 13:45:46.320174 napari_boxmanager-0.3.7/.napari/
--rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/.napari/DESCRIPTION.md
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    16726 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-02-17 13:45:46.340174 napari_boxmanager-0.3.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 13:45:46.320174 napari_boxmanager-0.3.7/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)      232 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/bin/napari_boxmanager
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 13:45:46.320174 napari_boxmanager-0.3.7/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 13:45:46.320174 napari_boxmanager-0.3.7/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/docs/_static/version-alert.js
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 13:45:46.320174 napari_boxmanager-0.3.7/docs/manual/
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/docs/manual/general.rst
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/docs/manual/manual.rst
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/docs/manual/read.rst
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/docs/manual/write.rst
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 13:45:46.320174 napari_boxmanager-0.3.7/reader_backup/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 13:45:46.320174 napari_boxmanager-0.3.7/reader_backup/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/reader_backup/_tests/test_box.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/reader_backup/_tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/reader_backup/_tests/test_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/reader_backup/_tests/test_tlpkl.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/reader_backup/cbox.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/reader_backup/star.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/reader_backup/tepkl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/reader_backup/tlpkl.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/reader_backup/tmpkl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/reader_backup/to_napari_backup.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-02-17 13:45:46.344174 napari_boxmanager-0.3.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 13:45:46.316174 napari_boxmanager-0.3.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 13:45:46.324174 napari_boxmanager-0.3.7/src/box_manager/
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/src/box_manager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 13:45:46.324174 napari_boxmanager-0.3.7/src/box_manager/_qt/
--rw-r--r--   0 runner    (1001) docker     (123)     9326 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/src/box_manager/_qt/FilterImage.py
--rw-r--r--   0 runner    (1001) docker     (123)    13471 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/src/box_manager/_qt/OrganizeBox.py
--rw-r--r--   0 runner    (1001) docker     (123)    17967 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/src/box_manager/_qt/OrganizeLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)    82644 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/src/box_manager/_qt/SelectMetric.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/src/box_manager/_qt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 13:45:46.324174 napari_boxmanager-0.3.7/src/box_manager/_qt/_icons/
--rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/src/box_manager/_qt/_icons/checkmark_black.png
--rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/src/box_manager/_qt/_icons/checkmark_white.png
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/src/box_manager/_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/src/box_manager/_sample_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 13:45:46.324174 napari_boxmanager-0.3.7/src/box_manager/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/src/box_manager/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/src/box_manager/_tests/_dummy_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/src/box_manager/_tests/test_box.py
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/src/box_manager/_tests/test_cbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/src/box_manager/_tests/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/src/box_manager/_tests/test_sample_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/src/box_manager/_tests/test_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/src/box_manager/_tests/test_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 13:45:46.324174 napari_boxmanager-0.3.7/src/box_manager/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/src/box_manager/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/src/box_manager/_utils/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/src/box_manager/_utils/general.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-02-17 13:45:46.000000 napari_boxmanager-0.3.7/src/box_manager/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/src/box_manager/_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/src/box_manager/_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 13:45:46.324174 napari_boxmanager-0.3.7/src/box_manager/io/
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/src/box_manager/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9777 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/src/box_manager/io/box.py
--rw-r--r--   0 runner    (1001) docker     (123)    10229 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/src/box_manager/io/cbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/src/box_manager/io/coords.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/src/box_manager/io/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    19085 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/src/box_manager/io/io_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/src/box_manager/io/mrc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5793 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/src/box_manager/io/star.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/src/box_manager/io/tif.py
--rw-r--r--   0 runner    (1001) docker     (123)    10404 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/src/box_manager/io/tloc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/src/box_manager/napari.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 13:45:46.328174 napari_boxmanager-0.3.7/src/napari_boxmanager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-02-17 13:45:46.000000 napari_boxmanager-0.3.7/src/napari_boxmanager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-02-17 13:45:46.000000 napari_boxmanager-0.3.7/src/napari_boxmanager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-17 13:45:46.000000 napari_boxmanager-0.3.7/src/napari_boxmanager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-02-17 13:45:46.000000 napari_boxmanager-0.3.7/src/napari_boxmanager.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-02-17 13:45:46.000000 napari_boxmanager-0.3.7/src/napari_boxmanager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-02-17 13:45:46.000000 napari_boxmanager-0.3.7/src/napari_boxmanager.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 13:45:46.336174 napari_boxmanager-0.3.7/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)    41024 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/test_data/2d.mrc
--rw-r--r--   0 runner    (1001) docker     (123)    41024 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/test_data/2d_0.mrc
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/test_data/2d_0_center.box
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/test_data/2d_center.box
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/test_data/2d_center_float.box
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/test_data/2d_corrupt_has_string.box
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/test_data/2d_corrupt_unqual_columns.box
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/test_data/2d_empty.box
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/test_data/2d_left.box
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/test_data/2d_particles.cbox
--rw-r--r--   0 runner    (1001) docker     (123)  4001024 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/test_data/3d.mrc
--rw-r--r--   0 runner    (1001) docker     (123)  4001024 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/test_data/3d.mrci
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/test_data/3d_particle.cbox
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 13:45:46.340174 napari_boxmanager-0.3.7/test_data/box_data/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/test_data/box_data/create_data.py
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/test_data/box_data/test_0.box
--rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/test_data/box_data/test_0.mrc
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/test_data/box_data/test_0_new.box
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/test_data/box_data/test_1.box
--rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/test_data/box_data/test_1.mrc
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/test_data/box_data/test_1_centered.box
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/test_data/box_data/test_1_new.box
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/test_data/box_data/test_2.box
--rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/test_data/box_data/test_2.mrc
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/test_data/box_data/test_2_centered.box
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/test_data/box_data/test_2_new.box
--rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/test_data/box_data/test_3.mrc
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/test_data/box_data/test_4.box
--rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/test_data/box_data/test_4.mrc
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/test_data/box_data/test_4_new.box
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/test_data/box_data/test_5.box
--rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/test_data/box_data/test_5.mrc
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/test_data/box_data/test_6.box
--rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/test_data/box_data/test_6.mrc
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/test_data/box_data/test_6_centered.box
--rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/test_data/box_data/test_7.mrc
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/test_data/box_data/test_7_centered.box
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/test_data/box_data/test_7_new.box
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/test_data/box_data/test_8.box
--rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/test_data/box_data/test_8.mrc
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/test_data/box_data/test_8_centered.box
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/test_data/box_data/test_9.box
--rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/test_data/box_data/test_9.mrc
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/test_data/box_data/test_9_new.box
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 13:45:46.340174 napari_boxmanager-0.3.7/test_data/filament_cbox_2d/
--rw-r--r--   0 runner    (1001) docker     (123)    19405 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/test_data/filament_cbox_2d/ActLifeact_02885.cbox
--rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/test_data/filament_cbox_2d/ActLifeact_03047.cbox
--rw-r--r--   0 runner    (1001) docker     (123)     6365 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/test_data/filament_cbox_2d/ActLifeact_03070.cbox
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/test_data/filament_cbox_2d/ActLifeact_03211.cbox
--rw-r--r--   0 runner    (1001) docker     (123)    63796 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/test_data/filament_cbox_2d/ActLifeact_04203.cbox
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/test_data/filament_cbox_2d/empty.cbox
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 13:45:46.340174 napari_boxmanager-0.3.7/test_data/particle_cbox_2d/
--rw-r--r--   0 runner    (1001) docker     (123)    11983 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/test_data/particle_cbox_2d/TcdA1-0018_frames_sum.cbox
--rw-r--r--   0 runner    (1001) docker     (123)    12858 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/test_data/particle_cbox_2d/TcdA1-0019_frames_sum.cbox
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/test_data/valid.tloc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 13:45:46.340174 napari_boxmanager-0.3.7/test_data/valid_box/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/test_data/valid_box/2d.box
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/test_data/valid_box/2d_0.box
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/test_data/valid_missing_dim_z.tloc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 13:45:46.340174 napari_boxmanager-0.3.7/test_data/valid_mrc/
--rw-r--r--   0 runner    (1001) docker     (123)    41024 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/test_data/valid_mrc/2d.mrc
--rw-r--r--   0 runner    (1001) docker     (123)    41024 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/test_data/valid_mrc/2d_0.mrc
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-02-17 13:45:29.000000 napari_boxmanager-0.3.7/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 15:40:24.525256 napari_boxmanager-0.3.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 15:40:24.501256 napari_boxmanager-0.3.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 15:40:24.505256 napari_boxmanager-0.3.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 15:40:24.505256 napari_boxmanager-0.3.9/.napari/
+-rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/.napari/DESCRIPTION.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    16726 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-02-17 15:40:24.525256 napari_boxmanager-0.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 15:40:24.505256 napari_boxmanager-0.3.9/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      232 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/bin/napari_boxmanager
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 15:40:24.505256 napari_boxmanager-0.3.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 15:40:24.505256 napari_boxmanager-0.3.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/docs/_static/version-alert.js
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 15:40:24.505256 napari_boxmanager-0.3.9/docs/manual/
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/docs/manual/general.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/docs/manual/manual.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/docs/manual/read.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/docs/manual/write.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 15:40:24.505256 napari_boxmanager-0.3.9/reader_backup/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 15:40:24.505256 napari_boxmanager-0.3.9/reader_backup/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/reader_backup/_tests/test_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/reader_backup/_tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/reader_backup/_tests/test_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/reader_backup/_tests/test_tlpkl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/reader_backup/cbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/reader_backup/star.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/reader_backup/tepkl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/reader_backup/tlpkl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/reader_backup/tmpkl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/reader_backup/to_napari_backup.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-02-17 15:40:24.525256 napari_boxmanager-0.3.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 15:40:24.501256 napari_boxmanager-0.3.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 15:40:24.505256 napari_boxmanager-0.3.9/src/box_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/src/box_manager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 15:40:24.509256 napari_boxmanager-0.3.9/src/box_manager/_qt/
+-rw-r--r--   0 runner    (1001) docker     (123)     9326 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/src/box_manager/_qt/FilterImage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13471 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/src/box_manager/_qt/OrganizeBox.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17967 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/src/box_manager/_qt/OrganizeLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82644 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/src/box_manager/_qt/SelectMetric.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/src/box_manager/_qt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 15:40:24.509256 napari_boxmanager-0.3.9/src/box_manager/_qt/_icons/
+-rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/src/box_manager/_qt/_icons/checkmark_black.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/src/box_manager/_qt/_icons/checkmark_white.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/src/box_manager/_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/src/box_manager/_sample_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 15:40:24.509256 napari_boxmanager-0.3.9/src/box_manager/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/src/box_manager/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/src/box_manager/_tests/_dummy_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/src/box_manager/_tests/test_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/src/box_manager/_tests/test_cbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/src/box_manager/_tests/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/src/box_manager/_tests/test_sample_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/src/box_manager/_tests/test_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/src/box_manager/_tests/test_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 15:40:24.509256 napari_boxmanager-0.3.9/src/box_manager/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/src/box_manager/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/src/box_manager/_utils/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/src/box_manager/_utils/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-02-17 15:40:24.000000 napari_boxmanager-0.3.9/src/box_manager/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/src/box_manager/_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/src/box_manager/_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 15:40:24.509256 napari_boxmanager-0.3.9/src/box_manager/io/
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/src/box_manager/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9777 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/src/box_manager/io/box.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10911 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/src/box_manager/io/cbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/src/box_manager/io/coords.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/src/box_manager/io/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19151 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/src/box_manager/io/io_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/src/box_manager/io/mrc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5793 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/src/box_manager/io/star.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/src/box_manager/io/tif.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10404 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/src/box_manager/io/tloc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/src/box_manager/napari.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 15:40:24.509256 napari_boxmanager-0.3.9/src/napari_boxmanager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-02-17 15:40:24.000000 napari_boxmanager-0.3.9/src/napari_boxmanager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-02-17 15:40:24.000000 napari_boxmanager-0.3.9/src/napari_boxmanager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-17 15:40:24.000000 napari_boxmanager-0.3.9/src/napari_boxmanager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-02-17 15:40:24.000000 napari_boxmanager-0.3.9/src/napari_boxmanager.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-02-17 15:40:24.000000 napari_boxmanager-0.3.9/src/napari_boxmanager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-02-17 15:40:24.000000 napari_boxmanager-0.3.9/src/napari_boxmanager.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 15:40:24.521256 napari_boxmanager-0.3.9/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    41024 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/2d.mrc
+-rw-r--r--   0 runner    (1001) docker     (123)    41024 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/2d_0.mrc
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/2d_0_center.box
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/2d_center.box
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/2d_center_float.box
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/2d_corrupt_has_string.box
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/2d_corrupt_unqual_columns.box
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/2d_empty.box
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/2d_left.box
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/2d_particles.cbox
+-rw-r--r--   0 runner    (1001) docker     (123)  4001024 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/3d.mrc
+-rw-r--r--   0 runner    (1001) docker     (123)  4001024 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/3d.mrci
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/3d_particle.cbox
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 15:40:24.525256 napari_boxmanager-0.3.9/test_data/box_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/box_data/create_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/box_data/test_0.box
+-rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/box_data/test_0.mrc
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/box_data/test_0_new.box
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/box_data/test_1.box
+-rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/box_data/test_1.mrc
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/box_data/test_1_centered.box
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/box_data/test_1_new.box
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/box_data/test_2.box
+-rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/box_data/test_2.mrc
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/box_data/test_2_centered.box
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/box_data/test_2_new.box
+-rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/box_data/test_3.mrc
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/box_data/test_4.box
+-rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/box_data/test_4.mrc
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/box_data/test_4_new.box
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/box_data/test_5.box
+-rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/box_data/test_5.mrc
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/box_data/test_6.box
+-rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/box_data/test_6.mrc
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/box_data/test_6_centered.box
+-rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/box_data/test_7.mrc
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/box_data/test_7_centered.box
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/box_data/test_7_new.box
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/box_data/test_8.box
+-rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/box_data/test_8.mrc
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/box_data/test_8_centered.box
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/box_data/test_9.box
+-rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/box_data/test_9.mrc
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/box_data/test_9_new.box
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 15:40:24.525256 napari_boxmanager-0.3.9/test_data/filament_cbox_2d/
+-rw-r--r--   0 runner    (1001) docker     (123)    19405 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/filament_cbox_2d/ActLifeact_02885.cbox
+-rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/filament_cbox_2d/ActLifeact_03047.cbox
+-rw-r--r--   0 runner    (1001) docker     (123)     6365 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/filament_cbox_2d/ActLifeact_03070.cbox
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/filament_cbox_2d/ActLifeact_03211.cbox
+-rw-r--r--   0 runner    (1001) docker     (123)    63796 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/filament_cbox_2d/ActLifeact_04203.cbox
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/filament_cbox_2d/empty.cbox
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 15:40:24.525256 napari_boxmanager-0.3.9/test_data/particle_cbox_2d/
+-rw-r--r--   0 runner    (1001) docker     (123)    11983 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/particle_cbox_2d/TcdA1-0018_frames_sum.cbox
+-rw-r--r--   0 runner    (1001) docker     (123)    12858 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/particle_cbox_2d/TcdA1-0019_frames_sum.cbox
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/valid.tloc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 15:40:24.525256 napari_boxmanager-0.3.9/test_data/valid_box/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/valid_box/2d.box
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/valid_box/2d_0.box
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/valid_missing_dim_z.tloc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 15:40:24.525256 napari_boxmanager-0.3.9/test_data/valid_mrc/
+-rw-r--r--   0 runner    (1001) docker     (123)    41024 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/valid_mrc/2d.mrc
+-rw-r--r--   0 runner    (1001) docker     (123)    41024 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/test_data/valid_mrc/2d_0.mrc
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-02-17 15:40:06.000000 napari_boxmanager-0.3.9/tox.ini
```

### Comparing `napari_boxmanager-0.3.7/.github/workflows/test_and_deploy.yml` & `napari_boxmanager-0.3.9/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.7/.gitignore` & `napari_boxmanager-0.3.9/.gitignore`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.7/.napari/DESCRIPTION.md` & `napari_boxmanager-0.3.9/.napari/DESCRIPTION.md`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.7/.pre-commit-config.yaml` & `napari_boxmanager-0.3.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.7/LICENSE` & `napari_boxmanager-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.7/PKG-INFO` & `napari_boxmanager-0.3.9/src/napari_boxmanager.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: napari_boxmanager
-Version: 0.3.7
+Name: napari-boxmanager
+Version: 0.3.9
 Summary: Particle selection tool for cryo-em
 Home-page: https://github.com/MPI-Dortmund/napari-boxmanager
 Author: Markus Stabrin
 Author-email: markus.stabrin@mpi-dortmund.mpg.de
 License: MPL-2.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: napari
```

### Comparing `napari_boxmanager-0.3.7/README.md` & `napari_boxmanager-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.7/docs/_static/version-alert.js` & `napari_boxmanager-0.3.9/docs/_static/version-alert.js`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.7/docs/changes.rst` & `napari_boxmanager-0.3.9/docs/changes.rst`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.7/docs/conf.py` & `napari_boxmanager-0.3.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.7/docs/manual/general.rst` & `napari_boxmanager-0.3.9/docs/manual/general.rst`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.7/reader_backup/_tests/test_box.py` & `napari_boxmanager-0.3.9/reader_backup/_tests/test_box.py`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.7/reader_backup/_tests/test_interface.py` & `napari_boxmanager-0.3.9/reader_backup/_tests/test_interface.py`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.7/reader_backup/_tests/test_tlpkl.py` & `napari_boxmanager-0.3.9/reader_backup/_tests/test_tlpkl.py`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.7/reader_backup/tlpkl.py` & `napari_boxmanager-0.3.9/reader_backup/tlpkl.py`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.7/reader_backup/to_napari_backup.txt` & `napari_boxmanager-0.3.9/reader_backup/to_napari_backup.txt`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.7/setup.cfg` & `napari_boxmanager-0.3.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.7/src/box_manager/_qt/FilterImage.py` & `napari_boxmanager-0.3.9/src/box_manager/_qt/FilterImage.py`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.7/src/box_manager/_qt/OrganizeBox.py` & `napari_boxmanager-0.3.9/src/box_manager/_qt/OrganizeBox.py`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.7/src/box_manager/_qt/OrganizeLayer.py` & `napari_boxmanager-0.3.9/src/box_manager/_qt/OrganizeLayer.py`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.7/src/box_manager/_qt/SelectMetric.py` & `napari_boxmanager-0.3.9/src/box_manager/_qt/SelectMetric.py`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.7/src/box_manager/_qt/_icons/checkmark_black.png` & `napari_boxmanager-0.3.9/src/box_manager/_qt/_icons/checkmark_black.png`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.7/src/box_manager/_qt/_icons/checkmark_white.png` & `napari_boxmanager-0.3.9/src/box_manager/_qt/_icons/checkmark_white.png`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.7/src/box_manager/_reader.py` & `napari_boxmanager-0.3.9/src/box_manager/_reader.py`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.7/src/box_manager/_tests/test_box.py` & `napari_boxmanager-0.3.9/src/box_manager/_tests/test_box.py`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.7/src/box_manager/_tests/test_reader.py` & `napari_boxmanager-0.3.9/src/box_manager/_tests/test_reader.py`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.7/src/box_manager/_tests/test_widget.py` & `napari_boxmanager-0.3.9/src/box_manager/_tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.7/src/box_manager/_utils/filters.py` & `napari_boxmanager-0.3.9/src/box_manager/_utils/filters.py`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.7/src/box_manager/_utils/general.py` & `napari_boxmanager-0.3.9/src/box_manager/_utils/general.py`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.7/src/box_manager/_widget.py` & `napari_boxmanager-0.3.9/src/box_manager/_widget.py`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.7/src/box_manager/_writer.py` & `napari_boxmanager-0.3.9/src/box_manager/_writer.py`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.7/src/box_manager/io/__init__.py` & `napari_boxmanager-0.3.9/src/box_manager/io/__init__.py`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.7/src/box_manager/io/box.py` & `napari_boxmanager-0.3.9/src/box_manager/io/box.py`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.7/src/box_manager/io/cbox.py` & `napari_boxmanager-0.3.9/src/box_manager/io/cbox.py`

 * *Files 9% similar despite different names*

```diff
@@ -33,28 +33,51 @@
 def to_napari(
     path: os.PathLike | list[os.PathLike],
 ) -> "list[NapariLayerData]":
     r = coordsio.to_napari_coordinates(
         path=path,
         read_func=read,
         prepare_napari_func=_prepare_napari,
-        meta_columns=[],
-        feature_columns=[],
+        meta_columns=["confidence","size","num_boxes"],
+        feature_columns=['angle','fid'],
         valid_extensions=get_valid_extensions(),
     )
 
     return r
 
 
+
+def read_cbox_boxfile_old(path):
+    """
+    Read a box file in EMAN1 box format.
+    :param path: Path to box file
+    :return: List of bounding boxes
+    """
+    boxreader = np.atleast_2d(np.genfromtxt(path))
+    box_dat = {
+        "_CoordinateX": [box[0] for box in boxreader],
+        "_CoordinateY": [box[1] for box in boxreader],
+        "_Width": [box[2] for box in boxreader],
+        "_Height": [box[3] for box in boxreader],
+        "_Confidence": [box[4] for box in boxreader]
+    }
+
+    return pd.DataFrame(box_dat)
+
+
 def read(path: os.PathLike) -> pd.DataFrame:
     try:
         starfile = star.StarFile(path)
         data_dict = starfile["cryolo"]
-    except TypeError:
-        return None
+    except Exception:
+        try:
+            a =  read_cbox_boxfile_old(path)
+        except Exception:
+            return None
+        return a
     return pd.DataFrame(data_dict)
 
 
 ### Writing ####
 ################
 
 
@@ -194,15 +217,17 @@
     -------
     Dataframe with centered coordinates and additional metadate if necessary.
 
     """
 
     cryolo_data = input_df
 
+
     feature_columns, meta_columns = _fill_meta_features_idx(cryolo_data)
+
     is_3d = True
     if (
         "_CoordinateZ" not in cryolo_data
         or cryolo_data["_CoordinateZ"].isnull().values.any()
     ):
         is_3d = False
 
@@ -259,15 +284,14 @@
     Returns
     -------
     None
 
     """
     meta_columns = []
     feature_columns = []
-
     if (
         "_EstWidth" in input_df.columns
         and not input_df["_EstWidth"].isnull().values.any()
     ) and "size" not in meta_columns:
         meta_columns.append("size")
 
     if (
```

### Comparing `napari_boxmanager-0.3.7/src/box_manager/io/coords.py` & `napari_boxmanager-0.3.9/src/box_manager/io/coords.py`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.7/src/box_manager/io/interface.py` & `napari_boxmanager-0.3.9/src/box_manager/io/interface.py`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.7/src/box_manager/io/io_utils.py` & `napari_boxmanager-0.3.9/src/box_manager/io/io_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -296,14 +296,16 @@
     metadata.update(orgbox_meta)
     metadata["is_2d_stack"] = is_2d_stack
     metadata["ignore_idx"] = feature_columns
     features = {}
     for entry in feature_columns + meta_columns:
         if metadata["is_filament_layer"]:
             for fil in input_df_list:
+                if entry not in fil:
+                    continue
                 if entry in features:
                     features[entry] = np.concatenate(
                         [features[entry], fil[entry].to_numpy()]
                     )
                 else:
                     features[entry] = fil[entry].to_numpy()
         else:
```

### Comparing `napari_boxmanager-0.3.7/src/box_manager/io/mrc.py` & `napari_boxmanager-0.3.9/src/box_manager/io/mrc.py`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.7/src/box_manager/io/star.py` & `napari_boxmanager-0.3.9/src/box_manager/io/star.py`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.7/src/box_manager/io/tif.py` & `napari_boxmanager-0.3.9/src/box_manager/io/tif.py`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.7/src/box_manager/io/tloc.py` & `napari_boxmanager-0.3.9/src/box_manager/io/tloc.py`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.7/src/box_manager/napari.yaml` & `napari_boxmanager-0.3.9/src/box_manager/napari.yaml`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.7/src/napari_boxmanager.egg-info/PKG-INFO` & `napari_boxmanager-0.3.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: napari-boxmanager
-Version: 0.3.7
+Name: napari_boxmanager
+Version: 0.3.9
 Summary: Particle selection tool for cryo-em
 Home-page: https://github.com/MPI-Dortmund/napari-boxmanager
 Author: Markus Stabrin
 Author-email: markus.stabrin@mpi-dortmund.mpg.de
 License: MPL-2.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: napari
```

### Comparing `napari_boxmanager-0.3.7/src/napari_boxmanager.egg-info/SOURCES.txt` & `napari_boxmanager-0.3.9/src/napari_boxmanager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.7/test_data/2d.mrc` & `napari_boxmanager-0.3.9/test_data/2d.mrc`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.7/test_data/2d_0.mrc` & `napari_boxmanager-0.3.9/test_data/2d_0.mrc`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.7/test_data/2d_particles.cbox` & `napari_boxmanager-0.3.9/test_data/2d_particles.cbox`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.7/test_data/3d.mrc` & `napari_boxmanager-0.3.9/test_data/3d.mrc`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.7/test_data/3d.mrci` & `napari_boxmanager-0.3.9/test_data/3d.mrci`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.7/test_data/3d_particle.cbox` & `napari_boxmanager-0.3.9/test_data/3d_particle.cbox`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.7/test_data/box_data/create_data.py` & `napari_boxmanager-0.3.9/test_data/box_data/create_data.py`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.7/test_data/box_data/test_0.mrc` & `napari_boxmanager-0.3.9/test_data/box_data/test_0.mrc`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.7/test_data/box_data/test_1.mrc` & `napari_boxmanager-0.3.9/test_data/box_data/test_1.mrc`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.7/test_data/box_data/test_2.mrc` & `napari_boxmanager-0.3.9/test_data/box_data/test_2.mrc`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.7/test_data/box_data/test_3.mrc` & `napari_boxmanager-0.3.9/test_data/box_data/test_3.mrc`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.7/test_data/box_data/test_4.mrc` & `napari_boxmanager-0.3.9/test_data/box_data/test_4.mrc`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.7/test_data/box_data/test_5.mrc` & `napari_boxmanager-0.3.9/test_data/box_data/test_5.mrc`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.7/test_data/box_data/test_6.mrc` & `napari_boxmanager-0.3.9/test_data/box_data/test_6.mrc`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.7/test_data/box_data/test_7.mrc` & `napari_boxmanager-0.3.9/test_data/box_data/test_7.mrc`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.7/test_data/box_data/test_8.mrc` & `napari_boxmanager-0.3.9/test_data/box_data/test_8.mrc`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.7/test_data/box_data/test_9.mrc` & `napari_boxmanager-0.3.9/test_data/box_data/test_9.mrc`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.7/test_data/filament_cbox_2d/ActLifeact_02885.cbox` & `napari_boxmanager-0.3.9/test_data/filament_cbox_2d/ActLifeact_02885.cbox`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.7/test_data/filament_cbox_2d/ActLifeact_03047.cbox` & `napari_boxmanager-0.3.9/test_data/filament_cbox_2d/ActLifeact_03047.cbox`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.7/test_data/filament_cbox_2d/ActLifeact_03070.cbox` & `napari_boxmanager-0.3.9/test_data/filament_cbox_2d/ActLifeact_03070.cbox`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.7/test_data/filament_cbox_2d/ActLifeact_03211.cbox` & `napari_boxmanager-0.3.9/test_data/filament_cbox_2d/ActLifeact_03211.cbox`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.7/test_data/filament_cbox_2d/ActLifeact_04203.cbox` & `napari_boxmanager-0.3.9/test_data/filament_cbox_2d/ActLifeact_04203.cbox`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.7/test_data/particle_cbox_2d/TcdA1-0018_frames_sum.cbox` & `napari_boxmanager-0.3.9/test_data/particle_cbox_2d/TcdA1-0018_frames_sum.cbox`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.7/test_data/particle_cbox_2d/TcdA1-0019_frames_sum.cbox` & `napari_boxmanager-0.3.9/test_data/particle_cbox_2d/TcdA1-0019_frames_sum.cbox`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.7/test_data/valid.tloc` & `napari_boxmanager-0.3.9/test_data/valid.tloc`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.7/test_data/valid_missing_dim_z.tloc` & `napari_boxmanager-0.3.9/test_data/valid_missing_dim_z.tloc`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.7/test_data/valid_mrc/2d.mrc` & `napari_boxmanager-0.3.9/test_data/valid_mrc/2d.mrc`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.7/test_data/valid_mrc/2d_0.mrc` & `napari_boxmanager-0.3.9/test_data/valid_mrc/2d_0.mrc`

 * *Files identical despite different names*

### Comparing `napari_boxmanager-0.3.7/tox.ini` & `napari_boxmanager-0.3.9/tox.ini`

 * *Files identical despite different names*

