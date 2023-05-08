# Comparing `tmp/orbax-checkpoint-0.2.1.tar.gz` & `tmp/orbax-checkpoint-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orbax-checkpoint-0.2.1.tar", last modified: Fri Apr 14 17:20:24 2023, max compression
+gzip compressed data, was "orbax-checkpoint-0.2.2.tar", last modified: Mon May  8 17:57:15 2023, max compression
```

## Comparing `orbax-checkpoint-0.2.1.tar` & `orbax-checkpoint-0.2.2.tar`

### file list

```diff
@@ -1,29 +1,30 @@
--rw-r--r--   0        0        0    11357 2023-04-14 17:19:51.230321 orbax-checkpoint-0.2.1/LICENSE
--rw-r--r--   0        0        0      696 2023-04-14 17:19:51.230321 orbax-checkpoint-0.2.1/README.md
--rw-r--r--   0        0        0     2564 2023-04-14 17:19:51.230321 orbax-checkpoint-0.2.1/orbax/checkpoint/__init__.py
--rw-r--r--   0        0        0     2599 2023-04-14 17:19:51.230321 orbax-checkpoint-0.2.1/orbax/checkpoint/abstract_checkpointer.py
--rw-r--r--   0        0        0     2629 2023-04-14 17:19:51.230321 orbax-checkpoint-0.2.1/orbax/checkpoint/aggregate_handlers.py
--rw-r--r--   0        0        0     5348 2023-04-14 17:19:51.230321 orbax-checkpoint-0.2.1/orbax/checkpoint/array_checkpoint_handler.py
--rw-r--r--   0        0        0     1440 2023-04-14 17:19:51.230321 orbax-checkpoint-0.2.1/orbax/checkpoint/async_checkpoint_handler.py
--rw-r--r--   0        0        0     4742 2023-04-14 17:19:51.230321 orbax-checkpoint-0.2.1/orbax/checkpoint/async_checkpointer.py
--rw-r--r--   0        0        0     2119 2023-04-14 17:19:51.230321 orbax-checkpoint-0.2.1/orbax/checkpoint/checkpoint_handler.py
--rw-r--r--   0        0        0    33132 2023-04-14 17:19:51.230321 orbax-checkpoint-0.2.1/orbax/checkpoint/checkpoint_manager.py
--rw-r--r--   0        0        0     9920 2023-04-14 17:19:51.230321 orbax-checkpoint-0.2.1/orbax/checkpoint/checkpoint_utils.py
--rw-r--r--   0        0        0     7190 2023-04-14 17:19:51.230321 orbax-checkpoint-0.2.1/orbax/checkpoint/checkpoint_utils_test.py
--rw-r--r--   0        0        0     4022 2023-04-14 17:19:51.230321 orbax-checkpoint-0.2.1/orbax/checkpoint/checkpointer.py
--rw-r--r--   0        0        0      740 2023-04-14 17:19:51.230321 orbax-checkpoint-0.2.1/orbax/checkpoint/conftest.py
--rw-r--r--   0        0        0     1465 2023-04-14 17:19:51.230321 orbax-checkpoint-0.2.1/orbax/checkpoint/future.py
--rw-r--r--   0        0        0     2103 2023-04-14 17:19:51.230321 orbax-checkpoint-0.2.1/orbax/checkpoint/json_checkpoint_handler.py
--rw-r--r--   0        0        0     1821 2023-04-14 17:19:51.230321 orbax-checkpoint-0.2.1/orbax/checkpoint/json_checkpoint_handler_test.py
--rw-r--r--   0        0        0     2002 2023-04-14 17:19:51.230321 orbax-checkpoint-0.2.1/orbax/checkpoint/lazy_utils.py
--rw-r--r--   0        0        0     7146 2023-04-14 17:19:51.230321 orbax-checkpoint-0.2.1/orbax/checkpoint/msgpack_utils.py
--rw-r--r--   0        0        0    44930 2023-04-14 17:19:51.234321 orbax-checkpoint-0.2.1/orbax/checkpoint/orbax_checkpoint.ipynb
--rw-r--r--   0        0        0    21752 2023-04-14 17:19:51.234321 orbax-checkpoint-0.2.1/orbax/checkpoint/pytree_checkpoint_handler.py
--rw-r--r--   0        0        0     5234 2023-04-14 17:19:51.234321 orbax-checkpoint-0.2.1/orbax/checkpoint/test_utils.py
--rw-r--r--   0        0        0     9406 2023-04-14 17:19:51.234321 orbax-checkpoint-0.2.1/orbax/checkpoint/transform_utils.py
--rw-r--r--   0        0        0    13488 2023-04-14 17:19:51.234321 orbax-checkpoint-0.2.1/orbax/checkpoint/transform_utils_test.py
--rw-r--r--   0        0        0    21621 2023-04-14 17:19:51.234321 orbax-checkpoint-0.2.1/orbax/checkpoint/type_handlers.py
--rw-r--r--   0        0        0    19878 2023-04-14 17:19:51.238321 orbax-checkpoint-0.2.1/orbax/checkpoint/utils.py
--rw-r--r--   0        0        0     7444 2023-04-14 17:19:51.238321 orbax-checkpoint-0.2.1/orbax/checkpoint/utils_test.py
--rw-r--r--   0        0        0     1172 2023-04-14 17:19:51.238321 orbax-checkpoint-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1838 1970-01-01 00:00:00.000000 orbax-checkpoint-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-08 17:56:37.096296 orbax-checkpoint-0.2.2/LICENSE
+-rw-r--r--   0        0        0      699 2023-05-08 17:56:37.096296 orbax-checkpoint-0.2.2/README.md
+-rw-r--r--   0        0        0     2564 2023-05-08 17:56:37.096296 orbax-checkpoint-0.2.2/orbax/checkpoint/__init__.py
+-rw-r--r--   0        0        0     2599 2023-05-08 17:56:37.096296 orbax-checkpoint-0.2.2/orbax/checkpoint/abstract_checkpointer.py
+-rw-r--r--   0        0        0     2629 2023-05-08 17:56:37.096296 orbax-checkpoint-0.2.2/orbax/checkpoint/aggregate_handlers.py
+-rw-r--r--   0        0        0     5348 2023-05-08 17:56:37.096296 orbax-checkpoint-0.2.2/orbax/checkpoint/array_checkpoint_handler.py
+-rw-r--r--   0        0        0     1440 2023-05-08 17:56:37.096296 orbax-checkpoint-0.2.2/orbax/checkpoint/async_checkpoint_handler.py
+-rw-r--r--   0        0        0     4742 2023-05-08 17:56:37.096296 orbax-checkpoint-0.2.2/orbax/checkpoint/async_checkpointer.py
+-rw-r--r--   0        0        0     2119 2023-05-08 17:56:37.096296 orbax-checkpoint-0.2.2/orbax/checkpoint/checkpoint_handler.py
+-rw-r--r--   0        0        0    33945 2023-05-08 17:56:37.096296 orbax-checkpoint-0.2.2/orbax/checkpoint/checkpoint_manager.py
+-rw-r--r--   0        0        0     9920 2023-05-08 17:56:37.096296 orbax-checkpoint-0.2.2/orbax/checkpoint/checkpoint_utils.py
+-rw-r--r--   0        0        0     7190 2023-05-08 17:56:37.096296 orbax-checkpoint-0.2.2/orbax/checkpoint/checkpoint_utils_test.py
+-rw-r--r--   0        0        0     4022 2023-05-08 17:56:37.096296 orbax-checkpoint-0.2.2/orbax/checkpoint/checkpointer.py
+-rw-r--r--   0        0        0      740 2023-05-08 17:56:37.096296 orbax-checkpoint-0.2.2/orbax/checkpoint/conftest.py
+-rw-r--r--   0        0        0     1465 2023-05-08 17:56:37.096296 orbax-checkpoint-0.2.2/orbax/checkpoint/future.py
+-rw-r--r--   0        0        0     2103 2023-05-08 17:56:37.096296 orbax-checkpoint-0.2.2/orbax/checkpoint/json_checkpoint_handler.py
+-rw-r--r--   0        0        0     1821 2023-05-08 17:56:37.096296 orbax-checkpoint-0.2.2/orbax/checkpoint/json_checkpoint_handler_test.py
+-rw-r--r--   0        0        0     2002 2023-05-08 17:56:37.096296 orbax-checkpoint-0.2.2/orbax/checkpoint/lazy_utils.py
+-rw-r--r--   0        0        0     7672 2023-05-08 17:56:37.096296 orbax-checkpoint-0.2.2/orbax/checkpoint/msgpack_utils.py
+-rw-r--r--   0        0        0     1129 2023-05-08 17:56:37.096296 orbax-checkpoint-0.2.2/orbax/checkpoint/msgpack_utils_test.py
+-rw-r--r--   0        0        0    45137 2023-05-08 17:56:37.096296 orbax-checkpoint-0.2.2/orbax/checkpoint/orbax_checkpoint.ipynb
+-rw-r--r--   0        0        0    21766 2023-05-08 17:56:37.096296 orbax-checkpoint-0.2.2/orbax/checkpoint/pytree_checkpoint_handler.py
+-rw-r--r--   0        0        0     5234 2023-05-08 17:56:37.096296 orbax-checkpoint-0.2.2/orbax/checkpoint/test_utils.py
+-rw-r--r--   0        0        0     9406 2023-05-08 17:56:37.096296 orbax-checkpoint-0.2.2/orbax/checkpoint/transform_utils.py
+-rw-r--r--   0        0        0    13488 2023-05-08 17:56:37.100296 orbax-checkpoint-0.2.2/orbax/checkpoint/transform_utils_test.py
+-rw-r--r--   0        0        0    22579 2023-05-08 17:56:37.100296 orbax-checkpoint-0.2.2/orbax/checkpoint/type_handlers.py
+-rw-r--r--   0        0        0    20450 2023-05-08 17:56:37.100296 orbax-checkpoint-0.2.2/orbax/checkpoint/utils.py
+-rw-r--r--   0        0        0     7444 2023-05-08 17:56:37.100296 orbax-checkpoint-0.2.2/orbax/checkpoint/utils_test.py
+-rw-r--r--   0        0        0     1172 2023-05-08 17:56:37.100296 orbax-checkpoint-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     1841 1970-01-01 00:00:00.000000 orbax-checkpoint-0.2.2/PKG-INFO
```

### Comparing `orbax-checkpoint-0.2.1/LICENSE` & `orbax-checkpoint-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.2.1/README.md` & `orbax-checkpoint-0.2.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -9,7 +9,10 @@
 asynchronous checkpointing, various types, and various storage formats.
 We aim to provide a highly customizable and composable API which maximizes
 flexibility for diverse use cases.
 
 To get started, check out our [documentation](https://github.com/google/orbax/blob/main/docs/checkpoint.md).
 
 Check out our [colab](http://colab.research.google.com/github/google/orbax/blob/main/checkpoint/orbax//checkpoint/orbax_checkpoint.ipynb) for a hands-on introduction.
+
+
+
```

### Comparing `orbax-checkpoint-0.2.1/orbax/checkpoint/__init__.py` & `orbax-checkpoint-0.2.2/orbax/checkpoint/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,8 +52,8 @@
 # Convenient shorthand where instead of the following:
 #   `checkpointer = Checkpointer(PyTreeCheckpointer())`
 # we can just use:
 #   `checkpointer = PyTreeCheckpointer()`
 PyTreeCheckpointer = functools.partial(Checkpointer, PyTreeCheckpointHandler())
 
 # A new PyPI release will be pushed everytime `__version__` is increased.
-__version__ = '0.2.1'
+__version__ = '0.2.2'
```

### Comparing `orbax-checkpoint-0.2.1/orbax/checkpoint/abstract_checkpointer.py` & `orbax-checkpoint-0.2.2/orbax/checkpoint/abstract_checkpointer.py`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.2.1/orbax/checkpoint/aggregate_handlers.py` & `orbax-checkpoint-0.2.2/orbax/checkpoint/aggregate_handlers.py`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.2.1/orbax/checkpoint/array_checkpoint_handler.py` & `orbax-checkpoint-0.2.2/orbax/checkpoint/array_checkpoint_handler.py`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.2.1/orbax/checkpoint/async_checkpoint_handler.py` & `orbax-checkpoint-0.2.2/orbax/checkpoint/async_checkpoint_handler.py`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.2.1/orbax/checkpoint/async_checkpointer.py` & `orbax-checkpoint-0.2.2/orbax/checkpoint/async_checkpointer.py`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.2.1/orbax/checkpoint/checkpoint_handler.py` & `orbax-checkpoint-0.2.2/orbax/checkpoint/checkpoint_handler.py`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.2.1/orbax/checkpoint/checkpoint_manager.py` & `orbax-checkpoint-0.2.2/orbax/checkpoint/checkpoint_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 """CheckpointManager, a sync implementation of AbstractCheckpointManager."""
 
 import asyncio
 import dataclasses
 import datetime
 import threading
 from typing import Any, Callable, List, Mapping, Optional, Sequence, Tuple, Union
+import uuid
 
 from absl import logging
 from etils import epath
 import jax
 from jax.experimental import multihost_utils
 from jax.experimental.gda_serialization import serialization
 from orbax.checkpoint import utils
@@ -34,26 +35,37 @@
 
 PyTree = Any
 CheckpointDirs = Tuple[str, str]
 SaveParams = Mapping[str, Any]
 RestoreParams = SaveParams
 
 DEFAULT_ITEM_NAME = 'default'
+DESCRIPTOR_ITEM_NAME = 'descriptor'
 METRIC_ITEM_NAME = 'metrics'
 METADATA_ITEM_NAME = 'metadata'
 
+RESERVED_ITEM_NAMES = [DESCRIPTOR_ITEM_NAME, METRIC_ITEM_NAME]
+
 
 def _metrics_file_exists(metrics_item_path: epath.Path) -> bool:
   """True if item directory AND actual file both exist."""
   return (
       metrics_item_path.exists()
       and (metrics_item_path / METRIC_ITEM_NAME).exists()
   )
 
 
+def _descriptor_file_exists(descriptor_item_path: epath.Path) -> bool:
+  """True if item directory AND actual file both exist."""
+  return (
+      descriptor_item_path.exists()
+      and (descriptor_item_path / f'{DESCRIPTOR_ITEM_NAME}.pbtxt').exists()
+  )
+
+
 # TODO(b/268051457) Clean up when Pax no longer depends on separate
 # GlobalAsyncCheckpointManagerBase.
 def is_async_checkpointer(checkpointer: AbstractCheckpointer):
   return isinstance(checkpointer, AsyncCheckpointer) or isinstance(
       checkpointer,
       serialization.GlobalAsyncCheckpointManagerBase,
   )
@@ -96,25 +108,30 @@
   keep_checkpoints_without_metrics: If False, checkpoints with metrics present
     are eligible for cleanup. Otherwise, they will never be deleted.
   step_prefix: if provided, step directories will take the form
     f'{step_prefix}_<step>'. Otherwise, they will simply be an integer <step>.
   step_format_fixed_length: If set, formats step with n digits (leading zeros).
     This makes sorting steps easier. Otherwise, step has no leading zeros.
   create: if True, creates the top-level directory if it does not already exist.
+  cleanup_tmp_directories: if True, cleans up any existing temporary directories
+    on CheckpointManager creation.
+  enable_descriptor: if True, logs a Descriptor proto that contains lineage
+    information about a directory.
   """
   save_interval_steps: int = 1
   max_to_keep: Optional[int] = None
   keep_time_interval: Optional[datetime.timedelta] = None
   keep_period: Optional[int] = None
   best_fn: Optional[Callable[[PyTree], float]] = None
   best_mode: str = 'max'
   keep_checkpoints_without_metrics: bool = True
   step_prefix: Optional[str] = None
   step_format_fixed_length: Optional[int] = None
-  create: bool = False
+  create: bool = True
+  cleanup_tmp_directories: bool = False
 
   def __post_init__(self):
     if self.best_mode not in ('min', 'max'):
       msg = ("`CheckpointManagerOptions.best_mode` must be one of None, 'min' "
              "or 'max'. Got {self.dtype}.")
       raise ValueError(msg)
 
@@ -183,52 +200,54 @@
 
     Args:
       directory: the top level directory in which to save all files.
       checkpointers: a mapping of object name to Checkpointer object. For
         example, `items` provided to `save` below should have keys matching the
         keys in this argument. Alternatively, a single Checkpointer may be
         provided, in which case `save` and `restore` should always be called
-        with a single item rather than a dictionary of items.
-        See below for more details.
+        with a single item rather than a dictionary of items. See below for more
+        details.
      options: CheckpointManagerOptions. May be provided to specify additional
-       arugments. If None, uses default values of CheckpointManagerOptions.
+       arguments. If None, uses default values of CheckpointManagerOptions.
      metadata: High-level metadata that does not depend on step number, and only
        needs to be saved once.
     """
     jax.monitoring.record_event('/jax/orbax/checkpoint_manager/init')
     self._single_item = False
     if isinstance(checkpointers, AbstractCheckpointer):
       self._single_item = True
       checkpointers = {DEFAULT_ITEM_NAME: checkpointers}
     elif isinstance(checkpointers, dict):
-      if METRIC_ITEM_NAME in checkpointers:
+      for item in [k for k in checkpointers if k in RESERVED_ITEM_NAMES]:
         raise ValueError(
-            f'Found {METRIC_ITEM_NAME} in `checkpointers`; this is a reserved'
+            f'Found {item} in `checkpointers`; this is a reserved'
             ' key.'
         )
     else:
       raise ValueError(
           f'Invalid type for `checkpointers`. Found {checkpointers}.')
 
     self._checkpointers = checkpointers
     self._options = options or CheckpointManagerOptions()
     if self._options.best_mode not in ['min', 'max']:
       raise ValueError('`best_mode` must be one of: "min", "max"')
     if self._track_best:
       self._checkpointers[METRIC_ITEM_NAME] = Checkpointer(
-          JsonCheckpointHandler(filename=METRIC_ITEM_NAME))
+          JsonCheckpointHandler(filename=METRIC_ITEM_NAME)
+      )
 
     self._directory = epath.Path(directory)
     if self._options.create:
       if jax.process_index() == 0 and not self._directory.exists():
         self._directory.mkdir(parents=True)
       utils.sync_global_devices('CheckpointManager:create_directory')
 
     # Cleanup directories from previous runs that may not have been finalized.
-    self._cleanup_tmp_directories()
+    if self._options.cleanup_tmp_directories:
+      self._cleanup_tmp_directories()
     self._checkpoints = self._create_checkpoints()
     self._interval_preserved_checkpoints = (
         self._get_interval_preserved_checkpoints(self._checkpoints)
     )
     if self._checkpoints:
       self._last_checkpoint = self._checkpoints[-1]
     else:
@@ -282,28 +301,33 @@
     if not self._checkpoints:
       return None
     _, sorted_checkpoints = self._sort_checkpoints_by_metrics(self._checkpoints)
     if not sorted_checkpoints:
       return None
     return sorted_checkpoints[-1].step
 
+  def reached_preemption(self, step: int) -> bool:
+    """Returns True if a preemption sync point has been reached."""
+    return (
+        jax.config.jax_coordination_service
+        and multihost_utils.reached_preemption_sync_point(step)
+    )
+
   def should_save(self, step: int) -> bool:
     """Returns True if a checkpoint should be saved for the current step.
 
     This depends the previous step and save interval.
 
     Args:
       step: int
 
     Returns:
       True if the checkpoint should be saved.
     """
-    # Check whether to save an on-demand checkpoint due to preemption.
-    if (jax.config.jax_coordination_service and
-        multihost_utils.reached_preemption_sync_point(step)):
+    if self.reached_preemption(step):
       return True
     last_checkpoint_step = (
         self._last_checkpoint.step if self._last_checkpoint else None)
     # Ensure current step is between the last step and next step (accounting for
     # save interval). The `last_checkpoint_step` may not be initialized, in
     # which case we should save. Otherwise, step must fall on the specified
     # save interval. This condition accounts for the possibility of saving
@@ -429,15 +453,14 @@
       items = dict(items)
 
     if self._track_best:
       if metrics is None:
         logging.warning('Requested `tracked_metric`; did not provide metrics.')
       else:
         items[METRIC_ITEM_NAME] = metrics
-
     tmp_step_dir = self._create_tmp_directory(
         self._get_save_directory(step, self.directory)
     )
     for k, item in items.items():
       # Gets save dirs given top directory, step number, and a "collection". All
       # files from the same input object should be saved under this collection.
       item_dir = self._get_save_directory(
```

### Comparing `orbax-checkpoint-0.2.1/orbax/checkpoint/checkpoint_utils.py` & `orbax-checkpoint-0.2.2/orbax/checkpoint/checkpoint_utils.py`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.2.1/orbax/checkpoint/checkpoint_utils_test.py` & `orbax-checkpoint-0.2.2/orbax/checkpoint/checkpoint_utils_test.py`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.2.1/orbax/checkpoint/checkpointer.py` & `orbax-checkpoint-0.2.2/orbax/checkpoint/checkpointer.py`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.2.1/orbax/checkpoint/conftest.py` & `orbax-checkpoint-0.2.2/orbax/checkpoint/conftest.py`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.2.1/orbax/checkpoint/future.py` & `orbax-checkpoint-0.2.2/orbax/checkpoint/future.py`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.2.1/orbax/checkpoint/json_checkpoint_handler.py` & `orbax-checkpoint-0.2.2/orbax/checkpoint/json_checkpoint_handler.py`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.2.1/orbax/checkpoint/json_checkpoint_handler_test.py` & `orbax-checkpoint-0.2.2/orbax/checkpoint/json_checkpoint_handler_test.py`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.2.1/orbax/checkpoint/lazy_utils.py` & `orbax-checkpoint-0.2.2/orbax/checkpoint/lazy_utils.py`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.2.1/orbax/checkpoint/msgpack_utils.py` & `orbax-checkpoint-0.2.2/orbax/checkpoint/msgpack_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -63,14 +63,15 @@
 
 
 class _MsgpackExtType(enum.IntEnum):
   """Messagepack custom type ids."""
   NDARRAY = 1
   NATIVE_COMPLEX = 2
   NPSCALAR = 3
+  TUPLE = 4
 
 
 def _msgpack_ext_pack(x):
   """Messagepack encoders for custom types."""
   # TODO(flax-dev): Array here only work when they are fully addressable.
   # If they are not fully addressable, use the GDA path for checkpointing.
   if isinstance(x, (np.ndarray, jax.Array)):
@@ -80,27 +81,45 @@
     return msgpack.ExtType(
         _MsgpackExtType.NPSCALAR, _ndarray_to_bytes(np.asarray(x))
     )
   elif isinstance(x, complex):
     return msgpack.ExtType(
         _MsgpackExtType.NATIVE_COMPLEX, msgpack.packb((x.real, x.imag))
     )
+  elif isinstance(x, tuple):
+    return msgpack.ExtType(
+        _MsgpackExtType.TUPLE,
+        msgpack.packb(
+            list(x),
+            strict_types=True,
+            use_bin_type=True,
+            default=_msgpack_ext_pack,
+        ),
+    )
+  else:
+    raise ValueError(f'Unsupported msgpack object: {x}')
   return x
 
 
 def _msgpack_ext_unpack(code, data):
   """Messagepack decoders for custom types."""
   if code == _MsgpackExtType.NDARRAY:
     return _ndarray_from_bytes(data)
   elif code == _MsgpackExtType.NATIVE_COMPLEX:
     complex_tuple = msgpack.unpackb(data)
     return complex(complex_tuple[0], complex_tuple[1])
   elif code == _MsgpackExtType.NPSCALAR:
     ar = _ndarray_from_bytes(data)
     return ar[()]  # unpack ndarray to scalar
+  elif code == _MsgpackExtType.TUPLE:
+    return tuple(
+        msgpack.unpackb(data, raw=False, ext_hook=_msgpack_ext_unpack)
+    )
+  else:
+    raise ValueError(f'Unsupported msgpack code: {code}')
   return msgpack.ExtType(code, data)
 
 
 # Chunking array leaves
 
 # msgpack has a hard limit of 2**31 - 1 bytes per object leaf.  To circumvent
 # this limit for giant arrays (e.g. embedding tables), we traverse the tree
```

### Comparing `orbax-checkpoint-0.2.1/orbax/checkpoint/orbax_checkpoint.ipynb` & `orbax-checkpoint-0.2.2/orbax/checkpoint/orbax_checkpoint.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9959262013351842%*

 * *Differences: {"'cells'": "{6: {'source': {insert: [(1, 'if directory.exists():\\n'), (2, '  "*

 * *            "directory.rmtree()\\n'), (3, 'directory.mkdir(parents=True)')], delete: [1]}}, 9: "*

 * *            "{'source': {insert: [(1, 'if not basic_dir.exists():\\n'), (2, '  "*

 * *            "basic_dir.mkdir()')], delete: [1]}}, 22: {'source': {insert: [(1, 'if not "*

 * *            "ckpt_metrics_dir.exists():\\n'), (2, '  ckpt_metrics_dir.mkdir()')], delete: [1]}}, "*

 * *            "28: {'source': {insert: [(1, 'if not multi_dir.exist […]*

```diff
@@ -82,15 +82,17 @@
             "execution_count": null,
             "metadata": {
                 "id": "8Y1tG-q2agTf"
             },
             "outputs": [],
             "source": [
                 "directory = epath.Path('checkpoint_data')\n",
-                "directory.mkdir(parents=True, exist_ok=True)"
+                "if directory.exists():\n",
+                "  directory.rmtree()\n",
+                "directory.mkdir(parents=True)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "id": "x9J2vLLy_Kjh"
@@ -114,15 +116,16 @@
             "execution_count": null,
             "metadata": {
                 "id": "coa1aJ42-rfd"
             },
             "outputs": [],
             "source": [
                 "basic_dir = directory / 'basic'\n",
-                "basic_dir.mkdir()"
+                "if not basic_dir.exists():\n",
+                "  basic_dir.mkdir()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "id": "egh94fWsY8u3"
@@ -313,15 +316,16 @@
             "execution_count": null,
             "metadata": {
                 "id": "yxeNxKJycq9H"
             },
             "outputs": [],
             "source": [
                 "ckpt_metrics_dir = directory / 'ckpt_with_metrics'\n",
-                "ckpt_metrics_dir.mkdir()"
+                "if not ckpt_metrics_dir.exists():\n",
+                "  ckpt_metrics_dir.mkdir()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "id": "4JPDibaYc4xw"
@@ -396,15 +400,16 @@
             "execution_count": null,
             "metadata": {
                 "id": "EwHq9nmM-1PT"
             },
             "outputs": [],
             "source": [
                 "multi_dir = directory / 'multi'\n",
-                "multi_dir.mkdir()"
+                "if not multi_dir.exists():\n",
+                "  multi_dir.mkdir()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "id": "vMES1J-ni-WJ"
@@ -574,15 +579,16 @@
             "execution_count": null,
             "metadata": {
                 "id": "54lTCWujhEOl"
             },
             "outputs": [],
             "source": [
                 "async_dir = directory / 'async'\n",
-                "async_dir.mkdir()"
+                "if not async_dir.exists():\n",
+                "  async_dir.mkdir()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "id": "d5BWAer0hJk3"
@@ -1067,18 +1073,18 @@
                 "  'a1': Transform(original_key='a'),  # rename\n",
                 "  'b': {\n",
                 "    # doubled original\n",
                 "    'c': Transform(value_fn=lambda v: v * 2)\n",
                 "    # drop b/d\n",
                 "  },\n",
                 "  # one to many mapping\n",
-                "  'x': Transform(multi_value_fn=lambda kv: kv['b']['d'][0]),\n",
-                "  'y': Transform(multi_value_fn=lambda kv: kv['b']['d'][1:]),\n",
+                "  'x': Transform(multi_value_fn=lambda _, kv: kv['b']['d'][0]),\n",
+                "  'y': Transform(multi_value_fn=lambda _, kv: kv['b']['d'][1:]),\n",
                 "  # many to one mapping\n",
-                "  'z': Transform(multi_value_fn=lambda kv: kv['a'] * 2 + sum(kv['b']['d'])),\n",
+                "  'z': Transform(multi_value_fn=lambda _, kv: kv['a'] * 2 + sum(kv['b']['d'])),\n",
                 "}\n",
                 "new_tree = {  # defines the structure of the result\n",
                 "  'a1': ...,\n",
                 "  'b': {\n",
                 "    'c': ...,\n",
                 "  },\n",
                 "  'x': ...,\n",
@@ -1307,15 +1313,14 @@
             "source": [
                 "We can see in the result that layers 0 and 3 are still small, while layers 1 and 2 have large values, coming from the original checkpoint."
             ]
         }
     ],
     "metadata": {
         "colab": {
-            "collapsed_sections": [],
             "last_runtime": {
                 "build_target": "//learning/deepmind/public/tools/ml_python:ml_notebook",
                 "kind": "private"
             },
             "name": "orbax.checkpoint.ipynb",
             "private_outputs": true,
             "provenance": [
```

### Comparing `orbax-checkpoint-0.2.1/orbax/checkpoint/pytree_checkpoint_handler.py` & `orbax-checkpoint-0.2.2/orbax/checkpoint/pytree_checkpoint_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -577,13 +577,14 @@
 
     Returns:
       The structure of the checkpointed PyTree. Leaves may be of any type.
 
     Raises:
       FileNotFoundError: if the checkpoint is not found.
     """
-    if (directory / self._aggregate_filename).exists():
-      return self._aggregate_handler.deserialize(
-          directory / self._aggregate_filename
-      )
+    checkpoint_path = directory / self._aggregate_filename
+    if checkpoint_path.exists():
+      return self._aggregate_handler.deserialize(checkpoint_path)
     else:
-      raise FileNotFoundError(f'Checkpoint does not exist at {directory}.')
+      raise FileNotFoundError(
+          f'Checkpoint not found: {checkpoint_path}.'
+      )
```

### Comparing `orbax-checkpoint-0.2.1/orbax/checkpoint/test_utils.py` & `orbax-checkpoint-0.2.2/orbax/checkpoint/test_utils.py`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.2.1/orbax/checkpoint/transform_utils.py` & `orbax-checkpoint-0.2.2/orbax/checkpoint/transform_utils.py`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.2.1/orbax/checkpoint/transform_utils_test.py` & `orbax-checkpoint-0.2.2/orbax/checkpoint/transform_utils_test.py`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.2.1/orbax/checkpoint/type_handlers.py` & `orbax-checkpoint-0.2.2/orbax/checkpoint/type_handlers.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 from etils import epath
 import jax
 from jax.experimental.gda_serialization import serialization
 from jax.experimental.gda_serialization.serialization import get_tensorstore_spec
 import jax.numpy as jnp
 from jax.sharding import Mesh
 import numpy as np
+from orbax.checkpoint import utils
 from orbax.checkpoint.future import Future
 import tensorstore as ts
 
 
 Scalar = Union[int, float, np.number]
 _OCDBT_MANIFEST_FILE = 'manifest.ocdbt'
 _COORDINATOR_SETUP_TIMEOUT_SECS = 30
@@ -74,35 +75,57 @@
       jax_global_state.coordinator_address
   )
 
   coordinator_server = None
   if jax_global_state.process_id == 0:
     bind_address = f'{ocdbt_address}:0'
     logging.info('Starting DistributedCoordinatorServer at: %s', bind_address)
-    coordinator_server = ts.ocdbt.DistributedCoordinatorServer(
-        {'bind_addresses': [bind_address]}
-    )
+    coordinator_server = ts.ocdbt.DistributedCoordinatorServer({
+        'bind_addresses': [bind_address],
+    })
     jax_global_state.client.key_value_set(
         'ocdbt_coordinator', f'{ocdbt_address}:{coordinator_server.port}'
     )
 
   ocdbt_address = jax_global_state.client.blocking_key_value_get(
       'ocdbt_coordinator', _COORDINATOR_SETUP_TIMEOUT_SECS * 1000
   )
   ts_context = {
-      'ocdbt_coordinator': {'address': ocdbt_address},
+      'ocdbt_coordinator': {
+          'address': ocdbt_address,
+      },
       # Provide cache pool for B-tree nodes to avoid repeated reads.
       'cache_pool#ocdbt': {'total_bytes_limit': 100000000},
   }
   return (
       ts.Context(ts_context, parent=serialization.TS_CONTEXT),
       coordinator_server,
   )
 
 
+async def _assert_parameter_files_exist(
+    param_dir: epath.Path, metadata_key: Optional[str]
+):
+  """Checks for existence of parameter subdir and .zarray file."""
+  exists = await utils.async_exists(param_dir)
+  if not exists:
+    raise FileNotFoundError(
+        f'Individual parameter subdirectory not found at path: {param_dir}.'
+    )
+  if metadata_key is None:
+    metadata_key = '.zarray'
+  metadata_path = param_dir / metadata_key
+  exists = await utils.async_exists(metadata_path)
+  if not exists:
+    raise FileNotFoundError(
+        f'File not found: {metadata_path}. In many cases, this results from'
+        ' copying a checkpoint without using the `-a` flag.'
+    )
+
+
 @dataclasses.dataclass
 class ParamInfo:
   """Information describing a parameter in a PyTree.
 
   Note that ParamInfo is distinct from SaveArgs and RestoreArgs in that in
   represents information not provided by a user, and should be computed
   internally.
@@ -337,15 +360,16 @@
     return [write_future.commit]
 
   async def deserialize(self,
                         info: ParamInfo,
                         args: Optional[RestoreArgs] = None) -> np.ndarray:
     """Deserializes the array using Tensorstore."""
     args = args or RestoreArgs()
-
+    if not info.is_ocdbt_checkpoint:
+      await _assert_parameter_files_exist(info.path, self._metadata_key)
     # Using OCDBT, but existing checkpoint may be stored in old format.
     use_ocdbt = self._use_ocdbt and info.is_ocdbt_checkpoint
     tspec = self._get_json_tspec_read(info, use_ocdbt=use_ocdbt)
     tspec = _get_cast_tspec_deserialize(tspec, args)
     t = await ts.open(ts.Spec(tspec), open=True, context=self._ts_context)
     return await t.read()
 
@@ -493,14 +517,16 @@
           'Sharding of jax.Array cannot be None. Provide `mesh`'
           ' and `mesh_axes` OR `sharding`.'
       )
     if args.sharding is None:
       sharding = jax.sharding.NamedSharding(args.mesh, args.mesh_axes)
     else:
       sharding = args.sharding
+    if not info.is_ocdbt_checkpoint:
+      await _assert_parameter_files_exist(info.path, self._metadata_key)
     # Using OCDBT, but existing checkpoint may be stored in old format.
     use_ocdbt = self._use_ocdbt and info.is_ocdbt_checkpoint
     tspec = self._get_json_tspec_read(info, use_ocdbt=use_ocdbt)
     tspec = _get_cast_tspec_deserialize(tspec, args)
     return await serialization.async_deserialize(
         sharding,
         tspec,
```

### Comparing `orbax-checkpoint-0.2.1/orbax/checkpoint/utils.py` & `orbax-checkpoint-0.2.2/orbax/checkpoint/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,16 +48,22 @@
 _LAST_CHECKPOINT_WRITE_TIME = time.time()
 CheckpointDirs = Tuple[str, str]
 PyTree = Any
 
 
 
 
+def should_skip_device_sync() -> bool:
+  return False
+
+
 def sync_global_devices(name: str):
   """Thin wrapper to provide additional features support."""
+  if should_skip_device_sync():
+    return
   multihost_utils.sync_global_devices(name)
 
 
 def broadcast_one_to_all(pytree: PyTree) -> PyTree:
   """Thin wrapper to provide additional features support."""
   return multihost_utils.broadcast_one_to_all(pytree)
 
@@ -86,14 +92,18 @@
   return _wrap(path.mkdir)(*args, parents=parents, exist_ok=exist_ok, **kwargs)
 
 
 def async_write_bytes(path: epath.Path, data: Any):
   return _wrap(path.write_bytes)(data)
 
 
+def async_exists(path: epath.Path):
+  return _wrap(path.exists)()
+
+
 class EmptyNode:
   pass
 
 
 def is_empty_or_leaf(x: Any) -> bool:
   try:
     children, _ = jax._src.tree_util.flatten_one_level(x)  # pylint: disable=protected-access
@@ -479,15 +489,24 @@
         '/jax/checkpoint/write/duration_since_last_checkpoint_secs',
         duration_since_last_checkpoint)
   _LAST_CHECKPOINT_WRITE_TIME = checkpoint_start_time
 
 
 def on_commit_callback(temp_ckpt_dir: epath.Path, final_ckpt_dir: epath.Path,
                        checkpoint_start_time: float):
-  """Finalize atomic save and record training duration saved in a checkpoint."""
+  """A callback to run on completion of checkpoint save operation.
+
+  Args:
+    temp_ckpt_dir: A temporary checkpoint directory, where the checkpoint data
+      is currently saved.
+    final_ckpt_dir: A directory that represents the finalized name of the
+      checkpoint. Should not exist yet if atomicity is ensured via `rename`, but
+      may exist if atomicity is ensured by writing a commit success file.
+    checkpoint_start_time: The time at which checkpoint saving began.
+  """
   ensure_atomic_save(temp_ckpt_dir, final_ckpt_dir)
   record_saved_duration(checkpoint_start_time)
   logging.info('Finished saving checkpoint to `%s`.', final_ckpt_dir)
 
 
 def is_scalar(x):
   return isinstance(x, (int, float, np.number))
```

### Comparing `orbax-checkpoint-0.2.1/orbax/checkpoint/utils_test.py` & `orbax-checkpoint-0.2.2/orbax/checkpoint/utils_test.py`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.2.1/pyproject.toml` & `orbax-checkpoint-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.2.1/PKG-INFO` & `orbax-checkpoint-0.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orbax-checkpoint
-Version: 0.2.1
+Version: 0.2.2
 Summary: Orbax Checkpoint
 Keywords: JAX machine learning,checkpoint,training
 Author-email: Orbax Authors <orbax-dev@google.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -43,7 +43,10 @@
 We aim to provide a highly customizable and composable API which maximizes
 flexibility for diverse use cases.
 
 To get started, check out our [documentation](https://github.com/google/orbax/blob/main/docs/checkpoint.md).
 
 Check out our [colab](http://colab.research.google.com/github/google/orbax/blob/main/checkpoint/orbax//checkpoint/orbax_checkpoint.ipynb) for a hands-on introduction.
 
+
+
+
```

