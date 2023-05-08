# Comparing `tmp/parallel_bilby-2.0.1.tar.gz` & `tmp/parallel_bilby-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parallel_bilby-2.0.1.tar", last modified: Tue Mar 21 02:06:04 2023, max compression
+gzip compressed data, was "parallel_bilby-2.0.2.tar", last modified: Mon May  8 02:02:56 2023, max compression
```

## Comparing `parallel_bilby-2.0.1.tar` & `parallel_bilby-2.0.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-21 02:06:04.418522 parallel_bilby-2.0.1/
--rw-rw-rw-   0 root         (0) root         (0)     1066 2023-03-21 02:05:42.000000 parallel_bilby-2.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1885 2023-03-21 02:06:04.418522 parallel_bilby-2.0.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1375 2023-03-21 02:05:42.000000 parallel_bilby-2.0.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-21 02:06:04.414522 parallel_bilby-2.0.1/parallel_bilby/
--rw-r--r--   0 root         (0) root         (0)       54 2023-03-21 02:06:04.000000 parallel_bilby-2.0.1/parallel_bilby/.version
--rw-rw-rw-   0 root         (0) root         (0)       67 2023-03-21 02:05:42.000000 parallel_bilby-2.0.1/parallel_bilby/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-21 02:06:04.416522 parallel_bilby-2.0.1/parallel_bilby/analysis/
--rw-rw-rw-   0 root         (0) root         (0)      124 2023-03-21 02:05:42.000000 parallel_bilby-2.0.1/parallel_bilby/analysis/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13730 2023-03-21 02:05:42.000000 parallel_bilby-2.0.1/parallel_bilby/analysis/analysis_run.py
--rw-rw-rw-   0 root         (0) root         (0)     5653 2023-03-21 02:05:42.000000 parallel_bilby-2.0.1/parallel_bilby/analysis/likelihood.py
--rw-rw-rw-   0 root         (0) root         (0)    11107 2023-03-21 02:05:42.000000 parallel_bilby-2.0.1/parallel_bilby/analysis/main.py
--rw-rw-rw-   0 root         (0) root         (0)     1635 2023-03-21 02:05:42.000000 parallel_bilby-2.0.1/parallel_bilby/analysis/plotting.py
--rw-rw-rw-   0 root         (0) root         (0)     7493 2023-03-21 02:05:42.000000 parallel_bilby-2.0.1/parallel_bilby/analysis/read_write.py
--rw-rw-rw-   0 root         (0) root         (0)     1074 2023-03-21 02:05:42.000000 parallel_bilby-2.0.1/parallel_bilby/analysis/sample_space.py
--rw-rw-rw-   0 root         (0) root         (0)     6531 2023-03-21 02:05:42.000000 parallel_bilby-2.0.1/parallel_bilby/generation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-21 02:06:04.417522 parallel_bilby-2.0.1/parallel_bilby/parser/
--rw-rw-rw-   0 root         (0) root         (0)      138 2023-03-21 02:05:42.000000 parallel_bilby-2.0.1/parallel_bilby/parser/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1296 2023-03-21 02:05:42.000000 parallel_bilby-2.0.1/parallel_bilby/parser/analysis.py
--rw-rw-rw-   0 root         (0) root         (0)     4755 2023-03-21 02:05:42.000000 parallel_bilby-2.0.1/parallel_bilby/parser/generation.py
--rw-rw-rw-   0 root         (0) root         (0)     6834 2023-03-21 02:05:42.000000 parallel_bilby-2.0.1/parallel_bilby/parser/shared.py
--rw-rw-rw-   0 root         (0) root         (0)    13643 2023-03-21 02:05:42.000000 parallel_bilby-2.0.1/parallel_bilby/schwimmbad_fast.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-21 02:06:04.418522 parallel_bilby-2.0.1/parallel_bilby/slurm/
--rw-rw-rw-   0 root         (0) root         (0)       32 2023-03-21 02:05:42.000000 parallel_bilby-2.0.1/parallel_bilby/slurm/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6688 2023-03-21 02:05:42.000000 parallel_bilby-2.0.1/parallel_bilby/slurm/slurm.py
--rw-rw-rw-   0 root         (0) root         (0)      227 2023-03-21 02:05:42.000000 parallel_bilby-2.0.1/parallel_bilby/slurm/template_slurm.sh
--rw-rw-rw-   0 root         (0) root         (0)     2045 2023-03-21 02:05:42.000000 parallel_bilby-2.0.1/parallel_bilby/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-21 02:06:04.415522 parallel_bilby-2.0.1/parallel_bilby.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1885 2023-03-21 02:06:04.000000 parallel_bilby-2.0.1/parallel_bilby.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      974 2023-03-21 02:06:04.000000 parallel_bilby-2.0.1/parallel_bilby.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-21 02:06:04.000000 parallel_bilby-2.0.1/parallel_bilby.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      132 2023-03-21 02:06:04.000000 parallel_bilby-2.0.1/parallel_bilby.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      288 2023-03-21 02:06:04.000000 parallel_bilby-2.0.1/parallel_bilby.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-03-21 02:06:04.000000 parallel_bilby-2.0.1/parallel_bilby.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      538 2023-03-21 02:06:04.419522 parallel_bilby-2.0.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     3989 2023-03-21 02:05:42.000000 parallel_bilby-2.0.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-21 02:06:04.418522 parallel_bilby-2.0.1/tests/
--rw-rw-rw-   0 root         (0) root         (0)     5096 2023-03-21 02:05:42.000000 parallel_bilby-2.0.1/tests/test_generation.py
--rw-rw-rw-   0 root         (0) root         (0)     7028 2023-03-21 02:05:42.000000 parallel_bilby-2.0.1/tests/test_parser.py
--rw-rw-rw-   0 root         (0) root         (0)     2569 2023-03-21 02:05:42.000000 parallel_bilby-2.0.1/tests/test_schwimmbad.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 02:02:56.401964 parallel_bilby-2.0.2/
+-rw-rw-rw-   0 root         (0) root         (0)     1066 2023-05-08 02:02:38.000000 parallel_bilby-2.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1885 2023-05-08 02:02:56.401964 parallel_bilby-2.0.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1375 2023-05-08 02:02:38.000000 parallel_bilby-2.0.2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 02:02:56.396964 parallel_bilby-2.0.2/parallel_bilby/
+-rw-r--r--   0 root         (0) root         (0)       54 2023-05-08 02:02:56.000000 parallel_bilby-2.0.2/parallel_bilby/.version
+-rw-rw-rw-   0 root         (0) root         (0)       67 2023-05-08 02:02:38.000000 parallel_bilby-2.0.2/parallel_bilby/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 02:02:56.399964 parallel_bilby-2.0.2/parallel_bilby/analysis/
+-rw-rw-rw-   0 root         (0) root         (0)      124 2023-05-08 02:02:38.000000 parallel_bilby-2.0.2/parallel_bilby/analysis/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13730 2023-05-08 02:02:38.000000 parallel_bilby-2.0.2/parallel_bilby/analysis/analysis_run.py
+-rw-rw-rw-   0 root         (0) root         (0)     5653 2023-05-08 02:02:38.000000 parallel_bilby-2.0.2/parallel_bilby/analysis/likelihood.py
+-rw-rw-rw-   0 root         (0) root         (0)    11400 2023-05-08 02:02:38.000000 parallel_bilby-2.0.2/parallel_bilby/analysis/main.py
+-rw-rw-rw-   0 root         (0) root         (0)     1635 2023-05-08 02:02:38.000000 parallel_bilby-2.0.2/parallel_bilby/analysis/plotting.py
+-rw-rw-rw-   0 root         (0) root         (0)     7551 2023-05-08 02:02:38.000000 parallel_bilby-2.0.2/parallel_bilby/analysis/read_write.py
+-rw-rw-rw-   0 root         (0) root         (0)     1074 2023-05-08 02:02:38.000000 parallel_bilby-2.0.2/parallel_bilby/analysis/sample_space.py
+-rw-rw-rw-   0 root         (0) root         (0)     6531 2023-05-08 02:02:38.000000 parallel_bilby-2.0.2/parallel_bilby/generation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 02:02:56.400964 parallel_bilby-2.0.2/parallel_bilby/parser/
+-rw-rw-rw-   0 root         (0) root         (0)      138 2023-05-08 02:02:38.000000 parallel_bilby-2.0.2/parallel_bilby/parser/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1296 2023-05-08 02:02:38.000000 parallel_bilby-2.0.2/parallel_bilby/parser/analysis.py
+-rw-rw-rw-   0 root         (0) root         (0)     4755 2023-05-08 02:02:38.000000 parallel_bilby-2.0.2/parallel_bilby/parser/generation.py
+-rw-rw-rw-   0 root         (0) root         (0)     6834 2023-05-08 02:02:38.000000 parallel_bilby-2.0.2/parallel_bilby/parser/shared.py
+-rw-rw-rw-   0 root         (0) root         (0)    13643 2023-05-08 02:02:38.000000 parallel_bilby-2.0.2/parallel_bilby/schwimmbad_fast.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 02:02:56.400964 parallel_bilby-2.0.2/parallel_bilby/slurm/
+-rw-rw-rw-   0 root         (0) root         (0)       32 2023-05-08 02:02:38.000000 parallel_bilby-2.0.2/parallel_bilby/slurm/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6744 2023-05-08 02:02:38.000000 parallel_bilby-2.0.2/parallel_bilby/slurm/slurm.py
+-rw-rw-rw-   0 root         (0) root         (0)      227 2023-05-08 02:02:38.000000 parallel_bilby-2.0.2/parallel_bilby/slurm/template_slurm.sh
+-rw-rw-rw-   0 root         (0) root         (0)     2045 2023-05-08 02:02:38.000000 parallel_bilby-2.0.2/parallel_bilby/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 02:02:56.397964 parallel_bilby-2.0.2/parallel_bilby.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1885 2023-05-08 02:02:56.000000 parallel_bilby-2.0.2/parallel_bilby.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      974 2023-05-08 02:02:56.000000 parallel_bilby-2.0.2/parallel_bilby.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-08 02:02:56.000000 parallel_bilby-2.0.2/parallel_bilby.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      132 2023-05-08 02:02:56.000000 parallel_bilby-2.0.2/parallel_bilby.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      288 2023-05-08 02:02:56.000000 parallel_bilby-2.0.2/parallel_bilby.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-05-08 02:02:56.000000 parallel_bilby-2.0.2/parallel_bilby.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      538 2023-05-08 02:02:56.402964 parallel_bilby-2.0.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     3989 2023-05-08 02:02:38.000000 parallel_bilby-2.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 02:02:56.401964 parallel_bilby-2.0.2/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     5096 2023-05-08 02:02:39.000000 parallel_bilby-2.0.2/tests/test_generation.py
+-rw-rw-rw-   0 root         (0) root         (0)     7028 2023-05-08 02:02:39.000000 parallel_bilby-2.0.2/tests/test_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     2569 2023-05-08 02:02:39.000000 parallel_bilby-2.0.2/tests/test_schwimmbad.py
```

### Comparing `parallel_bilby-2.0.1/LICENSE` & `parallel_bilby-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `parallel_bilby-2.0.1/PKG-INFO` & `parallel_bilby-2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parallel_bilby
-Version: 2.0.1
+Version: 2.0.2
 Summary: Running bilby on GW data with MPI
 Home-page: https://git.ligo.org/lscsoft/parallel_bilby
 Author: pBilby Developers
 Author-email: gregory.ashton@ligo.org
 License: MIT
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `parallel_bilby-2.0.1/README.rst` & `parallel_bilby-2.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `parallel_bilby-2.0.1/parallel_bilby/analysis/analysis_run.py` & `parallel_bilby-2.0.2/parallel_bilby/analysis/analysis_run.py`

 * *Files identical despite different names*

### Comparing `parallel_bilby-2.0.1/parallel_bilby/analysis/likelihood.py` & `parallel_bilby-2.0.2/parallel_bilby/analysis/likelihood.py`

 * *Files identical despite different names*

### Comparing `parallel_bilby-2.0.1/parallel_bilby/analysis/main.py` & `parallel_bilby-2.0.2/parallel_bilby/analysis/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -288,21 +288,25 @@
                     if getattr(run.likelihood, f"{par}_marginalization", False):
                         run.priors[name] = run.likelihood.priors[name]
                 result.priors = run.priors
 
                 result.posterior = result.posterior.applymap(
                     lambda x: x[0] if isinstance(x, list) else x
                 )
+                result.posterior = result.posterior.select_dtypes([np.number])
                 logger.info(
                     f"Saving result to {run.outdir}/{run.label}_result.{result_format}"
                 )
+                if result_format != "json":  # json is saved by default
+                    result.save_to_file(extension="json")
                 result.save_to_file(extension=result_format)
                 print(
                     f"Sampling time = {datetime.timedelta(seconds=result.sampling_time)}s"
                 )
+                print(f"Number of lnl calls = {result.num_likelihood_evaluations}")
                 print(result)
                 if no_plot is False:
                     result.plot_corner()
 
         else:
             exit_reason = -1
         return exit_reason
```

### Comparing `parallel_bilby-2.0.1/parallel_bilby/analysis/plotting.py` & `parallel_bilby-2.0.2/parallel_bilby/analysis/plotting.py`

 * *Files identical despite different names*

### Comparing `parallel_bilby-2.0.1/parallel_bilby/analysis/read_write.py` & `parallel_bilby-2.0.2/parallel_bilby/analysis/read_write.py`

 * *Files 0% similar despite different names*

```diff
@@ -218,10 +218,11 @@
         logger.info("Resampling nested samples to posterior samples in place.")
 
     result.log_evidence = out.logz[-1] + run.likelihood.noise_log_likelihood()
     result.log_evidence_err = out.logzerr[-1]
     result.log_noise_evidence = run.likelihood.noise_log_likelihood()
     result.log_bayes_factor = result.log_evidence - result.log_noise_evidence
     result.sampling_time = sampling_time
+    result.num_likelihood_evaluations = np.sum(out.ncall)
 
     result.samples_to_posterior(likelihood=run.likelihood, priors=result.priors)
     return result
```

### Comparing `parallel_bilby-2.0.1/parallel_bilby/analysis/sample_space.py` & `parallel_bilby-2.0.2/parallel_bilby/analysis/sample_space.py`

 * *Files identical despite different names*

### Comparing `parallel_bilby-2.0.1/parallel_bilby/generation.py` & `parallel_bilby-2.0.2/parallel_bilby/generation.py`

 * *Files identical despite different names*

### Comparing `parallel_bilby-2.0.1/parallel_bilby/parser/analysis.py` & `parallel_bilby-2.0.2/parallel_bilby/parser/analysis.py`

 * *Files identical despite different names*

### Comparing `parallel_bilby-2.0.1/parallel_bilby/parser/generation.py` & `parallel_bilby-2.0.2/parallel_bilby/parser/generation.py`

 * *Files identical despite different names*

### Comparing `parallel_bilby-2.0.1/parallel_bilby/parser/shared.py` & `parallel_bilby-2.0.2/parallel_bilby/parser/shared.py`

 * *Files identical despite different names*

### Comparing `parallel_bilby-2.0.1/parallel_bilby/schwimmbad_fast.py` & `parallel_bilby-2.0.2/parallel_bilby/schwimmbad_fast.py`

 * *Files identical despite different names*

### Comparing `parallel_bilby-2.0.1/parallel_bilby/slurm/slurm.py` & `parallel_bilby-2.0.2/parallel_bilby/slurm/slurm.py`

 * *Files 2% similar despite different names*

```diff
@@ -185,9 +185,10 @@
 
     def get_contents(self):
         command = []
         command.append(f"bilby_result -r {self.file_list}")
         command.append("--merge")
         command.append(f"--label {self.merged_result_label}")
         command.append(f"--outdir {self.inputs.result_directory}")
+        command.append(f"-e {self.args.result_format}")
         command = " ".join(command)
         return super().get_contents(command=command)
```

### Comparing `parallel_bilby-2.0.1/parallel_bilby/utils.py` & `parallel_bilby-2.0.2/parallel_bilby/utils.py`

 * *Files identical despite different names*

### Comparing `parallel_bilby-2.0.1/parallel_bilby.egg-info/PKG-INFO` & `parallel_bilby-2.0.2/parallel_bilby.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parallel-bilby
-Version: 2.0.1
+Version: 2.0.2
 Summary: Running bilby on GW data with MPI
 Home-page: https://git.ligo.org/lscsoft/parallel_bilby
 Author: pBilby Developers
 Author-email: gregory.ashton@ligo.org
 License: MIT
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `parallel_bilby-2.0.1/parallel_bilby.egg-info/SOURCES.txt` & `parallel_bilby-2.0.2/parallel_bilby.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `parallel_bilby-2.0.1/setup.cfg` & `parallel_bilby-2.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `parallel_bilby-2.0.1/setup.py` & `parallel_bilby-2.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     """Finds the README and reads in the description"""
     here = os.path.abspath(os.path.dirname(__file__))
     with open(os.path.join(here, "README.rst")) as f:
         long_description = f.read()
     return long_description
 
 
-VERSION = "2.0.1"
+VERSION = "2.0.2"
 version_file = write_version_file(VERSION)
 long_description = get_long_description()
 
 setup(
     name="parallel_bilby",
     description="Running bilby on GW data with MPI",
     long_description=long_description,
```

### Comparing `parallel_bilby-2.0.1/tests/test_generation.py` & `parallel_bilby-2.0.2/tests/test_generation.py`

 * *Files identical despite different names*

### Comparing `parallel_bilby-2.0.1/tests/test_parser.py` & `parallel_bilby-2.0.2/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `parallel_bilby-2.0.1/tests/test_schwimmbad.py` & `parallel_bilby-2.0.2/tests/test_schwimmbad.py`

 * *Files identical despite different names*

