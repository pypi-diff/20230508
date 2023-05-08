# Comparing `tmp/proventosweb-0.6.tar.gz` & `tmp/proventosweb-0.65.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proventosweb-0.6.tar", last modified: Mon May  8 13:58:27 2023, max compression
+gzip compressed data, was "proventosweb-0.65.tar", last modified: Mon May  8 14:12:06 2023, max compression
```

## Comparing `proventosweb-0.6.tar` & `proventosweb-0.65.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 13:58:27.294315 proventosweb-0.6/
--rw-rw-rw-   0        0        0      314 2023-05-08 13:58:27.294315 proventosweb-0.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-08 13:58:27.263068 proventosweb-0.6/proventosweb/
--rw-rw-rw-   0        0        0       44 2023-05-08 12:50:56.000000 proventosweb-0.6/proventosweb/__init__.py
--rw-rw-rw-   0        0        0    12078 2023-05-08 13:48:33.000000 proventosweb-0.6/proventosweb/proventosweb.py
-drwxrwxrwx   0        0        0        0 2023-05-08 13:58:27.294315 proventosweb-0.6/proventosweb.egg-info/
--rw-rw-rw-   0        0        0      314 2023-05-08 13:58:26.000000 proventosweb-0.6/proventosweb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      276 2023-05-08 13:58:27.000000 proventosweb-0.6/proventosweb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 13:58:26.000000 proventosweb-0.6/proventosweb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-03 22:03:21.000000 proventosweb-0.6/proventosweb.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       35 2023-05-08 13:58:26.000000 proventosweb-0.6/proventosweb.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-08 13:58:26.000000 proventosweb-0.6/proventosweb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-08 13:58:27.294315 proventosweb-0.6/setup.cfg
--rw-rw-rw-   0        0        0      516 2023-05-08 13:50:08.000000 proventosweb-0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 14:12:06.800421 proventosweb-0.65/
+-rw-rw-rw-   0        0        0      315 2023-05-08 14:12:06.800421 proventosweb-0.65/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-08 14:12:06.771059 proventosweb-0.65/proventosweb/
+-rw-rw-rw-   0        0        0       44 2023-05-08 12:50:56.000000 proventosweb-0.65/proventosweb/__init__.py
+-rw-rw-rw-   0        0        0    12094 2023-05-08 14:10:55.000000 proventosweb-0.65/proventosweb/proventosweb.py
+drwxrwxrwx   0        0        0        0 2023-05-08 14:12:06.785412 proventosweb-0.65/proventosweb.egg-info/
+-rw-rw-rw-   0        0        0      315 2023-05-08 14:12:06.000000 proventosweb-0.65/proventosweb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      276 2023-05-08 14:12:06.000000 proventosweb-0.65/proventosweb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 14:12:06.000000 proventosweb-0.65/proventosweb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-03 22:03:21.000000 proventosweb-0.65/proventosweb.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       35 2023-05-08 14:12:06.000000 proventosweb-0.65/proventosweb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-08 14:12:06.000000 proventosweb-0.65/proventosweb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-08 14:12:06.800421 proventosweb-0.65/setup.cfg
+-rw-rw-rw-   0        0        0      517 2023-05-08 14:11:22.000000 proventosweb-0.65/setup.py
```

### Comparing `proventosweb-0.6/proventosweb/proventosweb.py` & `proventosweb-0.65/proventosweb/proventosweb.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
                     sub.loc[i, 'Executado'] = sub.loc[i, 'Negociação'].str.split(' a ').str[0]
                 else:
                     sub.loc[i, 'Executado'] = sub.loc[i, 'Data COM']
             except:
                 sub.loc[i, 'Executado'] = None
         dfs = sub.loc[:, ['Data COM', 'Executado', 'Valor', 'Quantia']]
         dfs['Tipo'] = 'Subscrição'
-    dfcons = pd.DataFrame(columns=['Tipo', 'Data COM', 'Executado', 'Valor', 'Valor Original', 'Quantia'])
+    dfcons = pd.DataFrame(columns=['Tipo', 'Data COM', 'Executado', 'Valor', 'Valor Original', 'Quantia', 'Proporção'])
     if dfp is None and dfb is None and dfbo is None and dfs is None:
         dfcons = None
     else:
         dfcons = pd.concat([dfp, dfb, dfbo, dfs], ignore_index=True)
         dfcons['Data COM'] = pd.to_datetime(dfcons['Data COM'], dayfirst=True).dt.date
         dfcons['Executado'] = dfcons['Executado'].replace('-', None)
         dfcons['Executado'] = pd.to_datetime(dfcons['Executado'], dayfirst=True).dt.date
@@ -242,15 +242,15 @@
         longest_atv = None
         longest_time = 0
         j = 0
         for i, atv in enumerate(acoes):
             if i/len(acoes)>cortes[j]:
                 print('Já foi '+str(cortes[j]*100)+"% das ações!")
                 j = j+1
-            print(f'Processing {atv} ({i+1}/{len(acoes)})...')
+            print(f'Processando {atv} ({i+1}/{len(acoes)})...')
             atv_start_time = time.time()
             dfnovo = eventos(atv)
             atv_time = time.time() - atv_start_time
             if atv_time > longest_time:
                 longest_atv = atv
                 longest_time = atv_time
             if dfnovo is not None:
```

### Comparing `proventosweb-0.6/setup.py` & `proventosweb-0.65/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 
 setup(name='proventosweb',
-      version='0.6',
+      version='0.65',
       description='Uma biblioteca para buscar proventos de ações na plataforma Status Invest',
       url='https://github.com/rafaelpsampaio/proventosweb',
       author='Rafael Sampaio',
       author_email='rafapsampaio@gmail.com',
       packages=['proventosweb'],
       install_requires=[
           'pandas',
```

