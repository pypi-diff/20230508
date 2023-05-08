# Comparing `tmp/slurm-parallel-0.1.0.tar.gz` & `tmp/slurm-parallel-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slurm-parallel-0.1.0.tar", last modified: Tue May  2 18:19:45 2023, max compression
+gzip compressed data, was "slurm-parallel-0.1.1.tar", last modified: Mon May  8 18:37:01 2023, max compression
```

## Comparing `slurm-parallel-0.1.0.tar` & `slurm-parallel-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxrwsr-x   0 hc3190   (413786699) domain users (413600513)        0 2023-05-02 18:19:45.160141 slurm-parallel-0.1.0/
--rw-rw-r--   0 hc3190   (413786699) domain users (413600513)     1065 2023-05-01 18:25:25.000000 slurm-parallel-0.1.0/LICENSE
--rw-rw-r--   0 hc3190   (413786699) domain users (413600513)      110 2023-05-01 22:51:25.000000 slurm-parallel-0.1.0/MANIFEST.in
--rw-rw-r--   0 hc3190   (413786699) domain users (413600513)     1823 2023-05-02 18:19:45.156108 slurm-parallel-0.1.0/PKG-INFO
--rw-rw-r--   0 hc3190   (413786699) domain users (413600513)       83 2023-05-01 18:25:25.000000 slurm-parallel-0.1.0/README.md
--rw-rw-r--   0 hc3190   (413786699) domain users (413600513)      774 2023-05-01 18:26:56.000000 slurm-parallel-0.1.0/pyproject.toml
--rw-rw-r--   0 hc3190   (413786699) domain users (413600513)       38 2023-05-02 18:19:45.161099 slurm-parallel-0.1.0/setup.cfg
-drwxrwsr-x   0 hc3190   (413786699) domain users (413600513)        0 2023-05-02 18:19:44.908852 slurm-parallel-0.1.0/src/
-drwxrwsr-x   0 hc3190   (413786699) domain users (413600513)        0 2023-05-02 18:19:45.063457 slurm-parallel-0.1.0/src/slurm_parallel/
--rw-rw-r--   0 hc3190   (413786699) domain users (413600513)      110 2023-05-01 20:47:47.000000 slurm-parallel-0.1.0/src/slurm_parallel/__init__.py
--rw-rw-r--   0 hc3190   (413786699) domain users (413600513)       19 2023-05-01 18:41:13.000000 slurm-parallel-0.1.0/src/slurm_parallel/cleanup.sh
--rw-rw-r--   0 hc3190   (413786699) domain users (413600513)       61 2023-05-02 01:39:05.000000 slurm-parallel-0.1.0/src/slurm_parallel/config.toml
--rw-rw-r--   0 hc3190   (413786699) domain users (413600513)       60 2023-05-01 18:26:56.000000 slurm-parallel-0.1.0/src/slurm_parallel/run.sh
--rw-rw-r--   0 hc3190   (413786699) domain users (413600513)     7902 2023-05-02 01:31:05.000000 slurm-parallel-0.1.0/src/slurm_parallel/slurm.py
-drwxrwsr-x   0 hc3190   (413786699) domain users (413600513)        0 2023-05-02 18:19:45.126449 slurm-parallel-0.1.0/src/slurm_parallel.egg-info/
--rw-rw-r--   0 hc3190   (413786699) domain users (413600513)     1823 2023-05-02 18:19:44.000000 slurm-parallel-0.1.0/src/slurm_parallel.egg-info/PKG-INFO
--rw-rw-r--   0 hc3190   (413786699) domain users (413600513)      412 2023-05-02 18:19:44.000000 slurm-parallel-0.1.0/src/slurm_parallel.egg-info/SOURCES.txt
--rw-rw-r--   0 hc3190   (413786699) domain users (413600513)        1 2023-05-02 18:19:44.000000 slurm-parallel-0.1.0/src/slurm_parallel.egg-info/dependency_links.txt
--rw-rw-r--   0 hc3190   (413786699) domain users (413600513)       32 2023-05-02 18:19:44.000000 slurm-parallel-0.1.0/src/slurm_parallel.egg-info/requires.txt
--rw-rw-r--   0 hc3190   (413786699) domain users (413600513)       15 2023-05-02 18:19:44.000000 slurm-parallel-0.1.0/src/slurm_parallel.egg-info/top_level.txt
-drwxrwsr-x   0 hc3190   (413786699) domain users (413600513)        0 2023-05-02 18:19:45.139139 slurm-parallel-0.1.0/test/
--rw-rw-r--   0 hc3190   (413786699) domain users (413600513)      984 2023-05-02 01:40:46.000000 slurm-parallel-0.1.0/test/test.py
+drwxrwsr-x   0 hc3190   (413786699) domain users (413600513)        0 2023-05-08 18:37:01.947971 slurm-parallel-0.1.1/
+-rw-rw-r--   0 hc3190   (413786699) domain users (413600513)     1065 2023-05-01 18:25:25.000000 slurm-parallel-0.1.1/LICENSE
+-rw-rw-r--   0 hc3190   (413786699) domain users (413600513)      110 2023-05-01 22:51:25.000000 slurm-parallel-0.1.1/MANIFEST.in
+-rw-rw-r--   0 hc3190   (413786699) domain users (413600513)     1823 2023-05-08 18:37:01.932850 slurm-parallel-0.1.1/PKG-INFO
+-rw-rw-r--   0 hc3190   (413786699) domain users (413600513)       83 2023-05-01 18:25:25.000000 slurm-parallel-0.1.1/README.md
+-rw-rw-r--   0 hc3190   (413786699) domain users (413600513)      702 2023-05-08 18:33:43.000000 slurm-parallel-0.1.1/pyproject.toml
+-rw-rw-r--   0 hc3190   (413786699) domain users (413600513)       38 2023-05-08 18:37:01.950252 slurm-parallel-0.1.1/setup.cfg
+drwxrwsr-x   0 hc3190   (413786699) domain users (413600513)        0 2023-05-08 18:37:00.077666 slurm-parallel-0.1.1/src/
+drwxrwsr-x   0 hc3190   (413786699) domain users (413600513)        0 2023-05-08 18:37:01.020038 slurm-parallel-0.1.1/src/slurm_parallel/
+-rw-rw-r--   0 hc3190   (413786699) domain users (413600513)      110 2023-05-01 20:47:47.000000 slurm-parallel-0.1.1/src/slurm_parallel/__init__.py
+-rw-rw-r--   0 hc3190   (413786699) domain users (413600513)       37 2023-05-08 18:25:50.000000 slurm-parallel-0.1.1/src/slurm_parallel/cleanup.sh
+-rw-rw-r--   0 hc3190   (413786699) domain users (413600513)       61 2023-05-02 01:39:05.000000 slurm-parallel-0.1.1/src/slurm_parallel/config.toml
+-rw-rw-r--   0 hc3190   (413786699) domain users (413600513)      478 2023-05-08 18:21:00.000000 slurm-parallel-0.1.1/src/slurm_parallel/run.py
+-rw-rw-r--   0 hc3190   (413786699) domain users (413600513)       35 2023-05-08 18:16:02.000000 slurm-parallel-0.1.1/src/slurm_parallel/run.sh
+-rw-rw-r--   0 hc3190   (413786699) domain users (413600513)     7680 2023-05-08 18:17:46.000000 slurm-parallel-0.1.1/src/slurm_parallel/slurm.py
+-rw-rw-r--   0 hc3190   (413786699) domain users (413600513)     2099 2023-05-08 17:39:51.000000 slurm-parallel-0.1.1/src/slurm_parallel/utils.py
+drwxrwsr-x   0 hc3190   (413786699) domain users (413600513)        0 2023-05-08 18:37:01.307776 slurm-parallel-0.1.1/src/slurm_parallel.egg-info/
+-rw-rw-r--   0 hc3190   (413786699) domain users (413600513)     1823 2023-05-08 18:36:59.000000 slurm-parallel-0.1.1/src/slurm_parallel.egg-info/PKG-INFO
+-rw-rw-r--   0 hc3190   (413786699) domain users (413600513)      466 2023-05-08 18:36:59.000000 slurm-parallel-0.1.1/src/slurm_parallel.egg-info/SOURCES.txt
+-rw-rw-r--   0 hc3190   (413786699) domain users (413600513)        1 2023-05-08 18:36:59.000000 slurm-parallel-0.1.1/src/slurm_parallel.egg-info/dependency_links.txt
+-rw-rw-r--   0 hc3190   (413786699) domain users (413600513)       15 2023-05-08 18:36:59.000000 slurm-parallel-0.1.1/src/slurm_parallel.egg-info/requires.txt
+-rw-rw-r--   0 hc3190   (413786699) domain users (413600513)       15 2023-05-08 18:36:59.000000 slurm-parallel-0.1.1/src/slurm_parallel.egg-info/top_level.txt
+drwxrwsr-x   0 hc3190   (413786699) domain users (413600513)        0 2023-05-08 18:37:01.862653 slurm-parallel-0.1.1/test/
+-rw-rw-r--   0 hc3190   (413786699) domain users (413600513)     1182 2023-05-08 18:25:32.000000 slurm-parallel-0.1.1/test/test.py
```

### Comparing `slurm-parallel-0.1.0/LICENSE` & `slurm-parallel-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `slurm-parallel-0.1.0/PKG-INFO` & `slurm-parallel-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slurm-parallel
-Version: 0.1.0
+Version: 0.1.1
 Summary: Easy parallelization of python functions on SLURM using job arrays.
 Author: Ho Yin Chau
 License: MIT License
         
         Copyright (c) 2023 hchau630
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `slurm-parallel-0.1.0/pyproject.toml` & `slurm-parallel-0.1.1/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 [build-system]
 requires = ["setuptools>=64.0"] # editable install using setuptool available since v64.0.0
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "slurm-parallel"
-version = "0.1.0"
+version = "0.1.1"
 description = "Easy parallelization of python functions on SLURM using job arrays."
 readme = "README.md"
 requires-python = ">=3.9"
 license = {file = "LICENSE"}
 authors = [
     {name = "Ho Yin Chau"},
 ]
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.9",
 ]
 dependencies = [
-    'dfdb>=0.1.8',
     'hyclib>=0.1.14',
-    'fire', # for calling function from command line
 ]
 
 [project.urls]
 repository = "https://github.com/hchau630/slurm-parallel"
```

### Comparing `slurm-parallel-0.1.0/src/slurm_parallel/slurm.py` & `slurm-parallel-0.1.1/src/slurm_parallel/slurm.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,18 +11,19 @@
 import copy
 import math
 from string import Template
 from importlib import resources
 
 import hyclib as lib
 
-from . import config
+from . import config, utils
 
 logger = logging.getLogger(__name__)
 run_script = resources.files('slurm_parallel').joinpath('run.sh')
+run_py_script = resources.files('slurm_parallel').joinpath('run.py')
 cleanup_script = resources.files('slurm_parallel').joinpath('cleanup.sh')
 
 allowed_args = {'A', 'account', 'acctg_freq', 'batch', 'bb', 'bbf', 'b', 'begin', 'D', 'chdir', 'cluster_constraint', 'M', 'clusters', 'comment', 'C', 'constraint', 'container', 'container_id', 'contiguous', 'S', 'core-spec', 'cores_per_socket', 'cpu_freq', 'cpus_per_gpu', 'c', 'cpus_per_task', 'deadline', 'delay_boot', 'd', 'dependency', 'm', 'distribution', 'e', 'error', 'x', 'exclude', 'exclusive', 'export', 'export_file', 'extra', 'B', 'extra_node_info', 'get_user_env', 'gid', 'gpu_bind', 'gpu_freq', 'G', 'gpus', 'gpus_per_node', 'gpus_per_socket', 'gpus_per_task', 'gres', 'gres_flags', 'h', 'help', 'hint', 'H', 'hold', 'ignore_pbs', 'i', 'input', 'J', 'job_name', 'kill_on_invalid_dep', 'L', 'licenses', 'mail_type', 'mail_user', 'mcs_label', 'mem', 'mem_bind', 'mem_per_cpu', 'mem_per_gpu', 'mincpus', 'network', 'nice', 'k', 'no_kill', 'no_requeue', 'F', 'nodefile', 'w', 'nodelist', 'N', 'nodes', 'n', 'ntasks', 'ntasks_per_core', 'ntasks_per_gpu', 'ntasks_per_node', 'ntasks_per_socket', 'open_mode', 'O', 'overcommit', 's', 'oversubscribe', 'p', 'partition', 'power', 'prefer', 'priority', 'profile', 'propagate', 'q', 'qos', 'Q', 'quiet', 'reboot', 'requeue', 'reservation', 'signal', 'sockets_per_node', 'spread_job', 'switches', 'test_only', 'thread_spec', 'threads_per_core', 't', 'time', 'time_min', 'tmp', 'tres_per_task', 'uid', 'usage', 'use_min_nodes', 'v', 'verbose', 'V', 'version', 'W', 'wait', 'wait_all_nodes', 'wckey', 'wrap'}
 
 __all__ = ['parallelize']
 
 class StringTemplate(Template):
@@ -113,26 +114,27 @@
         run_kwargs = {
             'c': 2,
             'mem_per_cpu': '2gb',
             'time': lib.datetime.strftime(time_per_task, '%d-%H:%M:%S'),
             'array': f'0-{n_tasks-1}',
             'output': out_dir / out_file,
             'parsable': True,
+            'job_name': f'{pathlib.Path(filename).stem}_{funcname}',
         } | default_kwargs | kwargs
-        run_options = _to_cmd_options(**run_kwargs)
+        run_options = utils.to_cmd_options(**run_kwargs)
         
         try:
             with tempfile.NamedTemporaryFile(dir=tmp_dir, mode='w', delete=False) as f:
                 json.dump(configs, f)
                 
             tmp_file = pathlib.Path(f.name)
             logger.info(f"Saved configs to tmp file {tmp_file}.")
             
             completed_process = subprocess.run(
-                ["sbatch", *run_options, str(run_script), filename, funcname, str(tmp_file)],
+                ["sbatch", *run_options, str(run_script), str(run_py_script), filename, funcname, str(tmp_file)],
                 capture_output=True,
                 check=True,
             )
         
             run_PID = completed_process.stdout.decode("utf-8").split('\n')[-2]
 
             logger.info(f"Submitted job to cluster to run {funcname} with job ID {run_PID}.")
@@ -141,16 +143,17 @@
             cleanup_kwargs = {
                 'c': 1,
                 'mem_per_cpu': '1mb',
                 'time': 1, # 1 minute
                 'dependency': f'afterany:{run_PID}',
                 'output': out_dir / "cleanup.out",
                 'parsable': True,
+                'job_name': f'{pathlib.Path(filename).stem}_{funcname}_cleanup',
             }
-            cleanup_options = _to_cmd_options(**cleanup_kwargs)
+            cleanup_options = utils.to_cmd_options(**cleanup_kwargs)
 
             completed_process = subprocess.run(
                 ["sbatch", *cleanup_options, str(cleanup_script), str(tmp_file)],
                 capture_output=True,
                 check=True,
             )
             
@@ -166,27 +169,7 @@
         return run_PID
     
     func.run_task = run_task
     func.remote = remote
     
     return func
         
-def _to_cmd_options(**kwargs):
-    options = []
-
-    for k, v in kwargs.items():
-        k = k.replace('_', '-')
-        k = f'--{k}' if len(k) > 1 else f'-{k}'
-
-        if isinstance(v, bool) and not v:
-            continue
-        
-        options.append(k)
-        
-        if isinstance(v, bool):
-            continue
-        elif isinstance(v, (list, tuple)):
-            options += [str(vi) for vi in v]
-        else:
-            options.append(str(v))
-
-    return options
```

### Comparing `slurm-parallel-0.1.0/src/slurm_parallel.egg-info/PKG-INFO` & `slurm-parallel-0.1.1/src/slurm_parallel.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slurm-parallel
-Version: 0.1.0
+Version: 0.1.1
 Summary: Easy parallelization of python functions on SLURM using job arrays.
 Author: Ho Yin Chau
 License: MIT License
         
         Copyright (c) 2023 hchau630
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `slurm-parallel-0.1.0/test/test.py` & `slurm-parallel-0.1.1/test/test.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,30 @@
 import logging
+import time
 
 import sqlalchemy as sa
 import dfdb
 import hyclib as lib
 
 import slurm_parallel as sp
 
 lib.logging.basic_config()
 logger = logging.getLogger()
 logger.setLevel('DEBUG')
 
 db = dfdb.Database(database='test/data/test.db')
 
-@sp.parallelize(database=db, table='results', columns='result', mem_per_cpu='1gb', c=1)
+@sp.parallelize(mem_per_cpu='1gb', c=1, partition='ctn')
+def print_results():
+    df = db['results'].fetch()
+    print(df)
+
+@sp.parallelize(database=db, table='results', columns='result', mem_per_cpu='1gb', c=1, partition='ctn')
 def func(a, b):
+    # time.sleep(30)
     return a + b
 
 def main():
     if 'results' in db:
         del db['results']
         
     db['results'] = dfdb.TableDef(
@@ -30,13 +37,12 @@
     
     configs = [
         {'a': 1, 'b': 2},
         {'a': 3, 'b': 4},
         {'a': 5, 'b': 6},
         {'a': 7, 'b': 8},
     ]
-    job = func.remote(configs, wait=True, max_n_tasks=3)
-    
-    print(db['results'].fetch())
+    job = func.remote(configs, wait=False, max_n_tasks=3)
+    print_results.remote([{}], dependency=f'afterany:{job}')
 
 if __name__ == '__main__':
     main()
```

