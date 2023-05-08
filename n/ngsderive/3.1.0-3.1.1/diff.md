# Comparing `tmp/ngsderive-3.1.0.tar.gz` & `tmp/ngsderive-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ngsderive-3.1.0.tar", max compression
+gzip compressed data, was "ngsderive-3.1.1.tar", max compression
```

## Comparing `ngsderive-3.1.0.tar` & `ngsderive-3.1.1.tar`

### file list

```diff
@@ -1,16 +1,15 @@
--rwxr-xr-x   0        0        0     1077 2023-03-23 18:53:15.371540 ngsderive-3.1.0/LICENSE.md
--rw-r--r--   0        0        0     4846 2023-03-23 18:53:15.371540 ngsderive-3.1.0/README.md
--rwxr-xr-x   0        0        0        0 2023-03-23 18:53:15.371540 ngsderive-3.1.0/ngsderive/__init__.py
--rwxr-xr-x   0        0        0    12531 2023-03-23 18:53:15.371540 ngsderive-3.1.0/ngsderive/__main__.py
--rwxr-xr-x   0        0        0        0 2023-03-23 18:53:15.371540 ngsderive-3.1.0/ngsderive/commands/__init__.py
--rw-r--r--   0        0        0     2482 2023-03-23 18:53:15.371540 ngsderive-3.1.0/ngsderive/commands/encoding.py
--rwxr-xr-x   0        0        0     9238 2023-03-23 18:53:15.371540 ngsderive-3.1.0/ngsderive/commands/instrument.py
--rw-r--r--   0        0        0    11245 2023-03-23 18:53:15.371540 ngsderive-3.1.0/ngsderive/commands/junction_annotation.py
--rw-r--r--   0        0        0     2855 2023-03-23 18:53:15.371540 ngsderive-3.1.0/ngsderive/commands/junction_saturation.py
--rwxr-xr-x   0        0        0     2260 2023-03-23 18:53:15.371540 ngsderive-3.1.0/ngsderive/commands/readlen.py
--rwxr-xr-x   0        0        0    11914 2023-03-23 18:53:15.371540 ngsderive-3.1.0/ngsderive/commands/strandedness.py
--rwxr-xr-x   0        0        0        0 2023-03-23 18:53:15.371540 ngsderive-3.1.0/ngsderive/readers/__init__.py
--rwxr-xr-x   0        0        0       13 2023-03-23 18:53:15.371540 ngsderive-3.1.0/ngsderive/readers/bam.py
--rwxr-xr-x   0        0        0    14826 2023-03-23 18:53:15.371540 ngsderive-3.1.0/ngsderive/utils.py
--rw-r--r--   0        0        0     1585 2023-03-23 18:53:51.824252 ngsderive-3.1.0/pyproject.toml
--rw-r--r--   0        0        0     5956 1970-01-01 00:00:00.000000 ngsderive-3.1.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1077 2023-05-08 20:12:05.819838 ngsderive-3.1.1/LICENSE.md
+-rw-r--r--   0        0        0     4846 2023-05-08 20:12:05.819838 ngsderive-3.1.1/README.md
+-rwxr-xr-x   0        0        0        0 2023-05-08 20:12:05.819838 ngsderive-3.1.1/ngsderive/__init__.py
+-rwxr-xr-x   0        0        0     9781 2023-05-08 20:12:05.819838 ngsderive-3.1.1/ngsderive/__main__.py
+-rwxr-xr-x   0        0        0        0 2023-05-08 20:12:05.819838 ngsderive-3.1.1/ngsderive/commands/__init__.py
+-rw-r--r--   0        0        0     2482 2023-05-08 20:12:05.819838 ngsderive-3.1.1/ngsderive/commands/encoding.py
+-rwxr-xr-x   0        0        0     9238 2023-05-08 20:12:05.819838 ngsderive-3.1.1/ngsderive/commands/instrument.py
+-rw-r--r--   0        0        0    11008 2023-05-08 20:12:05.819838 ngsderive-3.1.1/ngsderive/commands/junction_annotation.py
+-rwxr-xr-x   0        0        0     2260 2023-05-08 20:12:05.819838 ngsderive-3.1.1/ngsderive/commands/readlen.py
+-rwxr-xr-x   0        0        0    11914 2023-05-08 20:12:05.819838 ngsderive-3.1.1/ngsderive/commands/strandedness.py
+-rwxr-xr-x   0        0        0        0 2023-05-08 20:12:05.819838 ngsderive-3.1.1/ngsderive/readers/__init__.py
+-rwxr-xr-x   0        0        0       13 2023-05-08 20:12:05.819838 ngsderive-3.1.1/ngsderive/readers/bam.py
+-rwxr-xr-x   0        0        0    14826 2023-05-08 20:12:05.819838 ngsderive-3.1.1/ngsderive/utils.py
+-rw-r--r--   0        0        0     1585 2023-05-08 20:12:47.616349 ngsderive-3.1.1/pyproject.toml
+-rw-r--r--   0        0        0     5956 1970-01-01 00:00:00.000000 ngsderive-3.1.1/PKG-INFO
```

### Comparing `ngsderive-3.1.0/LICENSE.md` & `ngsderive-3.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ngsderive-3.1.0/README.md` & `ngsderive-3.1.1/README.md`

 * *Files identical despite different names*

### Comparing `ngsderive-3.1.0/ngsderive/__main__.py` & `ngsderive-3.1.1/ngsderive/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 from ngsderive import utils
 from ngsderive.commands import (
     readlen,
     instrument,
     strandedness,
     encoding,
     junction_annotation,
-    junction_saturation,
 )
 
 logger = logging.getLogger("ngsderive")
 
 
 def get_args():
     class SaneFormatter(
@@ -208,70 +207,14 @@
         action="store_true",
         default=False,
         help="For the summary report, consider all events on unannotated reference sequences `complete_novel`. "
              "Default is to exclude them from the summary. "
              "Either way, they will be annotated as `unannotated_reference` in the junctions file.",
     )
 
-    junction_saturation = subparsers.add_parser(
-        "junction-saturation", parents=[common], formatter_class=SaneFormatter
-    )
-    junction_saturation.add_argument(
-        "-g", "--gene-model", help="Gene model as a GFF/GTF file.", required=True
-    )
-    junction_saturation.add_argument(
-        "-s",
-        "--sample-start",
-        type=int,
-        help="Percentage to begin sampling.",
-        default=5,
-    )
-    junction_saturation.add_argument(
-        "-p",
-        "--sample-step",
-        type=int,
-        help="Percentage to step between sample-start and sample-end.",
-        default=5,
-    )
-    junction_saturation.add_argument(
-        "-e",
-        "--sample-end",
-        type=int,
-        help="Percentage to stop sampling.",
-        default=100,
-    )
-    junction_saturation.add_argument(
-        "-i",
-        "--min-intron",
-        type=int,
-        help="Minimum size of intron to be considered a splice.",
-        default=50,
-    )
-    junction_saturation.add_argument(
-        "-q",
-        "--min-mapq",
-        type=int,
-        help="Minimum MAPQ to consider for supporting reads.",
-        default=30,
-    )
-    junction_saturation.add_argument(
-        "-m",
-        "--min-reads",
-        type=int,
-        help="Filter any junctions that don't have at least `m` reads.",
-        default=2,
-    )
-    junction_saturation.add_argument(
-        "-k",
-        "--fuzzy-junction-match-range",
-        type=int,
-        help="Consider found splices within `+-k` bases of a known splice event annotated.",
-        default=0,
-    )
-
     args = parser.parse_args()
     if not args.subcommand:
         parser.print_help()
         sys.exit(1)
 
     return args
 
@@ -324,29 +267,14 @@
 
     # set output file
     if args.outfile == "stdout":
         args.outfile = sys.stdout
     else:
         args.outfile = open(args.outfile, "w")
 
-    # check junction-saturation args
-    if args.subcommand == "junction-saturation":
-        if (
-            (not 0 <= args.sample_start and not args.sample_start <= 100)
-            or (not 0 <= args.sample_step and not args.sample_step <= 100)
-            or (not 0 <= args.sample_end and not args.sample_end <= 100)
-        ):
-            raise argparse.ArgumentError(
-                "--sample-start, --sample-step, and --sample-end must be percentages between 0 and 100 (inclusive)"
-            )
-        if args.sample_start > args.sample_end:
-            raise argparse.ArgumentError(
-                "--sample-start must be less than --sample-end"
-            )
-
 
 def run():
     args = get_args()
     process_args(args)
 
     if args.subcommand == "readlen":
         readlen.main(
@@ -391,20 +319,7 @@
             min_mapq=args.min_mapq,
             min_reads=args.min_reads,
             fuzzy_range=args.fuzzy_junction_match_range,
             consider_unannotated_references_novel=args.consider_unannotated_references_novel,
             junction_dir=args.junction_files_dir,
             disable_junction_files=args.disable_junction_files,
         )
-    if args.subcommand == "junction-saturation":
-        junction_saturation.main(
-            args.ngsfiles,
-            args.gene_model,
-            outfile=args.outfile,
-            sample_start=args.sample_start,
-            sample_step=args.sample_step,
-            sample_end=args.sample_end,
-            min_intron=args.min_intron,
-            min_mapq=args.min_mapq,
-            min_reads=args.min_reads,
-            fuzzy_range=args.fuzzy_junction_match_range,
-        )
```

### Comparing `ngsderive-3.1.0/ngsderive/commands/encoding.py` & `ngsderive-3.1.1/ngsderive/commands/encoding.py`

 * *Files identical despite different names*

### Comparing `ngsderive-3.1.0/ngsderive/commands/instrument.py` & `ngsderive-3.1.1/ngsderive/commands/instrument.py`

 * *Files identical despite different names*

### Comparing `ngsderive-3.1.0/ngsderive/commands/junction_annotation.py` & `ngsderive-3.1.1/ngsderive/commands/junction_annotation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import logging
 import sys
 import os
 import csv
-import random
 
 from collections import defaultdict
 from pathlib import Path
 
 from ..utils import NGSFile, NGSFileType, GFF, JunctionCache
 
 logger = logging.getLogger("junction-annotation")
@@ -30,15 +29,14 @@
     min_intron,
     min_mapq,
     min_reads,
     fuzzy_range,
     consider_unannotated_references_novel,
     junction_dir,
     disable_junction_files,
-    sample_rate=1,
 ):
     try:
         ngsfile = NGSFile(ngsfilepath)
     except FileNotFoundError:
         result = {
             "File": ngsfilepath,
             "total_junctions": "N/A",
@@ -46,15 +44,15 @@
             "known_junctions": "N/A",
             "partial_novel_junctions": "N/A",
             "complete_novel_junctions": "N/A",
             "known_spliced_reads": "N/A",
             "complete_novel_spliced_reads": "N/A",
             "partial_novel_spliced_reads": "N/A",
         }
-        return result
+        return [result]
 
     if ngsfile.filetype != NGSFileType.BAM:
         raise RuntimeError(
             "Invalid file: {}. `junction-annotation` only supports aligned BAM files!".format(
                 ngsfilepath
             )
         )
@@ -95,19 +93,14 @@
                 f"No valid splice junctions in {contig}. {len(found_introns)} potential junctions too short."
             )
             continue
         logger.debug(
             f"Found {len(events)} potential splice junctions. {len(found_introns) - len(events)} potential junctions too short."
         )
 
-        if sample_rate < 1:
-            n_samples = round(len(events) * sample_rate)
-            events = random.sample(events, n_samples)
-            logger.debug(f"Randomly sampled {n_samples} events.")
-
         if contig not in cache.exon_starts:
             logger.info(f"{contig} not found in GFF. All events marked `unannotated_reference`.")
             annotation = "unannotated_reference"
             if consider_unannotated_references_novel:
                 logger.info(f"Events being considered novel for summary report.")
 
             for intron_start, intron_end, num_reads in events:
```

### Comparing `ngsderive-3.1.0/ngsderive/commands/readlen.py` & `ngsderive-3.1.1/ngsderive/commands/readlen.py`

 * *Files identical despite different names*

### Comparing `ngsderive-3.1.0/ngsderive/commands/strandedness.py` & `ngsderive-3.1.1/ngsderive/commands/strandedness.py`

 * *Files identical despite different names*

### Comparing `ngsderive-3.1.0/ngsderive/utils.py` & `ngsderive-3.1.1/ngsderive/utils.py`

 * *Files identical despite different names*

### Comparing `ngsderive-3.1.0/pyproject.toml` & `ngsderive-3.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry>=1.0.5"]
 build-backend = "poetry.masonry.api"
 
 [tool.poetry]
 name = "ngsderive"
-version = "3.1.0"
+version = "3.1.1"
 description = "Forensic analysis tool useful in backwards computing information from next-generation sequencing data."
 license = "MIT"
 authors = [
     "Clay McLeod <Clay.McLeod@STJUDE.org>",
     "Andrew Frantz <andrew.frantz@STJUDE.org"
 ]
 readme = "README.md"
```

### Comparing `ngsderive-3.1.0/PKG-INFO` & `ngsderive-3.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ngsderive
-Version: 3.1.0
+Version: 3.1.1
 Summary: Forensic analysis tool useful in backwards computing information from next-generation sequencing data.
 Home-page: https://github.com/claymcleod/ngsderive
 License: MIT
 Keywords: bioinformatics,genomics,sam,bam,fastq
 Author: Clay McLeod
 Author-email: Clay.McLeod@STJUDE.org
 Requires-Python: >=3.8,<3.10
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ngsderive Version: 3.1.0 Summary: Forensic analysis
+Metadata-Version: 2.1 Name: ngsderive Version: 3.1.1 Summary: Forensic analysis
 tool useful in backwards computing information from next-generation sequencing
 data. Home-page: https://github.com/claymcleod/ngsderive License: MIT Keywords:
 bioinformatics,genomics,sam,bam,fastq Author: Clay McLeod Author-email:
 Clay.McLeod@STJUDE.org Requires-Python: >=3.8,<3.10 Classifier: Development
 Status :: 4 - Beta Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
```

