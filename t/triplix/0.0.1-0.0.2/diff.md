# Comparing `tmp/triplix-0.0.1.tar.gz` & `tmp/triplix-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "triplix-0.0.1.tar", last modified: Mon May  1 15:52:30 2023, max compression
+gzip compressed data, was "triplix-0.0.2.tar", last modified: Mon May  8 08:15:29 2023, max compression
```

## Comparing `triplix-0.0.1.tar` & `triplix-0.0.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 aallahyar   (501) staff       (20)        0 2023-05-01 15:52:30.291077 triplix-0.0.1/
--rw-r--r--   0 aallahyar   (501) staff       (20)     1070 2022-10-26 11:33:28.000000 triplix-0.0.1/LICENSE
--rw-r--r--   0 aallahyar   (501) staff       (20)        0 2023-05-01 15:40:08.000000 triplix-0.0.1/MANIFEST.in
--rw-r--r--   0 aallahyar   (501) staff       (20)    12641 2023-05-01 15:52:30.290376 triplix-0.0.1/PKG-INFO
--rw-r--r--   0 aallahyar   (501) staff       (20)    10843 2023-05-01 15:50:47.000000 triplix-0.0.1/README.md
--rw-r--r--   0 aallahyar   (501) staff       (20)     1168 2023-05-01 15:39:23.000000 triplix-0.0.1/pyproject.toml
--rw-r--r--   0 aallahyar   (501) staff       (20)       38 2023-05-01 15:52:30.291316 triplix-0.0.1/setup.cfg
-drwxr-xr-x   0 aallahyar   (501) staff       (20)        0 2023-05-01 15:52:30.271980 triplix-0.0.1/src/
-drwxr-xr-x   0 aallahyar   (501) staff       (20)        0 2023-05-01 15:52:30.275135 triplix-0.0.1/src/triplix/
--rw-r--r--   0 aallahyar   (501) staff       (20)      361 2023-03-06 18:25:02.000000 triplix-0.0.1/src/triplix/__init__.py
--rw-r--r--   0 aallahyar   (501) staff       (20)      544 2023-05-01 15:30:45.000000 triplix-0.0.1/src/triplix/__main__.py
-drwxr-xr-x   0 aallahyar   (501) staff       (20)        0 2023-05-01 15:52:30.284175 triplix-0.0.1/src/triplix/core/
--rw-r--r--   0 aallahyar   (501) staff       (20)        1 2022-11-09 14:48:24.000000 triplix-0.0.1/src/triplix/core/__init__.py
--rw-r--r--   0 aallahyar   (501) staff       (20)     3072 2022-11-22 08:46:02.000000 triplix-0.0.1/src/triplix/core/bam.py
--rw-r--r--   0 aallahyar   (501) staff       (20)    32224 2023-02-01 17:08:29.000000 triplix-0.0.1/src/triplix/core/cli.py
--rw-r--r--   0 aallahyar   (501) staff       (20)    11890 2023-04-20 14:43:53.000000 triplix-0.0.1/src/triplix/core/concatemers.py
--rw-r--r--   0 aallahyar   (501) staff       (20)      878 2022-11-25 15:03:15.000000 triplix-0.0.1/src/triplix/core/configurations.py
--rw-r--r--   0 aallahyar   (501) staff       (20)     5644 2023-04-20 13:47:58.000000 triplix-0.0.1/src/triplix/core/hdf5.py
--rw-r--r--   0 aallahyar   (501) staff       (20)    21450 2023-02-10 10:47:25.000000 triplix-0.0.1/src/triplix/core/header.py
--rw-r--r--   0 aallahyar   (501) staff       (20)    39408 2023-04-20 11:44:41.000000 triplix-0.0.1/src/triplix/core/plot.py
--rw-r--r--   0 aallahyar   (501) staff       (20)     5500 2023-03-06 18:25:02.000000 triplix-0.0.1/src/triplix/core/stat.py
-drwxr-xr-x   0 aallahyar   (501) staff       (20)        0 2023-05-01 15:52:30.286766 triplix-0.0.1/src/triplix/core/tri_alignment/
--rw-r--r--   0 aallahyar   (501) staff       (20)       64 2022-12-22 16:15:38.000000 triplix-0.0.1/src/triplix/core/tri_alignment/__init__.py
--rw-r--r--   0 aallahyar   (501) staff       (20)     6585 2023-04-20 12:38:23.000000 triplix-0.0.1/src/triplix/core/tri_alignment/extract.py
--rw-r--r--   0 aallahyar   (501) staff       (20)     1219 2023-01-26 14:50:24.000000 triplix-0.0.1/src/triplix/core/tri_alignment/index.py
--rw-r--r--   0 aallahyar   (501) staff       (20)    11269 2023-01-26 14:50:24.000000 triplix-0.0.1/src/triplix/core/tri_alignment/merge.py
--rw-r--r--   0 aallahyar   (501) staff       (20)     4359 2023-01-26 14:50:24.000000 triplix-0.0.1/src/triplix/core/tri_alignment/sort.py
--rw-r--r--   0 aallahyar   (501) staff       (20)    14163 2023-03-06 18:25:02.000000 triplix-0.0.1/src/triplix/core/tri_alignments.py
-drwxr-xr-x   0 aallahyar   (501) staff       (20)        0 2023-05-01 15:52:30.289545 triplix-0.0.1/src/triplix/core/triplet/
--rw-r--r--   0 aallahyar   (501) staff       (20)       71 2023-01-18 13:59:44.000000 triplix-0.0.1/src/triplix/core/triplet/__init__.py
--rw-r--r--   0 aallahyar   (501) staff       (20)     8654 2023-03-06 18:25:02.000000 triplix-0.0.1/src/triplix/core/triplet/bin.py
--rw-r--r--   0 aallahyar   (501) staff       (20)    11156 2023-02-09 07:02:41.000000 triplix-0.0.1/src/triplix/core/triplet/enrichment.py
--rw-r--r--   0 aallahyar   (501) staff       (20)     7169 2023-02-01 17:17:25.000000 triplix-0.0.1/src/triplix/core/triplet/kdtree.py
--rw-r--r--   0 aallahyar   (501) staff       (20)    13697 2023-03-06 18:25:02.000000 triplix-0.0.1/src/triplix/core/triplet/transform.py
--rw-r--r--   0 aallahyar   (501) staff       (20)    33787 2023-04-20 11:44:41.000000 triplix-0.0.1/src/triplix/core/triplets.py
--rw-r--r--   0 aallahyar   (501) staff       (20)     7116 2023-01-26 14:50:24.000000 triplix-0.0.1/src/triplix/core/utilities.py
-drwxr-xr-x   0 aallahyar   (501) staff       (20)        0 2023-05-01 15:52:30.277959 triplix-0.0.1/src/triplix.egg-info/
--rw-r--r--   0 aallahyar   (501) staff       (20)    12641 2023-05-01 15:52:30.000000 triplix-0.0.1/src/triplix.egg-info/PKG-INFO
--rw-r--r--   0 aallahyar   (501) staff       (20)     1029 2023-05-01 15:52:30.000000 triplix-0.0.1/src/triplix.egg-info/SOURCES.txt
--rw-r--r--   0 aallahyar   (501) staff       (20)        1 2023-05-01 15:52:30.000000 triplix-0.0.1/src/triplix.egg-info/dependency_links.txt
--rw-r--r--   0 aallahyar   (501) staff       (20)       50 2023-05-01 15:52:30.000000 triplix-0.0.1/src/triplix.egg-info/entry_points.txt
--rw-r--r--   0 aallahyar   (501) staff       (20)      200 2023-05-01 15:52:30.000000 triplix-0.0.1/src/triplix.egg-info/requires.txt
--rw-r--r--   0 aallahyar   (501) staff       (20)        8 2023-05-01 15:52:30.000000 triplix-0.0.1/src/triplix.egg-info/top_level.txt
+drwxr-xr-x   0 aallahyar   (501) staff       (20)        0 2023-05-08 08:15:29.139098 triplix-0.0.2/
+-rw-r--r--   0 aallahyar   (501) staff       (20)     1070 2022-10-26 11:33:28.000000 triplix-0.0.2/LICENSE
+-rw-r--r--   0 aallahyar   (501) staff       (20)        0 2023-05-01 15:40:08.000000 triplix-0.0.2/MANIFEST.in
+-rw-r--r--   0 aallahyar   (501) staff       (20)    13118 2023-05-08 08:15:29.138465 triplix-0.0.2/PKG-INFO
+-rw-r--r--   0 aallahyar   (501) staff       (20)    11303 2023-05-08 08:01:12.000000 triplix-0.0.2/README.md
+-rw-r--r--   0 aallahyar   (501) staff       (20)     1185 2023-05-08 08:05:35.000000 triplix-0.0.2/pyproject.toml
+-rw-r--r--   0 aallahyar   (501) staff       (20)       38 2023-05-08 08:15:29.139280 triplix-0.0.2/setup.cfg
+drwxr-xr-x   0 aallahyar   (501) staff       (20)        0 2023-05-08 08:15:29.098437 triplix-0.0.2/src/
+drwxr-xr-x   0 aallahyar   (501) staff       (20)        0 2023-05-08 08:15:29.101804 triplix-0.0.2/src/triplix/
+-rw-r--r--   0 aallahyar   (501) staff       (20)      361 2023-03-06 18:25:02.000000 triplix-0.0.2/src/triplix/__init__.py
+-rw-r--r--   0 aallahyar   (501) staff       (20)      544 2023-05-01 15:30:45.000000 triplix-0.0.2/src/triplix/__main__.py
+drwxr-xr-x   0 aallahyar   (501) staff       (20)        0 2023-05-08 08:15:29.124569 triplix-0.0.2/src/triplix/core/
+-rw-r--r--   0 aallahyar   (501) staff       (20)        1 2022-11-09 14:48:24.000000 triplix-0.0.2/src/triplix/core/__init__.py
+-rw-r--r--   0 aallahyar   (501) staff       (20)     3072 2022-11-22 08:46:02.000000 triplix-0.0.2/src/triplix/core/bam.py
+-rw-r--r--   0 aallahyar   (501) staff       (20)    32620 2023-05-08 08:01:12.000000 triplix-0.0.2/src/triplix/core/cli.py
+-rw-r--r--   0 aallahyar   (501) staff       (20)    11890 2023-04-20 14:43:53.000000 triplix-0.0.2/src/triplix/core/concatemers.py
+-rw-r--r--   0 aallahyar   (501) staff       (20)      878 2022-11-25 15:03:15.000000 triplix-0.0.2/src/triplix/core/configurations.py
+-rw-r--r--   0 aallahyar   (501) staff       (20)     5644 2023-04-20 13:47:58.000000 triplix-0.0.2/src/triplix/core/hdf5.py
+-rw-r--r--   0 aallahyar   (501) staff       (20)    21475 2023-05-08 08:01:12.000000 triplix-0.0.2/src/triplix/core/header.py
+-rw-r--r--   0 aallahyar   (501) staff       (20)    39438 2023-05-08 08:01:12.000000 triplix-0.0.2/src/triplix/core/plot.py
+-rw-r--r--   0 aallahyar   (501) staff       (20)     5500 2023-03-06 18:25:02.000000 triplix-0.0.2/src/triplix/core/stat.py
+drwxr-xr-x   0 aallahyar   (501) staff       (20)        0 2023-05-08 08:15:29.130274 triplix-0.0.2/src/triplix/core/tri_alignment/
+-rw-r--r--   0 aallahyar   (501) staff       (20)       64 2022-12-22 16:15:38.000000 triplix-0.0.2/src/triplix/core/tri_alignment/__init__.py
+-rw-r--r--   0 aallahyar   (501) staff       (20)     6645 2023-05-08 08:01:12.000000 triplix-0.0.2/src/triplix/core/tri_alignment/extract.py
+-rw-r--r--   0 aallahyar   (501) staff       (20)     1219 2023-01-26 14:50:24.000000 triplix-0.0.2/src/triplix/core/tri_alignment/index.py
+-rw-r--r--   0 aallahyar   (501) staff       (20)    11270 2023-05-08 08:01:12.000000 triplix-0.0.2/src/triplix/core/tri_alignment/merge.py
+-rw-r--r--   0 aallahyar   (501) staff       (20)     4377 2023-05-08 08:01:12.000000 triplix-0.0.2/src/triplix/core/tri_alignment/sort.py
+-rw-r--r--   0 aallahyar   (501) staff       (20)    14163 2023-05-08 08:01:12.000000 triplix-0.0.2/src/triplix/core/tri_alignments.py
+drwxr-xr-x   0 aallahyar   (501) staff       (20)        0 2023-05-08 08:15:29.137151 triplix-0.0.2/src/triplix/core/triplet/
+-rw-r--r--   0 aallahyar   (501) staff       (20)       71 2023-01-18 13:59:44.000000 triplix-0.0.2/src/triplix/core/triplet/__init__.py
+-rw-r--r--   0 aallahyar   (501) staff       (20)     8614 2023-05-08 08:01:12.000000 triplix-0.0.2/src/triplix/core/triplet/bin.py
+-rw-r--r--   0 aallahyar   (501) staff       (20)    11156 2023-02-09 07:02:41.000000 triplix-0.0.2/src/triplix/core/triplet/enrichment.py
+-rw-r--r--   0 aallahyar   (501) staff       (20)     7169 2023-02-01 17:17:25.000000 triplix-0.0.2/src/triplix/core/triplet/kdtree.py
+-rw-r--r--   0 aallahyar   (501) staff       (20)    13694 2023-05-08 08:01:12.000000 triplix-0.0.2/src/triplix/core/triplet/transform.py
+-rw-r--r--   0 aallahyar   (501) staff       (20)    33787 2023-04-20 11:44:41.000000 triplix-0.0.2/src/triplix/core/triplets.py
+-rw-r--r--   0 aallahyar   (501) staff       (20)     7116 2023-01-26 14:50:24.000000 triplix-0.0.2/src/triplix/core/utilities.py
+drwxr-xr-x   0 aallahyar   (501) staff       (20)        0 2023-05-08 08:15:29.105440 triplix-0.0.2/src/triplix.egg-info/
+-rw-r--r--   0 aallahyar   (501) staff       (20)    13118 2023-05-08 08:15:29.000000 triplix-0.0.2/src/triplix.egg-info/PKG-INFO
+-rw-r--r--   0 aallahyar   (501) staff       (20)     1029 2023-05-08 08:15:29.000000 triplix-0.0.2/src/triplix.egg-info/SOURCES.txt
+-rw-r--r--   0 aallahyar   (501) staff       (20)        1 2023-05-08 08:15:29.000000 triplix-0.0.2/src/triplix.egg-info/dependency_links.txt
+-rw-r--r--   0 aallahyar   (501) staff       (20)       50 2023-05-08 08:15:29.000000 triplix-0.0.2/src/triplix.egg-info/entry_points.txt
+-rw-r--r--   0 aallahyar   (501) staff       (20)      200 2023-05-08 08:15:29.000000 triplix-0.0.2/src/triplix.egg-info/requires.txt
+-rw-r--r--   0 aallahyar   (501) staff       (20)        8 2023-05-08 08:15:29.000000 triplix-0.0.2/src/triplix.egg-info/top_level.txt
```

### Comparing `triplix-0.0.1/LICENSE` & `triplix-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `triplix-0.0.1/PKG-INFO` & `triplix-0.0.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,61 +1,39 @@
-Metadata-Version: 2.1
-Name: triplix
-Version: 0.0.1
-Summary: A python package to efficiently process, store and retrieve multi-contact data
-Author-email: Amin Allahyar <amin.allahyar@gmail.com>
-License: MIT License
-        
-        Copyright (c) 2022 Amin Allahyar
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-Project-URL: Homepage, https://github.com/deLaatLab/triplix
-Keywords: Bioinformatics,Genome,3D Genome Conformation,Multi-contact
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Triplix
+[![PyPI version](https://badge.fury.io/py/triplix.svg)](https://badge.fury.io/py/triplix)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/triplix.svg)
+[![MIT](https://img.shields.io/pypi/l/triplix.svg?color=green)](https://opensource.org/licenses/MIT)
+
+A python package to efficiently process, store and retrieve spatial genomics multi-contact data.
 
 ## Introduction:
 Triplix provides access to multi-contact data, that could be stored in three different spaces (i.e., resolution): 
 1. **Concatemers**: An HDF5 container that stores multi-contact data in a table-like format. 
 Each row in this table is an alignment that is captured by a particular `concatemer` (i.e., a sequenced long `read`). 
 There is an index (i.e., `read_idx`) column in this table that specifies alignments that originate from each specific `concatemer`.
 
-2. **Tri-Alignments**:
-Every possible three cis-alignments of each `concatemer` is stored in the Tri-Alignment file. Each three cis-alignment is called a `tri-alignment`. 
+2. **Tri-alignments**:
+Every possible three cis-alignments of each `concatemer` is stored in the Tri-alignment file. Each three cis-alignment is called a `tri-alignment`. 
 Such a data structure facilitates 3-way interaction analyses, and allow random-access. 
 To this end, `Triplix` has a simple wrapper around [pairix](https://github.com/4dn-dcic/pairix).
 In particular, the relevant `tri-alignments` are loaded by checking the first two given coordinates using `pairix`, and then filtering for the third coordinate via an ordinary overlap check.
 
 3. **Triplets**:
-Triples are essentially Tri-Alignment files, where `tri-alignments` are aggregated into genomic bins. 
+Triples are essentially Tri-alignment files, where `tri-alignments` are aggregated into genomic bins. 
 This not only reduces the disk (and memory) footprint, but also facilitates random-access. Considering the sparcity of the multi-contact data, most (if not all) multi-contact analyses are done in this "binned" space (rather than `alignment` space).
 
+## Installation
+You may run the following commands in your command line to install Triplix.
+```bash
+pip3 install triplix
+
+# or
+python3 -m pip install triplix
+```
+
 ## Usage:
 Below, you can see how you can extract data in each space.
 
 #### 1. Concatemer space  (*.concatemers.h5)
 Provides random-access to read (i.e., `concatemer`) level data. 
 
 First, we open `concatemers` container via:
@@ -124,26 +102,26 @@
 #    chrom_num     start  strand                             read_name
 # 0          5  92933191      -1  0000eea6-4554-40c3-b4ab-ecaa5cf5795b
 # 1          5  23899224       1  0000eea6-4554-40c3-b4ab-ecaa5cf5795b
 # 2          5  33962641      -1  0000eea6-4554-40c3-b4ab-ecaa5cf5795b
 # 
 ```
 
-#### 2. Tri-Alignment space (*.3ln):
-Provides access to alignment (i.e., `tri-alignment`) level data. 
+#### 2. Tri-alignment space (*.tri-alignments.tsv.bgz):
+Provides access to alignment (i.e., `tri-alignments`) level data. 
 These files are essentially formatted as compressed [pairix files](https://github.com/4dn-dcic/pairix). The difference is that they contain three coordinates instead of two coordinates (as is the case for regular pairix files)
 
-> **Note:** The tri-alignment files need to be indexed if you like to have random access to them. You can do this using `triplix index --input=input-file.3aln`
+> **Note:** The tri-alignment files need to be indexed if you like to have random access to them. You can do this using `triplix index --input=input-file.tri-alignments.tsv.bgz`
 
 An example of this usage is as follows:
 
 ```python
 import triplix
 
-tri_aln_path = './tri-alignments/GM12878.Merged.3aln'
+tri_aln_path = './tri-alignments/GM12878.Merged.tri-alignments.tsv.bgz'
 tri_container = triplix.TriAlignmentsContainer(trialn_path=tri_aln_path)
 
 tri_alignments_iter = tri_container.fetch(chrom_a='chrY', start_a=0e6, end_a=10e6, batch_size=10)
 for idx, tri_alignments in enumerate(tri_alignments_iter):
     df = tri_alignments.to_dataframe()
     print(df[['read_name', 'chrom_A', 'start_A', 'start_B', 'start_C']])
     if idx > 0:
@@ -168,22 +146,22 @@
 # 6  0f526116-e8fc-459b-aac9-d9d6d2843289    chrY    13584   278514   366665
 # 7  6589f1d9-cd7d-4cba-bfc9-06f123956157    chrY    13584   282655   440783
 # 8  0f526116-e8fc-459b-aac9-d9d6d2843289    chrY    13584   364567   366665
 # 9  11f46754-fbfe-4f9f-8aa6-7f03c7db48df    chrY    13584  1180971  1812799
 
 ```
 
-#### 3. Triplet space (*.trpl):
+#### 3. Triplet space (*.triplets.h5):
 Provides access to triplet-level data. A usage example is:
 
 ```python
 import pandas as pd
 import triplix
 
-trpl_path = './triplets/GM12878.MC-HiC.hg38.trpl'
+trpl_path = './triplets/GM12878.MC-HiC.hg38.triplets.h5'
 trpl_obj = triplix.TripletsContainer(container_path=trpl_path)
 triplets_input = trpl_obj.fetch(
     chrom_a='chr8', start_a=119e6, end_a=120e6,
     columns=['start_A', 'start_B', 'start_C', 'count_ABC'],
 )
 df = pd.DataFrame(triplets_input)
 print(df)
@@ -200,15 +178,7 @@
 # 136158  120000000  121975000  121975000          5
 # 136159  120000000  121975000  122000000          7
 # 136160  120000000  122000000  122000000          6
 # 
 # [136161 rows x 4 columns]
 ```
 
-## Installation
-Simply run the following command to install Triplix.
-```bash
-pip3 install triplix
-
-# or
-python3 -m pip install triplix
-```
```

### Comparing `triplix-0.0.1/pyproject.toml` & `triplix-0.0.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -4,16 +4,16 @@
     'wheel'
 ]
 build-backend = 'setuptools.build_meta'
 
 
 [project]
 name = 'triplix'
-version = '0.0.1'
-description = 'A python package to efficiently process, store and retrieve multi-contact data'
+version = '0.0.2'
+description = 'A python package to efficiently process, store and retrieve spatial genomics multi-contact data'
 readme = 'README.md'
 authors = [{ name = 'Amin Allahyar', email = 'amin.allahyar@gmail.com' }]
 license = { file = 'LICENSE' }
 classifiers = [
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python',
     'Programming Language :: Python :: 3',
```

### Comparing `triplix-0.0.1/src/triplix/__main__.py` & `triplix-0.0.2/src/triplix/__main__.py`

 * *Files identical despite different names*

### Comparing `triplix-0.0.1/src/triplix/core/bam.py` & `triplix-0.0.2/src/triplix/core/bam.py`

 * *Files identical despite different names*

### Comparing `triplix-0.0.1/src/triplix/core/cli.py` & `triplix-0.0.2/src/triplix/core/cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,30 +11,30 @@
 from triplix.core import configurations
 from triplix.core import stat
 from triplix.core import plot
 
 logger = logging.getLogger(__name__)
 
 
-def cli_concatemer(cli_args):
+def cli_concatemers(cli_args):
     exporter = concatemers.ExporterHDF5(
         bam_path=cli_args.input,
         assembly=cli_args.assembly,
         output_dir=cli_args.output_dir,
         output_name=cli_args.output_name,
         assume_sorted=cli_args.assume_sorted,
         cell_type=cli_args.cell_type,
         assay_name=cli_args.assay_name,
         experiment_name=cli_args.experiment_name,
     )
     exporter.initialize_hdf5()
     exporter.store_concatemers()
 
 
-def cli_tri_alignment(cli_args):
+def cli_tri_alignments(cli_args):
     extractor = tri_alignment.extract.TriAlignmentExtractor(
         concatemers_path=cli_args.input,
         output_dir=cli_args.output_dir,
         output_name=cli_args.output_name,
     )
     extractor.extract_tri_alignments()
 
@@ -270,127 +270,127 @@
     )
     parser_main.add_argument('-h', '--help', action='help', default=argparse.SUPPRESS, help='Show this help message and exit.')
     parser_main.add_argument('--debug', action='store_true', help='Activate the debug mode.')
     parser_main.add_argument('--log_level', type=int, default=logging.INFO, help='Log level. An integer in [0, 50] interval. With larger values Triplix will be more conservative in printing messages (default: %(default)s)')
 
     #########################################
     # forming concatemers
-    parser_concatemer = commands.add_parser('concatemer', help='Parse input BAM file and extract concatemer')
-    optional = parser_concatemer._action_groups.pop()
-    required = parser_concatemer.add_argument_group('required arguments')
+    parser_concatemers = commands.add_parser('concatemers', help='Parse input BAM file and extract Concatemers')
+    optional = parser_concatemers._action_groups.pop()
+    required = parser_concatemers.add_argument_group('required arguments')
     required.add_argument('--input', required=True, metavar='<PATH>', help='Path to the input BAM file. The BAM file should be sorted by `read name` (i.e., using `samtools sort -n`)')
     optional.add_argument('--assembly', default='unknown', metavar='<STRING>', help='Name of the assembly (or genome) such as `hg19`, `hg38`, `mm10`, etc. (default: %(default)s)')
     optional.add_argument('--output_dir', default='./concatemers/', metavar='<PATH>',
-                          help='Output directory where the output concatemer file (.concatemers.h5) will be stored (default: %(default)s)')
+                          help='Output directory where the output Concatemers file (.concatemers.h5) will be stored (default: %(default)s)')
     optional.add_argument('--output_name', default=None, metavar='<FILENAME>',
-                          help='Output concatemer file name. If not provided, the `experiment_name` is used with an added `.concatemers.h5` extension')
+                          help='Output Concatemers file name. If not provided, the `experiment_name` is used with an added `.concatemers.h5` extension')
     optional.add_argument('--assume_sorted', action='store_true', help='Disables the name-sort check and assumes that the input BAM file is name sorted (default: %(default)s)')
     optional.add_argument('--cell_type', default='unknown', metavar='<STRING>', help='Name of the cell-type that is used to produce the current experiment (default: %(default)s)')
     optional.add_argument('--assay_name', default='unknown', metavar='<STRING>', help='Name of the assay that is used to produce the current experiment (default: %(default)s)')
     optional.add_argument('--experiment_name', default=None, metavar='<STRING>', help='A name for the current experiment. If not provided, the input BAM filename will be used as the `--experiment_name` instead.')
-    parser_concatemer._action_groups.append(optional)
-    parser_concatemer.set_defaults(func=cli_concatemer)
+    parser_concatemers._action_groups.append(optional)
+    parser_concatemers.set_defaults(func=cli_concatemers)
 
     #########################################
     # extracting tri-alignments
-    parser_triplet = commands.add_parser('tri_alignment', help='Process a concatemer file (.concatemers.h5) and extract tri-alignments from it')
-    parser_triplet.add_argument('--input', required=True, metavar='<PATH>', help='Path to input concatemer file (e.g. `*.concatemers.h5`)')
-    parser_triplet.add_argument('--output_dir', default='./tri-alignments/', metavar='<PATH>',
-                                help='Output directory where the extracted triplet will be stored (default: %(default)s)')
-    parser_triplet.add_argument('--output_name', default=None, metavar='<FILENAME>',
-                                help='Output file name for the extracted triplet. If not provided, the output is stored using the input triplet file name, with a `.trp` extension')
-    parser_triplet.set_defaults(func=cli_tri_alignment)
+    parser_tri_alignments = commands.add_parser('tri_alignments', help='Process a Concatemers file (.concatemers.h5) and extract Tri-alignments from it')
+    parser_tri_alignments.add_argument('--input', required=True, metavar='<PATH>', help='Path to input Concatemers file (e.g. `*.concatemers.h5`)')
+    parser_tri_alignments.add_argument('--output_dir', default='./tri-alignments/', metavar='<PATH>',
+                                       help='Output directory where the extracted Tri-alignments will be stored (default: %(default)s)')
+    parser_tri_alignments.add_argument('--output_name', default=None, metavar='<FILENAME>',
+                                       help='Output file name for the extracted Tri-alignments. If not provided, the output is stored using the input Concatemers file name, with a `.tri-alignments.tsv.bgz` extension')
+    parser_tri_alignments.set_defaults(func=cli_tri_alignments)
 
     #########################################
-    # sorting triplet
-    parser_sort = commands.add_parser('sort', help='Sort a tri-alignment file according to the chromosomal positions of its tri-alignments anchors.')
-    parser_sort.add_argument('--input', required=True, metavar='<PATH>', help='Path to tri-alignment file (e.g. `*.trp`)')
+    # sorting tri-alignments
+    parser_sort = commands.add_parser('sort', help='Sort a Tri-alignments file according to the chromosomal positions of its Tri-alignments anchors.')
+    parser_sort.add_argument('--input', required=True, metavar='<PATH>', help='Path to Tri-alignments file (e.g. `*.tri-alignments.tsv.bgz`)')
     parser_sort.add_argument('--output_dir', default='./tri-alignments_sorted', metavar='<PATH>',
-                             help='Output directory where the sorted tri-alignment will be stored (default: %(default)s)')
+                             help='Output directory where the sorted Tri-alignments file will be stored (default: %(default)s)')
     parser_sort.add_argument('--output_name', default=None, metavar='<FILENAME>',
-                             help='Output file name for the sorted tri-alignments. If not provided, the output is stored using the input tri-alignment filename, with a `.sorted.trp` extension')
+                             help='Output name for the sorted Tri-alignments file. If not provided, the output is stored using the input Tri-alignments filename, with a `.sorted.tri-alignments.tsv.bgz` extension')
     parser_sort.add_argument('--memory', default='2G', metavar='<FLOAT>G', help='Amount of memory (in Gigabyte, or another supported size unit) that can be used by `sort` program (default: "%(default)s")')
     parser_sort.add_argument('--threads', default=1, type=int, metavar='<INTEGER>', help='Number of threads that can be used by `sort` program (default: "%(default)s")')
     parser_sort.set_defaults(func=cli_sort)
 
     #########################################
-    # merging triplet
-    parser_merge = commands.add_parser('merge', help='Merge a series of tri-alignment files')
-    parser_merge.add_argument('--input', required=True, metavar='<PATH>[,<PATH>]', help='A comma-separated list of paths to tri-alignment files (e.g. `*.trp`). Each PATH can be a pattern that contain `*` to match several files.')
+    # merging tri-alignments
+    parser_merge = commands.add_parser('merge', help='Merge a series of Tri-alignments files')
+    parser_merge.add_argument('--input', required=True, metavar='<PATH>[,<PATH>]', help='A comma-separated list of paths to Tri-alignments files (e.g. `*.tri-alignments.tsv.bgz`). Each PATH can be a pattern that contain `*` to match several files.')
     parser_merge.add_argument('--output_dir', default='./tri-alignments_merged/', metavar='<PATH>',
                               help='Output directory where the merged triplet will be stored (default: %(default)s)')
     parser_merge.add_argument('--output_name', default=None, metavar='<FILENAME>',
-                              help='Output file name for the merged triplet. If not provided, the output is stored using the first input tri-alignment filename, with a `.merged.trp` extension')
+                              help='Output file name for the merged Tri-alignments. If not provided, the output is stored using the first input Tri-alignments filename, with a `.merged.tri-alignments.tsv.bgz` extension')
     parser_merge.add_argument('--memory', default='2G', help='Amount of memory (in Gigabyte unit) that can be used by `merge` program (default: "%(default)s")')
     parser_merge.add_argument('--threads', default=4, type=int, metavar='<INTEGER>', help='Number of threads that can be used by `sort` program (default: "%(default)s")')
-    parser_merge.add_argument('--concatenate', action="store_true", help='Perform a simple concatenation of tri-alignment files instead of merging files in a sorted manner')
+    parser_merge.add_argument('--concatenate', action="store_true", help='Perform a simple concatenation of Tri-alignments files instead of merging files in a sorted manner')
     parser_merge.add_argument('--check_coverage', action="store_true", help='Checks whether merging chunks are overlapping, or if a chromosomal region is not covered by any chunk')
     parser_merge.add_argument('--sort_by', choices=['none', 'chrom'], default='chrom',
                               help='Sort the input files before merge/concatenation. `none` ignores sorting. `chrom` sorts files by the order of chromosomes in the original BAM file (default: "%(default)s")')
     # todo: add possibility to update the header/meta-data of the merged dataset, e.g. experiment_name
     # todo: implement a better header merger. Then remove this flag
     parser_merge.add_argument('--ignore_samheaders', action="store_true", help='Ignores merging sam headers.')
-    parser_merge.add_argument('--metadata', default=None, metavar='<STRING>:<STRING>,[...]', help='A comma-separated list of key:values to be stored as the container\'s attributes such as experiment or assay name')
+    parser_merge.add_argument('--metadata', default=None, metavar='<STRING>:<STRING>,[...]', help='A comma-separated list of key:values to be stored in the Tri-alignments file header such as experiment or assay name')
     parser_merge.set_defaults(func=cli_merge)
 
     #########################################
-    # indexing triplet
+    # indexing tri-alignments
     parser_index = commands.add_parser('index', help='Index a tri-alignment file')
-    parser_index.add_argument('--input', required=True, metavar='<PATH>', help='Path to tri-alignment file (e.g. `*.trp`). The index will be stored besides the input tri-alignment file.')
+    parser_index.add_argument('--input', required=True, metavar='<PATH>', help='Path to a Tri-alignments file (e.g. `*.tri-alignments.tsv.bgz`). The index will be stored besides the input Tri-alignments file')
     parser_index.set_defaults(func=cli_index)
 
     #########################################
-    # partition triplets into bins
-    parser_bin = commands.add_parser('bin', help='Discretize the genome into equally-spaced anchors (i.e., bins) and represent the interactions in terms of triplets.')
-    parser_bin.add_argument('--input', required=True, metavar='<PATH>', help='Path to input tri-alignment file (e.g. `*.trp`).')
+    # mapping tri-alignments into bins
+    parser_bin = commands.add_parser('bin', help='Discretize the genome into equally-spaced anchors (i.e., bins) and represent the interactions in terms of Triplets')
+    parser_bin.add_argument('--input', required=True, metavar='<PATH>', help='Path to input Tri-alignments file (e.g. `*.tri-alignments.tsv.bgz`).')
     parser_bin.add_argument('--output_dir', default='./triplets/', metavar='<PATH>',
-                            help='Output directory where the triplet file will be stored (default: %(default)s)')
+                            help='Output directory where the Triplets file will be stored (default: %(default)s)')
     parser_bin.add_argument('--output_name', default=None, metavar='<FILENAME>',
-                            help='Output file name for the triplets. If not provided, the output is stored using the input tri-alignment filename, with a `.trpl` extension.')
+                            help='Output name for the Triplets file. If not provided, the output is stored using the input Tri-alignments file name, with a `.triplets.h5` extension')
     parser_bin.add_argument('--chunk_chrom', required=True, metavar='<STRING>', help='Name of the chromosome from which triplet are formed')
     parser_bin.add_argument('--chunk_start', required=True, type=float, metavar='<INTEGER>', help='Start position of the chunk from which triplets are formed')
     parser_bin.add_argument('--chunk_end', required=True, type=float, metavar='<INTEGER>', help='End position of the chunk from which triplets are formed')
     parser_bin.add_argument('--anchor_width', default=int(25e3), type=float, metavar='<INTEGER>', help='Width of each anchor (i.e., genomic bin) (default: "%(default)s")')
     parser_bin.add_argument('--anchor_max_distance', default=int(2e6), type=float, metavar='<INTEGER>', help='Maximum distance between anchors of a triplet (default: "%(default)s")')
     parser_bin.add_argument('--mapping_quality', default=5, type=int, metavar='<INTEGER>', help='Minimum mapping quality threshold to consider an alignment to be valid (default: "%(default)s")')
     parser_bin.set_defaults(func=cli_bin)
 
     #########################################
     # transform triplet counts
     parser_transform = commands.add_parser('transform', help='Transform the raw counts using the requested transformation.')
-    parser_transform.add_argument('--input', required=True, metavar='<PATH>', help='Path to triplet file (e.g. `*.trpl`). This file needs to be indexed.')
+    parser_transform.add_argument('--input', required=True, metavar='<PATH>', help='Path to Triplets file (e.g. `*.triplets.h5`). This file needs to be indexed.')
     parser_transform.add_argument('--transform_name', choices=['Gaussian'], default='Gaussian', help='Transformation name')
     parser_transform.add_argument('--transform_params', default='{"kernel_width":15,"kernel_scale":1.0}', help='JSON-formatted parameters of the transformation (default: "%(default)s")')
     parser_transform.add_argument('--transform_label', default='observed', metavar='<STRING>', help='Each transformed column will be labeled using this parameter (default: "%(default)s")')
     parser_transform.add_argument('--chunk_chrom', required=True, metavar='<STRING>', help='Name of the chromosome from which triplets are collected')
     parser_transform.add_argument('--chunk_start', required=True, type=float, metavar='<INTEGER>', help='Start position of the chunk from which triplets are collected')
     parser_transform.add_argument('--chunk_end', required=True, type=float, metavar='<INTEGER>', help='End position of the chunk from which triplets are collected')
     parser_transform.add_argument('--min_distance', default=int(25e3), type=float, metavar='<INTEGER>', help='Minimum distance between anchors of a triplet (default: "%(default)s")')
     parser_transform.add_argument('--max_distance', default=int(2e6), type=float, metavar='<INTEGER>', help='Maximum distance between anchors of a triplet (default: "%(default)s")')
     parser_transform.set_defaults(func=cli_transform)
 
     #########################################
     # finding neighbors
-    parser_findnei = commands.add_parser('kdtree', help='Construct a KDTree structure to efficiently find triplet neighbors.')
-    parser_findnei.add_argument('--input', required=True, metavar='<PATH>', help='Path to Triplet file (e.g. `*.trpl`).')
+    parser_findnei = commands.add_parser('kdtree', help='Construct a KDTree structure to efficiently find Triplet neighbors.')
+    parser_findnei.add_argument('--input', required=True, metavar='<PATH>', help='Path to Triplets file (e.g. `*.triplets.h5`).')
     parser_findnei.add_argument('--output_dir', default='./kdtrees/', metavar='<PATH>',
                                 help='Output directory where the KDTree will be stored (default: %(default)s)')
     parser_findnei.add_argument('--output_name', default=None, metavar='<FILENAME>',
-                                help='Output file name for the KDTree. If not provided, the output is stored using the input Triplet filename, with a `.kdtree.joblib` extension.')
+                                help='Output file name for the KDTree. If not provided, the output is stored using the input Triplets filename, with a `.kdtree.joblib` extension.')
     parser_findnei.add_argument('--chroms', metavar='STRING[,STRING]', default=None, help='A comma-separated list of chromosome names to be used in KDTree construction. If not provided, all chromosomes will be used.')
     parser_findnei.add_argument('--factors', required=True, metavar='<PATH>|<COL>:<FUNC>[,<COL>:<FUNC>]', help='Path to correction factor definitions, or a comma-separated list of <column_name>:<normalization>')
     parser_findnei.add_argument('--target', required=True, default='observed_ABC', metavar='<STRING>', help='Name of the column to be used as "target", in the background model  (default: "%(default)s")')
     parser_findnei.add_argument('--n_samples', default=np.inf, type=float, help='Sets the maximum number of samples to be included in the KDTree (default: "%(default)s")')
     parser_findnei.set_defaults(func=cli_kdtree)
 
     #########################################
     # estimate enrichments
     parser_enrich = commands.add_parser('enrichment', help='Estimate the enrichments of (a chunk of) triplet.')
-    parser_enrich.add_argument('--input', required=True, metavar='<PATH>', help='Path to triplet file (e.g. `*.trpl`).')
-    parser_enrich.add_argument('--kdtree', required=True, metavar='<PATH>', help='Path to KDTree, constructed from the input triplet file.')
+    parser_enrich.add_argument('--input', required=True, metavar='<PATH>', help='Path to Triplets file (e.g. `*.triplets.h5`).')
+    parser_enrich.add_argument('--kdtree', required=True, metavar='<PATH>', help='Path to KDTree, constructed from the input Triplets file.')
     parser_enrich.add_argument('--chunk_chrom', required=True, metavar='<STRING>', help='Name of the chromosome from which the triplets are going to be collected')
     parser_enrich.add_argument('--chunk_start', required=True, type=float, metavar='<INTEGER>', help='Start position of the chunk from which the triplets are going to be collected')
     parser_enrich.add_argument('--chunk_end', required=True, type=float, metavar='<INTEGER>', help='End position of the chunk from which the triplets are going to be collected')
     parser_enrich.add_argument('--view_point', default=None, type=float, metavar='<INTEGER>', help='If given, only triplets that overlap with the viewpoint are considered')
     parser_enrich.add_argument('--n_neighbors', default=int(10e3), type=int, metavar='<INTEGER>', help='Number of neighbors to use during enrichment estimation (default: "%(default)s")')
     parser_enrich.set_defaults(func=cli_enrichment)
 
@@ -401,15 +401,17 @@
         title='available plots are',
         dest='type',
     )
 
     # plotting virtual-hic
     parser_virthic = command_plot.add_parser('virtual_hic', help='Generate a virtual HiC plot, depicting the requested columns (using `--columns`).')
     parser_virthic.add_argument('--input', required=True, metavar='<PATH>',
-                                help='Path to input file. Multiple paths could be provided using comma-separated format. Wild chars (i.e., "*") are also supported. The input file could be a BAM, tri-alignment, or triplets file. In case of BAM or tri-alignment, the file  needs to be indexed.')
+                                help='Path to input file. Multiple paths could be provided using comma-separated format. '
+                                     + 'Wild chars (i.e., "*") are also supported. The input file could be a BAM, tri-alignment, or triplets file. '
+                                     + 'In case of BAM or tri-alignment, the file  needs to be indexed.')
     parser_virthic.add_argument('--output_dir', default='./plots/', metavar='<PATH>',
                                 help='Output directory where the plot will be stored (default: %(default)s)')
     parser_virthic.add_argument('--output_name', default=None, metavar='<FILENAME>',
                                 help='Output file name for the plot. If not provided, the output is stored using the input filename, with a `.pdf` extension.')
     parser_virthic.add_argument('--view_chrom', required=True, metavar='<STRING>', help='Name of the chromosome from which contact data are collected')
     parser_virthic.add_argument('--view_start', required=True, type=float, metavar='<INTEGER>', help='Start position of the chunk from which counts are collected')
     parser_virthic.add_argument('--view_end', required=True, type=float, metavar='<INTEGER>', help='End position of the chunk from which contact data are collected')
@@ -434,34 +436,34 @@
     parser_hic.add_argument('--columns', default='count_AB,count_AC,count_ABC', metavar='<STRING>', help='A comma-separated list of column names that should be plotted (default: "%(default)s")')
     parser_hic.add_argument('--params', default=None, metavar='COLUMN-NAME:PARAM-NAME=PARAM-VALUE[,...]', help='A comma-separated list of column names and their corresponding parameteres and values')
     parser_hic.add_argument('--mapping_quality', default=5, type=int, metavar='<INTEGER>', help='Minimum mapping quality threshold to consider an alignment to be valid (default: "%(default)s")')
     parser_hic.set_defaults(func=cli_plot_hic)
 
     # plotting processing history
     parser_proc_hist = command_plot.add_parser('processing_history', help='Plot the processing history of the given input file.')
-    parser_proc_hist.add_argument('--input', required=True, metavar='<PATH>', help='Path to concatemer, triplet or bin-triplet file.')
+    parser_proc_hist.add_argument('--input', required=True, metavar='<PATH>', help='Path to Concatemers, Tri-alignments or Triplets file.')
     parser_proc_hist.add_argument('--output_dir', default='./plots/', metavar='<PATH>',
                                   help='Output directory where the plot will be stored (default: %(default)s)')
     parser_proc_hist.add_argument('--output_name', default=None, metavar='<FILENAME>',
                                   help='Output file name for the plot. If not provided, the output is stored using the input filename, with `.processing-history.pdf` suffix.')
     parser_proc_hist.add_argument('--igraph_params', default=None, metavar='<STRING>:<STRING>[,<STRING>:<STRING>]', help='A comma-separated list of key:value parameters. Will be sent directly to igraph for plotting.')
     parser_proc_hist.set_defaults(func=cli_plot_processing_history)
 
     # plotting read length histogram
     parser_hist_read_len = command_plot.add_parser('read_length', help='Plot the read length histogram of concatemers stored in the input file.')
-    parser_hist_read_len.add_argument('--input', required=True, metavar='<PATH>', help='Path to concatemer file.')
+    parser_hist_read_len.add_argument('--input', required=True, metavar='<PATH>', help='Path to Concatemers file.')
     parser_hist_read_len.add_argument('--output_dir', default='./plots/', metavar='<PATH>',
                                       help='Output directory where the plot will be stored (default: %(default)s)')
     parser_hist_read_len.add_argument('--output_name', default=None, metavar='<FILENAME>',
                                       help='Output file name for the plot. If not provided, the output is stored using the input filename, following `read-length.<filename>.pdf` pattern.')
     parser_hist_read_len.set_defaults(func=cli_plot_read_length_histogram)
 
     # plotting alignment length histogram
     parser_hist_aln_len = command_plot.add_parser('alignment_length', help='Plot the alignment length histogram of concatemers stored in the input file.')
-    parser_hist_aln_len.add_argument('--input', required=True, metavar='<PATH>', help='Path to concatemer file.')
+    parser_hist_aln_len.add_argument('--input', required=True, metavar='<PATH>', help='Path to Concatemers file.')
     parser_hist_aln_len.add_argument('--output_dir', default='./plots/', metavar='<PATH>',
                                      help='Output directory where the plot will be stored (default: %(default)s)')
     parser_hist_aln_len.add_argument('--output_name', default=None, metavar='<FILENAME>',
                                      help='Output file name for the plot. If not provided, the output is stored using the input filename, following `alignment-length.<filename>.pdf` pattern.')
     parser_hist_aln_len.add_argument('--mapping_quality', default=5, type=int, metavar='<INTEGER>', help='Minimum mapping quality threshold to consider an alignment to be valid (default: "%(default)s")')
     parser_hist_aln_len.add_argument('--max_length', default=int(3e3), type=float, metavar='<INTEGER>', help='Minimum mapping quality threshold to consider an alignment to be valid (default: "%(default)s")')
     parser_hist_aln_len.set_defaults(func=cli_plot_alignment_length_histogram)
@@ -470,20 +472,20 @@
     # calculating statistics
     parser_stats = commands.add_parser('stat', help='Generate statistics from a given input file.')
     command_stat = parser_stats.add_subparsers(
         title='available analyses are',
         dest='analysis',
     )
 
-    parser_decay = command_stat.add_parser('decay', help='Calculates decay stats for a given Concatemer file.')
-    parser_decay.add_argument('--input', required=True, metavar='<PATH>', help='Path to input Concatemer file (e.g. `*.concatemers.h5`).')
+    parser_decay = command_stat.add_parser('decay', help='Calculates decay stats for a given Concatemers file.')
+    parser_decay.add_argument('--input', required=True, metavar='<PATH>', help='Path to input Concatemers file (e.g. `*.concatemers.h5`).')
     parser_decay.add_argument('--output_dir', default='./stats/', metavar='<PATH>',
                               help='Output directory where the stats will be stored (default: %(default)s)')
     parser_decay.add_argument('--output_name', default=None, metavar='<FILENAME>',
-                              help='Output file name. If not provided, the output is stored using the input Concatemer filename, with a `.tsv` extension.')
+                              help='Output file name. If not provided, the output is stored using the input Concatemers filename, with a `.tsv` extension.')
     parser_decay.set_defaults(func=cli_stat_decay)
 
     # processing CLI input arguments
     cli_args = parser_main.parse_args()
 
     # set global logger
     logger_global = logging.getLogger()
```

### Comparing `triplix-0.0.1/src/triplix/core/concatemers.py` & `triplix-0.0.2/src/triplix/core/concatemers.py`

 * *Files identical despite different names*

### Comparing `triplix-0.0.1/src/triplix/core/configurations.py` & `triplix-0.0.2/src/triplix/core/configurations.py`

 * *Files identical despite different names*

### Comparing `triplix-0.0.1/src/triplix/core/hdf5.py` & `triplix-0.0.2/src/triplix/core/hdf5.py`

 * *Files identical despite different names*

### Comparing `triplix-0.0.1/src/triplix/core/header.py` & `triplix-0.0.2/src/triplix/core/header.py`

 * *Files 0% similar despite different names*

```diff
@@ -344,15 +344,15 @@
                     'chrom_C', 'start_C', 'end_C',
                     'strand_A', 'strand_B', 'strand_C',
                     'mapq_A', 'mapq_B', 'mapq_C',
                     'frag_index_A', 'frag_index_B', 'frag_index_C',
                     'read_name', 'read_length_nbp', 'read_length_nfrag',
                     'experiment_name',
                 ]
-        elif self.file_path.endswith(('.3aln', '.btrp')):
+        elif self.file_path.endswith(('.tri-alignments.tsv.bgz', '.btrp')):
             with gzip.open(self.file_path, 'rt') as gz_file:
 
                 # get file type
                 file_type = next(gz_file).rstrip()
                 assert file_type in ['## Triplets', '## Triplix'], 'Unknown file format'
 
                 sam_headers = []
@@ -391,15 +391,15 @@
                         #     continue
                         setattr(self, attr_name, int(attr_value))
                     else:
                         setattr(self, attr_name, attr_value)
                     if attr_name == 'column_names':
                         break
             self.process_history = ProcessHistoryDAG(sam_headers)
-        elif self.file_path.endswith('.trpl'):
+        elif self.file_path.endswith('.triplets.h5'):
             with HDF5Container(self.file_path, mode='r', exclusive=self.exclusive) as container:
                 expr_grp = container.h5_file['experiments']
                 self.experiment_name = list(expr_grp.keys())[0]
                 self.anchor_width = expr_grp[self.experiment_name].attrs['anchor_width']
 
                 chrom_grp = expr_grp[self.experiment_name]['chroms']
                 self.chrom_lengths = {chr_name.decode(): chr_length for chr_name, chr_length in zip(chrom_grp['name'], chrom_grp['length'])}
```

### Comparing `triplix-0.0.1/src/triplix/core/plot.py` & `triplix-0.0.2/src/triplix/core/plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -257,15 +257,15 @@
                                     #     print(read[['id', 'start', 'end', 'start_bidx', 'end_bidx']])
                                     #     print(images['count_ABC'][ovl_i, ovl_j])
 
             # seen_ids_collection[bam_fpath] = copy.deepcopy(seen_ids)
             logger.info(f'\t{n_contact:,d} contacts are stored, and {n_dup:,d} are ignored due to duplicity.')
 
         # tri-alignment input
-        elif input_path.suffix in ['.3aln', '.btrp']:
+        elif input_path.suffix in ['.tri-alignments.tsv.bgz', '.btrp']:
             logger.info(f'Loading tri-alignments from: {input_path}')
             tri_alignments_obj = TriAlignmentsContainer(trialn_path=input_path)
 
             # map tri-alignments to data cubes
             anchor_max_distance = anchor_edges[-1] - anchor_edges[0]
             counts = np.zeros([n_anchor, n_anchor, n_anchor], dtype=int)
             n_load = 0
@@ -304,15 +304,15 @@
 
             # collect data from the viewpoint slice
             for col_name in plot_names:
                 has_value = np.isnan(images[col_name]) & ~ np.isnan(cubes[col_name][vp_bdx])
                 images[col_name][has_value] = 0
                 images[col_name][has_value] += cubes[col_name][vp_bdx][has_value]
 
-        elif input_path.suffix == '.trpl':
+        elif input_path.suffix == '.triplets.h5':
             logger.info(f'Loading triplets from: {input_path}')
 
             # prepare Triplets object
             triplets_obj = TripletsContainer(input_path)
             triplets = triplets_obj.fetch(
                 chrom_a=view_chrom, start_a=anchor_edges[0], end_a=anchor_edges[-1] - 1,
                 chrom_b=view_chrom, start_b=anchor_edges[0], end_b=anchor_edges[-1] - 1,
@@ -599,15 +599,15 @@
                                 pair_id = (ovl_i, ovl_j)
                                 if pair_id not in seen_ids:
                                     seen_ids[pair_id] = set()
                                     if np.isnan(images['count_AB'][ovl_i, ovl_j]):
                                         images['count_AB'][ovl_i, ovl_j] = 0
                                         images['count_AB'][ovl_j, ovl_i] = 0
 
-                                # ignore if the read has contributed to the current bin-triplet
+                                # ignore, if the read has already contributed to the current triplet
                                 if read_id in seen_ids[pair_id]:
                                     n_dup += 1
                                     continue
                                 seen_ids[pair_id].add(read_id)
 
                                 images['count_AB'][ovl_i, ovl_j] += 1
                                 images['count_AB'][ovl_j, ovl_i] += 1
```

### Comparing `triplix-0.0.1/src/triplix/core/stat.py` & `triplix-0.0.2/src/triplix/core/stat.py`

 * *Files identical despite different names*

### Comparing `triplix-0.0.1/src/triplix/core/tri_alignment/extract.py` & `triplix-0.0.2/src/triplix/core/tri_alignment/extract.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# todo: add an argument to ignore adding triplet that are overlapping each other within a read
+# todo: add an argument to ignore adding Triplets that are overlapping with each other within a read
 
 
 import gzip
 import logging
 import pathlib
 import copy
 import time
@@ -32,26 +32,26 @@
         self.concatemers_path = pathlib.Path(concatemers_path).expanduser()
         self.header = TriplixHeader(file_path=concatemers_path)
         self.experiment_name = self.header.experiment_name
 
         if output_dir is None:
             output_dir = self.concatemers_path.parent
         if output_name is None:
-            output_name = str(self.concatemers_path.name).replace('.concatemers.h5', '') + '.3aln'
+            output_name = str(self.concatemers_path.name).replace('.concatemers.h5', '') + '.tri-alignments.tsv.bgz'
         self.output_path = pathlib.Path(output_dir).expanduser() / output_name
         self.output_path.parent.mkdir(parents=True, exist_ok=True)
 
     def extract_tri_alignments(self):
 
         # initialize output files and add Triplix headers
         output_files = {}
         for chrom in self.header.chrom_lengths.keys():
             if chrom == 'unmapped':
                 continue
-            output_path = str(self.output_path).replace('.3aln', f'.{chrom}.3aln')
+            output_path = str(self.output_path).replace('.tri-alignments.tsv.bgz', f'.{chrom}.tri-alignments.tsv.bgz')
             logger.debug(f'Initializing output file: {output_path}')
             output_files[chrom] = gzip.open(output_path, 'wt', compresslevel=3)
 
             # include a PG header SAM headers to describe the Triplet generation procedure
             taln_header = copy.deepcopy(self.header)
             taln_header.stored_chunks = [(chrom, 0, self.header.chrom_lengths[chrom])]
             taln_header.process_history.add_pg(dict(ID=COMMAND_ID, PN=COMMAND_NAME, VN=configurations.configs['version'], PS=[taln_header.process_history.destination_id]))
```

### Comparing `triplix-0.0.1/src/triplix/core/tri_alignment/index.py` & `triplix-0.0.2/src/triplix/core/tri_alignment/index.py`

 * *Files identical despite different names*

### Comparing `triplix-0.0.1/src/triplix/core/tri_alignment/merge.py` & `triplix-0.0.2/src/triplix/core/tri_alignment/merge.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     def __init__(self, input_patterns, output_dir=None, output_name=None, concatenate_only=False, check_coverage=False, sort_by=None, metadata=None):
         self.concatenate_only = concatenate_only
         self.check_coverage = check_coverage
         self.sort_by = sort_by
         operation_str = 'concatenated' if self.concatenate_only else 'merged'
 
         # collecting of input files details
-        logger.info('Collecting triplet headers ...')
+        logger.info('Collecting Triplets headers ...')
         self.input_files = []
         for pattern in input_patterns.split(','):
             pattern = str(pathlib.Path(pattern).expanduser())
             for file_path in glob.glob(pattern):
                 file = {
                     'pattern': pattern,
                     'path': pathlib.Path(file_path).expanduser(),
```

### Comparing `triplix-0.0.1/src/triplix/core/tri_alignment/sort.py` & `triplix-0.0.2/src/triplix/core/tri_alignment/sort.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     def __init__(self, trialign_path, output_dir=None, output_name=None):
         self.trialign_path = pathlib.Path(trialign_path).expanduser()
         self.header = TriplixHeader(file_path=trialign_path)
 
         if output_dir is None:
             output_dir = self.trialign_path.parent
         if output_name is None:
-            output_name = self.trialign_path.stem + '.sorted.3aln'
+            output_name = self.trialign_path.stem + '.sorted.tri-alignments.tsv.bgz'
         self.output_path = pathlib.Path(output_dir).expanduser() / output_name
         self.output_path.parent.mkdir(parents=True, exist_ok=True)
         if self.output_path.is_file():
             self.output_path.unlink()
 
     def sort_tri_alignments(self, n_thread, memory):
         col2num = {col_name: col_idx + 1 for col_idx, col_name in enumerate(self.header.column_names)}
```

### Comparing `triplix-0.0.1/src/triplix/core/tri_alignments.py` & `triplix-0.0.2/src/triplix/core/tri_alignments.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,28 +36,28 @@
     def initialize(self):
         for anc_lbl in ['A', 'B', 'C']:
             for anc_type in ['chrom', 'start', 'end']:
                 self[f'{anc_type}_{anc_lbl}'] = []
 
     def __repr__(self):
         if 'start_A' not in self:
-            return '<Miss-formatted Tri-Alignments>: Missing `start_A` column'
+            return '<Miss-formatted Tri-alignments>: Missing `start_A` column'
 
         n_row = len(self['start_A'])
         n_show = self.options['display.min_rows']
         if n_row == 0 or n_row <= n_show:
             show_df = pd.DataFrame(self).astype(str)
         else:
             show_idxs = list(range(0, n_show + 1)) + list(range(n_row - n_show, n_row))
             show_df = pd.DataFrame({key: np.array(values)[show_idxs] for (key, values) in self.items()}, index=show_idxs)
             show_df = show_df.astype(str)
             show_df.loc[n_show, :] = '***'
             show_df.index = show_df.index.astype(str)
             show_df.rename({str(n_show): '***'}, axis=0, inplace=True)
-        return '<Tri-Alignments>:\n' + repr(show_df)
+        return '<Tri-alignments>:\n' + repr(show_df)
 
     def __len__(self):
         for column in self.keys():
             return len(self[column])
 
     def convert_dtypes(self):
         for hdr in self.keys():
@@ -185,15 +185,15 @@
                 #     for hdr in tri_alignments.keys():
                 #         tri_alignments[hdr] = tri_alignments[hdr][is_mapped]
 
                 # find overlaps across bins
                 start_idxs = np.searchsorted(anchor_edges, tri_alignments['start_C'], side='right') - 1
                 end_idxs = np.searchsorted(anchor_edges, tri_alignments['end_C'], side='right') - 1
 
-                # make sure each read contributes only once to each triplet
+                # make sure each read contributes only once to each Triplet
                 seen_ids = [set() for _ in range(n_anchor)]
                 for start_idx, end_idx, read_id in zip(start_idxs, end_idxs, tri_alignments['read_name']):
                     for ak in range(start_idx, end_idx + 1):
                         if anchor_edges[ak] - vp_start > anchor_max_distance:
                             continue
                         if not aj <= ak < n_anchor:  # n_bin is needed, as the `alignment_end` could still fall outside `load_end`
                             continue
@@ -291,15 +291,15 @@
     def __iter__(self):
         return self
 
     def __next__(self):
         if self.EOF:
             raise StopIteration()
 
-        # initialize a Tri-Alignments container
+        # initialize a Tri-alignments container
         tri_alignments = TriAlignments()
         for col in self.return_columns:
             tri_alignments[col] = []
 
         # load a batch of tri-alignments
         n_load = 0
         for line in self.trialn_iter:
```

### Comparing `triplix-0.0.1/src/triplix/core/triplet/bin.py` & `triplix-0.0.2/src/triplix/core/triplet/bin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import time
 import pathlib
 import logging
-from collections import deque
 
 import numpy as np
 
 from triplix.core.triplets import TripletsContainer, Triplets
 from triplix.core.header import TriplixHeader
 from triplix.core import configurations
 from triplix.core.tri_alignments import TriAlignmentsContainer
-from triplix.core.utilities import generate_prog_id, merge_intervals
+from triplix.core.utilities import generate_prog_id
 
 COMMAND_NAME = 'triplix.bin'
 COMMAND_ID = f'{COMMAND_NAME}>{generate_prog_id()}'
 logger = logging.getLogger(COMMAND_NAME)
 
 
 class TriAlignmentBinner:
@@ -35,15 +34,15 @@
         self.header = TriplixHeader(file_path=input_path)
         self.output_dir = output_dir
         self.output_name = output_name
 
         if output_dir is None:
             output_dir = self.input_path.parent
         if output_name is None:
-            output_name = self.header.experiment_name + '.trpl'
+            output_name = self.header.experiment_name + '.triplets.h5'
         self.output_path = pathlib.Path(output_dir).expanduser() / output_name
         self.output_path.parent.mkdir(parents=True, exist_ok=True)
 
         # open or initialize the container
         self.trpl_container = TripletsContainer(
             container_path=self.output_path,
             tri_alignments_path=self.input_path,
```

### Comparing `triplix-0.0.1/src/triplix/core/triplet/enrichment.py` & `triplix-0.0.2/src/triplix/core/triplet/enrichment.py`

 * *Files identical despite different names*

### Comparing `triplix-0.0.1/src/triplix/core/triplet/kdtree.py` & `triplix-0.0.2/src/triplix/core/triplet/kdtree.py`

 * *Files identical despite different names*

### Comparing `triplix-0.0.1/src/triplix/core/triplet/transform.py` & `triplix-0.0.2/src/triplix/core/triplet/transform.py`

 * *Files 0% similar despite different names*

```diff
@@ -181,15 +181,15 @@
             'start_A', 'start_B', 'start_C',
             f'{label}_A', f'{label}_B', f'{label}_C',
             f'{label}_AB', f'{label}_AC', f'{label}_BC',
             f'{label}_ABC', f'{label}_surround',
         ]
         triplets_output = Triplets(columns=triplet_columns)
 
-        # storing bin-triplet counts
+        # storing Triplets counts
         logger.log_time = 0
         n_store = 0
         for ai in range(n_anchor):
             if not chunk_start <= anchor_edges[ai] < chunk_end:
                 continue
             if anchor_edges[ai] > chrom_size:
                 logger.debug(f'End of chromosome {chunk_chrom} ({chrom_size:,d} bp) is reached, ignoring the rest.')
```

### Comparing `triplix-0.0.1/src/triplix/core/triplets.py` & `triplix-0.0.2/src/triplix/core/triplets.py`

 * *Files identical despite different names*

### Comparing `triplix-0.0.1/src/triplix/core/utilities.py` & `triplix-0.0.2/src/triplix/core/utilities.py`

 * *Files identical despite different names*

### Comparing `triplix-0.0.1/src/triplix.egg-info/PKG-INFO` & `triplix-0.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: triplix
-Version: 0.0.1
-Summary: A python package to efficiently process, store and retrieve multi-contact data
+Version: 0.0.2
+Summary: A python package to efficiently process, store and retrieve spatial genomics multi-contact data
 Author-email: Amin Allahyar <amin.allahyar@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Amin Allahyar
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -31,31 +31,45 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Triplix
+[![PyPI version](https://badge.fury.io/py/triplix.svg)](https://badge.fury.io/py/triplix)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/triplix.svg)
+[![MIT](https://img.shields.io/pypi/l/triplix.svg?color=green)](https://opensource.org/licenses/MIT)
+
+A python package to efficiently process, store and retrieve spatial genomics multi-contact data.
 
 ## Introduction:
 Triplix provides access to multi-contact data, that could be stored in three different spaces (i.e., resolution): 
 1. **Concatemers**: An HDF5 container that stores multi-contact data in a table-like format. 
 Each row in this table is an alignment that is captured by a particular `concatemer` (i.e., a sequenced long `read`). 
 There is an index (i.e., `read_idx`) column in this table that specifies alignments that originate from each specific `concatemer`.
 
-2. **Tri-Alignments**:
-Every possible three cis-alignments of each `concatemer` is stored in the Tri-Alignment file. Each three cis-alignment is called a `tri-alignment`. 
+2. **Tri-alignments**:
+Every possible three cis-alignments of each `concatemer` is stored in the Tri-alignment file. Each three cis-alignment is called a `tri-alignment`. 
 Such a data structure facilitates 3-way interaction analyses, and allow random-access. 
 To this end, `Triplix` has a simple wrapper around [pairix](https://github.com/4dn-dcic/pairix).
 In particular, the relevant `tri-alignments` are loaded by checking the first two given coordinates using `pairix`, and then filtering for the third coordinate via an ordinary overlap check.
 
 3. **Triplets**:
-Triples are essentially Tri-Alignment files, where `tri-alignments` are aggregated into genomic bins. 
+Triples are essentially Tri-alignment files, where `tri-alignments` are aggregated into genomic bins. 
 This not only reduces the disk (and memory) footprint, but also facilitates random-access. Considering the sparcity of the multi-contact data, most (if not all) multi-contact analyses are done in this "binned" space (rather than `alignment` space).
 
+## Installation
+You may run the following commands in your command line to install Triplix.
+```bash
+pip3 install triplix
+
+# or
+python3 -m pip install triplix
+```
+
 ## Usage:
 Below, you can see how you can extract data in each space.
 
 #### 1. Concatemer space  (*.concatemers.h5)
 Provides random-access to read (i.e., `concatemer`) level data. 
 
 First, we open `concatemers` container via:
@@ -124,26 +138,26 @@
 #    chrom_num     start  strand                             read_name
 # 0          5  92933191      -1  0000eea6-4554-40c3-b4ab-ecaa5cf5795b
 # 1          5  23899224       1  0000eea6-4554-40c3-b4ab-ecaa5cf5795b
 # 2          5  33962641      -1  0000eea6-4554-40c3-b4ab-ecaa5cf5795b
 # 
 ```
 
-#### 2. Tri-Alignment space (*.3ln):
-Provides access to alignment (i.e., `tri-alignment`) level data. 
+#### 2. Tri-alignment space (*.tri-alignments.tsv.bgz):
+Provides access to alignment (i.e., `tri-alignments`) level data. 
 These files are essentially formatted as compressed [pairix files](https://github.com/4dn-dcic/pairix). The difference is that they contain three coordinates instead of two coordinates (as is the case for regular pairix files)
 
-> **Note:** The tri-alignment files need to be indexed if you like to have random access to them. You can do this using `triplix index --input=input-file.3aln`
+> **Note:** The tri-alignment files need to be indexed if you like to have random access to them. You can do this using `triplix index --input=input-file.tri-alignments.tsv.bgz`
 
 An example of this usage is as follows:
 
 ```python
 import triplix
 
-tri_aln_path = './tri-alignments/GM12878.Merged.3aln'
+tri_aln_path = './tri-alignments/GM12878.Merged.tri-alignments.tsv.bgz'
 tri_container = triplix.TriAlignmentsContainer(trialn_path=tri_aln_path)
 
 tri_alignments_iter = tri_container.fetch(chrom_a='chrY', start_a=0e6, end_a=10e6, batch_size=10)
 for idx, tri_alignments in enumerate(tri_alignments_iter):
     df = tri_alignments.to_dataframe()
     print(df[['read_name', 'chrom_A', 'start_A', 'start_B', 'start_C']])
     if idx > 0:
@@ -168,22 +182,22 @@
 # 6  0f526116-e8fc-459b-aac9-d9d6d2843289    chrY    13584   278514   366665
 # 7  6589f1d9-cd7d-4cba-bfc9-06f123956157    chrY    13584   282655   440783
 # 8  0f526116-e8fc-459b-aac9-d9d6d2843289    chrY    13584   364567   366665
 # 9  11f46754-fbfe-4f9f-8aa6-7f03c7db48df    chrY    13584  1180971  1812799
 
 ```
 
-#### 3. Triplet space (*.trpl):
+#### 3. Triplet space (*.triplets.h5):
 Provides access to triplet-level data. A usage example is:
 
 ```python
 import pandas as pd
 import triplix
 
-trpl_path = './triplets/GM12878.MC-HiC.hg38.trpl'
+trpl_path = './triplets/GM12878.MC-HiC.hg38.triplets.h5'
 trpl_obj = triplix.TripletsContainer(container_path=trpl_path)
 triplets_input = trpl_obj.fetch(
     chrom_a='chr8', start_a=119e6, end_a=120e6,
     columns=['start_A', 'start_B', 'start_C', 'count_ABC'],
 )
 df = pd.DataFrame(triplets_input)
 print(df)
@@ -200,15 +214,7 @@
 # 136158  120000000  121975000  121975000          5
 # 136159  120000000  121975000  122000000          7
 # 136160  120000000  122000000  122000000          6
 # 
 # [136161 rows x 4 columns]
 ```
 
-## Installation
-Simply run the following command to install Triplix.
-```bash
-pip3 install triplix
-
-# or
-python3 -m pip install triplix
-```
```

### Comparing `triplix-0.0.1/src/triplix.egg-info/SOURCES.txt` & `triplix-0.0.2/src/triplix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

