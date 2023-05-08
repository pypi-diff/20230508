# Comparing `tmp/graphsignal-0.9.4.tar.gz` & `tmp/graphsignal-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphsignal-0.9.4.tar", last modified: Sat Jul 23 09:51:08 2022, max compression
+gzip compressed data, was "graphsignal-0.9.5.tar", last modified: Sun Aug  7 12:36:50 2022, max compression
```

## Comparing `graphsignal-0.9.4.tar` & `graphsignal-0.9.5.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-23 09:51:08.033145 graphsignal-0.9.4/
--rw-r--r--   0 root         (0) root         (0)    11356 2022-01-21 07:45:21.000000 graphsignal-0.9.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)       49 2022-01-21 07:45:21.000000 graphsignal-0.9.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      220 2022-06-18 08:45:17.000000 graphsignal-0.9.4/NOTICE
--rw-r--r--   0 root         (0) root         (0)     8493 2022-07-23 09:51:08.033145 graphsignal-0.9.4/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     7438 2022-07-22 09:07:23.000000 graphsignal-0.9.4/README.md
--rw-r--r--   0 root         (0) root         (0)     8510 2022-07-23 09:50:32.000000 graphsignal-0.9.4/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-23 09:51:08.017146 graphsignal-0.9.4/graphsignal/
--rw-rw-r--   0 root         (0) root         (0)     6589 2022-07-22 09:06:35.000000 graphsignal-0.9.4/graphsignal/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      423 2022-07-17 06:51:12.000000 graphsignal-0.9.4/graphsignal/agent.py
--rw-rw-r--   0 root         (0) root         (0)     2271 2022-07-17 06:53:10.000000 graphsignal-0.9.4/graphsignal/graphsignal_test.py
--rw-rw-r--   0 root         (0) root         (0)     6082 2022-07-23 08:47:12.000000 graphsignal-0.9.4/graphsignal/inference_span.py
--rw-rw-r--   0 root         (0) root         (0)     5773 2022-07-23 08:49:19.000000 graphsignal-0.9.4/graphsignal/inference_span_test.py
--rw-r--r--   0 root         (0) root         (0)     1787 2022-07-20 12:16:12.000000 graphsignal-0.9.4/graphsignal/profile_scheduler.py
--rw-rw-r--   0 root         (0) root         (0)     1886 2022-07-10 05:30:19.000000 graphsignal-0.9.4/graphsignal/profile_scheduler_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-23 09:51:08.029145 graphsignal-0.9.4/graphsignal/profilers/
--rw-r--r--   0 root         (0) root         (0)        0 2021-12-04 12:55:49.000000 graphsignal-0.9.4/graphsignal/profilers/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2283 2022-07-11 13:45:23.000000 graphsignal-0.9.4/graphsignal/profilers/generic.py
--rw-rw-r--   0 root         (0) root         (0)     1489 2022-07-22 13:02:29.000000 graphsignal-0.9.4/graphsignal/profilers/generic_test.py
--rw-rw-r--   0 root         (0) root         (0)     1578 2022-07-22 13:03:01.000000 graphsignal-0.9.4/graphsignal/profilers/huggingface_generator_test.py
--rw-rw-r--   0 root         (0) root         (0)     3318 2022-07-22 13:03:05.000000 graphsignal-0.9.4/graphsignal/profilers/huggingface_subclass_test.py
--rw-rw-r--   0 root         (0) root         (0)     2160 2022-07-11 13:45:20.000000 graphsignal-0.9.4/graphsignal/profilers/jax.py
--rw-rw-r--   0 root         (0) root         (0)     2315 2022-07-22 13:02:54.000000 graphsignal-0.9.4/graphsignal/profilers/jax_test.py
--rw-rw-r--   0 root         (0) root         (0)     2732 2022-07-19 19:12:38.000000 graphsignal-0.9.4/graphsignal/profilers/keras.py
--rw-rw-r--   0 root         (0) root         (0)     3629 2022-07-22 13:02:46.000000 graphsignal-0.9.4/graphsignal/profilers/keras_test.py
--rw-rw-r--   0 root         (0) root         (0)     3686 2022-07-22 10:57:58.000000 graphsignal-0.9.4/graphsignal/profilers/onnxruntime.py
--rw-rw-r--   0 root         (0) root         (0)     2392 2022-07-22 13:04:28.000000 graphsignal-0.9.4/graphsignal/profilers/onnxruntime_test.py
--rw-rw-r--   0 root         (0) root         (0)      179 2022-07-11 13:45:54.000000 graphsignal-0.9.4/graphsignal/profilers/operation_profiler.py
--rw-rw-r--   0 root         (0) root         (0)     4234 2022-06-29 13:20:11.000000 graphsignal-0.9.4/graphsignal/profilers/profiler_utils.py
--rw-rw-r--   0 root         (0) root         (0)     6734 2022-07-17 06:48:44.000000 graphsignal-0.9.4/graphsignal/profilers/pytorch.py
--rw-rw-r--   0 root         (0) root         (0)     5471 2022-07-22 10:19:44.000000 graphsignal-0.9.4/graphsignal/profilers/pytorch_lightning.py
--rw-rw-r--   0 root         (0) root         (0)     5105 2022-07-22 13:04:03.000000 graphsignal-0.9.4/graphsignal/profilers/pytorch_lightning_test.py
--rw-rw-r--   0 root         (0) root         (0)     2209 2022-07-22 13:03:26.000000 graphsignal-0.9.4/graphsignal/profilers/pytorch_test.py
--rw-rw-r--   0 root         (0) root         (0)     3750 2022-07-17 06:48:44.000000 graphsignal-0.9.4/graphsignal/profilers/tensorflow.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-23 09:51:08.029145 graphsignal-0.9.4/graphsignal/profilers/tensorflow_proto/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-02-22 14:23:17.000000 graphsignal-0.9.4/graphsignal/profilers/tensorflow_proto/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1411 2022-07-23 08:48:54.000000 graphsignal-0.9.4/graphsignal/profilers/tensorflow_proto/diagnostics_pb2.py
--rw-r--r--   0 root         (0) root         (0)     9933 2022-07-23 08:48:54.000000 graphsignal-0.9.4/graphsignal/profilers/tensorflow_proto/input_pipeline_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2512 2022-07-23 08:48:54.000000 graphsignal-0.9.4/graphsignal/profilers/tensorflow_proto/kernel_stats_pb2.py
--rw-r--r--   0 root         (0) root         (0)     8314 2022-07-23 08:48:54.000000 graphsignal-0.9.4/graphsignal/profilers/tensorflow_proto/memory_profile_pb2.py
--rw-r--r--   0 root         (0) root         (0)    11719 2022-07-23 08:48:54.000000 graphsignal-0.9.4/graphsignal/profilers/tensorflow_proto/overview_page_pb2.py
--rw-r--r--   0 root         (0) root         (0)     3719 2022-07-23 08:48:54.000000 graphsignal-0.9.4/graphsignal/profilers/tensorflow_proto/tf_stats_pb2.py
--rw-rw-r--   0 root         (0) root         (0)     2471 2022-07-22 13:03:45.000000 graphsignal-0.9.4/graphsignal/profilers/tensorflow_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-23 09:51:08.029145 graphsignal-0.9.4/graphsignal/proto/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-03-07 12:20:05.000000 graphsignal-0.9.4/graphsignal/proto/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    17644 2022-07-23 08:48:54.000000 graphsignal-0.9.4/graphsignal/proto/profiles_pb2.py
--rw-r--r--   0 root         (0) root         (0)      979 2022-06-03 09:19:36.000000 graphsignal-0.9.4/graphsignal/proto_utils.py
--rw-rw-r--   0 root         (0) root         (0)     1308 2022-04-30 06:03:21.000000 graphsignal-0.9.4/graphsignal/proto_utils_test.py
--rw-r--r--   0 root         (0) root         (0)     3948 2022-06-27 12:33:38.000000 graphsignal-0.9.4/graphsignal/uploader.py
--rw-rw-r--   0 root         (0) root         (0)     4899 2022-04-26 14:46:30.000000 graphsignal-0.9.4/graphsignal/uploader_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-23 09:51:08.033145 graphsignal-0.9.4/graphsignal/usage/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-03-07 11:27:25.000000 graphsignal-0.9.4/graphsignal/usage/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8382 2022-07-21 13:39:11.000000 graphsignal-0.9.4/graphsignal/usage/nvml_reader.py
--rw-rw-r--   0 root         (0) root         (0)     2438 2022-07-05 08:53:12.000000 graphsignal-0.9.4/graphsignal/usage/nvml_reader_test.py
--rw-rw-r--   0 root         (0) root         (0)     6511 2022-07-23 08:45:39.000000 graphsignal-0.9.4/graphsignal/usage/process_reader.py
--rw-rw-r--   0 root         (0) root         (0)     1864 2022-07-23 08:46:02.000000 graphsignal-0.9.4/graphsignal/usage/process_reader_test.py
--rw-rw-r--   0 root         (0) root         (0)    59003 2022-07-05 11:18:16.000000 graphsignal-0.9.4/graphsignal/usage/pynvml.py
--rw-rw-r--   0 root         (0) root         (0)       22 2022-07-18 08:50:32.000000 graphsignal-0.9.4/graphsignal/version.py
--rw-rw-r--   0 root         (0) root         (0)     5101 2022-07-23 03:15:06.000000 graphsignal-0.9.4/graphsignal/workload_run.py
--rw-rw-r--   0 root         (0) root         (0)     1567 2022-07-23 03:18:50.000000 graphsignal-0.9.4/graphsignal/workload_run_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-23 09:51:08.021146 graphsignal-0.9.4/graphsignal.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8493 2022-07-23 09:51:07.000000 graphsignal-0.9.4/graphsignal.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2064 2022-07-23 09:51:07.000000 graphsignal-0.9.4/graphsignal.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-23 09:51:07.000000 graphsignal-0.9.4/graphsignal.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2022-07-23 09:51:07.000000 graphsignal-0.9.4/graphsignal.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2022-07-23 09:51:07.000000 graphsignal-0.9.4/graphsignal.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       67 2022-07-23 09:51:08.037145 graphsignal-0.9.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1485 2022-07-07 16:48:59.000000 graphsignal-0.9.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-07 12:36:50.632622 graphsignal-0.9.5/
+-rw-r--r--   0 root         (0) root         (0)    11356 2022-01-21 07:45:21.000000 graphsignal-0.9.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       49 2022-01-21 07:45:21.000000 graphsignal-0.9.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      220 2022-06-18 08:45:17.000000 graphsignal-0.9.5/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     8483 2022-08-07 12:36:50.632622 graphsignal-0.9.5/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     7428 2022-07-23 12:31:40.000000 graphsignal-0.9.5/README.md
+-rw-r--r--   0 root         (0) root         (0)     8500 2022-08-07 12:36:13.000000 graphsignal-0.9.5/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-07 12:36:50.608622 graphsignal-0.9.5/graphsignal/
+-rw-rw-r--   0 root         (0) root         (0)     6589 2022-07-22 09:06:35.000000 graphsignal-0.9.5/graphsignal/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      423 2022-07-17 06:51:12.000000 graphsignal-0.9.5/graphsignal/agent.py
+-rw-rw-r--   0 root         (0) root         (0)     2271 2022-07-17 06:53:10.000000 graphsignal-0.9.5/graphsignal/graphsignal_test.py
+-rw-rw-r--   0 root         (0) root         (0)     6629 2022-08-07 12:29:02.000000 graphsignal-0.9.5/graphsignal/inference_span.py
+-rw-rw-r--   0 root         (0) root         (0)     6861 2022-07-27 10:46:02.000000 graphsignal-0.9.5/graphsignal/inference_span_test.py
+-rw-r--r--   0 root         (0) root         (0)     1787 2022-07-20 12:16:12.000000 graphsignal-0.9.5/graphsignal/profile_scheduler.py
+-rw-rw-r--   0 root         (0) root         (0)     1886 2022-07-10 05:30:19.000000 graphsignal-0.9.5/graphsignal/profile_scheduler_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-07 12:36:50.628622 graphsignal-0.9.5/graphsignal/profilers/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-12-04 12:55:49.000000 graphsignal-0.9.5/graphsignal/profilers/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2283 2022-07-11 13:45:23.000000 graphsignal-0.9.5/graphsignal/profilers/generic.py
+-rw-rw-r--   0 root         (0) root         (0)     1489 2022-07-22 13:02:29.000000 graphsignal-0.9.5/graphsignal/profilers/generic_test.py
+-rw-rw-r--   0 root         (0) root         (0)     1567 2022-07-23 12:32:10.000000 graphsignal-0.9.5/graphsignal/profilers/huggingface_pipeline_test.py
+-rw-rw-r--   0 root         (0) root         (0)     3318 2022-07-22 13:03:05.000000 graphsignal-0.9.5/graphsignal/profilers/huggingface_subclass_test.py
+-rw-rw-r--   0 root         (0) root         (0)     2160 2022-07-11 13:45:20.000000 graphsignal-0.9.5/graphsignal/profilers/jax.py
+-rw-rw-r--   0 root         (0) root         (0)     2315 2022-07-22 13:02:54.000000 graphsignal-0.9.5/graphsignal/profilers/jax_test.py
+-rw-rw-r--   0 root         (0) root         (0)     2732 2022-07-19 19:12:38.000000 graphsignal-0.9.5/graphsignal/profilers/keras.py
+-rw-rw-r--   0 root         (0) root         (0)     3629 2022-07-22 13:02:46.000000 graphsignal-0.9.5/graphsignal/profilers/keras_test.py
+-rw-rw-r--   0 root         (0) root         (0)     3686 2022-07-22 10:57:58.000000 graphsignal-0.9.5/graphsignal/profilers/onnxruntime.py
+-rw-rw-r--   0 root         (0) root         (0)     2392 2022-07-22 13:04:28.000000 graphsignal-0.9.5/graphsignal/profilers/onnxruntime_test.py
+-rw-rw-r--   0 root         (0) root         (0)      179 2022-07-11 13:45:54.000000 graphsignal-0.9.5/graphsignal/profilers/operation_profiler.py
+-rw-rw-r--   0 root         (0) root         (0)     4173 2022-07-27 11:46:50.000000 graphsignal-0.9.5/graphsignal/profilers/profiler_utils.py
+-rw-rw-r--   0 root         (0) root         (0)     6734 2022-07-17 06:48:44.000000 graphsignal-0.9.5/graphsignal/profilers/pytorch.py
+-rw-rw-r--   0 root         (0) root         (0)     5471 2022-07-22 10:19:44.000000 graphsignal-0.9.5/graphsignal/profilers/pytorch_lightning.py
+-rw-rw-r--   0 root         (0) root         (0)     5105 2022-07-22 13:04:03.000000 graphsignal-0.9.5/graphsignal/profilers/pytorch_lightning_test.py
+-rw-rw-r--   0 root         (0) root         (0)     2209 2022-07-22 13:03:26.000000 graphsignal-0.9.5/graphsignal/profilers/pytorch_test.py
+-rw-rw-r--   0 root         (0) root         (0)     3750 2022-07-17 06:48:44.000000 graphsignal-0.9.5/graphsignal/profilers/tensorflow.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-07 12:36:50.628622 graphsignal-0.9.5/graphsignal/profilers/tensorflow_proto/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-02-22 14:23:17.000000 graphsignal-0.9.5/graphsignal/profilers/tensorflow_proto/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1411 2022-07-27 10:45:32.000000 graphsignal-0.9.5/graphsignal/profilers/tensorflow_proto/diagnostics_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     9933 2022-07-27 10:45:32.000000 graphsignal-0.9.5/graphsignal/profilers/tensorflow_proto/input_pipeline_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2512 2022-07-27 10:45:32.000000 graphsignal-0.9.5/graphsignal/profilers/tensorflow_proto/kernel_stats_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     8314 2022-07-27 10:45:32.000000 graphsignal-0.9.5/graphsignal/profilers/tensorflow_proto/memory_profile_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    11719 2022-07-27 10:45:32.000000 graphsignal-0.9.5/graphsignal/profilers/tensorflow_proto/overview_page_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3719 2022-07-27 10:45:32.000000 graphsignal-0.9.5/graphsignal/profilers/tensorflow_proto/tf_stats_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)     2471 2022-07-22 13:03:45.000000 graphsignal-0.9.5/graphsignal/profilers/tensorflow_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-07 12:36:50.632622 graphsignal-0.9.5/graphsignal/proto/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-03-07 12:20:05.000000 graphsignal-0.9.5/graphsignal/proto/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    18207 2022-07-27 10:45:32.000000 graphsignal-0.9.5/graphsignal/proto/profiles_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      979 2022-06-03 09:19:36.000000 graphsignal-0.9.5/graphsignal/proto_utils.py
+-rw-rw-r--   0 root         (0) root         (0)     1308 2022-04-30 06:03:21.000000 graphsignal-0.9.5/graphsignal/proto_utils_test.py
+-rw-r--r--   0 root         (0) root         (0)     3948 2022-06-27 12:33:38.000000 graphsignal-0.9.5/graphsignal/uploader.py
+-rw-rw-r--   0 root         (0) root         (0)     4899 2022-04-26 14:46:30.000000 graphsignal-0.9.5/graphsignal/uploader_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-07 12:36:50.632622 graphsignal-0.9.5/graphsignal/usage/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-03-07 11:27:25.000000 graphsignal-0.9.5/graphsignal/usage/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8382 2022-07-25 10:20:46.000000 graphsignal-0.9.5/graphsignal/usage/nvml_reader.py
+-rw-rw-r--   0 root         (0) root         (0)     2438 2022-07-05 08:53:12.000000 graphsignal-0.9.5/graphsignal/usage/nvml_reader_test.py
+-rw-rw-r--   0 root         (0) root         (0)     6511 2022-07-23 08:45:39.000000 graphsignal-0.9.5/graphsignal/usage/process_reader.py
+-rw-rw-r--   0 root         (0) root         (0)     1864 2022-07-23 08:46:02.000000 graphsignal-0.9.5/graphsignal/usage/process_reader_test.py
+-rw-rw-r--   0 root         (0) root         (0)    59003 2022-07-05 11:18:16.000000 graphsignal-0.9.5/graphsignal/usage/pynvml.py
+-rw-rw-r--   0 root         (0) root         (0)       22 2022-07-23 12:32:19.000000 graphsignal-0.9.5/graphsignal/version.py
+-rw-rw-r--   0 root         (0) root         (0)     5101 2022-07-23 03:15:06.000000 graphsignal-0.9.5/graphsignal/workload_run.py
+-rw-rw-r--   0 root         (0) root         (0)     1567 2022-07-23 03:18:50.000000 graphsignal-0.9.5/graphsignal/workload_run_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-07 12:36:50.612622 graphsignal-0.9.5/graphsignal.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8483 2022-08-07 12:36:50.000000 graphsignal-0.9.5/graphsignal.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2063 2022-08-07 12:36:50.000000 graphsignal-0.9.5/graphsignal.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-08-07 12:36:50.000000 graphsignal-0.9.5/graphsignal.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2022-08-07 12:36:50.000000 graphsignal-0.9.5/graphsignal.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2022-08-07 12:36:50.000000 graphsignal-0.9.5/graphsignal.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       67 2022-08-07 12:36:50.632622 graphsignal-0.9.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1485 2022-07-07 16:48:59.000000 graphsignal-0.9.5/setup.py
```

### Comparing `graphsignal-0.9.4/LICENSE` & `graphsignal-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `graphsignal-0.9.4/PKG-INFO` & `graphsignal-0.9.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphsignal
-Version: 0.9.4
+Version: 0.9.5
 Summary: Graphsignal Profiler
 Home-page: https://graphsignal.com
 Author: Graphsignal, Inc.
 Author-email: devops@graphsignal.com
 License: Apache-2.0
 Keywords: machine learning,deep learning,data science,machine learning profiler,deep learning profiler,tensorflow profiler,keras profiler,pytorch profiler,inference profiling
 Platform: UNKNOWN
@@ -131,18 +131,18 @@
 #### [Hugging Face](https://graphsignal.com/docs/integrations/hugging-face/)
 
 ```python
 from transformers import pipeline
 from graphsignal.profilers.pytorch import profile_inference
 # or from graphsignal.profilers.tensorflow import profile_inference
 
-generator = pipeline(task="text-generation")
+pipe = pipeline(task="text-generation")
 
 with profile_inference():
-    output = generator('some text')
+    output = pipe('some text')
 ```
 
 #### [JAX](https://graphsignal.com/docs/integrations/jax/)
 
 ```python
 from graphsignal.profilers.jax import profile_inference
```

### Comparing `graphsignal-0.9.4/README.md` & `graphsignal-0.9.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -105,18 +105,18 @@
 #### [Hugging Face](https://graphsignal.com/docs/integrations/hugging-face/)
 
 ```python
 from transformers import pipeline
 from graphsignal.profilers.pytorch import profile_inference
 # or from graphsignal.profilers.tensorflow import profile_inference
 
-generator = pipeline(task="text-generation")
+pipe = pipeline(task="text-generation")
 
 with profile_inference():
-    output = generator('some text')
+    output = pipe('some text')
 ```
 
 #### [JAX](https://graphsignal.com/docs/integrations/jax/)
 
 ```python
 from graphsignal.profilers.jax import profile_inference
```

### Comparing `graphsignal-0.9.4/README.rst` & `graphsignal-0.9.5/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -136,18 +136,18 @@
 
 .. code:: python
 
    from transformers import pipeline
    from graphsignal.profilers.pytorch import profile_inference
    # or from graphsignal.profilers.tensorflow import profile_inference
 
-   generator = pipeline(task="text-generation")
+   pipe = pipeline(task="text-generation")
 
    with profile_inference():
-       output = generator('some text')
+       output = pipe('some text')
 
 `JAX <https://graphsignal.com/docs/integrations/jax/>`__
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 .. code:: python
 
    from graphsignal.profilers.jax import profile_inference
```

### Comparing `graphsignal-0.9.4/graphsignal/__init__.py` & `graphsignal-0.9.5/graphsignal/__init__.py`

 * *Files identical despite different names*

### Comparing `graphsignal-0.9.4/graphsignal/graphsignal_test.py` & `graphsignal-0.9.5/graphsignal/graphsignal_test.py`

 * *Files identical despite different names*

### Comparing `graphsignal-0.9.4/graphsignal/inference_span.py` & `graphsignal-0.9.5/graphsignal/inference_span.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         '_operation_profiler',
         '_context',
         '_is_scheduled',
         '_is_profiling',
         '_profile',
         '_stop_lock',
         '_batch_size',
-        '_start_us',
+        '_start_counter',
         '_metrics'
     ]
 
     def __init__(self, 
             batch_size=None, 
             ensure_profile=False, 
             operation_profiler=None,
@@ -40,15 +40,15 @@
         self._stop_lock = Lock()
         self._metrics = None
 
         current_run = graphsignal.current_run()
 
         if current_run.profile_scheduler.lock(ensure=ensure_profile):
             if logger.isEnabledFor(logging.DEBUG):
-                profiling_start_ts = time.time()
+                profiling_start_overhead_counter = time.perf_counter()
 
             self._is_scheduled = True
             self._profile = profiles_pb2.MLProfile()
             self._profile.workload_name = graphsignal._agent.workload_name
             self._profile.worker_id = graphsignal._agent.worker_id
             self._profile.run_id = graphsignal.current_run().run_id
             self._profile.run_start_ms = graphsignal.current_run().start_ms
@@ -72,62 +72,64 @@
                     self._is_profiling = False
                     self._add_profiler_exception(exc)
                     logger.error('Error starting profiler', exc_info=True)
 
             self._profile.start_us = _timestamp_us()
 
             if logger.isEnabledFor(logging.DEBUG):
-                logger.debug('Profiling start took: %fs', time.time() - profiling_start_ts)
+                logger.debug('Profiling start took: %fs', time.perf_counter() - profiling_start_overhead_counter)
 
-        self._start_us = _timestamp_us()
+        self._start_counter = time.perf_counter()
 
     def __enter__(self):
         return self
 
-    def __exit__(self, *exc):
-        self.stop()
+    def __exit__(self, *exc_info):
+        self.stop(exc_info=exc_info)
 
-    def stop(self) -> None:
-        stop_us = _timestamp_us()
+    def stop(self, exc_info=None) -> None:
+        stop_counter = time.perf_counter()
 
         with self._stop_lock:
             if self._is_scheduled:
+                self._profile.end_us = _timestamp_us()
+
                 if self._is_profiling:
                     try:
                         self._operation_profiler.stop(self._profile, self._context)
                     except Exception as exc:
                         logger.error('Error stopping profiler', exc_info=True)
                         self._add_profiler_exception(exc)
 
             current_run = graphsignal.current_run()
-
             current_run.inc_total_inference_count()
 
             # only measure if not profiling to exclude spans with profiler overhead
             if not self._is_profiling:
                 current_run.update_inference_stats(
-                    stop_us - self._start_us,
+                    int((stop_counter - self._start_counter) * 1e6),
                     batch_size=self._batch_size)
 
             if self._is_scheduled:
                 if logger.isEnabledFor(logging.DEBUG):
-                    profiling_stop_ts = time.time()
-
-                self._profile.end_us = stop_us
+                    profiling_stop_overhead_counter = time.perf_counter()
 
                 self._profile.inference_stats.inference_count = current_run.total_inference_count
                 stats = current_run.inference_stats
                 self._profile.inference_stats.inference_time_p95_us = stats.inference_time_p95_us()
                 self._profile.inference_stats.inference_time_avg_us = stats.inference_time_avg_us()
                 self._profile.inference_stats.inference_rate = stats.inference_rate()
                 self._profile.inference_stats.sample_rate = stats.sample_rate()
                 if self._batch_size:
                     self._profile.inference_stats.batch_size = self._batch_size
                 current_run.reset_inference_stats()
 
+                if exc_info and exc_info[1]:
+                    self._add_inference_exception(exc_info)
+
                 try:
                     graphsignal._agent.process_reader.read(self._profile)
                     graphsignal._agent.nvml_reader.read(self._profile)
                 except Exception as exc:
                     logger.error('Error reading usage information', exc_info=True)
                     self._add_profiler_exception(exc)
 
@@ -135,26 +137,33 @@
 
                 self._is_scheduled = False
                 self._is_profiling = False
                 self._profile = None
                 current_run.profile_scheduler.unlock()
 
                 if logger.isEnabledFor(logging.DEBUG):
-                    logger.debug('Profiling stop took: %fs', time.time() - profiling_stop_ts)
+                    logger.debug('Profiling stop took: %fs', time.perf_counter() - profiling_stop_overhead_counter)
 
     def set_batch_size(self, batch_size: int) -> None:
         if not isinstance(batch_size, int):
             raise ValueError('Invalid batch_size')
         self._batch_size = batch_size
 
+    def _add_inference_exception(self, exc_info):
+        exception = self._profile.exceptions.add()
+        exception.message = str(exc_info[1])
+        if exc_info[2]:
+            frames = traceback.format_tb(exc_info[2])
+            if len(frames) > 0:
+                exception.stack_trace = ''.join(frames)
+
     def _add_profiler_exception(self, exc):
-        if self._profile:
-            profiler_error = self._profile.profiler_errors.add()
-            profiler_error.message = str(exc)
-            if exc.__traceback__:
-                frames = traceback.format_tb(exc.__traceback__)
-                if len(frames) > 0:
-                    profiler_error.stack_trace = ''.join(frames)
+        profiler_error = self._profile.profiler_errors.add()
+        profiler_error.message = str(exc)
+        if exc.__traceback__:
+            frames = traceback.format_tb(exc.__traceback__)
+            if len(frames) > 0:
+                profiler_error.stack_trace = ''.join(frames)
 
 
 def _timestamp_us():
     return int(time.time() * 1e6)
```

### Comparing `graphsignal-0.9.4/graphsignal/inference_span_test.py` & `graphsignal-0.9.5/graphsignal/inference_span_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -115,15 +115,15 @@
         self.assertNotEqual(profile.profiler_errors[0].stack_trace, '')
 
     @patch.object(TensorflowProfiler, 'start', return_value=True)
     @patch.object(TensorflowProfiler, 'stop', return_value=True)
     @patch.object(ProcessReader, 'read')
     @patch.object(NvmlReader, 'read')
     @patch.object(Uploader, 'upload_profile')
-    def test_stop_exception(self, mocked_upload_profile, mocked_nvml_read, mocked_host_read,
+    def test_profiler_exception(self, mocked_upload_profile, mocked_nvml_read, mocked_host_read,
                             mocked_stop, mocked_start):
         mocked_stop.side_effect = Exception('ex1')
         span = InferenceSpan(
             ensure_profile=True,
             operation_profiler=TensorflowProfiler())
         span.stop()
 
@@ -134,7 +134,33 @@
 
         self.assertEqual(profile.workload_name, 'w1')
         self.assertTrue(profile.worker_id != '')
         self.assertTrue(profile.start_us > 0)
         self.assertTrue(profile.end_us > 0)
         self.assertEqual(profile.profiler_errors[0].message, 'ex1')
         self.assertNotEqual(profile.profiler_errors[0].stack_trace, '')
+
+    @patch.object(TensorflowProfiler, 'start', return_value=True)
+    @patch.object(TensorflowProfiler, 'stop', return_value=True)
+    @patch.object(ProcessReader, 'read')
+    @patch.object(NvmlReader, 'read')
+    @patch.object(Uploader, 'upload_profile')
+    def test_inference_exception(self, mocked_upload_profile, mocked_nvml_read, mocked_host_read,
+                            mocked_stop, mocked_start):
+
+        try:
+            with InferenceSpan(ensure_profile=True, operation_profiler=TensorflowProfiler()):
+                raise Exception('ex1')
+        except:
+            pass
+
+        graphsignal.upload()
+        mocked_start.assert_called_once()
+        mocked_stop.assert_called_once()
+        profile = mocked_upload_profile.call_args[0][0]
+
+        self.assertEqual(profile.workload_name, 'w1')
+        self.assertTrue(profile.worker_id != '')
+        self.assertTrue(profile.start_us > 0)
+        self.assertTrue(profile.end_us > 0)
+        self.assertEqual(profile.exceptions[0].message, 'ex1')
+        self.assertNotEqual(profile.exceptions[0].stack_trace, '')
```

### Comparing `graphsignal-0.9.4/graphsignal/profile_scheduler.py` & `graphsignal-0.9.5/graphsignal/profile_scheduler.py`

 * *Files identical despite different names*

### Comparing `graphsignal-0.9.4/graphsignal/profile_scheduler_test.py` & `graphsignal-0.9.5/graphsignal/profile_scheduler_test.py`

 * *Files identical despite different names*

### Comparing `graphsignal-0.9.4/graphsignal/profilers/generic.py` & `graphsignal-0.9.5/graphsignal/profilers/generic.py`

 * *Files identical despite different names*

### Comparing `graphsignal-0.9.4/graphsignal/profilers/generic_test.py` & `graphsignal-0.9.5/graphsignal/profilers/generic_test.py`

 * *Files identical despite different names*

### Comparing `graphsignal-0.9.4/graphsignal/profilers/huggingface_generator_test.py` & `graphsignal-0.9.5/graphsignal/profilers/huggingface_pipeline_test.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,22 +21,22 @@
             workload_name='w1',
             debug_mode=True)
 
     def tearDown(self):
         graphsignal.shutdown()
 
     @patch.object(Uploader, 'upload_profile')
-    def test_generator(self, mocked_upload_profile):
+    def test_pipeline(self, mocked_upload_profile):
         from transformers import pipeline
         from graphsignal.profilers.pytorch import profile_inference
 
-        generator = pipeline(task="text-generation", model='distilgpt2')
+        pipe = pipeline(task="text-generation", model='distilgpt2')
 
         with profile_inference():
-            output = generator('some text')
+            output = pipe('some text')
 
         graphsignal.upload()
         profile = mocked_upload_profile.call_args[0][0]
 
         #pp = pprint.PrettyPrinter()
         #pp.pprint(MessageToJson(profile))
```

### Comparing `graphsignal-0.9.4/graphsignal/profilers/huggingface_subclass_test.py` & `graphsignal-0.9.5/graphsignal/profilers/huggingface_subclass_test.py`

 * *Files identical despite different names*

### Comparing `graphsignal-0.9.4/graphsignal/profilers/jax.py` & `graphsignal-0.9.5/graphsignal/profilers/jax.py`

 * *Files identical despite different names*

### Comparing `graphsignal-0.9.4/graphsignal/profilers/jax_test.py` & `graphsignal-0.9.5/graphsignal/profilers/jax_test.py`

 * *Files identical despite different names*

### Comparing `graphsignal-0.9.4/graphsignal/profilers/keras.py` & `graphsignal-0.9.5/graphsignal/profilers/keras.py`

 * *Files identical despite different names*

### Comparing `graphsignal-0.9.4/graphsignal/profilers/keras_test.py` & `graphsignal-0.9.5/graphsignal/profilers/keras_test.py`

 * *Files identical despite different names*

### Comparing `graphsignal-0.9.4/graphsignal/profilers/onnxruntime.py` & `graphsignal-0.9.5/graphsignal/profilers/onnxruntime.py`

 * *Files identical despite different names*

### Comparing `graphsignal-0.9.4/graphsignal/profilers/onnxruntime_test.py` & `graphsignal-0.9.5/graphsignal/profilers/onnxruntime_test.py`

 * *Files identical despite different names*

### Comparing `graphsignal-0.9.4/graphsignal/profilers/profiler_utils.py` & `graphsignal-0.9.5/graphsignal/profilers/profiler_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,19 +23,16 @@
 def remove_log_dir(log_dir):
     shutil.rmtree(log_dir)
     logger.debug('Removed temporary log directory %s', log_dir)
 
 def find_and_read(log_dir, file_pattern, decompress=True, max_size=None):
     file_paths = glob.glob(os.path.join(log_dir, file_pattern))
     if len(file_paths) == 0:
-        raise Exception(
-            'Files are not found at {}'.format(
-                os.path.join(
-                    log_dir,
-                    file_pattern)))
+        logger.debug('Files are not found at %s', os.path.join(log_dir, file_pattern))
+        return None
 
     found_path = file_paths[-1]
 
     if max_size:
         if os.path.getsize(found_path) > max_size:
             raise Exception('File is too big: {0}'.format())
```

### Comparing `graphsignal-0.9.4/graphsignal/profilers/pytorch.py` & `graphsignal-0.9.5/graphsignal/profilers/pytorch.py`

 * *Files identical despite different names*

### Comparing `graphsignal-0.9.4/graphsignal/profilers/pytorch_lightning.py` & `graphsignal-0.9.5/graphsignal/profilers/pytorch_lightning.py`

 * *Files identical despite different names*

### Comparing `graphsignal-0.9.4/graphsignal/profilers/pytorch_lightning_test.py` & `graphsignal-0.9.5/graphsignal/profilers/pytorch_lightning_test.py`

 * *Files identical despite different names*

### Comparing `graphsignal-0.9.4/graphsignal/profilers/pytorch_test.py` & `graphsignal-0.9.5/graphsignal/profilers/pytorch_test.py`

 * *Files identical despite different names*

### Comparing `graphsignal-0.9.4/graphsignal/profilers/tensorflow.py` & `graphsignal-0.9.5/graphsignal/profilers/tensorflow.py`

 * *Files identical despite different names*

### Comparing `graphsignal-0.9.4/graphsignal/profilers/tensorflow_proto/diagnostics_pb2.py` & `graphsignal-0.9.5/graphsignal/profilers/tensorflow_proto/diagnostics_pb2.py`

 * *Files identical despite different names*

### Comparing `graphsignal-0.9.4/graphsignal/profilers/tensorflow_proto/input_pipeline_pb2.py` & `graphsignal-0.9.5/graphsignal/profilers/tensorflow_proto/input_pipeline_pb2.py`

 * *Files identical despite different names*

### Comparing `graphsignal-0.9.4/graphsignal/profilers/tensorflow_proto/kernel_stats_pb2.py` & `graphsignal-0.9.5/graphsignal/profilers/tensorflow_proto/kernel_stats_pb2.py`

 * *Files identical despite different names*

### Comparing `graphsignal-0.9.4/graphsignal/profilers/tensorflow_proto/memory_profile_pb2.py` & `graphsignal-0.9.5/graphsignal/profilers/tensorflow_proto/memory_profile_pb2.py`

 * *Files identical despite different names*

### Comparing `graphsignal-0.9.4/graphsignal/profilers/tensorflow_proto/overview_page_pb2.py` & `graphsignal-0.9.5/graphsignal/profilers/tensorflow_proto/overview_page_pb2.py`

 * *Files identical despite different names*

### Comparing `graphsignal-0.9.4/graphsignal/profilers/tensorflow_proto/tf_stats_pb2.py` & `graphsignal-0.9.5/graphsignal/profilers/tensorflow_proto/tf_stats_pb2.py`

 * *Files identical despite different names*

### Comparing `graphsignal-0.9.4/graphsignal/profilers/tensorflow_test.py` & `graphsignal-0.9.5/graphsignal/profilers/tensorflow_test.py`

 * *Files identical despite different names*

### Comparing `graphsignal-0.9.4/graphsignal/proto/profiles_pb2.py` & `graphsignal-0.9.5/graphsignal/proto/profiles_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0eprofiles.proto\x12\x14graphsignal.profiles\"X\n\rUploadRequest\x12\x34\n\x0bml_profiles\x18\x01 \x03(\x0b\x32\x1f.graphsignal.profiles.MLProfile\x12\x11\n\tupload_ms\x18\x02 \x01(\x04\"\x10\n\x0eUploadResponse\"\xb0\x01\n\rProfileRecord\x12\x0f\n\x07\x64\x61ta_id\x18\x01 \x01(\t\x12\x13\n\x0bworkload_id\x18\x02 \x01(\t\x12\x12\n\nprofile_id\x18\x03 \x01(\t\x12\x33\n\nml_profile\x18\x04 \x01(\x0b\x32\x1f.graphsignal.profiles.MLProfile\x12\x1a\n\x12\x64\x61ta_retention_sec\x18\x05 \x01(\x04\x12\x14\n\x0ctime_skew_ms\x18\x06 \x01(\x12\"\xa9\x07\n\tMLProfile\x12\x15\n\rworkload_name\x18\x01 \x01(\t\x12\x11\n\tworker_id\x18\x1c \x01(\t\x12\x0e\n\x06run_id\x18\x02 \x01(\t\x12\x14\n\x0crun_start_ms\x18\' \x01(\x04\x12\x10\n\x08start_us\x18\x05 \x01(\x04\x12\x0e\n\x06\x65nd_us\x18\x06 \x01(\x04\x12\'\n\x04tags\x18  \x03(\x0b\x32\x19.graphsignal.profiles.Tag\x12\x37\n\nframeworks\x18$ \x03(\x0b\x32#.graphsignal.profiles.FrameworkInfo\x12+\n\x06params\x18\x16 \x03(\x0b\x32\x1b.graphsignal.profiles.Param\x12-\n\x07metrics\x18\x1e \x03(\x0b\x32\x1c.graphsignal.profiles.Metric\x12=\n\x0finference_stats\x18% \x01(\x0b\x32$.graphsignal.profiles.InferenceStats\x12\x33\n\nmodel_info\x18& \x01(\x0b\x32\x1f.graphsignal.profiles.ModelInfo\x12<\n\ncomm_usage\x18\x1b \x01(\x0b\x32(.graphsignal.profiles.CommunicationUsage\x12\x33\n\nnode_usage\x18\x19 \x01(\x0b\x32\x1f.graphsignal.profiles.NodeUsage\x12\x39\n\rprocess_usage\x18\x1a \x01(\x0b\x32\".graphsignal.profiles.ProcessUsage\x12\x37\n\x0c\x64\x65vice_usage\x18\x12 \x03(\x0b\x32!.graphsignal.profiles.DeviceUsage\x12/\n\x08op_stats\x18\x0b \x03(\x0b\x32\x1d.graphsignal.profiles.OpStats\x12\x37\n\x0ckernel_stats\x18\x0c \x03(\x0b\x32!.graphsignal.profiles.KernelStats\x12\x12\n\ntrace_data\x18! \x01(\x0c\x12\x1a\n\x12is_trace_available\x18\" \x01(\x08\x12\x39\n\rprofiler_info\x18# \x01(\x0b\x32\".graphsignal.profiles.ProfilerInfo\x12<\n\x0fprofiler_errors\x18\x07 \x03(\x0b\x32#.graphsignal.profiles.ProfilerError\"5\n\x06SemVer\x12\r\n\x05major\x18\x01 \x01(\x05\x12\r\n\x05minor\x18\x02 \x01(\x05\x12\r\n\x05patch\x18\x03 \x01(\x05\"\xb8\x02\n\rFrameworkInfo\x12?\n\x04type\x18\x01 \x01(\x0e\x32\x31.graphsignal.profiles.FrameworkInfo.FrameworkType\x12-\n\x07version\x18\x02 \x01(\x0b\x32\x1c.graphsignal.profiles.SemVer\"\xb6\x01\n\rFrameworkType\x12\x17\n\x13\x46RAMEWORK_UNDEFINED\x10\x00\x12\x18\n\x14TENSORFLOW_FRAMEWORK\x10\x01\x12\x15\n\x11PYTORCH_FRAMEWORK\x10\x02\x12\x13\n\x0fKERAS_FRAMEWORK\x10\x03\x12\x1f\n\x1bPYTORCH_LIGHTNING_FRAMEWORK\x10\x04\x12\x11\n\rJAX_FRAMEWORK\x10\x07\x12\x12\n\x0eONNX_FRAMEWORK\x10\t\"\x14\n\x03Tag\x12\r\n\x05value\x18\x01 \x01(\t\"$\n\x05Param\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"%\n\x06Metric\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x01\"\xbc\x01\n\x0eInferenceStats\x12\x17\n\x0finference_count\x18\t \x01(\x04\x12\x1d\n\x15inference_time_p95_us\x18\n \x01(\x01\x12\x1d\n\x15inference_time_avg_us\x18\x0b \x01(\x01\x12\x16\n\x0einference_rate\x18\x0c \x01(\x01\x12\x13\n\x0bsample_rate\x18\r \x01(\x01\x12\x12\n\nbatch_size\x18\x04 \x01(\x05\x12\x12\n\nworld_size\x18\x06 \x01(\x05\"\xb2\x01\n\tModelInfo\x12\x41\n\x0cmodel_format\x18\x01 \x01(\x0e\x32+.graphsignal.profiles.ModelInfo.ModelFormat\x12\x18\n\x10model_size_bytes\x18\x02 \x01(\x04\"H\n\x0bModelFormat\x12\x14\n\x10\x46ORMAT_UNDEFINED\x10\x00\x12\x12\n\x0ePYTORCH_FORMAT\x10\x01\x12\x0f\n\x0bONNX_FORMAT\x10\x02\"\xd5\x01\n\x12\x43ommunicationUsage\x12W\n\x0c\x62\x61\x63kend_type\x18\x01 \x01(\x0e\x32\x41.graphsignal.profiles.CommunicationUsage.CommunicationBackendType\"f\n\x18\x43ommunicationBackendType\x12#\n\x1f\x43OMMUNICATION_BACKEND_UNDEFINED\x10\x00\x12\x08\n\x04NCCL\x10\x01\x12\x08\n\x04GLOO\x10\x02\x12\x07\n\x03MPI\x10\x03\x12\x08\n\x04RING\x10\x04\"\xc6\x01\n\tNodeUsage\x12\x10\n\x08hostname\x18\x01 \x01(\t\x12\x12\n\nip_address\x18\x07 \x01(\t\x12\x11\n\tnode_rank\x18\x08 \x01(\x05\x12\x10\n\x08mem_used\x18\t \x01(\x04\x12\x11\n\tmem_total\x18\n \x01(\x04\x12\x10\n\x08platform\x18\x02 \x01(\t\x12\x0f\n\x07machine\x18\x03 \x01(\t\x12\x0f\n\x07os_name\x18\x04 \x01(\t\x12\x12\n\nos_version\x18\x05 \x01(\t\x12\x13\n\x0bnum_devices\x18\x06 \x01(\x05\"\xf9\x02\n\x0cProcessUsage\x12\x12\n\nprocess_id\x18\x05 \x01(\t\x12\x10\n\x08start_ms\x18\x0e \x01(\x04\x12\x12\n\nlocal_rank\x18\x0c \x01(\x05\x12\x13\n\x0bglobal_rank\x18\x0f \x01(\x05\x12\x10\n\x08\x63pu_name\x18\x10 \x01(\t\x12\x19\n\x11\x63pu_usage_percent\x18\x01 \x01(\x01\x12\x0f\n\x07max_rss\x18\x02 \x01(\x04\x12\x13\n\x0b\x63urrent_rss\x18\x03 \x01(\x04\x12\x0f\n\x07vm_size\x18\x04 \x01(\x04\x12;\n\x07runtime\x18\x06 \x01(\x0e\x32*.graphsignal.profiles.ProcessUsage.Runtime\x12\x35\n\x0fruntime_version\x18\x07 \x01(\x0b\x32\x1c.graphsignal.profiles.SemVer\x12\x14\n\x0cruntime_impl\x18\x08 \x01(\t\",\n\x07Runtime\x12\x15\n\x11RUNTIME_UNDEFINED\x10\x00\x12\n\n\x06PYTHON\x10\x01\"\x95\x04\n\x0b\x44\x65viceUsage\x12\x35\n\x0b\x64\x65vice_type\x18\x0b \x01(\x0e\x32 .graphsignal.profiles.DeviceType\x12\x11\n\tdevice_id\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65vice_name\x18\x02 \x01(\t\x12\x14\n\x0c\x61rchitecture\x18\x11 \x01(\t\x12\x38\n\x12\x63ompute_capability\x18\x0f \x01(\x0b\x32\x1c.graphsignal.profiles.SemVer\x12\x11\n\tmem_total\x18\x03 \x01(\x04\x12\x10\n\x08mem_used\x18\x04 \x01(\x04\x12\x10\n\x08mem_free\x18\x05 \x01(\x04\x12\x1f\n\x17gpu_utilization_percent\x18\x06 \x01(\x01\x12\x1a\n\x12mem_access_percent\x18\x10 \x01(\x01\x12\x1a\n\x12pcie_throughput_tx\x18\r \x01(\x01\x12\x1a\n\x12pcie_throughput_rx\x18\x0e \x01(\x01\x12!\n\x19nvlink_throughput_tx_kibs\x18\x12 \x01(\x01\x12!\n\x19nvlink_throughput_rx_kibs\x18\x13 \x01(\x01\x12\x12\n\ngpu_temp_c\x18\x08 \x01(\x01\x12\x15\n\rpower_usage_w\x18\t \x01(\x01\x12\x19\n\x11\x66\x61n_speed_percent\x18\n \x01(\x01\x12\x1f\n\x17mxu_utilization_percent\x18\x0c \x01(\x01\"\xea\x03\n\x07OpStats\x12\x35\n\x0b\x64\x65vice_type\x18\x01 \x01(\x0e\x32 .graphsignal.profiles.DeviceType\x12\x11\n\tdevice_id\x18\x02 \x01(\t\x12\x0f\n\x07op_type\x18\x03 \x01(\t\x12\x0f\n\x07op_name\x18\x04 \x01(\t\x12\r\n\x05\x63ount\x18\x05 \x01(\x04\x12\x1a\n\x12total_host_time_us\x18\x06 \x01(\x04\x12\x1c\n\x14total_device_time_us\x18\x07 \x01(\x04\x12\x19\n\x11self_host_time_us\x18\x08 \x01(\x04\x12\x1b\n\x13self_device_time_us\x18\t \x01(\x04\x12\x19\n\x11total_host_memory\x18\n \x01(\x04\x12\x1b\n\x13total_device_memory\x18\x0b \x01(\x04\x12\x18\n\x10self_host_memory\x18\x0c \x01(\x04\x12\x1a\n\x12self_device_memory\x18\r \x01(\x04\x12\x1d\n\x15self_host_memory_rate\x18\x0e \x01(\x04\x12\x1f\n\x17self_device_memory_rate\x18\x0f \x01(\x04\x12\r\n\x05\x66lops\x18\x10 \x01(\x04\x12\x15\n\rflops_per_sec\x18\x12 \x01(\x01\x12\x1e\n\x16tensorcore_utilization\x18\x11 \x01(\x01\"\xbe\x01\n\x0bKernelStats\x12\x35\n\x0b\x64\x65vice_type\x18\x01 \x01(\x0e\x32 .graphsignal.profiles.DeviceType\x12\x11\n\tdevice_id\x18\x02 \x01(\t\x12\x0f\n\x07op_name\x18\x03 \x01(\t\x12\x13\n\x0bkernel_name\x18\x04 \x01(\t\x12\r\n\x05\x63ount\x18\x05 \x01(\x04\x12\x13\n\x0b\x64uration_ns\x18\x06 \x01(\x04\x12\x1b\n\x13is_using_tensorcore\x18\x07 \x01(\x08\"\xa8\x03\n\x0cProfilerInfo\x12P\n\x17operation_profiler_type\x18\x01 \x01(\x0e\x32/.graphsignal.profiles.ProfilerInfo.ProfilerType\x12P\n\x17\x66ramework_profiler_type\x18\x02 \x01(\x0e\x32/.graphsignal.profiles.ProfilerInfo.ProfilerType\x12-\n\x07version\x18\x03 \x01(\x0b\x32\x1c.graphsignal.profiles.SemVer\"\xc4\x01\n\x0cProfilerType\x12\x16\n\x12PROFILER_UNDEFINED\x10\x00\x12\x14\n\x10GENERIC_PROFILER\x10\x01\x12\x17\n\x13TENSORFLOW_PROFILER\x10\x02\x12\x14\n\x10PYTORCH_PROFILER\x10\x03\x12\x12\n\x0eKERAS_PROFILER\x10\x04\x12\x1e\n\x1aPYTORCH_LIGHTNING_PROFILER\x10\x06\x12\x10\n\x0cJAX_PROFILER\x10\x08\x12\x11\n\rONNX_PROFILER\x10\n\"5\n\rProfilerError\x12\x0f\n\x07message\x18\x01 \x01(\t\x12\x13\n\x0bstack_trace\x18\x02 \x01(\t*B\n\nDeviceType\x12\x19\n\x15\x44\x45VICE_TYPE_UNDEFINED\x10\x00\x12\x07\n\x03\x43PU\x10\x01\x12\x07\n\x03GPU\x10\x02\x12\x07\n\x03TPU\x10\x03\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0eprofiles.proto\x12\x14graphsignal.profiles\"X\n\rUploadRequest\x12\x34\n\x0bml_profiles\x18\x01 \x03(\x0b\x32\x1f.graphsignal.profiles.MLProfile\x12\x11\n\tupload_ms\x18\x02 \x01(\x04\"\x10\n\x0eUploadResponse\"\xb0\x01\n\rProfileRecord\x12\x0f\n\x07\x64\x61ta_id\x18\x01 \x01(\t\x12\x13\n\x0bworkload_id\x18\x02 \x01(\t\x12\x12\n\nprofile_id\x18\x03 \x01(\t\x12\x33\n\nml_profile\x18\x04 \x01(\x0b\x32\x1f.graphsignal.profiles.MLProfile\x12\x1a\n\x12\x64\x61ta_retention_sec\x18\x05 \x01(\x04\x12\x14\n\x0ctime_skew_ms\x18\x06 \x01(\x12\"\xde\x07\n\tMLProfile\x12\x15\n\rworkload_name\x18\x01 \x01(\t\x12\x11\n\tworker_id\x18\x1c \x01(\t\x12\x0e\n\x06run_id\x18\x02 \x01(\t\x12\x14\n\x0crun_start_ms\x18\' \x01(\x04\x12\x10\n\x08start_us\x18\x05 \x01(\x04\x12\x0e\n\x06\x65nd_us\x18\x06 \x01(\x04\x12\'\n\x04tags\x18  \x03(\x0b\x32\x19.graphsignal.profiles.Tag\x12\x37\n\nframeworks\x18$ \x03(\x0b\x32#.graphsignal.profiles.FrameworkInfo\x12+\n\x06params\x18\x16 \x03(\x0b\x32\x1b.graphsignal.profiles.Param\x12-\n\x07metrics\x18\x1e \x03(\x0b\x32\x1c.graphsignal.profiles.Metric\x12=\n\x0finference_stats\x18% \x01(\x0b\x32$.graphsignal.profiles.InferenceStats\x12\x33\n\nmodel_info\x18& \x01(\x0b\x32\x1f.graphsignal.profiles.ModelInfo\x12<\n\ncomm_usage\x18\x1b \x01(\x0b\x32(.graphsignal.profiles.CommunicationUsage\x12\x33\n\nnode_usage\x18\x19 \x01(\x0b\x32\x1f.graphsignal.profiles.NodeUsage\x12\x39\n\rprocess_usage\x18\x1a \x01(\x0b\x32\".graphsignal.profiles.ProcessUsage\x12\x37\n\x0c\x64\x65vice_usage\x18\x12 \x03(\x0b\x32!.graphsignal.profiles.DeviceUsage\x12/\n\x08op_stats\x18\x0b \x03(\x0b\x32\x1d.graphsignal.profiles.OpStats\x12\x37\n\x0ckernel_stats\x18\x0c \x03(\x0b\x32!.graphsignal.profiles.KernelStats\x12\x12\n\ntrace_data\x18! \x01(\x0c\x12\x1a\n\x12is_trace_available\x18\" \x01(\x08\x12\x33\n\nexceptions\x18( \x03(\x0b\x32\x1f.graphsignal.profiles.Exception\x12\x39\n\rprofiler_info\x18# \x01(\x0b\x32\".graphsignal.profiles.ProfilerInfo\x12<\n\x0fprofiler_errors\x18\x07 \x03(\x0b\x32#.graphsignal.profiles.ProfilerError\"5\n\x06SemVer\x12\r\n\x05major\x18\x01 \x01(\x05\x12\r\n\x05minor\x18\x02 \x01(\x05\x12\r\n\x05patch\x18\x03 \x01(\x05\"\xb8\x02\n\rFrameworkInfo\x12?\n\x04type\x18\x01 \x01(\x0e\x32\x31.graphsignal.profiles.FrameworkInfo.FrameworkType\x12-\n\x07version\x18\x02 \x01(\x0b\x32\x1c.graphsignal.profiles.SemVer\"\xb6\x01\n\rFrameworkType\x12\x17\n\x13\x46RAMEWORK_UNDEFINED\x10\x00\x12\x18\n\x14TENSORFLOW_FRAMEWORK\x10\x01\x12\x15\n\x11PYTORCH_FRAMEWORK\x10\x02\x12\x13\n\x0fKERAS_FRAMEWORK\x10\x03\x12\x1f\n\x1bPYTORCH_LIGHTNING_FRAMEWORK\x10\x04\x12\x11\n\rJAX_FRAMEWORK\x10\x07\x12\x12\n\x0eONNX_FRAMEWORK\x10\t\"\x14\n\x03Tag\x12\r\n\x05value\x18\x01 \x01(\t\"$\n\x05Param\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"%\n\x06Metric\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x01\"\xbc\x01\n\x0eInferenceStats\x12\x17\n\x0finference_count\x18\t \x01(\x04\x12\x1d\n\x15inference_time_p95_us\x18\n \x01(\x01\x12\x1d\n\x15inference_time_avg_us\x18\x0b \x01(\x01\x12\x16\n\x0einference_rate\x18\x0c \x01(\x01\x12\x13\n\x0bsample_rate\x18\r \x01(\x01\x12\x12\n\nbatch_size\x18\x04 \x01(\x05\x12\x12\n\nworld_size\x18\x06 \x01(\x05\"\xb2\x01\n\tModelInfo\x12\x41\n\x0cmodel_format\x18\x01 \x01(\x0e\x32+.graphsignal.profiles.ModelInfo.ModelFormat\x12\x18\n\x10model_size_bytes\x18\x02 \x01(\x04\"H\n\x0bModelFormat\x12\x14\n\x10\x46ORMAT_UNDEFINED\x10\x00\x12\x12\n\x0ePYTORCH_FORMAT\x10\x01\x12\x0f\n\x0bONNX_FORMAT\x10\x02\"\xd5\x01\n\x12\x43ommunicationUsage\x12W\n\x0c\x62\x61\x63kend_type\x18\x01 \x01(\x0e\x32\x41.graphsignal.profiles.CommunicationUsage.CommunicationBackendType\"f\n\x18\x43ommunicationBackendType\x12#\n\x1f\x43OMMUNICATION_BACKEND_UNDEFINED\x10\x00\x12\x08\n\x04NCCL\x10\x01\x12\x08\n\x04GLOO\x10\x02\x12\x07\n\x03MPI\x10\x03\x12\x08\n\x04RING\x10\x04\"\xc6\x01\n\tNodeUsage\x12\x10\n\x08hostname\x18\x01 \x01(\t\x12\x12\n\nip_address\x18\x07 \x01(\t\x12\x11\n\tnode_rank\x18\x08 \x01(\x05\x12\x10\n\x08mem_used\x18\t \x01(\x04\x12\x11\n\tmem_total\x18\n \x01(\x04\x12\x10\n\x08platform\x18\x02 \x01(\t\x12\x0f\n\x07machine\x18\x03 \x01(\t\x12\x0f\n\x07os_name\x18\x04 \x01(\t\x12\x12\n\nos_version\x18\x05 \x01(\t\x12\x13\n\x0bnum_devices\x18\x06 \x01(\x05\"\xf9\x02\n\x0cProcessUsage\x12\x12\n\nprocess_id\x18\x05 \x01(\t\x12\x10\n\x08start_ms\x18\x0e \x01(\x04\x12\x12\n\nlocal_rank\x18\x0c \x01(\x05\x12\x13\n\x0bglobal_rank\x18\x0f \x01(\x05\x12\x10\n\x08\x63pu_name\x18\x10 \x01(\t\x12\x19\n\x11\x63pu_usage_percent\x18\x01 \x01(\x01\x12\x0f\n\x07max_rss\x18\x02 \x01(\x04\x12\x13\n\x0b\x63urrent_rss\x18\x03 \x01(\x04\x12\x0f\n\x07vm_size\x18\x04 \x01(\x04\x12;\n\x07runtime\x18\x06 \x01(\x0e\x32*.graphsignal.profiles.ProcessUsage.Runtime\x12\x35\n\x0fruntime_version\x18\x07 \x01(\x0b\x32\x1c.graphsignal.profiles.SemVer\x12\x14\n\x0cruntime_impl\x18\x08 \x01(\t\",\n\x07Runtime\x12\x15\n\x11RUNTIME_UNDEFINED\x10\x00\x12\n\n\x06PYTHON\x10\x01\"\x95\x04\n\x0b\x44\x65viceUsage\x12\x35\n\x0b\x64\x65vice_type\x18\x0b \x01(\x0e\x32 .graphsignal.profiles.DeviceType\x12\x11\n\tdevice_id\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65vice_name\x18\x02 \x01(\t\x12\x14\n\x0c\x61rchitecture\x18\x11 \x01(\t\x12\x38\n\x12\x63ompute_capability\x18\x0f \x01(\x0b\x32\x1c.graphsignal.profiles.SemVer\x12\x11\n\tmem_total\x18\x03 \x01(\x04\x12\x10\n\x08mem_used\x18\x04 \x01(\x04\x12\x10\n\x08mem_free\x18\x05 \x01(\x04\x12\x1f\n\x17gpu_utilization_percent\x18\x06 \x01(\x01\x12\x1a\n\x12mem_access_percent\x18\x10 \x01(\x01\x12\x1a\n\x12pcie_throughput_tx\x18\r \x01(\x01\x12\x1a\n\x12pcie_throughput_rx\x18\x0e \x01(\x01\x12!\n\x19nvlink_throughput_tx_kibs\x18\x12 \x01(\x01\x12!\n\x19nvlink_throughput_rx_kibs\x18\x13 \x01(\x01\x12\x12\n\ngpu_temp_c\x18\x08 \x01(\x01\x12\x15\n\rpower_usage_w\x18\t \x01(\x01\x12\x19\n\x11\x66\x61n_speed_percent\x18\n \x01(\x01\x12\x1f\n\x17mxu_utilization_percent\x18\x0c \x01(\x01\"\xea\x03\n\x07OpStats\x12\x35\n\x0b\x64\x65vice_type\x18\x01 \x01(\x0e\x32 .graphsignal.profiles.DeviceType\x12\x11\n\tdevice_id\x18\x02 \x01(\t\x12\x0f\n\x07op_type\x18\x03 \x01(\t\x12\x0f\n\x07op_name\x18\x04 \x01(\t\x12\r\n\x05\x63ount\x18\x05 \x01(\x04\x12\x1a\n\x12total_host_time_us\x18\x06 \x01(\x04\x12\x1c\n\x14total_device_time_us\x18\x07 \x01(\x04\x12\x19\n\x11self_host_time_us\x18\x08 \x01(\x04\x12\x1b\n\x13self_device_time_us\x18\t \x01(\x04\x12\x19\n\x11total_host_memory\x18\n \x01(\x04\x12\x1b\n\x13total_device_memory\x18\x0b \x01(\x04\x12\x18\n\x10self_host_memory\x18\x0c \x01(\x04\x12\x1a\n\x12self_device_memory\x18\r \x01(\x04\x12\x1d\n\x15self_host_memory_rate\x18\x0e \x01(\x04\x12\x1f\n\x17self_device_memory_rate\x18\x0f \x01(\x04\x12\r\n\x05\x66lops\x18\x10 \x01(\x04\x12\x15\n\rflops_per_sec\x18\x12 \x01(\x01\x12\x1e\n\x16tensorcore_utilization\x18\x11 \x01(\x01\"\xbe\x01\n\x0bKernelStats\x12\x35\n\x0b\x64\x65vice_type\x18\x01 \x01(\x0e\x32 .graphsignal.profiles.DeviceType\x12\x11\n\tdevice_id\x18\x02 \x01(\t\x12\x0f\n\x07op_name\x18\x03 \x01(\t\x12\x13\n\x0bkernel_name\x18\x04 \x01(\t\x12\r\n\x05\x63ount\x18\x05 \x01(\x04\x12\x13\n\x0b\x64uration_ns\x18\x06 \x01(\x04\x12\x1b\n\x13is_using_tensorcore\x18\x07 \x01(\x08\"1\n\tException\x12\x0f\n\x07message\x18\x01 \x01(\t\x12\x13\n\x0bstack_trace\x18\x02 \x01(\t\"\xa8\x03\n\x0cProfilerInfo\x12P\n\x17operation_profiler_type\x18\x01 \x01(\x0e\x32/.graphsignal.profiles.ProfilerInfo.ProfilerType\x12P\n\x17\x66ramework_profiler_type\x18\x02 \x01(\x0e\x32/.graphsignal.profiles.ProfilerInfo.ProfilerType\x12-\n\x07version\x18\x03 \x01(\x0b\x32\x1c.graphsignal.profiles.SemVer\"\xc4\x01\n\x0cProfilerType\x12\x16\n\x12PROFILER_UNDEFINED\x10\x00\x12\x14\n\x10GENERIC_PROFILER\x10\x01\x12\x17\n\x13TENSORFLOW_PROFILER\x10\x02\x12\x14\n\x10PYTORCH_PROFILER\x10\x03\x12\x12\n\x0eKERAS_PROFILER\x10\x04\x12\x1e\n\x1aPYTORCH_LIGHTNING_PROFILER\x10\x06\x12\x10\n\x0cJAX_PROFILER\x10\x08\x12\x11\n\rONNX_PROFILER\x10\n\"5\n\rProfilerError\x12\x0f\n\x07message\x18\x01 \x01(\t\x12\x13\n\x0bstack_trace\x18\x02 \x01(\t*B\n\nDeviceType\x12\x19\n\x15\x44\x45VICE_TYPE_UNDEFINED\x10\x00\x12\x07\n\x03\x43PU\x10\x01\x12\x07\n\x03GPU\x10\x02\x12\x07\n\x03TPU\x10\x03\x62\x06proto3')
 
 _DEVICETYPE = DESCRIPTOR.enum_types_by_name['DeviceType']
 DeviceType = enum_type_wrapper.EnumTypeWrapper(_DEVICETYPE)
 DEVICE_TYPE_UNDEFINED = 0
 CPU = 1
 GPU = 2
 TPU = 3
@@ -38,14 +38,15 @@
 _MODELINFO = DESCRIPTOR.message_types_by_name['ModelInfo']
 _COMMUNICATIONUSAGE = DESCRIPTOR.message_types_by_name['CommunicationUsage']
 _NODEUSAGE = DESCRIPTOR.message_types_by_name['NodeUsage']
 _PROCESSUSAGE = DESCRIPTOR.message_types_by_name['ProcessUsage']
 _DEVICEUSAGE = DESCRIPTOR.message_types_by_name['DeviceUsage']
 _OPSTATS = DESCRIPTOR.message_types_by_name['OpStats']
 _KERNELSTATS = DESCRIPTOR.message_types_by_name['KernelStats']
+_EXCEPTION = DESCRIPTOR.message_types_by_name['Exception']
 _PROFILERINFO = DESCRIPTOR.message_types_by_name['ProfilerInfo']
 _PROFILERERROR = DESCRIPTOR.message_types_by_name['ProfilerError']
 _FRAMEWORKINFO_FRAMEWORKTYPE = _FRAMEWORKINFO.enum_types_by_name['FrameworkType']
 _MODELINFO_MODELFORMAT = _MODELINFO.enum_types_by_name['ModelFormat']
 _COMMUNICATIONUSAGE_COMMUNICATIONBACKENDTYPE = _COMMUNICATIONUSAGE.enum_types_by_name['CommunicationBackendType']
 _PROCESSUSAGE_RUNTIME = _PROCESSUSAGE.enum_types_by_name['Runtime']
 _PROFILERINFO_PROFILERTYPE = _PROFILERINFO.enum_types_by_name['ProfilerType']
@@ -164,14 +165,21 @@
 KernelStats = _reflection.GeneratedProtocolMessageType('KernelStats', (_message.Message,), {
   'DESCRIPTOR' : _KERNELSTATS,
   '__module__' : 'profiles_pb2'
   # @@protoc_insertion_point(class_scope:graphsignal.profiles.KernelStats)
   })
 _sym_db.RegisterMessage(KernelStats)
 
+Exception = _reflection.GeneratedProtocolMessageType('Exception', (_message.Message,), {
+  'DESCRIPTOR' : _EXCEPTION,
+  '__module__' : 'profiles_pb2'
+  # @@protoc_insertion_point(class_scope:graphsignal.profiles.Exception)
+  })
+_sym_db.RegisterMessage(Exception)
+
 ProfilerInfo = _reflection.GeneratedProtocolMessageType('ProfilerInfo', (_message.Message,), {
   'DESCRIPTOR' : _PROFILERINFO,
   '__module__' : 'profiles_pb2'
   # @@protoc_insertion_point(class_scope:graphsignal.profiles.ProfilerInfo)
   })
 _sym_db.RegisterMessage(ProfilerInfo)
 
@@ -181,58 +189,60 @@
   # @@protoc_insertion_point(class_scope:graphsignal.profiles.ProfilerError)
   })
 _sym_db.RegisterMessage(ProfilerError)
 
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  _DEVICETYPE._serialized_start=4609
-  _DEVICETYPE._serialized_end=4675
+  _DEVICETYPE._serialized_start=4713
+  _DEVICETYPE._serialized_end=4779
   _UPLOADREQUEST._serialized_start=40
   _UPLOADREQUEST._serialized_end=128
   _UPLOADRESPONSE._serialized_start=130
   _UPLOADRESPONSE._serialized_end=146
   _PROFILERECORD._serialized_start=149
   _PROFILERECORD._serialized_end=325
   _MLPROFILE._serialized_start=328
-  _MLPROFILE._serialized_end=1265
-  _SEMVER._serialized_start=1267
-  _SEMVER._serialized_end=1320
-  _FRAMEWORKINFO._serialized_start=1323
-  _FRAMEWORKINFO._serialized_end=1635
-  _FRAMEWORKINFO_FRAMEWORKTYPE._serialized_start=1453
-  _FRAMEWORKINFO_FRAMEWORKTYPE._serialized_end=1635
-  _TAG._serialized_start=1637
-  _TAG._serialized_end=1657
-  _PARAM._serialized_start=1659
-  _PARAM._serialized_end=1695
-  _METRIC._serialized_start=1697
-  _METRIC._serialized_end=1734
-  _INFERENCESTATS._serialized_start=1737
-  _INFERENCESTATS._serialized_end=1925
-  _MODELINFO._serialized_start=1928
-  _MODELINFO._serialized_end=2106
-  _MODELINFO_MODELFORMAT._serialized_start=2034
-  _MODELINFO_MODELFORMAT._serialized_end=2106
-  _COMMUNICATIONUSAGE._serialized_start=2109
-  _COMMUNICATIONUSAGE._serialized_end=2322
-  _COMMUNICATIONUSAGE_COMMUNICATIONBACKENDTYPE._serialized_start=2220
-  _COMMUNICATIONUSAGE_COMMUNICATIONBACKENDTYPE._serialized_end=2322
-  _NODEUSAGE._serialized_start=2325
-  _NODEUSAGE._serialized_end=2523
-  _PROCESSUSAGE._serialized_start=2526
-  _PROCESSUSAGE._serialized_end=2903
-  _PROCESSUSAGE_RUNTIME._serialized_start=2859
-  _PROCESSUSAGE_RUNTIME._serialized_end=2903
-  _DEVICEUSAGE._serialized_start=2906
-  _DEVICEUSAGE._serialized_end=3439
-  _OPSTATS._serialized_start=3442
-  _OPSTATS._serialized_end=3932
-  _KERNELSTATS._serialized_start=3935
-  _KERNELSTATS._serialized_end=4125
-  _PROFILERINFO._serialized_start=4128
-  _PROFILERINFO._serialized_end=4552
-  _PROFILERINFO_PROFILERTYPE._serialized_start=4356
-  _PROFILERINFO_PROFILERTYPE._serialized_end=4552
-  _PROFILERERROR._serialized_start=4554
-  _PROFILERERROR._serialized_end=4607
+  _MLPROFILE._serialized_end=1318
+  _SEMVER._serialized_start=1320
+  _SEMVER._serialized_end=1373
+  _FRAMEWORKINFO._serialized_start=1376
+  _FRAMEWORKINFO._serialized_end=1688
+  _FRAMEWORKINFO_FRAMEWORKTYPE._serialized_start=1506
+  _FRAMEWORKINFO_FRAMEWORKTYPE._serialized_end=1688
+  _TAG._serialized_start=1690
+  _TAG._serialized_end=1710
+  _PARAM._serialized_start=1712
+  _PARAM._serialized_end=1748
+  _METRIC._serialized_start=1750
+  _METRIC._serialized_end=1787
+  _INFERENCESTATS._serialized_start=1790
+  _INFERENCESTATS._serialized_end=1978
+  _MODELINFO._serialized_start=1981
+  _MODELINFO._serialized_end=2159
+  _MODELINFO_MODELFORMAT._serialized_start=2087
+  _MODELINFO_MODELFORMAT._serialized_end=2159
+  _COMMUNICATIONUSAGE._serialized_start=2162
+  _COMMUNICATIONUSAGE._serialized_end=2375
+  _COMMUNICATIONUSAGE_COMMUNICATIONBACKENDTYPE._serialized_start=2273
+  _COMMUNICATIONUSAGE_COMMUNICATIONBACKENDTYPE._serialized_end=2375
+  _NODEUSAGE._serialized_start=2378
+  _NODEUSAGE._serialized_end=2576
+  _PROCESSUSAGE._serialized_start=2579
+  _PROCESSUSAGE._serialized_end=2956
+  _PROCESSUSAGE_RUNTIME._serialized_start=2912
+  _PROCESSUSAGE_RUNTIME._serialized_end=2956
+  _DEVICEUSAGE._serialized_start=2959
+  _DEVICEUSAGE._serialized_end=3492
+  _OPSTATS._serialized_start=3495
+  _OPSTATS._serialized_end=3985
+  _KERNELSTATS._serialized_start=3988
+  _KERNELSTATS._serialized_end=4178
+  _EXCEPTION._serialized_start=4180
+  _EXCEPTION._serialized_end=4229
+  _PROFILERINFO._serialized_start=4232
+  _PROFILERINFO._serialized_end=4656
+  _PROFILERINFO_PROFILERTYPE._serialized_start=4460
+  _PROFILERINFO_PROFILERTYPE._serialized_end=4656
+  _PROFILERERROR._serialized_start=4658
+  _PROFILERERROR._serialized_end=4711
 # @@protoc_insertion_point(module_scope)
```

### Comparing `graphsignal-0.9.4/graphsignal/proto_utils.py` & `graphsignal-0.9.5/graphsignal/proto_utils.py`

 * *Files identical despite different names*

### Comparing `graphsignal-0.9.4/graphsignal/proto_utils_test.py` & `graphsignal-0.9.5/graphsignal/proto_utils_test.py`

 * *Files identical despite different names*

### Comparing `graphsignal-0.9.4/graphsignal/uploader.py` & `graphsignal-0.9.5/graphsignal/uploader.py`

 * *Files identical despite different names*

### Comparing `graphsignal-0.9.4/graphsignal/uploader_test.py` & `graphsignal-0.9.5/graphsignal/uploader_test.py`

 * *Files identical despite different names*

### Comparing `graphsignal-0.9.4/graphsignal/usage/nvml_reader.py` & `graphsignal-0.9.5/graphsignal/usage/nvml_reader.py`

 * *Files identical despite different names*

### Comparing `graphsignal-0.9.4/graphsignal/usage/nvml_reader_test.py` & `graphsignal-0.9.5/graphsignal/usage/nvml_reader_test.py`

 * *Files identical despite different names*

### Comparing `graphsignal-0.9.4/graphsignal/usage/process_reader.py` & `graphsignal-0.9.5/graphsignal/usage/process_reader.py`

 * *Files identical despite different names*

### Comparing `graphsignal-0.9.4/graphsignal/usage/process_reader_test.py` & `graphsignal-0.9.5/graphsignal/usage/process_reader_test.py`

 * *Files identical despite different names*

### Comparing `graphsignal-0.9.4/graphsignal/usage/pynvml.py` & `graphsignal-0.9.5/graphsignal/usage/pynvml.py`

 * *Files identical despite different names*

### Comparing `graphsignal-0.9.4/graphsignal/workload_run.py` & `graphsignal-0.9.5/graphsignal/workload_run.py`

 * *Files identical despite different names*

### Comparing `graphsignal-0.9.4/graphsignal/workload_run_test.py` & `graphsignal-0.9.5/graphsignal/workload_run_test.py`

 * *Files identical despite different names*

### Comparing `graphsignal-0.9.4/graphsignal.egg-info/PKG-INFO` & `graphsignal-0.9.5/graphsignal.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphsignal
-Version: 0.9.4
+Version: 0.9.5
 Summary: Graphsignal Profiler
 Home-page: https://graphsignal.com
 Author: Graphsignal, Inc.
 Author-email: devops@graphsignal.com
 License: Apache-2.0
 Keywords: machine learning,deep learning,data science,machine learning profiler,deep learning profiler,tensorflow profiler,keras profiler,pytorch profiler,inference profiling
 Platform: UNKNOWN
@@ -131,18 +131,18 @@
 #### [Hugging Face](https://graphsignal.com/docs/integrations/hugging-face/)
 
 ```python
 from transformers import pipeline
 from graphsignal.profilers.pytorch import profile_inference
 # or from graphsignal.profilers.tensorflow import profile_inference
 
-generator = pipeline(task="text-generation")
+pipe = pipeline(task="text-generation")
 
 with profile_inference():
-    output = generator('some text')
+    output = pipe('some text')
 ```
 
 #### [JAX](https://graphsignal.com/docs/integrations/jax/)
 
 ```python
 from graphsignal.profilers.jax import profile_inference
```

### Comparing `graphsignal-0.9.4/graphsignal.egg-info/SOURCES.txt` & `graphsignal-0.9.5/graphsignal.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 graphsignal.egg-info/SOURCES.txt
 graphsignal.egg-info/dependency_links.txt
 graphsignal.egg-info/requires.txt
 graphsignal.egg-info/top_level.txt
 graphsignal/profilers/__init__.py
 graphsignal/profilers/generic.py
 graphsignal/profilers/generic_test.py
-graphsignal/profilers/huggingface_generator_test.py
+graphsignal/profilers/huggingface_pipeline_test.py
 graphsignal/profilers/huggingface_subclass_test.py
 graphsignal/profilers/jax.py
 graphsignal/profilers/jax_test.py
 graphsignal/profilers/keras.py
 graphsignal/profilers/keras_test.py
 graphsignal/profilers/onnxruntime.py
 graphsignal/profilers/onnxruntime_test.py
```

### Comparing `graphsignal-0.9.4/setup.py` & `graphsignal-0.9.5/setup.py`

 * *Files identical despite different names*

