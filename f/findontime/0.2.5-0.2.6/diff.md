# Comparing `tmp/findontime-0.2.5.tar.gz` & `tmp/findontime-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "findontime-0.2.5.tar", max compression
+gzip compressed data, was "findontime-0.2.6.tar", max compression
```

## Comparing `findontime-0.2.5.tar` & `findontime-0.2.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    31904 2023-04-09 11:15:18.037313 findontime-0.2.5/LICENSE
--rw-r--r--   0        0        0    11060 2023-04-14 12:51:03.222693 findontime-0.2.5/README.md
--rw-r--r--   0        0        0      875 2023-04-19 11:19:11.744737 findontime-0.2.5/pyproject.toml
--rw-r--r--   0        0        0       24 2023-04-11 13:13:09.220772 findontime-0.2.5/src/findontime/__init__.py
--rw-r--r--   0        0        0      315 2023-04-13 15:22:43.482616 findontime-0.2.5/src/findontime/__main__.py
--rw-r--r--   0        0        0     2471 2023-04-18 15:46:13.271182 findontime-0.2.5/src/findontime/configs.py
--rw-r--r--   0        0        0     9288 2023-04-13 13:28:27.639194 findontime-0.2.5/src/findontime/connectors.py
--rw-r--r--   0        0        0     3646 2023-04-11 13:01:20.270281 findontime-0.2.5/src/findontime/drones.py
--rw-r--r--   0        0        0    16655 2023-04-19 11:17:45.199895 findontime-0.2.5/src/findontime/insaflu_uploads.py
--rw-r--r--   0        0        0     9365 2023-04-18 15:46:17.183215 findontime-0.2.5/src/findontime/manager.py
--rw-r--r--   0        0        0     4822 2023-04-11 13:01:20.270281 findontime-0.2.5/src/findontime/plot_utils.py
--rw-r--r--   0        0        0     9902 2023-04-09 11:12:06.161507 findontime-0.2.5/src/findontime/plotting_from_all_reports.py
--rw-r--r--   0        0        0     3447 2023-04-19 11:13:32.517266 findontime-0.2.5/src/findontime/records.py
--rw-r--r--   0        0        0     3444 2023-04-11 13:01:20.270281 findontime-0.2.5/src/findontime/tables_post.py
--rw-r--r--   0        0        0    21536 2023-04-13 13:27:24.031739 findontime-0.2.5/src/findontime/upload_utils.py
--rw-r--r--   0        0        0    12293 2023-04-19 11:19:23.627763 findontime-0.2.5/setup.py
--rw-r--r--   0        0        0    11964 2023-04-19 11:19:23.628511 findontime-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0    31904 2023-04-09 11:15:18.037313 findontime-0.2.6/LICENSE
+-rw-r--r--   0        0        0    10895 2023-04-19 11:20:59.393755 findontime-0.2.6/README.md
+-rw-r--r--   0        0        0      875 2023-05-08 17:19:01.369791 findontime-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0       24 2023-04-11 13:13:09.220772 findontime-0.2.6/src/findontime/__init__.py
+-rw-r--r--   0        0        0      315 2023-04-13 15:22:43.482616 findontime-0.2.6/src/findontime/__main__.py
+-rw-r--r--   0        0        0     2471 2023-04-18 15:46:13.271182 findontime-0.2.6/src/findontime/configs.py
+-rw-r--r--   0        0        0     9288 2023-04-13 13:28:27.639194 findontime-0.2.6/src/findontime/connectors.py
+-rw-r--r--   0        0        0     3767 2023-05-08 17:18:09.069512 findontime-0.2.6/src/findontime/drones.py
+-rw-r--r--   0        0        0    16655 2023-04-19 11:17:45.199895 findontime-0.2.6/src/findontime/insaflu_uploads.py
+-rw-r--r--   0        0        0     9365 2023-04-18 15:46:17.183215 findontime-0.2.6/src/findontime/manager.py
+-rw-r--r--   0        0        0     4822 2023-04-11 13:01:20.270281 findontime-0.2.6/src/findontime/plot_utils.py
+-rw-r--r--   0        0        0     9902 2023-04-09 11:12:06.161507 findontime-0.2.6/src/findontime/plotting_from_all_reports.py
+-rw-r--r--   0        0        0     3447 2023-04-19 11:13:32.517266 findontime-0.2.6/src/findontime/records.py
+-rw-r--r--   0        0        0     3444 2023-04-11 13:01:20.270281 findontime-0.2.6/src/findontime/tables_post.py
+-rw-r--r--   0        0        0    21536 2023-04-13 13:27:24.031739 findontime-0.2.6/src/findontime/upload_utils.py
+-rw-r--r--   0        0        0    12126 2023-05-08 17:19:07.921529 findontime-0.2.6/setup.py
+-rw-r--r--   0        0        0    11799 2023-05-08 17:19:07.922579 findontime-0.2.6/PKG-INFO
```

### Comparing `findontime-0.2.5/LICENSE` & `findontime-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `findontime-0.2.5/README.md` & `findontime-0.2.6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # findONTime
 
 [![PyPI version](https://badge.fury.io/py/findontime.svg)](https://badge.fury.io/py/findontime)
 [![PyPI version](https://img.shields.io/pypi/pyversions/findontime.svg)](https://pypi.python.org/pypi/findontime/)
 [![PyPI version](https://img.shields.io/pypi/format/findontime.svg)](https://pypi.python.org/pypi/findontime/)
 
-The **findONTime** tool **runs concurrently with MinION sequencing** and **merges (at user defined time intervals) the FASTQ files** that are being generated in real-time for each sample. It can also automatically **upload the files the INSaFLU-TELEVIR platform** and launch the **metagenomics virus detection** analysis using the TELEVIR module.
+The **findONTime** tool **runs concurrently with MinION sequencing** and **merges (at user defined time intervals) the FASTQ files** that are being generated in real-time for each sample. It can also automatically **upload the files to the INSaFLU-TELEVIR platform** (https://insaflu.insa.pt/) and launch the **metagenomics virus detection** analysis using the TELEVIR module.
 
 ## Motivation
 
 Reducing the time needed for pathogen detection and the sequencing costs per sample is crucial in the context of diagnostics using metagenomics sequencing. In fact, when performing hypothesis-free viral diagnosis by sequencing complex biological samples, the proportion of the virus in a sample is unknown. As such, the amount of sequencing data, and consequently run length, needed to accurately detect the virus cannot be predicted a priori.
 
 **findONTime runs concurrently with MinION sequencing and monitors the FASTQ files that are being generated in real-time for each sample, merges the files (at user defined time intervals), uploads them to the INSaFLU-TELEVIR platform and launches the metagenomics virus detection analysis using the [TELEVIR module](https://insaflu.readthedocs.io/en/latest/metagenomics_virus_detection.html)**.
 
 This allows users to **detect a virus in a sample as early as possible during the sequencing run**, reducing the time gap between obtaining the sample and the diagnosis, and also **reducing sequencing costs** (as ONT runs can be stopped at any time and the flow cells can be cleaned and reused). **findONTime** can be used as a “start-to-end” solution or for particular tasks (e.g., merging ONT output files, metadata preparation and upload to INSaFLU-TELEVIR).
 
 ## Details
 
 - It **runs concurrently with MinION sequencing** and **merges (at user defined time intervals) the FASTQ files** that are being generated in real-time for each sample. For this, it relies on [fastq-handler](https://pypi.org/project/fastq-handler/), a package to process ONT fastq files by concatenating reads as they are generated during a sequencing run.
 
-- It can also automatically **upload the files the INSaFLU-TELEVIR platform** (docker installation or local server) and launch the **metagenomics virus detection** analysis using the TELEVIR module.
+- It can also automatically **upload the files to the INSaFLU-TELEVIR platform** (docker installation or local server) and launch the **metagenomics virus detection** analysis using the TELEVIR module.
 
 - The user has the option to upload all files collected throughout the ONT run (sampling occurs at user-defined period) or only upload the lastest file (i.e, the file compiling all reads generated until the lastest sampling point).
 
 - For upload, metadata files are also generated for each sequence file, according to the INSaFLU-TELEVIR input template file. Metadata files are stored in the metadata sub-directory following the output directory specified by the user.
 
 ### Upload reads to INSaFLU-TELEVIR
 
@@ -32,23 +32,21 @@
 
 - **SSH**. The user needs to have access to an INSaFLU-TELEVIR database server. The tool will then upload the files to the database using SSH. The user needs to provide the path for uploads and the credentials for the database server.
 
 **Note**: Automatic upload to the [INSaFLU-TELEVIR website](https://insaflu.insa.pt/) accounts is not available yet. If you only have an online account (and not a local INSaFLU installation), findONTime will be run concurrently with MinION sequencing to monitor and concatenate the FASTQ files that are being generated in real-time for each sample and prepare metadata templates ready to be upload to INSaFLU-TELEVIR.
 
 ### Launch a virus detection analysis (TELEVIR)
 
-If requested the tool creates one INSaFLU-TELEVIR project for each inpp directory containing fastq files. The project name is the name of the directory. Files generated within the same directory are uploaded to the same project.
-
-If you have a local INSaFLU-TELEVIR installation (docker or server), and set the "--televir argument", findONTtimeThe tool can creates one INSaFLU-TELEVIR (virus detection) project including the samples under ONT sequencing. The project name is defined by the user (--tag argument) and the sample names are the ones of the input directory (usually barcode01, barcode02, etc) with an extra user-defined tag as suffix.
+If you have a local INSaFLU-TELEVIR installation (docker or server), and set the "--televir argument", findONTtimeThe tool can create one INSaFLU-TELEVIR (virus detection) project including the samples under ONT sequencing. The project name is defined by the user (--tag argument) and the sample names are the ones of the input directory (usually barcode01, barcode02, etc) with an extra user-defined tag as suffix.
 
 ### Input Files
 
 - **fastq.gz** - Output directory for the ONT run, containing sequence files. The files can be in subfolders. The files can be gzipped or not.
 
-- **config.ini** - A configuration file containing the parameters for the tool. The file is generated by the tool when it is run for the first time. The user can edit the file to change the parameters.
+- **config.ini** - (needed if --upload is requested). Configuration file containing the parameters for the tool. The file is generated by the tool when it is run for the first time. The user can edit the file to change the parameters.
 
 Config must contain:
 
 - section [INSAFLU] containing insaflu username and app directory path.
 
 - (optional) section [SSH] containing ssh credentials: username, ip_address and rsa key;
```

### Comparing `findontime-0.2.5/pyproject.toml` & `findontime-0.2.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "findontime"
-version = "0.2.5"
+version = "0.2.6"
 description = "A tool to upload Fastq files to the INSaFLU database and perform metagenomics pathogen detection"
 authors = ["SantosJGND <dourado.jns@gmail.com>", "insapathogenomics <insapathogenomics@insa.min-saude.pt>"]
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `findontime-0.2.5/src/findontime/configs.py` & `findontime-0.2.6/src/findontime/configs.py`

 * *Files identical despite different names*

### Comparing `findontime-0.2.5/src/findontime/connectors.py` & `findontime-0.2.6/src/findontime/connectors.py`

 * *Files identical despite different names*

### Comparing `findontime-0.2.5/src/findontime/drones.py` & `findontime-0.2.6/src/findontime/drones.py`

 * *Files 8% similar despite different names*

```diff
@@ -89,14 +89,16 @@
         try:
 
             while not self._stopevent.is_set():
                 start_time = time.time()
                 execution_time = 0
                 self._stopevent.clear()  # Make sure the thread is unset
                 self.lock.acquire_for("B")
+                print("--------------------")
+                print("televir sleep period: {}".format(self.work_period))
 
                 while execution_time < self.work_period:
                     self.processor.run()
                     execution_time = time.time() - start_time
 
                     self.counter += 1
```

### Comparing `findontime-0.2.5/src/findontime/insaflu_uploads.py` & `findontime-0.2.6/src/findontime/insaflu_uploads.py`

 * *Files identical despite different names*

### Comparing `findontime-0.2.5/src/findontime/manager.py` & `findontime-0.2.6/src/findontime/manager.py`

 * *Files identical despite different names*

### Comparing `findontime-0.2.5/src/findontime/plot_utils.py` & `findontime-0.2.6/src/findontime/plot_utils.py`

 * *Files identical despite different names*

### Comparing `findontime-0.2.5/src/findontime/plotting_from_all_reports.py` & `findontime-0.2.6/src/findontime/plotting_from_all_reports.py`

 * *Files identical despite different names*

### Comparing `findontime-0.2.5/src/findontime/records.py` & `findontime-0.2.6/src/findontime/records.py`

 * *Files identical despite different names*

### Comparing `findontime-0.2.5/src/findontime/tables_post.py` & `findontime-0.2.6/src/findontime/tables_post.py`

 * *Files identical despite different names*

### Comparing `findontime-0.2.5/src/findontime/upload_utils.py` & `findontime-0.2.6/src/findontime/upload_utils.py`

 * *Files identical despite different names*

### Comparing `findontime-0.2.5/setup.py` & `findontime-0.2.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,17 +22,17 @@
  'xopen==1.7.0']
 
 entry_points = \
 {'console_scripts': ['findontime = findontime.__main__:main']}
 
 setup_kwargs = {
     'name': 'findontime',
-    'version': '0.2.5',
+    'version': '0.2.6',
     'description': 'A tool to upload Fastq files to the INSaFLU database and perform metagenomics pathogen detection',
-    'long_description': '# findONTime\n\n[![PyPI version](https://badge.fury.io/py/findontime.svg)](https://badge.fury.io/py/findontime)\n[![PyPI version](https://img.shields.io/pypi/pyversions/findontime.svg)](https://pypi.python.org/pypi/findontime/)\n[![PyPI version](https://img.shields.io/pypi/format/findontime.svg)](https://pypi.python.org/pypi/findontime/)\n\nThe **findONTime** tool **runs concurrently with MinION sequencing** and **merges (at user defined time intervals) the FASTQ files** that are being generated in real-time for each sample. It can also automatically **upload the files the INSaFLU-TELEVIR platform** and launch the **metagenomics virus detection** analysis using the TELEVIR module.\n\n## Motivation\n\nReducing the time needed for pathogen detection and the sequencing costs per sample is crucial in the context of diagnostics using metagenomics sequencing. In fact, when performing hypothesis-free viral diagnosis by sequencing complex biological samples, the proportion of the virus in a sample is unknown. As such, the amount of sequencing data, and consequently run length, needed to accurately detect the virus cannot be predicted a priori.\n\n**findONTime runs concurrently with MinION sequencing and monitors the FASTQ files that are being generated in real-time for each sample, merges the files (at user defined time intervals), uploads them to the INSaFLU-TELEVIR platform and launches the metagenomics virus detection analysis using the [TELEVIR module](https://insaflu.readthedocs.io/en/latest/metagenomics_virus_detection.html)**.\n\nThis allows users to **detect a virus in a sample as early as possible during the sequencing run**, reducing the time gap between obtaining the sample and the diagnosis, and also **reducing sequencing costs** (as ONT runs can be stopped at any time and the flow cells can be cleaned and reused). **findONTime** can be used as a “start-to-end” solution or for particular tasks (e.g., merging ONT output files, metadata preparation and upload to INSaFLU-TELEVIR).\n\n## Details\n\n- It **runs concurrently with MinION sequencing** and **merges (at user defined time intervals) the FASTQ files** that are being generated in real-time for each sample. For this, it relies on [fastq-handler](https://pypi.org/project/fastq-handler/), a package to process ONT fastq files by concatenating reads as they are generated during a sequencing run.\n\n- It can also automatically **upload the files the INSaFLU-TELEVIR platform** (docker installation or local server) and launch the **metagenomics virus detection** analysis using the TELEVIR module.\n\n- The user has the option to upload all files collected throughout the ONT run (sampling occurs at user-defined period) or only upload the lastest file (i.e, the file compiling all reads generated until the lastest sampling point).\n\n- For upload, metadata files are also generated for each sequence file, according to the INSaFLU-TELEVIR input template file. Metadata files are stored in the metadata sub-directory following the output directory specified by the user.\n\n### Upload reads to INSaFLU-TELEVIR\n\n_findONTime_ can interact with the INSaFLU-TELEVIR platfotm in two ways:\n\n- **Docker**. The user needs to have the INSaFLU-TELEVIR docker installed and running. The tool will then upload the files to the docker image. The user needs to provide the name of the docker image and the path for uploads.\n\n- **SSH**. The user needs to have access to an INSaFLU-TELEVIR database server. The tool will then upload the files to the database using SSH. The user needs to provide the path for uploads and the credentials for the database server.\n\n**Note**: Automatic upload to the [INSaFLU-TELEVIR website](https://insaflu.insa.pt/) accounts is not available yet. If you only have an online account (and not a local INSaFLU installation), findONTime will be run concurrently with MinION sequencing to monitor and concatenate the FASTQ files that are being generated in real-time for each sample and prepare metadata templates ready to be upload to INSaFLU-TELEVIR.\n\n### Launch a virus detection analysis (TELEVIR)\n\nIf requested the tool creates one INSaFLU-TELEVIR project for each inpp directory containing fastq files. The project name is the name of the directory. Files generated within the same directory are uploaded to the same project.\n\nIf you have a local INSaFLU-TELEVIR installation (docker or server), and set the "--televir argument", findONTtimeThe tool can creates one INSaFLU-TELEVIR (virus detection) project including the samples under ONT sequencing. The project name is defined by the user (--tag argument) and the sample names are the ones of the input directory (usually barcode01, barcode02, etc) with an extra user-defined tag as suffix.\n\n### Input Files\n\n- **fastq.gz** - Output directory for the ONT run, containing sequence files. The files can be in subfolders. The files can be gzipped or not.\n\n- **config.ini** - A configuration file containing the parameters for the tool. The file is generated by the tool when it is run for the first time. The user can edit the file to change the parameters.\n\nConfig must contain:\n\n- section [INSAFLU] containing insaflu username and app directory path.\n\n- (optional) section [SSH] containing ssh credentials: username, ip_address and rsa key;\n\n- (optional) section [DOCKER] containing docker image name.\n\nsee example [config.ini](config.ini)\n\n## API\n\n```bash\n\nusage: findontime [-h] -i IN_DIR -o OUT_DIR [-s SLEEP] [-n TAG] [--config CONFIG] [--max_size MAX_SIZE] [--merge] [--downsize] [--upload {last,all,none}] [--connect {docker,ssh}] [--keep_names] [--monitor] [--televir]\n\nProcess fastq files.\n\noptional arguments:\n  -h, --help            show this help message and exit\n  -i IN_DIR, --in_dir IN_DIR\n                        Input directory\n  -o OUT_DIR, --out_dir OUT_DIR\n                        Output directory\n  -s SLEEP, --sleep SLEEP\n                        Sleep time between checks in monitor mode (default 600 seconds)\n  -n TAG, --tag TAG     name tag, if given, will be added to the output file names\n  --config CONFIG       config file\n  --max_size MAX_SIZE   max size of the output file, in kilobytes (default 400000 kbytes)\n  --merge               merge files\n  --downsize            downsize fastq files to max_size\n  --upload {last,all,none}\n                        file upload strategy (default: last)\n  --connect {docker,ssh}\n                        file upload strategy (default: docker)\n  --keep_names          keep original file names\n  --monitor             monitor directory until killed\n  --televir             deploy televir pathogen identification on each sample\n\n```\n\n### REQUIREMENTS\n\n- **python 3.6** or higher\n- dataclasses==0.6\n- natsort==8.3.1\n- pandas==1.5.3\n- paramiko==3.1.0\n- pip==21.2.3\n- setuptools==57.4.0\n- xopen==1.7.0\n\n### INSTALLATION\n\n```bash\npython -m venv .venv\nsource .venv/bin/activate\npython -m pip install findontime\n```\n\n### USAGE\n\n_(from simple to more advanced usage situations)_\n\n- Example 1. **Merge fastq files from an ONT run.**\n\n```bash\nfindontime -i input_directory -o output_directory --tag suffix --max_size 100000000 --merge --upload none\n\n```\n\n_NOTE: In this simpler usage case, the fastq.gz files will only be only merged, i.e., they will not be automatically uploaded to the INSaFLU-TELEVIR platform. In case you want to concatenate all ONT same-sample files (file_0.fastq.gz, file_1.fastq.gz, etc), make sure you set up a "max_size" (e.g., 100000000 kbytes) enough to ensure that the merged file compiles all partial files._\n\n- Example 2. **Merge fastq files generated during a ONT run at every 10 min (600 seconds).**\n\n```bash\nfindontime -i input_directory -o output_directory --tag suffix -s 600 --max_size 100000000 --monitor --merge --upload none\n\n```\n\n_NOTE: In this simpler usage case, the fastq.gz files will only be only merged, i.e., they will not be automatically uploaded to the INSaFLU-TELEVIR platform. In case you want to concatenate all ONT same-sample files (file_0.fastq.gz, file_1.fastq.gz, etc), make sure you set up a "max_size" (e.g., 100000000 kbytes) enough to ensure that the merged file compiles all partial files._\n\n- Example 3. **Merge fastq files generated during a ONT run at every 10 min (600 seconds), downsize the merged file to 400 MB (ready to be uploaded to INSaFLU-TELEVIR).**\n\n```bash\nfindontime -i input_directory -o output_directory --tag suffix -s 600 --max_size 400000 --monitor --merge --upload none --downsize\n\n```\n\n_NOTE: In this case, the fastq.gz files will only be concatenated (i.e., they will not be automatically uploaded to the INSaFLU-TELEVIR platform), but the merged files will be downsized to the user-defined "max_sixe" (e.g., 400000 kbytes). This usage is useful to prepare files ready to be uploaded to the online [INSaFLU-TELEVIR platform](https://insaflu.insa.pt/), which is currently limited to an upload max size per file of 400 MB._\n\n- Example 4. **Merge fastq files generated during a ONT run at every 10 min (600 seconds) and upload them to INSaFLU-TELEVIR**\n\n```bash\nfindontime -i input_directory -o output_directory --tag suffix -s 600 --max_size 400000 --monitor --connect docker --merge --upload last --connect docker\n\n```\n\n_NOTE: In this case, the fastq.gz files will be concatenated and automatically uploaded to the INSaFLU-TELEVIR platform. The merged files will be downsized to the user-defined "max_sixe" (e.g., 400000 kbytes), which must be fitted to the maximum upload file size defined in your local INSaFLU_TELEVIR installation_\n\n- Example 5. **Merge fastq files generated during a ONT run at every 10 min (600 seconds), upload them to INSaFLU-TELEVIR and run a virus detection project**\n\n```bash\nfindontime -i input_directory -o output_directory --tag suffix -s 600 --max_size 400000 --monitor --connect docker --merge --upload last –-televir\n\n```\n\n_NOTE: In this case, the fastq.gz files will be concatenated, automatically uploaded to the INSaFLU-TELEVIR platform and run under a virus detection (TELEVIR) project. The merged files will be downsized to the user-defined "max_sixe" (e.g., 400000 kbytes), which must be fitted to the maximum upload file size defined in your local INSaFLU_TELEVIR installation_\n\n### TESTING\n\nRunning pytest in the root directory will run all tests that do not interact with INSaFLU-TELEVIR. In order to test the upload and metagenomics functionalities, the user needs to provide a valid config file to a local docker installation, and to pass the `--docker` flag to pytest:\n\n```bash\n\npytest --docker --config-file config.ini\n\n```\n\n### MAIN OUTPUT\n\n> **Note:** The output directory structure is maintained.\n\n- **fastq.gz** files containing all reads from the previous files.\n- **log.txt** file containing the concatenation process.\n- **metadata** individual metadata files for each fastq file uploaded.\n- **results.tsv** file containing the main results of the TELEVIR pathogen detection. One file per project.\n\n## Maintainers\n\n- [**@santosjgnd**](https://github.com/SantosJGND)\n- [**@insaflu**](https://github.com/insapathogenomics)\n',
+    'long_description': '# findONTime\n\n[![PyPI version](https://badge.fury.io/py/findontime.svg)](https://badge.fury.io/py/findontime)\n[![PyPI version](https://img.shields.io/pypi/pyversions/findontime.svg)](https://pypi.python.org/pypi/findontime/)\n[![PyPI version](https://img.shields.io/pypi/format/findontime.svg)](https://pypi.python.org/pypi/findontime/)\n\nThe **findONTime** tool **runs concurrently with MinION sequencing** and **merges (at user defined time intervals) the FASTQ files** that are being generated in real-time for each sample. It can also automatically **upload the files to the INSaFLU-TELEVIR platform** (https://insaflu.insa.pt/) and launch the **metagenomics virus detection** analysis using the TELEVIR module.\n\n## Motivation\n\nReducing the time needed for pathogen detection and the sequencing costs per sample is crucial in the context of diagnostics using metagenomics sequencing. In fact, when performing hypothesis-free viral diagnosis by sequencing complex biological samples, the proportion of the virus in a sample is unknown. As such, the amount of sequencing data, and consequently run length, needed to accurately detect the virus cannot be predicted a priori.\n\n**findONTime runs concurrently with MinION sequencing and monitors the FASTQ files that are being generated in real-time for each sample, merges the files (at user defined time intervals), uploads them to the INSaFLU-TELEVIR platform and launches the metagenomics virus detection analysis using the [TELEVIR module](https://insaflu.readthedocs.io/en/latest/metagenomics_virus_detection.html)**.\n\nThis allows users to **detect a virus in a sample as early as possible during the sequencing run**, reducing the time gap between obtaining the sample and the diagnosis, and also **reducing sequencing costs** (as ONT runs can be stopped at any time and the flow cells can be cleaned and reused). **findONTime** can be used as a “start-to-end” solution or for particular tasks (e.g., merging ONT output files, metadata preparation and upload to INSaFLU-TELEVIR).\n\n## Details\n\n- It **runs concurrently with MinION sequencing** and **merges (at user defined time intervals) the FASTQ files** that are being generated in real-time for each sample. For this, it relies on [fastq-handler](https://pypi.org/project/fastq-handler/), a package to process ONT fastq files by concatenating reads as they are generated during a sequencing run.\n\n- It can also automatically **upload the files to the INSaFLU-TELEVIR platform** (docker installation or local server) and launch the **metagenomics virus detection** analysis using the TELEVIR module.\n\n- The user has the option to upload all files collected throughout the ONT run (sampling occurs at user-defined period) or only upload the lastest file (i.e, the file compiling all reads generated until the lastest sampling point).\n\n- For upload, metadata files are also generated for each sequence file, according to the INSaFLU-TELEVIR input template file. Metadata files are stored in the metadata sub-directory following the output directory specified by the user.\n\n### Upload reads to INSaFLU-TELEVIR\n\n_findONTime_ can interact with the INSaFLU-TELEVIR platfotm in two ways:\n\n- **Docker**. The user needs to have the INSaFLU-TELEVIR docker installed and running. The tool will then upload the files to the docker image. The user needs to provide the name of the docker image and the path for uploads.\n\n- **SSH**. The user needs to have access to an INSaFLU-TELEVIR database server. The tool will then upload the files to the database using SSH. The user needs to provide the path for uploads and the credentials for the database server.\n\n**Note**: Automatic upload to the [INSaFLU-TELEVIR website](https://insaflu.insa.pt/) accounts is not available yet. If you only have an online account (and not a local INSaFLU installation), findONTime will be run concurrently with MinION sequencing to monitor and concatenate the FASTQ files that are being generated in real-time for each sample and prepare metadata templates ready to be upload to INSaFLU-TELEVIR.\n\n### Launch a virus detection analysis (TELEVIR)\n\nIf you have a local INSaFLU-TELEVIR installation (docker or server), and set the "--televir argument", findONTtimeThe tool can create one INSaFLU-TELEVIR (virus detection) project including the samples under ONT sequencing. The project name is defined by the user (--tag argument) and the sample names are the ones of the input directory (usually barcode01, barcode02, etc) with an extra user-defined tag as suffix.\n\n### Input Files\n\n- **fastq.gz** - Output directory for the ONT run, containing sequence files. The files can be in subfolders. The files can be gzipped or not.\n\n- **config.ini** - (needed if --upload is requested). Configuration file containing the parameters for the tool. The file is generated by the tool when it is run for the first time. The user can edit the file to change the parameters.\n\nConfig must contain:\n\n- section [INSAFLU] containing insaflu username and app directory path.\n\n- (optional) section [SSH] containing ssh credentials: username, ip_address and rsa key;\n\n- (optional) section [DOCKER] containing docker image name.\n\nsee example [config.ini](config.ini)\n\n## API\n\n```bash\n\nusage: findontime [-h] -i IN_DIR -o OUT_DIR [-s SLEEP] [-n TAG] [--config CONFIG] [--max_size MAX_SIZE] [--merge] [--downsize] [--upload {last,all,none}] [--connect {docker,ssh}] [--keep_names] [--monitor] [--televir]\n\nProcess fastq files.\n\noptional arguments:\n  -h, --help            show this help message and exit\n  -i IN_DIR, --in_dir IN_DIR\n                        Input directory\n  -o OUT_DIR, --out_dir OUT_DIR\n                        Output directory\n  -s SLEEP, --sleep SLEEP\n                        Sleep time between checks in monitor mode (default 600 seconds)\n  -n TAG, --tag TAG     name tag, if given, will be added to the output file names\n  --config CONFIG       config file\n  --max_size MAX_SIZE   max size of the output file, in kilobytes (default 400000 kbytes)\n  --merge               merge files\n  --downsize            downsize fastq files to max_size\n  --upload {last,all,none}\n                        file upload strategy (default: last)\n  --connect {docker,ssh}\n                        file upload strategy (default: docker)\n  --keep_names          keep original file names\n  --monitor             monitor directory until killed\n  --televir             deploy televir pathogen identification on each sample\n\n```\n\n### REQUIREMENTS\n\n- **python 3.6** or higher\n- dataclasses==0.6\n- natsort==8.3.1\n- pandas==1.5.3\n- paramiko==3.1.0\n- pip==21.2.3\n- setuptools==57.4.0\n- xopen==1.7.0\n\n### INSTALLATION\n\n```bash\npython -m venv .venv\nsource .venv/bin/activate\npython -m pip install findontime\n```\n\n### USAGE\n\n_(from simple to more advanced usage situations)_\n\n- Example 1. **Merge fastq files from an ONT run.**\n\n```bash\nfindontime -i input_directory -o output_directory --tag suffix --max_size 100000000 --merge --upload none\n\n```\n\n_NOTE: In this simpler usage case, the fastq.gz files will only be only merged, i.e., they will not be automatically uploaded to the INSaFLU-TELEVIR platform. In case you want to concatenate all ONT same-sample files (file_0.fastq.gz, file_1.fastq.gz, etc), make sure you set up a "max_size" (e.g., 100000000 kbytes) enough to ensure that the merged file compiles all partial files._\n\n- Example 2. **Merge fastq files generated during a ONT run at every 10 min (600 seconds).**\n\n```bash\nfindontime -i input_directory -o output_directory --tag suffix -s 600 --max_size 100000000 --monitor --merge --upload none\n\n```\n\n_NOTE: In this simpler usage case, the fastq.gz files will only be only merged, i.e., they will not be automatically uploaded to the INSaFLU-TELEVIR platform. In case you want to concatenate all ONT same-sample files (file_0.fastq.gz, file_1.fastq.gz, etc), make sure you set up a "max_size" (e.g., 100000000 kbytes) enough to ensure that the merged file compiles all partial files._\n\n- Example 3. **Merge fastq files generated during a ONT run at every 10 min (600 seconds), downsize the merged file to 400 MB (ready to be uploaded to INSaFLU-TELEVIR).**\n\n```bash\nfindontime -i input_directory -o output_directory --tag suffix -s 600 --max_size 400000 --monitor --merge --upload none --downsize\n\n```\n\n_NOTE: In this case, the fastq.gz files will only be concatenated (i.e., they will not be automatically uploaded to the INSaFLU-TELEVIR platform), but the merged files will be downsized to the user-defined "max_sixe" (e.g., 400000 kbytes). This usage is useful to prepare files ready to be uploaded to the online [INSaFLU-TELEVIR platform](https://insaflu.insa.pt/), which is currently limited to an upload max size per file of 400 MB._\n\n- Example 4. **Merge fastq files generated during a ONT run at every 10 min (600 seconds) and upload them to INSaFLU-TELEVIR**\n\n```bash\nfindontime -i input_directory -o output_directory --tag suffix -s 600 --max_size 400000 --monitor --connect docker --merge --upload last --connect docker\n\n```\n\n_NOTE: In this case, the fastq.gz files will be concatenated and automatically uploaded to the INSaFLU-TELEVIR platform. The merged files will be downsized to the user-defined "max_sixe" (e.g., 400000 kbytes), which must be fitted to the maximum upload file size defined in your local INSaFLU_TELEVIR installation_\n\n- Example 5. **Merge fastq files generated during a ONT run at every 10 min (600 seconds), upload them to INSaFLU-TELEVIR and run a virus detection project**\n\n```bash\nfindontime -i input_directory -o output_directory --tag suffix -s 600 --max_size 400000 --monitor --connect docker --merge --upload last –-televir\n\n```\n\n_NOTE: In this case, the fastq.gz files will be concatenated, automatically uploaded to the INSaFLU-TELEVIR platform and run under a virus detection (TELEVIR) project. The merged files will be downsized to the user-defined "max_sixe" (e.g., 400000 kbytes), which must be fitted to the maximum upload file size defined in your local INSaFLU_TELEVIR installation_\n\n### TESTING\n\nRunning pytest in the root directory will run all tests that do not interact with INSaFLU-TELEVIR. In order to test the upload and metagenomics functionalities, the user needs to provide a valid config file to a local docker installation, and to pass the `--docker` flag to pytest:\n\n```bash\n\npytest --docker --config-file config.ini\n\n```\n\n### MAIN OUTPUT\n\n> **Note:** The output directory structure is maintained.\n\n- **fastq.gz** files containing all reads from the previous files.\n- **log.txt** file containing the concatenation process.\n- **metadata** individual metadata files for each fastq file uploaded.\n- **results.tsv** file containing the main results of the TELEVIR pathogen detection. One file per project.\n\n## Maintainers\n\n- [**@santosjgnd**](https://github.com/SantosJGND)\n- [**@insaflu**](https://github.com/insapathogenomics)\n',
     'author': 'SantosJGND',
     'author_email': 'dourado.jns@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `findontime-0.2.5/PKG-INFO` & `findontime-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: findontime
-Version: 0.2.5
+Version: 0.2.6
 Summary: A tool to upload Fastq files to the INSaFLU database and perform metagenomics pathogen detection
 License: MIT
 Author: SantosJGND
 Author-email: dourado.jns@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -24,29 +24,29 @@
 
 # findONTime
 
 [![PyPI version](https://badge.fury.io/py/findontime.svg)](https://badge.fury.io/py/findontime)
 [![PyPI version](https://img.shields.io/pypi/pyversions/findontime.svg)](https://pypi.python.org/pypi/findontime/)
 [![PyPI version](https://img.shields.io/pypi/format/findontime.svg)](https://pypi.python.org/pypi/findontime/)
 
-The **findONTime** tool **runs concurrently with MinION sequencing** and **merges (at user defined time intervals) the FASTQ files** that are being generated in real-time for each sample. It can also automatically **upload the files the INSaFLU-TELEVIR platform** and launch the **metagenomics virus detection** analysis using the TELEVIR module.
+The **findONTime** tool **runs concurrently with MinION sequencing** and **merges (at user defined time intervals) the FASTQ files** that are being generated in real-time for each sample. It can also automatically **upload the files to the INSaFLU-TELEVIR platform** (https://insaflu.insa.pt/) and launch the **metagenomics virus detection** analysis using the TELEVIR module.
 
 ## Motivation
 
 Reducing the time needed for pathogen detection and the sequencing costs per sample is crucial in the context of diagnostics using metagenomics sequencing. In fact, when performing hypothesis-free viral diagnosis by sequencing complex biological samples, the proportion of the virus in a sample is unknown. As such, the amount of sequencing data, and consequently run length, needed to accurately detect the virus cannot be predicted a priori.
 
 **findONTime runs concurrently with MinION sequencing and monitors the FASTQ files that are being generated in real-time for each sample, merges the files (at user defined time intervals), uploads them to the INSaFLU-TELEVIR platform and launches the metagenomics virus detection analysis using the [TELEVIR module](https://insaflu.readthedocs.io/en/latest/metagenomics_virus_detection.html)**.
 
 This allows users to **detect a virus in a sample as early as possible during the sequencing run**, reducing the time gap between obtaining the sample and the diagnosis, and also **reducing sequencing costs** (as ONT runs can be stopped at any time and the flow cells can be cleaned and reused). **findONTime** can be used as a “start-to-end” solution or for particular tasks (e.g., merging ONT output files, metadata preparation and upload to INSaFLU-TELEVIR).
 
 ## Details
 
 - It **runs concurrently with MinION sequencing** and **merges (at user defined time intervals) the FASTQ files** that are being generated in real-time for each sample. For this, it relies on [fastq-handler](https://pypi.org/project/fastq-handler/), a package to process ONT fastq files by concatenating reads as they are generated during a sequencing run.
 
-- It can also automatically **upload the files the INSaFLU-TELEVIR platform** (docker installation or local server) and launch the **metagenomics virus detection** analysis using the TELEVIR module.
+- It can also automatically **upload the files to the INSaFLU-TELEVIR platform** (docker installation or local server) and launch the **metagenomics virus detection** analysis using the TELEVIR module.
 
 - The user has the option to upload all files collected throughout the ONT run (sampling occurs at user-defined period) or only upload the lastest file (i.e, the file compiling all reads generated until the lastest sampling point).
 
 - For upload, metadata files are also generated for each sequence file, according to the INSaFLU-TELEVIR input template file. Metadata files are stored in the metadata sub-directory following the output directory specified by the user.
 
 ### Upload reads to INSaFLU-TELEVIR
 
@@ -56,23 +56,21 @@
 
 - **SSH**. The user needs to have access to an INSaFLU-TELEVIR database server. The tool will then upload the files to the database using SSH. The user needs to provide the path for uploads and the credentials for the database server.
 
 **Note**: Automatic upload to the [INSaFLU-TELEVIR website](https://insaflu.insa.pt/) accounts is not available yet. If you only have an online account (and not a local INSaFLU installation), findONTime will be run concurrently with MinION sequencing to monitor and concatenate the FASTQ files that are being generated in real-time for each sample and prepare metadata templates ready to be upload to INSaFLU-TELEVIR.
 
 ### Launch a virus detection analysis (TELEVIR)
 
-If requested the tool creates one INSaFLU-TELEVIR project for each inpp directory containing fastq files. The project name is the name of the directory. Files generated within the same directory are uploaded to the same project.
-
-If you have a local INSaFLU-TELEVIR installation (docker or server), and set the "--televir argument", findONTtimeThe tool can creates one INSaFLU-TELEVIR (virus detection) project including the samples under ONT sequencing. The project name is defined by the user (--tag argument) and the sample names are the ones of the input directory (usually barcode01, barcode02, etc) with an extra user-defined tag as suffix.
+If you have a local INSaFLU-TELEVIR installation (docker or server), and set the "--televir argument", findONTtimeThe tool can create one INSaFLU-TELEVIR (virus detection) project including the samples under ONT sequencing. The project name is defined by the user (--tag argument) and the sample names are the ones of the input directory (usually barcode01, barcode02, etc) with an extra user-defined tag as suffix.
 
 ### Input Files
 
 - **fastq.gz** - Output directory for the ONT run, containing sequence files. The files can be in subfolders. The files can be gzipped or not.
 
-- **config.ini** - A configuration file containing the parameters for the tool. The file is generated by the tool when it is run for the first time. The user can edit the file to change the parameters.
+- **config.ini** - (needed if --upload is requested). Configuration file containing the parameters for the tool. The file is generated by the tool when it is run for the first time. The user can edit the file to change the parameters.
 
 Config must contain:
 
 - section [INSAFLU] containing insaflu username and app directory path.
 
 - (optional) section [SSH] containing ssh credentials: username, ip_address and rsa key;
```

