# Comparing `tmp/pycomex-0.9.3.tar.gz` & `tmp/pycomex-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycomex-0.9.3.tar", max compression
+gzip compressed data, was "pycomex-0.9.4.tar", max compression
```

## Comparing `pycomex-0.9.3.tar` & `pycomex-0.9.4.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rwxr-xr-x   0        0        0     1071 2022-07-09 08:06:36.748802 pycomex-0.9.3/LICENSE
--rwxr-xr-x   0        0        0     8890 2023-04-27 14:30:13.471269 pycomex-0.9.3/README.rst
--rwxr-xr-x   0        0        0        6 2023-05-05 13:03:19.243057 pycomex-0.9.3/pycomex/VERSION
--rwxr-xr-x   0        0        0      178 2023-05-05 13:03:19.243057 pycomex-0.9.3/pycomex/__init__.py
--rwxr-xr-x   0        0        0        0 2022-08-20 17:22:07.854881 pycomex-0.9.3/pycomex/app/__init__.py
--rwxr-xr-x   0        0        0     7375 2023-01-03 06:49:42.464925 pycomex-0.9.3/pycomex/cli.py
--rwxr-xr-x   0        0        0     2723 2023-04-28 09:23:59.597325 pycomex-0.9.3/pycomex/examples/001_quickstart.py
--rwxr-xr-x   0        0        0     3514 2023-04-28 09:16:39.398304 pycomex-0.9.3/pycomex/examples/002_basic.py
--rwxr-xr-x   0        0        0     3920 2023-04-28 09:23:59.589325 pycomex-0.9.3/pycomex/examples/003_analysing.py
--rwxr-xr-x   0        0        0     3947 2023-04-28 09:52:25.866646 pycomex-0.9.3/pycomex/examples/004_inheritance.py
--rwxr-xr-x   0        0        0      915 2023-04-28 09:23:35.509077 pycomex-0.9.3/pycomex/examples/README.rst
--rwxr-xr-x   0        0        0     3920 2023-04-28 11:45:05.200585 pycomex-0.9.3/pycomex/examples/results/004_inheritance/28_04_2023__13_45__bTbc/003_analysing.py
--rw-r--r--   0        0        0     3822 2023-04-28 11:45:05.472587 pycomex-0.9.3/pycomex/examples/results/004_inheritance/28_04_2023__13_45__bTbc/00_random.txt
--rw-r--r--   0        0        0     3747 2023-04-28 11:45:05.472587 pycomex-0.9.3/pycomex/examples/results/004_inheritance/28_04_2023__13_45__bTbc/01_random.txt
--rw-r--r--   0        0        0     3827 2023-04-28 11:45:05.472587 pycomex-0.9.3/pycomex/examples/results/004_inheritance/28_04_2023__13_45__bTbc/02_random.txt
--rw-r--r--   0        0        0     3812 2023-04-28 11:45:05.472587 pycomex-0.9.3/pycomex/examples/results/004_inheritance/28_04_2023__13_45__bTbc/03_random.txt
--rw-r--r--   0        0        0     3794 2023-04-28 11:45:05.472587 pycomex-0.9.3/pycomex/examples/results/004_inheritance/28_04_2023__13_45__bTbc/04_random.txt
--rw-r--r--   0        0        0     3848 2023-04-28 11:45:05.476587 pycomex-0.9.3/pycomex/examples/results/004_inheritance/28_04_2023__13_45__bTbc/05_random.txt
--rw-r--r--   0        0        0     3823 2023-04-28 11:45:05.476587 pycomex-0.9.3/pycomex/examples/results/004_inheritance/28_04_2023__13_45__bTbc/06_random.txt
--rw-r--r--   0        0        0     3689 2023-04-28 11:45:05.476587 pycomex-0.9.3/pycomex/examples/results/004_inheritance/28_04_2023__13_45__bTbc/07_random.txt
--rw-r--r--   0        0        0     3770 2023-04-28 11:45:05.476587 pycomex-0.9.3/pycomex/examples/results/004_inheritance/28_04_2023__13_45__bTbc/08_random.txt
--rw-r--r--   0        0        0     3802 2023-04-28 11:45:05.476587 pycomex-0.9.3/pycomex/examples/results/004_inheritance/28_04_2023__13_45__bTbc/09_random.txt
--rw-r--r--   0        0        0     2255 2023-04-28 11:45:05.204585 pycomex-0.9.3/pycomex/examples/results/004_inheritance/28_04_2023__13_45__bTbc/analysis.py
--rw-r--r--   0        0        0       96 2023-04-28 11:45:05.480587 pycomex-0.9.3/pycomex/examples/results/004_inheritance/28_04_2023__13_45__bTbc/analysis_results.json
--rwxr-xr-x   0        0        0     3947 2023-04-28 11:45:05.200585 pycomex-0.9.3/pycomex/examples/results/004_inheritance/28_04_2023__13_45__bTbc/code.py
--rw-r--r--   0        0        0      176 2023-04-28 11:45:05.476587 pycomex-0.9.3/pycomex/examples/results/004_inheritance/28_04_2023__13_45__bTbc/experiment_data.json
--rw-r--r--   0        0        0      873 2023-04-28 11:45:05.476587 pycomex-0.9.3/pycomex/examples/results/004_inheritance/28_04_2023__13_45__bTbc/experiment_meta.json
--rwxr-xr-x   0        0        0      249 2023-02-13 21:10:16.382151 pycomex-0.9.3/pycomex/examples/run_experiment.py
--rwxr-xr-x   0        0        0    67161 2023-03-24 07:43:14.740032 pycomex-0.9.3/pycomex/experiment.py
--rw-r--r--   0        0        0        0 2023-04-20 08:46:28.005560 pycomex-0.9.3/pycomex/functional/__init__.py
--rw-r--r--   0        0        0    19968 2023-05-05 13:01:49.206402 pycomex-0.9.3/pycomex/functional/experiment.py
--rwxr-xr-x   0        0        0      865 2023-02-13 19:06:58.700540 pycomex-0.9.3/pycomex/templates/analysis.py.j2
--rwxr-xr-x   0        0        0      336 2022-07-17 07:15:39.751824 pycomex-0.9.3/pycomex/templates/annotations.py.j2
--rwxr-xr-x   0        0        0      464 2022-09-12 19:13:15.159972 pycomex-0.9.3/pycomex/templates/experiment_ended.text.j2
--rwxr-xr-x   0        0        0     1083 2022-09-19 07:16:21.662861 pycomex-0.9.3/pycomex/templates/experiment_info.out.j2
--rwxr-xr-x   0        0        0      389 2022-08-21 07:30:07.791594 pycomex-0.9.3/pycomex/templates/experiment_started.text.j2
--rwxr-xr-x   0        0        0     1106 2022-08-21 08:59:19.545111 pycomex-0.9.3/pycomex/templates/experiment_status.text.j2
--rw-r--r--   0        0        0      994 2023-04-27 10:24:01.392742 pycomex-0.9.3/pycomex/templates/functional_analysis.py.j2
--rw-r--r--   0        0        0      626 2023-04-27 09:26:03.450132 pycomex-0.9.3/pycomex/templates/functional_experiment_end.out.j2
--rw-r--r--   0        0        0      149 2023-04-27 10:32:23.124417 pycomex-0.9.3/pycomex/templates/functional_experiment_error.out.j2
--rw-r--r--   0        0        0      403 2023-04-27 09:18:50.959202 pycomex-0.9.3/pycomex/templates/functional_experiment_start.out.j2
--rwxr-xr-x   0        0        0      204 2022-09-18 17:25:07.672803 pycomex-0.9.3/pycomex/templates/list_experiments.out.j2
--rwxr-xr-x   0        0        0     3728 2023-02-13 21:09:19.222087 pycomex-0.9.3/pycomex/testing.py
--rwxr-xr-x   0        0        0    11368 2023-05-05 12:58:19.944885 pycomex-0.9.3/pycomex/util.py
--rw-r--r--   0        0        0      300 2023-04-20 08:56:18.406253 pycomex-0.9.3/pycomex/utils.py
--rwxr-xr-x   0        0        0     1837 2022-07-11 10:00:30.134647 pycomex-0.9.3/pycomex/work.py
--rwxr-xr-x   0        0        0     1294 2023-05-05 13:03:19.235057 pycomex-0.9.3/pyproject.toml
--rw-r--r--   0        0        0    10102 1970-01-01 00:00:00.000000 pycomex-0.9.3/setup.py
--rw-r--r--   0        0        0     9777 1970-01-01 00:00:00.000000 pycomex-0.9.3/PKG-INFO
+-rwxr-xr-x   0        0        0     1071 2022-07-09 08:06:36.748802 pycomex-0.9.4/LICENSE
+-rwxr-xr-x   0        0        0     8890 2023-04-27 14:30:13.471269 pycomex-0.9.4/README.rst
+-rwxr-xr-x   0        0        0        6 2023-05-08 10:37:49.526366 pycomex-0.9.4/pycomex/VERSION
+-rwxr-xr-x   0        0        0      178 2023-05-08 10:37:49.526366 pycomex-0.9.4/pycomex/__init__.py
+-rwxr-xr-x   0        0        0        0 2022-08-20 17:22:07.854881 pycomex-0.9.4/pycomex/app/__init__.py
+-rwxr-xr-x   0        0        0     7375 2023-01-03 06:49:42.464925 pycomex-0.9.4/pycomex/cli.py
+-rwxr-xr-x   0        0        0     2723 2023-04-28 09:23:59.597325 pycomex-0.9.4/pycomex/examples/001_quickstart.py
+-rwxr-xr-x   0        0        0     3514 2023-04-28 09:16:39.398304 pycomex-0.9.4/pycomex/examples/002_basic.py
+-rwxr-xr-x   0        0        0     3920 2023-04-28 09:23:59.589325 pycomex-0.9.4/pycomex/examples/003_analysing.py
+-rwxr-xr-x   0        0        0     3947 2023-04-28 09:52:25.866646 pycomex-0.9.4/pycomex/examples/004_inheritance.py
+-rwxr-xr-x   0        0        0      915 2023-04-28 09:23:35.509077 pycomex-0.9.4/pycomex/examples/README.rst
+-rwxr-xr-x   0        0        0     3920 2023-04-28 11:45:05.200585 pycomex-0.9.4/pycomex/examples/results/004_inheritance/28_04_2023__13_45__bTbc/003_analysing.py
+-rw-r--r--   0        0        0     3822 2023-04-28 11:45:05.472587 pycomex-0.9.4/pycomex/examples/results/004_inheritance/28_04_2023__13_45__bTbc/00_random.txt
+-rw-r--r--   0        0        0     3747 2023-04-28 11:45:05.472587 pycomex-0.9.4/pycomex/examples/results/004_inheritance/28_04_2023__13_45__bTbc/01_random.txt
+-rw-r--r--   0        0        0     3827 2023-04-28 11:45:05.472587 pycomex-0.9.4/pycomex/examples/results/004_inheritance/28_04_2023__13_45__bTbc/02_random.txt
+-rw-r--r--   0        0        0     3812 2023-04-28 11:45:05.472587 pycomex-0.9.4/pycomex/examples/results/004_inheritance/28_04_2023__13_45__bTbc/03_random.txt
+-rw-r--r--   0        0        0     3794 2023-04-28 11:45:05.472587 pycomex-0.9.4/pycomex/examples/results/004_inheritance/28_04_2023__13_45__bTbc/04_random.txt
+-rw-r--r--   0        0        0     3848 2023-04-28 11:45:05.476587 pycomex-0.9.4/pycomex/examples/results/004_inheritance/28_04_2023__13_45__bTbc/05_random.txt
+-rw-r--r--   0        0        0     3823 2023-04-28 11:45:05.476587 pycomex-0.9.4/pycomex/examples/results/004_inheritance/28_04_2023__13_45__bTbc/06_random.txt
+-rw-r--r--   0        0        0     3689 2023-04-28 11:45:05.476587 pycomex-0.9.4/pycomex/examples/results/004_inheritance/28_04_2023__13_45__bTbc/07_random.txt
+-rw-r--r--   0        0        0     3770 2023-04-28 11:45:05.476587 pycomex-0.9.4/pycomex/examples/results/004_inheritance/28_04_2023__13_45__bTbc/08_random.txt
+-rw-r--r--   0        0        0     3802 2023-04-28 11:45:05.476587 pycomex-0.9.4/pycomex/examples/results/004_inheritance/28_04_2023__13_45__bTbc/09_random.txt
+-rw-r--r--   0        0        0     2255 2023-04-28 11:45:05.204585 pycomex-0.9.4/pycomex/examples/results/004_inheritance/28_04_2023__13_45__bTbc/analysis.py
+-rw-r--r--   0        0        0       96 2023-04-28 11:45:05.480587 pycomex-0.9.4/pycomex/examples/results/004_inheritance/28_04_2023__13_45__bTbc/analysis_results.json
+-rwxr-xr-x   0        0        0     3947 2023-04-28 11:45:05.200585 pycomex-0.9.4/pycomex/examples/results/004_inheritance/28_04_2023__13_45__bTbc/code.py
+-rw-r--r--   0        0        0      176 2023-04-28 11:45:05.476587 pycomex-0.9.4/pycomex/examples/results/004_inheritance/28_04_2023__13_45__bTbc/experiment_data.json
+-rw-r--r--   0        0        0      873 2023-04-28 11:45:05.476587 pycomex-0.9.4/pycomex/examples/results/004_inheritance/28_04_2023__13_45__bTbc/experiment_meta.json
+-rwxr-xr-x   0        0        0      249 2023-02-13 21:10:16.382151 pycomex-0.9.4/pycomex/examples/run_experiment.py
+-rwxr-xr-x   0        0        0    67161 2023-03-24 07:43:14.740032 pycomex-0.9.4/pycomex/experiment.py
+-rw-r--r--   0        0        0        0 2023-04-20 08:46:28.005560 pycomex-0.9.4/pycomex/functional/__init__.py
+-rw-r--r--   0        0        0    21265 2023-05-08 10:36:24.030169 pycomex-0.9.4/pycomex/functional/experiment.py
+-rwxr-xr-x   0        0        0      865 2023-02-13 19:06:58.700540 pycomex-0.9.4/pycomex/templates/analysis.py.j2
+-rwxr-xr-x   0        0        0      336 2022-07-17 07:15:39.751824 pycomex-0.9.4/pycomex/templates/annotations.py.j2
+-rwxr-xr-x   0        0        0      464 2022-09-12 19:13:15.159972 pycomex-0.9.4/pycomex/templates/experiment_ended.text.j2
+-rwxr-xr-x   0        0        0     1083 2022-09-19 07:16:21.662861 pycomex-0.9.4/pycomex/templates/experiment_info.out.j2
+-rwxr-xr-x   0        0        0      389 2022-08-21 07:30:07.791594 pycomex-0.9.4/pycomex/templates/experiment_started.text.j2
+-rwxr-xr-x   0        0        0     1106 2022-08-21 08:59:19.545111 pycomex-0.9.4/pycomex/templates/experiment_status.text.j2
+-rw-r--r--   0        0        0     1078 2023-05-08 10:36:09.734144 pycomex-0.9.4/pycomex/templates/functional_analysis.py.j2
+-rw-r--r--   0        0        0      626 2023-04-27 09:26:03.450132 pycomex-0.9.4/pycomex/templates/functional_experiment_end.out.j2
+-rw-r--r--   0        0        0      149 2023-04-27 10:32:23.124417 pycomex-0.9.4/pycomex/templates/functional_experiment_error.out.j2
+-rw-r--r--   0        0        0      403 2023-04-27 09:18:50.959202 pycomex-0.9.4/pycomex/templates/functional_experiment_start.out.j2
+-rwxr-xr-x   0        0        0      204 2022-09-18 17:25:07.672803 pycomex-0.9.4/pycomex/templates/list_experiments.out.j2
+-rwxr-xr-x   0        0        0     3728 2023-02-13 21:09:19.222087 pycomex-0.9.4/pycomex/testing.py
+-rwxr-xr-x   0        0        0    11368 2023-05-05 12:58:19.944885 pycomex-0.9.4/pycomex/util.py
+-rw-r--r--   0        0        0      300 2023-04-20 08:56:18.406253 pycomex-0.9.4/pycomex/utils.py
+-rwxr-xr-x   0        0        0     1837 2022-07-11 10:00:30.134647 pycomex-0.9.4/pycomex/work.py
+-rwxr-xr-x   0        0        0     1294 2023-05-08 10:37:49.518365 pycomex-0.9.4/pyproject.toml
+-rw-r--r--   0        0        0    10102 1970-01-01 00:00:00.000000 pycomex-0.9.4/setup.py
+-rw-r--r--   0        0        0     9777 1970-01-01 00:00:00.000000 pycomex-0.9.4/PKG-INFO
```

### Comparing `pycomex-0.9.3/LICENSE` & `pycomex-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pycomex-0.9.3/README.rst` & `pycomex-0.9.4/README.rst`

 * *Files identical despite different names*

### Comparing `pycomex-0.9.3/pycomex/cli.py` & `pycomex-0.9.4/pycomex/cli.py`

 * *Files identical despite different names*

### Comparing `pycomex-0.9.3/pycomex/examples/001_quickstart.py` & `pycomex-0.9.4/pycomex/examples/001_quickstart.py`

 * *Files identical despite different names*

### Comparing `pycomex-0.9.3/pycomex/examples/002_basic.py` & `pycomex-0.9.4/pycomex/examples/002_basic.py`

 * *Files identical despite different names*

### Comparing `pycomex-0.9.3/pycomex/examples/003_analysing.py` & `pycomex-0.9.4/pycomex/examples/003_analysing.py`

 * *Files identical despite different names*

### Comparing `pycomex-0.9.3/pycomex/examples/004_inheritance.py` & `pycomex-0.9.4/pycomex/examples/004_inheritance.py`

 * *Files identical despite different names*

### Comparing `pycomex-0.9.3/pycomex/examples/README.rst` & `pycomex-0.9.4/pycomex/examples/README.rst`

 * *Files identical despite different names*

### Comparing `pycomex-0.9.3/pycomex/examples/results/004_inheritance/28_04_2023__13_45__bTbc/003_analysing.py` & `pycomex-0.9.4/pycomex/examples/results/004_inheritance/28_04_2023__13_45__bTbc/003_analysing.py`

 * *Files identical despite different names*

### Comparing `pycomex-0.9.3/pycomex/examples/results/004_inheritance/28_04_2023__13_45__bTbc/00_random.txt` & `pycomex-0.9.4/pycomex/examples/results/004_inheritance/28_04_2023__13_45__bTbc/00_random.txt`

 * *Files identical despite different names*

### Comparing `pycomex-0.9.3/pycomex/examples/results/004_inheritance/28_04_2023__13_45__bTbc/01_random.txt` & `pycomex-0.9.4/pycomex/examples/results/004_inheritance/28_04_2023__13_45__bTbc/01_random.txt`

 * *Files identical despite different names*

### Comparing `pycomex-0.9.3/pycomex/examples/results/004_inheritance/28_04_2023__13_45__bTbc/02_random.txt` & `pycomex-0.9.4/pycomex/examples/results/004_inheritance/28_04_2023__13_45__bTbc/02_random.txt`

 * *Files identical despite different names*

### Comparing `pycomex-0.9.3/pycomex/examples/results/004_inheritance/28_04_2023__13_45__bTbc/03_random.txt` & `pycomex-0.9.4/pycomex/examples/results/004_inheritance/28_04_2023__13_45__bTbc/03_random.txt`

 * *Files identical despite different names*

### Comparing `pycomex-0.9.3/pycomex/examples/results/004_inheritance/28_04_2023__13_45__bTbc/04_random.txt` & `pycomex-0.9.4/pycomex/examples/results/004_inheritance/28_04_2023__13_45__bTbc/04_random.txt`

 * *Files identical despite different names*

### Comparing `pycomex-0.9.3/pycomex/examples/results/004_inheritance/28_04_2023__13_45__bTbc/05_random.txt` & `pycomex-0.9.4/pycomex/examples/results/004_inheritance/28_04_2023__13_45__bTbc/05_random.txt`

 * *Files identical despite different names*

### Comparing `pycomex-0.9.3/pycomex/examples/results/004_inheritance/28_04_2023__13_45__bTbc/06_random.txt` & `pycomex-0.9.4/pycomex/examples/results/004_inheritance/28_04_2023__13_45__bTbc/06_random.txt`

 * *Files identical despite different names*

### Comparing `pycomex-0.9.3/pycomex/examples/results/004_inheritance/28_04_2023__13_45__bTbc/07_random.txt` & `pycomex-0.9.4/pycomex/examples/results/004_inheritance/28_04_2023__13_45__bTbc/07_random.txt`

 * *Files identical despite different names*

### Comparing `pycomex-0.9.3/pycomex/examples/results/004_inheritance/28_04_2023__13_45__bTbc/08_random.txt` & `pycomex-0.9.4/pycomex/examples/results/004_inheritance/28_04_2023__13_45__bTbc/08_random.txt`

 * *Files identical despite different names*

### Comparing `pycomex-0.9.3/pycomex/examples/results/004_inheritance/28_04_2023__13_45__bTbc/09_random.txt` & `pycomex-0.9.4/pycomex/examples/results/004_inheritance/28_04_2023__13_45__bTbc/09_random.txt`

 * *Files identical despite different names*

### Comparing `pycomex-0.9.3/pycomex/examples/results/004_inheritance/28_04_2023__13_45__bTbc/analysis.py` & `pycomex-0.9.4/pycomex/examples/results/004_inheritance/28_04_2023__13_45__bTbc/analysis.py`

 * *Files identical despite different names*

### Comparing `pycomex-0.9.3/pycomex/examples/results/004_inheritance/28_04_2023__13_45__bTbc/code.py` & `pycomex-0.9.4/pycomex/examples/results/004_inheritance/28_04_2023__13_45__bTbc/code.py`

 * *Files identical despite different names*

### Comparing `pycomex-0.9.3/pycomex/examples/results/004_inheritance/28_04_2023__13_45__bTbc/experiment_meta.json` & `pycomex-0.9.4/pycomex/examples/results/004_inheritance/28_04_2023__13_45__bTbc/experiment_meta.json`

 * *Files identical despite different names*

### Comparing `pycomex-0.9.3/pycomex/experiment.py` & `pycomex-0.9.4/pycomex/experiment.py`

 * *Files identical despite different names*

### Comparing `pycomex-0.9.3/pycomex/functional/experiment.py` & `pycomex-0.9.4/pycomex/functional/experiment.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,23 +52,39 @@
             'namespace': str(namespace),
             'description': '',
             'short_description': '',
         }
         self.error = None
         self.tb = None
 
+        # This list will contain the absolute string paths to all the python module files, which this
+        # experiment depends on (for example in the case that this experiment is a sub experiment that was
+        # created with the "extend" constructor)
         self.dependencies: t.List[str] = []
 
         self.analyses: t.List[t.Callable] = []
         self.hook_map: t.Dict[str, t.List[t.Callable]] = defaultdict(list)
 
         self.update_parameters()
 
         self.glob['__experiment__'] = self
 
+    @property
+    def dependency_names(self) -> t.List[str]:
+        """
+        A list of all the names of the python dependency modules, without the file extensions.
+        """
+        names = []
+        for path in self.dependencies:
+            name = os.path.basename(path)
+            name = os.path.splitext(name)[0]
+            names.append(name)
+
+        return names
+
     def update_parameters_special(self):
         if '__DEBUG__' in self.parameters:
             self.debug = bool(self.parameters['__DEBUG__'])
 
     def update_parameters(self):
         for name, value in self.glob.items():
             if name.isupper():
@@ -89,17 +105,21 @@
 
     def log_parameters(self):
         for name, value in self.parameters:
             self.log(name)
 
     # ~ Hook System
 
-    def hook(self, name: str, replace: bool = True):
+    def hook(self, name: str, replace: bool = True, default: bool = True):
 
         def decorator(func, *args, **kwargs):
+            # 07.05.23 - The thingy
+            if default and name in self.hook_map:
+                return
+
             if replace:
                 self.hook_map[name] = [func]
             else:
                 self.hook_map[name].append(func)
 
         return decorator
 
@@ -395,17 +415,33 @@
             self.glob[key] = value
         else:
             super(Experiment, self).__setattr__(key, value)
 
     # ~ File Handling Utility
 
     def open(self, file_name: str, *args, **kwargs):
+        """
+        This is an alternative file context for the default python ``open`` implementation.
+        """
         path = os.path.join(self.path, file_name)
         return open(path, *args, **kwargs)
 
+    def commit_fig(self,
+                   file_name: str,
+                   fig: t.Any,
+                   ) -> None:
+        """
+        Given the name ``file_name`` for a file and matplotlib Figure instance, this method will save the
+        figure into a new image file in the archive folder.
+
+        :returns: None
+        """
+        path = os.path.join(self.path, file_name)
+        fig.savefig(path)
+
     def commit_json(self,
                     file_name: str,
                     data: t.Union[t.Dict, t.List],
                     encoder_cls=CustomJsonEncoder
                     ) -> None:
         """
         Given the name ``file_name`` for a file and some json encodable data structure ``data``, this method
```

### Comparing `pycomex-0.9.3/pycomex/templates/analysis.py.j2` & `pycomex-0.9.4/pycomex/templates/analysis.py.j2`

 * *Files identical despite different names*

### Comparing `pycomex-0.9.3/pycomex/templates/experiment_info.out.j2` & `pycomex-0.9.4/pycomex/templates/experiment_info.out.j2`

 * *Files identical despite different names*

### Comparing `pycomex-0.9.3/pycomex/templates/experiment_status.text.j2` & `pycomex-0.9.4/pycomex/templates/experiment_status.text.j2`

 * *Files identical despite different names*

### Comparing `pycomex-0.9.3/pycomex/templates/functional_analysis.py.j2` & `pycomex-0.9.4/pycomex/templates/functional_analysis.py.j2`

 * *Files 14% similar despite different names*

```diff
@@ -14,14 +14,17 @@
 
 # Useful imports for conducting analysis
 import numpy as np
 import matplotlib.pyplot as plt
 from pycomex.functional.experiment import Experiment
 
 # Importing the experiment
+{% for name in experiment.dependency_names %}
+from {{ name }} import *
+{% endfor %}
 from code import *
 
 PATH = pathlib.Path(__file__).parent.absolute()
 CODE_PATH = os.path.join(PATH, 'code.py')
 experiment = Experiment.load(CODE_PATH)
 experiment.analyses = []
 {% set analysis_map = experiment.get_analysis_code_map() %}
```

### Comparing `pycomex-0.9.3/pycomex/templates/functional_experiment_end.out.j2` & `pycomex-0.9.4/pycomex/templates/functional_experiment_end.out.j2`

 * *Files identical despite different names*

### Comparing `pycomex-0.9.3/pycomex/testing.py` & `pycomex-0.9.4/pycomex/testing.py`

 * *Files identical despite different names*

### Comparing `pycomex-0.9.3/pycomex/util.py` & `pycomex-0.9.4/pycomex/util.py`

 * *Files identical despite different names*

### Comparing `pycomex-0.9.3/pycomex/work.py` & `pycomex-0.9.4/pycomex/work.py`

 * *Files identical despite different names*

### Comparing `pycomex-0.9.3/pyproject.toml` & `pycomex-0.9.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry.core>=1.2.0b2"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pycomex"
-version = "0.9.3"
+version = "0.9.4"
 description = "Python Computational Experiments"
 license = "MIT"
 authors = ["Jonas Teufel <jonseb1998@gmail.com>"]
 maintainers = ["Jonas Teufel <jonseb1998@gmail.com>"]
 readme = "README.rst"
 documentation = "https://pycomex.readthedocs.io"
 keywords = ["computational experiments", "data science", "maschine learning", "academia"]
```

### Comparing `pycomex-0.9.3/setup.py` & `pycomex-0.9.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
  'psutil>=5.7.2']
 
 entry_points = \
 {'console_scripts': ['pycomex = pycomex.cli:main']}
 
 setup_kwargs = {
     'name': 'pycomex',
-    'version': '0.9.3',
+    'version': '0.9.4',
     'description': 'Python Computational Experiments',
     'long_description': '.. image:: https://img.shields.io/pypi/v/pycomex.svg\n        :target: https://pypi.python.org/pypi/pycomex\n\n.. image:: https://readthedocs.org/projects/pycomex/badge/?version=latest\n        :target: https://pycomex.readthedocs.io/en/latest/?version=latest\n        :alt: Documentation Status\n\nPyComex - Python Computational Experiments\n================================================\n\nMicroframework to improve the experience of running and managing archival records of computational\nexperiments, such as machine learning and data science experiments, in Python.\n\n* Free software: MIT license\n\nFeatures\n--------\n\n* Automatically create (nested) folder structure for results of each run of an experiment\n* Simply attach metadata such as performance metrics to experiment object and they will be automatically\n  stored as JSON file\n* Easily attach file artifacts such as ``matplotlib`` figures to experiment records\n* Log messages to stdout as well as permanently store into log file\n* Ready-to-use automatically generated boilerplate code for the analysis and post-processing of\n  experiment data after experiments have terminated.\n* Experiment inheritance: Experiment modules can inherit from other modules and extend their functionality\n  via parameter overwrites and hooks!\n\nInstallation\n------------\n\nInstall stable version with ``pip``\n\n.. code-block:: console\n\n    pip3 install pycomex\n\nOr the most recent development version\n\n.. code-block:: console\n\n    git clone https://github.com/the16thpythonist/pycomex.git\n    cd pycomex ; pip3 install .\n\nQuickstart\n----------\n\nEach computational experiment has to be bundled as a standalone python module. Important experiment\nparameters are placed at the top of this module. All variable names written in upper case will automatically\nbe detected as parameters of the experiment.\n\nThe actual implementation of the experiment execution is placed into a single file which will have to be\ndecorated with the ``Experiment`` decorator.\n\nUpon execution the experiment, a new archive folder is automatically created. This archive folder can\nbe used to store all the file artifacts that are created during the experiment.\nSome artifacts are stored automatically by default, such as a JSON file containing all data stored in the\nmain experiment storage, a snapshot of the experiment module and more...\n\nArchiving of metadata, file artifacts and error handling is automatically managed on context exit.\n\n.. code-block:: python\n\n    # quickstart.py\n    """\n    This doc string will be saved as the "description" meta data of the experiment records\n    """\n    import os\n    from pycomex.functional.experiment import Experiment\n    from pycomex.utils import folder_path, file_namespace\n\n    # Experiment parameters can simply be defined as uppercase global variables.\n    # These are automatically detected and can possibly be overwritten in command\n    # line invocation\n    HELLO = "hello "\n    WORLD = "world!"\n\n    # There are certain special parameters which will be detected by the experiment\n    # such as this, which will put the experiment into debug mode.\n    # That means instead of creating a new archive for every execution, it will always\n    # create/overwrite the "debug" archive folder.\n    __DEBUG__ = True\n\n    # An experiment is essentially a function. All of the code that constitutes\n    # one experiment should ultimately be called from this one function...\n\n    # The main experiment function has to be decorated with the "Experiment"\n    # decorator, which needs three main arguments:\n    # - base_path: The absolute string path to an existing FOLDER, where the\n    #   archive structure should be created\n    # - namespace: This is a relative path which defines the concrete folder\n    #   structure of the specific archive folder for this specific experiment\n    # - glob: The globals() dictionary for the current file\n    @Experiment(base_path=os.getcwd(),\n                namespace=\'results/quickstart\',\n                glob=globals())\n    def experiment(e: Experiment):\n        # Internally saved into automatically created nested dict\n        # {\'strings\': {\'hello_world\': \'...\'}}\n        e["strings/hello_world"] = HELLO + WORLD\n\n        # Alternative to "print". Message is printed to stdout as well as\n        # recorded to log file\n        e.log("some debug message")\n\n        # Automatically saves text file artifact to the experiment record folder\n        file_name = "hello_world.txt"\n        e.commit_raw(file_name, HELLO + WORLD)\n        # e.commit_fig(file_name, fig)\n        # e.commit_png(file_name, image)\n        # ...\n\n\n    @experiment.analysis\n    def analysis(e: Experiment):\n        # And we can access all the internal fields of the experiment object\n        # and the experiment parameters here!\n        print(HELLO, WORLD)\n        print(e[\'strings/hello_world\'])\n        # logging will print to stdout but not modify the log file\n        e.log(\'analysis done\')\n\n\n    # This needs to be put at the end of the experiment. This method will\n    # then actually execute the main experiment code defined in the function\n    # above.\n    # NOTE: The experiment will only be run if this module is directly\n    # executed (__name__ == \'__main__\'). Otherwise the experiment will NOT\n    # be executed, which implies that the experiment module can be imported\n    # from somewhere else without triggering experiment execution!\n    experiment.run_if_main()\n\n\nThis example would create the following folder structure:\n\n.. code-block:: python\n\n    cwd\n    |- results\n       |- quickstart\n          |- debug\n             |+ experiment_out.log     # Contains all the log messages printed by experiment\n             |+ experiment_meta.json   # Meta information about the experiment\n             |+ experiment_data.json   # All the data that was added to the internal exp. dict\n             |+ hello_world.txt        # Text artifact that was committed to the experiment\n             |+ code.py                # Copy of the original experiment python module\n             |+ analysis.py            # boilerplate code to get started with analysis of results\n\nThe ``analysis.py`` file is of special importance. It is created as a boilerplate starting\nplace for additional code, which performs analysis or post processing on the results of the experiment.\nThis can for example be used to transform data into a different format or create plots for visualization.\n\nSpecifically note these two aspects:\n\n1. The analysis file contains all of the code which was defined in the ``analysis`` function of the\n   original experiment file! This code snippet is automatically transferred at the end of the experiment.\n2. The analysis file actually imports the snapshot copy of the original experiment file. This does not\n   trigger the experiment to be executed again! The ``Experiment`` instance automatically notices that it\n   is being imported and not explicitly executed. It will also populate all of it\'s internal attributes\n   from the persistently saved data in ``experiment_data.json``, which means it is still possible to access\n   all the data of the experiment without having to execute it again!\n\n.. code-block:: python\n\n    # analysis.py\n\n    # [...] imports omitted\n    from code import *\n    from pycomex.functional.experiment import Experiment\n\n    PATH = pathlib.Path(__file__).parent.absolute()\n    # "Experiment.load" is used to load the the experiment data from the\n    # archive. it returns an "Experiment" object which will act exactly the\n    # same way as if the experiment had just finished it\'s execution!\n    CODE_PATH = os.path.join(PATH, \'code.py\')\n    experiment = Experiment.load(CODE_PATH)\n    experiment.analyses = []\n\n    # All of the following code is automatically extracted from main\n    # experiment module itself and can now be edited and re-executed.\n    # Re-execution of this analysis.py file will not trigger an\n    # execution of the experiment but all the stored results will be\n    # available anyways!\n    @experiment.analysis\n    def analysis(e: Experiment):\n        # And we can access all the internal fields of the experiment\n        # object and the experiment parameters here!\n        print(HELLO, WORLD)\n        print(e[\'strings/hello_world\'])\n        # logging will print to stdout but not modify the log file\n        e.info(\'analysis done\')\n\n\n    # This method will execute only the analysis code!\n    experiment.execute_analyses()\n\n\nFor an introduction to more advanced features take a look at the examples in\n``pycomex/examples`` ( https://github.com/the16thpythonist/pycomex/tree/master/pycomex/examples )\n\nCredits\n-------\n\nThis package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.\n\n.. _Cookiecutter: https://github.com/audreyr/cookiecutter\n.. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage\n',
     'author': 'Jonas Teufel',
     'author_email': 'jonseb1998@gmail.com',
     'maintainer': 'Jonas Teufel',
     'maintainer_email': 'jonseb1998@gmail.com',
     'url': 'None',
```

### Comparing `pycomex-0.9.3/PKG-INFO` & `pycomex-0.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycomex
-Version: 0.9.3
+Version: 0.9.4
 Summary: Python Computational Experiments
 License: MIT
 Keywords: computational experiments,data science,maschine learning,academia
 Author: Jonas Teufel
 Author-email: jonseb1998@gmail.com
 Maintainer: Jonas Teufel
 Maintainer-email: jonseb1998@gmail.com
```

