# Comparing `tmp/steinbock-0.9.0.tar.gz` & `tmp/steinbock-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "steinbock-0.9.0.tar", last modified: Mon Oct 11 17:12:14 2021, max compression
+gzip compressed data, was "steinbock-0.9.1.tar", last modified: Tue Oct 12 13:28:51 2021, max compression
```

## Comparing `steinbock-0.9.0.tar` & `steinbock-0.9.1.tar`

### file list

```diff
@@ -1,158 +1,160 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 17:12:14.607956 steinbock-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (121)     2254 2021-10-11 17:12:04.000000 steinbock-0.9.0/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 17:12:14.579955 steinbock-0.9.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 17:12:14.583956 steinbock-0.9.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2297 2021-10-11 17:12:04.000000 steinbock-0.9.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2021-10-11 17:12:04.000000 steinbock-0.9.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2077 2021-10-11 17:12:04.000000 steinbock-0.9.0/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 17:12:14.587956 steinbock-0.9.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (121)     1556 2021-10-11 17:12:04.000000 steinbock-0.9.0/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (121)      334 2021-10-11 17:12:04.000000 steinbock-0.9.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (121)      792 2021-10-11 17:12:04.000000 steinbock-0.9.0/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (121)       87 2021-10-11 17:12:04.000000 steinbock-0.9.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (121)     8198 2021-10-11 17:12:04.000000 steinbock-0.9.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)     1739 2021-10-11 17:12:04.000000 steinbock-0.9.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)      222 2021-10-11 17:12:04.000000 steinbock-0.9.0/CONTRIBUTORS.md
--rw-r--r--   0 runner    (1001) docker     (121)     3069 2021-10-11 17:12:04.000000 steinbock-0.9.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (121)     1077 2021-10-11 17:12:04.000000 steinbock-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       28 2021-10-11 17:12:04.000000 steinbock-0.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2266 2021-10-11 17:12:14.607956 steinbock-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1558 2021-10-11 17:12:04.000000 steinbock-0.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     1029 2021-10-11 17:12:04.000000 steinbock-0.9.0/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     1392 2021-10-11 17:12:04.000000 steinbock-0.9.0/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 17:12:14.587956 steinbock-0.9.0/docs/
--rw-r--r--   0 runner    (1001) docker     (121)       87 2021-10-11 17:12:04.000000 steinbock-0.9.0/docs/authors.md
--rw-r--r--   0 runner    (1001) docker     (121)     8198 2021-10-11 17:12:04.000000 steinbock-0.9.0/docs/changelog.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 17:12:14.587956 steinbock-0.9.0/docs/cli/
--rw-r--r--   0 runner    (1001) docker     (121)      617 2021-10-11 17:12:04.000000 steinbock-0.9.0/docs/cli/apps.md
--rw-r--r--   0 runner    (1001) docker     (121)     6316 2021-10-11 17:12:04.000000 steinbock-0.9.0/docs/cli/classification.md
--rw-r--r--   0 runner    (1001) docker     (121)     2915 2021-10-11 17:12:04.000000 steinbock-0.9.0/docs/cli/export.md
--rw-r--r--   0 runner    (1001) docker     (121)     2074 2021-10-11 17:12:04.000000 steinbock-0.9.0/docs/cli/intro.md
--rw-r--r--   0 runner    (1001) docker     (121)     6159 2021-10-11 17:12:04.000000 steinbock-0.9.0/docs/cli/measurement.md
--rw-r--r--   0 runner    (1001) docker     (121)     6514 2021-10-11 17:12:04.000000 steinbock-0.9.0/docs/cli/preprocessing.md
--rw-r--r--   0 runner    (1001) docker     (121)     6842 2021-10-11 17:12:04.000000 steinbock-0.9.0/docs/cli/segmentation.md
--rw-r--r--   0 runner    (1001) docker     (121)     2036 2021-10-11 17:12:04.000000 steinbock-0.9.0/docs/cli/utils.md
--rw-r--r--   0 runner    (1001) docker     (121)     1739 2021-10-11 17:12:04.000000 steinbock-0.9.0/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (121)      222 2021-10-11 17:12:04.000000 steinbock-0.9.0/docs/contributors.md
--rw-r--r--   0 runner    (1001) docker     (121)     1252 2021-10-11 17:12:04.000000 steinbock-0.9.0/docs/directories.md
--rw-r--r--   0 runner    (1001) docker     (121)     6699 2021-10-11 17:12:04.000000 steinbock-0.9.0/docs/docker.md
--rw-r--r--   0 runner    (1001) docker     (121)     3170 2021-10-11 17:12:04.000000 steinbock-0.9.0/docs/file-types.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 17:12:14.587956 steinbock-0.9.0/docs/img/
--rw-r--r--   0 runner    (1001) docker     (121)    42162 2021-10-11 17:12:04.000000 steinbock-0.9.0/docs/img/steinbock-logo.png
--rw-r--r--   0 runner    (1001) docker     (121)     2507 2021-10-11 17:12:04.000000 steinbock-0.9.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (121)      163 2021-10-11 17:12:04.000000 steinbock-0.9.0/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (121)      149 2021-10-11 17:12:04.000000 steinbock-0.9.0/docs/mkdocstrings.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 17:12:14.587956 steinbock-0.9.0/docs/python/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 17:12:14.587956 steinbock-0.9.0/docs/python/api/
--rw-r--r--   0 runner    (1001) docker     (121)       57 2021-10-11 17:12:04.000000 steinbock-0.9.0/docs/python/api/steinbock.classification.md
--rw-r--r--   0 runner    (1001) docker     (121)       41 2021-10-11 17:12:04.000000 steinbock-0.9.0/docs/python/api/steinbock.export.md
--rw-r--r--   0 runner    (1001) docker     (121)       33 2021-10-11 17:12:04.000000 steinbock-0.9.0/docs/python/api/steinbock.io.md
--rw-r--r--   0 runner    (1001) docker     (121)       51 2021-10-11 17:12:04.000000 steinbock-0.9.0/docs/python/api/steinbock.measurement.md
--rw-r--r--   0 runner    (1001) docker     (121)       55 2021-10-11 17:12:04.000000 steinbock-0.9.0/docs/python/api/steinbock.preprocessing.md
--rw-r--r--   0 runner    (1001) docker     (121)       53 2021-10-11 17:12:04.000000 steinbock-0.9.0/docs/python/api/steinbock.segmentation.md
--rw-r--r--   0 runner    (1001) docker     (121)       39 2021-10-11 17:12:04.000000 steinbock-0.9.0/docs/python/api/steinbock.utils.md
--rw-r--r--   0 runner    (1001) docker     (121)      267 2021-10-11 17:12:04.000000 steinbock-0.9.0/docs/python/intro.md
--rw-r--r--   0 runner    (1001) docker     (121)     1254 2021-10-11 17:12:04.000000 steinbock-0.9.0/docs/python.md
--rw-r--r--   0 runner    (1001) docker     (121)       56 2021-10-11 17:12:04.000000 steinbock-0.9.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       65 2021-10-11 17:12:04.000000 steinbock-0.9.0/entrypoint.sh
--rw-r--r--   0 runner    (1001) docker     (121)       70 2021-10-11 17:12:04.000000 steinbock-0.9.0/fixuid.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1340 2021-10-11 17:12:04.000000 steinbock-0.9.0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)      266 2021-10-11 17:12:04.000000 steinbock-0.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      423 2021-10-11 17:12:04.000000 steinbock-0.9.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      995 2021-10-11 17:12:14.607956 steinbock-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       91 2021-10-11 17:12:04.000000 steinbock-0.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 17:12:14.591956 steinbock-0.9.0/steinbock/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-11 17:12:04.000000 steinbock-0.9.0/steinbock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      123 2021-10-11 17:12:04.000000 steinbock-0.9.0/steinbock/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 17:12:14.591956 steinbock-0.9.0/steinbock/_cli/
--rw-r--r--   0 runner    (1001) docker     (121)     1000 2021-10-11 17:12:04.000000 steinbock-0.9.0/steinbock/_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1448 2021-10-11 17:12:04.000000 steinbock-0.9.0/steinbock/_cli/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)      325 2021-10-11 17:12:04.000000 steinbock-0.9.0/steinbock/_cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2868 2021-10-11 17:12:04.000000 steinbock-0.9.0/steinbock/_env.py
--rw-r--r--   0 runner    (1001) docker     (121)      142 2021-10-11 17:12:14.000000 steinbock-0.9.0/steinbock/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 17:12:14.591956 steinbock-0.9.0/steinbock/classification/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-11 17:12:04.000000 steinbock-0.9.0/steinbock/classification/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 17:12:14.591956 steinbock-0.9.0/steinbock/classification/_cli/
--rw-r--r--   0 runner    (1001) docker     (121)      352 2021-10-11 17:12:04.000000 steinbock-0.9.0/steinbock/classification/_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9458 2021-10-11 17:12:04.000000 steinbock-0.9.0/steinbock/classification/_cli/ilastik.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 17:12:14.591956 steinbock-0.9.0/steinbock/classification/ilastik/
--rw-r--r--   0 runner    (1001) docker     (121)      959 2021-10-11 17:12:04.000000 steinbock-0.9.0/steinbock/classification/ilastik/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    21211 2021-10-11 17:12:04.000000 steinbock-0.9.0/steinbock/classification/ilastik/_ilastik.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 17:12:14.591956 steinbock-0.9.0/steinbock/classification/ilastik/data/
--rw-r--r--   0 runner    (1001) docker     (121)  1108944 2021-10-11 17:12:04.000000 steinbock-0.9.0/steinbock/classification/ilastik/data/pixel_classifier.ilp
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 17:12:14.595956 steinbock-0.9.0/steinbock/export/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-11 17:12:04.000000 steinbock-0.9.0/steinbock/export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9540 2021-10-11 17:12:04.000000 steinbock-0.9.0/steinbock/export/_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     1858 2021-10-11 17:12:04.000000 steinbock-0.9.0/steinbock/export/data.py
--rw-r--r--   0 runner    (1001) docker     (121)     1939 2021-10-11 17:12:04.000000 steinbock-0.9.0/steinbock/export/graphs.py
--rw-r--r--   0 runner    (1001) docker     (121)     9059 2021-10-11 17:12:04.000000 steinbock-0.9.0/steinbock/io.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 17:12:14.595956 steinbock-0.9.0/steinbock/measurement/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-11 17:12:04.000000 steinbock-0.9.0/steinbock/measurement/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 17:12:14.599956 steinbock-0.9.0/steinbock/measurement/_cli/
--rw-r--r--   0 runner    (1001) docker     (121)      685 2021-10-11 17:12:04.000000 steinbock-0.9.0/steinbock/measurement/_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3382 2021-10-11 17:12:04.000000 steinbock-0.9.0/steinbock/measurement/_cli/cellprofiler.py
--rw-r--r--   0 runner    (1001) docker     (121)     2371 2021-10-11 17:12:04.000000 steinbock-0.9.0/steinbock/measurement/_cli/intensities.py
--rw-r--r--   0 runner    (1001) docker     (121)     2048 2021-10-11 17:12:04.000000 steinbock-0.9.0/steinbock/measurement/_cli/neighbors.py
--rw-r--r--   0 runner    (1001) docker     (121)     1715 2021-10-11 17:12:04.000000 steinbock-0.9.0/steinbock/measurement/_cli/regionprops.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 17:12:14.599956 steinbock-0.9.0/steinbock/measurement/cellprofiler/
--rw-r--r--   0 runner    (1001) docker     (121)      207 2021-10-11 17:12:04.000000 steinbock-0.9.0/steinbock/measurement/cellprofiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1190 2021-10-11 17:12:04.000000 steinbock-0.9.0/steinbock/measurement/cellprofiler/_cellprofiler.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 17:12:14.599956 steinbock-0.9.0/steinbock/measurement/cellprofiler/data/
--rw-r--r--   0 runner    (1001) docker     (121)     6801 2021-10-11 17:12:04.000000 steinbock-0.9.0/steinbock/measurement/cellprofiler/data/cell_measurement.cppipe
--rw-r--r--   0 runner    (1001) docker     (121)     1927 2021-10-11 17:12:04.000000 steinbock-0.9.0/steinbock/measurement/intensities.py
--rw-r--r--   0 runner    (1001) docker     (121)     7149 2021-10-11 17:12:04.000000 steinbock-0.9.0/steinbock/measurement/neighbors.py
--rw-r--r--   0 runner    (1001) docker     (121)     1499 2021-10-11 17:12:04.000000 steinbock-0.9.0/steinbock/measurement/regionprops.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 17:12:14.599956 steinbock-0.9.0/steinbock/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-11 17:12:04.000000 steinbock-0.9.0/steinbock/preprocessing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 17:12:14.599956 steinbock-0.9.0/steinbock/preprocessing/_cli/
--rw-r--r--   0 runner    (1001) docker     (121)      380 2021-10-11 17:12:04.000000 steinbock-0.9.0/steinbock/preprocessing/_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7259 2021-10-11 17:12:04.000000 steinbock-0.9.0/steinbock/preprocessing/_cli/imc.py
--rw-r--r--   0 runner    (1001) docker     (121)     8580 2021-10-11 17:12:04.000000 steinbock-0.9.0/steinbock/preprocessing/imc.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 17:12:14.599956 steinbock-0.9.0/steinbock/segmentation/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-11 17:12:04.000000 steinbock-0.9.0/steinbock/segmentation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 17:12:14.599956 steinbock-0.9.0/steinbock/segmentation/_cli/
--rw-r--r--   0 runner    (1001) docker     (121)      532 2021-10-11 17:12:04.000000 steinbock-0.9.0/steinbock/segmentation/_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2346 2021-10-11 17:12:04.000000 steinbock-0.9.0/steinbock/segmentation/_cli/cellprofiler.py
--rw-r--r--   0 runner    (1001) docker     (121)     4760 2021-10-11 17:12:04.000000 steinbock-0.9.0/steinbock/segmentation/_cli/deepcell.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 17:12:14.599956 steinbock-0.9.0/steinbock/segmentation/cellprofiler/
--rw-r--r--   0 runner    (1001) docker     (121)      210 2021-10-11 17:12:04.000000 steinbock-0.9.0/steinbock/segmentation/cellprofiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1101 2021-10-11 17:12:04.000000 steinbock-0.9.0/steinbock/segmentation/cellprofiler/_cellprofiler.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 17:12:14.599956 steinbock-0.9.0/steinbock/segmentation/cellprofiler/data/
--rw-r--r--   0 runner    (1001) docker     (121)    10832 2021-10-11 17:12:04.000000 steinbock-0.9.0/steinbock/segmentation/cellprofiler/data/cell_segmentation.cppipe
--rw-r--r--   0 runner    (1001) docker     (121)     3273 2021-10-11 17:12:04.000000 steinbock-0.9.0/steinbock/segmentation/deepcell.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 17:12:14.603956 steinbock-0.9.0/steinbock/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-11 17:12:04.000000 steinbock-0.9.0/steinbock/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 17:12:14.603956 steinbock-0.9.0/steinbock/utils/_cli/
--rw-r--r--   0 runner    (1001) docker     (121)     1620 2021-10-11 17:12:04.000000 steinbock-0.9.0/steinbock/utils/_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2726 2021-10-11 17:12:04.000000 steinbock-0.9.0/steinbock/utils/_cli/mosaics.py
--rw-r--r--   0 runner    (1001) docker     (121)     1476 2021-10-11 17:12:04.000000 steinbock-0.9.0/steinbock/utils/matching.py
--rw-r--r--   0 runner    (1001) docker     (121)     2372 2021-10-11 17:12:04.000000 steinbock-0.9.0/steinbock/utils/mosaics.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 17:12:14.591956 steinbock-0.9.0/steinbock.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2266 2021-10-11 17:12:14.000000 steinbock-0.9.0/steinbock.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3592 2021-10-11 17:12:14.000000 steinbock-0.9.0/steinbock.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-11 17:12:14.000000 steinbock-0.9.0/steinbock.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       66 2021-10-11 17:12:14.000000 steinbock-0.9.0/steinbock.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-11 17:12:14.000000 steinbock-0.9.0/steinbock.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      151 2021-10-11 17:12:14.000000 steinbock-0.9.0/steinbock.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2021-10-11 17:12:14.000000 steinbock-0.9.0/steinbock.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 17:12:14.603956 steinbock-0.9.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 17:12:14.603956 steinbock-0.9.0/tests/classification/
--rw-r--r--   0 runner    (1001) docker     (121)     5986 2021-10-11 17:12:04.000000 steinbock-0.9.0/tests/classification/test_ilastik_classification.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 17:12:14.603956 steinbock-0.9.0/tests/export/
--rw-r--r--   0 runner    (1001) docker     (121)     1184 2021-10-11 17:12:04.000000 steinbock-0.9.0/tests/export/test_data_export.py
--rw-r--r--   0 runner    (1001) docker     (121)     1392 2021-10-11 17:12:04.000000 steinbock-0.9.0/tests/export/test_graphs_export.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 17:12:14.603956 steinbock-0.9.0/tests/measurement/
--rw-r--r--   0 runner    (1001) docker     (121)     1042 2021-10-11 17:12:04.000000 steinbock-0.9.0/tests/measurement/test_cellprofiler_measurement.py
--rw-r--r--   0 runner    (1001) docker     (121)     1830 2021-10-11 17:12:04.000000 steinbock-0.9.0/tests/measurement/test_intensities_measurement.py
--rw-r--r--   0 runner    (1001) docker     (121)     1888 2021-10-11 17:12:04.000000 steinbock-0.9.0/tests/measurement/test_neighbors_measurement.py
--rw-r--r--   0 runner    (1001) docker     (121)     1310 2021-10-11 17:12:04.000000 steinbock-0.9.0/tests/measurement/test_regionprops_measurement.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 17:12:14.603956 steinbock-0.9.0/tests/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (121)     3184 2021-10-11 17:12:04.000000 steinbock-0.9.0/tests/preprocessing/test_imc_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (121)       49 2021-10-11 17:12:04.000000 steinbock-0.9.0/tests/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 17:12:14.607956 steinbock-0.9.0/tests/segmentation/
--rw-r--r--   0 runner    (1001) docker     (121)     1034 2021-10-11 17:12:04.000000 steinbock-0.9.0/tests/segmentation/test_cellprofiler_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (121)     1171 2021-10-11 17:12:04.000000 steinbock-0.9.0/tests/segmentation/test_deepcell_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (121)     2428 2021-10-11 17:12:04.000000 steinbock-0.9.0/tests/test_io.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 17:12:14.607956 steinbock-0.9.0/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (121)     1050 2021-10-11 17:12:04.000000 steinbock-0.9.0/tests/utils/test_matching_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1218 2021-10-11 17:12:04.000000 steinbock-0.9.0/tests/utils/test_mosaics_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-12 13:28:51.149100 steinbock-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (121)     2254 2021-10-12 13:28:40.000000 steinbock-0.9.1/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-12 13:28:51.133099 steinbock-0.9.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-12 13:28:51.137100 steinbock-0.9.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2297 2021-10-12 13:28:40.000000 steinbock-0.9.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2021-10-12 13:28:40.000000 steinbock-0.9.1/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2077 2021-10-12 13:28:40.000000 steinbock-0.9.1/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-12 13:28:51.137100 steinbock-0.9.1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (121)     1556 2021-10-12 13:28:40.000000 steinbock-0.9.1/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (121)      334 2021-10-12 13:28:40.000000 steinbock-0.9.1/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (121)      792 2021-10-12 13:28:40.000000 steinbock-0.9.1/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (121)       87 2021-10-12 13:28:40.000000 steinbock-0.9.1/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (121)     8364 2021-10-12 13:28:40.000000 steinbock-0.9.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1739 2021-10-12 13:28:40.000000 steinbock-0.9.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (121)      222 2021-10-12 13:28:40.000000 steinbock-0.9.1/CONTRIBUTORS.md
+-rw-r--r--   0 runner    (1001) docker     (121)     3069 2021-10-12 13:28:40.000000 steinbock-0.9.1/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (121)     1077 2021-10-12 13:28:40.000000 steinbock-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       28 2021-10-12 13:28:40.000000 steinbock-0.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     2332 2021-10-12 13:28:51.149100 steinbock-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1624 2021-10-12 13:28:40.000000 steinbock-0.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1029 2021-10-12 13:28:40.000000 steinbock-0.9.1/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1392 2021-10-12 13:28:40.000000 steinbock-0.9.1/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-12 13:28:51.141100 steinbock-0.9.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (121)       87 2021-10-12 13:28:40.000000 steinbock-0.9.1/docs/authors.md
+-rw-r--r--   0 runner    (1001) docker     (121)     8364 2021-10-12 13:28:40.000000 steinbock-0.9.1/docs/changelog.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-12 13:28:51.141100 steinbock-0.9.1/docs/cli/
+-rw-r--r--   0 runner    (1001) docker     (121)      617 2021-10-12 13:28:40.000000 steinbock-0.9.1/docs/cli/apps.md
+-rw-r--r--   0 runner    (1001) docker     (121)     6316 2021-10-12 13:28:40.000000 steinbock-0.9.1/docs/cli/classification.md
+-rw-r--r--   0 runner    (1001) docker     (121)     2915 2021-10-12 13:28:40.000000 steinbock-0.9.1/docs/cli/export.md
+-rw-r--r--   0 runner    (1001) docker     (121)     2074 2021-10-12 13:28:40.000000 steinbock-0.9.1/docs/cli/intro.md
+-rw-r--r--   0 runner    (1001) docker     (121)     6159 2021-10-12 13:28:40.000000 steinbock-0.9.1/docs/cli/measurement.md
+-rw-r--r--   0 runner    (1001) docker     (121)     6564 2021-10-12 13:28:40.000000 steinbock-0.9.1/docs/cli/preprocessing.md
+-rw-r--r--   0 runner    (1001) docker     (121)     6842 2021-10-12 13:28:40.000000 steinbock-0.9.1/docs/cli/segmentation.md
+-rw-r--r--   0 runner    (1001) docker     (121)     2036 2021-10-12 13:28:40.000000 steinbock-0.9.1/docs/cli/utils.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1739 2021-10-12 13:28:40.000000 steinbock-0.9.1/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (121)      222 2021-10-12 13:28:40.000000 steinbock-0.9.1/docs/contributors.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1252 2021-10-12 13:28:40.000000 steinbock-0.9.1/docs/directories.md
+-rw-r--r--   0 runner    (1001) docker     (121)     6699 2021-10-12 13:28:40.000000 steinbock-0.9.1/docs/docker.md
+-rw-r--r--   0 runner    (1001) docker     (121)     3170 2021-10-12 13:28:40.000000 steinbock-0.9.1/docs/file-types.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-12 13:28:51.141100 steinbock-0.9.1/docs/img/
+-rw-r--r--   0 runner    (1001) docker     (121)     1465 2021-10-12 13:28:40.000000 steinbock-0.9.1/docs/img/steinbock-favicon.png
+-rw-r--r--   0 runner    (1001) docker     (121)    19671 2021-10-12 13:28:40.000000 steinbock-0.9.1/docs/img/steinbock-logo-white.png
+-rw-r--r--   0 runner    (1001) docker     (121)    42162 2021-10-12 13:28:40.000000 steinbock-0.9.1/docs/img/steinbock-logo.png
+-rw-r--r--   0 runner    (1001) docker     (121)     2507 2021-10-12 13:28:40.000000 steinbock-0.9.1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (121)      230 2021-10-12 13:28:40.000000 steinbock-0.9.1/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (121)      149 2021-10-12 13:28:40.000000 steinbock-0.9.1/docs/mkdocstrings.css
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-12 13:28:51.141100 steinbock-0.9.1/docs/python/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-12 13:28:51.141100 steinbock-0.9.1/docs/python/api/
+-rw-r--r--   0 runner    (1001) docker     (121)       57 2021-10-12 13:28:40.000000 steinbock-0.9.1/docs/python/api/steinbock.classification.md
+-rw-r--r--   0 runner    (1001) docker     (121)       41 2021-10-12 13:28:40.000000 steinbock-0.9.1/docs/python/api/steinbock.export.md
+-rw-r--r--   0 runner    (1001) docker     (121)       33 2021-10-12 13:28:40.000000 steinbock-0.9.1/docs/python/api/steinbock.io.md
+-rw-r--r--   0 runner    (1001) docker     (121)       51 2021-10-12 13:28:40.000000 steinbock-0.9.1/docs/python/api/steinbock.measurement.md
+-rw-r--r--   0 runner    (1001) docker     (121)       55 2021-10-12 13:28:40.000000 steinbock-0.9.1/docs/python/api/steinbock.preprocessing.md
+-rw-r--r--   0 runner    (1001) docker     (121)       53 2021-10-12 13:28:40.000000 steinbock-0.9.1/docs/python/api/steinbock.segmentation.md
+-rw-r--r--   0 runner    (1001) docker     (121)       39 2021-10-12 13:28:40.000000 steinbock-0.9.1/docs/python/api/steinbock.utils.md
+-rw-r--r--   0 runner    (1001) docker     (121)      267 2021-10-12 13:28:40.000000 steinbock-0.9.1/docs/python/intro.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1254 2021-10-12 13:28:40.000000 steinbock-0.9.1/docs/python.md
+-rw-r--r--   0 runner    (1001) docker     (121)       56 2021-10-12 13:28:40.000000 steinbock-0.9.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       65 2021-10-12 13:28:40.000000 steinbock-0.9.1/entrypoint.sh
+-rw-r--r--   0 runner    (1001) docker     (121)       70 2021-10-12 13:28:40.000000 steinbock-0.9.1/fixuid.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1423 2021-10-12 13:28:40.000000 steinbock-0.9.1/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      266 2021-10-12 13:28:40.000000 steinbock-0.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      423 2021-10-12 13:28:40.000000 steinbock-0.9.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      995 2021-10-12 13:28:51.153101 steinbock-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)       91 2021-10-12 13:28:40.000000 steinbock-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-12 13:28:51.141100 steinbock-0.9.1/steinbock/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-12 13:28:40.000000 steinbock-0.9.1/steinbock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2021-10-12 13:28:40.000000 steinbock-0.9.1/steinbock/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-12 13:28:51.145100 steinbock-0.9.1/steinbock/_cli/
+-rw-r--r--   0 runner    (1001) docker     (121)     1000 2021-10-12 13:28:40.000000 steinbock-0.9.1/steinbock/_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1448 2021-10-12 13:28:40.000000 steinbock-0.9.1/steinbock/_cli/apps.py
+-rw-r--r--   0 runner    (1001) docker     (121)      325 2021-10-12 13:28:40.000000 steinbock-0.9.1/steinbock/_cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2868 2021-10-12 13:28:40.000000 steinbock-0.9.1/steinbock/_env.py
+-rw-r--r--   0 runner    (1001) docker     (121)      142 2021-10-12 13:28:51.000000 steinbock-0.9.1/steinbock/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-12 13:28:51.145100 steinbock-0.9.1/steinbock/classification/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-12 13:28:40.000000 steinbock-0.9.1/steinbock/classification/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-12 13:28:51.145100 steinbock-0.9.1/steinbock/classification/_cli/
+-rw-r--r--   0 runner    (1001) docker     (121)      352 2021-10-12 13:28:40.000000 steinbock-0.9.1/steinbock/classification/_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9458 2021-10-12 13:28:40.000000 steinbock-0.9.1/steinbock/classification/_cli/ilastik.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-12 13:28:51.145100 steinbock-0.9.1/steinbock/classification/ilastik/
+-rw-r--r--   0 runner    (1001) docker     (121)      959 2021-10-12 13:28:40.000000 steinbock-0.9.1/steinbock/classification/ilastik/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21211 2021-10-12 13:28:40.000000 steinbock-0.9.1/steinbock/classification/ilastik/_ilastik.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-12 13:28:51.145100 steinbock-0.9.1/steinbock/classification/ilastik/data/
+-rw-r--r--   0 runner    (1001) docker     (121)  1108944 2021-10-12 13:28:40.000000 steinbock-0.9.1/steinbock/classification/ilastik/data/pixel_classifier.ilp
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-12 13:28:51.145100 steinbock-0.9.1/steinbock/export/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-12 13:28:40.000000 steinbock-0.9.1/steinbock/export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9540 2021-10-12 13:28:40.000000 steinbock-0.9.1/steinbock/export/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1858 2021-10-12 13:28:40.000000 steinbock-0.9.1/steinbock/export/data.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1939 2021-10-12 13:28:40.000000 steinbock-0.9.1/steinbock/export/graphs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9059 2021-10-12 13:28:40.000000 steinbock-0.9.1/steinbock/io.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-12 13:28:51.145100 steinbock-0.9.1/steinbock/measurement/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-12 13:28:40.000000 steinbock-0.9.1/steinbock/measurement/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-12 13:28:51.145100 steinbock-0.9.1/steinbock/measurement/_cli/
+-rw-r--r--   0 runner    (1001) docker     (121)      685 2021-10-12 13:28:40.000000 steinbock-0.9.1/steinbock/measurement/_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3382 2021-10-12 13:28:40.000000 steinbock-0.9.1/steinbock/measurement/_cli/cellprofiler.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2371 2021-10-12 13:28:40.000000 steinbock-0.9.1/steinbock/measurement/_cli/intensities.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2048 2021-10-12 13:28:40.000000 steinbock-0.9.1/steinbock/measurement/_cli/neighbors.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1715 2021-10-12 13:28:40.000000 steinbock-0.9.1/steinbock/measurement/_cli/regionprops.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-12 13:28:51.145100 steinbock-0.9.1/steinbock/measurement/cellprofiler/
+-rw-r--r--   0 runner    (1001) docker     (121)      207 2021-10-12 13:28:40.000000 steinbock-0.9.1/steinbock/measurement/cellprofiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1190 2021-10-12 13:28:40.000000 steinbock-0.9.1/steinbock/measurement/cellprofiler/_cellprofiler.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-12 13:28:51.145100 steinbock-0.9.1/steinbock/measurement/cellprofiler/data/
+-rw-r--r--   0 runner    (1001) docker     (121)     6801 2021-10-12 13:28:40.000000 steinbock-0.9.1/steinbock/measurement/cellprofiler/data/cell_measurement.cppipe
+-rw-r--r--   0 runner    (1001) docker     (121)     1927 2021-10-12 13:28:40.000000 steinbock-0.9.1/steinbock/measurement/intensities.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7149 2021-10-12 13:28:40.000000 steinbock-0.9.1/steinbock/measurement/neighbors.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1499 2021-10-12 13:28:40.000000 steinbock-0.9.1/steinbock/measurement/regionprops.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-12 13:28:51.149100 steinbock-0.9.1/steinbock/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-12 13:28:40.000000 steinbock-0.9.1/steinbock/preprocessing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-12 13:28:51.149100 steinbock-0.9.1/steinbock/preprocessing/_cli/
+-rw-r--r--   0 runner    (1001) docker     (121)      380 2021-10-12 13:28:40.000000 steinbock-0.9.1/steinbock/preprocessing/_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7259 2021-10-12 13:28:40.000000 steinbock-0.9.1/steinbock/preprocessing/_cli/imc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9000 2021-10-12 13:28:40.000000 steinbock-0.9.1/steinbock/preprocessing/imc.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-12 13:28:51.149100 steinbock-0.9.1/steinbock/segmentation/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-12 13:28:40.000000 steinbock-0.9.1/steinbock/segmentation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-12 13:28:51.149100 steinbock-0.9.1/steinbock/segmentation/_cli/
+-rw-r--r--   0 runner    (1001) docker     (121)      532 2021-10-12 13:28:40.000000 steinbock-0.9.1/steinbock/segmentation/_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2346 2021-10-12 13:28:40.000000 steinbock-0.9.1/steinbock/segmentation/_cli/cellprofiler.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4760 2021-10-12 13:28:40.000000 steinbock-0.9.1/steinbock/segmentation/_cli/deepcell.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-12 13:28:51.149100 steinbock-0.9.1/steinbock/segmentation/cellprofiler/
+-rw-r--r--   0 runner    (1001) docker     (121)      210 2021-10-12 13:28:40.000000 steinbock-0.9.1/steinbock/segmentation/cellprofiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1101 2021-10-12 13:28:40.000000 steinbock-0.9.1/steinbock/segmentation/cellprofiler/_cellprofiler.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-12 13:28:51.149100 steinbock-0.9.1/steinbock/segmentation/cellprofiler/data/
+-rw-r--r--   0 runner    (1001) docker     (121)    10832 2021-10-12 13:28:40.000000 steinbock-0.9.1/steinbock/segmentation/cellprofiler/data/cell_segmentation.cppipe
+-rw-r--r--   0 runner    (1001) docker     (121)     3273 2021-10-12 13:28:40.000000 steinbock-0.9.1/steinbock/segmentation/deepcell.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-12 13:28:51.149100 steinbock-0.9.1/steinbock/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-12 13:28:40.000000 steinbock-0.9.1/steinbock/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-12 13:28:51.149100 steinbock-0.9.1/steinbock/utils/_cli/
+-rw-r--r--   0 runner    (1001) docker     (121)     1620 2021-10-12 13:28:40.000000 steinbock-0.9.1/steinbock/utils/_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2726 2021-10-12 13:28:40.000000 steinbock-0.9.1/steinbock/utils/_cli/mosaics.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1476 2021-10-12 13:28:40.000000 steinbock-0.9.1/steinbock/utils/matching.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2372 2021-10-12 13:28:40.000000 steinbock-0.9.1/steinbock/utils/mosaics.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-12 13:28:51.141100 steinbock-0.9.1/steinbock.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2332 2021-10-12 13:28:51.000000 steinbock-0.9.1/steinbock.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3657 2021-10-12 13:28:51.000000 steinbock-0.9.1/steinbock.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-12 13:28:51.000000 steinbock-0.9.1/steinbock.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       66 2021-10-12 13:28:51.000000 steinbock-0.9.1/steinbock.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-12 13:28:50.000000 steinbock-0.9.1/steinbock.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      151 2021-10-12 13:28:51.000000 steinbock-0.9.1/steinbock.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       10 2021-10-12 13:28:51.000000 steinbock-0.9.1/steinbock.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-12 13:28:51.149100 steinbock-0.9.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-12 13:28:51.149100 steinbock-0.9.1/tests/classification/
+-rw-r--r--   0 runner    (1001) docker     (121)     5986 2021-10-12 13:28:40.000000 steinbock-0.9.1/tests/classification/test_ilastik_classification.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-12 13:28:51.149100 steinbock-0.9.1/tests/export/
+-rw-r--r--   0 runner    (1001) docker     (121)     1184 2021-10-12 13:28:40.000000 steinbock-0.9.1/tests/export/test_data_export.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1392 2021-10-12 13:28:40.000000 steinbock-0.9.1/tests/export/test_graphs_export.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-12 13:28:51.149100 steinbock-0.9.1/tests/measurement/
+-rw-r--r--   0 runner    (1001) docker     (121)     1042 2021-10-12 13:28:40.000000 steinbock-0.9.1/tests/measurement/test_cellprofiler_measurement.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1830 2021-10-12 13:28:40.000000 steinbock-0.9.1/tests/measurement/test_intensities_measurement.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1888 2021-10-12 13:28:40.000000 steinbock-0.9.1/tests/measurement/test_neighbors_measurement.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1310 2021-10-12 13:28:40.000000 steinbock-0.9.1/tests/measurement/test_regionprops_measurement.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-12 13:28:51.149100 steinbock-0.9.1/tests/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (121)     3184 2021-10-12 13:28:40.000000 steinbock-0.9.1/tests/preprocessing/test_imc_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (121)       49 2021-10-12 13:28:40.000000 steinbock-0.9.1/tests/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-12 13:28:51.149100 steinbock-0.9.1/tests/segmentation/
+-rw-r--r--   0 runner    (1001) docker     (121)     1034 2021-10-12 13:28:40.000000 steinbock-0.9.1/tests/segmentation/test_cellprofiler_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1171 2021-10-12 13:28:40.000000 steinbock-0.9.1/tests/segmentation/test_deepcell_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2428 2021-10-12 13:28:40.000000 steinbock-0.9.1/tests/test_io.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-12 13:28:51.149100 steinbock-0.9.1/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)     1050 2021-10-12 13:28:40.000000 steinbock-0.9.1/tests/utils/test_matching_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1218 2021-10-12 13:28:40.000000 steinbock-0.9.1/tests/utils/test_mosaics_utils.py
```

### Comparing `steinbock-0.9.0/.dockerignore` & `steinbock-0.9.1/.dockerignore`

 * *Files identical despite different names*

### Comparing `steinbock-0.9.0/.github/workflows/build.yml` & `steinbock-0.9.1/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `steinbock-0.9.0/.github/workflows/docs.yml` & `steinbock-0.9.1/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `steinbock-0.9.0/.gitignore` & `steinbock-0.9.1/.gitignore`

 * *Files identical despite different names*

### Comparing `steinbock-0.9.0/.vscode/launch.json` & `steinbock-0.9.1/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `steinbock-0.9.0/.vscode/tasks.json` & `steinbock-0.9.1/.vscode/tasks.json`

 * *Files identical despite different names*

### Comparing `steinbock-0.9.0/CHANGELOG.md` & `steinbock-0.9.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,19 @@
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 
+## [0.9.1] - 2021-10-12
+
+  - Fixed preprocessing of IMC Segmentation Pipeline panels
+
+
 ## [0.9.0] - 2021-10-11
 
   - Upgraded dependencies
   - Improved documentation
   - Reduced Docker image size
   - Replaced imctools with readimc
   - Added dockerized unit tests (w.i.p.)
@@ -208,14 +213,15 @@
 
 
 ## [0.1.0] - 2021-04-08
 
 Initial release for beta testing
 
 
+[0.9.1]: https://github.com/BodenmillerGroup/steinbock/compare/v0.9.0...v0.9.1
 [0.9.0]: https://github.com/BodenmillerGroup/steinbock/compare/v0.8.1...v0.9.0
 [0.8.1]: https://github.com/BodenmillerGroup/steinbock/compare/v0.8.0...v0.8.1
 [0.8.0]: https://github.com/BodenmillerGroup/steinbock/compare/v0.7.3...v0.8.0
 [0.7.3]: https://github.com/BodenmillerGroup/steinbock/compare/v0.7.2...v0.7.3
 [0.7.2]: https://github.com/BodenmillerGroup/steinbock/compare/v0.7.1...v0.7.2
 [0.7.1]: https://github.com/BodenmillerGroup/steinbock/compare/v0.7.0...v0.7.1
 [0.7.0]: https://github.com/BodenmillerGroup/steinbock/compare/v0.6.2...v0.7.0
```

### Comparing `steinbock-0.9.0/CONTRIBUTING.md` & `steinbock-0.9.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `steinbock-0.9.0/Dockerfile` & `steinbock-0.9.1/Dockerfile`

 * *Files identical despite different names*

### Comparing `steinbock-0.9.0/LICENSE` & `steinbock-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `steinbock-0.9.0/PKG-INFO` & `steinbock-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: steinbock
-Version: 0.9.0
+Version: 0.9.1
 Summary: Dockerized multi-channel image processing framework
 Home-page: https://github.com/BodenmillerGroup/steinbock
 Author: Jonas Windhager
 Author-email: jonas.windhager@uzh.ch
 License: MIT
 Keywords: Fluidigm,Imaging Mass Cytometry,IMC
 Platform: UNKNOWN
@@ -16,15 +16,15 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: imc
 Provides-Extra: deepcell
 Provides-Extra: all
 License-File: LICENSE
 
-<img src="docs/img/steinbock-logo.png" align="right" alt="Logo" width="150" />
+<img src="https://raw.githubusercontent.com/BodenmillerGroup/steinbock/main/docs/img/steinbock-logo.png" align="right" alt="Logo" width="150" />
 
 # steinbock
 
 <a href="https://python.org"><img alt="Python" src="https://img.shields.io/pypi/pyversions/steinbock"></a>
 <a href="https://github.com/BodenmillerGroup/steinbock/pkgs/container/steinbock" alt="Build"><img alt="Build" src="https://img.shields.io/github/workflow/status/BodenmillerGroup/steinbock/build?label=build"></a>
 <a href="https://pypi.org/project/steinbock" alt="PyPI"><img alt="PyPI" src="https://img.shields.io/pypi/v/steinbock"></a>
 <a href="https://codecov.io/gh/BodenmillerGroup/steinbock"><img alt="Coverage" src="https://img.shields.io/codecov/c/github/BodenmillerGroup/steinbock"></a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: steinbock Version: 0.9.0 Summary: Dockerized multi-
+Metadata-Version: 2.1 Name: steinbock Version: 0.9.1 Summary: Dockerized multi-
 channel image processing framework Home-page: https://github.com/
 BodenmillerGroup/steinbock Author: Jonas Windhager Author-email:
 jonas.windhager@uzh.ch License: MIT Keywords: Fluidigm,Imaging Mass
 Cytometry,IMC Platform: UNKNOWN Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License Requires-Python: >=3.8
```

### Comparing `steinbock-0.9.0/README.md` & `steinbock-0.9.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<img src="docs/img/steinbock-logo.png" align="right" alt="Logo" width="150" />
+<img src="https://raw.githubusercontent.com/BodenmillerGroup/steinbock/main/docs/img/steinbock-logo.png" align="right" alt="Logo" width="150" />
 
 # steinbock
 
 <a href="https://python.org"><img alt="Python" src="https://img.shields.io/pypi/pyversions/steinbock"></a>
 <a href="https://github.com/BodenmillerGroup/steinbock/pkgs/container/steinbock" alt="Build"><img alt="Build" src="https://img.shields.io/github/workflow/status/BodenmillerGroup/steinbock/build?label=build"></a>
 <a href="https://pypi.org/project/steinbock" alt="PyPI"><img alt="PyPI" src="https://img.shields.io/pypi/v/steinbock"></a>
 <a href="https://codecov.io/gh/BodenmillerGroup/steinbock"><img alt="Coverage" src="https://img.shields.io/codecov/c/github/BodenmillerGroup/steinbock"></a>
```

### Comparing `steinbock-0.9.0/conftest.py` & `steinbock-0.9.1/conftest.py`

 * *Files identical despite different names*

### Comparing `steinbock-0.9.0/docker-compose.yml` & `steinbock-0.9.1/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `steinbock-0.9.0/docs/changelog.md` & `steinbock-0.9.1/docs/changelog.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,19 @@
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 
+## [0.9.1] - 2021-10-12
+
+  - Fixed preprocessing of IMC Segmentation Pipeline panels
+
+
 ## [0.9.0] - 2021-10-11
 
   - Upgraded dependencies
   - Improved documentation
   - Reduced Docker image size
   - Replaced imctools with readimc
   - Added dockerized unit tests (w.i.p.)
@@ -208,14 +213,15 @@
 
 
 ## [0.1.0] - 2021-04-08
 
 Initial release for beta testing
 
 
+[0.9.1]: https://github.com/BodenmillerGroup/steinbock/compare/v0.9.0...v0.9.1
 [0.9.0]: https://github.com/BodenmillerGroup/steinbock/compare/v0.8.1...v0.9.0
 [0.8.1]: https://github.com/BodenmillerGroup/steinbock/compare/v0.8.0...v0.8.1
 [0.8.0]: https://github.com/BodenmillerGroup/steinbock/compare/v0.7.3...v0.8.0
 [0.7.3]: https://github.com/BodenmillerGroup/steinbock/compare/v0.7.2...v0.7.3
 [0.7.2]: https://github.com/BodenmillerGroup/steinbock/compare/v0.7.1...v0.7.2
 [0.7.1]: https://github.com/BodenmillerGroup/steinbock/compare/v0.7.0...v0.7.1
 [0.7.0]: https://github.com/BodenmillerGroup/steinbock/compare/v0.6.2...v0.7.0
```

### Comparing `steinbock-0.9.0/docs/cli/apps.md` & `steinbock-0.9.1/docs/cli/apps.md`

 * *Files identical despite different names*

### Comparing `steinbock-0.9.0/docs/cli/classification.md` & `steinbock-0.9.1/docs/cli/classification.md`

 * *Files identical despite different names*

### Comparing `steinbock-0.9.0/docs/cli/export.md` & `steinbock-0.9.1/docs/cli/export.md`

 * *Files identical despite different names*

### Comparing `steinbock-0.9.0/docs/cli/intro.md` & `steinbock-0.9.1/docs/cli/intro.md`

 * *Files identical despite different names*

### Comparing `steinbock-0.9.0/docs/cli/measurement.md` & `steinbock-0.9.1/docs/cli/measurement.md`

 * *Files identical despite different names*

### Comparing `steinbock-0.9.0/docs/cli/preprocessing.md` & `steinbock-0.9.1/docs/cli/preprocessing.md`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
 ### Image conversion
 
 To convert .mcd/.txt files in the raw data directory to TIFF and filter hot pixels:
 
     steinbock preprocess imc images --hpf 50
 
-This will extract images from .mcd files at the specified location (defaults to `raw`). Each image corresponds to one acquisition in one file, with the image channels filtered and sorted according to the *steinbock* panel file at the specified location (defaults to `panel.csv`). For corrupted .mcd files, *steinbock* will try to recover the missing acquisitions from matching .txt files. In a second step, images from *unmatched* .txt files are extracted as well.
+This will extract images from raw files (source directory defaults to `raw`) and save them at the specified location (defaults to `img`). Each image corresponds to one acquisition in one file, with the image channels filtered and sorted according to the *steinbock* panel file at the specified location (defaults to `panel.csv`). For corrupted .mcd files, *steinbock* will try to recover the missing acquisitions from matching .txt files. In a second step, images from *unmatched* .txt files are extracted as well.
 
 Furthermore, this commands also creates an image information table as described in [File types](../file-types.md#image-information). In addition to the default columns, the following IMC-specific columns will be added:
 
   - `source`: the raw .mcd/.txt file name
   - `recovered`: *True* if the .mcd acquisition was recovered from the corresponding .txt file
   - Acquisition-specific information: 
     - `acquisition_id`: numeric acquisition ID
```

### Comparing `steinbock-0.9.0/docs/cli/segmentation.md` & `steinbock-0.9.1/docs/cli/segmentation.md`

 * *Files identical despite different names*

### Comparing `steinbock-0.9.0/docs/cli/utils.md` & `steinbock-0.9.1/docs/cli/utils.md`

 * *Files identical despite different names*

### Comparing `steinbock-0.9.0/docs/contributing.md` & `steinbock-0.9.1/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `steinbock-0.9.0/docs/directories.md` & `steinbock-0.9.1/docs/directories.md`

 * *Files identical despite different names*

### Comparing `steinbock-0.9.0/docs/docker.md` & `steinbock-0.9.1/docs/docker.md`

 * *Files 5% similar despite different names*

```diff
@@ -27,64 +27,64 @@
 
 In principle, the *steinbock* Docker container can be run on any Docker-enabled platform:
 
     docker run ghcr.io/bodenmillergroup/steinbock
 
 For reproducibility, it is recommended to always pull a specific release, e.g.:
 
-    docker run ghcr.io/bodenmillergroup/steinbock:0.9.0
+    docker run ghcr.io/bodenmillergroup/steinbock:0.9.1
 
 [Bind mounts](https://docs.docker.com/storage/bind-mounts/) can be used to make data from the host system available to the Docker container (see below). Commands that launch a graphical user interface may require further system configuration and additional arguments to `docker run` as outlined in the following.
 
 
 ### Windows
 
 On the command line, use the following command to run the *steinbock* Docker container:
 
-    docker run -v "C:\Data":/data ghcr.io/bodenmillergroup/steinbock:0.9.0
+    docker run -v "C:\Data":/data ghcr.io/bodenmillergroup/steinbock:0.9.1
 
-In the command above, adapt the bind mount path to your data/working directory (`C:\Data`) and the *steinbock* Docker container version (`0.9.0`) as needed. To simplify the use of the *steinbock* command-line interface, it is recommended to set up a `steinbock` command alias:
+In the command above, adapt the bind mount path to your data/working directory (`C:\Data`) and the *steinbock* Docker container version (`0.9.1`) as needed. To simplify the use of the *steinbock* command-line interface, it is recommended to set up a `steinbock` command alias:
 
-    doskey steinbock=docker run -v "C:\Data":/data ghcr.io/bodenmillergroup/steinbock:0.9.0 $*
+    doskey steinbock=docker run -v "C:\Data":/data ghcr.io/bodenmillergroup/steinbock:0.9.1 $*
 
 The created command alias is retained for the current session and enables running `steinbock` from the current command line without typing the full Docker command, for example:
 
     steinbock --version
 
 !!! note "Graphical user interfaces on Windows hosts"
     Commands that launch a graphical user interface (e.g. for Ilastik, CellProfiler) will not work on Windows hosts. It is recommended to run these programs directly on the Windows host, if graphical user interfaces are required. For compatibility, versions of third-party applications can be found in the [*steinbock* Dockerfile](https://github.com/BodenmillerGroup/steinbock/blob/main/Dockerfile).
 
 ### Linux
 
 On the terminal, use the following command to run the *steinbock* Docker container:
 
-    docker run -v /path/to/data:/data -v /tmp/.X11-unix:/tmp/.X11-unix -v ~/.Xauthority:/home/steinbock/.Xauthority:ro -u $(id -u):$(id -g) -e DISPLAY ghcr.io/bodenmillergroup/steinbock:0.9.0
+    docker run -v /path/to/data:/data -v /tmp/.X11-unix:/tmp/.X11-unix -v ~/.Xauthority:/home/steinbock/.Xauthority:ro -u $(id -u):$(id -g) -e DISPLAY ghcr.io/bodenmillergroup/steinbock:0.9.1
 
-In the command above, adapt the bind mount path to your data/working directory (`/path/to/data`) and the *steinbock* Docker container version (`0.9.0`) as needed. To simplify the use of the *steinbock* command-line interface, it is recommended to set up a `steinbock` command alias:
+In the command above, adapt the bind mount path to your data/working directory (`/path/to/data`) and the *steinbock* Docker container version (`0.9.1`) as needed. To simplify the use of the *steinbock* command-line interface, it is recommended to set up a `steinbock` command alias:
 
-    alias steinbock="docker run -v /path/to/data:/data -v /tmp/.X11-unix:/tmp/.X11-unix -v ~/.Xauthority:/home/steinbock/.Xauthority:ro -u $(id -u):$(id -g) -e DISPLAY ghcr.io/bodenmillergroup/steinbock:0.9.0"
+    alias steinbock="docker run -v /path/to/data:/data -v /tmp/.X11-unix:/tmp/.X11-unix -v ~/.Xauthority:/home/steinbock/.Xauthority:ro -u $(id -u):$(id -g) -e DISPLAY ghcr.io/bodenmillergroup/steinbock:0.9.1"
 
 The created command alias is retained for the current session and enables running `steinbock` from the current terminal without typing the full Docker command, for example:
 
     steinbock --version
 
 !!! note "Graphical user interfaces on Linux hosts"
     To allow the *steinbock* Docker container to run graphical user interfaces, if necessary, allow the local root user (i.e., the user running the Docker daemon) to access the running X server:
 
         xhost +local:root
 
 ### MacOS
 
 On the terminal, use the following command to run the *steinbock* Docker container (Docker must be running):
 
-    docker run -v /path/to/data:/data -v /tmp/.X11-unix:/tmp/.X11-unix -v ~/.Xauthority:/home/steinbock/.Xauthority:ro -u $(id -u):$(id -g) -e DISPLAY=$(hostname):0 ghcr.io/bodenmillergroup/steinbock:0.9.0
+    docker run -v /path/to/data:/data -v /tmp/.X11-unix:/tmp/.X11-unix -v ~/.Xauthority:/home/steinbock/.Xauthority:ro -u $(id -u):$(id -g) -e DISPLAY=$(hostname):0 ghcr.io/bodenmillergroup/steinbock:0.9.1
 
-In the command above, adapt the bind mount path to your data/working directory (`/path/to/data`) and the *steinbock* Docker container version (`0.9.0`) as needed. To simplify the use of the *steinbock* command-line interface, it is recommended to set up a `steinbock` command alias:
+In the command above, adapt the bind mount path to your data/working directory (`/path/to/data`) and the *steinbock* Docker container version (`0.9.1`) as needed. To simplify the use of the *steinbock* command-line interface, it is recommended to set up a `steinbock` command alias:
 
-    alias steinbock="docker run -v /path/to/data:/data -v /tmp/.X11-unix:/tmp/.X11-unix -v ~/.Xauthority:/home/steinbock/.Xauthority:ro -u $(id -u):$(id -g) -e DISPLAY=$(hostname):0 ghcr.io/bodenmillergroup/steinbock:0.9.0"
+    alias steinbock="docker run -v /path/to/data:/data -v /tmp/.X11-unix:/tmp/.X11-unix -v ~/.Xauthority:/home/steinbock/.Xauthority:ro -u $(id -u):$(id -g) -e DISPLAY=$(hostname):0 ghcr.io/bodenmillergroup/steinbock:0.9.1"
 
 The created command alias is retained for the current session and enables running `steinbock` from the current terminal without typing the full Docker command, for example:
 
     steinbock --version
 
 !!! note "Graphical user interfaces on MacOS hosts"
     To allow the *steinbock* Docker container to run graphical user interfaces, first install and start [XQuartz](https://www.xquartz.org/). Then, open *XQuartz* > *Security* > *Preferences* and tick *Allow connections from network clients*. Log out of your user account and login again; restart Docker and XQuartz. Finally, to allow the local root user (i.e., the user running the Docker daemon) to access the running XQuartz X server:
```

### Comparing `steinbock-0.9.0/docs/file-types.md` & `steinbock-0.9.1/docs/file-types.md`

 * *Files identical despite different names*

### Comparing `steinbock-0.9.0/docs/img/steinbock-logo.png` & `steinbock-0.9.1/docs/img/steinbock-logo.png`

 * *Files identical despite different names*

### Comparing `steinbock-0.9.0/docs/index.md` & `steinbock-0.9.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `steinbock-0.9.0/docs/python.md` & `steinbock-0.9.1/docs/python.md`

 * *Files identical despite different names*

### Comparing `steinbock-0.9.0/mkdocs.yml` & `steinbock-0.9.1/mkdocs.yml`

 * *Files 6% similar despite different names*

```diff
@@ -14,25 +14,27 @@
   - mike:
       version_selector: true
 markdown_extensions:
   - admonition
   - footnotes
 theme:
   name: material
+  logo: img/steinbock-logo-white.png
+  favicon: img/steinbock-favicon.png
   features:
     - navigation.tabs
     - navigation.top
 extra:
   version:
     provider: mike
 extra_css:
   - mkdocstrings.css
 nav:
   - Home:
-    - index.md
+    - Welcome: index.md
     - Installation:
       - docker.md
       - python.md
     - Specifications:
       - file-types.md
       - directories.md
     - Development:
```

### Comparing `steinbock-0.9.0/setup.cfg` & `steinbock-0.9.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `steinbock-0.9.0/steinbock/_cli/__init__.py` & `steinbock-0.9.1/steinbock/_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `steinbock-0.9.0/steinbock/_cli/apps.py` & `steinbock-0.9.1/steinbock/_cli/apps.py`

 * *Files identical despite different names*

### Comparing `steinbock-0.9.0/steinbock/_env.py` & `steinbock-0.9.1/steinbock/_env.py`

 * *Files identical despite different names*

### Comparing `steinbock-0.9.0/steinbock/classification/_cli/ilastik.py` & `steinbock-0.9.1/steinbock/classification/_cli/ilastik.py`

 * *Files identical despite different names*

### Comparing `steinbock-0.9.0/steinbock/classification/ilastik/__init__.py` & `steinbock-0.9.1/steinbock/classification/ilastik/__init__.py`

 * *Files identical despite different names*

### Comparing `steinbock-0.9.0/steinbock/classification/ilastik/_ilastik.py` & `steinbock-0.9.1/steinbock/classification/ilastik/_ilastik.py`

 * *Files identical despite different names*

### Comparing `steinbock-0.9.0/steinbock/classification/ilastik/data/pixel_classifier.ilp` & `steinbock-0.9.1/steinbock/classification/ilastik/data/pixel_classifier.ilp`

 * *Files identical despite different names*

### Comparing `steinbock-0.9.0/steinbock/export/_cli.py` & `steinbock-0.9.1/steinbock/export/_cli.py`

 * *Files identical despite different names*

### Comparing `steinbock-0.9.0/steinbock/export/data.py` & `steinbock-0.9.1/steinbock/export/data.py`

 * *Files identical despite different names*

### Comparing `steinbock-0.9.0/steinbock/export/graphs.py` & `steinbock-0.9.1/steinbock/export/graphs.py`

 * *Files identical despite different names*

### Comparing `steinbock-0.9.0/steinbock/io.py` & `steinbock-0.9.1/steinbock/io.py`

 * *Files identical despite different names*

### Comparing `steinbock-0.9.0/steinbock/measurement/_cli/__init__.py` & `steinbock-0.9.1/steinbock/measurement/_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `steinbock-0.9.0/steinbock/measurement/_cli/cellprofiler.py` & `steinbock-0.9.1/steinbock/measurement/_cli/cellprofiler.py`

 * *Files identical despite different names*

### Comparing `steinbock-0.9.0/steinbock/measurement/_cli/intensities.py` & `steinbock-0.9.1/steinbock/measurement/_cli/intensities.py`

 * *Files identical despite different names*

### Comparing `steinbock-0.9.0/steinbock/measurement/_cli/neighbors.py` & `steinbock-0.9.1/steinbock/measurement/_cli/neighbors.py`

 * *Files identical despite different names*

### Comparing `steinbock-0.9.0/steinbock/measurement/_cli/regionprops.py` & `steinbock-0.9.1/steinbock/measurement/_cli/regionprops.py`

 * *Files identical despite different names*

### Comparing `steinbock-0.9.0/steinbock/measurement/cellprofiler/_cellprofiler.py` & `steinbock-0.9.1/steinbock/measurement/cellprofiler/_cellprofiler.py`

 * *Files identical despite different names*

### Comparing `steinbock-0.9.0/steinbock/measurement/cellprofiler/data/cell_measurement.cppipe` & `steinbock-0.9.1/steinbock/measurement/cellprofiler/data/cell_measurement.cppipe`

 * *Files identical despite different names*

### Comparing `steinbock-0.9.0/steinbock/measurement/intensities.py` & `steinbock-0.9.1/steinbock/measurement/intensities.py`

 * *Files identical despite different names*

### Comparing `steinbock-0.9.0/steinbock/measurement/neighbors.py` & `steinbock-0.9.1/steinbock/measurement/neighbors.py`

 * *Files identical despite different names*

### Comparing `steinbock-0.9.0/steinbock/measurement/regionprops.py` & `steinbock-0.9.1/steinbock/measurement/regionprops.py`

 * *Files identical despite different names*

### Comparing `steinbock-0.9.0/steinbock/preprocessing/_cli/imc.py` & `steinbock-0.9.1/steinbock/preprocessing/_cli/imc.py`

 * *Files identical despite different names*

### Comparing `steinbock-0.9.0/steinbock/preprocessing/imc.py` & `steinbock-0.9.1/steinbock/preprocessing/imc.py`

 * *Files 10% similar despite different names*

```diff
@@ -65,39 +65,46 @@
         _imc_panel_metal_col,
         _imc_panel_keep_col,
         _imc_panel_ilastik_col,
         _imc_panel_deepcell_col,
     ):
         if notnan_col in imc_panel and imc_panel[notnan_col].isna().any():
             raise ValueError(f"Missing values for '{notnan_col}' in IMC panel")
-    panel = imc_panel.rename(
-        columns={
-            _imc_panel_metal_col: "channel",
-            _imc_panel_target_col: "name",
-            _imc_panel_keep_col: "keep",
-            _imc_panel_ilastik_col: "ilastik",
-            _imc_panel_deepcell_col: "deepcell",
-        }
-    )
+    rename_columns = {
+        _imc_panel_metal_col: "channel",
+        _imc_panel_target_col: "name",
+        _imc_panel_keep_col: "keep",
+        _imc_panel_ilastik_col: "ilastik",
+        _imc_panel_deepcell_col: "deepcell",
+    }
+    drop_columns = [
+        panel_col
+        for imc_panel_col, panel_col in rename_columns.items()
+        if panel_col in imc_panel.columns and panel_col != imc_panel_col
+    ]
+    panel = imc_panel.drop(columns=drop_columns).rename(columns=rename_columns)
     for _, group in panel.groupby("channel"):
-        panel.loc[group.index, "name"] = "/".join(
+        panel.loc[group.index, "name"] = " / ".join(
             group["name"].dropna().unique()
         )
         if "keep" in panel:
             panel.loc[group.index, "keep"] = group["keep"].any()
         if "ilastik" in panel:
             panel.loc[group.index, "ilastik"] = group["ilastik"].any()
         if "deepcell" in panel:
             panel.loc[group.index, "deepcell"] = group["deepcell"].any()
     panel = panel.groupby(panel["channel"].values).aggregate("first")
     panel.sort_values(
         "channel",
         key=lambda s: pd.to_numeric(s.str.replace("[^0-9]", "", regex=True)),
         inplace=True,
     )
+    duplicated_mask = panel["name"].duplicated(keep=False)
+    name_suffixes = panel.groupby("name").cumcount().map(lambda i: f" {i + 1}")
+    panel.loc[duplicated_mask, "name"] += name_suffixes[duplicated_mask]
     if "keep" not in panel:
         panel["keep"] = pd.Series(True, dtype=pd.BooleanDtype())
     if "ilastik" in panel:
         ilastik_mask = panel["ilastik"].astype(bool)
         panel["ilastik"] = pd.Series(dtype=pd.UInt8Dtype())
         panel.loc[ilastik_mask, "ilastik"] = range(1, ilastik_mask.sum() + 1)
     else:
```

### Comparing `steinbock-0.9.0/steinbock/segmentation/_cli/__init__.py` & `steinbock-0.9.1/steinbock/segmentation/_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `steinbock-0.9.0/steinbock/segmentation/_cli/cellprofiler.py` & `steinbock-0.9.1/steinbock/segmentation/_cli/cellprofiler.py`

 * *Files identical despite different names*

### Comparing `steinbock-0.9.0/steinbock/segmentation/_cli/deepcell.py` & `steinbock-0.9.1/steinbock/segmentation/_cli/deepcell.py`

 * *Files identical despite different names*

### Comparing `steinbock-0.9.0/steinbock/segmentation/cellprofiler/_cellprofiler.py` & `steinbock-0.9.1/steinbock/segmentation/cellprofiler/_cellprofiler.py`

 * *Files identical despite different names*

### Comparing `steinbock-0.9.0/steinbock/segmentation/cellprofiler/data/cell_segmentation.cppipe` & `steinbock-0.9.1/steinbock/segmentation/cellprofiler/data/cell_segmentation.cppipe`

 * *Files identical despite different names*

### Comparing `steinbock-0.9.0/steinbock/segmentation/deepcell.py` & `steinbock-0.9.1/steinbock/segmentation/deepcell.py`

 * *Files identical despite different names*

### Comparing `steinbock-0.9.0/steinbock/utils/_cli/__init__.py` & `steinbock-0.9.1/steinbock/utils/_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `steinbock-0.9.0/steinbock/utils/_cli/mosaics.py` & `steinbock-0.9.1/steinbock/utils/_cli/mosaics.py`

 * *Files identical despite different names*

### Comparing `steinbock-0.9.0/steinbock/utils/matching.py` & `steinbock-0.9.1/steinbock/utils/matching.py`

 * *Files identical despite different names*

### Comparing `steinbock-0.9.0/steinbock/utils/mosaics.py` & `steinbock-0.9.1/steinbock/utils/mosaics.py`

 * *Files identical despite different names*

### Comparing `steinbock-0.9.0/steinbock.egg-info/PKG-INFO` & `steinbock-0.9.1/steinbock.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: steinbock
-Version: 0.9.0
+Version: 0.9.1
 Summary: Dockerized multi-channel image processing framework
 Home-page: https://github.com/BodenmillerGroup/steinbock
 Author: Jonas Windhager
 Author-email: jonas.windhager@uzh.ch
 License: MIT
 Keywords: Fluidigm,Imaging Mass Cytometry,IMC
 Platform: UNKNOWN
@@ -16,15 +16,15 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: imc
 Provides-Extra: deepcell
 Provides-Extra: all
 License-File: LICENSE
 
-<img src="docs/img/steinbock-logo.png" align="right" alt="Logo" width="150" />
+<img src="https://raw.githubusercontent.com/BodenmillerGroup/steinbock/main/docs/img/steinbock-logo.png" align="right" alt="Logo" width="150" />
 
 # steinbock
 
 <a href="https://python.org"><img alt="Python" src="https://img.shields.io/pypi/pyversions/steinbock"></a>
 <a href="https://github.com/BodenmillerGroup/steinbock/pkgs/container/steinbock" alt="Build"><img alt="Build" src="https://img.shields.io/github/workflow/status/BodenmillerGroup/steinbock/build?label=build"></a>
 <a href="https://pypi.org/project/steinbock" alt="PyPI"><img alt="PyPI" src="https://img.shields.io/pypi/v/steinbock"></a>
 <a href="https://codecov.io/gh/BodenmillerGroup/steinbock"><img alt="Coverage" src="https://img.shields.io/codecov/c/github/BodenmillerGroup/steinbock"></a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: steinbock Version: 0.9.0 Summary: Dockerized multi-
+Metadata-Version: 2.1 Name: steinbock Version: 0.9.1 Summary: Dockerized multi-
 channel image processing framework Home-page: https://github.com/
 BodenmillerGroup/steinbock Author: Jonas Windhager Author-email:
 jonas.windhager@uzh.ch License: MIT Keywords: Fluidigm,Imaging Mass
 Cytometry,IMC Platform: UNKNOWN Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License Requires-Python: >=3.8
```

### Comparing `steinbock-0.9.0/steinbock.egg-info/SOURCES.txt` & `steinbock-0.9.1/steinbock.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -38,14 +38,16 @@
 docs/cli/classification.md
 docs/cli/export.md
 docs/cli/intro.md
 docs/cli/measurement.md
 docs/cli/preprocessing.md
 docs/cli/segmentation.md
 docs/cli/utils.md
+docs/img/steinbock-favicon.png
+docs/img/steinbock-logo-white.png
 docs/img/steinbock-logo.png
 docs/python/intro.md
 docs/python/api/steinbock.classification.md
 docs/python/api/steinbock.export.md
 docs/python/api/steinbock.io.md
 docs/python/api/steinbock.measurement.md
 docs/python/api/steinbock.preprocessing.md
```

### Comparing `steinbock-0.9.0/tests/classification/test_ilastik_classification.py` & `steinbock-0.9.1/tests/classification/test_ilastik_classification.py`

 * *Files identical despite different names*

### Comparing `steinbock-0.9.0/tests/export/test_data_export.py` & `steinbock-0.9.1/tests/export/test_data_export.py`

 * *Files identical despite different names*

### Comparing `steinbock-0.9.0/tests/export/test_graphs_export.py` & `steinbock-0.9.1/tests/export/test_graphs_export.py`

 * *Files identical despite different names*

### Comparing `steinbock-0.9.0/tests/measurement/test_cellprofiler_measurement.py` & `steinbock-0.9.1/tests/measurement/test_cellprofiler_measurement.py`

 * *Files identical despite different names*

### Comparing `steinbock-0.9.0/tests/measurement/test_intensities_measurement.py` & `steinbock-0.9.1/tests/measurement/test_intensities_measurement.py`

 * *Files identical despite different names*

### Comparing `steinbock-0.9.0/tests/measurement/test_neighbors_measurement.py` & `steinbock-0.9.1/tests/measurement/test_neighbors_measurement.py`

 * *Files identical despite different names*

### Comparing `steinbock-0.9.0/tests/measurement/test_regionprops_measurement.py` & `steinbock-0.9.1/tests/measurement/test_regionprops_measurement.py`

 * *Files identical despite different names*

### Comparing `steinbock-0.9.0/tests/preprocessing/test_imc_preprocessing.py` & `steinbock-0.9.1/tests/preprocessing/test_imc_preprocessing.py`

 * *Files identical despite different names*

### Comparing `steinbock-0.9.0/tests/segmentation/test_cellprofiler_segmentation.py` & `steinbock-0.9.1/tests/segmentation/test_cellprofiler_segmentation.py`

 * *Files identical despite different names*

### Comparing `steinbock-0.9.0/tests/segmentation/test_deepcell_segmentation.py` & `steinbock-0.9.1/tests/segmentation/test_deepcell_segmentation.py`

 * *Files identical despite different names*

### Comparing `steinbock-0.9.0/tests/test_io.py` & `steinbock-0.9.1/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `steinbock-0.9.0/tests/utils/test_matching_utils.py` & `steinbock-0.9.1/tests/utils/test_matching_utils.py`

 * *Files identical despite different names*

### Comparing `steinbock-0.9.0/tests/utils/test_mosaics_utils.py` & `steinbock-0.9.1/tests/utils/test_mosaics_utils.py`

 * *Files identical despite different names*

