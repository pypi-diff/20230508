# Comparing `tmp/hummuspy-0.0.4.tar.gz` & `tmp/hummuspy-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hummuspy-0.0.4.tar", max compression
+gzip compressed data, was "hummuspy-0.0.5.tar", max compression
```

## Comparing `hummuspy-0.0.4.tar` & `hummuspy-0.0.5.tar`

### file list

```diff
@@ -1,7 +1,10 @@
--rw-r--r--   0        0        0        0 2023-04-04 11:48:19.958459 hummuspy-0.0.4/LICENSE
--rw-r--r--   0        0        0       46 2023-04-04 12:00:32.696076 hummuspy-0.0.4/README.md
--rw-r--r--   0        0        0      584 2023-04-05 15:00:18.300208 hummuspy-0.0.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-04 12:51:39.859533 hummuspy-0.0.4/src/hummuspy/__init__.py
--rw-r--r--   0        0        0       42 2023-04-04 12:58:18.183124 hummuspy-0.0.4/src/hummuspy/example.py
--rw-r--r--   0        0        0    14828 2023-04-05 14:59:45.787952 hummuspy-0.0.4/src/hummuspy/explore_network.py
--rw-r--r--   0        0        0      992 1970-01-01 00:00:00.000000 hummuspy-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-04 11:48:19.958459 hummuspy-0.0.5/LICENSE
+-rw-r--r--   0        0        0       46 2023-04-04 12:00:32.696076 hummuspy-0.0.5/README.md
+-rw-r--r--   0        0        0      585 2023-05-08 11:45:57.232054 hummuspy-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0    37274 2023-04-05 16:53:37.048925 hummuspy-0.0.5/src/hummuspy/.ipynb_checkpoints/Untitled-checkpoint.ipynb
+-rw-r--r--   0        0        0     6051 2023-04-05 17:15:37.384728 hummuspy-0.0.5/src/hummuspy/Untitled.ipynb
+-rw-r--r--   0        0        0        0 2023-04-04 12:51:39.859533 hummuspy-0.0.5/src/hummuspy/__init__.py
+-rw-r--r--   0        0        0     3627 2023-05-08 11:39:34.811147 hummuspy-0.0.5/src/hummuspy/config.py
+-rw-r--r--   0        0        0       42 2023-04-04 12:58:18.183124 hummuspy-0.0.5/src/hummuspy/example.py
+-rw-r--r--   0        0        0    15206 2023-05-08 09:02:31.288706 hummuspy-0.0.5/src/hummuspy/explore_network.py
+-rw-r--r--   0        0        0      992 1970-01-01 00:00:00.000000 hummuspy-0.0.5/PKG-INFO
```

### Comparing `hummuspy-0.0.4/pyproject.toml` & `hummuspy-0.0.5/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hummuspy"
-version = "0.0.4"
+version = "0.0.5"
 description = "HuMMuS is a novel method for the inference of regulatory mechanisms from multi-omics data with any type and number of omics, thorugh a heterogeneous multilayer networks framework."
 authors = ["Rémi Trimbour <remi.trimbour@pasteur.fr>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8"
@@ -13,8 +13,8 @@
 tqdm = "^4.65.0"
 numpy = "^1.24.2"
 pandas = "^2.0.0"
 pyyaml = "^6.0"
 
 [build-system]
 requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+build-backend = "poetry.core.masonry.api"
```

### Comparing `hummuspy-0.0.4/src/hummuspy/explore_network.py` & `hummuspy-0.0.5/src/hummuspy/explore_network.py`

 * *Files 11% similar despite different names*

```diff
@@ -204,73 +204,73 @@
     config['eta']  = [eta for _, eta  in sorted(zip(layers_names, layers_eta))]
     
     with open(filename, 'w') as f:
         yaml.dump(config, f)
 
     if return_config:
         return config
-    
-    
+
+
 def compute_multiple_RandomWalk(
-    multilayer_f, 
-    config_name, 
-    output_f, 
-    list_seeds, 
-    config_folder = 'config',
-    save=True, 
-    Return=False, 
-    spec_layer_result_saved='all', 
+    multilayer_f,
+    config_name,
+    output_f,
+    list_seeds,
+    config_folder='config',
+    save=True,
+    Return=False,
+    spec_layer_result_saved='all',
     njobs=1):
-    
+
     ranking_all_dfs = pd.DataFrame(columns = ['layer', 'target', 'path_layer', 'score', 'tf'])
 
     l_ranking_df = Parallel(n_jobs=njobs)(delayed(compute_RandomWalk)(multilayer_f, config_name, seeds, config_folder, spec_layer_result_saved) for seeds in tqdm(list_seeds))
     ranking_all_dfs = pd.concat([ranking_all_dfs]+l_ranking_df)
-    
+
     if save:
         ranking_all_dfs.sort_values(by='score').to_csv(output_f, sep='\t', index=False, header=True)
     if Return:
         return ranking_all_dfs
 
 def compute_RandomWalk(
     multilayer_f,
     config_name,
     seeds,
-    config_folder = 'config',
+    config_folder='config',
     spec_layer_result_saved='all',
     unnamed=False,
     njobs=1):
-    
-    #seeds file names
-    seeds = make_values_list(seeds) 
-    if unnamed == True:
-        seeds_filename = 'seeds.txt'        
+
+    # seeds file names
+    seeds = make_values_list(seeds)
+    if unnamed is True:
+        seeds_filename = 'seeds.txt'
         if njobs>1:
             raise Exception("Impossible to use unnamed seeds files while parallelising random walks.")
     else:
         seeds_filename = '_'.join(seeds)
 
-    #write seeds file
+    # write seeds file
     with open(multilayer_f+'/seeds/'+seeds_filename+'.txt', 'w') as f:
         f.write('\n'.join(seeds)+'\n')        
     
-    #config file personalised with seed file
+    # config file personalised with seed file
     with open(multilayer_f+'/{}/'.format(config_folder)+config_name, 'r') as f:
         config = yaml.load(f, Loader=yaml.BaseLoader)
         config['seed'] = 'seeds/'+seeds_filename+'.txt'
     with open(multilayer_f+'/{}/'.format(config_folder)+seeds_filename+'_'+config_name, 'w') as f:
         yaml.dump(config, f)
         
     # multixrank
     multixrank_obj = mxr.Multixrank(config=multilayer_f+'/{}/'.format(config_folder)+seeds_filename+'_'+config_name, wdir=multilayer_f)
     ranking_df = multixrank_obj.random_walk_rank()
     
     # and filter df results andadd seeds name
     ranking_df['tf'] = '_'.join(seeds)
-    ranking_df = ranking_df[ranking_df.score>0] #??
+    ranking_df = ranking_df[ranking_df.score > 0]  # ??
     ranking_df.columns = ['layer', 'target', 'path_layer', 'score', 'seed']
     if spec_layer_result_saved != 'all':
         if type(spec_layer_result_saved)==str:
             spec_layer_result_saved = [spec_layer_result_saved]
         ranking_df = ranking_df[ranking_df['layer'].isin(spec_layer_result_saved)]
 
     return ranking_df
@@ -285,16 +285,16 @@
     njobs:int = 1,
     target_saved: typing.Union['genes', 'peaks', 'tfs'] = 'genes',
     tf_layers: typing.Union[str, list[str], dict[str]] = 'tf_edges.tsv',
     atac_layers: typing.Union[str, list[str], dict[str]] = 'peak_edges.tsv',
     rna_layers: typing.Union[str, list[str], dict[str]] = 'gene_edges.tsv',
     tf_atac_links: str = 'bipartite/tfs2peaks.tsv', 
     atac_rna_links: str = 'bipartite/peaks2genes.tsv',
-    config_name = 'grn_config.yml',
-    config_folder = 'config',
+    config_name='grn_config.yml',
+    config_folder='config',
     seed_path: str = 'seeds/seeds.txt',
     folder_tf_layers: str = 'multiplex/layer_TFS',
     folder_atac_layers: str = 'multiplex/layer_PEAKS',
     folder_rna_layers: str = 'multiplex/layer_GENES',
     tf_layers_weighted: typing.Union[bool, list[bool], dict[bool]] = False, 
     atac_layers_weighted: typing.Union[bool, list[bool], dict[bool]] = True, 
     rna_layers_weighted: typing.Union[bool, list[bool], dict[bool]] = True,
@@ -305,53 +305,66 @@
     atac_rna_links_weighted: bool = False,
     tf_atac_links_directed: bool = False, 
     atac_rna_links_directed: bool = False,
     r:float = 0.7,
     self_loops: bool = 0):
 
     detailed_config(
-        request = 'grn',
-        filename = multilayer_f+'/'+config_folder+'/'+config_name,
+        request='grn',
+        filename=multilayer_f+'/'+config_folder+'/'+config_name,
         tf_layers=tf_layers,
         atac_layers=atac_layers,
         rna_layers=rna_layers,
-        tf_atac_links=tf_atac_links, 
+        tf_atac_links=tf_atac_links,
         atac_rna_links=atac_rna_links,
         seed_path=seed_path,
-        folder_tf_layers = folder_tf_layers,
-        folder_atac_layers = folder_atac_layers,
-        folder_rna_layers = folder_rna_layers,
-        tf_layers_weighted=tf_layers_weighted, 
-        atac_layers_weighted=atac_layers_weighted, 
+        folder_tf_layers=folder_tf_layers,
+        folder_atac_layers=folder_atac_layers,
+        folder_rna_layers=folder_rna_layers,
+        tf_layers_weighted=tf_layers_weighted,
+        atac_layers_weighted=atac_layers_weighted,
         rna_layers_weighted=rna_layers_weighted,
-        tf_layers_directed=tf_layers_directed, 
-        atac_layers_directed=atac_layers_directed, 
+        tf_layers_directed=tf_layers_directed,
+        atac_layers_directed=atac_layers_directed,
         rna_layers_directed=rna_layers_directed,
         tf_atac_links_weighted=tf_atac_links_weighted,
         atac_rna_links_weighted=atac_rna_links_weighted,
-        tf_atac_links_directed=tf_atac_links_directed, 
+        tf_atac_links_directed=tf_atac_links_directed,
         atac_rna_links_directed=atac_rna_links_directed,
         r=r,
-        self_loops = self_loops,
-        return_config = False)
+        self_loops=self_loops,
+        return_config=False)
     
     if TFs == 'all':
         TFs = list(pd.read_csv(multilayer_f + '/' + tf_atac_links, sep="\t", header=None)[0].str.strip().unique())
     TFs = make_values_list(TFs)
     
     rna_layers = make_values_list(rna_layers)
     print([folder_rna_layers+'/'+rna_layer for rna_layer in rna_layers])
 
+    if Return is True:
+        grn = compute_multiple_RandomWalk(
+            multilayer_f=multilayer_f,
+            config_name=config_name,
+            output_f=output_f_grn,
+            list_seeds=TFs,
+            config_folder=config_folder,
+            save=save,
+            Return=Return,
+            spec_layer_result_saved=folder_rna_layers,
+            njobs=njobs)
+        return grn
+    else:
+        grn = compute_multiple_RandomWalk(
+            multilayer_f=multilayer_f,
+            config_name=config_name,
+            output_f=output_f_grn,
+            list_seeds=TFs,
+            config_folder=config_folder,
+            save=save,
+            Return=Return,
+            spec_layer_result_saved=folder_rna_layers,
+            njobs=njobs)
+
 
-    compute_multiple_RandomWalk(
-        multilayer_f = multilayer_f, 
-        config_name = config_name, 
-        output_f=output_f_grn, 
-        list_seeds = TFs, 
-        config_folder = config_folder,
-        save=True, 
-        Return=False, 
-        spec_layer_result_saved=folder_rna_layers, 
-        njobs=njobs)
-    
-#multilayer_f = '../../flattened_networks/ML_hESC_Chen_GeneNW_all_Peaks2Genes_UP0.5K_DOWN0.5K_nofilt_nofilt_TFlayer_nolinks'
-#define_grn(multilayer_f, njobs=45)
+# multilayer_f = '../../flattened_networks/ML_hESC_Chen_GeneNW_all_Peaks2Genes_UP0.5K_DOWN0.5K_nofilt_nofilt_TFlayer_nolinks'
+# define_grn(multilayer_f, njobs=45)
```

### Comparing `hummuspy-0.0.4/PKG-INFO` & `hummuspy-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hummuspy
-Version: 0.0.4
+Version: 0.0.5
 Summary: HuMMuS is a novel method for the inference of regulatory mechanisms from multi-omics data with any type and number of omics, thorugh a heterogeneous multilayer networks framework.
 License: GPL-3.0-only
 Author: Rémi Trimbour
 Author-email: remi.trimbour@pasteur.fr
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

