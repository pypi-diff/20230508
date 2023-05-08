# Comparing `tmp/ds4finance-0.1.13.tar.gz` & `tmp/ds4finance-0.1.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ds4finance-0.1.13.tar", last modified: Sun Apr 30 22:37:39 2023, max compression
+gzip compressed data, was "dist\ds4finance-0.1.14.tar", last modified: Mon May  8 14:09:04 2023, max compression
```

## Comparing `ds4finance-0.1.13.tar` & `ds4finance-0.1.14.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 22:37:39.781592 ds4finance-0.1.13/
--rw-rw-rw-   0        0        0     2627 2023-04-30 22:37:39.780593 ds4finance-0.1.13/PKG-INFO
--rw-rw-rw-   0        0        0     1243 2023-04-20 20:51:26.000000 ds4finance-0.1.13/README.md
-drwxrwxrwx   0        0        0        0 2023-04-30 22:37:39.763593 ds4finance-0.1.13/ds4finance/
--rw-rw-rw-   0        0        0      963 2023-04-23 19:09:16.000000 ds4finance-0.1.13/ds4finance/__init__.py
--rw-rw-rw-   0        0        0    30573 2023-04-23 21:43:38.000000 ds4finance-0.1.13/ds4finance/functions.py
-drwxrwxrwx   0        0        0        0 2023-04-30 22:37:39.779613 ds4finance-0.1.13/ds4finance.egg-info/
--rw-rw-rw-   0        0        0     2627 2023-04-30 22:37:39.000000 ds4finance-0.1.13/ds4finance.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      234 2023-04-30 22:37:39.000000 ds4finance-0.1.13/ds4finance.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 22:37:39.000000 ds4finance-0.1.13/ds4finance.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-04-30 22:37:39.000000 ds4finance-0.1.13/ds4finance.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-30 22:37:39.000000 ds4finance-0.1.13/ds4finance.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-30 22:37:39.781592 ds4finance-0.1.13/setup.cfg
--rw-rw-rw-   0        0        0     1174 2023-04-30 22:37:32.000000 ds4finance-0.1.13/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 14:09:04.264680 ds4finance-0.1.14/
+-rw-rw-rw-   0        0        0     2627 2023-05-08 14:09:04.263680 ds4finance-0.1.14/PKG-INFO
+-rw-rw-rw-   0        0        0     1243 2023-04-20 20:51:26.000000 ds4finance-0.1.14/README.md
+drwxrwxrwx   0        0        0        0 2023-05-08 14:09:04.244049 ds4finance-0.1.14/ds4finance/
+-rw-rw-rw-   0        0        0      963 2023-04-23 19:09:16.000000 ds4finance-0.1.14/ds4finance/__init__.py
+-rw-rw-rw-   0        0        0    31358 2023-05-08 14:07:04.000000 ds4finance-0.1.14/ds4finance/functions.py
+drwxrwxrwx   0        0        0        0 2023-05-08 14:09:04.262679 ds4finance-0.1.14/ds4finance.egg-info/
+-rw-rw-rw-   0        0        0     2627 2023-05-08 14:09:04.000000 ds4finance-0.1.14/ds4finance.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      234 2023-05-08 14:09:04.000000 ds4finance-0.1.14/ds4finance.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 14:09:04.000000 ds4finance-0.1.14/ds4finance.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-08 14:09:04.000000 ds4finance-0.1.14/ds4finance.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-08 14:09:04.000000 ds4finance-0.1.14/ds4finance.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-08 14:09:04.264680 ds4finance-0.1.14/setup.cfg
+-rw-rw-rw-   0        0        0     1174 2023-05-08 14:05:59.000000 ds4finance-0.1.14/setup.py
```

### Comparing `ds4finance-0.1.13/PKG-INFO` & `ds4finance-0.1.14/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ds4finance
-Version: 0.1.13
+Version: 0.1.14
 Summary: A collection of data science tools for finance
 Home-page: https://github.com/LuisSousaSilva/ds4finance
 Author: Luis Silva
 Author-email: luis_paulo_silva@hotmail.com
 License: MIT
 Description: # ds4finance
```

### Comparing `ds4finance-0.1.13/README.md` & `ds4finance-0.1.14/README.md`

 * *Files identical despite different names*

### Comparing `ds4finance-0.1.13/ds4finance/__init__.py` & `ds4finance-0.1.14/ds4finance/__init__.py`

 * *Files identical despite different names*

### Comparing `ds4finance-0.1.13/ds4finance/functions.py` & `ds4finance-0.1.14/ds4finance/functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -844,15 +844,15 @@
     yearly_returns = yearly_returns.loc[first_year + 1:last_year].transpose()
     yearly_returns = round(yearly_returns, 2)
 
     # As strings and percentages
     yearly_returns.columns = yearly_returns.columns.map(str)    
     yearly_returns_numeric = yearly_returns.copy()
 
-    if style=='table'and color==False:
+    if style=='table' and color==False:
         yearly_returns = yearly_returns / 100
         yearly_returns = yearly_returns.style.format("{:.2%}")
         print_title(title)
 
     elif style=='numeric':
         yearly_returns = yearly_returns_numeric.copy()
     
@@ -874,8 +874,31 @@
         yearly_returns = sns.heatmap(yearly_returns_numeric, annot=True, cmap="RdYlGn", linewidths=.2, fmt=".2f", cbar=False, center=0)
         for t in yearly_returns.texts: t.set_text(t.get_text() + "%")
         plt.title(title)
     
     else:
         print('At least one parameter has a wrong input')
 
-    return yearly_returns
+    return yearly_returns
+
+def compute_time_series(dataframe: pd.DataFrame, start_value: float = 100) -> pd.DataFrame:
+    """
+    Compute the growth time series given a DataFrame of returns.
+
+    Parameters
+    ----------
+    dataframe : pandas.DataFrame
+        DataFrame containing return data.
+    start_value : float, optional
+        Initial value of the time series. Default is 100.
+
+    Returns
+    -------
+    pandas.DataFrame
+        A pandas DataFrame containing the growth time series for each column in the input DataFrame.
+    """
+    # Validate input
+    if not isinstance(dataframe, pd.DataFrame):
+        raise TypeError("Input 'dataframe' must be a pandas DataFrame.")
+
+    # Calculate growth time series
+    return (np.exp(np.log1p(dataframe).cumsum())) * start_value
```

### Comparing `ds4finance-0.1.13/ds4finance.egg-info/PKG-INFO` & `ds4finance-0.1.14/ds4finance.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ds4finance
-Version: 0.1.13
+Version: 0.1.14
 Summary: A collection of data science tools for finance
 Home-page: https://github.com/LuisSousaSilva/ds4finance
 Author: Luis Silva
 Author-email: luis_paulo_silva@hotmail.com
 License: MIT
 Description: # ds4finance
```

### Comparing `ds4finance-0.1.13/setup.py` & `ds4finance-0.1.14/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="ds4finance",
-    version="0.1.13",
+    version="0.1.14",
     description="A collection of data science tools for finance",
     long_description=open("README.md", "r").read(),
     long_description_content_type="text/markdown",
     author="Luis Silva",
     author_email="luis_paulo_silva@hotmail.com",
     url="https://github.com/LuisSousaSilva/ds4finance",
     packages=find_packages(),
```

