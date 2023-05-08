# Comparing `tmp/panfeed-1.2.1.tar.gz` & `tmp/panfeed-1.3.0.tar.gz`

## Comparing `panfeed-1.2.1.tar` & `panfeed-1.3.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 panfeed-1.2.1/environment.yml
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 panfeed-1.2.1/make_release.txt
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 panfeed-1.2.1/panfeed-get-clusters-runner.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 panfeed-1.2.1/panfeed-get-kmers-runner.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 panfeed-1.2.1/panfeed-plot-runner.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 panfeed-1.2.1/panfeed-runner.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 panfeed-1.2.1/panfeed/__init__.py
--rw-r--r--   0        0        0    12672 2020-02-02 00:00:00.000000 panfeed-1.2.1/panfeed/__main__.py
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 panfeed-1.2.1/panfeed/classes.py
--rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 panfeed-1.2.1/panfeed/colorlog.py
--rw-r--r--   0        0        0     3459 2020-02-02 00:00:00.000000 panfeed-1.2.1/panfeed/get_clusters.py
--rw-r--r--   0        0        0     4491 2020-02-02 00:00:00.000000 panfeed-1.2.1/panfeed/get_kmers.py
--rw-r--r--   0        0        0    13821 2020-02-02 00:00:00.000000 panfeed-1.2.1/panfeed/input.py
--rw-r--r--   0        0        0     9235 2020-02-02 00:00:00.000000 panfeed-1.2.1/panfeed/panfeed.py
--rw-r--r--   0        0        0    16055 2020-02-02 00:00:00.000000 panfeed-1.2.1/panfeed/plot.py
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 panfeed-1.2.1/LICENSE
--rw-r--r--   0        0        0     6516 2020-02-02 00:00:00.000000 panfeed-1.2.1/README.md
--rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 panfeed-1.2.1/pyproject.toml
--rw-r--r--   0        0        0    20337 2020-02-02 00:00:00.000000 panfeed-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 panfeed-1.3.0/environment.yml
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 panfeed-1.3.0/make_release.txt
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 panfeed-1.3.0/panfeed-get-clusters-runner.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 panfeed-1.3.0/panfeed-get-kmers-runner.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 panfeed-1.3.0/panfeed-plot-runner.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 panfeed-1.3.0/panfeed-runner.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 panfeed-1.3.0/panfeed/__init__.py
+-rw-r--r--   0        0        0    13003 2020-02-02 00:00:00.000000 panfeed-1.3.0/panfeed/__main__.py
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 panfeed-1.3.0/panfeed/classes.py
+-rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 panfeed-1.3.0/panfeed/colorlog.py
+-rw-r--r--   0        0        0     3459 2020-02-02 00:00:00.000000 panfeed-1.3.0/panfeed/get_clusters.py
+-rw-r--r--   0        0        0     4491 2020-02-02 00:00:00.000000 panfeed-1.3.0/panfeed/get_kmers.py
+-rw-r--r--   0        0        0    14576 2020-02-02 00:00:00.000000 panfeed-1.3.0/panfeed/input.py
+-rw-r--r--   0        0        0     9235 2020-02-02 00:00:00.000000 panfeed-1.3.0/panfeed/panfeed.py
+-rw-r--r--   0        0        0    16055 2020-02-02 00:00:00.000000 panfeed-1.3.0/panfeed/plot.py
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 panfeed-1.3.0/LICENSE
+-rw-r--r--   0        0        0     6516 2020-02-02 00:00:00.000000 panfeed-1.3.0/README.md
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 panfeed-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0    20337 2020-02-02 00:00:00.000000 panfeed-1.3.0/PKG-INFO
```

### Comparing `panfeed-1.2.1/panfeed/__main__.py` & `panfeed-1.3.0/panfeed/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -199,14 +199,20 @@
                         default = 3,
                         help = "limit on items that may be put into the reading"
                                "and writing queues. (default: %(default)d)"
                                "this option is only relevant for cores > 1"
                                "reading queue limit = ql * cores"
                                "writing queue limit = ql")
 
+    parser.add_argument("--stop-on-missing",
+                        action = "store_true",
+                        default = False,
+                        help = "Crash if samples/chromosomes/genes "
+                               "are not found (default: throw warnings)")
+
     parser.add_argument("-v", action='count',
                         default=0,
                         help='Increase verbosity level')
     parser.add_argument('--version', action='version',
                         version='%(prog)s '+__version__)
 
     return parser.parse_args()
@@ -257,15 +263,16 @@
     logger.info("Extracting k-mers")
     iter_i = iter_gene_clusters(genepres, 
                                 data,
                                 args.upstream,
                                 args.downstream,
                                 args.downstream_start_codon,
                                 not args.no_filter,
-                                genes)
+                                genes,
+                                args.stop_on_missing)
     iter_o = partial(cluster_cutter,
                      klength=klength,
                      stroi=stroi,
                      multiple_files=args.multiple_files,
                      canon=not args.non_canonical,
                      consider_missing_cluster=args.consider_missing,
                      output=args.output,
```

### Comparing `panfeed-1.2.1/panfeed/classes.py` & `panfeed-1.3.0/panfeed/classes.py`

 * *Files identical despite different names*

### Comparing `panfeed-1.2.1/panfeed/colorlog.py` & `panfeed-1.3.0/panfeed/colorlog.py`

 * *Files identical despite different names*

### Comparing `panfeed-1.2.1/panfeed/get_clusters.py` & `panfeed-1.3.0/panfeed/get_clusters.py`

 * *Files identical despite different names*

### Comparing `panfeed-1.2.1/panfeed/get_kmers.py` & `panfeed-1.3.0/panfeed/get_kmers.py`

 * *Files identical despite different names*

### Comparing `panfeed-1.2.1/panfeed/input.py` & `panfeed-1.3.0/panfeed/input.py`

 * *Files 4% similar despite different names*

```diff
@@ -259,25 +259,27 @@
                 logger.warning(f'{e}, skipping line "{line.rstrip()}" from {file_name}')                
                 continue
     
     return features
 
 
 def iter_gene_clusters(panaroo, genome_data, up, down, down_start_codon, patfilt,
-                       gene_list=None):
+                       gene_list=None, raise_missing=False):
     # check if we have genome data for all
     # strains in the pangenome
     # if not give a warning
     all_strains = set(panaroo.columns)
     missing_strains = all_strains.difference(genome_data.keys())
     if len(missing_strains) > 0:
         logger.warning(f'There are {len(missing_strains)} strains present '
                        'in the pangenome table but not in the GFF directory')
         for strain in missing_strains:
             logger.debug(f'Missing GFF file: {strain}')
+        if raise_missing:
+            raise KeyError(f'Missing {len(missing_strains)} from the GFF directory')
 
     # go through each gene cluster
     all_ogs = panaroo.shape[0]
     for i, (idx, row) in enumerate(panaroo.iterrows()):
         if gene_list is not None and idx not in gene_list:
             logger.debug(f"Skipping {idx} ({i+1}/{all_ogs})")
             continue
@@ -320,14 +322,25 @@
             for gene in genes.split(';'):
                 # access a particular gene
                 try:
                     feat = features[gene]
                 except KeyError:
                     # e.g. refound genes are not in the GFF
                     logger.warning(f"Could not find gene {gene} from {idx} in {strain}")
+                    if raise_missing:
+                        raise KeyError(f"Could not find gene {gene} from {idx} in {strain}")
+                    continue
+                # double check if the chromosome is in the fasta file
+                try:
+                    sequences[feat.chromosome]
+                except KeyError:
+                    # e.g. refound genes are not in the GFF
+                    logger.warning(f"Could not find chromosome {feat.chromosome} in {strain}")
+                    if raise_missing:
+                        raise KeyError(f"Could not find chromosome {feat.chromosome} in {strain}")
                     continue
                 
                 # corner case: upstream offset is over the contig's edge
                 # adjust if so and save the true offset
                 if feat.strand > 0 and feat.start-1-up < 0:
                     offset = feat.start - 1
                 elif feat.strand < 0 and feat.end+up > len(sequences[feat.chromosome]):
```

### Comparing `panfeed-1.2.1/panfeed/panfeed.py` & `panfeed-1.3.0/panfeed/panfeed.py`

 * *Files identical despite different names*

### Comparing `panfeed-1.2.1/panfeed/plot.py` & `panfeed-1.3.0/panfeed/plot.py`

 * *Files identical despite different names*

### Comparing `panfeed-1.2.1/LICENSE` & `panfeed-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `panfeed-1.2.1/README.md` & `panfeed-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `panfeed-1.2.1/pyproject.toml` & `panfeed-1.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `panfeed-1.2.1/PKG-INFO` & `panfeed-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panfeed
-Version: 1.2.1
+Version: 1.3.0
 Summary: Compute gene-cluster specific k-mers over a pangenome
 Project-URL: Homepage, https://github.com/microbial-pangenomes-lab/panfeed
 Project-URL: Bug Tracker, https://github.com/microbial-pangenomes-lab/panfeed/issues
 Author-email: Hannes Neubauer <neubauer.hannes@mh-hannover.de>, Marco Galardini <galardini.marco@mh-hannover.de>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

