# Comparing `tmp/scalecodec-1.2.1.tar.gz` & `tmp/scalecodec-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scalecodec-1.2.1.tar", last modified: Tue Feb 21 12:35:47 2023, max compression
+gzip compressed data, was "scalecodec-1.2.2.tar", last modified: Tue Feb 28 11:54:47 2023, max compression
```

## Comparing `scalecodec-1.2.1.tar` & `scalecodec-1.2.2.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 12:35:47.946303 scalecodec-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-02-21 12:34:40.000000 scalecodec-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    23128 2023-02-21 12:35:47.946303 scalecodec-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22308 2023-02-21 12:34:40.000000 scalecodec-1.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 12:35:47.938303 scalecodec-1.2.1/scalecodec/
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-02-21 12:34:40.000000 scalecodec-1.2.1/scalecodec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32523 2023-02-21 12:34:40.000000 scalecodec-1.2.1/scalecodec/base.py
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-02-21 12:34:40.000000 scalecodec-1.2.1/scalecodec/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-02-21 12:34:40.000000 scalecodec-1.2.1/scalecodec/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 12:35:47.946303 scalecodec-1.2.1/scalecodec/type_registry/
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-02-21 12:34:40.000000 scalecodec-1.2.1/scalecodec/type_registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-02-21 12:34:40.000000 scalecodec-1.2.1/scalecodec/type_registry/acala.json
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-02-21 12:34:40.000000 scalecodec-1.2.1/scalecodec/type_registry/canvas.json
--rw-r--r--   0 runner    (1001) docker     (123)    66503 2023-02-21 12:34:40.000000 scalecodec-1.2.1/scalecodec/type_registry/core.json
--rw-r--r--   0 runner    (1001) docker     (123)     8094 2023-02-21 12:34:40.000000 scalecodec-1.2.1/scalecodec/type_registry/crust.json
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-02-21 12:34:40.000000 scalecodec-1.2.1/scalecodec/type_registry/development.json
--rw-r--r--   0 runner    (1001) docker     (123)    16189 2023-02-21 12:34:40.000000 scalecodec-1.2.1/scalecodec/type_registry/karura.json
--rw-r--r--   0 runner    (1001) docker     (123)    11820 2023-02-21 12:34:40.000000 scalecodec-1.2.1/scalecodec/type_registry/kusama.json
--rw-r--r--   0 runner    (1001) docker     (123)   208169 2023-02-21 12:34:40.000000 scalecodec-1.2.1/scalecodec/type_registry/legacy.json
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-02-21 12:34:40.000000 scalecodec-1.2.1/scalecodec/type_registry/moonbase-alpha.json
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-02-21 12:34:40.000000 scalecodec-1.2.1/scalecodec/type_registry/moonbeam.json
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-02-21 12:34:40.000000 scalecodec-1.2.1/scalecodec/type_registry/moonriver.json
--rw-r--r--   0 runner    (1001) docker     (123)     4266 2023-02-21 12:34:40.000000 scalecodec-1.2.1/scalecodec/type_registry/polkadot.json
--rw-r--r--   0 runner    (1001) docker     (123)    47596 2023-02-21 12:34:40.000000 scalecodec-1.2.1/scalecodec/type_registry/polymesh-mainnet.json
--rw-r--r--   0 runner    (1001) docker     (123)    47596 2023-02-21 12:34:40.000000 scalecodec-1.2.1/scalecodec/type_registry/polymesh-testnet.json
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-02-21 12:34:40.000000 scalecodec-1.2.1/scalecodec/type_registry/rococo.json
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-02-21 12:34:40.000000 scalecodec-1.2.1/scalecodec/type_registry/statemine.json
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-02-21 12:34:40.000000 scalecodec-1.2.1/scalecodec/type_registry/statemint.json
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-02-21 12:34:40.000000 scalecodec-1.2.1/scalecodec/type_registry/substrate-node-template.json
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-02-21 12:34:40.000000 scalecodec-1.2.1/scalecodec/type_registry/test.json
--rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-02-21 12:34:40.000000 scalecodec-1.2.1/scalecodec/type_registry/westend.json
--rw-r--r--   0 runner    (1001) docker     (123)   100997 2023-02-21 12:34:40.000000 scalecodec-1.2.1/scalecodec/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-02-21 12:34:40.000000 scalecodec-1.2.1/scalecodec/updater.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 12:35:47.946303 scalecodec-1.2.1/scalecodec/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-02-21 12:34:40.000000 scalecodec-1.2.1/scalecodec/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-02-21 12:34:40.000000 scalecodec-1.2.1/scalecodec/utils/math.py
--rw-r--r--   0 runner    (1001) docker     (123)     7985 2023-02-21 12:34:40.000000 scalecodec-1.2.1/scalecodec/utils/ss58.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 12:35:47.938303 scalecodec-1.2.1/scalecodec.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23128 2023-02-21 12:35:47.000000 scalecodec-1.2.1/scalecodec.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-02-21 12:35:47.000000 scalecodec-1.2.1/scalecodec.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-21 12:35:47.000000 scalecodec-1.2.1/scalecodec.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-02-21 12:35:47.000000 scalecodec-1.2.1/scalecodec.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-02-21 12:35:47.000000 scalecodec-1.2.1/scalecodec.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-21 12:35:47.946303 scalecodec-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    10217 2023-02-21 12:34:40.000000 scalecodec-1.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 12:35:47.946303 scalecodec-1.2.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)    89166 2023-02-21 12:34:40.000000 scalecodec-1.2.1/test/test_extrinsic_payload.py
--rw-r--r--   0 runner    (1001) docker     (123)     7371 2023-02-21 12:34:40.000000 scalecodec-1.2.1/test/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-02-21 12:34:40.000000 scalecodec-1.2.1/test/test_runtime_call.py
--rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-02-21 12:34:40.000000 scalecodec-1.2.1/test/test_runtime_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    10405 2023-02-21 12:34:40.000000 scalecodec-1.2.1/test/test_scale_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    36470 2023-02-21 12:34:40.000000 scalecodec-1.2.1/test/test_scale_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-02-21 12:34:40.000000 scalecodec-1.2.1/test/test_scalebytes.py
--rw-r--r--   0 runner    (1001) docker     (123)     9509 2023-02-21 12:34:40.000000 scalecodec-1.2.1/test/test_ss58.py
--rw-r--r--   0 runner    (1001) docker     (123)    17395 2023-02-21 12:34:40.000000 scalecodec-1.2.1/test/test_type_encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)   179798 2023-02-21 12:34:40.000000 scalecodec-1.2.1/test/test_type_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 11:54:47.647682 scalecodec-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-02-28 11:53:32.000000 scalecodec-1.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17006 2023-02-28 11:54:47.647682 scalecodec-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16186 2023-02-28 11:53:32.000000 scalecodec-1.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 11:54:47.643682 scalecodec-1.2.2/scalecodec/
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-02-28 11:53:32.000000 scalecodec-1.2.2/scalecodec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36646 2023-02-28 11:53:32.000000 scalecodec-1.2.2/scalecodec/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-02-28 11:53:32.000000 scalecodec-1.2.2/scalecodec/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-02-28 11:53:32.000000 scalecodec-1.2.2/scalecodec/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 11:54:47.647682 scalecodec-1.2.2/scalecodec/type_registry/
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-02-28 11:53:32.000000 scalecodec-1.2.2/scalecodec/type_registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-02-28 11:53:32.000000 scalecodec-1.2.2/scalecodec/type_registry/acala.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-02-28 11:53:32.000000 scalecodec-1.2.2/scalecodec/type_registry/canvas.json
+-rw-r--r--   0 runner    (1001) docker     (123)    66503 2023-02-28 11:53:32.000000 scalecodec-1.2.2/scalecodec/type_registry/core.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8094 2023-02-28 11:53:32.000000 scalecodec-1.2.2/scalecodec/type_registry/crust.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-02-28 11:53:32.000000 scalecodec-1.2.2/scalecodec/type_registry/development.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16189 2023-02-28 11:53:32.000000 scalecodec-1.2.2/scalecodec/type_registry/karura.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11820 2023-02-28 11:53:32.000000 scalecodec-1.2.2/scalecodec/type_registry/kusama.json
+-rw-r--r--   0 runner    (1001) docker     (123)   208169 2023-02-28 11:53:32.000000 scalecodec-1.2.2/scalecodec/type_registry/legacy.json
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-02-28 11:53:32.000000 scalecodec-1.2.2/scalecodec/type_registry/moonbase-alpha.json
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-02-28 11:53:32.000000 scalecodec-1.2.2/scalecodec/type_registry/moonbeam.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-02-28 11:53:32.000000 scalecodec-1.2.2/scalecodec/type_registry/moonriver.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4266 2023-02-28 11:53:32.000000 scalecodec-1.2.2/scalecodec/type_registry/polkadot.json
+-rw-r--r--   0 runner    (1001) docker     (123)    47596 2023-02-28 11:53:32.000000 scalecodec-1.2.2/scalecodec/type_registry/polymesh-mainnet.json
+-rw-r--r--   0 runner    (1001) docker     (123)    47596 2023-02-28 11:53:32.000000 scalecodec-1.2.2/scalecodec/type_registry/polymesh-testnet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-02-28 11:53:32.000000 scalecodec-1.2.2/scalecodec/type_registry/rococo.json
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-02-28 11:53:32.000000 scalecodec-1.2.2/scalecodec/type_registry/statemine.json
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-02-28 11:53:32.000000 scalecodec-1.2.2/scalecodec/type_registry/statemint.json
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-02-28 11:53:32.000000 scalecodec-1.2.2/scalecodec/type_registry/substrate-node-template.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-02-28 11:53:32.000000 scalecodec-1.2.2/scalecodec/type_registry/test.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-02-28 11:53:32.000000 scalecodec-1.2.2/scalecodec/type_registry/westend.json
+-rw-r--r--   0 runner    (1001) docker     (123)   105662 2023-02-28 11:53:32.000000 scalecodec-1.2.2/scalecodec/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-02-28 11:53:32.000000 scalecodec-1.2.2/scalecodec/updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 11:54:47.647682 scalecodec-1.2.2/scalecodec/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-02-28 11:53:32.000000 scalecodec-1.2.2/scalecodec/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-02-28 11:53:32.000000 scalecodec-1.2.2/scalecodec/utils/math.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7999 2023-02-28 11:53:32.000000 scalecodec-1.2.2/scalecodec/utils/ss58.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 11:54:47.643682 scalecodec-1.2.2/scalecodec.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17006 2023-02-28 11:54:47.000000 scalecodec-1.2.2/scalecodec.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-02-28 11:54:47.000000 scalecodec-1.2.2/scalecodec.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-28 11:54:47.000000 scalecodec-1.2.2/scalecodec.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-02-28 11:54:47.000000 scalecodec-1.2.2/scalecodec.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-02-28 11:54:47.000000 scalecodec-1.2.2/scalecodec.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-28 11:54:47.647682 scalecodec-1.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    10217 2023-02-28 11:53:32.000000 scalecodec-1.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 11:54:47.647682 scalecodec-1.2.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    89166 2023-02-28 11:53:32.000000 scalecodec-1.2.2/test/test_extrinsic_payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7371 2023-02-28 11:53:32.000000 scalecodec-1.2.2/test/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-02-28 11:53:32.000000 scalecodec-1.2.2/test/test_runtime_call.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-02-28 11:53:32.000000 scalecodec-1.2.2/test/test_runtime_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10405 2023-02-28 11:53:32.000000 scalecodec-1.2.2/test/test_scale_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36470 2023-02-28 11:53:32.000000 scalecodec-1.2.2/test/test_scale_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-02-28 11:53:32.000000 scalecodec-1.2.2/test/test_scalebytes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9509 2023-02-28 11:53:32.000000 scalecodec-1.2.2/test/test_ss58.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17662 2023-02-28 11:53:32.000000 scalecodec-1.2.2/test/test_type_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)   179798 2023-02-28 11:53:32.000000 scalecodec-1.2.2/test/test_type_registry.py
```

### Comparing `scalecodec-1.2.1/LICENSE` & `scalecodec-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `scalecodec-1.2.1/scalecodec/__init__.py` & `scalecodec-1.2.2/scalecodec/__init__.py`

 * *Files identical despite different names*

### Comparing `scalecodec-1.2.1/scalecodec/base.py` & `scalecodec-1.2.2/scalecodec/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,14 +38,17 @@
 
         if instance_key not in cls._instances:
             cls._instances[instance_key] = super(Singleton, cls).__call__(*args, **kwargs)
         return cls._instances[instance_key]
 
 
 class RuntimeConfigurationObject:
+    """
+    Container for runtime configuration, for example type definitions and runtime upgrade information
+    """
 
     @classmethod
     def all_subclasses(cls, class_):
         return set(class_.__subclasses__()).union(
             [s for c in class_.__subclasses__() for s in cls.all_subclasses(c)])
 
     def __init__(self, config_id=None, ss58_format=None, only_primitives_on_init=False, implements_scale_info=False):
@@ -89,14 +92,25 @@
             return 'Compact<Moment>'
         if name.lower() == '<inherentofflinereport as inherentofflinereport>::inherent':
             return 'InherentOfflineReport'
 
         return name
 
     def get_decoder_class(self, type_string: Union[str, dict]):
+        """
+        Lookup and return a ScaleDecoder class for given `type_string`
+
+        Parameters
+        ----------
+        type_string
+
+        Returns
+        -------
+        ScaleDecoder
+        """
 
         if type(type_string) is dict:
             # Inner struct
             decoder_class = type('InnerStruct', (self.get_decoder_class('Struct'),), {
                 'type_mapping': tuple(type_string.items())
             })
             decoder_class.runtime_config = self
@@ -514,83 +528,132 @@
 
         scale_info_types = metadata.portable_registry.value_object['types'].value_object
 
         self.update_from_scale_info_types(scale_info_types, prefix=prefix)
 
         # Process extrinsic type in metadata to register correct Address and ExtrinsicSignature types
         try:
-            extrinsic_type_id = metadata[1][1]['extrinsic']['ty'].value
+            # Retrieve Extrinsic using common namespace
+            extrinsic_type = self.get_decoder_class("sp_runtime::generic::unchecked_extrinsic::UncheckedExtrinsic")
+
+            # Try to fall back on extrinsic type in metadata
+            if extrinsic_type is None:
+                extrinsic_type_id = metadata[1][1]['extrinsic']['ty'].value
+                extrinsic_type = self.get_decoder_class(f"{prefix}::{extrinsic_type_id}")
 
-            extrinsic_type = self.get_decoder_class(f"{prefix}::{extrinsic_type_id}")
+            if extrinsic_type is not None:
+                # Extract Address and Signature type and set in type registry
 
-            types_dict = {}
+                types_dict = {}
 
-            for param in extrinsic_type.scale_info_type.value['params']:
-                if param['name'] == 'Address':
+                for param in extrinsic_type.scale_info_type.value['params']:
+                    if param['name'] == 'Address':
 
-                    type_string = f'{prefix}::{param["type"]}'
+                        type_string = f'{prefix}::{param["type"]}'
 
-                    types_dict['Address'] = type_string
-                    types_dict['AccountId'] = type_string
-                    types_dict['LookupSource'] = type_string
+                        types_dict['Address'] = type_string
+                        types_dict['AccountId'] = type_string
+                        types_dict['LookupSource'] = type_string
 
-                    # Check if Address is MultiAddress
-                    addres_type = self.get_decoder_class(type_string)
+                        # Check if Address is MultiAddress
+                        addres_type = self.get_decoder_class(type_string)
 
-                    if addres_type is self.get_decoder_class('sp_runtime::multiaddress::MultiAddress'):
-                        for address_param in addres_type.scale_info_type.value['params']:
-                            if address_param['name'] == 'AccountId':
-                                # Set AccountId
-                                types_dict['AccountId'] = f'{prefix}::{address_param["type"]}'
+                        if addres_type is self.get_decoder_class('sp_runtime::multiaddress::MultiAddress'):
+                            for address_param in addres_type.scale_info_type.value['params']:
+                                if address_param['name'] == 'AccountId':
+                                    # Set AccountId
+                                    types_dict['AccountId'] = f'{prefix}::{address_param["type"]}'
 
-                elif param['name'] == 'Signature':
-                    types_dict['ExtrinsicSignature'] = f'{prefix}::{param["type"]}'
+                    elif param['name'] == 'Signature':
+                        types_dict['ExtrinsicSignature'] = f'{prefix}::{param["type"]}'
 
-            # Update type registry
-            self.update_type_registry_types(types_dict)
+                # Update type registry
+                self.update_type_registry_types(types_dict)
         except NotImplementedError:
             pass
 
-
     def add_contract_metadata_dict_to_type_registry(self, metadata_dict):
         # TODO
         prefix = f"ink::{metadata_dict['source']['hash']}"
         return self.update_from_scale_info_types(metadata_dict['types'], prefix=prefix)
 
 
 class ScaleBytes:
+    """
+    Representation of SCALE encoded Bytes.
+    """
 
     def __init__(self, data: Union[str, bytes, bytearray]):
+        """
+        Constructs a SCALE bytes-stream with provided `data`
+
+        Parameters
+        ----------
+        data
+        """
         self.offset = 0
 
         if type(data) is bytearray:
             self.data = data
         elif type(data) is bytes:
             self.data = bytearray(data)
         elif type(data) is str and data[0:2] == '0x':
             self.data = bytearray.fromhex(data[2:])
         else:
             raise ValueError("Provided data is not in supported format: provided '{}'".format(type(data)))
 
         self.length = len(self.data)
 
     def get_next_bytes(self, length: int) -> bytearray:
+        """
+        Retrieve `length` amount of bytes of the stream
+
+        Parameters
+        ----------
+        length: amount of requested bytes
+
+        Returns
+        -------
+        bytearray
+        """
         data = self.data[self.offset:self.offset + length]
         self.offset += length
         return data
 
     def get_remaining_bytes(self) -> bytearray:
+        """
+        Retrieves all remaining bytes from the stream
+
+        Returns
+        -------
+        bytearray
+        """
+
         data = self.data[self.offset:]
         self.offset = self.length
         return data
 
     def get_remaining_length(self) -> int:
+        """
+        Returns how many bytes are left in the stream
+
+        Returns
+        -------
+        int
+        """
         return self.length - self.offset
 
     def reset(self):
+        """
+        Resets the pointer of the stream to the beginning
+
+        Returns
+        -------
+
+        """
         self.offset = 0
 
     def __str__(self):
         return "0x{}".format(self.data.hex())
 
     def __eq__(self, other):
         if not hasattr(other, 'data'):
@@ -613,29 +676,47 @@
         elif type(data) == str and data[0:2] == '0x':
             data = bytearray.fromhex(data[2:])
 
         if type(data) == bytearray:
             return ScaleBytes(self.data + data)
 
     def to_hex(self) -> str:
+        """
+        Return a hex-string (e.g. "0x00") representation of the byte-stream
+
+        Returns
+        -------
+        str
+        """
         return f'0x{self.data.hex()}'
 
 
 class ScaleDecoder(ABC):
+    """
+    Base class for all SCALE decoding/encoding
+    """
 
     type_string = None
 
     type_mapping = None
 
     sub_type = None
 
     runtime_config = None
 
     def __init__(self, data: ScaleBytes, sub_type: str = None, runtime_config: RuntimeConfigurationObject = None):
+        """
+        Constructs an SCALE codec class capable of encoding and decoding SCALE-bytes
 
+        Parameters
+        ----------
+        data: ScaleBytes stream of SCALE data
+        sub_type
+        runtime_config
+        """
         if sub_type:
             self.sub_type = sub_type
 
         if self.type_mapping is None and self.type_string:
             self.build_type_mapping()
 
         if data:
@@ -692,38 +773,100 @@
 
             for tuple_element in tuple_contents.split(','):
                 type_mapping += (tuple_element.strip().replace('|', ','),)
 
             cls.type_mapping = type_mapping
 
     def get_next_bytes(self, length) -> bytearray:
+        """
+        Retrieve `length` amount of bytes of the SCALE-bytes stream
+
+        Parameters
+        ----------
+        length: amount of requested bytes
+
+        Returns
+        -------
+        bytearray
+        """
         data = self.data.get_next_bytes(length)
         return data
 
     def get_next_u8(self) -> int:
+        """
+        Retrieves the next byte and convert to an int
+
+        Returns
+        -------
+        int
+        """
         return int.from_bytes(self.get_next_bytes(1), byteorder='little')
 
     def get_next_bool(self) -> bool:
+        """
+        Retrieves the next byte and convert to an bool
+
+        Returns
+        -------
+        bool
+        """
         data = self.get_next_bytes(1)
         if data not in [b'\x00', b'\x01']:
             raise InvalidScaleTypeValueException('Invalid value for datatype "bool"')
         return data == b'\x01'
 
     def get_remaining_bytes(self) -> bytearray:
+        """
+        Retrieves all remaining bytes from the stream
+
+        Returns
+        -------
+        bytearray
+        """
         data = self.data.get_remaining_bytes()
         return data
 
     def get_used_bytes(self) -> bytearray:
+        """
+        Returns a bytearray of all SCALE-bytes used in the decoding process
+
+        Returns
+        -------
+        bytearray
+        """
         return self.data.data[self.data_start_offset:self.data_end_offset]
 
     @abstractmethod
     def process(self):
+        """
+        Implementation of the decoding process
+
+        Returns
+        -------
+
+        """
         raise NotImplementedError
 
     def decode(self, data: ScaleBytes = None, check_remaining=True):
+        """
+        Decodes available SCALE-bytes according to type specification of this ScaleType
+
+        If no `data` is provided, it will try to decode data specified during init
+
+        If `check_remaining` is enabled, an exception will be raised when data is remaining after decoding
+
+        Parameters
+        ----------
+        data
+        check_remaining: If enabled, an exception will be raised when data is remaining after decoding
+
+        Returns
+        -------
+
+        """
 
         if data is not None:
             self.decoded = False
             self.data = data
 
         if not self.decoded:
 
@@ -751,15 +894,26 @@
 
     def __str__(self):
         return str(self.serialize()) or ''
 
     def __repr__(self):
         return "<{}(value={})>".format(self.__class__.__name__, self.serialize())
 
-    def encode(self, value=None):
+    def encode(self, value=None) -> ScaleBytes:
+        """
+        Encodes the serialized `value` representation of current `ScaleType` to a `ScaleBytes` stream
+
+        Parameters
+        ----------
+        value
+
+        Returns
+        -------
+        ScaleBytes
+        """
 
         if value and issubclass(self.__class__, value.__class__):
             # Accept instance of current class directly
             self.data = value.data
             self.value_object = value.value_object
             self.value_serialized = value.value_serialized
             return value.data
@@ -772,19 +926,31 @@
 
         if self.value_object is None:
             self.value_object = self.value_serialized
 
         return self.data
 
     def process_encode(self, value) -> ScaleBytes:
+        """
+        Implementation of the encoding process
+
+        Parameters
+        ----------
+        value
+
+        Returns
+        -------
+        ScaleBytes
+        """
         raise NotImplementedError("Encoding not implemented for this ScaleType")
 
     @classmethod
     def get_decoder_class(cls, type_string, data=None, runtime_config=None, **kwargs):
         """
+        Retrieves the decoding class for provided `type_string`
 
         Parameters
         ----------
         type_string
         data
         runtime_config
         kwargs
@@ -810,32 +976,43 @@
     # TODO rename to decode_type (confusing when encoding is introduced)
     def process_type(self, type_string, **kwargs):
         obj = self.runtime_config.create_scale_object(type_string, self.data, **kwargs)
         obj.decode(check_remaining=False)
         return obj
 
     def serialize(self):
+        """
+        Returns a serialized representation of current ScaleType
+
+        Returns
+        -------
+
+        """
         return self.value_serialized
 
     @classmethod
     def convert_type(cls, name):
         return RuntimeConfigurationObject.convert_type_string(name)
 
 
 class RuntimeConfiguration(RuntimeConfigurationObject, metaclass=Singleton):
     pass
 
 
 class ScaleType(ScaleDecoder, ABC):
-
+    """
+    Base class for all SCALE types
+    """
     scale_info_type: 'GenericRegistryType' = None
 
     def __init__(self, data=None, sub_type=None, metadata=None, runtime_config=None):
         """
 
+        Initializes an `ScaleType`
+
         Parameters
         ----------
         data: ScaleBytes
         sub_type: str
         metadata: VersionedMetadata
         runtime_config: RuntimeConfigurationObject
         """
@@ -887,14 +1064,16 @@
 
     @classmethod
     def generate_type_decomposition(cls, _recursion_level: int = 0, max_recursion: int = TYPE_DECOMP_MAX_RECURSIVE):
         return cls.__name__
 
 
 class ScalePrimitive(ScaleType, ABC):
-
+    """
+    A SCALE representation of a RUST primitive
+    """
     @classmethod
     def generate_type_decomposition(cls, _recursion_level: int = 0, max_recursion: int = TYPE_DECOMP_MAX_RECURSIVE):
         return cls.__name__.lower()
```

### Comparing `scalecodec-1.2.1/scalecodec/exceptions.py` & `scalecodec-1.2.2/scalecodec/exceptions.py`

 * *Files identical despite different names*

### Comparing `scalecodec-1.2.1/scalecodec/type_registry/__init__.py` & `scalecodec-1.2.2/scalecodec/type_registry/__init__.py`

 * *Files identical despite different names*

### Comparing `scalecodec-1.2.1/scalecodec/type_registry/canvas.json` & `scalecodec-1.2.2/scalecodec/type_registry/canvas.json`

 * *Files identical despite different names*

### Comparing `scalecodec-1.2.1/scalecodec/type_registry/core.json` & `scalecodec-1.2.2/scalecodec/type_registry/core.json`

 * *Files identical despite different names*

### Comparing `scalecodec-1.2.1/scalecodec/type_registry/crust.json` & `scalecodec-1.2.2/scalecodec/type_registry/crust.json`

 * *Files identical despite different names*

### Comparing `scalecodec-1.2.1/scalecodec/type_registry/development.json` & `scalecodec-1.2.2/scalecodec/type_registry/development.json`

 * *Files identical despite different names*

### Comparing `scalecodec-1.2.1/scalecodec/type_registry/karura.json` & `scalecodec-1.2.2/scalecodec/type_registry/karura.json`

 * *Files identical despite different names*

### Comparing `scalecodec-1.2.1/scalecodec/type_registry/kusama.json` & `scalecodec-1.2.2/scalecodec/type_registry/kusama.json`

 * *Files identical despite different names*

### Comparing `scalecodec-1.2.1/scalecodec/type_registry/legacy.json` & `scalecodec-1.2.2/scalecodec/type_registry/legacy.json`

 * *Files identical despite different names*

### Comparing `scalecodec-1.2.1/scalecodec/type_registry/moonriver.json` & `scalecodec-1.2.2/scalecodec/type_registry/moonriver.json`

 * *Files identical despite different names*

### Comparing `scalecodec-1.2.1/scalecodec/type_registry/polkadot.json` & `scalecodec-1.2.2/scalecodec/type_registry/polkadot.json`

 * *Files identical despite different names*

### Comparing `scalecodec-1.2.1/scalecodec/type_registry/polymesh-mainnet.json` & `scalecodec-1.2.2/scalecodec/type_registry/polymesh-mainnet.json`

 * *Files identical despite different names*

### Comparing `scalecodec-1.2.1/scalecodec/type_registry/polymesh-testnet.json` & `scalecodec-1.2.2/scalecodec/type_registry/polymesh-testnet.json`

 * *Files identical despite different names*

### Comparing `scalecodec-1.2.1/scalecodec/type_registry/rococo.json` & `scalecodec-1.2.2/scalecodec/type_registry/rococo.json`

 * *Files identical despite different names*

### Comparing `scalecodec-1.2.1/scalecodec/type_registry/substrate-node-template.json` & `scalecodec-1.2.2/scalecodec/type_registry/substrate-node-template.json`

 * *Files identical despite different names*

### Comparing `scalecodec-1.2.1/scalecodec/type_registry/test.json` & `scalecodec-1.2.2/scalecodec/type_registry/test.json`

 * *Files identical despite different names*

### Comparing `scalecodec-1.2.1/scalecodec/type_registry/westend.json` & `scalecodec-1.2.2/scalecodec/type_registry/westend.json`

 * *Files identical despite different names*

### Comparing `scalecodec-1.2.1/scalecodec/types.py` & `scalecodec-1.2.2/scalecodec/types.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,14 +25,17 @@
 
 from scalecodec.base import ScaleType, ScaleBytes, ScalePrimitive
 from scalecodec.exceptions import InvalidScaleTypeValueException, MetadataCallFunctionNotFound
 from scalecodec.utils.math import trailing_zeros, next_power_of_two
 
 
 class Compact(ScaleType):
+    """
+    A space efficient type to encoding fixed-width integers
+    """
 
     def __init__(self, data=None, **kwargs):
         self.compact_length = 0
         self.compact_bytes = None
         super().__init__(data, **kwargs)
 
     def process_compact_bytes(self):
@@ -132,14 +135,19 @@
                 if 2 ** (8 * (bytes_length-1)) <= value < 2 ** (8 * bytes_length):
                     return ScaleBytes(bytearray(((bytes_length - 4) << 2 | 0b11).to_bytes(1, 'little') + value.to_bytes(bytes_length, 'little')))
             else:
                 raise ValueError('{} out of range'.format(value))
 
 
 class Option(ScaleType):
+    """
+    Option is a type that represents an optional value, which can be either Some(value) if a value is present or None
+    if it is absent, allowing for safe handling of null or missing values without causing runtime errors.
+    """
+
     def process(self):
 
         option_byte = self.get_next_bytes(1)
 
         if self.sub_type and option_byte != b'\x00':
             self.value_object = self.process_type(self.sub_type)
             return self.value_object.value
@@ -167,15 +175,17 @@
         sub_type_obj = cls.runtime_config.create_scale_object(cls.sub_type)
         return None, sub_type_obj.generate_type_decomposition(
             _recursion_level=_recursion_level + 1, max_recursion=max_recursion
         )
 
 
 class Bytes(ScaleType):
-
+    """
+    A variable collection of bytes, stored as an `Vec<u8>`
+    """
     type_string = 'Vec<u8>'
 
     def process(self):
 
         length = self.process_type('Compact<u32>').value
         value = self.get_next_bytes(length)
 
@@ -285,158 +295,186 @@
         return f'0x{self.value_object.hex()}'
 
     def process_encode(self, value):
         return ScaleBytes(bytes.fromhex(value[2:]))
 
 
 class U8(ScalePrimitive):
+    """
+    Unsigned 8-bit int type, encoded in little-endian (LE) format
+    """
 
     def process(self):
         return self.get_next_u8()
 
     def process_encode(self, value):
 
         if 0 <= int(value) <= 2**8 - 1:
             return ScaleBytes(bytearray(int(value).to_bytes(1, 'little')))
         else:
             raise ValueError('{} out of range for u8'.format(value))
 
 
 class U16(ScalePrimitive):
+    """
+    Unsigned 16-bit int type, encoded in little-endian (LE) format
+    """
 
     def process(self):
         return int.from_bytes(self.get_next_bytes(2), byteorder='little')
 
     def process_encode(self, value):
 
         if 0 <= int(value) <= 2**16 - 1:
             return ScaleBytes(bytearray(int(value).to_bytes(2, 'little')))
         else:
             raise ValueError('{} out of range for u16'.format(value))
 
 
 class U32(ScalePrimitive):
-
+    """
+    Unsigned 32-bit int type, encoded in little-endian (LE) format
+    """
     def process(self):
         return int.from_bytes(self.get_next_bytes(4), byteorder='little')
 
     def process_encode(self, value):
 
         if 0 <= int(value) <= 2**32 - 1:
             return ScaleBytes(bytearray(int(value).to_bytes(4, 'little')))
         else:
             raise ValueError('{} out of range for u32'.format(value))
 
 
 class U64(ScalePrimitive):
-
+    """
+    Unsigned 64-bit int type, encoded in little-endian (LE) format
+    """
     def process(self):
         return int(int.from_bytes(self.get_next_bytes(8), byteorder='little'))
 
     def process_encode(self, value):
 
         if 0 <= int(value) <= 2**64 - 1:
             return ScaleBytes(bytearray(int(value).to_bytes(8, 'little')))
         else:
             raise ValueError('{} out of range for u64'.format(value))
 
 
 class U128(ScalePrimitive):
+    """
+    Unsigned 128-bit int type, encoded in little-endian (LE) format
+    """
 
     def process(self):
         return int(int.from_bytes(self.get_next_bytes(16), byteorder='little'))
 
     def process_encode(self, value):
 
         if 0 <= int(value) <= 2**128 - 1:
             return ScaleBytes(bytearray(int(value).to_bytes(16, 'little')))
         else:
             raise ValueError('{} out of range for u128'.format(value))
 
 
 class U256(ScalePrimitive):
+    """
+    Unsigned 256-bit int type, encoded in little-endian (LE) format
+    """
 
     def process(self):
         return int(int.from_bytes(self.get_next_bytes(32), byteorder='little'))
 
     def process_encode(self, value):
 
         if 0 <= int(value) <= 2**256 - 1:
             return ScaleBytes(bytearray(int(value).to_bytes(32, 'little')))
         else:
             raise ValueError('{} out of range for u256'.format(value))
 
 
 class I8(ScalePrimitive):
-
+    """
+    Signed 8-bit int type, encoded in little-endian (LE) format
+    """
     def process(self):
         return int.from_bytes(self.get_next_bytes(1), byteorder='little', signed=True)
 
     def process_encode(self, value):
 
         if -128 <= int(value) <= 127:
             return ScaleBytes(bytearray(int(value).to_bytes(1, 'little', signed=True)))
         else:
             raise ValueError('{} out of range for i8'.format(value))
 
 
 class I16(ScalePrimitive):
-
+    """
+    Signed 16-bit int type, encoded in little-endian (LE) format
+    """
     def process(self):
         return int.from_bytes(self.get_next_bytes(2), byteorder='little', signed=True)
 
     def process_encode(self, value):
 
         if -32768 <= int(value) <= 32767:
             return ScaleBytes(bytearray(int(value).to_bytes(2, 'little', signed=True)))
         else:
             raise ValueError('{} out of range for i16'.format(value))
 
 
 class I32(ScalePrimitive):
-
+    """
+    Signed 32-bit int type, encoded in little-endian (LE) format
+    """
     def process(self):
         return int.from_bytes(self.get_next_bytes(4), byteorder='little', signed=True)
 
     def process_encode(self, value):
 
         if -2147483648 <= int(value) <= 2147483647:
             return ScaleBytes(bytearray(int(value).to_bytes(4, 'little', signed=True)))
         else:
             raise ValueError('{} out of range for i32'.format(value))
 
 
 class I64(ScalePrimitive):
-
+    """
+    Signed 64-bit int type, encoded in little-endian (LE) format
+    """
     def process(self):
         return int.from_bytes(self.get_next_bytes(8), byteorder='little', signed=True)
 
     def process_encode(self, value):
 
         if -2**64 <= int(value) <= 2**64-1:
             return ScaleBytes(bytearray(int(value).to_bytes(8, 'little', signed=True)))
         else:
             raise ValueError('{} out of range for i64'.format(value))
 
 
 class I128(ScalePrimitive):
-
+    """
+    Signed 128-bit int type, encoded in little-endian (LE) format
+    """
     def process(self):
         return int.from_bytes(self.get_next_bytes(16), byteorder='little', signed=True)
 
     def process_encode(self, value):
 
         if -2**128 <= int(value) <= 2**128-1:
             return ScaleBytes(bytearray(int(value).to_bytes(16, 'little', signed=True)))
         else:
             raise ValueError('{} out of range for i128'.format(value))
 
 
 class I256(ScalePrimitive):
-
+    """
+    Signed 256-bit int type, encoded in little-endian (LE) format
+    """
     def process(self):
         return int.from_bytes(self.get_next_bytes(32), byteorder='little', signed=True)
 
     def process_encode(self, value):
 
         if -2**256 <= int(value) <= 2**256-1:
             return ScaleBytes(bytearray(int(value).to_bytes(32, 'little', signed=True)))
@@ -465,37 +503,43 @@
         if type(value) is not float:
             raise ValueError(f'{value} is not a float')
 
         return ScaleBytes(struct.pack('d', value))
 
 
 class H160(ScalePrimitive):
-
+    """
+    Fixed-size uninterpreted hash type with 20 bytes (160 bits) size.
+    """
     def process(self):
         return '0x{}'.format(self.get_next_bytes(20).hex())
 
     def process_encode(self, value):
         if value[0:2] != '0x' or len(value) != 42:
             raise ValueError('Value should start with "0x" and should be 20 bytes long')
         return ScaleBytes(value)
 
 
 class H256(ScalePrimitive):
-
+    """
+    Fixed-size uninterpreted hash type with 32 bytes (256 bits) size.
+    """
     def process(self):
         return '0x{}'.format(self.get_next_bytes(32).hex())
 
     def process_encode(self, value):
         if value[0:2] != '0x' or len(value) != 66:
             raise ValueError('Value should start with "0x" and should be 32 bytes long')
         return ScaleBytes(value)
 
 
 class H512(ScalePrimitive):
-
+    """
+    Fixed-size uninterpreted hash type with 64 bytes (512 bits) size.
+    """
     def process(self):
         return '0x{}'.format(self.get_next_bytes(64).hex())
 
     def process_encode(self, value: Union[str, bytes]):
 
         if type(value) is bytes and len(value) != 64:
             raise ValueError('Value should be 64 bytes long')
@@ -503,15 +547,17 @@
         if type(value) is str and (value[0:2] != '0x' or len(value) != 130):
             raise ValueError('Value should start with "0x" and should be 64 bytes long')
 
         return ScaleBytes(value)
 
 
 class Struct(ScaleType):
-
+    """
+    A struct is a composite data type that groups together zero or more values with various types into a single object
+    """
     def __init__(self, data=None, type_mapping=None, **kwargs):
 
         if type_mapping:
             self.type_mapping = type_mapping
 
         super().__init__(data, **kwargs)
 
@@ -527,22 +573,29 @@
 
             self.value_object[key] = field_obj
 
             result[key] = field_obj.value
 
         return result
 
-    def process_encode(self, value: Union[dict, tuple]) -> ScaleBytes:
+    def process_encode(self, value: Union[dict, tuple, str, int, bool]) -> ScaleBytes:
         data = ScaleBytes(bytearray())
 
         self.value_object = {}
 
+        if type(value) in (str, int, bool):
+            # Convert to tuple with one element
+            value = (value,)
+
         if type(value) is tuple:
             # Convert tuple to dict
-            value = {key: value[idx] for idx, (key, _) in enumerate(self.type_mapping)}
+            try:
+                value = {key: value[idx] for idx, (key, _) in enumerate(self.type_mapping)}
+            except IndexError:
+                raise ValueError("Not enough items in tuple to match type_mapping")
 
         for key, data_type in self.type_mapping:
             if key not in value:
                 raise ValueError('Element "{}" of struct is missing in given value'.format(key))
 
             element_obj = self.runtime_config.create_scale_object(
                 type_string=data_type, metadata=self.metadata
@@ -636,14 +689,19 @@
                         return member_type
 
                 result += (member_type,)
         return result
 
 
 class Set(ScaleType):
+    """
+    The Set type in Substrate is an unordered collection that contains unique elements.
+    It is implemented using a binary search tree, allowing for efficient insertion, removal, and lookup operations.
+    """
+
     value_list = []
     value_type = 'u64'
 
     def __init__(self, data, value_list=None, **kwargs):
         self.set_value = None
 
         if value_list:
@@ -779,15 +837,17 @@
 
     @classmethod
     def process_scale_info_definition(cls, scale_info_definition: 'GenericRegistryType', prefix: str):
         return
 
 
 class Bool(ScalePrimitive):
-
+    """
+    Boolean type
+    """
     def process(self):
         return self.get_next_bool()
 
     def process_encode(self, value):
         if value is True:
             return ScaleBytes('0x01')
         elif value is False:
@@ -824,14 +884,17 @@
             'Proposal', data=ScaleBytes(result['proposal']), metadata=self.metadata
         ).decode()
 
         return result
 
 
 class GenericAccountId(H256):
+    """
+    An SS58 formatted representation of an account
+    """
 
     def __init__(self, data=None, **kwargs):
         self.ss58_address = None
         self.public_key = None
         super().__init__(data, **kwargs)
 
     def process_encode(self, value):
@@ -861,26 +924,35 @@
 
     @classmethod
     def generate_type_decomposition(cls, _recursion_level: int = 0, max_recursion: int = TYPE_DECOMP_MAX_RECURSIVE):
         return 'AccountId'
 
 
 class GenericEthereumAccountId(H160):
-
+    """
+    Representation of an Ethereum address, internally a `H160`
+    """
     @classmethod
     def process_scale_info_definition(cls, scale_info_definition: 'GenericRegistryType', prefix: str):
         return
 
 
 class GenericAccountIndex(U32):
+    """
+    The AccountIndex type Substrate represents an account index, which is a unique identifier assigned
+    to an account in the Substrate runtime.
+    """
     pass
 
 
 class Vec(ScaleType):
-
+    """
+    A Vec in RUST is a dynamically resizable array that can hold a sequence of elements of the same type, allowing for
+    efficient random access and insertion or removal of elements at the end of the vector.
+    """
     def __init__(self, data=None, **kwargs):
         self.elements = []
         super().__init__(data, **kwargs)
 
     def process(self):
         element_count = self.process_type('Compact<u32>').value
 
@@ -970,14 +1042,19 @@
         else:
             return [
                 sub_obj.generate_type_decomposition(_recursion_level=_recursion_level + 1, max_recursion=max_recursion)
             ]
 
 
 class BoundedVec(Vec):
+    """
+    BoundedVec is a fixed-size vector used in Substrate, with a maximum number of elements that can be added.
+    It is used in cases where a fixed-size buffer is required, such as in the case of the transaction input/output
+    limit in the Substrate runtime.
+    """
     def __init__(self, data=None, **kwargs):
 
         if self.sub_type and ',' in self.sub_type:
             # Rebuild sub_type as last item is the upper bound of elements allowed
             self.sub_type, self.max_elements = [x.strip() for x in self.sub_type.rsplit(',', 1)]
 
         super().__init__(data, **kwargs)
@@ -1125,15 +1202,17 @@
 
 
 class RawAddress(GenericAddress):
     pass
 
 
 class Enum(ScaleType):
-
+    """
+    A fixed number of variants, each mutually exclusive and potentially implying a further value or series of values.
+    """
     value_list = []
     type_mapping = None
 
     def __init__(self, data=None, value_list=None, type_mapping=None, **kwargs):
 
         self.index = None
 
@@ -1365,14 +1444,20 @@
         return self.index == 5
 
     def is_identity(self):
         return self.index == 6
 
 
 class Conviction(Enum):
+    """
+    Conviction represents a measure of the degree of confidence or trust that a stakeholder has in a particular proposal
+    in the Substrate runtime. It is used to determine the voting power of a stakeholder for a particular proposal,
+    with higher conviction leading to more voting power.
+    """
+
     CONVICTION_MASK = 0b01111111
     DEFAULT_CONVICTION = 0b00000000
 
     value_list = ['None', 'Locked1x', 'Locked2x', 'Locked3x', 'Locked4x', 'Locked5x', 'Locked6x']
 
 
 class GenericBlock(ScaleType):
@@ -1716,15 +1801,17 @@
         try:
             return self.value_object['result'][1]['data']
         except KeyError:
             return None
 
 
 class OpaqueCall(Bytes):
-
+    """
+    A Bytes representation of a `Call`, without having to decode the contents
+    """
     def process_encode(self, value):
         call_obj = self.runtime_config.create_scale_object(
             type_string='Call', metadata=self.metadata
         )
         return super().process_encode(str(call_obj.encode(value)))
 
     def process(self):
@@ -1823,15 +1910,17 @@
         multi_account_obj.signatories = sorted(account_ids)
         multi_account_obj.threshold = threshold
 
         return multi_account_obj
 
 
 class FixedLengthArray(ScaleType):
-
+    """
+    Fixed sized array of specified subtype e.g. [u8; 8]
+    """
     element_count = 0
 
     def process(self):
 
         if self.element_count:
             if self.runtime_config.get_decoder_class(self.sub_type) is U8:
                 self.value_object = self.get_next_bytes(self.element_count)
@@ -1888,14 +1977,19 @@
         sub_cls_decomp = sub_cls.generate_type_decomposition(
             _recursion_level=_recursion_level + 1, max_recursion=max_recursion
         )
         return f'[{sub_cls_decomp}; {cls.element_count}]'
 
 
 class GenericMultiAddress(Enum):
+
+    """
+    MultiAddress is a type used in the Substrate runtime to represent an address that can be expressed in multiple ways, such as an account ID, a public key, or a human-readable name, allowing for flexible addressing and storage of data.
+    """
+
     type_mapping = [
         ["Id", "AccountId"],
         ["Index", "Compact<AccountIndex>"],
         ["Raw", "HexBytes"],
         ["Address32", "H256"],
         ["Address20", "H160"],
       ]
@@ -2046,14 +2140,19 @@
         self.value_object = self.runtime_config.create_scale_object(
             type_string=self.type_mapping[0], metadata=self.metadata
         )
         return self.value_object.encode(value)
 
 
 class GenericMetadataAll(Enum):
+    """
+    Enum that contains a Metadata version.
+
+    E.g.  `{"V14": MetadataV14}`
+    """
 
     def __init__(self, data, sub_type=None, **kwargs):
         self.__call_index = {}
         self.event_index = {}
         self.error_index = {}
 
         super().__init__(data, sub_type, **kwargs)
@@ -2145,14 +2244,17 @@
                         self.error_index[f'{error_module_index}-{idx}'] = error
                     error_module_index += 1
 
         return value
 
 
 class GenericMetadataVersioned(Tuple):
+    """
+    Tuple that contains a backwards compatible MetadataAll type
+    """
 
     @property
     def call_index(self):
         return self.value_object[1].call_index
 
     @property
     def event_index(self):
@@ -2740,15 +2842,18 @@
         raise ValueError(f"Scale type '{self.sub_type}' not support")
 
     def process_encode(self, value):
         raise ValueError(f"Scale type '{self.sub_type}' not support")
 
 
 class GenericExtrinsic(ScaleType):
-
+    """
+    The Extrinsic type is used to send transactions from an account to the Substrate runtime, and it can contain
+    one or more calls to the runtime functions.
+    """
     def __init__(self, *arg, **kwargs):
         self.signed = None
         super().__init__(*arg, **kwargs)
 
     @property
     def extrinsic_hash(self):
         return blake2b(self.data.data, digest_size=32).digest()
@@ -2872,15 +2977,21 @@
 
                 self.type_mapping.append(['call', 'Call'])
 
         super().__init__(*args, **kwargs)
 
 
 class GenericEvent(Enum):
+    """
+    An Event is a type used to represent a runtime event, which is a signal that indicates that a
+    specific state transition has occurred.
 
+    It is implemented as a variant enum that contains different types of events, such as system events, runtime events,
+    and custom events, each with its own set of fields that describe the event.
+    """
     def __init__(self, *args, **kwargs):
 
         self.event_idx = None
         self.event_index = None
         self.attributes = []
         self.event = None
         self.event_module = None
```

### Comparing `scalecodec-1.2.1/scalecodec/updater.py` & `scalecodec-1.2.2/scalecodec/updater.py`

 * *Files identical despite different names*

### Comparing `scalecodec-1.2.1/scalecodec/utils/__init__.py` & `scalecodec-1.2.2/scalecodec/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `scalecodec-1.2.1/scalecodec/utils/math.py` & `scalecodec-1.2.2/scalecodec/utils/math.py`

 * *Files identical despite different names*

### Comparing `scalecodec-1.2.1/scalecodec/utils/ss58.py` & `scalecodec-1.2.2/scalecodec/utils/ss58.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,15 @@
     Parameters
     ----------
     address
     ss58_format
 
     Returns
     -------
-
+    str
     """
     checksum_prefix = b'SS58PRE'
 
     if ss58_format < 0 or ss58_format > 16383 or ss58_format in [46, 47]:
         raise ValueError("Invalid value for ss58_format")
 
     if type(address) is bytes or type(address) is bytearray:
@@ -148,15 +148,15 @@
     Parameters
     ----------
     account_index
     ss58_format
 
     Returns
     -------
-
+    str
     """
 
     if 0 <= account_index <= 2 ** 8 - 1:
         account_idx_encoder = RuntimeConfiguration().create_scale_object('u8')
     elif 2 ** 8 <= account_index <= 2 ** 16 - 1:
         account_idx_encoder = RuntimeConfiguration().create_scale_object('u16')
     elif 2 ** 16 <= account_index <= 2 ** 32 - 1:
```

### Comparing `scalecodec-1.2.1/scalecodec.egg-info/SOURCES.txt` & `scalecodec-1.2.2/scalecodec.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scalecodec-1.2.1/setup.py` & `scalecodec-1.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `scalecodec-1.2.1/test/test_extrinsic_payload.py` & `scalecodec-1.2.2/test/test_extrinsic_payload.py`

 * *Files identical despite different names*

### Comparing `scalecodec-1.2.1/test/test_metadata.py` & `scalecodec-1.2.2/test/test_metadata.py`

 * *Files identical despite different names*

### Comparing `scalecodec-1.2.1/test/test_runtime_call.py` & `scalecodec-1.2.2/test/test_runtime_call.py`

 * *Files identical despite different names*

### Comparing `scalecodec-1.2.1/test/test_runtime_configuration.py` & `scalecodec-1.2.2/test/test_runtime_configuration.py`

 * *Files identical despite different names*

### Comparing `scalecodec-1.2.1/test/test_scale_info.py` & `scalecodec-1.2.2/test/test_scale_info.py`

 * *Files identical despite different names*

### Comparing `scalecodec-1.2.1/test/test_scale_types.py` & `scalecodec-1.2.2/test/test_scale_types.py`

 * *Files identical despite different names*

### Comparing `scalecodec-1.2.1/test/test_scalebytes.py` & `scalecodec-1.2.2/test/test_scalebytes.py`

 * *Files identical despite different names*

### Comparing `scalecodec-1.2.1/test/test_ss58.py` & `scalecodec-1.2.2/test/test_ss58.py`

 * *Files identical despite different names*

### Comparing `scalecodec-1.2.1/test/test_type_encoding.py` & `scalecodec-1.2.2/test/test_type_encoding.py`

 * *Files 1% similar despite different names*

```diff
@@ -239,18 +239,29 @@
     def test_struct_encode_tuple(self):
 
         TestStruct = type('TestStruct', (Struct,), {
             'type_mapping': (('aye', 'u32'), ('nay', 'u32'))
         })
 
         obj = TestStruct()
-
         data = obj.encode((4, 2))
+
         self.assertEqual(ScaleBytes("0x0400000002000000"), data)
 
+    def test_struct_encode_int(self):
+
+        TestStruct = type('TestStruct', (Struct,), {
+            'type_mapping': (('nonce', 'u32'),)
+        })
+
+        obj = TestStruct()
+        data = obj.encode(1)
+
+        self.assertEqual(ScaleBytes("0x01000000"), data)
+
     # def test_struct_raw_encode(self):
     #     RuntimeConfiguration().update_type_registry_types({
     #         "TestKeys": {
     #             "type": "struct",
     #             "type_mapping": [
     #                 ["grandpa", "AccountId"],
     #                 ["babe", "AccountId"],
```

### Comparing `scalecodec-1.2.1/test/test_type_registry.py` & `scalecodec-1.2.2/test/test_type_registry.py`

 * *Files identical despite different names*

