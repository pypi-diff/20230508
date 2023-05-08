# Comparing `tmp/finance_ml-0.0.3.tar.gz` & `tmp/finance_ml-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\finance_ml-0.0.3.tar", last modified: Mon May  8 01:13:20 2023, max compression
+gzip compressed data, was "dist\finance_ml-0.0.4.tar", last modified: Mon May  8 02:23:46 2023, max compression
```

## Comparing `finance_ml-0.0.3.tar` & `finance_ml-0.0.4.tar`

### file list

```diff
@@ -1,29 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 01:13:20.000000 finance_ml-0.0.3/
--rw-rw-rw-   0        0        0     3259 2023-05-07 18:26:13.000000 finance_ml-0.0.3/.gitignore
--rw-rw-rw-   0        0        0        0 2023-05-06 16:37:21.000000 finance_ml-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      603 2023-05-08 01:13:20.000000 finance_ml-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       45 2023-05-06 16:43:18.000000 finance_ml-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-08 01:13:20.000000 finance_ml-0.0.3/dist/
--rw-rw-rw-   0        0        0     2589 2023-05-08 01:12:45.000000 finance_ml-0.0.3/dist/finance_ml-0.0.2-py3-none-any.whl
--rw-rw-rw-   0        0        0    10041 2023-05-08 01:12:44.000000 finance_ml-0.0.3/dist/finance_ml-0.0.2.tar.gz
-drwxrwxrwx   0        0        0        0 2023-05-08 01:13:20.000000 finance_ml-0.0.3/finance_ml.egg-info/
--rw-rw-rw-   0        0        0      556 2023-05-06 18:41:27.000000 finance_ml-0.0.3/finance_ml.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      267 2023-05-06 18:41:27.000000 finance_ml-0.0.3/finance_ml.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 18:41:27.000000 finance_ml-0.0.3/finance_ml.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-05-06 18:41:27.000000 finance_ml-0.0.3/finance_ml.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 18:41:27.000000 finance_ml-0.0.3/finance_ml.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-08 01:13:20.000000 finance_ml-0.0.3/notebooks/
--rw-rw-rw-   0        0        0    16037 2023-05-08 01:10:05.000000 finance_ml-0.0.3/notebooks/module_testing.ipynb
--rw-rw-rw-   0        0        0      201 2023-05-06 16:37:21.000000 finance_ml-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-08 01:13:20.000000 finance_ml-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1138 2023-05-08 01:13:14.000000 finance_ml-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-08 01:13:20.000000 finance_ml-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-05-08 01:13:20.000000 finance_ml-0.0.3/src/finance_ml/
--rw-rw-rw-   0        0        0       39 2023-05-06 19:18:52.000000 finance_ml-0.0.3/src/finance_ml/__init__.py
--rw-rw-rw-   0        0        0     2383 2023-05-08 01:10:08.000000 finance_ml-0.0.3/src/finance_ml/dataprep_ml.py
-drwxrwxrwx   0        0        0        0 2023-05-08 01:13:20.000000 finance_ml-0.0.3/src/finance_ml.egg-info/
--rw-rw-rw-   0        0        0      603 2023-05-08 01:13:19.000000 finance_ml-0.0.3/src/finance_ml.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      566 2023-05-08 01:13:20.000000 finance_ml-0.0.3/src/finance_ml.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 01:13:19.000000 finance_ml-0.0.3/src/finance_ml.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-05-08 01:13:19.000000 finance_ml-0.0.3/src/finance_ml.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-08 01:13:19.000000 finance_ml-0.0.3/src/finance_ml.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-08 02:23:46.000000 finance_ml-0.0.4/
+-rw-rw-rw-   0        0        0     3259 2023-05-07 18:26:13.000000 finance_ml-0.0.4/.gitignore
+-rw-rw-rw-   0        0        0        0 2023-05-06 16:37:21.000000 finance_ml-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      603 2023-05-08 02:23:46.000000 finance_ml-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       45 2023-05-06 16:43:18.000000 finance_ml-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-08 02:23:46.000000 finance_ml-0.0.4/finance_ml.egg-info/
+-rw-rw-rw-   0        0        0      556 2023-05-06 18:41:27.000000 finance_ml-0.0.4/finance_ml.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      267 2023-05-06 18:41:27.000000 finance_ml-0.0.4/finance_ml.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 18:41:27.000000 finance_ml-0.0.4/finance_ml.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-05-06 18:41:27.000000 finance_ml-0.0.4/finance_ml.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 18:41:27.000000 finance_ml-0.0.4/finance_ml.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-08 02:23:46.000000 finance_ml-0.0.4/notebooks/
+-rw-rw-rw-   0        0        0    25218 2023-05-08 02:15:25.000000 finance_ml-0.0.4/notebooks/module_testing.ipynb
+-rw-rw-rw-   0        0        0      201 2023-05-06 16:37:21.000000 finance_ml-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-08 02:23:46.000000 finance_ml-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1138 2023-05-08 02:23:33.000000 finance_ml-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 02:23:46.000000 finance_ml-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-05-08 02:23:46.000000 finance_ml-0.0.4/src/finance_ml/
+-rw-rw-rw-   0        0        0       39 2023-05-06 19:18:52.000000 finance_ml-0.0.4/src/finance_ml/__init__.py
+-rw-rw-rw-   0        0        0     3185 2023-05-08 02:20:23.000000 finance_ml-0.0.4/src/finance_ml/dataprep_ml.py
+drwxrwxrwx   0        0        0        0 2023-05-08 02:23:46.000000 finance_ml-0.0.4/src/finance_ml.egg-info/
+-rw-rw-rw-   0        0        0      603 2023-05-08 02:23:46.000000 finance_ml-0.0.4/src/finance_ml.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      498 2023-05-08 02:23:46.000000 finance_ml-0.0.4/src/finance_ml.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 02:23:46.000000 finance_ml-0.0.4/src/finance_ml.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-05-08 02:23:46.000000 finance_ml-0.0.4/src/finance_ml.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-08 02:23:46.000000 finance_ml-0.0.4/src/finance_ml.egg-info/top_level.txt
```

### Comparing `finance_ml-0.0.3/.gitignore` & `finance_ml-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `finance_ml-0.0.3/PKG-INFO` & `finance_ml-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finance_ml
-Version: 0.0.3
+Version: 0.0.4
 Summary: Application of Machine Learning in Finances
 Author: Fabio Maia
 Author-email: <fabio.masaracchia@gmail.com>
 Keywords: python,finance,mlops
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `finance_ml-0.0.3/finance_ml.egg-info/PKG-INFO` & `finance_ml-0.0.4/finance_ml.egg-info/PKG-INFO`

 * *Files identical despite different names*

### Comparing `finance_ml-0.0.3/notebooks/module_testing.ipynb` & `finance_ml-0.0.4/notebooks/module_testing.ipynb`

 * *Files 23% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9312251814601439%*

 * *Differences: {"'cells'": "{0: {'execution_count': 7, 'id': '33d37f49'}, 1: {'execution_count': 8, 'id': "*

 * *            "'bf9ea3d0', 'outputs': {0: {'execution_count': 8}}}, 4: {'execution_count': 9, 'id': "*

 * *            '\'84e64650\', \'source\': ["dataloader = dataprep_ml.DataLoader(time_index_col= '*

 * *            "'DATE', keep_cols = ['VOLUME','OPEN', 'CLOSE', 'HIGH', 'LOW', "*

 * *            '\'TRANSACTIONS\'])\\n", "# dataloader = DataLoader(time_index_col= \'DATE\', '*

 * *            'keep_cols = [\'VOLUME\',\'OPEN\', \'CLOSE\ […]*

```diff
@@ -1,60 +1,320 @@
 {
     "cells": [
         {
             "cell_type": "code",
-            "execution_count": 108,
-            "id": "f9416adb",
+            "execution_count": 7,
+            "id": "33d37f49",
             "metadata": {},
             "outputs": [],
             "source": [
                 "import sys\n",
                 "import os\n",
                 "import pandas as pd\n",
                 "sys.path.append(os.path.abspath(os.path.join(os.getcwd(), os.pardir)))"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 109,
-            "id": "0f1782b1",
+            "execution_count": 8,
+            "id": "bf9ea3d0",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "<module 'src.finance_ml.dataprep_ml' from 'C:\\\\Users\\\\fabio\\\\OneDrive\\\\\u00c1rea de Trabalho\\\\Mestrado\\\\MAP5922\\\\Dev\\\\finance_ml\\\\src\\\\finance_ml\\\\dataprep_ml.py'>"
                         ]
                     },
-                    "execution_count": 109,
+                    "execution_count": 8,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "from src.finance_ml import dataprep_ml\n",
                 "\n",
                 "import importlib\n",
                 "importlib.reload(dataprep_ml)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 110,
-            "id": "9a9a3859",
+            "execution_count": null,
+            "id": "786dde6e",
             "metadata": {},
             "outputs": [],
             "source": [
-                "dataloader = dataprep_ml.DataLoader(time_index_col= 'DATE', keep_cols = ['VOLUME','OPEN', 'CLOSE'])"
+                "# !pip install finance-ml"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 111,
-            "id": "cf308df0",
+            "execution_count": 3,
+            "id": "4c3adfcd",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# from finance_ml.dataprep_ml import DataLoader"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 9,
+            "id": "84e64650",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "dataloader = dataprep_ml.DataLoader(time_index_col= 'DATE', keep_cols = ['VOLUME','OPEN', 'CLOSE', 'HIGH', 'LOW', 'TRANSACTIONS'])\n",
+                "# dataloader = DataLoader(time_index_col= 'DATE', keep_cols = ['VOLUME','OPEN', 'CLOSE'])"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 12,
+            "id": "ec23f6d0",
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "text/html": [
+                            "<div>\n",
+                            "<style scoped>\n",
+                            "    .dataframe tbody tr th:only-of-type {\n",
+                            "        vertical-align: middle;\n",
+                            "    }\n",
+                            "\n",
+                            "    .dataframe tbody tr th {\n",
+                            "        vertical-align: top;\n",
+                            "    }\n",
+                            "\n",
+                            "    .dataframe thead th {\n",
+                            "        text-align: right;\n",
+                            "    }\n",
+                            "</style>\n",
+                            "<table border=\"1\" class=\"dataframe\">\n",
+                            "  <thead>\n",
+                            "    <tr style=\"text-align: right;\">\n",
+                            "      <th></th>\n",
+                            "      <th>VOLUME</th>\n",
+                            "      <th>VW</th>\n",
+                            "      <th>OPEN</th>\n",
+                            "      <th>CLOSE</th>\n",
+                            "      <th>HIGHT</th>\n",
+                            "      <th>LOW</th>\n",
+                            "      <th>t</th>\n",
+                            "      <th>TRANSACTIONS</th>\n",
+                            "      <th>a</th>\n",
+                            "      <th>op</th>\n",
+                            "      <th>DATE</th>\n",
+                            "    </tr>\n",
+                            "  </thead>\n",
+                            "  <tbody>\n",
+                            "    <tr>\n",
+                            "      <th>0</th>\n",
+                            "      <td>21071.0</td>\n",
+                            "      <td>155.9052</td>\n",
+                            "      <td>155.880</td>\n",
+                            "      <td>155.9260</td>\n",
+                            "      <td>155.94</td>\n",
+                            "      <td>155.8600</td>\n",
+                            "      <td>1586274180000</td>\n",
+                            "      <td>152.0</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>2020-04-07 15:43:00</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>1</th>\n",
+                            "      <td>23010.0</td>\n",
+                            "      <td>155.9342</td>\n",
+                            "      <td>155.930</td>\n",
+                            "      <td>155.9000</td>\n",
+                            "      <td>155.97</td>\n",
+                            "      <td>155.9000</td>\n",
+                            "      <td>1586274240000</td>\n",
+                            "      <td>165.0</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>2020-04-07 15:44:00</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>2</th>\n",
+                            "      <td>31544.0</td>\n",
+                            "      <td>155.8012</td>\n",
+                            "      <td>155.920</td>\n",
+                            "      <td>155.7350</td>\n",
+                            "      <td>155.94</td>\n",
+                            "      <td>155.7200</td>\n",
+                            "      <td>1586274300000</td>\n",
+                            "      <td>292.0</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>2020-04-07 15:45:00</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>3</th>\n",
+                            "      <td>42645.0</td>\n",
+                            "      <td>155.7910</td>\n",
+                            "      <td>155.760</td>\n",
+                            "      <td>155.8400</td>\n",
+                            "      <td>155.84</td>\n",
+                            "      <td>155.7600</td>\n",
+                            "      <td>1586274360000</td>\n",
+                            "      <td>153.0</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>2020-04-07 15:46:00</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>4</th>\n",
+                            "      <td>3735.0</td>\n",
+                            "      <td>155.8070</td>\n",
+                            "      <td>155.805</td>\n",
+                            "      <td>155.8100</td>\n",
+                            "      <td>155.82</td>\n",
+                            "      <td>155.7950</td>\n",
+                            "      <td>1586274420000</td>\n",
+                            "      <td>47.0</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>2020-04-07 15:47:00</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>...</th>\n",
+                            "      <td>...</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>...</td>\n",
+                            "      <td>...</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>279473</th>\n",
+                            "      <td>600.0</td>\n",
+                            "      <td>179.5100</td>\n",
+                            "      <td>179.510</td>\n",
+                            "      <td>179.5100</td>\n",
+                            "      <td>179.51</td>\n",
+                            "      <td>179.5100</td>\n",
+                            "      <td>1649287620000</td>\n",
+                            "      <td>1.0</td>\n",
+                            "      <td>179.6537</td>\n",
+                            "      <td>179.78</td>\n",
+                            "      <td>2022-04-06 23:27:00</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>279474</th>\n",
+                            "      <td>3033.0</td>\n",
+                            "      <td>179.4004</td>\n",
+                            "      <td>179.410</td>\n",
+                            "      <td>179.4000</td>\n",
+                            "      <td>179.41</td>\n",
+                            "      <td>179.4000</td>\n",
+                            "      <td>1649288100000</td>\n",
+                            "      <td>8.0</td>\n",
+                            "      <td>179.6536</td>\n",
+                            "      <td>179.78</td>\n",
+                            "      <td>2022-04-06 23:35:00</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>279475</th>\n",
+                            "      <td>393.0</td>\n",
+                            "      <td>179.4000</td>\n",
+                            "      <td>179.400</td>\n",
+                            "      <td>179.4000</td>\n",
+                            "      <td>179.40</td>\n",
+                            "      <td>179.4000</td>\n",
+                            "      <td>1649288160000</td>\n",
+                            "      <td>4.0</td>\n",
+                            "      <td>179.6536</td>\n",
+                            "      <td>179.78</td>\n",
+                            "      <td>2022-04-06 23:36:00</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>279476</th>\n",
+                            "      <td>100.0</td>\n",
+                            "      <td>179.5700</td>\n",
+                            "      <td>179.570</td>\n",
+                            "      <td>179.5700</td>\n",
+                            "      <td>179.57</td>\n",
+                            "      <td>179.5700</td>\n",
+                            "      <td>1649289000000</td>\n",
+                            "      <td>1.0</td>\n",
+                            "      <td>179.6536</td>\n",
+                            "      <td>179.78</td>\n",
+                            "      <td>2022-04-06 23:50:00</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>279477</th>\n",
+                            "      <td>204.0</td>\n",
+                            "      <td>179.5396</td>\n",
+                            "      <td>179.540</td>\n",
+                            "      <td>179.5399</td>\n",
+                            "      <td>179.54</td>\n",
+                            "      <td>179.5399</td>\n",
+                            "      <td>1649289240000</td>\n",
+                            "      <td>3.0</td>\n",
+                            "      <td>179.6536</td>\n",
+                            "      <td>179.78</td>\n",
+                            "      <td>2022-04-06 23:54:00</td>\n",
+                            "    </tr>\n",
+                            "  </tbody>\n",
+                            "</table>\n",
+                            "<p>279478 rows \u00d7 11 columns</p>\n",
+                            "</div>"
+                        ],
+                        "text/plain": [
+                            "         VOLUME        VW     OPEN     CLOSE   HIGHT       LOW              t  \\\n",
+                            "0       21071.0  155.9052  155.880  155.9260  155.94  155.8600  1586274180000   \n",
+                            "1       23010.0  155.9342  155.930  155.9000  155.97  155.9000  1586274240000   \n",
+                            "2       31544.0  155.8012  155.920  155.7350  155.94  155.7200  1586274300000   \n",
+                            "3       42645.0  155.7910  155.760  155.8400  155.84  155.7600  1586274360000   \n",
+                            "4        3735.0  155.8070  155.805  155.8100  155.82  155.7950  1586274420000   \n",
+                            "...         ...       ...      ...       ...     ...       ...            ...   \n",
+                            "279473    600.0  179.5100  179.510  179.5100  179.51  179.5100  1649287620000   \n",
+                            "279474   3033.0  179.4004  179.410  179.4000  179.41  179.4000  1649288100000   \n",
+                            "279475    393.0  179.4000  179.400  179.4000  179.40  179.4000  1649288160000   \n",
+                            "279476    100.0  179.5700  179.570  179.5700  179.57  179.5700  1649289000000   \n",
+                            "279477    204.0  179.5396  179.540  179.5399  179.54  179.5399  1649289240000   \n",
+                            "\n",
+                            "        TRANSACTIONS         a      op                DATE  \n",
+                            "0              152.0       NaN     NaN 2020-04-07 15:43:00  \n",
+                            "1              165.0       NaN     NaN 2020-04-07 15:44:00  \n",
+                            "2              292.0       NaN     NaN 2020-04-07 15:45:00  \n",
+                            "3              153.0       NaN     NaN 2020-04-07 15:46:00  \n",
+                            "4               47.0       NaN     NaN 2020-04-07 15:47:00  \n",
+                            "...              ...       ...     ...                 ...  \n",
+                            "279473           1.0  179.6537  179.78 2022-04-06 23:27:00  \n",
+                            "279474           8.0  179.6536  179.78 2022-04-06 23:35:00  \n",
+                            "279475           4.0  179.6536  179.78 2022-04-06 23:36:00  \n",
+                            "279476           1.0  179.6536  179.78 2022-04-06 23:50:00  \n",
+                            "279477           3.0  179.6536  179.78 2022-04-06 23:54:00  \n",
+                            "\n",
+                            "[279478 rows x 11 columns]"
+                        ]
+                    },
+                    "execution_count": 12,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "pd.read_parquet('../data/commodities/GLD_2020-04-07_2022-04-06.parquet', engine='pyarrow')"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 10,
+            "id": "971ddebe",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
                             "<style scoped>\n",
@@ -89,163 +349,163 @@
                             "      <th></th>\n",
                             "      <th></th>\n",
                             "      <th></th>\n",
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
-                            "      <th>2020-04-07 17:48:00</th>\n",
-                            "      <td>6498.0</td>\n",
-                            "      <td>154.8500</td>\n",
-                            "      <td>154.8200</td>\n",
-                            "      <td>15.835240</td>\n",
-                            "      <td>7363.09</td>\n",
-                            "      <td>7352.66</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>2020-04-07 17:49:00</th>\n",
-                            "      <td>11244.0</td>\n",
-                            "      <td>154.8200</td>\n",
-                            "      <td>154.7700</td>\n",
-                            "      <td>7.652123</td>\n",
-                            "      <td>7358.42</td>\n",
-                            "      <td>7361.54</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>2020-04-07 17:50:00</th>\n",
-                            "      <td>26288.0</td>\n",
-                            "      <td>154.7711</td>\n",
-                            "      <td>154.7285</td>\n",
-                            "      <td>16.446123</td>\n",
-                            "      <td>7361.54</td>\n",
-                            "      <td>7354.09</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>2020-04-07 17:51:00</th>\n",
-                            "      <td>6961.0</td>\n",
-                            "      <td>154.7300</td>\n",
-                            "      <td>154.7467</td>\n",
-                            "      <td>7.068813</td>\n",
-                            "      <td>7354.14</td>\n",
-                            "      <td>7345.00</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>2020-04-07 17:52:00</th>\n",
-                            "      <td>14951.0</td>\n",
-                            "      <td>154.7400</td>\n",
-                            "      <td>154.8300</td>\n",
-                            "      <td>8.162850</td>\n",
-                            "      <td>7350.10</td>\n",
-                            "      <td>7355.16</td>\n",
+                            "      <th>2020-04-07 15:43:00</th>\n",
+                            "      <td>21071.0</td>\n",
+                            "      <td>155.880</td>\n",
+                            "      <td>155.9260</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>2020-04-07 15:44:00</th>\n",
+                            "      <td>23010.0</td>\n",
+                            "      <td>155.930</td>\n",
+                            "      <td>155.9000</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>2020-04-07 15:45:00</th>\n",
+                            "      <td>31544.0</td>\n",
+                            "      <td>155.920</td>\n",
+                            "      <td>155.7350</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>2020-04-07 15:46:00</th>\n",
+                            "      <td>42645.0</td>\n",
+                            "      <td>155.760</td>\n",
+                            "      <td>155.8400</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>2020-04-07 15:47:00</th>\n",
+                            "      <td>3735.0</td>\n",
+                            "      <td>155.805</td>\n",
+                            "      <td>155.8100</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>...</th>\n",
                             "      <td>...</td>\n",
                             "      <td>...</td>\n",
                             "      <td>...</td>\n",
                             "      <td>...</td>\n",
                             "      <td>...</td>\n",
                             "      <td>...</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>2022-04-06 23:36:00</th>\n",
-                            "      <td>393.0</td>\n",
-                            "      <td>179.4000</td>\n",
-                            "      <td>179.4000</td>\n",
-                            "      <td>16.400271</td>\n",
-                            "      <td>43329.27</td>\n",
-                            "      <td>43290.72</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>2022-04-06 23:50:00</th>\n",
-                            "      <td>100.0</td>\n",
-                            "      <td>179.5700</td>\n",
-                            "      <td>179.5700</td>\n",
-                            "      <td>18.054926</td>\n",
-                            "      <td>43295.56</td>\n",
-                            "      <td>43252.21</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>2022-04-06 23:50:00</th>\n",
-                            "      <td>100.0</td>\n",
-                            "      <td>179.5700</td>\n",
-                            "      <td>179.5700</td>\n",
-                            "      <td>18.054926</td>\n",
-                            "      <td>43295.56</td>\n",
-                            "      <td>43252.21</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
                             "      <th>2022-04-06 23:54:00</th>\n",
                             "      <td>204.0</td>\n",
-                            "      <td>179.5400</td>\n",
+                            "      <td>179.540</td>\n",
                             "      <td>179.5399</td>\n",
                             "      <td>37.006803</td>\n",
                             "      <td>43146.71</td>\n",
                             "      <td>43144.08</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>2022-04-06 23:54:00</th>\n",
-                            "      <td>204.0</td>\n",
-                            "      <td>179.5400</td>\n",
-                            "      <td>179.5399</td>\n",
-                            "      <td>37.006803</td>\n",
-                            "      <td>43146.71</td>\n",
+                            "      <th>2022-04-06 23:55:00</th>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>65.685080</td>\n",
                             "      <td>43144.08</td>\n",
+                            "      <td>43188.59</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>2022-04-06 23:56:00</th>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>25.763792</td>\n",
+                            "      <td>43188.44</td>\n",
+                            "      <td>43111.80</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>2022-04-06 23:57:00</th>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>21.241159</td>\n",
+                            "      <td>43122.93</td>\n",
+                            "      <td>43149.90</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>2022-04-06 23:58:00</th>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>NaN</td>\n",
+                            "      <td>120.336717</td>\n",
+                            "      <td>43146.69</td>\n",
+                            "      <td>43173.96</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
-                            "<p>278901 rows \u00d7 6 columns</p>\n",
+                            "<p>1051079 rows \u00d7 6 columns</p>\n",
                             "</div>"
                         ],
                         "text/plain": [
                             "                     GOLD_VOLUME  GOLD_OPEN  GOLD_CLOSE  BITCOINS_VOLUME  \\\n",
                             "DATE                                                                       \n",
-                            "2020-04-07 17:48:00       6498.0   154.8500    154.8200        15.835240   \n",
-                            "2020-04-07 17:49:00      11244.0   154.8200    154.7700         7.652123   \n",
-                            "2020-04-07 17:50:00      26288.0   154.7711    154.7285        16.446123   \n",
-                            "2020-04-07 17:51:00       6961.0   154.7300    154.7467         7.068813   \n",
-                            "2020-04-07 17:52:00      14951.0   154.7400    154.8300         8.162850   \n",
+                            "2020-04-07 15:43:00      21071.0    155.880    155.9260              NaN   \n",
+                            "2020-04-07 15:44:00      23010.0    155.930    155.9000              NaN   \n",
+                            "2020-04-07 15:45:00      31544.0    155.920    155.7350              NaN   \n",
+                            "2020-04-07 15:46:00      42645.0    155.760    155.8400              NaN   \n",
+                            "2020-04-07 15:47:00       3735.0    155.805    155.8100              NaN   \n",
                             "...                          ...        ...         ...              ...   \n",
-                            "2022-04-06 23:36:00        393.0   179.4000    179.4000        16.400271   \n",
-                            "2022-04-06 23:50:00        100.0   179.5700    179.5700        18.054926   \n",
-                            "2022-04-06 23:50:00        100.0   179.5700    179.5700        18.054926   \n",
-                            "2022-04-06 23:54:00        204.0   179.5400    179.5399        37.006803   \n",
-                            "2022-04-06 23:54:00        204.0   179.5400    179.5399        37.006803   \n",
+                            "2022-04-06 23:54:00        204.0    179.540    179.5399        37.006803   \n",
+                            "2022-04-06 23:55:00          NaN        NaN         NaN        65.685080   \n",
+                            "2022-04-06 23:56:00          NaN        NaN         NaN        25.763792   \n",
+                            "2022-04-06 23:57:00          NaN        NaN         NaN        21.241159   \n",
+                            "2022-04-06 23:58:00          NaN        NaN         NaN       120.336717   \n",
                             "\n",
                             "                     BITCOINS_OPEN  BITCOINS_CLOSE  \n",
                             "DATE                                                \n",
-                            "2020-04-07 17:48:00        7363.09         7352.66  \n",
-                            "2020-04-07 17:49:00        7358.42         7361.54  \n",
-                            "2020-04-07 17:50:00        7361.54         7354.09  \n",
-                            "2020-04-07 17:51:00        7354.14         7345.00  \n",
-                            "2020-04-07 17:52:00        7350.10         7355.16  \n",
+                            "2020-04-07 15:43:00            NaN             NaN  \n",
+                            "2020-04-07 15:44:00            NaN             NaN  \n",
+                            "2020-04-07 15:45:00            NaN             NaN  \n",
+                            "2020-04-07 15:46:00            NaN             NaN  \n",
+                            "2020-04-07 15:47:00            NaN             NaN  \n",
                             "...                            ...             ...  \n",
-                            "2022-04-06 23:36:00       43329.27        43290.72  \n",
-                            "2022-04-06 23:50:00       43295.56        43252.21  \n",
-                            "2022-04-06 23:50:00       43295.56        43252.21  \n",
-                            "2022-04-06 23:54:00       43146.71        43144.08  \n",
                             "2022-04-06 23:54:00       43146.71        43144.08  \n",
+                            "2022-04-06 23:55:00       43144.08        43188.59  \n",
+                            "2022-04-06 23:56:00       43188.44        43111.80  \n",
+                            "2022-04-06 23:57:00       43122.93        43149.90  \n",
+                            "2022-04-06 23:58:00       43146.69        43173.96  \n",
                             "\n",
-                            "[278901 rows x 6 columns]"
+                            "[1051079 rows x 6 columns]"
                         ]
                     },
-                    "execution_count": 111,
+                    "execution_count": 10,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "dataloader.load_dataset({'GOLD':'../data/commodities/GLD_2020-04-07_2022-04-06.parquet',\n",
                 "                        'BITCOINS':'../data/cryptos/BTCUSD_2020-04-07_2022-04-06.parquet'})"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 113,
-            "id": "88e6763d",
+            "execution_count": 11,
+            "id": "4d94ae99",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
                             "<style scoped>\n",
@@ -426,22 +686,30 @@
                             "2022-04-04         1440.0  \n",
                             "2022-04-05         1439.0  \n",
                             "2022-04-06         1439.0  \n",
                             "\n",
                             "[730 rows x 6 columns]"
                         ]
                     },
-                    "execution_count": 113,
+                    "execution_count": 11,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "dataloader.tablefreq"
             ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "97da764e",
+            "metadata": {},
+            "outputs": [],
+            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3",
             "language": "python",
             "name": "python3"
```

### Comparing `finance_ml-0.0.3/setup.py` & `finance_ml-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 DESCRIPTION = 'Application of Machine Learning in Finances'
 LONG_DESCRIPTION = 'A package that allows you to build pipelines and evaluate trading strategies, resulting in instructions to operate in the market.'
 
 
 with open("README.md", "r") as f:
     long_description = f.read()
```

### Comparing `finance_ml-0.0.3/src/finance_ml/dataprep_ml.py` & `finance_ml-0.0.4/src/finance_ml/dataprep_ml.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,25 +2,40 @@
 
 def print_test():
     print('hello world!')
 
 class DataLoader():
     
     def __init__(self, 
-                 time_index_col,
-                 keep_cols, 
-                 join_dfs= True):
+                 time_index_col:str,
+                 keep_cols:list):
         
         self.keep_cols = keep_cols
         self.time_index_col = time_index_col
 
-    def guess_format(self, path_file):
+    def guess_format(self, 
+                     path_file:str)->str:
         return path_file.split('.')[-1].lower()
         
-    def load_dataset(self,path_files):
+    def load_dataset(self,
+                     path_files:dict)->pd.DataFrame:
+        
+        '''    
+        Retorna todas databases unificadas indexadas pelo timestamp 
+        
+        Args:        
+        -----            
+        path_files: dict 
+            Dicionário contendo como chave os tags utilizado como prefixos da tabela e como valor o respectivo caminho do arquivo.        
+            
+        Returns: 
+        -----
+        dataset: pandas DataFrame       
+            Base unificada contendo todas referências passadas como argumento.
+        '''
 
         self.tablefreq = pd.DataFrame()
 
         dataset = pd.DataFrame()
         assert isinstance(path_files, dict),'path_file must be dictionary which keys are tags and values are file paths'
 
         for i, (tag, path) in enumerate(path_files.items()):
@@ -35,28 +50,34 @@
                 df_ = df_[self.keep_cols]
                 self.tablefreq = pd.merge(self.tablefreq,
                                           self.raw_database_tablefreq(df_).add_prefix(tag+ '_'),
                                           left_index= True,
                                           right_index=True,
                                           how='outer')
                 df_ = df_.add_prefix(tag+ '_')
-                dataset = dataset.merge(df_, right_index=True, left_index=True,)
+                dataset = dataset.merge(df_, 
+                                        right_index=True, 
+                                        left_index=True,
+                                        how='outer')
                 
         return dataset
 
-    def file_read(self, path_file, format) -> pd.DataFrame:
+    def file_read(self, 
+                  path_file:str, 
+                  format:str) -> pd.DataFrame:
         assert format in ['parquet', 'csv', 'excel'], 'Format must be "parquet", "csv", "xlsx"'
 
         if format =='parquet':
             df = pd.read_parquet(path_file, engine='pyarrow')
             df[self.time_index_col] = pd.to_datetime(df[self.time_index_col])
             df.set_index(self.time_index_col, inplace=True)
         return df
 
-    def raw_database_tablefreq(self, df):
+    def raw_database_tablefreq(self,
+                                df:pd.DataFrame)->pd.DataFrame:
         tablefreq = df.copy()
         tablefreq['date'] = tablefreq.index.date
         tablefreq['time'] = tablefreq.index.time
         tablefreq = tablefreq.groupby('date').agg({'time':['min', 'max','count']})
         return tablefreq
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `finance_ml-0.0.3/src/finance_ml.egg-info/PKG-INFO` & `finance_ml-0.0.4/src/finance_ml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finance-ml
-Version: 0.0.3
+Version: 0.0.4
 Summary: Application of Machine Learning in Finances
 Author: Fabio Maia
 Author-email: <fabio.masaracchia@gmail.com>
 Keywords: python,finance,mlops
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

