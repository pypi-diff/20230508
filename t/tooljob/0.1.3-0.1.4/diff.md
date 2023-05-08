# Comparing `tmp/tooljob-0.1.3.tar.gz` & `tmp/tooljob-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tooljob-0.1.3.tar", last modified: Sat Apr 29 17:53:27 2023, max compression
+gzip compressed data, was "tooljob-0.1.4.tar", last modified: Mon May  8 00:48:38 2023, max compression
```

## Comparing `tooljob-0.1.3.tar` & `tooljob-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0      217 2023-02-26 19:33:55.835763 tooljob-0.1.3/.gitignore
--rw-r--r--   0        0        0      742 2023-02-26 02:20:54.175448 tooljob-0.1.3/README.md
--rw-r--r--   0        0        0      274 2023-02-26 19:46:21.973498 tooljob-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      147 2023-04-29 17:53:03.211684 tooljob-0.1.3/tooljob/__init__.py
--rw-r--r--   0        0        0    12952 2023-04-29 16:07:02.844212 tooljob-0.1.3/tooljob/batch_class.py
--rw-r--r--   0        0        0        0 2023-04-10 03:48:04.176428 tooljob-0.1.3/tooljob/py.typed
--rw-r--r--   0        0        0       68 2023-02-26 07:21:03.717968 tooljob-0.1.3/tooljob/spec/__init__.py
--rw-r--r--   0        0        0      124 2023-04-28 23:01:22.123067 tooljob-0.1.3/tooljob/spec/typedefs.py
--rw-r--r--   0        0        0       29 2023-02-26 07:48:30.506903 tooljob-0.1.3/tooljob/trackers/__init__.py
--rw-r--r--   0        0        0      197 2023-02-26 06:53:20.062932 tooljob-0.1.3/tooljob/trackers/bucket_tracker.py
--rw-r--r--   0        0        0     2932 2023-04-28 23:01:49.155581 tooljob-0.1.3/tooljob/trackers/file_tracker.py
--rw-r--r--   0        0        0     5358 2023-02-26 19:46:45.227524 tooljob-0.1.3/tooljob/trackers/sql_tracker.py
--rw-r--r--   0        0        0      535 2023-02-26 07:49:26.664051 tooljob-0.1.3/tooljob/trackers/tracker.py
--rw-r--r--   0        0        0     1514 2023-04-28 23:07:49.016212 tooljob-0.1.3/tooljob/trackers/tracker_utils.py
--rw-r--r--   0        0        0      127 1970-01-01 00:00:00.000000 tooljob-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      217 2023-02-26 19:33:55.835763 tooljob-0.1.4/.gitignore
+-rw-r--r--   0        0        0      742 2023-02-26 02:20:54.175448 tooljob-0.1.4/README.md
+-rw-r--r--   0        0        0      415 2023-05-08 00:41:28.141877 tooljob-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      147 2023-05-08 00:42:32.476173 tooljob-0.1.4/tooljob/__init__.py
+-rw-r--r--   0        0        0    13720 2023-05-08 00:47:08.020829 tooljob-0.1.4/tooljob/batch_class.py
+-rw-r--r--   0        0        0        0 2023-04-10 03:48:04.176428 tooljob-0.1.4/tooljob/py.typed
+-rw-r--r--   0        0        0       68 2023-02-26 07:21:03.717968 tooljob-0.1.4/tooljob/spec/__init__.py
+-rw-r--r--   0        0        0      521 2023-05-02 23:13:32.556227 tooljob-0.1.4/tooljob/spec/typedefs.py
+-rw-r--r--   0        0        0       29 2023-02-26 07:48:30.506903 tooljob-0.1.4/tooljob/trackers/__init__.py
+-rw-r--r--   0        0        0      197 2023-02-26 06:53:20.062932 tooljob-0.1.4/tooljob/trackers/bucket_tracker.py
+-rw-r--r--   0        0        0     2581 2023-05-01 23:06:11.250903 tooljob-0.1.4/tooljob/trackers/file_tracker.py
+-rw-r--r--   0        0        0     5509 2023-05-02 23:15:55.671275 tooljob-0.1.4/tooljob/trackers/multifile_tracker.py
+-rw-r--r--   0        0        0     5358 2023-02-26 19:46:45.227524 tooljob-0.1.4/tooljob/trackers/sql_tracker.py
+-rw-r--r--   0        0        0      535 2023-02-26 07:49:26.664051 tooljob-0.1.4/tooljob/trackers/tracker.py
+-rw-r--r--   0        0        0     2321 2023-05-02 23:14:50.134997 tooljob-0.1.4/tooljob/trackers/tracker_utils.py
+-rw-r--r--   0        0        0      281 1970-01-01 00:00:00.000000 tooljob-0.1.4/PKG-INFO
```

### Comparing `tooljob-0.1.3/README.md` & `tooljob-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `tooljob-0.1.3/tooljob/batch_class.py` & `tooljob-0.1.4/tooljob/batch_class.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from __future__ import annotations
 
-import concurrent
 import time
 import typing
 
 if typing.TYPE_CHECKING:
     from typing_extensions import Literal
 
     import polars as pl
@@ -33,14 +32,15 @@
     def __init__(
         self,
         *,
         jobs: typing.Sequence[spec.JobData] | None = None,
         tracker: str | None = None,
         output_dir: str | None = None,
         output_filetype: str | None = None,
+        outputs: typing.Mapping[str, str] | None = None,
         db_config: toolsql.DBConfig | None = None,
         bucket_path: str | None = None,
         name: str | None = None,
         styles: toolcli.StyleTheme | None = None,
         verbose: bool = False,
     ) -> None:
         self.name = name
@@ -67,33 +67,42 @@
             return type(self).__name__
 
     def get_job_name(
         self,
         i: int | None = None,
         *,
         job_data: spec.JobData | None = None,
+        parameters: typing.Mapping[str, str] | None = None,
     ) -> str:
         if job_data is None:
             if i is None:
                 raise Exception('must specify job_data or i')
             job_data = self.get_job_data(i)
-        simple_types = (str, int, bool)
-        if isinstance(job_data, simple_types):
+
+        if isinstance(job_data, (str, int, bool)):
             return self.get_job_list_name() + str(job_data)
+
         elif isinstance(job_data, dict):
             for key, value in job_data.items():
-                if not isinstance(value, simple_types):
+                if not isinstance(value, (str, int, bool)):
                     raise NotImplementedError(
                         'must define job_name() for this type of job_data'
                     )
             tokens = [
                 key + '_' + job_data[key]
                 for key, value in sorted(job_data.items())
             ]
+
+            # add additional parameters to name
+            if parameters is not None:
+                for key, value in sorted(parameters.items()):
+                    tokens.append(key + '_' + value)
+
             return self.get_job_list_name() + '__'.join(tokens)
+
         else:
             raise NotImplementedError(
                 'must define get_job_name() for this type of job_data'
             )
 
     def parse_job_name(self, name: str) -> spec.JobData:
         job_data = {}
@@ -219,25 +228,40 @@
         self.print_conclusion(
             start_time=start_time,
             end_time=time.time(),
             jobs=remaining_jobs,
         )
 
     def serial_execute(self, jobs: typing.Sequence[int]) -> None:
-        for job in jobs:
+        import tqdm
+
+        color = self._get_progress_bar_color()
+        for job in tqdm.tqdm(jobs, colour=color):
             self.run_job(job)
 
     def parallel_execute(
         self,
         jobs: typing.Sequence[int],
         n_processes: int | None = None,
     ) -> None:
+        import concurrent.futures
+        import tqdm
+
+        color = self._get_progress_bar_color()
         with concurrent.futures.ProcessPoolExecutor(n_processes) as executor:
             futures = [executor.submit(self.run_job, i=job) for job in jobs]
-            concurrent.futures.wait(futures)
+            with tqdm.tqdm(total=len(jobs), colour=color) as pbar:
+                for future in concurrent.futures.as_completed(futures):
+                    pbar.update(1)
+
+    def _get_progress_bar_color(self) -> str | None:
+        if self.styles is None:
+            return None
+        else:
+            return self.styles.get('content')
 
     def run_job(self, i: int) -> None:
         self.start_job(i=i)
         self.execute_job(i=i)
         self.end_job(i=i)
 
     def start_job(self, i: int) -> None:
```

### Comparing `tooljob-0.1.3/tooljob/trackers/file_tracker.py` & `tooljob-0.1.4/tooljob/trackers/file_tracker.py`

 * *Files 12% similar despite different names*

```diff
@@ -53,25 +53,14 @@
 
     def get_job_output_path(
         self, i: int | None = None, *, job_data: spec.JobData | None = None
     ) -> str:
         filename = self.get_job_output_filename(i=i, job_data=job_data)
         return os.path.join(self.output_dir, filename)
 
-    def get_job_output_file_names(self) -> typing.Sequence[str]:
-        return [
-            self.get_job_output_filename(i)
-            for i in range(self.batch.get_n_jobs())
-        ]
-
-    def get_job_output_paths(self) -> typing.Sequence[str]:
-        return [
-            self.get_job_output_path(i) for i in range(self.batch.get_n_jobs())
-        ]
-
     def parse_job_output_path(self, path: str) -> typing.Any:
         job_name, ext = os.path.splitext(os.path.basename(path))
         return self.batch.parse_job_name(job_name)
 
     #
     # # sumary methods
     #
@@ -89,14 +78,14 @@
             return os.path.getmtime(path)
         else:
             return None
 
     def print_status(self) -> None:
         import toolstr
 
-        dirsize = 0
-        for f in os.listdir(self.output_dir):
-            path = os.path.join(self.output_dir, f)
+        total_size = 0
+        for i in range(self.batch.get_n_jobs()):
+            path = self.get_job_output_path(i)
             if os.path.isfile(path):
-                dirsize += os.path.getsize(path)
-        print('- output_dir size:', toolstr.format_nbytes(dirsize))
+                total_size = os.path.getsize(path)
+        print('- output_dir size:', toolstr.format_nbytes(total_size))
```

### Comparing `tooljob-0.1.3/tooljob/trackers/sql_tracker.py` & `tooljob-0.1.4/tooljob/trackers/sql_tracker.py`

 * *Files identical despite different names*

### Comparing `tooljob-0.1.3/tooljob/trackers/tracker.py` & `tooljob-0.1.4/tooljob/trackers/tracker.py`

 * *Files identical despite different names*

### Comparing `tooljob-0.1.3/tooljob/trackers/tracker_utils.py` & `tooljob-0.1.4/tooljob/trackers/tracker_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,28 +3,39 @@
 import typing
 
 if typing.TYPE_CHECKING:
 
     import toolsql
 
     from .. import batch_class
+    from .. import spec
     from . import tracker
 
 
 def create_tracker(
     tracker: str | None = None,
+    *,
     output_dir: str | None = None,
     output_filetype: str | None = None,
+    outputs: spec.ShorthandOutputsSpec | None = None,
     db_config: toolsql.DBConfig | None = None,
     bucket_path: str | None = None,
     batch: batch_class.Batch | None = None,
 ) -> tracker.Tracker:
 
+    # determine tracker
     if tracker is None:
-        pass
+        if output_dir is not None and output_filetype is not None:
+            tracker = 'file'
+        elif db_config is not None:
+            tracker = 'sql'
+        elif bucket_path is not None:
+            tracker = 'bucket'
+        else:
+            raise Exception('invalid tracker: ' + str(tracker))
 
     if tracker == 'file':
         from . import file_tracker
 
         assert (
             output_dir is not None
         ), 'must specify output_dir for file tracker'
@@ -34,27 +45,41 @@
 
         return file_tracker.FileTracker(
             batch=batch,
             output_dir=output_dir,
             output_filetype=output_filetype,
         )
 
+    elif tracker == 'multifile':
+        from . import multifile_tracker
+
+        assert outputs is not None, 'must specify outputs for MultifileTracker'
+
+        return multifile_tracker.MultifileTracker(
+            batch=batch,
+            outputs=outputs,
+            output_dir=output_dir,
+            output_filetype=output_filetype,
+        )
+
     elif tracker == 'sql':
         from . import sql_tracker
 
         assert db_config is not None, 'must specify db_config for sql tracker'
 
         return sql_tracker.SqlTracker(
             batch=batch,
             db_config=db_config,
         )
 
     elif tracker == 'bucket':
         from . import bucket_tracker
 
+        raise NotImplementedError('bucket tracker')
+
         assert (
             bucket_path is not None
         ), 'must specify bucket_path for bucket tracker'
 
         return bucket_tracker.BucketTracker(
             batch=batch,
             bucket_path=bucket_path,
```

