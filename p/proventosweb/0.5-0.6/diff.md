# Comparing `tmp/proventosweb-0.5.tar.gz` & `tmp/proventosweb-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proventosweb-0.5.tar", last modified: Mon May  8 13:12:33 2023, max compression
+gzip compressed data, was "proventosweb-0.6.tar", last modified: Mon May  8 13:58:27 2023, max compression
```

## Comparing `proventosweb-0.5.tar` & `proventosweb-0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 13:12:33.031374 proventosweb-0.5/
--rw-rw-rw-   0        0        0      314 2023-05-08 13:12:33.031374 proventosweb-0.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-08 13:12:32.993971 proventosweb-0.5/proventosweb/
--rw-rw-rw-   0        0        0       44 2023-05-08 12:50:56.000000 proventosweb-0.5/proventosweb/__init__.py
--rw-rw-rw-   0        0        0    11029 2023-05-08 12:51:57.000000 proventosweb-0.5/proventosweb/proventosweb.py
-drwxrwxrwx   0        0        0        0 2023-05-08 13:12:33.031374 proventosweb-0.5/proventosweb.egg-info/
--rw-rw-rw-   0        0        0      314 2023-05-08 13:12:32.000000 proventosweb-0.5/proventosweb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      276 2023-05-08 13:12:32.000000 proventosweb-0.5/proventosweb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 13:12:32.000000 proventosweb-0.5/proventosweb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-03 22:03:21.000000 proventosweb-0.5/proventosweb.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       35 2023-05-08 13:12:32.000000 proventosweb-0.5/proventosweb.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-08 13:12:32.000000 proventosweb-0.5/proventosweb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-08 13:12:33.031374 proventosweb-0.5/setup.cfg
--rw-rw-rw-   0        0        0      516 2023-05-08 13:01:52.000000 proventosweb-0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 13:58:27.294315 proventosweb-0.6/
+-rw-rw-rw-   0        0        0      314 2023-05-08 13:58:27.294315 proventosweb-0.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-08 13:58:27.263068 proventosweb-0.6/proventosweb/
+-rw-rw-rw-   0        0        0       44 2023-05-08 12:50:56.000000 proventosweb-0.6/proventosweb/__init__.py
+-rw-rw-rw-   0        0        0    12078 2023-05-08 13:48:33.000000 proventosweb-0.6/proventosweb/proventosweb.py
+drwxrwxrwx   0        0        0        0 2023-05-08 13:58:27.294315 proventosweb-0.6/proventosweb.egg-info/
+-rw-rw-rw-   0        0        0      314 2023-05-08 13:58:26.000000 proventosweb-0.6/proventosweb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      276 2023-05-08 13:58:27.000000 proventosweb-0.6/proventosweb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 13:58:26.000000 proventosweb-0.6/proventosweb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-03 22:03:21.000000 proventosweb-0.6/proventosweb.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       35 2023-05-08 13:58:26.000000 proventosweb-0.6/proventosweb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-08 13:58:26.000000 proventosweb-0.6/proventosweb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-08 13:58:27.294315 proventosweb-0.6/setup.cfg
+-rw-rw-rw-   0        0        0      516 2023-05-08 13:50:08.000000 proventosweb-0.6/setup.py
```

### Comparing `proventosweb-0.5/proventosweb/proventosweb.py` & `proventosweb-0.6/proventosweb/proventosweb.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,16 +27,17 @@
         dob['Quantia To'] = dob['Quantia To'].astype(float)
         dob['Valor'] = dob.apply(lambda row: row['Quantia From'] if row['Quantia To'] == 1 else row['Quantia To'],
                                  axis=1)
         dfb = dob.loc[:, ['Tipo', 'Data COM', 'Executado', 'Valor']]
 
     if boni is not None and not boni.empty:
         boni['Executado'] = boni['Data de incorporação']
-        boni['Valor'] = boni['Valor base']
-        dfbo = boni.loc[:, ['Data COM', 'Executado', 'Valor']]
+        boni['Proporção'] = boni['Proporção'].apply(lambda x: float(x.replace(',', '.'))) / 100
+        boni['Valor'] = boni['Valor base'].apply(lambda x: float(x.replace(',', '.')))
+        dfbo = boni.loc[:, ['Data COM', 'Executado', 'Valor', 'Proporção']]
         dfbo['Tipo'] = 'Bonificação'
 
     if sub is not None and not sub.empty:
         sub['Quantia'] = sub['Valor Base']
         sub['Quantia'] = sub['Quantia'].str.replace('R$ ', '', regex=False).str.replace(',', '.', regex=False).astype(
             float)
         sub['Valor'] = sub['Percentual']
@@ -62,14 +63,16 @@
         dfcons['Data COM'] = pd.to_datetime(dfcons['Data COM'], dayfirst=True).dt.date
         dfcons['Executado'] = dfcons['Executado'].replace('-', None)
         dfcons['Executado'] = pd.to_datetime(dfcons['Executado'], dayfirst=True).dt.date
         if sub is not None and not sub.empty:
             dfcons['Quantia'] = dfcons['Quantia'].replace({np.nan: None})
         if prov is not None and not prov.empty:
             dfcons['Valor Original'] = dfcons['Valor Original'].replace({pd.NA: None})
+        if boni is not None and not prov.empty:
+            dfcons['Proporção'] = dfcons['Proporção'].replace({pd.NA: None})
         dfcons.sort_values(by=['Tipo', 'Data COM'])
     return dfcons
 
 
 def eventos(acao):
     acao = acao.upper()
     tipos = ['acoes', 'bdrs', 'fundos-imobiliarios', 'fiinfras', 'fiagros', 'etfs']
@@ -248,14 +251,20 @@
             dfnovo = eventos(atv)
             atv_time = time.time() - atv_start_time
             if atv_time > longest_time:
                 longest_atv = atv
                 longest_time = atv_time
             if dfnovo is not None:
                 dfprov = pd.concat([dfprov,dfnovo])
+        if 'Valor Original' in dfprov.columns:
+            dfprov['Valor Original'] = dfprov['Valor Original'].replace({pd.NA: None})
+        if 'Quantia' in dfprov.columns:
+            dfprov['Quantia'] = dfprov['Quantia'].replace({np.nan: None})
+        if 'Proporção' in dfprov.columns:
+            dfprov['Proporção'] = dfprov['Proporção'].replace({pd.NA: None})
         print('Acabou!')
         total_time = time.time() - start_time
         print(f'Tempo total: {total_time:.2f} segundos')
         print(f'Média por ativo: {(total_time/len(acoes)):.2f} segundos')
         print(f'Tempo máximo: {longest_atv} ({longest_time:.2f} segundos)')
     else:
         dfprov = pd.DataFrame(columns=['Ativo', 'Tipo', 'Data COM', 'Executado', 'Valor', 'Valor Original', 'Quantia'])
@@ -265,9 +274,15 @@
         for i in range(len(acoes)):
             if i/len(acoes)>cortes[j]:
                 print('Já foi '+str(cortes[j]*100)+"% das ações!")
             atv = acoes[i]
             dfnovo = eventos(atv)
             if dfnovo is not None:
                 dfprov = pd.concat([dfprov,dfnovo])
+        if 'Valor Original' in dfprov.columns:
+            dfprov['Valor Original'] = dfprov['Valor Original'].replace({pd.NA: None})
+        if 'Quantia' in dfprov.columns:
+            dfprov['Quantia'] = dfprov['Quantia'].replace({np.nan: None})
+        if 'Proporção' in dfprov.columns:
+            dfprov['Proporção'] = dfprov['Proporção'].replace({pd.NA: None})
         print('Acabou!')
     return dfprov
```

### Comparing `proventosweb-0.5/setup.py` & `proventosweb-0.6/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 
 setup(name='proventosweb',
-      version='0.5',
+      version='0.6',
       description='Uma biblioteca para buscar proventos de ações na plataforma Status Invest',
       url='https://github.com/rafaelpsampaio/proventosweb',
       author='Rafael Sampaio',
       author_email='rafapsampaio@gmail.com',
       packages=['proventosweb'],
       install_requires=[
           'pandas',
```

