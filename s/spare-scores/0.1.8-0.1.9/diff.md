# Comparing `tmp/spare_scores-0.1.8.tar.gz` & `tmp/spare_scores-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spare_scores-0.1.8.tar", last modified: Fri Mar 17 14:40:44 2023, max compression
+gzip compressed data, was "spare_scores-0.1.9.tar", last modified: Mon Mar 20 15:27:15 2023, max compression
```

## Comparing `spare_scores-0.1.8.tar` & `spare_scores-0.1.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 hwangg   (25642) sbiauser (25000)        0 2023-03-17 14:40:44.412337 spare_scores-0.1.8/
--rw-r--r--   0 hwangg   (25642) sbiauser (25000)      142 2023-03-14 18:05:05.000000 spare_scores-0.1.8/LICENSE
--rw-r--r--   0 hwangg   (25642) sbiauser (25000)       85 2023-03-14 18:05:05.000000 spare_scores-0.1.8/MANIFEST.in
--rw-r--r--   0 hwangg   (25642) sbiauser (25000)     3012 2023-03-17 14:40:44.411477 spare_scores-0.1.8/PKG-INFO
--rw-r--r--   0 hwangg   (25642) sbiauser (25000)     2505 2023-03-14 18:05:05.000000 spare_scores-0.1.8/README.md
--rw-r--r--   0 hwangg   (25642) sbiauser (25000)      103 2023-03-14 18:05:05.000000 spare_scores-0.1.8/pyproject.toml
--rw-r--r--   0 hwangg   (25642) sbiauser (25000)       38 2023-03-17 14:40:44.412636 spare_scores-0.1.8/setup.cfg
--rw-r--r--   0 hwangg   (25642) sbiauser (25000)      765 2023-03-17 14:37:28.000000 spare_scores-0.1.8/setup.py
-drwxr-xr-x   0 hwangg   (25642) sbiauser (25000)        0 2023-03-17 14:40:44.370851 spare_scores-0.1.8/spare_scores/
--rw-r--r--   0 hwangg   (25642) sbiauser (25000)       61 2023-03-14 18:05:05.000000 spare_scores-0.1.8/spare_scores/__init__.py
--rw-r--r--   0 hwangg   (25642) sbiauser (25000)    13559 2023-03-17 14:31:16.000000 spare_scores-0.1.8/spare_scores/data_prep.py
--rw-r--r--   0 hwangg   (25642) sbiauser (25000)     7231 2023-03-14 22:19:51.000000 spare_scores-0.1.8/spare_scores/spare_scores.py
--rw-r--r--   0 hwangg   (25642) sbiauser (25000)     3949 2023-03-14 18:05:05.000000 spare_scores-0.1.8/spare_scores/svm.py
-drwxr-xr-x   0 hwangg   (25642) sbiauser (25000)        0 2023-03-17 14:40:44.410025 spare_scores-0.1.8/spare_scores.egg-info/
--rw-r--r--   0 hwangg   (25642) sbiauser (25000)     3012 2023-03-17 14:40:44.405958 spare_scores-0.1.8/spare_scores.egg-info/PKG-INFO
--rw-r--r--   0 hwangg   (25642) sbiauser (25000)      332 2023-03-17 14:40:44.406865 spare_scores-0.1.8/spare_scores.egg-info/SOURCES.txt
--rw-r--r--   0 hwangg   (25642) sbiauser (25000)        1 2023-03-17 14:40:44.407974 spare_scores-0.1.8/spare_scores.egg-info/dependency_links.txt
--rw-r--r--   0 hwangg   (25642) sbiauser (25000)       49 2023-03-17 14:40:44.409079 spare_scores-0.1.8/spare_scores.egg-info/requires.txt
--rw-r--r--   0 hwangg   (25642) sbiauser (25000)       13 2023-03-17 14:40:44.410567 spare_scores-0.1.8/spare_scores.egg-info/top_level.txt
+drwxr-xr-x   0 hwangg   (25642) sbiauser (25000)        0 2023-03-20 15:27:15.535667 spare_scores-0.1.9/
+-rw-r--r--   0 hwangg   (25642) sbiauser (25000)      142 2023-03-14 18:05:05.000000 spare_scores-0.1.9/LICENSE
+-rw-r--r--   0 hwangg   (25642) sbiauser (25000)       85 2023-03-14 18:05:05.000000 spare_scores-0.1.9/MANIFEST.in
+-rw-r--r--   0 hwangg   (25642) sbiauser (25000)     3012 2023-03-20 15:27:15.534835 spare_scores-0.1.9/PKG-INFO
+-rw-r--r--   0 hwangg   (25642) sbiauser (25000)     2505 2023-03-14 18:05:05.000000 spare_scores-0.1.9/README.md
+-rw-r--r--   0 hwangg   (25642) sbiauser (25000)      103 2023-03-14 18:05:05.000000 spare_scores-0.1.9/pyproject.toml
+-rw-r--r--   0 hwangg   (25642) sbiauser (25000)       38 2023-03-20 15:27:15.535926 spare_scores-0.1.9/setup.cfg
+-rw-r--r--   0 hwangg   (25642) sbiauser (25000)      694 2023-03-20 15:22:18.000000 spare_scores-0.1.9/setup.py
+drwxr-xr-x   0 hwangg   (25642) sbiauser (25000)        0 2023-03-20 15:27:15.511657 spare_scores-0.1.9/spare_scores/
+-rw-r--r--   0 hwangg   (25642) sbiauser (25000)       61 2023-03-14 18:05:05.000000 spare_scores-0.1.9/spare_scores/__init__.py
+-rw-r--r--   0 hwangg   (25642) sbiauser (25000)    12478 2023-03-20 15:18:37.000000 spare_scores-0.1.9/spare_scores/data_prep.py
+-rw-r--r--   0 hwangg   (25642) sbiauser (25000)     7114 2023-03-17 21:47:54.000000 spare_scores-0.1.9/spare_scores/spare_scores.py
+-rw-r--r--   0 hwangg   (25642) sbiauser (25000)     3949 2023-03-14 18:05:05.000000 spare_scores-0.1.9/spare_scores/svm.py
+drwxr-xr-x   0 hwangg   (25642) sbiauser (25000)        0 2023-03-20 15:27:15.533639 spare_scores-0.1.9/spare_scores.egg-info/
+-rw-r--r--   0 hwangg   (25642) sbiauser (25000)     3012 2023-03-20 15:27:14.000000 spare_scores-0.1.9/spare_scores.egg-info/PKG-INFO
+-rw-r--r--   0 hwangg   (25642) sbiauser (25000)      332 2023-03-20 15:27:15.530547 spare_scores-0.1.9/spare_scores.egg-info/SOURCES.txt
+-rw-r--r--   0 hwangg   (25642) sbiauser (25000)        1 2023-03-20 15:27:14.000000 spare_scores-0.1.9/spare_scores.egg-info/dependency_links.txt
+-rw-r--r--   0 hwangg   (25642) sbiauser (25000)       26 2023-03-20 15:27:14.000000 spare_scores-0.1.9/spare_scores.egg-info/requires.txt
+-rw-r--r--   0 hwangg   (25642) sbiauser (25000)       13 2023-03-20 15:27:14.000000 spare_scores-0.1.9/spare_scores.egg-info/top_level.txt
```

### Comparing `spare_scores-0.1.8/PKG-INFO` & `spare_scores-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spare_scores
-Version: 0.1.8
+Version: 0.1.9
 Summary: Compute characteristic brain signatures of your case population.
 Home-page: UNKNOWN
 Author: Gyujoon Hwang
 Author-email: ghwang1106@gmail.com
 License: MIT
 Description: For detailed documentation, please see here: **https://cbica.github.io/spare_score/**
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: spare_scores Version: 0.1.8 Summary: Compute
+Metadata-Version: 2.1 Name: spare_scores Version: 0.1.9 Summary: Compute
 characteristic brain signatures of your case population. Home-page: UNKNOWN
 Author: Gyujoon Hwang Author-email: ghwang1106@gmail.com License: MIT
 Description: For detailed documentation, please see here: **https://
 cbica.github.io/spare_score/** # Compute SPARE Scores for Your Case "SPARE" is
 short for "Spatial Pattern of Abnormalities for Recognition of ..." If you have
 brain images of a case population, such as the Alzheimer's disease (AD), the
 SPARE model will try to find characteristic brain patterns of AD with respect
```

### Comparing `spare_scores-0.1.8/README.md` & `spare_scores-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `spare_scores-0.1.8/setup.py` & `spare_scores-0.1.9/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(name='spare_scores',
-      version='0.1.8',
+      version='0.1.9',
       description='Compute characteristic brain signatures of your case population.',
       long_description=long_description,
       long_description_content_type='text/markdown',
       author='Gyujoon Hwang',
       author_email='ghwang1106@gmail.com',
       license='MIT',
       packages=find_packages(),
       package_data={'spare_scores':['mdl/*.pkl.gz','data/*.csv']},
       include_package_data=True,
-      install_requires=['numpy==1.20.3',
-                        'pandas==1.5.3',
-                        'scikit-learn==0.23.2']
+      install_requires=['numpy', 'pandas', 'scikit-learn']
       )
```

### Comparing `spare_scores-0.1.8/spare_scores/data_prep.py` & `spare_scores-0.1.9/spare_scores/data_prep.py`

 * *Files 16% similar despite different names*

```diff
@@ -34,44 +34,14 @@
     return load_model(f'{pkg_path}/mdl/{file_name}')
   else:
     print('Available example data:')
     [print(f' - {a}') for a in list_data]
     print('Available example SPARE models:')
     [print(f' - {a}') for a in list_mdl]
 
-def col_names(df: pd.DataFrame,
-              cols: list=['ID','Age','Sex']) -> tuple:
-  """Matches required column names with common name variants. 
-
-  Args:
-    df: pandas dataframe.
-    cols: columns to search for name variants.
-
-  Returns:
-    a string or a tuple with matched variants.
-  """
-  col_name_variants = {'ID':['ID','id','PTID','participant_id'],
-                       'Age':['Age','age','AGE'],
-                       'Sex':['Sex','sex','SEX']}
-  col_name_variants = {a: col_name_variants[a] for a in cols}
-  for k in col_name_variants.keys():
-    if k not in cols:
-      continue
-    for i in col_name_variants[k]:
-      if i in df.columns:
-        col_name_variants[k] = i
-        break
-  col_not_found = [a for a in col_name_variants.keys() if type(col_name_variants[a])==list]
-  if len(col_not_found) > 0:
-    return logging.error(f'Required columns not found: {col_not_found}')
-  if len(cols) == 1:
-    return col_name_variants[cols[0]]
-  else: 
-    return tuple(col_name_variants.values())
-
 def check_train(df: pd.DataFrame, 
                 predictors: list,
                 to_predict: str,
                 pos_group: str = '') -> Tuple[pd.DataFrame, list, str]:
   """Checks training dataframe for errors.
 
   Args:
@@ -79,47 +49,48 @@
     predictors: a list of predictors for SPARE model training.
     to_predict: variable to predict.
     pos_group: group to assign a positive SPARE score (only for classification).
 
   Returns:
     a tuple containing 1) filtered dataframe, 2) filtered predictors, 3) SPARE model type.
   """
+  if not {'ID','Age','Sex'}.issubset(set(df.columns)):
+    return logging.error('Please check equired columns: ID, Age, Sex.')
   if not set(predictors).issubset(df.columns):
     return logging.error('Not all predictors exist in the input dataframe.')
   if to_predict not in df.columns:
     return logging.error('Variable to predict is not in the input dataframe.')
   if to_predict in predictors:
     logging.info('Variable to predict is in the predictor set. This will be removed from the set.')
     predictors.remove(to_predict)
   if np.sum(np.sum(pd.isna(df[predictors]))) > 0:
     logging.info('Some participants have invalid predictor variables (i.e. n/a). They will be excluded.')
     df = df.loc[np.sum(pd.isna(df[predictors]), axis=1) == 0].reset_index(drop=True)
 
-  col_id = col_names(df,['ID'])
   if len(df[to_predict].unique()) == 2:
     if pos_group == '':
       return logging.error('"pos_group" not provided (group to assign a positive score).')
     elif pos_group not in df[to_predict].unique():
       return logging.error('"pos_group" is not one of the two groups in the variable to predict.')
     if np.min(df[to_predict].value_counts()) < 10:
       return logging.error('At least one of the groups to classify is too small (n<10).')
     elif np.min(df[to_predict].value_counts()) < 100:
       logging.warn('At least one of the groups to classify may be too small (n<100).')
-    if np.sum((df[col_id].astype(str)+df[to_predict]).duplicated()) > 0:
+    if np.sum((df['ID']+df[to_predict]).duplicated()) > 0:
       logging.warn('Training dataset has duplicate participants.')
     spare_type = 'classification'
 
   elif len(df[to_predict].unique()) > 2:
     if df[to_predict].dtype not in ['int64', 'float64']:
       return logging.error('Variable to predict must be either binary or numeric.')
     if len(df.index) < 10:
       return logging.error('Sample size is too small (n<10).')
     elif len(df.index) < 100:
       logging.warn('Sample size may be too small (n<100).')
-    if np.sum(df[col_id].duplicated()) > 0:
+    if np.sum(df['ID'].duplicated()) > 0:
       logging.warn('Training dataset has duplicate participants.')
     if pos_group != '':
       logging.info('SPARE regression does not need a "pos_group". This will be ignored.')
     spare_type = 'regression'
   else:
     return logging.error('Variable to predict has no variance.')
     
@@ -130,27 +101,28 @@
                meta_data: dict):
   """Checks testing dataframe for errors.
 
   Args:
     df: a pandas dataframe containing testing data.
     meta_data: a dictionary containing training information on its paired SPARE model.
   """
-  col_id, col_age = col_names(df,['ID','Age'])
+  if not {'ID','Age','Sex'}.issubset(set(df.columns)):
+    return logging.error('Please check equired columns: ID, Age, Sex.')
   if not set(meta_data['predictors']).issubset(df.columns):
     cols_not_found = sorted(set(meta_data['predictors']) - set(df.columns))
     return logging.error(f'Not all predictors exist in the input dataframe: {cols_not_found}')
     
-  if (np.min(df[col_age]) < meta_data['age_range'][0]) or (
-           np.max(df[col_age]) > meta_data['age_range'][1]):
+  if (np.min(df['Age']) < meta_data['age_range'][0]) or (
+           np.max(df['Age']) > meta_data['age_range'][1]):
     logging.warn('Some participants fall outside the age range of the SPARE model.')
 
   if np.sum(np.sum(pd.isna(df[meta_data['predictors']]))) > 0:
     logging.warn('Some participants have invalid predictor variables.')
 
-  if np.any(df[col_id].isin(meta_data['cv_results'][col_id])):
+  if np.any(df['ID'].isin(meta_data['cv_results']['ID'])):
     logging.info('Some participants seem to have been in the model training.')
 
 def smart_unique(df1: pd.DataFrame,
                  df2: pd.DataFrame=None,
                  to_predict: str=None,
                  verbose: int=1) -> Union[pd.DataFrame, tuple]:
   """Select unique data points in a way that optimizes SPARE training.
@@ -166,58 +138,56 @@
   Returns:
     a trimmed pandas dataframe or a tuple of two dataframes with only one time point per ID.
   """
   assert (isinstance(df2, pd.DataFrame) or (df2 is None)), (
     'Either provide a 2nd pandas dataframe for the 2nd argument or specify it with "to_predict"')
   if verbose == 0:
     logging.basicConfig(level=logging.WARNING, format='%(levelname)s: %(message)s', force=True)
-  col_id = col_names(df1, cols=['ID'])
   if df2 is None:
     if to_predict is None:
       return logging.error('Either provide a second dataframe or provide a column "to_predict"')
     elif len(df1[to_predict].unique()) > 2:
-      if ~np.any(df1[col_id].duplicated()):
+      if ~np.any(df1['ID'].duplicated()):
         logging.info('No duplicated IDs.')
       else:
         logging.info('Select unique time points for SPARE regression training.')
         df1[f'{to_predict}_from_mean'] = np.abs(df1[to_predict] - np.mean(df1[to_predict]))
-        df1 = df1[df1.groupby(col_id)[f'{to_predict}_from_mean'].transform(
+        df1 = df1[df1.groupby('ID')[f'{to_predict}_from_mean'].transform(
                           max) == df1[f'{to_predict}_from_mean']].reset_index(drop=True)
         df1 = df1.drop(columns=f'{to_predict}_from_mean')
-        df1 = df1[~df1[col_id].duplicated()].reset_index(drop=True)
+        df1 = df1[~df1['ID'].duplicated()].reset_index(drop=True)
       return df1
     elif len(df1[to_predict].unique()) < 2:
       return logging.error('Variable to predict has no variance.')
-    if ~np.any((df1[col_id].astype(str) + df1[to_predict].astype(str)).duplicated()):
+    if ~np.any((df1['ID'].astype(str) + df1[to_predict].astype(str)).duplicated()):
       logging.info('No duplicated IDs in either group.')
       return df1
     grps = list(df1[to_predict].unique())
     df1, df2 = df1[df1[to_predict] == grps[0]], df1[df1[to_predict] == grps[1]]
     no_df2 = True
   else:
     if to_predict is not None:
       logging.info('"to_predict" will be ignored.')
-    if (~np.any(df1[col_id].duplicated())) and (~np.any(df2[col_id].duplicated())):
+    if (~np.any(df1['ID'].duplicated())) and (~np.any(df2['ID'].duplicated())):
       logging.info('No duplicated IDs in either group.')
       return (df1, df2)
     no_df2 = False
 
   logging.info('Select unique time points for SPARE classification training.')
-  col_age = col_names(df1, cols=['Age'])
   swap = False
-  if stats.ttest_ind(df1[col_age], df2[col_age]).pvalue < 0.05:
-    if np.mean(df1[col_age]) < np.mean(df2[col_age]):
+  if stats.ttest_ind(df1['Age'], df2['Age']).pvalue < 0.05:
+    if np.mean(df1['Age']) < np.mean(df2['Age']):
         df1, df2, swap = df2.copy(), df1.copy(), True
-    df2 = df2.loc[df2[col_age] >= np.min(df1[col_age])].reset_index(drop=True)
-    df1 = df1[df1.groupby(col_id)[col_age].transform(min) == df1[col_age]].reset_index(drop=True)
-    df2 = df2[df2.groupby(col_id)[col_age].transform(max) == df2[col_age]].reset_index(drop=True)
+    df2 = df2.loc[df2['Age'] >= np.min(df1['Age'])].reset_index(drop=True)
+    df1 = df1[df1.groupby('ID')['Age'].transform(min) == df1['Age']].reset_index(drop=True)
+    df2 = df2[df2.groupby('ID')['Age'].transform(max) == df2['Age']].reset_index(drop=True)
   else:
     logging.info('Age difference not significant between two groups.')
-  df1 = df1[~df1[col_id].duplicated()].reset_index(drop=True)
-  df2 = df2[~df2[col_id].duplicated()].reset_index(drop=True)
+  df1 = df1[~df1['ID'].duplicated()].reset_index(drop=True)
+  df2 = df2[~df2['ID'].duplicated()].reset_index(drop=True)
   if swap:
     df1, df2 = df2.copy(), df1.copy()
   if no_df2:
     return pd.concat([df1, df2], ignore_index=True)
   else:
     return (df1, df2)
 
@@ -263,50 +233,49 @@
 
   if (age_out_percentage <= 0) or (age_out_percentage >= 100):
     return logging.error('Age-out-percentage must be between 0 and 100')
  
   swap = 1
   random.seed(2022)
   n_orig = len(df1.index) + len(df2.index)
-  col_age, col_sex = col_names(df1, ['Age', 'Sex'])
-  s1, s2 = df1[col_sex].unique()
+  s1, s2 = df1['Sex'].unique()
 
-  p_age = stats.ttest_ind(df1[col_age], df2[col_age]).pvalue
-  p_sex = stats.chi2_contingency([np.array(df1[col_sex].value_counts()), np.array(df2[col_sex].value_counts())])[1]
+  p_age = stats.ttest_ind(df1['Age'], df2['Age']).pvalue
+  p_sex = stats.chi2_contingency([np.array(df1['Sex'].value_counts()), np.array(df2['Sex'].value_counts())])[1]
   if verbose > 1:
     print(f' Orig.: P_age: {np.round(p_age,2)}/ P_sex {np.round(p_sex,2)}')
 
   p_age_all, p_sex_all = np.array(p_age), np.array(p_sex)
   while np.min([p_age, p_sex]) < p_threshold:
     if len(df2.index) > len(df1.index):
       df1, df2 = df2.copy(), df1.copy()
       swap *= -1
     if p_age < p_threshold:
-      if np.mean(df1[col_age]) < np.mean(df2[col_age]):
-        i_age = df1[col_age] < np.percentile(df1[col_age], age_out_percentage)
+      if np.mean(df1['Age']) < np.mean(df2['Age']):
+        i_age = df1['Age'] < np.percentile(df1['Age'], age_out_percentage)
       else:
-        i_age = df1[col_age] > np.percentile(df1[col_age], 100-age_out_percentage)
+        i_age = df1['Age'] > np.percentile(df1['Age'], 100-age_out_percentage)
     else:
-      i_age = df1[col_age] >= 0
+      i_age = df1['Age'] >= 0
     if p_sex < p_threshold:
-      if np.sum(df1[col_sex] == s1)/np.sum(df1[col_sex] == s2) > np.sum(df2[col_sex] == s1)/np.sum(df2[col_sex] == s2):
-        i_sex = df1[col_sex] == s1
+      if np.sum(df1['Sex'] == s1)/np.sum(df1['Sex'] == s2) > np.sum(df2['Sex'] == s1)/np.sum(df2['Sex'] == s2):
+        i_sex = df1['Sex'] == s1
       else:
-        i_sex = df1[col_sex] == s2
+        i_sex = df1['Sex'] == s2
     else:
-      i_sex = df1[col_sex].isin([s1, s2])
+      i_sex = df1['Sex'].isin([s1, s2])
 
     try:
       df1 = df1.drop(random.sample(list(df1[i_age & i_sex].index), 1)).reset_index(drop=True)
     except:
       if np.min([len(df1.index), len(df2.index)]) > 10:
         print('Try increasing "age_out_percentage" parameter')
       return logging.error('Matching failed...')
-    p_age = stats.ttest_ind(df1[col_age], df2[col_age]).pvalue
-    p_sex = stats.chi2_contingency([np.array(df1[col_sex].value_counts()), np.array(df2[col_sex].value_counts())])[1]
+    p_age = stats.ttest_ind(df1['Age'], df2['Age']).pvalue
+    p_sex = stats.chi2_contingency([np.array(df1['Sex'].value_counts()), np.array(df2['Sex'].value_counts())])[1]
     p_age_all = np.append(p_age_all, p_age)
     p_sex_all = np.append(p_sex_all, p_sex)
   if swap == -1:
     df1, df2 = df2.copy(), df1.copy()
 
   if verbose > 1:
     n_dropped = n_orig - len(df1.index) - len(df2.index)
```

### Comparing `spare_scores-0.1.8/spare_scores/spare_scores.py` & `spare_scores-0.1.9/spare_scores/spare_scores.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import pickle
 import logging
 import numpy as np
 import pandas as pd
 from typing import Tuple, Union
 from dataclasses import dataclass
 from spare_scores.svm import run_SVC, run_SVR
-from spare_scores.data_prep import col_names, check_train, check_test, load_model
+from spare_scores.data_prep import check_train, check_test, load_model
 
 logging.basicConfig(level=logging.INFO, format='%(levelname)s: %(message)s')
 
 @dataclass
 class MetaData:
   """Stores training information on its paired SPARE model
   """
@@ -39,23 +39,22 @@
 
   Returns:
     a tuple of two dictionaries: first to contain SPARE model coefficients, and
       second to contain model information
   """
 
   df = _load_df(df)
-  col_id, col_age, col_sex = col_names(df)
   df, predictors, spare_type = check_train(df, predictors, to_predict, pos_group)
   if spare_type == 'classification':
     groups_to_classify = [a for a in df[to_predict].unique() if a != pos_group] + [pos_group]
 
   # Initiate SPARE model
   meta_data = MetaData(spare_type, kernel, predictors, to_predict)
   meta_data.n = len(df.index)
-  meta_data.age_range = [np.min(df[col_age]), np.max(df[col_age])]
+  meta_data.age_range = [np.min(df['Age']), np.max(df['Age'])]
 
   # Convert categorical variables
   var_categorical = df[predictors].dtypes == np.object
   var_categorical = var_categorical[var_categorical].index
   meta_data.categorical_var_map = dict(zip(var_categorical, [None]*len(var_categorical)))
   for var in var_categorical:
     if len(df[var].unique()) == 2:
@@ -85,15 +84,15 @@
     if len(df.index) > 1000:
       _, _, _, params = run_SVR(df.sample(n=500, random_state=2022).reset_index(drop=True), predictors,
                 to_predict, param_grid=param_grid, n_repeats=1, verbose=0)
       for par in param_grid.keys():
         param_grid[par] = _expspace([np.min(params[f'{par}_optimal']), np.max(params[f'{par}_optimal'])])
     df['predicted'], mdl, meta_data.mae, meta_data.params = run_SVR(
                   df, predictors, to_predict, param_grid=param_grid)
-  meta_data.cv_results = df[list(dict.fromkeys([col_id, col_age, col_sex, to_predict, 'predicted']))]
+  meta_data.cv_results = df[list(dict.fromkeys(['ID', 'Age', 'Sex', to_predict, 'predicted']))]
 
   # Save model
   if save_path is not None:
     if ~save_path.endswith('.pkl.gz'):
       save_path = save_path + '.pkl.gz'
     with gzip.open(save_path, 'wb') as f:
       pickle.dump((mdl, vars(meta_data)), f)
@@ -150,16 +149,16 @@
     X = mdl['scaler'][i].transform(df[meta_data['predictors']])
     if meta_data['kernel'] == 'linear':
       ss[:, i] = np.sum(X * mdl['mdl'][i].coef_, axis=1) + mdl['mdl'][i].intercept_
     else:
       ss[:, i] = mdl['mdl'][i].decision_function(X)
     if meta_data['spare_type'] == 'regression':
       ss[:, i] = (ss[:, i] - mdl['bias_correct']['int'][i]) / mdl['bias_correct']['slope'][i]
-    ss[df[col_names(df,['ID'])].isin(
-      meta_data['cv_results'][col_names(meta_data['cv_results'],['ID'])][mdl['cv_folds'][i][0]]), i] = np.nan
+    ss[df['ID'].isin(
+      meta_data['cv_results']['ID'][mdl['cv_folds'][i][0]]), i] = np.nan
   ss_mean = np.nanmean(ss, axis=1)
   ss_mean[np.all(np.isnan(ss),axis=1)] = np.nan
 
   return pd.DataFrame(data={'SPARE_scores': ss_mean})
 
 def _expspace(span: list):
   return np.exp(np.linspace(span[0], span[1], num=int(span[1])-int(span[0])+1))
```

### Comparing `spare_scores-0.1.8/spare_scores/svm.py` & `spare_scores-0.1.9/spare_scores/svm.py`

 * *Files identical despite different names*

### Comparing `spare_scores-0.1.8/spare_scores.egg-info/PKG-INFO` & `spare_scores-0.1.9/spare_scores.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spare-scores
-Version: 0.1.8
+Version: 0.1.9
 Summary: Compute characteristic brain signatures of your case population.
 Home-page: UNKNOWN
 Author: Gyujoon Hwang
 Author-email: ghwang1106@gmail.com
 License: MIT
 Description: For detailed documentation, please see here: **https://cbica.github.io/spare_score/**
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: spare-scores Version: 0.1.8 Summary: Compute
+Metadata-Version: 2.1 Name: spare-scores Version: 0.1.9 Summary: Compute
 characteristic brain signatures of your case population. Home-page: UNKNOWN
 Author: Gyujoon Hwang Author-email: ghwang1106@gmail.com License: MIT
 Description: For detailed documentation, please see here: **https://
 cbica.github.io/spare_score/** # Compute SPARE Scores for Your Case "SPARE" is
 short for "Spatial Pattern of Abnormalities for Recognition of ..." If you have
 brain images of a case population, such as the Alzheimer's disease (AD), the
 SPARE model will try to find characteristic brain patterns of AD with respect
```

