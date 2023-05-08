# Comparing `tmp/fastq_dl-2.0.0.tar.gz` & `tmp/fastq_dl-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastq_dl-2.0.0.tar", max compression
+gzip compressed data, was "fastq_dl-2.0.1.tar", max compression
```

## Comparing `fastq_dl-2.0.0.tar` & `fastq_dl-2.0.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1076 2023-02-10 04:33:07.891029 fastq_dl-2.0.0/LICENSE
--rw-r--r--   0        0        0    10364 2023-02-10 04:33:07.891029 fastq_dl-2.0.0/README.md
--rw-r--r--   0        0        0        0 2023-02-10 04:33:07.891029 fastq_dl-2.0.0/fastq_dl/__init__.py
--rwxr-xr-x   0        0        0    21636 2023-02-10 04:33:07.891029 fastq_dl-2.0.0/fastq_dl/fastq_dl.py
--rw-r--r--   0        0        0      829 2023-02-10 04:33:07.895029 fastq_dl-2.0.0/pyproject.toml
--rw-r--r--   0        0        0    11443 1970-01-01 00:00:00.000000 fastq_dl-2.0.0/setup.py
--rw-r--r--   0        0        0    11284 1970-01-01 00:00:00.000000 fastq_dl-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-05-08 03:35:04.772854 fastq_dl-2.0.1/LICENSE
+-rw-r--r--   0        0        0    10364 2023-05-08 03:35:04.772854 fastq_dl-2.0.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-08 03:35:04.772854 fastq_dl-2.0.1/fastq_dl/__init__.py
+-rwxr-xr-x   0        0        0    20611 2023-05-08 03:35:04.772854 fastq_dl-2.0.1/fastq_dl/fastq_dl.py
+-rw-r--r--   0        0        0      854 2023-05-08 03:35:04.776854 fastq_dl-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0    11469 1970-01-01 00:00:00.000000 fastq_dl-2.0.1/setup.py
+-rw-r--r--   0        0        0    11324 1970-01-01 00:00:00.000000 fastq_dl-2.0.1/PKG-INFO
```

### Comparing `fastq_dl-2.0.0/LICENSE` & `fastq_dl-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fastq_dl-2.0.0/README.md` & `fastq_dl-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `fastq_dl-2.0.0/fastq_dl/fastq_dl.py` & `fastq_dl-2.0.1/fastq_dl/fastq_dl.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,74 +35,20 @@
                 "--help",
             ],
         },
     ]
 }
 
 PROGRAM = "fastq-dl"
-VERSION = "2.0.0"
+VERSION = "2.0.1"
 ENA_FAILED = "ENA_NOT_FOUND"
 SRA_FAILED = "SRA_NOT_FOUND"
 SRA = "SRA"
 ENA = "ENA"
-
 ENA_URL = "https://www.ebi.ac.uk/ena/portal/api/search?result=read_run&format=tsv"
-FIELDS = [
-    "study_accession",
-    "secondary_study_accession",
-    "sample_accession",
-    "secondary_sample_accession",
-    "experiment_accession",
-    "run_accession",
-    "submission_accession",
-    "tax_id",
-    "scientific_name",
-    "instrument_platform",
-    "instrument_model",
-    "library_name",
-    "library_layout",
-    "nominal_length",
-    "library_strategy",
-    "library_source",
-    "library_selection",
-    "read_count",
-    "base_count",
-    "center_name",
-    "first_public",
-    "last_updated",
-    "experiment_title",
-    "study_title",
-    "study_alias",
-    "experiment_alias",
-    "run_alias",
-    "fastq_bytes",
-    "fastq_md5",
-    "fastq_ftp",
-    "fastq_aspera",
-    "fastq_galaxy",
-    "submitted_bytes",
-    "submitted_md5",
-    "submitted_ftp",
-    "submitted_aspera",
-    "submitted_galaxy",
-    "submitted_format",
-    "sra_bytes",
-    "sra_md5",
-    "sra_ftp",
-    "sra_aspera",
-    "sra_galaxy",
-    "cram_index_ftp",
-    "cram_index_aspera",
-    "cram_index_galaxy",
-    "sample_alias",
-    "broker_name",
-    "sample_title",
-    "nominal_sdev",
-    "first_created",
-]
 
 
 def execute(
     cmd: str,
     directory: str = str(Path.cwd()),
     capture_stdout: bool = False,
     stdout_file: str = None,
@@ -369,22 +315,23 @@
     if df is None:
         return [False, []]
     return [True, df.to_dict(orient="records")]
 
 
 def get_ena_metadata(query: str) -> list:
     """Fetch metadata from ENA.
+    https://docs.google.com/document/d/1CwoY84MuZ3SdKYocqssumghBF88PWxUZ/edit#heading=h.ag0eqy2wfin5
 
     Args:
         query (str): The query to search for.
 
     Returns:
         list: Records associated with the accession.
     """
-    url = f'{ENA_URL}&query="{query}"&fields={",".join(FIELDS)}'
+    url = f'{ENA_URL}&query="{query}"&fields=all'
     headers = {"Content-type": "application/x-www-form-urlencoded"}
     r = requests.get(url, headers=headers)
     if r.status_code == requests.codes.ok:
         data = []
         col_names = None
         for line in r.text.split("\n"):
             cols = line.rstrip().split("\t")
```

### Comparing `fastq_dl-2.0.0/pyproject.toml` & `fastq_dl-2.0.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastq-dl"
-version = "2.0.0"
+version = "2.0.1"
 description = "Download FASTQ files from SRA or ENA repositories."
 authors = [
     "Robert A. Petit III <robbie.petit@gmail.com>",
     "Michael B. Hall <michael@mbh.sh>"
 ]
 license = "MIT"
 readme = "README.md"
@@ -18,14 +18,15 @@
 [tool.poetry.dependencies]
 python = "^3.7.1"
 requests = "^2.28.2"
 pysradb = "^1.4"
 rich-click = "^1.6.1"
 executor = "^23.2"
 rich = "^13.3.1"
+markdown-it-py = "2.2.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.1.0"
 isort = "^5.0"
 flake8 = "^5.0"
 
 [tool.isort]
```

### Comparing `fastq_dl-2.0.0/setup.py` & `fastq_dl-2.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,25 +5,26 @@
 ['fastq_dl']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['executor>=23.2,<24.0',
+ 'markdown-it-py==2.2.0',
  'pysradb>=1.4,<2.0',
  'requests>=2.28.2,<3.0.0',
  'rich-click>=1.6.1,<2.0.0',
  'rich>=13.3.1,<14.0.0']
 
 entry_points = \
 {'console_scripts': ['fastq-dl = fastq_dl.fastq_dl:main']}
 
 setup_kwargs = {
     'name': 'fastq-dl',
-    'version': '2.0.0',
+    'version': '2.0.1',
     'description': 'Download FASTQ files from SRA or ENA repositories.',
     'long_description': "[![GitHub release (latest by date)](https://img.shields.io/github/v/release/rpetit3/fastq-dl)](https://github.com/bactopia/rpetit3/fastq-dl)\n[![Anaconda-Server Badge](https://anaconda.org/bioconda/fastq-dl/badges/downloads.svg)](https://anaconda.org/bioconda/fastq-dl)\n[![Gitpod ready-to-code](https://img.shields.io/badge/Gitpod-ready--to--code-908a85?logo=gitpod)](https://gitpod.io/#https://github.com/rpetit3/fastq-dl)\n\n# fastq-dl\n\nDownload FASTQ files from the [European Nucleotide Archive](https://www.ebi.ac.uk/ena) or the\n[Sequence Read Archive](https://www.ncbi.nlm.nih.gov/sra) repositories.\n\n## Introduction\n\n`fastq-dl` takes an ENA/SRA accession (Study, Sample, Experiment, or Run) and queries ENA (via\n[Data Warehouse API](https://www.ebi.ac.uk/ena/browse/search-rest)) to determine the associated\nmetadata. It then downloads FASTQ files for each Run. For Samples or Experiments with multiple\nRuns, users can optionally merge the runs.\n\n## Installation\n\n### Bioconda\n\n`fastq-dl` is available from [Bioconda](https://bioconda.github.io/) and I highly recommend you\ngo this route to for installation.\n\n```{bash}\nconda create -n fastq-dl -c conda-forge -c bioconda fastq-dl\nconda activate fastq-dl \n```\n\n## Usage\n\n```{bash}\nfastq-dl --help\n                                                                                          \n Usage: fastq-dl [OPTIONS]                                                                \n                                                                                          \n Download FASTQ files from ENA or SRA.                                                    \n                                                                                          \n╭─ Required Options ─────────────────────────────────────────────────────────────────────╮\n│ *  --accession  -a  TEXT  ENA/SRA accession to query. (Study, Sample, Experiment, Run  │\n│                           accession) [required]                                        │\n╰────────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Additional Options ───────────────────────────────────────────────────────────────────╮\n│ --provider                 [ena|sra]  Specify which provider (ENA or SRA) to use.      │\n│                                       [default: ena]                                   │\n│ --group-by-experiment                 Group Runs by experiment accession.              │\n│ --group-by-sample                     Group Runs by sample accession.                  │\n│ --outdir               -o  TEXT       Directory to output downloads to. [default: ./]  │\n│ --prefix                   TEXT       Prefix to use for naming log files.              │\n│                                       [default: fastq]                                 │\n│ --cpus                     INTEGER    Total cpus used for downloading from SRA.        │\n│                                       [default: 1]                                     │\n│ --max-attempts         -m  INTEGER    Maximum number of download attempts.             │\n│                                       [default: 10]                                    │\n│ --only-provider        -F             Only attempt download from specified provider.   │\n│ --silent                              Only critical errors will be printed.            │\n│ --version              -V             Show the version and exit.                       │\n│ --verbose              -v             Print debug related text.                        │\n│ --help                 -h             Show this message and exit.                      │\n╰────────────────────────────────────────────────────────────────────────────────────────╯\n```\n\n*fastq-dl* requires a single ENA/SRA Study, Sample, Experiment, or Run accession and FASTQs\nfor all Runs that fall under the given accession will be downloaded. For example, if a Study\naccession is given all Runs under that studies umbrella will be downloaded. By default, \n`fastq-dl` will try to download from ENA first, then SRA.\n\n### --accession\n\nThe accession you would like to download associated FASTQS for. Currently the following types\nof accessions are accepted.\n\n| Accession Type | Prefixes            | Example                                  |\n|----------------|---------------------|------------------------------------------|\n| BioProject     | PRJEB, PRJNA, PRJDB | PRJEB42779, PRJNA480016, PRJDB14838      |\n| Study          | ERP, DRP, SRP       | ERP126685, DRP009283, SRP158268          |\n| BioSample      | SAMD, SAME, SAMN    | SAMD00258402, SAMEA7997453, SAMN06479985 |\n| Sample         | ERS, DRS, SRS       | ERS5684710, DRS259711, SRS2024210        |\n| Experiment     | ERX, DRX, SRX       | ERX5050800, DRX406443, SRX4563689        |\n| Run            | ERR, DRR, SRR       | ERR5260405, DRR421224, SRR7706354        |\n\nThe accessions are using regular expressions from the [ENA Training Modules - Accession Numbers](https://ena-docs.readthedocs.io/en/latest/submit/general-guide/accessions.html#accession-numbers) section.\n\n### --provider\n\n`fastq-dl` gives you the option to download from ENA or SRA. the `--provider` option will\nspecify which provider you would like to attempt downloads from first. If a download fails\nfrom the first provider, additional attempts will be made using the other provider.\n\nENA was selected as the default provider because the FASTQs are available directly without\nthe need for conversion.\n\n### --only-provider\n\nBy default, `fastq-dl` will fallback on a secondary provider to attempt downloads. There\nmay be cases where you would prefer to disable this feature, and that is exactly the\npurpose of `--only-provider`. When provided, if a FASTQ cannot be downloaded from the\noriginal provider, no additional attempts will be made.\n\n### --group-by-experiment & --group-by-sample\n\nThere maybe times you might want to group Run accessions based on a Experiment or Sample\naccessions. This will merge FASTQs associated with a Run accession based its associated\nExperiment accession (`--group-by-experiment`) or Sample accession (`--group-by-sample`).\n\n## Output Files\n\n| Extension          | Description                                                                              |\n|--------------------|------------------------------------------------------------------------------------------|\n| `-run-info.tsv`    | Tab-delimited file containing metadata for each Run downloaded                           |\n| `-run-mergers.tsv` | Tab-delimited file merge information from `--group-by-experiment` or `--group-by-sample` |\n| `.fastq.gz`        | FASTQ files downloaded from ENA or SRA                                                   |\n\n## Example Usage\n\n#### Download FASTQs associated with a Study\n\nSometimes you might be reading a paper and they very kindly provided a Bioproject of all\nthe samples they sequenced. So, you decide you want to download FASTQs for all the samples\nasscociated with the Bioproject. `fastq-dl` can help you with that! \n\n```{bash}\nfastq-dl --accession PRJNA248678 --provider SRA\nfastq-dl --accession PRJNA248678\n```\n\nThe above commands will download the 3 Runs that fall under Study accession [PRJNA248678](https://www.ebi.ac.uk/ena/browser/view/PRJNA248678)\nfrom either SRA (`--provider SRA`) or ENA (without `--provider`).\n\n#### Download FASTQs associated with an Experiment\n\nLet's say instead of the whole Bioproject you just want a single Experiment. You can do\nthat as well.\n\n```{bash}\nfastq-dl --accession SRX477044\n```\n\nThe above command would download the Run accessions from ENA that fall under Experiment SRX477044.\n\nThe relationship of Experiment to Run is a 1-to-many relationship, or there can be many Run accessions\nassociated with a single Experiment Accession (e.g. re-sequencing the same sample). Although in most\ncases, it is a 1-to-1 relationship, you can use `--group-by-experiment` to merge multiple runs\nassociated with an Experiment accession into a single FASTQ file.\n\n#### Download FASTQs associated with an Sample\n\nOk, this time you just want a single Sample, or Biosample.\n\n```{bash}\nfastq-dl --accession SRS1904245 --provider SRA\n```\n\nThe above command would download the Run accessions from SRA that fall under Sample SRS1904245.\n\nSimilar to Experiment accessions, the relationship of Sample to Run is a 1-to-many relationship,\nor there can be many Run accessions associated with a single Sample Accession. Although in most\ncases, it is a 1-to-1 relationship, you can use `--group-by-sample` to merge multiple runs\nassociated with an Sample accession into a single FASTQ file.\n\n_Warning! For some type strains (e.g. S. aureus USA300) a Biosample accession might be associated with\n100s or 1000s of Run accessions. These Runs are likely associated with many different conditions and\nreally should not fall under a single BioSample accession. Please consider this when using\n`--group-by-sample`.\n\n#### Download FASTQs associated with a Run\n\nLet's keep it super simple and just download a Run.\n\n```\nfastq-dl --accession SRR1178105 --provider SRA\n```\n\nThe above command would download the Run SRR1178105 from SRA. Run accessions are the end of the\nline (1-to-1 relationship), so you will always get the expected Run.\n\n## Alternatives\n`fastq-dl`, is a spin-off of [ena-dl](https://github.com/rpetit3/ena-dl), that has been developed for\nusage with [Bactopia](https://github.com/bactopia/bactopia). With this in mind, EBI/NCBI and provide\ntheir own tools ([enaBrowserTools](https://github.com/enasequence/enaBrowserTools) and\n[SRA Toolkit](https://github.com/ncbi/sra-tools)) that offer more extensive access to their databases.\n",
     'author': 'Robert A. Petit III',
     'author_email': 'robbie.petit@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/rpetit3/fastq-dl',
```

### Comparing `fastq_dl-2.0.0/PKG-INFO` & `fastq_dl-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: fastq-dl
-Version: 2.0.0
+Version: 2.0.1
 Summary: Download FASTQ files from SRA or ENA repositories.
 Home-page: https://github.com/rpetit3/fastq-dl
 License: MIT
 Keywords: bioinformatics,fastq,download,SRA,ENA
 Author: Robert A. Petit III
 Author-email: robbie.petit@gmail.com
 Requires-Python: >=3.7.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: executor (>=23.2,<24.0)
+Requires-Dist: markdown-it-py (==2.2.0)
 Requires-Dist: pysradb (>=1.4,<2.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: rich (>=13.3.1,<14.0.0)
 Requires-Dist: rich-click (>=1.6.1,<2.0.0)
 Project-URL: Repository, https://github.com/rpetit3/fastq-dl
 Description-Content-Type: text/markdown
```

