# Comparing `tmp/a2-0.3.2.tar.gz` & `tmp/a2-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "a2-0.3.2.tar", max compression
+gzip compressed data, was "a2-0.3.3.tar", max compression
```

## Comparing `a2-0.3.2.tar` & `a2-0.3.3.tar`

### file list

```diff
@@ -1,54 +1,53 @@
--rw-r--r--   0        0        0     3769 2023-04-20 06:31:32.717643 a2-0.3.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-20 15:29:54.345253 a2-0.3.2/src/a2/__init__.py
--rw-r--r--   0        0        0       45 2023-01-13 09:43:31.404482 a2-0.3.2/src/a2/cli/__init__.py
--rw-r--r--   0        0        0       39 2023-01-13 09:45:19.522669 a2-0.3.2/src/a2/cli/cli_plotting/__init__.py
--rw-r--r--   0        0        0      107 2023-01-13 09:46:23.599985 a2-0.3.2/src/a2/cli/cli_plotting/plot.py
--rw-r--r--   0        0        0     2056 2023-02-16 10:12:08.320539 a2-0.3.2/src/a2/cli/cli_plotting/single_plots.py
--rw-r--r--   0        0        0       66 2023-01-13 09:36:10.235731 a2-0.3.2/src/a2/cli/main.py
--rw-r--r--   0        0        0        0 2022-11-01 14:44:14.720032 a2-0.3.2/src/a2/data/__init__.py
--rw-r--r--   0        0        0        0 2022-11-01 14:44:14.720032 a2-0.3.2/src/a2/data/emoji/__init__.py
--rw-r--r--   0        0        0   379747 2022-11-01 14:44:14.724032 a2-0.3.2/src/a2/data/emoji/emoji_df.csv
--rw-r--r--   0        0        0        0 2022-11-01 14:44:14.724032 a2-0.3.2/src/a2/data/vocabularies/__init__.py
--rw-r--r--   0        0        0     2789 2023-02-21 08:27:21.563839 a2-0.3.2/src/a2/data/vocabularies/weather_vocab_enchanted_learning_com.txt
--rw-r--r--   0        0        0      236 2023-02-21 08:27:21.563869 a2-0.3.2/src/a2/data/vocabularies/weather_vocab_enchanted_precipitation.txt
--rw-r--r--   0        0        0      188 2023-02-21 14:04:17.568649 a2-0.3.2/src/a2/dataset/__init__.py
--rw-r--r--   0        0        0      556 2023-01-30 14:59:51.635141 a2-0.3.2/src/a2/dataset/emojis.py
--rw-r--r--   0        0        0     7525 2023-02-20 13:53:30.152744 a2-0.3.2/src/a2/dataset/load_dataset.py
--rw-r--r--   0        0        0    50068 2023-01-30 14:59:51.635141 a2-0.3.2/src/a2/dataset/radar.py
--rw-r--r--   0        0        0    10354 2023-01-30 14:59:51.635141 a2-0.3.2/src/a2/dataset/stations.py
--rw-r--r--   0        0        0      699 2023-02-20 13:53:30.152744 a2-0.3.2/src/a2/dataset/tweets.py
--rw-r--r--   0        0        0     1464 2022-12-14 09:36:33.150856 a2-0.3.2/src/a2/dataset/units.py
--rw-r--r--   0        0        0    16914 2023-02-15 13:23:54.265629 a2-0.3.2/src/a2/dataset/utils_dataset.py
--rw-r--r--   0        0        0      191 2022-12-14 09:36:33.150856 a2-0.3.2/src/a2/plotting/__init__.py
--rw-r--r--   0        0        0     8266 2023-03-03 16:00:04.992588 a2-0.3.2/src/a2/plotting/analysis.py
--rw-r--r--   0        0        0     1964 2023-02-14 14:11:41.262470 a2-0.3.2/src/a2/plotting/axes_utils.py
--rw-r--r--   0        0        0    29338 2023-04-12 11:32:44.371869 a2-0.3.2/src/a2/plotting/histograms.py
--rw-r--r--   0        0        0     3007 2022-12-14 09:36:33.154856 a2-0.3.2/src/a2/plotting/parallel_plotting.py
--rw-r--r--   0        0        0     2809 2022-12-14 09:36:33.154856 a2-0.3.2/src/a2/plotting/timeseries.py
--rw-r--r--   0        0        0    16032 2023-03-03 15:56:41.072135 a2-0.3.2/src/a2/plotting/utils_plotting.py
--rw-r--r--   0        0        0    34741 2023-02-20 13:53:30.156744 a2-0.3.2/src/a2/plotting/weather_maps.py
--rw-r--r--   0        0        0       67 2022-11-01 14:44:14.724032 a2-0.3.2/src/a2/preprocess/__init__.py
--rw-r--r--   0        0        0     3645 2022-12-06 08:38:01.708129 a2-0.3.2/src/a2/preprocess/embedding.py
--rw-r--r--   0        0        0    29471 2022-12-06 08:38:01.708129 a2-0.3.2/src/a2/preprocess/normalize_text.py
--rw-r--r--   0        0        0      172 2023-03-03 15:56:22.067727 a2-0.3.2/src/a2/training/__init__.py
--rw-r--r--   0        0        0     3618 2023-04-20 06:29:52.911455 a2-0.3.2/src/a2/training/benchmarks.py
--rw-r--r--   0        0        0     2556 2022-12-14 09:36:33.154856 a2-0.3.2/src/a2/training/dataset_hugging.py
--rw-r--r--   0        0        0     4131 2023-02-02 13:31:55.647577 a2-0.3.2/src/a2/training/evaluate_hugging.py
--rw-r--r--   0        0        0     4421 2023-04-12 09:53:21.965604 a2-0.3.2/src/a2/training/tracking.py
--rw-r--r--   0        0        0     1780 2023-04-12 09:29:10.503408 a2-0.3.2/src/a2/training/tracking_hugging.py
--rw-r--r--   0        0        0     6390 2023-03-02 16:51:55.930811 a2-0.3.2/src/a2/training/training_deep500.py
--rw-r--r--   0        0        0     8949 2023-04-12 09:53:21.577595 a2-0.3.2/src/a2/training/training_hugging.py
--rw-r--r--   0        0        0     6821 2023-04-17 13:38:37.032507 a2-0.3.2/src/a2/training/training_performance.py
--rw-r--r--   0        0        0       73 2023-01-30 14:59:51.639141 a2-0.3.2/src/a2/training/utils_training.py
--rw-r--r--   0        0        0       87 2022-11-01 14:44:14.728032 a2-0.3.2/src/a2/twitter/__init__.py
--rw-r--r--   0        0        0     4570 2023-02-20 13:53:30.156744 a2-0.3.2/src/a2/twitter/downloader.py
--rw-r--r--   0        0        0    11233 2023-02-20 13:53:30.156744 a2-0.3.2/src/a2/twitter/locations.py
--rw-r--r--   0        0        0     6765 2023-02-20 13:53:30.156744 a2-0.3.2/src/a2/twitter/twitter_api.py
--rw-r--r--   0        0        0      147 2022-12-14 09:36:33.154856 a2-0.3.2/src/a2/utils/__init__.py
--rw-r--r--   0        0        0      518 2022-12-14 09:36:33.154856 a2-0.3.2/src/a2/utils/checks.py
--rw-r--r--   0        0        0      362 2023-02-20 15:01:52.076201 a2-0.3.2/src/a2/utils/constants.py
--rw-r--r--   0        0        0     9181 2023-04-12 10:07:20.603125 a2-0.3.2/src/a2/utils/file_handling.py
--rw-r--r--   0        0        0     5220 2023-04-19 06:56:16.631322 a2-0.3.2/src/a2/utils/testing.py
--rw-r--r--   0        0        0      394 2022-12-14 09:36:33.154856 a2-0.3.2/src/a2/utils/times.py
--rw-r--r--   0        0        0     6044 2023-03-03 15:56:22.027726 a2-0.3.2/src/a2/utils/utils.py
--rw-r--r--   0        0        0     1887 1970-01-01 00:00:00.000000 a2-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     3450 2023-05-08 07:43:41.881508 a2-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-02-20 15:29:54.345253 a2-0.3.3/src/a2/__init__.py
+-rw-r--r--   0        0        0       45 2023-01-13 09:43:31.404482 a2-0.3.3/src/a2/cli/__init__.py
+-rw-r--r--   0        0        0       39 2023-01-13 09:45:19.522669 a2-0.3.3/src/a2/cli/cli_plotting/__init__.py
+-rw-r--r--   0        0        0      107 2023-01-13 09:46:23.599985 a2-0.3.3/src/a2/cli/cli_plotting/plot.py
+-rw-r--r--   0        0        0     2056 2023-02-16 10:12:08.320539 a2-0.3.3/src/a2/cli/cli_plotting/single_plots.py
+-rw-r--r--   0        0        0       66 2023-01-13 09:36:10.235731 a2-0.3.3/src/a2/cli/main.py
+-rw-r--r--   0        0        0        0 2022-11-01 14:44:14.720032 a2-0.3.3/src/a2/data/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-01 14:44:14.720032 a2-0.3.3/src/a2/data/emoji/__init__.py
+-rw-r--r--   0        0        0   379747 2022-11-01 14:44:14.724032 a2-0.3.3/src/a2/data/emoji/emoji_df.csv
+-rw-r--r--   0        0        0        0 2022-11-01 14:44:14.724032 a2-0.3.3/src/a2/data/vocabularies/__init__.py
+-rw-r--r--   0        0        0     2789 2023-02-21 08:27:21.563839 a2-0.3.3/src/a2/data/vocabularies/weather_vocab_enchanted_learning_com.txt
+-rw-r--r--   0        0        0      236 2023-02-21 08:27:21.563869 a2-0.3.3/src/a2/data/vocabularies/weather_vocab_enchanted_precipitation.txt
+-rw-r--r--   0        0        0      188 2023-02-21 14:04:17.568649 a2-0.3.3/src/a2/dataset/__init__.py
+-rw-r--r--   0        0        0      556 2023-01-30 14:59:51.635141 a2-0.3.3/src/a2/dataset/emojis.py
+-rw-r--r--   0        0        0     7525 2023-05-02 15:07:25.505833 a2-0.3.3/src/a2/dataset/load_dataset.py
+-rw-r--r--   0        0        0    50068 2023-01-30 14:59:51.635141 a2-0.3.3/src/a2/dataset/radar.py
+-rw-r--r--   0        0        0    10354 2023-01-30 14:59:51.635141 a2-0.3.3/src/a2/dataset/stations.py
+-rw-r--r--   0        0        0      699 2023-02-20 13:53:30.152744 a2-0.3.3/src/a2/dataset/tweets.py
+-rw-r--r--   0        0        0     1464 2022-12-14 09:36:33.150856 a2-0.3.3/src/a2/dataset/units.py
+-rw-r--r--   0        0        0    16914 2023-05-02 15:07:25.505833 a2-0.3.3/src/a2/dataset/utils_dataset.py
+-rw-r--r--   0        0        0      191 2022-12-14 09:36:33.150856 a2-0.3.3/src/a2/plotting/__init__.py
+-rw-r--r--   0        0        0     8266 2023-03-03 16:00:04.992588 a2-0.3.3/src/a2/plotting/analysis.py
+-rw-r--r--   0        0        0     1964 2023-02-14 14:11:41.262470 a2-0.3.3/src/a2/plotting/axes_utils.py
+-rw-r--r--   0        0        0    30229 2023-05-05 14:40:53.816499 a2-0.3.3/src/a2/plotting/histograms.py
+-rw-r--r--   0        0        0     3007 2022-12-14 09:36:33.154856 a2-0.3.3/src/a2/plotting/parallel_plotting.py
+-rw-r--r--   0        0        0     2809 2022-12-14 09:36:33.154856 a2-0.3.3/src/a2/plotting/timeseries.py
+-rw-r--r--   0        0        0    16094 2023-05-05 14:40:53.468490 a2-0.3.3/src/a2/plotting/utils_plotting.py
+-rw-r--r--   0        0        0    34741 2023-02-20 13:53:30.156744 a2-0.3.3/src/a2/plotting/weather_maps.py
+-rw-r--r--   0        0        0       67 2022-11-01 14:44:14.724032 a2-0.3.3/src/a2/preprocess/__init__.py
+-rw-r--r--   0        0        0     3645 2022-12-06 08:38:01.708129 a2-0.3.3/src/a2/preprocess/embedding.py
+-rw-r--r--   0        0        0    29471 2023-05-02 15:07:25.505833 a2-0.3.3/src/a2/preprocess/normalize_text.py
+-rw-r--r--   0        0        0      172 2023-03-03 15:56:22.067727 a2-0.3.3/src/a2/training/__init__.py
+-rw-r--r--   0        0        0     3824 2023-05-05 07:20:43.819827 a2-0.3.3/src/a2/training/benchmarks.py
+-rw-r--r--   0        0        0     2556 2023-04-26 11:36:30.427087 a2-0.3.3/src/a2/training/dataset_hugging.py
+-rw-r--r--   0        0        0     4131 2023-02-02 13:31:55.647577 a2-0.3.3/src/a2/training/evaluate_hugging.py
+-rw-r--r--   0        0        0     4421 2023-05-05 07:05:59.302657 a2-0.3.3/src/a2/training/tracking.py
+-rw-r--r--   0        0        0     1780 2023-04-12 09:29:10.503408 a2-0.3.3/src/a2/training/tracking_hugging.py
+-rw-r--r--   0        0        0     6390 2023-03-02 16:51:55.930811 a2-0.3.3/src/a2/training/training_deep500.py
+-rw-r--r--   0        0        0    10827 2023-05-05 08:25:01.183922 a2-0.3.3/src/a2/training/training_hugging.py
+-rw-r--r--   0        0        0       73 2023-01-30 14:59:51.639141 a2-0.3.3/src/a2/training/utils_training.py
+-rw-r--r--   0        0        0       87 2022-11-01 14:44:14.728032 a2-0.3.3/src/a2/twitter/__init__.py
+-rw-r--r--   0        0        0     4570 2023-02-20 13:53:30.156744 a2-0.3.3/src/a2/twitter/downloader.py
+-rw-r--r--   0        0        0    11233 2023-05-02 15:07:25.505833 a2-0.3.3/src/a2/twitter/locations.py
+-rw-r--r--   0        0        0     6765 2023-02-20 13:53:30.156744 a2-0.3.3/src/a2/twitter/twitter_api.py
+-rw-r--r--   0        0        0      147 2023-05-02 15:07:25.505833 a2-0.3.3/src/a2/utils/__init__.py
+-rw-r--r--   0        0        0      518 2022-12-14 09:36:33.154856 a2-0.3.3/src/a2/utils/checks.py
+-rw-r--r--   0        0        0      362 2023-02-20 15:01:52.076201 a2-0.3.3/src/a2/utils/constants.py
+-rw-r--r--   0        0        0     9219 2023-05-05 08:00:02.140306 a2-0.3.3/src/a2/utils/file_handling.py
+-rw-r--r--   0        0        0     5220 2023-05-02 15:07:25.505833 a2-0.3.3/src/a2/utils/testing.py
+-rw-r--r--   0        0        0      394 2022-12-14 09:36:33.154856 a2-0.3.3/src/a2/utils/times.py
+-rw-r--r--   0        0        0     6088 2023-05-05 07:18:42.720934 a2-0.3.3/src/a2/utils/utils.py
+-rw-r--r--   0        0        0     1746 1970-01-01 00:00:00.000000 a2-0.3.3/PKG-INFO
```

### Comparing `a2-0.3.2/pyproject.toml` & `a2-0.3.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,100 +1,94 @@
 [tool.poetry]
 name = "a2"
-version = "0.3.2"
+version = "0.3.3"
 description = "Package for predicting information about the weather from social media data as application 2 for maelstrom project"
 authors = ["Kristian Ehlert <kristian.ehlert@4-cast.de>"]
 packages = [{ include = "a2", from = "src"}]
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
 jupyterlab = "^3.4.3"
 requests = "^2.28.1"
 pandas = "^1.4.2"
 DateTime = "^4.4"
 matplotlib = "^3.5.2"
 xarray = "^2022.3.0"
 emoji = "<1.0.0"
 dask = "^2022.6.1"
+pytest-recording = "^0.12.1"
 ipywidgets = "^7.7.1"
 spacymoji = "^3.0.1"
 wget = "^3.2"
 jsonlines = "^3.1.0"
 tweepy = "^4.10.0"
 Shapely = "^1.8.2"
 pyproj = "^3.3.1"
 h5py = "^3.7.0"
 netCDF4 = "^1.6.0"
 h5netcdf = "^1.0.1"
 mantik = "^0.1.0"
+pytest-xdist = "^2.5.0"
 urllib3 = "^1.26.12"
 scikit-learn = "^1.1.2"
 kaleido = "0.2.1"
 rioxarray = "^0.12.2"
 rasterio = "^1.3.3"
 convertbng = "^0.6.39"
 plotly = "^5.11.0"
 seaborn = "^0.12.1"
 geopy = "^2.3.0"
 click = "^8.1.3"
 ipython = "^8.7.0"
-llvmlite = "^0.39.1"
-datasets = "^2.11.0"
-#transformers = {git = "https://github.com/huggingface/transformers", branch = "main", optional = true }
-torch = {version = "^2.0.0", optional = true}
-sentencepiece = {version = "^0.1.98", optional = true}
 
 [tool.poetry.group.dev.dependencies]
 black = {extras = ["jupyter"], version = "^22.6.0"}
 mypy = "^0.971"
 reorder-python-imports = "^3.1.0"
 types-python-dateutil = "^2.8.18"
 types-requests = "^2.28.0"
 pandas-stubs = "^1.4.2"
 pytest = "^7.1.2"
 pytest-cov = "^3.0.0"
 pytest-cases = "^3.6.13"
-pytest-recording = "^0.12.1"
-pytest-xdist = "^2.5.0"
 types-tqdm = "^4.64.4"
 line-profiler = {extras = ["ipython"], version = "^3.5.1"}
 pyflakes = "^2.5.0"
 traceback-with-variables = "^2.0.4"
 sacremoses = "^0.0.53"
 deepdiff = "^5.8.1"
 guppy3 = "^3.1.2"
 memory-profiler = "^0.60.0"
 pre-commit = "^2.20.0"
 docformatter = "^1.5.0"
 pytest-mpl = "^0.16.1"
 responses = "0.18"
 pytest-mock = "^3.10.0"
 
-[tool.poetry.extras]
-llama-chatbot = ["transformers", "sentencepiece"]
-torch = ["torch"]
 
 [tool.poetry.group.parallel.dependencies]
 p-tqdm = "^1.4.0"
 
-[tool.poetry.group.train]
-optional = true
+
 [tool.poetry.group.train.dependencies]
 xgboost = "^1.6.2"
 catboost = "^1.1"
 nltk = "^3.7"
 sentence-transformers = "^2.2.2"
+datasets = "^2.7.1"
+transformers = {extras = ["torch"], version = "^4.25.1"}
+sentencepiece = "^0.1.97"
 ray = {extras = ["tune"], version = "^2.2.0"}
 tensorboard = "^2.11.0"
 
 
-[tool.poetry.group.benchmarking]
-optional = true
 [tool.poetry.group.benchmarking.dependencies]
+onnx = "^1.13.0"
 optimum = {extras = ["onnxruntime"], version = "^1.7.1", optional = true}
+transformers = {extras = ["onnx"], version = "^4.27.1"}
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 a2 = 'a2.cli.main:cli'
@@ -143,20 +137,19 @@
 line-length = 120
 
 [tool.flake8]
 max-line-length = 120
 per-file-ignores = [
     "__init__.py:F401,E501",
     "training_deep500.py:F403,F405",
-    "training_performance.py:F403,F405",
 ]
 
-# [tool.poetry.extras]
-# extend-exclude = [
-#     "notebooks/training/helper_deep500.py"
-# ]
+[tool.poetry.extras]
+extend-exclude = [
+    "helper_deep500.py"
+]
 
 [tool.pytest.ini_options]
 log_cli = true
 log_cli_level = "INFO"
 log_cli_format = "%(asctime)s [%(levelname)8s] %(message)s (%(filename)s:%(lineno)s)"
 log_cli_date_format = "%Y-%m-%d %H:%M:%S"
```

### Comparing `a2-0.3.2/src/a2/cli/cli_plotting/single_plots.py` & `a2-0.3.3/src/a2/cli/cli_plotting/single_plots.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.2/src/a2/data/emoji/emoji_df.csv` & `a2-0.3.3/src/a2/data/emoji/emoji_df.csv`

 * *Files identical despite different names*

### Comparing `a2-0.3.2/src/a2/data/vocabularies/weather_vocab_enchanted_learning_com.txt` & `a2-0.3.3/src/a2/data/vocabularies/weather_vocab_enchanted_learning_com.txt`

 * *Files identical despite different names*

### Comparing `a2-0.3.2/src/a2/dataset/emojis.py` & `a2-0.3.3/src/a2/dataset/emojis.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.2/src/a2/dataset/load_dataset.py` & `a2-0.3.3/src/a2/dataset/load_dataset.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.2/src/a2/dataset/radar.py` & `a2-0.3.3/src/a2/dataset/radar.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.2/src/a2/dataset/stations.py` & `a2-0.3.3/src/a2/dataset/stations.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.2/src/a2/dataset/tweets.py` & `a2-0.3.3/src/a2/dataset/tweets.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.2/src/a2/dataset/units.py` & `a2-0.3.3/src/a2/dataset/units.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.2/src/a2/dataset/utils_dataset.py` & `a2-0.3.3/src/a2/dataset/utils_dataset.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.2/src/a2/plotting/analysis.py` & `a2-0.3.3/src/a2/plotting/analysis.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.2/src/a2/plotting/axes_utils.py` & `a2-0.3.3/src/a2/plotting/axes_utils.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.2/src/a2/plotting/histograms.py` & `a2-0.3.3/src/a2/plotting/histograms.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import logging
 import pathlib
 import typing as t
 
 import a2.dataset
 import a2.plotting.utils_plotting
 import a2.utils.constants
+import matplotlib.figure
 import matplotlib.offsetbox
 import matplotlib.pyplot as plt
 import numpy as np
 import xarray
 
 
 FILE_LOC = pathlib.Path(__file__).parent
@@ -22,15 +23,14 @@
     bins: t.Sequence | None = None,
     xlim: t.Sequence | None = None,
     ylim: t.Sequence | None = None,
     ax: a2.utils.constants.TYPE_MATPLOTLIB_AXES | None = None,
     ax_colorbar: a2.utils.constants.TYPE_MATPLOTLIB_AXES | None = None,
     log: t.Union[bool, t.List[bool]] = False,
     filename: str | pathlib.Path | None = None,
-    fig: a2.utils.constants.TYPE_MATPLOTLIB_FIGURES | None = None,
     n_bins: t.Union[int, t.List[int]] = 60,
     norm: str | None = None,
     linear_thresh: t.Union[float, t.List[float]] = 1e-9,
     label_x: str | None = None,
     label_y: str | None = None,
     label_colorbar: str | None = None,
     font_size: int = 12,
@@ -114,64 +114,23 @@
     """
     marginal_x, marginal_y = _resolve_defaults(facet_column, facet_row, marginal_x, marginal_y)
     _check_histogram_parameter_consistency(facet_column, facet_row, marginal_x, marginal_y, ds)
 
     facet_column_values, column_masks, n_facet_column_values, facet_column_title = prepare_facet(ds, facet_column)
     facet_row_values, row_masks, n_facet_row_values, facet_row_title = prepare_facet(ds, facet_row)
 
-    n_columns = 1
-    if n_facet_column_values:
-        n_columns = n_facet_column_values
-    elif marginal_x is not None:
-        n_columns = 2
+    n_columns, n_rows = _set_number_rows_and_columns(marginal_x, marginal_y, n_facet_column_values, n_facet_row_values)
 
-    n_rows = 1
-    if n_facet_row_values:
-        n_rows = n_facet_row_values
-    elif marginal_y is not None:
-        n_rows = 2
+    masks = _set_masks(column_masks, row_masks, n_columns, n_rows)
 
-    def add_masks(mask, to_add):
-        if to_add is None:
-            return mask
-        if mask is None:
-            return to_add
-        else:
-            return mask & to_add
+    titles = _set_axes_titles(facet_column, facet_row, title, facet_column_title, facet_row_title, n_columns, n_rows)
 
-    masks = np.full((n_rows, n_columns), None, dtype=object)
-    for i_row in range(n_rows):
-        for i_column in range(n_columns):
-            if column_masks is not None:
-                masks[i_row, i_column] = add_masks(masks[i_row, i_column], column_masks[i_column])
-            if row_masks is not None:
-                masks[i_row, i_column] = add_masks(masks[i_row, i_column], row_masks[i_row])
-
-    def add_titles(titles, delimeter=", "):
-        return f"{delimeter}".join([t for t in titles if len(t)])
-
-    titles = np.full((n_rows, n_columns), title, dtype=object)
-    for i_row in range(n_rows):
-        for i_column in range(n_columns):
-            if facet_row:
-                titles[i_row, i_column] = add_titles([titles[i_row, i_column], facet_row_title[i_row]])
-            if facet_column:
-                titles[i_row, i_column] = add_titles([titles[i_row, i_column], facet_column_title[i_column]])
-
-    skip_row_col = None
-    widths_along_x = None
-    heights_along_y = None
-    colorbar_include_row_col = None
-
-    colorbar_off = False
-    if marginal_x is not None and marginal_y is not None:
-        skip_row_col = [[0, 1]]
-        widths_along_x = [0.2, 0.1]
-        heights_along_y = [0.1, 0.2]
-        colorbar_include_row_col = [[1, 1]]
+    skip_row_col, widths_along_x, heights_along_y, colorbar_include_row_col, colorbar_off = _prepare_axes_grid_creation(
+        marginal_x, marginal_y
+    )
 
     fig, axes, axes_colorbar = a2.plotting.utils_plotting.create_axes_grid(
         n_cols=n_columns,
         n_rows=n_rows,
         figure_size=figure_size,
         skip_row_col=skip_row_col,
         colorbar_width=colorbar_width,
@@ -179,14 +138,15 @@
         spacing_y=spacing_y,
         widths_along_x=widths_along_x,
         heights_along_y=heights_along_y,
         colorbar_include_row_col=colorbar_include_row_col,
         spacing_colorbar=spacing_colorbar,
         colorbar_off=colorbar_off,
     )
+
     if font_size is not None:
         a2.plotting.utils_plotting.set_font(font_size=font_size)
 
     results_dic = {"axes": [], "histograms": []}
     for i_row in range(n_rows):
         for i_column in range(n_columns):
             ax = axes[i_row, i_column]
@@ -240,14 +200,79 @@
 
             if marginal_x is not None and marginal_y is not None:
                 break
     a2.plotting.utils_plotting.save_figure(fig, filename)
     return results_dic
 
 
+def _prepare_axes_grid_creation(marginal_x, marginal_y):
+    skip_row_col = None
+    widths_along_x = None
+    heights_along_y = None
+    colorbar_include_row_col = None
+
+    colorbar_off = False
+    if marginal_x is not None and marginal_y is not None:
+        skip_row_col = [[0, 1]]
+        widths_along_x = [0.2, 0.1]
+        heights_along_y = [0.1, 0.2]
+        colorbar_include_row_col = [[1, 1]]
+    return skip_row_col, widths_along_x, heights_along_y, colorbar_include_row_col, colorbar_off
+
+
+def _set_axes_titles(facet_column, facet_row, title, facet_column_title, facet_row_title, n_columns, n_rows):
+    titles = np.full((n_rows, n_columns), title, dtype=object)
+    for i_row in range(n_rows):
+        for i_column in range(n_columns):
+            if facet_row:
+                titles[i_row, i_column] = _add_titles([titles[i_row, i_column], facet_row_title[i_row]])
+            if facet_column:
+                titles[i_row, i_column] = _add_titles([titles[i_row, i_column], facet_column_title[i_column]])
+    return titles
+
+
+def _add_titles(titles, delimeter=", "):
+    return f"{delimeter}".join([t for t in titles if len(t)])
+
+
+def _set_masks(column_masks, row_masks, n_columns, n_rows):
+    masks = np.full((n_rows, n_columns), None, dtype=object)
+    for i_row in range(n_rows):
+        for i_column in range(n_columns):
+            if column_masks is not None:
+                masks[i_row, i_column] = _add_masks(masks[i_row, i_column], column_masks[i_column])
+            if row_masks is not None:
+                masks[i_row, i_column] = _add_masks(masks[i_row, i_column], row_masks[i_row])
+    return masks
+
+
+def _add_masks(mask, to_add):
+    if to_add is None:
+        return mask
+    if mask is None:
+        return to_add
+    else:
+        return mask & to_add
+
+
+def _set_number_rows_and_columns(marginal_x, marginal_y, n_facet_column_values, n_facet_row_values):
+    n_columns = 1
+    if n_facet_column_values:
+        n_columns = n_facet_column_values
+    elif marginal_x is not None:
+        n_columns = 2
+
+    n_rows = 1
+    if n_facet_row_values:
+        n_rows = n_facet_row_values
+    elif marginal_y is not None:
+        n_rows = 2
+    return n_columns, n_rows
+
+
 def _resolve_defaults(facet_column, facet_row, marginal_x, marginal_y):
     if marginal_x == "default":
         if facet_column is None and facet_row is None:
             marginal_x = "histogram"
         else:
             marginal_x = None
     if marginal_y == "default":
```

### Comparing `a2-0.3.2/src/a2/plotting/parallel_plotting.py` & `a2-0.3.3/src/a2/plotting/parallel_plotting.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.2/src/a2/plotting/timeseries.py` & `a2-0.3.3/src/a2/plotting/timeseries.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.2/src/a2/plotting/utils_plotting.py` & `a2-0.3.3/src/a2/plotting/utils_plotting.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import logging
 import os
 import pathlib
 import typing as t
 
 import a2.utils.utils
 import matplotlib.colors
+import matplotlib.figure
 import numpy as np
 from matplotlib import pyplot as plt
 
 
 def set_x_log(ax: plt.axes, log: bool = False, linear_thresh: t.Optional[float] = None) -> plt.axes:
     """
     Sets scale of x-axis
@@ -422,15 +423,17 @@
 
 
 def remove_tick_labels(ax: plt.axes, axis: str = "x"):
     """Remove ticks and tick labels for specified axis"""
     set_axis_tick_labels(ax=ax, values=[], labels=[], axis=axis)
 
 
-def save_figure(fig: plt.figure, filename: t.Union[str, pathlib.Path] = None, dpi: int = 450) -> None:
+def save_figure(
+    fig: a2.utils.constants.TYPE_MATPLOTLIB_FIGURES, filename: str | pathlib.Path | None = None, dpi: int = 450
+) -> None:
     """Save figure to filename"""
     if filename is not None:
         logging.info(f"... saving {filename}")
         folder = os.path.split(filename.__str__())[0]
         if folder:
             os.makedirs(folder, exist_ok=True)
         fig.savefig(filename, bbox_inches="tight", dpi=dpi)
```

### Comparing `a2-0.3.2/src/a2/plotting/weather_maps.py` & `a2-0.3.3/src/a2/plotting/weather_maps.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.2/src/a2/preprocess/embedding.py` & `a2-0.3.3/src/a2/preprocess/embedding.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.2/src/a2/preprocess/normalize_text.py` & `a2-0.3.3/src/a2/preprocess/normalize_text.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.2/src/a2/training/benchmarks.py` & `a2-0.3.3/src/a2/training/benchmarks.py`

 * *Files 8% similar despite different names*

```diff
@@ -72,33 +72,35 @@
                 f"counts: {len(times):>5}"
             )
             if self.debug:
                 for _type, elapsed_time in self.times_running.items():
                     logging.info(f"{_type} still running for {elapsed_time}s.")
 
 
-def get_max_memory_usage():
-    """In bytes"""
-    return resource.getrusage(resource.RUSAGE_SELF).ru_maxrss * 1000
-
-
-def init_cuda():
-    if torch.cuda.is_available():
-        torch.cuda.init()
-
-
-def reset_cuda_memory_monitoring():
-    for i_cuda in range(torch.cuda.device_count()):
-        torch.cuda.reset_peak_memory_stats(i_cuda)
-
-
-def get_cuda_memory_usage(log_message, style="verbose"):
-    logging.info("CUDA memory logging....\n")
-    for i_cuda in range(torch.cuda.device_count()):
-        logging.info(f"{log_message}: Cuda device {i_cuda}, {style} report:\n")
-        if style =="verbose":
+class CudaMemoryMonitor:
+    def __init__(self) -> None:
+        self.init_cuda()
+
+    def get_max_memory_usage(self):
+        """In bytes"""
+        return resource.getrusage(resource.RUSAGE_SELF).ru_maxrss * 1000
+
+    def init_cuda(self):
+        if torch.cuda.is_available():
+            torch.cuda.init()
+        else:
+            logging.info("Cuda initialization failed, as cuda is not available.")
+
+    def reset_cuda_memory_monitoring(self):
+        for i_cuda in range(torch.cuda.device_count()):
+            torch.cuda.reset_peak_memory_stats(i_cuda)
+
+    def get_cuda_memory_usage(self, log_message):
+        logging.info("CUDA memory logging....\n")
+        for i_cuda in range(torch.cuda.device_count()):
+            logging.info(f"{log_message}: Cuda device {i_cuda} report:\n")
             pprint.pprint(torch.cuda.memory_stats(i_cuda))
             logging.info(f"Report done! for Cuda device {i_cuda}\n")
-        logging.info(f"Gpu memory currently allocated: {torch.cuda.memory_allocated(i_cuda)/1e9} GB.")
-        logging.info(f"Gpu max memory allocated: {torch.cuda.max_memory_allocated(i_cuda)/1e9} GB.")
-        logging.info(f"Gpu memory currently reserved: {torch.cuda.memory_reserved(i_cuda)/1e9} GB.")
-        logging.info(f"Gpu max memory reserved: {torch.cuda.max_memory_reserved(i_cuda)/1e9} GB.")
+            logging.info(f"Gpu memory currently allocated: {torch.cuda.memory_allocated(i_cuda)/1e9} GB.")
+            logging.info(f"Gpu max memory allocated: {torch.cuda.max_memory_allocated(i_cuda)/1e9} GB.")
+            logging.info(f"Gpu memory currently reserved: {torch.cuda.memory_reserved(i_cuda)/1e9} GB.")
+            logging.info(f"Gpu max memory reserved: {torch.cuda.max_memory_reserved(i_cuda)/1e9} GB.")
```

### Comparing `a2-0.3.2/src/a2/training/dataset_hugging.py` & `a2-0.3.3/src/a2/training/dataset_hugging.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.2/src/a2/training/evaluate_hugging.py` & `a2-0.3.3/src/a2/training/evaluate_hugging.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.2/src/a2/training/tracking.py` & `a2-0.3.3/src/a2/training/tracking.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.2/src/a2/training/tracking_hugging.py` & `a2-0.3.3/src/a2/training/tracking_hugging.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.2/src/a2/training/training_deep500.py` & `a2-0.3.3/src/a2/training/training_deep500.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.2/src/a2/training/training_hugging.py` & `a2-0.3.3/src/a2/training/training_hugging.py`

 * *Files 16% similar despite different names*

```diff
@@ -219,28 +219,81 @@
     """
     Returns indices of training and validation set
 
     Parameters:
     ----------
     ds: Xarray dataset
     key_stratify: Stratified based on this key, `None` if not required
-    test_size: Fraction of validation set [0-1]
+    validation_size: Fraction of validation set; 1 - validation_size - test_size > 0
+    test_size: Fraction of test set; 1 - validation_size - test_size > 0
     random_state: Random seed to initialize selection
     shuffle: Whether or not to shuffle the data before splitting.
              If shuffle=False then stratify must be None.
 
     Returns
     -------
-    Indices of training and test set
+    Indices of training, validation and test set
     """
-    if key_stratify is None:
+    print(ds)
+
+    if key_stratify is not None:
         stratify = ds[key_stratify].values
     else:
         stratify = None
-    indices_train, indices_validate = sklearn.model_selection.train_test_split(
+    indices_train, indices_test = sklearn.model_selection.train_test_split(
         np.arange(ds[a2.dataset.utils_dataset.get_variable_name_first(ds)].shape[0]),
         test_size=test_size,
         random_state=random_state,
         shuffle=shuffle,
         stratify=stratify,
     )
-    return indices_train, indices_validate
+    return indices_train, indices_test
+
+
+def split_training_set_tripple(
+    ds: xarray.Dataset,
+    key_stratify: str = "raining",
+    validation_size: float | None = None,
+    test_size: float = 0.2,
+    random_state: int = 42,
+    shuffle: bool = True,
+):
+    """
+    Returns indices of training and validation set
+
+    Parameters:
+    ----------
+    ds: Xarray dataset
+    key_stratify: Stratified based on this key, `None` if not required
+    validation_size: Fraction of validation set; 1 - validation_size - test_size > 0
+    test_size: Fraction of test set; 1 - validation_size - test_size > 0
+    random_state: Random seed to initialize selection
+    shuffle: Whether or not to shuffle the data before splitting.
+             If shuffle=False then stratify must be None.
+
+    Returns
+    -------
+    Indices of training, validation and test set
+    """
+    ds = a2.dataset.load_dataset.reset_index_coordinate(ds.copy())
+    train_size = 1 - test_size
+    if validation_size is not None:
+        train_size -= validation_size
+    if train_size < 0:
+        raise ValueError(f"{train_size=} is below zero! (Decrease {validation_size=} and/or {test_size=})")
+    indices_train, indices_test = split_training_set(
+        ds=ds,
+        key_stratify=key_stratify,
+        test_size=test_size,
+        random_state=random_state,
+        shuffle=shuffle,
+    )
+    indices_validate = np.array([], dtype=int)
+    if validation_size is not None:
+        indices_train, indices_validate = split_training_set(
+            ds=ds.sel(index=indices_train),
+            key_stratify=key_stratify,
+            test_size=validation_size / (1 - test_size),
+            random_state=random_state,
+            shuffle=shuffle,
+        )
+    return indices_train, indices_validate, indices_test
```

### Comparing `a2-0.3.2/src/a2/twitter/downloader.py` & `a2-0.3.3/src/a2/twitter/downloader.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.2/src/a2/twitter/locations.py` & `a2-0.3.3/src/a2/twitter/locations.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.2/src/a2/twitter/twitter_api.py` & `a2-0.3.3/src/a2/twitter/twitter_api.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.2/src/a2/utils/checks.py` & `a2-0.3.3/src/a2/utils/checks.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.2/src/a2/utils/file_handling.py` & `a2-0.3.3/src/a2/utils/file_handling.py`

 * *Files 2% similar despite different names*

```diff
@@ -291,17 +291,17 @@
         print(f"User cannot write {description} {file_or_folder}")
     if os.access(file_or_folder, os.R_OK):
         print(f"User can read {description} {file_or_folder}")
     else:
         print(f"User cannot read {description} {file_or_folder}")
 
 
-def check_folder_exists(path, check_is_empty=False, raise_exception=False):
+def folder_exists(path: str | pathlib.Path, check_if_empty: bool = False, raise_exception: bool = False) -> bool:
     if not os.path.isdir(path):
         if raise_exception:
             raise ValueError(f"{path=} doesn't exist!")
         return False
-    if check_is_empty and os.path.getsize(path) <= 4096:
+    if check_if_empty and os.path.getsize(path) <= 4096:
         if raise_exception:
             raise ValueError(f"{path=} is empty!")
         return False
     return True
```

### Comparing `a2-0.3.2/src/a2/utils/testing.py` & `a2-0.3.3/src/a2/utils/testing.py`

 * *Files identical despite different names*

### Comparing `a2-0.3.2/src/a2/utils/utils.py` & `a2-0.3.3/src/a2/utils/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,25 +154,25 @@
         for v, typ in zip(variable, type_from_variable):
             _assert_same_type(v, typ)
     else:
         if not isinstance(variable, type(type_from_variable)):
             raise TypeError(f"Variable {variable=} different type than expected {type_from_variable=}")
 
 
-def assert_same_type_as(variable, type_from_variable, alternative=None):
+def assert_same_type_as(variable: object, type_from_variable: object, alternative: object = None):
     """Check if `variable` is same type as `type_from_variable` unless `variable` is `alternative`"""
     if variable is alternative:
         return
     try:
         _assert_same_type(variable, type_from_variable)
     except TypeError:
         raise TypeError(f"Variable {variable} not of expected type {type_from_variable}")
 
 
-def all_same_type(variable_list, type_):
+def all_same_type(variable_list: t.Iterable, type_: type):
     for var in variable_list:
         if not isinstance(var, type_):
             raise ValueError(f"{var} not of type {type_.__name__}!")
 
 
 def assert_shape(variable, shape: t.Tuple, name: str = None, ignore_none: bool = True):
     if ignore_none:
```

### Comparing `a2-0.3.2/PKG-INFO` & `a2-0.3.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,46 +1,43 @@
 Metadata-Version: 2.1
 Name: a2
-Version: 0.3.2
+Version: 0.3.3
 Summary: Package for predicting information about the weather from social media data as application 2 for maelstrom project
 Author: Kristian Ehlert
 Author-email: kristian.ehlert@4-cast.de
 Requires-Python: >=3.10,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Provides-Extra: llama-chatbot
-Provides-Extra: torch
+Provides-Extra: extend-exclude
 Requires-Dist: DateTime (>=4.4,<5.0)
 Requires-Dist: Shapely (>=1.8.2,<2.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: convertbng (>=0.6.39,<0.7.0)
 Requires-Dist: dask (>=2022.6.1,<2023.0.0)
-Requires-Dist: datasets (>=2.11.0,<3.0.0)
 Requires-Dist: emoji (<1.0.0)
 Requires-Dist: geopy (>=2.3.0,<3.0.0)
 Requires-Dist: h5netcdf (>=1.0.1,<2.0.0)
 Requires-Dist: h5py (>=3.7.0,<4.0.0)
 Requires-Dist: ipython (>=8.7.0,<9.0.0)
 Requires-Dist: ipywidgets (>=7.7.1,<8.0.0)
 Requires-Dist: jsonlines (>=3.1.0,<4.0.0)
 Requires-Dist: jupyterlab (>=3.4.3,<4.0.0)
 Requires-Dist: kaleido (==0.2.1)
-Requires-Dist: llvmlite (>=0.39.1,<0.40.0)
 Requires-Dist: mantik (>=0.1.0,<0.2.0)
 Requires-Dist: matplotlib (>=3.5.2,<4.0.0)
 Requires-Dist: netCDF4 (>=1.6.0,<2.0.0)
 Requires-Dist: pandas (>=1.4.2,<2.0.0)
 Requires-Dist: plotly (>=5.11.0,<6.0.0)
 Requires-Dist: pyproj (>=3.3.1,<4.0.0)
+Requires-Dist: pytest-recording (>=0.12.1,<0.13.0)
+Requires-Dist: pytest-xdist (>=2.5.0,<3.0.0)
 Requires-Dist: rasterio (>=1.3.3,<2.0.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Requires-Dist: rioxarray (>=0.12.2,<0.13.0)
 Requires-Dist: scikit-learn (>=1.1.2,<2.0.0)
 Requires-Dist: seaborn (>=0.12.1,<0.13.0)
-Requires-Dist: sentencepiece (>=0.1.98,<0.2.0) ; extra == "llama-chatbot"
 Requires-Dist: spacymoji (>=3.0.1,<4.0.0)
-Requires-Dist: torch (>=2.0.0,<3.0.0) ; extra == "torch"
 Requires-Dist: tweepy (>=4.10.0,<5.0.0)
 Requires-Dist: urllib3 (>=1.26.12,<2.0.0)
 Requires-Dist: wget (>=3.2,<4.0)
 Requires-Dist: xarray (>=2022.3.0,<2023.0.0)
```

