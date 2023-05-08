# Comparing `tmp/mixalime-2.9.8.tar.gz` & `tmp/mixalime-2.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mixalime-2.9.8.tar", last modified: Mon Mar 27 07:08:34 2023, max compression
+gzip compressed data, was "mixalime-2.9.9.tar", last modified: Mon Mar 27 18:45:12 2023, max compression
```

## Comparing `mixalime-2.9.8.tar` & `mixalime-2.9.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 georgy    (1000) georgy    (1001)        0 2023-03-27 07:08:34.916621 mixalime-2.9.8/
--rw-r--r--   0 georgy    (1000) georgy    (1001)       23 2022-10-30 08:47:57.000000 mixalime-2.9.8/MANIFEST.in
--rw-r--r--   0 georgy    (1000) georgy    (1001)     4435 2023-03-27 07:08:34.916621 mixalime-2.9.8/PKG-INFO
--rw-r--r--   0 georgy    (1000) georgy    (1001)     3792 2022-10-30 08:57:43.000000 mixalime-2.9.8/README.md
-drwxr-xr-x   0 georgy    (1000) georgy    (1001)        0 2023-03-27 07:08:34.916621 mixalime-2.9.8/mixalime/
--rw-r--r--   0 georgy    (1000) georgy    (1001)      964 2023-03-27 06:59:48.000000 mixalime-2.9.8/mixalime/__init__.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)     6058 2023-03-25 17:27:15.000000 mixalime-2.9.8/mixalime/combine.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)    14940 2023-03-25 17:07:55.000000 mixalime-2.9.8/mixalime/create.py
-drwxr-xr-x   0 georgy    (1000) georgy    (1001)        0 2023-03-27 07:08:34.916621 mixalime-2.9.8/mixalime/data/
--rw-r--r--   0 georgy    (1000) georgy    (1001)   637068 2023-03-25 17:07:55.000000 mixalime-2.9.8/mixalime/data/Lato-Medium.ttf
--rw-r--r--   0 georgy    (1000) georgy    (1001)   657212 2023-03-25 17:07:55.000000 mixalime-2.9.8/mixalime/data/Lato-Regular.ttf
--rwxr-xr-x   0 georgy    (1000) georgy    (1001)     4494 2023-03-25 17:07:55.000000 mixalime-2.9.8/mixalime/data/OFL.txt
--rw-r--r--   0 georgy    (1000) georgy    (1001)  2417797 2023-03-25 17:07:55.000000 mixalime-2.9.8/mixalime/data/chip.tar.gz
--rw-r--r--   0 georgy    (1000) georgy    (1001)    19318 2023-03-27 07:06:06.000000 mixalime-2.9.8/mixalime/diff.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)    15228 2023-03-25 17:07:55.000000 mixalime-2.9.8/mixalime/export.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)     9040 2023-03-25 17:07:55.000000 mixalime-2.9.8/mixalime/fit.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)    45805 2023-03-25 17:07:55.000000 mixalime-2.9.8/mixalime/main.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)    13606 2023-03-25 17:07:55.000000 mixalime-2.9.8/mixalime/plot.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)     7218 2023-03-25 17:07:55.000000 mixalime-2.9.8/mixalime/tests.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)     4471 2023-03-25 17:07:55.000000 mixalime-2.9.8/mixalime/utils.py
-drwxr-xr-x   0 georgy    (1000) georgy    (1001)        0 2023-03-27 07:08:34.916621 mixalime-2.9.8/mixalime.egg-info/
--rw-r--r--   0 georgy    (1000) georgy    (1001)     4435 2023-03-27 07:08:34.000000 mixalime-2.9.8/mixalime.egg-info/PKG-INFO
--rw-r--r--   0 georgy    (1000) georgy    (1001)      515 2023-03-27 07:08:34.000000 mixalime-2.9.8/mixalime.egg-info/SOURCES.txt
--rw-r--r--   0 georgy    (1000) georgy    (1001)        1 2023-03-27 07:08:34.000000 mixalime-2.9.8/mixalime.egg-info/dependency_links.txt
--rw-r--r--   0 georgy    (1000) georgy    (1001)       48 2023-03-27 07:08:34.000000 mixalime-2.9.8/mixalime.egg-info/entry_points.txt
--rw-r--r--   0 georgy    (1000) georgy    (1001)      219 2023-03-27 07:08:34.000000 mixalime-2.9.8/mixalime.egg-info/requires.txt
--rw-r--r--   0 georgy    (1000) georgy    (1001)        9 2023-03-27 07:08:34.000000 mixalime-2.9.8/mixalime.egg-info/top_level.txt
--rw-r--r--   0 georgy    (1000) georgy    (1001)       38 2023-03-27 07:08:34.916621 mixalime-2.9.8/setup.cfg
--rw-r--r--   0 georgy    (1000) georgy    (1001)     1136 2022-11-01 19:34:12.000000 mixalime-2.9.8/setup.py
+drwxr-xr-x   0 georgy    (1000) georgy    (1001)        0 2023-03-27 18:45:12.313927 mixalime-2.9.9/
+-rw-r--r--   0 georgy    (1000) georgy    (1001)       23 2022-10-30 08:47:57.000000 mixalime-2.9.9/MANIFEST.in
+-rw-r--r--   0 georgy    (1000) georgy    (1001)     4398 2023-03-27 18:45:12.313927 mixalime-2.9.9/PKG-INFO
+-rw-r--r--   0 georgy    (1000) georgy    (1001)     3792 2022-10-30 08:57:43.000000 mixalime-2.9.9/README.md
+drwxr-xr-x   0 georgy    (1000) georgy    (1001)        0 2023-03-27 18:45:12.310593 mixalime-2.9.9/mixalime/
+-rw-r--r--   0 georgy    (1000) georgy    (1001)      965 2023-03-27 18:43:57.000000 mixalime-2.9.9/mixalime/__init__.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)     6058 2023-03-25 17:27:15.000000 mixalime-2.9.9/mixalime/combine.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)    14940 2023-03-25 17:07:55.000000 mixalime-2.9.9/mixalime/create.py
+drwxr-xr-x   0 georgy    (1000) georgy    (1001)        0 2023-03-27 18:45:12.313927 mixalime-2.9.9/mixalime/data/
+-rw-r--r--   0 georgy    (1000) georgy    (1001)   637068 2023-03-25 17:07:55.000000 mixalime-2.9.9/mixalime/data/Lato-Medium.ttf
+-rw-r--r--   0 georgy    (1000) georgy    (1001)   657212 2023-03-25 17:07:55.000000 mixalime-2.9.9/mixalime/data/Lato-Regular.ttf
+-rwxr-xr-x   0 georgy    (1000) georgy    (1001)     4494 2023-03-25 17:07:55.000000 mixalime-2.9.9/mixalime/data/OFL.txt
+-rw-r--r--   0 georgy    (1000) georgy    (1001)  2417797 2023-03-25 17:07:55.000000 mixalime-2.9.9/mixalime/data/chip.tar.gz
+-rw-r--r--   0 georgy    (1000) georgy    (1001)    19336 2023-03-27 18:37:51.000000 mixalime-2.9.9/mixalime/diff.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)    15255 2023-03-27 08:10:48.000000 mixalime-2.9.9/mixalime/export.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)     9040 2023-03-25 17:07:55.000000 mixalime-2.9.9/mixalime/fit.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)    45847 2023-03-27 08:10:37.000000 mixalime-2.9.9/mixalime/main.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)    13606 2023-03-25 17:07:55.000000 mixalime-2.9.9/mixalime/plot.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)     7218 2023-03-25 17:07:55.000000 mixalime-2.9.9/mixalime/tests.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)     4471 2023-03-25 17:07:55.000000 mixalime-2.9.9/mixalime/utils.py
+drwxr-xr-x   0 georgy    (1000) georgy    (1001)        0 2023-03-27 18:45:12.310593 mixalime-2.9.9/mixalime.egg-info/
+-rw-r--r--   0 georgy    (1000) georgy    (1001)     4398 2023-03-27 18:45:12.000000 mixalime-2.9.9/mixalime.egg-info/PKG-INFO
+-rw-r--r--   0 georgy    (1000) georgy    (1001)      515 2023-03-27 18:45:12.000000 mixalime-2.9.9/mixalime.egg-info/SOURCES.txt
+-rw-r--r--   0 georgy    (1000) georgy    (1001)        1 2023-03-27 18:45:12.000000 mixalime-2.9.9/mixalime.egg-info/dependency_links.txt
+-rw-r--r--   0 georgy    (1000) georgy    (1001)       48 2023-03-27 18:45:12.000000 mixalime-2.9.9/mixalime.egg-info/entry_points.txt
+-rw-r--r--   0 georgy    (1000) georgy    (1001)      220 2023-03-27 18:45:12.000000 mixalime-2.9.9/mixalime.egg-info/requires.txt
+-rw-r--r--   0 georgy    (1000) georgy    (1001)        9 2023-03-27 18:45:12.000000 mixalime-2.9.9/mixalime.egg-info/top_level.txt
+-rw-r--r--   0 georgy    (1000) georgy    (1001)       38 2023-03-27 18:45:12.313927 mixalime-2.9.9/setup.cfg
+-rw-r--r--   0 georgy    (1000) georgy    (1001)     1136 2022-11-01 19:34:12.000000 mixalime-2.9.9/setup.py
```

### Comparing `mixalime-2.9.8/PKG-INFO` & `mixalime-2.9.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: mixalime
-Version: 2.9.8
+Version: 2.9.9
 Summary: Identification of allele-specific events in sequencing experiments.
 Home-page: https://github.com/autosome-ru/mixalime
 Author: Georgy Meshcheryakov
 Author-email: iam@georgy.top
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6, <3.10
@@ -77,9 +75,7 @@
 ```
 or
 ```
 > mixalime combine --subname treatment -g group_treatment.tsv combine myproject
 > mixalime combine --subname control -g group_control.tsv combine myproject
 ```
 The `--subname` option is necessary if you wish to avoid different `combine` invocations overriding each other.
-
-
```

### Comparing `mixalime-2.9.8/README.md` & `mixalime-2.9.9/README.md`

 * *Files identical despite different names*

### Comparing `mixalime-2.9.8/mixalime/__init__.py` & `mixalime-2.9.9/mixalime/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-__version__ = '2.9.8'
+__version__ = '2.9.9'
 import importlib
 
 __min_reqs__ = [
             'pip>=23.0',
             'typer>=0.6.1',
             'numpy>=1.23.4',
             'jax>=0.4.4',
             'jaxlib>=0.4.4',
             'matplotlib>=3.5.1',
             'pandas>=1.4.1',
-            'scipy>=1.9.3',
+            'scipy>=1.10.1',
             'statsmodels>=0.13.2',
             'betanegbinfit>=1.7.4',
             'datatable>=1.0.0',
             'dill>=0.3.6',
             'rich>=12.6.0',
             'portion>=2.3.0',
             'pysam>=0.19.1'
```

### Comparing `mixalime-2.9.8/mixalime/combine.py` & `mixalime-2.9.9/mixalime/combine.py`

 * *Files identical despite different names*

### Comparing `mixalime-2.9.8/mixalime/create.py` & `mixalime-2.9.9/mixalime/create.py`

 * *Files identical despite different names*

### Comparing `mixalime-2.9.8/mixalime/data/Lato-Medium.ttf` & `mixalime-2.9.9/mixalime/data/Lato-Medium.ttf`

 * *Files identical despite different names*

### Comparing `mixalime-2.9.8/mixalime/data/Lato-Regular.ttf` & `mixalime-2.9.9/mixalime/data/Lato-Regular.ttf`

 * *Files identical despite different names*

### Comparing `mixalime-2.9.8/mixalime/data/OFL.txt` & `mixalime-2.9.9/mixalime/data/OFL.txt`

 * *Files identical despite different names*

### Comparing `mixalime-2.9.8/mixalime/data/chip.tar.gz` & `mixalime-2.9.9/mixalime/data/chip.tar.gz`

 * *Files identical despite different names*

### Comparing `mixalime-2.9.8/mixalime/diff.py` & `mixalime-2.9.9/mixalime/diff.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
         if steps:
             ps = list(np.linspace(0.01, 0.99, steps))
             i = np.nanargmin(list(map(f, ps)))
             ps = [0.0] + ps + [1.0]
             b = ps[i], ps[i + 2]
         else:
             b = (0.0, 1.0)
-        return minimize_scalar(f, bounds=b, options={'xatol': xatol, 'maxiter': 200})
+        return minimize_scalar(f, bounds=b, method='bounded', options={'xatol': xatol, 'maxiter': 200})
     
     def adjust_r(self, r, k, w=None):
         bad = self.bad
         if w is None or bad == 1:
             return r
         p2 = 1 / (bad + 1)
         p1 = 1 - p2
```

### Comparing `mixalime-2.9.8/mixalime/export.py` & `mixalime-2.9.9/mixalime/export.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,15 +159,15 @@
         folder = folder.lstrip('/\\')
         folder = os.path.join(out, folder)
         file = get_name(file) + '.pvalue.tsv'
         file = os.path.join(folder, file)
         os.makedirs(folder, exist_ok=True)
         pd.DataFrame(d).to_csv(file, sep='\t', index=None)
 
-def export_combined_pvalues(project, out: str, rep_info=False, subname=None):
+def export_combined_pvalues(project, out: str, sample_info=False, subname=None):
     if type(project) is str:
         file = get_init_file(project)
         compression = file.split('.')[-1]
         open = openers[compression]
         with open(file, 'rb') as snvs, open(f'{project}.test.{compression}', 'rb') as test, open(f'{project}.comb.{compression}', 'rb') as comb:
             snvs = dill.load(snvs)
             test = dill.load(test)
@@ -212,15 +212,15 @@
         ref_pvals = ','.join(ref_pvals); alt_pvals = ','.join(alt_pvals)
         ref_eses = ','.join(ref_eses); alt_eses = ','.join(alt_eses)
         n = len(scores_f)
         scores_f = ','.join(scores_f)
         d['#chr'].append(chr); d['start'].append(pos); d['end'].append(end); d['mean_bad'].append(mean_bad); d['id'].append(name)
         d['ref'].append(ref); d['alt'].append(alt); d['n_reps'].append(n);
         
-        if rep_info:
+        if sample_info:
             d['bads'].append(bads)
             d['scorefiles'].append(scores_f)
             d['ref_counts'].append(ref_counts); d['alt_counts'].append(alt_counts); d['ref_es'].append(ref_eses); d['alt_es'].append(alt_eses)
             d['ref_pval'].append(ref_pvals); d['alt_pval'].append(alt_pvals); 
         d['ref_comb_es'].append(es_ref); d['alt_comb_es'].append(es_alt)
         d['ref_comb_pval'].append(pval_ref); d['alt_comb_pval'].append(pval_alt)
         d['ref_fdr_comb_pval'].append(fdr_ref); d['alt_fdr_comb_pval'].append(fdr_alt)
@@ -232,15 +232,15 @@
         d['comb_es'].append(es); d['comb_pval'].append(pval); d['fdr_comb_pval'].append(fdr)
         
     folder, _ = os.path.split(out)
     if folder:
         os.makedirs(folder, exist_ok=True)
     pd.DataFrame(d).to_csv(out, sep='\t', index=None)
 
-def export_difftests(project, out: str,  rep_info=False, subname=None):
+def export_difftests(project, out: str,  sample_info=False, subname=None):
     if type(project) is str:
         file = get_init_file(project)
         compression = file.split('.')[-1]
         open = openers[compression]
         with open(file, 'rb') as snvs,  open(f'{project}.difftest.{compression}', 'rb') as diff:
             diff = dill.load(diff)[subname]
     else:
@@ -282,15 +282,15 @@
         # alt_es_count.append(np.log2(b_es_alt_ref) - np.log2(a_es_alt_ref))
         bad.append(sum(bads) / len(bads))
         a_ref_counts.append(','.join(a_ref_count))
         b_ref_counts.append(','.join(b_ref_count))
         a_alt_counts.append(','.join(a_alt_count))
         b_alt_counts.append(','.join(b_alt_count))
     diff = tests.drop('ind', axis=1)
-    if rep_info:
+    if sample_info:
         df = pd.DataFrame({'#chr': chrom, 'start': start, 'end': end, 'mean_bad': bad, 'id': name, 'ref': ref, 'alt': alt,
                            'a_ref_counts': a_ref_counts, 'a_alt_counts': a_alt_counts, 
                            'b_ref_counts': b_ref_counts, 'b_alt_counts': b_alt_counts})
     else:
         df = pd.DataFrame({'#chr': chrom, 'start': start, 'end': end, 'mean_bad': bad, 'id': name, 'ref': ref, 'alt': alt })
     diff = pd.concat([df, diff], axis=1)
     # diff['ref_es_count'] = ref_es_count
@@ -316,15 +316,15 @@
         diff.loc[~t, col] = diff.loc[~t, f'alt_{col}']
     folder, _ = os.path.split(out)
     if folder:
         os.makedirs(folder, exist_ok=True)
     diff.to_csv(out, sep='\t', index=None)
 
 
-def export_all(name: str, out: str, rep_info: bool = None):
+def export_all(name: str, out: str, sample_info: bool = None):
     file = get_init_file(name)
     compression = file.split('.')[-1]
     open = openers[compression]
     with open(file, 'rb') as init:
         init = dill.load(init)
     export_counts(init, out)
     try:
@@ -337,15 +337,15 @@
     try:
         with open(f'{name}.difftest.{compression}', 'rb') as f:
             difftests = dill.load(f)
             subfolder = os.path.join(out, 'difftest')
             t = (init, difftests)
             for subname in difftests:
                 export_difftests(t, os.path.join(subfolder, f'{subname}.tsv' if subname else 'difftests.tsv'), subname=subname,
-                                 rep_info=rep_info)
+                                 sample_info=sample_info)
     except FileNotFoundError:
         pass     
             
     try:
         with open(f'{name}.test.{compression}', 'rb') as f:
             raw_pvals = dill.load(f)
     except FileNotFoundError:
@@ -355,14 +355,14 @@
     try:
         with open(f'{name}.comb.{compression}', 'rb') as f:
             pvals = dill.load(f)
     except FileNotFoundError:
         return
     t = (init, raw_pvals, pvals)
     for subname in pvals:
-        export_combined_pvalues(t, os.path.join(out, f'{subname}.tsv' if subname else 'pvals.tsv'), subname=subname, rep_info=rep_info)
+        export_combined_pvalues(t, os.path.join(out, f'{subname}.tsv' if subname else 'pvals.tsv'), subname=subname, sample_info=sample_info)
 
 def export_demo(path: str = str()):
     folder = os.path.join(os.path.split(os.path.realpath(__file__))[0], 'data')
     filename = os.path.join(folder, 'chip.tar.gz')
     with tarfile.open(filename, 'r:gz') as f:
         f.extractall(os.path.join(path, 'scorefiles'))
```

### Comparing `mixalime-2.9.8/mixalime/fit.py` & `mixalime-2.9.9/mixalime/fit.py`

 * *Files identical despite different names*

### Comparing `mixalime-2.9.8/mixalime/main.py` & `mixalime-2.9.9/mixalime/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -610,27 +610,27 @@
         print(f'✔️ Done!\t time: {dt:.2f} s.')
     return expected_res
 
 
 
 @app_export.command('all', help='Export everything.')
 def _export_all(name: str = Argument(..., help='Project name.'), out: Path = Argument(..., help='Output filename/path.'),
-                rep_info: bool = Option(False, help='Include raw p-values and names of sample scorefiles to the tabular. '
-                                                    'Note that this may bloat output if number of samples is high.'),
+                sample_info: bool = Option(False, help='Include raw p-values and names of sample scorefiles to the tabular. '
+                                                       'Note that this may bloat output if number of samples is high.'),
                 pretty: bool = Option(True, help='Use "rich" package to produce eye-candy output.')):
     out = str(out)
     t0 = time()
     if pretty:
         p = Progress(SpinnerColumn(speed=0.5), TextColumn("[progress.description]{task.description}"), transient=True)
         p.add_task(description="Exporting tabular data...", total=None)
         p.start()
-    export.export_all(name, out, rep_info=rep_info)
+    export.export_all(name, out, sample_info=sample_info)
     if pretty:
         p.stop()
-    update_history(name, 'export', out=out, rep_info=rep_info)
+    update_history(name, 'export', out=out, sample_info=sample_info)
     dt = time() - t0
     if pretty:
         rprint(f'[green][bold]✔️[/bold] Done![/green]\t time: {dt:.2f} s.')
     else:
         print(f'✔️ Done!\t time: {dt:.2f} s.')
 
 @app_export.command('counts')
@@ -689,25 +689,25 @@
         rprint('[green][bold]✔️[/bold] Done![/green]')
     else:
         print('✔️ Done!')
 
 
 @app_export.command('pvalues')
 def _combined_pvalues(name: str = Argument(..., help='Project name.'), out: Path = Argument(..., help='Output filename/path.'),
-                      rep_info: bool = Option(False, help='Include raw p-values and names of sample scorefiles to the tabular. '
+                      sample_info: bool = Option(False, help='Include raw p-values and names of sample scorefiles to the tabular. '
                                                           'Note that this may bloat output if number of samples is high.'),
                       subname: str = Option(None, help='A subname that can be used to reference a set of combined p-values in case if you'
                                                        ' provided one at [cyan bold]combine[/cyan bold] step.'),
                       pretty: bool = Option(True, help='Use "rich" package to produce eye-candy output.')):
     '''
     Export combined across samples and FDR-corrected p-values.
     '''
     out = str(out)
-    export.export_combined_pvalues(name, out, rep_info=rep_info, subname=subname)
-    update_history(name, 'export pvalues', out=out, rep_info=rep_info, subname=subname)
+    export.export_combined_pvalues(name, out, sample_info=sample_info, subname=subname)
+    update_history(name, 'export pvalues', out=out, sample_info=sample_info, subname=subname)
     if pretty:
         rprint('[green][bold]✔️[/bold] Done![/green]')
     else:
         print('✔️ Done!')
 
 
 help_str = 'Export "raw" pvalues (i.e. prior to combining them across samples and FDR-corrections). '\
@@ -725,22 +725,22 @@
         print('✔️ Done!')
 
 
 @app_export.command('difftest')
 def _difftests(name: str = Argument(..., help='Project name.'), out: Path = Argument(..., help='Output filename/path.'),
                       subname: str = Option(None, help='A subname that can be used to reference a set of combined p-values in case if you'
                                                        ' provided one at [cyan bold]difftest[/cyan bold] step.'),
-                      rep_info: bool = Option(False, help='Include ref, alt counts and names of sample scorefiles to the tabular. '
+                      sample_info: bool = Option(False, help='Include ref, alt counts and names of sample scorefiles to the tabular. '
                                                           'Note that this may bloat output if number of samples is high.'),
                       pretty: bool = Option(True, help='Use "rich" package to produce eye-candy output.')):
     '''
     Export FDR-corrected p-values for differential test.
     '''
     out = str(out)
-    export.export_difftests(name, out, subname=subname, rep_info=rep_info)
+    export.export_difftests(name, out, subname=subname, sample_info=sample_info)
     update_history(name, 'export difftest', out=out, subname=subname)
     if pretty:
         rprint('[green][bold]✔️[/bold] Done![/green]')
     else:
         print('✔️ Done!')
 
 @app_export.command('demo')
```

### Comparing `mixalime-2.9.8/mixalime/plot.py` & `mixalime-2.9.9/mixalime/plot.py`

 * *Files identical despite different names*

### Comparing `mixalime-2.9.8/mixalime/tests.py` & `mixalime-2.9.9/mixalime/tests.py`

 * *Files identical despite different names*

### Comparing `mixalime-2.9.8/mixalime/utils.py` & `mixalime-2.9.9/mixalime/utils.py`

 * *Files identical despite different names*

### Comparing `mixalime-2.9.8/mixalime.egg-info/PKG-INFO` & `mixalime-2.9.9/mixalime.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: mixalime
-Version: 2.9.8
+Version: 2.9.9
 Summary: Identification of allele-specific events in sequencing experiments.
 Home-page: https://github.com/autosome-ru/mixalime
 Author: Georgy Meshcheryakov
 Author-email: iam@georgy.top
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6, <3.10
@@ -77,9 +75,7 @@
 ```
 or
 ```
 > mixalime combine --subname treatment -g group_treatment.tsv combine myproject
 > mixalime combine --subname control -g group_control.tsv combine myproject
 ```
 The `--subname` option is necessary if you wish to avoid different `combine` invocations overriding each other.
-
-
```

### Comparing `mixalime-2.9.8/mixalime.egg-info/SOURCES.txt` & `mixalime-2.9.9/mixalime.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mixalime-2.9.8/setup.py` & `mixalime-2.9.9/setup.py`

 * *Files identical despite different names*

