# Comparing `tmp/cdot-0.2.8.tar.gz` & `tmp/cdot-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdot-0.2.8.tar", last modified: Mon Aug 29 12:15:47 2022, max compression
+gzip compressed data, was "cdot-0.2.9.tar", last modified: Thu Sep  1 02:28:17 2022, max compression
```

## Comparing `cdot-0.2.8.tar` & `cdot-0.2.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 dlawrence  (1000) dlawrence  (1000)        0 2022-08-29 12:15:47.672525 cdot-0.2.8/
--rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)     1062 2022-06-27 00:48:45.000000 cdot-0.2.8/LICENSE
--rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)     4670 2022-08-29 12:15:47.672525 cdot-0.2.8/PKG-INFO
--rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)     4192 2022-08-29 12:11:13.000000 cdot-0.2.8/README.md
-drwxrwxr-x   0 dlawrence  (1000) dlawrence  (1000)        0 2022-08-29 12:15:47.668525 cdot-0.2.8/cdot/
--rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)      242 2022-08-29 03:34:48.000000 cdot-0.2.8/cdot/__init__.py
-drwxrwxr-x   0 dlawrence  (1000) dlawrence  (1000)        0 2022-08-29 12:15:47.668525 cdot-0.2.8/cdot/gff/
--rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)        0 2022-06-27 00:48:45.000000 cdot-0.2.8/cdot/gff/__init__.py
--rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)    22227 2022-08-29 07:24:41.000000 cdot-0.2.8/cdot/gff/gff_parser.py
-drwxrwxr-x   0 dlawrence  (1000) dlawrence  (1000)        0 2022-08-29 12:15:47.668525 cdot-0.2.8/cdot/hgvs/
--rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)        0 2022-06-27 00:48:45.000000 cdot-0.2.8/cdot/hgvs/__init__.py
-drwxrwxr-x   0 dlawrence  (1000) dlawrence  (1000)        0 2022-08-29 12:15:47.668525 cdot-0.2.8/cdot/hgvs/dataproviders/
--rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)       34 2022-06-27 00:48:45.000000 cdot-0.2.8/cdot/hgvs/dataproviders/__init__.py
--rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)    12357 2022-08-29 11:49:45.000000 cdot-0.2.8/cdot/hgvs/dataproviders/json_data_provider.py
-drwxrwxr-x   0 dlawrence  (1000) dlawrence  (1000)        0 2022-08-29 12:15:47.668525 cdot-0.2.8/cdot/pyhgvs/
--rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)        0 2022-06-27 00:48:45.000000 cdot-0.2.8/cdot/pyhgvs/__init__.py
--rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)     4990 2022-06-27 00:48:45.000000 cdot-0.2.8/cdot/pyhgvs/pyhgvs_transcript.py
-drwxrwxr-x   0 dlawrence  (1000) dlawrence  (1000)        0 2022-08-29 12:15:47.668525 cdot-0.2.8/cdot.egg-info/
--rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)     4670 2022-08-29 12:15:47.000000 cdot-0.2.8/cdot.egg-info/PKG-INFO
--rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)      570 2022-08-29 12:15:47.000000 cdot-0.2.8/cdot.egg-info/SOURCES.txt
--rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)        1 2022-08-29 12:15:47.000000 cdot-0.2.8/cdot.egg-info/dependency_links.txt
--rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)       31 2022-08-29 12:15:47.000000 cdot-0.2.8/cdot.egg-info/requires.txt
--rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)       11 2022-08-29 12:15:47.000000 cdot-0.2.8/cdot.egg-info/top_level.txt
--rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)      104 2022-06-27 00:48:45.000000 cdot-0.2.8/pyproject.toml
--rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)      664 2022-08-29 12:15:47.672525 cdot-0.2.8/setup.cfg
-drwxrwxr-x   0 dlawrence  (1000) dlawrence  (1000)        0 2022-08-29 12:15:47.672525 cdot-0.2.8/tests/
--rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)        0 2022-06-27 00:48:45.000000 cdot-0.2.8/tests/__init__.py
--rwxrwxr-x   0 dlawrence  (1000) dlawrence  (1000)     4447 2022-06-27 00:48:45.000000 cdot-0.2.8/tests/benchmark_hgvs.py
--rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)     6064 2022-06-27 00:48:45.000000 cdot-0.2.8/tests/genome.py
--rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)     3396 2022-08-29 06:28:05.000000 cdot-0.2.8/tests/test_gff_parsers.py
--rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)     2387 2022-08-29 03:49:17.000000 cdot-0.2.8/tests/test_json_data_provider.py
--rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)     1392 2022-06-27 00:48:45.000000 cdot-0.2.8/tests/test_pyhgvs.py
--rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)     1351 2022-06-27 01:49:52.000000 cdot-0.2.8/tests/test_uta_conversion.py
+drwxrwxr-x   0 dlawrence  (1000) dlawrence  (1000)        0 2022-09-01 02:28:17.781823 cdot-0.2.9/
+-rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)     1062 2022-08-18 05:05:00.000000 cdot-0.2.9/LICENSE
+-rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)     4670 2022-09-01 02:28:17.781823 cdot-0.2.9/PKG-INFO
+-rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)     4192 2022-08-29 23:55:11.000000 cdot-0.2.9/README.md
+drwxrwxr-x   0 dlawrence  (1000) dlawrence  (1000)        0 2022-09-01 02:28:17.777823 cdot-0.2.9/cdot/
+-rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)      242 2022-09-01 02:25:36.000000 cdot-0.2.9/cdot/__init__.py
+drwxrwxr-x   0 dlawrence  (1000) dlawrence  (1000)        0 2022-09-01 02:28:17.777823 cdot-0.2.9/cdot/gff/
+-rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)        0 2022-08-18 05:05:00.000000 cdot-0.2.9/cdot/gff/__init__.py
+-rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)    22227 2022-08-29 23:55:11.000000 cdot-0.2.9/cdot/gff/gff_parser.py
+drwxrwxr-x   0 dlawrence  (1000) dlawrence  (1000)        0 2022-09-01 02:28:17.777823 cdot-0.2.9/cdot/hgvs/
+-rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)        0 2022-08-18 05:05:00.000000 cdot-0.2.9/cdot/hgvs/__init__.py
+drwxrwxr-x   0 dlawrence  (1000) dlawrence  (1000)        0 2022-09-01 02:28:17.777823 cdot-0.2.9/cdot/hgvs/dataproviders/
+-rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)       34 2022-08-18 05:05:00.000000 cdot-0.2.9/cdot/hgvs/dataproviders/__init__.py
+-rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)    12899 2022-09-01 02:22:32.000000 cdot-0.2.9/cdot/hgvs/dataproviders/json_data_provider.py
+drwxrwxr-x   0 dlawrence  (1000) dlawrence  (1000)        0 2022-09-01 02:28:17.777823 cdot-0.2.9/cdot/pyhgvs/
+-rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)        0 2022-08-18 05:05:00.000000 cdot-0.2.9/cdot/pyhgvs/__init__.py
+-rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)     4990 2022-08-18 05:05:00.000000 cdot-0.2.9/cdot/pyhgvs/pyhgvs_transcript.py
+drwxrwxr-x   0 dlawrence  (1000) dlawrence  (1000)        0 2022-09-01 02:28:17.777823 cdot-0.2.9/cdot.egg-info/
+-rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)     4670 2022-09-01 02:28:17.000000 cdot-0.2.9/cdot.egg-info/PKG-INFO
+-rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)      570 2022-09-01 02:28:17.000000 cdot-0.2.9/cdot.egg-info/SOURCES.txt
+-rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)        1 2022-09-01 02:28:17.000000 cdot-0.2.9/cdot.egg-info/dependency_links.txt
+-rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)       31 2022-09-01 02:28:17.000000 cdot-0.2.9/cdot.egg-info/requires.txt
+-rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)       11 2022-09-01 02:28:17.000000 cdot-0.2.9/cdot.egg-info/top_level.txt
+-rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)      104 2022-08-18 05:05:00.000000 cdot-0.2.9/pyproject.toml
+-rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)      664 2022-09-01 02:28:17.781823 cdot-0.2.9/setup.cfg
+drwxrwxr-x   0 dlawrence  (1000) dlawrence  (1000)        0 2022-09-01 02:28:17.781823 cdot-0.2.9/tests/
+-rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)        0 2022-08-18 05:05:00.000000 cdot-0.2.9/tests/__init__.py
+-rwxrwxr-x   0 dlawrence  (1000) dlawrence  (1000)     4447 2022-08-18 05:05:00.000000 cdot-0.2.9/tests/benchmark_hgvs.py
+-rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)     6064 2022-08-18 05:05:00.000000 cdot-0.2.9/tests/genome.py
+-rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)     3396 2022-08-29 23:55:11.000000 cdot-0.2.9/tests/test_gff_parsers.py
+-rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)     2387 2022-08-29 23:55:11.000000 cdot-0.2.9/tests/test_json_data_provider.py
+-rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)     1392 2022-08-18 05:05:00.000000 cdot-0.2.9/tests/test_pyhgvs.py
+-rw-rw-r--   0 dlawrence  (1000) dlawrence  (1000)     1351 2022-08-18 05:05:00.000000 cdot-0.2.9/tests/test_uta_conversion.py
```

### Comparing `cdot-0.2.8/LICENSE` & `cdot-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cdot-0.2.8/PKG-INFO` & `cdot-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdot
-Version: 0.2.8
+Version: 0.2.9
 Summary: Transcripts for HGVS libraries
 Home-page: https://github.com/SACGF/cdot
 Author: Dave Lawrence
 Author-email: davmlaw@gmail.com
 Project-URL: Bug Tracker, https://github.com/SACGF/cdot/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cdot-0.2.8/README.md` & `cdot-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `cdot-0.2.8/cdot/gff/gff_parser.py` & `cdot-0.2.9/cdot/gff/gff_parser.py`

 * *Files identical despite different names*

### Comparing `cdot-0.2.8/cdot/hgvs/dataproviders/json_data_provider.py` & `cdot-0.2.9/cdot/hgvs/dataproviders/json_data_provider.py`

 * *Files 3% similar despite different names*

```diff
@@ -242,33 +242,48 @@
         for transcript_id in tx_by_gene[gene]:
             transcript_data = self._get_transcript(transcript_id)
             cds_start_i = transcript_data.get("start_codon")
             cds_end_i = transcript_data.get("stop_codon")
             for build_data in transcript_data["genome_builds"].values():
                 contig, tx_start, tx_end, _ = self._get_contig_start_end_strand(build_data)
                 length = tx_end - tx_start
-                tx_list.append((length, [gene, cds_start_i, cds_end_i, transcript_id, contig, self.NCBI_ALN_METHOD]))
+                tx_data = {
+                    "hgnc": gene,
+                    "cds_start_i": cds_start_i,
+                    "cds_end_i": cds_end_i,
+                    "tx_ac": transcript_id,
+                    "alt_ac": contig,
+                    "alt_aln_method": self.NCBI_ALN_METHOD,
+                }
+                tx_list.append((length, tx_data))
 
         return [x[1] for x in sorted(tx_list, key=lambda x: x[0], reverse=True)]
 
     def get_tx_for_region(self, alt_ac, alt_aln_method, start_i, end_i):
         """ return transcripts that overlap given region """
 
         tx_list = []
         if alt_aln_method == self.NCBI_ALN_METHOD:
             _, tx_intervals = self._tx_by_gene_and_intervals
-            for interval in tx_intervals[alt_ac][start_i:end_i]:
+            for interval in tx_intervals[alt_ac][start_i:end_i+1]:
                 transcript_id = interval.data
                 transcript_data = self._get_transcript(transcript_id)
                 build_data = self._get_transcript_coordinates_for_contig(transcript_data, alt_ac)
                 contig, tx_start, tx_end, strand = self._get_contig_start_end_strand(build_data)
                 if contig == alt_ac:
                     for exon in build_data["exons"]:
                         if exon[0] < start_i and end_i <= exon[1]:
-                            tx_list.append([transcript_id, alt_ac, strand, self.NCBI_ALN_METHOD, tx_start, tx_end])
+                            tx_list.append({
+                                "alt_ac": alt_ac,
+                                "alt_aln_method": self.NCBI_ALN_METHOD,
+                                "alt_strand": strand,
+                                "start_i": tx_start,
+                                "end_i": tx_end,
+                                "tx_ac": transcript_id,
+                            })
                             break
         return tx_list
 
     @lazy
     def _tx_by_gene_and_intervals(self):
         # The region query works on exons, but storing all of these makes the interval tree huge
         # So we just store the start/end of each transcript ID, then look up the exons at retrieval time
```

### Comparing `cdot-0.2.8/cdot/pyhgvs/pyhgvs_transcript.py` & `cdot-0.2.9/cdot/pyhgvs/pyhgvs_transcript.py`

 * *Files identical despite different names*

### Comparing `cdot-0.2.8/cdot.egg-info/PKG-INFO` & `cdot-0.2.9/cdot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdot
-Version: 0.2.8
+Version: 0.2.9
 Summary: Transcripts for HGVS libraries
 Home-page: https://github.com/SACGF/cdot
 Author: Dave Lawrence
 Author-email: davmlaw@gmail.com
 Project-URL: Bug Tracker, https://github.com/SACGF/cdot/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cdot-0.2.8/cdot.egg-info/SOURCES.txt` & `cdot-0.2.9/cdot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cdot-0.2.8/setup.cfg` & `cdot-0.2.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `cdot-0.2.8/tests/benchmark_hgvs.py` & `cdot-0.2.9/tests/benchmark_hgvs.py`

 * *Files identical despite different names*

### Comparing `cdot-0.2.8/tests/genome.py` & `cdot-0.2.9/tests/genome.py`

 * *Files identical despite different names*

### Comparing `cdot-0.2.8/tests/test_gff_parsers.py` & `cdot-0.2.9/tests/test_gff_parsers.py`

 * *Files identical despite different names*

### Comparing `cdot-0.2.8/tests/test_json_data_provider.py` & `cdot-0.2.9/tests/test_json_data_provider.py`

 * *Files identical despite different names*

### Comparing `cdot-0.2.8/tests/test_pyhgvs.py` & `cdot-0.2.9/tests/test_pyhgvs.py`

 * *Files identical despite different names*

### Comparing `cdot-0.2.8/tests/test_uta_conversion.py` & `cdot-0.2.9/tests/test_uta_conversion.py`

 * *Files identical despite different names*

