# Comparing `tmp/substrate-interface-1.6.2.tar.gz` & `tmp/substrate-interface-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "substrate-interface-1.6.2.tar", last modified: Tue Mar 28 10:03:52 2023, max compression
+gzip compressed data, was "substrate-interface-1.7.0.tar", last modified: Mon May  8 13:57:05 2023, max compression
```

## Comparing `substrate-interface-1.6.2.tar` & `substrate-interface-1.7.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:03:52.567323 substrate-interface-1.6.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-28 09:56:02.000000 substrate-interface-1.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-03-28 10:03:52.567323 substrate-interface-1.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-03-28 09:56:02.000000 substrate-interface-1.6.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-28 10:03:52.567323 substrate-interface-1.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    10690 2023-03-28 09:56:02.000000 substrate-interface-1.6.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:03:52.559322 substrate-interface-1.6.2/substrate_interface.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-03-28 10:03:52.000000 substrate-interface-1.6.2/substrate_interface.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-03-28 10:03:52.000000 substrate-interface-1.6.2/substrate_interface.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 10:03:52.000000 substrate-interface-1.6.2/substrate_interface.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-03-28 10:03:52.000000 substrate-interface-1.6.2/substrate_interface.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-28 10:03:52.000000 substrate-interface-1.6.2/substrate_interface.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:03:52.563323 substrate-interface-1.6.2/substrateinterface/
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-03-28 09:56:02.000000 substrate-interface-1.6.2/substrateinterface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   126315 2023-03-28 09:56:02.000000 substrate-interface-1.6.2/substrateinterface/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-03-28 09:56:02.000000 substrate-interface-1.6.2/substrateinterface/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    35337 2023-03-28 09:56:02.000000 substrate-interface-1.6.2/substrateinterface/contracts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-03-28 09:56:02.000000 substrate-interface-1.6.2/substrateinterface/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8345 2023-03-28 09:56:02.000000 substrate-interface-1.6.2/substrateinterface/extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-03-28 09:56:02.000000 substrate-interface-1.6.2/substrateinterface/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-03-28 09:56:02.000000 substrate-interface-1.6.2/substrateinterface/key.py
--rw-r--r--   0 runner    (1001) docker     (123)    20655 2023-03-28 09:56:02.000000 substrate-interface-1.6.2/substrateinterface/keypair.py
--rw-r--r--   0 runner    (1001) docker     (123)     9857 2023-03-28 09:56:02.000000 substrate-interface-1.6.2/substrateinterface/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:03:52.563323 substrate-interface-1.6.2/substrateinterface/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-03-28 09:56:02.000000 substrate-interface-1.6.2/substrateinterface/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-03-28 09:56:02.000000 substrate-interface-1.6.2/substrateinterface/utils/caching.py
--rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-03-28 09:56:02.000000 substrate-interface-1.6.2/substrateinterface/utils/ecdsa_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-03-28 09:56:02.000000 substrate-interface-1.6.2/substrateinterface/utils/encrypted_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-03-28 09:56:02.000000 substrate-interface-1.6.2/substrateinterface/utils/hasher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-03-28 09:56:02.000000 substrate-interface-1.6.2/substrateinterface/utils/ss58.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:03:52.567323 substrate-interface-1.6.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)    16994 2023-03-28 09:56:02.000000 substrate-interface-1.6.2/test/test_block.py
--rw-r--r--   0 runner    (1001) docker     (123)    19098 2023-03-28 09:56:02.000000 substrate-interface-1.6.2/test/test_contracts.py
--rw-r--r--   0 runner    (1001) docker     (123)    16587 2023-03-28 09:56:02.000000 substrate-interface-1.6.2/test/test_create_extrinsics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-03-28 09:56:02.000000 substrate-interface-1.6.2/test/test_extension_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    19797 2023-03-28 09:56:02.000000 substrate-interface-1.6.2/test/test_helper_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4248 2023-03-28 09:56:02.000000 substrate-interface-1.6.2/test/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)    20044 2023-03-28 09:56:02.000000 substrate-interface-1.6.2/test/test_keypair.py
--rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-03-28 09:56:02.000000 substrate-interface-1.6.2/test/test_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     9730 2023-03-28 09:56:02.000000 substrate-interface-1.6.2/test/test_query_map.py
--rw-r--r--   0 runner    (1001) docker     (123)    11188 2023-03-28 09:56:02.000000 substrate-interface-1.6.2/test/test_rpc_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-03-28 09:56:02.000000 substrate-interface-1.6.2/test/test_runtime_call.py
--rw-r--r--   0 runner    (1001) docker     (123)     9374 2023-03-28 09:56:02.000000 substrate-interface-1.6.2/test/test_ss58.py
--rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-03-28 09:56:02.000000 substrate-interface-1.6.2/test/test_subscriptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7721 2023-03-28 09:56:02.000000 substrate-interface-1.6.2/test/test_type_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:57:05.599689 substrate-interface-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-08 13:51:40.000000 substrate-interface-1.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-05-08 13:57:05.599689 substrate-interface-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-05-08 13:51:40.000000 substrate-interface-1.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 13:57:05.599689 substrate-interface-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    10690 2023-05-08 13:51:40.000000 substrate-interface-1.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:57:05.595689 substrate-interface-1.7.0/substrate_interface.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-05-08 13:57:05.000000 substrate-interface-1.7.0/substrate_interface.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-05-08 13:57:05.000000 substrate-interface-1.7.0/substrate_interface.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 13:57:05.000000 substrate-interface-1.7.0/substrate_interface.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-08 13:57:05.000000 substrate-interface-1.7.0/substrate_interface.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-08 13:57:05.000000 substrate-interface-1.7.0/substrate_interface.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:57:05.599689 substrate-interface-1.7.0/substrateinterface/
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-08 13:51:40.000000 substrate-interface-1.7.0/substrateinterface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   126315 2023-05-08 13:51:40.000000 substrate-interface-1.7.0/substrateinterface/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-08 13:51:40.000000 substrate-interface-1.7.0/substrateinterface/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31151 2023-05-08 13:51:40.000000 substrate-interface-1.7.0/substrateinterface/contracts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-08 13:51:40.000000 substrate-interface-1.7.0/substrateinterface/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8345 2023-05-08 13:51:40.000000 substrate-interface-1.7.0/substrateinterface/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-05-08 13:51:40.000000 substrate-interface-1.7.0/substrateinterface/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-05-08 13:51:40.000000 substrate-interface-1.7.0/substrateinterface/key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20655 2023-05-08 13:51:40.000000 substrate-interface-1.7.0/substrateinterface/keypair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9857 2023-05-08 13:51:40.000000 substrate-interface-1.7.0/substrateinterface/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:57:05.599689 substrate-interface-1.7.0/substrateinterface/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-08 13:51:40.000000 substrate-interface-1.7.0/substrateinterface/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-05-08 13:51:40.000000 substrate-interface-1.7.0/substrateinterface/utils/caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-05-08 13:51:40.000000 substrate-interface-1.7.0/substrateinterface/utils/ecdsa_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-05-08 13:51:40.000000 substrate-interface-1.7.0/substrateinterface/utils/encrypted_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-05-08 13:51:40.000000 substrate-interface-1.7.0/substrateinterface/utils/hasher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-08 13:51:40.000000 substrate-interface-1.7.0/substrateinterface/utils/ss58.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:57:05.599689 substrate-interface-1.7.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    16994 2023-05-08 13:51:40.000000 substrate-interface-1.7.0/test/test_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17149 2023-05-08 13:51:40.000000 substrate-interface-1.7.0/test/test_contracts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16587 2023-05-08 13:51:40.000000 substrate-interface-1.7.0/test/test_create_extrinsics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-05-08 13:51:40.000000 substrate-interface-1.7.0/test/test_extension_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19797 2023-05-08 13:51:40.000000 substrate-interface-1.7.0/test/test_helper_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4248 2023-05-08 13:51:40.000000 substrate-interface-1.7.0/test/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20044 2023-05-08 13:51:40.000000 substrate-interface-1.7.0/test/test_keypair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-05-08 13:51:40.000000 substrate-interface-1.7.0/test/test_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9730 2023-05-08 13:51:40.000000 substrate-interface-1.7.0/test/test_query_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11188 2023-05-08 13:51:40.000000 substrate-interface-1.7.0/test/test_rpc_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-05-08 13:51:40.000000 substrate-interface-1.7.0/test/test_runtime_call.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9374 2023-05-08 13:51:40.000000 substrate-interface-1.7.0/test/test_ss58.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-05-08 13:51:40.000000 substrate-interface-1.7.0/test/test_subscriptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7721 2023-05-08 13:51:40.000000 substrate-interface-1.7.0/test/test_type_registry.py
```

### Comparing `substrate-interface-1.6.2/LICENSE` & `substrate-interface-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.6.2/PKG-INFO` & `substrate-interface-1.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: substrate-interface
-Version: 1.6.2
+Version: 1.7.0
 Summary: Library for interfacing with a Substrate node
 Home-page: https://github.com/polkascan/py-substrate-interface
 Author: Stichting Polkascan (Polkascan Foundation)
 Author-email: info@polkascan.org
 License: UNKNOWN
 Description: # Python Substrate Interface
```

### Comparing `substrate-interface-1.6.2/README.md` & `substrate-interface-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.6.2/setup.py` & `substrate-interface-1.7.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -184,15 +184,15 @@
         'requests>=2.21.0,<3',
         'xxhash>=1.3.0,<4',
         'ecdsa>=0.17.0,<1',
         'eth-keys>=0.2.1,<1',
         'eth_utils>=1.3.0,<3',
         'pycryptodome>=3.11.0,<4',
         'PyNaCl>=1.0.1,<2',
-        'scalecodec>=1.2.2,<1.3',
+        'scalecodec>=1.2.3,<1.3',
         'py-sr25519-bindings>=0.2.0,<1',
         'py-ed25519-zebra-bindings>=1.0,<2',
         'py-bip39-bindings>=0.1.9,<1'
     ],
 
     # List additional groups of dependencies here (e.g. development
     # dependencies). Users will be able to install these using the "extras"
```

### Comparing `substrate-interface-1.6.2/substrate_interface.egg-info/PKG-INFO` & `substrate-interface-1.7.0/substrate_interface.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: substrate-interface
-Version: 1.6.2
+Version: 1.7.0
 Summary: Library for interfacing with a Substrate node
 Home-page: https://github.com/polkascan/py-substrate-interface
 Author: Stichting Polkascan (Polkascan Foundation)
 Author-email: info@polkascan.org
 License: UNKNOWN
 Description: # Python Substrate Interface
```

### Comparing `substrate-interface-1.6.2/substrate_interface.egg-info/SOURCES.txt` & `substrate-interface-1.7.0/substrate_interface.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.6.2/substrateinterface/__init__.py` & `substrate-interface-1.7.0/substrateinterface/__init__.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.6.2/substrateinterface/base.py` & `substrate-interface-1.7.0/substrateinterface/base.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.6.2/substrateinterface/constants.py` & `substrate-interface-1.7.0/substrateinterface/constants.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.6.2/substrateinterface/contracts.py` & `substrate-interface-1.7.0/substrateinterface/contracts.py`

 * *Files 6% similar despite different names*

```diff
@@ -617,96 +617,67 @@
             }
         )
 
         extrinsic = self.substrate.create_signed_extrinsic(call=call, keypair=keypair)
 
         return self.substrate.submit_extrinsic(extrinsic, wait_for_inclusion=True)
 
-    def deploy(self, keypair: Keypair, endowment: int, gas_limit: int, constructor: str, args: dict = None,
+    def deploy(self, keypair: Keypair, constructor: str, args: dict = None, value: int = 0, gas_limit: dict = None,
                deployment_salt: str = None, upload_code: bool = False, storage_deposit_limit: int = None
                ) -> "ContractInstance":
         """
         Deploys a new instance of the contract after it has been uploaded on-chain, with provided constructor and
         constructor arguments
 
         Parameters
         ----------
         keypair
-        endowment: Initial deposit for the newly created contract address
-        gas_limit:
         constructor: name of the constructor to use, provided in the metadata
         args: arguments for the constructor
+        value: Value sent to created contract address
+        gas_limit: Gas limit as WeightV2 type. Will default to {'ref_time': 25990000000, 'proof_size': 11990383647911208550}.
         deployment_salt: optional string or hex-string that acts as a salt for this deployment
         upload_code: When True the WASM blob itself will be uploaded with the deploy, False if the WASM is already present on-chain
         storage_deposit_limit: The maximum amount of balance that can be charged to pay for the storage consumed.
 
         Returns
         -------
         ContractInstance
         """
 
         # Lookup constructor
         data = self.metadata.generate_constructor_data(name=constructor, args=args)
 
-        # Check metadata for available call functions
-        call_function = self.substrate.get_metadata_call_function('Contracts', 'instantiate_with_code')
-        if call_function is not None:
-
-            # Check gas_limit weight format
-            param_info = call_function.get_param_info()
-            if type(param_info['gas_limit']) is dict:
-                gas_limit = {'ref_time': gas_limit, 'proof_size': 0}
-
+        if gas_limit is None:
+            gas_limit = {'ref_time': 25990000000, 'proof_size': 11990383647911208550}
 
         if upload_code is True:
 
-            if call_function is not None:
-
-                if not self.wasm_bytes:
-                    raise ValueError("No WASM bytes to upload")
-
-                call = self.substrate.compose_call(
-                    call_module='Contracts',
-                    call_function='instantiate_with_code',
-                    call_params={
-                        'endowment': endowment,  # deprecated
-                        'value': endowment,
-                        'gas_limit': gas_limit,
-                        'storage_deposit_limit': storage_deposit_limit,
-                        'code': '0x{}'.format(self.wasm_bytes.hex()),
-                        'data': data.to_hex(),
-                        'salt': deployment_salt or ''
-                    }
-                )
-            else:
-                # Legacy mode: put code in separate call
-
-                self.upload_wasm(keypair)
+            if not self.wasm_bytes:
+                raise ValueError("No WASM bytes to upload")
 
-                call = self.substrate.compose_call(
-                    call_module='Contracts',
-                    call_function='instantiate',
-                    call_params={
-                        'endowment': endowment,  # deprecated
-                        'value': endowment,
-                        'gas_limit': gas_limit,
-                        'storage_deposit_limit': storage_deposit_limit,
-                        'code_hash': f'0x{self.code_hash.hex()}',
-                        'data': data.to_hex(),
-                        'salt': deployment_salt or ''
-                    }
-                )
+            call = self.substrate.compose_call(
+                call_module='Contracts',
+                call_function='instantiate_with_code',
+                call_params={
+                    'value': value,
+                    'gas_limit': gas_limit,
+                    'storage_deposit_limit': storage_deposit_limit,
+                    'code': '0x{}'.format(self.wasm_bytes.hex()),
+                    'data': data.to_hex(),
+                    'salt': deployment_salt or ''
+                }
+            )
         else:
 
             call = self.substrate.compose_call(
                 call_module='Contracts',
                 call_function='instantiate',
                 call_params={
-                    'endowment': endowment,  # deprecated
-                    'value': endowment,
+                    'value': value,
                     'gas_limit': gas_limit,
                     'storage_deposit_limit': storage_deposit_limit,
                     'code_hash': f'0x{self.code_hash.hex()}',
                     'data': data.to_hex(),
                     'salt': deployment_salt or ''
                 }
             )
@@ -778,134 +749,63 @@
 
         Parameters
         ----------
         keypair
         method: name of message to execute
         args: arguments of message in {'name': value} format
         value: value to send when executing the message
-        gas_limit:
+        gas_limit: dict repesentation of `WeightV2` type
 
         Returns
         -------
         GenericContractExecResult
         """
 
         input_data = self.metadata.generate_message_data(name=method, args=args)
 
-        if self.substrate.supports_rpc_method('state_call'):
-            call_result = self.substrate.runtime_call("ContractsApi", "call", {
-                'dest': self.contract_address,
-                'gas_limit': gas_limit,
-                'input_data': input_data.to_hex(),
-                'origin': keypair.ss58_address,
-                'value': value,
-                'storage_deposit_limit': None
-            })
-            if 'Error' in call_result['result']:
-                raise ContractReadFailedException(call_result.value['result']['Error'])
-
-            if 'Ok' in call_result['result']:
-
-                try:
-                    return_type_string = self.metadata.get_return_type_string_for_message(method)
-                    result_scale_obj = self.substrate.create_scale_object(return_type_string)
-                    result_scale_obj.decode(ScaleBytes(call_result['result'][1]['data'].value_object))
-                    call_result.value_object['result'].value_object[1].value_object['data'] = result_scale_obj
-                    call_result.value['result']['Ok']['data'] = result_scale_obj.value
-
-                except NotImplementedError:
-                    pass
-
-            return call_result
-
-        else:
-            # Deprecated RPC call
-            response = self.substrate.rpc_request(method='contracts_call', params=[{
-                'dest': self.contract_address,
-                'gasLimit': gas_limit,
-                'inputData': input_data.to_hex(),
-                'origin': keypair.ss58_address,
-                'value': value
-            }])
-
-            if 'result' in response:
+        # Execute runtime call in ContractsApi
+        call_result = self.substrate.runtime_call("ContractsApi", "call", {
+            'dest': self.contract_address,
+            'gas_limit': gas_limit,
+            'input_data': input_data.to_hex(),
+            'origin': keypair.ss58_address,
+            'value': value,
+            'storage_deposit_limit': None
+        })
+        if 'Error' in call_result['result']:
+            raise ContractReadFailedException(call_result.value['result']['Error'])
 
-                self.substrate.init_runtime()
+        if 'Ok' in call_result['result']:
 
+            try:
                 return_type_string = self.metadata.get_return_type_string_for_message(method)
+                result_scale_obj = self.substrate.create_scale_object(return_type_string)
+                result_scale_obj.decode(ScaleBytes(call_result['result'][1]['data'].value_object))
+                call_result.value_object['result'].value_object[1].value_object['data'] = result_scale_obj
+                call_result.value['result']['Ok']['data'] = result_scale_obj.value
 
-                # Wrap the result in a ContractExecResult Enum because the exec will result in the same
-                ContractExecResult = self.substrate.runtime_config.get_decoder_class('ContractExecResult')
-
-                contract_exec_result = ContractExecResult(contract_result_scale_type=return_type_string)
-
-                if 'result' in response['result']:
-
-                    contract_exec_result.gas_consumed = response['result']['gasConsumed']
-                    contract_exec_result.gas_required = response['result']['gasRequired']
-
-                    if 'Ok' in response['result']['result']:
-
-                        contract_exec_result.flags = response['result']['result']['Ok']['flags']
-
-                        try:
-
-                            result_scale_obj = self.substrate.decode_scale(
-                                type_string=return_type_string,
-                                scale_bytes=ScaleBytes(response['result']['result']['Ok']['data']),
-                                return_scale_obj=True
-                            )
-
-                            response['result']['result']['Ok']['data'] = result_scale_obj.value
-                            contract_exec_result.contract_result_data = result_scale_obj
-                            contract_exec_result.value_object = result_scale_obj
+            except NotImplementedError:
+                pass
 
-                        except NotImplementedError:
-                            pass
-
-                # Backwards compatibility
-                elif 'success' in response['result']:
-
-                    contract_exec_result.gas_consumed = response['result']['success']['gas_consumed']
-                    contract_exec_result.flags = response['result']['success']['flags']
-
-                    try:
-
-                        result_scale_obj = self.substrate.decode_scale(
-                            type_string=return_type_string,
-                            scale_bytes=ScaleBytes(response['result']['success']['data']),
-                            return_scale_obj=True
-                        )
-
-                        response['result']['success']['data'] = result_scale_obj.value
-                        contract_exec_result.contract_result_data = result_scale_obj
-
-                    except NotImplementedError:
-                        pass
-
-                contract_exec_result.value = response['result']
-
-                return contract_exec_result
-
-            raise ContractReadFailedException(response)
+        return call_result
 
     def exec(self, keypair: Keypair, method: str, args: dict = None,
-             value: int = 0, gas_limit: Optional[int] = None, storage_deposit_limit: int = None
+             value: int = 0, gas_limit: Optional[dict] = None, storage_deposit_limit: int = None
              ) -> ContractExecutionReceipt:
         """
         Executes provided message by creating and submitting an extrinsic. To get a gas prediction or perform a
         'dry-run' of executing this message, see `ContractInstance.read`.
 
         Parameters
         ----------
         keypair
         method: name of message to execute
         args: arguments of message in {'name': value} format
         value: value to send when executing the message
-        gas_limit: When left to None the gas limit will be calculated with a read()
+        gas_limit: dict repesentation of `WeightV2` type. When omited the gas limit will be calculated with a `read()`
         storage_deposit_limit: The maximum amount of balance that can be charged to pay for the storage consumed
 
         Returns
         -------
         ContractExecutionReceipt
         """
 
@@ -928,8 +828,7 @@
         )
 
         extrinsic = self.substrate.create_signed_extrinsic(call=call, keypair=keypair)
 
         receipt = self.substrate.submit_extrinsic(extrinsic, wait_for_inclusion=True)
 
         return ContractExecutionReceipt.create_from_extrinsic_receipt(receipt, self.metadata)
-
```

### Comparing `substrate-interface-1.6.2/substrateinterface/exceptions.py` & `substrate-interface-1.7.0/substrateinterface/exceptions.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.6.2/substrateinterface/extensions.py` & `substrate-interface-1.7.0/substrateinterface/extensions.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.6.2/substrateinterface/interfaces.py` & `substrate-interface-1.7.0/substrateinterface/interfaces.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.6.2/substrateinterface/key.py` & `substrate-interface-1.7.0/substrateinterface/key.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.6.2/substrateinterface/keypair.py` & `substrate-interface-1.7.0/substrateinterface/keypair.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.6.2/substrateinterface/storage.py` & `substrate-interface-1.7.0/substrateinterface/storage.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.6.2/substrateinterface/utils/__init__.py` & `substrate-interface-1.7.0/substrateinterface/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.6.2/substrateinterface/utils/caching.py` & `substrate-interface-1.7.0/substrateinterface/utils/caching.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.6.2/substrateinterface/utils/ecdsa_helpers.py` & `substrate-interface-1.7.0/substrateinterface/utils/ecdsa_helpers.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.6.2/substrateinterface/utils/encrypted_json.py` & `substrate-interface-1.7.0/substrateinterface/utils/encrypted_json.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.6.2/substrateinterface/utils/hasher.py` & `substrate-interface-1.7.0/substrateinterface/utils/hasher.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.6.2/substrateinterface/utils/ss58.py` & `substrate-interface-1.7.0/substrateinterface/utils/ss58.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.6.2/test/test_block.py` & `substrate-interface-1.7.0/test/test_block.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.6.2/test/test_contracts.py` & `substrate-interface-1.7.0/test/test_contracts.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,19 +13,17 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
 import unittest
 
-from scalecodec.base import ScaleBytes
-from substrateinterface import SubstrateInterface, ContractMetadata, ContractInstance, Keypair
-from substrateinterface.contracts import ContractEvent
+from scalecodec import ScaleBytes
+from substrateinterface import SubstrateInterface, ContractMetadata, ContractInstance, Keypair, ContractEvent
 from substrateinterface.exceptions import ContractMetadataParseException
-from substrateinterface.utils.ss58 import ss58_encode
 from test import settings
 
 
 class ContractMetadataTestCase(unittest.TestCase):
 
     @classmethod
     def setUpClass(cls):
@@ -274,89 +272,22 @@
 
             ContractMetadata.create_from_file(
                 metadata_file=os.path.join(os.path.dirname(__file__), 'fixtures', 'unsupported_type_metadata.json'),
                 substrate=self.substrate
             )
 
 
-class ContractInstanceTestCase(unittest.TestCase):
-
-    @classmethod
-    def setUpClass(cls):
-
-        class MockedSubstrateInterface(SubstrateInterface):
-
-            def rpc_request(self, method, params, result_handler=None):
-                if method == 'rpc_methods':
-                    response = super().rpc_request(method, params, result_handler)
-                    response['result']['methods'].remove('state_call')
-                    return response
-                if method == 'contracts_call':
-                    return {
-                        'jsonrpc': '2.0',
-                        'result': {
-                            'success': {
-                                'data': '0x000064a7b3b6e00d0000000000000000', 'flags': 0, 'gas_consumed': 2616500000
-                            }
-                         }, 'id': self.request_id
-                    }
-
-                return super().rpc_request(method, params, result_handler)
-
-        cls.substrate = MockedSubstrateInterface(url=settings.KUSAMA_NODE_URL, type_registry_preset='kusama')
-
-        cls.keypair = Keypair.create_from_uri('//Alice')
-
-    def setUp(self) -> None:
-        self.contract = ContractInstance.create_from_address(
-            contract_address="5FV9cnzFc2tDrWcDkmoup7VZWpH9HrTaw8STnWpAQqT7KvUK",
-            metadata_file=os.path.join(os.path.dirname(__file__), 'fixtures', 'erc20-v0.json'),
-            substrate=self.substrate
-        )
-
-    def test_instance_read(self):
-
-        result = self.contract.read(self.keypair, 'total_supply')
-
-        self.assertEqual(1000000000000000000, result.contract_result_data.value)
-
-    def test_instance_read_with_args(self):
-
-        result = self.contract.read(self.keypair, 'balance_of',
-                                    args={'owner': '5GrwvaEF5zXb26Fz9rcQpDWS57CtERHpNehXCPcNoHGKutQY'})
-
-        self.assertEqual(1000000000000000000, result.contract_result_data.value)
-
-
-class ContractInstanceV1TestCase(ContractInstanceTestCase):
-    def setUp(self) -> None:
-        self.contract = ContractInstance.create_from_address(
-            contract_address="5FV9cnzFc2tDrWcDkmoup7VZWpH9HrTaw8STnWpAQqT7KvUK",
-            metadata_file=os.path.join(os.path.dirname(__file__), 'fixtures', 'erc20-v1.json'),
-            substrate=self.substrate
-        )
-
-
 class ContractMetadataV3TestCase(ContractMetadataV1TestCase):
     def setUp(self) -> None:
         self.contract_metadata = ContractMetadata.create_from_file(
             metadata_file=os.path.join(os.path.dirname(__file__), 'fixtures', 'erc20-v3.json'),
             substrate=self.substrate
         )
 
 
-class ContractInstanceV3TestCase(ContractInstanceTestCase):
-    def setUp(self) -> None:
-        self.contract = ContractInstance.create_from_address(
-            contract_address="5FV9cnzFc2tDrWcDkmoup7VZWpH9HrTaw8STnWpAQqT7KvUK",
-            metadata_file=os.path.join(os.path.dirname(__file__), 'fixtures', 'erc20-v3.json'),
-            substrate=self.substrate
-        )
-
-
 class FlipperMetadataV3TestCase(unittest.TestCase):
 
     @classmethod
     def setUpClass(cls):
         cls.substrate = SubstrateInterface(url=settings.KUSAMA_NODE_URL)
 
     def setUp(self) -> None:
@@ -364,14 +295,21 @@
             metadata_file=os.path.join(os.path.dirname(__file__), 'fixtures', 'flipper-v3.json'),
             substrate=self.substrate
         )
 
     def test_metadata_parsed(self):
         self.assertNotEqual(self.contract_metadata.metadata_dict, {})
 
+    def test_incorrect_metadata_file(self):
+        with self.assertRaises(ContractMetadataParseException):
+            ContractMetadata.create_from_file(
+                metadata_file=os.path.join(os.path.dirname(__file__), 'fixtures', 'incorrect_metadata.json'),
+                substrate=self.substrate
+            )
+
     def test_extract_typestring_from_types(self):
         self.assertEqual(
             'ink::0xf051c631190ac47f82e280ba763df932210f6e2447978e24cbe0dcc6d6903c7a::0',
             self.contract_metadata.get_type_string_for_metadata_type(0)
         )
 
     def test_contract_types_added_type_registry(self):
@@ -392,14 +330,26 @@
         self.assertEqual('0x9bae9d5e01', scale_data.to_hex())
 
     def test_generate_message_data(self):
 
         scale_data = self.contract_metadata.generate_message_data("get")
         self.assertEqual('0x2f865bd9', scale_data.to_hex())
 
+    def test_invalid_constructor_name(self):
+        with self.assertRaises(ValueError) as cm:
+            self.contract_metadata.generate_constructor_data("invalid")
+
+        self.assertEqual('Constructor "invalid" not found', str(cm.exception))
+
+    def test_invalid_message_name(self):
+        with self.assertRaises(ValueError) as cm:
+            self.contract_metadata.generate_message_data("invalid_msg_name")
+
+        self.assertEqual('Message "invalid_msg_name" not found', str(cm.exception))
+
 
 class FlipperInstanceTestCase(unittest.TestCase):
 
     @classmethod
     def setUpClass(cls):
 
         class MockedSubstrateInterface(SubstrateInterface):
```

### Comparing `substrate-interface-1.6.2/test/test_create_extrinsics.py` & `substrate-interface-1.7.0/test/test_create_extrinsics.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.6.2/test/test_extension_interface.py` & `substrate-interface-1.7.0/test/test_extension_interface.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.6.2/test/test_helper_functions.py` & `substrate-interface-1.7.0/test/test_helper_functions.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.6.2/test/test_init.py` & `substrate-interface-1.7.0/test/test_init.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.6.2/test/test_keypair.py` & `substrate-interface-1.7.0/test/test_keypair.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.6.2/test/test_query.py` & `substrate-interface-1.7.0/test/test_query.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.6.2/test/test_query_map.py` & `substrate-interface-1.7.0/test/test_query_map.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.6.2/test/test_rpc_compatibility.py` & `substrate-interface-1.7.0/test/test_rpc_compatibility.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.6.2/test/test_runtime_call.py` & `substrate-interface-1.7.0/test/test_runtime_call.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.6.2/test/test_ss58.py` & `substrate-interface-1.7.0/test/test_ss58.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.6.2/test/test_subscriptions.py` & `substrate-interface-1.7.0/test/test_subscriptions.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.6.2/test/test_type_registry.py` & `substrate-interface-1.7.0/test/test_type_registry.py`

 * *Files identical despite different names*

