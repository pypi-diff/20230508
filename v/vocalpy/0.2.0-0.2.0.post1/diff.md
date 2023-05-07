# Comparing `tmp/vocalpy-0.2.0.tar.gz` & `tmp/vocalpy-0.2.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vocalpy-0.2.0.tar", last modified: Sun May  7 21:52:39 2023, max compression
+gzip compressed data, was "vocalpy-0.2.0.post1.tar", last modified: Sun May  7 22:11:50 2023, max compression
```

## Comparing `vocalpy-0.2.0.tar` & `vocalpy-0.2.0.post1.tar`

### file list

```diff
@@ -1,82 +1,82 @@
--rw-r--r--   0        0        0     1307 2023-05-07 21:41:12.898528 vocalpy-0.2.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      248 2023-05-07 21:39:43.229568 vocalpy-0.2.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      615 2023-05-07 21:39:43.228362 vocalpy-0.2.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      750 2023-05-07 20:16:29.801006 vocalpy-0.2.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0      286 2023-04-25 13:42:56.058591 vocalpy-0.2.0/.gitignore
--rw-r--r--   0        0        0      769 2023-04-25 13:42:56.059258 vocalpy-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      367 2023-05-07 21:38:34.576998 vocalpy-0.2.0/.readthedocs.yaml
--rw-r--r--   0        0        0     5556 2023-05-07 20:52:52.998672 vocalpy-0.2.0/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1867 2023-05-07 20:53:11.404957 vocalpy-0.2.0/CONTRIBUTING.md
--rw-r--r--   0        0        0     1540 2023-04-08 15:55:30.246016 vocalpy-0.2.0/LICENSE
--rw-r--r--   0        0        0     2064 2023-04-08 15:55:30.246197 vocalpy-0.2.0/Makefile
--rw-r--r--   0        0        0     3341 2023-05-07 20:54:49.402519 vocalpy-0.2.0/README.md
--rw-r--r--   0        0        0      251 2023-05-07 20:48:44.343584 vocalpy-0.2.0/docs/CHANGELOG.md
--rw-r--r--   0        0        0    29965 2023-05-07 20:41:50.515176 vocalpy-0.2.0/docs/_static/vocalpy-logomark.png
--rw-r--r--   0        0        0   285798 2023-05-07 20:41:50.763203 vocalpy-0.2.0/docs/_static/vocalpy-primary.png
--rw-r--r--   0        0        0   194159 2023-05-07 20:41:50.588788 vocalpy-0.2.0/docs/_static/vocalpy-secondary.png
--rw-r--r--   0        0        0     6436 2023-05-07 21:36:59.006708 vocalpy-0.2.0/noxfile.py
--rw-r--r--   0        0        0     1447 2023-05-07 21:50:50.220546 vocalpy-0.2.0/pyproject.toml
--rw-r--r--   0        0        0    19133 2023-04-25 13:43:12.342347 vocalpy-0.2.0/src/scripts/attrs-sqlalchemy.ipynb
--rw-r--r--   0        0        0     5151 2023-04-25 13:43:12.360555 vocalpy-0.2.0/src/scripts/carpentries-sql-practice.ipynb
--rw-r--r--   0        0        0    46531 2023-04-25 13:43:12.330739 vocalpy-0.2.0/src/scripts/dataclass-orm.ipynb
--rw-r--r--   0        0        0    21715 2023-04-25 13:43:12.389389 vocalpy-0.2.0/src/scripts/dataset.ipynb
--rw-r--r--   0        0        0     3130 2023-05-04 01:22:37.617838 vocalpy-0.2.0/src/scripts/sqlite-python-tutorial.ipynb
--rw-r--r--   0        0        0    22868 2023-05-07 21:52:26.377951 vocalpy-0.2.0/src/scripts/vocalpy-sqlalchemy-orm.ipynb
--rw-r--r--   0        0        0      804 2023-05-07 21:50:50.216183 vocalpy-0.2.0/src/vocalpy/__about__.py
--rw-r--r--   0        0        0     1304 2023-05-07 21:44:06.314669 vocalpy-0.2.0/src/vocalpy/__init__.py
--rw-r--r--   0        0        0       33 2023-04-25 13:42:56.065849 vocalpy-0.2.0/src/vocalpy/annotation/__init__.py
--rw-r--r--   0        0        0     1895 2023-05-04 01:22:20.075891 vocalpy-0.2.0/src/vocalpy/annotation_file.py
--rw-r--r--   0        0        0        0 2023-05-04 01:22:20.076056 vocalpy-0.2.0/src/vocalpy/annotator.py
--rw-r--r--   0        0        0     7738 2023-05-07 21:44:41.309650 vocalpy-0.2.0/src/vocalpy/audio.py
--rw-r--r--   0        0        0      635 2023-05-04 01:22:20.078518 vocalpy-0.2.0/src/vocalpy/audio_file.py
--rw-r--r--   0        0        0       30 2023-04-25 13:42:56.066572 vocalpy-0.2.0/src/vocalpy/constants.py
--rw-r--r--   0        0        0        0 2023-04-08 15:55:30.247903 vocalpy-0.2.0/src/vocalpy/converters.py
--rw-r--r--   0        0        0     4879 2023-05-04 01:22:20.079083 vocalpy-0.2.0/src/vocalpy/dataset.py
--rw-r--r--   0        0        0     2552 2023-05-07 21:02:40.315808 vocalpy-0.2.0/src/vocalpy/dataset_file.py
--rw-r--r--   0        0        0        0 2023-05-04 01:22:20.079995 vocalpy-0.2.0/src/vocalpy/feature_extractor.py
--rw-r--r--   0        0        0     1918 2023-05-04 01:22:20.080691 vocalpy-0.2.0/src/vocalpy/feature_file.py
--rw-r--r--   0        0        0     1118 2023-04-25 13:42:56.072844 vocalpy-0.2.0/src/vocalpy/paths.py
--rw-r--r--   0        0        0      146 2023-05-07 20:16:29.802759 vocalpy-0.2.0/src/vocalpy/repository/__init__.py
--rw-r--r--   0        0        0      441 2023-05-07 20:16:29.803288 vocalpy-0.2.0/src/vocalpy/repository/base.py
--rw-r--r--   0        0        0     3136 2023-05-04 01:22:20.081989 vocalpy-0.2.0/src/vocalpy/repository/orm.py
--rw-r--r--   0        0        0      677 2023-05-07 20:16:29.803723 vocalpy-0.2.0/src/vocalpy/repository/sqlalchemy.py
--rw-r--r--   0        0        0     3155 2023-05-07 21:44:06.438381 vocalpy-0.2.0/src/vocalpy/segmenter.py
--rw-r--r--   0        0        0     2502 2023-05-07 21:44:06.401117 vocalpy-0.2.0/src/vocalpy/sequence.py
--rw-r--r--   0        0        0      114 2023-05-04 01:22:20.084546 vocalpy-0.2.0/src/vocalpy/signal/__init__.py
--rw-r--r--   0        0        0     2301 2023-05-07 21:45:30.491360 vocalpy-0.2.0/src/vocalpy/signal/audio.py
--rw-r--r--   0        0        0     2244 2023-05-04 01:22:20.085058 vocalpy-0.2.0/src/vocalpy/signal/preprocess.py
--rw-r--r--   0        0        0     3012 2023-05-07 21:45:41.887997 vocalpy-0.2.0/src/vocalpy/signal/segment.py
--rw-r--r--   0        0        0     3062 2023-05-07 21:07:37.895584 vocalpy-0.2.0/src/vocalpy/signal/spectrogram.py
--rw-r--r--   0        0        0     7437 2023-05-04 01:22:20.086913 vocalpy-0.2.0/src/vocalpy/spectrogram.py
--rw-r--r--   0        0        0     1491 2023-05-04 01:22:20.087395 vocalpy-0.2.0/src/vocalpy/spectrogram_file.py
--rw-r--r--   0        0        0     8358 2023-05-07 21:44:06.512977 vocalpy-0.2.0/src/vocalpy/spectrogram_maker.py
--rw-r--r--   0        0        0      508 2023-05-04 01:22:20.088654 vocalpy-0.2.0/src/vocalpy/spectrogram_parameters.py
--rw-r--r--   0        0        0     1565 2023-05-07 21:44:06.416113 vocalpy-0.2.0/src/vocalpy/unit.py
--rw-r--r--   0        0        0      738 2023-04-25 13:42:56.074584 vocalpy-0.2.0/src/vocalpy/validators.py
--rw-r--r--   0        0        0        0 2023-04-08 15:55:30.249971 vocalpy-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0       24 2023-04-08 15:55:30.250132 vocalpy-0.2.0/tests/conftest.py
--rw-r--r--   0        0        0      112 2023-04-25 13:42:56.075165 vocalpy-0.2.0/tests/fixtures/__init__.py
--rw-r--r--   0        0        0     2744 2023-04-25 13:42:56.075834 vocalpy-0.2.0/tests/fixtures/annot.py
--rw-r--r--   0        0        0     4620 2023-04-25 13:42:56.076380 vocalpy-0.2.0/tests/fixtures/audio.py
--rw-r--r--   0        0        0      834 2023-04-25 13:42:56.076724 vocalpy-0.2.0/tests/fixtures/datasets.py
--rw-r--r--   0        0        0     6669 2023-05-04 01:22:20.090376 vocalpy-0.2.0/tests/fixtures/spect.py
--rw-r--r--   0        0        0     1032 2023-04-25 13:42:56.077753 vocalpy-0.2.0/tests/fixtures/test_data.py
--rw-r--r--   0        0        0     2248 2023-04-25 13:42:56.078328 vocalpy-0.2.0/tests/scripts/generate_data_for_tests.py
--rw-r--r--   0        0        0     2695 2023-05-04 01:22:20.090889 vocalpy-0.2.0/tests/test_annotation_file.py
--rw-r--r--   0        0        0     8793 2023-05-07 21:46:44.905812 vocalpy-0.2.0/tests/test_audio.py
--rw-r--r--   0        0        0      992 2023-05-04 01:22:20.091867 vocalpy-0.2.0/tests/test_audio_file.py
--rw-r--r--   0        0        0     1605 2023-05-04 01:22:20.092370 vocalpy-0.2.0/tests/test_dataset.py
--rw-r--r--   0        0        0     2819 2023-05-07 21:46:44.715868 vocalpy-0.2.0/tests/test_paths.py
--rw-r--r--   0        0        0        0 2023-05-04 01:22:20.093556 vocalpy-0.2.0/tests/test_repository/__init__.py
--rw-r--r--   0        0        0        0 2023-05-04 01:22:20.093841 vocalpy-0.2.0/tests/test_repository/test_repository.py
--rw-r--r--   0        0        0     2258 2023-05-07 21:46:44.720020 vocalpy-0.2.0/tests/test_segmenter.py
--rw-r--r--   0        0        0      547 2023-05-07 21:46:44.670223 vocalpy-0.2.0/tests/test_sequence.py
--rw-r--r--   0        0        0        0 2023-04-08 15:55:30.252298 vocalpy-0.2.0/tests/test_signal/__init__.py
--rw-r--r--   0        0        0      314 2023-05-07 20:16:29.809278 vocalpy-0.2.0/tests/test_signal/test_audio.py
--rw-r--r--   0        0        0      629 2023-05-07 20:16:29.809675 vocalpy-0.2.0/tests/test_signal/test_segment.py
--rw-r--r--   0        0        0        0 2023-04-08 15:55:30.252385 vocalpy-0.2.0/tests/test_signal/test_spectrogram.py
--rw-r--r--   0        0        0     4186 2023-05-04 01:22:20.095358 vocalpy-0.2.0/tests/test_spectrogram.py
--rw-r--r--   0        0        0     1500 2023-05-04 01:22:20.095856 vocalpy-0.2.0/tests/test_spectrogram_file.py
--rw-r--r--   0        0        0     4476 2023-05-07 21:09:06.876025 vocalpy-0.2.0/tests/test_spectrogram_maker.py
--rw-r--r--   0        0        0      848 2023-05-07 21:46:44.691384 vocalpy-0.2.0/tests/test_unit.py
--rw-r--r--   0        0        0     5037 1970-01-01 00:00:00.000000 vocalpy-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1307 2023-05-07 21:41:12.898528 vocalpy-0.2.0.post1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      248 2023-05-07 21:39:43.229568 vocalpy-0.2.0.post1/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      615 2023-05-07 21:39:43.228362 vocalpy-0.2.0.post1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      750 2023-05-07 20:16:29.801006 vocalpy-0.2.0.post1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      286 2023-04-25 13:42:56.058591 vocalpy-0.2.0.post1/.gitignore
+-rw-r--r--   0        0        0      769 2023-04-25 13:42:56.059258 vocalpy-0.2.0.post1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      367 2023-05-07 21:38:34.576998 vocalpy-0.2.0.post1/.readthedocs.yaml
+-rw-r--r--   0        0        0     5556 2023-05-07 20:52:52.998672 vocalpy-0.2.0.post1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1867 2023-05-07 20:53:11.404957 vocalpy-0.2.0.post1/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1540 2023-04-08 15:55:30.246016 vocalpy-0.2.0.post1/LICENSE
+-rw-r--r--   0        0        0     2064 2023-04-08 15:55:30.246197 vocalpy-0.2.0.post1/Makefile
+-rw-r--r--   0        0        0     3353 2023-05-07 22:07:24.777217 vocalpy-0.2.0.post1/README.md
+-rw-r--r--   0        0        0      251 2023-05-07 20:48:44.343584 vocalpy-0.2.0.post1/docs/CHANGELOG.md
+-rw-r--r--   0        0        0    29965 2023-05-07 20:41:50.515176 vocalpy-0.2.0.post1/docs/_static/vocalpy-logomark.png
+-rw-r--r--   0        0        0   285798 2023-05-07 20:41:50.763203 vocalpy-0.2.0.post1/docs/_static/vocalpy-primary.png
+-rw-r--r--   0        0        0   194159 2023-05-07 20:41:50.588788 vocalpy-0.2.0.post1/docs/_static/vocalpy-secondary.png
+-rw-r--r--   0        0        0     6436 2023-05-07 21:36:59.006708 vocalpy-0.2.0.post1/noxfile.py
+-rw-r--r--   0        0        0     1453 2023-05-07 22:11:05.316861 vocalpy-0.2.0.post1/pyproject.toml
+-rw-r--r--   0        0        0    19133 2023-04-25 13:43:12.342347 vocalpy-0.2.0.post1/src/scripts/attrs-sqlalchemy.ipynb
+-rw-r--r--   0        0        0     5151 2023-04-25 13:43:12.360555 vocalpy-0.2.0.post1/src/scripts/carpentries-sql-practice.ipynb
+-rw-r--r--   0        0        0    46531 2023-04-25 13:43:12.330739 vocalpy-0.2.0.post1/src/scripts/dataclass-orm.ipynb
+-rw-r--r--   0        0        0    21715 2023-04-25 13:43:12.389389 vocalpy-0.2.0.post1/src/scripts/dataset.ipynb
+-rw-r--r--   0        0        0     3130 2023-05-04 01:22:37.617838 vocalpy-0.2.0.post1/src/scripts/sqlite-python-tutorial.ipynb
+-rw-r--r--   0        0        0    22868 2023-05-07 21:52:44.503972 vocalpy-0.2.0.post1/src/scripts/vocalpy-sqlalchemy-orm.ipynb
+-rw-r--r--   0        0        0      810 2023-05-07 22:11:05.312790 vocalpy-0.2.0.post1/src/vocalpy/__about__.py
+-rw-r--r--   0        0        0     1304 2023-05-07 21:44:06.314669 vocalpy-0.2.0.post1/src/vocalpy/__init__.py
+-rw-r--r--   0        0        0       33 2023-04-25 13:42:56.065849 vocalpy-0.2.0.post1/src/vocalpy/annotation/__init__.py
+-rw-r--r--   0        0        0     1895 2023-05-04 01:22:20.075891 vocalpy-0.2.0.post1/src/vocalpy/annotation_file.py
+-rw-r--r--   0        0        0        0 2023-05-04 01:22:20.076056 vocalpy-0.2.0.post1/src/vocalpy/annotator.py
+-rw-r--r--   0        0        0     7738 2023-05-07 21:44:41.309650 vocalpy-0.2.0.post1/src/vocalpy/audio.py
+-rw-r--r--   0        0        0      635 2023-05-04 01:22:20.078518 vocalpy-0.2.0.post1/src/vocalpy/audio_file.py
+-rw-r--r--   0        0        0       30 2023-04-25 13:42:56.066572 vocalpy-0.2.0.post1/src/vocalpy/constants.py
+-rw-r--r--   0        0        0        0 2023-04-08 15:55:30.247903 vocalpy-0.2.0.post1/src/vocalpy/converters.py
+-rw-r--r--   0        0        0     4879 2023-05-04 01:22:20.079083 vocalpy-0.2.0.post1/src/vocalpy/dataset.py
+-rw-r--r--   0        0        0     2552 2023-05-07 21:02:40.315808 vocalpy-0.2.0.post1/src/vocalpy/dataset_file.py
+-rw-r--r--   0        0        0        0 2023-05-04 01:22:20.079995 vocalpy-0.2.0.post1/src/vocalpy/feature_extractor.py
+-rw-r--r--   0        0        0     1918 2023-05-04 01:22:20.080691 vocalpy-0.2.0.post1/src/vocalpy/feature_file.py
+-rw-r--r--   0        0        0     1118 2023-04-25 13:42:56.072844 vocalpy-0.2.0.post1/src/vocalpy/paths.py
+-rw-r--r--   0        0        0      146 2023-05-07 20:16:29.802759 vocalpy-0.2.0.post1/src/vocalpy/repository/__init__.py
+-rw-r--r--   0        0        0      441 2023-05-07 20:16:29.803288 vocalpy-0.2.0.post1/src/vocalpy/repository/base.py
+-rw-r--r--   0        0        0     3136 2023-05-04 01:22:20.081989 vocalpy-0.2.0.post1/src/vocalpy/repository/orm.py
+-rw-r--r--   0        0        0      677 2023-05-07 20:16:29.803723 vocalpy-0.2.0.post1/src/vocalpy/repository/sqlalchemy.py
+-rw-r--r--   0        0        0     3155 2023-05-07 21:44:06.438381 vocalpy-0.2.0.post1/src/vocalpy/segmenter.py
+-rw-r--r--   0        0        0     2502 2023-05-07 21:44:06.401117 vocalpy-0.2.0.post1/src/vocalpy/sequence.py
+-rw-r--r--   0        0        0      114 2023-05-04 01:22:20.084546 vocalpy-0.2.0.post1/src/vocalpy/signal/__init__.py
+-rw-r--r--   0        0        0     2301 2023-05-07 21:45:30.491360 vocalpy-0.2.0.post1/src/vocalpy/signal/audio.py
+-rw-r--r--   0        0        0     2244 2023-05-04 01:22:20.085058 vocalpy-0.2.0.post1/src/vocalpy/signal/preprocess.py
+-rw-r--r--   0        0        0     3012 2023-05-07 21:45:41.887997 vocalpy-0.2.0.post1/src/vocalpy/signal/segment.py
+-rw-r--r--   0        0        0     3062 2023-05-07 21:07:37.895584 vocalpy-0.2.0.post1/src/vocalpy/signal/spectrogram.py
+-rw-r--r--   0        0        0     7437 2023-05-04 01:22:20.086913 vocalpy-0.2.0.post1/src/vocalpy/spectrogram.py
+-rw-r--r--   0        0        0     1491 2023-05-04 01:22:20.087395 vocalpy-0.2.0.post1/src/vocalpy/spectrogram_file.py
+-rw-r--r--   0        0        0     8358 2023-05-07 21:44:06.512977 vocalpy-0.2.0.post1/src/vocalpy/spectrogram_maker.py
+-rw-r--r--   0        0        0      508 2023-05-04 01:22:20.088654 vocalpy-0.2.0.post1/src/vocalpy/spectrogram_parameters.py
+-rw-r--r--   0        0        0     1565 2023-05-07 21:44:06.416113 vocalpy-0.2.0.post1/src/vocalpy/unit.py
+-rw-r--r--   0        0        0      738 2023-04-25 13:42:56.074584 vocalpy-0.2.0.post1/src/vocalpy/validators.py
+-rw-r--r--   0        0        0        0 2023-04-08 15:55:30.249971 vocalpy-0.2.0.post1/tests/__init__.py
+-rw-r--r--   0        0        0       24 2023-04-08 15:55:30.250132 vocalpy-0.2.0.post1/tests/conftest.py
+-rw-r--r--   0        0        0      112 2023-04-25 13:42:56.075165 vocalpy-0.2.0.post1/tests/fixtures/__init__.py
+-rw-r--r--   0        0        0     2744 2023-04-25 13:42:56.075834 vocalpy-0.2.0.post1/tests/fixtures/annot.py
+-rw-r--r--   0        0        0     4620 2023-04-25 13:42:56.076380 vocalpy-0.2.0.post1/tests/fixtures/audio.py
+-rw-r--r--   0        0        0      834 2023-04-25 13:42:56.076724 vocalpy-0.2.0.post1/tests/fixtures/datasets.py
+-rw-r--r--   0        0        0     6669 2023-05-04 01:22:20.090376 vocalpy-0.2.0.post1/tests/fixtures/spect.py
+-rw-r--r--   0        0        0     1032 2023-04-25 13:42:56.077753 vocalpy-0.2.0.post1/tests/fixtures/test_data.py
+-rw-r--r--   0        0        0     2248 2023-04-25 13:42:56.078328 vocalpy-0.2.0.post1/tests/scripts/generate_data_for_tests.py
+-rw-r--r--   0        0        0     2695 2023-05-04 01:22:20.090889 vocalpy-0.2.0.post1/tests/test_annotation_file.py
+-rw-r--r--   0        0        0     8793 2023-05-07 21:46:44.905812 vocalpy-0.2.0.post1/tests/test_audio.py
+-rw-r--r--   0        0        0      992 2023-05-04 01:22:20.091867 vocalpy-0.2.0.post1/tests/test_audio_file.py
+-rw-r--r--   0        0        0     1605 2023-05-04 01:22:20.092370 vocalpy-0.2.0.post1/tests/test_dataset.py
+-rw-r--r--   0        0        0     2819 2023-05-07 21:46:44.715868 vocalpy-0.2.0.post1/tests/test_paths.py
+-rw-r--r--   0        0        0        0 2023-05-04 01:22:20.093556 vocalpy-0.2.0.post1/tests/test_repository/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 01:22:20.093841 vocalpy-0.2.0.post1/tests/test_repository/test_repository.py
+-rw-r--r--   0        0        0     2258 2023-05-07 21:46:44.720020 vocalpy-0.2.0.post1/tests/test_segmenter.py
+-rw-r--r--   0        0        0      547 2023-05-07 21:46:44.670223 vocalpy-0.2.0.post1/tests/test_sequence.py
+-rw-r--r--   0        0        0        0 2023-04-08 15:55:30.252298 vocalpy-0.2.0.post1/tests/test_signal/__init__.py
+-rw-r--r--   0        0        0      314 2023-05-07 20:16:29.809278 vocalpy-0.2.0.post1/tests/test_signal/test_audio.py
+-rw-r--r--   0        0        0      629 2023-05-07 20:16:29.809675 vocalpy-0.2.0.post1/tests/test_signal/test_segment.py
+-rw-r--r--   0        0        0        0 2023-04-08 15:55:30.252385 vocalpy-0.2.0.post1/tests/test_signal/test_spectrogram.py
+-rw-r--r--   0        0        0     4186 2023-05-04 01:22:20.095358 vocalpy-0.2.0.post1/tests/test_spectrogram.py
+-rw-r--r--   0        0        0     1500 2023-05-04 01:22:20.095856 vocalpy-0.2.0.post1/tests/test_spectrogram_file.py
+-rw-r--r--   0        0        0     4476 2023-05-07 21:09:06.876025 vocalpy-0.2.0.post1/tests/test_spectrogram_maker.py
+-rw-r--r--   0        0        0      848 2023-05-07 21:46:44.691384 vocalpy-0.2.0.post1/tests/test_unit.py
+-rw-r--r--   0        0        0     5055 1970-01-01 00:00:00.000000 vocalpy-0.2.0.post1/PKG-INFO
```

### Comparing `vocalpy-0.2.0/.github/ISSUE_TEMPLATE/bug_report.md` & `vocalpy-0.2.0.post1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `vocalpy-0.2.0/.github/ISSUE_TEMPLATE/feature_request.md` & `vocalpy-0.2.0.post1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `vocalpy-0.2.0/.github/workflows/ci.yml` & `vocalpy-0.2.0.post1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `vocalpy-0.2.0/.pre-commit-config.yaml` & `vocalpy-0.2.0.post1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `vocalpy-0.2.0/CODE_OF_CONDUCT.md` & `vocalpy-0.2.0.post1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `vocalpy-0.2.0/CONTRIBUTING.md` & `vocalpy-0.2.0.post1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `vocalpy-0.2.0/LICENSE` & `vocalpy-0.2.0.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `vocalpy-0.2.0/Makefile` & `vocalpy-0.2.0.post1/Makefile`

 * *Files identical despite different names*

### Comparing `vocalpy-0.2.0/README.md` & `vocalpy-0.2.0.post1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -80,8 +80,9 @@
 
 ### License
 
 The project is licensed under the [BSD license](./LICENSE).
 
 ### Citation
 If you use vocalpy, please cite the DOI:
-[![DOI](https://zenodo.org/badge/159904494.svg)](https://zenodo.org/badge/latestdoi/159904494)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7905426.svg)](https://doi.org/10.5281/zenodo.7905426)
+
```

### Comparing `vocalpy-0.2.0/docs/_static/vocalpy-logomark.png` & `vocalpy-0.2.0.post1/docs/_static/vocalpy-logomark.png`

 * *Files identical despite different names*

### Comparing `vocalpy-0.2.0/docs/_static/vocalpy-primary.png` & `vocalpy-0.2.0.post1/docs/_static/vocalpy-primary.png`

 * *Files identical despite different names*

### Comparing `vocalpy-0.2.0/docs/_static/vocalpy-secondary.png` & `vocalpy-0.2.0.post1/docs/_static/vocalpy-secondary.png`

 * *Files identical despite different names*

### Comparing `vocalpy-0.2.0/noxfile.py` & `vocalpy-0.2.0.post1/noxfile.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.2.0/pyproject.toml` & `vocalpy-0.2.0.post1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [project]
 name = "vocalpy"
 authors = [
     {name = "David Nicholson", email = "nickledave@users.noreply.github.com"}
 ]
 description = "Core package for acoustic communication in Python"
-version = "0.2.0"
+version = "0.2.0.post1"
 classifiers = [
         'License :: OSI Approved :: BSD License',
         'Development Status :: 5 - Production/Stable',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
```

### Comparing `vocalpy-0.2.0/src/scripts/attrs-sqlalchemy.ipynb` & `vocalpy-0.2.0.post1/src/scripts/attrs-sqlalchemy.ipynb`

 * *Files identical despite different names*

### Comparing `vocalpy-0.2.0/src/scripts/carpentries-sql-practice.ipynb` & `vocalpy-0.2.0.post1/src/scripts/carpentries-sql-practice.ipynb`

 * *Files identical despite different names*

### Comparing `vocalpy-0.2.0/src/scripts/dataclass-orm.ipynb` & `vocalpy-0.2.0.post1/src/scripts/dataclass-orm.ipynb`

 * *Files identical despite different names*

### Comparing `vocalpy-0.2.0/src/scripts/dataset.ipynb` & `vocalpy-0.2.0.post1/src/scripts/dataset.ipynb`

 * *Files identical despite different names*

### Comparing `vocalpy-0.2.0/src/scripts/sqlite-python-tutorial.ipynb` & `vocalpy-0.2.0.post1/src/scripts/sqlite-python-tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `vocalpy-0.2.0/src/scripts/vocalpy-sqlalchemy-orm.ipynb` & `vocalpy-0.2.0.post1/src/scripts/vocalpy-sqlalchemy-orm.ipynb`

 * *Files identical despite different names*

### Comparing `vocalpy-0.2.0/src/vocalpy/__about__.py` & `vocalpy-0.2.0.post1/src/vocalpy/__about__.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     base_dir = None
 
 
 __title__ = "vocalpy"
 __summary__ = "A core package for acoustic communication research in Python"
 __uri__ = "https://github.com/vocalpy/vocalpy"
 
-__version__ = "0.2.0"
+__version__ = "0.2.0.post1"
 
 if base_dir is not None and os.path.exists(os.path.join(base_dir, ".commit")):
     with open(os.path.join(base_dir, ".commit")) as fp:
         __commit__ = fp.read().strip()
 else:
     __commit__ = None
```

### Comparing `vocalpy-0.2.0/src/vocalpy/__init__.py` & `vocalpy-0.2.0.post1/src/vocalpy/__init__.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.2.0/src/vocalpy/annotation_file.py` & `vocalpy-0.2.0.post1/src/vocalpy/annotation_file.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.2.0/src/vocalpy/audio.py` & `vocalpy-0.2.0.post1/src/vocalpy/audio.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.2.0/src/vocalpy/audio_file.py` & `vocalpy-0.2.0.post1/src/vocalpy/audio_file.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.2.0/src/vocalpy/dataset.py` & `vocalpy-0.2.0.post1/src/vocalpy/dataset.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.2.0/src/vocalpy/dataset_file.py` & `vocalpy-0.2.0.post1/src/vocalpy/dataset_file.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.2.0/src/vocalpy/feature_file.py` & `vocalpy-0.2.0.post1/src/vocalpy/feature_file.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.2.0/src/vocalpy/paths.py` & `vocalpy-0.2.0.post1/src/vocalpy/paths.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.2.0/src/vocalpy/repository/orm.py` & `vocalpy-0.2.0.post1/src/vocalpy/repository/orm.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.2.0/src/vocalpy/repository/sqlalchemy.py` & `vocalpy-0.2.0.post1/src/vocalpy/repository/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.2.0/src/vocalpy/segmenter.py` & `vocalpy-0.2.0.post1/src/vocalpy/segmenter.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.2.0/src/vocalpy/sequence.py` & `vocalpy-0.2.0.post1/src/vocalpy/sequence.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.2.0/src/vocalpy/signal/audio.py` & `vocalpy-0.2.0.post1/src/vocalpy/signal/audio.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.2.0/src/vocalpy/signal/preprocess.py` & `vocalpy-0.2.0.post1/src/vocalpy/signal/preprocess.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.2.0/src/vocalpy/signal/segment.py` & `vocalpy-0.2.0.post1/src/vocalpy/signal/segment.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.2.0/src/vocalpy/signal/spectrogram.py` & `vocalpy-0.2.0.post1/src/vocalpy/signal/spectrogram.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.2.0/src/vocalpy/spectrogram.py` & `vocalpy-0.2.0.post1/src/vocalpy/spectrogram.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.2.0/src/vocalpy/spectrogram_file.py` & `vocalpy-0.2.0.post1/src/vocalpy/spectrogram_file.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.2.0/src/vocalpy/spectrogram_maker.py` & `vocalpy-0.2.0.post1/src/vocalpy/spectrogram_maker.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.2.0/src/vocalpy/unit.py` & `vocalpy-0.2.0.post1/src/vocalpy/unit.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.2.0/src/vocalpy/validators.py` & `vocalpy-0.2.0.post1/src/vocalpy/validators.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.2.0/tests/fixtures/annot.py` & `vocalpy-0.2.0.post1/tests/fixtures/annot.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.2.0/tests/fixtures/audio.py` & `vocalpy-0.2.0.post1/tests/fixtures/audio.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.2.0/tests/fixtures/datasets.py` & `vocalpy-0.2.0.post1/tests/fixtures/datasets.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.2.0/tests/fixtures/spect.py` & `vocalpy-0.2.0.post1/tests/fixtures/spect.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.2.0/tests/fixtures/test_data.py` & `vocalpy-0.2.0.post1/tests/fixtures/test_data.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.2.0/tests/scripts/generate_data_for_tests.py` & `vocalpy-0.2.0.post1/tests/scripts/generate_data_for_tests.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.2.0/tests/test_annotation_file.py` & `vocalpy-0.2.0.post1/tests/test_annotation_file.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.2.0/tests/test_audio.py` & `vocalpy-0.2.0.post1/tests/test_audio.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.2.0/tests/test_audio_file.py` & `vocalpy-0.2.0.post1/tests/test_audio_file.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.2.0/tests/test_dataset.py` & `vocalpy-0.2.0.post1/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.2.0/tests/test_paths.py` & `vocalpy-0.2.0.post1/tests/test_paths.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.2.0/tests/test_segmenter.py` & `vocalpy-0.2.0.post1/tests/test_segmenter.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.2.0/tests/test_sequence.py` & `vocalpy-0.2.0.post1/tests/test_sequence.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.2.0/tests/test_signal/test_segment.py` & `vocalpy-0.2.0.post1/tests/test_signal/test_segment.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.2.0/tests/test_spectrogram.py` & `vocalpy-0.2.0.post1/tests/test_spectrogram.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.2.0/tests/test_spectrogram_file.py` & `vocalpy-0.2.0.post1/tests/test_spectrogram_file.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.2.0/tests/test_spectrogram_maker.py` & `vocalpy-0.2.0.post1/tests/test_spectrogram_maker.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.2.0/tests/test_unit.py` & `vocalpy-0.2.0.post1/tests/test_unit.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.2.0/PKG-INFO` & `vocalpy-0.2.0.post1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vocalpy
-Version: 0.2.0
+Version: 0.2.0.post1
 Summary: Core package for acoustic communication in Python
 Author-email: David Nicholson <nickledave@users.noreply.github.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
@@ -122,9 +122,10 @@
 
 ### License
 
 The project is licensed under the [BSD license](./LICENSE).
 
 ### Citation
 If you use vocalpy, please cite the DOI:
-[![DOI](https://zenodo.org/badge/159904494.svg)](https://zenodo.org/badge/latestdoi/159904494)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7905426.svg)](https://doi.org/10.5281/zenodo.7905426)
+
```

